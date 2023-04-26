# Comparing `tmp/easytree-0.1.8.tar.gz` & `tmp/easytree-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easytree-0.1.8.tar", last modified: Sun Jun 13 18:07:41 2021, max compression
+gzip compressed data, was "easytree-0.1.9.tar", last modified: Mon Jun 21 22:38:28 2021, max compression
```

## Comparing `easytree-0.1.8.tar` & `easytree-0.1.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 dschenck   (501) staff       (20)        0 2021-06-13 18:07:41.431859 easytree-0.1.8/
--rw-r--r--   0 dschenck   (501) staff       (20)     2907 2021-06-13 18:07:41.431682 easytree-0.1.8/PKG-INFO
--rw-r--r--   0 dschenck   (501) staff       (20)     1843 2021-06-13 18:03:58.000000 easytree-0.1.8/README.md
-drwxr-xr-x   0 dschenck   (501) staff       (20)        0 2021-06-13 18:07:41.430203 easytree-0.1.8/easytree/
--rw-r--r--   0 dschenck   (501) staff       (20)      233 2021-06-13 17:15:29.000000 easytree-0.1.8/easytree/__init__.py
--rw-r--r--   0 dschenck   (501) staff       (20)    18814 2021-06-13 17:19:56.000000 easytree-0.1.8/easytree/tree.py
-drwxr-xr-x   0 dschenck   (501) staff       (20)        0 2021-06-13 18:07:41.431016 easytree-0.1.8/easytree.egg-info/
--rw-r--r--   0 dschenck   (501) staff       (20)     2907 2021-06-13 18:07:41.000000 easytree-0.1.8/easytree.egg-info/PKG-INFO
--rw-r--r--   0 dschenck   (501) staff       (20)      216 2021-06-13 18:07:41.000000 easytree-0.1.8/easytree.egg-info/SOURCES.txt
--rw-r--r--   0 dschenck   (501) staff       (20)        1 2021-06-13 18:07:41.000000 easytree-0.1.8/easytree.egg-info/dependency_links.txt
--rw-r--r--   0 dschenck   (501) staff       (20)       15 2021-06-13 18:07:41.000000 easytree-0.1.8/easytree.egg-info/top_level.txt
--rw-r--r--   0 dschenck   (501) staff       (20)       38 2021-06-13 18:07:41.431908 easytree-0.1.8/setup.cfg
--rw-r--r--   0 dschenck   (501) staff       (20)      713 2021-06-13 18:03:16.000000 easytree-0.1.8/setup.py
-drwxr-xr-x   0 dschenck   (501) staff       (20)        0 2021-06-13 18:07:41.431239 easytree-0.1.8/tests/
--rw-r--r--   0 dschenck   (501) staff       (20)        0 2021-06-12 17:20:11.000000 easytree-0.1.8/tests/__init__.py
--rw-r--r--   0 dschenck   (501) staff       (20)     9970 2021-06-13 17:21:18.000000 easytree-0.1.8/tests/tree.py
+drwxr-xr-x   0 dschenck   (501) staff       (20)        0 2021-06-21 22:38:28.019868 easytree-0.1.9/
+-rw-r--r--   0 dschenck   (501) staff       (20)     3000 2021-06-21 22:38:28.019687 easytree-0.1.9/PKG-INFO
+-rw-r--r--   0 dschenck   (501) staff       (20)     1920 2021-06-20 16:17:19.000000 easytree-0.1.9/README.md
+drwxr-xr-x   0 dschenck   (501) staff       (20)        0 2021-06-21 22:38:28.018561 easytree-0.1.9/easytree/
+-rw-r--r--   0 dschenck   (501) staff       (20)      233 2021-06-13 18:21:49.000000 easytree-0.1.9/easytree/__init__.py
+-rw-r--r--   0 dschenck   (501) staff       (20)    20833 2021-06-21 22:36:32.000000 easytree-0.1.9/easytree/tree.py
+drwxr-xr-x   0 dschenck   (501) staff       (20)        0 2021-06-21 22:38:28.019109 easytree-0.1.9/easytree.egg-info/
+-rw-r--r--   0 dschenck   (501) staff       (20)     3000 2021-06-21 22:38:27.000000 easytree-0.1.9/easytree.egg-info/PKG-INFO
+-rw-r--r--   0 dschenck   (501) staff       (20)      216 2021-06-21 22:38:27.000000 easytree-0.1.9/easytree.egg-info/SOURCES.txt
+-rw-r--r--   0 dschenck   (501) staff       (20)        1 2021-06-21 22:38:27.000000 easytree-0.1.9/easytree.egg-info/dependency_links.txt
+-rw-r--r--   0 dschenck   (501) staff       (20)       15 2021-06-21 22:38:27.000000 easytree-0.1.9/easytree.egg-info/top_level.txt
+-rw-r--r--   0 dschenck   (501) staff       (20)       38 2021-06-21 22:38:28.019919 easytree-0.1.9/setup.cfg
+-rw-r--r--   0 dschenck   (501) staff       (20)      713 2021-06-21 22:24:52.000000 easytree-0.1.9/setup.py
+drwxr-xr-x   0 dschenck   (501) staff       (20)        0 2021-06-21 22:38:28.019317 easytree-0.1.9/tests/
+-rw-r--r--   0 dschenck   (501) staff       (20)        0 2021-06-13 18:21:49.000000 easytree-0.1.9/tests/__init__.py
+-rw-r--r--   0 dschenck   (501) staff       (20)    11227 2021-06-21 22:34:43.000000 easytree-0.1.9/tests/tree.py
```

### Comparing `easytree-0.1.8/PKG-INFO` & `easytree-0.1.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: easytree
-Version: 0.1.8
+Version: 0.1.9
 Summary: A fluent tree builder, useful to create multi-level, nested JSON configurations.
 Home-page: https://easytree.readthedocs.io/en/latest
 Author: david.schenck@outlook.com
 Author-email: david.schenck@outlook.com
 License: UNKNOWN
 Description: # easytree
         
-        [![PyPI version](https://badge.fury.io/py/easytree.svg)](https://badge.fury.io/py/easytree) [![Documentation Status](https://readthedocs.org/projects/easytree/badge/?version=latest)](https://easytree.readthedocs.io/en/latest/?badge=latest) 
+        ![build](https://github.com/dschenck/easytree/workflows/easytree/badge.svg)
+        [![PyPI version](https://badge.fury.io/py/easytree.svg)](https://badge.fury.io/py/easytree) 
+        [![Documentation Status](https://readthedocs.org/projects/easytree/badge/?version=latest)](https://easytree.readthedocs.io/en/latest/?badge=latest) 
         [![Downloads count](https://img.shields.io/pypi/dd/easytree)](https://img.shields.io/pypi/dd/easytree)
         [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
         
         A fluent tree builder, useful to create multi-level, nested JSON configurations.
         
         ## Documentation
         Documentation is hosted on [read the docs](https://easytree.readthedocs.io/en/latest/)
```

### Comparing `easytree-0.1.8/README.md` & `easytree-0.1.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # easytree
 
-[![PyPI version](https://badge.fury.io/py/easytree.svg)](https://badge.fury.io/py/easytree) [![Documentation Status](https://readthedocs.org/projects/easytree/badge/?version=latest)](https://easytree.readthedocs.io/en/latest/?badge=latest) 
+![build](https://github.com/dschenck/easytree/workflows/easytree/badge.svg)
+[![PyPI version](https://badge.fury.io/py/easytree.svg)](https://badge.fury.io/py/easytree) 
+[![Documentation Status](https://readthedocs.org/projects/easytree/badge/?version=latest)](https://easytree.readthedocs.io/en/latest/?badge=latest) 
 [![Downloads count](https://img.shields.io/pypi/dd/easytree)](https://img.shields.io/pypi/dd/easytree)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 A fluent tree builder, useful to create multi-level, nested JSON configurations.
 
 ## Documentation
 Documentation is hosted on [read the docs](https://easytree.readthedocs.io/en/latest/)
```

### Comparing `easytree-0.1.8/easytree/tree.py` & `easytree-0.1.9/easytree/tree.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,24 +9,82 @@
 class NODETYPES:
     DICT = "dict"
     LIST = "list"
     UNDEFINED = "undefined"
 
 
 class Node:
+    """
+    A recursive tree structure, supporting both dict and list nodes. New children nodes can be read and written as attributes, and dynamically becomes nodes themselves. 
+
+    Example
+    -------------
+    >>> root = easytree.Tree()
+    >>> root.user.firstname = "foo"
+    >>> root.user.firstname == root["user"]["firstname"] == "foo"
+    True
+    >>> root.user.friends.append(username="@jack")
+    >>> root
+    {
+        "user":{
+            "firstname":"foo"
+        },
+        "friends":[
+            {
+                "username":"@jack"
+            }
+        ]
+    }
+
+    The type of a newly-accessed node is initially *undefined*, but is cast as a dict or a list depending on subsequent interactions.
+
+    Example
+    ------------
+    >>> root = easytree.Tree()
+    >>> root.abc                              #abc is an undefined node
+    >>> root.abc.xyz                          #abc is cast to a dict node; xyz is undefined
+    >>> root.abc.xyz.append(firstname="Bob")  #xyz is cast to a list node with one dict node
+
+    A tree can be *serialized* back to native python objects using the :code:`serialize` method
+    
+    Example
+    -------------
+    >>> tree = easytree.Tree()
+    >>> tree.abc.xyz.append(44)
+    >>> tree.serialize()
+    {
+        "abc":{
+            "xyz:[
+                44
+            ]
+        }
+    }
+
+    A tree can be *sealed* or *frozen* to prevent further changes
+
+    Example
+    --------------
+    >>> tree = easytree.Tree({"abc":{"xyz":True}}, sealed=True)
+    >>> tree.abc.xyz = False
+    >>> tree.foo = "bar"
+    AttributeError: cannot set new attribute 'foo' on sealed node
+    """
+
     __hash__ = None
 
     def __new__(cls, value=None, *args, **kwargs):
         if cls is not Node:
             return super().__new__(cls)
         if value is None or isinstance(
-            value,
-            (list, tuple, set, range, zip, dict, Node, abc.KeysView, abc.ValuesView),
+            value, (list, tuple, set, range, zip, dict, abc.KeysView, abc.ValuesView)
         ):
             return super().__new__(cls)
+        # keep subclass instances intact
+        if isinstance(value, Node) and type(value) is Node:
+            return super().__new__(cls)
         return value
 
     def __init__(self, value=None, *, sealed=False, frozen=False):
         if isinstance(value, Node):
             value = value.serialize()
         if isinstance(value, dict):
             value = {k: Node(v, sealed=sealed, frozen=frozen) for k, v in value.items()}
@@ -39,15 +97,15 @@
                 "tree node must be initialized with either None, dict, or list"
             )
         self._value = value
         self._frozen = frozen
         self._sealed = sealed
 
     def __repr__(self):
-        return repr(serialize(self))
+        return f"Tree({repr(serialize(self))})"
 
     def __str__(self):
         return str(serialize(self))
 
     @property
     def __nodetype(self):
         """
@@ -61,45 +119,43 @@
             return NODETYPES.DICT
         raise RuntimeError
 
     def __getattr__(self, name):
         """
         Retrieves an attribute by name for dict nodes.
 
-        If the node is undefined, this operations casts the node to
-        a dict node.
+        If the node is undefined, this operations casts the node to a dict node.
 
         Raises an AttributeError for list nodes. 
         """
         if name == "_ipython_canary_method_should_not_exist_":
             return True  # ipython workaround
         if name in ("_frozen", "_sealed"):
             return False  # defaults for inheritence
         if self.__nodetype == NODETYPES.LIST:
-            raise AttributeError(f"list node has not attribute '{name}'")
+            raise AttributeError(f"list node has no attribute '{name}'")
         if self.__nodetype == NODETYPES.UNDEFINED:
             if self._frozen:
-                raise AttributeError(f"frozen node does not have '{name}' attribute")
+                raise AttributeError(f"frozen node has no attribute '{name}'")
             if self._sealed:
-                raise AttributeError(f"sealed node does not have '{name}' attribute")
+                raise AttributeError(f"sealed node has no attribute '{name}'")
             self._value = {}
         if name not in self._value:
             if self._frozen:
-                raise AttributeError(f"frozen node does not have '{name}' attribute")
+                raise AttributeError(f"frozen node has no attribute '{name}'")
             if self._sealed:
-                raise AttributeError(f"sealed node does not have '{name}' attribute")
+                raise AttributeError(f"sealed node has no attribute '{name}'")
             self._value[name] = Node(sealed=self._sealed, frozen=self._frozen)
         return self._value[name]
 
     def __setattr__(self, name, value):
         """
         Sets the value at an attribute for dict nodes. 
 
-        If the node is undefined, this operation casts the node to 
-        a dict node.
+        If the node is undefined, this operation casts the node to a dict node.
 
         Raises an AttributeError for list nodes. 
         """
         if name in ("_value", "_frozen", "_sealed"):
             return super().__setattr__(name, value)
         if name in {"serialize", "get", "append"}:
             raise AttributeError(f"Attribute '{name}' is read-only")
@@ -118,15 +174,15 @@
                 raise AttributeError(f"cannot set attribute '{name}' on frozen node")
             if name not in self._value and self._sealed:
                 raise AttributeError(
                     f"cannot set new attribute '{name}' on sealed node"
                 )
             self._value[name] = Node(value, sealed=self._sealed, frozen=self._frozen)
             return
-        raise AttributeError(f"list node has not attribute '{name}'")
+        raise AttributeError(f"list node has no attribute '{name}'")
 
     def __delattr__(self, name):
         """
         Remove an attribute by name
         """
         if name in {
             "__nodetype",
@@ -146,17 +202,15 @@
             raise AttributeError(f"cannot delete attribute '{name}' on sealed node")
         del self._value[name]
 
     def __getitem__(self, name):
         """
         Retrieves an item at an index (for list nodes) or at a key (for dict nodes). 
 
-        If the node is undefined, this operation casts the node to a dict node, 
-        unless the given key/index is an integer; instead, an AmbiguityError error is 
-        raised.
+        If the node is undefined, this operation casts the node to a dict node, unless the given key/index is an integer; instead, an AmbiguityError error is raised.
         """
         if self.__nodetype == NODETYPES.UNDEFINED:
             if self._frozen:
                 raise KeyError(f"frozen node has no value for '{name}'")
             if self._sealed:
                 raise KeyError(f"sealed node has no value for '{name}'")
             if isinstance(name, (int, slice)):
@@ -181,16 +235,15 @@
             return self._value[name]
         raise RuntimeError
 
     def __setitem__(self, name, value):
         """
         Sets the value at an index (for list nodes) or at a key (for dict node). 
 
-        If the node is undefined, this operation casts the node to a dict node, 
-        unlesss the given key/index is a slice object. 
+        If the node is undefined, this operation casts the node to a dict node, unlesss the given key/index is a slice object. 
         """
         if self._frozen:
             raise TypeError(f"cannot set item '{name}' on frozen node")
         if self.__nodetype == NODETYPES.UNDEFINED:
             if isinstance(name, int):
                 raise IndexError("list assignment index out of range")
             elif isinstance(name, slice):
@@ -261,20 +314,20 @@
 
         Example
         ---------
         >>> tree = easytree.Tree()                                 #undefined node
         >>> tree.append("hello world")                            #casts node to list
         >>> tree.append(name="David", age=29)                     #call with kwargs
         >>> tree.append({"animal":"elephant", "country":"India"}) #call with args
-        >>> easytree.serialize(tree)
+        >>> tree.serialize()
         ["Hello world",{"name":"David","age":29},{"animal":"elephant", "country":"India"}]
 
         Note
         ---------
-        The append method intentionally returns a reference to the last-added item, if that item is a new node. This allows for more fluent code using the context manager. 
+        The append method intentionally returns a reference to the last-added item, if that item is a new node. This allows for fluent code using the context manager. 
 
         Example
         -----------
         >>> chart = easytree.Tree()
         >>> with chart.axes.append({}) as axis: 
         ...     axis.title.text = "primary axis"
         >>> with chart.axes.append({}) as axis: 
@@ -312,16 +365,15 @@
             value = Node(value, sealed=self._sealed, frozen=self._frozen)
             self._value.append(value)
             return value if isinstance(value, Node) else None
         raise AttributeError("dict node has no attribute 'append'")
 
     def get(self, key, default=None):
         """
-        Returns the value at a given key, or default if the key does 
-        not exists.
+        Returns the value at a given key, or default if the key does not exists.
 
         Example
         ---------------------
         >>> config = easytree.Tree({"context":{"starting":"2016-03-31"}})
         >>> config.context.get("starting", "2014-01-01")
         2016-03-31
         >>> config.context.get("ending", "2021-12-31")
@@ -391,15 +443,15 @@
         }
         """
         return serialize(self)
 
 
 def serialize(tree):
     """
-    Recursively converts an :code:`easytree.Tree` to a native python type.
+    Recursively converts an :code:`easytree.Tree` back to a native python type.
 
     Example
     ---------------------
     >>> chart = easytree.Tree()
     >>> chart.chart.type = "bar"
     >>> chart.title.text = "France Olympic Medals"
     >>> chart.xAxis.categories = ["Gold", "Silver", "Bronze"]
@@ -462,57 +514,63 @@
     Creates a new :code:`easytree.Tree`
     """
     return Node(root, sealed=sealed, frozen=frozen)
 
 
 def load(stream, *args, frozen=False, sealed=False, **kwargs):
     """
-    Deserialize a text file or binary file containing a JSON 
-    document to an easytree.Tree object 
+    Deserialize a text file or binary file containing a JSON document to an :code:`Tree` object 
+
+
+    :code:`*args` and :code:`**kwargs` are passed to the :code:`json.load` function
 
     Example
     -------------
     >>> with open("data.json", "r") as file: 
     ...     tree = easytree.load(file)
     """
     return Node(json.load(stream, *args, **kwargs), sealed=sealed, frozen=frozen)
 
 
 def loads(s, *args, frozen=False, sealed=False, **kwargs):
     """
-    Deserialize s (a str, bytes or bytearray instance containing a JSON document) 
-    to an easytree.Node object 
+    Deserialize s (a str, bytes or bytearray instance containing a JSON document) to an :code:`Tree` object 
+
+    :code:`*args` and :code:`**kwargs` are passed to the :code:`json.loads` function
     """
     return Node(json.loads(s, *args, **kwargs), sealed=sealed, frozen=frozen)
 
 
 def dump(obj, stream, *args, **kwargs):
     """
-    Serialize easytree.Tree object as a JSON formatted string 
-    to stream (a .write()-supporting file-like object)
+    Serialize :code:`Tree` object as a JSON formatted string to stream (a .write()-supporting file-like object). 
+
+    :code:`*args` and :code:`**kwargs` are passed to the :code:`json.dump` function
 
     Example
     -------------
     >>> tree = easytree.Tree({"foo": "bar"})
     >>> with open("data.json", "w") as file: 
     ...     easytree.dump(tree, file, indent=4)
     """
     return json.dump(serialize(obj), stream, *args, **kwargs)
 
 
 def dumps(obj, *args, **kwargs):
     """
-    Serialize easytree.Tree to a JSON formatted string
+    Serialize :code:`Tree` to a JSON formatted string. 
+
+    :code:`*args` and :code:`**kwargs` are passed to the :code:`json.dumps` function
     """
     return json.dumps(serialize(obj), *args, **kwargs)
 
 
 def frozen(tree):
     """
-    Returns True if the tree is frozen
+    Returns :code:`True` if the tree is frozen
     """
     if not isinstance(tree, Node):
         raise TypeError(
             f"Expected tree to be instance of easytree.Tree, received {type(tree)}"
         )
     return tree._frozen
 
@@ -537,15 +595,15 @@
             f"Expected tree to be instance of easytree.Tree, received {type(tree)}"
         )
     return Node(tree, frozen=False)
 
 
 def sealed(tree):
     """
-    Returns True if the tree is sealed
+    Returns :code:`True` if the tree is sealed
     """
     if not isinstance(tree, Node):
         raise TypeError(
             f"Expected tree to be instance of easytree.Tree, received {type(tree)}"
         )
     return tree._frozen
```

### Comparing `easytree-0.1.8/easytree.egg-info/PKG-INFO` & `easytree-0.1.9/easytree.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: easytree
-Version: 0.1.8
+Version: 0.1.9
 Summary: A fluent tree builder, useful to create multi-level, nested JSON configurations.
 Home-page: https://easytree.readthedocs.io/en/latest
 Author: david.schenck@outlook.com
 Author-email: david.schenck@outlook.com
 License: UNKNOWN
 Description: # easytree
         
-        [![PyPI version](https://badge.fury.io/py/easytree.svg)](https://badge.fury.io/py/easytree) [![Documentation Status](https://readthedocs.org/projects/easytree/badge/?version=latest)](https://easytree.readthedocs.io/en/latest/?badge=latest) 
+        ![build](https://github.com/dschenck/easytree/workflows/easytree/badge.svg)
+        [![PyPI version](https://badge.fury.io/py/easytree.svg)](https://badge.fury.io/py/easytree) 
+        [![Documentation Status](https://readthedocs.org/projects/easytree/badge/?version=latest)](https://easytree.readthedocs.io/en/latest/?badge=latest) 
         [![Downloads count](https://img.shields.io/pypi/dd/easytree)](https://img.shields.io/pypi/dd/easytree)
         [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
         
         A fluent tree builder, useful to create multi-level, nested JSON configurations.
         
         ## Documentation
         Documentation is hosted on [read the docs](https://easytree.readthedocs.io/en/latest/)
```

### Comparing `easytree-0.1.8/setup.py` & `easytree-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="easytree",
-    version="0.1.8",
+    version="0.1.9",
     author="david.schenck@outlook.com",
     author_email="david.schenck@outlook.com",
     description="A fluent tree builder, useful to create multi-level, nested JSON configurations.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://easytree.readthedocs.io/en/latest",
     packages=setuptools.find_packages(),
```

### Comparing `easytree-0.1.8/tests/tree.py` & `easytree-0.1.9/tests/tree.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,14 +25,18 @@
         self.assertEqual(tree, 1)
         self.assertIsInstance(tree, int)
 
         tree = easytree.tree.Node(True)
         self.assertEqual(tree, True)
         self.assertIsInstance(tree, bool)
 
+        foo = easytree.Tree({})
+        bar = easytree.Tree(foo)
+        self.assertIsNot(foo, bar)
+
     def test_copy(self):
         this = easytree.Tree(
             {"name": "foo", "numbers": [1, 3, 5], "address": {"country": "US"}}
         )
         that = easytree.Tree(this)
 
         self.assertIsInstance(that, easytree.Tree)
@@ -145,34 +149,63 @@
             self.assertIsInstance(child, int)
 
         tree = easytree.new({"name": "David", "age": 29})
         for child in tree:
             self.assertIsInstance(child, str)
 
     def test_inheritence(self):
+        class Grandchild(easytree.Tree):
+            def walk(self):
+                return "walking"
+
         class Child(easytree.Tree):
             def __init__(self, name, age):
+                self.child = Grandchild()
                 self.name = name
                 self.age = age
 
         instance = Child("Bob", 29)
         instance.address.number = 1
         instance.address.street = "avenue Montaigne"
         instance.address.city = "Paris"
         instance.address.country = "France"
 
         self.assertIsInstance(instance.address, easytree.Tree)
         self.assertIsInstance(instance.address, easytree.tree.Node)
-        self.assertEqual(set(instance.serialize()), set(("name", "age", "address")))
+        self.assertIsInstance(instance.child, Grandchild)
+        self.assertEqual(instance.child.walk(), "walking")
+        self.assertEqual(
+            set(instance.serialize()), set(("child", "name", "age", "address"))
+        )
         self.assertEqual(
             set(instance.serialize()["address"]),
             set(("number", "street", "city", "country")),
         )
         self.assertEqual(instance.serialize()["address"]["city"], "Paris")
 
+        # passing subclasses returns instance
+        grandchild = Grandchild()
+        altinstance = easytree.Tree(grandchild)
+        self.assertIsInstance(altinstance, Grandchild)
+        self.assertIs(altinstance, grandchild)
+
+        class Child(easytree.Tree):
+            def append(self, value, *args, **kwargs):
+                super().append(value=value, **kwargs)
+                return (value, len(args), len(kwargs))
+
+        instance = Child()
+
+        self.assertIsInstance(instance, easytree.Tree)
+        self.assertIsInstance(instance, Child)
+        self.assertEqual(instance.append("test"), ("test", 0, 0))
+        self.assertEqual(instance.append("test", 1), ("test", 1, 0))
+        self.assertEqual(instance.append("test", name="alpha"), ("test", 0, 1))
+        self.assertEqual(instance.append("test", True, name="alpha"), ("test", 1, 1))
+
     def test_contextmanager(self):
         chart = easytree.new()
 
         with chart.axes.append({}) as axis:
             axis.title.text = "primary axis"
         with chart.axes.append({}) as axis:
             axis.title.text = "secondary axis"
```

