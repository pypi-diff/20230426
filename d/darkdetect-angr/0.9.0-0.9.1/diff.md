# Comparing `tmp/darkdetect_angr-0.9.0.tar.gz` & `tmp/darkdetect_angr-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "darkdetect_angr-0.9.0.tar", last modified: Tue Apr 25 22:19:02 2023, max compression
+gzip compressed data, was "darkdetect_angr-0.9.1.tar", last modified: Wed Apr 26 01:27:47 2023, max compression
```

## Comparing `darkdetect_angr-0.9.0.tar` & `darkdetect_angr-0.9.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 zwimer     (501) staff       (20)        0 2023-04-25 22:19:02.466239 darkdetect_angr-0.9.0/
--rw-r--r--   0 zwimer     (501) staff       (20)     1529 2023-04-25 22:14:42.000000 darkdetect_angr-0.9.0/LICENSE
--rw-r--r--   0 zwimer     (501) staff       (20)      196 2023-04-25 21:58:33.000000 darkdetect_angr-0.9.0/MANIFEST.in
--rw-r--r--   0 zwimer     (501) staff       (20)     6067 2023-04-25 22:19:02.466117 darkdetect_angr-0.9.0/PKG-INFO
--rw-r--r--   0 zwimer     (501) staff       (20)     5141 2023-04-25 22:10:31.000000 darkdetect_angr-0.9.0/README.md
-drwxr-xr-x   0 zwimer     (501) staff       (20)        0 2023-04-25 22:19:02.465146 darkdetect_angr-0.9.0/darkdetect/
--rw-r--r--   0 zwimer     (501) staff       (20)     2149 2023-04-25 22:18:44.000000 darkdetect_angr-0.9.0/darkdetect/__init__.py
--rw-r--r--   0 zwimer     (501) staff       (20)      339 2023-04-25 22:15:51.000000 darkdetect_angr-0.9.0/darkdetect/__main__.py
--rw-r--r--   0 zwimer     (501) staff       (20)     4026 2023-04-25 22:06:21.000000 darkdetect_angr-0.9.0/darkdetect/_base_listener.py
--rw-r--r--   0 zwimer     (501) staff       (20)      517 2023-04-25 22:14:26.000000 darkdetect_angr-0.9.0/darkdetect/_dummy.py
--rw-r--r--   0 zwimer     (501) staff       (20)     1905 2023-04-25 22:14:26.000000 darkdetect_angr-0.9.0/darkdetect/_linux_detect.py
--rw-r--r--   0 zwimer     (501) staff       (20)     4468 2023-04-25 22:14:26.000000 darkdetect_angr-0.9.0/darkdetect/_mac_detect.py
--rw-r--r--   0 zwimer     (501) staff       (20)     5259 2023-04-25 22:06:21.000000 darkdetect_angr-0.9.0/darkdetect/_windows_detect.py
--rw-r--r--   0 zwimer     (501) staff       (20)        8 2023-04-25 22:06:21.000000 darkdetect_angr-0.9.0/darkdetect/py.typed
-drwxr-xr-x   0 zwimer     (501) staff       (20)        0 2023-04-25 22:19:02.465963 darkdetect_angr-0.9.0/darkdetect_angr.egg-info/
--rw-r--r--   0 zwimer     (501) staff       (20)     6067 2023-04-25 22:19:02.000000 darkdetect_angr-0.9.0/darkdetect_angr.egg-info/PKG-INFO
--rw-r--r--   0 zwimer     (501) staff       (20)      438 2023-04-25 22:19:02.000000 darkdetect_angr-0.9.0/darkdetect_angr.egg-info/SOURCES.txt
--rw-r--r--   0 zwimer     (501) staff       (20)        1 2023-04-25 22:19:02.000000 darkdetect_angr-0.9.0/darkdetect_angr.egg-info/dependency_links.txt
--rw-r--r--   0 zwimer     (501) staff       (20)       87 2023-04-25 22:19:02.000000 darkdetect_angr-0.9.0/darkdetect_angr.egg-info/requires.txt
--rw-r--r--   0 zwimer     (501) staff       (20)       11 2023-04-25 22:19:02.000000 darkdetect_angr-0.9.0/darkdetect_angr.egg-info/top_level.txt
--rw-r--r--   0 zwimer     (501) staff       (20)     1323 2023-04-25 22:11:56.000000 darkdetect_angr-0.9.0/pyproject.toml
--rw-r--r--   0 zwimer     (501) staff       (20)       38 2023-04-25 22:19:02.466282 darkdetect_angr-0.9.0/setup.cfg
+drwxr-xr-x   0 zwimer     (501) staff       (20)        0 2023-04-26 01:27:47.367440 darkdetect_angr-0.9.1/
+-rw-r--r--   0 zwimer     (501) staff       (20)     1529 2023-04-26 01:13:08.000000 darkdetect_angr-0.9.1/LICENSE
+-rw-r--r--   0 zwimer     (501) staff       (20)      196 2023-04-26 01:13:08.000000 darkdetect_angr-0.9.1/MANIFEST.in
+-rw-r--r--   0 zwimer     (501) staff       (20)     6072 2023-04-26 01:27:47.367311 darkdetect_angr-0.9.1/PKG-INFO
+-rw-r--r--   0 zwimer     (501) staff       (20)     5146 2023-04-26 01:13:08.000000 darkdetect_angr-0.9.1/README.md
+drwxr-xr-x   0 zwimer     (501) staff       (20)        0 2023-04-26 01:27:47.366261 darkdetect_angr-0.9.1/darkdetect/
+-rw-r--r--   0 zwimer     (501) staff       (20)     2149 2023-04-26 01:16:00.000000 darkdetect_angr-0.9.1/darkdetect/__init__.py
+-rw-r--r--   0 zwimer     (501) staff       (20)      339 2023-04-26 01:13:08.000000 darkdetect_angr-0.9.1/darkdetect/__main__.py
+-rw-r--r--   0 zwimer     (501) staff       (20)     4026 2023-04-26 01:13:08.000000 darkdetect_angr-0.9.1/darkdetect/_base_listener.py
+-rw-r--r--   0 zwimer     (501) staff       (20)      517 2023-04-26 01:13:08.000000 darkdetect_angr-0.9.1/darkdetect/_dummy.py
+-rw-r--r--   0 zwimer     (501) staff       (20)     1905 2023-04-26 01:13:08.000000 darkdetect_angr-0.9.1/darkdetect/_linux_detect.py
+-rw-r--r--   0 zwimer     (501) staff       (20)     4723 2023-04-26 01:27:06.000000 darkdetect_angr-0.9.1/darkdetect/_mac_detect.py
+-rw-r--r--   0 zwimer     (501) staff       (20)     5259 2023-04-26 01:13:08.000000 darkdetect_angr-0.9.1/darkdetect/_windows_detect.py
+-rw-r--r--   0 zwimer     (501) staff       (20)        8 2023-04-26 01:13:08.000000 darkdetect_angr-0.9.1/darkdetect/py.typed
+drwxr-xr-x   0 zwimer     (501) staff       (20)        0 2023-04-26 01:27:47.367111 darkdetect_angr-0.9.1/darkdetect_angr.egg-info/
+-rw-r--r--   0 zwimer     (501) staff       (20)     6072 2023-04-26 01:27:47.000000 darkdetect_angr-0.9.1/darkdetect_angr.egg-info/PKG-INFO
+-rw-r--r--   0 zwimer     (501) staff       (20)      438 2023-04-26 01:27:47.000000 darkdetect_angr-0.9.1/darkdetect_angr.egg-info/SOURCES.txt
+-rw-r--r--   0 zwimer     (501) staff       (20)        1 2023-04-26 01:27:47.000000 darkdetect_angr-0.9.1/darkdetect_angr.egg-info/dependency_links.txt
+-rw-r--r--   0 zwimer     (501) staff       (20)       87 2023-04-26 01:27:47.000000 darkdetect_angr-0.9.1/darkdetect_angr.egg-info/requires.txt
+-rw-r--r--   0 zwimer     (501) staff       (20)       11 2023-04-26 01:27:47.000000 darkdetect_angr-0.9.1/darkdetect_angr.egg-info/top_level.txt
+-rw-r--r--   0 zwimer     (501) staff       (20)     1323 2023-04-26 01:13:08.000000 darkdetect_angr-0.9.1/pyproject.toml
+-rw-r--r--   0 zwimer     (501) staff       (20)       38 2023-04-26 01:27:47.367478 darkdetect_angr-0.9.1/setup.cfg
```

### Comparing `darkdetect_angr-0.9.0/LICENSE` & `darkdetect_angr-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `darkdetect_angr-0.9.0/PKG-INFO` & `darkdetect_angr-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: darkdetect_angr
-Version: 0.9.0
+Version: 0.9.1
 Summary: Detect OS Dark Mode from Python
 Author-email: Zachary Wimer <zwimer@gmail.com>
 License: BSD-3-Clause
 Project-URL: homepage, http://github.com/zwimer/darkdetect
 Project-URL: download, http://github.com/zwimer/darkdetect/releases
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: MacOS :: MacOS X
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: macos-listener
 License-File: LICENSE
 
-# Darkdetect
+# Darkdetect-angr
 
 This package allows to detect if the user is using Dark Mode on:
 
 - [macOS 10.14+](https://support.apple.com/en-us/HT208976)
 - [Windows 10 1607+](https://blogs.windows.com/windowsexperience/2016/08/08/windows-10-tip-personalize-your-pc-by-enabling-the-dark-theme/)
 - Linux with [a dark GTK theme](https://www.gnome-look.org/browse/cat/135/ord/rating/?tag=dark).
```

### Comparing `darkdetect_angr-0.9.0/README.md` & `darkdetect_angr-0.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Darkdetect
+# Darkdetect-angr
 
 This package allows to detect if the user is using Dark Mode on:
 
 - [macOS 10.14+](https://support.apple.com/en-us/HT208976)
 - [Windows 10 1607+](https://blogs.windows.com/windowsexperience/2016/08/08/windows-10-tip-personalize-your-pc-by-enabling-the-dark-theme/)
 - Linux with [a dark GTK theme](https://www.gnome-look.org/browse/cat/135/ord/rating/?tag=dark).
```

### Comparing `darkdetect_angr-0.9.0/darkdetect/__init__.py` & `darkdetect_angr-0.9.1/darkdetect/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #-----------------------------------------------------------------------------
 #  Copyright (C) 2019 Alberto Sottile, Zachary Wimer
 #
 #  Distributed under the terms of the 3-clause BSD License.
 #-----------------------------------------------------------------------------
 
-__version__ = '0.9.0'
+__version__ = '0.9.1'
 
 import sys
 import platform
 from typing import Callable, Optional, Type
 
 from ._base_listener import BaseListener
 Listener: Type[BaseListener]
```

### Comparing `darkdetect_angr-0.9.0/darkdetect/_base_listener.py` & `darkdetect_angr-0.9.1/darkdetect/_base_listener.py`

 * *Files identical despite different names*

### Comparing `darkdetect_angr-0.9.0/darkdetect/_dummy.py` & `darkdetect_angr-0.9.1/darkdetect/_dummy.py`

 * *Files identical despite different names*

### Comparing `darkdetect_angr-0.9.0/darkdetect/_linux_detect.py` & `darkdetect_angr-0.9.1/darkdetect/_linux_detect.py`

 * *Files identical despite different names*

### Comparing `darkdetect_angr-0.9.0/darkdetect/_mac_detect.py` & `darkdetect_angr-0.9.1/darkdetect/_mac_detect.py`

 * *Files 5% similar despite different names*

```diff
@@ -82,17 +82,22 @@
     """
     A listener class for macOS
     """
 
     def _listen(self) -> None:
         if not _can_listen:
             raise NotImplementedError("Optional dependencies not found; fix this with: pip install darkdetect[macos-listener]")
-        fix = "from multiprocessing.resource_tracker import main;"
+        cmd = "import darkdetect as d; d.MacListener._listen_child()"
+        if getattr(sys, "frozen", False):
+            # This arrangement allows compatibility with pyinstaller and such (it is what multiprocessing does)
+            args = ("-B", "-s", "-S", "-E","-c", "from multiprocessing.resource_tracker import main;" + cmd)
+        else:
+            args = ("-B", "-c", cmd)
         with subprocess.Popen(
-                (sys.executable, "-c", fix + "import darkdetect as d; d.MacListener._listen_child()"),
+                (sys.executable, *args),
                 stdout=subprocess.PIPE,
                 universal_newlines=True,
                 cwd=Path(__file__).parents[1],
         ) as self._proc:
             for line in self._proc.stdout:
                 self._invoke_callback(line.strip())
```

### Comparing `darkdetect_angr-0.9.0/darkdetect/_windows_detect.py` & `darkdetect_angr-0.9.1/darkdetect/_windows_detect.py`

 * *Files identical despite different names*

### Comparing `darkdetect_angr-0.9.0/darkdetect_angr.egg-info/PKG-INFO` & `darkdetect_angr-0.9.1/darkdetect_angr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: darkdetect-angr
-Version: 0.9.0
+Version: 0.9.1
 Summary: Detect OS Dark Mode from Python
 Author-email: Zachary Wimer <zwimer@gmail.com>
 License: BSD-3-Clause
 Project-URL: homepage, http://github.com/zwimer/darkdetect
 Project-URL: download, http://github.com/zwimer/darkdetect/releases
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: MacOS :: MacOS X
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: macos-listener
 License-File: LICENSE
 
-# Darkdetect
+# Darkdetect-angr
 
 This package allows to detect if the user is using Dark Mode on:
 
 - [macOS 10.14+](https://support.apple.com/en-us/HT208976)
 - [Windows 10 1607+](https://blogs.windows.com/windowsexperience/2016/08/08/windows-10-tip-personalize-your-pc-by-enabling-the-dark-theme/)
 - Linux with [a dark GTK theme](https://www.gnome-look.org/browse/cat/135/ord/rating/?tag=dark).
```

### Comparing `darkdetect_angr-0.9.0/pyproject.toml` & `darkdetect_angr-0.9.1/pyproject.toml`

 * *Files identical despite different names*

