# Comparing `tmp/here-polyline-converter-0.2.0.tar.gz` & `tmp/here-polyline-converter-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "here-polyline-converter-0.2.0.tar", last modified: Tue Apr 25 08:43:35 2023, max compression
+gzip compressed data, was "here-polyline-converter-0.2.1.tar", last modified: Wed Apr 26 08:50:30 2023, max compression
```

## Comparing `here-polyline-converter-0.2.0.tar` & `here-polyline-converter-0.2.1.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:43:35.881357 here-polyline-converter-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-25 08:43:23.000000 here-polyline-converter-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-25 08:43:23.000000 here-polyline-converter-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-04-25 08:43:35.881357 here-polyline-converter-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-04-25 08:43:23.000000 here-polyline-converter-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-25 08:43:23.000000 here-polyline-converter-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-25 08:43:23.000000 here-polyline-converter-0.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-04-25 08:43:35.881357 here-polyline-converter-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-25 08:43:23.000000 here-polyline-converter-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:43:35.877357 here-polyline-converter-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:43:35.881357 here-polyline-converter-0.2.0/src/here_polyline_converter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-04-25 08:43:35.000000 here-polyline-converter-0.2.0/src/here_polyline_converter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-25 08:43:35.000000 here-polyline-converter-0.2.0/src/here_polyline_converter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 08:43:35.000000 here-polyline-converter-0.2.0/src/here_polyline_converter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 08:43:35.000000 here-polyline-converter-0.2.0/src/here_polyline_converter.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-25 08:43:35.000000 here-polyline-converter-0.2.0/src/here_polyline_converter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 08:43:35.000000 here-polyline-converter-0.2.0/src/here_polyline_converter.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:43:35.877357 here-polyline-converter-0.2.0/src/here_search/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:43:35.881357 here-polyline-converter-0.2.0/src/here_search/polyline_converter/
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-04-25 08:43:23.000000 here-polyline-converter-0.2.0/src/here_search/polyline_converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-04-25 08:43:23.000000 here-polyline-converter-0.2.0/src/here_search/polyline_converter/decoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-25 08:43:23.000000 here-polyline-converter-0.2.0/src/here_search/polyline_converter/encoding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:50:30.808040 here-polyline-converter-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-26 08:50:12.000000 here-polyline-converter-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-26 08:50:12.000000 here-polyline-converter-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-04-26 08:50:30.808040 here-polyline-converter-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-04-26 08:50:12.000000 here-polyline-converter-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-26 08:50:12.000000 here-polyline-converter-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-26 08:50:12.000000 here-polyline-converter-0.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-04-26 08:50:30.808040 here-polyline-converter-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-26 08:50:12.000000 here-polyline-converter-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:50:30.808040 here-polyline-converter-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:50:30.808040 here-polyline-converter-0.2.1/src/here_polyline_converter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-04-26 08:50:30.000000 here-polyline-converter-0.2.1/src/here_polyline_converter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-26 08:50:30.000000 here-polyline-converter-0.2.1/src/here_polyline_converter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 08:50:30.000000 here-polyline-converter-0.2.1/src/here_polyline_converter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 08:50:30.000000 here-polyline-converter-0.2.1/src/here_polyline_converter.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-26 08:50:30.000000 here-polyline-converter-0.2.1/src/here_polyline_converter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-26 08:50:30.000000 here-polyline-converter-0.2.1/src/here_polyline_converter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:50:30.808040 here-polyline-converter-0.2.1/src/here_search/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:50:30.808040 here-polyline-converter-0.2.1/src/here_search/polyline_converter/
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-04-26 08:50:12.000000 here-polyline-converter-0.2.1/src/here_search/polyline_converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-04-26 08:50:12.000000 here-polyline-converter-0.2.1/src/here_search/polyline_converter/decoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-26 08:50:12.000000 here-polyline-converter-0.2.1/src/here_search/polyline_converter/encoding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:50:30.808040 here-polyline-converter-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6940 2023-04-26 08:50:12.000000 here-polyline-converter-0.2.1/tests/test_converter.py
```

### Comparing `here-polyline-converter-0.2.0/LICENSE` & `here-polyline-converter-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `here-polyline-converter-0.2.0/PKG-INFO` & `here-polyline-converter-0.2.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,92 +1,96 @@
 Metadata-Version: 2.1
 Name: here-polyline-converter
-Version: 0.2.0
+Version: 0.2.1
 Summary: A tool to convert strings between HERE Flexible Polyline format and the (now legacy) format used in HERE Places API
 Home-page: https://here.com
 Author: HERE Europe B.V.
 Author-email: emmanuel.decitre@here.com
 License: The MIT License
-Description: ![workflow][b]
-        [![codecov][c1]][c2]
-        
-        A tool to encode/decode [HERE legacy polyline][4] strings and convert them from/into HERE [Flexible Polyline][1] format.
-        
-        Note that the [HERE Places (Search) API][2] is in maintenance: Developers need to adapt their applications to the newer
-        [HERE Geocoding & Search API][3] to benefit from the features developed after 2018.
-        
-        
-        ## Install
-        
-        ```shell
-        pip install here-polyline-converter
-        ```
-        
-        ## Usage
-        
-        
-        ```python
-        >>> convert_legacy_to_flex(legacy_polyline_string)
-        ```
-        
-        Transforms a HERE legacy polyline string into a flexible polyline string. The legacy Polyline third dimension (segments width changes) is ignored.
-        
-        ```python
-        >>> encode_legacy(iterable)
-        ```
-        
-        Encodes a list of coordinates to the corresponding HERE legacy polyline string representation. 
-        Expected coordinates order: `(lat, lng[, width])`. Note that `width` is expected to be one of `DW`, `HW`, `CW`.
-        
-        
-        ```python
-        >>> decode_legacy(legacy_polyline_string)
-        ```
-        
-        Decodes a HERE legacy polyline string into an array of coordinates `(lat, lng[, width])`.
-        
-        
-        Note that `width` is expected to be one of `DW`, `HW`, `CW`.
-        
-        #### Examples
-        
-        ```python
-        >>> import here_search.polyline_converter as pc
-        >>> legacy_polyline = "oz5xJ67i1B1B7PzIhaxL7Y"
-        >>> flexible_polyline = pc.convert_legacy_to_flex(legacy_polyline)
-        >>> flexible_polyline
-        'BFoz5xJ67i1B1B7PzIhaxL7Y'
-        
-        >>> points = [(50.1022829, 8.6982122), (50.1020076, 8.6956695), (50.1006313, 8.6914960), (50.0987800, 8.6875156)]
-        >>> pc.encode_legacy(points)
-        'oz5xJ67i1B1B7PzIhaxL7Y'
-        
-        >>> legacy_polyline = "oz5xJ67i1B.C1B7PzIha.DxL7Y"
-        >>> pc.decode_legacy(legacy_polyline)
-        [(50.10228, 8.69821, 'CW'), (50.10201, 8.69567), (50.10063, 8.6915, 'DW'), (50.09878, 8.68752)]
-        ```
-        
-        ## License
-        
-        Copyright (C) 2023 HERE Europe B.V.
-        
-        See the [LICENSE](./LICENSE) file in the root of this project for license details.
-        
-        [1]: https://github.com/heremaps/flexible-polyline
-        [2]: https://developer.here.com/documentation/places/dev_guide/topics/guide.html
-        [3]: https://developer.here.com/documentation/geocoding-search-api/dev_guide/index.html
-        [4]: https://developer.here.com/documentation/places/dev_guide/topics/location-contexts.html#location-contexts__here-polyline-encoding
-        [b]: https://github.com/heremaps/here-polyline-converter/actions/workflows/test.yml/badge.svg
-        [c1]: https://codecov.io/gh/heremaps/here-polyline-converter/branch/main/graph/badge.svg?token=9LPI9T7BMN
-        [c2]: https://codecov.io/gh/heremaps/here-polyline-converter
+Project-URL: Bug Tracker, https://github.com/heremaps/here-polyline-converter/issues
+Project-URL: Source, https://github.com/heremaps/here-polyline-converter
 Keywords: HERE,Search,Polyline,GS7
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+![workflow][b]
+[![codecov][c1]][c2]
+
+A tool to encode/decode [HERE legacy polyline][4] strings and convert them from/into HERE [Flexible Polyline][1] format.
+
+Note that the [HERE Places (Search) API][2] is in maintenance: Developers need to adapt their applications to the newer
+[HERE Geocoding & Search API][3] to benefit from the features developed after 2018.
+
+
+## Install
+
+```shell
+pip install here-polyline-converter
+```
+
+## Usage
+
+
+```python
+>>> convert_legacy_to_flex(legacy_polyline_string)
+```
+
+Transforms a HERE legacy polyline string into a flexible polyline string. The legacy Polyline third dimension (segments width changes) is ignored.
+
+```python
+>>> encode_legacy(iterable)
+```
+
+Encodes a list of coordinates to the corresponding HERE legacy polyline string representation. 
+Expected coordinates order: `(lat, lng[, width])`. Note that `width` is expected to be one of `DW`, `HW`, `CW`.
+
+
+```python
+>>> decode_legacy(legacy_polyline_string)
+```
+
+Decodes a HERE legacy polyline string into an array of coordinates `(lat, lng[, width])`.
+
+
+Note that `width` is expected to be one of `DW`, `HW`, `CW`.
+
+#### Examples
+
+```python
+>>> import here_search.polyline_converter as pc
+>>> legacy_polyline = "oz5xJ67i1B1B7PzIhaxL7Y"
+>>> flexible_polyline = pc.convert_legacy_to_flex(legacy_polyline)
+>>> flexible_polyline
+'BFoz5xJ67i1B1B7PzIhaxL7Y'
+
+>>> points = [(50.1022829, 8.6982122), (50.1020076, 8.6956695), (50.1006313, 8.6914960), (50.0987800, 8.6875156)]
+>>> pc.encode_legacy(points)
+'oz5xJ67i1B1B7PzIhaxL7Y'
+
+>>> legacy_polyline = "oz5xJ67i1B.C1B7PzIha.DxL7Y"
+>>> pc.decode_legacy(legacy_polyline)
+[(50.10228, 8.69821, 'CW'), (50.10201, 8.69567), (50.10063, 8.6915, 'DW'), (50.09878, 8.68752)]
+```
+
+## License
+
+Copyright (C) 2023 HERE Europe B.V.
+
+See the [LICENSE](./LICENSE) file in the root of this project for license details.
+
+[1]: https://github.com/heremaps/flexible-polyline
+[2]: https://developer.here.com/documentation/places/dev_guide/topics/guide.html
+[3]: https://developer.here.com/documentation/geocoding-search-api/dev_guide/index.html
+[4]: https://developer.here.com/documentation/places/dev_guide/topics/location-contexts.html#location-contexts__here-polyline-encoding
+[b]: https://github.com/heremaps/here-polyline-converter/actions/workflows/test.yml/badge.svg
+[c1]: https://codecov.io/gh/heremaps/here-polyline-converter/branch/main/graph/badge.svg?token=9LPI9T7BMN
+[c2]: https://codecov.io/gh/heremaps/here-polyline-converter
```

### Comparing `here-polyline-converter-0.2.0/README.md` & `here-polyline-converter-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `here-polyline-converter-0.2.0/setup.cfg` & `here-polyline-converter-0.2.1/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [metadata]
 name = here-polyline-converter
-version = 0.2.0
+version = 0.2.1
 author = HERE Europe B.V.
 author_email = emmanuel.decitre@here.com
 url = https://here.com
-home-page = home-page = https://github.com/heremaps/here-polyline-converter
+home_page = https://github.com/heremaps/here-polyline-converter
 description = A tool to convert strings between HERE Flexible Polyline format and the (now legacy) format used in HERE Places API
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = The MIT License
 license_files = 
 	LICENSE
 keywords = HERE, Search, Polyline, GS7
@@ -18,14 +18,17 @@
 	Intended Audience :: Developers
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	License :: OSI Approved :: MIT License
+project_urls = 
+	Bug Tracker = https://github.com/heremaps/here-polyline-converter/issues
+	Source = https://github.com/heremaps/here-polyline-converter
 
 [options]
 zip_safe = False
 python_requires = >=3.7
 package_dir = 
 	= src
 install_requires = flexpolyline
```

### Comparing `here-polyline-converter-0.2.0/src/here_polyline_converter.egg-info/PKG-INFO` & `here-polyline-converter-0.2.1/src/here_polyline_converter.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,92 +1,96 @@
 Metadata-Version: 2.1
 Name: here-polyline-converter
-Version: 0.2.0
+Version: 0.2.1
 Summary: A tool to convert strings between HERE Flexible Polyline format and the (now legacy) format used in HERE Places API
 Home-page: https://here.com
 Author: HERE Europe B.V.
 Author-email: emmanuel.decitre@here.com
 License: The MIT License
-Description: ![workflow][b]
-        [![codecov][c1]][c2]
-        
-        A tool to encode/decode [HERE legacy polyline][4] strings and convert them from/into HERE [Flexible Polyline][1] format.
-        
-        Note that the [HERE Places (Search) API][2] is in maintenance: Developers need to adapt their applications to the newer
-        [HERE Geocoding & Search API][3] to benefit from the features developed after 2018.
-        
-        
-        ## Install
-        
-        ```shell
-        pip install here-polyline-converter
-        ```
-        
-        ## Usage
-        
-        
-        ```python
-        >>> convert_legacy_to_flex(legacy_polyline_string)
-        ```
-        
-        Transforms a HERE legacy polyline string into a flexible polyline string. The legacy Polyline third dimension (segments width changes) is ignored.
-        
-        ```python
-        >>> encode_legacy(iterable)
-        ```
-        
-        Encodes a list of coordinates to the corresponding HERE legacy polyline string representation. 
-        Expected coordinates order: `(lat, lng[, width])`. Note that `width` is expected to be one of `DW`, `HW`, `CW`.
-        
-        
-        ```python
-        >>> decode_legacy(legacy_polyline_string)
-        ```
-        
-        Decodes a HERE legacy polyline string into an array of coordinates `(lat, lng[, width])`.
-        
-        
-        Note that `width` is expected to be one of `DW`, `HW`, `CW`.
-        
-        #### Examples
-        
-        ```python
-        >>> import here_search.polyline_converter as pc
-        >>> legacy_polyline = "oz5xJ67i1B1B7PzIhaxL7Y"
-        >>> flexible_polyline = pc.convert_legacy_to_flex(legacy_polyline)
-        >>> flexible_polyline
-        'BFoz5xJ67i1B1B7PzIhaxL7Y'
-        
-        >>> points = [(50.1022829, 8.6982122), (50.1020076, 8.6956695), (50.1006313, 8.6914960), (50.0987800, 8.6875156)]
-        >>> pc.encode_legacy(points)
-        'oz5xJ67i1B1B7PzIhaxL7Y'
-        
-        >>> legacy_polyline = "oz5xJ67i1B.C1B7PzIha.DxL7Y"
-        >>> pc.decode_legacy(legacy_polyline)
-        [(50.10228, 8.69821, 'CW'), (50.10201, 8.69567), (50.10063, 8.6915, 'DW'), (50.09878, 8.68752)]
-        ```
-        
-        ## License
-        
-        Copyright (C) 2023 HERE Europe B.V.
-        
-        See the [LICENSE](./LICENSE) file in the root of this project for license details.
-        
-        [1]: https://github.com/heremaps/flexible-polyline
-        [2]: https://developer.here.com/documentation/places/dev_guide/topics/guide.html
-        [3]: https://developer.here.com/documentation/geocoding-search-api/dev_guide/index.html
-        [4]: https://developer.here.com/documentation/places/dev_guide/topics/location-contexts.html#location-contexts__here-polyline-encoding
-        [b]: https://github.com/heremaps/here-polyline-converter/actions/workflows/test.yml/badge.svg
-        [c1]: https://codecov.io/gh/heremaps/here-polyline-converter/branch/main/graph/badge.svg?token=9LPI9T7BMN
-        [c2]: https://codecov.io/gh/heremaps/here-polyline-converter
+Project-URL: Bug Tracker, https://github.com/heremaps/here-polyline-converter/issues
+Project-URL: Source, https://github.com/heremaps/here-polyline-converter
 Keywords: HERE,Search,Polyline,GS7
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+![workflow][b]
+[![codecov][c1]][c2]
+
+A tool to encode/decode [HERE legacy polyline][4] strings and convert them from/into HERE [Flexible Polyline][1] format.
+
+Note that the [HERE Places (Search) API][2] is in maintenance: Developers need to adapt their applications to the newer
+[HERE Geocoding & Search API][3] to benefit from the features developed after 2018.
+
+
+## Install
+
+```shell
+pip install here-polyline-converter
+```
+
+## Usage
+
+
+```python
+>>> convert_legacy_to_flex(legacy_polyline_string)
+```
+
+Transforms a HERE legacy polyline string into a flexible polyline string. The legacy Polyline third dimension (segments width changes) is ignored.
+
+```python
+>>> encode_legacy(iterable)
+```
+
+Encodes a list of coordinates to the corresponding HERE legacy polyline string representation. 
+Expected coordinates order: `(lat, lng[, width])`. Note that `width` is expected to be one of `DW`, `HW`, `CW`.
+
+
+```python
+>>> decode_legacy(legacy_polyline_string)
+```
+
+Decodes a HERE legacy polyline string into an array of coordinates `(lat, lng[, width])`.
+
+
+Note that `width` is expected to be one of `DW`, `HW`, `CW`.
+
+#### Examples
+
+```python
+>>> import here_search.polyline_converter as pc
+>>> legacy_polyline = "oz5xJ67i1B1B7PzIhaxL7Y"
+>>> flexible_polyline = pc.convert_legacy_to_flex(legacy_polyline)
+>>> flexible_polyline
+'BFoz5xJ67i1B1B7PzIhaxL7Y'
+
+>>> points = [(50.1022829, 8.6982122), (50.1020076, 8.6956695), (50.1006313, 8.6914960), (50.0987800, 8.6875156)]
+>>> pc.encode_legacy(points)
+'oz5xJ67i1B1B7PzIhaxL7Y'
+
+>>> legacy_polyline = "oz5xJ67i1B.C1B7PzIha.DxL7Y"
+>>> pc.decode_legacy(legacy_polyline)
+[(50.10228, 8.69821, 'CW'), (50.10201, 8.69567), (50.10063, 8.6915, 'DW'), (50.09878, 8.68752)]
+```
+
+## License
+
+Copyright (C) 2023 HERE Europe B.V.
+
+See the [LICENSE](./LICENSE) file in the root of this project for license details.
+
+[1]: https://github.com/heremaps/flexible-polyline
+[2]: https://developer.here.com/documentation/places/dev_guide/topics/guide.html
+[3]: https://developer.here.com/documentation/geocoding-search-api/dev_guide/index.html
+[4]: https://developer.here.com/documentation/places/dev_guide/topics/location-contexts.html#location-contexts__here-polyline-encoding
+[b]: https://github.com/heremaps/here-polyline-converter/actions/workflows/test.yml/badge.svg
+[c1]: https://codecov.io/gh/heremaps/here-polyline-converter/branch/main/graph/badge.svg?token=9LPI9T7BMN
+[c2]: https://codecov.io/gh/heremaps/here-polyline-converter
```

### Comparing `here-polyline-converter-0.2.0/src/here_polyline_converter.egg-info/SOURCES.txt` & `here-polyline-converter-0.2.1/src/here_polyline_converter.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -9,8 +9,9 @@
 src/here_polyline_converter.egg-info/SOURCES.txt
 src/here_polyline_converter.egg-info/dependency_links.txt
 src/here_polyline_converter.egg-info/not-zip-safe
 src/here_polyline_converter.egg-info/requires.txt
 src/here_polyline_converter.egg-info/top_level.txt
 src/here_search/polyline_converter/__init__.py
 src/here_search/polyline_converter/decoding.py
-src/here_search/polyline_converter/encoding.py
+src/here_search/polyline_converter/encoding.py
+tests/test_converter.py
```

### Comparing `here-polyline-converter-0.2.0/src/here_search/polyline_converter/__init__.py` & `here-polyline-converter-0.2.1/src/here_search/polyline_converter/__init__.py`

 * *Files identical despite different names*

### Comparing `here-polyline-converter-0.2.0/src/here_search/polyline_converter/decoding.py` & `here-polyline-converter-0.2.1/src/here_search/polyline_converter/decoding.py`

 * *Files identical despite different names*

### Comparing `here-polyline-converter-0.2.0/src/here_search/polyline_converter/encoding.py` & `here-polyline-converter-0.2.1/src/here_search/polyline_converter/encoding.py`

 * *Files identical despite different names*

