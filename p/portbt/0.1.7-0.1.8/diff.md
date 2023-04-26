# Comparing `tmp/portbt-0.1.7.tar.gz` & `tmp/portbt-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "portbt-0.1.7.tar", max compression
+gzip compressed data, was "portbt-0.1.8.tar", max compression
```

## Comparing `portbt-0.1.7.tar` & `portbt-0.1.8.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1099 2023-04-08 18:19:42.889204 portbt-0.1.7/LICENSE.txt
--rw-r--r--   0        0        0      127 2023-04-12 00:16:50.304309 portbt-0.1.7/portbt/__init__.py
--rw-r--r--   0        0        0     3736 2023-04-14 20:17:20.047447 portbt-0.1.7/portbt/backtest_functions.py
--rw-r--r--   0        0        0     2606 2023-04-14 20:17:20.003537 portbt-0.1.7/portbt/portfolio.py
--rw-r--r--   0        0        0      676 2023-04-14 20:17:19.984585 portbt-0.1.7/portbt/utils.py
--rw-r--r--   0        0        0      575 2023-04-14 20:17:34.364045 portbt-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     4417 2023-04-14 20:04:30.388418 portbt-0.1.7/README.md
--rw-r--r--   0        0        0     5014 1970-01-01 00:00:00.000000 portbt-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1099 2023-04-08 18:19:42.889204 portbt-0.1.8/LICENSE.txt
+-rw-r--r--   0        0        0      127 2023-04-12 00:16:50.304309 portbt-0.1.8/portbt/__init__.py
+-rw-r--r--   0        0        0     3736 2023-04-14 20:18:22.520995 portbt-0.1.8/portbt/backtest_functions.py
+-rw-r--r--   0        0        0     2606 2023-04-14 20:17:20.003537 portbt-0.1.8/portbt/portfolio.py
+-rw-r--r--   0        0        0      676 2023-04-14 20:17:19.984585 portbt-0.1.8/portbt/utils.py
+-rw-r--r--   0        0        0      510 2023-04-26 00:26:42.294399 portbt-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     4417 2023-04-14 20:04:30.388418 portbt-0.1.8/README.md
+-rw-r--r--   0        0        0     5065 1970-01-01 00:00:00.000000 portbt-0.1.8/PKG-INFO
```

### Comparing `portbt-0.1.7/LICENSE.txt` & `portbt-0.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `portbt-0.1.7/portbt/backtest_functions.py` & `portbt-0.1.8/portbt/backtest_functions.py`

 * *Files identical despite different names*

### Comparing `portbt-0.1.7/portbt/portfolio.py` & `portbt-0.1.8/portbt/portfolio.py`

 * *Files identical despite different names*

### Comparing `portbt-0.1.7/portbt/utils.py` & `portbt-0.1.8/portbt/utils.py`

 * *Files identical despite different names*

### Comparing `portbt-0.1.7/README.md` & `portbt-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `portbt-0.1.7/PKG-INFO` & `portbt-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: portbt
-Version: 0.1.7
+Version: 0.1.8
 Summary: Python library designed to make portfolio backtesting easy and intuitive
 Home-page: https://github.com/renanmoretto/portbt
 License: MIT
 Author: renanmoretto
 Author-email: himynameisrenan@outlook.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: datetime (>=5.1,<6.0)
-Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
-Requires-Dist: numpy (>=1.24.2,<2.0.0)
-Requires-Dist: pandas (>=2.0.0,<3.0.0)
+Requires-Dist: datetime (>=4.9,<5.0)
+Requires-Dist: matplotlib (>=3.6.0,<4.0.0)
+Requires-Dist: numpy (>=1.23.0,<2.0.0)
+Requires-Dist: pandas (>=1.5.0,<2.0.0)
 Project-URL: Repository, https://github.com/renanmoretto/portbt
 Description-Content-Type: text/markdown
 
 # portbt
 **portbt** is a Python library designed to make backtesting a custom portfolio of assets easy and intuitive. With PortBT, you can test a range of rebalancing strategies and asset allocations using just a few lines of code. 
 
 ## Features
```

