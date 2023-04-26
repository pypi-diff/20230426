# Comparing `tmp/nsepython-1.tar.gz` & `tmp/nsepython-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsepython-1.tar", last modified: Wed Apr 26 20:37:01 2023, max compression
+gzip compressed data, was "nsepython-1.1.tar", last modified: Wed Apr 26 20:47:45 2023, max compression
```

## Comparing `nsepython-1.tar` & `nsepython-1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 20:37:01.128758 nsepython-1/
--rw-rw-rw-   0        0        0    35176 2021-05-30 09:46:07.000000 nsepython-1/LICENSE
--rw-rw-rw-   0        0        0     2372 2023-04-26 20:37:01.126130 nsepython-1/PKG-INFO
--rw-rw-rw-   0        0        0     1682 2023-04-26 20:24:52.000000 nsepython-1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-26 20:37:01.076778 nsepython-1/nsepython/
--rw-rw-rw-   0        0        0       44 2021-05-30 09:46:07.000000 nsepython-1/nsepython/__init__.py
--rw-rw-rw-   0        0        0    36359 2023-04-26 20:23:32.000000 nsepython-1/nsepython/rahu.py
--rw-rw-rw-   0        0        0    36357 2023-04-26 20:27:16.000000 nsepython-1/nsepython/rahuserver.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:37:01.119524 nsepython-1/nsepython.egg-info/
--rw-rw-rw-   0        0        0     2372 2023-04-26 20:36:54.000000 nsepython-1/nsepython.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      254 2023-04-26 20:36:54.000000 nsepython-1/nsepython.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 20:36:54.000000 nsepython-1/nsepython.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-04-26 20:36:54.000000 nsepython-1/nsepython.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-26 20:36:54.000000 nsepython-1/nsepython.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-26 20:37:01.129277 nsepython-1/setup.cfg
--rw-rw-rw-   0        0        0     1008 2023-04-26 20:25:51.000000 nsepython-1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 20:47:45.832784 nsepython-1.1/
+-rw-rw-rw-   0        0        0    35176 2021-05-30 09:46:07.000000 nsepython-1.1/LICENSE
+-rw-rw-rw-   0        0        0     2374 2023-04-26 20:47:45.830226 nsepython-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1682 2023-04-26 20:24:52.000000 nsepython-1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-26 20:47:45.728443 nsepython-1.1/nsepython/
+-rw-rw-rw-   0        0        0       44 2021-05-30 09:46:07.000000 nsepython-1.1/nsepython/__init__.py
+-rw-rw-rw-   0        0        0    36568 2023-04-26 20:46:23.000000 nsepython-1.1/nsepython/rahu.py
+-rw-rw-rw-   0        0        0    36566 2023-04-26 20:46:31.000000 nsepython-1.1/nsepython/rahuserver.py
+drwxrwxrwx   0        0        0        0 2023-04-26 20:47:45.826623 nsepython-1.1/nsepython.egg-info/
+-rw-rw-rw-   0        0        0     2374 2023-04-26 20:47:44.000000 nsepython-1.1/nsepython.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      254 2023-04-26 20:47:45.000000 nsepython-1.1/nsepython.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 20:47:44.000000 nsepython-1.1/nsepython.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-04-26 20:47:44.000000 nsepython-1.1/nsepython.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-26 20:47:44.000000 nsepython-1.1/nsepython.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-26 20:47:45.832784 nsepython-1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1010 2023-04-26 20:47:10.000000 nsepython-1.1/setup.py
```

### Comparing `nsepython-1/LICENSE` & `nsepython-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nsepython-1/PKG-INFO` & `nsepython-1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsepython
-Version: 1
+Version: 1.1
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
-Metadata-Version: 2.1 Name: nsepython Version: 1 Summary: Python library for
+Metadata-Version: 2.1 Name: nsepython Version: 1.1 Summary: Python library for
 NSE India APIs Home-page: https://github.com/aeron7/nsepython Author: Aeron7
 Author-email: dexter@unofficed.com Keywords:
 nseindia,nse,python,sdk,trading,stock markets Classifier: Intended Audience ::
 Developers Classifier: Natural Language :: English Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: Implementation :: PyPy Classifier: Topic :: Software Development ::
```

### Comparing `nsepython-1/README.md` & `nsepython-1.1/README.md`

 * *Files identical despite different names*

### Comparing `nsepython-1/nsepython/rahu.py` & `nsepython-1.1/nsepython/rahu.py`

 * *Files 0% similar despite different names*

```diff
@@ -802,8 +802,11 @@
 
 def nse_most_active(type="securities",sort="value"):
     payload = nsefetch("https://www.nseindia.com/api/live-analysis-most-active-"+type+"?index="+sort+"")
     payload = pd.DataFrame(payload["data"])
     return payload
 
 
-def nse_eq_symbols():
+def nse_eq_symbols():
+    #https://forum.unofficed.com/t/feature-request-stocklist-api/1073/11
+    eq_list_pd = pd.read_csv('https://archives.nseindia.com/content/equities/EQUITY_L.csv')
+    return eq_list_pd['SYMBOL'].tolist()
```

### Comparing `nsepython-1/nsepython/rahuserver.py` & `nsepython-1.1/nsepython/rahuserver.py`

 * *Files 0% similar despite different names*

```diff
@@ -802,8 +802,11 @@
 
 def nse_most_active(type="securities",sort="value"):
     payload = nsefetch("https://www.nseindia.com/api/live-analysis-most-active-"+type+"?index="+sort+"")
     payload = pd.DataFrame(payload["data"])
     return payload
 
 
-def nse_eq_symbols():
+def nse_eq_symbols():
+    #https://forum.unofficed.com/t/feature-request-stocklist-api/1073/11
+    eq_list_pd = pd.read_csv('https://archives.nseindia.com/content/equities/EQUITY_L.csv')
+    return eq_list_pd['SYMBOL'].tolist()
```

### Comparing `nsepython-1/nsepython.egg-info/PKG-INFO` & `nsepython-1.1/nsepython.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsepython
-Version: 1
+Version: 1.1
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
-Metadata-Version: 2.1 Name: nsepython Version: 1 Summary: Python library for
+Metadata-Version: 2.1 Name: nsepython Version: 1.1 Summary: Python library for
 NSE India APIs Home-page: https://github.com/aeron7/nsepython Author: Aeron7
 Author-email: dexter@unofficed.com Keywords:
 nseindia,nse,python,sdk,trading,stock markets Classifier: Intended Audience ::
 Developers Classifier: Natural Language :: English Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: Implementation :: PyPy Classifier: Topic :: Software Development ::
```

### Comparing `nsepython-1/setup.py` & `nsepython-1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = 'nsepython',
     packages=setuptools.find_packages(),
-    version = '1',
+    version = '1.1',
     include_package_data=True,
     description = 'Python library for NSE India APIs',
     long_description=long_description,
     long_description_content_type="text/markdown",  author = 'Aeron7',
     author_email = 'dexter@unofficed.com',
     url = 'https://github.com/aeron7/nsepython',
     install_requires=['requests', 'pandas','scipy'],
```

