# Comparing `tmp/parseweb-2.tar.gz` & `tmp/parseweb-3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parseweb-2.tar", last modified: Tue Apr 25 22:01:16 2023, max compression
+gzip compressed data, was "parseweb-3.tar", last modified: Tue Apr 25 22:11:26 2023, max compression
```

## Comparing `parseweb-2.tar` & `parseweb-3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 22:01:16.241536 parseweb-2/
--rw-rw-rw-   0        0        0    14723 2023-04-25 22:01:16.242536 parseweb-2/PKG-INFO
--rw-rw-rw-   0        0        0    13715 2023-03-04 16:03:05.000000 parseweb-2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-25 22:01:16.216543 parseweb-2/parseweb/
--rw-rw-rw-   0        0        0       66 2023-04-25 21:54:26.000000 parseweb-2/parseweb/__init__.py
--rw-rw-rw-   0        0        0     4210 2023-04-25 22:00:38.000000 parseweb-2/parseweb/parseweb_file.py
-drwxrwxrwx   0        0        0        0 2023-04-25 22:01:16.240536 parseweb-2/parseweb.egg-info/
--rw-rw-rw-   0        0        0    14723 2023-04-25 22:01:16.000000 parseweb-2/parseweb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2023-04-25 22:01:16.000000 parseweb-2/parseweb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 22:01:16.000000 parseweb-2/parseweb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-25 22:01:16.000000 parseweb-2/parseweb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-25 22:01:16.000000 parseweb-2/parseweb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       43 2023-04-25 22:01:16.245535 parseweb-2/setup.cfg
--rw-rw-rw-   0        0        0     1022 2023-04-25 22:00:52.000000 parseweb-2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 22:11:26.962088 parseweb-3/
+-rw-rw-rw-   0        0        0    14723 2023-04-25 22:11:26.963088 parseweb-3/PKG-INFO
+-rw-rw-rw-   0        0        0    13715 2023-03-04 16:03:05.000000 parseweb-3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-25 22:11:26.937096 parseweb-3/parseweb/
+-rw-rw-rw-   0        0        0       66 2023-04-25 21:54:26.000000 parseweb-3/parseweb/__init__.py
+-rw-rw-rw-   0        0        0     4210 2023-04-25 22:00:38.000000 parseweb-3/parseweb/parseweb_file.py
+drwxrwxrwx   0        0        0        0 2023-04-25 22:11:26.960089 parseweb-3/parseweb.egg-info/
+-rw-rw-rw-   0        0        0    14723 2023-04-25 22:11:26.000000 parseweb-3/parseweb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2023-04-25 22:11:26.000000 parseweb-3/parseweb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 22:11:26.000000 parseweb-3/parseweb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-04-25 22:11:26.000000 parseweb-3/parseweb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-25 22:11:26.000000 parseweb-3/parseweb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       43 2023-04-25 22:11:26.964088 parseweb-3/setup.cfg
+-rw-rw-rw-   0        0        0     1033 2023-04-25 22:10:51.000000 parseweb-3/setup.py
```

### Comparing `parseweb-2/PKG-INFO` & `parseweb-3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parseweb
-Version: 2
+Version: 3
 Summary: Pure-python Colors implementation
 Home-page: https://github.com/tartley/colorama
 Author: Jonathan Hartley
 Author-email: tartley@tartley.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `parseweb-2/README.md` & `parseweb-3/README.md`

 * *Files identical despite different names*

### Comparing `parseweb-2/parseweb/parseweb_file.py` & `parseweb-3/parseweb/parseweb_file.py`

 * *Files identical despite different names*

### Comparing `parseweb-2/parseweb.egg-info/PKG-INFO` & `parseweb-3/parseweb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parseweb
-Version: 2
+Version: 3
 Summary: Pure-python Colors implementation
 Home-page: https://github.com/tartley/colorama
 Author: Jonathan Hartley
 Author-email: tartley@tartley.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `parseweb-2/setup.py` & `parseweb-3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 
 setup(
     name='parseweb',
-    version='2',
+    version='3',
     author='Jonathan Hartley',
     author_email='tartley@tartley.com',
     description='Pure-python Colors implementation',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/tartley/colorama',
     packages=find_packages(),
     install_requires=[
-        'requests'
+        'requests','colorama'
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
```

