# Comparing `tmp/calibdiff-0.1.0.tar.gz` & `tmp/calibdiff-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/calibdiff-0.1.0.tar", last modified: Mon Apr 24 11:07:33 2023, max compression
+gzip compressed data, was "dist/calibdiff-0.1.1.tar", last modified: Wed Apr 26 05:53:05 2023, max compression
```

## Comparing `calibdiff-0.1.0.tar` & `calibdiff-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2023-04-24 11:07:33.000000 calibdiff-0.1.0/
--rw-rw-r--   0 dl        (1000) dl        (1000)       35 2023-04-10 08:40:35.000000 calibdiff-0.1.0/MANIFEST.in
--rw-rw-r--   0 dl        (1000) dl        (1000)      687 2023-04-24 11:07:33.000000 calibdiff-0.1.0/PKG-INFO
--rw-rw-r--   0 dl        (1000) dl        (1000)      861 2023-04-16 14:40:41.000000 calibdiff-0.1.0/README.md
-drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2023-04-24 11:07:33.000000 calibdiff-0.1.0/calibdiff/
--rw-rw-r--   0 dl        (1000) dl        (1000)      661 2023-04-24 11:01:05.000000 calibdiff-0.1.0/calibdiff/__info__.py
--rw-rw-r--   0 dl        (1000) dl        (1000)      170 2023-04-13 11:48:03.000000 calibdiff-0.1.0/calibdiff/__init__.py
--rw-rw-r--   0 dl        (1000) dl        (1000)     1476 2023-04-14 08:01:00.000000 calibdiff-0.1.0/calibdiff/apply_rectify_on_uv.py
--rw-rw-r--   0 dl        (1000) dl        (1000)     8456 2023-04-24 11:00:47.000000 calibdiff-0.1.0/calibdiff/calibdiff_utils.py
--rw-rw-r--   0 dl        (1000) dl        (1000)     8241 2023-04-24 11:00:47.000000 calibdiff-0.1.0/calibdiff/feature_matching.py
--rw-rw-r--   0 dl        (1000) dl        (1000)     2689 2023-04-14 05:14:41.000000 calibdiff-0.1.0/calibdiff/rt_to_rectify.py
--rw-rw-r--   0 dl        (1000) dl        (1000)     7325 2023-04-24 11:05:04.000000 calibdiff-0.1.0/calibdiff/stereo_optimize.py
-drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2023-04-24 11:07:33.000000 calibdiff-0.1.0/calibdiff.egg-info/
--rw-rw-r--   0 dl        (1000) dl        (1000)      687 2023-04-24 11:07:33.000000 calibdiff-0.1.0/calibdiff.egg-info/PKG-INFO
--rw-rw-r--   0 dl        (1000) dl        (1000)      403 2023-04-24 11:07:33.000000 calibdiff-0.1.0/calibdiff.egg-info/SOURCES.txt
--rw-rw-r--   0 dl        (1000) dl        (1000)        1 2023-04-24 11:07:33.000000 calibdiff-0.1.0/calibdiff.egg-info/dependency_links.txt
--rw-rw-r--   0 dl        (1000) dl        (1000)       26 2023-04-24 11:07:33.000000 calibdiff-0.1.0/calibdiff.egg-info/requires.txt
--rw-rw-r--   0 dl        (1000) dl        (1000)       10 2023-04-24 11:07:33.000000 calibdiff-0.1.0/calibdiff.egg-info/top_level.txt
--rw-rw-r--   0 dl        (1000) dl        (1000)       26 2023-04-16 15:30:04.000000 calibdiff-0.1.0/requirements.txt
--rw-rw-r--   0 dl        (1000) dl        (1000)       38 2023-04-24 11:07:33.000000 calibdiff-0.1.0/setup.cfg
--rw-rw-r--   0 dl        (1000) dl        (1000)      957 2023-04-10 08:42:07.000000 calibdiff-0.1.0/setup.py
+drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2023-04-26 05:53:05.000000 calibdiff-0.1.1/
+-rw-rw-r--   0 dl        (1000) dl        (1000)       35 2023-04-10 08:40:35.000000 calibdiff-0.1.1/MANIFEST.in
+-rw-rw-r--   0 dl        (1000) dl        (1000)      687 2023-04-26 05:53:05.000000 calibdiff-0.1.1/PKG-INFO
+-rw-rw-r--   0 dl        (1000) dl        (1000)      861 2023-04-16 14:40:41.000000 calibdiff-0.1.1/README.md
+drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2023-04-26 05:53:05.000000 calibdiff-0.1.1/calibdiff/
+-rw-rw-r--   0 dl        (1000) dl        (1000)      661 2023-04-26 05:45:51.000000 calibdiff-0.1.1/calibdiff/__info__.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)      226 2023-04-25 05:37:11.000000 calibdiff-0.1.1/calibdiff/__init__.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)     1476 2023-04-14 08:01:00.000000 calibdiff-0.1.1/calibdiff/apply_rectify_on_uv.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)     8515 2023-04-26 05:37:39.000000 calibdiff-0.1.1/calibdiff/calibdiff_utils.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)     8391 2023-04-26 05:52:05.000000 calibdiff-0.1.1/calibdiff/feature_matching.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)     2689 2023-04-14 05:14:41.000000 calibdiff-0.1.1/calibdiff/rt_to_rectify.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)     7557 2023-04-26 05:39:26.000000 calibdiff-0.1.1/calibdiff/stereo_optimize.py
+drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2023-04-26 05:53:05.000000 calibdiff-0.1.1/calibdiff.egg-info/
+-rw-rw-r--   0 dl        (1000) dl        (1000)      687 2023-04-26 05:53:05.000000 calibdiff-0.1.1/calibdiff.egg-info/PKG-INFO
+-rw-rw-r--   0 dl        (1000) dl        (1000)      403 2023-04-26 05:53:05.000000 calibdiff-0.1.1/calibdiff.egg-info/SOURCES.txt
+-rw-rw-r--   0 dl        (1000) dl        (1000)        1 2023-04-26 05:53:05.000000 calibdiff-0.1.1/calibdiff.egg-info/dependency_links.txt
+-rw-rw-r--   0 dl        (1000) dl        (1000)       26 2023-04-26 05:53:05.000000 calibdiff-0.1.1/calibdiff.egg-info/requires.txt
+-rw-rw-r--   0 dl        (1000) dl        (1000)       10 2023-04-26 05:53:05.000000 calibdiff-0.1.1/calibdiff.egg-info/top_level.txt
+-rw-rw-r--   0 dl        (1000) dl        (1000)       26 2023-04-26 05:45:34.000000 calibdiff-0.1.1/requirements.txt
+-rw-rw-r--   0 dl        (1000) dl        (1000)       38 2023-04-26 05:53:05.000000 calibdiff-0.1.1/setup.cfg
+-rw-rw-r--   0 dl        (1000) dl        (1000)      957 2023-04-10 08:42:07.000000 calibdiff-0.1.1/setup.py
```

### Comparing `calibdiff-0.1.0/PKG-INFO` & `calibdiff-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calibdiff
-Version: 0.1.0
+Version: 0.1.1
 Summary: A PyTorch-based differential camera calibration library for intrinsic, extrinsic, and stereo camera calibration.
 Home-page: https://github.com/DIYer22/calibdiff
 Author: DIYer22
 Author-email: ylxx@live.com
 License: UNKNOWN
 Description: A PyTorch-based differential camera calibration library for intrinsic, extrinsic, and stereo camera calibration.
 Platform: UNKNOWN
```

### Comparing `calibdiff-0.1.0/README.md` & `calibdiff-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `calibdiff-0.1.0/calibdiff/__info__.py` & `calibdiff-0.1.1/calibdiff/__info__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 __description__ = "A PyTorch-based differential camera calibration library for intrinsic, extrinsic, and stereo camera calibration."
 __license__ = "MIT"
 __author__ = "DIYer22"
 __author_email__ = "ylxx@live.com"
 __maintainer__ = "DIYer22"
 __maintainer_email__ = "ylxx@live.com"
 __github_username__ = "DIYer22"
```

### Comparing `calibdiff-0.1.0/calibdiff/apply_rectify_on_uv.py` & `calibdiff-0.1.1/calibdiff/apply_rectify_on_uv.py`

 * *Files identical despite different names*

### Comparing `calibdiff-0.1.0/calibdiff/calibdiff_utils.py` & `calibdiff-0.1.1/calibdiff/calibdiff_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,15 +210,16 @@
 - if has confidence shape(n,), less confidence more tranparent
 - support img1 and img2 have different shape
 - line thickness are adaptive to img size 
 """
 
 
 def vis_matched_uvs(uvs1, uvs2, img1=None, img2=None, confidence=None):
-    if uvs1.max() > 1 and uvs2.max() > 1:
+
+    if uvs1.size and uvs1.max() > 1 and uvs2.max() > 1:
         maxx = max(uvs1.max(), uvs2.max())
         uvs1 = uvs1 / ([maxx, maxx] if img1 is None else img1.shape[:2][::-1])
         uvs2 = uvs2 / ([maxx, maxx] if img2 is None else img2.shape[:2][::-1])
     if img1 is None:
         img1 = np.zeros((1024, 1024, 3), dtype=np.uint8) + 192
     if img2 is None:
         img2 = np.zeros((1024, 1024, 3), dtype=np.uint8) + 64
@@ -232,14 +233,16 @@
         img1 = cv2.resize(img1, (new_w1, h2))
         h1, w1, _ = img1.shape
 
     # Create a black canvas with the same height as img1 and img2, and the sum of their widths
     canvas = np.zeros((h1, w1 + w2, 3), dtype=np.uint8)
     canvas[:, :w1, :] = img1
     canvas[:, w1:, :] = img2
+    if not uvs1.size:
+        return canvas
 
     if confidence is not None:
         if confidence.ndim == 1:
             confidence = np.expand_dims(confidence, axis=1)
         assert (
             uvs1.shape[0] == confidence.shape[0]
         ), "Confidence values must match the number of points in uvs1"
```

### Comparing `calibdiff-0.1.0/calibdiff/feature_matching.py` & `calibdiff-0.1.1/calibdiff/feature_matching.py`

 * *Files 4% similar despite different names*

```diff
@@ -107,25 +107,23 @@
 
 class LoftrFeatureMatching(MetaFeatureMatching):
     def __init__(self, cfg=None):
         import kornia
 
         self.kornia = kornia
         self.cfg = cfg or {}
+        self.cfg.setdefault("shape", (576, 768))
+        # self.cfg.setdefault("shape", (384, 512))
         self.device = (
             torch.device("cuda") if torch.cuda.is_available() else torch.device("cpu")
         )
         self.matcher = kornia.feature.LoFTR(pretrained="indoor_new").to(self.device)
 
     def matching_in_torch(self, th_img1, th_img2):
-        # resize_shape = (480, 640)
-        resize_shape = (768, 1024)
-        # resize_shape = (576, 768)
-        # if boxx.mg():
-        #     resize_shape = (240, 320)
+        resize_shape = self.cfg.get("shape")
 
         img1 = self.kornia.geometry.resize(th_img1, resize_shape, antialias=True)
         img2 = self.kornia.geometry.resize(th_img2, resize_shape, antialias=True)
         input_dict = {
             "image0": self.kornia.color.rgb_to_grayscale(img1).to(
                 self.device
             ),  # LofTR works on grayscale images only
@@ -167,25 +165,27 @@
         th_img2 = to_th_img(img2)
         correspondences = self.matching_in_torch(th_img1, th_img2)
 
         uvs1 = correspondences["keypoints0"].cpu().numpy()
         uvs2 = correspondences["keypoints1"].cpu().numpy()
         confidence = correspondences["confidence"].cpu().numpy()
 
-        assert uvs1.size > 20, f"Too few matched points {uvs1}"
-        Fm, inliers = cv2.findFundamentalMat(
-            uvs1 * img1.shape[:2][::-1],
-            uvs2 * img2.shape[:2][::-1],
-            cv2.USAC_MAGSAC,
-            1.0,
-            0.99995,
-            100000,
-        )
-        # TODO why 0.99 => .75 works for aruco?
-        idxs = inliers[:, 0] > -10
+        idxs = np.ones(len(uvs1), np.bool8)
+        if self.cfg.get("fundamental_mat_confidence"):
+            assert uvs1.size > 20, f"Too few matched points {uvs1}"
+            Fm, inliers = cv2.findFundamentalMat(
+                uvs1 * img1.shape[:2][::-1],
+                uvs2 * img2.shape[:2][::-1],
+                cv2.USAC_MAGSAC,
+                1.0,
+                self.cfg.get("fundamental_mat_confidence"),
+                100000,
+            )
+            # TODO why 0.99 => .75 works for aruco?
+            idxs = inliers[:, 0] > 0
         topk = self.cfg.get("topk", len(uvs1))
         if topk <= 1:
             topk = int(idxs.sum() * topk + 1)
 
         # 找到第topk个True值的索引
         true_indices = np.where(idxs)[0]
         if topk < len(true_indices):
```

### Comparing `calibdiff-0.1.0/calibdiff/rt_to_rectify.py` & `calibdiff-0.1.1/calibdiff/rt_to_rectify.py`

 * *Files identical despite different names*

### Comparing `calibdiff-0.1.0/calibdiff/stereo_optimize.py` & `calibdiff-0.1.1/calibdiff/stereo_optimize.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,16 @@
     from . import rt_to_rectify
     from .calibdiff_utils import eps, device
 
 # calibdiff_utils.set_rotate_imread_for_test()
 
 
 class StereoOptimize:
-    def __init__(self, stereo, uvs1, uvs2):
+    def __init__(self, stereo, uvs1, uvs2, cfg=None):
+        self.cfg = cfg or {}
         self.stereo = stereo
         if not all(stereo.t):
             import warnings
 
             warnings.warn(
                 f"stereo.t({stereo.t}) has zeros, try to add eps as {self.stereo.t + eps}",
                 UserWarning,
@@ -90,18 +91,22 @@
             # )/(18))**2)[loss_idx].mean()
 
             target_baseline = self.stereo.baseline
             lossd["distance"] = (
                 (target_baseline - (param["t"] ** 2 + eps).sum() ** 0.5)
                 / (target_baseline * 1 + eps)
             ) ** 2
+            if self.cfg.get("z_to_0"):
+                lossd["z_to_0"] = (
+                    (param["t"][-1] - 0) / (target_baseline * 1 + eps)
+                ) ** 2
 
             loss = sum(lossd.values())
             loss.backward()
-            if idx % 100 == 0 and 1:  # boxx.mg():
+            if idx % 100 == 0 and self.cfg.get("log", True):  # boxx.mg():
                 # print({k: v.grad for k, v in param.items()})
                 print(
                     f"Iteration {idx}: retval={strnum(retval.item())}, {', '.join([f'{k}={strnum(lossd[k])}' for k in lossd])}"
                 )
             optimizer.step()
 
         return calibrating.Stereo.load(
```

### Comparing `calibdiff-0.1.0/calibdiff.egg-info/PKG-INFO` & `calibdiff-0.1.1/calibdiff.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calibdiff
-Version: 0.1.0
+Version: 0.1.1
 Summary: A PyTorch-based differential camera calibration library for intrinsic, extrinsic, and stereo camera calibration.
 Home-page: https://github.com/DIYer22/calibdiff
 Author: DIYer22
 Author-email: ylxx@live.com
 License: UNKNOWN
 Description: A PyTorch-based differential camera calibration library for intrinsic, extrinsic, and stereo camera calibration.
 Platform: UNKNOWN
```

### Comparing `calibdiff-0.1.0/setup.py` & `calibdiff-0.1.1/setup.py`

 * *Files identical despite different names*

