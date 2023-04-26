# Comparing `tmp/ipv4tree-0.0.6.tar.gz` & `tmp/ipv4tree-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipv4tree-0.0.6.tar", last modified: Sat Apr 15 09:52:10 2023, max compression
+gzip compressed data, was "ipv4tree-0.0.7.tar", last modified: Tue Apr 25 20:04:23 2023, max compression
```

## Comparing `ipv4tree-0.0.6.tar` & `ipv4tree-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 dvolkow   (1000) dvolkow   (1000)        0 2023-04-15 09:52:10.634602 ipv4tree-0.0.6/
--rw-rw-r--   0 dvolkow   (1000) dvolkow   (1000)    35149 2023-04-05 06:34:33.000000 ipv4tree-0.0.6/LICENSE
--rw-rw-r--   0 dvolkow   (1000) dvolkow   (1000)        0 2023-04-05 06:34:33.000000 ipv4tree-0.0.6/MANIFEST.in
--rw-rw-r--   0 dvolkow   (1000) dvolkow   (1000)      259 2023-04-15 09:52:10.634602 ipv4tree-0.0.6/PKG-INFO
--rw-rw-r--   0 dvolkow   (1000) dvolkow   (1000)     5344 2023-04-15 09:51:17.000000 ipv4tree-0.0.6/README.md
-drwxrwxr-x   0 dvolkow   (1000) dvolkow   (1000)        0 2023-04-15 09:52:10.634602 ipv4tree-0.0.6/ipv4tree/
--rw-rw-r--   0 dvolkow   (1000) dvolkow   (1000)       69 2023-04-15 08:33:57.000000 ipv4tree-0.0.6/ipv4tree/__init__.py
--rw-rw-r--   0 dvolkow   (1000) dvolkow   (1000)    16870 2023-04-15 09:42:17.000000 ipv4tree-0.0.6/ipv4tree/ipv4tree.py
--rw-rw-r--   0 dvolkow   (1000) dvolkow   (1000)     1395 2023-04-15 08:46:50.000000 ipv4tree-0.0.6/ipv4tree/multiprocessing.py
--rw-rw-r--   0 dvolkow   (1000) dvolkow   (1000)     1043 2023-04-14 17:06:56.000000 ipv4tree-0.0.6/ipv4tree/utils.py
-drwxrwxr-x   0 dvolkow   (1000) dvolkow   (1000)        0 2023-04-15 09:52:10.634602 ipv4tree-0.0.6/ipv4tree.egg-info/
--rw-rw-r--   0 dvolkow   (1000) dvolkow   (1000)      259 2023-04-15 09:52:10.000000 ipv4tree-0.0.6/ipv4tree.egg-info/PKG-INFO
--rw-rw-r--   0 dvolkow   (1000) dvolkow   (1000)      285 2023-04-15 09:52:10.000000 ipv4tree-0.0.6/ipv4tree.egg-info/SOURCES.txt
--rw-rw-r--   0 dvolkow   (1000) dvolkow   (1000)        1 2023-04-15 09:52:10.000000 ipv4tree-0.0.6/ipv4tree.egg-info/dependency_links.txt
--rw-rw-r--   0 dvolkow   (1000) dvolkow   (1000)       10 2023-04-15 09:52:10.000000 ipv4tree-0.0.6/ipv4tree.egg-info/requires.txt
--rw-rw-r--   0 dvolkow   (1000) dvolkow   (1000)        9 2023-04-15 09:52:10.000000 ipv4tree-0.0.6/ipv4tree.egg-info/top_level.txt
--rw-rw-r--   0 dvolkow   (1000) dvolkow   (1000)       38 2023-04-15 09:52:10.634602 ipv4tree-0.0.6/setup.cfg
--rw-rw-r--   0 dvolkow   (1000) dvolkow   (1000)      447 2023-04-05 06:34:33.000000 ipv4tree-0.0.6/setup.py
+drwxrwxr-x   0 dvolkow   (1000) dvolkow   (1000)        0 2023-04-25 20:04:23.803401 ipv4tree-0.0.7/
+-rw-rw-r--   0 dvolkow   (1000) dvolkow   (1000)    35149 2023-04-05 06:34:33.000000 ipv4tree-0.0.7/LICENSE
+-rw-rw-r--   0 dvolkow   (1000) dvolkow   (1000)        0 2023-04-05 06:34:33.000000 ipv4tree-0.0.7/MANIFEST.in
+-rw-rw-r--   0 dvolkow   (1000) dvolkow   (1000)      259 2023-04-25 20:04:23.803401 ipv4tree-0.0.7/PKG-INFO
+-rw-rw-r--   0 dvolkow   (1000) dvolkow   (1000)     5344 2023-04-25 18:54:09.000000 ipv4tree-0.0.7/README.md
+drwxrwxr-x   0 dvolkow   (1000) dvolkow   (1000)        0 2023-04-25 20:04:23.803401 ipv4tree-0.0.7/ipv4tree/
+-rw-rw-r--   0 dvolkow   (1000) dvolkow   (1000)       69 2023-04-25 19:52:16.000000 ipv4tree-0.0.7/ipv4tree/__init__.py
+-rw-rw-r--   0 dvolkow   (1000) dvolkow   (1000)    17722 2023-04-25 19:52:16.000000 ipv4tree-0.0.7/ipv4tree/ipv4tree.py
+-rw-rw-r--   0 dvolkow   (1000) dvolkow   (1000)     1395 2023-04-25 18:54:09.000000 ipv4tree-0.0.7/ipv4tree/multiprocessing.py
+-rw-rw-r--   0 dvolkow   (1000) dvolkow   (1000)     1043 2023-04-25 18:54:09.000000 ipv4tree-0.0.7/ipv4tree/utils.py
+drwxrwxr-x   0 dvolkow   (1000) dvolkow   (1000)        0 2023-04-25 20:04:23.803401 ipv4tree-0.0.7/ipv4tree.egg-info/
+-rw-rw-r--   0 dvolkow   (1000) dvolkow   (1000)      259 2023-04-25 20:04:23.000000 ipv4tree-0.0.7/ipv4tree.egg-info/PKG-INFO
+-rw-rw-r--   0 dvolkow   (1000) dvolkow   (1000)      285 2023-04-25 20:04:23.000000 ipv4tree-0.0.7/ipv4tree.egg-info/SOURCES.txt
+-rw-rw-r--   0 dvolkow   (1000) dvolkow   (1000)        1 2023-04-25 20:04:23.000000 ipv4tree-0.0.7/ipv4tree.egg-info/dependency_links.txt
+-rw-rw-r--   0 dvolkow   (1000) dvolkow   (1000)       10 2023-04-25 20:04:23.000000 ipv4tree-0.0.7/ipv4tree.egg-info/requires.txt
+-rw-rw-r--   0 dvolkow   (1000) dvolkow   (1000)        9 2023-04-25 20:04:23.000000 ipv4tree-0.0.7/ipv4tree.egg-info/top_level.txt
+-rw-rw-r--   0 dvolkow   (1000) dvolkow   (1000)       38 2023-04-25 20:04:23.803401 ipv4tree-0.0.7/setup.cfg
+-rw-rw-r--   0 dvolkow   (1000) dvolkow   (1000)      447 2023-04-25 18:54:02.000000 ipv4tree-0.0.7/setup.py
```

### Comparing `ipv4tree-0.0.6/LICENSE` & `ipv4tree-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ipv4tree-0.0.6/README.md` & `ipv4tree-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `ipv4tree-0.0.6/ipv4tree/ipv4tree.py` & `ipv4tree-0.0.7/ipv4tree/ipv4tree.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 from collections.abc import Collection, Iterable
 from ipaddress import IPv4Address, IPv4Network
 from typing import Union, Optional, Dict
 from ipv4tree.utils import _get_binary_path_from_ipv4_addr
 
 
+def prefixsize(n: int) -> int:
+    return 2 ** (32 - n)
+
+
 class IPv4TreeNode(Iterable):
     """
     Unit for IPv4Tree structure.
     """
 
     def __init__(self, key: Union[int, str],
                  prefixlen: int,
@@ -39,14 +43,18 @@
     def prefix(self) -> str:
         return self._prefix
 
     @property
     def prefixlen(self) -> int:
         return self._prefixlen
 
+    @property
+    def prefixsize(self) -> int:
+        return 2 ** (32 - self.prefixlen)
+
     def child(self, key: Union[int, str]) -> Union['IPv4TreeNode', None]:
         return self._children[int(key)]
 
     @property
     def children(self) -> list:
         return self._children
 
@@ -94,14 +102,25 @@
     def __int__(self) -> int:
         from copy import deepcopy
         s = deepcopy(self._prefix)
         for _ in range(32 - self._prefixlen):
             s = "".join([s, "0"])
         return int(s, 2)
 
+    def sizeof(self) -> int:
+        if self.islast:
+            return self._size if self._size > 0 else self.prefixsize
+
+        size = 0
+        for child in self._children:
+            if child is not None:
+                size += child.sizeof()
+
+        return size
+
     def __str__(self) -> str:
         if self._prefixlen > 0:
             return "/".join([str(IPv4Address(int(self))),
                              str(self._prefixlen)])
         return "root"
 
     def _is_root(self) -> bool:
@@ -143,40 +162,53 @@
     def __add__(self, other: 'IPv4Tree'):
         for node in other:
             if node.islast:
                 self.insert(str(node))
 
         return self
 
+    def sizeof(self, ip: Union[str, int, IPv4Address, IPv4Network]) -> int:
+        net = IPv4Network(ip)
+        node = self._root
+        for n in _get_binary_path_from_ipv4_addr(net):
+            node = node.child(n)
+            if node is None:
+                return 0
+
+            if node.prefixlen == net.prefixlen:
+                break
+
+        return node.sizeof()
+
     def delete(self, ip: Union[str, int, IPv4Address, IPv4Network]) -> None:
         """
         Delete IPv4 address or network from tree
         :param ip: IPv4 address or network
         """
         net = IPv4Network(ip)
         if not self.intree(ip):
             raise ValueError('Network {} not in tree'.format(str(net)))
 
-        size = net.num_addresses
+        size = self.sizeof(ip)
         node = self._root
         prev = node
         in_last = False
         for n in _get_binary_path_from_ipv4_addr(net):
             prev = node
             node = prev.child(n)
             inv_key = '1' if n == '0' else '0'
             inv_node = prev.child(inv_key)
             if prev.islast and not in_last:
                 in_last = True
 
             if node is None:
-                node = self._insert_node(prev, n, 0)
+                node = self._insert_node(prev, n, prefixsize(prev.prefixlen + 1))
 
             if inv_node is None:
-                inv_node = self._insert_node(prev, inv_key, 0)
+                inv_node = self._insert_node(prev, inv_key, prefixsize(prev.prefixlen + 1))
                 inv_node._islast = in_last
 
             prev._islast = False
             if node.prefixlen == net.prefixlen:
                 break
 
         prev.new_child(n, None)
```

### Comparing `ipv4tree-0.0.6/ipv4tree/multiprocessing.py` & `ipv4tree-0.0.7/ipv4tree/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `ipv4tree-0.0.6/ipv4tree/utils.py` & `ipv4tree-0.0.7/ipv4tree/utils.py`

 * *Files identical despite different names*

