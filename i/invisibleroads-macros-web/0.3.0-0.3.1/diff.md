# Comparing `tmp/invisibleroads-macros-web-0.3.0.tar.gz` & `tmp/invisibleroads-macros-web-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invisibleroads-macros-web-0.3.0.tar", last modified: Fri Mar 31 19:09:48 2023, max compression
+gzip compressed data, was "invisibleroads-macros-web-0.3.1.tar", last modified: Wed Apr 26 17:24:02 2023, max compression
```

## Comparing `invisibleroads-macros-web-0.3.0.tar` & `invisibleroads-macros-web-0.3.1.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-03-31 19:09:48.144946 invisibleroads-macros-web-0.3.0/
--rw-r--r--   0 rhh       (1000) rhh       (1000)      288 2022-12-14 19:46:41.000000 invisibleroads-macros-web-0.3.0/CHANGES.md
--rw-r--r--   0 rhh       (1000) rhh       (1000)       13 2022-10-28 18:39:04.000000 invisibleroads-macros-web-0.3.0/MANIFEST.in
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1875 2023-03-31 19:09:48.143946 invisibleroads-macros-web-0.3.0/PKG-INFO
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1086 2023-02-06 17:49:03.000000 invisibleroads-macros-web-0.3.0/README.md
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-03-31 19:09:48.142946 invisibleroads-macros-web-0.3.0/invisibleroads_macros_web/
--rw-r--r--   0 rhh       (1000) rhh       (1000)        0 2022-10-28 18:39:04.000000 invisibleroads-macros-web-0.3.0/invisibleroads_macros_web/__init__.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)      846 2022-10-28 18:39:04.000000 invisibleroads-macros-web-0.3.0/invisibleroads_macros_web/browser.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)      290 2022-10-28 18:39:04.000000 invisibleroads-macros-web-0.3.0/invisibleroads_macros_web/escape.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1263 2023-02-06 20:19:53.000000 invisibleroads-macros-web-0.3.0/invisibleroads_macros_web/jinja.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)      670 2023-03-31 19:09:05.000000 invisibleroads-macros-web-0.3.0/invisibleroads_macros_web/markdown.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)      882 2022-10-28 18:39:04.000000 invisibleroads-macros-web-0.3.0/invisibleroads_macros_web/port.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1117 2023-03-31 18:25:46.000000 invisibleroads-macros-web-0.3.0/invisibleroads_macros_web/starlette.py
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-03-31 19:09:48.143946 invisibleroads-macros-web-0.3.0/invisibleroads_macros_web.egg-info/
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1875 2023-03-31 19:09:48.000000 invisibleroads-macros-web-0.3.0/invisibleroads_macros_web.egg-info/PKG-INFO
--rw-r--r--   0 rhh       (1000) rhh       (1000)      649 2023-03-31 19:09:48.000000 invisibleroads-macros-web-0.3.0/invisibleroads_macros_web.egg-info/SOURCES.txt
--rw-r--r--   0 rhh       (1000) rhh       (1000)        1 2023-03-31 19:09:48.000000 invisibleroads-macros-web-0.3.0/invisibleroads_macros_web.egg-info/dependency_links.txt
--rw-r--r--   0 rhh       (1000) rhh       (1000)      163 2023-03-31 19:09:48.000000 invisibleroads-macros-web-0.3.0/invisibleroads_macros_web.egg-info/requires.txt
--rw-r--r--   0 rhh       (1000) rhh       (1000)       26 2023-03-31 19:09:48.000000 invisibleroads-macros-web-0.3.0/invisibleroads_macros_web.egg-info/top_level.txt
--rw-r--r--   0 rhh       (1000) rhh       (1000)        1 2022-10-28 18:53:12.000000 invisibleroads-macros-web-0.3.0/invisibleroads_macros_web.egg-info/zip-safe
--rw-r--r--   0 rhh       (1000) rhh       (1000)       38 2023-03-31 19:09:48.144946 invisibleroads-macros-web-0.3.0/setup.cfg
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1374 2023-03-31 18:59:19.000000 invisibleroads-macros-web-0.3.0/setup.py
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-03-31 19:09:48.143946 invisibleroads-macros-web-0.3.0/tests/
--rw-r--r--   0 rhh       (1000) rhh       (1000)      344 2022-10-28 18:39:04.000000 invisibleroads-macros-web-0.3.0/tests/test_escape.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)      549 2022-12-16 16:28:59.000000 invisibleroads-macros-web-0.3.0/tests/test_markdown.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)      609 2022-10-28 18:39:04.000000 invisibleroads-macros-web-0.3.0/tests/test_port.py
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-04-26 17:24:02.819001 invisibleroads-macros-web-0.3.1/
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      288 2023-02-04 11:54:56.000000 invisibleroads-macros-web-0.3.1/CHANGES.md
+-rw-r--r--   0 rhh       (1000) rhh       (1000)       13 2023-02-04 11:54:56.000000 invisibleroads-macros-web-0.3.1/MANIFEST.in
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1875 2023-04-26 17:24:02.818001 invisibleroads-macros-web-0.3.1/PKG-INFO
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1086 2023-02-04 11:58:00.000000 invisibleroads-macros-web-0.3.1/README.md
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-04-26 17:24:02.814000 invisibleroads-macros-web-0.3.1/invisibleroads_macros_web/
+-rw-r--r--   0 rhh       (1000) rhh       (1000)        0 2023-02-04 11:54:56.000000 invisibleroads-macros-web-0.3.1/invisibleroads_macros_web/__init__.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      846 2023-02-04 11:54:56.000000 invisibleroads-macros-web-0.3.1/invisibleroads_macros_web/browser.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      290 2023-02-04 11:54:56.000000 invisibleroads-macros-web-0.3.1/invisibleroads_macros_web/escape.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1263 2023-02-08 13:47:12.000000 invisibleroads-macros-web-0.3.1/invisibleroads_macros_web/jinja.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      652 2023-04-25 11:27:49.000000 invisibleroads-macros-web-0.3.1/invisibleroads_macros_web/markdown.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      882 2023-02-04 11:54:56.000000 invisibleroads-macros-web-0.3.1/invisibleroads_macros_web/port.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1117 2023-04-05 01:08:22.000000 invisibleroads-macros-web-0.3.1/invisibleroads_macros_web/starlette.py
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-04-26 17:24:02.816001 invisibleroads-macros-web-0.3.1/invisibleroads_macros_web.egg-info/
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1875 2023-04-26 17:24:02.000000 invisibleroads-macros-web-0.3.1/invisibleroads_macros_web.egg-info/PKG-INFO
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      667 2023-04-26 17:24:02.000000 invisibleroads-macros-web-0.3.1/invisibleroads_macros_web.egg-info/SOURCES.txt
+-rw-r--r--   0 rhh       (1000) rhh       (1000)        1 2023-04-26 17:24:02.000000 invisibleroads-macros-web-0.3.1/invisibleroads_macros_web.egg-info/dependency_links.txt
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      163 2023-04-26 17:24:02.000000 invisibleroads-macros-web-0.3.1/invisibleroads_macros_web.egg-info/requires.txt
+-rw-r--r--   0 rhh       (1000) rhh       (1000)       32 2023-04-26 17:24:02.000000 invisibleroads-macros-web-0.3.1/invisibleroads_macros_web.egg-info/top_level.txt
+-rw-r--r--   0 rhh       (1000) rhh       (1000)        1 2023-02-04 12:09:21.000000 invisibleroads-macros-web-0.3.1/invisibleroads_macros_web.egg-info/zip-safe
+-rw-r--r--   0 rhh       (1000) rhh       (1000)       38 2023-04-26 17:24:02.819001 invisibleroads-macros-web-0.3.1/setup.cfg
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1374 2023-04-26 17:18:20.000000 invisibleroads-macros-web-0.3.1/setup.py
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-04-26 17:24:02.817000 invisibleroads-macros-web-0.3.1/tests/
+-rw-r--r--   0 rhh       (1000) rhh       (1000)        0 2023-04-26 17:22:15.000000 invisibleroads-macros-web-0.3.1/tests/__init__.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      344 2023-02-04 11:54:56.000000 invisibleroads-macros-web-0.3.1/tests/test_escape.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      549 2023-02-04 11:54:56.000000 invisibleroads-macros-web-0.3.1/tests/test_markdown.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      882 2023-04-26 17:17:57.000000 invisibleroads-macros-web-0.3.1/tests/test_port.py
```

### Comparing `invisibleroads-macros-web-0.3.0/PKG-INFO` & `invisibleroads-macros-web-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invisibleroads-macros-web
-Version: 0.3.0
+Version: 0.3.1
 Summary: Shortcut functions for web operations
 Home-page: https://github.com/invisibleroads/invisibleroads-macros-web
 Author: Roy Hyunjin Han
 Author-email: rhh@crosscompute.com
 Keywords: invisibleroads
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `invisibleroads-macros-web-0.3.0/README.md` & `invisibleroads-macros-web-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `invisibleroads-macros-web-0.3.0/invisibleroads_macros_web/browser.py` & `invisibleroads-macros-web-0.3.1/invisibleroads_macros_web/browser.py`

 * *Files identical despite different names*

### Comparing `invisibleroads-macros-web-0.3.0/invisibleroads_macros_web/jinja.py` & `invisibleroads-macros-web-0.3.1/invisibleroads_macros_web/jinja.py`

 * *Files identical despite different names*

### Comparing `invisibleroads-macros-web-0.3.0/invisibleroads_macros_web/markdown.py` & `invisibleroads-macros-web-0.3.1/invisibleroads_macros_web/markdown.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 NESTED_TAG_PATTERN = re.compile(r'<p>(<.*>)</p>')
 EXTRAS = [
     'break-on-newline',
     'code-friendly',
     'cuddled-lists',
     'fenced-code-blocks',
     'footnotes',
-    'header-ids',
     'markdown-in-html',
     'strike',
     'target-blank-links',
     'tables',
     'use-file-vars',
     'task_list']
```

### Comparing `invisibleroads-macros-web-0.3.0/invisibleroads_macros_web/port.py` & `invisibleroads-macros-web-0.3.1/invisibleroads_macros_web/port.py`

 * *Files identical despite different names*

### Comparing `invisibleroads-macros-web-0.3.0/invisibleroads_macros_web/starlette.py` & `invisibleroads-macros-web-0.3.1/invisibleroads_macros_web/starlette.py`

 * *Files identical despite different names*

### Comparing `invisibleroads-macros-web-0.3.0/invisibleroads_macros_web.egg-info/PKG-INFO` & `invisibleroads-macros-web-0.3.1/invisibleroads_macros_web.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invisibleroads-macros-web
-Version: 0.3.0
+Version: 0.3.1
 Summary: Shortcut functions for web operations
 Home-page: https://github.com/invisibleroads/invisibleroads-macros-web
 Author: Roy Hyunjin Han
 Author-email: rhh@crosscompute.com
 Keywords: invisibleroads
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `invisibleroads-macros-web-0.3.0/invisibleroads_macros_web.egg-info/SOURCES.txt` & `invisibleroads-macros-web-0.3.1/invisibleroads_macros_web.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -11,10 +11,11 @@
 invisibleroads_macros_web/starlette.py
 invisibleroads_macros_web.egg-info/PKG-INFO
 invisibleroads_macros_web.egg-info/SOURCES.txt
 invisibleroads_macros_web.egg-info/dependency_links.txt
 invisibleroads_macros_web.egg-info/requires.txt
 invisibleroads_macros_web.egg-info/top_level.txt
 invisibleroads_macros_web.egg-info/zip-safe
+tests/__init__.py
 tests/test_escape.py
 tests/test_markdown.py
 tests/test_port.py
```

### Comparing `invisibleroads-macros-web-0.3.0/setup.py` & `invisibleroads-macros-web-0.3.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 FOLDER = dirname(abspath(__file__))
 DESCRIPTION = '\n\n'.join(open(join(FOLDER, _)).read().strip() for _ in [
     'README.md', 'CHANGES.md'])
 
 
 setup(
     name='invisibleroads-macros-web',
-    version='0.3.0',
+    version='0.3.1',
     description='Shortcut functions for web operations',
     long_description=DESCRIPTION,
     long_description_content_type='text/markdown',
     classifiers=[
         'Programming Language :: Python',
         'License :: OSI Approved :: MIT License',
     ],
```

### Comparing `invisibleroads-macros-web-0.3.0/tests/test_markdown.py` & `invisibleroads-macros-web-0.3.1/tests/test_markdown.py`

 * *Files identical despite different names*

