# Comparing `tmp/win-cmd-escaper-0.0.0.tar.gz` & `tmp/win-cmd-escaper-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "win-cmd-escaper-0.0.0.tar", last modified: Wed Apr 26 04:25:41 2023, max compression
+gzip compressed data, was "win-cmd-escaper-1.0.0.tar", last modified: Wed Apr 26 04:39:45 2023, max compression
```

## Comparing `win-cmd-escaper-0.0.0.tar` & `win-cmd-escaper-1.0.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 04:25:41.651649 win-cmd-escaper-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-26 04:25:29.000000 win-cmd-escaper-0.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6446 2023-04-26 04:25:41.651649 win-cmd-escaper-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-04-26 04:25:29.000000 win-cmd-escaper-0.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-26 04:25:41.651649 win-cmd-escaper-0.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-04-26 04:25:29.000000 win-cmd-escaper-0.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 04:25:41.651649 win-cmd-escaper-0.0.0/win_cmd_escaper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6446 2023-04-26 04:25:41.000000 win-cmd-escaper-0.0.0/win_cmd_escaper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-26 04:25:41.000000 win-cmd-escaper-0.0.0/win_cmd_escaper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 04:25:41.000000 win-cmd-escaper-0.0.0/win_cmd_escaper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-26 04:25:41.000000 win-cmd-escaper-0.0.0/win_cmd_escaper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-04-26 04:25:29.000000 win-cmd-escaper-0.0.0/win_cmd_escaper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 04:39:45.053356 win-cmd-escaper-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-26 04:39:34.000000 win-cmd-escaper-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7012 2023-04-26 04:39:45.053356 win-cmd-escaper-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-04-26 04:39:34.000000 win-cmd-escaper-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-26 04:39:45.053356 win-cmd-escaper-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-04-26 04:39:34.000000 win-cmd-escaper-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 04:39:45.053356 win-cmd-escaper-1.0.0/win_cmd_escaper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7012 2023-04-26 04:39:45.000000 win-cmd-escaper-1.0.0/win_cmd_escaper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-26 04:39:45.000000 win-cmd-escaper-1.0.0/win_cmd_escaper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 04:39:45.000000 win-cmd-escaper-1.0.0/win_cmd_escaper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-26 04:39:45.000000 win-cmd-escaper-1.0.0/win_cmd_escaper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-04-26 04:39:34.000000 win-cmd-escaper-1.0.0/win_cmd_escaper.py
```

### Comparing `win-cmd-escaper-0.0.0/LICENSE` & `win-cmd-escaper-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `win-cmd-escaper-0.0.0/PKG-INFO` & `win-cmd-escaper-1.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: win-cmd-escaper
-Version: 0.0.0
+Version: 1.0.0
 Summary: A Python library to properly handle escaping of command line arguments in Windows' CMD.exe and Powershell.
 Home-page: https://github.com/nicolas-van/win-cmd-escaper
 Author: Nicolas Vanhoren
 License: MIT
 Project-URL: Bug Reports, https://github.com/nicolas-van/win-cmd-escaper/issues
 Project-URL: Source, https://github.com/nicolas-van/win-cmd-escaper
 Keywords: windows cmd powershell
@@ -23,18 +23,38 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # win-cmd-escaper
 
-[![Windows Tests](https://github.com/nicolas-van/win-cmd-escaper/actions/workflows/python-app.yml/badge.svg)](https://github.com/nicolas-van/win-cmd-escaper/actions/workflows/python-app.yml)
+[![Windows Tests](https://github.com/nicolas-van/win-cmd-escaper/actions/workflows/python-app.yml/badge.svg)](https://github.com/nicolas-van/win-cmd-escaper/actions/workflows/python-app.yml) [![PyPI](https://img.shields.io/pypi/v/win-cmd-escaper)](https://pypi.org/project/win-cmd-escaper/)
 
 A Python library to properly handle escaping of command line arguments in both Windows' CMD.exe and Powershell.
 
+## Usage
+
+First install with `pip`:
+
+```bash
+pip install win_cmd_escaper
+```
+
+Then import the library and use the functions it provides:
+
+```python
+import win_cmd_escaper
+
+print(win_cmd_escaper.escape_powershell_argument_script("hello world")) # escapes for Powershell
+
+print(win_cmd_escaper.escape_cmd_argument_script("hello world")) # escapes for CMD
+
+print(win_cmd_escaper.escape_cmd_argument_direct("hello world")) # escapes for CMD when using direct calls
+```
+
 ## Rationale
 
 This library was born out of frustration due to the apparent *completely unknown* behavior of CMD and Powershell regarding command line argument parsing. While bash is very well supported on that subject (notably having a [standard Python module](https://docs.python.org/3/library/shlex.html?highlight=shlex#module-shlex) handling both formatting and parsing) that's far from being the case for CMD and Powershell.
 
 Concretely, *no one on earth* seems to have a real understanding of how those things are supposed to work and to have a clean algorithm to format command line arguments in those languages. A huge part of ressources available on Internet are just *wrong* or *lying*, including official documentation from Microsoft. Globally, *all* "smart" formatters you can find on whatever forums *do not work*. Well, to be fair, they usually work "at least a little". But none of them work *all the time*, for *all strings* (which is clearly what any serious programmer expects from a well designed formatter).
 
 Due to the necessity to get the job done with those scripting languages I decided to create a pure *reverse engineering* project to try, as much as possible, to get something that really works in the real world of real things that work for real.
```

### Comparing `win-cmd-escaper-0.0.0/README.md` & `win-cmd-escaper-1.0.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,33 @@
 # win-cmd-escaper
 
-[![Windows Tests](https://github.com/nicolas-van/win-cmd-escaper/actions/workflows/python-app.yml/badge.svg)](https://github.com/nicolas-van/win-cmd-escaper/actions/workflows/python-app.yml)
+[![Windows Tests](https://github.com/nicolas-van/win-cmd-escaper/actions/workflows/python-app.yml/badge.svg)](https://github.com/nicolas-van/win-cmd-escaper/actions/workflows/python-app.yml) [![PyPI](https://img.shields.io/pypi/v/win-cmd-escaper)](https://pypi.org/project/win-cmd-escaper/)
 
 A Python library to properly handle escaping of command line arguments in both Windows' CMD.exe and Powershell.
 
+## Usage
+
+First install with `pip`:
+
+```bash
+pip install win_cmd_escaper
+```
+
+Then import the library and use the functions it provides:
+
+```python
+import win_cmd_escaper
+
+print(win_cmd_escaper.escape_powershell_argument_script("hello world")) # escapes for Powershell
+
+print(win_cmd_escaper.escape_cmd_argument_script("hello world")) # escapes for CMD
+
+print(win_cmd_escaper.escape_cmd_argument_direct("hello world")) # escapes for CMD when using direct calls
+```
+
 ## Rationale
 
 This library was born out of frustration due to the apparent *completely unknown* behavior of CMD and Powershell regarding command line argument parsing. While bash is very well supported on that subject (notably having a [standard Python module](https://docs.python.org/3/library/shlex.html?highlight=shlex#module-shlex) handling both formatting and parsing) that's far from being the case for CMD and Powershell.
 
 Concretely, *no one on earth* seems to have a real understanding of how those things are supposed to work and to have a clean algorithm to format command line arguments in those languages. A huge part of ressources available on Internet are just *wrong* or *lying*, including official documentation from Microsoft. Globally, *all* "smart" formatters you can find on whatever forums *do not work*. Well, to be fair, they usually work "at least a little". But none of them work *all the time*, for *all strings* (which is clearly what any serious programmer expects from a well designed formatter).
 
 Due to the necessity to get the job done with those scripting languages I decided to create a pure *reverse engineering* project to try, as much as possible, to get something that really works in the real world of real things that work for real.
```

### Comparing `win-cmd-escaper-0.0.0/setup.py` & `win-cmd-escaper-1.0.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 here = os.path.dirname(__file__)
 with open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='win-cmd-escaper',
-    version='0.0.0',
+    version='1.0.0',
     license='MIT',
     author="Nicolas Vanhoren",
     description='A Python library to properly handle escaping of command line arguments in Windows\' CMD.exe and Powershell.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     py_modules=["win_cmd_escaper"],
     url='https://github.com/nicolas-van/win-cmd-escaper',
```

### Comparing `win-cmd-escaper-0.0.0/win_cmd_escaper.egg-info/PKG-INFO` & `win-cmd-escaper-1.0.0/win_cmd_escaper.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: win-cmd-escaper
-Version: 0.0.0
+Version: 1.0.0
 Summary: A Python library to properly handle escaping of command line arguments in Windows' CMD.exe and Powershell.
 Home-page: https://github.com/nicolas-van/win-cmd-escaper
 Author: Nicolas Vanhoren
 License: MIT
 Project-URL: Bug Reports, https://github.com/nicolas-van/win-cmd-escaper/issues
 Project-URL: Source, https://github.com/nicolas-van/win-cmd-escaper
 Keywords: windows cmd powershell
@@ -23,18 +23,38 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # win-cmd-escaper
 
-[![Windows Tests](https://github.com/nicolas-van/win-cmd-escaper/actions/workflows/python-app.yml/badge.svg)](https://github.com/nicolas-van/win-cmd-escaper/actions/workflows/python-app.yml)
+[![Windows Tests](https://github.com/nicolas-van/win-cmd-escaper/actions/workflows/python-app.yml/badge.svg)](https://github.com/nicolas-van/win-cmd-escaper/actions/workflows/python-app.yml) [![PyPI](https://img.shields.io/pypi/v/win-cmd-escaper)](https://pypi.org/project/win-cmd-escaper/)
 
 A Python library to properly handle escaping of command line arguments in both Windows' CMD.exe and Powershell.
 
+## Usage
+
+First install with `pip`:
+
+```bash
+pip install win_cmd_escaper
+```
+
+Then import the library and use the functions it provides:
+
+```python
+import win_cmd_escaper
+
+print(win_cmd_escaper.escape_powershell_argument_script("hello world")) # escapes for Powershell
+
+print(win_cmd_escaper.escape_cmd_argument_script("hello world")) # escapes for CMD
+
+print(win_cmd_escaper.escape_cmd_argument_direct("hello world")) # escapes for CMD when using direct calls
+```
+
 ## Rationale
 
 This library was born out of frustration due to the apparent *completely unknown* behavior of CMD and Powershell regarding command line argument parsing. While bash is very well supported on that subject (notably having a [standard Python module](https://docs.python.org/3/library/shlex.html?highlight=shlex#module-shlex) handling both formatting and parsing) that's far from being the case for CMD and Powershell.
 
 Concretely, *no one on earth* seems to have a real understanding of how those things are supposed to work and to have a clean algorithm to format command line arguments in those languages. A huge part of ressources available on Internet are just *wrong* or *lying*, including official documentation from Microsoft. Globally, *all* "smart" formatters you can find on whatever forums *do not work*. Well, to be fair, they usually work "at least a little". But none of them work *all the time*, for *all strings* (which is clearly what any serious programmer expects from a well designed formatter).
 
 Due to the necessity to get the job done with those scripting languages I decided to create a pure *reverse engineering* project to try, as much as possible, to get something that really works in the real world of real things that work for real.
```

### Comparing `win-cmd-escaper-0.0.0/win_cmd_escaper.py` & `win-cmd-escaper-1.0.0/win_cmd_escaper.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+A module to properly handle escaping of command line arguments in Windows' CMD.exe and Powershell. 
+"""
+
 
 def escape_cmd_argument_direct(str):
     """
     Escapes an argument for the CMD command in Windows.
 
     This variant is the one to use when using direct system call invoking CMD on Windows. If
     you are intending to integrate the result of this function in a .bat script you should use
```

