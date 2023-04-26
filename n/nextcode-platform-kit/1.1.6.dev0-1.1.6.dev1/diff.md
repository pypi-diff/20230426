# Comparing `tmp/nextcode-platform-kit-1.1.6.dev0.tar.gz` & `tmp/nextcode-platform-kit-1.1.6.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nextcode-platform-kit-1.1.6.dev0.tar", last modified: Wed Apr 26 15:35:48 2023, max compression
+gzip compressed data, was "nextcode-platform-kit-1.1.6.dev1.tar", last modified: Wed Apr 26 16:56:07 2023, max compression
```

## Comparing `nextcode-platform-kit-1.1.6.dev0.tar` & `nextcode-platform-kit-1.1.6.dev1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 15:35:48.567858 nextcode-platform-kit-1.1.6.dev0/
--rw-rw-rw-   0 root         (0) root         (0)       99 2023-04-26 15:35:17.000000 nextcode-platform-kit-1.1.6.dev0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      928 2023-04-26 15:35:48.567858 nextcode-platform-kit-1.1.6.dev0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3958 2023-04-26 15:35:17.000000 nextcode-platform-kit-1.1.6.dev0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 15:35:48.560858 nextcode-platform-kit-1.1.6.dev0/nextcode_platform_kit.egg-info/
--rw-r--r--   0 root         (0) root         (0)      928 2023-04-26 15:35:48.000000 nextcode-platform-kit-1.1.6.dev0/nextcode_platform_kit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      790 2023-04-26 15:35:48.000000 nextcode-platform-kit-1.1.6.dev0/nextcode_platform_kit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 15:35:48.000000 nextcode-platform-kit-1.1.6.dev0/nextcode_platform_kit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 15:35:47.000000 nextcode-platform-kit-1.1.6.dev0/nextcode_platform_kit.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      197 2023-04-26 15:35:48.000000 nextcode-platform-kit-1.1.6.dev0/nextcode_platform_kit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-26 15:35:48.000000 nextcode-platform-kit-1.1.6.dev0/nextcode_platform_kit.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 15:35:48.564858 nextcode-platform-kit-1.1.6.dev0/platkit/
--rw-rw-rw-   0 root         (0) root         (0)       11 2023-04-26 15:35:48.000000 nextcode-platform-kit-1.1.6.dev0/platkit/VERSION
--rw-rw-rw-   0 root         (0) root         (0)      228 2023-04-26 15:35:17.000000 nextcode-platform-kit-1.1.6.dev0/platkit/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13791 2023-04-26 15:35:17.000000 nextcode-platform-kit-1.1.6.dev0/platkit/auth.py
--rw-rw-rw-   0 root         (0) root         (0)     6141 2023-04-26 15:35:17.000000 nextcode-platform-kit-1.1.6.dev0/platkit/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      682 2023-04-26 15:35:17.000000 nextcode-platform-kit-1.1.6.dev0/platkit/config.py
--rw-rw-rw-   0 root         (0) root         (0)     1798 2023-04-26 15:35:17.000000 nextcode-platform-kit-1.1.6.dev0/platkit/csautils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 15:35:48.565858 nextcode-platform-kit-1.1.6.dev0/platkit/endpoints/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-26 15:35:17.000000 nextcode-platform-kit-1.1.6.dev0/platkit/endpoints/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2038 2023-04-26 15:35:17.000000 nextcode-platform-kit-1.1.6.dev0/platkit/endpoints/auth.py
--rw-rw-rw-   0 root         (0) root         (0)      416 2023-04-26 15:35:17.000000 nextcode-platform-kit-1.1.6.dev0/platkit/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     8561 2023-04-26 15:35:17.000000 nextcode-platform-kit-1.1.6.dev0/platkit/flasksetup.py
--rw-rw-rw-   0 root         (0) root         (0)     1784 2023-04-26 15:35:17.000000 nextcode-platform-kit-1.1.6.dev0/platkit/librarypatches.py
--rw-rw-rw-   0 root         (0) root         (0)     4902 2023-04-26 15:35:17.000000 nextcode-platform-kit-1.1.6.dev0/platkit/logsetup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 15:35:48.566858 nextcode-platform-kit-1.1.6.dev0/platkit/middleware/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-26 15:35:17.000000 nextcode-platform-kit-1.1.6.dev0/platkit/middleware/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3713 2023-04-26 15:35:17.000000 nextcode-platform-kit-1.1.6.dev0/platkit/middleware/logstash_formatter.py
--rw-rw-rw-   0 root         (0) root         (0)     2550 2023-04-26 15:35:17.000000 nextcode-platform-kit-1.1.6.dev0/platkit/middleware/reverse_proxied.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 15:35:48.567858 nextcode-platform-kit-1.1.6.dev0/platkit/models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-26 15:35:17.000000 nextcode-platform-kit-1.1.6.dev0/platkit/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1041 2023-04-26 15:35:17.000000 nextcode-platform-kit-1.1.6.dev0/platkit/models/responses.py
--rw-rw-rw-   0 root         (0) root         (0)      134 2023-04-26 15:35:17.000000 nextcode-platform-kit-1.1.6.dev0/platkit/prometheus.py
--rw-rw-rw-   0 root         (0) root         (0)     5724 2023-04-26 15:35:17.000000 nextcode-platform-kit-1.1.6.dev0/platkit/testcase.py
--rw-rw-rw-   0 root         (0) root         (0)     6175 2023-04-26 15:35:17.000000 nextcode-platform-kit-1.1.6.dev0/platkit/utils.py
--rw-rw-rw-   0 root         (0) root         (0)      272 2023-04-26 15:35:17.000000 nextcode-platform-kit-1.1.6.dev0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-26 15:35:48.568858 nextcode-platform-kit-1.1.6.dev0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1586 2023-04-26 15:35:17.000000 nextcode-platform-kit-1.1.6.dev0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 16:56:07.996359 nextcode-platform-kit-1.1.6.dev1/
+-rw-rw-rw-   0 root         (0) root         (0)       99 2023-04-26 16:55:35.000000 nextcode-platform-kit-1.1.6.dev1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      928 2023-04-26 16:56:07.995443 nextcode-platform-kit-1.1.6.dev1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3958 2023-04-26 16:55:35.000000 nextcode-platform-kit-1.1.6.dev1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 16:56:07.989026 nextcode-platform-kit-1.1.6.dev1/nextcode_platform_kit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      928 2023-04-26 16:56:07.000000 nextcode-platform-kit-1.1.6.dev1/nextcode_platform_kit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      790 2023-04-26 16:56:07.000000 nextcode-platform-kit-1.1.6.dev1/nextcode_platform_kit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 16:56:07.000000 nextcode-platform-kit-1.1.6.dev1/nextcode_platform_kit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 16:56:06.000000 nextcode-platform-kit-1.1.6.dev1/nextcode_platform_kit.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      197 2023-04-26 16:56:07.000000 nextcode-platform-kit-1.1.6.dev1/nextcode_platform_kit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-26 16:56:07.000000 nextcode-platform-kit-1.1.6.dev1/nextcode_platform_kit.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 16:56:07.993609 nextcode-platform-kit-1.1.6.dev1/platkit/
+-rw-rw-rw-   0 root         (0) root         (0)       11 2023-04-26 16:56:07.000000 nextcode-platform-kit-1.1.6.dev1/platkit/VERSION
+-rw-rw-rw-   0 root         (0) root         (0)      228 2023-04-26 16:55:35.000000 nextcode-platform-kit-1.1.6.dev1/platkit/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13791 2023-04-26 16:55:35.000000 nextcode-platform-kit-1.1.6.dev1/platkit/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)     6141 2023-04-26 16:55:35.000000 nextcode-platform-kit-1.1.6.dev1/platkit/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      682 2023-04-26 16:55:35.000000 nextcode-platform-kit-1.1.6.dev1/platkit/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     1798 2023-04-26 16:55:35.000000 nextcode-platform-kit-1.1.6.dev1/platkit/csautils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 16:56:07.993609 nextcode-platform-kit-1.1.6.dev1/platkit/endpoints/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-26 16:55:35.000000 nextcode-platform-kit-1.1.6.dev1/platkit/endpoints/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2038 2023-04-26 16:55:35.000000 nextcode-platform-kit-1.1.6.dev1/platkit/endpoints/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)      416 2023-04-26 16:55:35.000000 nextcode-platform-kit-1.1.6.dev1/platkit/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     8561 2023-04-26 16:55:35.000000 nextcode-platform-kit-1.1.6.dev1/platkit/flasksetup.py
+-rw-rw-rw-   0 root         (0) root         (0)     1784 2023-04-26 16:55:35.000000 nextcode-platform-kit-1.1.6.dev1/platkit/librarypatches.py
+-rw-rw-rw-   0 root         (0) root         (0)     4902 2023-04-26 16:55:35.000000 nextcode-platform-kit-1.1.6.dev1/platkit/logsetup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 16:56:07.994526 nextcode-platform-kit-1.1.6.dev1/platkit/middleware/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-26 16:55:35.000000 nextcode-platform-kit-1.1.6.dev1/platkit/middleware/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3713 2023-04-26 16:55:35.000000 nextcode-platform-kit-1.1.6.dev1/platkit/middleware/logstash_formatter.py
+-rw-rw-rw-   0 root         (0) root         (0)     2550 2023-04-26 16:55:35.000000 nextcode-platform-kit-1.1.6.dev1/platkit/middleware/reverse_proxied.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 16:56:07.995443 nextcode-platform-kit-1.1.6.dev1/platkit/models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-26 16:55:35.000000 nextcode-platform-kit-1.1.6.dev1/platkit/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1041 2023-04-26 16:55:35.000000 nextcode-platform-kit-1.1.6.dev1/platkit/models/responses.py
+-rw-rw-rw-   0 root         (0) root         (0)      134 2023-04-26 16:55:35.000000 nextcode-platform-kit-1.1.6.dev1/platkit/prometheus.py
+-rw-rw-rw-   0 root         (0) root         (0)     5724 2023-04-26 16:55:35.000000 nextcode-platform-kit-1.1.6.dev1/platkit/testcase.py
+-rw-rw-rw-   0 root         (0) root         (0)     6175 2023-04-26 16:55:35.000000 nextcode-platform-kit-1.1.6.dev1/platkit/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      279 2023-04-26 16:55:35.000000 nextcode-platform-kit-1.1.6.dev1/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-26 16:56:07.996359 nextcode-platform-kit-1.1.6.dev1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1586 2023-04-26 16:55:35.000000 nextcode-platform-kit-1.1.6.dev1/setup.py
```

### Comparing `nextcode-platform-kit-1.1.6.dev0/PKG-INFO` & `nextcode-platform-kit-1.1.6.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextcode-platform-kit
-Version: 1.1.6.dev0
+Version: 1.1.6.dev1
 Summary: Flask setup packages
 Home-page: https://www.wuxinextcode.com
 Author: WUXI NextCODE
 Author-email: support@wuxinextcode.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `nextcode-platform-kit-1.1.6.dev0/README.md` & `nextcode-platform-kit-1.1.6.dev1/README.md`

 * *Files identical despite different names*

### Comparing `nextcode-platform-kit-1.1.6.dev0/nextcode_platform_kit.egg-info/PKG-INFO` & `nextcode-platform-kit-1.1.6.dev1/nextcode_platform_kit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextcode-platform-kit
-Version: 1.1.6.dev0
+Version: 1.1.6.dev1
 Summary: Flask setup packages
 Home-page: https://www.wuxinextcode.com
 Author: WUXI NextCODE
 Author-email: support@wuxinextcode.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `nextcode-platform-kit-1.1.6.dev0/nextcode_platform_kit.egg-info/SOURCES.txt` & `nextcode-platform-kit-1.1.6.dev1/nextcode_platform_kit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nextcode-platform-kit-1.1.6.dev0/platkit/auth.py` & `nextcode-platform-kit-1.1.6.dev1/platkit/auth.py`

 * *Files identical despite different names*

### Comparing `nextcode-platform-kit-1.1.6.dev0/platkit/cli.py` & `nextcode-platform-kit-1.1.6.dev1/platkit/cli.py`

 * *Files identical despite different names*

### Comparing `nextcode-platform-kit-1.1.6.dev0/platkit/config.py` & `nextcode-platform-kit-1.1.6.dev1/platkit/config.py`

 * *Files identical despite different names*

### Comparing `nextcode-platform-kit-1.1.6.dev0/platkit/csautils.py` & `nextcode-platform-kit-1.1.6.dev1/platkit/csautils.py`

 * *Files identical despite different names*

### Comparing `nextcode-platform-kit-1.1.6.dev0/platkit/endpoints/auth.py` & `nextcode-platform-kit-1.1.6.dev1/platkit/endpoints/auth.py`

 * *Files identical despite different names*

### Comparing `nextcode-platform-kit-1.1.6.dev0/platkit/flasksetup.py` & `nextcode-platform-kit-1.1.6.dev1/platkit/flasksetup.py`

 * *Files identical despite different names*

### Comparing `nextcode-platform-kit-1.1.6.dev0/platkit/librarypatches.py` & `nextcode-platform-kit-1.1.6.dev1/platkit/librarypatches.py`

 * *Files identical despite different names*

### Comparing `nextcode-platform-kit-1.1.6.dev0/platkit/logsetup.py` & `nextcode-platform-kit-1.1.6.dev1/platkit/logsetup.py`

 * *Files identical despite different names*

### Comparing `nextcode-platform-kit-1.1.6.dev0/platkit/middleware/logstash_formatter.py` & `nextcode-platform-kit-1.1.6.dev1/platkit/middleware/logstash_formatter.py`

 * *Files identical despite different names*

### Comparing `nextcode-platform-kit-1.1.6.dev0/platkit/middleware/reverse_proxied.py` & `nextcode-platform-kit-1.1.6.dev1/platkit/middleware/reverse_proxied.py`

 * *Files identical despite different names*

### Comparing `nextcode-platform-kit-1.1.6.dev0/platkit/models/responses.py` & `nextcode-platform-kit-1.1.6.dev1/platkit/models/responses.py`

 * *Files identical despite different names*

### Comparing `nextcode-platform-kit-1.1.6.dev0/platkit/testcase.py` & `nextcode-platform-kit-1.1.6.dev1/platkit/testcase.py`

 * *Files identical despite different names*

### Comparing `nextcode-platform-kit-1.1.6.dev0/platkit/utils.py` & `nextcode-platform-kit-1.1.6.dev1/platkit/utils.py`

 * *Files identical despite different names*

### Comparing `nextcode-platform-kit-1.1.6.dev0/setup.py` & `nextcode-platform-kit-1.1.6.dev1/setup.py`

 * *Files identical despite different names*

