# Comparing `tmp/toml_tools-0.10.3-py2.py3-none-any.whl.zip` & `tmp/toml_tools-0.10.4-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 17300 bytes, number of entries: 10
--rw-rw-rw-  2.0 fat      742 b- defN 23-Apr-25 16:28 toml_tools/__init__.py
+Zip file size: 17289 bytes, number of entries: 10
+-rw-rw-rw-  2.0 fat      700 b- defN 23-Apr-25 18:51 toml_tools/__init__.py
 -rw-rw-rw-  2.0 fat    39995 b- defN 23-Apr-25 14:18 toml_tools/decoder.py
--rw-rw-rw-  2.0 fat    11323 b- defN 23-Apr-25 16:29 toml_tools/encoder.py
+-rw-rw-rw-  2.0 fat    11307 b- defN 23-Apr-25 18:49 toml_tools/encoder.py
 -rw-rw-rw-  2.0 fat      363 b- defN 23-Apr-25 14:18 toml_tools/ordered.py
 -rw-rw-rw-  2.0 fat      795 b- defN 23-Apr-25 14:18 toml_tools/tz.py
--rw-rw-rw-  2.0 fat     1278 b- defN 23-Apr-25 16:36 toml_tools-0.10.3.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     7660 b- defN 23-Apr-25 16:36 toml_tools-0.10.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Apr-25 16:36 toml_tools-0.10.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 23-Apr-25 16:36 toml_tools-0.10.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      792 b- defN 23-Apr-25 16:36 toml_tools-0.10.3.dist-info/RECORD
-10 files, 63069 bytes uncompressed, 15958 bytes compressed:  74.7%
+-rw-rw-rw-  2.0 fat     1278 b- defN 23-Apr-25 18:57 toml_tools-0.10.4.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     7698 b- defN 23-Apr-25 18:57 toml_tools-0.10.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Apr-25 18:57 toml_tools-0.10.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 23-Apr-25 18:57 toml_tools-0.10.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      792 b- defN 23-Apr-25 18:57 toml_tools-0.10.4.dist-info/RECORD
+10 files, 63049 bytes uncompressed, 15947 bytes compressed:  74.7%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: toml_tools/ordered.py
 Comment: 
 
 Filename: toml_tools/tz.py
 Comment: 
 
-Filename: toml_tools-0.10.3.dist-info/LICENSE
+Filename: toml_tools-0.10.4.dist-info/LICENSE
 Comment: 
 
-Filename: toml_tools-0.10.3.dist-info/METADATA
+Filename: toml_tools-0.10.4.dist-info/METADATA
 Comment: 
 
-Filename: toml_tools-0.10.3.dist-info/WHEEL
+Filename: toml_tools-0.10.4.dist-info/WHEEL
 Comment: 
 
-Filename: toml_tools-0.10.3.dist-info/top_level.txt
+Filename: toml_tools-0.10.4.dist-info/top_level.txt
 Comment: 
 
-Filename: toml_tools-0.10.3.dist-info/RECORD
+Filename: toml_tools-0.10.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## toml_tools/__init__.py

```diff
@@ -2,16 +2,14 @@
 
 Released under the MIT license.
 """
 
 from . import encoder
 from . import decoder
 
-__version__ = "0.10.3"
-_spec_ = "0.5.0"
 
 load = decoder.load
 loads = decoder.loads
 TomlDecoder = decoder.TomlDecoder
 TomlDecodeError = decoder.TomlDecodeError
 TomlPreserveCommentDecoder = decoder.TomlPreserveCommentDecoder
```

## toml_tools/encoder.py

```diff
@@ -79,26 +79,24 @@
                     retval += addtoretval
             for s in addtosections:
                 newsections[section + "." + s] = addtosections[s]
         sections = newsections
     return retval
 
 
-_Python_escaped_hex = re.compile(r"""  (?P<literal_backslashes>(\\\\)*)   
-                                       (\\x)  # Python Hex escape prefix 
+_Python_escaped_hex = re.compile(r"""(?<!\\) # not preceded by backslashes
+                                     (?P<literal_backslashes>(\\\\)*)   
+                                     (\\x)  # Python Hex escape prefix 
                                               # (used for extended-ASCII 
                                               # chars, e.g. repr('\xad'))
                                   """,
                                  flags = re.VERBOSE)
 
 def _Python_escaped_hex_to_escaped_toml(m):
-    backslashes = m.group('literal_backslashes')
-    if len(backslashes) % 2:
-        return m.group(0)
-    return backslashes + '\\u00' 
+    return m.group('literal_backslashes') + '\\u00' 
 
 
 def _dump_str(v):
     if sys.version_info < (3,) and hasattr(v, 'decode') and isinstance(v, str):
         v = v.decode('utf-8')
     v = "%r" % v
     if v[0] == 'u':
```

## Comparing `toml_tools-0.10.3.dist-info/LICENSE` & `toml_tools-0.10.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `toml_tools-0.10.3.dist-info/METADATA` & `toml_tools-0.10.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toml-tools
-Version: 0.10.3
+Version: 0.10.4
 Summary: A fork of toml, a Python Library for TOML
 Home-page: https://github.com/JamesParrott/toml_tools
 Author: William Pearson, James Parrott
 Author-email: james.parrott@proton.me
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -24,14 +24,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=2.6, !=3.0.*, !=3.1.*, !=3.2.*
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ***************************
 TOML_tools, a fork of TOML.
 ***************************
```

