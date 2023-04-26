# Comparing `tmp/pylinalg-0.3.3.tar.gz` & `tmp/pylinalg-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylinalg-0.3.3.tar", max compression
+gzip compressed data, was "pylinalg-0.3.4.tar", max compression
```

## Comparing `pylinalg-0.3.3.tar` & `pylinalg-0.3.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1077 2023-04-07 11:06:26.891140 pylinalg-0.3.3/LICENSE
--rw-r--r--   0        0        0      142 2023-04-07 11:06:26.891140 pylinalg-0.3.3/README.md
--rw-r--r--   0        0        0      191 2023-04-07 11:06:26.891140 pylinalg-0.3.3/pylinalg/__init__.py
--rw-r--r--   0        0        0      216 2023-04-07 11:06:26.891140 pylinalg-0.3.3/pylinalg/func/__init__.py
--rw-r--r--   0        0        0    20035 2023-04-07 11:06:26.891140 pylinalg-0.3.3/pylinalg/func/matrix.py
--rw-r--r--   0        0        0     3303 2023-04-07 11:06:26.891140 pylinalg-0.3.3/pylinalg/func/misc.py
--rw-r--r--   0        0        0     7277 2023-04-07 11:06:26.891140 pylinalg-0.3.3/pylinalg/func/quaternion.py
--rw-r--r--   0        0        0    15026 2023-04-07 11:06:26.891140 pylinalg-0.3.3/pylinalg/func/vector.py
--rw-r--r--   0        0        0        0 2023-04-07 11:06:26.891140 pylinalg-0.3.3/pylinalg/obj/__init__.py
--rw-r--r--   0        0        0      761 2023-04-07 11:06:26.891140 pylinalg-0.3.3/pyproject.toml
--rw-r--r--   0        0        0      822 1970-01-01 00:00:00.000000 pylinalg-0.3.3/setup.py
--rw-r--r--   0        0        0      751 1970-01-01 00:00:00.000000 pylinalg-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-04-26 13:22:06.925579 pylinalg-0.3.4/LICENSE
+-rw-r--r--   0        0        0      142 2023-04-26 13:22:06.925579 pylinalg-0.3.4/README.md
+-rw-r--r--   0        0        0      245 2023-04-26 13:22:06.929579 pylinalg-0.3.4/pylinalg/__init__.py
+-rw-r--r--   0        0        0      216 2023-04-26 13:22:06.929579 pylinalg-0.3.4/pylinalg/func/__init__.py
+-rw-r--r--   0        0        0    19983 2023-04-26 13:22:06.929579 pylinalg-0.3.4/pylinalg/func/matrix.py
+-rw-r--r--   0        0        0     4712 2023-04-26 13:22:06.929579 pylinalg-0.3.4/pylinalg/func/misc.py
+-rw-r--r--   0        0        0     9272 2023-04-26 13:22:06.929579 pylinalg-0.3.4/pylinalg/func/quaternion.py
+-rw-r--r--   0        0        0    15070 2023-04-26 13:22:06.929579 pylinalg-0.3.4/pylinalg/func/vector.py
+-rw-r--r--   0        0        0        0 2023-04-26 13:22:06.929579 pylinalg-0.3.4/pylinalg/obj/__init__.py
+-rw-r--r--   0        0        0      761 2023-04-26 13:22:06.929579 pylinalg-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0      822 1970-01-01 00:00:00.000000 pylinalg-0.3.4/setup.py
+-rw-r--r--   0        0        0      751 1970-01-01 00:00:00.000000 pylinalg-0.3.4/PKG-INFO
```

### Comparing `pylinalg-0.3.3/LICENSE` & `pylinalg-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pylinalg-0.3.3/pylinalg/func/matrix.py` & `pylinalg-0.3.4/pylinalg/func/matrix.py`

 * *Files 1% similar despite different names*

```diff
@@ -600,21 +600,20 @@
     # Currently numpy doesn't support axes on fill_diagonal, so we do it
     # ourselves to support input batches and mimic the `np.linalg` API.
     n_matrices = np.prod(result_shape[:-1], dtype=int)
     itemsize = out.itemsize
     view = as_strided(out, shape=(n_matrices, 4), strides=(16 * itemsize, 5 * itemsize))
     view[:] = 1
 
-    # Note: building the inverse/transpose directly
-    out[..., 2, :-1] = new_z / np.linalg.norm(new_z, axis=-1)
-    out[..., 0, :-1] = np.cross(
-        up_reference, out[..., 2, :-1], axisa=-1, axisb=-1, axisc=-1
+    out[..., :-1, 2] = new_z / np.linalg.norm(new_z, axis=-1)
+    out[..., :-1, 0] = np.cross(
+        up_reference, out[..., :-1, 2], axisa=-1, axisb=-1, axisc=-1
     )
-    out[..., 1, :-1] = np.cross(
-        out[..., 2, :-1], out[..., 0, :-1], axisa=-1, axisb=-1, axisc=-1
+    out[..., :-1, 1] = np.cross(
+        out[..., :-1, 2], out[..., :-1, 0], axisa=-1, axisb=-1, axisc=-1
     )
-    out /= np.linalg.norm(out, axis=-1)[..., :, None]
+    out /= np.linalg.norm(out, axis=-2)[..., None, :]
 
     return out
 
 
 __all__ = [name for name in globals() if name.startswith("matrix_")]
```

### Comparing `pylinalg-0.3.3/pylinalg/func/misc.py` & `pylinalg-0.3.4/pylinalg/func/misc.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 from numpy.lib.stride_tricks import as_strided
 
-__all__ = ["aabb_to_sphere", "aabb_transform"]
+__all__ = ["aabb_to_sphere", "aabb_transform", "axis_angle_from_quaternion"]
 
 
 def aabb_to_sphere(aabb, /, *, out=None, dtype=None):
     """A sphere that envelops an Axis-Aligned Bounding Box.
 
     Parameters
     ----------
@@ -103,7 +103,51 @@
     corners[..., 3] = 1
 
     corners = corners @ matrix
     out[..., 0, :] = np.min(corners[..., :-1], axis=-2)
     out[..., 1, :] = np.max(corners[..., :-1], axis=-2)
 
     return out
+
+
+def axis_angle_from_quaternion(quaternion, /, *, out=None, dtype=None):
+    """Convert a quaternion to axis-angle representation.
+
+    Parameters
+    ----------
+    quaternion : ndarray, [4]
+        A quaternion describing the rotation.
+    out : Tuple[ndarray, ...], optional
+        A location into which the result is stored. If provided, it
+        must have a shape that the inputs broadcast to. If not provided or
+        None, a freshly-allocated array is returned. A tuple must have
+        length equal to the number of outputs.
+    dtype : data-type, optional
+        Overrides the data type of the result.
+
+    Returns
+    -------
+    axis : ndarray, [3]
+        The axis around which the quaternion rotates in euclidean coordinates.
+    angle : ndarray, [1]
+        The angle (in rad) by which the quaternion rotates.
+
+    Notes
+    -----
+    To use `out` with a single quaternion you need to provide a ndarray of shape
+    ``(1,)`` for angle.
+
+    """
+
+    quaternion = np.asarray(quaternion)
+
+    if out is None:
+        quaternion = quaternion.astype(dtype)
+        out = (
+            quaternion[..., :3] / np.sqrt(1 - quaternion[..., 3] ** 2),
+            2 * np.arccos(quaternion[..., 3]),
+        )
+    else:
+        out[0][:] = quaternion[..., :3] / np.sqrt(1 - quaternion[..., 3] ** 2)
+        out[1][:] = 2 * np.arccos(quaternion[..., 3])
+
+    return out
```

### Comparing `pylinalg-0.3.3/pylinalg/func/vector.py` & `pylinalg-0.3.4/pylinalg/func/vector.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,16 +206,18 @@
 
     # based on https://gamedev.stackexchange.com/a/50545
     # (more readable than my attempt at doing the same)
 
     quat_vector = quaternion[..., :-1]
     quat_scalar = quaternion[..., -1]
 
-    out += 2 * np.sum(quat_vector * vector, axis=-1) * quat_vector
-    out += (quat_scalar**2 - np.sum(quat_vector * quat_vector, axis=-1)) * vector
+    out += 2 * np.sum(quat_vector * vector, axis=-1, keepdims=True) * quat_vector
+    out += (
+        quat_scalar**2 - np.sum(quat_vector * quat_vector, axis=-1, keepdims=True)
+    ) * vector
     out += 2 * quat_scalar * np.cross(quat_vector, vector)
 
     return out
 
 
 def vector_spherical_to_euclidean(spherical, /, *, out=None, dtype=None):
     """Convert spherical -> euclidian coordinates.
```

### Comparing `pylinalg-0.3.3/pyproject.toml` & `pylinalg-0.3.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pylinalg"
-version = "0.3.3"
+version = "0.3.4"
 description = "Linear algebra utilities for Python"
 authors = ["Korijn van Golen <korijn@gmail.com>"]
 license = "MIT"
 homepage = "https://github.com/pygfx/pylinalg"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `pylinalg-0.3.3/setup.py` & `pylinalg-0.3.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['numpy>=1.20.0']
 
 setup_kwargs = {
     'name': 'pylinalg',
-    'version': '0.3.3',
+    'version': '0.3.4',
     'description': 'Linear algebra utilities for Python',
     'long_description': '[![PyPI version](https://badge.fury.io/py/pylinalg.svg)](https://badge.fury.io/py/pylinalg)\n\n# pylinalg\n\nLinear algebra utilities for Python.\n',
     'author': 'Korijn van Golen',
     'author_email': 'korijn@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/pygfx/pylinalg',
```

### Comparing `pylinalg-0.3.3/PKG-INFO` & `pylinalg-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylinalg
-Version: 0.3.3
+Version: 0.3.4
 Summary: Linear algebra utilities for Python
 Home-page: https://github.com/pygfx/pylinalg
 License: MIT
 Author: Korijn van Golen
 Author-email: korijn@gmail.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
```

