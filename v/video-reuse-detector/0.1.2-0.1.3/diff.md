# Comparing `tmp/video_reuse_detector-0.1.2.tar.gz` & `tmp/video_reuse_detector-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "video_reuse_detector-0.1.2.tar", max compression
+gzip compressed data, was "video_reuse_detector-0.1.3.tar", max compression
```

## Comparing `video_reuse_detector-0.1.2.tar` & `video_reuse_detector-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rwxr-xr-x   0        0        0      473 2023-03-16 11:59:24.538884 video_reuse_detector-0.1.2/README.md
--rw-r--r--   0        0        0      557 2023-03-16 12:07:20.528132 video_reuse_detector-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-10 13:15:34.586534 video_reuse_detector-0.1.2/vrd/__init__.py
--rw-r--r--   0        0        0     7108 2023-03-10 13:15:34.586534 video_reuse_detector-0.1.2/vrd/annotation_matcher.py
--rw-r--r--   0        0        0     8582 2023-03-10 13:15:34.586534 video_reuse_detector-0.1.2/vrd/dbhandler.py
--rw-r--r--   0        0        0    10226 2023-03-16 12:02:09.580704 video_reuse_detector-0.1.2/vrd/faiss_helper.py
--rw-r--r--   0        0        0     9168 2023-03-10 13:15:34.586534 video_reuse_detector-0.1.2/vrd/frame_extractor.py
--rw-r--r--   0        0        0     4528 2023-03-16 11:59:49.747162 video_reuse_detector-0.1.2/vrd/image_preprocessing.py
--rw-r--r--   0        0        0     3939 2023-03-16 12:04:47.942450 video_reuse_detector-0.1.2/vrd/keras_layer_helper.py
--rw-r--r--   0        0        0    35384 2023-03-10 13:15:34.586534 video_reuse_detector-0.1.2/vrd/neighbours.py
--rw-r--r--   0        0        0     1853 2023-03-16 12:02:09.504703 video_reuse_detector-0.1.2/vrd/neural_networks.py
--rw-r--r--   0        0        0    28571 2023-03-16 12:02:09.740706 video_reuse_detector-0.1.2/vrd/notebook_helper.py
--rw-r--r--   0        0        0    30541 2023-03-16 10:48:57.684639 video_reuse_detector-0.1.2/vrd/overlap_calculator.py
--rw-r--r--   0        0        0    18983 2023-03-16 12:03:06.181328 video_reuse_detector-0.1.2/vrd/sequence_finder.py
--rw-r--r--   0        0        0    13450 2023-03-16 12:02:09.604704 video_reuse_detector-0.1.2/vrd/vrd_project.py
--rw-r--r--   0        0        0        0 2023-03-10 13:15:34.586534 video_reuse_detector-0.1.2/vrd/widgets/__init__.py
--rw-r--r--   0        0        0     5045 2023-03-10 13:15:34.586534 video_reuse_detector-0.1.2/vrd/widgets/manual_image_preview.py
--rw-r--r--   0        0        0     4145 2023-03-10 13:15:34.586534 video_reuse_detector-0.1.2/vrd/widgets/sequences_w_lowest_distance_by_duration.py
--rw-r--r--   0        0        0     4572 2023-03-10 13:15:34.586534 video_reuse_detector-0.1.2/vrd/widgets/sequences_w_lowest_distances.py
--rw-r--r--   0        0        0     1349 1970-01-01 00:00:00.000000 video_reuse_detector-0.1.2/PKG-INFO
+-rwxr-xr-x   0        0        0      473 2023-03-16 11:59:24.538884 video_reuse_detector-0.1.3/README.md
+-rw-r--r--   0        0        0      557 2023-04-26 13:27:56.653126 video_reuse_detector-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-10 13:15:34.586534 video_reuse_detector-0.1.3/vrd/__init__.py
+-rw-r--r--   0        0        0     7108 2023-03-10 13:15:34.586534 video_reuse_detector-0.1.3/vrd/annotation_matcher.py
+-rw-r--r--   0        0        0     8582 2023-03-10 13:15:34.586534 video_reuse_detector-0.1.3/vrd/dbhandler.py
+-rw-r--r--   0        0        0    10226 2023-03-16 12:02:09.580704 video_reuse_detector-0.1.3/vrd/faiss_helper.py
+-rw-r--r--   0        0        0     9168 2023-03-10 13:15:34.586534 video_reuse_detector-0.1.3/vrd/frame_extractor.py
+-rw-r--r--   0        0        0     4528 2023-03-16 11:59:49.747162 video_reuse_detector-0.1.3/vrd/image_preprocessing.py
+-rw-r--r--   0        0        0     3939 2023-03-16 12:04:47.942450 video_reuse_detector-0.1.3/vrd/keras_layer_helper.py
+-rw-r--r--   0        0        0    35384 2023-03-10 13:15:34.586534 video_reuse_detector-0.1.3/vrd/neighbours.py
+-rw-r--r--   0        0        0     1853 2023-03-16 12:02:09.504703 video_reuse_detector-0.1.3/vrd/neural_networks.py
+-rw-r--r--   0        0        0    28571 2023-03-16 12:02:09.740706 video_reuse_detector-0.1.3/vrd/notebook_helper.py
+-rw-r--r--   0        0        0    30541 2023-03-16 10:48:57.684639 video_reuse_detector-0.1.3/vrd/overlap_calculator.py
+-rw-r--r--   0        0        0    21750 2023-04-26 13:10:06.029443 video_reuse_detector-0.1.3/vrd/sequence_finder.py
+-rw-r--r--   0        0        0    13450 2023-03-16 12:02:09.604704 video_reuse_detector-0.1.3/vrd/vrd_project.py
+-rw-r--r--   0        0        0        0 2023-03-10 13:15:34.586534 video_reuse_detector-0.1.3/vrd/widgets/__init__.py
+-rw-r--r--   0        0        0     5045 2023-03-10 13:15:34.586534 video_reuse_detector-0.1.3/vrd/widgets/manual_image_preview.py
+-rw-r--r--   0        0        0     4145 2023-03-10 13:15:34.586534 video_reuse_detector-0.1.3/vrd/widgets/sequences_w_lowest_distance_by_duration.py
+-rw-r--r--   0        0        0     4572 2023-03-10 13:15:34.586534 video_reuse_detector-0.1.3/vrd/widgets/sequences_w_lowest_distances.py
+-rw-r--r--   0        0        0     1349 1970-01-01 00:00:00.000000 video_reuse_detector-0.1.3/PKG-INFO
```

### Comparing `video_reuse_detector-0.1.2/pyproject.toml` & `video_reuse_detector-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "video-reuse-detector"
-version = "0.1.2"
+version = "0.1.3"
 description = "The video reuse detector"
 authors = ["TomasSkotare <tomas.skotare@umu.se>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "vrd"}]
 
 [tool.poetry.dependencies]
```

### Comparing `video_reuse_detector-0.1.2/vrd/annotation_matcher.py` & `video_reuse_detector-0.1.3/vrd/annotation_matcher.py`

 * *Files identical despite different names*

### Comparing `video_reuse_detector-0.1.2/vrd/dbhandler.py` & `video_reuse_detector-0.1.3/vrd/dbhandler.py`

 * *Files identical despite different names*

### Comparing `video_reuse_detector-0.1.2/vrd/faiss_helper.py` & `video_reuse_detector-0.1.3/vrd/faiss_helper.py`

 * *Files identical despite different names*

### Comparing `video_reuse_detector-0.1.2/vrd/frame_extractor.py` & `video_reuse_detector-0.1.3/vrd/frame_extractor.py`

 * *Files identical despite different names*

### Comparing `video_reuse_detector-0.1.2/vrd/image_preprocessing.py` & `video_reuse_detector-0.1.3/vrd/image_preprocessing.py`

 * *Files identical despite different names*

### Comparing `video_reuse_detector-0.1.2/vrd/keras_layer_helper.py` & `video_reuse_detector-0.1.3/vrd/keras_layer_helper.py`

 * *Files identical despite different names*

### Comparing `video_reuse_detector-0.1.2/vrd/neighbours.py` & `video_reuse_detector-0.1.3/vrd/neighbours.py`

 * *Files identical despite different names*

### Comparing `video_reuse_detector-0.1.2/vrd/neural_networks.py` & `video_reuse_detector-0.1.3/vrd/neural_networks.py`

 * *Files identical despite different names*

### Comparing `video_reuse_detector-0.1.2/vrd/notebook_helper.py` & `video_reuse_detector-0.1.3/vrd/notebook_helper.py`

 * *Files identical despite different names*

### Comparing `video_reuse_detector-0.1.2/vrd/overlap_calculator.py` & `video_reuse_detector-0.1.3/vrd/overlap_calculator.py`

 * *Files identical despite different names*

### Comparing `video_reuse_detector-0.1.2/vrd/sequence_finder.py` & `video_reuse_detector-0.1.3/vrd/sequence_finder.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,47 +4,54 @@
 """
 import sys
 import time
 
 import numpy as np
 import pandas as pd
 import PIL
+from PIL import ImageDraw
 
 try:
     from IPython.display import display
+    from IPython.display import Image as ipy_image
 except:
     pass
 
+from io import BytesIO
+
 from scipy.sparse import lil_matrix, triu
 from tqdm.auto import tqdm
 
 from vrd.vrd_project import VRDProject
 
-from . import frame_extractor, neighbours
+from . import neighbours
 
 sys.path.append("..")
 
 
 class SequenceFinder:
     """Finds sequences (frames matching second-per-second) from a given neighbours class."""
 
     sequence_lil_matrix: lil_matrix
     shortest_allowed_sequence: int
     max_distance: int
     neigh: neighbours.Neighbours
+    pandas_background: str
 
     def __init__(
         self,
         neigh: neighbours.Neighbours,
         max_distance=30000,
         shortest_allowed_sequence=3,
+        pandas_background=None,
     ) -> None:
         self.neigh = neigh
         self.max_distance = max_distance
         self.shortest_allowed_sequence = shortest_allowed_sequence
+        self.pandas_background = pandas_background
 
         matrix = self._calculate_sequence_matrix(max_distance=max_distance)
         # Make upper triangular
         matrix = triu(matrix + matrix.T)
         self.sequence_lil_matrix_distance = matrix.tolil()
         self.sequence_lil_matrix = self.sequence_lil_matrix_distance.astype(np.bool8)
 
@@ -337,26 +344,32 @@
     def show_notebook_sequence(
         self,
         sequences,
         show_limit: int = None,
         show_shift=False,
         frame_resize=(30, 30),
         sort_order: callable = None,
+        convert_format=None,
+        pandas_background=None,
     ):
         """Displays longest-to-shortest sequences in a notebook
 
         Args:
             sequences (list): The sequence list of tuples (start1, start2, duration)
             show_limit (int, optional): The maximum number of sequences to show (Default: all)
             show_shift (bool, optional): Show statistics for "shifting", i.e. moving the matches one or 
                 several seconds forward or backwards.
             frame_resize (tuple, optional): Size of the thumbnails of each frame
             sort_order (callable): A handler that can sort or filter the sequence list.
+            convert_format: The image format to return, for example "jpeg" to save space.
+            pandas_background: Override background color of pandas to this value
         """
         frames = self.neigh.frames
+        if pandas_background is None:
+            pandas_background = self.pandas_background
 
         if sort_order is None:
             # Default: Sort by duration
             sequences = sorted(sequences, key=lambda x: x[2], reverse=True)
         else:
             sequences = sort_order(sequences)
 
@@ -392,21 +405,40 @@
                     "Index": start2,
                     "Match mean distance": dist_mean,
                     "# not matching": dist_zeros,
                 },
             ]
             df = pd.DataFrame(pd_data).set_index("Video")
             df = df.style.set_caption(f"Sequence no. {idx}:")
+            if pandas_background:
+                headers = {
+                    "selector": "tr:not(.col_trim)",
+                    "props": f"background-color: {pandas_background};",
+                }
+                df = df.set_properties(**{"background-color": pandas_background})
+                df = df.set_table_styles([headers])
             display(df)
 
-            display(
-                self.show_sequence(
-                    start1, start2, duration, frames, frame_resize=frame_resize
-                )
+            img = self.show_sequence(
+                start1, start2, duration, frames, frame_resize=frame_resize
             )
+            if convert_format:
+                img_bytes = BytesIO()
+                try:
+                    img.save(img_bytes, format=convert_format)
+                except Exception as e: # This should be OSError only, but that didn't work
+                    # Likely can't handle transparency, try again
+                    if img.mode in ("RGBA", "P"):
+                        img = img.convert("RGB")
+                    img.save(img_bytes, format=convert_format)
+
+                to_show = ipy_image(img_bytes.getvalue())
+            else:
+                to_show = img
+            display(to_show)
 
     def get_sequence_mean_distance(self, start1, start2, duration):
         res_arr = np.zeros(duration, dtype=np.float32)
         for i in range(duration):
             res_arr[i] = self.sequence_lil_matrix_distance[start2 + i, start1 + i]
         nonzeros = res_arr[np.where(res_arr > 0)[0]]
         dist_mean = np.mean(nonzeros) if len(nonzeros) > 0 else np.nan
@@ -426,19 +458,14 @@
             dist_mean = np.mean(nonzeros) if len(nonzeros) > 0 else np.nan
             dist_zeros = np.sum(res_arr == 0)
             shift_results.append(
                 {"Shift": shift, "Mean": dist_mean, "Zeros": dist_zeros}
             )
         df = pd.DataFrame(shift_results).set_index("Shift")
         display(df)
-        # if minimize_nonmatch:
-        #     df = df[df.Zeros == df.Zeros.min()]
-        #     if len(df > 1):
-        #         df = df[df.Mean == df.Mean.min()]
-        #     start1 -= df.reset_index().Shift.values[0]
 
     @staticmethod
     def remove_unwanted_sequences(sequences, project: VRDProject, excel_file: str):
         """ Removes unwanted sequences. The unwanted sequences are defined in an excel file,
         containing the columns:
                 'Video': The video name
                 'Start time': The start time in a string, formatted as HH:MM:SS 
@@ -478,35 +505,74 @@
             del sequences[seq_index]
 
     @staticmethod
     def show_sequence(
         start1: int,
         start2: int,
         duration: int,
-        frames: frame_extractor.FrameExtractor,
-        frame_resize=(200, 200),
+        frames,
+        frame_resize=(90, 70),
+        row_max_width=700,
+        row_spacing=10,
+        background_opacity=0,
     ):
         """Generates a comparison image for a given sequence
 
         Args:
             start1 (int): Start time 1 (as related to the Frame)
             start2 (int): _description_
             duration (int): _description_
             frames (FrameExtractor): _description_
             frame_resize (tuple, optional): Size of each resulting image in the sequence. Defaults to (200, 200).
+            row_max_width: The maximum number of pixels allowed for one row. If this value is exceeded 
+                (i.e. width * # frames), the rows are broken up into several rows
+            row_spacing: The number of pixels between each row (if any)
+            background_opacity: The opacity of the unused pixels (if any)
 
         Returns:
             A PIL image with the whole sequence
         """
 
         images = frames.all_images
+        width, height = frame_resize
+        max_width = width * duration
+        if max_width > row_max_width:
+            per_row = np.floor(row_max_width / width).astype(int)
+            no_rows = np.ceil(duration / per_row).astype(int)
+        else:
+            per_row = duration
+            no_rows = 1
+        row_spacing_pixels = row_spacing * (no_rows - 1)
 
         merged = PIL.Image.new(
-            "RGB", (frame_resize[0] * duration, frame_resize[1] * 2), (250, 250, 250)
+            "RGBA",
+            (width * per_row, height * 2 * no_rows + row_spacing_pixels),
+            (250, 250, 250, background_opacity),
         )
-
+        draw = ImageDraw.Draw(merged)
         for i in range(0, duration):
             img1 = PIL.Image.open(images[start1 + i]).resize(frame_resize)
             img2 = PIL.Image.open(images[start2 + i]).resize(frame_resize)
-            merged.paste(img1, (frame_resize[0] * i, 0))
-            merged.paste(img2, (frame_resize[0] * i, frame_resize[1]))
+            current_row = np.floor(i / per_row).astype(int)
+            image_column = i % per_row
+            merged.paste(
+                img1,
+                (
+                    width * image_column,
+                    current_row * row_spacing + current_row * 2 * height,
+                ),
+            )
+            merged.paste(
+                img2,
+                (
+                    width * image_column,
+                    current_row * row_spacing + current_row * 2 * height + height,
+                ),
+            )
+            if i > 0 and image_column == 0:
+                y_loc = current_row * height * 2 + (current_row - 1) * row_spacing
+                draw.text(
+                    (10, y_loc),
+                    f"Frames {i+1}-{i + np.min([duration-i, per_row])}",
+                    fill=(0, 0, 0),
+                )
         return merged
```

### Comparing `video_reuse_detector-0.1.2/vrd/vrd_project.py` & `video_reuse_detector-0.1.3/vrd/vrd_project.py`

 * *Files identical despite different names*

### Comparing `video_reuse_detector-0.1.2/vrd/widgets/manual_image_preview.py` & `video_reuse_detector-0.1.3/vrd/widgets/manual_image_preview.py`

 * *Files identical despite different names*

### Comparing `video_reuse_detector-0.1.2/vrd/widgets/sequences_w_lowest_distance_by_duration.py` & `video_reuse_detector-0.1.3/vrd/widgets/sequences_w_lowest_distance_by_duration.py`

 * *Files identical despite different names*

### Comparing `video_reuse_detector-0.1.2/vrd/widgets/sequences_w_lowest_distances.py` & `video_reuse_detector-0.1.3/vrd/widgets/sequences_w_lowest_distances.py`

 * *Files identical despite different names*

### Comparing `video_reuse_detector-0.1.2/PKG-INFO` & `video_reuse_detector-0.1.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: video-reuse-detector
-Version: 0.1.2
+Version: 0.1.3
 Summary: The video reuse detector
 License: MIT
 Author: TomasSkotare
 Author-email: tomas.skotare@umu.se
 Requires-Python: >=3.7,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

