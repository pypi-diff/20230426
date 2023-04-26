# Comparing `tmp/CharacterEncoding-0.0.2.tar.gz` & `tmp/CharacterEncoding-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CharacterEncoding-0.0.2.tar", last modified: Wed Apr 26 16:45:06 2023, max compression
+gzip compressed data, was "CharacterEncoding-0.0.3.tar", last modified: Wed Apr 26 16:47:33 2023, max compression
```

## Comparing `CharacterEncoding-0.0.2.tar` & `CharacterEncoding-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 rishabhchopda   (501) staff       (20)        0 2023-04-26 16:45:06.012258 CharacterEncoding-0.0.2/
--rw-r--r--   0 rishabhchopda   (501) staff       (20)      135 2023-04-26 16:44:27.000000 CharacterEncoding-0.0.2/CHANGELOG.txt
-drwxr-xr-x   0 rishabhchopda   (501) staff       (20)        0 2023-04-26 16:45:06.011135 CharacterEncoding-0.0.2/CharacterEncoding/
--rw-r--r--   0 rishabhchopda   (501) staff       (20)    15100 2023-04-26 16:32:28.000000 CharacterEncoding-0.0.2/CharacterEncoding/__init__.py
-drwxr-xr-x   0 rishabhchopda   (501) staff       (20)        0 2023-04-26 16:45:06.011929 CharacterEncoding-0.0.2/CharacterEncoding.egg-info/
--rw-r--r--   0 rishabhchopda   (501) staff       (20)     3091 2023-04-26 16:45:05.000000 CharacterEncoding-0.0.2/CharacterEncoding.egg-info/PKG-INFO
--rw-r--r--   0 rishabhchopda   (501) staff       (20)      290 2023-04-26 16:45:05.000000 CharacterEncoding-0.0.2/CharacterEncoding.egg-info/SOURCES.txt
--rw-r--r--   0 rishabhchopda   (501) staff       (20)        1 2023-04-26 16:45:05.000000 CharacterEncoding-0.0.2/CharacterEncoding.egg-info/dependency_links.txt
--rw-r--r--   0 rishabhchopda   (501) staff       (20)        5 2023-04-26 16:45:05.000000 CharacterEncoding-0.0.2/CharacterEncoding.egg-info/requires.txt
--rw-r--r--   0 rishabhchopda   (501) staff       (20)       18 2023-04-26 16:45:05.000000 CharacterEncoding-0.0.2/CharacterEncoding.egg-info/top_level.txt
--rw-r--r--   0 rishabhchopda   (501) staff       (20)     1053 2023-04-26 16:24:30.000000 CharacterEncoding-0.0.2/LICENSE.txt
--rw-r--r--   0 rishabhchopda   (501) staff       (20)       25 2022-11-04 03:05:27.000000 CharacterEncoding-0.0.2/MANIFEST.in
--rw-r--r--   0 rishabhchopda   (501) staff       (20)     3091 2023-04-26 16:45:06.012101 CharacterEncoding-0.0.2/PKG-INFO
--rw-r--r--   0 rishabhchopda   (501) staff       (20)     2120 2023-04-26 16:44:24.000000 CharacterEncoding-0.0.2/README.md
--rw-r--r--   0 rishabhchopda   (501) staff       (20)       38 2023-04-26 16:45:06.012323 CharacterEncoding-0.0.2/setup.cfg
--rw-r--r--   0 rishabhchopda   (501) staff       (20)     1118 2023-04-26 16:44:40.000000 CharacterEncoding-0.0.2/setup.py
+drwxr-xr-x   0 rishabhchopda   (501) staff       (20)        0 2023-04-26 16:47:33.060647 CharacterEncoding-0.0.3/
+-rw-r--r--   0 rishabhchopda   (501) staff       (20)      194 2023-04-26 16:47:19.000000 CharacterEncoding-0.0.3/CHANGELOG.txt
+drwxr-xr-x   0 rishabhchopda   (501) staff       (20)        0 2023-04-26 16:47:33.059438 CharacterEncoding-0.0.3/CharacterEncoding/
+-rw-r--r--   0 rishabhchopda   (501) staff       (20)    15100 2023-04-26 16:32:28.000000 CharacterEncoding-0.0.3/CharacterEncoding/__init__.py
+drwxr-xr-x   0 rishabhchopda   (501) staff       (20)        0 2023-04-26 16:47:33.060316 CharacterEncoding-0.0.3/CharacterEncoding.egg-info/
+-rw-r--r--   0 rishabhchopda   (501) staff       (20)     3150 2023-04-26 16:47:32.000000 CharacterEncoding-0.0.3/CharacterEncoding.egg-info/PKG-INFO
+-rw-r--r--   0 rishabhchopda   (501) staff       (20)      290 2023-04-26 16:47:33.000000 CharacterEncoding-0.0.3/CharacterEncoding.egg-info/SOURCES.txt
+-rw-r--r--   0 rishabhchopda   (501) staff       (20)        1 2023-04-26 16:47:32.000000 CharacterEncoding-0.0.3/CharacterEncoding.egg-info/dependency_links.txt
+-rw-r--r--   0 rishabhchopda   (501) staff       (20)        5 2023-04-26 16:47:32.000000 CharacterEncoding-0.0.3/CharacterEncoding.egg-info/requires.txt
+-rw-r--r--   0 rishabhchopda   (501) staff       (20)       18 2023-04-26 16:47:32.000000 CharacterEncoding-0.0.3/CharacterEncoding.egg-info/top_level.txt
+-rw-r--r--   0 rishabhchopda   (501) staff       (20)     1053 2023-04-26 16:24:30.000000 CharacterEncoding-0.0.3/LICENSE.txt
+-rw-r--r--   0 rishabhchopda   (501) staff       (20)       25 2022-11-04 03:05:27.000000 CharacterEncoding-0.0.3/MANIFEST.in
+-rw-r--r--   0 rishabhchopda   (501) staff       (20)     3150 2023-04-26 16:47:33.060488 CharacterEncoding-0.0.3/PKG-INFO
+-rw-r--r--   0 rishabhchopda   (501) staff       (20)     2120 2023-04-26 16:44:24.000000 CharacterEncoding-0.0.3/README.md
+-rw-r--r--   0 rishabhchopda   (501) staff       (20)       38 2023-04-26 16:47:33.060704 CharacterEncoding-0.0.3/setup.cfg
+-rw-r--r--   0 rishabhchopda   (501) staff       (20)     1118 2023-04-26 16:47:23.000000 CharacterEncoding-0.0.3/setup.py
```

### Comparing `CharacterEncoding-0.0.2/CharacterEncoding/__init__.py` & `CharacterEncoding-0.0.3/CharacterEncoding/__init__.py`

 * *Files identical despite different names*

### Comparing `CharacterEncoding-0.0.2/CharacterEncoding.egg-info/PKG-INFO` & `CharacterEncoding-0.0.3/CharacterEncoding.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CharacterEncoding
-Version: 0.0.2
+Version: 0.0.3
 Summary: Character Encoding Algorithms
 Home-page: https://github.com/rishabhc9
 Author: Rishabh Chopda
 Author-email: aaditchopda2@gmail.com
 License: MIT
 Keywords: Encoding,7-Segment Display,ASCII85 Encoding,ASCII Code,Aztec Barcode,Base-32 Crockford,Base32,Base45,Base 58,Base62,Base64,Base91,Baudot,Binary,Chuck Norris Unary Code,EBCDIC Encoding,French Postal Barcode,Gray Code,Morse Code,BCD Encoding,Excess-3 Code (Stibitz),Resistor Value
 Platform: UNKNOWN
@@ -93,17 +93,21 @@
 print('Excess-3 Code (Stibitz) : ' ,CharacterEncoding.encode_excess_3(string))
 print('Resistor Value  : ' ,CharacterEncoding.encode_resistor_value(7979, 10))
 
 ```
 
 Change Log
 ==========
+0.0.3 (26/04/2023)
+-------------------
+- Updated Readme 
+
 0.0.2 (26/04/2023)
 -------------------
 - Updated Readme 
 
 0.0.1 (26/04/2023)
 -------------------
--First Release
+- First Release
```

### Comparing `CharacterEncoding-0.0.2/LICENSE.txt` & `CharacterEncoding-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `CharacterEncoding-0.0.2/PKG-INFO` & `CharacterEncoding-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CharacterEncoding
-Version: 0.0.2
+Version: 0.0.3
 Summary: Character Encoding Algorithms
 Home-page: https://github.com/rishabhc9
 Author: Rishabh Chopda
 Author-email: aaditchopda2@gmail.com
 License: MIT
 Keywords: Encoding,7-Segment Display,ASCII85 Encoding,ASCII Code,Aztec Barcode,Base-32 Crockford,Base32,Base45,Base 58,Base62,Base64,Base91,Baudot,Binary,Chuck Norris Unary Code,EBCDIC Encoding,French Postal Barcode,Gray Code,Morse Code,BCD Encoding,Excess-3 Code (Stibitz),Resistor Value
 Platform: UNKNOWN
@@ -93,17 +93,21 @@
 print('Excess-3 Code (Stibitz) : ' ,CharacterEncoding.encode_excess_3(string))
 print('Resistor Value  : ' ,CharacterEncoding.encode_resistor_value(7979, 10))
 
 ```
 
 Change Log
 ==========
+0.0.3 (26/04/2023)
+-------------------
+- Updated Readme 
+
 0.0.2 (26/04/2023)
 -------------------
 - Updated Readme 
 
 0.0.1 (26/04/2023)
 -------------------
--First Release
+- First Release
```

### Comparing `CharacterEncoding-0.0.2/README.md` & `CharacterEncoding-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `CharacterEncoding-0.0.2/setup.py` & `CharacterEncoding-0.0.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
   'Operating System :: OS Independent',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='CharacterEncoding',
-  version='0.0.2',
+  version='0.0.3',
   description='Character Encoding Algorithms',
   long_description=open('README.md').read() + '\n\n' + open('CHANGELOG.txt').read(),
   long_description_content_type='text/markdown',
   url='https://github.com/rishabhc9',  
   author='Rishabh Chopda',
   author_email='aaditchopda2@gmail.com',
   license='MIT',
```

