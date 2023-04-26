# Comparing `tmp/thisnotthat-0.2.1.tar.gz` & `tmp/thisnotthat-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thisnotthat-0.2.1.tar", last modified: Fri Nov 25 16:27:25 2022, max compression
+gzip compressed data, was "thisnotthat-0.3.tar", last modified: Wed Apr 26 12:53:19 2023, max compression
```

## Comparing `thisnotthat-0.2.1.tar` & `thisnotthat-0.3.tar`

### file list

```diff
@@ -1,29 +1,34 @@
-drwxr-xr-x   0 hamelin   (1001) hamelin   (1001)        0 2022-11-25 16:27:25.059006 thisnotthat-0.2.1/
--rw-r--r--   0 hamelin   (1001) hamelin   (1001)     1533 2022-11-25 16:03:13.000000 thisnotthat-0.2.1/LICENSE
--rw-r--r--   0 hamelin   (1001) hamelin   (1001)     4343 2022-11-25 16:27:25.059006 thisnotthat-0.2.1/PKG-INFO
--rw-r--r--   0 hamelin   (1001) hamelin   (1001)     3288 2022-11-25 16:03:13.000000 thisnotthat-0.2.1/README.rst
--rw-r--r--   0 hamelin   (1001) hamelin   (1001)       38 2022-11-25 16:27:25.059006 thisnotthat-0.2.1/setup.cfg
--rw-r--r--   0 hamelin   (1001) hamelin   (1001)     2320 2022-11-25 16:27:12.000000 thisnotthat-0.2.1/setup.py
-drwxr-xr-x   0 hamelin   (1001) hamelin   (1001)        0 2022-11-25 16:27:25.059006 thisnotthat-0.2.1/thisnotthat/
--rw-r--r--   0 hamelin   (1001) hamelin   (1001)      723 2022-11-25 16:03:13.000000 thisnotthat-0.2.1/thisnotthat/__init__.py
--rw-r-----   0 hamelin   (1001) hamelin   (1001)       22 2022-11-25 16:25:43.000000 thisnotthat-0.2.1/thisnotthat/_version.py
--rw-r--r--   0 hamelin   (1001) hamelin   (1001)    34518 2022-11-25 16:03:13.000000 thisnotthat-0.2.1/thisnotthat/bokeh_plot.py
--rw-r--r--   0 hamelin   (1001) hamelin   (1001)    12524 2022-11-25 16:03:13.000000 thisnotthat-0.2.1/thisnotthat/data_viewer.py
--rw-r--r--   0 hamelin   (1001) hamelin   (1001)    20778 2022-11-25 16:03:13.000000 thisnotthat-0.2.1/thisnotthat/deckgl_plot.py
--rw-r--r--   0 hamelin   (1001) hamelin   (1001)     4557 2022-11-25 16:03:13.000000 thisnotthat-0.2.1/thisnotthat/instance_viewer.py
--rw-r--r--   0 hamelin   (1001) hamelin   (1001)    21125 2022-11-25 16:03:13.000000 thisnotthat-0.2.1/thisnotthat/label_editor.py
--rw-r--r--   0 hamelin   (1001) hamelin   (1001)    58925 2022-11-25 16:03:13.000000 thisnotthat-0.2.1/thisnotthat/map_cluster_labelling.py
--rw-r--r--   0 hamelin   (1001) hamelin   (1001)     4371 2022-11-25 16:03:13.000000 thisnotthat-0.2.1/thisnotthat/palettes.py
--rw-r--r--   0 hamelin   (1001) hamelin   (1001)    13751 2022-11-25 16:03:13.000000 thisnotthat-0.2.1/thisnotthat/plot_controls.py
--rw-r--r--   0 hamelin   (1001) hamelin   (1001)    11712 2022-11-25 16:03:13.000000 thisnotthat-0.2.1/thisnotthat/search.py
-drwxr-xr-x   0 hamelin   (1001) hamelin   (1001)        0 2022-11-25 16:27:25.059006 thisnotthat-0.2.1/thisnotthat/tests/
--rw-r--r--   0 hamelin   (1001) hamelin   (1001)        0 2022-11-25 16:03:13.000000 thisnotthat-0.2.1/thisnotthat/tests/__init__.py
--rw-r--r--   0 hamelin   (1001) hamelin   (1001)      316 2022-11-25 16:03:13.000000 thisnotthat-0.2.1/thisnotthat/tests/test_cluster_labelling.py
--rw-r--r--   0 hamelin   (1001) hamelin   (1001)      533 2022-11-25 16:03:13.000000 thisnotthat-0.2.1/thisnotthat/utils.py
-drwxr-xr-x   0 hamelin   (1001) hamelin   (1001)        0 2022-11-25 16:27:25.059006 thisnotthat-0.2.1/thisnotthat.egg-info/
--rw-rw-r--   0 hamelin   (1001) hamelin   (1001)     4343 2022-11-25 16:27:25.000000 thisnotthat-0.2.1/thisnotthat.egg-info/PKG-INFO
--rw-rw-r--   0 hamelin   (1001) hamelin   (1001)      629 2022-11-25 16:27:25.000000 thisnotthat-0.2.1/thisnotthat.egg-info/SOURCES.txt
--rw-rw-r--   0 hamelin   (1001) hamelin   (1001)        1 2022-11-25 16:27:25.000000 thisnotthat-0.2.1/thisnotthat.egg-info/dependency_links.txt
--rw-r--r--   0 hamelin   (1001) hamelin   (1001)        1 2022-11-25 16:27:24.000000 thisnotthat-0.2.1/thisnotthat.egg-info/not-zip-safe
--rw-rw-r--   0 hamelin   (1001) hamelin   (1001)      208 2022-11-25 16:27:25.000000 thisnotthat-0.2.1/thisnotthat.egg-info/requires.txt
--rw-rw-r--   0 hamelin   (1001) hamelin   (1001)       12 2022-11-25 16:27:25.000000 thisnotthat-0.2.1/thisnotthat.egg-info/top_level.txt
+drwxr-xr-x   0 hamelin   (1011) hamelin   (1011)        0 2023-04-26 12:53:19.228144 thisnotthat-0.3/
+-rw-r--r--   0 hamelin   (1011) hamelin   (1011)     1533 2022-11-25 16:03:13.000000 thisnotthat-0.3/LICENSE
+-rw-r--r--   0 hamelin   (1011) hamelin   (1011)     4393 2023-04-26 12:53:19.228144 thisnotthat-0.3/PKG-INFO
+-rw-r--r--   0 hamelin   (1011) hamelin   (1011)     3440 2023-04-26 12:34:50.000000 thisnotthat-0.3/README.rst
+-rw-r--r--   0 hamelin   (1011) hamelin   (1011)       38 2023-04-26 12:53:19.228144 thisnotthat-0.3/setup.cfg
+-rw-r--r--   0 hamelin   (1011) hamelin   (1011)     2245 2023-04-26 12:34:50.000000 thisnotthat-0.3/setup.py
+drwxr-xr-x   0 hamelin   (1011) hamelin   (1011)        0 2023-04-26 12:53:19.228144 thisnotthat-0.3/thisnotthat/
+-rw-r--r--   0 hamelin   (1011) hamelin   (1011)     1176 2023-04-26 12:34:50.000000 thisnotthat-0.3/thisnotthat/__init__.py
+-rw-r--r--   0 hamelin   (1011) hamelin   (1011)       20 2023-04-26 12:51:17.000000 thisnotthat-0.3/thisnotthat/_version.py
+-rw-r--r--   0 hamelin   (1011) hamelin   (1011)    36695 2023-04-26 12:34:50.000000 thisnotthat-0.3/thisnotthat/bokeh_plot.py
+-rw-r--r--   0 hamelin   (1011) hamelin   (1011)    12524 2022-11-25 16:03:13.000000 thisnotthat-0.3/thisnotthat/data_viewer.py
+-rw-r--r--   0 hamelin   (1011) hamelin   (1011)    20778 2023-04-26 12:34:50.000000 thisnotthat-0.3/thisnotthat/deckgl_plot.py
+-rw-r--r--   0 hamelin   (1011) hamelin   (1011)      653 2023-04-26 12:34:50.000000 thisnotthat-0.3/thisnotthat/image_utils.py
+-rw-r--r--   0 hamelin   (1011) hamelin   (1011)     4951 2023-04-26 12:34:50.000000 thisnotthat-0.3/thisnotthat/instance_viewer.py
+-rw-r--r--   0 hamelin   (1011) hamelin   (1011)    19961 2023-04-26 12:34:50.000000 thisnotthat-0.3/thisnotthat/label_editor.py
+-rw-r--r--   0 hamelin   (1011) hamelin   (1011)    68608 2023-02-16 16:46:52.000000 thisnotthat-0.3/thisnotthat/map_cluster_labelling.py
+-rw-r--r--   0 hamelin   (1011) hamelin   (1011)     4371 2022-11-25 16:03:13.000000 thisnotthat-0.3/thisnotthat/palettes.py
+-rw-r--r--   0 hamelin   (1011) hamelin   (1011)    13751 2023-04-26 12:34:50.000000 thisnotthat-0.3/thisnotthat/plot_controls.py
+-rw-r--r--   0 hamelin   (1011) hamelin   (1011)    23600 2023-04-26 12:34:50.000000 thisnotthat-0.3/thisnotthat/search.py
+drwxr-xr-x   0 hamelin   (1011) hamelin   (1011)        0 2023-04-26 12:53:19.228144 thisnotthat-0.3/thisnotthat/summary/
+-rw-r--r--   0 hamelin   (1011) hamelin   (1011)        0 2023-04-26 12:34:50.000000 thisnotthat-0.3/thisnotthat/summary/__init__.py
+-rw-r--r--   0 hamelin   (1011) hamelin   (1011)     7806 2023-04-26 12:34:50.000000 thisnotthat-0.3/thisnotthat/summary/dataframe.py
+-rw-r--r--   0 hamelin   (1011) hamelin   (1011)    16916 2023-04-26 12:34:50.000000 thisnotthat-0.3/thisnotthat/summary/plot.py
+drwxr-xr-x   0 hamelin   (1011) hamelin   (1011)        0 2023-04-26 12:53:19.228144 thisnotthat-0.3/thisnotthat/tests/
+-rw-r--r--   0 hamelin   (1011) hamelin   (1011)        0 2022-11-25 16:03:13.000000 thisnotthat-0.3/thisnotthat/tests/__init__.py
+-rw-r--r--   0 hamelin   (1011) hamelin   (1011)      316 2022-11-25 16:03:13.000000 thisnotthat-0.3/thisnotthat/tests/test_cluster_labelling.py
+-rw-r--r--   0 hamelin   (1011) hamelin   (1011)      533 2022-11-25 16:03:13.000000 thisnotthat-0.3/thisnotthat/utils.py
+drwxr-xr-x   0 hamelin   (1011) hamelin   (1011)        0 2023-04-26 12:53:19.228144 thisnotthat-0.3/thisnotthat.egg-info/
+-rw-rw-r--   0 hamelin   (1011) hamelin   (1011)     4393 2023-04-26 12:53:19.000000 thisnotthat-0.3/thisnotthat.egg-info/PKG-INFO
+-rw-rw-r--   0 hamelin   (1011) hamelin   (1011)      749 2023-04-26 12:53:19.000000 thisnotthat-0.3/thisnotthat.egg-info/SOURCES.txt
+-rw-rw-r--   0 hamelin   (1011) hamelin   (1011)        1 2023-04-26 12:53:19.000000 thisnotthat-0.3/thisnotthat.egg-info/dependency_links.txt
+-rw-r--r--   0 hamelin   (1011) hamelin   (1011)        1 2022-11-25 16:27:24.000000 thisnotthat-0.3/thisnotthat.egg-info/not-zip-safe
+-rw-rw-r--   0 hamelin   (1011) hamelin   (1011)      230 2023-04-26 12:53:19.000000 thisnotthat-0.3/thisnotthat.egg-info/requires.txt
+-rw-rw-r--   0 hamelin   (1011) hamelin   (1011)       12 2023-04-26 12:53:19.000000 thisnotthat-0.3/thisnotthat.egg-info/top_level.txt
```

### Comparing `thisnotthat-0.2.1/LICENSE` & `thisnotthat-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `thisnotthat-0.2.1/PKG-INFO` & `thisnotthat-0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 Metadata-Version: 2.1
 Name: thisnotthat
-Version: 0.2.1
+Version: 0.3
 Summary: Tools for interactive visualization and exploration of _data maps_
-Home-page: https://github.com/TutteInstitute/vectorizers
+Home-page: https://github.com/TutteInstitute/thisnotthat
 Download-URL: https://github.com/TutteInstitute/thisnotthat
 Maintainer: Benoit Hamelin, John Healy, Leland McInnes
 Maintainer-email: leland.mcinnes@gmail.com
 License: new BSD
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: tests
 Provides-Extra: docs
 License-File: LICENSE
 
 .. -*- mode: rst -*-
@@ -63,14 +61,20 @@
 -------------------------------
 This Not That for Data Map Apps
 -------------------------------
 
 Because This Not That is built on top of the `Panel library`_ it is trivial to deploy TNT based solutions as
 interactive web applications.
 
+-------------
+Documentation
+-------------
+
+Get the latest on `Read The Docs <https://thisnotthat.readthedocs.io/en/latest/>`_.
+
 ----------
 Installing
 ----------
 
 This Not That is built on top of Panel and Bokeh, so you will need these installed. In all you will need:
 
 * panel
@@ -78,14 +82,16 @@
 * numpy >= 1.22
 * pandas
 * scikit-learn
 * matplotlib
 * umap-learn
 * hdbscan
 * glasbey
+* cmocean
+* vectorizers
 
 We also highly recommend installing:
 
 * networkx
 * apricot-select
 
 Currently you can pip install directly from this repository:
@@ -111,14 +117,14 @@
 submit a pull request. We will do our best to work through any issues with
 you and get your code merged into the main branch.
 
 -------
 License
 -------
 
-The This Not That package is 2-clause BSD licensed.
+The This Not That package is 3-clause BSD licensed.
 
 
 .. _Panel library: https://panel.holoviz.org/
```

### Comparing `thisnotthat-0.2.1/README.rst` & `thisnotthat-0.3/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -36,14 +36,20 @@
 -------------------------------
 This Not That for Data Map Apps
 -------------------------------
 
 Because This Not That is built on top of the `Panel library`_ it is trivial to deploy TNT based solutions as
 interactive web applications.
 
+-------------
+Documentation
+-------------
+
+Get the latest on `Read The Docs <https://thisnotthat.readthedocs.io/en/latest/>`_.
+
 ----------
 Installing
 ----------
 
 This Not That is built on top of Panel and Bokeh, so you will need these installed. In all you will need:
 
 * panel
@@ -51,14 +57,16 @@
 * numpy >= 1.22
 * pandas
 * scikit-learn
 * matplotlib
 * umap-learn
 * hdbscan
 * glasbey
+* cmocean
+* vectorizers
 
 We also highly recommend installing:
 
 * networkx
 * apricot-select
 
 Currently you can pip install directly from this repository:
@@ -84,14 +92,14 @@
 submit a pull request. We will do our best to work through any issues with
 you and get your code merged into the main branch.
 
 -------
 License
 -------
 
-The This Not That package is 2-clause BSD licensed.
+The This Not That package is 3-clause BSD licensed.
 
 
 .. _Panel library: https://panel.holoviz.org/
```

### Comparing `thisnotthat-0.2.1/setup.py` & `thisnotthat-0.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 DISTNAME = 'thisnotthat'
 DESCRIPTION = 'Tools for interactive visualization and exploration of _data maps_'
 with codecs.open('README.rst', encoding='utf-8-sig') as f:
     LONG_DESCRIPTION = f.read()
 MAINTAINER = 'Benoit Hamelin, John Healy, Leland McInnes'
 MAINTAINER_EMAIL = 'leland.mcinnes@gmail.com'
-URL = 'https://github.com/TutteInstitute/vectorizers'
+URL = 'https://github.com/TutteInstitute/thisnotthat'
 LICENSE = 'new BSD'
 DOWNLOAD_URL = 'https://github.com/TutteInstitute/thisnotthat'
 VERSION = __version__
 INSTALL_REQUIRES = [
     "bokeh",
     "cmocean",
     "colorcet",
@@ -26,28 +26,28 @@
     "hdbscan",
     "matplotlib",
     "numpy>=1.22",
     "pandas",
     "panel",
     "param",
     "scikit-learn",
-    "umap-learn"
+    "umap-learn",
+    "vectorizers",
+    "wordcloud",
 ]
 CLASSIFIERS = ['Intended Audience :: Science/Research',
                'Intended Audience :: Developers',
                'License :: OSI Approved',
                'Programming Language :: Python',
                'Topic :: Software Development',
                'Topic :: Scientific/Engineering',
                'Operating System :: Microsoft :: Windows',
                'Operating System :: POSIX',
                'Operating System :: Unix',
                'Operating System :: MacOS',
-               'Programming Language :: Python :: 3.7',
-               'Programming Language :: Python :: 3.8',
                'Programming Language :: Python :: 3.9',
                'Programming Language :: Python :: 3.10'
                ]
 EXTRAS_REQUIRE = {
     'tests': [
         'pytest',
         'pytest-cov'],
```

### Comparing `thisnotthat-0.2.1/thisnotthat/bokeh_plot.py` & `thisnotthat-0.3/thisnotthat/bokeh_plot.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,14 +26,17 @@
     text_dataframe: pd.DataFrame,
     text_size: float,
     layer_type: str = "middle",
     *,
     angle: float = 0,
     text_color: str = "#444444",
     text_outline_color: str = "#dddddd",
+    background_fill_color: str = "#eeeeee22",
+    padding: int = 0,
+    border_radius: int = 5,
     text_font: Dict[str, str] = {"value": "helvetica"},
     text_font_style: str = "normal",
     text_line_height: float = 0.9,
     text_alpha: float = 1.0,
     max_text_size: float = 64.0,
     min_text_size: float = 2.0,
     text_transition_width: float = 16.0,
@@ -92,14 +95,17 @@
         labels = bokeh.models.Text(
             text_font_size=str(text_size) + "pt",
             text_baseline="bottom",
             text_align="center",
             angle=angle,
             text_color=text_color,
             text_outline_color=text_outline_color,
+            background_fill_color=background_fill_color,
+            padding=padding,
+            border_radius=border_radius,
             text_font=text_font,
             text_font_style=text_font_style,
             text_line_height=text_line_height,
             text_alpha=text_alpha,
         )
     except AttributeError:
         labels = bokeh.models.Text(
@@ -112,31 +118,33 @@
             text_font_style=text_font_style,
             text_line_height=text_line_height,
             text_alpha=text_alpha,
         )
     upper_transition_val = max_text_size - text_transition_width
     lower_transition_val = min_text_size + text_transition_width
     text_resize_callback = bokeh.models.callbacks.CustomJS(
-        args=dict(labels=labels),
+        args=dict(labels=labels, background_fill_color=background_fill_color),
         code="""
     const scale = cb_obj.end - cb_obj.start;
     const text_size = (%f / scale);
     if (text_size > %f && %s) {
         var alpha = (%f - text_size) / %f;
 
     } else if (text_size < %f && %s) {
         var alpha = (text_size - %f) / %f;
 
     } else {
         var alpha = 1.0;
     }
     if (alpha > 0) {
         labels.text_alpha = alpha;
+        labels.background_fill_color = background_fill_color;
     } else {
         labels.text_alpha = 0.0;
+        labels.background_fill_color = "#ffffff00";
     }
     labels.text_font_size = text_size + "pt";
     labels.change.emit();
     """
         % (
             text_size,
             upper_transition_val,
@@ -239,20 +247,38 @@
     tooltip_template: str (optional, default = "<div>@hover_text</div>"
         The template used to define the hover tooltip in the scatterplot. See custom tooltips in the bokeh documentation
         for more details on this.
 
     selection_fill_alpha: float (optional, default = 1.0)
         The alpha value to use for selected points in the scatterplot.
 
+    selection_line_color: str (optional, default = "black")
+        The line colour of selected points in the scatterplot.
+
+    selection_line_width: float (optional, default = 0.5)
+        The line width of selected points in the scatterplot.
+
+    selection_line_alpha: float (optional, default = 0.5)
+        The line alpha of selected points in the scatterplot.
+
     nonselection_fill_alpha: float (optional, default = 0.1)
         The alpha value to use for points that are not in an active selection in the scatterplot.
 
     nonselection_fill_color: str (optional, default = "gray")
         The colour to use to fill points that are not in an active selection in the scatterplot.
 
+    nonselection_line_color: str (optional, default = None)
+        The outline color to use for points that are not in an active selection in the scatterplot.
+
+    nonselection_line_width: float (optional, default = 0.0)
+        The outline line weight for points that are not in an active selection in the scatterplot.
+
+    nonselection_line_alpha: float (optional, default = 0.0)
+        The outline alpha for points that are not in an active selection in the scatterplot.
+
     background_fill_color: str (optional, default = "#FFFFFF")
         The colour to use for the background of the scatterplot.
 
     border_fill_color: str (optional, default = "whitesmoke")
         The colour to use for the background of the non-plot region of the bokeh figure.
 
     toolbar_location: str (optional, default = "above")
@@ -326,24 +352,31 @@
         line_color: str = "white",
         line_width: float = 0.25,
         hover_fill_color: str = "red",
         hover_line_color: str = "black",
         hover_line_width: float = 2,
         tooltip_template: str = """<div>@hover_text</div>""",
         selection_fill_alpha: float = 1.0,
+        selection_line_color: str = "label",
+        selection_line_width: float = 0.5,
+        selection_line_alpha: float = 0.5,
         nonselection_fill_alpha: float = 0.1,
         nonselection_fill_color: str = "gray",
+        nonselection_line_color: Optional[str] = None,
+        nonselection_line_width: float = 0.0,
+        nonselection_line_alpha: float = 0.0,
         background_fill_color: str = "#ffffff",
         border_fill_color: str = "whitesmoke",
         toolbar_location: str = "above",
         tools="pan,wheel_zoom,lasso_select,save,reset,help",
         title: Optional[str] = None,
         title_location: str = "above",
         show_legend: bool = True,
         legend_location: str = "outside",
+        sizing_mode="fixed",
         name: str = "Plot",
     ):
         super().__init__(name=name)
         if labels is None:
             labels = ["unlabelled"] * len(data)
         if type(marker_size) in (int, float):
             marker_size = np.full(len(data), marker_size, dtype=np.float64)
@@ -414,14 +447,15 @@
             output_backend="webgl",
             background_fill_color=background_fill_color,
             border_fill_color=border_fill_color,
             toolbar_location=toolbar_location,
             tools=tools,
             title=title,
             title_location=title_location,
+            sizing_mode=sizing_mode,
         )
         self.plot.toolbar.active_scroll = self.plot.select_one(
             bokeh.models.WheelZoomTool
         )
 
         self.points = self.plot.circle(
             source=self.data_source,
@@ -430,16 +464,22 @@
             fill_alpha=fill_alpha,
             line_color=line_color,
             line_width=line_width,
             hover_fill_color=hover_fill_color,
             hover_line_color=hover_line_color,
             hover_line_width=hover_line_width,
             selection_fill_alpha=selection_fill_alpha,
+            selection_line_color=selection_line_color,
+            selection_line_width=selection_line_width,
+            selection_line_alpha=selection_line_alpha,
             nonselection_fill_alpha=nonselection_fill_alpha,
             nonselection_fill_color=nonselection_fill_color,
+            nonselection_line_color=nonselection_line_color,
+            nonselection_line_width=nonselection_line_width,
+            nonselection_line_alpha=nonselection_line_alpha,
         )
         if show_legend:
             self._legend = bokeh.models.Legend(
                 items=[
                     bokeh.models.LegendItem(
                         label={"field": "label"}, renderers=[self.points]
                     )
@@ -503,15 +543,15 @@
         self.plot.add_tools(
             bokeh.models.HoverTool(tooltips=tooltip_template, renderers=[self.points])
         )
         self.plot.xgrid.grid_line_color = None
         self.plot.ygrid.grid_line_color = None
         self.plot.xaxis.bounds = (0, 0)
         self.plot.yaxis.bounds = (0, 0)
-        self.pane = pn.pane.Bokeh(self.plot)
+        self.pane = pn.pane.Bokeh(self.plot, sizing_mode=sizing_mode)
 
         self.show_legend = show_legend
         self.color_by_vector = pd.Series([], dtype=object)
         self.labels = pd.Series(labels).copy()  # .reset_index(drop=True)
         self.label_color_palette = list(self.color_mapping.palette)
         self.label_color_factors = list(self.color_mapping.factors)
         self.color_by_palette = list(self.color_mapping.palette)
@@ -714,14 +754,17 @@
         text_layer_scale_factor: float = 2.0,
         text_color: str = "#444444",
         text_outline_color: str = "#dddddd",
         text_font: Dict[str, str] = {"value": "helvetica"},
         text_font_style: str = "normal",
         text_line_height: float = 0.9,
         text_alpha: float = 1.0,
+        background_fill_color: str = "#eeeeee22",
+        padding = 0,
+        border_radius=5,
         max_text_size: float = 64.0,
         min_text_size: float = 2.0,
         text_transition_width: float = 16.0,
     ):
         """Given a cluster labelling generated via one of the methods in the ``map_cluster_labelling``
         module, add the labelling information to this plot in a manner that allows lower level, more detailed,
         labels to be revealed upon zooming in, with transitions between the layers, and appropriate sizing
@@ -788,14 +831,17 @@
                 self.plot,
                 cluster_label_layer,
                 text_size_scale * text_layer_scale_factor ** i,
                 layer_type=layer_type,
                 angle=angle,
                 text_color=text_color,
                 text_outline_color=text_outline_color,
+                background_fill_color=background_fill_color,
+                padding=padding,
+                border_radius=border_radius,
                 text_font=text_font,
                 text_font_style=text_font_style,
                 text_line_height=text_line_height,
                 text_alpha=text_alpha,
                 max_text_size=max_text_size,
                 min_text_size=min_text_size,
                 text_transition_width=text_transition_width,
```

### Comparing `thisnotthat-0.2.1/thisnotthat/data_viewer.py` & `thisnotthat-0.3/thisnotthat/data_viewer.py`

 * *Files identical despite different names*

### Comparing `thisnotthat-0.2.1/thisnotthat/deckgl_plot.py` & `thisnotthat-0.3/thisnotthat/deckgl_plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,15 +175,15 @@
                 height=32,
                 style={
                     "font-weight": "bold",
                     "line-height": "32px",
                     "height": "64px",
                     "text-align": "right",
                 },
-                margin=[5, 0],
+                margin=(5, 0),
             ),
             self.select_method,
         )
         self.select_method.param.watch(
             self._change_selection_type, "value", onlychanged=True
         )
         self.select_message = pn.pane.Alert(
@@ -203,15 +203,15 @@
             style={
                 "font-weight": "bold",
                 "font-size": "32px",
                 "line-height": "32px",
                 "height": "64px",
                 "text-align": "left",
             },
-            margin=[5, 0],
+            margin=(5, 0),
         )
         self.points["data"] = self.dataframe
         self.deck_pane.param.trigger("object")
         self.deck_pane.param.watch(
             self._click_event_handler, "click_state", onlychanged=True
         )
         self.deck_pane.param.watch(self._hover_event_handler, "hover_state")
```

### Comparing `thisnotthat-0.2.1/thisnotthat/instance_viewer.py` & `thisnotthat-0.3/thisnotthat/instance_viewer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import panel as pn
 import param
 import pandas as pd
+import time
 
 from typing import *
 
 
 class InformationPane(pn.reactive.Reactive):
     """An information pane allowing you to provide more details in a well formatted way on a single specific
     selected instance of data. The goal is similar to the ``DataPane`` -- to allow a user to go from points in the map 
@@ -20,15 +21,15 @@
     ----------
     raw_dataframe: DataFrame
         The dataframe to associate with data in a map representation in a PlotPane. The dataframe should have one row
         per sample in the map representation, and be in the same order as the data in the map representation.
 
     markdown_template: str
         A string in markdown providing formatting for a single row of data from the dataframe. Within the string
-        a substitution of the row value of of a column will be done where ``{column_name}`` appears in the string.
+        a substitution of the row value of a column will be done where ``{column_name}`` appears in the string.
 
     width: int (optional, default = 200)
         The width of the pane.
 
     height: int (optional, default = 600)
         The height of the pane.
 
@@ -65,53 +66,60 @@
         width: int = 200,
         height: int = 600,
         placeholder_text: str = "<center> ... nothing selected ...",
         dedent: bool = False,
         disable_math: bool = False,
         extensions: List[str] = ["extra", "smarty", "codehilite"],
         style: dict = {},
-        margin: List[int] = [5, 5],
+        margin: Tuple[int] = (5, 5),
+        sizing_mode: str = "stretch_height",
+        throttle = 200,
         name: str = "Information",
     ):
         super().__init__(name=name)
         self.data = raw_dataframe
         self.markdown_template = markdown_template
         self.placeholder_text = placeholder_text
+        self.throttle = throttle
+        self._last_update = time.perf_counter() * 1000.0
         self.markdown = pn.pane.Markdown(
             self.placeholder_text,
             width=width - 20,
             height=height - 20,
             margin=margin,
             dedent=dedent,
             disable_math=disable_math,
             extensions=extensions,
+            sizing_mode=sizing_mode,
             style=style,
         )
-        self.pane = pn.Column(self.markdown, width=width, height=height, scroll=True)
+        self.pane = pn.Column(self.markdown, width=width, height=height, sizing_mode=sizing_mode, scroll=True)
 
     def _get_model(self, *args, **kwds):
         return self.pane._get_model(*args, **kwds)
 
     @param.depends("selected", watch=True)
     def _info_pane_update_selection(self) -> None:
         if len(self.selected) == 0:
             self.markdown.object = self.placeholder_text
         else:
-            substitution_dict = {
-                col: self.data[col].iloc[self.selected[-1]] for col in self.data.columns
-            }
-            self.markdown.object = self.markdown_template.format(**substitution_dict)
+            if time.perf_counter() * 1000.0 - self._last_update > self.throttle:
+                substitution_dict = {
+                    col: self.data[col].iloc[self.selected[-1]] for col in self.data.columns
+                }
+                self.markdown.object = self.markdown_template.format(**substitution_dict)
+                self._last_update = time.perf_counter() * 1000.0
 
     def link_to_plot(self, plot):
         """Link this pane to a plot pane using a default set of params that can sensibly be linked.
 
         Parameters
         ----------
         plot: PlotPane
             The plot pane to link to.
 
         Returns
         -------
         link:
             The link object.
         """
-        return self.link(plot, selected="selected", bidirectional=True)
+        return plot.link(self, selected="selected", bidirectional=False)
```

### Comparing `thisnotthat-0.2.1/thisnotthat/label_editor.py` & `thisnotthat-0.3/thisnotthat/label_editor.py`

 * *Files 3% similar despite different names*

```diff
@@ -115,15 +115,15 @@
 
         if palette is None:
             self.label_color_palette = get_palette("glasbey_category10", length=palette_length, scrambled=palette_shuffle)
         elif type(palette) is str:
             self.label_color_palette = get_palette(palette, length=palette_length, scrambled=palette_shuffle)
         else:
             if palette_length > len(palette):
-                self.label_color_palette = extend_palette(palette, palette_length=palette_length)
+                self.label_color_palette = extend_palette(palette, palette_size=palette_length)
             else:
                 self.label_color_palette = palette[:palette_length]
 
             if palette_shuffle:
                 self.label_color_palette = [self.label_color_palette[x] for x in _palette_index(len(self.label_color_palette))]
 
 
@@ -133,15 +133,18 @@
         self.color_picker_height = color_picker_height
         self.color_picker_margin = color_picker_margin
         self.label_width = label_width
         self.label_height = label_height
         self.label_max_width = label_max_width
         self.label_min_width = label_min_width
         self.label_margin = label_margin
-        self.pane = pn.Column()
+
+        self._internal_selection = False
+
+        self.pane = pn.Column(sizing_mode="stretch_height")
         self._rebuild_pane()
 
     def _color_callback(self, event: param.parameterized.Event) -> None:
         self.label_color_palette = [
             event.new if color == event.old else color
             for color in self.label_color_palette
         ]
@@ -223,15 +226,15 @@
                         min_width=self.label_min_width,
                     ),
                     pn.widgets.Button(
                         name="",
                         button_type="default",
                         width=self.label_height,
                         height=self.label_height,
-                        margin=[0, 2],
+                        margin=(0, 2),
                     ),
                 )
                 legend_items.append(legend_item)
                 legend_item[0].param.watch(
                     self._color_callback, "value", onlychanged=True
                 )
                 legend_item[1].param.watch(
@@ -255,77 +258,33 @@
         self.label_color_factors = self.label_color_factors + list(
             new_label_set - set(self.label_color_factors)
         )
 
         if new_label_set != self.label_set:
             self._rebuild_pane()
 
-
-class NewLabelButton(pn.reactive.Reactive):
-    """A simple button for generating a new label for use with an editable legend. This simply wraps up a button
-    widget with default options set, and an understanding of selections and labels for connecting with plots and
-    editable legends.
-
-    Parameters
-    ----------
-    labels: Array of shape (n_samples,)
-        The class labels vector giving the class label of each sample.
-
-    button_type: str (optional, default = "success")
-        The panel button type used. See the panel documentation for more details.
-
-    button_text: str (optional, default = "New Label")
-        The text to display on the button.
-
-    width: int or None (optional, default = None)
-        The width of the button. If ``None`` then let the button size itself.
-
-    name: str (optional, default = "New Label")
-        The panel name of the pane. See panel documentation for more details.
-    """
-
-    labels = param.Series(default=pd.Series([], dtype="object"), doc="Labels")
-    selected = param.List(default=[], item_type=int, doc="Indices of selected samples")
-
-    def __init__(
-        self,
-        labels: npt.ArrayLike,
-        *,
-        button_type: str = "success",
-        button_text: str = "New Label",
-        width: Optional[int] = None,
-        name: str = "New Label",
-    ) -> None:
-        super().__init__(name=name)
-        self.label_count = 1
-        self.pane = pn.widgets.Button(
-            name=button_text, button_type=button_type, width=width
-        )
-        self.pane.on_click(self._on_click)
-        self.pane.disabled = True
-        self.labels = pd.Series(labels).copy()  # .reset_index(drop=True)
-
-    def _on_click(self, event: param.parameterized.Event) -> None:
-        if len(self.selected) > 0:
-            new_labels = self.labels
-            new_labels.iloc[self.selected] = f"new_label_{self.label_count}"
-            self.labels = new_labels
-            self.label_count += 1
-
-            self.selected = []
-
-    @param.depends("selected", watch=True)
-    def _toggle_active(self):
-        if len(self.selected) > 0:
-            self.pane.disabled = False
+    def link_to_plot(self, plot):
+        self.labels = plot.labels
+        if self.selectable:
+            self.link(plot, selected="selected", bidirectional=False)
+            return self.link(
+                plot,
+                labels="labels",
+                label_color_factors="label_color_factors",
+                label_color_palette="label_color_palette",
+                bidirectional=True,
+            )
         else:
-            self.pane.disabled = True
-
-    def _get_model(self, *args, **kwds):
-        return self.pane._get_model(*args, **kwds)
+            return self.link(
+                plot,
+                labels="labels",
+                label_color_factors="label_color_factors",
+                label_color_palette="label_color_palette",
+                bidirectional=True,
+            )
 
 
 class LabelEditorWidget(pn.reactive.Reactive):
     """A pane for editing class labels, ideally intended to be linked with a PlotPane. The pane itself is composed of
     an editable legend, and a "new label" button. With the editable legend you can edit the names of class labels,
     and alter the colours used in the palette for plotting class labels, while having those changes reflected in the
     labels themselves. The "new label" button is selection aware and can create a new class label based on the
@@ -440,35 +399,44 @@
             color_picker_margin=color_picker_margin,
             label_height=label_height,
             label_width=label_width,
             label_max_width=label_max_width,
             label_min_width=label_min_width,
             label_margin=label_margin,
         )
-        self.new_label_button = NewLabelButton(
-            labels,
-            button_type=newlabel_button_type,
-            button_text=newlabel_button_text,
-            width=label_width + color_picker_width,
-        )
-        self.legend.link(
-            self,
-            labels="labels",
-            label_color_palette="label_color_palette",
-            label_color_factors="label_color_factors",
-            selected="selected",
-            bidirectional=True,
-        )
-        self.new_label_button.link(
-            self, labels="labels", selected="selected", bidirectional=True,
+        self.new_label_count = 1
+        self.new_label_button = pn.widgets.Button(
+            name=newlabel_button_text, button_type=newlabel_button_type, width=width
         )
+        self.new_label_button.on_click(self._on_click)
+        self.new_label_button.disabled = True
         self.pane = pn.WidgetBox(
             title, self.legend, self.new_label_button, width=width, height=height
         )
 
+    def _on_click(self, event: param.parameterized.Event) -> None:
+        if len(self.selected) > 0:
+            new_labels = self.labels.copy()
+            new_labels.iloc[self.selected] = f"new_label_{self.new_label_count}"
+            self.labels = new_labels
+            self.new_label_count += 1
+
+            # self.legend.labels = new_labels
+            # self.legend._rebuild_pane()
+
+            self.selected = []
+
+
+    @param.depends("selected", watch=True)
+    def _toggle_active(self):
+        if len(self.selected) > 0:
+            self.new_label_button.disabled = False
+        else:
+            self.new_label_button.disabled = True
+
     def _get_model(self, *args, **kwds):
         return self.pane._get_model(*args, **kwds)
 
     def link_to_plot(self, plot):
         """Link this pane to a plot pane using a default set of params that can sensibly be linked.
 
         Parameters
@@ -481,14 +449,15 @@
         link:
             The link object.
         """
         self.labels = plot.labels
         self.label_color_factors = plot.label_color_factors
         self.label_color_palette = plot.label_color_palette
         self.legend._rebuild_pane()
+        self.legend.link_to_plot(plot)
         return self.link(
             plot,
             labels="labels",
             label_color_factors="label_color_factors",
             label_color_palette="label_color_palette",
             selected="selected",
             bidirectional=True,
```

### Comparing `thisnotthat-0.2.1/thisnotthat/map_cluster_labelling.py` & `thisnotthat-0.3/thisnotthat/map_cluster_labelling.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 from hdbscan._hdbscan_tree import recurse_leaf_dfs, get_cluster_tree_leaves
 from sklearn.neighbors import LocalOutlierFactor
 from sklearn.cluster import AgglomerativeClustering
 from sklearn.linear_model import LogisticRegression
 from sklearn.preprocessing import RobustScaler
 from sklearn.metrics import pairwise_distances
 from pynndescent import NNDescent
+from scipy.sparse import spmatrix
+from vectorizers.transformers import InformationWeightTransformer
 
 import numpy as np
 import numpy.typing as npt
 
 try:
     import networkx as nx
 
@@ -759,15 +761,17 @@
     -------
     labels: List of list of lists of label items
         The resulting layers; each layer is a list of cluster labels; each cluster label is a list of label items
     """
     if HAS_APRICOT and sample_selection_method != "random":
         if sample_selection_method == "facility_location":
             selector = apricot.FacilityLocationSelection(
-                items_per_label, metric=vector_metric, n_neighbors=100,
+                items_per_label,
+                metric=vector_metric,
+                n_neighbors=100,
             )
         elif sample_selection_method == "graph_cut":
             selector = apricot.GraphCutSelection(items_per_label, metric=vector_metric)
         elif sample_selection_method == "sum_redundancy":
             selector = apricot.SumRedundancySelection(
                 items_per_label, metric=vector_metric
             )
@@ -799,14 +803,44 @@
             layer_labels.append(list(label_selection))
 
         labels.append(layer_labels)
 
     return labels
 
 
+def text_labels_from_sparse_metadata(
+    pointset_layers: List[List[npt.NDArray]],
+    sparse_metadata: spmatrix,
+    feature_name_dictionary: Dict[int, str],
+    *,
+    items_per_label: int = 3,
+):
+    labels = []
+    positive_matrix = np.abs(sparse_metadata)
+    for layer in pointset_layers:
+        layer_labels = []
+        cluster_class_labels = np.full(positive_matrix.shape[0], -1, dtype=np.int64)
+        for i, pointset in enumerate(layer):
+            cluster_class_labels[pointset] = i
+
+        weighted_matrix = InformationWeightTransformer().fit_transform(
+            positive_matrix, cluster_class_labels
+        )
+        for pointset in layer:
+            cluster_scores = np.squeeze(np.array(weighted_matrix[pointset].sum(axis=0)))
+            top_indices = np.argsort(cluster_scores)[-items_per_label:]
+            layer_labels.append(
+                [feature_name_dictionary[idx] for idx in reversed(top_indices)]
+            )
+
+        labels.append(layer_labels)
+
+    return labels
+
+
 class JointVectorLabelLayers(object):
     """Generate multiple layers of labelling for a map based on the existence of a joint vector space representation
      of the source vector data for the map, and a separate set of label vectors that exist in the same vector space. To
      do this we assume we have a ``text_representation`` providing a vector to each "word" such that the vectors exist in
      the *same* vector space as the ``vector_layers`` vector representations.
 
      Multiple layers of clusters are generated, with higher level layers having larger more general clusters. Each
@@ -1374,9 +1408,193 @@
         )
         self.label_formatter = label_formatter
 
     @property
     def labels_for_display(self):
         return [
             [self.label_formatter(label) for label in label_layer]
+            for label_layer in self.labels
+        ]
+
+
+class SparseMetadataLabelLayers(object):
+    """Generate multiple layers of labelling for a map based on a dataframe of metadata associated to points. Multiple
+    layers of clusters are generated, with higher level layers having larger more general clusters. Each cluster is
+    then labelled by training a one versus the rest classifier to discern the cluster in terms of the associated
+    metadata. The feature importances can then be used to label a cluster with the most discerning features.
+
+    Parameters
+    ----------
+     source_vectors: Array of shape (n_samples, n_features)
+         The original high dimensional vector representation of the data
+
+     map_representation: Array of shape (n_samples, n_map_features)
+         The map representation of the data
+
+    sparse_metadata: spmatrix
+        A sparse matrix of metadata associated to the points of data / map representation. Usually this is associated
+        with metadata that has a high number of features, and any given sample only has non-zero values for a small
+        number of features. A prime example is a bag-of-words representation of a corpus of documents.
+
+    fetaure_name_dictionary: dict
+        A dictionary mapping column indices of the sparse matrix to feature names. For example, if the sparse matrix
+        were the output of sklearn's ``CountVectorizer`` the dict would be
+        ``{idx: word for word, idx in model.vocabulary_.items()}``.
+
+    vector_metric: str (optional, default = "cosine")
+        The metric to use on the source vector space.
+
+    cluster_map_representation: bool (optional, default = False)
+        Whether to directly cluster the map representation, or use UMAP to generate a representation for clustering
+        using ``umap_n_components`` many dimensions.
+
+    umap_n_components:
+        The number of dimensions to use UMAP to reduce to if ``cluster_map_representation`` is ``False``.
+
+    umap_n_neighbors: int (optional, default = 15)
+        The number of neighbors to use for UMAP  if ``cluster_map_representation`` is ``False``.
+
+    hdbscan_min_samples: int (optional, default = 10)
+        The ``min_samples`` value to use with HDBSCAN for clustering.
+
+    hdbscan_min_cluster_size: int (optional, default = 20)
+        The ``min_cluster_size`` value to use with HDBSCAN for clustering.
+
+    min_clusters: int (optional, default = 4)
+        The number of clusters to have at the highest layer; layers with fewer than this number of clusters will
+        be discarded
+
+    contamination: float (optional, default = 0.05)
+        The base contamination score used for outlier detection of fine grained clusters. Larger values will
+        prune out more outliers
+
+    contamination_multiplier: float (optional, default = 1.5)
+        The value to multiply the contamination score by as we increase the layers -- thus applying
+        higher contamination and removing more outliers from higher layers. Larger values will prune
+        more aggressively
+
+    max_contamination: float (optional, default = 0.25)
+        The maximum contamination value to use in outlier pruning -- once the multiplier increases
+        contamination beyond this value the contamination used will simply be capped at this value.
+
+    cluster_distance_threshold: float (optional, default = 0.025)
+        Cluster centroid representatives from a higher layer that are within this distance of an already selected
+        cluster centroid in a lower layer will be ignored (so we don't repeat clusters)
+
+    adjust_label_locations: bool (optional, default = True)
+        Whether to attempt to adjust label locations to avoid overlaps with lower layers.
+
+    label_adjust_spring_constant: float (optional, default = 0.1)
+        The "optimal" distance from the source position; larger values will allow the adjusted cluster to move farther
+
+    label_adjust_spring_constant_multiplier: float (optional, default = 1.5)
+         We can increase the spring constant for higher level layers; to do this we multiply by the
+         ``spring_constant_multiplier`` as we go up a layer. Smaller values (closer to 1.0) will ensure locations
+         do no stray too far; this is particularly desireable in the case where there are many layers.
+
+    label_adjust_edge_weight: float (optional, default = 1.0)
+        How strong the springs pull
+
+    items_per_label: int (optional, default = 3)
+        The number of items to use for each cluster label
+
+    label_formatter: Function (optional, default = string_label_formatter)
+        A function used for format a list of label items into a usable label (usually a single string).
+
+    random_state: int or None (optional, default = None)
+        A random state parameter which can be used to ensure fixed results for reproducibility.
+
+     Attributes
+     ----------
+    labels: List of list of lists of label items
+        A list of layers; each layer is a list of labels; each label is a list of label ``items_per_label`` many items
+
+    location_layers: List of Arrays of shape (n_cluster_in_layer, n_map_features)
+        A list of layers; each layer is an array of locations in the map representation to place the labels of that layer
+
+    labels_for_display: List of list of labels
+        A list of layers; each layer is a list of labels; each label is formatted for display use by ``label_formatter``
+    """
+
+    def __init__(
+        self,
+        source_vectors: npt.ArrayLike,
+        map_representation: npt.ArrayLike,
+        sparse_metadata: spmatrix,
+        feature_name_dictionary: Dict[int, str],
+        *,
+        vector_metric: str = "cosine",
+        cluster_map_representation: bool = False,
+        umap_n_components: int = 5,
+        umap_n_neighbors: int = 15,
+        hdbscan_min_samples: int = 10,
+        hdbscan_min_cluster_size: int = 20,
+        min_clusters_in_layer: int = 4,
+        contamination: float = 0.05,
+        contamination_multiplier: float = 1.5,
+        max_contamination: float = 0.25,
+        cluster_distance_threshold: float = 0.025,
+        adjust_label_locations: bool = True,
+        label_adjust_spring_constant: float = 0.1,
+        label_adjust_spring_constant_multiplier: float = 1.5,
+        label_adjust_edge_weight: float = 1.0,
+        items_per_label: int = 3,
+        label_formatter: Callable[[List[Any]], Any] = string_label_formatter,
+        random_state: Optional[int] = None,
+    ):
+        if adjust_label_locations and not HAS_NETWORKX:
+            warn("NetworkX is required for label adjustments; try pip install networkx")
+            adjust_label_locations = False
+
+        (
+            cluster_vectors,
+            cluster_locations,
+            hdbscan_tree,
+        ) = build_fine_grained_cluster_centers(
+            source_vectors,
+            map_representation,
+            cluster_map_representation=cluster_map_representation,
+            umap_metric=vector_metric,
+            umap_n_components=umap_n_components,
+            umap_n_neighbors=umap_n_neighbors,
+            hdbscan_min_samples=hdbscan_min_samples,
+            hdbscan_min_cluster_size=hdbscan_min_cluster_size,
+            random_state=random_state,
+        )
+        (
+            vector_layers,
+            self.location_layers,
+            self.pointset_layers,
+        ) = build_cluster_layers(
+            cluster_vectors,
+            cluster_locations,
+            min_clusters=min_clusters_in_layer,
+            contamination=contamination,
+            vector_metric=vector_metric,
+            cluster_distance_threshold=cluster_distance_threshold,
+            contamination_multiplier=contamination_multiplier,
+            max_contamination=max_contamination,
+            return_pointsets=True,
+            hdbscan_tree=hdbscan_tree,
+        )
+        if adjust_label_locations:
+            self.location_layers = text_locations(
+                self.location_layers,
+                spring_constant=label_adjust_spring_constant,
+                spring_constant_multiplier=label_adjust_spring_constant_multiplier,
+                edge_weight=label_adjust_edge_weight,
+            )
+
+        self.labels = text_labels_from_sparse_metadata(
+            self.pointset_layers,
+            sparse_metadata,
+            feature_name_dictionary,
+            items_per_label=items_per_label,
+        )
+        self.label_formatter = label_formatter
+
+    @property
+    def labels_for_display(self):
+        return [
+            [self.label_formatter(label) for label in label_layer]
             for label_layer in self.labels
         ]
```

### Comparing `thisnotthat-0.2.1/thisnotthat/palettes.py` & `thisnotthat-0.3/thisnotthat/palettes.py`

 * *Files identical despite different names*

### Comparing `thisnotthat-0.2.1/thisnotthat/plot_controls.py` & `thisnotthat-0.3/thisnotthat/plot_controls.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,19 +86,19 @@
         self.color_by_column = pn.widgets.Select(
             name="Color by column", options=["Default"] + list(self.dataframe.columns),
         )
         self.color_by_column.param.watch(
             self._options_changed, "value", onlychanged=True
         )
         self.color_by_scale_selector = pn.Row(
-            pn.widgets.StaticText(value="Scale type", align=("end", "center"), margin=[5, 0, 5, 5]),
+            pn.widgets.StaticText(value="Scale type", align=("end", "center"), margin=(5, 0, 5, 5)),
             pn.widgets.ToggleGroup(
                 name="Color by scale", options=["Linear", "Log", "Sqrt"], behavior="radio", value="Linear"
             ),
-            margin=[0, 10],
+            margin=(0, 10),
             visible=scale_type_selector
         )
         self.color_by_scale_selector[1].param.watch(self._options_changed, "value", onlychanged=True)
         self.hover_text_column = pn.widgets.Select(
             name="Hover text column",
             options=["Default"] + list(self.dataframe.columns),
         )
@@ -110,43 +110,43 @@
             options=["Default"]
             + list(self.dataframe.select_dtypes(include="number").columns),
         )
         self.marker_size_column.param.watch(
             self._options_changed, "value", onlychanged=True
         )
         self.marker_size_scale_selector = pn.Row(
-            pn.widgets.StaticText(value="Scale type", align=("end", "center"), margin=[5, 0, 5, 5]),
+            pn.widgets.StaticText(value="Scale type", align=("end", "center"), margin=(5, 0, 5, 5)),
             pn.widgets.ToggleGroup(
                 name="Marker size scale", options=["Linear", "Log", "Sqrt"], behavior="radio", value="Linear"
             ),
-            margin=[0, 5,  0, 10],
+            margin=(0, 5,  0, 10),
             visible=scale_type_selector
         )
         self.marker_size_scale_selector[1].param.watch(self._options_changed, "value", onlychanged=True)
         self.apply_changes = pn.widgets.Button(
             name="Apply Changes", button_type="success", disabled=True,
         )
         self.apply_changes.on_click(self._reapply_changes)
         self.bad_scaling_alert = pn.pane.Alert(
             "### Bad scale\nColumn with Log or Sqrt scale contains negative values; Using a linear scale",
             alert_type="danger",
             visible=False,
         )
         self.pane = pn.WidgetBox(
             title,
-            pn.layout.Divider(margin=[0, 10, 10, 10], height=5),
+            pn.layout.Divider(margin=(0, 10, 10, 10), height=5),
             self.palette_selector,
             self.color_by_column,
             self.color_by_scale_selector,
-            pn.layout.Divider(margin=[0, 10, 10, 10], height=5),
+            pn.layout.Divider(margin=(0, 10, 10, 10), height=5),
             self.marker_size_column,
             self.marker_size_scale_selector,
-            pn.layout.Divider(margin=[0, 10, 10, 10], height=5),
+            pn.layout.Divider(margin=(0, 10, 10, 10), height=5),
             self.hover_text_column,
-            pn.layout.Divider(margin=[0, 10, 10, 10], height=5),
+            pn.layout.Divider(margin=(0, 10, 10, 10), height=5),
             self.apply_changes,
             self.bad_scaling_alert,
             width=width,
             height=height,
         )
 
     def _get_model(self, *args, **kwds):
```

### Comparing `thisnotthat-0.2.1/thisnotthat/utils.py` & `thisnotthat-0.3/thisnotthat/utils.py`

 * *Files identical despite different names*

### Comparing `thisnotthat-0.2.1/thisnotthat.egg-info/PKG-INFO` & `thisnotthat-0.3/thisnotthat.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 Metadata-Version: 2.1
 Name: thisnotthat
-Version: 0.2.1
+Version: 0.3
 Summary: Tools for interactive visualization and exploration of _data maps_
-Home-page: https://github.com/TutteInstitute/vectorizers
+Home-page: https://github.com/TutteInstitute/thisnotthat
 Download-URL: https://github.com/TutteInstitute/thisnotthat
 Maintainer: Benoit Hamelin, John Healy, Leland McInnes
 Maintainer-email: leland.mcinnes@gmail.com
 License: new BSD
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: tests
 Provides-Extra: docs
 License-File: LICENSE
 
 .. -*- mode: rst -*-
@@ -63,14 +61,20 @@
 -------------------------------
 This Not That for Data Map Apps
 -------------------------------
 
 Because This Not That is built on top of the `Panel library`_ it is trivial to deploy TNT based solutions as
 interactive web applications.
 
+-------------
+Documentation
+-------------
+
+Get the latest on `Read The Docs <https://thisnotthat.readthedocs.io/en/latest/>`_.
+
 ----------
 Installing
 ----------
 
 This Not That is built on top of Panel and Bokeh, so you will need these installed. In all you will need:
 
 * panel
@@ -78,14 +82,16 @@
 * numpy >= 1.22
 * pandas
 * scikit-learn
 * matplotlib
 * umap-learn
 * hdbscan
 * glasbey
+* cmocean
+* vectorizers
 
 We also highly recommend installing:
 
 * networkx
 * apricot-select
 
 Currently you can pip install directly from this repository:
@@ -111,14 +117,14 @@
 submit a pull request. We will do our best to work through any issues with
 you and get your code merged into the main branch.
 
 -------
 License
 -------
 
-The This Not That package is 2-clause BSD licensed.
+The This Not That package is 3-clause BSD licensed.
 
 
 .. _Panel library: https://panel.holoviz.org/
```

