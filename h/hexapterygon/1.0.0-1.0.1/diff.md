# Comparing `tmp/hexapterygon-1.0.0.tar.gz` & `tmp/hexapterygon-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hexapterygon-1.0.0.tar", last modified: Wed Apr 26 18:39:44 2023, max compression
+gzip compressed data, was "hexapterygon-1.0.1.tar", last modified: Wed Apr 26 18:54:19 2023, max compression
```

## Comparing `hexapterygon-1.0.0.tar` & `hexapterygon-1.0.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 xou       (1000) xou       (1000)        0 2023-04-26 18:39:44.839481 hexapterygon-1.0.0/
--rw-r--r--   0 xou       (1000) xou       (1000)    35149 2023-04-26 16:34:05.000000 hexapterygon-1.0.0/LICENSE
--rw-r--r--   0 xou       (1000) xou       (1000)      391 2023-04-26 18:39:44.839481 hexapterygon-1.0.0/PKG-INFO
--rw-r--r--   0 xou       (1000) xou       (1000)     6338 2023-04-26 18:32:42.000000 hexapterygon-1.0.0/README.md
-drwxr-xr-x   0 xou       (1000) xou       (1000)        0 2023-04-26 18:39:44.839481 hexapterygon-1.0.0/hexapterygon/
--rw-r--r--   0 xou       (1000) xou       (1000)     1442 2023-04-04 21:25:43.000000 hexapterygon-1.0.0/hexapterygon/DeviceEvents.py
--rw-r--r--   0 xou       (1000) xou       (1000)    10731 2023-04-26 17:01:36.000000 hexapterygon-1.0.0/hexapterygon/DeviceOverlay.py
--rw-r--r--   0 xou       (1000) xou       (1000)      691 2023-04-26 17:13:52.000000 hexapterygon-1.0.0/hexapterygon/HexaGlobals.py
--rw-r--r--   0 xou       (1000) xou       (1000)    14217 2023-04-26 17:43:09.000000 hexapterygon-1.0.0/hexapterygon/HexaTUI.py
--rw-r--r--   0 xou       (1000) xou       (1000)     1506 2023-04-19 11:46:33.000000 hexapterygon-1.0.0/hexapterygon/InsortForOldPython.py
--rw-r--r--   0 xou       (1000) xou       (1000)      324 2023-04-15 09:36:08.000000 hexapterygon-1.0.0/hexapterygon/StateEnums.py
--rw-r--r--   0 xou       (1000) xou       (1000)    17981 2023-04-14 03:20:33.000000 hexapterygon-1.0.0/hexapterygon/TUItilities.py
--rw-r--r--   0 xou       (1000) xou       (1000)     4197 2023-04-24 14:20:12.000000 hexapterygon-1.0.0/hexapterygon/__init__.py
--rw-r--r--   0 xou       (1000) xou       (1000)     2260 2023-04-26 18:36:02.000000 hexapterygon-1.0.0/hexapterygon/__main__.py
-drwxr-xr-x   0 xou       (1000) xou       (1000)        0 2023-04-26 18:39:44.839481 hexapterygon-1.0.0/hexapterygon.egg-info/
--rw-r--r--   0 xou       (1000) xou       (1000)      391 2023-04-26 18:39:44.000000 hexapterygon-1.0.0/hexapterygon.egg-info/PKG-INFO
--rw-r--r--   0 xou       (1000) xou       (1000)      495 2023-04-26 18:39:44.000000 hexapterygon-1.0.0/hexapterygon.egg-info/SOURCES.txt
--rw-r--r--   0 xou       (1000) xou       (1000)        1 2023-04-26 18:39:44.000000 hexapterygon-1.0.0/hexapterygon.egg-info/dependency_links.txt
--rw-r--r--   0 xou       (1000) xou       (1000)       60 2023-04-26 18:39:44.000000 hexapterygon-1.0.0/hexapterygon.egg-info/entry_points.txt
--rw-r--r--   0 xou       (1000) xou       (1000)       36 2023-04-26 18:39:44.000000 hexapterygon-1.0.0/hexapterygon.egg-info/requires.txt
--rw-r--r--   0 xou       (1000) xou       (1000)       13 2023-04-26 18:39:44.000000 hexapterygon-1.0.0/hexapterygon.egg-info/top_level.txt
--rw-r--r--   0 xou       (1000) xou       (1000)       38 2023-04-26 18:39:44.839481 hexapterygon-1.0.0/setup.cfg
--rw-r--r--   0 xou       (1000) xou       (1000)      962 2023-04-26 18:38:32.000000 hexapterygon-1.0.0/setup.py
+drwxr-xr-x   0 xou       (1000) xou       (1000)        0 2023-04-26 18:54:19.057233 hexapterygon-1.0.1/
+-rw-r--r--   0 xou       (1000) xou       (1000)    35149 2023-04-26 16:34:05.000000 hexapterygon-1.0.1/LICENSE
+-rw-r--r--   0 xou       (1000) xou       (1000)      391 2023-04-26 18:54:19.057233 hexapterygon-1.0.1/PKG-INFO
+-rw-r--r--   0 xou       (1000) xou       (1000)     6338 2023-04-26 18:32:42.000000 hexapterygon-1.0.1/README.md
+drwxr-xr-x   0 xou       (1000) xou       (1000)        0 2023-04-26 18:54:19.057233 hexapterygon-1.0.1/hexapterygon/
+-rw-r--r--   0 xou       (1000) xou       (1000)     1442 2023-04-04 21:25:43.000000 hexapterygon-1.0.1/hexapterygon/DeviceEvents.py
+-rw-r--r--   0 xou       (1000) xou       (1000)    10731 2023-04-26 18:51:30.000000 hexapterygon-1.0.1/hexapterygon/DeviceOverlay.py
+-rw-r--r--   0 xou       (1000) xou       (1000)      691 2023-04-26 17:13:52.000000 hexapterygon-1.0.1/hexapterygon/HexaGlobals.py
+-rw-r--r--   0 xou       (1000) xou       (1000)    14230 2023-04-26 18:52:35.000000 hexapterygon-1.0.1/hexapterygon/HexaTUI.py
+-rw-r--r--   0 xou       (1000) xou       (1000)     1506 2023-04-19 11:46:33.000000 hexapterygon-1.0.1/hexapterygon/InsortForOldPython.py
+-rw-r--r--   0 xou       (1000) xou       (1000)      324 2023-04-15 09:36:08.000000 hexapterygon-1.0.1/hexapterygon/StateEnums.py
+-rw-r--r--   0 xou       (1000) xou       (1000)    17981 2023-04-14 03:20:33.000000 hexapterygon-1.0.1/hexapterygon/TUItilities.py
+-rw-r--r--   0 xou       (1000) xou       (1000)     4209 2023-04-26 18:51:34.000000 hexapterygon-1.0.1/hexapterygon/__init__.py
+-rw-r--r--   0 xou       (1000) xou       (1000)     2260 2023-04-26 18:36:02.000000 hexapterygon-1.0.1/hexapterygon/__main__.py
+drwxr-xr-x   0 xou       (1000) xou       (1000)        0 2023-04-26 18:54:19.057233 hexapterygon-1.0.1/hexapterygon.egg-info/
+-rw-r--r--   0 xou       (1000) xou       (1000)      391 2023-04-26 18:54:18.000000 hexapterygon-1.0.1/hexapterygon.egg-info/PKG-INFO
+-rw-r--r--   0 xou       (1000) xou       (1000)      495 2023-04-26 18:54:19.000000 hexapterygon-1.0.1/hexapterygon.egg-info/SOURCES.txt
+-rw-r--r--   0 xou       (1000) xou       (1000)        1 2023-04-26 18:54:18.000000 hexapterygon-1.0.1/hexapterygon.egg-info/dependency_links.txt
+-rw-r--r--   0 xou       (1000) xou       (1000)       60 2023-04-26 18:54:18.000000 hexapterygon-1.0.1/hexapterygon.egg-info/entry_points.txt
+-rw-r--r--   0 xou       (1000) xou       (1000)       36 2023-04-26 18:54:18.000000 hexapterygon-1.0.1/hexapterygon.egg-info/requires.txt
+-rw-r--r--   0 xou       (1000) xou       (1000)       13 2023-04-26 18:54:18.000000 hexapterygon-1.0.1/hexapterygon.egg-info/top_level.txt
+-rw-r--r--   0 xou       (1000) xou       (1000)       38 2023-04-26 18:54:19.057233 hexapterygon-1.0.1/setup.cfg
+-rw-r--r--   0 xou       (1000) xou       (1000)      962 2023-04-26 18:44:39.000000 hexapterygon-1.0.1/setup.py
```

### Comparing `hexapterygon-1.0.0/LICENSE` & `hexapterygon-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hexapterygon-1.0.0/README.md` & `hexapterygon-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `hexapterygon-1.0.0/hexapterygon/DeviceEvents.py` & `hexapterygon-1.0.1/hexapterygon/DeviceEvents.py`

 * *Files identical despite different names*

### Comparing `hexapterygon-1.0.0/hexapterygon/DeviceOverlay.py` & `hexapterygon-1.0.1/hexapterygon/DeviceOverlay.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from   ppadb                  import InstallError
 from   os.path                import isfile, basename, exists, isdir, sep
 from   github.GithubException import UnknownObjectException
 from   .StateEnums            import DownloadState, InstallState, UninstallState
 from   ppadb.device           import Device
 from   .DeviceEvents          import DeviceEvents
 from   sys                    import version_info
-import HexaGlobals          as     g
+import hexapterygon.HexaGlobals as g
 import requests
 
 if version_info >= (3,10): # because i think it has a C implementation too (from _bisect import *)
     from bisect import insort_left
 else:
     from .InsortForOldPython import insort_left
```

### Comparing `hexapterygon-1.0.0/hexapterygon/HexaGlobals.py` & `hexapterygon-1.0.1/hexapterygon/HexaGlobals.py`

 * *Files identical despite different names*

### Comparing `hexapterygon-1.0.0/hexapterygon/HexaTUI.py` & `hexapterygon-1.0.1/hexapterygon/HexaTUI.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import unicurses as uc
 
 from .StateEnums import DownloadState, InstallState, UninstallState
 from .TUItilities import Border, Highlight, Label, TextBox, Parent
 from time import sleep
 import re
 import threading
-import HexaGlobals as g
+import hexapterygon.HexaGlobals as g
 
 
 class HexaTUI(Parent): # And a Component that can be used stand alone as it is with a uni-curses project | uni-curses compatible component
 
     def on_debloat(self, instruction, comment):
         self.comment = comment
```

### Comparing `hexapterygon-1.0.0/hexapterygon/InsortForOldPython.py` & `hexapterygon-1.0.1/hexapterygon/InsortForOldPython.py`

 * *Files identical despite different names*

### Comparing `hexapterygon-1.0.0/hexapterygon/TUItilities.py` & `hexapterygon-1.0.1/hexapterygon/TUItilities.py`

 * *Files identical despite different names*

### Comparing `hexapterygon-1.0.0/hexapterygon/__init__.py` & `hexapterygon-1.0.1/hexapterygon/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from subprocess     import Popen, PIPE 
 from ppadb.client   import Client as AdbClient
 from os             import makedirs
 from .DeviceEvents  import DeviceEvents
 from .DeviceOverlay import DeviceOverlay
 from github         import Github
-import HexaGlobals  as g
+import hexapterygon.HexaGlobals as g
 from shutil import rmtree
 
 
 
-__version__ = '1.0.0'
+__version__ = '1.0.1'
 def get_global_server_repo(): return g.SERVER_REPO
 def set_global_server_repo(value): g.SERVER_REPO = value
 def set_github_token      (value): g.GIT         = Github(login_or_token=value)
 
 
 
 class Hexapterygon(DeviceEvents): # TODO: restore via cmd package install-existing <package>
```

### Comparing `hexapterygon-1.0.0/hexapterygon/__main__.py` & `hexapterygon-1.0.1/hexapterygon/__main__.py`

 * *Files identical despite different names*

### Comparing `hexapterygon-1.0.0/setup.py` & `hexapterygon-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #def readfile(filename):
 #    with open(filename, 'r+') as f:
 #        return f.read()
 
 
 setup(
     name="hexapterygon",
-    version="1.0.0",
+    version="1.0.1",
     description="A user-friendly all-in-one cross-platform, (uni-curses compatible component, module and uitility) software for orchestrating and debloating your Android devices from unwanted pre-installed crap.",
     #long_description=readfile('README.md'),
     author="George Chousos",
     author_email="gxousos@gmail.com",
     url="https://github.com/GiorgosXou/hexapterygon",
     packages=['hexapterygon'],
     install_requires=['uni-curses', 'pure-python-adb', 'PyGithub'],
```

