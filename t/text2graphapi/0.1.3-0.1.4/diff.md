# Comparing `tmp/text2graphapi-0.1.3.tar.gz` & `tmp/text2graphapi-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text2graphapi-0.1.3.tar", last modified: Tue Apr 25 17:13:58 2023, max compression
+gzip compressed data, was "text2graphapi-0.1.4.tar", last modified: Tue Apr 25 17:23:09 2023, max compression
```

## Comparing `text2graphapi-0.1.3.tar` & `text2graphapi-0.1.4.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 17:13:58.512748 text2graphapi-0.1.3/
--rw-rw-rw-   0        0        0       82 2023-01-17 01:14:45.000000 text2graphapi-0.1.3/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1058 2022-12-02 17:54:23.000000 text2graphapi-0.1.3/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2022-12-02 17:54:23.000000 text2graphapi-0.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0     5410 2023-04-25 17:13:58.511748 text2graphapi-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     4877 2023-04-25 17:11:34.000000 text2graphapi-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-25 17:13:58.278340 text2graphapi-0.1.3/docs/
-drwxrwxrwx   0        0        0        0 2023-04-25 17:13:58.204043 text2graphapi-0.1.3/docs/_build/
-drwxrwxrwx   0        0        0        0 2023-04-25 17:13:58.205044 text2graphapi-0.1.3/docs/_build/html/
-drwxrwxrwx   0        0        0        0 2023-04-25 17:13:58.331012 text2graphapi-0.1.3/docs/_build/html/_sources/
--rw-rw-rw-   0        0        0     1745 2023-03-30 13:11:13.000000 text2graphapi-0.1.3/docs/_build/html/_sources/Cooocurrence.rst.txt
--rw-rw-rw-   0        0        0     1663 2023-03-30 14:12:11.000000 text2graphapi-0.1.3/docs/_build/html/_sources/index.rst.txt
--rw-rw-rw-   0        0        0       46 2022-12-05 21:50:59.000000 text2graphapi-0.1.3/docs/_build/html/_sources/modules.rst.txt
--rw-rw-rw-   0        0        0      408 2022-12-05 21:50:59.000000 text2graphapi-0.1.3/docs/_build/html/_sources/src.rst.txt
--rw-rw-rw-   0        0        0     1783 2022-12-05 21:50:59.000000 text2graphapi-0.1.3/docs/conf.py
--rw-rw-rw-   0        0        0      590 2023-03-30 04:06:40.000000 text2graphapi-0.1.3/notes.txt
--rw-rw-rw-   0        0        0      201 2023-01-17 01:14:45.000000 text2graphapi-0.1.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-25 17:13:58.513749 text2graphapi-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1160 2023-04-25 17:11:34.000000 text2graphapi-0.1.3/setup.py
--rw-rw-rw-   0        0        0      379 2023-03-16 18:14:42.000000 text2graphapi-0.1.3/test_spacy.py
-drwxrwxrwx   0        0        0        0 2023-04-25 17:13:58.332923 text2graphapi-0.1.3/tests/
--rw-rw-rw-   0        0        0        0 2022-10-12 14:46:40.000000 text2graphapi-0.1.3/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 17:13:58.343923 text2graphapi-0.1.3/text2graphapi/
--rw-rw-rw-   0        0        0        0 2023-01-17 01:14:45.000000 text2graphapi-0.1.3/text2graphapi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 17:13:58.218043 text2graphapi-0.1.3/text2graphapi/docs/
-drwxrwxrwx   0        0        0        0 2023-04-25 17:13:58.215050 text2graphapi-0.1.3/text2graphapi/docs/build/
-drwxrwxrwx   0        0        0        0 2023-04-25 17:13:58.216047 text2graphapi-0.1.3/text2graphapi/docs/build/html/
-drwxrwxrwx   0        0        0        0 2023-04-25 17:13:58.437605 text2graphapi-0.1.3/text2graphapi/docs/build/html/_sources/
--rw-rw-rw-   0        0        0     1745 2023-03-30 13:11:13.000000 text2graphapi-0.1.3/text2graphapi/docs/build/html/_sources/Cooocurrence.rst.txt
--rw-rw-rw-   0        0        0     1768 2023-03-30 13:07:45.000000 text2graphapi-0.1.3/text2graphapi/docs/build/html/_sources/Heterogeneous.rst.txt
--rw-rw-rw-   0        0        0     1702 2023-03-30 11:19:22.000000 text2graphapi-0.1.3/text2graphapi/docs/build/html/_sources/index.rst.txt
-drwxrwxrwx   0        0        0        0 2023-04-25 17:13:58.442350 text2graphapi-0.1.3/text2graphapi/docs/source/
--rw-rw-rw-   0        0        0     1352 2023-04-25 17:11:34.000000 text2graphapi-0.1.3/text2graphapi/docs/source/conf.py
--rw-rw-rw-   0        0        0     8000 2023-04-25 17:11:34.000000 text2graphapi-0.1.3/text2graphapi/main.py
-drwxrwxrwx   0        0        0        0 2023-04-25 17:13:58.473764 text2graphapi-0.1.3/text2graphapi/src/
--rw-rw-rw-   0        0        0     7156 2023-04-25 17:11:34.000000 text2graphapi-0.1.3/text2graphapi/src/Cooccurrence.py
--rw-rw-rw-   0        0        0     1088 2023-01-17 01:14:45.000000 text2graphapi-0.1.3/text2graphapi/src/Graph.py
--rw-rw-rw-   0        0        0     1018 2023-01-17 01:14:45.000000 text2graphapi-0.1.3/text2graphapi/src/GraphTransformation.py
--rw-rw-rw-   0        0        0    13653 2023-04-25 17:11:34.000000 text2graphapi-0.1.3/text2graphapi/src/Heterogeneous.py
--rw-rw-rw-   0        0        0     8833 2023-04-25 17:11:34.000000 text2graphapi-0.1.3/text2graphapi/src/Preprocessing.py
--rw-rw-rw-   0        0        0     1873 2023-04-25 17:11:34.000000 text2graphapi-0.1.3/text2graphapi/src/Utils.py
--rw-rw-rw-   0        0        0        0 2023-01-17 01:14:45.000000 text2graphapi-0.1.3/text2graphapi/src/__init__.py
--rw-rw-rw-   0        0        0      482 2023-04-25 17:11:34.000000 text2graphapi-0.1.3/text2graphapi/src/configs.py
-drwxrwxrwx   0        0        0        0 2023-04-25 17:13:58.508747 text2graphapi-0.1.3/text2graphapi/src/resources/
--rw-rw-rw-   0        0        0     4160 2023-01-17 01:14:45.000000 text2graphapi-0.1.3/text2graphapi/src/resources/stopwords_english.txt
--rw-rw-rw-   0        0        0     5256 2023-03-08 18:09:28.000000 text2graphapi-0.1.3/text2graphapi/src/resources/stopwords_french.txt
--rw-rw-rw-   0        0        0     4852 2023-01-17 01:14:45.000000 text2graphapi-0.1.3/text2graphapi/src/resources/stopwords_spanish.txt
--rw-rw-rw-   0        0        0     2248 2023-03-30 02:11:28.000000 text2graphapi-0.1.3/text2graphapi/testing.py
-drwxrwxrwx   0        0        0        0 2023-04-25 17:13:58.399936 text2graphapi-0.1.3/text2graphapi.egg-info/
--rw-rw-rw-   0        0        0     5410 2023-04-25 17:13:57.000000 text2graphapi-0.1.3/text2graphapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1167 2023-04-25 17:13:58.000000 text2graphapi-0.1.3/text2graphapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 17:13:57.000000 text2graphapi-0.1.3/text2graphapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      109 2023-04-25 17:13:57.000000 text2graphapi-0.1.3/text2graphapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-04-25 17:13:57.000000 text2graphapi-0.1.3/text2graphapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-25 17:23:09.471457 text2graphapi-0.1.4/
+-rw-rw-rw-   0        0        0       82 2023-01-17 01:14:45.000000 text2graphapi-0.1.4/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1058 2022-12-02 17:54:23.000000 text2graphapi-0.1.4/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2022-12-02 17:54:23.000000 text2graphapi-0.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     5410 2023-04-25 17:23:09.470422 text2graphapi-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4877 2023-04-25 17:11:34.000000 text2graphapi-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-25 17:23:09.368109 text2graphapi-0.1.4/docs/
+drwxrwxrwx   0        0        0        0 2023-04-25 17:23:09.334046 text2graphapi-0.1.4/docs/_build/
+drwxrwxrwx   0        0        0        0 2023-04-25 17:23:09.335048 text2graphapi-0.1.4/docs/_build/html/
+drwxrwxrwx   0        0        0        0 2023-04-25 17:23:09.379112 text2graphapi-0.1.4/docs/_build/html/_sources/
+-rw-rw-rw-   0        0        0     1745 2023-03-30 13:11:13.000000 text2graphapi-0.1.4/docs/_build/html/_sources/Cooocurrence.rst.txt
+-rw-rw-rw-   0        0        0     1663 2023-03-30 14:12:11.000000 text2graphapi-0.1.4/docs/_build/html/_sources/index.rst.txt
+-rw-rw-rw-   0        0        0       46 2022-12-05 21:50:59.000000 text2graphapi-0.1.4/docs/_build/html/_sources/modules.rst.txt
+-rw-rw-rw-   0        0        0      408 2022-12-05 21:50:59.000000 text2graphapi-0.1.4/docs/_build/html/_sources/src.rst.txt
+-rw-rw-rw-   0        0        0     1783 2022-12-05 21:50:59.000000 text2graphapi-0.1.4/docs/conf.py
+-rw-rw-rw-   0        0        0      590 2023-03-30 04:06:40.000000 text2graphapi-0.1.4/notes.txt
+-rw-rw-rw-   0        0        0      201 2023-01-17 01:14:45.000000 text2graphapi-0.1.4/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-25 17:23:09.471977 text2graphapi-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1160 2023-04-25 17:22:52.000000 text2graphapi-0.1.4/setup.py
+-rw-rw-rw-   0        0        0      379 2023-03-16 18:14:42.000000 text2graphapi-0.1.4/test_spacy.py
+drwxrwxrwx   0        0        0        0 2023-04-25 17:23:09.383108 text2graphapi-0.1.4/tests/
+-rw-rw-rw-   0        0        0        0 2022-10-12 14:46:40.000000 text2graphapi-0.1.4/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 17:23:09.390105 text2graphapi-0.1.4/text2graphapi/
+-rw-rw-rw-   0        0        0        0 2023-01-17 01:14:45.000000 text2graphapi-0.1.4/text2graphapi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 17:23:09.343064 text2graphapi-0.1.4/text2graphapi/docs/
+drwxrwxrwx   0        0        0        0 2023-04-25 17:23:09.340075 text2graphapi-0.1.4/text2graphapi/docs/build/
+drwxrwxrwx   0        0        0        0 2023-04-25 17:23:09.341046 text2graphapi-0.1.4/text2graphapi/docs/build/html/
+drwxrwxrwx   0        0        0        0 2023-04-25 17:23:09.438263 text2graphapi-0.1.4/text2graphapi/docs/build/html/_sources/
+-rw-rw-rw-   0        0        0     1745 2023-03-30 13:11:13.000000 text2graphapi-0.1.4/text2graphapi/docs/build/html/_sources/Cooocurrence.rst.txt
+-rw-rw-rw-   0        0        0     1768 2023-03-30 13:07:45.000000 text2graphapi-0.1.4/text2graphapi/docs/build/html/_sources/Heterogeneous.rst.txt
+-rw-rw-rw-   0        0        0     1702 2023-03-30 11:19:22.000000 text2graphapi-0.1.4/text2graphapi/docs/build/html/_sources/index.rst.txt
+drwxrwxrwx   0        0        0        0 2023-04-25 17:23:09.441259 text2graphapi-0.1.4/text2graphapi/docs/source/
+-rw-rw-rw-   0        0        0     1352 2023-04-25 17:11:34.000000 text2graphapi-0.1.4/text2graphapi/docs/source/conf.py
+-rw-rw-rw-   0        0        0     8000 2023-04-25 17:11:34.000000 text2graphapi-0.1.4/text2graphapi/main.py
+drwxrwxrwx   0        0        0        0 2023-04-25 17:23:09.461438 text2graphapi-0.1.4/text2graphapi/src/
+-rw-rw-rw-   0        0        0     7155 2023-04-25 17:20:48.000000 text2graphapi-0.1.4/text2graphapi/src/Cooccurrence.py
+-rw-rw-rw-   0        0        0     1088 2023-01-17 01:14:45.000000 text2graphapi-0.1.4/text2graphapi/src/Graph.py
+-rw-rw-rw-   0        0        0     1018 2023-01-17 01:14:45.000000 text2graphapi-0.1.4/text2graphapi/src/GraphTransformation.py
+-rw-rw-rw-   0        0        0    13651 2023-04-25 17:20:54.000000 text2graphapi-0.1.4/text2graphapi/src/Heterogeneous.py
+-rw-rw-rw-   0        0        0     8833 2023-04-25 17:11:34.000000 text2graphapi-0.1.4/text2graphapi/src/Preprocessing.py
+-rw-rw-rw-   0        0        0     1873 2023-04-25 17:11:34.000000 text2graphapi-0.1.4/text2graphapi/src/Utils.py
+-rw-rw-rw-   0        0        0        0 2023-01-17 01:14:45.000000 text2graphapi-0.1.4/text2graphapi/src/__init__.py
+-rw-rw-rw-   0        0        0      482 2023-04-25 17:11:34.000000 text2graphapi-0.1.4/text2graphapi/src/configs.py
+drwxrwxrwx   0        0        0        0 2023-04-25 17:23:09.468420 text2graphapi-0.1.4/text2graphapi/src/resources/
+-rw-rw-rw-   0        0        0     4160 2023-01-17 01:14:45.000000 text2graphapi-0.1.4/text2graphapi/src/resources/stopwords_english.txt
+-rw-rw-rw-   0        0        0     5256 2023-03-08 18:09:28.000000 text2graphapi-0.1.4/text2graphapi/src/resources/stopwords_french.txt
+-rw-rw-rw-   0        0        0     4852 2023-01-17 01:14:45.000000 text2graphapi-0.1.4/text2graphapi/src/resources/stopwords_spanish.txt
+-rw-rw-rw-   0        0        0     2248 2023-03-30 02:11:28.000000 text2graphapi-0.1.4/text2graphapi/testing.py
+drwxrwxrwx   0        0        0        0 2023-04-25 17:23:09.429264 text2graphapi-0.1.4/text2graphapi.egg-info/
+-rw-rw-rw-   0        0        0     5410 2023-04-25 17:23:09.000000 text2graphapi-0.1.4/text2graphapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1167 2023-04-25 17:23:09.000000 text2graphapi-0.1.4/text2graphapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 17:23:09.000000 text2graphapi-0.1.4/text2graphapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      109 2023-04-25 17:23:09.000000 text2graphapi-0.1.4/text2graphapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-04-25 17:23:09.000000 text2graphapi-0.1.4/text2graphapi.egg-info/top_level.txt
```

### Comparing `text2graphapi-0.1.3/LICENSE.txt` & `text2graphapi-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `text2graphapi-0.1.3/PKG-INFO` & `text2graphapi-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2graphapi
-Version: 0.1.3
+Version: 0.1.4
 Summary: Use this library to transform raw text into differents graph representations.
 Home-page: UNKNOWN
 Author: PLN-disca-iimas
 Author-email: andric.valdez@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `text2graphapi-0.1.3/README.md` & `text2graphapi-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `text2graphapi-0.1.3/docs/_build/html/_sources/Cooocurrence.rst.txt` & `text2graphapi-0.1.4/docs/_build/html/_sources/Cooocurrence.rst.txt`

 * *Files identical despite different names*

### Comparing `text2graphapi-0.1.3/docs/_build/html/_sources/index.rst.txt` & `text2graphapi-0.1.4/docs/_build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `text2graphapi-0.1.3/docs/conf.py` & `text2graphapi-0.1.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `text2graphapi-0.1.3/notes.txt` & `text2graphapi-0.1.4/notes.txt`

 * *Files identical despite different names*

### Comparing `text2graphapi-0.1.3/setup.py` & `text2graphapi-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ROOT = path.abspath(path.dirname(__file__))
 
 with open(path.join(ROOT, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="text2graphapi",
-    version="0.1.3",
+    version="0.1.4",
     description="Use this library to transform raw text into differents graph representations.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     author="PLN-disca-iimas",
     author_email="andric.valdez@gmail.com",
     license="MIT",
```

### Comparing `text2graphapi-0.1.3/text2graphapi/docs/build/html/_sources/Cooocurrence.rst.txt` & `text2graphapi-0.1.4/text2graphapi/docs/build/html/_sources/Cooocurrence.rst.txt`

 * *Files identical despite different names*

### Comparing `text2graphapi-0.1.3/text2graphapi/docs/build/html/_sources/Heterogeneous.rst.txt` & `text2graphapi-0.1.4/text2graphapi/docs/build/html/_sources/Heterogeneous.rst.txt`

 * *Files identical despite different names*

### Comparing `text2graphapi-0.1.3/text2graphapi/docs/build/html/_sources/index.rst.txt` & `text2graphapi-0.1.4/text2graphapi/docs/build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `text2graphapi-0.1.3/text2graphapi/docs/source/conf.py` & `text2graphapi-0.1.4/text2graphapi/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `text2graphapi-0.1.3/text2graphapi/main.py` & `text2graphapi-0.1.4/text2graphapi/main.py`

 * *Files identical despite different names*

### Comparing `text2graphapi-0.1.3/text2graphapi/src/Cooccurrence.py` & `text2graphapi-0.1.4/text2graphapi/src/Cooccurrence.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import sys
 import traceback
 import time
 from joblib import Parallel, delayed
 import warnings
 
 # Configs
-TEST_API_FROM = 'LOCAL' #posible values: LOCAL, PYPI
+TEST_API_FROM = 'PYPI' #posible values: LOCAL, PYPI
 warnings.filterwarnings("ignore")
 logging.basicConfig(stream=sys.stdout, level=logging.INFO, format="%(asctime)s; - %(levelname)s; - %(message)s")
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.INFO)
 
 logger.debug('Import libraries/modules from :%s', TEST_API_FROM)
 if TEST_API_FROM == 'PYPI':
```

### Comparing `text2graphapi-0.1.3/text2graphapi/src/Graph.py` & `text2graphapi-0.1.4/text2graphapi/src/Graph.py`

 * *Files identical despite different names*

### Comparing `text2graphapi-0.1.3/text2graphapi/src/GraphTransformation.py` & `text2graphapi-0.1.4/text2graphapi/src/GraphTransformation.py`

 * *Files identical despite different names*

### Comparing `text2graphapi-0.1.3/text2graphapi/src/Heterogeneous.py` & `text2graphapi-0.1.4/text2graphapi/src/Heterogeneous.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 import collections
 import itertools
 import os
 import warnings
 
 
 # Logging configs
-TEST_API_FROM = 'LOCAL' #posible values: LOCAL, PYPI
+TEST_API_FROM = 'PYPI' #posible values: LOCAL, PYPI
 warnings.filterwarnings("ignore")
 logging.basicConfig(stream=sys.stdout, level=logging.INFO, format="%(asctime)s; - %(levelname)s; - %(message)s")
 logger = logging.getLogger(__name__)
-logger.setLevel(logging.DEBUG)
+logger.setLevel(logging.INFO)
 
 
 
 logger.debug('Import libraries/modules from :%s', TEST_API_FROM)
 if TEST_API_FROM == 'PYPI':
     from text2graphapi.src.Utils import Utils
     from text2graphapi.src.Preprocessing import Preprocessing
```

### Comparing `text2graphapi-0.1.3/text2graphapi/src/Preprocessing.py` & `text2graphapi-0.1.4/text2graphapi/src/Preprocessing.py`

 * *Files identical despite different names*

### Comparing `text2graphapi-0.1.3/text2graphapi/src/Utils.py` & `text2graphapi-0.1.4/text2graphapi/src/Utils.py`

 * *Files identical despite different names*

### Comparing `text2graphapi-0.1.3/text2graphapi/src/resources/stopwords_english.txt` & `text2graphapi-0.1.4/text2graphapi/src/resources/stopwords_english.txt`

 * *Files identical despite different names*

### Comparing `text2graphapi-0.1.3/text2graphapi/src/resources/stopwords_french.txt` & `text2graphapi-0.1.4/text2graphapi/src/resources/stopwords_french.txt`

 * *Files identical despite different names*

### Comparing `text2graphapi-0.1.3/text2graphapi/src/resources/stopwords_spanish.txt` & `text2graphapi-0.1.4/text2graphapi/src/resources/stopwords_spanish.txt`

 * *Files identical despite different names*

### Comparing `text2graphapi-0.1.3/text2graphapi/testing.py` & `text2graphapi-0.1.4/text2graphapi/testing.py`

 * *Files identical despite different names*

### Comparing `text2graphapi-0.1.3/text2graphapi.egg-info/PKG-INFO` & `text2graphapi-0.1.4/text2graphapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2graphapi
-Version: 0.1.3
+Version: 0.1.4
 Summary: Use this library to transform raw text into differents graph representations.
 Home-page: UNKNOWN
 Author: PLN-disca-iimas
 Author-email: andric.valdez@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `text2graphapi-0.1.3/text2graphapi.egg-info/SOURCES.txt` & `text2graphapi-0.1.4/text2graphapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

