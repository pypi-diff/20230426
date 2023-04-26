# Comparing `tmp/toolplot-0.3.1.tar.gz` & `tmp/toolplot-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toolplot-0.3.1.tar", last modified: Tue Mar 21 20:34:27 2023, max compression
+gzip compressed data, was "toolplot-0.3.2.tar", last modified: Tue Apr 25 21:14:20 2023, max compression
```

## Comparing `toolplot-0.3.1.tar` & `toolplot-0.3.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0       58 2023-03-11 02:30:55.209013 toolplot-0.3.1/.gitignore
--rw-r--r--   0        0        0     1083 2023-03-11 02:30:55.209139 toolplot-0.3.1/LICENSE
--rw-r--r--   0        0        0      229 2023-03-11 02:30:55.209248 toolplot-0.3.1/README.md
--rw-r--r--   0        0        0      369 2023-03-11 02:30:55.209368 toolplot-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      215 2023-03-21 20:34:03.939078 toolplot-0.3.1/toolplot/__init__.py
--rw-r--r--   0        0        0     5176 2023-03-11 02:30:55.209682 toolplot-0.3.1/toolplot/plot_create.py
--rw-r--r--   0        0        0      140 2023-03-11 02:30:55.209793 toolplot-0.3.1/toolplot/plot_fonts.py
--rw-r--r--   0        0        0     1770 2023-03-11 02:30:55.209925 toolplot-0.3.1/toolplot/plot_save.py
--rw-r--r--   0        0        0      996 2023-03-11 02:30:55.210048 toolplot-0.3.1/toolplot/plot_setup.py
--rw-r--r--   0        0        0     2713 2023-03-11 02:30:55.210168 toolplot-0.3.1/toolplot/plot_ticks.py
--rw-r--r--   0        0        0       88 2023-03-11 02:33:48.174763 toolplot-0.3.1/toolplot/special_plots/__init__.py
--rw-r--r--   0        0        0      748 2023-03-11 02:30:55.210424 toolplot-0.3.1/toolplot/special_plots/bar_plots.py
--rw-r--r--   0        0        0     1279 2023-03-11 02:30:55.210531 toolplot-0.3.1/toolplot/special_plots/candlestick_plots.py
--rw-r--r--   0        0        0      618 2023-03-15 07:40:12.774167 toolplot-0.3.1/toolplot/special_plots/log_histograms.py
--rw-r--r--   0        0        0      567 1970-01-01 00:00:00.000000 toolplot-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0       58 2023-03-11 02:30:55.209013 toolplot-0.3.2/.gitignore
+-rw-r--r--   0        0        0     1083 2023-03-11 02:30:55.209139 toolplot-0.3.2/LICENSE
+-rw-r--r--   0        0        0      229 2023-03-11 02:30:55.209248 toolplot-0.3.2/README.md
+-rw-r--r--   0        0        0      369 2023-03-11 02:30:55.209368 toolplot-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      215 2023-04-25 21:13:33.311364 toolplot-0.3.2/toolplot/__init__.py
+-rw-r--r--   0        0        0     5176 2023-03-11 02:30:55.209682 toolplot-0.3.2/toolplot/plot_create.py
+-rw-r--r--   0        0        0      140 2023-03-11 02:30:55.209793 toolplot-0.3.2/toolplot/plot_fonts.py
+-rw-r--r--   0        0        0     1770 2023-03-11 02:30:55.209925 toolplot-0.3.2/toolplot/plot_save.py
+-rw-r--r--   0        0        0      996 2023-03-11 02:30:55.210048 toolplot-0.3.2/toolplot/plot_setup.py
+-rw-r--r--   0        0        0     3364 2023-04-25 21:12:12.432572 toolplot-0.3.2/toolplot/plot_ticks.py
+-rw-r--r--   0        0        0       88 2023-03-11 02:33:48.174763 toolplot-0.3.2/toolplot/special_plots/__init__.py
+-rw-r--r--   0        0        0      748 2023-03-11 02:30:55.210424 toolplot-0.3.2/toolplot/special_plots/bar_plots.py
+-rw-r--r--   0        0        0     1279 2023-03-11 02:30:55.210531 toolplot-0.3.2/toolplot/special_plots/candlestick_plots.py
+-rw-r--r--   0        0        0      618 2023-03-15 07:40:12.774167 toolplot-0.3.2/toolplot/special_plots/log_histograms.py
+-rw-r--r--   0        0        0      567 1970-01-01 00:00:00.000000 toolplot-0.3.2/PKG-INFO
```

### Comparing `toolplot-0.3.1/LICENSE` & `toolplot-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `toolplot-0.3.1/toolplot/plot_create.py` & `toolplot-0.3.2/toolplot/plot_create.py`

 * *Files identical despite different names*

### Comparing `toolplot-0.3.1/toolplot/plot_save.py` & `toolplot-0.3.2/toolplot/plot_save.py`

 * *Files identical despite different names*

### Comparing `toolplot-0.3.1/toolplot/plot_setup.py` & `toolplot-0.3.2/toolplot/plot_setup.py`

 * *Files identical despite different names*

### Comparing `toolplot-0.3.1/toolplot/plot_ticks.py` & `toolplot-0.3.2/toolplot/plot_ticks.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,38 @@
-import matplotlib
-import matplotlib.pyplot as plt
+from __future__ import annotations
+
+import matplotlib  # type: ignore
+import matplotlib.pyplot as plt  # type: ignore
 import toolstr
 
 
+def set_labels(
+    *,
+    title: str | None = None,
+    xlabel: str | None = None,
+    ylabel: str | None = None,
+    y_percentage: bool = False,
+    y_decimals: int | None = None,
+    x_decimals: int | None = None,
+) -> None:
+    if title is not None:
+        plt.title(title)
+    if xlabel is not None:
+        plt.xlabel(xlabel)
+    if ylabel is not None:
+        plt.ylabel(ylabel)
+    format_xticks()
+    if y_percentage:
+        toolstr_kwargs = {'percentage': True}
+    else:
+        toolstr_kwargs = {}
+    format_yticks(toolstr_kwargs=toolstr_kwargs)
+    add_tick_grid()
+
+
 def format_xticks(
     rotation=-25,
     timestamps=False,
     dates=False,
     toolstr_kwargs=None,
     xticks_kwargs=None,
     tickmap=None,
```

### Comparing `toolplot-0.3.1/toolplot/special_plots/bar_plots.py` & `toolplot-0.3.2/toolplot/special_plots/bar_plots.py`

 * *Files identical despite different names*

### Comparing `toolplot-0.3.1/toolplot/special_plots/candlestick_plots.py` & `toolplot-0.3.2/toolplot/special_plots/candlestick_plots.py`

 * *Files identical despite different names*

### Comparing `toolplot-0.3.1/toolplot/special_plots/log_histograms.py` & `toolplot-0.3.2/toolplot/special_plots/log_histograms.py`

 * *Files identical despite different names*

### Comparing `toolplot-0.3.1/PKG-INFO` & `toolplot-0.3.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toolplot
-Version: 0.3.1
+Version: 0.3.2
 Summary: toolplot is a alternative API to plotting backends
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: tooltime>=0.2.0
 Requires-Dist: toolstr>=0.4.0
 Requires-Dist: typing-extensions>=4.0.0
 Requires-Dist: matplotlib>=3.1
```

