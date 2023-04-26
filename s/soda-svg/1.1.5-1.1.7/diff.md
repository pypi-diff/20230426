# Comparing `tmp/soda_svg-1.1.5.tar.gz` & `tmp/soda_svg-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soda_svg-1.1.5.tar", max compression
+gzip compressed data, was "soda_svg-1.1.7.tar", max compression
```

## Comparing `soda_svg-1.1.5.tar` & `soda_svg-1.1.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1073 2023-04-26 12:02:59.528414 soda_svg-1.1.5/LICENSE
--rw-r--r--   0        0        0    11021 2023-04-26 12:02:59.528414 soda_svg-1.1.5/README.md
--rw-r--r--   0        0        0      497 2023-04-26 12:02:59.532413 soda_svg-1.1.5/pyproject.toml
--rw-r--r--   0        0        0      274 2023-04-26 12:02:59.532413 soda_svg-1.1.5/soda/__init__.py
--rw-r--r--   0        0        0      123 2023-04-26 12:02:59.532413 soda_svg-1.1.5/soda/config_mod.py
--rw-r--r--   0        0        0     2081 2023-04-26 12:02:59.532413 soda_svg-1.1.5/soda/custom_tags.py
--rw-r--r--   0        0        0     7353 2023-04-26 12:02:59.532413 soda_svg-1.1.5/soda/paths.py
--rw-r--r--   0        0        0    11905 2023-04-26 12:02:59.532413 soda_svg-1.1.5/soda/point.py
--rw-r--r--   0        0        0     8656 2023-04-26 12:02:59.532413 soda_svg-1.1.5/soda/tags.py
--rw-r--r--   0        0        0     1551 2023-04-26 12:02:59.532413 soda_svg-1.1.5/soda/utils.py
--rw-r--r--   0        0        0      924 2023-04-26 12:02:59.532413 soda_svg-1.1.5/soda/xml_parse.py
--rw-r--r--   0        0        0    11707 1970-01-01 00:00:00.000000 soda_svg-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-26 15:31:57.169270 soda_svg-1.1.7/LICENSE
+-rw-r--r--   0        0        0    11789 2023-04-26 15:31:57.169270 soda_svg-1.1.7/README.md
+-rw-r--r--   0        0        0      515 2023-04-26 15:31:57.169270 soda_svg-1.1.7/pyproject.toml
+-rw-r--r--   0        0        0      274 2023-04-26 15:31:57.169270 soda_svg-1.1.7/soda/__init__.py
+-rw-r--r--   0        0        0      123 2023-04-26 15:31:57.169270 soda_svg-1.1.7/soda/config_mod.py
+-rw-r--r--   0        0        0     2161 2023-04-26 15:31:57.169270 soda_svg-1.1.7/soda/custom_tags.py
+-rw-r--r--   0        0        0     7357 2023-04-26 15:31:57.169270 soda_svg-1.1.7/soda/paths.py
+-rw-r--r--   0        0        0    11689 2023-04-26 15:31:57.169270 soda_svg-1.1.7/soda/point.py
+-rw-r--r--   0        0        0    10460 2023-04-26 15:31:57.169270 soda_svg-1.1.7/soda/tags.py
+-rw-r--r--   0        0        0     1838 2023-04-26 15:31:57.169270 soda_svg-1.1.7/soda/utils.py
+-rw-r--r--   0        0        0      924 2023-04-26 15:31:57.169270 soda_svg-1.1.7/soda/xml_parse.py
+-rw-r--r--   0        0        0    12475 1970-01-01 00:00:00.000000 soda_svg-1.1.7/PKG-INFO
```

### Comparing `soda_svg-1.1.5/LICENSE` & `soda_svg-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `soda_svg-1.1.5/README.md` & `soda_svg-1.1.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -205,15 +205,25 @@
 
 tag = Tag.g(Tag.a)
 tag[0]["href"] = "https://github.com/evtn/soda"
 print(tag[1]) # IndexError
 print(tag[0]) # prints <a href="https://github.com/evtn/soda" />
 ```
 
-Children can also be accessed directly through `tag.children` attribute.
+~~Children can also be accessed directly through `tag.children` attribute.~~
+
+This is not necessary for most tasks as of 1.1.6 with new methods and iterator protocol:
+
+- `Tag.insert(int, Node)` inserts a node on an index. Be aware that `tag.children` is not flattened: `Tag.g("test", ["test1", "test2"]).insert(2, elem)` will insert `elem` *after* the array.
+- `Tag.append(Node)` appends one node to the tag.
+- `Tag.extend(*Node)` appends several nodes to the tag. *This is not the same as `.append([*Node])`*
+- `Tag.pop(int?)` pops one node from specified index. If index is not provided, pops the last one.
+- `Tag.iter_raw()` returns an iterable to get every Node of the tag. This doesn't dive into nested arrays, for that behaviour iterate over `Tag`
+- You can also iterate over the `Tag` itself to get every flat node of it (no arrays)
+
 
 ## Fragments
 
 Fragments use concept similar to React's fragment. It renders just it's children:
 
 ```python
 from soda import Tag, Fragment
```

### Comparing `soda_svg-1.1.5/soda/custom_tags.py` & `soda_svg-1.1.7/soda/custom_tags.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from __future__ import annotations
 
 from base64 import b64encode
+from os import PathLike
 from typing import BinaryIO
 from .tags import Node, Tag
+from pathlib import Path
 
 
 class Root(Tag):
     def __init__(
         self, *children: Node, use_namespace: bool = False, **attributes: Node
     ):
         super().__init__("svg", *children, self_closing=False, **attributes)
@@ -59,10 +61,12 @@
     @staticmethod
     def from_file(file_object: BinaryIO, extension: str, **init_kwargs: bool) -> Image:
         contents: str = b64encode(file_object.read()).decode("ascii")
 
         return Image(f"data:image/{extension};base64,{contents}", **init_kwargs)
 
     @staticmethod
-    def from_filename(filename: str, extension: str, **init_kwargs: bool) -> Image:
-        with open(filename, "rb") as file:
+    def from_path(
+        pathlike: str | PathLike[str], extension: str, **init_kwargs: bool
+    ) -> Image:
+        with Path(pathlike).open("rb") as file:
             return Image.from_file(file, extension, **init_kwargs)
```

### Comparing `soda_svg-1.1.5/soda/paths.py` & `soda_svg-1.1.7/soda/paths.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,19 +61,19 @@
     @staticmethod
     def horizontal(x: float = 0, *, relative: bool = False) -> str:
         prefix = "Hh"[relative]
         return " ".join(map(value_to_str, [prefix, x]))
 
     @staticmethod
     def H(x: float) -> str:
-        return Path.vertical(x, relative=False)
+        return Path.horizontal(x, relative=False)
 
     @staticmethod
     def h(x: float) -> str:
-        return Path.vertical(x, relative=True)
+        return Path.horizontal(x, relative=True)
 
     # Z
     @staticmethod
     def close(*, relative: bool = False) -> str:
         # there's no difference between two, but consistent API is better
         return "Zz"[relative]
```

### Comparing `soda_svg-1.1.5/soda/point.py` & `soda_svg-1.1.7/soda/point.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,17 @@
 from __future__ import annotations
 from typing import Iterator, Sequence, Union, overload
-from math import pi, cos, sin, hypot, acos
+from math import cos, sin, hypot, acos, radians as degrees_to_radians
 
 from .utils import eq
 from .paths import Path, compact_path
 from .tags import Node, Tag
 
 PointLike = Union["Point", float, Sequence[float]]
 
-rad_to_deg_k = 180 / pi
-
-
-def radians_to_degrees(radians: float) -> float:
-    return radians * rad_to_deg_k
-
-
-def degrees_to_radians(degrees: float) -> float:
-    return degrees / rad_to_deg_k
-
 
 class Point:
     def __init__(self, x: float = 0, y: float = 0):
         self.coords = x, y
         self.x: float = x
         self.y: float = y
 
@@ -147,30 +137,26 @@
         return f"Point[{self.x}, {self.y}]"
 
     def as_(self, x_argname: str = "x", y_argname: str = "y") -> dict[str, float]:
         return {x_argname: self.x, y_argname: self.y}
 
     def angle(self, other: PointLike = (1, 0), center: PointLike = 0) -> float:
         center = Point.from_(center)
-        other = Point.from_(other) - center
-        self = self - center
+        other = (Point.from_(other) - center).normalized()
+        self = (self - center).normalized()
 
         dot_product = sum(self * other)
-        distance_product = self.distance() * other.distance()
 
-        if distance_product == 0:
-            return 0
-
-        return acos(dot_product / distance_product)
+        return acos(dot_product)
 
     def normalized(self) -> Point:
         return self / self.distance()
 
     def __eq__(self, other: object) -> bool:
-        if not isinstance(other, (Point, float, list, tuple)):
+        if not isinstance(other, (Point, float, int, list, tuple)):
             return False
         other = Point.from_(other)
         return eq((self - other).distance(), 0)
 
 
 class PointPath:
     @staticmethod
@@ -225,19 +211,19 @@
     @staticmethod
     def horizontal(point: PointLike = 0, *, relative: bool = False) -> str:
         point = Point.from_(point)
         return Path.horizontal(point.x, relative=relative)
 
     @staticmethod
     def H(point: PointLike = 0) -> str:
-        return PointPath.vertical(point, relative=False)
+        return PointPath.horizontal(point, relative=False)
 
     @staticmethod
     def h(point: PointLike = 0) -> str:
-        return PointPath.vertical(point, relative=True)
+        return PointPath.horizontal(point, relative=True)
 
     # Z
     @staticmethod
     def close(*, relative: bool = False) -> str:
         return Path.close(relative=relative)
 
     @staticmethod
@@ -383,17 +369,19 @@
     @staticmethod
     def polygon(*points: Point, **attributes: Node) -> Tag:
         commands = [
             PointPath.line(point) if i else PointPath.moveto(point)
             for i, point in enumerate(points)
         ]
 
-        return Tag.path(d=PointPath.build(*commands, PointPath.close()), **attributes)
+        return Tag.path(
+            d=PointPath.build(*commands, PointPath.close(), compact=True), **attributes
+        )
 
     @staticmethod
     def polyline(*points: Point, **attributes: Node) -> Tag:
         commands = [
             PointPath.line(point) if i else PointPath.moveto(point)
             for i, point in enumerate(points)
         ]
 
-        return Tag.path(d=PointPath.build(*commands), **attributes)
+        return Tag.path(d=PointPath.build(*commands, compact=True), **attributes)
```

### Comparing `soda_svg-1.1.5/soda/tags.py` & `soda_svg-1.1.7/soda/tags.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 from __future__ import annotations
-from typing import Iterable, Optional, Union, overload
+from typing import Iterable, Iterator, Optional, Sequence, Union, overload
 
-
-Node = Union["Tag", str, float, "list[Node]"]
-
-
-from .utils import escape, normalize_ident, trunc
+FlatNode = Union["Tag", str, float]
+Node = Union[FlatNode, "list[Node]"]
 
 
 class MetaTag(type):
     def __getattr__(self, tag_name: str) -> Tag:
         return Tag(tag_name)
 
 
@@ -137,45 +134,109 @@
     ) -> Optional[Union[Node, list[Node], Node]]:
         # check __setitem__ for explanation of ignore
         if isinstance(item, (int, slice)):  # type: ignore[misc]
             return self.children[item]
 
         return self.get_attribute(item)
 
+    def insert(self, index: int, node: Node) -> None:
+        """Inserts an entry into the tag"""
+        self.children.insert(index, node)
+
+    def append(self, child: Node) -> None:
+        """A more list-like way to add a node to the tag"""
+        self(child)
+
+    def extend(self, children: Sequence[Node]) -> None:
+        """A more list-like way to add several nodes to the tag"""
+        self(*children)
+
+    def pop(self, index: int = -1) -> Node:
+        """Pop one (by default last one) entry from the tag"""
+        return self.children.pop(index)
+
+    def __iter__(self) -> Iterator[FlatNode]:
+        return iter(node_iterator(self.children))
+
+    def iter_raw(self) -> Iterator[Node]:
+        return iter(self.children)
+
     def __call__(self, *children: Node, **attributes: Node) -> Tag:
-        if children:
-            self.children.extend(children)
+        self.children.extend(children)
+
         if attributes:
             for attr in attributes:
                 self[attr] = attributes[attr]
         return self
 
     def __repr__(self) -> str:
         return f"Tag<{self.tag_name} attributes: {len(self.attributes)}>children: {len(self.children)}</{self.tag_name}>"
 
     def __str__(self) -> str:
         return self.render()
 
     def build_child(
-        self, child: Node, tab_size: int = 0, tab_level: int = 0
+        self, child: FlatNode, tab_size: int = 0, tab_level: int = 0
     ) -> Iterable[str]:
         if isinstance(child, (float, int)):
-            return self.build_child(str(trunc(child)), tab_size, tab_level)
+            yield from self.build_child(str(trunc(child)), tab_size, tab_level)
+            return
 
         if isinstance(child, str):
             yield " " * (tab_size * tab_level)
             yield escape(child)
 
-        elif isinstance(child, list):
-            for subchild in child:
-                yield from self.build_child(subchild, tab_size, tab_level)
-
         else:
             yield from child.build(tab_size, tab_level)
 
+    def compare_attrs(self, other: Tag) -> bool:
+        attrs1 = self.attributes
+        attrs2 = other.attributes
+
+        if attrs1.keys() ^ attrs2.keys():
+            return False
+
+        for key in attrs1:
+            if attrs1[key] != attrs2[key]:
+                return False
+
+        return True
+
+    def compare_children(self, other: Tag) -> bool:
+        iter_self = iter(self)
+        iter_other = iter(other)
+
+        # be aware that we can't compare length here because possible
+        # node nesting prevents us from doing so
+
+        for self_child in iter_self:
+            other_child = next(iter_other, None)
+
+            if other_child is None:
+                return False
+
+            if self_child != other_child:
+                return False
+
+        # remaining elements in `other`
+        if next(iter_other, None) is not None:
+            return False
+
+        return True
+
+    def __eq__(self, other: object) -> bool:
+        if not isinstance(other, Tag):
+            return False
+
+        return (
+            (self.tag_name == other.tag_name)
+            and self.compare_attrs(other)
+            and self.compare_children(other)
+        )
+
     def build(self, tab_size: int = 0, tab_level: int = 0) -> Iterable[str]:
         tag_name = self.tag_name
         pretty = bool(tab_size)
 
         tab = " " * tab_size
         tag_indent = " " * (tab_size * tab_level)
         separator = "\n" * pretty
@@ -208,15 +269,15 @@
 
         if self.attributes:
             yield from newline_indented
 
         if self.children or not self.self_closing:
             yield self.brackets[2]  # >
 
-        for child in self.children:
+        for child in self:
             yield separator
             yield from self.build_child(child, tab_size, tab_level + 1)
 
         if self.children:
             yield from newline_indented
 
         if self.children or not self.self_closing:
@@ -272,19 +333,20 @@
 class Fragment(Tag):
     """React-like fragment, renders just its children"""
 
     def __init__(self, *children: Node):
         super().__init__("soda:fragment", *children)
 
     def build(self, tab_size: int = 0, tab_level: int = 0) -> Iterable[str]:
-        for child in self.children:
+        for child in self:
             yield from self.build_child(child, tab_size, tab_level)
 
     def render(self, pretty: bool = False, tab_size: int = 2) -> str:
         sep = "\n" * pretty
         return sep.join(self.build(tab_size * pretty))
 
     def copy(self) -> Fragment:
         return Fragment(*self.children)
 
 
 from .xml_parse import xml_to_tag
+from .utils import escape, node_iterator, normalize_ident, trunc
```

### Comparing `soda_svg-1.1.5/soda/utils.py` & `soda_svg-1.1.7/soda/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Callable, Iterable
 
-from .tags import Node
+from .tags import FlatNode, Fragment, Node
 from .config_mod import config
 
 char_range: Callable[[str, str], "map[str]"] = lambda s, e: map(
     chr, range(ord(s), ord(e) + 1)
 )
 
 ident_chars = {
@@ -38,16 +38,14 @@
     skipped_underscores = 0
     replacement_char = "-" if config.replace_underscores else "_"
 
     for c in attr:
         if c == "_":
             if started:
                 skipped_underscores += 1
-            elif not config.strip_underscores:
-                yield "_"
             continue
         else:
             started = True
 
         yield replacement_char * skipped_underscores
         skipped_underscores = 0
 
@@ -55,15 +53,27 @@
 
     if not config.strip_underscores:
         yield "_" * skipped_underscores
 
 
 def trunc(value: Node) -> Node:
     if isinstance(value, float):
+        if value.is_integer():
+            return int(value)
         return round(value, config.decimal_length)
     return value
 
 
 def eq(v1: float, v2: float) -> bool:
     eps: float = 10 ** -(2 * config.decimal_length)
 
     return abs(v1 - v2) < eps
+
+
+def node_iterator(iterable: Iterable[Node]) -> Iterable[FlatNode]:
+    for elem in iterable:
+        if isinstance(elem, list):
+            yield from node_iterator(elem)
+        elif isinstance(elem, Fragment):
+            yield from elem
+        else:
+            yield elem
```

### Comparing `soda_svg-1.1.5/soda/xml_parse.py` & `soda_svg-1.1.7/soda/xml_parse.py`

 * *Files identical despite different names*

### Comparing `soda_svg-1.1.5/PKG-INFO` & `soda_svg-1.1.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soda-svg
-Version: 1.1.5
+Version: 1.1.7
 Summary: Fast SVG generation tool
 Home-page: https://github.com/evtn/soda
 License: MIT
 Keywords: soda,svg,xml
 Author: Dmitry Gritsenko
 Author-email: soda@evtn.ru
 Requires-Python: >=3.7.0
@@ -225,15 +225,25 @@
 
 tag = Tag.g(Tag.a)
 tag[0]["href"] = "https://github.com/evtn/soda"
 print(tag[1]) # IndexError
 print(tag[0]) # prints <a href="https://github.com/evtn/soda" />
 ```
 
-Children can also be accessed directly through `tag.children` attribute.
+~~Children can also be accessed directly through `tag.children` attribute.~~
+
+This is not necessary for most tasks as of 1.1.6 with new methods and iterator protocol:
+
+- `Tag.insert(int, Node)` inserts a node on an index. Be aware that `tag.children` is not flattened: `Tag.g("test", ["test1", "test2"]).insert(2, elem)` will insert `elem` *after* the array.
+- `Tag.append(Node)` appends one node to the tag.
+- `Tag.extend(*Node)` appends several nodes to the tag. *This is not the same as `.append([*Node])`*
+- `Tag.pop(int?)` pops one node from specified index. If index is not provided, pops the last one.
+- `Tag.iter_raw()` returns an iterable to get every Node of the tag. This doesn't dive into nested arrays, for that behaviour iterate over `Tag`
+- You can also iterate over the `Tag` itself to get every flat node of it (no arrays)
+
 
 ## Fragments
 
 Fragments use concept similar to React's fragment. It renders just it's children:
 
 ```python
 from soda import Tag, Fragment
```

