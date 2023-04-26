# Comparing `tmp/fakify-1.0.0.tar.gz` & `tmp/fakify-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fakify-1.0.0.tar", last modified: Wed Apr 26 12:02:05 2023, max compression
+gzip compressed data, was "fakify-1.0.1.tar", last modified: Wed Apr 26 18:53:13 2023, max compression
```

## Comparing `fakify-1.0.0.tar` & `fakify-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 itssoumit   (501) staff       (20)        0 2023-04-26 12:02:05.779579 fakify-1.0.0/
--rw-r--r--   0 itssoumit   (501) staff       (20)     1066 2023-04-24 22:08:05.000000 fakify-1.0.0/LICENSE
--rw-r--r--   0 itssoumit   (501) staff       (20)       20 2023-04-26 09:35:40.000000 fakify-1.0.0/MANIFEST.in
--rw-r--r--   0 itssoumit   (501) staff       (20)     3660 2023-04-26 12:02:05.779686 fakify-1.0.0/PKG-INFO
--rw-r--r--   0 itssoumit   (501) staff       (20)     3191 2023-04-26 11:47:27.000000 fakify-1.0.0/README.md
-drwxr-xr-x   0 itssoumit   (501) staff       (20)        0 2023-04-26 12:02:05.778267 fakify-1.0.0/fakify/
--rw-r--r--   0 itssoumit   (501) staff       (20)     4065 2023-04-25 20:37:06.000000 fakify-1.0.0/fakify/countries.csv
--rw-r--r--   0 itssoumit   (501) staff       (20)     6271 2023-04-24 19:08:54.000000 fakify-1.0.0/fakify/domains-common.csv
--rw-r--r--   0 itssoumit   (501) staff       (20)    85116 2023-04-24 17:39:08.000000 fakify-1.0.0/fakify/domains.csv
--rw-r--r--   0 itssoumit   (501) staff       (20)      679 2023-04-24 20:06:34.000000 fakify-1.0.0/fakify/firstname-female.csv
--rw-r--r--   0 itssoumit   (501) staff       (20)      643 2023-04-24 20:05:25.000000 fakify-1.0.0/fakify/firstname-male.csv
--rw-r--r--   0 itssoumit   (501) staff       (20)     1064 2023-04-24 12:30:18.000000 fakify-1.0.0/fakify/lastname.csv
-drwxr-xr-x   0 itssoumit   (501) staff       (20)        0 2023-04-26 12:02:05.779456 fakify-1.0.0/fakify.egg-info/
--rw-r--r--   0 itssoumit   (501) staff       (20)     3660 2023-04-26 12:02:05.000000 fakify-1.0.0/fakify.egg-info/PKG-INFO
--rw-r--r--   0 itssoumit   (501) staff       (20)      343 2023-04-26 12:02:05.000000 fakify-1.0.0/fakify.egg-info/SOURCES.txt
--rw-r--r--   0 itssoumit   (501) staff       (20)        1 2023-04-26 12:02:05.000000 fakify-1.0.0/fakify.egg-info/dependency_links.txt
--rw-r--r--   0 itssoumit   (501) staff       (20)        7 2023-04-26 12:02:05.000000 fakify-1.0.0/fakify.egg-info/requires.txt
--rw-r--r--   0 itssoumit   (501) staff       (20)        1 2023-04-26 12:02:05.000000 fakify-1.0.0/fakify.egg-info/top_level.txt
--rw-r--r--   0 itssoumit   (501) staff       (20)      103 2023-04-25 17:18:22.000000 fakify-1.0.0/pyproject.toml
--rw-r--r--   0 itssoumit   (501) staff       (20)      583 2023-04-26 12:02:05.779954 fakify-1.0.0/setup.cfg
+drwxr-xr-x   0 itssoumit   (501) staff       (20)        0 2023-04-26 18:53:13.933057 fakify-1.0.1/
+-rw-r--r--   0 itssoumit   (501) staff       (20)     1066 2023-04-24 22:08:05.000000 fakify-1.0.1/LICENSE
+-rw-r--r--   0 itssoumit   (501) staff       (20)       20 2023-04-26 09:35:40.000000 fakify-1.0.1/MANIFEST.in
+-rw-r--r--   0 itssoumit   (501) staff       (20)     3727 2023-04-26 18:53:13.933154 fakify-1.0.1/PKG-INFO
+-rw-r--r--   0 itssoumit   (501) staff       (20)     3258 2023-04-26 18:52:47.000000 fakify-1.0.1/README.md
+drwxr-xr-x   0 itssoumit   (501) staff       (20)        0 2023-04-26 18:53:13.932165 fakify-1.0.1/fakify/
+-rw-r--r--   0 itssoumit   (501) staff       (20)     4065 2023-04-25 20:37:06.000000 fakify-1.0.1/fakify/countries.csv
+-rw-r--r--   0 itssoumit   (501) staff       (20)     6271 2023-04-24 19:08:54.000000 fakify-1.0.1/fakify/domains-common.csv
+-rw-r--r--   0 itssoumit   (501) staff       (20)    85116 2023-04-24 17:39:08.000000 fakify-1.0.1/fakify/domains.csv
+-rw-r--r--   0 itssoumit   (501) staff       (20)      679 2023-04-24 20:06:34.000000 fakify-1.0.1/fakify/firstname-female.csv
+-rw-r--r--   0 itssoumit   (501) staff       (20)      643 2023-04-24 20:05:25.000000 fakify-1.0.1/fakify/firstname-male.csv
+-rw-r--r--   0 itssoumit   (501) staff       (20)     1064 2023-04-24 12:30:18.000000 fakify-1.0.1/fakify/lastname.csv
+drwxr-xr-x   0 itssoumit   (501) staff       (20)        0 2023-04-26 18:53:13.932946 fakify-1.0.1/fakify.egg-info/
+-rw-r--r--   0 itssoumit   (501) staff       (20)     3727 2023-04-26 18:53:13.000000 fakify-1.0.1/fakify.egg-info/PKG-INFO
+-rw-r--r--   0 itssoumit   (501) staff       (20)      343 2023-04-26 18:53:13.000000 fakify-1.0.1/fakify.egg-info/SOURCES.txt
+-rw-r--r--   0 itssoumit   (501) staff       (20)        1 2023-04-26 18:53:13.000000 fakify-1.0.1/fakify.egg-info/dependency_links.txt
+-rw-r--r--   0 itssoumit   (501) staff       (20)        7 2023-04-26 18:53:13.000000 fakify-1.0.1/fakify.egg-info/requires.txt
+-rw-r--r--   0 itssoumit   (501) staff       (20)        1 2023-04-26 18:53:13.000000 fakify-1.0.1/fakify.egg-info/top_level.txt
+-rw-r--r--   0 itssoumit   (501) staff       (20)      103 2023-04-25 17:18:22.000000 fakify-1.0.1/pyproject.toml
+-rw-r--r--   0 itssoumit   (501) staff       (20)      583 2023-04-26 18:53:13.933434 fakify-1.0.1/setup.cfg
```

### Comparing `fakify-1.0.0/LICENSE` & `fakify-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fakify-1.0.0/PKG-INFO` & `fakify-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fakify
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python package for generating random dummy data for testing purposes.
 Home-page: https://github.com/ITSSOUMIT/fakify
 Author: Soumit Das
 Author-email: its.soumit.das@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -105,12 +105,13 @@
 ### Country
 ```python
 from fakify import generator as ge
 ge.country(quantity, countrycode=False)
 ```
 | Parameter | Type | Description |
 | :-- | :-- | :-- |
+| quantity | **all** (*Default*) | Returns list of all countries |
 | quantity | **numeric value** | Quantity of results to be generated |
 |countrycode|**False** (*Default*)|Donot provide country code along with name|
 ||**True**|Provide country code along with name|
 
 Output type: `Python list []`
```

### Comparing `fakify-1.0.0/README.md` & `fakify-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -91,12 +91,13 @@
 ### Country
 ```python
 from fakify import generator as ge
 ge.country(quantity, countrycode=False)
 ```
 | Parameter | Type | Description |
 | :-- | :-- | :-- |
+| quantity | **all** (*Default*) | Returns list of all countries |
 | quantity | **numeric value** | Quantity of results to be generated |
 |countrycode|**False** (*Default*)|Donot provide country code along with name|
 ||**True**|Provide country code along with name|
 
 Output type: `Python list []`
```

### Comparing `fakify-1.0.0/fakify/countries.csv` & `fakify-1.0.1/fakify/countries.csv`

 * *Files identical despite different names*

### Comparing `fakify-1.0.0/fakify/domains-common.csv` & `fakify-1.0.1/fakify/domains-common.csv`

 * *Files identical despite different names*

### Comparing `fakify-1.0.0/fakify/domains.csv` & `fakify-1.0.1/fakify/domains.csv`

 * *Files identical despite different names*

### Comparing `fakify-1.0.0/fakify/firstname-female.csv` & `fakify-1.0.1/fakify/firstname-female.csv`

 * *Files identical despite different names*

### Comparing `fakify-1.0.0/fakify/firstname-male.csv` & `fakify-1.0.1/fakify/firstname-male.csv`

 * *Files identical despite different names*

### Comparing `fakify-1.0.0/fakify/lastname.csv` & `fakify-1.0.1/fakify/lastname.csv`

 * *Files identical despite different names*

### Comparing `fakify-1.0.0/fakify.egg-info/PKG-INFO` & `fakify-1.0.1/fakify.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fakify
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python package for generating random dummy data for testing purposes.
 Home-page: https://github.com/ITSSOUMIT/fakify
 Author: Soumit Das
 Author-email: its.soumit.das@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -105,12 +105,13 @@
 ### Country
 ```python
 from fakify import generator as ge
 ge.country(quantity, countrycode=False)
 ```
 | Parameter | Type | Description |
 | :-- | :-- | :-- |
+| quantity | **all** (*Default*) | Returns list of all countries |
 | quantity | **numeric value** | Quantity of results to be generated |
 |countrycode|**False** (*Default*)|Donot provide country code along with name|
 ||**True**|Provide country code along with name|
 
 Output type: `Python list []`
```

### Comparing `fakify-1.0.0/setup.cfg` & `fakify-1.0.1/setup.cfg`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = fakify
-version = 1.0.0
+version = 1.0.1
 author = Soumit Das
 author_email = its.soumit.das@gmail.com
 description = A Python package for generating random dummy data for testing purposes.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ITSSOUMIT/fakify
 classifiers =
```

