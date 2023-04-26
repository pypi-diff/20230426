# Comparing `tmp/unipolator-0.2.6.tar.gz` & `tmp/unipolator-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unipolator-0.2.6.tar", last modified: Thu Mar 30 17:36:12 2023, max compression
+gzip compressed data, was "unipolator-0.2.7.tar", last modified: Wed Apr 26 14:13:47 2023, max compression
```

## Comparing `unipolator-0.2.6.tar` & `unipolator-0.2.7.tar`

### file list

```diff
@@ -1,43 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-03-30 17:36:12.636667 unipolator-0.2.6/
--rw-rw-rw-   0        0        0     1096 2023-03-30 17:27:57.000000 unipolator-0.2.6/LICENSE
--rw-rw-rw-   0        0        0       86 2023-03-30 17:27:57.000000 unipolator-0.2.6/MANIFEST.in
--rw-rw-rw-   0        0        0     1795 2023-03-30 17:36:12.637666 unipolator-0.2.6/PKG-INFO
--rw-rw-rw-   0        0        0     1072 2023-03-30 17:27:57.000000 unipolator-0.2.6/README.md
--rw-rw-rw-   0        0        0       30 2023-03-30 17:27:57.000000 unipolator-0.2.6/requirements-dev.txt
--rw-rw-rw-   0        0        0       27 2023-03-30 17:27:57.000000 unipolator-0.2.6/requirements.txt
--rw-rw-rw-   0        0        0      976 2023-03-30 17:36:12.639669 unipolator-0.2.6/setup.cfg
--rw-rw-rw-   0        0        0     3297 2023-03-30 17:35:26.000000 unipolator-0.2.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-30 17:36:12.511539 unipolator-0.2.6/src/
-drwxrwxrwx   0        0        0        0 2023-03-30 17:36:12.613103 unipolator-0.2.6/src/unipolator/
--rw-rw-rw-   0        0        0      408 2023-03-30 16:40:02.000000 unipolator-0.2.6/src/unipolator/__init__.py
--rw-rw-rw-   0        0        0  1031537 2023-03-30 17:35:37.000000 unipolator-0.2.6/src/unipolator/blas_functions.c
--rw-rw-rw-   0        0        0     3446 2023-03-14 14:26:20.000000 unipolator-0.2.6/src/unipolator/blas_functions.pxd
--rw-rw-rw-   0        0        0    12512 2023-03-14 14:26:20.000000 unipolator-0.2.6/src/unipolator/blas_functions.pyx
--rw-rw-rw-   0        0        0  1168547 2023-03-30 17:35:40.000000 unipolator-0.2.6/src/unipolator/caching.c
--rw-rw-rw-   0        0        0      327 2023-03-14 14:26:20.000000 unipolator-0.2.6/src/unipolator/caching.pxd
--rw-rw-rw-   0        0        0    16121 2023-03-14 14:26:20.000000 unipolator-0.2.6/src/unipolator/caching.pyx
--rw-rw-rw-   0        0        0        0 2023-03-13 14:59:20.000000 unipolator-0.2.6/src/unipolator/discrete_quantum.py
--rw-rw-rw-   0        0        0  1116857 2023-03-30 17:35:46.000000 unipolator-0.2.6/src/unipolator/exp_and_log.c
--rw-rw-rw-   0        0        0     4322 2023-03-14 14:26:20.000000 unipolator-0.2.6/src/unipolator/exp_and_log.pxd
--rw-rw-rw-   0        0        0    16417 2023-03-14 14:26:20.000000 unipolator-0.2.6/src/unipolator/exp_and_log.pyx
--rw-rw-rw-   0        0        0  1038842 2023-03-30 17:35:51.000000 unipolator-0.2.6/src/unipolator/hamiltonian_system.c
--rw-rw-rw-   0        0        0    10783 2023-03-14 14:26:20.000000 unipolator-0.2.6/src/unipolator/hamiltonian_system.pyx
--rw-rw-rw-   0        0        0  1174002 2023-03-30 17:35:54.000000 unipolator-0.2.6/src/unipolator/indexing.c
--rw-rw-rw-   0        0        0     1918 2023-03-14 14:26:20.000000 unipolator-0.2.6/src/unipolator/indexing.pxd
--rw-rw-rw-   0        0        0    11597 2023-03-14 14:26:21.000000 unipolator-0.2.6/src/unipolator/indexing.pyx
--rw-rw-rw-   0        0        0   984869 2023-03-30 17:36:00.000000 unipolator-0.2.6/src/unipolator/sym_trotter_system.c
--rw-rw-rw-   0        0        0    13773 2023-03-14 14:26:21.000000 unipolator-0.2.6/src/unipolator/sym_trotter_system.pyx
--rw-rw-rw-   0        0        0  1079140 2023-03-30 17:36:03.000000 unipolator-0.2.6/src/unipolator/symmetric_unitary_interpolation.c
--rw-rw-rw-   0        0        0    11099 2023-03-14 14:26:21.000000 unipolator-0.2.6/src/unipolator/symmetric_unitary_interpolation.pyx
--rw-rw-rw-   0        0        0   974809 2023-03-30 17:36:08.000000 unipolator-0.2.6/src/unipolator/trotter_system.c
--rw-rw-rw-   0        0        0    13677 2023-03-14 14:26:21.000000 unipolator-0.2.6/src/unipolator/trotter_system.pyx
--rw-rw-rw-   0        0        0      260 2023-03-29 19:01:51.000000 unipolator-0.2.6/src/unipolator/unipolator.pyx
--rw-rw-rw-   0        0        0  1175554 2023-03-30 17:36:11.000000 unipolator-0.2.6/src/unipolator/unitary_interpolation.c
--rw-rw-rw-   0        0        0    20997 2023-03-15 20:15:17.000000 unipolator-0.2.6/src/unipolator/unitary_interpolation.pyx
-drwxrwxrwx   0        0        0        0 2023-03-30 17:36:12.636667 unipolator-0.2.6/src/unipolator.egg-info/
--rw-rw-rw-   0        0        0     1795 2023-03-30 17:36:11.000000 unipolator-0.2.6/src/unipolator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1150 2023-03-30 17:36:12.000000 unipolator-0.2.6/src/unipolator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-30 17:36:11.000000 unipolator-0.2.6/src/unipolator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-30 17:36:11.000000 unipolator-0.2.6/src/unipolator.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       86 2023-03-30 17:36:11.000000 unipolator-0.2.6/src/unipolator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-03-30 17:36:11.000000 unipolator-0.2.6/src/unipolator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-26 14:13:47.782727 unipolator-0.2.7/
+-rw-rw-rw-   0        0        0     1096 2023-04-26 14:12:56.000000 unipolator-0.2.7/LICENSE
+-rw-rw-rw-   0        0        0       86 2023-04-26 14:12:56.000000 unipolator-0.2.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     1791 2023-04-26 14:13:47.783726 unipolator-0.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1068 2023-04-26 14:12:56.000000 unipolator-0.2.7/README.md
+-rw-rw-rw-   0        0        0       30 2023-04-26 14:12:56.000000 unipolator-0.2.7/requirements-dev.txt
+-rw-rw-rw-   0        0        0       27 2023-04-26 14:12:56.000000 unipolator-0.2.7/requirements.txt
+-rw-rw-rw-   0        0        0      976 2023-04-26 14:13:47.816600 unipolator-0.2.7/setup.cfg
+-rw-rw-rw-   0        0        0     3298 2023-04-26 14:12:56.000000 unipolator-0.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 14:13:47.346764 unipolator-0.2.7/src/
+drwxrwxrwx   0        0        0        0 2023-04-26 14:13:47.666504 unipolator-0.2.7/src/unipolator/
+-rw-rw-rw-   0        0        0      408 2023-03-30 16:40:02.000000 unipolator-0.2.7/src/unipolator/__init__.py
+-rw-rw-rw-   0        0        0  1031537 2023-04-26 14:13:07.000000 unipolator-0.2.7/src/unipolator/blas_functions.c
+-rw-rw-rw-   0        0        0     3446 2023-03-14 14:26:20.000000 unipolator-0.2.7/src/unipolator/blas_functions.pxd
+-rw-rw-rw-   0        0        0    12512 2023-03-14 14:26:20.000000 unipolator-0.2.7/src/unipolator/blas_functions.pyx
+-rw-rw-rw-   0        0        0  1168547 2023-04-26 14:13:10.000000 unipolator-0.2.7/src/unipolator/caching.c
+-rw-rw-rw-   0        0        0      327 2023-03-14 14:26:20.000000 unipolator-0.2.7/src/unipolator/caching.pxd
+-rw-rw-rw-   0        0        0    16121 2023-03-14 14:26:20.000000 unipolator-0.2.7/src/unipolator/caching.pyx
+-rw-rw-rw-   0        0        0  1116857 2023-04-26 14:13:15.000000 unipolator-0.2.7/src/unipolator/exp_and_log.c
+-rw-rw-rw-   0        0        0     4322 2023-03-14 14:26:20.000000 unipolator-0.2.7/src/unipolator/exp_and_log.pxd
+-rw-rw-rw-   0        0        0    16417 2023-03-14 14:26:20.000000 unipolator-0.2.7/src/unipolator/exp_and_log.pyx
+-rw-rw-rw-   0        0        0  1054030 2023-04-26 14:13:22.000000 unipolator-0.2.7/src/unipolator/hamiltonian_system.c
+-rw-rw-rw-   0        0        0    11198 2023-04-26 14:07:05.000000 unipolator-0.2.7/src/unipolator/hamiltonian_system.pyx
+-rw-rw-rw-   0        0        0  1174002 2023-04-26 14:13:25.000000 unipolator-0.2.7/src/unipolator/indexing.c
+-rw-rw-rw-   0        0        0     1918 2023-03-14 14:26:20.000000 unipolator-0.2.7/src/unipolator/indexing.pxd
+-rw-rw-rw-   0        0        0    11597 2023-03-14 14:26:21.000000 unipolator-0.2.7/src/unipolator/indexing.pyx
+-rw-rw-rw-   0        0        0   996531 2023-04-26 14:13:31.000000 unipolator-0.2.7/src/unipolator/sym_trotter_system.c
+-rw-rw-rw-   0        0        0    13737 2023-04-26 08:32:03.000000 unipolator-0.2.7/src/unipolator/sym_trotter_system.pyx
+-rw-rw-rw-   0        0        0  1087291 2023-04-26 14:13:35.000000 unipolator-0.2.7/src/unipolator/symmetric_unitary_interpolation.c
+-rw-rw-rw-   0        0        0    11305 2023-04-24 12:15:16.000000 unipolator-0.2.7/src/unipolator/symmetric_unitary_interpolation.pyx
+-rw-rw-rw-   0        0        0   986270 2023-04-26 14:13:41.000000 unipolator-0.2.7/src/unipolator/trotter_system.c
+-rw-rw-rw-   0        0        0    13643 2023-04-24 12:19:37.000000 unipolator-0.2.7/src/unipolator/trotter_system.pyx
+-rw-rw-rw-   0        0        0      220 2023-04-24 11:56:46.000000 unipolator-0.2.7/src/unipolator/unipolator.pyx
+-rw-rw-rw-   0        0        0  1186825 2023-04-26 14:13:44.000000 unipolator-0.2.7/src/unipolator/unitary_interpolation.c
+-rw-rw-rw-   0        0        0    21275 2023-04-24 12:14:55.000000 unipolator-0.2.7/src/unipolator/unitary_interpolation.pyx
+drwxrwxrwx   0        0        0        0 2023-04-26 14:13:47.779708 unipolator-0.2.7/src/unipolator.egg-info/
+-rw-rw-rw-   0        0        0     1791 2023-04-26 14:13:45.000000 unipolator-0.2.7/src/unipolator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1115 2023-04-26 14:13:46.000000 unipolator-0.2.7/src/unipolator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 14:13:45.000000 unipolator-0.2.7/src/unipolator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-26 14:13:45.000000 unipolator-0.2.7/src/unipolator.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       86 2023-04-26 14:13:45.000000 unipolator-0.2.7/src/unipolator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-26 14:13:45.000000 unipolator-0.2.7/src/unipolator.egg-info/top_level.txt
```

### Comparing `unipolator-0.2.6/LICENSE` & `unipolator-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `unipolator-0.2.6/PKG-INFO` & `unipolator-0.2.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: unipolator
-Version: 0.2.6
+Version: 0.2.7
 Summary: Unipolator allows for n dimensional unitary interpolation, and the calculation of propagators using unitary interpolation. Speeds up your propagators for linear quantum systems.
 Home-page: https://github.com/Ntropic/unipolator
-Download-URL: https://github.com/Ntropic/unipolator/archive/refs/tags/v0.2.6.tar.gz
+Download-URL: https://github.com/Ntropic/unipolator/archive/refs/tags/v0.2.7.tar.gz
 Author: Michael Schilling
 Author-email: michael@ntropic.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
@@ -44,10 +44,9 @@
 ui.expmH_pulse(cs, U)
 ``` 
 Finally the GRAPE method is supported via (pass an array `dI_dj.shape(n, cs.shape[0])` to store the gradients)
 ```
 ui.grape(cs, U_target, target_indexes, U, dU, dI_dj)
 ```
 
-
- ## Author: 
- Michael Schilling
+## Author: 
+Michael Schilling
```

### Comparing `unipolator-0.2.6/README.md` & `unipolator-0.2.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -27,10 +27,9 @@
 ui.expmH_pulse(cs, U)
 ``` 
 Finally the GRAPE method is supported via (pass an array `dI_dj.shape(n, cs.shape[0])` to store the gradients)
 ```
 ui.grape(cs, U_target, target_indexes, U, dU, dI_dj)
 ```
 
-
- ## Author: 
- Michael Schilling
+## Author: 
+Michael Schilling
```

### Comparing `unipolator-0.2.6/setup.cfg` & `unipolator-0.2.7/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2075 6e69 706f 6c61 746f 720d 0a76   = unipolator..v
-00000020: 6572 7369 6f6e 203d 2030 2e32 2e36 0d0a  ersion = 0.2.6..
+00000020: 6572 7369 6f6e 203d 2030 2e32 2e37 0d0a  ersion = 0.2.7..
 00000030: 6175 7468 6f72 203d 204d 6963 6861 656c  author = Michael
 00000040: 2053 6368 696c 6c69 6e67 0d0a 6175 7468   Schilling..auth
 00000050: 6f72 5f65 6d61 696c 203d 206d 6963 6861  or_email = micha
 00000060: 656c 406e 7472 6f70 6963 2e64 650d 0a64  el@ntropic.de..d
 00000070: 6573 6372 6970 7469 6f6e 203d 2055 6e69  escription = Uni
 00000080: 706f 6c61 746f 7220 616c 6c6f 7773 2066  polator allows f
 00000090: 6f72 206e 2064 696d 656e 7369 6f6e 616c  or n dimensional
@@ -25,15 +25,15 @@
 00000180: 6e0d 0a75 726c 203d 2068 7474 7073 3a2f  n..url = https:/
 00000190: 2f67 6974 6875 622e 636f 6d2f 4e74 726f  /github.com/Ntro
 000001a0: 7069 632f 756e 6970 6f6c 6174 6f72 0d0a  pic/unipolator..
 000001b0: 646f 776e 6c6f 6164 5f75 726c 203d 2068  download_url = h
 000001c0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
 000001d0: 6d2f 4e74 726f 7069 632f 756e 6970 6f6c  m/Ntropic/unipol
 000001e0: 6174 6f72 2f61 7263 6869 7665 2f72 6566  ator/archive/ref
-000001f0: 732f 7461 6773 2f76 302e 322e 362e 7461  s/tags/v0.2.6.ta
+000001f0: 732f 7461 6773 2f76 302e 322e 372e 7461  s/tags/v0.2.7.ta
 00000200: 722e 677a 0d0a 5072 6f67 7261 6d6d 696e  r.gz..Programmin
 00000210: 6720 4c61 6e67 7561 6765 203d 203a 2050  g Language = : P
 00000220: 7974 686f 6e20 3a3a 2033 0d0a 0950 726f  ython :: 3...Pro
 00000230: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
 00000240: 6520 3a3a 2050 7974 686f 6e20 3a3a 2049  e :: Python :: I
 00000250: 6d70 6c65 6d65 6e74 6174 696f 6e20 3a3a  mplementation ::
 00000260: 2043 5079 7468 6f6e 0d0a 0949 6e74 656e   CPython...Inten
```

### Comparing `unipolator-0.2.6/setup.py` & `unipolator-0.2.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,22 +52,22 @@
 
 with open("requirements-dev.txt") as fp:
     dev_requires = fp.read().strip().split("\n")
 
 setup(   
     name = "unipolator",
     #zip_safe = False,
-    version         = "0.2.6",
+    version          = "0.2.7",
     author = "Michael Schilling",
     author_email = "michael@ntropic.de",
     description  = "Unipolator allows for n dimensional unitary interpolation, and the calculation of propagators using unitary interpolation. Speeds up your propagators for linear quantum systems.",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/Ntropic/unipolator",
-    download_url = "https://github.com/Ntropic/unipolator/archive/refs/tags/v0.2.6.tar.gz",
+    download_url = "https://github.com/Ntropic/unipolator/archive/refs/tags/v0.2.7.tar.gz",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     ext_modules = extensions,
     install_requires = install_requires,
```

### Comparing `unipolator-0.2.6/src/unipolator/blas_functions.c` & `unipolator-0.2.7/src/unipolator/blas_functions.c`

 * *Files identical despite different names*

### Comparing `unipolator-0.2.6/src/unipolator/blas_functions.pxd` & `unipolator-0.2.7/src/unipolator/blas_functions.pxd`

 * *Files identical despite different names*

### Comparing `unipolator-0.2.6/src/unipolator/blas_functions.pyx` & `unipolator-0.2.7/src/unipolator/blas_functions.pyx`

 * *Files identical despite different names*

### Comparing `unipolator-0.2.6/src/unipolator/caching.c` & `unipolator-0.2.7/src/unipolator/caching.c`

 * *Files identical despite different names*

### Comparing `unipolator-0.2.6/src/unipolator/caching.pyx` & `unipolator-0.2.7/src/unipolator/caching.pyx`

 * *Files identical despite different names*

### Comparing `unipolator-0.2.6/src/unipolator/exp_and_log.c` & `unipolator-0.2.7/src/unipolator/exp_and_log.c`

 * *Files identical despite different names*

### Comparing `unipolator-0.2.6/src/unipolator/exp_and_log.pxd` & `unipolator-0.2.7/src/unipolator/exp_and_log.pxd`

 * *Files identical despite different names*

### Comparing `unipolator-0.2.6/src/unipolator/exp_and_log.pyx` & `unipolator-0.2.7/src/unipolator/exp_and_log.pyx`

 * *Files identical despite different names*

### Comparing `unipolator-0.2.6/src/unipolator/hamiltonian_system.c` & `unipolator-0.2.7/src/unipolator/hamiltonian_system.c`

 * *Files 0% similar despite different names*

```diff
@@ -1480,27 +1480,27 @@
  * 
  * cdef void cbbcsd(char *jobu1, char *jobu2, char *jobv1t, char *jobv2t, char *trans, int *m, int *p, int *q, s *theta, s *phi, c *u1, int *ldu1, c *u2, int *ldu2, c *v1t, int *ldv1t, c *v2t, int *ldv2t, s *b11d, s *b11e, s *b12d, s *b12e, s *b21d, s *b21e, s *b22d, s *b22e, s *rwork, int *lrwork, int *info) nogil
  */
 typedef int __pyx_t_5scipy_6linalg_13cython_lapack_zselect2(__pyx_t_double_complex *, __pyx_t_double_complex *);
 struct __pyx_opt_args_10unipolator_18hamiltonian_system_18Hamiltonian_System_dexpmH_pointer;
 struct __pyx_opt_args_10unipolator_18hamiltonian_system_18Hamiltonian_System_expmH_pulse_pointer;
 
-/* "unipolator/hamiltonian_system.pyx":112
- *         DagM_M_cdot_pointer(self.v0, self.u1, u0, self.d)
+/* "unipolator/hamiltonian_system.pyx":122
+ *             u0 += self.d2
  * 
  *     cdef dexpmH_pointer(self, double[::1] c, double complex *u0, double complex *du0, dt=1.0):  #int[::1] d_di,             # <<<<<<<<<<<<<<
  *         # Construct Hamiltonian
  *         cdef int i
  */
 struct __pyx_opt_args_10unipolator_18hamiltonian_system_18Hamiltonian_System_dexpmH_pointer {
   int __pyx_n;
   PyObject *dt;
 };
 
-/* "unipolator/hamiltonian_system.pyx":145
+/* "unipolator/hamiltonian_system.pyx":155
  *         self.dexpmH_pointer(c, u0, du0, dt)
  * 
  *     cdef expmH_pulse_pointer(self, double[:,::1] cs, double complex *u0, double dt=1.0):             # <<<<<<<<<<<<<<
  *         cdef int i
  *         cdef int steps = cs.shape[0]
  */
 struct __pyx_opt_args_10unipolator_18hamiltonian_system_18Hamiltonian_System_expmH_pulse_pointer {
@@ -1643,14 +1643,15 @@
  * cdef class Hamiltonian_System:             # <<<<<<<<<<<<<<
  *     # Initialize variables, to quickly calculate interpolations while minimizing memmory allocation overheads
  *     cdef int n_dims, n_dims_1, d, d2, n_d_di_1, n_d_di,
  */
 
 struct __pyx_vtabstruct_10unipolator_18hamiltonian_system_Hamiltonian_System {
   PyObject *(*weighted_hamiltonian)(struct __pyx_obj_10unipolator_18hamiltonian_system_Hamiltonian_System *, __Pyx_memviewslice);
+  PyObject *(*expmH_pointer)(struct __pyx_obj_10unipolator_18hamiltonian_system_Hamiltonian_System *, __Pyx_memviewslice, __pyx_t_double_complex *, double);
   PyObject *(*dexpmH_pointer)(struct __pyx_obj_10unipolator_18hamiltonian_system_Hamiltonian_System *, __Pyx_memviewslice, __pyx_t_double_complex *, __pyx_t_double_complex *, struct __pyx_opt_args_10unipolator_18hamiltonian_system_18Hamiltonian_System_dexpmH_pointer *__pyx_optional_args);
   PyObject *(*expmH_pulse_pointer)(struct __pyx_obj_10unipolator_18hamiltonian_system_Hamiltonian_System *, __Pyx_memviewslice, __pyx_t_double_complex *, struct __pyx_opt_args_10unipolator_18hamiltonian_system_18Hamiltonian_System_expmH_pulse_pointer *__pyx_optional_args);
 };
 static struct __pyx_vtabstruct_10unipolator_18hamiltonian_system_Hamiltonian_System *__pyx_vtabptr_10unipolator_18hamiltonian_system_Hamiltonian_System;
 
 
 /* "View.MemoryView":106
@@ -2449,14 +2450,15 @@
 /* FunctionImport.proto */
 static int __Pyx_ImportFunction(PyObject *module, const char *funcname, void (**f)(void), const char *sig);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
 static PyObject *__pyx_f_10unipolator_18hamiltonian_system_18Hamiltonian_System_weighted_hamiltonian(struct __pyx_obj_10unipolator_18hamiltonian_system_Hamiltonian_System *__pyx_v_self, __Pyx_memviewslice __pyx_v_c); /* proto*/
+static PyObject *__pyx_f_10unipolator_18hamiltonian_system_18Hamiltonian_System_expmH_pointer(struct __pyx_obj_10unipolator_18hamiltonian_system_Hamiltonian_System *__pyx_v_self, __Pyx_memviewslice __pyx_v_c, __pyx_t_double_complex *__pyx_v_u0, double __pyx_v_dt); /* proto*/
 static PyObject *__pyx_f_10unipolator_18hamiltonian_system_18Hamiltonian_System_dexpmH_pointer(struct __pyx_obj_10unipolator_18hamiltonian_system_Hamiltonian_System *__pyx_v_self, __Pyx_memviewslice __pyx_v_c, __pyx_t_double_complex *__pyx_v_u0, __pyx_t_double_complex *__pyx_v_du0, struct __pyx_opt_args_10unipolator_18hamiltonian_system_18Hamiltonian_System_dexpmH_pointer *__pyx_optional_args); /* proto*/
 static PyObject *__pyx_f_10unipolator_18hamiltonian_system_18Hamiltonian_System_expmH_pulse_pointer(struct __pyx_obj_10unipolator_18hamiltonian_system_Hamiltonian_System *__pyx_v_self, __Pyx_memviewslice __pyx_v_cs, __pyx_t_double_complex *__pyx_v_u0, struct __pyx_opt_args_10unipolator_18hamiltonian_system_18Hamiltonian_System_expmH_pulse_pointer *__pyx_optional_args); /* proto*/
 static PyObject *__pyx_array_get_memview(struct __pyx_array_obj *__pyx_v_self); /* proto*/
 static char *__pyx_memoryview_get_item_pointer(struct __pyx_memoryview_obj *__pyx_v_self, PyObject *__pyx_v_index); /* proto*/
 static PyObject *__pyx_memoryview_is_slice(struct __pyx_memoryview_obj *__pyx_v_self, PyObject *__pyx_v_obj); /* proto*/
 static PyObject *__pyx_memoryview_setitem_slice_assignment(struct __pyx_memoryview_obj *__pyx_v_self, PyObject *__pyx_v_dst, PyObject *__pyx_v_src); /* proto*/
 static PyObject *__pyx_memoryview_setitem_slice_assign_scalar(struct __pyx_memoryview_obj *__pyx_v_self, struct __pyx_memoryview_obj *__pyx_v_dst, PyObject *__pyx_v_value); /* proto*/
@@ -2821,19 +2823,20 @@
 static PyObject *__pyx_n_s_unpack;
 static PyObject *__pyx_n_s_update;
 static PyObject *__pyx_n_s_which_diffs;
 static int __pyx_pf_10unipolator_18hamiltonian_system_18Hamiltonian_System___cinit__(struct __pyx_obj_10unipolator_18hamiltonian_system_Hamiltonian_System *__pyx_v_self, __Pyx_memviewslice __pyx_v_H_s, __Pyx_memviewslice __pyx_v_which_diffs); /* proto */
 static PyObject *__pyx_pf_10unipolator_18hamiltonian_system_18Hamiltonian_System_2set_which_diffs(struct __pyx_obj_10unipolator_18hamiltonian_system_Hamiltonian_System *__pyx_v_self, __Pyx_memviewslice __pyx_v_which_diffs); /* proto */
 static PyObject *__pyx_pf_10unipolator_18hamiltonian_system_18Hamiltonian_System_4get_which_diffs(struct __pyx_obj_10unipolator_18hamiltonian_system_Hamiltonian_System *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_10unipolator_18hamiltonian_system_18Hamiltonian_System_6expmH(struct __pyx_obj_10unipolator_18hamiltonian_system_Hamiltonian_System *__pyx_v_self, __Pyx_memviewslice __pyx_v_c, __Pyx_memviewslice __pyx_v_U, double __pyx_v_dt); /* proto */
-static PyObject *__pyx_pf_10unipolator_18hamiltonian_system_18Hamiltonian_System_8dexpmH(struct __pyx_obj_10unipolator_18hamiltonian_system_Hamiltonian_System *__pyx_v_self, __Pyx_memviewslice __pyx_v_c, __Pyx_memviewslice __pyx_v_U, __Pyx_memviewslice __pyx_v_dU, double __pyx_v_dt); /* proto */
-static PyObject *__pyx_pf_10unipolator_18hamiltonian_system_18Hamiltonian_System_10expmH_pulse(struct __pyx_obj_10unipolator_18hamiltonian_system_Hamiltonian_System *__pyx_v_self, __Pyx_memviewslice __pyx_v_cs, __Pyx_memviewslice __pyx_v_U, double __pyx_v_dt); /* proto */
-static PyObject *__pyx_pf_10unipolator_18hamiltonian_system_18Hamiltonian_System_12grape(struct __pyx_obj_10unipolator_18hamiltonian_system_Hamiltonian_System *__pyx_v_self, __Pyx_memviewslice __pyx_v_cs, __Pyx_memviewslice __pyx_v_U_target, __Pyx_memviewslice __pyx_v_target_indexes, __Pyx_memviewslice __pyx_v_U, __Pyx_memviewslice __pyx_v_dU, __Pyx_memviewslice __pyx_v_dI_dj); /* proto */
-static PyObject *__pyx_pf_10unipolator_18hamiltonian_system_18Hamiltonian_System_14__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_10unipolator_18hamiltonian_system_Hamiltonian_System *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_10unipolator_18hamiltonian_system_18Hamiltonian_System_16__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_10unipolator_18hamiltonian_system_Hamiltonian_System *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
+static PyObject *__pyx_pf_10unipolator_18hamiltonian_system_18Hamiltonian_System_8expmH_pulse_no_multiply(struct __pyx_obj_10unipolator_18hamiltonian_system_Hamiltonian_System *__pyx_v_self, __Pyx_memviewslice __pyx_v_cs, __Pyx_memviewslice __pyx_v_U, double __pyx_v_dt); /* proto */
+static PyObject *__pyx_pf_10unipolator_18hamiltonian_system_18Hamiltonian_System_10dexpmH(struct __pyx_obj_10unipolator_18hamiltonian_system_Hamiltonian_System *__pyx_v_self, __Pyx_memviewslice __pyx_v_c, __Pyx_memviewslice __pyx_v_U, __Pyx_memviewslice __pyx_v_dU, double __pyx_v_dt); /* proto */
+static PyObject *__pyx_pf_10unipolator_18hamiltonian_system_18Hamiltonian_System_12expmH_pulse(struct __pyx_obj_10unipolator_18hamiltonian_system_Hamiltonian_System *__pyx_v_self, __Pyx_memviewslice __pyx_v_cs, __Pyx_memviewslice __pyx_v_U, double __pyx_v_dt); /* proto */
+static PyObject *__pyx_pf_10unipolator_18hamiltonian_system_18Hamiltonian_System_14grape(struct __pyx_obj_10unipolator_18hamiltonian_system_Hamiltonian_System *__pyx_v_self, __Pyx_memviewslice __pyx_v_cs, __Pyx_memviewslice __pyx_v_U_target, __Pyx_memviewslice __pyx_v_target_indexes, __Pyx_memviewslice __pyx_v_U, __Pyx_memviewslice __pyx_v_dU, __Pyx_memviewslice __pyx_v_dI_dj); /* proto */
+static PyObject *__pyx_pf_10unipolator_18hamiltonian_system_18Hamiltonian_System_16__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_10unipolator_18hamiltonian_system_Hamiltonian_System *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_10unipolator_18hamiltonian_system_18Hamiltonian_System_18__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_10unipolator_18hamiltonian_system_Hamiltonian_System *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
 static int __pyx_array___pyx_pf_15View_dot_MemoryView_5array___cinit__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_shape, Py_ssize_t __pyx_v_itemsize, PyObject *__pyx_v_format, PyObject *__pyx_v_mode, int __pyx_v_allocate_buffer); /* proto */
 static int __pyx_array___pyx_pf_15View_dot_MemoryView_5array_2__getbuffer__(struct __pyx_array_obj *__pyx_v_self, Py_buffer *__pyx_v_info, int __pyx_v_flags); /* proto */
 static void __pyx_array___pyx_pf_15View_dot_MemoryView_5array_4__dealloc__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_15View_dot_MemoryView_5array_7memview___get__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static Py_ssize_t __pyx_array___pyx_pf_15View_dot_MemoryView_5array_6__len__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_array___pyx_pf_15View_dot_MemoryView_5array_8__getattr__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_attr); /* proto */
 static PyObject *__pyx_array___pyx_pf_15View_dot_MemoryView_5array_10__getitem__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_item); /* proto */
@@ -4208,15 +4211,15 @@
     __pyx_v_self->curr_h0 = (__pyx_v_self->curr_h0 + __pyx_v_self->d2);
 
     /* "unipolator/hamiltonian_system.pyx":99
  *         for i in range(self.n_dims_1):
  *             self.curr_h0 += self.d2
  *             d_mat_add_pointer(self.v0, self.curr_h0, c[i], self.d2)             # <<<<<<<<<<<<<<
  * 
- *     def expmH(self, double[::1] c, double complex[:,::1] U, double dt=1.0):
+ *     cdef expmH_pointer(self, double[::1] c, double complex *u0, double dt):
  */
     __pyx_t_5 = __pyx_v_i;
     __pyx_f_10unipolator_14blas_functions_d_mat_add_pointer(__pyx_v_self->v0, __pyx_v_self->curr_h0, (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_c.data) + __pyx_t_5)) ))), __pyx_v_self->d2);
   }
 
   /* "unipolator/hamiltonian_system.pyx":94
  *         return np.asarray(self.d_di), self.n_d_di
@@ -4232,14 +4235,99 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "unipolator/hamiltonian_system.pyx":101
  *             d_mat_add_pointer(self.v0, self.curr_h0, c[i], self.d2)
  * 
+ *     cdef expmH_pointer(self, double[::1] c, double complex *u0, double dt):             # <<<<<<<<<<<<<<
+ *         self.weighted_hamiltonian(c)
+ *         zheevd(self.jobz, self.uplo, &self.d, self.v0, &self.d, self.e0, self.work0, &self.lwork, self.rwork0, &self.lrwork, self.iwork0, &self.liwork, &self.info)
+ */
+
+static PyObject *__pyx_f_10unipolator_18hamiltonian_system_18Hamiltonian_System_expmH_pointer(struct __pyx_obj_10unipolator_18hamiltonian_system_Hamiltonian_System *__pyx_v_self, __Pyx_memviewslice __pyx_v_c, __pyx_t_double_complex *__pyx_v_u0, double __pyx_v_dt) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("expmH_pointer", 0);
+
+  /* "unipolator/hamiltonian_system.pyx":102
+ * 
+ *     cdef expmH_pointer(self, double[::1] c, double complex *u0, double dt):
+ *         self.weighted_hamiltonian(c)             # <<<<<<<<<<<<<<
+ *         zheevd(self.jobz, self.uplo, &self.d, self.v0, &self.d, self.e0, self.work0, &self.lwork, self.rwork0, &self.lrwork, self.iwork0, &self.liwork, &self.info)
+ *         copy_pointer(self.v0, self.u1, self.d2)
+ */
+  __pyx_t_1 = ((struct __pyx_vtabstruct_10unipolator_18hamiltonian_system_Hamiltonian_System *)__pyx_v_self->__pyx_vtab)->weighted_hamiltonian(__pyx_v_self, __pyx_v_c); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 102, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+  /* "unipolator/hamiltonian_system.pyx":103
+ *     cdef expmH_pointer(self, double[::1] c, double complex *u0, double dt):
+ *         self.weighted_hamiltonian(c)
+ *         zheevd(self.jobz, self.uplo, &self.d, self.v0, &self.d, self.e0, self.work0, &self.lwork, self.rwork0, &self.lrwork, self.iwork0, &self.liwork, &self.info)             # <<<<<<<<<<<<<<
+ *         copy_pointer(self.v0, self.u1, self.d2)
+ *         v_exp_pointer(self.e0, self.u1, dt, self.d)
+ */
+  __pyx_f_5scipy_6linalg_13cython_lapack_zheevd(__pyx_v_self->jobz, __pyx_v_self->uplo, (&__pyx_v_self->d), __pyx_v_self->v0, (&__pyx_v_self->d), __pyx_v_self->e0, __pyx_v_self->work0, (&__pyx_v_self->lwork), __pyx_v_self->rwork0, (&__pyx_v_self->lrwork), __pyx_v_self->iwork0, (&__pyx_v_self->liwork), (&__pyx_v_self->info));
+
+  /* "unipolator/hamiltonian_system.pyx":104
+ *         self.weighted_hamiltonian(c)
+ *         zheevd(self.jobz, self.uplo, &self.d, self.v0, &self.d, self.e0, self.work0, &self.lwork, self.rwork0, &self.lrwork, self.iwork0, &self.liwork, &self.info)
+ *         copy_pointer(self.v0, self.u1, self.d2)             # <<<<<<<<<<<<<<
+ *         v_exp_pointer(self.e0, self.u1, dt, self.d)
+ *         DagM_M_cdot_pointer(self.v0, self.u1, u0, self.d)
+ */
+  __pyx_f_10unipolator_11exp_and_log_copy_pointer(__pyx_v_self->v0, __pyx_v_self->u1, __pyx_v_self->d2);
+
+  /* "unipolator/hamiltonian_system.pyx":105
+ *         zheevd(self.jobz, self.uplo, &self.d, self.v0, &self.d, self.e0, self.work0, &self.lwork, self.rwork0, &self.lrwork, self.iwork0, &self.liwork, &self.info)
+ *         copy_pointer(self.v0, self.u1, self.d2)
+ *         v_exp_pointer(self.e0, self.u1, dt, self.d)             # <<<<<<<<<<<<<<
+ *         DagM_M_cdot_pointer(self.v0, self.u1, u0, self.d)
+ * 
+ */
+  __pyx_f_10unipolator_11exp_and_log_v_exp_pointer(__pyx_v_self->e0, __pyx_v_self->u1, __pyx_v_dt, __pyx_v_self->d);
+
+  /* "unipolator/hamiltonian_system.pyx":106
+ *         copy_pointer(self.v0, self.u1, self.d2)
+ *         v_exp_pointer(self.e0, self.u1, dt, self.d)
+ *         DagM_M_cdot_pointer(self.v0, self.u1, u0, self.d)             # <<<<<<<<<<<<<<
+ * 
+ *     def expmH(self, double[::1] c, double complex[:,::1] U, double dt=1.0):
+ */
+  __pyx_f_10unipolator_14blas_functions_DagM_M_cdot_pointer(__pyx_v_self->v0, __pyx_v_self->u1, __pyx_v_u0, __pyx_v_self->d);
+
+  /* "unipolator/hamiltonian_system.pyx":101
+ *             d_mat_add_pointer(self.v0, self.curr_h0, c[i], self.d2)
+ * 
+ *     cdef expmH_pointer(self, double[::1] c, double complex *u0, double dt):             # <<<<<<<<<<<<<<
+ *         self.weighted_hamiltonian(c)
+ *         zheevd(self.jobz, self.uplo, &self.d, self.v0, &self.d, self.e0, self.work0, &self.lwork, self.rwork0, &self.lrwork, self.iwork0, &self.liwork, &self.info)
+ */
+
+  /* function exit code */
+  __pyx_r = Py_None; __Pyx_INCREF(Py_None);
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("unipolator.hamiltonian_system.Hamiltonian_System.expmH_pointer", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "unipolator/hamiltonian_system.pyx":108
+ *         DagM_M_cdot_pointer(self.v0, self.u1, u0, self.d)
+ * 
  *     def expmH(self, double[::1] c, double complex[:,::1] U, double dt=1.0):             # <<<<<<<<<<<<<<
  *         # Construct Hamiltonian
  *         if not c.shape[0] == self.n_dims_1:
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_10unipolator_18hamiltonian_system_18Hamiltonian_System_7expmH(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
@@ -4275,47 +4363,47 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_c)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_U)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("expmH", 0, 2, 3, 1); __PYX_ERR(0, 101, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("expmH", 0, 2, 3, 1); __PYX_ERR(0, 108, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_dt);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "expmH") < 0)) __PYX_ERR(0, 101, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "expmH") < 0)) __PYX_ERR(0, 108, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
-    __pyx_v_c = __Pyx_PyObject_to_MemoryviewSlice_dc_double(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_c.memview)) __PYX_ERR(0, 101, __pyx_L3_error)
-    __pyx_v_U = __Pyx_PyObject_to_MemoryviewSlice_d_dc___pyx_t_double_complex(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_U.memview)) __PYX_ERR(0, 101, __pyx_L3_error)
+    __pyx_v_c = __Pyx_PyObject_to_MemoryviewSlice_dc_double(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_c.memview)) __PYX_ERR(0, 108, __pyx_L3_error)
+    __pyx_v_U = __Pyx_PyObject_to_MemoryviewSlice_d_dc___pyx_t_double_complex(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_U.memview)) __PYX_ERR(0, 108, __pyx_L3_error)
     if (values[2]) {
-      __pyx_v_dt = __pyx_PyFloat_AsDouble(values[2]); if (unlikely((__pyx_v_dt == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 101, __pyx_L3_error)
+      __pyx_v_dt = __pyx_PyFloat_AsDouble(values[2]); if (unlikely((__pyx_v_dt == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 108, __pyx_L3_error)
     } else {
       __pyx_v_dt = ((double)1.0);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("expmH", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 101, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("expmH", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 108, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("unipolator.hamiltonian_system.Hamiltonian_System.expmH", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_10unipolator_18hamiltonian_system_18Hamiltonian_System_6expmH(((struct __pyx_obj_10unipolator_18hamiltonian_system_Hamiltonian_System *)__pyx_v_self), __pyx_v_c, __pyx_v_U, __pyx_v_dt);
 
@@ -4333,129 +4421,354 @@
   Py_ssize_t __pyx_t_3;
   Py_ssize_t __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("expmH", 0);
 
-  /* "unipolator/hamiltonian_system.pyx":103
+  /* "unipolator/hamiltonian_system.pyx":110
  *     def expmH(self, double[::1] c, double complex[:,::1] U, double dt=1.0):
  *         # Construct Hamiltonian
  *         if not c.shape[0] == self.n_dims_1:             # <<<<<<<<<<<<<<
  *             raise ValueError('c.shape[0] needs to be equal to H_s[0].shape[0]-1.')
  *         cdef double complex *u0 = &U[0,0]
  */
   __pyx_t_1 = ((!(((__pyx_v_c.shape[0]) == __pyx_v_self->n_dims_1) != 0)) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "unipolator/hamiltonian_system.pyx":104
+    /* "unipolator/hamiltonian_system.pyx":111
  *         # Construct Hamiltonian
  *         if not c.shape[0] == self.n_dims_1:
  *             raise ValueError('c.shape[0] needs to be equal to H_s[0].shape[0]-1.')             # <<<<<<<<<<<<<<
  *         cdef double complex *u0 = &U[0,0]
- *         self.weighted_hamiltonian(c)
+ *         self.expmH_pointer(c, u0, dt)
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 104, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 111, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 104, __pyx_L1_error)
+    __PYX_ERR(0, 111, __pyx_L1_error)
 
-    /* "unipolator/hamiltonian_system.pyx":103
+    /* "unipolator/hamiltonian_system.pyx":110
  *     def expmH(self, double[::1] c, double complex[:,::1] U, double dt=1.0):
  *         # Construct Hamiltonian
  *         if not c.shape[0] == self.n_dims_1:             # <<<<<<<<<<<<<<
  *             raise ValueError('c.shape[0] needs to be equal to H_s[0].shape[0]-1.')
  *         cdef double complex *u0 = &U[0,0]
  */
   }
 
-  /* "unipolator/hamiltonian_system.pyx":105
+  /* "unipolator/hamiltonian_system.pyx":112
  *         if not c.shape[0] == self.n_dims_1:
  *             raise ValueError('c.shape[0] needs to be equal to H_s[0].shape[0]-1.')
  *         cdef double complex *u0 = &U[0,0]             # <<<<<<<<<<<<<<
- *         self.weighted_hamiltonian(c)
- *         zheevd(self.jobz, self.uplo, &self.d, self.v0, &self.d, self.e0, self.work0, &self.lwork, self.rwork0, &self.lrwork, self.iwork0, &self.liwork, &self.info)
+ *         self.expmH_pointer(c, u0, dt)
+ * 
  */
   __pyx_t_3 = 0;
   __pyx_t_4 = 0;
   __pyx_v_u0 = (&(*((__pyx_t_double_complex *) ( /* dim=1 */ ((char *) (((__pyx_t_double_complex *) ( /* dim=0 */ (__pyx_v_U.data + __pyx_t_3 * __pyx_v_U.strides[0]) )) + __pyx_t_4)) ))));
 
-  /* "unipolator/hamiltonian_system.pyx":106
+  /* "unipolator/hamiltonian_system.pyx":113
  *             raise ValueError('c.shape[0] needs to be equal to H_s[0].shape[0]-1.')
  *         cdef double complex *u0 = &U[0,0]
- *         self.weighted_hamiltonian(c)             # <<<<<<<<<<<<<<
- *         zheevd(self.jobz, self.uplo, &self.d, self.v0, &self.d, self.e0, self.work0, &self.lwork, self.rwork0, &self.lrwork, self.iwork0, &self.liwork, &self.info)
- *         copy_pointer(self.v0, self.u1, self.d2)
+ *         self.expmH_pointer(c, u0, dt)             # <<<<<<<<<<<<<<
+ * 
+ *     def expmH_pulse_no_multiply(self, double[:,::1] cs, double complex[:,:,::1] U, double dt=1.0):
  */
-  __pyx_t_2 = ((struct __pyx_vtabstruct_10unipolator_18hamiltonian_system_Hamiltonian_System *)__pyx_v_self->__pyx_vtab)->weighted_hamiltonian(__pyx_v_self, __pyx_v_c); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 106, __pyx_L1_error)
+  __pyx_t_2 = ((struct __pyx_vtabstruct_10unipolator_18hamiltonian_system_Hamiltonian_System *)__pyx_v_self->__pyx_vtab)->expmH_pointer(__pyx_v_self, __pyx_v_c, __pyx_v_u0, __pyx_v_dt); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 113, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "unipolator/hamiltonian_system.pyx":107
- *         cdef double complex *u0 = &U[0,0]
- *         self.weighted_hamiltonian(c)
- *         zheevd(self.jobz, self.uplo, &self.d, self.v0, &self.d, self.e0, self.work0, &self.lwork, self.rwork0, &self.lrwork, self.iwork0, &self.liwork, &self.info)             # <<<<<<<<<<<<<<
- *         copy_pointer(self.v0, self.u1, self.d2)
- *         v_exp_pointer(self.e0, self.u1, dt, self.d)
- */
-  __pyx_f_5scipy_6linalg_13cython_lapack_zheevd(__pyx_v_self->jobz, __pyx_v_self->uplo, (&__pyx_v_self->d), __pyx_v_self->v0, (&__pyx_v_self->d), __pyx_v_self->e0, __pyx_v_self->work0, (&__pyx_v_self->lwork), __pyx_v_self->rwork0, (&__pyx_v_self->lrwork), __pyx_v_self->iwork0, (&__pyx_v_self->liwork), (&__pyx_v_self->info));
-
   /* "unipolator/hamiltonian_system.pyx":108
- *         self.weighted_hamiltonian(c)
- *         zheevd(self.jobz, self.uplo, &self.d, self.v0, &self.d, self.e0, self.work0, &self.lwork, self.rwork0, &self.lrwork, self.iwork0, &self.liwork, &self.info)
- *         copy_pointer(self.v0, self.u1, self.d2)             # <<<<<<<<<<<<<<
- *         v_exp_pointer(self.e0, self.u1, dt, self.d)
  *         DagM_M_cdot_pointer(self.v0, self.u1, u0, self.d)
+ * 
+ *     def expmH(self, double[::1] c, double complex[:,::1] U, double dt=1.0):             # <<<<<<<<<<<<<<
+ *         # Construct Hamiltonian
+ *         if not c.shape[0] == self.n_dims_1:
  */
-  __pyx_f_10unipolator_11exp_and_log_copy_pointer(__pyx_v_self->v0, __pyx_v_self->u1, __pyx_v_self->d2);
 
-  /* "unipolator/hamiltonian_system.pyx":109
- *         zheevd(self.jobz, self.uplo, &self.d, self.v0, &self.d, self.e0, self.work0, &self.lwork, self.rwork0, &self.lrwork, self.iwork0, &self.liwork, &self.info)
- *         copy_pointer(self.v0, self.u1, self.d2)
- *         v_exp_pointer(self.e0, self.u1, dt, self.d)             # <<<<<<<<<<<<<<
- *         DagM_M_cdot_pointer(self.v0, self.u1, u0, self.d)
+  /* function exit code */
+  __pyx_r = Py_None; __Pyx_INCREF(Py_None);
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_AddTraceback("unipolator.hamiltonian_system.Hamiltonian_System.expmH", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __PYX_XDEC_MEMVIEW(&__pyx_v_c, 1);
+  __PYX_XDEC_MEMVIEW(&__pyx_v_U, 1);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "unipolator/hamiltonian_system.pyx":115
+ *         self.expmH_pointer(c, u0, dt)
  * 
+ *     def expmH_pulse_no_multiply(self, double[:,::1] cs, double complex[:,:,::1] U, double dt=1.0):             # <<<<<<<<<<<<<<
+ *         cdef double complex *u0 = &U[0, 0, 0]
+ *         cdef how_many = cs.shape[0]
  */
-  __pyx_f_10unipolator_11exp_and_log_v_exp_pointer(__pyx_v_self->e0, __pyx_v_self->u1, __pyx_v_dt, __pyx_v_self->d);
 
-  /* "unipolator/hamiltonian_system.pyx":110
- *         copy_pointer(self.v0, self.u1, self.d2)
- *         v_exp_pointer(self.e0, self.u1, dt, self.d)
- *         DagM_M_cdot_pointer(self.v0, self.u1, u0, self.d)             # <<<<<<<<<<<<<<
+/* Python wrapper */
+static PyObject *__pyx_pw_10unipolator_18hamiltonian_system_18Hamiltonian_System_9expmH_pulse_no_multiply(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_10unipolator_18hamiltonian_system_18Hamiltonian_System_8expmH_pulse_no_multiply[] = "Hamiltonian_System.expmH_pulse_no_multiply(self, double[:, ::1] cs, double complex[:, :, ::1] U, double dt=1.0)";
+static PyObject *__pyx_pw_10unipolator_18hamiltonian_system_18Hamiltonian_System_9expmH_pulse_no_multiply(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+  __Pyx_memviewslice __pyx_v_cs = { 0, 0, { 0 }, { 0 }, { 0 } };
+  __Pyx_memviewslice __pyx_v_U = { 0, 0, { 0 }, { 0 }, { 0 } };
+  double __pyx_v_dt;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("expmH_pulse_no_multiply (wrapper)", 0);
+  {
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_cs,&__pyx_n_s_U,&__pyx_n_s_dt,0};
+    PyObject* values[3] = {0,0,0};
+    if (unlikely(__pyx_kwds)) {
+      Py_ssize_t kw_args;
+      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
+      switch (pos_args) {
+        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+        CYTHON_FALLTHROUGH;
+        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
+        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = PyDict_Size(__pyx_kwds);
+      switch (pos_args) {
+        case  0:
+        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_cs)) != 0)) kw_args--;
+        else goto __pyx_L5_argtuple_error;
+        CYTHON_FALLTHROUGH;
+        case  1:
+        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_U)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("expmH_pulse_no_multiply", 0, 2, 3, 1); __PYX_ERR(0, 115, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  2:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_dt);
+          if (value) { values[2] = value; kw_args--; }
+        }
+      }
+      if (unlikely(kw_args > 0)) {
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "expmH_pulse_no_multiply") < 0)) __PYX_ERR(0, 115, __pyx_L3_error)
+      }
+    } else {
+      switch (PyTuple_GET_SIZE(__pyx_args)) {
+        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+        CYTHON_FALLTHROUGH;
+        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+    }
+    __pyx_v_cs = __Pyx_PyObject_to_MemoryviewSlice_d_dc_double(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_cs.memview)) __PYX_ERR(0, 115, __pyx_L3_error)
+    __pyx_v_U = __Pyx_PyObject_to_MemoryviewSlice_d_d_dc___pyx_t_double_complex(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_U.memview)) __PYX_ERR(0, 115, __pyx_L3_error)
+    if (values[2]) {
+      __pyx_v_dt = __pyx_PyFloat_AsDouble(values[2]); if (unlikely((__pyx_v_dt == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 115, __pyx_L3_error)
+    } else {
+      __pyx_v_dt = ((double)1.0);
+    }
+  }
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("expmH_pulse_no_multiply", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 115, __pyx_L3_error)
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("unipolator.hamiltonian_system.Hamiltonian_System.expmH_pulse_no_multiply", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  __pyx_r = __pyx_pf_10unipolator_18hamiltonian_system_18Hamiltonian_System_8expmH_pulse_no_multiply(((struct __pyx_obj_10unipolator_18hamiltonian_system_Hamiltonian_System *)__pyx_v_self), __pyx_v_cs, __pyx_v_U, __pyx_v_dt);
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_10unipolator_18hamiltonian_system_18Hamiltonian_System_8expmH_pulse_no_multiply(struct __pyx_obj_10unipolator_18hamiltonian_system_Hamiltonian_System *__pyx_v_self, __Pyx_memviewslice __pyx_v_cs, __Pyx_memviewslice __pyx_v_U, double __pyx_v_dt) {
+  __pyx_t_double_complex *__pyx_v_u0;
+  PyObject *__pyx_v_how_many = 0;
+  PyObject *__pyx_v_i = NULL;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  Py_ssize_t __pyx_t_1;
+  Py_ssize_t __pyx_t_2;
+  Py_ssize_t __pyx_t_3;
+  PyObject *__pyx_t_4 = NULL;
+  PyObject *__pyx_t_5 = NULL;
+  Py_ssize_t __pyx_t_6;
+  PyObject *(*__pyx_t_7)(PyObject *);
+  Py_ssize_t __pyx_t_8;
+  __Pyx_memviewslice __pyx_t_9 = { 0, 0, { 0 }, { 0 }, { 0 } };
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("expmH_pulse_no_multiply", 0);
+
+  /* "unipolator/hamiltonian_system.pyx":116
+ * 
+ *     def expmH_pulse_no_multiply(self, double[:,::1] cs, double complex[:,:,::1] U, double dt=1.0):
+ *         cdef double complex *u0 = &U[0, 0, 0]             # <<<<<<<<<<<<<<
+ *         cdef how_many = cs.shape[0]
+ *         for i in range(how_many):
+ */
+  __pyx_t_1 = 0;
+  __pyx_t_2 = 0;
+  __pyx_t_3 = 0;
+  __pyx_v_u0 = (&(*((__pyx_t_double_complex *) ( /* dim=2 */ ((char *) (((__pyx_t_double_complex *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_U.data + __pyx_t_1 * __pyx_v_U.strides[0]) ) + __pyx_t_2 * __pyx_v_U.strides[1]) )) + __pyx_t_3)) ))));
+
+  /* "unipolator/hamiltonian_system.pyx":117
+ *     def expmH_pulse_no_multiply(self, double[:,::1] cs, double complex[:,:,::1] U, double dt=1.0):
+ *         cdef double complex *u0 = &U[0, 0, 0]
+ *         cdef how_many = cs.shape[0]             # <<<<<<<<<<<<<<
+ *         for i in range(how_many):
+ *             self.expmH_pointer(cs[i,:], u0, dt)
+ */
+  __pyx_t_4 = PyInt_FromSsize_t((__pyx_v_cs.shape[0])); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 117, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_v_how_many = __pyx_t_4;
+  __pyx_t_4 = 0;
+
+  /* "unipolator/hamiltonian_system.pyx":118
+ *         cdef double complex *u0 = &U[0, 0, 0]
+ *         cdef how_many = cs.shape[0]
+ *         for i in range(how_many):             # <<<<<<<<<<<<<<
+ *             self.expmH_pointer(cs[i,:], u0, dt)
+ *             u0 += self.d2
+ */
+  __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_range, __pyx_v_how_many); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 118, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  if (likely(PyList_CheckExact(__pyx_t_4)) || PyTuple_CheckExact(__pyx_t_4)) {
+    __pyx_t_5 = __pyx_t_4; __Pyx_INCREF(__pyx_t_5); __pyx_t_6 = 0;
+    __pyx_t_7 = NULL;
+  } else {
+    __pyx_t_6 = -1; __pyx_t_5 = PyObject_GetIter(__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 118, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_t_7 = Py_TYPE(__pyx_t_5)->tp_iternext; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 118, __pyx_L1_error)
+  }
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  for (;;) {
+    if (likely(!__pyx_t_7)) {
+      if (likely(PyList_CheckExact(__pyx_t_5))) {
+        if (__pyx_t_6 >= PyList_GET_SIZE(__pyx_t_5)) break;
+        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_5, __pyx_t_6); __Pyx_INCREF(__pyx_t_4); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 118, __pyx_L1_error)
+        #else
+        __pyx_t_4 = PySequence_ITEM(__pyx_t_5, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 118, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_4);
+        #endif
+      } else {
+        if (__pyx_t_6 >= PyTuple_GET_SIZE(__pyx_t_5)) break;
+        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_5, __pyx_t_6); __Pyx_INCREF(__pyx_t_4); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 118, __pyx_L1_error)
+        #else
+        __pyx_t_4 = PySequence_ITEM(__pyx_t_5, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 118, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_4);
+        #endif
+      }
+    } else {
+      __pyx_t_4 = __pyx_t_7(__pyx_t_5);
+      if (unlikely(!__pyx_t_4)) {
+        PyObject* exc_type = PyErr_Occurred();
+        if (exc_type) {
+          if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
+          else __PYX_ERR(0, 118, __pyx_L1_error)
+        }
+        break;
+      }
+      __Pyx_GOTREF(__pyx_t_4);
+    }
+    __Pyx_XDECREF_SET(__pyx_v_i, __pyx_t_4);
+    __pyx_t_4 = 0;
+
+    /* "unipolator/hamiltonian_system.pyx":119
+ *         cdef how_many = cs.shape[0]
+ *         for i in range(how_many):
+ *             self.expmH_pointer(cs[i,:], u0, dt)             # <<<<<<<<<<<<<<
+ *             u0 += self.d2
+ * 
+ */
+    __pyx_t_8 = __Pyx_PyIndex_AsSsize_t(__pyx_v_i); if (unlikely((__pyx_t_8 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 119, __pyx_L1_error)
+    __pyx_t_9.data = __pyx_v_cs.data;
+    __pyx_t_9.memview = __pyx_v_cs.memview;
+    __PYX_INC_MEMVIEW(&__pyx_t_9, 0);
+    {
+    Py_ssize_t __pyx_tmp_idx = __pyx_t_8;
+    Py_ssize_t __pyx_tmp_stride = __pyx_v_cs.strides[0];
+        __pyx_t_9.data += __pyx_tmp_idx * __pyx_tmp_stride;
+}
+
+__pyx_t_9.shape[0] = __pyx_v_cs.shape[1];
+__pyx_t_9.strides[0] = __pyx_v_cs.strides[1];
+    __pyx_t_9.suboffsets[0] = -1;
+
+__pyx_t_4 = ((struct __pyx_vtabstruct_10unipolator_18hamiltonian_system_Hamiltonian_System *)__pyx_v_self->__pyx_vtab)->expmH_pointer(__pyx_v_self, __pyx_t_9, __pyx_v_u0, __pyx_v_dt); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 119, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __PYX_XDEC_MEMVIEW(&__pyx_t_9, 1);
+    __pyx_t_9.memview = NULL;
+    __pyx_t_9.data = NULL;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+
+    /* "unipolator/hamiltonian_system.pyx":120
+ *         for i in range(how_many):
+ *             self.expmH_pointer(cs[i,:], u0, dt)
+ *             u0 += self.d2             # <<<<<<<<<<<<<<
  * 
  *     cdef dexpmH_pointer(self, double[::1] c, double complex *u0, double complex *du0, dt=1.0):  #int[::1] d_di,
  */
-  __pyx_f_10unipolator_14blas_functions_DagM_M_cdot_pointer(__pyx_v_self->v0, __pyx_v_self->u1, __pyx_v_u0, __pyx_v_self->d);
+    __pyx_v_u0 = (__pyx_v_u0 + __pyx_v_self->d2);
 
-  /* "unipolator/hamiltonian_system.pyx":101
- *             d_mat_add_pointer(self.v0, self.curr_h0, c[i], self.d2)
+    /* "unipolator/hamiltonian_system.pyx":118
+ *         cdef double complex *u0 = &U[0, 0, 0]
+ *         cdef how_many = cs.shape[0]
+ *         for i in range(how_many):             # <<<<<<<<<<<<<<
+ *             self.expmH_pointer(cs[i,:], u0, dt)
+ *             u0 += self.d2
+ */
+  }
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+
+  /* "unipolator/hamiltonian_system.pyx":115
+ *         self.expmH_pointer(c, u0, dt)
  * 
- *     def expmH(self, double[::1] c, double complex[:,::1] U, double dt=1.0):             # <<<<<<<<<<<<<<
- *         # Construct Hamiltonian
- *         if not c.shape[0] == self.n_dims_1:
+ *     def expmH_pulse_no_multiply(self, double[:,::1] cs, double complex[:,:,::1] U, double dt=1.0):             # <<<<<<<<<<<<<<
+ *         cdef double complex *u0 = &U[0, 0, 0]
+ *         cdef how_many = cs.shape[0]
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_AddTraceback("unipolator.hamiltonian_system.Hamiltonian_System.expmH", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_5);
+  __PYX_XDEC_MEMVIEW(&__pyx_t_9, 1);
+  __Pyx_AddTraceback("unipolator.hamiltonian_system.Hamiltonian_System.expmH_pulse_no_multiply", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
-  __PYX_XDEC_MEMVIEW(&__pyx_v_c, 1);
+  __Pyx_XDECREF(__pyx_v_how_many);
+  __Pyx_XDECREF(__pyx_v_i);
+  __PYX_XDEC_MEMVIEW(&__pyx_v_cs, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_v_U, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unipolator/hamiltonian_system.pyx":112
- *         DagM_M_cdot_pointer(self.v0, self.u1, u0, self.d)
+/* "unipolator/hamiltonian_system.pyx":122
+ *             u0 += self.d2
  * 
  *     cdef dexpmH_pointer(self, double[::1] c, double complex *u0, double complex *du0, dt=1.0):  #int[::1] d_di,             # <<<<<<<<<<<<<<
  *         # Construct Hamiltonian
  *         cdef int i
  */
 
 static PyObject *__pyx_f_10unipolator_18hamiltonian_system_18Hamiltonian_System_dexpmH_pointer(struct __pyx_obj_10unipolator_18hamiltonian_system_Hamiltonian_System *__pyx_v_self, __Pyx_memviewslice __pyx_v_c, __pyx_t_double_complex *__pyx_v_u0, __pyx_t_double_complex *__pyx_v_du0, struct __pyx_opt_args_10unipolator_18hamiltonian_system_18Hamiltonian_System_dexpmH_pointer *__pyx_optional_args) {
@@ -4479,164 +4792,164 @@
   __Pyx_RefNannySetupContext("dexpmH_pointer", 0);
   if (__pyx_optional_args) {
     if (__pyx_optional_args->__pyx_n > 0) {
       __pyx_v_dt = __pyx_optional_args->dt;
     }
   }
 
-  /* "unipolator/hamiltonian_system.pyx":117
+  /* "unipolator/hamiltonian_system.pyx":127
  *         cdef double complex *h0
  *         cdef int curr_d_di_1
  *         self.weighted_hamiltonian(c)             # <<<<<<<<<<<<<<
  *         zheevd(self.jobz, self.uplo, &self.d, self.v0, &self.d, self.e0, self.work0, &self.lwork, self.rwork0, &self.lrwork, self.iwork0, &self.liwork, &self.info)
  *         copy_pointer(self.v0, self.u1, self.d2)
  */
-  __pyx_t_1 = ((struct __pyx_vtabstruct_10unipolator_18hamiltonian_system_Hamiltonian_System *)__pyx_v_self->__pyx_vtab)->weighted_hamiltonian(__pyx_v_self, __pyx_v_c); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 117, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_10unipolator_18hamiltonian_system_Hamiltonian_System *)__pyx_v_self->__pyx_vtab)->weighted_hamiltonian(__pyx_v_self, __pyx_v_c); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 127, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "unipolator/hamiltonian_system.pyx":118
+  /* "unipolator/hamiltonian_system.pyx":128
  *         cdef int curr_d_di_1
  *         self.weighted_hamiltonian(c)
  *         zheevd(self.jobz, self.uplo, &self.d, self.v0, &self.d, self.e0, self.work0, &self.lwork, self.rwork0, &self.lrwork, self.iwork0, &self.liwork, &self.info)             # <<<<<<<<<<<<<<
  *         copy_pointer(self.v0, self.u1, self.d2)
  *         v_exp_pointer(self.e0, self.u1, dt, self.d)
  */
   __pyx_f_5scipy_6linalg_13cython_lapack_zheevd(__pyx_v_self->jobz, __pyx_v_self->uplo, (&__pyx_v_self->d), __pyx_v_self->v0, (&__pyx_v_self->d), __pyx_v_self->e0, __pyx_v_self->work0, (&__pyx_v_self->lwork), __pyx_v_self->rwork0, (&__pyx_v_self->lrwork), __pyx_v_self->iwork0, (&__pyx_v_self->liwork), (&__pyx_v_self->info));
 
-  /* "unipolator/hamiltonian_system.pyx":119
+  /* "unipolator/hamiltonian_system.pyx":129
  *         self.weighted_hamiltonian(c)
  *         zheevd(self.jobz, self.uplo, &self.d, self.v0, &self.d, self.e0, self.work0, &self.lwork, self.rwork0, &self.lrwork, self.iwork0, &self.liwork, &self.info)
  *         copy_pointer(self.v0, self.u1, self.d2)             # <<<<<<<<<<<<<<
  *         v_exp_pointer(self.e0, self.u1, dt, self.d)
  *         DagM_M_cdot_pointer(self.v0, self.u1, u0, self.d)
  */
   __pyx_f_10unipolator_11exp_and_log_copy_pointer(__pyx_v_self->v0, __pyx_v_self->u1, __pyx_v_self->d2);
 
-  /* "unipolator/hamiltonian_system.pyx":120
+  /* "unipolator/hamiltonian_system.pyx":130
  *         zheevd(self.jobz, self.uplo, &self.d, self.v0, &self.d, self.e0, self.work0, &self.lwork, self.rwork0, &self.lrwork, self.iwork0, &self.liwork, &self.info)
  *         copy_pointer(self.v0, self.u1, self.d2)
  *         v_exp_pointer(self.e0, self.u1, dt, self.d)             # <<<<<<<<<<<<<<
  *         DagM_M_cdot_pointer(self.v0, self.u1, u0, self.d)
  *         # Calculate the differentials
  */
-  __pyx_t_2 = __pyx_PyFloat_AsDouble(__pyx_v_dt); if (unlikely((__pyx_t_2 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 120, __pyx_L1_error)
+  __pyx_t_2 = __pyx_PyFloat_AsDouble(__pyx_v_dt); if (unlikely((__pyx_t_2 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 130, __pyx_L1_error)
   __pyx_f_10unipolator_11exp_and_log_v_exp_pointer(__pyx_v_self->e0, __pyx_v_self->u1, __pyx_t_2, __pyx_v_self->d);
 
-  /* "unipolator/hamiltonian_system.pyx":121
+  /* "unipolator/hamiltonian_system.pyx":131
  *         copy_pointer(self.v0, self.u1, self.d2)
  *         v_exp_pointer(self.e0, self.u1, dt, self.d)
  *         DagM_M_cdot_pointer(self.v0, self.u1, u0, self.d)             # <<<<<<<<<<<<<<
  *         # Calculate the differentials
  *         for i in range(self.n_d_di): # According to https://arxiv.org/pdf/2006.00935.pdf (Daalgard, Motzoi paper --> Original source?)
  */
   __pyx_f_10unipolator_14blas_functions_DagM_M_cdot_pointer(__pyx_v_self->v0, __pyx_v_self->u1, __pyx_v_u0, __pyx_v_self->d);
 
-  /* "unipolator/hamiltonian_system.pyx":123
+  /* "unipolator/hamiltonian_system.pyx":133
  *         DagM_M_cdot_pointer(self.v0, self.u1, u0, self.d)
  *         # Calculate the differentials
  *         for i in range(self.n_d_di): # According to https://arxiv.org/pdf/2006.00935.pdf (Daalgard, Motzoi paper --> Original source?)             # <<<<<<<<<<<<<<
  *             curr_d_di_1 = self.d_di[i] + 1
  *             h0 = &self.H[curr_d_di_1, 0, 0]
  */
   __pyx_t_3 = __pyx_v_self->n_d_di;
   __pyx_t_4 = __pyx_t_3;
   for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_4; __pyx_t_5+=1) {
     __pyx_v_i = __pyx_t_5;
 
-    /* "unipolator/hamiltonian_system.pyx":124
+    /* "unipolator/hamiltonian_system.pyx":134
  *         # Calculate the differentials
  *         for i in range(self.n_d_di): # According to https://arxiv.org/pdf/2006.00935.pdf (Daalgard, Motzoi paper --> Original source?)
  *             curr_d_di_1 = self.d_di[i] + 1             # <<<<<<<<<<<<<<
  *             h0 = &self.H[curr_d_di_1, 0, 0]
  *             MM_cdot_scale_pointer(dt, self.v0, h0, self.u1, self.d) #self.u1, self.d)
  */
     __pyx_t_6 = __pyx_v_i;
     __pyx_v_curr_d_di_1 = ((*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->d_di.data) + __pyx_t_6)) ))) + 1);
 
-    /* "unipolator/hamiltonian_system.pyx":125
+    /* "unipolator/hamiltonian_system.pyx":135
  *         for i in range(self.n_d_di): # According to https://arxiv.org/pdf/2006.00935.pdf (Daalgard, Motzoi paper --> Original source?)
  *             curr_d_di_1 = self.d_di[i] + 1
  *             h0 = &self.H[curr_d_di_1, 0, 0]             # <<<<<<<<<<<<<<
  *             MM_cdot_scale_pointer(dt, self.v0, h0, self.u1, self.d) #self.u1, self.d)
  *             M_DagM_cdot_pointer(self.u1, self.v0, du0, self.d)
  */
     __pyx_t_6 = __pyx_v_curr_d_di_1;
     __pyx_t_7 = 0;
     __pyx_t_8 = 0;
     __pyx_v_h0 = (&(*((__pyx_t_double_complex *) ( /* dim=2 */ ((char *) (((__pyx_t_double_complex *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_self->H.data + __pyx_t_6 * __pyx_v_self->H.strides[0]) ) + __pyx_t_7 * __pyx_v_self->H.strides[1]) )) + __pyx_t_8)) ))));
 
-    /* "unipolator/hamiltonian_system.pyx":126
+    /* "unipolator/hamiltonian_system.pyx":136
  *             curr_d_di_1 = self.d_di[i] + 1
  *             h0 = &self.H[curr_d_di_1, 0, 0]
  *             MM_cdot_scale_pointer(dt, self.v0, h0, self.u1, self.d) #self.u1, self.d)             # <<<<<<<<<<<<<<
  *             M_DagM_cdot_pointer(self.u1, self.v0, du0, self.d)
  * 
  */
-    __pyx_t_2 = __pyx_PyFloat_AsDouble(__pyx_v_dt); if (unlikely((__pyx_t_2 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 126, __pyx_L1_error)
+    __pyx_t_2 = __pyx_PyFloat_AsDouble(__pyx_v_dt); if (unlikely((__pyx_t_2 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 136, __pyx_L1_error)
     __pyx_f_10unipolator_14blas_functions_MM_cdot_scale_pointer(__pyx_t_2, __pyx_v_self->v0, __pyx_v_h0, __pyx_v_self->u1, __pyx_v_self->d);
 
-    /* "unipolator/hamiltonian_system.pyx":127
+    /* "unipolator/hamiltonian_system.pyx":137
  *             h0 = &self.H[curr_d_di_1, 0, 0]
  *             MM_cdot_scale_pointer(dt, self.v0, h0, self.u1, self.d) #self.u1, self.d)
  *             M_DagM_cdot_pointer(self.u1, self.v0, du0, self.d)             # <<<<<<<<<<<<<<
  * 
  *             phase_shift_matrix_pointer(self.e0, self.c1, self.u1, dt, self.d)
  */
     __pyx_f_10unipolator_14blas_functions_M_DagM_cdot_pointer(__pyx_v_self->u1, __pyx_v_self->v0, __pyx_v_du0, __pyx_v_self->d);
 
-    /* "unipolator/hamiltonian_system.pyx":129
+    /* "unipolator/hamiltonian_system.pyx":139
  *             M_DagM_cdot_pointer(self.u1, self.v0, du0, self.d)
  * 
  *             phase_shift_matrix_pointer(self.e0, self.c1, self.u1, dt, self.d)             # <<<<<<<<<<<<<<
  *             AxB_elementwise_pointer(du0, self.u1, self.u2, self.d2)
  * 
  */
-    __pyx_t_2 = __pyx_PyFloat_AsDouble(__pyx_v_dt); if (unlikely((__pyx_t_2 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 129, __pyx_L1_error)
+    __pyx_t_2 = __pyx_PyFloat_AsDouble(__pyx_v_dt); if (unlikely((__pyx_t_2 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 139, __pyx_L1_error)
     __pyx_f_10unipolator_11exp_and_log_phase_shift_matrix_pointer(__pyx_v_self->e0, __pyx_v_self->c1, __pyx_v_self->u1, __pyx_t_2, __pyx_v_self->d);
 
-    /* "unipolator/hamiltonian_system.pyx":130
+    /* "unipolator/hamiltonian_system.pyx":140
  * 
  *             phase_shift_matrix_pointer(self.e0, self.c1, self.u1, dt, self.d)
  *             AxB_elementwise_pointer(du0, self.u1, self.u2, self.d2)             # <<<<<<<<<<<<<<
  * 
  *             MM_cdot_pointer( self.u2, self.v0, self.u1, self.d)
  */
     __pyx_f_10unipolator_14blas_functions_AxB_elementwise_pointer(__pyx_v_du0, __pyx_v_self->u1, __pyx_v_self->u2, __pyx_v_self->d2);
 
-    /* "unipolator/hamiltonian_system.pyx":132
+    /* "unipolator/hamiltonian_system.pyx":142
  *             AxB_elementwise_pointer(du0, self.u1, self.u2, self.d2)
  * 
  *             MM_cdot_pointer( self.u2, self.v0, self.u1, self.d)             # <<<<<<<<<<<<<<
  *             DagM_M_cdot_pointer(self.v0, self.u1, du0, self.d)
  *             du0 += self.d2
  */
     __pyx_f_10unipolator_14blas_functions_MM_cdot_pointer(__pyx_v_self->u2, __pyx_v_self->v0, __pyx_v_self->u1, __pyx_v_self->d);
 
-    /* "unipolator/hamiltonian_system.pyx":133
+    /* "unipolator/hamiltonian_system.pyx":143
  * 
  *             MM_cdot_pointer( self.u2, self.v0, self.u1, self.d)
  *             DagM_M_cdot_pointer(self.v0, self.u1, du0, self.d)             # <<<<<<<<<<<<<<
  *             du0 += self.d2
  *     def dexpmH(self, double[::1] c, double complex[:,::1] U, double complex[:,:,::1] dU, double dt=1.0):  #int[::1] d_di,
  */
     __pyx_f_10unipolator_14blas_functions_DagM_M_cdot_pointer(__pyx_v_self->v0, __pyx_v_self->u1, __pyx_v_du0, __pyx_v_self->d);
 
-    /* "unipolator/hamiltonian_system.pyx":134
+    /* "unipolator/hamiltonian_system.pyx":144
  *             MM_cdot_pointer( self.u2, self.v0, self.u1, self.d)
  *             DagM_M_cdot_pointer(self.v0, self.u1, du0, self.d)
  *             du0 += self.d2             # <<<<<<<<<<<<<<
  *     def dexpmH(self, double[::1] c, double complex[:,::1] U, double complex[:,:,::1] dU, double dt=1.0):  #int[::1] d_di,
  *         # d_di contains the indexes of the derivatives that we want to calculate (needs to be in ascending order with a negative value at the end)
  */
     __pyx_v_du0 = (__pyx_v_du0 + __pyx_v_self->d2);
   }
 
-  /* "unipolator/hamiltonian_system.pyx":112
- *         DagM_M_cdot_pointer(self.v0, self.u1, u0, self.d)
+  /* "unipolator/hamiltonian_system.pyx":122
+ *             u0 += self.d2
  * 
  *     cdef dexpmH_pointer(self, double[::1] c, double complex *u0, double complex *du0, dt=1.0):  #int[::1] d_di,             # <<<<<<<<<<<<<<
  *         # Construct Hamiltonian
  *         cdef int i
  */
 
   /* function exit code */
@@ -4648,26 +4961,26 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unipolator/hamiltonian_system.pyx":135
+/* "unipolator/hamiltonian_system.pyx":145
  *             DagM_M_cdot_pointer(self.v0, self.u1, du0, self.d)
  *             du0 += self.d2
  *     def dexpmH(self, double[::1] c, double complex[:,::1] U, double complex[:,:,::1] dU, double dt=1.0):  #int[::1] d_di,             # <<<<<<<<<<<<<<
  *         # d_di contains the indexes of the derivatives that we want to calculate (needs to be in ascending order with a negative value at the end)
  *         cdef double complex *u0 = &U[0, 0]
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_10unipolator_18hamiltonian_system_18Hamiltonian_System_9dexpmH(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_10unipolator_18hamiltonian_system_18Hamiltonian_System_8dexpmH[] = "Hamiltonian_System.dexpmH(self, double[::1] c, double complex[:, ::1] U, double complex[:, :, ::1] dU, double dt=1.0)";
-static PyObject *__pyx_pw_10unipolator_18hamiltonian_system_18Hamiltonian_System_9dexpmH(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_10unipolator_18hamiltonian_system_18Hamiltonian_System_11dexpmH(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_10unipolator_18hamiltonian_system_18Hamiltonian_System_10dexpmH[] = "Hamiltonian_System.dexpmH(self, double[::1] c, double complex[:, ::1] U, double complex[:, :, ::1] dU, double dt=1.0)";
+static PyObject *__pyx_pw_10unipolator_18hamiltonian_system_18Hamiltonian_System_11dexpmH(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   __Pyx_memviewslice __pyx_v_c = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_U = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_dU = { 0, 0, { 0 }, { 0 }, { 0 } };
   double __pyx_v_dt;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
@@ -4697,68 +5010,68 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_c)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_U)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("dexpmH", 0, 3, 4, 1); __PYX_ERR(0, 135, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("dexpmH", 0, 3, 4, 1); __PYX_ERR(0, 145, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_dU)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("dexpmH", 0, 3, 4, 2); __PYX_ERR(0, 135, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("dexpmH", 0, 3, 4, 2); __PYX_ERR(0, 145, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_dt);
           if (value) { values[3] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "dexpmH") < 0)) __PYX_ERR(0, 135, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "dexpmH") < 0)) __PYX_ERR(0, 145, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
-    __pyx_v_c = __Pyx_PyObject_to_MemoryviewSlice_dc_double(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_c.memview)) __PYX_ERR(0, 135, __pyx_L3_error)
-    __pyx_v_U = __Pyx_PyObject_to_MemoryviewSlice_d_dc___pyx_t_double_complex(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_U.memview)) __PYX_ERR(0, 135, __pyx_L3_error)
-    __pyx_v_dU = __Pyx_PyObject_to_MemoryviewSlice_d_d_dc___pyx_t_double_complex(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_dU.memview)) __PYX_ERR(0, 135, __pyx_L3_error)
+    __pyx_v_c = __Pyx_PyObject_to_MemoryviewSlice_dc_double(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_c.memview)) __PYX_ERR(0, 145, __pyx_L3_error)
+    __pyx_v_U = __Pyx_PyObject_to_MemoryviewSlice_d_dc___pyx_t_double_complex(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_U.memview)) __PYX_ERR(0, 145, __pyx_L3_error)
+    __pyx_v_dU = __Pyx_PyObject_to_MemoryviewSlice_d_d_dc___pyx_t_double_complex(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_dU.memview)) __PYX_ERR(0, 145, __pyx_L3_error)
     if (values[3]) {
-      __pyx_v_dt = __pyx_PyFloat_AsDouble(values[3]); if (unlikely((__pyx_v_dt == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 135, __pyx_L3_error)
+      __pyx_v_dt = __pyx_PyFloat_AsDouble(values[3]); if (unlikely((__pyx_v_dt == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 145, __pyx_L3_error)
     } else {
       __pyx_v_dt = ((double)1.0);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("dexpmH", 0, 3, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 135, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("dexpmH", 0, 3, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 145, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("unipolator.hamiltonian_system.Hamiltonian_System.dexpmH", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_10unipolator_18hamiltonian_system_18Hamiltonian_System_8dexpmH(((struct __pyx_obj_10unipolator_18hamiltonian_system_Hamiltonian_System *)__pyx_v_self), __pyx_v_c, __pyx_v_U, __pyx_v_dU, __pyx_v_dt);
+  __pyx_r = __pyx_pf_10unipolator_18hamiltonian_system_18Hamiltonian_System_10dexpmH(((struct __pyx_obj_10unipolator_18hamiltonian_system_Hamiltonian_System *)__pyx_v_self), __pyx_v_c, __pyx_v_U, __pyx_v_dU, __pyx_v_dt);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_10unipolator_18hamiltonian_system_18Hamiltonian_System_8dexpmH(struct __pyx_obj_10unipolator_18hamiltonian_system_Hamiltonian_System *__pyx_v_self, __Pyx_memviewslice __pyx_v_c, __Pyx_memviewslice __pyx_v_U, __Pyx_memviewslice __pyx_v_dU, double __pyx_v_dt) {
+static PyObject *__pyx_pf_10unipolator_18hamiltonian_system_18Hamiltonian_System_10dexpmH(struct __pyx_obj_10unipolator_18hamiltonian_system_Hamiltonian_System *__pyx_v_self, __Pyx_memviewslice __pyx_v_c, __Pyx_memviewslice __pyx_v_U, __Pyx_memviewslice __pyx_v_dU, double __pyx_v_dt) {
   __pyx_t_double_complex *__pyx_v_u0;
   __pyx_t_double_complex *__pyx_v_du0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   Py_ssize_t __pyx_t_1;
   Py_ssize_t __pyx_t_2;
   Py_ssize_t __pyx_t_3;
@@ -4767,118 +5080,118 @@
   PyObject *__pyx_t_6 = NULL;
   struct __pyx_opt_args_10unipolator_18hamiltonian_system_18Hamiltonian_System_dexpmH_pointer __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("dexpmH", 0);
 
-  /* "unipolator/hamiltonian_system.pyx":137
+  /* "unipolator/hamiltonian_system.pyx":147
  *     def dexpmH(self, double[::1] c, double complex[:,::1] U, double complex[:,:,::1] dU, double dt=1.0):  #int[::1] d_di,
  *         # d_di contains the indexes of the derivatives that we want to calculate (needs to be in ascending order with a negative value at the end)
  *         cdef double complex *u0 = &U[0, 0]             # <<<<<<<<<<<<<<
  *         cdef double complex *du0 = &dU[0,0,0]
  *         if not c.shape[0] == self.n_dims_1:
  */
   __pyx_t_1 = 0;
   __pyx_t_2 = 0;
   __pyx_v_u0 = (&(*((__pyx_t_double_complex *) ( /* dim=1 */ ((char *) (((__pyx_t_double_complex *) ( /* dim=0 */ (__pyx_v_U.data + __pyx_t_1 * __pyx_v_U.strides[0]) )) + __pyx_t_2)) ))));
 
-  /* "unipolator/hamiltonian_system.pyx":138
+  /* "unipolator/hamiltonian_system.pyx":148
  *         # d_di contains the indexes of the derivatives that we want to calculate (needs to be in ascending order with a negative value at the end)
  *         cdef double complex *u0 = &U[0, 0]
  *         cdef double complex *du0 = &dU[0,0,0]             # <<<<<<<<<<<<<<
  *         if not c.shape[0] == self.n_dims_1:
  *             raise ValueError('The coefficient c must be of size [interpolation_dimensions].')
  */
   __pyx_t_2 = 0;
   __pyx_t_1 = 0;
   __pyx_t_3 = 0;
   __pyx_v_du0 = (&(*((__pyx_t_double_complex *) ( /* dim=2 */ ((char *) (((__pyx_t_double_complex *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_dU.data + __pyx_t_2 * __pyx_v_dU.strides[0]) ) + __pyx_t_1 * __pyx_v_dU.strides[1]) )) + __pyx_t_3)) ))));
 
-  /* "unipolator/hamiltonian_system.pyx":139
+  /* "unipolator/hamiltonian_system.pyx":149
  *         cdef double complex *u0 = &U[0, 0]
  *         cdef double complex *du0 = &dU[0,0,0]
  *         if not c.shape[0] == self.n_dims_1:             # <<<<<<<<<<<<<<
  *             raise ValueError('The coefficient c must be of size [interpolation_dimensions].')
  *         if not self.d_di.shape[0] == dU.shape[0]:
  */
   __pyx_t_4 = ((!(((__pyx_v_c.shape[0]) == __pyx_v_self->n_dims_1) != 0)) != 0);
   if (unlikely(__pyx_t_4)) {
 
-    /* "unipolator/hamiltonian_system.pyx":140
+    /* "unipolator/hamiltonian_system.pyx":150
  *         cdef double complex *du0 = &dU[0,0,0]
  *         if not c.shape[0] == self.n_dims_1:
  *             raise ValueError('The coefficient c must be of size [interpolation_dimensions].')             # <<<<<<<<<<<<<<
  *         if not self.d_di.shape[0] == dU.shape[0]:
  *             raise ValueError('Inputs must fulfill: which_diffs.shape[0] = dU.shape[0].')
  */
-    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 140, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 150, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_Raise(__pyx_t_5, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __PYX_ERR(0, 140, __pyx_L1_error)
+    __PYX_ERR(0, 150, __pyx_L1_error)
 
-    /* "unipolator/hamiltonian_system.pyx":139
+    /* "unipolator/hamiltonian_system.pyx":149
  *         cdef double complex *u0 = &U[0, 0]
  *         cdef double complex *du0 = &dU[0,0,0]
  *         if not c.shape[0] == self.n_dims_1:             # <<<<<<<<<<<<<<
  *             raise ValueError('The coefficient c must be of size [interpolation_dimensions].')
  *         if not self.d_di.shape[0] == dU.shape[0]:
  */
   }
 
-  /* "unipolator/hamiltonian_system.pyx":141
+  /* "unipolator/hamiltonian_system.pyx":151
  *         if not c.shape[0] == self.n_dims_1:
  *             raise ValueError('The coefficient c must be of size [interpolation_dimensions].')
  *         if not self.d_di.shape[0] == dU.shape[0]:             # <<<<<<<<<<<<<<
  *             raise ValueError('Inputs must fulfill: which_diffs.shape[0] = dU.shape[0].')
  *         self.dexpmH_pointer(c, u0, du0, dt)
  */
   __pyx_t_4 = ((!(((__pyx_v_self->d_di.shape[0]) == (__pyx_v_dU.shape[0])) != 0)) != 0);
   if (unlikely(__pyx_t_4)) {
 
-    /* "unipolator/hamiltonian_system.pyx":142
+    /* "unipolator/hamiltonian_system.pyx":152
  *             raise ValueError('The coefficient c must be of size [interpolation_dimensions].')
  *         if not self.d_di.shape[0] == dU.shape[0]:
  *             raise ValueError('Inputs must fulfill: which_diffs.shape[0] = dU.shape[0].')             # <<<<<<<<<<<<<<
  *         self.dexpmH_pointer(c, u0, du0, dt)
  * 
  */
-    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 142, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 152, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_Raise(__pyx_t_5, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __PYX_ERR(0, 142, __pyx_L1_error)
+    __PYX_ERR(0, 152, __pyx_L1_error)
 
-    /* "unipolator/hamiltonian_system.pyx":141
+    /* "unipolator/hamiltonian_system.pyx":151
  *         if not c.shape[0] == self.n_dims_1:
  *             raise ValueError('The coefficient c must be of size [interpolation_dimensions].')
  *         if not self.d_di.shape[0] == dU.shape[0]:             # <<<<<<<<<<<<<<
  *             raise ValueError('Inputs must fulfill: which_diffs.shape[0] = dU.shape[0].')
  *         self.dexpmH_pointer(c, u0, du0, dt)
  */
   }
 
-  /* "unipolator/hamiltonian_system.pyx":143
+  /* "unipolator/hamiltonian_system.pyx":153
  *         if not self.d_di.shape[0] == dU.shape[0]:
  *             raise ValueError('Inputs must fulfill: which_diffs.shape[0] = dU.shape[0].')
  *         self.dexpmH_pointer(c, u0, du0, dt)             # <<<<<<<<<<<<<<
  * 
  *     cdef expmH_pulse_pointer(self, double[:,::1] cs, double complex *u0, double dt=1.0):
  */
-  __pyx_t_5 = PyFloat_FromDouble(__pyx_v_dt); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 143, __pyx_L1_error)
+  __pyx_t_5 = PyFloat_FromDouble(__pyx_v_dt); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 153, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_7.__pyx_n = 1;
   __pyx_t_7.dt = __pyx_t_5;
-  __pyx_t_6 = ((struct __pyx_vtabstruct_10unipolator_18hamiltonian_system_Hamiltonian_System *)__pyx_v_self->__pyx_vtab)->dexpmH_pointer(__pyx_v_self, __pyx_v_c, __pyx_v_u0, __pyx_v_du0, &__pyx_t_7); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 143, __pyx_L1_error)
+  __pyx_t_6 = ((struct __pyx_vtabstruct_10unipolator_18hamiltonian_system_Hamiltonian_System *)__pyx_v_self->__pyx_vtab)->dexpmH_pointer(__pyx_v_self, __pyx_v_c, __pyx_v_u0, __pyx_v_du0, &__pyx_t_7); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 153, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-  /* "unipolator/hamiltonian_system.pyx":135
+  /* "unipolator/hamiltonian_system.pyx":145
  *             DagM_M_cdot_pointer(self.v0, self.u1, du0, self.d)
  *             du0 += self.d2
  *     def dexpmH(self, double[::1] c, double complex[:,::1] U, double complex[:,:,::1] dU, double dt=1.0):  #int[::1] d_di,             # <<<<<<<<<<<<<<
  *         # d_di contains the indexes of the derivatives that we want to calculate (needs to be in ascending order with a negative value at the end)
  *         cdef double complex *u0 = &U[0, 0]
  */
 
@@ -4895,15 +5208,15 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_U, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_v_dU, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unipolator/hamiltonian_system.pyx":145
+/* "unipolator/hamiltonian_system.pyx":155
  *         self.dexpmH_pointer(c, u0, du0, dt)
  * 
  *     cdef expmH_pulse_pointer(self, double[:,::1] cs, double complex *u0, double dt=1.0):             # <<<<<<<<<<<<<<
  *         cdef int i
  *         cdef int steps = cs.shape[0]
  */
 
@@ -4924,24 +5237,24 @@
   __Pyx_RefNannySetupContext("expmH_pulse_pointer", 0);
   if (__pyx_optional_args) {
     if (__pyx_optional_args->__pyx_n > 0) {
       __pyx_v_dt = __pyx_optional_args->dt;
     }
   }
 
-  /* "unipolator/hamiltonian_system.pyx":147
+  /* "unipolator/hamiltonian_system.pyx":157
  *     cdef expmH_pulse_pointer(self, double[:,::1] cs, double complex *u0, double dt=1.0):
  *         cdef int i
  *         cdef int steps = cs.shape[0]             # <<<<<<<<<<<<<<
  * 
  *         self.weighted_hamiltonian(cs[0,:])
  */
   __pyx_v_steps = (__pyx_v_cs.shape[0]);
 
-  /* "unipolator/hamiltonian_system.pyx":149
+  /* "unipolator/hamiltonian_system.pyx":159
  *         cdef int steps = cs.shape[0]
  * 
  *         self.weighted_hamiltonian(cs[0,:])             # <<<<<<<<<<<<<<
  *         zheevd(self.jobz, self.uplo, &self.d, self.v0, &self.d, self.e0, self.work0, &self.lwork, self.rwork0, &self.lrwork, self.iwork0, &self.liwork, &self.info)
  *         copy_pointer(self.v0, self.u1, self.d2)
  */
   __pyx_t_1.data = __pyx_v_cs.data;
@@ -4953,70 +5266,70 @@
         __pyx_t_1.data += __pyx_tmp_idx * __pyx_tmp_stride;
 }
 
 __pyx_t_1.shape[0] = __pyx_v_cs.shape[1];
 __pyx_t_1.strides[0] = __pyx_v_cs.strides[1];
     __pyx_t_1.suboffsets[0] = -1;
 
-__pyx_t_2 = ((struct __pyx_vtabstruct_10unipolator_18hamiltonian_system_Hamiltonian_System *)__pyx_v_self->__pyx_vtab)->weighted_hamiltonian(__pyx_v_self, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 149, __pyx_L1_error)
+__pyx_t_2 = ((struct __pyx_vtabstruct_10unipolator_18hamiltonian_system_Hamiltonian_System *)__pyx_v_self->__pyx_vtab)->weighted_hamiltonian(__pyx_v_self, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 159, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __PYX_XDEC_MEMVIEW(&__pyx_t_1, 1);
   __pyx_t_1.memview = NULL;
   __pyx_t_1.data = NULL;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "unipolator/hamiltonian_system.pyx":150
+  /* "unipolator/hamiltonian_system.pyx":160
  * 
  *         self.weighted_hamiltonian(cs[0,:])
  *         zheevd(self.jobz, self.uplo, &self.d, self.v0, &self.d, self.e0, self.work0, &self.lwork, self.rwork0, &self.lrwork, self.iwork0, &self.liwork, &self.info)             # <<<<<<<<<<<<<<
  *         copy_pointer(self.v0, self.u1, self.d2)
  *         v_exp_pointer(self.e0, self.v0, dt, self.d)
  */
   __pyx_f_5scipy_6linalg_13cython_lapack_zheevd(__pyx_v_self->jobz, __pyx_v_self->uplo, (&__pyx_v_self->d), __pyx_v_self->v0, (&__pyx_v_self->d), __pyx_v_self->e0, __pyx_v_self->work0, (&__pyx_v_self->lwork), __pyx_v_self->rwork0, (&__pyx_v_self->lrwork), __pyx_v_self->iwork0, (&__pyx_v_self->liwork), (&__pyx_v_self->info));
 
-  /* "unipolator/hamiltonian_system.pyx":151
+  /* "unipolator/hamiltonian_system.pyx":161
  *         self.weighted_hamiltonian(cs[0,:])
  *         zheevd(self.jobz, self.uplo, &self.d, self.v0, &self.d, self.e0, self.work0, &self.lwork, self.rwork0, &self.lrwork, self.iwork0, &self.liwork, &self.info)
  *         copy_pointer(self.v0, self.u1, self.d2)             # <<<<<<<<<<<<<<
  *         v_exp_pointer(self.e0, self.v0, dt, self.d)
  *         DagM_M_cdot_pointer(self.u1, self.v0, u0, self.d)
  */
   __pyx_f_10unipolator_11exp_and_log_copy_pointer(__pyx_v_self->v0, __pyx_v_self->u1, __pyx_v_self->d2);
 
-  /* "unipolator/hamiltonian_system.pyx":152
+  /* "unipolator/hamiltonian_system.pyx":162
  *         zheevd(self.jobz, self.uplo, &self.d, self.v0, &self.d, self.e0, self.work0, &self.lwork, self.rwork0, &self.lrwork, self.iwork0, &self.liwork, &self.info)
  *         copy_pointer(self.v0, self.u1, self.d2)
  *         v_exp_pointer(self.e0, self.v0, dt, self.d)             # <<<<<<<<<<<<<<
  *         DagM_M_cdot_pointer(self.u1, self.v0, u0, self.d)
  * 
  */
   __pyx_f_10unipolator_11exp_and_log_v_exp_pointer(__pyx_v_self->e0, __pyx_v_self->v0, __pyx_v_dt, __pyx_v_self->d);
 
-  /* "unipolator/hamiltonian_system.pyx":153
+  /* "unipolator/hamiltonian_system.pyx":163
  *         copy_pointer(self.v0, self.u1, self.d2)
  *         v_exp_pointer(self.e0, self.v0, dt, self.d)
  *         DagM_M_cdot_pointer(self.u1, self.v0, u0, self.d)             # <<<<<<<<<<<<<<
  * 
  *         for i in range(1,steps):
  */
   __pyx_f_10unipolator_14blas_functions_DagM_M_cdot_pointer(__pyx_v_self->u1, __pyx_v_self->v0, __pyx_v_u0, __pyx_v_self->d);
 
-  /* "unipolator/hamiltonian_system.pyx":155
+  /* "unipolator/hamiltonian_system.pyx":165
  *         DagM_M_cdot_pointer(self.u1, self.v0, u0, self.d)
  * 
  *         for i in range(1,steps):             # <<<<<<<<<<<<<<
  *             self.weighted_hamiltonian(cs[i, :])
  *             zheevd(self.jobz, self.uplo, &self.d, self.v0, &self.d, self.e0, self.work0, &self.lwork, self.rwork0, &self.lrwork, self.iwork0, &self.liwork, &self.info)
  */
   __pyx_t_3 = __pyx_v_steps;
   __pyx_t_4 = __pyx_t_3;
   for (__pyx_t_5 = 1; __pyx_t_5 < __pyx_t_4; __pyx_t_5+=1) {
     __pyx_v_i = __pyx_t_5;
 
-    /* "unipolator/hamiltonian_system.pyx":156
+    /* "unipolator/hamiltonian_system.pyx":166
  * 
  *         for i in range(1,steps):
  *             self.weighted_hamiltonian(cs[i, :])             # <<<<<<<<<<<<<<
  *             zheevd(self.jobz, self.uplo, &self.d, self.v0, &self.d, self.e0, self.work0, &self.lwork, self.rwork0, &self.lrwork, self.iwork0, &self.liwork, &self.info)
  *             MM_cdot_pointer(self.v0, u0, self.u1, self.d)
  */
     __pyx_t_1.data = __pyx_v_cs.data;
@@ -5028,59 +5341,59 @@
         __pyx_t_1.data += __pyx_tmp_idx * __pyx_tmp_stride;
 }
 
 __pyx_t_1.shape[0] = __pyx_v_cs.shape[1];
 __pyx_t_1.strides[0] = __pyx_v_cs.strides[1];
     __pyx_t_1.suboffsets[0] = -1;
 
-__pyx_t_2 = ((struct __pyx_vtabstruct_10unipolator_18hamiltonian_system_Hamiltonian_System *)__pyx_v_self->__pyx_vtab)->weighted_hamiltonian(__pyx_v_self, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 156, __pyx_L1_error)
+__pyx_t_2 = ((struct __pyx_vtabstruct_10unipolator_18hamiltonian_system_Hamiltonian_System *)__pyx_v_self->__pyx_vtab)->weighted_hamiltonian(__pyx_v_self, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 166, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __PYX_XDEC_MEMVIEW(&__pyx_t_1, 1);
     __pyx_t_1.memview = NULL;
     __pyx_t_1.data = NULL;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "unipolator/hamiltonian_system.pyx":157
+    /* "unipolator/hamiltonian_system.pyx":167
  *         for i in range(1,steps):
  *             self.weighted_hamiltonian(cs[i, :])
  *             zheevd(self.jobz, self.uplo, &self.d, self.v0, &self.d, self.e0, self.work0, &self.lwork, self.rwork0, &self.lrwork, self.iwork0, &self.liwork, &self.info)             # <<<<<<<<<<<<<<
  *             MM_cdot_pointer(self.v0, u0, self.u1, self.d)
  *             v_exp_pointer(self.e0, self.u1, dt, self.d)
  */
     __pyx_f_5scipy_6linalg_13cython_lapack_zheevd(__pyx_v_self->jobz, __pyx_v_self->uplo, (&__pyx_v_self->d), __pyx_v_self->v0, (&__pyx_v_self->d), __pyx_v_self->e0, __pyx_v_self->work0, (&__pyx_v_self->lwork), __pyx_v_self->rwork0, (&__pyx_v_self->lrwork), __pyx_v_self->iwork0, (&__pyx_v_self->liwork), (&__pyx_v_self->info));
 
-    /* "unipolator/hamiltonian_system.pyx":158
+    /* "unipolator/hamiltonian_system.pyx":168
  *             self.weighted_hamiltonian(cs[i, :])
  *             zheevd(self.jobz, self.uplo, &self.d, self.v0, &self.d, self.e0, self.work0, &self.lwork, self.rwork0, &self.lrwork, self.iwork0, &self.liwork, &self.info)
  *             MM_cdot_pointer(self.v0, u0, self.u1, self.d)             # <<<<<<<<<<<<<<
  *             v_exp_pointer(self.e0, self.u1, dt, self.d)
  *             DagM_M_cdot_pointer(self.v0, self.u1, u0, self.d)
  */
     __pyx_f_10unipolator_14blas_functions_MM_cdot_pointer(__pyx_v_self->v0, __pyx_v_u0, __pyx_v_self->u1, __pyx_v_self->d);
 
-    /* "unipolator/hamiltonian_system.pyx":159
+    /* "unipolator/hamiltonian_system.pyx":169
  *             zheevd(self.jobz, self.uplo, &self.d, self.v0, &self.d, self.e0, self.work0, &self.lwork, self.rwork0, &self.lrwork, self.iwork0, &self.liwork, &self.info)
  *             MM_cdot_pointer(self.v0, u0, self.u1, self.d)
  *             v_exp_pointer(self.e0, self.u1, dt, self.d)             # <<<<<<<<<<<<<<
  *             DagM_M_cdot_pointer(self.v0, self.u1, u0, self.d)
  *     def expmH_pulse(self, double[:,::1] cs, double complex[:,::1] U, double dt=1.0):
  */
     __pyx_f_10unipolator_11exp_and_log_v_exp_pointer(__pyx_v_self->e0, __pyx_v_self->u1, __pyx_v_dt, __pyx_v_self->d);
 
-    /* "unipolator/hamiltonian_system.pyx":160
+    /* "unipolator/hamiltonian_system.pyx":170
  *             MM_cdot_pointer(self.v0, u0, self.u1, self.d)
  *             v_exp_pointer(self.e0, self.u1, dt, self.d)
  *             DagM_M_cdot_pointer(self.v0, self.u1, u0, self.d)             # <<<<<<<<<<<<<<
  *     def expmH_pulse(self, double[:,::1] cs, double complex[:,::1] U, double dt=1.0):
  *         # Construct Hamiltonian
  */
     __pyx_f_10unipolator_14blas_functions_DagM_M_cdot_pointer(__pyx_v_self->v0, __pyx_v_self->u1, __pyx_v_u0, __pyx_v_self->d);
   }
 
-  /* "unipolator/hamiltonian_system.pyx":145
+  /* "unipolator/hamiltonian_system.pyx":155
  *         self.dexpmH_pointer(c, u0, du0, dt)
  * 
  *     cdef expmH_pulse_pointer(self, double[:,::1] cs, double complex *u0, double dt=1.0):             # <<<<<<<<<<<<<<
  *         cdef int i
  *         cdef int steps = cs.shape[0]
  */
 
@@ -5094,26 +5407,26 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unipolator/hamiltonian_system.pyx":161
+/* "unipolator/hamiltonian_system.pyx":171
  *             v_exp_pointer(self.e0, self.u1, dt, self.d)
  *             DagM_M_cdot_pointer(self.v0, self.u1, u0, self.d)
  *     def expmH_pulse(self, double[:,::1] cs, double complex[:,::1] U, double dt=1.0):             # <<<<<<<<<<<<<<
  *         # Construct Hamiltonian
  *         cdef double complex *u0 = &U[0, 0]
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_10unipolator_18hamiltonian_system_18Hamiltonian_System_11expmH_pulse(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_10unipolator_18hamiltonian_system_18Hamiltonian_System_10expmH_pulse[] = "Hamiltonian_System.expmH_pulse(self, double[:, ::1] cs, double complex[:, ::1] U, double dt=1.0)";
-static PyObject *__pyx_pw_10unipolator_18hamiltonian_system_18Hamiltonian_System_11expmH_pulse(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_10unipolator_18hamiltonian_system_18Hamiltonian_System_13expmH_pulse(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_10unipolator_18hamiltonian_system_18Hamiltonian_System_12expmH_pulse[] = "Hamiltonian_System.expmH_pulse(self, double[:, ::1] cs, double complex[:, ::1] U, double dt=1.0)";
+static PyObject *__pyx_pw_10unipolator_18hamiltonian_system_18Hamiltonian_System_13expmH_pulse(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   __Pyx_memviewslice __pyx_v_cs = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_U = { 0, 0, { 0 }, { 0 }, { 0 } };
   double __pyx_v_dt;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
@@ -5140,97 +5453,97 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_cs)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_U)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("expmH_pulse", 0, 2, 3, 1); __PYX_ERR(0, 161, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("expmH_pulse", 0, 2, 3, 1); __PYX_ERR(0, 171, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_dt);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "expmH_pulse") < 0)) __PYX_ERR(0, 161, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "expmH_pulse") < 0)) __PYX_ERR(0, 171, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
-    __pyx_v_cs = __Pyx_PyObject_to_MemoryviewSlice_d_dc_double(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_cs.memview)) __PYX_ERR(0, 161, __pyx_L3_error)
-    __pyx_v_U = __Pyx_PyObject_to_MemoryviewSlice_d_dc___pyx_t_double_complex(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_U.memview)) __PYX_ERR(0, 161, __pyx_L3_error)
+    __pyx_v_cs = __Pyx_PyObject_to_MemoryviewSlice_d_dc_double(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_cs.memview)) __PYX_ERR(0, 171, __pyx_L3_error)
+    __pyx_v_U = __Pyx_PyObject_to_MemoryviewSlice_d_dc___pyx_t_double_complex(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_U.memview)) __PYX_ERR(0, 171, __pyx_L3_error)
     if (values[2]) {
-      __pyx_v_dt = __pyx_PyFloat_AsDouble(values[2]); if (unlikely((__pyx_v_dt == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 161, __pyx_L3_error)
+      __pyx_v_dt = __pyx_PyFloat_AsDouble(values[2]); if (unlikely((__pyx_v_dt == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 171, __pyx_L3_error)
     } else {
       __pyx_v_dt = ((double)1.0);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("expmH_pulse", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 161, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("expmH_pulse", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 171, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("unipolator.hamiltonian_system.Hamiltonian_System.expmH_pulse", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_10unipolator_18hamiltonian_system_18Hamiltonian_System_10expmH_pulse(((struct __pyx_obj_10unipolator_18hamiltonian_system_Hamiltonian_System *)__pyx_v_self), __pyx_v_cs, __pyx_v_U, __pyx_v_dt);
+  __pyx_r = __pyx_pf_10unipolator_18hamiltonian_system_18Hamiltonian_System_12expmH_pulse(((struct __pyx_obj_10unipolator_18hamiltonian_system_Hamiltonian_System *)__pyx_v_self), __pyx_v_cs, __pyx_v_U, __pyx_v_dt);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_10unipolator_18hamiltonian_system_18Hamiltonian_System_10expmH_pulse(struct __pyx_obj_10unipolator_18hamiltonian_system_Hamiltonian_System *__pyx_v_self, __Pyx_memviewslice __pyx_v_cs, __Pyx_memviewslice __pyx_v_U, double __pyx_v_dt) {
+static PyObject *__pyx_pf_10unipolator_18hamiltonian_system_18Hamiltonian_System_12expmH_pulse(struct __pyx_obj_10unipolator_18hamiltonian_system_Hamiltonian_System *__pyx_v_self, __Pyx_memviewslice __pyx_v_cs, __Pyx_memviewslice __pyx_v_U, double __pyx_v_dt) {
   __pyx_t_double_complex *__pyx_v_u0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   Py_ssize_t __pyx_t_1;
   Py_ssize_t __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   struct __pyx_opt_args_10unipolator_18hamiltonian_system_18Hamiltonian_System_expmH_pulse_pointer __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("expmH_pulse", 0);
 
-  /* "unipolator/hamiltonian_system.pyx":163
+  /* "unipolator/hamiltonian_system.pyx":173
  *     def expmH_pulse(self, double[:,::1] cs, double complex[:,::1] U, double dt=1.0):
  *         # Construct Hamiltonian
  *         cdef double complex *u0 = &U[0, 0]             # <<<<<<<<<<<<<<
  *         self.expmH_pulse_pointer(cs, u0, dt)
  * 
  */
   __pyx_t_1 = 0;
   __pyx_t_2 = 0;
   __pyx_v_u0 = (&(*((__pyx_t_double_complex *) ( /* dim=1 */ ((char *) (((__pyx_t_double_complex *) ( /* dim=0 */ (__pyx_v_U.data + __pyx_t_1 * __pyx_v_U.strides[0]) )) + __pyx_t_2)) ))));
 
-  /* "unipolator/hamiltonian_system.pyx":164
+  /* "unipolator/hamiltonian_system.pyx":174
  *         # Construct Hamiltonian
  *         cdef double complex *u0 = &U[0, 0]
  *         self.expmH_pulse_pointer(cs, u0, dt)             # <<<<<<<<<<<<<<
  * 
  *     def grape(self, double[:,::1] cs, double complex[:,::1] U_target, int[::1] target_indexes, double complex[:,::1] U, double complex[:,:,::1] dU, double[:,::1] dI_dj):
  */
   __pyx_t_4.__pyx_n = 1;
   __pyx_t_4.dt = __pyx_v_dt;
-  __pyx_t_3 = ((struct __pyx_vtabstruct_10unipolator_18hamiltonian_system_Hamiltonian_System *)__pyx_v_self->__pyx_vtab)->expmH_pulse_pointer(__pyx_v_self, __pyx_v_cs, __pyx_v_u0, &__pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 164, __pyx_L1_error)
+  __pyx_t_3 = ((struct __pyx_vtabstruct_10unipolator_18hamiltonian_system_Hamiltonian_System *)__pyx_v_self->__pyx_vtab)->expmH_pulse_pointer(__pyx_v_self, __pyx_v_cs, __pyx_v_u0, &__pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 174, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "unipolator/hamiltonian_system.pyx":161
+  /* "unipolator/hamiltonian_system.pyx":171
  *             v_exp_pointer(self.e0, self.u1, dt, self.d)
  *             DagM_M_cdot_pointer(self.v0, self.u1, u0, self.d)
  *     def expmH_pulse(self, double[:,::1] cs, double complex[:,::1] U, double dt=1.0):             # <<<<<<<<<<<<<<
  *         # Construct Hamiltonian
  *         cdef double complex *u0 = &U[0, 0]
  */
 
@@ -5245,26 +5558,26 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_cs, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_v_U, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unipolator/hamiltonian_system.pyx":166
+/* "unipolator/hamiltonian_system.pyx":176
  *         self.expmH_pulse_pointer(cs, u0, dt)
  * 
  *     def grape(self, double[:,::1] cs, double complex[:,::1] U_target, int[::1] target_indexes, double complex[:,::1] U, double complex[:,:,::1] dU, double[:,::1] dI_dj):             # <<<<<<<<<<<<<<
  *         # Calculate fidelity for a pulse and the differentials of the fidelity at every timestep using the grape trick
  *         cdef int i, j
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_10unipolator_18hamiltonian_system_18Hamiltonian_System_13grape(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_10unipolator_18hamiltonian_system_18Hamiltonian_System_12grape[] = "Hamiltonian_System.grape(self, double[:, ::1] cs, double complex[:, ::1] U_target, int[::1] target_indexes, double complex[:, ::1] U, double complex[:, :, ::1] dU, double[:, ::1] dI_dj)";
-static PyObject *__pyx_pw_10unipolator_18hamiltonian_system_18Hamiltonian_System_13grape(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_10unipolator_18hamiltonian_system_18Hamiltonian_System_15grape(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_10unipolator_18hamiltonian_system_18Hamiltonian_System_14grape[] = "Hamiltonian_System.grape(self, double[:, ::1] cs, double complex[:, ::1] U_target, int[::1] target_indexes, double complex[:, ::1] U, double complex[:, :, ::1] dU, double[:, ::1] dI_dj)";
+static PyObject *__pyx_pw_10unipolator_18hamiltonian_system_18Hamiltonian_System_15grape(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   __Pyx_memviewslice __pyx_v_cs = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_U_target = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_target_indexes = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_U = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_dU = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_dI_dj = { 0, 0, { 0 }, { 0 }, { 0 } };
   int __pyx_lineno = 0;
@@ -5300,77 +5613,77 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_cs)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_U_target)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("grape", 1, 6, 6, 1); __PYX_ERR(0, 166, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("grape", 1, 6, 6, 1); __PYX_ERR(0, 176, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_target_indexes)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("grape", 1, 6, 6, 2); __PYX_ERR(0, 166, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("grape", 1, 6, 6, 2); __PYX_ERR(0, 176, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_U)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("grape", 1, 6, 6, 3); __PYX_ERR(0, 166, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("grape", 1, 6, 6, 3); __PYX_ERR(0, 176, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (likely((values[4] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_dU)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("grape", 1, 6, 6, 4); __PYX_ERR(0, 166, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("grape", 1, 6, 6, 4); __PYX_ERR(0, 176, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  5:
         if (likely((values[5] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_dI_dj)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("grape", 1, 6, 6, 5); __PYX_ERR(0, 166, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("grape", 1, 6, 6, 5); __PYX_ERR(0, 176, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "grape") < 0)) __PYX_ERR(0, 166, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "grape") < 0)) __PYX_ERR(0, 176, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 6) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
       values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
       values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
       values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
     }
-    __pyx_v_cs = __Pyx_PyObject_to_MemoryviewSlice_d_dc_double(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_cs.memview)) __PYX_ERR(0, 166, __pyx_L3_error)
-    __pyx_v_U_target = __Pyx_PyObject_to_MemoryviewSlice_d_dc___pyx_t_double_complex(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_U_target.memview)) __PYX_ERR(0, 166, __pyx_L3_error)
-    __pyx_v_target_indexes = __Pyx_PyObject_to_MemoryviewSlice_dc_int(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_target_indexes.memview)) __PYX_ERR(0, 166, __pyx_L3_error)
-    __pyx_v_U = __Pyx_PyObject_to_MemoryviewSlice_d_dc___pyx_t_double_complex(values[3], PyBUF_WRITABLE); if (unlikely(!__pyx_v_U.memview)) __PYX_ERR(0, 166, __pyx_L3_error)
-    __pyx_v_dU = __Pyx_PyObject_to_MemoryviewSlice_d_d_dc___pyx_t_double_complex(values[4], PyBUF_WRITABLE); if (unlikely(!__pyx_v_dU.memview)) __PYX_ERR(0, 166, __pyx_L3_error)
-    __pyx_v_dI_dj = __Pyx_PyObject_to_MemoryviewSlice_d_dc_double(values[5], PyBUF_WRITABLE); if (unlikely(!__pyx_v_dI_dj.memview)) __PYX_ERR(0, 166, __pyx_L3_error)
+    __pyx_v_cs = __Pyx_PyObject_to_MemoryviewSlice_d_dc_double(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_cs.memview)) __PYX_ERR(0, 176, __pyx_L3_error)
+    __pyx_v_U_target = __Pyx_PyObject_to_MemoryviewSlice_d_dc___pyx_t_double_complex(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_U_target.memview)) __PYX_ERR(0, 176, __pyx_L3_error)
+    __pyx_v_target_indexes = __Pyx_PyObject_to_MemoryviewSlice_dc_int(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_target_indexes.memview)) __PYX_ERR(0, 176, __pyx_L3_error)
+    __pyx_v_U = __Pyx_PyObject_to_MemoryviewSlice_d_dc___pyx_t_double_complex(values[3], PyBUF_WRITABLE); if (unlikely(!__pyx_v_U.memview)) __PYX_ERR(0, 176, __pyx_L3_error)
+    __pyx_v_dU = __Pyx_PyObject_to_MemoryviewSlice_d_d_dc___pyx_t_double_complex(values[4], PyBUF_WRITABLE); if (unlikely(!__pyx_v_dU.memview)) __PYX_ERR(0, 176, __pyx_L3_error)
+    __pyx_v_dI_dj = __Pyx_PyObject_to_MemoryviewSlice_d_dc_double(values[5], PyBUF_WRITABLE); if (unlikely(!__pyx_v_dI_dj.memview)) __PYX_ERR(0, 176, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("grape", 1, 6, 6, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 166, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("grape", 1, 6, 6, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 176, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("unipolator.hamiltonian_system.Hamiltonian_System.grape", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_10unipolator_18hamiltonian_system_18Hamiltonian_System_12grape(((struct __pyx_obj_10unipolator_18hamiltonian_system_Hamiltonian_System *)__pyx_v_self), __pyx_v_cs, __pyx_v_U_target, __pyx_v_target_indexes, __pyx_v_U, __pyx_v_dU, __pyx_v_dI_dj);
+  __pyx_r = __pyx_pf_10unipolator_18hamiltonian_system_18Hamiltonian_System_14grape(((struct __pyx_obj_10unipolator_18hamiltonian_system_Hamiltonian_System *)__pyx_v_self), __pyx_v_cs, __pyx_v_U_target, __pyx_v_target_indexes, __pyx_v_U, __pyx_v_dU, __pyx_v_dI_dj);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_10unipolator_18hamiltonian_system_18Hamiltonian_System_12grape(struct __pyx_obj_10unipolator_18hamiltonian_system_Hamiltonian_System *__pyx_v_self, __Pyx_memviewslice __pyx_v_cs, __Pyx_memviewslice __pyx_v_U_target, __Pyx_memviewslice __pyx_v_target_indexes, __Pyx_memviewslice __pyx_v_U, __Pyx_memviewslice __pyx_v_dU, __Pyx_memviewslice __pyx_v_dI_dj) {
+static PyObject *__pyx_pf_10unipolator_18hamiltonian_system_18Hamiltonian_System_14grape(struct __pyx_obj_10unipolator_18hamiltonian_system_Hamiltonian_System *__pyx_v_self, __Pyx_memviewslice __pyx_v_cs, __Pyx_memviewslice __pyx_v_U_target, __Pyx_memviewslice __pyx_v_target_indexes, __Pyx_memviewslice __pyx_v_U, __Pyx_memviewslice __pyx_v_dU, __Pyx_memviewslice __pyx_v_dI_dj) {
   int __pyx_v_i;
   int __pyx_v_j;
   int __pyx_v_steps;
   __pyx_t_double_complex *__pyx_v_new_p0;
   __pyx_t_double_complex *__pyx_v_new_q0;
   __pyx_t_double_complex *__pyx_v_p0;
   __pyx_t_double_complex *__pyx_v_q0;
@@ -5403,278 +5716,278 @@
   int __pyx_t_14;
   __pyx_t_double_complex *__pyx_t_15;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("grape", 0);
 
-  /* "unipolator/hamiltonian_system.pyx":169
+  /* "unipolator/hamiltonian_system.pyx":179
  *         # Calculate fidelity for a pulse and the differentials of the fidelity at every timestep using the grape trick
  *         cdef int i, j
  *         cdef int steps = cs.shape[0]             # <<<<<<<<<<<<<<
  * 
  *         cdef double complex *new_p0 = self.u1
  */
   __pyx_v_steps = (__pyx_v_cs.shape[0]);
 
-  /* "unipolator/hamiltonian_system.pyx":171
+  /* "unipolator/hamiltonian_system.pyx":181
  *         cdef int steps = cs.shape[0]
  * 
  *         cdef double complex *new_p0 = self.u1             # <<<<<<<<<<<<<<
  *         cdef double complex *new_q0 = self.u2
  *         cdef double complex *p0 = self.u4
  */
   __pyx_t_1 = __pyx_v_self->u1;
   __pyx_v_new_p0 = __pyx_t_1;
 
-  /* "unipolator/hamiltonian_system.pyx":172
+  /* "unipolator/hamiltonian_system.pyx":182
  * 
  *         cdef double complex *new_p0 = self.u1
  *         cdef double complex *new_q0 = self.u2             # <<<<<<<<<<<<<<
  *         cdef double complex *p0 = self.u4
  *         cdef double complex *q0 = self.u5
  */
   __pyx_t_1 = __pyx_v_self->u2;
   __pyx_v_new_q0 = __pyx_t_1;
 
-  /* "unipolator/hamiltonian_system.pyx":173
+  /* "unipolator/hamiltonian_system.pyx":183
  *         cdef double complex *new_p0 = self.u1
  *         cdef double complex *new_q0 = self.u2
  *         cdef double complex *p0 = self.u4             # <<<<<<<<<<<<<<
  *         cdef double complex *q0 = self.u5
  *         cdef double complex *u0 = &U[0, 0]
  */
   __pyx_t_1 = __pyx_v_self->u4;
   __pyx_v_p0 = __pyx_t_1;
 
-  /* "unipolator/hamiltonian_system.pyx":174
+  /* "unipolator/hamiltonian_system.pyx":184
  *         cdef double complex *new_q0 = self.u2
  *         cdef double complex *p0 = self.u4
  *         cdef double complex *q0 = self.u5             # <<<<<<<<<<<<<<
  *         cdef double complex *u0 = &U[0, 0]
  *         cdef double complex *u_tar = &U_target[0, 0]
  */
   __pyx_t_1 = __pyx_v_self->u5;
   __pyx_v_q0 = __pyx_t_1;
 
-  /* "unipolator/hamiltonian_system.pyx":175
+  /* "unipolator/hamiltonian_system.pyx":185
  *         cdef double complex *p0 = self.u4
  *         cdef double complex *q0 = self.u5
  *         cdef double complex *u0 = &U[0, 0]             # <<<<<<<<<<<<<<
  *         cdef double complex *u_tar = &U_target[0, 0]
  *         cdef double complex *curr_u = self.u3
  */
   __pyx_t_2 = 0;
   __pyx_t_3 = 0;
   __pyx_v_u0 = (&(*((__pyx_t_double_complex *) ( /* dim=1 */ ((char *) (((__pyx_t_double_complex *) ( /* dim=0 */ (__pyx_v_U.data + __pyx_t_2 * __pyx_v_U.strides[0]) )) + __pyx_t_3)) ))));
 
-  /* "unipolator/hamiltonian_system.pyx":176
+  /* "unipolator/hamiltonian_system.pyx":186
  *         cdef double complex *q0 = self.u5
  *         cdef double complex *u0 = &U[0, 0]
  *         cdef double complex *u_tar = &U_target[0, 0]             # <<<<<<<<<<<<<<
  *         cdef double complex *curr_u = self.u3
  *         cdef double complex *du = &dU[0,0,0]
  */
   __pyx_t_3 = 0;
   __pyx_t_2 = 0;
   __pyx_v_u_tar = (&(*((__pyx_t_double_complex *) ( /* dim=1 */ ((char *) (((__pyx_t_double_complex *) ( /* dim=0 */ (__pyx_v_U_target.data + __pyx_t_3 * __pyx_v_U_target.strides[0]) )) + __pyx_t_2)) ))));
 
-  /* "unipolator/hamiltonian_system.pyx":177
+  /* "unipolator/hamiltonian_system.pyx":187
  *         cdef double complex *u0 = &U[0, 0]
  *         cdef double complex *u_tar = &U_target[0, 0]
  *         cdef double complex *curr_u = self.u3             # <<<<<<<<<<<<<<
  *         cdef double complex *du = &dU[0,0,0]
  * 
  */
   __pyx_t_1 = __pyx_v_self->u3;
   __pyx_v_curr_u = __pyx_t_1;
 
-  /* "unipolator/hamiltonian_system.pyx":178
+  /* "unipolator/hamiltonian_system.pyx":188
  *         cdef double complex *u_tar = &U_target[0, 0]
  *         cdef double complex *curr_u = self.u3
  *         cdef double complex *du = &dU[0,0,0]             # <<<<<<<<<<<<<<
  * 
  *         cdef double complex trM, trdM, two_nni
  */
   __pyx_t_2 = 0;
   __pyx_t_3 = 0;
   __pyx_t_4 = 0;
   __pyx_v_du = (&(*((__pyx_t_double_complex *) ( /* dim=2 */ ((char *) (((__pyx_t_double_complex *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_dU.data + __pyx_t_2 * __pyx_v_dU.strides[0]) ) + __pyx_t_3 * __pyx_v_dU.strides[1]) )) + __pyx_t_4)) ))));
 
-  /* "unipolator/hamiltonian_system.pyx":181
+  /* "unipolator/hamiltonian_system.pyx":191
  * 
  *         cdef double complex trM, trdM, two_nni
  *         cdef double n = <double> target_indexes.shape[0]             # <<<<<<<<<<<<<<
  *         cdef double nni = 1.0 / (n * (n + 1))
  *         cdef double one_minus = 1.0 - n * nni
  */
   __pyx_v_n = ((double)(__pyx_v_target_indexes.shape[0]));
 
-  /* "unipolator/hamiltonian_system.pyx":182
+  /* "unipolator/hamiltonian_system.pyx":192
  *         cdef double complex trM, trdM, two_nni
  *         cdef double n = <double> target_indexes.shape[0]
  *         cdef double nni = 1.0 / (n * (n + 1))             # <<<<<<<<<<<<<<
  *         cdef double one_minus = 1.0 - n * nni
  * 
  */
   __pyx_v_nni = (1.0 / (__pyx_v_n * (__pyx_v_n + 1.0)));
 
-  /* "unipolator/hamiltonian_system.pyx":183
+  /* "unipolator/hamiltonian_system.pyx":193
  *         cdef double n = <double> target_indexes.shape[0]
  *         cdef double nni = 1.0 / (n * (n + 1))
  *         cdef double one_minus = 1.0 - n * nni             # <<<<<<<<<<<<<<
  * 
  *         if not dI_dj.shape[0] == steps:
  */
   __pyx_v_one_minus = (1.0 - (__pyx_v_n * __pyx_v_nni));
 
-  /* "unipolator/hamiltonian_system.pyx":185
+  /* "unipolator/hamiltonian_system.pyx":195
  *         cdef double one_minus = 1.0 - n * nni
  * 
  *         if not dI_dj.shape[0] == steps:             # <<<<<<<<<<<<<<
  *             raise ValueError('Inputs must fulfill: cs.shape[0] = dI_dj.shape[0].')
  *         if not dI_dj.shape[1] == self.n_d_di:
  */
   __pyx_t_5 = ((!(((__pyx_v_dI_dj.shape[0]) == __pyx_v_steps) != 0)) != 0);
   if (unlikely(__pyx_t_5)) {
 
-    /* "unipolator/hamiltonian_system.pyx":186
+    /* "unipolator/hamiltonian_system.pyx":196
  * 
  *         if not dI_dj.shape[0] == steps:
  *             raise ValueError('Inputs must fulfill: cs.shape[0] = dI_dj.shape[0].')             # <<<<<<<<<<<<<<
  *         if not dI_dj.shape[1] == self.n_d_di:
  *             raise ValueError('Inputs must fulfill: which_diffs.shape[0] = dI_dj.shape[1].')
  */
-    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 186, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 196, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_Raise(__pyx_t_6, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __PYX_ERR(0, 186, __pyx_L1_error)
+    __PYX_ERR(0, 196, __pyx_L1_error)
 
-    /* "unipolator/hamiltonian_system.pyx":185
+    /* "unipolator/hamiltonian_system.pyx":195
  *         cdef double one_minus = 1.0 - n * nni
  * 
  *         if not dI_dj.shape[0] == steps:             # <<<<<<<<<<<<<<
  *             raise ValueError('Inputs must fulfill: cs.shape[0] = dI_dj.shape[0].')
  *         if not dI_dj.shape[1] == self.n_d_di:
  */
   }
 
-  /* "unipolator/hamiltonian_system.pyx":187
+  /* "unipolator/hamiltonian_system.pyx":197
  *         if not dI_dj.shape[0] == steps:
  *             raise ValueError('Inputs must fulfill: cs.shape[0] = dI_dj.shape[0].')
  *         if not dI_dj.shape[1] == self.n_d_di:             # <<<<<<<<<<<<<<
  *             raise ValueError('Inputs must fulfill: which_diffs.shape[0] = dI_dj.shape[1].')
  *         if not cs.shape[1] == self.n_d_di:
  */
   __pyx_t_5 = ((!(((__pyx_v_dI_dj.shape[1]) == __pyx_v_self->n_d_di) != 0)) != 0);
   if (unlikely(__pyx_t_5)) {
 
-    /* "unipolator/hamiltonian_system.pyx":188
+    /* "unipolator/hamiltonian_system.pyx":198
  *             raise ValueError('Inputs must fulfill: cs.shape[0] = dI_dj.shape[0].')
  *         if not dI_dj.shape[1] == self.n_d_di:
  *             raise ValueError('Inputs must fulfill: which_diffs.shape[0] = dI_dj.shape[1].')             # <<<<<<<<<<<<<<
  *         if not cs.shape[1] == self.n_d_di:
  *             raise ValueError('Inputs must fulfill: which_diffs.shape[0] = cs.shape[1].')
  */
-    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 188, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 198, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_Raise(__pyx_t_6, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __PYX_ERR(0, 188, __pyx_L1_error)
+    __PYX_ERR(0, 198, __pyx_L1_error)
 
-    /* "unipolator/hamiltonian_system.pyx":187
+    /* "unipolator/hamiltonian_system.pyx":197
  *         if not dI_dj.shape[0] == steps:
  *             raise ValueError('Inputs must fulfill: cs.shape[0] = dI_dj.shape[0].')
  *         if not dI_dj.shape[1] == self.n_d_di:             # <<<<<<<<<<<<<<
  *             raise ValueError('Inputs must fulfill: which_diffs.shape[0] = dI_dj.shape[1].')
  *         if not cs.shape[1] == self.n_d_di:
  */
   }
 
-  /* "unipolator/hamiltonian_system.pyx":189
+  /* "unipolator/hamiltonian_system.pyx":199
  *         if not dI_dj.shape[1] == self.n_d_di:
  *             raise ValueError('Inputs must fulfill: which_diffs.shape[0] = dI_dj.shape[1].')
  *         if not cs.shape[1] == self.n_d_di:             # <<<<<<<<<<<<<<
  *             raise ValueError('Inputs must fulfill: which_diffs.shape[0] = cs.shape[1].')
  *         # Fidelity constants
  */
   __pyx_t_5 = ((!(((__pyx_v_cs.shape[1]) == __pyx_v_self->n_d_di) != 0)) != 0);
   if (unlikely(__pyx_t_5)) {
 
-    /* "unipolator/hamiltonian_system.pyx":190
+    /* "unipolator/hamiltonian_system.pyx":200
  *             raise ValueError('Inputs must fulfill: which_diffs.shape[0] = dI_dj.shape[1].')
  *         if not cs.shape[1] == self.n_d_di:
  *             raise ValueError('Inputs must fulfill: which_diffs.shape[0] = cs.shape[1].')             # <<<<<<<<<<<<<<
  *         # Fidelity constants
  * 
  */
-    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 190, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 200, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_Raise(__pyx_t_6, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __PYX_ERR(0, 190, __pyx_L1_error)
+    __PYX_ERR(0, 200, __pyx_L1_error)
 
-    /* "unipolator/hamiltonian_system.pyx":189
+    /* "unipolator/hamiltonian_system.pyx":199
  *         if not dI_dj.shape[1] == self.n_d_di:
  *             raise ValueError('Inputs must fulfill: which_diffs.shape[0] = dI_dj.shape[1].')
  *         if not cs.shape[1] == self.n_d_di:             # <<<<<<<<<<<<<<
  *             raise ValueError('Inputs must fulfill: which_diffs.shape[0] = cs.shape[1].')
  *         # Fidelity constants
  */
   }
 
-  /* "unipolator/hamiltonian_system.pyx":193
+  /* "unipolator/hamiltonian_system.pyx":203
  *         # Fidelity constants
  * 
  *         self.expmH_pulse_pointer(cs, u0)             # <<<<<<<<<<<<<<
  *         #Dag_fast(U_target, self.Ur3) # -> Ur3 is identical to Q  -> replaced by new approach
  *         DagM_M_cdot_pointer(u_tar, u0, q0, self.d)
  */
-  __pyx_t_6 = ((struct __pyx_vtabstruct_10unipolator_18hamiltonian_system_Hamiltonian_System *)__pyx_v_self->__pyx_vtab)->expmH_pulse_pointer(__pyx_v_self, __pyx_v_cs, __pyx_v_u0, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 193, __pyx_L1_error)
+  __pyx_t_6 = ((struct __pyx_vtabstruct_10unipolator_18hamiltonian_system_Hamiltonian_System *)__pyx_v_self->__pyx_vtab)->expmH_pulse_pointer(__pyx_v_self, __pyx_v_cs, __pyx_v_u0, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 203, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-  /* "unipolator/hamiltonian_system.pyx":195
+  /* "unipolator/hamiltonian_system.pyx":205
  *         self.expmH_pulse_pointer(cs, u0)
  *         #Dag_fast(U_target, self.Ur3) # -> Ur3 is identical to Q  -> replaced by new approach
  *         DagM_M_cdot_pointer(u_tar, u0, q0, self.d)             # <<<<<<<<<<<<<<
  *         trM = target_indexes_trace_pointer(q0, self.d, target_indexes)
  *         two_nni = - 2 / (n * (n + 1)) * conj(trM)
  */
   __pyx_f_10unipolator_14blas_functions_DagM_M_cdot_pointer(__pyx_v_u_tar, __pyx_v_u0, __pyx_v_q0, __pyx_v_self->d);
 
-  /* "unipolator/hamiltonian_system.pyx":196
+  /* "unipolator/hamiltonian_system.pyx":206
  *         #Dag_fast(U_target, self.Ur3) # -> Ur3 is identical to Q  -> replaced by new approach
  *         DagM_M_cdot_pointer(u_tar, u0, q0, self.d)
  *         trM = target_indexes_trace_pointer(q0, self.d, target_indexes)             # <<<<<<<<<<<<<<
  *         two_nni = - 2 / (n * (n + 1)) * conj(trM)
  *         cdef double I0 = one_minus - nni * abs_2(trM) # Sub Fidelity
  */
   __pyx_v_trM = __pyx_f_10unipolator_14blas_functions_target_indexes_trace_pointer(__pyx_v_q0, __pyx_v_self->d, __pyx_v_target_indexes);
 
-  /* "unipolator/hamiltonian_system.pyx":197
+  /* "unipolator/hamiltonian_system.pyx":207
  *         DagM_M_cdot_pointer(u_tar, u0, q0, self.d)
  *         trM = target_indexes_trace_pointer(q0, self.d, target_indexes)
  *         two_nni = - 2 / (n * (n + 1)) * conj(trM)             # <<<<<<<<<<<<<<
  *         cdef double I0 = one_minus - nni * abs_2(trM) # Sub Fidelity
  * 
  */
   __pyx_v_two_nni = __Pyx_c_prod_double(__pyx_t_double_complex_from_parts((-2.0 / (__pyx_v_n * (__pyx_v_n + 1.0))), 0), __pyx_f_10unipolator_11exp_and_log_conj(__pyx_v_trM));
 
-  /* "unipolator/hamiltonian_system.pyx":198
+  /* "unipolator/hamiltonian_system.pyx":208
  *         trM = target_indexes_trace_pointer(q0, self.d, target_indexes)
  *         two_nni = - 2 / (n * (n + 1)) * conj(trM)
  *         cdef double I0 = one_minus - nni * abs_2(trM) # Sub Fidelity             # <<<<<<<<<<<<<<
  * 
  *         # Do GRAPE trick
  */
   __pyx_v_I0 = (__pyx_v_one_minus - (__pyx_v_nni * __pyx_f_10unipolator_11exp_and_log_abs_2(__pyx_v_trM, 0)));
 
-  /* "unipolator/hamiltonian_system.pyx":201
+  /* "unipolator/hamiltonian_system.pyx":211
  * 
  *         # Do GRAPE trick
  *         self.dexpmH_pointer(cs[0,:], curr_u, du) # Calculate Unitary and its derivatives             # <<<<<<<<<<<<<<
  *         M_DagM_cdot_pointer(q0, curr_u, new_q0, self.d)  # Reduce q0
  *         copy_pointer(new_q0, q0, self.d2)
  */
   __pyx_t_7.data = __pyx_v_cs.data;
@@ -5686,113 +5999,113 @@
         __pyx_t_7.data += __pyx_tmp_idx * __pyx_tmp_stride;
 }
 
 __pyx_t_7.shape[0] = __pyx_v_cs.shape[1];
 __pyx_t_7.strides[0] = __pyx_v_cs.strides[1];
     __pyx_t_7.suboffsets[0] = -1;
 
-__pyx_t_6 = ((struct __pyx_vtabstruct_10unipolator_18hamiltonian_system_Hamiltonian_System *)__pyx_v_self->__pyx_vtab)->dexpmH_pointer(__pyx_v_self, __pyx_t_7, __pyx_v_curr_u, __pyx_v_du, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 201, __pyx_L1_error)
+__pyx_t_6 = ((struct __pyx_vtabstruct_10unipolator_18hamiltonian_system_Hamiltonian_System *)__pyx_v_self->__pyx_vtab)->dexpmH_pointer(__pyx_v_self, __pyx_t_7, __pyx_v_curr_u, __pyx_v_du, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 211, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __PYX_XDEC_MEMVIEW(&__pyx_t_7, 1);
   __pyx_t_7.memview = NULL;
   __pyx_t_7.data = NULL;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-  /* "unipolator/hamiltonian_system.pyx":202
+  /* "unipolator/hamiltonian_system.pyx":212
  *         # Do GRAPE trick
  *         self.dexpmH_pointer(cs[0,:], curr_u, du) # Calculate Unitary and its derivatives
  *         M_DagM_cdot_pointer(q0, curr_u, new_q0, self.d)  # Reduce q0             # <<<<<<<<<<<<<<
  *         copy_pointer(new_q0, q0, self.d2)
  *         for j in range(self.n_d_di):
  */
   __pyx_f_10unipolator_14blas_functions_M_DagM_cdot_pointer(__pyx_v_q0, __pyx_v_curr_u, __pyx_v_new_q0, __pyx_v_self->d);
 
-  /* "unipolator/hamiltonian_system.pyx":203
+  /* "unipolator/hamiltonian_system.pyx":213
  *         self.dexpmH_pointer(cs[0,:], curr_u, du) # Calculate Unitary and its derivatives
  *         M_DagM_cdot_pointer(q0, curr_u, new_q0, self.d)  # Reduce q0
  *         copy_pointer(new_q0, q0, self.d2)             # <<<<<<<<<<<<<<
  *         for j in range(self.n_d_di):
  *             #MM_cdot_pointer(curr_du, p0, new_p0, self.d)  # p0 is not defined yet
  */
   __pyx_f_10unipolator_11exp_and_log_copy_pointer(__pyx_v_new_q0, __pyx_v_q0, __pyx_v_self->d2);
 
-  /* "unipolator/hamiltonian_system.pyx":204
+  /* "unipolator/hamiltonian_system.pyx":214
  *         M_DagM_cdot_pointer(q0, curr_u, new_q0, self.d)  # Reduce q0
  *         copy_pointer(new_q0, q0, self.d2)
  *         for j in range(self.n_d_di):             # <<<<<<<<<<<<<<
  *             #MM_cdot_pointer(curr_du, p0, new_p0, self.d)  # p0 is not defined yet
  *             trdM = tr_dot_pointer_target_indexes(q0, du, self.d, target_indexes)
  */
   __pyx_t_8 = __pyx_v_self->n_d_di;
   __pyx_t_9 = __pyx_t_8;
   for (__pyx_t_10 = 0; __pyx_t_10 < __pyx_t_9; __pyx_t_10+=1) {
     __pyx_v_j = __pyx_t_10;
 
-    /* "unipolator/hamiltonian_system.pyx":206
+    /* "unipolator/hamiltonian_system.pyx":216
  *         for j in range(self.n_d_di):
  *             #MM_cdot_pointer(curr_du, p0, new_p0, self.d)  # p0 is not defined yet
  *             trdM = tr_dot_pointer_target_indexes(q0, du, self.d, target_indexes)             # <<<<<<<<<<<<<<
  *             dI_dj[0, j] = ( two_nni * trdM ).real
  *             du += self.d2
  */
     __pyx_v_trdM = __pyx_f_10unipolator_14blas_functions_tr_dot_pointer_target_indexes(__pyx_v_q0, __pyx_v_du, __pyx_v_self->d, __pyx_v_target_indexes);
 
-    /* "unipolator/hamiltonian_system.pyx":207
+    /* "unipolator/hamiltonian_system.pyx":217
  *             #MM_cdot_pointer(curr_du, p0, new_p0, self.d)  # p0 is not defined yet
  *             trdM = tr_dot_pointer_target_indexes(q0, du, self.d, target_indexes)
  *             dI_dj[0, j] = ( two_nni * trdM ).real             # <<<<<<<<<<<<<<
  *             du += self.d2
  *         copy_pointer(curr_u, p0, self.d2)  # Define p0 from curr_u
  */
     __pyx_t_11 = __Pyx_CREAL(__Pyx_c_prod_double(__pyx_v_two_nni, __pyx_v_trdM));
     __pyx_t_4 = 0;
     __pyx_t_3 = __pyx_v_j;
     *((double *) ( /* dim=1 */ ((char *) (((double *) ( /* dim=0 */ (__pyx_v_dI_dj.data + __pyx_t_4 * __pyx_v_dI_dj.strides[0]) )) + __pyx_t_3)) )) = __pyx_t_11;
 
-    /* "unipolator/hamiltonian_system.pyx":208
+    /* "unipolator/hamiltonian_system.pyx":218
  *             trdM = tr_dot_pointer_target_indexes(q0, du, self.d, target_indexes)
  *             dI_dj[0, j] = ( two_nni * trdM ).real
  *             du += self.d2             # <<<<<<<<<<<<<<
  *         copy_pointer(curr_u, p0, self.d2)  # Define p0 from curr_u
  *         for i in range(1, steps):
  */
     __pyx_v_du = (__pyx_v_du + __pyx_v_self->d2);
   }
 
-  /* "unipolator/hamiltonian_system.pyx":209
+  /* "unipolator/hamiltonian_system.pyx":219
  *             dI_dj[0, j] = ( two_nni * trdM ).real
  *             du += self.d2
  *         copy_pointer(curr_u, p0, self.d2)  # Define p0 from curr_u             # <<<<<<<<<<<<<<
  *         for i in range(1, steps):
  *             du -= self.d2 * self.n_d_di
  */
   __pyx_f_10unipolator_11exp_and_log_copy_pointer(__pyx_v_curr_u, __pyx_v_p0, __pyx_v_self->d2);
 
-  /* "unipolator/hamiltonian_system.pyx":210
+  /* "unipolator/hamiltonian_system.pyx":220
  *             du += self.d2
  *         copy_pointer(curr_u, p0, self.d2)  # Define p0 from curr_u
  *         for i in range(1, steps):             # <<<<<<<<<<<<<<
  *             du -= self.d2 * self.n_d_di
  *             self.dexpmH_pointer(cs[i, :], curr_u, du)  # Calculate Unitary and its derivatives
  */
   __pyx_t_8 = __pyx_v_steps;
   __pyx_t_9 = __pyx_t_8;
   for (__pyx_t_10 = 1; __pyx_t_10 < __pyx_t_9; __pyx_t_10+=1) {
     __pyx_v_i = __pyx_t_10;
 
-    /* "unipolator/hamiltonian_system.pyx":211
+    /* "unipolator/hamiltonian_system.pyx":221
  *         copy_pointer(curr_u, p0, self.d2)  # Define p0 from curr_u
  *         for i in range(1, steps):
  *             du -= self.d2 * self.n_d_di             # <<<<<<<<<<<<<<
  *             self.dexpmH_pointer(cs[i, :], curr_u, du)  # Calculate Unitary and its derivatives
  *             M_DagM_cdot_pointer(q0, curr_u, new_q0, self.d)  # Remove current unitary (curr_u) from Q
  */
     __pyx_v_du = (__pyx_v_du - (__pyx_v_self->d2 * __pyx_v_self->n_d_di));
 
-    /* "unipolator/hamiltonian_system.pyx":212
+    /* "unipolator/hamiltonian_system.pyx":222
  *         for i in range(1, steps):
  *             du -= self.d2 * self.n_d_di
  *             self.dexpmH_pointer(cs[i, :], curr_u, du)  # Calculate Unitary and its derivatives             # <<<<<<<<<<<<<<
  *             M_DagM_cdot_pointer(q0, curr_u, new_q0, self.d)  # Remove current unitary (curr_u) from Q
  *             for j in range(self.n_d_di):
  */
     __pyx_t_7.data = __pyx_v_cs.data;
@@ -5804,154 +6117,154 @@
         __pyx_t_7.data += __pyx_tmp_idx * __pyx_tmp_stride;
 }
 
 __pyx_t_7.shape[0] = __pyx_v_cs.shape[1];
 __pyx_t_7.strides[0] = __pyx_v_cs.strides[1];
     __pyx_t_7.suboffsets[0] = -1;
 
-__pyx_t_6 = ((struct __pyx_vtabstruct_10unipolator_18hamiltonian_system_Hamiltonian_System *)__pyx_v_self->__pyx_vtab)->dexpmH_pointer(__pyx_v_self, __pyx_t_7, __pyx_v_curr_u, __pyx_v_du, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 212, __pyx_L1_error)
+__pyx_t_6 = ((struct __pyx_vtabstruct_10unipolator_18hamiltonian_system_Hamiltonian_System *)__pyx_v_self->__pyx_vtab)->dexpmH_pointer(__pyx_v_self, __pyx_t_7, __pyx_v_curr_u, __pyx_v_du, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 222, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __PYX_XDEC_MEMVIEW(&__pyx_t_7, 1);
     __pyx_t_7.memview = NULL;
     __pyx_t_7.data = NULL;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-    /* "unipolator/hamiltonian_system.pyx":213
+    /* "unipolator/hamiltonian_system.pyx":223
  *             du -= self.d2 * self.n_d_di
  *             self.dexpmH_pointer(cs[i, :], curr_u, du)  # Calculate Unitary and its derivatives
  *             M_DagM_cdot_pointer(q0, curr_u, new_q0, self.d)  # Remove current unitary (curr_u) from Q             # <<<<<<<<<<<<<<
  *             for j in range(self.n_d_di):
  *                 MM_cdot_pointer(du, p0, new_p0, self.d)
  */
     __pyx_f_10unipolator_14blas_functions_M_DagM_cdot_pointer(__pyx_v_q0, __pyx_v_curr_u, __pyx_v_new_q0, __pyx_v_self->d);
 
-    /* "unipolator/hamiltonian_system.pyx":214
+    /* "unipolator/hamiltonian_system.pyx":224
  *             self.dexpmH_pointer(cs[i, :], curr_u, du)  # Calculate Unitary and its derivatives
  *             M_DagM_cdot_pointer(q0, curr_u, new_q0, self.d)  # Remove current unitary (curr_u) from Q
  *             for j in range(self.n_d_di):             # <<<<<<<<<<<<<<
  *                 MM_cdot_pointer(du, p0, new_p0, self.d)
  *                 trdM = tr_dot_pointer_target_indexes(new_q0, new_p0, self.d, target_indexes)
  */
     __pyx_t_12 = __pyx_v_self->n_d_di;
     __pyx_t_13 = __pyx_t_12;
     for (__pyx_t_14 = 0; __pyx_t_14 < __pyx_t_13; __pyx_t_14+=1) {
       __pyx_v_j = __pyx_t_14;
 
-      /* "unipolator/hamiltonian_system.pyx":215
+      /* "unipolator/hamiltonian_system.pyx":225
  *             M_DagM_cdot_pointer(q0, curr_u, new_q0, self.d)  # Remove current unitary (curr_u) from Q
  *             for j in range(self.n_d_di):
  *                 MM_cdot_pointer(du, p0, new_p0, self.d)             # <<<<<<<<<<<<<<
  *                 trdM = tr_dot_pointer_target_indexes(new_q0, new_p0, self.d, target_indexes)
  *                 dI_dj[i, j] = ( two_nni * trdM ).real
  */
       __pyx_f_10unipolator_14blas_functions_MM_cdot_pointer(__pyx_v_du, __pyx_v_p0, __pyx_v_new_p0, __pyx_v_self->d);
 
-      /* "unipolator/hamiltonian_system.pyx":216
+      /* "unipolator/hamiltonian_system.pyx":226
  *             for j in range(self.n_d_di):
  *                 MM_cdot_pointer(du, p0, new_p0, self.d)
  *                 trdM = tr_dot_pointer_target_indexes(new_q0, new_p0, self.d, target_indexes)             # <<<<<<<<<<<<<<
  *                 dI_dj[i, j] = ( two_nni * trdM ).real
  *                 du += self.d2
  */
       __pyx_v_trdM = __pyx_f_10unipolator_14blas_functions_tr_dot_pointer_target_indexes(__pyx_v_new_q0, __pyx_v_new_p0, __pyx_v_self->d, __pyx_v_target_indexes);
 
-      /* "unipolator/hamiltonian_system.pyx":217
+      /* "unipolator/hamiltonian_system.pyx":227
  *                 MM_cdot_pointer(du, p0, new_p0, self.d)
  *                 trdM = tr_dot_pointer_target_indexes(new_q0, new_p0, self.d, target_indexes)
  *                 dI_dj[i, j] = ( two_nni * trdM ).real             # <<<<<<<<<<<<<<
  *                 du += self.d2
  *             MM_cdot_pointer(curr_u, p0, new_p0, self.d)  # Add current unitary (curr_u) to P
  */
       __pyx_t_11 = __Pyx_CREAL(__Pyx_c_prod_double(__pyx_v_two_nni, __pyx_v_trdM));
       __pyx_t_3 = __pyx_v_i;
       __pyx_t_4 = __pyx_v_j;
       *((double *) ( /* dim=1 */ ((char *) (((double *) ( /* dim=0 */ (__pyx_v_dI_dj.data + __pyx_t_3 * __pyx_v_dI_dj.strides[0]) )) + __pyx_t_4)) )) = __pyx_t_11;
 
-      /* "unipolator/hamiltonian_system.pyx":218
+      /* "unipolator/hamiltonian_system.pyx":228
  *                 trdM = tr_dot_pointer_target_indexes(new_q0, new_p0, self.d, target_indexes)
  *                 dI_dj[i, j] = ( two_nni * trdM ).real
  *                 du += self.d2             # <<<<<<<<<<<<<<
  *             MM_cdot_pointer(curr_u, p0, new_p0, self.d)  # Add current unitary (curr_u) to P
  *             # flip pointers
  */
       __pyx_v_du = (__pyx_v_du + __pyx_v_self->d2);
     }
 
-    /* "unipolator/hamiltonian_system.pyx":219
+    /* "unipolator/hamiltonian_system.pyx":229
  *                 dI_dj[i, j] = ( two_nni * trdM ).real
  *                 du += self.d2
  *             MM_cdot_pointer(curr_u, p0, new_p0, self.d)  # Add current unitary (curr_u) to P             # <<<<<<<<<<<<<<
  *             # flip pointers
  *             self.u1, self.u4 = self.u4, self.u1
  */
     __pyx_f_10unipolator_14blas_functions_MM_cdot_pointer(__pyx_v_curr_u, __pyx_v_p0, __pyx_v_new_p0, __pyx_v_self->d);
 
-    /* "unipolator/hamiltonian_system.pyx":221
+    /* "unipolator/hamiltonian_system.pyx":231
  *             MM_cdot_pointer(curr_u, p0, new_p0, self.d)  # Add current unitary (curr_u) to P
  *             # flip pointers
  *             self.u1, self.u4 = self.u4, self.u1             # <<<<<<<<<<<<<<
  *             self.u2, self.u5 = self.u5, self.u2
  *             new_p0, p0 = p0, new_p0
  */
     __pyx_t_1 = __pyx_v_self->u4;
     __pyx_t_15 = __pyx_v_self->u1;
     __pyx_v_self->u1 = __pyx_t_1;
     __pyx_v_self->u4 = __pyx_t_15;
 
-    /* "unipolator/hamiltonian_system.pyx":222
+    /* "unipolator/hamiltonian_system.pyx":232
  *             # flip pointers
  *             self.u1, self.u4 = self.u4, self.u1
  *             self.u2, self.u5 = self.u5, self.u2             # <<<<<<<<<<<<<<
  *             new_p0, p0 = p0, new_p0
  *             new_q0, q0 = q0, new_q0
  */
     __pyx_t_15 = __pyx_v_self->u5;
     __pyx_t_1 = __pyx_v_self->u2;
     __pyx_v_self->u2 = __pyx_t_15;
     __pyx_v_self->u5 = __pyx_t_1;
 
-    /* "unipolator/hamiltonian_system.pyx":223
+    /* "unipolator/hamiltonian_system.pyx":233
  *             self.u1, self.u4 = self.u4, self.u1
  *             self.u2, self.u5 = self.u5, self.u2
  *             new_p0, p0 = p0, new_p0             # <<<<<<<<<<<<<<
  *             new_q0, q0 = q0, new_q0
  *         return I0
  */
     __pyx_t_1 = __pyx_v_p0;
     __pyx_t_15 = __pyx_v_new_p0;
     __pyx_v_new_p0 = __pyx_t_1;
     __pyx_v_p0 = __pyx_t_15;
 
-    /* "unipolator/hamiltonian_system.pyx":224
+    /* "unipolator/hamiltonian_system.pyx":234
  *             self.u2, self.u5 = self.u5, self.u2
  *             new_p0, p0 = p0, new_p0
  *             new_q0, q0 = q0, new_q0             # <<<<<<<<<<<<<<
  *         return I0
  * 
  */
     __pyx_t_15 = __pyx_v_q0;
     __pyx_t_1 = __pyx_v_new_q0;
     __pyx_v_new_q0 = __pyx_t_15;
     __pyx_v_q0 = __pyx_t_1;
   }
 
-  /* "unipolator/hamiltonian_system.pyx":225
+  /* "unipolator/hamiltonian_system.pyx":235
  *             new_p0, p0 = p0, new_p0
  *             new_q0, q0 = q0, new_q0
  *         return I0             # <<<<<<<<<<<<<<
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_6 = PyFloat_FromDouble(__pyx_v_I0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 225, __pyx_L1_error)
+  __pyx_t_6 = PyFloat_FromDouble(__pyx_v_I0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 235, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_r = __pyx_t_6;
   __pyx_t_6 = 0;
   goto __pyx_L0;
 
-  /* "unipolator/hamiltonian_system.pyx":166
+  /* "unipolator/hamiltonian_system.pyx":176
  *         self.expmH_pulse_pointer(cs, u0, dt)
  * 
  *     def grape(self, double[:,::1] cs, double complex[:,::1] U_target, int[::1] target_indexes, double complex[:,::1] U, double complex[:,:,::1] dU, double[:,::1] dI_dj):             # <<<<<<<<<<<<<<
  *         # Calculate fidelity for a pulse and the differentials of the fidelity at every timestep using the grape trick
  *         cdef int i, j
  */
 
@@ -5976,28 +6289,28 @@
 /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_10unipolator_18hamiltonian_system_18Hamiltonian_System_15__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static char __pyx_doc_10unipolator_18hamiltonian_system_18Hamiltonian_System_14__reduce_cython__[] = "Hamiltonian_System.__reduce_cython__(self)";
-static PyObject *__pyx_pw_10unipolator_18hamiltonian_system_18Hamiltonian_System_15__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_10unipolator_18hamiltonian_system_18Hamiltonian_System_17__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc_10unipolator_18hamiltonian_system_18Hamiltonian_System_16__reduce_cython__[] = "Hamiltonian_System.__reduce_cython__(self)";
+static PyObject *__pyx_pw_10unipolator_18hamiltonian_system_18Hamiltonian_System_17__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_10unipolator_18hamiltonian_system_18Hamiltonian_System_14__reduce_cython__(((struct __pyx_obj_10unipolator_18hamiltonian_system_Hamiltonian_System *)__pyx_v_self));
+  __pyx_r = __pyx_pf_10unipolator_18hamiltonian_system_18Hamiltonian_System_16__reduce_cython__(((struct __pyx_obj_10unipolator_18hamiltonian_system_Hamiltonian_System *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_10unipolator_18hamiltonian_system_18Hamiltonian_System_14__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_10unipolator_18hamiltonian_system_Hamiltonian_System *__pyx_v_self) {
+static PyObject *__pyx_pf_10unipolator_18hamiltonian_system_18Hamiltonian_System_16__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_10unipolator_18hamiltonian_system_Hamiltonian_System *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__reduce_cython__", 0);
@@ -6034,28 +6347,28 @@
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_10unipolator_18hamiltonian_system_18Hamiltonian_System_17__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
-static char __pyx_doc_10unipolator_18hamiltonian_system_18Hamiltonian_System_16__setstate_cython__[] = "Hamiltonian_System.__setstate_cython__(self, __pyx_state)";
-static PyObject *__pyx_pw_10unipolator_18hamiltonian_system_18Hamiltonian_System_17__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pw_10unipolator_18hamiltonian_system_18Hamiltonian_System_19__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
+static char __pyx_doc_10unipolator_18hamiltonian_system_18Hamiltonian_System_18__setstate_cython__[] = "Hamiltonian_System.__setstate_cython__(self, __pyx_state)";
+static PyObject *__pyx_pw_10unipolator_18hamiltonian_system_18Hamiltonian_System_19__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_10unipolator_18hamiltonian_system_18Hamiltonian_System_16__setstate_cython__(((struct __pyx_obj_10unipolator_18hamiltonian_system_Hamiltonian_System *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
+  __pyx_r = __pyx_pf_10unipolator_18hamiltonian_system_18Hamiltonian_System_18__setstate_cython__(((struct __pyx_obj_10unipolator_18hamiltonian_system_Hamiltonian_System *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_10unipolator_18hamiltonian_system_18Hamiltonian_System_16__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_10unipolator_18hamiltonian_system_Hamiltonian_System *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pf_10unipolator_18hamiltonian_system_18Hamiltonian_System_18__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_10unipolator_18hamiltonian_system_Hamiltonian_System *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
@@ -20214,19 +20527,20 @@
   (*Py_TYPE(o)->tp_free)(o);
 }
 
 static PyMethodDef __pyx_methods_10unipolator_18hamiltonian_system_Hamiltonian_System[] = {
   {"set_which_diffs", (PyCFunction)__pyx_pw_10unipolator_18hamiltonian_system_18Hamiltonian_System_3set_which_diffs, METH_O, __pyx_doc_10unipolator_18hamiltonian_system_18Hamiltonian_System_2set_which_diffs},
   {"get_which_diffs", (PyCFunction)__pyx_pw_10unipolator_18hamiltonian_system_18Hamiltonian_System_5get_which_diffs, METH_NOARGS, __pyx_doc_10unipolator_18hamiltonian_system_18Hamiltonian_System_4get_which_diffs},
   {"expmH", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_10unipolator_18hamiltonian_system_18Hamiltonian_System_7expmH, METH_VARARGS|METH_KEYWORDS, __pyx_doc_10unipolator_18hamiltonian_system_18Hamiltonian_System_6expmH},
-  {"dexpmH", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_10unipolator_18hamiltonian_system_18Hamiltonian_System_9dexpmH, METH_VARARGS|METH_KEYWORDS, __pyx_doc_10unipolator_18hamiltonian_system_18Hamiltonian_System_8dexpmH},
-  {"expmH_pulse", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_10unipolator_18hamiltonian_system_18Hamiltonian_System_11expmH_pulse, METH_VARARGS|METH_KEYWORDS, __pyx_doc_10unipolator_18hamiltonian_system_18Hamiltonian_System_10expmH_pulse},
-  {"grape", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_10unipolator_18hamiltonian_system_18Hamiltonian_System_13grape, METH_VARARGS|METH_KEYWORDS, __pyx_doc_10unipolator_18hamiltonian_system_18Hamiltonian_System_12grape},
-  {"__reduce_cython__", (PyCFunction)__pyx_pw_10unipolator_18hamiltonian_system_18Hamiltonian_System_15__reduce_cython__, METH_NOARGS, __pyx_doc_10unipolator_18hamiltonian_system_18Hamiltonian_System_14__reduce_cython__},
-  {"__setstate_cython__", (PyCFunction)__pyx_pw_10unipolator_18hamiltonian_system_18Hamiltonian_System_17__setstate_cython__, METH_O, __pyx_doc_10unipolator_18hamiltonian_system_18Hamiltonian_System_16__setstate_cython__},
+  {"expmH_pulse_no_multiply", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_10unipolator_18hamiltonian_system_18Hamiltonian_System_9expmH_pulse_no_multiply, METH_VARARGS|METH_KEYWORDS, __pyx_doc_10unipolator_18hamiltonian_system_18Hamiltonian_System_8expmH_pulse_no_multiply},
+  {"dexpmH", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_10unipolator_18hamiltonian_system_18Hamiltonian_System_11dexpmH, METH_VARARGS|METH_KEYWORDS, __pyx_doc_10unipolator_18hamiltonian_system_18Hamiltonian_System_10dexpmH},
+  {"expmH_pulse", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_10unipolator_18hamiltonian_system_18Hamiltonian_System_13expmH_pulse, METH_VARARGS|METH_KEYWORDS, __pyx_doc_10unipolator_18hamiltonian_system_18Hamiltonian_System_12expmH_pulse},
+  {"grape", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_10unipolator_18hamiltonian_system_18Hamiltonian_System_15grape, METH_VARARGS|METH_KEYWORDS, __pyx_doc_10unipolator_18hamiltonian_system_18Hamiltonian_System_14grape},
+  {"__reduce_cython__", (PyCFunction)__pyx_pw_10unipolator_18hamiltonian_system_18Hamiltonian_System_17__reduce_cython__, METH_NOARGS, __pyx_doc_10unipolator_18hamiltonian_system_18Hamiltonian_System_16__reduce_cython__},
+  {"__setstate_cython__", (PyCFunction)__pyx_pw_10unipolator_18hamiltonian_system_18Hamiltonian_System_19__setstate_cython__, METH_O, __pyx_doc_10unipolator_18hamiltonian_system_18Hamiltonian_System_18__setstate_cython__},
   {0, 0, 0, 0}
 };
 
 static PyTypeObject __pyx_type_10unipolator_18hamiltonian_system_Hamiltonian_System = {
   PyVarObject_HEAD_INIT(0, 0)
   "unipolator.hamiltonian_system.Hamiltonian_System", /*tp_name*/
   sizeof(struct __pyx_obj_10unipolator_18hamiltonian_system_Hamiltonian_System), /*tp_basicsize*/
@@ -21186,15 +21500,15 @@
   {&__pyx_n_s_unpack, __pyx_k_unpack, sizeof(__pyx_k_unpack), 0, 0, 1, 1},
   {&__pyx_n_s_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 0, 1, 1},
   {&__pyx_n_s_which_diffs, __pyx_k_which_diffs, sizeof(__pyx_k_which_diffs), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 97, __pyx_L1_error)
-  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 104, __pyx_L1_error)
+  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 111, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(1, 2, __pyx_L1_error)
   __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(2, 945, __pyx_L1_error)
   __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(1, 149, __pyx_L1_error)
   __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(1, 152, __pyx_L1_error)
   __pyx_builtin_Ellipsis = __Pyx_GetBuiltinName(__pyx_n_s_Ellipsis); if (!__pyx_builtin_Ellipsis) __PYX_ERR(1, 406, __pyx_L1_error)
   __pyx_builtin_id = __Pyx_GetBuiltinName(__pyx_n_s_id); if (!__pyx_builtin_id) __PYX_ERR(1, 615, __pyx_L1_error)
   __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(1, 834, __pyx_L1_error)
@@ -21203,77 +21517,77 @@
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "unipolator/hamiltonian_system.pyx":104
+  /* "unipolator/hamiltonian_system.pyx":111
  *         # Construct Hamiltonian
  *         if not c.shape[0] == self.n_dims_1:
  *             raise ValueError('c.shape[0] needs to be equal to H_s[0].shape[0]-1.')             # <<<<<<<<<<<<<<
  *         cdef double complex *u0 = &U[0,0]
- *         self.weighted_hamiltonian(c)
+ *         self.expmH_pointer(c, u0, dt)
  */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_c_shape_0_needs_to_be_equal_to_H); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 104, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_c_shape_0_needs_to_be_equal_to_H); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 111, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
-  /* "unipolator/hamiltonian_system.pyx":140
+  /* "unipolator/hamiltonian_system.pyx":150
  *         cdef double complex *du0 = &dU[0,0,0]
  *         if not c.shape[0] == self.n_dims_1:
  *             raise ValueError('The coefficient c must be of size [interpolation_dimensions].')             # <<<<<<<<<<<<<<
  *         if not self.d_di.shape[0] == dU.shape[0]:
  *             raise ValueError('Inputs must fulfill: which_diffs.shape[0] = dU.shape[0].')
  */
-  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_u_The_coefficient_c_must_be_of_siz); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 140, __pyx_L1_error)
+  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_u_The_coefficient_c_must_be_of_siz); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 150, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
 
-  /* "unipolator/hamiltonian_system.pyx":142
+  /* "unipolator/hamiltonian_system.pyx":152
  *             raise ValueError('The coefficient c must be of size [interpolation_dimensions].')
  *         if not self.d_di.shape[0] == dU.shape[0]:
  *             raise ValueError('Inputs must fulfill: which_diffs.shape[0] = dU.shape[0].')             # <<<<<<<<<<<<<<
  *         self.dexpmH_pointer(c, u0, du0, dt)
  * 
  */
-  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_u_Inputs_must_fulfill_which_diffs); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 142, __pyx_L1_error)
+  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_u_Inputs_must_fulfill_which_diffs); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 152, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
 
-  /* "unipolator/hamiltonian_system.pyx":186
+  /* "unipolator/hamiltonian_system.pyx":196
  * 
  *         if not dI_dj.shape[0] == steps:
  *             raise ValueError('Inputs must fulfill: cs.shape[0] = dI_dj.shape[0].')             # <<<<<<<<<<<<<<
  *         if not dI_dj.shape[1] == self.n_d_di:
  *             raise ValueError('Inputs must fulfill: which_diffs.shape[0] = dI_dj.shape[1].')
  */
-  __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_u_Inputs_must_fulfill_cs_shape_0_d); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 186, __pyx_L1_error)
+  __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_u_Inputs_must_fulfill_cs_shape_0_d); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 196, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__5);
   __Pyx_GIVEREF(__pyx_tuple__5);
 
-  /* "unipolator/hamiltonian_system.pyx":188
+  /* "unipolator/hamiltonian_system.pyx":198
  *             raise ValueError('Inputs must fulfill: cs.shape[0] = dI_dj.shape[0].')
  *         if not dI_dj.shape[1] == self.n_d_di:
  *             raise ValueError('Inputs must fulfill: which_diffs.shape[0] = dI_dj.shape[1].')             # <<<<<<<<<<<<<<
  *         if not cs.shape[1] == self.n_d_di:
  *             raise ValueError('Inputs must fulfill: which_diffs.shape[0] = cs.shape[1].')
  */
-  __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_u_Inputs_must_fulfill_which_diffs_2); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_u_Inputs_must_fulfill_which_diffs_2); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 198, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__6);
   __Pyx_GIVEREF(__pyx_tuple__6);
 
-  /* "unipolator/hamiltonian_system.pyx":190
+  /* "unipolator/hamiltonian_system.pyx":200
  *             raise ValueError('Inputs must fulfill: which_diffs.shape[0] = dI_dj.shape[1].')
  *         if not cs.shape[1] == self.n_d_di:
  *             raise ValueError('Inputs must fulfill: which_diffs.shape[0] = cs.shape[1].')             # <<<<<<<<<<<<<<
  *         # Fidelity constants
  * 
  */
-  __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_u_Inputs_must_fulfill_which_diffs_3); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 190, __pyx_L1_error)
+  __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_u_Inputs_must_fulfill_which_diffs_3); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 200, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__7);
   __Pyx_GIVEREF(__pyx_tuple__7);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
@@ -21636,14 +21950,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
   __pyx_vtabptr_10unipolator_18hamiltonian_system_Hamiltonian_System = &__pyx_vtable_10unipolator_18hamiltonian_system_Hamiltonian_System;
   __pyx_vtable_10unipolator_18hamiltonian_system_Hamiltonian_System.weighted_hamiltonian = (PyObject *(*)(struct __pyx_obj_10unipolator_18hamiltonian_system_Hamiltonian_System *, __Pyx_memviewslice))__pyx_f_10unipolator_18hamiltonian_system_18Hamiltonian_System_weighted_hamiltonian;
+  __pyx_vtable_10unipolator_18hamiltonian_system_Hamiltonian_System.expmH_pointer = (PyObject *(*)(struct __pyx_obj_10unipolator_18hamiltonian_system_Hamiltonian_System *, __Pyx_memviewslice, __pyx_t_double_complex *, double))__pyx_f_10unipolator_18hamiltonian_system_18Hamiltonian_System_expmH_pointer;
   __pyx_vtable_10unipolator_18hamiltonian_system_Hamiltonian_System.dexpmH_pointer = (PyObject *(*)(struct __pyx_obj_10unipolator_18hamiltonian_system_Hamiltonian_System *, __Pyx_memviewslice, __pyx_t_double_complex *, __pyx_t_double_complex *, struct __pyx_opt_args_10unipolator_18hamiltonian_system_18Hamiltonian_System_dexpmH_pointer *__pyx_optional_args))__pyx_f_10unipolator_18hamiltonian_system_18Hamiltonian_System_dexpmH_pointer;
   __pyx_vtable_10unipolator_18hamiltonian_system_Hamiltonian_System.expmH_pulse_pointer = (PyObject *(*)(struct __pyx_obj_10unipolator_18hamiltonian_system_Hamiltonian_System *, __Pyx_memviewslice, __pyx_t_double_complex *, struct __pyx_opt_args_10unipolator_18hamiltonian_system_18Hamiltonian_System_expmH_pulse_pointer *__pyx_optional_args))__pyx_f_10unipolator_18hamiltonian_system_18Hamiltonian_System_expmH_pulse_pointer;
   if (PyType_Ready(&__pyx_type_10unipolator_18hamiltonian_system_Hamiltonian_System) < 0) __PYX_ERR(0, 11, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_10unipolator_18hamiltonian_system_Hamiltonian_System.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_10unipolator_18hamiltonian_system_Hamiltonian_System.tp_dictoffset && __pyx_type_10unipolator_18hamiltonian_system_Hamiltonian_System.tp_getattro == PyObject_GenericGetAttr)) {
```

### Comparing `unipolator-0.2.6/src/unipolator/hamiltonian_system.pyx` & `unipolator-0.2.7/src/unipolator/hamiltonian_system.pyx`

 * *Files 4% similar despite different names*

```diff
@@ -94,25 +94,35 @@
     cdef weighted_hamiltonian(self, double[::1] c):
         self.curr_h0 = self.h0
         copy_pointer(self.curr_h0, self.v0, self.d2)
         for i in range(self.n_dims_1):
             self.curr_h0 += self.d2
             d_mat_add_pointer(self.v0, self.curr_h0, c[i], self.d2)
 
-    def expmH(self, double[::1] c, double complex[:,::1] U, double dt=1.0):
-        # Construct Hamiltonian
-        if not c.shape[0] == self.n_dims_1:
-            raise ValueError('c.shape[0] needs to be equal to H_s[0].shape[0]-1.')
-        cdef double complex *u0 = &U[0,0]
+    cdef expmH_pointer(self, double[::1] c, double complex *u0, double dt):
         self.weighted_hamiltonian(c)
         zheevd(self.jobz, self.uplo, &self.d, self.v0, &self.d, self.e0, self.work0, &self.lwork, self.rwork0, &self.lrwork, self.iwork0, &self.liwork, &self.info)
         copy_pointer(self.v0, self.u1, self.d2)
         v_exp_pointer(self.e0, self.u1, dt, self.d)
         DagM_M_cdot_pointer(self.v0, self.u1, u0, self.d)
 
+    def expmH(self, double[::1] c, double complex[:,::1] U, double dt=1.0):
+        # Construct Hamiltonian
+        if not c.shape[0] == self.n_dims_1:
+            raise ValueError('c.shape[0] needs to be equal to H_s[0].shape[0]-1.')
+        cdef double complex *u0 = &U[0,0]
+        self.expmH_pointer(c, u0, dt)
+
+    def expmH_pulse_no_multiply(self, double[:,::1] cs, double complex[:,:,::1] U, double dt=1.0):
+        cdef double complex *u0 = &U[0, 0, 0]
+        cdef how_many = cs.shape[0]
+        for i in range(how_many):
+            self.expmH_pointer(cs[i,:], u0, dt)
+            u0 += self.d2
+
     cdef dexpmH_pointer(self, double[::1] c, double complex *u0, double complex *du0, dt=1.0):  #int[::1] d_di,
         # Construct Hamiltonian
         cdef int i
         cdef double complex *h0
         cdef int curr_d_di_1
         self.weighted_hamiltonian(c)
         zheevd(self.jobz, self.uplo, &self.d, self.v0, &self.d, self.e0, self.work0, &self.lwork, self.rwork0, &self.lrwork, self.iwork0, &self.liwork, &self.info)
```

### Comparing `unipolator-0.2.6/src/unipolator/indexing.c` & `unipolator-0.2.7/src/unipolator/indexing.c`

 * *Files identical despite different names*

### Comparing `unipolator-0.2.6/src/unipolator/indexing.pxd` & `unipolator-0.2.7/src/unipolator/indexing.pxd`

 * *Files identical despite different names*

### Comparing `unipolator-0.2.6/src/unipolator/indexing.pyx` & `unipolator-0.2.7/src/unipolator/indexing.pyx`

 * *Files identical despite different names*

### Comparing `unipolator-0.2.6/src/unipolator/sym_trotter_system.c` & `unipolator-0.2.7/src/unipolator/sym_trotter_system.c`

 * *Files 0% similar despite different names*

```diff
@@ -2351,24 +2351,24 @@
 
 /* ObjectToMemviewSlice.proto */
 static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_dc_double(PyObject *, int writable_flag);
 
 /* ObjectToMemviewSlice.proto */
 static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_d_dc___pyx_t_double_complex(PyObject *, int writable_flag);
 
+/* ObjectToMemviewSlice.proto */
+static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_d_dc_double(PyObject *, int writable_flag);
+
 /* IntPow.proto */
 static CYTHON_INLINE long __Pyx_pow_long(long, long);
 
 /* ObjectToMemviewSlice.proto */
 static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_dc___pyx_t_double_complex(PyObject *, int writable_flag);
 
 /* ObjectToMemviewSlice.proto */
-static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_d_dc_double(PyObject *, int writable_flag);
-
-/* ObjectToMemviewSlice.proto */
 static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_dc_int(PyObject *, int writable_flag);
 
 /* ToPy.proto */
 #define __pyx_PyComplex_FromComplex(z)\
         PyComplex_FromDoubles((double)__Pyx_CREAL(z),\
                               (double)__Pyx_CIMAG(z))
 
@@ -2587,14 +2587,15 @@
 static PyObject *__pyx_builtin_enumerate;
 static PyObject *__pyx_builtin_Ellipsis;
 static PyObject *__pyx_builtin_id;
 static PyObject *__pyx_builtin_IndexError;
 static const char __pyx_k_O[] = "O";
 static const char __pyx_k_U[] = "U";
 static const char __pyx_k_c[] = "c";
+static const char __pyx_k_cs[] = "cs";
 static const char __pyx_k_id[] = "id";
 static const char __pyx_k_np[] = "np";
 static const char __pyx_k_H_s[] = "H_s";
 static const char __pyx_k_new[] = "__new__";
 static const char __pyx_k_obj[] = "obj";
 static const char __pyx_k_base[] = "base";
 static const char __pyx_k_dict[] = "__dict__";
@@ -2725,14 +2726,15 @@
 static PyObject *__pyx_n_u_c;
 static PyObject *__pyx_kp_u_c_shape_0_needs_to_be_equal_to_H;
 static PyObject *__pyx_n_s_class;
 static PyObject *__pyx_n_s_cline_in_traceback;
 static PyObject *__pyx_n_s_complex128;
 static PyObject *__pyx_kp_s_contiguous_and_direct;
 static PyObject *__pyx_kp_s_contiguous_and_indirect;
+static PyObject *__pyx_n_s_cs;
 static PyObject *__pyx_n_s_dict;
 static PyObject *__pyx_n_s_double;
 static PyObject *__pyx_n_s_dtype;
 static PyObject *__pyx_n_s_dtype_is_object;
 static PyObject *__pyx_n_s_empty;
 static PyObject *__pyx_n_s_encode;
 static PyObject *__pyx_n_s_enumerate;
@@ -2793,16 +2795,17 @@
 static PyObject *__pyx_kp_s_unable_to_allocate_shape_and_str;
 static PyObject *__pyx_n_s_unpack;
 static PyObject *__pyx_n_s_update;
 static PyObject *__pyx_n_s_which_diffs;
 static int __pyx_pf_10unipolator_18sym_trotter_system_18Sym_Trotter_System___cinit__(struct __pyx_obj_10unipolator_18sym_trotter_system_Sym_Trotter_System *__pyx_v_self, __Pyx_memviewslice __pyx_v_H_s, __Pyx_memviewslice __pyx_v_which_diffs, int __pyx_v_m_times); /* proto */
 static PyObject *__pyx_pf_10unipolator_18sym_trotter_system_18Sym_Trotter_System_2get_cache(struct __pyx_obj_10unipolator_18sym_trotter_system_Sym_Trotter_System *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_10unipolator_18sym_trotter_system_18Sym_Trotter_System_4expmH(struct __pyx_obj_10unipolator_18sym_trotter_system_Sym_Trotter_System *__pyx_v_self, __Pyx_memviewslice __pyx_v_c, __Pyx_memviewslice __pyx_v_U); /* proto */
-static PyObject *__pyx_pf_10unipolator_18sym_trotter_system_18Sym_Trotter_System_6__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_10unipolator_18sym_trotter_system_Sym_Trotter_System *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_10unipolator_18sym_trotter_system_18Sym_Trotter_System_8__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_10unipolator_18sym_trotter_system_Sym_Trotter_System *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
+static PyObject *__pyx_pf_10unipolator_18sym_trotter_system_18Sym_Trotter_System_6expmH_pulse_no_multiply(struct __pyx_obj_10unipolator_18sym_trotter_system_Sym_Trotter_System *__pyx_v_self, __Pyx_memviewslice __pyx_v_cs, __Pyx_memviewslice __pyx_v_U); /* proto */
+static PyObject *__pyx_pf_10unipolator_18sym_trotter_system_18Sym_Trotter_System_8__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_10unipolator_18sym_trotter_system_Sym_Trotter_System *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_10unipolator_18sym_trotter_system_18Sym_Trotter_System_10__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_10unipolator_18sym_trotter_system_Sym_Trotter_System *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
 static int __pyx_array___pyx_pf_15View_dot_MemoryView_5array___cinit__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_shape, Py_ssize_t __pyx_v_itemsize, PyObject *__pyx_v_format, PyObject *__pyx_v_mode, int __pyx_v_allocate_buffer); /* proto */
 static int __pyx_array___pyx_pf_15View_dot_MemoryView_5array_2__getbuffer__(struct __pyx_array_obj *__pyx_v_self, Py_buffer *__pyx_v_info, int __pyx_v_flags); /* proto */
 static void __pyx_array___pyx_pf_15View_dot_MemoryView_5array_4__dealloc__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_15View_dot_MemoryView_5array_7memview___get__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static Py_ssize_t __pyx_array___pyx_pf_15View_dot_MemoryView_5array_6__len__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_array___pyx_pf_15View_dot_MemoryView_5array_8__getattr__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_attr); /* proto */
 static PyObject *__pyx_array___pyx_pf_15View_dot_MemoryView_5array_10__getitem__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_item); /* proto */
@@ -4635,14 +4638,16 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   Py_ssize_t __pyx_t_2;
   long __pyx_t_3;
   __pyx_t_double_complex *__pyx_t_4;
   double *__pyx_t_5;
+  int __pyx_t_6;
+  int __pyx_t_7;
   __Pyx_RefNannySetupContext("expmH_pointer", 0);
 
   /* "unipolator/sym_trotter_system.pyx":131
  *     cdef expmH_pointer(self, double[::1] c, double complex *u0):
  *         # Construct Hamiltonian
  *         if c.shape[0] == 1: # Special case             # <<<<<<<<<<<<<<
  *             copy_pointer(self.r0, self.u1, self.d2)
@@ -4795,31 +4800,99 @@
     __pyx_f_10unipolator_14blas_functions_MM_cdot_pointer(__pyx_v_self->u1, __pyx_v_self->r0, __pyx_v_u0, __pyx_v_self->d);
 
     /* "unipolator/sym_trotter_system.pyx":147
  *             MM_cdot_pointer(self.l0, u0, self.u1, self.d)
  *             MM_cdot_pointer(self.u1, self.r0, u0, self.d)
  *             self.c1 = self.c0  # Restore original value of pointer             # <<<<<<<<<<<<<<
  *             self.e1s = self.e0s
- * 
+ *         for i in range(1, self.m_times, 2):
  */
     __pyx_t_4 = __pyx_v_self->c0;
     __pyx_v_self->c1 = __pyx_t_4;
 
     /* "unipolator/sym_trotter_system.pyx":148
  *             MM_cdot_pointer(self.u1, self.r0, u0, self.d)
  *             self.c1 = self.c0  # Restore original value of pointer
  *             self.e1s = self.e0s             # <<<<<<<<<<<<<<
- * 
- *     #def expmH(self, double[::1] c, double complex[:,::1] U):
+ *         for i in range(1, self.m_times, 2):
+ *             MM_cdot_pointer(u0, u0, self.u1, self.d)
  */
     __pyx_t_5 = __pyx_v_self->e0s;
     __pyx_v_self->e1s = __pyx_t_5;
   }
   __pyx_L3:;
 
+  /* "unipolator/sym_trotter_system.pyx":149
+ *             self.c1 = self.c0  # Restore original value of pointer
+ *             self.e1s = self.e0s
+ *         for i in range(1, self.m_times, 2):             # <<<<<<<<<<<<<<
+ *             MM_cdot_pointer(u0, u0, self.u1, self.d)
+ *             MM_cdot_pointer(self.u1, self.u1, u0, self.d)
+ */
+  __pyx_t_6 = __pyx_v_self->m_times;
+  __pyx_t_7 = __pyx_t_6;
+  for (__pyx_t_3 = 1; __pyx_t_3 < __pyx_t_7; __pyx_t_3+=2) {
+    __pyx_v_i = __pyx_t_3;
+
+    /* "unipolator/sym_trotter_system.pyx":150
+ *             self.e1s = self.e0s
+ *         for i in range(1, self.m_times, 2):
+ *             MM_cdot_pointer(u0, u0, self.u1, self.d)             # <<<<<<<<<<<<<<
+ *             MM_cdot_pointer(self.u1, self.u1, u0, self.d)
+ *         if self.m_times % 2:
+ */
+    __pyx_f_10unipolator_14blas_functions_MM_cdot_pointer(__pyx_v_u0, __pyx_v_u0, __pyx_v_self->u1, __pyx_v_self->d);
+
+    /* "unipolator/sym_trotter_system.pyx":151
+ *         for i in range(1, self.m_times, 2):
+ *             MM_cdot_pointer(u0, u0, self.u1, self.d)
+ *             MM_cdot_pointer(self.u1, self.u1, u0, self.d)             # <<<<<<<<<<<<<<
+ *         if self.m_times % 2:
+ *             MM_cdot_pointer(u0, u0, self.u1, self.d)
+ */
+    __pyx_f_10unipolator_14blas_functions_MM_cdot_pointer(__pyx_v_self->u1, __pyx_v_self->u1, __pyx_v_u0, __pyx_v_self->d);
+  }
+
+  /* "unipolator/sym_trotter_system.pyx":152
+ *             MM_cdot_pointer(u0, u0, self.u1, self.d)
+ *             MM_cdot_pointer(self.u1, self.u1, u0, self.d)
+ *         if self.m_times % 2:             # <<<<<<<<<<<<<<
+ *             MM_cdot_pointer(u0, u0, self.u1, self.d)
+ *             copy_pointer(self.u1, u0, self.d2)
+ */
+  __pyx_t_1 = ((__pyx_v_self->m_times % 2) != 0);
+  if (__pyx_t_1) {
+
+    /* "unipolator/sym_trotter_system.pyx":153
+ *             MM_cdot_pointer(self.u1, self.u1, u0, self.d)
+ *         if self.m_times % 2:
+ *             MM_cdot_pointer(u0, u0, self.u1, self.d)             # <<<<<<<<<<<<<<
+ *             copy_pointer(self.u1, u0, self.d2)
+ * 
+ */
+    __pyx_f_10unipolator_14blas_functions_MM_cdot_pointer(__pyx_v_u0, __pyx_v_u0, __pyx_v_self->u1, __pyx_v_self->d);
+
+    /* "unipolator/sym_trotter_system.pyx":154
+ *         if self.m_times % 2:
+ *             MM_cdot_pointer(u0, u0, self.u1, self.d)
+ *             copy_pointer(self.u1, u0, self.d2)             # <<<<<<<<<<<<<<
+ * 
+ *     def expmH(self, double[::1] c, double complex[:,::1] U):
+ */
+    __pyx_f_10unipolator_11exp_and_log_copy_pointer(__pyx_v_self->u1, __pyx_v_u0, __pyx_v_self->d2);
+
+    /* "unipolator/sym_trotter_system.pyx":152
+ *             MM_cdot_pointer(u0, u0, self.u1, self.d)
+ *             MM_cdot_pointer(self.u1, self.u1, u0, self.d)
+ *         if self.m_times % 2:             # <<<<<<<<<<<<<<
+ *             MM_cdot_pointer(u0, u0, self.u1, self.d)
+ *             copy_pointer(self.u1, u0, self.d2)
+ */
+  }
+
   /* "unipolator/sym_trotter_system.pyx":129
  *         return np.array(self.C), np.array(self.Es), np.array(self.L), np.array(self.R)
  * 
  *     cdef expmH_pointer(self, double[::1] c, double complex *u0):             # <<<<<<<<<<<<<<
  *         # Construct Hamiltonian
  *         if c.shape[0] == 1: # Special case
  */
@@ -4827,16 +4900,16 @@
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unipolator/sym_trotter_system.pyx":157
- *     #    self.expmH_pointer(c, u0)
+/* "unipolator/sym_trotter_system.pyx":156
+ *             copy_pointer(self.u1, u0, self.d2)
  * 
  *     def expmH(self, double[::1] c, double complex[:,::1] U):             # <<<<<<<<<<<<<<
  *         # Construct Hamiltonian
  *         if not c.shape[0] == self.n_dims_1:
  */
 
 /* Python wrapper */
@@ -4870,227 +4943,398 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_c)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_U)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("expmH", 1, 2, 2, 1); __PYX_ERR(0, 157, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("expmH", 1, 2, 2, 1); __PYX_ERR(0, 156, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "expmH") < 0)) __PYX_ERR(0, 157, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "expmH") < 0)) __PYX_ERR(0, 156, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
-    __pyx_v_c = __Pyx_PyObject_to_MemoryviewSlice_dc_double(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_c.memview)) __PYX_ERR(0, 157, __pyx_L3_error)
-    __pyx_v_U = __Pyx_PyObject_to_MemoryviewSlice_d_dc___pyx_t_double_complex(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_U.memview)) __PYX_ERR(0, 157, __pyx_L3_error)
+    __pyx_v_c = __Pyx_PyObject_to_MemoryviewSlice_dc_double(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_c.memview)) __PYX_ERR(0, 156, __pyx_L3_error)
+    __pyx_v_U = __Pyx_PyObject_to_MemoryviewSlice_d_dc___pyx_t_double_complex(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_U.memview)) __PYX_ERR(0, 156, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("expmH", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 157, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("expmH", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 156, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("unipolator.sym_trotter_system.Sym_Trotter_System.expmH", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_10unipolator_18sym_trotter_system_18Sym_Trotter_System_4expmH(((struct __pyx_obj_10unipolator_18sym_trotter_system_Sym_Trotter_System *)__pyx_v_self), __pyx_v_c, __pyx_v_U);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_10unipolator_18sym_trotter_system_18Sym_Trotter_System_4expmH(struct __pyx_obj_10unipolator_18sym_trotter_system_Sym_Trotter_System *__pyx_v_self, __Pyx_memviewslice __pyx_v_c, __Pyx_memviewslice __pyx_v_U) {
   __pyx_t_double_complex *__pyx_v_u0;
-  CYTHON_UNUSED long __pyx_v_i;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   Py_ssize_t __pyx_t_3;
   Py_ssize_t __pyx_t_4;
-  int __pyx_t_5;
-  int __pyx_t_6;
-  long __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("expmH", 0);
 
-  /* "unipolator/sym_trotter_system.pyx":159
+  /* "unipolator/sym_trotter_system.pyx":158
  *     def expmH(self, double[::1] c, double complex[:,::1] U):
  *         # Construct Hamiltonian
  *         if not c.shape[0] == self.n_dims_1:             # <<<<<<<<<<<<<<
  *             raise ValueError('c.shape[0] needs to be equal to H_s[0].shape[0]-1.')
  *         cdef double complex *u0 = &U[0,0]
  */
   __pyx_t_1 = ((!(((__pyx_v_c.shape[0]) == __pyx_v_self->n_dims_1) != 0)) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "unipolator/sym_trotter_system.pyx":160
+    /* "unipolator/sym_trotter_system.pyx":159
  *         # Construct Hamiltonian
  *         if not c.shape[0] == self.n_dims_1:
  *             raise ValueError('c.shape[0] needs to be equal to H_s[0].shape[0]-1.')             # <<<<<<<<<<<<<<
  *         cdef double complex *u0 = &U[0,0]
  *         self.expmH_pointer(c, u0)
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 160, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 159, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 160, __pyx_L1_error)
+    __PYX_ERR(0, 159, __pyx_L1_error)
 
-    /* "unipolator/sym_trotter_system.pyx":159
+    /* "unipolator/sym_trotter_system.pyx":158
  *     def expmH(self, double[::1] c, double complex[:,::1] U):
  *         # Construct Hamiltonian
  *         if not c.shape[0] == self.n_dims_1:             # <<<<<<<<<<<<<<
  *             raise ValueError('c.shape[0] needs to be equal to H_s[0].shape[0]-1.')
  *         cdef double complex *u0 = &U[0,0]
  */
   }
 
-  /* "unipolator/sym_trotter_system.pyx":161
+  /* "unipolator/sym_trotter_system.pyx":160
  *         if not c.shape[0] == self.n_dims_1:
  *             raise ValueError('c.shape[0] needs to be equal to H_s[0].shape[0]-1.')
  *         cdef double complex *u0 = &U[0,0]             # <<<<<<<<<<<<<<
  *         self.expmH_pointer(c, u0)
- *         for i in range(1, self.m_times, 2):
+ * 
  */
   __pyx_t_3 = 0;
   __pyx_t_4 = 0;
   __pyx_v_u0 = (&(*((__pyx_t_double_complex *) ( /* dim=1 */ ((char *) (((__pyx_t_double_complex *) ( /* dim=0 */ (__pyx_v_U.data + __pyx_t_3 * __pyx_v_U.strides[0]) )) + __pyx_t_4)) ))));
 
-  /* "unipolator/sym_trotter_system.pyx":162
+  /* "unipolator/sym_trotter_system.pyx":161
  *             raise ValueError('c.shape[0] needs to be equal to H_s[0].shape[0]-1.')
  *         cdef double complex *u0 = &U[0,0]
  *         self.expmH_pointer(c, u0)             # <<<<<<<<<<<<<<
- *         for i in range(1, self.m_times, 2):
- *             MM_cdot_pointer(u0, u0, self.u1, self.d)
+ * 
+ *     def expmH_pulse_no_multiply(self, double[:,::1] cs, double complex[:,:,::1] U):
  */
-  __pyx_t_2 = ((struct __pyx_vtabstruct_10unipolator_18sym_trotter_system_Sym_Trotter_System *)__pyx_v_self->__pyx_vtab)->expmH_pointer(__pyx_v_self, __pyx_v_c, __pyx_v_u0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 162, __pyx_L1_error)
+  __pyx_t_2 = ((struct __pyx_vtabstruct_10unipolator_18sym_trotter_system_Sym_Trotter_System *)__pyx_v_self->__pyx_vtab)->expmH_pointer(__pyx_v_self, __pyx_v_c, __pyx_v_u0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 161, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "unipolator/sym_trotter_system.pyx":163
- *         cdef double complex *u0 = &U[0,0]
- *         self.expmH_pointer(c, u0)
- *         for i in range(1, self.m_times, 2):             # <<<<<<<<<<<<<<
- *             MM_cdot_pointer(u0, u0, self.u1, self.d)
- *             MM_cdot_pointer(self.u1, self.u1, u0, self.d)
+  /* "unipolator/sym_trotter_system.pyx":156
+ *             copy_pointer(self.u1, u0, self.d2)
+ * 
+ *     def expmH(self, double[::1] c, double complex[:,::1] U):             # <<<<<<<<<<<<<<
+ *         # Construct Hamiltonian
+ *         if not c.shape[0] == self.n_dims_1:
  */
-  __pyx_t_5 = __pyx_v_self->m_times;
-  __pyx_t_6 = __pyx_t_5;
-  for (__pyx_t_7 = 1; __pyx_t_7 < __pyx_t_6; __pyx_t_7+=2) {
-    __pyx_v_i = __pyx_t_7;
 
-    /* "unipolator/sym_trotter_system.pyx":164
+  /* function exit code */
+  __pyx_r = Py_None; __Pyx_INCREF(Py_None);
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_AddTraceback("unipolator.sym_trotter_system.Sym_Trotter_System.expmH", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __PYX_XDEC_MEMVIEW(&__pyx_v_c, 1);
+  __PYX_XDEC_MEMVIEW(&__pyx_v_U, 1);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "unipolator/sym_trotter_system.pyx":163
  *         self.expmH_pointer(c, u0)
- *         for i in range(1, self.m_times, 2):
- *             MM_cdot_pointer(u0, u0, self.u1, self.d)             # <<<<<<<<<<<<<<
- *             MM_cdot_pointer(self.u1, self.u1, u0, self.d)
- *         if self.m_times % 2:
+ * 
+ *     def expmH_pulse_no_multiply(self, double[:,::1] cs, double complex[:,:,::1] U):             # <<<<<<<<<<<<<<
+ *         cdef double complex *u0 = &U[0, 0, 0]
+ *         cdef how_many = cs.shape[0]
  */
-    __pyx_f_10unipolator_14blas_functions_MM_cdot_pointer(__pyx_v_u0, __pyx_v_u0, __pyx_v_self->u1, __pyx_v_self->d);
 
-    /* "unipolator/sym_trotter_system.pyx":165
- *         for i in range(1, self.m_times, 2):
- *             MM_cdot_pointer(u0, u0, self.u1, self.d)
- *             MM_cdot_pointer(self.u1, self.u1, u0, self.d)             # <<<<<<<<<<<<<<
- *         if self.m_times % 2:
- *             MM_cdot_pointer(u0, u0, self.u1, self.d)
- */
-    __pyx_f_10unipolator_14blas_functions_MM_cdot_pointer(__pyx_v_self->u1, __pyx_v_self->u1, __pyx_v_u0, __pyx_v_self->d);
+/* Python wrapper */
+static PyObject *__pyx_pw_10unipolator_18sym_trotter_system_18Sym_Trotter_System_7expmH_pulse_no_multiply(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_10unipolator_18sym_trotter_system_18Sym_Trotter_System_6expmH_pulse_no_multiply[] = "Sym_Trotter_System.expmH_pulse_no_multiply(self, double[:, ::1] cs, double complex[:, :, ::1] U)";
+static PyObject *__pyx_pw_10unipolator_18sym_trotter_system_18Sym_Trotter_System_7expmH_pulse_no_multiply(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+  __Pyx_memviewslice __pyx_v_cs = { 0, 0, { 0 }, { 0 }, { 0 } };
+  __Pyx_memviewslice __pyx_v_U = { 0, 0, { 0 }, { 0 }, { 0 } };
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("expmH_pulse_no_multiply (wrapper)", 0);
+  {
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_cs,&__pyx_n_s_U,0};
+    PyObject* values[2] = {0,0};
+    if (unlikely(__pyx_kwds)) {
+      Py_ssize_t kw_args;
+      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
+      switch (pos_args) {
+        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
+        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = PyDict_Size(__pyx_kwds);
+      switch (pos_args) {
+        case  0:
+        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_cs)) != 0)) kw_args--;
+        else goto __pyx_L5_argtuple_error;
+        CYTHON_FALLTHROUGH;
+        case  1:
+        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_U)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("expmH_pulse_no_multiply", 1, 2, 2, 1); __PYX_ERR(0, 163, __pyx_L3_error)
+        }
+      }
+      if (unlikely(kw_args > 0)) {
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "expmH_pulse_no_multiply") < 0)) __PYX_ERR(0, 163, __pyx_L3_error)
+      }
+    } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
+      goto __pyx_L5_argtuple_error;
+    } else {
+      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+      values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+    }
+    __pyx_v_cs = __Pyx_PyObject_to_MemoryviewSlice_d_dc_double(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_cs.memview)) __PYX_ERR(0, 163, __pyx_L3_error)
+    __pyx_v_U = __Pyx_PyObject_to_MemoryviewSlice_d_d_dc___pyx_t_double_complex(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_U.memview)) __PYX_ERR(0, 163, __pyx_L3_error)
   }
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("expmH_pulse_no_multiply", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 163, __pyx_L3_error)
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("unipolator.sym_trotter_system.Sym_Trotter_System.expmH_pulse_no_multiply", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  __pyx_r = __pyx_pf_10unipolator_18sym_trotter_system_18Sym_Trotter_System_6expmH_pulse_no_multiply(((struct __pyx_obj_10unipolator_18sym_trotter_system_Sym_Trotter_System *)__pyx_v_self), __pyx_v_cs, __pyx_v_U);
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_10unipolator_18sym_trotter_system_18Sym_Trotter_System_6expmH_pulse_no_multiply(struct __pyx_obj_10unipolator_18sym_trotter_system_Sym_Trotter_System *__pyx_v_self, __Pyx_memviewslice __pyx_v_cs, __Pyx_memviewslice __pyx_v_U) {
+  __pyx_t_double_complex *__pyx_v_u0;
+  PyObject *__pyx_v_how_many = 0;
+  PyObject *__pyx_v_i = NULL;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  Py_ssize_t __pyx_t_1;
+  Py_ssize_t __pyx_t_2;
+  Py_ssize_t __pyx_t_3;
+  PyObject *__pyx_t_4 = NULL;
+  PyObject *__pyx_t_5 = NULL;
+  Py_ssize_t __pyx_t_6;
+  PyObject *(*__pyx_t_7)(PyObject *);
+  Py_ssize_t __pyx_t_8;
+  __Pyx_memviewslice __pyx_t_9 = { 0, 0, { 0 }, { 0 }, { 0 } };
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("expmH_pulse_no_multiply", 0);
+
+  /* "unipolator/sym_trotter_system.pyx":164
+ * 
+ *     def expmH_pulse_no_multiply(self, double[:,::1] cs, double complex[:,:,::1] U):
+ *         cdef double complex *u0 = &U[0, 0, 0]             # <<<<<<<<<<<<<<
+ *         cdef how_many = cs.shape[0]
+ *         for i in range(how_many):
+ */
+  __pyx_t_1 = 0;
+  __pyx_t_2 = 0;
+  __pyx_t_3 = 0;
+  __pyx_v_u0 = (&(*((__pyx_t_double_complex *) ( /* dim=2 */ ((char *) (((__pyx_t_double_complex *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_U.data + __pyx_t_1 * __pyx_v_U.strides[0]) ) + __pyx_t_2 * __pyx_v_U.strides[1]) )) + __pyx_t_3)) ))));
+
+  /* "unipolator/sym_trotter_system.pyx":165
+ *     def expmH_pulse_no_multiply(self, double[:,::1] cs, double complex[:,:,::1] U):
+ *         cdef double complex *u0 = &U[0, 0, 0]
+ *         cdef how_many = cs.shape[0]             # <<<<<<<<<<<<<<
+ *         for i in range(how_many):
+ *             self.expmH_pointer(cs[i,:], u0)
+ */
+  __pyx_t_4 = PyInt_FromSsize_t((__pyx_v_cs.shape[0])); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 165, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_v_how_many = __pyx_t_4;
+  __pyx_t_4 = 0;
 
   /* "unipolator/sym_trotter_system.pyx":166
- *             MM_cdot_pointer(u0, u0, self.u1, self.d)
- *             MM_cdot_pointer(self.u1, self.u1, u0, self.d)
- *         if self.m_times % 2:             # <<<<<<<<<<<<<<
- *             MM_cdot_pointer(u0, u0, self.u1, self.d)
- *             copy_pointer(self.u1, u0, self.d2)
+ *         cdef double complex *u0 = &U[0, 0, 0]
+ *         cdef how_many = cs.shape[0]
+ *         for i in range(how_many):             # <<<<<<<<<<<<<<
+ *             self.expmH_pointer(cs[i,:], u0)
+ *             u0 += self.d2
  */
-  __pyx_t_1 = ((__pyx_v_self->m_times % 2) != 0);
-  if (__pyx_t_1) {
+  __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_range, __pyx_v_how_many); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 166, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  if (likely(PyList_CheckExact(__pyx_t_4)) || PyTuple_CheckExact(__pyx_t_4)) {
+    __pyx_t_5 = __pyx_t_4; __Pyx_INCREF(__pyx_t_5); __pyx_t_6 = 0;
+    __pyx_t_7 = NULL;
+  } else {
+    __pyx_t_6 = -1; __pyx_t_5 = PyObject_GetIter(__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 166, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_t_7 = Py_TYPE(__pyx_t_5)->tp_iternext; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 166, __pyx_L1_error)
+  }
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  for (;;) {
+    if (likely(!__pyx_t_7)) {
+      if (likely(PyList_CheckExact(__pyx_t_5))) {
+        if (__pyx_t_6 >= PyList_GET_SIZE(__pyx_t_5)) break;
+        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_5, __pyx_t_6); __Pyx_INCREF(__pyx_t_4); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 166, __pyx_L1_error)
+        #else
+        __pyx_t_4 = PySequence_ITEM(__pyx_t_5, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 166, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_4);
+        #endif
+      } else {
+        if (__pyx_t_6 >= PyTuple_GET_SIZE(__pyx_t_5)) break;
+        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_5, __pyx_t_6); __Pyx_INCREF(__pyx_t_4); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 166, __pyx_L1_error)
+        #else
+        __pyx_t_4 = PySequence_ITEM(__pyx_t_5, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 166, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_4);
+        #endif
+      }
+    } else {
+      __pyx_t_4 = __pyx_t_7(__pyx_t_5);
+      if (unlikely(!__pyx_t_4)) {
+        PyObject* exc_type = PyErr_Occurred();
+        if (exc_type) {
+          if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
+          else __PYX_ERR(0, 166, __pyx_L1_error)
+        }
+        break;
+      }
+      __Pyx_GOTREF(__pyx_t_4);
+    }
+    __Pyx_XDECREF_SET(__pyx_v_i, __pyx_t_4);
+    __pyx_t_4 = 0;
 
     /* "unipolator/sym_trotter_system.pyx":167
- *             MM_cdot_pointer(self.u1, self.u1, u0, self.d)
- *         if self.m_times % 2:
- *             MM_cdot_pointer(u0, u0, self.u1, self.d)             # <<<<<<<<<<<<<<
- *             copy_pointer(self.u1, u0, self.d2)
- * 
+ *         cdef how_many = cs.shape[0]
+ *         for i in range(how_many):
+ *             self.expmH_pointer(cs[i,:], u0)             # <<<<<<<<<<<<<<
+ *             u0 += self.d2
+ *     """
  */
-    __pyx_f_10unipolator_14blas_functions_MM_cdot_pointer(__pyx_v_u0, __pyx_v_u0, __pyx_v_self->u1, __pyx_v_self->d);
+    __pyx_t_8 = __Pyx_PyIndex_AsSsize_t(__pyx_v_i); if (unlikely((__pyx_t_8 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 167, __pyx_L1_error)
+    __pyx_t_9.data = __pyx_v_cs.data;
+    __pyx_t_9.memview = __pyx_v_cs.memview;
+    __PYX_INC_MEMVIEW(&__pyx_t_9, 0);
+    {
+    Py_ssize_t __pyx_tmp_idx = __pyx_t_8;
+    Py_ssize_t __pyx_tmp_stride = __pyx_v_cs.strides[0];
+        __pyx_t_9.data += __pyx_tmp_idx * __pyx_tmp_stride;
+}
+
+__pyx_t_9.shape[0] = __pyx_v_cs.shape[1];
+__pyx_t_9.strides[0] = __pyx_v_cs.strides[1];
+    __pyx_t_9.suboffsets[0] = -1;
+
+__pyx_t_4 = ((struct __pyx_vtabstruct_10unipolator_18sym_trotter_system_Sym_Trotter_System *)__pyx_v_self->__pyx_vtab)->expmH_pointer(__pyx_v_self, __pyx_t_9, __pyx_v_u0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 167, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __PYX_XDEC_MEMVIEW(&__pyx_t_9, 1);
+    __pyx_t_9.memview = NULL;
+    __pyx_t_9.data = NULL;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "unipolator/sym_trotter_system.pyx":168
- *         if self.m_times % 2:
- *             MM_cdot_pointer(u0, u0, self.u1, self.d)
- *             copy_pointer(self.u1, u0, self.d2)             # <<<<<<<<<<<<<<
- * 
- * 
+ *         for i in range(how_many):
+ *             self.expmH_pointer(cs[i,:], u0)
+ *             u0 += self.d2             # <<<<<<<<<<<<<<
+ *     """
+ *     def set_which_diffs(self, int[::1] which_diffs):
  */
-    __pyx_f_10unipolator_11exp_and_log_copy_pointer(__pyx_v_self->u1, __pyx_v_u0, __pyx_v_self->d2);
+    __pyx_v_u0 = (__pyx_v_u0 + __pyx_v_self->d2);
 
     /* "unipolator/sym_trotter_system.pyx":166
- *             MM_cdot_pointer(u0, u0, self.u1, self.d)
- *             MM_cdot_pointer(self.u1, self.u1, u0, self.d)
- *         if self.m_times % 2:             # <<<<<<<<<<<<<<
- *             MM_cdot_pointer(u0, u0, self.u1, self.d)
- *             copy_pointer(self.u1, u0, self.d2)
+ *         cdef double complex *u0 = &U[0, 0, 0]
+ *         cdef how_many = cs.shape[0]
+ *         for i in range(how_many):             # <<<<<<<<<<<<<<
+ *             self.expmH_pointer(cs[i,:], u0)
+ *             u0 += self.d2
  */
   }
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "unipolator/sym_trotter_system.pyx":157
- *     #    self.expmH_pointer(c, u0)
+  /* "unipolator/sym_trotter_system.pyx":163
+ *         self.expmH_pointer(c, u0)
  * 
- *     def expmH(self, double[::1] c, double complex[:,::1] U):             # <<<<<<<<<<<<<<
- *         # Construct Hamiltonian
- *         if not c.shape[0] == self.n_dims_1:
+ *     def expmH_pulse_no_multiply(self, double[:,::1] cs, double complex[:,:,::1] U):             # <<<<<<<<<<<<<<
+ *         cdef double complex *u0 = &U[0, 0, 0]
+ *         cdef how_many = cs.shape[0]
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_AddTraceback("unipolator.sym_trotter_system.Sym_Trotter_System.expmH", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_5);
+  __PYX_XDEC_MEMVIEW(&__pyx_t_9, 1);
+  __Pyx_AddTraceback("unipolator.sym_trotter_system.Sym_Trotter_System.expmH_pulse_no_multiply", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
-  __PYX_XDEC_MEMVIEW(&__pyx_v_c, 1);
+  __Pyx_XDECREF(__pyx_v_how_many);
+  __Pyx_XDECREF(__pyx_v_i);
+  __PYX_XDEC_MEMVIEW(&__pyx_v_cs, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_v_U, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_10unipolator_18sym_trotter_system_18Sym_Trotter_System_7__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static char __pyx_doc_10unipolator_18sym_trotter_system_18Sym_Trotter_System_6__reduce_cython__[] = "Sym_Trotter_System.__reduce_cython__(self)";
-static PyObject *__pyx_pw_10unipolator_18sym_trotter_system_18Sym_Trotter_System_7__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_10unipolator_18sym_trotter_system_18Sym_Trotter_System_9__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc_10unipolator_18sym_trotter_system_18Sym_Trotter_System_8__reduce_cython__[] = "Sym_Trotter_System.__reduce_cython__(self)";
+static PyObject *__pyx_pw_10unipolator_18sym_trotter_system_18Sym_Trotter_System_9__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_10unipolator_18sym_trotter_system_18Sym_Trotter_System_6__reduce_cython__(((struct __pyx_obj_10unipolator_18sym_trotter_system_Sym_Trotter_System *)__pyx_v_self));
+  __pyx_r = __pyx_pf_10unipolator_18sym_trotter_system_18Sym_Trotter_System_8__reduce_cython__(((struct __pyx_obj_10unipolator_18sym_trotter_system_Sym_Trotter_System *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_10unipolator_18sym_trotter_system_18Sym_Trotter_System_6__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_10unipolator_18sym_trotter_system_Sym_Trotter_System *__pyx_v_self) {
+static PyObject *__pyx_pf_10unipolator_18sym_trotter_system_18Sym_Trotter_System_8__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_10unipolator_18sym_trotter_system_Sym_Trotter_System *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__reduce_cython__", 0);
@@ -5127,28 +5371,28 @@
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_10unipolator_18sym_trotter_system_18Sym_Trotter_System_9__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
-static char __pyx_doc_10unipolator_18sym_trotter_system_18Sym_Trotter_System_8__setstate_cython__[] = "Sym_Trotter_System.__setstate_cython__(self, __pyx_state)";
-static PyObject *__pyx_pw_10unipolator_18sym_trotter_system_18Sym_Trotter_System_9__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pw_10unipolator_18sym_trotter_system_18Sym_Trotter_System_11__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
+static char __pyx_doc_10unipolator_18sym_trotter_system_18Sym_Trotter_System_10__setstate_cython__[] = "Sym_Trotter_System.__setstate_cython__(self, __pyx_state)";
+static PyObject *__pyx_pw_10unipolator_18sym_trotter_system_18Sym_Trotter_System_11__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_10unipolator_18sym_trotter_system_18Sym_Trotter_System_8__setstate_cython__(((struct __pyx_obj_10unipolator_18sym_trotter_system_Sym_Trotter_System *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
+  __pyx_r = __pyx_pf_10unipolator_18sym_trotter_system_18Sym_Trotter_System_10__setstate_cython__(((struct __pyx_obj_10unipolator_18sym_trotter_system_Sym_Trotter_System *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_10unipolator_18sym_trotter_system_18Sym_Trotter_System_8__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_10unipolator_18sym_trotter_system_Sym_Trotter_System *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pf_10unipolator_18sym_trotter_system_18Sym_Trotter_System_10__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_10unipolator_18sym_trotter_system_Sym_Trotter_System *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
@@ -19315,16 +19559,17 @@
   __PYX_XDEC_MEMVIEW(&p->iwork, 1);
   (*Py_TYPE(o)->tp_free)(o);
 }
 
 static PyMethodDef __pyx_methods_10unipolator_18sym_trotter_system_Sym_Trotter_System[] = {
   {"get_cache", (PyCFunction)__pyx_pw_10unipolator_18sym_trotter_system_18Sym_Trotter_System_3get_cache, METH_NOARGS, __pyx_doc_10unipolator_18sym_trotter_system_18Sym_Trotter_System_2get_cache},
   {"expmH", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_10unipolator_18sym_trotter_system_18Sym_Trotter_System_5expmH, METH_VARARGS|METH_KEYWORDS, __pyx_doc_10unipolator_18sym_trotter_system_18Sym_Trotter_System_4expmH},
-  {"__reduce_cython__", (PyCFunction)__pyx_pw_10unipolator_18sym_trotter_system_18Sym_Trotter_System_7__reduce_cython__, METH_NOARGS, __pyx_doc_10unipolator_18sym_trotter_system_18Sym_Trotter_System_6__reduce_cython__},
-  {"__setstate_cython__", (PyCFunction)__pyx_pw_10unipolator_18sym_trotter_system_18Sym_Trotter_System_9__setstate_cython__, METH_O, __pyx_doc_10unipolator_18sym_trotter_system_18Sym_Trotter_System_8__setstate_cython__},
+  {"expmH_pulse_no_multiply", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_10unipolator_18sym_trotter_system_18Sym_Trotter_System_7expmH_pulse_no_multiply, METH_VARARGS|METH_KEYWORDS, __pyx_doc_10unipolator_18sym_trotter_system_18Sym_Trotter_System_6expmH_pulse_no_multiply},
+  {"__reduce_cython__", (PyCFunction)__pyx_pw_10unipolator_18sym_trotter_system_18Sym_Trotter_System_9__reduce_cython__, METH_NOARGS, __pyx_doc_10unipolator_18sym_trotter_system_18Sym_Trotter_System_8__reduce_cython__},
+  {"__setstate_cython__", (PyCFunction)__pyx_pw_10unipolator_18sym_trotter_system_18Sym_Trotter_System_11__setstate_cython__, METH_O, __pyx_doc_10unipolator_18sym_trotter_system_18Sym_Trotter_System_10__setstate_cython__},
   {0, 0, 0, 0}
 };
 
 static PyTypeObject __pyx_type_10unipolator_18sym_trotter_system_Sym_Trotter_System = {
   PyVarObject_HEAD_INIT(0, 0)
   "unipolator.sym_trotter_system.Sym_Trotter_System", /*tp_name*/
   sizeof(struct __pyx_obj_10unipolator_18sym_trotter_system_Sym_Trotter_System), /*tp_basicsize*/
@@ -20204,14 +20449,15 @@
   {&__pyx_n_u_c, __pyx_k_c, sizeof(__pyx_k_c), 0, 1, 0, 1},
   {&__pyx_kp_u_c_shape_0_needs_to_be_equal_to_H, __pyx_k_c_shape_0_needs_to_be_equal_to_H, sizeof(__pyx_k_c_shape_0_needs_to_be_equal_to_H), 0, 1, 0, 0},
   {&__pyx_n_s_class, __pyx_k_class, sizeof(__pyx_k_class), 0, 0, 1, 1},
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
   {&__pyx_n_s_complex128, __pyx_k_complex128, sizeof(__pyx_k_complex128), 0, 0, 1, 1},
   {&__pyx_kp_s_contiguous_and_direct, __pyx_k_contiguous_and_direct, sizeof(__pyx_k_contiguous_and_direct), 0, 0, 1, 0},
   {&__pyx_kp_s_contiguous_and_indirect, __pyx_k_contiguous_and_indirect, sizeof(__pyx_k_contiguous_and_indirect), 0, 0, 1, 0},
+  {&__pyx_n_s_cs, __pyx_k_cs, sizeof(__pyx_k_cs), 0, 0, 1, 1},
   {&__pyx_n_s_dict, __pyx_k_dict, sizeof(__pyx_k_dict), 0, 0, 1, 1},
   {&__pyx_n_s_double, __pyx_k_double, sizeof(__pyx_k_double), 0, 0, 1, 1},
   {&__pyx_n_s_dtype, __pyx_k_dtype, sizeof(__pyx_k_dtype), 0, 0, 1, 1},
   {&__pyx_n_s_dtype_is_object, __pyx_k_dtype_is_object, sizeof(__pyx_k_dtype_is_object), 0, 0, 1, 1},
   {&__pyx_n_s_empty, __pyx_k_empty, sizeof(__pyx_k_empty), 0, 0, 1, 1},
   {&__pyx_n_s_encode, __pyx_k_encode, sizeof(__pyx_k_encode), 0, 0, 1, 1},
   {&__pyx_n_s_enumerate, __pyx_k_enumerate, sizeof(__pyx_k_enumerate), 0, 0, 1, 1},
@@ -20273,15 +20519,15 @@
   {&__pyx_n_s_unpack, __pyx_k_unpack, sizeof(__pyx_k_unpack), 0, 0, 1, 1},
   {&__pyx_n_s_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 0, 1, 1},
   {&__pyx_n_s_which_diffs, __pyx_k_which_diffs, sizeof(__pyx_k_which_diffs), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 111, __pyx_L1_error)
-  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 160, __pyx_L1_error)
+  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 159, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(1, 2, __pyx_L1_error)
   __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(2, 945, __pyx_L1_error)
   __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(1, 149, __pyx_L1_error)
   __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(1, 152, __pyx_L1_error)
   __pyx_builtin_Ellipsis = __Pyx_GetBuiltinName(__pyx_n_s_Ellipsis); if (!__pyx_builtin_Ellipsis) __PYX_ERR(1, 406, __pyx_L1_error)
   __pyx_builtin_id = __Pyx_GetBuiltinName(__pyx_n_s_id); if (!__pyx_builtin_id) __PYX_ERR(1, 615, __pyx_L1_error)
   __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(1, 834, __pyx_L1_error)
@@ -20290,22 +20536,22 @@
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "unipolator/sym_trotter_system.pyx":160
+  /* "unipolator/sym_trotter_system.pyx":159
  *         # Construct Hamiltonian
  *         if not c.shape[0] == self.n_dims_1:
  *             raise ValueError('c.shape[0] needs to be equal to H_s[0].shape[0]-1.')             # <<<<<<<<<<<<<<
  *         cdef double complex *u0 = &U[0,0]
  *         self.expmH_pointer(c, u0)
  */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_c_shape_0_needs_to_be_equal_to_H); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 160, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_c_shape_0_needs_to_be_equal_to_H); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 159, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
@@ -24570,14 +24816,37 @@
     return result;
 __pyx_fail:
     result.memview = NULL;
     result.data = NULL;
     return result;
 }
 
+/* ObjectToMemviewSlice */
+  static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_d_dc_double(PyObject *obj, int writable_flag) {
+    __Pyx_memviewslice result = { 0, 0, { 0 }, { 0 }, { 0 } };
+    __Pyx_BufFmt_StackElem stack[1];
+    int axes_specs[] = { (__Pyx_MEMVIEW_DIRECT | __Pyx_MEMVIEW_FOLLOW), (__Pyx_MEMVIEW_DIRECT | __Pyx_MEMVIEW_CONTIG) };
+    int retcode;
+    if (obj == Py_None) {
+        result.memview = (struct __pyx_memoryview_obj *) Py_None;
+        return result;
+    }
+    retcode = __Pyx_ValidateAndInit_memviewslice(axes_specs, __Pyx_IS_C_CONTIG,
+                                                 (PyBUF_C_CONTIGUOUS | PyBUF_FORMAT) | writable_flag, 2,
+                                                 &__Pyx_TypeInfo_double, stack,
+                                                 &result, obj);
+    if (unlikely(retcode == -1))
+        goto __pyx_fail;
+    return result;
+__pyx_fail:
+    result.memview = NULL;
+    result.data = NULL;
+    return result;
+}
+
 /* IntPow */
   static CYTHON_INLINE long __Pyx_pow_long(long b, long e) {
     long t = b;
     switch (e) {
         case 3:
             t *= b;
         CYTHON_FALLTHROUGH;
@@ -24617,37 +24886,14 @@
                                                  &result, obj);
     if (unlikely(retcode == -1))
         goto __pyx_fail;
     return result;
 __pyx_fail:
     result.memview = NULL;
     result.data = NULL;
-    return result;
-}
-
-/* ObjectToMemviewSlice */
-  static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_d_dc_double(PyObject *obj, int writable_flag) {
-    __Pyx_memviewslice result = { 0, 0, { 0 }, { 0 }, { 0 } };
-    __Pyx_BufFmt_StackElem stack[1];
-    int axes_specs[] = { (__Pyx_MEMVIEW_DIRECT | __Pyx_MEMVIEW_FOLLOW), (__Pyx_MEMVIEW_DIRECT | __Pyx_MEMVIEW_CONTIG) };
-    int retcode;
-    if (obj == Py_None) {
-        result.memview = (struct __pyx_memoryview_obj *) Py_None;
-        return result;
-    }
-    retcode = __Pyx_ValidateAndInit_memviewslice(axes_specs, __Pyx_IS_C_CONTIG,
-                                                 (PyBUF_C_CONTIGUOUS | PyBUF_FORMAT) | writable_flag, 2,
-                                                 &__Pyx_TypeInfo_double, stack,
-                                                 &result, obj);
-    if (unlikely(retcode == -1))
-        goto __pyx_fail;
-    return result;
-__pyx_fail:
-    result.memview = NULL;
-    result.data = NULL;
     return result;
 }
 
 /* ObjectToMemviewSlice */
   static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_dc_int(PyObject *obj, int writable_flag) {
     __Pyx_memviewslice result = { 0, 0, { 0 }, { 0 }, { 0 } };
     __Pyx_BufFmt_StackElem stack[1];
```

### Comparing `unipolator-0.2.6/src/unipolator/sym_trotter_system.pyx` & `unipolator-0.2.7/src/unipolator/sym_trotter_system.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -142,36 +142,34 @@
                 MM_cdot_pointer(self.v0, self.c1, u0, self.d)
             self.e1s -= self.d
             expE_V_expE_pointer(self.e1s, u0, c[0], self.exp0, self.d)
             MM_cdot_pointer(self.l0, u0, self.u1, self.d)
             MM_cdot_pointer(self.u1, self.r0, u0, self.d)
             self.c1 = self.c0  # Restore original value of pointer
             self.e1s = self.e0s
-
-    #def expmH(self, double[::1] c, double complex[:,::1] U):
-    #    # Construct Hamiltonian
-    #    if not c.shape[0] == self.n_dims_1:
-    #        raise ValueError('c.shape[0] needs to be equal to H_s[0].shape[0]-1.')
-    #    cdef double complex *u0 = &U[0,0]
-    #    self.expmH_pointer(c, u0)
-
-    def expmH(self, double[::1] c, double complex[:,::1] U):
-        # Construct Hamiltonian
-        if not c.shape[0] == self.n_dims_1:
-            raise ValueError('c.shape[0] needs to be equal to H_s[0].shape[0]-1.')
-        cdef double complex *u0 = &U[0,0]
-        self.expmH_pointer(c, u0)
         for i in range(1, self.m_times, 2):
             MM_cdot_pointer(u0, u0, self.u1, self.d)
             MM_cdot_pointer(self.u1, self.u1, u0, self.d)
         if self.m_times % 2:
             MM_cdot_pointer(u0, u0, self.u1, self.d)
             copy_pointer(self.u1, u0, self.d2)
 
+    def expmH(self, double[::1] c, double complex[:,::1] U):
+        # Construct Hamiltonian
+        if not c.shape[0] == self.n_dims_1:
+            raise ValueError('c.shape[0] needs to be equal to H_s[0].shape[0]-1.')
+        cdef double complex *u0 = &U[0,0]
+        self.expmH_pointer(c, u0)
 
+    def expmH_pulse_no_multiply(self, double[:,::1] cs, double complex[:,:,::1] U):
+        cdef double complex *u0 = &U[0, 0, 0]
+        cdef how_many = cs.shape[0]
+        for i in range(how_many):
+            self.expmH_pointer(cs[i,:], u0)
+            u0 += self.d2
     """
     def set_which_diffs(self, int[::1] which_diffs):
         self.d_di = which_diffs
         self.n_d_di = self.d_di.shape[0]
 
     def get_which_diffs(self):
         return np.asarray(self.d_di), self.n_d_di
```

### Comparing `unipolator-0.2.6/src/unipolator/symmetric_unitary_interpolation.c` & `unipolator-0.2.7/src/unipolator/symmetric_unitary_interpolation.c`

 * *Files 1% similar despite different names*

```diff
@@ -1412,15 +1412,14 @@
   int d;
   int d2;
   int n_dims_1;
   int n_dims_2;
   int n_d_di_1;
   int n_d_di;
   int i;
-  __Pyx_memviewslice E_C;
   __Pyx_memviewslice E;
   __Pyx_memviewslice Vr;
   __Pyx_memviewslice Vl;
   __Pyx_memviewslice CL_L;
   __Pyx_memviewslice CH_L;
   __Pyx_memviewslice CL_R;
   __Pyx_memviewslice CH_R;
@@ -1440,15 +1439,14 @@
   __pyx_t_double_complex *ur0;
   __pyx_t_double_complex *ur1;
   __pyx_t_double_complex *ur2;
   __pyx_t_double_complex *dul;
   __pyx_t_double_complex *dur;
   __pyx_t_double_complex *duc;
   __Pyx_memviewslice strides_L;
-  __Pyx_memviewslice strides_EC;
   __Pyx_memviewslice strides_E;
   __Pyx_memviewslice strides_C;
   __Pyx_memviewslice location;
   __Pyx_memviewslice d_location;
   __Pyx_memviewslice abs_alpha_rest;
   __Pyx_memviewslice alpha;
   __Pyx_memviewslice first_elements_E;
@@ -2266,14 +2264,17 @@
 
 /* ObjectToMemviewSlice.proto */
 static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_dc_double(PyObject *, int writable_flag);
 
 /* ObjectToMemviewSlice.proto */
 static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_d_dc___pyx_t_double_complex(PyObject *, int writable_flag);
 
+/* ObjectToMemviewSlice.proto */
+static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_d_dc_double(PyObject *, int writable_flag);
+
 /* GCCDiagnostics.proto */
 #if defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 6))
 #define __Pyx_HAS_GCC_DIAGNOSTIC
 #endif
 
 /* ToPy.proto */
 #define __pyx_PyComplex_FromComplex(z)\
@@ -2284,17 +2285,14 @@
 static __pyx_t_double_complex __Pyx_PyComplex_As___pyx_t_double_complex(PyObject*);
 
 /* MemviewDtypeToObject.proto */
 static CYTHON_INLINE PyObject *__pyx_memview_get___pyx_t_double_complex(const char *itemp);
 static CYTHON_INLINE int __pyx_memview_set___pyx_t_double_complex(const char *itemp, PyObject *obj);
 
 /* ObjectToMemviewSlice.proto */
-static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_d_dc_double(PyObject *, int writable_flag);
-
-/* ObjectToMemviewSlice.proto */
 static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_d_dc_long(PyObject *, int writable_flag);
 
 /* ObjectToMemviewSlice.proto */
 static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_dc___pyx_t_double_complex(PyObject *, int writable_flag);
 
 /* MemviewDtypeToObject.proto */
 static CYTHON_INLINE PyObject *__pyx_memview_get_long(const char *itemp);
@@ -2520,14 +2518,15 @@
 static PyObject *__pyx_builtin_enumerate;
 static PyObject *__pyx_builtin_Ellipsis;
 static PyObject *__pyx_builtin_id;
 static PyObject *__pyx_builtin_IndexError;
 static const char __pyx_k_O[] = "O";
 static const char __pyx_k_U[] = "U";
 static const char __pyx_k_c[] = "c";
+static const char __pyx_k_cs[] = "cs";
 static const char __pyx_k_id[] = "id";
 static const char __pyx_k_np[] = "np";
 static const char __pyx_k_H_s[] = "H_s";
 static const char __pyx_k_new[] = "__new__";
 static const char __pyx_k_obj[] = "obj";
 static const char __pyx_k_base[] = "base";
 static const char __pyx_k_dict[] = "__dict__";
@@ -2576,15 +2575,14 @@
 static const char __pyx_k_itemsize[] = "itemsize";
 static const char __pyx_k_pyx_type[] = "__pyx_type";
 static const char __pyx_k_setstate[] = "__setstate__";
 static const char __pyx_k_TypeError[] = "TypeError";
 static const char __pyx_k_enumerate[] = "enumerate";
 static const char __pyx_k_pyx_state[] = "__pyx_state";
 static const char __pyx_k_reduce_ex[] = "__reduce_ex__";
-static const char __pyx_k_strides_R[] = "strides_R";
 static const char __pyx_k_IndexError[] = "IndexError";
 static const char __pyx_k_ValueError[] = "ValueError";
 static const char __pyx_k_complex128[] = "complex128";
 static const char __pyx_k_pyx_result[] = "__pyx_result";
 static const char __pyx_k_pyx_vtable[] = "__pyx_vtable__";
 static const char __pyx_k_ImportError[] = "ImportError";
 static const char __pyx_k_MemoryError[] = "MemoryError";
@@ -2673,14 +2671,15 @@
 static PyObject *__pyx_n_s_c_max_s;
 static PyObject *__pyx_n_s_c_min_s;
 static PyObject *__pyx_n_s_class;
 static PyObject *__pyx_n_s_cline_in_traceback;
 static PyObject *__pyx_n_s_complex128;
 static PyObject *__pyx_kp_s_contiguous_and_direct;
 static PyObject *__pyx_kp_s_contiguous_and_indirect;
+static PyObject *__pyx_n_s_cs;
 static PyObject *__pyx_n_s_dict;
 static PyObject *__pyx_n_s_double;
 static PyObject *__pyx_n_s_dtype;
 static PyObject *__pyx_n_s_dtype_is_object;
 static PyObject *__pyx_n_s_empty;
 static PyObject *__pyx_n_s_encode;
 static PyObject *__pyx_n_s_enumerate;
@@ -2729,31 +2728,31 @@
 static PyObject *__pyx_n_s_size;
 static PyObject *__pyx_n_s_start;
 static PyObject *__pyx_n_s_step;
 static PyObject *__pyx_n_s_stop;
 static PyObject *__pyx_kp_s_strided_and_direct;
 static PyObject *__pyx_kp_s_strided_and_direct_or_indirect;
 static PyObject *__pyx_kp_s_strided_and_indirect;
-static PyObject *__pyx_n_s_strides_R;
 static PyObject *__pyx_kp_s_stringsource;
 static PyObject *__pyx_n_s_struct;
 static PyObject *__pyx_n_s_test;
 static PyObject *__pyx_kp_u_to_1;
 static PyObject *__pyx_kp_s_unable_to_allocate_array_data;
 static PyObject *__pyx_kp_s_unable_to_allocate_shape_and_str;
 static PyObject *__pyx_n_s_unpack;
 static PyObject *__pyx_n_s_update;
 static PyObject *__pyx_n_s_which_diffs;
 static int __pyx_pf_10unipolator_31symmetric_unitary_interpolation_6Sym_UI___cinit__(struct __pyx_obj_10unipolator_31symmetric_unitary_interpolation_Sym_UI *__pyx_v_self, __Pyx_memviewslice __pyx_v_H_s, __Pyx_memviewslice __pyx_v_c_min_s, __Pyx_memviewslice __pyx_v_c_max_s, __Pyx_memviewslice __pyx_v_c_bins, __Pyx_memviewslice __pyx_v_which_diffs); /* proto */
 static PyObject *__pyx_pf_10unipolator_31symmetric_unitary_interpolation_6Sym_UI_2set_which_diffs(struct __pyx_obj_10unipolator_31symmetric_unitary_interpolation_Sym_UI *__pyx_v_self, __Pyx_memviewslice __pyx_v_which_diffs); /* proto */
 static PyObject *__pyx_pf_10unipolator_31symmetric_unitary_interpolation_6Sym_UI_4get_single_param(struct __pyx_obj_10unipolator_31symmetric_unitary_interpolation_Sym_UI *__pyx_v_self, __Pyx_memviewslice __pyx_v_c); /* proto */
 static PyObject *__pyx_pf_10unipolator_31symmetric_unitary_interpolation_6Sym_UI_6get_cache(struct __pyx_obj_10unipolator_31symmetric_unitary_interpolation_Sym_UI *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_10unipolator_31symmetric_unitary_interpolation_6Sym_UI_8expmH(struct __pyx_obj_10unipolator_31symmetric_unitary_interpolation_Sym_UI *__pyx_v_self, __Pyx_memviewslice __pyx_v_c, __Pyx_memviewslice __pyx_v_U); /* proto */
-static PyObject *__pyx_pf_10unipolator_31symmetric_unitary_interpolation_6Sym_UI_10__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_10unipolator_31symmetric_unitary_interpolation_Sym_UI *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_10unipolator_31symmetric_unitary_interpolation_6Sym_UI_12__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_10unipolator_31symmetric_unitary_interpolation_Sym_UI *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
+static PyObject *__pyx_pf_10unipolator_31symmetric_unitary_interpolation_6Sym_UI_10expmH_pulse_no_multiply(struct __pyx_obj_10unipolator_31symmetric_unitary_interpolation_Sym_UI *__pyx_v_self, __Pyx_memviewslice __pyx_v_cs, __Pyx_memviewslice __pyx_v_U); /* proto */
+static PyObject *__pyx_pf_10unipolator_31symmetric_unitary_interpolation_6Sym_UI_12__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_10unipolator_31symmetric_unitary_interpolation_Sym_UI *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_10unipolator_31symmetric_unitary_interpolation_6Sym_UI_14__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_10unipolator_31symmetric_unitary_interpolation_Sym_UI *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
 static int __pyx_array___pyx_pf_15View_dot_MemoryView_5array___cinit__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_shape, Py_ssize_t __pyx_v_itemsize, PyObject *__pyx_v_format, PyObject *__pyx_v_mode, int __pyx_v_allocate_buffer); /* proto */
 static int __pyx_array___pyx_pf_15View_dot_MemoryView_5array_2__getbuffer__(struct __pyx_array_obj *__pyx_v_self, Py_buffer *__pyx_v_info, int __pyx_v_flags); /* proto */
 static void __pyx_array___pyx_pf_15View_dot_MemoryView_5array_4__dealloc__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_15View_dot_MemoryView_5array_7memview___get__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static Py_ssize_t __pyx_array___pyx_pf_15View_dot_MemoryView_5array_6__len__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_array___pyx_pf_15View_dot_MemoryView_5array_8__getattr__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_attr); /* proto */
 static PyObject *__pyx_array___pyx_pf_15View_dot_MemoryView_5array_10__getitem__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_item); /* proto */
@@ -3672,15 +3671,15 @@
   __pyx_t_5 = 0;
 
   /* "unipolator/symmetric_unitary_interpolation.pyx":73
  *         U_grid2, cum_prod = Unitary_Grid(H_s2, self.c_mins, self.dcs, self.c_bins) # Half grid -> H_s2 = H_s / 2
  *         ## Construct interpolation cache
  *         self.E, self.Vl, self.Vr, self.CL_L, self.CL_R, self.CH_L, self.CH_R, self.strides_E, self.strides_L, self.strides_C, self.first_elements_E, self.first_elements_C = Create_Sym_Interpolation_Cache( U_grid2, cum_prod, self.c_bins)             # <<<<<<<<<<<<<<
  * 
- *         self.ei = &self.E_C[0, 0]
+ *         self.ei = &self.E[0, 0]
  */
   __pyx_t_20 = __Pyx_PyObject_to_MemoryviewSlice_d_d_dc___pyx_t_double_complex(__pyx_v_U_grid2, PyBUF_WRITABLE); if (unlikely(!__pyx_t_20.memview)) __PYX_ERR(0, 73, __pyx_L1_error)
   __pyx_t_6 = __Pyx_PyObject_to_MemoryviewSlice_dc_long(__pyx_v_cum_prod, PyBUF_WRITABLE); if (unlikely(!__pyx_t_6.memview)) __PYX_ERR(0, 73, __pyx_L1_error)
   __pyx_t_13 = __pyx_f_10unipolator_7caching_Create_Sym_Interpolation_Cache(__pyx_t_20, __pyx_t_6, __pyx_v_self->c_bins, 0); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 73, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_13);
   __PYX_XDEC_MEMVIEW(&__pyx_t_20, 1);
   __pyx_t_20.memview = NULL;
@@ -3843,36 +3842,36 @@
   __pyx_v_self->first_elements_C = __pyx_t_38;
   __pyx_t_38.memview = NULL;
   __pyx_t_38.data = NULL;
 
   /* "unipolator/symmetric_unitary_interpolation.pyx":75
  *         self.E, self.Vl, self.Vr, self.CL_L, self.CL_R, self.CH_L, self.CH_R, self.strides_E, self.strides_L, self.strides_C, self.first_elements_E, self.first_elements_C = Create_Sym_Interpolation_Cache( U_grid2, cum_prod, self.c_bins)
  * 
- *         self.ei = &self.E_C[0, 0]             # <<<<<<<<<<<<<<
+ *         self.ei = &self.E[0, 0]             # <<<<<<<<<<<<<<
  *         self.vl = &self.Vl[0, 0, 0]
  *         self.vr = &self.Vr[0, 0, 0]
  */
   __pyx_t_10 = 0;
   __pyx_t_12 = 0;
-  __pyx_v_self->ei = (&(*((double *) ( /* dim=1 */ ((char *) (((double *) ( /* dim=0 */ (__pyx_v_self->E_C.data + __pyx_t_10 * __pyx_v_self->E_C.strides[0]) )) + __pyx_t_12)) ))));
+  __pyx_v_self->ei = (&(*((double *) ( /* dim=1 */ ((char *) (((double *) ( /* dim=0 */ (__pyx_v_self->E.data + __pyx_t_10 * __pyx_v_self->E.strides[0]) )) + __pyx_t_12)) ))));
 
   /* "unipolator/symmetric_unitary_interpolation.pyx":76
  * 
- *         self.ei = &self.E_C[0, 0]
+ *         self.ei = &self.E[0, 0]
  *         self.vl = &self.Vl[0, 0, 0]             # <<<<<<<<<<<<<<
  *         self.vr = &self.Vr[0, 0, 0]
  *         self.cl = &self.CL_L[0, 0, 0]
  */
   __pyx_t_12 = 0;
   __pyx_t_10 = 0;
   __pyx_t_39 = 0;
   __pyx_v_self->vl = (&(*((__pyx_t_double_complex *) ( /* dim=2 */ ((char *) (((__pyx_t_double_complex *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_self->Vl.data + __pyx_t_12 * __pyx_v_self->Vl.strides[0]) ) + __pyx_t_10 * __pyx_v_self->Vl.strides[1]) )) + __pyx_t_39)) ))));
 
   /* "unipolator/symmetric_unitary_interpolation.pyx":77
- *         self.ei = &self.E_C[0, 0]
+ *         self.ei = &self.E[0, 0]
  *         self.vl = &self.Vl[0, 0, 0]
  *         self.vr = &self.Vr[0, 0, 0]             # <<<<<<<<<<<<<<
  *         self.cl = &self.CL_L[0, 0, 0]
  *         self.cr = &self.CL_R[0, 0, 0]
  */
   __pyx_t_39 = 0;
   __pyx_t_10 = 0;
@@ -5125,15 +5124,15 @@
   return __pyx_r;
 }
 
 /* "unipolator/symmetric_unitary_interpolation.pyx":145
  *         return np.asarray(self.location), np.asarray(self.d_location), np.asarray(self.abs_alpha_rest)
  * 
  *     def get_cache(self): # To verify interpolation grid             # <<<<<<<<<<<<<<
- *         return np.asarray(self.E_C), np.asarray(self.E), np.asarray(self.Vl), np.asarray(self.Vr), np.asarray(self.CL_L), np.asarray(self.CL_R), np.asarray(self.CH_L), np.asarray(self.CH_R), np.asarray(self.strides_EC), np.asarray(self.strides_E), np.asarray(self.strides_R), np.asarray(self.strides_C), np.asarray(self.first_elements_E), np.asarray(self.first_elements_C)
+ *         return np.asarray(self.E), np.asarray(self.Vl), np.asarray(self.Vr), np.asarray(self.CL_L), np.asarray(self.CL_R), np.asarray(self.CH_L), np.asarray(self.CH_R), np.asarray(self.strides_E), np.asarray(self.strides_L), np.asarray(self.strides_C), np.asarray(self.first_elements_E), np.asarray(self.first_elements_C)
  * 
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_10unipolator_31symmetric_unitary_interpolation_6Sym_UI_7get_cache(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
 static char __pyx_doc_10unipolator_31symmetric_unitary_interpolation_6Sym_UI_6get_cache[] = "Sym_UI.get_cache(self)";
 static PyObject *__pyx_pw_10unipolator_31symmetric_unitary_interpolation_6Sym_UI_7get_cache(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
@@ -5161,35 +5160,33 @@
   PyObject *__pyx_t_9 = NULL;
   PyObject *__pyx_t_10 = NULL;
   PyObject *__pyx_t_11 = NULL;
   PyObject *__pyx_t_12 = NULL;
   PyObject *__pyx_t_13 = NULL;
   PyObject *__pyx_t_14 = NULL;
   PyObject *__pyx_t_15 = NULL;
-  PyObject *__pyx_t_16 = NULL;
-  PyObject *__pyx_t_17 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_cache", 0);
 
   /* "unipolator/symmetric_unitary_interpolation.pyx":146
  * 
  *     def get_cache(self): # To verify interpolation grid
- *         return np.asarray(self.E_C), np.asarray(self.E), np.asarray(self.Vl), np.asarray(self.Vr), np.asarray(self.CL_L), np.asarray(self.CL_R), np.asarray(self.CH_L), np.asarray(self.CH_R), np.asarray(self.strides_EC), np.asarray(self.strides_E), np.asarray(self.strides_R), np.asarray(self.strides_C), np.asarray(self.first_elements_E), np.asarray(self.first_elements_C)             # <<<<<<<<<<<<<<
+ *         return np.asarray(self.E), np.asarray(self.Vl), np.asarray(self.Vr), np.asarray(self.CL_L), np.asarray(self.CL_R), np.asarray(self.CH_L), np.asarray(self.CH_R), np.asarray(self.strides_E), np.asarray(self.strides_L), np.asarray(self.strides_C), np.asarray(self.first_elements_E), np.asarray(self.first_elements_C)             # <<<<<<<<<<<<<<
  * 
  *     cdef interpolate_single_u(self, double complex *u0):  #u0 => input the matrices for output
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 146, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_asarray); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 146, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_self->E_C, 2, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 146, __pyx_L1_error)
+  __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_self->E, 2, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 146, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_4);
@@ -5204,15 +5201,15 @@
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 146, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_asarray); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 146, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_self->E, 2, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 146, __pyx_L1_error)
+  __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_self->Vl, 3, (PyObject *(*)(char *)) __pyx_memview_get___pyx_t_double_complex, (int (*)(char *, PyObject *)) __pyx_memview_set___pyx_t_double_complex, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 146, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
       __Pyx_INCREF(__pyx_t_5);
@@ -5227,15 +5224,15 @@
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 146, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_asarray); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 146, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_self->Vl, 3, (PyObject *(*)(char *)) __pyx_memview_get___pyx_t_double_complex, (int (*)(char *, PyObject *)) __pyx_memview_set___pyx_t_double_complex, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 146, __pyx_L1_error)
+  __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_self->Vr, 3, (PyObject *(*)(char *)) __pyx_memview_get___pyx_t_double_complex, (int (*)(char *, PyObject *)) __pyx_memview_set___pyx_t_double_complex, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 146, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_6 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_6)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_6);
@@ -5250,15 +5247,15 @@
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 146, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_asarray); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 146, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_self->Vr, 3, (PyObject *(*)(char *)) __pyx_memview_get___pyx_t_double_complex, (int (*)(char *, PyObject *)) __pyx_memview_set___pyx_t_double_complex, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 146, __pyx_L1_error)
+  __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_self->CL_L, 3, (PyObject *(*)(char *)) __pyx_memview_get___pyx_t_double_complex, (int (*)(char *, PyObject *)) __pyx_memview_set___pyx_t_double_complex, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 146, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_7 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
     if (likely(__pyx_t_7)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
       __Pyx_INCREF(__pyx_t_7);
@@ -5273,15 +5270,15 @@
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 146, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_asarray); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 146, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_self->CL_L, 3, (PyObject *(*)(char *)) __pyx_memview_get___pyx_t_double_complex, (int (*)(char *, PyObject *)) __pyx_memview_set___pyx_t_double_complex, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 146, __pyx_L1_error)
+  __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_self->CL_R, 3, (PyObject *(*)(char *)) __pyx_memview_get___pyx_t_double_complex, (int (*)(char *, PyObject *)) __pyx_memview_set___pyx_t_double_complex, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 146, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_8 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_7))) {
     __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_7);
     if (likely(__pyx_t_8)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
       __Pyx_INCREF(__pyx_t_8);
@@ -5296,15 +5293,15 @@
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 146, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_asarray); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 146, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_self->CL_R, 3, (PyObject *(*)(char *)) __pyx_memview_get___pyx_t_double_complex, (int (*)(char *, PyObject *)) __pyx_memview_set___pyx_t_double_complex, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 146, __pyx_L1_error)
+  __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_self->CH_L, 3, (PyObject *(*)(char *)) __pyx_memview_get___pyx_t_double_complex, (int (*)(char *, PyObject *)) __pyx_memview_set___pyx_t_double_complex, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 146, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_9 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_8))) {
     __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_8);
     if (likely(__pyx_t_9)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
       __Pyx_INCREF(__pyx_t_9);
@@ -5319,15 +5316,15 @@
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 146, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_asarray); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 146, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_self->CH_L, 3, (PyObject *(*)(char *)) __pyx_memview_get___pyx_t_double_complex, (int (*)(char *, PyObject *)) __pyx_memview_set___pyx_t_double_complex, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 146, __pyx_L1_error)
+  __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_self->CH_R, 3, (PyObject *(*)(char *)) __pyx_memview_get___pyx_t_double_complex, (int (*)(char *, PyObject *)) __pyx_memview_set___pyx_t_double_complex, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 146, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_10 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_9))) {
     __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_9);
     if (likely(__pyx_t_10)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
       __Pyx_INCREF(__pyx_t_10);
@@ -5342,15 +5339,15 @@
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 146, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_asarray); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 146, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_self->CH_R, 3, (PyObject *(*)(char *)) __pyx_memview_get___pyx_t_double_complex, (int (*)(char *, PyObject *)) __pyx_memview_set___pyx_t_double_complex, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 146, __pyx_L1_error)
+  __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_self->strides_E, 2, (PyObject *(*)(char *)) __pyx_memview_get_long, (int (*)(char *, PyObject *)) __pyx_memview_set_long, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 146, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_11 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_10))) {
     __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_10);
     if (likely(__pyx_t_11)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_10);
       __Pyx_INCREF(__pyx_t_11);
@@ -5365,15 +5362,15 @@
   __Pyx_GOTREF(__pyx_t_9);
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 146, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_asarray); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 146, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_11);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_self->strides_EC, 1, (PyObject *(*)(char *)) __pyx_memview_get_long, (int (*)(char *, PyObject *)) __pyx_memview_set_long, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 146, __pyx_L1_error)
+  __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_self->strides_L, 1, (PyObject *(*)(char *)) __pyx_memview_get_long, (int (*)(char *, PyObject *)) __pyx_memview_set_long, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 146, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_12 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_11))) {
     __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_11);
     if (likely(__pyx_t_12)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_11);
       __Pyx_INCREF(__pyx_t_12);
@@ -5388,15 +5385,15 @@
   __Pyx_GOTREF(__pyx_t_10);
   __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 146, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_asarray); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 146, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_12);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_self->strides_E, 2, (PyObject *(*)(char *)) __pyx_memview_get_long, (int (*)(char *, PyObject *)) __pyx_memview_set_long, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 146, __pyx_L1_error)
+  __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_self->strides_C, 2, (PyObject *(*)(char *)) __pyx_memview_get_long, (int (*)(char *, PyObject *)) __pyx_memview_set_long, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 146, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_13 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_12))) {
     __pyx_t_13 = PyMethod_GET_SELF(__pyx_t_12);
     if (likely(__pyx_t_13)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_12);
       __Pyx_INCREF(__pyx_t_13);
@@ -5411,15 +5408,15 @@
   __Pyx_GOTREF(__pyx_t_11);
   __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 146, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_asarray); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 146, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_13);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_strides_R); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 146, __pyx_L1_error)
+  __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_self->first_elements_E, 1, (PyObject *(*)(char *)) __pyx_memview_get_long, (int (*)(char *, PyObject *)) __pyx_memview_set_long, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 146, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_14 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_13))) {
     __pyx_t_14 = PyMethod_GET_SELF(__pyx_t_13);
     if (likely(__pyx_t_14)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_13);
       __Pyx_INCREF(__pyx_t_14);
@@ -5434,15 +5431,15 @@
   __Pyx_GOTREF(__pyx_t_12);
   __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 146, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_14 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_asarray); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 146, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_14);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_self->strides_C, 2, (PyObject *(*)(char *)) __pyx_memview_get_long, (int (*)(char *, PyObject *)) __pyx_memview_set_long, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 146, __pyx_L1_error)
+  __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_self->first_elements_C, 1, (PyObject *(*)(char *)) __pyx_memview_get_long, (int (*)(char *, PyObject *)) __pyx_memview_set_long, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 146, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_15 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_14))) {
     __pyx_t_15 = PyMethod_GET_SELF(__pyx_t_14);
     if (likely(__pyx_t_15)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_14);
       __Pyx_INCREF(__pyx_t_15);
@@ -5452,113 +5449,61 @@
   }
   __pyx_t_13 = (__pyx_t_15) ? __Pyx_PyObject_Call2Args(__pyx_t_14, __pyx_t_15, __pyx_t_2) : __Pyx_PyObject_CallOneArg(__pyx_t_14, __pyx_t_2);
   __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 146, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_13);
   __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 146, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_15 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_asarray); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 146, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_15);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_self->first_elements_E, 1, (PyObject *(*)(char *)) __pyx_memview_get_long, (int (*)(char *, PyObject *)) __pyx_memview_set_long, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 146, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_16 = NULL;
-  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_15))) {
-    __pyx_t_16 = PyMethod_GET_SELF(__pyx_t_15);
-    if (likely(__pyx_t_16)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_15);
-      __Pyx_INCREF(__pyx_t_16);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_15, function);
-    }
-  }
-  __pyx_t_14 = (__pyx_t_16) ? __Pyx_PyObject_Call2Args(__pyx_t_15, __pyx_t_16, __pyx_t_2) : __Pyx_PyObject_CallOneArg(__pyx_t_15, __pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_16); __pyx_t_16 = 0;
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 146, __pyx_L1_error)
+  __pyx_t_14 = PyTuple_New(12); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 146, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_14);
-  __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 146, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_16 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_asarray); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 146, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_16);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_self->first_elements_C, 1, (PyObject *(*)(char *)) __pyx_memview_get_long, (int (*)(char *, PyObject *)) __pyx_memview_set_long, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 146, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_17 = NULL;
-  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_16))) {
-    __pyx_t_17 = PyMethod_GET_SELF(__pyx_t_16);
-    if (likely(__pyx_t_17)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_16);
-      __Pyx_INCREF(__pyx_t_17);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_16, function);
-    }
-  }
-  __pyx_t_15 = (__pyx_t_17) ? __Pyx_PyObject_Call2Args(__pyx_t_16, __pyx_t_17, __pyx_t_2) : __Pyx_PyObject_CallOneArg(__pyx_t_16, __pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_17); __pyx_t_17 = 0;
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 146, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_15);
-  __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
-  __pyx_t_16 = PyTuple_New(14); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 146, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_16);
   __Pyx_GIVEREF(__pyx_t_1);
-  PyTuple_SET_ITEM(__pyx_t_16, 0, __pyx_t_1);
+  PyTuple_SET_ITEM(__pyx_t_14, 0, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_3);
-  PyTuple_SET_ITEM(__pyx_t_16, 1, __pyx_t_3);
+  PyTuple_SET_ITEM(__pyx_t_14, 1, __pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_4);
-  PyTuple_SET_ITEM(__pyx_t_16, 2, __pyx_t_4);
+  PyTuple_SET_ITEM(__pyx_t_14, 2, __pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_5);
-  PyTuple_SET_ITEM(__pyx_t_16, 3, __pyx_t_5);
+  PyTuple_SET_ITEM(__pyx_t_14, 3, __pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_6);
-  PyTuple_SET_ITEM(__pyx_t_16, 4, __pyx_t_6);
+  PyTuple_SET_ITEM(__pyx_t_14, 4, __pyx_t_6);
   __Pyx_GIVEREF(__pyx_t_7);
-  PyTuple_SET_ITEM(__pyx_t_16, 5, __pyx_t_7);
+  PyTuple_SET_ITEM(__pyx_t_14, 5, __pyx_t_7);
   __Pyx_GIVEREF(__pyx_t_8);
-  PyTuple_SET_ITEM(__pyx_t_16, 6, __pyx_t_8);
+  PyTuple_SET_ITEM(__pyx_t_14, 6, __pyx_t_8);
   __Pyx_GIVEREF(__pyx_t_9);
-  PyTuple_SET_ITEM(__pyx_t_16, 7, __pyx_t_9);
+  PyTuple_SET_ITEM(__pyx_t_14, 7, __pyx_t_9);
   __Pyx_GIVEREF(__pyx_t_10);
-  PyTuple_SET_ITEM(__pyx_t_16, 8, __pyx_t_10);
+  PyTuple_SET_ITEM(__pyx_t_14, 8, __pyx_t_10);
   __Pyx_GIVEREF(__pyx_t_11);
-  PyTuple_SET_ITEM(__pyx_t_16, 9, __pyx_t_11);
+  PyTuple_SET_ITEM(__pyx_t_14, 9, __pyx_t_11);
   __Pyx_GIVEREF(__pyx_t_12);
-  PyTuple_SET_ITEM(__pyx_t_16, 10, __pyx_t_12);
+  PyTuple_SET_ITEM(__pyx_t_14, 10, __pyx_t_12);
   __Pyx_GIVEREF(__pyx_t_13);
-  PyTuple_SET_ITEM(__pyx_t_16, 11, __pyx_t_13);
-  __Pyx_GIVEREF(__pyx_t_14);
-  PyTuple_SET_ITEM(__pyx_t_16, 12, __pyx_t_14);
-  __Pyx_GIVEREF(__pyx_t_15);
-  PyTuple_SET_ITEM(__pyx_t_16, 13, __pyx_t_15);
+  PyTuple_SET_ITEM(__pyx_t_14, 11, __pyx_t_13);
   __pyx_t_1 = 0;
   __pyx_t_3 = 0;
   __pyx_t_4 = 0;
   __pyx_t_5 = 0;
   __pyx_t_6 = 0;
   __pyx_t_7 = 0;
   __pyx_t_8 = 0;
   __pyx_t_9 = 0;
   __pyx_t_10 = 0;
   __pyx_t_11 = 0;
   __pyx_t_12 = 0;
   __pyx_t_13 = 0;
+  __pyx_r = __pyx_t_14;
   __pyx_t_14 = 0;
-  __pyx_t_15 = 0;
-  __pyx_r = __pyx_t_16;
-  __pyx_t_16 = 0;
   goto __pyx_L0;
 
   /* "unipolator/symmetric_unitary_interpolation.pyx":145
  *         return np.asarray(self.location), np.asarray(self.d_location), np.asarray(self.abs_alpha_rest)
  * 
  *     def get_cache(self): # To verify interpolation grid             # <<<<<<<<<<<<<<
- *         return np.asarray(self.E_C), np.asarray(self.E), np.asarray(self.Vl), np.asarray(self.Vr), np.asarray(self.CL_L), np.asarray(self.CL_R), np.asarray(self.CH_L), np.asarray(self.CH_R), np.asarray(self.strides_EC), np.asarray(self.strides_E), np.asarray(self.strides_R), np.asarray(self.strides_C), np.asarray(self.first_elements_E), np.asarray(self.first_elements_C)
+ *         return np.asarray(self.E), np.asarray(self.Vl), np.asarray(self.Vr), np.asarray(self.CL_L), np.asarray(self.CL_R), np.asarray(self.CH_L), np.asarray(self.CH_R), np.asarray(self.strides_E), np.asarray(self.strides_L), np.asarray(self.strides_C), np.asarray(self.first_elements_E), np.asarray(self.first_elements_C)
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
@@ -5571,26 +5516,24 @@
   __Pyx_XDECREF(__pyx_t_9);
   __Pyx_XDECREF(__pyx_t_10);
   __Pyx_XDECREF(__pyx_t_11);
   __Pyx_XDECREF(__pyx_t_12);
   __Pyx_XDECREF(__pyx_t_13);
   __Pyx_XDECREF(__pyx_t_14);
   __Pyx_XDECREF(__pyx_t_15);
-  __Pyx_XDECREF(__pyx_t_16);
-  __Pyx_XDECREF(__pyx_t_17);
   __Pyx_AddTraceback("unipolator.symmetric_unitary_interpolation.Sym_UI.get_cache", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "unipolator/symmetric_unitary_interpolation.pyx":148
- *         return np.asarray(self.E_C), np.asarray(self.E), np.asarray(self.Vl), np.asarray(self.Vr), np.asarray(self.CL_L), np.asarray(self.CL_R), np.asarray(self.CH_L), np.asarray(self.CH_R), np.asarray(self.strides_EC), np.asarray(self.strides_E), np.asarray(self.strides_R), np.asarray(self.strides_C), np.asarray(self.first_elements_E), np.asarray(self.first_elements_C)
+ *         return np.asarray(self.E), np.asarray(self.Vl), np.asarray(self.Vr), np.asarray(self.CL_L), np.asarray(self.CL_R), np.asarray(self.CH_L), np.asarray(self.CH_R), np.asarray(self.strides_E), np.asarray(self.strides_L), np.asarray(self.strides_C), np.asarray(self.first_elements_E), np.asarray(self.first_elements_C)
  * 
  *     cdef interpolate_single_u(self, double complex *u0):  #u0 => input the matrices for output             # <<<<<<<<<<<<<<
  *         cdef int i, j
  *         cdef int ind, indE
  */
 
 static PyObject *__pyx_f_10unipolator_31symmetric_unitary_interpolation_6Sym_UI_interpolate_single_u(struct __pyx_obj_10unipolator_31symmetric_unitary_interpolation_Sym_UI *__pyx_v_self, __pyx_t_double_complex *__pyx_v_u0) {
@@ -6047,39 +5990,50 @@
       __pyx_v_i = __pyx_t_5;
 
       /* "unipolator/symmetric_unitary_interpolation.pyx":182
  *             for k in range(self.n_dims_2):  # All except for the last element
  *                 i = k + 1
  *                 j = k + 2             # <<<<<<<<<<<<<<
  *                 self.ei = &self.E[indE, 0]
- *                 indE = findex_0(self.L, self.strides_E[j, :], self.n_dims) + self.first_elements_E[j]  # For E
+ *                 self.L[j] += self.d_location[j]
  */
       __pyx_t_10 = __Pyx_PyInt_AddObjC(__pyx_v_k, __pyx_int_2, 2, 0, 0); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 182, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_10); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 182, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       __pyx_v_j = __pyx_t_5;
 
       /* "unipolator/symmetric_unitary_interpolation.pyx":183
  *                 i = k + 1
  *                 j = k + 2
  *                 self.ei = &self.E[indE, 0]             # <<<<<<<<<<<<<<
- *                 indE = findex_0(self.L, self.strides_E[j, :], self.n_dims) + self.first_elements_E[j]  # For E
  *                 self.L[j] += self.d_location[j]
+ *                 indE = findex_0(self.L, self.strides_E[j, :], self.n_dims) + self.first_elements_E[j]  # For E
  */
       __pyx_t_2 = __pyx_v_indE;
       __pyx_t_3 = 0;
       __pyx_v_self->ei = (&(*((double *) ( /* dim=1 */ ((char *) (((double *) ( /* dim=0 */ (__pyx_v_self->E.data + __pyx_t_2 * __pyx_v_self->E.strides[0]) )) + __pyx_t_3)) ))));
 
       /* "unipolator/symmetric_unitary_interpolation.pyx":184
  *                 j = k + 2
  *                 self.ei = &self.E[indE, 0]
- *                 indE = findex_0(self.L, self.strides_E[j, :], self.n_dims) + self.first_elements_E[j]  # For E             # <<<<<<<<<<<<<<
+ *                 self.L[j] += self.d_location[j]             # <<<<<<<<<<<<<<
+ *                 indE = findex_0(self.L, self.strides_E[j, :], self.n_dims) + self.first_elements_E[j]  # For E
+ *                 if self.d_location[i]:  ### Higher
+ */
+      __pyx_t_3 = __pyx_v_j;
+      __pyx_t_2 = __pyx_v_j;
+      *((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->L.data) + __pyx_t_2)) )) += (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->d_location.data) + __pyx_t_3)) )));
+
+      /* "unipolator/symmetric_unitary_interpolation.pyx":185
+ *                 self.ei = &self.E[indE, 0]
  *                 self.L[j] += self.d_location[j]
+ *                 indE = findex_0(self.L, self.strides_E[j, :], self.n_dims) + self.first_elements_E[j]  # For E             # <<<<<<<<<<<<<<
  *                 if self.d_location[i]:  ### Higher
+ *                     self.L[i] += -1
  */
       __pyx_t_8.data = __pyx_v_self->strides_E.data;
       __pyx_t_8.memview = __pyx_v_self->strides_E.memview;
       __PYX_INC_MEMVIEW(&__pyx_t_8, 0);
       {
     Py_ssize_t __pyx_tmp_idx = __pyx_v_j;
     Py_ssize_t __pyx_tmp_stride = __pyx_v_self->strides_E.strides[0];
@@ -6092,38 +6046,27 @@
 
 __pyx_t_3 = __pyx_v_j;
       __pyx_v_indE = (__pyx_f_10unipolator_8indexing_findex_0(__pyx_v_self->L, __pyx_t_8, __pyx_v_self->n_dims, 0) + (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->first_elements_E.data) + __pyx_t_3)) ))));
       __PYX_XDEC_MEMVIEW(&__pyx_t_8, 1);
       __pyx_t_8.memview = NULL;
       __pyx_t_8.data = NULL;
 
-      /* "unipolator/symmetric_unitary_interpolation.pyx":185
- *                 self.ei = &self.E[indE, 0]
- *                 indE = findex_0(self.L, self.strides_E[j, :], self.n_dims) + self.first_elements_E[j]  # For E
- *                 self.L[j] += self.d_location[j]             # <<<<<<<<<<<<<<
- *                 if self.d_location[i]:  ### Higher
- *                     self.L[i] += -1
- */
-      __pyx_t_3 = __pyx_v_j;
-      __pyx_t_2 = __pyx_v_j;
-      *((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->L.data) + __pyx_t_2)) )) += (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->d_location.data) + __pyx_t_3)) )));
-
       /* "unipolator/symmetric_unitary_interpolation.pyx":186
- *                 indE = findex_0(self.L, self.strides_E[j, :], self.n_dims) + self.first_elements_E[j]  # For E
  *                 self.L[j] += self.d_location[j]
+ *                 indE = findex_0(self.L, self.strides_E[j, :], self.n_dims) + self.first_elements_E[j]  # For E
  *                 if self.d_location[i]:  ### Higher             # <<<<<<<<<<<<<<
  *                     self.L[i] += -1
  *                     ind = findex_0(self.L, self.strides_C[i, :], self.n_dims) + self.first_elements_C[i]
  */
       __pyx_t_3 = __pyx_v_i;
       __pyx_t_1 = ((*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->d_location.data) + __pyx_t_3)) ))) != 0);
       if (__pyx_t_1) {
 
         /* "unipolator/symmetric_unitary_interpolation.pyx":187
- *                 self.L[j] += self.d_location[j]
+ *                 indE = findex_0(self.L, self.strides_E[j, :], self.n_dims) + self.first_elements_E[j]  # For E
  *                 if self.d_location[i]:  ### Higher
  *                     self.L[i] += -1             # <<<<<<<<<<<<<<
  *                     ind = findex_0(self.L, self.strides_C[i, :], self.n_dims) + self.first_elements_C[i]
  *                     self.cl = &self.CL_L[ind, 0, 0]
  */
         __pyx_t_3 = __pyx_v_i;
         *((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->L.data) + __pyx_t_3)) )) += -1L;
@@ -6185,16 +6128,16 @@
  *                 else:  ### Lower
  *                     ind = findex_0(self.L, self.strides_C[i, :], self.n_dims) + self.first_elements_C[i]
  */
         __pyx_t_3 = __pyx_v_i;
         *((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->L.data) + __pyx_t_3)) )) += 1;
 
         /* "unipolator/symmetric_unitary_interpolation.pyx":186
- *                 indE = findex_0(self.L, self.strides_E[j, :], self.n_dims) + self.first_elements_E[j]  # For E
  *                 self.L[j] += self.d_location[j]
+ *                 indE = findex_0(self.L, self.strides_E[j, :], self.n_dims) + self.first_elements_E[j]  # For E
  *                 if self.d_location[i]:  ### Higher             # <<<<<<<<<<<<<<
  *                     self.L[i] += -1
  *                     ind = findex_0(self.L, self.strides_C[i, :], self.n_dims) + self.first_elements_C[i]
  */
         goto __pyx_L9;
       }
 
@@ -6364,15 +6307,15 @@
  *     cdef expmH_pointer(self, double[::1] c, double complex *u0):
  */
     __pyx_f_10unipolator_14blas_functions_MMM_cdot_pointer(__pyx_v_self->vl, __pyx_v_self->ur1, __pyx_v_self->vr, __pyx_v_u0, __pyx_v_self->ur2, __pyx_v_self->d);
   }
   __pyx_L3:;
 
   /* "unipolator/symmetric_unitary_interpolation.pyx":148
- *         return np.asarray(self.E_C), np.asarray(self.E), np.asarray(self.Vl), np.asarray(self.Vr), np.asarray(self.CL_L), np.asarray(self.CL_R), np.asarray(self.CH_L), np.asarray(self.CH_R), np.asarray(self.strides_EC), np.asarray(self.strides_E), np.asarray(self.strides_R), np.asarray(self.strides_C), np.asarray(self.first_elements_E), np.asarray(self.first_elements_C)
+ *         return np.asarray(self.E), np.asarray(self.Vl), np.asarray(self.Vr), np.asarray(self.CL_L), np.asarray(self.CL_R), np.asarray(self.CH_L), np.asarray(self.CH_R), np.asarray(self.strides_E), np.asarray(self.strides_L), np.asarray(self.strides_C), np.asarray(self.first_elements_E), np.asarray(self.first_elements_C)
  * 
  *     cdef interpolate_single_u(self, double complex *u0):  #u0 => input the matrices for output             # <<<<<<<<<<<<<<
  *         cdef int i, j
  *         cdef int ind, indE
  */
 
   /* function exit code */
@@ -6570,23 +6513,26 @@
   __Pyx_RefNannySetupContext("expmH", 0);
 
   /* "unipolator/symmetric_unitary_interpolation.pyx":215
  *         self.interpolate_single_u(u0)
  *     def expmH(self, double[::1] c, double complex[:,::1] U):
  *         cdef double complex *u0 = &U[0, 0]             # <<<<<<<<<<<<<<
  *         self.expmH_pointer(c, u0)
+ * 
  */
   __pyx_t_1 = 0;
   __pyx_t_2 = 0;
   __pyx_v_u0 = (&(*((__pyx_t_double_complex *) ( /* dim=1 */ ((char *) (((__pyx_t_double_complex *) ( /* dim=0 */ (__pyx_v_U.data + __pyx_t_1 * __pyx_v_U.strides[0]) )) + __pyx_t_2)) ))));
 
   /* "unipolator/symmetric_unitary_interpolation.pyx":216
  *     def expmH(self, double[::1] c, double complex[:,::1] U):
  *         cdef double complex *u0 = &U[0, 0]
  *         self.expmH_pointer(c, u0)             # <<<<<<<<<<<<<<
+ * 
+ *     def expmH_pulse_no_multiply(self, double[:,::1] cs, double complex[:,:,::1] U):
  */
   __pyx_t_3 = ((struct __pyx_vtabstruct_10unipolator_31symmetric_unitary_interpolation_Sym_UI *)__pyx_v_self->__pyx_vtab)->expmH_pointer(__pyx_v_self, __pyx_v_c, __pyx_v_u0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 216, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "unipolator/symmetric_unitary_interpolation.pyx":214
  *         self.single_parameters2oddgrid(c)
@@ -6607,35 +6553,275 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_c, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_v_U, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
+/* "unipolator/symmetric_unitary_interpolation.pyx":218
+ *         self.expmH_pointer(c, u0)
+ * 
+ *     def expmH_pulse_no_multiply(self, double[:,::1] cs, double complex[:,:,::1] U):             # <<<<<<<<<<<<<<
+ *         cdef double complex *u0 = &U[0, 0, 0]
+ *         cdef how_many = cs.shape[0]
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_10unipolator_31symmetric_unitary_interpolation_6Sym_UI_11expmH_pulse_no_multiply(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_10unipolator_31symmetric_unitary_interpolation_6Sym_UI_10expmH_pulse_no_multiply[] = "Sym_UI.expmH_pulse_no_multiply(self, double[:, ::1] cs, double complex[:, :, ::1] U)";
+static PyObject *__pyx_pw_10unipolator_31symmetric_unitary_interpolation_6Sym_UI_11expmH_pulse_no_multiply(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+  __Pyx_memviewslice __pyx_v_cs = { 0, 0, { 0 }, { 0 }, { 0 } };
+  __Pyx_memviewslice __pyx_v_U = { 0, 0, { 0 }, { 0 }, { 0 } };
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("expmH_pulse_no_multiply (wrapper)", 0);
+  {
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_cs,&__pyx_n_s_U,0};
+    PyObject* values[2] = {0,0};
+    if (unlikely(__pyx_kwds)) {
+      Py_ssize_t kw_args;
+      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
+      switch (pos_args) {
+        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
+        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = PyDict_Size(__pyx_kwds);
+      switch (pos_args) {
+        case  0:
+        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_cs)) != 0)) kw_args--;
+        else goto __pyx_L5_argtuple_error;
+        CYTHON_FALLTHROUGH;
+        case  1:
+        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_U)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("expmH_pulse_no_multiply", 1, 2, 2, 1); __PYX_ERR(0, 218, __pyx_L3_error)
+        }
+      }
+      if (unlikely(kw_args > 0)) {
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "expmH_pulse_no_multiply") < 0)) __PYX_ERR(0, 218, __pyx_L3_error)
+      }
+    } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
+      goto __pyx_L5_argtuple_error;
+    } else {
+      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+      values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+    }
+    __pyx_v_cs = __Pyx_PyObject_to_MemoryviewSlice_d_dc_double(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_cs.memview)) __PYX_ERR(0, 218, __pyx_L3_error)
+    __pyx_v_U = __Pyx_PyObject_to_MemoryviewSlice_d_d_dc___pyx_t_double_complex(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_U.memview)) __PYX_ERR(0, 218, __pyx_L3_error)
+  }
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("expmH_pulse_no_multiply", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 218, __pyx_L3_error)
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("unipolator.symmetric_unitary_interpolation.Sym_UI.expmH_pulse_no_multiply", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  __pyx_r = __pyx_pf_10unipolator_31symmetric_unitary_interpolation_6Sym_UI_10expmH_pulse_no_multiply(((struct __pyx_obj_10unipolator_31symmetric_unitary_interpolation_Sym_UI *)__pyx_v_self), __pyx_v_cs, __pyx_v_U);
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_10unipolator_31symmetric_unitary_interpolation_6Sym_UI_10expmH_pulse_no_multiply(struct __pyx_obj_10unipolator_31symmetric_unitary_interpolation_Sym_UI *__pyx_v_self, __Pyx_memviewslice __pyx_v_cs, __Pyx_memviewslice __pyx_v_U) {
+  __pyx_t_double_complex *__pyx_v_u0;
+  PyObject *__pyx_v_how_many = 0;
+  PyObject *__pyx_v_i = NULL;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  Py_ssize_t __pyx_t_1;
+  Py_ssize_t __pyx_t_2;
+  Py_ssize_t __pyx_t_3;
+  PyObject *__pyx_t_4 = NULL;
+  PyObject *__pyx_t_5 = NULL;
+  Py_ssize_t __pyx_t_6;
+  PyObject *(*__pyx_t_7)(PyObject *);
+  Py_ssize_t __pyx_t_8;
+  __Pyx_memviewslice __pyx_t_9 = { 0, 0, { 0 }, { 0 }, { 0 } };
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("expmH_pulse_no_multiply", 0);
+
+  /* "unipolator/symmetric_unitary_interpolation.pyx":219
+ * 
+ *     def expmH_pulse_no_multiply(self, double[:,::1] cs, double complex[:,:,::1] U):
+ *         cdef double complex *u0 = &U[0, 0, 0]             # <<<<<<<<<<<<<<
+ *         cdef how_many = cs.shape[0]
+ *         for i in range(how_many):
+ */
+  __pyx_t_1 = 0;
+  __pyx_t_2 = 0;
+  __pyx_t_3 = 0;
+  __pyx_v_u0 = (&(*((__pyx_t_double_complex *) ( /* dim=2 */ ((char *) (((__pyx_t_double_complex *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_U.data + __pyx_t_1 * __pyx_v_U.strides[0]) ) + __pyx_t_2 * __pyx_v_U.strides[1]) )) + __pyx_t_3)) ))));
+
+  /* "unipolator/symmetric_unitary_interpolation.pyx":220
+ *     def expmH_pulse_no_multiply(self, double[:,::1] cs, double complex[:,:,::1] U):
+ *         cdef double complex *u0 = &U[0, 0, 0]
+ *         cdef how_many = cs.shape[0]             # <<<<<<<<<<<<<<
+ *         for i in range(how_many):
+ *             self.expmH_pointer(cs[i,:], u0)
+ */
+  __pyx_t_4 = PyInt_FromSsize_t((__pyx_v_cs.shape[0])); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 220, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_v_how_many = __pyx_t_4;
+  __pyx_t_4 = 0;
+
+  /* "unipolator/symmetric_unitary_interpolation.pyx":221
+ *         cdef double complex *u0 = &U[0, 0, 0]
+ *         cdef how_many = cs.shape[0]
+ *         for i in range(how_many):             # <<<<<<<<<<<<<<
+ *             self.expmH_pointer(cs[i,:], u0)
+ *             u0 += self.d2
+ */
+  __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_range, __pyx_v_how_many); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 221, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  if (likely(PyList_CheckExact(__pyx_t_4)) || PyTuple_CheckExact(__pyx_t_4)) {
+    __pyx_t_5 = __pyx_t_4; __Pyx_INCREF(__pyx_t_5); __pyx_t_6 = 0;
+    __pyx_t_7 = NULL;
+  } else {
+    __pyx_t_6 = -1; __pyx_t_5 = PyObject_GetIter(__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 221, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_t_7 = Py_TYPE(__pyx_t_5)->tp_iternext; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 221, __pyx_L1_error)
+  }
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  for (;;) {
+    if (likely(!__pyx_t_7)) {
+      if (likely(PyList_CheckExact(__pyx_t_5))) {
+        if (__pyx_t_6 >= PyList_GET_SIZE(__pyx_t_5)) break;
+        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_5, __pyx_t_6); __Pyx_INCREF(__pyx_t_4); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 221, __pyx_L1_error)
+        #else
+        __pyx_t_4 = PySequence_ITEM(__pyx_t_5, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 221, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_4);
+        #endif
+      } else {
+        if (__pyx_t_6 >= PyTuple_GET_SIZE(__pyx_t_5)) break;
+        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_5, __pyx_t_6); __Pyx_INCREF(__pyx_t_4); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 221, __pyx_L1_error)
+        #else
+        __pyx_t_4 = PySequence_ITEM(__pyx_t_5, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 221, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_4);
+        #endif
+      }
+    } else {
+      __pyx_t_4 = __pyx_t_7(__pyx_t_5);
+      if (unlikely(!__pyx_t_4)) {
+        PyObject* exc_type = PyErr_Occurred();
+        if (exc_type) {
+          if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
+          else __PYX_ERR(0, 221, __pyx_L1_error)
+        }
+        break;
+      }
+      __Pyx_GOTREF(__pyx_t_4);
+    }
+    __Pyx_XDECREF_SET(__pyx_v_i, __pyx_t_4);
+    __pyx_t_4 = 0;
+
+    /* "unipolator/symmetric_unitary_interpolation.pyx":222
+ *         cdef how_many = cs.shape[0]
+ *         for i in range(how_many):
+ *             self.expmH_pointer(cs[i,:], u0)             # <<<<<<<<<<<<<<
+ *             u0 += self.d2
+ */
+    __pyx_t_8 = __Pyx_PyIndex_AsSsize_t(__pyx_v_i); if (unlikely((__pyx_t_8 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 222, __pyx_L1_error)
+    __pyx_t_9.data = __pyx_v_cs.data;
+    __pyx_t_9.memview = __pyx_v_cs.memview;
+    __PYX_INC_MEMVIEW(&__pyx_t_9, 0);
+    {
+    Py_ssize_t __pyx_tmp_idx = __pyx_t_8;
+    Py_ssize_t __pyx_tmp_stride = __pyx_v_cs.strides[0];
+        __pyx_t_9.data += __pyx_tmp_idx * __pyx_tmp_stride;
+}
+
+__pyx_t_9.shape[0] = __pyx_v_cs.shape[1];
+__pyx_t_9.strides[0] = __pyx_v_cs.strides[1];
+    __pyx_t_9.suboffsets[0] = -1;
+
+__pyx_t_4 = ((struct __pyx_vtabstruct_10unipolator_31symmetric_unitary_interpolation_Sym_UI *)__pyx_v_self->__pyx_vtab)->expmH_pointer(__pyx_v_self, __pyx_t_9, __pyx_v_u0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 222, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __PYX_XDEC_MEMVIEW(&__pyx_t_9, 1);
+    __pyx_t_9.memview = NULL;
+    __pyx_t_9.data = NULL;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+
+    /* "unipolator/symmetric_unitary_interpolation.pyx":223
+ *         for i in range(how_many):
+ *             self.expmH_pointer(cs[i,:], u0)
+ *             u0 += self.d2             # <<<<<<<<<<<<<<
+ */
+    __pyx_v_u0 = (__pyx_v_u0 + __pyx_v_self->d2);
+
+    /* "unipolator/symmetric_unitary_interpolation.pyx":221
+ *         cdef double complex *u0 = &U[0, 0, 0]
+ *         cdef how_many = cs.shape[0]
+ *         for i in range(how_many):             # <<<<<<<<<<<<<<
+ *             self.expmH_pointer(cs[i,:], u0)
+ *             u0 += self.d2
+ */
+  }
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+
+  /* "unipolator/symmetric_unitary_interpolation.pyx":218
+ *         self.expmH_pointer(c, u0)
+ * 
+ *     def expmH_pulse_no_multiply(self, double[:,::1] cs, double complex[:,:,::1] U):             # <<<<<<<<<<<<<<
+ *         cdef double complex *u0 = &U[0, 0, 0]
+ *         cdef how_many = cs.shape[0]
+ */
+
+  /* function exit code */
+  __pyx_r = Py_None; __Pyx_INCREF(Py_None);
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_5);
+  __PYX_XDEC_MEMVIEW(&__pyx_t_9, 1);
+  __Pyx_AddTraceback("unipolator.symmetric_unitary_interpolation.Sym_UI.expmH_pulse_no_multiply", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_how_many);
+  __Pyx_XDECREF(__pyx_v_i);
+  __PYX_XDEC_MEMVIEW(&__pyx_v_cs, 1);
+  __PYX_XDEC_MEMVIEW(&__pyx_v_U, 1);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
 /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_10unipolator_31symmetric_unitary_interpolation_6Sym_UI_11__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static char __pyx_doc_10unipolator_31symmetric_unitary_interpolation_6Sym_UI_10__reduce_cython__[] = "Sym_UI.__reduce_cython__(self)";
-static PyObject *__pyx_pw_10unipolator_31symmetric_unitary_interpolation_6Sym_UI_11__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_10unipolator_31symmetric_unitary_interpolation_6Sym_UI_13__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc_10unipolator_31symmetric_unitary_interpolation_6Sym_UI_12__reduce_cython__[] = "Sym_UI.__reduce_cython__(self)";
+static PyObject *__pyx_pw_10unipolator_31symmetric_unitary_interpolation_6Sym_UI_13__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_10unipolator_31symmetric_unitary_interpolation_6Sym_UI_10__reduce_cython__(((struct __pyx_obj_10unipolator_31symmetric_unitary_interpolation_Sym_UI *)__pyx_v_self));
+  __pyx_r = __pyx_pf_10unipolator_31symmetric_unitary_interpolation_6Sym_UI_12__reduce_cython__(((struct __pyx_obj_10unipolator_31symmetric_unitary_interpolation_Sym_UI *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_10unipolator_31symmetric_unitary_interpolation_6Sym_UI_10__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_10unipolator_31symmetric_unitary_interpolation_Sym_UI *__pyx_v_self) {
+static PyObject *__pyx_pf_10unipolator_31symmetric_unitary_interpolation_6Sym_UI_12__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_10unipolator_31symmetric_unitary_interpolation_Sym_UI *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__reduce_cython__", 0);
@@ -6672,28 +6858,28 @@
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_10unipolator_31symmetric_unitary_interpolation_6Sym_UI_13__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
-static char __pyx_doc_10unipolator_31symmetric_unitary_interpolation_6Sym_UI_12__setstate_cython__[] = "Sym_UI.__setstate_cython__(self, __pyx_state)";
-static PyObject *__pyx_pw_10unipolator_31symmetric_unitary_interpolation_6Sym_UI_13__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pw_10unipolator_31symmetric_unitary_interpolation_6Sym_UI_15__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
+static char __pyx_doc_10unipolator_31symmetric_unitary_interpolation_6Sym_UI_14__setstate_cython__[] = "Sym_UI.__setstate_cython__(self, __pyx_state)";
+static PyObject *__pyx_pw_10unipolator_31symmetric_unitary_interpolation_6Sym_UI_15__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_10unipolator_31symmetric_unitary_interpolation_6Sym_UI_12__setstate_cython__(((struct __pyx_obj_10unipolator_31symmetric_unitary_interpolation_Sym_UI *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
+  __pyx_r = __pyx_pf_10unipolator_31symmetric_unitary_interpolation_6Sym_UI_14__setstate_cython__(((struct __pyx_obj_10unipolator_31symmetric_unitary_interpolation_Sym_UI *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_10unipolator_31symmetric_unitary_interpolation_6Sym_UI_12__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_10unipolator_31symmetric_unitary_interpolation_Sym_UI *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pf_10unipolator_31symmetric_unitary_interpolation_6Sym_UI_14__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_10unipolator_31symmetric_unitary_interpolation_Sym_UI *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
@@ -20802,16 +20988,14 @@
   p->c_maxs.memview = NULL;
   p->dcs.data = NULL;
   p->dcs.memview = NULL;
   p->das.data = NULL;
   p->das.memview = NULL;
   p->c_bins.data = NULL;
   p->c_bins.memview = NULL;
-  p->E_C.data = NULL;
-  p->E_C.memview = NULL;
   p->E.data = NULL;
   p->E.memview = NULL;
   p->Vr.data = NULL;
   p->Vr.memview = NULL;
   p->Vl.data = NULL;
   p->Vl.memview = NULL;
   p->CL_L.data = NULL;
@@ -20834,16 +21018,14 @@
   p->Ur2.memview = NULL;
   p->dUc.data = NULL;
   p->dUc.memview = NULL;
   p->expE.data = NULL;
   p->expE.memview = NULL;
   p->strides_L.data = NULL;
   p->strides_L.memview = NULL;
-  p->strides_EC.data = NULL;
-  p->strides_EC.memview = NULL;
   p->strides_E.data = NULL;
   p->strides_E.memview = NULL;
   p->strides_C.data = NULL;
   p->strides_C.memview = NULL;
   p->location.data = NULL;
   p->location.memview = NULL;
   p->d_location.data = NULL;
@@ -20875,15 +21057,14 @@
   }
   #endif
   __PYX_XDEC_MEMVIEW(&p->c_mins, 1);
   __PYX_XDEC_MEMVIEW(&p->c_maxs, 1);
   __PYX_XDEC_MEMVIEW(&p->dcs, 1);
   __PYX_XDEC_MEMVIEW(&p->das, 1);
   __PYX_XDEC_MEMVIEW(&p->c_bins, 1);
-  __PYX_XDEC_MEMVIEW(&p->E_C, 1);
   __PYX_XDEC_MEMVIEW(&p->E, 1);
   __PYX_XDEC_MEMVIEW(&p->Vr, 1);
   __PYX_XDEC_MEMVIEW(&p->Vl, 1);
   __PYX_XDEC_MEMVIEW(&p->CL_L, 1);
   __PYX_XDEC_MEMVIEW(&p->CH_L, 1);
   __PYX_XDEC_MEMVIEW(&p->CL_R, 1);
   __PYX_XDEC_MEMVIEW(&p->CH_R, 1);
@@ -20891,15 +21072,14 @@
   __PYX_XDEC_MEMVIEW(&p->dUr, 1);
   __PYX_XDEC_MEMVIEW(&p->Ur, 1);
   __PYX_XDEC_MEMVIEW(&p->Ur1, 1);
   __PYX_XDEC_MEMVIEW(&p->Ur2, 1);
   __PYX_XDEC_MEMVIEW(&p->dUc, 1);
   __PYX_XDEC_MEMVIEW(&p->expE, 1);
   __PYX_XDEC_MEMVIEW(&p->strides_L, 1);
-  __PYX_XDEC_MEMVIEW(&p->strides_EC, 1);
   __PYX_XDEC_MEMVIEW(&p->strides_E, 1);
   __PYX_XDEC_MEMVIEW(&p->strides_C, 1);
   __PYX_XDEC_MEMVIEW(&p->location, 1);
   __PYX_XDEC_MEMVIEW(&p->d_location, 1);
   __PYX_XDEC_MEMVIEW(&p->abs_alpha_rest, 1);
   __PYX_XDEC_MEMVIEW(&p->alpha, 1);
   __PYX_XDEC_MEMVIEW(&p->first_elements_E, 1);
@@ -20910,16 +21090,17 @@
 }
 
 static PyMethodDef __pyx_methods_10unipolator_31symmetric_unitary_interpolation_Sym_UI[] = {
   {"set_which_diffs", (PyCFunction)__pyx_pw_10unipolator_31symmetric_unitary_interpolation_6Sym_UI_3set_which_diffs, METH_O, __pyx_doc_10unipolator_31symmetric_unitary_interpolation_6Sym_UI_2set_which_diffs},
   {"get_single_param", (PyCFunction)__pyx_pw_10unipolator_31symmetric_unitary_interpolation_6Sym_UI_5get_single_param, METH_O, __pyx_doc_10unipolator_31symmetric_unitary_interpolation_6Sym_UI_4get_single_param},
   {"get_cache", (PyCFunction)__pyx_pw_10unipolator_31symmetric_unitary_interpolation_6Sym_UI_7get_cache, METH_NOARGS, __pyx_doc_10unipolator_31symmetric_unitary_interpolation_6Sym_UI_6get_cache},
   {"expmH", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_10unipolator_31symmetric_unitary_interpolation_6Sym_UI_9expmH, METH_VARARGS|METH_KEYWORDS, __pyx_doc_10unipolator_31symmetric_unitary_interpolation_6Sym_UI_8expmH},
-  {"__reduce_cython__", (PyCFunction)__pyx_pw_10unipolator_31symmetric_unitary_interpolation_6Sym_UI_11__reduce_cython__, METH_NOARGS, __pyx_doc_10unipolator_31symmetric_unitary_interpolation_6Sym_UI_10__reduce_cython__},
-  {"__setstate_cython__", (PyCFunction)__pyx_pw_10unipolator_31symmetric_unitary_interpolation_6Sym_UI_13__setstate_cython__, METH_O, __pyx_doc_10unipolator_31symmetric_unitary_interpolation_6Sym_UI_12__setstate_cython__},
+  {"expmH_pulse_no_multiply", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_10unipolator_31symmetric_unitary_interpolation_6Sym_UI_11expmH_pulse_no_multiply, METH_VARARGS|METH_KEYWORDS, __pyx_doc_10unipolator_31symmetric_unitary_interpolation_6Sym_UI_10expmH_pulse_no_multiply},
+  {"__reduce_cython__", (PyCFunction)__pyx_pw_10unipolator_31symmetric_unitary_interpolation_6Sym_UI_13__reduce_cython__, METH_NOARGS, __pyx_doc_10unipolator_31symmetric_unitary_interpolation_6Sym_UI_12__reduce_cython__},
+  {"__setstate_cython__", (PyCFunction)__pyx_pw_10unipolator_31symmetric_unitary_interpolation_6Sym_UI_15__setstate_cython__, METH_O, __pyx_doc_10unipolator_31symmetric_unitary_interpolation_6Sym_UI_14__setstate_cython__},
   {0, 0, 0, 0}
 };
 
 static PyTypeObject __pyx_type_10unipolator_31symmetric_unitary_interpolation_Sym_UI = {
   PyVarObject_HEAD_INIT(0, 0)
   "unipolator.symmetric_unitary_interpolation.Sym_UI", /*tp_name*/
   sizeof(struct __pyx_obj_10unipolator_31symmetric_unitary_interpolation_Sym_UI), /*tp_basicsize*/
@@ -21806,14 +21987,15 @@
   {&__pyx_n_s_c_max_s, __pyx_k_c_max_s, sizeof(__pyx_k_c_max_s), 0, 0, 1, 1},
   {&__pyx_n_s_c_min_s, __pyx_k_c_min_s, sizeof(__pyx_k_c_min_s), 0, 0, 1, 1},
   {&__pyx_n_s_class, __pyx_k_class, sizeof(__pyx_k_class), 0, 0, 1, 1},
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
   {&__pyx_n_s_complex128, __pyx_k_complex128, sizeof(__pyx_k_complex128), 0, 0, 1, 1},
   {&__pyx_kp_s_contiguous_and_direct, __pyx_k_contiguous_and_direct, sizeof(__pyx_k_contiguous_and_direct), 0, 0, 1, 0},
   {&__pyx_kp_s_contiguous_and_indirect, __pyx_k_contiguous_and_indirect, sizeof(__pyx_k_contiguous_and_indirect), 0, 0, 1, 0},
+  {&__pyx_n_s_cs, __pyx_k_cs, sizeof(__pyx_k_cs), 0, 0, 1, 1},
   {&__pyx_n_s_dict, __pyx_k_dict, sizeof(__pyx_k_dict), 0, 0, 1, 1},
   {&__pyx_n_s_double, __pyx_k_double, sizeof(__pyx_k_double), 0, 0, 1, 1},
   {&__pyx_n_s_dtype, __pyx_k_dtype, sizeof(__pyx_k_dtype), 0, 0, 1, 1},
   {&__pyx_n_s_dtype_is_object, __pyx_k_dtype_is_object, sizeof(__pyx_k_dtype_is_object), 0, 0, 1, 1},
   {&__pyx_n_s_empty, __pyx_k_empty, sizeof(__pyx_k_empty), 0, 0, 1, 1},
   {&__pyx_n_s_encode, __pyx_k_encode, sizeof(__pyx_k_encode), 0, 0, 1, 1},
   {&__pyx_n_s_enumerate, __pyx_k_enumerate, sizeof(__pyx_k_enumerate), 0, 0, 1, 1},
@@ -21862,15 +22044,14 @@
   {&__pyx_n_s_size, __pyx_k_size, sizeof(__pyx_k_size), 0, 0, 1, 1},
   {&__pyx_n_s_start, __pyx_k_start, sizeof(__pyx_k_start), 0, 0, 1, 1},
   {&__pyx_n_s_step, __pyx_k_step, sizeof(__pyx_k_step), 0, 0, 1, 1},
   {&__pyx_n_s_stop, __pyx_k_stop, sizeof(__pyx_k_stop), 0, 0, 1, 1},
   {&__pyx_kp_s_strided_and_direct, __pyx_k_strided_and_direct, sizeof(__pyx_k_strided_and_direct), 0, 0, 1, 0},
   {&__pyx_kp_s_strided_and_direct_or_indirect, __pyx_k_strided_and_direct_or_indirect, sizeof(__pyx_k_strided_and_direct_or_indirect), 0, 0, 1, 0},
   {&__pyx_kp_s_strided_and_indirect, __pyx_k_strided_and_indirect, sizeof(__pyx_k_strided_and_indirect), 0, 0, 1, 0},
-  {&__pyx_n_s_strides_R, __pyx_k_strides_R, sizeof(__pyx_k_strides_R), 0, 0, 1, 1},
   {&__pyx_kp_s_stringsource, __pyx_k_stringsource, sizeof(__pyx_k_stringsource), 0, 0, 1, 0},
   {&__pyx_n_s_struct, __pyx_k_struct, sizeof(__pyx_k_struct), 0, 0, 1, 1},
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
   {&__pyx_kp_u_to_1, __pyx_k_to_1, sizeof(__pyx_k_to_1), 0, 1, 0, 0},
   {&__pyx_kp_s_unable_to_allocate_array_data, __pyx_k_unable_to_allocate_array_data, sizeof(__pyx_k_unable_to_allocate_array_data), 0, 0, 1, 0},
   {&__pyx_kp_s_unable_to_allocate_shape_and_str, __pyx_k_unable_to_allocate_shape_and_str, sizeof(__pyx_k_unable_to_allocate_shape_and_str), 0, 0, 1, 0},
   {&__pyx_n_s_unpack, __pyx_k_unpack, sizeof(__pyx_k_unpack), 0, 0, 1, 1},
@@ -26225,14 +26406,37 @@
     return result;
 __pyx_fail:
     result.memview = NULL;
     result.data = NULL;
     return result;
 }
 
+/* ObjectToMemviewSlice */
+  static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_d_dc_double(PyObject *obj, int writable_flag) {
+    __Pyx_memviewslice result = { 0, 0, { 0 }, { 0 }, { 0 } };
+    __Pyx_BufFmt_StackElem stack[1];
+    int axes_specs[] = { (__Pyx_MEMVIEW_DIRECT | __Pyx_MEMVIEW_FOLLOW), (__Pyx_MEMVIEW_DIRECT | __Pyx_MEMVIEW_CONTIG) };
+    int retcode;
+    if (obj == Py_None) {
+        result.memview = (struct __pyx_memoryview_obj *) Py_None;
+        return result;
+    }
+    retcode = __Pyx_ValidateAndInit_memviewslice(axes_specs, __Pyx_IS_C_CONTIG,
+                                                 (PyBUF_C_CONTIGUOUS | PyBUF_FORMAT) | writable_flag, 2,
+                                                 &__Pyx_TypeInfo_double, stack,
+                                                 &result, obj);
+    if (unlikely(retcode == -1))
+        goto __pyx_fail;
+    return result;
+__pyx_fail:
+    result.memview = NULL;
+    result.data = NULL;
+    return result;
+}
+
 /* FromPy */
   static __pyx_t_double_complex __Pyx_PyComplex_As___pyx_t_double_complex(PyObject* o) {
     Py_complex cval;
 #if !CYTHON_COMPILING_IN_PYPY
     if (PyComplex_CheckExact(o))
         cval = ((PyComplexObject *)o)->cval;
     else
@@ -26252,37 +26456,14 @@
     if (PyErr_Occurred())
         return 0;
     *(__pyx_t_double_complex *) itemp = value;
     return 1;
 }
 
 /* ObjectToMemviewSlice */
-  static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_d_dc_double(PyObject *obj, int writable_flag) {
-    __Pyx_memviewslice result = { 0, 0, { 0 }, { 0 }, { 0 } };
-    __Pyx_BufFmt_StackElem stack[1];
-    int axes_specs[] = { (__Pyx_MEMVIEW_DIRECT | __Pyx_MEMVIEW_FOLLOW), (__Pyx_MEMVIEW_DIRECT | __Pyx_MEMVIEW_CONTIG) };
-    int retcode;
-    if (obj == Py_None) {
-        result.memview = (struct __pyx_memoryview_obj *) Py_None;
-        return result;
-    }
-    retcode = __Pyx_ValidateAndInit_memviewslice(axes_specs, __Pyx_IS_C_CONTIG,
-                                                 (PyBUF_C_CONTIGUOUS | PyBUF_FORMAT) | writable_flag, 2,
-                                                 &__Pyx_TypeInfo_double, stack,
-                                                 &result, obj);
-    if (unlikely(retcode == -1))
-        goto __pyx_fail;
-    return result;
-__pyx_fail:
-    result.memview = NULL;
-    result.data = NULL;
-    return result;
-}
-
-/* ObjectToMemviewSlice */
   static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_d_dc_long(PyObject *obj, int writable_flag) {
     __Pyx_memviewslice result = { 0, 0, { 0 }, { 0 }, { 0 } };
     __Pyx_BufFmt_StackElem stack[1];
     int axes_specs[] = { (__Pyx_MEMVIEW_DIRECT | __Pyx_MEMVIEW_FOLLOW), (__Pyx_MEMVIEW_DIRECT | __Pyx_MEMVIEW_CONTIG) };
     int retcode;
     if (obj == Py_None) {
         result.memview = (struct __pyx_memoryview_obj *) Py_None;
```

### Comparing `unipolator-0.2.6/src/unipolator/symmetric_unitary_interpolation.pyx` & `unipolator-0.2.7/src/unipolator/symmetric_unitary_interpolation.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 # Unitary Interpolation
 cdef class Sym_UI:
     # Initialize variables, to quickly calculate interpolations while minimizing memmory allocation overheads
     cdef double[::1] c_mins, c_maxs, dcs, das
     cdef long[::1] c_bins
     cdef int n_dims, d, d2, n_dims_1, n_dims_2, n_d_di_1, n_d_di, i
-    cdef double[:, ::1] E_C, E
+    cdef double[:, ::1] E
     cdef double complex[:,:,::1] Vr, Vl, CL_L, CH_L, CL_R, CH_R, dUl, dUr
     cdef double complex[:,::1] Ur, Ur1, Ur2, dUc
     cdef double complex[::1] expE
     cdef double *ei
     cdef double complex *expe
     cdef double complex *vl
     cdef double complex *vr
@@ -26,15 +26,15 @@
     cdef double complex *cr
     cdef double complex *ur0
     cdef double complex *ur1
     cdef double complex *ur2
     cdef double complex *dul
     cdef double complex *dur
     cdef double complex *duc
-    cdef long[::1] strides_L, strides_EC
+    cdef long[::1] strides_L
     cdef long[:,::1] strides_E, strides_C
     cdef long[::1] location, d_location
     cdef double[::1] abs_alpha_rest, alpha
     cdef long[::1] first_elements_E, first_elements_C, L, 
     cdef long[::1] d_di
     def __cinit__(self, double complex[:,:,::1] H_s, double[::1] c_min_s, double[::1] c_max_s, long[::1] c_bins, long[::1] which_diffs = np.array([], dtype=long)):
         # Construct parameters
@@ -68,15 +68,15 @@
         # Construct interpolation grid points
         H_s2 = H_s.copy()
         d_third_order_tensor_scale(H_s2, 0.5 )
         U_grid2, cum_prod = Unitary_Grid(H_s2, self.c_mins, self.dcs, self.c_bins) # Half grid -> H_s2 = H_s / 2
         ## Construct interpolation cache
         self.E, self.Vl, self.Vr, self.CL_L, self.CL_R, self.CH_L, self.CH_R, self.strides_E, self.strides_L, self.strides_C, self.first_elements_E, self.first_elements_C = Create_Sym_Interpolation_Cache( U_grid2, cum_prod, self.c_bins)
 
-        self.ei = &self.E_C[0, 0]
+        self.ei = &self.E[0, 0]
         self.vl = &self.Vl[0, 0, 0]
         self.vr = &self.Vr[0, 0, 0]
         self.cl = &self.CL_L[0, 0, 0]
         self.cr = &self.CL_R[0, 0, 0]
         self.Ur = np.empty([self.d, self.d], dtype=np.complex128)
         self.ur0 = &self.Ur[0, 0]
         self.Ur1 = np.empty([self.d, self.d], dtype=np.complex128)
@@ -139,15 +139,15 @@
         self.n_d_di = self.d_di.shape[0]
 
     def get_single_param(self, double[::1] c): # To verify interpolation grid
         self.single_parameters2oddgrid(c)
         return np.asarray(self.location), np.asarray(self.d_location), np.asarray(self.abs_alpha_rest)
 
     def get_cache(self): # To verify interpolation grid
-        return np.asarray(self.E_C), np.asarray(self.E), np.asarray(self.Vl), np.asarray(self.Vr), np.asarray(self.CL_L), np.asarray(self.CL_R), np.asarray(self.CH_L), np.asarray(self.CH_R), np.asarray(self.strides_EC), np.asarray(self.strides_E), np.asarray(self.strides_R), np.asarray(self.strides_C), np.asarray(self.first_elements_E), np.asarray(self.first_elements_C)
+        return np.asarray(self.E), np.asarray(self.Vl), np.asarray(self.Vr), np.asarray(self.CL_L), np.asarray(self.CL_R), np.asarray(self.CH_L), np.asarray(self.CH_R), np.asarray(self.strides_E), np.asarray(self.strides_L), np.asarray(self.strides_C), np.asarray(self.first_elements_E), np.asarray(self.first_elements_C)
 
     cdef interpolate_single_u(self, double complex *u0):  #u0 => input the matrices for output
         cdef int i, j
         cdef int ind, indE
         if self.n_dims == 1:  # Shouldn't make any difference if you use symmetric 1D or non symmetric 1D interpolation
             ind = self.location[0] + self.d_location[0]
             self.vr = &self.Vr[ind, 0, 0]  # In 1D strides are 1
@@ -177,16 +177,16 @@
             self.L[1] = self.location[1]
             V_expE_W_pointer(self.cl, self.cr, self.ei, self.abs_alpha_rest[0], self.ur0, self.ur1, self.d, self.d2)  # Save onto self.ur1
             # Now outward
             for k in range(self.n_dims_2):  # All except for the last element
                 i = k + 1
                 j = k + 2
                 self.ei = &self.E[indE, 0]
-                indE = findex_0(self.L, self.strides_E[j, :], self.n_dims) + self.first_elements_E[j]  # For E
                 self.L[j] += self.d_location[j]
+                indE = findex_0(self.L, self.strides_E[j, :], self.n_dims) + self.first_elements_E[j]  # For E
                 if self.d_location[i]:  ### Higher
                     self.L[i] += -1
                     ind = findex_0(self.L, self.strides_C[i, :], self.n_dims) + self.first_elements_C[i]
                     self.cl = &self.CL_L[ind, 0, 0]
                     self.cr = &self.CL_R[ind, 0, 0]
                     self.L[i] += 1 # Restore value
                 else:  ### Lower
@@ -210,7 +210,14 @@
         if not c.shape[0] == self.n_dims:
             raise ValueError('The coefficient c must be of size [interpolation_dimensions].')
         self.single_parameters2oddgrid(c)
         self.interpolate_single_u(u0)
     def expmH(self, double[::1] c, double complex[:,::1] U):
         cdef double complex *u0 = &U[0, 0]
         self.expmH_pointer(c, u0)
+
+    def expmH_pulse_no_multiply(self, double[:,::1] cs, double complex[:,:,::1] U):
+        cdef double complex *u0 = &U[0, 0, 0]
+        cdef how_many = cs.shape[0]
+        for i in range(how_many):
+            self.expmH_pointer(cs[i,:], u0)
+            u0 += self.d2
```

### Comparing `unipolator-0.2.6/src/unipolator/trotter_system.c` & `unipolator-0.2.7/src/unipolator/trotter_system.c`

 * *Files 1% similar despite different names*

```diff
@@ -2349,24 +2349,24 @@
 
 /* ObjectToMemviewSlice.proto */
 static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_dc_double(PyObject *, int writable_flag);
 
 /* ObjectToMemviewSlice.proto */
 static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_d_dc___pyx_t_double_complex(PyObject *, int writable_flag);
 
+/* ObjectToMemviewSlice.proto */
+static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_d_dc_double(PyObject *, int writable_flag);
+
 /* IntPow.proto */
 static CYTHON_INLINE long __Pyx_pow_long(long, long);
 
 /* ObjectToMemviewSlice.proto */
 static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_dc___pyx_t_double_complex(PyObject *, int writable_flag);
 
 /* ObjectToMemviewSlice.proto */
-static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_d_dc_double(PyObject *, int writable_flag);
-
-/* ObjectToMemviewSlice.proto */
 static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_dc_int(PyObject *, int writable_flag);
 
 /* ToPy.proto */
 #define __pyx_PyComplex_FromComplex(z)\
         PyComplex_FromDoubles((double)__Pyx_CREAL(z),\
                               (double)__Pyx_CIMAG(z))
 
@@ -2581,14 +2581,15 @@
 static PyObject *__pyx_builtin_enumerate;
 static PyObject *__pyx_builtin_Ellipsis;
 static PyObject *__pyx_builtin_id;
 static PyObject *__pyx_builtin_IndexError;
 static const char __pyx_k_O[] = "O";
 static const char __pyx_k_U[] = "U";
 static const char __pyx_k_c[] = "c";
+static const char __pyx_k_cs[] = "cs";
 static const char __pyx_k_id[] = "id";
 static const char __pyx_k_np[] = "np";
 static const char __pyx_k_H_s[] = "H_s";
 static const char __pyx_k_new[] = "__new__";
 static const char __pyx_k_obj[] = "obj";
 static const char __pyx_k_base[] = "base";
 static const char __pyx_k_dict[] = "__dict__";
@@ -2719,14 +2720,15 @@
 static PyObject *__pyx_n_u_c;
 static PyObject *__pyx_kp_u_c_shape_0_needs_to_be_equal_to_H;
 static PyObject *__pyx_n_s_class;
 static PyObject *__pyx_n_s_cline_in_traceback;
 static PyObject *__pyx_n_s_complex128;
 static PyObject *__pyx_kp_s_contiguous_and_direct;
 static PyObject *__pyx_kp_s_contiguous_and_indirect;
+static PyObject *__pyx_n_s_cs;
 static PyObject *__pyx_n_s_dict;
 static PyObject *__pyx_n_s_double;
 static PyObject *__pyx_n_s_dtype;
 static PyObject *__pyx_n_s_dtype_is_object;
 static PyObject *__pyx_n_s_empty;
 static PyObject *__pyx_n_s_encode;
 static PyObject *__pyx_n_s_enumerate;
@@ -2787,16 +2789,17 @@
 static PyObject *__pyx_kp_s_unable_to_allocate_shape_and_str;
 static PyObject *__pyx_n_s_unpack;
 static PyObject *__pyx_n_s_update;
 static PyObject *__pyx_n_s_which_diffs;
 static int __pyx_pf_10unipolator_14trotter_system_14Trotter_System___cinit__(struct __pyx_obj_10unipolator_14trotter_system_Trotter_System *__pyx_v_self, __Pyx_memviewslice __pyx_v_H_s, __Pyx_memviewslice __pyx_v_which_diffs, int __pyx_v_m_times); /* proto */
 static PyObject *__pyx_pf_10unipolator_14trotter_system_14Trotter_System_2get_cache(struct __pyx_obj_10unipolator_14trotter_system_Trotter_System *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_10unipolator_14trotter_system_14Trotter_System_4expmH(struct __pyx_obj_10unipolator_14trotter_system_Trotter_System *__pyx_v_self, __Pyx_memviewslice __pyx_v_c, __Pyx_memviewslice __pyx_v_U); /* proto */
-static PyObject *__pyx_pf_10unipolator_14trotter_system_14Trotter_System_6__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_10unipolator_14trotter_system_Trotter_System *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_10unipolator_14trotter_system_14Trotter_System_8__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_10unipolator_14trotter_system_Trotter_System *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
+static PyObject *__pyx_pf_10unipolator_14trotter_system_14Trotter_System_6expmH_pulse_no_multiply(struct __pyx_obj_10unipolator_14trotter_system_Trotter_System *__pyx_v_self, __Pyx_memviewslice __pyx_v_cs, __Pyx_memviewslice __pyx_v_U); /* proto */
+static PyObject *__pyx_pf_10unipolator_14trotter_system_14Trotter_System_8__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_10unipolator_14trotter_system_Trotter_System *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_10unipolator_14trotter_system_14Trotter_System_10__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_10unipolator_14trotter_system_Trotter_System *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
 static int __pyx_array___pyx_pf_15View_dot_MemoryView_5array___cinit__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_shape, Py_ssize_t __pyx_v_itemsize, PyObject *__pyx_v_format, PyObject *__pyx_v_mode, int __pyx_v_allocate_buffer); /* proto */
 static int __pyx_array___pyx_pf_15View_dot_MemoryView_5array_2__getbuffer__(struct __pyx_array_obj *__pyx_v_self, Py_buffer *__pyx_v_info, int __pyx_v_flags); /* proto */
 static void __pyx_array___pyx_pf_15View_dot_MemoryView_5array_4__dealloc__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_15View_dot_MemoryView_5array_7memview___get__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static Py_ssize_t __pyx_array___pyx_pf_15View_dot_MemoryView_5array_6__len__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_array___pyx_pf_15View_dot_MemoryView_5array_8__getattr__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_attr); /* proto */
 static PyObject *__pyx_array___pyx_pf_15View_dot_MemoryView_5array_10__getitem__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_item); /* proto */
@@ -4654,29 +4657,97 @@
   __pyx_L3:;
 
   /* "unipolator/trotter_system.pyx":143
  *             self.l1 += self.d2
  *             V_expE_W_pointer(self.u1, self.l1, self.e1s, c[self.n_dims_2], self.v0, u0, self.d, self.d2)
  *         self.l1 = self.l0  # Restore original value of pointer             # <<<<<<<<<<<<<<
  *         self.e1s = self.e0s
- * 
+ *         for i in range(1, self.m_times, 2):
  */
   __pyx_t_6 = __pyx_v_self->l0;
   __pyx_v_self->l1 = __pyx_t_6;
 
   /* "unipolator/trotter_system.pyx":144
  *             V_expE_W_pointer(self.u1, self.l1, self.e1s, c[self.n_dims_2], self.v0, u0, self.d, self.d2)
  *         self.l1 = self.l0  # Restore original value of pointer
  *         self.e1s = self.e0s             # <<<<<<<<<<<<<<
- * 
- *     #def expmH(self, double[::1] c, double complex[:,::1] U):
+ *         for i in range(1, self.m_times, 2):
+ *             MM_cdot_pointer(u0, u0, self.u1, self.d)
  */
   __pyx_t_7 = __pyx_v_self->e0s;
   __pyx_v_self->e1s = __pyx_t_7;
 
+  /* "unipolator/trotter_system.pyx":145
+ *         self.l1 = self.l0  # Restore original value of pointer
+ *         self.e1s = self.e0s
+ *         for i in range(1, self.m_times, 2):             # <<<<<<<<<<<<<<
+ *             MM_cdot_pointer(u0, u0, self.u1, self.d)
+ *             MM_cdot_pointer(self.u1, self.u1, u0, self.d)
+ */
+  __pyx_t_2 = __pyx_v_self->m_times;
+  __pyx_t_3 = __pyx_t_2;
+  for (__pyx_t_4 = 1; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=2) {
+    __pyx_v_i = __pyx_t_4;
+
+    /* "unipolator/trotter_system.pyx":146
+ *         self.e1s = self.e0s
+ *         for i in range(1, self.m_times, 2):
+ *             MM_cdot_pointer(u0, u0, self.u1, self.d)             # <<<<<<<<<<<<<<
+ *             MM_cdot_pointer(self.u1, self.u1, u0, self.d)
+ *         if self.m_times % 2:
+ */
+    __pyx_f_10unipolator_14blas_functions_MM_cdot_pointer(__pyx_v_u0, __pyx_v_u0, __pyx_v_self->u1, __pyx_v_self->d);
+
+    /* "unipolator/trotter_system.pyx":147
+ *         for i in range(1, self.m_times, 2):
+ *             MM_cdot_pointer(u0, u0, self.u1, self.d)
+ *             MM_cdot_pointer(self.u1, self.u1, u0, self.d)             # <<<<<<<<<<<<<<
+ *         if self.m_times % 2:
+ *             MM_cdot_pointer(u0, u0, self.u1, self.d)
+ */
+    __pyx_f_10unipolator_14blas_functions_MM_cdot_pointer(__pyx_v_self->u1, __pyx_v_self->u1, __pyx_v_u0, __pyx_v_self->d);
+  }
+
+  /* "unipolator/trotter_system.pyx":148
+ *             MM_cdot_pointer(u0, u0, self.u1, self.d)
+ *             MM_cdot_pointer(self.u1, self.u1, u0, self.d)
+ *         if self.m_times % 2:             # <<<<<<<<<<<<<<
+ *             MM_cdot_pointer(u0, u0, self.u1, self.d)
+ *             copy_pointer(self.u1, u0, self.d2)
+ */
+  __pyx_t_1 = ((__pyx_v_self->m_times % 2) != 0);
+  if (__pyx_t_1) {
+
+    /* "unipolator/trotter_system.pyx":149
+ *             MM_cdot_pointer(self.u1, self.u1, u0, self.d)
+ *         if self.m_times % 2:
+ *             MM_cdot_pointer(u0, u0, self.u1, self.d)             # <<<<<<<<<<<<<<
+ *             copy_pointer(self.u1, u0, self.d2)
+ * 
+ */
+    __pyx_f_10unipolator_14blas_functions_MM_cdot_pointer(__pyx_v_u0, __pyx_v_u0, __pyx_v_self->u1, __pyx_v_self->d);
+
+    /* "unipolator/trotter_system.pyx":150
+ *         if self.m_times % 2:
+ *             MM_cdot_pointer(u0, u0, self.u1, self.d)
+ *             copy_pointer(self.u1, u0, self.d2)             # <<<<<<<<<<<<<<
+ * 
+ *     def expmH(self, double[::1] c, double complex[:,::1] U):
+ */
+    __pyx_f_10unipolator_11exp_and_log_copy_pointer(__pyx_v_self->u1, __pyx_v_u0, __pyx_v_self->d2);
+
+    /* "unipolator/trotter_system.pyx":148
+ *             MM_cdot_pointer(u0, u0, self.u1, self.d)
+ *             MM_cdot_pointer(self.u1, self.u1, u0, self.d)
+ *         if self.m_times % 2:             # <<<<<<<<<<<<<<
+ *             MM_cdot_pointer(u0, u0, self.u1, self.d)
+ *             copy_pointer(self.u1, u0, self.d2)
+ */
+  }
+
   /* "unipolator/trotter_system.pyx":121
  *         return np.array(self.L), np.array(self.Es)
  * 
  *     cdef expmH_pointer(self, double[::1] c, double complex *u0):             # <<<<<<<<<<<<<<
  *         cdef int i
  *         if self.n_dims_1 % 2 == 0:
  */
@@ -4684,16 +4755,16 @@
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unipolator/trotter_system.pyx":153
- *     #    self.expmH_pointer(c, u0)
+/* "unipolator/trotter_system.pyx":152
+ *             copy_pointer(self.u1, u0, self.d2)
  * 
  *     def expmH(self, double[::1] c, double complex[:,::1] U):             # <<<<<<<<<<<<<<
  *         # Construct Hamiltonian
  *         if not c.shape[0] == self.n_dims_1:
  */
 
 /* Python wrapper */
@@ -4727,227 +4798,398 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_c)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_U)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("expmH", 1, 2, 2, 1); __PYX_ERR(0, 153, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("expmH", 1, 2, 2, 1); __PYX_ERR(0, 152, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "expmH") < 0)) __PYX_ERR(0, 153, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "expmH") < 0)) __PYX_ERR(0, 152, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
-    __pyx_v_c = __Pyx_PyObject_to_MemoryviewSlice_dc_double(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_c.memview)) __PYX_ERR(0, 153, __pyx_L3_error)
-    __pyx_v_U = __Pyx_PyObject_to_MemoryviewSlice_d_dc___pyx_t_double_complex(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_U.memview)) __PYX_ERR(0, 153, __pyx_L3_error)
+    __pyx_v_c = __Pyx_PyObject_to_MemoryviewSlice_dc_double(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_c.memview)) __PYX_ERR(0, 152, __pyx_L3_error)
+    __pyx_v_U = __Pyx_PyObject_to_MemoryviewSlice_d_dc___pyx_t_double_complex(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_U.memview)) __PYX_ERR(0, 152, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("expmH", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 153, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("expmH", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 152, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("unipolator.trotter_system.Trotter_System.expmH", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_10unipolator_14trotter_system_14Trotter_System_4expmH(((struct __pyx_obj_10unipolator_14trotter_system_Trotter_System *)__pyx_v_self), __pyx_v_c, __pyx_v_U);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_10unipolator_14trotter_system_14Trotter_System_4expmH(struct __pyx_obj_10unipolator_14trotter_system_Trotter_System *__pyx_v_self, __Pyx_memviewslice __pyx_v_c, __Pyx_memviewslice __pyx_v_U) {
   __pyx_t_double_complex *__pyx_v_u0;
-  CYTHON_UNUSED long __pyx_v_i;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   Py_ssize_t __pyx_t_3;
   Py_ssize_t __pyx_t_4;
-  int __pyx_t_5;
-  int __pyx_t_6;
-  long __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("expmH", 0);
 
-  /* "unipolator/trotter_system.pyx":155
+  /* "unipolator/trotter_system.pyx":154
  *     def expmH(self, double[::1] c, double complex[:,::1] U):
  *         # Construct Hamiltonian
  *         if not c.shape[0] == self.n_dims_1:             # <<<<<<<<<<<<<<
  *             raise ValueError('c.shape[0] needs to be equal to H_s[0].shape[0]-1.')
  *         cdef double complex *u0 = &U[0,0]
  */
   __pyx_t_1 = ((!(((__pyx_v_c.shape[0]) == __pyx_v_self->n_dims_1) != 0)) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "unipolator/trotter_system.pyx":156
+    /* "unipolator/trotter_system.pyx":155
  *         # Construct Hamiltonian
  *         if not c.shape[0] == self.n_dims_1:
  *             raise ValueError('c.shape[0] needs to be equal to H_s[0].shape[0]-1.')             # <<<<<<<<<<<<<<
  *         cdef double complex *u0 = &U[0,0]
  *         self.expmH_pointer(c, u0)
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 156, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 155, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 156, __pyx_L1_error)
+    __PYX_ERR(0, 155, __pyx_L1_error)
 
-    /* "unipolator/trotter_system.pyx":155
+    /* "unipolator/trotter_system.pyx":154
  *     def expmH(self, double[::1] c, double complex[:,::1] U):
  *         # Construct Hamiltonian
  *         if not c.shape[0] == self.n_dims_1:             # <<<<<<<<<<<<<<
  *             raise ValueError('c.shape[0] needs to be equal to H_s[0].shape[0]-1.')
  *         cdef double complex *u0 = &U[0,0]
  */
   }
 
-  /* "unipolator/trotter_system.pyx":157
+  /* "unipolator/trotter_system.pyx":156
  *         if not c.shape[0] == self.n_dims_1:
  *             raise ValueError('c.shape[0] needs to be equal to H_s[0].shape[0]-1.')
  *         cdef double complex *u0 = &U[0,0]             # <<<<<<<<<<<<<<
  *         self.expmH_pointer(c, u0)
- *         for i in range(1, self.m_times, 2):
+ * 
  */
   __pyx_t_3 = 0;
   __pyx_t_4 = 0;
   __pyx_v_u0 = (&(*((__pyx_t_double_complex *) ( /* dim=1 */ ((char *) (((__pyx_t_double_complex *) ( /* dim=0 */ (__pyx_v_U.data + __pyx_t_3 * __pyx_v_U.strides[0]) )) + __pyx_t_4)) ))));
 
-  /* "unipolator/trotter_system.pyx":158
+  /* "unipolator/trotter_system.pyx":157
  *             raise ValueError('c.shape[0] needs to be equal to H_s[0].shape[0]-1.')
  *         cdef double complex *u0 = &U[0,0]
  *         self.expmH_pointer(c, u0)             # <<<<<<<<<<<<<<
- *         for i in range(1, self.m_times, 2):
- *             MM_cdot_pointer(u0, u0, self.u1, self.d)
+ * 
+ *     def expmH_pulse_no_multiply(self, double[:,::1] cs, double complex[:,:,::1] U):
  */
-  __pyx_t_2 = ((struct __pyx_vtabstruct_10unipolator_14trotter_system_Trotter_System *)__pyx_v_self->__pyx_vtab)->expmH_pointer(__pyx_v_self, __pyx_v_c, __pyx_v_u0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 158, __pyx_L1_error)
+  __pyx_t_2 = ((struct __pyx_vtabstruct_10unipolator_14trotter_system_Trotter_System *)__pyx_v_self->__pyx_vtab)->expmH_pointer(__pyx_v_self, __pyx_v_c, __pyx_v_u0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 157, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "unipolator/trotter_system.pyx":159
- *         cdef double complex *u0 = &U[0,0]
- *         self.expmH_pointer(c, u0)
- *         for i in range(1, self.m_times, 2):             # <<<<<<<<<<<<<<
- *             MM_cdot_pointer(u0, u0, self.u1, self.d)
- *             MM_cdot_pointer(self.u1, self.u1, u0, self.d)
+  /* "unipolator/trotter_system.pyx":152
+ *             copy_pointer(self.u1, u0, self.d2)
+ * 
+ *     def expmH(self, double[::1] c, double complex[:,::1] U):             # <<<<<<<<<<<<<<
+ *         # Construct Hamiltonian
+ *         if not c.shape[0] == self.n_dims_1:
  */
-  __pyx_t_5 = __pyx_v_self->m_times;
-  __pyx_t_6 = __pyx_t_5;
-  for (__pyx_t_7 = 1; __pyx_t_7 < __pyx_t_6; __pyx_t_7+=2) {
-    __pyx_v_i = __pyx_t_7;
 
-    /* "unipolator/trotter_system.pyx":160
+  /* function exit code */
+  __pyx_r = Py_None; __Pyx_INCREF(Py_None);
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_AddTraceback("unipolator.trotter_system.Trotter_System.expmH", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __PYX_XDEC_MEMVIEW(&__pyx_v_c, 1);
+  __PYX_XDEC_MEMVIEW(&__pyx_v_U, 1);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "unipolator/trotter_system.pyx":159
  *         self.expmH_pointer(c, u0)
- *         for i in range(1, self.m_times, 2):
- *             MM_cdot_pointer(u0, u0, self.u1, self.d)             # <<<<<<<<<<<<<<
- *             MM_cdot_pointer(self.u1, self.u1, u0, self.d)
- *         if self.m_times % 2:
+ * 
+ *     def expmH_pulse_no_multiply(self, double[:,::1] cs, double complex[:,:,::1] U):             # <<<<<<<<<<<<<<
+ *         cdef double complex *u0 = &U[0, 0, 0]
+ *         cdef how_many = cs.shape[0]
  */
-    __pyx_f_10unipolator_14blas_functions_MM_cdot_pointer(__pyx_v_u0, __pyx_v_u0, __pyx_v_self->u1, __pyx_v_self->d);
 
-    /* "unipolator/trotter_system.pyx":161
- *         for i in range(1, self.m_times, 2):
- *             MM_cdot_pointer(u0, u0, self.u1, self.d)
- *             MM_cdot_pointer(self.u1, self.u1, u0, self.d)             # <<<<<<<<<<<<<<
- *         if self.m_times % 2:
- *             MM_cdot_pointer(u0, u0, self.u1, self.d)
- */
-    __pyx_f_10unipolator_14blas_functions_MM_cdot_pointer(__pyx_v_self->u1, __pyx_v_self->u1, __pyx_v_u0, __pyx_v_self->d);
+/* Python wrapper */
+static PyObject *__pyx_pw_10unipolator_14trotter_system_14Trotter_System_7expmH_pulse_no_multiply(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_10unipolator_14trotter_system_14Trotter_System_6expmH_pulse_no_multiply[] = "Trotter_System.expmH_pulse_no_multiply(self, double[:, ::1] cs, double complex[:, :, ::1] U)";
+static PyObject *__pyx_pw_10unipolator_14trotter_system_14Trotter_System_7expmH_pulse_no_multiply(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+  __Pyx_memviewslice __pyx_v_cs = { 0, 0, { 0 }, { 0 }, { 0 } };
+  __Pyx_memviewslice __pyx_v_U = { 0, 0, { 0 }, { 0 }, { 0 } };
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("expmH_pulse_no_multiply (wrapper)", 0);
+  {
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_cs,&__pyx_n_s_U,0};
+    PyObject* values[2] = {0,0};
+    if (unlikely(__pyx_kwds)) {
+      Py_ssize_t kw_args;
+      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
+      switch (pos_args) {
+        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
+        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = PyDict_Size(__pyx_kwds);
+      switch (pos_args) {
+        case  0:
+        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_cs)) != 0)) kw_args--;
+        else goto __pyx_L5_argtuple_error;
+        CYTHON_FALLTHROUGH;
+        case  1:
+        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_U)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("expmH_pulse_no_multiply", 1, 2, 2, 1); __PYX_ERR(0, 159, __pyx_L3_error)
+        }
+      }
+      if (unlikely(kw_args > 0)) {
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "expmH_pulse_no_multiply") < 0)) __PYX_ERR(0, 159, __pyx_L3_error)
+      }
+    } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
+      goto __pyx_L5_argtuple_error;
+    } else {
+      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+      values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+    }
+    __pyx_v_cs = __Pyx_PyObject_to_MemoryviewSlice_d_dc_double(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_cs.memview)) __PYX_ERR(0, 159, __pyx_L3_error)
+    __pyx_v_U = __Pyx_PyObject_to_MemoryviewSlice_d_d_dc___pyx_t_double_complex(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_U.memview)) __PYX_ERR(0, 159, __pyx_L3_error)
   }
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("expmH_pulse_no_multiply", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 159, __pyx_L3_error)
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("unipolator.trotter_system.Trotter_System.expmH_pulse_no_multiply", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  __pyx_r = __pyx_pf_10unipolator_14trotter_system_14Trotter_System_6expmH_pulse_no_multiply(((struct __pyx_obj_10unipolator_14trotter_system_Trotter_System *)__pyx_v_self), __pyx_v_cs, __pyx_v_U);
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_10unipolator_14trotter_system_14Trotter_System_6expmH_pulse_no_multiply(struct __pyx_obj_10unipolator_14trotter_system_Trotter_System *__pyx_v_self, __Pyx_memviewslice __pyx_v_cs, __Pyx_memviewslice __pyx_v_U) {
+  __pyx_t_double_complex *__pyx_v_u0;
+  PyObject *__pyx_v_how_many = 0;
+  PyObject *__pyx_v_i = NULL;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  Py_ssize_t __pyx_t_1;
+  Py_ssize_t __pyx_t_2;
+  Py_ssize_t __pyx_t_3;
+  PyObject *__pyx_t_4 = NULL;
+  PyObject *__pyx_t_5 = NULL;
+  Py_ssize_t __pyx_t_6;
+  PyObject *(*__pyx_t_7)(PyObject *);
+  Py_ssize_t __pyx_t_8;
+  __Pyx_memviewslice __pyx_t_9 = { 0, 0, { 0 }, { 0 }, { 0 } };
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("expmH_pulse_no_multiply", 0);
+
+  /* "unipolator/trotter_system.pyx":160
+ * 
+ *     def expmH_pulse_no_multiply(self, double[:,::1] cs, double complex[:,:,::1] U):
+ *         cdef double complex *u0 = &U[0, 0, 0]             # <<<<<<<<<<<<<<
+ *         cdef how_many = cs.shape[0]
+ *         for i in range(how_many):
+ */
+  __pyx_t_1 = 0;
+  __pyx_t_2 = 0;
+  __pyx_t_3 = 0;
+  __pyx_v_u0 = (&(*((__pyx_t_double_complex *) ( /* dim=2 */ ((char *) (((__pyx_t_double_complex *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_U.data + __pyx_t_1 * __pyx_v_U.strides[0]) ) + __pyx_t_2 * __pyx_v_U.strides[1]) )) + __pyx_t_3)) ))));
+
+  /* "unipolator/trotter_system.pyx":161
+ *     def expmH_pulse_no_multiply(self, double[:,::1] cs, double complex[:,:,::1] U):
+ *         cdef double complex *u0 = &U[0, 0, 0]
+ *         cdef how_many = cs.shape[0]             # <<<<<<<<<<<<<<
+ *         for i in range(how_many):
+ *             self.expmH_pointer(cs[i,:], u0)
+ */
+  __pyx_t_4 = PyInt_FromSsize_t((__pyx_v_cs.shape[0])); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 161, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_v_how_many = __pyx_t_4;
+  __pyx_t_4 = 0;
 
   /* "unipolator/trotter_system.pyx":162
- *             MM_cdot_pointer(u0, u0, self.u1, self.d)
- *             MM_cdot_pointer(self.u1, self.u1, u0, self.d)
- *         if self.m_times % 2:             # <<<<<<<<<<<<<<
- *             MM_cdot_pointer(u0, u0, self.u1, self.d)
- *             copy_pointer(self.u1, u0, self.d2)
+ *         cdef double complex *u0 = &U[0, 0, 0]
+ *         cdef how_many = cs.shape[0]
+ *         for i in range(how_many):             # <<<<<<<<<<<<<<
+ *             self.expmH_pointer(cs[i,:], u0)
+ *             u0 += self.d2
  */
-  __pyx_t_1 = ((__pyx_v_self->m_times % 2) != 0);
-  if (__pyx_t_1) {
+  __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_range, __pyx_v_how_many); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 162, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  if (likely(PyList_CheckExact(__pyx_t_4)) || PyTuple_CheckExact(__pyx_t_4)) {
+    __pyx_t_5 = __pyx_t_4; __Pyx_INCREF(__pyx_t_5); __pyx_t_6 = 0;
+    __pyx_t_7 = NULL;
+  } else {
+    __pyx_t_6 = -1; __pyx_t_5 = PyObject_GetIter(__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 162, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_t_7 = Py_TYPE(__pyx_t_5)->tp_iternext; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 162, __pyx_L1_error)
+  }
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  for (;;) {
+    if (likely(!__pyx_t_7)) {
+      if (likely(PyList_CheckExact(__pyx_t_5))) {
+        if (__pyx_t_6 >= PyList_GET_SIZE(__pyx_t_5)) break;
+        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_5, __pyx_t_6); __Pyx_INCREF(__pyx_t_4); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 162, __pyx_L1_error)
+        #else
+        __pyx_t_4 = PySequence_ITEM(__pyx_t_5, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 162, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_4);
+        #endif
+      } else {
+        if (__pyx_t_6 >= PyTuple_GET_SIZE(__pyx_t_5)) break;
+        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_5, __pyx_t_6); __Pyx_INCREF(__pyx_t_4); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 162, __pyx_L1_error)
+        #else
+        __pyx_t_4 = PySequence_ITEM(__pyx_t_5, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 162, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_4);
+        #endif
+      }
+    } else {
+      __pyx_t_4 = __pyx_t_7(__pyx_t_5);
+      if (unlikely(!__pyx_t_4)) {
+        PyObject* exc_type = PyErr_Occurred();
+        if (exc_type) {
+          if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
+          else __PYX_ERR(0, 162, __pyx_L1_error)
+        }
+        break;
+      }
+      __Pyx_GOTREF(__pyx_t_4);
+    }
+    __Pyx_XDECREF_SET(__pyx_v_i, __pyx_t_4);
+    __pyx_t_4 = 0;
 
     /* "unipolator/trotter_system.pyx":163
- *             MM_cdot_pointer(self.u1, self.u1, u0, self.d)
- *         if self.m_times % 2:
- *             MM_cdot_pointer(u0, u0, self.u1, self.d)             # <<<<<<<<<<<<<<
- *             copy_pointer(self.u1, u0, self.d2)
- * 
+ *         cdef how_many = cs.shape[0]
+ *         for i in range(how_many):
+ *             self.expmH_pointer(cs[i,:], u0)             # <<<<<<<<<<<<<<
+ *             u0 += self.d2
+ *     """
  */
-    __pyx_f_10unipolator_14blas_functions_MM_cdot_pointer(__pyx_v_u0, __pyx_v_u0, __pyx_v_self->u1, __pyx_v_self->d);
+    __pyx_t_8 = __Pyx_PyIndex_AsSsize_t(__pyx_v_i); if (unlikely((__pyx_t_8 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 163, __pyx_L1_error)
+    __pyx_t_9.data = __pyx_v_cs.data;
+    __pyx_t_9.memview = __pyx_v_cs.memview;
+    __PYX_INC_MEMVIEW(&__pyx_t_9, 0);
+    {
+    Py_ssize_t __pyx_tmp_idx = __pyx_t_8;
+    Py_ssize_t __pyx_tmp_stride = __pyx_v_cs.strides[0];
+        __pyx_t_9.data += __pyx_tmp_idx * __pyx_tmp_stride;
+}
+
+__pyx_t_9.shape[0] = __pyx_v_cs.shape[1];
+__pyx_t_9.strides[0] = __pyx_v_cs.strides[1];
+    __pyx_t_9.suboffsets[0] = -1;
+
+__pyx_t_4 = ((struct __pyx_vtabstruct_10unipolator_14trotter_system_Trotter_System *)__pyx_v_self->__pyx_vtab)->expmH_pointer(__pyx_v_self, __pyx_t_9, __pyx_v_u0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 163, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __PYX_XDEC_MEMVIEW(&__pyx_t_9, 1);
+    __pyx_t_9.memview = NULL;
+    __pyx_t_9.data = NULL;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "unipolator/trotter_system.pyx":164
- *         if self.m_times % 2:
- *             MM_cdot_pointer(u0, u0, self.u1, self.d)
- *             copy_pointer(self.u1, u0, self.d2)             # <<<<<<<<<<<<<<
- * 
+ *         for i in range(how_many):
+ *             self.expmH_pointer(cs[i,:], u0)
+ *             u0 += self.d2             # <<<<<<<<<<<<<<
  *     """
+ *     def set_which_diffs(self, int[::1] which_diffs):
  */
-    __pyx_f_10unipolator_11exp_and_log_copy_pointer(__pyx_v_self->u1, __pyx_v_u0, __pyx_v_self->d2);
+    __pyx_v_u0 = (__pyx_v_u0 + __pyx_v_self->d2);
 
     /* "unipolator/trotter_system.pyx":162
- *             MM_cdot_pointer(u0, u0, self.u1, self.d)
- *             MM_cdot_pointer(self.u1, self.u1, u0, self.d)
- *         if self.m_times % 2:             # <<<<<<<<<<<<<<
- *             MM_cdot_pointer(u0, u0, self.u1, self.d)
- *             copy_pointer(self.u1, u0, self.d2)
+ *         cdef double complex *u0 = &U[0, 0, 0]
+ *         cdef how_many = cs.shape[0]
+ *         for i in range(how_many):             # <<<<<<<<<<<<<<
+ *             self.expmH_pointer(cs[i,:], u0)
+ *             u0 += self.d2
  */
   }
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "unipolator/trotter_system.pyx":153
- *     #    self.expmH_pointer(c, u0)
+  /* "unipolator/trotter_system.pyx":159
+ *         self.expmH_pointer(c, u0)
  * 
- *     def expmH(self, double[::1] c, double complex[:,::1] U):             # <<<<<<<<<<<<<<
- *         # Construct Hamiltonian
- *         if not c.shape[0] == self.n_dims_1:
+ *     def expmH_pulse_no_multiply(self, double[:,::1] cs, double complex[:,:,::1] U):             # <<<<<<<<<<<<<<
+ *         cdef double complex *u0 = &U[0, 0, 0]
+ *         cdef how_many = cs.shape[0]
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_AddTraceback("unipolator.trotter_system.Trotter_System.expmH", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_5);
+  __PYX_XDEC_MEMVIEW(&__pyx_t_9, 1);
+  __Pyx_AddTraceback("unipolator.trotter_system.Trotter_System.expmH_pulse_no_multiply", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
-  __PYX_XDEC_MEMVIEW(&__pyx_v_c, 1);
+  __Pyx_XDECREF(__pyx_v_how_many);
+  __Pyx_XDECREF(__pyx_v_i);
+  __PYX_XDEC_MEMVIEW(&__pyx_v_cs, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_v_U, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_10unipolator_14trotter_system_14Trotter_System_7__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static char __pyx_doc_10unipolator_14trotter_system_14Trotter_System_6__reduce_cython__[] = "Trotter_System.__reduce_cython__(self)";
-static PyObject *__pyx_pw_10unipolator_14trotter_system_14Trotter_System_7__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_10unipolator_14trotter_system_14Trotter_System_9__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc_10unipolator_14trotter_system_14Trotter_System_8__reduce_cython__[] = "Trotter_System.__reduce_cython__(self)";
+static PyObject *__pyx_pw_10unipolator_14trotter_system_14Trotter_System_9__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_10unipolator_14trotter_system_14Trotter_System_6__reduce_cython__(((struct __pyx_obj_10unipolator_14trotter_system_Trotter_System *)__pyx_v_self));
+  __pyx_r = __pyx_pf_10unipolator_14trotter_system_14Trotter_System_8__reduce_cython__(((struct __pyx_obj_10unipolator_14trotter_system_Trotter_System *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_10unipolator_14trotter_system_14Trotter_System_6__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_10unipolator_14trotter_system_Trotter_System *__pyx_v_self) {
+static PyObject *__pyx_pf_10unipolator_14trotter_system_14Trotter_System_8__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_10unipolator_14trotter_system_Trotter_System *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__reduce_cython__", 0);
@@ -4984,28 +5226,28 @@
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_10unipolator_14trotter_system_14Trotter_System_9__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
-static char __pyx_doc_10unipolator_14trotter_system_14Trotter_System_8__setstate_cython__[] = "Trotter_System.__setstate_cython__(self, __pyx_state)";
-static PyObject *__pyx_pw_10unipolator_14trotter_system_14Trotter_System_9__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pw_10unipolator_14trotter_system_14Trotter_System_11__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
+static char __pyx_doc_10unipolator_14trotter_system_14Trotter_System_10__setstate_cython__[] = "Trotter_System.__setstate_cython__(self, __pyx_state)";
+static PyObject *__pyx_pw_10unipolator_14trotter_system_14Trotter_System_11__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_10unipolator_14trotter_system_14Trotter_System_8__setstate_cython__(((struct __pyx_obj_10unipolator_14trotter_system_Trotter_System *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
+  __pyx_r = __pyx_pf_10unipolator_14trotter_system_14Trotter_System_10__setstate_cython__(((struct __pyx_obj_10unipolator_14trotter_system_Trotter_System *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_10unipolator_14trotter_system_14Trotter_System_8__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_10unipolator_14trotter_system_Trotter_System *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pf_10unipolator_14trotter_system_14Trotter_System_10__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_10unipolator_14trotter_system_Trotter_System *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
@@ -19169,16 +19411,17 @@
   __PYX_XDEC_MEMVIEW(&p->iwork, 1);
   (*Py_TYPE(o)->tp_free)(o);
 }
 
 static PyMethodDef __pyx_methods_10unipolator_14trotter_system_Trotter_System[] = {
   {"get_cache", (PyCFunction)__pyx_pw_10unipolator_14trotter_system_14Trotter_System_3get_cache, METH_NOARGS, __pyx_doc_10unipolator_14trotter_system_14Trotter_System_2get_cache},
   {"expmH", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_10unipolator_14trotter_system_14Trotter_System_5expmH, METH_VARARGS|METH_KEYWORDS, __pyx_doc_10unipolator_14trotter_system_14Trotter_System_4expmH},
-  {"__reduce_cython__", (PyCFunction)__pyx_pw_10unipolator_14trotter_system_14Trotter_System_7__reduce_cython__, METH_NOARGS, __pyx_doc_10unipolator_14trotter_system_14Trotter_System_6__reduce_cython__},
-  {"__setstate_cython__", (PyCFunction)__pyx_pw_10unipolator_14trotter_system_14Trotter_System_9__setstate_cython__, METH_O, __pyx_doc_10unipolator_14trotter_system_14Trotter_System_8__setstate_cython__},
+  {"expmH_pulse_no_multiply", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_10unipolator_14trotter_system_14Trotter_System_7expmH_pulse_no_multiply, METH_VARARGS|METH_KEYWORDS, __pyx_doc_10unipolator_14trotter_system_14Trotter_System_6expmH_pulse_no_multiply},
+  {"__reduce_cython__", (PyCFunction)__pyx_pw_10unipolator_14trotter_system_14Trotter_System_9__reduce_cython__, METH_NOARGS, __pyx_doc_10unipolator_14trotter_system_14Trotter_System_8__reduce_cython__},
+  {"__setstate_cython__", (PyCFunction)__pyx_pw_10unipolator_14trotter_system_14Trotter_System_11__setstate_cython__, METH_O, __pyx_doc_10unipolator_14trotter_system_14Trotter_System_10__setstate_cython__},
   {0, 0, 0, 0}
 };
 
 static PyTypeObject __pyx_type_10unipolator_14trotter_system_Trotter_System = {
   PyVarObject_HEAD_INIT(0, 0)
   "unipolator.trotter_system.Trotter_System", /*tp_name*/
   sizeof(struct __pyx_obj_10unipolator_14trotter_system_Trotter_System), /*tp_basicsize*/
@@ -20058,14 +20301,15 @@
   {&__pyx_n_u_c, __pyx_k_c, sizeof(__pyx_k_c), 0, 1, 0, 1},
   {&__pyx_kp_u_c_shape_0_needs_to_be_equal_to_H, __pyx_k_c_shape_0_needs_to_be_equal_to_H, sizeof(__pyx_k_c_shape_0_needs_to_be_equal_to_H), 0, 1, 0, 0},
   {&__pyx_n_s_class, __pyx_k_class, sizeof(__pyx_k_class), 0, 0, 1, 1},
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
   {&__pyx_n_s_complex128, __pyx_k_complex128, sizeof(__pyx_k_complex128), 0, 0, 1, 1},
   {&__pyx_kp_s_contiguous_and_direct, __pyx_k_contiguous_and_direct, sizeof(__pyx_k_contiguous_and_direct), 0, 0, 1, 0},
   {&__pyx_kp_s_contiguous_and_indirect, __pyx_k_contiguous_and_indirect, sizeof(__pyx_k_contiguous_and_indirect), 0, 0, 1, 0},
+  {&__pyx_n_s_cs, __pyx_k_cs, sizeof(__pyx_k_cs), 0, 0, 1, 1},
   {&__pyx_n_s_dict, __pyx_k_dict, sizeof(__pyx_k_dict), 0, 0, 1, 1},
   {&__pyx_n_s_double, __pyx_k_double, sizeof(__pyx_k_double), 0, 0, 1, 1},
   {&__pyx_n_s_dtype, __pyx_k_dtype, sizeof(__pyx_k_dtype), 0, 0, 1, 1},
   {&__pyx_n_s_dtype_is_object, __pyx_k_dtype_is_object, sizeof(__pyx_k_dtype_is_object), 0, 0, 1, 1},
   {&__pyx_n_s_empty, __pyx_k_empty, sizeof(__pyx_k_empty), 0, 0, 1, 1},
   {&__pyx_n_s_encode, __pyx_k_encode, sizeof(__pyx_k_encode), 0, 0, 1, 1},
   {&__pyx_n_s_enumerate, __pyx_k_enumerate, sizeof(__pyx_k_enumerate), 0, 0, 1, 1},
@@ -20127,15 +20371,15 @@
   {&__pyx_n_s_unpack, __pyx_k_unpack, sizeof(__pyx_k_unpack), 0, 0, 1, 1},
   {&__pyx_n_s_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 0, 1, 1},
   {&__pyx_n_s_which_diffs, __pyx_k_which_diffs, sizeof(__pyx_k_which_diffs), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 106, __pyx_L1_error)
-  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 156, __pyx_L1_error)
+  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 155, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(1, 2, __pyx_L1_error)
   __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(2, 945, __pyx_L1_error)
   __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(1, 149, __pyx_L1_error)
   __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(1, 152, __pyx_L1_error)
   __pyx_builtin_Ellipsis = __Pyx_GetBuiltinName(__pyx_n_s_Ellipsis); if (!__pyx_builtin_Ellipsis) __PYX_ERR(1, 406, __pyx_L1_error)
   __pyx_builtin_id = __Pyx_GetBuiltinName(__pyx_n_s_id); if (!__pyx_builtin_id) __PYX_ERR(1, 615, __pyx_L1_error)
   __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(1, 834, __pyx_L1_error)
@@ -20144,22 +20388,22 @@
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "unipolator/trotter_system.pyx":156
+  /* "unipolator/trotter_system.pyx":155
  *         # Construct Hamiltonian
  *         if not c.shape[0] == self.n_dims_1:
  *             raise ValueError('c.shape[0] needs to be equal to H_s[0].shape[0]-1.')             # <<<<<<<<<<<<<<
  *         cdef double complex *u0 = &U[0,0]
  *         self.expmH_pointer(c, u0)
  */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_c_shape_0_needs_to_be_equal_to_H); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 156, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_c_shape_0_needs_to_be_equal_to_H); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 155, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
@@ -24420,14 +24664,37 @@
     return result;
 __pyx_fail:
     result.memview = NULL;
     result.data = NULL;
     return result;
 }
 
+/* ObjectToMemviewSlice */
+  static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_d_dc_double(PyObject *obj, int writable_flag) {
+    __Pyx_memviewslice result = { 0, 0, { 0 }, { 0 }, { 0 } };
+    __Pyx_BufFmt_StackElem stack[1];
+    int axes_specs[] = { (__Pyx_MEMVIEW_DIRECT | __Pyx_MEMVIEW_FOLLOW), (__Pyx_MEMVIEW_DIRECT | __Pyx_MEMVIEW_CONTIG) };
+    int retcode;
+    if (obj == Py_None) {
+        result.memview = (struct __pyx_memoryview_obj *) Py_None;
+        return result;
+    }
+    retcode = __Pyx_ValidateAndInit_memviewslice(axes_specs, __Pyx_IS_C_CONTIG,
+                                                 (PyBUF_C_CONTIGUOUS | PyBUF_FORMAT) | writable_flag, 2,
+                                                 &__Pyx_TypeInfo_double, stack,
+                                                 &result, obj);
+    if (unlikely(retcode == -1))
+        goto __pyx_fail;
+    return result;
+__pyx_fail:
+    result.memview = NULL;
+    result.data = NULL;
+    return result;
+}
+
 /* IntPow */
   static CYTHON_INLINE long __Pyx_pow_long(long b, long e) {
     long t = b;
     switch (e) {
         case 3:
             t *= b;
         CYTHON_FALLTHROUGH;
@@ -24467,37 +24734,14 @@
                                                  &result, obj);
     if (unlikely(retcode == -1))
         goto __pyx_fail;
     return result;
 __pyx_fail:
     result.memview = NULL;
     result.data = NULL;
-    return result;
-}
-
-/* ObjectToMemviewSlice */
-  static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_d_dc_double(PyObject *obj, int writable_flag) {
-    __Pyx_memviewslice result = { 0, 0, { 0 }, { 0 }, { 0 } };
-    __Pyx_BufFmt_StackElem stack[1];
-    int axes_specs[] = { (__Pyx_MEMVIEW_DIRECT | __Pyx_MEMVIEW_FOLLOW), (__Pyx_MEMVIEW_DIRECT | __Pyx_MEMVIEW_CONTIG) };
-    int retcode;
-    if (obj == Py_None) {
-        result.memview = (struct __pyx_memoryview_obj *) Py_None;
-        return result;
-    }
-    retcode = __Pyx_ValidateAndInit_memviewslice(axes_specs, __Pyx_IS_C_CONTIG,
-                                                 (PyBUF_C_CONTIGUOUS | PyBUF_FORMAT) | writable_flag, 2,
-                                                 &__Pyx_TypeInfo_double, stack,
-                                                 &result, obj);
-    if (unlikely(retcode == -1))
-        goto __pyx_fail;
-    return result;
-__pyx_fail:
-    result.memview = NULL;
-    result.data = NULL;
     return result;
 }
 
 /* ObjectToMemviewSlice */
   static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_dc_int(PyObject *obj, int writable_flag) {
     __Pyx_memviewslice result = { 0, 0, { 0 }, { 0 }, { 0 } };
     __Pyx_BufFmt_StackElem stack[1];
```

### Comparing `unipolator-0.2.6/src/unipolator/trotter_system.pyx` & `unipolator-0.2.7/src/unipolator/trotter_system.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -138,35 +138,34 @@
                 self.l1 += self.d2
                 V_expE_W_pointer(u0, self.l1, self.e1s, c[i+1], self.v0, self.u1, self.d, self.d2)
                 self.e1s += self.d
             self.l1 += self.d2
             V_expE_W_pointer(self.u1, self.l1, self.e1s, c[self.n_dims_2], self.v0, u0, self.d, self.d2)
         self.l1 = self.l0  # Restore original value of pointer
         self.e1s = self.e0s
-
-    #def expmH(self, double[::1] c, double complex[:,::1] U):
-    #    # Construct Hamiltonian
-    #    if not c.shape[0] == self.n_dims_1:
-    #        raise ValueError('c.shape[0] needs to be equal to H_s[0].shape[0]-1.')
-    #    cdef double complex *u0 = &U[0,0]
-    #    self.expmH_pointer(c, u0)
+        for i in range(1, self.m_times, 2):
+            MM_cdot_pointer(u0, u0, self.u1, self.d)
+            MM_cdot_pointer(self.u1, self.u1, u0, self.d)
+        if self.m_times % 2:
+            MM_cdot_pointer(u0, u0, self.u1, self.d)
+            copy_pointer(self.u1, u0, self.d2)
 
     def expmH(self, double[::1] c, double complex[:,::1] U):
         # Construct Hamiltonian
         if not c.shape[0] == self.n_dims_1:
             raise ValueError('c.shape[0] needs to be equal to H_s[0].shape[0]-1.')
         cdef double complex *u0 = &U[0,0]
         self.expmH_pointer(c, u0)
-        for i in range(1, self.m_times, 2):
-            MM_cdot_pointer(u0, u0, self.u1, self.d)
-            MM_cdot_pointer(self.u1, self.u1, u0, self.d)
-        if self.m_times % 2:
-            MM_cdot_pointer(u0, u0, self.u1, self.d)
-            copy_pointer(self.u1, u0, self.d2)
             
+    def expmH_pulse_no_multiply(self, double[:,::1] cs, double complex[:,:,::1] U):
+        cdef double complex *u0 = &U[0, 0, 0]
+        cdef how_many = cs.shape[0]
+        for i in range(how_many):
+            self.expmH_pointer(cs[i,:], u0)
+            u0 += self.d2
     """
     def set_which_diffs(self, int[::1] which_diffs):
         self.d_di = which_diffs
         self.n_d_di = self.d_di.shape[0]
 
     def get_which_diffs(self):
         return np.asarray(self.d_di), self.n_d_di
```

### Comparing `unipolator-0.2.6/src/unipolator/unitary_interpolation.c` & `unipolator-0.2.7/src/unipolator/unitary_interpolation.c`

 * *Files 0% similar despite different names*

```diff
@@ -2755,17 +2755,18 @@
 static int __pyx_pf_10unipolator_21unitary_interpolation_2UI___cinit__(struct __pyx_obj_10unipolator_21unitary_interpolation_UI *__pyx_v_self, __Pyx_memviewslice __pyx_v_H_s, __Pyx_memviewslice __pyx_v_c_min_s, __Pyx_memviewslice __pyx_v_c_max_s, __Pyx_memviewslice __pyx_v_c_bins, __Pyx_memviewslice __pyx_v_which_diffs); /* proto */
 static PyObject *__pyx_pf_10unipolator_21unitary_interpolation_2UI_2set_which_diffs(struct __pyx_obj_10unipolator_21unitary_interpolation_UI *__pyx_v_self, __Pyx_memviewslice __pyx_v_which_diffs); /* proto */
 static PyObject *__pyx_pf_10unipolator_21unitary_interpolation_2UI_4get_single_param(struct __pyx_obj_10unipolator_21unitary_interpolation_UI *__pyx_v_self, __Pyx_memviewslice __pyx_v_c); /* proto */
 static PyObject *__pyx_pf_10unipolator_21unitary_interpolation_2UI_6get_cache(struct __pyx_obj_10unipolator_21unitary_interpolation_UI *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_10unipolator_21unitary_interpolation_2UI_8expmH(struct __pyx_obj_10unipolator_21unitary_interpolation_UI *__pyx_v_self, __Pyx_memviewslice __pyx_v_c, __Pyx_memviewslice __pyx_v_U); /* proto */
 static PyObject *__pyx_pf_10unipolator_21unitary_interpolation_2UI_10dexpmH(struct __pyx_obj_10unipolator_21unitary_interpolation_UI *__pyx_v_self, __Pyx_memviewslice __pyx_v_c, __Pyx_memviewslice __pyx_v_U, __Pyx_memviewslice __pyx_v_dU); /* proto */
 static PyObject *__pyx_pf_10unipolator_21unitary_interpolation_2UI_12expmH_pulse(struct __pyx_obj_10unipolator_21unitary_interpolation_UI *__pyx_v_self, __Pyx_memviewslice __pyx_v_cs, __Pyx_memviewslice __pyx_v_U); /* proto */
-static PyObject *__pyx_pf_10unipolator_21unitary_interpolation_2UI_14grape(struct __pyx_obj_10unipolator_21unitary_interpolation_UI *__pyx_v_self, __Pyx_memviewslice __pyx_v_cs, __Pyx_memviewslice __pyx_v_U_target, __Pyx_memviewslice __pyx_v_target_indexes, __Pyx_memviewslice __pyx_v_U, __Pyx_memviewslice __pyx_v_dU, __Pyx_memviewslice __pyx_v_dI_dj); /* proto */
-static PyObject *__pyx_pf_10unipolator_21unitary_interpolation_2UI_16__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_10unipolator_21unitary_interpolation_UI *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_10unipolator_21unitary_interpolation_2UI_18__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_10unipolator_21unitary_interpolation_UI *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
+static PyObject *__pyx_pf_10unipolator_21unitary_interpolation_2UI_14expmH_pulse_no_multiply(struct __pyx_obj_10unipolator_21unitary_interpolation_UI *__pyx_v_self, __Pyx_memviewslice __pyx_v_cs, __Pyx_memviewslice __pyx_v_U); /* proto */
+static PyObject *__pyx_pf_10unipolator_21unitary_interpolation_2UI_16grape(struct __pyx_obj_10unipolator_21unitary_interpolation_UI *__pyx_v_self, __Pyx_memviewslice __pyx_v_cs, __Pyx_memviewslice __pyx_v_U_target, __Pyx_memviewslice __pyx_v_target_indexes, __Pyx_memviewslice __pyx_v_U, __Pyx_memviewslice __pyx_v_dU, __Pyx_memviewslice __pyx_v_dI_dj); /* proto */
+static PyObject *__pyx_pf_10unipolator_21unitary_interpolation_2UI_18__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_10unipolator_21unitary_interpolation_UI *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_10unipolator_21unitary_interpolation_2UI_20__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_10unipolator_21unitary_interpolation_UI *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
 static int __pyx_array___pyx_pf_15View_dot_MemoryView_5array___cinit__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_shape, Py_ssize_t __pyx_v_itemsize, PyObject *__pyx_v_format, PyObject *__pyx_v_mode, int __pyx_v_allocate_buffer); /* proto */
 static int __pyx_array___pyx_pf_15View_dot_MemoryView_5array_2__getbuffer__(struct __pyx_array_obj *__pyx_v_self, Py_buffer *__pyx_v_info, int __pyx_v_flags); /* proto */
 static void __pyx_array___pyx_pf_15View_dot_MemoryView_5array_4__dealloc__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_15View_dot_MemoryView_5array_7memview___get__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static Py_ssize_t __pyx_array___pyx_pf_15View_dot_MemoryView_5array_6__len__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_array___pyx_pf_15View_dot_MemoryView_5array_8__getattr__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_attr); /* proto */
 static PyObject *__pyx_array___pyx_pf_15View_dot_MemoryView_5array_10__getitem__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_item); /* proto */
@@ -7847,15 +7848,15 @@
   __pyx_v_u0 = (&(*((__pyx_t_double_complex *) ( /* dim=1 */ ((char *) (((__pyx_t_double_complex *) ( /* dim=0 */ (__pyx_v_U.data + __pyx_t_1 * __pyx_v_U.strides[0]) )) + __pyx_t_2)) ))));
 
   /* "unipolator/unitary_interpolation.pyx":341
  *     def expmH_pulse(self, double[:,::1] cs, double complex[:,::1] U):
  *         cdef double complex *u0 = &U[0, 0]
  *         self.expmH_pulse_pointer(cs, u0)             # <<<<<<<<<<<<<<
  * 
- *     def grape(self, double[:,::1] cs, double complex[:,::1] U_target, int[::1] target_indexes, double complex[:,::1] U, double complex[:,:,::1] dU, double[:,::1] dI_dj):
+ *     def expmH_pulse_no_multiply(self, double[:,::1] cs, double complex[:,:,::1] U):
  */
   __pyx_t_3 = ((struct __pyx_vtabstruct_10unipolator_21unitary_interpolation_UI *)__pyx_v_self->__pyx_vtab)->expmH_pulse_pointer(__pyx_v_self, __pyx_v_cs, __pyx_v_u0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 341, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "unipolator/unitary_interpolation.pyx":339
  *             self.interpolate_single_u(ur2)
@@ -7879,23 +7880,266 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "unipolator/unitary_interpolation.pyx":343
  *         self.expmH_pulse_pointer(cs, u0)
  * 
+ *     def expmH_pulse_no_multiply(self, double[:,::1] cs, double complex[:,:,::1] U):             # <<<<<<<<<<<<<<
+ *         cdef double complex *u0 = &U[0, 0, 0]
+ *         cdef how_many = cs.shape[0]
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_10unipolator_21unitary_interpolation_2UI_15expmH_pulse_no_multiply(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_10unipolator_21unitary_interpolation_2UI_14expmH_pulse_no_multiply[] = "UI.expmH_pulse_no_multiply(self, double[:, ::1] cs, double complex[:, :, ::1] U)";
+static PyObject *__pyx_pw_10unipolator_21unitary_interpolation_2UI_15expmH_pulse_no_multiply(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+  __Pyx_memviewslice __pyx_v_cs = { 0, 0, { 0 }, { 0 }, { 0 } };
+  __Pyx_memviewslice __pyx_v_U = { 0, 0, { 0 }, { 0 }, { 0 } };
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("expmH_pulse_no_multiply (wrapper)", 0);
+  {
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_cs,&__pyx_n_s_U,0};
+    PyObject* values[2] = {0,0};
+    if (unlikely(__pyx_kwds)) {
+      Py_ssize_t kw_args;
+      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
+      switch (pos_args) {
+        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
+        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = PyDict_Size(__pyx_kwds);
+      switch (pos_args) {
+        case  0:
+        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_cs)) != 0)) kw_args--;
+        else goto __pyx_L5_argtuple_error;
+        CYTHON_FALLTHROUGH;
+        case  1:
+        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_U)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("expmH_pulse_no_multiply", 1, 2, 2, 1); __PYX_ERR(0, 343, __pyx_L3_error)
+        }
+      }
+      if (unlikely(kw_args > 0)) {
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "expmH_pulse_no_multiply") < 0)) __PYX_ERR(0, 343, __pyx_L3_error)
+      }
+    } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
+      goto __pyx_L5_argtuple_error;
+    } else {
+      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+      values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+    }
+    __pyx_v_cs = __Pyx_PyObject_to_MemoryviewSlice_d_dc_double(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_cs.memview)) __PYX_ERR(0, 343, __pyx_L3_error)
+    __pyx_v_U = __Pyx_PyObject_to_MemoryviewSlice_d_d_dc___pyx_t_double_complex(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_U.memview)) __PYX_ERR(0, 343, __pyx_L3_error)
+  }
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("expmH_pulse_no_multiply", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 343, __pyx_L3_error)
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("unipolator.unitary_interpolation.UI.expmH_pulse_no_multiply", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  __pyx_r = __pyx_pf_10unipolator_21unitary_interpolation_2UI_14expmH_pulse_no_multiply(((struct __pyx_obj_10unipolator_21unitary_interpolation_UI *)__pyx_v_self), __pyx_v_cs, __pyx_v_U);
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_10unipolator_21unitary_interpolation_2UI_14expmH_pulse_no_multiply(struct __pyx_obj_10unipolator_21unitary_interpolation_UI *__pyx_v_self, __Pyx_memviewslice __pyx_v_cs, __Pyx_memviewslice __pyx_v_U) {
+  __pyx_t_double_complex *__pyx_v_u0;
+  PyObject *__pyx_v_how_many = 0;
+  PyObject *__pyx_v_i = NULL;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  Py_ssize_t __pyx_t_1;
+  Py_ssize_t __pyx_t_2;
+  Py_ssize_t __pyx_t_3;
+  PyObject *__pyx_t_4 = NULL;
+  PyObject *__pyx_t_5 = NULL;
+  Py_ssize_t __pyx_t_6;
+  PyObject *(*__pyx_t_7)(PyObject *);
+  Py_ssize_t __pyx_t_8;
+  __Pyx_memviewslice __pyx_t_9 = { 0, 0, { 0 }, { 0 }, { 0 } };
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("expmH_pulse_no_multiply", 0);
+
+  /* "unipolator/unitary_interpolation.pyx":344
+ * 
+ *     def expmH_pulse_no_multiply(self, double[:,::1] cs, double complex[:,:,::1] U):
+ *         cdef double complex *u0 = &U[0, 0, 0]             # <<<<<<<<<<<<<<
+ *         cdef how_many = cs.shape[0]
+ *         for i in range(how_many):
+ */
+  __pyx_t_1 = 0;
+  __pyx_t_2 = 0;
+  __pyx_t_3 = 0;
+  __pyx_v_u0 = (&(*((__pyx_t_double_complex *) ( /* dim=2 */ ((char *) (((__pyx_t_double_complex *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_U.data + __pyx_t_1 * __pyx_v_U.strides[0]) ) + __pyx_t_2 * __pyx_v_U.strides[1]) )) + __pyx_t_3)) ))));
+
+  /* "unipolator/unitary_interpolation.pyx":345
+ *     def expmH_pulse_no_multiply(self, double[:,::1] cs, double complex[:,:,::1] U):
+ *         cdef double complex *u0 = &U[0, 0, 0]
+ *         cdef how_many = cs.shape[0]             # <<<<<<<<<<<<<<
+ *         for i in range(how_many):
+ *             self.expmH_pointer(cs[i,:], u0)
+ */
+  __pyx_t_4 = PyInt_FromSsize_t((__pyx_v_cs.shape[0])); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 345, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_v_how_many = __pyx_t_4;
+  __pyx_t_4 = 0;
+
+  /* "unipolator/unitary_interpolation.pyx":346
+ *         cdef double complex *u0 = &U[0, 0, 0]
+ *         cdef how_many = cs.shape[0]
+ *         for i in range(how_many):             # <<<<<<<<<<<<<<
+ *             self.expmH_pointer(cs[i,:], u0)
+ *             u0 += self.d2
+ */
+  __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_range, __pyx_v_how_many); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 346, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  if (likely(PyList_CheckExact(__pyx_t_4)) || PyTuple_CheckExact(__pyx_t_4)) {
+    __pyx_t_5 = __pyx_t_4; __Pyx_INCREF(__pyx_t_5); __pyx_t_6 = 0;
+    __pyx_t_7 = NULL;
+  } else {
+    __pyx_t_6 = -1; __pyx_t_5 = PyObject_GetIter(__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 346, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_t_7 = Py_TYPE(__pyx_t_5)->tp_iternext; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 346, __pyx_L1_error)
+  }
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  for (;;) {
+    if (likely(!__pyx_t_7)) {
+      if (likely(PyList_CheckExact(__pyx_t_5))) {
+        if (__pyx_t_6 >= PyList_GET_SIZE(__pyx_t_5)) break;
+        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_5, __pyx_t_6); __Pyx_INCREF(__pyx_t_4); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 346, __pyx_L1_error)
+        #else
+        __pyx_t_4 = PySequence_ITEM(__pyx_t_5, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 346, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_4);
+        #endif
+      } else {
+        if (__pyx_t_6 >= PyTuple_GET_SIZE(__pyx_t_5)) break;
+        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_5, __pyx_t_6); __Pyx_INCREF(__pyx_t_4); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 346, __pyx_L1_error)
+        #else
+        __pyx_t_4 = PySequence_ITEM(__pyx_t_5, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 346, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_4);
+        #endif
+      }
+    } else {
+      __pyx_t_4 = __pyx_t_7(__pyx_t_5);
+      if (unlikely(!__pyx_t_4)) {
+        PyObject* exc_type = PyErr_Occurred();
+        if (exc_type) {
+          if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
+          else __PYX_ERR(0, 346, __pyx_L1_error)
+        }
+        break;
+      }
+      __Pyx_GOTREF(__pyx_t_4);
+    }
+    __Pyx_XDECREF_SET(__pyx_v_i, __pyx_t_4);
+    __pyx_t_4 = 0;
+
+    /* "unipolator/unitary_interpolation.pyx":347
+ *         cdef how_many = cs.shape[0]
+ *         for i in range(how_many):
+ *             self.expmH_pointer(cs[i,:], u0)             # <<<<<<<<<<<<<<
+ *             u0 += self.d2
+ * 
+ */
+    __pyx_t_8 = __Pyx_PyIndex_AsSsize_t(__pyx_v_i); if (unlikely((__pyx_t_8 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 347, __pyx_L1_error)
+    __pyx_t_9.data = __pyx_v_cs.data;
+    __pyx_t_9.memview = __pyx_v_cs.memview;
+    __PYX_INC_MEMVIEW(&__pyx_t_9, 0);
+    {
+    Py_ssize_t __pyx_tmp_idx = __pyx_t_8;
+    Py_ssize_t __pyx_tmp_stride = __pyx_v_cs.strides[0];
+        __pyx_t_9.data += __pyx_tmp_idx * __pyx_tmp_stride;
+}
+
+__pyx_t_9.shape[0] = __pyx_v_cs.shape[1];
+__pyx_t_9.strides[0] = __pyx_v_cs.strides[1];
+    __pyx_t_9.suboffsets[0] = -1;
+
+__pyx_t_4 = ((struct __pyx_vtabstruct_10unipolator_21unitary_interpolation_UI *)__pyx_v_self->__pyx_vtab)->expmH_pointer(__pyx_v_self, __pyx_t_9, __pyx_v_u0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 347, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __PYX_XDEC_MEMVIEW(&__pyx_t_9, 1);
+    __pyx_t_9.memview = NULL;
+    __pyx_t_9.data = NULL;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+
+    /* "unipolator/unitary_interpolation.pyx":348
+ *         for i in range(how_many):
+ *             self.expmH_pointer(cs[i,:], u0)
+ *             u0 += self.d2             # <<<<<<<<<<<<<<
+ * 
+ *     def grape(self, double[:,::1] cs, double complex[:,::1] U_target, int[::1] target_indexes, double complex[:,::1] U, double complex[:,:,::1] dU, double[:,::1] dI_dj):
+ */
+    __pyx_v_u0 = (__pyx_v_u0 + __pyx_v_self->d2);
+
+    /* "unipolator/unitary_interpolation.pyx":346
+ *         cdef double complex *u0 = &U[0, 0, 0]
+ *         cdef how_many = cs.shape[0]
+ *         for i in range(how_many):             # <<<<<<<<<<<<<<
+ *             self.expmH_pointer(cs[i,:], u0)
+ *             u0 += self.d2
+ */
+  }
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+
+  /* "unipolator/unitary_interpolation.pyx":343
+ *         self.expmH_pulse_pointer(cs, u0)
+ * 
+ *     def expmH_pulse_no_multiply(self, double[:,::1] cs, double complex[:,:,::1] U):             # <<<<<<<<<<<<<<
+ *         cdef double complex *u0 = &U[0, 0, 0]
+ *         cdef how_many = cs.shape[0]
+ */
+
+  /* function exit code */
+  __pyx_r = Py_None; __Pyx_INCREF(Py_None);
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_5);
+  __PYX_XDEC_MEMVIEW(&__pyx_t_9, 1);
+  __Pyx_AddTraceback("unipolator.unitary_interpolation.UI.expmH_pulse_no_multiply", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_how_many);
+  __Pyx_XDECREF(__pyx_v_i);
+  __PYX_XDEC_MEMVIEW(&__pyx_v_cs, 1);
+  __PYX_XDEC_MEMVIEW(&__pyx_v_U, 1);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "unipolator/unitary_interpolation.pyx":350
+ *             u0 += self.d2
+ * 
  *     def grape(self, double[:,::1] cs, double complex[:,::1] U_target, int[::1] target_indexes, double complex[:,::1] U, double complex[:,:,::1] dU, double[:,::1] dI_dj):             # <<<<<<<<<<<<<<
  *         # Calculate fidelity for a pulse and the differentials of the fidelity at every timestep using the grape trick
  *         cdef int i, j
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_10unipolator_21unitary_interpolation_2UI_15grape(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_10unipolator_21unitary_interpolation_2UI_14grape[] = "UI.grape(self, double[:, ::1] cs, double complex[:, ::1] U_target, int[::1] target_indexes, double complex[:, ::1] U, double complex[:, :, ::1] dU, double[:, ::1] dI_dj)";
-static PyObject *__pyx_pw_10unipolator_21unitary_interpolation_2UI_15grape(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_10unipolator_21unitary_interpolation_2UI_17grape(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_10unipolator_21unitary_interpolation_2UI_16grape[] = "UI.grape(self, double[:, ::1] cs, double complex[:, ::1] U_target, int[::1] target_indexes, double complex[:, ::1] U, double complex[:, :, ::1] dU, double[:, ::1] dI_dj)";
+static PyObject *__pyx_pw_10unipolator_21unitary_interpolation_2UI_17grape(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   __Pyx_memviewslice __pyx_v_cs = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_U_target = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_target_indexes = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_U = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_dU = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_dI_dj = { 0, 0, { 0 }, { 0 }, { 0 } };
   int __pyx_lineno = 0;
@@ -7931,77 +8175,77 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_cs)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_U_target)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("grape", 1, 6, 6, 1); __PYX_ERR(0, 343, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("grape", 1, 6, 6, 1); __PYX_ERR(0, 350, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_target_indexes)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("grape", 1, 6, 6, 2); __PYX_ERR(0, 343, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("grape", 1, 6, 6, 2); __PYX_ERR(0, 350, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_U)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("grape", 1, 6, 6, 3); __PYX_ERR(0, 343, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("grape", 1, 6, 6, 3); __PYX_ERR(0, 350, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (likely((values[4] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_dU)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("grape", 1, 6, 6, 4); __PYX_ERR(0, 343, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("grape", 1, 6, 6, 4); __PYX_ERR(0, 350, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  5:
         if (likely((values[5] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_dI_dj)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("grape", 1, 6, 6, 5); __PYX_ERR(0, 343, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("grape", 1, 6, 6, 5); __PYX_ERR(0, 350, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "grape") < 0)) __PYX_ERR(0, 343, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "grape") < 0)) __PYX_ERR(0, 350, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 6) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
       values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
       values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
       values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
     }
-    __pyx_v_cs = __Pyx_PyObject_to_MemoryviewSlice_d_dc_double(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_cs.memview)) __PYX_ERR(0, 343, __pyx_L3_error)
-    __pyx_v_U_target = __Pyx_PyObject_to_MemoryviewSlice_d_dc___pyx_t_double_complex(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_U_target.memview)) __PYX_ERR(0, 343, __pyx_L3_error)
-    __pyx_v_target_indexes = __Pyx_PyObject_to_MemoryviewSlice_dc_int(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_target_indexes.memview)) __PYX_ERR(0, 343, __pyx_L3_error)
-    __pyx_v_U = __Pyx_PyObject_to_MemoryviewSlice_d_dc___pyx_t_double_complex(values[3], PyBUF_WRITABLE); if (unlikely(!__pyx_v_U.memview)) __PYX_ERR(0, 343, __pyx_L3_error)
-    __pyx_v_dU = __Pyx_PyObject_to_MemoryviewSlice_d_d_dc___pyx_t_double_complex(values[4], PyBUF_WRITABLE); if (unlikely(!__pyx_v_dU.memview)) __PYX_ERR(0, 343, __pyx_L3_error)
-    __pyx_v_dI_dj = __Pyx_PyObject_to_MemoryviewSlice_d_dc_double(values[5], PyBUF_WRITABLE); if (unlikely(!__pyx_v_dI_dj.memview)) __PYX_ERR(0, 343, __pyx_L3_error)
+    __pyx_v_cs = __Pyx_PyObject_to_MemoryviewSlice_d_dc_double(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_cs.memview)) __PYX_ERR(0, 350, __pyx_L3_error)
+    __pyx_v_U_target = __Pyx_PyObject_to_MemoryviewSlice_d_dc___pyx_t_double_complex(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_U_target.memview)) __PYX_ERR(0, 350, __pyx_L3_error)
+    __pyx_v_target_indexes = __Pyx_PyObject_to_MemoryviewSlice_dc_int(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_target_indexes.memview)) __PYX_ERR(0, 350, __pyx_L3_error)
+    __pyx_v_U = __Pyx_PyObject_to_MemoryviewSlice_d_dc___pyx_t_double_complex(values[3], PyBUF_WRITABLE); if (unlikely(!__pyx_v_U.memview)) __PYX_ERR(0, 350, __pyx_L3_error)
+    __pyx_v_dU = __Pyx_PyObject_to_MemoryviewSlice_d_d_dc___pyx_t_double_complex(values[4], PyBUF_WRITABLE); if (unlikely(!__pyx_v_dU.memview)) __PYX_ERR(0, 350, __pyx_L3_error)
+    __pyx_v_dI_dj = __Pyx_PyObject_to_MemoryviewSlice_d_dc_double(values[5], PyBUF_WRITABLE); if (unlikely(!__pyx_v_dI_dj.memview)) __PYX_ERR(0, 350, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("grape", 1, 6, 6, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 343, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("grape", 1, 6, 6, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 350, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("unipolator.unitary_interpolation.UI.grape", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_10unipolator_21unitary_interpolation_2UI_14grape(((struct __pyx_obj_10unipolator_21unitary_interpolation_UI *)__pyx_v_self), __pyx_v_cs, __pyx_v_U_target, __pyx_v_target_indexes, __pyx_v_U, __pyx_v_dU, __pyx_v_dI_dj);
+  __pyx_r = __pyx_pf_10unipolator_21unitary_interpolation_2UI_16grape(((struct __pyx_obj_10unipolator_21unitary_interpolation_UI *)__pyx_v_self), __pyx_v_cs, __pyx_v_U_target, __pyx_v_target_indexes, __pyx_v_U, __pyx_v_dU, __pyx_v_dI_dj);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_10unipolator_21unitary_interpolation_2UI_14grape(struct __pyx_obj_10unipolator_21unitary_interpolation_UI *__pyx_v_self, __Pyx_memviewslice __pyx_v_cs, __Pyx_memviewslice __pyx_v_U_target, __Pyx_memviewslice __pyx_v_target_indexes, __Pyx_memviewslice __pyx_v_U, __Pyx_memviewslice __pyx_v_dU, __Pyx_memviewslice __pyx_v_dI_dj) {
+static PyObject *__pyx_pf_10unipolator_21unitary_interpolation_2UI_16grape(struct __pyx_obj_10unipolator_21unitary_interpolation_UI *__pyx_v_self, __Pyx_memviewslice __pyx_v_cs, __Pyx_memviewslice __pyx_v_U_target, __Pyx_memviewslice __pyx_v_target_indexes, __Pyx_memviewslice __pyx_v_U, __Pyx_memviewslice __pyx_v_dU, __Pyx_memviewslice __pyx_v_dI_dj) {
   int __pyx_v_i;
   int __pyx_v_j;
   int __pyx_v_steps;
   __pyx_t_double_complex *__pyx_v_new_p0;
   __pyx_t_double_complex *__pyx_v_new_q0;
   __pyx_t_double_complex *__pyx_v_p0;
   __pyx_t_double_complex *__pyx_v_q0;
@@ -8034,278 +8278,278 @@
   int __pyx_t_14;
   __pyx_t_double_complex *__pyx_t_15;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("grape", 0);
 
-  /* "unipolator/unitary_interpolation.pyx":346
+  /* "unipolator/unitary_interpolation.pyx":353
  *         # Calculate fidelity for a pulse and the differentials of the fidelity at every timestep using the grape trick
  *         cdef int i, j
  *         cdef int steps = cs.shape[0]             # <<<<<<<<<<<<<<
  * 
  *         cdef double complex *new_p0 = self.ur0
  */
   __pyx_v_steps = (__pyx_v_cs.shape[0]);
 
-  /* "unipolator/unitary_interpolation.pyx":348
+  /* "unipolator/unitary_interpolation.pyx":355
  *         cdef int steps = cs.shape[0]
  * 
  *         cdef double complex *new_p0 = self.ur0             # <<<<<<<<<<<<<<
  *         cdef double complex *new_q0 = self.ur1
  *         cdef double complex *p0 = self.ur4
  */
   __pyx_t_1 = __pyx_v_self->ur0;
   __pyx_v_new_p0 = __pyx_t_1;
 
-  /* "unipolator/unitary_interpolation.pyx":349
+  /* "unipolator/unitary_interpolation.pyx":356
  * 
  *         cdef double complex *new_p0 = self.ur0
  *         cdef double complex *new_q0 = self.ur1             # <<<<<<<<<<<<<<
  *         cdef double complex *p0 = self.ur4
  *         cdef double complex *q0 = self.ur5
  */
   __pyx_t_1 = __pyx_v_self->ur1;
   __pyx_v_new_q0 = __pyx_t_1;
 
-  /* "unipolator/unitary_interpolation.pyx":350
+  /* "unipolator/unitary_interpolation.pyx":357
  *         cdef double complex *new_p0 = self.ur0
  *         cdef double complex *new_q0 = self.ur1
  *         cdef double complex *p0 = self.ur4             # <<<<<<<<<<<<<<
  *         cdef double complex *q0 = self.ur5
  *         cdef double complex *u0 = &U[0, 0]
  */
   __pyx_t_1 = __pyx_v_self->ur4;
   __pyx_v_p0 = __pyx_t_1;
 
-  /* "unipolator/unitary_interpolation.pyx":351
+  /* "unipolator/unitary_interpolation.pyx":358
  *         cdef double complex *new_q0 = self.ur1
  *         cdef double complex *p0 = self.ur4
  *         cdef double complex *q0 = self.ur5             # <<<<<<<<<<<<<<
  *         cdef double complex *u0 = &U[0, 0]
  *         cdef double complex *u_tar = &U_target[0, 0]
  */
   __pyx_t_1 = __pyx_v_self->ur5;
   __pyx_v_q0 = __pyx_t_1;
 
-  /* "unipolator/unitary_interpolation.pyx":352
+  /* "unipolator/unitary_interpolation.pyx":359
  *         cdef double complex *p0 = self.ur4
  *         cdef double complex *q0 = self.ur5
  *         cdef double complex *u0 = &U[0, 0]             # <<<<<<<<<<<<<<
  *         cdef double complex *u_tar = &U_target[0, 0]
  *         cdef double complex *curr_u = self.ur3
  */
   __pyx_t_2 = 0;
   __pyx_t_3 = 0;
   __pyx_v_u0 = (&(*((__pyx_t_double_complex *) ( /* dim=1 */ ((char *) (((__pyx_t_double_complex *) ( /* dim=0 */ (__pyx_v_U.data + __pyx_t_2 * __pyx_v_U.strides[0]) )) + __pyx_t_3)) ))));
 
-  /* "unipolator/unitary_interpolation.pyx":353
+  /* "unipolator/unitary_interpolation.pyx":360
  *         cdef double complex *q0 = self.ur5
  *         cdef double complex *u0 = &U[0, 0]
  *         cdef double complex *u_tar = &U_target[0, 0]             # <<<<<<<<<<<<<<
  *         cdef double complex *curr_u = self.ur3
  *         cdef double complex *du = &dU[0,0,0]
  */
   __pyx_t_3 = 0;
   __pyx_t_2 = 0;
   __pyx_v_u_tar = (&(*((__pyx_t_double_complex *) ( /* dim=1 */ ((char *) (((__pyx_t_double_complex *) ( /* dim=0 */ (__pyx_v_U_target.data + __pyx_t_3 * __pyx_v_U_target.strides[0]) )) + __pyx_t_2)) ))));
 
-  /* "unipolator/unitary_interpolation.pyx":354
+  /* "unipolator/unitary_interpolation.pyx":361
  *         cdef double complex *u0 = &U[0, 0]
  *         cdef double complex *u_tar = &U_target[0, 0]
  *         cdef double complex *curr_u = self.ur3             # <<<<<<<<<<<<<<
  *         cdef double complex *du = &dU[0,0,0]
  * 
  */
   __pyx_t_1 = __pyx_v_self->ur3;
   __pyx_v_curr_u = __pyx_t_1;
 
-  /* "unipolator/unitary_interpolation.pyx":355
+  /* "unipolator/unitary_interpolation.pyx":362
  *         cdef double complex *u_tar = &U_target[0, 0]
  *         cdef double complex *curr_u = self.ur3
  *         cdef double complex *du = &dU[0,0,0]             # <<<<<<<<<<<<<<
  * 
  *         cdef double complex trM, trdM, two_nni
  */
   __pyx_t_2 = 0;
   __pyx_t_3 = 0;
   __pyx_t_4 = 0;
   __pyx_v_du = (&(*((__pyx_t_double_complex *) ( /* dim=2 */ ((char *) (((__pyx_t_double_complex *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_dU.data + __pyx_t_2 * __pyx_v_dU.strides[0]) ) + __pyx_t_3 * __pyx_v_dU.strides[1]) )) + __pyx_t_4)) ))));
 
-  /* "unipolator/unitary_interpolation.pyx":358
+  /* "unipolator/unitary_interpolation.pyx":365
  * 
  *         cdef double complex trM, trdM, two_nni
  *         cdef double n = <double> target_indexes.shape[0]             # <<<<<<<<<<<<<<
  *         cdef double nni = 1.0 / (n * (n + 1))
  *         cdef double one_minus = 1.0 - n * nni
  */
   __pyx_v_n = ((double)(__pyx_v_target_indexes.shape[0]));
 
-  /* "unipolator/unitary_interpolation.pyx":359
+  /* "unipolator/unitary_interpolation.pyx":366
  *         cdef double complex trM, trdM, two_nni
  *         cdef double n = <double> target_indexes.shape[0]
  *         cdef double nni = 1.0 / (n * (n + 1))             # <<<<<<<<<<<<<<
  *         cdef double one_minus = 1.0 - n * nni
  * 
  */
   __pyx_v_nni = (1.0 / (__pyx_v_n * (__pyx_v_n + 1.0)));
 
-  /* "unipolator/unitary_interpolation.pyx":360
+  /* "unipolator/unitary_interpolation.pyx":367
  *         cdef double n = <double> target_indexes.shape[0]
  *         cdef double nni = 1.0 / (n * (n + 1))
  *         cdef double one_minus = 1.0 - n * nni             # <<<<<<<<<<<<<<
  * 
  *         if not dI_dj.shape[0] == steps:
  */
   __pyx_v_one_minus = (1.0 - (__pyx_v_n * __pyx_v_nni));
 
-  /* "unipolator/unitary_interpolation.pyx":362
+  /* "unipolator/unitary_interpolation.pyx":369
  *         cdef double one_minus = 1.0 - n * nni
  * 
  *         if not dI_dj.shape[0] == steps:             # <<<<<<<<<<<<<<
  *             raise ValueError('Inputs must fulfill: cs.shape[0] = dI_dj.shape[0].')
  *         if not dI_dj.shape[1] == self.n_d_di:
  */
   __pyx_t_5 = ((!(((__pyx_v_dI_dj.shape[0]) == __pyx_v_steps) != 0)) != 0);
   if (unlikely(__pyx_t_5)) {
 
-    /* "unipolator/unitary_interpolation.pyx":363
+    /* "unipolator/unitary_interpolation.pyx":370
  * 
  *         if not dI_dj.shape[0] == steps:
  *             raise ValueError('Inputs must fulfill: cs.shape[0] = dI_dj.shape[0].')             # <<<<<<<<<<<<<<
  *         if not dI_dj.shape[1] == self.n_d_di:
  *             raise ValueError('Inputs must fulfill: which_diffs.shape[0] = dI_dj.shape[1].')
  */
-    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 363, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 370, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_Raise(__pyx_t_6, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __PYX_ERR(0, 363, __pyx_L1_error)
+    __PYX_ERR(0, 370, __pyx_L1_error)
 
-    /* "unipolator/unitary_interpolation.pyx":362
+    /* "unipolator/unitary_interpolation.pyx":369
  *         cdef double one_minus = 1.0 - n * nni
  * 
  *         if not dI_dj.shape[0] == steps:             # <<<<<<<<<<<<<<
  *             raise ValueError('Inputs must fulfill: cs.shape[0] = dI_dj.shape[0].')
  *         if not dI_dj.shape[1] == self.n_d_di:
  */
   }
 
-  /* "unipolator/unitary_interpolation.pyx":364
+  /* "unipolator/unitary_interpolation.pyx":371
  *         if not dI_dj.shape[0] == steps:
  *             raise ValueError('Inputs must fulfill: cs.shape[0] = dI_dj.shape[0].')
  *         if not dI_dj.shape[1] == self.n_d_di:             # <<<<<<<<<<<<<<
  *             raise ValueError('Inputs must fulfill: which_diffs.shape[0] = dI_dj.shape[1].')
  *         if not cs.shape[1] == self.n_d_di:
  */
   __pyx_t_5 = ((!(((__pyx_v_dI_dj.shape[1]) == __pyx_v_self->n_d_di) != 0)) != 0);
   if (unlikely(__pyx_t_5)) {
 
-    /* "unipolator/unitary_interpolation.pyx":365
+    /* "unipolator/unitary_interpolation.pyx":372
  *             raise ValueError('Inputs must fulfill: cs.shape[0] = dI_dj.shape[0].')
  *         if not dI_dj.shape[1] == self.n_d_di:
  *             raise ValueError('Inputs must fulfill: which_diffs.shape[0] = dI_dj.shape[1].')             # <<<<<<<<<<<<<<
  *         if not cs.shape[1] == self.n_d_di:
  *             raise ValueError('Inputs must fulfill: which_diffs.shape[0] = cs.shape[1].')
  */
-    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 365, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 372, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_Raise(__pyx_t_6, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __PYX_ERR(0, 365, __pyx_L1_error)
+    __PYX_ERR(0, 372, __pyx_L1_error)
 
-    /* "unipolator/unitary_interpolation.pyx":364
+    /* "unipolator/unitary_interpolation.pyx":371
  *         if not dI_dj.shape[0] == steps:
  *             raise ValueError('Inputs must fulfill: cs.shape[0] = dI_dj.shape[0].')
  *         if not dI_dj.shape[1] == self.n_d_di:             # <<<<<<<<<<<<<<
  *             raise ValueError('Inputs must fulfill: which_diffs.shape[0] = dI_dj.shape[1].')
  *         if not cs.shape[1] == self.n_d_di:
  */
   }
 
-  /* "unipolator/unitary_interpolation.pyx":366
+  /* "unipolator/unitary_interpolation.pyx":373
  *         if not dI_dj.shape[1] == self.n_d_di:
  *             raise ValueError('Inputs must fulfill: which_diffs.shape[0] = dI_dj.shape[1].')
  *         if not cs.shape[1] == self.n_d_di:             # <<<<<<<<<<<<<<
  *             raise ValueError('Inputs must fulfill: which_diffs.shape[0] = cs.shape[1].')
  *         # Fidelity constants
  */
   __pyx_t_5 = ((!(((__pyx_v_cs.shape[1]) == __pyx_v_self->n_d_di) != 0)) != 0);
   if (unlikely(__pyx_t_5)) {
 
-    /* "unipolator/unitary_interpolation.pyx":367
+    /* "unipolator/unitary_interpolation.pyx":374
  *             raise ValueError('Inputs must fulfill: which_diffs.shape[0] = dI_dj.shape[1].')
  *         if not cs.shape[1] == self.n_d_di:
  *             raise ValueError('Inputs must fulfill: which_diffs.shape[0] = cs.shape[1].')             # <<<<<<<<<<<<<<
  *         # Fidelity constants
  * 
  */
-    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 367, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 374, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_Raise(__pyx_t_6, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __PYX_ERR(0, 367, __pyx_L1_error)
+    __PYX_ERR(0, 374, __pyx_L1_error)
 
-    /* "unipolator/unitary_interpolation.pyx":366
+    /* "unipolator/unitary_interpolation.pyx":373
  *         if not dI_dj.shape[1] == self.n_d_di:
  *             raise ValueError('Inputs must fulfill: which_diffs.shape[0] = dI_dj.shape[1].')
  *         if not cs.shape[1] == self.n_d_di:             # <<<<<<<<<<<<<<
  *             raise ValueError('Inputs must fulfill: which_diffs.shape[0] = cs.shape[1].')
  *         # Fidelity constants
  */
   }
 
-  /* "unipolator/unitary_interpolation.pyx":370
+  /* "unipolator/unitary_interpolation.pyx":377
  *         # Fidelity constants
  * 
  *         self.expmH_pulse_pointer(cs, u0)             # <<<<<<<<<<<<<<
  *         #Dag_fast(U_target, self.Ur3) # -> Ur3 is identical to Q  -> replaced by new approach
  *         DagM_M_cdot_pointer(u_tar, u0, q0, self.d)
  */
-  __pyx_t_6 = ((struct __pyx_vtabstruct_10unipolator_21unitary_interpolation_UI *)__pyx_v_self->__pyx_vtab)->expmH_pulse_pointer(__pyx_v_self, __pyx_v_cs, __pyx_v_u0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 370, __pyx_L1_error)
+  __pyx_t_6 = ((struct __pyx_vtabstruct_10unipolator_21unitary_interpolation_UI *)__pyx_v_self->__pyx_vtab)->expmH_pulse_pointer(__pyx_v_self, __pyx_v_cs, __pyx_v_u0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 377, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-  /* "unipolator/unitary_interpolation.pyx":372
+  /* "unipolator/unitary_interpolation.pyx":379
  *         self.expmH_pulse_pointer(cs, u0)
  *         #Dag_fast(U_target, self.Ur3) # -> Ur3 is identical to Q  -> replaced by new approach
  *         DagM_M_cdot_pointer(u_tar, u0, q0, self.d)             # <<<<<<<<<<<<<<
  *         trM = target_indexes_trace_pointer(q0, self.d, target_indexes)
  *         two_nni = - 2 / (n * (n + 1)) * conj(trM)
  */
   __pyx_f_10unipolator_14blas_functions_DagM_M_cdot_pointer(__pyx_v_u_tar, __pyx_v_u0, __pyx_v_q0, __pyx_v_self->d);
 
-  /* "unipolator/unitary_interpolation.pyx":373
+  /* "unipolator/unitary_interpolation.pyx":380
  *         #Dag_fast(U_target, self.Ur3) # -> Ur3 is identical to Q  -> replaced by new approach
  *         DagM_M_cdot_pointer(u_tar, u0, q0, self.d)
  *         trM = target_indexes_trace_pointer(q0, self.d, target_indexes)             # <<<<<<<<<<<<<<
  *         two_nni = - 2 / (n * (n + 1)) * conj(trM)
  *         cdef double I0 = one_minus - nni * abs_2(trM) # Sub Fidelity
  */
   __pyx_v_trM = __pyx_f_10unipolator_14blas_functions_target_indexes_trace_pointer(__pyx_v_q0, __pyx_v_self->d, __pyx_v_target_indexes);
 
-  /* "unipolator/unitary_interpolation.pyx":374
+  /* "unipolator/unitary_interpolation.pyx":381
  *         DagM_M_cdot_pointer(u_tar, u0, q0, self.d)
  *         trM = target_indexes_trace_pointer(q0, self.d, target_indexes)
  *         two_nni = - 2 / (n * (n + 1)) * conj(trM)             # <<<<<<<<<<<<<<
  *         cdef double I0 = one_minus - nni * abs_2(trM) # Sub Fidelity
  * 
  */
   __pyx_v_two_nni = __Pyx_c_prod_double(__pyx_t_double_complex_from_parts((-2.0 / (__pyx_v_n * (__pyx_v_n + 1.0))), 0), __pyx_f_10unipolator_11exp_and_log_conj(__pyx_v_trM));
 
-  /* "unipolator/unitary_interpolation.pyx":375
+  /* "unipolator/unitary_interpolation.pyx":382
  *         trM = target_indexes_trace_pointer(q0, self.d, target_indexes)
  *         two_nni = - 2 / (n * (n + 1)) * conj(trM)
  *         cdef double I0 = one_minus - nni * abs_2(trM) # Sub Fidelity             # <<<<<<<<<<<<<<
  * 
  *         # Do GRAPE trick
  */
   __pyx_v_I0 = (__pyx_v_one_minus - (__pyx_v_nni * __pyx_f_10unipolator_11exp_and_log_abs_2(__pyx_v_trM, 0)));
 
-  /* "unipolator/unitary_interpolation.pyx":378
+  /* "unipolator/unitary_interpolation.pyx":385
  * 
  *         # Do GRAPE trick
  *         self.dexpmH_pointer(cs[0,:], curr_u, du) # Calculate Unitary and its derivatives             # <<<<<<<<<<<<<<
  *         M_DagM_cdot_pointer(q0, curr_u, new_q0, self.d)  # Reduce q0
  *         copy_pointer(new_q0, q0, self.d2)
  */
   __pyx_t_7.data = __pyx_v_cs.data;
@@ -8317,113 +8561,113 @@
         __pyx_t_7.data += __pyx_tmp_idx * __pyx_tmp_stride;
 }
 
 __pyx_t_7.shape[0] = __pyx_v_cs.shape[1];
 __pyx_t_7.strides[0] = __pyx_v_cs.strides[1];
     __pyx_t_7.suboffsets[0] = -1;
 
-__pyx_t_6 = ((struct __pyx_vtabstruct_10unipolator_21unitary_interpolation_UI *)__pyx_v_self->__pyx_vtab)->dexpmH_pointer(__pyx_v_self, __pyx_t_7, __pyx_v_curr_u, __pyx_v_du); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 378, __pyx_L1_error)
+__pyx_t_6 = ((struct __pyx_vtabstruct_10unipolator_21unitary_interpolation_UI *)__pyx_v_self->__pyx_vtab)->dexpmH_pointer(__pyx_v_self, __pyx_t_7, __pyx_v_curr_u, __pyx_v_du); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 385, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __PYX_XDEC_MEMVIEW(&__pyx_t_7, 1);
   __pyx_t_7.memview = NULL;
   __pyx_t_7.data = NULL;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-  /* "unipolator/unitary_interpolation.pyx":379
+  /* "unipolator/unitary_interpolation.pyx":386
  *         # Do GRAPE trick
  *         self.dexpmH_pointer(cs[0,:], curr_u, du) # Calculate Unitary and its derivatives
  *         M_DagM_cdot_pointer(q0, curr_u, new_q0, self.d)  # Reduce q0             # <<<<<<<<<<<<<<
  *         copy_pointer(new_q0, q0, self.d2)
  *         for j in range(self.n_d_di):
  */
   __pyx_f_10unipolator_14blas_functions_M_DagM_cdot_pointer(__pyx_v_q0, __pyx_v_curr_u, __pyx_v_new_q0, __pyx_v_self->d);
 
-  /* "unipolator/unitary_interpolation.pyx":380
+  /* "unipolator/unitary_interpolation.pyx":387
  *         self.dexpmH_pointer(cs[0,:], curr_u, du) # Calculate Unitary and its derivatives
  *         M_DagM_cdot_pointer(q0, curr_u, new_q0, self.d)  # Reduce q0
  *         copy_pointer(new_q0, q0, self.d2)             # <<<<<<<<<<<<<<
  *         for j in range(self.n_d_di):
  *             #MM_cdot_pointer(curr_du, p0, new_p0, self.d)  # p0 is not defined yet
  */
   __pyx_f_10unipolator_11exp_and_log_copy_pointer(__pyx_v_new_q0, __pyx_v_q0, __pyx_v_self->d2);
 
-  /* "unipolator/unitary_interpolation.pyx":381
+  /* "unipolator/unitary_interpolation.pyx":388
  *         M_DagM_cdot_pointer(q0, curr_u, new_q0, self.d)  # Reduce q0
  *         copy_pointer(new_q0, q0, self.d2)
  *         for j in range(self.n_d_di):             # <<<<<<<<<<<<<<
  *             #MM_cdot_pointer(curr_du, p0, new_p0, self.d)  # p0 is not defined yet
  *             trdM = tr_dot_pointer_target_indexes(q0, du, self.d, target_indexes)
  */
   __pyx_t_8 = __pyx_v_self->n_d_di;
   __pyx_t_9 = __pyx_t_8;
   for (__pyx_t_10 = 0; __pyx_t_10 < __pyx_t_9; __pyx_t_10+=1) {
     __pyx_v_j = __pyx_t_10;
 
-    /* "unipolator/unitary_interpolation.pyx":383
+    /* "unipolator/unitary_interpolation.pyx":390
  *         for j in range(self.n_d_di):
  *             #MM_cdot_pointer(curr_du, p0, new_p0, self.d)  # p0 is not defined yet
  *             trdM = tr_dot_pointer_target_indexes(q0, du, self.d, target_indexes)             # <<<<<<<<<<<<<<
  *             dI_dj[0, j] = ( two_nni * trdM ).real
  *             du += self.d2
  */
     __pyx_v_trdM = __pyx_f_10unipolator_14blas_functions_tr_dot_pointer_target_indexes(__pyx_v_q0, __pyx_v_du, __pyx_v_self->d, __pyx_v_target_indexes);
 
-    /* "unipolator/unitary_interpolation.pyx":384
+    /* "unipolator/unitary_interpolation.pyx":391
  *             #MM_cdot_pointer(curr_du, p0, new_p0, self.d)  # p0 is not defined yet
  *             trdM = tr_dot_pointer_target_indexes(q0, du, self.d, target_indexes)
  *             dI_dj[0, j] = ( two_nni * trdM ).real             # <<<<<<<<<<<<<<
  *             du += self.d2
  *         copy_pointer(curr_u, p0, self.d2)  # Define p0 from curr_u
  */
     __pyx_t_11 = __Pyx_CREAL(__Pyx_c_prod_double(__pyx_v_two_nni, __pyx_v_trdM));
     __pyx_t_4 = 0;
     __pyx_t_3 = __pyx_v_j;
     *((double *) ( /* dim=1 */ ((char *) (((double *) ( /* dim=0 */ (__pyx_v_dI_dj.data + __pyx_t_4 * __pyx_v_dI_dj.strides[0]) )) + __pyx_t_3)) )) = __pyx_t_11;
 
-    /* "unipolator/unitary_interpolation.pyx":385
+    /* "unipolator/unitary_interpolation.pyx":392
  *             trdM = tr_dot_pointer_target_indexes(q0, du, self.d, target_indexes)
  *             dI_dj[0, j] = ( two_nni * trdM ).real
  *             du += self.d2             # <<<<<<<<<<<<<<
  *         copy_pointer(curr_u, p0, self.d2)  # Define p0 from curr_u
  *         for i in range(1, steps):
  */
     __pyx_v_du = (__pyx_v_du + __pyx_v_self->d2);
   }
 
-  /* "unipolator/unitary_interpolation.pyx":386
+  /* "unipolator/unitary_interpolation.pyx":393
  *             dI_dj[0, j] = ( two_nni * trdM ).real
  *             du += self.d2
  *         copy_pointer(curr_u, p0, self.d2)  # Define p0 from curr_u             # <<<<<<<<<<<<<<
  *         for i in range(1, steps):
  *             du -= self.d2 * self.n_d_di
  */
   __pyx_f_10unipolator_11exp_and_log_copy_pointer(__pyx_v_curr_u, __pyx_v_p0, __pyx_v_self->d2);
 
-  /* "unipolator/unitary_interpolation.pyx":387
+  /* "unipolator/unitary_interpolation.pyx":394
  *             du += self.d2
  *         copy_pointer(curr_u, p0, self.d2)  # Define p0 from curr_u
  *         for i in range(1, steps):             # <<<<<<<<<<<<<<
  *             du -= self.d2 * self.n_d_di
  *             self.dexpmH_pointer(cs[i, :], curr_u, du)  # Calculate Unitary and its derivatives
  */
   __pyx_t_8 = __pyx_v_steps;
   __pyx_t_9 = __pyx_t_8;
   for (__pyx_t_10 = 1; __pyx_t_10 < __pyx_t_9; __pyx_t_10+=1) {
     __pyx_v_i = __pyx_t_10;
 
-    /* "unipolator/unitary_interpolation.pyx":388
+    /* "unipolator/unitary_interpolation.pyx":395
  *         copy_pointer(curr_u, p0, self.d2)  # Define p0 from curr_u
  *         for i in range(1, steps):
  *             du -= self.d2 * self.n_d_di             # <<<<<<<<<<<<<<
  *             self.dexpmH_pointer(cs[i, :], curr_u, du)  # Calculate Unitary and its derivatives
  *             M_DagM_cdot_pointer(q0, curr_u, new_q0, self.d)  # Remove current unitary (curr_u) from Q
  */
     __pyx_v_du = (__pyx_v_du - (__pyx_v_self->d2 * __pyx_v_self->n_d_di));
 
-    /* "unipolator/unitary_interpolation.pyx":389
+    /* "unipolator/unitary_interpolation.pyx":396
  *         for i in range(1, steps):
  *             du -= self.d2 * self.n_d_di
  *             self.dexpmH_pointer(cs[i, :], curr_u, du)  # Calculate Unitary and its derivatives             # <<<<<<<<<<<<<<
  *             M_DagM_cdot_pointer(q0, curr_u, new_q0, self.d)  # Remove current unitary (curr_u) from Q
  *             for j in range(self.n_d_di):
  */
     __pyx_t_7.data = __pyx_v_cs.data;
@@ -8435,155 +8679,155 @@
         __pyx_t_7.data += __pyx_tmp_idx * __pyx_tmp_stride;
 }
 
 __pyx_t_7.shape[0] = __pyx_v_cs.shape[1];
 __pyx_t_7.strides[0] = __pyx_v_cs.strides[1];
     __pyx_t_7.suboffsets[0] = -1;
 
-__pyx_t_6 = ((struct __pyx_vtabstruct_10unipolator_21unitary_interpolation_UI *)__pyx_v_self->__pyx_vtab)->dexpmH_pointer(__pyx_v_self, __pyx_t_7, __pyx_v_curr_u, __pyx_v_du); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 389, __pyx_L1_error)
+__pyx_t_6 = ((struct __pyx_vtabstruct_10unipolator_21unitary_interpolation_UI *)__pyx_v_self->__pyx_vtab)->dexpmH_pointer(__pyx_v_self, __pyx_t_7, __pyx_v_curr_u, __pyx_v_du); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 396, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __PYX_XDEC_MEMVIEW(&__pyx_t_7, 1);
     __pyx_t_7.memview = NULL;
     __pyx_t_7.data = NULL;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-    /* "unipolator/unitary_interpolation.pyx":390
+    /* "unipolator/unitary_interpolation.pyx":397
  *             du -= self.d2 * self.n_d_di
  *             self.dexpmH_pointer(cs[i, :], curr_u, du)  # Calculate Unitary and its derivatives
  *             M_DagM_cdot_pointer(q0, curr_u, new_q0, self.d)  # Remove current unitary (curr_u) from Q             # <<<<<<<<<<<<<<
  *             for j in range(self.n_d_di):
  *                 MM_cdot_pointer(du, p0, new_p0, self.d)
  */
     __pyx_f_10unipolator_14blas_functions_M_DagM_cdot_pointer(__pyx_v_q0, __pyx_v_curr_u, __pyx_v_new_q0, __pyx_v_self->d);
 
-    /* "unipolator/unitary_interpolation.pyx":391
+    /* "unipolator/unitary_interpolation.pyx":398
  *             self.dexpmH_pointer(cs[i, :], curr_u, du)  # Calculate Unitary and its derivatives
  *             M_DagM_cdot_pointer(q0, curr_u, new_q0, self.d)  # Remove current unitary (curr_u) from Q
  *             for j in range(self.n_d_di):             # <<<<<<<<<<<<<<
  *                 MM_cdot_pointer(du, p0, new_p0, self.d)
  *                 trdM = tr_dot_pointer_target_indexes(new_q0, new_p0, self.d, target_indexes)
  */
     __pyx_t_12 = __pyx_v_self->n_d_di;
     __pyx_t_13 = __pyx_t_12;
     for (__pyx_t_14 = 0; __pyx_t_14 < __pyx_t_13; __pyx_t_14+=1) {
       __pyx_v_j = __pyx_t_14;
 
-      /* "unipolator/unitary_interpolation.pyx":392
+      /* "unipolator/unitary_interpolation.pyx":399
  *             M_DagM_cdot_pointer(q0, curr_u, new_q0, self.d)  # Remove current unitary (curr_u) from Q
  *             for j in range(self.n_d_di):
  *                 MM_cdot_pointer(du, p0, new_p0, self.d)             # <<<<<<<<<<<<<<
  *                 trdM = tr_dot_pointer_target_indexes(new_q0, new_p0, self.d, target_indexes)
  *                 dI_dj[i, j] = ( two_nni * trdM ).real
  */
       __pyx_f_10unipolator_14blas_functions_MM_cdot_pointer(__pyx_v_du, __pyx_v_p0, __pyx_v_new_p0, __pyx_v_self->d);
 
-      /* "unipolator/unitary_interpolation.pyx":393
+      /* "unipolator/unitary_interpolation.pyx":400
  *             for j in range(self.n_d_di):
  *                 MM_cdot_pointer(du, p0, new_p0, self.d)
  *                 trdM = tr_dot_pointer_target_indexes(new_q0, new_p0, self.d, target_indexes)             # <<<<<<<<<<<<<<
  *                 dI_dj[i, j] = ( two_nni * trdM ).real
  *                 du += self.d2
  */
       __pyx_v_trdM = __pyx_f_10unipolator_14blas_functions_tr_dot_pointer_target_indexes(__pyx_v_new_q0, __pyx_v_new_p0, __pyx_v_self->d, __pyx_v_target_indexes);
 
-      /* "unipolator/unitary_interpolation.pyx":394
+      /* "unipolator/unitary_interpolation.pyx":401
  *                 MM_cdot_pointer(du, p0, new_p0, self.d)
  *                 trdM = tr_dot_pointer_target_indexes(new_q0, new_p0, self.d, target_indexes)
  *                 dI_dj[i, j] = ( two_nni * trdM ).real             # <<<<<<<<<<<<<<
  *                 du += self.d2
  *             MM_cdot_pointer(curr_u, p0, new_p0, self.d)  # Add current unitary (curr_u) to P
  */
       __pyx_t_11 = __Pyx_CREAL(__Pyx_c_prod_double(__pyx_v_two_nni, __pyx_v_trdM));
       __pyx_t_3 = __pyx_v_i;
       __pyx_t_4 = __pyx_v_j;
       *((double *) ( /* dim=1 */ ((char *) (((double *) ( /* dim=0 */ (__pyx_v_dI_dj.data + __pyx_t_3 * __pyx_v_dI_dj.strides[0]) )) + __pyx_t_4)) )) = __pyx_t_11;
 
-      /* "unipolator/unitary_interpolation.pyx":395
+      /* "unipolator/unitary_interpolation.pyx":402
  *                 trdM = tr_dot_pointer_target_indexes(new_q0, new_p0, self.d, target_indexes)
  *                 dI_dj[i, j] = ( two_nni * trdM ).real
  *                 du += self.d2             # <<<<<<<<<<<<<<
  *             MM_cdot_pointer(curr_u, p0, new_p0, self.d)  # Add current unitary (curr_u) to P
  *             #copy_pointer(new_p0, p0, self.d2)
  */
       __pyx_v_du = (__pyx_v_du + __pyx_v_self->d2);
     }
 
-    /* "unipolator/unitary_interpolation.pyx":396
+    /* "unipolator/unitary_interpolation.pyx":403
  *                 dI_dj[i, j] = ( two_nni * trdM ).real
  *                 du += self.d2
  *             MM_cdot_pointer(curr_u, p0, new_p0, self.d)  # Add current unitary (curr_u) to P             # <<<<<<<<<<<<<<
  *             #copy_pointer(new_p0, p0, self.d2)
  *             #copy_pointer(new_q0, q0, self.d2)
  */
     __pyx_f_10unipolator_14blas_functions_MM_cdot_pointer(__pyx_v_curr_u, __pyx_v_p0, __pyx_v_new_p0, __pyx_v_self->d);
 
-    /* "unipolator/unitary_interpolation.pyx":400
+    /* "unipolator/unitary_interpolation.pyx":407
  *             #copy_pointer(new_q0, q0, self.d2)
  *             # flip pointers
  *             self.ur0, self.ur4 = self.ur4, self.ur0             # <<<<<<<<<<<<<<
  *             self.ur1, self.ur5 = self.ur5, self.ur1
  *             new_p0, p0 = p0, new_p0
  */
     __pyx_t_1 = __pyx_v_self->ur4;
     __pyx_t_15 = __pyx_v_self->ur0;
     __pyx_v_self->ur0 = __pyx_t_1;
     __pyx_v_self->ur4 = __pyx_t_15;
 
-    /* "unipolator/unitary_interpolation.pyx":401
+    /* "unipolator/unitary_interpolation.pyx":408
  *             # flip pointers
  *             self.ur0, self.ur4 = self.ur4, self.ur0
  *             self.ur1, self.ur5 = self.ur5, self.ur1             # <<<<<<<<<<<<<<
  *             new_p0, p0 = p0, new_p0
  *             new_q0, q0 = q0, new_q0
  */
     __pyx_t_15 = __pyx_v_self->ur5;
     __pyx_t_1 = __pyx_v_self->ur1;
     __pyx_v_self->ur1 = __pyx_t_15;
     __pyx_v_self->ur5 = __pyx_t_1;
 
-    /* "unipolator/unitary_interpolation.pyx":402
+    /* "unipolator/unitary_interpolation.pyx":409
  *             self.ur0, self.ur4 = self.ur4, self.ur0
  *             self.ur1, self.ur5 = self.ur5, self.ur1
  *             new_p0, p0 = p0, new_p0             # <<<<<<<<<<<<<<
  *             new_q0, q0 = q0, new_q0
  *         return I0
  */
     __pyx_t_1 = __pyx_v_p0;
     __pyx_t_15 = __pyx_v_new_p0;
     __pyx_v_new_p0 = __pyx_t_1;
     __pyx_v_p0 = __pyx_t_15;
 
-    /* "unipolator/unitary_interpolation.pyx":403
+    /* "unipolator/unitary_interpolation.pyx":410
  *             self.ur1, self.ur5 = self.ur5, self.ur1
  *             new_p0, p0 = p0, new_p0
  *             new_q0, q0 = q0, new_q0             # <<<<<<<<<<<<<<
  *         return I0
  * 
  */
     __pyx_t_15 = __pyx_v_q0;
     __pyx_t_1 = __pyx_v_new_q0;
     __pyx_v_new_q0 = __pyx_t_15;
     __pyx_v_q0 = __pyx_t_1;
   }
 
-  /* "unipolator/unitary_interpolation.pyx":404
+  /* "unipolator/unitary_interpolation.pyx":411
  *             new_p0, p0 = p0, new_p0
  *             new_q0, q0 = q0, new_q0
  *         return I0             # <<<<<<<<<<<<<<
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_6 = PyFloat_FromDouble(__pyx_v_I0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 404, __pyx_L1_error)
+  __pyx_t_6 = PyFloat_FromDouble(__pyx_v_I0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 411, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_r = __pyx_t_6;
   __pyx_t_6 = 0;
   goto __pyx_L0;
 
-  /* "unipolator/unitary_interpolation.pyx":343
- *         self.expmH_pulse_pointer(cs, u0)
+  /* "unipolator/unitary_interpolation.pyx":350
+ *             u0 += self.d2
  * 
  *     def grape(self, double[:,::1] cs, double complex[:,::1] U_target, int[::1] target_indexes, double complex[:,::1] U, double complex[:,:,::1] dU, double[:,::1] dI_dj):             # <<<<<<<<<<<<<<
  *         # Calculate fidelity for a pulse and the differentials of the fidelity at every timestep using the grape trick
  *         cdef int i, j
  */
 
   /* function exit code */
@@ -8607,28 +8851,28 @@
 /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_10unipolator_21unitary_interpolation_2UI_17__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static char __pyx_doc_10unipolator_21unitary_interpolation_2UI_16__reduce_cython__[] = "UI.__reduce_cython__(self)";
-static PyObject *__pyx_pw_10unipolator_21unitary_interpolation_2UI_17__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_10unipolator_21unitary_interpolation_2UI_19__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc_10unipolator_21unitary_interpolation_2UI_18__reduce_cython__[] = "UI.__reduce_cython__(self)";
+static PyObject *__pyx_pw_10unipolator_21unitary_interpolation_2UI_19__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_10unipolator_21unitary_interpolation_2UI_16__reduce_cython__(((struct __pyx_obj_10unipolator_21unitary_interpolation_UI *)__pyx_v_self));
+  __pyx_r = __pyx_pf_10unipolator_21unitary_interpolation_2UI_18__reduce_cython__(((struct __pyx_obj_10unipolator_21unitary_interpolation_UI *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_10unipolator_21unitary_interpolation_2UI_16__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_10unipolator_21unitary_interpolation_UI *__pyx_v_self) {
+static PyObject *__pyx_pf_10unipolator_21unitary_interpolation_2UI_18__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_10unipolator_21unitary_interpolation_UI *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__reduce_cython__", 0);
@@ -8665,28 +8909,28 @@
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_10unipolator_21unitary_interpolation_2UI_19__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
-static char __pyx_doc_10unipolator_21unitary_interpolation_2UI_18__setstate_cython__[] = "UI.__setstate_cython__(self, __pyx_state)";
-static PyObject *__pyx_pw_10unipolator_21unitary_interpolation_2UI_19__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pw_10unipolator_21unitary_interpolation_2UI_21__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
+static char __pyx_doc_10unipolator_21unitary_interpolation_2UI_20__setstate_cython__[] = "UI.__setstate_cython__(self, __pyx_state)";
+static PyObject *__pyx_pw_10unipolator_21unitary_interpolation_2UI_21__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_10unipolator_21unitary_interpolation_2UI_18__setstate_cython__(((struct __pyx_obj_10unipolator_21unitary_interpolation_UI *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
+  __pyx_r = __pyx_pf_10unipolator_21unitary_interpolation_2UI_20__setstate_cython__(((struct __pyx_obj_10unipolator_21unitary_interpolation_UI *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_10unipolator_21unitary_interpolation_2UI_18__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_10unipolator_21unitary_interpolation_UI *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pf_10unipolator_21unitary_interpolation_2UI_20__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_10unipolator_21unitary_interpolation_UI *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
@@ -22896,17 +23140,18 @@
 static PyMethodDef __pyx_methods_10unipolator_21unitary_interpolation_UI[] = {
   {"set_which_diffs", (PyCFunction)__pyx_pw_10unipolator_21unitary_interpolation_2UI_3set_which_diffs, METH_O, __pyx_doc_10unipolator_21unitary_interpolation_2UI_2set_which_diffs},
   {"get_single_param", (PyCFunction)__pyx_pw_10unipolator_21unitary_interpolation_2UI_5get_single_param, METH_O, __pyx_doc_10unipolator_21unitary_interpolation_2UI_4get_single_param},
   {"get_cache", (PyCFunction)__pyx_pw_10unipolator_21unitary_interpolation_2UI_7get_cache, METH_NOARGS, __pyx_doc_10unipolator_21unitary_interpolation_2UI_6get_cache},
   {"expmH", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_10unipolator_21unitary_interpolation_2UI_9expmH, METH_VARARGS|METH_KEYWORDS, __pyx_doc_10unipolator_21unitary_interpolation_2UI_8expmH},
   {"dexpmH", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_10unipolator_21unitary_interpolation_2UI_11dexpmH, METH_VARARGS|METH_KEYWORDS, __pyx_doc_10unipolator_21unitary_interpolation_2UI_10dexpmH},
   {"expmH_pulse", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_10unipolator_21unitary_interpolation_2UI_13expmH_pulse, METH_VARARGS|METH_KEYWORDS, __pyx_doc_10unipolator_21unitary_interpolation_2UI_12expmH_pulse},
-  {"grape", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_10unipolator_21unitary_interpolation_2UI_15grape, METH_VARARGS|METH_KEYWORDS, __pyx_doc_10unipolator_21unitary_interpolation_2UI_14grape},
-  {"__reduce_cython__", (PyCFunction)__pyx_pw_10unipolator_21unitary_interpolation_2UI_17__reduce_cython__, METH_NOARGS, __pyx_doc_10unipolator_21unitary_interpolation_2UI_16__reduce_cython__},
-  {"__setstate_cython__", (PyCFunction)__pyx_pw_10unipolator_21unitary_interpolation_2UI_19__setstate_cython__, METH_O, __pyx_doc_10unipolator_21unitary_interpolation_2UI_18__setstate_cython__},
+  {"expmH_pulse_no_multiply", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_10unipolator_21unitary_interpolation_2UI_15expmH_pulse_no_multiply, METH_VARARGS|METH_KEYWORDS, __pyx_doc_10unipolator_21unitary_interpolation_2UI_14expmH_pulse_no_multiply},
+  {"grape", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_10unipolator_21unitary_interpolation_2UI_17grape, METH_VARARGS|METH_KEYWORDS, __pyx_doc_10unipolator_21unitary_interpolation_2UI_16grape},
+  {"__reduce_cython__", (PyCFunction)__pyx_pw_10unipolator_21unitary_interpolation_2UI_19__reduce_cython__, METH_NOARGS, __pyx_doc_10unipolator_21unitary_interpolation_2UI_18__reduce_cython__},
+  {"__setstate_cython__", (PyCFunction)__pyx_pw_10unipolator_21unitary_interpolation_2UI_21__setstate_cython__, METH_O, __pyx_doc_10unipolator_21unitary_interpolation_2UI_20__setstate_cython__},
   {0, 0, 0, 0}
 };
 
 static PyTypeObject __pyx_type_10unipolator_21unitary_interpolation_UI = {
   PyVarObject_HEAD_INIT(0, 0)
   "unipolator.unitary_interpolation.UI", /*tp_name*/
   sizeof(struct __pyx_obj_10unipolator_21unitary_interpolation_UI), /*tp_basicsize*/
@@ -23943,44 +24188,44 @@
  *         # First timestep
  *         if steps_1 % 2:
  */
   __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_u_The_coefficient_matrix_must_be_o); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 319, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__6);
   __Pyx_GIVEREF(__pyx_tuple__6);
 
-  /* "unipolator/unitary_interpolation.pyx":363
+  /* "unipolator/unitary_interpolation.pyx":370
  * 
  *         if not dI_dj.shape[0] == steps:
  *             raise ValueError('Inputs must fulfill: cs.shape[0] = dI_dj.shape[0].')             # <<<<<<<<<<<<<<
  *         if not dI_dj.shape[1] == self.n_d_di:
  *             raise ValueError('Inputs must fulfill: which_diffs.shape[0] = dI_dj.shape[1].')
  */
-  __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_u_Inputs_must_fulfill_cs_shape_0_d); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 363, __pyx_L1_error)
+  __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_u_Inputs_must_fulfill_cs_shape_0_d); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 370, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__7);
   __Pyx_GIVEREF(__pyx_tuple__7);
 
-  /* "unipolator/unitary_interpolation.pyx":365
+  /* "unipolator/unitary_interpolation.pyx":372
  *             raise ValueError('Inputs must fulfill: cs.shape[0] = dI_dj.shape[0].')
  *         if not dI_dj.shape[1] == self.n_d_di:
  *             raise ValueError('Inputs must fulfill: which_diffs.shape[0] = dI_dj.shape[1].')             # <<<<<<<<<<<<<<
  *         if not cs.shape[1] == self.n_d_di:
  *             raise ValueError('Inputs must fulfill: which_diffs.shape[0] = cs.shape[1].')
  */
-  __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_u_Inputs_must_fulfill_which_diffs_2); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 365, __pyx_L1_error)
+  __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_u_Inputs_must_fulfill_which_diffs_2); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 372, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "unipolator/unitary_interpolation.pyx":367
+  /* "unipolator/unitary_interpolation.pyx":374
  *             raise ValueError('Inputs must fulfill: which_diffs.shape[0] = dI_dj.shape[1].')
  *         if not cs.shape[1] == self.n_d_di:
  *             raise ValueError('Inputs must fulfill: which_diffs.shape[0] = cs.shape[1].')             # <<<<<<<<<<<<<<
  *         # Fidelity constants
  * 
  */
-  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_Inputs_must_fulfill_which_diffs_3); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 367, __pyx_L1_error)
+  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_Inputs_must_fulfill_which_diffs_3); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 374, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
```

### Comparing `unipolator-0.2.6/src/unipolator/unitary_interpolation.pyx` & `unipolator-0.2.7/src/unipolator/unitary_interpolation.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -336,14 +336,21 @@
             self.single_parameters2oddgrid(cs[steps_1,:])
             self.interpolate_single_u(ur2)
             MM_cdot_pointer(ur2, u0, ur3, self.d)
     def expmH_pulse(self, double[:,::1] cs, double complex[:,::1] U):
         cdef double complex *u0 = &U[0, 0]
         self.expmH_pulse_pointer(cs, u0)
 
+    def expmH_pulse_no_multiply(self, double[:,::1] cs, double complex[:,:,::1] U):
+        cdef double complex *u0 = &U[0, 0, 0]
+        cdef how_many = cs.shape[0]
+        for i in range(how_many):
+            self.expmH_pointer(cs[i,:], u0)
+            u0 += self.d2
+
     def grape(self, double[:,::1] cs, double complex[:,::1] U_target, int[::1] target_indexes, double complex[:,::1] U, double complex[:,:,::1] dU, double[:,::1] dI_dj):
         # Calculate fidelity for a pulse and the differentials of the fidelity at every timestep using the grape trick
         cdef int i, j
         cdef int steps = cs.shape[0]
 
         cdef double complex *new_p0 = self.ur0
         cdef double complex *new_q0 = self.ur1
```

### Comparing `unipolator-0.2.6/src/unipolator.egg-info/PKG-INFO` & `unipolator-0.2.7/src/unipolator.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: unipolator
-Version: 0.2.6
+Version: 0.2.7
 Summary: Unipolator allows for n dimensional unitary interpolation, and the calculation of propagators using unitary interpolation. Speeds up your propagators for linear quantum systems.
 Home-page: https://github.com/Ntropic/unipolator
-Download-URL: https://github.com/Ntropic/unipolator/archive/refs/tags/v0.2.6.tar.gz
+Download-URL: https://github.com/Ntropic/unipolator/archive/refs/tags/v0.2.7.tar.gz
 Author: Michael Schilling
 Author-email: michael@ntropic.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
@@ -44,10 +44,9 @@
 ui.expmH_pulse(cs, U)
 ``` 
 Finally the GRAPE method is supported via (pass an array `dI_dj.shape(n, cs.shape[0])` to store the gradients)
 ```
 ui.grape(cs, U_target, target_indexes, U, dU, dI_dj)
 ```
 
-
- ## Author: 
- Michael Schilling
+## Author: 
+Michael Schilling
```

### Comparing `unipolator-0.2.6/src/unipolator.egg-info/SOURCES.txt` & `unipolator-0.2.7/src/unipolator.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 src/unipolator/__init__.py
 src/unipolator/blas_functions.c
 src/unipolator/blas_functions.pxd
 src/unipolator/blas_functions.pyx
 src/unipolator/caching.c
 src/unipolator/caching.pxd
 src/unipolator/caching.pyx
-src/unipolator/discrete_quantum.py
 src/unipolator/exp_and_log.c
 src/unipolator/exp_and_log.pxd
 src/unipolator/exp_and_log.pyx
 src/unipolator/hamiltonian_system.c
 src/unipolator/hamiltonian_system.pyx
 src/unipolator/indexing.c
 src/unipolator/indexing.pxd
```

