# Comparing `tmp/FlipperNested-1.9.1.tar.gz` & `tmp/FlipperNested-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FlipperNested-1.9.1.tar", last modified: Sun Apr 16 19:06:49 2023, max compression
+gzip compressed data, was "FlipperNested-2.0.1.tar", last modified: Tue Apr 25 18:49:31 2023, max compression
```

## Comparing `FlipperNested-1.9.1.tar` & `FlipperNested-2.0.1.tar`

### file list

```diff
@@ -1,40 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:06:49.841029 FlipperNested-1.9.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:06:49.837029 FlipperNested-1.9.1/FlipperNested/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 19:06:40.000000 FlipperNested-1.9.1/FlipperNested/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-16 19:06:40.000000 FlipperNested-1.9.1/FlipperNested/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6345 2023-04-16 19:06:40.000000 FlipperNested-1.9.1/FlipperNested/bridge.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-16 19:06:40.000000 FlipperNested-1.9.1/FlipperNested/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     9056 2023-04-16 19:06:40.000000 FlipperNested-1.9.1/FlipperNested/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:06:49.837029 FlipperNested-1.9.1/FlipperNested/proto/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 19:06:40.000000 FlipperNested-1.9.1/FlipperNested/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-04-16 19:06:40.000000 FlipperNested-1.9.1/FlipperNested/proto/flipper_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-04-16 19:06:40.000000 FlipperNested-1.9.1/FlipperNested/proto/storage_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:06:49.837029 FlipperNested-1.9.1/FlipperNested.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-04-16 19:06:49.000000 FlipperNested-1.9.1/FlipperNested.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-16 19:06:49.000000 FlipperNested-1.9.1/FlipperNested.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 19:06:49.000000 FlipperNested-1.9.1/FlipperNested.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-16 19:06:49.000000 FlipperNested-1.9.1/FlipperNested.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-16 19:06:49.000000 FlipperNested-1.9.1/FlipperNested.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-16 19:06:49.000000 FlipperNested-1.9.1/FlipperNested.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-16 19:06:40.000000 FlipperNested-1.9.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-16 19:06:40.000000 FlipperNested-1.9.1/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:06:49.841029 FlipperNested-1.9.1/NestedSolver/
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-04-16 19:06:40.000000 FlipperNested-1.9.1/NestedSolver/bucketsort.c
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-16 19:06:40.000000 FlipperNested-1.9.1/NestedSolver/bucketsort.h
--rw-r--r--   0 runner    (1001) docker     (123)    18805 2023-04-16 19:06:40.000000 FlipperNested-1.9.1/NestedSolver/crapto1.c
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-04-16 19:06:40.000000 FlipperNested-1.9.1/NestedSolver/crapto1.h
--rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-04-16 19:06:40.000000 FlipperNested-1.9.1/NestedSolver/crypto1.c
--rw-r--r--   0 runner    (1001) docker     (123)     8716 2023-04-16 19:06:40.000000 FlipperNested-1.9.1/NestedSolver/library.c
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-16 19:06:40.000000 FlipperNested-1.9.1/NestedSolver/library.h
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-04-16 19:06:40.000000 FlipperNested-1.9.1/NestedSolver/parity.h
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-04-16 19:06:40.000000 FlipperNested-1.9.1/NestedSolver/progress.c
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-16 19:06:40.000000 FlipperNested-1.9.1/NestedSolver/progress.h
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-16 19:06:40.000000 FlipperNested-1.9.1/NestedSolver/python.c
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-04-16 19:06:49.841029 FlipperNested-1.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-04-16 19:06:40.000000 FlipperNested-1.9.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 19:06:49.841029 FlipperNested-1.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-16 19:06:40.000000 FlipperNested-1.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:06:49.841029 FlipperNested-1.9.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-16 19:06:40.000000 FlipperNested-1.9.1/tests/test_calculate.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-16 19:06:40.000000 FlipperNested-1.9.1/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-16 19:06:40.000000 FlipperNested-1.9.1/tests/test_parse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:49:31.809728 FlipperNested-2.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:49:31.797727 FlipperNested-2.0.1/FlipperNested/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 18:49:21.000000 FlipperNested-2.0.1/FlipperNested/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-25 18:49:21.000000 FlipperNested-2.0.1/FlipperNested/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6345 2023-04-25 18:49:21.000000 FlipperNested-2.0.1/FlipperNested/bridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-25 18:49:21.000000 FlipperNested-2.0.1/FlipperNested/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12348 2023-04-25 18:49:21.000000 FlipperNested-2.0.1/FlipperNested/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:49:31.797727 FlipperNested-2.0.1/FlipperNested/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 18:49:21.000000 FlipperNested-2.0.1/FlipperNested/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-04-25 18:49:21.000000 FlipperNested-2.0.1/FlipperNested/proto/flipper_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-04-25 18:49:21.000000 FlipperNested-2.0.1/FlipperNested/proto/storage_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:49:31.797727 FlipperNested-2.0.1/FlipperNested.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-04-25 18:49:31.000000 FlipperNested-2.0.1/FlipperNested.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-25 18:49:31.000000 FlipperNested-2.0.1/FlipperNested.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 18:49:31.000000 FlipperNested-2.0.1/FlipperNested.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-25 18:49:31.000000 FlipperNested-2.0.1/FlipperNested.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-25 18:49:31.000000 FlipperNested-2.0.1/FlipperNested.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-25 18:49:31.000000 FlipperNested-2.0.1/FlipperNested.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:49:31.797727 FlipperNested-2.0.1/HardNestedSolver/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2504 2023-04-25 18:49:21.000000 FlipperNested-2.0.1/HardNestedSolver/bucketsort.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)    87569 2023-04-25 18:49:21.000000 FlipperNested-2.0.1/HardNestedSolver/cmdhfmfhard.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18805 2023-04-25 18:49:21.000000 FlipperNested-2.0.1/HardNestedSolver/crapto1.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6561 2023-04-25 18:49:21.000000 FlipperNested-2.0.1/HardNestedSolver/crypto1.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:49:31.797727 FlipperNested-2.0.1/HardNestedSolver/hardnested/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33334 2023-04-25 18:49:21.000000 FlipperNested-2.0.1/HardNestedSolver/hardnested/hardnested_bf_core.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31568 2023-04-25 18:49:21.000000 FlipperNested-2.0.1/HardNestedSolver/hardnested/hardnested_bitarray_core.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20997 2023-04-25 18:49:21.000000 FlipperNested-2.0.1/HardNestedSolver/hardnested/hardnested_bruteforce.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)  5060431 2023-04-25 18:49:21.000000 FlipperNested-2.0.1/HardNestedSolver/hardnested/tables.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)      435 2023-04-25 18:49:21.000000 FlipperNested-2.0.1/HardNestedSolver/library.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:49:31.805727 FlipperNested-2.0.1/HardNestedSolver/pm3/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6876 2023-04-25 18:49:21.000000 FlipperNested-2.0.1/HardNestedSolver/pm3/commonutil.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5824 2023-04-25 18:49:21.000000 FlipperNested-2.0.1/HardNestedSolver/pm3/crc.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10060 2023-04-25 18:49:21.000000 FlipperNested-2.0.1/HardNestedSolver/pm3/crc16.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1686 2023-04-25 18:49:21.000000 FlipperNested-2.0.1/HardNestedSolver/pm3/crc32.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6604 2023-04-25 18:49:21.000000 FlipperNested-2.0.1/HardNestedSolver/pm3/crc64.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)    39500 2023-04-25 18:49:21.000000 FlipperNested-2.0.1/HardNestedSolver/pm3/fileutils.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:49:31.805727 FlipperNested-2.0.1/HardNestedSolver/pm3/uart/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17390 2023-04-25 18:49:21.000000 FlipperNested-2.0.1/HardNestedSolver/pm3/uart/uart_posix.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12654 2023-04-25 18:49:21.000000 FlipperNested-2.0.1/HardNestedSolver/pm3/uart/uart_win32.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24666 2023-04-25 18:49:21.000000 FlipperNested-2.0.1/HardNestedSolver/pm3/ui.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)    35946 2023-04-25 18:49:21.000000 FlipperNested-2.0.1/HardNestedSolver/pm3/util.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4044 2023-04-25 18:49:21.000000 FlipperNested-2.0.1/HardNestedSolver/pm3/util_posix.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)      773 2023-04-25 18:49:21.000000 FlipperNested-2.0.1/HardNestedSolver/python.c
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-25 18:49:21.000000 FlipperNested-2.0.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-25 18:49:21.000000 FlipperNested-2.0.1/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:49:31.809728 FlipperNested-2.0.1/NestedSolver/
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-04-25 18:49:21.000000 FlipperNested-2.0.1/NestedSolver/bucketsort.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-25 18:49:21.000000 FlipperNested-2.0.1/NestedSolver/bucketsort.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18805 2023-04-25 18:49:21.000000 FlipperNested-2.0.1/NestedSolver/crapto1.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-04-25 18:49:21.000000 FlipperNested-2.0.1/NestedSolver/crapto1.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-04-25 18:49:21.000000 FlipperNested-2.0.1/NestedSolver/crypto1.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8716 2023-04-25 18:49:21.000000 FlipperNested-2.0.1/NestedSolver/library.c
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-25 18:49:21.000000 FlipperNested-2.0.1/NestedSolver/library.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-04-25 18:49:21.000000 FlipperNested-2.0.1/NestedSolver/parity.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-04-25 18:49:21.000000 FlipperNested-2.0.1/NestedSolver/progress.c
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-25 18:49:21.000000 FlipperNested-2.0.1/NestedSolver/progress.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-25 18:49:21.000000 FlipperNested-2.0.1/NestedSolver/python.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-04-25 18:49:31.809728 FlipperNested-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-25 18:49:21.000000 FlipperNested-2.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 18:49:31.809728 FlipperNested-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-04-25 18:49:21.000000 FlipperNested-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:49:31.809728 FlipperNested-2.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-25 18:49:21.000000 FlipperNested-2.0.1/tests/test_calculate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-25 18:49:21.000000 FlipperNested-2.0.1/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-25 18:49:21.000000 FlipperNested-2.0.1/tests/test_parse.py
```

### Comparing `FlipperNested-1.9.1/FlipperNested/bridge.py` & `FlipperNested-2.0.1/FlipperNested/bridge.py`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.9.1/FlipperNested/cli.py` & `FlipperNested-2.0.1/FlipperNested/cli.py`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.9.1/FlipperNested/main.py` & `FlipperNested-2.0.1/FlipperNested/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,26 @@
 import _queue
 import re
+import tempfile
 from multiprocessing import Manager, Process
+
 from FlipperNested.bridge import FlipperBridge
 
 
 def wrapper(queue, *args):
     queue.put(FlipperNested.calculate_keys(*args))
 
 
+def wrapper_hard(queue, *args):
+    queue.put(FlipperNested.calculate_keys_hard(*args))
+
+
 class FlipperNested:
-    VERSION = 2
+    VERSION = 3
+    FILE_TYPES = ["Flipper Nested Nonce Manifest File", "Flipper Nested Nonces File"]
     DEPTH_VALUES = {1: 25, 2: 50, 3: 100}
     FLIPPER_PATH = "/ext/nfc/.nested/"
     LEGACY_PATH = "/ext/nfc/nested/"
 
     def __init__(self):
         self.connection = None
         self.filename = None
@@ -37,49 +44,92 @@
         else:
             self.extract_nonces_from_file(args.file)
 
     def parse_file(self, contents):
         self.nonces = {"A": {}, "B": {}}
         self.found_keys = {"A": {}, "B": {}}
         self.bruteforce_distance = [0, 0]
-        lines = contents.splitlines()[1:]
+        lines = contents.splitlines()
+        type_string = lines.pop(0)
+        if "Filetype" not in type_string:
+            print("[!] No type in", self.filename)
+            return False
+        file_type = type_string.split(": ")[1]
+        if file_type.strip() not in self.FILE_TYPES:
+            print("[!] Invalid file type in", self.filename)
+            return False
         version_string = lines.pop(0)
         if "Version" not in version_string:
-            print("No version info in", self.filename)
+            print("[!] No version info in", self.filename)
             return False
         file_version = int(version_string.split(": ")[1])
         if file_version != self.VERSION:
             print("[!!!] Invalid version for", self.filename)
             print("[!] You should update " + ("app" if file_version < self.VERSION else "recovery script"))
             return False
-        if "Nested: Delay" in contents:
-            print("[!] Nested attack with delay was used, will try more PRNG values (will take more time)")
-            result = re.search(r"Nested: Delay [0-9]*, distance ([0-9]*)", contents.strip())
-            print("[?] Please select depth of check")
-            print("[1] Fast: +-25 values")
-            print("[2] Normal: +-50 values")
-            print("[3] Full: +-100 values [Recommended, ~2Gb RAM usage]")
-            print("[-] Custom [..any other value..]")
-            depth = int(input("[1-3/custom] > "))
-            distance = int(result.groups()[0])
-            if depth < 1:
-                print("[!] Invalid input, using Normal depth")
-                depth = 2
-            if depth < 4:
-                self.bruteforce_distance = [distance - self.DEPTH_VALUES[depth], distance + self.DEPTH_VALUES[depth]]
+        lines.pop(0)  # remove note
+        if file_type == "Flipper Nested Nonce Manifest File":
+            if "HardNested" in contents:
+                for line in lines:
+                    values = self.parse_line(line)
+                    sec, key_type = values[-2:]
+                    if sec not in self.nonces[key_type].keys():
+                        self.nonces[key_type][sec] = []
+                    file = tempfile.NamedTemporaryFile(delete=False)
+                    value = self.connection.file_read(values[1])
+                    open(file.name, "wb+").write(b"\n".join(value.split(b"\n")[4:]))
+                    if self.save:
+                        open(values[1].rsplit("/", 1)[1], "wb+").write(value)
+                    values[1] = file.name
+                    self.nonces[key_type][sec].append(values)
+                return len(self.nonces["A"]) + len(self.nonces["B"]) > 0
+            elif "Nested: " in contents:
+                if "Nested: Delay" in contents:
+                    print("[!] Nested attack with delay was used, will try more PRNG values (will take more time)")
+                    result = re.search(r"Nested: Delay [0-9]*, distance ([0-9]*)", contents.strip())
+                    print("[?] Please select depth of check")
+                    print("[1] Fast: +-25 values")
+                    print("[2] Normal: +-50 values")
+                    print("[3] Full: +-100 values [Recommended, ~2Gb RAM usage]")
+                    print("[-] Custom [..any other value..]")
+                    depth = int(input("[1-3/custom] > "))
+                    distance = int(result.groups()[0])
+                    if depth < 1:
+                        print("[!] Invalid input, using Normal depth")
+                        depth = 2
+                    if depth < 4:
+                        self.bruteforce_distance = [distance - self.DEPTH_VALUES[depth],
+                                                    distance + self.DEPTH_VALUES[depth]]
+                    else:
+                        self.bruteforce_distance = [distance - depth, distance + depth]
+                    lines.pop()
+                for line in lines:
+                    values = self.parse_line(line)
+                    sec, key_type = values[-2:]
+                    if sec not in self.nonces[key_type].keys():
+                        self.nonces[key_type][sec] = []
+                    self.nonces[key_type][sec].append(values)
+                return len(self.nonces["A"]) + len(self.nonces["B"]) > 0
             else:
-                self.bruteforce_distance = [distance - depth, distance + depth]
-            lines.pop()
-        for line in lines:
-            values = self.parse_line(line)
+                print("[!] No nonces found")
+                return False
+        elif file_type == "Flipper Nested Nonces File":
+            cuid_string = lines.pop(0)
+            if "cuid 0x" not in cuid_string:
+                print("[!] No cuid in", self.filename)
+                return False
+            file = tempfile.NamedTemporaryFile(delete=False)
+            values = self.parse_line(cuid_string)
             sec, key_type = values[-2:]
-            if not sec in self.nonces[key_type].keys():
+            if sec not in self.nonces[key_type].keys():
                 self.nonces[key_type][sec] = []
+            open(file.name, "w+").write("\n".join(lines))
+            values.insert(1, file.name)
             self.nonces[key_type][sec].append(values)
-        return len(self.nonces["A"]) + len(self.nonces["B"]) > 0
+            return len(self.nonces["A"]) + len(self.nonces["B"]) > 0
 
     def extract_nonces_from_flipper(self):
         self.check_legacy_folder()
         for file in self.connection.get_files(self.FLIPPER_PATH[:-1]):
             if file["name"].endswith(".nonces"):
                 if self.uid:
                     if file["name"].split(".")[0] != self.uid.upper():
@@ -107,33 +157,36 @@
 
     def check_legacy_folder(self):
         files = self.connection.get_files(self.LEGACY_PATH[:-1])
         if len(files):
             print("[!!!] Found files in legacy folder", self.LEGACY_PATH)
             self.connection.mkdir(self.FLIPPER_PATH[:-1])
             for file in files:
-                self.connection.file_rename(self.LEGACY_PATH + file['name'], self.FLIPPER_PATH + file['name'])
+                self.connection.file_rename(self.LEGACY_PATH + file["name"], self.FLIPPER_PATH + file["name"])
             print("[!] Moved {} files to new directory".format(len(files)))
             print("[!] You MUST update app to version 1.1.0 or you won't be able to check keys")
             self.connection.file_delete(self.LEGACY_PATH[:-1])
 
     def recover_keys(self):
         for key_type in self.nonces.keys():
             for sector in self.nonces[key_type].keys():
                 for info in self.nonces[key_type][sector]:
-                    print("[?] Recovering key type", key_type + ", sector", sector)
+                    print("Recovering key type", key_type + ", sector", sector)
                     m = Manager()
                     q = m.Queue()
-
                     value = info[:-2]
-                    value.append(self.bruteforce_distance)
-                    value.append(self.progress_bar)
                     value.insert(0, q)
 
-                    p = Process(target=wrapper, args=value)
+                    if len(value) == 3:
+                        p = Process(target=wrapper_hard, args=value)
+                    else:
+                        value.append(self.bruteforce_distance)
+                        value.append(self.progress_bar)
+                        p = Process(target=wrapper, args=value)
+
                     p.start()
 
                     try:
                         p.join()
                     except KeyboardInterrupt:
                         print("Stopping...")
                         p.kill()
@@ -193,21 +246,31 @@
             if not self.save:
                 open(filename, "w+").write(output)
                 print("[!] Lost connection to Flipper!")
                 print("[?] Saved keys to", filename)
 
     @staticmethod
     def parse_line(line):
-        result = re.search(
-            r"Nested: Key ([A-B]) cuid (0x[0-9a-f]*) nt0 (0x[0-9a-f]*) ks0 (0x[0-9a-f]*) par0 ([0-9a-f]*) nt1 (0x[0-9a-f]*) ks1 (0x[0-9a-f]*) par1 ([0-9a-f]*) sec (\d{1,2})",
-            line.strip())
+        if "HardNested" in line:
+            result = re.search(
+                r"HardNested: Key ([A-B]) cuid (0x[0-9a-f]*) file (\S+) sec (\d{1,2})",
+                line.strip())
+        elif "Nested" in line:
+            result = re.search(
+                r"Nested: Key ([A-B]) cuid (0x[0-9a-f]*) nt0 (0x[0-9a-f]*) ks0 (0x[0-9a-f]*) par0 ([0-9a-f]*) nt1 (0x[0-9a-f]*) ks1 (0x[0-9a-f]*) par1 ([0-9a-f]*) sec (\d{1,2})",
+                line.strip())
+        else:
+            result = re.search(
+                r"Key ([A-B]) cuid (0x[0-9a-f]*) sec (\d{1,2})",
+                line.strip())
         groups = result.groups()
 
         key_type, sec = groups[0], int(groups[-1])
-        values = list(map(lambda x: int(x, 16) if x.startswith("0x") else int(x), groups[1:-1]))
+        values = list(
+            map(lambda x: x if x.startswith("/") else (int(x, 16) if x.startswith("0x") else int(x)), groups[1:-1]))
         values.append(sec)
         values.append(key_type)
         return values
 
     @staticmethod
     def calculate_keys(uid, nt0, ks0, par0, nt1, ks1, par1, bruteforce_distance, progress):
         import faulthandler
@@ -215,7 +278,15 @@
         import nested
         if bruteforce_distance != [0, 0]:
             run = nested.run_full_nested(uid, nt0, ks0, par0, nt1, ks1, par1, bruteforce_distance[0],
                                          bruteforce_distance[1], progress)
         else:
             run = nested.run_nested(uid, nt0, ks0, nt1, ks1)
         return run
+
+    @staticmethod
+    def calculate_keys_hard(uid, filename):
+        import faulthandler
+        faulthandler.enable()
+        import hardnested
+        run = hardnested.run_hardnested(uid, filename)
+        return run
```

### Comparing `FlipperNested-1.9.1/FlipperNested/proto/flipper_pb2.py` & `FlipperNested-2.0.1/FlipperNested/proto/flipper_pb2.py`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.9.1/FlipperNested/proto/storage_pb2.py` & `FlipperNested-2.0.1/FlipperNested/proto/storage_pb2.py`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.9.1/FlipperNested.egg-info/PKG-INFO` & `FlipperNested-2.0.1/FlipperNested.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlipperNested
-Version: 1.9.1
+Version: 2.0.1
 Summary: Recover keys from collected nonces
 Home-page: https://github.com/AloneLiberty/FlipperNestedRecovery
 Author: AloneLiberty
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -15,15 +15,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # Flipper Nested Recovery script
 
 Script recovers keys from collected authorization attempts (nonces).
-You can collect nonces on Flipper Zero with https://github.com/AloneLiberty/FlipperNested
+You can collect nonces on Flipper Zero with [FlipperNested](https://github.com/AloneLiberty/FlipperNested)
 
 #### Flipper Zero should be connected with USB cable and not used by ANY other software (./fbt log, qFlipper, lab.flipper.net)
 
 ## Installation
 
 ```bash
 pip install --upgrade FlipperNested
```

### Comparing `FlipperNested-1.9.1/LICENSE.md` & `FlipperNested-2.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.9.1/NestedSolver/bucketsort.c` & `FlipperNested-2.0.1/HardNestedSolver/bucketsort.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.9.1/NestedSolver/bucketsort.h` & `FlipperNested-2.0.1/NestedSolver/bucketsort.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.9.1/NestedSolver/crapto1.c` & `FlipperNested-2.0.1/HardNestedSolver/crapto1.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.9.1/NestedSolver/crapto1.h` & `FlipperNested-2.0.1/NestedSolver/crapto1.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.9.1/NestedSolver/crypto1.c` & `FlipperNested-2.0.1/HardNestedSolver/crypto1.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.9.1/NestedSolver/library.c` & `FlipperNested-2.0.1/NestedSolver/library.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.9.1/NestedSolver/library.h` & `FlipperNested-2.0.1/NestedSolver/library.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.9.1/NestedSolver/parity.h` & `FlipperNested-2.0.1/NestedSolver/parity.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.9.1/NestedSolver/progress.c` & `FlipperNested-2.0.1/NestedSolver/progress.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.9.1/NestedSolver/python.c` & `FlipperNested-2.0.1/NestedSolver/python.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.9.1/PKG-INFO` & `FlipperNested-2.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlipperNested
-Version: 1.9.1
+Version: 2.0.1
 Summary: Recover keys from collected nonces
 Home-page: https://github.com/AloneLiberty/FlipperNestedRecovery
 Author: AloneLiberty
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -15,15 +15,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # Flipper Nested Recovery script
 
 Script recovers keys from collected authorization attempts (nonces).
-You can collect nonces on Flipper Zero with https://github.com/AloneLiberty/FlipperNested
+You can collect nonces on Flipper Zero with [FlipperNested](https://github.com/AloneLiberty/FlipperNested)
 
 #### Flipper Zero should be connected with USB cable and not used by ANY other software (./fbt log, qFlipper, lab.flipper.net)
 
 ## Installation
 
 ```bash
 pip install --upgrade FlipperNested
```

### Comparing `FlipperNested-1.9.1/README.md` & `FlipperNested-2.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Flipper Nested Recovery script
 
 Script recovers keys from collected authorization attempts (nonces).
-You can collect nonces on Flipper Zero with https://github.com/AloneLiberty/FlipperNested
+You can collect nonces on Flipper Zero with [FlipperNested](https://github.com/AloneLiberty/FlipperNested)
 
 #### Flipper Zero should be connected with USB cable and not used by ANY other software (./fbt log, qFlipper, lab.flipper.net)
 
 ## Installation
 
 ```bash
 pip install --upgrade FlipperNested
```

### Comparing `FlipperNested-1.9.1/tests/test_calculate.py` & `FlipperNested-2.0.1/tests/test_calculate.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,22 @@
+import os.path
+import pathlib
 from FlipperNested.main import FlipperNested
 
 
 def test_calculate():
-    keys = FlipperNested.calculate_keys(0x29c6824a, 0x292daf7a, 0xff3f91be, 1111, 0x48f9f977, 0xffbf94fd, 1100, [0, 0], False)
-    assert keys == 'ffffffffffff;'
+    keys = FlipperNested.calculate_keys(0x29c6824a, 0x292daf7a, 0xff3f91be, 1111, 0x48f9f977, 0xffbf94fd, 1100, [0, 0],
+                                        False)
+    assert keys == "ffffffffffff;"
 
 
 def test_calculate_full():
     keys = FlipperNested.calculate_keys(0x9a22bf95, 0x60011fd9, 0x21098875, 1111, 0xd274da74, 0x6a12a32f, 1111,
                                         [805, 810], False)
-    assert keys == '20b9f1ebffff;9088dcfc2ffe;45baf6bffeff;15f9fefeaffe;ffffffffffff;'
+    assert keys == "20b9f1ebffff;9088dcfc2ffe;45baf6bffeff;15f9fefeaffe;ffffffffffff;"
+
+
+def test_calculate_hard():
+    file = str(pathlib.Path(__file__).parent.resolve()) + "/.clean_nonces"
+    if os.path.isfile(file):
+        keys = FlipperNested.calculate_keys_hard(0x773D6B86, file)
+        assert keys == "89eca97f8c2a;"
```

