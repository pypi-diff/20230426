# Comparing `tmp/py_common_fetch-0.342.tar.gz` & `tmp/py_common_fetch-0.352.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_common_fetch-0.342.tar", last modified: Mon Mar 13 15:46:59 2023, max compression
+gzip compressed data, was "py_common_fetch-0.352.tar", last modified: Wed Apr 26 16:56:15 2023, max compression
```

## Comparing `py_common_fetch-0.342.tar` & `py_common_fetch-0.352.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 greg       (501) staff       (20)        0 2023-03-13 15:46:59.356586 py_common_fetch-0.342/
--rw-r--r--   0 greg       (501) staff       (20)     1535 2023-03-13 15:46:59.356085 py_common_fetch-0.342/PKG-INFO
--rw-r--r--   0 greg       (501) staff       (20)     1200 2018-05-11 19:03:10.000000 py_common_fetch-0.342/README.md
-drwxr-xr-x   0 greg       (501) staff       (20)        0 2023-03-13 15:46:59.350153 py_common_fetch-0.342/aniachi/
--rw-r--r--   0 greg       (501) staff       (20)        0 2017-03-03 18:42:55.000000 py_common_fetch-0.342/aniachi/__init__.py
--rw-r--r--   0 greg       (501) staff       (20)     4435 2023-03-13 15:46:03.000000 py_common_fetch-0.342/aniachi/stringUtils.py
--rw-r--r--   0 greg       (501) staff       (20)    10495 2022-12-28 14:08:55.000000 py_common_fetch-0.342/aniachi/systemUtils.py
--rw-r--r--   0 greg       (501) staff       (20)     1291 2022-12-28 13:57:20.000000 py_common_fetch-0.342/aniachi/timeUtils.py
-drwxr-xr-x   0 greg       (501) staff       (20)        0 2023-03-13 15:46:59.355533 py_common_fetch-0.342/py_common_fetch.egg-info/
--rw-r--r--   0 greg       (501) staff       (20)     1535 2023-03-13 15:46:59.000000 py_common_fetch-0.342/py_common_fetch.egg-info/PKG-INFO
--rw-r--r--   0 greg       (501) staff       (20)      337 2023-03-13 15:46:59.000000 py_common_fetch-0.342/py_common_fetch.egg-info/SOURCES.txt
--rw-r--r--   0 greg       (501) staff       (20)        1 2023-03-13 15:46:59.000000 py_common_fetch-0.342/py_common_fetch.egg-info/dependency_links.txt
--rw-r--r--   0 greg       (501) staff       (20)        1 2018-05-11 03:32:51.000000 py_common_fetch-0.342/py_common_fetch.egg-info/not-zip-safe
--rw-r--r--   0 greg       (501) staff       (20)       64 2023-03-13 15:46:59.000000 py_common_fetch-0.342/py_common_fetch.egg-info/requires.txt
--rw-r--r--   0 greg       (501) staff       (20)        8 2023-03-13 15:46:59.000000 py_common_fetch-0.342/py_common_fetch.egg-info/top_level.txt
--rw-r--r--   0 greg       (501) staff       (20)       38 2023-03-13 15:46:59.356753 py_common_fetch-0.342/setup.cfg
--rw-r--r--   0 greg       (501) staff       (20)      987 2023-03-13 15:46:30.000000 py_common_fetch-0.342/setup.py
+drwxr-xr-x   0 greg       (501) staff       (20)        0 2023-04-26 16:56:15.548262 py_common_fetch-0.352/
+-rw-r--r--   0 greg       (501) staff       (20)     1535 2023-04-26 16:56:15.548132 py_common_fetch-0.352/PKG-INFO
+-rw-r--r--   0 greg       (501) staff       (20)     1200 2018-05-11 19:03:10.000000 py_common_fetch-0.352/README.md
+drwxr-xr-x   0 greg       (501) staff       (20)        0 2023-04-26 16:56:15.544474 py_common_fetch-0.352/aniachi/
+-rw-r--r--   0 greg       (501) staff       (20)        0 2017-03-03 18:42:55.000000 py_common_fetch-0.352/aniachi/__init__.py
+-rw-r--r--   0 greg       (501) staff       (20)     4500 2023-04-26 16:55:23.000000 py_common_fetch-0.352/aniachi/stringUtils.py
+-rw-r--r--   0 greg       (501) staff       (20)    10495 2022-12-28 14:08:55.000000 py_common_fetch-0.352/aniachi/systemUtils.py
+-rw-r--r--   0 greg       (501) staff       (20)     1291 2022-12-28 13:57:20.000000 py_common_fetch-0.352/aniachi/timeUtils.py
+drwxr-xr-x   0 greg       (501) staff       (20)        0 2023-04-26 16:56:15.547914 py_common_fetch-0.352/py_common_fetch.egg-info/
+-rw-r--r--   0 greg       (501) staff       (20)     1535 2023-04-26 16:56:15.000000 py_common_fetch-0.352/py_common_fetch.egg-info/PKG-INFO
+-rw-r--r--   0 greg       (501) staff       (20)      337 2023-04-26 16:56:15.000000 py_common_fetch-0.352/py_common_fetch.egg-info/SOURCES.txt
+-rw-r--r--   0 greg       (501) staff       (20)        1 2023-04-26 16:56:15.000000 py_common_fetch-0.352/py_common_fetch.egg-info/dependency_links.txt
+-rw-r--r--   0 greg       (501) staff       (20)        1 2018-05-11 03:32:51.000000 py_common_fetch-0.352/py_common_fetch.egg-info/not-zip-safe
+-rw-r--r--   0 greg       (501) staff       (20)       64 2023-04-26 16:56:15.000000 py_common_fetch-0.352/py_common_fetch.egg-info/requires.txt
+-rw-r--r--   0 greg       (501) staff       (20)        8 2023-04-26 16:56:15.000000 py_common_fetch-0.352/py_common_fetch.egg-info/top_level.txt
+-rw-r--r--   0 greg       (501) staff       (20)       38 2023-04-26 16:56:15.548308 py_common_fetch-0.352/setup.cfg
+-rw-r--r--   0 greg       (501) staff       (20)      987 2023-04-26 16:55:44.000000 py_common_fetch-0.352/setup.py
```

### Comparing `py_common_fetch-0.342/PKG-INFO` & `py_common_fetch-0.352/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_common_fetch
-Version: 0.342
+Version: 0.352
 Summary: A really simple to use Python fetch screen
 Home-page: https://github.com/bygregonline/py-common-fetch
 Author: Greg flores
 Author-email: bygregonline@yahoo.com
 License: MIT
 Keywords: noefetch common information welcome screen
 Description-Content-Type: text/markdown
```

### Comparing `py_common_fetch-0.342/README.md` & `py_common_fetch-0.352/README.md`

 * *Files identical despite different names*

### Comparing `py_common_fetch-0.342/aniachi/stringUtils.py` & `py_common_fetch-0.352/aniachi/stringUtils.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,20 @@
 #   / ____/ / / / | / / ____/
 #  / /_  / / / /  |/ / /     
 # / __/ / /_/ / /|  / /___   
 #/_/    \____/_/ |_/\____/ 
 #
 
 def str2bool(v):
-    return v.lower() in ("yes", "true", "t", "1","si","oui","SI","YES","TRUE")
+    if v is not None:
+        b=str(v)
+        return b.lower() in ('yes', 'true', 't', '1','si','oui','y')
+    else:
+        return False
+    
 
 
 #
 #
 #
 #
 #   / ____/ / / / | / / ____/
```

### Comparing `py_common_fetch-0.342/aniachi/systemUtils.py` & `py_common_fetch-0.352/aniachi/systemUtils.py`

 * *Files identical despite different names*

### Comparing `py_common_fetch-0.342/aniachi/timeUtils.py` & `py_common_fetch-0.352/aniachi/timeUtils.py`

 * *Files identical despite different names*

### Comparing `py_common_fetch-0.342/py_common_fetch.egg-info/PKG-INFO` & `py_common_fetch-0.352/py_common_fetch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-common-fetch
-Version: 0.342
+Version: 0.352
 Summary: A really simple to use Python fetch screen
 Home-page: https://github.com/bygregonline/py-common-fetch
 Author: Greg flores
 Author-email: bygregonline@yahoo.com
 License: MIT
 Keywords: noefetch common information welcome screen
 Description-Content-Type: text/markdown
```

### Comparing `py_common_fetch-0.342/setup.py` & `py_common_fetch-0.352/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 setup(
     author='Greg flores',
     author_email='bygregonline@yahoo.com',
     license='MIT',
     zip_safe=False,
     packages=['aniachi'],
     name='py_common_fetch',    # This is the name of your PyPI-package.
-    version='0.342',                          # Update the version number for new releases
+    version='0.352',                          # Update the version number for new releases
     scripts=['aniachi/timeUtils.py', 'aniachi/stringUtils.py','aniachi/systemUtils.py'],   
     keywords='noefetch common information welcome screen',
     install_requires=['pip', 'psutil>=5.4.5','json2html','py-cpuinfo','termcolor','numpy','tabulate'],
     url='https://github.com/bygregonline/py-common-fetch',
     description='A really simple to use Python fetch screen',
     long_description_content_type='text/markdown',
     long_description=long_description  # Optional
```

