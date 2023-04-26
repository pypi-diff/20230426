# Comparing `tmp/urihandler-1.1.0.tar.gz` & `tmp/urihandler-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/urihandler-1.1.0.tar", last modified: Mon Feb 27 13:36:15 2023, max compression
+gzip compressed data, was "urihandler-1.2.0.tar", last modified: Tue Apr 25 07:23:39 2023, max compression
```

## Comparing `urihandler-1.1.0.tar` & `urihandler-1.2.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxrwxr-x   0 goessebr  (1001) goessebr  (1001)        0 2023-02-27 13:36:15.000000 urihandler-1.1.0/
--rw-rw-r--   0 goessebr  (1001) goessebr  (1001)      567 2023-02-10 06:02:12.000000 urihandler-1.1.0/.pre-commit-config.yaml
--rw-rw-r--   0 goessebr  (1001) goessebr  (1001)      724 2023-02-27 13:26:54.000000 urihandler-1.1.0/CHANGES.rst
--rw-rw-r--   0 goessebr  (1001) goessebr  (1001)       51 2023-02-10 06:02:12.000000 urihandler-1.1.0/MANIFEST.in
--rw-rw-r--   0 goessebr  (1001) goessebr  (1001)     3450 2023-02-27 13:36:15.000000 urihandler-1.1.0/PKG-INFO
--rw-rw-r--   0 goessebr  (1001) goessebr  (1001)     1562 2023-02-10 06:02:12.000000 urihandler-1.1.0/README.rst
--rw-rw-r--   0 goessebr  (1001) goessebr  (1001)     1105 2023-02-10 06:02:12.000000 urihandler-1.1.0/development.ini
--rw-rw-r--   0 goessebr  (1001) goessebr  (1001)      931 2023-02-10 06:02:12.000000 urihandler-1.1.0/production.ini
--rw-rw-r--   0 goessebr  (1001) goessebr  (1001)      293 2023-02-17 10:48:28.000000 urihandler-1.1.0/requirements-dev.txt
--rw-rw-r--   0 goessebr  (1001) goessebr  (1001)       25 2023-02-10 06:02:12.000000 urihandler-1.1.0/requirements.txt
--rw-rw-r--   0 goessebr  (1001) goessebr  (1001)      372 2023-02-10 06:02:12.000000 urihandler-1.1.0/sample.yaml
--rw-rw-r--   0 goessebr  (1001) goessebr  (1001)       38 2023-02-27 13:36:15.000000 urihandler-1.1.0/setup.cfg
--rw-rw-r--   0 goessebr  (1001) goessebr  (1001)     1232 2023-02-27 13:22:16.000000 urihandler-1.1.0/setup.py
--rw-rw-r--   0 goessebr  (1001) goessebr  (1001)      384 2023-02-10 06:02:12.000000 urihandler-1.1.0/tox.ini
-drwxrwxr-x   0 goessebr  (1001) goessebr  (1001)        0 2023-02-27 13:36:15.000000 urihandler-1.1.0/urihandler/
--rw-rw-r--   0 goessebr  (1001) goessebr  (1001)     2509 2023-02-17 10:48:28.000000 urihandler-1.1.0/urihandler/__init__.py
--rw-rw-r--   0 goessebr  (1001) goessebr  (1001)     3091 2023-02-27 13:29:18.000000 urihandler-1.1.0/urihandler/handler.py
--rw-rw-r--   0 goessebr  (1001) goessebr  (1001)      550 2023-02-10 06:02:12.000000 urihandler-1.1.0/urihandler/utils.py
--rw-rw-r--   0 goessebr  (1001) goessebr  (1001)     1642 2023-02-10 06:02:12.000000 urihandler-1.1.0/urihandler/views.py
-drwxrwxr-x   0 goessebr  (1001) goessebr  (1001)        0 2023-02-27 13:36:15.000000 urihandler-1.1.0/urihandler.egg-info/
--rw-rw-r--   0 goessebr  (1001) goessebr  (1001)     3450 2023-02-27 13:36:15.000000 urihandler-1.1.0/urihandler.egg-info/PKG-INFO
--rw-rw-r--   0 goessebr  (1001) goessebr  (1001)      480 2023-02-27 13:36:15.000000 urihandler-1.1.0/urihandler.egg-info/SOURCES.txt
--rw-rw-r--   0 goessebr  (1001) goessebr  (1001)        1 2023-02-27 13:36:15.000000 urihandler-1.1.0/urihandler.egg-info/dependency_links.txt
--rw-rw-r--   0 goessebr  (1001) goessebr  (1001)       61 2023-02-27 13:36:15.000000 urihandler-1.1.0/urihandler.egg-info/entry_points.txt
--rw-rw-r--   0 goessebr  (1001) goessebr  (1001)        1 2023-02-27 13:36:15.000000 urihandler-1.1.0/urihandler.egg-info/not-zip-safe
--rw-rw-r--   0 goessebr  (1001) goessebr  (1001)       15 2023-02-27 13:36:15.000000 urihandler-1.1.0/urihandler.egg-info/requires.txt
--rw-rw-r--   0 goessebr  (1001) goessebr  (1001)       11 2023-02-27 13:36:15.000000 urihandler-1.1.0/urihandler.egg-info/top_level.txt
+drwxr-xr-x   0 geuensjo   (501) staff       (20)        0 2023-04-25 07:23:39.542507 urihandler-1.2.0/
+-rw-r--r--   0 geuensjo   (501) staff       (20)      567 2023-04-25 06:51:20.000000 urihandler-1.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 geuensjo   (501) staff       (20)      796 2023-04-25 06:51:20.000000 urihandler-1.2.0/CHANGES.rst
+-rw-r--r--   0 geuensjo   (501) staff       (20)    35120 2023-04-25 06:51:20.000000 urihandler-1.2.0/LICENSE
+-rw-r--r--   0 geuensjo   (501) staff       (20)       51 2023-04-25 06:51:20.000000 urihandler-1.2.0/MANIFEST.in
+-rw-r--r--   0 geuensjo   (501) staff       (20)     2977 2023-04-25 07:23:39.542330 urihandler-1.2.0/PKG-INFO
+-rw-r--r--   0 geuensjo   (501) staff       (20)     1562 2023-04-25 06:51:20.000000 urihandler-1.2.0/README.rst
+-rw-r--r--   0 geuensjo   (501) staff       (20)     1105 2023-04-25 06:51:20.000000 urihandler-1.2.0/development.ini
+-rw-r--r--   0 geuensjo   (501) staff       (20)      931 2023-04-25 06:51:20.000000 urihandler-1.2.0/production.ini
+-rw-r--r--   0 geuensjo   (501) staff       (20)      293 2023-04-25 06:51:20.000000 urihandler-1.2.0/requirements-dev.txt
+-rw-r--r--   0 geuensjo   (501) staff       (20)       25 2023-04-25 06:51:20.000000 urihandler-1.2.0/requirements.txt
+-rw-r--r--   0 geuensjo   (501) staff       (20)      372 2023-04-25 06:51:20.000000 urihandler-1.2.0/sample.yaml
+-rw-r--r--   0 geuensjo   (501) staff       (20)       38 2023-04-25 07:23:39.542562 urihandler-1.2.0/setup.cfg
+-rw-r--r--   0 geuensjo   (501) staff       (20)     1232 2023-04-25 06:51:20.000000 urihandler-1.2.0/setup.py
+-rw-r--r--   0 geuensjo   (501) staff       (20)      384 2023-04-25 06:51:20.000000 urihandler-1.2.0/tox.ini
+drwxr-xr-x   0 geuensjo   (501) staff       (20)        0 2023-04-25 07:23:39.541105 urihandler-1.2.0/urihandler/
+-rw-r--r--   0 geuensjo   (501) staff       (20)     2509 2023-04-25 06:51:20.000000 urihandler-1.2.0/urihandler/__init__.py
+-rw-r--r--   0 geuensjo   (501) staff       (20)     3309 2023-04-25 06:51:20.000000 urihandler-1.2.0/urihandler/handler.py
+-rw-r--r--   0 geuensjo   (501) staff       (20)      550 2023-04-25 06:51:20.000000 urihandler-1.2.0/urihandler/utils.py
+-rw-r--r--   0 geuensjo   (501) staff       (20)     1642 2023-04-25 06:51:20.000000 urihandler-1.2.0/urihandler/views.py
+drwxr-xr-x   0 geuensjo   (501) staff       (20)        0 2023-04-25 07:23:39.542129 urihandler-1.2.0/urihandler.egg-info/
+-rw-r--r--   0 geuensjo   (501) staff       (20)     2977 2023-04-25 07:23:39.000000 urihandler-1.2.0/urihandler.egg-info/PKG-INFO
+-rw-r--r--   0 geuensjo   (501) staff       (20)      488 2023-04-25 07:23:39.000000 urihandler-1.2.0/urihandler.egg-info/SOURCES.txt
+-rw-r--r--   0 geuensjo   (501) staff       (20)        1 2023-04-25 07:23:39.000000 urihandler-1.2.0/urihandler.egg-info/dependency_links.txt
+-rw-r--r--   0 geuensjo   (501) staff       (20)       43 2023-04-25 07:23:39.000000 urihandler-1.2.0/urihandler.egg-info/entry_points.txt
+-rw-r--r--   0 geuensjo   (501) staff       (20)        1 2023-04-25 07:23:34.000000 urihandler-1.2.0/urihandler.egg-info/not-zip-safe
+-rw-r--r--   0 geuensjo   (501) staff       (20)       15 2023-04-25 07:23:39.000000 urihandler-1.2.0/urihandler.egg-info/requires.txt
+-rw-r--r--   0 geuensjo   (501) staff       (20)       11 2023-04-25 07:23:39.000000 urihandler-1.2.0/urihandler.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `urihandler-1.1.0/.pre-commit-config.yaml` & `urihandler-1.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `urihandler-1.1.0/CHANGES.rst` & `urihandler-1.2.0/CHANGES.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,13 @@
-1.0.0 (27-02-2023)
+1.2.0 (25-04-2023)
+------------------
+
+- URL parameters meegeven (#92)
+
+1.1.0 (27-02-2023)
 ------------------
 
 - Onderscheid op accept header toelaten (#86)
 
 
 1.0.0 (06-07-2022)
 ------------------
```

### Comparing `urihandler-1.1.0/README.rst` & `urihandler-1.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `urihandler-1.1.0/development.ini` & `urihandler-1.2.0/development.ini`

 * *Files identical despite different names*

### Comparing `urihandler-1.1.0/production.ini` & `urihandler-1.2.0/production.ini`

 * *Files identical despite different names*

### Comparing `urihandler-1.1.0/setup.py` & `urihandler-1.2.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 with open(os.path.join(here, "CHANGES.rst")) as f:
     CHANGES = f.read()
 
 requires = ["pyramid", "PyYAML"]
 
 setup(
     name="urihandler",
-    version="1.1.0",
+    version="1.2.0",
     description="A tiny application that handles (cool) uri's.",
     long_description=README + "\n\n" + CHANGES,
     classifiers=[
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.8",
         "Framework :: Pyramid",
```

### Comparing `urihandler-1.1.0/urihandler/__init__.py` & `urihandler-1.2.0/urihandler/__init__.py`

 * *Files identical despite different names*

### Comparing `urihandler-1.1.0/urihandler/handler.py` & `urihandler-1.2.0/urihandler/handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,17 @@
     Central handler that deals with redirecting uri's.
     """
 
     def __init__(self, uris=[]):
         self.uris = uris
 
     def handle(self, uri, request):
+        params = ""
+        if "?" in uri:
+            uri, params = uri.split("?", 1)
         uris = copy.deepcopy(self.uris)
         for u in uris:
             if "mount" not in u or u["mount"]:
                 if u["match"].startswith("^"):
                     u["match"] = u["match"].replace("^", "^" + request.host_url)
                 else:
                     u["match"] = request.host_url + "/.*" + u["match"]
@@ -33,15 +36,18 @@
             m = re.match(u["match"], uri)
             if m:
                 redirect = u["redirect"]
                 if isinstance(redirect, dict):
                     redirect = self._get_redirect_based_on_accept_header(
                         request.accept, redirect
                     )
-                redirect = redirect.format(**m.groupdict())
+                if params:
+                    redirect = f"{redirect.format(**m.groupdict())}?{params}"
+                else:
+                    redirect = redirect.format(**m.groupdict())
                 log.debug(f"Match found. Redirecting to {redirect}.")
                 return redirect
         return None
 
     def _get_redirect_based_on_accept_header(self, accept_header, redirect_rule):
         """
         Return the redirect rule based on accept header.
```

### Comparing `urihandler-1.1.0/urihandler/utils.py` & `urihandler-1.2.0/urihandler/utils.py`

 * *Files identical despite different names*

### Comparing `urihandler-1.1.0/urihandler/views.py` & `urihandler-1.2.0/urihandler/views.py`

 * *Files identical despite different names*

