# Comparing `tmp/nsepythonserver-1.2.tar.gz` & `tmp/nsepythonserver-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsepythonserver-1.2.tar", last modified: Wed Apr 26 20:59:01 2023, max compression
+gzip compressed data, was "nsepythonserver-1.3.tar", last modified: Wed Apr 26 21:01:38 2023, max compression
```

## Comparing `nsepythonserver-1.2.tar` & `nsepythonserver-1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 20:59:01.294534 nsepythonserver-1.2/
--rw-rw-rw-   0        0        0    35176 2021-05-30 09:46:07.000000 nsepythonserver-1.2/LICENSE
--rw-rw-rw-   0        0        0     2380 2023-04-26 20:59:01.293478 nsepythonserver-1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1682 2023-04-26 20:24:52.000000 nsepythonserver-1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-26 20:59:01.255449 nsepythonserver-1.2/nsepythonserver/
--rw-rw-rw-   0        0        0       44 2021-05-30 09:46:07.000000 nsepythonserver-1.2/nsepythonserver/__init__.py
--rw-rw-rw-   0        0        0    36434 2023-04-26 20:57:51.000000 nsepythonserver-1.2/nsepythonserver/rahu.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:59:01.290874 nsepythonserver-1.2/nsepythonserver.egg-info/
--rw-rw-rw-   0        0        0     2380 2023-04-26 20:59:01.000000 nsepythonserver-1.2/nsepythonserver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2023-04-26 20:59:01.000000 nsepythonserver-1.2/nsepythonserver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 20:59:01.000000 nsepythonserver-1.2/nsepythonserver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-04-26 20:59:01.000000 nsepythonserver-1.2/nsepythonserver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-04-26 20:59:01.000000 nsepythonserver-1.2/nsepythonserver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-26 20:59:01.295051 nsepythonserver-1.2/setup.cfg
--rw-rw-rw-   0        0        0     1016 2023-04-26 20:57:23.000000 nsepythonserver-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 21:01:38.913543 nsepythonserver-1.3/
+-rw-rw-rw-   0        0        0    35176 2021-05-30 09:46:07.000000 nsepythonserver-1.3/LICENSE
+-rw-rw-rw-   0        0        0     2380 2023-04-26 21:01:38.912007 nsepythonserver-1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1682 2023-04-26 20:24:52.000000 nsepythonserver-1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-26 21:01:38.887585 nsepythonserver-1.3/nsepythonserver/
+-rw-rw-rw-   0        0        0       44 2021-05-30 09:46:07.000000 nsepythonserver-1.3/nsepythonserver/__init__.py
+-rw-rw-rw-   0        0        0    36434 2023-04-26 20:57:51.000000 nsepythonserver-1.3/nsepythonserver/rahu.py
+drwxrwxrwx   0        0        0        0 2023-04-26 21:01:38.909465 nsepythonserver-1.3/nsepythonserver.egg-info/
+-rw-rw-rw-   0        0        0     2380 2023-04-26 21:01:38.000000 nsepythonserver-1.3/nsepythonserver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2023-04-26 21:01:38.000000 nsepythonserver-1.3/nsepythonserver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 21:01:38.000000 nsepythonserver-1.3/nsepythonserver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-04-26 21:01:38.000000 nsepythonserver-1.3/nsepythonserver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-04-26 21:01:38.000000 nsepythonserver-1.3/nsepythonserver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-26 21:01:38.914067 nsepythonserver-1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1016 2023-04-26 21:01:34.000000 nsepythonserver-1.3/setup.py
```

### Comparing `nsepythonserver-1.2/LICENSE` & `nsepythonserver-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nsepythonserver-1.2/PKG-INFO` & `nsepythonserver-1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsepythonserver
-Version: 1.2
+Version: 1.3
 Summary: Python library for NSE India APIs
 Home-page: https://github.com/aeron7/nsepython
 Author: Aeron7
 Author-email: dexter@unofficed.com
 Keywords: nseindia,nse,python,sdk,trading,stock markets
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nsepythonserver Version: 1.2 Summary: Python
+Metadata-Version: 2.1 Name: nsepythonserver Version: 1.3 Summary: Python
 library for NSE India APIs Home-page: https://github.com/aeron7/nsepython
 Author: Aeron7 Author-email: dexter@unofficed.com Keywords:
 nseindia,nse,python,sdk,trading,stock markets Classifier: Intended Audience ::
 Developers Classifier: Natural Language :: English Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: Implementation :: PyPy Classifier: Topic :: Software Development ::
```

### Comparing `nsepythonserver-1.2/README.md` & `nsepythonserver-1.3/README.md`

 * *Files identical despite different names*

### Comparing `nsepythonserver-1.2/nsepythonserver/rahu.py` & `nsepythonserver-1.3/nsepythonserver/rahu.py`

 * *Files identical despite different names*

### Comparing `nsepythonserver-1.2/nsepythonserver.egg-info/PKG-INFO` & `nsepythonserver-1.3/nsepythonserver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsepythonserver
-Version: 1.2
+Version: 1.3
 Summary: Python library for NSE India APIs
 Home-page: https://github.com/aeron7/nsepython
 Author: Aeron7
 Author-email: dexter@unofficed.com
 Keywords: nseindia,nse,python,sdk,trading,stock markets
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nsepythonserver Version: 1.2 Summary: Python
+Metadata-Version: 2.1 Name: nsepythonserver Version: 1.3 Summary: Python
 library for NSE India APIs Home-page: https://github.com/aeron7/nsepython
 Author: Aeron7 Author-email: dexter@unofficed.com Keywords:
 nseindia,nse,python,sdk,trading,stock markets Classifier: Intended Audience ::
 Developers Classifier: Natural Language :: English Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: Implementation :: PyPy Classifier: Topic :: Software Development ::
```

### Comparing `nsepythonserver-1.2/setup.py` & `nsepythonserver-1.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = 'nsepythonserver',
     packages=setuptools.find_packages(),
-    version = '1.2',
+    version = '1.3',
     include_package_data=True,
     description = 'Python library for NSE India APIs',
     long_description=long_description,
     long_description_content_type="text/markdown",  author = 'Aeron7',
     author_email = 'dexter@unofficed.com',
     url = 'https://github.com/aeron7/nsepython',
     install_requires=['requests', 'pandas','scipy'],
```

