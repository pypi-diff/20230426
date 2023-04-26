# Comparing `tmp/terrace-0.0.76.tar.gz` & `tmp/terrace-0.0.77.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terrace-0.0.76.tar", last modified: Tue Apr  4 19:15:40 2023, max compression
+gzip compressed data, was "terrace-0.0.77.tar", last modified: Wed Apr 26 13:49:28 2023, max compression
```

## Comparing `terrace-0.0.76.tar` & `terrace-0.0.77.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 boris     (1000) boris     (1001)        0 2023-04-04 19:15:40.547098 terrace-0.0.76/
--rw-r--r--   0 boris     (1000) boris     (1001)      678 2023-04-04 19:15:40.547098 terrace-0.0.76/PKG-INFO
--rw-r--r--   0 boris     (1000) boris     (1001)      341 2022-10-27 14:35:47.000000 terrace-0.0.76/README.md
--rw-r--r--   0 boris     (1000) boris     (1001)       38 2023-04-04 19:15:40.547098 terrace-0.0.76/setup.cfg
--rw-r--r--   0 boris     (1000) boris     (1001)      693 2023-04-04 19:15:14.000000 terrace-0.0.76/setup.py
-drwxr-xr-x   0 boris     (1000) boris     (1001)        0 2023-04-04 19:15:40.547098 terrace-0.0.76/src/
-drwxr-xr-x   0 boris     (1000) boris     (1001)        0 2023-04-04 19:15:40.547098 terrace-0.0.76/src/terrace/
--rw-r--r--   0 boris     (1000) boris     (1001)      249 2023-04-04 18:32:55.000000 terrace-0.0.76/src/terrace/__init__.py
--rw-r--r--   0 boris     (1000) boris     (1001)    12628 2023-04-04 18:52:50.000000 terrace-0.0.76/src/terrace/batch.py
--rw-r--r--   0 boris     (1000) boris     (1001)     4688 2023-02-13 23:18:46.000000 terrace-0.0.76/src/terrace/categorical_tensor.py
--rw-r--r--   0 boris     (1000) boris     (1001)     1000 2023-02-09 21:20:38.000000 terrace-0.0.76/src/terrace/dataframe.py
--rw-r--r--   0 boris     (1000) boris     (1001)     9139 2023-04-04 18:52:01.000000 terrace-0.0.76/src/terrace/graph.py
--rw-r--r--   0 boris     (1000) boris     (1001)     2592 2022-10-27 14:29:11.000000 terrace-0.0.76/src/terrace/meta_utils.py
--rw-r--r--   0 boris     (1000) boris     (1001)     4038 2023-03-27 00:02:39.000000 terrace-0.0.76/src/terrace/module.py
-drwxr-xr-x   0 boris     (1000) boris     (1001)        0 2023-04-04 19:15:40.547098 terrace-0.0.76/src/terrace.egg-info/
--rw-r--r--   0 boris     (1000) boris     (1001)      678 2023-04-04 19:15:40.000000 terrace-0.0.76/src/terrace.egg-info/PKG-INFO
--rw-r--r--   0 boris     (1000) boris     (1001)      365 2023-04-04 19:15:40.000000 terrace-0.0.76/src/terrace.egg-info/SOURCES.txt
--rw-r--r--   0 boris     (1000) boris     (1001)        1 2023-04-04 19:15:40.000000 terrace-0.0.76/src/terrace.egg-info/dependency_links.txt
--rw-r--r--   0 boris     (1000) boris     (1001)       11 2023-04-04 19:15:40.000000 terrace-0.0.76/src/terrace.egg-info/requires.txt
--rw-r--r--   0 boris     (1000) boris     (1001)        8 2023-04-04 19:15:40.000000 terrace-0.0.76/src/terrace.egg-info/top_level.txt
+drwxr-xr-x   0 boris     (1000) boris     (1001)        0 2023-04-26 13:49:28.678956 terrace-0.0.77/
+-rw-r--r--   0 boris     (1000) boris     (1001)      678 2023-04-26 13:49:28.678956 terrace-0.0.77/PKG-INFO
+-rw-r--r--   0 boris     (1000) boris     (1001)      341 2022-10-27 14:35:47.000000 terrace-0.0.77/README.md
+-rw-r--r--   0 boris     (1000) boris     (1001)       38 2023-04-26 13:49:28.678956 terrace-0.0.77/setup.cfg
+-rw-r--r--   0 boris     (1000) boris     (1001)      693 2023-04-26 13:48:59.000000 terrace-0.0.77/setup.py
+drwxr-xr-x   0 boris     (1000) boris     (1001)        0 2023-04-26 13:49:28.675623 terrace-0.0.77/src/
+drwxr-xr-x   0 boris     (1000) boris     (1001)        0 2023-04-26 13:49:28.678956 terrace-0.0.77/src/terrace/
+-rw-r--r--   0 boris     (1000) boris     (1001)      249 2023-04-04 18:32:55.000000 terrace-0.0.77/src/terrace/__init__.py
+-rw-r--r--   0 boris     (1000) boris     (1001)    12682 2023-04-26 13:45:05.000000 terrace-0.0.77/src/terrace/batch.py
+-rw-r--r--   0 boris     (1000) boris     (1001)     5191 2023-04-06 19:35:34.000000 terrace-0.0.77/src/terrace/categorical_tensor.py
+-rw-r--r--   0 boris     (1000) boris     (1001)     1000 2023-02-09 21:20:38.000000 terrace-0.0.77/src/terrace/dataframe.py
+-rw-r--r--   0 boris     (1000) boris     (1001)     9139 2023-04-04 18:52:01.000000 terrace-0.0.77/src/terrace/graph.py
+-rw-r--r--   0 boris     (1000) boris     (1001)     2592 2022-10-27 14:29:11.000000 terrace-0.0.77/src/terrace/meta_utils.py
+-rw-r--r--   0 boris     (1000) boris     (1001)     4038 2023-03-27 00:02:39.000000 terrace-0.0.77/src/terrace/module.py
+drwxr-xr-x   0 boris     (1000) boris     (1001)        0 2023-04-26 13:49:28.678956 terrace-0.0.77/src/terrace.egg-info/
+-rw-r--r--   0 boris     (1000) boris     (1001)      678 2023-04-26 13:49:28.000000 terrace-0.0.77/src/terrace.egg-info/PKG-INFO
+-rw-r--r--   0 boris     (1000) boris     (1001)      365 2023-04-26 13:49:28.000000 terrace-0.0.77/src/terrace.egg-info/SOURCES.txt
+-rw-r--r--   0 boris     (1000) boris     (1001)        1 2023-04-26 13:49:28.000000 terrace-0.0.77/src/terrace.egg-info/dependency_links.txt
+-rw-r--r--   0 boris     (1000) boris     (1001)       11 2023-04-26 13:49:28.000000 terrace-0.0.77/src/terrace.egg-info/requires.txt
+-rw-r--r--   0 boris     (1000) boris     (1001)        8 2023-04-26 13:49:28.000000 terrace-0.0.77/src/terrace.egg-info/top_level.txt
```

### Comparing `terrace-0.0.76/PKG-INFO` & `terrace-0.0.77/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terrace
-Version: 0.0.76
+Version: 0.0.77
 Summary: high level PyTorch utils
 Home-page: https://github.com/mixarcid/terrace
 Author: Michael Brocidiacono
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `terrace-0.0.76/setup.py` & `terrace-0.0.77/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setuptools.setup(
     name="terrace",
-    version="0.0.76",
+    version="0.0.77",
     author="Michael Brocidiacono",
     author_email="",
     description="high level PyTorch utils",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mixarcid/terrace",
     packages=setuptools.find_packages(
```

### Comparing `terrace-0.0.76/src/terrace/batch.py` & `terrace-0.0.77/src/terrace/batch.py`

 * *Files 0% similar despite different names*

```diff
@@ -247,26 +247,29 @@
     _batch_type: Type[Batchable]
     _internal_attribs = [ "_items", "_batch_type" ]
 
     def __init__(self, items):
         self._items = items
         self._batch_type = type(items[0])
 
+    def __len__(self):
+        return len(self._items)
+
     def __getitem__(self, index):
         return self._items[index]
 
     def __getattribute__(self, name):
         if name == "__dict__" or name in LazyBatch._internal_attribs or name in self.__dict__:
             return object.__getattribute__(self, name)
         batch_method_name = "batch_" + name
         if hasattr(self, "_batch_type") and hasattr(self._batch_type, batch_method_name):
             batch_method = getattr(self._batch_type, batch_method_name)
             if callable(batch_method):
                 return partial(batch_method, self)
-        if name in self[0].__dict__:
+        if hasattr(self[0], name):
             return collate([getattr(item, name) for item in self._items], lazy=True)
         return object.__getattribute__(self, name)
 
     def __repr__(self):
         return "LazyBatch"
 
 class NoStackTensor(torch.Tensor):
```

### Comparing `terrace-0.0.76/src/terrace/categorical_tensor.py` & `terrace-0.0.77/src/terrace/categorical_tensor.py`

 * *Files 10% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     @classmethod
     def __torch_function__(cls, func, types, args=(), kwargs=None):
         if kwargs is None:
             kwargs = {}
         if func in HANDLED_FUNCTIONS:
             return HANDLED_FUNCTIONS[func](*args, **kwargs)
         # return func(*args, **kwargs)
+        print(func)
         raise NotImplementedError(func)
 
 class NoStackCatTensor(CategoricalTensor):
     pass
 
 
 def implements(torch_function):
@@ -68,14 +69,34 @@
     ret = torch.split(ct.tensor, *args, **kwargs)
     return [ CategoricalTensor(t, ct.num_classes) for t in ret ]
 
 @implements(torch.Tensor.__len__)
 def cat_tensor_len(ct):
     return len(ct.tensor)
 
+@implements(torch.Tensor.is_sparse.__get__)
+def cat_is_sparse(ct):
+    return ct.tensor.is_sparse
+
+@implements(torch.Tensor.storage)
+def cat_storage(ct):
+    return ct.tensor.storage()
+
+@implements(torch.Tensor.element_size)
+def cat_element_size(ct):
+    return ct.tensor.element_size()
+
+@implements(torch.Tensor.size)
+def cat_size(ct, *args, **kwargs):
+    return ct.tensor.size(*args, **kwargs)
+    
+@implements(torch.Tensor.numel)
+def cat_numel(ct):
+    return ct.tensor.numel()
+
 @implements(torch.Tensor.cuda)
 def cuda(ct):
     return CategoricalTensor(ct.tensor.cuda(), num_classes=ct.num_classes)
 
 @implements(torch.Tensor.cpu)
 def cpu(ct):
     return CategoricalTensor(ct.tensor.cpu(), num_classes=ct.num_classes)
```

### Comparing `terrace-0.0.76/src/terrace/dataframe.py` & `terrace-0.0.77/src/terrace/dataframe.py`

 * *Files identical despite different names*

### Comparing `terrace-0.0.76/src/terrace/graph.py` & `terrace-0.0.77/src/terrace/graph.py`

 * *Files identical despite different names*

### Comparing `terrace-0.0.76/src/terrace/meta_utils.py` & `terrace-0.0.77/src/terrace/meta_utils.py`

 * *Files identical despite different names*

### Comparing `terrace-0.0.76/src/terrace/module.py` & `terrace-0.0.77/src/terrace/module.py`

 * *Files identical despite different names*

### Comparing `terrace-0.0.76/src/terrace.egg-info/PKG-INFO` & `terrace-0.0.77/src/terrace.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terrace
-Version: 0.0.76
+Version: 0.0.77
 Summary: high level PyTorch utils
 Home-page: https://github.com/mixarcid/terrace
 Author: Michael Brocidiacono
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

