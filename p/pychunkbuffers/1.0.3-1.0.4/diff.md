# Comparing `tmp/pychunkbuffers-1.0.3.tar.gz` & `tmp/pychunkbuffers-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pychunkbuffers-1.0.3.tar", last modified: Mon Apr 24 07:49:32 2023, max compression
+gzip compressed data, was "pychunkbuffers-1.0.4.tar", last modified: Wed Apr 26 10:08:27 2023, max compression
```

## Comparing `pychunkbuffers-1.0.3.tar` & `pychunkbuffers-1.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 07:49:32.283294 pychunkbuffers-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-24 07:49:13.000000 pychunkbuffers-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-04-24 07:49:32.279294 pychunkbuffers-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-04-24 07:49:13.000000 pychunkbuffers-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 07:49:32.279294 pychunkbuffers-1.0.3/pychunkbuffers/
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-04-24 07:49:13.000000 pychunkbuffers-1.0.3/pychunkbuffers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 07:49:32.279294 pychunkbuffers-1.0.3/pychunkbuffers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-04-24 07:49:32.000000 pychunkbuffers-1.0.3/pychunkbuffers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-24 07:49:32.000000 pychunkbuffers-1.0.3/pychunkbuffers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 07:49:32.000000 pychunkbuffers-1.0.3/pychunkbuffers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-24 07:49:32.000000 pychunkbuffers-1.0.3/pychunkbuffers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 07:49:32.283294 pychunkbuffers-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-24 07:49:13.000000 pychunkbuffers-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:08:27.032872 pychunkbuffers-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-26 10:08:11.000000 pychunkbuffers-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-04-26 10:08:27.032872 pychunkbuffers-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-04-26 10:08:11.000000 pychunkbuffers-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:08:27.028872 pychunkbuffers-1.0.4/pychunkbuffers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-04-26 10:08:11.000000 pychunkbuffers-1.0.4/pychunkbuffers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:08:27.032872 pychunkbuffers-1.0.4/pychunkbuffers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-04-26 10:08:27.000000 pychunkbuffers-1.0.4/pychunkbuffers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-26 10:08:27.000000 pychunkbuffers-1.0.4/pychunkbuffers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 10:08:27.000000 pychunkbuffers-1.0.4/pychunkbuffers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-26 10:08:27.000000 pychunkbuffers-1.0.4/pychunkbuffers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 10:08:27.032872 pychunkbuffers-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-26 10:08:11.000000 pychunkbuffers-1.0.4/setup.py
```

### Comparing `pychunkbuffers-1.0.3/LICENSE` & `pychunkbuffers-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pychunkbuffers-1.0.3/PKG-INFO` & `pychunkbuffers-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pychunkbuffers
-Version: 1.0.3
+Version: 1.0.4
 Summary: An open-source python library for writing large amounts of data to buffers via chunks
 Home-page: https://github.com/AdityaIyer2k7/pychunkbuffers
 Author: AdityaIyer2k7
 Author-email: adityaiyer2007@gmail.com
 Keywords: python 3,threading,thread,chunking,buffers,pychunk,pybuffer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `pychunkbuffers-1.0.3/README.md` & `pychunkbuffers-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pychunkbuffers-1.0.3/pychunkbuffers/__init__.py` & `pychunkbuffers-1.0.4/pychunkbuffers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         Initially, all values are False.
         When a chunk finishes its function, it's corresponding status is set to True.
         `while not all(LIST): pass` can be used to wait for all chunks to finish
     """
     assert type(chunksz)==int
     assert type(minidx)==int
     assert type(maxidx)==int
-    n = minidx+math.ceil((maxidx-minidx)/chunksz)
+    n = math.ceil((maxidx-minidx)/chunksz)
     statuslist = [False]*n
     for i in range(n):
         ChunkedFunction(func, i, chunksz, minidx, maxidx, args, kwargs, daemon, statuslist).start()
     return statuslist
 
 def run(func:Callable, *args, **kwargs) -> List[bool]:
     return run_chunked(func, *args, **kwargs)
```

### Comparing `pychunkbuffers-1.0.3/pychunkbuffers.egg-info/PKG-INFO` & `pychunkbuffers-1.0.4/pychunkbuffers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pychunkbuffers
-Version: 1.0.3
+Version: 1.0.4
 Summary: An open-source python library for writing large amounts of data to buffers via chunks
 Home-page: https://github.com/AdityaIyer2k7/pychunkbuffers
 Author: AdityaIyer2k7
 Author-email: adityaiyer2007@gmail.com
 Keywords: python 3,threading,thread,chunking,buffers,pychunk,pybuffer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `pychunkbuffers-1.0.3/setup.py` & `pychunkbuffers-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 with open("README.md") as fl: ldesc = fl.read()
 setuptools.setup(
     name="pychunkbuffers",
-    version="1.0.3",
+    version="1.0.4",
     author="AdityaIyer2k7",
     author_email="adityaiyer2007@gmail.com",
     description="An open-source python library for writing large amounts of data to buffers via chunks",
     long_description=ldesc,
     long_description_content_type="text/markdown",
     url="https://github.com/AdityaIyer2k7/pychunkbuffers",
     packages=setuptools.find_packages(),
```

