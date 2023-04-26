# Comparing `tmp/airflow_metrics_gbq-0.0.4a0.tar.gz` & `tmp/airflow_metrics_gbq-0.0.4a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airflow_metrics_gbq-0.0.4a0.tar", max compression
+gzip compressed data, was "airflow_metrics_gbq-0.0.4a1.tar", max compression
```

## Comparing `airflow_metrics_gbq-0.0.4a0.tar` & `airflow_metrics_gbq-0.0.4a1.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1296 2023-04-20 22:07:21.054985 airflow_metrics_gbq-0.0.4a0/LICENSE
--rw-r--r--   0        0        0     2549 2023-04-20 22:07:21.054985 airflow_metrics_gbq-0.0.4a0/README.md
--rw-r--r--   0        0        0        0 2023-04-20 22:07:21.054985 airflow_metrics_gbq-0.0.4a0/airflow_metrics_gbq/__init__.py
--rw-r--r--   0        0        0     7541 2023-04-20 22:07:21.054985 airflow_metrics_gbq-0.0.4a0/airflow_metrics_gbq/metrics.py
--rw-r--r--   0        0        0      700 2023-04-20 22:07:21.054985 airflow_metrics_gbq-0.0.4a0/airflow_metrics_gbq/utils/__init__.py
--rw-r--r--   0        0        0     1674 2023-04-20 22:07:21.054985 airflow_metrics_gbq-0.0.4a0/airflow_metrics_gbq/utils/gbq_connector.py
--rw-r--r--   0        0        0     1300 2023-04-20 22:07:21.058985 airflow_metrics_gbq-0.0.4a0/pyproject.toml
--rw-r--r--   0        0        0     3737 1970-01-01 00:00:00.000000 airflow_metrics_gbq-0.0.4a0/PKG-INFO
+-rw-r--r--   0        0        0     1296 2023-04-26 17:11:40.271869 airflow_metrics_gbq-0.0.4a1/LICENSE
+-rw-r--r--   0        0        0     2549 2023-04-26 17:11:40.271869 airflow_metrics_gbq-0.0.4a1/README.md
+-rw-r--r--   0        0        0        0 2023-04-26 17:11:40.271869 airflow_metrics_gbq-0.0.4a1/airflow_metrics_gbq/__init__.py
+-rw-r--r--   0        0        0       94 2023-04-26 17:11:40.271869 airflow_metrics_gbq-0.0.4a1/airflow_metrics_gbq/exceptions.py
+-rw-r--r--   0        0        0    10537 2023-04-26 17:11:40.271869 airflow_metrics_gbq-0.0.4a1/airflow_metrics_gbq/metrics.py
+-rw-r--r--   0        0        0      700 2023-04-26 17:11:40.271869 airflow_metrics_gbq-0.0.4a1/airflow_metrics_gbq/utils/__init__.py
+-rw-r--r--   0        0        0     1674 2023-04-26 17:11:40.271869 airflow_metrics_gbq-0.0.4a1/airflow_metrics_gbq/utils/gbq_connector.py
+-rw-r--r--   0        0        0     1320 2023-04-26 17:11:40.271869 airflow_metrics_gbq-0.0.4a1/pyproject.toml
+-rw-r--r--   0        0        0     3778 1970-01-01 00:00:00.000000 airflow_metrics_gbq-0.0.4a1/PKG-INFO
```

### Comparing `airflow_metrics_gbq-0.0.4a0/LICENSE` & `airflow_metrics_gbq-0.0.4a1/LICENSE`

 * *Files identical despite different names*

### Comparing `airflow_metrics_gbq-0.0.4a0/README.md` & `airflow_metrics_gbq-0.0.4a1/README.md`

 * *Files identical despite different names*

### Comparing `airflow_metrics_gbq-0.0.4a0/airflow_metrics_gbq/metrics.py` & `airflow_metrics_gbq-0.0.4a1/airflow_metrics_gbq/metrics.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,45 @@
+import concurrent.futures
+import multiprocessing
 import os
 import socket
 import time
-import random
-from typing import Optional
+import threading
+import queue
+from queue import Queue
+from concurrent.futures import ThreadPoolExecutor
+import atexit
+import typing as t
 from enum import Enum, unique
 from collections import defaultdict
 from dataclasses import dataclass
 import pandas as pd
+from tenacity import (
+    retry,
+    retry_if_exception_type,
+    wait_fixed,
+    wait_random,
+    stop_after_attempt,
+)
 
 from airflow_metrics_gbq.utils import GoogleBigQueryConnector, setup_gcloud_logging
+from airflow_metrics_gbq.exceptions import NoMetricFoundException
 
 
 # pylint: disable=too-few-public-methods
 @dataclass
 class Point:
     """Represents a single metric record"""
 
     app: str
     domain: str
     value: float
     timestamp: float
-    check: Optional[str] = None
-    name: Optional[str] = None
+    check: t.Optional[str] = None
+    name: t.Optional[str] = None
 
 
 @unique
 class Measure(Enum):
     """Type of measure"""
 
     COUNT = "count"
@@ -78,58 +92,134 @@
                 ".".join(fields[3:]),
             )
         else:
             raise RuntimeError("Unknown measure encountered!", record)
         return PointWithType(point, mtype)
 
 
-# TODO: Run in separate process
 # pylint: disable=too-many-instance-attributes
 class AirflowMonitor:
     """Main class to ship metrics to GBQ"""
 
-    CAPACITY = 500
+    CAPACITY: t.Final = 500
+    BATCH_TIME: t.Final = 5
 
     def __init__(
         self,
         host: str,
         port: int,
         gcp_credentials: str,
         dataset_id: str,
         counts_table: str,
         last_table: str,
         timers_table: str,
+        num_threads: int = (multiprocessing.cpu_count() // 2),
     ):
         self.dataset_id = dataset_id
         self.counts_table = counts_table
         self.last_table = last_table
         self.timers_table = timers_table
         os.environ["GOOGLE_APPLICATION_CREDENTIALS"] = gcp_credentials
         self.gbq_connector = GoogleBigQueryConnector(gcp_credentials)
         self.logger = setup_gcloud_logging("airflow_monitoring", gcp_credentials)
-        self._buffer = []
-        self._current = 0
+        # track batch time
+        self._last_flush = time.time()
+        # buffer
+        self.pool = ThreadPoolExecutor(max_workers=num_threads)
+        self._metrics = []
+        self._buffer = Queue(maxsize=self.CAPACITY + 50)
+        self.monitor_batch = threading.Event()
+        self.monitor_batch.set()
+        self.pool.submit(self.monitor).add_done_callback(self.callback)
+
+        # Flush running
+        self.is_flush_running = threading.Event()
+        self.is_flush_running.clear()
+
+        # Fetch into queue from socket
+        self.pool.submit(self._fetch).add_done_callback(self.callback)
+
+        # Metrics connection
         self._sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
         self._sock.bind((host, port))
 
+        atexit.register(self.close)
+
+    def monitor(self):
+        """Monitor batch time for flushing metrics"""
+        while self.monitor_batch.is_set():
+            if not self.is_flush_running.is_set():
+                self.is_flush_running.set()
+                if time.time() - self._last_flush > self.BATCH_TIME:
+                    if not self._buffer.empty():
+                        self.logger.info("Flushing queue, batch time exceeded")
+                        self.flush_queue()
+                self.is_flush_running.clear()
+            time.sleep(self.BATCH_TIME)
+
+    @staticmethod
+    def callback(future: concurrent.futures.Future):
+        """Future callback"""
+        exc = future.exception()
+        if exc:
+            raise exc
+
+    def close(self):
+        """Cleanup resources at exit"""
+        self.logger.debug("Closing exporter")
+        self.flush_queue()
+        self.monitor_batch.clear()
+        self.is_flush_running.clear()
+        self.pool.shutdown()
+        self.logger.debug("Done")
+
+    def run(self):
+        """Entrypoint to flush the queue to BigQuery based on num. records"""
+        while True:
+            if self._buffer.qsize() >= self.CAPACITY and not self.is_flush_running.is_set():
+                self.is_flush_running.set()
+                self.flush_queue()
+                self.is_flush_running.clear()
+            time.sleep(1)
+
+    def flush_queue(self):
+        """Flush the queue to BigQuery"""
+        metrics = []
+
+        while not self._buffer.empty() and len(metrics) <= self.CAPACITY:
+            metrics.append(self._buffer.get())
+
+        if metrics:
+            self.logger.debug(f"Flushing out {len(metrics)} metrics to BigQuery")
+            self.send_metrics(metrics)
+            self._last_flush = time.time()
+
+    @retry(
+        retry=(retry_if_exception_type(queue.Full) | retry_if_exception_type(NoMetricFoundException)),
+        wait=wait_fixed(2) + wait_random(0, 2),
+        stop=stop_after_attempt(5),
+    )
     def _fetch(self):
-        self._current = 0
-        self._buffer = []
-        while self._current <= self.CAPACITY:
-            # TODO: Add error handling if empty buffer or df, time based buffer
+        """Fetch metrics from Airflow"""
+        while True:
             measure: str = self._sock.recv(1024).decode("utf-8")
+
+            if measure == "":
+                raise NoMetricFoundException("No metrics detected!")
+
             try:
-                self._buffer.append(PointWithType.from_record(measure))
-                self._current += 1
-            except IndexError as e:
-                self.logger.error(f"Seems like there is no record, measure: {measure}, error: {e}")
-
-    def _get_dfs(self) -> (pd.DataFrame, pd.DataFrame, pd.DataFrame):
-        self._fetch()
-        measure_dict = self._part_types()
+                # non blocking
+                self._buffer.put_nowait(PointWithType.from_record(measure))
+            except queue.Full as e:
+                self.logger.error("Queue is full")
+                raise e
+
+    def _get_dfs(self, metrics: t.List[PointWithType]) -> (pd.DataFrame, pd.DataFrame, pd.DataFrame):
+        """Get dataframes to upload"""
+        measure_dict = self._part_types(metrics)
 
         df_counts, df_last, df_timer = pd.DataFrame(), pd.DataFrame(), pd.DataFrame()
 
         if len(measure_dict["count"]) > 0:
             df_counts = (
                 pd.DataFrame([record.__dict__ for record in measure_dict["count"]])
                 .groupby(["app", "domain", "check", "name"], dropna=False)
@@ -153,44 +243,43 @@
                     df_timer["domain"].isin(["dagrun"])
                     & df_timer["name"].apply(lambda x: x.startswith("success") or x.startswith("failed") if x is not None else False)
                 )
             ]
         self.logger.info(f"Dimensions: \nCounts: {len(df_counts)} \nLast: {len(df_last)} \nTimers: {len(df_timer)}")
         return df_counts, df_last, df_timer
 
-    def run(self):
+    def send_metrics(self, metrics: t.List[PointWithType]):
         """Entrypoint to run a continuous loop"""
 
-        while True:
-            time.sleep(random.randint(1, 5))
-            df_counts, df_last, df_timer = self._get_dfs()
-            df_counts = self.fix_pd_to_bq_types(df_counts, self.dataset_id, self.counts_table)
-            df_last = self.fix_pd_to_bq_types(df_last, self.dataset_id, self.last_table)
-            df_timer = self.fix_pd_to_bq_types(df_timer, self.dataset_id, self.timers_table)
+        df_counts, df_last, df_timer = self._get_dfs(metrics)
+        df_counts = self.fix_pd_to_bq_types(df_counts, self.dataset_id, self.counts_table)
+        df_last = self.fix_pd_to_bq_types(df_last, self.dataset_id, self.last_table)
+        df_timer = self.fix_pd_to_bq_types(df_timer, self.dataset_id, self.timers_table)
 
-            self.logger.info("Uploading datasets to GBQ")
+        self.logger.debug("Uploading datasets to GBQ")
 
-            if not df_counts.empty:
-                self.gbq_connector.upload_data(df_counts, self.counts_table, self.dataset_id)
+        if not df_counts.empty:
+            self.gbq_connector.upload_data(df_counts, self.counts_table, self.dataset_id)
 
-            if not df_last.empty:
-                self.gbq_connector.upload_data(df_last, self.last_table, self.dataset_id)
+        if not df_last.empty:
+            self.gbq_connector.upload_data(df_last, self.last_table, self.dataset_id)
 
-            if not df_timer.empty:
-                self.gbq_connector.upload_data(df_timer, self.timers_table, self.dataset_id)
+        if not df_timer.empty:
+            self.gbq_connector.upload_data(df_timer, self.timers_table, self.dataset_id)
 
-    def _part_types(self):
+    @staticmethod
+    def _part_types(metrics: t.List[PointWithType]):
         """Update measure type dict with list of records from the buffer"""
 
         measure_dict = defaultdict(list)
-        for record in self._buffer:
+        for record in metrics:
             measure_dict[record.measure].append(record.point)
         return measure_dict
 
-    def fix_pd_to_bq_types(self, df, dataset, table):
+    def fix_pd_to_bq_types(self, df: pd.DataFrame, dataset: str, table: str):
         """Fix pandas to GBQ types"""
 
         schema_fields = self.gbq_connector.retrieve_table_schema(dataset, table, list(df.columns))
         type_map = {
             "INT64": int,
             "FLOAT64": float,
             "STRING": str,
```

### Comparing `airflow_metrics_gbq-0.0.4a0/airflow_metrics_gbq/utils/__init__.py` & `airflow_metrics_gbq-0.0.4a1/airflow_metrics_gbq/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `airflow_metrics_gbq-0.0.4a0/airflow_metrics_gbq/utils/gbq_connector.py` & `airflow_metrics_gbq-0.0.4a1/airflow_metrics_gbq/utils/gbq_connector.py`

 * *Files identical despite different names*

### Comparing `airflow_metrics_gbq-0.0.4a0/pyproject.toml` & `airflow_metrics_gbq-0.0.4a1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "airflow-metrics-gbq"
-version = "0.0.4a0"
+version = "0.0.4a1"
 description = "Airflow metrics to Google BigQuery"
 authors = ["Shaurya Rawat <rawatshaurya1994@gmail.com>"]
 license = "BSD2"
 readme = "README.md"
 homepage="https://github.com/abyssnlp/airflow-metrics-gbq"
 repository="https://github.com/abyssnlp/airflow-metrics-gbq"
 include=[
@@ -23,14 +23,15 @@
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 pandas = "^2.0.0"
 google-cloud-bigquery = {extras = ["pandas"], version = "^3.10.0"}
 google-api-python-client = "^2.85.0"
 google-cloud-logging = "^3.5.0"
+tenacity = "^8.2.2"
 
 
 [tool.poetry.group.dev.dependencies]
 black = {extras = ["d"], version = "^23.3.0"}
 pylint = "^2.17.2"
 flake8 = "^6.0.0"
 pytest = "^7.3.1"
```

### Comparing `airflow_metrics_gbq-0.0.4a0/PKG-INFO` & `airflow_metrics_gbq-0.0.4a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow-metrics-gbq
-Version: 0.0.4a0
+Version: 0.0.4a1
 Summary: Airflow metrics to Google BigQuery
 Home-page: https://github.com/abyssnlp/airflow-metrics-gbq
 License: BSD2
 Author: Shaurya Rawat
 Author-email: rawatshaurya1994@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 3 - Alpha
@@ -19,14 +19,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: google-api-python-client (>=2.85.0,<3.0.0)
 Requires-Dist: google-cloud-bigquery[pandas] (>=3.10.0,<4.0.0)
 Requires-Dist: google-cloud-logging (>=3.5.0,<4.0.0)
 Requires-Dist: pandas (>=2.0.0,<3.0.0)
+Requires-Dist: tenacity (>=8.2.2,<9.0.0)
 Project-URL: Repository, https://github.com/abyssnlp/airflow-metrics-gbq
 Description-Content-Type: text/markdown
 
 Airflow Metrics to BigQuery
 ===
 
 <p align="center">
```

