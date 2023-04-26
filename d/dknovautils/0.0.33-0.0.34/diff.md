# Comparing `tmp/dknovautils-0.0.33.tar.gz` & `tmp/dknovautils-0.0.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dknovautils-0.0.33.tar", last modified: Sun Apr 23 14:12:42 2023, max compression
+gzip compressed data, was "dist/dknovautils-0.0.34.tar", last modified: Wed Apr 26 05:10:16 2023, max compression
```

## Comparing `dknovautils-0.0.33.tar` & `dknovautils-0.0.34.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-04-23 14:12:42.000000 dknovautils-0.0.33/
-drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-04-23 14:12:42.000000 dknovautils-0.0.33/dknovautils/
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1881 2023-04-22 16:09:58.000000 dknovautils-0.0.33/dknovautils/commons.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     5513 2023-04-23 14:12:41.000000 dknovautils-0.0.33/dknovautils/dkat.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1510 2023-04-13 12:40:40.000000 dknovautils-0.0.33/dknovautils/dkfiles.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1149 2023-04-22 02:58:52.000000 dknovautils-0.0.33/dknovautils/dkipy.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      711 2023-04-23 14:12:41.000000 dknovautils-0.0.33/dknovautils/dk_imports.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      490 2023-04-13 12:40:48.000000 dknovautils-0.0.33/dknovautils/example.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      140 2023-04-13 15:12:06.000000 dknovautils-0.0.33/dknovautils/myadd.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      160 2023-04-13 15:11:54.000000 dknovautils-0.0.33/dknovautils/mysubtract.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      307 2023-04-21 15:52:41.000000 dknovautils-0.0.33/dknovautils/__init__.py
-drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-04-23 14:12:42.000000 dknovautils-0.0.33/dknovautils.egg-info/
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)        1 2023-04-23 14:12:42.000000 dknovautils-0.0.33/dknovautils.egg-info/dependency_links.txt
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      881 2023-04-23 14:12:42.000000 dknovautils-0.0.33/dknovautils.egg-info/PKG-INFO
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)        6 2023-04-23 14:12:42.000000 dknovautils-0.0.33/dknovautils.egg-info/requires.txt
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      407 2023-04-23 14:12:42.000000 dknovautils-0.0.33/dknovautils.egg-info/SOURCES.txt
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)       12 2023-04-23 14:12:42.000000 dknovautils-0.0.33/dknovautils.egg-info/top_level.txt
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      105 2023-03-09 04:32:08.000000 dknovautils-0.0.33/LICENSE
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      881 2023-04-23 14:12:42.000000 dknovautils-0.0.33/PKG-INFO
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      472 2023-03-09 06:46:27.000000 dknovautils-0.0.33/README.md
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)       38 2023-04-23 14:12:42.000000 dknovautils-0.0.33/setup.cfg
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1140 2023-04-23 14:12:41.000000 dknovautils-0.0.33/setup.py
+drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-04-26 05:10:16.000000 dknovautils-0.0.34/
+drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-04-26 05:10:16.000000 dknovautils-0.0.34/dknovautils/
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     2308 2023-04-26 05:09:42.000000 dknovautils-0.0.34/dknovautils/commons.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     5866 2023-04-26 05:10:15.000000 dknovautils-0.0.34/dknovautils/dkat.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1510 2023-04-13 12:40:40.000000 dknovautils-0.0.34/dknovautils/dkfiles.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1149 2023-04-22 02:58:52.000000 dknovautils-0.0.34/dknovautils/dkipy.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      711 2023-04-26 05:10:15.000000 dknovautils-0.0.34/dknovautils/dk_imports.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      490 2023-04-13 12:40:48.000000 dknovautils-0.0.34/dknovautils/example.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      140 2023-04-13 15:12:06.000000 dknovautils-0.0.34/dknovautils/myadd.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      160 2023-04-13 15:11:54.000000 dknovautils-0.0.34/dknovautils/mysubtract.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      307 2023-04-21 15:52:41.000000 dknovautils-0.0.34/dknovautils/__init__.py
+drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-04-26 05:10:16.000000 dknovautils-0.0.34/dknovautils.egg-info/
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)        1 2023-04-26 05:10:16.000000 dknovautils-0.0.34/dknovautils.egg-info/dependency_links.txt
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      881 2023-04-26 05:10:16.000000 dknovautils-0.0.34/dknovautils.egg-info/PKG-INFO
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)        6 2023-04-26 05:10:16.000000 dknovautils-0.0.34/dknovautils.egg-info/requires.txt
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      407 2023-04-26 05:10:16.000000 dknovautils-0.0.34/dknovautils.egg-info/SOURCES.txt
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)       12 2023-04-26 05:10:16.000000 dknovautils-0.0.34/dknovautils.egg-info/top_level.txt
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      105 2023-03-09 04:32:08.000000 dknovautils-0.0.34/LICENSE
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      881 2023-04-26 05:10:16.000000 dknovautils-0.0.34/PKG-INFO
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      472 2023-03-09 06:46:27.000000 dknovautils-0.0.34/README.md
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)       38 2023-04-26 05:10:16.000000 dknovautils-0.0.34/setup.cfg
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1140 2023-04-26 05:10:15.000000 dknovautils-0.0.34/setup.py
```

### Comparing `dknovautils-0.0.33/dknovautils/commons.py` & `dknovautils-0.0.34/dknovautils/commons.py`

 * *Files 24% similar despite different names*

```diff
@@ -36,25 +36,43 @@
     _iprint(obj, level=LLevel.Warn)
 
 
 def iprint_error(obj):
     _iprint(obj, level=LLevel.Error)
 
 
+_log_inited = False
+
+
 def _iprint(obj, level: LLevel):
 
     if AT._innerLoggerFun_ is not None:
         AT._innerLoggerFun_(obj, level)
         return
     else:
         pass
 
-    now = datetime.now()
+    # now = datetime.now()
     # dts = now.strftime("%d/%m/%Y %H:%M:%S")
-    otstr = now.isoformat()[:(10 + 1 + 8+4)]
+    # otstr = now.isoformat()[:(10 + 1 + 8+4)]
+
+    # _FORMAT_111 = '%(asctime)s %(message)s'
+    # logging.basicConfig(format=_FORMAT)
+
+    global _log_inited
+    if not _log_inited:
+        _log_inited = True
+
+        # 只在没有配置的时候起作用 不会重复执行
+        logging.basicConfig(level=logging.NOTSET,
+                            format=AT._LOG_FORMAT_106)
+
+    logging.log(level.value, obj)
+
+    return
 
     if False:
 
         otstr2 = datetime.fromtimestamp(time.time()).strftime(
             "%Y-%m-%dT%H:%M:%S.%f")[0:23]
 
         msg = f'[{otstr}]{obj}'
```

### Comparing `dknovautils-0.0.33/dknovautils/dkat.py` & `dknovautils-0.0.34/dknovautils/dkat.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 import dknovautils
 from dknovautils.commons import *
 
 import beepy
 
 
-DkAppVer = '0.0.33'
+DkAppVer = '0.0.34'
 _unknown_err = '_unknown_err4035'
 
 
 class AT(object):
 
     _innerLoggerFun_ = None
 
@@ -45,32 +45,36 @@
             pass
 
         if initInnerLoggerFun:
             AT._innerLoggerFun_ = mloggerFun
 
         return mloggerFun
 
-    @staticmethod
-    def log_basicConfig(filename='my.log', loggerName='dkn', initInnerLoggerFun=True):
-        LOG_FORMAT = "%(asctime)s - %(levelname)s - %(message)s"
-        DATE_FORMAT = "%m/%d/%Y %H:%M:%S %p"
+    _LOG_FORMAT_100 = "%(asctime)s - %(levelname)s - %(message)s"
+    _DATE_FORMAT_100 = "%m/%d/%Y %H:%M:%S %p"
+    # _DATE_FORMAT_iso_simple = "%m/%d/%Y %H:%M:%S %p"
+
+    _LOG_FORMAT_106 = '%(asctime)s - %(name)s - %(levelname)s - %(message)s'
+
+    @classmethod
+    def log_basicConfig(cls, filename='my.log', loggerName='dkn', initInnerLoggerFun=True):
 
         logging.basicConfig(filename=filename, level=logging.NOTSET,
-                            format=LOG_FORMAT, datefmt=DATE_FORMAT)
+                            format=cls._LOG_FORMAT_100, datefmt=cls._DATE_FORMAT_100, force=True)
 
         logger = logging.getLogger(loggerName)
         logger.setLevel(logging.DEBUG)
 
         # create console handler and set level to debug
         ch = logging.StreamHandler()
         ch.setLevel(logging.DEBUG)
 
         # create formatter
         formatter = logging.Formatter(
-            '%(asctime)s - %(name)s - %(levelname)s - %(message)s')
+            cls._LOG_FORMAT_106)
 
         # add formatter to ch
         ch.setFormatter(formatter)
 
         # add ch to logger
         logger.addHandler(ch)
 
@@ -117,30 +121,37 @@
         assert sys.version_info >= (3, 11)
 
     @staticmethod
     def fepochMillis() -> int:
         millisec = int(AT.fepochSecs() * 1000)
         return millisec
 
-    @staticmethod
-    def fepochSecs() -> float:
+    _last_epochsecs = 0.0
+
+    @classmethod
+    def fepochSecs(cls) -> float:
         '''
-         time.monotonic()
+         time.monotonic()不是epoch值。fuck
 
         '''
-        return time.monotonic()
-        return time.time()
+        # return time.monotonic()
+        r = time.time()
+        if r <= cls._last_epochsecs:
+            return cls._last_epochsecs
+        else:
+            cls._last_epochsecs = r
+            return r
 
     '''
         # dd/mm/YY H:M:S
     dts = now.strftime("%d/%m/%Y %H:%M:%S")
     print("date and time =", dts)
 
     # 20200101T120000
-    dts = now.strftime("%Y%m%dT%H%M%S")
+    dts = datetime.now().strftime("%Y%m%dT%H%M%S")
     print("date and time =", dts)
     
     
     '''
 
     @staticmethod
     def sdf_logger():
```

### Comparing `dknovautils-0.0.33/dknovautils/dkfiles.py` & `dknovautils-0.0.34/dknovautils/dkfiles.py`

 * *Files identical despite different names*

### Comparing `dknovautils-0.0.33/dknovautils/dkipy.py` & `dknovautils-0.0.34/dknovautils/dkipy.py`

 * *Files identical despite different names*

### Comparing `dknovautils-0.0.33/dknovautils/dk_imports.py` & `dknovautils-0.0.34/dknovautils/dk_imports.py`

 * *Files identical despite different names*

### Comparing `dknovautils-0.0.33/dknovautils.egg-info/PKG-INFO` & `dknovautils-0.0.34/dknovautils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dknovautils
-Version: 0.0.33
+Version: 0.0.34
 Summary: This is the tools for dknova.
 Home-page: http://example.com
 Author: dknova
 Author-email: dknova@example.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dknovautils-0.0.33/PKG-INFO` & `dknovautils-0.0.34/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dknovautils
-Version: 0.0.33
+Version: 0.0.34
 Summary: This is the tools for dknova.
 Home-page: http://example.com
 Author: dknova
 Author-email: dknova@example.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dknovautils-0.0.33/setup.py` & `dknovautils-0.0.34/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import re
 import setuptools
 
 from distutils.core import setup
 from setuptools import find_packages
 
-DkAppVer = '0.0.33'
+DkAppVer = '0.0.34'
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="dknovautils",
     version=DkAppVer,
```

