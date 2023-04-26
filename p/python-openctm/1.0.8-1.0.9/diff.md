# Comparing `tmp/python_openctm-1.0.8-cp37-cp37m-manylinux1_x86_64.whl.zip` & `tmp/python_openctm-1.0.9-cp37-cp37m-manylinux1_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 52830 bytes, number of entries: 10
--rwxr-xr-x  2.0 unx     5956 b- defN 18-Aug-28 14:44 _foo.cpython-37m-x86_64-linux-gnu.so
--rw-r--r--  2.0 unx       46 b- defN 18-Aug-28 14:42 openctm/__init__.py
--rw-r--r--  2.0 unx       21 b- defN 18-Aug-28 14:42 openctm/version.py
--rw-r--r--  2.0 unx     6648 b- defN 18-Aug-28 14:42 openctm/openctm.py
--rw-r--r--  2.0 unx     3086 b- defN 18-Aug-28 14:42 openctm/io.py
--rwxr-xr-x  2.0 unx    93480 b- defN 18-Aug-28 14:43 openctm/libs/libopenctm.so
--rw-r--r--  2.0 unx      109 b- defN 18-Aug-28 14:44 python_openctm-1.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 18-Aug-28 14:44 python_openctm-1.0.8.dist-info/top_level.txt
--rw-r--r--  2.0 unx     1545 b- defN 18-Aug-28 14:44 python_openctm-1.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx      806 b- defN 18-Aug-28 14:44 python_openctm-1.0.8.dist-info/RECORD
-10 files, 111710 bytes uncompressed, 51476 bytes compressed:  53.9%
+Zip file size: 52825 bytes, number of entries: 10
+-rwxr-xr-x  2.0 unx     5956 b- defN 18-Aug-28 15:15 _foo.cpython-37m-x86_64-linux-gnu.so
+-rw-r--r--  2.0 unx       46 b- defN 18-Aug-28 15:14 openctm/__init__.py
+-rw-r--r--  2.0 unx       21 b- defN 18-Aug-28 15:14 openctm/version.py
+-rw-r--r--  2.0 unx     6648 b- defN 18-Aug-28 15:14 openctm/openctm.py
+-rw-r--r--  2.0 unx     3050 b- defN 18-Aug-28 15:14 openctm/io.py
+-rwxr-xr-x  2.0 unx    93480 b- defN 18-Aug-28 15:14 openctm/libs/libopenctm.so
+-rw-r--r--  2.0 unx      109 b- defN 18-Aug-28 15:15 python_openctm-1.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 18-Aug-28 15:15 python_openctm-1.0.9.dist-info/top_level.txt
+-rw-r--r--  2.0 unx     1545 b- defN 18-Aug-28 15:15 python_openctm-1.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx      806 b- defN 18-Aug-28 15:15 python_openctm-1.0.9.dist-info/RECORD
+10 files, 111674 bytes uncompressed, 51471 bytes compressed:  53.9%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: openctm/io.py
 Comment: 
 
 Filename: openctm/libs/libopenctm.so
 Comment: 
 
-Filename: python_openctm-1.0.8.dist-info/WHEEL
+Filename: python_openctm-1.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: python_openctm-1.0.8.dist-info/top_level.txt
+Filename: python_openctm-1.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: python_openctm-1.0.8.dist-info/METADATA
+Filename: python_openctm-1.0.9.dist-info/METADATA
 Comment: 
 
-Filename: python_openctm-1.0.8.dist-info/RECORD
+Filename: python_openctm-1.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## openctm/version.py

```diff
@@ -1 +1 @@
-__version__ = '1.0.8'
+__version__ = '1.0.9'
```

## openctm/io.py

```diff
@@ -3,19 +3,18 @@
 
 
 class CTM:
     """
     Object that encapsulates a CTM file
     """
 
-    def __init__(self, _vertices, _faces, _normals=None, _filename=""):
+    def __init__(self, _vertices, _faces, _normals=None):
         self.vertices = _vertices
         self.faces = _faces
         self.normals = _normals
-        self.filename = _filename
 
     def __eq__(self, other):
         return (self.vertices == other.vertices).all() and (self.faces == other.faces).all()
 
 
 def import_mesh(_filename):
     ctm_context = ctmNewContext(CTM_IMPORT)
@@ -68,15 +67,15 @@
 
         face_count = len(_ctm.faces)
         faces = _ctm.faces.reshape((-1, 1))
         p_faces = ctypes.cast((CTMuint * face_count * 3)(), ctypes.POINTER(CTMuint))
         for i in range(face_count * 3):
             p_faces[i] = CTMuint(faces[i])
 
-        if _ctm.normals:
+        if _ctm.normals is not None:
             normal_count = len(_ctm.normals)
             normals = _ctm.normals.reshape((-1, 1))
             p_normals = ctypes.cast((CTMfloat * normal_count * 3)(), ctypes.POINTER(CTMfloat))
             for i in range(normal_count * 3):
                 p_normals[i] = CTMfloat(normals[i])
         else:
             p_normals = None
```

## Comparing `python_openctm-1.0.8.dist-info/METADATA` & `python_openctm-1.0.9.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-openctm
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python Interface for the OpenCTM File Format
 Home-page: https://github.com/lejafar/python-openctm
 Author: Rafael Hautekiet
 Author-email: rafaelhautekiet@gmail.com
 License: zlib License
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 2.7
```

