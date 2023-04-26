# Comparing `tmp/nnx-0.0.1.tar.gz` & `tmp/nnx-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nnx-0.0.1.tar", max compression
+gzip compressed data, was "nnx-0.0.2.tar", max compression
```

## Comparing `nnx-0.0.1.tar` & `nnx-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1072 2023-03-18 22:40:31.494888 nnx-0.0.1/LICENSE
--rw-r--r--   0        0        0     3952 2023-04-22 20:13:31.443728 nnx-0.0.1/README.md
--rw-r--r--   0        0        0      776 2023-04-22 15:20:28.647804 nnx-0.0.1/nnx/__init__.py
--rw-r--r--   0        0        0     2235 2023-04-08 23:38:12.700869 nnx-0.0.1/nnx/fields.py
--rw-r--r--   0        0        0     3789 2023-04-22 15:20:28.647804 nnx-0.0.1/nnx/filters.py
--rw-r--r--   0        0        0      140 2023-04-22 15:20:28.647804 nnx-0.0.1/nnx/nn/__init__.py
--rw-r--r--   0        0        0     1076 2023-04-22 15:20:28.647804 nnx-0.0.1/nnx/nn/activations.py
--rw-r--r--   0        0        0     2764 2023-04-08 19:11:50.337195 nnx-0.0.1/nnx/nn/dtypes.py
--rw-r--r--   0        0        0     1888 2023-04-08 18:42:49.425089 nnx-0.0.1/nnx/nn/initializers.py
--rw-r--r--   0        0        0    13270 2023-04-22 15:20:28.647804 nnx-0.0.1/nnx/nn/linear.py
--rw-r--r--   0        0        0     7325 2023-04-24 23:40:16.468746 nnx-0.0.1/nnx/nn/module.py
--rw-r--r--   0        0        0    10680 2023-04-22 15:20:28.647804 nnx-0.0.1/nnx/nn/normalization.py
--rw-r--r--   0        0        0     2250 2023-04-22 15:20:28.647804 nnx-0.0.1/nnx/nn/stochastic.py
--rw-r--r--   0        0        0     2431 2023-04-10 14:13:14.802122 nnx-0.0.1/nnx/partitioning.py
--rw-r--r--   0        0        0     2417 2023-03-30 22:50:08.758780 nnx-0.0.1/nnx/rng_stream.py
--rw-r--r--   0        0        0     5483 2023-04-22 15:20:28.647804 nnx-0.0.1/nnx/scope_lib.py
--rw-r--r--   0        0        0     6838 2023-04-22 15:20:28.647804 nnx-0.0.1/nnx/transforms.py
--rw-r--r--   0        0        0      563 2023-04-22 15:20:28.647804 nnx-0.0.1/nnx/utils.py
--rw-r--r--   0        0        0      751 2023-04-25 22:29:59.969018 nnx-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     4451 1970-01-01 00:00:00.000000 nnx-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-03-18 22:40:31.494888 nnx-0.0.2/LICENSE
+-rw-r--r--   0        0        0    13864 2023-04-26 21:37:05.662113 nnx-0.0.2/README.md
+-rw-r--r--   0        0        0      776 2023-04-22 15:20:28.647804 nnx-0.0.2/nnx/__init__.py
+-rw-r--r--   0        0        0     2235 2023-04-08 23:38:12.700869 nnx-0.0.2/nnx/fields.py
+-rw-r--r--   0        0        0     3789 2023-04-22 15:20:28.647804 nnx-0.0.2/nnx/filters.py
+-rw-r--r--   0        0        0      140 2023-04-22 15:20:28.647804 nnx-0.0.2/nnx/nn/__init__.py
+-rw-r--r--   0        0        0     1076 2023-04-22 15:20:28.647804 nnx-0.0.2/nnx/nn/activations.py
+-rw-r--r--   0        0        0     2764 2023-04-08 19:11:50.337195 nnx-0.0.2/nnx/nn/dtypes.py
+-rw-r--r--   0        0        0     1888 2023-04-08 18:42:49.425089 nnx-0.0.2/nnx/nn/initializers.py
+-rw-r--r--   0        0        0    13270 2023-04-22 15:20:28.647804 nnx-0.0.2/nnx/nn/linear.py
+-rw-r--r--   0        0        0     7341 2023-04-25 22:58:04.568349 nnx-0.0.2/nnx/nn/module.py
+-rw-r--r--   0        0        0    10680 2023-04-22 15:20:28.647804 nnx-0.0.2/nnx/nn/normalization.py
+-rw-r--r--   0        0        0     2250 2023-04-22 15:20:28.647804 nnx-0.0.2/nnx/nn/stochastic.py
+-rw-r--r--   0        0        0     2431 2023-04-10 14:13:14.802122 nnx-0.0.2/nnx/partitioning.py
+-rw-r--r--   0        0        0     2417 2023-03-30 22:50:08.758780 nnx-0.0.2/nnx/rng_stream.py
+-rw-r--r--   0        0        0     5483 2023-04-22 15:20:28.647804 nnx-0.0.2/nnx/scope_lib.py
+-rw-r--r--   0        0        0     6838 2023-04-22 15:20:28.647804 nnx-0.0.2/nnx/transforms.py
+-rw-r--r--   0        0        0      563 2023-04-22 15:20:28.647804 nnx-0.0.2/nnx/utils.py
+-rw-r--r--   0        0        0      751 2023-04-26 21:37:25.371790 nnx-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0    14363 1970-01-01 00:00:00.000000 nnx-0.0.2/PKG-INFO
```

### Comparing `nnx-0.0.1/LICENSE` & `nnx-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nnx-0.0.1/nnx/__init__.py` & `nnx-0.0.2/nnx/__init__.py`

 * *Files identical despite different names*

### Comparing `nnx-0.0.1/nnx/fields.py` & `nnx-0.0.2/nnx/fields.py`

 * *Files identical despite different names*

### Comparing `nnx-0.0.1/nnx/filters.py` & `nnx-0.0.2/nnx/filters.py`

 * *Files identical despite different names*

### Comparing `nnx-0.0.1/nnx/nn/activations.py` & `nnx-0.0.2/nnx/nn/activations.py`

 * *Files identical despite different names*

### Comparing `nnx-0.0.1/nnx/nn/dtypes.py` & `nnx-0.0.2/nnx/nn/dtypes.py`

 * *Files identical despite different names*

### Comparing `nnx-0.0.1/nnx/nn/initializers.py` & `nnx-0.0.2/nnx/nn/initializers.py`

 * *Files identical despite different names*

### Comparing `nnx-0.0.1/nnx/nn/linear.py` & `nnx-0.0.2/nnx/nn/linear.py`

 * *Files identical despite different names*

### Comparing `nnx-0.0.1/nnx/nn/module.py` & `nnx-0.0.2/nnx/nn/module.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,19 +39,19 @@
 
     def make_rng(self, collection: str) -> jax.random.KeyArray:
         return scope_lib.make_rng(collection)
 
     def get_flag(self, name: str, default: tp.Any = dataclasses.MISSING) -> tp.Any:
         return scope_lib.get_flag(name, default)
 
-    def __getitem__(self, filter: str) -> refx.Partition:
-        return partitioning.get_partition(self.deref()[0], filter)
+    def __getitem__(self, collection: str) -> refx.Partition:
+        return partitioning.get_partition(self.deref()[0], collection)
 
-    def __setitem__(self, filter: str, value: refx.Partition):
-        refx.update_refs(partitioning.get_partition(self, filter), value)
+    def __setitem__(self, collection: str, value: refx.Partition):
+        refx.update_refs(partitioning.get_partition(self, collection), value)
 
     def collections(self) -> tp.FrozenSet[str]:
         return frozenset(
             x.collection
             for x in jtu.tree_leaves(
                 self, is_leaf=lambda x: isinstance(x, refx.Referential)
             )
```

### Comparing `nnx-0.0.1/nnx/nn/normalization.py` & `nnx-0.0.2/nnx/nn/normalization.py`

 * *Files identical despite different names*

### Comparing `nnx-0.0.1/nnx/nn/stochastic.py` & `nnx-0.0.2/nnx/nn/stochastic.py`

 * *Files identical despite different names*

### Comparing `nnx-0.0.1/nnx/partitioning.py` & `nnx-0.0.2/nnx/partitioning.py`

 * *Files identical despite different names*

### Comparing `nnx-0.0.1/nnx/rng_stream.py` & `nnx-0.0.2/nnx/rng_stream.py`

 * *Files identical despite different names*

### Comparing `nnx-0.0.1/nnx/scope_lib.py` & `nnx-0.0.2/nnx/scope_lib.py`

 * *Files identical despite different names*

### Comparing `nnx-0.0.1/nnx/transforms.py` & `nnx-0.0.2/nnx/transforms.py`

 * *Files identical despite different names*

### Comparing `nnx-0.0.1/nnx/utils.py` & `nnx-0.0.2/nnx/utils.py`

 * *Files identical despite different names*

### Comparing `nnx-0.0.1/pyproject.toml` & `nnx-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nnx"
-version = "0.0.1"
+version = "0.0.2"
 description = ""
 authors = ["Cristian Garcia <cgarcia.e88@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 # refx = { path = "../refx", develop = true }
```

