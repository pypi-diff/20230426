# Comparing `tmp/aggdirect_route_estimation_calculator-0.2.tar.gz` & `tmp/aggdirect_route_estimation_calculator-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aggdirect_route_estimation_calculator-0.2.tar", last modified: Fri Mar 10 07:53:09 2023, max compression
+gzip compressed data, was "aggdirect_route_estimation_calculator-0.3.tar", last modified: Wed Apr 26 07:13:23 2023, max compression
```

## Comparing `aggdirect_route_estimation_calculator-0.2.tar` & `aggdirect_route_estimation_calculator-0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 chinmoy   (1000) chinmoy   (1000)        0 2023-03-10 07:53:09.718256 aggdirect_route_estimation_calculator-0.2/
--rw-rw-r--   0 chinmoy   (1000) chinmoy   (1000)        0 2023-03-10 07:05:23.000000 aggdirect_route_estimation_calculator-0.2/LICENSE
--rw-rw-r--   0 chinmoy   (1000) chinmoy   (1000)      504 2023-03-10 07:53:09.718256 aggdirect_route_estimation_calculator-0.2/PKG-INFO
--rw-rw-r--   0 chinmoy   (1000) chinmoy   (1000)     1520 2023-03-10 07:05:58.000000 aggdirect_route_estimation_calculator-0.2/README.md
-drwxrwxr-x   0 chinmoy   (1000) chinmoy   (1000)        0 2023-03-10 07:53:09.718256 aggdirect_route_estimation_calculator-0.2/aggdirect_route_estimation_calculator/
--rw-rw-r--   0 chinmoy   (1000) chinmoy   (1000)      930 2023-03-10 07:05:23.000000 aggdirect_route_estimation_calculator-0.2/aggdirect_route_estimation_calculator/__init__.py
-drwxrwxr-x   0 chinmoy   (1000) chinmoy   (1000)        0 2023-03-10 07:53:09.718256 aggdirect_route_estimation_calculator-0.2/aggdirect_route_estimation_calculator.egg-info/
--rw-rw-r--   0 chinmoy   (1000) chinmoy   (1000)      504 2023-03-10 07:53:09.000000 aggdirect_route_estimation_calculator-0.2/aggdirect_route_estimation_calculator.egg-info/PKG-INFO
--rw-rw-r--   0 chinmoy   (1000) chinmoy   (1000)      380 2023-03-10 07:53:09.000000 aggdirect_route_estimation_calculator-0.2/aggdirect_route_estimation_calculator.egg-info/SOURCES.txt
--rw-rw-r--   0 chinmoy   (1000) chinmoy   (1000)        1 2023-03-10 07:53:09.000000 aggdirect_route_estimation_calculator-0.2/aggdirect_route_estimation_calculator.egg-info/dependency_links.txt
--rw-rw-r--   0 chinmoy   (1000) chinmoy   (1000)        9 2023-03-10 07:53:09.000000 aggdirect_route_estimation_calculator-0.2/aggdirect_route_estimation_calculator.egg-info/requires.txt
--rw-rw-r--   0 chinmoy   (1000) chinmoy   (1000)       38 2023-03-10 07:53:09.000000 aggdirect_route_estimation_calculator-0.2/aggdirect_route_estimation_calculator.egg-info/top_level.txt
--rw-rw-r--   0 chinmoy   (1000) chinmoy   (1000)       38 2023-03-10 07:53:09.718256 aggdirect_route_estimation_calculator-0.2/setup.cfg
--rw-rw-r--   0 chinmoy   (1000) chinmoy   (1000)     1074 2023-03-10 07:52:49.000000 aggdirect_route_estimation_calculator-0.2/setup.py
+drwxrwxr-x   0 chinmoy   (1000) chinmoy   (1000)        0 2023-04-26 07:13:23.380789 aggdirect_route_estimation_calculator-0.3/
+-rw-rw-r--   0 chinmoy   (1000) chinmoy   (1000)        0 2023-03-10 07:05:23.000000 aggdirect_route_estimation_calculator-0.3/LICENSE
+-rw-rw-r--   0 chinmoy   (1000) chinmoy   (1000)      504 2023-04-26 07:13:23.380789 aggdirect_route_estimation_calculator-0.3/PKG-INFO
+-rw-rw-r--   0 chinmoy   (1000) chinmoy   (1000)     1463 2023-04-25 14:10:26.000000 aggdirect_route_estimation_calculator-0.3/README.md
+drwxrwxr-x   0 chinmoy   (1000) chinmoy   (1000)        0 2023-04-26 07:13:23.376789 aggdirect_route_estimation_calculator-0.3/aggdirect_route_estimation_calculator/
+-rw-rw-r--   0 chinmoy   (1000) chinmoy   (1000)      925 2023-04-26 07:09:17.000000 aggdirect_route_estimation_calculator-0.3/aggdirect_route_estimation_calculator/__init__.py
+drwxrwxr-x   0 chinmoy   (1000) chinmoy   (1000)        0 2023-04-26 07:13:23.380789 aggdirect_route_estimation_calculator-0.3/aggdirect_route_estimation_calculator.egg-info/
+-rw-rw-r--   0 chinmoy   (1000) chinmoy   (1000)      504 2023-04-26 07:13:23.000000 aggdirect_route_estimation_calculator-0.3/aggdirect_route_estimation_calculator.egg-info/PKG-INFO
+-rw-rw-r--   0 chinmoy   (1000) chinmoy   (1000)      380 2023-04-26 07:13:23.000000 aggdirect_route_estimation_calculator-0.3/aggdirect_route_estimation_calculator.egg-info/SOURCES.txt
+-rw-rw-r--   0 chinmoy   (1000) chinmoy   (1000)        1 2023-04-26 07:13:23.000000 aggdirect_route_estimation_calculator-0.3/aggdirect_route_estimation_calculator.egg-info/dependency_links.txt
+-rw-rw-r--   0 chinmoy   (1000) chinmoy   (1000)        9 2023-04-26 07:13:23.000000 aggdirect_route_estimation_calculator-0.3/aggdirect_route_estimation_calculator.egg-info/requires.txt
+-rw-rw-r--   0 chinmoy   (1000) chinmoy   (1000)       38 2023-04-26 07:13:23.000000 aggdirect_route_estimation_calculator-0.3/aggdirect_route_estimation_calculator.egg-info/top_level.txt
+-rw-rw-r--   0 chinmoy   (1000) chinmoy   (1000)       38 2023-04-26 07:13:23.380789 aggdirect_route_estimation_calculator-0.3/setup.cfg
+-rw-rw-r--   0 chinmoy   (1000) chinmoy   (1000)     1074 2023-04-26 07:09:12.000000 aggdirect_route_estimation_calculator-0.3/setup.py
```

### Comparing `aggdirect_route_estimation_calculator-0.2/README.md` & `aggdirect_route_estimation_calculator-0.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -52,15 +52,14 @@
 
 ```python
 cool_obj.estimated_distance(required_unit='m')
 ```
      
         "m" - REturn the distance time in Miles
         "k" - Return the distance time in Kilometer
-        "n" - Reeturn the distance time in Nautical Mile
         "t" - Reeturn the distance time in Meter
 
 
 Example:
     
     Input:
```

### Comparing `aggdirect_route_estimation_calculator-0.2/setup.py` & `aggdirect_route_estimation_calculator-0.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 setup(
     name = 'aggdirect_route_estimation_calculator',         # How you named your package folder (MyLib)
     packages = ['aggdirect_route_estimation_calculator'],
-    version = '0.2',
+    version = '0.3',
     description = 'Route Estimation Calculator functions',
     author = 'Chinmoy Das',
     author_email = '',
     url = '',   # Provide either the link to your github or to your website
     keywords = ['Route Estimation Calculator', 'Route Calculator' , 'AGGDIRECT'],   # Keywords that define your package best
     install_requires=['polyline'],
     classifiers=[
```

