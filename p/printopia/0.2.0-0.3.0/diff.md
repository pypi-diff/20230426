# Comparing `tmp/printopia-0.2.0.tar.gz` & `tmp/printopia-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "printopia-0.2.0.tar", max compression
+gzip compressed data, was "printopia-0.3.0.tar", max compression
```

## Comparing `printopia-0.2.0.tar` & `printopia-0.3.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      488 2023-04-23 20:35:13.946210 printopia-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1555 2023-04-21 18:12:12.063824 printopia-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-04-23 13:37:52.857957 printopia-0.2.0/src/printopia/__init__.py
--rw-r--r--   0        0        0     4008 2023-04-21 13:38:43.419184 printopia-0.2.0/src/printopia/printopia.py
--rw-r--r--   0        0        0     1831 1970-01-01 00:00:00.000000 printopia-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      496 2023-04-26 19:43:46.274094 printopia-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1555 2023-04-21 18:12:12.063824 printopia-0.3.0/README.md
+-rw-r--r--   0        0        0      293 2023-04-26 19:41:01.878029 printopia-0.3.0/src/printopia/__init__.py
+-rw-r--r--   0        0        0     3959 2023-04-26 20:01:04.922480 printopia-0.3.0/src/printopia/printopia.py
+-rw-r--r--   0        0        0     1935 1970-01-01 00:00:00.000000 printopia-0.3.0/PKG-INFO
```

### Comparing `printopia-0.2.0/README.md` & `printopia-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `printopia-0.2.0/src/printopia/printopia.py` & `printopia-0.3.0/src/printopia/printopia.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     """
 
     print(color, end="")
     print(*args, sep=sep, end="")
     print(Style.RESET_ALL, end=end)
 
 
-def print_error(*args: any, sep: str | None = " ", end: str | None = "\n") -> None:
+def print_error(*args: any, sep: str = " ", end: str = "\n") -> None:
     """
     Prints the given arguments as error message in red color, with the specified separator and ending character.
 
     Parameters
     ----------
     args : tuple
         Arguments to be printed as error message.
@@ -51,15 +51,15 @@
         *args,
         color=Fore.RED,
         sep=sep,
         end=end,
     )
 
 
-def print_log(*args: any, sep: str | None = " ", end: str | None = "\n") -> None:
+def print_log(*args: any, sep: str = " ", end: str = "\n") -> None:
     """
     Prints the given arguments as a log message in yellow color, with the specified separator and ending character.
 
     Parameters
     ----------
     args : tuple
         Arguments to be printed as log message.
@@ -77,15 +77,15 @@
         *args,
         color=Fore.YELLOW,
         sep=sep,
         end=end,
     )
 
 
-def print_success(*args: any, sep: str | None = " ", end: str | None = "\n") -> None:
+def print_success(*args: any, sep=" ", end: str = "\n") -> None:
     """
     Prints the given arguments as success message in green color, with the specified separator and ending character.
 
     Parameters
     ----------
     args : tuple
         Arguments to be printed as success message.
```

### Comparing `printopia-0.2.0/PKG-INFO` & `printopia-0.3.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: printopia
-Version: 0.2.0
+Version: 0.3.0
 Summary: 
 Author: akshat
 Author-email: akshat1997tamrakar@gmail.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.9,<=3.11.3
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Description-Content-Type: text/markdown
 
 <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg?&style=for-the-badge&logo=python&logoColor=blue"></a>
```

