# Comparing `tmp/netml-0.5.0.tar.gz` & `tmp/netml-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netml-0.5.0.tar", last modified: Tue Apr 25 17:00:14 2023, max compression
+gzip compressed data, was "netml-0.5.1.tar", last modified: Tue Apr 25 17:28:52 2023, max compression
```

## Comparing `netml-0.5.0.tar` & `netml-0.5.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 jslondon  (1000) jslondon  (1000)        0 2023-04-25 17:00:14.570410 netml-0.5.0/
--rw-rw-r--   0 jslondon  (1000) jslondon  (1000)    11357 2022-11-01 17:33:24.000000 netml-0.5.0/LICENSE
--rw-rw-r--   0 jslondon  (1000) jslondon  (1000)    10762 2023-04-25 17:00:14.570410 netml-0.5.0/PKG-INFO
--rw-rw-r--   0 jslondon  (1000) jslondon  (1000)     9665 2022-11-03 16:45:28.000000 netml-0.5.0/README.md
--rw-rw-r--   0 jslondon  (1000) jslondon  (1000)      198 2023-04-25 17:00:14.570410 netml-0.5.0/setup.cfg
--rw-rw-r--   0 jslondon  (1000) jslondon  (1000)     2157 2023-04-25 16:55:05.000000 netml-0.5.0/setup.py
-drwxrwxr-x   0 jslondon  (1000) jslondon  (1000)        0 2023-04-25 17:00:14.566410 netml-0.5.0/src/
-drwxrwxr-x   0 jslondon  (1000) jslondon  (1000)        0 2023-04-25 17:00:14.566410 netml-0.5.0/src/netml/
--rw-rw-r--   0 jslondon  (1000) jslondon  (1000)       22 2023-04-25 16:55:05.000000 netml-0.5.0/src/netml/__init__.py
--rw-rw-r--   0 jslondon  (1000) jslondon  (1000)    24337 2022-11-01 15:28:07.000000 netml-0.5.0/src/netml/cli.py
-drwxrwxr-x   0 jslondon  (1000) jslondon  (1000)        0 2023-04-25 17:00:14.570410 netml-0.5.0/src/netml/ndm/
--rw-r--r--   0 jslondon  (1000) jslondon  (1000)        0 2020-08-10 22:55:55.000000 netml-0.5.0/src/netml/ndm/__init__.py
--rw-rw-r--   0 jslondon  (1000) jslondon  (1000)     7233 2020-09-23 18:19:58.000000 netml-0.5.0/src/netml/ndm/ae.py
--rw-r--r--   0 jslondon  (1000) jslondon  (1000)     5814 2020-08-10 22:55:55.000000 netml-0.5.0/src/netml/ndm/gmm.py
--rw-r--r--   0 jslondon  (1000) jslondon  (1000)     3180 2020-08-10 22:55:55.000000 netml-0.5.0/src/netml/ndm/iforest.py
--rw-r--r--   0 jslondon  (1000) jslondon  (1000)     4452 2020-08-10 22:55:55.000000 netml-0.5.0/src/netml/ndm/kde.py
--rw-rw-r--   0 jslondon  (1000) jslondon  (1000)     3161 2022-10-11 16:56:47.000000 netml-0.5.0/src/netml/ndm/model.py
--rw-rw-r--   0 jslondon  (1000) jslondon  (1000)     2542 2022-10-11 17:02:08.000000 netml-0.5.0/src/netml/ndm/ocsvm.py
--rw-r--r--   0 jslondon  (1000) jslondon  (1000)     4409 2020-08-10 22:55:55.000000 netml-0.5.0/src/netml/ndm/pca.py
-drwxrwxr-x   0 jslondon  (1000) jslondon  (1000)        0 2023-04-25 17:00:14.570410 netml-0.5.0/src/netml/pparser/
--rw-r--r--   0 jslondon  (1000) jslondon  (1000)        0 2020-08-10 22:55:55.000000 netml-0.5.0/src/netml/pparser/__init__.py
--rw-rw-r--   0 jslondon  (1000) jslondon  (1000)    37110 2022-11-01 17:29:58.000000 netml-0.5.0/src/netml/pparser/parser.py
-drwxrwxr-x   0 jslondon  (1000) jslondon  (1000)        0 2023-04-25 17:00:14.570410 netml-0.5.0/src/netml/utils/
--rw-r--r--   0 jslondon  (1000) jslondon  (1000)        0 2020-08-10 22:55:55.000000 netml-0.5.0/src/netml/utils/__init__.py
--rw-rw-r--   0 jslondon  (1000) jslondon  (1000)     3716 2020-09-23 18:19:58.000000 netml-0.5.0/src/netml/utils/tool.py
-drwxrwxr-x   0 jslondon  (1000) jslondon  (1000)        0 2023-04-25 17:00:14.570410 netml-0.5.0/src/netml/visual/
--rw-r--r--   0 jslondon  (1000) jslondon  (1000)        0 2020-08-10 22:55:55.000000 netml-0.5.0/src/netml/visual/__init__.py
-drwxrwxr-x   0 jslondon  (1000) jslondon  (1000)        0 2023-04-25 17:00:14.566410 netml-0.5.0/src/netml.egg-info/
--rw-r--r--   0 jslondon  (1000) jslondon  (1000)    10762 2023-04-25 17:00:14.000000 netml-0.5.0/src/netml.egg-info/PKG-INFO
--rw-r--r--   0 jslondon  (1000) jslondon  (1000)      594 2023-04-25 17:00:14.000000 netml-0.5.0/src/netml.egg-info/SOURCES.txt
--rw-r--r--   0 jslondon  (1000) jslondon  (1000)        1 2023-04-25 17:00:14.000000 netml-0.5.0/src/netml.egg-info/dependency_links.txt
--rw-r--r--   0 jslondon  (1000) jslondon  (1000)       51 2023-04-25 17:00:14.000000 netml-0.5.0/src/netml.egg-info/entry_points.txt
--rw-r--r--   0 jslondon  (1000) jslondon  (1000)      310 2023-04-25 17:00:14.000000 netml-0.5.0/src/netml.egg-info/requires.txt
--rw-r--r--   0 jslondon  (1000) jslondon  (1000)        6 2023-04-25 17:00:14.000000 netml-0.5.0/src/netml.egg-info/top_level.txt
+drwxrwxr-x   0 jslondon  (1000) jslondon  (1000)        0 2023-04-25 17:28:52.663817 netml-0.5.1/
+-rw-rw-r--   0 jslondon  (1000) jslondon  (1000)    11357 2022-11-01 17:33:24.000000 netml-0.5.1/LICENSE
+-rw-rw-r--   0 jslondon  (1000) jslondon  (1000)    10762 2023-04-25 17:28:52.663817 netml-0.5.1/PKG-INFO
+-rw-rw-r--   0 jslondon  (1000) jslondon  (1000)     9665 2022-11-03 16:45:28.000000 netml-0.5.1/README.md
+-rw-rw-r--   0 jslondon  (1000) jslondon  (1000)      198 2023-04-25 17:28:52.663817 netml-0.5.1/setup.cfg
+-rw-rw-r--   0 jslondon  (1000) jslondon  (1000)     2387 2023-04-25 17:26:45.000000 netml-0.5.1/setup.py
+drwxrwxr-x   0 jslondon  (1000) jslondon  (1000)        0 2023-04-25 17:28:52.659817 netml-0.5.1/src/
+drwxrwxr-x   0 jslondon  (1000) jslondon  (1000)        0 2023-04-25 17:28:52.659817 netml-0.5.1/src/netml/
+-rw-rw-r--   0 jslondon  (1000) jslondon  (1000)       22 2023-04-25 17:26:45.000000 netml-0.5.1/src/netml/__init__.py
+-rw-rw-r--   0 jslondon  (1000) jslondon  (1000)    24337 2022-11-01 15:28:07.000000 netml-0.5.1/src/netml/cli.py
+drwxrwxr-x   0 jslondon  (1000) jslondon  (1000)        0 2023-04-25 17:28:52.663817 netml-0.5.1/src/netml/ndm/
+-rw-r--r--   0 jslondon  (1000) jslondon  (1000)        0 2020-08-10 22:55:55.000000 netml-0.5.1/src/netml/ndm/__init__.py
+-rw-rw-r--   0 jslondon  (1000) jslondon  (1000)     7233 2020-09-23 18:19:58.000000 netml-0.5.1/src/netml/ndm/ae.py
+-rw-r--r--   0 jslondon  (1000) jslondon  (1000)     5814 2020-08-10 22:55:55.000000 netml-0.5.1/src/netml/ndm/gmm.py
+-rw-r--r--   0 jslondon  (1000) jslondon  (1000)     3180 2020-08-10 22:55:55.000000 netml-0.5.1/src/netml/ndm/iforest.py
+-rw-r--r--   0 jslondon  (1000) jslondon  (1000)     4452 2020-08-10 22:55:55.000000 netml-0.5.1/src/netml/ndm/kde.py
+-rw-rw-r--   0 jslondon  (1000) jslondon  (1000)     3161 2022-10-11 16:56:47.000000 netml-0.5.1/src/netml/ndm/model.py
+-rw-rw-r--   0 jslondon  (1000) jslondon  (1000)     2542 2022-10-11 17:02:08.000000 netml-0.5.1/src/netml/ndm/ocsvm.py
+-rw-r--r--   0 jslondon  (1000) jslondon  (1000)     4409 2020-08-10 22:55:55.000000 netml-0.5.1/src/netml/ndm/pca.py
+drwxrwxr-x   0 jslondon  (1000) jslondon  (1000)        0 2023-04-25 17:28:52.663817 netml-0.5.1/src/netml/pparser/
+-rw-r--r--   0 jslondon  (1000) jslondon  (1000)        0 2020-08-10 22:55:55.000000 netml-0.5.1/src/netml/pparser/__init__.py
+-rw-rw-r--   0 jslondon  (1000) jslondon  (1000)    37110 2022-11-01 17:29:58.000000 netml-0.5.1/src/netml/pparser/parser.py
+drwxrwxr-x   0 jslondon  (1000) jslondon  (1000)        0 2023-04-25 17:28:52.663817 netml-0.5.1/src/netml/utils/
+-rw-r--r--   0 jslondon  (1000) jslondon  (1000)        0 2020-08-10 22:55:55.000000 netml-0.5.1/src/netml/utils/__init__.py
+-rw-rw-r--   0 jslondon  (1000) jslondon  (1000)     3716 2020-09-23 18:19:58.000000 netml-0.5.1/src/netml/utils/tool.py
+drwxrwxr-x   0 jslondon  (1000) jslondon  (1000)        0 2023-04-25 17:28:52.663817 netml-0.5.1/src/netml/visual/
+-rw-r--r--   0 jslondon  (1000) jslondon  (1000)        0 2020-08-10 22:55:55.000000 netml-0.5.1/src/netml/visual/__init__.py
+drwxrwxr-x   0 jslondon  (1000) jslondon  (1000)        0 2023-04-25 17:28:52.663817 netml-0.5.1/src/netml.egg-info/
+-rw-r--r--   0 jslondon  (1000) jslondon  (1000)    10762 2023-04-25 17:28:52.000000 netml-0.5.1/src/netml.egg-info/PKG-INFO
+-rw-r--r--   0 jslondon  (1000) jslondon  (1000)      594 2023-04-25 17:28:52.000000 netml-0.5.1/src/netml.egg-info/SOURCES.txt
+-rw-r--r--   0 jslondon  (1000) jslondon  (1000)        1 2023-04-25 17:28:52.000000 netml-0.5.1/src/netml.egg-info/dependency_links.txt
+-rw-r--r--   0 jslondon  (1000) jslondon  (1000)       51 2023-04-25 17:28:52.000000 netml-0.5.1/src/netml.egg-info/entry_points.txt
+-rw-r--r--   0 jslondon  (1000) jslondon  (1000)      327 2023-04-25 17:28:52.000000 netml-0.5.1/src/netml.egg-info/requires.txt
+-rw-r--r--   0 jslondon  (1000) jslondon  (1000)        6 2023-04-25 17:28:52.000000 netml-0.5.1/src/netml.egg-info/top_level.txt
```

### Comparing `netml-0.5.0/LICENSE` & `netml-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `netml-0.5.0/PKG-INFO` & `netml-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netml
-Version: 0.5.0
+Version: 0.5.1
 Summary: Feature Extraction and Machine Learning from Network Traffic Traces
 Home-page: https://github.com/noise-lab/netml
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `netml-0.5.0/README.md` & `netml-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `netml-0.5.0/setup.py` & `netml-0.5.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,23 @@
 
 from setuptools import find_packages, setup
 
 
 README_PATH = pathlib.Path(__file__).parent / 'README.md'
 
 INSTALL_REQUIRES = [
+    #
+    # numba is only a requirement of pyod
+    #
+    # we force an rc only to permit installation under Py311
+    #
+    # (TODO: remove this line once 0.57 is stable and installed on its own)
+    #
+    'numba >= 0.57.0rc1',
+
     'netaddr ~= 0.8.0',
     'numpy ~= 1.23.3',
     'pandas ~= 1.5.0',
     'pyod ~= 1.0.5',
     'scapy ~= 2.4.5',
     'scikit-learn ~= 1.1.2',
 ]
@@ -43,15 +52,15 @@
 
     # (as yet) unused:
     # 'visualize': ['matplotlib==3.2.1'],
 }
 
 
 setup(name='netml',
-      version='0.5.0',
+      version='0.5.1',
       description='Feature Extraction and Machine Learning from Network Traffic Traces',
       long_description=README_PATH.read_text(),
       long_description_content_type="text/markdown",
       url='https://github.com/noise-lab/netml',
       license='Apache 2.0',
       python_requires='>=3.8.11,<4',
       install_requires=INSTALL_REQUIRES,
```

### Comparing `netml-0.5.0/src/netml/cli.py` & `netml-0.5.1/src/netml/cli.py`

 * *Files identical despite different names*

### Comparing `netml-0.5.0/src/netml/ndm/ae.py` & `netml-0.5.1/src/netml/ndm/ae.py`

 * *Files identical despite different names*

### Comparing `netml-0.5.0/src/netml/ndm/gmm.py` & `netml-0.5.1/src/netml/ndm/gmm.py`

 * *Files identical despite different names*

### Comparing `netml-0.5.0/src/netml/ndm/iforest.py` & `netml-0.5.1/src/netml/ndm/iforest.py`

 * *Files identical despite different names*

### Comparing `netml-0.5.0/src/netml/ndm/kde.py` & `netml-0.5.1/src/netml/ndm/kde.py`

 * *Files identical despite different names*

### Comparing `netml-0.5.0/src/netml/ndm/model.py` & `netml-0.5.1/src/netml/ndm/model.py`

 * *Files identical despite different names*

### Comparing `netml-0.5.0/src/netml/ndm/ocsvm.py` & `netml-0.5.1/src/netml/ndm/ocsvm.py`

 * *Files identical despite different names*

### Comparing `netml-0.5.0/src/netml/ndm/pca.py` & `netml-0.5.1/src/netml/ndm/pca.py`

 * *Files identical despite different names*

### Comparing `netml-0.5.0/src/netml/pparser/parser.py` & `netml-0.5.1/src/netml/pparser/parser.py`

 * *Files identical despite different names*

### Comparing `netml-0.5.0/src/netml/utils/tool.py` & `netml-0.5.1/src/netml/utils/tool.py`

 * *Files identical despite different names*

### Comparing `netml-0.5.0/src/netml.egg-info/PKG-INFO` & `netml-0.5.1/src/netml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netml
-Version: 0.5.0
+Version: 0.5.1
 Summary: Feature Extraction and Machine Learning from Network Traffic Traces
 Home-page: https://github.com/noise-lab/netml
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `netml-0.5.0/src/netml.egg-info/SOURCES.txt` & `netml-0.5.1/src/netml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

