# Comparing `tmp/dask_awkward-2023.4.1.tar.gz` & `tmp/dask_awkward-2023.4.2.tar.gz`

## Comparing `dask_awkward-2023.4.1.tar` & `dask_awkward-2023.4.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 dask_awkward-2023.4.1/src/dask_awkward/__init__.py
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 dask_awkward-2023.4.1/src/dask_awkward/awkward.yaml
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 dask_awkward-2023.4.1/src/dask_awkward/config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dask_awkward-2023.4.1/src/dask_awkward/py.typed
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 dask_awkward-2023.4.1/src/dask_awkward/sizeof.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 dask_awkward-2023.4.1/src/dask_awkward/typing.py
--rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 dask_awkward-2023.4.1/src/dask_awkward/utils.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 dask_awkward-2023.4.1/src/dask_awkward/version.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 dask_awkward-2023.4.1/src/dask_awkward/version.pyi
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 dask_awkward-2023.4.1/src/dask_awkward/layers/__init__.py
--rw-r--r--   0        0        0     5759 2020-02-02 00:00:00.000000 dask_awkward-2023.4.1/src/dask_awkward/layers/layers.py
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 dask_awkward-2023.4.1/src/dask_awkward/lib/__init__.py
--rw-r--r--   0        0        0    61222 2020-02-02 00:00:00.000000 dask_awkward-2023.4.1/src/dask_awkward/lib/core.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 dask_awkward-2023.4.1/src/dask_awkward/lib/describe.py
--rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 dask_awkward-2023.4.1/src/dask_awkward/lib/inspect.py
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 dask_awkward-2023.4.1/src/dask_awkward/lib/operations.py
--rw-r--r--   0        0        0    10409 2020-02-02 00:00:00.000000 dask_awkward-2023.4.1/src/dask_awkward/lib/optimize.py
--rw-r--r--   0        0        0    11155 2020-02-02 00:00:00.000000 dask_awkward-2023.4.1/src/dask_awkward/lib/reducers.py
--rw-r--r--   0        0        0    28745 2020-02-02 00:00:00.000000 dask_awkward-2023.4.1/src/dask_awkward/lib/structure.py
--rw-r--r--   0        0        0     5894 2020-02-02 00:00:00.000000 dask_awkward-2023.4.1/src/dask_awkward/lib/testutils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dask_awkward-2023.4.1/src/dask_awkward/lib/io/__init__.py
--rw-r--r--   0        0        0    15332 2020-02-02 00:00:00.000000 dask_awkward-2023.4.1/src/dask_awkward/lib/io/io.py
--rw-r--r--   0        0        0    15172 2020-02-02 00:00:00.000000 dask_awkward-2023.4.1/src/dask_awkward/lib/io/json.py
--rw-r--r--   0        0        0    14183 2020-02-02 00:00:00.000000 dask_awkward-2023.4.1/src/dask_awkward/lib/io/parquet.py
--rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 dask_awkward-2023.4.1/.gitignore
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 dask_awkward-2023.4.1/LICENSE
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 dask_awkward-2023.4.1/README.md
--rw-r--r--   0        0        0     3480 2020-02-02 00:00:00.000000 dask_awkward-2023.4.1/pyproject.toml
--rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 dask_awkward-2023.4.1/PKG-INFO
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 dask_awkward-2023.4.2/src/dask_awkward/__init__.py
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 dask_awkward-2023.4.2/src/dask_awkward/awkward.yaml
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 dask_awkward-2023.4.2/src/dask_awkward/config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dask_awkward-2023.4.2/src/dask_awkward/py.typed
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 dask_awkward-2023.4.2/src/dask_awkward/sizeof.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 dask_awkward-2023.4.2/src/dask_awkward/typing.py
+-rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 dask_awkward-2023.4.2/src/dask_awkward/utils.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 dask_awkward-2023.4.2/src/dask_awkward/version.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 dask_awkward-2023.4.2/src/dask_awkward/version.pyi
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 dask_awkward-2023.4.2/src/dask_awkward/layers/__init__.py
+-rw-r--r--   0        0        0     6836 2020-02-02 00:00:00.000000 dask_awkward-2023.4.2/src/dask_awkward/layers/layers.py
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 dask_awkward-2023.4.2/src/dask_awkward/lib/__init__.py
+-rw-r--r--   0        0        0    61405 2020-02-02 00:00:00.000000 dask_awkward-2023.4.2/src/dask_awkward/lib/core.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 dask_awkward-2023.4.2/src/dask_awkward/lib/describe.py
+-rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 dask_awkward-2023.4.2/src/dask_awkward/lib/inspect.py
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 dask_awkward-2023.4.2/src/dask_awkward/lib/operations.py
+-rw-r--r--   0        0        0    10884 2020-02-02 00:00:00.000000 dask_awkward-2023.4.2/src/dask_awkward/lib/optimize.py
+-rw-r--r--   0        0        0    11155 2020-02-02 00:00:00.000000 dask_awkward-2023.4.2/src/dask_awkward/lib/reducers.py
+-rw-r--r--   0        0        0    28896 2020-02-02 00:00:00.000000 dask_awkward-2023.4.2/src/dask_awkward/lib/structure.py
+-rw-r--r--   0        0        0     5894 2020-02-02 00:00:00.000000 dask_awkward-2023.4.2/src/dask_awkward/lib/testutils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dask_awkward-2023.4.2/src/dask_awkward/lib/io/__init__.py
+-rw-r--r--   0        0        0    15411 2020-02-02 00:00:00.000000 dask_awkward-2023.4.2/src/dask_awkward/lib/io/io.py
+-rw-r--r--   0        0        0    15172 2020-02-02 00:00:00.000000 dask_awkward-2023.4.2/src/dask_awkward/lib/io/json.py
+-rw-r--r--   0        0        0    14183 2020-02-02 00:00:00.000000 dask_awkward-2023.4.2/src/dask_awkward/lib/io/parquet.py
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 dask_awkward-2023.4.2/.gitignore
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 dask_awkward-2023.4.2/LICENSE
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 dask_awkward-2023.4.2/README.md
+-rw-r--r--   0        0        0     3480 2020-02-02 00:00:00.000000 dask_awkward-2023.4.2/pyproject.toml
+-rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 dask_awkward-2023.4.2/PKG-INFO
```

### Comparing `dask_awkward-2023.4.1/src/dask_awkward/awkward.yaml` & `dask_awkward-2023.4.2/src/dask_awkward/awkward.yaml`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.4.1/src/dask_awkward/typing.py` & `dask_awkward-2023.4.2/src/dask_awkward/typing.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.4.1/src/dask_awkward/utils.py` & `dask_awkward-2023.4.2/src/dask_awkward/utils.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.4.1/src/dask_awkward/layers/layers.py` & `dask_awkward-2023.4.2/src/dask_awkward/layers/layers.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,58 @@
 from __future__ import annotations
 
 import copy
+import pickle
 from collections.abc import Callable, Mapping
 from typing import TYPE_CHECKING, Any
 
 from dask.blockwise import Blockwise, BlockwiseDepDict, blockwise_token
 
 from dask_awkward.utils import LazyInputsDict
 
 if TYPE_CHECKING:
     from awkward._nplikes.typetracer import TypeTracerReport
 
 
-class AwkwardInputLayer(Blockwise):
+class AwkwardBlockwiseLayer(Blockwise):
+    """Just like upstream Blockwise, except we override pickling"""
+
+    @classmethod
+    def from_blockwise(cls, layer) -> AwkwardBlockwiseLayer:
+        ob = object.__new__(cls)
+        ob.__dict__.update(layer.__dict__)
+        return ob
+
+    def mock(self):
+        layer = copy.copy(self)
+        nb = layer.numblocks
+        layer.numblocks = {k: tuple(1 for _ in v) for k, v in nb.items()}
+        layer.__dict__.pop("_dims", None)
+        return layer
+
+    def __getstate__(self) -> dict:
+        d = self.__dict__.copy()
+        try:
+            pickle.dumps(d["_meta"])
+        except (ValueError, TypeError, KeyError):
+            d.pop(
+                "_meta", None
+            )  # must be a typetracer, does not pickle and not needed on scheduler
+        return d
+
+    def __repr__(self) -> str:
+        return "Awkward" + super().__repr__()
+
+
+class AwkwardInputLayer(AwkwardBlockwiseLayer):
+    """A layer known to perform IO and produce Awkward arrays
+
+    We specialise this so that we have a way to prune column selection on load
+    """
+
     def __init__(
         self,
         *,
         name: str,
         columns: str | list[str] | None,
         inputs: Any,
         io_func: Callable,
@@ -110,15 +146,15 @@
         set_form_keys(form, key=self.name)
 
         new_meta_labelled, report = ak._nplikes.typetracer.typetracer_with_report(form)
         new_meta_array = ak.Array(new_meta_labelled, behavior=self._behavior)
         new_input_layer = AwkwardInputLayer(
             name=self.name,
             columns=self.columns,
-            inputs=[None] * int(list(self.numblocks.values())[0][0]),
+            inputs=[None][: int(list(self.numblocks.values())[0][0])],
             io_func=lambda *_, **__: new_meta_array,
             label=self.label,
             produces_tasks=self.produces_tasks,
             creation_info=self.creation_info,
             annotations=self.annotations,
             meta=new_meta_array,
             behavior=self._behavior,
```

### Comparing `dask_awkward-2023.4.1/src/dask_awkward/lib/__init__.py` & `dask_awkward-2023.4.2/src/dask_awkward/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.4.1/src/dask_awkward/lib/core.py` & `dask_awkward-2023.4.2/src/dask_awkward/lib/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 from dask.delayed import Delayed
 from dask.highlevelgraph import HighLevelGraph
 from dask.threaded import get as threaded_get
 from dask.utils import IndexCallable, funcname, key_split
 from numpy.lib.mixins import NDArrayOperatorsMixin
 from tlz import first
 
+from dask_awkward.layers import AwkwardBlockwiseLayer
 from dask_awkward.lib.optimize import all_optimizations
 from dask_awkward.typing import AwkwardDaskCollection
 from dask_awkward.utils import (
     DaskAwkwardNotImplemented,
     IncompatiblePartitions,
     hyphenize,
     is_empty_slice,
@@ -44,15 +45,14 @@
 if TYPE_CHECKING:
     from awkward.contents.content import Content
     from awkward.forms.form import Form
     from awkward.types.arraytype import ArrayType
     from awkward.types.type import Type
     from dask.array.core import Array as DaskArray
     from dask.bag.core import Bag as DaskBag
-    from dask.blockwise import Blockwise
     from numpy.typing import DTypeLike
 
 
 T = TypeVar("T")
 
 
 log = logging.getLogger(__name__)
@@ -484,15 +484,17 @@
         meta: ak.Array,
         divisions: tuple[int | None, ...],
     ) -> None:
         self._dask: HighLevelGraph = dsk
         if hasattr(dsk, "layers"):
             # i.e., NOT matrializes/persisted state
             # output typetracer
-            list(dsk.layers.values())[-1]._meta = meta  # type: ignore
+            lay = list(dsk.layers.values())[-1]
+            if isinstance(lay, AwkwardBlockwiseLayer):
+                lay._meta = meta  # type: ignore
         self._name: str = name
         self._divisions: tuple[int | None, ...] = divisions
         self._meta: ak.Array = meta
 
     def __dask_graph__(self) -> HighLevelGraph:
         return self.dask
 
@@ -520,17 +522,17 @@
     def __setitem__(self, where: Any, what: Any) -> None:
         if not (
             isinstance(where, str)
             or (isinstance(where, tuple) and all(isinstance(x, str) for x in where))
         ):
             raise TypeError("only fields may be assigned in-place (by field name)")
 
-        if not isinstance(what, Array):
+        if not isinstance(what, (Array, Number)):
             raise DaskAwkwardNotImplemented(
-                "Supplying anything other than a dak.Array to __setitem__ is not yet available!"
+                "Supplying anything other than a dak.Array, or Number to __setitem__ is not yet available!"
             )
 
         from dask_awkward.lib.structure import with_field
 
         appended = with_field(self, what, where=where, behavior=self.behavior)
 
         self._meta = appended._meta
@@ -1284,15 +1286,15 @@
 
 def partitionwise_layer(
     func: Callable,
     name: str,
     *args: Any,
     opt_touch_all: bool = False,
     **kwargs: Any,
-) -> Blockwise:
+) -> AwkwardBlockwiseLayer:
     """Create a partitionwise graph layer.
 
     Parameters
     ----------
     func : Callable
         Function to apply on all partitions.
     name : str
@@ -1330,14 +1332,15 @@
         name,
         "i",
         *pairs,
         numblocks=numblocks,
         concatenate=True,
         **kwargs,
     )
+    layer = AwkwardBlockwiseLayer.from_blockwise(layer)
     if opt_touch_all:
         layer._opt_touch_all = True
     return layer
 
 
 def map_partitions(
     fn: Callable,
```

### Comparing `dask_awkward-2023.4.1/src/dask_awkward/lib/describe.py` & `dask_awkward-2023.4.2/src/dask_awkward/lib/describe.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.4.1/src/dask_awkward/lib/inspect.py` & `dask_awkward-2023.4.2/src/dask_awkward/lib/inspect.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.4.1/src/dask_awkward/lib/operations.py` & `dask_awkward-2023.4.2/src/dask_awkward/lib/operations.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.4.1/src/dask_awkward/lib/optimize.py` & `dask_awkward-2023.4.2/src/dask_awkward/lib/optimize.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,14 +126,16 @@
         column-projectable.
 
     """
     return [
         n
         for n, v in dsk.layers.items()
         if isinstance(v, AwkwardInputLayer) and hasattr(v.io_func, "project_columns")
+        # following condition means dep/pickled layers cannot be optimised
+        and hasattr(v, "_meta")
     ]
 
 
 def _layers_with_annotation(dsk: HighLevelGraph, key: str) -> list[str]:
     return [n for n, v in dsk.layers.items() if (v.annotations or {}).get(key)]
 
 
@@ -179,34 +181,34 @@
 
 
 def _mock_output(layer):
     """Update a layer to run the _touch_all_data."""
     assert len(layer.dsk) == 1
 
     new_layer = copy.deepcopy(layer)
-    mp = new_layer.mapping.copy()
+    mp = new_layer.dsk.copy()
     for k in iter(mp.keys()):
         mp[k] = (_touch_all_data,) + mp[k][1:]
-    new_layer.mapping = mp
+    new_layer.dsk = mp
     return new_layer
 
 
 def _touch_and_call_fn(fn, *args, **kwargs):
     _touch_all_data(*args, **kwargs)
     return fn(*args, **kwargs)
 
 
 def _touch_and_call(layer):
     assert len(layer.dsk) == 1
 
     new_layer = copy.deepcopy(layer)
-    mp = new_layer.mapping.copy()
+    mp = new_layer.dsk.copy()
     for k in iter(mp.keys()):
         mp[k] = (_touch_and_call_fn,) + mp[k]
-    new_layer.mapping = mp
+    new_layer.dsk = mp
     return new_layer
 
 
 def _get_column_reports(dsk: HighLevelGraph) -> dict[str, Any]:
     """Get the TypeTracerReport for each input layer in a task graph."""
     if not _has_projectable_awkward_io_layer(dsk):
         return {}
@@ -214,28 +216,38 @@
     import awkward as ak
 
     layers = dsk.layers.copy()  # type: ignore
     deps = dsk.dependencies.copy()  # type: ignore
     reports = {}
 
     # make labelled report
+    projectable = _projectable_input_layer_names(dsk)
+    for name, lay in dsk.layers.copy().items():
+        if name in projectable:
+            layers[name], report = lay.mock()
+            reports[name] = report
+        elif hasattr(lay, "mock"):
+            layers[name] = lay.mock()
+
     for name in _projectable_input_layer_names(dsk):
         layers[name], report = layers[name].mock()
         reports[name] = report
 
     for name in _ak_output_layer_names(dsk):
         layers[name] = _mock_output(layers[name])
 
     for name in _opt_touch_all_layer_names(dsk):
         layers[name] = _touch_and_call(layers[name])
 
     hlg = HighLevelGraph(layers, deps)
     outlayer = hlg.layers[hlg._toposort_layers()[-1]]
 
     try:
+        for layer in hlg.layers.values():
+            layer.__dict__.pop("_cached_dict", None)
         out = get_sync(hlg, list(outlayer.keys())[0])
     except Exception as err:
         on_fail = dask.config.get("awkward.optimization.on-fail")
         # this is the default, throw a warning but skip the optimization.
         if on_fail == "warn":
             warnings.warn(f"Column projection optimization failed: {type(err)}, {err}")
             return {}
```

### Comparing `dask_awkward-2023.4.1/src/dask_awkward/lib/reducers.py` & `dask_awkward-2023.4.2/src/dask_awkward/lib/reducers.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.4.1/src/dask_awkward/lib/structure.py` & `dask_awkward-2023.4.2/src/dask_awkward/lib/structure.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from __future__ import annotations
 
 import builtins
 import warnings
 from collections.abc import Sequence
+from numbers import Number
 from typing import TYPE_CHECKING, Any
 
 import awkward as ak
 import numpy as np
 from awkward._nplikes.typetracer import TypeTracerArray
+from dask.base import is_dask_collection
 
 from dask_awkward.lib.core import (
     Array,
     compatible_partitions,
     map_partitions,
     new_known_scalar,
     total_reduction_to_scalar,
@@ -427,70 +429,44 @@
     if dtype is str:
         raise ValueError(
             """dtype cannot be 'str' for dak.full_like,
             you can accomplish this with dask-array and
             dak.flatten/dak.unflatten"""
         )
 
-    #  TODO: fix when available in awkward
-    meta = typetracer_from_form(
-        ak.full_like(
-            array._meta.layout.form.length_zero_array(behavior=array.behavior),
-            fill_value,
-            highlevel=highlevel,
-            behavior=behavior,
-            dtype=dtype,
-        ).layout.form
-    )
-
     return map_partitions(
         ak.full_like,
         array,
         fill_value,
         highlevel=highlevel,
         behavior=behavior,
         dtype=dtype,
-        meta=meta,
     )
 
 
 @borrow_docstring(ak.isclose)
 def isclose(
     a, b, rtol=1e-05, atol=1e-08, equal_nan=False, highlevel=True, behavior=None
 ):
     if not highlevel:
         raise ValueError("Only highlevel=True is supported")
 
     if not compatible_partitions(a, b):
         raise IncompatiblePartitions("isclose", a, b)
 
-    #  TODO: fix this when https://github.com/scikit-hep/awkward/issues/2124 is addressed
-    meta = typetracer_from_form(
-        ak.isclose(
-            a._meta.layout.form.length_zero_array(behavior=a.behavior),
-            b._meta.layout.form.length_zero_array(behavior=b.behavior),
-            rtol=rtol,
-            atol=atol,
-            equal_nan=equal_nan,
-            highlevel=highlevel,
-            behavior=behavior,
-        ).layout.form
-    )
-
     return map_partitions(
         ak.isclose,
         a,
         b,
         rtol=rtol,
         atol=atol,
         equal_nan=equal_nan,
         highlevel=highlevel,
         behavior=behavior,
         label="is-close",
-        meta=meta,
     )
 
 
 class _IsNoneFn:
     def __init__(self, **kwargs):
         self.kwargs = kwargs
 
@@ -502,15 +478,26 @@
 def is_none(array, axis=0, highlevel=True, behavior=None):
     fn = _IsNoneFn(axis=axis, highlevel=highlevel, behavior=behavior)
     return map_partitions(fn, array, label="is-none", output_divisions=1)
 
 
 @borrow_docstring(ak.local_index)
 def local_index(array, axis=-1, highlevel=True, behavior=None):
-    raise DaskAwkwardNotImplemented("TODO")
+    if not highlevel:
+        raise ValueError("Only highlevel=True is supported")
+    if axis == 0:
+        DaskAwkwardNotImplemented("axis=0 for local_index is not supported")
+    if axis and axis != 0:
+        return map_partitions(
+            ak.local_index,
+            array,
+            axis=axis,
+            highlevel=highlevel,
+            behavior=behavior,
+        )
 
 
 @borrow_docstring(ak.mask)
 def mask(array, mask, valid_when=True, highlevel=True, behavior=None):
     # if not compatible_partitions(array, mask):
     #     raise IncompatiblePartitions("mask", array, mask)
     # return map_partitions(
@@ -677,56 +664,53 @@
     # TODO: fix incorrect results for run_lengths when one dimensional
     minmax_depth = array._meta.layout.minmax_depth
     if minmax_depth[0] == 1 or minmax_depth[1] == 1:
         warnings.warn(
             "run_lengths can produce incorrect results for one dimensional arrays!"
         )
 
-    # TODO: fix typetracer error in awkward
-    meta = typetracer_from_form(
-        ak.run_lengths(
-            array._meta.layout.form.length_zero_array(behavior=array.behavior),
-            highlevel=highlevel,
-            behavior=behavior,
-        ).layout.form
-    )
-
     return map_partitions(
         ak.run_lengths,
         array,
         highlevel=highlevel,
         behavior=behavior,
         label="run-lengths",
-        meta=meta,
     )
 
 
+class _SingletonsFn:
+    def __init__(self, axis, **kwargs):
+        self.axis = axis
+        self.kwargs = kwargs
+
+    def __call__(self, array):
+        # TODO: remove this length-zero calculation once https://github.com/scikit-hep/awkward/issues/2123 is addressed
+        if ak.backend(array) == "typetracer":
+            array.layout._touch_data(recursive=False)
+            zl_out = ak.singletons(
+                array.layout.form.length_zero_array(behavior=array.behavior),
+                axis=self.axis,
+                **self.kwargs,
+            )
+            return ak.Array(
+                zl_out.layout.to_typetracer(forget_length=True),
+                behavior=zl_out.behavior,
+            )
+        return ak.singletons(array, axis=self.axis, **self.kwargs)
+
+
 @borrow_docstring(ak.singletons)
 def singletons(array, axis=0, highlevel=True, behavior=None):
     if not highlevel:
         raise ValueError("Only highlevel=True is supported")
 
-    # TODO: remove this length-zero calculation once https://github.com/scikit-hep/awkward/issues/2123 is addressed
-    meta = typetracer_from_form(
-        ak.singletons(
-            array._meta.layout.form.length_zero_array(behavior=array.behavior),
-            axis=axis,
-            highlevel=highlevel,
-            behavior=behavior,
-        ).layout.form
-    )
-
     return map_partitions(
-        ak.singletons,
+        _SingletonsFn(axis, highlevel=highlevel, behavior=behavior),
         array,
-        axis=axis,
-        highlevel=highlevel,
-        behavior=behavior,
         label="singletons",
-        meta=meta,
     )
 
 
 class _SortFn:
     def __init__(self, **kwargs):
         self.kwargs = kwargs
 
@@ -863,16 +847,26 @@
     y: Array,
     mergebool: bool = True,
     highlevel: bool = True,
     behavior: dict | None = None,
 ) -> Array:
     if not highlevel:
         raise ValueError("Only highlevel=True is supported")
-    if not compatible_partitions(condition, x, y):
-        raise IncompatiblePartitions("where", condition, x, y)
+
+    maybe_dask_args = [condition, x, y]
+    dask_args = tuple(arg for arg in maybe_dask_args if is_dask_collection(arg))
+
+    if not isinstance(condition, Array):
+        raise ValueError(
+            "The condition argugment to where must be a dask_awkward.Array"
+        )
+
+    if not compatible_partitions(*dask_args):
+        raise IncompatiblePartitions("where", *dask_args)
+
     return map_partitions(
         _WhereFn(mergebool=mergebool, highlevel=highlevel, behavior=behavior),
         condition,
         x,
         y,
         label="where",
     )
@@ -886,31 +880,40 @@
         behavior: dict | None = None,
     ) -> None:
         self.where = where
         self.highlevel = highlevel
         self.behavior = behavior
 
     def __call__(self, base: ak.Array, what: ak.Array) -> ak.Array:
-        # TODO: remove backend handling when touch is handled automatically
-        if ak.backend(what) == "typetracer":
-            what.layout._touch_data(recursive=False)
         return ak.with_field(
             base,
             what,
             where=self.where,
             highlevel=self.highlevel,
             behavior=self.behavior,
         )
 
 
 @borrow_docstring(ak.with_field)
 def with_field(base, what, where=None, highlevel=True, behavior=None):
     if not highlevel:
         raise ValueError("Only highlevel=True is supported")
-    if not compatible_partitions(base, what):
+
+    if not isinstance(base, Array):
+        raise ValueError("Base argument in with_field must be a dask_awkward.Array")
+
+    if not isinstance(what, (Array, Number)):
+        raise ValueError(
+            "with_field cannot accept string, bytes, list, or dict values yet"
+        )
+
+    maybe_dask_args = [base, what]
+    dask_args = tuple(arg for arg in maybe_dask_args if is_dask_collection(arg))
+
+    if not compatible_partitions(*dask_args):
         raise IncompatiblePartitions("with_field", base, what)
     return map_partitions(
         _WithFieldFn(where=where, highlevel=highlevel, behavior=behavior),
         base,
         what,
         label="with-field",
         output_divisions=1,
```

### Comparing `dask_awkward-2023.4.1/src/dask_awkward/lib/testutils.py` & `dask_awkward-2023.4.2/src/dask_awkward/lib/testutils.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.4.1/src/dask_awkward/lib/io/io.py` & `dask_awkward-2023.4.2/src/dask_awkward/lib/io/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import awkward as ak
 import numpy as np
 from awkward.types.numpytype import primitive_to_dtype
 from dask.base import flatten, tokenize
 from dask.highlevelgraph import HighLevelGraph
 from dask.utils import funcname
 
-from dask_awkward.layers import AwkwardInputLayer
+from dask_awkward.layers import AwkwardBlockwiseLayer, AwkwardInputLayer
 from dask_awkward.lib.core import (
     empty_typetracer,
     map_partitions,
     new_array_object,
     typetracer_array,
 )
 
@@ -355,14 +355,15 @@
         ak.from_numpy,
         name,
         "i",
         *pairs,
         numblocks=numblocks,
         concatenate=True,
     )
+    layer = AwkwardBlockwiseLayer.from_blockwise(layer)
     hlg = HighLevelGraph.from_collections(name, layer, dependencies=[array])
     if np.any(np.isnan(array.chunks)):
         return new_array_object(
             hlg, name, npartitions=array.npartitions, meta=meta, behavior=behavior
         )
     else:
         divs = (0, *np.cumsum(array.chunks))
```

### Comparing `dask_awkward-2023.4.1/src/dask_awkward/lib/io/json.py` & `dask_awkward-2023.4.2/src/dask_awkward/lib/io/json.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.4.1/src/dask_awkward/lib/io/parquet.py` & `dask_awkward-2023.4.2/src/dask_awkward/lib/io/parquet.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.4.1/.gitignore` & `dask_awkward-2023.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.4.1/LICENSE` & `dask_awkward-2023.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.4.1/README.md` & `dask_awkward-2023.4.2/README.md`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.4.1/pyproject.toml` & `dask_awkward-2023.4.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Topic :: Scientific/Engineering",
 ]
 dependencies = [
   "awkward >=2.1.3",
-  "dask >=2022.02.1",
+  "dask >=2023.04.0",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://github.com/dask-contrib/dask-awkward"
 "Bug Tracker" = "https://github.com/dask-contrib/dask-awkward/issues"
```

### Comparing `dask_awkward-2023.4.1/PKG-INFO` & `dask_awkward-2023.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-awkward
-Version: 2023.4.1
+Version: 2023.4.2
 Summary: Awkward Array meets Dask
 Project-URL: Homepage, https://github.com/dask-contrib/dask-awkward
 Project-URL: Bug Tracker, https://github.com/dask-contrib/dask-awkward/issues
 Author-email: Doug Davis <ddavis@ddavis.io>, Martin Durant <mdurant@anaconda.com>
 Maintainer-email: Doug Davis <ddavis@ddavis.io>, Martin Durant <mdurant@anaconda.com>
 License: BSD-3-Clause
 License-File: LICENSE
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
 Requires-Dist: awkward>=2.1.3
-Requires-Dist: dask>=2022.02.1
+Requires-Dist: dask>=2023.04.0
 Provides-Extra: complete
 Requires-Dist: aiohttp; extra == 'complete'
 Requires-Dist: pyarrow; extra == 'complete'
 Requires-Dist: pytest-cov>=3.0.0; extra == 'complete'
 Requires-Dist: pytest>=6.0; extra == 'complete'
 Requires-Dist: requests>=2.27.1; extra == 'complete'
 Provides-Extra: docs
```

