# Comparing `tmp/featurizerai-1.4.7.tar.gz` & `tmp/featurizerai-1.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featurizerai-1.4.7.tar", last modified: Tue Apr 25 16:56:05 2023, max compression
+gzip compressed data, was "featurizerai-1.4.8.tar", last modified: Tue Apr 25 17:13:05 2023, max compression
```

## Comparing `featurizerai-1.4.7.tar` & `featurizerai-1.4.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-25 16:56:05.730071 featurizerai-1.4.7/
--rw-r--r--   0 burakkebapci   (501) staff       (20)     1079 2023-03-26 20:50:31.000000 featurizerai-1.4.7/LICENSE
--rw-r--r--   0 burakkebapci   (501) staff       (20)       85 2023-03-26 20:50:31.000000 featurizerai-1.4.7/MANIFEST.in
--rw-r--r--   0 burakkebapci   (501) staff       (20)      857 2023-04-25 16:56:05.730131 featurizerai-1.4.7/PKG-INFO
--rw-r--r--   0 burakkebapci   (501) staff       (20)       98 2023-03-26 20:50:31.000000 featurizerai-1.4.7/pyproject.toml
--rw-r--r--   0 burakkebapci   (501) staff       (20)      115 2023-04-25 16:56:05.730344 featurizerai-1.4.7/setup.cfg
--rw-r--r--   0 burakkebapci   (501) staff       (20)     1378 2023-04-25 16:55:20.000000 featurizerai-1.4.7/setup.py
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-25 16:56:05.726411 featurizerai-1.4.7/src/
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-25 16:56:05.728337 featurizerai-1.4.7/src/features/
--rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-04-22 17:23:59.000000 featurizerai-1.4.7/src/features/__init__.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)      686 2023-04-22 23:39:43.000000 featurizerai-1.4.7/src/features/authenticate.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)     4229 2023-04-23 11:29:31.000000 featurizerai-1.4.7/src/features/create_stream.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)      845 2023-04-23 11:45:28.000000 featurizerai-1.4.7/src/features/custom_schema.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)     4605 2023-04-25 16:55:15.000000 featurizerai-1.4.7/src/features/materialize.py
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-25 16:56:05.729016 featurizerai-1.4.7/src/features/tests/
--rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-04-25 16:35:40.000000 featurizerai-1.4.7/src/features/tests/__init__.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)     2309 2023-04-25 16:43:12.000000 featurizerai-1.4.7/src/features/tests/test_materialize.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)     1490 2023-04-25 16:15:10.000000 featurizerai-1.4.7/src/features/tests/test_pipeline.py
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-25 16:56:05.729952 featurizerai-1.4.7/src/featurizerai.egg-info/
--rw-r--r--   0 burakkebapci   (501) staff       (20)      857 2023-04-25 16:56:05.000000 featurizerai-1.4.7/src/featurizerai.egg-info/PKG-INFO
--rw-r--r--   0 burakkebapci   (501) staff       (20)      500 2023-04-25 16:56:05.000000 featurizerai-1.4.7/src/featurizerai.egg-info/SOURCES.txt
--rw-r--r--   0 burakkebapci   (501) staff       (20)        1 2023-04-25 16:56:05.000000 featurizerai-1.4.7/src/featurizerai.egg-info/dependency_links.txt
--rw-r--r--   0 burakkebapci   (501) staff       (20)       22 2023-04-25 16:56:05.000000 featurizerai-1.4.7/src/featurizerai.egg-info/requires.txt
--rw-r--r--   0 burakkebapci   (501) staff       (20)        9 2023-04-25 16:56:05.000000 featurizerai-1.4.7/src/featurizerai.egg-info/top_level.txt
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-25 17:13:05.988199 featurizerai-1.4.8/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     1079 2023-03-26 20:50:31.000000 featurizerai-1.4.8/LICENSE
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       85 2023-03-26 20:50:31.000000 featurizerai-1.4.8/MANIFEST.in
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      857 2023-04-25 17:13:05.988263 featurizerai-1.4.8/PKG-INFO
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       98 2023-03-26 20:50:31.000000 featurizerai-1.4.8/pyproject.toml
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      115 2023-04-25 17:13:05.988492 featurizerai-1.4.8/setup.cfg
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     1378 2023-04-25 17:13:02.000000 featurizerai-1.4.8/setup.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-25 17:13:05.985083 featurizerai-1.4.8/src/
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-25 17:13:05.987025 featurizerai-1.4.8/src/features/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-04-22 17:23:59.000000 featurizerai-1.4.8/src/features/__init__.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      686 2023-04-22 23:39:43.000000 featurizerai-1.4.8/src/features/authenticate.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     4229 2023-04-23 11:29:31.000000 featurizerai-1.4.8/src/features/create_stream.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      845 2023-04-23 11:45:28.000000 featurizerai-1.4.8/src/features/custom_schema.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     4695 2023-04-25 17:12:53.000000 featurizerai-1.4.8/src/features/materialize.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-25 17:13:05.987410 featurizerai-1.4.8/src/features/tests/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-04-25 16:35:40.000000 featurizerai-1.4.8/src/features/tests/__init__.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     2309 2023-04-25 16:43:12.000000 featurizerai-1.4.8/src/features/tests/test_materialize.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     1490 2023-04-25 16:15:10.000000 featurizerai-1.4.8/src/features/tests/test_pipeline.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-25 17:13:05.988076 featurizerai-1.4.8/src/featurizerai.egg-info/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      857 2023-04-25 17:13:05.000000 featurizerai-1.4.8/src/featurizerai.egg-info/PKG-INFO
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      500 2023-04-25 17:13:05.000000 featurizerai-1.4.8/src/featurizerai.egg-info/SOURCES.txt
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        1 2023-04-25 17:13:05.000000 featurizerai-1.4.8/src/featurizerai.egg-info/dependency_links.txt
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       22 2023-04-25 17:13:05.000000 featurizerai-1.4.8/src/featurizerai.egg-info/requires.txt
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        9 2023-04-25 17:13:05.000000 featurizerai-1.4.8/src/featurizerai.egg-info/top_level.txt
```

### Comparing `featurizerai-1.4.7/LICENSE` & `featurizerai-1.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `featurizerai-1.4.7/PKG-INFO` & `featurizerai-1.4.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurizerai
-Version: 1.4.7
+Version: 1.4.8
 Summary: Python library for Featurizer AI
 Home-page: https://github.com/burakglobal/featurizerai
 Author: Burak
 Author-email: burakgblobal@gmail.com
 Keywords: featurizer,package
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `featurizerai-1.4.7/setup.py` & `featurizerai-1.4.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 setuptools.setup(
     name='featurizerai',
     author='Burak',
-    version='1.4.7',
+    version='1.4.8',
     author_email='burakgblobal@gmail.com',
     description='Python library for Featurizer AI',
     keywords='featurizer, package',
     url='https://github.com/burakglobal/featurizerai',
     package_dir={'': 'src'},
     packages=setuptools.find_packages(where='src'),
     classifiers=[
```

### Comparing `featurizerai-1.4.7/src/features/authenticate.py` & `featurizerai-1.4.8/src/features/authenticate.py`

 * *Files identical despite different names*

### Comparing `featurizerai-1.4.7/src/features/create_stream.py` & `featurizerai-1.4.8/src/features/create_stream.py`

 * *Files identical despite different names*

### Comparing `featurizerai-1.4.7/src/features/custom_schema.py` & `featurizerai-1.4.8/src/features/custom_schema.py`

 * *Files identical despite different names*

### Comparing `featurizerai-1.4.7/src/features/materialize.py` & `featurizerai-1.4.8/src/features/materialize.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,15 @@
         raw_data_list = [doc for doc in raw_data]
         df = self.spark.createDataFrame(raw_data_list, self.schema)
 
         # Apply partitioning if the partition_column is specified
         if self.partition_column:
             print("Partitioning the DataFrame based on the column: " + self.partition_column)
             raw_data_collection.create_index(self.partition_column)
+            raw_data_collection.create_index(self.groupby_attr)
             df = df.repartition(col(self.partition_column))
 
         # Filter the DataFrame based on the given device_id
         df = df.filter(col(self.groupby_attr) == self.groupby)
         start_time = self.aggregation_date
         df = df.filter((col(self.groupby_attr) == self.groupby) & (col("timestamp") < start_time.timestamp()))
         df = df.withColumn("timestamp_unix", F.col("timestamp").cast("bigint"))
@@ -85,15 +86,15 @@
                 .select(df.columns + [col for col in c_count.columns if col not in df.columns])
             df = joined_df
 
         df = df.drop("timestamp_unix", "timestamp", "name", "email")
         # Convert the aggregated data to JSON
 
         if df.isEmpty():
-            json_aggregated_data = ""
+            json_aggregated_data = "{'error': 'No data found'}"
         else:
             json_aggregated_data = df.toJSON().collect()[0]
 
         if json_aggregated_data is not None:
             aggregated_data_collection.update_one(
                 {"date": start_time, "deviceid": self.groupby},
                 {"$set": {"aggregated_data": json_aggregated_data}},
```

### Comparing `featurizerai-1.4.7/src/features/tests/test_materialize.py` & `featurizerai-1.4.8/src/features/tests/test_materialize.py`

 * *Files identical despite different names*

### Comparing `featurizerai-1.4.7/src/features/tests/test_pipeline.py` & `featurizerai-1.4.8/src/features/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `featurizerai-1.4.7/src/featurizerai.egg-info/PKG-INFO` & `featurizerai-1.4.8/src/featurizerai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurizerai
-Version: 1.4.7
+Version: 1.4.8
 Summary: Python library for Featurizer AI
 Home-page: https://github.com/burakglobal/featurizerai
 Author: Burak
 Author-email: burakgblobal@gmail.com
 Keywords: featurizer,package
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

