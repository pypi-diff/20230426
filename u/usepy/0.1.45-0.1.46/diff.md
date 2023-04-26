# Comparing `tmp/usepy-0.1.45.tar.gz` & `tmp/usepy-0.1.46.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usepy-0.1.45.tar", max compression
+gzip compressed data, was "usepy-0.1.46.tar", max compression
```

## Comparing `usepy-0.1.45.tar` & `usepy-0.1.46.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0      749 2023-04-23 02:21:03.395878 usepy-0.1.45/README.md
--rw-r--r--   0        0        0      752 2023-04-23 02:21:03.411879 usepy-0.1.45/pyproject.toml
--rw-r--r--   0        0        0     1763 2023-04-23 02:21:03.411879 usepy-0.1.45/src/usepy/__init__.py
--rw-r--r--   0        0        0     6407 2023-04-23 02:21:03.411879 usepy-0.1.45/src/usepy/_datetime.py
--rw-r--r--   0        0        0     3119 2023-04-23 02:21:03.411879 usepy-0.1.45/src/usepy/_path.py
--rw-r--r--   0        0        0     1217 2023-04-23 02:21:03.411879 usepy-0.1.45/src/usepy/_thread.py
--rw-r--r--   0        0        0        0 2023-04-23 02:21:03.411879 usepy-0.1.45/src/usepy/contrib/__init__.py
--rw-r--r--   0        0        0     1302 2023-04-23 02:21:03.411879 usepy-0.1.45/src/usepy/contrib/pydantic_.py
--rw-r--r--   0        0        0     2039 2023-04-23 02:21:03.411879 usepy-0.1.45/src/usepy/contrib/tenacity_.py
--rw-r--r--   0        0        0      156 2023-04-23 02:21:03.411879 usepy-0.1.45/src/usepy/data/__init__.py
--rw-r--r--   0        0        0     6773 2023-04-23 02:21:03.411879 usepy-0.1.45/src/usepy/data/_string.py
--rw-r--r--   0        0        0     5000 2023-04-23 02:21:03.411879 usepy-0.1.45/src/usepy/data/addict.py
--rw-r--r--   0        0        0     8331 2023-04-23 02:21:03.411879 usepy-0.1.45/src/usepy/data/dict.py
--rw-r--r--   0        0        0     6453 2023-04-23 02:21:03.411879 usepy-0.1.45/src/usepy/data/list.py
--rw-r--r--   0        0        0      681 2023-04-23 02:21:03.411879 usepy-0.1.45/src/usepy/decorator/__init__.py
--rw-r--r--   0        0        0      457 2023-04-23 02:21:03.411879 usepy-0.1.45/src/usepy/decorator/cache.py
--rw-r--r--   0        0        0      415 2023-04-23 02:21:03.411879 usepy-0.1.45/src/usepy/decorator/catch_error.py
--rw-r--r--   0        0        0      382 2023-04-23 02:21:03.411879 usepy-0.1.45/src/usepy/decorator/except_debug.py
--rw-r--r--   0        0        0      416 2023-04-23 02:21:03.411879 usepy-0.1.45/src/usepy/decorator/listify.py
--rw-r--r--   0        0        0     1879 2023-04-23 02:21:03.411879 usepy-0.1.45/src/usepy/decorator/retry.py
--rw-r--r--   0        0        0      377 2023-04-23 02:21:03.411879 usepy-0.1.45/src/usepy/decorator/run_in_thread.py
--rw-r--r--   0        0        0      510 2023-04-23 02:21:03.411879 usepy-0.1.45/src/usepy/decorator/singleton.py
--rw-r--r--   0        0        0      410 2023-04-23 02:21:03.411879 usepy-0.1.45/src/usepy/decorator/timeit.py
--rw-r--r--   0        0        0      138 2023-04-23 02:21:03.411879 usepy-0.1.45/src/usepy/parser/__init__.py
--rw-r--r--   0        0        0     3429 2023-04-23 02:21:03.411879 usepy-0.1.45/src/usepy/parser/curl.py
--rw-r--r--   0        0        0     1379 2023-04-23 02:21:03.411879 usepy-0.1.45/src/usepy/parser/url.py
--rw-r--r--   0        0        0      599 2023-04-23 02:21:03.411879 usepy-0.1.45/src/usepy/utils/__init__.py
--rw-r--r--   0        0        0      677 2023-04-23 02:21:03.415879 usepy-0.1.45/src/usepy/utils/_is.py
--rw-r--r--   0        0        0     1550 2023-04-23 02:21:03.415879 usepy-0.1.45/src/usepy/utils/_to.py
--rw-r--r--   0        0        0     1929 2023-04-23 02:21:03.415879 usepy-0.1.45/src/usepy/utils/bloom_filter.py
--rw-r--r--   0        0        0      307 2023-04-23 02:21:03.415879 usepy-0.1.45/src/usepy/utils/func.py
--rw-r--r--   0        0        0      879 2023-04-23 02:21:03.415879 usepy-0.1.45/src/usepy/utils/html.py
--rw-r--r--   0        0        0     1528 2023-04-23 02:21:03.415879 usepy-0.1.45/src/usepy/utils/import_object.py
--rw-r--r--   0        0        0     4727 2023-04-23 02:21:03.415879 usepy-0.1.45/src/usepy/utils/timer.py
--rw-r--r--   0        0        0   684816 2023-04-23 02:21:03.415879 usepy-0.1.45/src/usepy/utils/useragent.py
--rw-r--r--   0        0        0     1406 2023-04-23 02:21:03.415879 usepy-0.1.45/src/usepy/utils/utils.py
--rw-r--r--   0        0        0     1403 1970-01-01 00:00:00.000000 usepy-0.1.45/PKG-INFO
+-rw-r--r--   0        0        0      749 2023-04-26 05:50:47.132387 usepy-0.1.46/README.md
+-rw-r--r--   0        0        0      752 2023-04-26 05:50:47.144387 usepy-0.1.46/pyproject.toml
+-rw-r--r--   0        0        0     1759 2023-04-26 05:50:47.144387 usepy-0.1.46/src/usepy/__init__.py
+-rw-r--r--   0        0        0     6407 2023-04-26 05:50:47.144387 usepy-0.1.46/src/usepy/_datetime.py
+-rw-r--r--   0        0        0     3119 2023-04-26 05:50:47.144387 usepy-0.1.46/src/usepy/_path.py
+-rw-r--r--   0        0        0     1217 2023-04-26 05:50:47.144387 usepy-0.1.46/src/usepy/_thread.py
+-rw-r--r--   0        0        0        0 2023-04-26 05:50:47.144387 usepy-0.1.46/src/usepy/contrib/__init__.py
+-rw-r--r--   0        0        0     1302 2023-04-26 05:50:47.144387 usepy-0.1.46/src/usepy/contrib/pydantic_.py
+-rw-r--r--   0        0        0     2039 2023-04-26 05:50:47.144387 usepy-0.1.46/src/usepy/contrib/tenacity_.py
+-rw-r--r--   0        0        0      156 2023-04-26 05:50:47.144387 usepy-0.1.46/src/usepy/data/__init__.py
+-rw-r--r--   0        0        0     6773 2023-04-26 05:50:47.144387 usepy-0.1.46/src/usepy/data/_string.py
+-rw-r--r--   0        0        0     5000 2023-04-26 05:50:47.144387 usepy-0.1.46/src/usepy/data/addict.py
+-rw-r--r--   0        0        0     8331 2023-04-26 05:50:47.144387 usepy-0.1.46/src/usepy/data/dict.py
+-rw-r--r--   0        0        0     7116 2023-04-26 05:50:47.144387 usepy-0.1.46/src/usepy/data/list.py
+-rw-r--r--   0        0        0      681 2023-04-26 05:50:47.144387 usepy-0.1.46/src/usepy/decorator/__init__.py
+-rw-r--r--   0        0        0      457 2023-04-26 05:50:47.144387 usepy-0.1.46/src/usepy/decorator/cache.py
+-rw-r--r--   0        0        0      415 2023-04-26 05:50:47.144387 usepy-0.1.46/src/usepy/decorator/catch_error.py
+-rw-r--r--   0        0        0      382 2023-04-26 05:50:47.144387 usepy-0.1.46/src/usepy/decorator/except_debug.py
+-rw-r--r--   0        0        0      416 2023-04-26 05:50:47.144387 usepy-0.1.46/src/usepy/decorator/listify.py
+-rw-r--r--   0        0        0     1879 2023-04-26 05:50:47.144387 usepy-0.1.46/src/usepy/decorator/retry.py
+-rw-r--r--   0        0        0      377 2023-04-26 05:50:47.144387 usepy-0.1.46/src/usepy/decorator/run_in_thread.py
+-rw-r--r--   0        0        0      510 2023-04-26 05:50:47.144387 usepy-0.1.46/src/usepy/decorator/singleton.py
+-rw-r--r--   0        0        0      410 2023-04-26 05:50:47.144387 usepy-0.1.46/src/usepy/decorator/timeit.py
+-rw-r--r--   0        0        0      138 2023-04-26 05:50:47.144387 usepy-0.1.46/src/usepy/parser/__init__.py
+-rw-r--r--   0        0        0     3429 2023-04-26 05:50:47.144387 usepy-0.1.46/src/usepy/parser/curl.py
+-rw-r--r--   0        0        0     1379 2023-04-26 05:50:47.144387 usepy-0.1.46/src/usepy/parser/url.py
+-rw-r--r--   0        0        0      599 2023-04-26 05:50:47.144387 usepy-0.1.46/src/usepy/utils/__init__.py
+-rw-r--r--   0        0        0      677 2023-04-26 05:50:47.144387 usepy-0.1.46/src/usepy/utils/_is.py
+-rw-r--r--   0        0        0     1550 2023-04-26 05:50:47.144387 usepy-0.1.46/src/usepy/utils/_to.py
+-rw-r--r--   0        0        0     1929 2023-04-26 05:50:47.144387 usepy-0.1.46/src/usepy/utils/bloom_filter.py
+-rw-r--r--   0        0        0      307 2023-04-26 05:50:47.144387 usepy-0.1.46/src/usepy/utils/func.py
+-rw-r--r--   0        0        0      879 2023-04-26 05:50:47.144387 usepy-0.1.46/src/usepy/utils/html.py
+-rw-r--r--   0        0        0     1528 2023-04-26 05:50:47.144387 usepy-0.1.46/src/usepy/utils/import_object.py
+-rw-r--r--   0        0        0     4727 2023-04-26 05:50:47.144387 usepy-0.1.46/src/usepy/utils/timer.py
+-rw-r--r--   0        0        0   684816 2023-04-26 05:50:47.144387 usepy-0.1.46/src/usepy/utils/useragent.py
+-rw-r--r--   0        0        0     1406 2023-04-26 05:50:47.144387 usepy-0.1.46/src/usepy/utils/utils.py
+-rw-r--r--   0        0        0     1403 1970-01-01 00:00:00.000000 usepy-0.1.46/PKG-INFO
```

### Comparing `usepy-0.1.45/README.md` & `usepy-0.1.46/README.md`

 * *Files identical despite different names*

### Comparing `usepy-0.1.45/pyproject.toml` & `usepy-0.1.46/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "usepy"
-version = "0.1.45"
+version = "0.1.46"
 description = "usepy"
 homepage = "https://usepy.code05.com/"
 authors = ["miclon <jcnd@163.com>"]
 readme = "README.md"
 packages = [
     { include = 'usepy', from = 'src' }
 ]
```

### Comparing `usepy-0.1.45/src/usepy/__init__.py` & `usepy-0.1.46/src/usepy/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
 # plugins
 try:
     from usepy_notify import useNotify, channels as useNotifyChannels
 except ImportError:
     pass
 try:
-    from usepy_logger import useLogger, useLoggerIntercept, useLoggerInterceptUvicorn
+    from usepy_logger import *
 except ImportError:
     pass
 
 __all__ = [
     # data
     'useDict',
     'useList',
@@ -92,8 +92,10 @@
     # plugins
     'useNotify',
     'useNotifyChannels',
 
     'useLogger',
     'useLoggerIntercept',
     'useLoggerInterceptUvicorn',
+    'useLoggerHandlers',
+    'useLoggerFormatters'
 ]
```

### Comparing `usepy-0.1.45/src/usepy/_datetime.py` & `usepy-0.1.46/src/usepy/_datetime.py`

 * *Files identical despite different names*

### Comparing `usepy-0.1.45/src/usepy/_path.py` & `usepy-0.1.46/src/usepy/_path.py`

 * *Files identical despite different names*

### Comparing `usepy-0.1.45/src/usepy/_thread.py` & `usepy-0.1.46/src/usepy/_thread.py`

 * *Files identical despite different names*

### Comparing `usepy-0.1.45/src/usepy/contrib/pydantic_.py` & `usepy-0.1.46/src/usepy/contrib/pydantic_.py`

 * *Files identical despite different names*

### Comparing `usepy-0.1.45/src/usepy/contrib/tenacity_.py` & `usepy-0.1.46/src/usepy/contrib/tenacity_.py`

 * *Files identical despite different names*

### Comparing `usepy-0.1.45/src/usepy/data/_string.py` & `usepy-0.1.46/src/usepy/data/_string.py`

 * *Files identical despite different names*

### Comparing `usepy-0.1.45/src/usepy/data/addict.py` & `usepy-0.1.46/src/usepy/data/addict.py`

 * *Files identical despite different names*

### Comparing `usepy-0.1.45/src/usepy/data/dict.py` & `usepy-0.1.46/src/usepy/data/dict.py`

 * *Files identical despite different names*

### Comparing `usepy-0.1.45/src/usepy/data/list.py` & `usepy-0.1.46/src/usepy/data/list.py`

 * *Files 6% similar despite different names*

```diff
@@ -195,7 +195,26 @@
         :param fn: 函数
         :return: 最大值
 
         >>> UseList.max_by([{'n': 4}, {'n': 2}, {'n': 8}, {'n': 6}], lambda v: v['n'])
         {'n': 8}
         """
         return max(collection, key=fn)
+
+    @staticmethod
+    def difference(original_list: List, exclude_list: List, fn: Optional[Callable] = None):
+        """
+        求差集
+        :param original_list: 原数组
+        :param exclude_list: 排除数组
+        :param fn: 函数
+        :return: 差集
+
+        >>> UseList.difference([1, 2, 3], [1, 4])
+        [2, 3]
+        >>> UseList.difference([{'a': 1, 'b': 2}, {'a': 2, 'b': 3}], [{'a': 1, 'b': 2}])
+        [{'a': 2, 'b': 3}]
+        >>> UseList.difference([1, 2, 3], [1, 4], fn=lambda x: x ** 2)
+        [3]
+        """
+        fn = fn or (lambda x: x)
+        return [item for item in original_list if fn(item) not in exclude_list]
```

### Comparing `usepy-0.1.45/src/usepy/decorator/__init__.py` & `usepy-0.1.46/src/usepy/decorator/__init__.py`

 * *Files identical despite different names*

### Comparing `usepy-0.1.45/src/usepy/decorator/retry.py` & `usepy-0.1.46/src/usepy/decorator/retry.py`

 * *Files identical despite different names*

### Comparing `usepy-0.1.45/src/usepy/parser/curl.py` & `usepy-0.1.46/src/usepy/parser/curl.py`

 * *Files identical despite different names*

### Comparing `usepy-0.1.45/src/usepy/parser/url.py` & `usepy-0.1.46/src/usepy/parser/url.py`

 * *Files identical despite different names*

### Comparing `usepy-0.1.45/src/usepy/utils/__init__.py` & `usepy-0.1.46/src/usepy/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `usepy-0.1.45/src/usepy/utils/_is.py` & `usepy-0.1.46/src/usepy/utils/_is.py`

 * *Files identical despite different names*

### Comparing `usepy-0.1.45/src/usepy/utils/_to.py` & `usepy-0.1.46/src/usepy/utils/_to.py`

 * *Files identical despite different names*

### Comparing `usepy-0.1.45/src/usepy/utils/bloom_filter.py` & `usepy-0.1.46/src/usepy/utils/bloom_filter.py`

 * *Files identical despite different names*

### Comparing `usepy-0.1.45/src/usepy/utils/html.py` & `usepy-0.1.46/src/usepy/utils/html.py`

 * *Files identical despite different names*

### Comparing `usepy-0.1.45/src/usepy/utils/import_object.py` & `usepy-0.1.46/src/usepy/utils/import_object.py`

 * *Files identical despite different names*

### Comparing `usepy-0.1.45/src/usepy/utils/timer.py` & `usepy-0.1.46/src/usepy/utils/timer.py`

 * *Files identical despite different names*

### Comparing `usepy-0.1.45/src/usepy/utils/useragent.py` & `usepy-0.1.46/src/usepy/utils/useragent.py`

 * *Files identical despite different names*

### Comparing `usepy-0.1.45/src/usepy/utils/utils.py` & `usepy-0.1.46/src/usepy/utils/utils.py`

 * *Files identical despite different names*

### Comparing `usepy-0.1.45/PKG-INFO` & `usepy-0.1.46/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usepy
-Version: 0.1.45
+Version: 0.1.46
 Summary: usepy
 Home-page: https://usepy.code05.com/
 Author: miclon
 Author-email: jcnd@163.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: usepy Version: 0.1.45 Summary: usepy Home-page:
+Metadata-Version: 2.1 Name: usepy Version: 0.1.46 Summary: usepy Home-page:
 https://usepy.code05.com/ Author: miclon Author-email: jcnd@163.com Requires-
 Python: >=3.8,<4.0 Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Provides-Extra: logger Provides-Extra:
 notify Requires-Dist: usepy-plugin-logger (>=0.1.0,<0.2.0) ; extra == "logger"
 Requires-Dist: usepy-plugin-notify (>=0.2.2,<0.3.0) ; extra == "notify"
```

