# Comparing `tmp/ofrak_type-2.1.0.tar.gz` & `tmp/ofrak_type-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofrak_type-2.1.0.tar", last modified: Tue Jan 24 04:05:31 2023, max compression
+gzip compressed data, was "ofrak_type-2.2.0.tar", last modified: Wed Apr 26 19:02:11 2023, max compression
```

## Comparing `ofrak_type-2.1.0.tar` & `ofrak_type-2.2.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 edward     (501) staff       (20)        0 2023-01-24 04:05:31.497058 ofrak_type-2.1.0/
--rw-r--r--   0 edward     (501) staff       (20)    14321 2022-08-24 21:38:35.000000 ofrak_type-2.1.0/LICENSE
--rw-r--r--   0 edward     (501) staff       (20)     2713 2023-01-24 04:05:31.496714 ofrak_type-2.1.0/PKG-INFO
--rw-r--r--   0 edward     (501) staff       (20)     1808 2023-01-18 23:40:02.000000 ofrak_type-2.1.0/README.md
-drwxr-xr-x   0 edward     (501) staff       (20)        0 2023-01-24 04:05:31.491696 ofrak_type-2.1.0/ofrak_type/
--rw-r--r--   0 edward     (501) staff       (20)      215 2023-01-11 21:57:41.000000 ofrak_type-2.1.0/ofrak_type/__init__.py
--rw-r--r--   0 edward     (501) staff       (20)     4082 2023-01-11 21:57:41.000000 ofrak_type-2.1.0/ofrak_type/architecture.py
--rw-r--r--   0 edward     (501) staff       (20)      273 2022-08-23 19:53:06.000000 ofrak_type-2.1.0/ofrak_type/bit_width.py
--rw-r--r--   0 edward     (501) staff       (20)      299 2022-08-23 19:53:06.000000 ofrak_type-2.1.0/ofrak_type/endianness.py
--rw-r--r--   0 edward     (501) staff       (20)      194 2022-12-02 22:19:26.000000 ofrak_type-2.1.0/ofrak_type/error.py
--rw-r--r--   0 edward     (501) staff       (20)     1831 2022-10-29 00:06:05.000000 ofrak_type-2.1.0/ofrak_type/memory_permissions.py
--rw-r--r--   0 edward     (501) staff       (20)        0 2022-08-23 19:53:06.000000 ofrak_type-2.1.0/ofrak_type/py.typed
--rw-r--r--   0 edward     (501) staff       (20)     7995 2022-11-01 16:30:05.000000 ofrak_type-2.1.0/ofrak_type/range.py
-drwxr-xr-x   0 edward     (501) staff       (20)        0 2023-01-24 04:05:31.493938 ofrak_type-2.1.0/ofrak_type.egg-info/
--rw-r--r--   0 edward     (501) staff       (20)     2713 2023-01-24 04:05:31.000000 ofrak_type-2.1.0/ofrak_type.egg-info/PKG-INFO
--rw-r--r--   0 edward     (501) staff       (20)      556 2023-01-24 04:05:31.000000 ofrak_type-2.1.0/ofrak_type.egg-info/SOURCES.txt
--rw-r--r--   0 edward     (501) staff       (20)        1 2023-01-24 04:05:31.000000 ofrak_type-2.1.0/ofrak_type.egg-info/dependency_links.txt
--rw-r--r--   0 edward     (501) staff       (20)       91 2023-01-24 04:05:31.000000 ofrak_type-2.1.0/ofrak_type.egg-info/requires.txt
--rw-r--r--   0 edward     (501) staff       (20)       27 2023-01-24 04:05:31.000000 ofrak_type-2.1.0/ofrak_type.egg-info/top_level.txt
-drwxr-xr-x   0 edward     (501) staff       (20)        0 2023-01-24 04:05:31.496003 ofrak_type-2.1.0/ofrak_type_test/
--rw-r--r--   0 edward     (501) staff       (20)        0 2022-08-23 19:53:06.000000 ofrak_type-2.1.0/ofrak_type_test/__init__.py
--rw-r--r--   0 edward     (501) staff       (20)      324 2022-08-23 19:53:06.000000 ofrak_type-2.1.0/ofrak_type_test/test_bitwidth.py
--rw-r--r--   0 edward     (501) staff       (20)      373 2022-08-23 19:53:06.000000 ofrak_type-2.1.0/ofrak_type_test/test_endianness.py
--rw-r--r--   0 edward     (501) staff       (20)     1454 2022-08-23 19:53:06.000000 ofrak_type-2.1.0/ofrak_type_test/test_memory_permissions.py
--rw-r--r--   0 edward     (501) staff       (20)     8509 2022-11-01 16:30:05.000000 ofrak_type-2.1.0/ofrak_type_test/test_range.py
--rw-r--r--   0 edward     (501) staff       (20)       38 2023-01-24 04:05:31.497140 ofrak_type-2.1.0/setup.cfg
--rw-r--r--   0 edward     (501) staff       (20)     1973 2023-01-24 04:01:33.000000 ofrak_type-2.1.0/setup.py
+drwxr-xr-x   0 edward     (501) staff       (20)        0 2023-04-26 19:02:11.517385 ofrak_type-2.2.0/
+-rw-r--r--   0 edward     (501) staff       (20)    14321 2022-08-24 21:38:35.000000 ofrak_type-2.2.0/LICENSE
+-rw-r--r--   0 edward     (501) staff       (20)     2713 2023-04-26 19:02:11.516986 ofrak_type-2.2.0/PKG-INFO
+-rw-r--r--   0 edward     (501) staff       (20)     1808 2023-02-02 23:02:32.000000 ofrak_type-2.2.0/README.md
+drwxr-xr-x   0 edward     (501) staff       (20)        0 2023-04-26 19:02:11.507638 ofrak_type-2.2.0/ofrak_type/
+-rw-r--r--   0 edward     (501) staff       (20)      252 2023-03-30 19:29:16.000000 ofrak_type-2.2.0/ofrak_type/__init__.py
+-rw-r--r--   0 edward     (501) staff       (20)     4112 2023-03-30 19:29:24.000000 ofrak_type-2.2.0/ofrak_type/architecture.py
+-rw-r--r--   0 edward     (501) staff       (20)      273 2022-08-23 19:53:06.000000 ofrak_type-2.2.0/ofrak_type/bit_width.py
+-rw-r--r--   0 edward     (501) staff       (20)      299 2022-08-23 19:53:06.000000 ofrak_type-2.2.0/ofrak_type/endianness.py
+-rw-r--r--   0 edward     (501) staff       (20)      194 2022-12-02 22:19:26.000000 ofrak_type-2.2.0/ofrak_type/error.py
+-rw-r--r--   0 edward     (501) staff       (20)     1831 2022-10-29 00:06:05.000000 ofrak_type-2.2.0/ofrak_type/memory_permissions.py
+-rw-r--r--   0 edward     (501) staff       (20)        0 2022-08-23 19:53:06.000000 ofrak_type-2.2.0/ofrak_type/py.typed
+-rw-r--r--   0 edward     (501) staff       (20)     7995 2022-11-01 16:30:05.000000 ofrak_type-2.2.0/ofrak_type/range.py
+-rw-r--r--   0 edward     (501) staff       (20)      116 2023-03-30 19:29:16.000000 ofrak_type-2.2.0/ofrak_type/symbol_type.py
+drwxr-xr-x   0 edward     (501) staff       (20)        0 2023-04-26 19:02:11.512300 ofrak_type-2.2.0/ofrak_type.egg-info/
+-rw-r--r--   0 edward     (501) staff       (20)     2713 2023-04-26 19:02:11.000000 ofrak_type-2.2.0/ofrak_type.egg-info/PKG-INFO
+-rw-r--r--   0 edward     (501) staff       (20)      582 2023-04-26 19:02:11.000000 ofrak_type-2.2.0/ofrak_type.egg-info/SOURCES.txt
+-rw-r--r--   0 edward     (501) staff       (20)        1 2023-04-26 19:02:11.000000 ofrak_type-2.2.0/ofrak_type.egg-info/dependency_links.txt
+-rw-r--r--   0 edward     (501) staff       (20)       91 2023-04-26 19:02:11.000000 ofrak_type-2.2.0/ofrak_type.egg-info/requires.txt
+-rw-r--r--   0 edward     (501) staff       (20)       27 2023-04-26 19:02:11.000000 ofrak_type-2.2.0/ofrak_type.egg-info/top_level.txt
+drwxr-xr-x   0 edward     (501) staff       (20)        0 2023-04-26 19:02:11.516125 ofrak_type-2.2.0/ofrak_type_test/
+-rw-r--r--   0 edward     (501) staff       (20)        0 2022-08-23 19:53:06.000000 ofrak_type-2.2.0/ofrak_type_test/__init__.py
+-rw-r--r--   0 edward     (501) staff       (20)      324 2022-08-23 19:53:06.000000 ofrak_type-2.2.0/ofrak_type_test/test_bitwidth.py
+-rw-r--r--   0 edward     (501) staff       (20)      373 2022-08-23 19:53:06.000000 ofrak_type-2.2.0/ofrak_type_test/test_endianness.py
+-rw-r--r--   0 edward     (501) staff       (20)     1454 2022-08-23 19:53:06.000000 ofrak_type-2.2.0/ofrak_type_test/test_memory_permissions.py
+-rw-r--r--   0 edward     (501) staff       (20)     8509 2022-11-01 16:30:05.000000 ofrak_type-2.2.0/ofrak_type_test/test_range.py
+-rw-r--r--   0 edward     (501) staff       (20)       38 2023-04-26 19:02:11.517515 ofrak_type-2.2.0/setup.cfg
+-rw-r--r--   0 edward     (501) staff       (20)     1973 2023-04-26 17:27:08.000000 ofrak_type-2.2.0/setup.py
```

### Comparing `ofrak_type-2.1.0/LICENSE` & `ofrak_type-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ofrak_type-2.1.0/PKG-INFO` & `ofrak_type-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofrak_type
-Version: 2.1.0
+Version: 2.2.0
 Summary: Custom classes and types used in OFRAK
 Home-page: https://ofrak.com/
 Download-URL: https://github.com/redballoonsecurity/ofrak
 Author: Red Balloon Security
 Author-email: ofrak@redballoonsecurity.com
 License: Proprietary
 Project-URL: Documentation, https://ofrak.com/docs/
```

### Comparing `ofrak_type-2.1.0/README.md` & `ofrak_type-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ofrak_type-2.1.0/ofrak_type/architecture.py` & `ofrak_type-2.2.0/ofrak_type/architecture.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,14 +149,15 @@
     X186_32 = "x186_32"
     I386 = "i386"
     X64 = "x86_64"
     XSCALE = "xscale"
     COLDFIRE4E = "cfv4e"
     CORTEX_A53 = "cortex-a53"
     CORTEX_A55 = "cortex-a55"
+    CORTEX_A72 = "cortex-a72"
     AVR = "avr"
 
 
 @dataclass(frozen=True, eq=True)
 class ArchInfo:
     """
     Collection of fields used to describe an architecture
```

### Comparing `ofrak_type-2.1.0/ofrak_type/memory_permissions.py` & `ofrak_type-2.2.0/ofrak_type/memory_permissions.py`

 * *Files identical despite different names*

### Comparing `ofrak_type-2.1.0/ofrak_type/range.py` & `ofrak_type-2.2.0/ofrak_type/range.py`

 * *Files identical despite different names*

### Comparing `ofrak_type-2.1.0/ofrak_type.egg-info/PKG-INFO` & `ofrak_type-2.2.0/ofrak_type.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofrak-type
-Version: 2.1.0
+Version: 2.2.0
 Summary: Custom classes and types used in OFRAK
 Home-page: https://ofrak.com/
 Download-URL: https://github.com/redballoonsecurity/ofrak
 Author: Red Balloon Security
 Author-email: ofrak@redballoonsecurity.com
 License: Proprietary
 Project-URL: Documentation, https://ofrak.com/docs/
```

### Comparing `ofrak_type-2.1.0/ofrak_type_test/test_memory_permissions.py` & `ofrak_type-2.2.0/ofrak_type_test/test_memory_permissions.py`

 * *Files identical despite different names*

### Comparing `ofrak_type-2.1.0/ofrak_type_test/test_range.py` & `ofrak_type-2.2.0/ofrak_type_test/test_range.py`

 * *Files identical despite different names*

### Comparing `ofrak_type-2.1.0/setup.py` & `ofrak_type-2.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,22 +17,22 @@
 
 with open("README.md") as f:
     long_description = f.read()
 
 
 setuptools.setup(
     name="ofrak_type",
-    version="2.1.0",
+    version="2.2.0",
     description="Custom classes and types used in OFRAK",
     package_data={
         "ofrak_type": ["py.typed"],
     },
     extras_require={
         "test": [
-            "black==22.3.0",
+            "black==22.6.0",
             "fun-coverage==0.2.0",
             "hypothesis~=6.39.3",
             "mypy==0.942",
             "pytest",
             "pytest-cov",
         ]
     },
```

