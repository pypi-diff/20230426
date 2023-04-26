# Comparing `tmp/clannotation-0.0.4.tar.gz` & `tmp/clannotation-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clannotation-0.0.4.tar", last modified: Tue Apr 25 14:30:12 2023, max compression
+gzip compressed data, was "clannotation-0.0.5.tar", last modified: Tue Apr 25 14:38:50 2023, max compression
```

## Comparing `clannotation-0.0.4.tar` & `clannotation-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-25 14:30:12.914093 clannotation-0.0.4/
--rw-rw-r--   0 martin    (1000) martin    (1000)     1054 2023-01-26 10:26:21.000000 clannotation-0.0.4/LICENSE.md
--rw-rw-r--   0 martin    (1000) martin    (1000)     2846 2023-04-25 14:30:12.914093 clannotation-0.0.4/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)      986 2023-04-20 09:30:48.000000 clannotation-0.0.4/README.md
--rw-rw-r--   0 martin    (1000) martin    (1000)      958 2023-04-25 14:27:20.000000 clannotation-0.0.4/pyproject.toml
--rw-rw-r--   0 martin    (1000) martin    (1000)      926 2023-04-25 14:30:12.914093 clannotation-0.0.4/setup.cfg
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-25 14:30:12.914093 clannotation-0.0.4/src/
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-25 14:30:12.914093 clannotation-0.0.4/src/clannotation/
--rw-rw-r--   0 martin    (1000) martin    (1000)        0 2023-04-20 07:44:29.000000 clannotation-0.0.4/src/clannotation/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    10784 2023-04-20 11:37:28.000000 clannotation-0.0.4/src/clannotation/annotator.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-25 14:30:12.914093 clannotation-0.0.4/src/clannotation.egg-info/
--rw-rw-r--   0 martin    (1000) martin    (1000)     2846 2023-04-25 14:30:12.000000 clannotation-0.0.4/src/clannotation.egg-info/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)      334 2023-04-25 14:30:12.000000 clannotation-0.0.4/src/clannotation.egg-info/SOURCES.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-04-25 14:30:12.000000 clannotation-0.0.4/src/clannotation.egg-info/dependency_links.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       72 2023-04-25 14:30:12.000000 clannotation-0.0.4/src/clannotation.egg-info/requires.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       13 2023-04-25 14:30:12.000000 clannotation-0.0.4/src/clannotation.egg-info/top_level.txt
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-25 14:30:12.914093 clannotation-0.0.4/tests/
--rw-rw-r--   0 martin    (1000) martin    (1000)    18311 2023-04-20 08:47:46.000000 clannotation-0.0.4/tests/test_annotator_plugin.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-25 14:38:50.868650 clannotation-0.0.5/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1054 2023-01-26 10:26:21.000000 clannotation-0.0.5/LICENSE.md
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2846 2023-04-25 14:38:50.868650 clannotation-0.0.5/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)      986 2023-04-20 09:30:48.000000 clannotation-0.0.5/README.md
+-rw-rw-r--   0 martin    (1000) martin    (1000)      958 2023-04-25 14:38:35.000000 clannotation-0.0.5/pyproject.toml
+-rw-rw-r--   0 martin    (1000) martin    (1000)      926 2023-04-25 14:38:50.868650 clannotation-0.0.5/setup.cfg
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-25 14:38:50.868650 clannotation-0.0.5/src/
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-25 14:38:50.868650 clannotation-0.0.5/src/clannotation/
+-rw-rw-r--   0 martin    (1000) martin    (1000)        0 2023-04-20 07:44:29.000000 clannotation-0.0.5/src/clannotation/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    10784 2023-04-20 11:37:28.000000 clannotation-0.0.5/src/clannotation/annotator.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-25 14:38:50.868650 clannotation-0.0.5/src/clannotation.egg-info/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2846 2023-04-25 14:38:50.000000 clannotation-0.0.5/src/clannotation.egg-info/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)      334 2023-04-25 14:38:50.000000 clannotation-0.0.5/src/clannotation.egg-info/SOURCES.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-04-25 14:38:50.000000 clannotation-0.0.5/src/clannotation.egg-info/dependency_links.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       72 2023-04-25 14:38:50.000000 clannotation-0.0.5/src/clannotation.egg-info/requires.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       13 2023-04-25 14:38:50.000000 clannotation-0.0.5/src/clannotation.egg-info/top_level.txt
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-25 14:38:50.868650 clannotation-0.0.5/tests/
+-rw-rw-r--   0 martin    (1000) martin    (1000)    18311 2023-04-20 08:47:46.000000 clannotation-0.0.5/tests/test_annotator_plugin.py
```

### Comparing `clannotation-0.0.4/LICENSE.md` & `clannotation-0.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `clannotation-0.0.4/PKG-INFO` & `clannotation-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clannotation
-Version: 0.0.4
+Version: 0.0.5
 Summary: The Crossref Labs annotation tool.
 Home-page: https://gitlab.com/crossref/labs/annotator
 Author: Martin Paul Eve
 Author-email: meve@crossref.org
 Maintainer-email: Martin Paul Eve <meve@crossref.org>
 License: Copyright &copy; 2023 Crossref
```

### Comparing `clannotation-0.0.4/README.md` & `clannotation-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `clannotation-0.0.4/pyproject.toml` & `clannotation-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "clannotation"
-version = "0.0.4"
+version = "0.0.5"
 description = "The Crossref Labs annotation tool."
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE.md"}
 keywords = ["API", "Crossref", "annotation", "AWS", "Lambda"]
 authors = [
   {email = "meve@crossref.org"},
@@ -17,15 +17,15 @@
   "Development Status :: 4 - Beta",
   "Programming Language :: Python"
 ]
 
 dependencies = [
     "claws==0.0.11",
     "aws-lambda-powertools[all]",
-    "longsight==1.0.5",
+    "longsight>=1.0.5",
     "moto",
     "botocore"
 ]
 
 [project.urls]
 homepage = "https://labs.crossref.org"
 documentation = "https://labs.crossref.org"
```

### Comparing `clannotation-0.0.4/setup.cfg` & `clannotation-0.0.5/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = clannotation
-version = 0.0.4
+version = 0.0.5
 description = The Crossref Labs annotation tool.
 url = https://gitlab.com/crossref/labs/annotator
 author = Martin Paul Eve
 author_email = meve@crossref.org
 license = MIT
 classifiers = 
 	Intended Audience :: Developers
@@ -23,15 +23,15 @@
 include_package_data = true
 package_dir = =src
 packages = find:
 python_requires = >=3.8
 install_requires = 
 	claws==0.0.11
 	aws-lambda-powertools[all]
-	longsight==1.0.5
+	longsight>=1.0.5
 	moto
 	botocore
 
 [options.packages.find]
 where = src
 
 [egg_info]
```

### Comparing `clannotation-0.0.4/src/clannotation/annotator.py` & `clannotation-0.0.5/src/clannotation/annotator.py`

 * *Files identical despite different names*

### Comparing `clannotation-0.0.4/src/clannotation.egg-info/PKG-INFO` & `clannotation-0.0.5/src/clannotation.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clannotation
-Version: 0.0.4
+Version: 0.0.5
 Summary: The Crossref Labs annotation tool.
 Home-page: https://gitlab.com/crossref/labs/annotator
 Author: Martin Paul Eve
 Author-email: meve@crossref.org
 Maintainer-email: Martin Paul Eve <meve@crossref.org>
 License: Copyright &copy; 2023 Crossref
```

### Comparing `clannotation-0.0.4/tests/test_annotator_plugin.py` & `clannotation-0.0.5/tests/test_annotator_plugin.py`

 * *Files identical despite different names*

