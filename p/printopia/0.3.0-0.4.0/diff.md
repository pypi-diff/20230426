# Comparing `tmp/printopia-0.3.0.tar.gz` & `tmp/printopia-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "printopia-0.3.0.tar", max compression
+gzip compressed data, was "printopia-0.4.0.tar", max compression
```

## Comparing `printopia-0.3.0.tar` & `printopia-0.4.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      496 2023-04-26 19:43:46.274094 printopia-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1555 2023-04-21 18:12:12.063824 printopia-0.3.0/README.md
--rw-r--r--   0        0        0      293 2023-04-26 19:41:01.878029 printopia-0.3.0/src/printopia/__init__.py
--rw-r--r--   0        0        0     3959 2023-04-26 20:01:04.922480 printopia-0.3.0/src/printopia/printopia.py
--rw-r--r--   0        0        0     1935 1970-01-01 00:00:00.000000 printopia-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      492 2023-04-26 20:11:19.061991 printopia-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1555 2023-04-21 18:12:12.063824 printopia-0.4.0/README.md
+-rw-r--r--   0        0        0      293 2023-04-26 19:41:01.878029 printopia-0.4.0/src/printopia/__init__.py
+-rw-r--r--   0        0        0     3959 2023-04-26 20:01:04.922480 printopia-0.4.0/src/printopia/printopia.py
+-rw-r--r--   0        0        0     1931 1970-01-01 00:00:00.000000 printopia-0.4.0/PKG-INFO
```

### Comparing `printopia-0.3.0/README.md` & `printopia-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `printopia-0.3.0/src/printopia/printopia.py` & `printopia-0.4.0/src/printopia/printopia.py`

 * *Files identical despite different names*

### Comparing `printopia-0.3.0/PKG-INFO` & `printopia-0.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: printopia
-Version: 0.3.0
+Version: 0.4.0
 Summary: 
 Author: akshat
 Author-email: akshat1997tamrakar@gmail.com
-Requires-Python: >=3.9,<=3.11.3
+Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Description-Content-Type: text/markdown
```

