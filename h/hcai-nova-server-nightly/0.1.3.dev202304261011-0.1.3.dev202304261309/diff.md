# Comparing `tmp/hcai-nova-server-nightly-0.1.3.dev202304261011.tar.gz` & `tmp/hcai-nova-server-nightly-0.1.3.dev202304261309.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcai-nova-server-nightly-0.1.3.dev202304261011.tar", last modified: Wed Apr 26 10:11:17 2023, max compression
+gzip compressed data, was "hcai-nova-server-nightly-0.1.3.dev202304261309.tar", last modified: Wed Apr 26 13:09:15 2023, max compression
```

## Comparing `hcai-nova-server-nightly-0.1.3.dev202304261011.tar` & `hcai-nova-server-nightly-0.1.3.dev202304261309.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 10:11:17.334726 hcai-nova-server-nightly-0.1.3.dev202304261011/
--rw-r--r--   0 runner    (1001) docker     (122)      117 2023-04-26 10:11:02.000000 hcai-nova-server-nightly-0.1.3.dev202304261011/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1568 2023-04-26 10:11:17.334726 hcai-nova-server-nightly-0.1.3.dev202304261011/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      573 2023-04-26 10:11:02.000000 hcai-nova-server-nightly-0.1.3.dev202304261011/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 10:11:17.330726 hcai-nova-server-nightly-0.1.3.dev202304261011/hcai_nova_server_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1568 2023-04-26 10:11:17.000000 hcai-nova-server-nightly-0.1.3.dev202304261011/hcai_nova_server_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      944 2023-04-26 10:11:17.000000 hcai-nova-server-nightly-0.1.3.dev202304261011/hcai_nova_server_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-26 10:11:17.000000 hcai-nova-server-nightly-0.1.3.dev202304261011/hcai_nova_server_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       75 2023-04-26 10:11:17.000000 hcai-nova-server-nightly-0.1.3.dev202304261011/hcai_nova_server_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-04-26 10:11:17.000000 hcai-nova-server-nightly-0.1.3.dev202304261011/hcai_nova_server_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 10:11:17.330726 hcai-nova-server-nightly-0.1.3.dev202304261011/nova_server/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-26 10:11:02.000000 hcai-nova-server-nightly-0.1.3.dev202304261011/nova_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2568 2023-04-26 10:11:02.000000 hcai-nova-server-nightly-0.1.3.dev202304261011/nova_server/nova_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 10:11:17.330726 hcai-nova-server-nightly-0.1.3.dev202304261011/nova_server/route/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-26 10:11:02.000000 hcai-nova-server-nightly-0.1.3.dev202304261011/nova_server/route/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-04-26 10:11:02.000000 hcai-nova-server-nightly-0.1.3.dev202304261011/nova_server/route/cancel.py
--rw-r--r--   0 runner    (1001) docker     (122)    13062 2023-04-26 10:11:02.000000 hcai-nova-server-nightly-0.1.3.dev202304261011/nova_server/route/explain.py
--rw-r--r--   0 runner    (1001) docker     (122)     9430 2023-04-26 10:11:02.000000 hcai-nova-server-nightly-0.1.3.dev202304261011/nova_server/route/extract.py
--rw-r--r--   0 runner    (1001) docker     (122)      809 2023-04-26 10:11:02.000000 hcai-nova-server-nightly-0.1.3.dev202304261011/nova_server/route/log.py
--rw-r--r--   0 runner    (1001) docker     (122)     7836 2023-04-26 10:11:02.000000 hcai-nova-server-nightly-0.1.3.dev202304261011/nova_server/route/predict.py
--rw-r--r--   0 runner    (1001) docker     (122)      756 2023-04-26 10:11:02.000000 hcai-nova-server-nightly-0.1.3.dev202304261011/nova_server/route/status.py
--rw-r--r--   0 runner    (1001) docker     (122)     6075 2023-04-26 10:11:02.000000 hcai-nova-server-nightly-0.1.3.dev202304261011/nova_server/route/train.py
--rw-r--r--   0 runner    (1001) docker     (122)      351 2023-04-26 10:11:02.000000 hcai-nova-server-nightly-0.1.3.dev202304261011/nova_server/route/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 10:11:17.330726 hcai-nova-server-nightly-0.1.3.dev202304261011/nova_server/templates/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-26 10:11:02.000000 hcai-nova-server-nightly-0.1.3.dev202304261011/nova_server/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 10:11:17.334726 hcai-nova-server-nightly-0.1.3.dev202304261011/nova_server/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-26 10:11:02.000000 hcai-nova-server-nightly-0.1.3.dev202304261011/nova_server/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2254 2023-04-26 10:11:02.000000 hcai-nova-server-nightly-0.1.3.dev202304261011/nova_server/utils/dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    11559 2023-04-26 10:11:02.000000 hcai-nova-server-nightly-0.1.3.dev202304261011/nova_server/utils/db_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1785 2023-04-26 10:11:02.000000 hcai-nova-server-nightly-0.1.3.dev202304261011/nova_server/utils/explain_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      447 2023-04-26 10:11:02.000000 hcai-nova-server-nightly-0.1.3.dev202304261011/nova_server/utils/img_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1233 2023-04-26 10:11:02.000000 hcai-nova-server-nightly-0.1.3.dev202304261011/nova_server/utils/import_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      983 2023-04-26 10:11:02.000000 hcai-nova-server-nightly-0.1.3.dev202304261011/nova_server/utils/key_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1375 2023-04-26 10:11:02.000000 hcai-nova-server-nightly-0.1.3.dev202304261011/nova_server/utils/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     2159 2023-04-26 10:11:02.000000 hcai-nova-server-nightly-0.1.3.dev202304261011/nova_server/utils/status_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1984 2023-04-26 10:11:02.000000 hcai-nova-server-nightly-0.1.3.dev202304261011/nova_server/utils/thread_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      103 2023-04-26 10:11:02.000000 hcai-nova-server-nightly-0.1.3.dev202304261011/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-26 10:11:17.334726 hcai-nova-server-nightly-0.1.3.dev202304261011/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2383 2023-04-26 10:11:02.000000 hcai-nova-server-nightly-0.1.3.dev202304261011/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 13:09:15.826677 hcai-nova-server-nightly-0.1.3.dev202304261309/
+-rw-r--r--   0 runner    (1001) docker     (122)      117 2023-04-26 13:09:05.000000 hcai-nova-server-nightly-0.1.3.dev202304261309/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1568 2023-04-26 13:09:15.826677 hcai-nova-server-nightly-0.1.3.dev202304261309/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      573 2023-04-26 13:09:05.000000 hcai-nova-server-nightly-0.1.3.dev202304261309/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 13:09:15.818677 hcai-nova-server-nightly-0.1.3.dev202304261309/hcai_nova_server_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1568 2023-04-26 13:09:15.000000 hcai-nova-server-nightly-0.1.3.dev202304261309/hcai_nova_server_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      944 2023-04-26 13:09:15.000000 hcai-nova-server-nightly-0.1.3.dev202304261309/hcai_nova_server_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-26 13:09:15.000000 hcai-nova-server-nightly-0.1.3.dev202304261309/hcai_nova_server_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       75 2023-04-26 13:09:15.000000 hcai-nova-server-nightly-0.1.3.dev202304261309/hcai_nova_server_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-04-26 13:09:15.000000 hcai-nova-server-nightly-0.1.3.dev202304261309/hcai_nova_server_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 13:09:15.822677 hcai-nova-server-nightly-0.1.3.dev202304261309/nova_server/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-26 13:09:05.000000 hcai-nova-server-nightly-0.1.3.dev202304261309/nova_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2568 2023-04-26 13:09:05.000000 hcai-nova-server-nightly-0.1.3.dev202304261309/nova_server/nova_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 13:09:15.822677 hcai-nova-server-nightly-0.1.3.dev202304261309/nova_server/route/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-26 13:09:05.000000 hcai-nova-server-nightly-0.1.3.dev202304261309/nova_server/route/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-04-26 13:09:05.000000 hcai-nova-server-nightly-0.1.3.dev202304261309/nova_server/route/cancel.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13062 2023-04-26 13:09:05.000000 hcai-nova-server-nightly-0.1.3.dev202304261309/nova_server/route/explain.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9430 2023-04-26 13:09:05.000000 hcai-nova-server-nightly-0.1.3.dev202304261309/nova_server/route/extract.py
+-rw-r--r--   0 runner    (1001) docker     (122)      809 2023-04-26 13:09:05.000000 hcai-nova-server-nightly-0.1.3.dev202304261309/nova_server/route/log.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7836 2023-04-26 13:09:05.000000 hcai-nova-server-nightly-0.1.3.dev202304261309/nova_server/route/predict.py
+-rw-r--r--   0 runner    (1001) docker     (122)      756 2023-04-26 13:09:05.000000 hcai-nova-server-nightly-0.1.3.dev202304261309/nova_server/route/status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6075 2023-04-26 13:09:05.000000 hcai-nova-server-nightly-0.1.3.dev202304261309/nova_server/route/train.py
+-rw-r--r--   0 runner    (1001) docker     (122)      351 2023-04-26 13:09:05.000000 hcai-nova-server-nightly-0.1.3.dev202304261309/nova_server/route/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 13:09:15.822677 hcai-nova-server-nightly-0.1.3.dev202304261309/nova_server/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-26 13:09:05.000000 hcai-nova-server-nightly-0.1.3.dev202304261309/nova_server/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 13:09:15.826677 hcai-nova-server-nightly-0.1.3.dev202304261309/nova_server/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-26 13:09:05.000000 hcai-nova-server-nightly-0.1.3.dev202304261309/nova_server/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2254 2023-04-26 13:09:05.000000 hcai-nova-server-nightly-0.1.3.dev202304261309/nova_server/utils/dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11559 2023-04-26 13:09:05.000000 hcai-nova-server-nightly-0.1.3.dev202304261309/nova_server/utils/db_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1785 2023-04-26 13:09:05.000000 hcai-nova-server-nightly-0.1.3.dev202304261309/nova_server/utils/explain_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      447 2023-04-26 13:09:05.000000 hcai-nova-server-nightly-0.1.3.dev202304261309/nova_server/utils/img_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1233 2023-04-26 13:09:05.000000 hcai-nova-server-nightly-0.1.3.dev202304261309/nova_server/utils/import_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      983 2023-04-26 13:09:05.000000 hcai-nova-server-nightly-0.1.3.dev202304261309/nova_server/utils/key_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1375 2023-04-26 13:09:05.000000 hcai-nova-server-nightly-0.1.3.dev202304261309/nova_server/utils/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2159 2023-04-26 13:09:05.000000 hcai-nova-server-nightly-0.1.3.dev202304261309/nova_server/utils/status_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1984 2023-04-26 13:09:05.000000 hcai-nova-server-nightly-0.1.3.dev202304261309/nova_server/utils/thread_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-04-26 13:09:05.000000 hcai-nova-server-nightly-0.1.3.dev202304261309/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-26 13:09:15.826677 hcai-nova-server-nightly-0.1.3.dev202304261309/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2383 2023-04-26 13:09:05.000000 hcai-nova-server-nightly-0.1.3.dev202304261309/setup.py
```

### Comparing `hcai-nova-server-nightly-0.1.3.dev202304261011/PKG-INFO` & `hcai-nova-server-nightly-0.1.3.dev202304261309/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcai-nova-server-nightly
-Version: 0.1.3.dev202304261011
+Version: 0.1.3.dev202304261309
 Summary: !Alpha Version! - This repository contains code to setup a computational backend server for the nova annotation tool. You can use this backend to train models of your choosing or create explanations for existing models.
 Home-page: https://github.com/pypa/sampleproject
 Author: Dominik Schiller
 Author-email: dominik.schiller@uni-a.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `hcai-nova-server-nightly-0.1.3.dev202304261011/README.md` & `hcai-nova-server-nightly-0.1.3.dev202304261309/README.md`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.3.dev202304261011/hcai_nova_server_nightly.egg-info/PKG-INFO` & `hcai-nova-server-nightly-0.1.3.dev202304261309/hcai_nova_server_nightly.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcai-nova-server-nightly
-Version: 0.1.3.dev202304261011
+Version: 0.1.3.dev202304261309
 Summary: !Alpha Version! - This repository contains code to setup a computational backend server for the nova annotation tool. You can use this backend to train models of your choosing or create explanations for existing models.
 Home-page: https://github.com/pypa/sampleproject
 Author: Dominik Schiller
 Author-email: dominik.schiller@uni-a.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `hcai-nova-server-nightly-0.1.3.dev202304261011/hcai_nova_server_nightly.egg-info/SOURCES.txt` & `hcai-nova-server-nightly-0.1.3.dev202304261309/hcai_nova_server_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.3.dev202304261011/nova_server/nova_backend.py` & `hcai-nova-server-nightly-0.1.3.dev202304261309/nova_server/nova_backend.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.3.dev202304261011/nova_server/route/cancel.py` & `hcai-nova-server-nightly-0.1.3.dev202304261309/nova_server/route/cancel.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.3.dev202304261011/nova_server/route/explain.py` & `hcai-nova-server-nightly-0.1.3.dev202304261309/nova_server/route/explain.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.3.dev202304261011/nova_server/route/extract.py` & `hcai-nova-server-nightly-0.1.3.dev202304261309/nova_server/route/extract.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.3.dev202304261011/nova_server/route/log.py` & `hcai-nova-server-nightly-0.1.3.dev202304261309/nova_server/route/log.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.3.dev202304261011/nova_server/route/predict.py` & `hcai-nova-server-nightly-0.1.3.dev202304261309/nova_server/route/predict.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.3.dev202304261011/nova_server/route/status.py` & `hcai-nova-server-nightly-0.1.3.dev202304261309/nova_server/route/status.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.3.dev202304261011/nova_server/route/train.py` & `hcai-nova-server-nightly-0.1.3.dev202304261309/nova_server/route/train.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.3.dev202304261011/nova_server/utils/dataset_utils.py` & `hcai-nova-server-nightly-0.1.3.dev202304261309/nova_server/utils/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.3.dev202304261011/nova_server/utils/db_utils.py` & `hcai-nova-server-nightly-0.1.3.dev202304261309/nova_server/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.3.dev202304261011/nova_server/utils/explain_utils.py` & `hcai-nova-server-nightly-0.1.3.dev202304261309/nova_server/utils/explain_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.3.dev202304261011/nova_server/utils/import_utils.py` & `hcai-nova-server-nightly-0.1.3.dev202304261309/nova_server/utils/import_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.3.dev202304261011/nova_server/utils/key_utils.py` & `hcai-nova-server-nightly-0.1.3.dev202304261309/nova_server/utils/key_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.3.dev202304261011/nova_server/utils/log_utils.py` & `hcai-nova-server-nightly-0.1.3.dev202304261309/nova_server/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.3.dev202304261011/nova_server/utils/status_utils.py` & `hcai-nova-server-nightly-0.1.3.dev202304261309/nova_server/utils/status_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.3.dev202304261011/nova_server/utils/thread_utils.py` & `hcai-nova-server-nightly-0.1.3.dev202304261309/nova_server/utils/thread_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.3.dev202304261011/setup.py` & `hcai-nova-server-nightly-0.1.3.dev202304261309/setup.py`

 * *Files identical despite different names*

