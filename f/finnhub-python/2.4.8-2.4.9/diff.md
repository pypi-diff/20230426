# Comparing `tmp/finnhub-python-2.4.8.tar.gz` & `tmp/finnhub-python-2.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/finnhub-python-2.4.8.tar", last modified: Wed Jan 19 08:30:24 2022, max compression
+gzip compressed data, was "dist/finnhub-python-2.4.9.tar", last modified: Tue Feb  8 17:04:14 2022, max compression
```

## Comparing `finnhub-python-2.4.8.tar` & `finnhub-python-2.4.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 trido      (501) staff       (20)        0 2022-01-19 08:30:24.000000 finnhub-python-2.4.8/
--rw-r--r--   0 trido      (501) staff       (20)     8966 2022-01-19 08:30:24.000000 finnhub-python-2.4.8/PKG-INFO
--rw-r--r--   0 trido      (501) staff       (20)     6593 2022-01-19 08:29:53.000000 finnhub-python-2.4.8/README.md
-drwxr-xr-x   0 trido      (501) staff       (20)        0 2022-01-19 08:30:24.000000 finnhub-python-2.4.8/finnhub/
--rw-r--r--   0 trido      (501) staff       (20)      150 2021-07-22 09:33:00.000000 finnhub-python-2.4.8/finnhub/__init__.py
--rw-r--r--   0 trido      (501) staff       (20)    14098 2022-01-19 08:25:09.000000 finnhub-python-2.4.8/finnhub/client.py
--rw-r--r--   0 trido      (501) staff       (20)      974 2021-07-22 09:33:00.000000 finnhub-python-2.4.8/finnhub/exceptions.py
-drwxr-xr-x   0 trido      (501) staff       (20)        0 2022-01-19 08:30:24.000000 finnhub-python-2.4.8/finnhub_python.egg-info/
--rw-r--r--   0 trido      (501) staff       (20)     8966 2022-01-19 08:30:24.000000 finnhub-python-2.4.8/finnhub_python.egg-info/PKG-INFO
--rw-r--r--   0 trido      (501) staff       (20)      277 2022-01-19 08:30:24.000000 finnhub-python-2.4.8/finnhub_python.egg-info/SOURCES.txt
--rw-r--r--   0 trido      (501) staff       (20)        1 2022-01-19 08:30:24.000000 finnhub-python-2.4.8/finnhub_python.egg-info/dependency_links.txt
--rw-r--r--   0 trido      (501) staff       (20)       17 2022-01-19 08:30:24.000000 finnhub-python-2.4.8/finnhub_python.egg-info/requires.txt
--rw-r--r--   0 trido      (501) staff       (20)        8 2022-01-19 08:30:24.000000 finnhub-python-2.4.8/finnhub_python.egg-info/top_level.txt
--rw-r--r--   0 trido      (501) staff       (20)       69 2022-01-19 08:30:24.000000 finnhub-python-2.4.8/setup.cfg
--rw-r--r--   0 trido      (501) staff       (20)      678 2022-01-19 08:29:17.000000 finnhub-python-2.4.8/setup.py
+drwxr-xr-x   0 trido      (501) staff       (20)        0 2022-02-08 17:04:14.000000 finnhub-python-2.4.9/
+-rw-r--r--   0 trido      (501) staff       (20)     9079 2022-02-08 17:04:14.000000 finnhub-python-2.4.9/PKG-INFO
+-rw-r--r--   0 trido      (501) staff       (20)     6682 2022-02-08 17:03:30.000000 finnhub-python-2.4.9/README.md
+drwxr-xr-x   0 trido      (501) staff       (20)        0 2022-02-08 17:04:14.000000 finnhub-python-2.4.9/finnhub/
+-rw-r--r--   0 trido      (501) staff       (20)      150 2021-07-22 09:33:00.000000 finnhub-python-2.4.9/finnhub/__init__.py
+-rw-r--r--   0 trido      (501) staff       (20)    14248 2022-02-08 17:00:14.000000 finnhub-python-2.4.9/finnhub/client.py
+-rw-r--r--   0 trido      (501) staff       (20)      974 2021-07-22 09:33:00.000000 finnhub-python-2.4.9/finnhub/exceptions.py
+drwxr-xr-x   0 trido      (501) staff       (20)        0 2022-02-08 17:04:14.000000 finnhub-python-2.4.9/finnhub_python.egg-info/
+-rw-r--r--   0 trido      (501) staff       (20)     9079 2022-02-08 17:04:13.000000 finnhub-python-2.4.9/finnhub_python.egg-info/PKG-INFO
+-rw-r--r--   0 trido      (501) staff       (20)      277 2022-02-08 17:04:13.000000 finnhub-python-2.4.9/finnhub_python.egg-info/SOURCES.txt
+-rw-r--r--   0 trido      (501) staff       (20)        1 2022-02-08 17:04:13.000000 finnhub-python-2.4.9/finnhub_python.egg-info/dependency_links.txt
+-rw-r--r--   0 trido      (501) staff       (20)       17 2022-02-08 17:04:13.000000 finnhub-python-2.4.9/finnhub_python.egg-info/requires.txt
+-rw-r--r--   0 trido      (501) staff       (20)        8 2022-02-08 17:04:13.000000 finnhub-python-2.4.9/finnhub_python.egg-info/top_level.txt
+-rw-r--r--   0 trido      (501) staff       (20)       69 2022-02-08 17:04:14.000000 finnhub-python-2.4.9/setup.cfg
+-rw-r--r--   0 trido      (501) staff       (20)      678 2022-02-08 17:03:58.000000 finnhub-python-2.4.9/setup.py
```

### Comparing `finnhub-python-2.4.8/PKG-INFO` & `finnhub-python-2.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finnhub-python
-Version: 2.4.8
+Version: 2.4.9
 Summary: Finnhub API
 Home-page: https://finnhub.io/docs/api
 Author: Finnhub
 Author-email: support@finnhub.io
 License: Apache-2.0
 Description: # finnhub-python
         
@@ -154,14 +154,17 @@
         
         # Upgrade downgrade
         print(finnhub_client.upgrade_downgrade(symbol='AAPL', _from='2020-01-01', to='2020-06-30'))
         
         # Economic code
         print(finnhub_client.economic_code()[0:5])
         
+        # Economic calendar
+        print(finnhub_client.calendar_economic('2021-01-01', '2021-01-07'))
+        
         # Support resistance
         print(finnhub_client.support_resistance('AAPL', 'D'))
         
         # Technical Indicator
         print(finnhub_client.technical_indicator(symbol="AAPL", resolution='D', _from=1583098857, to=1584308457, indicator='rsi', indicator_fields={"timeperiod": 3}))
         
         # Stock splits
```

### Comparing `finnhub-python-2.4.8/README.md` & `finnhub-python-2.4.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -146,14 +146,17 @@
 
 # Upgrade downgrade
 print(finnhub_client.upgrade_downgrade(symbol='AAPL', _from='2020-01-01', to='2020-06-30'))
 
 # Economic code
 print(finnhub_client.economic_code()[0:5])
 
+# Economic calendar
+print(finnhub_client.calendar_economic('2021-01-01', '2021-01-07'))
+
 # Support resistance
 print(finnhub_client.support_resistance('AAPL', 'D'))
 
 # Technical Indicator
 print(finnhub_client.technical_indicator(symbol="AAPL", resolution='D', _from=1583098857, to=1584308457, indicator='rsi', indicator_fields={"timeperiod": 3}))
 
 # Stock splits
```

### Comparing `finnhub-python-2.4.8/finnhub/client.py` & `finnhub-python-2.4.9/finnhub/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,16 +124,16 @@
 
     def recommendation_trends(self, symbol):
         return self._get("/stock/recommendation", params={"symbol": symbol})
 
     def price_target(self, symbol):
         return self._get("/stock/price-target", params={"symbol": symbol})
 
-    def upgrade_downgrade(self, **params):
-        return self._get("/stock/upgrade-downgrade", params=params)
+    def upgrade_downgrade(self, symbol=None, _from=None, to=None):
+        return self._get("/stock/upgrade-downgrade", params={'symbol': symbol, 'from': _from, 'to': to})
 
     def option_chain(self, **params):
         return self._get("/stock/option-chain", params=params)
 
     def company_peers(self, symbol):
         return self._get("/stock/peers", params={"symbol": symbol})
 
@@ -333,16 +333,19 @@
 
     def economic_code(self):
         return self._get("/economic/code")
 
     def economic_data(self, code):
         return self._get("/economic", params={"code": code})
 
-    def calendar_economic(self):
-        return self._get("/calendar/economic")
+    def calendar_economic(self, _from=None, to=None):
+        return self._get("/calendar/economic", params={
+            "from": _from,
+            "to": to
+        })
 
     def earnings_calendar(self, _from, to, symbol, international=False):
         return self._get("/calendar/earnings", params={
             "from": _from,
             "to": to,
             "symbol": symbol,
             "international": international
```

### Comparing `finnhub-python-2.4.8/finnhub/exceptions.py` & `finnhub-python-2.4.9/finnhub/exceptions.py`

 * *Files identical despite different names*

### Comparing `finnhub-python-2.4.8/finnhub_python.egg-info/PKG-INFO` & `finnhub-python-2.4.9/finnhub_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finnhub-python
-Version: 2.4.8
+Version: 2.4.9
 Summary: Finnhub API
 Home-page: https://finnhub.io/docs/api
 Author: Finnhub
 Author-email: support@finnhub.io
 License: Apache-2.0
 Description: # finnhub-python
         
@@ -154,14 +154,17 @@
         
         # Upgrade downgrade
         print(finnhub_client.upgrade_downgrade(symbol='AAPL', _from='2020-01-01', to='2020-06-30'))
         
         # Economic code
         print(finnhub_client.economic_code()[0:5])
         
+        # Economic calendar
+        print(finnhub_client.calendar_economic('2021-01-01', '2021-01-07'))
+        
         # Support resistance
         print(finnhub_client.support_resistance('AAPL', 'D'))
         
         # Technical Indicator
         print(finnhub_client.technical_indicator(symbol="AAPL", resolution='D', _from=1583098857, to=1584308457, indicator='rsi', indicator_fields={"timeperiod": 3}))
         
         # Stock splits
```

### Comparing `finnhub-python-2.4.8/setup.py` & `finnhub-python-2.4.9/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "finnhub-python"
-VERSION = "2.4.8"
+VERSION = "2.4.9"
 REQUIRES = ["requests >= 2.22.0"]
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name=NAME,
```

