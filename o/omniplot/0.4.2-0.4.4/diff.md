# Comparing `tmp/omniplot-0.4.2.tar.gz` & `tmp/omniplot-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omniplot-0.4.2.tar", last modified: Wed Apr 26 08:10:14 2023, max compression
+gzip compressed data, was "omniplot-0.4.4.tar", last modified: Wed Apr 26 10:03:04 2023, max compression
```

## Comparing `omniplot-0.4.2.tar` & `omniplot-0.4.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 koh       (1000) koh       (1000)        0 2023-04-26 08:10:14.935906 omniplot-0.4.2/
--rw-rw-r--   0 koh       (1000) koh       (1000)    35149 2023-04-22 04:16:47.000000 omniplot-0.4.2/LICENSE
--rw-rw-r--   0 koh       (1000) koh       (1000)      976 2023-04-26 08:10:14.935906 omniplot-0.4.2/PKG-INFO
--rw-rw-r--   0 koh       (1000) koh       (1000)     3276 2023-04-22 04:16:47.000000 omniplot-0.4.2/README.md
-drwxrwxr-x   0 koh       (1000) koh       (1000)        0 2023-04-26 08:10:14.935906 omniplot-0.4.2/omniplot/
--rw-rw-r--   0 koh       (1000) koh       (1000)      580 2023-04-22 04:16:47.000000 omniplot-0.4.2/omniplot/__init__.py
--rw-rw-r--   0 koh       (1000) koh       (1000)    21778 2023-04-22 04:16:47.000000 omniplot-0.4.2/omniplot/_adjustText.py
--rw-rw-r--   0 koh       (1000) koh       (1000)       21 2023-04-26 07:55:31.000000 omniplot-0.4.2/omniplot/_version.py
--rw-rw-r--   0 koh       (1000) koh       (1000)    57911 2023-04-22 04:16:47.000000 omniplot-0.4.2/omniplot/chipseq.py
--rw-rw-r--   0 koh       (1000) koh       (1000)    21857 2023-04-22 04:16:47.000000 omniplot-0.4.2/omniplot/chipseq_utils.py
-drwxrwxr-x   0 koh       (1000) koh       (1000)        0 2023-04-26 08:10:14.935906 omniplot-0.4.2/omniplot/cython_utils/
--rw-rw-r--   0 koh       (1000) koh       (1000)        0 2023-04-22 04:16:47.000000 omniplot-0.4.2/omniplot/cython_utils/__init__.py
--rw-rw-r--   0 koh       (1000) koh       (1000)      288 2023-04-22 04:16:47.000000 omniplot-0.4.2/omniplot/data.py
--rw-rw-r--   0 koh       (1000) koh       (1000)   100722 2023-04-26 05:15:30.000000 omniplot-0.4.2/omniplot/heatmap.py
--rw-rw-r--   0 koh       (1000) koh       (1000)    12843 2023-04-22 04:16:47.000000 omniplot-0.4.2/omniplot/igraph_classes.py
--rw-rw-r--   0 koh       (1000) koh       (1000)    32121 2023-04-22 04:16:47.000000 omniplot-0.4.2/omniplot/networkplot.py
--rw-rw-r--   0 koh       (1000) koh       (1000)    10853 2023-04-22 05:11:17.000000 omniplot-0.4.2/omniplot/plot.py
--rw-rw-r--   0 koh       (1000) koh       (1000)     3511 2023-04-22 04:16:47.000000 omniplot-0.4.2/omniplot/plot_classes.py
--rw-rw-r--   0 koh       (1000) koh       (1000)    73070 2023-04-22 04:16:47.000000 omniplot-0.4.2/omniplot/proportion.py
--rw-rw-r--   0 koh       (1000) koh       (1000)    10740 2023-04-22 04:16:47.000000 omniplot-0.4.2/omniplot/regressionplot.py
--rw-rw-r--   0 koh       (1000) koh       (1000)   134250 2023-04-22 04:16:47.000000 omniplot-0.4.2/omniplot/scatter.py
-drwxrwxr-x   0 koh       (1000) koh       (1000)        0 2023-04-26 08:10:14.935906 omniplot-0.4.2/omniplot/scripts/
--rw-rw-r--   0 koh       (1000) koh       (1000)        0 2023-04-22 04:16:47.000000 omniplot-0.4.2/omniplot/scripts/__init__.py
--rw-rw-r--   0 koh       (1000) koh       (1000)      694 2023-04-22 04:16:47.000000 omniplot-0.4.2/omniplot/scripts/gff2tss.py
--rw-rw-r--   0 koh       (1000) koh       (1000)     1584 2023-04-22 04:16:47.000000 omniplot-0.4.2/omniplot/statistics.py
--rw-rw-r--   0 koh       (1000) koh       (1000)    44811 2023-04-23 08:15:37.000000 omniplot-0.4.2/omniplot/utils.py
-drwxrwxr-x   0 koh       (1000) koh       (1000)        0 2023-04-26 08:10:14.935906 omniplot-0.4.2/omniplot.egg-info/
--rw-rw-r--   0 koh       (1000) koh       (1000)      976 2023-04-26 08:10:14.000000 omniplot-0.4.2/omniplot.egg-info/PKG-INFO
--rw-rw-r--   0 koh       (1000) koh       (1000)      674 2023-04-26 08:10:14.000000 omniplot-0.4.2/omniplot.egg-info/SOURCES.txt
--rw-rw-r--   0 koh       (1000) koh       (1000)        1 2023-04-26 08:10:14.000000 omniplot-0.4.2/omniplot.egg-info/dependency_links.txt
--rw-rw-r--   0 koh       (1000) koh       (1000)      220 2023-04-26 08:10:14.000000 omniplot-0.4.2/omniplot.egg-info/requires.txt
--rw-rw-r--   0 koh       (1000) koh       (1000)        9 2023-04-26 08:10:14.000000 omniplot-0.4.2/omniplot.egg-info/top_level.txt
--rw-rw-r--   0 koh       (1000) koh       (1000)       38 2023-04-26 08:10:14.935906 omniplot-0.4.2/setup.cfg
--rw-rw-r--   0 koh       (1000) koh       (1000)     2770 2023-04-22 04:16:47.000000 omniplot-0.4.2/setup.py
-drwxrwxr-x   0 koh       (1000) koh       (1000)        0 2023-04-26 08:10:14.935906 omniplot-0.4.2/tests/
--rw-rw-r--   0 koh       (1000) koh       (1000)     4359 2023-04-22 04:16:47.000000 omniplot-0.4.2/tests/test_chipseq.py
--rw-rw-r--   0 koh       (1000) koh       (1000)     5232 2023-04-26 07:43:20.000000 omniplot-0.4.2/tests/tests heatmap.py
+drwxrwxr-x   0 koh       (1000) koh       (1000)        0 2023-04-26 10:03:04.461285 omniplot-0.4.4/
+-rw-rw-r--   0 koh       (1000) koh       (1000)    35149 2023-04-22 04:16:47.000000 omniplot-0.4.4/LICENSE
+-rw-rw-r--   0 koh       (1000) koh       (1000)      976 2023-04-26 10:03:04.461285 omniplot-0.4.4/PKG-INFO
+-rw-rw-r--   0 koh       (1000) koh       (1000)     3276 2023-04-22 04:16:47.000000 omniplot-0.4.4/README.md
+drwxrwxr-x   0 koh       (1000) koh       (1000)        0 2023-04-26 10:03:04.461285 omniplot-0.4.4/omniplot/
+-rw-rw-r--   0 koh       (1000) koh       (1000)      580 2023-04-22 04:16:47.000000 omniplot-0.4.4/omniplot/__init__.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)    21778 2023-04-22 04:16:47.000000 omniplot-0.4.4/omniplot/_adjustText.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)       21 2023-04-26 10:02:49.000000 omniplot-0.4.4/omniplot/_version.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)    57911 2023-04-22 04:16:47.000000 omniplot-0.4.4/omniplot/chipseq.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)    21857 2023-04-22 04:16:47.000000 omniplot-0.4.4/omniplot/chipseq_utils.py
+drwxrwxr-x   0 koh       (1000) koh       (1000)        0 2023-04-26 10:03:04.461285 omniplot-0.4.4/omniplot/cython_utils/
+-rw-rw-r--   0 koh       (1000) koh       (1000)        0 2023-04-22 04:16:47.000000 omniplot-0.4.4/omniplot/cython_utils/__init__.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)      288 2023-04-22 04:16:47.000000 omniplot-0.4.4/omniplot/data.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)   100746 2023-04-26 09:57:01.000000 omniplot-0.4.4/omniplot/heatmap.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)    12843 2023-04-22 04:16:47.000000 omniplot-0.4.4/omniplot/igraph_classes.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)    32121 2023-04-22 04:16:47.000000 omniplot-0.4.4/omniplot/networkplot.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)    10853 2023-04-22 05:11:17.000000 omniplot-0.4.4/omniplot/plot.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)     3511 2023-04-22 04:16:47.000000 omniplot-0.4.4/omniplot/plot_classes.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)    73070 2023-04-22 04:16:47.000000 omniplot-0.4.4/omniplot/proportion.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)    10740 2023-04-22 04:16:47.000000 omniplot-0.4.4/omniplot/regressionplot.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)   134250 2023-04-22 04:16:47.000000 omniplot-0.4.4/omniplot/scatter.py
+drwxrwxr-x   0 koh       (1000) koh       (1000)        0 2023-04-26 10:03:04.461285 omniplot-0.4.4/omniplot/scripts/
+-rw-rw-r--   0 koh       (1000) koh       (1000)        0 2023-04-22 04:16:47.000000 omniplot-0.4.4/omniplot/scripts/__init__.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)      694 2023-04-22 04:16:47.000000 omniplot-0.4.4/omniplot/scripts/gff2tss.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)     1584 2023-04-22 04:16:47.000000 omniplot-0.4.4/omniplot/statistics.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)    44811 2023-04-23 08:15:37.000000 omniplot-0.4.4/omniplot/utils.py
+drwxrwxr-x   0 koh       (1000) koh       (1000)        0 2023-04-26 10:03:04.461285 omniplot-0.4.4/omniplot.egg-info/
+-rw-rw-r--   0 koh       (1000) koh       (1000)      976 2023-04-26 10:03:04.000000 omniplot-0.4.4/omniplot.egg-info/PKG-INFO
+-rw-rw-r--   0 koh       (1000) koh       (1000)      674 2023-04-26 10:03:04.000000 omniplot-0.4.4/omniplot.egg-info/SOURCES.txt
+-rw-rw-r--   0 koh       (1000) koh       (1000)        1 2023-04-26 10:03:04.000000 omniplot-0.4.4/omniplot.egg-info/dependency_links.txt
+-rw-rw-r--   0 koh       (1000) koh       (1000)      220 2023-04-26 10:03:04.000000 omniplot-0.4.4/omniplot.egg-info/requires.txt
+-rw-rw-r--   0 koh       (1000) koh       (1000)        9 2023-04-26 10:03:04.000000 omniplot-0.4.4/omniplot.egg-info/top_level.txt
+-rw-rw-r--   0 koh       (1000) koh       (1000)       38 2023-04-26 10:03:04.461285 omniplot-0.4.4/setup.cfg
+-rw-rw-r--   0 koh       (1000) koh       (1000)     2770 2023-04-22 04:16:47.000000 omniplot-0.4.4/setup.py
+drwxrwxr-x   0 koh       (1000) koh       (1000)        0 2023-04-26 10:03:04.461285 omniplot-0.4.4/tests/
+-rw-rw-r--   0 koh       (1000) koh       (1000)     4359 2023-04-22 04:16:47.000000 omniplot-0.4.4/tests/test_chipseq.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)     5232 2023-04-26 07:43:20.000000 omniplot-0.4.4/tests/tests heatmap.py
```

### Comparing `omniplot-0.4.2/LICENSE` & `omniplot-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `omniplot-0.4.2/PKG-INFO` & `omniplot-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omniplot
-Version: 0.4.2
+Version: 0.4.4
 Summary: To draw scientific plots easily
 Home-page: https://github.com/koonimaru/omniplot
 Author: Koh Onimaru
 Author-email: koh.onimaru@gmail.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
```

### Comparing `omniplot-0.4.2/README.md` & `omniplot-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `omniplot-0.4.2/omniplot/__init__.py` & `omniplot-0.4.4/omniplot/__init__.py`

 * *Files identical despite different names*

### Comparing `omniplot-0.4.2/omniplot/_adjustText.py` & `omniplot-0.4.4/omniplot/_adjustText.py`

 * *Files identical despite different names*

### Comparing `omniplot-0.4.2/omniplot/chipseq.py` & `omniplot-0.4.4/omniplot/chipseq.py`

 * *Files identical despite different names*

### Comparing `omniplot-0.4.2/omniplot/chipseq_utils.py` & `omniplot-0.4.4/omniplot/chipseq_utils.py`

 * *Files identical despite different names*

### Comparing `omniplot-0.4.2/omniplot/heatmap.py` & `omniplot-0.4.4/omniplot/heatmap.py`

 * *Files 2% similar despite different names*

```diff
@@ -1488,15 +1488,15 @@
             if len(shape_colors)>0:
                 scX=scX[sortindexr]
         elif clustering_method=="kmeans":
             _kmeans = KMeans(n_clusters=approx_clusternum, random_state=0, n_init="auto").fit(X, *kmeans_kw)
             row_colors["kmeans_row"]=_kmeans.labels_.astype(str)
             sortindexr=np.lexsort((X.mean(axis=1),_kmeans.labels_))
             X=X[sortindexr]
-            if type(Xsize)!=None:
+            if type(Xsize)!=type(None):
                 Xsize=Xsize[sortindexr]
             if len(shape_colors)>0:
                 scX=scX[sortindexr]
             rowlabels=rowlabels[sortindexr]
             _klabels=_kmeans.labels_[sortindexr]
             for i, (kclass, label) in enumerate(zip(_klabels, rowlabels)):
                 if not kclass in rclusters:
@@ -1510,15 +1510,15 @@
                 pip(['install', '--user', 'kmodes'])
                 from kmodes.kmodes import KModes
             km = KModes(n_clusters=3, init='Huang', n_init=5, verbose=1)
             clusters = km.fit_predict(X)
             row_colors["kmodes_row"]=clusters.astype(str)
             sortindexr=np.argsort(clusters)
             X=X[sortindexr]
-            if type(Xsize)!=None:
+            if type(Xsize)!=type(None):
                 Xsize=Xsize[sortindexr]
 
             if len(shape_colors)>0:
                 scX=scX[sortindexr]
             rowlabels=rowlabels[sortindexr]
             _klabels=clusters[sortindexr]
             for i, (kclass, label) in enumerate(zip(_klabels, rowlabels)):
@@ -1545,15 +1545,15 @@
                 scX=scX[:, sortindexc]
             ax_dict["toptree"]=ax1
         elif clustering_method=="kmeans":
             _ckmeans = KMeans(n_clusters=approx_clusternum, random_state=0, n_init="auto").fit(X.T, *kmeans_kw)
             col_colors["kmeans_column"]=_ckmeans.labels_.astype(str)
             sortindexc=np.lexsort((X.mean(axis=0),_ckmeans.labels_))
             X=X[:,sortindexc]
-            if type(Xsize)!=None:
+            if type(Xsize)!=type(None):
                 Xsize=Xsize[:, sortindexc]
 
             if len(shape_colors)>0:
                 scX=scX[:, sortindexc]
 
             collabels=collabels[sortindexc]
             _cklabels=_ckmeans.labels_[sortindexc]
@@ -1569,15 +1569,15 @@
                 pip(['install', '--user', 'kmodes'])
                 from kmodes.kmodes import KModes
             km = KModes(n_clusters=3, init='Huang', n_init=5, verbose=1)
             clustersc = km.fit_predict(X.T)
             col_colors["kmodes_column"]=clustersc.astype(str)
             sortindexc=np.argsort(clustersc)
             X=X[:, sortindexc]
-            if type(Xsize)!=None:
+            if type(Xsize)!=type(None):
                 Xsize=Xsize[:, sortindexc]
 
             if len(shape_colors)>0:
                 scX=scX[:, sortindexc]
             collabels=collabels[sortindexc]
             _cklabels=clustersc[sortindexc]
             # print(_cklabels,collabels )
```

### Comparing `omniplot-0.4.2/omniplot/igraph_classes.py` & `omniplot-0.4.4/omniplot/igraph_classes.py`

 * *Files identical despite different names*

### Comparing `omniplot-0.4.2/omniplot/networkplot.py` & `omniplot-0.4.4/omniplot/networkplot.py`

 * *Files identical despite different names*

### Comparing `omniplot-0.4.2/omniplot/plot.py` & `omniplot-0.4.4/omniplot/plot.py`

 * *Files identical despite different names*

### Comparing `omniplot-0.4.2/omniplot/plot_classes.py` & `omniplot-0.4.4/omniplot/plot_classes.py`

 * *Files identical despite different names*

### Comparing `omniplot-0.4.2/omniplot/proportion.py` & `omniplot-0.4.4/omniplot/proportion.py`

 * *Files identical despite different names*

### Comparing `omniplot-0.4.2/omniplot/regressionplot.py` & `omniplot-0.4.4/omniplot/regressionplot.py`

 * *Files identical despite different names*

### Comparing `omniplot-0.4.2/omniplot/scatter.py` & `omniplot-0.4.4/omniplot/scatter.py`

 * *Files identical despite different names*

### Comparing `omniplot-0.4.2/omniplot/scripts/gff2tss.py` & `omniplot-0.4.4/omniplot/scripts/gff2tss.py`

 * *Files identical despite different names*

### Comparing `omniplot-0.4.2/omniplot/statistics.py` & `omniplot-0.4.4/omniplot/statistics.py`

 * *Files identical despite different names*

### Comparing `omniplot-0.4.2/omniplot/utils.py` & `omniplot-0.4.4/omniplot/utils.py`

 * *Files identical despite different names*

### Comparing `omniplot-0.4.2/omniplot.egg-info/PKG-INFO` & `omniplot-0.4.4/omniplot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omniplot
-Version: 0.4.2
+Version: 0.4.4
 Summary: To draw scientific plots easily
 Home-page: https://github.com/koonimaru/omniplot
 Author: Koh Onimaru
 Author-email: koh.onimaru@gmail.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
```

### Comparing `omniplot-0.4.2/omniplot.egg-info/SOURCES.txt` & `omniplot-0.4.4/omniplot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `omniplot-0.4.2/setup.py` & `omniplot-0.4.4/setup.py`

 * *Files identical despite different names*

### Comparing `omniplot-0.4.2/tests/test_chipseq.py` & `omniplot-0.4.4/tests/test_chipseq.py`

 * *Files identical despite different names*

### Comparing `omniplot-0.4.2/tests/tests heatmap.py` & `omniplot-0.4.4/tests/tests heatmap.py`

 * *Files identical despite different names*

