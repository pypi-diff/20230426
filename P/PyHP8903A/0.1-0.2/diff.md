# Comparing `tmp/PyHP8903A-0.1.tar.gz` & `tmp/PyHP8903A-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyHP8903A-0.1.tar", last modified: Tue Apr 25 17:53:15 2023, max compression
+gzip compressed data, was "PyHP8903A-0.2.tar", last modified: Tue Apr 25 18:02:21 2023, max compression
```

## Comparing `PyHP8903A-0.1.tar` & `PyHP8903A-0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 17:53:15.282574 PyHP8903A-0.1/
--rw-rw-rw-   0        0        0     1091 2023-01-16 20:41:41.000000 PyHP8903A-0.1/LICENSE
--rw-rw-rw-   0        0        0      326 2023-04-25 17:53:15.281574 PyHP8903A-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-25 17:53:15.271054 PyHP8903A-0.1/PyHP8903A/
--rw-rw-rw-   0        0        0    12189 2023-04-01 13:12:51.000000 PyHP8903A-0.1/PyHP8903A/PyHP8903A.py
--rw-rw-rw-   0        0        0       30 2023-04-25 17:20:45.000000 PyHP8903A-0.1/PyHP8903A/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 17:53:15.280574 PyHP8903A-0.1/PyHP8903A.egg-info/
--rw-rw-rw-   0        0        0      326 2023-04-25 17:53:15.000000 PyHP8903A-0.1/PyHP8903A.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2023-04-25 17:53:15.000000 PyHP8903A-0.1/PyHP8903A.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 17:53:15.000000 PyHP8903A-0.1/PyHP8903A.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-25 17:53:15.000000 PyHP8903A-0.1/PyHP8903A.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-25 17:53:15.000000 PyHP8903A-0.1/PyHP8903A.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      128 2023-04-25 17:24:00.000000 PyHP8903A-0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-25 17:53:15.282574 PyHP8903A-0.1/setup.cfg
--rw-rw-rw-   0        0        0      849 2023-04-25 17:45:43.000000 PyHP8903A-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 18:02:21.853497 PyHP8903A-0.2/
+-rw-rw-rw-   0        0        0     1091 2023-01-16 20:41:41.000000 PyHP8903A-0.2/LICENSE
+-rw-rw-rw-   0        0        0      326 2023-04-25 18:02:21.852496 PyHP8903A-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-25 18:02:21.837960 PyHP8903A-0.2/PyHP8903A/
+-rw-rw-rw-   0        0        0    12181 2023-04-25 18:02:13.000000 PyHP8903A-0.2/PyHP8903A/PyHP8903A.py
+-rw-rw-rw-   0        0        0       30 2023-04-25 17:20:45.000000 PyHP8903A-0.2/PyHP8903A/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 18:02:21.851497 PyHP8903A-0.2/PyHP8903A.egg-info/
+-rw-rw-rw-   0        0        0      326 2023-04-25 18:02:21.000000 PyHP8903A-0.2/PyHP8903A.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2023-04-25 18:02:21.000000 PyHP8903A-0.2/PyHP8903A.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 18:02:21.000000 PyHP8903A-0.2/PyHP8903A.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-25 18:02:21.000000 PyHP8903A-0.2/PyHP8903A.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-25 18:02:21.000000 PyHP8903A-0.2/PyHP8903A.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      128 2023-04-25 17:24:00.000000 PyHP8903A-0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-25 18:02:21.853497 PyHP8903A-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      849 2023-04-25 17:45:43.000000 PyHP8903A-0.2/setup.py
```

### Comparing `PyHP8903A-0.1/LICENSE` & `PyHP8903A-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PyHP8903A-0.1/PyHP8903A/PyHP8903A.py` & `PyHP8903A-0.2/PyHP8903A/PyHP8903A.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 
 class HP8903A:
     """ module for controlling HP8903A from AR488 GPIb to USB adapter
         written by : Manuel Minutello"""
 
-    from PyAR488.PyAR488 import AR488
+    from PyAR488 import AR488
 
     class Trigger:
         class _T:
             def __init__(self, command: str) -> None:
                 self.command = command
 
         free_run = _T('T0')
```

### Comparing `PyHP8903A-0.1/setup.py` & `PyHP8903A-0.2/setup.py`

 * *Files identical despite different names*

