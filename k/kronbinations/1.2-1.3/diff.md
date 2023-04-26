# Comparing `tmp/kronbinations-1.2.tar.gz` & `tmp/kronbinations-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kronbinations-1.2.tar", last modified: Wed Apr 26 14:02:13 2023, max compression
+gzip compressed data, was "kronbinations-1.3.tar", last modified: Wed Apr 26 15:02:14 2023, max compression
```

## Comparing `kronbinations-1.2.tar` & `kronbinations-1.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 14:02:13.541791 kronbinations-1.2/
--rw-rw-rw-   0        0        0     1096 2023-04-26 14:02:09.000000 kronbinations-1.2/LICENSE
--rw-rw-rw-   0        0        0     6252 2023-04-26 14:02:13.541791 kronbinations-1.2/PKG-INFO
--rw-rw-rw-   0        0        0     5724 2023-04-26 14:02:09.000000 kronbinations-1.2/README.md
--rw-rw-rw-   0        0        0      523 2023-04-26 14:02:13.541791 kronbinations-1.2/setup.cfg
--rw-rw-rw-   0        0        0      874 2023-04-26 14:02:09.000000 kronbinations-1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-26 14:02:13.510522 kronbinations-1.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-26 14:02:13.526156 kronbinations-1.2/src/kronbinations/
--rw-rw-rw-   0        0        0     9324 2023-04-17 10:40:53.000000 kronbinations-1.2/src/kronbinations/JIT_Array.py
--rw-rw-rw-   0        0        0    14505 2023-04-26 14:01:14.000000 kronbinations-1.2/src/kronbinations/JIT_kronbinations.py
--rw-rw-rw-   0        0        0     3087 2023-04-17 10:40:45.000000 kronbinations-1.2/src/kronbinations/Kron_Array.py
--rw-rw-rw-   0        0        0    44564 2023-02-24 16:06:05.000000 kronbinations-1.2/src/kronbinations/Kron_Fun_Modifier.py
--rw-rw-rw-   0        0        0      241 2023-02-27 13:26:54.000000 kronbinations-1.2/src/kronbinations/__init__.py
--rw-rw-rw-   0        0        0    10981 2023-04-24 15:10:06.000000 kronbinations-1.2/src/kronbinations/kronbinations.py
-drwxrwxrwx   0        0        0        0 2023-04-26 14:02:13.541791 kronbinations-1.2/src/kronbinations.egg-info/
--rw-rw-rw-   0        0        0     6252 2023-04-26 14:02:13.000000 kronbinations-1.2/src/kronbinations.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      504 2023-04-26 14:02:13.000000 kronbinations-1.2/src/kronbinations.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 14:02:13.000000 kronbinations-1.2/src/kronbinations.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-04-26 14:02:13.000000 kronbinations-1.2/src/kronbinations.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-26 14:02:13.000000 kronbinations-1.2/src/kronbinations.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-26 14:02:13.541791 kronbinations-1.2/test/
--rw-rw-rw-   0        0        0     4862 2023-04-17 15:21:41.000000 kronbinations-1.2/test/test_JIT_kronbinations.py
--rw-rw-rw-   0        0        0     3564 2023-04-17 13:58:07.000000 kronbinations-1.2/test/test_kronbinations.py
+drwxrwxrwx   0        0        0        0 2023-04-26 15:02:14.214005 kronbinations-1.3/
+-rw-rw-rw-   0        0        0     1096 2023-04-26 15:02:07.000000 kronbinations-1.3/LICENSE
+-rw-rw-rw-   0        0        0     6252 2023-04-26 15:02:14.214005 kronbinations-1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5724 2023-04-26 15:02:07.000000 kronbinations-1.3/README.md
+-rw-rw-rw-   0        0        0      523 2023-04-26 15:02:14.229632 kronbinations-1.3/setup.cfg
+-rw-rw-rw-   0        0        0      875 2023-04-26 15:02:07.000000 kronbinations-1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 15:02:14.182758 kronbinations-1.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-26 15:02:14.182758 kronbinations-1.3/src/kronbinations/
+-rw-rw-rw-   0        0        0     9324 2023-04-17 10:40:53.000000 kronbinations-1.3/src/kronbinations/JIT_Array.py
+-rw-rw-rw-   0        0        0    15664 2023-04-26 15:00:27.000000 kronbinations-1.3/src/kronbinations/JIT_kronbinations.py
+-rw-rw-rw-   0        0        0     3087 2023-04-17 10:40:45.000000 kronbinations-1.3/src/kronbinations/Kron_Array.py
+-rw-rw-rw-   0        0        0    44564 2023-02-24 16:06:05.000000 kronbinations-1.3/src/kronbinations/Kron_Fun_Modifier.py
+-rw-rw-rw-   0        0        0      241 2023-02-27 13:26:54.000000 kronbinations-1.3/src/kronbinations/__init__.py
+-rw-rw-rw-   0        0        0    10981 2023-04-24 15:10:06.000000 kronbinations-1.3/src/kronbinations/kronbinations.py
+drwxrwxrwx   0        0        0        0 2023-04-26 15:02:14.214005 kronbinations-1.3/src/kronbinations.egg-info/
+-rw-rw-rw-   0        0        0     6252 2023-04-26 15:02:13.000000 kronbinations-1.3/src/kronbinations.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      504 2023-04-26 15:02:14.000000 kronbinations-1.3/src/kronbinations.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 15:02:13.000000 kronbinations-1.3/src/kronbinations.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-04-26 15:02:13.000000 kronbinations-1.3/src/kronbinations.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-26 15:02:13.000000 kronbinations-1.3/src/kronbinations.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-26 15:02:14.214005 kronbinations-1.3/test/
+-rw-rw-rw-   0        0        0     4862 2023-04-17 15:21:41.000000 kronbinations-1.3/test/test_JIT_kronbinations.py
+-rw-rw-rw-   0        0        0     3564 2023-04-17 13:58:07.000000 kronbinations-1.3/test/test_kronbinations.py
```

### Comparing `kronbinations-1.2/LICENSE` & `kronbinations-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kronbinations-1.2/PKG-INFO` & `kronbinations-1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: kronbinations
-Version: 1.2
+Version: 1.3
 Summary: kronbinations is used to remove nested loops and perform parameter sweeps.
-Home-page: https://github.com/Ntropic/kronbinations/archive/refs/tags/v1.2.tar.gz
+Home-page: https://github.com/Ntropic/kronbinations/archive/refs/tags/v1.3.tar.gz
 Author: Michael Schilling
 Author-email: michael@ntropic.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `kronbinations-1.2/README.md` & `kronbinations-1.3/README.md`

 * *Files identical despite different names*

### Comparing `kronbinations-1.2/setup.cfg` & `kronbinations-1.3/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206b 726f 6e62 696e 6174 696f 6e73   = kronbinations
-00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 320d  ..version = 1.2.
+00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 330d  ..version = 1.3.
 00000030: 0a61 7574 686f 7220 3d20 4d69 6368 6165  .author = Michae
 00000040: 6c20 5363 6869 6c6c 696e 670d 0a61 7574  l Schilling..aut
 00000050: 686f 725f 656d 6169 6c20 3d20 6d69 6368  hor_email = mich
 00000060: 6165 6c40 6e74 726f 7069 632e 6465 0d0a  ael@ntropic.de..
 00000070: 6465 7363 7269 7074 696f 6e20 3d20 6b72  description = kr
 00000080: 6f6e 6269 6e61 7469 6f6e 7320 6973 2075  onbinations is u
 00000090: 7365 6420 746f 2072 656d 6f76 6520 6e65  sed to remove ne
@@ -16,15 +16,15 @@
 000000f0: 6e67 5f64 6573 6372 6970 7469 6f6e 5f63  ng_description_c
 00000100: 6f6e 7465 6e74 5f74 7970 6520 3d20 7465  ontent_type = te
 00000110: 7874 2f6d 6172 6b64 6f77 6e0d 0a75 726c  xt/markdown..url
 00000120: 203d 2068 7474 7073 3a2f 2f67 6974 6875   = https://githu
 00000130: 622e 636f 6d2f 4e74 726f 7069 632f 6b72  b.com/Ntropic/kr
 00000140: 6f6e 6269 6e61 7469 6f6e 732f 6172 6368  onbinations/arch
 00000150: 6976 652f 7265 6673 2f74 6167 732f 7631  ive/refs/tags/v1
-00000160: 2e32 2e74 6172 2e67 7a0d 0a50 726f 6772  .2.tar.gz..Progr
+00000160: 2e33 2e74 6172 2e67 7a0d 0a50 726f 6772  .3.tar.gz..Progr
 00000170: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
 00000180: 3d20 3a20 5079 7468 6f6e 203a 3a20 330d  = : Python :: 3.
 00000190: 0a09 4c69 6365 6e73 6520 3a3a 204f 5349  ..License :: OSI
 000001a0: 2041 7070 726f 7665 6420 3a3a 204d 4954   Approved :: MIT
 000001b0: 204c 6963 656e 7365 0d0a 094f 7065 7261   License...Opera
 000001c0: 7469 6e67 2053 7973 7465 6d20 3a3a 204f  ting System :: O
 000001d0: 5320 496e 6465 7065 6e64 656e 740d 0a0d  S Independent...
```

### Comparing `kronbinations-1.2/setup.py` & `kronbinations-1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "kronbinations",
-    version        = "1.2",
+    version         = "1.3",
     author = "Michael Schilling",
     author_email = "michael@ntropic.de",
     description  = "kronbinations is used to remove nested loops and perform parameter sweeps.",
     long_description = long_description,
     long_description_content_type = "text/markdown",
-    url = "https://github.com/Ntropic/kronbinations/archive/refs/tags/v1.2.tar.gz",
+    url = "https://github.com/Ntropic/kronbinations/archive/refs/tags/v1.3.tar.gz",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
```

### Comparing `kronbinations-1.2/src/kronbinations/JIT_Array.py` & `kronbinations-1.3/src/kronbinations/JIT_Array.py`

 * *Files identical despite different names*

### Comparing `kronbinations-1.2/src/kronbinations/JIT_kronbinations.py` & `kronbinations-1.3/src/kronbinations/JIT_kronbinations.py`

 * *Files 7% similar despite different names*

```diff
@@ -107,16 +107,40 @@
                 key = subs_list[key_list.index(key)]
             x.append(getattr(self, key))
         if len(x) == 1:
             return x[0]
         else:
             return x
 
+    def change_all_dtype(self, object, dtype='int'):
+        # navigates through the objects lists tuples and dictionaries until it finds a numpy array 
+        # and changes the dtype if it is an integer to 'int'
+        if isinstance(object, (list, tuple, dict)):
+            # recursively call the function on the elements of the object
+            is_tuple = isinstance(object, tuple)
+            if is_tuple:
+                object = list(object)
+            if isinstance(object, dict):
+                # navigate every key value pair
+                for key, value in object.items():
+                    object[key] = self.change_all_dtype(value, dtype=dtype)
+            else: # isinstance(object, list):
+                for i in range(len(object)):
+                    object[i] = self.change_all_dtype(object[i], dtype=dtype)
+            if is_tuple:
+                object = tuple(object)
+        elif isinstance(object, np.ndarray):
+            if 'int' in str(object.dtype):
+                object = object.astype(dtype)
+        return object
+    
     def checksum(self, *args):
         # check every arg in args, if arg is an object of a class 
+        # change all dtype int
+        args = self.change_all_dtype(args)
         return sha1(str(args).encode('utf-8')).hexdigest()
 
     def __getitem__(self, key):
         # If the key is not in the data, return None
         if key in key_list:
             key = subs_list[key_list.index(key)]
             print(key)
```

### Comparing `kronbinations-1.2/src/kronbinations/Kron_Array.py` & `kronbinations-1.3/src/kronbinations/Kron_Array.py`

 * *Files identical despite different names*

### Comparing `kronbinations-1.2/src/kronbinations/Kron_Fun_Modifier.py` & `kronbinations-1.3/src/kronbinations/Kron_Fun_Modifier.py`

 * *Files identical despite different names*

### Comparing `kronbinations-1.2/src/kronbinations/kronbinations.py` & `kronbinations-1.3/src/kronbinations/kronbinations.py`

 * *Files identical despite different names*

### Comparing `kronbinations-1.2/src/kronbinations.egg-info/PKG-INFO` & `kronbinations-1.3/src/kronbinations.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: kronbinations
-Version: 1.2
+Version: 1.3
 Summary: kronbinations is used to remove nested loops and perform parameter sweeps.
-Home-page: https://github.com/Ntropic/kronbinations/archive/refs/tags/v1.2.tar.gz
+Home-page: https://github.com/Ntropic/kronbinations/archive/refs/tags/v1.3.tar.gz
 Author: Michael Schilling
 Author-email: michael@ntropic.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `kronbinations-1.2/test/test_JIT_kronbinations.py` & `kronbinations-1.3/test/test_JIT_kronbinations.py`

 * *Files identical despite different names*

### Comparing `kronbinations-1.2/test/test_kronbinations.py` & `kronbinations-1.3/test/test_kronbinations.py`

 * *Files identical despite different names*

