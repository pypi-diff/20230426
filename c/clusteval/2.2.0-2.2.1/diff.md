# Comparing `tmp/clusteval-2.2.0.tar.gz` & `tmp/clusteval-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clusteval-2.2.0.tar", last modified: Wed Apr 19 20:57:19 2023, max compression
+gzip compressed data, was "clusteval-2.2.1.tar", last modified: Wed Apr 26 05:37:59 2023, max compression
```

## Comparing `clusteval-2.2.0.tar` & `clusteval-2.2.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 20:57:19.646233 clusteval-2.2.0/
--rw-rw-rw-   0        0        0     1146 2023-04-10 15:32:29.000000 clusteval-2.2.0/LICENSE
--rw-rw-rw-   0        0        0        0 2023-04-10 15:32:29.000000 clusteval-2.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     8181 2023-04-19 20:57:19.627646 clusteval-2.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     7628 2023-04-19 20:54:55.000000 clusteval-2.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 20:57:19.585531 clusteval-2.2.0/clusteval/
--rw-rw-rw-   0        0        0     1118 2023-04-19 20:52:04.000000 clusteval-2.2.0/clusteval/__init__.py
--rw-rw-rw-   0        0        0     2361 2023-04-19 11:33:35.000000 clusteval-2.2.0/clusteval/bubblegrid.py
--rw-rw-rw-   0        0        0    38503 2023-04-19 20:45:55.000000 clusteval-2.2.0/clusteval/clusteval.py
--rw-rw-rw-   0        0        0     2015 2023-04-10 15:32:29.000000 clusteval-2.2.0/clusteval/coord2density.py
--rw-rw-rw-   0        0        0     8104 2023-04-15 13:48:17.000000 clusteval-2.2.0/clusteval/dbindex.py
--rw-rw-rw-   0        0        0     8605 2023-04-17 22:09:35.000000 clusteval-2.2.0/clusteval/dbscan.py
--rw-rw-rw-   0        0        0     6909 2023-04-15 14:19:24.000000 clusteval-2.2.0/clusteval/derivative.py
--rw-rw-rw-   0        0        0    22922 2023-04-19 20:56:14.000000 clusteval-2.2.0/clusteval/examples.py
--rw-rw-rw-   0        0        0     7479 2023-04-11 18:26:51.000000 clusteval-2.2.0/clusteval/hdbscan.py
--rw-rw-rw-   0        0        0     2841 2023-04-10 15:32:29.000000 clusteval-2.2.0/clusteval/plot_dendrogram.py
--rw-rw-rw-   0        0        0    14608 2023-04-19 20:06:49.000000 clusteval-2.2.0/clusteval/silhouette.py
-drwxrwxrwx   0        0        0        0 2023-04-19 20:57:19.626650 clusteval-2.2.0/clusteval/tests/
--rw-rw-rw-   0        0        0        0 2023-04-10 15:32:29.000000 clusteval-2.2.0/clusteval/tests/__init__.py
--rw-rw-rw-   0        0        0     6438 2023-04-19 20:54:22.000000 clusteval-2.2.0/clusteval/tests/test_clusteval.py
--rw-rw-rw-   0        0        0     4508 2023-04-18 09:18:54.000000 clusteval-2.2.0/clusteval/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-19 20:57:19.611223 clusteval-2.2.0/clusteval.egg-info/
--rw-rw-rw-   0        0        0     8181 2023-04-19 20:57:19.000000 clusteval-2.2.0/clusteval.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      540 2023-04-19 20:57:19.000000 clusteval-2.2.0/clusteval.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 20:57:19.000000 clusteval-2.2.0/clusteval.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       78 2023-04-19 20:57:19.000000 clusteval-2.2.0/clusteval.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-19 20:57:19.000000 clusteval-2.2.0/clusteval.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-19 20:57:19.646233 clusteval-2.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1456 2023-04-16 16:29:41.000000 clusteval-2.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 05:37:59.022703 clusteval-2.2.1/
+-rw-rw-rw-   0        0        0     1146 2023-04-10 15:32:29.000000 clusteval-2.2.1/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-04-10 15:32:29.000000 clusteval-2.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     8181 2023-04-26 05:37:59.021688 clusteval-2.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     7628 2023-04-19 20:54:55.000000 clusteval-2.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-26 05:37:59.005685 clusteval-2.2.1/clusteval/
+-rw-rw-rw-   0        0        0     1118 2023-04-25 20:10:45.000000 clusteval-2.2.1/clusteval/__init__.py
+-rw-rw-rw-   0        0        0     2361 2023-04-19 11:33:35.000000 clusteval-2.2.1/clusteval/bubblegrid.py
+-rw-rw-rw-   0        0        0    38410 2023-04-25 20:07:58.000000 clusteval-2.2.1/clusteval/clusteval.py
+-rw-rw-rw-   0        0        0     2015 2023-04-10 15:32:29.000000 clusteval-2.2.1/clusteval/coord2density.py
+-rw-rw-rw-   0        0        0     8104 2023-04-15 13:48:17.000000 clusteval-2.2.1/clusteval/dbindex.py
+-rw-rw-rw-   0        0        0     8605 2023-04-17 22:09:35.000000 clusteval-2.2.1/clusteval/dbscan.py
+-rw-rw-rw-   0        0        0     6909 2023-04-15 14:19:24.000000 clusteval-2.2.1/clusteval/derivative.py
+-rw-rw-rw-   0        0        0    22985 2023-04-25 20:06:00.000000 clusteval-2.2.1/clusteval/examples.py
+-rw-rw-rw-   0        0        0     7479 2023-04-11 18:26:51.000000 clusteval-2.2.1/clusteval/hdbscan.py
+-rw-rw-rw-   0        0        0     2841 2023-04-10 15:32:29.000000 clusteval-2.2.1/clusteval/plot_dendrogram.py
+-rw-rw-rw-   0        0        0    14608 2023-04-19 20:06:49.000000 clusteval-2.2.1/clusteval/silhouette.py
+drwxrwxrwx   0        0        0        0 2023-04-26 05:37:59.020680 clusteval-2.2.1/clusteval/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-10 15:32:29.000000 clusteval-2.2.1/clusteval/tests/__init__.py
+-rw-rw-rw-   0        0        0     6435 2023-04-19 21:06:14.000000 clusteval-2.2.1/clusteval/tests/test_clusteval.py
+-rw-rw-rw-   0        0        0     4508 2023-04-18 09:18:54.000000 clusteval-2.2.1/clusteval/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-26 05:37:59.018653 clusteval-2.2.1/clusteval.egg-info/
+-rw-rw-rw-   0        0        0     8181 2023-04-26 05:37:58.000000 clusteval-2.2.1/clusteval.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      540 2023-04-26 05:37:58.000000 clusteval-2.2.1/clusteval.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 05:37:58.000000 clusteval-2.2.1/clusteval.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       78 2023-04-26 05:37:58.000000 clusteval-2.2.1/clusteval.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-26 05:37:58.000000 clusteval-2.2.1/clusteval.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-26 05:37:59.022703 clusteval-2.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1456 2023-04-16 16:29:41.000000 clusteval-2.2.1/setup.py
```

### Comparing `clusteval-2.2.0/LICENSE` & `clusteval-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `clusteval-2.2.0/PKG-INFO` & `clusteval-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: clusteval
-Version: 2.2.0
+Version: 2.2.1
 Summary: clusteval is a python package for unsupervised cluster validation.
 Home-page: https://erdogant.github.io/clusteval
-Download-URL: https://github.com/erdogant/clusteval/archive/2.2.0.tar.gz
+Download-URL: https://github.com/erdogant/clusteval/archive/2.2.1.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: clusteval Version: 2.2.0 Summary: clusteval is a
+Metadata-Version: 2.1 Name: clusteval Version: 2.2.1 Summary: clusteval is a
 python package for unsupervised cluster validation. Home-page: https://
 erdogant.github.io/clusteval Download-URL: https://github.com/erdogant/
-clusteval/archive/2.2.0.tar.gz Author: Erdogan Taskesen Author-email:
+clusteval/archive/2.2.1.tar.gz Author: Erdogan Taskesen Author-email:
 erdogant@gmail.com Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3 Description-Content-Type: text/markdown
 License-File: LICENSE # clusteval
 [https://github.com/erdogant/clusteval/blob/master/docs/figs/logo_large_2.png]
 [![Python](https://img.shields.io/pypi/pyversions/clusteval)](https://
 img.shields.io/pypi/pyversions/clusteval) [![PyPI Version](https://
```

### Comparing `clusteval-2.2.0/README.md` & `clusteval-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `clusteval-2.2.0/clusteval/__init__.py` & `clusteval-2.2.1/clusteval/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     dbscan,
     # hdbscan_custom,
     )
 
 
 __author__ = 'Erdogan Tasksen'
 __email__ = 'erdogant@gmail.com'
-__version__ = '2.2.0'
+__version__ = '2.2.1'
 
 
 __doc__ = """
 clusteval
 =====================================================================
 
 Description
```

### Comparing `clusteval-2.2.0/clusteval/bubblegrid.py` & `clusteval-2.2.1/clusteval/bubblegrid.py`

 * *Files identical despite different names*

### Comparing `clusteval-2.2.0/clusteval/clusteval.py` & `clusteval-2.2.1/clusteval/clusteval.py`

 * *Files 1% similar despite different names*

```diff
@@ -326,16 +326,19 @@
                 n_feat=2,
                 legend=False,
                 jitter=None,
                 cmap='tab20c',
                 figsize=(25, 15),
                 fontsize=16,
                 fontcolor='k',
-                savefig={'fname': None, format: 'png', 'dpi ': None, 'orientation': 'portrait', 'facecolor': 'auto'},
+                density=False,
+                grid=True,
                 showfig=True,
+                savefig={'fname': None, format: 'png', 'dpi ': None, 'orientation': 'portrait', 'facecolor': 'auto'},
+                params_scatterd = {'dpi': 100, 'marker': 'o', 'alpha': 0.8},
                 ):
         """Scatterplot.
 
         Create a scatterplot for the first two features or with an t-SNE embedding.
         The clusters are colored based on the cluster labels and labeld with the features from the enrichment analysis.
 
         Parameters
@@ -396,16 +399,15 @@
         # Make some checks
         if not _check_results(self, logger): return None
         X = _check_input_data(self, X, logger)
         if X is None: return None
         if isinstance(X, pd.DataFrame): X = X.values
 
         # Defaults
-        defaults = {'figsize': (25, 15), 'cmap': 'tab20c', 'z': None, 'c': [0, 0, 0], 'marker': None, 'alpha': 0.8, 'gradient': None, 'density': False, 'norm': False, 'xlabel': 'x-axis', 'ylabel': 'y-axis', 'title': '', 'fontsize': 20, 'fontcolor': None, 'axiscolor': '#dddddd', 'jitter': None}
-        params = {**defaults, **{'jitter': jitter, 'cmap': cmap}, 'figsize': figsize, 'fontsize': fontsize, 'fontcolor': fontcolor}
+        params = {**params_scatterd, **{'grid': grid, 'edgecolor': '#000000', 'jitter': jitter, 'cmap': cmap, 'figsize': figsize, 'fontsize': fontsize, 'fontcolor': fontcolor, 'density': density}}
 
         # Compute embedding
         X = compute_embedding(self, X, embedding, logger)
 
         if self.results.get('enrichment') is None:
             labels = self.results['labx']
             scores = np.ones(X.shape[0]) * s
```

### Comparing `clusteval-2.2.0/clusteval/coord2density.py` & `clusteval-2.2.1/clusteval/coord2density.py`

 * *Files identical despite different names*

### Comparing `clusteval-2.2.0/clusteval/dbindex.py` & `clusteval-2.2.1/clusteval/dbindex.py`

 * *Files identical despite different names*

### Comparing `clusteval-2.2.0/clusteval/dbscan.py` & `clusteval-2.2.1/clusteval/dbscan.py`

 * *Files identical despite different names*

### Comparing `clusteval-2.2.0/clusteval/derivative.py` & `clusteval-2.2.1/clusteval/derivative.py`

 * *Files identical despite different names*

### Comparing `clusteval-2.2.0/clusteval/examples.py` & `clusteval-2.2.1/clusteval/examples.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 xycoord = TSNE(n_components=2, init='random', perplexity=30).fit_transform(dfhot.values)
 # ce = clusteval(cluster='dbscan', min_clust=2, verbose='info')
 ce = clusteval(evaluate='silhouette', cluster='agglomerative', linkage='complete', min_clust=5, max_clust=30, verbose='info')
 ce.fit(xycoord)
 
 ce.plot()
 ce.plot_silhouette()
-ce.scatter()
+ce.scatter(jitter=0.05, density=True, params_scatterd={'grid': True}, s=10)
 ce.enrichment(df)
 ce.scatter(fontcolor='k', n_feat=2)
 
 from scatterd import scatterd
 # scatterd(xycoord[:,0], xycoord[:,1], labels=ce.results['labx'], cmap='tab20c')
 scatterd(xycoord[:,0], xycoord[:,1], labels=df['Browser'], fontcolor='k', cmap='tab20c')
 scatterd(xycoord[:,0], xycoord[:,1], labels=dfhot['TrafficType_11.0'], fontcolor='k', cmap='tab20c')
```

### Comparing `clusteval-2.2.0/clusteval/hdbscan.py` & `clusteval-2.2.1/clusteval/hdbscan.py`

 * *Files identical despite different names*

### Comparing `clusteval-2.2.0/clusteval/plot_dendrogram.py` & `clusteval-2.2.1/clusteval/plot_dendrogram.py`

 * *Files identical despite different names*

### Comparing `clusteval-2.2.0/clusteval/silhouette.py` & `clusteval-2.2.1/clusteval/silhouette.py`

 * *Files identical despite different names*

### Comparing `clusteval-2.2.0/clusteval/tests/test_clusteval.py` & `clusteval-2.2.1/clusteval/tests/test_clusteval.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,16 +67,16 @@
             assert df.shape==size
 
     def test_fit(self):
         ce = clusteval()
         X, y_true = ce.import_example(data='blobs', params={'random_state': 1})
 
         # Set all parameters to be evaluated
-        clusters = ['agglomerative', 'kmeans', 'dbscan']
-        evaluates = ['silhouette', 'dbindex', 'derivative']
+        clusters = ['dbscan', 'agglomerative', 'kmeans']
+        evaluates = ['dbindex', 'derivative', 'silhouette']
         metrics = ['euclidean', 'hamming']
         linkages = ['ward', 'single', 'complete']
         min_clusts = [1, 2, 10]
         max_clusts = [1, 10, 2]
 
         # Evaluate across all paramters
         out = parameter_gridtest(X, y_true, clusters, evaluates, metrics, linkages, min_clusts, max_clusts)
@@ -112,15 +112,15 @@
                                 ce = clusteval(evaluate=evaluate, cluster=cluster, metric=metric, linkage=linkage, min_clust=min_clust, max_clust=max_clust, verbose=2)
                                 results = ce.fit(X)
                                 # print('Clusters: %s' %(str(np.unique(results['labx']))))
                                 # assert ce.plot()
                                 # assert ce.scatter(X)
                                 # assert ce.dendrogram()
 
-                                if (ce.results is not None) and (ce.results['labx'] is not None) and (linkage!='single') and (min_clust < len(np.unique(y_true))) and (max_clust > len(np.unique(y_true))) and (metric=='euclidean'):
+                                if (results is not None) and (ce.results['labx'] is not None) and (linkage!='single') and (min_clust < len(np.unique(y_true))) and (max_clust > len(np.unique(y_true))) and (metric=='euclidean'):
                                     # print(len(np.unique(results['labx'])))
                                     # print(len(np.unique(y_true)))
                                     assert len(np.unique(results['labx']))==len(np.unique(y_true))
 
                             except ValueError as err:
                                 assert not 'clusteval' in err.args
                                 status = err.args
```

### Comparing `clusteval-2.2.0/clusteval/utils.py` & `clusteval-2.2.1/clusteval/utils.py`

 * *Files identical despite different names*

### Comparing `clusteval-2.2.0/clusteval.egg-info/PKG-INFO` & `clusteval-2.2.1/clusteval.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: clusteval
-Version: 2.2.0
+Version: 2.2.1
 Summary: clusteval is a python package for unsupervised cluster validation.
 Home-page: https://erdogant.github.io/clusteval
-Download-URL: https://github.com/erdogant/clusteval/archive/2.2.0.tar.gz
+Download-URL: https://github.com/erdogant/clusteval/archive/2.2.1.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: clusteval Version: 2.2.0 Summary: clusteval is a
+Metadata-Version: 2.1 Name: clusteval Version: 2.2.1 Summary: clusteval is a
 python package for unsupervised cluster validation. Home-page: https://
 erdogant.github.io/clusteval Download-URL: https://github.com/erdogant/
-clusteval/archive/2.2.0.tar.gz Author: Erdogan Taskesen Author-email:
+clusteval/archive/2.2.1.tar.gz Author: Erdogan Taskesen Author-email:
 erdogant@gmail.com Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3 Description-Content-Type: text/markdown
 License-File: LICENSE # clusteval
 [https://github.com/erdogant/clusteval/blob/master/docs/figs/logo_large_2.png]
 [![Python](https://img.shields.io/pypi/pyversions/clusteval)](https://
 img.shields.io/pypi/pyversions/clusteval) [![PyPI Version](https://
```

### Comparing `clusteval-2.2.0/clusteval.egg-info/SOURCES.txt` & `clusteval-2.2.1/clusteval.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clusteval-2.2.0/setup.py` & `clusteval-2.2.1/setup.py`

 * *Files identical despite different names*

