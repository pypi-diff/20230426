# Comparing `tmp/maestro_python_client-0.9.4.tar.gz` & `tmp/maestro_python_client-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maestro_python_client-0.9.4.tar", last modified: Tue Jan 10 10:56:54 2023, max compression
+gzip compressed data, was "maestro_python_client-0.9.5.tar", last modified: Wed Apr 26 12:25:14 2023, max compression
```

## Comparing `maestro_python_client-0.9.4.tar` & `maestro_python_client-0.9.5.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 gaellanez   (501) staff       (20)        0 2023-01-10 10:56:54.510746 maestro_python_client-0.9.4/
--rw-r--r--   0 gaellanez   (501) staff       (20)      560 2023-01-10 10:56:54.510414 maestro_python_client-0.9.4/PKG-INFO
--rw-r--r--   0 gaellanez   (501) staff       (20)       24 2022-12-20 12:57:35.000000 maestro_python_client-0.9.4/README.md
-drwxr-xr-x   0 gaellanez   (501) staff       (20)        0 2023-01-10 10:56:54.499633 maestro_python_client-0.9.4/maestro_python_client/
-drwxr-xr-x   0 gaellanez   (501) staff       (20)        0 2023-01-10 10:56:54.509595 maestro_python_client-0.9.4/maestro_python_client/Cache/
--rw-r--r--   0 gaellanez   (501) staff       (20)      349 2022-12-22 10:45:07.000000 maestro_python_client-0.9.4/maestro_python_client/Cache/Cache.py
--rw-r--r--   0 gaellanez   (501) staff       (20)      750 2022-12-22 10:45:07.000000 maestro_python_client-0.9.4/maestro_python_client/Cache/RedisCache.py
--rw-r--r--   0 gaellanez   (501) staff       (20)        0 2022-12-22 13:32:39.000000 maestro_python_client-0.9.4/maestro_python_client/Cache/__init__.py
--rw-r--r--   0 gaellanez   (501) staff       (20)     1516 2022-12-22 13:26:03.000000 maestro_python_client-0.9.4/maestro_python_client/Cache/test_RedisCache.py
--rw-r--r--   0 gaellanez   (501) staff       (20)     6713 2023-01-10 10:55:05.000000 maestro_python_client-0.9.4/maestro_python_client/CachedClient.py
--rw-r--r--   0 gaellanez   (501) staff       (20)    11865 2023-01-10 10:55:05.000000 maestro_python_client-0.9.4/maestro_python_client/Client.py
--rw-r--r--   0 gaellanez   (501) staff       (20)       68 2023-01-10 10:55:05.000000 maestro_python_client-0.9.4/maestro_python_client/__init__.py
--rw-r--r--   0 gaellanez   (501) staff       (20)    12045 2022-12-23 13:12:10.000000 maestro_python_client-0.9.4/maestro_python_client/test_CachedClient.py
-drwxr-xr-x   0 gaellanez   (501) staff       (20)        0 2023-01-10 10:56:54.503515 maestro_python_client-0.9.4/maestro_python_client.egg-info/
--rw-r--r--   0 gaellanez   (501) staff       (20)      560 2023-01-10 10:56:54.000000 maestro_python_client-0.9.4/maestro_python_client.egg-info/PKG-INFO
--rw-r--r--   0 gaellanez   (501) staff       (20)      570 2023-01-10 10:56:54.000000 maestro_python_client-0.9.4/maestro_python_client.egg-info/SOURCES.txt
--rw-r--r--   0 gaellanez   (501) staff       (20)        1 2023-01-10 10:56:54.000000 maestro_python_client-0.9.4/maestro_python_client.egg-info/dependency_links.txt
--rw-r--r--   0 gaellanez   (501) staff       (20)        9 2023-01-10 10:56:54.000000 maestro_python_client-0.9.4/maestro_python_client.egg-info/requires.txt
--rw-r--r--   0 gaellanez   (501) staff       (20)       22 2023-01-10 10:56:54.000000 maestro_python_client-0.9.4/maestro_python_client.egg-info/top_level.txt
--rw-r--r--   0 gaellanez   (501) staff       (20)       31 2022-12-22 10:45:07.000000 maestro_python_client-0.9.4/pyproject.toml
--rw-r--r--   0 gaellanez   (501) staff       (20)       38 2023-01-10 10:56:54.511827 maestro_python_client-0.9.4/setup.cfg
--rw-r--r--   0 gaellanez   (501) staff       (20)     2740 2022-12-22 13:11:18.000000 maestro_python_client-0.9.4/setup.py
+drwxr-xr-x   0 wazaby    (1000) wazaby    (1000)        0 2023-04-26 12:25:14.472372 maestro_python_client-0.9.5/
+-rw-r--r--   0 wazaby    (1000) wazaby    (1000)      560 2023-04-26 12:25:14.472372 maestro_python_client-0.9.5/PKG-INFO
+-rw-r--r--   0 wazaby    (1000) wazaby    (1000)       24 2023-04-26 12:19:27.000000 maestro_python_client-0.9.5/README.md
+-rwxr-xr-x   0 wazaby    (1000) wazaby    (1000)     1874 2023-04-26 12:19:27.000000 maestro_python_client-0.9.5/maestro_client
+drwxr-xr-x   0 wazaby    (1000) wazaby    (1000)        0 2023-04-26 12:25:14.469039 maestro_python_client-0.9.5/maestro_python_client/
+drwxr-xr-x   0 wazaby    (1000) wazaby    (1000)        0 2023-04-26 12:25:14.472372 maestro_python_client-0.9.5/maestro_python_client/Cache/
+-rw-r--r--   0 wazaby    (1000) wazaby    (1000)      349 2023-04-26 12:19:27.000000 maestro_python_client-0.9.5/maestro_python_client/Cache/Cache.py
+-rw-r--r--   0 wazaby    (1000) wazaby    (1000)      750 2023-04-26 12:19:27.000000 maestro_python_client-0.9.5/maestro_python_client/Cache/RedisCache.py
+-rw-r--r--   0 wazaby    (1000) wazaby    (1000)        0 2023-04-26 12:19:27.000000 maestro_python_client-0.9.5/maestro_python_client/Cache/__init__.py
+-rw-r--r--   0 wazaby    (1000) wazaby    (1000)     1516 2023-04-26 12:19:27.000000 maestro_python_client-0.9.5/maestro_python_client/Cache/test_RedisCache.py
+-rw-r--r--   0 wazaby    (1000) wazaby    (1000)     6713 2023-04-26 12:19:27.000000 maestro_python_client-0.9.5/maestro_python_client/CachedClient.py
+-rw-r--r--   0 wazaby    (1000) wazaby    (1000)    11937 2023-04-26 12:19:27.000000 maestro_python_client-0.9.5/maestro_python_client/Client.py
+-rw-r--r--   0 wazaby    (1000) wazaby    (1000)       68 2023-04-26 12:19:27.000000 maestro_python_client-0.9.5/maestro_python_client/__init__.py
+-rw-r--r--   0 wazaby    (1000) wazaby    (1000)    12045 2023-04-26 12:19:27.000000 maestro_python_client-0.9.5/maestro_python_client/test_CachedClient.py
+drwxr-xr-x   0 wazaby    (1000) wazaby    (1000)        0 2023-04-26 12:25:14.469039 maestro_python_client-0.9.5/maestro_python_client.egg-info/
+-rw-r--r--   0 wazaby    (1000) wazaby    (1000)      560 2023-04-26 12:25:13.000000 maestro_python_client-0.9.5/maestro_python_client.egg-info/PKG-INFO
+-rw-r--r--   0 wazaby    (1000) wazaby    (1000)      585 2023-04-26 12:25:14.000000 maestro_python_client-0.9.5/maestro_python_client.egg-info/SOURCES.txt
+-rw-r--r--   0 wazaby    (1000) wazaby    (1000)        1 2023-04-26 12:25:13.000000 maestro_python_client-0.9.5/maestro_python_client.egg-info/dependency_links.txt
+-rw-r--r--   0 wazaby    (1000) wazaby    (1000)        9 2023-04-26 12:25:14.000000 maestro_python_client-0.9.5/maestro_python_client.egg-info/requires.txt
+-rw-r--r--   0 wazaby    (1000) wazaby    (1000)       22 2023-04-26 12:25:14.000000 maestro_python_client-0.9.5/maestro_python_client.egg-info/top_level.txt
+-rw-r--r--   0 wazaby    (1000) wazaby    (1000)       31 2023-04-26 12:19:27.000000 maestro_python_client-0.9.5/pyproject.toml
+-rw-r--r--   0 wazaby    (1000) wazaby    (1000)       38 2023-04-26 12:25:14.472372 maestro_python_client-0.9.5/setup.cfg
+-rw-r--r--   0 wazaby    (1000) wazaby    (1000)     2772 2023-04-26 12:19:27.000000 maestro_python_client-0.9.5/setup.py
```

### Comparing `maestro_python_client-0.9.4/PKG-INFO` & `maestro_python_client-0.9.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maestro_python_client
-Version: 0.9.4
+Version: 0.9.5
 Summary: Maestro client in python
 Home-page: https://github.com/owlint/maestro_python_client
 Author: Laurent Evrard
 Author-email: evrardlaurent77@gmail.com
 License: WTFPL
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 1 - Planning
```

### Comparing `maestro_python_client-0.9.4/maestro_python_client/Cache/RedisCache.py` & `maestro_python_client-0.9.5/maestro_python_client/Cache/RedisCache.py`

 * *Files identical despite different names*

### Comparing `maestro_python_client-0.9.4/maestro_python_client/Cache/test_RedisCache.py` & `maestro_python_client-0.9.5/maestro_python_client/Cache/test_RedisCache.py`

 * *Files identical despite different names*

### Comparing `maestro_python_client-0.9.4/maestro_python_client/CachedClient.py` & `maestro_python_client-0.9.5/maestro_python_client/CachedClient.py`

 * *Files identical despite different names*

### Comparing `maestro_python_client-0.9.4/maestro_python_client/Client.py` & `maestro_python_client-0.9.5/maestro_python_client/Client.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,14 +66,15 @@
             owner: owner of the task. Used for fair scheduling.
             queue: name of the queue to use.
             task_payload: encoded payload for the task.
             retries: Number of allowed retries in case of fail or timeouts.
             timeout: Allowed time span for the task to execute.
             executes_in: Number of seconds to wait before executing the task
             start_timeout: Allowed time span in seconds for the task to start.
+            callback_url: URL called after task execution is completed.
 
         Returns:
             A string representing the Maestro task id
 
         Raises:
             ValueError: Problem in the communication with maestro.
         """
```

### Comparing `maestro_python_client-0.9.4/maestro_python_client/test_CachedClient.py` & `maestro_python_client-0.9.5/maestro_python_client/test_CachedClient.py`

 * *Files identical despite different names*

### Comparing `maestro_python_client-0.9.4/maestro_python_client.egg-info/PKG-INFO` & `maestro_python_client-0.9.5/maestro_python_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maestro-python-client
-Version: 0.9.4
+Version: 0.9.5
 Summary: Maestro client in python
 Home-page: https://github.com/owlint/maestro_python_client
 Author: Laurent Evrard
 Author-email: evrardlaurent77@gmail.com
 License: WTFPL
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 1 - Planning
```

### Comparing `maestro_python_client-0.9.4/maestro_python_client.egg-info/SOURCES.txt` & `maestro_python_client-0.9.5/maestro_python_client.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 README.md
+maestro_client
 pyproject.toml
 setup.py
 maestro_python_client/CachedClient.py
 maestro_python_client/Client.py
 maestro_python_client/__init__.py
 maestro_python_client/test_CachedClient.py
 maestro_python_client.egg-info/PKG-INFO
```

### Comparing `maestro_python_client-0.9.4/setup.py` & `maestro_python_client-0.9.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,10 +55,11 @@
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3.10",
         "Topic :: Communications",
     ],
     # A fournir uniquement si votre licence n'est pas listée dans "classifiers"
     # ce qui est notre cas
     license="WTFPL",
+    scripts=["maestro_client"],
     # Il y a encore une chiée de paramètres possibles, mais avec ça vous
     # couvrez 90% des besoins
 )
```

