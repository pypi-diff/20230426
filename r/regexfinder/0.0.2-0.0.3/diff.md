# Comparing `tmp/regexfinder-0.0.2.tar.gz` & `tmp/regexfinder-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "regexfinder-0.0.2.tar", last modified: Fri Feb 24 14:08:31 2023, max compression
+gzip compressed data, was "regexfinder-0.0.3.tar", last modified: Wed Apr 26 15:52:55 2023, max compression
```

## Comparing `regexfinder-0.0.2.tar` & `regexfinder-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-02-24 14:08:31.477791 regexfinder-0.0.2/
--rw-rw-rw-   0        0        0     1089 2023-02-23 19:50:28.000000 regexfinder-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     3801 2023-02-24 14:08:31.477791 regexfinder-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3379 2023-02-24 14:06:29.000000 regexfinder-0.0.2/README.md
--rw-rw-rw-   0        0        0      521 2023-02-24 14:06:29.000000 regexfinder-0.0.2/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-02-24 14:08:31.437680 regexfinder-0.0.2/regexfinder/
--rw-rw-rw-   0        0        0       30 2023-02-23 17:01:49.000000 regexfinder-0.0.2/regexfinder/__init__.py
--rw-rw-rw-   0        0        0    12185 2023-02-24 14:06:29.000000 regexfinder-0.0.2/regexfinder/main.py
-drwxrwxrwx   0        0        0        0 2023-02-24 14:08:31.477791 regexfinder-0.0.2/regexfinder.egg-info/
--rw-rw-rw-   0        0        0     3801 2023-02-24 14:08:31.000000 regexfinder-0.0.2/regexfinder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      216 2023-02-24 14:08:31.000000 regexfinder-0.0.2/regexfinder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-24 14:08:31.000000 regexfinder-0.0.2/regexfinder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-02-24 14:08:31.000000 regexfinder-0.0.2/regexfinder.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-24 14:08:31.477791 regexfinder-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-26 15:52:55.086166 regexfinder-0.0.3/
+-rw-rw-rw-   0        0        0     1089 2023-02-23 19:50:28.000000 regexfinder-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     3801 2023-04-26 15:52:55.086166 regexfinder-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3379 2023-02-24 14:06:29.000000 regexfinder-0.0.3/README.md
+-rw-rw-rw-   0        0        0      521 2023-04-26 15:52:00.000000 regexfinder-0.0.3/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-04-26 15:52:55.061449 regexfinder-0.0.3/regexfinder/
+-rw-rw-rw-   0        0        0       42 2023-04-26 15:52:00.000000 regexfinder-0.0.3/regexfinder/__init__.py
+-rw-rw-rw-   0        0        0    12185 2023-02-24 14:06:29.000000 regexfinder-0.0.3/regexfinder/main.py
+drwxrwxrwx   0        0        0        0 2023-04-26 15:52:55.086166 regexfinder-0.0.3/regexfinder.egg-info/
+-rw-rw-rw-   0        0        0     3801 2023-04-26 15:52:55.000000 regexfinder-0.0.3/regexfinder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      216 2023-04-26 15:52:55.000000 regexfinder-0.0.3/regexfinder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 15:52:55.000000 regexfinder-0.0.3/regexfinder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-04-26 15:52:55.000000 regexfinder-0.0.3/regexfinder.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-26 15:52:55.086166 regexfinder-0.0.3/setup.cfg
```

### Comparing `regexfinder-0.0.2/LICENSE` & `regexfinder-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `regexfinder-0.0.2/PKG-INFO` & `regexfinder-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regexfinder
-Version: 0.0.2
+Version: 0.0.3
 Author-email: Flori Batusha <floribatusha0@gmail.com>
 Project-URL: Check Github, https://github.com/riflosnake/RegexFinder
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `regexfinder-0.0.2/README.md` & `regexfinder-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `regexfinder-0.0.2/pyproject.toml` & `regexfinder-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "regexfinder"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Flori Batusha", email="floribatusha0@gmail.com" },
 ]
 description = ""
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `regexfinder-0.0.2/regexfinder/main.py` & `regexfinder-0.0.3/regexfinder/main.py`

 * *Files identical despite different names*

### Comparing `regexfinder-0.0.2/regexfinder.egg-info/PKG-INFO` & `regexfinder-0.0.3/regexfinder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regexfinder
-Version: 0.0.2
+Version: 0.0.3
 Author-email: Flori Batusha <floribatusha0@gmail.com>
 Project-URL: Check Github, https://github.com/riflosnake/RegexFinder
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

