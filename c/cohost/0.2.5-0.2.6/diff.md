# Comparing `tmp/cohost-0.2.5.tar.gz` & `tmp/cohost-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cohost-0.2.5.tar", last modified: Sun Apr  2 20:11:37 2023, max compression
+gzip compressed data, was "cohost-0.2.6.tar", last modified: Wed Apr 26 18:52:54 2023, max compression
```

## Comparing `cohost-0.2.5.tar` & `cohost-0.2.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 val.knight   (501) staff       (20)        0 2023-04-02 20:11:37.459676 cohost-0.2.5/
--rw-r--r--   0 val.knight   (501) staff       (20)     1072 2022-12-19 21:34:56.000000 cohost-0.2.5/LICENSE
--rw-r--r--   0 val.knight   (501) staff       (20)     6141 2023-04-02 20:11:37.459297 cohost-0.2.5/PKG-INFO
--rw-r--r--   0 val.knight   (501) staff       (20)     3983 2022-12-19 21:34:56.000000 cohost-0.2.5/README.md
-drwxr-xr-x   0 val.knight   (501) staff       (20)        0 2023-04-02 20:11:37.454028 cohost-0.2.5/cohost/
--rw-r--r--   0 val.knight   (501) staff       (20)       99 2022-12-19 21:34:56.000000 cohost-0.2.5/cohost/__init__.py
-drwxr-xr-x   0 val.knight   (501) staff       (20)        0 2023-04-02 20:11:37.458843 cohost-0.2.5/cohost/models/
--rw-r--r--   0 val.knight   (501) staff       (20)       26 2022-12-19 21:34:56.000000 cohost-0.2.5/cohost/models/__init__.py
--rw-r--r--   0 val.knight   (501) staff       (20)     4093 2022-12-19 21:34:56.000000 cohost-0.2.5/cohost/models/block.py
--rw-r--r--   0 val.knight   (501) staff       (20)      411 2022-12-19 21:34:56.000000 cohost-0.2.5/cohost/models/comment.py
--rw-r--r--   0 val.knight   (501) staff       (20)     8252 2023-04-02 20:02:17.000000 cohost-0.2.5/cohost/models/notification.py
--rw-r--r--   0 val.knight   (501) staff       (20)     3822 2022-12-19 21:34:56.000000 cohost-0.2.5/cohost/models/post.py
--rw-r--r--   0 val.knight   (501) staff       (20)    10506 2023-04-02 19:43:58.000000 cohost-0.2.5/cohost/models/project.py
--rw-r--r--   0 val.knight   (501) staff       (20)     5432 2023-04-02 19:43:58.000000 cohost-0.2.5/cohost/models/user.py
--rw-r--r--   0 val.knight   (501) staff       (20)     2967 2023-04-02 19:43:58.000000 cohost-0.2.5/cohost/network.py
-drwxr-xr-x   0 val.knight   (501) staff       (20)        0 2023-04-02 20:11:37.456183 cohost-0.2.5/cohost.egg-info/
--rw-r--r--   0 val.knight   (501) staff       (20)     6141 2023-04-02 20:11:37.000000 cohost-0.2.5/cohost.egg-info/PKG-INFO
--rw-r--r--   0 val.knight   (501) staff       (20)      391 2023-04-02 20:11:37.000000 cohost-0.2.5/cohost.egg-info/SOURCES.txt
--rw-r--r--   0 val.knight   (501) staff       (20)        1 2023-04-02 20:11:37.000000 cohost-0.2.5/cohost.egg-info/dependency_links.txt
--rw-r--r--   0 val.knight   (501) staff       (20)        9 2023-04-02 20:11:37.000000 cohost-0.2.5/cohost.egg-info/requires.txt
--rw-r--r--   0 val.knight   (501) staff       (20)        7 2023-04-02 20:11:37.000000 cohost-0.2.5/cohost.egg-info/top_level.txt
--rw-r--r--   0 val.knight   (501) staff       (20)     1124 2023-04-02 20:03:41.000000 cohost-0.2.5/pyproject.toml
--rw-r--r--   0 val.knight   (501) staff       (20)       38 2023-04-02 20:11:37.459811 cohost-0.2.5/setup.cfg
+drwxr-xr-x   0 valknight   (501) staff       (20)        0 2023-04-26 18:52:54.962380 cohost-0.2.6/
+-rw-r--r--   0 valknight   (501) staff       (20)     1072 2023-04-26 18:15:22.000000 cohost-0.2.6/LICENSE
+-rw-r--r--   0 valknight   (501) staff       (20)     6141 2023-04-26 18:52:54.961393 cohost-0.2.6/PKG-INFO
+-rw-r--r--   0 valknight   (501) staff       (20)     3983 2023-04-26 18:15:22.000000 cohost-0.2.6/README.md
+drwxr-xr-x   0 valknight   (501) staff       (20)        0 2023-04-26 18:52:54.938357 cohost-0.2.6/cohost/
+-rw-r--r--   0 valknight   (501) staff       (20)       99 2023-04-26 18:15:22.000000 cohost-0.2.6/cohost/__init__.py
+drwxr-xr-x   0 valknight   (501) staff       (20)        0 2023-04-26 18:52:54.957482 cohost-0.2.6/cohost/models/
+-rw-r--r--   0 valknight   (501) staff       (20)       26 2023-04-26 18:15:22.000000 cohost-0.2.6/cohost/models/__init__.py
+-rw-r--r--   0 valknight   (501) staff       (20)     4102 2023-04-26 18:49:55.000000 cohost-0.2.6/cohost/models/block.py
+-rw-r--r--   0 valknight   (501) staff       (20)      411 2023-04-26 18:15:22.000000 cohost-0.2.6/cohost/models/comment.py
+-rw-r--r--   0 valknight   (501) staff       (20)     8252 2023-04-26 18:15:22.000000 cohost-0.2.6/cohost/models/notification.py
+-rw-r--r--   0 valknight   (501) staff       (20)     3822 2023-04-26 18:15:22.000000 cohost-0.2.6/cohost/models/post.py
+-rw-r--r--   0 valknight   (501) staff       (20)    10506 2023-04-26 18:15:22.000000 cohost-0.2.6/cohost/models/project.py
+-rw-r--r--   0 valknight   (501) staff       (20)     5432 2023-04-26 18:15:22.000000 cohost-0.2.6/cohost/models/user.py
+-rw-r--r--   0 valknight   (501) staff       (20)     2967 2023-04-26 18:15:22.000000 cohost-0.2.6/cohost/network.py
+drwxr-xr-x   0 valknight   (501) staff       (20)        0 2023-04-26 18:52:54.943990 cohost-0.2.6/cohost.egg-info/
+-rw-r--r--   0 valknight   (501) staff       (20)     6141 2023-04-26 18:52:54.000000 cohost-0.2.6/cohost.egg-info/PKG-INFO
+-rw-r--r--   0 valknight   (501) staff       (20)      391 2023-04-26 18:52:54.000000 cohost-0.2.6/cohost.egg-info/SOURCES.txt
+-rw-r--r--   0 valknight   (501) staff       (20)        1 2023-04-26 18:52:54.000000 cohost-0.2.6/cohost.egg-info/dependency_links.txt
+-rw-r--r--   0 valknight   (501) staff       (20)        9 2023-04-26 18:52:54.000000 cohost-0.2.6/cohost.egg-info/requires.txt
+-rw-r--r--   0 valknight   (501) staff       (20)        7 2023-04-26 18:52:54.000000 cohost-0.2.6/cohost.egg-info/top_level.txt
+-rw-r--r--   0 valknight   (501) staff       (20)     1124 2023-04-26 18:51:57.000000 cohost-0.2.6/pyproject.toml
+-rw-r--r--   0 valknight   (501) staff       (20)       38 2023-04-26 18:52:54.962794 cohost-0.2.6/setup.cfg
```

### Comparing `cohost-0.2.5/LICENSE` & `cohost-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cohost-0.2.5/PKG-INFO` & `cohost-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cohost
-Version: 0.2.5
+Version: 0.2.6
 Summary: Unofficial Python API wrapper for Cohost.org - the fourth website!
 Author-email: Val Knight <val@valknight.xyz>
 Maintainer-email: Val Knight <val@valknight.xyz>
 License: MIT License
         
         Copyright (c) 2022 Vallerie Knight
```

### Comparing `cohost-0.2.5/README.md` & `cohost-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `cohost-0.2.5/cohost/models/block.py` & `cohost-0.2.6/cohost/models/block.py`

 * *Files 5% similar despite different names*

```diff
@@ -81,18 +81,18 @@
             return
         # we don't have an attachment ID! that means this file isn't tied to a cohost file
         # Step 1: tell cohost we're uploading a file, using project/v-dev/posts/53633/attach/start
         endpoint = 'project/{}/posts/{}/attach/start'.format(
             project.handle, postId)
 
         # example data: filename=VxwLMgKF_400x400.jpg&content_type=image%2Fjpeg&content_length=20829
-        dospacecreds = fetch('post', endpoint, {
+        dospacecreds = fetch('postjson', endpoint, {
             'filename': self.filename,
             'content_type': self.content_type,
-            'content_length': self.content_length
+            'content_length': int(self.content_length)
         }, generate_login_cookies(project.user.cookie))
         # Step 2: ok sick, we now have digitalocean creds to upload the image to Spaces
         # we need to use raw requests here, as we're not actually talking to cohost
         spacesUrl = dospacecreds.get('url')
         b = None
         with open(self.filepath, 'rb') as f:
             b = f.read()
```

### Comparing `cohost-0.2.5/cohost/models/notification.py` & `cohost-0.2.6/cohost/models/notification.py`

 * *Files identical despite different names*

### Comparing `cohost-0.2.5/cohost/models/post.py` & `cohost-0.2.6/cohost/models/post.py`

 * *Files identical despite different names*

### Comparing `cohost-0.2.5/cohost/models/project.py` & `cohost-0.2.6/cohost/models/project.py`

 * *Files identical despite different names*

### Comparing `cohost-0.2.5/cohost/models/user.py` & `cohost-0.2.6/cohost/models/user.py`

 * *Files identical despite different names*

### Comparing `cohost-0.2.5/cohost/network.py` & `cohost-0.2.6/cohost/network.py`

 * *Files identical despite different names*

### Comparing `cohost-0.2.5/cohost.egg-info/PKG-INFO` & `cohost-0.2.6/cohost.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cohost
-Version: 0.2.5
+Version: 0.2.6
 Summary: Unofficial Python API wrapper for Cohost.org - the fourth website!
 Author-email: Val Knight <val@valknight.xyz>
 Maintainer-email: Val Knight <val@valknight.xyz>
 License: MIT License
         
         Copyright (c) 2022 Vallerie Knight
```

### Comparing `cohost-0.2.5/pyproject.toml` & `cohost-0.2.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cohost"
-version = "0.2.5"
+version = "0.2.6"
 description = "Unofficial Python API wrapper for Cohost.org - the fourth website!"
 readme = "README.md"
 requires-python = ">=3.7"
 license = { file = "LICENSE" }
 keywords = [ "cohost.org", "cohost", "api" ]
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
```

