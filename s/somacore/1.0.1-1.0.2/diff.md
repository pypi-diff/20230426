# Comparing `tmp/somacore-1.0.1.tar.gz` & `tmp/somacore-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "somacore-1.0.1.tar", last modified: Fri Mar 24 20:48:48 2023, max compression
+gzip compressed data, was "somacore-1.0.2.tar", last modified: Wed Apr 26 14:47:47 2023, max compression
```

## Comparing `somacore-1.0.1.tar` & `somacore-1.0.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 20:48:48.989274 somacore-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-03-24 20:48:30.000000 somacore-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-03-24 20:48:30.000000 somacore-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-03-24 20:48:48.989274 somacore-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-03-24 20:48:30.000000 somacore-1.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 20:48:48.985274 somacore-1.0.1/python-spec/
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-03-24 20:48:30.000000 somacore-1.0.1/python-spec/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 20:48:48.985274 somacore-1.0.1/python-spec/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 20:48:48.985274 somacore-1.0.1/python-spec/src/somacore/
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-03-24 20:48:30.000000 somacore-1.0.1/python-spec/src/somacore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-03-24 20:48:30.000000 somacore-1.0.1/python-spec/src/somacore/_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-24 20:48:48.000000 somacore-1.0.1/python-spec/src/somacore/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-03-24 20:48:30.000000 somacore-1.0.1/python-spec/src/somacore/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8891 2023-03-24 20:48:30.000000 somacore-1.0.1/python-spec/src/somacore/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    19796 2023-03-24 20:48:30.000000 somacore-1.0.1/python-spec/src/somacore/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 20:48:48.989274 somacore-1.0.1/python-spec/src/somacore/ephemeral/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-03-24 20:48:30.000000 somacore-1.0.1/python-spec/src/somacore/ephemeral/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-03-24 20:48:30.000000 somacore-1.0.1/python-spec/src/somacore/ephemeral/collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-03-24 20:48:30.000000 somacore-1.0.1/python-spec/src/somacore/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-03-24 20:48:30.000000 somacore-1.0.1/python-spec/src/somacore/measurement.py
--rw-r--r--   0 runner    (1001) docker     (123)     4948 2023-03-24 20:48:30.000000 somacore-1.0.1/python-spec/src/somacore/options.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-03-24 20:48:30.000000 somacore-1.0.1/python-spec/src/somacore/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 20:48:48.989274 somacore-1.0.1/python-spec/src/somacore/query/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-03-24 20:48:30.000000 somacore-1.0.1/python-spec/src/somacore/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-03-24 20:48:30.000000 somacore-1.0.1/python-spec/src/somacore/query/_eager_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-03-24 20:48:30.000000 somacore-1.0.1/python-spec/src/somacore/query/_fast_csr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-03-24 20:48:30.000000 somacore-1.0.1/python-spec/src/somacore/query/axis.py
--rw-r--r--   0 runner    (1001) docker     (123)    17973 2023-03-24 20:48:30.000000 somacore-1.0.1/python-spec/src/somacore/query/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-03-24 20:48:30.000000 somacore-1.0.1/python-spec/src/somacore/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 20:48:48.989274 somacore-1.0.1/python-spec/src/somacore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-03-24 20:48:48.000000 somacore-1.0.1/python-spec/src/somacore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-24 20:48:48.989274 somacore-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:47:47.685483 somacore-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-04-26 14:47:17.000000 somacore-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-26 14:47:17.000000 somacore-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-26 14:47:47.685483 somacore-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-26 14:47:17.000000 somacore-1.0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:47:47.685483 somacore-1.0.2/python-spec/
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-26 14:47:17.000000 somacore-1.0.2/python-spec/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:47:47.681483 somacore-1.0.2/python-spec/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:47:47.685483 somacore-1.0.2/python-spec/src/somacore/
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-26 14:47:17.000000 somacore-1.0.2/python-spec/src/somacore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-04-26 14:47:17.000000 somacore-1.0.2/python-spec/src/somacore/_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-26 14:47:47.000000 somacore-1.0.2/python-spec/src/somacore/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-04-26 14:47:17.000000 somacore-1.0.2/python-spec/src/somacore/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8891 2023-04-26 14:47:17.000000 somacore-1.0.2/python-spec/src/somacore/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19796 2023-04-26 14:47:17.000000 somacore-1.0.2/python-spec/src/somacore/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:47:47.685483 somacore-1.0.2/python-spec/src/somacore/ephemeral/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-26 14:47:17.000000 somacore-1.0.2/python-spec/src/somacore/ephemeral/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-04-26 14:47:17.000000 somacore-1.0.2/python-spec/src/somacore/ephemeral/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-04-26 14:47:17.000000 somacore-1.0.2/python-spec/src/somacore/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-04-26 14:47:17.000000 somacore-1.0.2/python-spec/src/somacore/measurement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-04-26 14:47:17.000000 somacore-1.0.2/python-spec/src/somacore/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-26 14:47:17.000000 somacore-1.0.2/python-spec/src/somacore/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:47:47.685483 somacore-1.0.2/python-spec/src/somacore/query/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-26 14:47:17.000000 somacore-1.0.2/python-spec/src/somacore/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-26 14:47:17.000000 somacore-1.0.2/python-spec/src/somacore/query/_eager_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-04-26 14:47:17.000000 somacore-1.0.2/python-spec/src/somacore/query/_fast_csr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-04-26 14:47:17.000000 somacore-1.0.2/python-spec/src/somacore/query/axis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18156 2023-04-26 14:47:17.000000 somacore-1.0.2/python-spec/src/somacore/query/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-04-26 14:47:17.000000 somacore-1.0.2/python-spec/src/somacore/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:47:47.685483 somacore-1.0.2/python-spec/src/somacore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-26 14:47:47.000000 somacore-1.0.2/python-spec/src/somacore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 14:47:47.685483 somacore-1.0.2/setup.cfg
```

### Comparing `somacore-1.0.1/LICENSE` & `somacore-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `somacore-1.0.1/PKG-INFO` & `somacore-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: somacore
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python-language API specification and base utilities for implementation of the SOMA system.
 Project-URL: repository, https://github.com/single-cell-data/SOMA.git
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `somacore-1.0.1/pyproject.toml` & `somacore-1.0.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,15 @@
   "anndata",
   "attrs>=22.1",
   "numba",
   "numpy>=1.21",
   "pandas",
   "pyarrow",
   "scipy",
-  "typing-extensions",
+  "typing-extensions>=4.1", # For LiteralString
 ]
 requires-python = "~=3.7"
 urls = { repository = "https://github.com/single-cell-data/SOMA.git" }
 classifiers = ["License :: OSI Approved :: MIT License"]
 
 [project.optional-dependencies]
 dev = ["black", "isort", "mypy~=1.0", "ruff"]
```

### Comparing `somacore-1.0.1/python-spec/README.md` & `somacore-1.0.2/python-spec/README.md`

 * *Files identical despite different names*

### Comparing `somacore-1.0.1/python-spec/src/somacore/__init__.py` & `somacore-1.0.2/python-spec/src/somacore/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 from .collection import Collection
 from .data import DataFrame
 from .data import DenseNDArray
 from .data import NDArray
 from .data import ReadIter
 from .data import SparseNDArray
 from .data import SparseRead
+from .experiment import Experiment
+from .measurement import Measurement
 from .options import BatchSize
 from .options import IOfN
 from .options import ResultOrder
 from .query import AxisColumnNames
 from .query import AxisQuery
 from .query import ExperimentAxisQuery
 
@@ -40,14 +42,16 @@
     "Collection",
     "DataFrame",
     "DenseNDArray",
     "NDArray",
     "ReadIter",
     "SparseNDArray",
     "SparseRead",
+    "Experiment",
+    "Measurement",
     "BatchSize",
     "IOfN",
     "ResultOrder",
     "AxisColumnNames",
     "AxisQuery",
     "ExperimentAxisQuery",
 )
```

### Comparing `somacore-1.0.1/python-spec/src/somacore/_mixin.py` & `somacore-1.0.2/python-spec/src/somacore/_mixin.py`

 * *Files identical despite different names*

### Comparing `somacore-1.0.1/python-spec/src/somacore/base.py` & `somacore-1.0.2/python-spec/src/somacore/base.py`

 * *Files identical despite different names*

### Comparing `somacore-1.0.1/python-spec/src/somacore/collection.py` & `somacore-1.0.2/python-spec/src/somacore/collection.py`

 * *Files identical despite different names*

### Comparing `somacore-1.0.1/python-spec/src/somacore/data.py` & `somacore-1.0.2/python-spec/src/somacore/data.py`

 * *Files identical despite different names*

### Comparing `somacore-1.0.1/python-spec/src/somacore/ephemeral/collections.py` & `somacore-1.0.2/python-spec/src/somacore/ephemeral/collections.py`

 * *Files identical despite different names*

### Comparing `somacore-1.0.1/python-spec/src/somacore/experiment.py` & `somacore-1.0.2/python-spec/src/somacore/experiment.py`

 * *Files identical despite different names*

### Comparing `somacore-1.0.1/python-spec/src/somacore/measurement.py` & `somacore-1.0.2/python-spec/src/somacore/measurement.py`

 * *Files 5% similar despite different names*

```diff
@@ -72,27 +72,27 @@
     X = _mixin.item[_NDColl]()
     """A collection of matrices containing feature values.
 
     Each matrix is indexed by ``[obsid, varid]``. Sparse and dense 2D arrays may
     both be used in any combination in ``X``.
     """
 
-    obsm = _mixin.item[_DenseNDColl]()
+    obsm = _mixin.item[_NDColl]()
     """Matrices containing annotations of each ``obs`` row.
 
     This has the same shape as ``obs`` and is indexed with ``obsid``.
     """
 
     obsp = _mixin.item[_SparseNDColl]()
     """Matrices containg pairwise annotations of each ``obs`` row.
 
     This is indexed by ``[obsid_1, obsid_2]``.
     """
 
-    varm = _mixin.item[_DenseNDColl]()
+    varm = _mixin.item[_NDColl]()
     """Matrices containing annotations of each ``var`` row.
 
     This has the same shape as ``var`` and is indexed with ``varid``.
     """
 
     varp = _mixin.item[_SparseNDColl]()
     """Matrices containg pairwise annotations of each ``var`` row.
```

### Comparing `somacore-1.0.1/python-spec/src/somacore/options.py` & `somacore-1.0.2/python-spec/src/somacore/options.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,14 +109,15 @@
 an implementation-defined configuration structure.
 """
 
 
 class ResultOrder(enum.Enum):
     """
     The order results should be returned in.
+
     Lifecycle:
         Experimental
     """
 
     AUTO = "auto"
     ROW_MAJOR = "row-major"
     COLUMN_MAJOR = "column-major"
```

### Comparing `somacore-1.0.1/python-spec/src/somacore/query/_eager_iter.py` & `somacore-1.0.2/python-spec/src/somacore/query/_eager_iter.py`

 * *Files identical despite different names*

### Comparing `somacore-1.0.1/python-spec/src/somacore/query/_fast_csr.py` & `somacore-1.0.2/python-spec/src/somacore/query/_fast_csr.py`

 * *Files identical despite different names*

### Comparing `somacore-1.0.1/python-spec/src/somacore/query/axis.py` & `somacore-1.0.2/python-spec/src/somacore/query/axis.py`

 * *Files identical despite different names*

### Comparing `somacore-1.0.1/python-spec/src/somacore/query/query.py` & `somacore-1.0.2/python-spec/src/somacore/query/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 """TypeVar for the concrete type of an experiment-like object."""
 
 
 class ExperimentAxisQuery(Generic[_Exp]):
     """Axis-based query against a SOMA Experiment.
 
     ExperimentAxisQuery allows easy selection and extraction of data from a
-    single soma.Measurement in a soma.Experiment, by obs/var (axis) coordinates
+    single :class:`Measurement` in an :class:`Experiment`, by obs/var (axis) coordinates
     and/or value filter.
 
     The primary use for this class is slicing :class:`Experiment` ``X`` layers by obs or
     var value and/or coordinates. Slicing on :class:`SparseNDArray` ``X`` matrices is
     supported; :class:`DenseNDArray` is not supported at this time.
 
     IMPORTANT: this class is not thread-safe.
@@ -95,29 +95,33 @@
         self._joinids = _JoinIDCache(self)
         self._indexer = AxisIndexer(self)
         self._threadpool_: Optional[futures.ThreadPoolExecutor] = None
 
     def obs(
         self, *, column_names: Optional[Sequence[str]] = None
     ) -> data.ReadIter[pa.Table]:
-        """Returns ``obs`` as an Arrow table iterator.
+        """Returns ``obs`` as an `Arrow table
+        <https://arrow.apache.org/docs/python/generated/pyarrow.Table.html>`_
+        iterator.
 
         Lifecycle: experimental
         """
         obs_query = self._matrix_axis_query.obs
         return self._obs_df.read(
             obs_query.coords,
             value_filter=obs_query.value_filter,
             column_names=column_names,
         )
 
     def var(
         self, *, column_names: Optional[Sequence[str]] = None
     ) -> data.ReadIter[pa.Table]:
-        """Returns ``var`` as an Arrow table iterator.
+        """Returns ``var`` as an `Arrow table
+        <https://arrow.apache.org/docs/python/generated/pyarrow.Table.html>`_
+        iterator.
 
         Lifecycle: experimental
         """
         var_query = self._matrix_axis_query.var
         return self._var_df.read(
             var_query.coords,
             value_filter=var_query.value_filter,
```

### Comparing `somacore-1.0.1/python-spec/src/somacore/types.py` & `somacore-1.0.2/python-spec/src/somacore/types.py`

 * *Files identical despite different names*

### Comparing `somacore-1.0.1/python-spec/src/somacore.egg-info/SOURCES.txt` & `somacore-1.0.2/python-spec/src/somacore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

