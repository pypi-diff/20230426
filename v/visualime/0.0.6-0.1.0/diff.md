# Comparing `tmp/visualime-0.0.6.tar.gz` & `tmp/visualime-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "visualime-0.0.6.tar", last modified: Fri Apr 14 08:34:30 2023, max compression
+gzip compressed data, was "visualime-0.1.0.tar", last modified: Mon Apr 24 07:57:24 2023, max compression
```

## Comparing `visualime-0.0.6.tar` & `visualime-0.1.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:34:30.235718 visualime-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-04-14 08:34:15.000000 visualime-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-14 08:34:15.000000 visualime-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-04-14 08:34:30.235718 visualime-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-04-14 08:34:15.000000 visualime-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-14 08:34:15.000000 visualime-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-14 08:34:15.000000 visualime-0.0.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 08:34:30.235718 visualime-0.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:34:30.231717 visualime-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-04-14 08:34:15.000000 visualime-0.0.6/tests/test_baylime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-04-14 08:34:15.000000 visualime-0.0.6/tests/test_explain.py
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-04-14 08:34:15.000000 visualime-0.0.6/tests/test_feature_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-04-14 08:34:15.000000 visualime-0.0.6/tests/test_lime.py
--rw-r--r--   0 runner    (1001) docker     (123)    10011 2023-04-14 08:34:15.000000 visualime-0.0.6/tests/test_visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:34:30.231717 visualime-0.0.6/visualime/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-14 08:34:15.000000 visualime-0.0.6/visualime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-04-14 08:34:15.000000 visualime-0.0.6/visualime/_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-04-14 08:34:15.000000 visualime-0.0.6/visualime/baylime.py
--rw-r--r--   0 runner    (1001) docker     (123)     8105 2023-04-14 08:34:15.000000 visualime-0.0.6/visualime/explain.py
--rw-r--r--   0 runner    (1001) docker     (123)     6197 2023-04-14 08:34:15.000000 visualime-0.0.6/visualime/feature_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)    11540 2023-04-14 08:34:15.000000 visualime-0.0.6/visualime/lime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-04-14 08:34:15.000000 visualime-0.0.6/visualime/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    14849 2023-04-14 08:34:15.000000 visualime-0.0.6/visualime/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:34:30.235718 visualime-0.0.6/visualime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-04-14 08:34:30.000000 visualime-0.0.6/visualime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-14 08:34:30.000000 visualime-0.0.6/visualime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 08:34:30.000000 visualime-0.0.6/visualime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-14 08:34:30.000000 visualime-0.0.6/visualime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-14 08:34:30.000000 visualime-0.0.6/visualime.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 07:57:24.870148 visualime-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-04-24 07:57:11.000000 visualime-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-24 07:57:11.000000 visualime-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-04-24 07:57:24.870148 visualime-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-04-24 07:57:11.000000 visualime-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-04-24 07:57:11.000000 visualime-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-24 07:57:11.000000 visualime-0.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 07:57:24.870148 visualime-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 07:57:24.866147 visualime-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-04-24 07:57:11.000000 visualime-0.1.0/tests/test_baylime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-04-24 07:57:11.000000 visualime-0.1.0/tests/test_explain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-04-24 07:57:11.000000 visualime-0.1.0/tests/test_feature_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4318 2023-04-24 07:57:11.000000 visualime-0.1.0/tests/test_lime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11525 2023-04-24 07:57:11.000000 visualime-0.1.0/tests/test_visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 07:57:24.870148 visualime-0.1.0/visualime/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-24 07:57:11.000000 visualime-0.1.0/visualime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-04-24 07:57:11.000000 visualime-0.1.0/visualime/_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-04-24 07:57:11.000000 visualime-0.1.0/visualime/baylime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9975 2023-04-24 07:57:11.000000 visualime-0.1.0/visualime/explain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6197 2023-04-24 07:57:11.000000 visualime-0.1.0/visualime/feature_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11543 2023-04-24 07:57:11.000000 visualime-0.1.0/visualime/lime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-04-24 07:57:11.000000 visualime-0.1.0/visualime/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15636 2023-04-24 07:57:11.000000 visualime-0.1.0/visualime/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 07:57:24.870148 visualime-0.1.0/visualime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-04-24 07:57:24.000000 visualime-0.1.0/visualime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-24 07:57:24.000000 visualime-0.1.0/visualime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 07:57:24.000000 visualime-0.1.0/visualime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-24 07:57:24.000000 visualime-0.1.0/visualime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-24 07:57:24.000000 visualime-0.1.0/visualime.egg-info/top_level.txt
```

### Comparing `visualime-0.0.6/LICENSE` & `visualime-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `visualime-0.0.6/PKG-INFO` & `visualime-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: visualime
-Version: 0.0.6
+Version: 0.1.0
 Summary: Implementation of LIME focused on producing user-centric local explanations for image classifiers.
 Author-email: Kilian Kluge <dev@kluge.ai>, The VisuaLIME developers <xai.demonstrator@gmail.com>
 License: Apache 2.0 License
 Project-URL: Documentation, https://visualime.readthedocs.io/
 Project-URL: Repository, https://github.com/xai-demonstrator/visualime
 Project-URL: Bug Tracker, https://github.com/xai-demonstrator/visualime/issues
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `visualime-0.0.6/README.md` & `visualime-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `visualime-0.0.6/pyproject.toml` & `visualime-0.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 authors = [
     { name = "Kilian Kluge", email = "dev@kluge.ai" },
     { name = "The VisuaLIME developers", email = "xai.demonstrator@gmail.com" }
 ]
 readme = "README.md"
 license = { text = "Apache 2.0 License" }
 classifiers = [
-    "Development Status :: 3 - Alpha",
+    "Development Status :: 4 - Beta",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent"
 ]
 dynamic = ["version", "dependencies"]
 
 [project.urls]
@@ -39,11 +39,9 @@
 
 [[tool.mypy.overrides]]
 module = [
     "sklearn",
     "sklearn.*",
     "skimage",
     "skimage.*",
-    "PIL",
-    "PIL.*"
 ]
 ignore_missing_imports = true
```

### Comparing `visualime-0.0.6/tests/test_baylime.py` & `visualime-0.1.0/tests/test_baylime.py`

 * *Files identical despite different names*

### Comparing `visualime-0.0.6/tests/test_explain.py` & `visualime-0.1.0/tests/test_explain.py`

 * *Files 27% similar despite different names*

```diff
@@ -43,18 +43,52 @@
     _ = render_explanation(
         image,
         segment_mask,
         segment_weights,
         positive="green",
         negative="red",
         coverage=0.2,
+        min_num_of_segments=1,
+        max_num_of_segments=10,
+    )
+
+    _ = render_explanation(
+        image,
+        segment_mask,
+        segment_weights,
+        positive="green",
+        negative="red",
+        coverage=None,
+        num_of_segments=2,
     )
 
 
 def test_that_unknown_selection_method_raises_exception():
     with pytest.raises(ValueError):
         _, _ = explain_classification(
             image=image,
             predict_fn=predict_fn,
             num_of_samples=1,
             segment_selection_method="this-method-does-not-exist",
         )
+
+
+def test_that_either_coverage_or_num_of_segments_has_to_be_specified():
+    segment_mask = np.zeros((128, 128), dtype=int)
+    segment_weights = np.array([0])
+    with pytest.raises(ValueError):
+        _ = render_explanation(
+            image=image,
+            segment_mask=segment_mask,
+            segment_weights=segment_weights,
+            coverage=None,
+            num_of_segments=None,
+        )
+
+    with pytest.raises(ValueError):
+        _ = render_explanation(
+            image=image,
+            segment_mask=segment_mask,
+            segment_weights=segment_weights,
+            coverage=0.5,
+            num_of_segments=1,
+        )
```

### Comparing `visualime-0.0.6/tests/test_feature_selection.py` & `visualime-0.1.0/tests/test_feature_selection.py`

 * *Files identical despite different names*

### Comparing `visualime-0.0.6/tests/test_lime.py` & `visualime-0.1.0/tests/test_lime.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,20 +8,22 @@
     compute_distances,
     create_segments,
     generate_images,
     generate_samples,
     weigh_segments,
 )
 
-MAX_SEGMENT_INDEX = 25
+MAX_SEGMENT_INDEX = 24
 
 img_size_x, img_size_y = (224, 224)
 
 image = np.random.randint(0, 255, size=(img_size_x, img_size_y, 3))
-segment_mask = np.random.randint(0, MAX_SEGMENT_INDEX, size=(img_size_x, img_size_y))
+segment_mask = np.random.randint(
+    0, MAX_SEGMENT_INDEX + 1, size=(img_size_x, img_size_y)
+)
 samples = generate_samples(segment_mask, 100, p=0.5)
 
 
 def test_that_create_segments_only_accepts_known_methods():
     with pytest.raises(ValueError):
         _ = create_segments(
             image=image, segmentation_method="this-method-does-not-exist-and-never-will"
@@ -84,23 +86,58 @@
             samples=samples,
             predictions=np.zeros((samples.shape[0], 10)),
             label_idx=0,
             model_type="this-model-does-not-exist-and-never-will",
         )
 
 
-def test_segment_subset_validation_in_weigh_segments():
+def test_that_subset_indices_cannot_be_below_zero():
     with pytest.raises(ValueError):
         _ = weigh_segments(
             samples=samples,
             predictions=np.zeros((samples.shape[0], 5)),
             label_idx=0,
             segment_subset=[-5, 0, 1],
         )
 
+
+def test_that_subset_indices_cannot_be_outside_available_range():
+    assert samples.shape[1] == MAX_SEGMENT_INDEX + 1
+
+    _ = weigh_segments(
+        samples=samples,
+        predictions=np.zeros((samples.shape[0], 5)),
+        label_idx=0,
+        segment_subset=[0, 1, 2, MAX_SEGMENT_INDEX],
+    )
+
     with pytest.raises(ValueError):
         _ = weigh_segments(
             samples=samples,
             predictions=np.zeros((samples.shape[0], 5)),
             label_idx=0,
             segment_subset=[0, 1, 2, MAX_SEGMENT_INDEX + 1],
         )
+
+
+def test_that_distances_and_segment_subset_are_generated_if_not_given():
+    _ = weigh_segments(
+        samples=samples, predictions=np.zeros((samples.shape[0], 5)), label_idx=0
+    )
+
+
+def test_that_segments_not_in_segment_subset_get_zero_weight():
+    segment_subset = [1, 2, 5, 6]
+    segment_weights = weigh_segments(
+        samples=samples,
+        predictions=np.random.rand(samples.shape[0], 20),
+        label_idx=0,
+        segment_subset=segment_subset,
+    )
+
+    assert np.all(
+        [
+            weight == 0.0
+            for idx, weight in enumerate(list(segment_weights))
+            if idx not in segment_subset
+        ]
+    )
```

### Comparing `visualime-0.0.6/tests/test_visualize.py` & `visualime-0.1.0/tests/test_visualize.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import pytest
 
 from visualime.visualize import (
     _get_color,
     generate_overlay,
     mark_boundaries,
     scale_opacity,
+    scale_overlay,
     select_segments,
 )
 
 
 def test_that_either_coverage_or_num_of_segments_has_to_be_specified():
     segment_mask = np.zeros((128, 128), dtype=int)
     segment_weights = np.array([0])
@@ -34,22 +35,48 @@
             segment_weights=segment_weights,
             num_of_segments=1,
             min_coverage=0.8,
             max_coverage=0.2,
         )
 
 
+def test_that_min_coverage_cannot_equal_max_coverage():
+    segment_mask = np.zeros((128, 128), dtype=int)
+    segment_weights = np.array([0])
+    with pytest.raises(ValueError):
+        _ = select_segments(
+            segment_mask=segment_mask,
+            segment_weights=segment_weights,
+            num_of_segments=1,
+            min_coverage=0.8,
+            max_coverage=0.8,
+        )
+
+
 def test_that_min_num_of_segments_has_to_be_smaller_than_max_num_of_segments():
     segment_mask = np.zeros((128, 128), dtype=int)
     segment_weights = np.array([0])
     with pytest.raises(ValueError):
         _ = select_segments(
             segment_mask=segment_mask,
             segment_weights=segment_weights,
             coverage=0.5,
+            min_num_of_segments=15,
+            max_num_of_segments=5,
+        )
+
+
+def test_that_min_num_of_segments_cannot_equal_max_num_of_segments():
+    segment_mask = np.zeros((128, 128), dtype=int)
+    segment_weights = np.array([0])
+    with pytest.raises(ValueError):
+        _ = select_segments(
+            segment_mask=segment_mask,
+            segment_weights=segment_weights,
+            coverage=0.5,
             min_num_of_segments=5,
             max_num_of_segments=5,
         )
 
 
 def test_that_each_segment_needs_a_weight():
     segment_mask = np.zeros((128, 128), dtype=int)
@@ -146,15 +173,18 @@
     segment_mask[12:24, 12:24] = 2
     segment_mask[99, 101] = 3
 
     overlay = generate_overlay(
         segment_mask=segment_mask, segments_to_color=[1, 3], color="blue", opacity=1.0
     )
 
+    # basic properties
     assert overlay.shape == (128, 128, 4)
+    assert np.min(overlay) == 0
+    assert np.max(overlay) == 255
     assert np.any(overlay[:, :, 3] == 255)
     # segment 1 is colored in blue
     assert np.all(overlay[5, 5:8, 2:4] == 255)
     assert np.all(overlay[5, 5:8, 0:2] == 0)
     # segment 2 is not colored
     assert np.all(overlay[12:24, 12:24] == 0)
     # segment 3 is colored in blue
@@ -281,14 +311,39 @@
             segment_mask=segment_mask,
             segment_weights=segment_weights,
             segments_to_color=segments_to_color,
             relative_to="this-option-does-not-exist-and-never-will",
         )
 
 
+def test_scale_overlay():
+    segment_mask = np.zeros((10, 10), dtype=int)
+    segment_mask[2, 2:2] = 1
+    segment_mask[3, 2:3] = 1
+    segment_mask[4, 2:4] = 1
+    segment_mask[5, 2:5] = 1
+    segment_mask[6, 2:6] = 1
+
+    segments_to_color = [1]
+    color = "red"
+    opacity = 1.0
+
+    overlay = generate_overlay(
+        segment_mask=segment_mask,
+        segments_to_color=segments_to_color,
+        color=color,
+        opacity=opacity,
+    )
+    # show the overlay
+
+    scaled_overlay = scale_overlay(overlay=overlay, shape=(100, 100))
+
+    assert scaled_overlay.shape == (100, 100, 4)
+
+
 @pytest.mark.parametrize(
     "color_name,rgb",
     [("green", [0, 128, 0]), ("magenta", [255, 0, 255]), ("purple", [128, 0, 128])],
 )
 def test_that_color_can_be_obtained_by_name(color_name, rgb):
     assert np.array_equal(_get_color(color_name, 1.0), np.array(rgb + [255]))
```

### Comparing `visualime-0.0.6/visualime/_models.py` & `visualime-0.1.0/visualime/_models.py`

 * *Files identical despite different names*

### Comparing `visualime-0.0.6/visualime/baylime.py` & `visualime-0.1.0/visualime/baylime.py`

 * *Files identical despite different names*

### Comparing `visualime-0.0.6/visualime/explain.py` & `visualime-0.1.0/visualime/explain.py`

 * *Files 16% similar despite different names*

```diff
@@ -140,22 +140,33 @@
     return segment_mask, segment_weights
 
 
 def render_explanation(
     image: np.ndarray,
     segment_mask: np.ndarray,
     segment_weights: np.ndarray,
+    *,
     positive: Optional[Union[Tuple[int, int, int], str]] = "green",
     negative: Optional[Union[Tuple[int, int, int], str]] = None,
     opacity: float = 0.7,
-    coverage: float = 0.2,
+    coverage: Optional[float] = 0.2,
+    num_of_segments: Optional[int] = None,
+    min_num_of_segments: int = 0,
+    max_num_of_segments: Optional[int] = None,
 ) -> PIL_Image:
     """Render a visual explanation from the `segment_mask` and `segment_weights`
     produced by :meth:`visualime.explain.explain_classification`.
 
+    Segments are selected in the order of descending weight until the desired `coverage`
+    or `num_of_segments` is reached.
+    Exactly one of these parameters has to be specified when calling the function.
+
+    If both 'positive' and 'negative' colors are specified, the 'coverage' or
+    `num_of_segments` will be distributed evenly between the two classes of segments.
+
     Parameters
     ----------
     image : np.ndarray
         The image to explain the classification for as a three-dimensional array
         of shape `(image_width, image_height, 3)` representing an RGB image.
 
     segment_mask : np.ndarray
@@ -173,33 +184,64 @@
     negative : str or int 3-tuple (RGB), optional
         The color for the segments that contribute negatively towards the classification.
         If `None` (the default), these segments are not colored.
 
     opacity : float, default 0.7
         The opacity of the explanation overlay.
 
-    coverage : float, default 0.2
+    coverage : float, optional, default 0.2
         The coverage of each overlay relative to the area of the image.
         E.g., if set to 0.2 (the default), about 20% of the image are colored.
 
+    num_of_segments : int, optional
+        The number of segments to be colored.
+
+    min_num_of_segments : int, default 0
+        The minimum number of segments to be colored.
+
+    max_num_of_segments : int, optional
+        The maximum number of segments to be colored.
+
     Returns
     -------
     PIL.Image
         The rendered explanation as a PIL Image object.
 
     Examples
     --------
     TODO: Add end-to-end example
     """
+    if coverage is None and num_of_segments is None:
+        raise ValueError("Either coverage or num_of_segments has to be specified.")
+
+    if coverage is not None and num_of_segments is not None:
+        raise ValueError("Only either coverage or num_of_segments can be given.")
+
+    if positive is not None and negative is not None:
+        if coverage is not None:
+            coverage /= 2
+        if num_of_segments is not None:
+            num_of_segments = max(num_of_segments // 2, 1)
+        if min_num_of_segments is not None:
+            min_num_of_segments = max(min_num_of_segments // 2, 0)
+        if max_num_of_segments is not None:
+            max_num_of_segments = max(max_num_of_segments // 2, 1)
+
     final_img = Image.fromarray(image.astype(np.uint8), "RGB").convert("RGBA")
 
     if positive is not None:
         positive_segments = select_segments(
-            segment_weights, segment_mask, coverage=coverage
+            segment_weights,
+            segment_mask,
+            coverage=coverage,
+            num_of_segments=num_of_segments,
+            min_num_of_segments=min_num_of_segments,
+            max_num_of_segments=max_num_of_segments,
         )
+
         positive_overlay = generate_overlay(
             segment_mask, positive_segments, color=positive, opacity=opacity
         )
 
         positive_overlay = scale_opacity(
             overlay=positive_overlay,
             segment_weights=segment_weights,
@@ -209,15 +251,20 @@
         )
 
         overlay_image = Image.fromarray(positive_overlay.astype(np.uint8), "RGBA")
         final_img.alpha_composite(overlay_image)
 
     if negative is not None:
         negative_segments = select_segments(
-            -segment_weights, segment_mask, coverage=coverage
+            -segment_weights,
+            segment_mask,
+            coverage=coverage,
+            num_of_segments=num_of_segments,
+            min_num_of_segments=min_num_of_segments,
+            max_num_of_segments=max_num_of_segments,
         )
         negative_overlay = generate_overlay(
             segment_mask, negative_segments, color=negative, opacity=opacity
         )
 
         negative_overlay = scale_opacity(
             overlay=negative_overlay,
```

### Comparing `visualime-0.0.6/visualime/feature_selection.py` & `visualime-0.1.0/visualime/feature_selection.py`

 * *Files identical despite different names*

### Comparing `visualime-0.0.6/visualime/lime.py` & `visualime-0.1.0/visualime/lime.py`

 * *Files 1% similar despite different names*

```diff
@@ -294,15 +294,15 @@
     if distances is None:
         distances = cosine_distance(samples)
     sample_weight = kernel(distances)
 
     if segment_subset is not None:
         if min(segment_subset) < 0:
             raise ValueError("Indices in segment subset cannot be below 0.")
-        if max(segment_subset) > samples.shape[1]:
+        if max(segment_subset) >= samples.shape[1]:
             raise ValueError(
                 "Indices in segment subset exceed number of available segments."
             )
         reduced_samples = samples[:, segment_subset]
     else:
         reduced_samples = samples
         segment_subset = list(range(samples.shape[1]))
@@ -311,25 +311,25 @@
         reduced_samples, predictions[:, label_idx], sample_weight=sample_weight
     )
 
     reduced_weights = list(linear_model.coef_)
 
     segment_weights = np.array(
         [
-            reduced_weights[segment_subset.index(feature_idx)]
-            if feature_idx in segment_subset
+            reduced_weights[segment_subset.index(segment_idx)]
+            if segment_idx in segment_subset
             else 0.0
-            for feature_idx in range(samples.shape[1])
+            for segment_idx in range(samples.shape[1])
         ]
     )
 
     return segment_weights
 
 
-weigh_segments.__doc__ = f"""Generating list of coefficients to weigh segments.
+weigh_segments.__doc__ = f"""Generate the list of coefficients to weigh segments.
 
     Parameters
     ----------
     {SAMPLES_PREDICTIONS_LABEL_IDX_DOC}
 
     {MODEL_TYPE_PARAMS_DOC}
```

### Comparing `visualime-0.0.6/visualime/metrics.py` & `visualime-0.1.0/visualime/metrics.py`

 * *Files identical despite different names*

### Comparing `visualime-0.0.6/visualime/visualize.py` & `visualime-0.1.0/visualime/visualize.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import warnings
 from typing import List, Literal, Optional, Tuple, Union
 
 import numpy as np
 from PIL.ImageColor import getrgb
+from skimage.transform import resize
 
 
 def select_segments(
     segment_weights: np.ndarray,
     segment_mask: np.ndarray,
     coverage: Optional[float] = None,
     num_of_segments: Optional[int] = None,
@@ -158,25 +159,27 @@
 
 
 def _get_color(color: Union[str, Tuple[int, int, int]], opacity: float) -> np.ndarray:
     """Convert a color specified by name or RGB tuple into an RGBA color.
 
     Note that `color` can also be an RGB(A) string in various formats.
     """
+    rgb_color: Union[Tuple[int, int, int], Tuple[int, int, int, int]]
+
     if isinstance(color, str):
         try:
-            parsed_color = getrgb(color)
+            rgb_color = getrgb(color)
         except ValueError:
             raise ValueError(
                 f"Unknown color '{color}'. See documentation for available colors."
             )
-        else:
-            color = parsed_color
+    else:
+        rgb_color = color
 
-    _rgba = np.array(list(color[:3]) + [int(255 * opacity)]).astype(int)
+    _rgba = np.array(list(rgb_color[:3]) + [int(255 * opacity)]).astype(int)
 
     if np.any(_rgba < 0) or np.any(_rgba > 255):
         raise ValueError(
             f"Channel values must be between 0 and 255. Got {tuple(_rgba)} instead."
         )
 
     return _rgba
@@ -314,14 +317,36 @@
     for segment_id in segments_to_color:
         mask = segment_mask == segment_id
         new_overlay[mask, 3] = new_opacity[segment_id]
 
     return new_overlay
 
 
+def scale_overlay(overlay: np.ndarray, shape: Tuple[int, int]) -> np.ndarray:
+    """Scale the overlay to a given size.
+
+    Parameters
+    ----------
+    overlay : np.ndarray
+        The output of :meth:`visualime.visualize.generate_overlay`:
+        An array of shape `(image_width, image_height, 4)` representing an RGBA image.
+
+    shape : tuple of ints
+        The size to scale the overlay to.
+
+    Returns
+    -------
+    np.ndarray
+        An array of shape `(image_width, image_height, 4)` representing an RGBA image.
+
+        Note that this function does not modify the original `overlay` but returns a new array.
+    """
+    return resize(overlay, shape, preserve_range=True)
+
+
 def mark_boundaries(
     image: np.ndarray,
     segment_mask: np.ndarray,
     color: Union[str, Tuple[int, int, int]] = "red",
     opacity: float = 1.0,
 ) -> np.ndarray:
     """Mark the boundaries of the segments in the image.
```

### Comparing `visualime-0.0.6/visualime.egg-info/PKG-INFO` & `visualime-0.1.0/visualime.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: visualime
-Version: 0.0.6
+Version: 0.1.0
 Summary: Implementation of LIME focused on producing user-centric local explanations for image classifiers.
 Author-email: Kilian Kluge <dev@kluge.ai>, The VisuaLIME developers <xai.demonstrator@gmail.com>
 License: Apache 2.0 License
 Project-URL: Documentation, https://visualime.readthedocs.io/
 Project-URL: Repository, https://github.com/xai-demonstrator/visualime
 Project-URL: Bug Tracker, https://github.com/xai-demonstrator/visualime/issues
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `visualime-0.0.6/visualime.egg-info/SOURCES.txt` & `visualime-0.1.0/visualime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

