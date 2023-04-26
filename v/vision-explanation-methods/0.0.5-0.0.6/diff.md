# Comparing `tmp/vision_explanation_methods-0.0.5.tar.gz` & `tmp/vision_explanation_methods-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vision_explanation_methods-0.0.5.tar", last modified: Fri Apr 14 18:36:27 2023, max compression
+gzip compressed data, was "vision_explanation_methods-0.0.6.tar", last modified: Tue Apr 25 17:33:55 2023, max compression
```

## Comparing `vision_explanation_methods-0.0.5.tar` & `vision_explanation_methods-0.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:36:27.621512 vision_explanation_methods-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-14 18:36:27.000000 vision_explanation_methods-0.0.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-04-14 18:36:27.617512 vision_explanation_methods-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-04-14 18:21:04.000000 vision_explanation_methods-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 18:36:27.621512 vision_explanation_methods-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-04-14 18:21:04.000000 vision_explanation_methods-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:36:27.617512 vision_explanation_methods-0.0.5/vision_explanation_methods/
--rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-04-14 18:21:04.000000 vision_explanation_methods-0.0.5/vision_explanation_methods/DRISE_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-14 18:21:04.000000 vision_explanation_methods-0.0.5/vision_explanation_methods/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:36:27.617512 vision_explanation_methods-0.0.5/vision_explanation_methods/explanations/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-14 18:21:04.000000 vision_explanation_methods-0.0.5/vision_explanation_methods/explanations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9445 2023-04-14 18:21:04.000000 vision_explanation_methods-0.0.5/vision_explanation_methods/explanations/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     8977 2023-04-14 18:21:04.000000 vision_explanation_methods-0.0.5/vision_explanation_methods/explanations/drise.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-14 18:21:04.000000 vision_explanation_methods-0.0.5/vision_explanation_methods/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:36:27.617512 vision_explanation_methods-0.0.5/vision_explanation_methods.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-04-14 18:36:27.000000 vision_explanation_methods-0.0.5/vision_explanation_methods.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-14 18:36:27.000000 vision_explanation_methods-0.0.5/vision_explanation_methods.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 18:36:27.000000 vision_explanation_methods-0.0.5/vision_explanation_methods.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 18:36:27.000000 vision_explanation_methods-0.0.5/vision_explanation_methods.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-14 18:36:27.000000 vision_explanation_methods-0.0.5/vision_explanation_methods.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-14 18:36:27.000000 vision_explanation_methods-0.0.5/vision_explanation_methods.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:33:55.266099 vision_explanation_methods-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-25 17:33:55.000000 vision_explanation_methods-0.0.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-04-25 17:33:55.266099 vision_explanation_methods-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-04-25 17:13:07.000000 vision_explanation_methods-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 17:33:55.266099 vision_explanation_methods-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-04-25 17:13:07.000000 vision_explanation_methods-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:33:55.266099 vision_explanation_methods-0.0.6/vision_explanation_methods/
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-04-25 17:13:07.000000 vision_explanation_methods-0.0.6/vision_explanation_methods/DRISE_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-25 17:13:07.000000 vision_explanation_methods-0.0.6/vision_explanation_methods/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:33:55.266099 vision_explanation_methods-0.0.6/vision_explanation_methods/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-25 17:13:07.000000 vision_explanation_methods-0.0.6/vision_explanation_methods/explanations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9450 2023-04-25 17:13:07.000000 vision_explanation_methods-0.0.6/vision_explanation_methods/explanations/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12738 2023-04-25 17:13:07.000000 vision_explanation_methods-0.0.6/vision_explanation_methods/explanations/drise.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-25 17:13:07.000000 vision_explanation_methods-0.0.6/vision_explanation_methods/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:33:55.266099 vision_explanation_methods-0.0.6/vision_explanation_methods.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-04-25 17:33:55.000000 vision_explanation_methods-0.0.6/vision_explanation_methods.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-25 17:33:55.000000 vision_explanation_methods-0.0.6/vision_explanation_methods.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 17:33:55.000000 vision_explanation_methods-0.0.6/vision_explanation_methods.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 17:33:55.000000 vision_explanation_methods-0.0.6/vision_explanation_methods.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-25 17:33:55.000000 vision_explanation_methods-0.0.6/vision_explanation_methods.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-25 17:33:55.000000 vision_explanation_methods-0.0.6/vision_explanation_methods.egg-info/top_level.txt
```

### Comparing `vision_explanation_methods-0.0.5/LICENSE.txt` & `vision_explanation_methods-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vision_explanation_methods-0.0.5/PKG-INFO` & `vision_explanation_methods-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision_explanation_methods
-Version: 0.0.5
+Version: 0.0.6
 Summary: Microsoft Vision Explanation Methods SDK for Python
 Home-page: https://github.com/microsoft/vision-explanation-methods
 Author: Microsoft Corp
 Author-email: jamhall@microsoft.com
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `vision_explanation_methods-0.0.5/README.md` & `vision_explanation_methods-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `vision_explanation_methods-0.0.5/setup.py` & `vision_explanation_methods-0.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `vision_explanation_methods-0.0.5/vision_explanation_methods/DRISE_runner.py` & `vision_explanation_methods-0.0.6/vision_explanation_methods/DRISE_runner.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 """Method for generating saliency maps for object detection models."""
 
+import base64
 from io import BytesIO
 from typing import Optional, Tuple
 
 import matplotlib
 import matplotlib.pyplot as plt
 import numpy
+import pandas as pd
 import requests
 import torch
 import torchvision
 from captum.attr import visualization as viz
-from ml_wrappers.model.image_model_wrapper import PytorchDRiseWrapper
+from ml_wrappers.model.image_model_wrapper import (MLflowDRiseWrapper,
+                                                   PytorchDRiseWrapper)
 from PIL import Image
 from torchvision import transforms as T
 from torchvision.models import detection
 from torchvision.models.detection.faster_rcnn import FastRCNNPredictor
 
 from .explanations import drise
 
@@ -126,44 +129,72 @@
     if (imagelocation.startswith("http://")
        or imagelocation.startswith("https://")):
         response = requests.get(imagelocation)
         image_open_pointer = BytesIO(response.content)
 
     test_image = Image.open(image_open_pointer).convert('RGB')
 
-    detections = model.predict(
-        T.ToTensor()(test_image).unsqueeze(0).to(device))
+    if isinstance(model, MLflowDRiseWrapper):
+        x, y = test_image.size
+        imgio = BytesIO()
+        test_image.save(imgio, format='PNG')
+        img_str = base64.b64encode(imgio.getvalue()).decode('utf8')
+        img_input = pd.DataFrame(
+            data=[[img_str, (y, x)]],
+            columns=['image', 'image_size'],
+        )
+
+        detections = model.predict(img_input)
+        saliency_scores = drise.DRISE_saliency_for_mlflow(
+            model=model,
+            # Repeated the tensor to test batching
+            image_tensor=img_input,
+            target_detections=detections,
+            # This is how many masks to run -
+            # more is slower but gives higher quality mask.
+            number_of_masks=nummasks,
+            mask_padding=maskpadding,
+            device=device,
+            # This is the resolution of the random masks.
+            # High resolutions will give finer masks, but more need to be run.
+            mask_res=maskres,
+            verbose=True  # Turns progress bar on/off.
+        )
+    else:
+        img_input = T.ToTensor()(test_image).unsqueeze(0).to(device)
 
-    saliency_scores = drise.DRISE_saliency(
-        model=model,
-        # Repeated the tensor to test batching
-        image_tensor=T.ToTensor()(test_image).unsqueeze(0).to(device),
-        target_detections=detections,
-        # This is how many masks to run -
-        # more is slower but gives higher quality mask.
-        number_of_masks=nummasks,
-        mask_padding=maskpadding,
-        device=device,
-        # This is the resolution of the random masks.
-        # High resolutions will give finer masks, but more need to be run.
-        mask_res=maskres,
-        verbose=True  # Turns progress bar on/off.
-    )
+        detections = model.predict(img_input)
+
+        saliency_scores = drise.DRISE_saliency(
+            model=model,
+            # Repeated the tensor to test batching
+            image_tensor=img_input,
+            target_detections=detections,
+            # This is how many masks to run -
+            # more is slower but gives higher quality mask.
+            number_of_masks=nummasks,
+            mask_padding=maskpadding,
+            device=device,
+            # This is the resolution of the random masks.
+            # High resolutions will give finer masks, but more need to be run.
+            mask_res=maskres,
+            verbose=True  # Turns progress bar on/off.
+        )
 
     img_index = 0
 
     # Filter out saliency scores containing nan values
     saliency_scores = [saliency_scores[img_index][i]
                        for i in range(len(saliency_scores[img_index]))
                        if not torch.isnan(
                        saliency_scores[img_index][i]['detection']).any()]
 
     num_detections = len(saliency_scores)
-
-    if num_detections == 0:  # If no objects have been detected...
+    if num_detections == 0:
+        print("No detections found. Saving empty figure.")
         fail = Image.new('RGB', (100, 100))
         fail = fail.save(savename)
         return None, None, None
 
     label_list = []
     fig_list = []
     for i in range((max_figures if num_detections > max_figures
@@ -183,9 +214,10 @@
             cmap=plt.cm.gist_rainbow,
             title="Detection " + str(i),
             plt_fig_axis=(fig, ax),
             use_pyplot=False
         )
 
         fig.savefig(savename+str(i)+IMAGE_TYPE)
+        fig.clear()
         fig_list.append(fig)
     return fig_list, savename, label_list
```

### Comparing `vision_explanation_methods-0.0.5/vision_explanation_methods/explanations/common.py` & `vision_explanation_methods-0.0.6/vision_explanation_methods/explanations/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -249,10 +249,10 @@
 
     expanded_scores = torch.ones(number_of_detections, number_of_classes + 1)
 
     for i, (score, label) in enumerate(zip(scores, labels)):
 
         residual = (1. - score.item()) / (number_of_classes)
         expanded_scores[i, :] *= residual
-        expanded_scores[i, label.item()] = score
+        expanded_scores[i, int(label.item())] = score
 
     return expanded_scores
```

### Comparing `vision_explanation_methods-0.0.5/vision_explanation_methods/explanations/drise.py` & `vision_explanation_methods-0.0.6/vision_explanation_methods/explanations/drise.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,23 +3,27 @@
 # ---------------------------------------------------------
 
 """Implementation of DRISE.
 
 A black box explainability method for object detection.
 """
 
-
+import base64
 import copy
+import io
 from dataclasses import dataclass
+from io import BytesIO
 from typing import List, Optional, Tuple
 
+import pandas as pd
 import PIL.Image as Image
 import torch
 import torchvision.transforms as T
 import tqdm
+from torch import Tensor
 
 from .common import (DetectionRecord, GeneralObjectDetectionModelWrapper,
                      compute_affinity_matrix)
 
 
 @dataclass
 class MaskAffinityRecord:
@@ -123,15 +127,14 @@
     :type base_detections: Detection Record
     :param masked_detections: Set of detections to score against
     :type masked_detections: Detection Record
     :return: Set of affinity scores associated with each detections
     :rtype: Tensor of shape D, where D is number of base detections
     """
     score_matrix = compute_affinity_matrix(base_detections, masked_detections)
-
     return torch.max(score_matrix, dim=1)[0]
 
 
 def saliency_fusion(
         affinity_records: List[MaskAffinityRecord],
         normalize: Optional[bool] = True,
         verbose: bool = False
@@ -164,28 +167,28 @@
             weighted_masks = affinity_record.get_weighted_masks()
 
             for weighted_mask_accum, weighted_mask in zip(weighted_masks_accum,
                                                           weighted_masks):
                 weighted_mask_accum += weighted_mask
 
             for average_score_accum, affinity_score in zip(
-                                                        average_scores_accum,
-                                                        affinity_scores):
+                    average_scores_accum,
+                    affinity_scores):
                 average_score_accum += affinity_score
         except RuntimeError:
             continue
 
     for scores in average_scores_accum:
         scores /= len(affinity_records)
 
     if normalize:
         for average_score, weighted_mask in zip(average_scores_accum,
                                                 weighted_masks_accum):
             weighted_mask -= average_score.unsqueeze(1).unsqueeze(1). \
-                            unsqueeze(1) * unweighted_mask_accum
+                unsqueeze(1) * unweighted_mask_accum
 
     normalized_masks = []
 
     for imgs in weighted_masks_accum:
         normed_masks = []
         for mask in imgs:
             mask = mask - torch.min(mask)
@@ -194,15 +197,15 @@
         normalized_masks.append(normed_masks)
 
     return normalized_masks
 
 
 def DRISE_saliency(
         model: GeneralObjectDetectionModelWrapper,
-        image_tensor: torch.Tensor,
+        image_tensor: Tensor,
         target_detections: List[DetectionRecord],
         number_of_masks: int,
         mask_res: Tuple[int, int] = (16, 16),
         mask_padding: Optional[int] = None,
         device: str = "cpu",
         verbose: bool = False,
 ) -> List[torch.Tensor]:
@@ -253,7 +256,119 @@
 
         mask_records.append(MaskAffinityRecord(
             mask=mask.to("cpu"),
             affinity_scores=[s.detach().to("cpu") for s in affinity_scores])
         )
 
     return saliency_fusion(mask_records, verbose=verbose)
+
+
+def convert_base64_to_tensor(b64_img: str) -> Tensor:
+    """Convert base64 image to tensor.
+
+    :param b64_img: Base64 encoded image
+    :type b64_img: str
+    :return: Image tensor
+    :rtype: Tensor
+    """
+    base64_decoded = base64.b64decode(b64_img)
+    image = Image.open(io.BytesIO(base64_decoded))
+    img_tens = T.ToTensor()(image)
+    return img_tens
+
+
+def convert_tensor_to_base64(img_tens: Tensor) -> Tuple[str, Tuple[int, int]]:
+    """Convert image tensor to base64 string.
+
+    :param img_tens: Image tensor
+    :type img_tens: Tensor
+    :return: Base64 encoded image
+    :rtype: str
+    """
+    img_pil = T.ToPILImage()(img_tens)
+    imgio = BytesIO()
+    img_pil.save(imgio, format='PNG')
+    img_str = base64.b64encode(imgio.getvalue()).decode('utf8')
+    return img_str, img_pil.size
+
+
+def DRISE_saliency_for_mlflow(
+        model,
+        image_tensor: pd.DataFrame,
+        target_detections: List[DetectionRecord],
+        number_of_masks: int,
+        mask_res: Tuple[int, int] = (16, 16),
+        mask_padding: Optional[int] = None,
+        device: str = "cpu",
+        verbose: bool = False,
+) -> List[torch.Tensor]:
+    """Compute DRISE saliency map.
+
+    :param model: Object detection model wrapped for occlusion
+    :type model: OcclusionModelWrapper
+    :param target_detections: Baseline detections to get saliency
+        maps for
+    :type target_detections: List of Detection Records
+    :param number_of_masks: Number of masks to use for saliency
+    :type number_of_masks: int
+    :param mask_res: Resolution of mask before scale up
+    :type maks_res: Tuple of ints
+    :param mask_padding: How much to pad the mask before cropping
+    :type: Optional int
+    :device: Device to use to run the function
+    :type: str
+    :return: A list of tensors, one tensor for each image. Each tensor
+        is of shape [D, 3, W, H], and [i ,3 W, H] is the saliency map
+        associated with detection i.
+    :rtype: List torch.Tensor
+    """
+    if not isinstance(image_tensor, pd.DataFrame):
+        raise ValueError(
+            "TypeError: Image needs to be a torch.Tensor or pd.DataFrame")
+    if not image_tensor.shape[0] == 1:
+        raise ValueError(
+            "Currently only one image supported for AutoML mlflow model")
+
+    img_size = image_tensor.loc[0, 'image_size']
+
+    if mask_padding is None:
+        mask_padding = int(max(
+            img_size[0] / mask_res[0], img_size[1] / mask_res[1]))
+
+    mask_records = []
+
+    mask_iterator = tqdm.tqdm(range(number_of_masks)) if verbose \
+        else range(number_of_masks)
+
+    for _ in mask_iterator:
+        # Converts image base64 to a tensor
+        # Fuses mask tensor with image tensor
+        # Converts fused image tensor to base64
+        mask = generate_mask(mask_res, img_size, mask_padding)
+
+        # Currently only supports single image
+        img_tens = convert_base64_to_tensor(
+            image_tensor.loc[0, 'image'])
+
+        masked_image = fuse_mask(img_tens.to(device), mask.to(device))
+
+        masked_image_str, masked_image_size = convert_tensor_to_base64(
+            masked_image)
+
+        masked_df = pd.DataFrame(
+            data=[[masked_image_str, masked_image_size]],
+            columns=['image', "image_size"],
+        )
+
+        masked_detections = model.predict(masked_df)
+
+        affinity_scores = [
+            compute_affinity_scores(target_detection, masked_detection)
+            for (target_detection, masked_detection)
+            in zip(target_detections, masked_detections)
+        ]
+
+        mask_records.append(MaskAffinityRecord(
+            mask=mask.detach().cpu(),
+            affinity_scores=[s.detach().cpu() for s in affinity_scores])
+        )
+    return saliency_fusion(mask_records, verbose=verbose)
```

### Comparing `vision_explanation_methods-0.0.5/vision_explanation_methods.egg-info/PKG-INFO` & `vision_explanation_methods-0.0.6/vision_explanation_methods.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision-explanation-methods
-Version: 0.0.5
+Version: 0.0.6
 Summary: Microsoft Vision Explanation Methods SDK for Python
 Home-page: https://github.com/microsoft/vision-explanation-methods
 Author: Microsoft Corp
 Author-email: jamhall@microsoft.com
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `vision_explanation_methods-0.0.5/vision_explanation_methods.egg-info/SOURCES.txt` & `vision_explanation_methods-0.0.6/vision_explanation_methods.egg-info/SOURCES.txt`

 * *Files identical despite different names*

