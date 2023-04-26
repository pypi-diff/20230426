# Comparing `tmp/baumdiff-0.1.1.tar.gz` & `tmp/baumdiff-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\baumdiff-0.1.1.tar", last modified: Thu Jun 24 05:19:47 2021, max compression
+gzip compressed data, was "dist\baumdiff-0.2.0.tar", last modified: Wed Apr 26 18:47:04 2023, max compression
```

## Comparing `baumdiff-0.1.1.tar` & `baumdiff-0.2.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2021-06-24 05:19:47.540277 baumdiff-0.1.1/
--rw-rw-rw-   0        0        0       67 2020-09-19 21:30:55.000000 baumdiff-0.1.1/.gitignore
--rw-rw-rw-   0        0        0      198 2020-09-20 02:17:54.000000 baumdiff-0.1.1/.travis.yml
--rw-rw-rw-   0        0        0     1105 2020-09-19 21:30:55.000000 baumdiff-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     1158 2021-06-24 05:19:47.528308 baumdiff-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      222 2020-09-20 09:08:25.000000 baumdiff-0.1.1/README.rst
--rw-rw-rw-   0        0        0       58 2020-09-20 11:27:02.000000 baumdiff-0.1.1/dev-requirements.txt
--rw-rw-rw-   0        0        0      142 2020-09-20 11:23:14.000000 baumdiff-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       87 2020-09-19 21:30:55.000000 baumdiff-0.1.1/pytest.ini
--rw-rw-rw-   0        0        0       42 2021-06-24 05:19:47.541274 baumdiff-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1132 2020-09-20 19:40:45.000000 baumdiff-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2021-06-24 05:19:47.287952 baumdiff-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2021-06-24 05:19:47.391674 baumdiff-0.1.1/src/baumdiff/
--rw-rw-rw-   0        0        0       64 2020-09-19 21:30:55.000000 baumdiff-0.1.1/src/baumdiff/__init__.py
--rw-rw-rw-   0        0        0     1098 2020-09-20 08:32:01.000000 baumdiff-0.1.1/src/baumdiff/matcher.py
--rw-rw-rw-   0        0        0     3695 2020-09-19 21:30:55.000000 baumdiff-0.1.1/src/baumdiff/script.py
--rw-rw-rw-   0        0        0     2054 2021-06-23 18:22:22.000000 baumdiff-0.1.1/src/baumdiff/shadow.py
--rw-rw-rw-   0        0        0     1753 2020-09-20 11:21:04.000000 baumdiff-0.1.1/src/baumdiff/simpletree.py
--rw-rw-rw-   0        0        0     2415 2020-09-19 21:30:55.000000 baumdiff-0.1.1/src/baumdiff/treeaccess.py
--rw-rw-rw-   0        0        0     9667 2020-09-20 08:34:24.000000 baumdiff-0.1.1/src/baumdiff/treediff.py
--rw-rw-rw-   0        0        0     9149 2020-09-20 09:05:42.000000 baumdiff-0.1.1/src/baumdiff/treemerge.py
-drwxrwxrwx   0        0        0        0 2021-06-24 05:19:47.440544 baumdiff-0.1.1/src/baumdiff.egg-info/
--rw-rw-rw-   0        0        0     1158 2021-06-24 05:19:46.000000 baumdiff-0.1.1/src/baumdiff.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      763 2021-06-24 05:19:47.000000 baumdiff-0.1.1/src/baumdiff.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-06-24 05:19:46.000000 baumdiff-0.1.1/src/baumdiff.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2021-06-24 05:19:46.000000 baumdiff-0.1.1/src/baumdiff.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2021-06-24 05:19:46.000000 baumdiff-0.1.1/src/baumdiff.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2021-06-24 05:19:47.458496 baumdiff-0.1.1/tests/
--rw-rw-rw-   0        0        0        0 2020-09-19 21:30:55.000000 baumdiff-0.1.1/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2021-06-24 05:19:47.508361 baumdiff-0.1.1/tests/test_diff/
--rw-rw-rw-   0        0        0        0 2020-09-19 21:30:55.000000 baumdiff-0.1.1/tests/test_diff/__init__.py
--rw-rw-rw-   0        0        0     5540 2020-09-20 19:36:24.000000 baumdiff-0.1.1/tests/test_diff/test_diff.py
--rw-rw-rw-   0        0        0     1676 2020-09-19 21:30:55.000000 baumdiff-0.1.1/tests/test_diff/test_randomtree_diff.py
--rw-rw-rw-   0        0        0      611 2020-09-19 21:30:55.000000 baumdiff-0.1.1/tests/test_diff/test_script.py
--rw-rw-rw-   0        0        0     2691 2020-09-19 21:30:55.000000 baumdiff-0.1.1/tests/test_diff/test_shadow.py
--rw-rw-rw-   0        0        0      571 2020-09-20 08:28:16.000000 baumdiff-0.1.1/tests/test_diff/test_treeaccess.py
-drwxrwxrwx   0        0        0        0 2021-06-24 05:19:47.525316 baumdiff-0.1.1/tests/test_merge/
--rw-rw-rw-   0        0        0        0 2020-09-19 21:30:55.000000 baumdiff-0.1.1/tests/test_merge/__init__.py
--rw-rw-rw-   0        0        0     2523 2020-09-19 21:30:55.000000 baumdiff-0.1.1/tests/test_merge/test_merge.py
--rw-rw-rw-   0        0        0     1899 2020-09-20 19:36:17.000000 baumdiff-0.1.1/tests/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-26 18:47:04.190976 baumdiff-0.2.0/
+-rw-rw-rw-   0        0        0       67 2020-09-19 21:30:55.000000 baumdiff-0.2.0/.gitignore
+-rw-rw-rw-   0        0        0      198 2020-09-20 02:17:54.000000 baumdiff-0.2.0/.travis.yml
+-rw-rw-rw-   0        0        0     1105 2020-09-19 21:30:55.000000 baumdiff-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     1158 2023-04-26 18:47:04.189971 baumdiff-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2020-09-20 09:08:25.000000 baumdiff-0.2.0/README.rst
+-rw-rw-rw-   0        0        0       58 2020-09-20 11:27:02.000000 baumdiff-0.2.0/dev-requirements.txt
+-rw-rw-rw-   0        0        0      142 2020-09-20 11:23:14.000000 baumdiff-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       87 2020-09-19 21:30:55.000000 baumdiff-0.2.0/pytest.ini
+-rw-rw-rw-   0        0        0       42 2023-04-26 18:47:04.190976 baumdiff-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1132 2020-09-20 19:40:45.000000 baumdiff-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 18:47:04.020430 baumdiff-0.2.0/src/
+drwxrwxrwx   0        0        0        0 2023-04-26 18:47:04.100219 baumdiff-0.2.0/src/baumdiff/
+-rw-rw-rw-   0        0        0       64 2020-09-19 21:30:55.000000 baumdiff-0.2.0/src/baumdiff/__init__.py
+-rw-rw-rw-   0        0        0     1098 2020-09-20 08:32:01.000000 baumdiff-0.2.0/src/baumdiff/matcher.py
+-rw-rw-rw-   0        0        0     4098 2023-04-26 18:42:07.000000 baumdiff-0.2.0/src/baumdiff/script.py
+-rw-rw-rw-   0        0        0     2273 2023-04-26 18:37:54.000000 baumdiff-0.2.0/src/baumdiff/shadow.py
+-rw-rw-rw-   0        0        0     1753 2020-09-20 11:21:04.000000 baumdiff-0.2.0/src/baumdiff/simpletree.py
+-rw-rw-rw-   0        0        0     2415 2020-09-19 21:30:55.000000 baumdiff-0.2.0/src/baumdiff/treeaccess.py
+-rw-rw-rw-   0        0        0    11090 2023-04-26 18:39:28.000000 baumdiff-0.2.0/src/baumdiff/treediff.py
+-rw-rw-rw-   0        0        0     9149 2020-09-20 09:05:42.000000 baumdiff-0.2.0/src/baumdiff/treemerge.py
+drwxrwxrwx   0        0        0        0 2023-04-26 18:47:04.155063 baumdiff-0.2.0/src/baumdiff.egg-info/
+-rw-rw-rw-   0        0        0     1158 2023-04-26 18:47:03.000000 baumdiff-0.2.0/src/baumdiff.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      763 2023-04-26 18:47:03.000000 baumdiff-0.2.0/src/baumdiff.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 18:47:03.000000 baumdiff-0.2.0/src/baumdiff.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-04-26 18:47:03.000000 baumdiff-0.2.0/src/baumdiff.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-26 18:47:03.000000 baumdiff-0.2.0/src/baumdiff.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-26 18:47:04.163043 baumdiff-0.2.0/tests/
+-rw-rw-rw-   0        0        0        0 2020-09-19 21:30:55.000000 baumdiff-0.2.0/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 18:47:04.181992 baumdiff-0.2.0/tests/test_diff/
+-rw-rw-rw-   0        0        0        0 2020-09-19 21:30:55.000000 baumdiff-0.2.0/tests/test_diff/__init__.py
+-rw-rw-rw-   0        0        0     5540 2020-09-20 19:36:24.000000 baumdiff-0.2.0/tests/test_diff/test_diff.py
+-rw-rw-rw-   0        0        0     1676 2020-09-19 21:30:55.000000 baumdiff-0.2.0/tests/test_diff/test_randomtree_diff.py
+-rw-rw-rw-   0        0        0      611 2020-09-19 21:30:55.000000 baumdiff-0.2.0/tests/test_diff/test_script.py
+-rw-rw-rw-   0        0        0     2691 2020-09-19 21:30:55.000000 baumdiff-0.2.0/tests/test_diff/test_shadow.py
+-rw-rw-rw-   0        0        0      571 2020-09-20 08:28:16.000000 baumdiff-0.2.0/tests/test_diff/test_treeaccess.py
+drwxrwxrwx   0        0        0        0 2023-04-26 18:47:04.186978 baumdiff-0.2.0/tests/test_merge/
+-rw-rw-rw-   0        0        0        0 2020-09-19 21:30:55.000000 baumdiff-0.2.0/tests/test_merge/__init__.py
+-rw-rw-rw-   0        0        0     2523 2020-09-19 21:30:55.000000 baumdiff-0.2.0/tests/test_merge/test_merge.py
+-rw-rw-rw-   0        0        0     1899 2020-09-20 19:36:17.000000 baumdiff-0.2.0/tests/utils.py
```

### Comparing `baumdiff-0.1.1/LICENSE` & `baumdiff-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `baumdiff-0.1.1/PKG-INFO` & `baumdiff-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baumdiff
-Version: 0.1.1
+Version: 0.2.0
 Summary: Tree Diff and Merge Library
 Home-page: https://github.com/podolsir/baumdiff
 Author: Igor Podolskiy
 Author-email: igor.podolskiy@gmx.de
 License: UNKNOWN
 Description: ========
         baumdiff
```

### Comparing `baumdiff-0.1.1/setup.py` & `baumdiff-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `baumdiff-0.1.1/src/baumdiff/matcher.py` & `baumdiff-0.2.0/src/baumdiff/matcher.py`

 * *Files identical despite different names*

### Comparing `baumdiff-0.1.1/src/baumdiff/script.py` & `baumdiff-0.2.0/src/baumdiff/script.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,18 +6,19 @@
         (self.node, self.parentPath, self.index) = (node, parentPath, index)
     def __repr__(self):
         return "Insert %s to %s at index %s" % (
             self.node, self.parentPath, self.index)
 
 class DeleteOp(object):
     type = 'DEL'
-    def __init__(self, path):
+    def __init__(self, path, deleted_id):
         self.path = path
+        self.deleted_id = deleted_id
     def __repr__(self):
-        return "Delete %s" % (self.path)
+        return "Delete %s (%s)" % (self.path, self.deleted_id)
 
 class UpdateOp(object):
     type = 'UPD'
     def __init__(self, path, value):
         (self.path, self.value) = path, value
     def __repr__(self):
         return "Update value of %s to %s" % (
@@ -58,23 +59,24 @@
         raise NotImplementedError
 
     def handleDelete(self, op, tree): # pragma: no cover
         raise NotImplementedError
     
 class DefaultExecutor(_ExecutorBase):
     def __init__(self, tree_adapter=None, parent_getter=None, child_seq_func=None, value_setter=None,
-        child_add_func=None, child_remove_func=None):
+        child_add_func=None, child_remove_func=None, id_getter=None):
         
         _ExecutorBase.__init__(self)
         tree_adapter = tree_adapter or DefaultTreeAdapter()
         self.value_setter = value_setter or tree_adapter.set_value
         self.parent_getter = parent_getter or tree_adapter.get_parent
         self.child_add_func = child_add_func or tree_adapter.add_child
         self.child_remove_func = child_remove_func or tree_adapter.remove_child
         self.child_seq_func = child_seq_func or tree_adapter.child_sequence
+        self.id_getter = id_getter or tree_adapter.get_id
  
     def handleMove(self, op, tree):
         node = descend(tree, op.path, child_seq_func =  self.child_seq_func)
         oldParent = self.parent_getter(node)
         newParent = descend(tree, op.newParentPath, child_seq_func = self.child_seq_func)
         self.child_remove_func(self.parent_getter(node), op.path[-1])
         newPos = op.index
@@ -88,8 +90,11 @@
 
     def handleUpdate(self, op, tree):
         node = descend(tree, op.path, child_seq_func = self.child_seq_func)
         self.value_setter(node, op.value)
 
     def handleDelete(self, op, tree):
         parent = descend(tree, op.path[0:-1], child_seq_func = self.child_seq_func)
+        assert(len(self.child_seq_func(parent)[op.path[-1]]) == 0)
+        assert(op.deleted_id == self.id_getter(self.child_seq_func(parent)[op.path[-1]])), \
+            f"{op.deleted_id} != {self.id_getter(self.child_seq_func(parent)[op.path[-1]])}"
         self.child_remove_func(parent, op.path[-1])
```

### Comparing `baumdiff-0.1.1/src/baumdiff/shadow.py` & `baumdiff-0.2.0/src/baumdiff/shadow.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,17 @@
         self.allchildren = []
         self._fixups = []
         super().__init__(*args)
         self.status = []
         self.initialized = True
 
     def _add_del_index(self, index):
+        for i in range(len(self._fixups)):
+            if index < self._fixups[i]:
+                self._fixups[i] -= 1
         bisect.insort(self._fixups, index)
 
     def _get_fixed_up_index(self, index):
         return index + sum(1 for _ in itertools.takewhile(lambda x: x <= index, self._fixups))
 
     def add(self, t, index = -1, status = 'inserted'):
         if self.initialized and not isinstance(t, ShadowNode):
@@ -28,16 +31,17 @@
         if self.initialized:
             t.status.append(status)
             for i in range(len(self._fixups)):
                 if index < self._fixups[i]:
                     self._fixups[i] += 1
 
     def remove(self, index, status = 'deleted'):
+        assert(self.children[index].id == self.allchildren[self._get_fixed_up_index(index)].id)
         super().remove(index)
-        self.allchildren[self._get_fixed_up_index(index)].status.append(status)
+        self.allchildren[self._get_fixed_up_index(index)].status = ['deleted']
         self._add_del_index(index)
 
     def _get_value(self):
         return super()._get_value()
     def _set_value(self, value):
         super()._set_value(value)
         self.status.append('updated')
```

### Comparing `baumdiff-0.1.1/src/baumdiff/simpletree.py` & `baumdiff-0.2.0/src/baumdiff/simpletree.py`

 * *Files identical despite different names*

### Comparing `baumdiff-0.1.1/src/baumdiff/treeaccess.py` & `baumdiff-0.2.0/src/baumdiff/treeaccess.py`

 * *Files identical despite different names*

### Comparing `baumdiff-0.1.1/src/baumdiff/treediff.py` & `baumdiff-0.2.0/src/baumdiff/treediff.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 import difflib
 from .treeaccess import DefaultTreeAdapter
 from .script import InsertOp, MoveOp, DeleteOp, UpdateOp
+from collections import namedtuple
+
+MoveResult = namedtuple('MoveResult', ('ops', 'fixedPos'))
 
 class NullProgressMonitor(object):
     def __init__(self):
         pass
     def progress(self, progress):
         pass
 
@@ -13,28 +16,30 @@
         tree_adapter=None,
         value_getter=None, value_setter=None, value_eq=None,
         parent_getter=None, path_getter=None,
         index_getter=None,
         child_add_func=None,
         child_remove_func=None,
         child_seq_func=None,
-        clone_func=None):
+        clone_func=None,
+        id_getter=None):
 
         tree_adapter = tree_adapter or DefaultTreeAdapter()
         self.progress_monitor = progress_monitor or NullProgressMonitor()
         self.value_getter = value_getter or tree_adapter.get_value
         self.value_setter = value_setter or tree_adapter.set_value
         self.value_eq = value_getter or tree_adapter.value_eq
         self.parent_getter = parent_getter or tree_adapter.get_parent
         self.path_getter = path_getter or tree_adapter.get_path
         self.index_getter = index_getter or tree_adapter.get_index
         self.child_add_func = child_add_func or tree_adapter.add_child
         self.child_remove_func = child_remove_func or tree_adapter.remove_child
         self.child_seq_func = child_seq_func or tree_adapter.child_sequence
         self.clone_func = clone_func or tree_adapter.clone_node
+        self.id_getter = id_getter or tree_adapter.get_id
 
         self.matcher = matcher
 
         self._marks1, self._marks2 = set(), set()
 
     def _postOrder(self, root, f, *args):
         for i in reversed(self.child_seq_func(root)):
@@ -104,23 +109,26 @@
         if (len_lcs == len(seq1) and len(seq1) == len(seq2)):
             return
 
         toMove = (x for x in seq1 if not self._has_mark1(x))
         for a in toMove:
             b = matching[a]
             newPos = self._findPos(b, node1)
-            script.extend(self._getMove(a, self.path_getter(node1), newPos, usemoves))
-            move(node1, a, newPos)
+            mr = self._getMove(a, self.path_getter(node1), newPos, usemoves)
+            script.extend(mr.ops)
+            move(node1, a, mr.fixedPos)
             self._mark(a, b)
         return
 
     def _delete(self, root, revMatching, script):
         if revMatching[root] is None:
-            script.append(DeleteOp(self.path_getter(root)))
+            op = DeleteOp(self.path_getter(root), self.id_getter(root))
+            script.append(op)
             parent = self.parent_getter(root)
+            assert(len(root.children) == 0)
             self.child_remove_func(parent, self.index_getter(parent, root))
         return [revMatching, script]
 
     def _pathFixup(self, deletePath, insertPath):
         # The deleted node is 'deeper' in the tree than the inserted node
         # so that it cannot possibly affect the insert path
         if len(deletePath) > len(insertPath):
@@ -138,22 +146,49 @@
             # -> shift insert path component by -1 and append rest of the insert path
             newInsertPath.append(insertPath[pathIndex] - 1)
             newInsertPath.extend(insertPath[pathIndex + 1:])
             return newInsertPath
         # otherwise, just return the original path
         return insertPath
 
-    def _getMove(self, node, targetParentPath, pos, usemoves):
+    def _subtractPathPrefix(self, path, prefix):
+        while len(prefix) > 0:
+            if path[0] == prefix[0]:
+                path = path[1:]
+                prefix = prefix[1:]
+            else:
+                break
+        return path
+
+    def _getMove(self, node, targetParentPath, pos, usemoves) -> MoveResult:
         if usemoves:
-            return (MoveOp(self.path_getter(node), targetParentPath, pos),)
+            raise NotImplementedError
+            # return MoveResult([MoveOp(self.path_getter(node), targetParentPath, pos)], pos)
         else:
-            insertNode = self.clone_func(node, True)
-            deletedNodePath = self.path_getter(node) 
-            return (DeleteOp(deletedNodePath),
-                    InsertOp(self._pathFixup(deletedNodePath, targetParentPath), insertNode, pos))
+            insertNode = self.clone_func(node, False)
+            deletedNodePath = self.path_getter(node)
+            newRootPath = self._pathFixup(deletedNodePath, targetParentPath)
+
+            inserts = []
+            deletes = []
+            
+            if deletedNodePath[:-1] == newRootPath and deletedNodePath[-1] < pos:
+                pos -= 1
+
+            def _d(node):
+                pathSuffix = self._subtractPathPrefix(self.path_getter(node), deletedNodePath)
+                assert(len(pathSuffix) > 0)
+                delete_op = DeleteOp(self.path_getter(node), self.id_getter(node))
+                deletes.append(delete_op)
+                inserts.insert(0, InsertOp(newRootPath + [pos] + pathSuffix[:-1], self.clone_func(node, False), pathSuffix[-1]))
+
+            self._postOrder(node, _d)
+            delete_op = DeleteOp(deletedNodePath, self.id_getter(node))
+
+            return MoveResult(deletes + [delete_op, InsertOp(newRootPath, insertNode, pos)] + inserts, pos)
         
     def _core(self, root2, newMatching, revMatching, script, usemoves):
         partnerParent = newMatching[root2]
 
         # Align Phase (at the beginning as the algorithm
         # is shifted by a level compare to the original paper)
         # The result are the 'in-order' markings which are stored in a set; 
@@ -186,18 +221,19 @@
                 # Move Phase
                 if partnerParent != self.parent_getter(node1):
                     # find a new position and update the markers
                     newPos = self._findPos(node2, partnerParent)
                     self._mark(node1, node2)
                     
                     # do the move
-                    script.extend(self._getMove(node1, self.path_getter(partnerParent), newPos, usemoves))
+                    mr = self._getMove(node1, self.path_getter(partnerParent), newPos, usemoves)
+                    script.extend(mr.ops)
                     parent1 = self.parent_getter(node1)
                     self.child_remove_func(parent1, self.index_getter(parent1, node1))
-                    self.child_add_func(partnerParent, node1, newPos)
+                    self.child_add_func(partnerParent, node1, mr.fixedPos)
 
                 # Update Phase
                 v1, v2 = self.value_getter(node1), self.value_getter(node2)
                 if not self.value_eq(v1, v2):
                     script.append(UpdateOp(self.path_getter(node1), v2))
                     self.value_setter(node1, v2)
```

### Comparing `baumdiff-0.1.1/src/baumdiff/treemerge.py` & `baumdiff-0.2.0/src/baumdiff/treemerge.py`

 * *Files identical despite different names*

### Comparing `baumdiff-0.1.1/src/baumdiff.egg-info/PKG-INFO` & `baumdiff-0.2.0/src/baumdiff.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baumdiff
-Version: 0.1.1
+Version: 0.2.0
 Summary: Tree Diff and Merge Library
 Home-page: https://github.com/podolsir/baumdiff
 Author: Igor Podolskiy
 Author-email: igor.podolskiy@gmx.de
 License: UNKNOWN
 Description: ========
         baumdiff
```

### Comparing `baumdiff-0.1.1/src/baumdiff.egg-info/SOURCES.txt` & `baumdiff-0.2.0/src/baumdiff.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `baumdiff-0.1.1/tests/test_diff/test_diff.py` & `baumdiff-0.2.0/tests/test_diff/test_diff.py`

 * *Files identical despite different names*

### Comparing `baumdiff-0.1.1/tests/test_diff/test_randomtree_diff.py` & `baumdiff-0.2.0/tests/test_diff/test_randomtree_diff.py`

 * *Files identical despite different names*

### Comparing `baumdiff-0.1.1/tests/test_diff/test_script.py` & `baumdiff-0.2.0/tests/test_diff/test_script.py`

 * *Files identical despite different names*

### Comparing `baumdiff-0.1.1/tests/test_diff/test_shadow.py` & `baumdiff-0.2.0/tests/test_diff/test_shadow.py`

 * *Files identical despite different names*

### Comparing `baumdiff-0.1.1/tests/test_diff/test_treeaccess.py` & `baumdiff-0.2.0/tests/test_diff/test_treeaccess.py`

 * *Files identical despite different names*

### Comparing `baumdiff-0.1.1/tests/test_merge/test_merge.py` & `baumdiff-0.2.0/tests/test_merge/test_merge.py`

 * *Files identical despite different names*

### Comparing `baumdiff-0.1.1/tests/utils.py` & `baumdiff-0.2.0/tests/utils.py`

 * *Files identical despite different names*

