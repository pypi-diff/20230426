# Comparing `tmp/yasiu-math-0.0.3.tar.gz` & `tmp/yasiu-math-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yasiu-math-0.0.3.tar", last modified: Sat Jan 14 21:01:36 2023, max compression
+gzip compressed data, was "P:\LocalPrograms\repos\yasiu\yasiu_math\dist\.tmp-mvcxacge\yasiu-math-0.0.4.tar", last modified: Tue Apr 25 23:32:47 2023, max compression
```

## Comparing `yasiu-math-0.0.3.tar` & `yasiu-math-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-01-14 21:01:36.041225 yasiu-math-0.0.3/
--rw-rw-rw-   0        0        0     1070 2023-01-04 09:51:34.000000 yasiu-math-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     2077 2023-01-14 21:01:36.041225 yasiu-math-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      631 2023-01-14 20:31:06.000000 yasiu-math-0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-01-14 21:01:36.041225 yasiu-math-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     2138 2023-01-14 20:28:31.000000 yasiu-math-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-01-14 21:01:36.037236 yasiu-math-0.0.3/yasiu_math/
--rw-rw-rw-   0        0        0       64 2023-01-14 21:01:14.000000 yasiu-math-0.0.3/yasiu_math/__init__.py
--rw-rw-rw-   0        0        0     4102 2023-01-12 16:25:32.000000 yasiu-math-0.0.3/yasiu_math/math.py
-drwxrwxrwx   0        0        0        0 2023-01-14 21:01:36.040228 yasiu-math-0.0.3/yasiu_math.egg-info/
--rw-rw-rw-   0        0        0     2077 2023-01-14 21:01:36.000000 yasiu-math-0.0.3/yasiu_math.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-01-14 21:01:36.000000 yasiu-math-0.0.3/yasiu_math.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-14 21:01:36.000000 yasiu-math-0.0.3/yasiu_math.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-01-14 21:01:36.000000 yasiu-math-0.0.3/yasiu_math.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-01-14 21:01:36.000000 yasiu-math-0.0.3/yasiu_math.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-25 23:32:47.102923 yasiu-math-0.0.4/
+-rw-rw-rw-   0        0        0     1070 2023-01-04 09:51:34.000000 yasiu-math-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     2077 2023-04-25 23:32:47.101926 yasiu-math-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      631 2023-01-14 20:31:06.000000 yasiu-math-0.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-25 23:32:47.102923 yasiu-math-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     2138 2023-01-14 20:28:31.000000 yasiu-math-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 23:32:47.095942 yasiu-math-0.0.4/tests/
+-rw-rw-rw-   0        0        0     1136 2023-01-12 16:19:30.000000 yasiu-math-0.0.4/tests/test_rounding_number.py
+drwxrwxrwx   0        0        0        0 2023-04-25 23:32:47.096940 yasiu-math-0.0.4/yasiu_math/
+-rw-rw-rw-   0        0        0       64 2023-04-25 23:28:56.000000 yasiu-math-0.0.4/yasiu_math/__init__.py
+-rw-rw-rw-   0        0        0     4340 2023-04-25 23:28:56.000000 yasiu-math-0.0.4/yasiu_math/math.py
+drwxrwxrwx   0        0        0        0 2023-04-25 23:32:47.100929 yasiu-math-0.0.4/yasiu_math.egg-info/
+-rw-rw-rw-   0        0        0     2077 2023-04-25 23:32:47.000000 yasiu-math-0.0.4/yasiu_math.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      267 2023-04-25 23:32:47.000000 yasiu-math-0.0.4/yasiu_math.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 23:32:47.000000 yasiu-math-0.0.4/yasiu_math.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-04-25 23:32:47.000000 yasiu-math-0.0.4/yasiu_math.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-25 23:32:47.000000 yasiu-math-0.0.4/yasiu_math.egg-info/top_level.txt
```

### Comparing `yasiu-math-0.0.3/LICENSE` & `yasiu-math-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `yasiu-math-0.0.3/PKG-INFO` & `yasiu-math-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yasiu-math
-Version: 0.0.3
+Version: 0.0.4
 Summary: Math functions that are missing in numpy / scipy
 Author: Grzegorz Krug
 Author-email: kruggrzegorz@gmail.com
 Maintainer: Grzegorz Krug
 Maintainer-email: kruggrzegorz@gmail.com
 License: MIT
 Project-URL: 1. Native Package, https://pypi.org/project/yasiu-native/
```

### Comparing `yasiu-math-0.0.3/README.md` & `yasiu-math-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `yasiu-math-0.0.3/setup.py` & `yasiu-math-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `yasiu-math-0.0.3/yasiu_math/math.py` & `yasiu-math-0.0.4/yasiu_math/math.py`

 * *Files 11% similar despite different names*

```diff
@@ -55,20 +55,22 @@
         kernel = np.ones(smoothing_frames) / smoothing_frames
 
     elif kernel_type == "linear":
         kernel = np.arange(radius + 1) + 1
         kernel = np.concatenate([kernel[:-1], np.flip(kernel)])
         kernel = kernel / kernel.sum()
 
-    else:
+    elif kernel_type == 'exp':
         "Exponential"
         kernel = np.arange(radius + 1) + 1
         kernel = np.concatenate([kernel[:-1], np.flip(kernel)])
         kernel = kernel ** kernel_exp
         kernel = kernel / kernel.sum()
+    else:
+        raise KeyError(f"Invalid kernel_type{kernel_type}. Use one: exp,linear,avg.")
 
     if padding == "same":
         out = convolve(array, kernel, 'same')
 
     elif padding == "try" or padding == 'keep':
         out = convolve(array, kernel, 'valid')
 
@@ -84,17 +86,19 @@
             # print(len(left), len(out), len(right))
 
         out = np.concatenate([left, out, right])
 
     elif padding == "full":
         out = convolve(array, kernel, 'full')
 
-    else:
+    elif padding == 'valid':
         "valid"
         out = convolve(array, kernel, 'valid')
+    else:
+        raise KeyError(f"Invalid padding key:{padding}. Use one: valid,same,try,keep.")
 
     # posx[:smoothing_frames] = tempx[:smoothing_frames]
     return out
 
 
 def convolve_array_edges(arr, radius):
     """
```

### Comparing `yasiu-math-0.0.3/yasiu_math.egg-info/PKG-INFO` & `yasiu-math-0.0.4/yasiu_math.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yasiu-math
-Version: 0.0.3
+Version: 0.0.4
 Summary: Math functions that are missing in numpy / scipy
 Author: Grzegorz Krug
 Author-email: kruggrzegorz@gmail.com
 Maintainer: Grzegorz Krug
 Maintainer-email: kruggrzegorz@gmail.com
 License: MIT
 Project-URL: 1. Native Package, https://pypi.org/project/yasiu-native/
```

