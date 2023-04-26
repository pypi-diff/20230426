# Comparing `tmp/RunRate-0.0.4.tar.gz` & `tmp/RunRate-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RunRate-0.0.4.tar", last modified: Wed Apr 26 08:14:19 2023, max compression
+gzip compressed data, was "RunRate-0.0.5.tar", last modified: Wed Apr 26 08:19:02 2023, max compression
```

## Comparing `RunRate-0.0.4.tar` & `RunRate-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 akshay     (501) staff       (20)        0 2023-04-26 08:14:19.052818 RunRate-0.0.4/
--rw-r--r--   0 akshay     (501) staff       (20)       77 2023-04-26 07:11:04.000000 RunRate-0.0.4/CHANGELOG.txt
--rw-r--r--   0 akshay     (501) staff       (20)     1106 2023-04-26 06:35:24.000000 RunRate-0.0.4/LICENCE.txt
--rw-r--r--   0 akshay     (501) staff       (20)       25 2023-04-26 06:35:28.000000 RunRate-0.0.4/MANIFEST.in
--rw-r--r--   0 akshay     (501) staff       (20)      749 2023-04-26 08:14:19.052682 RunRate-0.0.4/PKG-INFO
--rw-r--r--   0 akshay     (501) staff       (20)      182 2023-04-26 06:35:31.000000 RunRate-0.0.4/README.txt
-drwxr-xr-x   0 akshay     (501) staff       (20)        0 2023-04-26 08:14:19.052047 RunRate-0.0.4/RunRate.egg-info/
--rw-r--r--   0 akshay     (501) staff       (20)      749 2023-04-26 08:14:19.000000 RunRate-0.0.4/RunRate.egg-info/PKG-INFO
--rw-r--r--   0 akshay     (501) staff       (20)      261 2023-04-26 08:14:19.000000 RunRate-0.0.4/RunRate.egg-info/SOURCES.txt
--rw-r--r--   0 akshay     (501) staff       (20)        1 2023-04-26 08:14:19.000000 RunRate-0.0.4/RunRate.egg-info/dependency_links.txt
--rw-r--r--   0 akshay     (501) staff       (20)       23 2023-04-26 08:14:19.000000 RunRate-0.0.4/RunRate.egg-info/top_level.txt
-drwxr-xr-x   0 akshay     (501) staff       (20)        0 2023-04-26 08:14:19.052263 RunRate-0.0.4/runrate_properties_pkg/
--rw-r--r--   0 akshay     (501) staff       (20)        0 2023-04-26 07:32:40.000000 RunRate-0.0.4/runrate_properties_pkg/__init__.py
--rw-r--r--   0 akshay     (501) staff       (20)       95 2023-04-26 08:13:34.000000 RunRate-0.0.4/runrate_properties_pkg/runrate_properties.py
--rw-r--r--   0 akshay     (501) staff       (20)       38 2023-04-26 08:14:19.052862 RunRate-0.0.4/setup.cfg
--rw-r--r--   0 akshay     (501) staff       (20)      676 2023-04-26 08:14:14.000000 RunRate-0.0.4/setup.py
+drwxr-xr-x   0 akshay     (501) staff       (20)        0 2023-04-26 08:19:02.784485 RunRate-0.0.5/
+-rw-r--r--   0 akshay     (501) staff       (20)       77 2023-04-26 07:11:04.000000 RunRate-0.0.5/CHANGELOG.txt
+-rw-r--r--   0 akshay     (501) staff       (20)     1106 2023-04-26 06:35:24.000000 RunRate-0.0.5/LICENCE.txt
+-rw-r--r--   0 akshay     (501) staff       (20)       25 2023-04-26 06:35:28.000000 RunRate-0.0.5/MANIFEST.in
+-rw-r--r--   0 akshay     (501) staff       (20)      749 2023-04-26 08:19:02.784366 RunRate-0.0.5/PKG-INFO
+-rw-r--r--   0 akshay     (501) staff       (20)      182 2023-04-26 06:35:31.000000 RunRate-0.0.5/README.txt
+drwxr-xr-x   0 akshay     (501) staff       (20)        0 2023-04-26 08:19:02.783780 RunRate-0.0.5/RunRate.egg-info/
+-rw-r--r--   0 akshay     (501) staff       (20)      749 2023-04-26 08:19:02.000000 RunRate-0.0.5/RunRate.egg-info/PKG-INFO
+-rw-r--r--   0 akshay     (501) staff       (20)      261 2023-04-26 08:19:02.000000 RunRate-0.0.5/RunRate.egg-info/SOURCES.txt
+-rw-r--r--   0 akshay     (501) staff       (20)        1 2023-04-26 08:19:02.000000 RunRate-0.0.5/RunRate.egg-info/dependency_links.txt
+-rw-r--r--   0 akshay     (501) staff       (20)       23 2023-04-26 08:19:02.000000 RunRate-0.0.5/RunRate.egg-info/top_level.txt
+drwxr-xr-x   0 akshay     (501) staff       (20)        0 2023-04-26 08:19:02.784031 RunRate-0.0.5/runrate_properties_pkg/
+-rw-r--r--   0 akshay     (501) staff       (20)        0 2023-04-26 07:32:40.000000 RunRate-0.0.5/runrate_properties_pkg/__init__.py
+-rw-r--r--   0 akshay     (501) staff       (20)      106 2023-04-26 08:18:12.000000 RunRate-0.0.5/runrate_properties_pkg/runrate_properties.py
+-rw-r--r--   0 akshay     (501) staff       (20)       38 2023-04-26 08:19:02.784543 RunRate-0.0.5/setup.cfg
+-rw-r--r--   0 akshay     (501) staff       (20)      676 2023-04-26 08:18:50.000000 RunRate-0.0.5/setup.py
```

### Comparing `RunRate-0.0.4/LICENCE.txt` & `RunRate-0.0.5/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `RunRate-0.0.4/PKG-INFO` & `RunRate-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RunRate
-Version: 0.0.4
+Version: 0.0.5
 Summary: A very basic discount calculator
 Home-page: 
 Author: Pradeep Tej Dandikuppam Sreenivasulu
 Author-email: x21196303@student.ncirl.ie
 License: MIT
 Keywords: Cricket
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `RunRate-0.0.4/RunRate.egg-info/PKG-INFO` & `RunRate-0.0.5/RunRate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RunRate
-Version: 0.0.4
+Version: 0.0.5
 Summary: A very basic discount calculator
 Home-page: 
 Author: Pradeep Tej Dandikuppam Sreenivasulu
 Author-email: x21196303@student.ncirl.ie
 License: MIT
 Keywords: Cricket
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `RunRate-0.0.4/setup.py` & `RunRate-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: MacOS',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3.8'
 ]
  
 setup(
   name='RunRate',
-  version='0.0.4',
+  version='0.0.5',
   description='A very basic discount calculator',
   long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
   url='',  
   author='Pradeep Tej Dandikuppam Sreenivasulu',
   author_email='x21196303@student.ncirl.ie',
   license='MIT', 
   classifiers=classifiers,
```

