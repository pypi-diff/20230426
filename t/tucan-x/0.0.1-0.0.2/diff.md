# Comparing `tmp/tucan-x-0.0.1.tar.gz` & `tmp/tucan-x-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tucan-x-0.0.1.tar", last modified: Tue Apr 25 23:12:58 2023, max compression
+gzip compressed data, was "tucan-x-0.0.2.tar", last modified: Tue Apr 25 23:19:48 2023, max compression
```

## Comparing `tucan-x-0.0.1.tar` & `tucan-x-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 23:12:58.546218 tucan-x-0.0.1/
--rw-rw-rw-   0        0        0      882 2023-04-25 23:12:58.544220 tucan-x-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       17 2023-04-25 23:09:37.000000 tucan-x-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-25 23:12:58.546218 tucan-x-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     2174 2023-04-25 23:12:43.000000 tucan-x-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-25 23:12:58.543208 tucan-x-0.0.1/tucan_x.egg-info/
--rw-rw-rw-   0        0        0      882 2023-04-25 23:12:58.000000 tucan-x-0.0.1/tucan_x.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      142 2023-04-25 23:12:58.000000 tucan-x-0.0.1/tucan_x.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 23:12:58.000000 tucan-x-0.0.1/tucan_x.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 23:12:58.000000 tucan-x-0.0.1/tucan_x.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-25 23:19:48.620395 tucan-x-0.0.2/
+-rw-rw-rw-   0        0        0      901 2023-04-25 23:19:48.619396 tucan-x-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       36 2023-04-25 23:18:18.000000 tucan-x-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-25 23:19:48.620395 tucan-x-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     2174 2023-04-25 23:19:32.000000 tucan-x-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 23:19:48.618395 tucan-x-0.0.2/tucan_x.egg-info/
+-rw-rw-rw-   0        0        0      901 2023-04-25 23:19:48.000000 tucan-x-0.0.2/tucan_x.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      142 2023-04-25 23:19:48.000000 tucan-x-0.0.2/tucan_x.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 23:19:48.000000 tucan-x-0.0.2/tucan_x.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 23:19:48.000000 tucan-x-0.0.2/tucan_x.egg-info/top_level.txt
```

### Comparing `tucan-x-0.0.1/PKG-INFO` & `tucan-x-0.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: tucan-x
-Version: 0.0.1
+Version: 0.0.2
 Summary: Captcha api wrapper for discord
 Home-page: https://github.com/
 License: GPLv3
-Description: PYTHON FOR ROBLOX
+Description: Discord Wrapper with HCAPTCHA Solver
 Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `tucan-x-0.0.1/setup.py` & `tucan-x-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     def run(self):
         execute()
         install.run(self)
 
 
 setup(
     name='tucan-x',
-    version='0.0.1',
+    version='0.0.2',
     description='Captcha api wrapper for discord',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/',
     packages=[],
     license='GPLv3',
     classifiers=[
```

### Comparing `tucan-x-0.0.1/tucan_x.egg-info/PKG-INFO` & `tucan-x-0.0.2/tucan_x.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: tucan-x
-Version: 0.0.1
+Version: 0.0.2
 Summary: Captcha api wrapper for discord
 Home-page: https://github.com/
 License: GPLv3
-Description: PYTHON FOR ROBLOX
+Description: Discord Wrapper with HCAPTCHA Solver
 Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 2.7
```

