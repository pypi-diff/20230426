# Comparing `tmp/pyastroweatherio-0.23.0.dev3.tar.gz` & `tmp/pyastroweatherio-0.23.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyastroweatherio-0.23.0.dev3.tar", last modified: Tue Apr 11 11:27:34 2023, max compression
+gzip compressed data, was "pyastroweatherio-0.23.1.tar", last modified: Wed Apr 26 03:45:55 2023, max compression
```

## Comparing `pyastroweatherio-0.23.0.dev3.tar` & `pyastroweatherio-0.23.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-04-11 11:27:34.583760 pyastroweatherio-0.23.0.dev3/
--rw-rw-r--   0 markus    (1000) markus    (1000)     1071 2023-04-10 18:40:11.000000 pyastroweatherio-0.23.0.dev3/LICENSE
--rw-rw-r--   0 markus    (1000) markus    (1000)      866 2023-04-11 11:27:34.583760 pyastroweatherio-0.23.0.dev3/PKG-INFO
--rw-rw-r--   0 markus    (1000) markus    (1000)     3538 2023-04-10 18:28:08.000000 pyastroweatherio-0.23.0.dev3/README.md
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-04-11 11:27:34.575760 pyastroweatherio-0.23.0.dev3/pyastroweatherio/
--rw-rw-r--   0 markus    (1000) markus    (1000)      285 2023-04-10 18:40:11.000000 pyastroweatherio-0.23.0.dev3/pyastroweatherio/__init__.py
--rw-rw-r--   0 markus    (1000) markus    (1000)    25576 2023-04-11 11:25:21.000000 pyastroweatherio-0.23.0.dev3/pyastroweatherio/client.py
--rw-rw-r--   0 markus    (1000) markus    (1000)     4473 2023-04-08 14:28:26.000000 pyastroweatherio-0.23.0.dev3/pyastroweatherio/const.py
--rw-rw-r--   0 markus    (1000) markus    (1000)    16844 2023-04-10 15:29:18.000000 pyastroweatherio-0.23.0.dev3/pyastroweatherio/dataclasses.py
--rw-rw-r--   0 markus    (1000) markus    (1000)      337 2023-04-10 18:40:11.000000 pyastroweatherio-0.23.0.dev3/pyastroweatherio/errors.py
--rw-rw-r--   0 markus    (1000) markus    (1000)    14262 2023-04-10 18:34:19.000000 pyastroweatherio-0.23.0.dev3/pyastroweatherio/helper_functions.py
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-04-11 11:27:34.583760 pyastroweatherio-0.23.0.dev3/pyastroweatherio.egg-info/
--rw-rw-r--   0 markus    (1000) markus    (1000)      866 2023-04-11 11:27:34.000000 pyastroweatherio-0.23.0.dev3/pyastroweatherio.egg-info/PKG-INFO
--rw-rw-r--   0 markus    (1000) markus    (1000)      413 2023-04-11 11:27:34.000000 pyastroweatherio-0.23.0.dev3/pyastroweatherio.egg-info/SOURCES.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)        1 2023-04-11 11:27:34.000000 pyastroweatherio-0.23.0.dev3/pyastroweatherio.egg-info/dependency_links.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)       16 2023-04-11 11:27:34.000000 pyastroweatherio-0.23.0.dev3/pyastroweatherio.egg-info/requires.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)       17 2023-04-11 11:27:34.000000 pyastroweatherio-0.23.0.dev3/pyastroweatherio.egg-info/top_level.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)       79 2023-04-11 11:27:34.583760 pyastroweatherio-0.23.0.dev3/setup.cfg
--rw-rw-r--   0 markus    (1000) markus    (1000)     1174 2023-04-11 11:26:18.000000 pyastroweatherio-0.23.0.dev3/setup.py
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-04-26 03:45:55.960012 pyastroweatherio-0.23.1/
+-rw-rw-r--   0 markus    (1000) markus    (1000)     1071 2023-04-10 18:40:11.000000 pyastroweatherio-0.23.1/LICENSE
+-rw-rw-r--   0 markus    (1000) markus    (1000)      861 2023-04-26 03:45:55.960012 pyastroweatherio-0.23.1/PKG-INFO
+-rw-rw-r--   0 markus    (1000) markus    (1000)     3538 2023-04-24 06:36:59.000000 pyastroweatherio-0.23.1/README.md
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-04-26 03:45:55.956012 pyastroweatherio-0.23.1/pyastroweatherio/
+-rw-rw-r--   0 markus    (1000) markus    (1000)      285 2023-04-10 18:40:11.000000 pyastroweatherio-0.23.1/pyastroweatherio/__init__.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)    25577 2023-04-26 03:44:28.000000 pyastroweatherio-0.23.1/pyastroweatherio/client.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)     4474 2023-04-26 03:44:35.000000 pyastroweatherio-0.23.1/pyastroweatherio/const.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)    16844 2023-04-24 06:36:59.000000 pyastroweatherio-0.23.1/pyastroweatherio/dataclasses.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)      337 2023-04-10 18:40:11.000000 pyastroweatherio-0.23.1/pyastroweatherio/errors.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)    14262 2023-04-24 06:36:59.000000 pyastroweatherio-0.23.1/pyastroweatherio/helper_functions.py
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-04-26 03:45:55.960012 pyastroweatherio-0.23.1/pyastroweatherio.egg-info/
+-rw-rw-r--   0 markus    (1000) markus    (1000)      861 2023-04-26 03:45:55.000000 pyastroweatherio-0.23.1/pyastroweatherio.egg-info/PKG-INFO
+-rw-rw-r--   0 markus    (1000) markus    (1000)      413 2023-04-26 03:45:55.000000 pyastroweatherio-0.23.1/pyastroweatherio.egg-info/SOURCES.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)        1 2023-04-26 03:45:55.000000 pyastroweatherio-0.23.1/pyastroweatherio.egg-info/dependency_links.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)       16 2023-04-26 03:45:55.000000 pyastroweatherio-0.23.1/pyastroweatherio.egg-info/requires.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)       17 2023-04-26 03:45:55.000000 pyastroweatherio-0.23.1/pyastroweatherio.egg-info/top_level.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)       79 2023-04-26 03:45:55.960012 pyastroweatherio-0.23.1/setup.cfg
+-rw-rw-r--   0 markus    (1000) markus    (1000)     1169 2023-04-26 03:45:17.000000 pyastroweatherio-0.23.1/setup.py
```

### Comparing `pyastroweatherio-0.23.0.dev3/LICENSE` & `pyastroweatherio-0.23.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyastroweatherio-0.23.0.dev3/PKG-INFO` & `pyastroweatherio-0.23.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyastroweatherio
-Version: 0.23.0.dev3
+Version: 0.23.1
 Summary: Python Wrapper for 7Timer REST API
 Home-page: https://github.com/mawinkler/pyastroweatherio
 Author: Markus Winkler
 Author-email: winkler.info@icloud.com
 License: MIT
 Keywords: AstroWeather,7Timer,Python
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pyastroweatherio-0.23.0.dev3/README.md` & `pyastroweatherio-0.23.1/README.md`

 * *Files identical despite different names*

### Comparing `pyastroweatherio-0.23.0.dev3/pyastroweatherio/client.py` & `pyastroweatherio-0.23.1/pyastroweatherio/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -529,15 +529,15 @@
         if use_running_session:
             session = self._session
         else:
             session = ClientSession(
                 timeout=ClientTimeout(total=DEFAULT_TIMEOUT),
             )
 
-        # BASE_URL_SEVENTIMER = "http://www.7timer.info/bin/api.pl?lon=XX.XX&lat=YY.YY&product=astro&output=json"
+        # BASE_URL_SEVENTIMER = "https://www.7timer.info/bin/api.pl?lon=XX.XX&lat=YY.YY&product=astro&output=json"
         # STIMER_OUTPUT = "json"
         url = (
             str(f"{BASE_URL_SEVENTIMER}")
             + "?lon="
             + str("%.1f" % round(self._longitude, 2))
             + "&lat="
             + str("%.1f" % round(self._latitude, 2))
```

### Comparing `pyastroweatherio-0.23.0.dev3/pyastroweatherio/const.py` & `pyastroweatherio-0.23.1/pyastroweatherio/const.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Constant Definitions for AstroWeather."""
 
-BASE_URL_SEVENTIMER = "http://www.7timer.info/bin/api.pl"
+BASE_URL_SEVENTIMER = "https://www.7timer.info/bin/api.pl"
 BASE_URL_MET = "https://api.met.no/weatherapi/locationforecast/2.0/complete"
 STIMER_OUTPUT = "json"
 
 DEFAULT_TIMEOUT = 10
 DEFAULT_CACHE_TIMEOUT = 1770
 DEFAULT_ELEVATION = 0
 DEFAULT_TIMEZONE = "Etc/UTC"
```

### Comparing `pyastroweatherio-0.23.0.dev3/pyastroweatherio/dataclasses.py` & `pyastroweatherio-0.23.1/pyastroweatherio/dataclasses.py`

 * *Files identical despite different names*

### Comparing `pyastroweatherio-0.23.0.dev3/pyastroweatherio/helper_functions.py` & `pyastroweatherio-0.23.1/pyastroweatherio/helper_functions.py`

 * *Files identical despite different names*

### Comparing `pyastroweatherio-0.23.0.dev3/pyastroweatherio.egg-info/PKG-INFO` & `pyastroweatherio-0.23.1/pyastroweatherio.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyastroweatherio
-Version: 0.23.0.dev3
+Version: 0.23.1
 Summary: Python Wrapper for 7Timer REST API
 Home-page: https://github.com/mawinkler/pyastroweatherio
 Author: Markus Winkler
 Author-email: winkler.info@icloud.com
 License: MIT
 Keywords: AstroWeather,7Timer,Python
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pyastroweatherio-0.23.0.dev3/setup.py` & `pyastroweatherio-0.23.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 setup(
     name="pyastroweatherio",
     packages=["pyastroweatherio"],
-    version="0.23.0.dev3",
+    version="0.23.1",
     license="MIT",
     description="Python Wrapper for 7Timer REST API",
     long_description=" ".join(
         ["Lightweight Python 3 module to receive data via", "REST API from 7Timer."],
     ),
     author="Markus Winkler",
     author_email="winkler.info@icloud.com",
```

