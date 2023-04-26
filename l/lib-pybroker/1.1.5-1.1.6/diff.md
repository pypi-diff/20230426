# Comparing `tmp/lib-pybroker-1.1.5.tar.gz` & `tmp/lib-pybroker-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib-pybroker-1.1.5.tar", last modified: Wed Apr 26 02:01:56 2023, max compression
+gzip compressed data, was "lib-pybroker-1.1.6.tar", last modified: Wed Apr 26 06:50:02 2023, max compression
```

## Comparing `lib-pybroker-1.1.5.tar` & `lib-pybroker-1.1.6.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 02:01:56.420224 lib-pybroker-1.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)    12318 2023-04-26 02:01:46.000000 lib-pybroker-1.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-26 02:01:46.000000 lib-pybroker-1.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5793 2023-04-26 02:01:56.420224 lib-pybroker-1.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-04-26 02:01:46.000000 lib-pybroker-1.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-26 02:01:46.000000 lib-pybroker-1.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-04-26 02:01:56.420224 lib-pybroker-1.1.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 02:01:56.412224 lib-pybroker-1.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 02:01:56.416224 lib-pybroker-1.1.5/src/lib_pybroker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5793 2023-04-26 02:01:56.000000 lib-pybroker-1.1.5/src/lib_pybroker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-26 02:01:56.000000 lib-pybroker-1.1.5/src/lib_pybroker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 02:01:56.000000 lib-pybroker-1.1.5/src/lib_pybroker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-26 02:01:56.000000 lib-pybroker-1.1.5/src/lib_pybroker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-26 02:01:56.000000 lib-pybroker-1.1.5/src/lib_pybroker.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 02:01:56.416224 lib-pybroker-1.1.5/src/pybroker/
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-04-26 02:01:46.000000 lib-pybroker-1.1.5/src/pybroker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7295 2023-04-26 02:01:46.000000 lib-pybroker-1.1.5/src/pybroker/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     9298 2023-04-26 02:01:46.000000 lib-pybroker-1.1.5/src/pybroker/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-04-26 02:01:46.000000 lib-pybroker-1.1.5/src/pybroker/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    43490 2023-04-26 02:01:46.000000 lib-pybroker-1.1.5/src/pybroker/context.py
--rw-r--r--   0 runner    (1001) docker     (123)    19068 2023-04-26 02:01:46.000000 lib-pybroker-1.1.5/src/pybroker/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    34553 2023-04-26 02:01:46.000000 lib-pybroker-1.1.5/src/pybroker/eval.py
--rw-r--r--   0 runner    (1001) docker     (123)    15385 2023-04-26 02:01:46.000000 lib-pybroker-1.1.5/src/pybroker/indicator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15188 2023-04-26 02:01:46.000000 lib-pybroker-1.1.5/src/pybroker/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    15398 2023-04-26 02:01:46.000000 lib-pybroker-1.1.5/src/pybroker/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    38568 2023-04-26 02:01:46.000000 lib-pybroker-1.1.5/src/pybroker/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 02:01:46.000000 lib-pybroker-1.1.5/src/pybroker/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    25575 2023-04-26 02:01:46.000000 lib-pybroker-1.1.5/src/pybroker/scope.py
--rw-r--r--   0 runner    (1001) docker     (123)    58267 2023-04-26 02:01:46.000000 lib-pybroker-1.1.5/src/pybroker/strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-04-26 02:01:46.000000 lib-pybroker-1.1.5/src/pybroker/vect.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 02:01:56.420224 lib-pybroker-1.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-04-26 02:01:46.000000 lib-pybroker-1.1.5/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-04-26 02:01:46.000000 lib-pybroker-1.1.5/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    21167 2023-04-26 02:01:46.000000 lib-pybroker-1.1.5/tests/test_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    18142 2023-04-26 02:01:46.000000 lib-pybroker-1.1.5/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    18876 2023-04-26 02:01:46.000000 lib-pybroker-1.1.5/tests/test_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-04-26 02:01:46.000000 lib-pybroker-1.1.5/tests/test_indicator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-04-26 02:01:46.000000 lib-pybroker-1.1.5/tests/test_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-04-26 02:01:46.000000 lib-pybroker-1.1.5/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    81106 2023-04-26 02:01:46.000000 lib-pybroker-1.1.5/tests/test_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)    16244 2023-04-26 02:01:46.000000 lib-pybroker-1.1.5/tests/test_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)    72694 2023-04-26 02:01:46.000000 lib-pybroker-1.1.5/tests/test_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-04-26 02:01:46.000000 lib-pybroker-1.1.5/tests/test_vect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:50:02.964577 lib-pybroker-1.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    12318 2023-04-26 06:49:54.000000 lib-pybroker-1.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-26 06:49:54.000000 lib-pybroker-1.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-04-26 06:50:02.964577 lib-pybroker-1.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-04-26 06:49:54.000000 lib-pybroker-1.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-26 06:49:54.000000 lib-pybroker-1.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-04-26 06:50:02.964577 lib-pybroker-1.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:50:02.952577 lib-pybroker-1.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:50:02.956577 lib-pybroker-1.1.6/src/lib_pybroker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-04-26 06:50:02.000000 lib-pybroker-1.1.6/src/lib_pybroker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-26 06:50:02.000000 lib-pybroker-1.1.6/src/lib_pybroker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 06:50:02.000000 lib-pybroker-1.1.6/src/lib_pybroker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-26 06:50:02.000000 lib-pybroker-1.1.6/src/lib_pybroker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-26 06:50:02.000000 lib-pybroker-1.1.6/src/lib_pybroker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:50:02.960577 lib-pybroker-1.1.6/src/pybroker/
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-04-26 06:49:54.000000 lib-pybroker-1.1.6/src/pybroker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7295 2023-04-26 06:49:54.000000 lib-pybroker-1.1.6/src/pybroker/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9298 2023-04-26 06:49:54.000000 lib-pybroker-1.1.6/src/pybroker/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-04-26 06:49:54.000000 lib-pybroker-1.1.6/src/pybroker/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43710 2023-04-26 06:49:54.000000 lib-pybroker-1.1.6/src/pybroker/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19068 2023-04-26 06:49:54.000000 lib-pybroker-1.1.6/src/pybroker/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34553 2023-04-26 06:49:54.000000 lib-pybroker-1.1.6/src/pybroker/eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15385 2023-04-26 06:49:54.000000 lib-pybroker-1.1.6/src/pybroker/indicator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15188 2023-04-26 06:49:54.000000 lib-pybroker-1.1.6/src/pybroker/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15398 2023-04-26 06:49:54.000000 lib-pybroker-1.1.6/src/pybroker/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38568 2023-04-26 06:49:54.000000 lib-pybroker-1.1.6/src/pybroker/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:49:54.000000 lib-pybroker-1.1.6/src/pybroker/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    25656 2023-04-26 06:49:54.000000 lib-pybroker-1.1.6/src/pybroker/scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56921 2023-04-26 06:49:54.000000 lib-pybroker-1.1.6/src/pybroker/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-04-26 06:49:54.000000 lib-pybroker-1.1.6/src/pybroker/vect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:50:02.960577 lib-pybroker-1.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-04-26 06:49:54.000000 lib-pybroker-1.1.6/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-04-26 06:49:54.000000 lib-pybroker-1.1.6/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21421 2023-04-26 06:49:54.000000 lib-pybroker-1.1.6/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18142 2023-04-26 06:49:54.000000 lib-pybroker-1.1.6/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18876 2023-04-26 06:49:54.000000 lib-pybroker-1.1.6/tests/test_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-04-26 06:49:54.000000 lib-pybroker-1.1.6/tests/test_indicator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-04-26 06:49:54.000000 lib-pybroker-1.1.6/tests/test_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-04-26 06:49:54.000000 lib-pybroker-1.1.6/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81106 2023-04-26 06:49:54.000000 lib-pybroker-1.1.6/tests/test_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16301 2023-04-26 06:49:54.000000 lib-pybroker-1.1.6/tests/test_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71227 2023-04-26 06:49:54.000000 lib-pybroker-1.1.6/tests/test_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-04-26 06:49:54.000000 lib-pybroker-1.1.6/tests/test_vect.py
```

### Comparing `lib-pybroker-1.1.5/LICENSE` & `lib-pybroker-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.5/PKG-INFO` & `lib-pybroker-1.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-pybroker
-Version: 1.1.5
+Version: 1.1.6
 Summary: Algorithmic trading with machine learning
 Home-page: http://www.pybroker.com
 Author: Edward West
 Author-email: edwest@pybroker.com
 License: Apache License 2.0 with Commons Clause
 Classifier: License :: Free for non-commercial use
 Description-Content-Type: text/markdown
@@ -119,14 +119,15 @@
 - [Evaluating with Bootstrap Metrics](https://www.pybroker.com/en/latest/notebooks/3.%20Evaluating%20with%20Bootstrap%20Metrics.html)
 - [Ranking and Position Sizing](https://www.pybroker.com/en/latest/notebooks/4.%20Ranking%20and%20Position%20Sizing.html)
 - [Writing Indicators](https://www.pybroker.com/en/latest/notebooks/5.%20Writing%20Indicators.html)
 - [Training a Model](https://www.pybroker.com/en/latest/notebooks/6.%20Training%20a%20Model.html)
 - [Creating a Custom Data Source](https://www.pybroker.com/en/latest/notebooks/7.%20Creating%20a%20Custom%20Data%20Source.html)
 - [Applying Stops](https://www.pybroker.com/en/latest/notebooks/8.%20Applying%20Stops.html)
 - [Rebalancing Positions](https://www.pybroker.com/en/latest/notebooks/9.%20Rebalancing%20Positions.html)
+- [Rotational Trading](https://www.pybroker.com/en/latest/notebooks/10.%20Rotational%20Trading.html)
 - [FAQs](https://www.pybroker.com/en/latest/notebooks/FAQs.html)
 
 ## Online Documentation
 
 [The full reference documentation is hosted at **www.pybroker.com**.](https://www.pybroker.com)
 
 ## Contact
```

### Comparing `lib-pybroker-1.1.5/README.md` & `lib-pybroker-1.1.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -107,14 +107,15 @@
 - [Evaluating with Bootstrap Metrics](https://www.pybroker.com/en/latest/notebooks/3.%20Evaluating%20with%20Bootstrap%20Metrics.html)
 - [Ranking and Position Sizing](https://www.pybroker.com/en/latest/notebooks/4.%20Ranking%20and%20Position%20Sizing.html)
 - [Writing Indicators](https://www.pybroker.com/en/latest/notebooks/5.%20Writing%20Indicators.html)
 - [Training a Model](https://www.pybroker.com/en/latest/notebooks/6.%20Training%20a%20Model.html)
 - [Creating a Custom Data Source](https://www.pybroker.com/en/latest/notebooks/7.%20Creating%20a%20Custom%20Data%20Source.html)
 - [Applying Stops](https://www.pybroker.com/en/latest/notebooks/8.%20Applying%20Stops.html)
 - [Rebalancing Positions](https://www.pybroker.com/en/latest/notebooks/9.%20Rebalancing%20Positions.html)
+- [Rotational Trading](https://www.pybroker.com/en/latest/notebooks/10.%20Rotational%20Trading.html)
 - [FAQs](https://www.pybroker.com/en/latest/notebooks/FAQs.html)
 
 ## Online Documentation
 
 [The full reference documentation is hosted at **www.pybroker.com**.](https://www.pybroker.com)
 
 ## Contact
```

### Comparing `lib-pybroker-1.1.5/setup.cfg` & `lib-pybroker-1.1.6/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = lib-pybroker
-version = 1.1.5
+version = 1.1.6
 url = http://www.pybroker.com
 author = Edward West
 author_email = edwest@pybroker.com
 description = Algorithmic trading with machine learning
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = Apache License 2.0 with Commons Clause
```

### Comparing `lib-pybroker-1.1.5/src/lib_pybroker.egg-info/PKG-INFO` & `lib-pybroker-1.1.6/src/lib_pybroker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-pybroker
-Version: 1.1.5
+Version: 1.1.6
 Summary: Algorithmic trading with machine learning
 Home-page: http://www.pybroker.com
 Author: Edward West
 Author-email: edwest@pybroker.com
 License: Apache License 2.0 with Commons Clause
 Classifier: License :: Free for non-commercial use
 Description-Content-Type: text/markdown
@@ -119,14 +119,15 @@
 - [Evaluating with Bootstrap Metrics](https://www.pybroker.com/en/latest/notebooks/3.%20Evaluating%20with%20Bootstrap%20Metrics.html)
 - [Ranking and Position Sizing](https://www.pybroker.com/en/latest/notebooks/4.%20Ranking%20and%20Position%20Sizing.html)
 - [Writing Indicators](https://www.pybroker.com/en/latest/notebooks/5.%20Writing%20Indicators.html)
 - [Training a Model](https://www.pybroker.com/en/latest/notebooks/6.%20Training%20a%20Model.html)
 - [Creating a Custom Data Source](https://www.pybroker.com/en/latest/notebooks/7.%20Creating%20a%20Custom%20Data%20Source.html)
 - [Applying Stops](https://www.pybroker.com/en/latest/notebooks/8.%20Applying%20Stops.html)
 - [Rebalancing Positions](https://www.pybroker.com/en/latest/notebooks/9.%20Rebalancing%20Positions.html)
+- [Rotational Trading](https://www.pybroker.com/en/latest/notebooks/10.%20Rotational%20Trading.html)
 - [FAQs](https://www.pybroker.com/en/latest/notebooks/FAQs.html)
 
 ## Online Documentation
 
 [The full reference documentation is hosted at **www.pybroker.com**.](https://www.pybroker.com)
 
 ## Contact
```

### Comparing `lib-pybroker-1.1.5/src/lib_pybroker.egg-info/SOURCES.txt` & `lib-pybroker-1.1.6/src/lib_pybroker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.5/src/pybroker/__init__.py` & `lib-pybroker-1.1.6/src/pybroker/__init__.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.5/src/pybroker/cache.py` & `lib-pybroker-1.1.6/src/pybroker/cache.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.5/src/pybroker/common.py` & `lib-pybroker-1.1.6/src/pybroker/common.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.5/src/pybroker/config.py` & `lib-pybroker-1.1.6/src/pybroker/config.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.5/src/pybroker/context.py` & `lib-pybroker-1.1.6/src/pybroker/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     DataCol,
     ModelSymbol,
     PriceType,
     StopType,
     to_datetime,
     to_decimal,
 )
+from .config import StrategyConfig
 from .model import TrainedModel
 from .portfolio import Entry, Order, Portfolio, Position, Stop, Trade
 from .scope import (
     ColumnScope,
     IndicatorScope,
     ModelInputScope,
     PendingOrder,
@@ -52,27 +53,33 @@
     NamedTuple,
     Optional,
     Union,
 )
 
 
 class BaseContext:
-    """Base context class."""
+    """Base context class.
+
+    Attributes:
+        config: :class:`pybroker.config.StrategyConfig`.
+    """
 
     def __init__(
         self,
+        config: StrategyConfig,
         portfolio: Portfolio,
         col_scope: ColumnScope,
         ind_scope: IndicatorScope,
         input_scope: ModelInputScope,
         pred_scope: PredictionScope,
         pending_order_scope: PendingOrderScope,
         models: Mapping[ModelSymbol, TrainedModel],
         sym_end_index: Mapping[str, int],
     ):
+        self.config = config
         self._portfolio = portfolio
         self._col_scope = col_scope
         self._ind_scope = ind_scope
         self._input_scope = input_scope
         self._pred_scope = pred_scope
         self._models = models
         self._sym_end_index = sym_end_index
@@ -407,42 +414,42 @@
 
     Attributes:
         sessions: ``dict`` used to store custom data for all symbols.
     """
 
     def __init__(
         self,
+        config: StrategyConfig,
         portfolio: Portfolio,
         col_scope: ColumnScope,
         ind_scope: IndicatorScope,
         input_scope: ModelInputScope,
         pred_scope: PredictionScope,
         pending_order_scope: PendingOrderScope,
         models: Mapping[ModelSymbol, TrainedModel],
         sessions: Mapping[str, Mapping],
         sym_end_index: Mapping[str, int],
-        max_long_positions: Optional[int],
-        max_short_positions: Optional[int],
     ):
         super().__init__(
+            config=config,
             portfolio=portfolio,
             col_scope=col_scope,
             ind_scope=ind_scope,
             input_scope=input_scope,
             pred_scope=pred_scope,
             pending_order_scope=pending_order_scope,
             models=models,
             sym_end_index=sym_end_index,
         )
         self.sessions = sessions
         self._signal_shares: dict[int, Union[int, float, Decimal]] = {}
         self._buy_results: Optional[list[ExecResult]] = None
         self._sell_results: Optional[list[ExecResult]] = None
-        self._max_long_positions = max_long_positions
-        self._max_short_positions = max_short_positions
+        self._max_long_positions = config.max_long_positions
+        self._max_short_positions = config.max_short_positions
 
     def signals(
         self, signal_type: Optional[Literal["buy", "sell"]] = None
     ) -> Iterator[ExecSignal]:
         r"""Returns :class:`Iterator` of :class:`.ExecSignal`\ s containing
         data for buy and sell signals.
         """
@@ -579,25 +586,27 @@
     """
 
     _stop_id: int = 0
 
     def __init__(
         self,
         symbol: str,
+        config: StrategyConfig,
         portfolio: Portfolio,
         col_scope: ColumnScope,
         ind_scope: IndicatorScope,
         input_scope: ModelInputScope,
         pred_scope: PredictionScope,
         pending_order_scope: PendingOrderScope,
         models: Mapping[ModelSymbol, TrainedModel],
         sym_end_index: Mapping[str, int],
         session: Mapping,
     ):
         super().__init__(
+            config=config,
             portfolio=portfolio,
             col_scope=col_scope,
             ind_scope=ind_scope,
             input_scope=input_scope,
             pred_scope=pred_scope,
             pending_order_scope=pending_order_scope,
             models=models,
```

### Comparing `lib-pybroker-1.1.5/src/pybroker/data.py` & `lib-pybroker-1.1.6/src/pybroker/data.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.5/src/pybroker/eval.py` & `lib-pybroker-1.1.6/src/pybroker/eval.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.5/src/pybroker/indicator.py` & `lib-pybroker-1.1.6/src/pybroker/indicator.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.5/src/pybroker/log.py` & `lib-pybroker-1.1.6/src/pybroker/log.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.5/src/pybroker/model.py` & `lib-pybroker-1.1.6/src/pybroker/model.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.5/src/pybroker/portfolio.py` & `lib-pybroker-1.1.6/src/pybroker/portfolio.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.5/src/pybroker/scope.py` & `lib-pybroker-1.1.6/src/pybroker/scope.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,23 +33,26 @@
 from decimal import Decimal
 from diskcache import Cache
 from numpy.typing import NDArray
 from typing import (
     Any,
     Callable,
     Collection,
+    Final,
     Iterable,
     Literal,
     Mapping,
     NamedTuple,
     Optional,
     Sequence,
     Union,
 )
 
+_EMPTY_PARAM: Final = object()
+
 
 class StaticScope:
     """A static registry of data and object references.
 
     Attributes:
         logger: :class:`pybroker.log.Logger`
         data_source_cache: :class:`diskcache.Cache` that stores data retrieved
@@ -170,17 +173,19 @@
 
     def unfreeze_data_cols(self):
         """Allows additional data columns to be registered if
         :func:`pybroker.scope.StaticScope.freeze_data_cols` was called.
         """
         self._cols_frozen = False
 
-    def param(self, name: str, value: Optional[Any] = None) -> Optional[Any]:
+    def param(
+        self, name: str, value: Optional[Any] = _EMPTY_PARAM
+    ) -> Optional[Any]:
         """Get or set a global parameter."""
-        if value is None:
+        if value == _EMPTY_PARAM:
             return self._params.get(name, None)
         self._params[name] = value
         return value
 
     @classmethod
     def instance(cls) -> "StaticScope":
         """Returns singleton instance."""
@@ -215,15 +220,15 @@
 
 
 def unregister_columns(names: Union[str, Iterable[str]], *args):
     """Unregisters ``names`` of user-defined data columns."""
     StaticScope.instance().unregister_custom_cols(names, *args)
 
 
-def param(name: str, value: Optional[Any] = None) -> Optional[Any]:
+def param(name: str, value: Optional[Any] = _EMPTY_PARAM) -> Optional[Any]:
     """Get or set a global parameter."""
     return StaticScope.instance().param(name, value)
 
 
 class ColumnScope:
     """Caches and retrieves column data queried from :class:`pandas.DataFrame`.
```

### Comparing `lib-pybroker-1.1.5/src/pybroker/strategy.py` & `lib-pybroker-1.1.6/src/pybroker/strategy.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,66 +109,47 @@
 
 
 class BacktestMixin:
     """Mixin implementing backtesting functionality."""
 
     def backtest_executions(
         self,
+        config: StrategyConfig,
         executions: set[Execution],
         before_exec_fn: Optional[Callable[[Mapping[str, ExecContext]], None]],
         after_exec_fn: Optional[Callable[[Mapping[str, ExecContext]], None]],
         sessions: Mapping[str, Mapping],
         models: Mapping[ModelSymbol, TrainedModel],
         indicator_data: Mapping[IndicatorSymbol, pd.Series],
         test_data: pd.DataFrame,
         portfolio: Portfolio,
-        buy_delay: int,
-        sell_delay: int,
-        max_long_positions: Optional[int],
-        max_short_positions: Optional[int],
         pos_size_handler: Optional[Callable[[PosSizeContext], None]],
         exit_dates: Mapping[str, np.datetime64],
-        exit_buy_fill_price: Union[
-            PriceType, Callable[[str, BarData], Union[int, float, Decimal]]
-        ] = PriceType.MIDDLE,
-        exit_sell_fill_price: Union[
-            PriceType, Callable[[str, BarData], Union[int, float, Decimal]]
-        ] = PriceType.MIDDLE,
         enable_fractional_shares: bool = False,
     ):
         r"""Backtests a ``set`` of :class:`.Execution`\ s that implement
         trading logic.
 
         Args:
+            config: :class:`pybroker.config.StrategyConfig`.
             executions: :class:`.Execution`\ s to run.
             sessions: :class:`Mapping` of symbols to :class:`Mapping` of custom
                 data that persists for every bar during the
                 :class:`.Execution`.
             models: :class:`Mapping` of :class:`pybroker.common.ModelSymbol`
                 pairs to :class:`pybroker.common.TrainedModel`\ s.
             indicator_data: :class:`Mapping` of
                 :class:`pybroker.common.IndicatorSymbol` pairs to
                 :class:`pandas.Series` of :class:`pybroker.indicator.Indicator`
                 values.
             test_data: :class:`pandas.DataFrame` of test data.
             portfolio: :class:`pybroker.portfolio.Portfolio`.
-            buy_delay: Number of bars before placing an order for a buy signal.
-            sell_delay: Number of bars before placing an order for a sell
-                signal.
-            max_long_positions: Maximum number of long positions that can be
-                held at a time. If ``None``, then unlimited.
-            max_short_positions: Maximum number of short positions that can be
-                held at a time. If ``None``, then unlimited.
             pos_size_handler: :class:`Callable` that sets position sizes when
                 placing orders for buy and sell signals.
             exit_dates: :class:`Mapping` of symbols to exit dates.
-            exit_buy_fill_price: Fill price for covering an open short position
-                for ``exit_dates``.
-            exit_sell_fill_price: Fill price for selling an open long position
-                for ``exit_dates``.
             enable_fractional_shares: Whether to enable trading fractional
                 shares.
 
         Returns:
             :class:`.TestResult` of the backtest.
         """
         test_dates = test_data[DataCol.DATE.value].unique()
@@ -190,14 +171,15 @@
         exec_fns: dict[str, Callable[[ExecContext], None]] = {}
         for sym in test_syms:
             for exec in executions:
                 if sym not in exec.symbols:
                     continue
                 exec_ctxs[sym] = ExecContext(
                     symbol=sym,
+                    config=config,
                     portfolio=portfolio,
                     col_scope=col_scope,
                     ind_scope=ind_scope,
                     input_scope=input_scope,
                     pred_scope=pred_scope,
                     pending_order_scope=pending_order_scope,
                     models=models,
@@ -210,25 +192,24 @@
             sym: frozenset(test_data.loc[pd.IndexSlice[sym, :]].index.values)
             for sym in exec_ctxs.keys()
         }
         buy_sched: dict[np.datetime64, list[ExecResult]] = defaultdict(list)
         sell_sched: dict[np.datetime64, list[ExecResult]] = defaultdict(list)
         if pos_size_handler is not None:
             pos_ctx = PosSizeContext(
+                config=config,
                 portfolio=portfolio,
                 col_scope=col_scope,
                 ind_scope=ind_scope,
                 input_scope=input_scope,
                 pred_scope=pred_scope,
                 pending_order_scope=pending_order_scope,
                 models=models,
                 sessions=sessions,
                 sym_end_index=sym_end_index,
-                max_long_positions=max_long_positions,
-                max_short_positions=max_short_positions,
             )
         logger = StaticScope.instance().logger
         logger.backtest_executions_start(test_dates)
         buy_results: deque[ExecResult] = deque()
         sell_results: deque[ExecResult] = deque()
         exit_syms: deque[str] = deque()
         active_ctxs: dict[str, ExecContext] = {}
@@ -245,19 +226,21 @@
                     and sym in exit_dates
                     and date == exit_dates[sym]
                 ):
                     exit_syms.append(sym)
             is_buy_sched = date in buy_sched
             is_sell_sched = date in sell_sched
             if is_buy_sched and (
-                max_long_positions is not None or pos_size_handler is not None
+                config.max_long_positions is not None
+                or pos_size_handler is not None
             ):
                 buy_sched[date].sort(key=_sort_by_score, reverse=True)
             if is_sell_sched and (
-                max_short_positions is not None or pos_size_handler is not None
+                config.max_short_positions is not None
+                or pos_size_handler is not None
             ):
                 sell_sched[date].sort(key=_sort_by_score, reverse=True)
             if pos_size_handler is not None and (
                 is_buy_sched or is_sell_sched
             ):
                 self._set_pos_sizes(
                     pos_size_handler=pos_size_handler,
@@ -301,36 +284,36 @@
                 if result.sell_shares is not None:
                     sell_results.append(result)
             while buy_results:
                 self._schedule_order(
                     result=buy_results.popleft(),
                     created=date,
                     sym_end_index=sym_end_index,
-                    delay=buy_delay,
+                    delay=config.buy_delay,
                     sched=buy_sched,
                     col_scope=col_scope,
                     pending_order_scope=pending_order_scope,
                 )
             while sell_results:
                 self._schedule_order(
                     result=sell_results.popleft(),
                     created=date,
                     sym_end_index=sym_end_index,
-                    delay=sell_delay,
+                    delay=config.sell_delay,
                     sched=sell_sched,
                     col_scope=col_scope,
                     pending_order_scope=pending_order_scope,
                 )
             while exit_syms:
                 self._exit_position(
                     portfolio=portfolio,
                     date=date,
                     symbol=exit_syms.popleft(),
-                    exit_buy_fill_price=exit_buy_fill_price,
-                    exit_sell_fill_price=exit_sell_fill_price,
+                    exit_cover_fill_price=config.exit_cover_fill_price,
+                    exit_sell_fill_price=config.exit_sell_fill_price,
                     price_scope=price_scope,
                 )
             portfolio.incr_bars()
             if i % 10 == 0 or i == len(test_dates) - 1:
                 logger.backtest_executions_loading(i + 1)
 
     def _to_result(self, ctx: ExecContext) -> Optional[ExecResult]:
@@ -352,23 +335,23 @@
         return ctx.to_result()
 
     def _exit_position(
         self,
         portfolio: Portfolio,
         date: np.datetime64,
         symbol: str,
-        exit_buy_fill_price: Union[
+        exit_cover_fill_price: Union[
             PriceType, Callable[[str, BarData], Union[int, float, Decimal]]
         ],
         exit_sell_fill_price: Union[
             PriceType, Callable[[str, BarData], Union[int, float, Decimal]]
         ],
         price_scope: PriceScope,
     ):
-        buy_fill_price = price_scope.fetch(symbol, exit_buy_fill_price)
+        buy_fill_price = price_scope.fetch(symbol, exit_cover_fill_price)
         sell_fill_price = price_scope.fetch(symbol, exit_sell_fill_price)
         portfolio.exit_position(
             date,
             symbol,
             buy_fill_price=buy_fill_price,
             sell_fill_price=sell_fill_price,
         )
@@ -1277,31 +1260,26 @@
                         tf_seconds=tf_seconds,
                         between_time=between_time,
                         days=days,
                     ),
                 )
             if not train_only and not test_data.empty:
                 self.backtest_executions(
+                    config=self._config,
                     executions=self._executions,
                     before_exec_fn=self._before_exec_fn,
                     after_exec_fn=self._after_exec_fn,
                     sessions=sessions,
                     models=models,
                     indicator_data=indicator_data,
                     test_data=test_data,
                     portfolio=portfolio,
-                    buy_delay=self._config.buy_delay,
-                    sell_delay=self._config.sell_delay,
-                    max_long_positions=self._config.max_long_positions,
-                    max_short_positions=self._config.max_short_positions,
                     pos_size_handler=self._pos_size_handler,
                     exit_dates=exit_dates,
                     enable_fractional_shares=self._fractional_shares_enabled(),
-                    exit_buy_fill_price=self._config.exit_cover_fill_price,
-                    exit_sell_fill_price=self._config.exit_sell_fill_price,
                 )
 
     def _filter_dates(
         self,
         df: pd.DataFrame,
         start_date: datetime,
         end_date: datetime,
```

### Comparing `lib-pybroker-1.1.5/src/pybroker/vect.py` & `lib-pybroker-1.1.6/src/pybroker/vect.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.5/tests/test_cache.py` & `lib-pybroker-1.1.6/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.5/tests/test_common.py` & `lib-pybroker-1.1.6/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.5/tests/test_context.py` & `lib-pybroker-1.1.6/tests/test_context.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 import numpy as np
 import pytest
 import re
 from .fixtures import *
 from collections import deque
 from decimal import Decimal
 from pybroker.common import PriceType, StopType, to_datetime
+from pybroker.config import StrategyConfig
 from pybroker.context import (
     ExecContext,
     ExecResult,
     PosSizeContext,
     set_exec_ctx_data,
     set_pos_size_ctx_data,
 )
@@ -120,14 +121,15 @@
     sym_end_index,
     session,
     symbol,
     date,
 ):
     ctx = ExecContext(
         symbol=symbol,
+        config=StrategyConfig(max_long_positions=5),
         portfolio=portfolio,
         col_scope=col_scope,
         ind_scope=ind_scope,
         input_scope=input_scope,
         pred_scope=pred_scope,
         pending_order_scope=pending_order_scope,
         models=trained_models,
@@ -157,14 +159,15 @@
         sym: Position(sym, 200, "long") for sym in symbols
     }
     portfolio.short_positions = {
         sym: Position(sym, 100, "short") for sym in symbols
     }
     ctx = ExecContext(
         symbol=symbol,
+        config=StrategyConfig(max_long_positions=5),
         portfolio=portfolio,
         col_scope=col_scope,
         ind_scope=ind_scope,
         input_scope=input_scope,
         pred_scope=pred_scope,
         pending_order_scope=pending_order_scope,
         models=trained_models,
@@ -193,28 +196,33 @@
 ):
     portfolio.orders = deque(orders)
     portfolio.trades = deque(trades)
     portfolio.win_rate = 1
     portfolio.lose_rate = 0
     ctx = ExecContext(
         symbol=symbol,
+        config=StrategyConfig(max_long_positions=5),
         portfolio=portfolio,
         col_scope=col_scope,
         ind_scope=ind_scope,
         input_scope=input_scope,
         pred_scope=pred_scope,
         pending_order_scope=pending_order_scope,
         models=trained_models,
         sym_end_index=sym_end_index,
         session=session,
     )
     set_exec_ctx_data(ctx, date)
     return ctx
 
 
+def test_config(ctx):
+    assert ctx.config.max_long_positions == 5
+
+
 def test_dt(ctx, date):
     assert ctx.dt == to_datetime(date)
 
 
 def test_win_rate(ctx_with_orders):
     assert ctx_with_orders.win_rate == 1
 
@@ -689,25 +697,24 @@
             score=1,
             long_stops=None,
             short_stops=None,
         ),
     ]
     sessions = {"SPY": {}, "AAPL": {}, "TSLA": {"foo": 1}}
     ctx = PosSizeContext(
+        StrategyConfig(max_long_positions=1),
         portfolio,
         col_scope,
         ind_scope,
         input_scope,
         pred_scope,
         pending_order_scope,
         trained_models,
         sessions,
         sym_end_index,
-        max_long_positions=1,
-        max_short_positions=None,
     )
     set_pos_size_ctx_data(ctx, buy_results, sell_results)
     assert ctx.sessions == sessions
     buy_signals = list(ctx.signals("buy"))
     assert len(buy_signals) == 1
     assert buy_signals[0].id == 0
     assert buy_signals[0].symbol == "SPY"
```

### Comparing `lib-pybroker-1.1.5/tests/test_data.py` & `lib-pybroker-1.1.6/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.5/tests/test_eval.py` & `lib-pybroker-1.1.6/tests/test_eval.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.5/tests/test_indicator.py` & `lib-pybroker-1.1.6/tests/test_indicator.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.5/tests/test_log.py` & `lib-pybroker-1.1.6/tests/test_log.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.5/tests/test_model.py` & `lib-pybroker-1.1.6/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.5/tests/test_portfolio.py` & `lib-pybroker-1.1.6/tests/test_portfolio.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.5/tests/test_scope.py` & `lib-pybroker-1.1.6/tests/test_scope.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,17 +109,18 @@
     mock_logger.disable_progress_bar.assert_called_once()
 
 
 def test_param_when_empty():
     assert param("bar") is None
 
 
-def test_param_when_set_and_get():
-    param("foo", 42)
-    assert param("foo") == 42
+@pytest.mark.parametrize("value", [42, None])
+def test_param_when_set_and_get(value):
+    param("foo", value)
+    assert param("foo") == value
 
 
 class TestStaticScope:
     def test_set_and_get_indicator(self, scope, hhv_ind):
         scope.set_indicator(hhv_ind)
         assert scope.has_indicator(hhv_ind.name)
         assert scope.get_indicator(hhv_ind.name) == hhv_ind
```

### Comparing `lib-pybroker-1.1.5/tests/test_strategy.py` & `lib-pybroker-1.1.6/tests/test_strategy.py`

 * *Files 3% similar despite different names*

```diff
@@ -194,26 +194,23 @@
             model_names=frozenset(),
             indicator_names=frozenset(),
         )
         execs = {buy_exec, sell_exec}
         mock_portfolio = Mock()
         mixin = BacktestMixin()
         mixin.backtest_executions(
+            config=StrategyConfig(),
             executions=execs,
             before_exec_fn=None,
             after_exec_fn=None,
             sessions=defaultdict(dict),
             models={},
             indicator_data={},
             test_data=data_source_df,
             portfolio=mock_portfolio,
-            buy_delay=1,
-            sell_delay=1,
-            max_long_positions=None,
-            max_short_positions=None,
             pos_size_handler=pos_size_handler,
             exit_dates={},
         )
         buy_df = data_source_df[data_source_df["symbol"] == "SPY"]
         buy_dates = buy_df["date"].unique()[1:]
         assert len(mock_portfolio.buy.call_args_list) == len(buy_dates)
         for i, date in enumerate(buy_dates):
@@ -251,26 +248,23 @@
             model_names=frozenset(),
             indicator_names=frozenset(),
         )
         execs = {buy_exec}
         mock_portfolio = Mock()
         mixin = BacktestMixin()
         mixin.backtest_executions(
+            config=StrategyConfig(buy_delay=2),
             executions=execs,
             before_exec_fn=None,
             after_exec_fn=None,
             sessions=defaultdict(dict),
             models={},
             indicator_data={},
             test_data=data_source_df,
             portfolio=mock_portfolio,
-            buy_delay=2,
-            sell_delay=1,
-            max_long_positions=None,
-            max_short_positions=None,
             pos_size_handler=None,
             exit_dates={},
         )
         buy_df = data_source_df[data_source_df["symbol"] == "SPY"]
         buy_dates = buy_df["date"].unique()[2:]
         assert len(mock_portfolio.buy.call_args_list) == len(buy_dates)
         for i, date in enumerate(buy_dates):
@@ -296,26 +290,23 @@
             model_names=frozenset(),
             indicator_names=frozenset(),
         )
         execs = {sell_exec}
         mock_portfolio = Mock()
         mixin = BacktestMixin()
         mixin.backtest_executions(
+            config=StrategyConfig(sell_delay=2),
             executions=execs,
             before_exec_fn=None,
             after_exec_fn=None,
             sessions=defaultdict(dict),
             models={},
             indicator_data={},
             test_data=data_source_df,
             portfolio=mock_portfolio,
-            buy_delay=1,
-            sell_delay=2,
-            max_long_positions=None,
-            max_short_positions=None,
             pos_size_handler=None,
             exit_dates={},
         )
         sell_df = data_source_df[data_source_df["symbol"] == "AAPL"]
         sell_dates = sell_df["date"].unique()[2:]
         assert len(mock_portfolio.sell.call_args_list) == len(sell_dates)
         for i, date in enumerate(sell_dates):
@@ -344,26 +335,23 @@
         )
         execs = {buy_exec}
         mixin = BacktestMixin()
         with pytest.raises(
             ValueError, match=re.escape("hold_bars must be greater than 0.")
         ):
             mixin.backtest_executions(
+                config=StrategyConfig(),
                 executions=execs,
                 before_exec_fn=None,
                 after_exec_fn=None,
                 sessions=defaultdict(dict),
                 models={},
                 indicator_data={},
                 test_data=data_source_df,
                 portfolio=Mock(),
-                buy_delay=1,
-                sell_delay=1,
-                max_long_positions=None,
-                max_short_positions=None,
                 pos_size_handler=None,
                 exit_dates={},
             )
 
     def test_backtest_executions_when_invalid_sell_hold_bars_then_error(
         self, data_source_df
     ):
@@ -380,26 +368,23 @@
         )
         execs = {sell_exec}
         mixin = BacktestMixin()
         with pytest.raises(
             ValueError, match=re.escape("hold_bars must be greater than 0.")
         ):
             mixin.backtest_executions(
+                config=StrategyConfig(),
                 executions=execs,
                 before_exec_fn=None,
                 after_exec_fn=None,
                 sessions=defaultdict(dict),
                 models={},
                 indicator_data={},
                 test_data=data_source_df,
                 portfolio=Mock(),
-                buy_delay=1,
-                sell_delay=1,
-                max_long_positions=None,
-                max_short_positions=None,
                 pos_size_handler=None,
                 exit_dates={},
             )
 
     def test_backtest_executions_when_no_fn(self, data_source_df):
         exec = Execution(
             id=1,
@@ -408,26 +393,23 @@
             model_names=frozenset(),
             indicator_names=frozenset(),
         )
         execs = {exec}
         portfolio = Portfolio(100_000)
         mixin = BacktestMixin()
         mixin.backtest_executions(
+            config=StrategyConfig(),
             executions=execs,
             before_exec_fn=None,
             after_exec_fn=None,
             sessions=defaultdict(dict),
             models={},
             indicator_data={},
             test_data=data_source_df,
             portfolio=portfolio,
-            buy_delay=1,
-            sell_delay=1,
-            max_long_positions=None,
-            max_short_positions=None,
             pos_size_handler=None,
             exit_dates={},
         )
         assert len(portfolio.bars) == len(data_source_df["date"].unique())
         assert not len(portfolio.position_bars)
         assert not len(portfolio.orders)
         assert not len(portfolio.trades)
@@ -443,26 +425,23 @@
             model_names=frozenset(),
             indicator_names=frozenset(),
         )
         execs = {exec}
         portfolio = Portfolio(100_000)
         mixin = BacktestMixin()
         mixin.backtest_executions(
+            config=StrategyConfig(),
             executions=execs,
             before_exec_fn=None,
             after_exec_fn=None,
             sessions=defaultdict(dict),
             models={},
             indicator_data={},
             test_data=data_source_df[data_source_df["symbol"] != "AAPL"],
             portfolio=portfolio,
-            buy_delay=1,
-            sell_delay=1,
-            max_long_positions=None,
-            max_short_positions=None,
             pos_size_handler=None,
             exit_dates={},
         )
         assert len(portfolio.bars) == len(data_source_df["date"].unique())
         assert not len(portfolio.position_bars)
         assert not len(portfolio.orders)
         assert not len(portfolio.trades)
@@ -480,26 +459,23 @@
             model_names=frozenset(),
             indicator_names=frozenset(),
         )
         execs = {exec}
         portfolio = Portfolio(100_000)
         mixin = BacktestMixin()
         mixin.backtest_executions(
+            config=StrategyConfig(buy_delay=1_000),
             executions=execs,
             before_exec_fn=None,
             after_exec_fn=None,
             sessions=defaultdict(dict),
             models={},
             indicator_data={},
             test_data=data_source_df,
             portfolio=portfolio,
-            buy_delay=1000,
-            sell_delay=1,
-            max_long_positions=None,
-            max_short_positions=None,
             pos_size_handler=None,
             exit_dates={},
         )
 
         assert len(portfolio.bars) == len(data_source_df["date"].unique())
         assert not len(portfolio.position_bars)
         assert not len(portfolio.orders)
@@ -518,26 +494,23 @@
             model_names=frozenset(),
             indicator_names=frozenset(),
         )
         execs = {exec}
         portfolio = Portfolio(100_000)
         mixin = BacktestMixin()
         mixin.backtest_executions(
+            config=StrategyConfig(sell_delay=1000),
             executions=execs,
             before_exec_fn=None,
             after_exec_fn=None,
             sessions=defaultdict(dict),
             models={},
             indicator_data={},
             test_data=data_source_df,
             portfolio=portfolio,
-            buy_delay=1,
-            sell_delay=1000,
-            max_long_positions=None,
-            max_short_positions=None,
             pos_size_handler=None,
             exit_dates={},
         )
         assert len(portfolio.bars)
         assert not len(portfolio.position_bars)
         assert not len(portfolio.orders)
         assert not len(portfolio.trades)
@@ -558,26 +531,23 @@
             model_names=frozenset(),
             indicator_names=frozenset(),
         )
         execs = {exec}
         mock_portfolio = Mock()
         mixin = BacktestMixin()
         mixin.backtest_executions(
+            config=StrategyConfig(max_long_positions=1),
             executions=execs,
             before_exec_fn=None,
             after_exec_fn=None,
             sessions=defaultdict(dict),
             models={},
             indicator_data={},
             test_data=data_source_df,
             portfolio=mock_portfolio,
-            buy_delay=1,
-            sell_delay=1,
-            max_long_positions=1,
-            max_short_positions=None,
             pos_size_handler=None,
             exit_dates={},
         )
         df = data_source_df[data_source_df["symbol"].isin(["AAPL", "SPY"])]
         buy_dates = sorted(df["date"].values)[2:]
         assert len(mock_portfolio.buy.call_args_list) == len(buy_dates)
         for i, date in enumerate(buy_dates):
@@ -611,26 +581,23 @@
             model_names=frozenset(),
             indicator_names=frozenset(),
         )
         execs = {exec}
         mock_portfolio = Mock()
         mixin = BacktestMixin()
         mixin.backtest_executions(
+            config=StrategyConfig(max_short_positions=1),
             executions=execs,
             before_exec_fn=None,
             after_exec_fn=None,
             sessions=defaultdict(dict),
             models={},
             indicator_data={},
             test_data=data_source_df,
             portfolio=mock_portfolio,
-            buy_delay=1,
-            sell_delay=1,
-            max_long_positions=None,
-            max_short_positions=1,
             pos_size_handler=None,
             exit_dates={},
         )
         df = data_source_df[data_source_df["symbol"].isin(["AAPL", "SPY"])]
         sell_dates = sorted(df["date"].values)[2:]
         assert len(mock_portfolio.sell.call_args_list) == len(sell_dates)
         for i, date in enumerate(sell_dates):
@@ -689,26 +656,23 @@
             model_names=frozenset(),
             indicator_names=frozenset(),
         )
         execs = {exec}
         mock_portfolio = Mock()
         mixin = BacktestMixin()
         mixin.backtest_executions(
+            config=StrategyConfig(),
             executions=execs,
             before_exec_fn=None,
             after_exec_fn=None,
             sessions=defaultdict(dict),
             models={},
             indicator_data={},
             test_data=df,
             portfolio=mock_portfolio,
-            buy_delay=1,
-            sell_delay=1,
-            max_long_positions=None,
-            max_short_positions=None,
             pos_size_handler=None,
             exit_dates={},
         )
         buy_dates = dates[1:]
         assert len(mock_portfolio.buy.call_args_list) == len(buy_dates)
         for i, date in enumerate(buy_dates):
             _, kwargs = mock_portfolio.buy.call_args_list[i]
@@ -732,26 +696,23 @@
             model_names=frozenset(),
             indicator_names=frozenset(),
         )
         execs = {exec}
         mixin = BacktestMixin()
         with pytest.raises(ValueError, match=r"Unknown price: .*"):
             mixin.backtest_executions(
+                config=StrategyConfig(),
                 executions=execs,
                 before_exec_fn=None,
                 after_exec_fn=None,
                 sessions=defaultdict(dict),
                 models={},
                 indicator_data={},
                 test_data=data_source_df,
                 portfolio=Portfolio(100_000),
-                buy_delay=1,
-                sell_delay=1,
-                max_long_positions=None,
-                max_short_positions=None,
                 pos_size_handler=None,
                 exit_dates={},
             )
 
     def test_backtest_executions_when_buy_limit_and_no_shares_then_error(
         self, data_source_df
     ):
@@ -770,26 +731,23 @@
         with pytest.raises(
             ValueError,
             match=re.escape(
                 "buy_shares must be set when buy_limit_price is set."
             ),
         ):
             mixin.backtest_executions(
+                config=StrategyConfig(),
                 executions=execs,
                 before_exec_fn=None,
                 after_exec_fn=None,
                 sessions=defaultdict(dict),
                 models={},
                 indicator_data={},
                 test_data=data_source_df,
                 portfolio=Portfolio(100_000),
-                buy_delay=1,
-                sell_delay=1,
-                max_long_positions=1,
-                max_short_positions=None,
                 pos_size_handler=None,
                 exit_dates={},
             )
 
     def test_backtest_executions_when_sell_limit_and_no_shares_then_error(
         self, data_source_df
     ):
@@ -808,26 +766,23 @@
         with pytest.raises(
             ValueError,
             match=re.escape(
                 "sell_shares must be set when sell_limit_price is set."
             ),
         ):
             mixin.backtest_executions(
+                config=StrategyConfig(),
                 executions=execs,
                 before_exec_fn=None,
                 after_exec_fn=None,
                 sessions=defaultdict(dict),
                 models={},
                 indicator_data={},
                 test_data=data_source_df,
                 portfolio=Portfolio(100_000),
-                buy_delay=1,
-                sell_delay=1,
-                max_long_positions=1,
-                max_short_positions=None,
                 pos_size_handler=None,
                 exit_dates={},
             )
 
     def test_backtest_executions_when_buy_order_not_filled(
         self, data_source_df
     ):
@@ -842,26 +797,23 @@
             model_names=frozenset(),
             indicator_names=frozenset(),
         )
         execs = {exec}
         portfolio = Portfolio(1)
         mixin = BacktestMixin()
         mixin.backtest_executions(
+            config=StrategyConfig(),
             executions=execs,
             before_exec_fn=None,
             after_exec_fn=None,
             sessions=defaultdict(dict),
             models={},
             indicator_data={},
             test_data=data_source_df,
             portfolio=portfolio,
-            buy_delay=1,
-            sell_delay=1,
-            max_long_positions=1,
-            max_short_positions=None,
             pos_size_handler=None,
             exit_dates={},
         )
         assert not len(portfolio.orders)
 
     def test_backtest_executions_when_sell_order_not_filled(
         self, data_source_df
@@ -878,26 +830,23 @@
             model_names=frozenset(),
             indicator_names=frozenset(),
         )
         execs = {exec}
         portfolio = Portfolio(1)
         mixin = BacktestMixin()
         mixin.backtest_executions(
+            config=StrategyConfig(),
             executions=execs,
             before_exec_fn=None,
             after_exec_fn=None,
             sessions=defaultdict(dict),
             models={},
             indicator_data={},
             test_data=data_source_df,
             portfolio=portfolio,
-            buy_delay=1,
-            sell_delay=1,
-            max_long_positions=1,
-            max_short_positions=None,
             pos_size_handler=None,
             exit_dates={},
         )
         assert not len(portfolio.orders)
 
 
 @pytest.fixture()
```

### Comparing `lib-pybroker-1.1.5/tests/test_vect.py` & `lib-pybroker-1.1.6/tests/test_vect.py`

 * *Files identical despite different names*

