# Comparing `tmp/refx-0.0.2.tar.gz` & `tmp/refx-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "refx-0.0.2.tar", max compression
+gzip compressed data, was "refx-0.0.3.tar", max compression
```

## Comparing `refx-0.0.2.tar` & `refx-0.0.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1072 2023-03-18 22:40:50.988547 refx-0.0.2/LICENSE
--rw-r--r--   0        0        0     4989 2023-04-10 23:48:37.427358 refx-0.0.2/README.md
--rw-r--r--   0        0        0      679 2023-04-10 23:57:56.814952 refx-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      402 2023-04-10 23:18:10.151914 refx-0.0.2/refx/__init__.py
--rw-r--r--   0        0        0     4917 2023-04-04 14:45:47.636573 refx-0.0.2/refx/partitioning.py
--rw-r--r--   0        0        0    11270 2023-04-10 23:19:39.719530 refx-0.0.2/refx/ref.py
--rw-r--r--   0        0        0     1941 2023-04-08 23:10:50.361152 refx-0.0.2/refx/ref_field.py
--rw-r--r--   0        0        0     1839 2023-04-10 13:35:10.915812 refx-0.0.2/refx/tracers.py
--rw-r--r--   0        0        0     5457 1970-01-01 00:00:00.000000 refx-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-03-18 22:40:50.988547 refx-0.0.3/LICENSE
+-rw-r--r--   0        0        0     4989 2023-04-10 23:48:37.427358 refx-0.0.3/README.md
+-rw-r--r--   0        0        0      679 2023-04-25 22:27:47.641760 refx-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      425 2023-04-22 15:20:50.001621 refx-0.0.3/refx/__init__.py
+-rw-r--r--   0        0        0     4917 2023-04-04 14:45:47.636573 refx-0.0.3/refx/partitioning.py
+-rw-r--r--   0        0        0    12689 2023-04-22 15:20:50.001621 refx-0.0.3/refx/ref.py
+-rw-r--r--   0        0        0     1925 2023-04-22 20:53:41.336761 refx-0.0.3/refx/ref_field.py
+-rw-r--r--   0        0        0     1839 2023-04-10 13:35:10.915812 refx-0.0.3/refx/tracers.py
+-rw-r--r--   0        0        0     5457 1970-01-01 00:00:00.000000 refx-0.0.3/PKG-INFO
```

### Comparing `refx-0.0.2/LICENSE` & `refx-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `refx-0.0.2/README.md` & `refx-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `refx-0.0.2/pyproject.toml` & `refx-0.0.3/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "refx"
-version = "0.0.2"
+version = "0.0.3"
 description = ""
 authors = ["Cristian Garcia <cgarcia.e88@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 jax = ">=0.4.6"
```

### Comparing `refx-0.0.2/refx/partitioning.py` & `refx-0.0.3/refx/partitioning.py`

 * *Files identical despite different names*

### Comparing `refx-0.0.2/refx/ref.py` & `refx-0.0.3/refx/ref.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from abc import ABC, abstractmethod
 import contextlib
 import dataclasses
 from functools import partial
 import typing as tp
 
 import jax
 import jax.tree_util as jtu
@@ -64,51 +65,43 @@
 
 
 NOTHING = Nothing()
 
 jtu.register_pytree_node(Nothing, _nothing_flatten, _nothing_unflatten)
 
 
-class Referential:
-    __slots__ = ()
+class Referential(tp.Generic[A], ABC):
+    __slots__ = ("_collection",)
+
+    def __init__(self, collection: tp.Hashable):
+        self._collection = collection
 
     @property
-    def index(self) -> int:
+    @abstractmethod
+    def value(self) -> A:
         ...
 
     @property
     def collection(self) -> tp.Hashable:
-        ...
+        return self._collection
 
 
-class Deref(Referential):
+class Deref(Referential[A]):
     __slots__ = ()
 
-    @property
-    def index(self) -> int:
-        ...
-
-    @property
-    def collection(self) -> tp.Hashable:
-        ...
-
 
-class Ref(Referential, tp.Generic[A]):
-    __slots__ = ("_value", "_collection", "_jax_trace", "_refx_trace", "_trace_set")
+class Ref(Referential[A]):
+    __slots__ = ("_value", "_jax_trace", "_refx_trace", "_trace_set")
 
     def __init__(self, value: A, collection: tp.Hashable = None):
         self._value = value
-        self._collection = collection
         self._jax_trace = tracers.current_jax_trace()
         self._refx_trace = tracers.current_refx_trace()
         self._trace_set = frozenset((self._jax_trace, self._refx_trace))
-
-    @property
-    def collection(self) -> tp.Hashable:
-        return self._collection
+        super().__init__(collection)
 
     @property
     def value(self) -> A:
         if (
             self._jax_trace is not tracers.current_jax_trace()
             or self._refx_trace is not tracers.current_refx_trace()
         ):
@@ -131,94 +124,84 @@
             raise ValueError(
                 "Cannot mutate ref with value that contains tracers from other "
                 f"traces: {invalid_traces}"
             )
 
         self._value = value
 
-    @property
-    def index(self) -> int:
-        return -id(self)
-
-    def to_value(self, index: int) -> "Value[A]":
-        return Value(self.value, index, self.collection)
+    def to_value(self) -> "Value[A]":
+        return Value(self.value, self.collection)
 
-    def to_index(self, index: int) -> "Index":
-        return Index(index, self.collection)
+    def to_index(self) -> "Index[A]":
+        return Index(self.collection)
 
 
-class Value(Deref, tp.Generic[A]):
-    __slots__ = ("_value", "_index", "_collection")
+class Value(Deref[A]):
+    __slots__ = ("_value",)
 
-    def __init__(self, value: A, index: int, collection: tp.Hashable):
+    def __init__(self, value: A, collection: tp.Hashable):
         self._value = value
-        self._index = index
-        self._collection = collection
+        super().__init__(collection)
 
     @property
     def value(self) -> A:
         return self._value
 
-    @property
-    def index(self) -> int:
-        return self._index
-
-    @property
-    def collection(self) -> tp.Hashable:
-        return self._collection
-
     def to_ref(self) -> "Ref[A]":
-        return Ref(self.value, self.collection)
+        return Ref(self._value, self.collection)
 
     def __repr__(self) -> str:
-        return f"Value(index={self.index}, collection={repr(self.collection)})"
+        return f"Value(collection={repr(self.collection)}, value={repr(self._value)})"
 
 
-def _value_flatten_with_keys(
+def _value_flatten(
     x: Value[A],
-) -> tp.Tuple[tp.Tuple[tp.Tuple[jtu.GetAttrKey, A]], tp.Tuple[int, tp.Hashable]]:
-    return ((jtu.GetAttrKey("value"), x.value),), (x.index, x.collection)
+    *,
+    with_keys: bool,
+) -> tp.Tuple[tp.Tuple[tp.Any], tp.Hashable]:
+    if with_keys:
+        node = (jtu.GetAttrKey("value"), x._value)
+    else:
+        node = x._value
 
+    return (node,), x.collection
 
-def _value_unflatten(
-    aux_data: tp.Tuple[int, tp.Hashable], children: tp.Tuple[A]
-) -> Value[A]:
-    return Value(children[0], *aux_data)
 
+def _value_unflatten(collection: tp.Hashable, children: tp.Tuple[A]) -> Value[A]:
+    return Value(children[0], collection)
 
-jtu.register_pytree_with_keys(Value, _value_flatten_with_keys, _value_unflatten)
 
+jtu.register_pytree_with_keys(
+    Value,
+    partial(_value_flatten, with_keys=True),
+    _value_unflatten,
+    flatten_func=partial(_value_flatten, with_keys=False),
+)
 
-class Index(Deref):
-    __slots__ = ("_index", "_collection")
 
-    def __init__(self, index: int, collection: tp.Hashable):
-        self._index = index
-        self._collection = collection
+class Index(Deref[A]):
+    __slots__ = ()
 
-    @property
-    def index(self) -> int:
-        return self._index
+    def __init__(self, collection: tp.Hashable):
+        self._collection = collection
 
     @property
-    def collection(self) -> tp.Hashable:
-        return self._collection
+    def value(self) -> A:
+        raise ValueError(f"Cannot get value from '{type(self).__name__}' instances")
 
     def __repr__(self) -> str:
-        return f"Index(index={self.index}, collection={self.collection})"
+        return f"Index(collection={self.collection})"
 
 
-def _index_flatten(x: Index) -> tp.Tuple[tp.Tuple[()], tp.Tuple[int, tp.Hashable]]:
-    return (), (x.index, x.collection)
+def _index_flatten(x: Index[A]) -> tp.Tuple[tp.Tuple[()], tp.Hashable]:
+    return (), x.collection
 
 
-def _index_unflatten(
-    aux_data: tp.Tuple[int, tp.Hashable], children: tp.Tuple[()]
-) -> Index:
-    return Index(*aux_data)
+def _index_unflatten(colletion: tp.Hashable, children: tp.Tuple[()]) -> Index[A]:
+    return Index(colletion)
 
 
 jtu.register_pytree_node(Index, _index_flatten, _index_unflatten)
 
 
 class Static(tp.Generic[A]):
     __slots__ = ("_value",)
@@ -238,112 +221,192 @@
 def _static_unflatten(aux_data: A, _: tp.Tuple[()]) -> Static[A]:
     return Static(aux_data)
 
 
 jtu.register_pytree_node(Static, _static_flatten, _static_unflatten)
 
 
+DagIndexes = tp.Tuple[tp.Tuple[int, ...], ...]
+DagIndexesList = tp.List[tp.List[int]]
+
+
+class DagDef:
+    __slots__ = ("_indexes", "_treedef")
+
+    def __init__(self, indexes: DagIndexes, treedef: jtu.PyTreeDef):
+        self._indexes = indexes
+        self._treedef = treedef
+
+    def unflatten(self, leaves: Leaves) -> tp.Any:
+        return self._treedef.unflatten(leaves)
+
+    def flatten_up_to(self, __pytree: tp.Any, /) -> Leaves:
+        return self.treedef.flatten_up_to(__pytree)
+
+    @property
+    def indexes(self) -> DagIndexes:
+        return self._indexes
+
+    @property
+    def treedef(self) -> jtu.PyTreeDef:
+        return self._treedef
+
+    def __hash__(self) -> int:
+        return hash((self._indexes, self._treedef))
+
+    def __eq__(self, other: tp.Any) -> bool:
+        if not isinstance(other, DagDef):
+            return ValueError(f"Cannot compare DagDef with {type(other)}")
+        return self._indexes == other._indexes and self._treedef == other._treedef
+
+
+def _dagdef_flatten(
+    x: DagDef,
+) -> tp.Tuple[tp.Tuple[()], tp.Tuple[DagIndexes, jtu.PyTreeDef]]:
+    return (), (x._indexes, x._treedef)
+
+
+def _dagdef_unflatten(
+    metadata: tp.Tuple[DagIndexes, jtu.PyTreeDef], _: tp.Tuple[()]
+) -> DagDef:
+    return DagDef(*metadata)
+
+
+jtu.register_pytree_node(DagDef, _dagdef_flatten, _dagdef_unflatten)
+
+
 class Dag(tp.Generic[A]):
     __slots__ = ("_value",)
 
     def __init__(self, value: A):
         self._value = value
 
     @property
     def value(self) -> A:
         return self._value
 
 
-def _dag_flatten_with_keys(
+def _dag_flatten(
     x: Dag[tp.Any],
-) -> tp.Tuple[tp.Tuple[tp.Tuple[jtu.GetAttrKey, Leaves]], jtu.PyTreeDef]:
-    leaves, treedef = deref_flatten(x.value)
-    key_node = (jtu.GetAttrKey("value"), leaves)
-    return (key_node,), treedef
-
-
-def _dag_unflatten(treedef: jtu.PyTreeDef, leaves: Leaves) -> Dag[tp.Any]:
-    return Dag(reref_unflatten(treedef, leaves))
+    *,
+    with_keys: bool,
+) -> tp.Tuple[tp.Tuple[tp.Any], DagDef]:
+    leaves, dagdef = deref_flatten(x.value)
+    if with_keys:
+        node = (jtu.GetAttrKey("value"), leaves)
+    else:
+        node = leaves
+    return (node,), dagdef
 
 
-jtu.register_pytree_with_keys(Dag, _dag_flatten_with_keys, _dag_unflatten)
+def _dag_unflatten(dagdef: DagDef, nodes: tp.Tuple[Leaves]) -> Dag[tp.Any]:
+    return Dag(reref_unflatten(nodes[0], dagdef))
 
 
-def deref_fn(ref_index: tp.Dict[Ref[tp.Any], int], x: tp.Any) -> tp.Any:
-    if isinstance(x, Ref):
-        if x not in ref_index:
-            index = len(ref_index)
-            ref_index[x] = index
-            return x.to_value(index)
+jtu.register_pytree_with_keys(
+    Dag,
+    partial(_dag_flatten, with_keys=True),
+    _dag_unflatten,
+    flatten_func=partial(_dag_flatten, with_keys=False),
+)
+
+
+def deref_leaves(
+    ref_index: tp.Dict[Ref[tp.Any], int],
+    indexes: DagIndexesList,
+    leaves: Leaves,
+) -> tp.Iterator[tp.Any]:
+    for leaf_idx, x in enumerate(leaves):
+        if isinstance(x, Ref):
+            if x not in ref_index:
+                ref_index[x] = len(ref_index)
+                indexes.append([leaf_idx])
+                yield x.to_value()
+            else:
+                indexes[ref_index[x]].append(leaf_idx)
+                yield x.to_index()
+        elif isinstance(x, Deref):
+            raise ValueError("Cannot 'deref' pytree containing Derefs")
         else:
-            return x.to_index(ref_index[x])
-    elif isinstance(x, Deref) and ref_index:
-        raise ValueError("Cannot 'deref' pytree containing Derefs")
-    else:
-        return x
+            yield x
 
 
-def deref_flatten(pytree: tp.Any) -> tp.Tuple[Leaves, jtu.PyTreeDef]:
+def deref_flatten(pytree: tp.Any) -> tp.Tuple[Leaves, DagDef]:
     ref_index: tp.Dict[Ref[tp.Any], int] = {}
+    indexes = []
     leaves, treedef = jtu.tree_flatten(pytree, is_leaf=lambda x: isinstance(x, Deref))
-    return list(map(partial(deref_fn, ref_index), leaves)), treedef
+    leaves = list(deref_leaves(ref_index, indexes, leaves))
+    indexes = tuple(map(tuple, indexes))
+    return leaves, DagDef(indexes, treedef)
 
 
-def deref_unflatten(treedef: jtu.PyTreeDef, leaves: Leaves) -> A:
+def deref_unflatten(treedef: jtu.PyTreeDef, leaves: Leaves) -> tp.Tuple[A, DagDef]:
     ref_index: tp.Dict[Ref[tp.Any], int] = {}
-    leaves = list(map(partial(deref_fn, ref_index), leaves))
-    return jtu.tree_unflatten(treedef, leaves)
+    indexes = []
+    leaves = list(deref_leaves(ref_index, indexes, leaves))
+    indexes = tuple(map(tuple, indexes))
+    return jtu.tree_unflatten(treedef, leaves), DagDef(indexes, treedef)
 
 
-def deref(pytree: A) -> A:
-    ref_index: tp.Dict[Ref[tp.Any], int] = {}
-    return jax.tree_map(
-        partial(deref_fn, ref_index), pytree, is_leaf=lambda x: isinstance(x, Deref)
-    )
+def deref(pytree: A) -> tp.Tuple[A, DagDef]:
+    leaves, dagdef = deref_flatten(pytree)
+    return dagdef.unflatten(leaves), dagdef
 
 
-def reref_fn(index_ref: tp.Dict[int, Ref[tp.Any]], x: tp.Any) -> tp.Any:
+def _validate_reref(x: A) -> A:
     if isinstance(x, Ref):
         raise ValueError("Cannot 'reref' pytree containing Refs")
-    elif isinstance(x, Value):
-        if x.index in index_ref:
-            raise ValueError("Value already exists")
-        ref = x.to_ref()
-        index_ref[x.index] = ref
-        return ref
-    elif isinstance(x, Index):
-        if x.index not in index_ref:
-            # NOTE: because pytree flatten and unflatten in a deterministic
-            # order, this should never trigger
-            raise RuntimeError(
-                "BUG: Got multiple values for the same index. This should never "
-                "happen, please report it."
+
+    return x
+
+
+def reref_leaves(indexes: DagIndexes, leaves: Leaves) -> Leaves:
+    leaves_out = list(map(_validate_reref, leaves))
+
+    for leaf_indexes in indexes:
+        leaf_index = leaf_indexes[0]
+        value = leaves[leaf_index]
+
+        if not isinstance(value, Value):
+            raise ValueError(
+                f"Expected 'Value' as first leaf, got {type(value).__name__}"
             )
-        return index_ref[x.index]
-    else:
-        return x
 
+        ref = value.to_ref()
+        leaves_out[leaf_index] = ref
 
-def reref_flatten(pytree: tp.Any) -> tp.Tuple[Leaves, jtu.PyTreeDef]:
-    index_ref: tp.Dict[int, Ref[tp.Any]] = {}
-    leaves, treedef = jtu.tree_flatten(pytree, is_leaf=lambda x: isinstance(x, Deref))
-    return list(map(partial(reref_fn, index_ref), leaves)), treedef
+        for leaf_index in leaf_indexes[1:]:
+            x = leaves[leaf_index]
 
+            if not isinstance(x, Index):
+                raise ValueError(f"Expected 'Index' as leaf, got {type(x).__name__}")
 
-def reref_unflatten(treedef: jtu.PyTreeDef, leaves: Leaves) -> tp.Any:
-    index_ref: tp.Dict[int, Ref[tp.Any]] = {}
-    leaves = list(map(partial(reref_fn, index_ref), leaves))
-    return jtu.tree_unflatten(treedef, leaves)
+            leaves_out[leaf_index] = ref
 
+    return leaves_out
 
-def reref(pytree: A) -> A:
-    index_ref: tp.Dict[int, Ref[tp.Any]] = {}
-    return jax.tree_map(
-        partial(reref_fn, index_ref), pytree, is_leaf=lambda x: isinstance(x, Deref)
-    )
+
+def reref_flatten(pytree: tp.Any, dagdef: DagDef) -> Leaves:
+    indexes = dagdef.indexes
+    leaves = dagdef.treedef.flatten_up_to(pytree)
+    return reref_leaves(indexes, leaves)
+
+
+def reref_unflatten(leaves: Leaves, dagdef: DagDef) -> tp.Any:
+    leaves = reref_leaves(dagdef.indexes, leaves)
+    return dagdef.unflatten(leaves)
+
+
+def reref(pytree: A, dagdef: DagDef) -> A:
+    leaves = reref_flatten(pytree, dagdef)
+    return dagdef.unflatten(leaves)
+
+
+def clone(pytree: A) -> A:
+    return reref_unflatten(*deref_flatten(pytree))
 
 
 def update_refs(target_tree: tp.Any, source_tree: tp.Any):
     target_leaves = jtu.tree_leaves(
         target_tree, is_leaf=lambda x: isinstance(x, Referential) or x is NOTHING
     )
     source_leaves = jtu.tree_leaves(
@@ -352,41 +415,43 @@
 
     if len(target_leaves) != len(source_leaves):
         raise ValueError(
             f"Target and source leaves must have the same length, got "
             f"{len(target_leaves)} and {len(source_leaves)}"
         )
 
-    ref_to_index: tp.Dict[Ref[tp.Any], int] = {}
+    seen_target_refs: tp.Set[Ref[tp.Any]] = set()
+    seen_source_refs: tp.Set[Ref[tp.Any]] = set()
     source_has_ref = False
     source_has_deref = False
 
     for i, (target_leaf, source_leaf) in enumerate(zip(target_leaves, source_leaves)):
         if isinstance(source_leaf, Deref):
             source_has_deref = True
         elif isinstance(source_leaf, Ref):
             source_has_ref = True
         if source_has_ref and source_has_deref:
             raise ValueError("Got source with mixed Ref and Deref instances")
 
         if isinstance(target_leaf, Ref):
-            if target_leaf in ref_to_index:
-                if isinstance(source_leaf, (Ref, Index)):
-                    if ref_to_index[target_leaf] != source_leaf.index:
-                        raise ValueError
-                else:
-                    raise ValueError
+            if target_leaf in seen_target_refs:
+                if isinstance(source_leaf, Ref) and source_leaf not in seen_source_refs:
+                    raise ValueError()
+                if not isinstance(source_leaf, (Index, Ref)):
+                    raise ValueError()
                 continue
             elif isinstance(source_leaf, (Value, Ref)):
-                target_leaf.value = source_leaf.value
-                ref_to_index[target_leaf] = source_leaf.index
+                target_leaf.value = source_leaf._value
+                seen_target_refs.add(target_leaf)
+                if isinstance(source_leaf, Ref):
+                    seen_source_refs.add(source_leaf)
             elif isinstance(source_leaf, Index):
                 raise ValueError(
                     f"Unseen Ref '{type(target_leaf).__name__}' at position [{i}] "
-                    f"aligned with source 'Index(index={source_leaf.index})'"
+                    f"aligned with source '{source_leaf}'"
                 )
             else:
                 raise ValueError(
                     f"Unexpected source type '{type(source_leaf).__name__}' "
                     f"at position [{i}]"
                 )
         elif isinstance(target_leaf, Deref):
```

### Comparing `refx-0.0.2/refx/ref_field.py` & `refx-0.0.3/refx/ref_field.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,29 +23,29 @@
         if metadata is None:
             metadata = {}
         super().__init__(default, default_factory, init, repr, hash, compare, metadata)
         self.collection = collection
         self._first_get_call = True
         self.class_field_name: tp.Optional[str] = None
 
-    def __set_name__(self, owner, name):
+    def __set_name__(self, cls, name):
         """__set_name__ initializer for properties as per [PEP-487](https://peps.python.org/pep-0487/)"""
         self.class_field_name = name
 
     @property
     def object_field_name(self):
         return f"{self.class_field_name}__ref"
 
     def __get__(self, obj, objtype=None):
         if obj is None:
             if self._first_get_call:
                 self._first_get_call = False
                 return self
             else:
-                raise AttributeError
+                return
 
         if not hasattr(obj, self.object_field_name):
             raise AttributeError(f"Attribute '{self.class_field_name}' is not set")
 
         return getattr(obj, self.object_field_name).value
 
     def __set__(self, obj, value: A):
```

### Comparing `refx-0.0.2/refx/tracers.py` & `refx-0.0.3/refx/tracers.py`

 * *Files identical despite different names*

### Comparing `refx-0.0.2/PKG-INFO` & `refx-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refx
-Version: 0.0.2
+Version: 0.0.3
 Summary: 
 Author: Cristian Garcia
 Author-email: cgarcia.e88@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

