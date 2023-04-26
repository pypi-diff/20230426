# Comparing `tmp/flytekitplugins-deck-standard-1.6.0a1.tar.gz` & `tmp/flytekitplugins-deck-standard-1.6.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-deck-standard-1.6.0a1.tar", last modified: Wed Apr 26 20:37:24 2023, max compression
+gzip compressed data, was "flytekitplugins-deck-standard-1.6.0b0.tar", last modified: Wed Apr 19 20:54:28 2023, max compression
```

## Comparing `flytekitplugins-deck-standard-1.6.0a1.tar` & `flytekitplugins-deck-standard-1.6.0b0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:37:24.265398 flytekitplugins-deck-standard-1.6.0a1/
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-26 20:37:24.265398 flytekitplugins-deck-standard-1.6.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-26 20:36:40.000000 flytekitplugins-deck-standard-1.6.0a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:37:24.261398 flytekitplugins-deck-standard-1.6.0a1/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:37:24.261398 flytekitplugins-deck-standard-1.6.0a1/flytekitplugins/deck/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-26 20:36:40.000000 flytekitplugins-deck-standard-1.6.0a1/flytekitplugins/deck/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-04-26 20:36:40.000000 flytekitplugins-deck-standard-1.6.0a1/flytekitplugins/deck/renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:37:24.265398 flytekitplugins-deck-standard-1.6.0a1/flytekitplugins_deck_standard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-26 20:37:24.000000 flytekitplugins-deck-standard-1.6.0a1/flytekitplugins_deck_standard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-26 20:37:24.000000 flytekitplugins-deck-standard-1.6.0a1/flytekitplugins_deck_standard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 20:37:24.000000 flytekitplugins-deck-standard-1.6.0a1/flytekitplugins_deck_standard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-26 20:37:24.000000 flytekitplugins-deck-standard-1.6.0a1/flytekitplugins_deck_standard.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-26 20:37:24.000000 flytekitplugins-deck-standard-1.6.0a1/flytekitplugins_deck_standard.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-26 20:37:24.000000 flytekitplugins-deck-standard-1.6.0a1/flytekitplugins_deck_standard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-26 20:37:24.000000 flytekitplugins-deck-standard-1.6.0a1/flytekitplugins_deck_standard.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 20:37:24.265398 flytekitplugins-deck-standard-1.6.0a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-04-26 20:37:20.000000 flytekitplugins-deck-standard-1.6.0a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:28.263054 flytekitplugins-deck-standard-1.6.0b0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-19 20:54:28.263054 flytekitplugins-deck-standard-1.6.0b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-19 20:54:06.000000 flytekitplugins-deck-standard-1.6.0b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:28.263054 flytekitplugins-deck-standard-1.6.0b0/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:28.263054 flytekitplugins-deck-standard-1.6.0b0/flytekitplugins/deck/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-19 20:54:06.000000 flytekitplugins-deck-standard-1.6.0b0/flytekitplugins/deck/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-04-19 20:54:06.000000 flytekitplugins-deck-standard-1.6.0b0/flytekitplugins/deck/renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:28.263054 flytekitplugins-deck-standard-1.6.0b0/flytekitplugins_deck_standard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-19 20:54:28.000000 flytekitplugins-deck-standard-1.6.0b0/flytekitplugins_deck_standard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-19 20:54:28.000000 flytekitplugins-deck-standard-1.6.0b0/flytekitplugins_deck_standard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 20:54:28.000000 flytekitplugins-deck-standard-1.6.0b0/flytekitplugins_deck_standard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-19 20:54:28.000000 flytekitplugins-deck-standard-1.6.0b0/flytekitplugins_deck_standard.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-19 20:54:28.000000 flytekitplugins-deck-standard-1.6.0b0/flytekitplugins_deck_standard.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-19 20:54:28.000000 flytekitplugins-deck-standard-1.6.0b0/flytekitplugins_deck_standard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-19 20:54:28.000000 flytekitplugins-deck-standard-1.6.0b0/flytekitplugins_deck_standard.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 20:54:28.267054 flytekitplugins-deck-standard-1.6.0b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-04-19 20:54:25.000000 flytekitplugins-deck-standard-1.6.0b0/setup.py
```

### Comparing `flytekitplugins-deck-standard-1.6.0a1/PKG-INFO` & `flytekitplugins-deck-standard-1.6.0b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-deck-standard
-Version: 1.6.0a1
+Version: 1.6.0b0
 Summary: This Plugin provides more renderers to improve task visibility
 Home-page: https://github.com/flyteorg/flytekit/tree/master/plugins/flytekit-data-fsspec
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `flytekitplugins-deck-standard-1.6.0a1/flytekitplugins/deck/renderer.py` & `flytekitplugins-deck-standard-1.6.0b0/flytekitplugins/deck/renderer.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,23 @@
-import base64
-from io import BytesIO
-from typing import Union
-
 import markdown
-import pandas as pd
+import pandas
 import plotly.express as px
-from PIL import Image
 from ydata_profiling import ProfileReport
 
-from flytekit.types.file import FlyteFile
-
 
 class FrameProfilingRenderer:
     """
     Generate a ProfileReport based on a pandas DataFrame
     """
 
     def __init__(self, title: str = "Pandas Profiling Report"):
         self._title = title
 
-    def to_html(self, df: pd.DataFrame) -> str:
-        assert isinstance(df, pd.DataFrame)
+    def to_html(self, df: pandas.DataFrame) -> str:
+        assert isinstance(df, pandas.DataFrame)
         profile = ProfileReport(df, title=self._title)
         return profile.to_html()
 
 
 class MarkdownRenderer:
     """Convert a markdown string to HTML and return HTML as a unicode string.
 
@@ -48,37 +41,10 @@
     range (IQR: Q3-Q1), see "points" for other options.
     """
 
     # More detail, see https://plotly.com/python/box-plots/
     def __init__(self, column_name):
         self._column_name = column_name
 
-    def to_html(self, df: pd.DataFrame) -> str:
+    def to_html(self, df: pandas.DataFrame) -> str:
         fig = px.box(df, y=self._column_name)
         return fig.to_html()
-
-
-class ImageRenderer:
-    """Converts a FlyteFile or PIL.Image.Image object to an HTML string with the image data
-    represented as a base64-encoded string.
-    """
-
-    def to_html(cls, image_src: Union[FlyteFile, Image.Image]) -> str:
-        img = cls._get_image_object(image_src)
-        return cls._image_to_html_string(img)
-
-    @staticmethod
-    def _get_image_object(image_src: Union[FlyteFile, Image.Image]) -> Image.Image:
-        if isinstance(image_src, FlyteFile):
-            local_path = image_src.download()
-            return Image.open(local_path)
-        elif isinstance(image_src, Image.Image):
-            return image_src
-        else:
-            raise ValueError("Unsupported image source type")
-
-    @staticmethod
-    def _image_to_html_string(img: Image.Image) -> str:
-        buffered = BytesIO()
-        img.save(buffered, format="PNG")
-        img_base64 = base64.b64encode(buffered.getvalue()).decode()
-        return f'<img src="data:image/png;base64,{img_base64}" alt="Rendered Image" />'
```

### Comparing `flytekitplugins-deck-standard-1.6.0a1/flytekitplugins_deck_standard.egg-info/PKG-INFO` & `flytekitplugins-deck-standard-1.6.0b0/flytekitplugins_deck_standard.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-deck-standard
-Version: 1.6.0a1
+Version: 1.6.0b0
 Summary: This Plugin provides more renderers to improve task visibility
 Home-page: https://github.com/flyteorg/flytekit/tree/master/plugins/flytekit-data-fsspec
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `flytekitplugins-deck-standard-1.6.0a1/setup.py` & `flytekitplugins-deck-standard-1.6.0b0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "deck"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}-standard"
 
 plugin_requires = ["flytekit>=1.3.0b2,<2.0.0", "markdown", "plotly", "ydata-profiling", "ipywidgets"]
 
-__version__ = "1.6.0a1"
+__version__ = "1.6.0b0"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="This Plugin provides more renderers to improve task visibility",
```

