# Comparing `tmp/findmyorder-1.0.0.tar.gz` & `tmp/findmyorder-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findmyorder-1.0.0.tar", max compression
+gzip compressed data, was "findmyorder-1.0.1.tar", max compression
```

## Comparing `findmyorder-1.0.0.tar` & `findmyorder-1.0.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-04-26 15:01:19.233066 findmyorder-1.0.0/LICENSE
--rw-r--r--   0        0        0     1426 2023-04-26 15:01:19.233066 findmyorder-1.0.0/README.md
--rw-r--r--   0        0        0      106 2023-04-26 15:01:19.961066 findmyorder-1.0.0/findmyorder/__init__.py
--rw-r--r--   0        0        0      723 2023-04-26 15:01:19.233066 findmyorder-1.0.0/findmyorder/config.py
--rw-r--r--   0        0        0      120 2023-04-26 15:01:19.233066 findmyorder-1.0.0/findmyorder/default_settings.toml
--rw-r--r--   0        0        0     3112 2023-04-26 15:01:19.233066 findmyorder-1.0.0/findmyorder/main.py
--rw-r--r--   0        0        0     1194 2023-04-26 15:01:19.961066 findmyorder-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2248 1970-01-01 00:00:00.000000 findmyorder-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-04-26 16:00:10.275506 findmyorder-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1426 2023-04-26 16:00:10.275506 findmyorder-1.0.1/README.md
+-rw-r--r--   0        0        0      106 2023-04-26 16:00:11.155521 findmyorder-1.0.1/findmyorder/__init__.py
+-rw-r--r--   0        0        0      723 2023-04-26 16:00:10.275506 findmyorder-1.0.1/findmyorder/config.py
+-rw-r--r--   0        0        0      120 2023-04-26 16:00:10.275506 findmyorder-1.0.1/findmyorder/default_settings.toml
+-rw-r--r--   0        0        0     3113 2023-04-26 16:00:10.275506 findmyorder-1.0.1/findmyorder/main.py
+-rw-r--r--   0        0        0     1194 2023-04-26 16:00:11.155521 findmyorder-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2248 1970-01-01 00:00:00.000000 findmyorder-1.0.1/PKG-INFO
```

### Comparing `findmyorder-1.0.0/LICENSE` & `findmyorder-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `findmyorder-1.0.0/README.md` & `findmyorder-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `findmyorder-1.0.0/findmyorder/config.py` & `findmyorder-1.0.1/findmyorder/config.py`

 * *Files identical despite different names*

### Comparing `findmyorder-1.0.0/findmyorder/main.py` & `findmyorder-1.0.1/findmyorder/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
               return True
         self.logger.debug(f"no word identified in {message_to_parse}")
         return False
       except Exception as e:
         self.logger.debug(f"error search {e}")
         return False
 
-    def identify_order(self,mystring: str = None,)
+    def identify_order(self,mystring: str = None,):
       # Define the grammar for parsing orders
       action = oneOf("BUY SELL LONG SHORT")
       currency_pair = Word(alphas, exact=6)
       market = Optional(Word(alphas, exact=4))
       leverage = Regex(r'Leverage: \w+ \((\d+(\.\d+)?X)\)')('leverage')
       percentage = Regex(r'\d+(\.\d+)?%')
       quantity = Regex(r'\d+(\.\d+)?')('quantity')
```

### Comparing `findmyorder-1.0.0/pyproject.toml` & `findmyorder-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "findmyorder"
-version = "1.0.0"
+version = "1.0.1"
 description = "A python package to identify and parse order for trade execution."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["trading", "order", "trade","buy","sell"]
```

### Comparing `findmyorder-1.0.0/PKG-INFO` & `findmyorder-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: findmyorder
-Version: 1.0.0
+Version: 1.0.1
 Summary: A python package to identify and parse order for trade execution.
 License: MIT
 Keywords: trading,order,trade,buy,sell
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
```

