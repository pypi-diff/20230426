# Comparing `tmp/numpy3-0.1.tar.gz` & `tmp/numpy3-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numpy3-0.1.tar", last modified: Wed Apr 26 18:19:20 2023, max compression
+gzip compressed data, was "numpy3-0.2.tar", last modified: Wed Apr 26 18:24:29 2023, max compression
```

## Comparing `numpy3-0.1.tar` & `numpy3-0.2.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 18:19:20.202861 numpy3-0.1/
--rw-rw-rw-   0        0        0      211 2023-04-26 18:19:20.196832 numpy3-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-26 18:19:20.136491 numpy3-0.1/numpy3/
--rw-rw-rw-   0        0        0     4913 2023-04-25 05:16:48.000000 numpy3-0.1/numpy3/Astar.py
--rw-rw-rw-   0        0        0     2810 2023-04-24 15:11:51.000000 numpy3-0.1/numpy3/BFS.py
--rw-rw-rw-   0        0        0     2230 2023-04-25 09:48:21.000000 numpy3-0.1/numpy3/DFID.py
--rw-rw-rw-   0        0        0     2082 2023-04-24 15:15:40.000000 numpy3-0.1/numpy3/DFS.py
--rw-rw-rw-   0        0        0     3425 2023-04-25 09:10:07.000000 numpy3-0.1/numpy3/Genetic.py
--rw-rw-rw-   0        0        0     3614 2023-04-26 17:59:17.000000 numpy3-0.1/numpy3/Hill_Climbing.py
--rw-rw-rw-   0        0        0     2158 2023-04-26 17:48:41.000000 numpy3-0.1/numpy3/Simulated_Annealing.py
--rw-rw-rw-   0        0        0     2842 2023-04-25 07:58:00.000000 numpy3-0.1/numpy3/UCS.py
--rw-rw-rw-   0        0        0        0 2023-04-26 18:17:37.000000 numpy3-0.1/numpy3/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-26 18:19:20.193309 numpy3-0.1/numpy3.egg-info/
--rw-rw-rw-   0        0        0      211 2023-04-26 18:19:19.000000 numpy3-0.1/numpy3.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2023-04-26 18:19:19.000000 numpy3-0.1/numpy3.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 18:19:19.000000 numpy3-0.1/numpy3.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-26 18:19:19.000000 numpy3-0.1/numpy3.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-26 18:19:20.203860 numpy3-0.1/setup.cfg
--rw-rw-rw-   0        0        0      219 2023-04-26 18:18:24.000000 numpy3-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 18:24:29.494621 numpy3-0.2/
+-rw-rw-rw-   0        0        0      211 2023-04-26 18:24:29.493625 numpy3-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-26 18:24:29.448901 numpy3-0.2/numpy3/
+-rw-rw-rw-   0        0        0     4913 2023-04-25 05:16:48.000000 numpy3-0.2/numpy3/Astar.py
+-rw-rw-rw-   0        0        0     2810 2023-04-24 15:11:51.000000 numpy3-0.2/numpy3/BFS.py
+-rw-rw-rw-   0        0        0     2230 2023-04-25 09:48:21.000000 numpy3-0.2/numpy3/DFID.py
+-rw-rw-rw-   0        0        0     2082 2023-04-24 15:15:40.000000 numpy3-0.2/numpy3/DFS.py
+-rw-rw-rw-   0        0        0     1648 2023-04-26 18:23:03.000000 numpy3-0.2/numpy3/DFS2.py
+-rw-rw-rw-   0        0        0     3425 2023-04-25 09:10:07.000000 numpy3-0.2/numpy3/Genetic.py
+-rw-rw-rw-   0        0        0     3614 2023-04-26 17:59:17.000000 numpy3-0.2/numpy3/Hill_Climbing.py
+-rw-rw-rw-   0        0        0     2158 2023-04-26 17:48:41.000000 numpy3-0.2/numpy3/Simulated_Annealing.py
+-rw-rw-rw-   0        0        0     2842 2023-04-25 07:58:00.000000 numpy3-0.2/numpy3/UCS.py
+-rw-rw-rw-   0        0        0        0 2023-04-26 18:17:37.000000 numpy3-0.2/numpy3/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 18:24:29.491619 numpy3-0.2/numpy3.egg-info/
+-rw-rw-rw-   0        0        0      211 2023-04-26 18:24:29.000000 numpy3-0.2/numpy3.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2023-04-26 18:24:29.000000 numpy3-0.2/numpy3.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 18:24:29.000000 numpy3-0.2/numpy3.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-26 18:24:29.000000 numpy3-0.2/numpy3.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-26 18:24:29.494621 numpy3-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      219 2023-04-26 18:22:35.000000 numpy3-0.2/setup.py
```

### Comparing `numpy3-0.1/numpy3/Astar.py` & `numpy3-0.2/numpy3/Astar.py`

 * *Files identical despite different names*

### Comparing `numpy3-0.1/numpy3/BFS.py` & `numpy3-0.2/numpy3/BFS.py`

 * *Files identical despite different names*

### Comparing `numpy3-0.1/numpy3/DFID.py` & `numpy3-0.2/numpy3/DFID.py`

 * *Files identical despite different names*

### Comparing `numpy3-0.1/numpy3/DFS.py` & `numpy3-0.2/numpy3/DFS.py`

 * *Files identical despite different names*

### Comparing `numpy3-0.1/numpy3/Genetic.py` & `numpy3-0.2/numpy3/Genetic.py`

 * *Files identical despite different names*

### Comparing `numpy3-0.1/numpy3/Hill_Climbing.py` & `numpy3-0.2/numpy3/Hill_Climbing.py`

 * *Files identical despite different names*

### Comparing `numpy3-0.1/numpy3/Simulated_Annealing.py` & `numpy3-0.2/numpy3/Simulated_Annealing.py`

 * *Files identical despite different names*

### Comparing `numpy3-0.1/numpy3/UCS.py` & `numpy3-0.2/numpy3/UCS.py`

 * *Files identical despite different names*

