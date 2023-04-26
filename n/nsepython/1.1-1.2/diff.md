# Comparing `tmp/nsepython-1.1.tar.gz` & `tmp/nsepython-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsepython-1.1.tar", last modified: Wed Apr 26 20:47:45 2023, max compression
+gzip compressed data, was "nsepython-1.2.tar", last modified: Wed Apr 26 20:58:05 2023, max compression
```

## Comparing `nsepython-1.1.tar` & `nsepython-1.2.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 20:47:45.832784 nsepython-1.1/
--rw-rw-rw-   0        0        0    35176 2021-05-30 09:46:07.000000 nsepython-1.1/LICENSE
--rw-rw-rw-   0        0        0     2374 2023-04-26 20:47:45.830226 nsepython-1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1682 2023-04-26 20:24:52.000000 nsepython-1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-26 20:47:45.728443 nsepython-1.1/nsepython/
--rw-rw-rw-   0        0        0       44 2021-05-30 09:46:07.000000 nsepython-1.1/nsepython/__init__.py
--rw-rw-rw-   0        0        0    36568 2023-04-26 20:46:23.000000 nsepython-1.1/nsepython/rahu.py
--rw-rw-rw-   0        0        0    36566 2023-04-26 20:46:31.000000 nsepython-1.1/nsepython/rahuserver.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:47:45.826623 nsepython-1.1/nsepython.egg-info/
--rw-rw-rw-   0        0        0     2374 2023-04-26 20:47:44.000000 nsepython-1.1/nsepython.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      254 2023-04-26 20:47:45.000000 nsepython-1.1/nsepython.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 20:47:44.000000 nsepython-1.1/nsepython.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-04-26 20:47:44.000000 nsepython-1.1/nsepython.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-26 20:47:44.000000 nsepython-1.1/nsepython.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-26 20:47:45.832784 nsepython-1.1/setup.cfg
--rw-rw-rw-   0        0        0     1010 2023-04-26 20:47:10.000000 nsepython-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 20:58:05.830448 nsepython-1.2/
+-rw-rw-rw-   0        0        0    35176 2021-05-30 09:46:07.000000 nsepython-1.2/LICENSE
+-rw-rw-rw-   0        0        0     2374 2023-04-26 20:58:05.829412 nsepython-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1682 2023-04-26 20:24:52.000000 nsepython-1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-26 20:58:05.798058 nsepython-1.2/nsepython/
+-rw-rw-rw-   0        0        0       44 2021-05-30 09:46:07.000000 nsepython-1.2/nsepython/__init__.py
+-rw-rw-rw-   0        0        0    35817 2023-04-26 20:57:40.000000 nsepython-1.2/nsepython/rahu.py
+drwxrwxrwx   0        0        0        0 2023-04-26 20:58:05.826150 nsepython-1.2/nsepython.egg-info/
+-rw-rw-rw-   0        0        0     2374 2023-04-26 20:58:05.000000 nsepython-1.2/nsepython.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2023-04-26 20:58:05.000000 nsepython-1.2/nsepython.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 20:58:05.000000 nsepython-1.2/nsepython.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-04-26 20:58:05.000000 nsepython-1.2/nsepython.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-26 20:58:05.000000 nsepython-1.2/nsepython.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-26 20:58:05.830956 nsepython-1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1010 2023-04-26 20:57:24.000000 nsepython-1.2/setup.py
```

### Comparing `nsepython-1.1/LICENSE` & `nsepython-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nsepython-1.1/PKG-INFO` & `nsepython-1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsepython
-Version: 1.1
+Version: 1.2
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
-Metadata-Version: 2.1 Name: nsepython Version: 1.1 Summary: Python library for
+Metadata-Version: 2.1 Name: nsepython Version: 1.2 Summary: Python library for
 NSE India APIs Home-page: https://github.com/aeron7/nsepython Author: Aeron7
 Author-email: dexter@unofficed.com Keywords:
 nseindia,nse,python,sdk,trading,stock markets Classifier: Intended Audience ::
 Developers Classifier: Natural Language :: English Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: Implementation :: PyPy Classifier: Topic :: Software Development ::
```

### Comparing `nsepython-1.1/README.md` & `nsepython-1.2/README.md`

 * *Files identical despite different names*

### Comparing `nsepython-1.1/nsepython/rahu.py` & `nsepython-1.2/nsepython/rahu.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,31 +9,14 @@
 import datetime,time
 import logging
 import re
 
 
 mode ='local'
 
-if(mode=='vpn'):
-    def nsefetch(payload):
-        if (("%26" in payload) or ("%20" in payload)):
-            encoded_url = payload
-        else:
-            encoded_url = urllib.parse.quote(payload, safe=':/?&=')
-        payload_var = 'curl -b cookies.txt "' + encoded_url + '"' + curl_headers + ''
-        try:
-            output = os.popen(payload_var).read()
-            output=json.loads(output)
-        except ValueError:  # includes simplejson.decoder.JSONDecodeError:
-            payload2 = "https://www.nseindia.com"
-            output2 = os.popen('curl -c cookies.txt "'+payload2+'"'+curl_headers+'').read()
-    
-            output = os.popen(payload_var).read()
-            output=json.loads(output)
-        return output
 if(mode=='local'):
     def nsefetch(payload):
         output = requests.get(payload,headers=headers).json()
         return output
 
 
 headers = {
```

### Comparing `nsepython-1.1/nsepython.egg-info/PKG-INFO` & `nsepython-1.2/nsepython.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsepython
-Version: 1.1
+Version: 1.2
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
-Metadata-Version: 2.1 Name: nsepython Version: 1.1 Summary: Python library for
+Metadata-Version: 2.1 Name: nsepython Version: 1.2 Summary: Python library for
 NSE India APIs Home-page: https://github.com/aeron7/nsepython Author: Aeron7
 Author-email: dexter@unofficed.com Keywords:
 nseindia,nse,python,sdk,trading,stock markets Classifier: Intended Audience ::
 Developers Classifier: Natural Language :: English Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: Implementation :: PyPy Classifier: Topic :: Software Development ::
```

### Comparing `nsepython-1.1/setup.py` & `nsepython-1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = 'nsepython',
     packages=setuptools.find_packages(),
-    version = '1.1',
+    version = '1.2',
     include_package_data=True,
     description = 'Python library for NSE India APIs',
     long_description=long_description,
     long_description_content_type="text/markdown",  author = 'Aeron7',
     author_email = 'dexter@unofficed.com',
     url = 'https://github.com/aeron7/nsepython',
     install_requires=['requests', 'pandas','scipy'],
```

