# Comparing `tmp/hullencrypt-0.0.3.tar.gz` & `tmp/hullencrypt-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hullencrypt-0.0.3.tar", last modified: Tue Apr 25 17:32:54 2023, max compression
+gzip compressed data, was "hullencrypt-0.0.4.tar", last modified: Tue Apr 25 17:42:09 2023, max compression
```

## Comparing `hullencrypt-0.0.3.tar` & `hullencrypt-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-04-25 17:32:54.765854 hullencrypt-0.0.3/
--rw-r--r--   0 john      (1000) john      (1000)    35149 2023-04-25 16:33:25.000000 hullencrypt-0.0.3/LICENSE
--rw-r--r--   0 john      (1000) john      (1000)     2052 2023-04-25 17:32:54.765854 hullencrypt-0.0.3/PKG-INFO
--rw-r--r--   0 john      (1000) john      (1000)     1623 2023-04-25 16:18:17.000000 hullencrypt-0.0.3/README.md
--rw-r--r--   0 john      (1000) john      (1000)     5988 2023-04-25 17:32:29.000000 hullencrypt-0.0.3/base.py
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-04-25 17:32:54.765854 hullencrypt-0.0.3/hullencrypt.egg-info/
--rw-r--r--   0 john      (1000) john      (1000)     2052 2023-04-25 17:32:54.000000 hullencrypt-0.0.3/hullencrypt.egg-info/PKG-INFO
--rw-r--r--   0 john      (1000) john      (1000)      214 2023-04-25 17:32:54.000000 hullencrypt-0.0.3/hullencrypt.egg-info/SOURCES.txt
--rw-r--r--   0 john      (1000) john      (1000)        1 2023-04-25 17:32:54.000000 hullencrypt-0.0.3/hullencrypt.egg-info/dependency_links.txt
--rw-r--r--   0 john      (1000) john      (1000)       21 2023-04-25 17:32:54.000000 hullencrypt-0.0.3/hullencrypt.egg-info/requires.txt
--rw-r--r--   0 john      (1000) john      (1000)        5 2023-04-25 17:32:54.000000 hullencrypt-0.0.3/hullencrypt.egg-info/top_level.txt
--rw-r--r--   0 john      (1000) john      (1000)      485 2023-04-25 17:32:48.000000 hullencrypt-0.0.3/pyproject.toml
--rw-r--r--   0 john      (1000) john      (1000)       38 2023-04-25 17:32:54.765854 hullencrypt-0.0.3/setup.cfg
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-04-25 17:42:09.815528 hullencrypt-0.0.4/
+-rw-r--r--   0 john      (1000) john      (1000)    35149 2023-04-25 16:33:25.000000 hullencrypt-0.0.4/LICENSE
+-rw-r--r--   0 john      (1000) john      (1000)     2052 2023-04-25 17:42:09.815528 hullencrypt-0.0.4/PKG-INFO
+-rw-r--r--   0 john      (1000) john      (1000)     1623 2023-04-25 16:18:17.000000 hullencrypt-0.0.4/README.md
+-rw-r--r--   0 john      (1000) john      (1000)      485 2023-04-25 17:41:33.000000 hullencrypt-0.0.4/pyproject.toml
+-rw-r--r--   0 john      (1000) john      (1000)       38 2023-04-25 17:42:09.815528 hullencrypt-0.0.4/setup.cfg
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-04-25 17:42:09.815528 hullencrypt-0.0.4/src/
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-04-25 17:42:09.815528 hullencrypt-0.0.4/src/hullencrypt/
+-rw-r--r--   0 john      (1000) john      (1000)     5988 2023-04-25 17:32:29.000000 hullencrypt-0.0.4/src/hullencrypt/base.py
+-rw-r--r--   0 john      (1000) john      (1000)     1130 2023-04-25 17:35:11.000000 hullencrypt-0.0.4/src/hullencrypt/test.py
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-04-25 17:42:09.815528 hullencrypt-0.0.4/src/hullencrypt.egg-info/
+-rw-r--r--   0 john      (1000) john      (1000)     2052 2023-04-25 17:42:09.000000 hullencrypt-0.0.4/src/hullencrypt.egg-info/PKG-INFO
+-rw-r--r--   0 john      (1000) john      (1000)      274 2023-04-25 17:42:09.000000 hullencrypt-0.0.4/src/hullencrypt.egg-info/SOURCES.txt
+-rw-r--r--   0 john      (1000) john      (1000)        1 2023-04-25 17:42:09.000000 hullencrypt-0.0.4/src/hullencrypt.egg-info/dependency_links.txt
+-rw-r--r--   0 john      (1000) john      (1000)       21 2023-04-25 17:42:09.000000 hullencrypt-0.0.4/src/hullencrypt.egg-info/requires.txt
+-rw-r--r--   0 john      (1000) john      (1000)       12 2023-04-25 17:42:09.000000 hullencrypt-0.0.4/src/hullencrypt.egg-info/top_level.txt
```

### Comparing `hullencrypt-0.0.3/LICENSE` & `hullencrypt-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hullencrypt-0.0.3/PKG-INFO` & `hullencrypt-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hullencrypt
-Version: 0.0.3
+Version: 0.0.4
 Summary: A selfmade cryptolib for sharing passwords in a tree structure
 Author-email: John Janzen <rc-dev@johnjanzen.me>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `hullencrypt-0.0.3/README.md` & `hullencrypt-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `hullencrypt-0.0.3/base.py` & `hullencrypt-0.0.4/src/hullencrypt/base.py`

 * *Files identical despite different names*

### Comparing `hullencrypt-0.0.3/hullencrypt.egg-info/PKG-INFO` & `hullencrypt-0.0.4/src/hullencrypt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hullencrypt
-Version: 0.0.3
+Version: 0.0.4
 Summary: A selfmade cryptolib for sharing passwords in a tree structure
 Author-email: John Janzen <rc-dev@johnjanzen.me>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

