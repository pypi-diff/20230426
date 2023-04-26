# Comparing `tmp/hullencrypt-0.0.4.tar.gz` & `tmp/hullencrypt-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hullencrypt-0.0.4.tar", last modified: Tue Apr 25 17:42:09 2023, max compression
+gzip compressed data, was "hullencrypt-0.0.5.tar", last modified: Wed Apr 26 17:44:51 2023, max compression
```

## Comparing `hullencrypt-0.0.4.tar` & `hullencrypt-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-04-25 17:42:09.815528 hullencrypt-0.0.4/
--rw-r--r--   0 john      (1000) john      (1000)    35149 2023-04-25 16:33:25.000000 hullencrypt-0.0.4/LICENSE
--rw-r--r--   0 john      (1000) john      (1000)     2052 2023-04-25 17:42:09.815528 hullencrypt-0.0.4/PKG-INFO
--rw-r--r--   0 john      (1000) john      (1000)     1623 2023-04-25 16:18:17.000000 hullencrypt-0.0.4/README.md
--rw-r--r--   0 john      (1000) john      (1000)      485 2023-04-25 17:41:33.000000 hullencrypt-0.0.4/pyproject.toml
--rw-r--r--   0 john      (1000) john      (1000)       38 2023-04-25 17:42:09.815528 hullencrypt-0.0.4/setup.cfg
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-04-25 17:42:09.815528 hullencrypt-0.0.4/src/
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-04-25 17:42:09.815528 hullencrypt-0.0.4/src/hullencrypt/
--rw-r--r--   0 john      (1000) john      (1000)     5988 2023-04-25 17:32:29.000000 hullencrypt-0.0.4/src/hullencrypt/base.py
--rw-r--r--   0 john      (1000) john      (1000)     1130 2023-04-25 17:35:11.000000 hullencrypt-0.0.4/src/hullencrypt/test.py
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-04-25 17:42:09.815528 hullencrypt-0.0.4/src/hullencrypt.egg-info/
--rw-r--r--   0 john      (1000) john      (1000)     2052 2023-04-25 17:42:09.000000 hullencrypt-0.0.4/src/hullencrypt.egg-info/PKG-INFO
--rw-r--r--   0 john      (1000) john      (1000)      274 2023-04-25 17:42:09.000000 hullencrypt-0.0.4/src/hullencrypt.egg-info/SOURCES.txt
--rw-r--r--   0 john      (1000) john      (1000)        1 2023-04-25 17:42:09.000000 hullencrypt-0.0.4/src/hullencrypt.egg-info/dependency_links.txt
--rw-r--r--   0 john      (1000) john      (1000)       21 2023-04-25 17:42:09.000000 hullencrypt-0.0.4/src/hullencrypt.egg-info/requires.txt
--rw-r--r--   0 john      (1000) john      (1000)       12 2023-04-25 17:42:09.000000 hullencrypt-0.0.4/src/hullencrypt.egg-info/top_level.txt
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-04-26 17:44:51.133825 hullencrypt-0.0.5/
+-rw-r--r--   0 john      (1000) john      (1000)    35149 2023-04-25 16:33:25.000000 hullencrypt-0.0.5/LICENSE
+-rw-r--r--   0 john      (1000) john      (1000)     2052 2023-04-26 17:44:51.133825 hullencrypt-0.0.5/PKG-INFO
+-rw-r--r--   0 john      (1000) john      (1000)     1623 2023-04-25 16:18:17.000000 hullencrypt-0.0.5/README.md
+-rw-r--r--   0 john      (1000) john      (1000)      485 2023-04-26 17:43:36.000000 hullencrypt-0.0.5/pyproject.toml
+-rw-r--r--   0 john      (1000) john      (1000)       38 2023-04-26 17:44:51.133825 hullencrypt-0.0.5/setup.cfg
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-04-26 17:44:51.110491 hullencrypt-0.0.5/src/
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-04-26 17:44:51.130492 hullencrypt-0.0.5/src/hullencrypt/
+-rw-r--r--   0 john      (1000) john      (1000)     5703 2023-04-26 17:44:40.000000 hullencrypt-0.0.5/src/hullencrypt/base.py
+-rw-r--r--   0 john      (1000) john      (1000)     1130 2023-04-25 17:35:11.000000 hullencrypt-0.0.5/src/hullencrypt/test.py
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-04-26 17:44:51.133825 hullencrypt-0.0.5/src/hullencrypt.egg-info/
+-rw-r--r--   0 john      (1000) john      (1000)     2052 2023-04-26 17:44:51.000000 hullencrypt-0.0.5/src/hullencrypt.egg-info/PKG-INFO
+-rw-r--r--   0 john      (1000) john      (1000)      274 2023-04-26 17:44:51.000000 hullencrypt-0.0.5/src/hullencrypt.egg-info/SOURCES.txt
+-rw-r--r--   0 john      (1000) john      (1000)        1 2023-04-26 17:44:51.000000 hullencrypt-0.0.5/src/hullencrypt.egg-info/dependency_links.txt
+-rw-r--r--   0 john      (1000) john      (1000)       21 2023-04-26 17:44:51.000000 hullencrypt-0.0.5/src/hullencrypt.egg-info/requires.txt
+-rw-r--r--   0 john      (1000) john      (1000)       12 2023-04-26 17:44:51.000000 hullencrypt-0.0.5/src/hullencrypt.egg-info/top_level.txt
```

### Comparing `hullencrypt-0.0.4/LICENSE` & `hullencrypt-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hullencrypt-0.0.4/PKG-INFO` & `hullencrypt-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hullencrypt
-Version: 0.0.4
+Version: 0.0.5
 Summary: A selfmade cryptolib for sharing passwords in a tree structure
 Author-email: John Janzen <rc-dev@johnjanzen.me>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `hullencrypt-0.0.4/README.md` & `hullencrypt-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `hullencrypt-0.0.4/src/hullencrypt/base.py` & `hullencrypt-0.0.5/src/hullencrypt/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -54,23 +54,15 @@
             return f.decrypt(self.enc_key)
 
     def get_content(self, key):
         assert self.content != None
         f = fernet.Fernet(key)
         return f.decrypt(self.content)
 
-    def set_password(self, password: bytes, parent_key: bytes=None, old_pass=None):
-        assert parent_key != None or old_pass != None
-        key = None
-        if parent_key:
-            key = self.get_key(parent_key=parent_key)
-        elif old_pas:
-            key = self.get_key(password=old_pass)
-        
-        assert key != None
+    def set_password(self, password: bytes, key: bytes):
         # this will fail if you have the wrong key
         # to make sure you have the correct key, call get_content
         self.get_content(key)
 
         password_key = self.get_key(parent_key=password)
         f = fernet.Fernet(password_key)
         self.enc_key = f.encrypt(key)
```

### Comparing `hullencrypt-0.0.4/src/hullencrypt/test.py` & `hullencrypt-0.0.5/src/hullencrypt/test.py`

 * *Files identical despite different names*

### Comparing `hullencrypt-0.0.4/src/hullencrypt.egg-info/PKG-INFO` & `hullencrypt-0.0.5/src/hullencrypt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hullencrypt
-Version: 0.0.4
+Version: 0.0.5
 Summary: A selfmade cryptolib for sharing passwords in a tree structure
 Author-email: John Janzen <rc-dev@johnjanzen.me>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

