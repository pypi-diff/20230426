# Comparing `tmp/notion-dashworks-fork-0.0.8.tar.gz` & `tmp/notion-dashworks-fork-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notion-dashworks-fork-0.0.8.tar", last modified: Tue Oct 18 21:59:16 2022, max compression
+gzip compressed data, was "notion-dashworks-fork-0.0.9.tar", last modified: Wed Oct 19 18:19:24 2022, max compression
```

## Comparing `notion-dashworks-fork-0.0.8.tar` & `notion-dashworks-fork-0.0.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 pavan      (501) staff       (20)        0 2022-10-18 21:59:16.490606 notion-dashworks-fork-0.0.8/
--rw-r--r--   0 pavan      (501) staff       (20)     1058 2022-07-18 03:30:04.000000 notion-dashworks-fork-0.0.8/LICENSE
--rw-r--r--   0 pavan      (501) staff       (20)      107 2022-07-18 03:30:04.000000 notion-dashworks-fork-0.0.8/MANIFEST.in
--rw-r--r--   0 pavan      (501) staff       (20)    14076 2022-10-18 21:59:16.490436 notion-dashworks-fork-0.0.8/PKG-INFO
--rw-r--r--   0 pavan      (501) staff       (20)    13544 2022-07-19 18:36:48.000000 notion-dashworks-fork-0.0.8/README.md
--rw-r--r--   0 pavan      (501) staff       (20)       73 2022-07-18 03:30:04.000000 notion-dashworks-fork-0.0.8/requirements.txt
--rw-r--r--   0 pavan      (501) staff       (20)       38 2022-10-18 21:59:16.490640 notion-dashworks-fork-0.0.8/setup.cfg
--rw-r--r--   0 pavan      (501) staff       (20)     1320 2022-10-18 21:58:41.000000 notion-dashworks-fork-0.0.8/setup.py
-drwxr-xr-x   0 pavan      (501) staff       (20)        0 2022-10-18 21:59:16.485962 notion-dashworks-fork-0.0.8/src/
-drwxr-xr-x   0 pavan      (501) staff       (20)        0 2022-10-18 21:59:16.489648 notion-dashworks-fork-0.0.8/src/notion/
--rw-r--r--   0 pavan      (501) staff       (20)        0 2022-07-18 03:30:04.000000 notion-dashworks-fork-0.0.8/src/notion/__init__.py
--rw-r--r--   0 pavan      (501) staff       (20)    25469 2022-10-18 21:58:19.000000 notion-dashworks-fork-0.0.8/src/notion/block.py
--rw-r--r--   0 pavan      (501) staff       (20)    17300 2022-10-18 21:58:19.000000 notion-dashworks-fork-0.0.8/src/notion/client.py
--rw-r--r--   0 pavan      (501) staff       (20)    25716 2022-07-20 03:04:23.000000 notion-dashworks-fork-0.0.8/src/notion/collection.py
--rw-r--r--   0 pavan      (501) staff       (20)     1107 2022-07-18 03:30:04.000000 notion-dashworks-fork-0.0.8/src/notion/logger.py
--rw-r--r--   0 pavan      (501) staff       (20)     3662 2022-10-18 21:58:19.000000 notion-dashworks-fork-0.0.8/src/notion/maps.py
--rw-r--r--   0 pavan      (501) staff       (20)     9350 2022-07-18 03:30:04.000000 notion-dashworks-fork-0.0.8/src/notion/markdown.py
--rw-r--r--   0 pavan      (501) staff       (20)     8126 2022-10-18 21:58:19.000000 notion-dashworks-fork-0.0.8/src/notion/monitor.py
--rw-r--r--   0 pavan      (501) staff       (20)      997 2022-07-18 03:30:04.000000 notion-dashworks-fork-0.0.8/src/notion/operations.py
--rw-r--r--   0 pavan      (501) staff       (20)        0 2022-10-18 21:58:19.000000 notion-dashworks-fork-0.0.8/src/notion/py.typed
--rw-r--r--   0 pavan      (501) staff       (20)     4698 2022-10-18 21:58:19.000000 notion-dashworks-fork-0.0.8/src/notion/records.py
--rw-r--r--   0 pavan      (501) staff       (20)      671 2022-07-18 03:30:04.000000 notion-dashworks-fork-0.0.8/src/notion/settings.py
--rw-r--r--   0 pavan      (501) staff       (20)     9398 2022-07-18 03:30:04.000000 notion-dashworks-fork-0.0.8/src/notion/smoke_test.py
--rw-r--r--   0 pavan      (501) staff       (20)     1595 2022-10-18 21:58:19.000000 notion-dashworks-fork-0.0.8/src/notion/space.py
--rw-r--r--   0 pavan      (501) staff       (20)    15646 2022-10-18 21:58:19.000000 notion-dashworks-fork-0.0.8/src/notion/store.py
--rw-r--r--   0 pavan      (501) staff       (20)      555 2022-10-18 21:58:19.000000 notion-dashworks-fork-0.0.8/src/notion/user.py
--rw-r--r--   0 pavan      (501) staff       (20)     2851 2022-07-18 03:30:04.000000 notion-dashworks-fork-0.0.8/src/notion/utils.py
-drwxr-xr-x   0 pavan      (501) staff       (20)        0 2022-10-18 21:59:16.490272 notion-dashworks-fork-0.0.8/src/notion_dashworks_fork.egg-info/
--rw-r--r--   0 pavan      (501) staff       (20)    14076 2022-10-18 21:59:16.000000 notion-dashworks-fork-0.0.8/src/notion_dashworks_fork.egg-info/PKG-INFO
--rw-r--r--   0 pavan      (501) staff       (20)      667 2022-10-18 21:59:16.000000 notion-dashworks-fork-0.0.8/src/notion_dashworks_fork.egg-info/SOURCES.txt
--rw-r--r--   0 pavan      (501) staff       (20)        1 2022-10-18 21:59:16.000000 notion-dashworks-fork-0.0.8/src/notion_dashworks_fork.egg-info/dependency_links.txt
--rw-r--r--   0 pavan      (501) staff       (20)       74 2022-10-18 21:59:16.000000 notion-dashworks-fork-0.0.8/src/notion_dashworks_fork.egg-info/requires.txt
--rw-r--r--   0 pavan      (501) staff       (20)        7 2022-10-18 21:59:16.000000 notion-dashworks-fork-0.0.8/src/notion_dashworks_fork.egg-info/top_level.txt
+drwxr-xr-x   0 sischick   (501) staff       (20)        0 2022-10-19 18:19:24.811951 notion-dashworks-fork-0.0.9/
+-rw-r--r--   0 sischick   (501) staff       (20)     1058 2022-10-17 20:53:48.000000 notion-dashworks-fork-0.0.9/LICENSE
+-rw-r--r--   0 sischick   (501) staff       (20)      107 2022-10-17 20:53:48.000000 notion-dashworks-fork-0.0.9/MANIFEST.in
+-rw-r--r--   0 sischick   (501) staff       (20)    14039 2022-10-19 18:19:24.811574 notion-dashworks-fork-0.0.9/PKG-INFO
+-rw-r--r--   0 sischick   (501) staff       (20)    13544 2022-10-17 20:53:48.000000 notion-dashworks-fork-0.0.9/README.md
+-rw-r--r--   0 sischick   (501) staff       (20)       73 2022-10-17 20:53:48.000000 notion-dashworks-fork-0.0.9/requirements.txt
+-rw-r--r--   0 sischick   (501) staff       (20)       38 2022-10-19 18:19:24.812047 notion-dashworks-fork-0.0.9/setup.cfg
+-rw-r--r--   0 sischick   (501) staff       (20)     1320 2022-10-19 18:18:48.000000 notion-dashworks-fork-0.0.9/setup.py
+drwxr-xr-x   0 sischick   (501) staff       (20)        0 2022-10-19 18:19:24.803603 notion-dashworks-fork-0.0.9/src/
+drwxr-xr-x   0 sischick   (501) staff       (20)        0 2022-10-19 18:19:24.809745 notion-dashworks-fork-0.0.9/src/notion/
+-rw-r--r--   0 sischick   (501) staff       (20)        0 2022-10-17 20:53:48.000000 notion-dashworks-fork-0.0.9/src/notion/__init__.py
+-rw-r--r--   0 sischick   (501) staff       (20)    25476 2022-10-19 18:18:41.000000 notion-dashworks-fork-0.0.9/src/notion/block.py
+-rw-r--r--   0 sischick   (501) staff       (20)    17300 2022-10-19 18:18:39.000000 notion-dashworks-fork-0.0.9/src/notion/client.py
+-rw-r--r--   0 sischick   (501) staff       (20)    25716 2022-10-17 20:53:48.000000 notion-dashworks-fork-0.0.9/src/notion/collection.py
+-rw-r--r--   0 sischick   (501) staff       (20)     1107 2022-10-17 20:53:48.000000 notion-dashworks-fork-0.0.9/src/notion/logger.py
+-rw-r--r--   0 sischick   (501) staff       (20)     3662 2022-10-19 18:18:39.000000 notion-dashworks-fork-0.0.9/src/notion/maps.py
+-rw-r--r--   0 sischick   (501) staff       (20)     9350 2022-10-17 20:53:48.000000 notion-dashworks-fork-0.0.9/src/notion/markdown.py
+-rw-r--r--   0 sischick   (501) staff       (20)     8126 2022-10-19 18:18:39.000000 notion-dashworks-fork-0.0.9/src/notion/monitor.py
+-rw-r--r--   0 sischick   (501) staff       (20)      997 2022-10-17 20:53:48.000000 notion-dashworks-fork-0.0.9/src/notion/operations.py
+-rw-r--r--   0 sischick   (501) staff       (20)        0 2022-10-19 18:18:39.000000 notion-dashworks-fork-0.0.9/src/notion/py.typed
+-rw-r--r--   0 sischick   (501) staff       (20)     4725 2022-10-19 18:18:41.000000 notion-dashworks-fork-0.0.9/src/notion/records.py
+-rw-r--r--   0 sischick   (501) staff       (20)      671 2022-10-17 20:53:48.000000 notion-dashworks-fork-0.0.9/src/notion/settings.py
+-rw-r--r--   0 sischick   (501) staff       (20)     9398 2022-10-17 20:53:48.000000 notion-dashworks-fork-0.0.9/src/notion/smoke_test.py
+-rw-r--r--   0 sischick   (501) staff       (20)     1595 2022-10-19 18:18:39.000000 notion-dashworks-fork-0.0.9/src/notion/space.py
+-rw-r--r--   0 sischick   (501) staff       (20)    15646 2022-10-19 18:18:39.000000 notion-dashworks-fork-0.0.9/src/notion/store.py
+-rw-r--r--   0 sischick   (501) staff       (20)      555 2022-10-19 18:18:39.000000 notion-dashworks-fork-0.0.9/src/notion/user.py
+-rw-r--r--   0 sischick   (501) staff       (20)     2851 2022-10-17 20:53:48.000000 notion-dashworks-fork-0.0.9/src/notion/utils.py
+drwxr-xr-x   0 sischick   (501) staff       (20)        0 2022-10-19 18:19:24.811096 notion-dashworks-fork-0.0.9/src/notion_dashworks_fork.egg-info/
+-rw-r--r--   0 sischick   (501) staff       (20)    14039 2022-10-19 18:19:24.000000 notion-dashworks-fork-0.0.9/src/notion_dashworks_fork.egg-info/PKG-INFO
+-rw-r--r--   0 sischick   (501) staff       (20)      667 2022-10-19 18:19:24.000000 notion-dashworks-fork-0.0.9/src/notion_dashworks_fork.egg-info/SOURCES.txt
+-rw-r--r--   0 sischick   (501) staff       (20)        1 2022-10-19 18:19:24.000000 notion-dashworks-fork-0.0.9/src/notion_dashworks_fork.egg-info/dependency_links.txt
+-rw-r--r--   0 sischick   (501) staff       (20)       74 2022-10-19 18:19:24.000000 notion-dashworks-fork-0.0.9/src/notion_dashworks_fork.egg-info/requires.txt
+-rw-r--r--   0 sischick   (501) staff       (20)        7 2022-10-19 18:19:24.000000 notion-dashworks-fork-0.0.9/src/notion_dashworks_fork.egg-info/top_level.txt
```

### Comparing `notion-dashworks-fork-0.0.8/LICENSE` & `notion-dashworks-fork-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `notion-dashworks-fork-0.0.8/PKG-INFO` & `notion-dashworks-fork-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: notion-dashworks-fork
-Version: 0.0.8
+Version: 0.0.9
 Summary: Unofficial Python API client for Notion.so forked for dashworks
 Home-page: https://github.com/dashworkstech/notion-dashworks
 Author: Developers Dashworks
 Author-email: support@dashworks.ai
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -285,9 +283,7 @@
 - "Import page from html" mode
 
 # Deployment
 
 - Update the version number in `setup.py`
 - `python setup.py sdist`
 - `twine upload dist/*`
-
-
```

### Comparing `notion-dashworks-fork-0.0.8/README.md` & `notion-dashworks-fork-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `notion-dashworks-fork-0.0.8/setup.py` & `notion-dashworks-fork-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         return reqs
 
 
 install_requires = get_requirements("requirements.txt")
 
 setuptools.setup(
     name="notion-dashworks-fork",
-    version="0.0.8",
+    version="0.0.9",
     author="Developers Dashworks",
     author_email="support@dashworks.ai",
     description="Unofficial Python API client for Notion.so forked for dashworks",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dashworkstech/notion-dashworks",
     install_requires=install_requires,
```

### Comparing `notion-dashworks-fork-0.0.8/src/notion/block.py` & `notion-dashworks-fork-0.0.9/src/notion/block.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,15 +178,15 @@
     _alias_parent = None
 
     child_list_key = "content"
 
     type = field_map("type")
     alive = field_map("alive")
 
-    def get_browseable_url(self):
+    def get_browseable_url(self) -> str:
         if "page" in self._type:
             return BASE_URL + self.id.replace("-", "")
         else:
             return self.parent.get_browseable_url() + "#" + self.id.replace("-", "")
 
     @property
     def children(self) -> List[Record]:
```

### Comparing `notion-dashworks-fork-0.0.8/src/notion/client.py` & `notion-dashworks-fork-0.0.9/src/notion/client.py`

 * *Files identical despite different names*

### Comparing `notion-dashworks-fork-0.0.8/src/notion/collection.py` & `notion-dashworks-fork-0.0.9/src/notion/collection.py`

 * *Files identical despite different names*

### Comparing `notion-dashworks-fork-0.0.8/src/notion/logger.py` & `notion-dashworks-fork-0.0.9/src/notion/logger.py`

 * *Files identical despite different names*

### Comparing `notion-dashworks-fork-0.0.8/src/notion/maps.py` & `notion-dashworks-fork-0.0.9/src/notion/maps.py`

 * *Files identical despite different names*

### Comparing `notion-dashworks-fork-0.0.8/src/notion/markdown.py` & `notion-dashworks-fork-0.0.9/src/notion/markdown.py`

 * *Files identical despite different names*

### Comparing `notion-dashworks-fork-0.0.8/src/notion/monitor.py` & `notion-dashworks-fork-0.0.9/src/notion/monitor.py`

 * *Files identical despite different names*

### Comparing `notion-dashworks-fork-0.0.8/src/notion/operations.py` & `notion-dashworks-fork-0.0.9/src/notion/operations.py`

 * *Files identical despite different names*

### Comparing `notion-dashworks-fork-0.0.8/src/notion/records.py` & `notion-dashworks-fork-0.0.9/src/notion/records.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from copy import deepcopy
-from typing import Any, List, Optional
+from typing import Any, List, Optional, Union
 
 from .operations import build_operation
 from .utils import extract_id, get_by_path
 
 
 class Record(object):
 
@@ -39,15 +39,15 @@
                 if getattr(self, field, "")
             ]
         )
 
     def __repr__(self):
         return "<{} ({})>".format(self.__class__.__name__, self)
 
-    def refresh(self):
+    def refresh(self) -> None:
         """
         Update the cached data for this record from the server (data for other records may be updated as a side effect).
         """
         self._get_record_data(force_refresh=True)
 
     def _convert_diff_to_changelist(self, difference, old_val, new_val):
         changed_values = set()
@@ -100,15 +100,15 @@
 
     def data(self):
         """
         Return the data structure for this record.
         """
         return self._get_record_data(force_refresh=True)
 
-    def get(self, path:List[str]=[], default:Optional[Any]=None, force_refresh:bool=False) -> Optional[Any]:
+    def get(self, path:Union[str, List[str]]=[], default:Optional[Any]=None, force_refresh:bool=False) -> Optional[Any]:
         """
         Retrieve cached data for this record. The `path` is a list (or dot-delimited string) the specifies the field
         to retrieve the value for. If no path is supplied, return the entire cached data structure for this record.
         If `force_refresh` is set to True, we force_refresh the data cache from the server before reading the values.
         """
         return get_by_path(
             path, self._get_record_data(force_refresh=force_refresh), default=default
```

### Comparing `notion-dashworks-fork-0.0.8/src/notion/settings.py` & `notion-dashworks-fork-0.0.9/src/notion/settings.py`

 * *Files identical despite different names*

### Comparing `notion-dashworks-fork-0.0.8/src/notion/smoke_test.py` & `notion-dashworks-fork-0.0.9/src/notion/smoke_test.py`

 * *Files identical despite different names*

### Comparing `notion-dashworks-fork-0.0.8/src/notion/space.py` & `notion-dashworks-fork-0.0.9/src/notion/space.py`

 * *Files identical despite different names*

### Comparing `notion-dashworks-fork-0.0.8/src/notion/store.py` & `notion-dashworks-fork-0.0.9/src/notion/store.py`

 * *Files identical despite different names*

### Comparing `notion-dashworks-fork-0.0.8/src/notion/user.py` & `notion-dashworks-fork-0.0.9/src/notion/user.py`

 * *Files identical despite different names*

### Comparing `notion-dashworks-fork-0.0.8/src/notion/utils.py` & `notion-dashworks-fork-0.0.9/src/notion/utils.py`

 * *Files identical despite different names*

### Comparing `notion-dashworks-fork-0.0.8/src/notion_dashworks_fork.egg-info/PKG-INFO` & `notion-dashworks-fork-0.0.9/src/notion_dashworks_fork.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: notion-dashworks-fork
-Version: 0.0.8
+Version: 0.0.9
 Summary: Unofficial Python API client for Notion.so forked for dashworks
 Home-page: https://github.com/dashworkstech/notion-dashworks
 Author: Developers Dashworks
 Author-email: support@dashworks.ai
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -285,9 +283,7 @@
 - "Import page from html" mode
 
 # Deployment
 
 - Update the version number in `setup.py`
 - `python setup.py sdist`
 - `twine upload dist/*`
-
-
```

### Comparing `notion-dashworks-fork-0.0.8/src/notion_dashworks_fork.egg-info/SOURCES.txt` & `notion-dashworks-fork-0.0.9/src/notion_dashworks_fork.egg-info/SOURCES.txt`

 * *Files identical despite different names*

