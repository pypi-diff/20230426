# Comparing `tmp/pyastroweatherio-0.23.1.tar.gz` & `tmp/pyastroweatherio-0.23.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyastroweatherio-0.23.1.tar", last modified: Wed Apr 26 03:45:55 2023, max compression
+gzip compressed data, was "pyastroweatherio-0.23.2.tar", last modified: Wed Apr 26 14:11:23 2023, max compression
```

## Comparing `pyastroweatherio-0.23.1.tar` & `pyastroweatherio-0.23.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-04-26 03:45:55.960012 pyastroweatherio-0.23.1/
--rw-rw-r--   0 markus    (1000) markus    (1000)     1071 2023-04-10 18:40:11.000000 pyastroweatherio-0.23.1/LICENSE
--rw-rw-r--   0 markus    (1000) markus    (1000)      861 2023-04-26 03:45:55.960012 pyastroweatherio-0.23.1/PKG-INFO
--rw-rw-r--   0 markus    (1000) markus    (1000)     3538 2023-04-24 06:36:59.000000 pyastroweatherio-0.23.1/README.md
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-04-26 03:45:55.956012 pyastroweatherio-0.23.1/pyastroweatherio/
--rw-rw-r--   0 markus    (1000) markus    (1000)      285 2023-04-10 18:40:11.000000 pyastroweatherio-0.23.1/pyastroweatherio/__init__.py
--rw-rw-r--   0 markus    (1000) markus    (1000)    25577 2023-04-26 03:44:28.000000 pyastroweatherio-0.23.1/pyastroweatherio/client.py
--rw-rw-r--   0 markus    (1000) markus    (1000)     4474 2023-04-26 03:44:35.000000 pyastroweatherio-0.23.1/pyastroweatherio/const.py
--rw-rw-r--   0 markus    (1000) markus    (1000)    16844 2023-04-24 06:36:59.000000 pyastroweatherio-0.23.1/pyastroweatherio/dataclasses.py
--rw-rw-r--   0 markus    (1000) markus    (1000)      337 2023-04-10 18:40:11.000000 pyastroweatherio-0.23.1/pyastroweatherio/errors.py
--rw-rw-r--   0 markus    (1000) markus    (1000)    14262 2023-04-24 06:36:59.000000 pyastroweatherio-0.23.1/pyastroweatherio/helper_functions.py
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-04-26 03:45:55.960012 pyastroweatherio-0.23.1/pyastroweatherio.egg-info/
--rw-rw-r--   0 markus    (1000) markus    (1000)      861 2023-04-26 03:45:55.000000 pyastroweatherio-0.23.1/pyastroweatherio.egg-info/PKG-INFO
--rw-rw-r--   0 markus    (1000) markus    (1000)      413 2023-04-26 03:45:55.000000 pyastroweatherio-0.23.1/pyastroweatherio.egg-info/SOURCES.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)        1 2023-04-26 03:45:55.000000 pyastroweatherio-0.23.1/pyastroweatherio.egg-info/dependency_links.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)       16 2023-04-26 03:45:55.000000 pyastroweatherio-0.23.1/pyastroweatherio.egg-info/requires.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)       17 2023-04-26 03:45:55.000000 pyastroweatherio-0.23.1/pyastroweatherio.egg-info/top_level.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)       79 2023-04-26 03:45:55.960012 pyastroweatherio-0.23.1/setup.cfg
--rw-rw-r--   0 markus    (1000) markus    (1000)     1169 2023-04-26 03:45:17.000000 pyastroweatherio-0.23.1/setup.py
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-04-26 14:11:23.475766 pyastroweatherio-0.23.2/
+-rw-rw-r--   0 markus    (1000) markus    (1000)     1071 2023-04-10 18:40:11.000000 pyastroweatherio-0.23.2/LICENSE
+-rw-rw-r--   0 markus    (1000) markus    (1000)      889 2023-04-26 14:11:23.475766 pyastroweatherio-0.23.2/PKG-INFO
+-rw-rw-r--   0 markus    (1000) markus    (1000)     3538 2023-04-24 06:36:59.000000 pyastroweatherio-0.23.2/README.md
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-04-26 14:11:23.475766 pyastroweatherio-0.23.2/pyastroweatherio/
+-rw-rw-r--   0 markus    (1000) markus    (1000)      285 2023-04-10 18:40:11.000000 pyastroweatherio-0.23.2/pyastroweatherio/__init__.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)    25577 2023-04-26 03:44:28.000000 pyastroweatherio-0.23.2/pyastroweatherio/client.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)     4474 2023-04-26 03:44:35.000000 pyastroweatherio-0.23.2/pyastroweatherio/const.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)    16844 2023-04-24 06:36:59.000000 pyastroweatherio-0.23.2/pyastroweatherio/dataclasses.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)      337 2023-04-10 18:40:11.000000 pyastroweatherio-0.23.2/pyastroweatherio/errors.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)    14262 2023-04-26 04:29:12.000000 pyastroweatherio-0.23.2/pyastroweatherio/helper_functions.py
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-04-26 14:11:23.475766 pyastroweatherio-0.23.2/pyastroweatherio.egg-info/
+-rw-rw-r--   0 markus    (1000) markus    (1000)      889 2023-04-26 14:11:23.000000 pyastroweatherio-0.23.2/pyastroweatherio.egg-info/PKG-INFO
+-rw-rw-r--   0 markus    (1000) markus    (1000)      413 2023-04-26 14:11:23.000000 pyastroweatherio-0.23.2/pyastroweatherio.egg-info/SOURCES.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)        1 2023-04-26 14:11:23.000000 pyastroweatherio-0.23.2/pyastroweatherio.egg-info/dependency_links.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)       16 2023-04-26 14:11:23.000000 pyastroweatherio-0.23.2/pyastroweatherio.egg-info/requires.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)       17 2023-04-26 14:11:23.000000 pyastroweatherio-0.23.2/pyastroweatherio.egg-info/top_level.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)       79 2023-04-26 14:11:23.475766 pyastroweatherio-0.23.2/setup.cfg
+-rw-rw-r--   0 markus    (1000) markus    (1000)     1235 2023-04-26 14:11:07.000000 pyastroweatherio-0.23.2/setup.py
```

### Comparing `pyastroweatherio-0.23.1/LICENSE` & `pyastroweatherio-0.23.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyastroweatherio-0.23.1/PKG-INFO` & `pyastroweatherio-0.23.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: pyastroweatherio
-Version: 0.23.1
-Summary: Python Wrapper for 7Timer REST API
+Version: 0.23.2
+Summary: Python Wrapper for 7Timer and Met.no REST API
 Home-page: https://github.com/mawinkler/pyastroweatherio
 Author: Markus Winkler
 Author-email: winkler.info@icloud.com
 License: MIT
-Keywords: AstroWeather,7Timer,Python
-Classifier: Development Status :: 3 - Alpha
+Keywords: AstroWeather,7Timer,Met.no,Python
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 License-File: LICENSE
 
-Lightweight Python 3 module to receive data via REST API from 7Timer.
+Lightweight Python 3 module to receive data via REST API from 7Timer and Met.no.
```

### Comparing `pyastroweatherio-0.23.1/README.md` & `pyastroweatherio-0.23.2/README.md`

 * *Files identical despite different names*

### Comparing `pyastroweatherio-0.23.1/pyastroweatherio/client.py` & `pyastroweatherio-0.23.2/pyastroweatherio/client.py`

 * *Files identical despite different names*

### Comparing `pyastroweatherio-0.23.1/pyastroweatherio/const.py` & `pyastroweatherio-0.23.2/pyastroweatherio/const.py`

 * *Files identical despite different names*

### Comparing `pyastroweatherio-0.23.1/pyastroweatherio/dataclasses.py` & `pyastroweatherio-0.23.2/pyastroweatherio/dataclasses.py`

 * *Files identical despite different names*

### Comparing `pyastroweatherio-0.23.1/pyastroweatherio/helper_functions.py` & `pyastroweatherio-0.23.2/pyastroweatherio/helper_functions.py`

 * *Files identical despite different names*

### Comparing `pyastroweatherio-0.23.1/pyastroweatherio.egg-info/PKG-INFO` & `pyastroweatherio-0.23.2/pyastroweatherio.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: pyastroweatherio
-Version: 0.23.1
-Summary: Python Wrapper for 7Timer REST API
+Version: 0.23.2
+Summary: Python Wrapper for 7Timer and Met.no REST API
 Home-page: https://github.com/mawinkler/pyastroweatherio
 Author: Markus Winkler
 Author-email: winkler.info@icloud.com
 License: MIT
-Keywords: AstroWeather,7Timer,Python
-Classifier: Development Status :: 3 - Alpha
+Keywords: AstroWeather,7Timer,Met.no,Python
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 License-File: LICENSE
 
-Lightweight Python 3 module to receive data via REST API from 7Timer.
+Lightweight Python 3 module to receive data via REST API from 7Timer and Met.no.
```

### Comparing `pyastroweatherio-0.23.1/setup.py` & `pyastroweatherio-0.23.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 from setuptools import setup
 
 setup(
     name="pyastroweatherio",
     packages=["pyastroweatherio"],
-    version="0.23.1",
+    version="0.23.2",
     license="MIT",
-    description="Python Wrapper for 7Timer REST API",
+    description="Python Wrapper for 7Timer and Met.no REST API",
     long_description=" ".join(
-        ["Lightweight Python 3 module to receive data via", "REST API from 7Timer."],
+        [
+            "Lightweight Python 3 module to receive data via",
+            "REST API from 7Timer and Met.no.",
+        ],
     ),
     author="Markus Winkler",
     author_email="winkler.info@icloud.com",
     url="https://github.com/mawinkler/pyastroweatherio",
-    keywords=["AstroWeather", "7Timer", "Python"],
+    keywords=["AstroWeather", "7Timer", "Met.no", "Python"],
     install_requires=["aiohttp", "pyephem"],
     classifiers=[
         # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
-        "Development Status :: 3 - Alpha",
+        "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Build Tools",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
```

