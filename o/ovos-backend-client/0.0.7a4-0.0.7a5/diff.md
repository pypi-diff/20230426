# Comparing `tmp/ovos-backend-client-0.0.7a4.tar.gz` & `tmp/ovos-backend-client-0.0.7a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-backend-client-0.0.7a4.tar", last modified: Sat Apr 22 00:11:40 2023, max compression
+gzip compressed data, was "ovos-backend-client-0.0.7a5.tar", last modified: Tue Apr 25 14:59:56 2023, max compression
```

## Comparing `ovos-backend-client-0.0.7a4.tar` & `ovos-backend-client-0.0.7a5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:11:40.461818 ovos-backend-client-0.0.7a4/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-22 00:11:40.461818 ovos-backend-client-0.0.7a4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-04-22 00:11:30.000000 ovos-backend-client-0.0.7a4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:11:40.461818 ovos-backend-client-0.0.7a4/ovos_backend_client/
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-22 00:11:30.000000 ovos-backend-client-0.0.7a4/ovos_backend_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21426 2023-04-22 00:11:30.000000 ovos-backend-client-0.0.7a4/ovos_backend_client/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:11:40.461818 ovos-backend-client-0.0.7a4/ovos_backend_client/backends/
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-04-22 00:11:30.000000 ovos-backend-client-0.0.7a4/ovos_backend_client/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16318 2023-04-22 00:11:30.000000 ovos-backend-client-0.0.7a4/ovos_backend_client/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    22979 2023-04-22 00:11:30.000000 ovos-backend-client-0.0.7a4/ovos_backend_client/backends/offline.py
--rw-r--r--   0 runner    (1001) docker     (123)     8991 2023-04-22 00:11:30.000000 ovos-backend-client-0.0.7a4/ovos_backend_client/backends/ovos.py
--rw-r--r--   0 runner    (1001) docker     (123)    18041 2023-04-22 00:11:30.000000 ovos-backend-client-0.0.7a4/ovos_backend_client/backends/personal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-22 00:11:30.000000 ovos-backend-client-0.0.7a4/ovos_backend_client/backends/selene.py
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-04-22 00:11:30.000000 ovos-backend-client-0.0.7a4/ovos_backend_client/cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-04-22 00:11:30.000000 ovos-backend-client-0.0.7a4/ovos_backend_client/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-04-22 00:11:30.000000 ovos-backend-client-0.0.7a4/ovos_backend_client/database.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-22 00:11:30.000000 ovos-backend-client-0.0.7a4/ovos_backend_client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-04-22 00:11:30.000000 ovos-backend-client-0.0.7a4/ovos_backend_client/identity.py
--rw-r--r--   0 runner    (1001) docker     (123)    12079 2023-04-22 00:11:30.000000 ovos-backend-client-0.0.7a4/ovos_backend_client/pairing.py
--rw-r--r--   0 runner    (1001) docker     (123)    15623 2023-04-22 00:11:30.000000 ovos-backend-client-0.0.7a4/ovos_backend_client/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-22 00:11:33.000000 ovos-backend-client-0.0.7a4/ovos_backend_client/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:11:40.461818 ovos-backend-client-0.0.7a4/ovos_backend_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-22 00:11:40.000000 ovos-backend-client-0.0.7a4/ovos_backend_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-22 00:11:40.000000 ovos-backend-client-0.0.7a4/ovos_backend_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 00:11:40.000000 ovos-backend-client-0.0.7a4/ovos_backend_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-22 00:11:40.000000 ovos-backend-client-0.0.7a4/ovos_backend_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-22 00:11:40.000000 ovos-backend-client-0.0.7a4/ovos_backend_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 00:11:40.461818 ovos-backend-client-0.0.7a4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-22 00:11:30.000000 ovos-backend-client-0.0.7a4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:59:56.823380 ovos-backend-client-0.0.7a5/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-25 14:59:56.823380 ovos-backend-client-0.0.7a5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-04-25 14:59:40.000000 ovos-backend-client-0.0.7a5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:59:56.819379 ovos-backend-client-0.0.7a5/ovos_backend_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-25 14:59:40.000000 ovos-backend-client-0.0.7a5/ovos_backend_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21426 2023-04-25 14:59:40.000000 ovos-backend-client-0.0.7a5/ovos_backend_client/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:59:56.823380 ovos-backend-client-0.0.7a5/ovos_backend_client/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-04-25 14:59:40.000000 ovos-backend-client-0.0.7a5/ovos_backend_client/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16318 2023-04-25 14:59:40.000000 ovos-backend-client-0.0.7a5/ovos_backend_client/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22979 2023-04-25 14:59:40.000000 ovos-backend-client-0.0.7a5/ovos_backend_client/backends/offline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8991 2023-04-25 14:59:40.000000 ovos-backend-client-0.0.7a5/ovos_backend_client/backends/ovos.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18134 2023-04-25 14:59:40.000000 ovos-backend-client-0.0.7a5/ovos_backend_client/backends/personal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-25 14:59:40.000000 ovos-backend-client-0.0.7a5/ovos_backend_client/backends/selene.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-04-25 14:59:40.000000 ovos-backend-client-0.0.7a5/ovos_backend_client/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-04-25 14:59:40.000000 ovos-backend-client-0.0.7a5/ovos_backend_client/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-04-25 14:59:40.000000 ovos-backend-client-0.0.7a5/ovos_backend_client/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-25 14:59:40.000000 ovos-backend-client-0.0.7a5/ovos_backend_client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-04-25 14:59:40.000000 ovos-backend-client-0.0.7a5/ovos_backend_client/identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12079 2023-04-25 14:59:40.000000 ovos-backend-client-0.0.7a5/ovos_backend_client/pairing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15623 2023-04-25 14:59:40.000000 ovos-backend-client-0.0.7a5/ovos_backend_client/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-25 14:59:46.000000 ovos-backend-client-0.0.7a5/ovos_backend_client/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:59:56.823380 ovos-backend-client-0.0.7a5/ovos_backend_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-25 14:59:56.000000 ovos-backend-client-0.0.7a5/ovos_backend_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-25 14:59:56.000000 ovos-backend-client-0.0.7a5/ovos_backend_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 14:59:56.000000 ovos-backend-client-0.0.7a5/ovos_backend_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-25 14:59:56.000000 ovos-backend-client-0.0.7a5/ovos_backend_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-25 14:59:56.000000 ovos-backend-client-0.0.7a5/ovos_backend_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 14:59:56.823380 ovos-backend-client-0.0.7a5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-25 14:59:40.000000 ovos-backend-client-0.0.7a5/setup.py
```

### Comparing `ovos-backend-client-0.0.7a4/README.md` & `ovos-backend-client-0.0.7a5/README.md`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.0.7a4/ovos_backend_client/api.py` & `ovos-backend-client-0.0.7a5/ovos_backend_client/api.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.0.7a4/ovos_backend_client/backends/__init__.py` & `ovos-backend-client-0.0.7a5/ovos_backend_client/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.0.7a4/ovos_backend_client/backends/base.py` & `ovos-backend-client-0.0.7a5/ovos_backend_client/backends/base.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.0.7a4/ovos_backend_client/backends/offline.py` & `ovos-backend-client-0.0.7a5/ovos_backend_client/backends/offline.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.0.7a4/ovos_backend_client/backends/ovos.py` & `ovos-backend-client-0.0.7a5/ovos_backend_client/backends/ovos.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.0.7a4/ovos_backend_client/backends/personal.py` & `ovos-backend-client-0.0.7a5/ovos_backend_client/backends/personal.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 class PersonalBackend(AbstractPartialBackend):
 
     def __init__(self, url="http://0.0.0.0:6712", version="v1", identity_file=None, credentials=None):
         super().__init__(url, version, identity_file, BackendType.PERSONAL, credentials)
 
     def refresh_token(self):
         try:
+            self.identity.get() # Ensure loading so identity property doesn't cause deadlock
             identity_lock.acquire(blocking=False)
             # NOTE: requests needs to be used instead of self.get due to self.get calling this
             data = requests.get(f"{self.backend_url}/{self.backend_version}/auth/token", headers=self.headers).json()
             IdentityManager.save(data, lock=False)
             LOG.debug('Saved credentials')
         except:
             LOG.warning("Failed to refresh access token")
```

### Comparing `ovos-backend-client-0.0.7a4/ovos_backend_client/backends/selene.py` & `ovos-backend-client-0.0.7a5/ovos_backend_client/backends/selene.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.0.7a4/ovos_backend_client/cloud.py` & `ovos-backend-client-0.0.7a5/ovos_backend_client/cloud.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.0.7a4/ovos_backend_client/config.py` & `ovos-backend-client-0.0.7a5/ovos_backend_client/config.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.0.7a4/ovos_backend_client/database.py` & `ovos-backend-client-0.0.7a5/ovos_backend_client/database.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.0.7a4/ovos_backend_client/identity.py` & `ovos-backend-client-0.0.7a5/ovos_backend_client/identity.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.0.7a4/ovos_backend_client/pairing.py` & `ovos-backend-client-0.0.7a5/ovos_backend_client/pairing.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.0.7a4/ovos_backend_client/settings.py` & `ovos-backend-client-0.0.7a5/ovos_backend_client/settings.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.0.7a4/ovos_backend_client.egg-info/SOURCES.txt` & `ovos-backend-client-0.0.7a5/ovos_backend_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.0.7a4/setup.py` & `ovos-backend-client-0.0.7a5/setup.py`

 * *Files identical despite different names*

