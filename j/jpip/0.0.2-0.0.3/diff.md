# Comparing `tmp/jpip-0.0.2.tar.gz` & `tmp/jpip-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jpip-0.0.2.tar", last modified: Wed Apr 26 14:26:00 2023, max compression
+gzip compressed data, was "jpip-0.0.3.tar", last modified: Wed Apr 26 14:35:16 2023, max compression
```

## Comparing `jpip-0.0.2.tar` & `jpip-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxrwxrwx   0 junichi   (1000) junichi   (1000)        0 2023-04-26 14:26:00.622172 jpip-0.0.2/
--rwxrwxrwx   0 junichi   (1000) junichi   (1000)     1072 2023-04-26 13:40:26.000000 jpip-0.0.2/LICENSE
--rwxrwxrwx   0 junichi   (1000) junichi   (1000)      557 2023-04-26 14:26:00.621988 jpip-0.0.2/PKG-INFO
--rwxrwxrwx   0 junichi   (1000) junichi   (1000)       22 2023-04-26 13:40:26.000000 jpip-0.0.2/README.md
-drwxrwxrwx   0 junichi   (1000) junichi   (1000)        0 2023-04-26 14:26:00.619679 jpip-0.0.2/jpip/
--rwxrwxrwx   0 junichi   (1000) junichi   (1000)       23 2023-04-26 14:15:45.000000 jpip-0.0.2/jpip/__init__.py
--rwxrwxrwx   0 junichi   (1000) junichi   (1000)       33 2023-04-26 14:14:45.000000 jpip-0.0.2/jpip/hello.py
-drwxrwxrwx   0 junichi   (1000) junichi   (1000)        0 2023-04-26 14:26:00.621602 jpip-0.0.2/jpip.egg-info/
--rwxrwxrwx   0 junichi   (1000) junichi   (1000)      557 2023-04-26 14:26:00.000000 jpip-0.0.2/jpip.egg-info/PKG-INFO
--rwxrwxrwx   0 junichi   (1000) junichi   (1000)      196 2023-04-26 14:26:00.000000 jpip-0.0.2/jpip.egg-info/SOURCES.txt
--rwxrwxrwx   0 junichi   (1000) junichi   (1000)        1 2023-04-26 14:26:00.000000 jpip-0.0.2/jpip.egg-info/dependency_links.txt
--rwxrwxrwx   0 junichi   (1000) junichi   (1000)       32 2023-04-26 14:26:00.000000 jpip-0.0.2/jpip.egg-info/requires.txt
--rwxrwxrwx   0 junichi   (1000) junichi   (1000)        5 2023-04-26 14:26:00.000000 jpip-0.0.2/jpip.egg-info/top_level.txt
--rwxrwxrwx   0 junichi   (1000) junichi   (1000)       38 2023-04-26 14:26:00.622253 jpip-0.0.2/setup.cfg
--rwxrwxrwx   0 junichi   (1000) junichi   (1000)      991 2023-04-26 14:25:55.000000 jpip-0.0.2/setup.py
+drwxrwxrwx   0 junichi   (1000) junichi   (1000)        0 2023-04-26 14:35:16.209640 jpip-0.0.3/
+-rwxrwxrwx   0 junichi   (1000) junichi   (1000)     1072 2023-04-26 13:40:26.000000 jpip-0.0.3/LICENSE
+-rwxrwxrwx   0 junichi   (1000) junichi   (1000)      559 2023-04-26 14:35:16.209424 jpip-0.0.3/PKG-INFO
+-rwxrwxrwx   0 junichi   (1000) junichi   (1000)       24 2023-04-26 14:31:56.000000 jpip-0.0.3/README.md
+drwxrwxrwx   0 junichi   (1000) junichi   (1000)        0 2023-04-26 14:35:16.207587 jpip-0.0.3/jpip/
+-rwxrwxrwx   0 junichi   (1000) junichi   (1000)       23 2023-04-26 14:15:45.000000 jpip-0.0.3/jpip/__init__.py
+-rwxrwxrwx   0 junichi   (1000) junichi   (1000)       33 2023-04-26 14:14:45.000000 jpip-0.0.3/jpip/hello.py
+drwxrwxrwx   0 junichi   (1000) junichi   (1000)        0 2023-04-26 14:35:16.208943 jpip-0.0.3/jpip.egg-info/
+-rwxrwxrwx   0 junichi   (1000) junichi   (1000)      559 2023-04-26 14:35:16.000000 jpip-0.0.3/jpip.egg-info/PKG-INFO
+-rwxrwxrwx   0 junichi   (1000) junichi   (1000)      169 2023-04-26 14:35:16.000000 jpip-0.0.3/jpip.egg-info/SOURCES.txt
+-rwxrwxrwx   0 junichi   (1000) junichi   (1000)        1 2023-04-26 14:35:16.000000 jpip-0.0.3/jpip.egg-info/dependency_links.txt
+-rwxrwxrwx   0 junichi   (1000) junichi   (1000)        5 2023-04-26 14:35:16.000000 jpip-0.0.3/jpip.egg-info/top_level.txt
+-rwxrwxrwx   0 junichi   (1000) junichi   (1000)       38 2023-04-26 14:35:16.209726 jpip-0.0.3/setup.cfg
+-rwxrwxrwx   0 junichi   (1000) junichi   (1000)      954 2023-04-26 14:33:59.000000 jpip-0.0.3/setup.py
```

### Comparing `jpip-0.0.2/LICENSE` & `jpip-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jpip-0.0.2/PKG-INFO` & `jpip-0.0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jpip
-Version: 0.0.2
+Version: 0.0.3
 Summary: basic hello package
 Home-page: UNKNOWN
 Author: Junichi Shimizu
 Author-email: jun.shimi51@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
@@ -15,7 +15,9 @@
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # pip-package-template
 
+
+
```

### Comparing `jpip-0.0.2/jpip.egg-info/PKG-INFO` & `jpip-0.0.3/jpip.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jpip
-Version: 0.0.2
+Version: 0.0.3
 Summary: basic hello package
 Home-page: UNKNOWN
 Author: Junichi Shimizu
 Author-email: jun.shimi51@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
@@ -15,7 +15,9 @@
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # pip-package-template
 
+
+
```

### Comparing `jpip-0.0.2/setup.py` & `jpip-0.0.3/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,29 +3,29 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'basic hello package'
 LONG_DESCRIPTION = 'basic hello pacakge'
 
 # Setting up
 setup(
     name="jpip",
     version=VERSION,
     author="Junichi Shimizu",
     author_email="jun.shimi51@gmail.com",
     description=DESCRIPTION,
     packages=find_packages(),
     long_description_content_type="text/markdown",
     long_description=long_description,
-    install_requires=['opencv-python', 'pyautogui', 'pyaudio'],
+    install_requires=[''],
     keywords=[''],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

