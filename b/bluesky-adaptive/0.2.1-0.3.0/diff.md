# Comparing `tmp/bluesky-adaptive-0.2.1.tar.gz` & `tmp/bluesky-adaptive-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bluesky-adaptive-0.2.1.tar", last modified: Fri Oct 29 19:18:42 2021, max compression
+gzip compressed data, was "bluesky-adaptive-0.3.0.tar", last modified: Wed Apr 26 18:31:54 2023, max compression
```

## Comparing `bluesky-adaptive-0.2.1.tar` & `bluesky-adaptive-0.3.0.tar`

### file list

```diff
@@ -1,44 +1,70 @@
-drwxr-xr-x   0 joshualynch   (503) staff       (20)        0 2021-10-29 19:18:41.999759 bluesky-adaptive-0.2.1/
--rw-r--r--   0 joshualynch   (503) staff       (20)      168 2021-10-29 19:12:00.000000 bluesky-adaptive-0.2.1/AUTHORS.rst
--rw-r--r--   0 joshualynch   (503) staff       (20)     3122 2021-10-29 19:12:00.000000 bluesky-adaptive-0.2.1/CONTRIBUTING.rst
--rw-r--r--   0 joshualynch   (503) staff       (20)     1515 2021-10-29 19:12:00.000000 bluesky-adaptive-0.2.1/LICENSE
--rw-r--r--   0 joshualynch   (503) staff       (20)      369 2021-10-29 19:12:00.000000 bluesky-adaptive-0.2.1/MANIFEST.in
--rw-r--r--   0 joshualynch   (503) staff       (20)      941 2021-10-29 19:18:41.999863 bluesky-adaptive-0.2.1/PKG-INFO
--rw-r--r--   0 joshualynch   (503) staff       (20)      489 2021-10-29 19:12:00.000000 bluesky-adaptive-0.2.1/README.rst
-drwxr-xr-x   0 joshualynch   (503) staff       (20)        0 2021-10-29 19:18:42.000672 bluesky-adaptive-0.2.1/bluesky_adaptive/
--rw-r--r--   0 joshualynch   (503) staff       (20)       93 2021-10-29 19:12:00.000000 bluesky-adaptive-0.2.1/bluesky_adaptive/__init__.py
--rw-r--r--   0 joshualynch   (503) staff       (20)      497 2021-10-29 19:18:42.000747 bluesky-adaptive-0.2.1/bluesky_adaptive/_version.py
--rw-r--r--   0 joshualynch   (503) staff       (20)     6466 2021-10-29 19:12:00.000000 bluesky-adaptive-0.2.1/bluesky_adaptive/on_stop.py
--rw-r--r--   0 joshualynch   (503) staff       (20)     5871 2021-10-29 19:12:00.000000 bluesky-adaptive-0.2.1/bluesky_adaptive/per_event.py
--rw-r--r--   0 joshualynch   (503) staff       (20)     6346 2021-10-29 19:12:00.000000 bluesky-adaptive-0.2.1/bluesky_adaptive/per_start.py
--rw-r--r--   0 joshualynch   (503) staff       (20)     1496 2021-10-29 19:12:00.000000 bluesky-adaptive-0.2.1/bluesky_adaptive/recommendations.py
--rw-r--r--   0 joshualynch   (503) staff       (20)     2317 2021-10-29 19:12:00.000000 bluesky-adaptive-0.2.1/bluesky_adaptive/scipy_reccomendations.py
-drwxr-xr-x   0 joshualynch   (503) staff       (20)        0 2021-10-29 19:18:41.994778 bluesky-adaptive-0.2.1/bluesky_adaptive/tests/
--rw-r--r--   0 joshualynch   (503) staff       (20)        0 2021-10-29 19:12:00.000000 bluesky-adaptive-0.2.1/bluesky_adaptive/tests/__init__.py
--rw-r--r--   0 joshualynch   (503) staff       (20)       90 2021-10-29 19:12:00.000000 bluesky-adaptive-0.2.1/bluesky_adaptive/tests/conftest.py
--rw-r--r--   0 joshualynch   (503) staff       (20)      643 2021-10-29 19:12:00.000000 bluesky-adaptive-0.2.1/bluesky_adaptive/tests/test_per_event.py
--rw-r--r--   0 joshualynch   (503) staff       (20)      907 2021-10-29 19:12:00.000000 bluesky-adaptive-0.2.1/bluesky_adaptive/tests/test_per_start.py
--rw-r--r--   0 joshualynch   (503) staff       (20)     1107 2021-10-29 19:12:00.000000 bluesky-adaptive-0.2.1/bluesky_adaptive/tests/test_scipy_rec.py
--rw-r--r--   0 joshualynch   (503) staff       (20)     2605 2021-10-29 19:12:00.000000 bluesky-adaptive-0.2.1/bluesky_adaptive/utils.py
-drwxr-xr-x   0 joshualynch   (503) staff       (20)        0 2021-10-29 19:18:41.993032 bluesky-adaptive-0.2.1/bluesky_adaptive.egg-info/
--rw-r--r--   0 joshualynch   (503) staff       (20)      941 2021-10-29 19:18:41.000000 bluesky-adaptive-0.2.1/bluesky_adaptive.egg-info/PKG-INFO
--rw-r--r--   0 joshualynch   (503) staff       (20)     1001 2021-10-29 19:18:41.000000 bluesky-adaptive-0.2.1/bluesky_adaptive.egg-info/SOURCES.txt
--rw-r--r--   0 joshualynch   (503) staff       (20)        1 2021-10-29 19:18:41.000000 bluesky-adaptive-0.2.1/bluesky_adaptive.egg-info/dependency_links.txt
--rw-r--r--   0 joshualynch   (503) staff       (20)       20 2021-10-29 19:18:41.000000 bluesky-adaptive-0.2.1/bluesky_adaptive.egg-info/entry_points.txt
--rw-r--r--   0 joshualynch   (503) staff       (20)       43 2021-10-29 19:18:41.000000 bluesky-adaptive-0.2.1/bluesky_adaptive.egg-info/requires.txt
--rw-r--r--   0 joshualynch   (503) staff       (20)       17 2021-10-29 19:18:41.000000 bluesky-adaptive-0.2.1/bluesky_adaptive.egg-info/top_level.txt
-drwxr-xr-x   0 joshualynch   (503) staff       (20)        0 2021-10-29 19:18:41.995799 bluesky-adaptive-0.2.1/docs/
--rw-r--r--   0 joshualynch   (503) staff       (20)      783 2021-10-29 19:12:00.000000 bluesky-adaptive-0.2.1/docs/Makefile
--rw-r--r--   0 joshualynch   (503) staff       (20)      797 2021-10-29 19:12:00.000000 bluesky-adaptive-0.2.1/docs/make.bat
-drwxr-xr-x   0 joshualynch   (503) staff       (20)        0 2021-10-29 19:18:41.999422 bluesky-adaptive-0.2.1/docs/source/
--rw-r--r--   0 joshualynch   (503) staff       (20)     6660 2021-10-29 19:12:00.000000 bluesky-adaptive-0.2.1/docs/source/conf.py
--rw-r--r--   0 joshualynch   (503) staff       (20)    11025 2021-10-29 19:12:00.000000 bluesky-adaptive-0.2.1/docs/source/examples.rst
--rw-r--r--   0 joshualynch   (503) staff       (20)    11873 2021-10-29 19:12:00.000000 bluesky-adaptive-0.2.1/docs/source/index.rst
--rw-r--r--   0 joshualynch   (503) staff       (20)       98 2021-10-29 19:12:00.000000 bluesky-adaptive-0.2.1/docs/source/installation.rst
--rw-r--r--   0 joshualynch   (503) staff       (20)     1083 2021-10-29 19:12:00.000000 bluesky-adaptive-0.2.1/docs/source/min_versions.rst
--rw-r--r--   0 joshualynch   (503) staff       (20)      258 2021-10-29 19:12:00.000000 bluesky-adaptive-0.2.1/docs/source/release-history.rst
--rw-r--r--   0 joshualynch   (503) staff       (20)      109 2021-10-29 19:12:00.000000 bluesky-adaptive-0.2.1/docs/source/usage.rst
--rw-r--r--   0 joshualynch   (503) staff       (20)       97 2021-10-29 19:12:00.000000 bluesky-adaptive-0.2.1/requirements.txt
--rw-r--r--   0 joshualynch   (503) staff       (20)      196 2021-10-29 19:18:42.000256 bluesky-adaptive-0.2.1/setup.cfg
--rw-r--r--   0 joshualynch   (503) staff       (20)     2169 2021-10-29 19:12:00.000000 bluesky-adaptive-0.2.1/setup.py
--rw-r--r--   0 joshualynch   (503) staff       (20)    68611 2021-10-29 19:12:00.000000 bluesky-adaptive-0.2.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:31:54.060794 bluesky-adaptive-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-26 18:31:54.060794 bluesky-adaptive-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:31:54.060794 bluesky-adaptive-0.3.0/bluesky_adaptive/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/bluesky_adaptive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-26 18:31:54.060794 bluesky-adaptive-0.3.0/bluesky_adaptive/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:31:54.056794 bluesky-adaptive-0.3.0/bluesky_adaptive/adjudicators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/bluesky_adaptive/adjudicators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9768 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/bluesky_adaptive/adjudicators/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/bluesky_adaptive/adjudicators/msg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:31:54.056794 bluesky-adaptive-0.3.0/bluesky_adaptive/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/bluesky_adaptive/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43242 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/bluesky_adaptive/agents/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7194 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/bluesky_adaptive/agents/botorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/bluesky_adaptive/agents/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8416 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/bluesky_adaptive/agents/sklearn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6312 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/bluesky_adaptive/on_stop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/bluesky_adaptive/per_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/bluesky_adaptive/per_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/bluesky_adaptive/recommendations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/bluesky_adaptive/scipy_reccomendations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:31:54.056794 bluesky-adaptive-0.3.0/bluesky_adaptive/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/bluesky_adaptive/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19733 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/bluesky_adaptive/server/comms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7342 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/bluesky_adaptive/server/ioc_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/bluesky_adaptive/server/logging_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/bluesky_adaptive/server/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/bluesky_adaptive/server/server_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/bluesky_adaptive/server/server_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13531 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/bluesky_adaptive/server/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16060 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/bluesky_adaptive/server/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:31:54.060794 bluesky-adaptive-0.3.0/bluesky_adaptive/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/bluesky_adaptive/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/bluesky_adaptive/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12302 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/bluesky_adaptive/tests/test_adjudicators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15155 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/bluesky_adaptive/tests/test_agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/bluesky_adaptive/tests/test_botorch_agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/bluesky_adaptive/tests/test_kafka.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/bluesky_adaptive/tests/test_per_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/bluesky_adaptive/tests/test_per_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/bluesky_adaptive/tests/test_scipy_rec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9571 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/bluesky_adaptive/tests/test_sklearn_agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/bluesky_adaptive/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:31:54.056794 bluesky-adaptive-0.3.0/bluesky_adaptive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-26 18:31:54.000000 bluesky-adaptive-0.3.0/bluesky_adaptive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-04-26 18:31:54.000000 bluesky-adaptive-0.3.0/bluesky_adaptive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 18:31:54.000000 bluesky-adaptive-0.3.0/bluesky_adaptive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-26 18:31:54.000000 bluesky-adaptive-0.3.0/bluesky_adaptive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-26 18:31:54.000000 bluesky-adaptive-0.3.0/bluesky_adaptive.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:31:54.060794 bluesky-adaptive-0.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:31:54.060794 bluesky-adaptive-0.3.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     6667 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9899 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/docs/source/distributed.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11025 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/docs/source/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13358 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/docs/source/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/docs/source/min_versions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/docs/source/release-history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/docs/source/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-26 18:31:54.060794 bluesky-adaptive-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68576 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/versioneer.py
```

### Comparing `bluesky-adaptive-0.2.1/CONTRIBUTING.rst` & `bluesky-adaptive-0.3.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `bluesky-adaptive-0.2.1/LICENSE` & `bluesky-adaptive-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bluesky-adaptive-0.2.1/PKG-INFO` & `bluesky-adaptive-0.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: bluesky-adaptive
-Version: 0.2.1
+Version: 0.3.0
 Summary: Tools for writing adaptive plans
 Home-page: https://github.com/bluesky/bluesky-adaptive
 Author: NSLS-II
 Author-email: dama@bnl.gov
 License: BSD (3-clause)
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
+Provides-Extra: agents
+Provides-Extra: all
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 ================
 bluesky-adaptive
 ================
 
@@ -30,9 +31,7 @@
 * Free software: 3-clause BSD license
 * Documentation: (COMING SOON!) https://bluesky.github.io/bluesky-adaptive.
 
 Features
 --------
 
 * TODO
-
-
```

### Comparing `bluesky-adaptive-0.2.1/bluesky_adaptive/on_stop.py` & `bluesky-adaptive-0.3.0/bluesky_adaptive/on_stop.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,22 +10,21 @@
 dictates.
 
 This corresponds to a "middle" scale of adaptive integration into
 data collection.
 """
 from queue import Queue
 
-from .recommendations import NoRecommendation
-
+import event_model
 from bluesky_live.bluesky_run import BlueskyRun, DocumentCache
 from bluesky_widgets.models.utils import call_or_eval
-import event_model
-
 from ophyd.sim import NumpySeqHandler
 
+from .recommendations import NoRecommendation
+
 
 def stream_documents_into_runs(add_run):
     """
     Convert a flat stream of documents to "live" BlueskyRuns.
 
     Parameters
     ----------
@@ -159,40 +158,30 @@
     if queue is None:
         queue = Queue()
 
     if target_transforms is None:
         target_transforms = {}
 
     def tell_recommender(event):
-
         run = event.run
 
-        independent_map = call_or_eval(
-            {j: val for j, val in enumerate(independent_keys)}, run, stream_names
-        )
-        dependent_map = call_or_eval(
-            {j: val for j, val in enumerate(dependent_keys)}, run, stream_names
-        )
+        independent_map = call_or_eval({j: val for j, val in enumerate(independent_keys)}, run, stream_names)
+        dependent_map = call_or_eval({j: val for j, val in enumerate(dependent_keys)}, run, stream_names)
 
         independent = tuple(independent_map[j] for j in range(len(independent_keys)))
         measurement = tuple(dependent_map[j] for j in range(len(dependent_keys)))
         adaptive_obj.tell_many(independent, measurement)
         # pull the next point out of the adaptive API
         try:
             next_point = adaptive_obj.ask(1)
         except NoRecommendation:
             queue.put(None)
         else:
             if run.metadata["start"].get("batch_count") >= max_count:
                 queue.put(None)
             else:
-                queue.put(
-                    {
-                        k: target_transforms.get(k, lambda x: x)(v)
-                        for k, v in zip(target_keys, next_point)
-                    }
-                )
+                queue.put({k: target_transforms.get(k, lambda x: x)(v) for k, v in zip(target_keys, next_point)})
 
     def tell_recommender_on_completion(run):
         run.events.completed.connect(tell_recommender)
 
     return stream_documents_into_runs(tell_recommender_on_completion), queue
```

### Comparing `bluesky-adaptive-0.2.1/bluesky_adaptive/per_event.py` & `bluesky-adaptive-0.3.0/bluesky_adaptive/per_event.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,29 +7,26 @@
 time to make the decision is short compared to acquisition / movement time
 and the computation is amenable to streaming analysis.
 
 This is a "fine" grained integration of the adaptive logic into data acquisition.
 
 """
 
-from queue import Queue
 import itertools
+from queue import Queue
 
-import bluesky.preprocessors as bpp
 import bluesky.plan_stubs as bps
-
+import bluesky.preprocessors as bpp
 from event_model import RunRouter
 
 from .recommendations import NoRecommendation
 from .utils import extract_event_page
 
 
-def recommender_factory(
-    recommender, independent_keys, dependent_keys, *, max_count=10, queue=None
-):
+def recommender_factory(recommender, independent_keys, dependent_keys, *, max_count=10, queue=None):
     """
     Generate the callback and queue for gpCAM integration.
 
     For each Event that the callback sees it will place either a
     recommendation or `None` into the queue.  Recommendations will be
     of a dict mapping the independent_keys to the recommended values and
     should be interpreted by the plan as a request for more data.  A `None`
@@ -73,38 +70,30 @@
     def callback(name, doc):
         if name == "event_page":
             if doc["seq_num"][-1] > max_count:
                 # if at max number of points poison the queue and return early
                 queue.put(None)
                 return
 
-            independent, measurement = extract_event_page(
-                independent_keys, dependent_keys, payload=doc["data"]
-            )
+            independent, measurement = extract_event_page(independent_keys, dependent_keys, payload=doc["data"])
             recommender.tell_many(independent, measurement)
             try:
                 next_point = recommender.ask(1)
             except NoRecommendation:
                 # no recommendation
                 queue.put(None)
             else:
                 queue.put({k: v for k, v in zip(independent_keys, next_point)})
 
     rr = RunRouter([lambda name, doc: ([callback], [])])
     return rr, queue
 
 
 def adaptive_plan(
-    dets,
-    first_point,
-    *,
-    to_recommender,
-    from_recommender,
-    md=None,
-    take_reading=bps.trigger_and_read
+    dets, first_point, *, to_recommender, from_recommender, md=None, take_reading=bps.trigger_and_read
 ):
     """
     Execute an adaptive scan using an per event-run recommendation engine.
 
     The communication pattern here is that there is 1 recommendation for
     each Event that is generate
 
@@ -147,17 +136,15 @@
 
         Defaults to `bluesky.plan_stubs.trigger_and_read`
     """
     # TODO inject args / kwargs here.
     _md = {"hints": {}}
     _md.update(md or {})
     try:
-        _md["hints"].setdefault(
-            "dimensions", [(m.hints["fields"], "primary") for m in first_point.keys()]
-        )
+        _md["hints"].setdefault("dimensions", [(m.hints["fields"], "primary") for m in first_point.keys()])
     except (AttributeError, KeyError):
         ...
 
     # extract the motors
     motors = list(first_point.keys())
     # convert the first_point variable to from we will be getting
     # from queue
```

### Comparing `bluesky-adaptive-0.2.1/bluesky_adaptive/per_start.py` & `bluesky-adaptive-0.3.0/bluesky_adaptive/per_start.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,31 +8,28 @@
 computation and the experiment, of the data collection is not amenable
 to streaming analysis, or the natural structure of the experiment
 dictates.
 
 This corresponds to a "middle" scale of adaptive integration into
 data collection.
 """
-import uuid
 import itertools
-from queue import Queue, Empty
+import uuid
+from queue import Empty, Queue
 
-import bluesky.preprocessors as bpp
 import bluesky.plan_stubs as bps
 import bluesky.plans as bp
-
+import bluesky.preprocessors as bpp
 from event_model import RunRouter
 
 from .recommendations import NoRecommendation
 from .utils import extract_event_page
 
 
-def recommender_factory(
-    adaptive_obj, independent_keys, dependent_keys, *, max_count=10, queue=None
-):
+def recommender_factory(adaptive_obj, independent_keys, dependent_keys, *, max_count=10, queue=None):
     """
     Generate the callback and queue for an Adaptive API backed reccomender.
 
     This recommends a fixed step size independent of the measurement.
 
     For each Run (aka Start) that the callback sees it will place
     either a recommendation or `None` into the queue.  Recommendations
@@ -90,33 +87,29 @@
                 return
             else:
                 poisoned = False
 
         if name == "event_page":
             if poisoned:
                 return
-            independent, measurement = extract_event_page(
-                independent_keys, dependent_keys, payload=doc["data"]
-            )
+            independent, measurement = extract_event_page(independent_keys, dependent_keys, payload=doc["data"])
             adaptive_obj.tell_many(independent, measurement)
             # pull the next point out of the adaptive API
             try:
                 next_point = adaptive_obj.ask(1)
             except NoRecommendation:
                 queue.put(None)
             else:
                 queue.put({k: v for k, v in zip(independent_keys, next_point)})
 
     rr = RunRouter([lambda name, doc: ([callback], [])])
     return rr, queue
 
 
-def adaptive_plan(
-    dets, first_point, *, to_recommender, from_recommender, md=None, take_reading=bp.count
-):
+def adaptive_plan(dets, first_point, *, to_recommender, from_recommender, md=None, take_reading=bp.count):
     """
     Execute an adaptive scan using an inter-run recommendation engine.
 
     Parameters
     ----------
     dets : List[OphydObj]
        The detector to read at each point.  The dependent keys that the
```

### Comparing `bluesky-adaptive-0.2.1/bluesky_adaptive/recommendations.py` & `bluesky-adaptive-0.3.0/bluesky_adaptive/recommendations.py`

 * *Files identical despite different names*

### Comparing `bluesky-adaptive-0.2.1/bluesky_adaptive/scipy_reccomendations.py` & `bluesky-adaptive-0.3.0/bluesky_adaptive/scipy_reccomendations.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from scipy.optimize import minimize
-from threading import Thread, Event
 from queue import Empty, Queue
+from threading import Event, Thread
+
+from scipy.optimize import minimize
 
 from bluesky_adaptive.recommendations import NoRecommendation
 
 
 class MinimizerReccomender:
     """A very naive recommendation engine that uses scipy.optomize.minimize"""
```

### Comparing `bluesky-adaptive-0.2.1/bluesky_adaptive/tests/test_per_event.py` & `bluesky-adaptive-0.3.0/bluesky_adaptive/tests/test_per_start.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,44 @@
+from queue import Empty
+
+import pytest
 from bluesky.tests.utils import DocCollector
 
-from bluesky_adaptive.per_event import (
-    recommender_factory,
-    adaptive_plan,
-)
+from bluesky_adaptive.per_start import adaptive_plan, recommender_factory
 from bluesky_adaptive.recommendations import SequenceRecommender
 
 
 def test_seq_recommender(RE, hw):
-
-    recommender = SequenceRecommender([[1,], [2,], [3,]])  # noqa
+    recommender = SequenceRecommender(
+        [
+            [
+                1,
+            ],
+            [
+                2,
+            ],
+            [
+                3,
+            ],
+        ]
+    )  # noqa
 
     cb, queue = recommender_factory(recommender, ["motor"], ["det"])
     dc = DocCollector()
 
+    # pre-poison the queue to simulate a messy reccomender
+    queue.put(None)
+    queue.put({})
+
     RE(
         adaptive_plan([hw.det], {hw.motor: 0}, to_recommender=cb, from_recommender=queue),
         dc.insert,
     )
 
-    assert len(dc.start) == 1
-    assert len(dc.event) == 1
-    (events,) = dc.event.values()
-    assert len(events) == 4
+    assert len(dc.start) == 4
+    assert len(dc.event) == 4
+    for ev in dc.event.values():
+        assert len(ev) == 1
+
+    # check that our reccomender does not leave anything behind
+    with pytest.raises(Empty):
+        queue.get(block=False)
```

### Comparing `bluesky-adaptive-0.2.1/bluesky_adaptive/tests/test_scipy_rec.py` & `bluesky-adaptive-0.3.0/bluesky_adaptive/tests/test_scipy_rec.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-import pytest
 import bluesky.plan_stubs as bps
+import pytest
 
-from bluesky_adaptive.per_start import adaptive_plan
 from bluesky_adaptive.on_stop import recommender_factory
+from bluesky_adaptive.per_start import adaptive_plan
 
 
 def test_scipy_minimize_recommender(RE, hw):
     pytest.importorskip("scipy")
     from bluesky_adaptive.scipy_reccomendations import MinimizerReccomender
 
     results_list = []
@@ -16,17 +16,15 @@
         cb, queue = recommender_factory(
             adaptive_obj=recommender,
             independent_keys=["np.mean(motor)"],
             dependent_keys=[det_key],
             target_keys=["motor"],
             max_count=100,
         )
-        yield from adaptive_plan(
-            [det], {hw.motor: 1}, to_recommender=cb, from_recommender=queue
-        )
+        yield from adaptive_plan([det], {hw.motor: 1}, to_recommender=cb, from_recommender=queue)
         yield from bps.mv(hw.motor, recommender.result.x)
         print(recommender.result)
         results_list.append(recommender.result)
 
     RE(do_the_thing(hw.det, "np.asarray(det)"))
     RE(do_the_thing(hw.img, "np.median(img)"))
     assert len(results_list) == 2
```

### Comparing `bluesky-adaptive-0.2.1/bluesky_adaptive/utils.py` & `bluesky-adaptive-0.3.0/bluesky_adaptive/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Helper functions an classes that will be shared across per-event and per-run."""
 
 import itertools
+
 import numpy as np
 
 
 def chain_zip(motors, next_point):
     """
     Interlace motors and next_point values.
 
@@ -88,11 +89,8 @@
 
     measurements : np.array
         A numpy array where the first axis maps to the dependent variables
 
     """
     # the data comes out of the EventPag "column major"
     # we transpose to get "row major"
-    return tuple(
-        np.atleast_2d(np.asarray([payload[k] for k in key_list])).T
-        for key_list in key_lists
-    )
+    return tuple(np.atleast_2d(np.asarray([payload[k] for k in key_list])).T for key_list in key_lists)
```

### Comparing `bluesky-adaptive-0.2.1/bluesky_adaptive.egg-info/PKG-INFO` & `bluesky-adaptive-0.3.0/bluesky_adaptive.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: bluesky-adaptive
-Version: 0.2.1
+Version: 0.3.0
 Summary: Tools for writing adaptive plans
 Home-page: https://github.com/bluesky/bluesky-adaptive
 Author: NSLS-II
 Author-email: dama@bnl.gov
 License: BSD (3-clause)
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
+Provides-Extra: agents
+Provides-Extra: all
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 ================
 bluesky-adaptive
 ================
 
@@ -30,9 +31,7 @@
 * Free software: 3-clause BSD license
 * Documentation: (COMING SOON!) https://bluesky.github.io/bluesky-adaptive.
 
 Features
 --------
 
 * TODO
-
-
```

### Comparing `bluesky-adaptive-0.2.1/docs/Makefile` & `bluesky-adaptive-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bluesky-adaptive-0.2.1/docs/make.bat` & `bluesky-adaptive-0.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `bluesky-adaptive-0.2.1/docs/source/conf.py` & `bluesky-adaptive-0.3.0/docs/source/conf.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,188 +20,189 @@
 # import os
 # import sys
 # sys.path.insert(0, os.path.abspath('.'))
 
 
 # -- General configuration ------------------------------------------------
 import sphinx
+
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
-    'sphinx.ext.autodoc',
-    'sphinx.ext.autosummary',
-    'sphinx.ext.githubpages',
-    'sphinx.ext.intersphinx',
-    'sphinx.ext.mathjax',
-    'sphinx.ext.viewcode',
-    'IPython.sphinxext.ipython_directive',
-    'IPython.sphinxext.ipython_console_highlighting',
-    'matplotlib.sphinxext.plot_directive',
-    'numpydoc',
-    'sphinx_copybutton',
+    "sphinx.ext.autodoc",
+    "sphinx.ext.autosummary",
+    "sphinx.ext.githubpages",
+    "sphinx.ext.mathjax",
+    "sphinx.ext.viewcode",
+    "IPython.sphinxext.ipython_directive",
+    "IPython.sphinxext.ipython_console_highlighting",
+    "matplotlib.sphinxext.plot_directive",
+    "numpydoc",
+    "sphinx_copybutton",
 ]
 
 # Configuration options for plot_directive. See:
 # https://github.com/matplotlib/matplotlib/blob/f3ed922d935751e08494e5fb5311d3050a3b637b/lib/matplotlib/sphinxext/plot_directive.py#L81
 plot_html_show_source_link = False
 plot_html_show_formats = False
 
 # Generate the API documentation when building
 autosummary_generate = True
 numpydoc_show_class_members = False
 
 # Add any paths that contain templates here, relative to this directory.
-templates_path = ['_templates']
+templates_path = ["_templates"]
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
 #
 # source_suffix = ['.rst', '.md']
-source_suffix = '.rst'
+source_suffix = ".rst"
 
 # The master toctree document.
-master_doc = 'index'
+master_doc = "index"
 
 # General information about the project.
-project = 'bluesky-adaptive'
-copyright = '2020, NSLS-II'
-author = 'NSLS-II'
+project = "bluesky-adaptive"
+copyright = "2020, NSLS-II"
+author = "NSLS-II"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 import bluesky_adaptive
+
 # The short X.Y version.
 version = bluesky_adaptive.__version__
 # The full version, including alpha/beta/rc tags.
 release = bluesky_adaptive.__version__
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = "en"
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This patterns also effect to html_static_path and html_extra_path
 exclude_patterns = []
 
 # The name of the Pygments (syntax highlighting) style to use.
-pygments_style = 'sphinx'
+pygments_style = "sphinx"
 
 # If true, `todo` and `todoList` produce output, else they produce nothing.
 todo_include_todos = False
 
 
 # -- Options for HTML output ----------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
-html_theme = 'sphinx_rtd_theme'
+html_theme = "sphinx_rtd_theme"
 import sphinx_rtd_theme
+
 html_theme_path = [sphinx_rtd_theme.get_html_theme_path()]
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
 #
 # html_theme_options = {}
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
-html_static_path = ['_static']
+html_static_path = ["_static"]
 
 # Custom sidebar templates, must be a dictionary that maps document names
 # to template names.
 #
 # This is required for the alabaster theme
 # refs: http://alabaster.readthedocs.io/en/latest/installation.html#sidebars
 html_sidebars = {
-    '**': [
-        'relations.html',  # needs 'show_related': True theme option to display
-        'searchbox.html',
+    "**": [
+        "relations.html",  # needs 'show_related': True theme option to display
+        "searchbox.html",
     ]
 }
 
 
 # -- Options for HTMLHelp output ------------------------------------------
 
 # Output file base name for HTML help builder.
-htmlhelp_basename = 'bluesky-adaptive'
+htmlhelp_basename = "bluesky-adaptive"
 
 
 # -- Options for LaTeX output ---------------------------------------------
 
 latex_elements = {
     # The paper size ('letterpaper' or 'a4paper').
     #
     # 'papersize': 'letterpaper',
-
     # The font size ('10pt', '11pt' or '12pt').
     #
     # 'pointsize': '10pt',
-
     # Additional stuff for the LaTeX preamble.
     #
     # 'preamble': '',
-
     # Latex figure (float) alignment
     #
     # 'figure_align': 'htbp',
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title,
 #  author, documentclass [howto, manual, or own class]).
 latex_documents = [
-    (master_doc, 'bluesky-adaptive.tex', 'bluesky-adaptive Documentation',
-     'Contributors', 'manual'),
+    (master_doc, "bluesky-adaptive.tex", "bluesky-adaptive Documentation", "Contributors", "manual"),
 ]
 
 
 # -- Options for manual page output ---------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
-man_pages = [
-    (master_doc, 'bluesky-adaptive', 'bluesky-adaptive Documentation',
-     [author], 1)
-]
+man_pages = [(master_doc, "bluesky-adaptive", "bluesky-adaptive Documentation", [author], 1)]
 
 
 # -- Options for Texinfo output -------------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
-    (master_doc, 'bluesky-adaptive', 'bluesky-adaptive Documentation',
-     author, 'bluesky-adaptive', 'Tools for writing adaptive plans',
-     'Miscellaneous'),
+    (
+        master_doc,
+        "bluesky-adaptive",
+        "bluesky-adaptive Documentation",
+        author,
+        "bluesky-adaptive",
+        "Tools for writing adaptive plans",
+        "Miscellaneous",
+    ),
 ]
 
-default_role = 'obj'
+default_role = "obj"
 
 
 # Example configuration for intersphinx: refer to the Python standard library.
 intersphinx_mapping = {
-    'python': ('https://docs.python.org/3/', None),
-    'numpy': ('https://numpy.org/doc/stable/', None),
-    'scipy': ('https://docs.scipy.org/doc/scipy/reference/', None),
-    'pandas': ('https://pandas.pydata.org/pandas-docs/stable', None),
-    'matplotlib': ('https://matplotlib.org', None),
-    'bluesky': ('https://blueskyproject.io/bluesky/', None),
-    'ophyd': ('https://blueskyproject.io/ophyd/', None),
-    'event-model': ('https://blueskyproject.io/event-model/', None),
+    "python": ("https://docs.python.org/3/", None),
+    "numpy": ("https://numpy.org/doc/stable/", None),
+    "scipy": ("https://docs.scipy.org/doc/scipy/reference/", None),
+    "pandas": ("https://pandas.pydata.org/pandas-docs/stable", None),
+    "matplotlib": ("https://matplotlib.org", None),
+    "bluesky": ("https://blueskyproject.io/bluesky/", None),
+    "ophyd": ("https://blueskyproject.io/ophyd/", None),
+    "event-model": ("https://blueskyproject.io/event-model/", None),
 }
 
 # nitpicky = sphinx.version_info >= (3,)
```

### Comparing `bluesky-adaptive-0.2.1/docs/source/examples.rst` & `bluesky-adaptive-0.3.0/docs/source/examples.rst`

 * *Files identical despite different names*

### Comparing `bluesky-adaptive-0.2.1/docs/source/index.rst` & `bluesky-adaptive-0.3.0/docs/source/index.rst`

 * *Files 10% similar despite different names*

```diff
@@ -11,14 +11,15 @@
    :titlesonly:
 
    installation
    usage
    release-history
    min_versions
    examples
+   distributed
 
 .. warning::
 
    This is currently under rapid development, the API may change at
    any time.
 
 
@@ -248,9 +249,30 @@
 (or a human!) watching the data and adjusting the step size based on the how
 "interesting" the data currently looks.  By this mechanism we would spend more
 time collecting data in "interesting" parts of phase space and extract more
 science for a given amount of beamtime.
 
 In both of these cases the feedback is adding value without imposing a cost to
 the plans and the failure mode of the computation failing is the current status
-quo.  There are many ways that asynchronous feedback can be
-implemented and is out of scope for this package.
+quo.
+
+An increasingly desirable operating paradigm for autonomous experiments considers
+the directives of many agents, or even networks of agents,
+including multiple human agents. The previously described lock-step approaches to
+experiment and analysis, leave no room for human experts to engage in the loop,
+incorporation of information from complementary techniques, or the integration of
+multiple computational agents. In this more complex paradigm, various agents must be
+able to process the captured data stream, suggest plans to be executed,
+and create reports for human consumption. This is exemplified in the case where
+multiple passive agents are performing dataset factorization or AI-based compression
+algorithms that provide visualization tools for users,  multiple active learning
+agents are providing suggestions for next experiments as they complete their
+computation, and human agents are also guiding the experiment
+(see this `NeurIPS Workshop Paper <https://arxiv.org/abs/2301.09177>`_).
+
+Here, the same :code:`tell`, :code:`report`, :code:`ask` grammar can be used in conjunction with
+Kafka, Tiled, and the RunManager. This adds some additional dependencies including
+``bluesky-queueserver``, ``tiled``, and ``bluesky-kafka``.
+Examples of these agents are provided in :ref:`distributed`.
+Furthermore, using Kafka for distributed communication, one can construct meta-agents,
+or *adjudicators*, which coordinate between a collection of agents in more sophisticated ways
+than the RunManager priority queue and provide an additional avenue for human intervention.
```

### Comparing `bluesky-adaptive-0.2.1/docs/source/min_versions.rst` & `bluesky-adaptive-0.3.0/docs/source/min_versions.rst`

 * *Files identical despite different names*

### Comparing `bluesky-adaptive-0.2.1/setup.py` & `bluesky-adaptive-0.3.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-from os import path
-from setuptools import setup, find_packages
 import sys
-import versioneer
+from os import path
 
+from setuptools import find_packages, setup
+
+import versioneer
 
 # NOTE: This file must remain Python 2 compatible for the foreseeable future,
 # to ensure that we error out properly for people with outdated setuptools
 # and/or pip.
 min_version = (3, 7)
 if sys.version_info < min_version:
     error = """
@@ -25,22 +26,28 @@
     sys.exit(error)
 
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, "README.rst"), encoding="utf-8") as readme_file:
     readme = readme_file.read()
 
-with open(path.join(here, "requirements.txt")) as requirements_file:
-    # Parse requirements.txt, ignoring any commented-out lines.
-    requirements = [
-        line
-        for line in requirements_file.read().splitlines()
-        if not line.startswith("#")
-    ]
 
+def read_requirements(filename):
+    with open(path.join(here, filename)) as requirements_file:
+        # Parse requirements.txt, ignoring any commented-out lines.
+        requirements = [line for line in requirements_file.read().splitlines() if not line.startswith("#")]
+    return requirements
+
+
+requirements = read_requirements("requirements.txt")
+categorized_requirements = {key: read_requirements(f"requirements-{key}.txt") for key in ["agents"]}
+
+extras_require = {}
+extras_require["agents"] = categorized_requirements["agents"]
+extras_require["all"] = categorized_requirements["agents"]
 
 setup(
     name="bluesky-adaptive",
     version=versioneer.get_version(),
     cmdclass=versioneer.get_cmdclass(),
     description="Tools for writing adaptive plans",
     long_description=readme,
@@ -59,14 +66,15 @@
         "bluesky_adaptive": [
             # When adding files here, remember to update MANIFEST.in as well,
             # or else they will not be included in the distribution on PyPI!
             # 'path/to/data_file',
         ]
     },
     install_requires=requirements,
+    extras_require=extras_require,
     license="BSD (3-clause)",
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
     ],
 )
```

### Comparing `bluesky-adaptive-0.2.1/versioneer.py` & `bluesky-adaptive-0.3.0/versioneer.py`

 * *Files 1% similar despite different names*

```diff
@@ -273,18 +273,20 @@
 Specifically, both are released under the Creative Commons "Public Domain
 Dedication" license (CC0-1.0), as described in
 https://creativecommons.org/publicdomain/zero/1.0/ .
 
 """
 
 from __future__ import print_function
+
 try:
     import configparser
 except ImportError:
     import ConfigParser as configparser
+
 import errno
 import json
 import os
 import re
 import subprocess
 import sys
 
@@ -335,17 +337,16 @@
 def get_config_from_root(root):
     """Read the project setup.cfg file to determine Versioneer config."""
     # This might raise EnvironmentError (if setup.cfg is missing), or
     # configparser.NoSectionError (if it lacks a [versioneer] section), or
     # configparser.NoOptionError (if it lacks "VCS="). See the docstring at
     # the top of versioneer.py for instructions on writing your setup.cfg .
     setup_cfg = os.path.join(root, "setup.cfg")
-    parser = configparser.SafeConfigParser()
-    with open(setup_cfg, "r") as f:
-        parser.readfp(f)
+    parser = configparser.ConfigParser()
+    parser.read(setup_cfg)
     VCS = parser.get("versioneer", "VCS")  # mandatory
 
     def get(parser, name):
         if parser.has_option("versioneer", name):
             return parser.get("versioneer", name)
         return None
     cfg = VersioneerConfig()
@@ -1557,14 +1558,15 @@
                                                   cfg.versionfile_build)
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
     cmds["build_py"] = cmd_build_py
 
     if "cx_Freeze" in sys.modules:  # cx_freeze enabled?
         from cx_Freeze.dist import build_exe as _build_exe
+
         # nczeczulin reports that py2exe won't like the pep440-style string
         # as FILEVERSION, but it can be used for PRODUCTVERSION, e.g.
         # setup(console=[{
         #   "version": versioneer.get_version().split("+", 1)[0], # FILEVERSION
         #   "product_version": versioneer.get_version(),
         #   ...
```

