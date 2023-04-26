# Comparing `tmp/face-crop-plus-1.0.2.tar.gz` & `tmp/face-crop-plus-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "face-crop-plus-1.0.2.tar", last modified: Sun Apr 23 13:55:38 2023, max compression
+gzip compressed data, was "face-crop-plus-1.0.3.tar", last modified: Wed Apr 26 19:24:41 2023, max compression
```

## Comparing `face-crop-plus-1.0.2.tar` & `face-crop-plus-1.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:55:38.096177 face-crop-plus-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-23 13:55:27.000000 face-crop-plus-1.0.2/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)    23703 2023-04-23 13:55:38.096177 face-crop-plus-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22696 2023-04-23 13:55:27.000000 face-crop-plus-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 13:55:38.096177 face-crop-plus-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-23 13:55:27.000000 face-crop-plus-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:55:38.092177 face-crop-plus-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:55:38.092177 face-crop-plus-1.0.2/src/face_crop_plus/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-23 13:55:27.000000 face-crop-plus-1.0.2/src/face_crop_plus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10366 2023-04-23 13:55:27.000000 face-crop-plus-1.0.2/src/face_crop_plus/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42905 2023-04-23 13:55:27.000000 face-crop-plus-1.0.2/src/face_crop_plus/cropper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:55:38.096177 face-crop-plus-1.0.2/src/face_crop_plus/models/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-23 13:55:27.000000 face-crop-plus-1.0.2/src/face_crop_plus/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13019 2023-04-23 13:55:27.000000 face-crop-plus-1.0.2/src/face_crop_plus/models/_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    19842 2023-04-23 13:55:27.000000 face-crop-plus-1.0.2/src/face_crop_plus/models/bise.py
--rw-r--r--   0 runner    (1001) docker     (123)    21126 2023-04-23 13:55:27.000000 face-crop-plus-1.0.2/src/face_crop_plus/models/retinaface.py
--rw-r--r--   0 runner    (1001) docker     (123)     6289 2023-04-23 13:55:27.000000 face-crop-plus-1.0.2/src/face_crop_plus/models/rrdb.py
--rw-r--r--   0 runner    (1001) docker     (123)    11459 2023-04-23 13:55:27.000000 face-crop-plus-1.0.2/src/face_crop_plus/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:55:38.092177 face-crop-plus-1.0.2/src/face_crop_plus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23703 2023-04-23 13:55:38.000000 face-crop-plus-1.0.2/src/face_crop_plus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-23 13:55:38.000000 face-crop-plus-1.0.2/src/face_crop_plus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 13:55:38.000000 face-crop-plus-1.0.2/src/face_crop_plus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-23 13:55:38.000000 face-crop-plus-1.0.2/src/face_crop_plus.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-23 13:55:38.000000 face-crop-plus-1.0.2/src/face_crop_plus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-23 13:55:38.000000 face-crop-plus-1.0.2/src/face_crop_plus.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:24:41.804395 face-crop-plus-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-26 19:24:24.000000 face-crop-plus-1.0.3/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)    23699 2023-04-26 19:24:41.804395 face-crop-plus-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22692 2023-04-26 19:24:24.000000 face-crop-plus-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 19:24:41.804395 face-crop-plus-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-26 19:24:24.000000 face-crop-plus-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:24:41.804395 face-crop-plus-1.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:24:41.804395 face-crop-plus-1.0.3/src/face_crop_plus/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-26 19:24:24.000000 face-crop-plus-1.0.3/src/face_crop_plus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10366 2023-04-26 19:24:24.000000 face-crop-plus-1.0.3/src/face_crop_plus/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42437 2023-04-26 19:24:24.000000 face-crop-plus-1.0.3/src/face_crop_plus/cropper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:24:41.804395 face-crop-plus-1.0.3/src/face_crop_plus/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-26 19:24:24.000000 face-crop-plus-1.0.3/src/face_crop_plus/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13019 2023-04-26 19:24:24.000000 face-crop-plus-1.0.3/src/face_crop_plus/models/_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19842 2023-04-26 19:24:24.000000 face-crop-plus-1.0.3/src/face_crop_plus/models/bise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21126 2023-04-26 19:24:24.000000 face-crop-plus-1.0.3/src/face_crop_plus/models/retinaface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6289 2023-04-26 19:24:24.000000 face-crop-plus-1.0.3/src/face_crop_plus/models/rrdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12918 2023-04-26 19:24:24.000000 face-crop-plus-1.0.3/src/face_crop_plus/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:24:41.804395 face-crop-plus-1.0.3/src/face_crop_plus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23699 2023-04-26 19:24:41.000000 face-crop-plus-1.0.3/src/face_crop_plus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-26 19:24:41.000000 face-crop-plus-1.0.3/src/face_crop_plus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 19:24:41.000000 face-crop-plus-1.0.3/src/face_crop_plus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-26 19:24:41.000000 face-crop-plus-1.0.3/src/face_crop_plus.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-26 19:24:41.000000 face-crop-plus-1.0.3/src/face_crop_plus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-26 19:24:41.000000 face-crop-plus-1.0.3/src/face_crop_plus.egg-info/top_level.txt
```

### Comparing `face-crop-plus-1.0.2/LICENCE` & `face-crop-plus-1.0.3/LICENCE`

 * *Files identical despite different names*

### Comparing `face-crop-plus-1.0.2/PKG-INFO` & `face-crop-plus-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: face-crop-plus
-Version: 1.0.2
+Version: 1.0.3
 Summary: Automatic face aligner and cropper with quality enhancement and attribute parsing.
 Home-page: https://github.com/mantasu/face-crop-plus
 Author: Mantas Birškus
 Author-email: mantix7@gmail.com
 License: MIT
 Project-URL: Documentation, https://mantasu.github.io/face-crop-plus
 Project-URL: Bug Tracker, https://github.com/mantasu/face-crop-plus/issues
@@ -34,15 +34,15 @@
 
 </p>
 
 ## About
 
 Image preprocessing package for automatic face alignment and cropping with additional features. It provides the following functionality:
 1. **Face cropping** - face alignment and center-cropping using facial landmarks. Landmarks can be automatically predicted or, if they are already know, can be supplied through a separate file. It is possible to specify face factor, i.e., face area relative to the cropped image, and face extraction strategy, e.g., all faces or largest face per image.
-2. **Face enhancement** - face image quality enhancement. If images are blurry or contain many small faces, quality enhancement model can be used to make the images clearer. Small faces in the image are automatically checked and and enhanced if desired.
+2. **Face enhancement** - face image quality enhancement. If images are blurry or contain many small faces, quality enhancement model can be used to make the images clearer. Small faces in the image are automatically checked and enhanced if desired.
 3. **Face parsing** - face attribute parsing and cropped image grouping to sub-directories. Face images can be grouped according to some facial attributes or some combination, such as _glasses_, _earrings and neckless_, _hats_. It is also possible to generate masks for facial attributes or some combination of them, for instance, _glasses_, _nose_, _nose and eyes_.
 
 Please see _References_ section for more details about which models are used for each feature.
 
 > **Note**: each feature can be used separately, e.g., if you just need to enhance the quality of blurry photos, or if you just need to generate attribute masks (like hats, glasses, face parts).
 
 ## Installation
@@ -279,21 +279,21 @@
     ```
     rm -r data/img_celeba.7z data/img_celeba
     rm data/annotations.zip data/*.txt
     ```
 
 ## Tips
 
-1. When using `num_processes`, only set it to a larger value if you have enough GPU memory, or reduce `batch_size`. Unless you only perform face cropping with already known landmarks and don;t perform quality enhancement nor face parsing, in which case set it to the number of CPU cores you have.
+1. When using `num_processes`, only set it to a larger value if you have enough GPU memory, or reduce `batch_size`. Unless you only perform face cropping with already known landmarks and don't perform quality enhancement nor face parsing, in which case set it to the number of CPU cores you have.
 2. If you experience any of the following:
     * RuntimeError: CUDA error: an illegal memory access was encountered.
     * torch.cuda.OutOfMemoryError: CUDA out of memory.
     * cuDNN error: CUDNN_STATUS_MAPPING_ERROR.
 
-   This is likely because you are processing images on too many processes or have a large batch size. It you run all 3 models on GPU, it may be helpful to just run on a single process with a larger batch size.
+   This is likely because you are processing images on too many processes or have a large batch size. If you run all 3 models on GPU, it may be helpful to just run on a single process with a larger batch size.
 
 ## References
 
 This package uses the code and the pre-trained models from the following repositories:
 * [PyTorch RetinaFace](https://github.com/biubug6/Pytorch_Retinaface) - 5-point landmark prediction
 * [BSRGAN](https://github.com/cszn/BSRGAN) - super resolution and quality enhancement
 * [Face Parsing PyTorch](https://github.com/zllrunning/face-parsing.PyTorch) - grouping by face attributes and segmentation
@@ -305,10 +305,10 @@
 @misc{face-crop-plus,
   author = {Mantas Birškus},
   title = {Face Crop Plus},
   year = {2023},
   publisher = {GitHub},
   journal = {GitHub repository},
   howpublished = {\url{https://github.com/mantasu/face-crop-plus}},
-  doi = {10.5281/zenodo.7856908}
+  doi = {10.5281/zenodo.7856749}
 }
 ```
```

### Comparing `face-crop-plus-1.0.2/README.md` & `face-crop-plus-1.0.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 </p>
 
 ## About
 
 Image preprocessing package for automatic face alignment and cropping with additional features. It provides the following functionality:
 1. **Face cropping** - face alignment and center-cropping using facial landmarks. Landmarks can be automatically predicted or, if they are already know, can be supplied through a separate file. It is possible to specify face factor, i.e., face area relative to the cropped image, and face extraction strategy, e.g., all faces or largest face per image.
-2. **Face enhancement** - face image quality enhancement. If images are blurry or contain many small faces, quality enhancement model can be used to make the images clearer. Small faces in the image are automatically checked and and enhanced if desired.
+2. **Face enhancement** - face image quality enhancement. If images are blurry or contain many small faces, quality enhancement model can be used to make the images clearer. Small faces in the image are automatically checked and enhanced if desired.
 3. **Face parsing** - face attribute parsing and cropped image grouping to sub-directories. Face images can be grouped according to some facial attributes or some combination, such as _glasses_, _earrings and neckless_, _hats_. It is also possible to generate masks for facial attributes or some combination of them, for instance, _glasses_, _nose_, _nose and eyes_.
 
 Please see _References_ section for more details about which models are used for each feature.
 
 > **Note**: each feature can be used separately, e.g., if you just need to enhance the quality of blurry photos, or if you just need to generate attribute masks (like hats, glasses, face parts).
 
 ## Installation
@@ -257,21 +257,21 @@
     ```
     rm -r data/img_celeba.7z data/img_celeba
     rm data/annotations.zip data/*.txt
     ```
 
 ## Tips
 
-1. When using `num_processes`, only set it to a larger value if you have enough GPU memory, or reduce `batch_size`. Unless you only perform face cropping with already known landmarks and don;t perform quality enhancement nor face parsing, in which case set it to the number of CPU cores you have.
+1. When using `num_processes`, only set it to a larger value if you have enough GPU memory, or reduce `batch_size`. Unless you only perform face cropping with already known landmarks and don't perform quality enhancement nor face parsing, in which case set it to the number of CPU cores you have.
 2. If you experience any of the following:
     * RuntimeError: CUDA error: an illegal memory access was encountered.
     * torch.cuda.OutOfMemoryError: CUDA out of memory.
     * cuDNN error: CUDNN_STATUS_MAPPING_ERROR.
 
-   This is likely because you are processing images on too many processes or have a large batch size. It you run all 3 models on GPU, it may be helpful to just run on a single process with a larger batch size.
+   This is likely because you are processing images on too many processes or have a large batch size. If you run all 3 models on GPU, it may be helpful to just run on a single process with a larger batch size.
 
 ## References
 
 This package uses the code and the pre-trained models from the following repositories:
 * [PyTorch RetinaFace](https://github.com/biubug6/Pytorch_Retinaface) - 5-point landmark prediction
 * [BSRGAN](https://github.com/cszn/BSRGAN) - super resolution and quality enhancement
 * [Face Parsing PyTorch](https://github.com/zllrunning/face-parsing.PyTorch) - grouping by face attributes and segmentation
@@ -283,10 +283,10 @@
 @misc{face-crop-plus,
   author = {Mantas Birškus},
   title = {Face Crop Plus},
   year = {2023},
   publisher = {GitHub},
   journal = {GitHub repository},
   howpublished = {\url{https://github.com/mantasu/face-crop-plus}},
-  doi = {10.5281/zenodo.7856908}
+  doi = {10.5281/zenodo.7856749}
 }
 ```
```

### Comparing `face-crop-plus-1.0.2/setup.py` & `face-crop-plus-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name = "face-crop-plus",
-    version = "1.0.2",
+    version = "1.0.3",
     author = "Mantas Birškus",
     author_email = "mantix7@gmail.com",
     license = "MIT",
     description = f"Automatic face aligner and cropper with quality "
                   f"enhancement and attribute parsing.",
     long_description = long_description,
     long_description_content_type = "text/markdown",
```

### Comparing `face-crop-plus-1.0.2/src/face_crop_plus/__main__.py` & `face-crop-plus-1.0.3/src/face_crop_plus/__main__.py`

 * *Files identical despite different names*

### Comparing `face-crop-plus-1.0.2/src/face_crop_plus/cropper.py` & `face-crop-plus-1.0.3/src/face_crop_plus/cropper.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,18 @@
 from .models import RRDBNet
 from .models import RetinaFace
 
 from .utils import (
     STANDARD_LANDMARKS_5, 
     parse_landmarks_file, 
     get_ldm_slices, 
-    create_batch_from_files, 
     as_numpy, 
     as_tensor,
+    read_images,
+    as_batch,
 )
 
 
 class Cropper():
     """Face cropper class with bonus features.
 
     This class is capable of automatically aligning and center-cropping 
@@ -736,15 +737,15 @@
                 self.save_group(face_group, file_name_group, group_dir)
 
                 if masks is not None:
                     # Save to masks dir
                     group_dir += "_mask"
                     masks = masks[[mask_indices.index(i) for i in group_idx]]
                     self.save_group(masks, file_name_group, group_dir)
-
+    
     def process_batch(self, file_names: list[str], input_dir: str, output_dir: str):
         """Extracts faces from a batch of images and saves them.
 
         Takes file names, input directory, reads images and extracts 
         faces and saves them to the output directory. This method works 
         as follows:
 
@@ -779,48 +780,39 @@
         Args:
             file_names: The list of image file names (not full paths). 
                 All the images should be in the same directory.
             input_dir: Path to input directory with image files.
             output_dir: Path to output directory to save the extracted 
                 face images.
         """
-        if self.landmarks is None and self.det_model is None:
-            # Initialize empty lists, landmarks and paddings as None
-            images, indices, landmarks, paddings = [], [], None, None
+        # Read images and filter valid corresponding file names
+        images, file_names = read_images(file_names, input_dir)
 
-            for i, file_name in enumerate(file_names):
-                # Make path, load image, convert to RGB
-                path = os.path.join(input_dir, file_name)
-                image = cv2.cvtColor(cv2.imread(path), cv2.COLOR_BGR2RGB)
-
-                # Update the lists
-                indices.append(i)
-                images.append(image)
+        if self.landmarks is None and self.det_model is None:
+            # One-to-one image to index mapping and no landmarks
+            indices, landmarks = list(range(len(file_names))), None
         elif self.landmarks is not None:
-            # Initialize empty image and index lists, set padding None
-            images, img_indices, ldm_indices, paddings = [], [], [], None
+            # Initialize empty idx lists
+            indices, indices_ldm = [], []
 
             for i, file_name in enumerate(file_names):
-                # Make path, load image, check indices
-                path = os.path.join(input_dir, file_name)
-                image = cv2.cvtColor(cv2.imread(path), cv2.COLOR_BGR2RGB)
+                # Check the indices of landmark sets in landmarks file
                 indices_i = np.where(file_name == self.landmarks[1])[0]
 
-                # Update the lists
-                images.append(image)
-                img_indices.extend([i] * len(indices_i))
-                ldm_indices.extend(indices_i.tolist())
+                # Update img & ldm file name indices
+                indices.extend([i] * len(indices_i))
+                indices_ldm.extend(indices_i.tolist())
+            
+            # Set landmarks according to the indices
+            landmarks = self.landmarks[0][indices_ldm]
             
-            # Update indices and select landmarks
-            indices = img_indices
-            landmarks = self.landmarks[0][ldm_indices]
         elif self.det_model is not None:
-            # Create a batch of images (with faces) and their paddings
-            b = create_batch_from_files(file_names, input_dir, self.resize_size)
-            images, paddings = as_tensor(b[0], self.device), b[2]
+             # Create a batch of images (with faces) and their paddings
+            images, _, paddings = as_batch(images, self.resize_size)
+            images, paddings = as_tensor(images, self.device), paddings
 
             # If landmarks were not given, predict, undo padding
             landmarks, indices = self.det_model.predict(images)
             landmarks -= paddings[indices][:, None, [2, 0]]
 
         if landmarks is not None and len(landmarks) == 0:
             # Nothing to save
@@ -843,17 +835,16 @@
             # Generate source, target landmarks, estimate & apply transform
             images = self.crop_align(images, paddings, indices, landmarks)
 
         if self.par_model is not None:
             # Predict attribute and mask groups if face parsing desired
             groups = self.par_model.predict(as_tensor(images, self.device))
 
-        # Pick file names for each face, save faces
-        file_names = np.array(file_names)[indices]
-        self.save_groups(images, file_names, output_dir, *groups)
+        # Pick file names for each face, save faces (by groups if exist)
+        self.save_groups(images, file_names[indices], output_dir, *groups)
     
     def process_dir(self, input_dir: str, output_dir: str | None = None):
         """Processes images in the specified input directory.
 
         Splits all the file names in the input directory to batches 
         and processes batches on multiple cores. For every file name 
         batch, images are loaded, some are optionally enhanced,
```

### Comparing `face-crop-plus-1.0.2/src/face_crop_plus/models/_layers.py` & `face-crop-plus-1.0.3/src/face_crop_plus/models/_layers.py`

 * *Files identical despite different names*

### Comparing `face-crop-plus-1.0.2/src/face_crop_plus/models/bise.py` & `face-crop-plus-1.0.3/src/face_crop_plus/models/bise.py`

 * *Files identical despite different names*

### Comparing `face-crop-plus-1.0.2/src/face_crop_plus/models/retinaface.py` & `face-crop-plus-1.0.3/src/face_crop_plus/models/retinaface.py`

 * *Files identical despite different names*

### Comparing `face-crop-plus-1.0.2/src/face_crop_plus/models/rrdb.py` & `face-crop-plus-1.0.3/src/face_crop_plus/models/rrdb.py`

 * *Files identical despite different names*

### Comparing `face-crop-plus-1.0.2/src/face_crop_plus/utils.py` & `face-crop-plus-1.0.3/src/face_crop_plus/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import cv2
 import json
 import torch
+import warnings
 import numpy as np
 
 
 STANDARD_LANDMARKS_5 = np.float32([
     [0.31556875000000000, 0.4615741071428571],
     [0.68262291666666670, 0.4615741071428571],
     [0.50026249999999990, 0.6405053571428571],
@@ -216,38 +217,81 @@
     elif isinstance(img, list):
         img = [torch.from_numpy(x).permute(2, 0, 1).float().to(device) for x in img]
     else:
         img = torch.from_numpy(img).permute(0, 3, 1, 2).float().to(device)
     
     return img
 
-def create_batch_from_files(
+def read_images(
     file_names: list[str],
     input_dir: str,
+) -> tuple[list[np.ndarray], np.ndarray]:
+    """Reads images from the specified paths.
+
+    Takes a list of file names and an input directory and loads the 
+    specified images from it. If an image could not be loaded, a warning 
+    is raised.
+
+    Args:
+        file_names: The list of image file names.
+        input_dir (str): The input directory with the images.
+
+    Returns:
+        A tuple where the first element is a list of length N (number of 
+        loaded images) where each element is an RGB image represented as 
+        a numpy array of type :attr:`numpy.uint8` of shape (H, W, 3) 
+        (note that H and W for each image can be different) and the 
+        second element is a numpy array of type :class:`numpy.str_` of 
+        shape (N,) representing the list of file names that correspond 
+        to each image. The second element is just a numpy form of 
+        ``file_names`` but it can have a lower length, in case some 
+        images were not read successfully.
+    """
+    # Init index and img list
+    indices, images = [], []
+
+    for i, file_name in enumerate(file_names):
+        # Generate full path to the input image
+        path = os.path.join(input_dir, file_name)
+
+        try:
+            # Read the image from the given path, convert to RGB form
+            image = cv2.cvtColor(cv2.imread(path), cv2.COLOR_BGR2RGB)
+        except cv2.error as e:
+            warnings.warn(f"Could not read the image {path}")
+            continue
+        
+        # Add image and index
+        images.append(image)
+        indices.append(i)
+    
+    return images, np.array(file_names)[indices]
+
+def as_batch(
+    images: list[np.ndarray],
     size: int | tuple[int, int] = 512,
     padding_mode: str = "constant",
 ) -> tuple[np.ndarray, np.ndarray, np.ndarray]:
     """Creates image batch from a list of image paths.
 
-    For every image path in the given list, the image is read, resized
-    to not exceed either of the dimensions specified in ``size`` while
-    keeping the same aspect ratio and the shorter dimension is padded to
-    fully match the specified size. All the images are stacked and
-    returned as a batch. Variables required to transform the images back
-    to the original ones (padding and scale) are also returned as a
-    batch.
+    For every image in the given list, the image is resized to not 
+    exceed either of the dimensions specified in ``size`` while keeping 
+    the same aspect ratio and the shorter dimension is padded to fully 
+    match the specified size. All the images are stacked and returned as 
+    a batch. Variables required to transform the images back to the 
+    original ones (padding and scale) are also returned as a batch.
 
     Example:
         If some loaded image dimension is (1280×720) and the desired
         output ``size`` is specified as *(512, 256)*, then the image is
         first be resized to *(455, 256)* and then the width is padded 
         from both sides. The final image size is *(512, 256)*.
 
     Args:
-        file_names: The list of paths to images.
+        images: The list of paths to images.
         padding_mode: The type of padding to apply to pad the shorter
             dimension. For the available options, see
             `OpenCV BorderTypes <https://docs.opencv.org/3.4/d2/de8/group__core__array.html#ga209f2f4869e304c82d07739337eae7c5>`_.
             It can be all lowercase. Defaults to "constant".
         size: The width and the height each image should be resized +
             padded to. I.e., the spacial dimensions of the batch. If
             a single number is specified then it is the same for width
@@ -258,23 +302,19 @@
         + padded images of shape (N, H, W, 3) of type 
         :attr:`numpy.uint8` with values from 0 to 255, un-scale factors 
         of shape (N,) of type :attr:`numpy.float32`, and applied 
         paddings of shape (N, 4) of type :attr:`numpy.int64` with 
         values >= 0.
     """
     # Init lists, resize dims, border type
-    images, unscales, paddings = [], [], []
+    img_batch, unscales, paddings = [], [], []
     size = (size, size) if isinstance(size, int) else size
     border_type = getattr(cv2, f"BORDER_{padding_mode.upper()}")
-    file_paths = [os.path.join(input_dir, file) for file in file_names]
 
-    for path in file_paths:
-        # Read the image from the given path, convert to RGB form
-        image = cv2.cvtColor(cv2.imread(path), cv2.COLOR_BGR2RGB)
-    
+    for image in images:    
         # Get width, height, padding & check interpolation
         (h, w), m = image.shape[:2], max(*image.shape[:2])
         interpolation = cv2.INTER_AREA if m > max(size) else cv2.INTER_CUBIC
 
         if (ratio_w := size[0] / w) < (ratio_h := size[1] / h):
             # Based on width 
             unscale = ratio_w
@@ -287,12 +327,12 @@
             padding = [0, 0, (size[0] - ww) // 2, (size[0] - ww + 1) // 2]
     
         # Pad the lower dimension with specific border type, then resize
         image = cv2.resize(image, (ww, hh), interpolation=interpolation)
         image = cv2.copyMakeBorder(image, *padding, borderType=border_type)
 
         # Append to lists
-        images.append(image)
+        img_batch.append(image)
         unscales.append(np.array(unscale))
         paddings.append(np.array(padding))
 
-    return np.stack(images), np.stack(unscales), np.stack(paddings)
+    return np.stack(img_batch), np.stack(unscales), np.stack(paddings)
```

### Comparing `face-crop-plus-1.0.2/src/face_crop_plus.egg-info/PKG-INFO` & `face-crop-plus-1.0.3/src/face_crop_plus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: face-crop-plus
-Version: 1.0.2
+Version: 1.0.3
 Summary: Automatic face aligner and cropper with quality enhancement and attribute parsing.
 Home-page: https://github.com/mantasu/face-crop-plus
 Author: Mantas Birškus
 Author-email: mantix7@gmail.com
 License: MIT
 Project-URL: Documentation, https://mantasu.github.io/face-crop-plus
 Project-URL: Bug Tracker, https://github.com/mantasu/face-crop-plus/issues
@@ -34,15 +34,15 @@
 
 </p>
 
 ## About
 
 Image preprocessing package for automatic face alignment and cropping with additional features. It provides the following functionality:
 1. **Face cropping** - face alignment and center-cropping using facial landmarks. Landmarks can be automatically predicted or, if they are already know, can be supplied through a separate file. It is possible to specify face factor, i.e., face area relative to the cropped image, and face extraction strategy, e.g., all faces or largest face per image.
-2. **Face enhancement** - face image quality enhancement. If images are blurry or contain many small faces, quality enhancement model can be used to make the images clearer. Small faces in the image are automatically checked and and enhanced if desired.
+2. **Face enhancement** - face image quality enhancement. If images are blurry or contain many small faces, quality enhancement model can be used to make the images clearer. Small faces in the image are automatically checked and enhanced if desired.
 3. **Face parsing** - face attribute parsing and cropped image grouping to sub-directories. Face images can be grouped according to some facial attributes or some combination, such as _glasses_, _earrings and neckless_, _hats_. It is also possible to generate masks for facial attributes or some combination of them, for instance, _glasses_, _nose_, _nose and eyes_.
 
 Please see _References_ section for more details about which models are used for each feature.
 
 > **Note**: each feature can be used separately, e.g., if you just need to enhance the quality of blurry photos, or if you just need to generate attribute masks (like hats, glasses, face parts).
 
 ## Installation
@@ -279,21 +279,21 @@
     ```
     rm -r data/img_celeba.7z data/img_celeba
     rm data/annotations.zip data/*.txt
     ```
 
 ## Tips
 
-1. When using `num_processes`, only set it to a larger value if you have enough GPU memory, or reduce `batch_size`. Unless you only perform face cropping with already known landmarks and don;t perform quality enhancement nor face parsing, in which case set it to the number of CPU cores you have.
+1. When using `num_processes`, only set it to a larger value if you have enough GPU memory, or reduce `batch_size`. Unless you only perform face cropping with already known landmarks and don't perform quality enhancement nor face parsing, in which case set it to the number of CPU cores you have.
 2. If you experience any of the following:
     * RuntimeError: CUDA error: an illegal memory access was encountered.
     * torch.cuda.OutOfMemoryError: CUDA out of memory.
     * cuDNN error: CUDNN_STATUS_MAPPING_ERROR.
 
-   This is likely because you are processing images on too many processes or have a large batch size. It you run all 3 models on GPU, it may be helpful to just run on a single process with a larger batch size.
+   This is likely because you are processing images on too many processes or have a large batch size. If you run all 3 models on GPU, it may be helpful to just run on a single process with a larger batch size.
 
 ## References
 
 This package uses the code and the pre-trained models from the following repositories:
 * [PyTorch RetinaFace](https://github.com/biubug6/Pytorch_Retinaface) - 5-point landmark prediction
 * [BSRGAN](https://github.com/cszn/BSRGAN) - super resolution and quality enhancement
 * [Face Parsing PyTorch](https://github.com/zllrunning/face-parsing.PyTorch) - grouping by face attributes and segmentation
@@ -305,10 +305,10 @@
 @misc{face-crop-plus,
   author = {Mantas Birškus},
   title = {Face Crop Plus},
   year = {2023},
   publisher = {GitHub},
   journal = {GitHub repository},
   howpublished = {\url{https://github.com/mantasu/face-crop-plus}},
-  doi = {10.5281/zenodo.7856908}
+  doi = {10.5281/zenodo.7856749}
 }
 ```
```

### Comparing `face-crop-plus-1.0.2/src/face_crop_plus.egg-info/SOURCES.txt` & `face-crop-plus-1.0.3/src/face_crop_plus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

