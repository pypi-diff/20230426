# Comparing `tmp/aio_overpass-0.1.0.tar.gz` & `tmp/aio_overpass-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aio_overpass-0.1.0.tar", max compression
+gzip compressed data, was "aio_overpass-0.1.1.tar", max compression
```

## Comparing `aio_overpass-0.1.0.tar` & `aio_overpass-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1069 2023-01-07 23:46:48.048295 aio_overpass-0.1.0/LICENSE
--rw-r--r--   0        0        0     7428 2023-04-23 23:35:43.508933 aio_overpass-0.1.0/README.md
--rwxr-xr-x   0        0        0      316 2023-04-22 19:11:12.083982 aio_overpass-0.1.0/aio_overpass/__init__.py
--rw-r--r--   0        0        0      977 2023-04-20 23:16:58.247002 aio_overpass-0.1.0/aio_overpass/_dist.py
--rwxr-xr-x   0        0        0      971 2023-04-20 23:16:58.244337 aio_overpass-0.1.0/aio_overpass/_ql.py
--rwxr-xr-x   0        0        0    10947 2023-04-24 00:29:51.714956 aio_overpass-0.1.0/aio_overpass/client.py
--rwxr-xr-x   0        0        0    27979 2023-04-24 00:29:51.792641 aio_overpass-0.1.0/aio_overpass/element.py
--rwxr-xr-x   0        0        0    13665 2023-04-23 00:09:18.209185 aio_overpass-0.1.0/aio_overpass/error.py
--rwxr-xr-x   0        0        0    24559 2023-04-24 00:29:51.788456 aio_overpass-0.1.0/aio_overpass/pt.py
--rwxr-xr-x   0        0        0    22325 2023-04-24 00:29:51.805752 aio_overpass-0.1.0/aio_overpass/pt_ordered.py
--rwxr-xr-x   0        0        0    14338 2023-04-24 00:29:51.735571 aio_overpass-0.1.0/aio_overpass/query.py
--rwxr-xr-x   0        0        0     2140 2023-04-23 23:20:18.815106 aio_overpass-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     8744 1970-01-01 00:00:00.000000 aio_overpass-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-01-07 23:46:48.048295 aio_overpass-0.1.1/LICENSE
+-rw-r--r--   0        0        0     7949 2023-04-25 17:48:06.992954 aio_overpass-0.1.1/README.md
+-rwxr-xr-x   0        0        0      316 2023-04-25 17:54:12.413446 aio_overpass-0.1.1/aio_overpass/__init__.py
+-rw-r--r--   0        0        0      977 2023-04-20 23:16:58.247002 aio_overpass-0.1.1/aio_overpass/_dist.py
+-rwxr-xr-x   0        0        0      971 2023-04-20 23:16:58.244337 aio_overpass-0.1.1/aio_overpass/_ql.py
+-rwxr-xr-x   0        0        0    10947 2023-04-25 17:41:10.527121 aio_overpass-0.1.1/aio_overpass/client.py
+-rwxr-xr-x   0        0        0    28053 2023-04-25 17:43:06.114287 aio_overpass-0.1.1/aio_overpass/element.py
+-rwxr-xr-x   0        0        0    13665 2023-04-23 00:09:18.209185 aio_overpass-0.1.1/aio_overpass/error.py
+-rwxr-xr-x   0        0        0    24559 2023-04-25 17:41:10.606022 aio_overpass-0.1.1/aio_overpass/pt.py
+-rwxr-xr-x   0        0        0    22325 2023-04-25 17:41:10.603938 aio_overpass-0.1.1/aio_overpass/pt_ordered.py
+-rwxr-xr-x   0        0        0    14338 2023-04-25 17:41:10.546650 aio_overpass-0.1.1/aio_overpass/query.py
+-rwxr-xr-x   0        0        0     2160 2023-04-25 17:54:15.999637 aio_overpass-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     9265 1970-01-01 00:00:00.000000 aio_overpass-0.1.1/PKG-INFO
```

### Comparing `aio_overpass-0.1.0/LICENSE` & `aio_overpass-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aio_overpass-0.1.0/README.md` & `aio_overpass-0.1.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,36 @@
-# aio-overpass
+<h1 align="center">
+aio-overpass
+
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/timwie/aio-overpass/ci.yml)](https://github.com/timwie/aio-overpass/actions/workflows/ci.yml)
+[![codecov](https://codecov.io/gh/timwie/aio-overpass/branch/main/graph/badge.svg?token=YX1218U740)](https://codecov.io/gh/timwie/aio-overpass)
+[![PyPI version](https://badge.fury.io/py/aio_overpass.svg)](https://badge.fury.io/py/aio_overpass)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/aio-overpass)
+</h1>
+
 A client for the [Overpass API], a read-only API that serves up custom selected
 parts of [OpenStreetMap] data. It is optimized for data consumers that need a few
 elements within a glimpse or up to roughly 10 million elements in some minutes,
 both selected by search criteria like location, type of objects, tag properties,
 proximity, or combinations of them. To make use of it, you should familiarize yourself
 with [Overpass QL], the query language used to select the elements that you want.
 
 #### Contents
 - [Features](#features)
 - [Getting Started](#getting-started)
   - [Choosing Extras](#choosing-extras)
-  - [Dependencies](#dependencies)
 - [Basic Usage](#basic-usage)
   - [Example](#example)
 - [Motivation](#motivation)
 - [Related Projects](#related-projects)
 - [License](#license)
 
 #### See also
 - API reference is forthcoming :construction: 
-- Changelog is forthcoming :construction:
+- The version history is available in [CHANGELOG.md](CHANGELOG.md).
 - Contributor guide is forthcoming :construction:
 
 <br>
 
 ## Features
 - Asynchronous requests using [aiohttp]
 - Concurrent queries
@@ -177,18 +184,18 @@
             53.540877,
             9.9832434,
             53.5416212,
             9.9849674
         ]
     },
     "bbox": [
-        53.540877,
         9.9832434,
-        53.5416212,
+        53.540877,
         9.9849674
+        53.5416212,
     ]
 }
 ```
 
 <br>
 
 ## Motivation
@@ -214,14 +221,16 @@
 - [Folium], which can be used to visualize GeoJSON on [Leaflet] maps
 - [OSMnx], which is specialized on street networks
 - [overpass-api-python-wrapper], another Python client for the Overpass API
 - [overpy], another Python client for the Overpass API
 - [OSMPythonTools], a Python client for OSM-related services 
 - [overpassify], a Python to Overpass QL transpiler
 
+<br>
+
 ## License
 Distributed under the MIT License. See `LICENSE` for more information.
 
 
 [Overpass API]: https://wiki.openstreetmap.org/wiki/Overpass_API
 [Overpass QL]: https://wiki.openstreetmap.org/wiki/Overpass_API/Overpass_QL
 [OpenStreetMap]: https://www.openstreetmap.org
```

### Comparing `aio_overpass-0.1.0/aio_overpass/_dist.py` & `aio_overpass-0.1.1/aio_overpass/_dist.py`

 * *Files identical despite different names*

### Comparing `aio_overpass-0.1.0/aio_overpass/_ql.py` & `aio_overpass-0.1.1/aio_overpass/_ql.py`

 * *Files identical despite different names*

### Comparing `aio_overpass-0.1.0/aio_overpass/client.py` & `aio_overpass-0.1.1/aio_overpass/client.py`

 * *Files identical despite different names*

### Comparing `aio_overpass-0.1.0/aio_overpass/element.py` & `aio_overpass-0.1.1/aio_overpass/element.py`

 * *Files 1% similar despite different names*

```diff
@@ -280,15 +280,16 @@
 
 
 def _geojson_bbox(obj: Union[Element, "Relationship"]) -> Optional[Bbox]:
     elem = obj if isinstance(obj, Element) else obj.member
 
     bounds = elem._geometry.bounds
     if bounds:
-        return bounds
+        (minlat, minlon, maxlat, maxlon) = bounds
+        return minlon, minlat, maxlon, maxlat
 
 
 def _geojson_feature(obj: Union[Element, "Relationship"]) -> GeoJsonDict:
     feature = {
         "type": "Feature",
         "geometry": _geojson_geometry(obj),
         "properties": _geojson_properties(obj),
```

### Comparing `aio_overpass-0.1.0/aio_overpass/error.py` & `aio_overpass-0.1.1/aio_overpass/error.py`

 * *Files identical despite different names*

### Comparing `aio_overpass-0.1.0/aio_overpass/pt.py` & `aio_overpass-0.1.1/aio_overpass/pt.py`

 * *Files identical despite different names*

### Comparing `aio_overpass-0.1.0/aio_overpass/pt_ordered.py` & `aio_overpass-0.1.1/aio_overpass/pt_ordered.py`

 * *Files identical despite different names*

### Comparing `aio_overpass-0.1.0/aio_overpass/query.py` & `aio_overpass-0.1.1/aio_overpass/query.py`

 * *Files identical despite different names*

### Comparing `aio_overpass-0.1.0/pyproject.toml` & `aio_overpass-0.1.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "aio-overpass"
-version = "0.1.0"
+version = "0.1.1"
 description = "Async client for the Overpass API"
 authors = ["Tim Wiechers <mail@timwie.dev>"]
 license = "MIT"
 readme = "README.md"
-repository = "https://github.com/timwie/aio_overpass"
+repository = "https://github.com/timwie/aio-overpass"
 # TODO documentation = "https://..."
 packages = [{ include = "aio_overpass" }]
 include = [] # TODO "CHANGELOG.md"
 exclude = ["test/", "tasks.py"]
 keywords = [
     "geojson",
     "geospatial",
@@ -41,24 +41,25 @@
 joblib = ["joblib"]
 networkx = ["networkx"]
 shapely = ["shapely"]
 
 [tool.poetry.dev-dependencies]
 aioresponses = "^0.7.4"
 black = "^23.3.0"
+codecov = "^2.1.13"
 folium = "^0.14.0"
 invoke = "^2.0.0"
 isort = "^5.12.0"
 jupyterlab = "^3.6.3"
-pdoc = "^13.1.0"
+pdoc = "^13.1.1"
 pytest = "^7.3.1"
 pytest-asyncio = "^0.21.0"
 pytest-cov = "^4.0.0"
 randomcolor = "^0.4.4.6"
-ruff = "^0.0.262"
+ruff = "^0.0.263"
 tabulate = "^0.9.0"
 
 [tool.ruff]
 # https://github.com/charliermarsh/ruff#configuration
 # https://beta.ruff.rs/docs/rules/
 line-length = 100
 target-version = "py38"
```

### Comparing `aio_overpass-0.1.0/PKG-INFO` & `aio_overpass-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: aio-overpass
-Version: 0.1.0
+Version: 0.1.1
 Summary: Async client for the Overpass API
-Home-page: https://github.com/timwie/aio_overpass
+Home-page: https://github.com/timwie/aio-overpass
 License: MIT
 Keywords: geojson,geospatial,gis,open-street-map,osm,overpass-api,public-transport
 Author: Tim Wiechers
 Author-email: mail@timwie.dev
 Requires-Python: >=3.8,<4.0
 Classifier: Framework :: AsyncIO
 Classifier: Framework :: aiohttp
@@ -24,39 +24,46 @@
 Provides-Extra: joblib
 Provides-Extra: networkx
 Provides-Extra: shapely
 Requires-Dist: aiohttp (>=3.8.4,<3.9.0)
 Requires-Dist: joblib (>=1.2.0,<1.3.0) ; extra == "joblib"
 Requires-Dist: networkx (>=3.1,<3.2) ; extra == "networkx"
 Requires-Dist: shapely (>=2.0.1,<2.1.0) ; extra == "shapely"
-Project-URL: Repository, https://github.com/timwie/aio_overpass
+Project-URL: Repository, https://github.com/timwie/aio-overpass
 Description-Content-Type: text/markdown
 
-# aio-overpass
+<h1 align="center">
+aio-overpass
+
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/timwie/aio-overpass/ci.yml)](https://github.com/timwie/aio-overpass/actions/workflows/ci.yml)
+[![codecov](https://codecov.io/gh/timwie/aio-overpass/branch/main/graph/badge.svg?token=YX1218U740)](https://codecov.io/gh/timwie/aio-overpass)
+[![PyPI version](https://badge.fury.io/py/aio_overpass.svg)](https://badge.fury.io/py/aio_overpass)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/aio-overpass)
+</h1>
+
 A client for the [Overpass API], a read-only API that serves up custom selected
 parts of [OpenStreetMap] data. It is optimized for data consumers that need a few
 elements within a glimpse or up to roughly 10 million elements in some minutes,
 both selected by search criteria like location, type of objects, tag properties,
 proximity, or combinations of them. To make use of it, you should familiarize yourself
 with [Overpass QL], the query language used to select the elements that you want.
 
 #### Contents
 - [Features](#features)
 - [Getting Started](#getting-started)
   - [Choosing Extras](#choosing-extras)
-  - [Dependencies](#dependencies)
 - [Basic Usage](#basic-usage)
   - [Example](#example)
 - [Motivation](#motivation)
 - [Related Projects](#related-projects)
 - [License](#license)
 
 #### See also
 - API reference is forthcoming :construction: 
-- Changelog is forthcoming :construction:
+- The version history is available in [CHANGELOG.md](CHANGELOG.md).
 - Contributor guide is forthcoming :construction:
 
 <br>
 
 ## Features
 - Asynchronous requests using [aiohttp]
 - Concurrent queries
@@ -210,18 +217,18 @@
             53.540877,
             9.9832434,
             53.5416212,
             9.9849674
         ]
     },
     "bbox": [
-        53.540877,
         9.9832434,
-        53.5416212,
+        53.540877,
         9.9849674
+        53.5416212,
     ]
 }
 ```
 
 <br>
 
 ## Motivation
@@ -247,14 +254,16 @@
 - [Folium], which can be used to visualize GeoJSON on [Leaflet] maps
 - [OSMnx], which is specialized on street networks
 - [overpass-api-python-wrapper], another Python client for the Overpass API
 - [overpy], another Python client for the Overpass API
 - [OSMPythonTools], a Python client for OSM-related services 
 - [overpassify], a Python to Overpass QL transpiler
 
+<br>
+
 ## License
 Distributed under the MIT License. See `LICENSE` for more information.
 
 
 [Overpass API]: https://wiki.openstreetmap.org/wiki/Overpass_API
 [Overpass QL]: https://wiki.openstreetmap.org/wiki/Overpass_API/Overpass_QL
 [OpenStreetMap]: https://www.openstreetmap.org
```

