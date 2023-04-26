# Comparing `tmp/fakify-1.0.2.tar.gz` & `tmp/fakify-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fakify-1.0.2.tar", last modified: Wed Apr 26 18:59:30 2023, max compression
+gzip compressed data, was "fakify-1.0.3.tar", last modified: Wed Apr 26 19:25:14 2023, max compression
```

## Comparing `fakify-1.0.2.tar` & `fakify-1.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 itssoumit   (501) staff       (20)        0 2023-04-26 18:59:30.576768 fakify-1.0.2/
--rw-r--r--   0 itssoumit   (501) staff       (20)     1066 2023-04-24 22:08:05.000000 fakify-1.0.2/LICENSE
--rw-r--r--   0 itssoumit   (501) staff       (20)       20 2023-04-26 09:35:40.000000 fakify-1.0.2/MANIFEST.in
--rw-r--r--   0 itssoumit   (501) staff       (20)     3727 2023-04-26 18:59:30.576872 fakify-1.0.2/PKG-INFO
--rw-r--r--   0 itssoumit   (501) staff       (20)     3258 2023-04-26 18:58:35.000000 fakify-1.0.2/README.md
-drwxr-xr-x   0 itssoumit   (501) staff       (20)        0 2023-04-26 18:59:30.575835 fakify-1.0.2/fakify/
--rw-r--r--   0 itssoumit   (501) staff       (20)     4065 2023-04-25 20:37:06.000000 fakify-1.0.2/fakify/countries.csv
--rw-r--r--   0 itssoumit   (501) staff       (20)     6271 2023-04-24 19:08:54.000000 fakify-1.0.2/fakify/domains-common.csv
--rw-r--r--   0 itssoumit   (501) staff       (20)    85116 2023-04-24 17:39:08.000000 fakify-1.0.2/fakify/domains.csv
--rw-r--r--   0 itssoumit   (501) staff       (20)      679 2023-04-24 20:06:34.000000 fakify-1.0.2/fakify/firstname-female.csv
--rw-r--r--   0 itssoumit   (501) staff       (20)      643 2023-04-24 20:05:25.000000 fakify-1.0.2/fakify/firstname-male.csv
--rw-r--r--   0 itssoumit   (501) staff       (20)     1064 2023-04-24 12:30:18.000000 fakify-1.0.2/fakify/lastname.csv
-drwxr-xr-x   0 itssoumit   (501) staff       (20)        0 2023-04-26 18:59:30.576655 fakify-1.0.2/fakify.egg-info/
--rw-r--r--   0 itssoumit   (501) staff       (20)     3727 2023-04-26 18:59:30.000000 fakify-1.0.2/fakify.egg-info/PKG-INFO
--rw-r--r--   0 itssoumit   (501) staff       (20)      343 2023-04-26 18:59:30.000000 fakify-1.0.2/fakify.egg-info/SOURCES.txt
--rw-r--r--   0 itssoumit   (501) staff       (20)        1 2023-04-26 18:59:30.000000 fakify-1.0.2/fakify.egg-info/dependency_links.txt
--rw-r--r--   0 itssoumit   (501) staff       (20)        7 2023-04-26 18:59:30.000000 fakify-1.0.2/fakify.egg-info/requires.txt
--rw-r--r--   0 itssoumit   (501) staff       (20)        1 2023-04-26 18:59:30.000000 fakify-1.0.2/fakify.egg-info/top_level.txt
--rw-r--r--   0 itssoumit   (501) staff       (20)      103 2023-04-25 17:18:22.000000 fakify-1.0.2/pyproject.toml
--rw-r--r--   0 itssoumit   (501) staff       (20)      583 2023-04-26 18:59:30.577167 fakify-1.0.2/setup.cfg
+drwxr-xr-x   0 itssoumit   (501) staff       (20)        0 2023-04-26 19:25:14.156706 fakify-1.0.3/
+-rw-r--r--   0 itssoumit   (501) staff       (20)     1066 2023-04-24 22:08:05.000000 fakify-1.0.3/LICENSE
+-rw-r--r--   0 itssoumit   (501) staff       (20)       20 2023-04-26 09:35:40.000000 fakify-1.0.3/MANIFEST.in
+-rw-r--r--   0 itssoumit   (501) staff       (20)     3717 2023-04-26 19:25:14.156787 fakify-1.0.3/PKG-INFO
+-rw-r--r--   0 itssoumit   (501) staff       (20)     3248 2023-04-26 19:24:56.000000 fakify-1.0.3/README.md
+drwxr-xr-x   0 itssoumit   (501) staff       (20)        0 2023-04-26 19:25:14.155771 fakify-1.0.3/fakify/
+-rw-r--r--   0 itssoumit   (501) staff       (20)     4065 2023-04-25 20:37:06.000000 fakify-1.0.3/fakify/countries.csv
+-rw-r--r--   0 itssoumit   (501) staff       (20)     6271 2023-04-24 19:08:54.000000 fakify-1.0.3/fakify/domains-common.csv
+-rw-r--r--   0 itssoumit   (501) staff       (20)    85116 2023-04-24 17:39:08.000000 fakify-1.0.3/fakify/domains.csv
+-rw-r--r--   0 itssoumit   (501) staff       (20)      679 2023-04-24 20:06:34.000000 fakify-1.0.3/fakify/firstname-female.csv
+-rw-r--r--   0 itssoumit   (501) staff       (20)      643 2023-04-24 20:05:25.000000 fakify-1.0.3/fakify/firstname-male.csv
+-rw-r--r--   0 itssoumit   (501) staff       (20)     1064 2023-04-24 12:30:18.000000 fakify-1.0.3/fakify/lastname.csv
+drwxr-xr-x   0 itssoumit   (501) staff       (20)        0 2023-04-26 19:25:14.156592 fakify-1.0.3/fakify.egg-info/
+-rw-r--r--   0 itssoumit   (501) staff       (20)     3717 2023-04-26 19:25:14.000000 fakify-1.0.3/fakify.egg-info/PKG-INFO
+-rw-r--r--   0 itssoumit   (501) staff       (20)      343 2023-04-26 19:25:14.000000 fakify-1.0.3/fakify.egg-info/SOURCES.txt
+-rw-r--r--   0 itssoumit   (501) staff       (20)        1 2023-04-26 19:25:14.000000 fakify-1.0.3/fakify.egg-info/dependency_links.txt
+-rw-r--r--   0 itssoumit   (501) staff       (20)        7 2023-04-26 19:25:14.000000 fakify-1.0.3/fakify.egg-info/requires.txt
+-rw-r--r--   0 itssoumit   (501) staff       (20)        1 2023-04-26 19:25:14.000000 fakify-1.0.3/fakify.egg-info/top_level.txt
+-rw-r--r--   0 itssoumit   (501) staff       (20)      103 2023-04-25 17:18:22.000000 fakify-1.0.3/pyproject.toml
+-rw-r--r--   0 itssoumit   (501) staff       (20)      583 2023-04-26 19:25:14.157061 fakify-1.0.3/setup.cfg
```

### Comparing `fakify-1.0.2/LICENSE` & `fakify-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fakify-1.0.2/PKG-INFO` & `fakify-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fakify
-Version: 1.0.2
+Version: 1.0.3
 Summary: A Python package for generating random dummy data for testing purposes.
 Home-page: https://github.com/ITSSOUMIT/fakify
 Author: Soumit Das
 Author-email: its.soumit.das@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -16,15 +16,15 @@
 A Python package for generating random dummy data for testing purposes.
 
 Installation:
 ```bash
 pip install fakify
 ```
 
-Data types supported as of `v1.0.2`:\
+Data types supported as of `v1.0.3`:\
 👉 [Name](#name)\
 👉 [Email](#email)\
 👉 [Password](#password)\
 👉 [Website](#website)\
 👉 [Phone](#phone)\
 👉 [Country](#country)
 
@@ -106,12 +106,12 @@
 ```python
 from fakify import generator as ge
 ge.country(quantity, countrycode=False)
 ```
 | Parameter | Type | Description |
 | :-- | :-- | :-- |
 | quantity | **all** (*Default*) | Returns list of all countries |
-| quantity | **numeric value** | Quantity of results to be generated |
+|| **numeric value** | Quantity of results to be generated |
 |countrycode|**False** (*Default*)|Donot provide country code along with name|
 ||**True**|Provide country code along with name|
 
 Output type: `Python list []`
```

### Comparing `fakify-1.0.2/README.md` & `fakify-1.0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 A Python package for generating random dummy data for testing purposes.
 
 Installation:
 ```bash
 pip install fakify
 ```
 
-Data types supported as of `v1.0.2`:\
+Data types supported as of `v1.0.3`:\
 👉 [Name](#name)\
 👉 [Email](#email)\
 👉 [Password](#password)\
 👉 [Website](#website)\
 👉 [Phone](#phone)\
 👉 [Country](#country)
 
@@ -92,12 +92,12 @@
 ```python
 from fakify import generator as ge
 ge.country(quantity, countrycode=False)
 ```
 | Parameter | Type | Description |
 | :-- | :-- | :-- |
 | quantity | **all** (*Default*) | Returns list of all countries |
-| quantity | **numeric value** | Quantity of results to be generated |
+|| **numeric value** | Quantity of results to be generated |
 |countrycode|**False** (*Default*)|Donot provide country code along with name|
 ||**True**|Provide country code along with name|
 
 Output type: `Python list []`
```

### Comparing `fakify-1.0.2/fakify/countries.csv` & `fakify-1.0.3/fakify/countries.csv`

 * *Files identical despite different names*

### Comparing `fakify-1.0.2/fakify/domains-common.csv` & `fakify-1.0.3/fakify/domains-common.csv`

 * *Files identical despite different names*

### Comparing `fakify-1.0.2/fakify/domains.csv` & `fakify-1.0.3/fakify/domains.csv`

 * *Files identical despite different names*

### Comparing `fakify-1.0.2/fakify/firstname-female.csv` & `fakify-1.0.3/fakify/firstname-female.csv`

 * *Files identical despite different names*

### Comparing `fakify-1.0.2/fakify/firstname-male.csv` & `fakify-1.0.3/fakify/firstname-male.csv`

 * *Files identical despite different names*

### Comparing `fakify-1.0.2/fakify/lastname.csv` & `fakify-1.0.3/fakify/lastname.csv`

 * *Files identical despite different names*

### Comparing `fakify-1.0.2/fakify.egg-info/PKG-INFO` & `fakify-1.0.3/fakify.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fakify
-Version: 1.0.2
+Version: 1.0.3
 Summary: A Python package for generating random dummy data for testing purposes.
 Home-page: https://github.com/ITSSOUMIT/fakify
 Author: Soumit Das
 Author-email: its.soumit.das@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -16,15 +16,15 @@
 A Python package for generating random dummy data for testing purposes.
 
 Installation:
 ```bash
 pip install fakify
 ```
 
-Data types supported as of `v1.0.2`:\
+Data types supported as of `v1.0.3`:\
 👉 [Name](#name)\
 👉 [Email](#email)\
 👉 [Password](#password)\
 👉 [Website](#website)\
 👉 [Phone](#phone)\
 👉 [Country](#country)
 
@@ -106,12 +106,12 @@
 ```python
 from fakify import generator as ge
 ge.country(quantity, countrycode=False)
 ```
 | Parameter | Type | Description |
 | :-- | :-- | :-- |
 | quantity | **all** (*Default*) | Returns list of all countries |
-| quantity | **numeric value** | Quantity of results to be generated |
+|| **numeric value** | Quantity of results to be generated |
 |countrycode|**False** (*Default*)|Donot provide country code along with name|
 ||**True**|Provide country code along with name|
 
 Output type: `Python list []`
```

### Comparing `fakify-1.0.2/setup.cfg` & `fakify-1.0.3/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = fakify
-version = 1.0.2
+version = 1.0.3
 author = Soumit Das
 author_email = its.soumit.das@gmail.com
 description = A Python package for generating random dummy data for testing purposes.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ITSSOUMIT/fakify
 classifiers =
```

