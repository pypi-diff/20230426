# Comparing `tmp/resotoshell-3.3.3.tar.gz` & `tmp/resotoshell-3.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resotoshell-3.3.3.tar", last modified: Fri Apr 21 14:37:13 2023, max compression
+gzip compressed data, was "resotoshell-3.3.4.tar", last modified: Wed Apr 26 16:52:51 2023, max compression
```

## Comparing `resotoshell-3.3.3.tar` & `resotoshell-3.3.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:37:13.993404 resotoshell-3.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-21 14:34:38.000000 resotoshell-3.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-04-21 14:37:13.993404 resotoshell-3.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-04-21 14:34:38.000000 resotoshell-3.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-21 14:34:38.000000 resotoshell-3.3.3/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:37:13.989404 resotoshell-3.3.3/resotoshell/
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-21 14:34:38.000000 resotoshell-3.3.3/resotoshell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7396 2023-04-21 14:34:38.000000 resotoshell-3.3.3/resotoshell/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35797 2023-04-21 14:34:38.000000 resotoshell-3.3.3/resotoshell/promptsession.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-21 14:34:38.000000 resotoshell-3.3.3/resotoshell/protected_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-04-21 14:34:38.000000 resotoshell-3.3.3/resotoshell/shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:37:13.989404 resotoshell-3.3.3/resotoshell.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-04-21 14:37:13.000000 resotoshell-3.3.3/resotoshell.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-21 14:37:13.000000 resotoshell-3.3.3/resotoshell.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 14:37:13.000000 resotoshell-3.3.3/resotoshell.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-21 14:37:13.000000 resotoshell-3.3.3/resotoshell.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 14:37:13.000000 resotoshell-3.3.3/resotoshell.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-21 14:37:13.000000 resotoshell-3.3.3/resotoshell.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-21 14:37:13.000000 resotoshell-3.3.3/resotoshell.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-21 14:37:13.993404 resotoshell-3.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-04-21 14:34:38.000000 resotoshell-3.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:37:13.993404 resotoshell-3.3.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)    11262 2023-04-21 14:34:38.000000 resotoshell-3.3.3/test/test_promptsession.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-21 14:34:38.000000 resotoshell-3.3.3/test/test_protected_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:52:51.969545 resotoshell-3.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-26 16:49:37.000000 resotoshell-3.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-04-26 16:52:51.969545 resotoshell-3.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-04-26 16:49:37.000000 resotoshell-3.3.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-26 16:49:37.000000 resotoshell-3.3.4/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:52:51.969545 resotoshell-3.3.4/resotoshell/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-26 16:49:37.000000 resotoshell-3.3.4/resotoshell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7396 2023-04-26 16:49:37.000000 resotoshell-3.3.4/resotoshell/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35797 2023-04-26 16:49:37.000000 resotoshell-3.3.4/resotoshell/promptsession.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-26 16:49:37.000000 resotoshell-3.3.4/resotoshell/protected_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-04-26 16:49:37.000000 resotoshell-3.3.4/resotoshell/shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:52:51.969545 resotoshell-3.3.4/resotoshell.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-04-26 16:52:51.000000 resotoshell-3.3.4/resotoshell.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-26 16:52:51.000000 resotoshell-3.3.4/resotoshell.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 16:52:51.000000 resotoshell-3.3.4/resotoshell.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-26 16:52:51.000000 resotoshell-3.3.4/resotoshell.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 16:52:51.000000 resotoshell-3.3.4/resotoshell.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-26 16:52:51.000000 resotoshell-3.3.4/resotoshell.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-26 16:52:51.000000 resotoshell-3.3.4/resotoshell.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-26 16:52:51.969545 resotoshell-3.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-04-26 16:49:37.000000 resotoshell-3.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:52:51.969545 resotoshell-3.3.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    11262 2023-04-26 16:49:37.000000 resotoshell-3.3.4/test/test_promptsession.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-26 16:49:37.000000 resotoshell-3.3.4/test/test_protected_files.py
```

### Comparing `resotoshell-3.3.3/PKG-INFO` & `resotoshell-3.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotoshell
-Version: 3.3.3
+Version: 3.3.4
 Summary: Commandline interpreter to interact with Resoto.
 Home-page: https://github.com/someengineering/resoto/tree/main/resotoshell
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resotoshell-3.3.3/README.md` & `resotoshell-3.3.4/README.md`

 * *Files identical despite different names*

### Comparing `resotoshell-3.3.3/resotoshell/__main__.py` & `resotoshell-3.3.4/resotoshell/__main__.py`

 * *Files identical despite different names*

### Comparing `resotoshell-3.3.3/resotoshell/promptsession.py` & `resotoshell-3.3.4/resotoshell/promptsession.py`

 * *Files identical despite different names*

### Comparing `resotoshell-3.3.3/resotoshell/protected_files.py` & `resotoshell-3.3.4/resotoshell/protected_files.py`

 * *Files identical despite different names*

### Comparing `resotoshell-3.3.3/resotoshell/shell.py` & `resotoshell-3.3.4/resotoshell/shell.py`

 * *Files identical despite different names*

### Comparing `resotoshell-3.3.3/resotoshell.egg-info/PKG-INFO` & `resotoshell-3.3.4/resotoshell.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotoshell
-Version: 3.3.3
+Version: 3.3.4
 Summary: Commandline interpreter to interact with Resoto.
 Home-page: https://github.com/someengineering/resoto/tree/main/resotoshell
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resotoshell-3.3.3/setup.py` & `resotoshell-3.3.4/setup.py`

 * *Files identical despite different names*

### Comparing `resotoshell-3.3.3/test/test_promptsession.py` & `resotoshell-3.3.4/test/test_promptsession.py`

 * *Files identical despite different names*

### Comparing `resotoshell-3.3.3/test/test_protected_files.py` & `resotoshell-3.3.4/test/test_protected_files.py`

 * *Files identical despite different names*

