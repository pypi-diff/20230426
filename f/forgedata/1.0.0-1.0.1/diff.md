# Comparing `tmp/forgedata-1.0.0.tar.gz` & `tmp/forgedata-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forgedata-1.0.0.tar", last modified: Wed Apr 26 21:31:38 2023, max compression
+gzip compressed data, was "forgedata-1.0.1.tar", last modified: Wed Apr 26 21:43:25 2023, max compression
```

## Comparing `forgedata-1.0.0.tar` & `forgedata-1.0.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 itssoumit   (501) staff       (20)        0 2023-04-26 21:31:38.611965 forgedata-1.0.0/
--rw-r--r--   0 itssoumit   (501) staff       (20)     1066 2023-04-24 22:08:05.000000 forgedata-1.0.0/LICENSE
--rw-r--r--   0 itssoumit   (501) staff       (20)       23 2023-04-26 21:31:26.000000 forgedata-1.0.0/MANIFEST.in
--rw-r--r--   0 itssoumit   (501) staff       (20)     3737 2023-04-26 21:31:38.612063 forgedata-1.0.0/PKG-INFO
--rw-r--r--   0 itssoumit   (501) staff       (20)     3272 2023-04-26 21:29:48.000000 forgedata-1.0.0/README.md
-drwxr-xr-x   0 itssoumit   (501) staff       (20)        0 2023-04-26 21:31:38.610442 forgedata-1.0.0/forgedata/
--rw-r--r--   0 itssoumit   (501) staff       (20)        0 2023-04-26 21:05:59.000000 forgedata-1.0.0/forgedata/__init__.py
--rw-r--r--   0 itssoumit   (501) staff       (20)     4065 2023-04-25 20:37:06.000000 forgedata-1.0.0/forgedata/countries.csv
--rw-r--r--   0 itssoumit   (501) staff       (20)     6271 2023-04-24 19:08:54.000000 forgedata-1.0.0/forgedata/domains-common.csv
--rw-r--r--   0 itssoumit   (501) staff       (20)    85116 2023-04-24 17:39:08.000000 forgedata-1.0.0/forgedata/domains.csv
--rw-r--r--   0 itssoumit   (501) staff       (20)      679 2023-04-24 20:06:34.000000 forgedata-1.0.0/forgedata/firstname-female.csv
--rw-r--r--   0 itssoumit   (501) staff       (20)      643 2023-04-24 20:05:25.000000 forgedata-1.0.0/forgedata/firstname-male.csv
--rw-r--r--   0 itssoumit   (501) staff       (20)    12061 2023-04-26 21:31:10.000000 forgedata-1.0.0/forgedata/generator.py
--rw-r--r--   0 itssoumit   (501) staff       (20)     1064 2023-04-24 12:30:18.000000 forgedata-1.0.0/forgedata/lastname.csv
-drwxr-xr-x   0 itssoumit   (501) staff       (20)        0 2023-04-26 21:31:38.611856 forgedata-1.0.0/forgedata.egg-info/
--rw-r--r--   0 itssoumit   (501) staff       (20)     3737 2023-04-26 21:31:38.000000 forgedata-1.0.0/forgedata.egg-info/PKG-INFO
--rw-r--r--   0 itssoumit   (501) staff       (20)      421 2023-04-26 21:31:38.000000 forgedata-1.0.0/forgedata.egg-info/SOURCES.txt
--rw-r--r--   0 itssoumit   (501) staff       (20)        1 2023-04-26 21:31:38.000000 forgedata-1.0.0/forgedata.egg-info/dependency_links.txt
--rw-r--r--   0 itssoumit   (501) staff       (20)        7 2023-04-26 21:31:38.000000 forgedata-1.0.0/forgedata.egg-info/requires.txt
--rw-r--r--   0 itssoumit   (501) staff       (20)       10 2023-04-26 21:31:38.000000 forgedata-1.0.0/forgedata.egg-info/top_level.txt
--rw-r--r--   0 itssoumit   (501) staff       (20)      103 2023-04-25 17:18:22.000000 forgedata-1.0.0/pyproject.toml
--rw-r--r--   0 itssoumit   (501) staff       (20)      579 2023-04-26 21:31:38.612323 forgedata-1.0.0/setup.cfg
+drwxr-xr-x   0 itssoumit   (501) staff       (20)        0 2023-04-26 21:43:25.202506 forgedata-1.0.1/
+-rw-r--r--   0 itssoumit   (501) staff       (20)     1066 2023-04-24 22:08:05.000000 forgedata-1.0.1/LICENSE
+-rw-r--r--   0 itssoumit   (501) staff       (20)       23 2023-04-26 21:31:26.000000 forgedata-1.0.1/MANIFEST.in
+-rw-r--r--   0 itssoumit   (501) staff       (20)     3747 2023-04-26 21:43:25.202598 forgedata-1.0.1/PKG-INFO
+-rw-r--r--   0 itssoumit   (501) staff       (20)     3272 2023-04-26 21:42:52.000000 forgedata-1.0.1/README.md
+drwxr-xr-x   0 itssoumit   (501) staff       (20)        0 2023-04-26 21:43:25.201590 forgedata-1.0.1/forgedata/
+-rw-r--r--   0 itssoumit   (501) staff       (20)        0 2023-04-26 21:05:59.000000 forgedata-1.0.1/forgedata/__init__.py
+-rw-r--r--   0 itssoumit   (501) staff       (20)     4065 2023-04-25 20:37:06.000000 forgedata-1.0.1/forgedata/countries.csv
+-rw-r--r--   0 itssoumit   (501) staff       (20)     6271 2023-04-24 19:08:54.000000 forgedata-1.0.1/forgedata/domains-common.csv
+-rw-r--r--   0 itssoumit   (501) staff       (20)    85116 2023-04-24 17:39:08.000000 forgedata-1.0.1/forgedata/domains.csv
+-rw-r--r--   0 itssoumit   (501) staff       (20)      679 2023-04-24 20:06:34.000000 forgedata-1.0.1/forgedata/firstname-female.csv
+-rw-r--r--   0 itssoumit   (501) staff       (20)      643 2023-04-24 20:05:25.000000 forgedata-1.0.1/forgedata/firstname-male.csv
+-rw-r--r--   0 itssoumit   (501) staff       (20)    12061 2023-04-26 21:31:10.000000 forgedata-1.0.1/forgedata/generator.py
+-rw-r--r--   0 itssoumit   (501) staff       (20)     1064 2023-04-24 12:30:18.000000 forgedata-1.0.1/forgedata/lastname.csv
+drwxr-xr-x   0 itssoumit   (501) staff       (20)        0 2023-04-26 21:43:25.202397 forgedata-1.0.1/forgedata.egg-info/
+-rw-r--r--   0 itssoumit   (501) staff       (20)     3747 2023-04-26 21:43:25.000000 forgedata-1.0.1/forgedata.egg-info/PKG-INFO
+-rw-r--r--   0 itssoumit   (501) staff       (20)      421 2023-04-26 21:43:25.000000 forgedata-1.0.1/forgedata.egg-info/SOURCES.txt
+-rw-r--r--   0 itssoumit   (501) staff       (20)        1 2023-04-26 21:43:25.000000 forgedata-1.0.1/forgedata.egg-info/dependency_links.txt
+-rw-r--r--   0 itssoumit   (501) staff       (20)        7 2023-04-26 21:43:25.000000 forgedata-1.0.1/forgedata.egg-info/requires.txt
+-rw-r--r--   0 itssoumit   (501) staff       (20)       10 2023-04-26 21:43:25.000000 forgedata-1.0.1/forgedata.egg-info/top_level.txt
+-rw-r--r--   0 itssoumit   (501) staff       (20)      103 2023-04-25 17:18:22.000000 forgedata-1.0.1/pyproject.toml
+-rw-r--r--   0 itssoumit   (501) staff       (20)      589 2023-04-26 21:43:25.202862 forgedata-1.0.1/setup.cfg
```

### Comparing `forgedata-1.0.0/LICENSE` & `forgedata-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `forgedata-1.0.0/PKG-INFO` & `forgedata-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: forgedata
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python package for generating random dummy data for testing purposes.
-Home-page: https://github.com/ITSSOUMIT
+Home-page: https://github.com/ITSSOUMIT/ForgeData
 Author: Soumit Das
 Author-email: its.soumit.das@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Forgedata
+# ForgeData
 A Python package for generating random dummy data for testing purposes.
 
 Installation:
 ```bash
 pip install forgedata
 ```
 
-Data types supported as of `v1.0.0`:\
+Data types supported as of `v1.0.1`:\
 👉 [Name](#name)\
 👉 [Email](#email)\
 👉 [Password](#password)\
 👉 [Website](#website)\
 👉 [Phone](#phone)\
 👉 [Country](#country)
```

### Comparing `forgedata-1.0.0/README.md` & `forgedata-1.0.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-# Forgedata
+# ForgeData
 A Python package for generating random dummy data for testing purposes.
 
 Installation:
 ```bash
 pip install forgedata
 ```
 
-Data types supported as of `v1.0.0`:\
+Data types supported as of `v1.0.1`:\
 👉 [Name](#name)\
 👉 [Email](#email)\
 👉 [Password](#password)\
 👉 [Website](#website)\
 👉 [Phone](#phone)\
 👉 [Country](#country)
```

### Comparing `forgedata-1.0.0/forgedata/countries.csv` & `forgedata-1.0.1/forgedata/countries.csv`

 * *Files identical despite different names*

### Comparing `forgedata-1.0.0/forgedata/domains-common.csv` & `forgedata-1.0.1/forgedata/domains-common.csv`

 * *Files identical despite different names*

### Comparing `forgedata-1.0.0/forgedata/domains.csv` & `forgedata-1.0.1/forgedata/domains.csv`

 * *Files identical despite different names*

### Comparing `forgedata-1.0.0/forgedata/firstname-female.csv` & `forgedata-1.0.1/forgedata/firstname-female.csv`

 * *Files identical despite different names*

### Comparing `forgedata-1.0.0/forgedata/firstname-male.csv` & `forgedata-1.0.1/forgedata/firstname-male.csv`

 * *Files identical despite different names*

### Comparing `forgedata-1.0.0/forgedata/generator.py` & `forgedata-1.0.1/forgedata/generator.py`

 * *Files identical despite different names*

### Comparing `forgedata-1.0.0/forgedata/lastname.csv` & `forgedata-1.0.1/forgedata/lastname.csv`

 * *Files identical despite different names*

### Comparing `forgedata-1.0.0/forgedata.egg-info/PKG-INFO` & `forgedata-1.0.1/forgedata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: forgedata
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python package for generating random dummy data for testing purposes.
-Home-page: https://github.com/ITSSOUMIT
+Home-page: https://github.com/ITSSOUMIT/ForgeData
 Author: Soumit Das
 Author-email: its.soumit.das@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Forgedata
+# ForgeData
 A Python package for generating random dummy data for testing purposes.
 
 Installation:
 ```bash
 pip install forgedata
 ```
 
-Data types supported as of `v1.0.0`:\
+Data types supported as of `v1.0.1`:\
 👉 [Name](#name)\
 👉 [Email](#email)\
 👉 [Password](#password)\
 👉 [Website](#website)\
 👉 [Phone](#phone)\
 👉 [Country](#country)
```

### Comparing `forgedata-1.0.0/setup.cfg` & `forgedata-1.0.1/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [metadata]
 name = forgedata
-version = 1.0.0
+version = 1.0.1
 author = Soumit Das
 author_email = its.soumit.das@gmail.com
 description = A Python package for generating random dummy data for testing purposes.
 long_description = file: README.md
 long_description_content_type = text/markdown
-url = https://github.com/ITSSOUMIT
+url = https://github.com/ITSSOUMIT/ForgeData
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 install_requires = pandas
```

