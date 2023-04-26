# Comparing `tmp/soda_svg-1.1.3.tar.gz` & `tmp/soda_svg-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soda_svg-1.1.3.tar", max compression
+gzip compressed data, was "soda_svg-1.1.5.tar", max compression
```

## Comparing `soda_svg-1.1.3.tar` & `soda_svg-1.1.5.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0     1073 2022-10-31 23:48:13.918161 soda_svg-1.1.3/LICENSE
--rw-r--r--   0        0        0    11200 2022-10-31 23:48:13.922160 soda_svg-1.1.3/README.md
--rw-r--r--   0        0        0      494 2022-10-31 23:48:13.922160 soda_svg-1.1.3/pyproject.toml
--rw-r--r--   0        0        0      173 2022-10-31 23:48:13.922160 soda_svg-1.1.3/soda/__init__.py
--rw-r--r--   0        0        0      123 2022-10-31 23:48:13.922160 soda_svg-1.1.3/soda/config.py
--rw-r--r--   0        0        0     2085 2022-10-31 23:48:13.922160 soda_svg-1.1.3/soda/custom_tags.py
--rw-r--r--   0        0        0     6736 2022-10-31 23:48:13.922160 soda_svg-1.1.3/soda/paths.py
--rw-r--r--   0        0        0    11899 2022-10-31 23:48:13.922160 soda_svg-1.1.3/soda/point.py
--rw-r--r--   0        0        0     7891 2022-10-31 23:48:13.922160 soda_svg-1.1.3/soda/tags.py
--rw-r--r--   0        0        0     1523 2022-10-31 23:48:13.922160 soda_svg-1.1.3/soda/utils.py
--rw-r--r--   0        0        0      924 2022-10-31 23:48:13.922160 soda_svg-1.1.3/soda/xml_parse.py
--rw-r--r--   0        0        0    12281 1970-01-01 00:00:00.000000 soda_svg-1.1.3/setup.py
--rw-r--r--   0        0        0    11889 1970-01-01 00:00:00.000000 soda_svg-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-26 12:02:59.528414 soda_svg-1.1.5/LICENSE
+-rw-r--r--   0        0        0    11021 2023-04-26 12:02:59.528414 soda_svg-1.1.5/README.md
+-rw-r--r--   0        0        0      497 2023-04-26 12:02:59.532413 soda_svg-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0      274 2023-04-26 12:02:59.532413 soda_svg-1.1.5/soda/__init__.py
+-rw-r--r--   0        0        0      123 2023-04-26 12:02:59.532413 soda_svg-1.1.5/soda/config_mod.py
+-rw-r--r--   0        0        0     2081 2023-04-26 12:02:59.532413 soda_svg-1.1.5/soda/custom_tags.py
+-rw-r--r--   0        0        0     7353 2023-04-26 12:02:59.532413 soda_svg-1.1.5/soda/paths.py
+-rw-r--r--   0        0        0    11905 2023-04-26 12:02:59.532413 soda_svg-1.1.5/soda/point.py
+-rw-r--r--   0        0        0     8656 2023-04-26 12:02:59.532413 soda_svg-1.1.5/soda/tags.py
+-rw-r--r--   0        0        0     1551 2023-04-26 12:02:59.532413 soda_svg-1.1.5/soda/utils.py
+-rw-r--r--   0        0        0      924 2023-04-26 12:02:59.532413 soda_svg-1.1.5/soda/xml_parse.py
+-rw-r--r--   0        0        0    11707 1970-01-01 00:00:00.000000 soda_svg-1.1.5/PKG-INFO
```

### Comparing `soda_svg-1.1.3/LICENSE` & `soda_svg-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `soda_svg-1.1.3/README.md` & `soda_svg-1.1.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,17 @@
 )
 
 print(root.render(pretty=True))
 ```
 
 ## Installation
 
-Just use `python setup.py` or `python -m pip install soda-svg`
+Install `soda-svg` from PyPI, like `python -m pip install soda-svg`. 
+
+Note that `soda` on PyPI is a different package.
 
 ## Tag construction
 
 The main class of the module is `Tag`. You can create it with a constructor:
 
 ```python
 Tag("g")
@@ -502,19 +504,13 @@
 
 ## Speed
 
 soda is able to render tens of thousands tags per second, but if you wanna optimize your execution, there are some tips:
 
 ### Building a tree efficiently
 
-If you using the same structure many times (especially if it's a heavy one), avoid rebuilds. Rather than building a new tree every time, consider changing specific parts of it when needed. It won't speed up the render time, though
+If you using the same structure many times (especially if it's a heavy one), avoid rebuilds. Rather than building a new tree every time, consider changing specific parts of it when needed. It won't speed up the render time, though (check Prerendering right below for that)
 
 ### Prerendering
 
 If you have some static tags, you can use `tag.prerender()` to get a prerendered `Literal`.
-This could speed up your render significantly in some cases.
-
-### Pretty or not?
-
-Pretty render gives a nice formatted output, which is very readable.  
-~~But using `pretty=True` in rendering would make renders 3-5x slower than default `pretty=False`.~~  
-Starting with 0.1.5 version, pretty rendering is roughly the same in speed as default one.
+This could speed up your render significantly in some complex cases.
```

### Comparing `soda_svg-1.1.3/soda/custom_tags.py` & `soda_svg-1.1.5/soda/custom_tags.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from base64 import b64encode
 from typing import BinaryIO
-from soda.tags import Node, Tag
+from .tags import Node, Tag
 
 
 class Root(Tag):
     def __init__(
         self, *children: Node, use_namespace: bool = False, **attributes: Node
     ):
         super().__init__("svg", *children, self_closing=False, **attributes)
@@ -25,41 +25,44 @@
 
     def __init__(self, version: str = "1.0", encoding: str = "UTF-8"):
         super().__init__("xml", version=version, encoding=encoding)
 
 
 class Image(Tag):
     """
-    
-    Simple <image> tag wrapper. 
 
-    - Pass a url as a `source`. 
+    Simple <image> tag wrapper.
+
+    - Pass a url as a `source`.
     - To use `xlink:href` along `href` pass `use_xlink=True`
     - To use only `xlink:href`, pass `use_xlink_only=True`
     - To create from file (as base64 dataurl) use `Image.from_file(file_object: BinaryIO, extension: str, **init_kwargs)`
     - ...or `Image.from_filename(filename: str, extension: str, **init_kwargs)`
 
     """
-    def __init__(self, source: str, use_xlink: bool = False, use_xlink_only: bool = False, **attributes: Node):        
+
+    def __init__(
+        self,
+        source: str,
+        use_xlink: bool = False,
+        use_xlink_only: bool = False,
+        **attributes: Node,
+    ):
         super().__init__("image")
         if not use_xlink_only:
             self.set_attribute("href", source)
 
         if use_xlink or use_xlink_only:
             self.set_attribute("xlink:href", source)
 
         self(**attributes)
 
-
     @staticmethod
     def from_file(file_object: BinaryIO, extension: str, **init_kwargs: bool) -> Image:
-        contents: str = b64encode(file_object.read()).decode('ascii')
+        contents: str = b64encode(file_object.read()).decode("ascii")
 
-        return Image(
-            f"data:image/{extension};base64,{contents}",
-            **init_kwargs
-        )
+        return Image(f"data:image/{extension};base64,{contents}", **init_kwargs)
 
     @staticmethod
     def from_filename(filename: str, extension: str, **init_kwargs: bool) -> Image:
         with open(filename, "rb") as file:
-            return Image.from_file(file, extension, **init_kwargs)
+            return Image.from_file(file, extension, **init_kwargs)
```

### Comparing `soda_svg-1.1.3/soda/paths.py` & `soda_svg-1.1.5/soda/paths.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,81 +1,69 @@
 from __future__ import annotations
-from soda.utils import trunc
+from .utils import trunc
+
 
 def value_to_str(value: object) -> str:
     if isinstance(value, float):
         return str(trunc(value))
     return str(value)
 
+
 class Path:
     @staticmethod
     def build(*commands: str, compact: bool = False) -> str:
         if compact:
             return compact_path(" ".join(commands).split(" "))
         return " ".join(commands)
 
     # M x y
     @staticmethod
-    def moveto(
-        x: float = 0, 
-        y: float = 0, 
-        *, relative: bool = False
-    ) -> str:
+    def moveto(x: float = 0, y: float = 0, *, relative: bool = False) -> str:
         prefix = "Mm"[relative]
         return " ".join(map(value_to_str, [prefix, x, y]))
 
     @staticmethod
     def M(x: float, y: float) -> str:
         return Path.moveto(x, y, relative=False)
 
     @staticmethod
     def m(x: float, y: float) -> str:
         return Path.moveto(x, y, relative=True)
 
     # L x y
     @staticmethod
-    def line(
-        x: float = 0, 
-        y: float = 0, 
-        *, relative: bool = False
-    ) -> str:
+    def line(x: float = 0, y: float = 0, *, relative: bool = False) -> str:
         prefix = "Ll"[relative]
         return " ".join(map(value_to_str, [prefix, x, y]))
 
     @staticmethod
     def L(x: float, y: float) -> str:
         return Path.line(x, y, relative=False)
 
     @staticmethod
     def l(x: float, y: float) -> str:
         return Path.line(x, y, relative=True)
 
     # V y
     @staticmethod
-    def vertical(
-        y: float = 0, 
-        *, relative: bool = False
-    ) -> str:
+    def vertical(y: float = 0, *, relative: bool = False) -> str:
         prefix = "Vv"[relative]
         return " ".join(map(value_to_str, [prefix, y]))
 
     @staticmethod
     def V(y: float) -> str:
         return Path.vertical(y, relative=False)
 
     @staticmethod
     def v(y: float) -> str:
         return Path.vertical(y, relative=True)
 
     # H x
     @staticmethod
-    def horizontal(
-        x: float = 0, 
-        *, relative: bool = False
-    ) -> str:
+    def horizontal(x: float = 0, *, relative: bool = False) -> str:
         prefix = "Hh"[relative]
         return " ".join(map(value_to_str, [prefix, x]))
 
     @staticmethod
     def H(x: float) -> str:
         return Path.vertical(x, relative=False)
 
@@ -95,43 +83,80 @@
 
     @staticmethod
     def z() -> str:
         return Path.close(relative=True)
 
     # C x1 y1 x2 y2 x y
     @staticmethod
-    def cubic(x1: float = 0, y1: float = 0, x2: float = 0, y2: float = 0, x: float = 0, y: float = 0, *, relative: bool = False) -> str:
+    def cubic(
+        x1: float = 0,
+        y1: float = 0,
+        x2: float = 0,
+        y2: float = 0,
+        x: float = 0,
+        y: float = 0,
+        *,
+        relative: bool = False,
+    ) -> str:
         prefix = "Cc"[relative]
         return " ".join(map(value_to_str, [prefix, x1, y1, x2, y2, x, y]))
 
     @staticmethod
-    def C(x1: float = 0, y1: float = 0, x2: float = 0, y2: float = 0, x: float = 0, y: float = 0) -> str:
+    def C(
+        x1: float = 0,
+        y1: float = 0,
+        x2: float = 0,
+        y2: float = 0,
+        x: float = 0,
+        y: float = 0,
+    ) -> str:
         return Path.cubic(x1, y1, x2, y2, x, y, relative=False)
 
     @staticmethod
-    def c(x1: float = 0, y1: float = 0, x2: float = 0, y2: float = 0, x: float = 0, y: float = 0) -> str:
+    def c(
+        x1: float = 0,
+        y1: float = 0,
+        x2: float = 0,
+        y2: float = 0,
+        x: float = 0,
+        y: float = 0,
+    ) -> str:
         return Path.cubic(x1, y1, x2, y2, x, y, relative=True)
 
     # S x2 y2, x y
     @staticmethod
-    def shorthand(x2: float = 0, y2: float = 0, x: float = 0, y: float = 0, *, relative: bool = False) -> str:
+    def shorthand(
+        x2: float = 0,
+        y2: float = 0,
+        x: float = 0,
+        y: float = 0,
+        *,
+        relative: bool = False,
+    ) -> str:
         prefix = "Ss"[relative]
         return " ".join(map(value_to_str, [prefix, x2, y2, x, y]))
 
     @staticmethod
     def S(x2: float = 0, y2: float = 0, x: float = 0, y: float = 0) -> str:
         return Path.shorthand(x2, y2, x, y, relative=False)
 
     @staticmethod
     def s(x2: float = 0, y2: float = 0, x: float = 0, y: float = 0) -> str:
         return Path.shorthand(x2, y2, x, y, relative=True)
 
     # Q x1 y1 x y
     @staticmethod
-    def quadratic(x1: float = 0, y1: float = 0, x: float = 0, y: float = 0, *, relative: bool = False) -> str:
+    def quadratic(
+        x1: float = 0,
+        y1: float = 0,
+        x: float = 0,
+        y: float = 0,
+        *,
+        relative: bool = False,
+    ) -> str:
         prefix = "Qq"[relative]
         return " ".join(map(value_to_str, [prefix, x1, y1, x, y]))
 
     @staticmethod
     def Q(x1: float = 0, y1: float = 0, x: float = 0, y: float = 0) -> str:
         return Path.quadratic(x1, y1, x, y, relative=False)
 
@@ -152,68 +177,101 @@
     @staticmethod
     def t(x: float = 0, y: float = 0) -> str:
         return Path.q_shorthand(x, y, relative=True)
 
     # A rx ry x-axis-rotation large-arc-flag sweep-flag x y
     @staticmethod
     def arc(
-        radius_x: float = 0, 
-        radius_y: float = 0, 
-        x_axis_rotation: float = 0, 
-        large_arc_flag: bool | int = 0, 
-        sweep_flag: bool | int = 0, 
-        x: float = 0, 
-        y: float = 0, 
-        *, relative: bool = False
+        radius_x: float = 0,
+        radius_y: float = 0,
+        x_axis_rotation: float = 0,
+        large_arc_flag: bool | int = 0,
+        sweep_flag: bool | int = 0,
+        x: float = 0,
+        y: float = 0,
+        *,
+        relative: bool = False,
     ) -> str:
-        prefix = "Aa"[relative] 
-        return " ".join(map(value_to_str, [prefix, radius_x, radius_y, x_axis_rotation, int(large_arc_flag) & 1, int(sweep_flag) & 1, x, y]))
+        prefix = "Aa"[relative]
+        return " ".join(
+            map(
+                value_to_str,
+                [
+                    prefix,
+                    radius_x,
+                    radius_y,
+                    x_axis_rotation,
+                    int(large_arc_flag) & 1,
+                    int(sweep_flag) & 1,
+                    x,
+                    y,
+                ],
+            )
+        )
 
     @staticmethod
     def A(
-        radius_x: float = 0, 
-        radius_y: float = 0, 
-        x_axis_rotation: float = 0, 
-        large_arc_flag: bool | int = 0, 
-        sweep_flag: bool | int = 0, 
-        x: float = 0, 
-        y: float = 0, 
+        radius_x: float = 0,
+        radius_y: float = 0,
+        x_axis_rotation: float = 0,
+        large_arc_flag: bool | int = 0,
+        sweep_flag: bool | int = 0,
+        x: float = 0,
+        y: float = 0,
     ) -> str:
-        return Path.arc(radius_x, radius_y, x_axis_rotation, large_arc_flag, sweep_flag, x, y, relative=False)
+        return Path.arc(
+            radius_x,
+            radius_y,
+            x_axis_rotation,
+            large_arc_flag,
+            sweep_flag,
+            x,
+            y,
+            relative=False,
+        )
 
     @staticmethod
     def a(
-        radius_x: float = 0, 
-        radius_y: float = 0, 
-        x_axis_rotation: float = 0, 
-        large_arc_flag: bool | int = 0, 
-        sweep_flag: bool | int = 0, 
-        x: float = 0, 
-        y: float = 0, 
+        radius_x: float = 0,
+        radius_y: float = 0,
+        x_axis_rotation: float = 0,
+        large_arc_flag: bool | int = 0,
+        sweep_flag: bool | int = 0,
+        x: float = 0,
+        y: float = 0,
     ) -> str:
-        return Path.arc(radius_x, radius_y, x_axis_rotation, large_arc_flag, sweep_flag, x, y, relative=True)
+        return Path.arc(
+            radius_x,
+            radius_y,
+            x_axis_rotation,
+            large_arc_flag,
+            sweep_flag,
+            x,
+            y,
+            relative=True,
+        )
 
 
 def compact_path(path: list[str]) -> str:
     result: list[str] = []
     digits = set("0123456789")
-    
+
     for part in path:
         if not result:
             result.append(part)
             continue
 
         if part.isalpha():
             result.append(part)
             continue
 
         is_negative = part[0] == "-"
 
         part = part.lstrip("-").lstrip("0")
-        
+
         if not part:
             is_negative = False
             part = "0"
 
         if is_negative:
             result.append("-")
             result.append(part)
@@ -225,8 +283,8 @@
             if "." not in result[-1]:
                 result.append(" ")
         elif result[-1][-1] in digits:
             result.append(" ")
 
         result.append(part)
 
-    return "".join(result)
+    return "".join(result)
```

### Comparing `soda_svg-1.1.3/soda/point.py` & `soda_svg-1.1.5/soda/point.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 from typing import Iterator, Sequence, Union, overload
 from math import pi, cos, sin, hypot, acos
 
-from soda.paths import Path, compact_path
-from soda.tags import Node, Tag
-
+from .utils import eq
+from .paths import Path, compact_path
+from .tags import Node, Tag
 
 PointLike = Union["Point", float, Sequence[float]]
 
 rad_to_deg_k = 180 / pi
 
 
 def radians_to_degrees(radians: float) -> float:
@@ -27,15 +27,15 @@
 
     @staticmethod
     def from_(value: PointLike = 0) -> Point:
         if isinstance(value, Point):
             return value
         if isinstance(value, (float, int)):
             return Point(value, value)
-        return Point(*value[:2])
+        return Point(*map(float, value[:2]))
 
     def __add__(self, other: PointLike = 0) -> Point:
         other = Point.from_(other)
         return Point(self.x + other.x, self.y + other.y)
 
     def __radd__(self, other: PointLike = 0) -> Point:
         return self + other
@@ -61,16 +61,16 @@
     def __rtruediv__(self, other: PointLike = 0) -> Point:
         return Point.from_(other) / self
 
     def __pow__(self, other: PointLike = 0) -> Point:
         other = Point.from_(other)
 
         # this is due to the fact that float.__pow__(float) is suddenly Any (not float, not complex | float, etc.)
-        new_x: float = self.x ** other.x
-        new_y: float = self.y ** other.y
+        new_x: float = self.x**other.x
+        new_y: float = self.y**other.y
 
         assert isinstance(new_x, (float, int))
         assert isinstance(new_y, (float, int))
 
         return Point(new_x, new_y)
 
     def __rpow__(self, other: PointLike = 0) -> Point:
@@ -96,23 +96,35 @@
             round(self.y, ndigits),
         )
 
     def __iter__(self) -> Iterator[float]:
         return iter(self.coords)
 
     @overload
-    def rotate(self, center: PointLike = 0, *, degrees: float, radians: None = None) -> Point:
+    def rotate(
+        self, center: PointLike = 0, *, degrees: float, radians: None = None
+    ) -> Point:
         ...
 
     @overload
-    def rotate(self, center: PointLike = 0, *, degrees: None = None, radians: float) -> Point:
+    def rotate(
+        self, center: PointLike = 0, *, degrees: None = None, radians: float
+    ) -> Point:
         ...
 
-    def rotate(self, center: PointLike = 0, *, degrees: float | None = None, radians: float | None = None) -> Point:
-        error = ValueError("Either degrees or radians should be provided, not both nor neither")
+    def rotate(
+        self,
+        center: PointLike = 0,
+        *,
+        degrees: float | None = None,
+        radians: float | None = None,
+    ) -> Point:
+        error = ValueError(
+            "Either degrees or radians should be provided, not both nor neither"
+        )
         center = Point.from_(center)
 
         if radians is None:
             if degrees is None:
                 raise error
             radians = degrees_to_radians(degrees)
         elif degrees is not None:
@@ -127,15 +139,15 @@
         y = sin_vec.x + cos_vec.y
 
         return Point(x, y) + center
 
     def distance(self, other: PointLike = 0) -> float:
         return hypot(*(self - other))
 
-    def __str__(self) -> str:
+    def __repr__(self) -> str:
         return f"Point[{self.x}, {self.y}]"
 
     def as_(self, x_argname: str = "x", y_argname: str = "y") -> dict[str, float]:
         return {x_argname: self.x, y_argname: self.y}
 
     def angle(self, other: PointLike = (1, 0), center: PointLike = 0) -> float:
         center = Point.from_(center)
@@ -144,101 +156,80 @@
 
         dot_product = sum(self * other)
         distance_product = self.distance() * other.distance()
 
         if distance_product == 0:
             return 0
 
-        return acos(
-            dot_product / distance_product
-        )
+        return acos(dot_product / distance_product)
 
     def normalized(self) -> Point:
         return self / self.distance()
 
+    def __eq__(self, other: object) -> bool:
+        if not isinstance(other, (Point, float, list, tuple)):
+            return False
+        other = Point.from_(other)
+        return eq((self - other).distance(), 0)
+
+
 class PointPath:
     @staticmethod
     def build(*commands: str, compact: bool = False) -> str:
         if compact:
             return compact_path(" ".join(commands).split(" "))
         return " ".join(commands)
 
     # M x y
     @staticmethod
-    def moveto(
-        point: PointLike = 0,
-        *, relative: bool = False
-    ) -> str:
+    def moveto(point: PointLike = 0, *, relative: bool = False) -> str:
         point = Point.from_(point)
-        return Path.moveto(
-            point.x,
-            point.y, 
-            relative=relative
-        )
+        return Path.moveto(point.x, point.y, relative=relative)
 
     @staticmethod
     def M(point: PointLike = 0) -> str:
         return PointPath.moveto(point, relative=False)
 
     @staticmethod
     def m(point: PointLike = 0) -> str:
         return PointPath.moveto(point, relative=True)
 
     # L x y
     @staticmethod
-    def line(
-        point: PointLike = 0, 
-        *, relative: bool = False
-    ) -> str:
+    def line(point: PointLike = 0, *, relative: bool = False) -> str:
         point = Point.from_(point)
-        return Path.line(
-            point.x,
-            point.y,
-            relative=relative
-        )
+        return Path.line(point.x, point.y, relative=relative)
 
     @staticmethod
     def L(point: PointLike = 0) -> str:
         return PointPath.line(point, relative=False)
 
     @staticmethod
     def l(point: PointLike = 0) -> str:
         return PointPath.line(point, relative=True)
 
     # V y
     @staticmethod
-    def vertical(
-        point: PointLike = 0,
-        *, relative: bool = False
-    ) -> str:
+    def vertical(point: PointLike = 0, *, relative: bool = False) -> str:
         point = Point.from_(point)
-        return Path.vertical(
-            point.y,
-            relative=relative
-        )
+        return Path.vertical(point.y, relative=relative)
 
     @staticmethod
-    def V(y: float) -> str:
-        return PointPath.vertical(y, relative=False)
+    def V(point: PointLike = 0) -> str:
+        return PointPath.vertical(point, relative=False)
 
     @staticmethod
-    def v(y: float) -> str:
-        return PointPath.vertical(y, relative=True)
+    def v(point: PointLike = 0) -> str:
+        return PointPath.vertical(point, relative=True)
 
     # H x
     @staticmethod
-    def horizontal(
-        point: PointLike = 0,
-        *, relative: bool = False
-    ) -> str:
+    def horizontal(point: PointLike = 0, *, relative: bool = False) -> str:
         point = Point.from_(point)
-        return Path.horizontal(
-            point.x,
-            relative=relative
-        )
+        return Path.horizontal(point.x, relative=relative)
 
     @staticmethod
     def H(point: PointLike = 0) -> str:
         return PointPath.vertical(point, relative=False)
 
     @staticmethod
     def h(point: PointLike = 0) -> str:
@@ -255,155 +246,154 @@
 
     @staticmethod
     def z() -> str:
         return PointPath.close(relative=True)
 
     # C x1 y1 x2 y2 x y
     @staticmethod
-    def cubic(first_control: PointLike = 0, second_control: PointLike = 0, end: PointLike = 0, *, relative: bool = False) -> str:
+    def cubic(
+        first_control: PointLike = 0,
+        second_control: PointLike = 0,
+        end: PointLike = 0,
+        *,
+        relative: bool = False,
+    ) -> str:
         first_control = Point.from_(first_control)
         second_control = Point.from_(second_control)
         end = Point.from_(end)
         return Path.cubic(
             first_control.x,
             first_control.y,
             second_control.x,
             second_control.y,
             end.x,
             end.y,
-            relative=relative
+            relative=relative,
         )
 
     @staticmethod
-    def C(first_control: PointLike = 0, second_control: PointLike = 0, end: PointLike = 0) -> str:
+    def C(
+        first_control: PointLike = 0, second_control: PointLike = 0, end: PointLike = 0
+    ) -> str:
         return PointPath.cubic(first_control, second_control, end, relative=False)
 
     @staticmethod
-    def c(first_control: PointLike = 0, second_control: PointLike = 0, end: PointLike = 0) -> str:
+    def c(
+        first_control: PointLike = 0, second_control: PointLike = 0, end: PointLike = 0
+    ) -> str:
         return PointPath.cubic(first_control, second_control, end, relative=True)
 
     # S x2 y2, x y
     @staticmethod
-    def shorthand(second_control: PointLike = 0, end: PointLike = 0, *, relative: bool = False) -> str:
+    def shorthand(
+        second_control: PointLike = 0, end: PointLike = 0, *, relative: bool = False
+    ) -> str:
         second_control = Point.from_(second_control)
         end = Point.from_(end)
         return Path.shorthand(
-            second_control.x,
-            second_control.y,
-            end.x,
-            end.y,
-            relative=relative
+            second_control.x, second_control.y, end.x, end.y, relative=relative
         )
 
     @staticmethod
     def S(second_control: PointLike = 0, end: PointLike = 0) -> str:
         return PointPath.shorthand(second_control, end, relative=False)
 
     @staticmethod
     def s(second_control: PointLike = 0, end: PointLike = 0) -> str:
         return PointPath.shorthand(second_control, end, relative=True)
 
     # Q x1 y1 x y
     @staticmethod
-    def quadratic(control: PointLike = 0, end: PointLike = 0, *, relative: bool = False) -> str:
+    def quadratic(
+        control: PointLike = 0, end: PointLike = 0, *, relative: bool = False
+    ) -> str:
         control = Point.from_(control)
         end = Point.from_(end)
-        return Path.quadratic(
-            control.x,
-            control.y,
-            end.x,
-            end.y,
-            relative=relative
-        )
+        return Path.quadratic(control.x, control.y, end.x, end.y, relative=relative)
 
     @staticmethod
     def Q(control: PointLike = 0, end: PointLike = 0) -> str:
         return PointPath.quadratic(control, end, relative=False)
 
     @staticmethod
     def q(control: PointLike = 0, end: PointLike = 0) -> str:
         return PointPath.quadratic(control, end, relative=True)
 
     # T x y
     @staticmethod
     def q_shorthand(end: PointLike = 0, *, relative: bool = False) -> str:
         end = Point.from_(end)
-        return Path.q_shorthand(
-            end.x,
-            end.y,
-            relative=relative
-        )
+        return Path.q_shorthand(end.x, end.y, relative=relative)
 
     @staticmethod
     def T(end: PointLike = 0) -> str:
         return PointPath.q_shorthand(end, relative=False)
 
     @staticmethod
     def t(end: PointLike = 0) -> str:
         return PointPath.q_shorthand(end, relative=True)
 
     # A rx ry x-axis-rotation large-arc-flag sweep-flag x y
     @staticmethod
     def arc(
-        radius: PointLike = 0, 
-        x_axis_rotation: float = 0, 
-        large_arc_flag: bool | int = 0, 
-        sweep_flag: bool | int = 0, 
-        end: PointLike = 0, 
-        *, relative: bool = False
+        radius: PointLike = 0,
+        x_axis_rotation: float = 0,
+        large_arc_flag: bool | int = 0,
+        sweep_flag: bool | int = 0,
+        end: PointLike = 0,
+        *,
+        relative: bool = False,
     ) -> str:
         radius = Point.from_(radius)
         end = Point.from_(end)
         return Path.arc(
             radius.x,
             radius.y,
             x_axis_rotation,
-            large_arc_flag, 
-            sweep_flag, 
+            large_arc_flag,
+            sweep_flag,
             end.x,
             end.y,
-            relative=relative 
+            relative=relative,
         )
 
     @staticmethod
     def A(
-        radius: PointLike = 0, 
-        x_axis_rotation: float = 0, 
-        large_arc_flag: bool | int = 0, 
-        sweep_flag: bool | int = 0, 
-        end: PointLike = 0, 
+        radius: PointLike = 0,
+        x_axis_rotation: float = 0,
+        large_arc_flag: bool | int = 0,
+        sweep_flag: bool | int = 0,
+        end: PointLike = 0,
     ) -> str:
-        return PointPath.arc(radius, x_axis_rotation, large_arc_flag, sweep_flag, end, relative=False)
+        return PointPath.arc(
+            radius, x_axis_rotation, large_arc_flag, sweep_flag, end, relative=False
+        )
 
     @staticmethod
     def a(
-        radius: PointLike = 0, 
-        x_axis_rotation: float = 0, 
-        large_arc_flag: bool | int = 0, 
-        sweep_flag: bool | int = 0, 
-        end: PointLike = 0, 
+        radius: PointLike = 0,
+        x_axis_rotation: float = 0,
+        large_arc_flag: bool | int = 0,
+        sweep_flag: bool | int = 0,
+        end: PointLike = 0,
     ) -> str:
-        return PointPath.arc(radius, x_axis_rotation, large_arc_flag, sweep_flag, end, relative=True)
+        return PointPath.arc(
+            radius, x_axis_rotation, large_arc_flag, sweep_flag, end, relative=True
+        )
 
     @staticmethod
     def polygon(*points: Point, **attributes: Node) -> Tag:
         commands = [
             PointPath.line(point) if i else PointPath.moveto(point)
             for i, point in enumerate(points)
         ]
 
-        return Tag.path(
-            d=PointPath.build(*commands, PointPath.close()),
-            **attributes
-        )
+        return Tag.path(d=PointPath.build(*commands, PointPath.close()), **attributes)
 
     @staticmethod
     def polyline(*points: Point, **attributes: Node) -> Tag:
         commands = [
             PointPath.line(point) if i else PointPath.moveto(point)
             for i, point in enumerate(points)
         ]
 
-        return Tag.path(
-            d=PointPath.build(*commands),
-            **attributes
-        )
+        return Tag.path(d=PointPath.build(*commands), **attributes)
```

### Comparing `soda_svg-1.1.3/soda/tags.py` & `soda_svg-1.1.5/soda/tags.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,40 @@
 from __future__ import annotations
-from typing import Iterable, Optional, Type, Union, cast, overload
+from typing import Iterable, Optional, Union, overload
 
 
 Node = Union["Tag", str, float, "list[Node]"]
 
 
 from .utils import escape, normalize_ident, trunc
 
 
 class MetaTag(type):
     def __getattr__(self, tag_name: str) -> Tag:
         return Tag(tag_name)
 
 
 class Tag(metaclass=MetaTag):
+    """
+
+    Main class of the module, used to create tags.
+
+    To create a simple `<tagname>` tag, use a shorthand: `Tag.tagname`.
+
+    You can then call it to mutate its contents:
+
+    - `Tag.tagname(child1, child2)` adds two children nodes (could be tags or text-like values: strings/numbers, or a list of nodes)
+    - `Tag.tagname(child1, child2, a=1, b=2)` same as above, but sets `a` attribute to `1`, `b` to 2. Attribute types could be the same as with nodes.
+
+    To set contents in one call and/or manage self-closing behaviour, use Tag constructor:
+
+    `Tag(tag_name: str, *children: Node, self_closing: bool = True, **attributes: Node)`
+
+    """
+
     tag_name: str
     children: list[Node]
     attributes: dict[str, Node]
     self_closing: bool
     brackets: list[str] = ["<", "</", ">", "/>"]
     key_value_sep: str = "="
 
@@ -32,25 +49,33 @@
         self.children = list(children)
         self.attributes = {}
         for k in attributes:
             self[k] = attributes[k]
         self.self_closing = self_closing
 
     def copy(self) -> Tag:
-        return Tag(self.tag_name, *self.children, self_closing=self.self_closing, **self.attributes)
+        return Tag(
+            self.tag_name,
+            *self.children,
+            self_closing=self.self_closing,
+            **self.attributes,
+        )
 
     @overload
     def set_attribute(self, attr: str, value: None) -> None:
         ...
+
     @overload
     def set_attribute(self, attr: str, value: Node) -> Node:
         ...
+
     @overload
     def set_attribute(self, attr: str, value: Node | None) -> Node | None:
         ...
+
     def set_attribute(self, attr: str, value: Optional[Node]) -> Optional[Node]:
         """sets tag attribute to value. If None is passed, deletes attribute"""
         attr = normalize_ident(attr)
         if value is None:
             if attr in self.attributes:
                 self.attributes.pop(attr)
         else:
@@ -60,24 +85,31 @@
     def get_attribute(self, attr: str) -> Optional[Node]:
         """returns tag attribute or None"""
         return self.attributes.get(normalize_ident(attr))
 
     @overload
     def __setitem__(self, item: str | int | slice, value: Node) -> Node:
         ...
+
     @overload
     def __setitem__(self, item: str | int | slice, value: None) -> None:
         ...
+
     @overload
-    def __setitem__(self, item: str | int | slice, value: Optional[Node]) -> Optional[Node]:
+    def __setitem__(
+        self, item: str | int | slice, value: Optional[Node]
+    ) -> Optional[Node]:
         ...
-    def __setitem__(self, item: str | int | slice, value: Optional[Node]) -> Optional[Node]:
+
+    def __setitem__(
+        self, item: str | int | slice, value: Optional[Node]
+    ) -> Optional[Node]:
         # slice is basically slice[Any, Any, Any] and https://github.com/python/typeshed/issues/8647 looks dead
         # after an hour of thinking and three broken keyboards I've decided to do this:
-        if isinstance(item, slice): # type: ignore[misc]
+        if isinstance(item, slice):  # type: ignore[misc]
             if value is None:
                 value = []
             elif not isinstance(value, list):
                 value = [value]
             self.children[item] = value
             return value
         elif isinstance(item, int):
@@ -87,25 +119,28 @@
             return value
 
         return self.set_attribute(item, value)
 
     @overload
     def __getitem__(self, item: int) -> Node:
         ...
+
     @overload
     def __getitem__(self, item: slice) -> list[Node]:
         ...
+
     @overload
     def __getitem__(self, item: str) -> Node:
         ...
+
     def __getitem__(
         self, item: Union[str, int, slice]
     ) -> Optional[Union[Node, list[Node], Node]]:
         # check __setitem__ for explanation of ignore
-        if isinstance(item, (int, slice)): # type: ignore[misc]
+        if isinstance(item, (int, slice)):  # type: ignore[misc]
             return self.children[item]
 
         return self.get_attribute(item)
 
     def __call__(self, *children: Node, **attributes: Node) -> Tag:
         if children:
             self.children.extend(children)
@@ -116,24 +151,28 @@
 
     def __repr__(self) -> str:
         return f"Tag<{self.tag_name} attributes: {len(self.attributes)}>children: {len(self.children)}</{self.tag_name}>"
 
     def __str__(self) -> str:
         return self.render()
 
-    def build_child(self, child: Node, tab_size: int = 0, tab_level: int = 0) -> Iterable[str]:
+    def build_child(
+        self, child: Node, tab_size: int = 0, tab_level: int = 0
+    ) -> Iterable[str]:
         if isinstance(child, (float, int)):
             return self.build_child(str(trunc(child)), tab_size, tab_level)
-        
+
         if isinstance(child, str):
             yield " " * (tab_size * tab_level)
             yield escape(child)
+
         elif isinstance(child, list):
             for subchild in child:
                 yield from self.build_child(subchild, tab_size, tab_level)
+
         else:
             yield from child.build(tab_size, tab_level)
 
     def build(self, tab_size: int = 0, tab_level: int = 0) -> Iterable[str]:
         tag_name = self.tag_name
         pretty = bool(tab_size)
 
@@ -145,57 +184,57 @@
 
         attr_separator = [attr_space, tag_indent, tab]
         newline_indented = [separator, tag_indent]
 
         if tab_size:
             yield tag_indent
 
-        yield self.brackets[0] # <
+        yield self.brackets[0]  # <
         yield tag_name
 
         for key in self.attributes:
             yield from attr_separator
             yield str(key)
-            yield self.key_value_sep
+            yield self.key_value_sep  # =
             yield quote
 
             value = self.attributes[key]
             if isinstance(value, Tag):
                 value = value.render()
             else:
                 value = str(value)
 
-            yield value.replace(quote, '&quot;')
+            yield value.replace(quote, "&quot;")
             yield quote
-        
+
         if self.attributes:
             yield from newline_indented
 
         if self.children or not self.self_closing:
-            yield self.brackets[2]
+            yield self.brackets[2]  # >
 
         for child in self.children:
             yield separator
             yield from self.build_child(child, tab_size, tab_level + 1)
 
         if self.children:
             yield from newline_indented
 
         if self.children or not self.self_closing:
-            yield self.brackets[1] # </
+            yield self.brackets[1]  # </
             yield tag_name
-            yield self.brackets[2] # >
+            yield self.brackets[2]  # >
         else:
-            yield self.brackets[3] # />
+            yield self.brackets[3]  # />
 
     def render(self, pretty: bool = False, tab_size: int = 2) -> str:
         return "".join(self.build(tab_size * pretty))
 
     def prerender(self, pretty: bool = False) -> Literal:
-        """Renders a tag into a non-escaping literal. Could be useful for heavy tags."""
+        """Renders a tag into a non-escaping literal. Could speed up rendering of heavy tags."""
         return Literal(self.render(pretty), escape=False)
 
     @staticmethod
     def from_str(text: str) -> Tag:
         return xml_to_tag(text)
 
 
@@ -244,8 +283,8 @@
         sep = "\n" * pretty
         return sep.join(self.build(tab_size * pretty))
 
     def copy(self) -> Fragment:
         return Fragment(*self.children)
 
 
-from soda.xml_parse import xml_to_tag
+from .xml_parse import xml_to_tag
```

### Comparing `soda_svg-1.1.3/soda/utils.py` & `soda_svg-1.1.5/soda/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,36 @@
 from typing import Callable, Iterable
 
 from .tags import Node
-from .config import config
+from .config_mod import config
 
 char_range: Callable[[str, str], "map[str]"] = lambda s, e: map(
-    chr, 
-    range(
-        ord(s), 
-        ord(e) + 1
-    )
+    chr, range(ord(s), ord(e) + 1)
 )
 
 ident_chars = {
     *char_range("a", "z"),
     *char_range("A", "Z"),
     *char_range("0", "9"),
     "-",
     "_",
-    ":"
+    ":",
 }
 
 
 def escape(text: str) -> str:
     return text.replace("&", "&amp;").replace(">", "&gt;").replace("<", "&lt;")
 
 
 def filter_ident_func(char: str) -> bool:
-    return (
-        char in ident_chars
-    )
+    return char in ident_chars
 
 
 def filter_ident(text: Iterable[str]) -> str:
-    return "".join(
-        filter(
-            filter_ident_func,
-            text 
-        )
-    )
+    return "".join(filter(filter_ident_func, text))
 
 
 def normalize_ident(attr: str) -> str:
     return filter_ident(normalize_ident_gen(attr))
 
 
 def normalize_ident_gen(attr: str) -> Iterable[str]:
@@ -54,21 +43,27 @@
             if started:
                 skipped_underscores += 1
             elif not config.strip_underscores:
                 yield "_"
             continue
         else:
             started = True
-        
+
         yield replacement_char * skipped_underscores
         skipped_underscores = 0
 
         yield c
 
     if not config.strip_underscores:
         yield "_" * skipped_underscores
 
 
 def trunc(value: Node) -> Node:
     if isinstance(value, float):
         return round(value, config.decimal_length)
-    return value
+    return value
+
+
+def eq(v1: float, v2: float) -> bool:
+    eps: float = 10 ** -(2 * config.decimal_length)
+
+    return abs(v1 - v2) < eps
```

### Comparing `soda_svg-1.1.3/soda/xml_parse.py` & `soda_svg-1.1.5/soda/xml_parse.py`

 * *Files identical despite different names*

### Comparing `soda_svg-1.1.3/PKG-INFO` & `soda_svg-1.1.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: soda-svg
-Version: 1.1.3
+Version: 1.1.5
 Summary: Fast SVG generation tool
 Home-page: https://github.com/evtn/soda
 License: MIT
 Keywords: soda,svg,xml
 Author: Dmitry Gritsenko
 Author-email: soda@evtn.ru
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.7.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -32,15 +32,17 @@
 )
 
 print(root.render(pretty=True))
 ```
 
 ## Installation
 
-Just use `python setup.py` or `python -m pip install soda-svg`
+Install `soda-svg` from PyPI, like `python -m pip install soda-svg`. 
+
+Note that `soda` on PyPI is a different package.
 
 ## Tag construction
 
 The main class of the module is `Tag`. You can create it with a constructor:
 
 ```python
 Tag("g")
@@ -522,20 +524,14 @@
 
 ## Speed
 
 soda is able to render tens of thousands tags per second, but if you wanna optimize your execution, there are some tips:
 
 ### Building a tree efficiently
 
-If you using the same structure many times (especially if it's a heavy one), avoid rebuilds. Rather than building a new tree every time, consider changing specific parts of it when needed. It won't speed up the render time, though
+If you using the same structure many times (especially if it's a heavy one), avoid rebuilds. Rather than building a new tree every time, consider changing specific parts of it when needed. It won't speed up the render time, though (check Prerendering right below for that)
 
 ### Prerendering
 
 If you have some static tags, you can use `tag.prerender()` to get a prerendered `Literal`.
-This could speed up your render significantly in some cases.
-
-### Pretty or not?
-
-Pretty render gives a nice formatted output, which is very readable.  
-~~But using `pretty=True` in rendering would make renders 3-5x slower than default `pretty=False`.~~  
-Starting with 0.1.5 version, pretty rendering is roughly the same in speed as default one.
+This could speed up your render significantly in some complex cases.
```

