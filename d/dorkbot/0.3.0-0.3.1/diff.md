# Comparing `tmp/dorkbot-0.3.0.tar.gz` & `tmp/dorkbot-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dorkbot-0.3.0.tar", last modified: Tue Apr 25 20:55:53 2023, max compression
+gzip compressed data, was "dorkbot-0.3.1.tar", last modified: Tue Apr 25 21:22:20 2023, max compression
```

## Comparing `dorkbot-0.3.0.tar` & `dorkbot-0.3.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 jgor       (501) staff       (20)        0 2023-04-25 20:55:53.993072 dorkbot-0.3.0/
--rw-r--r--   0 jgor       (501) staff       (20)    10596 2023-04-19 17:48:56.000000 dorkbot-0.3.0/LICENSE
--rw-r--r--   0 jgor       (501) staff       (20)       35 2023-04-19 17:48:56.000000 dorkbot-0.3.0/MANIFEST.in
--rw-r--r--   0 jgor       (501) staff       (20)    10550 2023-04-25 20:55:53.993168 dorkbot-0.3.0/PKG-INFO
--rw-r--r--   0 jgor       (501) staff       (20)    10148 2023-04-25 17:56:00.000000 dorkbot-0.3.0/README.md
-drwxr-xr-x   0 jgor       (501) staff       (20)        0 2023-04-25 20:55:53.931773 dorkbot-0.3.0/dorkbot/
--rw-r--r--   0 jgor       (501) staff       (20)       34 2023-04-19 17:48:56.000000 dorkbot-0.3.0/dorkbot/__init__.py
--rw-r--r--   0 jgor       (501) staff       (20)       22 2023-04-25 20:54:52.000000 dorkbot-0.3.0/dorkbot/_version.py
--rwxr-xr-x   0 jgor       (501) staff       (20)    28427 2023-04-25 20:49:55.000000 dorkbot-0.3.0/dorkbot/dorkbot.py
-drwxr-xr-x   0 jgor       (501) staff       (20)        0 2023-04-25 20:55:53.986180 dorkbot-0.3.0/dorkbot/indexers/
--rw-r--r--   0 jgor       (501) staff       (20)        0 2023-04-19 17:48:56.000000 dorkbot-0.3.0/dorkbot/indexers/__init__.py
--rw-r--r--   0 jgor       (501) staff       (20)     1714 2023-04-19 17:48:56.000000 dorkbot-0.3.0/dorkbot/indexers/bing_api.py
--rwxr-xr-x   0 jgor       (501) staff       (20)     5474 2023-04-25 17:09:52.000000 dorkbot-0.3.0/dorkbot/indexers/commoncrawl.py
--rw-r--r--   0 jgor       (501) staff       (20)      329 2023-04-19 17:48:56.000000 dorkbot-0.3.0/dorkbot/indexers/example.py
--rw-r--r--   0 jgor       (501) staff       (20)     3131 2023-04-19 17:48:56.000000 dorkbot-0.3.0/dorkbot/indexers/google.js
--rw-r--r--   0 jgor       (501) staff       (20)     1910 2023-04-19 17:48:56.000000 dorkbot-0.3.0/dorkbot/indexers/google.py
--rw-r--r--   0 jgor       (501) staff       (20)     2630 2023-04-19 17:48:56.000000 dorkbot-0.3.0/dorkbot/indexers/google_api.py
--rwxr-xr-x   0 jgor       (501) staff       (20)     5643 2023-04-25 17:59:04.000000 dorkbot-0.3.0/dorkbot/indexers/pywb.py
--rw-r--r--   0 jgor       (501) staff       (20)      412 2023-04-19 17:48:56.000000 dorkbot-0.3.0/dorkbot/indexers/stdin.py
--rwxr-xr-x   0 jgor       (501) staff       (20)     4131 2023-04-19 17:48:56.000000 dorkbot-0.3.0/dorkbot/indexers/wayback.py
-drwxr-xr-x   0 jgor       (501) staff       (20)        0 2023-04-25 20:55:53.992752 dorkbot-0.3.0/dorkbot/scanners/
--rw-r--r--   0 jgor       (501) staff       (20)        0 2023-04-19 17:48:56.000000 dorkbot-0.3.0/dorkbot/scanners/__init__.py
--rw-r--r--   0 jgor       (501) staff       (20)     2733 2023-04-19 17:48:56.000000 dorkbot-0.3.0/dorkbot/scanners/arachni.py
--rw-r--r--   0 jgor       (501) staff       (20)      673 2023-04-19 17:48:56.000000 dorkbot-0.3.0/dorkbot/scanners/example.py
--rw-r--r--   0 jgor       (501) staff       (20)     2524 2023-04-19 17:48:56.000000 dorkbot-0.3.0/dorkbot/scanners/wapiti.py
-drwxr-xr-x   0 jgor       (501) staff       (20)        0 2023-04-25 20:55:53.934209 dorkbot-0.3.0/dorkbot.egg-info/
--rw-r--r--   0 jgor       (501) staff       (20)    10550 2023-04-25 20:55:53.000000 dorkbot-0.3.0/dorkbot.egg-info/PKG-INFO
--rw-r--r--   0 jgor       (501) staff       (20)      659 2023-04-25 20:55:53.000000 dorkbot-0.3.0/dorkbot.egg-info/SOURCES.txt
--rw-r--r--   0 jgor       (501) staff       (20)        1 2023-04-25 20:55:53.000000 dorkbot-0.3.0/dorkbot.egg-info/dependency_links.txt
--rw-r--r--   0 jgor       (501) staff       (20)       49 2023-04-25 20:55:53.000000 dorkbot-0.3.0/dorkbot.egg-info/entry_points.txt
--rw-r--r--   0 jgor       (501) staff       (20)        8 2023-04-25 20:55:53.000000 dorkbot-0.3.0/dorkbot.egg-info/top_level.txt
--rw-r--r--   0 jgor       (501) staff       (20)       74 2023-04-25 20:55:53.993838 dorkbot-0.3.0/setup.cfg
--rw-r--r--   0 jgor       (501) staff       (20)      950 2023-04-19 17:48:56.000000 dorkbot-0.3.0/setup.py
+drwxr-xr-x   0 jgor       (501) staff       (20)        0 2023-04-25 21:22:20.005293 dorkbot-0.3.1/
+-rw-r--r--   0 jgor       (501) staff       (20)    10596 2023-04-19 17:48:56.000000 dorkbot-0.3.1/LICENSE
+-rw-r--r--   0 jgor       (501) staff       (20)       35 2023-04-19 17:48:56.000000 dorkbot-0.3.1/MANIFEST.in
+-rw-r--r--   0 jgor       (501) staff       (20)    10550 2023-04-25 21:22:20.005400 dorkbot-0.3.1/PKG-INFO
+-rw-r--r--   0 jgor       (501) staff       (20)    10148 2023-04-25 17:56:00.000000 dorkbot-0.3.1/README.md
+drwxr-xr-x   0 jgor       (501) staff       (20)        0 2023-04-25 21:22:19.976103 dorkbot-0.3.1/dorkbot/
+-rw-r--r--   0 jgor       (501) staff       (20)       34 2023-04-19 17:48:56.000000 dorkbot-0.3.1/dorkbot/__init__.py
+-rw-r--r--   0 jgor       (501) staff       (20)       22 2023-04-25 21:22:09.000000 dorkbot-0.3.1/dorkbot/_version.py
+-rwxr-xr-x   0 jgor       (501) staff       (20)    28397 2023-04-25 21:19:09.000000 dorkbot-0.3.1/dorkbot/dorkbot.py
+drwxr-xr-x   0 jgor       (501) staff       (20)        0 2023-04-25 21:22:19.999926 dorkbot-0.3.1/dorkbot/indexers/
+-rw-r--r--   0 jgor       (501) staff       (20)        0 2023-04-19 17:48:56.000000 dorkbot-0.3.1/dorkbot/indexers/__init__.py
+-rw-r--r--   0 jgor       (501) staff       (20)     1714 2023-04-19 17:48:56.000000 dorkbot-0.3.1/dorkbot/indexers/bing_api.py
+-rwxr-xr-x   0 jgor       (501) staff       (20)     5474 2023-04-25 17:09:52.000000 dorkbot-0.3.1/dorkbot/indexers/commoncrawl.py
+-rw-r--r--   0 jgor       (501) staff       (20)      329 2023-04-19 17:48:56.000000 dorkbot-0.3.1/dorkbot/indexers/example.py
+-rw-r--r--   0 jgor       (501) staff       (20)     3131 2023-04-19 17:48:56.000000 dorkbot-0.3.1/dorkbot/indexers/google.js
+-rw-r--r--   0 jgor       (501) staff       (20)     1910 2023-04-19 17:48:56.000000 dorkbot-0.3.1/dorkbot/indexers/google.py
+-rw-r--r--   0 jgor       (501) staff       (20)     2630 2023-04-19 17:48:56.000000 dorkbot-0.3.1/dorkbot/indexers/google_api.py
+-rwxr-xr-x   0 jgor       (501) staff       (20)     5643 2023-04-25 17:59:04.000000 dorkbot-0.3.1/dorkbot/indexers/pywb.py
+-rw-r--r--   0 jgor       (501) staff       (20)      412 2023-04-19 17:48:56.000000 dorkbot-0.3.1/dorkbot/indexers/stdin.py
+-rwxr-xr-x   0 jgor       (501) staff       (20)     4131 2023-04-19 17:48:56.000000 dorkbot-0.3.1/dorkbot/indexers/wayback.py
+drwxr-xr-x   0 jgor       (501) staff       (20)        0 2023-04-25 21:22:20.004790 dorkbot-0.3.1/dorkbot/scanners/
+-rw-r--r--   0 jgor       (501) staff       (20)        0 2023-04-19 17:48:56.000000 dorkbot-0.3.1/dorkbot/scanners/__init__.py
+-rw-r--r--   0 jgor       (501) staff       (20)     2733 2023-04-19 17:48:56.000000 dorkbot-0.3.1/dorkbot/scanners/arachni.py
+-rw-r--r--   0 jgor       (501) staff       (20)      673 2023-04-19 17:48:56.000000 dorkbot-0.3.1/dorkbot/scanners/example.py
+-rw-r--r--   0 jgor       (501) staff       (20)     2524 2023-04-19 17:48:56.000000 dorkbot-0.3.1/dorkbot/scanners/wapiti.py
+drwxr-xr-x   0 jgor       (501) staff       (20)        0 2023-04-25 21:22:19.978465 dorkbot-0.3.1/dorkbot.egg-info/
+-rw-r--r--   0 jgor       (501) staff       (20)    10550 2023-04-25 21:22:19.000000 dorkbot-0.3.1/dorkbot.egg-info/PKG-INFO
+-rw-r--r--   0 jgor       (501) staff       (20)      659 2023-04-25 21:22:19.000000 dorkbot-0.3.1/dorkbot.egg-info/SOURCES.txt
+-rw-r--r--   0 jgor       (501) staff       (20)        1 2023-04-25 21:22:19.000000 dorkbot-0.3.1/dorkbot.egg-info/dependency_links.txt
+-rw-r--r--   0 jgor       (501) staff       (20)       49 2023-04-25 21:22:19.000000 dorkbot-0.3.1/dorkbot.egg-info/entry_points.txt
+-rw-r--r--   0 jgor       (501) staff       (20)        8 2023-04-25 21:22:19.000000 dorkbot-0.3.1/dorkbot.egg-info/top_level.txt
+-rw-r--r--   0 jgor       (501) staff       (20)       74 2023-04-25 21:22:20.006638 dorkbot-0.3.1/setup.cfg
+-rw-r--r--   0 jgor       (501) staff       (20)      950 2023-04-19 17:48:56.000000 dorkbot-0.3.1/setup.py
```

### Comparing `dorkbot-0.3.0/LICENSE` & `dorkbot-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dorkbot-0.3.0/PKG-INFO` & `dorkbot-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dorkbot
-Version: 0.3.0
+Version: 0.3.1
 Summary: Command-line tool to scan search results for vulnerabilities
 Home-page: http://dorkbot.io
 Author: jgor
 Author-email: jgor@utexas.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Free for non-commercial use
 Classifier: Operating System :: OS Independent
```

### Comparing `dorkbot-0.3.0/README.md` & `dorkbot-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `dorkbot-0.3.0/dorkbot/dorkbot.py` & `dorkbot-0.3.1/dorkbot/dorkbot.py`

 * *Files 2% similar despite different names*

```diff
@@ -375,27 +375,25 @@
         self.db.close()
 
     def get_urls(self, unscanned_only=False, source=False):
         fields = "url"
         if source is True:
             fields += ",source"
 
-        where = None
+        sql = f"SELECT {fields} FROM targets"
         if unscanned_only:
-            where = " WHERE scanned != 1"
-
-        sql = f"SELECT {fields} FROM targets" + where
+            sql += " WHERE scanned != 1"
 
         try:
             with self.db, closing(self.db.cursor()) as c:
                 if source and source is not True:
-                    if where is None:
-                        sql += " WHERE "
-                    else:
+                    if "WHERE" in sql:
                         sql += " AND "
+                    else:
+                        sql += " WHERE "
                     sql += "source = %s" % self.param
                     c.execute(sql, (source,))
                 else:
                     c.execute(sql)
                 urls = [" | ".join(row) for row in c.fetchall()]
         except self.module.Error as e:
             logging.error("Failed to get targets - %s", str(e))
```

### Comparing `dorkbot-0.3.0/dorkbot/indexers/bing_api.py` & `dorkbot-0.3.1/dorkbot/indexers/bing_api.py`

 * *Files identical despite different names*

### Comparing `dorkbot-0.3.0/dorkbot/indexers/commoncrawl.py` & `dorkbot-0.3.1/dorkbot/indexers/commoncrawl.py`

 * *Files identical despite different names*

### Comparing `dorkbot-0.3.0/dorkbot/indexers/google.js` & `dorkbot-0.3.1/dorkbot/indexers/google.js`

 * *Files identical despite different names*

### Comparing `dorkbot-0.3.0/dorkbot/indexers/google.py` & `dorkbot-0.3.1/dorkbot/indexers/google.py`

 * *Files identical despite different names*

### Comparing `dorkbot-0.3.0/dorkbot/indexers/google_api.py` & `dorkbot-0.3.1/dorkbot/indexers/google_api.py`

 * *Files identical despite different names*

### Comparing `dorkbot-0.3.0/dorkbot/indexers/pywb.py` & `dorkbot-0.3.1/dorkbot/indexers/pywb.py`

 * *Files identical despite different names*

### Comparing `dorkbot-0.3.0/dorkbot/indexers/wayback.py` & `dorkbot-0.3.1/dorkbot/indexers/wayback.py`

 * *Files identical despite different names*

### Comparing `dorkbot-0.3.0/dorkbot/scanners/arachni.py` & `dorkbot-0.3.1/dorkbot/scanners/arachni.py`

 * *Files identical despite different names*

### Comparing `dorkbot-0.3.0/dorkbot/scanners/example.py` & `dorkbot-0.3.1/dorkbot/scanners/example.py`

 * *Files identical despite different names*

### Comparing `dorkbot-0.3.0/dorkbot/scanners/wapiti.py` & `dorkbot-0.3.1/dorkbot/scanners/wapiti.py`

 * *Files identical despite different names*

### Comparing `dorkbot-0.3.0/dorkbot.egg-info/PKG-INFO` & `dorkbot-0.3.1/dorkbot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dorkbot
-Version: 0.3.0
+Version: 0.3.1
 Summary: Command-line tool to scan search results for vulnerabilities
 Home-page: http://dorkbot.io
 Author: jgor
 Author-email: jgor@utexas.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Free for non-commercial use
 Classifier: Operating System :: OS Independent
```

### Comparing `dorkbot-0.3.0/dorkbot.egg-info/SOURCES.txt` & `dorkbot-0.3.1/dorkbot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dorkbot-0.3.0/setup.py` & `dorkbot-0.3.1/setup.py`

 * *Files identical despite different names*

