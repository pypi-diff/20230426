# Comparing `tmp/fortifyapi-3.1.3.tar.gz` & `tmp/fortifyapi-3.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fortifyapi-3.1.3.tar", last modified: Thu Sep  1 22:52:21 2022, max compression
+gzip compressed data, was "fortifyapi-3.1.4.tar", last modified: Wed Apr 26 13:45:10 2023, max compression
```

## Comparing `fortifyapi-3.1.3.tar` & `fortifyapi-3.1.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-01 22:52:21.572327 fortifyapi-3.1.3/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1046 2022-09-01 22:52:14.000000 fortifyapi-3.1.3/LICENSE.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       29 2022-09-01 22:52:14.000000 fortifyapi-3.1.3/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3896 2022-09-01 22:52:21.572327 fortifyapi-3.1.3/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2228 2022-09-01 22:52:14.000000 fortifyapi-3.1.3/README.rst
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-01 22:52:21.572327 fortifyapi-3.1.3/docs/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7460 2022-09-01 22:52:14.000000 fortifyapi-3.1.3/docs/README.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      329 2022-09-01 22:52:14.000000 fortifyapi-3.1.3/docs/couscous.yml
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-01 22:52:21.572327 fortifyapi-3.1.3/fortifyapi/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      174 2022-09-01 22:52:14.000000 fortifyapi-3.1.3/fortifyapi/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6749 2022-09-01 22:52:14.000000 fortifyapi-3.1.3/fortifyapi/api.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    27796 2022-09-01 22:52:14.000000 fortifyapi-3.1.3/fortifyapi/client.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      283 2022-09-01 22:52:14.000000 fortifyapi-3.1.3/fortifyapi/exceptions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    39501 2022-09-01 22:52:14.000000 fortifyapi-3.1.3/fortifyapi/fortify.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1007 2022-09-01 22:52:14.000000 fortifyapi-3.1.3/fortifyapi/query.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7013 2022-09-01 22:52:14.000000 fortifyapi-3.1.3/fortifyapi/template.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-01 22:52:21.572327 fortifyapi-3.1.3/fortifyapi.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3896 2022-09-01 22:52:21.000000 fortifyapi-3.1.3/fortifyapi.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      436 2022-09-01 22:52:21.000000 fortifyapi-3.1.3/fortifyapi.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-09-01 22:52:21.000000 fortifyapi-3.1.3/fortifyapi.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        9 2022-09-01 22:52:21.000000 fortifyapi-3.1.3/fortifyapi.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       11 2022-09-01 22:52:21.000000 fortifyapi-3.1.3/fortifyapi.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-09-01 22:52:21.000000 fortifyapi-3.1.3/fortifyapi.egg-info/zip-safe
--rw-r--r--   0 circleci  (3434) circleci  (3434)      106 2022-09-01 22:52:21.572327 fortifyapi-3.1.3/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2078 2022-09-01 22:52:14.000000 fortifyapi-3.1.3/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 13:45:10.799162 fortifyapi-3.1.4/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1046 2023-04-26 13:45:03.000000 fortifyapi-3.1.4/LICENSE.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       29 2023-04-26 13:45:03.000000 fortifyapi-3.1.4/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3896 2023-04-26 13:45:10.799162 fortifyapi-3.1.4/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2228 2023-04-26 13:45:03.000000 fortifyapi-3.1.4/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 13:45:10.795162 fortifyapi-3.1.4/docs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7460 2023-04-26 13:45:03.000000 fortifyapi-3.1.4/docs/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      329 2023-04-26 13:45:03.000000 fortifyapi-3.1.4/docs/couscous.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 13:45:10.795162 fortifyapi-3.1.4/fortifyapi/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      174 2023-04-26 13:45:03.000000 fortifyapi-3.1.4/fortifyapi/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6749 2023-04-26 13:45:03.000000 fortifyapi-3.1.4/fortifyapi/api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    27850 2023-04-26 13:45:03.000000 fortifyapi-3.1.4/fortifyapi/client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      283 2023-04-26 13:45:03.000000 fortifyapi-3.1.4/fortifyapi/exceptions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    39501 2023-04-26 13:45:03.000000 fortifyapi-3.1.4/fortifyapi/fortify.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1007 2023-04-26 13:45:03.000000 fortifyapi-3.1.4/fortifyapi/query.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7013 2023-04-26 13:45:03.000000 fortifyapi-3.1.4/fortifyapi/template.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 13:45:10.799162 fortifyapi-3.1.4/fortifyapi.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3896 2023-04-26 13:45:10.000000 fortifyapi-3.1.4/fortifyapi.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      436 2023-04-26 13:45:10.000000 fortifyapi-3.1.4/fortifyapi.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-04-26 13:45:10.000000 fortifyapi-3.1.4/fortifyapi.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        9 2023-04-26 13:45:10.000000 fortifyapi-3.1.4/fortifyapi.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       11 2023-04-26 13:45:10.000000 fortifyapi-3.1.4/fortifyapi.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-04-26 13:45:10.000000 fortifyapi-3.1.4/fortifyapi.egg-info/zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      106 2023-04-26 13:45:10.799162 fortifyapi-3.1.4/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2078 2023-04-26 13:45:03.000000 fortifyapi-3.1.4/setup.py
```

### Comparing `fortifyapi-3.1.3/LICENSE.txt` & `fortifyapi-3.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fortifyapi-3.1.3/PKG-INFO` & `fortifyapi-3.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: fortifyapi
-Version: 3.1.3
+Version: 3.1.4
 Summary: Python library for Fortify Software Security Center (SSC) RESTFul API
 Home-page: https://github.com/fortifyadmin/fortifyapi
 Author: Brandon Spruth, Matthew Gill
 Author-email: brandon@spruth.co, mgill@c0ffee.me
 License: MIT
-Download-URL: https://github.com/fortifyadmin/fortifyapi/tarball/3.1.3
+Download-URL: https://github.com/fortifyadmin/fortifyapi/tarball/3.1.4
 Description: .. image:: https://img.shields.io/pypi/v/fortifyapi.svg
         .. image:: https://img.shields.io/pypi/pyversions/fortifyapi.svg
         .. image:: https://img.shields.io/circleci/build/github/fortifyadmin/fortifyapi/master?logo=CircleCI
         
         Fortify API
         ***********
```

### Comparing `fortifyapi-3.1.3/README.rst` & `fortifyapi-3.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `fortifyapi-3.1.3/docs/README.md` & `fortifyapi-3.1.4/docs/README.md`

 * *Files identical despite different names*

### Comparing `fortifyapi-3.1.3/fortifyapi/api.py` & `fortifyapi-3.1.4/fortifyapi/api.py`

 * *Files identical despite different names*

### Comparing `fortifyapi-3.1.3/fortifyapi/client.py` & `fortifyapi-3.1.4/fortifyapi/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         self.projects = Project(self._api, None, self)
         self.pools = CloudPool(self._api, None, self)
         self.workers = CloudWorker(self._api, None, self)
         self.jobs = CloudJob(self._api, None, self)
         self.reports = Report(self._api, None, self)
         self.auth_entities = AuthEntity(self._api, None, self)
         self.ldap_user = LdapUser(self._api, None, self)
-        self.rulepack = Rulepack(self._api, None, self)
+        self.rulepacks = Rulepack(self._api, None, self)
 
     def _list(self, endpoint, **kwargs):
         with self._api as api:
             for e in api.page_data(endpoint, **kwargs):
                 yield e
 
     def list_engine_types(self, **kwargs):
@@ -642,35 +642,37 @@
     def revoke(self):
         f"/api/v1/tokens/revoke"  # POST with body
         raise NotImplementedError()
 
 
 class Rulepack(SSCObject):
 
+    def get(self):
+        with self._api as api:
+            return Rulepack(self._api, api.get(f"/api/v1/coreRulepacks")['data'], self.parent)
+
     def list(self, **kwargs):
         with self._api as api:
             for e in api.page_data(f"/api/v1/coreRulepacks", **kwargs):
                 yield Rulepack(self._api, e, self.parent)
 
     def upload(self):
+        #TODO: need to implement this
         f"/api/v1/coreRulepacks" # POST
         raise NotImplementedError()
 
     def delete(self):
-        f"/api/v1/coreRulepacks/{self['id']}"  # DELETE
-        raise NotImplementedError()
+        self.assert_is_instance()
+        with self._api as api:
+            return api.delete(f"/api/v1/coreRulepacks/{self['id']}")
 
     def update(self):
-        try:
-            with self._api as api:
-                for rules in api.page_data(f"/api/v1/updateRulepacks"):
-                    yield Rulepack(self._api, rules, self.parent)
-        except KeyError:
-            #TODO: remove print - why is this except here anyway? what key error?
-            print(f"{rules['message']}")
+        with self._api as api:
+            for rules in api.page_data(f"/api/v1/updateRulepacks"):
+                yield Rulepack(self._api, rules, self.parent)
 
 
 class CustomTag(SSCObject):
     """ Specifically for project versions """
 
     def list(self, **kwargs):
         with self._api as api:
```

### Comparing `fortifyapi-3.1.3/fortifyapi/fortify.py` & `fortifyapi-3.1.4/fortifyapi/fortify.py`

 * *Files identical despite different names*

### Comparing `fortifyapi-3.1.3/fortifyapi/query.py` & `fortifyapi-3.1.4/fortifyapi/query.py`

 * *Files identical despite different names*

### Comparing `fortifyapi-3.1.3/fortifyapi/template.py` & `fortifyapi-3.1.4/fortifyapi/template.py`

 * *Files identical despite different names*

### Comparing `fortifyapi-3.1.3/fortifyapi.egg-info/PKG-INFO` & `fortifyapi-3.1.4/fortifyapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: fortifyapi
-Version: 3.1.3
+Version: 3.1.4
 Summary: Python library for Fortify Software Security Center (SSC) RESTFul API
 Home-page: https://github.com/fortifyadmin/fortifyapi
 Author: Brandon Spruth, Matthew Gill
 Author-email: brandon@spruth.co, mgill@c0ffee.me
 License: MIT
-Download-URL: https://github.com/fortifyadmin/fortifyapi/tarball/3.1.3
+Download-URL: https://github.com/fortifyadmin/fortifyapi/tarball/3.1.4
 Description: .. image:: https://img.shields.io/pypi/v/fortifyapi.svg
         .. image:: https://img.shields.io/pypi/pyversions/fortifyapi.svg
         .. image:: https://img.shields.io/circleci/build/github/fortifyadmin/fortifyapi/master?logo=CircleCI
         
         Fortify API
         ***********
```

### Comparing `fortifyapi-3.1.3/setup.py` & `fortifyapi-3.1.4/setup.py`

 * *Files identical despite different names*

