# Comparing `tmp/ztffields-0.3.4.tar.gz` & `tmp/ztffields-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ztffields-0.3.4.tar", last modified: Wed Apr 26 12:49:22 2023, max compression
+gzip compressed data, was "ztffields-0.4.0.tar", last modified: Wed Apr 26 14:03:14 2023, max compression
```

## Comparing `ztffields-0.3.4.tar` & `ztffields-0.4.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-04-26 12:49:22.530425 ztffields-0.3.4/
--rw-r--r--   0 rigault   (2358) staff       (20)    11357 2022-12-09 18:53:25.000000 ztffields-0.3.4/LICENSE
--rw-r--r--   0 rigault   (2358) staff       (20)      731 2023-04-26 12:49:22.530484 ztffields-0.3.4/PKG-INFO
--rw-r--r--   0 rigault   (2358) staff       (20)      432 2022-12-13 14:52:32.000000 ztffields-0.3.4/README.md
--rw-r--r--   0 rigault   (2358) staff       (20)     1132 2023-04-26 12:49:22.530776 ztffields-0.3.4/setup.cfg
--rw-r--r--   0 rigault   (2358) staff       (20)       37 2022-12-11 14:43:45.000000 ztffields-0.3.4/setup.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-04-26 12:49:22.529317 ztffields-0.3.4/ztffields/
--rw-r--r--   0 rigault   (2358) staff       (20)       95 2023-04-26 12:48:59.000000 ztffields-0.3.4/ztffields/__init__.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-04-26 12:49:22.530266 ztffields-0.3.4/ztffields/data/
--rwxr-xr-x   0 rigault   (2358) staff       (20)     1419 2022-12-11 14:44:47.000000 ztffields-0.3.4/ztffields/data/ztf_ccd_layout.tbl
--rwxr-xr-x   0 rigault   (2358) staff       (20)     6230 2022-12-11 14:44:47.000000 ztffields-0.3.4/ztffields/data/ztf_ccd_quad_layout.tbl
--rwxr-xr-x   0 rigault   (2358) staff       (20)   123430 2022-12-11 14:44:47.000000 ztffields-0.3.4/ztffields/data/ztf_fields.txt
--rw-r--r--   0 rigault   (2358) staff       (20)    19743 2023-04-25 14:27:27.000000 ztffields-0.3.4/ztffields/fields.py
--rw-r--r--   0 rigault   (2358) staff       (20)      175 2022-12-11 14:47:26.000000 ztffields-0.3.4/ztffields/io.py
--rw-r--r--   0 rigault   (2358) staff       (20)    28795 2023-04-26 12:48:29.000000 ztffields-0.3.4/ztffields/plotting.py
--rw-r--r--   0 rigault   (2358) staff       (20)    12067 2023-04-19 13:38:56.000000 ztffields-0.3.4/ztffields/projection.py
--rw-r--r--   0 rigault   (2358) staff       (20)     2268 2023-02-12 07:53:02.000000 ztffields-0.3.4/ztffields/utils.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-04-26 12:49:22.529951 ztffields-0.3.4/ztffields.egg-info/
--rw-r--r--   0 rigault   (2358) staff       (20)      731 2023-04-26 12:49:22.000000 ztffields-0.3.4/ztffields.egg-info/PKG-INFO
--rw-r--r--   0 rigault   (2358) staff       (20)      458 2023-04-26 12:49:22.000000 ztffields-0.3.4/ztffields.egg-info/SOURCES.txt
--rw-r--r--   0 rigault   (2358) staff       (20)        1 2023-04-26 12:49:22.000000 ztffields-0.3.4/ztffields.egg-info/dependency_links.txt
--rw-r--r--   0 rigault   (2358) staff       (20)        1 2022-12-11 14:44:59.000000 ztffields-0.3.4/ztffields.egg-info/not-zip-safe
--rw-r--r--   0 rigault   (2358) staff       (20)      132 2023-04-26 12:49:22.000000 ztffields-0.3.4/ztffields.egg-info/requires.txt
--rw-r--r--   0 rigault   (2358) staff       (20)       10 2023-04-26 12:49:22.000000 ztffields-0.3.4/ztffields.egg-info/top_level.txt
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-04-26 14:03:14.766876 ztffields-0.4.0/
+-rw-r--r--   0 rigault   (2358) staff       (20)    11357 2022-12-09 18:53:25.000000 ztffields-0.4.0/LICENSE
+-rw-r--r--   0 rigault   (2358) staff       (20)      731 2023-04-26 14:03:14.766953 ztffields-0.4.0/PKG-INFO
+-rw-r--r--   0 rigault   (2358) staff       (20)      432 2022-12-13 14:52:32.000000 ztffields-0.4.0/README.md
+-rw-r--r--   0 rigault   (2358) staff       (20)     1132 2023-04-26 14:03:14.767279 ztffields-0.4.0/setup.cfg
+-rw-r--r--   0 rigault   (2358) staff       (20)       37 2022-12-11 14:43:45.000000 ztffields-0.4.0/setup.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-04-26 14:03:14.765723 ztffields-0.4.0/ztffields/
+-rw-r--r--   0 rigault   (2358) staff       (20)       95 2023-04-26 14:02:47.000000 ztffields-0.4.0/ztffields/__init__.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-04-26 14:03:14.766698 ztffields-0.4.0/ztffields/data/
+-rwxr-xr-x   0 rigault   (2358) staff       (20)     1419 2022-12-11 14:44:47.000000 ztffields-0.4.0/ztffields/data/ztf_ccd_layout.tbl
+-rwxr-xr-x   0 rigault   (2358) staff       (20)     6230 2022-12-11 14:44:47.000000 ztffields-0.4.0/ztffields/data/ztf_ccd_quad_layout.tbl
+-rwxr-xr-x   0 rigault   (2358) staff       (20)   123430 2022-12-11 14:44:47.000000 ztffields-0.4.0/ztffields/data/ztf_fields.txt
+-rw-r--r--   0 rigault   (2358) staff       (20)    19743 2023-04-25 14:27:27.000000 ztffields-0.4.0/ztffields/fields.py
+-rw-r--r--   0 rigault   (2358) staff       (20)      175 2022-12-11 14:47:26.000000 ztffields-0.4.0/ztffields/io.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    28795 2023-04-26 14:00:48.000000 ztffields-0.4.0/ztffields/plotting.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    12067 2023-04-19 13:38:56.000000 ztffields-0.4.0/ztffields/projection.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     2268 2023-02-12 07:53:02.000000 ztffields-0.4.0/ztffields/utils.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-04-26 14:03:14.766369 ztffields-0.4.0/ztffields.egg-info/
+-rw-r--r--   0 rigault   (2358) staff       (20)      731 2023-04-26 14:03:14.000000 ztffields-0.4.0/ztffields.egg-info/PKG-INFO
+-rw-r--r--   0 rigault   (2358) staff       (20)      458 2023-04-26 14:03:14.000000 ztffields-0.4.0/ztffields.egg-info/SOURCES.txt
+-rw-r--r--   0 rigault   (2358) staff       (20)        1 2023-04-26 14:03:14.000000 ztffields-0.4.0/ztffields.egg-info/dependency_links.txt
+-rw-r--r--   0 rigault   (2358) staff       (20)        1 2022-12-11 14:44:59.000000 ztffields-0.4.0/ztffields.egg-info/not-zip-safe
+-rw-r--r--   0 rigault   (2358) staff       (20)      132 2023-04-26 14:03:14.000000 ztffields-0.4.0/ztffields.egg-info/requires.txt
+-rw-r--r--   0 rigault   (2358) staff       (20)       10 2023-04-26 14:03:14.000000 ztffields-0.4.0/ztffields.egg-info/top_level.txt
```

### Comparing `ztffields-0.3.4/LICENSE` & `ztffields-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ztffields-0.3.4/PKG-INFO` & `ztffields-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ztffields
-Version: 0.3.4
+Version: 0.4.0
 Summary: Access and Interact with ZTF Fields
 Home-page: https://github.com/MickaelRigault/ztffields
 Author: Mickael Rigault
 Author-email: m.rigault@ipnl.in2p3.fr
 License: BSD 3-Clause "New" or "Revised" License
 Keywords: astronomy,astrophysics
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `ztffields-0.3.4/setup.cfg` & `ztffields-0.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `ztffields-0.3.4/ztffields/data/ztf_ccd_layout.tbl` & `ztffields-0.4.0/ztffields/data/ztf_ccd_layout.tbl`

 * *Files identical despite different names*

### Comparing `ztffields-0.3.4/ztffields/data/ztf_ccd_quad_layout.tbl` & `ztffields-0.4.0/ztffields/data/ztf_ccd_quad_layout.tbl`

 * *Files identical despite different names*

### Comparing `ztffields-0.3.4/ztffields/data/ztf_fields.txt` & `ztffields-0.4.0/ztffields/data/ztf_fields.txt`

 * *Files identical despite different names*

### Comparing `ztffields-0.3.4/ztffields/fields.py` & `ztffields-0.4.0/ztffields/fields.py`

 * *Files identical despite different names*

### Comparing `ztffields-0.3.4/ztffields/plotting.py` & `ztffields-0.4.0/ztffields/plotting.py`

 * *Files 1% similar despite different names*

```diff
@@ -650,15 +650,15 @@
             cax, histax = cax
         else:
             bboxax = self.ax.get_position()
             cax = self.ax.figure.add_axes([bboxax.xmin, ymin, bboxax.width, height*(1-(hratio+gapratio))])
             histax = self.ax.figure.add_axes([bboxax.xmin, ymin+height*(1-hratio), bboxax.width, 
                                          height*hratio])
 
-        if self._plotting["bins"] is None:
+        if "vrange" not in self._plotting:
             cax.set_visible(False)
             histax.set_visible(False)
             return None, None
     
         cax.set_visible(True) # just to make sure
         histax.set_visible(True) # just to make sure
```

### Comparing `ztffields-0.3.4/ztffields/projection.py` & `ztffields-0.4.0/ztffields/projection.py`

 * *Files identical despite different names*

### Comparing `ztffields-0.3.4/ztffields/utils.py` & `ztffields-0.4.0/ztffields/utils.py`

 * *Files identical despite different names*

### Comparing `ztffields-0.3.4/ztffields.egg-info/PKG-INFO` & `ztffields-0.4.0/ztffields.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ztffields
-Version: 0.3.4
+Version: 0.4.0
 Summary: Access and Interact with ZTF Fields
 Home-page: https://github.com/MickaelRigault/ztffields
 Author: Mickael Rigault
 Author-email: m.rigault@ipnl.in2p3.fr
 License: BSD 3-Clause "New" or "Revised" License
 Keywords: astronomy,astrophysics
 Classifier: Development Status :: 2 - Pre-Alpha
```

