# Comparing `tmp/spectralib-0.0.3.tar.gz` & `tmp/spectralib-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spectralib-0.0.3.tar", last modified: Wed Apr 26 11:46:45 2023, max compression
+gzip compressed data, was "spectralib-0.0.4.tar", last modified: Wed Apr 26 11:51:05 2023, max compression
```

## Comparing `spectralib-0.0.3.tar` & `spectralib-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,25 @@
-drwxrwxrwx   0 jack      (1000) jack      (1000)        0 2023-04-26 11:46:45.354968 spectralib-0.0.3/
--rwxrwxrwx   0 jack      (1000) jack      (1000)      580 2023-04-26 11:46:45.351967 spectralib-0.0.3/PKG-INFO
--rwxrwxrwx   0 jack      (1000) jack      (1000)     1087 2023-04-26 11:24:27.000000 spectralib-0.0.3/README.md
--rwxrwxrwx   0 jack      (1000) jack      (1000)       38 2023-04-26 11:46:45.356970 spectralib-0.0.3/setup.cfg
--rwxrwxrwx   0 jack      (1000) jack      (1000)      766 2023-04-26 11:46:41.000000 spectralib-0.0.3/setup.py
-drwxrwxrwx   0 jack      (1000) jack      (1000)        0 2023-04-26 11:46:45.134904 spectralib-0.0.3/src/
-drwxrwxrwx   0 jack      (1000) jack      (1000)        0 2023-04-26 11:46:45.138419 spectralib-0.0.3/src/spectralib/
-drwxrwxrwx   0 jack      (1000) jack      (1000)        0 2023-04-26 11:46:45.312432 spectralib-0.0.3/src/spectralib/spectralib.egg-info/
--rwxrwxrwx   0 jack      (1000) jack      (1000)      580 2023-04-26 11:46:44.000000 spectralib-0.0.3/src/spectralib/spectralib.egg-info/PKG-INFO
--rwxrwxrwx   0 jack      (1000) jack      (1000)      214 2023-04-26 11:46:45.000000 spectralib-0.0.3/src/spectralib/spectralib.egg-info/SOURCES.txt
--rwxrwxrwx   0 jack      (1000) jack      (1000)        1 2023-04-26 11:46:44.000000 spectralib-0.0.3/src/spectralib/spectralib.egg-info/dependency_links.txt
--rwxrwxrwx   0 jack      (1000) jack      (1000)        1 2023-04-26 11:46:45.000000 spectralib-0.0.3/src/spectralib/spectralib.egg-info/top_level.txt
+drwxrwxrwx   0 jack      (1000) jack      (1000)        0 2023-04-26 11:51:05.877972 spectralib-0.0.4/
+-rwxrwxrwx   0 jack      (1000) jack      (1000)      580 2023-04-26 11:51:05.873434 spectralib-0.0.4/PKG-INFO
+-rwxrwxrwx   0 jack      (1000) jack      (1000)     1087 2023-04-26 11:24:27.000000 spectralib-0.0.4/README.md
+-rwxrwxrwx   0 jack      (1000) jack      (1000)       38 2023-04-26 11:51:05.879487 spectralib-0.0.4/setup.cfg
+-rwxrwxrwx   0 jack      (1000) jack      (1000)      744 2023-04-26 11:51:01.000000 spectralib-0.0.4/setup.py
+drwxrwxrwx   0 jack      (1000) jack      (1000)        0 2023-04-26 11:51:05.289531 spectralib-0.0.4/src/
+drwxrwxrwx   0 jack      (1000) jack      (1000)        0 2023-04-26 11:51:05.507487 spectralib-0.0.4/src/spectralib/
+-rwxrwxrwx   0 jack      (1000) jack      (1000)        0 2023-04-26 11:50:14.000000 spectralib-0.0.4/src/spectralib/__init__.py
+-rwxrwxrwx   0 jack      (1000) jack      (1000)     6921 2023-04-26 11:05:26.000000 spectralib-0.0.4/src/spectralib/filterbank.py
+-rwxrwxrwx   0 jack      (1000) jack      (1000)     1398 2023-04-26 10:33:13.000000 spectralib-0.0.4/src/spectralib/frb.py
+-rwxrwxrwx   0 jack      (1000) jack      (1000)        0 2023-04-26 10:33:24.000000 spectralib-0.0.4/src/spectralib/main.py
+-rwxrwxrwx   0 jack      (1000) jack      (1000)     3683 2023-04-26 10:33:33.000000 spectralib-0.0.4/src/spectralib/pulsar.py
+-rwxrwxrwx   0 jack      (1000) jack      (1000)     4892 2023-04-26 10:33:46.000000 spectralib-0.0.4/src/spectralib/rfi.py
+drwxrwxrwx   0 jack      (1000) jack      (1000)        0 2023-04-26 11:51:05.645349 spectralib-0.0.4/src/spectralib.egg-info/
+-rwxrwxrwx   0 jack      (1000) jack      (1000)      580 2023-04-26 11:51:05.000000 spectralib-0.0.4/src/spectralib.egg-info/PKG-INFO
+-rwxrwxrwx   0 jack      (1000) jack      (1000)      461 2023-04-26 11:51:05.000000 spectralib-0.0.4/src/spectralib.egg-info/SOURCES.txt
+-rwxrwxrwx   0 jack      (1000) jack      (1000)        1 2023-04-26 11:51:05.000000 spectralib-0.0.4/src/spectralib.egg-info/dependency_links.txt
+-rwxrwxrwx   0 jack      (1000) jack      (1000)       17 2023-04-26 11:51:05.000000 spectralib-0.0.4/src/spectralib.egg-info/top_level.txt
+drwxrwxrwx   0 jack      (1000) jack      (1000)        0 2023-04-26 11:51:05.839183 spectralib-0.0.4/src/tests/
+-rwxrwxrwx   0 jack      (1000) jack      (1000)        0 2023-04-26 11:50:43.000000 spectralib-0.0.4/src/tests/__init__.py
+-rwxrwxrwx   0 jack      (1000) jack      (1000)     3942 2023-04-26 10:33:55.000000 spectralib-0.0.4/src/tests/benchmark.py
+-rwxrwxrwx   0 jack      (1000) jack      (1000)     2520 2023-04-26 10:38:37.000000 spectralib-0.0.4/src/tests/test_filterbank.py
+-rwxrwxrwx   0 jack      (1000) jack      (1000)     1161 2023-04-26 10:38:42.000000 spectralib-0.0.4/src/tests/test_frb.py
+-rwxrwxrwx   0 jack      (1000) jack      (1000)     2087 2023-04-26 10:38:51.000000 spectralib-0.0.4/src/tests/test_pulsar.py
+-rwxrwxrwx   0 jack      (1000) jack      (1000)     1218 2023-04-26 10:38:58.000000 spectralib-0.0.4/src/tests/test_rfi.py
```

### Comparing `spectralib-0.0.3/PKG-INFO` & `spectralib-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectralib
-Version: 0.0.3
+Version: 0.0.4
 Summary: Synthetic Pulsar Emission, Contamination and Transients Radio Astronomy Library (SPECTRALib)
 Home-page: https://github.com/jack-white1/spectralib
 Author: Jack White
 Author-email: jack.white@eng.ox.ac.uk
 License: UNKNOWN
 Description: A python library for creating synthetic filterbank files (pulsars, FRBs, RFI) for radio astronomy. Integrate functions in your code or use standalone to generate custom datasets.
 Platform: UNKNOWN
```

### Comparing `spectralib-0.0.3/README.md` & `spectralib-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `spectralib-0.0.3/setup.py` & `spectralib-0.0.4/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name="spectralib",
-    version="0.0.3",
-    packages=find_packages(where="src/spectralib"),
-    package_dir={"": "src/spectralib"},
+    version="0.0.4",
+    packages=find_packages(where="src"),
+    package_dir={"": "src"},
     classifiers=[
         "Development Status :: 1 - Planning",
     ],
     author="Jack White",
     author_email="jack.white@eng.ox.ac.uk",
     description="Synthetic Pulsar Emission, Contamination and Transients Radio Astronomy Library (SPECTRALib)",
     long_description="A python library for creating synthetic filterbank files (pulsars, FRBs, RFI) for radio astronomy. Integrate functions in your code or use standalone to generate custom datasets.",
```

### Comparing `spectralib-0.0.3/src/spectralib/spectralib.egg-info/PKG-INFO` & `spectralib-0.0.4/src/spectralib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectralib
-Version: 0.0.3
+Version: 0.0.4
 Summary: Synthetic Pulsar Emission, Contamination and Transients Radio Astronomy Library (SPECTRALib)
 Home-page: https://github.com/jack-white1/spectralib
 Author: Jack White
 Author-email: jack.white@eng.ox.ac.uk
 License: UNKNOWN
 Description: A python library for creating synthetic filterbank files (pulsars, FRBs, RFI) for radio astronomy. Integrate functions in your code or use standalone to generate custom datasets.
 Platform: UNKNOWN
```

