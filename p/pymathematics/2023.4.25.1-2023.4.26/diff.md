# Comparing `tmp/pymathematics-2023.4.25.1.tar.gz` & `tmp/pymathematics-2023.4.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymathematics-2023.4.25.1.tar", last modified: Tue Apr 25 13:56:12 2023, max compression
+gzip compressed data, was "pymathematics-2023.4.26.tar", last modified: Wed Apr 26 15:51:58 2023, max compression
```

## Comparing `pymathematics-2023.4.25.1.tar` & `pymathematics-2023.4.26.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-25 13:56:12.944833 pymathematics-2023.4.25.1/
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)     1088 2023-04-16 06:03:02.000000 pymathematics-2023.4.25.1/LICENSE
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      509 2023-04-25 13:56:12.930831 pymathematics-2023.4.25.1/PKG-INFO
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      152 2023-04-25 13:51:05.000000 pymathematics-2023.4.25.1/README.md
-drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-25 13:56:12.565835 pymathematics-2023.4.25.1/pymathematics/
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)    21998 2023-04-25 13:01:09.000000 pymathematics-2023.4.25.1/pymathematics/__init__.py
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      113 2023-04-25 13:01:18.000000 pymathematics-2023.4.25.1/pymathematics/info.py
-drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-25 13:56:12.869835 pymathematics-2023.4.25.1/pymathematics.egg-info/
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      509 2023-04-25 13:56:11.000000 pymathematics-2023.4.25.1/pymathematics.egg-info/PKG-INFO
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      258 2023-04-25 13:56:11.000000 pymathematics-2023.4.25.1/pymathematics.egg-info/SOURCES.txt
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        1 2023-04-25 13:56:11.000000 pymathematics-2023.4.25.1/pymathematics.egg-info/dependency_links.txt
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        6 2023-04-25 13:56:11.000000 pymathematics-2023.4.25.1/pymathematics.egg-info/requires.txt
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)       14 2023-04-25 13:56:11.000000 pymathematics-2023.4.25.1/pymathematics.egg-info/top_level.txt
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)       38 2023-04-25 13:56:12.949833 pymathematics-2023.4.25.1/setup.cfg
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      698 2023-04-25 13:02:38.000000 pymathematics-2023.4.25.1/setup.py
+drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-26 15:51:58.108329 pymathematics-2023.4.26/
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)     1088 2023-04-16 06:03:02.000000 pymathematics-2023.4.26/LICENSE
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      507 2023-04-26 15:51:58.096332 pymathematics-2023.4.26/PKG-INFO
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      166 2023-04-26 15:45:31.000000 pymathematics-2023.4.26/README.md
+drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-26 15:51:57.575325 pymathematics-2023.4.26/pymathematics/
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)    22129 2023-04-26 15:51:10.000000 pymathematics-2023.4.26/pymathematics/__init__.py
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      111 2023-04-26 15:45:02.000000 pymathematics-2023.4.26/pymathematics/info.py
+drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-26 15:51:57.931333 pymathematics-2023.4.26/pymathematics.egg-info/
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      507 2023-04-26 15:51:50.000000 pymathematics-2023.4.26/pymathematics.egg-info/PKG-INFO
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      258 2023-04-26 15:51:50.000000 pymathematics-2023.4.26/pymathematics.egg-info/SOURCES.txt
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        1 2023-04-26 15:51:50.000000 pymathematics-2023.4.26/pymathematics.egg-info/dependency_links.txt
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        6 2023-04-26 15:51:50.000000 pymathematics-2023.4.26/pymathematics.egg-info/requires.txt
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)       14 2023-04-26 15:51:50.000000 pymathematics-2023.4.26/pymathematics.egg-info/top_level.txt
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)       38 2023-04-26 15:51:58.113329 pymathematics-2023.4.26/setup.cfg
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      696 2023-04-26 15:45:24.000000 pymathematics-2023.4.26/setup.py
```

### Comparing `pymathematics-2023.4.25.1/LICENSE` & `pymathematics-2023.4.26/LICENSE`

 * *Files identical despite different names*

### Comparing `pymathematics-2023.4.25.1/pymathematics/__init__.py` & `pymathematics-2023.4.26/pymathematics/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,16 @@
     author = author
     version = version
     homepage = homepage
 
 class constants:
     pi = 3.1415926535897932384626433832795
     e = 2.7182818284590452353602874713527
-    inf = infinity = float("inf")
-    nan = NaN = float("nan")
+    inf = float("inf")
+    nan = float("nan")
 
 class vector:
     def cross_product(vector1:list,vector2:list) -> int|float:
         if len(vector1) != 3 or len(vector2) != 3:
             raise ValueError("vector should have 3 directions")
         return [vector1[1]*vector2[2]-vector2[1]*vector1[2],-(vector1[0]*vector2[2]-vector2[0]*vector1[2]),vector1[0]*vector2[1]-vector2[0]*vector1[1]]
 
@@ -573,16 +573,22 @@
     xdiff = [x-xmean for x in array1]
     ydiff = [y-ymean for y in array2]
     slope = summation([xdiff[i]*ydiff[i] for i in range(len(array1))])/summation([d**2 for d in xdiff])
     intercept = ymean-slope*xmean
     return [slope,intercept]
 
 def min_max(array):
-    sorted_array = quick_sort(array)
-    return [sorted_array[0],sorted_array[len(sorted_array)-1]]
+    min_val = constants.inf
+    max_val = -constants.inf
+    for x in range(len(array)):
+        if min_val > array[x]:
+            min_val = array[x]
+        if max_val < array[x]:
+            max_val = array[x]
+    return [min_val,max_val]
 
 def mean_sqrd_error(actual:list,predicted:list) -> int|float:
     if len(actual) != len(predicted):
         raise ValueError("length of actual and predicted data aren't equal!")
     errors = [(actual[i]-predicted[i])**2 for i in range(len(actual))]
     return summation(errors)/len(actual)
```

### Comparing `pymathematics-2023.4.25.1/setup.py` & `pymathematics-2023.4.26/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup,find_packages
 
 setup(
     name = "pymathematics",
-    version = "2023.4.25.1",
+    version = "2023.4.26",
     description = "package for mathematics",
     long_description = "for more info, check the github repository",
     author = "Sahil Rajwar",
     maintainer = "its_Sahil",
     author_email = "justsahilrajwar2004@gmail.com",
     packages = ["pymathematics"],
     license = "MIT",
```

