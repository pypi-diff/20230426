# Comparing `tmp/pyfed_macos-0.0.4.tar.gz` & `tmp/pyfed_macos-0.0.6.tar.gz`

## Comparing `pyfed_macos-0.0.4.tar` & `pyfed_macos-0.0.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pyfed_macos-0.0.4/.DS_Store
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pyfed_macos-0.0.4/.pypirc
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyfed_macos-0.0.4/src/__init__.py
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 pyfed_macos-0.0.4/src/global_var.py
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 pyfed_macos-0.0.4/src/ml_socket.py
--rw-r--r--   0        0        0     4175 2020-02-02 00:00:00.000000 pyfed_macos-0.0.4/src/pyfed.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pyfed_macos-0.0.4/.gitignore
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 pyfed_macos-0.0.4/LICENSE
--rw-r--r--   0        0        0     5827 2020-02-02 00:00:00.000000 pyfed_macos-0.0.4/README.md
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 pyfed_macos-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     6528 2020-02-02 00:00:00.000000 pyfed_macos-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pyfed_macos-0.0.6/.DS_Store
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pyfed_macos-0.0.6/.pypirc
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyfed_macos-0.0.6/src/pyfed/__init__.py
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 pyfed_macos-0.0.6/src/pyfed/global_var.py
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 pyfed_macos-0.0.6/src/pyfed/ml_socket.py
+-rw-r--r--   0        0        0     4175 2020-02-02 00:00:00.000000 pyfed_macos-0.0.6/src/pyfed/pyfed.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pyfed_macos-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 pyfed_macos-0.0.6/LICENSE
+-rw-r--r--   0        0        0     5827 2020-02-02 00:00:00.000000 pyfed_macos-0.0.6/README.md
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 pyfed_macos-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     6528 2020-02-02 00:00:00.000000 pyfed_macos-0.0.6/PKG-INFO
```

### Comparing `pyfed_macos-0.0.4/.DS_Store` & `pyfed_macos-0.0.6/.DS_Store`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 00000000: 0000 0001 4275 6431 0000 1000 0000 0800  ....Bud1........
 00000010: 0000 1000 0000 0209 0000 0000 0000 0000  ................
 00000020: 0000 0000 0000 0000 0000 0000 0000 0800  ................
 00000030: 0000 0800 0000 0000 0000 0000 0000 0000  ................
-00000040: 0000 0000 0000 0002 0000 0000 0000 0007  ................
-00000050: 0000 0001 0000 1000 7370 626c 6f62 0000  ........spblob..
-00000060: 00b8 6270 0000 0000 0000 0000 0000 0000  ..bp............
+00000040: 0000 0000 0000 0002 0000 0000 0000 0008  ................
+00000050: 0000 0001 0000 1000 6473 636c 626f 6f6c  ........dsclbool
+00000060: 0100 0000 0000 0000 0000 0000 0000 0000  ................
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -26,39 +26,39 @@
 00000190: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000200: 0000 0000 0000 0000 0000 0007 0000 0003  ................
-00000210: 0073 0072 0063 6277 7370 626c 6f62 0000  .s.r.cbwspblob..
-00000220: 00b8 6270 6c69 7374 3030 d601 0203 0405  ..bplist00......
-00000230: 0607 0807 080b 085d 5368 6f77 5374 6174  .......]ShowStat
-00000240: 7573 4261 725b 5368 6f77 546f 6f6c 6261  usBar[ShowToolba
-00000250: 725b 5368 6f77 5461 6256 6965 775f 1014  r[ShowTabView_..
-00000260: 436f 6e74 6169 6e65 7253 686f 7753 6964  ContainerShowSid
-00000270: 6562 6172 5c57 696e 646f 7742 6f75 6e64  ebar\WindowBound
-00000280: 735b 5368 6f77 5369 6465 6261 7208 0908  s[ShowSidebar...
-00000290: 095f 1018 7b7b 3237 382c 2032 3834 7d2c  ._..{{278, 284},
-000002a0: 207b 3932 302c 2034 3634 7d7d 0908 1523   {920, 464}}...#
-000002b0: 2f3b 525f 6b6c 6d6e 6f8a 0000 0000 0000  /;R_klmno.......
-000002c0: 0101 0000 0000 0000 000d 0000 0000 0000  ................
-000002d0: 0000 0000 0000 0000 008b 0000 0003 0073  ...............s
-000002e0: 0072 0063 6473 636c 626f 6f6c 0000 0000  .r.cdsclbool....
-000002f0: 0300 7300 7200 636c 6731 5363 6f6d 7000  ..s.r.clg1Scomp.
-00000300: 0000 0000 0000 0000 0000 0300 7300 7200  ............s.r.
-00000310: 636d 6f44 4462 6c6f 6200 0000 089c bb0f  cmoDDblob.......
-00000320: 1d22 fcc4 4100 0000 0300 7300 7200 636d  ."..A.....s.r.cm
-00000330: 6f64 4462 6c6f 6200 0000 089c bb0f 1d22  odDblob........"
-00000340: fcc4 4100 0000 0300 7300 7200 6370 6831  ..A.....s.r.cph1
-00000350: 5363 6f6d 7000 0000 0000 0000 0000 0000  Scomp...........
-00000360: 0300 7300 7200 6376 5372 6e6c 6f6e 6700  ..s.r.cvSrnlong.
-00000370: 0000 0100 0000 0000 0000 0000 0000 0000  ................
-00000380: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000200: 0000 0000 0000 0000 0000 0008 0000 0004  ................
+00000210: 0064 0069 0073 0074 6473 636c 626f 6f6c  .d.i.s.tdsclbool
+00000220: 0100 0000 0300 7300 7200 6362 7773 7062  ......s.r.cbwspb
+00000230: 6c6f 6200 0000 b862 706c 6973 7430 30d6  lob....bplist00.
+00000240: 0102 0304 0506 0708 0708 0b08 5d53 686f  ............]Sho
+00000250: 7753 7461 7475 7342 6172 5b53 686f 7754  wStatusBar[ShowT
+00000260: 6f6f 6c62 6172 5b53 686f 7754 6162 5669  oolbar[ShowTabVi
+00000270: 6577 5f10 1443 6f6e 7461 696e 6572 5368  ew_..ContainerSh
+00000280: 6f77 5369 6465 6261 725c 5769 6e64 6f77  owSidebar\Window
+00000290: 426f 756e 6473 5b53 686f 7753 6964 6562  Bounds[ShowSideb
+000002a0: 6172 0809 0809 5f10 187b 7b32 3738 2c20  ar...._..{{278, 
+000002b0: 3238 347d 2c20 7b39 3230 2c20 3436 347d  284}, {920, 464}
+000002c0: 7d09 0815 232f 3b52 5f6b 6c6d 6e6f 8a00  }...#/;R_klmno..
+000002d0: 0000 0000 0001 0100 0000 0000 0000 0d00  ................
+000002e0: 0000 0000 0000 0000 0000 0000 0000 8b00  ................
+000002f0: 0000 0300 7300 7200 6364 7363 6c62 6f6f  ....s.r.cdsclboo
+00000300: 6c00 0000 0003 0073 0072 0063 6c67 3153  l......s.r.clg1S
+00000310: 636f 6d70 0000 0000 0000 0000 0000 0003  comp............
+00000320: 0073 0072 0063 6d6f 4444 626c 6f62 0000  .s.r.cmoDDblob..
+00000330: 0008 9cbb 0f1d 22fc c441 0000 0003 0073  ......"..A.....s
+00000340: 0072 0063 6d6f 6444 626c 6f62 0000 0008  .r.cmodDblob....
+00000350: 9cbb 0f1d 22fc c441 0000 0003 0073 0072  ...."..A.....s.r
+00000360: 0063 7068 3153 636f 6d70 0000 0000 0000  .cph1Scomp......
+00000370: 0000 0000 0003 0073 0072 0063 7653 726e  .......s.r.cvSrn
+00000380: 6c6f 6e67 0000 0001 0000 0000 0000 0000  long............
 00000390: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `pyfed_macos-0.0.4/src/ml_socket.py` & `pyfed_macos-0.0.6/src/pyfed/ml_socket.py`

 * *Files identical despite different names*

### Comparing `pyfed_macos-0.0.4/src/pyfed.py` & `pyfed_macos-0.0.6/src/pyfed/pyfed.py`

 * *Files identical despite different names*

### Comparing `pyfed_macos-0.0.4/.gitignore` & `pyfed_macos-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `pyfed_macos-0.0.4/LICENSE` & `pyfed_macos-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfed_macos-0.0.4/README.md` & `pyfed_macos-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pyfed_macos-0.0.4/pyproject.toml` & `pyfed_macos-0.0.6/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "PyFed_macos"
-version = "0.0.4"
+version = "0.0.6"
 authors = [
   { name="Amirreza Sokhankhosh", email="amirreza.sokhankhosh@gmail.com" },
 ]
 description = "PyFed is an open-source framework for federated learning algorithms." 
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pyfed_macos-0.0.4/PKG-INFO` & `pyfed_macos-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyFed_macos
-Version: 0.0.4
+Version: 0.0.6
 Summary: PyFed is an open-source framework for federated learning algorithms.
 Project-URL: Homepage, https://github.com/amirrezasokhankhosh/PyFed
 Project-URL: Bug Tracker, https://github.com/amirrezasokhankhosh/PyFed/issues
 Author-email: Amirreza Sokhankhosh <amirreza.sokhankhosh@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
```

