# Comparing `tmp/awesome-object-store-2.2.0.tar.gz` & `tmp/awesome-object-store-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awesome-object-store-2.2.0.tar", max compression
+gzip compressed data, was "awesome-object-store-2.2.1.tar", max compression
```

## Comparing `awesome-object-store-2.2.0.tar` & `awesome-object-store-2.2.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11358 2022-12-01 02:13:59.211942 awesome-object-store-2.2.0/LICENSE.txt
--rw-r--r--   0        0        0     1342 2022-12-01 02:13:59.211942 awesome-object-store-2.2.0/README.md
--rw-r--r--   0        0        0      757 2022-12-01 02:13:59.211942 awesome-object-store-2.2.0/awesome_object_store/__init__.py
--rw-r--r--   0        0        0     3816 2022-12-01 02:13:59.211942 awesome-object-store-2.2.0/awesome_object_store/base.py
--rw-r--r--   0        0        0     5328 2022-12-01 02:13:59.211942 awesome-object-store-2.2.0/awesome_object_store/gcs.py
--rw-r--r--   0        0        0     5349 2022-12-01 02:13:59.211942 awesome-object-store-2.2.0/awesome_object_store/minio.py
--rw-r--r--   0        0        0     2135 2022-12-01 02:13:59.211942 awesome-object-store-2.2.0/pyproject.toml
--rw-r--r--   0        0        0     2180 2022-12-01 02:14:09.417810 awesome-object-store-2.2.0/setup.py
--rw-r--r--   0        0        0     2665 2022-12-01 02:14:09.418111 awesome-object-store-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-04-26 06:36:55.625542 awesome-object-store-2.2.1/LICENSE.txt
+-rw-r--r--   0        0        0     1342 2023-04-26 06:36:55.625542 awesome-object-store-2.2.1/README.md
+-rw-r--r--   0        0        0      757 2023-04-26 06:36:55.625542 awesome-object-store-2.2.1/awesome_object_store/__init__.py
+-rw-r--r--   0        0        0     3816 2023-04-26 06:36:55.625542 awesome-object-store-2.2.1/awesome_object_store/base.py
+-rw-r--r--   0        0        0     5328 2023-04-26 06:36:55.625542 awesome-object-store-2.2.1/awesome_object_store/gcs.py
+-rw-r--r--   0        0        0     5349 2023-04-26 06:36:55.625542 awesome-object-store-2.2.1/awesome_object_store/minio.py
+-rw-r--r--   0        0        0     2135 2023-04-26 06:36:55.625542 awesome-object-store-2.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2174 2023-04-26 06:37:05.893156 awesome-object-store-2.2.1/setup.py
+-rw-r--r--   0        0        0     2659 2023-04-26 06:37:05.893519 awesome-object-store-2.2.1/PKG-INFO
```

### Comparing `awesome-object-store-2.2.0/LICENSE.txt` & `awesome-object-store-2.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `awesome-object-store-2.2.0/README.md` & `awesome-object-store-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `awesome-object-store-2.2.0/awesome_object_store/__init__.py` & `awesome-object-store-2.2.1/awesome_object_store/__init__.py`

 * *Files identical despite different names*

### Comparing `awesome-object-store-2.2.0/awesome_object_store/base.py` & `awesome-object-store-2.2.1/awesome_object_store/base.py`

 * *Files identical despite different names*

### Comparing `awesome-object-store-2.2.0/awesome_object_store/gcs.py` & `awesome-object-store-2.2.1/awesome_object_store/gcs.py`

 * *Files identical despite different names*

### Comparing `awesome-object-store-2.2.0/awesome_object_store/minio.py` & `awesome-object-store-2.2.1/awesome_object_store/minio.py`

 * *Files identical despite different names*

### Comparing `awesome-object-store-2.2.0/pyproject.toml` & `awesome-object-store-2.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "awesome-object-store"
-version = "2.2.0"
+version = "2.2.1"
 license = "Apache-2.0"
 readme = "README.md"
 description = "minio wrapper to perform task like pandas dataframe upload, download"
 authors = ["Schwannden Kuo <schwannden@mobagel.com>"]
 homepage = "https://github.com/MoBagel/awesome-object-store"
 classifiers = [
   "Development Status :: 1 - Planning",
@@ -28,15 +28,15 @@
 ]
 
 [tool.poetry.dependencies]
 python = "~=3.8"
 minio = "^7.1.1"
 pandas = "^1.4.1"
 starlette = ">=0.16.0"
-google-cloud-storage = "^2.3.0"
+google-cloud-storage = "1.44.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2"
 pytest-cov = "^3.0.0"
 black = "~=22.6.0"
 flake8 = "^4.0.0"
 isort = "^5.10.1"
```

### Comparing `awesome-object-store-2.2.0/setup.py` & `awesome-object-store-2.2.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 packages = \
 ['awesome_object_store']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['google-cloud-storage>=2.3.0,<3.0.0',
+['google-cloud-storage==1.44.0',
  'minio>=7.1.1,<8.0.0',
  'pandas>=1.4.1,<2.0.0',
  'starlette>=0.16.0']
 
 setup_kwargs = {
     'name': 'awesome-object-store',
-    'version': '2.2.0',
+    'version': '2.2.1',
     'description': 'minio wrapper to perform task like pandas dataframe upload, download',
     'long_description': '[![Stable Version](https://badge.fury.io/py/awesome-object-store.svg)](https://pypi.org/project/awesome-object-store/)\n[![tests](https://github.com/MoBagel/awesome-object-store/workflows/develop/badge.svg)](https://github.com/MoBagel/awesome-object-store)\n[![Coverage Status](https://coveralls.io/repos/github/MoBagel/awesome-object-store/badge.svg?branch=develop)](https://coveralls.io/github/MoBagel/awesome-object-store?branch=develop)\n\n# Awesome Object Store \n\nA library that extends minio python client to perform more complex task like read/write pandas DataFrame, json file, ...etc\n\n# Feature\n* list_buckets: list all buckets.\n* list_objects: list object under a prefix.\n* put_as_json: put a dict as json file on s3.\n* exists: check if an object exist on s3.\n* remove_dir: remove a directory on s3.\n* upload_df: Upload df as csv to s3.\n* get_json: Get as dict from a json file on s3.\n* get_df: Get a dataframe from a csv object on s3.\n* remove_objects: Remove objects.\n* download: Downloads data of an object to file.\n\n# Development\n## run unit test\n1. getting service account credential:\n   1. visit google cloud console\n   1. go to project 8ndpoint-datalake-dev -> Security -> Secret Manager -> awesome-object-store-unit-test\n   1. action -> view secret value\n   1. store the value in tests/service-account.json\n2. run ./run_test.sh\n',
     'author': 'Schwannden Kuo',
     'author_email': 'schwannden@mobagel.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/MoBagel/awesome-object-store',
```

### Comparing `awesome-object-store-2.2.0/PKG-INFO` & `awesome-object-store-2.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awesome-object-store
-Version: 2.2.0
+Version: 2.2.1
 Summary: minio wrapper to perform task like pandas dataframe upload, download
 Home-page: https://github.com/MoBagel/awesome-object-store
 License: Apache-2.0
 Author: Schwannden Kuo
 Author-email: schwannden@mobagel.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 1 - Planning
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Internet
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: google-cloud-storage (>=2.3.0,<3.0.0)
+Requires-Dist: google-cloud-storage (==1.44.0)
 Requires-Dist: minio (>=7.1.1,<8.0.0)
 Requires-Dist: pandas (>=1.4.1,<2.0.0)
 Requires-Dist: starlette (>=0.16.0)
 Description-Content-Type: text/markdown
 
 [![Stable Version](https://badge.fury.io/py/awesome-object-store.svg)](https://pypi.org/project/awesome-object-store/)
 [![tests](https://github.com/MoBagel/awesome-object-store/workflows/develop/badge.svg)](https://github.com/MoBagel/awesome-object-store)
```

