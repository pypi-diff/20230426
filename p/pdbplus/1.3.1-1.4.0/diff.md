# Comparing `tmp/pdbplus-1.3.1.tar.gz` & `tmp/pdbplus-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdbplus-1.3.1.tar", last modified: Wed Apr 19 18:42:35 2023, max compression
+gzip compressed data, was "pdbplus-1.4.0.tar", last modified: Wed Apr 26 19:54:14 2023, max compression
```

## Comparing `pdbplus-1.3.1.tar` & `pdbplus-1.4.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-04-19 18:42:35.956641 pdbplus-1.3.1/
--rw-r--r--   0 michael    (501) staff       (20)    10435 2023-04-19 18:42:35.955914 pdbplus-1.3.1/PKG-INFO
--rwxr-xr-x   0 michael    (501) staff       (20)     8482 2023-04-19 18:41:19.000000 pdbplus-1.3.1/README.md
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-04-19 18:42:35.955773 pdbplus-1.3.1/pdbplus.egg-info/
--rw-r--r--   0 michael    (501) staff       (20)    10435 2023-04-19 18:42:35.000000 pdbplus-1.3.1/pdbplus.egg-info/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      172 2023-04-19 18:42:35.000000 pdbplus-1.3.1/pdbplus.egg-info/SOURCES.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2023-04-19 18:42:35.000000 pdbplus-1.3.1/pdbplus.egg-info/dependency_links.txt
--rw-r--r--   0 michael    (501) staff       (20)       12 2023-04-19 18:42:35.000000 pdbplus-1.3.1/pdbplus.egg-info/requires.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2023-04-19 18:42:35.000000 pdbplus-1.3.1/pdbplus.egg-info/top_level.txt
--rw-r--r--   0 michael    (501) staff       (20)       38 2023-04-19 18:42:35.956681 pdbplus-1.3.1/setup.cfg
--rwxr-xr-x   0 michael    (501) staff       (20)     4948 2023-04-19 18:41:50.000000 pdbplus-1.3.1/setup.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-04-26 19:54:14.325675 pdbplus-1.4.0/
+-rw-r--r--   0 michael    (501) staff       (20)    10439 2023-04-26 19:54:14.325459 pdbplus-1.4.0/PKG-INFO
+-rwxr-xr-x   0 michael    (501) staff       (20)     8486 2023-04-26 19:16:20.000000 pdbplus-1.4.0/README.md
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-04-26 19:54:14.325242 pdbplus-1.4.0/pdbplus.egg-info/
+-rw-r--r--   0 michael    (501) staff       (20)    10439 2023-04-26 19:54:14.000000 pdbplus-1.4.0/pdbplus.egg-info/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)      172 2023-04-26 19:54:14.000000 pdbplus-1.4.0/pdbplus.egg-info/SOURCES.txt
+-rw-r--r--   0 michael    (501) staff       (20)        1 2023-04-26 19:54:14.000000 pdbplus-1.4.0/pdbplus.egg-info/dependency_links.txt
+-rw-r--r--   0 michael    (501) staff       (20)       12 2023-04-26 19:54:14.000000 pdbplus-1.4.0/pdbplus.egg-info/requires.txt
+-rw-r--r--   0 michael    (501) staff       (20)        1 2023-04-26 19:54:14.000000 pdbplus-1.4.0/pdbplus.egg-info/top_level.txt
+-rw-r--r--   0 michael    (501) staff       (20)       38 2023-04-26 19:54:14.325708 pdbplus-1.4.0/setup.cfg
+-rwxr-xr-x   0 michael    (501) staff       (20)     4948 2023-04-26 16:43:02.000000 pdbplus-1.4.0/setup.py
```

### Comparing `pdbplus-1.3.1/PKG-INFO` & `pdbplus-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdbplus
-Version: 1.3.1
+Version: 1.4.0
 Summary: pdbp (Pdb+): A drop-in replacement for pdb and pdbpp.
 Home-page: https://github.com/mdmintz/pdbp
 Author: Michael Mintz
 Author-email: mdmintz@gmail.com
 Maintainer: Michael Mintz
 License: MIT
 Project-URL: Changelog, https://github.com/mdmintz/pdbp/releases
@@ -47,25 +47,25 @@
 **[<img src="https://img.shields.io/badge/pypi-pdbplus-22AAEE.svg" alt="pypi" />](https://pypi.python.org/pypi/pdbplus) is a proxy for installing [<img src="https://img.shields.io/badge/pypi-pdbp-22AAEE.svg" alt="pypi" />](https://pypi.python.org/pypi/pdbp) (Pdb+).**
 ****
 
 <!-- Pdb+ Docs -->
 
 # pdbp (Pdb+) [![](https://img.shields.io/pypi/v/pdbp.svg)](https://pypi.python.org/pypi/pdbp)
 
-<img width="600" alt="Pdb+ Advanced Python Console Debugger" src="https://user-images.githubusercontent.com/6788579/204896775-38d8551b-1d3c-4e95-9f5c-0e03c9de13da.png">
+<img width="600" alt="Pdb+ Advanced Python Console Debugger" src="https://user-images.githubusercontent.com/6788579/234679015-b1daa50f-94a8-4ef2-b3f5-3157b7a3733b.png">
 
 --------
 
 **[pdbp (Pdb+)](https://github.com/mdmintz/pdbp)** is an advanced console debugger for Python. It can be used as a drop-in replacement for ``pdb`` and [pdbpp](https://github.com/pdbpp/pdbpp).
 
 <p><b>pdbp (Pdb+)</b> makes Python debugging a lot easier (and more fun!)</p>
 
 --------
 
-<img width="600" alt="Pdb+" src="https://user-images.githubusercontent.com/6788579/204408641-9c221bb6-578b-4b0f-807b-8454844e42e8.png">
+<img width="600" alt="Pdb+" src="https://user-images.githubusercontent.com/6788579/234669562-30dae4ad-1207-47e4-8327-fbd5662c8b9c.png">
 
 
 ## Installation & Usage:
 
 ```bash
 pip install pdbp
 ```
@@ -102,17 +102,17 @@
 ```
 
 Here's how to customize **``pdbp``**/``pdb`` options if you don't like the default settings: (<i>Shown below are the default settings.</i>)
 
 ```python
 import pdb
 if hasattr(pdb, "DefaultConfig"):
-    pdb.DefaultConfig.filename_color = pdb.Color.blue
+    pdb.DefaultConfig.filename_color = pdb.Color.fuchsia
     pdb.DefaultConfig.line_number_color = pdb.Color.turquoise
-    pdb.DefaultConfig.truncate_long_lines = True
+    pdb.DefaultConfig.truncate_long_lines = False
     pdb.DefaultConfig.sticky_by_default = True
 ```
 
 You can also trigger **``Pdb+``** activation like this:
 
 ```python
 import pdbp
```

### Comparing `pdbplus-1.3.1/README.md` & `pdbplus-1.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 **[<img src="https://img.shields.io/badge/pypi-pdbplus-22AAEE.svg" alt="pypi" />](https://pypi.python.org/pypi/pdbplus) is a proxy for installing [<img src="https://img.shields.io/badge/pypi-pdbp-22AAEE.svg" alt="pypi" />](https://pypi.python.org/pypi/pdbp) (Pdb+).**
 ****
 
 <!-- Pdb+ Docs -->
 
 # pdbp (Pdb+) [![](https://img.shields.io/pypi/v/pdbp.svg)](https://pypi.python.org/pypi/pdbp)
 
-<img width="600" alt="Pdb+ Advanced Python Console Debugger" src="https://user-images.githubusercontent.com/6788579/204896775-38d8551b-1d3c-4e95-9f5c-0e03c9de13da.png">
+<img width="600" alt="Pdb+ Advanced Python Console Debugger" src="https://user-images.githubusercontent.com/6788579/234679015-b1daa50f-94a8-4ef2-b3f5-3157b7a3733b.png">
 
 --------
 
 **[pdbp (Pdb+)](https://github.com/mdmintz/pdbp)** is an advanced console debugger for Python. It can be used as a drop-in replacement for ``pdb`` and [pdbpp](https://github.com/pdbpp/pdbpp).
 
 <p><b>pdbp (Pdb+)</b> makes Python debugging a lot easier (and more fun!)</p>
 
 --------
 
-<img width="600" alt="Pdb+" src="https://user-images.githubusercontent.com/6788579/204408641-9c221bb6-578b-4b0f-807b-8454844e42e8.png">
+<img width="600" alt="Pdb+" src="https://user-images.githubusercontent.com/6788579/234669562-30dae4ad-1207-47e4-8327-fbd5662c8b9c.png">
 
 
 ## Installation & Usage:
 
 ```bash
 pip install pdbp
 ```
@@ -56,17 +56,17 @@
 ```
 
 Here's how to customize **``pdbp``**/``pdb`` options if you don't like the default settings: (<i>Shown below are the default settings.</i>)
 
 ```python
 import pdb
 if hasattr(pdb, "DefaultConfig"):
-    pdb.DefaultConfig.filename_color = pdb.Color.blue
+    pdb.DefaultConfig.filename_color = pdb.Color.fuchsia
     pdb.DefaultConfig.line_number_color = pdb.Color.turquoise
-    pdb.DefaultConfig.truncate_long_lines = True
+    pdb.DefaultConfig.truncate_long_lines = False
     pdb.DefaultConfig.sticky_by_default = True
 ```
 
 You can also trigger **``Pdb+``** activation like this:
 
 ```python
 import pdbp
```

### Comparing `pdbplus-1.3.1/pdbplus.egg-info/PKG-INFO` & `pdbplus-1.4.0/pdbplus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdbplus
-Version: 1.3.1
+Version: 1.4.0
 Summary: pdbp (Pdb+): A drop-in replacement for pdb and pdbpp.
 Home-page: https://github.com/mdmintz/pdbp
 Author: Michael Mintz
 Author-email: mdmintz@gmail.com
 Maintainer: Michael Mintz
 License: MIT
 Project-URL: Changelog, https://github.com/mdmintz/pdbp/releases
@@ -47,25 +47,25 @@
 **[<img src="https://img.shields.io/badge/pypi-pdbplus-22AAEE.svg" alt="pypi" />](https://pypi.python.org/pypi/pdbplus) is a proxy for installing [<img src="https://img.shields.io/badge/pypi-pdbp-22AAEE.svg" alt="pypi" />](https://pypi.python.org/pypi/pdbp) (Pdb+).**
 ****
 
 <!-- Pdb+ Docs -->
 
 # pdbp (Pdb+) [![](https://img.shields.io/pypi/v/pdbp.svg)](https://pypi.python.org/pypi/pdbp)
 
-<img width="600" alt="Pdb+ Advanced Python Console Debugger" src="https://user-images.githubusercontent.com/6788579/204896775-38d8551b-1d3c-4e95-9f5c-0e03c9de13da.png">
+<img width="600" alt="Pdb+ Advanced Python Console Debugger" src="https://user-images.githubusercontent.com/6788579/234679015-b1daa50f-94a8-4ef2-b3f5-3157b7a3733b.png">
 
 --------
 
 **[pdbp (Pdb+)](https://github.com/mdmintz/pdbp)** is an advanced console debugger for Python. It can be used as a drop-in replacement for ``pdb`` and [pdbpp](https://github.com/pdbpp/pdbpp).
 
 <p><b>pdbp (Pdb+)</b> makes Python debugging a lot easier (and more fun!)</p>
 
 --------
 
-<img width="600" alt="Pdb+" src="https://user-images.githubusercontent.com/6788579/204408641-9c221bb6-578b-4b0f-807b-8454844e42e8.png">
+<img width="600" alt="Pdb+" src="https://user-images.githubusercontent.com/6788579/234669562-30dae4ad-1207-47e4-8327-fbd5662c8b9c.png">
 
 
 ## Installation & Usage:
 
 ```bash
 pip install pdbp
 ```
@@ -102,17 +102,17 @@
 ```
 
 Here's how to customize **``pdbp``**/``pdb`` options if you don't like the default settings: (<i>Shown below are the default settings.</i>)
 
 ```python
 import pdb
 if hasattr(pdb, "DefaultConfig"):
-    pdb.DefaultConfig.filename_color = pdb.Color.blue
+    pdb.DefaultConfig.filename_color = pdb.Color.fuchsia
     pdb.DefaultConfig.line_number_color = pdb.Color.turquoise
-    pdb.DefaultConfig.truncate_long_lines = True
+    pdb.DefaultConfig.truncate_long_lines = False
     pdb.DefaultConfig.sticky_by_default = True
 ```
 
 You can also trigger **``Pdb+``** activation like this:
 
 ```python
 import pdbp
```

### Comparing `pdbplus-1.3.1/setup.py` & `pdbplus-1.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         print("\n*** The Release was PUBLISHED SUCCESSFULLY to PyPI! :) ***\n")
     else:
         print("\n>>> The Release was NOT PUBLISHED to PyPI! <<<\n")
     sys.exit()
 
 setup(
     name='pdbplus',
-    version='1.3.1',
+    version='1.4.0',
     description="pdbp (Pdb+): A drop-in replacement for pdb and pdbpp.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/mdmintz/pdbp",
     project_urls={
         "Changelog": "https://github.com/mdmintz/pdbp/releases",
         "Download": "https://pypi.org/project/pdbp/#files",
@@ -103,14 +103,14 @@
         "Topic :: Software Development :: Libraries",
         "Topic :: Software Development :: Quality Assurance",
         "Topic :: Software Development :: Testing",
         "Topic :: Utilities",
     ],
     python_requires=">=3.6",
     install_requires=[
-        'pdbp>=1.3.1',
+        'pdbp>=1.4.0',
     ],
     setup_requires=[],
     packages=[],
 )
 
 print("\n*** pdbplus Installation Complete! ***\n")
```

