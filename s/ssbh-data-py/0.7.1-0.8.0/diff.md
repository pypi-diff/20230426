# Comparing `tmp/ssbh_data_py-0.7.1-cp39-none-win_amd64.whl.zip` & `tmp/ssbh_data_py-0.8.0-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 881264 bytes, number of entries: 14
--rw-r--r--  4.6 unx       78 b- defN 22-Oct-24 03:40 ssbh_data_py-0.7.1.dist-info/METADATA
--rw-r--r--  4.6 unx       95 b- defN 22-Oct-24 03:40 ssbh_data_py-0.7.1.dist-info/WHEEL
--rw-r--r--  4.6 unx      670 b- defN 22-Oct-24 03:40 ssbh_data_py/adj_data.pyi
--rw-r--r--  4.6 unx     2589 b- defN 22-Oct-24 03:40 ssbh_data_py/anim_data.pyi
--rw-r--r--  4.6 unx     2175 b- defN 22-Oct-24 03:40 ssbh_data_py/hlpb_data.pyi
--rw-r--r--  4.6 unx    20261 b- defN 22-Oct-24 03:40 ssbh_data_py/matl_data.pyi
--rw-r--r--  4.6 unx     1028 b- defN 22-Oct-24 03:40 ssbh_data_py/meshex_data.pyi
--rw-r--r--  4.6 unx     2708 b- defN 22-Oct-24 03:40 ssbh_data_py/mesh_data.pyi
--rw-r--r--  4.6 unx      892 b- defN 22-Oct-24 03:40 ssbh_data_py/modl_data.pyi
--rw-r--r--  4.6 unx     1642 b- defN 22-Oct-24 03:40 ssbh_data_py/skel_data.pyi
--rw-r--r--  4.6 unx       27 b- defN 22-Oct-24 03:40 ssbh_data_py/__init__.py
--rw-r--r--  4.6 unx      181 b- defN 22-Oct-24 03:40 ssbh_data_py/__init__.pyi
--rwxr-xr-x  4.6 unx  2882560 b- defN 22-Oct-24 03:40 ssbh_data_py/ssbh_data_py.cp39-win_amd64.pyd
--rw-r--r--  4.6 unx     1147 b- defN 22-Oct-24 03:40 ssbh_data_py-0.7.1.dist-info/RECORD
-14 files, 2916053 bytes uncompressed, 879362 bytes compressed:  69.8%
+Zip file size: 839771 bytes, number of entries: 14
+-rw-r--r--  4.6 unx       78 b- defN 23-Apr-26 14:22 ssbh_data_py-0.8.0.dist-info/METADATA
+-rw-r--r--  4.6 unx       96 b- defN 23-Apr-26 14:22 ssbh_data_py-0.8.0.dist-info/WHEEL
+-rw-r--r--  4.6 unx      670 b- defN 23-Apr-26 14:22 ssbh_data_py/adj_data.pyi
+-rw-r--r--  4.6 unx     2748 b- defN 23-Apr-26 14:22 ssbh_data_py/anim_data.pyi
+-rw-r--r--  4.6 unx     2175 b- defN 23-Apr-26 14:22 ssbh_data_py/hlpb_data.pyi
+-rw-r--r--  4.6 unx    20261 b- defN 23-Apr-26 14:22 ssbh_data_py/matl_data.pyi
+-rw-r--r--  4.6 unx     1214 b- defN 23-Apr-26 14:22 ssbh_data_py/meshex_data.pyi
+-rw-r--r--  4.6 unx     2708 b- defN 23-Apr-26 14:22 ssbh_data_py/mesh_data.pyi
+-rw-r--r--  4.6 unx      892 b- defN 23-Apr-26 14:22 ssbh_data_py/modl_data.pyi
+-rw-r--r--  4.6 unx     1642 b- defN 23-Apr-26 14:22 ssbh_data_py/skel_data.pyi
+-rw-r--r--  4.6 unx       27 b- defN 23-Apr-26 14:22 ssbh_data_py/__init__.py
+-rw-r--r--  4.6 unx      209 b- defN 23-Apr-26 14:22 ssbh_data_py/__init__.pyi
+-rwxr-xr-x  4.6 unx  2630144 b- defN 23-Apr-26 14:22 ssbh_data_py/ssbh_data_py.cp39-win_amd64.pyd
+-rw-r--r--  4.6 unx     1147 b- defN 23-Apr-26 14:22 ssbh_data_py-0.8.0.dist-info/RECORD
+14 files, 2664011 bytes uncompressed, 837869 bytes compressed:  68.5%
```

## zipnote {}

```diff
@@ -1,11 +1,11 @@
-Filename: ssbh_data_py-0.7.1.dist-info/METADATA
+Filename: ssbh_data_py-0.8.0.dist-info/METADATA
 Comment: 
 
-Filename: ssbh_data_py-0.7.1.dist-info/WHEEL
+Filename: ssbh_data_py-0.8.0.dist-info/WHEEL
 Comment: 
 
 Filename: ssbh_data_py/adj_data.pyi
 Comment: 
 
 Filename: ssbh_data_py/anim_data.pyi
 Comment: 
@@ -33,11 +33,11 @@
 
 Filename: ssbh_data_py/__init__.pyi
 Comment: 
 
 Filename: ssbh_data_py/ssbh_data_py.cp39-win_amd64.pyd
 Comment: 
 
-Filename: ssbh_data_py-0.7.1.dist-info/RECORD
+Filename: ssbh_data_py-0.8.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ssbh_data_py/anim_data.pyi

```diff
@@ -57,37 +57,26 @@
         name: str,
         tracks: list[TrackData] = []
     ) -> None: ...
 
 
 class TrackData:
     name: str
-    values: Union[list[UvTransform], list[Transform],
-                  list[float], list[bool], list[int], list[list[float]]]
-    scale_options: ScaleOptions
+    compensate_scale: bool
     transform_flags: TransformFlags
+    values: Union[list[UvTransform], list[Transform],
+                      list[float], list[bool], list[int], list[list[float]]]
 
     def __init__(
         self,
         name: str,
+        compensate_scale: bool = False,
+        transform_flags: TransformFlags = TransformFlags(),
         values: Union[list[UvTransform], list[Transform],
-                  list[float], list[bool], list[int], list[list[float]]] = [],
-        scale_options: ScaleOptions = ScaleOptions(),
-        transform_flags: TransformFlags = TransformFlags()
-    ) -> None: ...
-
-
-class ScaleOptions:
-    inherit_scale: bool
-    compensate_scale: bool
-
-    def __init__(
-        self,
-        inherit_scale: bool = False,
-        compensate_scale: bool = False
+                      list[float], list[bool], list[int], list[list[float]]] = []
     ) -> None: ...
 
 
 class Transform:
     scale: list[float]
     rotation: list[float]
     translation: list[float]
@@ -111,7 +100,22 @@
         self,
         scale_u: float,
         scale_v: float,
         rotation: float,
         translate_u: float,
         translate_v: float
     ) -> None: ...
+
+
+class TransformFlags:
+    override_translation: bool
+    override_rotation: bool
+    override_scale: bool
+    override_compensate_scale: bool
+
+    def __init__(
+        self,
+        override_translation: bool = False,
+        override_rotation: bool = False,
+        override_scale: bool = False,
+        override_compensate_scale: bool = False
+    ) -> None: ...
```

## ssbh_data_py/meshex_data.pyi

```diff
@@ -14,22 +14,22 @@
     @staticmethod
     def from_mesh_objects(objects: list[MeshObjectData]) -> MeshExData: ...
     
     def save(self, path: str) -> None: ...
 
 
 class MeshObjectGroupData:
-    bounding_sphere: list[float]
+    bounding_sphere: BoundingSphere
     mesh_object_name: str
     mesh_object_full_name: str
     entry_flags: list[MeshObjectGroupData]
 
     def __init__(
         self,
-        bounding_sphere: list[float],
+        bounding_sphere: BoundingSphere,
         mesh_object_name: str,
         mesh_object_full_name: str,
         entry_flags: list[MeshObjectGroupData]
     ) -> None: ...
 
 
 class EntryFlags:
@@ -37,7 +37,18 @@
     cast_shadow: bool
 
     def __init__(
         self,
         draw_model: bool,
         cast_shadow: bool
     ) -> None: ...
+
+
+class BoundingSphere:
+    center: list[float]
+    radius: float
+
+    def __init__(
+        self,
+        center: list[float],
+        radius: float
+    ) -> None: ...
```

## ssbh_data_py/__init__.pyi

```diff
@@ -1,7 +1,8 @@
 from .mesh_data import *
 from .skel_data import *
 from .modl_data import *
 from .anim_data import *
 from .adj_data import *
 from .matl_data import *
-from .meshex_data import *
+from .meshex_data import *
+from .hlpb_data import *
```

## Comparing `ssbh_data_py-0.7.1.dist-info/RECORD` & `ssbh_data_py-0.8.0.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-ssbh_data_py-0.7.1.dist-info/METADATA,sha256=Rm1k24IVPEtbZRB8KYs_MrMg_Ahva1fLBjq5zOER20Q,78
-ssbh_data_py-0.7.1.dist-info/WHEEL,sha256=xkNCugsn-h8xf6GsJ3Jx6cvMIcEM3seDi6SclzAgkco,95
+ssbh_data_py-0.8.0.dist-info/METADATA,sha256=oic_20nAQYOWtMJdcQ83mQg88i-BxvJZ79ex8of46b8,78
+ssbh_data_py-0.8.0.dist-info/WHEEL,sha256=HfbNN9yA0Gn_6VCTRBzbKHMHpOwMN7MCpAKvpT7Uqyk,96
 ssbh_data_py/adj_data.pyi,sha256=8vTAtbEOR_0vtHHxwMdgq7En6rc89YbAprkB5MSOoqc,670
-ssbh_data_py/anim_data.pyi,sha256=Tx1UHF35uF-DBkszswBtUP_Fc7U3mXVfLQ3C6gdvRho,2589
+ssbh_data_py/anim_data.pyi,sha256=DFGY10kJ-eQG5d-Ow_BgR4_0rBMd_1LkhNzz88DcPvM,2748
 ssbh_data_py/hlpb_data.pyi,sha256=g5YHXMgArAACo6ZaDd0x2HdY4HatfoLtwYNu5I7_axc,2175
 ssbh_data_py/matl_data.pyi,sha256=aZBXf7F7qb5ZN1Vf5ffp5uljaUxmyf0J2LpIkImPaH4,20261
-ssbh_data_py/meshex_data.pyi,sha256=G0a17V4rgapYiGE_I5eNK6zLu2OUo3MH8RBmXGVsBdU,1028
+ssbh_data_py/meshex_data.pyi,sha256=mjJw4Aq_28zI30-8kyotN_LTMnakqbzyAQZEBK7a5GI,1214
 ssbh_data_py/mesh_data.pyi,sha256=KDmk3jh4nw-jysJcDQ1LEx0nQktmh4xh5JUvD0BvyC0,2708
 ssbh_data_py/modl_data.pyi,sha256=V-G2xGWMOUA_0yHehScPRF1Gzi3Jo--s7tjS2nROr9g,892
 ssbh_data_py/skel_data.pyi,sha256=G_00vwtKVjdP6QOw0CTwSO7zNsESxJyAmYwXGmtoXQU,1642
 ssbh_data_py/__init__.py,sha256=IBKvTWlMlCF7oXobagQcI2GPsa-S-4DjgbjlvoOchLA,27
-ssbh_data_py/__init__.pyi,sha256=wNY6Sm6zc-DNzNgfIw-k0h4pCIQk7JcjkbCGZ4Ek8-c,181
-ssbh_data_py/ssbh_data_py.cp39-win_amd64.pyd,sha256=Y9WKRvW39gFg-uZwvCZrC8NRQyeW3bOIhA8elj2yAfQ,2882560
-ssbh_data_py-0.7.1.dist-info/RECORD,,
+ssbh_data_py/__init__.pyi,sha256=6IV8oIXNXpEdS3NVRsoLur2XdXM1_OsXnJvf7vardgY,209
+ssbh_data_py/ssbh_data_py.cp39-win_amd64.pyd,sha256=sE0EJtXOX1D9RWD18sqIo-Ss-IaBm4CbEHBR3JEdJD4,2630144
+ssbh_data_py-0.8.0.dist-info/RECORD,,
```

