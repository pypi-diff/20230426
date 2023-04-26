# Comparing `tmp/multitax-1.3.0.tar.gz` & `tmp/multitax-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multitax-1.3.0.tar", last modified: Thu Mar 30 15:45:09 2023, max compression
+gzip compressed data, was "multitax-1.3.1.tar", last modified: Wed Apr 26 09:37:27 2023, max compression
```

## Comparing `multitax-1.3.0.tar` & `multitax-1.3.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 pirov    (258448) mi_agabi (10748)        0 2023-03-30 15:45:09.201500 multitax-1.3.0/
--rw-r--r--   0 pirov    (258448) mi_agabi (10748)     1089 2022-04-19 06:51:53.000000 multitax-1.3.0/LICENSE
--rw-r--r--   0 pirov    (258448) mi_agabi (10748)    11111 2023-03-30 15:45:09.201500 multitax-1.3.0/PKG-INFO
--rw-r--r--   0 pirov    (258448) mi_agabi (10748)    10450 2023-03-30 15:44:56.000000 multitax-1.3.0/README.md
-drwxr-xr-x   0 pirov    (258448) mi_agabi (10748)        0 2023-03-30 15:45:09.197500 multitax-1.3.0/multitax/
--rw-r--r--   0 pirov    (258448) mi_agabi (10748)      352 2023-03-30 15:44:56.000000 multitax-1.3.0/multitax/__init__.py
--rw-r--r--   0 pirov    (258448) mi_agabi (10748)     2527 2023-03-30 15:44:56.000000 multitax-1.3.0/multitax/customtx.py
--rw-r--r--   0 pirov    (258448) mi_agabi (10748)      435 2023-03-30 15:44:56.000000 multitax-1.3.0/multitax/dummytx.py
--rw-r--r--   0 pirov    (258448) mi_agabi (10748)     2247 2023-03-30 15:44:56.000000 multitax-1.3.0/multitax/greengenestx.py
--rw-r--r--   0 pirov    (258448) mi_agabi (10748)     5394 2023-03-30 15:44:56.000000 multitax-1.3.0/multitax/gtdbtx.py
--rw-r--r--   0 pirov    (258448) mi_agabi (10748)    25572 2023-03-30 15:44:56.000000 multitax-1.3.0/multitax/multitax.py
--rw-r--r--   0 pirov    (258448) mi_agabi (10748)     8758 2023-03-30 15:44:56.000000 multitax-1.3.0/multitax/ncbitx.py
--rw-r--r--   0 pirov    (258448) mi_agabi (10748)     5466 2023-03-30 15:44:56.000000 multitax-1.3.0/multitax/otttx.py
--rw-r--r--   0 pirov    (258448) mi_agabi (10748)     1904 2023-03-30 15:44:56.000000 multitax-1.3.0/multitax/silvatx.py
--rw-r--r--   0 pirov    (258448) mi_agabi (10748)     4966 2023-03-30 15:44:56.000000 multitax-1.3.0/multitax/utils.py
-drwxr-xr-x   0 pirov    (258448) mi_agabi (10748)        0 2023-03-30 15:45:09.201500 multitax-1.3.0/multitax.egg-info/
--rw-r--r--   0 pirov    (258448) mi_agabi (10748)    11111 2023-03-30 15:45:09.000000 multitax-1.3.0/multitax.egg-info/PKG-INFO
--rw-r--r--   0 pirov    (258448) mi_agabi (10748)      371 2023-03-30 15:45:09.000000 multitax-1.3.0/multitax.egg-info/SOURCES.txt
--rw-r--r--   0 pirov    (258448) mi_agabi (10748)        1 2023-03-30 15:45:09.000000 multitax-1.3.0/multitax.egg-info/dependency_links.txt
--rw-r--r--   0 pirov    (258448) mi_agabi (10748)        9 2023-03-30 15:45:09.000000 multitax-1.3.0/multitax.egg-info/top_level.txt
--rw-r--r--   0 pirov    (258448) mi_agabi (10748)      103 2022-04-12 11:54:24.000000 multitax-1.3.0/pyproject.toml
--rw-r--r--   0 pirov    (258448) mi_agabi (10748)       38 2023-03-30 15:45:09.201500 multitax-1.3.0/setup.cfg
--rwxr-xr-x   0 pirov    (258448) mi_agabi (10748)      907 2023-03-30 15:44:56.000000 multitax-1.3.0/setup.py
+drwxr-xr-x   0 pirov    (258448) mi_agabi (10748)        0 2023-04-26 09:37:27.753162 multitax-1.3.1/
+-rw-r--r--   0 pirov    (258448) mi_agabi (10748)     1089 2022-04-19 06:51:53.000000 multitax-1.3.1/LICENSE
+-rw-r--r--   0 pirov    (258448) mi_agabi (10748)    11111 2023-04-26 09:37:27.753162 multitax-1.3.1/PKG-INFO
+-rw-r--r--   0 pirov    (258448) mi_agabi (10748)    10450 2023-03-30 15:44:56.000000 multitax-1.3.1/README.md
+drwxr-xr-x   0 pirov    (258448) mi_agabi (10748)        0 2023-04-26 09:37:27.753162 multitax-1.3.1/multitax/
+-rw-r--r--   0 pirov    (258448) mi_agabi (10748)      352 2023-04-26 08:50:39.000000 multitax-1.3.1/multitax/__init__.py
+-rw-r--r--   0 pirov    (258448) mi_agabi (10748)     2527 2023-03-30 15:44:56.000000 multitax-1.3.1/multitax/customtx.py
+-rw-r--r--   0 pirov    (258448) mi_agabi (10748)      435 2023-03-30 15:44:56.000000 multitax-1.3.1/multitax/dummytx.py
+-rw-r--r--   0 pirov    (258448) mi_agabi (10748)     2247 2023-03-30 15:44:56.000000 multitax-1.3.1/multitax/greengenestx.py
+-rw-r--r--   0 pirov    (258448) mi_agabi (10748)     5394 2023-03-30 15:44:56.000000 multitax-1.3.1/multitax/gtdbtx.py
+-rw-r--r--   0 pirov    (258448) mi_agabi (10748)    25426 2023-04-26 09:15:44.000000 multitax-1.3.1/multitax/multitax.py
+-rw-r--r--   0 pirov    (258448) mi_agabi (10748)     8758 2023-03-30 15:44:56.000000 multitax-1.3.1/multitax/ncbitx.py
+-rw-r--r--   0 pirov    (258448) mi_agabi (10748)     5466 2023-03-30 15:44:56.000000 multitax-1.3.1/multitax/otttx.py
+-rw-r--r--   0 pirov    (258448) mi_agabi (10748)     1904 2023-03-30 15:44:56.000000 multitax-1.3.1/multitax/silvatx.py
+-rw-r--r--   0 pirov    (258448) mi_agabi (10748)     4966 2023-03-30 15:44:56.000000 multitax-1.3.1/multitax/utils.py
+drwxr-xr-x   0 pirov    (258448) mi_agabi (10748)        0 2023-04-26 09:37:27.753162 multitax-1.3.1/multitax.egg-info/
+-rw-r--r--   0 pirov    (258448) mi_agabi (10748)    11111 2023-04-26 09:37:27.000000 multitax-1.3.1/multitax.egg-info/PKG-INFO
+-rw-r--r--   0 pirov    (258448) mi_agabi (10748)      371 2023-04-26 09:37:27.000000 multitax-1.3.1/multitax.egg-info/SOURCES.txt
+-rw-r--r--   0 pirov    (258448) mi_agabi (10748)        1 2023-04-26 09:37:27.000000 multitax-1.3.1/multitax.egg-info/dependency_links.txt
+-rw-r--r--   0 pirov    (258448) mi_agabi (10748)        9 2023-04-26 09:37:27.000000 multitax-1.3.1/multitax.egg-info/top_level.txt
+-rw-r--r--   0 pirov    (258448) mi_agabi (10748)      103 2022-04-12 11:54:24.000000 multitax-1.3.1/pyproject.toml
+-rw-r--r--   0 pirov    (258448) mi_agabi (10748)       38 2023-04-26 09:37:27.753162 multitax-1.3.1/setup.cfg
+-rwxr-xr-x   0 pirov    (258448) mi_agabi (10748)      907 2023-04-26 09:24:00.000000 multitax-1.3.1/setup.py
```

### Comparing `multitax-1.3.0/LICENSE` & `multitax-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `multitax-1.3.0/PKG-INFO` & `multitax-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multitax
-Version: 1.3.0
+Version: 1.3.1
 Summary: Python package to obtain, parse and explore biological and custom taxonomies
 Home-page: https://www.github.com/pirovc/multitax
 Author: Vitor C. Piro
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
```

### Comparing `multitax-1.3.0/README.md` & `multitax-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `multitax-1.3.0/multitax/customtx.py` & `multitax-1.3.1/multitax/customtx.py`

 * *Files identical despite different names*

### Comparing `multitax-1.3.0/multitax/greengenestx.py` & `multitax-1.3.1/multitax/greengenestx.py`

 * *Files identical despite different names*

### Comparing `multitax-1.3.0/multitax/gtdbtx.py` & `multitax-1.3.1/multitax/gtdbtx.py`

 * *Files identical despite different names*

### Comparing `multitax-1.3.0/multitax/multitax.py` & `multitax-1.3.1/multitax/multitax.py`

 * *Files 0% similar despite different names*

```diff
@@ -361,27 +361,23 @@
             tax = GtdbTx()
             # Keep only descendants of 'g__Enterovibrio'
             tax.filter('g__Enterovibrio', desc=True)
         """
         if isinstance(nodes, str):
             nodes = [nodes]
 
-        # Cannot filter root node
-        if self.root_node in nodes:
-            raise ValueError("Root node [" + self.root_node + "] cannot be filtered.")
-
         # Keep track of nodes to be filtered out
         filtered_nodes = set(self._nodes)
         # Always keep root
         filtered_nodes.discard(self.root_node)
 
         if desc:
             # Keep descendants of the given nodes
             for node in nodes:
-                # Check if node exists
+                # Check if node exists (skips root)
                 if node in filtered_nodes:
                     # For each leaf of the selected nodes
                     for leaf in self.leaves(node):
                         # Build lineage of each leaf up-to node itself
                         for n in self.lineage(leaf, root_node=node):
                             # Discard nodes from set to be kept
                             filtered_nodes.discard(n)
@@ -397,15 +393,14 @@
 
         # Delete filtered nodes
         for node in filtered_nodes:
             self._remove(node)
 
         # Delete aux. data structures
         self._reset_aux_data()
-
         self.check_consistency()
 
     def latest(self, node: str):
         """
         Returns latest/updated version of a given node.
         If node is already the latests, returns itself.
         Mainly used for NCBI (merged.dmp) and OTT (forwards.tsv)
```

### Comparing `multitax-1.3.0/multitax/ncbitx.py` & `multitax-1.3.1/multitax/ncbitx.py`

 * *Files identical despite different names*

### Comparing `multitax-1.3.0/multitax/otttx.py` & `multitax-1.3.1/multitax/otttx.py`

 * *Files identical despite different names*

### Comparing `multitax-1.3.0/multitax/silvatx.py` & `multitax-1.3.1/multitax/silvatx.py`

 * *Files identical despite different names*

### Comparing `multitax-1.3.0/multitax/utils.py` & `multitax-1.3.1/multitax/utils.py`

 * *Files identical despite different names*

### Comparing `multitax-1.3.0/multitax.egg-info/PKG-INFO` & `multitax-1.3.1/multitax.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multitax
-Version: 1.3.0
+Version: 1.3.1
 Summary: Python package to obtain, parse and explore biological and custom taxonomies
 Home-page: https://www.github.com/pirovc/multitax
 Author: Vitor C. Piro
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
```

### Comparing `multitax-1.3.0/setup.py` & `multitax-1.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="multitax",
-    version="1.3.0",
+    version="1.3.1",
     url="https://www.github.com/pirovc/multitax",
     license="MIT",
     author="Vitor C. Piro",
     description="Python package to obtain, parse and explore biological and custom taxonomies",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=["multitax"],
```

