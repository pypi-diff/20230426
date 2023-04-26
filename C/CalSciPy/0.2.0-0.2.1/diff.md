# Comparing `tmp/CalSciPy-0.2.0.tar.gz` & `tmp/CalSciPy-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CalSciPy-0.2.0.tar", last modified: Thu Apr 13 14:10:37 2023, max compression
+gzip compressed data, was "CalSciPy-0.2.1.tar", last modified: Wed Apr 26 15:22:00 2023, max compression
```

## Comparing `CalSciPy-0.2.0.tar` & `CalSciPy-0.2.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 14:10:37.306677 CalSciPy-0.2.0/
--rw-rw-rw-   0        0        0     1094 2023-02-20 20:08:47.000000 CalSciPy-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     4998 2023-04-13 14:10:37.305677 CalSciPy-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     2840 2023-04-03 15:47:56.000000 CalSciPy-0.2.0/README.md
--rw-rw-rw-   0        0        0     2315 2023-04-06 15:13:42.000000 CalSciPy-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-13 14:10:37.307677 CalSciPy-0.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-13 14:10:37.204677 CalSciPy-0.2.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-13 14:10:37.249755 CalSciPy-0.2.0/src/CalSciPy/
--rw-rw-rw-   0        0        0      388 2023-04-03 13:04:29.000000 CalSciPy-0.2.0/src/CalSciPy/__init__.py
--rw-rw-rw-   0        0        0    11403 2023-04-05 15:38:36.000000 CalSciPy-0.2.0/src/CalSciPy/bruker.py
--rw-rw-rw-   0        0        0     3028 2023-04-07 16:45:41.000000 CalSciPy-0.2.0/src/CalSciPy/coloring.py
--rw-rw-rw-   0        0        0     2237 2023-04-03 13:04:29.000000 CalSciPy-0.2.0/src/CalSciPy/event_processing.py
--rw-rw-rw-   0        0        0     2024 2023-04-03 22:21:07.000000 CalSciPy-0.2.0/src/CalSciPy/image_processing.py
--rw-rw-rw-   0        0        0     9196 2023-04-05 16:04:42.000000 CalSciPy-0.2.0/src/CalSciPy/io_tools.py
--rw-rw-rw-   0        0        0     5129 2023-04-05 15:54:33.000000 CalSciPy-0.2.0/src/CalSciPy/misc.py
--rw-rw-rw-   0        0        0     3444 2023-03-29 17:06:08.000000 CalSciPy-0.2.0/src/CalSciPy/reorganization.py
--rw-rw-rw-   0        0        0     4770 2023-03-29 21:13:37.000000 CalSciPy-0.2.0/src/CalSciPy/trace_processing.py
--rw-rw-rw-   0        0        0      199 2023-02-20 22:24:54.000000 CalSciPy-0.2.0/src/CalSciPy/version.py
-drwxrwxrwx   0        0        0        0 2023-04-13 14:10:37.268678 CalSciPy-0.2.0/src/CalSciPy.egg-info/
--rw-rw-rw-   0        0        0     4998 2023-04-13 14:10:37.000000 CalSciPy-0.2.0/src/CalSciPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      701 2023-04-13 14:10:37.000000 CalSciPy-0.2.0/src/CalSciPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 14:10:37.000000 CalSciPy-0.2.0/src/CalSciPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      358 2023-04-13 14:10:37.000000 CalSciPy-0.2.0/src/CalSciPy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-04-13 14:10:37.000000 CalSciPy-0.2.0/src/CalSciPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2023-02-20 20:08:47.000000 CalSciPy-0.2.0/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 14:10:37.300677 CalSciPy-0.2.0/tests/
--rw-rw-rw-   0        0        0     1933 2023-04-03 13:04:29.000000 CalSciPy-0.2.0/tests/test_a_install.py
--rw-rw-rw-   0        0        0     3074 2023-04-05 17:07:30.000000 CalSciPy-0.2.0/tests/test_bruker.py
--rw-rw-rw-   0        0        0      887 2023-04-07 16:44:54.000000 CalSciPy-0.2.0/tests/test_coloring.py
--rw-rw-rw-   0        0        0     1218 2023-04-03 15:39:20.000000 CalSciPy-0.2.0/tests/test_event_processing.py
--rw-rw-rw-   0        0        0    12735 2023-04-05 16:39:27.000000 CalSciPy-0.2.0/tests/test_io_tools.py
--rw-rw-rw-   0        0        0     2373 2023-04-05 15:55:20.000000 CalSciPy-0.2.0/tests/test_misc.py
--rw-rw-rw-   0        0        0     5124 2023-03-29 19:08:15.000000 CalSciPy-0.2.0/tests/test_reorganization.py
--rw-rw-rw-   0        0        0     3250 2023-03-29 21:11:25.000000 CalSciPy-0.2.0/tests/test_trace_processing.py
+drwxrwxrwx   0        0        0        0 2023-04-26 15:22:00.030279 CalSciPy-0.2.1/
+-rw-rw-rw-   0        0        0     1094 2023-02-20 20:08:47.000000 CalSciPy-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0     4998 2023-04-26 15:22:00.029279 CalSciPy-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2840 2023-04-03 15:47:56.000000 CalSciPy-0.2.1/README.md
+-rw-rw-rw-   0        0        0     2330 2023-04-26 15:21:16.000000 CalSciPy-0.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-26 15:22:00.030279 CalSciPy-0.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-26 15:21:59.929318 CalSciPy-0.2.1/src/
+drwxrwxrwx   0        0        0        0 2023-04-26 15:21:59.968279 CalSciPy-0.2.1/src/CalSciPy/
+-rw-rw-rw-   0        0        0      388 2023-04-03 13:04:29.000000 CalSciPy-0.2.1/src/CalSciPy/__init__.py
+-rw-rw-rw-   0        0        0    11403 2023-04-05 15:38:36.000000 CalSciPy-0.2.1/src/CalSciPy/bruker.py
+-rw-rw-rw-   0        0        0     3028 2023-04-07 16:45:41.000000 CalSciPy-0.2.1/src/CalSciPy/coloring.py
+-rw-rw-rw-   0        0        0     2237 2023-04-03 13:04:29.000000 CalSciPy-0.2.1/src/CalSciPy/event_processing.py
+-rw-rw-rw-   0        0        0     2115 2023-04-26 15:19:07.000000 CalSciPy-0.2.1/src/CalSciPy/image_processing.py
+-rw-rw-rw-   0        0        0     9653 2023-04-26 15:19:07.000000 CalSciPy-0.2.1/src/CalSciPy/io_tools.py
+-rw-rw-rw-   0        0        0     5129 2023-04-05 15:54:33.000000 CalSciPy-0.2.1/src/CalSciPy/misc.py
+-rw-rw-rw-   0        0        0     3444 2023-03-29 17:06:08.000000 CalSciPy-0.2.1/src/CalSciPy/reorganization.py
+-rw-rw-rw-   0        0        0     4770 2023-03-29 21:13:37.000000 CalSciPy-0.2.1/src/CalSciPy/trace_processing.py
+-rw-rw-rw-   0        0        0      199 2023-02-20 22:24:54.000000 CalSciPy-0.2.1/src/CalSciPy/version.py
+drwxrwxrwx   0        0        0        0 2023-04-26 15:21:59.987278 CalSciPy-0.2.1/src/CalSciPy.egg-info/
+-rw-rw-rw-   0        0        0     4998 2023-04-26 15:21:59.000000 CalSciPy-0.2.1/src/CalSciPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      701 2023-04-26 15:21:59.000000 CalSciPy-0.2.1/src/CalSciPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 15:21:59.000000 CalSciPy-0.2.1/src/CalSciPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      365 2023-04-26 15:21:59.000000 CalSciPy-0.2.1/src/CalSciPy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-04-26 15:21:59.000000 CalSciPy-0.2.1/src/CalSciPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2023-02-20 20:08:47.000000 CalSciPy-0.2.1/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 15:22:00.025280 CalSciPy-0.2.1/tests/
+-rw-rw-rw-   0        0        0     1933 2023-04-03 13:04:29.000000 CalSciPy-0.2.1/tests/test_a_install.py
+-rw-rw-rw-   0        0        0     3074 2023-04-05 17:07:30.000000 CalSciPy-0.2.1/tests/test_bruker.py
+-rw-rw-rw-   0        0        0      887 2023-04-07 16:44:54.000000 CalSciPy-0.2.1/tests/test_coloring.py
+-rw-rw-rw-   0        0        0     1218 2023-04-03 15:39:20.000000 CalSciPy-0.2.1/tests/test_event_processing.py
+-rw-rw-rw-   0        0        0    12735 2023-04-05 16:39:27.000000 CalSciPy-0.2.1/tests/test_io_tools.py
+-rw-rw-rw-   0        0        0     2373 2023-04-05 15:55:20.000000 CalSciPy-0.2.1/tests/test_misc.py
+-rw-rw-rw-   0        0        0     5124 2023-03-29 19:08:15.000000 CalSciPy-0.2.1/tests/test_reorganization.py
+-rw-rw-rw-   0        0        0     3250 2023-03-29 21:11:25.000000 CalSciPy-0.2.1/tests/test_trace_processing.py
```

### Comparing `CalSciPy-0.2.0/LICENSE` & `CalSciPy-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.0/PKG-INFO` & `CalSciPy-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CalSciPy
-Version: 0.2.0
+Version: 0.2.1
 Summary: A collection
 Author: Darik A. O'Neil
 Maintainer: Darik A. O'Neil
 License: MIT License
         
         Copyright (c) 2023 Darik A O’Neil
```

### Comparing `CalSciPy-0.2.0/README.md` & `CalSciPy-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.0/pyproject.toml` & `CalSciPy-0.2.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "CalSciPy"
-version = "0.2.0"
+version = "0.2.1"
 description = "A collection"
 readme = "README.md"
 requires-python = ">=3.7, <4"
 license = {file = "LICENSE"}
 keywords = ["CalSciPy", "Calcium Imaging"]
 authors = [
   {name = "Darik A. O'Neil"}
@@ -28,14 +28,15 @@
     "Programming Language :: Python :: 3.10",
 ]
 
 dependencies = [
     "matplotlib",
     "numpy",
     "opencv-python",
+    "pillow",
     "PPVD",
     "prettytable",
     "pyside2",
     "seaborn",
     "scipy",
     "tqdm"
 ]
```

### Comparing `CalSciPy-0.2.0/src/CalSciPy/bruker.py` & `CalSciPy-0.2.1/src/CalSciPy/bruker.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.0/src/CalSciPy/coloring.py` & `CalSciPy-0.2.1/src/CalSciPy/coloring.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.0/src/CalSciPy/event_processing.py` & `CalSciPy-0.2.1/src/CalSciPy/event_processing.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.0/src/CalSciPy/image_processing.py` & `CalSciPy-0.2.1/src/CalSciPy/image_processing.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,14 +43,17 @@
 
     filtered_images = cupy.asarray(filtered_images)
 
     frames = filtered_images.shape[0]
 
     if block_size:
         block_gen = generate_blocks(range(frames), block_size, block_buffer)
-        for block in block_gen:
-            filtered_images[block, :, :] = cupyx.scipy.ndimage.median_filter(filtered_images[block, :, :],
-                                                                             footprint=mask)
+        try:
+            for block in block_gen:
+                filtered_images[block, :, :] = cupyx.scipy.ndimage.median_filter(filtered_images[block, :, :],
+                                                                                 footprint=mask)
+        except (RuntimeError, StopIteration):
+            pass
     else:
         filtered_images = cupyx.scipy.ndimage.median_filter(filtered_images, footprint=mask)
 
     return filtered_images.get()
```

### Comparing `CalSciPy-0.2.0/src/CalSciPy/io_tools.py` & `CalSciPy-0.2.1/src/CalSciPy/io_tools.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 from typing import Union, Optional
 from pathlib import Path
 import cv2
+from PIL import Image
 import numpy as np
 from json import load, dump
 from PPVD.validation import validate_extension, validate_filename
 from PPVD.parsing import convert_permitted_types_to_required
 from .misc import generate_blocks, calculate_frames_per_file
 
 
@@ -167,15 +168,25 @@
 
     return np.concatenate(images, axis=0)
 
 
 @validate_extension(required_extension=".tif", pos=0)
 @convert_permitted_types_to_required(permitted=(str, Path), required=str, pos=0)
 def _save_single_tif(path: Union[str, Path], images: np.ndarray) -> int:
-    cv2.imwritemulti(path, images)
+    # if single page save direct
+    if len(images.shape) == 2:
+        images = Image.fromarray(images)
+        images.save(path)
+    # if multi page iterate
+    else:
+        images_to_save = []
+        for single_image in range(images.shape[0]):
+            images_to_save.append(Image.fromarray(images[single_image, :, :]))
+        images_to_save[0].save(path, format="TIFF", save_all=True, append_images=images_to_save[1:])
+    return 0
 
 
 @validate_extension(required_extension=".tif", pos=0)
 @convert_permitted_types_to_required(permitted=(str, Path), required=Path, pos=0)
 def _save_many_tif(path: Union[str, Path], images: np.ndarray, size_cap: int = 3.9) -> int:
     frames_per_file = calculate_frames_per_file(*images.shape[1:], size_cap=size_cap)
     frames = list(range(images.shape[0]))
@@ -189,15 +200,15 @@
                 filename = base_filename.with_name("".join([base_filename.name, "_0", str(idx)]))
                 filename = filename.with_suffix(".tif")
             else:
                 filename = path.with_name("".join([base_filename.name, "_", str(idx)]))
                 filename = filename.with_suffix(".tif")
             _save_single_tif(filename, images[block, :, :])
             idx += 1
-    except RuntimeError:
+    except (RuntimeError, StopIteration):
         pass
     return 0
 
 
 class _Metadata:
     def __init__(self, images: Optional[np.ndarray] = None):
         """
```

### Comparing `CalSciPy-0.2.0/src/CalSciPy/misc.py` & `CalSciPy-0.2.1/src/CalSciPy/misc.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.0/src/CalSciPy/reorganization.py` & `CalSciPy-0.2.1/src/CalSciPy/reorganization.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.0/src/CalSciPy/trace_processing.py` & `CalSciPy-0.2.1/src/CalSciPy/trace_processing.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.0/src/CalSciPy.egg-info/PKG-INFO` & `CalSciPy-0.2.1/src/CalSciPy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CalSciPy
-Version: 0.2.0
+Version: 0.2.1
 Summary: A collection
 Author: Darik A. O'Neil
 Maintainer: Darik A. O'Neil
 License: MIT License
         
         Copyright (c) 2023 Darik A O’Neil
```

### Comparing `CalSciPy-0.2.0/src/CalSciPy.egg-info/SOURCES.txt` & `CalSciPy-0.2.1/src/CalSciPy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.0/tests/test_a_install.py` & `CalSciPy-0.2.1/tests/test_a_install.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.0/tests/test_bruker.py` & `CalSciPy-0.2.1/tests/test_bruker.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.0/tests/test_coloring.py` & `CalSciPy-0.2.1/tests/test_coloring.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.0/tests/test_event_processing.py` & `CalSciPy-0.2.1/tests/test_event_processing.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.0/tests/test_io_tools.py` & `CalSciPy-0.2.1/tests/test_io_tools.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.0/tests/test_misc.py` & `CalSciPy-0.2.1/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.0/tests/test_reorganization.py` & `CalSciPy-0.2.1/tests/test_reorganization.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.0/tests/test_trace_processing.py` & `CalSciPy-0.2.1/tests/test_trace_processing.py`

 * *Files identical despite different names*

