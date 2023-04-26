# Comparing `tmp/netsuite_python-1.5.4.tar.gz` & `tmp/netsuite_python-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netsuite_python-1.5.4.tar", last modified: Tue Apr 25 18:29:39 2023, max compression
+gzip compressed data, was "netsuite_python-1.5.5.tar", last modified: Tue Apr 25 18:31:14 2023, max compression
```

## Comparing `netsuite_python-1.5.4.tar` & `netsuite_python-1.5.5.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 18:29:39.128893 netsuite_python-1.5.4/
--rw-rw-rw-   0        0        0     5636 2023-04-25 18:29:39.128893 netsuite_python-1.5.4/PKG-INFO
--rw-rw-rw-   0        0        0     5306 2023-04-25 18:29:11.000000 netsuite_python-1.5.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-25 18:29:39.110894 netsuite_python-1.5.4/netsuite/
--rw-rw-rw-   0        0        0    12074 2023-04-25 18:20:23.000000 netsuite_python-1.5.4/netsuite/Netsuite.py
--rw-rw-rw-   0        0        0      494 2023-02-12 19:28:31.000000 netsuite_python-1.5.4/netsuite/NetsuiteToken.py
--rw-rw-rw-   0        0        0       74 2023-02-12 19:28:31.000000 netsuite_python-1.5.4/netsuite/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 18:29:39.114892 netsuite_python-1.5.4/netsuite/api_clients/
--rw-rw-rw-   0        0        0      235 2023-04-09 19:43:22.000000 netsuite_python-1.5.4/netsuite/api_clients/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 18:29:39.116893 netsuite_python-1.5.4/netsuite/api_clients/api/
--rw-rw-rw-   0        0        0       59 2023-04-09 19:48:25.000000 netsuite_python-1.5.4/netsuite/api_clients/api/__init__.py
--rw-rw-rw-   0        0        0     5489 2023-04-09 19:49:23.000000 netsuite_python-1.5.4/netsuite/api_clients/api/query_api.py
--rw-rw-rw-   0        0        0     2249 2023-04-09 19:48:25.000000 netsuite_python-1.5.4/netsuite/api_clients/api/restlet_api.py
--rw-rw-rw-   0        0        0    25577 2023-04-09 19:51:26.000000 netsuite_python-1.5.4/netsuite/api_clients/api_client.py
--rw-rw-rw-   0        0        0     8466 2023-03-23 15:55:18.000000 netsuite_python-1.5.4/netsuite/api_clients/configuration.py
--rw-rw-rw-   0        0        0    13259 2023-04-06 18:39:08.000000 netsuite_python-1.5.4/netsuite/api_clients/rest.py
--rw-rw-rw-   0        0        0      243 2023-02-12 19:28:31.000000 netsuite_python-1.5.4/netsuite/exceptions.py
--rw-rw-rw-   0        0        0     3921 2023-02-12 19:28:31.000000 netsuite_python-1.5.4/netsuite/module_loading.py
-drwxrwxrwx   0        0        0        0 2023-04-25 18:29:39.118895 netsuite_python-1.5.4/netsuite/netsuite_rest_client/
--rw-rw-rw-   0        0        0        0 2023-04-25 17:05:59.000000 netsuite_python-1.5.4/netsuite/netsuite_rest_client/__init__.py
--rw-rw-rw-   0        0        0      463 2023-04-17 18:07:52.000000 netsuite_python-1.5.4/netsuite/netsuite_rest_client/rest_api_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 18:29:39.119893 netsuite_python-1.5.4/netsuite/scripts/
--rw-rw-rw-   0        0        0        0 2023-02-12 19:28:31.000000 netsuite_python-1.5.4/netsuite/scripts/__init__.py
--rw-rw-rw-   0        0        0    11109 2023-04-25 18:27:59.000000 netsuite_python-1.5.4/netsuite/scripts/cli.py
--rw-rw-rw-   0        0        0     6300 2023-04-17 18:30:20.000000 netsuite_python-1.5.4/netsuite/settings.py
-drwxrwxrwx   0        0        0        0 2023-04-25 18:29:39.122893 netsuite_python-1.5.4/netsuite/storages/
--rw-rw-rw-   0        0        0      324 2023-02-12 19:28:31.000000 netsuite_python-1.5.4/netsuite/storages/BaseStorage.py
--rw-rw-rw-   0        0        0      653 2023-02-12 19:28:31.000000 netsuite_python-1.5.4/netsuite/storages/InMemoryStorage.py
--rw-rw-rw-   0        0        0     1594 2023-02-12 19:28:31.000000 netsuite_python-1.5.4/netsuite/storages/JSONStorage.py
--rw-rw-rw-   0        0        0      119 2023-02-12 19:28:31.000000 netsuite_python-1.5.4/netsuite/storages/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 18:29:39.127894 netsuite_python-1.5.4/netsuite_python.egg-info/
--rw-rw-rw-   0        0        0     5636 2023-04-25 18:29:39.000000 netsuite_python-1.5.4/netsuite_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      920 2023-04-25 18:29:39.000000 netsuite_python-1.5.4/netsuite_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 18:29:39.000000 netsuite_python-1.5.4/netsuite_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-04-25 18:29:39.000000 netsuite_python-1.5.4/netsuite_python.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       81 2023-04-25 18:29:39.000000 netsuite_python-1.5.4/netsuite_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-25 18:29:39.000000 netsuite_python-1.5.4/netsuite_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-25 18:29:39.129893 netsuite_python-1.5.4/setup.cfg
--rw-rw-rw-   0        0        0      961 2023-04-25 18:28:17.000000 netsuite_python-1.5.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 18:31:14.458414 netsuite_python-1.5.5/
+-rw-rw-rw-   0        0        0     5636 2023-04-25 18:31:14.458414 netsuite_python-1.5.5/PKG-INFO
+-rw-rw-rw-   0        0        0     5306 2023-04-25 18:29:11.000000 netsuite_python-1.5.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-25 18:31:14.440415 netsuite_python-1.5.5/netsuite/
+-rw-rw-rw-   0        0        0    12072 2023-04-25 18:30:40.000000 netsuite_python-1.5.5/netsuite/Netsuite.py
+-rw-rw-rw-   0        0        0      494 2023-02-12 19:28:31.000000 netsuite_python-1.5.5/netsuite/NetsuiteToken.py
+-rw-rw-rw-   0        0        0       74 2023-02-12 19:28:31.000000 netsuite_python-1.5.5/netsuite/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 18:31:14.443414 netsuite_python-1.5.5/netsuite/api_clients/
+-rw-rw-rw-   0        0        0      235 2023-04-09 19:43:22.000000 netsuite_python-1.5.5/netsuite/api_clients/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 18:31:14.446414 netsuite_python-1.5.5/netsuite/api_clients/api/
+-rw-rw-rw-   0        0        0       59 2023-04-09 19:48:25.000000 netsuite_python-1.5.5/netsuite/api_clients/api/__init__.py
+-rw-rw-rw-   0        0        0     5489 2023-04-09 19:49:23.000000 netsuite_python-1.5.5/netsuite/api_clients/api/query_api.py
+-rw-rw-rw-   0        0        0     2249 2023-04-09 19:48:25.000000 netsuite_python-1.5.5/netsuite/api_clients/api/restlet_api.py
+-rw-rw-rw-   0        0        0    25577 2023-04-09 19:51:26.000000 netsuite_python-1.5.5/netsuite/api_clients/api_client.py
+-rw-rw-rw-   0        0        0     8466 2023-03-23 15:55:18.000000 netsuite_python-1.5.5/netsuite/api_clients/configuration.py
+-rw-rw-rw-   0        0        0    13259 2023-04-06 18:39:08.000000 netsuite_python-1.5.5/netsuite/api_clients/rest.py
+-rw-rw-rw-   0        0        0      243 2023-02-12 19:28:31.000000 netsuite_python-1.5.5/netsuite/exceptions.py
+-rw-rw-rw-   0        0        0     3921 2023-02-12 19:28:31.000000 netsuite_python-1.5.5/netsuite/module_loading.py
+drwxrwxrwx   0        0        0        0 2023-04-25 18:31:14.448414 netsuite_python-1.5.5/netsuite/netsuite_rest_client/
+-rw-rw-rw-   0        0        0        0 2023-04-25 17:05:59.000000 netsuite_python-1.5.5/netsuite/netsuite_rest_client/__init__.py
+-rw-rw-rw-   0        0        0      463 2023-04-17 18:07:52.000000 netsuite_python-1.5.5/netsuite/netsuite_rest_client/rest_api_client.py
+drwxrwxrwx   0        0        0        0 2023-04-25 18:31:14.449418 netsuite_python-1.5.5/netsuite/scripts/
+-rw-rw-rw-   0        0        0        0 2023-02-12 19:28:31.000000 netsuite_python-1.5.5/netsuite/scripts/__init__.py
+-rw-rw-rw-   0        0        0    11109 2023-04-25 18:27:59.000000 netsuite_python-1.5.5/netsuite/scripts/cli.py
+-rw-rw-rw-   0        0        0     6300 2023-04-17 18:30:20.000000 netsuite_python-1.5.5/netsuite/settings.py
+drwxrwxrwx   0        0        0        0 2023-04-25 18:31:14.452415 netsuite_python-1.5.5/netsuite/storages/
+-rw-rw-rw-   0        0        0      324 2023-02-12 19:28:31.000000 netsuite_python-1.5.5/netsuite/storages/BaseStorage.py
+-rw-rw-rw-   0        0        0      653 2023-02-12 19:28:31.000000 netsuite_python-1.5.5/netsuite/storages/InMemoryStorage.py
+-rw-rw-rw-   0        0        0     1594 2023-02-12 19:28:31.000000 netsuite_python-1.5.5/netsuite/storages/JSONStorage.py
+-rw-rw-rw-   0        0        0      119 2023-02-12 19:28:31.000000 netsuite_python-1.5.5/netsuite/storages/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 18:31:14.457414 netsuite_python-1.5.5/netsuite_python.egg-info/
+-rw-rw-rw-   0        0        0     5636 2023-04-25 18:31:14.000000 netsuite_python-1.5.5/netsuite_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      920 2023-04-25 18:31:14.000000 netsuite_python-1.5.5/netsuite_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 18:31:14.000000 netsuite_python-1.5.5/netsuite_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-04-25 18:31:14.000000 netsuite_python-1.5.5/netsuite_python.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       81 2023-04-25 18:31:14.000000 netsuite_python-1.5.5/netsuite_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-25 18:31:14.000000 netsuite_python-1.5.5/netsuite_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-25 18:31:14.459414 netsuite_python-1.5.5/setup.cfg
+-rw-rw-rw-   0        0        0      961 2023-04-25 18:31:05.000000 netsuite_python-1.5.5/setup.py
```

### Comparing `netsuite_python-1.5.4/PKG-INFO` & `netsuite_python-1.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netsuite_python
-Version: 1.5.4
+Version: 1.5.5
 Summary: Python SDK for Netsuite API with Flask Integration
 Home-page: https://bitbucket.org/theapiguys/netsuite_python
 Author: Will @ TheAPIGuys
 Author-email: will@theapiguys.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `netsuite_python-1.5.4/README.md` & `netsuite_python-1.5.5/README.md`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.5.4/netsuite/Netsuite.py` & `netsuite_python-1.5.5/netsuite/Netsuite.py`

 * *Files 1% similar despite different names*

```diff
@@ -228,15 +228,15 @@
         shutil.copytree(docs_src, docs_dst, symlinks=True, ignore=None, ignore_dangling_symlinks=False,
                         dirs_exist_ok=True)
 
         shutil.copy(class_src, dst)
         shutil.copy(readme_src, dst)
 
 
-        # shutil.rmtree(Path.joinpath(Path(self.api_settings.NETSUITE_CLIENT_PATH), 'python-client'))
+        shutil.rmtree(Path.joinpath(Path(self.api_settings.NETSUITE_CLIENT_PATH), 'python-client'))
         print('temp folder was removed.')
 
         print('\nNetsuite client was successfully generated and is ready to use!')
         print('***************************************************************')
         print('\nUSAGE')
         print('----------------------')
         print('from netsuite import Netsuite'
```

### Comparing `netsuite_python-1.5.4/netsuite/api_clients/api/query_api.py` & `netsuite_python-1.5.5/netsuite/api_clients/api/query_api.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.5.4/netsuite/api_clients/api/restlet_api.py` & `netsuite_python-1.5.5/netsuite/api_clients/api/restlet_api.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.5.4/netsuite/api_clients/api_client.py` & `netsuite_python-1.5.5/netsuite/api_clients/api_client.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.5.4/netsuite/api_clients/configuration.py` & `netsuite_python-1.5.5/netsuite/api_clients/configuration.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.5.4/netsuite/api_clients/rest.py` & `netsuite_python-1.5.5/netsuite/api_clients/rest.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.5.4/netsuite/module_loading.py` & `netsuite_python-1.5.5/netsuite/module_loading.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.5.4/netsuite/scripts/cli.py` & `netsuite_python-1.5.5/netsuite/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.5.4/netsuite/settings.py` & `netsuite_python-1.5.5/netsuite/settings.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.5.4/netsuite/storages/InMemoryStorage.py` & `netsuite_python-1.5.5/netsuite/storages/InMemoryStorage.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.5.4/netsuite/storages/JSONStorage.py` & `netsuite_python-1.5.5/netsuite/storages/JSONStorage.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.5.4/netsuite_python.egg-info/PKG-INFO` & `netsuite_python-1.5.5/netsuite_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netsuite-python
-Version: 1.5.4
+Version: 1.5.5
 Summary: Python SDK for Netsuite API with Flask Integration
 Home-page: https://bitbucket.org/theapiguys/netsuite_python
 Author: Will @ TheAPIGuys
 Author-email: will@theapiguys.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `netsuite_python-1.5.4/netsuite_python.egg-info/SOURCES.txt` & `netsuite_python-1.5.5/netsuite_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.5.4/setup.py` & `netsuite_python-1.5.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='netsuite_python',
-    version='1.5.4',
+    version='1.5.5',
     description='Python SDK for Netsuite API with Flask Integration',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://bitbucket.org/theapiguys/netsuite_python',
     readme="README.md",
     author='Will @ TheAPIGuys',
     author_email='will@theapiguys.com',
```

