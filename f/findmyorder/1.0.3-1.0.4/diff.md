# Comparing `tmp/findmyorder-1.0.3.tar.gz` & `tmp/findmyorder-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findmyorder-1.0.3.tar", max compression
+gzip compressed data, was "findmyorder-1.0.4.tar", max compression
```

## Comparing `findmyorder-1.0.3.tar` & `findmyorder-1.0.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-04-26 19:59:47.748424 findmyorder-1.0.3/LICENSE
--rw-r--r--   0        0        0     1426 2023-04-26 19:59:47.748424 findmyorder-1.0.3/README.md
--rw-r--r--   0        0        0      106 2023-04-26 19:59:48.780516 findmyorder-1.0.3/findmyorder/__init__.py
--rw-r--r--   0        0        0      723 2023-04-26 19:59:47.748424 findmyorder-1.0.3/findmyorder/config.py
--rw-r--r--   0        0        0      120 2023-04-26 19:59:47.748424 findmyorder-1.0.3/findmyorder/default_settings.toml
--rw-r--r--   0        0        0     3147 2023-04-26 19:59:47.748424 findmyorder-1.0.3/findmyorder/main.py
--rw-r--r--   0        0        0     1194 2023-04-26 19:59:48.776515 findmyorder-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     2248 1970-01-01 00:00:00.000000 findmyorder-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-04-26 20:37:37.263603 findmyorder-1.0.4/LICENSE
+-rw-r--r--   0        0        0     1426 2023-04-26 20:37:37.263603 findmyorder-1.0.4/README.md
+-rw-r--r--   0        0        0      106 2023-04-26 20:37:38.483613 findmyorder-1.0.4/findmyorder/__init__.py
+-rw-r--r--   0        0        0      723 2023-04-26 20:37:37.263603 findmyorder-1.0.4/findmyorder/config.py
+-rw-r--r--   0        0        0      120 2023-04-26 20:37:37.263603 findmyorder-1.0.4/findmyorder/default_settings.toml
+-rw-r--r--   0        0        0     3153 2023-04-26 20:37:37.263603 findmyorder-1.0.4/findmyorder/main.py
+-rw-r--r--   0        0        0     1194 2023-04-26 20:37:38.483613 findmyorder-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2248 1970-01-01 00:00:00.000000 findmyorder-1.0.4/PKG-INFO
```

### Comparing `findmyorder-1.0.3/LICENSE` & `findmyorder-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `findmyorder-1.0.3/README.md` & `findmyorder-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `findmyorder-1.0.3/findmyorder/config.py` & `findmyorder-1.0.4/findmyorder/config.py`

 * *Files identical despite different names*

### Comparing `findmyorder-1.0.3/findmyorder/main.py` & `findmyorder-1.0.4/findmyorder/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
     def __init__(self,
                  ):
         self.logger =  logging.getLogger(__name__)
 
     def search(self,message_to_parse: str = None,):
       try:
-        print(settings.identifier)
+      #  print(settings.identifier)
         myDict = settings.identifier
 
         for word in myDict:
             self.logger.debug(f"Loop check {word}")
             if re.search(word, message_to_parse):
               self.logger.debug(f"found {word} in {message_to_parse}")
               return True
@@ -58,15 +58,15 @@
 
     def get_order(self,mystring: str = None,):
       try:
         self.logger.debug(f"get_order for {mystring}")
 
         if (self.search(mystring)):
 
-            parsed_order = identify_order(mystring)
+            parsed_order = self.identify_order(mystring)
             self.logger.info(msg=f"parsed_order: {parsed_order}")
 
             # order_raw = mystring.split()
             # self.logger.info(msg=f"Order identified: {order_raw}")
 
             # order = {}
             # order['market'] = 'Any'
```

### Comparing `findmyorder-1.0.3/pyproject.toml` & `findmyorder-1.0.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "findmyorder"
-version = "1.0.3"
+version = "1.0.4"
 description = "A python package to identify and parse order for trade execution."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["trading", "order", "trade","buy","sell"]
```

### Comparing `findmyorder-1.0.3/PKG-INFO` & `findmyorder-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: findmyorder
-Version: 1.0.3
+Version: 1.0.4
 Summary: A python package to identify and parse order for trade execution.
 License: MIT
 Keywords: trading,order,trade,buy,sell
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
```

