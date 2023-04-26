# Comparing `tmp/decodanda-0.6.3.tar.gz` & `tmp/decodanda-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decodanda-0.6.3.tar", last modified: Thu Apr 20 17:52:41 2023, max compression
+gzip compressed data, was "decodanda-0.6.4.tar", last modified: Wed Apr 26 18:03:23 2023, max compression
```

## Comparing `decodanda-0.6.3.tar` & `decodanda-0.6.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 lorenzo    (501) staff       (20)        0 2023-04-20 17:52:41.073698 decodanda-0.6.3/
--rw-r--r--   0 lorenzo    (501) staff       (20)    35149 2023-02-15 23:52:18.000000 decodanda-0.6.3/LICENSE.md
--rw-r--r--   0 lorenzo    (501) staff       (20)      991 2023-04-20 17:52:41.073360 decodanda-0.6.3/PKG-INFO
--rw-r--r--   0 lorenzo    (501) staff       (20)    36482 2023-04-19 18:21:22.000000 decodanda-0.6.3/README.md
-drwxr-xr-x   0 lorenzo    (501) staff       (20)        0 2023-04-20 17:52:41.068916 decodanda-0.6.3/decodanda/
--rw-r--r--   0 lorenzo    (501) staff       (20)      251 2023-02-17 22:21:32.000000 decodanda-0.6.3/decodanda/__init__.py
--rw-r--r--   0 lorenzo    (501) staff       (20)    98867 2023-04-19 18:20:38.000000 decodanda-0.6.3/decodanda/classes.py
--rw-r--r--   0 lorenzo    (501) staff       (20)     1194 2023-02-15 00:18:50.000000 decodanda-0.6.3/decodanda/imports.py
--rw-r--r--   0 lorenzo    (501) staff       (20)    11247 2023-02-17 19:33:24.000000 decodanda-0.6.3/decodanda/in_time.py
--rw-r--r--   0 lorenzo    (501) staff       (20)    39339 2023-02-17 17:08:36.000000 decodanda-0.6.3/decodanda/utilities.py
--rw-r--r--   0 lorenzo    (501) staff       (20)    22115 2023-04-18 20:45:44.000000 decodanda-0.6.3/decodanda/visualize.py
-drwxr-xr-x   0 lorenzo    (501) staff       (20)        0 2023-04-20 17:52:41.072850 decodanda-0.6.3/decodanda.egg-info/
--rw-r--r--   0 lorenzo    (501) staff       (20)      991 2023-04-20 17:52:41.000000 decodanda-0.6.3/decodanda.egg-info/PKG-INFO
--rw-r--r--   0 lorenzo    (501) staff       (20)      324 2023-04-20 17:52:41.000000 decodanda-0.6.3/decodanda.egg-info/SOURCES.txt
--rw-r--r--   0 lorenzo    (501) staff       (20)        1 2023-04-20 17:52:41.000000 decodanda-0.6.3/decodanda.egg-info/dependency_links.txt
--rw-r--r--   0 lorenzo    (501) staff       (20)      109 2023-04-20 17:52:41.000000 decodanda-0.6.3/decodanda.egg-info/requires.txt
--rw-r--r--   0 lorenzo    (501) staff       (20)       10 2023-04-20 17:52:41.000000 decodanda-0.6.3/decodanda.egg-info/top_level.txt
--rw-r--r--   0 lorenzo    (501) staff       (20)       38 2023-04-20 17:52:41.073816 decodanda-0.6.3/setup.cfg
--rw-r--r--   0 lorenzo    (501) staff       (20)     1388 2023-04-20 17:51:43.000000 decodanda-0.6.3/setup.py
+drwxr-xr-x   0 lorenzo    (501) staff       (20)        0 2023-04-26 18:03:23.321115 decodanda-0.6.4/
+-rw-r--r--   0 lorenzo    (501) staff       (20)    35149 2023-02-15 23:52:18.000000 decodanda-0.6.4/LICENSE.md
+-rw-r--r--   0 lorenzo    (501) staff       (20)      991 2023-04-26 18:03:23.320786 decodanda-0.6.4/PKG-INFO
+-rw-r--r--   0 lorenzo    (501) staff       (20)    36482 2023-04-19 18:21:22.000000 decodanda-0.6.4/README.md
+drwxr-xr-x   0 lorenzo    (501) staff       (20)        0 2023-04-26 18:03:23.317613 decodanda-0.6.4/decodanda/
+-rw-r--r--   0 lorenzo    (501) staff       (20)      251 2023-02-17 22:21:32.000000 decodanda-0.6.4/decodanda/__init__.py
+-rw-r--r--   0 lorenzo    (501) staff       (20)    98954 2023-04-26 18:00:57.000000 decodanda-0.6.4/decodanda/classes.py
+-rw-r--r--   0 lorenzo    (501) staff       (20)     1194 2023-02-15 00:18:50.000000 decodanda-0.6.4/decodanda/imports.py
+-rw-r--r--   0 lorenzo    (501) staff       (20)    11247 2023-02-17 19:33:24.000000 decodanda-0.6.4/decodanda/in_time.py
+-rw-r--r--   0 lorenzo    (501) staff       (20)    39339 2023-02-17 17:08:36.000000 decodanda-0.6.4/decodanda/utilities.py
+-rw-r--r--   0 lorenzo    (501) staff       (20)    24405 2023-04-26 17:59:31.000000 decodanda-0.6.4/decodanda/visualize.py
+drwxr-xr-x   0 lorenzo    (501) staff       (20)        0 2023-04-26 18:03:23.320340 decodanda-0.6.4/decodanda.egg-info/
+-rw-r--r--   0 lorenzo    (501) staff       (20)      991 2023-04-26 18:03:23.000000 decodanda-0.6.4/decodanda.egg-info/PKG-INFO
+-rw-r--r--   0 lorenzo    (501) staff       (20)      324 2023-04-26 18:03:23.000000 decodanda-0.6.4/decodanda.egg-info/SOURCES.txt
+-rw-r--r--   0 lorenzo    (501) staff       (20)        1 2023-04-26 18:03:23.000000 decodanda-0.6.4/decodanda.egg-info/dependency_links.txt
+-rw-r--r--   0 lorenzo    (501) staff       (20)      109 2023-04-26 18:03:23.000000 decodanda-0.6.4/decodanda.egg-info/requires.txt
+-rw-r--r--   0 lorenzo    (501) staff       (20)       10 2023-04-26 18:03:23.000000 decodanda-0.6.4/decodanda.egg-info/top_level.txt
+-rw-r--r--   0 lorenzo    (501) staff       (20)       38 2023-04-26 18:03:23.321233 decodanda-0.6.4/setup.cfg
+-rw-r--r--   0 lorenzo    (501) staff       (20)     1388 2023-04-26 18:01:26.000000 decodanda-0.6.4/setup.py
```

### Comparing `decodanda-0.6.3/LICENSE.md` & `decodanda-0.6.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `decodanda-0.6.3/PKG-INFO` & `decodanda-0.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decodanda
-Version: 0.6.3
+Version: 0.6.4
 Summary: A python package for neural decoding with built-in best practices.
 Home-page: https://github.com/lposani/decodanda
 Author: Lorenzo Posani
 Author-email: lorenzo.posani@gmail.com
 Keywords: python,decoding,neuroscience,ccgp,neural activity,population activity,neural decoding,geometry
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `decodanda-0.6.3/README.md` & `decodanda-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `decodanda-0.6.3/decodanda/classes.py` & `decodanda-0.6.4/decodanda/classes.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import numpy as np
 import scipy.stats.stats
 from numpy import ndarray
 from .imports import *
 from .utilities import generate_binary_words, string_bool, sample_training_testing_from_rasters, CrossValidator, \
     log_dichotomy, hamming, sample_from_rasters, generate_dichotomies, semantic_score, z_pval, DictSession, \
     contiguous_chunking, non_contiguous_mask, cosine
-from .visualize import corr_scatter, visualize_decoding, plot_perfs_null_model
+from .visualize import corr_scatter, visualize_decoding, plot_perfs_null_model, visualize_PCA
 
 
 # Main class
 
 class Decodanda:
     def __init__(self,
                  data: Union[list, dict],
@@ -387,15 +387,15 @@
 
         if self._debug:
             selectivity_training = np.nanmean(training_array_A, 0) - np.nanmean(training_array_B, 0)
             selectivity_testing = np.nanmean(testing_array_A, 0) - np.nanmean(testing_array_B, 0)
             corr_scatter(selectivity_training, selectivity_testing, 'Selectivity (training)', 'Selectivity (testing)')
 
         if self._zscore:
-            big_raster = np.vstack([training_array_A, training_array_B, testing_array_A, testing_array_B])
+            big_raster = np.vstack([training_array_A, training_array_B])  # z-scoring using the training data
             big_mean = np.nanmean(big_raster, 0)
             big_std = np.nanstd(big_raster, 0)
             big_std[big_std == 0] = np.inf
             training_array_A = (training_array_A - big_mean) / big_std
             training_array_B = (training_array_B - big_mean) / big_std
             testing_array_A = (testing_array_A - big_mean) / big_std
             testing_array_B = (testing_array_B - big_mean) / big_std
@@ -698,16 +698,15 @@
                             rotation_B = np.arange(testing_array_B.shape[1]).astype(int)
                             np.random.shuffle(rotation_A)
                             np.random.shuffle(rotation_B)
                             testing_array_A = testing_array_A[:, rotation_A]
                             testing_array_B = testing_array_B[:, rotation_A]
 
                         if self._zscore:
-                            big_raster = np.vstack(
-                                [training_array_A, training_array_B, testing_array_A, testing_array_B])
+                            big_raster = np.vstack([training_array_A, training_array_B])  # z-scoring using the training data
                             big_mean = np.nanmean(big_raster, 0)
                             big_std = np.nanstd(big_raster, 0)
                             big_std[big_std == 0] = np.inf
                             training_array_A = (training_array_A - big_mean) / big_std
                             training_array_B = (training_array_B - big_mean) / big_std
                             testing_array_A = (testing_array_A - big_mean) / big_std
                             testing_array_B = (testing_array_B - big_mean) / big_std
@@ -1525,15 +1524,20 @@
 
         dichotomies_data = [all_dics, semantic_overlap]
         decoding_data = [decoding_results, decoding_null]
         CCGP_data = [CCGP_results, CCGP_null]
 
         return dichotomies_data, decoding_data, CCGP_data
 
-    # init utilities
+    # Utilities
+
+    def visualize_PCA(self, **kwargs):
+        visualize_PCA(self, **kwargs)
+
+    # __init__ utilities
 
     def _divide_data_into_conditions(self, sessions):
         # TODO: rename sessions into datasets?
         # TODO: make sure conditions don't overlap somehow
 
         for si, session in enumerate(sessions):
```

### Comparing `decodanda-0.6.3/decodanda/imports.py` & `decodanda-0.6.4/decodanda/imports.py`

 * *Files identical despite different names*

### Comparing `decodanda-0.6.3/decodanda/in_time.py` & `decodanda-0.6.4/decodanda/in_time.py`

 * *Files identical despite different names*

### Comparing `decodanda-0.6.3/decodanda/utilities.py` & `decodanda-0.6.4/decodanda/utilities.py`

 * *Files identical despite different names*

### Comparing `decodanda-0.6.3/decodanda/visualize.py` & `decodanda-0.6.4/decodanda/visualize.py`

 * *Files 6% similar despite different names*

```diff
@@ -132,15 +132,15 @@
             pval = z_pval(perfs[l], perfs_nullmodel[l])[1]
 
         ax.scatter([i], [perfs[l]], marker=marker, s=100, color=pltcolors[i], facecolor='none', linewidth=2)
         if annotate:
             ptext = p_to_text(pval).split('\n')[1]
             trans = transforms.blended_transform_factory(
                 ax.transData, ax.transAxes)
-            ax.text(i-0.22, 0.0,
+            ax.text(i - 0.22, 0.0,
                     'data=%.2f\nnull=%.2f$\pm$%.2f\n%s' %
                     (perfs[l], np.nanmean(perfs_nullmodel[l]), np.nanstd(perfs_nullmodel[l]), ptext),
                     va='bottom', ha='left', fontsize=7, backgroundcolor='1.00', transform=trans)
             ax.set_xticklabels(labels, rotation=0, ha='center')
 
         pvals[l] = pval
         if pval < 0.05:
@@ -421,16 +421,16 @@
         if axs is None:
             fig = plt.figure(figsize=(6, 5))
             ax = fig.add_subplot(projection='3d')
         else:
             ax = axs
             fig = ax.get_figure()
 
-    #ax.grid(False)
-    #ax.set_axis_off()
+    # ax.grid(False)
+    # ax.set_axis_off()
     plt.subplots_adjust(left=0, right=0.95, top=1, bottom=0)
 
     def init():
         for i in range(len(names)):
             ax.scatter(components[i, 0], components[i, 1], components[i, 2], alpha=0.7, marker='$%s$' % names[i],
                        s=400)
         for i in range(len(names)):
@@ -459,35 +459,47 @@
         anim.save(savename, writer=mywriter)
     else:
         init()
     mpl.rcParams.update({'figure.autolayout': True})
     return fig
 
 
-def visualize_balanced_MDS(dec, dim=3, ndata=None, savename=None, title='', data=None, null=None, names=None, axs=None):
+def visualize_PCA(dec, dim=3,
+                  ndata=None, savename=None, title='',
+                  data=None, null=None, names=None, axs=None,
+                  alpha=None, z_score=False, mean=False, draw_hd2_lines=True):
     # performance and CCGP
 
     mpl.rcParams.update({'figure.autolayout': False})
     rasters = []
     labels = []
     if ndata is None:
-        ndata =  dec._max_conditioned_data
+        ndata = dec._max_conditioned_data
+    if names is None:
+        names = list(dec._semantic_vectors.keys())
 
-    for key in dec.conditioned_rasters:
+    for i, key in enumerate(dec.conditioned_rasters):
         X = sample_from_rasters(dec.conditioned_rasters[key], ndata)
         rasters.append(X)
-        y = np.repeat(key, ndata)
+        y = np.repeat(names[i], ndata)
         labels.append(y)
     X = np.vstack(rasters)
+    if z_score:
+        for i in range(X.shape[1]):
+            if np.nanstd(X[:, i]):
+                X[:, i] = (X[:, i] - np.nanmean(X[:, i])) / np.nanstd(X[:, i])
     y = np.hstack(labels)
     C = sklearn.decomposition.PCA(n_components=dim)
     components = C.fit_transform(X, y)
 
-    if names is None:
-        names = list(dec._semantic_vectors.keys())
+    means = []
+    for name in names:
+        mask = y == name
+        means.append(np.median(components[mask, :], 0))
+    means = np.asarray(means)
 
     if data is not None and null is not None:
         if axs is None:
             fig = plt.figure(figsize=(12, 5))
             G = GridSpec(12, 12)
             ax = fig.add_subplot(G[:, 0:6], projection='3d')
             ax_dec = fig.add_subplot(G[1:9, 6:9])
@@ -501,31 +513,63 @@
         ax_dec.set_title(title)
 
         plot_perfs_null_model(data['Decoding'], null['Decoding'], ax=ax_dec, marker='o')
         plot_perfs_null_model(data['CCGP'], null['CCGP'], ax=ax_ccgp, ylabel='CCGP', marker='s')
     else:
         if axs is None:
             fig = plt.figure(figsize=(6, 5))
-            ax = fig.add_subplot(projection='3d')
+            if dim >= 3:
+                ax = fig.add_subplot(projection='3d')
+            if dim == 2:
+                ax = fig.add_subplot()
         else:
             ax = axs
             fig = ax.get_figure()
 
     plt.subplots_adjust(left=0, right=0.95, top=1, bottom=0)
 
     def init():
         for i in range(len(names)):
             mask = (y == names[i])
-            ax.scatter(components[mask, 0], components[mask, 1], components[mask, 2], alpha=0.05, marker='o',
-                       s=20)
-        equalize_ax(ax)
-
-        ax.set_xticklabels([])
-        ax.set_yticklabels([])
-        ax.set_zticklabels([])
+            if alpha is None:
+                a = min(0.8, 40. / np.sum(mask))
+            else:
+                a = alpha
+            if dim >= 3:
+                if not mean:
+                    ax.scatter(components[mask, 0], components[mask, 1], components[mask, 2], alpha=a, marker='o',
+                               s=20, label=dec._semantic_vectors[names[i]])
+                else:
+                    for i in range(len(names)):
+                        ax.scatter(means[i, 0], means[i, 1], means[i, 2], alpha=0.7,
+                                   marker='$%s$' % names[i],
+                                   s=1000, color=pltcolors[i], edgecolor='w', linewidths=5)
+                        ax.scatter(means[i, 0], means[i, 1], means[i, 2], alpha=0.7,
+                                   marker='$%s$' % names[i],
+                                   s=1000, color=pltcolors[i])
+                    for i in range(len(names)):
+                        for j in range(i + 1, len(names)):
+                            if hamming_distance(names[i], names[j]) == 1:
+                                ax.plot([means[i][0], means[j][0]], [means[i][1], means[j][1]],
+                                        [means[i][2], means[j][2]], linestyle='-', linewidth=2, color='k',
+                                        alpha=0.7)
+                            elif (hamming_distance(names[i], names[j]) == 2) and draw_hd2_lines:
+                                ax.plot([means[i][0], means[j][0]], [means[i][1], means[j][1]],
+                                        [means[i][2], means[j][2]], linestyle='--', color='k', alpha=0.3)
+
+                # equalize_ax(ax)
+
+                ax.set_xticklabels([])
+                ax.set_yticklabels([])
+                ax.set_zticklabels([])
+            if dim == 2:
+                ax.scatter(components[mask, 0], components[mask, 1], alpha=a, marker='o',
+                           s=20, label=dec._semantic_vectors[names[i]])
+            if not mean:
+                plt.legend()
         return fig,
 
     def animate(i):
         ax.view_init(elev=10., azim=i * 2)
         return fig,
 
     if savename:
@@ -533,8 +577,7 @@
                                        frames=360, interval=20, blit=True)
         mywriter = animation.PillowWriter(fps=30)
         anim.save(savename, writer=mywriter)
     else:
         init()
     mpl.rcParams.update({'figure.autolayout': True})
     return fig
-
```

### Comparing `decodanda-0.6.3/decodanda.egg-info/PKG-INFO` & `decodanda-0.6.4/decodanda.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decodanda
-Version: 0.6.3
+Version: 0.6.4
 Summary: A python package for neural decoding with built-in best practices.
 Home-page: https://github.com/lposani/decodanda
 Author: Lorenzo Posani
 Author-email: lorenzo.posani@gmail.com
 Keywords: python,decoding,neuroscience,ccgp,neural activity,population activity,neural decoding,geometry
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `decodanda-0.6.3/setup.py` & `decodanda-0.6.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.6.3'
+VERSION = '0.6.4'
 DESCRIPTION = 'A python package for neural decoding with built-in best practices.'
 LONG_DESCRIPTION = 'Decodanda (dog latin for "to be decoded") is a best-practices-made-easy Python package for decoding neural data. Decodanda is designed to expose a user-friendly and flexible interface for population activity decoding, with a series of built-in best practices to avoid the most common pitfalls. In addition, Decodanda exposes a series of functions to compute the Cross-Condition Generalization Performance (CCGP, Bernardi et al. 2020) for the geometrical analysis of neural population activity.'
 
 setup(
     name="decodanda",
     version=VERSION,
     author="Lorenzo Posani",
```

