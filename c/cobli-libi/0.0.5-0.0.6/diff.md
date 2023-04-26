# Comparing `tmp/cobli-libi-0.0.5.tar.gz` & `tmp/cobli-libi-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/cobli/Bruno/Cobli/Repos/cobli-libi/dist/.tmp-r1hifezb/cobli-libi-0.0.5.tar", last modified: Tue Apr 25 14:00:44 2023, max compression
+gzip compressed data, was "/home/matheus/Documents/projects/cobli-libi/dist/.tmp-5kzxfuxr/cobli-libi-0.0.6.tar", last modified: Tue Apr 25 18:39:35 2023, max compression
```

## Comparing `cobli-libi-0.0.5.tar` & `cobli-libi-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 cobli     (1000) cobli     (1000)        0 2023-04-25 14:00:44.399073 cobli-libi-0.0.5/
--rw-rw-r--   0 cobli     (1000) cobli     (1000)     2789 2023-04-25 14:00:44.399073 cobli-libi-0.0.5/PKG-INFO
--rw-rw-r--   0 cobli     (1000) cobli     (1000)     2554 2023-04-25 13:57:04.000000 cobli-libi-0.0.5/README.md
-drwxrwxr-x   0 cobli     (1000) cobli     (1000)        0 2023-04-25 14:00:44.399073 cobli-libi-0.0.5/cobli_libi.egg-info/
--rw-rw-r--   0 cobli     (1000) cobli     (1000)     2789 2023-04-25 14:00:44.000000 cobli-libi-0.0.5/cobli_libi.egg-info/PKG-INFO
--rw-rw-r--   0 cobli     (1000) cobli     (1000)      202 2023-04-25 14:00:44.000000 cobli-libi-0.0.5/cobli_libi.egg-info/SOURCES.txt
--rw-rw-r--   0 cobli     (1000) cobli     (1000)        1 2023-04-25 14:00:44.000000 cobli-libi-0.0.5/cobli_libi.egg-info/dependency_links.txt
--rw-rw-r--   0 cobli     (1000) cobli     (1000)        5 2023-04-25 14:00:44.000000 cobli-libi-0.0.5/cobli_libi.egg-info/top_level.txt
-drwxrwxr-x   0 cobli     (1000) cobli     (1000)        0 2023-04-25 14:00:44.399073 cobli-libi-0.0.5/libi/
--rw-rw-r--   0 cobli     (1000) cobli     (1000)     4190 2023-04-25 13:59:57.000000 cobli-libi-0.0.5/libi/dataframes.py
--rw-rw-r--   0 cobli     (1000) cobli     (1000)       46 2023-04-25 12:39:02.000000 cobli-libi-0.0.5/libi/errors.py
--rw-rw-r--   0 cobli     (1000) cobli     (1000)     4854 2023-04-25 13:57:04.000000 cobli-libi-0.0.5/libi/utils.py
--rw-rw-r--   0 cobli     (1000) cobli     (1000)       38 2023-04-25 14:00:44.399073 cobli-libi-0.0.5/setup.cfg
--rw-rw-r--   0 cobli     (1000) cobli     (1000)      445 2023-04-25 13:57:53.000000 cobli-libi-0.0.5/setup.py
+drwxrwxr-x   0 matheus   (1000) matheus   (1000)        0 2023-04-25 18:39:35.317519 cobli-libi-0.0.6/
+-rw-rw-r--   0 matheus   (1000) matheus   (1000)     2888 2023-04-25 18:39:35.317519 cobli-libi-0.0.6/PKG-INFO
+-rw-rw-r--   0 matheus   (1000) matheus   (1000)     2653 2023-04-25 18:39:23.000000 cobli-libi-0.0.6/README.md
+drwxrwxr-x   0 matheus   (1000) matheus   (1000)        0 2023-04-25 18:39:35.317519 cobli-libi-0.0.6/cobli_libi.egg-info/
+-rw-rw-r--   0 matheus   (1000) matheus   (1000)     2888 2023-04-25 18:39:35.000000 cobli-libi-0.0.6/cobli_libi.egg-info/PKG-INFO
+-rw-rw-r--   0 matheus   (1000) matheus   (1000)      202 2023-04-25 18:39:35.000000 cobli-libi-0.0.6/cobli_libi.egg-info/SOURCES.txt
+-rw-rw-r--   0 matheus   (1000) matheus   (1000)        1 2023-04-25 18:39:35.000000 cobli-libi-0.0.6/cobli_libi.egg-info/dependency_links.txt
+-rw-rw-r--   0 matheus   (1000) matheus   (1000)        5 2023-04-25 18:39:35.000000 cobli-libi-0.0.6/cobli_libi.egg-info/top_level.txt
+drwxrwxr-x   0 matheus   (1000) matheus   (1000)        0 2023-04-25 18:39:35.317519 cobli-libi-0.0.6/libi/
+-rw-rw-r--   0 matheus   (1000) matheus   (1000)     4190 2023-04-25 18:33:43.000000 cobli-libi-0.0.6/libi/dataframes.py
+-rw-rw-r--   0 matheus   (1000) matheus   (1000)       46 2023-04-25 12:13:53.000000 cobli-libi-0.0.6/libi/errors.py
+-rw-rw-r--   0 matheus   (1000) matheus   (1000)     4855 2023-04-25 18:32:27.000000 cobli-libi-0.0.6/libi/utils.py
+-rw-rw-r--   0 matheus   (1000) matheus   (1000)       38 2023-04-25 18:39:35.317519 cobli-libi-0.0.6/setup.cfg
+-rw-rw-r--   0 matheus   (1000) matheus   (1000)      445 2023-04-25 18:35:18.000000 cobli-libi-0.0.6/setup.py
```

### Comparing `cobli-libi-0.0.5/PKG-INFO` & `cobli-libi-0.0.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cobli-libi
-Version: 0.0.5
+Version: 0.0.6
 Summary: Generate dataframes from Cobli public API
 Home-page: https://docs.cobli.co
 Author: Marcus Beckenkamp
 Author-email: mvbeck@gmai.com
 Description-Content-Type: text/markdown
 
 # cobli-libi
@@ -72,14 +72,18 @@
 
 ## Deploy
 
 This project is in [Pypi](https://pypi.org/manage/project/cobli-libi/releases/).
 
 In order to deploy this project, the first action needed is bump the version in the file `setup.py`.
 
+Then, you will have to install build with this command:
+
+`python3 -m pip install --upgrade build`
+
 After this, you will need to build the project with this command:
 
 `python3 -m build`
 
 Then, you will have to install twine with this command:
 
 `python3 -m pip install --upgrade twine`.
```

### Comparing `cobli-libi-0.0.5/README.md` & `cobli-libi-0.0.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -63,14 +63,18 @@
 
 ## Deploy
 
 This project is in [Pypi](https://pypi.org/manage/project/cobli-libi/releases/).
 
 In order to deploy this project, the first action needed is bump the version in the file `setup.py`.
 
+Then, you will have to install build with this command:
+
+`python3 -m pip install --upgrade build`
+
 After this, you will need to build the project with this command:
 
 `python3 -m build`
 
 Then, you will have to install twine with this command:
 
 `python3 -m pip install --upgrade twine`.
```

### Comparing `cobli-libi-0.0.5/cobli_libi.egg-info/PKG-INFO` & `cobli-libi-0.0.6/cobli_libi.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cobli-libi
-Version: 0.0.5
+Version: 0.0.6
 Summary: Generate dataframes from Cobli public API
 Home-page: https://docs.cobli.co
 Author: Marcus Beckenkamp
 Author-email: mvbeck@gmai.com
 Description-Content-Type: text/markdown
 
 # cobli-libi
@@ -72,14 +72,18 @@
 
 ## Deploy
 
 This project is in [Pypi](https://pypi.org/manage/project/cobli-libi/releases/).
 
 In order to deploy this project, the first action needed is bump the version in the file `setup.py`.
 
+Then, you will have to install build with this command:
+
+`python3 -m pip install --upgrade build`
+
 After this, you will need to build the project with this command:
 
 `python3 -m build`
 
 Then, you will have to install twine with this command:
 
 `python3 -m pip install --upgrade twine`.
```

### Comparing `cobli-libi-0.0.5/libi/dataframes.py` & `cobli-libi-0.0.6/libi/dataframes.py`

 * *Files identical despite different names*

### Comparing `cobli-libi-0.0.5/libi/utils.py` & `cobli-libi-0.0.6/libi/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
     return df
 
 
 def convert_datetime_to_unix_milliseconds(date_to_convert: datetime) -> int:
     return int(time.mktime(date_to_convert.timetuple())) * 1000
 
 
-def split_intervals(start_datetime, end_datetime, days_per_interval=5):
+def split_intervals(start_datetime, end_datetime, days_per_interval=30):
     interval = end_datetime - start_datetime
     days = interval.days
 
     number_of_intervals = days // days_per_interval
     if number_of_intervals < 1:
         return [(start_datetime, end_datetime), ]
```

