# Comparing `tmp/async-graph-data-flow-1.1.0.tar.gz` & `tmp/async-graph-data-flow-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async-graph-data-flow-1.1.0.tar", last modified: Thu Mar  2 21:56:30 2023, max compression
+gzip compressed data, was "async-graph-data-flow-1.2.0.tar", last modified: Wed Apr 26 14:57:04 2023, max compression
```

## Comparing `async-graph-data-flow-1.1.0.tar` & `async-graph-data-flow-1.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 jacksonlee   (503) staff       (20)        0 2023-03-02 21:56:30.948674 async-graph-data-flow-1.1.0/
--rw-r--r--   0 jacksonlee   (503) staff       (20)     1501 2023-01-03 15:46:58.000000 async-graph-data-flow-1.1.0/LICENSE.txt
--rw-r--r--   0 jacksonlee   (503) staff       (20)     2594 2023-03-02 21:56:30.948079 async-graph-data-flow-1.1.0/PKG-INFO
--rw-r--r--   0 jacksonlee   (503) staff       (20)     1583 2023-01-06 04:22:09.000000 async-graph-data-flow-1.1.0/README.md
--rw-r--r--   0 jacksonlee   (503) staff       (20)     1681 2023-03-02 21:54:29.000000 async-graph-data-flow-1.1.0/pyproject.toml
--rw-r--r--   0 jacksonlee   (503) staff       (20)       38 2023-03-02 21:56:30.948827 async-graph-data-flow-1.1.0/setup.cfg
-drwxr-xr-x   0 jacksonlee   (503) staff       (20)        0 2023-03-02 21:56:30.926668 async-graph-data-flow-1.1.0/src/
-drwxr-xr-x   0 jacksonlee   (503) staff       (20)        0 2023-03-02 21:56:30.937707 async-graph-data-flow-1.1.0/src/async_graph_data_flow/
--rw-r--r--   0 jacksonlee   (503) staff       (20)      197 2023-01-03 15:46:58.000000 async-graph-data-flow-1.1.0/src/async_graph_data_flow/__init__.py
--rw-r--r--   0 jacksonlee   (503) staff       (20)    13187 2023-03-02 21:54:29.000000 async-graph-data-flow-1.1.0/src/async_graph_data_flow/executor.py
--rw-r--r--   0 jacksonlee   (503) staff       (20)     9212 2023-03-02 21:54:29.000000 async-graph-data-flow-1.1.0/src/async_graph_data_flow/graph.py
-drwxr-xr-x   0 jacksonlee   (503) staff       (20)        0 2023-03-02 21:56:30.945271 async-graph-data-flow-1.1.0/src/async_graph_data_flow.egg-info/
--rw-r--r--   0 jacksonlee   (503) staff       (20)     2594 2023-03-02 21:56:30.000000 async-graph-data-flow-1.1.0/src/async_graph_data_flow.egg-info/PKG-INFO
--rw-r--r--   0 jacksonlee   (503) staff       (20)      511 2023-03-02 21:56:30.000000 async-graph-data-flow-1.1.0/src/async_graph_data_flow.egg-info/SOURCES.txt
--rw-r--r--   0 jacksonlee   (503) staff       (20)        1 2023-03-02 21:56:30.000000 async-graph-data-flow-1.1.0/src/async_graph_data_flow.egg-info/dependency_links.txt
--rw-r--r--   0 jacksonlee   (503) staff       (20)        1 2023-01-03 17:19:01.000000 async-graph-data-flow-1.1.0/src/async_graph_data_flow.egg-info/not-zip-safe
--rw-r--r--   0 jacksonlee   (503) staff       (20)      174 2023-03-02 21:56:30.000000 async-graph-data-flow-1.1.0/src/async_graph_data_flow.egg-info/requires.txt
--rw-r--r--   0 jacksonlee   (503) staff       (20)       22 2023-03-02 21:56:30.000000 async-graph-data-flow-1.1.0/src/async_graph_data_flow.egg-info/top_level.txt
-drwxr-xr-x   0 jacksonlee   (503) staff       (20)        0 2023-03-02 21:56:30.947347 async-graph-data-flow-1.1.0/tests/
--rw-r--r--   0 jacksonlee   (503) staff       (20)    14019 2023-03-02 21:54:29.000000 async-graph-data-flow-1.1.0/tests/test_executor.py
--rw-r--r--   0 jacksonlee   (503) staff       (20)     3987 2023-01-03 15:46:58.000000 async-graph-data-flow-1.1.0/tests/test_graph.py
--rw-r--r--   0 jacksonlee   (503) staff       (20)      686 2023-01-03 15:46:58.000000 async-graph-data-flow-1.1.0/tests/test_version_number.py
+drwxr-xr-x   0 jlee       (503) staff       (20)        0 2023-04-26 14:57:04.597411 async-graph-data-flow-1.2.0/
+-rw-r--r--   0 jlee       (503) staff       (20)     1506 2023-04-26 13:45:53.000000 async-graph-data-flow-1.2.0/LICENSE.txt
+-rw-r--r--   0 jlee       (503) staff       (20)     2807 2023-04-26 14:57:04.596765 async-graph-data-flow-1.2.0/PKG-INFO
+-rw-r--r--   0 jlee       (503) staff       (20)     1796 2023-04-26 13:45:53.000000 async-graph-data-flow-1.2.0/README.md
+-rw-r--r--   0 jlee       (503) staff       (20)     1681 2023-04-26 13:45:53.000000 async-graph-data-flow-1.2.0/pyproject.toml
+-rw-r--r--   0 jlee       (503) staff       (20)       38 2023-04-26 14:57:04.597858 async-graph-data-flow-1.2.0/setup.cfg
+drwxr-xr-x   0 jlee       (503) staff       (20)        0 2023-04-26 14:57:04.563883 async-graph-data-flow-1.2.0/src/
+drwxr-xr-x   0 jlee       (503) staff       (20)        0 2023-04-26 14:57:04.576006 async-graph-data-flow-1.2.0/src/async_graph_data_flow/
+-rw-r--r--   0 jlee       (503) staff       (20)      197 2023-03-29 21:45:25.000000 async-graph-data-flow-1.2.0/src/async_graph_data_flow/__init__.py
+-rw-r--r--   0 jlee       (503) staff       (20)    13649 2023-04-26 13:45:53.000000 async-graph-data-flow-1.2.0/src/async_graph_data_flow/executor.py
+-rw-r--r--   0 jlee       (503) staff       (20)     9212 2023-03-29 21:45:25.000000 async-graph-data-flow-1.2.0/src/async_graph_data_flow/graph.py
+drwxr-xr-x   0 jlee       (503) staff       (20)        0 2023-04-26 14:57:04.588256 async-graph-data-flow-1.2.0/src/async_graph_data_flow.egg-info/
+-rw-r--r--   0 jlee       (503) staff       (20)     2807 2023-04-26 14:57:04.000000 async-graph-data-flow-1.2.0/src/async_graph_data_flow.egg-info/PKG-INFO
+-rw-r--r--   0 jlee       (503) staff       (20)      511 2023-04-26 14:57:04.000000 async-graph-data-flow-1.2.0/src/async_graph_data_flow.egg-info/SOURCES.txt
+-rw-r--r--   0 jlee       (503) staff       (20)        1 2023-04-26 14:57:04.000000 async-graph-data-flow-1.2.0/src/async_graph_data_flow.egg-info/dependency_links.txt
+-rw-r--r--   0 jlee       (503) staff       (20)        1 2023-03-29 21:46:52.000000 async-graph-data-flow-1.2.0/src/async_graph_data_flow.egg-info/not-zip-safe
+-rw-r--r--   0 jlee       (503) staff       (20)      174 2023-04-26 14:57:04.000000 async-graph-data-flow-1.2.0/src/async_graph_data_flow.egg-info/requires.txt
+-rw-r--r--   0 jlee       (503) staff       (20)       22 2023-04-26 14:57:04.000000 async-graph-data-flow-1.2.0/src/async_graph_data_flow.egg-info/top_level.txt
+drwxr-xr-x   0 jlee       (503) staff       (20)        0 2023-04-26 14:57:04.594281 async-graph-data-flow-1.2.0/tests/
+-rw-r--r--   0 jlee       (503) staff       (20)    14473 2023-04-26 13:45:53.000000 async-graph-data-flow-1.2.0/tests/test_executor.py
+-rw-r--r--   0 jlee       (503) staff       (20)     3987 2023-03-29 21:45:25.000000 async-graph-data-flow-1.2.0/tests/test_graph.py
+-rw-r--r--   0 jlee       (503) staff       (20)      686 2023-03-29 21:45:25.000000 async-graph-data-flow-1.2.0/tests/test_version_number.py
```

### Comparing `async-graph-data-flow-1.1.0/LICENSE.txt` & `async-graph-data-flow-1.2.0/LICENSE.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2022, Civis Analytics
+Copyright (c) 2022-2023, Civis Analytics
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `async-graph-data-flow-1.1.0/PKG-INFO` & `async-graph-data-flow-1.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-graph-data-flow
-Version: 1.1.0
+Version: 1.2.0
 Summary: Asynchronous functions that pass data along a directed acyclic graph
 Author-email: Civis Analytics <opensource@civisanalytics.com>
 License: BSD 3-Clause
 Project-URL: Source, https://github.com/civisanalytics/async-graph-data-flow
 Keywords: async,asynchronous,asyncio,data flow,graph
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -28,14 +28,18 @@
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/async-graph-data-flow.svg)](https://pypi.org/project/async-graph-data-flow/)
 [![CircleCI Builds](https://circleci.com/gh/civisanalytics/async-graph-data-flow.svg?style=shield)](https://circleci.com/gh/civisanalytics/async-graph-data-flow)
 
 ## Full Documentation
 
 Please visit https://civisanalytics.github.io/async-graph-data-flow
 
+Please also check out this
+[blog post](https://www.civisanalytics.com/blog/open-source-software-release-introducing-async-graph-data-flow-a-python-library-for-efficient-data-pipelines/)
+introducing this package.
+
 ## License
 
 BSD 3-Clause License. Please see `LICENSE.txt` in the GitHub source code for details.
 
 ## Setting up a Development Environment
 
 The latest code under development is available on GitHub at
```

### Comparing `async-graph-data-flow-1.1.0/README.md` & `async-graph-data-flow-1.2.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/async-graph-data-flow.svg)](https://pypi.org/project/async-graph-data-flow/)
 [![CircleCI Builds](https://circleci.com/gh/civisanalytics/async-graph-data-flow.svg?style=shield)](https://circleci.com/gh/civisanalytics/async-graph-data-flow)
 
 ## Full Documentation
 
 Please visit https://civisanalytics.github.io/async-graph-data-flow
 
+Please also check out this
+[blog post](https://www.civisanalytics.com/blog/open-source-software-release-introducing-async-graph-data-flow-a-python-library-for-efficient-data-pipelines/)
+introducing this package.
+
 ## License
 
 BSD 3-Clause License. Please see `LICENSE.txt` in the GitHub source code for details.
 
 ## Setting up a Development Environment
 
 The latest code under development is available on GitHub at
```

### Comparing `async-graph-data-flow-1.1.0/pyproject.toml` & `async-graph-data-flow-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 65.3.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "async-graph-data-flow"
-version = "1.1.0"
+version = "1.2.0"
 description = "Asynchronous functions that pass data along a directed acyclic graph"
 readme = "README.md"
 requires-python = ">= 3.10"
 license = { text = "BSD 3-Clause" }
 authors = [ { name = "Civis Analytics", email = "opensource@civisanalytics.com" } ]
 keywords = [
     "async",
```

### Comparing `async-graph-data-flow-1.1.0/src/async_graph_data_flow/executor.py` & `async-graph-data-flow-1.2.0/src/async_graph_data_flow/executor.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,37 +61,49 @@
 
     @property
     def graph(self) -> AsyncGraph:
         """The graph to execute."""
         return self._graph
 
     @property
-    def exceptions(self) -> dict[str, list[Exception]]:
+    def exceptions(self) -> dict[str, list[Exception]] | None:
         """Exceptions from the graph execution.
 
         The key is a node by name (str), and the value is the list of exceptions
         raised from the node.
         """
+        if self._exceptions is None:
+            return
         from_deque_to_list = {}
         for node_name, excs in self._exceptions.items():
             # `excs` is a deque. Turning it into a list for user-friendliness.
             from_deque_to_list[node_name] = list(excs)
         return from_deque_to_list
 
     @property
-    def data_flow_stats(self) -> dict[str, dict[str, int]]:
+    def data_flow_stats(self) -> dict[str, dict[str, int]] | None:
         """Data flow statistics.
 
         These statistics keep track of (i) the number of times data has passed
         into each node, (ii) the number of times data has come out of each node, and
         (iii) the number of errors each node has had.
         The key is a node by name (str), and the value is a dict with three keys (str)
         of ``"in"``, ``"out"``, and ``"err"``, each corresponding to its count (int)."""
         return self._data_flow_stats
 
+    @property
+    def start_nodes(self) -> dict[str, tuple]:
+        """Start nodes and their arguments.
+
+        This is a dictionary that maps each start node (str) to its arguments
+        to be passed in when the graph execution begins."""
+        if self._start_node_args is None:
+            self._start_node_args = self._get_start_node_args(None)
+        return self._start_node_args
+
     def turn_on_data_flow_logging(
         self,
         node_format: Optional[str] = None,
         node_filter: Iterable[str] = None,
         time_interval: Optional[int] = None,
         logger: logging.Logger = None,
     ):
```

### Comparing `async-graph-data-flow-1.1.0/src/async_graph_data_flow/graph.py` & `async-graph-data-flow-1.2.0/src/async_graph_data_flow/graph.py`

 * *Files identical despite different names*

### Comparing `async-graph-data-flow-1.1.0/src/async_graph_data_flow.egg-info/PKG-INFO` & `async-graph-data-flow-1.2.0/src/async_graph_data_flow.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-graph-data-flow
-Version: 1.1.0
+Version: 1.2.0
 Summary: Asynchronous functions that pass data along a directed acyclic graph
 Author-email: Civis Analytics <opensource@civisanalytics.com>
 License: BSD 3-Clause
 Project-URL: Source, https://github.com/civisanalytics/async-graph-data-flow
 Keywords: async,asynchronous,asyncio,data flow,graph
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -28,14 +28,18 @@
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/async-graph-data-flow.svg)](https://pypi.org/project/async-graph-data-flow/)
 [![CircleCI Builds](https://circleci.com/gh/civisanalytics/async-graph-data-flow.svg?style=shield)](https://circleci.com/gh/civisanalytics/async-graph-data-flow)
 
 ## Full Documentation
 
 Please visit https://civisanalytics.github.io/async-graph-data-flow
 
+Please also check out this
+[blog post](https://www.civisanalytics.com/blog/open-source-software-release-introducing-async-graph-data-flow-a-python-library-for-efficient-data-pipelines/)
+introducing this package.
+
 ## License
 
 BSD 3-Clause License. Please see `LICENSE.txt` in the GitHub source code for details.
 
 ## Setting up a Development Environment
 
 The latest code under development is available on GitHub at
```

### Comparing `async-graph-data-flow-1.1.0/tests/test_executor.py` & `async-graph-data-flow-1.2.0/tests/test_executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -427,14 +427,16 @@
 
     graph = AsyncGraph()
     graph.add_node(node1)
     graph.add_node(node2)
     graph.add_edge("node1", "node2")
 
     executor = AsyncExecutor(graph)
+    assert executor.exceptions is None
+
     executor.execute()
     excs = executor.exceptions
 
     assert excs["node1"] == []
     assert len(excs["node2"]) == 2
 
     actual_exc_msgs = [e.args[0] for e in excs["node2"]]
@@ -445,7 +447,25 @@
     assert executor.data_flow_stats["node1"].get("in") == 0
     assert executor.data_flow_stats["node1"].get("out") == 2
     assert executor.data_flow_stats["node1"].get("err") == 0
 
     assert executor.data_flow_stats["node2"].get("in") == 2
     assert executor.data_flow_stats["node2"].get("out") == 0
     assert executor.data_flow_stats["node2"].get("err") == 2
+
+
+def test_graph_with_no_edges():
+    async def node1(data):
+        yield
+
+    async def node2(data):
+        yield
+
+    graph = AsyncGraph()
+    graph.add_node(node1)
+    graph.add_node(node2)
+
+    executor = AsyncExecutor(graph)
+    assert executor.start_nodes == {"node1": tuple(), "node2": tuple()}
+
+    executor.execute(start_nodes={"node1": ("foo",)})
+    assert executor.start_nodes == {"node1": ("foo",)}
```

### Comparing `async-graph-data-flow-1.1.0/tests/test_graph.py` & `async-graph-data-flow-1.2.0/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `async-graph-data-flow-1.1.0/tests/test_version_number.py` & `async-graph-data-flow-1.2.0/tests/test_version_number.py`

 * *Files identical despite different names*

