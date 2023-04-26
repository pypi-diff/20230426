# Comparing `tmp/xarray_map-0.0.1.tar.gz` & `tmp/xarray_map-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xarray_map-0.0.1.tar", last modified: Wed Apr 26 14:45:35 2023, max compression
+gzip compressed data, was "xarray_map-0.0.2.tar", last modified: Wed Apr 26 14:47:46 2023, max compression
```

## Comparing `xarray_map-0.0.1.tar` & `xarray_map-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-04-26 14:45:35.658983 xarray_map-0.0.1/
--rw-r--r--   0 javier     (501) staff       (20)      929 2023-04-26 14:45:35.659077 xarray_map-0.0.1/PKG-INFO
--rw-r--r--   0 javier     (501) staff       (20)     1056 2023-04-26 14:45:35.665060 xarray_map-0.0.1/setup.cfg
--rw-r--r--   0 javier     (501) staff       (20)      102 2023-04-26 13:39:17.000000 xarray_map-0.0.1/setup.py
-drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-04-26 14:45:35.649118 xarray_map-0.0.1/xarray-map/
--rw-r--r--   0 javier     (501) staff       (20)      112 2023-04-26 13:19:23.000000 xarray_map-0.0.1/xarray-map/__init__.py
-drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-04-26 14:45:35.649513 xarray_map-0.0.1/xarray-map/kmz/
--rw-r--r--   0 javier     (501) staff       (20)        0 2023-04-26 11:34:33.000000 xarray_map-0.0.1/xarray-map/kmz/__init__.py
--rw-r--r--   0 javier     (501) staff       (20)     1306 2023-04-26 13:46:32.000000 xarray_map-0.0.1/xarray-map/plot_folium.py
-drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-04-26 14:45:35.658703 xarray_map-0.0.1/xarray_map.egg-info/
--rw-r--r--   0 javier     (501) staff       (20)      929 2023-04-26 14:45:35.000000 xarray_map-0.0.1/xarray_map.egg-info/PKG-INFO
--rw-r--r--   0 javier     (501) staff       (20)      296 2023-04-26 14:45:35.000000 xarray_map-0.0.1/xarray_map.egg-info/SOURCES.txt
--rw-r--r--   0 javier     (501) staff       (20)        1 2023-04-26 14:45:35.000000 xarray_map-0.0.1/xarray_map.egg-info/dependency_links.txt
--rw-r--r--   0 javier     (501) staff       (20)        1 2023-04-26 13:39:56.000000 xarray_map-0.0.1/xarray_map.egg-info/not-zip-safe
--rw-r--r--   0 javier     (501) staff       (20)       31 2023-04-26 14:45:35.000000 xarray_map-0.0.1/xarray_map.egg-info/requires.txt
--rw-r--r--   0 javier     (501) staff       (20)       11 2023-04-26 14:45:35.000000 xarray_map-0.0.1/xarray_map.egg-info/top_level.txt
+drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-04-26 14:47:46.532532 xarray_map-0.0.2/
+-rw-r--r--   0 javier     (501) staff       (20)      929 2023-04-26 14:47:46.532600 xarray_map-0.0.2/PKG-INFO
+-rw-r--r--   0 javier     (501) staff       (20)     1056 2023-04-26 14:47:46.533724 xarray_map-0.0.2/setup.cfg
+-rw-r--r--   0 javier     (501) staff       (20)      102 2023-04-26 13:39:17.000000 xarray_map-0.0.2/setup.py
+drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-04-26 14:47:46.528086 xarray_map-0.0.2/xarray-map/
+-rw-r--r--   0 javier     (501) staff       (20)      112 2023-04-26 13:19:23.000000 xarray_map-0.0.2/xarray-map/__init__.py
+drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-04-26 14:47:46.528493 xarray_map-0.0.2/xarray-map/kmz/
+-rw-r--r--   0 javier     (501) staff       (20)        0 2023-04-26 11:34:33.000000 xarray_map-0.0.2/xarray-map/kmz/__init__.py
+-rw-r--r--   0 javier     (501) staff       (20)     1306 2023-04-26 13:46:32.000000 xarray_map-0.0.2/xarray-map/plot_folium.py
+drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-04-26 14:47:46.532425 xarray_map-0.0.2/xarray_map.egg-info/
+-rw-r--r--   0 javier     (501) staff       (20)      929 2023-04-26 14:47:46.000000 xarray_map-0.0.2/xarray_map.egg-info/PKG-INFO
+-rw-r--r--   0 javier     (501) staff       (20)      296 2023-04-26 14:47:46.000000 xarray_map-0.0.2/xarray_map.egg-info/SOURCES.txt
+-rw-r--r--   0 javier     (501) staff       (20)        1 2023-04-26 14:47:46.000000 xarray_map-0.0.2/xarray_map.egg-info/dependency_links.txt
+-rw-r--r--   0 javier     (501) staff       (20)        1 2023-04-26 13:39:56.000000 xarray_map-0.0.2/xarray_map.egg-info/not-zip-safe
+-rw-r--r--   0 javier     (501) staff       (20)       31 2023-04-26 14:47:46.000000 xarray_map-0.0.2/xarray_map.egg-info/requires.txt
+-rw-r--r--   0 javier     (501) staff       (20)       11 2023-04-26 14:47:46.000000 xarray_map-0.0.2/xarray_map.egg-info/top_level.txt
```

### Comparing `xarray_map-0.0.1/PKG-INFO` & `xarray_map-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xarray_map
-Version: 0.0.1
+Version: 0.0.2
 Summary: Plot xarrays lat-lon datasets using folium
 Home-page: https://github.com/pydata/xarray
 Author: Javier García-Valdecasas
 Author-email: garciavaldecasas@oritiayboreas.com
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,12 +14,12 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.9
+Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 
 Plot xarrays lat-lon datasets using folium
```

### Comparing `xarray_map-0.0.1/setup.cfg` & `xarray_map-0.0.2/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = xarray_map
-version = 0.0.1
+version = 0.0.2
 author = Javier García-Valdecasas
 author_email = garciavaldecasas@oritiayboreas.com
 license = Apache-2.0
 description = Plot xarrays lat-lon datasets using folium
 long_description_content_type = text/x-rst
 long_description = Plot xarrays lat-lon datasets using folium
 url = https://github.com/pydata/xarray
@@ -21,15 +21,15 @@
 	Programming Language :: Python :: 3.11
 	Topic :: Scientific/Engineering
 
 [options]
 packages = find:
 zip_safe = False  # https://mypy.readthedocs.io/en/latest/installed_packages.html
 include_package_data = True
-python_requires = >=3.9
+python_requires = >=3.6
 install_requires = 
 	xarray >= 0.21
 	folium
 	matplotlib
 
 [egg_info]
 tag_build =
```

### Comparing `xarray_map-0.0.1/xarray-map/plot_folium.py` & `xarray_map-0.0.2/xarray-map/plot_folium.py`

 * *Files identical despite different names*

### Comparing `xarray_map-0.0.1/xarray_map.egg-info/PKG-INFO` & `xarray_map-0.0.2/xarray_map.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xarray-map
-Version: 0.0.1
+Version: 0.0.2
 Summary: Plot xarrays lat-lon datasets using folium
 Home-page: https://github.com/pydata/xarray
 Author: Javier García-Valdecasas
 Author-email: garciavaldecasas@oritiayboreas.com
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,12 +14,12 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.9
+Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 
 Plot xarrays lat-lon datasets using folium
```

