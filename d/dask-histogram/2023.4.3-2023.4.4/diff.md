# Comparing `tmp/dask_histogram-2023.4.3.tar.gz` & `tmp/dask_histogram-2023.4.4.tar.gz`

## Comparing `dask_histogram-2023.4.3.tar` & `dask_histogram-2023.4.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 dask_histogram-2023.4.3/src/dask_histogram/__init__.py
--rw-r--r--   0        0        0     6417 2020-02-02 00:00:00.000000 dask_histogram-2023.4.3/src/dask_histogram/bins.py
--rw-r--r--   0        0        0    29283 2020-02-02 00:00:00.000000 dask_histogram-2023.4.3/src/dask_histogram/boost.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 dask_histogram-2023.4.3/src/dask_histogram/config.py
--rw-r--r--   0        0        0    38929 2020-02-02 00:00:00.000000 dask_histogram-2023.4.3/src/dask_histogram/core.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 dask_histogram-2023.4.3/src/dask_histogram/histogram.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dask_histogram-2023.4.3/src/dask_histogram/py.typed
--rw-r--r--   0        0        0    16836 2020-02-02 00:00:00.000000 dask_histogram-2023.4.3/src/dask_histogram/routines.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 dask_histogram-2023.4.3/src/dask_histogram/sizeof.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 dask_histogram-2023.4.3/src/dask_histogram/typing.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 dask_histogram-2023.4.3/src/dask_histogram/version.py
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 dask_histogram-2023.4.3/.gitignore
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 dask_histogram-2023.4.3/LICENSE
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 dask_histogram-2023.4.3/README.md
--rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 dask_histogram-2023.4.3/pyproject.toml
--rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 dask_histogram-2023.4.3/PKG-INFO
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 dask_histogram-2023.4.4/src/dask_histogram/__init__.py
+-rw-r--r--   0        0        0     6417 2020-02-02 00:00:00.000000 dask_histogram-2023.4.4/src/dask_histogram/bins.py
+-rw-r--r--   0        0        0    29302 2020-02-02 00:00:00.000000 dask_histogram-2023.4.4/src/dask_histogram/boost.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 dask_histogram-2023.4.4/src/dask_histogram/config.py
+-rw-r--r--   0        0        0    38929 2020-02-02 00:00:00.000000 dask_histogram-2023.4.4/src/dask_histogram/core.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 dask_histogram-2023.4.4/src/dask_histogram/histogram.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dask_histogram-2023.4.4/src/dask_histogram/py.typed
+-rw-r--r--   0        0        0    16836 2020-02-02 00:00:00.000000 dask_histogram-2023.4.4/src/dask_histogram/routines.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 dask_histogram-2023.4.4/src/dask_histogram/sizeof.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 dask_histogram-2023.4.4/src/dask_histogram/typing.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 dask_histogram-2023.4.4/src/dask_histogram/version.py
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 dask_histogram-2023.4.4/.gitignore
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 dask_histogram-2023.4.4/LICENSE
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 dask_histogram-2023.4.4/README.md
+-rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 dask_histogram-2023.4.4/pyproject.toml
+-rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 dask_histogram-2023.4.4/PKG-INFO
```

### Comparing `dask_histogram-2023.4.3/src/dask_histogram/__init__.py` & `dask_histogram-2023.4.4/src/dask_histogram/__init__.py`

 * *Files identical despite different names*

### Comparing `dask_histogram-2023.4.3/src/dask_histogram/bins.py` & `dask_histogram-2023.4.4/src/dask_histogram/bins.py`

 * *Files identical despite different names*

### Comparing `dask_histogram-2023.4.3/src/dask_histogram/boost.py` & `dask_histogram-2023.4.4/src/dask_histogram/boost.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,18 +83,21 @@
         metadata: Any = None,
     ) -> None:
         """Construct a Histogram object."""
         super().__init__(*axes, storage=storage, metadata=metadata)
         self._staged: AggHistogram | None = None
         self._dask_name: str | None = None
         self._dask: HighLevelGraph | None = None
-        self._histref = (
-            axes if isinstance(axes, tuple) else (axes,),
-            storage,
-            metadata,
+
+    @property
+    def _histref(self):
+        return (
+            tuple(self.axes),
+            self.storage_type(),
+            self.metadata,
         )
 
     def __iadd__(self, other):
         if self.staged_fills() and other.staged_fills():
             self._staged += other._staged
         elif not self.staged_fills() and other.staged_fills():
             self._staged = other._staged
```

### Comparing `dask_histogram-2023.4.3/src/dask_histogram/core.py` & `dask_histogram-2023.4.4/src/dask_histogram/core.py`

 * *Files identical despite different names*

### Comparing `dask_histogram-2023.4.3/src/dask_histogram/routines.py` & `dask_histogram-2023.4.4/src/dask_histogram/routines.py`

 * *Files identical despite different names*

### Comparing `dask_histogram-2023.4.3/src/dask_histogram/sizeof.py` & `dask_histogram-2023.4.4/src/dask_histogram/sizeof.py`

 * *Files identical despite different names*

### Comparing `dask_histogram-2023.4.3/.gitignore` & `dask_histogram-2023.4.4/.gitignore`

 * *Files identical despite different names*

### Comparing `dask_histogram-2023.4.3/LICENSE` & `dask_histogram-2023.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dask_histogram-2023.4.3/README.md` & `dask_histogram-2023.4.4/README.md`

 * *Files identical despite different names*

### Comparing `dask_histogram-2023.4.3/pyproject.toml` & `dask_histogram-2023.4.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dask_histogram-2023.4.3/PKG-INFO` & `dask_histogram-2023.4.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-histogram
-Version: 2023.4.3
+Version: 2023.4.4
 Summary: Histogramming with Dask.
 Project-URL: Homepage, https://github.com/dask-contrib/dask-histogram
 Project-URL: Documentation, https://dask-histogram.readthedocs.io/
 Project-URL: Bug Tracker, https://github.com/dask-contrib/dask-histogram/issues
 Author-email: Doug Davis <ddavis@ddavis.io>
 License: BSD-3-Clause
 License-File: LICENSE
```

