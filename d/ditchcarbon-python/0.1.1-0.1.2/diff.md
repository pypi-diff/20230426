# Comparing `tmp/ditchcarbon-python-0.1.1.tar.gz` & `tmp/ditchcarbon-python-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ditchcarbon-python-0.1.1.tar", last modified: Wed Apr 26 15:46:17 2023, max compression
+gzip compressed data, was "ditchcarbon-python-0.1.2.tar", last modified: Wed Apr 26 15:50:07 2023, max compression
```

## Comparing `ditchcarbon-python-0.1.1.tar` & `ditchcarbon-python-0.1.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 armin     (1000) armin     (1000)        0 2023-04-26 15:46:17.968766 ditchcarbon-python-0.1.1/
--rw-r--r--   0 armin     (1000) armin     (1000)     1059 2023-04-23 21:47:24.000000 ditchcarbon-python-0.1.1/LICENSE
--rw-r--r--   0 armin     (1000) armin     (1000)     3973 2023-04-26 15:46:17.968766 ditchcarbon-python-0.1.1/PKG-INFO
--rw-r--r--   0 armin     (1000) armin     (1000)     2233 2023-04-26 15:43:25.000000 ditchcarbon-python-0.1.1/README.md
-drwxr-xr-x   0 armin     (1000) armin     (1000)        0 2023-04-26 15:46:17.968766 ditchcarbon-python-0.1.1/ditchcarbon_python/
--rw-r--r--   0 armin     (1000) armin     (1000)       27 2023-04-14 15:29:24.000000 ditchcarbon-python-0.1.1/ditchcarbon_python/__init__.py
--rw-r--r--   0 armin     (1000) armin     (1000)      235 2023-04-14 15:41:08.000000 ditchcarbon-python-0.1.1/ditchcarbon_python/auth.py
--rw-r--r--   0 armin     (1000) armin     (1000)     1213 2023-04-23 21:17:12.000000 ditchcarbon-python-0.1.1/ditchcarbon_python/client.py
--rw-r--r--   0 armin     (1000) armin     (1000)       46 2023-04-14 15:38:54.000000 ditchcarbon-python-0.1.1/ditchcarbon_python/constants.py
-drwxr-xr-x   0 armin     (1000) armin     (1000)        0 2023-04-26 15:46:17.968766 ditchcarbon-python-0.1.1/ditchcarbon_python/resources/
--rw-r--r--   0 armin     (1000) armin     (1000)        0 2023-04-14 15:44:02.000000 ditchcarbon-python-0.1.1/ditchcarbon_python/resources/__init__.py
--rw-r--r--   0 armin     (1000) armin     (1000)      542 2023-04-16 10:53:19.000000 ditchcarbon-python-0.1.1/ditchcarbon_python/resources/activities.py
--rw-r--r--   0 armin     (1000) armin     (1000)       73 2023-04-14 15:39:41.000000 ditchcarbon-python-0.1.1/ditchcarbon_python/resources/base.py
--rw-r--r--   0 armin     (1000) armin     (1000)      186 2023-04-16 10:48:39.000000 ditchcarbon-python-0.1.1/ditchcarbon_python/resources/categories.py
--rw-r--r--   0 armin     (1000) armin     (1000)      196 2023-04-16 10:44:50.000000 ditchcarbon-python-0.1.1/ditchcarbon_python/resources/expenses.py
--rw-r--r--   0 armin     (1000) armin     (1000)      194 2023-04-16 10:46:49.000000 ditchcarbon-python-0.1.1/ditchcarbon_python/resources/products.py
--rw-r--r--   0 armin     (1000) armin     (1000)      399 2023-04-16 10:40:00.000000 ditchcarbon-python-0.1.1/ditchcarbon_python/resources/servers.py
--rw-r--r--   0 armin     (1000) armin     (1000)      196 2023-04-16 10:41:44.000000 ditchcarbon-python-0.1.1/ditchcarbon_python/resources/suppliers.py
-drwxr-xr-x   0 armin     (1000) armin     (1000)        0 2023-04-26 15:46:17.968766 ditchcarbon-python-0.1.1/ditchcarbon_python.egg-info/
--rw-r--r--   0 armin     (1000) armin     (1000)     3973 2023-04-26 15:46:17.000000 ditchcarbon-python-0.1.1/ditchcarbon_python.egg-info/PKG-INFO
--rw-r--r--   0 armin     (1000) armin     (1000)      731 2023-04-26 15:46:17.000000 ditchcarbon-python-0.1.1/ditchcarbon_python.egg-info/SOURCES.txt
--rw-r--r--   0 armin     (1000) armin     (1000)        1 2023-04-26 15:46:17.000000 ditchcarbon-python-0.1.1/ditchcarbon_python.egg-info/dependency_links.txt
--rw-r--r--   0 armin     (1000) armin     (1000)       23 2023-04-26 15:46:17.000000 ditchcarbon-python-0.1.1/ditchcarbon_python.egg-info/requires.txt
--rw-r--r--   0 armin     (1000) armin     (1000)       19 2023-04-26 15:46:17.000000 ditchcarbon-python-0.1.1/ditchcarbon_python.egg-info/top_level.txt
--rw-r--r--   0 armin     (1000) armin     (1000)      784 2023-04-26 15:43:25.000000 ditchcarbon-python-0.1.1/pyproject.toml
--rw-r--r--   0 armin     (1000) armin     (1000)       38 2023-04-26 15:46:17.968766 ditchcarbon-python-0.1.1/setup.cfg
-drwxr-xr-x   0 armin     (1000) armin     (1000)        0 2023-04-26 15:46:17.968766 ditchcarbon-python-0.1.1/tests/
--rw-r--r--   0 armin     (1000) armin     (1000)     1441 2023-04-23 21:34:17.000000 ditchcarbon-python-0.1.1/tests/test_client.py
--rw-r--r--   0 armin     (1000) armin     (1000)      625 2023-04-23 21:34:54.000000 ditchcarbon-python-0.1.1/tests/test_servers.py
+drwxr-xr-x   0 armin     (1000) armin     (1000)        0 2023-04-26 15:50:07.380874 ditchcarbon-python-0.1.2/
+-rw-r--r--   0 armin     (1000) armin     (1000)     1059 2023-04-23 21:47:24.000000 ditchcarbon-python-0.1.2/LICENSE
+-rw-r--r--   0 armin     (1000) armin     (1000)     3980 2023-04-26 15:50:07.380874 ditchcarbon-python-0.1.2/PKG-INFO
+-rw-r--r--   0 armin     (1000) armin     (1000)     2233 2023-04-26 15:43:25.000000 ditchcarbon-python-0.1.2/README.md
+drwxr-xr-x   0 armin     (1000) armin     (1000)        0 2023-04-26 15:50:07.376874 ditchcarbon-python-0.1.2/ditchcarbon_python/
+-rw-r--r--   0 armin     (1000) armin     (1000)       27 2023-04-14 15:29:24.000000 ditchcarbon-python-0.1.2/ditchcarbon_python/__init__.py
+-rw-r--r--   0 armin     (1000) armin     (1000)      235 2023-04-14 15:41:08.000000 ditchcarbon-python-0.1.2/ditchcarbon_python/auth.py
+-rw-r--r--   0 armin     (1000) armin     (1000)     1213 2023-04-23 21:17:12.000000 ditchcarbon-python-0.1.2/ditchcarbon_python/client.py
+-rw-r--r--   0 armin     (1000) armin     (1000)       46 2023-04-14 15:38:54.000000 ditchcarbon-python-0.1.2/ditchcarbon_python/constants.py
+drwxr-xr-x   0 armin     (1000) armin     (1000)        0 2023-04-26 15:50:07.376874 ditchcarbon-python-0.1.2/ditchcarbon_python/resources/
+-rw-r--r--   0 armin     (1000) armin     (1000)        0 2023-04-14 15:44:02.000000 ditchcarbon-python-0.1.2/ditchcarbon_python/resources/__init__.py
+-rw-r--r--   0 armin     (1000) armin     (1000)      542 2023-04-16 10:53:19.000000 ditchcarbon-python-0.1.2/ditchcarbon_python/resources/activities.py
+-rw-r--r--   0 armin     (1000) armin     (1000)       73 2023-04-14 15:39:41.000000 ditchcarbon-python-0.1.2/ditchcarbon_python/resources/base.py
+-rw-r--r--   0 armin     (1000) armin     (1000)      186 2023-04-16 10:48:39.000000 ditchcarbon-python-0.1.2/ditchcarbon_python/resources/categories.py
+-rw-r--r--   0 armin     (1000) armin     (1000)      196 2023-04-16 10:44:50.000000 ditchcarbon-python-0.1.2/ditchcarbon_python/resources/expenses.py
+-rw-r--r--   0 armin     (1000) armin     (1000)      194 2023-04-16 10:46:49.000000 ditchcarbon-python-0.1.2/ditchcarbon_python/resources/products.py
+-rw-r--r--   0 armin     (1000) armin     (1000)      399 2023-04-16 10:40:00.000000 ditchcarbon-python-0.1.2/ditchcarbon_python/resources/servers.py
+-rw-r--r--   0 armin     (1000) armin     (1000)      196 2023-04-16 10:41:44.000000 ditchcarbon-python-0.1.2/ditchcarbon_python/resources/suppliers.py
+drwxr-xr-x   0 armin     (1000) armin     (1000)        0 2023-04-26 15:50:07.376874 ditchcarbon-python-0.1.2/ditchcarbon_python.egg-info/
+-rw-r--r--   0 armin     (1000) armin     (1000)     3980 2023-04-26 15:50:07.000000 ditchcarbon-python-0.1.2/ditchcarbon_python.egg-info/PKG-INFO
+-rw-r--r--   0 armin     (1000) armin     (1000)      731 2023-04-26 15:50:07.000000 ditchcarbon-python-0.1.2/ditchcarbon_python.egg-info/SOURCES.txt
+-rw-r--r--   0 armin     (1000) armin     (1000)        1 2023-04-26 15:50:07.000000 ditchcarbon-python-0.1.2/ditchcarbon_python.egg-info/dependency_links.txt
+-rw-r--r--   0 armin     (1000) armin     (1000)       23 2023-04-26 15:50:07.000000 ditchcarbon-python-0.1.2/ditchcarbon_python.egg-info/requires.txt
+-rw-r--r--   0 armin     (1000) armin     (1000)       19 2023-04-26 15:50:07.000000 ditchcarbon-python-0.1.2/ditchcarbon_python.egg-info/top_level.txt
+-rw-r--r--   0 armin     (1000) armin     (1000)      791 2023-04-26 15:48:36.000000 ditchcarbon-python-0.1.2/pyproject.toml
+-rw-r--r--   0 armin     (1000) armin     (1000)       38 2023-04-26 15:50:07.380874 ditchcarbon-python-0.1.2/setup.cfg
+drwxr-xr-x   0 armin     (1000) armin     (1000)        0 2023-04-26 15:50:07.380874 ditchcarbon-python-0.1.2/tests/
+-rw-r--r--   0 armin     (1000) armin     (1000)     1441 2023-04-23 21:34:17.000000 ditchcarbon-python-0.1.2/tests/test_client.py
+-rw-r--r--   0 armin     (1000) armin     (1000)      625 2023-04-23 21:34:54.000000 ditchcarbon-python-0.1.2/tests/test_servers.py
```

### Comparing `ditchcarbon-python-0.1.1/LICENSE` & `ditchcarbon-python-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ditchcarbon-python-0.1.1/PKG-INFO` & `ditchcarbon-python-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ditchcarbon-python
-Version: 0.1.1
-Summary: A Python wrapper for the DitchCarbon API
+Version: 0.1.2
+Summary: Official Python wrapper for the DitchCarbon API
 Author-email: DitchCarbon <enquiries@ditchcarbon.com>
 License: Copyright 2023 DitchCarbon
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `ditchcarbon-python-0.1.1/README.md` & `ditchcarbon-python-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `ditchcarbon-python-0.1.1/ditchcarbon_python/client.py` & `ditchcarbon-python-0.1.2/ditchcarbon_python/client.py`

 * *Files identical despite different names*

### Comparing `ditchcarbon-python-0.1.1/ditchcarbon_python/resources/activities.py` & `ditchcarbon-python-0.1.2/ditchcarbon_python/resources/activities.py`

 * *Files identical despite different names*

### Comparing `ditchcarbon-python-0.1.1/ditchcarbon_python.egg-info/PKG-INFO` & `ditchcarbon-python-0.1.2/ditchcarbon_python.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ditchcarbon-python
-Version: 0.1.1
-Summary: A Python wrapper for the DitchCarbon API
+Version: 0.1.2
+Summary: Official Python wrapper for the DitchCarbon API
 Author-email: DitchCarbon <enquiries@ditchcarbon.com>
 License: Copyright 2023 DitchCarbon
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `ditchcarbon-python-0.1.1/ditchcarbon_python.egg-info/SOURCES.txt` & `ditchcarbon-python-0.1.2/ditchcarbon_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ditchcarbon-python-0.1.1/pyproject.toml` & `ditchcarbon-python-0.1.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ditchcarbon-python"
-version = "0.1.1"
-description = "A Python wrapper for the DitchCarbon API"
+version = "0.1.2"
+description = "Official Python wrapper for the DitchCarbon API"
 readme = "README.md"
 authors = [{ name = "DitchCarbon", email = "enquiries@ditchcarbon.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `ditchcarbon-python-0.1.1/tests/test_client.py` & `ditchcarbon-python-0.1.2/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `ditchcarbon-python-0.1.1/tests/test_servers.py` & `ditchcarbon-python-0.1.2/tests/test_servers.py`

 * *Files identical despite different names*

