# Comparing `tmp/antimeridian-0.1.0.tar.gz` & `tmp/antimeridian-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antimeridian-0.1.0.tar", last modified: Tue Apr 18 13:56:35 2023, max compression
+gzip compressed data, was "antimeridian-0.2.0.tar", last modified: Wed Apr 26 19:57:55 2023, max compression
```

## Comparing `antimeridian-0.1.0.tar` & `antimeridian-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:56:35.303094 antimeridian-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     9723 2023-04-18 13:56:26.000000 antimeridian-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-04-18 13:56:35.303094 antimeridian-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-04-18 13:56:26.000000 antimeridian-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-18 13:56:26.000000 antimeridian-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 13:56:35.303094 antimeridian-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:56:35.303094 antimeridian-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:56:35.303094 antimeridian-0.1.0/src/antimeridian/
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-04-18 13:56:26.000000 antimeridian-0.1.0/src/antimeridian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-18 13:56:26.000000 antimeridian-0.1.0/src/antimeridian/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7974 2023-04-18 13:56:26.000000 antimeridian-0.1.0/src/antimeridian/_implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:56:35.303094 antimeridian-0.1.0/src/antimeridian.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-04-18 13:56:35.000000 antimeridian-0.1.0/src/antimeridian.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-18 13:56:35.000000 antimeridian-0.1.0/src/antimeridian.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 13:56:35.000000 antimeridian-0.1.0/src/antimeridian.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-18 13:56:35.000000 antimeridian-0.1.0/src/antimeridian.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-18 13:56:35.000000 antimeridian-0.1.0/src/antimeridian.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-18 13:56:35.000000 antimeridian-0.1.0/src/antimeridian.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:56:35.303094 antimeridian-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-18 13:56:26.000000 antimeridian-0.1.0/tests/test_fix_geojson.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-18 13:56:26.000000 antimeridian-0.1.0/tests/test_multi_polygon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-04-18 13:56:26.000000 antimeridian-0.1.0/tests/test_polygon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:57:55.125674 antimeridian-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     9723 2023-04-26 19:57:41.000000 antimeridian-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5457 2023-04-26 19:57:55.125674 antimeridian-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-04-26 19:57:41.000000 antimeridian-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-26 19:57:41.000000 antimeridian-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 19:57:55.125674 antimeridian-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:57:55.121674 antimeridian-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:57:55.125674 antimeridian-0.2.0/src/antimeridian/
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-26 19:57:41.000000 antimeridian-0.2.0/src/antimeridian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-26 19:57:41.000000 antimeridian-0.2.0/src/antimeridian/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11445 2023-04-26 19:57:41.000000 antimeridian-0.2.0/src/antimeridian/_implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:57:55.125674 antimeridian-0.2.0/src/antimeridian.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5457 2023-04-26 19:57:55.000000 antimeridian-0.2.0/src/antimeridian.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-26 19:57:55.000000 antimeridian-0.2.0/src/antimeridian.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 19:57:55.000000 antimeridian-0.2.0/src/antimeridian.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-26 19:57:55.000000 antimeridian-0.2.0/src/antimeridian.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-26 19:57:55.000000 antimeridian-0.2.0/src/antimeridian.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-26 19:57:55.000000 antimeridian-0.2.0/src/antimeridian.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:57:55.125674 antimeridian-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-26 19:57:41.000000 antimeridian-0.2.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-26 19:57:41.000000 antimeridian-0.2.0/tests/test_geojson.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-26 19:57:41.000000 antimeridian-0.2.0/tests/test_multi_polygon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-26 19:57:41.000000 antimeridian-0.2.0/tests/test_polygon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-26 19:57:41.000000 antimeridian-0.2.0/tests/test_segment.py
```

### Comparing `antimeridian-0.1.0/LICENSE` & `antimeridian-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `antimeridian-0.1.0/PKG-INFO` & `antimeridian-0.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 Metadata-Version: 2.1
 Name: antimeridian
-Version: 0.1.0
+Version: 0.2.0
 Summary: Fix GeoJSON geometries that cross the antimeridian
 Author-email: Pete Gadomski <pete.gadomski@gmail.com>
 License: Apache-2.0
+Project-URL: documentation, https://antimeridian.readthedocs.io
+Project-URL: repository, https://github.com/gadomski/antimeridan
+Project-URL: changelog, https://github.com/gadomski/antimeridian/blob/main/CHANGELOG.md
 Keywords: geojson,antimeridian,shapely
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: cli
 Provides-Extra: dev
 Provides-Extra: docs
 License-File: LICENSE
 
 # antimeridian
 
 [![CI Status](https://img.shields.io/github/actions/workflow/status/gadomski/antimeridian/ci.yaml?style=for-the-badge&label=CI)](https://github.com/gadomski/antimeridian/actions/workflows/ci.yaml)
@@ -33,18 +37,19 @@
 Then, in your code:
 
 ```python
 import antimeridian
 fixed = antimeridian.fix_geojson(geojson)
 ```
 
-There's a command-line entrypoint, too:
+If you'd like to use the command line interface:
 
 ```shell
-fix-antimeridian input.json > output.json
+pip install 'antimeridian[cli]'
+antimeridian --help
 ```
 
 ## Background
 
 ### What's the antimeridian?
 
 Also known as the [180th meridian](https://en.wikipedia.org/wiki/180th_meridian), the antimeridian is the line of longitude on the opposite side of the world from the prime meridian.
```

### Comparing `antimeridian-0.1.0/README.md` & `antimeridian-0.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -18,18 +18,19 @@
 Then, in your code:
 
 ```python
 import antimeridian
 fixed = antimeridian.fix_geojson(geojson)
 ```
 
-There's a command-line entrypoint, too:
+If you'd like to use the command line interface:
 
 ```shell
-fix-antimeridian input.json > output.json
+pip install 'antimeridian[cli]'
+antimeridian --help
 ```
 
 ## Background
 
 ### What's the antimeridian?
 
 Also known as the [180th meridian](https://en.wikipedia.org/wiki/180th_meridian), the antimeridian is the line of longitude on the opposite side of the world from the prime meridian.
```

### Comparing `antimeridian-0.1.0/pyproject.toml` & `antimeridian-0.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools >= 64"]
 
 [project]
 name = "antimeridian"
-version = "0.1.0"
+version = "0.2.0"
 authors = [
     {name = "Pete Gadomski", email = "pete.gadomski@gmail.com"}
 ]
 description = "Fix GeoJSON geometries that cross the antimeridian"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["geojson", "antimeridian", "shapely"]
@@ -16,29 +16,38 @@
     "Programming Language :: Python :: 3",
     "Development Status :: 4 - Beta",
 ]
 dependencies = [
     "shapely>=1.8"
 ]
 
+[project.urls]
+documentation = "https://antimeridian.readthedocs.io"
+repository = "https://github.com/gadomski/antimeridan"
+changelog = "https://github.com/gadomski/antimeridian/blob/main/CHANGELOG.md"
+
 [project.optional-dependencies]
+cli = [
+    "click~=8.1"
+]
 dev = [
     "black~=23.3",
     "mypy~=1.2",
     "pre-commit~=3.2",
     "pytest~=7.3",
-    "ruff==0.0.261",
+    "pytest-console-scripts~=1.3",
+    "ruff==0.0.262",
 ]
 docs = [
     "pydata-sphinx-theme~=0.13",
     "sphinx~=6.1",
 ]
 
 [project.scripts]
-fix-antimeridian = "antimeridian:main"
+antimeridian = "antimeridian._cli:cli"
 
 [tool.mypy]
 strict = true
 
 [[tool.mypy.overrides]]
 module = ["shapely", "shapely.geometry"]
 ignore_missing_imports = true
```

### Comparing `antimeridian-0.1.0/src/antimeridian/_implementation.py` & `antimeridian-0.2.0/src/antimeridian/_implementation.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,21 @@
+"""Implementation module for the antimeridian package.
+
+This is a "private" module that is not part of our public API. Downstream users
+should not use these functions and objects directly; instead, use the functions
+explicitly imported into the top-level of the package. The interfaces in this
+module can change at any time without warning.
+"""
+
 from __future__ import annotations
 
 from typing import Any, Dict, List, Optional, Protocol, Tuple, Union, cast
 
 import shapely.geometry
-from shapely.geometry import MultiPolygon, Polygon
+from shapely.geometry import MultiLineString, MultiPolygon, Polygon
 
 Point = Tuple[float, float]
 
 
 class GeoInterface(Protocol):
     """A simple protocol for things that have a ``__geo_interface__`` method.
 
@@ -49,14 +57,46 @@
             features[i] = fix_geojson(feature)
         geojson["features"] = features
         return geojson
     else:
         return fix_shape(geojson)
 
 
+def segment_geojson(geojson: Dict[str, Any]) -> MultiLineString:
+    """Segments a GeoJSON object into a MultiLineString.
+
+    If the object does not cross the antimeridian, its exterior and interior
+    line strings are returned unchanged.
+
+    Args:
+        geojson: A GeoJSON object as a dictionary
+
+    Return:
+        A MutliLineString of segments.
+    """
+    type_ = geojson.get("type", None)
+    if type_ is None:
+        raise ValueError("no 'type' field found in GeoJSON")
+    elif type_ == "Feature":
+        geometry = geojson.get("geometry", None)
+        if geometry is None:
+            raise ValueError("no 'geometry' field found in GeoJSON Feature")
+        return MultiLineString(segment_shape(geometry))
+    elif type_ == "FeatureCollection":
+        features = geojson.get("features", None)
+        if features is None:
+            raise ValueError("no 'features' field found in GeoJSON FeatureCollection")
+        segments = list()
+        for feature in features:
+            segments.extend(segment_geojson(feature))
+        return MultiLineString(segments)
+    else:
+        return MultiLineString(segment_shape(geojson))
+
+
 def fix_shape(shape: Dict[str, Any] | GeoInterface) -> Dict[str, Any]:
     """Fixes a shape that crosses the antimeridian.
 
     Args:
         shape: A polygon or multi-polygon, either as a dictionary or as a
             :py:class:`GeoInterface`. Uses :py:func:`shapely.geometry.shape`
             under the hood.
@@ -69,14 +109,27 @@
         return cast(Dict[str, Any], shapely.geometry.mapping(fix_polygon(geom)))
     elif geom.geom_type == "MultiPolygon":
         return cast(Dict[str, Any], shapely.geometry.mapping(fix_multi_polygon(geom)))
     else:
         raise ValueError(f"unsupported geom_type: {geom.geom_type}")
 
 
+def segment_shape(shape: Dict[str, Any] | GeoInterface) -> List[List[Point]]:
+    geom = shapely.geometry.shape(shape)
+    if geom.geom_type == "Polygon":
+        return segment_polygon(geom)
+    elif geom.geom_type == "MultiPolygon":
+        segments = list()
+        for polygon in geom.geoms:
+            segments += segment_polygon(polygon)
+        return segments
+    else:
+        raise ValueError(f"unsupported geom_type: {geom.geom_type}")
+
+
 def fix_multi_polygon(multi_polygon: MultiPolygon) -> MultiPolygon:
     """Fixes a :py:class:`shapely.geometry.MultiPolygon`.
 
     Args:
         multi_polygon: The multi-polygon
 
     Returns:
@@ -101,41 +154,59 @@
     polygons = fix_polygon_to_list(polygon)
     if len(polygons) == 1:
         return polygons[0]
     else:
         return MultiPolygon(polygons)
 
 
+def segment_polygon(polygon: Polygon) -> List[List[Point]]:
+    segments = segment(list(polygon.exterior.coords))
+    if not segments:
+        segments = [list(polygon.exterior.coords)]
+    for interior in polygon.interiors:
+        interior_segments = segment(list(interior.coords))
+        if interior_segments:
+            segments.extend(interior_segments)
+        else:
+            segments.append(list(interior.coords))
+    return segments
+
+
 def fix_polygon_to_list(polygon: Polygon) -> List[Polygon]:
-    segments = segment(polygon.exterior.coords)
+    segments = segment(list(polygon.exterior.coords))
     if not segments:
         return [polygon]
     else:
         interiors = []
         for interior in polygon.interiors:
-            interior_segments = segment(interior.coords)
+            interior_segments = segment(list(interior.coords))
             if interior_segments:
                 segments.extend(interior_segments)
             else:
                 interiors.append(interior)
     segments = extend_over_poles(segments)
     polygons = build_polygons(segments)
     assert polygons
-    for interior in interiors:
-        for i, polygon in enumerate(polygons):
+    for i, polygon in enumerate(polygons):
+        for j, interior in enumerate(interiors):
             if polygon.contains(interior):
-                interiors = list(polygon.interiors)
-                interiors.append(interior)
-                polygons[i] = Polygon(polygon.exterior, interiors)
+                interior = interiors.pop(j)
+                polygon_interiors = list(polygon.interiors)
+                polygon_interiors.append(interior)
+                polygons[i] = Polygon(polygon.exterior, polygon_interiors)
+    assert not interiors
     return polygons
 
 
 def segment(coords: List[Point]) -> List[List[Point]]:
     segment = []
     segments = []
+    for i, point in enumerate(coords):
+        # Ensure all longitudes are between -180 and 180
+        coords[i] = (((point[0] + 180) % 360) - 180, point[1])
     for start, end in zip(coords, coords[1:]):
         segment.append(start)
         if (end[0] - start[0] > 180) and (end[0] - start[0] != 360):  # left
             latitude = crossing_latitude(start, end)
             segment.append((-180, latitude))
             segments.append(segment)
             segment = [(180, latitude)]
@@ -183,56 +254,73 @@
             left_ends.append((i, segment[-1][1]))
         else:
             right_ends.append((i, segment[-1][1]))
     left_ends.sort(key=lambda v: v[1])
     left_starts.sort(key=lambda v: v[1])
     right_ends.sort(key=lambda v: v[1], reverse=True)
     right_starts.sort(key=lambda v: v[1], reverse=True)
+    # If there's no segment ends between a start and the pole, extend the
+    # segment over the pole.
     if left_ends and (not left_starts or left_ends[0][1] < left_starts[0][1]):
         segments[left_ends[0][0]] += [(-180, -90), (180, -90)]
     if right_ends and (not right_starts or right_ends[0][1] > right_starts[0][1]):
         segments[right_ends[0][0]] += [(180, 90), (-180, 90)]
     return segments
 
 
 def build_polygons(
     segments: List[List[Point]],
 ) -> List[Polygon]:
     if not segments:
         return []
     segment = segments.pop()
-    right = (
-        segment[-1][0] == 180
-    )  # all segments should start and end at abs(180) longitude
-    candidates: List[
-        Tuple[Optional[int], float, bool]
-    ] = list()  # list of (index, latitude, is_start)
-    if segment[0][0] == segment[-1][0] and (
-        (right and segment[0][1] > segment[-1][1])
-        or (not right and segment[0][1] < segment[-1][1])
-    ):
-        candidates.append((None, segment[0][1], True))
+    is_right = segment[-1][0] == 180
+    candidates: List[Tuple[Optional[int], float]] = list()
+    if is_self_closing(segment):
+        # Self-closing segments might end up joining up with themselves. They
+        # might not, e.g. donuts.
+        candidates.append((None, segment[0][1]))
     for i, s in enumerate(segments):
+        # Is the start of s on the same side as the end of segment?
         if s[0][0] == segment[-1][0]:
-            if (right and s[0][1] > segment[-1][1]) or (
-                not right and s[0][1] < segment[-1][1]
-            ):
-                candidates.append((i, s[0][1], True))
-        if s[-1][0] == segment[-1][0]:
-            if (right and s[-1][1] > segment[-1][1]) or (
-                not right and s[-1][1] < segment[-1][1]
+            # If so, check the following:
+            # - Is the start of s closer to the pole than the end of segment, and
+            # - is the end of s on the other side, or
+            # - is the end of s further away from the pole than the start of
+            #   segment (e.g. donuts)?
+            if (
+                is_right
+                and s[0][1] > segment[-1][1]
+                and (not is_self_closing(s) or s[-1][1] < segment[0][1])
+            ) or (
+                not is_right
+                and s[0][1] < segment[-1][1]
+                and (not is_self_closing(s) or s[-1][1] > segment[0][1])
             ):
-                candidates.append((i, s[-1][1], False))
-    candidates.sort(key=lambda c: c[1], reverse=not right)
-    if candidates and candidates[0][2]:
+                candidates.append((i, s[0][1]))
+
+    # Sort the candidates so the closest point is first in the list.
+    candidates.sort(key=lambda c: c[1], reverse=not is_right)
+    if candidates:
         index = candidates[0][0]
     else:
         index = None
 
     if index is not None:
-        segment = segments.pop(index) + segment
+        # Join the segments, then re-add them to the list and recurse.
+        segment = segment + segments.pop(index)
         segments.append(segment)
         return build_polygons(segments)
     else:
+        # This segment should self-joining, so just build the rest of the
+        # polygons without it.
         polygons = build_polygons(segments)
         polygons.append(Polygon(segment))
         return polygons
+
+
+def is_self_closing(segment: List[Point]) -> bool:
+    is_right = segment[-1][0] == 180
+    return segment[0][0] == segment[-1][0] and (
+        (is_right and segment[0][1] > segment[-1][1])
+        or (not is_right and segment[0][1] < segment[-1][1])
+    )
```

### Comparing `antimeridian-0.1.0/src/antimeridian.egg-info/PKG-INFO` & `antimeridian-0.2.0/src/antimeridian.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 Metadata-Version: 2.1
 Name: antimeridian
-Version: 0.1.0
+Version: 0.2.0
 Summary: Fix GeoJSON geometries that cross the antimeridian
 Author-email: Pete Gadomski <pete.gadomski@gmail.com>
 License: Apache-2.0
+Project-URL: documentation, https://antimeridian.readthedocs.io
+Project-URL: repository, https://github.com/gadomski/antimeridan
+Project-URL: changelog, https://github.com/gadomski/antimeridian/blob/main/CHANGELOG.md
 Keywords: geojson,antimeridian,shapely
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: cli
 Provides-Extra: dev
 Provides-Extra: docs
 License-File: LICENSE
 
 # antimeridian
 
 [![CI Status](https://img.shields.io/github/actions/workflow/status/gadomski/antimeridian/ci.yaml?style=for-the-badge&label=CI)](https://github.com/gadomski/antimeridian/actions/workflows/ci.yaml)
@@ -33,18 +37,19 @@
 Then, in your code:
 
 ```python
 import antimeridian
 fixed = antimeridian.fix_geojson(geojson)
 ```
 
-There's a command-line entrypoint, too:
+If you'd like to use the command line interface:
 
 ```shell
-fix-antimeridian input.json > output.json
+pip install 'antimeridian[cli]'
+antimeridian --help
 ```
 
 ## Background
 
 ### What's the antimeridian?
 
 Also known as the [180th meridian](https://en.wikipedia.org/wiki/180th_meridian), the antimeridian is the line of longitude on the opposite side of the world from the prime meridian.
```

### Comparing `antimeridian-0.1.0/tests/test_fix_geojson.py` & `antimeridian-0.2.0/tests/test_geojson.py`

 * *Files 25% similar despite different names*

```diff
@@ -25,7 +25,14 @@
         "features": [feature_a, feature_b],
         "another": "property",
     }
     fixed = antimeridian.fix_geojson(feature_collection)
     assert fixed["features"][0]["properties"]["foo"] == "bar"
     assert fixed["features"][1]["properties"]["baz"] == "boz"
     assert fixed["another"] == "property"
+
+
+def test_segment_feature(read_input: Reader) -> None:
+    input = read_input("split")
+    feature = {"type": "Feature", "geometry": input}
+    fixed = antimeridian.segment_geojson(feature)
+    assert len(fixed.geoms) == 2
```

### Comparing `antimeridian-0.1.0/tests/test_multi_polygon.py` & `antimeridian-0.2.0/tests/test_multi_polygon.py`

 * *Files identical despite different names*

### Comparing `antimeridian-0.1.0/tests/test_polygon.py` & `antimeridian-0.2.0/tests/test_polygon.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
+import antimeridian
 import pytest
 import shapely.geometry
 from shapely.geometry import MultiPolygon, Polygon
 
-import antimeridian
-
 from .conftest import Reader
 
 
 @pytest.mark.parametrize(
     ("name"),
     [
         "both-poles",
         "complex-split",
         "crossing-latitude",
         "extra-crossing",
         "latitude-band",
         "north-pole",
         "one-hole",
+        "over-180",
+        "overlap",
         "simple",
         "south-pole",
         "split",
         "two-holes",
     ],
 )
 def test_fix_polygon(
@@ -29,15 +30,14 @@
     read_output: Reader,
 ) -> None:
     input = read_input(name)
     assert isinstance(input, Polygon)
     output = read_output(name)
     assert isinstance(input, Polygon | MultiPolygon)
     fixed = antimeridian.fix_polygon(input).normalize()
-    assert fixed.is_valid
     assert fixed == output.normalize()
 
 
 def test_fix_shape(read_input: Reader) -> None:
     # Just a smoke test
     input = shapely.geometry.mapping(read_input("simple"))
     antimeridian.fix_shape(input)
```

