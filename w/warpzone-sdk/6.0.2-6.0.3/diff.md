# Comparing `tmp/warpzone_sdk-6.0.2.tar.gz` & `tmp/warpzone_sdk-6.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "warpzone_sdk-6.0.2.tar", max compression
+gzip compressed data, was "warpzone_sdk-6.0.3.tar", max compression
```

## Comparing `warpzone_sdk-6.0.2.tar` & `warpzone_sdk-6.0.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1121 2023-04-24 06:27:18.750425 warpzone_sdk-6.0.2/pyproject.toml
--rw-r--r--   0        0        0     1185 2023-04-24 06:27:18.754425 warpzone_sdk-6.0.2/warpzone/__init__.py
--rw-r--r--   0        0        0       21 2023-04-24 06:27:18.754425 warpzone_sdk-6.0.2/warpzone/blobstorage/__init__.py
--rw-r--r--   0        0        0     2877 2023-04-24 06:27:18.754425 warpzone_sdk-6.0.2/warpzone/blobstorage/client.py
--rw-r--r--   0        0        0       24 2023-04-24 06:27:18.754425 warpzone_sdk-6.0.2/warpzone/enums/__init__.py
--rw-r--r--   0        0        0      187 2023-04-24 06:27:18.754425 warpzone_sdk-6.0.2/warpzone/enums/topicenum.py
--rw-r--r--   0        0        0       27 2023-04-24 06:27:18.754425 warpzone_sdk-6.0.2/warpzone/function/__init__.py
--rw-r--r--   0        0        0     1501 2023-04-24 06:27:18.754425 warpzone_sdk-6.0.2/warpzone/function/functionize.py
--rw-r--r--   0        0        0     2606 2023-04-24 06:27:18.754425 warpzone_sdk-6.0.2/warpzone/function/integrations.py
--rw-r--r--   0        0        0     2223 2023-04-24 06:27:18.754425 warpzone_sdk-6.0.2/warpzone/function/monitor.py
--rw-r--r--   0        0        0     1486 2023-04-24 06:27:18.754425 warpzone_sdk-6.0.2/warpzone/function/process.py
--rw-r--r--   0        0        0       32 2023-04-24 06:27:18.754425 warpzone_sdk-6.0.2/warpzone/function/processors/__init__.py
--rw-r--r--   0        0        0     1337 2023-04-24 06:27:18.754425 warpzone_sdk-6.0.2/warpzone/function/processors/outputs.py
--rw-r--r--   0        0        0     1379 2023-04-24 06:27:18.754425 warpzone_sdk-6.0.2/warpzone/function/processors/triggers.py
--rw-r--r--   0        0        0     2268 2023-04-24 06:27:18.754425 warpzone_sdk-6.0.2/warpzone/function/signature.py
--rw-r--r--   0        0        0       80 2023-04-24 06:27:18.754425 warpzone_sdk-6.0.2/warpzone/function/types.py
--rw-r--r--   0        0        0     2108 2023-04-24 06:27:18.754425 warpzone_sdk-6.0.2/warpzone/healthchecks/__init__.py
--rw-r--r--   0        0        0     1112 2023-04-24 06:27:18.754425 warpzone_sdk-6.0.2/warpzone/healthchecks/model.py
--rw-r--r--   0        0        0       87 2023-04-24 06:27:18.754425 warpzone_sdk-6.0.2/warpzone/monitor/__init__.py
--rw-r--r--   0        0        0     1650 2023-04-24 06:27:18.754425 warpzone_sdk-6.0.2/warpzone/monitor/logs.py
--rw-r--r--   0        0        0     4781 2023-04-24 06:27:18.754425 warpzone_sdk-6.0.2/warpzone/monitor/traces.py
--rw-r--r--   0        0        0       21 2023-04-24 06:27:18.754425 warpzone_sdk-6.0.2/warpzone/servicebus/data/__init__.py
--rw-r--r--   0        0        0     5433 2023-04-24 06:27:18.754425 warpzone_sdk-6.0.2/warpzone/servicebus/data/client.py
--rw-r--r--   0        0        0       21 2023-04-24 06:27:18.754425 warpzone_sdk-6.0.2/warpzone/servicebus/events/__init__.py
--rw-r--r--   0        0        0     4250 2023-04-24 06:27:18.754425 warpzone_sdk-6.0.2/warpzone/servicebus/events/client.py
--rw-r--r--   0        0        0       47 2023-04-24 06:27:18.754425 warpzone_sdk-6.0.2/warpzone/tablestorage/__init__.py
--rw-r--r--   0        0        0     2882 2023-04-24 06:27:18.754425 warpzone_sdk-6.0.2/warpzone/tablestorage/client.py
--rw-r--r--   0        0        0     2509 2023-04-24 06:27:18.754425 warpzone_sdk-6.0.2/warpzone/tablestorage/client_async.py
--rw-r--r--   0        0        0      521 2023-04-24 06:27:18.754425 warpzone_sdk-6.0.2/warpzone/tablestorage/helpers.py
--rw-r--r--   0        0        0     2470 2023-04-24 06:27:18.754425 warpzone_sdk-6.0.2/warpzone/tablestorage/operations.py
--rw-r--r--   0        0        0      176 2023-04-24 06:27:18.754425 warpzone_sdk-6.0.2/warpzone/testing/__init__.py
--rw-r--r--   0        0        0     2191 2023-04-24 06:27:18.754425 warpzone_sdk-6.0.2/warpzone/testing/assertions.py
--rw-r--r--   0        0        0     3499 2023-04-24 06:27:18.754425 warpzone_sdk-6.0.2/warpzone/testing/data.py
--rw-r--r--   0        0        0       19 2023-04-24 06:27:18.754425 warpzone_sdk-6.0.2/warpzone/transform/__init__.py
--rw-r--r--   0        0        0     1641 2023-04-24 06:27:18.754425 warpzone_sdk-6.0.2/warpzone/transform/data.py
--rw-r--r--   0        0        0     1048 1970-01-01 00:00:00.000000 warpzone_sdk-6.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1121 2023-04-26 12:11:59.723214 warpzone_sdk-6.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1185 2023-04-26 12:11:59.723214 warpzone_sdk-6.0.3/warpzone/__init__.py
+-rw-r--r--   0        0        0       21 2023-04-26 12:11:59.723214 warpzone_sdk-6.0.3/warpzone/blobstorage/__init__.py
+-rw-r--r--   0        0        0     2877 2023-04-26 12:11:59.723214 warpzone_sdk-6.0.3/warpzone/blobstorage/client.py
+-rw-r--r--   0        0        0       24 2023-04-26 12:11:59.723214 warpzone_sdk-6.0.3/warpzone/enums/__init__.py
+-rw-r--r--   0        0        0      187 2023-04-26 12:11:59.723214 warpzone_sdk-6.0.3/warpzone/enums/topicenum.py
+-rw-r--r--   0        0        0       27 2023-04-26 12:11:59.723214 warpzone_sdk-6.0.3/warpzone/function/__init__.py
+-rw-r--r--   0        0        0     1501 2023-04-26 12:11:59.723214 warpzone_sdk-6.0.3/warpzone/function/functionize.py
+-rw-r--r--   0        0        0     2606 2023-04-26 12:11:59.723214 warpzone_sdk-6.0.3/warpzone/function/integrations.py
+-rw-r--r--   0        0        0     2223 2023-04-26 12:11:59.723214 warpzone_sdk-6.0.3/warpzone/function/monitor.py
+-rw-r--r--   0        0        0     1486 2023-04-26 12:11:59.723214 warpzone_sdk-6.0.3/warpzone/function/process.py
+-rw-r--r--   0        0        0       32 2023-04-26 12:11:59.723214 warpzone_sdk-6.0.3/warpzone/function/processors/__init__.py
+-rw-r--r--   0        0        0     1337 2023-04-26 12:11:59.723214 warpzone_sdk-6.0.3/warpzone/function/processors/outputs.py
+-rw-r--r--   0        0        0     1727 2023-04-26 12:11:59.723214 warpzone_sdk-6.0.3/warpzone/function/processors/triggers.py
+-rw-r--r--   0        0        0     2268 2023-04-26 12:11:59.723214 warpzone_sdk-6.0.3/warpzone/function/signature.py
+-rw-r--r--   0        0        0       80 2023-04-26 12:11:59.723214 warpzone_sdk-6.0.3/warpzone/function/types.py
+-rw-r--r--   0        0        0     2108 2023-04-26 12:11:59.723214 warpzone_sdk-6.0.3/warpzone/healthchecks/__init__.py
+-rw-r--r--   0        0        0     1112 2023-04-26 12:11:59.723214 warpzone_sdk-6.0.3/warpzone/healthchecks/model.py
+-rw-r--r--   0        0        0       87 2023-04-26 12:11:59.723214 warpzone_sdk-6.0.3/warpzone/monitor/__init__.py
+-rw-r--r--   0        0        0     1650 2023-04-26 12:11:59.723214 warpzone_sdk-6.0.3/warpzone/monitor/logs.py
+-rw-r--r--   0        0        0     4781 2023-04-26 12:11:59.723214 warpzone_sdk-6.0.3/warpzone/monitor/traces.py
+-rw-r--r--   0        0        0       21 2023-04-26 12:11:59.723214 warpzone_sdk-6.0.3/warpzone/servicebus/data/__init__.py
+-rw-r--r--   0        0        0     5436 2023-04-26 12:11:59.723214 warpzone_sdk-6.0.3/warpzone/servicebus/data/client.py
+-rw-r--r--   0        0        0       21 2023-04-26 12:11:59.723214 warpzone_sdk-6.0.3/warpzone/servicebus/events/__init__.py
+-rw-r--r--   0        0        0     4250 2023-04-26 12:11:59.723214 warpzone_sdk-6.0.3/warpzone/servicebus/events/client.py
+-rw-r--r--   0        0        0       47 2023-04-26 12:11:59.723214 warpzone_sdk-6.0.3/warpzone/tablestorage/__init__.py
+-rw-r--r--   0        0        0     2882 2023-04-26 12:11:59.723214 warpzone_sdk-6.0.3/warpzone/tablestorage/client.py
+-rw-r--r--   0        0        0     2509 2023-04-26 12:11:59.723214 warpzone_sdk-6.0.3/warpzone/tablestorage/client_async.py
+-rw-r--r--   0        0        0      521 2023-04-26 12:11:59.723214 warpzone_sdk-6.0.3/warpzone/tablestorage/helpers.py
+-rw-r--r--   0        0        0     2470 2023-04-26 12:11:59.723214 warpzone_sdk-6.0.3/warpzone/tablestorage/operations.py
+-rw-r--r--   0        0        0      176 2023-04-26 12:11:59.723214 warpzone_sdk-6.0.3/warpzone/testing/__init__.py
+-rw-r--r--   0        0        0     2191 2023-04-26 12:11:59.723214 warpzone_sdk-6.0.3/warpzone/testing/assertions.py
+-rw-r--r--   0        0        0     3499 2023-04-26 12:11:59.727214 warpzone_sdk-6.0.3/warpzone/testing/data.py
+-rw-r--r--   0        0        0       19 2023-04-26 12:11:59.727214 warpzone_sdk-6.0.3/warpzone/transform/__init__.py
+-rw-r--r--   0        0        0     1641 2023-04-26 12:11:59.727214 warpzone_sdk-6.0.3/warpzone/transform/data.py
+-rw-r--r--   0        0        0     1048 1970-01-01 00:00:00.000000 warpzone_sdk-6.0.3/PKG-INFO
```

### Comparing `warpzone_sdk-6.0.2/pyproject.toml` & `warpzone_sdk-6.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "warpzone-sdk"
-version = "6.0.2"
+version = "6.0.3"
 description = "The main objective of this package is to centralize logic used to interact with Azure Functions, Azure Service Bus and Azure Table Storage"
 authors = ["Anders Launer Baek-Petersen <alp@energinet.dk>", "Mikkel Ladekarl Folmersen Nygaard <mny@energinet.dk>", "Ulrik Christensen <uch@energinet.dk>"]
 packages = [
     { include = "warpzone" },
 ]
 
 [tool.poetry.dependencies]
```

### Comparing `warpzone_sdk-6.0.2/warpzone/__init__.py` & `warpzone_sdk-6.0.3/warpzone/__init__.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.2/warpzone/blobstorage/client.py` & `warpzone_sdk-6.0.3/warpzone/blobstorage/client.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.2/warpzone/function/functionize.py` & `warpzone_sdk-6.0.3/warpzone/function/functionize.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.2/warpzone/function/integrations.py` & `warpzone_sdk-6.0.3/warpzone/function/integrations.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.2/warpzone/function/monitor.py` & `warpzone_sdk-6.0.3/warpzone/function/monitor.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.2/warpzone/function/process.py` & `warpzone_sdk-6.0.3/warpzone/function/process.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.2/warpzone/function/processors/outputs.py` & `warpzone_sdk-6.0.3/warpzone/function/processors/outputs.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.2/warpzone/function/signature.py` & `warpzone_sdk-6.0.3/warpzone/function/signature.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.2/warpzone/healthchecks/__init__.py` & `warpzone_sdk-6.0.3/warpzone/healthchecks/__init__.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.2/warpzone/healthchecks/model.py` & `warpzone_sdk-6.0.3/warpzone/healthchecks/model.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.2/warpzone/monitor/logs.py` & `warpzone_sdk-6.0.3/warpzone/monitor/logs.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.2/warpzone/monitor/traces.py` & `warpzone_sdk-6.0.3/warpzone/monitor/traces.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.2/warpzone/servicebus/data/client.py` & `warpzone_sdk-6.0.3/warpzone/servicebus/data/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,14 +99,15 @@
         # 2. download blob from <blob-name> location
         blob_data = self._storage_client.download(
             container_name=DATA_CONTAINER_NAME, blob_name=blob_name
         )
 
         # 3. create data message
         extension = blob_name.split(".")[-1]
+
         return DataMessage(
             content=blob_data.content,
             extension=extension,
             message_id=event_msg.message_id,
             subject=event_msg.subject,
             metadata=blob_data.metadata,
         )
@@ -118,24 +119,26 @@
 
         # 2. upload blob to <blob-name>
         blob_data = BlobData(
             content=data_msg.content,
             name=blob_name,
             metadata=data_msg.metadata,
         )
+
         self._storage_client.upload(
             blob_data=blob_data,
             container_name=DATA_CONTAINER_NAME,
         )
 
         # 3. create event message
         event = {
             BLOB_NAME_PARAM: blob_name,
             TIMESTAMP_PARAM: data_msg.timestamp.strftime(TIMESTAMP_FORMAT),
         }
+
         return EventMessage(
             event=event,
             subject=data_msg.subject,
             message_id=data_msg.message_id,
         )
 
     def receive(
```

### Comparing `warpzone_sdk-6.0.2/warpzone/servicebus/events/client.py` & `warpzone_sdk-6.0.3/warpzone/servicebus/events/client.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.2/warpzone/tablestorage/client.py` & `warpzone_sdk-6.0.3/warpzone/tablestorage/client.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.2/warpzone/tablestorage/client_async.py` & `warpzone_sdk-6.0.3/warpzone/tablestorage/client_async.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.2/warpzone/tablestorage/helpers.py` & `warpzone_sdk-6.0.3/warpzone/tablestorage/helpers.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.2/warpzone/tablestorage/operations.py` & `warpzone_sdk-6.0.3/warpzone/tablestorage/operations.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.2/warpzone/testing/assertions.py` & `warpzone_sdk-6.0.3/warpzone/testing/assertions.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.2/warpzone/testing/data.py` & `warpzone_sdk-6.0.3/warpzone/testing/data.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.2/warpzone/transform/data.py` & `warpzone_sdk-6.0.3/warpzone/transform/data.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.2/PKG-INFO` & `warpzone_sdk-6.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: warpzone-sdk
-Version: 6.0.2
+Version: 6.0.3
 Summary: The main objective of this package is to centralize logic used to interact with Azure Functions, Azure Service Bus and Azure Table Storage
 Author: Anders Launer Baek-Petersen
 Author-email: alp@energinet.dk
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

