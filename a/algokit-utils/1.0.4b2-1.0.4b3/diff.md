# Comparing `tmp/algokit_utils-1.0.4b2-py3-none-any.whl.zip` & `tmp/algokit_utils-1.0.4b3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 31270 bytes, number of entries: 14
+Zip file size: 31320 bytes, number of entries: 14
 -rw-r--r--  2.0 unx     3493 b- defN 80-Jan-01 00:00 algokit_utils/__init__.py
 -rw-r--r--  2.0 unx     3568 b- defN 80-Jan-01 00:00 algokit_utils/_transfer.py
 -rw-r--r--  2.0 unx     7709 b- defN 80-Jan-01 00:00 algokit_utils/account.py
 -rw-r--r--  2.0 unx    53906 b- defN 80-Jan-01 00:00 algokit_utils/application_client.py
 -rw-r--r--  2.0 unx     7466 b- defN 80-Jan-01 00:00 algokit_utils/application_specification.py
 -rw-r--r--  2.0 unx    29956 b- defN 80-Jan-01 00:00 algokit_utils/deploy.py
 -rw-r--r--  2.0 unx     1981 b- defN 80-Jan-01 00:00 algokit_utils/logic_error.py
 -rw-r--r--  2.0 unx     3930 b- defN 80-Jan-01 00:00 algokit_utils/models.py
 -rw-r--r--  2.0 unx     3838 b- defN 80-Jan-01 00:00 algokit_utils/network_clients.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 algokit_utils/py.typed
--rw-r--r--  2.0 unx     1076 b- defN 80-Jan-01 00:00 algokit_utils-1.0.4b2.dist-info/LICENSE
--rw-r--r--  2.0 unx     1873 b- defN 80-Jan-01 00:00 algokit_utils-1.0.4b2.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algokit_utils-1.0.4b2.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1175 b- defN 16-Jan-01 00:00 algokit_utils-1.0.4b2.dist-info/RECORD
-14 files, 120059 bytes uncompressed, 29316 bytes compressed:  75.6%
+-rw-r--r--  2.0 unx     1076 b- defN 80-Jan-01 00:00 algokit_utils-1.0.4b3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2037 b- defN 80-Jan-01 00:00 algokit_utils-1.0.4b3.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algokit_utils-1.0.4b3.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1175 b- defN 16-Jan-01 00:00 algokit_utils-1.0.4b3.dist-info/RECORD
+14 files, 120223 bytes uncompressed, 29366 bytes compressed:  75.6%
```

## zipnote {}

```diff
@@ -24,20 +24,20 @@
 
 Filename: algokit_utils/network_clients.py
 Comment: 
 
 Filename: algokit_utils/py.typed
 Comment: 
 
-Filename: algokit_utils-1.0.4b2.dist-info/LICENSE
+Filename: algokit_utils-1.0.4b3.dist-info/LICENSE
 Comment: 
 
-Filename: algokit_utils-1.0.4b2.dist-info/METADATA
+Filename: algokit_utils-1.0.4b3.dist-info/METADATA
 Comment: 
 
-Filename: algokit_utils-1.0.4b2.dist-info/WHEEL
+Filename: algokit_utils-1.0.4b3.dist-info/WHEEL
 Comment: 
 
-Filename: algokit_utils-1.0.4b2.dist-info/RECORD
+Filename: algokit_utils-1.0.4b3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `algokit_utils-1.0.4b2.dist-info/LICENSE` & `algokit_utils-1.0.4b3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `algokit_utils-1.0.4b2.dist-info/METADATA` & `algokit_utils-1.0.4b3.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algokit-utils
-Version: 1.0.4b2
+Version: 1.0.4b3
 Summary: Utilities for Algorand development for use by AlgoKit
 License: MIT
 Author: Algorand Foundation
 Author-email: contact@algorand.foundation
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -20,14 +20,16 @@
 
 The goal of this library is to provide intuitive, productive utility functions that make it easier, quicker and safer to build applications on Algorand. 
 Largely these functions wrap the underlying Algorand SDK, but provide a higher level interface with sensible defaults and capabilities for common tasks.
 
 > **Note**
 > If you prefer TypeScript there's an equivalent [TypeScript utility library](https://github.com/algorandfoundation/algokit-utils-ts).
 
+[Install](https://github.com/algorandfoundation/algokit-utils-py#install) | [Documentation](https://algorandfoundation.github.io/algokit-utils-py/html/index.html)
+
 ## Install
 
 This library can be installed using pip, e.g.:
 
 ```
 pip install algokit-utils
 ```
```

## Comparing `algokit_utils-1.0.4b2.dist-info/RECORD` & `algokit_utils-1.0.4b3.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -4,11 +4,11 @@
 algokit_utils/application_client.py,sha256=3oON9YJ-fU3rFhxacSPNxrpmnHUgG349oMH_Id9NdIA,53906
 algokit_utils/application_specification.py,sha256=XusOe7VrGPun2UoNspC9Ei202NzPkxRNx5USXiABuXc,7466
 algokit_utils/deploy.py,sha256=Vg5K7xDSp7F8ImwT9FyboZDZFHeq_HeZgZyU26lvjE0,29956
 algokit_utils/logic_error.py,sha256=ypu2DSyus-Kjy51_1oE8T3LHVhRSOrc21Gpbau_WjAc,1981
 algokit_utils/models.py,sha256=46vPWFNMowMyNOhmlInq58gVtOg91xgPhQ0w-bIMacw,3930
 algokit_utils/network_clients.py,sha256=N4Xcp3xE2LUXtXIWuWUjQlPRhuGaDTW2gjjio_X45k8,3838
 algokit_utils/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-algokit_utils-1.0.4b2.dist-info/LICENSE,sha256=J5i7U1Q9Q2c7saUzlvFRmrCCFhQyXb5Juz_LO5omNUw,1076
-algokit_utils-1.0.4b2.dist-info/METADATA,sha256=Rt-3nxCk2aKMGVImxVe0-2ixbZ4huUVyPmutVRa1cSo,1873
-algokit_utils-1.0.4b2.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-algokit_utils-1.0.4b2.dist-info/RECORD,,
+algokit_utils-1.0.4b3.dist-info/LICENSE,sha256=J5i7U1Q9Q2c7saUzlvFRmrCCFhQyXb5Juz_LO5omNUw,1076
+algokit_utils-1.0.4b3.dist-info/METADATA,sha256=t81g1kWZe6XgxOq10BCHf2uUntXwk7_2_B_ixhhKqZ8,2037
+algokit_utils-1.0.4b3.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+algokit_utils-1.0.4b3.dist-info/RECORD,,
```

