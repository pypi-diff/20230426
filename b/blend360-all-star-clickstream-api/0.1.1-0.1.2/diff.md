# Comparing `tmp/blend360_all_star_clickstream_api-0.1.1.tar.gz` & `tmp/blend360_all_star_clickstream_api-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blend360_all_star_clickstream_api-0.1.1.tar", last modified: Tue Apr  4 16:50:00 2023, max compression
+gzip compressed data, was "blend360_all_star_clickstream_api-0.1.2.tar", last modified: Tue Apr 25 14:33:42 2023, max compression
```

## Comparing `blend360_all_star_clickstream_api-0.1.1.tar` & `blend360_all_star_clickstream_api-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-04-04 16:50:00.112578 blend360_all_star_clickstream_api-0.1.1/
--rw-r--r--   0 alex      (1000) alex      (1000)     1799 2023-02-13 21:46:16.000000 blend360_all_star_clickstream_api-0.1.1/.gitignore
--rw-r--r--   0 alex      (1000) alex      (1000)     1100 2023-03-24 20:36:41.000000 blend360_all_star_clickstream_api-0.1.1/LICENSE
--rw-r--r--   0 alex      (1000) alex      (1000)     3566 2023-04-04 16:50:00.112578 blend360_all_star_clickstream_api-0.1.1/PKG-INFO
--rw-r--r--   0 alex      (1000) alex      (1000)     3329 2023-04-04 16:49:44.000000 blend360_all_star_clickstream_api-0.1.1/README.md
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-04-04 16:50:00.109245 blend360_all_star_clickstream_api-0.1.1/examples/
--rw-r--r--   0 alex      (1000) alex      (1000)     3624 2023-04-04 16:49:44.000000 blend360_all_star_clickstream_api-0.1.1/examples/example.ipynb
--rw-r--r--   0 alex      (1000) alex      (1000)      417 2023-04-04 16:49:44.000000 blend360_all_star_clickstream_api-0.1.1/pyproject.toml
--rw-r--r--   0 alex      (1000) alex      (1000)      159 2023-04-04 16:50:00.112578 blend360_all_star_clickstream_api-0.1.1/setup.cfg
--rw-r--r--   0 alex      (1000) alex      (1000)       68 2023-03-24 20:36:41.000000 blend360_all_star_clickstream_api-0.1.1/setup.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-04-04 16:50:00.109245 blend360_all_star_clickstream_api-0.1.1/src/
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-04-04 16:50:00.109245 blend360_all_star_clickstream_api-0.1.1/src/blend360_all_star_clickstream_api/
--rw-r--r--   0 alex      (1000) alex      (1000)        0 2023-04-04 16:49:44.000000 blend360_all_star_clickstream_api-0.1.1/src/blend360_all_star_clickstream_api/__init__.py
--rw-r--r--   0 alex      (1000) alex      (1000)     5018 2023-04-04 16:49:44.000000 blend360_all_star_clickstream_api-0.1.1/src/blend360_all_star_clickstream_api/datafetch.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-04-04 16:50:00.112578 blend360_all_star_clickstream_api-0.1.1/src/blend360_all_star_clickstream_api.egg-info/
--rw-r--r--   0 alex      (1000) alex      (1000)     3566 2023-04-04 16:50:00.000000 blend360_all_star_clickstream_api-0.1.1/src/blend360_all_star_clickstream_api.egg-info/PKG-INFO
--rw-r--r--   0 alex      (1000) alex      (1000)      513 2023-04-04 16:50:00.000000 blend360_all_star_clickstream_api-0.1.1/src/blend360_all_star_clickstream_api.egg-info/SOURCES.txt
--rw-r--r--   0 alex      (1000) alex      (1000)        1 2023-04-04 16:50:00.000000 blend360_all_star_clickstream_api-0.1.1/src/blend360_all_star_clickstream_api.egg-info/dependency_links.txt
--rw-r--r--   0 alex      (1000) alex      (1000)       28 2023-04-04 16:50:00.000000 blend360_all_star_clickstream_api-0.1.1/src/blend360_all_star_clickstream_api.egg-info/requires.txt
--rw-r--r--   0 alex      (1000) alex      (1000)       34 2023-04-04 16:50:00.000000 blend360_all_star_clickstream_api-0.1.1/src/blend360_all_star_clickstream_api.egg-info/top_level.txt
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-04-04 16:50:00.112578 blend360_all_star_clickstream_api-0.1.1/test/
--rw-r--r--   0 alex      (1000) alex      (1000)      921 2023-04-04 16:49:44.000000 blend360_all_star_clickstream_api-0.1.1/test/test_datafetch.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-04-25 14:33:42.566146 blend360_all_star_clickstream_api-0.1.2/
+-rw-r--r--   0 alex      (1000) alex      (1000)     1799 2023-02-13 21:46:16.000000 blend360_all_star_clickstream_api-0.1.2/.gitignore
+-rw-r--r--   0 alex      (1000) alex      (1000)     1100 2023-03-24 20:36:41.000000 blend360_all_star_clickstream_api-0.1.2/LICENSE
+-rw-r--r--   0 alex      (1000) alex      (1000)     3566 2023-04-25 14:33:42.566146 blend360_all_star_clickstream_api-0.1.2/PKG-INFO
+-rw-r--r--   0 alex      (1000) alex      (1000)     3329 2023-04-25 14:27:12.000000 blend360_all_star_clickstream_api-0.1.2/README.md
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-04-25 14:33:42.566146 blend360_all_star_clickstream_api-0.1.2/examples/
+-rw-r--r--   0 alex      (1000) alex      (1000)     3624 2023-04-25 14:27:12.000000 blend360_all_star_clickstream_api-0.1.2/examples/example.ipynb
+-rw-r--r--   0 alex      (1000) alex      (1000)      417 2023-04-25 14:30:10.000000 blend360_all_star_clickstream_api-0.1.2/pyproject.toml
+-rw-r--r--   0 alex      (1000) alex      (1000)      159 2023-04-25 14:33:42.566146 blend360_all_star_clickstream_api-0.1.2/setup.cfg
+-rw-r--r--   0 alex      (1000) alex      (1000)       68 2023-03-24 20:36:41.000000 blend360_all_star_clickstream_api-0.1.2/setup.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-04-25 14:33:42.562813 blend360_all_star_clickstream_api-0.1.2/src/
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-04-25 14:33:42.566146 blend360_all_star_clickstream_api-0.1.2/src/blend360_all_star_clickstream_api/
+-rw-r--r--   0 alex      (1000) alex      (1000)        0 2023-04-25 14:27:12.000000 blend360_all_star_clickstream_api-0.1.2/src/blend360_all_star_clickstream_api/__init__.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     5018 2023-04-25 14:30:10.000000 blend360_all_star_clickstream_api-0.1.2/src/blend360_all_star_clickstream_api/datafetch.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-04-25 14:33:42.566146 blend360_all_star_clickstream_api-0.1.2/src/blend360_all_star_clickstream_api.egg-info/
+-rw-r--r--   0 alex      (1000) alex      (1000)     3566 2023-04-25 14:33:42.000000 blend360_all_star_clickstream_api-0.1.2/src/blend360_all_star_clickstream_api.egg-info/PKG-INFO
+-rw-r--r--   0 alex      (1000) alex      (1000)      513 2023-04-25 14:33:42.000000 blend360_all_star_clickstream_api-0.1.2/src/blend360_all_star_clickstream_api.egg-info/SOURCES.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)        1 2023-04-25 14:33:42.000000 blend360_all_star_clickstream_api-0.1.2/src/blend360_all_star_clickstream_api.egg-info/dependency_links.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)       28 2023-04-25 14:33:42.000000 blend360_all_star_clickstream_api-0.1.2/src/blend360_all_star_clickstream_api.egg-info/requires.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)       34 2023-04-25 14:33:42.000000 blend360_all_star_clickstream_api-0.1.2/src/blend360_all_star_clickstream_api.egg-info/top_level.txt
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-04-25 14:33:42.566146 blend360_all_star_clickstream_api-0.1.2/test/
+-rw-r--r--   0 alex      (1000) alex      (1000)      921 2023-04-25 14:27:12.000000 blend360_all_star_clickstream_api-0.1.2/test/test_datafetch.py
```

### Comparing `blend360_all_star_clickstream_api-0.1.1/.gitignore` & `blend360_all_star_clickstream_api-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `blend360_all_star_clickstream_api-0.1.1/LICENSE` & `blend360_all_star_clickstream_api-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `blend360_all_star_clickstream_api-0.1.1/PKG-INFO` & `blend360_all_star_clickstream_api-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blend360_all_star_clickstream_api
-Version: 0.1.1
+Version: 0.1.2
 Summary: Package to request synthetic clickstream data.
 Author: Blend360
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # de-allstar-training-clickstream-api
```

### Comparing `blend360_all_star_clickstream_api-0.1.1/README.md` & `blend360_all_star_clickstream_api-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `blend360_all_star_clickstream_api-0.1.1/examples/example.ipynb` & `blend360_all_star_clickstream_api-0.1.2/examples/example.ipynb`

 * *Files identical despite different names*

### Comparing `blend360_all_star_clickstream_api-0.1.1/src/blend360_all_star_clickstream_api/datafetch.py` & `blend360_all_star_clickstream_api-0.1.2/src/blend360_all_star_clickstream_api/datafetch.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         """
         Module to interact with dataprocesing for DE All Star Project
         
         Args:
             `secret_scope` (`str`): Secrets scope to read/save secrets
             `key_name` (`str`): Name of api_key secret to read/save
         """       
-        self.parse_date = lambda dt: dt.strftime('%d-%m-%Y')
+        self.parse_date = lambda dt: dt.strftime('%m-%d-%Y')
 
         self.base_url = "https://en44bq5e33.execute-api.us-east-1.amazonaws.com/dev"
 
         self.header = {
             'Content-Type': 'application/json'
         }
```

### Comparing `blend360_all_star_clickstream_api-0.1.1/src/blend360_all_star_clickstream_api.egg-info/PKG-INFO` & `blend360_all_star_clickstream_api-0.1.2/src/blend360_all_star_clickstream_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blend360-all-star-clickstream-api
-Version: 0.1.1
+Version: 0.1.2
 Summary: Package to request synthetic clickstream data.
 Author: Blend360
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # de-allstar-training-clickstream-api
```

### Comparing `blend360_all_star_clickstream_api-0.1.1/src/blend360_all_star_clickstream_api.egg-info/SOURCES.txt` & `blend360_all_star_clickstream_api-0.1.2/src/blend360_all_star_clickstream_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blend360_all_star_clickstream_api-0.1.1/test/test_datafetch.py` & `blend360_all_star_clickstream_api-0.1.2/test/test_datafetch.py`

 * *Files identical despite different names*

