# Comparing `tmp/trianglechain-0.2.0.tar.gz` & `tmp/trianglechain-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trianglechain-0.2.0.tar", last modified: Mon Feb 13 19:12:35 2023, max compression
+gzip compressed data, was "trianglechain-0.3.0.tar", last modified: Wed Apr 26 13:37:04 2023, max compression
```

## Comparing `trianglechain-0.2.0.tar` & `trianglechain-0.3.0.tar`

### file list

```diff
@@ -1,32 +1,36 @@
-drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-02-13 19:12:35.562574 trianglechain-0.2.0/
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)      201 2023-02-13 18:35:19.000000 trianglechain-0.2.0/AUTHORS.rst
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1708 2022-10-31 13:23:31.000000 trianglechain-0.2.0/CONTRIBUTING.rst
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)      467 2023-02-13 18:50:35.000000 trianglechain-0.2.0/HISTORY.rst
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1116 2022-10-31 13:32:05.000000 trianglechain-0.2.0/LICENSE
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)       99 2022-10-31 13:23:31.000000 trianglechain-0.2.0/MANIFEST.in
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     2424 2023-02-13 19:12:35.562663 trianglechain-0.2.0/PKG-INFO
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1571 2023-02-13 18:50:07.000000 trianglechain-0.2.0/README.md
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)      735 2022-10-31 13:23:31.000000 trianglechain-0.2.0/pyproject.toml
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1353 2023-02-13 19:12:35.563029 trianglechain-0.2.0/setup.cfg
-drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-02-13 19:12:35.556358 trianglechain-0.2.0/src/
-drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-02-13 19:12:35.560940 trianglechain-0.2.0/src/trianglechain/
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     7770 2023-02-13 18:36:37.000000 trianglechain-0.2.0/src/trianglechain/BaseChain.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     5575 2022-10-31 13:38:09.000000 trianglechain-0.2.0/src/trianglechain/LineChain.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     3741 2022-08-03 13:27:06.000000 trianglechain-0.2.0/src/trianglechain/TransformedGaussianMixture.py
--rwxr-xr-x   0 silvanfischbacher   (501) staff       (20)    21848 2023-02-09 14:27:31.000000 trianglechain-0.2.0/src/trianglechain/TriangleChain.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)      278 2023-02-09 14:31:43.000000 trianglechain-0.2.0/src/trianglechain/__init__.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     8960 2023-02-02 16:59:08.000000 trianglechain-0.2.0/src/trianglechain/bestfit.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     7532 2023-02-02 16:59:08.000000 trianglechain-0.2.0/src/trianglechain/density_estimation.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     2308 2023-02-02 16:59:08.000000 trianglechain-0.2.0/src/trianglechain/limits.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)    13686 2023-02-02 16:59:08.000000 trianglechain-0.2.0/src/trianglechain/make_subplots.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1378 2023-02-02 16:59:08.000000 trianglechain-0.2.0/src/trianglechain/utils_pj_hpd.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)    10521 2023-02-09 14:31:08.000000 trianglechain-0.2.0/src/trianglechain/utils_plots.py
-drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-02-13 19:12:35.562163 trianglechain-0.2.0/src/trianglechain.egg-info/
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     2424 2023-02-13 19:12:35.000000 trianglechain-0.2.0/src/trianglechain.egg-info/PKG-INFO
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)      741 2023-02-13 19:12:35.000000 trianglechain-0.2.0/src/trianglechain.egg-info/SOURCES.txt
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)        1 2023-02-13 19:12:35.000000 trianglechain-0.2.0/src/trianglechain.egg-info/dependency_links.txt
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)        1 2022-10-31 14:35:08.000000 trianglechain-0.2.0/src/trianglechain.egg-info/not-zip-safe
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)      278 2023-02-13 19:12:35.000000 trianglechain-0.2.0/src/trianglechain.egg-info/requires.txt
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)       14 2023-02-13 19:12:35.000000 trianglechain-0.2.0/src/trianglechain.egg-info/top_level.txt
-drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-02-13 19:12:35.562333 trianglechain-0.2.0/tests/
--rwxr-xr-x   0 silvanfischbacher   (501) staff       (20)     3976 2023-02-02 16:59:08.000000 trianglechain-0.2.0/tests/test_trianglechain.py
+drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-04-26 13:37:04.356767 trianglechain-0.3.0/
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)      201 2023-04-26 13:23:10.000000 trianglechain-0.3.0/AUTHORS.rst
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1708 2023-04-26 13:23:10.000000 trianglechain-0.3.0/CONTRIBUTING.rst
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1017 2023-04-26 13:36:31.000000 trianglechain-0.3.0/HISTORY.rst
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1116 2023-04-26 13:23:10.000000 trianglechain-0.3.0/LICENSE
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)       99 2023-04-26 13:23:10.000000 trianglechain-0.3.0/MANIFEST.in
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     2427 2023-04-26 13:37:04.356829 trianglechain-0.3.0/PKG-INFO
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1594 2023-04-26 13:23:10.000000 trianglechain-0.3.0/README.md
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)      735 2023-04-26 13:23:11.000000 trianglechain-0.3.0/pyproject.toml
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1385 2023-04-26 13:37:04.357221 trianglechain-0.3.0/setup.cfg
+drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-04-26 13:37:04.352516 trianglechain-0.3.0/src/
+drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-04-26 13:37:04.355096 trianglechain-0.3.0/src/trianglechain/
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     8714 2023-04-26 13:23:11.000000 trianglechain-0.3.0/src/trianglechain/BaseChain.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)    13478 2023-04-26 13:23:11.000000 trianglechain-0.3.0/src/trianglechain/LineChain.py
+-rwxr-xr-x   0 silvanfischbacher   (501) staff       (20)    27750 2023-04-26 13:23:11.000000 trianglechain-0.3.0/src/trianglechain/TriangleChain.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)      319 2023-04-26 13:36:45.000000 trianglechain-0.3.0/src/trianglechain/__init__.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)    13417 2023-04-26 13:23:11.000000 trianglechain-0.3.0/src/trianglechain/bestfit.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)    10416 2023-04-26 13:23:11.000000 trianglechain-0.3.0/src/trianglechain/density_estimation.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     7853 2023-04-26 13:23:11.000000 trianglechain-0.3.0/src/trianglechain/limits.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)    16438 2023-04-26 13:23:11.000000 trianglechain-0.3.0/src/trianglechain/make_subplots.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     4349 2023-04-26 13:23:11.000000 trianglechain-0.3.0/src/trianglechain/params.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     3024 2023-04-26 13:23:11.000000 trianglechain-0.3.0/src/trianglechain/utils_pj_hpd.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)    18937 2023-04-26 13:23:11.000000 trianglechain-0.3.0/src/trianglechain/utils_plots.py
+drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-04-26 13:37:04.356043 trianglechain-0.3.0/src/trianglechain.egg-info/
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     2427 2023-04-26 13:37:04.000000 trianglechain-0.3.0/src/trianglechain.egg-info/PKG-INFO
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)      809 2023-04-26 13:37:04.000000 trianglechain-0.3.0/src/trianglechain.egg-info/SOURCES.txt
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)        1 2023-04-26 13:37:04.000000 trianglechain-0.3.0/src/trianglechain.egg-info/dependency_links.txt
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)        1 2023-04-26 13:23:29.000000 trianglechain-0.3.0/src/trianglechain.egg-info/not-zip-safe
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)      308 2023-04-26 13:37:04.000000 trianglechain-0.3.0/src/trianglechain.egg-info/requires.txt
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)       14 2023-04-26 13:37:04.000000 trianglechain-0.3.0/src/trianglechain.egg-info/top_level.txt
+drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-04-26 13:37:04.356659 trianglechain-0.3.0/tests/
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)      674 2023-04-26 13:23:11.000000 trianglechain-0.3.0/tests/test_bestfit.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     2013 2023-04-26 13:23:11.000000 trianglechain-0.3.0/tests/test_limits.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)      748 2023-04-26 13:23:11.000000 trianglechain-0.3.0/tests/test_linechain.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     2897 2023-04-26 13:23:11.000000 trianglechain-0.3.0/tests/test_params.py
+-rwxr-xr-x   0 silvanfischbacher   (501) staff       (20)     4006 2023-04-26 13:23:11.000000 trianglechain-0.3.0/tests/test_trianglechain.py
```

### Comparing `trianglechain-0.2.0/CONTRIBUTING.rst` & `trianglechain-0.3.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `trianglechain-0.2.0/LICENSE` & `trianglechain-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trianglechain-0.2.0/PKG-INFO` & `trianglechain-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: trianglechain
-Version: 0.2.0
+Version: 0.3.0
 Summary: Code to plot multidimensional distributions
-Author: Tomasz Kacprzak, Silvan Fischbacher
-Author-email: tomaszk@phys.ethz.ch, silvanf@phys.ethz.ch
+Author: Silvan Fischbacher, Tomasz Kacprzak
+Author-email: silvanf@phys.ethz.ch, tomaszk@phys.ethz.ch
 License: MIT License
 Project-URL: Source, https://cosmo-docs.phys.ethz.ch/trianglechain
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -51,22 +50,20 @@
     cov=np.diag(np.ones(3)),
     size=(10000)
 )
 
 tri = TriangleChain()
 tri.contour_cl(samples);
 ```
-The input data can be (structured) arrays or dictionaries.
+The input data can be rec arrays, numpy array, pandas dataframes or dictionaries.
 For more example plots, see [demos](https://cosmo-gitlab.phys.ethz.ch/cosmo_public/trianglechain/demo)
 
 Credits
 -------
 
 This package was created by Tomasz Kacprzak and further developed and extended by Silvan Fischbacher.
 The package is maintained by Silvan Fischbacher: silvanf@phys.ethz.ch.
 
 Contributions
 -------------
 Contributions are welcome, and they are greatly appreciated! Every
 little bit helps, and credit will always be given.
-
-
```

### Comparing `trianglechain-0.2.0/README.md` & `trianglechain-0.3.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     cov=np.diag(np.ones(3)),
     size=(10000)
 )
 
 tri = TriangleChain()
 tri.contour_cl(samples);
 ```
-The input data can be (structured) arrays or dictionaries.
+The input data can be rec arrays, numpy array, pandas dataframes or dictionaries.
 For more example plots, see [demos](https://cosmo-gitlab.phys.ethz.ch/cosmo_public/trianglechain/demo)
 
 Credits
 -------
 
 This package was created by Tomasz Kacprzak and further developed and extended by Silvan Fischbacher.
 The package is maintained by Silvan Fischbacher: silvanf@phys.ethz.ch.
```

### Comparing `trianglechain-0.2.0/pyproject.toml` & `trianglechain-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `trianglechain-0.2.0/setup.cfg` & `trianglechain-0.3.0/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [metadata]
 name = trianglechain
 version = attr: trianglechain.__version__
 license = MIT License
 description = Code to plot multidimensional distributions
 long_description = file: README.md
 long_description_content_type = text/markdown
-author = Tomasz Kacprzak, Silvan Fischbacher
-author_email = tomaszk@phys.ethz.ch, silvanf@phys.ethz.ch
+author = Silvan Fischbacher, Tomasz Kacprzak
+author_email = silvanf@phys.ethz.ch, tomaszk@phys.ethz.ch
 classifiers = 
 	Intended Audience :: Science/Research
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Natural Language :: English
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.9
@@ -21,17 +21,18 @@
 
 [options]
 install_requires = 
 	numpy
 	matplotlib
 	scikit-learn
 	scipy
-	ekit
 	tqdm
 	arviz
+	pandas
+	cosmic_toolbox
 packages = find:
 package_dir = 
 	=src
 zip_safe = False
 python_requires = >=3.7
 
 [options.packages.find]
@@ -59,12 +60,13 @@
 	myst-parser
 docs = 
 	sphinx
 	sphinx-pynpoint-theme
 	myst-parser
 	nbsphinx
 	sphinx-copybutton
+	recommonmark
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `trianglechain-0.2.0/src/trianglechain/BaseChain.py` & `trianglechain-0.3.0/src/trianglechain/BaseChain.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,14 @@
+# Copyright (C) 2022 ETH Zurich
+# Institute for Particle Physics and Astrophysics
+# Author: Silvan Fischbacher, Tomasz Kacprzak
+
+
 from functools import partial
+import matplotlib.pyplot as plt
 
 
 class BaseChain:
     def __init__(self, fig=None, size=4, **kwargs):
         """
         :param fig: matplotlib figure to use
             default: None
@@ -53,14 +59,15 @@
                     use Gaussian mixture to fit the 2D samples
                 median_filter:
                     use median filter on the 2D histogram
                 kde:
                     use TreeKDE, may be slow
                 hist:
                     simple 2D histogram
+        :param line_space: space between lines in LineChain
         :param de_kwargs: density estimation kwargs, dictionary with keys:
             n_points:
                 number of bins for 2d histograms used to create contours, etc
                 default: n_bins
             levels:
                 density levels for contours, the contours will enclose this
                 level of probability
@@ -102,17 +109,14 @@
         tri.contour_cl(samples)  # plot contours at given confidence levels
         tri.density_image(samples)  # plot PDF density image
         tri.scatter(samples)  # simple scatter plot
         tri.scatter_prob(samples)  # scatter plot
                                    # with probability for each sample provided
         tri.scatter_density(samples) # scatter plot
                                      # color corresponds to probability
-
-
-
         """
 
         kwargs.setdefault("ticks", {})
         kwargs.setdefault("ranges", {})
         kwargs.setdefault("labels", None)
         kwargs.setdefault("n_bins", 100)
         kwargs.setdefault("de_kwargs", {})
@@ -128,14 +132,15 @@
         kwargs.setdefault("grid", False)
         kwargs.setdefault("scatter_kwargs", {})
         kwargs.setdefault("grouping_kwargs", {})
         kwargs.setdefault("subplots_kwargs", {})
         kwargs.setdefault("add_empty_plots_like", None)
         kwargs.setdefault("label_fontsize", 24)
         kwargs.setdefault("params", "all")
+        kwargs.setdefault("line_space", 0.5)
         kwargs.setdefault("orientation", "horizontal")
         kwargs.setdefault("normalize_prob1D", True)
         kwargs.setdefault("normalize_prob2D", True)
         kwargs.setdefault("progress_bar", True)
         kwargs["de_kwargs"].setdefault("n_points", kwargs["n_bins"])
         kwargs["de_kwargs"].setdefault("levels", [0.68, 0.95])
         kwargs["de_kwargs"].setdefault("n_levels_check", 2000)
@@ -160,18 +165,41 @@
         self.funcs = [
             "contour_cl",
             "density_image",
             "scatter",
             "scatter_prob",
             "scatter_density",
         ]
+        self.colors = []
 
     def add_plotting_functions(self, func_add_plot):
+        """
+        Add plotting functions to the class.
+
+        :param func_add_plot: function that adds a plot to the class
+        """
 
         for fname in self.funcs:
             f = partial(func_add_plot, plottype=fname)
             doc = (
                 "This function is equivalent to add_plot with \n"
                 f"plottype={fname} \n" + func_add_plot.__doc__
             )
             f.__doc__ = doc
             setattr(self, fname, f)
+
+    def setup_color(self, color):
+        """
+        Setup color for plotting. If color is None, find next color in cycle.
+
+        :param color: color for plotting
+        :return: color
+        """
+
+        if color is None:
+            # find automatic next color
+            pos_in_cycle = len(self.colors)
+            colors = plt.rcParams["axes.prop_cycle"].by_key()["color"]
+            self.colors.append(colors)
+            return colors[pos_in_cycle % len(colors)]
+        else:
+            return color
```

### Comparing `trianglechain-0.2.0/src/trianglechain/TriangleChain.py` & `trianglechain-0.3.0/src/trianglechain/TriangleChain.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,78 +1,85 @@
+# Copyright (C) 2022 ETH Zurich
+# Institute for Particle Physics and Astrophysics
+# Author: Tomasz Kacprzak, Silvan Fischbacher
+
 import matplotlib.pyplot as plt
 import numpy as np
 import matplotlib as mpl
 from trianglechain.utils_plots import (
     prepare_columns,
     setup_grouping,
     get_labels,
     get_hw_ratios,
     setup_figure,
     update_current_ranges,
     update_current_ticks,
     set_limits,
     delete_all_ticks,
     add_vline,
-    ensure_rec,
     get_old_lims,
     get_best_old_lims,
     find_alpha,
+    get_lines_and_labels,
 )
+from trianglechain.params import ensure_rec
 from trianglechain.make_subplots import (
     contour_cl,
     density_image,
     scatter_density,
     plot_1d,
 )
 from trianglechain.BaseChain import BaseChain
 from tqdm.auto import tqdm, trange
 
-from ekit import logger as logger_utils
+from cosmic_toolbox.logger import get_logger
 
-LOGGER = logger_utils.init_logger(__name__)
+LOGGER = get_logger(__file__)
 
 
 class TriangleChain(BaseChain):
-    def __init__(self, fig=None, size=4, **kwargs):
+    """
+    Class to produce triangle plots of chains.
+    """
 
+    def __init__(self, fig=None, size=4, **kwargs):
         super().__init__(fig=fig, size=size, **kwargs)
 
         self.add_plotting_functions(self.add_plot)
 
     def add_plot(
         self,
         data,
         plottype,
         prob=None,
-        color="b",
-        cmap=plt.cm.plasma,
+        color=None,
+        cmap=plt.cm.viridis,
         tri="lower",
         plot_histograms_1D=True,
         **kwargs,
     ):
         """
-        :param data: numpy struct array
+        :param data: rec array
             the data that should be plotted with column data
         :param plottype: {"contour_cl", "density_image", "scatter",
             "scatter_density", "scatter_prob"}
             type of plot that should be plotted
         :param prob: None or array
             if not None, then probability attached to the samples,
             in that case samples are treated as grid not a chain
             default: None
         :param color: matplotlib color
-            color of the plot, default="b"
+            color of the plot, default=None (automatic)
         :param cmap: matplotlib colormap
-            colormap used for this plot, default="plasma"
+            colormap used for this plot, default="viridis"
         :param tri: {"lower", "upper"}
             if triangle should be in the upper or lower part, default="lower"
         :param plot_histograms_1D: boolean
             if the 1D histograms should be plotted as well, default=True
-
-        kwargs include the following parameters:
+        :param kwargs: additional arguments for the plotting functions, they include:
         :param cmap_vmin: fixed minimum in the colormap, default: 0
         :param cmap_vmax: fixed maximum of the colormap, default: None
         :param colorbar: if colorbar should be plotted, default: False
         :param colorbar_label: label of the colorbar, default: None
         :param colorbar_ax: position of colorbar
             default: [0.735, 0.5, 0.03, 0.25]
         :param show_values: if best-fit and uncertainty should be plotted
@@ -102,14 +109,18 @@
         """
 
         from copy import deepcopy
 
         kwargs_copy = deepcopy(self.kwargs)
         kwargs_copy.update(kwargs)
 
+        color = self.setup_color(color)
+        if (plottype == "scatter_prob") & (prob is None):
+            raise ValueError("prob needs to be defined for scatter_prob")
+
         self.fig, self.ax = plot_triangle_marginals(
             fig=self.fig,
             size=self.size,
             func=plottype,
             cmap=cmap,
             data=data,
             prob=prob,
@@ -121,19 +132,21 @@
         return self.fig, self.ax
 
 
 def plot_triangle_marginals(
     data,
     prob=None,
     params="all",
+    params_from=None,
+    names=None,
     func="contour_cl",
     tri="lower",
     single_tri=True,
-    color="b",
-    cmap=plt.cm.plasma,
+    color="#0063B9",
+    cmap=plt.cm.viridis,
     cmap_vmin=0,
     cmap_vmax=None,
     ranges={},
     ticks={},
     n_bins=20,
     fig=None,
     size=4,
@@ -171,23 +184,145 @@
     colorbar_label=None,
     colorbar_ax=[0.735, 0.5, 0.03, 0.25],
     normalize_prob1D=True,
     normalize_prob2D=True,
     progress_bar=True,
     **kwargs,
 ):
+    """
+    Plot a triangle plot with marginal distributions.
+
+    :param data: rec array
+        the data that should be plotted with column data
+    :param prob: None or array
+        probability attached to the samples, if None, then the density is estimated
+        from the samples, default: None
+    :param params: list of strings
+        list of parameters that should be plotted, default: "all"
+    :param params_from: data like array
+        if params is "all", then the parameters are taken from this array
+        default: None
+    :param names: list
+        list of names for the parameters in case data is np.ndarray, default: None
+    :param func: string
+        function that should be used for plotting,
+        options: "contour_cl", "density_image", "scatter", "scatter_prob", "scatter_density"
+        default: "contour_cl"
+    :param tri: string
+        if the upper or lower triangle should be plotted
+        options: "upper", "lower", default: "lower"
+    :param single_tri: bool
+        if only one triangle should be plotted, default: True
+    :param color: string
+        color of the plot, default: "#0063B9"
+    :param cmap: matplotlib colormap
+        colormap for the density plots, default: plt.cm.viridis
+    :param cmap_vmin: float
+        minimum value for the colormap, default: 0
+    :param cmap_vmax: float
+        maximum value for the colormap, default: None
+    :param ranges: dict
+        dictionary with ranges for the parameters, default: {}
+    :param ticks: dict
+        dictionary with ticks for the parameters, default: {}
+    :param n_bins: int
+        number of bins for the histograms, default: 20
+    :param fig: matplotlib figure
+        figure that should be used for plotting, default: None
+    :param size: float
+        size of the plot, default: 4
+    :param fill: bool
+        if the contours should be filled, default: True
+    :param grid: bool
+        if the grid should be plotted, default: False
+    :param labels: list of strings
+        labels for the parameters, default: None
+    :param plot_histograms_1D: bool
+        if the 1D histograms should be plotted, default: True
+    :param show_values: bool
+        if the values should be shown in the 1D histograms, default: False
+    :param bestfit_method: string
+        method that should be used for the bestfit value
+        options: "mode", "median", "mean", default: "mode"
+    :param levels_method: string
+        method that should be used for the levels
+        options: "hdi", "credible_interval", default: "hdi"
+    :param credible_interval: float
+        credible interval for the levels, default: 0.68
+    :param lnprobs: None or array
+        log probabilities attached to the samples for the level estimation,
+        default: None
+    :param scatter_vline_1D: bool
+        if a vertical line should be plotted at the scatter points in the 1D histograms,
+        default: False
+    :param label: string
+        label for the legend, default: None
+    :param density_estimation_method: method to use for density estimation
+        options: smoothing, histo, kde, gaussian_mixture, median_filter
+        default: smoothing
+    :param n_ticks: int
+        number of ticks for the axes, default: 3
+    :param tick_length: float
+        length of the ticks, default: 3
+    :param alpha1D: float
+        alpha value for the 1D histograms, default: 1
+    :param alpha2D: float
+        alpha value for the 2D histograms, default: 1
+    :param alpha_for_low_density: bool
+        if the alpha value should be adjusted for low density regions, default: False
+    :param alpha_threshold: float
+        threshold for the alpha value, default: 0
+    :param subplots_kwargs: dict
+        keyword arguments for the subplots function, default: {}
+    :param de_kwargs: dict
+        keyword arguments for the density estimation, default: {}
+    :param hist_kwargs: dict
+        keyword arguments for the histogram, default: {}
+    :param line_kwargs: dict
+        keyword arguments for the lines, default: {}
+    :param labels_kwargs: dict
+        keyword arguments for the labels, default: {}
+    :param grid_kwargs: dict
+        keyword arguments for the grid, default: {}
+    :param scatter_kwargs: dict
+        keyword arguments for the scatter plot, default: {}
+    :param grouping_kwargs: dict
+        keyword arguments for the grouping, default: {}
+    :param axvline_kwargs: dict
+        keyword arguments for the vertical lines, default: {}
+    :param add_empty_plots_like: string
+        DEPRECATED, default: None
+    :param label_fontsize: int
+        fontsize for the labels, default: 12
+    :param show_legend: bool
+        if the legend should be shown, default: False
+    :param colorbar: bool
+        if the colorbar should be shown, default: False
+    :param colorbar_label: string
+        label for the colorbar, default: None
+    :param colorbar_ax: list
+        position of the colorbar, default: [0.735, 0.5, 0.03, 0.25]
+    :param normalize_prob1D: bool
+        if the 1D probability should be normalized, default: True
+    :param normalize_prob2D: bool
+        if the 2D probability should be normalized, default: True
+    :param progress_bar: bool
+        if a progress bar should be shown, default: True
+    """
 
     ###############################
     # prepare data and setup plot #
     ###############################
-    data = ensure_rec(data)
+    data = ensure_rec(data, names=names)
     data, columns, empty_columns = prepare_columns(
-        data, params=params, add_empty_plots_like=add_empty_plots_like
+        data,
+        params=params,
+        params_from=params_from,
+        add_empty_plots_like=add_empty_plots_like,
     )
-
     # needed for plotting chains with different automatic limits
     current_ranges = {}
     current_ticks = {}
 
     # setup everything that grouping works properly
     columns, grouping_indices = setup_grouping(columns, grouping_kwargs)
     labels = get_labels(labels, columns, grouping_indices)
@@ -246,15 +381,14 @@
 
     if len(color) == len(data):
         color_hist = "k"
     else:
         color_hist = color
 
     def get_current_ax(ax, tri, i, j):
-
         if tri[0] == "u":
             if single_tri:
                 axc = ax[i, j]
             else:
                 axc = ax[i, j + 1]
         elif tri[0] == "l":
             if single_tri:
@@ -312,29 +446,35 @@
             if columns[i] != "EMPTY":
                 axc = get_current_ax(ax, tri, i, i)
                 add_vline(axc, columns[i], data, color, axvline_kwargs)
 
     #################
     # 2D histograms #
     #################
-    for i, j in tqdm(zip(*tri_indices), total=len(tri_indices[0]), disable=not progress_bar):
-        if columns[i] != "EMPTY" and columns[j] != "EMPTY":
+    for i, j in tqdm(
+        zip(*tri_indices), total=len(tri_indices[0]), disable=not progress_bar
+    ):
+        if (columns[i] != "EMPTY") & (columns[j] != "EMPTY"):
             axc = get_current_ax(ax, tri, i, j)
             old_xlims, old_ylims = get_old_lims(axc)
             if double_tri:
                 if tri == "lower":
                     other_tri = "upper"
                 else:
                     other_tri = "lower"
                 axc_mirror = get_current_ax(ax, other_tri, j, i)
                 old_xlims_mirror, old_ylims_mirror = get_old_lims(axc_mirror)
                 old_xlims, old_ylims = get_best_old_lims(
                     old_xlims, old_ylims_mirror, old_ylims, old_xlims_mirror
                 )
-            if func == "contour_cl":
+            if (columns[i] not in data.dtype.names) | (
+                columns[j] not in data.dtype.names
+            ):
+                pass
+            elif func == "contour_cl":
                 contour_cl(
                     axc,
                     data=data,
                     ranges=current_ranges,
                     columns=columns,
                     i=i,
                     j=j,
@@ -348,15 +488,15 @@
                     alpha=min(
                         (
                             find_alpha(columns[i], empty_columns, alpha2D),
                             find_alpha(columns[j], empty_columns, alpha2D),
                         )
                     ),
                 )
-            if func == "density_image":
+            elif func == "density_image":
                 density_image(
                     axc,
                     data=data,
                     ranges=current_ranges,
                     columns=columns,
                     i=i,
                     j=j,
@@ -426,15 +566,14 @@
                     ranges,
                     current_ranges,
                     columns[j],
                     columns[i],
                     old_ylims,
                     old_xlims,
                 )
-
     #########
     # ticks #
     #########
 
     def get_ticks(i):
         try:
             return ticks[columns[i]]
@@ -450,15 +589,14 @@
         if i != j:
             axc.xaxis.set_ticks_position("both")
         axc.set_xticks(get_ticks(j))
         axc.tick_params(direction=direction, length=length)
 
     delete_all_ticks(ax)
     update_current_ticks(current_ticks, columns, ranges, current_ranges, n_ticks)
-
     if tri[0] == "l" or double_tri:
         local_tri = "lower"
         for i in range(1, n_dim):  # rows
             for j in range(0, i):  # columns
                 if columns[i] != "EMPTY" and columns[j] != "EMPTY":
                     axc = get_current_ax(ax, local_tri, i, j)
                     plot_yticks(axc, i, tick_length)
@@ -479,15 +617,14 @@
             for j in range(i, n_dim):  # columns
                 if columns[i] != "EMPTY" and columns[j] != "EMPTY":
                     axc = get_current_ax(ax, local_tri, i, j)
                     plot_xticks(axc, i, j, tick_length)
 
     # ticklabels
     def plot_tick_labels(axc, xy, i, tri, grid_kwargs):
-        # ticklabels = [fmt_e(t) for t in get_ticks(i)]
         ticklabels = [t for t in get_ticks(i)]
         if xy == "y":
             axc.set_yticklabels(
                 ticklabels,
                 rotation=0,
                 fontsize=grid_kwargs["fontsize_ticklabels"],
                 family=grid_kwargs["font_family"],
@@ -552,15 +689,15 @@
                     if grid:
                         axc.grid(zorder=0, linestyle="--")
                     axc.set_axisbelow(True)
 
     ###########
     # legends #
     ###########
-    legend_lines, legend_labels = ax[0, 0].get_legend_handles_labels()
+    legend_lines, legend_labels = get_lines_and_labels(ax)
     if tri[0] == "l":
         labelpad = 10
         for i in range(n_dim):
             if columns[i] != "EMPTY":
                 axc = get_current_ax(ax, tri, i, 0)
 
                 axc.set_ylabel(
```

### Comparing `trianglechain-0.2.0/src/trianglechain/density_estimation.py` & `trianglechain-0.3.0/src/trianglechain/density_estimation.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# Copyright (C) 2022 ETH Zurich
+# Institute for Particle Physics and Astrophysics
+# Author: Tomasz Kacprzak, Silvan Fischbacher
+
+
 import numpy as np
 import scipy
 import warnings
 from trianglechain.utils_plots import (
     safe_normalise,
     normalise,
     pixel_coords,
@@ -14,26 +19,45 @@
     binedges,
     bincenters,
     lims,
     prob=None,
     method="smoothing",
     de_kwargs={},
 ):
+    """
+    Get density estimation for 1D data
 
-    if method == "gaussian_mixture":
+    :param data: data to estimate density from
+    :param binedges: bin edges for the histogram
+    :param bincenters: bin centers for the histogram
+    :param lims: limits for the histogram
+    :param prob: weights for the data
+    :param method: Method for density estimation. Valid options are:
+        - 'smoothing': First create a histogram of samples, and then smooth it
+        with a Gaussian kernel corresponding to the variance of the 20% of the
+        smallest eigenvalue of the 2D distribution (smoothing scale can be adapted
+        using the smoothing_scale parameter).
+        - 'gaussian_mixture': Fit a Gaussian mixture model to the data.
+        - 'median_filter': Use a median filter to smooth the histogram.
+        - 'kde': Use a kernel density estimation to estimate the density.
+        - 'hist': Use a histogram to estimate the density.
+    :param de_kwargs: keyword arguments for the density estimation method
+    :return: density estimation
+    """
 
+    if method == "gaussian_mixture":
         if prob is not None:
             ind = np.random.choice(
                 a=len(prob), size=10000, p=safe_normalise(prob), replace=True
             )
             data_ = data[ind][:, np.newaxis]
         else:
             data_ = data[:, np.newaxis]
 
-        from trianglechain.TransformedGaussianMixture import (
+        from cosmic_toolbox.TransformedGaussianMixture import (
             TransformedGaussianMixture,
         )
 
         clf = TransformedGaussianMixture(
             param_bounds=[lims], n_components=20, covariance_type="full"
         )
         clf.fit(data_)
@@ -47,15 +71,15 @@
         from scipy import ndimage
 
         prob1D = histogram_1D(data=data, prob=prob, binedges=binedges)
         data_pixel = pixel_coords(
             data, [[binedges[0], binedges[-1]]], n_pix_img=len(bincenters)
         )
         if prob is not None:
-            ind = np.random.choice(prob1D.shape[0], p=prob1D, size=1000)
+            ind = np.random.choice(prob.shape[0], p=prob, size=1000)
             data_pixel = data_pixel[0, ind]
 
         sig_pix = (
             get_smoothing_sigma(data_pixel, prob1D.shape[0])
             * de_kwargs["smoothing_parameter1D"]
         )
         n_pix = max(3, int(np.ceil(sig_pix * 10)))  # 10 sigma smoothing
@@ -63,45 +87,47 @@
         de = scipy.ndimage.convolve(prob1D, kernel, mode="reflect")
         de = normalise(de, bincenters)
 
         # de = np.convolve(a=prob1D, v=np.ones(5), mode='same')
         # de = signal.convolve2d(prob2d, kernel, mode='same', boundary='wrap')
 
     elif method == "median_filter":
-
         from scipy import ndimage
 
         prob1D = histogram_1D(data=data, prob=prob, binedges=binedges)
         de = ndimage.median_filter(prob1D, int(prob1D.shape[0] / 10))
 
     elif method == "kde":
-
         from KDEpy import TreeKDE
 
         de = TreeKDE(kernel="gaussian", bw="ISJ").fit(data).evaluate(bincenters)
 
     elif method == "hist":
-
         de = histogram_1D(data=data, prob=prob, binedges=binedges)
 
     else:
-
         raise Exception("unknown density estimation method {}".format(method))
 
     return de
 
 
 def histogram_1D(data, prob, binedges):
+    """
+    Create a histogram of the data
 
-    if prob is None:
+    :param data: data to create histogram from
+    :param prob: weights for the data
+    :param binedges: bin edges for the histogram
+    :return: histogram
+    """
 
+    if prob is None:
         prob1D, _ = np.histogram(data, bins=binedges)
 
     else:
-
         assert prob.shape[0] == data.shape[0]
 
         hist_counts, _ = np.histogram(data, bins=binedges)
         hist_prob, _ = np.histogram(data, bins=binedges, weights=prob)
         prob1D = hist_prob / hist_counts.astype(float)
         prob1D[hist_counts == 0] = 0
 
@@ -109,51 +135,70 @@
     prob1D = np.ma.array(prob1D, mask=prob1D == 0)
     return prob1D
 
 
 def get_density_grid_2D(
     data, ranges, columns, i, j, prob=None, method="smoothing", de_kwargs={}
 ):
+    """
+    Get density estimation for 2D data
+
+    :param data: data to estimate density from
+    :param ranges: ranges for the data
+    :param columns: columns to use for the data
+    :param i: index of the first column
+    :param j: index of the second column
+    :param prob: weights for the data
+    :param method: Method for density estimation. Valid options are:
+        - 'smoothing': First create a histogram of samples, and then smooth it
+        with a Gaussian kernel corresponding to the variance of the 20% of the
+        smallest eigenvalue of the 2D distribution (smoothing scale can be adapted
+        using the smoothing_scale parameter).
+        - 'gaussian_mixture': Fit a Gaussian mixture model to the data.
+        - 'median_filter': Use a median filter to smooth the histogram.
+        - 'kde': Use a kernel density estimation to estimate the density.
+        - 'hist': Use a histogram to estimate the density.
+    :param de_kwargs: keyword arguments for the density estimation method
+    :return: density estimation
+    """
 
     data_panel = np.vstack((data[columns[j]], data[columns[i]]))
     x_ls = np.linspace(*ranges[columns[j]], num=de_kwargs["n_points"])
     y_ls = np.linspace(*ranges[columns[i]], num=de_kwargs["n_points"])
     x_grid, y_grid = np.meshgrid(x_ls, y_ls)
     gridpoints = np.vstack([x_grid.ravel(), y_grid.ravel()])
     bins_x = np.linspace(x_ls[0], x_ls[-1], num=de_kwargs["n_points"] + 1)
     bins_y = np.linspace(y_ls[0], y_ls[-1], num=de_kwargs["n_points"] + 1)
     bins_x_centers = (bins_x[1:] + bins_x[:-1]) / 2.0
     bins_y_centers = (bins_y[1:] + bins_y[:-1]) / 2.0
     x_grid_centers, y_grid_centers = np.meshgrid(bins_x_centers, bins_y_centers)
 
     if method == "gaussian_mixture":
-
         if prob is not None:
             ind = np.random.choice(
                 a=len(prob), size=10000, p=safe_normalise(prob), replace=True
             )
             data_panel = data_panel[:, ind]
 
         bounds = [ranges[columns[j]], ranges[columns[i]]]
 
-        from trianglechain.TransformedGaussianMixture import (
+        from cosmic_toolbox.TransformedGaussianMixture import (
             TransformedGaussianMixture,
         )
 
         clf = TransformedGaussianMixture(
             param_bounds=bounds, n_components=10, covariance_type="full"
         )
         clf.fit(data_panel.T)
         logL = clf.score_samples(gridpoints.T)
 
         de = np.exp(logL - np.max(logL)).reshape(x_grid.shape)
         de = safe_normalise(de)
 
     elif method == "smoothing":
-
         prob2d = histogram_2D(data_panel, prob, bins_x, bins_y)
         prob2d = safe_normalise(prob2d)
 
         data_panel_pixel = pixel_coords(
             data_panel,
             [ranges[columns[j]], ranges[columns[i]]],
             n_pix_img=de_kwargs["n_points"],
@@ -168,56 +213,59 @@
         n_pix = int(np.ceil(sig_pix * 5))
 
         from scipy.ndimage import gaussian_filter
 
         de = gaussian_filter(prob2d, sigma=sig_pix)
 
     elif method == "median_filter":
-
         from scipy import ndimage
 
         prob2d = histogram_2D(data_panel, prob, bins_x, bins_y)
         prob2d = safe_normalise(prob2d)
         n_pix = int(prob2d.shape[0] / 5)
         de = ndimage.median_filter(prob2d, n_pix)
 
     elif method == "kde":
-
         from KDEpy import TreeKDE
 
         de = (
             TreeKDE(kernel="gaussian")
             .fit(data_panel.T)
             .evaluate(gridpoints.T)
             .reshape(x_grid.shape)
         )
 
     elif method == "hist":
-
         de = histogram_2D(data_panel, prob, bins_x, bins_y)
 
     else:
-
         raise Exception("unknown density estimation method {}".format(method))
 
     de[~np.isfinite(de)] = 0
     de = safe_normalise(de)
     return de, x_grid_centers, y_grid_centers
 
 
 def histogram_2D(data_panel, prob, bins_x, bins_y):
+    """
+    Create a 2D histogram
 
-    if prob is None:
+    :param data_panel: data to create histogram from
+    :param prob: weights for the data
+    :param bins_x: bins for the first dimension
+    :param bins_y: bins for the second dimension
+    :return: 2D histogram
+    """
 
+    if prob is None:
         prob2d = np.histogram2d(*data_panel, bins=(bins_x, bins_y))[0].T.astype(
             np.float32
         )
 
     else:
-
         assert prob.shape[0] == data_panel[0].shape[0]
 
         hist2d_counts = np.histogram2d(*data_panel, bins=(bins_x, bins_y))[0].T.astype(
             np.float32
         )
         hist2d_prob = np.histogram2d(*data_panel, weights=prob, bins=(bins_x, bins_y))[
             0
@@ -230,14 +278,22 @@
     if np.sum(prob2d) > 0:
         prob2d = prob2d / np.sum(prob2d)
 
     return prob2d
 
 
 def get_confidence_levels(de, levels, n_levels_check):
+    """
+    Get the confidence levels for a given density estimation
+
+    :param de: density estimation
+    :param levels: confidence levels
+    :param n_levels_check: number of levels to check
+    :return: confidence levels
+    """
 
     lvl_max = 0.99
     levels_check = np.linspace(0, np.amax(de) * lvl_max, n_levels_check)
     frac_levels = np.zeros_like(levels_check)
 
     for il, vl in enumerate(levels_check):
         pixels_above_level = de > vl
```

### Comparing `trianglechain-0.2.0/src/trianglechain/make_subplots.py` & `trianglechain-0.3.0/src/trianglechain/make_subplots.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,24 @@
+# Copyright (C) 2022 ETH Zurich
+# Institute for Particle Physics and Astrophysics
+# Author: Tomasz Kacprzak, Silvan Fischbacher
+
 import matplotlib.pyplot as plt
 import numpy as np
 from trianglechain.density_estimation import (
     get_density_grid_1D,
     get_density_grid_2D,
     get_confidence_levels,
 )
 from trianglechain.utils_plots import (
     get_old_lims,
     find_alpha,
     get_values,
     get_best_lims,
+    compute_plot_limits,
 )
 from matplotlib.colors import ListedColormap
 import matplotlib
 import warnings
 
 
 def plot_1d(
@@ -38,76 +43,82 @@
     lnprobs=None,
     levels_method="hdi",
     bestfit_method="mean",
     credible_interval=0.68,
     label_fontsize=12,
 ):
     """
-    axc : matplotlib axis
+    Plot 1D histogram and density estimation.
+
+    :param axc: matplotlib axis
         axis of the plot
-    column : str
+    :param column: str
         name of the parameter in data that is plotted
-    param_label : str
+    :param param_label: str
         name of the parameter that should be plotted in case
         bestfit and uncertainty are shown
-    data : numpy struct array
+    :param data: numpy struct array
         the data that should be plotted with column data
-    prob : None or array
+    :param prob: None or array
         if not None, then probability attached to the samples,
         in that case samples are treated as grid not a chain
-    ranges : dict
+    :param ranges: dict
         dictionary with the ranges of of the plot for each parameter
-    current_ranges : dict
+    :param current_ranges: dict
         dictionary with the current ranges of of the plot for each parameter
-    hist_binedges : array
+    :param hist_binedges: array
         edges of the histogram for the plot
-    hist_bincenters : array
+    :param hist_bincenters: array
         centers of the histogram for the plot
-    de_kwargs : dict
+    :param de_kwargs: dict
         additional kwargs for density estimation, passed to get_density_grid
-    hist_kwargs : dict
+    :param hist_kwargs: dict
         additional kwargs for the histogram plot, passed to plt.plot()
-    empty_columns : list
+    :param empty_columns: list
         list with the indices of empty columns
-    show_values : bool
+    :param show_values: bool
         if values of bestfit and uncertainty should be plotted
-    label : str
+    :param label: str
         label of the plot
-    density_estimation_method : {"gaussian_mixture", "smoothing",
+    :param density_estimation_method: {"gaussian_mixture", "smoothing",
         "median_filter", "kde", "hist"}
         method how to estimate the density
-    color_hist : color
+    :param color_hist: color
         color of the histogram
-    alpha1D : float in [0, 1]
+    :param alpha1D: float in [0, 1]
         alpha value of the histogram
-    fill : bool
+    :param fill: bool
         use filled histograms
-    lnprobs : array
+    :param lnprobs: array
         logprobabilites used for the bestfit and uncertainty finding
-    levels_method : {"hdi", "percentile", "PJ_HPD"}
+    :param levels_method: {"hdi", "percentile", "PJ_HPD"}
         method how to compute the uncertainty
-    bestfit_method : {"mode", "mean", "median", "best_sample"}
+    :param bestfit_method: {"mode", "mean", "median", "best_sample"}
         method how to compute the bestfit
-    credible_interval : float in [0, 1]
+    :param credible_interval: float in [0, 1]
         credible interval of the uncertainty bar
-    label_fontsize : int or float
+    :param label_fontsize: int or float
         fontsize of the label of the parameters
     """
+
+    try:
+        d = data[column]
+    except Exception:
+        return
+
     prob1D = get_density_grid_1D(
-        data=data[column],
+        data=d,
         prob=prob,
         lims=current_ranges[column],
         binedges=hist_binedges[column],
         bincenters=hist_bincenters[column],
         method=density_estimation_method,
         de_kwargs=de_kwargs,
     )
-
     old_xlims, old_ylims = get_old_lims(axc)
-    axc.autoscale()
     axc.plot(
         hist_bincenters[column],
         prob1D,
         "-",
         color=color_hist,
         alpha=find_alpha(column, empty_columns, alpha1D),
         label=label,
@@ -126,16 +137,18 @@
     except Exception:
         xlims = get_best_lims(
             current_ranges[column],
             current_ranges[column],
             old_xlims,
             old_ylims,
         )[0]
-    axc.set_xlim(xlims)
-    axc.set_ylim(0, max(old_ylims[1], axc.get_ylim()[1]))
+    if np.isfinite(xlims[0]):
+        axc.set_xlim(xlims)
+    new_ylim = compute_plot_limits(prob1D)[1]
+    axc.set_ylim(0, np.nanmax([old_ylims[1], new_ylim]))
     if show_values:
         add_values(
             axc,
             column,
             data,
             lnprobs,
             label=param_label,
@@ -153,79 +166,119 @@
     lnprobs,
     label,
     levels_method="hdi",
     bestfit_method="mean",
     credible_interval=0.68,
     label_fontsize=12,
 ):
-    str_bf, up, low = get_values(
+    """
+    Add values of bestfit and uncertainty to the plot.
+
+    :param axc: matplotlib axis
+        axis of the plot
+    :param column: str
+        name of the parameter in data that is plotted
+    :param data: numpy struct array
+        the data that should be plotted with column data
+    :param lnprobs: array
+        logprobabilites used for the bestfit and uncertainty finding
+    :param label: str
+        label of the plot
+    :param levels_method: {"hdi", "percentile", "PJ_HPD"}
+        method how to compute the uncertainty, default is hdi
+    :param bestfit_method: {"mode", "mean", "median", "best_sample"}
+        method how to compute the bestfit, default is mean
+    :param credible_interval: float in [0, 1]
+        credible interval of the uncertainty bar, default is 0.68
+    :param label_fontsize: int or float
+        fontsize of the label of the parameters, default is 12
+    """
+    two_tail, str_bf, up, low = get_values(
         column,
         data,
         lnprobs,
         levels_method=levels_method,
         bestfit_method=bestfit_method,
         credible_interval=credible_interval,
     )
-    axc.set_title(
-        r"{} $= {}^{{+{} }}_{{-{} }}$".format(label, str_bf, up, low),
-        fontsize=label_fontsize,
-    )
+    if two_tail:
+        axc.set_title(
+            r"{} $= {}^{{+{} }}_{{-{} }}$".format(label, str_bf, up, low),
+            fontsize=label_fontsize,
+        )
+    else:
+        side = str_bf
+        limit = up
+        if side[0] == "l":
+            axc.set_title(
+                r"{} $> {}$".format(label, limit),
+                fontsize=label_fontsize,
+            )
+        else:
+            axc.set_title(
+                r"{} $< {}$".format(label, limit),
+                fontsize=label_fontsize,
+            )
 
 
 def density_image(
     axc,
     data,
     ranges,
     columns,
     i,
     j,
     cmap,
-    de_kwargs,
+    de_kwargs={},
     vmin=0,
     vmax=None,
     prob=None,
     density_estimation_method="smoothing",
     label=None,
     alpha_for_low_density=False,
     alpha_threshold=0,
 ):
     """
-    axc : matplotlib axis
+    Plot the density of the data in the given axis as a density image.
+
+    :param axc: matplotlib axis
         axis of the plot
-    data : numpy struct array
+    :param data: numpy struct array
         the data that should be plotted with column data
-    ranges : dict
+    :param ranges: dict
         dictionary with the ranges of of the plot for each parameter
-    columns : list
+    :param columns: list
         list of all parameters
-    i, j : int
-        index of pair of columns to plot
-    cmap : matplotlib colormap
+    :param i: int
+        index of the first column to plot
+    :param j: int
+        index of the second column to plot
+    :param cmap: matplotlib colormap
         colormap that is used
-    de_kwargs : dict
+    :param de_kwargs: dict
         dict with kde settings, has to have n_points, n_levels_check, levels
-    vmin : None or float
+    :param vmin: None or float
         minimum value for the density (default=0)
-        if None, the minimu in each subplot will be chosen as vmin
-    vmax : float
+        if None, the minimum in each subplot will be chosen as vmin
+    :param vmax: float
         maximum value for the density (default=None),
-        if None, the maxmîmum in each subplot will be chosen as vmax
-    prob : None or array
+        if None, the maximum in each subplot will be chosen as vmax
+    :param prob: None or array
         if not None, then probability attached to the samples,
         in that case samples are treated as grid not a chain
-    density_estimation_method : {"gaussian_mixture", "smoothing",
-        "median_filter", "kde", "hist"}
+    :param density_estimation_method:
+        {"gaussian_mixture", "smoothing", "median_filter", "kde", "hist"}
         method how to estimate the density
-    label : str
+    :param label: str
         label of the plot
-    alpha_for_low_density : bool
+    :param alpha_for_low_density: bool
         if low density should fade out using alpha values
-    alpha_treshold : float in [0, 1]
+    :param alpha_treshold: float in [0, 1]
         fraction of sample where alpha value should reach 1
-        0 means alpha is 1 everwhere
+        0 means alpha is 1 everywhere
         1 means linear decrease of alpha from 0 to 1 over the whole range
     """
     kde, x_grid, y_grid = get_density_grid_2D(
         data=data,
         ranges=ranges,
         columns=columns,
         i=i,
@@ -257,51 +310,69 @@
     data,
     ranges,
     columns,
     i,
     j,
     fill,
     color,
-    de_kwargs,
-    line_kwargs,
+    de_kwargs={},
+    line_kwargs={},
     prob=None,
     density_estimation_method="smoothing",
     label=None,
     alpha=1,
 ):
     """
-    axc : matplotlib axis
+    Plot the density of the data in the given axis as a contour plot.
+
+    :param axc: matplotlib axis
         axis of the plot
-    data : numpy struct array
+    :param data: numpy struct array
         the data that should be plotted with column data
-    ranges : dict
+    :param ranges: dict
         dictionary with the ranges of of the plot for each parameter
-    columns : list
+    :param columns: list
         list of all parameters
-    i, j : int
-        index of pair of columns to plot
-    fill : bool
-        use filled contours
-    de_kwargs : dict
+    :param i: int
+        index of the first column to plot
+    :param j: int
+        index of the second column to plot
+    :param fill: bool
+        if the contour should be filled
+    :param color: str
+        color of the contour
+    :param de_kwargs: dict
         dict with kde settings, has to have n_points, n_levels_check, levels
-    line_kwargs: dict
-        dict with arguments passed to plt.contour or plt.contourf
-    prob : None or array
+    :param line_kwargs: dict
+        dict with line settings, has to have linewidth, linestyle
+    :param prob: None or array
         if not None, then probability attached to the samples,
         in that case samples are treated as grid not a chain
-    density_estimation_method : {"gaussian_mixture", "smoothing",
-        "median_filter", "kde", "hist"}
+    :param density_estimation_method:
+        {"gaussian_mixture", "smoothing", "median_filter", "kde", "hist"}
         method how to estimate the density
-    label : str
+    :param label: str
         label of the plot
-    alpha : float in [0, 1]
+    :param alpha: float
         alpha value of the contour
     """
 
     def _get_paler_colors(color_rgb, n_levels, pale_factor=None):
+        """
+        Get a list of colors that are paler than the given color.
+
+        :param color_rgb: str
+            color in rgb format
+        :param n_levels: int
+            number of levels
+        :param pale_factor: float
+            pale factor
+        :return: list
+            list of colors
+        """
 
         solid_contour_palefactor = 0.6
 
         # convert a color into an array of colors for used in contours
         color = matplotlib.colors.colorConverter.to_rgb(color_rgb)
         pale_factor = pale_factor or solid_contour_palefactor
         cols = [color]
@@ -321,60 +392,58 @@
     )
 
     levels_contour = get_confidence_levels(
         de=de,
         levels=de_kwargs["levels"],
         n_levels_check=de_kwargs["n_levels_check"],
     )
-
     with warnings.catch_warnings():
         # this will suppress all warnings in this block
         warnings.simplefilter("ignore")
         colors = _get_paler_colors(color_rgb=color, n_levels=len(de_kwargs["levels"]))
 
         for l_i, lvl in enumerate(levels_contour):
             if fill:
                 axc.contourf(
                     x_grid,
                     y_grid,
                     de,
                     levels=[lvl, np.inf],
                     colors=[colors[l_i]],
-                    label=label,
                     alpha=0.85 * alpha,
                     **line_kwargs,
                 )
                 if "zorder" not in line_kwargs:
                     line_kwargs["zorder"] = 299
                     delete_later = True
                 else:
                     delete_later = False
                 axc.contour(
                     x_grid,
                     y_grid,
                     de,
                     levels=[lvl, np.inf],
                     colors=color,
-                    label=label,
                     alpha=alpha,
                     **line_kwargs,
                 )
                 if delete_later:
                     del line_kwargs["zorder"]
             else:
                 axc.contour(
                     x_grid,
                     y_grid,
                     de,
                     levels=[lvl, np.inf],
                     colors=color,
                     alpha=alpha,
-                    label=label,
                     **line_kwargs,
                 )
+    # dummy plot to get legend
+    plt.plot(data[columns[i]][0], data[columns[j]][0], label=label, color=color)
 
 
 def scatter_density(
     axc,
     points1,
     points2,
     n_bins=50,
@@ -382,31 +451,37 @@
     lim2=None,
     norm_cols=False,
     n_points_scatter=-1,
     label=None,
     **kwargs,
 ):
     """
-    axc : matplotlib axis
+    Plot the density of the data in the given axis as a scatter plot. The color of
+    the scatter points is determined by the density of the points.
+
+    :param axc: matplotlib axis
         axis of the plot
-    points1, points2 : array
-        x and y coordinate of the scattered points
-    bins: int
-        number of bins used for the density estimation
-    lim1, lim2 : list with two entries
-        lower and upper limit for the two parameters
-    norm_cols : bool
-        if to normalize the value of the colums
-    n_points_scatter : int
-        number of points that should be plotted
-        if all points should be plotted, use -1
-    label : str
+    :param points1: numpy array
+        array of the first parameter
+    :param points2: numpy array
+        array of the second parameter
+    :param n_bins: int
+        number of bins
+    :param lim1: tuple
+        limits of the first parameter
+    :param lim2: tuple
+        limits of the second parameter
+    :param norm_cols: bool
+        if the columns should be normalized
+    :param n_points_scatter: int
+        number of points to plot
+    :param label: str
         label of the plot
-    kwargs: dict
-        arguments that are passed to plt.scatter()
+    :param kwargs: dict
+        dict with kwargs for the scatter plot
     """
 
     if lim1 is None:
         min1 = np.min(points1)
         max1 = np.max(points1)
     else:
         min1 = lim1[0]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trianglechain-0.2.0/src/trianglechain.egg-info/PKG-INFO` & `trianglechain-0.3.0/src/trianglechain.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: trianglechain
-Version: 0.2.0
+Version: 0.3.0
 Summary: Code to plot multidimensional distributions
-Author: Tomasz Kacprzak, Silvan Fischbacher
-Author-email: tomaszk@phys.ethz.ch, silvanf@phys.ethz.ch
+Author: Silvan Fischbacher, Tomasz Kacprzak
+Author-email: silvanf@phys.ethz.ch, tomaszk@phys.ethz.ch
 License: MIT License
 Project-URL: Source, https://cosmo-docs.phys.ethz.ch/trianglechain
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -51,22 +50,20 @@
     cov=np.diag(np.ones(3)),
     size=(10000)
 )
 
 tri = TriangleChain()
 tri.contour_cl(samples);
 ```
-The input data can be (structured) arrays or dictionaries.
+The input data can be rec arrays, numpy array, pandas dataframes or dictionaries.
 For more example plots, see [demos](https://cosmo-gitlab.phys.ethz.ch/cosmo_public/trianglechain/demo)
 
 Credits
 -------
 
 This package was created by Tomasz Kacprzak and further developed and extended by Silvan Fischbacher.
 The package is maintained by Silvan Fischbacher: silvanf@phys.ethz.ch.
 
 Contributions
 -------------
 Contributions are welcome, and they are greatly appreciated! Every
 little bit helps, and credit will always be given.
-
-
```

### Comparing `trianglechain-0.2.0/tests/test_trianglechain.py` & `trianglechain-0.3.0/tests/test_trianglechain.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # Copyright (C) 2022 ETH Zurich
 # Institute for Particle Physics and Astrophysics
+# Author: Silvan Fischbacher
+
 import numpy as np
 import os
 from trianglechain import TriangleChain
 
 
 def _get_abspath(file_name):
     return os.path.join(os.path.dirname(__file__), file_name)
```

