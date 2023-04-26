# Comparing `tmp/findmyorder-1.0.2.tar.gz` & `tmp/findmyorder-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findmyorder-1.0.2.tar", max compression
+gzip compressed data, was "findmyorder-1.0.3.tar", max compression
```

## Comparing `findmyorder-1.0.2.tar` & `findmyorder-1.0.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-04-26 17:25:39.557189 findmyorder-1.0.2/LICENSE
--rw-r--r--   0        0        0     1426 2023-04-26 17:25:39.557189 findmyorder-1.0.2/README.md
--rw-r--r--   0        0        0      106 2023-04-26 17:25:40.661217 findmyorder-1.0.2/findmyorder/__init__.py
--rw-r--r--   0        0        0      723 2023-04-26 17:25:39.557189 findmyorder-1.0.2/findmyorder/config.py
--rw-r--r--   0        0        0      120 2023-04-26 17:25:39.557189 findmyorder-1.0.2/findmyorder/default_settings.toml
--rw-r--r--   0        0        0     3110 2023-04-26 17:25:39.557189 findmyorder-1.0.2/findmyorder/main.py
--rw-r--r--   0        0        0     1194 2023-04-26 17:25:40.657217 findmyorder-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     2248 1970-01-01 00:00:00.000000 findmyorder-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-04-26 19:59:47.748424 findmyorder-1.0.3/LICENSE
+-rw-r--r--   0        0        0     1426 2023-04-26 19:59:47.748424 findmyorder-1.0.3/README.md
+-rw-r--r--   0        0        0      106 2023-04-26 19:59:48.780516 findmyorder-1.0.3/findmyorder/__init__.py
+-rw-r--r--   0        0        0      723 2023-04-26 19:59:47.748424 findmyorder-1.0.3/findmyorder/config.py
+-rw-r--r--   0        0        0      120 2023-04-26 19:59:47.748424 findmyorder-1.0.3/findmyorder/default_settings.toml
+-rw-r--r--   0        0        0     3147 2023-04-26 19:59:47.748424 findmyorder-1.0.3/findmyorder/main.py
+-rw-r--r--   0        0        0     1194 2023-04-26 19:59:48.776515 findmyorder-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2248 1970-01-01 00:00:00.000000 findmyorder-1.0.3/PKG-INFO
```

### Comparing `findmyorder-1.0.2/LICENSE` & `findmyorder-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `findmyorder-1.0.2/README.md` & `findmyorder-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `findmyorder-1.0.2/findmyorder/config.py` & `findmyorder-1.0.3/findmyorder/config.py`

 * *Files identical despite different names*

### Comparing `findmyorder-1.0.2/findmyorder/main.py` & `findmyorder-1.0.3/findmyorder/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -61,30 +61,30 @@
         self.logger.debug(f"get_order for {mystring}")
 
         if (self.search(mystring)):
 
             parsed_order = identify_order(mystring)
             self.logger.info(msg=f"parsed_order: {parsed_order}")
 
-            order_raw = mystring.split()
-            self.logger.info(msg=f"Order identified: {order_raw}")
+            # order_raw = mystring.split()
+            # self.logger.info(msg=f"Order identified: {order_raw}")
 
-            order = {}
-            order['market'] = 'Any'
-            order['exchange'] = 'Any'
-            order['timestamp'] = datetime.utcnow()
-            order['leverage'] = 1
-            order['ordertype'] = 'spot'
-            order['direction'] = 'BUY'
-            order['symbol'] = 'EURUSD'
-            order['quantity'] = 10
-            order['amount'] = 100
-            order['stoploss'] = 1000
-            order['takeprofit'] = {'tp1':1, 'tp2':10, 'tp3':100, 'tp4':1000, 'tp5':1000}
-            order['comments'] = 'findmyorder'
+            # order = {}
+            # order['market'] = 'Any'
+            # order['exchange'] = 'Any'
+            # order['timestamp'] = datetime.utcnow()
+            # order['leverage'] = 1
+            # order['ordertype'] = 'spot'
+            # order['direction'] = 'BUY'
+            # order['symbol'] = 'EURUSD'
+            # order['quantity'] = 10
+            # order['amount'] = 100
+            # order['stoploss'] = 1000
+            # order['takeprofit'] = {'tp1':1, 'tp2':10, 'tp3':100, 'tp4':1000, 'tp5':1000}
+            # order['comments'] = 'findmyorder'
             
-            return order
+            return parsed_order
 
       except Exception as e:
           self.logger.debug(f"error {e}")
           return
```

### Comparing `findmyorder-1.0.2/pyproject.toml` & `findmyorder-1.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "findmyorder"
-version = "1.0.2"
+version = "1.0.3"
 description = "A python package to identify and parse order for trade execution."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["trading", "order", "trade","buy","sell"]
```

### Comparing `findmyorder-1.0.2/PKG-INFO` & `findmyorder-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: findmyorder
-Version: 1.0.2
+Version: 1.0.3
 Summary: A python package to identify and parse order for trade execution.
 License: MIT
 Keywords: trading,order,trade,buy,sell
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
```

