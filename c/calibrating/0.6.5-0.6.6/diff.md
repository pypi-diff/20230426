# Comparing `tmp/calibrating-0.6.5.tar.gz` & `tmp/calibrating-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/calibrating-0.6.5.tar", last modified: Sun Apr 16 15:29:30 2023, max compression
+gzip compressed data, was "dist/calibrating-0.6.6.tar", last modified: Wed Apr 26 05:52:59 2023, max compression
```

## Comparing `calibrating-0.6.5.tar` & `calibrating-0.6.6.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2023-04-16 15:29:30.000000 calibrating-0.6.5/
--rw-rw-r--   0 dl        (1000) dl        (1000)       35 2021-08-19 08:36:59.000000 calibrating-0.6.5/MANIFEST.in
--rw-rw-r--   0 dl        (1000) dl        (1000)      647 2023-04-16 15:29:30.000000 calibrating-0.6.5/PKG-INFO
--rw-rw-r--   0 dl        (1000) dl        (1000)     5544 2023-01-11 07:48:52.000000 calibrating-0.6.5/README.md
-drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2023-04-16 15:29:30.000000 calibrating-0.6.5/calibrating/
--rw-rw-r--   0 dl        (1000) dl        (1000)      643 2023-04-16 15:28:31.000000 calibrating-0.6.5/calibrating/__info__.py
--rw-rw-r--   0 dl        (1000) dl        (1000)      249 2022-12-22 13:24:45.000000 calibrating-0.6.5/calibrating/__init__.py
--rw-rw-r--   0 dl        (1000) dl        (1000)    18323 2023-04-16 15:28:48.000000 calibrating-0.6.5/calibrating/boards.py
--rw-rw-r--   0 dl        (1000) dl        (1000)    21801 2023-04-14 05:38:18.000000 calibrating-0.6.5/calibrating/camera.py
--rw-rw-r--   0 dl        (1000) dl        (1000)     1521 2022-12-22 17:59:18.000000 calibrating-0.6.5/calibrating/feature_libs.py
--rw-rw-r--   0 dl        (1000) dl        (1000)     4730 2023-02-07 10:00:28.000000 calibrating-0.6.5/calibrating/multi_boards.py
--rw-rw-r--   0 dl        (1000) dl        (1000)     3200 2022-12-22 13:14:32.000000 calibrating-0.6.5/calibrating/reconstruction.py
--rw-rw-r--   0 dl        (1000) dl        (1000)    21305 2023-04-13 11:51:43.000000 calibrating-0.6.5/calibrating/stereo.py
--rw-rw-r--   0 dl        (1000) dl        (1000)    25439 2023-04-16 14:55:01.000000 calibrating-0.6.5/calibrating/utils.py
-drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2023-04-16 15:29:30.000000 calibrating-0.6.5/calibrating.egg-info/
--rw-rw-r--   0 dl        (1000) dl        (1000)      647 2023-04-16 15:29:30.000000 calibrating-0.6.5/calibrating.egg-info/PKG-INFO
--rw-rw-r--   0 dl        (1000) dl        (1000)      442 2023-04-16 15:29:30.000000 calibrating-0.6.5/calibrating.egg-info/SOURCES.txt
--rw-rw-r--   0 dl        (1000) dl        (1000)        1 2023-04-16 15:29:30.000000 calibrating-0.6.5/calibrating.egg-info/dependency_links.txt
--rw-rw-r--   0 dl        (1000) dl        (1000)       57 2023-04-16 15:29:30.000000 calibrating-0.6.5/calibrating.egg-info/requires.txt
--rw-rw-r--   0 dl        (1000) dl        (1000)       12 2023-04-16 15:29:30.000000 calibrating-0.6.5/calibrating.egg-info/top_level.txt
--rw-rw-r--   0 dl        (1000) dl        (1000)       57 2023-04-16 15:27:46.000000 calibrating-0.6.5/requirements.txt
--rw-rw-r--   0 dl        (1000) dl        (1000)       38 2023-04-16 15:29:30.000000 calibrating-0.6.5/setup.cfg
--rw-rw-r--   0 dl        (1000) dl        (1000)      853 2021-08-19 08:44:30.000000 calibrating-0.6.5/setup.py
+drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2023-04-26 05:52:59.000000 calibrating-0.6.6/
+-rw-rw-r--   0 dl        (1000) dl        (1000)       35 2021-08-19 08:36:59.000000 calibrating-0.6.6/MANIFEST.in
+-rw-rw-r--   0 dl        (1000) dl        (1000)      647 2023-04-26 05:52:59.000000 calibrating-0.6.6/PKG-INFO
+-rw-rw-r--   0 dl        (1000) dl        (1000)     5544 2023-01-11 07:48:52.000000 calibrating-0.6.6/README.md
+drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2023-04-26 05:52:59.000000 calibrating-0.6.6/calibrating/
+-rw-rw-r--   0 dl        (1000) dl        (1000)      643 2023-04-26 05:47:41.000000 calibrating-0.6.6/calibrating/__info__.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)      280 2023-04-25 05:33:13.000000 calibrating-0.6.6/calibrating/__init__.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)    18323 2023-04-16 15:28:48.000000 calibrating-0.6.6/calibrating/boards.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)    21816 2023-04-23 07:58:22.000000 calibrating-0.6.6/calibrating/camera.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)     1521 2022-12-22 17:59:18.000000 calibrating-0.6.6/calibrating/feature_libs.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)     4730 2023-02-07 10:00:28.000000 calibrating-0.6.6/calibrating/multi_boards.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)     3200 2022-12-22 13:14:32.000000 calibrating-0.6.6/calibrating/reconstruction.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)    17456 2023-04-25 06:03:55.000000 calibrating-0.6.6/calibrating/stereo.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)     6901 2023-04-26 05:50:03.000000 calibrating-0.6.6/calibrating/stereo_matching.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)    26459 2023-04-25 07:15:58.000000 calibrating-0.6.6/calibrating/utils.py
+drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2023-04-26 05:52:59.000000 calibrating-0.6.6/calibrating.egg-info/
+-rw-rw-r--   0 dl        (1000) dl        (1000)      647 2023-04-26 05:52:58.000000 calibrating-0.6.6/calibrating.egg-info/PKG-INFO
+-rw-rw-r--   0 dl        (1000) dl        (1000)      473 2023-04-26 05:52:58.000000 calibrating-0.6.6/calibrating.egg-info/SOURCES.txt
+-rw-rw-r--   0 dl        (1000) dl        (1000)        1 2023-04-26 05:52:58.000000 calibrating-0.6.6/calibrating.egg-info/dependency_links.txt
+-rw-rw-r--   0 dl        (1000) dl        (1000)       57 2023-04-26 05:52:58.000000 calibrating-0.6.6/calibrating.egg-info/requires.txt
+-rw-rw-r--   0 dl        (1000) dl        (1000)       12 2023-04-26 05:52:58.000000 calibrating-0.6.6/calibrating.egg-info/top_level.txt
+-rw-rw-r--   0 dl        (1000) dl        (1000)       57 2023-04-16 15:27:46.000000 calibrating-0.6.6/requirements.txt
+-rw-rw-r--   0 dl        (1000) dl        (1000)       38 2023-04-26 05:52:59.000000 calibrating-0.6.6/setup.cfg
+-rw-rw-r--   0 dl        (1000) dl        (1000)      853 2021-08-19 08:44:30.000000 calibrating-0.6.6/setup.py
```

### Comparing `calibrating-0.6.5/PKG-INFO` & `calibrating-0.6.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calibrating
-Version: 0.6.5
+Version: 0.6.6
 Summary: Calibrate camera's intrinsic/extristric, and build stereo depth camera with OpenCV python.
 Home-page: https://github.com/DIYer22/calibrating
 Author: DIYer22
 Author-email: ylxx@live.com
 License: UNKNOWN
 Description: Calibrate camera's intrinsic/extristric, and build stereo depth camera with OpenCV python.
 Platform: UNKNOWN
```

### Comparing `calibrating-0.6.5/README.md` & `calibrating-0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `calibrating-0.6.5/calibrating/__info__.py` & `calibrating-0.6.6/calibrating/__info__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.6.5"
+__version__ = "0.6.6"
 __description__ = "Calibrate camera's intrinsic/extristric, and build stereo depth camera with OpenCV python."
 __license__ = "MIT"
 __author__ = "DIYer22"
 __author_email__ = "ylxx@live.com"
 __maintainer__ = "DIYer22"
 __maintainer_email__ = "ylxx@live.com"
 __github_username__ = "DIYer22"
```

### Comparing `calibrating-0.6.5/calibrating/boards.py` & `calibrating-0.6.6/calibrating/boards.py`

 * *Files identical despite different names*

### Comparing `calibrating-0.6.5/calibrating/camera.py` & `calibrating-0.6.6/calibrating/camera.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 #!/usr/bin/env python3
 
-import boxx
-from boxx import imread
-
 import os
 import cv2
+import boxx
 import yaml
 import copy
 import uuid
 import pickle
 import numpy as np
 from glob import glob
 from tqdm import tqdm
@@ -51,15 +49,15 @@
             left_idx, right_idx = self.get_key_idx(img_paths)
             img_paths = {path[left_idx:right_idx]: path for path in sorted(img_paths)}
         self.img_paths = img_paths
         if self._cache():
             return
         for key in tqdm(sorted(img_paths)):
             path = img_paths[key]
-            d = dict(path=path, img=self.process_img(imread(path)))
+            d = dict(path=path, img=self.process_img(boxx.imread(path)))
             board.find_image_points(d)
             d.pop("img")
             self[key] = d
         self.calibrate()
 
     def calibrate(self):
         self.set_xy()
@@ -96,15 +94,15 @@
         self._cache(do_cache=self.enable_cache)
         if self.save_feature_vis:
             visdir = TEMP + "/calibrating-vis-" + self.name
             print("\nSave visualization of feature points in dir:", visdir)
             os.makedirs(visdir, exist_ok=True)
             for key in tqdm(self.valid_keys):
                 d = self[key]
-                d["img"] = self.process_img(imread(d["path"]))
+                d["img"] = self.process_img(boxx.imread(d["path"]))
                 vis = d.get("board", self.board).vis(d, self)
                 boxx.imsave(visdir + "/" + key + ".jpg", vis)
                 d.pop("img")
 
     def fine_tuning_intrinsic(self, base_cam, momenta=0.5):
         """
         Fine tuning intrinsic from base_cam's K and D.
@@ -187,15 +185,15 @@
         else:
             assert set(xy) == set(self.xy), f"{xy} != {self.xy}"
         return img
 
     def set_xy(self, img=None):
         if not hasattr(self, "xy"):
             if img is None:
-                img = imread(next(iter(self.values()))["path"])
+                img = boxx.imread(next(iter(self.values()))["path"])
             self.xy = img.shape[1], img.shape[0]
         return self.xy
 
     def stereo_with(caml, camr):
         return Stereo(caml, camr)
 
     def vis_stereo(caml, camr, stereo=None, visn=1):
@@ -212,18 +210,18 @@
         stereo.shows(*stereo.rectify(imgl, imgr))
         return stereo
 
     def get_calibration_board_T(self, img_or_path_or_d, board=None):
         if isinstance(img_or_path_or_d, dict):
             d = img_or_path_or_d.copy()
             if "img" not in d:
-                d["img"] = imread(d["path"])
+                d["img"] = boxx.imread(d["path"])
         else:
             img = (
-                imread(img_or_path_or_d)
+                boxx.imread(img_or_path_or_d)
                 if isinstance(img_or_path_or_d, str)
                 else img_or_path_or_d
             )
             d = dict(img=img)
         assert d["img"].shape[:2][::-1] == self.xy
         board = self.get_board(d, board)
 
@@ -616,17 +614,17 @@
     print(Cam.load(camd.dump()))
 
     stereo = Stereo(caml, camr)
     print(stereo)
 
     T_camd_in_caml = caml.get_T_cam2_in_self(camd)
     key = caml.valid_keys_intersection(camd)[0]
-    imgl = imread(caml[key]["path"])
+    imgl = boxx.imread(caml[key]["path"])
     color_path_d = camd[key]["path"]
-    imgd = imread(color_path_d)
-    depthd = imread(color_path_d.replace("color.jpg", "depth.png"))
+    imgd = boxx.imread(color_path_d)
+    depthd = boxx.imread(color_path_d.replace("color.jpg", "depth.png"))
     depthd = np.float32(depthd / 1000)
 
     caml.vis_reproject_img_alignment(camd, depthd, imgd, imgl)
 
     depthl = caml.project_cam2_depth(camd, depthd, T_camd_in_caml)
     caml.vis_depth_alignment(imgl, depthl)
```

### Comparing `calibrating-0.6.5/calibrating/feature_libs.py` & `calibrating-0.6.6/calibrating/feature_libs.py`

 * *Files identical despite different names*

### Comparing `calibrating-0.6.5/calibrating/multi_boards.py` & `calibrating-0.6.6/calibrating/multi_boards.py`

 * *Files identical despite different names*

### Comparing `calibrating-0.6.5/calibrating/reconstruction.py` & `calibrating-0.6.6/calibrating/reconstruction.py`

 * *Files identical despite different names*

### Comparing `calibrating-0.6.5/calibrating/stereo.py` & `calibrating-0.6.6/calibrating/stereo.py`

 * *Files 18% similar despite different names*

```diff
@@ -441,37 +441,41 @@
         self.translation_rectify_img = (
             bool(max_depth)
             if translation_rectify_img is None
             else translation_rectify_img
         )
         self.max_depth = max_depth or self.MAX_DEPTH
         self.min_disparity = int(self.cam1.K[0, 0] * self.baseline / self.max_depth)
+        return self
 
     # TODO: return_unrectify_depth default False
     def get_depth(
         self, img1, img2, return_unrectify_depth=True, return_distort_depth=False
     ):
         """
         Return:
             rectify_img1
             rectify_depth
         The unit of depth is m
         """
-
+        result = {}
         assert hasattr(
             self, "stereo_matching"
         ), "Please stereo.set_stereo_matching(stereo_matching)"
         rectify_img1, rectify_img2 = self.rectify(img1, img2)
         disparity = self.stereo_matching(rectify_img1, rectify_img2)
+        if isinstance(disparity, dict):
+            result.update(disparity)
+            disparity = disparity["disparity"]
         if getattr(self, "translation_rectify_img"):
             disparity += self.min_disparity
 
         rectify_depth = self.disparity_to_depth(disparity)
 
-        result = dict(
+        result.update(
             rectify_img1=rectify_img1,
             rectify_depth=rectify_depth,
             disparity=disparity,
             rectify_img2=rectify_img2,
         )
         if return_distort_depth or return_unrectify_depth:
             unrectify_depth = self.unrectify_depth(rectify_depth)
@@ -484,119 +488,20 @@
             result.update(
                 distort_img1=img1,
                 distort_depth=self.distort_depth(unrectify_depth),
             )
         return result
 
 
-class MetaStereoMatching:
-    def __init__(self, cfg=None):
-        self.cfg = cfg
-
-    def __call__(self, img1, img2):
-        # input: RGB uint8 (h, w, 3)uint8
-        raise NotImplementedError()
-        # output: float disparity (h, w)float64, unit is m
-        # return disparity
-
-
-# A Example of StereoMatching class
-class SemiGlobalBlockMatching(MetaStereoMatching):
-    def __init__(self, cfg=None):
-        if cfg is None:
-            cfg = {}
-        self.cfg = cfg
-        self.max_size = self.cfg.get("max_size", 1000)
-
-        # StereoSGBM_create from https://gist.github.com/andijakl/ffe6e5e16742455291ef2a4edbe63cb7
-        block_size = 11
-        min_disp = 2
-        max_disp = 220
-        # Maximum disparity minus minimum disparity. The value is always greater than zero.
-        # In the current implementation, this parameter must be divisible by 16.
-        num_disp = max_disp - min_disp
-        # Margin in percentage by which the best (minimum) computed cost function value should "win" the second best value to consider the found match correct.
-        # Normally, a value within the 5-15 range is good enough
-        uniquenessRatio = 5
-        # Maximum size of smooth disparity regions to consider their noise speckles and invalidate.
-        # Set it to 0 to disable speckle filtering. Otherwise, set it somewhere in the 50-200 range.
-        speckleWindowSize = 200
-        # Maximum disparity variation within each connected component.
-        # If you do speckle filtering, set the parameter to a positive value, it will be implicitly multiplied by 16.
-        # Normally, 1 or 2 is good enough.
-        speckleRange = 2
-        disp12MaxDiff = 0
-
-        self.stereo_sgbm = cv2.StereoSGBM_create(
-            minDisparity=min_disp,
-            numDisparities=num_disp,
-            blockSize=block_size,
-            uniquenessRatio=uniquenessRatio,
-            speckleWindowSize=speckleWindowSize,
-            speckleRange=speckleRange,
-            disp12MaxDiff=disp12MaxDiff,
-            P1=8 * 1 * block_size * block_size,
-            P2=32 * 1 * block_size * block_size,
-        )
-
-    def __call__(self, img1, img2):
-        resize_ratio = min(self.max_size / max(img1.shape[:2]), 1)
-        simg1, simg2 = boxx.resize(img1, resize_ratio), boxx.resize(img2, resize_ratio)
-        sdisparity = (self.stereo_sgbm.compute(simg1, simg2).astype(np.float32)).clip(0)
-        sdisparity[sdisparity < self.stereo_sgbm.getMinDisparity() * 16] = 0
-        disparity = (
-            boxx.resize(sdisparity / 16.0, img1.shape[:2])
-            * img1.shape[1]
-            / simg1.shape[1]
-        )
-        return disparity
-
-
-class MatchingByBoard(MetaStereoMatching):
-    """
-    Stereo mathch disp by board's image_points
-    return a dense disp on calibration board
-    """
-
-    def __init__(self, board, dense_predict=True):
-        self.board = board
-        self.dense_predict = dense_predict
-
-    def __call__(self, img1, img2):
-        self.board
-        d1 = dict(img=img1)
-        self.board.find_image_points(d1)
-        image_points1 = d1["image_points"]
-        d2 = dict(img=img2)
-        self.board.find_image_points(d2)
-        image_points2 = d2["image_points"]
-
-        if isinstance(image_points1, dict):
-            image_points1 = []
-            image_points2 = []
-            for key in sorted(set(d1["image_points"]).intersection(d2["image_points"])):
-                image_points1.append(d1["image_points"][key])
-                image_points2.append(d2["image_points"][key])
-            image_points1 = np.concatenate(image_points1, 0)
-            image_points2 = np.concatenate(image_points2, 0)
-
-        rectify_std = np.std((image_points2 - image_points1)[:, 1])
-        point_disps = (image_points1 - image_points2)[:, 0]
-        xyds = np.append(image_points1, point_disps[:, None], axis=-1)
-        sparse_disp = utils.uvzs_to_arr2d(xyds, img1.shape[:2])
-        if self.dense_predict:
-            dense_disp = utils.interpolate_sparse2d(sparse_disp, "convex_hull")
-            return dense_disp
-        else:
-            return sparse_disp
-
-
 if __name__ == "__main__":
     from boxx import *
-    from calibrating import Cam
+
+    with boxx.inpkg():
+        from .camera import Cam
+        from .stereo_matching import SemiGlobalBlockMatching
 
     cam1, cam2, camd = Cam.get_test_cams()
 
     stereo = Stereo(cam1, cam2)
     print(stereo)
 
     yaml_path = "/tmp/stereo.yaml"
```

### Comparing `calibrating-0.6.5/calibrating/utils.py` & `calibrating-0.6.6/calibrating/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -289,15 +289,23 @@
 
 def interpolate_sparse2d(sparse2d, constrained_type=None, inter_type="lstsq"):
     """
     if constrained_type == True, then only interpolate convexHull area
     """
     mask_to_uvzs = (sparse2d != 0) & np.isfinite(sparse2d)
     uvzs = arr2d_to_uvzs(sparse2d, mask_to_uvzs)
-    input_mask = np.zeros_like(sparse2d, np.uint8)
+    return interpolate_uvzs(uvzs, sparse2d.shape[:2], constrained_type, inter_type)
+
+
+def interpolate_uvzs(uvzs, hw=None, constrained_type=None, inter_type="lstsq"):
+    if hw is None:
+        hw = int(uvzs[:, 1].max()) + 2, int(uvzs[:, 0].max()) + 2
+    if not uvzs.size:
+        return np.zeros(hw, uvzs.dtype)
+    input_mask = np.zeros(hw, np.uint8)
     if constrained_type is not None and constrained_type:
         convex_hull = cv2.convexHull(np.int32(uvzs[:, :2].round()))
         cv2.drawContours(input_mask, [convex_hull], -1, 1, -1)
         input_uvs = arr2d_to_uvzs(input_mask, input_mask)
     else:
         input_uvs = arr2d_to_uvzs(input_mask)
 
@@ -323,16 +331,32 @@
         A = uvzs.copy()
         A[:, 2] = 1
         lstsq_re = np.linalg.lstsq(A, uvzs[:, 2], rcond=None)
         abc = lstsq_re[0]
         output_uvzs = np.float32(input_uvs)
         output_uvzs[:, 2] = 1
         output_uvzs[:, 2] = output_uvzs @ abc
+    elif inter_type == "nearest":
+        from scipy.spatial import KDTree
+
+        # with boxx.timeit("KDTree"):
+        kdtree = KDTree(uvzs[:, :2])
+        output_uvzs = np.float32(input_uvs)
 
-    dense = uvzs_to_arr2d(output_uvzs, sparse2d.shape, arr2d=sparse2d.copy())
+        # with boxx.timeit("KDTree.query"):
+        distance, nearest_index = kdtree.query(output_uvzs[:, :2])
+        # output_uvzs[:, 2] = uvzs[nearest_index, 2]
+        distance_idx = distance < 1.5
+        output_uvzs[distance_idx, 2] = uvzs[nearest_index[distance_idx], 2]
+
+        # for i, uv in __import__("tqdm").tqdm(list(enumerate(output_uvzs[:, :2]))):
+        #     distance, nearest_index = kdtree.query(uv)
+        #     output_uvzs[i, 2] = uvzs[nearest_index, 2]
+    # dense = uvzs_to_arr2d(output_uvzs, sparse2d.shape, arr2d=sparse2d.copy())
+    dense = uvzs_to_arr2d(output_uvzs, hw)
     return dense
 
 
 def mean_Ts(Ts):
     Ts = np.array(Ts)
     Rs = Ts[:, :3, :3]
     R0 = Rs[0]
```

### Comparing `calibrating-0.6.5/calibrating.egg-info/PKG-INFO` & `calibrating-0.6.6/calibrating.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calibrating
-Version: 0.6.5
+Version: 0.6.6
 Summary: Calibrate camera's intrinsic/extristric, and build stereo depth camera with OpenCV python.
 Home-page: https://github.com/DIYer22/calibrating
 Author: DIYer22
 Author-email: ylxx@live.com
 License: UNKNOWN
 Description: Calibrate camera's intrinsic/extristric, and build stereo depth camera with OpenCV python.
 Platform: UNKNOWN
```

### Comparing `calibrating-0.6.5/setup.py` & `calibrating-0.6.6/setup.py`

 * *Files identical despite different names*

