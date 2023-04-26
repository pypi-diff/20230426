# Comparing `tmp/pyptv-0.2.2.tar.gz` & `tmp/pyptv-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyptv-0.2.2.tar", last modified: Tue Mar 14 07:24:33 2023, max compression
+gzip compressed data, was "pyptv-0.2.3.tar", last modified: Wed Apr 26 14:16:11 2023, max compression
```

## Comparing `pyptv-0.2.2.tar` & `pyptv-0.2.3.tar`

### file list

```diff
@@ -1,36 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-03-14 07:24:33.300934 pyptv-0.2.2/
--rw-rw-rw-   0        0        0     1082 2022-11-30 07:16:48.000000 pyptv-0.2.2/LICENSE.txt
--rw-rw-rw-   0        0        0      307 2023-03-14 07:24:33.298934 pyptv-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     1661 2023-03-05 08:44:39.000000 pyptv-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-03-14 07:24:33.281929 pyptv-0.2.2/pyptv/
--rw-rw-rw-   0        0        0        0 2022-11-30 07:16:48.000000 pyptv-0.2.2/pyptv/__init__.py
--rw-rw-rw-   0        0        0       32 2022-11-30 07:16:48.000000 pyptv-0.2.2/pyptv/__main__.py
--rw-rw-rw-   0        0        0    42701 2023-03-05 06:38:07.000000 pyptv-0.2.2/pyptv/calibration_gui.py
--rw-rw-rw-   0        0        0       39 2022-11-30 07:16:48.000000 pyptv-0.2.2/pyptv/cli.py
--rw-rw-rw-   0        0        0     2402 2023-03-14 07:21:44.000000 pyptv-0.2.2/pyptv/code_editor.py
--rw-rw-rw-   0        0        0    20904 2023-03-05 06:38:07.000000 pyptv-0.2.2/pyptv/detection_gui.py
--rw-rw-rw-   0        0        0      960 2022-11-30 07:16:48.000000 pyptv-0.2.2/pyptv/directory_editor.py
--rw-rw-rw-   0        0        0      869 2022-11-30 07:16:48.000000 pyptv-0.2.2/pyptv/draw_3d_target.py
--rw-rw-rw-   0        0        0     2796 2023-03-05 06:38:07.000000 pyptv-0.2.2/pyptv/ext_sequence_denis.py
--rw-rw-rw-   0        0        0     1310 2022-11-30 07:16:48.000000 pyptv-0.2.2/pyptv/ext_tracker_denis.py
--rw-rw-rw-   0        0        0     3236 2023-03-01 06:54:27.000000 pyptv-0.2.2/pyptv/image_inspector.py
--rw-rw-rw-   0        0        0     1418 2023-03-01 06:54:27.000000 pyptv-0.2.2/pyptv/imageplot.py
--rw-rw-rw-   0        0        0     7396 2023-03-01 06:54:27.000000 pyptv-0.2.2/pyptv/imread_chaco.py
--rw-rw-rw-   0        0        0    47882 2023-03-01 07:37:03.000000 pyptv-0.2.2/pyptv/parameter_gui.py
--rw-rw-rw-   0        0        0    43893 2023-03-01 08:20:41.000000 pyptv-0.2.2/pyptv/parameters.py
--rw-rw-rw-   0        0        0    17242 2023-03-14 07:21:44.000000 pyptv-0.2.2/pyptv/ptv.py
--rw-rw-rw-   0        0        0     4105 2023-03-05 06:38:07.000000 pyptv-0.2.2/pyptv/pyptv_batch.py
--rw-rw-rw-   0        0        0    56206 2023-03-14 07:22:37.000000 pyptv-0.2.2/pyptv/pyptv_gui.py
--rw-rw-rw-   0        0        0     2038 2023-03-01 06:53:35.000000 pyptv-0.2.2/pyptv/quiver_demo.py
--rw-rw-rw-   0        0        0     4816 2022-11-30 07:16:48.000000 pyptv-0.2.2/pyptv/quiverplot.py
--rw-rw-rw-   0        0        0     3602 2023-03-14 07:21:44.000000 pyptv-0.2.2/pyptv/scatter_inspector2.py
--rw-rw-rw-   0        0        0     4409 2022-11-30 07:16:48.000000 pyptv-0.2.2/pyptv/text_box_overlay.py
-drwxrwxrwx   0        0        0        0 2023-03-14 07:24:33.296934 pyptv-0.2.2/pyptv.egg-info/
--rw-rw-rw-   0        0        0      307 2023-03-14 07:24:32.000000 pyptv-0.2.2/pyptv.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      686 2023-03-14 07:24:33.000000 pyptv-0.2.2/pyptv.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-14 07:24:32.000000 pyptv-0.2.2/pyptv.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-03-14 07:24:32.000000 pyptv-0.2.2/pyptv.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      102 2023-03-14 07:24:32.000000 pyptv-0.2.2/pyptv.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-03-14 07:24:32.000000 pyptv-0.2.2/pyptv.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-14 07:24:33.300934 pyptv-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0      764 2023-03-14 07:22:42.000000 pyptv-0.2.2/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-26 14:16:11.449212 pyptv-0.2.3/
+-rw-rw-r--   0 user      (1000) user      (1000)     1062 2022-11-16 19:45:05.000000 pyptv-0.2.3/LICENSE.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      297 2023-04-26 14:16:11.449212 pyptv-0.2.3/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1611 2023-03-05 14:40:34.000000 pyptv-0.2.3/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-26 14:16:11.445212 pyptv-0.2.3/pyptv/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2022-11-16 20:26:01.000000 pyptv-0.2.3/pyptv/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)       29 2022-11-16 19:45:05.000000 pyptv-0.2.3/pyptv/__main__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    41516 2023-04-21 19:00:59.000000 pyptv-0.2.3/pyptv/calibration_gui.py
+-rw-rw-r--   0 user      (1000) user      (1000)       37 2022-11-15 19:14:45.000000 pyptv-0.2.3/pyptv/cli.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2299 2023-03-12 06:56:19.000000 pyptv-0.2.3/pyptv/code_editor.py
+-rw-rw-r--   0 user      (1000) user      (1000)    20362 2023-03-05 14:40:34.000000 pyptv-0.2.3/pyptv/detection_gui.py
+-rw-rw-r--   0 user      (1000) user      (1000)      924 2022-11-16 19:45:05.000000 pyptv-0.2.3/pyptv/directory_editor.py
+-rw-rw-r--   0 user      (1000) user      (1000)      831 2022-11-16 19:45:05.000000 pyptv-0.2.3/pyptv/draw_3d_target.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2723 2023-03-05 14:40:34.000000 pyptv-0.2.3/pyptv/ext_sequence_denis.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1280 2022-11-16 19:45:05.000000 pyptv-0.2.3/pyptv/ext_tracker_denis.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3135 2023-03-05 14:40:34.000000 pyptv-0.2.3/pyptv/image_inspector.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1377 2023-03-05 14:40:34.000000 pyptv-0.2.3/pyptv/imageplot.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7172 2023-03-05 14:40:34.000000 pyptv-0.2.3/pyptv/imread_chaco.py
+-rw-rw-r--   0 user      (1000) user      (1000)    46489 2023-03-05 14:40:34.000000 pyptv-0.2.3/pyptv/parameter_gui.py
+-rw-rw-r--   0 user      (1000) user      (1000)    42351 2023-04-21 19:16:14.000000 pyptv-0.2.3/pyptv/parameters.py
+-rw-rw-r--   0 user      (1000) user      (1000)    16707 2023-03-12 06:56:19.000000 pyptv-0.2.3/pyptv/ptv.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3958 2023-03-05 14:40:34.000000 pyptv-0.2.3/pyptv/pyptv_batch.py
+-rw-rw-r--   0 user      (1000) user      (1000)    54729 2023-04-26 14:14:02.000000 pyptv-0.2.3/pyptv/pyptv_gui.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1974 2023-03-05 14:40:34.000000 pyptv-0.2.3/pyptv/quiver_demo.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4673 2022-11-16 19:45:05.000000 pyptv-0.2.3/pyptv/quiverplot.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3485 2023-03-12 06:56:19.000000 pyptv-0.2.3/pyptv/scatter_inspector2.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4277 2022-11-16 19:45:05.000000 pyptv-0.2.3/pyptv/text_box_overlay.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-26 14:16:11.449212 pyptv-0.2.3/pyptv.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)      297 2023-04-26 14:16:11.000000 pyptv-0.2.3/pyptv.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      730 2023-04-26 14:16:11.000000 pyptv-0.2.3/pyptv.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-04-26 14:16:11.000000 pyptv-0.2.3/pyptv.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       47 2023-04-26 14:16:11.000000 pyptv-0.2.3/pyptv.egg-info/entry_points.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      102 2023-04-26 14:16:11.000000 pyptv-0.2.3/pyptv.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        6 2023-04-26 14:16:11.000000 pyptv-0.2.3/pyptv.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-04-26 14:16:11.449212 pyptv-0.2.3/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)      727 2023-04-26 13:47:35.000000 pyptv-0.2.3/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-26 14:16:11.449212 pyptv-0.2.3/tests/
+-rw-rw-r--   0 user      (1000) user      (1000)       88 2022-11-16 19:45:05.000000 pyptv-0.2.3/tests/test_cli.py
+-rw-rw-r--   0 user      (1000) user      (1000)      149 2022-11-16 19:45:05.000000 pyptv-0.2.3/tests/test_pyptv_batch.py
```

### Comparing `pyptv-0.2.2/LICENSE.txt` & `pyptv-0.2.3/LICENSE.txt`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-Copyright (c) 2011-2022 Alex Liberzon
-
-Permission is hereby granted, free of charge, to any person obtaining
-a copy of this software and associated documentation files (the
-"Software"), to deal in the Software without restriction, including
-without limitation the rights to use, copy, modify, merge, publish,
-distribute, sublicense, and/or sell copies of the Software, and to
-permit persons to whom the Software is furnished to do so, subject to
-the following conditions:
-
-The above copyright notice and this permission notice shall be
-included in all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
-EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
-MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
-NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
-LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
-OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
-WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+Copyright (c) 2011-2022 Alex Liberzon
+
+Permission is hereby granted, free of charge, to any person obtaining
+a copy of this software and associated documentation files (the
+"Software"), to deal in the Software without restriction, including
+without limitation the rights to use, copy, modify, merge, publish,
+distribute, sublicense, and/or sell copies of the Software, and to
+permit persons to whom the Software is furnished to do so, subject to
+the following conditions:
+
+The above copyright notice and this permission notice shall be
+included in all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
+MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
+NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
+LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
+WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `pyptv-0.2.2/README.md` & `pyptv-0.2.3/README.md`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-# PyPTV
-Python GUI for the OpenPTV library `liboptv`
-
-[![Python package](https://github.com/alexlib/pyptv/actions/workflows/python-package.yml/badge.svg)](https://github.com/alexlib/pyptv/actions/workflows/python-package.yml)
-[![DOI](https://zenodo.org/badge/121291437.svg)](https://zenodo.org/badge/latestdoi/121291437)
-
-
-
-
-**PyPTV** or otherwise called **OpenPTV-Python** is the Python GUI for [OpenPTV](http://www.openptv.net). It is based on `traits`, `traitsui`, `chaco`, `enable` and `pyface` from Enthought Inc. and provides an UI *interface* the OpenPTV library that includes all the core algorithms (correspondence, tracking, calibration, etc.) written in ANSI C and has Python bindings using Cython.  
-
-Both PyPTV and the OpenPTV library are in the development phase and continuously refactored. Please follow the development on the community mailing list:
-
-	openptv@googlegroups.com
-
-
-## Documentation:
-
-<http://openptv-python.readthedocs.io>
-
-## Installation instructions
-
-Short version:
-
-    pip install numpy
-    python -m pip install pyptv --index-url https://pypi.fury.io/pyptv --extra-index-url https://pypi.org/simple
-
-
-Detailed instructions for various platforms are in our documentation: 
-https://openptv-python.readthedocs.io/en/latest/installation_instruction.html
-
-
-
-
-
-Follow the instructions in our **screencasts and tutorials**:
-  
-  *  Tutorial 1: <http://youtu.be/S2fY5WFsFwo>  
-  
-  *  Tutorial 2: <http://www.youtube.com/watch?v=_JxFxwVDSt0>   
-  
-  *  Tutorial 3: <http://www.youtube.com/watch?v=z1eqFL5JIJc>  
-  
-  
-Ask for help on our mailing list:
-
-	openptv@googlegroups.com
-
-
-
+# PyPTV
+Python GUI for the OpenPTV library `liboptv`
+
+[![Python package](https://github.com/alexlib/pyptv/actions/workflows/python-package.yml/badge.svg)](https://github.com/alexlib/pyptv/actions/workflows/python-package.yml)
+[![DOI](https://zenodo.org/badge/121291437.svg)](https://zenodo.org/badge/latestdoi/121291437)
+
+
+
+
+**PyPTV** or otherwise called **OpenPTV-Python** is the Python GUI for [OpenPTV](http://www.openptv.net). It is based on `traits`, `traitsui`, `chaco`, `enable` and `pyface` from Enthought Inc. and provides an UI *interface* the OpenPTV library that includes all the core algorithms (correspondence, tracking, calibration, etc.) written in ANSI C and has Python bindings using Cython.  
+
+Both PyPTV and the OpenPTV library are in the development phase and continuously refactored. Please follow the development on the community mailing list:
+
+	openptv@googlegroups.com
+
+
+## Documentation:
+
+<http://openptv-python.readthedocs.io>
+
+## Installation instructions
+
+Short version:
+
+    pip install numpy
+    python -m pip install pyptv --index-url https://pypi.fury.io/pyptv --extra-index-url https://pypi.org/simple
+
+
+Detailed instructions for various platforms are in our documentation: 
+https://openptv-python.readthedocs.io/en/latest/installation_instruction.html
+
+
+
+
+
+Follow the instructions in our **screencasts and tutorials**:
+  
+  *  Tutorial 1: <http://youtu.be/S2fY5WFsFwo>  
+  
+  *  Tutorial 2: <http://www.youtube.com/watch?v=_JxFxwVDSt0>   
+  
+  *  Tutorial 3: <http://www.youtube.com/watch?v=z1eqFL5JIJc>  
+  
+  
+Ask for help on our mailing list:
+
+	openptv@googlegroups.com
+
+
+
```

### Comparing `pyptv-0.2.2/pyptv/calibration_gui.py` & `pyptv-0.2.3/pyptv/calibration_gui.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,1185 +1,1185 @@
-"""
-Copyright (c) 2008-2013, Tel Aviv University
-Copyright (c) 2013 - the OpenPTV team
-The software is distributed under the terms of MIT-like license
-http://opensource.org/licenses/MIT
-"""
-
-import os
-import shutil
-import re
-from  pathlib import Path
-import numpy as np
-from skimage.io import imread
-from skimage import img_as_ubyte
-from skimage.color import rgb2gray
-
-from traits.api import HasTraits, Str, Int, Bool, Instance, Button
-from traitsui.api import View, Item, HGroup, VGroup, ListEditor
-from enable.component_editor import ComponentEditor
-from chaco.api import (
-    Plot,
-    ArrayPlotData,
-    gray,
-    ArrayDataSource,
-    LinearMapper,
-)
-
-# from traitsui.menu import MenuBar, ToolBar, Menu, Action
-from chaco.tools.image_inspector_tool import ImageInspectorTool
-from chaco.tools.better_zoom import BetterZoom as SimpleZoom
-
-# from chaco.tools.simple_zoom import SimpleZoom
-from pyptv.text_box_overlay import TextBoxOverlay
-from pyptv.code_editor import codeEditor
-from pyptv.quiverplot import QuiverPlot
-
-
-
-from optv.imgcoord import image_coordinates
-from optv.transforms import convert_arr_metric_to_pixel
-from optv.orientation import match_detection_to_ref
-from optv.orientation import external_calibration, full_calibration
-from optv.calibration import Calibration
-from optv.tracking_framebuf import TargetArray
-
-
-from pyptv import ptv, parameter_gui, parameters as par
-
-
-# -------------------------------------------
-class ClickerTool(ImageInspectorTool):
-    left_changed = Int(1)
-    right_changed = Int(1)
-    x = 0
-    y = 0
-
-    def normal_left_down(self, event):
-        """Handles the left mouse button being clicked.
-        Fires the **new_value** event with the data (if any) from the event's
-        position.
-        """
-        plot = self.component
-        if plot is not None:
-            ndx = plot.map_index((event.x, event.y))
-
-            x_index, y_index = ndx
-            # image_data = plot.value
-            self.x = x_index
-            self.y = y_index
-            print(self.x)
-            print(self.y)
-            self.left_changed = 1 - self.left_changed
-            self.last_mouse_position = (event.x, event.y)
-
-    def normal_right_down(self, event):
-        plot = self.component
-        if plot is not None:
-            ndx = plot.map_index((event.x, event.y))
-
-            x_index, y_index = ndx
-            # image_data = plot.value
-            self.x = x_index
-            self.y = y_index
-
-            self.right_changed = 1 - self.right_changed
-            print(self.x)
-            print(self.y)
-
-            self.last_mouse_position = (event.x, event.y)
-
-    def normal_mouse_move(self, event):
-        pass
-
-    def __init__(self, *args, **kwargs):
-        super(ClickerTool, self).__init__(*args, **kwargs)
-
-
-# ----------------------------------------------------------
-
-
-class PlotWindow(HasTraits):
-    _plot = Instance(Plot)
-    _click_tool = Instance(ClickerTool)
-    _right_click_avail = 0
-    name = Str
-    view = View(
-        Item(name="_plot", editor=ComponentEditor(), show_label=False),
-    )
-
-    def __init__(self):
-        # super(HasTraits, self).__init__()
-        super().__init__()
-        # -------------- Initialization of plot system ----------------
-        padd = 25
-        self._plot_data = ArrayPlotData()
-        self._x, self._y = [], []
-        self.man_ori = [1, 2, 3, 4]
-        self._plot = Plot(self._plot_data, default_origin="top left")
-        self._plot.padding = (padd, padd, padd, padd)
-        # self._quiverplots = []
-
-        # -------------------------------------------------------------
-
-    def left_clicked_event(self):
-        print("left clicked")
-        if len(self._x) < 4:
-            self._x.append(self._click_tool.x)
-            self._y.append(self._click_tool.y)
-        print(self._x, self._y)
-
-        self.drawcross("coord_x", "coord_y", self._x, self._y, "red", 5)
-        self._plot.overlays.clear()
-        self.plot_num_overlay(self._x, self._y, self.man_ori)
-
-    def right_clicked_event(self):
-        print("right clicked")
-        if len(self._x) > 0:
-            self._x.pop()
-            self._y.pop()
-            print(self._x, self._y)
-
-            self.drawcross("coord_x", "coord_y", self._x, self._y, "red", 5)
-            self._plot.overlays.clear()
-            self.plot_num_overlay(self._x, self._y, self.man_ori)
-        else:
-            if self._right_click_avail:
-                print("deleting point")
-                self.py_rclick_delete(
-                    self._click_tool.x, self._click_tool.y, self.cameraN
-                )
-                x = []
-                y = []
-                self.py_get_pix_N(x, y, self.cameraN)
-                self.drawcross("x", "y", x[0], y[0], "blue", 4)
-
-    def attach_tools(self):
-        self._click_tool = ClickerTool(self._img_plot)
-        self._click_tool.on_trait_change(
-            self.left_clicked_event, "left_changed"
-        )
-        self._click_tool.on_trait_change(
-            self.right_clicked_event, "right_changed"
-        )
-        self._img_plot.tools.append(self._click_tool)
-        self._zoom_tool = SimpleZoom(
-            component=self._plot, tool_mode="box", always_on=False
-        )
-        self._zoom_tool.max_zoom_out_factor = 1.0
-        self._img_plot.tools.append(self._zoom_tool)
-        if self._plot.index_mapper is not None:
-            self._plot.index_mapper.on_trait_change(
-                self.handle_mapper, "updated", remove=False
-            )
-        if self._plot.value_mapper is not None:
-            self._plot.value_mapper.on_trait_change(
-                self.handle_mapper, "updated", remove=False
-            )
-
-    def drawcross(self, str_x, str_y, x, y, color1="blue", mrk_size=1, marker="plus"):
-        """
-        Draws crosses on images
-        """
-        self._plot_data.set_data(str_x, x)
-        self._plot_data.set_data(str_y, y)
-        self._plot.plot(
-            (str_x, str_y),
-            type="scatter",
-            color=color1,
-            marker=marker,
-            marker_size=mrk_size,
-        )
-        self._plot.request_redraw()
-
-    def drawline(self, str_x, str_y, x1, y1, x2, y2, color1):
-        self._plot_data.set_data(str_x, [x1, x2])
-        self._plot_data.set_data(str_y, [y1, y2])
-        self._plot.plot((str_x, str_y), type="line", color=color1)
-        self._plot.request_redraw()
-
-    def drawquiver(self, x1c, y1c, x2c, y2c, color, linewidth=1.0, scale=1.0):
-        """drawquiver draws multiple lines at once on the screen x1,y1->x2,y2 in the current camera window
-        parameters:
-            x1c - array of x1 coordinates
-            y1c - array of y1 coordinates
-            x2c - array of x2 coordinates
-            y2c - array of y2 coordinates
-            color - color of the line
-            linewidth - linewidth of the line
-        example usage:
-            drawquiver ([100,200],[100,100],[400,400],[300,200],'red',linewidth=2.0)
-            draws 2 red lines with thickness = 2 :  100,100->400,300 and 200,100->400,200
-
-        """
-        x1, y1, x2, y2 = self.remove_short_lines(
-            x1c, y1c, x2c, y2c, min_length=0
-        )
-        if len(x1) > 0:
-            xs = ArrayDataSource(x1)
-            ys = ArrayDataSource(y1)
-
-            # quiverplot = QuiverPlot(
-            #     index=xs,
-            #     value=ys,
-            #     index_mapper=LinearMapper(range=self._plot.index_mapper.range),
-            #     value_mapper=LinearMapper(range=self._plot.value_mapper.range),
-            #     origin=self._plot.origin,
-            #     arrow_size=0,
-            #     line_color=color,
-            #     line_width=linewidth,
-            #     ep_index=np.array(x2) * scale,
-            #     ep_value=np.array(y2) * scale,
-            # )
-            vectors = np.array(((np.array(x2)-np.array(x1))/scale, 
-                                (np.array(y2)-np.array(y1))/scale)).T
-            self._plot_data.set_data("index", x1)
-            self._plot_data.set_data("value", y1)
-            self._plot_data.set_data("vectors", vectors)
-            # self._quiverplots.append(quiverplot)
-            self._plot.quiverplot(
-                ('index','value','vectors'),
-                arrow_size=0,
-                line_color="red"
-                )
-            # self._plot.overlays.append(quiverplot)
-        
-    def remove_short_lines(self, x1, y1, x2, y2, min_length=2):
-        """removes short lines from the array of lines
-        parameters:
-            x1,y1,x2,y2 - start and end coordinates of the lines
-        returns:
-            x1f,y1f,x2f,y2f - start and end coordinates of the lines, with short lines removed
-        example usage:
-            x1,y1,x2,y2=remove_short_lines([100,200,300],[100,200,300],[100,200,300],[102,210,320])
-            3 input lines, 1 short line will be removed (100,100->100,102)
-            returned coordinates:
-            x1=[200,300]; y1=[200,300]; x2=[200,300]; y2=[210,320]
-        """
-        # dx, dy = 2, 2  # minimum allowable dx,dy
-        x1f, y1f, x2f, y2f = [], [], [], []
-        for i in range(len(x1)):
-            if (
-                abs(x1[i] - x2[i]) > min_length
-                or abs(y1[i] - y2[i]) > min_length
-            ):
-                x1f.append(x1[i])
-                y1f.append(y1[i])
-                x2f.append(x2[i])
-                y2f.append(y2[i])
-        return x1f, y1f, x2f, y2f
-
-    def handle_mapper(self):
-        for i in range(0, len(self._plot.overlays)):
-            if hasattr(self._plot.overlays[i], "real_position"):
-                coord_x1, coord_y1 = self._plot.map_screen(
-                    [self._plot.overlays[i].real_position]
-                )[0]
-                self._plot.overlays[i].alternate_position = (
-                    coord_x1,
-                    coord_y1,
-                )
-
-    def plot_num_overlay(self, x, y, txt):
-        for i in range(len(x)):
-            coord_x, coord_y = self._plot.map_screen([(x[i], y[i])])[0]
-            ovlay = TextBoxOverlay(
-                component=self._plot,
-                text=str(txt[i]),
-                alternate_position=(coord_x, coord_y),
-                real_position=(x[i], y[i]),
-                text_color="white",
-                border_color="red",
-            )
-            self._plot.overlays.append(ovlay)
-
-    def update_image(self, image, is_float):
-        if is_float:
-            self._plot_data.set_data("imagedata", image.astype(float))
-        else:
-            self._plot_data.set_data("imagedata", image.astype(np.uint8))
-            
-        # Alex added to plot the image here from update image
-        self._img_plt = self._plot.img_plot("imagedata", colormap=gray)[0]
-
-        self._plot.request_redraw()
-
-
-# ---------------------------------------------------------
-
-
-class CalibrationGUI(HasTraits):
-    status_text = Str("")
-    ori_img_name = []
-    ori_img = []
-    pass_init = Bool(False)
-    pass_sortgrid = Bool(False)
-    pass_raw_orient = Bool(False)
-    pass_init_disabled = Bool(False)
-    # -------------------------------------------------------------
-    button_edit_cal_parameters = Button()
-    button_showimg = Button()
-    button_detection = Button()
-    button_manual = Button()
-    button_file_orient = Button()
-    button_init_guess = Button()
-    button_sort_grid = Button()
-    button_sort_grid_init = Button()
-    button_raw_orient = Button()
-    button_fine_orient = Button()
-    button_orient_part = Button()
-    button_orient_shaking = Button()
-    button_orient_dumbbell = Button()
-    button_restore_orient = Button()
-    button_checkpoint = Button()
-    button_ap_figures = Button()
-    button_edit_ori_files = Button()
-    button_test = Button()
-
-    # ---------------------------------------------------
-    # Constructor
-    # ---------------------------------------------------
-    def __init__(self, active_path: Path):
-        """Initialize CalibrationGUI
-
-        Inputs:
-            active_path is the path to the folder of prameters
-            active_path is a subfolder of a working folder with a
-            structure of /parameters, /res, /cal, /img and so on
-        """
-
-        super(CalibrationGUI, self).__init__()
-        self.need_reset = 0
-
-        self.active_path = active_path
-        self.working_folder = self.active_path.parent
-        self.par_path = self.working_folder / "parameters"
-        
-        self.man_ori_dat_path = self.working_folder / "man_ori.dat"
-
-        print(" Copying parameters inside Calibration GUI: \n")
-        par.copy_params_dir(self.active_path, self.par_path)
-
-        
-        os.chdir(self.working_folder)
-        print(f"Inside a folder: {Path.cwd()}")
-        
-        # read parameters
-        with open(self.par_path / "ptv.par", "r") as f:
-            self.n_cams = int(f.readline())
-
-        self.camera = [PlotWindow() for i in range(self.n_cams)]
-        for i in range(self.n_cams):
-            self.camera[i].name = "Camera" + str(i + 1)
-            self.camera[i].cameraN = i
-            self.camera[i].py_rclick_delete = ptv.py_rclick_delete
-            self.camera[i].py_get_pix_N = ptv.py_get_pix_N
-
-    # Defines GUI view --------------------------
-
-    view = View(
-        HGroup(
-            VGroup(
-                VGroup(
-                    Item(
-                        name="button_showimg",
-                        label="Load/Show Images",
-                        show_label=False,
-                    ),
-                    Item(
-                        name="button_detection",
-                        label="Detection",
-                        show_label=False,
-                        enabled_when="pass_init",
-                    ),
-                    Item(
-                        name="button_manual",
-                        label="Manual orient.",
-                        show_label=False,
-                        enabled_when="pass_init",
-                    ),
-                    Item(
-                        name="button_file_orient",
-                        label="Orient. with file",
-                        show_label=False,
-                        enabled_when="pass_init",
-                    ),
-                    Item(
-                        name="button_init_guess",
-                        label="Show initial guess",
-                        show_label=False,
-                        enabled_when="pass_init",
-                    ),
-                    Item(
-                        name="button_sort_grid",
-                        label="Sortgrid",
-                        show_label=False,
-                        enabled_when="pass_init",
-                    ),
-                    # Item(name='button_sort_grid_init',
-                    # label='Sortgrid = initial guess',
-                    # show_label=False, enabled_when='pass_init'),
-                    Item(
-                        name="button_raw_orient",
-                        label="Raw orientation",
-                        show_label=False,
-                        enabled_when="pass_sortgrid",
-                    ),
-                    Item(
-                        name="button_fine_orient",
-                        label="Fine tuning",
-                        show_label=False,
-                        enabled_when="pass_raw_orient",
-                    ),
-                    Item(
-                        name="button_orient_part",
-                        label="Orientation with particles",
-                        show_label=False,
-                        enabled_when="pass_init",
-                    ),
-                    Item(
-                        name="button_orient_dumbbell",
-                        label="Orientation from dumbbell",
-                        show_label=False,
-                        enabled_when="pass_init",
-                    ),
-                    Item(
-                        name="button_restore_orient",
-                        label="Restore ori files",
-                        show_label=False,
-                        enabled_when="pass_init",
-                    ),
-                    Item(
-                        name="button_checkpoint",
-                        label="Checkpoints",
-                        show_label=False,
-                        enabled_when="pass_init_disabled",
-                    ),
-                    Item(
-                        name="button_ap_figures",
-                        label="Ap figures",
-                        show_label=False,
-                        enabled_when="pass_init_disabled",
-                    ),
-                    show_left=False,
-                ),
-                VGroup(
-                    Item(
-                        name="button_edit_cal_parameters",
-                        label="Edit calibration parameters",
-                        show_label=False,
-                    ),
-                    Item(
-                        name="button_edit_ori_files",
-                        label="Edit ori files",
-                        show_label=False,
-                    ),
-                    show_left=False,
-                ),
-            ),
-            Item(
-                "camera",
-                style="custom",
-                editor=ListEditor(
-                    use_notebook=True,
-                    deletable=False,
-                    dock_style="tab",
-                    page_name=".name",
-                ),
-                show_label=False,
-            ),
-            orientation="horizontal",
-        ),
-        title="Calibration",
-        id="view1",
-        width=1.0,
-        height=1.0,
-        resizable=True,
-        statusbar="status_text",
-    )
-
-    # --------------------------------------------------
-
-    def _button_edit_cal_parameters_fired(self):
-        cp = parameter_gui.Calib_Params(par_path=self.par_path)
-        cp.edit_traits(kind="modal")
-        # at the end of a modification, copy the parameters
-        par.copy_params_dir(self.par_path, self.active_path)
-        (
-            self.cpar,
-            self.spar,
-            self.vpar,
-            self.track_par,
-            self.tpar,
-            self.cals,
-            self.epar,
-        ) = ptv.py_start_proc_c(self.n_cams)
-
-    def _button_showimg_fired(self):
-
-        print("Loading images/parameters \n")
-
-        # Initialize what is needed, copy necessary things
-
-        print("\n Copying man_ori.dat \n")
-        if os.path.isfile(os.path.join(self.par_path, "man_ori.dat")):
-            shutil.copyfile(
-                os.path.join(self.par_path, "man_ori.dat"),
-                os.path.join(self.working_folder, "man_ori.dat"),
-            )
-            print("\n Copied man_ori.dat \n")
-
-        # copy parameters from active to default folder parameters/
-        par.copy_params_dir(self.active_path, self.par_path)
-
-        # read from parameters
-        (
-            self.cpar,
-            self.spar,
-            self.vpar,
-            self.track_par,
-            self.tpar,
-            self.cals,
-            self.epar,
-        ) = ptv.py_start_proc_c(self.n_cams)
-
-        self.tpar.read(b"parameters/detect_plate.par")
-
-        print(self.tpar.get_grey_thresholds())
-
-        self.calParams = par.CalOriParams(self.n_cams, self.par_path)
-        self.calParams.read()
-
-        if self.epar.Combine_Flag is True:
-            print("Combine Flag")
-            self.MultiParams = par.MultiPlaneParams()
-            self.MultiParams.read()
-            for i in range(self.MultiParams.n_planes):
-                print(self.MultiParams.plane_name[i])
-
-            self.pass_raw_orient = True
-            self.status_text = "Multiplane calibration."
-
-        # read calibration images
-        self.cal_images = []
-        for i in range(len(self.camera)):
-            imname = self.calParams.img_cal_name[i]
-            im = imread(imname)
-            # im = ImageData.fromfile(imname).data
-            if im.ndim > 2:
-                im = rgb2gray(im[:,:,:3])
-
-            self.cal_images.append(img_as_ubyte(im))
-
-        self.reset_show_images()
-
-        # Loading manual parameters here
-
-        f = open(os.path.join(self.par_path, "man_ori.par"), "r")
-        if f is None:
-            print("\n Error loading man_ori.par from parameters")
-        else:
-            for i in range(len(self.camera)):
-                for j in range(4):
-                    self.camera[i].man_ori[j] = int(f.readline().strip())
-        f.close()
-
-        self.pass_init = True
-        self.status_text = "Initialization finished."
-
-    def _button_detection_fired(self):
-        if self.need_reset:
-            self.reset_show_images()
-            self.need_reset = False
-        print(" Detection procedure \n")
-        self.status_text = "Detection procedure"
-
-        if self.cpar.get_hp_flag():
-            self.cal_images = ptv.py_pre_processing_c(
-                self.cal_images, self.cpar
-            )
-
-        self.detections, corrected = ptv.py_detection_proc_c(
-            self.cal_images, self.cpar, self.tpar, self.cals
-        )
-
-        x = [[i.pos()[0] for i in row] for row in self.detections]
-        y = [[i.pos()[1] for i in row] for row in self.detections]
-
-        self.drawcross("x", "y", x, y, "blue", 4)
-
-        for i in range(self.n_cams):
-            self.camera[i]._right_click_avail = 1
-
-    def _button_manual_fired(self):
-        print('Start manual orientation, use clicks and then press this button again')
-        points_set = True
-        for i in range(self.n_cams):
-            if len(self.camera[i]._x) < 4:
-                print(f"Camera {i} less than 4 points: {self.camera[i]._x}")
-                points_set = False
-            else:
-                print(f"Camera {i} has 4 points: {self.camera[i]._x}")
-
-        if points_set:
-            print(f'Manual orientation file is {man_ori_path}')
-            with open(self.man_ori_path, "w", encoding="utf-8") as f:
-                if f is None:
-                    self.status_text = "Error saving man_ori.dat."
-                else:
-                    for i in range(self.n_cams):
-                        for j in range(4):
-                            f.write(
-                                "%f %f\n"
-                                % (self.camera[i]._x[j], self.camera[i]._y[j])
-                            )
-
-                    self.status_text = "man_ori.dat saved."
-                    # f.close()
-        else:
-            self.status_text = (
-                "Click on 4 points on each calibration image for manual orientation"
-            )
-
-    def _button_file_orient_fired(self):
-        if self.need_reset:
-            self.reset_show_images()
-            self.need_reset = 0
-
-        
-        with open(self.man_ori_dat_path, "r") as f:
-            for i in range(self.n_cams):
-                self.camera[i]._x = []
-                self.camera[i]._y = []
-                for j in range(4):  # 4 orientation points
-                    line = f.readline().split()
-                    self.camera[i]._x.append(float(line[0]))
-                    self.camera[i]._y.append(float(line[1]))
-
-        self.status_text = "man_ori.dat loaded."
-        shutil.copyfile(
-            self.man_ori_dat_path, 
-            self.par_path / "man_ori.dat",
-            )
-
-        # TODO: rewrite using Parameters subclass
-        man_ori_par_path = os.path.join(self.par_path, "man_ori.par")
-        f = open(man_ori_par_path, "r")
-        if f is None:
-            self.status_text = "Error loading man_ori.par."
-        else:
-            for i in range(self.n_cams):
-                for j in range(4):
-                    self.camera[i].man_ori[j] = int(f.readline().split()[0])
-                self.status_text = "man_ori.par loaded."
-                self.camera[i].left_clicked_event()
-            f.close()
-
-        self.status_text = "Loading orientation data from file finished."
-
-    def _button_init_guess_fired(self):
-        if self.need_reset:
-            self.reset_show_images()
-            self.need_reset = 0
-
-        self.cal_points = self._read_cal_points()
-
-        self.cals = []
-        for i_cam in range(self.n_cams):
-            cal = Calibration()
-            tmp = self.cpar.get_cal_img_base_name(i_cam)
-            cal.from_file(tmp + b".ori", tmp + b".addpar")
-            self.cals.append(cal)
-
-        for i_cam in range(self.n_cams):
-            self._project_cal_points(i_cam)
-
-    def _project_cal_points(self, i_cam, color="yellow"):
-        x, y = [], []
-        for row in self.cal_points:
-            projected = image_coordinates(
-                np.atleast_2d(row["pos"]),
-                self.cals[i_cam],
-                self.cpar.get_multimedia_params(),
-            )
-            pos = convert_arr_metric_to_pixel(projected, self.cpar)
-
-            x.append(pos[0][0])
-            y.append(pos[0][1])
-
-        # x.append(x1)
-        # y.append(y1)
-        self.drawcross("init_x", "init_y", x, y, color, 3, i_cam=i_cam)
-        self.status_text = "Initial guess finished."
-
-    def _button_sort_grid_fired(self):
-        """
-        Uses sortgrid function of liboptv to match between the
-        calibration points in the fixp target file and the targets
-        detected in the images
-        """
-        if self.need_reset:
-            self.reset_show_images()
-            self.need_reset = 0
-
-        self.cal_points = self._read_cal_points()
-        self.sorted_targs = []
-
-        print("_button_sort_grid_fired")
-
-        for i_cam in range(self.n_cams):
-
-            # if len(self.cal_points) > len(self.detections[i_cam]):
-            #     raise ValueError("Insufficient detected points, need at \
-            #                       least as many as fixed points")
-
-            targs = match_detection_to_ref(
-                self.cals[i_cam],
-                self.cal_points["pos"],
-                self.detections[i_cam],
-                self.cpar,
-            )
-            x, y, pnr = [], [], []
-            for t in targs:
-                if t.pnr() != -999:
-                    pnr.append(self.cal_points["id"][t.pnr()])
-                    x.append(t.pos()[0])
-                    y.append(t.pos()[1])
-
-            self.sorted_targs.append(targs)
-            self.camera[i_cam]._plot.overlays = []
-            self.camera[i_cam].plot_num_overlay(x, y, pnr)
-
-        self.status_text = "Sort grid finished."
-        self.pass_sortgrid = True
-
-    # def _button_sort_grid_init_fired(self):
-    #     """ TODO: Not implemented yet """
-    #     if self.need_reset:
-    #         self.reset_show_images()
-    #         self.need_reset = 0
-    #
-    #
-    #     ptv.py_calibration(14)
-    #     x = []
-    #     y = []
-    #     x1_cyan = []
-    #     y1_cyan = []
-    #     pnr = []
-    #     ptv.py_get_from_sortgrid(x, y, pnr)
-    #     self.drawcross("sort_x_init", "sort_y_init", x, y, "white", 4)
-    #     ptv.py_get_from_calib(x1_cyan, y1_cyan)
-    #     self.drawcross("init_x", "init_y", x1_cyan, y1_cyan, "cyan", 4)
-    #     for i in range(len(self.camera)):
-    #         self.camera[i]._plot.overlays = []
-    #         self.camera[i].plot_num_overlay(x[i], y[i], pnr[i])
-    #     self.status_text = "Sort grid initial guess finished."
-
-    def _button_raw_orient_fired(self):
-        """
-        update the external calibration with results of raw orientation, i.e.
-        the iterative process that adjust the initial guess' external
-        parameters (position and angle of cameras) without internal or
-        distortions.
-
-        See: https://github.com/openptv/openptv/liboptv/src/orientation.c#L591
-        """
-        if self.need_reset:
-            self.reset_show_images()
-            self.need_reset = 0
-
-        # backup the ORI/ADDPAR files first
-        self.backup_ori_files()
-
-        # get manual points from cal_points and use ids from man_ori.par
-
-        for i_cam in range(self.n_cams):
-            selected_points = np.zeros((4, 3))
-            for i, cp_id in enumerate(self.cal_points["id"]):
-                for j in range(4):
-                    if cp_id == self.camera[i_cam].man_ori[j]:
-                        selected_points[j, :] = self.cal_points["pos"][i, :]
-                        continue
-
-            # in pixels:
-            manual_detection_points = np.array(
-                (self.camera[i_cam]._x, self.camera[i_cam]._y)
-            ).T
-
-            success = external_calibration(
-                self.cals[i_cam],
-                selected_points,
-                manual_detection_points,
-                self.cpar,
-            )
-
-            if success is False:
-                print("Initial guess has not been successful\n")
-            else:
-                self.camera[i_cam]._plot.overlays = []
-                self._project_cal_points(i_cam, color="red")
-                self._write_ori(i_cam)
-
-        self.status_text = "Orientation finished"
-        self.pass_raw_orient = True
-
-    def _button_fine_orient_fired(self):
-        """
-        fine tuning of ORI and ADDPAR
-
-        """
-        scale = 5000
-
-        if self.need_reset:
-            self.reset_show_images()
-            self.need_reset = 0
-
-        # backup the ORI/ADDPAR files first
-        self.backup_ori_files()
-
-        op = par.OrientParams()
-        op.read()
-
-        # recognized names for the flags:
-        names = [
-            "cc",
-            "xh",
-            "yh",
-            "k1",
-            "k2",
-            "k3",
-            "p1",
-            "p2",
-            "scale",
-            "shear",
-        ]
-        op_names = [
-            op.cc,
-            op.xh,
-            op.yh,
-            op.k1,
-            op.k2,
-            op.k3,
-            op.p1,
-            op.p2,
-            op.scale,
-            op.shear,
-        ]
-
-        flags = []
-        for name, op_name in zip(names, op_names):
-            if op_name == 1:
-                flags.append(name)
-
-        for i_cam in range(self.n_cams):  # iterate over all cameras
-
-            if self.epar.Combine_Flag:
-
-                self.status_text = "Multiplane calibration."
-                """ Performs multiplane calibration, in which for all cameras the
-                pre-processed planes in multi_plane.par combined.
-                Overwrites the ori and addpar files of the cameras specified
-                in cal_ori.par of the multiplane parameter folder
-                """
-
-                all_known = []
-                all_detected = []
-
-                for i in range(
-                    self.MultiParams.n_planes
-                ):  # combine all single planes
-
-                    # c = self.calParams.img_ori[i_cam][-9] # Get camera id
-                    # not all ends with a number
-                    c = re.findall("\\d+", self.calParams.img_ori[i_cam])[0]
-
-                    file_known = (
-                        self.MultiParams.plane_name[i] + c + ".tif.fix"
-                    )
-                    file_detected = (
-                        self.MultiParams.plane_name[i] + c + ".tif.crd"
-                    )
-
-                    # Load calibration point information from plane i
-                    try:
-                        known = np.loadtxt(file_known)
-                        detected = np.loadtxt(file_detected)
-                    except BaseException:
-                        raise IOError(
-                            "reading {} or {} failed".format(
-                                file_known, file_detected
-                            )
-                        )
-
-                    if np.any(detected == -999):
-                        raise ValueError(
-                            (
-                                "Using undetected points in {} will cause "
-                                + "silliness. Quitting."
-                            ).format(file_detected)
-                        )
-
-                    num_known = len(known)
-                    num_detect = len(detected)
-
-                    if num_known != num_detect:
-                        raise ValueError(
-                            f"Number of detected points {num_known} does not match"
-                            " number of known points {num_detect} for \
-                                {file_known}, {file_detected}")
-
-                    if len(all_known) > 0:
-                        detected[:, 0] = (
-                            all_detected[-1][-1, 0]
-                            + 1
-                            + np.arange(len(detected))
-                        )
-
-                    # Append to list of total known and detected points
-                    all_known.append(known)
-                    all_detected.append(detected)
-
-                # Make into the format needed for full_calibration.
-                all_known = np.vstack(all_known)[:, 1:]
-                all_detected = np.vstack(all_detected)
-
-                # this is the main difference in the multiplane mode
-                # that we fill the targs and cal_points by the
-                # combined information
-
-                targs = TargetArray(len(all_detected))
-                for tix in range(len(all_detected)):
-                    targ = targs[tix]
-                    det = all_detected[tix]
-
-                    targ.set_pnr(tix)
-                    targ.set_pos(det[1:])
-
-                self.cal_points = np.empty((all_known.shape[0],)).astype(
-                    dtype=[("id", "i4"), ("pos", "3f8")]
-                )
-                self.cal_points["pos"] = all_known
-            else:
-                targs = self.sorted_targs[i_cam]
-
-            try:
-                residuals, targ_ix, err_est = full_calibration(
-                    self.cals[i_cam],
-                    self.cal_points["pos"],
-                    targs,
-                    self.cpar,
-                    flags,
-                )
-            except BaseException as exc:
-                raise ValueError("full calibration failed\n") from exc
-            # save the results
-            self._write_ori(i_cam, addpar_flag=True)
-
-            # Plot the output
-            # self.reset_plots()
-
-            x, y = [], []
-            for r, t in zip(residuals, targ_ix):
-                if t != -999:
-                    pos = targs[t].pos()
-                    x.append(pos[0])
-                    y.append(pos[1])
-
-            self.camera[i_cam]._plot.overlays.clear()
-            self.drawcross(
-                "orient_x", "orient_y", x, y, "orange", 5, i_cam=i_cam
-            )
-
-            # self.camera[i]._plot_data.set_data(
-            #     'imagedata', self.ori_img[i].astype(np.float))
-            # self.camera[i]._img_plot = self.camera[
-            #     i]._plot.img_plot('imagedata', colormap=gray)[0]
-            self.camera[i_cam].drawquiver(
-                x,
-                y,
-                x + scale * residuals[: len(x), 0],
-                y + scale * residuals[: len(x), 1],
-                "red",
-            )
-            # self.camera[i]._plot.index_mapper.range.set_bounds(0, self.h_pixel)
-            # self.camera[i]._plot.value_mapper.range.set_bounds(0, self.v_pixel)
-
-        self.status_text = "Orientation finished."
-
-    def _write_ori(self, i_cam, addpar_flag=False):
-        """Writes ORI and ADDPAR files for a single calibration result
-        of i_cam
-        addpar_flag is a boolean that allows to keep previous addpar
-        otherwise external_calibration overwrites zeros
-        """
-
-        ori = self.calParams.img_ori[i_cam]
-        if addpar_flag:
-            addpar = ori.replace("ori", "addpar")
-        else:
-            addpar = "tmp.addpar"
-
-        print("Saving:", ori, addpar)
-        self.cals[i_cam].write(ori.encode(), addpar.encode())
-        if self.epar.Examine_Flag and not self.epar.Combine_Flag:
-            self.save_point_sets(i_cam)
-
-    def save_point_sets(self, i_cam):
-        """
-        Saves detected and known calibration points in crd and fix format, respectively.
-        These files are needed for multiplane calibration.
-        """
-
-        ori = self.calParams.img_ori[i_cam]
-        txt_detected = ori.replace("ori", "crd")
-        txt_matched = ori.replace("ori", "fix")
-
-        detected, known = [], []
-        targs = self.sorted_targs[i_cam]
-        for i, t in enumerate(targs):
-            if t.pnr() != -999:
-                detected.append(t.pos())
-                known.append(self.cal_points["pos"][i])
-        nums = np.arange(len(detected))
-        # for pnr in nums:
-        #     print(targs[pnr].pnr())
-        #     print(targs[pnr].pos())
-        #   detected[pnr] = targs[pnr].pos()
-
-        detected = np.hstack((nums[:, None], np.array(detected)))
-        known = np.hstack((nums[:, None], np.array(known)))
-
-        np.savetxt(txt_detected, detected, fmt="%9.5f")
-        np.savetxt(txt_matched, known, fmt="%10.5f")
-
-    def _button_orient_part_fired(self):
-
-        self.backup_ori_files()
-        ptv.py_calibration(10)
-        x1, y1, x2, y2 = [], [], [], []
-        ptv.py_get_from_orient(x1, y1, x2, y2)
-
-        self.reset_plots()
-        for i in range(len(self.camera)):
-            self.camera[i]._plot_data.set_data(
-                "imagedata", self.ori_img[i].astype(np.float)
-            )
-            self.camera[i]._img_plot = self.camera[i]._plot.img_plot(
-                "imagedata", colormap=gray
-            )[0]
-            self.camera[i].drawquiver(x1[i], y1[i], x2[i], y2[i], "red")
-            self.camera[i]._plot.index_mapper.range.set_bounds(0, self.h_pixel)
-            self.camera[i]._plot.value_mapper.range.set_bounds(0, self.v_pixel)
-            self.drawcross("orient_x", "orient_y", x1, y1, "orange", 4)
-
-        self.status_text = "Orientation with particles finished."
-
-    def _button_restore_orient_fired(self):
-        print("Restoring ORI files\n")
-        self.restore_ori_files()
-
-    def reset_plots(self):
-        for i in range(len(self.camera)):
-            self.camera[i]._plot.delplot(
-                *self.camera[i]._plot.plots.keys()[0:]
-            )
-            self.camera[i]._plot.overlays.clear()
-            # for j in range(len(self.camera[i]._quiverplots)):
-            #     self.camera[i]._plot.remove(self.camera[i]._quiverplots[j])
-            # self.camera[i]._quiverplots = []
-
-    def reset_show_images(self):
-        for i, cam in enumerate(self.camera):
-            cam._plot.delplot(*list(cam._plot.plots.keys())[0:])
-            cam._plot.overlays = []
-            # self.camera[i]._plot_data.set_data('imagedata',self.ori_img[i].astype(np.byte))
-            cam._plot_data.set_data(
-                "imagedata", self.cal_images[i].astype(np.uint8)
-            )
-
-            cam._img_plot = cam._plot.img_plot("imagedata", colormap=gray)[0]
-            cam._x = []
-            cam._y = []
-            cam._img_plot.tools = []
-            
-            # for j in range(len(cam._quiverplots)):
-            #     cam._plot.remove(cam._quiverplots[j])
-            # cam._quiverplots = []
-            
-            cam.attach_tools()
-            cam._plot.request_redraw()
-
-    def _button_edit_ori_files_fired(self):
-        editor = codeEditor(path=self.par_path)
-        editor.edit_traits(kind="livemodal")
-
-    def drawcross(self, str_x, str_y, x, y, color1, size1, i_cam=None):
-        """
-
-        :rtype: None
-        """
-        if i_cam is None:
-            for i in range(self.n_cams):
-                self.camera[i].drawcross(
-                    str_x, str_y, x[i], y[i], color1, size1
-                )
-        else:
-            self.camera[i_cam].drawcross(str_x, str_y, x, y, color1, size1)
-
-    def backup_ori_files(self):
-        """backup ORI/ADDPAR files to the backup_cal directory"""
-        calOriParams = par.CalOriParams(self.n_cams, path=self.par_path)
-        calOriParams.read()
-        for f in calOriParams.img_ori[: self.n_cams]:
-            print(f"Backing up {f}")
-            shutil.copyfile(f, f + ".bck")
-            g = f.replace("ori", "addpar")
-            shutil.copyfile(g, g + ".bck")
-
-    def restore_ori_files(self):
-        # backup ORI/ADDPAR files to the backup_cal directory
-        calOriParams = par.CalOriParams(self.n_cams, path=self.par_path)
-        calOriParams.read()
-
-        for f in calOriParams.img_ori[: self.n_cams]:
-            print(f"Restoring {f}")
-            shutil.copyfile(f + ".bck", f)
-            g = f.replace("ori", "addpar")
-            shutil.copyfile(g + ".bck", g)
-
-    def protect_ori_files(self):
-        # backup ORI/ADDPAR files to the backup_cal directory
-        calOriParams = par.CalOriParams(self.n_cams, path=self.par_path)
-        calOriParams.read()
-        for f in calOriParams.img_ori[: self.n_cams]:
-            with open(f, "r") as d:
-                d.read().split()
-                if not np.all(
-                    np.isfinite(np.asarray(d).astype("f"))
-                ):  # if there NaN for instance
-                    print("protected ORI file %s " % f)
-                    shutil.copyfile(f + ".bck", f)
-
-    # def update_plots(self, images):
-    #     for i in range(len(images)):
-    #         self.camera[i].update_image(images[i])
-
-    def _read_cal_points(self):
-        return np.atleast_1d(
-            np.loadtxt(
-                self.calParams.fixp_name,
-                dtype=[("id", "i4"), ("pos", "3f8")],
-                skiprows=0,
-            )
-        )
-
-
-if __name__ == "__main__":
-    import sys
-
-    if len(sys.argv) == 1:
-        active_path = Path("../test_cavity/parametersRun1")
-    else:
-        active_path = Path(sys.argv[0])
-
-    calib_gui = CalibrationGUI(active_path)
-    calib_gui.configure_traits()
+"""
+Copyright (c) 2008-2013, Tel Aviv University
+Copyright (c) 2013 - the OpenPTV team
+The software is distributed under the terms of MIT-like license
+http://opensource.org/licenses/MIT
+"""
+
+import os
+import shutil
+import re
+from  pathlib import Path
+import numpy as np
+from skimage.io import imread
+from skimage import img_as_ubyte
+from skimage.color import rgb2gray
+
+from traits.api import HasTraits, Str, Int, Bool, Instance, Button
+from traitsui.api import View, Item, HGroup, VGroup, ListEditor
+from enable.component_editor import ComponentEditor
+from chaco.api import (
+    Plot,
+    ArrayPlotData,
+    gray,
+    ArrayDataSource,
+    LinearMapper,
+)
+
+# from traitsui.menu import MenuBar, ToolBar, Menu, Action
+from chaco.tools.image_inspector_tool import ImageInspectorTool
+from chaco.tools.better_zoom import BetterZoom as SimpleZoom
+
+# from chaco.tools.simple_zoom import SimpleZoom
+from pyptv.text_box_overlay import TextBoxOverlay
+from pyptv.code_editor import codeEditor
+from pyptv.quiverplot import QuiverPlot
+
+
+
+from optv.imgcoord import image_coordinates
+from optv.transforms import convert_arr_metric_to_pixel
+from optv.orientation import match_detection_to_ref
+from optv.orientation import external_calibration, full_calibration
+from optv.calibration import Calibration
+from optv.tracking_framebuf import TargetArray
+
+
+from pyptv import ptv, parameter_gui, parameters as par
+
+
+# -------------------------------------------
+class ClickerTool(ImageInspectorTool):
+    left_changed = Int(1)
+    right_changed = Int(1)
+    x = 0
+    y = 0
+
+    def normal_left_down(self, event):
+        """Handles the left mouse button being clicked.
+        Fires the **new_value** event with the data (if any) from the event's
+        position.
+        """
+        plot = self.component
+        if plot is not None:
+            ndx = plot.map_index((event.x, event.y))
+
+            x_index, y_index = ndx
+            # image_data = plot.value
+            self.x = x_index
+            self.y = y_index
+            print(self.x)
+            print(self.y)
+            self.left_changed = 1 - self.left_changed
+            self.last_mouse_position = (event.x, event.y)
+
+    def normal_right_down(self, event):
+        plot = self.component
+        if plot is not None:
+            ndx = plot.map_index((event.x, event.y))
+
+            x_index, y_index = ndx
+            # image_data = plot.value
+            self.x = x_index
+            self.y = y_index
+
+            self.right_changed = 1 - self.right_changed
+            print(self.x)
+            print(self.y)
+
+            self.last_mouse_position = (event.x, event.y)
+
+    def normal_mouse_move(self, event):
+        pass
+
+    def __init__(self, *args, **kwargs):
+        super(ClickerTool, self).__init__(*args, **kwargs)
+
+
+# ----------------------------------------------------------
+
+
+class PlotWindow(HasTraits):
+    _plot = Instance(Plot)
+    _click_tool = Instance(ClickerTool)
+    _right_click_avail = 0
+    name = Str
+    view = View(
+        Item(name="_plot", editor=ComponentEditor(), show_label=False),
+    )
+
+    def __init__(self):
+        # super(HasTraits, self).__init__()
+        super().__init__()
+        # -------------- Initialization of plot system ----------------
+        padd = 25
+        self._plot_data = ArrayPlotData()
+        self._x, self._y = [], []
+        self.man_ori = [1, 2, 3, 4]
+        self._plot = Plot(self._plot_data, default_origin="top left")
+        self._plot.padding = (padd, padd, padd, padd)
+        # self._quiverplots = []
+
+        # -------------------------------------------------------------
+
+    def left_clicked_event(self):
+        print("left clicked")
+        if len(self._x) < 4:
+            self._x.append(self._click_tool.x)
+            self._y.append(self._click_tool.y)
+        print(self._x, self._y)
+
+        self.drawcross("coord_x", "coord_y", self._x, self._y, "red", 5)
+        self._plot.overlays.clear()
+        self.plot_num_overlay(self._x, self._y, self.man_ori)
+
+    def right_clicked_event(self):
+        print("right clicked")
+        if len(self._x) > 0:
+            self._x.pop()
+            self._y.pop()
+            print(self._x, self._y)
+
+            self.drawcross("coord_x", "coord_y", self._x, self._y, "red", 5)
+            self._plot.overlays.clear()
+            self.plot_num_overlay(self._x, self._y, self.man_ori)
+        else:
+            if self._right_click_avail:
+                print("deleting point")
+                self.py_rclick_delete(
+                    self._click_tool.x, self._click_tool.y, self.cameraN
+                )
+                x = []
+                y = []
+                self.py_get_pix_N(x, y, self.cameraN)
+                self.drawcross("x", "y", x[0], y[0], "blue", 4)
+
+    def attach_tools(self):
+        self._click_tool = ClickerTool(self._img_plot)
+        self._click_tool.on_trait_change(
+            self.left_clicked_event, "left_changed"
+        )
+        self._click_tool.on_trait_change(
+            self.right_clicked_event, "right_changed"
+        )
+        self._img_plot.tools.append(self._click_tool)
+        self._zoom_tool = SimpleZoom(
+            component=self._plot, tool_mode="box", always_on=False
+        )
+        self._zoom_tool.max_zoom_out_factor = 1.0
+        self._img_plot.tools.append(self._zoom_tool)
+        if self._plot.index_mapper is not None:
+            self._plot.index_mapper.on_trait_change(
+                self.handle_mapper, "updated", remove=False
+            )
+        if self._plot.value_mapper is not None:
+            self._plot.value_mapper.on_trait_change(
+                self.handle_mapper, "updated", remove=False
+            )
+
+    def drawcross(self, str_x, str_y, x, y, color1="blue", mrk_size=1, marker="plus"):
+        """
+        Draws crosses on images
+        """
+        self._plot_data.set_data(str_x, x)
+        self._plot_data.set_data(str_y, y)
+        self._plot.plot(
+            (str_x, str_y),
+            type="scatter",
+            color=color1,
+            marker=marker,
+            marker_size=mrk_size,
+        )
+        self._plot.request_redraw()
+
+    def drawline(self, str_x, str_y, x1, y1, x2, y2, color1):
+        self._plot_data.set_data(str_x, [x1, x2])
+        self._plot_data.set_data(str_y, [y1, y2])
+        self._plot.plot((str_x, str_y), type="line", color=color1)
+        self._plot.request_redraw()
+
+    def drawquiver(self, x1c, y1c, x2c, y2c, color, linewidth=1.0, scale=1.0):
+        """drawquiver draws multiple lines at once on the screen x1,y1->x2,y2 in the current camera window
+        parameters:
+            x1c - array of x1 coordinates
+            y1c - array of y1 coordinates
+            x2c - array of x2 coordinates
+            y2c - array of y2 coordinates
+            color - color of the line
+            linewidth - linewidth of the line
+        example usage:
+            drawquiver ([100,200],[100,100],[400,400],[300,200],'red',linewidth=2.0)
+            draws 2 red lines with thickness = 2 :  100,100->400,300 and 200,100->400,200
+
+        """
+        x1, y1, x2, y2 = self.remove_short_lines(
+            x1c, y1c, x2c, y2c, min_length=0
+        )
+        if len(x1) > 0:
+            xs = ArrayDataSource(x1)
+            ys = ArrayDataSource(y1)
+
+            # quiverplot = QuiverPlot(
+            #     index=xs,
+            #     value=ys,
+            #     index_mapper=LinearMapper(range=self._plot.index_mapper.range),
+            #     value_mapper=LinearMapper(range=self._plot.value_mapper.range),
+            #     origin=self._plot.origin,
+            #     arrow_size=0,
+            #     line_color=color,
+            #     line_width=linewidth,
+            #     ep_index=np.array(x2) * scale,
+            #     ep_value=np.array(y2) * scale,
+            # )
+            vectors = np.array(((np.array(x2)-np.array(x1))/scale, 
+                                (np.array(y2)-np.array(y1))/scale)).T
+            self._plot_data.set_data("index", x1)
+            self._plot_data.set_data("value", y1)
+            self._plot_data.set_data("vectors", vectors)
+            # self._quiverplots.append(quiverplot)
+            self._plot.quiverplot(
+                ('index','value','vectors'),
+                arrow_size=0,
+                line_color="red"
+                )
+            # self._plot.overlays.append(quiverplot)
+        
+    def remove_short_lines(self, x1, y1, x2, y2, min_length=2):
+        """removes short lines from the array of lines
+        parameters:
+            x1,y1,x2,y2 - start and end coordinates of the lines
+        returns:
+            x1f,y1f,x2f,y2f - start and end coordinates of the lines, with short lines removed
+        example usage:
+            x1,y1,x2,y2=remove_short_lines([100,200,300],[100,200,300],[100,200,300],[102,210,320])
+            3 input lines, 1 short line will be removed (100,100->100,102)
+            returned coordinates:
+            x1=[200,300]; y1=[200,300]; x2=[200,300]; y2=[210,320]
+        """
+        # dx, dy = 2, 2  # minimum allowable dx,dy
+        x1f, y1f, x2f, y2f = [], [], [], []
+        for i in range(len(x1)):
+            if (
+                abs(x1[i] - x2[i]) > min_length
+                or abs(y1[i] - y2[i]) > min_length
+            ):
+                x1f.append(x1[i])
+                y1f.append(y1[i])
+                x2f.append(x2[i])
+                y2f.append(y2[i])
+        return x1f, y1f, x2f, y2f
+
+    def handle_mapper(self):
+        for i in range(0, len(self._plot.overlays)):
+            if hasattr(self._plot.overlays[i], "real_position"):
+                coord_x1, coord_y1 = self._plot.map_screen(
+                    [self._plot.overlays[i].real_position]
+                )[0]
+                self._plot.overlays[i].alternate_position = (
+                    coord_x1,
+                    coord_y1,
+                )
+
+    def plot_num_overlay(self, x, y, txt):
+        for i in range(len(x)):
+            coord_x, coord_y = self._plot.map_screen([(x[i], y[i])])[0]
+            ovlay = TextBoxOverlay(
+                component=self._plot,
+                text=str(txt[i]),
+                alternate_position=(coord_x, coord_y),
+                real_position=(x[i], y[i]),
+                text_color="white",
+                border_color="red",
+            )
+            self._plot.overlays.append(ovlay)
+
+    def update_image(self, image, is_float):
+        if is_float:
+            self._plot_data.set_data("imagedata", image.astype(float))
+        else:
+            self._plot_data.set_data("imagedata", image.astype(np.uint8))
+            
+        # Alex added to plot the image here from update image
+        self._img_plt = self._plot.img_plot("imagedata", colormap=gray)[0]
+
+        self._plot.request_redraw()
+
+
+# ---------------------------------------------------------
+
+
+class CalibrationGUI(HasTraits):
+    status_text = Str("")
+    ori_img_name = []
+    ori_img = []
+    pass_init = Bool(False)
+    pass_sortgrid = Bool(False)
+    pass_raw_orient = Bool(False)
+    pass_init_disabled = Bool(False)
+    # -------------------------------------------------------------
+    button_edit_cal_parameters = Button()
+    button_showimg = Button()
+    button_detection = Button()
+    button_manual = Button()
+    button_file_orient = Button()
+    button_init_guess = Button()
+    button_sort_grid = Button()
+    button_sort_grid_init = Button()
+    button_raw_orient = Button()
+    button_fine_orient = Button()
+    button_orient_part = Button()
+    button_orient_shaking = Button()
+    button_orient_dumbbell = Button()
+    button_restore_orient = Button()
+    button_checkpoint = Button()
+    button_ap_figures = Button()
+    button_edit_ori_files = Button()
+    button_test = Button()
+
+    # ---------------------------------------------------
+    # Constructor
+    # ---------------------------------------------------
+    def __init__(self, active_path: Path):
+        """Initialize CalibrationGUI
+
+        Inputs:
+            active_path is the path to the folder of prameters
+            active_path is a subfolder of a working folder with a
+            structure of /parameters, /res, /cal, /img and so on
+        """
+
+        super(CalibrationGUI, self).__init__()
+        self.need_reset = 0
+
+        self.active_path = active_path
+        self.working_folder = self.active_path.parent
+        self.par_path = self.working_folder / "parameters"
+        
+        self.man_ori_dat_path = self.working_folder / "man_ori.dat"
+
+        print(" Copying parameters inside Calibration GUI: \n")
+        par.copy_params_dir(self.active_path, self.par_path)
+
+        
+        os.chdir(self.working_folder)
+        print(f"Inside a folder: {Path.cwd()}")
+        
+        # read parameters
+        with open(self.par_path / "ptv.par", "r") as f:
+            self.n_cams = int(f.readline())
+
+        self.camera = [PlotWindow() for i in range(self.n_cams)]
+        for i in range(self.n_cams):
+            self.camera[i].name = "Camera" + str(i + 1)
+            self.camera[i].cameraN = i
+            self.camera[i].py_rclick_delete = ptv.py_rclick_delete
+            self.camera[i].py_get_pix_N = ptv.py_get_pix_N
+
+    # Defines GUI view --------------------------
+
+    view = View(
+        HGroup(
+            VGroup(
+                VGroup(
+                    Item(
+                        name="button_showimg",
+                        label="Load/Show Images",
+                        show_label=False,
+                    ),
+                    Item(
+                        name="button_detection",
+                        label="Detection",
+                        show_label=False,
+                        enabled_when="pass_init",
+                    ),
+                    Item(
+                        name="button_manual",
+                        label="Manual orient.",
+                        show_label=False,
+                        enabled_when="pass_init",
+                    ),
+                    Item(
+                        name="button_file_orient",
+                        label="Orient. with file",
+                        show_label=False,
+                        enabled_when="pass_init",
+                    ),
+                    Item(
+                        name="button_init_guess",
+                        label="Show initial guess",
+                        show_label=False,
+                        enabled_when="pass_init",
+                    ),
+                    Item(
+                        name="button_sort_grid",
+                        label="Sortgrid",
+                        show_label=False,
+                        enabled_when="pass_init",
+                    ),
+                    # Item(name='button_sort_grid_init',
+                    # label='Sortgrid = initial guess',
+                    # show_label=False, enabled_when='pass_init'),
+                    Item(
+                        name="button_raw_orient",
+                        label="Raw orientation",
+                        show_label=False,
+                        enabled_when="pass_sortgrid",
+                    ),
+                    Item(
+                        name="button_fine_orient",
+                        label="Fine tuning",
+                        show_label=False,
+                        enabled_when="pass_raw_orient",
+                    ),
+                    Item(
+                        name="button_orient_part",
+                        label="Orientation with particles",
+                        show_label=False,
+                        enabled_when="pass_init",
+                    ),
+                    Item(
+                        name="button_orient_dumbbell",
+                        label="Orientation from dumbbell",
+                        show_label=False,
+                        enabled_when="pass_init",
+                    ),
+                    Item(
+                        name="button_restore_orient",
+                        label="Restore ori files",
+                        show_label=False,
+                        enabled_when="pass_init",
+                    ),
+                    Item(
+                        name="button_checkpoint",
+                        label="Checkpoints",
+                        show_label=False,
+                        enabled_when="pass_init_disabled",
+                    ),
+                    Item(
+                        name="button_ap_figures",
+                        label="Ap figures",
+                        show_label=False,
+                        enabled_when="pass_init_disabled",
+                    ),
+                    show_left=False,
+                ),
+                VGroup(
+                    Item(
+                        name="button_edit_cal_parameters",
+                        label="Edit calibration parameters",
+                        show_label=False,
+                    ),
+                    Item(
+                        name="button_edit_ori_files",
+                        label="Edit ori files",
+                        show_label=False,
+                    ),
+                    show_left=False,
+                ),
+            ),
+            Item(
+                "camera",
+                style="custom",
+                editor=ListEditor(
+                    use_notebook=True,
+                    deletable=False,
+                    dock_style="tab",
+                    page_name=".name",
+                ),
+                show_label=False,
+            ),
+            orientation="horizontal",
+        ),
+        title="Calibration",
+        id="view1",
+        width=1.0,
+        height=1.0,
+        resizable=True,
+        statusbar="status_text",
+    )
+
+    # --------------------------------------------------
+
+    def _button_edit_cal_parameters_fired(self):
+        cp = parameter_gui.Calib_Params(par_path=self.par_path)
+        cp.edit_traits(kind="modal")
+        # at the end of a modification, copy the parameters
+        par.copy_params_dir(self.par_path, self.active_path)
+        (
+            self.cpar,
+            self.spar,
+            self.vpar,
+            self.track_par,
+            self.tpar,
+            self.cals,
+            self.epar,
+        ) = ptv.py_start_proc_c(self.n_cams)
+
+    def _button_showimg_fired(self):
+
+        print("Loading images/parameters \n")
+
+        # Initialize what is needed, copy necessary things
+
+        print("\n Copying man_ori.dat \n")
+        if os.path.isfile(os.path.join(self.par_path, "man_ori.dat")):
+            shutil.copyfile(
+                os.path.join(self.par_path, "man_ori.dat"),
+                os.path.join(self.working_folder, "man_ori.dat"),
+            )
+            print("\n Copied man_ori.dat \n")
+
+        # copy parameters from active to default folder parameters/
+        par.copy_params_dir(self.active_path, self.par_path)
+
+        # read from parameters
+        (
+            self.cpar,
+            self.spar,
+            self.vpar,
+            self.track_par,
+            self.tpar,
+            self.cals,
+            self.epar,
+        ) = ptv.py_start_proc_c(self.n_cams)
+
+        self.tpar.read(b"parameters/detect_plate.par")
+
+        print(self.tpar.get_grey_thresholds())
+
+        self.calParams = par.CalOriParams(self.n_cams, self.par_path)
+        self.calParams.read()
+
+        if self.epar.Combine_Flag is True:
+            print("Combine Flag")
+            self.MultiParams = par.MultiPlaneParams()
+            self.MultiParams.read()
+            for i in range(self.MultiParams.n_planes):
+                print(self.MultiParams.plane_name[i])
+
+            self.pass_raw_orient = True
+            self.status_text = "Multiplane calibration."
+
+        # read calibration images
+        self.cal_images = []
+        for i in range(len(self.camera)):
+            imname = self.calParams.img_cal_name[i]
+            im = imread(imname)
+            # im = ImageData.fromfile(imname).data
+            if im.ndim > 2:
+                im = rgb2gray(im[:,:,:3])
+
+            self.cal_images.append(img_as_ubyte(im))
+
+        self.reset_show_images()
+
+        # Loading manual parameters here
+
+        f = open(os.path.join(self.par_path, "man_ori.par"), "r")
+        if f is None:
+            print("\n Error loading man_ori.par from parameters")
+        else:
+            for i in range(len(self.camera)):
+                for j in range(4):
+                    self.camera[i].man_ori[j] = int(f.readline().strip())
+        f.close()
+
+        self.pass_init = True
+        self.status_text = "Initialization finished."
+
+    def _button_detection_fired(self):
+        if self.need_reset:
+            self.reset_show_images()
+            self.need_reset = False
+        print(" Detection procedure \n")
+        self.status_text = "Detection procedure"
+
+        if self.cpar.get_hp_flag():
+            self.cal_images = ptv.py_pre_processing_c(
+                self.cal_images, self.cpar
+            )
+
+        self.detections, corrected = ptv.py_detection_proc_c(
+            self.cal_images, self.cpar, self.tpar, self.cals
+        )
+
+        x = [[i.pos()[0] for i in row] for row in self.detections]
+        y = [[i.pos()[1] for i in row] for row in self.detections]
+
+        self.drawcross("x", "y", x, y, "blue", 4)
+
+        for i in range(self.n_cams):
+            self.camera[i]._right_click_avail = 1
+
+    def _button_manual_fired(self):
+        print('Start manual orientation, use clicks and then press this button again')
+        points_set = True
+        for i in range(self.n_cams):
+            if len(self.camera[i]._x) < 4:
+                print(f"Camera {i} less than 4 points: {self.camera[i]._x}")
+                points_set = False
+            else:
+                print(f"Camera {i} has 4 points: {self.camera[i]._x}")
+
+        if points_set:
+            print(f'Manual orientation file is {man_ori_path}')
+            with open(self.man_ori_path, "w", encoding="utf-8") as f:
+                if f is None:
+                    self.status_text = "Error saving man_ori.dat."
+                else:
+                    for i in range(self.n_cams):
+                        for j in range(4):
+                            f.write(
+                                "%f %f\n"
+                                % (self.camera[i]._x[j], self.camera[i]._y[j])
+                            )
+
+                    self.status_text = "man_ori.dat saved."
+                    # f.close()
+        else:
+            self.status_text = (
+                "Click on 4 points on each calibration image for manual orientation"
+            )
+
+    def _button_file_orient_fired(self):
+        if self.need_reset:
+            self.reset_show_images()
+            self.need_reset = 0
+
+        
+        with open(self.man_ori_dat_path, "r") as f:
+            for i in range(self.n_cams):
+                self.camera[i]._x = []
+                self.camera[i]._y = []
+                for j in range(4):  # 4 orientation points
+                    line = f.readline().split()
+                    self.camera[i]._x.append(float(line[0]))
+                    self.camera[i]._y.append(float(line[1]))
+
+        self.status_text = "man_ori.dat loaded."
+        shutil.copyfile(
+            self.man_ori_dat_path, 
+            self.par_path / "man_ori.dat",
+            )
+
+        # TODO: rewrite using Parameters subclass
+        man_ori_par_path = os.path.join(self.par_path, "man_ori.par")
+        f = open(man_ori_par_path, "r")
+        if f is None:
+            self.status_text = "Error loading man_ori.par."
+        else:
+            for i in range(self.n_cams):
+                for j in range(4):
+                    self.camera[i].man_ori[j] = int(f.readline().split()[0])
+                self.status_text = "man_ori.par loaded."
+                self.camera[i].left_clicked_event()
+            f.close()
+
+        self.status_text = "Loading orientation data from file finished."
+
+    def _button_init_guess_fired(self):
+        if self.need_reset:
+            self.reset_show_images()
+            self.need_reset = 0
+
+        self.cal_points = self._read_cal_points()
+
+        self.cals = []
+        for i_cam in range(self.n_cams):
+            cal = Calibration()
+            tmp = self.cpar.get_cal_img_base_name(i_cam)
+            cal.from_file(tmp + b".ori", tmp + b".addpar")
+            self.cals.append(cal)
+
+        for i_cam in range(self.n_cams):
+            self._project_cal_points(i_cam)
+
+    def _project_cal_points(self, i_cam, color="yellow"):
+        x, y = [], []
+        for row in self.cal_points:
+            projected = image_coordinates(
+                np.atleast_2d(row["pos"]),
+                self.cals[i_cam],
+                self.cpar.get_multimedia_params(),
+            )
+            pos = convert_arr_metric_to_pixel(projected, self.cpar)
+
+            x.append(pos[0][0])
+            y.append(pos[0][1])
+
+        # x.append(x1)
+        # y.append(y1)
+        self.drawcross("init_x", "init_y", x, y, color, 3, i_cam=i_cam)
+        self.status_text = "Initial guess finished."
+
+    def _button_sort_grid_fired(self):
+        """
+        Uses sortgrid function of liboptv to match between the
+        calibration points in the fixp target file and the targets
+        detected in the images
+        """
+        if self.need_reset:
+            self.reset_show_images()
+            self.need_reset = 0
+
+        self.cal_points = self._read_cal_points()
+        self.sorted_targs = []
+
+        print("_button_sort_grid_fired")
+
+        for i_cam in range(self.n_cams):
+
+            # if len(self.cal_points) > len(self.detections[i_cam]):
+            #     raise ValueError("Insufficient detected points, need at \
+            #                       least as many as fixed points")
+
+            targs = match_detection_to_ref(
+                self.cals[i_cam],
+                self.cal_points["pos"],
+                self.detections[i_cam],
+                self.cpar,
+            )
+            x, y, pnr = [], [], []
+            for t in targs:
+                if t.pnr() != -999:
+                    pnr.append(self.cal_points["id"][t.pnr()])
+                    x.append(t.pos()[0])
+                    y.append(t.pos()[1])
+
+            self.sorted_targs.append(targs)
+            self.camera[i_cam]._plot.overlays = []
+            self.camera[i_cam].plot_num_overlay(x, y, pnr)
+
+        self.status_text = "Sort grid finished."
+        self.pass_sortgrid = True
+
+    # def _button_sort_grid_init_fired(self):
+    #     """ TODO: Not implemented yet """
+    #     if self.need_reset:
+    #         self.reset_show_images()
+    #         self.need_reset = 0
+    #
+    #
+    #     ptv.py_calibration(14)
+    #     x = []
+    #     y = []
+    #     x1_cyan = []
+    #     y1_cyan = []
+    #     pnr = []
+    #     ptv.py_get_from_sortgrid(x, y, pnr)
+    #     self.drawcross("sort_x_init", "sort_y_init", x, y, "white", 4)
+    #     ptv.py_get_from_calib(x1_cyan, y1_cyan)
+    #     self.drawcross("init_x", "init_y", x1_cyan, y1_cyan, "cyan", 4)
+    #     for i in range(len(self.camera)):
+    #         self.camera[i]._plot.overlays = []
+    #         self.camera[i].plot_num_overlay(x[i], y[i], pnr[i])
+    #     self.status_text = "Sort grid initial guess finished."
+
+    def _button_raw_orient_fired(self):
+        """
+        update the external calibration with results of raw orientation, i.e.
+        the iterative process that adjust the initial guess' external
+        parameters (position and angle of cameras) without internal or
+        distortions.
+
+        See: https://github.com/openptv/openptv/liboptv/src/orientation.c#L591
+        """
+        if self.need_reset:
+            self.reset_show_images()
+            self.need_reset = 0
+
+        # backup the ORI/ADDPAR files first
+        self.backup_ori_files()
+
+        # get manual points from cal_points and use ids from man_ori.par
+
+        for i_cam in range(self.n_cams):
+            selected_points = np.zeros((4, 3))
+            for i, cp_id in enumerate(self.cal_points["id"]):
+                for j in range(4):
+                    if cp_id == self.camera[i_cam].man_ori[j]:
+                        selected_points[j, :] = self.cal_points["pos"][i, :]
+                        continue
+
+            # in pixels:
+            manual_detection_points = np.array(
+                (self.camera[i_cam]._x, self.camera[i_cam]._y)
+            ).T
+
+            success = external_calibration(
+                self.cals[i_cam],
+                selected_points,
+                manual_detection_points,
+                self.cpar,
+            )
+
+            if success is False:
+                print("Initial guess has not been successful\n")
+            else:
+                self.camera[i_cam]._plot.overlays = []
+                self._project_cal_points(i_cam, color="red")
+                self._write_ori(i_cam)
+
+        self.status_text = "Orientation finished"
+        self.pass_raw_orient = True
+
+    def _button_fine_orient_fired(self):
+        """
+        fine tuning of ORI and ADDPAR
+
+        """
+        scale = 5000
+
+        if self.need_reset:
+            self.reset_show_images()
+            self.need_reset = 0
+
+        # backup the ORI/ADDPAR files first
+        self.backup_ori_files()
+
+        op = par.OrientParams()
+        op.read()
+
+        # recognized names for the flags:
+        names = [
+            "cc",
+            "xh",
+            "yh",
+            "k1",
+            "k2",
+            "k3",
+            "p1",
+            "p2",
+            "scale",
+            "shear",
+        ]
+        op_names = [
+            op.cc,
+            op.xh,
+            op.yh,
+            op.k1,
+            op.k2,
+            op.k3,
+            op.p1,
+            op.p2,
+            op.scale,
+            op.shear,
+        ]
+
+        flags = []
+        for name, op_name in zip(names, op_names):
+            if op_name == 1:
+                flags.append(name)
+
+        for i_cam in range(self.n_cams):  # iterate over all cameras
+
+            if self.epar.Combine_Flag:
+
+                self.status_text = "Multiplane calibration."
+                """ Performs multiplane calibration, in which for all cameras the
+                pre-processed planes in multi_plane.par combined.
+                Overwrites the ori and addpar files of the cameras specified
+                in cal_ori.par of the multiplane parameter folder
+                """
+
+                all_known = []
+                all_detected = []
+
+                for i in range(
+                    self.MultiParams.n_planes
+                ):  # combine all single planes
+
+                    # c = self.calParams.img_ori[i_cam][-9] # Get camera id
+                    # not all ends with a number
+                    c = re.findall("\\d+", self.calParams.img_ori[i_cam])[0]
+
+                    file_known = (
+                        self.MultiParams.plane_name[i] + c + ".tif.fix"
+                    )
+                    file_detected = (
+                        self.MultiParams.plane_name[i] + c + ".tif.crd"
+                    )
+
+                    # Load calibration point information from plane i
+                    try:
+                        known = np.loadtxt(file_known)
+                        detected = np.loadtxt(file_detected)
+                    except BaseException:
+                        raise IOError(
+                            "reading {} or {} failed".format(
+                                file_known, file_detected
+                            )
+                        )
+
+                    if np.any(detected == -999):
+                        raise ValueError(
+                            (
+                                "Using undetected points in {} will cause "
+                                + "silliness. Quitting."
+                            ).format(file_detected)
+                        )
+
+                    num_known = len(known)
+                    num_detect = len(detected)
+
+                    if num_known != num_detect:
+                        raise ValueError(
+                            f"Number of detected points {num_known} does not match"
+                            " number of known points {num_detect} for \
+                                {file_known}, {file_detected}")
+
+                    if len(all_known) > 0:
+                        detected[:, 0] = (
+                            all_detected[-1][-1, 0]
+                            + 1
+                            + np.arange(len(detected))
+                        )
+
+                    # Append to list of total known and detected points
+                    all_known.append(known)
+                    all_detected.append(detected)
+
+                # Make into the format needed for full_calibration.
+                all_known = np.vstack(all_known)[:, 1:]
+                all_detected = np.vstack(all_detected)
+
+                # this is the main difference in the multiplane mode
+                # that we fill the targs and cal_points by the
+                # combined information
+
+                targs = TargetArray(len(all_detected))
+                for tix in range(len(all_detected)):
+                    targ = targs[tix]
+                    det = all_detected[tix]
+
+                    targ.set_pnr(tix)
+                    targ.set_pos(det[1:])
+
+                self.cal_points = np.empty((all_known.shape[0],)).astype(
+                    dtype=[("id", "i4"), ("pos", "3f8")]
+                )
+                self.cal_points["pos"] = all_known
+            else:
+                targs = self.sorted_targs[i_cam]
+
+            try:
+                residuals, targ_ix, err_est = full_calibration(
+                    self.cals[i_cam],
+                    self.cal_points["pos"],
+                    targs,
+                    self.cpar,
+                    flags,
+                )
+            except BaseException as exc:
+                raise ValueError("full calibration failed\n") from exc
+            # save the results
+            self._write_ori(i_cam, addpar_flag=True)
+
+            # Plot the output
+            # self.reset_plots()
+
+            x, y = [], []
+            for r, t in zip(residuals, targ_ix):
+                if t != -999:
+                    pos = targs[t].pos()
+                    x.append(pos[0])
+                    y.append(pos[1])
+
+            self.camera[i_cam]._plot.overlays.clear()
+            self.drawcross(
+                "orient_x", "orient_y", x, y, "orange", 5, i_cam=i_cam
+            )
+
+            # self.camera[i]._plot_data.set_data(
+            #     'imagedata', self.ori_img[i].astype(np.float))
+            # self.camera[i]._img_plot = self.camera[
+            #     i]._plot.img_plot('imagedata', colormap=gray)[0]
+            self.camera[i_cam].drawquiver(
+                x,
+                y,
+                x + scale * residuals[: len(x), 0],
+                y + scale * residuals[: len(x), 1],
+                "red",
+            )
+            # self.camera[i]._plot.index_mapper.range.set_bounds(0, self.h_pixel)
+            # self.camera[i]._plot.value_mapper.range.set_bounds(0, self.v_pixel)
+
+        self.status_text = "Orientation finished."
+
+    def _write_ori(self, i_cam, addpar_flag=False):
+        """Writes ORI and ADDPAR files for a single calibration result
+        of i_cam
+        addpar_flag is a boolean that allows to keep previous addpar
+        otherwise external_calibration overwrites zeros
+        """
+
+        ori = self.calParams.img_ori[i_cam]
+        if addpar_flag:
+            addpar = ori.replace("ori", "addpar")
+        else:
+            addpar = "tmp.addpar"
+
+        print("Saving:", ori, addpar)
+        self.cals[i_cam].write(ori.encode(), addpar.encode())
+        if self.epar.Examine_Flag and not self.epar.Combine_Flag:
+            self.save_point_sets(i_cam)
+
+    def save_point_sets(self, i_cam):
+        """
+        Saves detected and known calibration points in crd and fix format, respectively.
+        These files are needed for multiplane calibration.
+        """
+
+        ori = self.calParams.img_ori[i_cam]
+        txt_detected = ori.replace("ori", "crd")
+        txt_matched = ori.replace("ori", "fix")
+
+        detected, known = [], []
+        targs = self.sorted_targs[i_cam]
+        for i, t in enumerate(targs):
+            if t.pnr() != -999:
+                detected.append(t.pos())
+                known.append(self.cal_points["pos"][i])
+        nums = np.arange(len(detected))
+        # for pnr in nums:
+        #     print(targs[pnr].pnr())
+        #     print(targs[pnr].pos())
+        #   detected[pnr] = targs[pnr].pos()
+
+        detected = np.hstack((nums[:, None], np.array(detected)))
+        known = np.hstack((nums[:, None], np.array(known)))
+
+        np.savetxt(txt_detected, detected, fmt="%9.5f")
+        np.savetxt(txt_matched, known, fmt="%10.5f")
+
+    def _button_orient_part_fired(self):
+
+        self.backup_ori_files()
+        ptv.py_calibration(10)
+        x1, y1, x2, y2 = [], [], [], []
+        ptv.py_get_from_orient(x1, y1, x2, y2)
+
+        self.reset_plots()
+        for i in range(len(self.camera)):
+            self.camera[i]._plot_data.set_data(
+                "imagedata", self.ori_img[i].astype(np.float)
+            )
+            self.camera[i]._img_plot = self.camera[i]._plot.img_plot(
+                "imagedata", colormap=gray
+            )[0]
+            self.camera[i].drawquiver(x1[i], y1[i], x2[i], y2[i], "red")
+            self.camera[i]._plot.index_mapper.range.set_bounds(0, self.h_pixel)
+            self.camera[i]._plot.value_mapper.range.set_bounds(0, self.v_pixel)
+            self.drawcross("orient_x", "orient_y", x1, y1, "orange", 4)
+
+        self.status_text = "Orientation with particles finished."
+
+    def _button_restore_orient_fired(self):
+        print("Restoring ORI files\n")
+        self.restore_ori_files()
+
+    def reset_plots(self):
+        for i in range(len(self.camera)):
+            self.camera[i]._plot.delplot(
+                *self.camera[i]._plot.plots.keys()[0:]
+            )
+            self.camera[i]._plot.overlays.clear()
+            # for j in range(len(self.camera[i]._quiverplots)):
+            #     self.camera[i]._plot.remove(self.camera[i]._quiverplots[j])
+            # self.camera[i]._quiverplots = []
+
+    def reset_show_images(self):
+        for i, cam in enumerate(self.camera):
+            cam._plot.delplot(*list(cam._plot.plots.keys())[0:])
+            cam._plot.overlays = []
+            # self.camera[i]._plot_data.set_data('imagedata',self.ori_img[i].astype(np.byte))
+            cam._plot_data.set_data(
+                "imagedata", self.cal_images[i].astype(np.uint8)
+            )
+
+            cam._img_plot = cam._plot.img_plot("imagedata", colormap=gray)[0]
+            cam._x = []
+            cam._y = []
+            cam._img_plot.tools = []
+            
+            # for j in range(len(cam._quiverplots)):
+            #     cam._plot.remove(cam._quiverplots[j])
+            # cam._quiverplots = []
+            
+            cam.attach_tools()
+            cam._plot.request_redraw()
+
+    def _button_edit_ori_files_fired(self):
+        editor = codeEditor(path=self.par_path)
+        editor.edit_traits(kind="livemodal")
+
+    def drawcross(self, str_x, str_y, x, y, color1, size1, i_cam=None):
+        """
+
+        :rtype: None
+        """
+        if i_cam is None:
+            for i in range(self.n_cams):
+                self.camera[i].drawcross(
+                    str_x, str_y, x[i], y[i], color1, size1
+                )
+        else:
+            self.camera[i_cam].drawcross(str_x, str_y, x, y, color1, size1)
+
+    def backup_ori_files(self):
+        """backup ORI/ADDPAR files to the backup_cal directory"""
+        calOriParams = par.CalOriParams(self.n_cams, path=self.par_path)
+        calOriParams.read()
+        for f in calOriParams.img_ori[: self.n_cams]:
+            print(f"Backing up {f}")
+            shutil.copyfile(f, f + ".bck")
+            g = f.replace("ori", "addpar")
+            shutil.copyfile(g, g + ".bck")
+
+    def restore_ori_files(self):
+        # backup ORI/ADDPAR files to the backup_cal directory
+        calOriParams = par.CalOriParams(self.n_cams, path=self.par_path)
+        calOriParams.read()
+
+        for f in calOriParams.img_ori[: self.n_cams]:
+            print(f"Restoring {f}")
+            shutil.copyfile(f + ".bck", f)
+            g = f.replace("ori", "addpar")
+            shutil.copyfile(g + ".bck", g)
+
+    def protect_ori_files(self):
+        # backup ORI/ADDPAR files to the backup_cal directory
+        calOriParams = par.CalOriParams(self.n_cams, path=self.par_path)
+        calOriParams.read()
+        for f in calOriParams.img_ori[: self.n_cams]:
+            with open(f, "r") as d:
+                d.read().split()
+                if not np.all(
+                    np.isfinite(np.asarray(d).astype("f"))
+                ):  # if there NaN for instance
+                    print("protected ORI file %s " % f)
+                    shutil.copyfile(f + ".bck", f)
+
+    # def update_plots(self, images):
+    #     for i in range(len(images)):
+    #         self.camera[i].update_image(images[i])
+
+    def _read_cal_points(self):
+        return np.atleast_1d(
+            np.loadtxt(
+                self.calParams.fixp_name,
+                dtype=[("id", "i4"), ("pos", "3f8")],
+                skiprows=0,
+            )
+        )
+
+
+if __name__ == "__main__":
+    import sys
+
+    if len(sys.argv) == 1:
+        active_path = Path("../test_cavity/parametersRun1")
+    else:
+        active_path = Path(sys.argv[0])
+
+    calib_gui = CalibrationGUI(active_path)
+    calib_gui.configure_traits()
```

### Comparing `pyptv-0.2.2/pyptv/detection_gui.py` & `pyptv-0.2.3/pyptv/detection_gui.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,542 +1,542 @@
-"""
-Copyright (c) 2008-2013, Tel Aviv University
-Copyright (c) 2013 - the OpenPTV team
-The GUI software is distributed under the terms of MIT-like license
-http://opensource.org/licenses/MIT
-"""
-
-import os
-import sys
-import pathlib
-import numpy as np
-
-from traits.api import HasTraits, Str, Int, Bool, Instance, Button, Range 
-from traitsui.api import View, Item, HGroup, VGroup, ListEditor
-from enable.component_editor import ComponentEditor
-from chaco.api import Plot, ArrayPlotData, gray, \
-    ImagePlot, ArrayDataSource, LinearMapper
-# from traitsui.menu import MenuBar, ToolBar, Menu, Action
-from chaco.tools.image_inspector_tool import ImageInspectorTool
-from chaco.tools.better_zoom import BetterZoom as SimpleZoom
-
-from skimage.io import imread
-from skimage import img_as_ubyte
-from skimage.color import rgb2gray
-
-# from optv import segmentation
-from optv.segmentation import target_recognition
-from pyptv import ptv
-
-from pyptv.text_box_overlay import TextBoxOverlay
-from pyptv.quiverplot import QuiverPlot
-
-
-
-# -------------------------------------------
-class ClickerTool(ImageInspectorTool):
-    left_changed = Int(1)
-    right_changed = Int(1)
-    x = 0
-    y = 0
-    
-    def __init__(self, *args, **kwargs):
-        super(ClickerTool, self).__init__(*args, **kwargs)
-
-    def normal_left_down(self, event):
-        """ Handles the left mouse button being clicked.
-        Fires the **new_value** event with the data (if any) from the event's
-        position.
-        """
-        plot = self.component
-        if plot is not None:
-            ndx = plot.map_index((event.x, event.y))
-
-            x_index, y_index = ndx
-            # image_data = plot.value
-            self.x = (x_index)
-            self.y = (y_index)
-            print(self.x)
-            print(self.y)
-            self.left_changed = 1 - self.left_changed
-            self.last_mouse_position = (event.x, event.y)
-
-    def normal_right_down(self, event):
-        plot = self.component
-        if plot is not None:
-            ndx = plot.map_index((event.x, event.y))
-
-            x_index, y_index = ndx
-            # image_data = plot.value
-            self.x = (x_index)
-            self.y = (y_index)
-
-            self.right_changed = 1 - self.right_changed
-            print(self.x)
-            print(self.y)
-
-            self.last_mouse_position = (event.x, event.y)
-
-    def normal_mouse_move(self, event):
-        pass
-
-
-
-
-# ----------------------------------------------------------
-
-class PlotWindow(HasTraits):
-    """ Plot window traits component """
-    _plot_data = Instance(ArrayPlotData)
-    _plot = Instance(Plot)
-    _click_tool = Instance(ClickerTool)
-    _img_plot = Instance(ImagePlot)
-    _right_click_avail = 0
-    name = Str
-    view = View(
-        Item(name='_plot', editor=ComponentEditor(), show_label=False),
-
-    )
-
-    def __init__(self):
-        super(HasTraits, self).__init__()
-        # -------------- Initialization of plot system ----------------
-        padd = 25
-        self._plot_data = ArrayPlotData()
-        self._x = []
-        self._y = []
-        self.man_ori = [1, 2, 3, 4]
-        self._plot = Plot(self._plot_data, default_origin="top left")
-        self._plot.padding_left = padd
-        self._plot.padding_right = padd
-        self._plot.padding_top = padd
-        self._plot.padding_bottom = padd
-        self._quiverplots = []
-        self.py_rclick_delete = ptv.py_rclick_delete
-        self.py_get_pix_N = ptv.py_get_pix_N
-
-        # -------------------------------------------------------------
-
-
-    def left_clicked_event(self):
-        """
-        Adds x,y position to a list and draws a cross
-
-        """
-        self._x.append(self._click_tool.x)
-        self._y.append(self._click_tool.y)
-        print(self._x, self._y)
-
-        self.drawcross("coord_x", "coord_y", self._x, self._y, "red", 5)
-        self._plot.overlays = []
-        self.plot_num_overlay(self._x, self._y, self.man_ori)
-
-    def right_clicked_event(self):
-        print ("right clicked")
-        if len(self._x) > 0:
-            self._x.pop()
-            self._y.pop()
-            print(self._x, self._y)
-
-            self.drawcross("coord_x", "coord_y", self._x, self._y, "red", 5)
-            self._plot.overlays = []
-            self.plot_num_overlay(self._x, self._y, self.man_ori)
-        else:
-            if (self._right_click_avail):
-                print("deleting point")
-                self.py_rclick_delete(self._click_tool.x,
-                                      self._click_tool.y, self.cameraN)
-                x = []
-                y = []
-                self.py_get_pix_N(x, y, self.cameraN)
-                self.drawcross("x", "y", x[0], y[0], "blue", 4)
-
-    def attach_tools(self):
-        self._click_tool = ClickerTool(self._img_plot)
-        self._click_tool.on_trait_change(
-            self.left_clicked_event, 'left_changed')
-        self._click_tool.on_trait_change(
-            self.right_clicked_event, 'right_changed')
-        self._img_plot.tools.append(self._click_tool)
-        self._zoom_tool = SimpleZoom(
-            component=self._plot, tool_mode="box", always_on=False)
-        self._zoom_tool.max_zoom_out_factor = 1.0
-        self._img_plot.tools.append(self._zoom_tool)
-        if self._plot.index_mapper is not None:
-            self._plot.index_mapper.on_trait_change(
-                self.handle_mapper, 'updated', remove=False)
-        if self._plot.value_mapper is not None:
-            self._plot.value_mapper.on_trait_change(
-                self.handle_mapper, 'updated', remove=False)
-
-    def drawcross(self, str_x, str_y, x, y, color1, mrk_size, marker="plus"):
-        """
-        Draws crosses on images
-        """
-        # self._plot.plotdata = ArrayPlotData(x=x[0], y=y[0])
-        self._plot_data.set_data(str_x, x)
-        self._plot_data.set_data(str_y, y)
-        self._plot.plot((str_x, str_y), type="scatter",
-                        color=color1, marker=marker, marker_size=mrk_size)
-        self._plot.request_redraw()
-
-    def drawline(self, str_x, str_y, x1, y1, x2, y2, color1):
-        self._plot_data.set_data(str_x, [x1, x2])
-        self._plot_data.set_data(str_y, [y1, y2])
-        self._plot.plot((str_x, str_y), type="line", color=color1)
-        self._plot.request_redraw()
-
-    def drawquiver(self, x1c, y1c, x2c, y2c, color, linewidth=1.0, scale=1.0):
-        """ drawquiver draws multiple lines at once on the screen x1,y1->x2,y2 in the current camera window
-        parameters:
-            x1c - array of x1 coordinates
-            y1c - array of y1 coordinates
-            x2c - array of x2 coordinates
-            y2c - array of y2 coordinates
-            color - color of the line
-            linewidth - linewidth of the line
-        example usage:
-            drawquiver ([100,200],[100,100],[400,400],[300,200],'red',linewidth=2.0)
-            draws 2 red lines with thickness = 2 :  100,100->400,300 and 200,100->400,200
-
-        """
-        x1, y1, x2, y2 = self.remove_short_lines(x1c, y1c, x2c, y2c, min_length=0)
-        if len(x1) > 0:
-            xs = ArrayDataSource(x1)
-            ys = ArrayDataSource(y1)
-
-            quiverplot = QuiverPlot(index=xs, value=ys,
-                                    index_mapper=LinearMapper(
-                                        range=self._plot.index_mapper.range),
-                                    value_mapper=LinearMapper(
-                                        range=self._plot.value_mapper.range),
-                                    origin=self._plot.origin, arrow_size=0,
-                                    line_color=color, line_width=linewidth,
-                                    ep_index=np.array(x2) * scale,
-                                    ep_value=np.array(y2) * scale
-                                    )
-            self._plot.add(quiverplot)
-            # we need this to track how many quiverplots are in the current
-            # plot
-            self._quiverplots.append(quiverplot)
-            # import pdb; pdb.set_trace()
-
-    def remove_short_lines(self, x1, y1, x2, y2, min_length=2):
-        """ removes short lines from the array of lines
-        parameters:
-            x1,y1,x2,y2 - start and end coordinates of the lines
-        returns:
-            x1f,y1f,x2f,y2f - start and end coordinates of the lines, with short lines removed
-        example usage:
-            x1,y1,x2,y2=remove_short_lines([100,200,300],[100,200,300],[100,200,300],[102,210,320])
-            3 input lines, 1 short line will be removed (100,100->100,102)
-            returned coordinates:
-            x1=[200,300]; y1=[200,300]; x2=[200,300]; y2=[210,320]
-        """
-        # dx, dy = 2, 2  # minimum allowable dx,dy
-        x1f, y1f, x2f, y2f = [], [], [], []
-        for i in range(len(x1)):
-            if abs(x1[i] - x2[i]) > min_length or abs(y1[i] - y2[i]) > min_length:
-                x1f.append(x1[i])
-                y1f.append(y1[i])
-                x2f.append(x2[i])
-                y2f.append(y2[i])
-        return x1f, y1f, x2f, y2f
-
-    def handle_mapper(self):
-        for i in range(0, len(self._plot.overlays)):
-            if hasattr(self._plot.overlays[i], 'real_position'):
-                coord_x1, coord_y1 = self._plot.map_screen(
-                    [self._plot.overlays[i].real_position])[0]
-                self._plot.overlays[i].alternate_position = (
-                    coord_x1, coord_y1)
-
-    def plot_num_overlay(self, x, y, txt):
-        for i in range(0, len(x)):
-            coord_x, coord_y = self._plot.map_screen([(x[i], y[i])])[0]
-            ovlay = TextBoxOverlay(component=self._plot,
-                                   text=str(txt[i]), alternate_position=(coord_x, coord_y),
-                                   real_position=(x[i], y[i]),
-                                   text_color="white",
-                                   border_color="red"
-                                   )
-            self._plot.overlays.append(ovlay)
-
-    def update_image(self, image, is_float=False):
-        if is_float:
-            self._plot_data.set_data('imagedata', image.astype(np.float))
-        else:
-            self._plot_data.set_data('imagedata', image.astype(np.byte))
-
-        self._plot.request_redraw()
-
-
-# ---------------------------------------------------------
-
-
-class DetectionGUI(HasTraits):
-    """ detection GUI """
-    status_text = Str(" status ")
-    # -------------------------------------------------------------
-    
-    # grey_thresh= Range(1,255,5,mode='slider')
-
-    size_of_crosses = Int(4, label='Size of crosses')
-    # button_edit_cal_parameters = Button()
-    button_showimg = Button(label='Load image')
-    hp_flag = Bool(False,label='highpass')
-    inverse_flag = Bool(False, label='inverse')
-    button_detection = Button(label='Detect dots')
-    image_name = Str("cal/cam1.tif", label="Image file name")
-
-    # ---------------------------------------------------
-    # Constructor
-    # ---------------------------------------------------
-    def __init__(self, par_path: pathlib.Path):
-        """ Initialize DetectionGUI
-
-            Inputs:
-                active_path is the path to the folder of prameters
-                active_path is a subfolder of a working folder with a
-                structure of /parameters, /res, /cal, /img and so on
-        """
-
-        super(DetectionGUI, self).__init__()
-        self.need_reset = 0
-
-        # self.active_path = active_path
-        print(f'par_path is {par_path}')
-        if not isinstance(par_path, pathlib.Path):
-            par_path = pathlib.Path(par_path)
-            
-        self.par_path = par_path
-        self.working_folder = self.par_path.parent
-        # self.par_path = os.path.join(self.working_folder, 'parameters')
-
-        # print('active path = %s' % self.active_path)
-        print(f'working_folder = {self.working_folder}')
-        print(f'par_path = {self.par_path}')
-
-
-
-
-        # par.copy_params_dir(self.active_path, self.par_path)
-        os.chdir(self.working_folder)
-        print(f"Inside a folder: {pathlib.Path()}")
-        # read parameters
-        with open( (self.par_path / 'ptv.par'), 'r', encoding="utf-8") as f:
-            self.n_cams = int(f.readline())
-
-        print(f"Loading images/parameters in {self.n_cams} cams \n")
-
-        # copy parameters from active to default folder parameters/
-        # par.copy_params_dir(self.active_path, self.par_path)
-
-        # read from parameters
-        self.cpar, self.spar, self.vpar, self.track_par, self.tpar, \
-        self.cals, self.epar = ptv.py_start_proc_c(self.n_cams)
-
-        self.tpar.read(b'parameters/detect_plate.par')
-
-        self.thresholds = self.tpar.get_grey_thresholds()
-        self.pixel_count_bounds = list(self.tpar.get_pixel_count_bounds())
-        self.xsize_bounds = list(self.tpar.get_xsize_bounds())
-        self.ysize_bounds = list(self.tpar.get_ysize_bounds())
-        self.sum_grey = self.tpar.get_min_sum_grey()
-
-        # self.add_trait("i_cam", Enum(range(1,self.n_cams+1))) 
-        self.add_trait("grey_thresh", Range(1,255,self.thresholds[0],mode='slider'))
-        self.add_trait("min_npix",Range(0,self.pixel_count_bounds[0]+50, self.pixel_count_bounds[0], method='slider',label='min npix'))
-        self.add_trait("min_npix_x",Range(1,self.xsize_bounds[0]+20,self.xsize_bounds[0], mode='slider',label='min npix in x')) 
-        self.add_trait("min_npix_y", Range(1,self.ysize_bounds[0]+20,self.ysize_bounds[0], mode='slider',label='min npix in y'))
-        self.add_trait("max_npix", Range(1,self.pixel_count_bounds[1]+100,self.pixel_count_bounds[1], mode='slider',label='max npix'))
-        self.add_trait("max_npix_x", Range(1,self.xsize_bounds[1]+50,self.xsize_bounds[1], mode='slider',label='max npix in x'))
-        self.add_trait("max_npix_y", Range(1,self.ysize_bounds[1]+50,self.ysize_bounds[1], mode='slider',label='max npix in y'))
-        self.add_trait("sum_of_grey", Range(self.sum_grey/2,self.sum_grey*2,self.sum_grey, mode='slider',label='Sum of greyvalue'))
-
-
-        # Detection will work one by one for the beginning
-        self.camera = [PlotWindow()]
-        # self.camera_name = 'Camera' + str(self.i_cam)
-        
-
-    # Defines GUI view --------------------------
-
-    view = View(
-        HGroup(
-            VGroup(
-                VGroup(
-                    # Item(name='i_cam'),
-                    Item(name="image_name", width=150),
-                    Item(name='button_showimg'),
-                    Item(name='hp_flag'),
-                    Item(name='inverse_flag'),
-                    Item(name='button_detection'),
-                    Item(name='grey_thresh'),
-                    Item(name='min_npix'),
-                    Item(name='min_npix_x'),
-                    Item(name='min_npix_y'),
-                    Item(name='max_npix'),
-                    Item(name='max_npix_x'),
-                    Item(name='max_npix_y'),
-                    Item(name='sum_of_grey'),
-                    ),
-            ),
-            Item('camera', style='custom',
-                 editor=ListEditor(use_notebook=True,
-                                   deletable=False,
-                                   dock_style='tab',
-                                   page_name='.name',
-                                   ),
-                 show_label=False
-                 ),
-
-            orientation='horizontal'
-        ),
-        title='Detection',
-        id='view1',
-        width=1.,
-        height=1.,
-        resizable=True,
-        statusbar='status_text'
-    )
-
-    # --------------------------------------------------
-
-    def _inverse_flag_changed(self):
-        self._read_cal_image()
-        self.status_text = "Negative image"
-        self.reset_show_images()
-
-    def _hp_flag_changed(self):
-        self._read_cal_image()
-        self.status_text = "Highpassed image"
-        self.reset_show_images()
-
-
-    def _grey_thresh_changed(self):
-        self.thresholds[0] = self.grey_thresh
-        self.tpar.set_grey_thresholds(self.thresholds)
-        # print(f"tpar is now {self.tpar.get_grey_thresholds()}")
-        # run detection again
-        self._button_detection_fired()
-
-    def _min_npix_changed(self):
-        self.pixel_count_bounds[0] = self.min_npix
-        self.tpar.set_pixel_count_bounds(self.pixel_count_bounds)
-        # print(f"set min {self.tpar.get_pixel_count_bounds()}")
-        self._button_detection_fired()
-
-    def _max_npix_changed(self):
-        self.pixel_count_bounds[1] = self.max_npix
-        self.tpar.set_pixel_count_bounds(self.pixel_count_bounds)
-        # print(f"set max {self.tpar.get_pixel_count_bounds()}")
-        self._button_detection_fired()
-
-    def _min_npix_x_changed(self):
-        self.xsize_bounds[0] = self.min_npix_x
-        self.tpar.set_xsize_bounds(self.xsize_bounds)
-        self._button_detection_fired()
-
-    def _max_npix_x_changed(self):
-        self.xsize_bounds[1] = self.max_npix_x
-        self.tpar.set_xsize_bounds(self.xsize_bounds)
-        self._button_detection_fired()
-
-    def _min_npix_y_changed(self):
-        self.ysize_bounds[0] = self.min_npix_y
-        self.tpar.set_ysize_bounds(self.ysize_bounds)
-        # self._button_detection_fired()
-
-    def _max_npix_y_changed(self):
-        self.ysize_bounds[1] = self.max_npix_y
-        self.tpar.set_ysize_bounds(self.ysize_bounds)
-        self._button_detection_fired()
-
-    def _sum_of_grey_changed(self):
-        self.tpar.set_min_sum_grey(self.sum_of_grey)
-        self._button_detection_fired()
-
-
-    def _button_showimg_fired(self):
-        self._read_cal_image()
-        self.reset_show_images()
-
-    def _read_cal_image(self):
-        # read Detection images
-        # imname = self.cpar.get_cal_img_base_name(self.i_cam-1)
-        #         
-        # print(f'image name is {self.image_name}')# and \
-            #its string is {self.image_name.decode("utf-8")}')
-
-        im = imread(self.image_name)
-        # print(f'image size is {im.shape}')
-        if im.ndim > 2:
-            im = rgb2gray(im)
-        
-        if self.inverse_flag is True:
-            im = 255 - im
-            
-        if self.hp_flag is True:
-            tmp = [img_as_ubyte(im)]
-            tmp = ptv.py_pre_processing_c(tmp, self.cpar)
-            im = tmp[0]
-        else:
-            im = img_as_ubyte(im)
-            
-        self.cal_image = im.copy()       
-
-
-    def _button_detection_fired(self):
-        # self.reset_show_images()
-        # self.need_reset = False
-        self.status_text = " Detection procedure "
-
-        # self.detections, corrected = \
-        #     ptv.py_detection_proc_c([self.cal_image], self.cpar, self.tpar, self.cals)
-
-        targs = target_recognition(self.cal_image, self.tpar, 0, self.cpar)
-        targs.sort_y()
-
-        x = [i.pos()[0] for i in targs]
-        y = [i.pos()[1] for i in targs]
-
-        # print("n particles is %d " % len(x))
-
-        self.camera[0].drawcross("x", "y", np.array(x), np.array(y), "yellow", 8)
-        self.camera[0]._right_click_avail = 1
-
-        # for i in range(self.n_cams):
-        #     self.camera[i]._right_click_avail = 1
-
-    def reset_plots(self):
-        """ Resets all the images and overlays """
-        self.camera[0]._plot.delplot(*self.camera[0]._plot.plots.keys())
-        self.camera[0]._plot.overlays = []
-        for j in range(len(self.camera[0]._quiverplots)):
-            self.camera[0]._plot.remove(self.camera[0]._quiverplots[j])
-        self.camera[0]._quiverplots = []
-
-    def reset_show_images(self):
-        self.reset_plots()
-        self.camera[0]._plot_data.set_data('imagedata', self.cal_image)
-        self.camera[0]._img_plot = self.camera[0]._plot.img_plot('imagedata', colormap=gray)[0]
-        self.camera[0]._x = []
-        self.camera[0]._y = []
-        self.camera[0]._img_plot.tools = []
-        self.camera[0].attach_tools()
-        self.camera[0]._plot.request_redraw()
-
-
-    # def update_plots(self, images, is_float=False):
-    #     self.camera[0].update_image(self.cal_image, is_float)
-
-if __name__ == "__main__":
-
-    if len(sys.argv) == 1:
-        par_path = pathlib.Path().absolute() / 'tests' / 'test_cavity' / 'parameters'
-        # par_path = pathlib.Path('/home/user/Downloads/Test_8_with_50_pic/parameters')
-    else:
-        par_path = pathlib.Path(sys.argv[1]) / 'parameters'
-
-    detection_gui = DetectionGUI(par_path)
-    detection_gui.configure_traits()
+"""
+Copyright (c) 2008-2013, Tel Aviv University
+Copyright (c) 2013 - the OpenPTV team
+The GUI software is distributed under the terms of MIT-like license
+http://opensource.org/licenses/MIT
+"""
+
+import os
+import sys
+import pathlib
+import numpy as np
+
+from traits.api import HasTraits, Str, Int, Bool, Instance, Button, Range 
+from traitsui.api import View, Item, HGroup, VGroup, ListEditor
+from enable.component_editor import ComponentEditor
+from chaco.api import Plot, ArrayPlotData, gray, \
+    ImagePlot, ArrayDataSource, LinearMapper
+# from traitsui.menu import MenuBar, ToolBar, Menu, Action
+from chaco.tools.image_inspector_tool import ImageInspectorTool
+from chaco.tools.better_zoom import BetterZoom as SimpleZoom
+
+from skimage.io import imread
+from skimage import img_as_ubyte
+from skimage.color import rgb2gray
+
+# from optv import segmentation
+from optv.segmentation import target_recognition
+from pyptv import ptv
+
+from pyptv.text_box_overlay import TextBoxOverlay
+from pyptv.quiverplot import QuiverPlot
+
+
+
+# -------------------------------------------
+class ClickerTool(ImageInspectorTool):
+    left_changed = Int(1)
+    right_changed = Int(1)
+    x = 0
+    y = 0
+    
+    def __init__(self, *args, **kwargs):
+        super(ClickerTool, self).__init__(*args, **kwargs)
+
+    def normal_left_down(self, event):
+        """ Handles the left mouse button being clicked.
+        Fires the **new_value** event with the data (if any) from the event's
+        position.
+        """
+        plot = self.component
+        if plot is not None:
+            ndx = plot.map_index((event.x, event.y))
+
+            x_index, y_index = ndx
+            # image_data = plot.value
+            self.x = (x_index)
+            self.y = (y_index)
+            print(self.x)
+            print(self.y)
+            self.left_changed = 1 - self.left_changed
+            self.last_mouse_position = (event.x, event.y)
+
+    def normal_right_down(self, event):
+        plot = self.component
+        if plot is not None:
+            ndx = plot.map_index((event.x, event.y))
+
+            x_index, y_index = ndx
+            # image_data = plot.value
+            self.x = (x_index)
+            self.y = (y_index)
+
+            self.right_changed = 1 - self.right_changed
+            print(self.x)
+            print(self.y)
+
+            self.last_mouse_position = (event.x, event.y)
+
+    def normal_mouse_move(self, event):
+        pass
+
+
+
+
+# ----------------------------------------------------------
+
+class PlotWindow(HasTraits):
+    """ Plot window traits component """
+    _plot_data = Instance(ArrayPlotData)
+    _plot = Instance(Plot)
+    _click_tool = Instance(ClickerTool)
+    _img_plot = Instance(ImagePlot)
+    _right_click_avail = 0
+    name = Str
+    view = View(
+        Item(name='_plot', editor=ComponentEditor(), show_label=False),
+
+    )
+
+    def __init__(self):
+        super(HasTraits, self).__init__()
+        # -------------- Initialization of plot system ----------------
+        padd = 25
+        self._plot_data = ArrayPlotData()
+        self._x = []
+        self._y = []
+        self.man_ori = [1, 2, 3, 4]
+        self._plot = Plot(self._plot_data, default_origin="top left")
+        self._plot.padding_left = padd
+        self._plot.padding_right = padd
+        self._plot.padding_top = padd
+        self._plot.padding_bottom = padd
+        self._quiverplots = []
+        self.py_rclick_delete = ptv.py_rclick_delete
+        self.py_get_pix_N = ptv.py_get_pix_N
+
+        # -------------------------------------------------------------
+
+
+    def left_clicked_event(self):
+        """
+        Adds x,y position to a list and draws a cross
+
+        """
+        self._x.append(self._click_tool.x)
+        self._y.append(self._click_tool.y)
+        print(self._x, self._y)
+
+        self.drawcross("coord_x", "coord_y", self._x, self._y, "red", 5)
+        self._plot.overlays = []
+        self.plot_num_overlay(self._x, self._y, self.man_ori)
+
+    def right_clicked_event(self):
+        print ("right clicked")
+        if len(self._x) > 0:
+            self._x.pop()
+            self._y.pop()
+            print(self._x, self._y)
+
+            self.drawcross("coord_x", "coord_y", self._x, self._y, "red", 5)
+            self._plot.overlays = []
+            self.plot_num_overlay(self._x, self._y, self.man_ori)
+        else:
+            if (self._right_click_avail):
+                print("deleting point")
+                self.py_rclick_delete(self._click_tool.x,
+                                      self._click_tool.y, self.cameraN)
+                x = []
+                y = []
+                self.py_get_pix_N(x, y, self.cameraN)
+                self.drawcross("x", "y", x[0], y[0], "blue", 4)
+
+    def attach_tools(self):
+        self._click_tool = ClickerTool(self._img_plot)
+        self._click_tool.on_trait_change(
+            self.left_clicked_event, 'left_changed')
+        self._click_tool.on_trait_change(
+            self.right_clicked_event, 'right_changed')
+        self._img_plot.tools.append(self._click_tool)
+        self._zoom_tool = SimpleZoom(
+            component=self._plot, tool_mode="box", always_on=False)
+        self._zoom_tool.max_zoom_out_factor = 1.0
+        self._img_plot.tools.append(self._zoom_tool)
+        if self._plot.index_mapper is not None:
+            self._plot.index_mapper.on_trait_change(
+                self.handle_mapper, 'updated', remove=False)
+        if self._plot.value_mapper is not None:
+            self._plot.value_mapper.on_trait_change(
+                self.handle_mapper, 'updated', remove=False)
+
+    def drawcross(self, str_x, str_y, x, y, color1, mrk_size, marker="plus"):
+        """
+        Draws crosses on images
+        """
+        # self._plot.plotdata = ArrayPlotData(x=x[0], y=y[0])
+        self._plot_data.set_data(str_x, x)
+        self._plot_data.set_data(str_y, y)
+        self._plot.plot((str_x, str_y), type="scatter",
+                        color=color1, marker=marker, marker_size=mrk_size)
+        self._plot.request_redraw()
+
+    def drawline(self, str_x, str_y, x1, y1, x2, y2, color1):
+        self._plot_data.set_data(str_x, [x1, x2])
+        self._plot_data.set_data(str_y, [y1, y2])
+        self._plot.plot((str_x, str_y), type="line", color=color1)
+        self._plot.request_redraw()
+
+    def drawquiver(self, x1c, y1c, x2c, y2c, color, linewidth=1.0, scale=1.0):
+        """ drawquiver draws multiple lines at once on the screen x1,y1->x2,y2 in the current camera window
+        parameters:
+            x1c - array of x1 coordinates
+            y1c - array of y1 coordinates
+            x2c - array of x2 coordinates
+            y2c - array of y2 coordinates
+            color - color of the line
+            linewidth - linewidth of the line
+        example usage:
+            drawquiver ([100,200],[100,100],[400,400],[300,200],'red',linewidth=2.0)
+            draws 2 red lines with thickness = 2 :  100,100->400,300 and 200,100->400,200
+
+        """
+        x1, y1, x2, y2 = self.remove_short_lines(x1c, y1c, x2c, y2c, min_length=0)
+        if len(x1) > 0:
+            xs = ArrayDataSource(x1)
+            ys = ArrayDataSource(y1)
+
+            quiverplot = QuiverPlot(index=xs, value=ys,
+                                    index_mapper=LinearMapper(
+                                        range=self._plot.index_mapper.range),
+                                    value_mapper=LinearMapper(
+                                        range=self._plot.value_mapper.range),
+                                    origin=self._plot.origin, arrow_size=0,
+                                    line_color=color, line_width=linewidth,
+                                    ep_index=np.array(x2) * scale,
+                                    ep_value=np.array(y2) * scale
+                                    )
+            self._plot.add(quiverplot)
+            # we need this to track how many quiverplots are in the current
+            # plot
+            self._quiverplots.append(quiverplot)
+            # import pdb; pdb.set_trace()
+
+    def remove_short_lines(self, x1, y1, x2, y2, min_length=2):
+        """ removes short lines from the array of lines
+        parameters:
+            x1,y1,x2,y2 - start and end coordinates of the lines
+        returns:
+            x1f,y1f,x2f,y2f - start and end coordinates of the lines, with short lines removed
+        example usage:
+            x1,y1,x2,y2=remove_short_lines([100,200,300],[100,200,300],[100,200,300],[102,210,320])
+            3 input lines, 1 short line will be removed (100,100->100,102)
+            returned coordinates:
+            x1=[200,300]; y1=[200,300]; x2=[200,300]; y2=[210,320]
+        """
+        # dx, dy = 2, 2  # minimum allowable dx,dy
+        x1f, y1f, x2f, y2f = [], [], [], []
+        for i in range(len(x1)):
+            if abs(x1[i] - x2[i]) > min_length or abs(y1[i] - y2[i]) > min_length:
+                x1f.append(x1[i])
+                y1f.append(y1[i])
+                x2f.append(x2[i])
+                y2f.append(y2[i])
+        return x1f, y1f, x2f, y2f
+
+    def handle_mapper(self):
+        for i in range(0, len(self._plot.overlays)):
+            if hasattr(self._plot.overlays[i], 'real_position'):
+                coord_x1, coord_y1 = self._plot.map_screen(
+                    [self._plot.overlays[i].real_position])[0]
+                self._plot.overlays[i].alternate_position = (
+                    coord_x1, coord_y1)
+
+    def plot_num_overlay(self, x, y, txt):
+        for i in range(0, len(x)):
+            coord_x, coord_y = self._plot.map_screen([(x[i], y[i])])[0]
+            ovlay = TextBoxOverlay(component=self._plot,
+                                   text=str(txt[i]), alternate_position=(coord_x, coord_y),
+                                   real_position=(x[i], y[i]),
+                                   text_color="white",
+                                   border_color="red"
+                                   )
+            self._plot.overlays.append(ovlay)
+
+    def update_image(self, image, is_float=False):
+        if is_float:
+            self._plot_data.set_data('imagedata', image.astype(np.float))
+        else:
+            self._plot_data.set_data('imagedata', image.astype(np.byte))
+
+        self._plot.request_redraw()
+
+
+# ---------------------------------------------------------
+
+
+class DetectionGUI(HasTraits):
+    """ detection GUI """
+    status_text = Str(" status ")
+    # -------------------------------------------------------------
+    
+    # grey_thresh= Range(1,255,5,mode='slider')
+
+    size_of_crosses = Int(4, label='Size of crosses')
+    # button_edit_cal_parameters = Button()
+    button_showimg = Button(label='Load image')
+    hp_flag = Bool(False,label='highpass')
+    inverse_flag = Bool(False, label='inverse')
+    button_detection = Button(label='Detect dots')
+    image_name = Str("cal/cam1.tif", label="Image file name")
+
+    # ---------------------------------------------------
+    # Constructor
+    # ---------------------------------------------------
+    def __init__(self, par_path: pathlib.Path):
+        """ Initialize DetectionGUI
+
+            Inputs:
+                active_path is the path to the folder of prameters
+                active_path is a subfolder of a working folder with a
+                structure of /parameters, /res, /cal, /img and so on
+        """
+
+        super(DetectionGUI, self).__init__()
+        self.need_reset = 0
+
+        # self.active_path = active_path
+        print(f'par_path is {par_path}')
+        if not isinstance(par_path, pathlib.Path):
+            par_path = pathlib.Path(par_path)
+            
+        self.par_path = par_path
+        self.working_folder = self.par_path.parent
+        # self.par_path = os.path.join(self.working_folder, 'parameters')
+
+        # print('active path = %s' % self.active_path)
+        print(f'working_folder = {self.working_folder}')
+        print(f'par_path = {self.par_path}')
+
+
+
+
+        # par.copy_params_dir(self.active_path, self.par_path)
+        os.chdir(self.working_folder)
+        print(f"Inside a folder: {pathlib.Path()}")
+        # read parameters
+        with open( (self.par_path / 'ptv.par'), 'r', encoding="utf-8") as f:
+            self.n_cams = int(f.readline())
+
+        print(f"Loading images/parameters in {self.n_cams} cams \n")
+
+        # copy parameters from active to default folder parameters/
+        # par.copy_params_dir(self.active_path, self.par_path)
+
+        # read from parameters
+        self.cpar, self.spar, self.vpar, self.track_par, self.tpar, \
+        self.cals, self.epar = ptv.py_start_proc_c(self.n_cams)
+
+        self.tpar.read(b'parameters/detect_plate.par')
+
+        self.thresholds = self.tpar.get_grey_thresholds()
+        self.pixel_count_bounds = list(self.tpar.get_pixel_count_bounds())
+        self.xsize_bounds = list(self.tpar.get_xsize_bounds())
+        self.ysize_bounds = list(self.tpar.get_ysize_bounds())
+        self.sum_grey = self.tpar.get_min_sum_grey()
+
+        # self.add_trait("i_cam", Enum(range(1,self.n_cams+1))) 
+        self.add_trait("grey_thresh", Range(1,255,self.thresholds[0],mode='slider'))
+        self.add_trait("min_npix",Range(0,self.pixel_count_bounds[0]+50, self.pixel_count_bounds[0], method='slider',label='min npix'))
+        self.add_trait("min_npix_x",Range(1,self.xsize_bounds[0]+20,self.xsize_bounds[0], mode='slider',label='min npix in x')) 
+        self.add_trait("min_npix_y", Range(1,self.ysize_bounds[0]+20,self.ysize_bounds[0], mode='slider',label='min npix in y'))
+        self.add_trait("max_npix", Range(1,self.pixel_count_bounds[1]+100,self.pixel_count_bounds[1], mode='slider',label='max npix'))
+        self.add_trait("max_npix_x", Range(1,self.xsize_bounds[1]+50,self.xsize_bounds[1], mode='slider',label='max npix in x'))
+        self.add_trait("max_npix_y", Range(1,self.ysize_bounds[1]+50,self.ysize_bounds[1], mode='slider',label='max npix in y'))
+        self.add_trait("sum_of_grey", Range(self.sum_grey/2,self.sum_grey*2,self.sum_grey, mode='slider',label='Sum of greyvalue'))
+
+
+        # Detection will work one by one for the beginning
+        self.camera = [PlotWindow()]
+        # self.camera_name = 'Camera' + str(self.i_cam)
+        
+
+    # Defines GUI view --------------------------
+
+    view = View(
+        HGroup(
+            VGroup(
+                VGroup(
+                    # Item(name='i_cam'),
+                    Item(name="image_name", width=150),
+                    Item(name='button_showimg'),
+                    Item(name='hp_flag'),
+                    Item(name='inverse_flag'),
+                    Item(name='button_detection'),
+                    Item(name='grey_thresh'),
+                    Item(name='min_npix'),
+                    Item(name='min_npix_x'),
+                    Item(name='min_npix_y'),
+                    Item(name='max_npix'),
+                    Item(name='max_npix_x'),
+                    Item(name='max_npix_y'),
+                    Item(name='sum_of_grey'),
+                    ),
+            ),
+            Item('camera', style='custom',
+                 editor=ListEditor(use_notebook=True,
+                                   deletable=False,
+                                   dock_style='tab',
+                                   page_name='.name',
+                                   ),
+                 show_label=False
+                 ),
+
+            orientation='horizontal'
+        ),
+        title='Detection',
+        id='view1',
+        width=1.,
+        height=1.,
+        resizable=True,
+        statusbar='status_text'
+    )
+
+    # --------------------------------------------------
+
+    def _inverse_flag_changed(self):
+        self._read_cal_image()
+        self.status_text = "Negative image"
+        self.reset_show_images()
+
+    def _hp_flag_changed(self):
+        self._read_cal_image()
+        self.status_text = "Highpassed image"
+        self.reset_show_images()
+
+
+    def _grey_thresh_changed(self):
+        self.thresholds[0] = self.grey_thresh
+        self.tpar.set_grey_thresholds(self.thresholds)
+        # print(f"tpar is now {self.tpar.get_grey_thresholds()}")
+        # run detection again
+        self._button_detection_fired()
+
+    def _min_npix_changed(self):
+        self.pixel_count_bounds[0] = self.min_npix
+        self.tpar.set_pixel_count_bounds(self.pixel_count_bounds)
+        # print(f"set min {self.tpar.get_pixel_count_bounds()}")
+        self._button_detection_fired()
+
+    def _max_npix_changed(self):
+        self.pixel_count_bounds[1] = self.max_npix
+        self.tpar.set_pixel_count_bounds(self.pixel_count_bounds)
+        # print(f"set max {self.tpar.get_pixel_count_bounds()}")
+        self._button_detection_fired()
+
+    def _min_npix_x_changed(self):
+        self.xsize_bounds[0] = self.min_npix_x
+        self.tpar.set_xsize_bounds(self.xsize_bounds)
+        self._button_detection_fired()
+
+    def _max_npix_x_changed(self):
+        self.xsize_bounds[1] = self.max_npix_x
+        self.tpar.set_xsize_bounds(self.xsize_bounds)
+        self._button_detection_fired()
+
+    def _min_npix_y_changed(self):
+        self.ysize_bounds[0] = self.min_npix_y
+        self.tpar.set_ysize_bounds(self.ysize_bounds)
+        # self._button_detection_fired()
+
+    def _max_npix_y_changed(self):
+        self.ysize_bounds[1] = self.max_npix_y
+        self.tpar.set_ysize_bounds(self.ysize_bounds)
+        self._button_detection_fired()
+
+    def _sum_of_grey_changed(self):
+        self.tpar.set_min_sum_grey(self.sum_of_grey)
+        self._button_detection_fired()
+
+
+    def _button_showimg_fired(self):
+        self._read_cal_image()
+        self.reset_show_images()
+
+    def _read_cal_image(self):
+        # read Detection images
+        # imname = self.cpar.get_cal_img_base_name(self.i_cam-1)
+        #         
+        # print(f'image name is {self.image_name}')# and \
+            #its string is {self.image_name.decode("utf-8")}')
+
+        im = imread(self.image_name)
+        # print(f'image size is {im.shape}')
+        if im.ndim > 2:
+            im = rgb2gray(im)
+        
+        if self.inverse_flag is True:
+            im = 255 - im
+            
+        if self.hp_flag is True:
+            tmp = [img_as_ubyte(im)]
+            tmp = ptv.py_pre_processing_c(tmp, self.cpar)
+            im = tmp[0]
+        else:
+            im = img_as_ubyte(im)
+            
+        self.cal_image = im.copy()       
+
+
+    def _button_detection_fired(self):
+        # self.reset_show_images()
+        # self.need_reset = False
+        self.status_text = " Detection procedure "
+
+        # self.detections, corrected = \
+        #     ptv.py_detection_proc_c([self.cal_image], self.cpar, self.tpar, self.cals)
+
+        targs = target_recognition(self.cal_image, self.tpar, 0, self.cpar)
+        targs.sort_y()
+
+        x = [i.pos()[0] for i in targs]
+        y = [i.pos()[1] for i in targs]
+
+        # print("n particles is %d " % len(x))
+
+        self.camera[0].drawcross("x", "y", np.array(x), np.array(y), "yellow", 8)
+        self.camera[0]._right_click_avail = 1
+
+        # for i in range(self.n_cams):
+        #     self.camera[i]._right_click_avail = 1
+
+    def reset_plots(self):
+        """ Resets all the images and overlays """
+        self.camera[0]._plot.delplot(*self.camera[0]._plot.plots.keys())
+        self.camera[0]._plot.overlays = []
+        for j in range(len(self.camera[0]._quiverplots)):
+            self.camera[0]._plot.remove(self.camera[0]._quiverplots[j])
+        self.camera[0]._quiverplots = []
+
+    def reset_show_images(self):
+        self.reset_plots()
+        self.camera[0]._plot_data.set_data('imagedata', self.cal_image)
+        self.camera[0]._img_plot = self.camera[0]._plot.img_plot('imagedata', colormap=gray)[0]
+        self.camera[0]._x = []
+        self.camera[0]._y = []
+        self.camera[0]._img_plot.tools = []
+        self.camera[0].attach_tools()
+        self.camera[0]._plot.request_redraw()
+
+
+    # def update_plots(self, images, is_float=False):
+    #     self.camera[0].update_image(self.cal_image, is_float)
+
+if __name__ == "__main__":
+
+    if len(sys.argv) == 1:
+        par_path = pathlib.Path().absolute() / 'tests' / 'test_cavity' / 'parameters'
+        # par_path = pathlib.Path('/home/user/Downloads/Test_8_with_50_pic/parameters')
+    else:
+        par_path = pathlib.Path(sys.argv[1]) / 'parameters'
+
+    detection_gui = DetectionGUI(par_path)
+    detection_gui.configure_traits()
```

### Comparing `pyptv-0.2.2/pyptv/directory_editor.py` & `pyptv-0.2.3/pyptv/directory_editor.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-#!/usr/bin/pythonw
-"""
-Implementation of a DirectoryEditor demo plugin for Traits UI demo program.
-This demo shows each of the four styles of the DirectoryEditor
-"""
-# Imports:
-from traits.api import HasTraits, Directory
-
-from traitsui.api import Item, View
-
-# Define the demo class:
-
-
-class DirectoryEditorDialog(HasTraits):
-    """Define the main DirectoryEditor demo class."""
-
-    # Define a Directory trait to view:
-    dir_name = Directory
-    # Display specification (one Item per editor style):
-    dir_item = Item("dir_name", style="simple", label="Simple")
-    # Demo view:
-    view = View(
-        dir_item,
-        title="Choose the experimental directory",
-        buttons=["OK"],
-        width=0.5,
-        resizable=True,
-        kind="modal",
-    )
-
-
-# Create the demo:
-# demo = DirectoryEditorDemo()
-# Run the demo (if invoked from the command line):
-# if __name__ == '__main__':
-# 	demo.configure_traits()
+#!/usr/bin/pythonw
+"""
+Implementation of a DirectoryEditor demo plugin for Traits UI demo program.
+This demo shows each of the four styles of the DirectoryEditor
+"""
+# Imports:
+from traits.api import HasTraits, Directory
+
+from traitsui.api import Item, View
+
+# Define the demo class:
+
+
+class DirectoryEditorDialog(HasTraits):
+    """Define the main DirectoryEditor demo class."""
+
+    # Define a Directory trait to view:
+    dir_name = Directory
+    # Display specification (one Item per editor style):
+    dir_item = Item("dir_name", style="simple", label="Simple")
+    # Demo view:
+    view = View(
+        dir_item,
+        title="Choose the experimental directory",
+        buttons=["OK"],
+        width=0.5,
+        resizable=True,
+        kind="modal",
+    )
+
+
+# Create the demo:
+# demo = DirectoryEditorDemo()
+# Run the demo (if invoked from the command line):
+# if __name__ == '__main__':
+# 	demo.configure_traits()
```

### Comparing `pyptv-0.2.2/pyptv/draw_3d_target.py` & `pyptv-0.2.3/pyptv/draw_3d_target.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-# How to run:
-# python .\draw_3d_target.py .\cal\pyramide_target.txt
-
-
-import numpy as np
-import matplotlib.pyplot as plt
-# %matplotlib tk
-
-# %%
-# filename = '../cal/small_target_cam2.txt'
-def plot_3d_target(filename):
-    d = np.loadtxt(filename)
-
-    # %%
-    from mpl_toolkits.mplot3d import Axes3D
-    ax = plt.figure(figsize=(12,10)).add_subplot(projection='3d')
-
-    # 
-    for row in d:
-        ax.plot(row[1],row[2],row[3],'ro')
-        ax.text(row[1],row[2],row[3],f'{row[0]:.0f}',None)
-
-    ax.set_xlim(d[:,1].min(),d[:,1].max())
-    ax.set_ylim(d[:,2].min(),d[:,2].max())
-    ax.set_zlim(d[:,3].min(),d[:,3].max())
-
-    ax.set_xlabel('x')
-    ax.set_ylabel('y')
-    ax.set_zlabel('z')
-    ax.set_title(filename.split('/')[-1])
-
-    plt.show()
-
-if __name__ == "__main__":
-    import sys
-    plot_3d_target(sys.argv[1])
-
-
+# How to run:
+# python .\draw_3d_target.py .\cal\pyramide_target.txt
+
+
+import numpy as np
+import matplotlib.pyplot as plt
+# %matplotlib tk
+
+# %%
+# filename = '../cal/small_target_cam2.txt'
+def plot_3d_target(filename):
+    d = np.loadtxt(filename)
+
+    # %%
+    from mpl_toolkits.mplot3d import Axes3D
+    ax = plt.figure(figsize=(12,10)).add_subplot(projection='3d')
+
+    # 
+    for row in d:
+        ax.plot(row[1],row[2],row[3],'ro')
+        ax.text(row[1],row[2],row[3],f'{row[0]:.0f}',None)
+
+    ax.set_xlim(d[:,1].min(),d[:,1].max())
+    ax.set_ylim(d[:,2].min(),d[:,2].max())
+    ax.set_zlim(d[:,3].min(),d[:,3].max())
+
+    ax.set_xlabel('x')
+    ax.set_ylabel('y')
+    ax.set_zlabel('z')
+    ax.set_title(filename.split('/')[-1])
+
+    plt.show()
+
+if __name__ == "__main__":
+    import sys
+    plot_3d_target(sys.argv[1])
+
+
```

### Comparing `pyptv-0.2.2/pyptv/ext_sequence_denis.py` & `pyptv-0.2.3/pyptv/ext_sequence_denis.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,73 +1,73 @@
-import random
-
-import numpy as np
-from skimage.io import imread
-
-
-class Sequence:
-    """Sequence class defines external tracking addon for pyptv
-    User needs to implement the following functions:
-            do_sequence(self)
-
-    Connection to C ptv module is given via self.ptv and provided by pyptv software
-    Connection to active parameters is given via self.exp1 and provided by pyptv software.
-
-    User responsibility is to read necessary files, make the calculations and write the files back.
-    """
-
-    def __init__(self, ptv=None, exp1=None, camera_list=None):
-        self.ptv = ptv
-        self.exp1 = exp1
-        self.camera_list = camera_list
-        # Do your initialization here
-
-    def do_sequence(self):
-        """this function is callback for "tracking without display" """
-        print("inside denis_ext_sequence")
-        n_camera = self.exp1.active_params.m_params.Num_Cam
-        print("Starting sequence action")
-        seq_first = self.exp1.active_params.m_params.Seq_First
-        seq_last = self.exp1.active_params.m_params.Seq_Last
-        print(seq_first, seq_last)
-        base_name = []
-        for i in range(n_camera):
-            exec(
-                "base_name.append(self.exp1.active_params.m_params.Basename_%d_Seq)" %
-                (i + 1))
-            print(base_name[i])
-
-        self.ptv.py_sequence_init(0)  # init C sequence function
-        # get parameters and pass to main loop
-        stepshake = self.ptv.py_get_from_sequence_init()
-        if not stepshake:
-            stepshake = 1
-        print(stepshake)
-        temp_img = np.array([], dtype=np.ubyte)
-        # main loop - format image name, read it and call
-        # v.py_sequence_loop(..) for current step
-        for i in range(seq_first, seq_last + 1, stepshake):
-            if i < 10:
-                seq_ch = "%01d" % i
-            elif i < 100:
-                seq_ch = "%02d" % i
-            else:
-                seq_ch = "%03d" % i
-            for j in range(n_camera):
-                img_name = base_name[j] + seq_ch
-                # print("Setting image: ", img_name)
-                try:
-                    temp_img = imread(img_name).astype(np.ubyte)
-                except BaseException:
-                    print("Error reading file")
-
-                self.ptv.py_set_img(temp_img, j)
-            self.ptv.py_sequence_loop(0, i)
-            self.camera_list[0].drawquiver(
-                [int(300 * random.random())],
-                [int(300 * random.random())],
-                [int(300 * random.random())],
-                [int(300 * random.random())],
-                "green",
-                linewidth=3.0,
-            )
-            self.camera_list[0]._plot.request_redraw()
+import random
+
+import numpy as np
+from skimage.io import imread
+
+
+class Sequence:
+    """Sequence class defines external tracking addon for pyptv
+    User needs to implement the following functions:
+            do_sequence(self)
+
+    Connection to C ptv module is given via self.ptv and provided by pyptv software
+    Connection to active parameters is given via self.exp1 and provided by pyptv software.
+
+    User responsibility is to read necessary files, make the calculations and write the files back.
+    """
+
+    def __init__(self, ptv=None, exp1=None, camera_list=None):
+        self.ptv = ptv
+        self.exp1 = exp1
+        self.camera_list = camera_list
+        # Do your initialization here
+
+    def do_sequence(self):
+        """this function is callback for "tracking without display" """
+        print("inside denis_ext_sequence")
+        n_camera = self.exp1.active_params.m_params.Num_Cam
+        print("Starting sequence action")
+        seq_first = self.exp1.active_params.m_params.Seq_First
+        seq_last = self.exp1.active_params.m_params.Seq_Last
+        print(seq_first, seq_last)
+        base_name = []
+        for i in range(n_camera):
+            exec(
+                "base_name.append(self.exp1.active_params.m_params.Basename_%d_Seq)" %
+                (i + 1))
+            print(base_name[i])
+
+        self.ptv.py_sequence_init(0)  # init C sequence function
+        # get parameters and pass to main loop
+        stepshake = self.ptv.py_get_from_sequence_init()
+        if not stepshake:
+            stepshake = 1
+        print(stepshake)
+        temp_img = np.array([], dtype=np.ubyte)
+        # main loop - format image name, read it and call
+        # v.py_sequence_loop(..) for current step
+        for i in range(seq_first, seq_last + 1, stepshake):
+            if i < 10:
+                seq_ch = "%01d" % i
+            elif i < 100:
+                seq_ch = "%02d" % i
+            else:
+                seq_ch = "%03d" % i
+            for j in range(n_camera):
+                img_name = base_name[j] + seq_ch
+                # print("Setting image: ", img_name)
+                try:
+                    temp_img = imread(img_name).astype(np.ubyte)
+                except BaseException:
+                    print("Error reading file")
+
+                self.ptv.py_set_img(temp_img, j)
+            self.ptv.py_sequence_loop(0, i)
+            self.camera_list[0].drawquiver(
+                [int(300 * random.random())],
+                [int(300 * random.random())],
+                [int(300 * random.random())],
+                [int(300 * random.random())],
+                "green",
+                linewidth=3.0,
+            )
+            self.camera_list[0]._plot.request_redraw()
```

### Comparing `pyptv-0.2.2/pyptv/ext_tracker_denis.py` & `pyptv-0.2.3/pyptv/ext_tracker_denis.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-class Tracking:
-    """Tracking class defines external tracking addon for pyptv
-    User needs to implement the following functions:
-            do_tracking(self)
-            do_back_tracking(self)
-    Connection to C ptv module is given via self.ptv and provided by pyptv software
-    Connection to active parameters is given via self.exp1 and provided by pyptv software.
-    User responsibility is to read necessary files, make the calculations and write the files back.
-    """
-
-    def __init__(self, ptv=None, exp1=None):
-        self.ptv = ptv
-        self.exp1 = exp1
-        # Do your initialization here
-
-    def do_tracking(self):
-        """this function is callback for "tracking without display" """
-        print("inside denis_ext_tracker")
-        run_info = self.ptv.py_trackcorr_init()
-        print(run_info.get_sequence_range())
-        for step in range(*run_info.get_sequence_range()):
-            print("step %d" % step)
-            self.ptv.py_trackcorr_loop(run_info, step, display=0)
-            # finalize tracking
-        self.ptv.py_trackcorr_finish(run_info, step + 1)
-
-    def do_back_tracking(self):
-        """this function is callback for "tracking back" """
-        # do your back_tracking stuff here
-        print("inside custom back tracking")
+class Tracking:
+    """Tracking class defines external tracking addon for pyptv
+    User needs to implement the following functions:
+            do_tracking(self)
+            do_back_tracking(self)
+    Connection to C ptv module is given via self.ptv and provided by pyptv software
+    Connection to active parameters is given via self.exp1 and provided by pyptv software.
+    User responsibility is to read necessary files, make the calculations and write the files back.
+    """
+
+    def __init__(self, ptv=None, exp1=None):
+        self.ptv = ptv
+        self.exp1 = exp1
+        # Do your initialization here
+
+    def do_tracking(self):
+        """this function is callback for "tracking without display" """
+        print("inside denis_ext_tracker")
+        run_info = self.ptv.py_trackcorr_init()
+        print(run_info.get_sequence_range())
+        for step in range(*run_info.get_sequence_range()):
+            print("step %d" % step)
+            self.ptv.py_trackcorr_loop(run_info, step, display=0)
+            # finalize tracking
+        self.ptv.py_trackcorr_finish(run_info, step + 1)
+
+    def do_back_tracking(self):
+        """this function is callback for "tracking back" """
+        # do your back_tracking stuff here
+        print("inside custom back tracking")
```

### Comparing `pyptv-0.2.2/pyptv/image_inspector.py` & `pyptv-0.2.3/pyptv/image_inspector.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,101 +1,101 @@
-#!/usr/bin/env python
-"""
-Demonstrates the ImageInspectorTool and overlay on a colormapped image
-plot.  The underlying plot is similar to the one in cmap_image_plot.py.
-
- - Left-drag pans the plot.
- - Mousewheel up and down zooms the plot in and out.
- - Pressing "z" brings up the Zoom Box, and you can click-drag a rectangular
-   region to zoom.  If you use a sequence of zoom boxes, pressing alt-left-arrow
-   and alt-right-arrow moves you forwards and backwards through the "zoom
-   history".
-
- - Pressing "p" will toggle the display of the image inspector overlay.
-"""
-
-# Major library imports
-from numpy import linspace, meshgrid, pi, sin
-
-# Enthought library imports
-from enable.api import Component, ComponentEditor
-from traits.api import HasTraits, Instance
-from traitsui.api import Item, Group, View
-
-# Chaco imports
-from chaco.api import ArrayPlotData, viridis, Plot
-from chaco.tools.api import PanTool, ZoomTool
-from chaco.tools.image_inspector_tool import (
-    ImageInspectorTool,
-    ImageInspectorOverlay,
-)
-
-# ===============================================================================
-# # Create the Chaco plot.
-# ===============================================================================
-def _create_plot_component():  # Create a scalar field to colormap
-    xbounds = (-2 * pi, 2 * pi, 600)
-    ybounds = (-1.5 * pi, 1.5 * pi, 300)
-    xs = linspace(*xbounds)
-    ys = linspace(*ybounds)
-    x, y = meshgrid(xs, ys)
-    z = sin(x) * y
-
-    # Create a plot data obect and give it this data
-    pd = ArrayPlotData()
-    pd.set_data("imagedata", z)
-
-    # Create the plot
-    plot = Plot(pd)
-    img_plot = plot.img_plot(
-        "imagedata", xbounds=xbounds[:2], ybounds=ybounds[:2], colormap=viridis
-    )[0]
-
-    # Tweak some of the plot properties
-    plot.title = "My First Image Plot"
-    plot.padding = 50
-
-    # Attach some tools to the plot
-    plot.tools.append(PanTool(plot))
-    zoom = ZoomTool(component=plot, tool_mode="box", always_on=False)
-    plot.overlays.append(zoom)
-    imgtool = ImageInspectorTool(component=img_plot)
-    img_plot.tools.append(imgtool)
-    overlay = ImageInspectorOverlay(
-        component=img_plot,
-        image_inspector=imgtool,
-        bgcolor="white",
-        border_visible=True,
-    )
-
-    img_plot.overlays.append(overlay)
-    return plot
-
-
-# ===============================================================================
-# Attributes to use for the plot view.
-size = (800, 600)
-title = "Inspecting a Colormapped Image Plot"
-
-# ===============================================================================
-# # Demo class that is used by the demo.py application.
-# ===============================================================================
-class Demo(HasTraits):
-    plot = Instance(Component)
-
-    traits_view = View(
-        Group(
-            Item("plot", editor=ComponentEditor(size=size), show_label=False),
-            orientation="vertical",
-        ),
-        resizable=True,
-        title=title,
-    )
-
-    def _plot_default(self):
-        return _create_plot_component()
-
-
-demo = Demo()
-
-if __name__ == "__main__":
-    demo.configure_traits()
+#!/usr/bin/env python
+"""
+Demonstrates the ImageInspectorTool and overlay on a colormapped image
+plot.  The underlying plot is similar to the one in cmap_image_plot.py.
+
+ - Left-drag pans the plot.
+ - Mousewheel up and down zooms the plot in and out.
+ - Pressing "z" brings up the Zoom Box, and you can click-drag a rectangular
+   region to zoom.  If you use a sequence of zoom boxes, pressing alt-left-arrow
+   and alt-right-arrow moves you forwards and backwards through the "zoom
+   history".
+
+ - Pressing "p" will toggle the display of the image inspector overlay.
+"""
+
+# Major library imports
+from numpy import linspace, meshgrid, pi, sin
+
+# Enthought library imports
+from enable.api import Component, ComponentEditor
+from traits.api import HasTraits, Instance
+from traitsui.api import Item, Group, View
+
+# Chaco imports
+from chaco.api import ArrayPlotData, viridis, Plot
+from chaco.tools.api import PanTool, ZoomTool
+from chaco.tools.image_inspector_tool import (
+    ImageInspectorTool,
+    ImageInspectorOverlay,
+)
+
+# ===============================================================================
+# # Create the Chaco plot.
+# ===============================================================================
+def _create_plot_component():  # Create a scalar field to colormap
+    xbounds = (-2 * pi, 2 * pi, 600)
+    ybounds = (-1.5 * pi, 1.5 * pi, 300)
+    xs = linspace(*xbounds)
+    ys = linspace(*ybounds)
+    x, y = meshgrid(xs, ys)
+    z = sin(x) * y
+
+    # Create a plot data obect and give it this data
+    pd = ArrayPlotData()
+    pd.set_data("imagedata", z)
+
+    # Create the plot
+    plot = Plot(pd)
+    img_plot = plot.img_plot(
+        "imagedata", xbounds=xbounds[:2], ybounds=ybounds[:2], colormap=viridis
+    )[0]
+
+    # Tweak some of the plot properties
+    plot.title = "My First Image Plot"
+    plot.padding = 50
+
+    # Attach some tools to the plot
+    plot.tools.append(PanTool(plot))
+    zoom = ZoomTool(component=plot, tool_mode="box", always_on=False)
+    plot.overlays.append(zoom)
+    imgtool = ImageInspectorTool(component=img_plot)
+    img_plot.tools.append(imgtool)
+    overlay = ImageInspectorOverlay(
+        component=img_plot,
+        image_inspector=imgtool,
+        bgcolor="white",
+        border_visible=True,
+    )
+
+    img_plot.overlays.append(overlay)
+    return plot
+
+
+# ===============================================================================
+# Attributes to use for the plot view.
+size = (800, 600)
+title = "Inspecting a Colormapped Image Plot"
+
+# ===============================================================================
+# # Demo class that is used by the demo.py application.
+# ===============================================================================
+class Demo(HasTraits):
+    plot = Instance(Component)
+
+    traits_view = View(
+        Group(
+            Item("plot", editor=ComponentEditor(size=size), show_label=False),
+            orientation="vertical",
+        ),
+        resizable=True,
+        title=title,
+    )
+
+    def _plot_default(self):
+        return _create_plot_component()
+
+
+demo = Demo()
+
+if __name__ == "__main__":
+    demo.configure_traits()
```

### Comparing `pyptv-0.2.2/pyptv/imageplot.py` & `pyptv-0.2.3/pyptv/imageplot.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-from numpy import linspace, meshgrid, exp
-
-from chaco.api import ArrayPlotData, Plot, viridis, gray
-from enable.api import ComponentEditor
-from traits.api import HasTraits, Instance
-from traitsui.api import Item, View
-
-
-class ImagePlot(HasTraits):
-
-    plot = Instance(Plot)
-
-    traits_view = View(
-        Item("plot", editor=ComponentEditor(), show_label=False),
-        width=600,
-        height=600,
-        resizable=True,
-        title="Chaco Plot",
-    )
-
-    def __init__(self):
-        # Create the data and the PlotData object.  For a 2D plot, we need to
-        # take the row of X points and Y points and create a grid from them
-        # using meshgrid().
-        x = linspace(0, 10, 50)
-        y = linspace(0, 5, 50)
-        xgrid, ygrid = meshgrid(x, y)
-        z = exp(-(xgrid * xgrid + ygrid * ygrid) / 100)
-        plotdata = ArrayPlotData(imagedata=z)
-        # Create a Plot and associate it with the PlotData
-        plot = Plot(plotdata)
-        # Create an image plot in the Plot
-        plot.img_plot("imagedata", colormap=viridis)
-        self.plot = plot
-
-
-# ===============================================================================
-# demo object that is used by the demo.py application.
-# ===============================================================================
-demo = ImagePlot()
-if __name__ == "__main__":
+from numpy import linspace, meshgrid, exp
+
+from chaco.api import ArrayPlotData, Plot, viridis, gray
+from enable.api import ComponentEditor
+from traits.api import HasTraits, Instance
+from traitsui.api import Item, View
+
+
+class ImagePlot(HasTraits):
+
+    plot = Instance(Plot)
+
+    traits_view = View(
+        Item("plot", editor=ComponentEditor(), show_label=False),
+        width=600,
+        height=600,
+        resizable=True,
+        title="Chaco Plot",
+    )
+
+    def __init__(self):
+        # Create the data and the PlotData object.  For a 2D plot, we need to
+        # take the row of X points and Y points and create a grid from them
+        # using meshgrid().
+        x = linspace(0, 10, 50)
+        y = linspace(0, 5, 50)
+        xgrid, ygrid = meshgrid(x, y)
+        z = exp(-(xgrid * xgrid + ygrid * ygrid) / 100)
+        plotdata = ArrayPlotData(imagedata=z)
+        # Create a Plot and associate it with the PlotData
+        plot = Plot(plotdata)
+        # Create an image plot in the Plot
+        plot.img_plot("imagedata", colormap=viridis)
+        self.plot = plot
+
+
+# ===============================================================================
+# demo object that is used by the demo.py application.
+# ===============================================================================
+demo = ImagePlot()
+if __name__ == "__main__":
     demo.configure_traits()
```

### Comparing `pyptv-0.2.2/pyptv/parameter_gui.py` & `pyptv-0.2.3/pyptv/parameter_gui.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,1393 +1,1393 @@
-import os
-import json
-from pathlib import Path
-
-from traits.api import HasTraits, Str, Float, Int, List, Bool, Enum, Instance
-from traitsui.api import (
-    View,
-    Item,
-    HGroup,
-    VGroup,
-    Handler,
-    Group,
-    Tabbed,
-    spring,
-)
-
-# from traits.etsconfig.api import ETSConfig
-
-from pyptv import parameters as par
-import numpy as np
-
-
-DEFAULT_STRING = "---"
-DEFAULT_INT = -999
-DEFAULT_FLOAT = -999.0
-
-
-# define handler function for main parameters
-class ParamHandler(Handler):
-    def closed(self, info, is_ok):
-        mainParams = info.object
-        par_path = mainParams.par_path
-        Handler.closed(self, info, is_ok)
-        if is_ok:
-            img_name = [
-                mainParams.Name_1_Image,
-                mainParams.Name_2_Image,
-                mainParams.Name_3_Image,
-                mainParams.Name_4_Image,
-            ]
-            img_cal_name = [
-                mainParams.Cali_1_Image,
-                mainParams.Cali_2_Image,
-                mainParams.Cali_3_Image,
-                mainParams.Cali_4_Image,
-            ]
-
-            gvthres = [
-                mainParams.Gray_Tresh_1,
-                mainParams.Gray_Tresh_2,
-                mainParams.Gray_Tresh_3,
-                mainParams.Gray_Tresh_4,
-            ]
-            base_name = [
-                mainParams.Basename_1_Seq,
-                mainParams.Basename_2_Seq,
-                mainParams.Basename_3_Seq,
-                mainParams.Basename_4_Seq,
-            ]
-            X_lay = [mainParams.Xmin, mainParams.Xmax]
-            Zmin_lay = [mainParams.Zmin1, mainParams.Zmin2]
-            Zmax_lay = [mainParams.Zmax1, mainParams.Zmax2]
-
-            # write ptv_par
-            par.PtvParams(
-                mainParams.Num_Cam,
-                img_name,
-                img_cal_name,
-                mainParams.HighPass,
-                mainParams.Accept_OnlyAllCameras,
-                mainParams.tiff_flag,
-                mainParams.imx,
-                mainParams.imy,
-                mainParams.pix_x,
-                mainParams.pix_y,
-                mainParams.chfield,
-                mainParams.Refr_Air,
-                mainParams.Refr_Glass,
-                mainParams.Refr_Water,
-                mainParams.Thick_Glass,
-                path=par_path,
-            ).write()
-            # write calibration parameters
-            par.CalOriParams(
-                mainParams.Num_Cam,
-                mainParams.fixp_name,
-                mainParams.img_cal_name,
-                mainParams.img_ori,
-                mainParams.tiff_flag,
-                mainParams.pair_Flag,
-                mainParams.chfield,
-                path=par_path,
-            ).write()
-
-            # write targ_rec_par
-            par.TargRecParams(
-                mainParams.Num_Cam,
-                gvthres,
-                mainParams.Tol_Disc,
-                mainParams.Min_Npix,
-                mainParams.Max_Npix,
-                mainParams.Min_Npix_x,
-                mainParams.Max_Npix_x,
-                mainParams.Min_Npix_y,
-                mainParams.Max_Npix_y,
-                mainParams.Sum_Grey,
-                mainParams.Size_Cross,
-                path=par_path,
-            ).write()
-            # write pft_version_par
-            par.PftVersionParams(
-                mainParams.Existing_Target, path=par_path
-            ).write()
-            # write sequence_par
-            par.SequenceParams(
-                mainParams.Num_Cam,
-                base_name,
-                mainParams.Seq_First,
-                mainParams.Seq_Last,
-                path=par_path,
-            ).write()
-            # write criteria_par
-            par.CriteriaParams(
-                X_lay,
-                Zmin_lay,
-                Zmax_lay,
-                mainParams.Min_Corr_nx,
-                mainParams.Min_Corr_ny,
-                mainParams.Min_Corr_npix,
-                mainParams.Sum_gv,
-                mainParams.Min_Weight_corr,
-                mainParams.Tol_Band,
-                path=par_path,
-            ).write()
-            
-            # write masking parameters
-            masking_dict = {
-                "mask_flag":mainParams.Subtr_Mask,
-                "mask_base_name":mainParams.Base_Name_Mask,
-            }
-            with (Path(par_path) / 'masking.json').open('w') as json_file:
-                json.dump(masking_dict, json_file)
-
-
-# define handler function for calibration parameters
-class CalHandler(Handler):
-    def closed(self, info, is_ok):
-        calibParams = info.object
-        par_path = calibParams.par_path
-        print("inside CalHandler ", par_path)
-        Handler.closed(self, info, is_ok)
-        if is_ok:
-            img_cal_name = [
-                calibParams.cam_1,
-                calibParams.cam_2,
-                calibParams.cam_3,
-                calibParams.cam_4,
-            ]
-            img_ori = [
-                calibParams.ori_cam_1,
-                calibParams.ori_cam_2,
-                calibParams.ori_cam_3,
-                calibParams.ori_cam_4,
-            ]
-            nr1 = [
-                calibParams.img_1_p1,
-                calibParams.img_1_p2,
-                calibParams.img_1_p3,
-                calibParams.img_1_p4,
-            ]
-            nr2 = [
-                calibParams.img_2_p1,
-                calibParams.img_2_p2,
-                calibParams.img_2_p3,
-                calibParams.img_2_p4,
-            ]
-            nr3 = [
-                calibParams.img_3_p1,
-                calibParams.img_3_p2,
-                calibParams.img_3_p3,
-                calibParams.img_3_p4,
-            ]
-            nr4 = [
-                calibParams.img_4_p1,
-                calibParams.img_4_p2,
-                calibParams.img_4_p3,
-                calibParams.img_4_p4,
-            ]
-
-            nr = [nr1, nr2, nr3, nr4]
-
-            if calibParams.chfield == "Frame":
-                chfield = 0
-            elif calibParams.chfield == "Field odd":
-                chfield = 1
-            else:
-                chfield = 2
-            par.PtvParams(
-                calibParams.n_img,
-                calibParams.img_name,
-                calibParams.img_cal,
-                calibParams.hp_flag,
-                calibParams.allcam_flag,
-                calibParams.tiff_head,
-                calibParams.h_image_size,
-                calibParams.v_image_size,
-                calibParams.h_pixel_size,
-                calibParams.v_pixel_size,
-                chfield,
-                calibParams.mmp_n1,
-                calibParams.mmp_n2,
-                calibParams.mmp_n3,
-                calibParams.mmp_d,
-                path=par_path,
-            ).write()
-
-            par.CalOriParams(
-                calibParams.n_img,
-                calibParams.fixp_name,
-                img_cal_name,
-                img_ori,
-                calibParams.tiff_head,
-                calibParams.pair_head,
-                chfield,
-                path=par_path,
-            ).write()
-
-            par.DetectPlateParams(
-                calibParams.grey_value_treshold_1,
-                calibParams.grey_value_treshold_2,
-                calibParams.grey_value_treshold_3,
-                calibParams.grey_value_treshold_4,
-                calibParams.tolerable_discontinuity,
-                calibParams.min_npix,
-                calibParams.max_npix,
-                calibParams.min_npix_x,
-                calibParams.max_npix_x,
-                calibParams.min_npix_y,
-                calibParams.max_npix_y,
-                calibParams.sum_of_grey,
-                calibParams.size_of_crosses,
-                path=par_path,
-            ).write()
-
-            par.ManOriParams(calibParams.n_img, nr, path=par_path).write()
-            par.ExamineParams(
-                calibParams.Examine_Flag,
-                calibParams.Combine_Flag,
-                path=par_path,
-            ).write()
-            par.OrientParams(
-                calibParams.point_number_of_orientation,
-                calibParams.cc,
-                calibParams.xh,
-                calibParams.yh,
-                calibParams.k1,
-                calibParams.k2,
-                calibParams.k3,
-                calibParams.p1,
-                calibParams.p2,
-                calibParams.scale,
-                calibParams.shear,
-                calibParams.interf,
-                path=par_path,
-            ).write()
-            par.ShakingParams(
-                calibParams.shaking_first_frame,
-                calibParams.shaking_last_frame,
-                calibParams.shaking_max_num_points,
-                calibParams.shaking_max_num_frames,
-                path=par_path,
-            ).write()
-
-            par.DumbbellParams(
-                calibParams.dumbbell_eps,
-                calibParams.dumbbell_scale,
-                calibParams.dumbbell_gradient_descent,
-                calibParams.dumbbell_penalty_weight,
-                calibParams.dumbbell_step,
-                calibParams.dumbbell_niter,
-                path=par_path,
-            ).write()
-
-
-class TrackHandler(Handler):
-    def closed(self, info, is_ok):
-        trackParams = info.object
-        par_path = trackParams.par_path
-        Handler.closed(self, info, is_ok)
-        if is_ok:
-            par.TrackingParams(
-                trackParams.dvxmin,
-                trackParams.dvxmax,
-                trackParams.dvymin,
-                trackParams.dvymax,
-                trackParams.dvzmin,
-                trackParams.dvzmax,
-                trackParams.angle,
-                trackParams.dacc,
-                trackParams.flagNewParticles,
-                path=par_path,
-            ).write()
-
-
-#             print "Michael:", info.object.dvxmin, type(info.object.dvxmin)
-#             info.object.write()
-
-
-# This is the view class of the Tracking Parameters window
-class Tracking_Params(HasTraits):
-    dvxmin = Float(DEFAULT_FLOAT)
-    dvxmax = Float(DEFAULT_FLOAT)
-    dvymin = Float(DEFAULT_FLOAT)
-    dvymax = Float(DEFAULT_FLOAT)
-    dvzmin = Float(DEFAULT_FLOAT)
-    dvzmax = Float(DEFAULT_FLOAT)
-    angle = Float(DEFAULT_FLOAT)
-    dacc = Float(DEFAULT_FLOAT)
-    flagNewParticles = Bool(True)
-
-    def __init__(self, par_path):
-        super(Tracking_Params, self).__init__()
-        self.par_path = par_path
-        TrackingParams = par.TrackingParams(path=self.par_path)
-        TrackingParams.read()
-        self.dvxmin = TrackingParams.dvxmin
-        self.dvxmax = TrackingParams.dvxmax
-        self.dvymin = TrackingParams.dvymin
-        self.dvymax = TrackingParams.dvymax
-        self.dvzmin = TrackingParams.dvzmin
-        self.dvzmax = TrackingParams.dvzmax
-        self.angle = TrackingParams.angle
-        self.dacc = TrackingParams.dacc
-        self.flagNewParticles = np.bool8(TrackingParams.flagNewParticles)
-
-    Tracking_Params_View = View(
-        HGroup(
-            Item(name="dvxmin", label="dvxmin:"),
-            Item(name="dvxmax", label="dvxmax:"),
-        ),
-        HGroup(
-            Item(name="dvymin", label="dvymin:"),
-            Item(name="dvymax", label="dvymax:"),
-        ),
-        HGroup(
-            Item(name="dvzmin", label="dvzmin:"),
-            Item(name="dvzmax", label="dvzmax:"),
-        ),
-        VGroup(
-            Item(name="angle", label="angle [gon]:"),
-            Item(name="dacc", label="dacc:"),
-        ),
-        Item(name="flagNewParticles", label="Add new particles?"),
-        buttons=["Undo", "OK", "Cancel"],
-        handler=TrackHandler(),
-        title="Tracking Parameters",
-    )
-
-
-class Main_Params(HasTraits):
-    # loading parameters files:
-    # read main parameters
-
-    # Panel 1: General
-    Num_Cam = Int(4, label="Number of cameras: ")
-    Accept_OnlyAllCameras = Bool(
-        False, label="Accept only points seen from all cameras?"
-    )
-    pair_Flag = Bool(False, label="Include pairs")
-    pair_enable_flag = Bool(True)
-    all_enable_flag = Bool(True)
-    hp_enable_flag = Bool(True)
-    inverse_image_flag = Bool(False)
-
-    # add here also size of the images, e.g. 1280 x 1024 pix and
-    # the size of the pixels.
-    # future option: name of the camera from the list with these
-    # parameters saved once somewhere, e.g.
-    # Mikrotron EoSense (1280 x 1024, 12 micron pixels)
-
-    # Future - this should be kind of more flexible, e.g.
-    # select only some name structure: CamX.YYYYY is clear that the
-    # X should be 1-Num_Cam and YYYY should be
-    # the running counter of the images. or Cam.X_00YYY.TIFF is also kind
-    # of clear that we have 5 digits with
-    # same could be for calibration, we have no point to create different
-    # names for 4 cameras:
-    # calX_run3 will be fine as a base name and X is 1 - Num_Cam
-    # not clear yet how to use the variable name later. probably we need to
-    # build it as a structure
-    # and use it as: for cam in range(Num_Cam):
-    # Name_Pre_Image[cam] = ''.join(BaseName,eval(cam),'.',eval(counter))
-    #
-
-    # unused parameters
-    # TODO: then why are they here?
-    # Answer: historical reasons, back compatibility
-
-    tiff_flag = Bool()
-    imx = Int(DEFAULT_INT)
-    imy = Int(DEFAULT_INT)
-    pix_x = Float(DEFAULT_FLOAT)
-    pix_y = Float(DEFAULT_FLOAT)
-    chfield = Int(DEFAULT_INT)
-    img_cal_name = []
-
-    # unsed for calibration
-    fixp_name = Str()
-    img_ori = []
-
-    Name_1_Image = Str(DEFAULT_STRING, label="Name of 1. image")
-    Name_2_Image = Str(DEFAULT_STRING, label="Name of 2. image")
-    Name_3_Image = Str(DEFAULT_STRING, label="Name of 3. image")
-    Name_4_Image = Str(DEFAULT_STRING, label="Name of 4. image")
-    Cali_1_Image = Str(DEFAULT_STRING, label="Calibration data for 1. image")
-    Cali_2_Image = Str(DEFAULT_STRING, label="Calibration data for 2. image")
-    Cali_3_Image = Str(DEFAULT_STRING, label="Calibration data for 3. image")
-    Cali_4_Image = Str(DEFAULT_STRING, label="Calibration data for 4. image")
-
-    # TiffHeader=Bool(True,label='Tiff header') -> probably obsolete for
-    # the Python imread () function
-    # FrameType=Enum('Frame','Field-odd','Field-even') -> obsolete
-    # future option:  List -> Select Media 1 (for each one):
-    # {'Air','Glass','Water','Custom'}, etc.
-    Refr_Air = Float(1.0, label="Air:")
-    Refr_Glass = Float(1.33, label="Glass:")
-    Refr_Water = Float(1.46, label="Water:")
-    Thick_Glass = Float(1.0, label="Thickness of glass:")
-
-    # New panel 2: ImageProcessing
-    HighPass = Bool(True, label="High pass filter")
-    # future option: Slider between 0 and 1 for each one
-    Gray_Tresh_1 = Int(DEFAULT_INT, label="1st image")
-    Gray_Tresh_2 = Int(DEFAULT_INT, label="2nd image")
-    Gray_Tresh_3 = Int(DEFAULT_INT, label="3rd image")
-    Gray_Tresh_4 = Int(DEFAULT_INT, label="4th image")
-    Min_Npix = Int(DEFAULT_INT, label="min npix")
-    Max_Npix = Int(DEFAULT_INT, label="max npix")
-    Min_Npix_x = Int(DEFAULT_INT, label="min npix x")
-    Max_Npix_x = Int(DEFAULT_INT, label="max npix x")
-    Min_Npix_y = Int(DEFAULT_INT, label="min npix y")
-    Max_Npix_y = Int(DEFAULT_INT, label="max npix y")
-    Sum_Grey = Int(DEFAULT_INT, label="Sum of grey value")
-    Tol_Disc = Int(DEFAULT_INT, label="Tolerable discontinuity")
-    Size_Cross = Int(DEFAULT_INT, label="Size of crosses")
-    Subtr_Mask = Bool(False, label="Subtract mask")
-    Base_Name_Mask = Str(DEFAULT_STRING, label="Base name for the mask")
-    Existing_Target = Bool(False, label="Use existing_target files?")
-    Inverse = Bool(False, label="Negative images?")
-
-    # New panel 3: Sequence
-    Seq_First = Int(DEFAULT_INT, label="First sequence image:")
-    Seq_Last = Int(DEFAULT_INT, label="Last sequence image:")
-    Basename_1_Seq = Str(DEFAULT_STRING, label="Basename for 1. sequence")
-    Basename_2_Seq = Str(DEFAULT_STRING, label="Basename for 2. sequence")
-    Basename_3_Seq = Str(DEFAULT_STRING, label="Basename for 3. sequence")
-    Basename_4_Seq = Str(DEFAULT_STRING, label="Basename for 4. sequence")
-
-    # Panel 4: ObservationVolume
-    Xmin = Int(DEFAULT_FLOAT, label="Xmin")
-    Xmax = Int(DEFAULT_FLOAT, label="Xmax")
-    Zmin1 = Int(DEFAULT_FLOAT, label="Zmin")
-    Zmin2 = Int(DEFAULT_FLOAT, label="Zmin")
-    Zmax1 = Int(DEFAULT_FLOAT, label="Zmax")
-    Zmax2 = Int(DEFAULT_FLOAT, label="Zmax")
-
-    # Panel 5: ParticleDetection
-    Min_Corr_nx = Float(DEFAULT_FLOAT, label="min corr for ratio nx")
-    Min_Corr_ny = Float(DEFAULT_FLOAT, label="min corr for ratio ny")
-    Min_Corr_npix = Float(DEFAULT_FLOAT, label="min corr for ratio npix")
-    Sum_gv = Float(DEFAULT_FLOAT, label="sum of gv")
-    Min_Weight_corr = Float(
-        DEFAULT_FLOAT, label="min for weighted correlation"
-    )
-    Tol_Band = Float(DEFAULT_FLOAT, lable="Tolerance of epipolar band [mm]")
-
-    # Group 1 is the group of General parameters
-    # number of cameras, use only quadruplets or also triplets/pairs?
-    # names of the test images, calibration files
-    Group1 = Group(
-        Group(
-            Item(name="Num_Cam", width=30),
-            Item(name="Accept_OnlyAllCameras", enabled_when="all_enable_flag"),
-            Item(name="pair_Flag", enabled_when="pair_enable_flag"),
-            orientation="horizontal",
-        ),
-        Group(
-            Group(
-                Item(name="Name_1_Image", width=150),
-                Item(name="Name_2_Image"),
-                Item(name="Name_3_Image"),
-                Item(name="Name_4_Image"),
-                orientation="vertical",
-            ),
-            Group(
-                Item(name="Cali_1_Image", width=150),
-                Item(name="Cali_2_Image"),
-                Item(name="Cali_3_Image"),
-                Item(name="Cali_4_Image"),
-                orientation="vertical",
-            ),
-            orientation="horizontal",
-        ),
-        orientation="vertical",
-        label="General",
-    )
-
-    Group2 = Group(
-        Group(
-            Item(name="Refr_Air"),
-            Item(name="Refr_Glass"),
-            Item(name="Refr_Water"),
-            Item(name="Thick_Glass"),
-            orientation="horizontal",
-        ),
-        label="Refractive Indices",
-        show_border=True,
-        orientation="vertical",
-    )
-
-    Group3 = Group(
-        Group(
-            Item(name="Gray_Tresh_1"),
-            Item(name="Gray_Tresh_2"),
-            Item(name="Gray_Tresh_3"),
-            Item(name="Gray_Tresh_4"),
-            label="Gray value treshold: ",
-            show_border=True,
-            orientation="horizontal",
-        ),
-        Group(
-            Group(
-                Item(name="Min_Npix"),
-                Item(name="Max_Npix"),
-                Item(name="Sum_Grey"),
-                orientation="vertical",
-            ),
-            Group(
-                Item(name="Min_Npix_x"),
-                Item(name="Max_Npix_x"),
-                Item(name="Tol_Disc"),
-                orientation="vertical",
-            ),
-            Group(
-                Item(name="Min_Npix_y"),
-                Item(name="Max_Npix_y"),
-                Item(name="Size_Cross"),
-                orientation="vertical",
-            ),
-            orientation="horizontal",
-        ),
-        Group(
-            Item(name="Subtr_Mask"),
-            Item(name="Base_Name_Mask"),
-            Item(name="Existing_Target"),
-            Item(name="HighPass", enabled_when="hp_enable_flag"),
-            Item(name="Inverse"),
-            orientation="horizontal",
-        ),
-        orientation="vertical",
-        show_border=True,
-        label="Particle recognition",
-    )
-
-    Group4 = Group(
-        Group(
-            Item(name="Seq_First"),
-            Item(name="Seq_Last"),
-            orientation="horizontal",
-        ),
-        Group(
-            Item(name="Basename_1_Seq"),
-            Item(name="Basename_2_Seq"),
-            Item(name="Basename_3_Seq"),
-            Item(name="Basename_4_Seq"),
-            orientation="vertical",
-        ),
-        label="Parameters for sequence processing",
-        orientation="vertical",
-        show_border=True,
-    )
-
-    Group5 = Group(
-        Group(Item(name="Xmin"), Item(name="Xmax"), orientation="vertical"),
-        Group(Item(name="Zmin1"), Item(name="Zmin2"), orientation="vertical"),
-        Group(Item(name="Zmax1"), Item(name="Zmax2"), orientation="vertical"),
-        orientation="horizontal",
-        label="Observation Volume",
-        show_border=True,
-    )
-
-    Group6 = Group(
-        Group(
-            Item(name="Min_Corr_nx"),
-            Item(name="Min_Corr_npix"),
-            Item(name="Min_Weight_corr"),
-            orientation="vertical",
-        ),
-        Group(
-            Item(name="Min_Corr_ny"),
-            Item(name="Sum_gv"),
-            Item(name="Tol_Band"),
-            orientation="vertical",
-        ),
-        orientation="horizontal",
-        label="Criteria for correspondences",
-        show_border=True,
-    )
-
-    Main_Params_View = View(
-        Tabbed(Group1, Group2, Group3, Group4, Group5, Group6),
-        resizable=True,
-        width=0.5,
-        height=0.3,
-        dock="horizontal",
-        buttons=["Undo", "OK", "Cancel"],
-        handler=ParamHandler(),
-        title="Main Parameters",
-    )
-
-    def _pair_Flag_fired(self):
-        # print("test")
-        if self.pair_Flag:
-
-            self.all_enable_flag = False
-
-        else:
-
-            self.all_enable_flag = True
-
-    def _Accept_OnlyAllCameras_fired(self):
-
-        if self.Accept_OnlyAllCameras:
-
-            self.pair_enable_flag = False
-
-        else:
-
-            self.pair_enable_flag = True
-
-    # TODO: underscore in Python signifies a private method (i.e. it shouldn't be accessed from outside this module).
-    # Answer: change it to the proper names. here it probably means just
-    # 'reload'
-    def _reload(self):
-        # load ptv_par
-        ptvParams = par.PtvParams(path=self.par_path)
-        ptvParams.read()
-
-        for i in range(ptvParams.n_img):
-            exec("self.Name_%d_Image = ptvParams.img_name[%d]" % (i + 1, i))
-            exec("self.Cali_%d_Image = ptvParams.img_cal[%d]" % (i + 1, i))
-
-        self.Refr_Air = ptvParams.mmp_n1
-        self.Refr_Glass = ptvParams.mmp_n2
-        self.Refr_Water = ptvParams.mmp_n3
-        self.Thick_Glass = ptvParams.mmp_d
-        self.Accept_OnlyAllCameras = np.bool8(ptvParams.allcam_flag)
-        self.Num_Cam = ptvParams.n_img
-        self.HighPass = np.bool8(ptvParams.hp_flag)
-        # load unused
-        self.tiff_flag = np.bool8(ptvParams.tiff_flag)
-        self.imx = ptvParams.imx
-        self.imy = ptvParams.imy
-        self.pix_x = ptvParams.pix_x
-        self.pix_y = ptvParams.pix_y
-        self.chfield = ptvParams.chfield
-
-        # read_calibration parameters
-        calOriParams = par.CalOriParams(ptvParams.n_img, path=self.par_path)
-        calOriParams.read()
-
-        self.pair_Flag = np.bool8(calOriParams.pair_flag)
-        self.img_cal_name = calOriParams.img_cal_name
-        self.img_ori = calOriParams.img_ori
-        self.fixp_name = calOriParams.fixp_name
-
-        # load read_targ_rec
-        targRecParams = par.TargRecParams(ptvParams.n_img, path=self.par_path)
-        targRecParams.read()
-
-        for i in range(ptvParams.n_img):
-            exec(
-                "self.Gray_Tresh_{0} = targRecParams.gvthres[{1}]".format(
-                    i + 1, i
-                )
-            )
-
-        self.Min_Npix = targRecParams.nnmin
-        self.Max_Npix = targRecParams.nnmax
-        self.Min_Npix_x = targRecParams.nxmin
-        self.Max_Npix_x = targRecParams.nxmax
-        self.Min_Npix_y = targRecParams.nymin
-        self.Max_Npix_y = targRecParams.nymax
-        self.Sum_Grey = targRecParams.sumg_min
-        self.Tol_Disc = targRecParams.disco
-        self.Size_Cross = targRecParams.cr_sz
-
-        # load pft_version
-        pftVersionParams = par.PftVersionParams(path=self.par_path)
-        pftVersionParams.read()
-        self.Existing_Target = np.bool8(pftVersionParams.Existing_Target)
-
-        # load sequence_par
-        sequenceParams = par.SequenceParams(
-            ptvParams.n_img, path=self.par_path
-        )
-        sequenceParams.read()
-
-        for i in range(ptvParams.n_img):
-            exec(
-                "self.Basename_{0}_Seq = sequenceParams.base_name[{1}]".format(
-                    i + 1, i
-                )
-            )
-
-        self.Seq_First = sequenceParams.first
-        self.Seq_Last = sequenceParams.last
-
-        # load criteria_par
-        criteriaParams = par.CriteriaParams(path=self.par_path)
-        criteriaParams.read()
-        self.Xmin = criteriaParams.X_lay[0]
-        self.Xmax = criteriaParams.X_lay[1]
-        self.Zmin1 = criteriaParams.Zmin_lay[0]
-        self.Zmin2 = criteriaParams.Zmin_lay[1]
-        self.Zmax1 = criteriaParams.Zmax_lay[0]
-        self.Zmax2 = criteriaParams.Zmax_lay[1]
-        self.Min_Corr_nx = criteriaParams.cnx
-        self.Min_Corr_ny = criteriaParams.cny
-        self.Min_Corr_npix = criteriaParams.cn
-        self.Sum_gv = criteriaParams.csumg
-        self.Min_Weight_corr = criteriaParams.corrmin
-        self.Tol_Band = criteriaParams.eps0
-        
-        # write masking parameters
-        masking_filename = Path(self.par_path) / 'masking.json'
-        if masking_filename.exists():
-                masking_dict = json.load(masking_filename.open('r'))
-                # json.dump(masking_dict, json_file)
-                self.Subtr_Mask = masking_dict['mask_flag']
-                self.Base_Name_Mask = masking_dict['mask_base_name']
-
-    # create initfunc
-    def __init__(self, par_path):
-        HasTraits.__init__(self)
-        self.par_path = par_path
-        self._reload()
-
-
-# -----------------------------------------------------------------------------
-class Calib_Params(HasTraits):
-
-    # general and unsed variables
-    pair_enable_flag = Bool(True)
-    n_img = Int(DEFAULT_INT)
-    img_name = List
-    img_cal = List
-    hp_flag = Bool(False, label="highpass")
-    allcam_flag = Bool(False, label="all camera targets")
-    mmp_n1 = Float(DEFAULT_FLOAT)
-    mmp_n2 = Float(DEFAULT_FLOAT)
-    mmp_n3 = Float(DEFAULT_FLOAT)
-    mmp_d = Float(DEFAULT_FLOAT)
-
-    # images data
-    cam_1 = Str(DEFAULT_STRING, label="Calibration picture camera 1")
-    cam_2 = Str(DEFAULT_STRING, label="Calibration picture camera 2")
-    cam_3 = Str(DEFAULT_STRING, label="Calibration picture camera 3")
-    cam_4 = Str(DEFAULT_STRING, label="Calibration picture camera 4")
-    ori_cam_1 = Str(DEFAULT_STRING, label="Orientation data picture camera 1")
-    ori_cam_2 = Str(DEFAULT_STRING, label="Orientation data picture camera 2")
-    ori_cam_3 = Str(DEFAULT_STRING, label="Orientation data picture camera 3")
-    ori_cam_4 = Str(DEFAULT_STRING, label="Orientation data picture camera 4")
-
-    fixp_name = Str(DEFAULT_STRING, label="File of Coordinates on plate")
-    tiff_head = Bool(True, label="TIFF-Header")
-    pair_head = Bool(True, label="Include pairs")
-    chfield = Enum("Frame", "Field odd", "Field even")
-
-    Group1_1 = Group(
-        Item(name="cam_1"),
-        Item(name="cam_2"),
-        Item(name="cam_3"),
-        Item(name="cam_4"),
-        label="Calibration pictures",
-        show_border=True,
-    )
-    Group1_2 = Group(
-        Item(name="ori_cam_1"),
-        Item(name="ori_cam_2"),
-        Item(name="ori_cam_3"),
-        Item(name="ori_cam_4"),
-        label="Orientation data",
-        show_border=True,
-    )
-    Group1_3 = Group(
-        Item(name="fixp_name"),
-        Group(
-            Item(name="tiff_head"),
-            Item(name="pair_head", enabled_when="pair_enable_flag"),
-            Item(name="chfield", show_label=False, style="custom"),
-            orientation="vertical",
-            columns=3,
-        ),
-        orientation="vertical",
-    )
-
-    # Group 1 is the group of General parameters
-    # number of cameras, use only quadruplets or also triplets/pairs?
-    # names of the test images, calibration files
-
-    Group1 = Group(
-        Group1_1,
-        Group1_2,
-        Group1_3,
-        orientation="vertical",
-        label="Images Data",
-    )
-
-    # calibration data detection
-
-    h_image_size = Int(DEFAULT_INT, label="Image size horizontal")
-    v_image_size = Int(DEFAULT_INT, label="Image size vertical")
-    h_pixel_size = Float(DEFAULT_FLOAT, label="Pixel size horizontal")
-    v_pixel_size = Float(DEFAULT_FLOAT, label="Pixel size vertical")
-
-    grey_value_treshold_1 = Int(DEFAULT_INT, label="First Image")
-    grey_value_treshold_2 = Int(DEFAULT_INT, label="Second Image")
-    grey_value_treshold_3 = Int(DEFAULT_INT, label="Third Image")
-    grey_value_treshold_4 = Int(DEFAULT_INT, label="Forth Image")
-    tolerable_discontinuity = Int(DEFAULT_INT, label="Tolerable discontinuity")
-    min_npix = Int(DEFAULT_INT, label="min npix")
-    min_npix_x = Int(DEFAULT_INT, label="min npix in x")
-    min_npix_y = Int(DEFAULT_INT, label="min npix in y")
-    max_npix = Int(DEFAULT_INT, label="max npix")
-    max_npix_x = Int(DEFAULT_INT, label="max npix in x")
-    max_npix_y = Int(DEFAULT_INT, label="max npix in y")
-    sum_of_grey = Int(DEFAULT_INT, label="Sum of greyvalue")
-    size_of_crosses = Int(DEFAULT_INT, label="Size of crosses")
-
-    Group2_1 = Group(
-        Item(name="h_image_size"),
-        Item(name="v_image_size"),
-        Item(name="h_pixel_size"),
-        Item(name="v_pixel_size"),
-        label="Image properties",
-        show_border=True,
-        orientation="horizontal",
-    )
-
-    Group2_2 = (
-        Group(
-            Item(name="grey_value_treshold_1"),
-            Item(name="grey_value_treshold_2"),
-            Item(name="grey_value_treshold_3"),
-            Item(name="grey_value_treshold_4"),
-            orientation="horizontal",
-            label="Grayvalue threshold",
-            show_border=True,
-        ),
-    )
-
-    Group2_3 = Group(
-        Group(
-            Item(name="min_npix"),
-            Item(name="min_npix_x"),
-            Item(name="min_npix_y"),
-            orientation="vertical",
-        ),
-        Group(
-            Item(name="max_npix"),
-            Item(name="max_npix_x"),
-            Item(name="max_npix_y"),
-            orientation="vertical",
-        ),
-        Group(
-            Item(name="tolerable_discontinuity"),
-            Item(name="sum_of_grey"),
-            Item(name="size_of_crosses"),
-            orientation="vertical",
-        ),
-        orientation="horizontal",
-    )
-
-    Group2 = Group(
-        Group2_1,
-        Group2_2,
-        Group2_3,
-        orientation="vertical",
-        label="Calibration Data Detection",
-    )
-
-    # manuel pre orientation
-    img_1_p1 = Int(DEFAULT_INT, label="P1")
-    img_1_p2 = Int(DEFAULT_INT, label="P2")
-    img_1_p3 = Int(DEFAULT_INT, label="P3")
-    img_1_p4 = Int(DEFAULT_INT, label="P4")
-    img_2_p1 = Int(DEFAULT_INT, label="P1")
-    img_2_p2 = Int(DEFAULT_INT, label="P2")
-    img_2_p3 = Int(DEFAULT_INT, label="P3")
-    img_2_p4 = Int(DEFAULT_INT, label="P4")
-    img_3_p1 = Int(DEFAULT_INT, label="P1")
-    img_3_p2 = Int(DEFAULT_INT, label="P2")
-    img_3_p3 = Int(DEFAULT_INT, label="P3")
-    img_3_p4 = Int(DEFAULT_INT, label="P4")
-    img_4_p1 = Int(DEFAULT_INT, label="P1")
-    img_4_p2 = Int(DEFAULT_INT, label="P2")
-    img_4_p3 = Int(DEFAULT_INT, label="P3")
-    img_4_p4 = Int(DEFAULT_INT, label="P4")
-
-    Group3_1 = Group(
-        Item(name="img_1_p1"),
-        Item(name="img_1_p2"),
-        Item(name="img_1_p3"),
-        Item(name="img_1_p4"),
-        orientation="horizontal",
-        label="Image 1",
-        show_border=True,
-    )
-    Group3_2 = Group(
-        Item(name="img_2_p1"),
-        Item(name="img_2_p2"),
-        Item(name="img_2_p3"),
-        Item(name="img_2_p4"),
-        orientation="horizontal",
-        label="Image 2",
-        show_border=True,
-    )
-    Group3_3 = Group(
-        Item(name="img_3_p1"),
-        Item(name="img_3_p2"),
-        Item(name="img_3_p3"),
-        Item(name="img_3_p4"),
-        orientation="horizontal",
-        label="Image 3",
-        show_border=True,
-    )
-    Group3_4 = Group(
-        Item(name="img_4_p1"),
-        Item(name="img_4_p2"),
-        Item(name="img_4_p3"),
-        Item(name="img_4_p4"),
-        orientation="horizontal",
-        label="Image 4",
-        show_border=True,
-    )
-    Group3 = Group(
-        Group3_1,
-        Group3_2,
-        Group3_3,
-        Group3_4,
-        show_border=True,
-        label="Manual pre-orientation",
-    )
-
-    # calibration orientation param.
-
-    Examine_Flag = Bool(False, label="Calibrate with different Z")
-    Combine_Flag = Bool(False, label="Combine preprocessed planes")
-
-    point_number_of_orientation = Int(
-        DEFAULT_INT, label="Point number of orientation"
-    )
-    cc = Bool(False, label="cc")
-    xh = Bool(False, label="xh")
-    yh = Bool(False, label="yh")
-    k1 = Bool(False, label="k1")
-    k2 = Bool(False, label="k2")
-    k3 = Bool(False, label="k3")
-    p1 = Bool(False, label="p1")
-    p2 = Bool(False, label="p2")
-    scale = Bool(False, label="scale")
-    shear = Bool(False, label="shear")
-    interf = Bool(False, label="interfaces check box are available")
-
-    Group4_0 = Group(
-        Item(name="Examine_Flag"), Item(name="Combine_Flag"), show_border=True
-    )
-
-    Group4_1 = Group(
-        Item(name="cc"),
-        Item(name="xh"),
-        Item(name="yh"),
-        orientation="vertical",
-        columns=3,
-    )
-    Group4_2 = Group(
-        Item(name="k1"),
-        Item(name="k2"),
-        Item(name="k3"),
-        Item(name="p1"),
-        Item(name="p2"),
-        orientation="vertical",
-        columns=5,
-        label="Lens distortion(Brown)",
-        show_border=True,
-    )
-    Group4_3 = Group(
-        Item(name="scale"),
-        Item(name="shear"),
-        orientation="vertical",
-        columns=2,
-        label="Affin transformation",
-        show_border=True,
-    )
-    Group4_4 = Group(Item(name="interf"))
-
-    Group4 = Group(
-        Group(
-            Group4_0,
-            Item(name="point_number_of_orientation"),
-            Group4_1,
-            Group4_2,
-            Group4_3,
-            Group4_4,
-            label=" Orientation Parameters ",
-            show_border=True,
-        ),
-        orientation="horizontal",
-        show_border=True,
-        label="Calibration Orientation Param.",
-    )
-
-    # dumbbell parameters
-    # 5  eps (mm)
-    # 46.5 dumbbell scale
-    # 0.005 gradient descent factor
-    # 1 weight for dumbbell penalty
-    # 2 step size through sequence
-    # 500 num iterations per click
-
-    dumbbell_eps = Float(DEFAULT_FLOAT, label="dumbbell epsilon")
-    dumbbell_scale = Float(DEFAULT_FLOAT, label="dumbbell scale")
-    dumbbell_gradient_descent = Float(
-        DEFAULT_FLOAT, label="dumbbell gradient descent factor"
-    )
-    dumbbell_penalty_weight = Float(
-        DEFAULT_FLOAT, label="weight for dumbbell penalty"
-    )
-    dumbbell_step = Int(DEFAULT_INT, label="step size through sequence")
-    dumbbell_niter = Int(DEFAULT_INT, label="number of iterations per click")
-
-    Group5 = HGroup(
-        VGroup(
-            Item(name="dumbbell_eps"),
-            Item(name="dumbbell_scale"),
-            Item(name="dumbbell_gradient_descent"),
-            Item(name="dumbbell_penalty_weight"),
-            Item(name="dumbbell_step"),
-            Item(name="dumbbell_niter"),
-        ),
-        spring,
-        label="Dumbbell calibration parameters",
-        show_border=True,
-    )
-
-    # shaking parameters
-    # 10000 - first frame
-    # 10004 - last frame
-    # 10 - max num points used per frame
-    # 5 - max number of frames to track
-
-    shaking_first_frame = Int(DEFAULT_INT, label="shaking first frame")
-    shaking_last_frame = Int(DEFAULT_INT, label="shaking last frame")
-    shaking_max_num_points = Int(DEFAULT_INT, label="shaking max num points")
-    shaking_max_num_frames = Int(DEFAULT_INT, label="shaking max num frames")
-
-    Group6 = HGroup(
-        VGroup(
-            Item(
-                name="shaking_first_frame",
-            ),
-            Item(name="shaking_last_frame"),
-            Item(name="shaking_max_num_points"),
-            Item(name="shaking_max_num_frames"),
-        ),
-        spring,
-        label="Shaking calibration parameters",
-        show_border=True,
-    )
-
-    Calib_Params_View = View(
-        Tabbed(Group1, Group2, Group3, Group4, Group5, Group6),
-        buttons=["Undo", "OK", "Cancel"],
-        handler=CalHandler(),
-        title="Calibration Parameters",
-    )
-
-    def _reload(self):
-        # print("reloading")
-        # self.__init__(self)
-        # load ptv_par
-        ptvParams = par.PtvParams(path=self.par_path)
-        ptvParams.read()
-
-        # read picture size parameters
-        self.h_image_size = ptvParams.imx
-        self.v_image_size = ptvParams.imy
-        self.h_pixel_size = ptvParams.pix_x
-        self.v_pixel_size = ptvParams.pix_y
-        self.img_cal = ptvParams.img_cal
-        if ptvParams.allcam_flag:
-            self.pair_enable_flag = False
-        else:
-            self.pair_enable_flag = True
-
-        # unesed parameters
-
-        self.n_img = ptvParams.n_img
-        self.img_name = ptvParams.img_name
-        self.hp_flag = np.bool8(ptvParams.hp_flag)
-        self.allcam_flag = np.bool8(ptvParams.allcam_flag)
-        self.mmp_n1 = ptvParams.mmp_n1
-        self.mmp_n2 = ptvParams.mmp_n2
-        self.mmp_n3 = ptvParams.mmp_n3
-        self.mmp_d = ptvParams.mmp_d
-
-        # read_calibration parameters
-        calOriParams = par.CalOriParams(self.n_img, path=self.par_path)
-        calOriParams.read()
-        (fixp_name, img_cal_name, img_ori, tiff_flag, pair_flag, chfield) = (
-            calOriParams.fixp_name,
-            calOriParams.img_cal_name,
-            calOriParams.img_ori,
-            calOriParams.tiff_flag,
-            calOriParams.pair_flag,
-            calOriParams.chfield,
-        )
-
-        for i in range(self.n_img):
-            exec(
-                "self.cam_{0} = calOriParams.img_cal_name[{1}]".format(
-                    i + 1, i
-                )
-            )
-            exec(
-                "self.ori_cam_{0} = calOriParams.img_ori[{1}]".format(i + 1, i)
-            )
-
-        self.tiff_head = np.bool8(tiff_flag)
-        self.pair_head = np.bool8(pair_flag)
-        self.fixp_name = fixp_name
-        if chfield == 0:
-            self.chfield = "Frame"
-        elif chfield == 1:
-            self.chfield = "Field odd"
-        else:
-            self.chfield = "Field even"
-
-        # read detect plate parameters
-        detectPlateParams = par.DetectPlateParams(path=self.par_path)
-        detectPlateParams.read()
-
-        (
-            gv_th1,
-            gv_th2,
-            gv_th3,
-            gv_th4,
-            tolerable_discontinuity,
-            min_npix,
-            max_npix,
-            min_npix_x,
-            max_npix_x,
-            min_npix_y,
-            max_npix_y,
-            sum_of_grey,
-            size_of_crosses,
-        ) = (
-            detectPlateParams.gvth_1,
-            detectPlateParams.gvth_2,
-            detectPlateParams.gvth_3,
-            detectPlateParams.gvth_4,
-            detectPlateParams.tol_dis,
-            detectPlateParams.min_npix,
-            detectPlateParams.max_npix,
-            detectPlateParams.min_npix_x,
-            detectPlateParams.max_npix_x,
-            detectPlateParams.min_npix_y,
-            detectPlateParams.max_npix_y,
-            detectPlateParams.sum_grey,
-            detectPlateParams.size_cross,
-        )
-
-        for i in range(self.n_img):
-            exec("self.grey_value_treshold_{0} = gv_th{0}".format(i + 1))
-
-        self.tolerable_discontinuity = tolerable_discontinuity
-        self.min_npix = min_npix
-        self.min_npix_x = min_npix_x
-        self.min_npix_y = min_npix_y
-        self.max_npix = max_npix
-        self.max_npix_x = max_npix_x
-        self.max_npix_y = max_npix_y
-        self.sum_of_grey = sum_of_grey
-        self.size_of_crosses = size_of_crosses
-
-        # read manual orientaion parameters
-        manOriParams = par.ManOriParams(self.n_img, [], path=self.par_path)
-        manOriParams.read()
-
-        for i in range(self.n_img):
-            for j in range(4):  # 4 points per image
-                exec(f"self.img_{i+1}_p{j+1} = manOriParams.nr[{i*4+j}]")
-
-        # examine arameters
-        examineParams = par.ExamineParams(path=self.par_path)
-        examineParams.read()
-        (self.Examine_Flag, self.Combine_Flag) = (
-            examineParams.Examine_Flag,
-            examineParams.Combine_Flag,
-        )
-
-        # orientation parameters
-        orientParams = par.OrientParams(path=self.par_path)
-        orientParams.read()
-        (
-            po_num_of_ori,
-            cc,
-            xh,
-            yh,
-            k1,
-            k2,
-            k3,
-            p1,
-            p2,
-            scale,
-            shear,
-            interf,
-        ) = (
-            orientParams.pnfo,
-            orientParams.cc,
-            orientParams.xh,
-            orientParams.yh,
-            orientParams.k1,
-            orientParams.k2,
-            orientParams.k3,
-            orientParams.p1,
-            orientParams.p2,
-            orientParams.scale,
-            orientParams.shear,
-            orientParams.interf,
-        )
-
-        self.point_number_of_orientation = po_num_of_ori
-        self.cc = np.bool8(cc)
-        self.xh = np.bool8(xh)
-        self.yh = np.bool8(yh)
-        self.k1 = np.bool8(k1)
-        self.k2 = np.bool8(k2)
-        self.k3 = np.bool8(k3)
-        self.p1 = np.bool8(p1)
-        self.p2 = np.bool8(p2)
-        self.scale = np.bool8(scale)
-        self.shear = np.bool8(shear)
-        self.interf = np.bool8(interf)
-
-        dumbbellParams = par.DumbbellParams(path=self.par_path)
-        dumbbellParams.read()
-        (
-            self.dumbbell_eps,
-            self.dumbbell_scale,
-            self.dumbbell_gradient_descent,
-            self.dumbbell_penalty_weight,
-            self.dumbbell_step,
-            self.dumbbell_niter,
-        ) = (
-            dumbbellParams.dumbbell_eps,
-            dumbbellParams.dumbbell_scale,
-            dumbbellParams.dumbbell_gradient_descent,
-            dumbbellParams.dumbbell_penalty_weight,
-            dumbbellParams.dumbbell_step,
-            dumbbellParams.dumbbell_niter,
-        )
-
-        shakingParams = par.ShakingParams(path=self.par_path)
-        shakingParams.read()
-        (
-            self.shaking_first_frame,
-            self.shaking_last_frame,
-            self.shaking_max_num_points,
-            self.shaking_max_num_frames,
-        ) = (
-            shakingParams.shaking_first_frame,
-            shakingParams.shaking_last_frame,
-            shakingParams.shaking_max_num_points,
-            shakingParams.shaking_max_num_frames,
-        )
-
-    def __init__(self, par_path):
-        HasTraits.__init__(self)
-        self.par_path = par_path
-        self._reload()
-
-    # ---------------------------------------------------------------------------
-
-
-class Paramset(HasTraits):
-    name = Str
-    par_path = Path
-    m_params = Instance(Main_Params)
-    c_params = Instance(Calib_Params)
-    t_params = Instance(Tracking_Params)
-
-
-class Experiment(HasTraits):
-    active_params = Instance(Paramset)
-    paramsets = List(Paramset)
-
-    def __init__(self):
-        HasTraits.__init__(self)
-        self.changed_active_params = False
-
-    def getParamsetIdx(self, paramset):
-        if isinstance(
-                paramset,
-                type(1)):  # integer value (index of the paramset)
-            return paramset
-        else:  # Value is instance of Pramset
-            return self.paramsets.index(paramset)
-
-    def addParamset(self, name: str, par_path: Path):
-        self.paramsets.append(
-            Paramset(
-                name=name,
-                par_path=par_path,
-                m_params=Main_Params(par_path=par_path),
-                c_params=Calib_Params(par_path=par_path),
-                t_params=Tracking_Params(par_path=par_path),
-            )
-        )
-
-    def removeParamset(self, paramset):
-        paramset_idx = self.getParamsetIdx(paramset)
-        self.paramsets.remove(self.paramsets[paramset_idx])
-
-    def nParamsets(self):
-        return len(self.paramsets)
-
-    def setActive(self, paramset):
-        paramset_idx = self.getParamsetIdx(paramset)
-        self.active_params = self.paramsets[paramset_idx]
-        self.paramsets.pop(paramset_idx)
-        self.paramsets.insert(0, self.active_params)
-        self.syncActiveDir()
-
-    def syncActiveDir(self):
-        default_parameters_path = Path(par.par_dir_prefix).resolve()
-        print(f" Syncing parameters between two folders: \n")
-        print(f"{self.active_params.par_path}, {default_parameters_path}")
-        par.copy_params_dir(self.active_params.par_path, default_parameters_path)
-
-    def populate_runs(self, exp_path: Path):
-        # Read all parameters directories from an experiment directory
-        self.paramsets = []
-        
-        # list all directories
-        dir_contents = [
-            f
-            for f in exp_path.iterdir()
-            if (exp_path / f).is_dir()
-        ]
-        
-        # choose directories that has 'parameters' in their path
-        dir_contents = [
-            f for f in dir_contents if str(f.stem).startswith(par.par_dir_prefix)
-        ]
-        # print(f" parameter sets are in {dir_contents}")
-
-        # if only 'parameters' folder, create its copy 'parametersRun1'
-        if len(dir_contents) == 1 and str(dir_contents[0].stem) == par.par_dir_prefix:
-            # single parameters directory, backward compatibility
-            exp_name = "Run1"
-            new_name = str(dir_contents[0]) + exp_name
-            new_path = Path(new_name).resolve()
-            print(f" Copying to the new folder {new_path} \n")
-            print("------------------------------------------\n")
-            par.copy_params_dir(dir_contents[0], new_path)
-            dir_contents.append(new_path)
-
-        # take each path in the dir_contents and create a tree entity with the short name
-        for dir_item in dir_contents:
-            # par_path = exp_path / dir_item
-            if str(dir_item.stem) != par.par_dir_prefix:
-                # This should be a params dir, add a tree entry for it.
-                exp_name = str(dir_item.stem).rsplit('parameters',maxsplit=1)[-1]
-
-                print(f"Experiment name is: {exp_name}")
-                print(f" adding Parameter set\n")
-                self.addParamset(exp_name, dir_item)
-
-        if not self.changed_active_params:
-            if self.nParamsets() > 0:
-                self.setActive(0)
+import os
+import json
+from pathlib import Path
+
+from traits.api import HasTraits, Str, Float, Int, List, Bool, Enum, Instance
+from traitsui.api import (
+    View,
+    Item,
+    HGroup,
+    VGroup,
+    Handler,
+    Group,
+    Tabbed,
+    spring,
+)
+
+# from traits.etsconfig.api import ETSConfig
+
+from pyptv import parameters as par
+import numpy as np
+
+
+DEFAULT_STRING = "---"
+DEFAULT_INT = -999
+DEFAULT_FLOAT = -999.0
+
+
+# define handler function for main parameters
+class ParamHandler(Handler):
+    def closed(self, info, is_ok):
+        mainParams = info.object
+        par_path = mainParams.par_path
+        Handler.closed(self, info, is_ok)
+        if is_ok:
+            img_name = [
+                mainParams.Name_1_Image,
+                mainParams.Name_2_Image,
+                mainParams.Name_3_Image,
+                mainParams.Name_4_Image,
+            ]
+            img_cal_name = [
+                mainParams.Cali_1_Image,
+                mainParams.Cali_2_Image,
+                mainParams.Cali_3_Image,
+                mainParams.Cali_4_Image,
+            ]
+
+            gvthres = [
+                mainParams.Gray_Tresh_1,
+                mainParams.Gray_Tresh_2,
+                mainParams.Gray_Tresh_3,
+                mainParams.Gray_Tresh_4,
+            ]
+            base_name = [
+                mainParams.Basename_1_Seq,
+                mainParams.Basename_2_Seq,
+                mainParams.Basename_3_Seq,
+                mainParams.Basename_4_Seq,
+            ]
+            X_lay = [mainParams.Xmin, mainParams.Xmax]
+            Zmin_lay = [mainParams.Zmin1, mainParams.Zmin2]
+            Zmax_lay = [mainParams.Zmax1, mainParams.Zmax2]
+
+            # write ptv_par
+            par.PtvParams(
+                mainParams.Num_Cam,
+                img_name,
+                img_cal_name,
+                mainParams.HighPass,
+                mainParams.Accept_OnlyAllCameras,
+                mainParams.tiff_flag,
+                mainParams.imx,
+                mainParams.imy,
+                mainParams.pix_x,
+                mainParams.pix_y,
+                mainParams.chfield,
+                mainParams.Refr_Air,
+                mainParams.Refr_Glass,
+                mainParams.Refr_Water,
+                mainParams.Thick_Glass,
+                path=par_path,
+            ).write()
+            # write calibration parameters
+            par.CalOriParams(
+                mainParams.Num_Cam,
+                mainParams.fixp_name,
+                mainParams.img_cal_name,
+                mainParams.img_ori,
+                mainParams.tiff_flag,
+                mainParams.pair_Flag,
+                mainParams.chfield,
+                path=par_path,
+            ).write()
+
+            # write targ_rec_par
+            par.TargRecParams(
+                mainParams.Num_Cam,
+                gvthres,
+                mainParams.Tol_Disc,
+                mainParams.Min_Npix,
+                mainParams.Max_Npix,
+                mainParams.Min_Npix_x,
+                mainParams.Max_Npix_x,
+                mainParams.Min_Npix_y,
+                mainParams.Max_Npix_y,
+                mainParams.Sum_Grey,
+                mainParams.Size_Cross,
+                path=par_path,
+            ).write()
+            # write pft_version_par
+            par.PftVersionParams(
+                mainParams.Existing_Target, path=par_path
+            ).write()
+            # write sequence_par
+            par.SequenceParams(
+                mainParams.Num_Cam,
+                base_name,
+                mainParams.Seq_First,
+                mainParams.Seq_Last,
+                path=par_path,
+            ).write()
+            # write criteria_par
+            par.CriteriaParams(
+                X_lay,
+                Zmin_lay,
+                Zmax_lay,
+                mainParams.Min_Corr_nx,
+                mainParams.Min_Corr_ny,
+                mainParams.Min_Corr_npix,
+                mainParams.Sum_gv,
+                mainParams.Min_Weight_corr,
+                mainParams.Tol_Band,
+                path=par_path,
+            ).write()
+            
+            # write masking parameters
+            masking_dict = {
+                "mask_flag":mainParams.Subtr_Mask,
+                "mask_base_name":mainParams.Base_Name_Mask,
+            }
+            with (Path(par_path) / 'masking.json').open('w') as json_file:
+                json.dump(masking_dict, json_file)
+
+
+# define handler function for calibration parameters
+class CalHandler(Handler):
+    def closed(self, info, is_ok):
+        calibParams = info.object
+        par_path = calibParams.par_path
+        print("inside CalHandler ", par_path)
+        Handler.closed(self, info, is_ok)
+        if is_ok:
+            img_cal_name = [
+                calibParams.cam_1,
+                calibParams.cam_2,
+                calibParams.cam_3,
+                calibParams.cam_4,
+            ]
+            img_ori = [
+                calibParams.ori_cam_1,
+                calibParams.ori_cam_2,
+                calibParams.ori_cam_3,
+                calibParams.ori_cam_4,
+            ]
+            nr1 = [
+                calibParams.img_1_p1,
+                calibParams.img_1_p2,
+                calibParams.img_1_p3,
+                calibParams.img_1_p4,
+            ]
+            nr2 = [
+                calibParams.img_2_p1,
+                calibParams.img_2_p2,
+                calibParams.img_2_p3,
+                calibParams.img_2_p4,
+            ]
+            nr3 = [
+                calibParams.img_3_p1,
+                calibParams.img_3_p2,
+                calibParams.img_3_p3,
+                calibParams.img_3_p4,
+            ]
+            nr4 = [
+                calibParams.img_4_p1,
+                calibParams.img_4_p2,
+                calibParams.img_4_p3,
+                calibParams.img_4_p4,
+            ]
+
+            nr = [nr1, nr2, nr3, nr4]
+
+            if calibParams.chfield == "Frame":
+                chfield = 0
+            elif calibParams.chfield == "Field odd":
+                chfield = 1
+            else:
+                chfield = 2
+            par.PtvParams(
+                calibParams.n_img,
+                calibParams.img_name,
+                calibParams.img_cal,
+                calibParams.hp_flag,
+                calibParams.allcam_flag,
+                calibParams.tiff_head,
+                calibParams.h_image_size,
+                calibParams.v_image_size,
+                calibParams.h_pixel_size,
+                calibParams.v_pixel_size,
+                chfield,
+                calibParams.mmp_n1,
+                calibParams.mmp_n2,
+                calibParams.mmp_n3,
+                calibParams.mmp_d,
+                path=par_path,
+            ).write()
+
+            par.CalOriParams(
+                calibParams.n_img,
+                calibParams.fixp_name,
+                img_cal_name,
+                img_ori,
+                calibParams.tiff_head,
+                calibParams.pair_head,
+                chfield,
+                path=par_path,
+            ).write()
+
+            par.DetectPlateParams(
+                calibParams.grey_value_treshold_1,
+                calibParams.grey_value_treshold_2,
+                calibParams.grey_value_treshold_3,
+                calibParams.grey_value_treshold_4,
+                calibParams.tolerable_discontinuity,
+                calibParams.min_npix,
+                calibParams.max_npix,
+                calibParams.min_npix_x,
+                calibParams.max_npix_x,
+                calibParams.min_npix_y,
+                calibParams.max_npix_y,
+                calibParams.sum_of_grey,
+                calibParams.size_of_crosses,
+                path=par_path,
+            ).write()
+
+            par.ManOriParams(calibParams.n_img, nr, path=par_path).write()
+            par.ExamineParams(
+                calibParams.Examine_Flag,
+                calibParams.Combine_Flag,
+                path=par_path,
+            ).write()
+            par.OrientParams(
+                calibParams.point_number_of_orientation,
+                calibParams.cc,
+                calibParams.xh,
+                calibParams.yh,
+                calibParams.k1,
+                calibParams.k2,
+                calibParams.k3,
+                calibParams.p1,
+                calibParams.p2,
+                calibParams.scale,
+                calibParams.shear,
+                calibParams.interf,
+                path=par_path,
+            ).write()
+            par.ShakingParams(
+                calibParams.shaking_first_frame,
+                calibParams.shaking_last_frame,
+                calibParams.shaking_max_num_points,
+                calibParams.shaking_max_num_frames,
+                path=par_path,
+            ).write()
+
+            par.DumbbellParams(
+                calibParams.dumbbell_eps,
+                calibParams.dumbbell_scale,
+                calibParams.dumbbell_gradient_descent,
+                calibParams.dumbbell_penalty_weight,
+                calibParams.dumbbell_step,
+                calibParams.dumbbell_niter,
+                path=par_path,
+            ).write()
+
+
+class TrackHandler(Handler):
+    def closed(self, info, is_ok):
+        trackParams = info.object
+        par_path = trackParams.par_path
+        Handler.closed(self, info, is_ok)
+        if is_ok:
+            par.TrackingParams(
+                trackParams.dvxmin,
+                trackParams.dvxmax,
+                trackParams.dvymin,
+                trackParams.dvymax,
+                trackParams.dvzmin,
+                trackParams.dvzmax,
+                trackParams.angle,
+                trackParams.dacc,
+                trackParams.flagNewParticles,
+                path=par_path,
+            ).write()
+
+
+#             print "Michael:", info.object.dvxmin, type(info.object.dvxmin)
+#             info.object.write()
+
+
+# This is the view class of the Tracking Parameters window
+class Tracking_Params(HasTraits):
+    dvxmin = Float(DEFAULT_FLOAT)
+    dvxmax = Float(DEFAULT_FLOAT)
+    dvymin = Float(DEFAULT_FLOAT)
+    dvymax = Float(DEFAULT_FLOAT)
+    dvzmin = Float(DEFAULT_FLOAT)
+    dvzmax = Float(DEFAULT_FLOAT)
+    angle = Float(DEFAULT_FLOAT)
+    dacc = Float(DEFAULT_FLOAT)
+    flagNewParticles = Bool(True)
+
+    def __init__(self, par_path):
+        super(Tracking_Params, self).__init__()
+        self.par_path = par_path
+        TrackingParams = par.TrackingParams(path=self.par_path)
+        TrackingParams.read()
+        self.dvxmin = TrackingParams.dvxmin
+        self.dvxmax = TrackingParams.dvxmax
+        self.dvymin = TrackingParams.dvymin
+        self.dvymax = TrackingParams.dvymax
+        self.dvzmin = TrackingParams.dvzmin
+        self.dvzmax = TrackingParams.dvzmax
+        self.angle = TrackingParams.angle
+        self.dacc = TrackingParams.dacc
+        self.flagNewParticles = np.bool8(TrackingParams.flagNewParticles)
+
+    Tracking_Params_View = View(
+        HGroup(
+            Item(name="dvxmin", label="dvxmin:"),
+            Item(name="dvxmax", label="dvxmax:"),
+        ),
+        HGroup(
+            Item(name="dvymin", label="dvymin:"),
+            Item(name="dvymax", label="dvymax:"),
+        ),
+        HGroup(
+            Item(name="dvzmin", label="dvzmin:"),
+            Item(name="dvzmax", label="dvzmax:"),
+        ),
+        VGroup(
+            Item(name="angle", label="angle [gon]:"),
+            Item(name="dacc", label="dacc:"),
+        ),
+        Item(name="flagNewParticles", label="Add new particles?"),
+        buttons=["Undo", "OK", "Cancel"],
+        handler=TrackHandler(),
+        title="Tracking Parameters",
+    )
+
+
+class Main_Params(HasTraits):
+    # loading parameters files:
+    # read main parameters
+
+    # Panel 1: General
+    Num_Cam = Int(4, label="Number of cameras: ")
+    Accept_OnlyAllCameras = Bool(
+        False, label="Accept only points seen from all cameras?"
+    )
+    pair_Flag = Bool(False, label="Include pairs")
+    pair_enable_flag = Bool(True)
+    all_enable_flag = Bool(True)
+    hp_enable_flag = Bool(True)
+    inverse_image_flag = Bool(False)
+
+    # add here also size of the images, e.g. 1280 x 1024 pix and
+    # the size of the pixels.
+    # future option: name of the camera from the list with these
+    # parameters saved once somewhere, e.g.
+    # Mikrotron EoSense (1280 x 1024, 12 micron pixels)
+
+    # Future - this should be kind of more flexible, e.g.
+    # select only some name structure: CamX.YYYYY is clear that the
+    # X should be 1-Num_Cam and YYYY should be
+    # the running counter of the images. or Cam.X_00YYY.TIFF is also kind
+    # of clear that we have 5 digits with
+    # same could be for calibration, we have no point to create different
+    # names for 4 cameras:
+    # calX_run3 will be fine as a base name and X is 1 - Num_Cam
+    # not clear yet how to use the variable name later. probably we need to
+    # build it as a structure
+    # and use it as: for cam in range(Num_Cam):
+    # Name_Pre_Image[cam] = ''.join(BaseName,eval(cam),'.',eval(counter))
+    #
+
+    # unused parameters
+    # TODO: then why are they here?
+    # Answer: historical reasons, back compatibility
+
+    tiff_flag = Bool()
+    imx = Int(DEFAULT_INT)
+    imy = Int(DEFAULT_INT)
+    pix_x = Float(DEFAULT_FLOAT)
+    pix_y = Float(DEFAULT_FLOAT)
+    chfield = Int(DEFAULT_INT)
+    img_cal_name = []
+
+    # unsed for calibration
+    fixp_name = Str()
+    img_ori = []
+
+    Name_1_Image = Str(DEFAULT_STRING, label="Name of 1. image")
+    Name_2_Image = Str(DEFAULT_STRING, label="Name of 2. image")
+    Name_3_Image = Str(DEFAULT_STRING, label="Name of 3. image")
+    Name_4_Image = Str(DEFAULT_STRING, label="Name of 4. image")
+    Cali_1_Image = Str(DEFAULT_STRING, label="Calibration data for 1. image")
+    Cali_2_Image = Str(DEFAULT_STRING, label="Calibration data for 2. image")
+    Cali_3_Image = Str(DEFAULT_STRING, label="Calibration data for 3. image")
+    Cali_4_Image = Str(DEFAULT_STRING, label="Calibration data for 4. image")
+
+    # TiffHeader=Bool(True,label='Tiff header') -> probably obsolete for
+    # the Python imread () function
+    # FrameType=Enum('Frame','Field-odd','Field-even') -> obsolete
+    # future option:  List -> Select Media 1 (for each one):
+    # {'Air','Glass','Water','Custom'}, etc.
+    Refr_Air = Float(1.0, label="Air:")
+    Refr_Glass = Float(1.33, label="Glass:")
+    Refr_Water = Float(1.46, label="Water:")
+    Thick_Glass = Float(1.0, label="Thickness of glass:")
+
+    # New panel 2: ImageProcessing
+    HighPass = Bool(True, label="High pass filter")
+    # future option: Slider between 0 and 1 for each one
+    Gray_Tresh_1 = Int(DEFAULT_INT, label="1st image")
+    Gray_Tresh_2 = Int(DEFAULT_INT, label="2nd image")
+    Gray_Tresh_3 = Int(DEFAULT_INT, label="3rd image")
+    Gray_Tresh_4 = Int(DEFAULT_INT, label="4th image")
+    Min_Npix = Int(DEFAULT_INT, label="min npix")
+    Max_Npix = Int(DEFAULT_INT, label="max npix")
+    Min_Npix_x = Int(DEFAULT_INT, label="min npix x")
+    Max_Npix_x = Int(DEFAULT_INT, label="max npix x")
+    Min_Npix_y = Int(DEFAULT_INT, label="min npix y")
+    Max_Npix_y = Int(DEFAULT_INT, label="max npix y")
+    Sum_Grey = Int(DEFAULT_INT, label="Sum of grey value")
+    Tol_Disc = Int(DEFAULT_INT, label="Tolerable discontinuity")
+    Size_Cross = Int(DEFAULT_INT, label="Size of crosses")
+    Subtr_Mask = Bool(False, label="Subtract mask")
+    Base_Name_Mask = Str(DEFAULT_STRING, label="Base name for the mask")
+    Existing_Target = Bool(False, label="Use existing_target files?")
+    Inverse = Bool(False, label="Negative images?")
+
+    # New panel 3: Sequence
+    Seq_First = Int(DEFAULT_INT, label="First sequence image:")
+    Seq_Last = Int(DEFAULT_INT, label="Last sequence image:")
+    Basename_1_Seq = Str(DEFAULT_STRING, label="Basename for 1. sequence")
+    Basename_2_Seq = Str(DEFAULT_STRING, label="Basename for 2. sequence")
+    Basename_3_Seq = Str(DEFAULT_STRING, label="Basename for 3. sequence")
+    Basename_4_Seq = Str(DEFAULT_STRING, label="Basename for 4. sequence")
+
+    # Panel 4: ObservationVolume
+    Xmin = Int(DEFAULT_FLOAT, label="Xmin")
+    Xmax = Int(DEFAULT_FLOAT, label="Xmax")
+    Zmin1 = Int(DEFAULT_FLOAT, label="Zmin")
+    Zmin2 = Int(DEFAULT_FLOAT, label="Zmin")
+    Zmax1 = Int(DEFAULT_FLOAT, label="Zmax")
+    Zmax2 = Int(DEFAULT_FLOAT, label="Zmax")
+
+    # Panel 5: ParticleDetection
+    Min_Corr_nx = Float(DEFAULT_FLOAT, label="min corr for ratio nx")
+    Min_Corr_ny = Float(DEFAULT_FLOAT, label="min corr for ratio ny")
+    Min_Corr_npix = Float(DEFAULT_FLOAT, label="min corr for ratio npix")
+    Sum_gv = Float(DEFAULT_FLOAT, label="sum of gv")
+    Min_Weight_corr = Float(
+        DEFAULT_FLOAT, label="min for weighted correlation"
+    )
+    Tol_Band = Float(DEFAULT_FLOAT, lable="Tolerance of epipolar band [mm]")
+
+    # Group 1 is the group of General parameters
+    # number of cameras, use only quadruplets or also triplets/pairs?
+    # names of the test images, calibration files
+    Group1 = Group(
+        Group(
+            Item(name="Num_Cam", width=30),
+            Item(name="Accept_OnlyAllCameras", enabled_when="all_enable_flag"),
+            Item(name="pair_Flag", enabled_when="pair_enable_flag"),
+            orientation="horizontal",
+        ),
+        Group(
+            Group(
+                Item(name="Name_1_Image", width=150),
+                Item(name="Name_2_Image"),
+                Item(name="Name_3_Image"),
+                Item(name="Name_4_Image"),
+                orientation="vertical",
+            ),
+            Group(
+                Item(name="Cali_1_Image", width=150),
+                Item(name="Cali_2_Image"),
+                Item(name="Cali_3_Image"),
+                Item(name="Cali_4_Image"),
+                orientation="vertical",
+            ),
+            orientation="horizontal",
+        ),
+        orientation="vertical",
+        label="General",
+    )
+
+    Group2 = Group(
+        Group(
+            Item(name="Refr_Air"),
+            Item(name="Refr_Glass"),
+            Item(name="Refr_Water"),
+            Item(name="Thick_Glass"),
+            orientation="horizontal",
+        ),
+        label="Refractive Indices",
+        show_border=True,
+        orientation="vertical",
+    )
+
+    Group3 = Group(
+        Group(
+            Item(name="Gray_Tresh_1"),
+            Item(name="Gray_Tresh_2"),
+            Item(name="Gray_Tresh_3"),
+            Item(name="Gray_Tresh_4"),
+            label="Gray value treshold: ",
+            show_border=True,
+            orientation="horizontal",
+        ),
+        Group(
+            Group(
+                Item(name="Min_Npix"),
+                Item(name="Max_Npix"),
+                Item(name="Sum_Grey"),
+                orientation="vertical",
+            ),
+            Group(
+                Item(name="Min_Npix_x"),
+                Item(name="Max_Npix_x"),
+                Item(name="Tol_Disc"),
+                orientation="vertical",
+            ),
+            Group(
+                Item(name="Min_Npix_y"),
+                Item(name="Max_Npix_y"),
+                Item(name="Size_Cross"),
+                orientation="vertical",
+            ),
+            orientation="horizontal",
+        ),
+        Group(
+            Item(name="Subtr_Mask"),
+            Item(name="Base_Name_Mask"),
+            Item(name="Existing_Target"),
+            Item(name="HighPass", enabled_when="hp_enable_flag"),
+            Item(name="Inverse"),
+            orientation="horizontal",
+        ),
+        orientation="vertical",
+        show_border=True,
+        label="Particle recognition",
+    )
+
+    Group4 = Group(
+        Group(
+            Item(name="Seq_First"),
+            Item(name="Seq_Last"),
+            orientation="horizontal",
+        ),
+        Group(
+            Item(name="Basename_1_Seq"),
+            Item(name="Basename_2_Seq"),
+            Item(name="Basename_3_Seq"),
+            Item(name="Basename_4_Seq"),
+            orientation="vertical",
+        ),
+        label="Parameters for sequence processing",
+        orientation="vertical",
+        show_border=True,
+    )
+
+    Group5 = Group(
+        Group(Item(name="Xmin"), Item(name="Xmax"), orientation="vertical"),
+        Group(Item(name="Zmin1"), Item(name="Zmin2"), orientation="vertical"),
+        Group(Item(name="Zmax1"), Item(name="Zmax2"), orientation="vertical"),
+        orientation="horizontal",
+        label="Observation Volume",
+        show_border=True,
+    )
+
+    Group6 = Group(
+        Group(
+            Item(name="Min_Corr_nx"),
+            Item(name="Min_Corr_npix"),
+            Item(name="Min_Weight_corr"),
+            orientation="vertical",
+        ),
+        Group(
+            Item(name="Min_Corr_ny"),
+            Item(name="Sum_gv"),
+            Item(name="Tol_Band"),
+            orientation="vertical",
+        ),
+        orientation="horizontal",
+        label="Criteria for correspondences",
+        show_border=True,
+    )
+
+    Main_Params_View = View(
+        Tabbed(Group1, Group2, Group3, Group4, Group5, Group6),
+        resizable=True,
+        width=0.5,
+        height=0.3,
+        dock="horizontal",
+        buttons=["Undo", "OK", "Cancel"],
+        handler=ParamHandler(),
+        title="Main Parameters",
+    )
+
+    def _pair_Flag_fired(self):
+        # print("test")
+        if self.pair_Flag:
+
+            self.all_enable_flag = False
+
+        else:
+
+            self.all_enable_flag = True
+
+    def _Accept_OnlyAllCameras_fired(self):
+
+        if self.Accept_OnlyAllCameras:
+
+            self.pair_enable_flag = False
+
+        else:
+
+            self.pair_enable_flag = True
+
+    # TODO: underscore in Python signifies a private method (i.e. it shouldn't be accessed from outside this module).
+    # Answer: change it to the proper names. here it probably means just
+    # 'reload'
+    def _reload(self):
+        # load ptv_par
+        ptvParams = par.PtvParams(path=self.par_path)
+        ptvParams.read()
+
+        for i in range(ptvParams.n_img):
+            exec("self.Name_%d_Image = ptvParams.img_name[%d]" % (i + 1, i))
+            exec("self.Cali_%d_Image = ptvParams.img_cal[%d]" % (i + 1, i))
+
+        self.Refr_Air = ptvParams.mmp_n1
+        self.Refr_Glass = ptvParams.mmp_n2
+        self.Refr_Water = ptvParams.mmp_n3
+        self.Thick_Glass = ptvParams.mmp_d
+        self.Accept_OnlyAllCameras = np.bool8(ptvParams.allcam_flag)
+        self.Num_Cam = ptvParams.n_img
+        self.HighPass = np.bool8(ptvParams.hp_flag)
+        # load unused
+        self.tiff_flag = np.bool8(ptvParams.tiff_flag)
+        self.imx = ptvParams.imx
+        self.imy = ptvParams.imy
+        self.pix_x = ptvParams.pix_x
+        self.pix_y = ptvParams.pix_y
+        self.chfield = ptvParams.chfield
+
+        # read_calibration parameters
+        calOriParams = par.CalOriParams(ptvParams.n_img, path=self.par_path)
+        calOriParams.read()
+
+        self.pair_Flag = np.bool8(calOriParams.pair_flag)
+        self.img_cal_name = calOriParams.img_cal_name
+        self.img_ori = calOriParams.img_ori
+        self.fixp_name = calOriParams.fixp_name
+
+        # load read_targ_rec
+        targRecParams = par.TargRecParams(ptvParams.n_img, path=self.par_path)
+        targRecParams.read()
+
+        for i in range(ptvParams.n_img):
+            exec(
+                "self.Gray_Tresh_{0} = targRecParams.gvthres[{1}]".format(
+                    i + 1, i
+                )
+            )
+
+        self.Min_Npix = targRecParams.nnmin
+        self.Max_Npix = targRecParams.nnmax
+        self.Min_Npix_x = targRecParams.nxmin
+        self.Max_Npix_x = targRecParams.nxmax
+        self.Min_Npix_y = targRecParams.nymin
+        self.Max_Npix_y = targRecParams.nymax
+        self.Sum_Grey = targRecParams.sumg_min
+        self.Tol_Disc = targRecParams.disco
+        self.Size_Cross = targRecParams.cr_sz
+
+        # load pft_version
+        pftVersionParams = par.PftVersionParams(path=self.par_path)
+        pftVersionParams.read()
+        self.Existing_Target = np.bool8(pftVersionParams.Existing_Target)
+
+        # load sequence_par
+        sequenceParams = par.SequenceParams(
+            ptvParams.n_img, path=self.par_path
+        )
+        sequenceParams.read()
+
+        for i in range(ptvParams.n_img):
+            exec(
+                "self.Basename_{0}_Seq = sequenceParams.base_name[{1}]".format(
+                    i + 1, i
+                )
+            )
+
+        self.Seq_First = sequenceParams.first
+        self.Seq_Last = sequenceParams.last
+
+        # load criteria_par
+        criteriaParams = par.CriteriaParams(path=self.par_path)
+        criteriaParams.read()
+        self.Xmin = criteriaParams.X_lay[0]
+        self.Xmax = criteriaParams.X_lay[1]
+        self.Zmin1 = criteriaParams.Zmin_lay[0]
+        self.Zmin2 = criteriaParams.Zmin_lay[1]
+        self.Zmax1 = criteriaParams.Zmax_lay[0]
+        self.Zmax2 = criteriaParams.Zmax_lay[1]
+        self.Min_Corr_nx = criteriaParams.cnx
+        self.Min_Corr_ny = criteriaParams.cny
+        self.Min_Corr_npix = criteriaParams.cn
+        self.Sum_gv = criteriaParams.csumg
+        self.Min_Weight_corr = criteriaParams.corrmin
+        self.Tol_Band = criteriaParams.eps0
+        
+        # write masking parameters
+        masking_filename = Path(self.par_path) / 'masking.json'
+        if masking_filename.exists():
+                masking_dict = json.load(masking_filename.open('r'))
+                # json.dump(masking_dict, json_file)
+                self.Subtr_Mask = masking_dict['mask_flag']
+                self.Base_Name_Mask = masking_dict['mask_base_name']
+
+    # create initfunc
+    def __init__(self, par_path):
+        HasTraits.__init__(self)
+        self.par_path = par_path
+        self._reload()
+
+
+# -----------------------------------------------------------------------------
+class Calib_Params(HasTraits):
+
+    # general and unsed variables
+    pair_enable_flag = Bool(True)
+    n_img = Int(DEFAULT_INT)
+    img_name = List
+    img_cal = List
+    hp_flag = Bool(False, label="highpass")
+    allcam_flag = Bool(False, label="all camera targets")
+    mmp_n1 = Float(DEFAULT_FLOAT)
+    mmp_n2 = Float(DEFAULT_FLOAT)
+    mmp_n3 = Float(DEFAULT_FLOAT)
+    mmp_d = Float(DEFAULT_FLOAT)
+
+    # images data
+    cam_1 = Str(DEFAULT_STRING, label="Calibration picture camera 1")
+    cam_2 = Str(DEFAULT_STRING, label="Calibration picture camera 2")
+    cam_3 = Str(DEFAULT_STRING, label="Calibration picture camera 3")
+    cam_4 = Str(DEFAULT_STRING, label="Calibration picture camera 4")
+    ori_cam_1 = Str(DEFAULT_STRING, label="Orientation data picture camera 1")
+    ori_cam_2 = Str(DEFAULT_STRING, label="Orientation data picture camera 2")
+    ori_cam_3 = Str(DEFAULT_STRING, label="Orientation data picture camera 3")
+    ori_cam_4 = Str(DEFAULT_STRING, label="Orientation data picture camera 4")
+
+    fixp_name = Str(DEFAULT_STRING, label="File of Coordinates on plate")
+    tiff_head = Bool(True, label="TIFF-Header")
+    pair_head = Bool(True, label="Include pairs")
+    chfield = Enum("Frame", "Field odd", "Field even")
+
+    Group1_1 = Group(
+        Item(name="cam_1"),
+        Item(name="cam_2"),
+        Item(name="cam_3"),
+        Item(name="cam_4"),
+        label="Calibration pictures",
+        show_border=True,
+    )
+    Group1_2 = Group(
+        Item(name="ori_cam_1"),
+        Item(name="ori_cam_2"),
+        Item(name="ori_cam_3"),
+        Item(name="ori_cam_4"),
+        label="Orientation data",
+        show_border=True,
+    )
+    Group1_3 = Group(
+        Item(name="fixp_name"),
+        Group(
+            Item(name="tiff_head"),
+            Item(name="pair_head", enabled_when="pair_enable_flag"),
+            Item(name="chfield", show_label=False, style="custom"),
+            orientation="vertical",
+            columns=3,
+        ),
+        orientation="vertical",
+    )
+
+    # Group 1 is the group of General parameters
+    # number of cameras, use only quadruplets or also triplets/pairs?
+    # names of the test images, calibration files
+
+    Group1 = Group(
+        Group1_1,
+        Group1_2,
+        Group1_3,
+        orientation="vertical",
+        label="Images Data",
+    )
+
+    # calibration data detection
+
+    h_image_size = Int(DEFAULT_INT, label="Image size horizontal")
+    v_image_size = Int(DEFAULT_INT, label="Image size vertical")
+    h_pixel_size = Float(DEFAULT_FLOAT, label="Pixel size horizontal")
+    v_pixel_size = Float(DEFAULT_FLOAT, label="Pixel size vertical")
+
+    grey_value_treshold_1 = Int(DEFAULT_INT, label="First Image")
+    grey_value_treshold_2 = Int(DEFAULT_INT, label="Second Image")
+    grey_value_treshold_3 = Int(DEFAULT_INT, label="Third Image")
+    grey_value_treshold_4 = Int(DEFAULT_INT, label="Forth Image")
+    tolerable_discontinuity = Int(DEFAULT_INT, label="Tolerable discontinuity")
+    min_npix = Int(DEFAULT_INT, label="min npix")
+    min_npix_x = Int(DEFAULT_INT, label="min npix in x")
+    min_npix_y = Int(DEFAULT_INT, label="min npix in y")
+    max_npix = Int(DEFAULT_INT, label="max npix")
+    max_npix_x = Int(DEFAULT_INT, label="max npix in x")
+    max_npix_y = Int(DEFAULT_INT, label="max npix in y")
+    sum_of_grey = Int(DEFAULT_INT, label="Sum of greyvalue")
+    size_of_crosses = Int(DEFAULT_INT, label="Size of crosses")
+
+    Group2_1 = Group(
+        Item(name="h_image_size"),
+        Item(name="v_image_size"),
+        Item(name="h_pixel_size"),
+        Item(name="v_pixel_size"),
+        label="Image properties",
+        show_border=True,
+        orientation="horizontal",
+    )
+
+    Group2_2 = (
+        Group(
+            Item(name="grey_value_treshold_1"),
+            Item(name="grey_value_treshold_2"),
+            Item(name="grey_value_treshold_3"),
+            Item(name="grey_value_treshold_4"),
+            orientation="horizontal",
+            label="Grayvalue threshold",
+            show_border=True,
+        ),
+    )
+
+    Group2_3 = Group(
+        Group(
+            Item(name="min_npix"),
+            Item(name="min_npix_x"),
+            Item(name="min_npix_y"),
+            orientation="vertical",
+        ),
+        Group(
+            Item(name="max_npix"),
+            Item(name="max_npix_x"),
+            Item(name="max_npix_y"),
+            orientation="vertical",
+        ),
+        Group(
+            Item(name="tolerable_discontinuity"),
+            Item(name="sum_of_grey"),
+            Item(name="size_of_crosses"),
+            orientation="vertical",
+        ),
+        orientation="horizontal",
+    )
+
+    Group2 = Group(
+        Group2_1,
+        Group2_2,
+        Group2_3,
+        orientation="vertical",
+        label="Calibration Data Detection",
+    )
+
+    # manuel pre orientation
+    img_1_p1 = Int(DEFAULT_INT, label="P1")
+    img_1_p2 = Int(DEFAULT_INT, label="P2")
+    img_1_p3 = Int(DEFAULT_INT, label="P3")
+    img_1_p4 = Int(DEFAULT_INT, label="P4")
+    img_2_p1 = Int(DEFAULT_INT, label="P1")
+    img_2_p2 = Int(DEFAULT_INT, label="P2")
+    img_2_p3 = Int(DEFAULT_INT, label="P3")
+    img_2_p4 = Int(DEFAULT_INT, label="P4")
+    img_3_p1 = Int(DEFAULT_INT, label="P1")
+    img_3_p2 = Int(DEFAULT_INT, label="P2")
+    img_3_p3 = Int(DEFAULT_INT, label="P3")
+    img_3_p4 = Int(DEFAULT_INT, label="P4")
+    img_4_p1 = Int(DEFAULT_INT, label="P1")
+    img_4_p2 = Int(DEFAULT_INT, label="P2")
+    img_4_p3 = Int(DEFAULT_INT, label="P3")
+    img_4_p4 = Int(DEFAULT_INT, label="P4")
+
+    Group3_1 = Group(
+        Item(name="img_1_p1"),
+        Item(name="img_1_p2"),
+        Item(name="img_1_p3"),
+        Item(name="img_1_p4"),
+        orientation="horizontal",
+        label="Image 1",
+        show_border=True,
+    )
+    Group3_2 = Group(
+        Item(name="img_2_p1"),
+        Item(name="img_2_p2"),
+        Item(name="img_2_p3"),
+        Item(name="img_2_p4"),
+        orientation="horizontal",
+        label="Image 2",
+        show_border=True,
+    )
+    Group3_3 = Group(
+        Item(name="img_3_p1"),
+        Item(name="img_3_p2"),
+        Item(name="img_3_p3"),
+        Item(name="img_3_p4"),
+        orientation="horizontal",
+        label="Image 3",
+        show_border=True,
+    )
+    Group3_4 = Group(
+        Item(name="img_4_p1"),
+        Item(name="img_4_p2"),
+        Item(name="img_4_p3"),
+        Item(name="img_4_p4"),
+        orientation="horizontal",
+        label="Image 4",
+        show_border=True,
+    )
+    Group3 = Group(
+        Group3_1,
+        Group3_2,
+        Group3_3,
+        Group3_4,
+        show_border=True,
+        label="Manual pre-orientation",
+    )
+
+    # calibration orientation param.
+
+    Examine_Flag = Bool(False, label="Calibrate with different Z")
+    Combine_Flag = Bool(False, label="Combine preprocessed planes")
+
+    point_number_of_orientation = Int(
+        DEFAULT_INT, label="Point number of orientation"
+    )
+    cc = Bool(False, label="cc")
+    xh = Bool(False, label="xh")
+    yh = Bool(False, label="yh")
+    k1 = Bool(False, label="k1")
+    k2 = Bool(False, label="k2")
+    k3 = Bool(False, label="k3")
+    p1 = Bool(False, label="p1")
+    p2 = Bool(False, label="p2")
+    scale = Bool(False, label="scale")
+    shear = Bool(False, label="shear")
+    interf = Bool(False, label="interfaces check box are available")
+
+    Group4_0 = Group(
+        Item(name="Examine_Flag"), Item(name="Combine_Flag"), show_border=True
+    )
+
+    Group4_1 = Group(
+        Item(name="cc"),
+        Item(name="xh"),
+        Item(name="yh"),
+        orientation="vertical",
+        columns=3,
+    )
+    Group4_2 = Group(
+        Item(name="k1"),
+        Item(name="k2"),
+        Item(name="k3"),
+        Item(name="p1"),
+        Item(name="p2"),
+        orientation="vertical",
+        columns=5,
+        label="Lens distortion(Brown)",
+        show_border=True,
+    )
+    Group4_3 = Group(
+        Item(name="scale"),
+        Item(name="shear"),
+        orientation="vertical",
+        columns=2,
+        label="Affin transformation",
+        show_border=True,
+    )
+    Group4_4 = Group(Item(name="interf"))
+
+    Group4 = Group(
+        Group(
+            Group4_0,
+            Item(name="point_number_of_orientation"),
+            Group4_1,
+            Group4_2,
+            Group4_3,
+            Group4_4,
+            label=" Orientation Parameters ",
+            show_border=True,
+        ),
+        orientation="horizontal",
+        show_border=True,
+        label="Calibration Orientation Param.",
+    )
+
+    # dumbbell parameters
+    # 5  eps (mm)
+    # 46.5 dumbbell scale
+    # 0.005 gradient descent factor
+    # 1 weight for dumbbell penalty
+    # 2 step size through sequence
+    # 500 num iterations per click
+
+    dumbbell_eps = Float(DEFAULT_FLOAT, label="dumbbell epsilon")
+    dumbbell_scale = Float(DEFAULT_FLOAT, label="dumbbell scale")
+    dumbbell_gradient_descent = Float(
+        DEFAULT_FLOAT, label="dumbbell gradient descent factor"
+    )
+    dumbbell_penalty_weight = Float(
+        DEFAULT_FLOAT, label="weight for dumbbell penalty"
+    )
+    dumbbell_step = Int(DEFAULT_INT, label="step size through sequence")
+    dumbbell_niter = Int(DEFAULT_INT, label="number of iterations per click")
+
+    Group5 = HGroup(
+        VGroup(
+            Item(name="dumbbell_eps"),
+            Item(name="dumbbell_scale"),
+            Item(name="dumbbell_gradient_descent"),
+            Item(name="dumbbell_penalty_weight"),
+            Item(name="dumbbell_step"),
+            Item(name="dumbbell_niter"),
+        ),
+        spring,
+        label="Dumbbell calibration parameters",
+        show_border=True,
+    )
+
+    # shaking parameters
+    # 10000 - first frame
+    # 10004 - last frame
+    # 10 - max num points used per frame
+    # 5 - max number of frames to track
+
+    shaking_first_frame = Int(DEFAULT_INT, label="shaking first frame")
+    shaking_last_frame = Int(DEFAULT_INT, label="shaking last frame")
+    shaking_max_num_points = Int(DEFAULT_INT, label="shaking max num points")
+    shaking_max_num_frames = Int(DEFAULT_INT, label="shaking max num frames")
+
+    Group6 = HGroup(
+        VGroup(
+            Item(
+                name="shaking_first_frame",
+            ),
+            Item(name="shaking_last_frame"),
+            Item(name="shaking_max_num_points"),
+            Item(name="shaking_max_num_frames"),
+        ),
+        spring,
+        label="Shaking calibration parameters",
+        show_border=True,
+    )
+
+    Calib_Params_View = View(
+        Tabbed(Group1, Group2, Group3, Group4, Group5, Group6),
+        buttons=["Undo", "OK", "Cancel"],
+        handler=CalHandler(),
+        title="Calibration Parameters",
+    )
+
+    def _reload(self):
+        # print("reloading")
+        # self.__init__(self)
+        # load ptv_par
+        ptvParams = par.PtvParams(path=self.par_path)
+        ptvParams.read()
+
+        # read picture size parameters
+        self.h_image_size = ptvParams.imx
+        self.v_image_size = ptvParams.imy
+        self.h_pixel_size = ptvParams.pix_x
+        self.v_pixel_size = ptvParams.pix_y
+        self.img_cal = ptvParams.img_cal
+        if ptvParams.allcam_flag:
+            self.pair_enable_flag = False
+        else:
+            self.pair_enable_flag = True
+
+        # unesed parameters
+
+        self.n_img = ptvParams.n_img
+        self.img_name = ptvParams.img_name
+        self.hp_flag = np.bool8(ptvParams.hp_flag)
+        self.allcam_flag = np.bool8(ptvParams.allcam_flag)
+        self.mmp_n1 = ptvParams.mmp_n1
+        self.mmp_n2 = ptvParams.mmp_n2
+        self.mmp_n3 = ptvParams.mmp_n3
+        self.mmp_d = ptvParams.mmp_d
+
+        # read_calibration parameters
+        calOriParams = par.CalOriParams(self.n_img, path=self.par_path)
+        calOriParams.read()
+        (fixp_name, img_cal_name, img_ori, tiff_flag, pair_flag, chfield) = (
+            calOriParams.fixp_name,
+            calOriParams.img_cal_name,
+            calOriParams.img_ori,
+            calOriParams.tiff_flag,
+            calOriParams.pair_flag,
+            calOriParams.chfield,
+        )
+
+        for i in range(self.n_img):
+            exec(
+                "self.cam_{0} = calOriParams.img_cal_name[{1}]".format(
+                    i + 1, i
+                )
+            )
+            exec(
+                "self.ori_cam_{0} = calOriParams.img_ori[{1}]".format(i + 1, i)
+            )
+
+        self.tiff_head = np.bool8(tiff_flag)
+        self.pair_head = np.bool8(pair_flag)
+        self.fixp_name = fixp_name
+        if chfield == 0:
+            self.chfield = "Frame"
+        elif chfield == 1:
+            self.chfield = "Field odd"
+        else:
+            self.chfield = "Field even"
+
+        # read detect plate parameters
+        detectPlateParams = par.DetectPlateParams(path=self.par_path)
+        detectPlateParams.read()
+
+        (
+            gv_th1,
+            gv_th2,
+            gv_th3,
+            gv_th4,
+            tolerable_discontinuity,
+            min_npix,
+            max_npix,
+            min_npix_x,
+            max_npix_x,
+            min_npix_y,
+            max_npix_y,
+            sum_of_grey,
+            size_of_crosses,
+        ) = (
+            detectPlateParams.gvth_1,
+            detectPlateParams.gvth_2,
+            detectPlateParams.gvth_3,
+            detectPlateParams.gvth_4,
+            detectPlateParams.tol_dis,
+            detectPlateParams.min_npix,
+            detectPlateParams.max_npix,
+            detectPlateParams.min_npix_x,
+            detectPlateParams.max_npix_x,
+            detectPlateParams.min_npix_y,
+            detectPlateParams.max_npix_y,
+            detectPlateParams.sum_grey,
+            detectPlateParams.size_cross,
+        )
+
+        for i in range(self.n_img):
+            exec("self.grey_value_treshold_{0} = gv_th{0}".format(i + 1))
+
+        self.tolerable_discontinuity = tolerable_discontinuity
+        self.min_npix = min_npix
+        self.min_npix_x = min_npix_x
+        self.min_npix_y = min_npix_y
+        self.max_npix = max_npix
+        self.max_npix_x = max_npix_x
+        self.max_npix_y = max_npix_y
+        self.sum_of_grey = sum_of_grey
+        self.size_of_crosses = size_of_crosses
+
+        # read manual orientaion parameters
+        manOriParams = par.ManOriParams(self.n_img, [], path=self.par_path)
+        manOriParams.read()
+
+        for i in range(self.n_img):
+            for j in range(4):  # 4 points per image
+                exec(f"self.img_{i+1}_p{j+1} = manOriParams.nr[{i*4+j}]")
+
+        # examine arameters
+        examineParams = par.ExamineParams(path=self.par_path)
+        examineParams.read()
+        (self.Examine_Flag, self.Combine_Flag) = (
+            examineParams.Examine_Flag,
+            examineParams.Combine_Flag,
+        )
+
+        # orientation parameters
+        orientParams = par.OrientParams(path=self.par_path)
+        orientParams.read()
+        (
+            po_num_of_ori,
+            cc,
+            xh,
+            yh,
+            k1,
+            k2,
+            k3,
+            p1,
+            p2,
+            scale,
+            shear,
+            interf,
+        ) = (
+            orientParams.pnfo,
+            orientParams.cc,
+            orientParams.xh,
+            orientParams.yh,
+            orientParams.k1,
+            orientParams.k2,
+            orientParams.k3,
+            orientParams.p1,
+            orientParams.p2,
+            orientParams.scale,
+            orientParams.shear,
+            orientParams.interf,
+        )
+
+        self.point_number_of_orientation = po_num_of_ori
+        self.cc = np.bool8(cc)
+        self.xh = np.bool8(xh)
+        self.yh = np.bool8(yh)
+        self.k1 = np.bool8(k1)
+        self.k2 = np.bool8(k2)
+        self.k3 = np.bool8(k3)
+        self.p1 = np.bool8(p1)
+        self.p2 = np.bool8(p2)
+        self.scale = np.bool8(scale)
+        self.shear = np.bool8(shear)
+        self.interf = np.bool8(interf)
+
+        dumbbellParams = par.DumbbellParams(path=self.par_path)
+        dumbbellParams.read()
+        (
+            self.dumbbell_eps,
+            self.dumbbell_scale,
+            self.dumbbell_gradient_descent,
+            self.dumbbell_penalty_weight,
+            self.dumbbell_step,
+            self.dumbbell_niter,
+        ) = (
+            dumbbellParams.dumbbell_eps,
+            dumbbellParams.dumbbell_scale,
+            dumbbellParams.dumbbell_gradient_descent,
+            dumbbellParams.dumbbell_penalty_weight,
+            dumbbellParams.dumbbell_step,
+            dumbbellParams.dumbbell_niter,
+        )
+
+        shakingParams = par.ShakingParams(path=self.par_path)
+        shakingParams.read()
+        (
+            self.shaking_first_frame,
+            self.shaking_last_frame,
+            self.shaking_max_num_points,
+            self.shaking_max_num_frames,
+        ) = (
+            shakingParams.shaking_first_frame,
+            shakingParams.shaking_last_frame,
+            shakingParams.shaking_max_num_points,
+            shakingParams.shaking_max_num_frames,
+        )
+
+    def __init__(self, par_path):
+        HasTraits.__init__(self)
+        self.par_path = par_path
+        self._reload()
+
+    # ---------------------------------------------------------------------------
+
+
+class Paramset(HasTraits):
+    name = Str
+    par_path = Path
+    m_params = Instance(Main_Params)
+    c_params = Instance(Calib_Params)
+    t_params = Instance(Tracking_Params)
+
+
+class Experiment(HasTraits):
+    active_params = Instance(Paramset)
+    paramsets = List(Paramset)
+
+    def __init__(self):
+        HasTraits.__init__(self)
+        self.changed_active_params = False
+
+    def getParamsetIdx(self, paramset):
+        if isinstance(
+                paramset,
+                type(1)):  # integer value (index of the paramset)
+            return paramset
+        else:  # Value is instance of Pramset
+            return self.paramsets.index(paramset)
+
+    def addParamset(self, name: str, par_path: Path):
+        self.paramsets.append(
+            Paramset(
+                name=name,
+                par_path=par_path,
+                m_params=Main_Params(par_path=par_path),
+                c_params=Calib_Params(par_path=par_path),
+                t_params=Tracking_Params(par_path=par_path),
+            )
+        )
+
+    def removeParamset(self, paramset):
+        paramset_idx = self.getParamsetIdx(paramset)
+        self.paramsets.remove(self.paramsets[paramset_idx])
+
+    def nParamsets(self):
+        return len(self.paramsets)
+
+    def setActive(self, paramset):
+        paramset_idx = self.getParamsetIdx(paramset)
+        self.active_params = self.paramsets[paramset_idx]
+        self.paramsets.pop(paramset_idx)
+        self.paramsets.insert(0, self.active_params)
+        self.syncActiveDir()
+
+    def syncActiveDir(self):
+        default_parameters_path = Path(par.par_dir_prefix).resolve()
+        print(f" Syncing parameters between two folders: \n")
+        print(f"{self.active_params.par_path}, {default_parameters_path}")
+        par.copy_params_dir(self.active_params.par_path, default_parameters_path)
+
+    def populate_runs(self, exp_path: Path):
+        # Read all parameters directories from an experiment directory
+        self.paramsets = []
+        
+        # list all directories
+        dir_contents = [
+            f
+            for f in exp_path.iterdir()
+            if (exp_path / f).is_dir()
+        ]
+        
+        # choose directories that has 'parameters' in their path
+        dir_contents = [
+            f for f in dir_contents if str(f.stem).startswith(par.par_dir_prefix)
+        ]
+        # print(f" parameter sets are in {dir_contents}")
+
+        # if only 'parameters' folder, create its copy 'parametersRun1'
+        if len(dir_contents) == 1 and str(dir_contents[0].stem) == par.par_dir_prefix:
+            # single parameters directory, backward compatibility
+            exp_name = "Run1"
+            new_name = str(dir_contents[0]) + exp_name
+            new_path = Path(new_name).resolve()
+            print(f" Copying to the new folder {new_path} \n")
+            print("------------------------------------------\n")
+            par.copy_params_dir(dir_contents[0], new_path)
+            dir_contents.append(new_path)
+
+        # take each path in the dir_contents and create a tree entity with the short name
+        for dir_item in dir_contents:
+            # par_path = exp_path / dir_item
+            if str(dir_item.stem) != par.par_dir_prefix:
+                # This should be a params dir, add a tree entry for it.
+                exp_name = str(dir_item.stem).rsplit('parameters',maxsplit=1)[-1]
+
+                print(f"Experiment name is: {exp_name}")
+                print(f" adding Parameter set\n")
+                self.addParamset(exp_name, dir_item)
+
+        if not self.changed_active_params:
+            if self.nParamsets() > 0:
+                self.setActive(0)
```

### Comparing `pyptv-0.2.2/pyptv/ptv.py` & `pyptv-0.2.3/pyptv/ptv.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,535 +1,535 @@
-from pathlib import Path
-import numpy as np
-from optv.calibration import Calibration
-from optv.correspondences import correspondences, MatchedCoords
-from optv.image_processing import preprocess_image
-from optv.orientation import (
-    point_positions,
-    external_calibration,
-    full_calibration,
-)
-from optv.parameters import (
-    ControlParams,
-    VolumeParams,
-    TrackingParams,
-    SequenceParams,
-    TargetParams,
-)
-from optv.segmentation import target_recognition
-from optv.tracking_framebuf import CORRES_NONE, read_targets, TargetArray
-from optv.tracker import Tracker, default_naming
-from optv.epipolar import epipolar_curve
-from skimage.io import imread
-from pyptv import parameters as par
-
-
-def negative(img):
-    """ Negative 8-bit image """
-    return 255 - img
-
-def simple_highpass(img, cpar):
-    """ Simple highpass is using liboptv preprocess_image """
-    return preprocess_image(img, 0, cpar, 25)
-
-
-def py_set_img(img, i):
-    """Not used anymore, was transferring images to the C"""
-    pass
-
-
-def py_start_proc_c(n_cams):
-    """Read parameters"""
-
-    # Control parameters
-    cpar = ControlParams(n_cams)
-    cpar.read_control_par(b"parameters/ptv.par")
-
-    # Sequence parameters
-    spar = SequenceParams(num_cams=n_cams)
-    spar.read_sequence_par(b"parameters/sequence.par", n_cams)
-
-    # Volume parameters
-    vpar = VolumeParams()
-    vpar.read_volume_par(b"parameters/criteria.par")
-
-    # Tracking parameters
-    track_par = TrackingParams()
-    track_par.read_track_par(b"parameters/track.par")
-
-    # Target parameters
-    tpar = TargetParams(n_cams)
-    tpar.read(b"parameters/targ_rec.par")
-
-    # Examine parameters, multiplane (single plane vs combined calibration)
-    epar = par.ExamineParams()
-    epar.read()
-
-    # Calibration parameters
-    cals = []
-    for i_cam in range(n_cams):
-        cal = Calibration()
-        tmp = cpar.get_cal_img_base_name(i_cam)
-        cal.from_file(tmp + b".ori", tmp + b".addpar")
-        cals.append(cal)
-
-    return cpar, spar, vpar, track_par, tpar, cals, epar
-
-
-def py_pre_processing_c(list_of_images, cpar):
-    """Image pre-processing, mostly highpass filter, could be extended in
-    the future
-
-    Inputs:
-        list of images
-        cpar ControlParams()
-    """
-    newlist = []
-    for img in list_of_images:
-        newlist.append(simple_highpass(img, cpar))
-    return newlist
-
-
-def py_detection_proc_c(list_of_images, cpar, tpar, cals):
-    """Detection of targets"""
-
-    pftVersionParams = par.PftVersionParams(path=Path("parameters"))
-    pftVersionParams.read()
-    Existing_Target = bool(pftVersionParams.Existing_Target)
-
-    detections, corrected = [], []
-    for i_cam, img in enumerate(list_of_images):
-        if Existing_Target:
-            targs = read_targets(cpar.get_img_base_name(i_cam), 0)
-        else:
-            targs = target_recognition(img, tpar, i_cam, cpar)
-
-        targs.sort_y()
-        detections.append(targs)
-        mc = MatchedCoords(targs, cpar, cals[i_cam])
-        corrected.append(mc)
-
-    return detections, corrected
-
-
-def py_correspondences_proc_c(exp):
-    """Provides correspondences
-    Inputs:
-        exp = info.object from the pyptv_gui
-    Outputs:
-        quadruplets, ... : four empty lists filled later with the
-    correspondences of quadruplets, triplets, pairs, and so on
-    """
-
-    frame = 123456789  # just a temporary workaround. todo: think how to write
-
-    #        if any([len(det) == 0 for det in detections]):
-    #            return False
-
-    # Corresp. + positions.
-    sorted_pos, sorted_corresp, num_targs = correspondences(
-        exp.detections, exp.corrected, exp.cals, exp.vpar, exp.cpar)
-
-    # Save targets only after they've been modified:
-    for i_cam in range(exp.n_cams):
-        exp.detections[i_cam].write(exp.spar.get_img_base_name(i_cam), frame)
-
-    print("Frame " + str(frame) + " had " +
-          repr([s.shape[1] for s in sorted_pos]) + " correspondences.")
-
-    return sorted_pos, sorted_corresp, num_targs
-
-
-def py_determination_proc_c(n_cams, sorted_pos, sorted_corresp, corrected):
-    """Returns 3d positions"""
-
-    # Control parameters
-    cpar = ControlParams(n_cams)
-    cpar.read_control_par(b"parameters/ptv.par")
-
-    # Volume parameters
-    vpar = VolumeParams()
-    vpar.read_volume_par(b"parameters/criteria.par")
-
-    cals = []
-    for i_cam in range(n_cams):
-        cal = Calibration()
-        tmp = cpar.get_cal_img_base_name(i_cam)
-        cal.from_file(tmp + b".ori", tmp + b".addpar")
-        cals.append(cal)
-
-    # Distinction between quad/trip irrelevant here.
-    sorted_pos = np.concatenate(sorted_pos, axis=1)
-    sorted_corresp = np.concatenate(sorted_corresp, axis=1)
-
-    flat = np.array([
-        corrected[i].get_by_pnrs(sorted_corresp[i]) for i in range(len(cals))
-    ])
-    pos, rcm = point_positions(flat.transpose(1, 0, 2), cpar, cals, vpar)
-
-    if len(cals) < 4:
-        print_corresp = -1 * np.ones((4, sorted_corresp.shape[1]))
-        print_corresp[:len(cals), :] = sorted_corresp
-    else:
-        print_corresp = sorted_corresp
-
-    # Save rt_is in a temporary file
-    fname = b"".join([default_naming["corres"],
-                      b".123456789"])  # hard-coded frame number
-    print(f'Prepared {fname} to write positions\n')
-
-    try:
-        with open(fname, "w", encoding='utf-8') as rt_is:
-            print(f'Opened {fname} \n')
-            rt_is.write(str(pos.shape[0]) + "\n")
-            for pix, pt in enumerate(pos):
-                pt_args = (pix + 1, ) + tuple(pt) + tuple(print_corresp[:, pix])
-                rt_is.write("%4d %9.3f %9.3f %9.3f %4d %4d %4d %4d\n" % pt_args)
-    except FileNotFoundError:
-        msg = "Sorry, the file "+ fname + "does not exist."
-        print(msg) # Sorry, the file John.txt does not exist.
-
-    # rt_is.close()
-
-
-
-def py_sequence_loop(exp):
-    """Runs a sequence of detection, stereo-correspondence, determination and stores
-    the data in the cam#.XXX_targets (rewritten) and rt_is.XXX files. Basically
-    it is to run the batch as in pyptv_batch.py without tracking
-    """
-    n_cams, cpar, spar, vpar, tpar, cals = (
-        exp.n_cams,
-        exp.cpar,
-        exp.spar,
-        exp.vpar,
-        exp.tpar,
-        exp.cals,
-    )
-
-    pftVersionParams = par.PftVersionParams(path=Path("parameters"))
-    pftVersionParams.read()
-    Existing_Target = np.bool8(pftVersionParams.Existing_Target)
-
-    # sequence loop for all frames
-    for frame in range(spar.get_first(), spar.get_last() + 1):
-        # print(f"processing {frame} frame")
-
-        detections = []
-        corrected = []
-        for i_cam in range(n_cams):
-            if Existing_Target:
-                targs = read_targets(spar.get_img_base_name(i_cam), frame)
-            else:
-                # imname = spar.get_img_base_name(i_cam) + str(frame).encode()
-                imname = spar.get_img_base_name(i_cam).decode()
-                imname = Path(imname.replace('#',f'{frame}'))
-                # print(f'Image name {imname}')
-
-                if not imname.exists():
-                    print(f"{imname} does not exist")
-
-                img = imread(imname)
-                # time.sleep(.1) # I'm not sure we need it here
-                
-                if 'exp1' in exp.__dict__:
-                    if exp.exp1.active_params.m_params.Inverse:
-                        print("Invert image")
-                        img = 255 - img
-
-                    if exp.exp1.active_params.m_params.Subtr_Mask:
-                        # print("Subtracting mask")
-                        try:
-                            mask_name = exp.exp1.active_params.m_params.Base_Name_Mask.replace('#',str(i_cam+1))
-                            mask = imread(mask_name)
-                            img[mask] = 0
-
-                        except ValueError:
-                            print("failed to read the mask")
-                    
-                
-                high_pass = simple_highpass(img, cpar)
-                targs = target_recognition(high_pass, tpar, i_cam, cpar)
-
-            targs.sort_y()
-            detections.append(targs)
-            masked_coords = MatchedCoords(targs, cpar, cals[i_cam])
-            pos, _ = masked_coords.as_arrays()
-            corrected.append(masked_coords)
-
-        #        if any([len(det) == 0 for det in detections]):
-        #            return False
-
-        # Corresp. + positions.
-        sorted_pos, sorted_corresp, _ = correspondences(
-            detections, corrected, cals, vpar, cpar)
-
-        # Save targets only after they've been modified:
-        # this is a workaround of the proper way to construct _targets name
-        for i_cam in range(n_cams):
-            detections[i_cam].write(
-                spar.get_img_base_name(i_cam),
-                frame
-                )
-
-        print("Frame " + str(frame) + " had " +
-              repr([s.shape[1] for s in sorted_pos]) + " correspondences.")
-
-        # Distinction between quad/trip irrelevant here.
-        sorted_pos = np.concatenate(sorted_pos, axis=1)
-        sorted_corresp = np.concatenate(sorted_corresp, axis=1)
-
-        flat = np.array([
-            corrected[i].get_by_pnrs(sorted_corresp[i])
-            for i in range(len(cals))
-        ])
-        pos, _ = point_positions(flat.transpose(1, 0, 2), cpar, cals, vpar)
-
-        # if len(cals) == 1: # single camera case
-        #     sorted_corresp = np.tile(sorted_corresp,(4,1))
-        #     sorted_corresp[1:,:] = -1
-
-        if len(cals) < 4:
-            print_corresp = -1 * np.ones((4, sorted_corresp.shape[1]))
-            print_corresp[:len(cals), :] = sorted_corresp
-        else:
-            print_corresp = sorted_corresp
-
-        # Save rt_is
-        rt_is_filename = default_naming["corres"].decode()
-        rt_is_filename = rt_is_filename + f'.{frame}'
-        with open(rt_is_filename, "w", encoding="utf8") as rt_is:
-            rt_is.write(str(pos.shape[0]) + "\n")
-            for pix, pt in enumerate(pos):
-                pt_args = (pix + 1, ) + tuple(pt) + tuple(print_corresp[:, pix])
-                rt_is.write("%4d %9.3f %9.3f %9.3f %4d %4d %4d %4d\n" % pt_args)
-        # rt_is.close()
-    # end of a sequence loop
-
-
-def py_trackcorr_init(exp):
-    """Reads all the necessary stuff into Tracker"""
-    tracker = Tracker(exp.cpar, exp.vpar, exp.track_par, exp.spar, exp.cals,
-                      default_naming)
-    return tracker
-
-
-def py_trackcorr_loop():
-    """Supposedly returns some lists of the linked targets at every step of a tracker"""
-    pass
-
-
-def py_traject_loop():
-    """Used to plot trajectories after the full run
-
-    def py_traject_loop(seq):
-    global intx1_tr,intx2_tr,inty1_tr,inty2_tr,m1_tr
-    trajectories_c(seq, cpar)
-    intx1,intx2,inty1,inty2=[],[],[],[]
-
-    for i in range(cpar[0].num_cams):
-        intx1_t,intx2_t,inty1_t,inty2_t=[],[],[],[]
-        for j in range(m1_tr):
-            intx1_t.append(intx1_tr[i][j])
-            inty1_t.append(inty1_tr[i][j])
-            intx2_t.append(intx2_tr[i][j])
-            inty2_t.append(inty2_tr[i][j])
-        intx1.append(intx1_t)
-        inty1.append(inty1_t)
-        intx2.append(intx2_t)
-        inty2.append(inty2_t)
-    return intx1,inty1,intx2,inty2,m1_tr
-
-    """
-
-
-# ------- Utilities ----------#
-
-
-def py_rclick_delete(x, y, n):
-    """a tool to delete clicked points
-
-    def py_right_click(int coord_x, int coord_y, n_image):
-    global rclick_intx1,rclick_inty1,rclick_intx2,rclick_inty2,rclick_points_x1, rclick_points_y1,rclick_count,rclick_points_intx1, rclick_points_inty1
-
-    x2_points,y2_points,x1,y1,x2,y2=[],[],[],[],[],[]
-
-    cdef volume_par *vpar = read_volume_par("parameters/criteria.par")
-    r = mouse_proc_c (coord_x, coord_y, 3, n_image, vpar, cpar)
-    free(vpar)
-
-    if r == -1:
-        return -1,-1,-1,-1,-1,-1,-1,-1
-    for i in range(cpar[0].num_cams):
-        x2_temp,y2_temp=[],[]
-        for j in range(rclick_count[i]):
-            x2_temp.append(rclick_points_x1[i][j])
-            y2_temp.append(rclick_points_y1[i][j])
-
-        x2_points.append(x2_temp)
-        y2_points.append(y2_temp)
-        x1.append(rclick_intx1[i])
-        y1.append(rclick_inty1[i])
-        x2.append(rclick_intx2[i])
-        y2.append(rclick_inty2[i])
-
-    return  x1,y1,x2,y2,x2_points,y2_points,rclick_points_intx1, rclick_points_inty1
-
-
-    """
-    pass
-
-
-def py_get_pix_N(x, y, n):
-    """
-    def py_get_pix_N(x,y,n_image):
-    global pix
-    cdef int i,j
-    i=n_image
-    x1=[]
-    y1=[]
-    for j in range(num[i]):
-        x1.append(pix[i][j].x)
-        y1.append(pix[i][j].y)
-        x.append(x1)
-        y.append(y1)
-
-    """
-    pass
-
-
-def py_get_pix(x, y):
-    """
-    Returns a list of lists of target positions
-
-    def py_get_pix(x,y):
-    global pix
-    cdef int i,j
-    for i in range(cpar[0].num_cams):
-        x1=[]
-        y1=[]
-        for j in range(num[i]):
-            x1.append(pix[i][j].x)
-            y1.append(pix[i][j].y)
-        x.append(x1)
-        y.append(y1)
-
-    """
-    return x, y
-
-
-def py_calibration(selection):
-    """Calibration
-    def py_calibration(sel):
-    calibration_proc_c(sel)"""
-    if selection == 1:  # read calibration parameters into liboptv
-        pass
-
-    if selection == 2:  # run detection of targets
-        pass
-
-    if selection == 9:  # initial guess
-        """Reads from a target file the 3D points and projects them on
-        the calibration images
-        It is the same function as show trajectories, just read from a different
-        file
-        """
-
-
-def py_multiplanecalibration(exp):
-    """Performs multiplane calibration, in which for all cameras the pre-processed plane in multiplane.par al combined.
-    Overwrites the ori and addpar files of the cameras specified in cal_ori.par of the multiplane parameter folder
-    """
-
-    for i_cam in range(exp.n_cams):  # iterate over all cameras
-        all_known = []
-        all_detected = []
-        for i in range(exp.MultiParams.n_planes):  # combine all single planes
-
-            c = exp.calParams.img_ori[i_cam][-9]  # Get camera id
-
-            file_known = exp.MultiParams.plane_name[i] + str(c) + ".tif.fix"
-            file_detected = exp.MultiParams.plane_name[i] + str(c) + ".tif.crd"
-
-            # Load calibration point information from plane i
-            known = np.loadtxt(file_known)
-            detected = np.loadtxt(file_detected)
-
-            if np.any(detected == -999):
-                raise ValueError(
-                    ("Using undetected points in {} will cause " +
-                     "silliness. Quitting.").format(file_detected))
-
-            num_known = len(known)
-            num_detect = len(detected)
-
-            if num_known != num_detect:
-                raise ValueError(
-                    "Number of detected points (%d) does not match" +
-                    " number of known points (%d) for %s, %s" %
-                    (num_known, num_detect, file_known, file_detected))
-
-            if len(all_known) > 0:
-                detected[:, 0] = (all_detected[-1][-1, 0] + 1 +
-                                  np.arange(len(detected)))
-
-            # Append to list of total known and detected points
-            all_known.append(known)
-            all_detected.append(detected)
-
-        # Make into the format needed for full_calibration.
-        all_known = np.vstack(all_known)[:, 1:]
-        all_detected = np.vstack(all_detected)
-
-        targs = TargetArray(len(all_detected))
-        for tix in range(len(all_detected)):
-            targ = targs[tix]
-            det = all_detected[tix]
-
-            targ.set_pnr(tix)
-            targ.set_pos(det[1:])
-
-        # backup the ORI/ADDPAR files first
-        exp.backup_ori_files()
-
-        op = par.OrientParams()
-        op.read()
-
-        # recognized names for the flags:
-        names = [
-            "cc",
-            "xh",
-            "yh",
-            "k1",
-            "k2",
-            "k3",
-            "p1",
-            "p2",
-            "scale",
-            "shear",
-        ]
-        op_names = [
-            op.cc,
-            op.xh,
-            op.yh,
-            op.k1,
-            op.k2,
-            op.k3,
-            op.p1,
-            op.p2,
-            op.scale,
-            op.shear,
-        ]
-
-        flags = []
-        for name, op_name in zip(names, op_names):
-            if op_name == 1:
-                flags.append(name)
-
-        # Run the multiplane calibration
-        residuals, targ_ix, err_est = full_calibration(exp.cals[0], all_known,
-                                                       targs, exp.cpar, flags)
-
-        # Save the results
-        exp._write_ori(i_cam,
-                       addpar_flag=True)  # addpar_flag to save addpar file
-        print("End multiplane")
+from pathlib import Path
+import numpy as np
+from optv.calibration import Calibration
+from optv.correspondences import correspondences, MatchedCoords
+from optv.image_processing import preprocess_image
+from optv.orientation import (
+    point_positions,
+    external_calibration,
+    full_calibration,
+)
+from optv.parameters import (
+    ControlParams,
+    VolumeParams,
+    TrackingParams,
+    SequenceParams,
+    TargetParams,
+)
+from optv.segmentation import target_recognition
+from optv.tracking_framebuf import CORRES_NONE, read_targets, TargetArray
+from optv.tracker import Tracker, default_naming
+from optv.epipolar import epipolar_curve
+from skimage.io import imread
+from pyptv import parameters as par
+
+
+def negative(img):
+    """ Negative 8-bit image """
+    return 255 - img
+
+def simple_highpass(img, cpar):
+    """ Simple highpass is using liboptv preprocess_image """
+    return preprocess_image(img, 0, cpar, 25)
+
+
+def py_set_img(img, i):
+    """Not used anymore, was transferring images to the C"""
+    pass
+
+
+def py_start_proc_c(n_cams):
+    """Read parameters"""
+
+    # Control parameters
+    cpar = ControlParams(n_cams)
+    cpar.read_control_par(b"parameters/ptv.par")
+
+    # Sequence parameters
+    spar = SequenceParams(num_cams=n_cams)
+    spar.read_sequence_par(b"parameters/sequence.par", n_cams)
+
+    # Volume parameters
+    vpar = VolumeParams()
+    vpar.read_volume_par(b"parameters/criteria.par")
+
+    # Tracking parameters
+    track_par = TrackingParams()
+    track_par.read_track_par(b"parameters/track.par")
+
+    # Target parameters
+    tpar = TargetParams(n_cams)
+    tpar.read(b"parameters/targ_rec.par")
+
+    # Examine parameters, multiplane (single plane vs combined calibration)
+    epar = par.ExamineParams()
+    epar.read()
+
+    # Calibration parameters
+    cals = []
+    for i_cam in range(n_cams):
+        cal = Calibration()
+        tmp = cpar.get_cal_img_base_name(i_cam)
+        cal.from_file(tmp + b".ori", tmp + b".addpar")
+        cals.append(cal)
+
+    return cpar, spar, vpar, track_par, tpar, cals, epar
+
+
+def py_pre_processing_c(list_of_images, cpar):
+    """Image pre-processing, mostly highpass filter, could be extended in
+    the future
+
+    Inputs:
+        list of images
+        cpar ControlParams()
+    """
+    newlist = []
+    for img in list_of_images:
+        newlist.append(simple_highpass(img, cpar))
+    return newlist
+
+
+def py_detection_proc_c(list_of_images, cpar, tpar, cals):
+    """Detection of targets"""
+
+    pftVersionParams = par.PftVersionParams(path=Path("parameters"))
+    pftVersionParams.read()
+    Existing_Target = bool(pftVersionParams.Existing_Target)
+
+    detections, corrected = [], []
+    for i_cam, img in enumerate(list_of_images):
+        if Existing_Target:
+            targs = read_targets(cpar.get_img_base_name(i_cam), 0)
+        else:
+            targs = target_recognition(img, tpar, i_cam, cpar)
+
+        targs.sort_y()
+        detections.append(targs)
+        mc = MatchedCoords(targs, cpar, cals[i_cam])
+        corrected.append(mc)
+
+    return detections, corrected
+
+
+def py_correspondences_proc_c(exp):
+    """Provides correspondences
+    Inputs:
+        exp = info.object from the pyptv_gui
+    Outputs:
+        quadruplets, ... : four empty lists filled later with the
+    correspondences of quadruplets, triplets, pairs, and so on
+    """
+
+    frame = 123456789  # just a temporary workaround. todo: think how to write
+
+    #        if any([len(det) == 0 for det in detections]):
+    #            return False
+
+    # Corresp. + positions.
+    sorted_pos, sorted_corresp, num_targs = correspondences(
+        exp.detections, exp.corrected, exp.cals, exp.vpar, exp.cpar)
+
+    # Save targets only after they've been modified:
+    for i_cam in range(exp.n_cams):
+        exp.detections[i_cam].write(exp.spar.get_img_base_name(i_cam), frame)
+
+    print("Frame " + str(frame) + " had " +
+          repr([s.shape[1] for s in sorted_pos]) + " correspondences.")
+
+    return sorted_pos, sorted_corresp, num_targs
+
+
+def py_determination_proc_c(n_cams, sorted_pos, sorted_corresp, corrected):
+    """Returns 3d positions"""
+
+    # Control parameters
+    cpar = ControlParams(n_cams)
+    cpar.read_control_par(b"parameters/ptv.par")
+
+    # Volume parameters
+    vpar = VolumeParams()
+    vpar.read_volume_par(b"parameters/criteria.par")
+
+    cals = []
+    for i_cam in range(n_cams):
+        cal = Calibration()
+        tmp = cpar.get_cal_img_base_name(i_cam)
+        cal.from_file(tmp + b".ori", tmp + b".addpar")
+        cals.append(cal)
+
+    # Distinction between quad/trip irrelevant here.
+    sorted_pos = np.concatenate(sorted_pos, axis=1)
+    sorted_corresp = np.concatenate(sorted_corresp, axis=1)
+
+    flat = np.array([
+        corrected[i].get_by_pnrs(sorted_corresp[i]) for i in range(len(cals))
+    ])
+    pos, rcm = point_positions(flat.transpose(1, 0, 2), cpar, cals, vpar)
+
+    if len(cals) < 4:
+        print_corresp = -1 * np.ones((4, sorted_corresp.shape[1]))
+        print_corresp[:len(cals), :] = sorted_corresp
+    else:
+        print_corresp = sorted_corresp
+
+    # Save rt_is in a temporary file
+    fname = b"".join([default_naming["corres"],
+                      b".123456789"])  # hard-coded frame number
+    print(f'Prepared {fname} to write positions\n')
+
+    try:
+        with open(fname, "w", encoding='utf-8') as rt_is:
+            print(f'Opened {fname} \n')
+            rt_is.write(str(pos.shape[0]) + "\n")
+            for pix, pt in enumerate(pos):
+                pt_args = (pix + 1, ) + tuple(pt) + tuple(print_corresp[:, pix])
+                rt_is.write("%4d %9.3f %9.3f %9.3f %4d %4d %4d %4d\n" % pt_args)
+    except FileNotFoundError:
+        msg = "Sorry, the file "+ fname + "does not exist."
+        print(msg) # Sorry, the file John.txt does not exist.
+
+    # rt_is.close()
+
+
+
+def py_sequence_loop(exp):
+    """Runs a sequence of detection, stereo-correspondence, determination and stores
+    the data in the cam#.XXX_targets (rewritten) and rt_is.XXX files. Basically
+    it is to run the batch as in pyptv_batch.py without tracking
+    """
+    n_cams, cpar, spar, vpar, tpar, cals = (
+        exp.n_cams,
+        exp.cpar,
+        exp.spar,
+        exp.vpar,
+        exp.tpar,
+        exp.cals,
+    )
+
+    pftVersionParams = par.PftVersionParams(path=Path("parameters"))
+    pftVersionParams.read()
+    Existing_Target = np.bool8(pftVersionParams.Existing_Target)
+
+    # sequence loop for all frames
+    for frame in range(spar.get_first(), spar.get_last() + 1):
+        # print(f"processing {frame} frame")
+
+        detections = []
+        corrected = []
+        for i_cam in range(n_cams):
+            if Existing_Target:
+                targs = read_targets(spar.get_img_base_name(i_cam), frame)
+            else:
+                # imname = spar.get_img_base_name(i_cam) + str(frame).encode()
+                imname = spar.get_img_base_name(i_cam).decode()
+                imname = Path(imname.replace('#',f'{frame}'))
+                # print(f'Image name {imname}')
+
+                if not imname.exists():
+                    print(f"{imname} does not exist")
+
+                img = imread(imname)
+                # time.sleep(.1) # I'm not sure we need it here
+                
+                if 'exp1' in exp.__dict__:
+                    if exp.exp1.active_params.m_params.Inverse:
+                        print("Invert image")
+                        img = 255 - img
+
+                    if exp.exp1.active_params.m_params.Subtr_Mask:
+                        # print("Subtracting mask")
+                        try:
+                            mask_name = exp.exp1.active_params.m_params.Base_Name_Mask.replace('#',str(i_cam+1))
+                            mask = imread(mask_name)
+                            img[mask] = 0
+
+                        except ValueError:
+                            print("failed to read the mask")
+                    
+                
+                high_pass = simple_highpass(img, cpar)
+                targs = target_recognition(high_pass, tpar, i_cam, cpar)
+
+            targs.sort_y()
+            detections.append(targs)
+            masked_coords = MatchedCoords(targs, cpar, cals[i_cam])
+            pos, _ = masked_coords.as_arrays()
+            corrected.append(masked_coords)
+
+        #        if any([len(det) == 0 for det in detections]):
+        #            return False
+
+        # Corresp. + positions.
+        sorted_pos, sorted_corresp, _ = correspondences(
+            detections, corrected, cals, vpar, cpar)
+
+        # Save targets only after they've been modified:
+        # this is a workaround of the proper way to construct _targets name
+        for i_cam in range(n_cams):
+            detections[i_cam].write(
+                spar.get_img_base_name(i_cam),
+                frame
+                )
+
+        print("Frame " + str(frame) + " had " +
+              repr([s.shape[1] for s in sorted_pos]) + " correspondences.")
+
+        # Distinction between quad/trip irrelevant here.
+        sorted_pos = np.concatenate(sorted_pos, axis=1)
+        sorted_corresp = np.concatenate(sorted_corresp, axis=1)
+
+        flat = np.array([
+            corrected[i].get_by_pnrs(sorted_corresp[i])
+            for i in range(len(cals))
+        ])
+        pos, _ = point_positions(flat.transpose(1, 0, 2), cpar, cals, vpar)
+
+        # if len(cals) == 1: # single camera case
+        #     sorted_corresp = np.tile(sorted_corresp,(4,1))
+        #     sorted_corresp[1:,:] = -1
+
+        if len(cals) < 4:
+            print_corresp = -1 * np.ones((4, sorted_corresp.shape[1]))
+            print_corresp[:len(cals), :] = sorted_corresp
+        else:
+            print_corresp = sorted_corresp
+
+        # Save rt_is
+        rt_is_filename = default_naming["corres"].decode()
+        rt_is_filename = rt_is_filename + f'.{frame}'
+        with open(rt_is_filename, "w", encoding="utf8") as rt_is:
+            rt_is.write(str(pos.shape[0]) + "\n")
+            for pix, pt in enumerate(pos):
+                pt_args = (pix + 1, ) + tuple(pt) + tuple(print_corresp[:, pix])
+                rt_is.write("%4d %9.3f %9.3f %9.3f %4d %4d %4d %4d\n" % pt_args)
+        # rt_is.close()
+    # end of a sequence loop
+
+
+def py_trackcorr_init(exp):
+    """Reads all the necessary stuff into Tracker"""
+    tracker = Tracker(exp.cpar, exp.vpar, exp.track_par, exp.spar, exp.cals,
+                      default_naming)
+    return tracker
+
+
+def py_trackcorr_loop():
+    """Supposedly returns some lists of the linked targets at every step of a tracker"""
+    pass
+
+
+def py_traject_loop():
+    """Used to plot trajectories after the full run
+
+    def py_traject_loop(seq):
+    global intx1_tr,intx2_tr,inty1_tr,inty2_tr,m1_tr
+    trajectories_c(seq, cpar)
+    intx1,intx2,inty1,inty2=[],[],[],[]
+
+    for i in range(cpar[0].num_cams):
+        intx1_t,intx2_t,inty1_t,inty2_t=[],[],[],[]
+        for j in range(m1_tr):
+            intx1_t.append(intx1_tr[i][j])
+            inty1_t.append(inty1_tr[i][j])
+            intx2_t.append(intx2_tr[i][j])
+            inty2_t.append(inty2_tr[i][j])
+        intx1.append(intx1_t)
+        inty1.append(inty1_t)
+        intx2.append(intx2_t)
+        inty2.append(inty2_t)
+    return intx1,inty1,intx2,inty2,m1_tr
+
+    """
+
+
+# ------- Utilities ----------#
+
+
+def py_rclick_delete(x, y, n):
+    """a tool to delete clicked points
+
+    def py_right_click(int coord_x, int coord_y, n_image):
+    global rclick_intx1,rclick_inty1,rclick_intx2,rclick_inty2,rclick_points_x1, rclick_points_y1,rclick_count,rclick_points_intx1, rclick_points_inty1
+
+    x2_points,y2_points,x1,y1,x2,y2=[],[],[],[],[],[]
+
+    cdef volume_par *vpar = read_volume_par("parameters/criteria.par")
+    r = mouse_proc_c (coord_x, coord_y, 3, n_image, vpar, cpar)
+    free(vpar)
+
+    if r == -1:
+        return -1,-1,-1,-1,-1,-1,-1,-1
+    for i in range(cpar[0].num_cams):
+        x2_temp,y2_temp=[],[]
+        for j in range(rclick_count[i]):
+            x2_temp.append(rclick_points_x1[i][j])
+            y2_temp.append(rclick_points_y1[i][j])
+
+        x2_points.append(x2_temp)
+        y2_points.append(y2_temp)
+        x1.append(rclick_intx1[i])
+        y1.append(rclick_inty1[i])
+        x2.append(rclick_intx2[i])
+        y2.append(rclick_inty2[i])
+
+    return  x1,y1,x2,y2,x2_points,y2_points,rclick_points_intx1, rclick_points_inty1
+
+
+    """
+    pass
+
+
+def py_get_pix_N(x, y, n):
+    """
+    def py_get_pix_N(x,y,n_image):
+    global pix
+    cdef int i,j
+    i=n_image
+    x1=[]
+    y1=[]
+    for j in range(num[i]):
+        x1.append(pix[i][j].x)
+        y1.append(pix[i][j].y)
+        x.append(x1)
+        y.append(y1)
+
+    """
+    pass
+
+
+def py_get_pix(x, y):
+    """
+    Returns a list of lists of target positions
+
+    def py_get_pix(x,y):
+    global pix
+    cdef int i,j
+    for i in range(cpar[0].num_cams):
+        x1=[]
+        y1=[]
+        for j in range(num[i]):
+            x1.append(pix[i][j].x)
+            y1.append(pix[i][j].y)
+        x.append(x1)
+        y.append(y1)
+
+    """
+    return x, y
+
+
+def py_calibration(selection):
+    """Calibration
+    def py_calibration(sel):
+    calibration_proc_c(sel)"""
+    if selection == 1:  # read calibration parameters into liboptv
+        pass
+
+    if selection == 2:  # run detection of targets
+        pass
+
+    if selection == 9:  # initial guess
+        """Reads from a target file the 3D points and projects them on
+        the calibration images
+        It is the same function as show trajectories, just read from a different
+        file
+        """
+
+
+def py_multiplanecalibration(exp):
+    """Performs multiplane calibration, in which for all cameras the pre-processed plane in multiplane.par al combined.
+    Overwrites the ori and addpar files of the cameras specified in cal_ori.par of the multiplane parameter folder
+    """
+
+    for i_cam in range(exp.n_cams):  # iterate over all cameras
+        all_known = []
+        all_detected = []
+        for i in range(exp.MultiParams.n_planes):  # combine all single planes
+
+            c = exp.calParams.img_ori[i_cam][-9]  # Get camera id
+
+            file_known = exp.MultiParams.plane_name[i] + str(c) + ".tif.fix"
+            file_detected = exp.MultiParams.plane_name[i] + str(c) + ".tif.crd"
+
+            # Load calibration point information from plane i
+            known = np.loadtxt(file_known)
+            detected = np.loadtxt(file_detected)
+
+            if np.any(detected == -999):
+                raise ValueError(
+                    ("Using undetected points in {} will cause " +
+                     "silliness. Quitting.").format(file_detected))
+
+            num_known = len(known)
+            num_detect = len(detected)
+
+            if num_known != num_detect:
+                raise ValueError(
+                    "Number of detected points (%d) does not match" +
+                    " number of known points (%d) for %s, %s" %
+                    (num_known, num_detect, file_known, file_detected))
+
+            if len(all_known) > 0:
+                detected[:, 0] = (all_detected[-1][-1, 0] + 1 +
+                                  np.arange(len(detected)))
+
+            # Append to list of total known and detected points
+            all_known.append(known)
+            all_detected.append(detected)
+
+        # Make into the format needed for full_calibration.
+        all_known = np.vstack(all_known)[:, 1:]
+        all_detected = np.vstack(all_detected)
+
+        targs = TargetArray(len(all_detected))
+        for tix in range(len(all_detected)):
+            targ = targs[tix]
+            det = all_detected[tix]
+
+            targ.set_pnr(tix)
+            targ.set_pos(det[1:])
+
+        # backup the ORI/ADDPAR files first
+        exp.backup_ori_files()
+
+        op = par.OrientParams()
+        op.read()
+
+        # recognized names for the flags:
+        names = [
+            "cc",
+            "xh",
+            "yh",
+            "k1",
+            "k2",
+            "k3",
+            "p1",
+            "p2",
+            "scale",
+            "shear",
+        ]
+        op_names = [
+            op.cc,
+            op.xh,
+            op.yh,
+            op.k1,
+            op.k2,
+            op.k3,
+            op.p1,
+            op.p2,
+            op.scale,
+            op.shear,
+        ]
+
+        flags = []
+        for name, op_name in zip(names, op_names):
+            if op_name == 1:
+                flags.append(name)
+
+        # Run the multiplane calibration
+        residuals, targ_ix, err_est = full_calibration(exp.cals[0], all_known,
+                                                       targs, exp.cpar, flags)
+
+        # Save the results
+        exp._write_ori(i_cam,
+                       addpar_flag=True)  # addpar_flag to save addpar file
+        print("End multiplane")
```

### Comparing `pyptv-0.2.2/pyptv/pyptv_gui.py` & `pyptv-0.2.3/pyptv/pyptv_gui.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,1507 +1,1512 @@
-""" PyPTV_GUI is the GUI for the OpenPTV (www.openptv.net) written in
-Python with Traits, TraitsUI, Numpy, Scipy and Chaco
-
-Copyright (c) 2008-2023, Turbulence Structure Laboratory, Tel Aviv University
-The GUI software is distributed under the terms of MIT-like license
-http://opensource.org/licenses/MIT
-
-OpenPTV library is distributed under the terms of LGPL license
-see http://www.openptv.net for more details.
-
-"""
-from __future__ import division
-
-
-import os
-from pathlib import Path, PurePath
-import sys
-import time
-import importlib
-
-import numpy as np
-import optv
-from traits.api import HasTraits, Int, Bool, Instance, List, Enum, Any
-from traitsui.api import (
-    View,
-    Item,
-    ListEditor,
-    Handler,
-    TreeEditor,
-    TreeNode,
-    Separator,
-    Group,
-)
-from traitsui.menu import Action, Menu, MenuBar
-from chaco.api import ArrayDataSource, ArrayPlotData, LinearMapper, Plot, ImagePlot, gray
-from chaco.tools.api import PanTool, ZoomTool
-from chaco.tools.image_inspector_tool import ImageInspectorTool
-from enable.component_editor import ComponentEditor
-from skimage.util import img_as_ubyte
-from skimage.color import rgb2gray
-from skimage.io import imread
-
-from pyptv import parameters as par
-from pyptv import ptv
-from pyptv.calibration_gui import CalibrationGUI
-from pyptv.directory_editor import DirectoryEditorDialog
-from pyptv.parameter_gui import Experiment, Paramset
-from pyptv.quiverplot import QuiverPlot
-from pyptv.detection_gui import DetectionGUI
-import optv.orientation
-
-
-class Clicker(ImageInspectorTool):
-    """
-    Clicker class handles right mouse click actions from the tree
-    and menubar actions
-    """
-    left_changed = Int(0)
-    right_changed = Int(0)
-    x,y = 0,0
-
-    def __init__(self, *args, **kwargs):
-        # Clicker.__init__(self,*args, **kwargs)
-        super(Clicker, self).__init__(*args, **kwargs)
-
-    def normal_left_down(self, event):
-        """Handles the left mouse button being clicked.
-        Fires the **new_value** event with the data (if any) from the event's
-        position.
-        """
-        plot = self.component
-        if plot is not None:
-            self.x, self.y = plot.map_index((event.x, event.y))
-            self.data_value = plot.value.data[self.y, self.x]
-            self.last_mouse_position = (event.x, event.y)
-            self.left_changed = 1 - self.left_changed
-            # print(f"left: x={self.x}, y={self.y}, I={self.data_value}, {self.left_changed}")
-            
-
-    def normal_right_down(self, event):
-        plot = self.component
-        if plot is not None:
-            self.x, self.y = plot.map_index((event.x, event.y))
-            self.last_mouse_position = (event.x, event.y)
-            self.data_value = plot.value.data[self.y, self.x]
-            # print(f"right: x={self.x}, y={self.y}, I={self.data_value}")
-            self.right_changed = 1 - self.right_changed
-            
-        
-
-    # def normal_mouse_move(self, event):
-    #     pass
-
-
-
-# --------------------------------------------------------------
-class CameraWindow(HasTraits):
-    """CameraWindow class contains the relevant information and functions for
-    a single camera window: image, zoom, pan important members:
-    _plot_data  - contains image data to display (used by update_image)
-    _plot - instance of Plot class to use with _plot_data
-    _click_tool - instance of Clicker tool for the single camera window,
-    to handle mouse processing
-    """
-
-    _plot = Instance(Plot)
-    _click_tool = Instance(Clicker)
-    rclicked = Int(0)
-
-    cam_color = ""
-    name = ""
-    view = View(Item(name="_plot", editor=ComponentEditor(), show_label=False))
-
-    def __init__(self, color, name):
-        """
-        Initialization of plot system
-        """
-        super(HasTraits, self).__init__()
-        padd = 25
-        self._plot_data = ArrayPlotData() # we need set_data
-        self._plot = Plot(self._plot_data, default_origin="top left")
-        self._plot.padding_left = padd
-        self._plot.padding_right = padd
-        self._plot.padding_top = padd
-        self._plot.padding_bottom = padd
-        (
-            self.right_p_x0,
-            self.right_p_y0,
-            self.right_p_x1,
-            self.right_p_y1,
-            self._quiverplots,
-        ) = ([], [], [], [], [])
-        self.cam_color = color
-        self.name = name
-        
-
-    def attach_tools(self):
-        """attach_tools(self) contains the relevant tools:
-        clicker, pan, zoom"""
-      
-        print(f" Attaching clicker to camera {self.name}")
-        self._click_tool = Clicker(component=self._img_plot)
-        self._click_tool.on_trait_change(self.left_clicked_event, "left_changed")
-        self._click_tool.on_trait_change(self.right_clicked_event, "right_changed")
-        # self._img_plot.tools.clear()
-        self._img_plot.tools.append(self._click_tool)
-        
-        pan = PanTool(self._plot, drag_button="middle")
-        zoom_tool = ZoomTool(self._plot, tool_mode="box", always_on=False)
-        zoom_tool.max_zoom_out_factor = 1.0  # Disable "bird view" zoom out
-        self._img_plot.overlays.append(zoom_tool)
-        self._img_plot.tools.append(pan)
-        # print(self._img_plot.tools)
-        
-
-    def left_clicked_event(
-        self,
-    ):  # TODO: why do we need the ClickerTool if we can handle mouse
-        # clicks here?
-        """left_clicked_event - processes left click mouse
-        events and displays coordinate and grey value information
-        on the screen
-        """
-        print(
-            f"x={self._click_tool.x} pix,y={self._click_tool.y} pix,I={self._click_tool.data_value}"
-        )
-        
-    def right_clicked_event(self):
-        """right mouse button click event flag"""
-        # # self._click_tool.right_changed = 1
-        # print(
-        #     f"right_clicked, x={self._click_tool.x} pix,y={self._click_tool.y} pix, I={self._click_tool.data_value}, {self.rclicked}"
-        # )
-        self.rclicked = 1
-
-        
-    def create_image(self, image, is_float=False):
-        """create_image - displays/updates image in the current camera window
-        parameters:
-            image - image data
-            is_float - if true, displays an image as float array,
-            else displays as byte array (B&W or gray)
-        example usage:
-            create_image(image,is_float=False)
-        """
-        # print('image shape = ', image.shape, 'is_float =', is_float)
-        # if image.ndim > 2:
-        #     image = img_as_ubyte(rgb2gray(image))
-        #     is_float = False
-
-        if is_float:
-            self._plot_data.set_data("imagedata", image.astype(np.float32))
-        else:
-            self._plot_data.set_data("imagedata", image.astype(np.uint8))
-
-        # if not hasattr(
-        #         self,
-        #         "img_plot"):  # make a new plot if there is nothing to update
-        #     self.img_plot = Instance(ImagePlot)
-
-        self._img_plot = self._plot.img_plot("imagedata", colormap=gray)[0]
-        self.attach_tools()
-
-    def update_image(self, image, is_float=False):
-        """update_image - displays/updates image in the current camera window
-        parameters:
-            image - image data
-            is_float - if true, displays an image as float array,
-            else displays as byte array (B&W or gray)
-        example usage:
-            update_image(image,is_float=False)
-        """
-
-        if is_float:
-            self._plot_data.set_data("imagedata", image.astype(np.float32))
-        else:
-            self._plot_data.set_data("imagedata", image.astype(np.uint8))
-
-        self._plot.img_plot("imagedata", colormap=gray)[0]
-        self._plot.request_redraw()
-
-    def drawcross(self, str_x, str_y, x, y, color, mrk_size, marker="plus"):
-        """drawcross draws crosses at a given location (x,y) using color
-        and marker in the current camera window parameters:
-            str_x - label for x coordinates
-            str_y - label for y coordinates
-            x - array of x coordinates
-            y - array of y coordinates
-            mrk_size - marker size
-            marker - type of marker, e.g "plus","circle"
-        example usage:
-            drawcross("coord_x","coord_y",[100,200,300],[100,200,300],2)
-            draws plus markers of size 2 at points
-                (100,100),(200,200),(200,300)
-            :rtype:
-        """
-        self._plot_data.set_data(str_x, np.atleast_1d(x))
-        self._plot_data.set_data(str_y, np.atleast_1d(y))
-        self._plot.plot(
-            (str_x, str_y),
-            type="scatter",
-            color=color,
-            marker=marker,
-            marker_size=mrk_size,
-        )
-        self._plot.request_redraw()
-
-    def drawquiver(self, x1c, y1c, x2c, y2c, color, linewidth=1.0):
-        """Draws multiple lines at once on the screen x1,y1->x2,y2 in the
-        current camera window
-        parameters:
-            x1c - array of x1 coordinates
-            y1c - array of y1 coordinates
-            x2c - array of x2 coordinates
-            y2c - array of y2 coordinates
-            color - color of the line
-            linewidth - linewidth of the line
-        example usage:
-            drawquiver ([100,200],[100,100],[400,400],[300,200],\
-                'red',linewidth=2.0)
-            draws 2 red lines with thickness = 2 :  \
-                100,100->400,300 and 200,100->400,200
-
-        """
-        x1, y1, x2, y2 = self.remove_short_lines(x1c, y1c, x2c, y2c)
-        if len(x1) > 0:
-            xs = ArrayDataSource(x1)
-            ys = ArrayDataSource(y1)
-
-            quiverplot = QuiverPlot(
-                index=xs,
-                value=ys,
-                index_mapper=LinearMapper(range=self._plot.index_mapper.range),
-                value_mapper=LinearMapper(range=self._plot.value_mapper.range),
-                origin=self._plot.origin,
-                arrow_size=0,
-                line_color=color,
-                line_width=linewidth,
-                ep_index=np.array(x2),
-                ep_value=np.array(y2),
-            )
-            # Seems to be incorrect use of .add
-            # self._plot.add(quiverplot)
-            self._plot.overlays.append(quiverplot)
-
-            # we need this to track how many quiverplots are in the current
-            # plot
-            self._quiverplots.append(quiverplot)
-
-    @staticmethod
-    def remove_short_lines(x1, y1, x2, y2):
-        """removes short lines from the array of lines
-        parameters:
-            x1,y1,x2,y2 - start and end coordinates of the lines
-        returns:
-            x1f,y1f,x2f,y2f - start and end coordinates of the lines,
-            with short lines removed example usage:
-            x1,y1,x2,y2 = remove_short_lines( \
-                [100,200,300],[100,200,300],[100,200,300],[102,210,320])
-            3 input lines, 1 short line will be removed (100,100->100,102)
-            returned coordinates:
-            x1=[200,300]; y1=[200,300]; x2=[200,300]; y2=[210,320]
-        """
-        dx, dy = 2, 2  # minimum allowable dx,dy
-        x1f, y1f, x2f, y2f = [], [], [], []
-        for i in range(len(x1)):
-            if abs(x1[i] - x2[i]) > dx or abs(y1[i] - y2[i]) > dy:
-                x1f.append(x1[i])
-                y1f.append(y1[i])
-                x2f.append(x2[i])
-                y2f.append(y2[i])
-        return x1f, y1f, x2f, y2f
-
-    def drawline(self, str_x, str_y, x1, y1, x2, y2, color1):
-        """drawline draws 1 line on the screen by using lineplot x1,y1->x2,y2
-        parameters:
-            str_x - label of x coordinate
-            str_y - label of y coordinate
-            x1,y1,x2,y2 - start and end coordinates of the line
-            color1 - color of the line
-        example usage:
-            drawline("x_coord","y_coord",100,100,200,200,red)
-            draws a red line 100,100->200,200
-        """
-        # imx, imy = self._plot_data.get_data('imagedata').shape
-        self._plot_data.set_data(str_x, [x1, x2])
-        self._plot_data.set_data(str_y, [y1, y2])
-        self._plot.plot((str_x, str_y), type="line", color=color1)
-
-
-class TreeMenuHandler(Handler):
-    """TreeMenuHanlder contains all the callback actions of menu bar,
-    processing of tree editor, and reactions of the GUI to the user clicks
-    possible function declarations:
-        1) to process menubar actions:
-            def function(self, info):
-        parameters: self - needed for member function declaration,
-                info - contains pointer to calling parent class (e.g main_gui)
-                To access parent class objects use info.object, for example
-                info.object.exp1 gives access to exp1 member of main_gui class
-        2) to process tree editor actions:
-            def function(self,editor,object) - see examples below
-
-    """
-
-    def configure_main_par(self, editor, object):
-        experiment = editor.get_parent(object)
-        paramset = object
-        print("Total paramsets:", len(experiment.paramsets))
-        if paramset.m_params is None:
-            # TODO: is it possible that control reaches here? If not, probably
-            # the if should be removed.
-            paramset.m_params = par.PtvParams()
-        else:
-            paramset.m_params._reload()
-        paramset.m_params.edit_traits(kind="modal")
-
-    def configure_cal_par(self, editor, object):
-        experiment = editor.get_parent(object)
-        paramset = object
-        print(len(experiment.paramsets))
-        if paramset.c_params is None:
-            # TODO: is it possible that control reaches here? If not, probably
-            # the if should be removed.
-            paramset.c_params = par.CalOriParams()  # this is a very questionable line
-        else:
-            paramset.c_params._reload()
-        paramset.c_params.edit_traits(kind="modal")
-
-    def configure_track_par(self, editor, object):
-        experiment = editor.get_parent(object)
-        paramset = object
-        print(len(experiment.paramsets))
-        if paramset.t_params is None:
-            # TODO: is it possible that control reaches here? If not, probably
-            # the if should be removed.
-            paramset.t_params = par.TrackingParams()
-        paramset.t_params.edit_traits(kind="modal")
-
-    def set_active(self, editor, object):
-        """sets a set of parameters as active"""
-        experiment = editor.get_parent(object)
-        paramset = object
-        # experiment.active_params = paramset
-        experiment.setActive(paramset)
-        experiment.changed_active_params = True
-        # editor.object.__init__()
-
-    def copy_set_params(self, editor, object):
-        experiment = editor.get_parent(object)
-        paramset = object
-        print(f" Copying set of parameters \n")
-        print(f"paramset is {paramset.name}")
-        print(f"paramset id is {int(paramset.name.split('Run')[-1])}")
-        # print(f"experiment is {experiment}\n")
-
-        i = 1
-        new_name = None
-        new_dir_path = None
-        flag = False
-        while not flag:
-            new_name = f"{paramset.name}_{i}"
-            new_dir_path = Path(f"{par.par_dir_prefix}{new_name}")
-            if not new_dir_path.is_dir():
-                flag = True
-            else:
-                i = i + 1
-
-        print(f"New parameter set in: {new_name}, {new_dir_path} \n")
-
-        # new_dir_path.mkdir() # copy should be in the copy_params_dir
-        par.copy_params_dir(paramset.par_path, new_dir_path)
-        experiment.addParamset(new_name, new_dir_path)
-
-    def rename_set_params(editor, object):
-        """rename_set_params renames the node name on the tree and also
-        the folder of parameters"""
-        experiment = editor.get_parent(object)
-        paramset = object
-        # rename
-        # import pdb; pdb.set_trace()
-        editor._menu_rename_node()
-        new_name = object.name
-        new_dir_path = par.par_dir_prefix + new_name
-        os.mkdir(new_dir_path)
-        par.copy_params_dir(paramset.par_path, new_dir_path)
-        [
-            os.remove(os.path.join(paramset.par_path, f))
-            for f in os.listdir(paramset.par_path)
-        ]
-        os.rmdir(paramset.par_path)
-        experiment.removeParamset(paramset)
-        experiment.addParamset(new_name, new_dir_path)
-
-    def delete_set_params(editor, object):
-        """delete_set_params deletes the node and the folder of parameters"""
-        # experiment = editor.get_parent(object)
-        paramset = object
-        # delete node
-        editor._menu_delete_node()
-        # delete all the parameter files
-        [
-            os.remove(os.path.join(paramset.par_path, f))
-            for f in os.listdir(paramset.par_path)
-        ]
-        # remove folder
-        os.rmdir(paramset.par_path)
-
-    # ------------------------------------------
-    # Menubar actions
-    # ------------------------------------------
-    def new_action(self, info):
-        print("not implemented")
-
-    def open_action(self, info):
-        directory_dialog = DirectoryEditorDialog()
-        directory_dialog.edit_traits()
-        exp_path = directory_dialog.dir_name
-        print(f"Changing experimental path to {exp_path}")
-        os.chdir(exp_path)
-        info.object.exp1.populate_runs(exp_path)
-
-    def exit_action(self, info):
-        print("not implemented")
-
-    def saveas_action(self, info):
-        print("not implemented")
-
-    # def showimg_action(self, info):
-    #     info.object.update_plots(info.object.orig_image)
-
-    def highpass_action(self, info):
-        """highpass_action - calls ptv.py_pre_processing_c() binding which
-        does highpass on working images (object.orig_image) that were set
-        with init action
-        """
-        # I want to add here negative image if the parameter is set in the
-        # main parameters
-        if info.object.exp1.active_params.m_params.Inverse:
-            # print("Invert image")
-            for i, im in enumerate(info.object.orig_image):
-                info.object.orig_image[i] = 255 - im
-
-        if info.object.exp1.active_params.m_params.Subtr_Mask:
-            print("Subtracting mask")
-            try:
-                for i, im in enumerate(info.object.orig_image):
-                    mask_name = (
-                        info.object.exp1.active_params.m_params.Base_Name_Mask.replace(
-                            "#", str(i)
-                        )
-                    )
-                    mask = imread(mask_name)
-                    im[mask] = 0
-                    info.object.orig_image[i] = im
-            except ValueError as exc:
-                raise ValueError("Failed subtracting mask") from exc
-
-        print("highpass started")
-        info.object.orig_image = ptv.py_pre_processing_c(
-            info.object.orig_image, info.object.cpar
-        )
-        # info.object.update_plots(info.object.orig_image)
-        info.object.update_plots(info.object.orig_image)
-        print("highpass finished")
-
-    def img_coord_action(self, info):
-        """
-        img_coord_action - runs detection function by using
-        ptv.py_detection_proc_c()
-        binding. results are extracted with help of ptv.py_get_pix(x,y) binding
-        and plotted on the screen
-        """
-        print("Start detection")
-        (
-            info.object.detections,
-            info.object.corrected,
-        ) = ptv.py_detection_proc_c(
-            info.object.orig_image,
-            info.object.cpar,
-            info.object.tpar,
-            info.object.cals,
-        )
-        print("Detection finished")
-        x = [[i.pos()[0] for i in row] for row in info.object.detections]
-        y = [[i.pos()[1] for i in row] for row in info.object.detections]
-        info.object.drawcross_in_all_cams("x", "y", x, y, "blue", 3)
-
-    def _clean_correspondences(self, tmp):
-        """arr is a (n_cams,N,2) array that contains four lists of
-        correspondences (each per camera)
-        """
-        x1, y1 = [], []
-        for x in tmp:
-            tmp = x[(x != -999).any(axis=1)]  # remove all rows with -999
-            x1.append(tmp[:, 0])
-            y1.append(tmp[:, 1])
-
-        return x1, y1
-
-    def corresp_action(self, info):
-        """corresp_action calls ptv.py_correspondences_proc_c()
-        Result of correspondence action is filled to quadriplets, triplets,
-        pairs, and unused arrays
-        """
-
-        # if info.object.n_cams  > 1: # single camera is not checked
-        print("correspondence proc started")
-        (
-            info.object.sorted_pos,
-            info.object.sorted_corresp,
-            info.object.num_targs,
-        ) = ptv.py_correspondences_proc_c(info.object)
-
-        # we will always use from pairs or the last iter in sorted_pos
-        # and go upwards. so we'll stop at either triplets or quadruplets
-        names = ["pair", "tripl", "quad"]
-        use_colors = ["yellow", "green", "red"]
-
-        if len(info.object.camera_list) > 1 and len(info.object.sorted_pos) > 0:
-            # this is valid only if there are more than 1 camera
-            # quadruplets = info.object.sorted_pos[0]
-            # triplets = info.object.sorted_pos[1]
-            # pairs = info.object.sorted_pos[2]
-            # unused = []  # temporary solution
-
-            # if there are less than 4 cameras, then
-            # there are no quadruplets
-            # only triplets and pairs if 3
-            # only pairs if 2
-
-            # import pdb; pdb.set_trace()
-            # info.object.clear_plots(remove_background=False)
-            for i, subset in enumerate(reversed(info.object.sorted_pos)):
-                x, y = self._clean_correspondences(subset)
-                info.object.drawcross_in_all_cams(
-                    names[i] + "_x", names[i] + "_y", x, y, use_colors[i], 3
-                )
-
-        # x, y = self._clean_correspondences(triplets)
-        # info.object.drawcross("tripl_x", "tripl_y", x, y, "green", 3)
-        # x, y = self._clean_correspondences(pairs)
-        # info.object.drawcross("pair_x", "pair_y", x, y, "yellow", 3)
-        # info.object.drawcross("unused_x","unused_y",unused[:,0],unused[:,1],"blue",3)
-
-    def init_action(self, info):
-        """init_action - clears existing plots from the camera windows,
-        initializes C image arrays with mainGui.orig_image and
-        calls appropriate start_proc_c
-         by using ptv.py_start_proc_c()
-        """
-        mainGui = info.object
-        # synchronize the active run params dir with the temp params dir
-        mainGui.exp1.syncActiveDir()
-
-        for i in range(len(mainGui.camera_list)):
-            try:
-                im = imread(
-                    getattr(
-                        mainGui.exp1.active_params.m_params,
-                        f"Name_{i+1}_Image",
-                    )
-                )
-                if im.ndim > 2:
-                    im = rgb2gray(im)
-
-                mainGui.orig_image[i] = img_as_ubyte(im)
-            except IOError:
-                print("Error reading image, setting zero image")
-                h_img = mainGui.exp1.active_params.m_params.imx
-                v_img = mainGui.exp1.active_params.m_params.imy
-                temp_img = img_as_ubyte(np.zeros((h_img, v_img)))
-                # print(f"setting images of size {temp_img.shape}")
-                exec(f"mainGui.orig_image[{i}] = temp_img")
-
-            if hasattr(mainGui.camera_list[i], "img_plot"):
-                del mainGui.camera_list[i].img_plot
-        mainGui.clear_plots()
-        print("\n Init action \n")
-        # mainGui.update_plots(mainGui.orig_image, is_float=False)
-        mainGui.create_plots(mainGui.orig_image, is_float=False)
-        # mainGui.set_images(mainGui.orig_image)
-
-        (
-            info.object.cpar,
-            info.object.spar,
-            info.object.vpar,
-            info.object.track_par,
-            info.object.tpar,
-            info.object.cals,
-            info.object.epar,
-        ) = ptv.py_start_proc_c(info.object.n_cams)
-        mainGui.pass_init = True
-        print("Read all the parameters and calibrations successfully ")
-
-    def calib_action(self, info):
-        """calib_action - initializes calib class with appropriate number of
-        plot windows, passes to calib class pointer to ptv module and to
-        exp1 class, invokes the calibration GUI
-        """
-        print("\n Starting calibration dialog \n")
-
-        # reset the main GUI so the user will have to press Start again
-        info.object.pass_init = False
-        print("Active parameters set \n")
-        print(info.object.exp1.active_params.par_path)
-        calib_gui = CalibrationGUI(info.object.exp1.active_params.par_path)
-        calib_gui.configure_traits()
-
-    def detection_gui_action(self, info):
-        """activating detection GUI"""
-        print("\n Starting detection GUI dialog \n")
-
-        # reset the main GUI so the user will have to press Start again
-        info.object.pass_init = False
-        print("Active parameters set \n")
-        print(info.object.exp1.active_params.par_path)
-        detection_gui = DetectionGUI(info.object.exp1.active_params.par_path)
-        detection_gui.configure_traits()
-
-    def sequence_action(self, info):
-        """sequence action - implements binding to C sequence function.
-           Original function was split into 2 parts:
-        1) initialization - bonded by ptv.py_sequence_init(..) function
-        2) main loop processing - bonded by ptv.py_sequence_loop(..) function
-        """
-
-        extern_sequence = info.object.plugins.sequence_alg
-        if extern_sequence != "default":
-            try:
-                # change to pyptv folder, look for tracking module
-                sys.path.append(info.exp1.object.software_path)
-                # import chosen tracker from software dir
-
-                seq = importlib.import_module(extern_sequence)
-            except ImportError:
-                print(
-                    "Error loading or running "
-                    + extern_sequence
-                    + ". Falling back to default sequence algorithm"
-                )
-
-            print("Sequence by using " + extern_sequence)
-            sequence = seq.Sequence(
-                ptv=ptv,
-                exp1=info.object.exp1,
-                camera_list=info.object.camera_list,
-            )
-            sequence.do_sequence()
-            # print("Sequence by using "+extern_sequence+" has failed."
-
-        else:
-            ptv.py_sequence_loop(info.object)
-
-    def track_no_disp_action(self, info):
-        """track_no_disp_action uses ptv.py_trackcorr_loop(..) binding to
-        call tracking without display"""
-        extern_tracker = info.object.plugins.track_alg
-        if extern_tracker != "default":
-            try:
-                os.chdir(info.exp1.object.software_path)
-                track = importlib.import_module(extern_tracker)
-            except BaseException:
-                print(
-                    "Error loading "
-                    + extern_tracker
-                    + ". Falling back to default tracker"
-                )
-                extern_tracker = "default"
-            os.chdir(info.exp1.object.exp_path)  # change back to working path
-        if extern_tracker == "default":
-            print("Using default liboptv tracker")
-            info.object.tracker = ptv.py_trackcorr_init(info.object)
-            info.object.tracker.full_forward()
-        else:
-            print("Tracking by using " + extern_tracker)
-            tracker = track.Tracking(ptv=ptv, exp1=info.object.exp1)
-            tracker.do_tracking()
-
-        print("tracking without display finished")
-
-    def track_disp_action(self, info):
-        """tracking with display is handled by TrackThread which does
-        processing step by step and waits for GUI to update before
-        proceeding to the next step
-
-        This was not implemented in PyPTV
-        """
-        info.object.clear_plots(remove_background=False)
-        # info.object.tr_thread = TrackThread()
-        # info.object.tr_thread.start()
-
-    def track_back_action(self, info):
-        """tracking back action is handled by ptv.py_trackback_c() binding"""
-        print("Starting back tracking")
-        info.object.tracker.full_backward()
-
-    def three_d_positions(self, info):
-        """Extracts and saves 3D positions from the list of correspondences"""
-        ptv.py_determination_proc_c(
-            info.object.n_cams,
-            info.object.sorted_pos,
-            info.object.sorted_corresp,
-            info.object.corrected,
-        )
-
-    # def multigrid_demo(self, info):
-    #     demo_window = DemoGUI(ptv=ptv, exp1=info.object.exp1)
-    #     demo_window.configure_traits()
-
-    def detect_part_track(self, info):
-        """track detected particles is handled by 2 bindings:
-        1) tracking_framebuf.read_targets(..)
-        2) ptv.py_get_mark_track_c(..)
-        """
-        info.object.clear_plots(remove_background=False)  # clear everything
-        info.object.update_plots(info.object.orig_image, is_float=False)
-
-        prm = info.object.exp1.active_params.m_params
-        seq_first = prm.Seq_First  # get sequence parameters
-        seq_last = prm.Seq_Last
-        base_names = [
-            prm.Basename_1_Seq,
-            prm.Basename_2_Seq,
-            prm.Basename_3_Seq,
-            prm.Basename_4_Seq,
-        ]
-
-        # load first image from sequence
-        info.object.load_set_seq_image(seq_first)
-
-        print("Starting detect_part_track")
-        x1_a, x2_a, y1_a, y2_a = [], [], [], []
-        for i in range(info.object.n_cams):  # initialize result arrays
-            x1_a.append([])
-            x2_a.append([])
-            y1_a.append([])
-            y2_a.append([])
-
-    # imx, imy = info.object.cpar.get_image_size()
-
-        
-        for i_img in range(info.object.n_cams):
-            for i_seq in range(seq_first, seq_last + 1):  # loop over sequences
-                intx_green, inty_green = [], []
-                intx_blue, inty_blue = [], []
-                targets = optv.tracking_framebuf.read_targets(base_names[i_img], i_seq)
-
-                for t in targets:
-                    if t.tnr() > -1:
-                        intx_green.append(t.pos()[0])
-                        inty_green.append(t.pos()[1])
-                    else:
-                        intx_blue.append(t.pos()[0])
-                        inty_blue.append(t.pos()[1])
-
-                x1_a[i_img] = x1_a[i_img] + intx_green # add current step to result array
-                x2_a[i_img] = x2_a[i_img] + intx_blue
-                y1_a[i_img] = y1_a[i_img] + inty_green
-                y2_a[i_img] = y2_a[i_img] + inty_blue
-
-        # plot result arrays
-        for i_img in range(info.object.n_cams):
-            info.object.camera_list[i_img].drawcross(
-                "x_tr_gr", "y_tr_gr", x1_a[i_img], y1_a[i_img], "green", 3)
-            info.object.camera_list[i_img].drawcross(
-                "x_tr_bl","y_tr_bl", x2_a[i_img], y2_a[i_img], "blue",  2)
-            
-            info.object.camera_list[i_img]._plot.request_redraw()
-
-        print("Finished detect_part_track")
-
-    def traject_action_flowtracks(self, info):
-        """Shows trajectories reading and organizing by flowtracks
-
-        Args:
-            info (_type_): _description_
-        """
-        info.object.clear_plots(remove_background=False)
-        seq_first = info.object.exp1.active_params.m_params.Seq_First
-        seq_last = info.object.exp1.active_params.m_params.Seq_Last
-        info.object.load_set_seq_image(seq_first, display_only=True)
-
-        from flowtracks.io import trajectories_ptvis
-
-        dataset = trajectories_ptvis(
-            "res/ptv_is.%d", first=seq_first, last=seq_last, xuap=False, traj_min_len=3
-        )
-
-        heads_x, heads_y = [], []
-        tails_x, tails_y = [], []
-        ends_x, ends_y = [], []
-        for i_cam in range(info.object.n_cams):
-            head_x, head_y = [], []
-            tail_x, tail_y = [], []
-            end_x, end_y = [], []
-            for traj in dataset:
-                # projected = optv.imgcoord.image_coordinates(
-                #     np.atleast_2d(traj.pos()[0]*1000),
-                #     info.object.cals[i_cam],
-                #     info.object.cpar.get_multimedia_params(),
-                # )
-                # pos = optv.transforms.convert_arr_metric_to_pixel(
-                #     projected, info.object.cpar)
-
-                # head_x.append(pos[0][0])
-                # head_y.append(pos[0][1])
-
-                projected = optv.imgcoord.image_coordinates(
-                    np.atleast_2d(traj.pos() * 1000),
-                    info.object.cals[i_cam],
-                    info.object.cpar.get_multimedia_params(),
-                )
-                pos = optv.transforms.convert_arr_metric_to_pixel(
-                    projected, info.object.cpar
-                )
-
-                head_x.append(pos[0, 0])  # first row
-                head_y.append(pos[0, 1])
-                tail_x.extend(list(pos[1:-1, 0]))  # all other rows,
-                tail_y.extend(list(pos[1:-1, 1]))
-                end_x.append(pos[-1, 0])
-                end_y.append(pos[-1, 1])
-
-            heads_x.append(head_x)
-            heads_y.append(head_y)
-            tails_x.append(tail_x)
-            tails_y.append(tail_y)
-            ends_x.append(end_x)
-            ends_y.append(end_y)
-
-        for i_cam in range(info.object.n_cams):
-            info.object.camera_list[i_cam].drawcross(
-                "heads_x", "heads_y", heads_x[i_cam], heads_y[i_cam], "red", 3
-            )
-            info.object.camera_list[i_cam].drawcross(
-                "tails_x", "tails_y", tails_x[i_cam], tails_y[i_cam], "green", 2
-            )
-            info.object.camera_list[i_cam].drawcross(
-                "ends_x", "ends_y", ends_x[i_cam], ends_y[i_cam], "orange", 3
-            )
-
-
-    def plugin_action(self, info):
-        """Configure plugins by using GUI"""
-        info.object.plugins.read()
-        info.object.plugins.configure_traits()
-
-    def ptv_is_to_paraview(self, info):
-        """Button that runs the ptv_is.# conversion to Paraview"""
-
-        print("Saving trajectories for Paraview\n")
-        info.object.clear_plots(remove_background=False)
-        seq_first = info.object.exp1.active_params.m_params.Seq_First
-        seq_last = info.object.exp1.active_params.m_params.Seq_Last
-        info.object.load_set_seq_image(seq_first, display_only=True)
-
-        # borrowed from flowtracks that does much better job on this
-        # I think it's too much to import also postptv here, later
-        # we will make a single conda package for the full stack
-
-        # Example notebook translating OpenPTV files for Paraview using flowtracks
-        import pandas as pd
-        from flowtracks.io import trajectories_ptvis
-
-        dataset = trajectories_ptvis("res/ptv_is.%d", xuap=False)
-
-        dataframes = []
-        for traj in dataset:
-            dataframes.append(
-                pd.DataFrame.from_records(
-                    traj, columns=["x", "y", "z", "dx", "dy", "dz", "frame", "particle"]
-                )
-            )
-
-        df = pd.concat(dataframes, ignore_index=True)
-        df["particle"] = df["particle"].astype(np.int32)
-
-        # Paraview does not recognize it as a set without _000001.txt, so we the first 10000
-        # ptv_is.10001 is becoming ptv_00001.txt
-
-        df["frame"] = df["frame"].astype(np.int32)
-
-        df.reset_index(inplace=True, drop=True)
-        print(df.head())
-
-        df_grouped = df.reset_index().groupby("frame")
-        for index, group in df_grouped:
-            group.to_csv(
-                f"./res/ptv_{int(index):05d}.txt",
-                mode="w",
-                columns=["particle", "x", "y", "z", "dx", "dy", "dz"],
-                index=False,
-            )
-
-        print("Saving trajectories to Paraview finished\n")
-
-
-# ----------------------------------------------------------------
-# Actions associated with right mouse button clicks (treeeditor)
-# ---------------------------------------------------------------
-ConfigMainParams = Action(
-    name="Main parameters", action="handler.configure_main_par(editor,object)"
-)
-ConfigCalibParams = Action(
-    name="Calibration parameters",
-    action="handler.configure_cal_par(editor,object)",
-)
-ConfigTrackParams = Action(
-    name="Tracking parameters",
-    action="handler.configure_track_par(editor,object)",
-)
-SetAsDefault = Action(name="Set as active", action="handler.set_active(editor,object)")
-CopySetParams = Action(
-    name="Copy set of parameters",
-    action="handler.copy_set_params(editor,object)",
-)
-RenameSetParams = Action(
-    name="Rename run", action="handler.rename_set_params(editor,object)"
-)
-DeleteSetParams = Action(
-    name="Delete run", action="handler.delete_set_params(editor,object)"
-)
-
-# -----------------------------------------
-# Defines the menubar
-# ------------------------------------------
-menu_bar = MenuBar(
-    Menu(
-        Action(name="New", action="new_action"),
-        Action(name="Open", action="open_action"),
-        Action(name="Save As", action="saveas_action"),
-        Action(name="Exit", action="exit_action"),
-        name="File",
-    ),
-    Menu(Action(name="Init / Restart", action="init_action"), name="Start"),
-    Menu(
-        Action(
-            name="High pass filter",
-            action="highpass_action",
-            enabled_when="pass_init",
-        ),
-        Action(
-            name="Image coord",
-            action="img_coord_action",
-            enabled_when="pass_init",
-        ),
-        Action(
-            name="Correspondences",
-            action="corresp_action",
-            enabled_when="pass_init",
-        ),
-        name="Preprocess",
-    ),
-    Menu(
-        Action(
-            name="3D positions",
-            action="three_d_positions",
-            enabled_when="pass_init",
-        ),
-        name="3D Positions",
-    ),
-    Menu(
-        Action(
-            name="Create calibration",
-            action="calib_action",
-            enabled_when="pass_init",
-        ),
-        name="Calibration",
-    ),
-    Menu(
-        Action(
-            name="Sequence without display",
-            action="sequence_action",
-            enabled_when="pass_init",
-        ),
-        name="Sequence",
-    ),
-    Menu(
-        Action(
-            name="Detected Particles",
-            action="detect_part_track",
-            enabled_when="pass_init",
-        ),
-        Action(
-            name="Tracking without display",
-            action="track_no_disp_action",
-            enabled_when="pass_init",
-        ),
-        # not implemented Action(name='Tracking with
-        # display',action='track_disp_action',enabled_when='pass_init'),
-        Action(
-            name="Tracking backwards",
-            action="track_back_action",
-            enabled_when="pass_init",
-        ),
-        Action(
-            name="Show trajectories",
-            action="traject_action_flowtracks",
-            enabled_when="pass_init",
-        ),
-        Action(
-            name="Save Paraview files",
-            action="ptv_is_to_paraview",
-            enabled_when="pass_init",
-        ),
-        name="Tracking",
-    ),
-    Menu(Action(name="Select plugin", action="plugin_action"), name="Plugins"),
-    Menu(
-        Action(name="Detection GUI demo", action="detection_gui_action"),
-        name="Detection demo",
-    ),
-)
-
-# ----------------------------------------
-# tree editor for the Experiment() class
-#
-tree_editor_exp = TreeEditor(
-    nodes=[
-        TreeNode(
-            node_for=[Experiment],
-            auto_open=True,
-            children="",
-            label="=Experiment",
-        ),
-        TreeNode(
-            node_for=[Experiment],
-            auto_open=True,
-            children="paramsets",
-            label="=Parameters",
-            add=[Paramset],
-            menu=Menu(CopySetParams),
-        ),
-        TreeNode(
-            node_for=[Paramset],
-            auto_open=True,
-            children="",
-            label="name",
-            menu=Menu(
-                # NewAction,
-                CopySetParams,
-                RenameSetParams,
-                DeleteSetParams,
-                Separator(),
-                ConfigMainParams,
-                ConfigCalibParams,
-                ConfigTrackParams,
-                Separator(),
-                SetAsDefault,
-            ),
-        ),
-    ],
-    editable=False,
-)
-
-
-# -------------------------------------------------------------------------
-class Plugins(HasTraits):
-    track_list = List
-    seq_list = List
-    track_alg = Enum(values="track_list")
-    sequence_alg = Enum(values="seq_list")
-    view = View(
-        Group(
-            Item(name="track_alg", label="Choose tracking algorithm:"),
-            Item(name="sequence_alg", label="Choose sequence algorithm:"),
-        ),
-        buttons=["OK"],
-        title="External plugins configuration",
-    )
-
-    def __init__(self):
-        self.read()
-
-    def read(self):
-        # reading external tracking
-        if os.path.exists(
-            os.path.join(os.path.abspath(os.curdir), "external_tracker_list.txt")
-        ):
-            with open(
-                os.path.join(os.path.abspath(os.curdir), "external_tracker_list.txt"),
-                "r",
-            ) as f:
-                trackers = f.read().split("\n")
-                trackers.insert(0, "default")
-                self.track_list = trackers
-        else:
-            self.track_list = ["default"]
-        # reading external sequence
-        if os.path.exists(
-            os.path.join(os.path.abspath(os.curdir), "external_sequence_list.txt")
-        ):
-            with open(
-                os.path.join(os.path.abspath(os.curdir), "external_sequence_list.txt"),
-                "r",
-            ) as f:
-                seq = f.read().split("\n")
-                seq.insert(0, "default")
-                self.seq_list = seq
-        else:
-            self.seq_list = ["default"]
-
-
-# ----------------------------------------------
-class MainGUI(HasTraits):
-    """MainGUI is the main class under which the Model-View-Control
-    (MVC) model is defined"""
-
-    camera_list = List
-    # imgplt_flag = 0
-    pass_init = Bool(False)
-    update_thread_plot = Bool(False)
-    # tr_thread = Instance(TrackThread)
-    selected = Any
-
-    # Defines GUI view --------------------------
-    view = View(
-        Group(
-            Group(
-                Item(
-                    name="exp1",
-                    editor=tree_editor_exp,
-                    show_label=False,
-                    width=-400,
-                    resizable=False,
-                ),
-                Item(
-                    "camera_list",
-                    style="custom",
-                    editor=ListEditor(
-                        use_notebook=True,
-                        deletable=False,
-                        dock_style="tab",
-                        page_name=".name",
-                        selected="selected",
-                    ),
-                    show_label=False,
-                ),
-                orientation="horizontal",
-                show_left=False,
-            ),
-            orientation="vertical",
-        ),
-        title="pyPTV ver. 0.2.2",
-        id="main_view",
-        width=1.0,
-        height=1.0,
-        resizable=True,
-        handler=TreeMenuHandler(),  # <== Handler class is attached
-        menubar=menu_bar,
-    )
-
-    def _selected_changed(self):
-        self.current_camera = int(self.selected.name.split(" ")[1]) - 1
-
-    # ---------------------------------------------------
-    # Constructor and Chaco windows initialization
-    # ---------------------------------------------------
-    def __init__(self, exp_path: Path, software_path: Path):
-        super(MainGUI, self).__init__()
-        colors = ["yellow", "green", "red", "blue"]
-        self.exp1 = Experiment()
-        self.exp1.populate_runs(exp_path)
-        self.plugins = Plugins()
-        self.n_cams = self.exp1.active_params.m_params.Num_Cam
-        self.orig_image = self.n_cams * [[]]
-        self.current_camera = 0
-        self.camera_list = [
-            CameraWindow(colors[i], f"Camera {i+1}") for i in range(self.n_cams)
-        ]
-        self.software_path = software_path
-        self.exp_path = exp_path
-        for i in range(self.n_cams):
-            self.camera_list[i].on_trait_change(self.right_click_process, "rclicked")
-
-    def right_click_process(self):
-        """
-        Shows a line in camera color code corresponding to a point on another
-        camera's view plane.
-        """        
-        num_points = 2
-        
-        try:
-            _ = self.sorted_pos
-            plot_epipolar = True
-        except:
-            plot_epipolar = False
-            
-        
-        if plot_epipolar:
-
-            i = self.current_camera
-            point = np.array(
-                [
-                    self.camera_list[i]._click_tool.x,
-                    self.camera_list[i]._click_tool.y,
-                ],
-                dtype="float64",
-            )
-            
-            # find closest point
-            for pos_type in self.sorted_pos: # quadruplet, triplet, pair
-                distances = np.linalg.norm(pos_type[i] - point, axis=1)
-                if np.min(distances) < 5 :
-                    point = pos_type[i][np.argmin(distances)]
-                    
-            
-            if not np.allclose(point, [0.0, 0.0]):
-                # mark the point with a circle
-                c = str(np.random.rand())[2:]
-                self.camera_list[i].drawcross(
-                    "right_p_x0" + c,
-                    "right_p_y0" + c,
-                    point[0],
-                    point[1],
-                    "cyan",
-                    3,
-                    marker="circle",
-                )
-
-                # look for points along epipolars for other cameras
-                for j in range(self.n_cams):
-                    if i == j:
-                        continue
-                    pts = optv.epipolar.epipolar_curve(
-                        point,
-                        self.cals[i],
-                        self.cals[j],
-                        num_points,
-                        self.cpar,
-                        self.vpar,
-                    )
-
-                    if len(pts) > 1:
-                        self.camera_list[j].drawline(
-                            "right_cl_x" + c,
-                            "right_cl_y" + c,
-                            pts[0, 0],
-                            pts[0, 1],
-                            pts[-1, 0],
-                            pts[-1, 1],
-                            self.camera_list[i].cam_color,
-                        )
-                
-                self.camera_list[i].rclicked = 0
-                        
-        
-
-    def create_plots(self, images, is_float=False) -> None:
-        """update_plots
-
-        Args:
-            images (_type_): images to update
-            is_float (bool, optional): _description_. Defaults to False.
-        """
-        print("inside update plots, images changed\n")
-        for i in range(self.n_cams):
-            self.camera_list[i].create_image(images[i], is_float)
-            self.camera_list[i]._plot.request_redraw()
-            
-    def update_plots(self, images, is_float=False) -> None:
-        """update_plots
-
-        Args:
-            images (_type_): images to update
-            is_float (bool, optional): _description_. Defaults to False.
-        """
-        print("inside update plots, images changed\n")
-        for i in range(self.n_cams):
-            self.camera_list[i].update_image(images[i], is_float)
-            self.camera_list[i]._plot.request_redraw()
-
-    def drawcross_in_all_cams(self, str_x, str_y, x, y, color1, size1, marker="plus"):
-        """
-        Draws crosses
-        """
-        for i, cam in enumerate(self.camera_list):
-            cam.drawcross(str_x, str_y, x[i], y[i], color1, size1, marker=marker)
-
-    def clear_plots(self, remove_background=True):
-        # this function deletes all plots except basic image plot
-
-        if not remove_background:
-            index = "plot0"
-        else:
-            index = None
-
-        for i in range(self.n_cams):
-            plot_list = list(self.camera_list[i]._plot.plots.keys())
-            # if not remove_background:
-            #   index=None
-            if index in plot_list:
-                # try:
-                plot_list.remove(index)
-            # except:
-            # pass
-            self.camera_list[i]._plot.delplot(*plot_list[0:])
-            self.camera_list[i]._plot.tools = []
-            self.camera_list[i]._plot.request_redraw()
-            for j in range(len(self.camera_list[i]._quiverplots)):
-                self.camera_list[i]._plot.remove(self.camera_list[i]._quiverplots[j])
-            self.camera_list[i]._quiverplots = []
-            self.camera_list[i].right_p_x0 = []
-            self.camera_list[i].right_p_y0 = []
-            self.camera_list[i].right_p_x1 = []
-            self.camera_list[i].right_p_y1 = []
-
-    def _update_thread_plot_changed(self):
-        n_cams = len(self.camera_list)
-
-        if self.update_thread_plot and self.tr_thread:
-            print("updating plots..\n")
-            step = self.tr_thread.track_step
-
-            x0, x1, x2, y0, y1, y2 = (
-                self.tr_thread.intx0,
-                self.tr_thread.intx1,
-                self.tr_thread.intx2,
-                self.tr_thread.inty0,
-                self.tr_thread.inty1,
-                self.tr_thread.inty2,
-            )
-            for i in range(n_cams):
-                self.camera_list[i].drawcross(
-                    str(step) + "x0",
-                    str(step) + "y0",
-                    x0[i],
-                    y0[i],
-                    "green",
-                    2,
-                )
-                self.camera_list[i].drawcross(
-                    str(step) + "x1",
-                    str(step) + "y1",
-                    x1[i],
-                    y1[i],
-                    "yellow",
-                    2,
-                )
-                self.camera_list[i].drawcross(
-                    str(step) + "x2",
-                    str(step) + "y2",
-                    x2[i],
-                    y2[i],
-                    "white",
-                    2,
-                )
-                self.camera_list[i].drawquiver(x0[i], y0[i], x1[i], y1[i], "orange")
-                self.camera_list[i].drawquiver(x1[i], y1[i], x2[i], y2[i], "white")
-            # for j in range (m_tr):
-            # str_plt=str(step)+"_"+str(j)
-            ##
-            # self.camera_list[i].drawline\
-            # (str_plt+"vec_x0",str_plt+"vec_y0",x0[i][j],y0[i][j],x1[i][j],y1[i][j],"orange")
-            # self.camera_list[i].drawline\
-            # (str_plt+"vec_x1",str_plt+"vec_y1",x1[i][j],y1[i][j],x2[i][j],y2[i][j],"white")
-            self.load_set_seq_image(step, update_all=False, display_only=True)
-            self.camera_list[self.current_camera]._plot.request_redraw()
-            time.sleep(0.1)
-            self.tr_thread.can_continue = True
-            self.update_thread_plot = False
-
-    def load_set_seq_image(self, seq: int, update_all=True, display_only=False):
-        """load and set sequence image
-
-        Args:
-            seq (_type_): sequance properties
-            update_all (bool, optional): _description_. Defaults to True.
-            display_only (bool, optional): _description_. Defaults to False.
-        """
-        n_cams = len(self.camera_list)
-        if not hasattr(self, "base_name"):
-            self.base_name = []
-            for i in range(n_cams):
-                exec(
-                    "self.base_name.append"
-                    + f"(self.exp1.active_params.m_params.Basename_{i+1}_Seq)"
-                )
-                # print(f" base name in GUI is {self.base_name[i]}")
-
-        # i = seq
-        seq_ch = f"{seq:04d}"
-
-        if not update_all:
-            j = self.current_camera
-            # img_name = self.base_name[j] + seq_ch
-            img_name = self.base_name[j].replace("#", seq_ch)
-            # print(f"Image name in load_set_seq is {img_name}")
-            self.load_disp_image(img_name, j, display_only)
-        else:
-            for j in range(n_cams):
-                # img_name = self.base_name[j] + seq_ch
-                img_name = self.base_name[j].replace("#", seq_ch)
-                # print(f"Image name in load_set_seq is {img_name}")
-                self.load_disp_image(img_name, j, display_only)
-
-    def load_disp_image(self, img_name: str, j: int, display_only: bool = False):
-        """load and display image
-
-        Args:
-            img_name (_type_): filename of the image
-            j (_type_): integer counter
-            display_only (bool, optional): display only. Defaults to False.
-        """
-        # print(f"Setting image: {img_name}")
-        try:
-            temp_img = img_as_ubyte(imread(img_name))
-        except IOError:
-            print("Error reading file, setting zero image")
-            h_img = self.exp1.active_params.m_params.imx
-            v_img = self.exp1.active_params.m_params.imy
-            temp_img = img_as_ubyte(np.zeros((h_img, v_img)))
-        # if not display_only:
-        #     ptv.py_set_img(temp_img, j)
-        if len(temp_img) > 0:
-            self.camera_list[j].update_image(temp_img)
-
-
-def printException():
-    import traceback
-
-    print("=" * 50)
-    print("Exception:", sys.exc_info()[1])
-    print(f"{Path.cwd()}")
-    print("Traceback:")
-    traceback.print_tb(sys.exc_info()[2])
-    print("=" * 50)
-
-
-# -------------------------------------------------------------
-def main():
-    """main ()
-
-    Raises:
-        OSError: if software or folder path are missing
-    """
-    # Parse inputs:
-    software_path = Path.cwd().resolve()
-    print(f"Software path is {software_path}")
-
-    # Path to the experiment
-    if len(sys.argv) > 1:
-        exp_path = Path(sys.argv[1]).resolve()
-        print(f"Experimental path is {exp_path}")
-    else:
-        exp_path = software_path.parent / "test_cavity"
-        print(f"Without input, PyPTV fallbacks to a default {exp_path} \n")
-
-    if not exp_path.is_dir() or not exp_path.exists():
-        raise OSError(f"Wrong experimental directory {exp_path}")
-
-    # Change directory to the path
-    os.chdir(exp_path)
-
-    try:
-        main_gui = MainGUI(exp_path, software_path)
-        main_gui.configure_traits()
-    except OSError:
-        print("something wrong with the software or folder")
-        printException()
-
-    os.chdir(software_path)  # get back to the original workdir
-
-
-if __name__ == "__main__":
-    main()
+""" PyPTV_GUI is the GUI for the OpenPTV (www.openptv.net) written in
+Python with Traits, TraitsUI, Numpy, Scipy and Chaco
+
+Copyright (c) 2008-2023, Turbulence Structure Laboratory, Tel Aviv University
+The GUI software is distributed under the terms of MIT-like license
+http://opensource.org/licenses/MIT
+
+OpenPTV library is distributed under the terms of LGPL license
+see http://www.openptv.net for more details.
+
+"""
+
+from traits.etsconfig.api import ETSConfig
+ETSConfig.toolkit = 'qt4'
+
+import os
+from pathlib import Path, PurePath
+import sys
+import time
+import importlib
+
+import numpy as np
+import optv
+from traits.api import HasTraits, Int, Bool, Instance, List, Enum, Any
+from traitsui.api import (
+    View,
+    Item,
+    ListEditor,
+    Handler,
+    TreeEditor,
+    TreeNode,
+    Separator,
+    Group,
+)
+
+
+
+
+from traitsui.menu import Action, Menu, MenuBar
+from chaco.api import ArrayDataSource, ArrayPlotData, LinearMapper, Plot, gray
+from chaco.tools.api import PanTool, ZoomTool
+from chaco.tools.image_inspector_tool import ImageInspectorTool
+from enable.component_editor import ComponentEditor
+from skimage.util import img_as_ubyte
+from skimage.color import rgb2gray
+from skimage.io import imread
+
+from pyptv import parameters as par
+from pyptv import ptv
+from pyptv.calibration_gui import CalibrationGUI
+from pyptv.directory_editor import DirectoryEditorDialog
+from pyptv.parameter_gui import Experiment, Paramset
+from pyptv.quiverplot import QuiverPlot
+from pyptv.detection_gui import DetectionGUI
+import optv.orientation
+
+
+class Clicker(ImageInspectorTool):
+    """
+    Clicker class handles right mouse click actions from the tree
+    and menubar actions
+    """
+    left_changed = Int(0)
+    right_changed = Int(0)
+    x,y = 0,0
+
+    def __init__(self, *args, **kwargs):
+        # Clicker.__init__(self,*args, **kwargs)
+        super(Clicker, self).__init__(*args, **kwargs)
+
+    def normal_left_down(self, event):
+        """Handles the left mouse button being clicked.
+        Fires the **new_value** event with the data (if any) from the event's
+        position.
+        """
+        plot = self.component
+        if plot is not None:
+            self.x, self.y = plot.map_index((event.x, event.y))
+            self.data_value = plot.value.data[self.y, self.x]
+            self.last_mouse_position = (event.x, event.y)
+            self.left_changed = 1 - self.left_changed
+            # print(f"left: x={self.x}, y={self.y}, I={self.data_value}, {self.left_changed}")
+            
+
+    def normal_right_down(self, event):
+        plot = self.component
+        if plot is not None:
+            self.x, self.y = plot.map_index((event.x, event.y))
+            self.last_mouse_position = (event.x, event.y)
+            self.data_value = plot.value.data[self.y, self.x]
+            # print(f"right: x={self.x}, y={self.y}, I={self.data_value}")
+            self.right_changed = 1 - self.right_changed
+            
+        
+
+    # def normal_mouse_move(self, event):
+    #     pass
+
+
+
+# --------------------------------------------------------------
+class CameraWindow(HasTraits):
+    """CameraWindow class contains the relevant information and functions for
+    a single camera window: image, zoom, pan important members:
+    _plot_data  - contains image data to display (used by update_image)
+    _plot - instance of Plot class to use with _plot_data
+    _click_tool - instance of Clicker tool for the single camera window,
+    to handle mouse processing
+    """
+
+    _plot = Instance(Plot)
+    _click_tool = Instance(Clicker)
+    rclicked = Int(0)
+
+    cam_color = ""
+    name = ""
+    view = View(Item(name="_plot", editor=ComponentEditor(), show_label=False))
+
+    def __init__(self, color, name):
+        """
+        Initialization of plot system
+        """
+        super(HasTraits, self).__init__()
+        padd = 25
+        self._plot_data = ArrayPlotData() # we need set_data
+        self._plot = Plot(self._plot_data, default_origin="top left")
+        self._plot.padding_left = padd
+        self._plot.padding_right = padd
+        self._plot.padding_top = padd
+        self._plot.padding_bottom = padd
+        (
+            self.right_p_x0,
+            self.right_p_y0,
+            self.right_p_x1,
+            self.right_p_y1,
+            self._quiverplots,
+        ) = ([], [], [], [], [])
+        self.cam_color = color
+        self.name = name
+        
+
+    def attach_tools(self):
+        """attach_tools(self) contains the relevant tools:
+        clicker, pan, zoom"""
+      
+        print(f" Attaching clicker to camera {self.name}")
+        self._click_tool = Clicker(component=self._img_plot)
+        self._click_tool.on_trait_change(self.left_clicked_event, "left_changed")
+        self._click_tool.on_trait_change(self.right_clicked_event, "right_changed")
+        # self._img_plot.tools.clear()
+        self._img_plot.tools.append(self._click_tool)
+        
+        pan = PanTool(self._plot, drag_button="middle")
+        zoom_tool = ZoomTool(self._plot, tool_mode="box", always_on=False)
+        zoom_tool.max_zoom_out_factor = 1.0  # Disable "bird view" zoom out
+        self._img_plot.overlays.append(zoom_tool)
+        self._img_plot.tools.append(pan)
+        # print(self._img_plot.tools)
+        
+
+    def left_clicked_event(
+        self,
+    ):  # TODO: why do we need the ClickerTool if we can handle mouse
+        # clicks here?
+        """left_clicked_event - processes left click mouse
+        events and displays coordinate and grey value information
+        on the screen
+        """
+        print(
+            f"x={self._click_tool.x} pix,y={self._click_tool.y} pix,I={self._click_tool.data_value}"
+        )
+        
+    def right_clicked_event(self):
+        """right mouse button click event flag"""
+        # # self._click_tool.right_changed = 1
+        # print(
+        #     f"right_clicked, x={self._click_tool.x} pix,y={self._click_tool.y} pix, I={self._click_tool.data_value}, {self.rclicked}"
+        # )
+        self.rclicked = 1
+
+        
+    def create_image(self, image, is_float=False):
+        """create_image - displays/updates image in the current camera window
+        parameters:
+            image - image data
+            is_float - if true, displays an image as float array,
+            else displays as byte array (B&W or gray)
+        example usage:
+            create_image(image,is_float=False)
+        """
+        # print('image shape = ', image.shape, 'is_float =', is_float)
+        # if image.ndim > 2:
+        #     image = img_as_ubyte(rgb2gray(image))
+        #     is_float = False
+
+        if is_float:
+            self._plot_data.set_data("imagedata", image.astype(np.float32))
+        else:
+            self._plot_data.set_data("imagedata", image.astype(np.uint8))
+
+        # if not hasattr(
+        #         self,
+        #         "img_plot"):  # make a new plot if there is nothing to update
+        #     self.img_plot = Instance(ImagePlot)
+
+        self._img_plot = self._plot.img_plot("imagedata", colormap=gray)[0]
+        self.attach_tools()
+
+    def update_image(self, image, is_float=False):
+        """update_image - displays/updates image in the current camera window
+        parameters:
+            image - image data
+            is_float - if true, displays an image as float array,
+            else displays as byte array (B&W or gray)
+        example usage:
+            update_image(image,is_float=False)
+        """
+
+        if is_float:
+            self._plot_data.set_data("imagedata", image.astype(np.float32))
+        else:
+            self._plot_data.set_data("imagedata", image.astype(np.uint8))
+
+        self._plot.img_plot("imagedata", colormap=gray)[0]
+        self._plot.request_redraw()
+
+    def drawcross(self, str_x, str_y, x, y, color, mrk_size, marker="plus"):
+        """drawcross draws crosses at a given location (x,y) using color
+        and marker in the current camera window parameters:
+            str_x - label for x coordinates
+            str_y - label for y coordinates
+            x - array of x coordinates
+            y - array of y coordinates
+            mrk_size - marker size
+            marker - type of marker, e.g "plus","circle"
+        example usage:
+            drawcross("coord_x","coord_y",[100,200,300],[100,200,300],2)
+            draws plus markers of size 2 at points
+                (100,100),(200,200),(200,300)
+            :rtype:
+        """
+        self._plot_data.set_data(str_x, np.atleast_1d(x))
+        self._plot_data.set_data(str_y, np.atleast_1d(y))
+        self._plot.plot(
+            (str_x, str_y),
+            type="scatter",
+            color=color,
+            marker=marker,
+            marker_size=mrk_size,
+        )
+        self._plot.request_redraw()
+
+    def drawquiver(self, x1c, y1c, x2c, y2c, color, linewidth=1.0):
+        """Draws multiple lines at once on the screen x1,y1->x2,y2 in the
+        current camera window
+        parameters:
+            x1c - array of x1 coordinates
+            y1c - array of y1 coordinates
+            x2c - array of x2 coordinates
+            y2c - array of y2 coordinates
+            color - color of the line
+            linewidth - linewidth of the line
+        example usage:
+            drawquiver ([100,200],[100,100],[400,400],[300,200],\
+                'red',linewidth=2.0)
+            draws 2 red lines with thickness = 2 :  \
+                100,100->400,300 and 200,100->400,200
+
+        """
+        x1, y1, x2, y2 = self.remove_short_lines(x1c, y1c, x2c, y2c)
+        if len(x1) > 0:
+            xs = ArrayDataSource(x1)
+            ys = ArrayDataSource(y1)
+
+            quiverplot = QuiverPlot(
+                index=xs,
+                value=ys,
+                index_mapper=LinearMapper(range=self._plot.index_mapper.range),
+                value_mapper=LinearMapper(range=self._plot.value_mapper.range),
+                origin=self._plot.origin,
+                arrow_size=0,
+                line_color=color,
+                line_width=linewidth,
+                ep_index=np.array(x2),
+                ep_value=np.array(y2),
+            )
+            # Seems to be incorrect use of .add
+            # self._plot.add(quiverplot)
+            self._plot.overlays.append(quiverplot)
+
+            # we need this to track how many quiverplots are in the current
+            # plot
+            self._quiverplots.append(quiverplot)
+
+    @staticmethod
+    def remove_short_lines(x1, y1, x2, y2):
+        """removes short lines from the array of lines
+        parameters:
+            x1,y1,x2,y2 - start and end coordinates of the lines
+        returns:
+            x1f,y1f,x2f,y2f - start and end coordinates of the lines,
+            with short lines removed example usage:
+            x1,y1,x2,y2 = remove_short_lines( \
+                [100,200,300],[100,200,300],[100,200,300],[102,210,320])
+            3 input lines, 1 short line will be removed (100,100->100,102)
+            returned coordinates:
+            x1=[200,300]; y1=[200,300]; x2=[200,300]; y2=[210,320]
+        """
+        dx, dy = 2, 2  # minimum allowable dx,dy
+        x1f, y1f, x2f, y2f = [], [], [], []
+        for i in range(len(x1)):
+            if abs(x1[i] - x2[i]) > dx or abs(y1[i] - y2[i]) > dy:
+                x1f.append(x1[i])
+                y1f.append(y1[i])
+                x2f.append(x2[i])
+                y2f.append(y2[i])
+        return x1f, y1f, x2f, y2f
+
+    def drawline(self, str_x, str_y, x1, y1, x2, y2, color1):
+        """drawline draws 1 line on the screen by using lineplot x1,y1->x2,y2
+        parameters:
+            str_x - label of x coordinate
+            str_y - label of y coordinate
+            x1,y1,x2,y2 - start and end coordinates of the line
+            color1 - color of the line
+        example usage:
+            drawline("x_coord","y_coord",100,100,200,200,red)
+            draws a red line 100,100->200,200
+        """
+        # imx, imy = self._plot_data.get_data('imagedata').shape
+        self._plot_data.set_data(str_x, [x1, x2])
+        self._plot_data.set_data(str_y, [y1, y2])
+        self._plot.plot((str_x, str_y), type="line", color=color1)
+
+
+class TreeMenuHandler(Handler):
+    """TreeMenuHanlder contains all the callback actions of menu bar,
+    processing of tree editor, and reactions of the GUI to the user clicks
+    possible function declarations:
+        1) to process menubar actions:
+            def function(self, info):
+        parameters: self - needed for member function declaration,
+                info - contains pointer to calling parent class (e.g main_gui)
+                To access parent class objects use info.object, for example
+                info.object.exp1 gives access to exp1 member of main_gui class
+        2) to process tree editor actions:
+            def function(self,editor,object) - see examples below
+
+    """
+
+    def configure_main_par(self, editor, object):
+        experiment = editor.get_parent(object)
+        paramset = object
+        print("Total paramsets:", len(experiment.paramsets))
+        if paramset.m_params is None:
+            # TODO: is it possible that control reaches here? If not, probably
+            # the if should be removed.
+            paramset.m_params = par.PtvParams()
+        else:
+            paramset.m_params._reload()
+        paramset.m_params.edit_traits(kind="modal")
+
+    def configure_cal_par(self, editor, object):
+        experiment = editor.get_parent(object)
+        paramset = object
+        print(len(experiment.paramsets))
+        if paramset.c_params is None:
+            # TODO: is it possible that control reaches here? If not, probably
+            # the if should be removed.
+            paramset.c_params = par.CalOriParams()  # this is a very questionable line
+        else:
+            paramset.c_params._reload()
+        paramset.c_params.edit_traits(kind="modal")
+
+    def configure_track_par(self, editor, object):
+        experiment = editor.get_parent(object)
+        paramset = object
+        print(len(experiment.paramsets))
+        if paramset.t_params is None:
+            # TODO: is it possible that control reaches here? If not, probably
+            # the if should be removed.
+            paramset.t_params = par.TrackingParams()
+        paramset.t_params.edit_traits(kind="modal")
+
+    def set_active(self, editor, object):
+        """sets a set of parameters as active"""
+        experiment = editor.get_parent(object)
+        paramset = object
+        # experiment.active_params = paramset
+        experiment.setActive(paramset)
+        experiment.changed_active_params = True
+        # editor.object.__init__()
+
+    def copy_set_params(self, editor, object):
+        experiment = editor.get_parent(object)
+        paramset = object
+        print(f" Copying set of parameters \n")
+        print(f"paramset is {paramset.name}")
+        print(f"paramset id is {int(paramset.name.split('Run')[-1])}")
+        # print(f"experiment is {experiment}\n")
+
+        i = 1
+        new_name = None
+        new_dir_path = None
+        flag = False
+        while not flag:
+            new_name = f"{paramset.name}_{i}"
+            new_dir_path = Path(f"{par.par_dir_prefix}{new_name}")
+            if not new_dir_path.is_dir():
+                flag = True
+            else:
+                i = i + 1
+
+        print(f"New parameter set in: {new_name}, {new_dir_path} \n")
+
+        # new_dir_path.mkdir() # copy should be in the copy_params_dir
+        par.copy_params_dir(paramset.par_path, new_dir_path)
+        experiment.addParamset(new_name, new_dir_path)
+
+    def rename_set_params(editor, object):
+        """rename_set_params renames the node name on the tree and also
+        the folder of parameters"""
+        experiment = editor.get_parent(object)
+        paramset = object
+        # rename
+        # import pdb; pdb.set_trace()
+        editor._menu_rename_node()
+        new_name = object.name
+        new_dir_path = par.par_dir_prefix + new_name
+        os.mkdir(new_dir_path)
+        par.copy_params_dir(paramset.par_path, new_dir_path)
+        [
+            os.remove(os.path.join(paramset.par_path, f))
+            for f in os.listdir(paramset.par_path)
+        ]
+        os.rmdir(paramset.par_path)
+        experiment.removeParamset(paramset)
+        experiment.addParamset(new_name, new_dir_path)
+
+    def delete_set_params(editor, object):
+        """delete_set_params deletes the node and the folder of parameters"""
+        # experiment = editor.get_parent(object)
+        paramset = object
+        # delete node
+        editor._menu_delete_node()
+        # delete all the parameter files
+        [
+            os.remove(os.path.join(paramset.par_path, f))
+            for f in os.listdir(paramset.par_path)
+        ]
+        # remove folder
+        os.rmdir(paramset.par_path)
+
+    # ------------------------------------------
+    # Menubar actions
+    # ------------------------------------------
+    def new_action(self, info):
+        print("not implemented")
+
+    def open_action(self, info):
+        directory_dialog = DirectoryEditorDialog()
+        directory_dialog.edit_traits()
+        exp_path = directory_dialog.dir_name
+        print(f"Changing experimental path to {exp_path}")
+        os.chdir(exp_path)
+        info.object.exp1.populate_runs(exp_path)
+
+    def exit_action(self, info):
+        print("not implemented")
+
+    def saveas_action(self, info):
+        print("not implemented")
+
+    # def showimg_action(self, info):
+    #     info.object.update_plots(info.object.orig_image)
+
+    def highpass_action(self, info):
+        """highpass_action - calls ptv.py_pre_processing_c() binding which
+        does highpass on working images (object.orig_image) that were set
+        with init action
+        """
+        # I want to add here negative image if the parameter is set in the
+        # main parameters
+        if info.object.exp1.active_params.m_params.Inverse:
+            # print("Invert image")
+            for i, im in enumerate(info.object.orig_image):
+                info.object.orig_image[i] = 255 - im
+
+        if info.object.exp1.active_params.m_params.Subtr_Mask:
+            print("Subtracting mask")
+            try:
+                for i, im in enumerate(info.object.orig_image):
+                    mask_name = (
+                        info.object.exp1.active_params.m_params.Base_Name_Mask.replace(
+                            "#", str(i)
+                        )
+                    )
+                    mask = imread(mask_name)
+                    im[mask] = 0
+                    info.object.orig_image[i] = im
+            except ValueError as exc:
+                raise ValueError("Failed subtracting mask") from exc
+
+        print("highpass started")
+        info.object.orig_image = ptv.py_pre_processing_c(
+            info.object.orig_image, info.object.cpar
+        )
+        # info.object.update_plots(info.object.orig_image)
+        info.object.update_plots(info.object.orig_image)
+        print("highpass finished")
+
+    def img_coord_action(self, info):
+        """
+        img_coord_action - runs detection function by using
+        ptv.py_detection_proc_c()
+        binding. results are extracted with help of ptv.py_get_pix(x,y) binding
+        and plotted on the screen
+        """
+        print("Start detection")
+        (
+            info.object.detections,
+            info.object.corrected,
+        ) = ptv.py_detection_proc_c(
+            info.object.orig_image,
+            info.object.cpar,
+            info.object.tpar,
+            info.object.cals,
+        )
+        print("Detection finished")
+        x = [[i.pos()[0] for i in row] for row in info.object.detections]
+        y = [[i.pos()[1] for i in row] for row in info.object.detections]
+        info.object.drawcross_in_all_cams("x", "y", x, y, "blue", 3)
+
+    def _clean_correspondences(self, tmp):
+        """arr is a (n_cams,N,2) array that contains four lists of
+        correspondences (each per camera)
+        """
+        x1, y1 = [], []
+        for x in tmp:
+            tmp = x[(x != -999).any(axis=1)]  # remove all rows with -999
+            x1.append(tmp[:, 0])
+            y1.append(tmp[:, 1])
+
+        return x1, y1
+
+    def corresp_action(self, info):
+        """corresp_action calls ptv.py_correspondences_proc_c()
+        Result of correspondence action is filled to quadriplets, triplets,
+        pairs, and unused arrays
+        """
+
+        # if info.object.n_cams  > 1: # single camera is not checked
+        print("correspondence proc started")
+        (
+            info.object.sorted_pos,
+            info.object.sorted_corresp,
+            info.object.num_targs,
+        ) = ptv.py_correspondences_proc_c(info.object)
+
+        # we will always use from pairs or the last iter in sorted_pos
+        # and go upwards. so we'll stop at either triplets or quadruplets
+        names = ["pair", "tripl", "quad"]
+        use_colors = ["yellow", "green", "red"]
+
+        if len(info.object.camera_list) > 1 and len(info.object.sorted_pos) > 0:
+            # this is valid only if there are more than 1 camera
+            # quadruplets = info.object.sorted_pos[0]
+            # triplets = info.object.sorted_pos[1]
+            # pairs = info.object.sorted_pos[2]
+            # unused = []  # temporary solution
+
+            # if there are less than 4 cameras, then
+            # there are no quadruplets
+            # only triplets and pairs if 3
+            # only pairs if 2
+
+            # import pdb; pdb.set_trace()
+            # info.object.clear_plots(remove_background=False)
+            for i, subset in enumerate(reversed(info.object.sorted_pos)):
+                x, y = self._clean_correspondences(subset)
+                info.object.drawcross_in_all_cams(
+                    names[i] + "_x", names[i] + "_y", x, y, use_colors[i], 3
+                )
+
+        # x, y = self._clean_correspondences(triplets)
+        # info.object.drawcross("tripl_x", "tripl_y", x, y, "green", 3)
+        # x, y = self._clean_correspondences(pairs)
+        # info.object.drawcross("pair_x", "pair_y", x, y, "yellow", 3)
+        # info.object.drawcross("unused_x","unused_y",unused[:,0],unused[:,1],"blue",3)
+
+    def init_action(self, info):
+        """init_action - clears existing plots from the camera windows,
+        initializes C image arrays with mainGui.orig_image and
+        calls appropriate start_proc_c
+         by using ptv.py_start_proc_c()
+        """
+        mainGui = info.object
+        # synchronize the active run params dir with the temp params dir
+        mainGui.exp1.syncActiveDir()
+
+        for i in range(len(mainGui.camera_list)):
+            try:
+                im = imread(
+                    getattr(
+                        mainGui.exp1.active_params.m_params,
+                        f"Name_{i+1}_Image",
+                    )
+                )
+                if im.ndim > 2:
+                    im = rgb2gray(im)
+
+                mainGui.orig_image[i] = img_as_ubyte(im)
+            except IOError:
+                print("Error reading image, setting zero image")
+                h_img = mainGui.exp1.active_params.m_params.imx
+                v_img = mainGui.exp1.active_params.m_params.imy
+                temp_img = img_as_ubyte(np.zeros((h_img, v_img)))
+                # print(f"setting images of size {temp_img.shape}")
+                exec(f"mainGui.orig_image[{i}] = temp_img")
+
+            if hasattr(mainGui.camera_list[i], "img_plot"):
+                del mainGui.camera_list[i].img_plot
+        mainGui.clear_plots()
+        print("\n Init action \n")
+        # mainGui.update_plots(mainGui.orig_image, is_float=False)
+        mainGui.create_plots(mainGui.orig_image, is_float=False)
+        # mainGui.set_images(mainGui.orig_image)
+
+        (
+            info.object.cpar,
+            info.object.spar,
+            info.object.vpar,
+            info.object.track_par,
+            info.object.tpar,
+            info.object.cals,
+            info.object.epar,
+        ) = ptv.py_start_proc_c(info.object.n_cams)
+        mainGui.pass_init = True
+        print("Read all the parameters and calibrations successfully ")
+
+    def calib_action(self, info):
+        """calib_action - initializes calib class with appropriate number of
+        plot windows, passes to calib class pointer to ptv module and to
+        exp1 class, invokes the calibration GUI
+        """
+        print("\n Starting calibration dialog \n")
+
+        # reset the main GUI so the user will have to press Start again
+        info.object.pass_init = False
+        print("Active parameters set \n")
+        print(info.object.exp1.active_params.par_path)
+        calib_gui = CalibrationGUI(info.object.exp1.active_params.par_path)
+        calib_gui.configure_traits()
+
+    def detection_gui_action(self, info):
+        """activating detection GUI"""
+        print("\n Starting detection GUI dialog \n")
+
+        # reset the main GUI so the user will have to press Start again
+        info.object.pass_init = False
+        print("Active parameters set \n")
+        print(info.object.exp1.active_params.par_path)
+        detection_gui = DetectionGUI(info.object.exp1.active_params.par_path)
+        detection_gui.configure_traits()
+
+    def sequence_action(self, info):
+        """sequence action - implements binding to C sequence function.
+           Original function was split into 2 parts:
+        1) initialization - bonded by ptv.py_sequence_init(..) function
+        2) main loop processing - bonded by ptv.py_sequence_loop(..) function
+        """
+
+        extern_sequence = info.object.plugins.sequence_alg
+        if extern_sequence != "default":
+            try:
+                # change to pyptv folder, look for tracking module
+                sys.path.append(info.exp1.object.software_path)
+                # import chosen tracker from software dir
+
+                seq = importlib.import_module(extern_sequence)
+            except ImportError:
+                print(
+                    "Error loading or running "
+                    + extern_sequence
+                    + ". Falling back to default sequence algorithm"
+                )
+
+            print("Sequence by using " + extern_sequence)
+            sequence = seq.Sequence(
+                ptv=ptv,
+                exp1=info.object.exp1,
+                camera_list=info.object.camera_list,
+            )
+            sequence.do_sequence()
+            # print("Sequence by using "+extern_sequence+" has failed."
+
+        else:
+            ptv.py_sequence_loop(info.object)
+
+    def track_no_disp_action(self, info):
+        """track_no_disp_action uses ptv.py_trackcorr_loop(..) binding to
+        call tracking without display"""
+        extern_tracker = info.object.plugins.track_alg
+        if extern_tracker != "default":
+            try:
+                os.chdir(info.exp1.object.software_path)
+                track = importlib.import_module(extern_tracker)
+            except BaseException:
+                print(
+                    "Error loading "
+                    + extern_tracker
+                    + ". Falling back to default tracker"
+                )
+                extern_tracker = "default"
+            os.chdir(info.exp1.object.exp_path)  # change back to working path
+        if extern_tracker == "default":
+            print("Using default liboptv tracker")
+            info.object.tracker = ptv.py_trackcorr_init(info.object)
+            info.object.tracker.full_forward()
+        else:
+            print("Tracking by using " + extern_tracker)
+            tracker = track.Tracking(ptv=ptv, exp1=info.object.exp1)
+            tracker.do_tracking()
+
+        print("tracking without display finished")
+
+    def track_disp_action(self, info):
+        """tracking with display is handled by TrackThread which does
+        processing step by step and waits for GUI to update before
+        proceeding to the next step
+
+        This was not implemented in PyPTV
+        """
+        info.object.clear_plots(remove_background=False)
+        # info.object.tr_thread = TrackThread()
+        # info.object.tr_thread.start()
+
+    def track_back_action(self, info):
+        """tracking back action is handled by ptv.py_trackback_c() binding"""
+        print("Starting back tracking")
+        info.object.tracker.full_backward()
+
+    def three_d_positions(self, info):
+        """Extracts and saves 3D positions from the list of correspondences"""
+        ptv.py_determination_proc_c(
+            info.object.n_cams,
+            info.object.sorted_pos,
+            info.object.sorted_corresp,
+            info.object.corrected,
+        )
+
+    # def multigrid_demo(self, info):
+    #     demo_window = DemoGUI(ptv=ptv, exp1=info.object.exp1)
+    #     demo_window.configure_traits()
+
+    def detect_part_track(self, info):
+        """track detected particles is handled by 2 bindings:
+        1) tracking_framebuf.read_targets(..)
+        2) ptv.py_get_mark_track_c(..)
+        """
+        info.object.clear_plots(remove_background=False)  # clear everything
+        info.object.update_plots(info.object.orig_image, is_float=False)
+
+        prm = info.object.exp1.active_params.m_params
+        seq_first = prm.Seq_First  # get sequence parameters
+        seq_last = prm.Seq_Last
+        base_names = [
+            prm.Basename_1_Seq,
+            prm.Basename_2_Seq,
+            prm.Basename_3_Seq,
+            prm.Basename_4_Seq,
+        ]
+
+        # load first image from sequence
+        info.object.load_set_seq_image(seq_first)
+
+        print("Starting detect_part_track")
+        x1_a, x2_a, y1_a, y2_a = [], [], [], []
+        for i in range(info.object.n_cams):  # initialize result arrays
+            x1_a.append([])
+            x2_a.append([])
+            y1_a.append([])
+            y2_a.append([])
+
+    # imx, imy = info.object.cpar.get_image_size()
+
+        
+        for i_img in range(info.object.n_cams):
+            for i_seq in range(seq_first, seq_last + 1):  # loop over sequences
+                intx_green, inty_green = [], []
+                intx_blue, inty_blue = [], []
+                targets = optv.tracking_framebuf.read_targets(base_names[i_img], i_seq)
+
+                for t in targets:
+                    if t.tnr() > -1:
+                        intx_green.append(t.pos()[0])
+                        inty_green.append(t.pos()[1])
+                    else:
+                        intx_blue.append(t.pos()[0])
+                        inty_blue.append(t.pos()[1])
+
+                x1_a[i_img] = x1_a[i_img] + intx_green # add current step to result array
+                x2_a[i_img] = x2_a[i_img] + intx_blue
+                y1_a[i_img] = y1_a[i_img] + inty_green
+                y2_a[i_img] = y2_a[i_img] + inty_blue
+
+        # plot result arrays
+        for i_img in range(info.object.n_cams):
+            info.object.camera_list[i_img].drawcross(
+                "x_tr_gr", "y_tr_gr", x1_a[i_img], y1_a[i_img], "green", 3)
+            info.object.camera_list[i_img].drawcross(
+                "x_tr_bl","y_tr_bl", x2_a[i_img], y2_a[i_img], "blue",  2)
+            
+            info.object.camera_list[i_img]._plot.request_redraw()
+
+        print("Finished detect_part_track")
+
+    def traject_action_flowtracks(self, info):
+        """Shows trajectories reading and organizing by flowtracks
+
+        Args:
+            info (_type_): _description_
+        """
+        info.object.clear_plots(remove_background=False)
+        seq_first = info.object.exp1.active_params.m_params.Seq_First
+        seq_last = info.object.exp1.active_params.m_params.Seq_Last
+        info.object.load_set_seq_image(seq_first, display_only=True)
+
+        from flowtracks.io import trajectories_ptvis
+
+        dataset = trajectories_ptvis(
+            "res/ptv_is.%d", first=seq_first, last=seq_last, xuap=False, traj_min_len=3
+        )
+
+        heads_x, heads_y = [], []
+        tails_x, tails_y = [], []
+        ends_x, ends_y = [], []
+        for i_cam in range(info.object.n_cams):
+            head_x, head_y = [], []
+            tail_x, tail_y = [], []
+            end_x, end_y = [], []
+            for traj in dataset:
+                # projected = optv.imgcoord.image_coordinates(
+                #     np.atleast_2d(traj.pos()[0]*1000),
+                #     info.object.cals[i_cam],
+                #     info.object.cpar.get_multimedia_params(),
+                # )
+                # pos = optv.transforms.convert_arr_metric_to_pixel(
+                #     projected, info.object.cpar)
+
+                # head_x.append(pos[0][0])
+                # head_y.append(pos[0][1])
+
+                projected = optv.imgcoord.image_coordinates(
+                    np.atleast_2d(traj.pos() * 1000),
+                    info.object.cals[i_cam],
+                    info.object.cpar.get_multimedia_params(),
+                )
+                pos = optv.transforms.convert_arr_metric_to_pixel(
+                    projected, info.object.cpar
+                )
+
+                head_x.append(pos[0, 0])  # first row
+                head_y.append(pos[0, 1])
+                tail_x.extend(list(pos[1:-1, 0]))  # all other rows,
+                tail_y.extend(list(pos[1:-1, 1]))
+                end_x.append(pos[-1, 0])
+                end_y.append(pos[-1, 1])
+
+            heads_x.append(head_x)
+            heads_y.append(head_y)
+            tails_x.append(tail_x)
+            tails_y.append(tail_y)
+            ends_x.append(end_x)
+            ends_y.append(end_y)
+
+        for i_cam in range(info.object.n_cams):
+            info.object.camera_list[i_cam].drawcross(
+                "heads_x", "heads_y", heads_x[i_cam], heads_y[i_cam], "red", 3
+            )
+            info.object.camera_list[i_cam].drawcross(
+                "tails_x", "tails_y", tails_x[i_cam], tails_y[i_cam], "green", 2
+            )
+            info.object.camera_list[i_cam].drawcross(
+                "ends_x", "ends_y", ends_x[i_cam], ends_y[i_cam], "orange", 3
+            )
+
+
+    def plugin_action(self, info):
+        """Configure plugins by using GUI"""
+        info.object.plugins.read()
+        info.object.plugins.configure_traits()
+
+    def ptv_is_to_paraview(self, info):
+        """Button that runs the ptv_is.# conversion to Paraview"""
+
+        print("Saving trajectories for Paraview\n")
+        info.object.clear_plots(remove_background=False)
+        seq_first = info.object.exp1.active_params.m_params.Seq_First
+        seq_last = info.object.exp1.active_params.m_params.Seq_Last
+        info.object.load_set_seq_image(seq_first, display_only=True)
+
+        # borrowed from flowtracks that does much better job on this
+        # I think it's too much to import also postptv here, later
+        # we will make a single conda package for the full stack
+
+        # Example notebook translating OpenPTV files for Paraview using flowtracks
+        import pandas as pd
+        from flowtracks.io import trajectories_ptvis
+
+        dataset = trajectories_ptvis("res/ptv_is.%d", xuap=False)
+
+        dataframes = []
+        for traj in dataset:
+            dataframes.append(
+                pd.DataFrame.from_records(
+                    traj, columns=["x", "y", "z", "dx", "dy", "dz", "frame", "particle"]
+                )
+            )
+
+        df = pd.concat(dataframes, ignore_index=True)
+        df["particle"] = df["particle"].astype(np.int32)
+
+        # Paraview does not recognize it as a set without _000001.txt, so we the first 10000
+        # ptv_is.10001 is becoming ptv_00001.txt
+
+        df["frame"] = df["frame"].astype(np.int32)
+
+        df.reset_index(inplace=True, drop=True)
+        print(df.head())
+
+        df_grouped = df.reset_index().groupby("frame")
+        for index, group in df_grouped:
+            group.to_csv(
+                f"./res/ptv_{int(index):05d}.txt",
+                mode="w",
+                columns=["particle", "x", "y", "z", "dx", "dy", "dz"],
+                index=False,
+            )
+
+        print("Saving trajectories to Paraview finished\n")
+
+
+# ----------------------------------------------------------------
+# Actions associated with right mouse button clicks (treeeditor)
+# ---------------------------------------------------------------
+ConfigMainParams = Action(
+    name="Main parameters", action="handler.configure_main_par(editor,object)"
+)
+ConfigCalibParams = Action(
+    name="Calibration parameters",
+    action="handler.configure_cal_par(editor,object)",
+)
+ConfigTrackParams = Action(
+    name="Tracking parameters",
+    action="handler.configure_track_par(editor,object)",
+)
+SetAsDefault = Action(name="Set as active", action="handler.set_active(editor,object)")
+CopySetParams = Action(
+    name="Copy set of parameters",
+    action="handler.copy_set_params(editor,object)",
+)
+RenameSetParams = Action(
+    name="Rename run", action="handler.rename_set_params(editor,object)"
+)
+DeleteSetParams = Action(
+    name="Delete run", action="handler.delete_set_params(editor,object)"
+)
+
+# -----------------------------------------
+# Defines the menubar
+# ------------------------------------------
+menu_bar = MenuBar(
+    Menu(
+        Action(name="New", action="new_action"),
+        Action(name="Open", action="open_action"),
+        Action(name="Save As", action="saveas_action"),
+        Action(name="Exit", action="exit_action"),
+        name="File",
+    ),
+    Menu(Action(name="Init / Restart", action="init_action"), name="Start"),
+    Menu(
+        Action(
+            name="High pass filter",
+            action="highpass_action",
+            enabled_when="pass_init",
+        ),
+        Action(
+            name="Image coord",
+            action="img_coord_action",
+            enabled_when="pass_init",
+        ),
+        Action(
+            name="Correspondences",
+            action="corresp_action",
+            enabled_when="pass_init",
+        ),
+        name="Preprocess",
+    ),
+    Menu(
+        Action(
+            name="3D positions",
+            action="three_d_positions",
+            enabled_when="pass_init",
+        ),
+        name="3D Positions",
+    ),
+    Menu(
+        Action(
+            name="Create calibration",
+            action="calib_action",
+            enabled_when="pass_init",
+        ),
+        name="Calibration",
+    ),
+    Menu(
+        Action(
+            name="Sequence without display",
+            action="sequence_action",
+            enabled_when="pass_init",
+        ),
+        name="Sequence",
+    ),
+    Menu(
+        Action(
+            name="Detected Particles",
+            action="detect_part_track",
+            enabled_when="pass_init",
+        ),
+        Action(
+            name="Tracking without display",
+            action="track_no_disp_action",
+            enabled_when="pass_init",
+        ),
+        # not implemented Action(name='Tracking with
+        # display',action='track_disp_action',enabled_when='pass_init'),
+        Action(
+            name="Tracking backwards",
+            action="track_back_action",
+            enabled_when="pass_init",
+        ),
+        Action(
+            name="Show trajectories",
+            action="traject_action_flowtracks",
+            enabled_when="pass_init",
+        ),
+        Action(
+            name="Save Paraview files",
+            action="ptv_is_to_paraview",
+            enabled_when="pass_init",
+        ),
+        name="Tracking",
+    ),
+    Menu(Action(name="Select plugin", action="plugin_action"), name="Plugins"),
+    Menu(
+        Action(name="Detection GUI demo", action="detection_gui_action"),
+        name="Detection demo",
+    ),
+)
+
+# ----------------------------------------
+# tree editor for the Experiment() class
+#
+tree_editor_exp = TreeEditor(
+    nodes=[
+        TreeNode(
+            node_for=[Experiment],
+            auto_open=True,
+            children="",
+            label="=Experiment",
+        ),
+        TreeNode(
+            node_for=[Experiment],
+            auto_open=True,
+            children="paramsets",
+            label="=Parameters",
+            add=[Paramset],
+            menu=Menu(CopySetParams),
+        ),
+        TreeNode(
+            node_for=[Paramset],
+            auto_open=True,
+            children="",
+            label="name",
+            menu=Menu(
+                # NewAction,
+                CopySetParams,
+                RenameSetParams,
+                DeleteSetParams,
+                Separator(),
+                ConfigMainParams,
+                ConfigCalibParams,
+                ConfigTrackParams,
+                Separator(),
+                SetAsDefault,
+            ),
+        ),
+    ],
+    editable=False,
+)
+
+
+# -------------------------------------------------------------------------
+class Plugins(HasTraits):
+    track_list = List
+    seq_list = List
+    track_alg = Enum(values="track_list")
+    sequence_alg = Enum(values="seq_list")
+    view = View(
+        Group(
+            Item(name="track_alg", label="Choose tracking algorithm:"),
+            Item(name="sequence_alg", label="Choose sequence algorithm:"),
+        ),
+        buttons=["OK"],
+        title="External plugins configuration",
+    )
+
+    def __init__(self):
+        self.read()
+
+    def read(self):
+        # reading external tracking
+        if os.path.exists(
+            os.path.join(os.path.abspath(os.curdir), "external_tracker_list.txt")
+        ):
+            with open(
+                os.path.join(os.path.abspath(os.curdir), "external_tracker_list.txt"),
+                "r",
+            ) as f:
+                trackers = f.read().split("\n")
+                trackers.insert(0, "default")
+                self.track_list = trackers
+        else:
+            self.track_list = ["default"]
+        # reading external sequence
+        if os.path.exists(
+            os.path.join(os.path.abspath(os.curdir), "external_sequence_list.txt")
+        ):
+            with open(
+                os.path.join(os.path.abspath(os.curdir), "external_sequence_list.txt"),
+                "r",
+            ) as f:
+                seq = f.read().split("\n")
+                seq.insert(0, "default")
+                self.seq_list = seq
+        else:
+            self.seq_list = ["default"]
+
+
+# ----------------------------------------------
+class MainGUI(HasTraits):
+    """MainGUI is the main class under which the Model-View-Control
+    (MVC) model is defined"""
+
+    camera_list = List
+    # imgplt_flag = 0
+    pass_init = Bool(False)
+    update_thread_plot = Bool(False)
+    # tr_thread = Instance(TrackThread)
+    selected = Any
+
+    # Defines GUI view --------------------------
+    view = View(
+        Group(
+            Group(
+                Item(
+                    name="exp1",
+                    editor=tree_editor_exp,
+                    show_label=False,
+                    width=-400,
+                    resizable=False,
+                ),
+                Item(
+                    "camera_list",
+                    style="custom",
+                    editor=ListEditor(
+                        use_notebook=True,
+                        deletable=False,
+                        dock_style="tab",
+                        page_name=".name",
+                        selected="selected",
+                    ),
+                    show_label=False,
+                ),
+                orientation="horizontal",
+                show_left=False,
+            ),
+            orientation="vertical",
+        ),
+        title="pyPTV ver. 0.2.3",
+        id="main_view",
+        width=1.0,
+        height=1.0,
+        resizable=True,
+        handler=TreeMenuHandler(),  # <== Handler class is attached
+        menubar=menu_bar,
+    )
+
+    def _selected_changed(self):
+        self.current_camera = int(self.selected.name.split(" ")[1]) - 1
+
+    # ---------------------------------------------------
+    # Constructor and Chaco windows initialization
+    # ---------------------------------------------------
+    def __init__(self, exp_path: Path, software_path: Path):
+        super(MainGUI, self).__init__()
+        colors = ["yellow", "green", "red", "blue"]
+        self.exp1 = Experiment()
+        self.exp1.populate_runs(exp_path)
+        self.plugins = Plugins()
+        self.n_cams = self.exp1.active_params.m_params.Num_Cam
+        self.orig_image = self.n_cams * [[]]
+        self.current_camera = 0
+        self.camera_list = [
+            CameraWindow(colors[i], f"Camera {i+1}") for i in range(self.n_cams)
+        ]
+        self.software_path = software_path
+        self.exp_path = exp_path
+        for i in range(self.n_cams):
+            self.camera_list[i].on_trait_change(self.right_click_process, "rclicked")
+
+    def right_click_process(self):
+        """
+        Shows a line in camera color code corresponding to a point on another
+        camera's view plane.
+        """        
+        num_points = 2
+        
+        try:
+            _ = self.sorted_pos
+            plot_epipolar = True
+        except:
+            plot_epipolar = False
+            
+        
+        if plot_epipolar:
+
+            i = self.current_camera
+            point = np.array(
+                [
+                    self.camera_list[i]._click_tool.x,
+                    self.camera_list[i]._click_tool.y,
+                ],
+                dtype="float64",
+            )
+            
+            # find closest point
+            for pos_type in self.sorted_pos: # quadruplet, triplet, pair
+                distances = np.linalg.norm(pos_type[i] - point, axis=1)
+                if np.min(distances) < 5 :
+                    point = pos_type[i][np.argmin(distances)]
+                    
+            
+            if not np.allclose(point, [0.0, 0.0]):
+                # mark the point with a circle
+                c = str(np.random.rand())[2:]
+                self.camera_list[i].drawcross(
+                    "right_p_x0" + c,
+                    "right_p_y0" + c,
+                    point[0],
+                    point[1],
+                    "cyan",
+                    3,
+                    marker="circle",
+                )
+
+                # look for points along epipolars for other cameras
+                for j in range(self.n_cams):
+                    if i == j:
+                        continue
+                    pts = optv.epipolar.epipolar_curve(
+                        point,
+                        self.cals[i],
+                        self.cals[j],
+                        num_points,
+                        self.cpar,
+                        self.vpar,
+                    )
+
+                    if len(pts) > 1:
+                        self.camera_list[j].drawline(
+                            "right_cl_x" + c,
+                            "right_cl_y" + c,
+                            pts[0, 0],
+                            pts[0, 1],
+                            pts[-1, 0],
+                            pts[-1, 1],
+                            self.camera_list[i].cam_color,
+                        )
+                
+                self.camera_list[i].rclicked = 0
+                        
+        
+
+    def create_plots(self, images, is_float=False) -> None:
+        """update_plots
+
+        Args:
+            images (_type_): images to update
+            is_float (bool, optional): _description_. Defaults to False.
+        """
+        print("inside update plots, images changed\n")
+        for i in range(self.n_cams):
+            self.camera_list[i].create_image(images[i], is_float)
+            self.camera_list[i]._plot.request_redraw()
+            
+    def update_plots(self, images, is_float=False) -> None:
+        """update_plots
+
+        Args:
+            images (_type_): images to update
+            is_float (bool, optional): _description_. Defaults to False.
+        """
+        print("inside update plots, images changed\n")
+        for i in range(self.n_cams):
+            self.camera_list[i].update_image(images[i], is_float)
+            self.camera_list[i]._plot.request_redraw()
+
+    def drawcross_in_all_cams(self, str_x, str_y, x, y, color1, size1, marker="plus"):
+        """
+        Draws crosses
+        """
+        for i, cam in enumerate(self.camera_list):
+            cam.drawcross(str_x, str_y, x[i], y[i], color1, size1, marker=marker)
+
+    def clear_plots(self, remove_background=True):
+        # this function deletes all plots except basic image plot
+
+        if not remove_background:
+            index = "plot0"
+        else:
+            index = None
+
+        for i in range(self.n_cams):
+            plot_list = list(self.camera_list[i]._plot.plots.keys())
+            # if not remove_background:
+            #   index=None
+            if index in plot_list:
+                # try:
+                plot_list.remove(index)
+            # except:
+            # pass
+            self.camera_list[i]._plot.delplot(*plot_list[0:])
+            self.camera_list[i]._plot.tools = []
+            self.camera_list[i]._plot.request_redraw()
+            for j in range(len(self.camera_list[i]._quiverplots)):
+                self.camera_list[i]._plot.remove(self.camera_list[i]._quiverplots[j])
+            self.camera_list[i]._quiverplots = []
+            self.camera_list[i].right_p_x0 = []
+            self.camera_list[i].right_p_y0 = []
+            self.camera_list[i].right_p_x1 = []
+            self.camera_list[i].right_p_y1 = []
+
+    def _update_thread_plot_changed(self):
+        n_cams = len(self.camera_list)
+
+        if self.update_thread_plot and self.tr_thread:
+            print("updating plots..\n")
+            step = self.tr_thread.track_step
+
+            x0, x1, x2, y0, y1, y2 = (
+                self.tr_thread.intx0,
+                self.tr_thread.intx1,
+                self.tr_thread.intx2,
+                self.tr_thread.inty0,
+                self.tr_thread.inty1,
+                self.tr_thread.inty2,
+            )
+            for i in range(n_cams):
+                self.camera_list[i].drawcross(
+                    str(step) + "x0",
+                    str(step) + "y0",
+                    x0[i],
+                    y0[i],
+                    "green",
+                    2,
+                )
+                self.camera_list[i].drawcross(
+                    str(step) + "x1",
+                    str(step) + "y1",
+                    x1[i],
+                    y1[i],
+                    "yellow",
+                    2,
+                )
+                self.camera_list[i].drawcross(
+                    str(step) + "x2",
+                    str(step) + "y2",
+                    x2[i],
+                    y2[i],
+                    "white",
+                    2,
+                )
+                self.camera_list[i].drawquiver(x0[i], y0[i], x1[i], y1[i], "orange")
+                self.camera_list[i].drawquiver(x1[i], y1[i], x2[i], y2[i], "white")
+            # for j in range (m_tr):
+            # str_plt=str(step)+"_"+str(j)
+            ##
+            # self.camera_list[i].drawline\
+            # (str_plt+"vec_x0",str_plt+"vec_y0",x0[i][j],y0[i][j],x1[i][j],y1[i][j],"orange")
+            # self.camera_list[i].drawline\
+            # (str_plt+"vec_x1",str_plt+"vec_y1",x1[i][j],y1[i][j],x2[i][j],y2[i][j],"white")
+            self.load_set_seq_image(step, update_all=False, display_only=True)
+            self.camera_list[self.current_camera]._plot.request_redraw()
+            time.sleep(0.1)
+            self.tr_thread.can_continue = True
+            self.update_thread_plot = False
+
+    def load_set_seq_image(self, seq: int, update_all=True, display_only=False):
+        """load and set sequence image
+
+        Args:
+            seq (_type_): sequance properties
+            update_all (bool, optional): _description_. Defaults to True.
+            display_only (bool, optional): _description_. Defaults to False.
+        """
+        n_cams = len(self.camera_list)
+        if not hasattr(self, "base_name"):
+            self.base_name = []
+            for i in range(n_cams):
+                exec(
+                    "self.base_name.append"
+                    + f"(self.exp1.active_params.m_params.Basename_{i+1}_Seq)"
+                )
+                # print(f" base name in GUI is {self.base_name[i]}")
+
+        # i = seq
+        seq_ch = f"{seq:04d}"
+
+        if not update_all:
+            j = self.current_camera
+            # img_name = self.base_name[j] + seq_ch
+            img_name = self.base_name[j].replace("#", seq_ch)
+            # print(f"Image name in load_set_seq is {img_name}")
+            self.load_disp_image(img_name, j, display_only)
+        else:
+            for j in range(n_cams):
+                # img_name = self.base_name[j] + seq_ch
+                img_name = self.base_name[j].replace("#", seq_ch)
+                # print(f"Image name in load_set_seq is {img_name}")
+                self.load_disp_image(img_name, j, display_only)
+
+    def load_disp_image(self, img_name: str, j: int, display_only: bool = False):
+        """load and display image
+
+        Args:
+            img_name (_type_): filename of the image
+            j (_type_): integer counter
+            display_only (bool, optional): display only. Defaults to False.
+        """
+        # print(f"Setting image: {img_name}")
+        try:
+            temp_img = img_as_ubyte(imread(img_name))
+        except IOError:
+            print("Error reading file, setting zero image")
+            h_img = self.exp1.active_params.m_params.imx
+            v_img = self.exp1.active_params.m_params.imy
+            temp_img = img_as_ubyte(np.zeros((h_img, v_img)))
+        # if not display_only:
+        #     ptv.py_set_img(temp_img, j)
+        if len(temp_img) > 0:
+            self.camera_list[j].update_image(temp_img)
+
+
+def printException():
+    import traceback
+
+    print("=" * 50)
+    print("Exception:", sys.exc_info()[1])
+    print(f"{Path.cwd()}")
+    print("Traceback:")
+    traceback.print_tb(sys.exc_info()[2])
+    print("=" * 50)
+
+
+# -------------------------------------------------------------
+def main():
+    """main ()
+
+    Raises:
+        OSError: if software or folder path are missing
+    """
+    # Parse inputs:
+    software_path = Path.cwd().resolve()
+    print(f"Software path is {software_path}")
+
+    # Path to the experiment
+    if len(sys.argv) > 1:
+        exp_path = Path(sys.argv[1]).resolve()
+        print(f"Experimental path is {exp_path}")
+    else:
+        exp_path = software_path.parent / "test_cavity"
+        print(f"Without input, PyPTV fallbacks to a default {exp_path} \n")
+
+    if not exp_path.is_dir() or not exp_path.exists():
+        raise OSError(f"Wrong experimental directory {exp_path}")
+
+    # Change directory to the path
+    os.chdir(exp_path)
+
+    try:
+        main_gui = MainGUI(exp_path, software_path)
+        main_gui.configure_traits()
+    except OSError:
+        print("something wrong with the software or folder")
+        printException()
+
+    os.chdir(software_path)  # get back to the original workdir
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `pyptv-0.2.2/pyptv/quiverplot.py` & `pyptv-0.2.3/pyptv/quiverplot.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,143 +1,143 @@
-# Chaco relative imports
-from chaco.api import AbstractDataSource
-from chaco.api import ScatterPlot
-
-# Enthought library imports
-from enable.api import ColorTrait
-from numpy import (
-    array,
-    compress,
-    matrix,
-    newaxis,
-    sqrt,
-    transpose,
-    invert,
-    isnan,
-)
-from traits.api import Array, Enum, Float, Instance, Int
-
-
-class QuiverPlot(ScatterPlot):
-
-    # Determines how to interpret the data in the **vectors** data source.
-    # 	"vector": each tuple is a (dx, dy)
-    # 	"radial": each tuple is an (r, theta)
-    data_type = Enum("vector", "radial")  # TODO: implement "radial"
-
-    # A datasource that returns an Nx2 array array indicating directions
-    # of the vectors.  The interpretation of this array is dependent on
-    # the setting of the **data_type** attribute.
-    #
-    # Usually this will be a MultiArrayDataSource.
-    vectors = Instance(AbstractDataSource)
-
-    # ------------------------------------------------------------------------
-    # Visual attributes of the vector
-    # ------------------------------------------------------------------------
-
-    # The color of the lines
-    line_color = ColorTrait("black")
-
-    # The width of the lines
-    line_width = Float(1.0)
-
-    # The length, in pixels, of the arrowhead
-    arrow_size = Int(5)
-
-    # ------------------------------------------------------------------------
-    # Private traits
-    # ------------------------------------------------------------------------
-
-    _cached_vector_data = Array
-    _selected_vector_data = Array
-
-    def _gather_points_old(self):
-        """
-        Collects the data points that are within the bounds of the plot and
-        caches them
-        Overrides scatterplot's function
-        """
-        if self._cache_valid and self._selection_cache_valid:
-            return
-
-        if not self.index or not self.value:
-            return
-
-        index, index_mask = self.index.get_data_mask()
-        value, value_mask = self.value.get_data_mask()
-        ep_index, ep_value = self.ep_index, self.ep_value
-        if len(index) == 0 or len(value) == 0 or len(index) != len(value):
-            self._cached_data_pts = []
-            self._cached_point_mask = []
-            self._cache_valid = True
-            return
-
-        index_range_mask = self.index_mapper.range.mask_data(index)
-        value_range_mask = self.value_mapper.range.mask_data(value)
-        ep_index_mask = self.index_mapper.range.mask_data(ep_index)
-        ep_value_mask = self.value_mapper.range.mask_data(ep_value)
-
-        nan_mask = (
-            invert(isnan(index))
-            & index_mask
-            & invert(isnan(value))
-            & value_mask
-        )
-        point_mask = (
-            nan_mask
-            & index_range_mask
-            & value_range_mask
-            & ep_index_mask
-            & ep_value_mask
-        )
-        if not self._cache_valid:
-            points = transpose(array((index, value)))
-            endpoints = transpose(array((ep_index, ep_value)))
-            self._cached_data_pts = compress(point_mask, points, axis=0)
-            self._cached_end_epts = compress(point_mask, endpoints, axis=0)
-            self._cached_point_mask = point_mask[:]
-            self._cache_valid = True
-
-        return
-
-    def _render(self, gc, points, icon_mode=False):
-        gc.save_state()
-        gc.clip_to_rect(self.x, self.y, self.width, self.height)
-        # print "inside render"
-        gc.set_stroke_color(self.line_color_)
-        gc.set_line_width(self.line_width)
-
-        # Draw the body of the arrow
-        starts = points
-        ends = self.map_screen(self._cached_end_epts)
-
-        if len(starts) > 0:
-            gc.begin_path()
-            gc.line_set(starts, ends)
-            # gc.line_set(starts, self.end_points)
-            gc.stroke_path()
-
-        if self.arrow_size > 0:
-            vec = self._cached_vector_data
-            unit_vec = vec / sqrt(vec[:, 0] ** 2 + vec[:, 1] ** 2)[:, newaxis]
-            a = 0.707106781  # sqrt(2)/2
-
-            # Draw the left arrowhead (for an arrow pointing straight up)
-            arrow_ends = (
-                ends
-                - array(unit_vec * matrix([[a, a], [-a, a]])) * self.arrow_size
-            )
-            gc.begin_path()
-            gc.line_set(ends, arrow_ends)
-            gc.stroke_path()
-
-            # Draw the left arrowhead (for an arrow pointing straight up)
-            arrow_ends = (
-                ends
-                - array(unit_vec * matrix([[a, -a], [a, a]])) * self.arrow_size
-            )
-            gc.begin_path()
-            gc.line_set(ends, arrow_ends)
-            gc.stroke_path()
-
-        gc.restore_state()
+# Chaco relative imports
+from chaco.api import AbstractDataSource
+from chaco.api import ScatterPlot
+
+# Enthought library imports
+from enable.api import ColorTrait
+from numpy import (
+    array,
+    compress,
+    matrix,
+    newaxis,
+    sqrt,
+    transpose,
+    invert,
+    isnan,
+)
+from traits.api import Array, Enum, Float, Instance, Int
+
+
+class QuiverPlot(ScatterPlot):
+
+    # Determines how to interpret the data in the **vectors** data source.
+    # 	"vector": each tuple is a (dx, dy)
+    # 	"radial": each tuple is an (r, theta)
+    data_type = Enum("vector", "radial")  # TODO: implement "radial"
+
+    # A datasource that returns an Nx2 array array indicating directions
+    # of the vectors.  The interpretation of this array is dependent on
+    # the setting of the **data_type** attribute.
+    #
+    # Usually this will be a MultiArrayDataSource.
+    vectors = Instance(AbstractDataSource)
+
+    # ------------------------------------------------------------------------
+    # Visual attributes of the vector
+    # ------------------------------------------------------------------------
+
+    # The color of the lines
+    line_color = ColorTrait("black")
+
+    # The width of the lines
+    line_width = Float(1.0)
+
+    # The length, in pixels, of the arrowhead
+    arrow_size = Int(5)
+
+    # ------------------------------------------------------------------------
+    # Private traits
+    # ------------------------------------------------------------------------
+
+    _cached_vector_data = Array
+    _selected_vector_data = Array
+
+    def _gather_points_old(self):
+        """
+        Collects the data points that are within the bounds of the plot and
+        caches them
+        Overrides scatterplot's function
+        """
+        if self._cache_valid and self._selection_cache_valid:
+            return
+
+        if not self.index or not self.value:
+            return
+
+        index, index_mask = self.index.get_data_mask()
+        value, value_mask = self.value.get_data_mask()
+        ep_index, ep_value = self.ep_index, self.ep_value
+        if len(index) == 0 or len(value) == 0 or len(index) != len(value):
+            self._cached_data_pts = []
+            self._cached_point_mask = []
+            self._cache_valid = True
+            return
+
+        index_range_mask = self.index_mapper.range.mask_data(index)
+        value_range_mask = self.value_mapper.range.mask_data(value)
+        ep_index_mask = self.index_mapper.range.mask_data(ep_index)
+        ep_value_mask = self.value_mapper.range.mask_data(ep_value)
+
+        nan_mask = (
+            invert(isnan(index))
+            & index_mask
+            & invert(isnan(value))
+            & value_mask
+        )
+        point_mask = (
+            nan_mask
+            & index_range_mask
+            & value_range_mask
+            & ep_index_mask
+            & ep_value_mask
+        )
+        if not self._cache_valid:
+            points = transpose(array((index, value)))
+            endpoints = transpose(array((ep_index, ep_value)))
+            self._cached_data_pts = compress(point_mask, points, axis=0)
+            self._cached_end_epts = compress(point_mask, endpoints, axis=0)
+            self._cached_point_mask = point_mask[:]
+            self._cache_valid = True
+
+        return
+
+    def _render(self, gc, points, icon_mode=False):
+        gc.save_state()
+        gc.clip_to_rect(self.x, self.y, self.width, self.height)
+        # print "inside render"
+        gc.set_stroke_color(self.line_color_)
+        gc.set_line_width(self.line_width)
+
+        # Draw the body of the arrow
+        starts = points
+        ends = self.map_screen(self._cached_end_epts)
+
+        if len(starts) > 0:
+            gc.begin_path()
+            gc.line_set(starts, ends)
+            # gc.line_set(starts, self.end_points)
+            gc.stroke_path()
+
+        if self.arrow_size > 0:
+            vec = self._cached_vector_data
+            unit_vec = vec / sqrt(vec[:, 0] ** 2 + vec[:, 1] ** 2)[:, newaxis]
+            a = 0.707106781  # sqrt(2)/2
+
+            # Draw the left arrowhead (for an arrow pointing straight up)
+            arrow_ends = (
+                ends
+                - array(unit_vec * matrix([[a, a], [-a, a]])) * self.arrow_size
+            )
+            gc.begin_path()
+            gc.line_set(ends, arrow_ends)
+            gc.stroke_path()
+
+            # Draw the left arrowhead (for an arrow pointing straight up)
+            arrow_ends = (
+                ends
+                - array(unit_vec * matrix([[a, -a], [a, a]])) * self.arrow_size
+            )
+            gc.begin_path()
+            gc.line_set(ends, arrow_ends)
+            gc.stroke_path()
+
+        gc.restore_state()
```

### Comparing `pyptv-0.2.2/pyptv/text_box_overlay.py` & `pyptv-0.2.3/pyptv/text_box_overlay.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,132 +1,132 @@
-""" Defines the TextBoxOverlay class.
-"""
-# Enthought library imports
-from enable.api import ColorTrait, AbstractOverlay, Label, black_color_trait
-from kiva.trait_defs.kiva_font_trait import KivaFont
-from traits.api import Any, Enum, Int, Str, Float, Trait
-
-
-# Local, relative imports
-class TextBoxOverlay(AbstractOverlay):
-    """Draws a box with a text in it"""
-
-    #### Configuration traits ################################################
-    # The text to display in the box.
-    text = Str
-
-    # The font to use for the text.
-    font = KivaFont("swiss 12")
-
-    # The background color for the box (overrides AbstractOverlay).
-    bgcolor = ColorTrait("transparent")
-
-    # The alpha value to apply to **bgcolor**
-    alpha = Trait(1.0, None, Float)
-
-    # The color of the outside box.
-    border_color = ColorTrait("dodgerblue")
-
-    # The color of the text in the tooltip
-    text_color = black_color_trait
-
-    # The thickness of box border.
-    border_size = Int(1)
-
-    # Number of pixels of padding around the text within the box.
-    padding = Int(5)
-
-    # Alignment of the text in the box:
-    #
-    # * "ur": upper right
-    # * "ul": upper left
-    # * "ll": lower left
-    # * "lr": lower right
-    align = Enum("ur", "ul", "ll", "lr")
-    # This allows subclasses to specify an alternate position for the root
-    # of the text box.	Must be a sequence of length 2.
-    alternate_position = Any
-
-    #### Public 'AbstractOverlay' interface ##################################
-    def overlay(self, component, gc, view_bounds=None, mode="normal"):
-        """Draws the box overlaid on another component.
-
-        Overrides AbstractOverlay.
-        """
-        if not self.visible:
-            return
-
-        # draw the label on a transparent box. This allows us to draw
-        # different shapes and put the text inside it without the label
-        # filling a rectangle on top of it
-        label = Label(
-            text=self.text,
-            font=self.font,
-            bgcolor="transparent",
-            color=self.text_color,
-            margin=5,
-        )
-        width, height = label.get_width_height(gc)
-        valign, halign = self.align
-        if self.alternate_position:
-            x, y = self.alternate_position
-            if valign == "u":
-                y += self.padding
-            else:
-                y -= self.padding + height
-            if halign == "r":
-                x += self.padding
-            else:
-                x -= self.padding + width
-        else:
-            if valign == "u":
-                y = component.y2 - self.padding - height
-            else:
-                y = component.y + self.padding
-            if halign == "r":
-                x = component.x2 - self.padding - width
-            else:
-                x = component.x + self.padding
-        # attempt to get the box entirely within the component
-        if x + width > component.width:
-            x = max(0, component.width - width)
-        if y + height > component.height:
-            y = max(0, component.height - height)
-        elif y < 0:
-            y = 0
-        # apply the alpha channel
-        color = self.bgcolor_
-        if self.bgcolor != "transparent":
-            if self.alpha:
-                color = list(self.bgcolor_)
-                if len(color) == 4:
-                    color[3] = self.alpha
-                else:
-                    color += [self.alpha]
-        gc.save_state()
-        try:
-            gc.translate_ctm(x, y)
-
-            gc.set_line_width(self.border_size)
-            gc.set_stroke_color(self.border_color_)
-            gc.set_fill_color(color)
-
-            # draw a rounded rectangle
-            x = y = 0
-            end_radius = 8.0
-            gc.begin_path()
-            gc.move_to(x + end_radius, y)
-            gc.arc_to(x + width, y, x + width, y + end_radius, end_radius)
-            gc.arc_to(
-                x + width,
-                y + height,
-                x + width - end_radius,
-                y + height,
-                end_radius,
-            )
-            gc.arc_to(x, y + height, x, y, end_radius)
-            gc.arc_to(x, y, x + width + end_radius, y, end_radius)
-            gc.draw_path()
-
-            label.draw(gc)
-        finally:
-            gc.restore_state()
+""" Defines the TextBoxOverlay class.
+"""
+# Enthought library imports
+from enable.api import ColorTrait, AbstractOverlay, Label, black_color_trait
+from kiva.trait_defs.kiva_font_trait import KivaFont
+from traits.api import Any, Enum, Int, Str, Float, Trait
+
+
+# Local, relative imports
+class TextBoxOverlay(AbstractOverlay):
+    """Draws a box with a text in it"""
+
+    #### Configuration traits ################################################
+    # The text to display in the box.
+    text = Str
+
+    # The font to use for the text.
+    font = KivaFont("swiss 12")
+
+    # The background color for the box (overrides AbstractOverlay).
+    bgcolor = ColorTrait("transparent")
+
+    # The alpha value to apply to **bgcolor**
+    alpha = Trait(1.0, None, Float)
+
+    # The color of the outside box.
+    border_color = ColorTrait("dodgerblue")
+
+    # The color of the text in the tooltip
+    text_color = black_color_trait
+
+    # The thickness of box border.
+    border_size = Int(1)
+
+    # Number of pixels of padding around the text within the box.
+    padding = Int(5)
+
+    # Alignment of the text in the box:
+    #
+    # * "ur": upper right
+    # * "ul": upper left
+    # * "ll": lower left
+    # * "lr": lower right
+    align = Enum("ur", "ul", "ll", "lr")
+    # This allows subclasses to specify an alternate position for the root
+    # of the text box.	Must be a sequence of length 2.
+    alternate_position = Any
+
+    #### Public 'AbstractOverlay' interface ##################################
+    def overlay(self, component, gc, view_bounds=None, mode="normal"):
+        """Draws the box overlaid on another component.
+
+        Overrides AbstractOverlay.
+        """
+        if not self.visible:
+            return
+
+        # draw the label on a transparent box. This allows us to draw
+        # different shapes and put the text inside it without the label
+        # filling a rectangle on top of it
+        label = Label(
+            text=self.text,
+            font=self.font,
+            bgcolor="transparent",
+            color=self.text_color,
+            margin=5,
+        )
+        width, height = label.get_width_height(gc)
+        valign, halign = self.align
+        if self.alternate_position:
+            x, y = self.alternate_position
+            if valign == "u":
+                y += self.padding
+            else:
+                y -= self.padding + height
+            if halign == "r":
+                x += self.padding
+            else:
+                x -= self.padding + width
+        else:
+            if valign == "u":
+                y = component.y2 - self.padding - height
+            else:
+                y = component.y + self.padding
+            if halign == "r":
+                x = component.x2 - self.padding - width
+            else:
+                x = component.x + self.padding
+        # attempt to get the box entirely within the component
+        if x + width > component.width:
+            x = max(0, component.width - width)
+        if y + height > component.height:
+            y = max(0, component.height - height)
+        elif y < 0:
+            y = 0
+        # apply the alpha channel
+        color = self.bgcolor_
+        if self.bgcolor != "transparent":
+            if self.alpha:
+                color = list(self.bgcolor_)
+                if len(color) == 4:
+                    color[3] = self.alpha
+                else:
+                    color += [self.alpha]
+        gc.save_state()
+        try:
+            gc.translate_ctm(x, y)
+
+            gc.set_line_width(self.border_size)
+            gc.set_stroke_color(self.border_color_)
+            gc.set_fill_color(color)
+
+            # draw a rounded rectangle
+            x = y = 0
+            end_radius = 8.0
+            gc.begin_path()
+            gc.move_to(x + end_radius, y)
+            gc.arc_to(x + width, y, x + width, y + end_radius, end_radius)
+            gc.arc_to(
+                x + width,
+                y + height,
+                x + width - end_radius,
+                y + height,
+                end_radius,
+            )
+            gc.arc_to(x, y + height, x, y, end_radius)
+            gc.arc_to(x, y, x + width + end_radius, y, end_radius)
+            gc.draw_path()
+
+            label.draw(gc)
+        finally:
+            gc.restore_state()
```

### Comparing `pyptv-0.2.2/pyptv.egg-info/SOURCES.txt` & `pyptv-0.2.3/pyptv.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -24,8 +24,10 @@
 pyptv/scatter_inspector2.py
 pyptv/text_box_overlay.py
 pyptv.egg-info/PKG-INFO
 pyptv.egg-info/SOURCES.txt
 pyptv.egg-info/dependency_links.txt
 pyptv.egg-info/entry_points.txt
 pyptv.egg-info/requires.txt
-pyptv.egg-info/top_level.txt
+pyptv.egg-info/top_level.txt
+tests/test_cli.py
+tests/test_pyptv_batch.py
```

### Comparing `pyptv-0.2.2/setup.py` & `pyptv-0.2.3/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-from setuptools import setup
-
-requirements = [
-    'chaco',
-    'enable',
-    'optv',
-    'PyQt5',
-    'scikit-image',
-    'Pygments',
-    'six',
-    'imagecodecs',
-    'flowtracks',
-    'pandas',
-    'tables',
-    'pyparsing',
-    'tqdm'
-]
-
-setup(
-    name='pyptv',
-    version='0.2.2',
-    description='Python GUI for the OpenPTV library `liboptv`',
-    author="Alex Liberzon",
-    author_email='alex.liberzon@gmail.com',
-    url='https://github.com/alexlib/pyptv',
-    packages=['pyptv'],
-    entry_points={
-        'console_scripts': [
-            'pyptv=pyptv.pyptv_gui:main'
-        ]
-    },
-    install_requires=requirements,
-    keywords='pyptv',
-    classifiers=[
-        'Programming Language :: Python :: 3'
-    ]
-)
+from setuptools import setup
+
+requirements = [
+    'chaco',
+    'enable',
+    'optv',
+    'PyQt5',
+    'scikit-image',
+    'Pygments',
+    'six',
+    'imagecodecs',
+    'flowtracks',
+    'pandas',
+    'tables',
+    'pyparsing',
+    'tqdm'
+]
+
+setup(
+    name='pyptv',
+    version='0.2.3',
+    description='Python GUI for the OpenPTV library `liboptv`',
+    author="Alex Liberzon",
+    author_email='alex.liberzon@gmail.com',
+    url='https://github.com/alexlib/pyptv',
+    packages=['pyptv'],
+    entry_points={
+        'console_scripts': [
+            'pyptv=pyptv.pyptv_gui:main'
+        ]
+    },
+    install_requires=requirements,
+    keywords='pyptv',
+    classifiers=[
+        'Programming Language :: Python :: 3'
+    ]
+)
```

