# Comparing `tmp/mongoclass-1.4.tar.gz` & `tmp/mongoclass-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongoclass-1.4.tar", last modified: Thu Apr 20 07:44:18 2023, max compression
+gzip compressed data, was "mongoclass-1.5.tar", last modified: Wed Apr 26 02:21:11 2023, max compression
```

## Comparing `mongoclass-1.4.tar` & `mongoclass-1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 07:44:18.079955 mongoclass-1.4/
--rw-rw-rw-   0        0        0     1093 2022-10-28 01:48:28.000000 mongoclass-1.4/LICENSE
--rw-rw-rw-   0        0        0     3408 2023-04-20 07:44:18.080953 mongoclass-1.4/PKG-INFO
--rw-rw-rw-   0        0        0     2973 2022-10-28 01:48:28.000000 mongoclass-1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-20 07:44:18.045956 mongoclass-1.4/mongoclass/
--rw-rw-rw-   0        0        0       58 2022-10-28 01:48:28.000000 mongoclass-1.4/mongoclass/__init__.py
--rw-rw-rw-   0        0        0     5420 2023-04-18 14:44:13.000000 mongoclass-1.4/mongoclass/cache.py
--rw-rw-rw-   0        0        0    25900 2023-04-20 07:43:12.000000 mongoclass-1.4/mongoclass/client.py
--rw-rw-rw-   0        0        0     2015 2022-10-28 01:48:58.000000 mongoclass-1.4/mongoclass/cursor.py
-drwxrwxrwx   0        0        0        0 2023-04-20 07:44:18.078954 mongoclass-1.4/mongoclass.egg-info/
--rw-rw-rw-   0        0        0     3408 2023-04-20 07:44:17.000000 mongoclass-1.4/mongoclass.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      290 2023-04-20 07:44:17.000000 mongoclass-1.4/mongoclass.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 07:44:17.000000 mongoclass-1.4/mongoclass.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-04-20 07:44:17.000000 mongoclass-1.4/mongoclass.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-20 07:44:17.000000 mongoclass-1.4/mongoclass.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-04-20 07:44:18.082957 mongoclass-1.4/setup.cfg
--rw-rw-rw-   0        0        0      769 2023-04-20 07:43:42.000000 mongoclass-1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 02:21:11.818704 mongoclass-1.5/
+-rw-rw-rw-   0        0        0     1093 2022-10-28 01:48:28.000000 mongoclass-1.5/LICENSE
+-rw-rw-rw-   0        0        0     3408 2023-04-26 02:21:11.818704 mongoclass-1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2973 2022-10-28 01:48:28.000000 mongoclass-1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-26 02:21:11.786704 mongoclass-1.5/mongoclass/
+-rw-rw-rw-   0        0        0       58 2022-10-28 01:48:28.000000 mongoclass-1.5/mongoclass/__init__.py
+-rw-rw-rw-   0        0        0     5420 2023-04-18 14:44:13.000000 mongoclass-1.5/mongoclass/cache.py
+-rw-rw-rw-   0        0        0    25925 2023-04-26 02:19:59.000000 mongoclass-1.5/mongoclass/client.py
+-rw-rw-rw-   0        0        0     2015 2022-10-28 01:48:58.000000 mongoclass-1.5/mongoclass/cursor.py
+drwxrwxrwx   0        0        0        0 2023-04-26 02:21:11.816709 mongoclass-1.5/mongoclass.egg-info/
+-rw-rw-rw-   0        0        0     3408 2023-04-26 02:21:11.000000 mongoclass-1.5/mongoclass.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      290 2023-04-26 02:21:11.000000 mongoclass-1.5/mongoclass.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 02:21:11.000000 mongoclass-1.5/mongoclass.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-04-26 02:21:11.000000 mongoclass-1.5/mongoclass.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-26 02:21:11.000000 mongoclass-1.5/mongoclass.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-04-26 02:21:11.820703 mongoclass-1.5/setup.cfg
+-rw-rw-rw-   0        0        0      769 2023-04-26 02:20:39.000000 mongoclass-1.5/setup.py
```

### Comparing `mongoclass-1.4/LICENSE` & `mongoclass-1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mongoclass-1.4/PKG-INFO` & `mongoclass-1.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: mongoclass
-Version: 1.4
+Version: 1.5
 Summary: A basic ORM like interface for mongodb in python that uses dataclasses.
 Home-page: https://github.com/bossauh/mongoclass
-Download-URL: https://github.com/bossauh/mongoclass/archive/refs/tags/v_14.tar.gz
+Download-URL: https://github.com/bossauh/mongoclass/archive/refs/tags/v_15.tar.gz
 Author: Philippe Mathew
 Author-email: philmattdev@gmail.com
 License: MIT
 Keywords: pymongo,orm
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mongoclass-1.4/README.md` & `mongoclass-1.5/README.md`

 * *Files identical despite different names*

### Comparing `mongoclass-1.4/mongoclass/cache.py` & `mongoclass-1.5/mongoclass/cache.py`

 * *Files identical despite different names*

### Comparing `mongoclass-1.4/mongoclass/client.py` & `mongoclass-1.5/mongoclass/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,15 +106,15 @@
                                 v["data"],
                                 v["_nest_collection"],
                                 v["_nest_database"],
                                 force_nested=True,
                             )
                     elif isinstance(v, list):
                         for i, li in enumerate(v):
-                            if "_nest_collection" in li:
+                            if isinstance(li, dict) and "_nest_collection" in li:
                                 data[k][i] = self.map_document(
                                     li["data"],
                                     li["_nest_collection"],
                                     li["_nest_database"],
                                     force_nested=True,
                                 )
```

### Comparing `mongoclass-1.4/mongoclass/cursor.py` & `mongoclass-1.5/mongoclass/cursor.py`

 * *Files identical despite different names*

### Comparing `mongoclass-1.4/mongoclass.egg-info/PKG-INFO` & `mongoclass-1.5/mongoclass.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: mongoclass
-Version: 1.4
+Version: 1.5
 Summary: A basic ORM like interface for mongodb in python that uses dataclasses.
 Home-page: https://github.com/bossauh/mongoclass
-Download-URL: https://github.com/bossauh/mongoclass/archive/refs/tags/v_14.tar.gz
+Download-URL: https://github.com/bossauh/mongoclass/archive/refs/tags/v_15.tar.gz
 Author: Philippe Mathew
 Author-email: philmattdev@gmail.com
 License: MIT
 Keywords: pymongo,orm
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mongoclass-1.4/setup.py` & `mongoclass-1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 
 install_requires = ["dnspython==2.2.1", "mongita==1.1.1"]
 long_description = (Path(__file__).parent / "README.md").read_text()
 
 setup(
     name="mongoclass",
     packages=["mongoclass"],
-    version="1.4",
+    version="1.5",
     license="MIT",
     description="A basic ORM like interface for mongodb in python that uses dataclasses.",
     author="Philippe Mathew",
     author_email="philmattdev@gmail.com",
     url="https://github.com/bossauh/mongoclass",
-    download_url="https://github.com/bossauh/mongoclass/archive/refs/tags/v_14.tar.gz",
+    download_url="https://github.com/bossauh/mongoclass/archive/refs/tags/v_15.tar.gz",
     keywords=["pymongo", "orm"],
     install_requires=install_requires,
     long_description=long_description,
     long_description_content_type="text/markdown",
 )
```

