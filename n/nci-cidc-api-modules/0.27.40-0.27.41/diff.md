# Comparing `tmp/nci_cidc_api_modules-0.27.40.tar.gz` & `tmp/nci_cidc_api_modules-0.27.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/cidc-api-gae/cidc-api-gae/dist/.tmp-5nzqhw5a/nci_cidc_api_modules-0.27.40.tar", last modified: Tue Apr 25 17:17:57 2023, max compression
+gzip compressed data, was "/home/runner/work/cidc-api-gae/cidc-api-gae/dist/.tmp-wjnqwke_/nci_cidc_api_modules-0.27.41.tar", last modified: Tue Apr 25 18:53:08 2023, max compression
```

## Comparing `nci_cidc_api_modules-0.27.40.tar` & `nci_cidc_api_modules-0.27.41.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:17:57.000000 nci_cidc_api_modules-0.27.40/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-25 17:17:46.000000 nci_cidc_api_modules-0.27.40/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-25 17:17:46.000000 nci_cidc_api_modules-0.27.40/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    37413 2023-04-25 17:17:57.000000 nci_cidc_api_modules-0.27.40/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    37107 2023-04-25 17:17:46.000000 nci_cidc_api_modules-0.27.40/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:17:57.000000 nci_cidc_api_modules-0.27.40/cidc_api/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:17:57.000000 nci_cidc_api_modules-0.27.40/cidc_api/config/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-25 17:17:46.000000 nci_cidc_api_modules-0.27.40/cidc_api/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-04-25 17:17:46.000000 nci_cidc_api_modules-0.27.40/cidc_api/config/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-25 17:17:46.000000 nci_cidc_api_modules-0.27.40/cidc_api/config/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-04-25 17:17:46.000000 nci_cidc_api_modules-0.27.40/cidc_api/config/secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4548 2023-04-25 17:17:46.000000 nci_cidc_api_modules-0.27.40/cidc_api/config/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:17:57.000000 nci_cidc_api_modules-0.27.40/cidc_api/csms/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-25 17:17:46.000000 nci_cidc_api_modules-0.27.40/cidc_api/csms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-04-25 17:17:46.000000 nci_cidc_api_modules-0.27.40/cidc_api/csms/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:17:57.000000 nci_cidc_api_modules-0.27.40/cidc_api/models/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-25 17:17:46.000000 nci_cidc_api_modules-0.27.40/cidc_api/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31379 2023-04-25 17:17:46.000000 nci_cidc_api_modules-0.27.40/cidc_api/models/csms_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:17:57.000000 nci_cidc_api_modules-0.27.40/cidc_api/models/files/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-25 17:17:46.000000 nci_cidc_api_modules-0.27.40/cidc_api/models/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    62285 2023-04-25 17:17:46.000000 nci_cidc_api_modules-0.27.40/cidc_api/models/files/details.py
--rw-r--r--   0 runner    (1001) docker     (123)    28653 2023-04-25 17:17:46.000000 nci_cidc_api_modules-0.27.40/cidc_api/models/files/facets.py
--rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-04-25 17:17:46.000000 nci_cidc_api_modules-0.27.40/cidc_api/models/migrations.py
--rw-r--r--   0 runner    (1001) docker     (123)   100053 2023-04-25 17:17:46.000000 nci_cidc_api_modules-0.27.40/cidc_api/models/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-04-25 17:17:46.000000 nci_cidc_api_modules-0.27.40/cidc_api/models/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:17:57.000000 nci_cidc_api_modules-0.27.40/cidc_api/shared/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 17:17:46.000000 nci_cidc_api_modules-0.27.40/cidc_api/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11474 2023-04-25 17:17:46.000000 nci_cidc_api_modules-0.27.40/cidc_api/shared/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-04-25 17:17:46.000000 nci_cidc_api_modules-0.27.40/cidc_api/shared/emails.py
--rw-r--r--   0 runner    (1001) docker     (123)    32453 2023-04-25 17:17:46.000000 nci_cidc_api_modules-0.27.40/cidc_api/shared/gcloud_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-04-25 17:17:46.000000 nci_cidc_api_modules-0.27.40/cidc_api/shared/rest_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:17:57.000000 nci_cidc_api_modules-0.27.40/nci_cidc_api_modules.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    37413 2023-04-25 17:17:57.000000 nci_cidc_api_modules-0.27.40/nci_cidc_api_modules.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-25 17:17:57.000000 nci_cidc_api_modules-0.27.40/nci_cidc_api_modules.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 17:17:57.000000 nci_cidc_api_modules-0.27.40/nci_cidc_api_modules.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 17:17:57.000000 nci_cidc_api_modules-0.27.40/nci_cidc_api_modules.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-25 17:17:57.000000 nci_cidc_api_modules-0.27.40/nci_cidc_api_modules.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-25 17:17:57.000000 nci_cidc_api_modules-0.27.40/nci_cidc_api_modules.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-25 17:17:46.000000 nci_cidc_api_modules-0.27.40/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-25 17:17:46.000000 nci_cidc_api_modules-0.27.40/requirements.modules.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 17:17:57.000000 nci_cidc_api_modules-0.27.40/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-25 17:17:46.000000 nci_cidc_api_modules-0.27.40/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:17:57.000000 nci_cidc_api_modules-0.27.40/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    17108 2023-04-25 17:17:46.000000 nci_cidc_api_modules-0.27.40/tests/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:53:08.000000 nci_cidc_api_modules-0.27.41/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-25 18:53:00.000000 nci_cidc_api_modules-0.27.41/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-25 18:53:00.000000 nci_cidc_api_modules-0.27.41/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    37413 2023-04-25 18:53:08.000000 nci_cidc_api_modules-0.27.41/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    37107 2023-04-25 18:53:00.000000 nci_cidc_api_modules-0.27.41/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:53:08.000000 nci_cidc_api_modules-0.27.41/cidc_api/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:53:08.000000 nci_cidc_api_modules-0.27.41/cidc_api/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-25 18:53:00.000000 nci_cidc_api_modules-0.27.41/cidc_api/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-04-25 18:53:00.000000 nci_cidc_api_modules-0.27.41/cidc_api/config/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-25 18:53:00.000000 nci_cidc_api_modules-0.27.41/cidc_api/config/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-04-25 18:53:00.000000 nci_cidc_api_modules-0.27.41/cidc_api/config/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4548 2023-04-25 18:53:00.000000 nci_cidc_api_modules-0.27.41/cidc_api/config/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:53:08.000000 nci_cidc_api_modules-0.27.41/cidc_api/csms/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-25 18:53:00.000000 nci_cidc_api_modules-0.27.41/cidc_api/csms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-04-25 18:53:00.000000 nci_cidc_api_modules-0.27.41/cidc_api/csms/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:53:08.000000 nci_cidc_api_modules-0.27.41/cidc_api/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-25 18:53:00.000000 nci_cidc_api_modules-0.27.41/cidc_api/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31379 2023-04-25 18:53:00.000000 nci_cidc_api_modules-0.27.41/cidc_api/models/csms_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:53:08.000000 nci_cidc_api_modules-0.27.41/cidc_api/models/files/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-25 18:53:00.000000 nci_cidc_api_modules-0.27.41/cidc_api/models/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62285 2023-04-25 18:53:00.000000 nci_cidc_api_modules-0.27.41/cidc_api/models/files/details.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28653 2023-04-25 18:53:00.000000 nci_cidc_api_modules-0.27.41/cidc_api/models/files/facets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-04-25 18:53:00.000000 nci_cidc_api_modules-0.27.41/cidc_api/models/migrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100053 2023-04-25 18:53:00.000000 nci_cidc_api_modules-0.27.41/cidc_api/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-04-25 18:53:00.000000 nci_cidc_api_modules-0.27.41/cidc_api/models/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:53:08.000000 nci_cidc_api_modules-0.27.41/cidc_api/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 18:53:00.000000 nci_cidc_api_modules-0.27.41/cidc_api/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11474 2023-04-25 18:53:00.000000 nci_cidc_api_modules-0.27.41/cidc_api/shared/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-04-25 18:53:00.000000 nci_cidc_api_modules-0.27.41/cidc_api/shared/emails.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32453 2023-04-25 18:53:00.000000 nci_cidc_api_modules-0.27.41/cidc_api/shared/gcloud_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-04-25 18:53:00.000000 nci_cidc_api_modules-0.27.41/cidc_api/shared/rest_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:53:08.000000 nci_cidc_api_modules-0.27.41/nci_cidc_api_modules.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    37413 2023-04-25 18:53:08.000000 nci_cidc_api_modules-0.27.41/nci_cidc_api_modules.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-25 18:53:08.000000 nci_cidc_api_modules-0.27.41/nci_cidc_api_modules.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 18:53:08.000000 nci_cidc_api_modules-0.27.41/nci_cidc_api_modules.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 18:53:08.000000 nci_cidc_api_modules-0.27.41/nci_cidc_api_modules.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-25 18:53:08.000000 nci_cidc_api_modules-0.27.41/nci_cidc_api_modules.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-25 18:53:08.000000 nci_cidc_api_modules-0.27.41/nci_cidc_api_modules.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-25 18:53:00.000000 nci_cidc_api_modules-0.27.41/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-25 18:53:00.000000 nci_cidc_api_modules-0.27.41/requirements.modules.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 18:53:08.000000 nci_cidc_api_modules-0.27.41/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-25 18:53:00.000000 nci_cidc_api_modules-0.27.41/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:53:08.000000 nci_cidc_api_modules-0.27.41/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    17108 2023-04-25 18:53:00.000000 nci_cidc_api_modules-0.27.41/tests/test_api.py
```

### Comparing `nci_cidc_api_modules-0.27.40/LICENSE` & `nci_cidc_api_modules-0.27.41/LICENSE`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.40/PKG-INFO` & `nci_cidc_api_modules-0.27.41/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nci_cidc_api_modules
-Version: 0.27.40
+Version: 0.27.41
 Summary: SQLAlchemy data models and configuration tools used in the NCI CIDC API
 Home-page: https://github.com/NCI-CIDC/cidc-api-gae
 License: MIT license
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `nci_cidc_api_modules-0.27.40/README.md` & `nci_cidc_api_modules-0.27.41/README.md`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.40/cidc_api/config/db.py` & `nci_cidc_api_modules-0.27.41/cidc_api/config/db.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.40/cidc_api/config/logging.py` & `nci_cidc_api_modules-0.27.41/cidc_api/config/logging.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.40/cidc_api/config/secrets.py` & `nci_cidc_api_modules-0.27.41/cidc_api/config/secrets.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.40/cidc_api/config/settings.py` & `nci_cidc_api_modules-0.27.41/cidc_api/config/settings.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.40/cidc_api/csms/auth.py` & `nci_cidc_api_modules-0.27.41/cidc_api/csms/auth.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.40/cidc_api/models/csms_api.py` & `nci_cidc_api_modules-0.27.41/cidc_api/models/csms_api.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.40/cidc_api/models/files/details.py` & `nci_cidc_api_modules-0.27.41/cidc_api/models/files/details.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.40/cidc_api/models/files/facets.py` & `nci_cidc_api_modules-0.27.41/cidc_api/models/files/facets.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.40/cidc_api/models/migrations.py` & `nci_cidc_api_modules-0.27.41/cidc_api/models/migrations.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.40/cidc_api/models/models.py` & `nci_cidc_api_modules-0.27.41/cidc_api/models/models.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.40/cidc_api/models/schemas.py` & `nci_cidc_api_modules-0.27.41/cidc_api/models/schemas.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.40/cidc_api/shared/auth.py` & `nci_cidc_api_modules-0.27.41/cidc_api/shared/auth.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.40/cidc_api/shared/emails.py` & `nci_cidc_api_modules-0.27.41/cidc_api/shared/emails.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.40/cidc_api/shared/gcloud_client.py` & `nci_cidc_api_modules-0.27.41/cidc_api/shared/gcloud_client.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.40/cidc_api/shared/rest_utils.py` & `nci_cidc_api_modules-0.27.41/cidc_api/shared/rest_utils.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.40/nci_cidc_api_modules.egg-info/PKG-INFO` & `nci_cidc_api_modules-0.27.41/nci_cidc_api_modules.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nci-cidc-api-modules
-Version: 0.27.40
+Version: 0.27.41
 Summary: SQLAlchemy data models and configuration tools used in the NCI CIDC API
 Home-page: https://github.com/NCI-CIDC/cidc-api-gae
 License: MIT license
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `nci_cidc_api_modules-0.27.40/nci_cidc_api_modules.egg-info/SOURCES.txt` & `nci_cidc_api_modules-0.27.41/nci_cidc_api_modules.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.40/setup.py` & `nci_cidc_api_modules-0.27.41/setup.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.40/tests/test_api.py` & `nci_cidc_api_modules-0.27.41/tests/test_api.py`

 * *Files identical despite different names*

