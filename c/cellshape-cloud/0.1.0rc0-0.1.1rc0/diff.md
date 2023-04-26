# Comparing `tmp/cellshape-cloud-0.1.0rc0.tar.gz` & `tmp/cellshape-cloud-0.1.1rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellshape-cloud-0.1.0rc0.tar", last modified: Wed Feb 22 13:32:00 2023, max compression
+gzip compressed data, was "cellshape-cloud-0.1.1rc0.tar", last modified: Wed Apr 26 14:16:51 2023, max compression
```

## Comparing `cellshape-cloud-0.1.0rc0.tar` & `cellshape-cloud-0.1.1rc0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 13:32:00.699040 cellshape-cloud-0.1.0rc0/
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-02-22 13:31:46.000000 cellshape-cloud-0.1.0rc0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-02-22 13:31:46.000000 cellshape-cloud-0.1.0rc0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-02-22 13:32:00.699040 cellshape-cloud-0.1.0rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-02-22 13:31:46.000000 cellshape-cloud-0.1.0rc0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 13:32:00.695040 cellshape-cloud-0.1.0rc0/cellshape_cloud/
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-02-22 13:31:46.000000 cellshape-cloud-0.1.0rc0/cellshape_cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-02-22 13:31:46.000000 cellshape-cloud-0.1.0rc0/cellshape_cloud/cloud_autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-02-22 13:31:46.000000 cellshape-cloud-0.1.0rc0/cellshape_cloud/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-02-22 13:31:46.000000 cellshape-cloud-0.1.0rc0/cellshape_cloud/extract_features.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-02-22 13:31:46.000000 cellshape-cloud-0.1.0rc0/cellshape_cloud/helper_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-02-22 13:31:46.000000 cellshape-cloud-0.1.0rc0/cellshape_cloud/lightning_autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8334 2023-02-22 13:31:46.000000 cellshape-cloud-0.1.0rc0/cellshape_cloud/lightning_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-02-22 13:31:46.000000 cellshape-cloud-0.1.0rc0/cellshape_cloud/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-02-22 13:31:46.000000 cellshape-cloud-0.1.0rc0/cellshape_cloud/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)    14805 2023-02-22 13:31:46.000000 cellshape-cloud-0.1.0rc0/cellshape_cloud/pointcloud_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-02-22 13:31:46.000000 cellshape-cloud-0.1.0rc0/cellshape_cloud/reports.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-22 13:31:46.000000 cellshape-cloud-0.1.0rc0/cellshape_cloud/simclr_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-02-22 13:31:46.000000 cellshape-cloud-0.1.0rc0/cellshape_cloud/train_autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-02-22 13:31:46.000000 cellshape-cloud-0.1.0rc0/cellshape_cloud/training_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-02-22 13:31:46.000000 cellshape-cloud-0.1.0rc0/cellshape_cloud/transformations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 13:32:00.699040 cellshape-cloud-0.1.0rc0/cellshape_cloud/vendor/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-02-22 13:31:46.000000 cellshape-cloud-0.1.0rc0/cellshape_cloud/vendor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-02-22 13:31:46.000000 cellshape-cloud-0.1.0rc0/cellshape_cloud/vendor/chamfer_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-02-22 13:31:46.000000 cellshape-cloud-0.1.0rc0/cellshape_cloud/vendor/decoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     7767 2023-02-22 13:31:46.000000 cellshape-cloud-0.1.0rc0/cellshape_cloud/vendor/encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-02-22 13:31:46.000000 cellshape-cloud-0.1.0rc0/cellshape_cloud/vendor/graph_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 13:32:00.695040 cellshape-cloud-0.1.0rc0/cellshape_cloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-02-22 13:32:00.000000 cellshape-cloud-0.1.0rc0/cellshape_cloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-02-22 13:32:00.000000 cellshape-cloud-0.1.0rc0/cellshape_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-22 13:32:00.000000 cellshape-cloud-0.1.0rc0/cellshape_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-22 13:32:00.000000 cellshape-cloud-0.1.0rc0/cellshape_cloud.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-02-22 13:32:00.000000 cellshape-cloud-0.1.0rc0/cellshape_cloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-22 13:32:00.000000 cellshape-cloud-0.1.0rc0/cellshape_cloud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-02-22 13:31:46.000000 cellshape-cloud-0.1.0rc0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-02-22 13:32:00.699040 cellshape-cloud-0.1.0rc0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-02-22 13:31:46.000000 cellshape-cloud-0.1.0rc0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 13:32:00.699040 cellshape-cloud-0.1.0rc0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-22 13:31:46.000000 cellshape-cloud-0.1.0rc0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 13:32:00.699040 cellshape-cloud-0.1.0rc0/tests/test_integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-22 13:31:46.000000 cellshape-cloud-0.1.0rc0/tests/test_integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 13:32:00.699040 cellshape-cloud-0.1.0rc0/tests/test_unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-22 13:31:46.000000 cellshape-cloud-0.1.0rc0/tests/test_unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-02-22 13:31:46.000000 cellshape-cloud-0.1.0rc0/tests/test_unit/test_placeholder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:16:51.879791 cellshape-cloud-0.1.1rc0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-26 14:16:34.000000 cellshape-cloud-0.1.1rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-26 14:16:34.000000 cellshape-cloud-0.1.1rc0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-04-26 14:16:51.879791 cellshape-cloud-0.1.1rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-04-26 14:16:34.000000 cellshape-cloud-0.1.1rc0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:16:51.875791 cellshape-cloud-0.1.1rc0/cellshape_cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-26 14:16:34.000000 cellshape-cloud-0.1.1rc0/cellshape_cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-04-26 14:16:34.000000 cellshape-cloud-0.1.1rc0/cellshape_cloud/cloud_autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-04-26 14:16:34.000000 cellshape-cloud-0.1.1rc0/cellshape_cloud/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-26 14:16:34.000000 cellshape-cloud-0.1.1rc0/cellshape_cloud/extract_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-26 14:16:34.000000 cellshape-cloud-0.1.1rc0/cellshape_cloud/helper_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-04-26 14:16:34.000000 cellshape-cloud-0.1.1rc0/cellshape_cloud/lightning_autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10169 2023-04-26 14:16:34.000000 cellshape-cloud-0.1.1rc0/cellshape_cloud/lightning_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-04-26 14:16:34.000000 cellshape-cloud-0.1.1rc0/cellshape_cloud/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-04-26 14:16:34.000000 cellshape-cloud-0.1.1rc0/cellshape_cloud/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15503 2023-04-26 14:16:34.000000 cellshape-cloud-0.1.1rc0/cellshape_cloud/pointcloud_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-04-26 14:16:34.000000 cellshape-cloud-0.1.1rc0/cellshape_cloud/reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 14:16:34.000000 cellshape-cloud-0.1.1rc0/cellshape_cloud/simclr_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-04-26 14:16:34.000000 cellshape-cloud-0.1.1rc0/cellshape_cloud/train_autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-04-26 14:16:34.000000 cellshape-cloud-0.1.1rc0/cellshape_cloud/training_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-04-26 14:16:34.000000 cellshape-cloud-0.1.1rc0/cellshape_cloud/transformations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:16:51.879791 cellshape-cloud-0.1.1rc0/cellshape_cloud/vendor/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-26 14:16:34.000000 cellshape-cloud-0.1.1rc0/cellshape_cloud/vendor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-26 14:16:34.000000 cellshape-cloud-0.1.1rc0/cellshape_cloud/vendor/chamfer_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-04-26 14:16:34.000000 cellshape-cloud-0.1.1rc0/cellshape_cloud/vendor/decoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7767 2023-04-26 14:16:34.000000 cellshape-cloud-0.1.1rc0/cellshape_cloud/vendor/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-26 14:16:34.000000 cellshape-cloud-0.1.1rc0/cellshape_cloud/vendor/graph_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:16:51.879791 cellshape-cloud-0.1.1rc0/cellshape_cloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-04-26 14:16:51.000000 cellshape-cloud-0.1.1rc0/cellshape_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-04-26 14:16:51.000000 cellshape-cloud-0.1.1rc0/cellshape_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 14:16:51.000000 cellshape-cloud-0.1.1rc0/cellshape_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 14:16:51.000000 cellshape-cloud-0.1.1rc0/cellshape_cloud.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-26 14:16:51.000000 cellshape-cloud-0.1.1rc0/cellshape_cloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-26 14:16:51.000000 cellshape-cloud-0.1.1rc0/cellshape_cloud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-26 14:16:34.000000 cellshape-cloud-0.1.1rc0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-26 14:16:51.879791 cellshape-cloud-0.1.1rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-04-26 14:16:34.000000 cellshape-cloud-0.1.1rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:16:51.879791 cellshape-cloud-0.1.1rc0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 14:16:34.000000 cellshape-cloud-0.1.1rc0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:16:51.879791 cellshape-cloud-0.1.1rc0/tests/test_integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 14:16:34.000000 cellshape-cloud-0.1.1rc0/tests/test_integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:16:51.879791 cellshape-cloud-0.1.1rc0/tests/test_unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 14:16:34.000000 cellshape-cloud-0.1.1rc0/tests/test_unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-26 14:16:34.000000 cellshape-cloud-0.1.1rc0/tests/test_unit/test_placeholder.py
```

### Comparing `cellshape-cloud-0.1.0rc0/LICENSE` & `cellshape-cloud-0.1.1rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `cellshape-cloud-0.1.0rc0/PKG-INFO` & `cellshape-cloud-0.1.1rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellshape-cloud
-Version: 0.1.0rc0
+Version: 0.1.1rc0
 Summary: 3D cell shape analysis using geometric deep learning on point clouds
 Author: Matt De Vries, Lucas Dent, Adam Tyson
 Author-email: mattdevries.ai@gmail.com
 Project-URL: Source Code, https://github.com/Sentinal4D/cellshape-cloud
 Project-URL: Bug Tracker, https://github.com/Sentinal4D/cellshape-cloud/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `cellshape-cloud-0.1.0rc0/README.md` & `cellshape-cloud-0.1.1rc0/README.md`

 * *Files identical despite different names*

### Comparing `cellshape-cloud-0.1.0rc0/cellshape_cloud/cloud_autoencoder.py` & `cellshape-cloud-0.1.1rc0/cellshape_cloud/cloud_autoencoder.py`

 * *Files identical despite different names*

### Comparing `cellshape-cloud-0.1.0rc0/cellshape_cloud/extract.py` & `cellshape-cloud-0.1.1rc0/cellshape_cloud/extract.py`

 * *Files identical despite different names*

### Comparing `cellshape-cloud-0.1.0rc0/cellshape_cloud/extract_features.py` & `cellshape-cloud-0.1.1rc0/cellshape_cloud/extract_features.py`

 * *Files identical despite different names*

### Comparing `cellshape-cloud-0.1.0rc0/cellshape_cloud/lightning_autoencoder.py` & `cellshape-cloud-0.1.1rc0/cellshape_cloud/lightning_autoencoder.py`

 * *Files identical despite different names*

### Comparing `cellshape-cloud-0.1.0rc0/cellshape_cloud/lightning_classifier.py` & `cellshape-cloud-0.1.1rc0/cellshape_cloud/lightning_classifier.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,98 @@
 import torch
 from pytorch_lightning.callbacks import ModelCheckpoint
 from torch import nn
 from torch.utils.data import DataLoader, WeightedRandomSampler
 
 import pytorch_lightning as pl
 from torchmetrics import Accuracy, AUROC
-from pointcloud_dataset import VesselMNIST3D
+from pointcloud_dataset import VesselMNIST3D, SingleCellDataset
 
 from vendor.encoders import DGCNNEncoder
 
 
 def make_weights_for_balanced_classes(images, classes, nclasses=2):
     n_images = len(images)
+
     count_per_class = [150, 1185]
     weight_per_class = [0.0] * nclasses
     for i in range(nclasses):
         weight_per_class[i] = float(n_images) / float(count_per_class[i])
     weights = [0] * n_images
     for idx, image_class in enumerate(classes):
         weights[idx] = weight_per_class[image_class]
     return weights
 
 
+class SingleCellDataModule(pl.LightningDataModule):
+    def __init__(
+        self,
+        annotations_file="/home/mvries/Documents/Datasets/OPM/"
+        "SingleCellFromNathan_17122021/all_data_removedwrong"
+        "_ori_removedTwo_train_test.csv",
+        points_dir="/home/mvries/Documents/Datasets/OPM/"
+        "SingleCellFromNathan_17122021",
+        img_size=400,
+        transform=None,
+        cell_component="cell",
+        num_points=2048,
+        batch_size=16,
+    ):
+        super().__init__()
+        self.annot_df = annotations_file
+        self.img_dir = points_dir
+        self.img_size = img_size
+        self.transform = transform
+        self.cell_component = cell_component
+        self.num_points = num_points
+        self.batch_size = batch_size
+
+    def setup(self, stage=None):
+        self.train_dset = SingleCellDataset(
+            annotations_file=self.annot_df,
+            points_dir=self.img_dir,
+            partition="train",
+        )
+
+        self.val_dset = SingleCellDataset(
+            annotations_file=self.annot_df,
+            points_dir=self.img_dir,
+            partition="val",
+        )
+
+        self.test_dset = SingleCellDataset(
+            annotations_file=self.annot_df,
+            points_dir=self.img_dir,
+            partition="test",
+        )
+
+    def train_dataloader(self):
+        return DataLoader(
+            self.train_dset, batch_size=self.batch_size, shuffle=True
+        )
+
+    def val_dataloader(self):
+        return DataLoader(
+            self.val_dset, batch_size=self.batch_size, shuffle=True
+        )
+
+    def test_dataloader(self):
+        return DataLoader(
+            self.test_dset, batch_size=self.batch_size, shuffle=True
+        )
+
+
 class VesselDataModule(pl.LightningDataModule):
     """Cassava DataModule for Lightning"""
 
     def __init__(
         self,
         transform=None,
         batch_size=16,
-        points_dir="/home/mvries/Documents/Datasets/MedMNIST/vesselmnist3d/",
+        points_dir="/mnt/nvme0n1/Datasets/MedMNIST/vesselmnist3d/",
     ):
         super().__init__()
         self.batch_size = batch_size
         self.transform = transform
         self.points_dir = points_dir
 
     def setup(self, stage=None):
@@ -63,32 +122,32 @@
         return DataLoader(self.vessel_val, batch_size=self.batch_size)
 
     def test_dataloader(self):
         return DataLoader(self.vessel_test, batch_size=self.batch_size)
 
 
 class CloudClassifierPL(pl.LightningModule):
-    def __init__(self, criterion=nn.BCEWithLogitsLoss(), num_classes=2):
+    def __init__(self, criterion=nn.CrossEntropyLoss(), num_classes=10):
         super(CloudClassifierPL, self).__init__()
 
         self.save_hyperparameters(ignore=["criterion", "model"])
         self.lr = 0.00001
         self.criterion = criterion
-        self.model = DGCNNEncoder(num_features=1)
+        self.model = DGCNNEncoder(num_features=num_classes)
         self.num_classes = num_classes
         self.accuracy_macro = Accuracy(
-            task="binary", num_classes=2, average="macro"
+            task="binary", num_classes=num_classes, average="macro"
         )
         self.accuracy_micro = Accuracy(
-            task="binary", num_classes=2, average="micro"
+            task="binary", num_classes=num_classes, average="micro"
         )
         self.accuracy_weighted = Accuracy(
-            task="binary", num_classes=2, average="weighted"
+            task="binary", num_classes=num_classes, average="weighted"
         )
-        self.AUC = AUROC(task="binary")
+        self.AUC = AUROC(task="multiclass", num_classes=num_classes)
 
     def configure_optimizers(self):
         optimizer = torch.optim.Adam(
             self.parameters(),
             lr=self.lr,
             betas=(0.9, 0.999),
             weight_decay=1e-6,
@@ -146,17 +205,17 @@
                 print("    Found weight: " + k)
 
         self.model.load_state_dict(model_dict)
 
     def training_step(self, batch, batch_idx):
         inputs, labels = batch[0], batch[1]
         outputs = self.model(inputs)
-
-        loss = self.criterion(outputs, torch.unsqueeze(labels, 1).float())
-        preds = torch.sigmoid(outputs) > 0.5
+        labels = torch.squeeze(labels)
+        loss = self.criterion(outputs, labels)
+        preds = torch.sigmoid(outputs)
         acc = self.accuracy_weighted(torch.squeeze(preds), labels)
         self.log("train_loss", loss, on_step=True, on_epoch=True, logger=True)
         self.log(
             "train_acc",
             acc,
             on_step=True,
             on_epoch=True,
@@ -165,28 +224,27 @@
         )
         dic = {"loss": loss, "acc": acc}
         return dic
 
     def validation_step(self, batch, batch_idx):
         inputs, labels = batch[0], batch[1]
         outputs = self.model(inputs)
-
-        loss = self.criterion(outputs, torch.unsqueeze(labels, 1).float())
-        preds = torch.argmax(outputs, dim=1)
+        labels = torch.squeeze(labels)
+        loss = self.criterion(outputs, labels)
+        preds = torch.sigmoid(outputs)
         acc = self.accuracy_weighted(preds, labels)
         self.log("val_loss", loss, on_step=True, on_epoch=True, logger=True)
         self.log("val_acc", acc, on_step=True, on_epoch=True, logger=True)
 
     def test_step(self, batch, batch_idx):
         inputs, labels = batch[0], batch[1]
         outputs = self.model(inputs)
-
-        loss = self.criterion(outputs, torch.unsqueeze(labels, 1).float())
-        preds = torch.sigmoid(outputs) > 0.5
-        print(torch.sigmoid(outputs))
+        labels = torch.squeeze(labels)
+        loss = self.criterion(torch.squeeze(outputs), labels)
+        preds = torch.sigmoid(outputs)
 
         acc_macro = self.accuracy_macro(torch.squeeze(preds), labels)
         acc_micro = self.accuracy_micro(torch.squeeze(preds), labels)
         acc_weighted = self.accuracy_weighted(torch.squeeze(preds), labels)
         auc = self.AUC(torch.squeeze(torch.sigmoid(outputs)), labels)
         self.log("test_loss", loss, on_step=True, on_epoch=True, logger=True)
         self.log(
@@ -223,19 +281,22 @@
             pass
 
         def on_train_end(self, trainer, pl_module):
             # instead, do it at the end of training loop
             self._run_early_stopping_check(trainer)
 
     warnings.simplefilter("ignore", UserWarning)
-    model = CloudClassifierPL().load_from_checkpoint(
-        checkpoint_path="/home/mvries/Documents/GitHub/cellshape-cloud/"
-        "lightning_logs/version_52/checkpoints/epoch=132-step=11172.ckpt"
-    )
+    model = CloudClassifierPL(num_classes=5)
+    # .load_from_checkpoint(
+    # checkpoint_path="/home/mvries/Documents/GitHub/cellshape-cloud/"
+    # "lightning_logs/version_52/checkpoints/epoch=132-step=11172.ckpt"
+    # )
     checkpoint_callback = ModelCheckpoint(monitor="val_loss")
 
-    vessel_data = VesselDataModule()
-    vessel_data.setup()
-    trainer = pl.Trainer(gpus=1, callbacks=[checkpoint_callback])
+    cell_data = SingleCellDataModule()
+    cell_data.setup()
+    trainer = pl.Trainer(
+        accelerator="gpu", devices=1, callbacks=[checkpoint_callback]
+    )
 
-    # trainer.fit(model, vessel_data)
-    trainer.test(model=model, datamodule=vessel_data)
+    trainer.fit(model, cell_data)
+    trainer.test(model=model, datamodule=cell_data)
```

### Comparing `cellshape-cloud-0.1.0rc0/cellshape_cloud/main.py` & `cellshape-cloud-0.1.1rc0/cellshape_cloud/main.py`

 * *Files identical despite different names*

### Comparing `cellshape-cloud-0.1.0rc0/cellshape_cloud/plotting.py` & `cellshape-cloud-0.1.1rc0/cellshape_cloud/plotting.py`

 * *Files identical despite different names*

### Comparing `cellshape-cloud-0.1.0rc0/cellshape_cloud/pointcloud_dataset.py` & `cellshape-cloud-0.1.1rc0/cellshape_cloud/pointcloud_dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,34 +44,50 @@
         self,
         annotations_file,
         points_dir,
         img_size=400,
         transform=None,
         cell_component="cell",
         num_points=2048,
+        partition="all",
     ):
         self.annot_df = pd.read_csv(annotations_file)
         self.img_dir = points_dir
         self.img_size = img_size
         self.transform = transform
         self.cell_component = cell_component
         self.num_points = num_points
+        self.partition = partition
+        if self.partition != "all":
 
-        self.new_df = self.annot_df[
-            (self.annot_df.xDim <= self.img_size)
-            & (self.annot_df.yDim <= self.img_size)
-            & (self.annot_df.zDim <= self.img_size)
-        ].reset_index(drop=True)
+            self.new_df = self.annot_df[
+                (self.annot_df.xDim <= self.img_size)
+                & (self.annot_df.yDim <= self.img_size)
+                & (self.annot_df.zDim <= self.img_size)
+                & (self.annot_df.Splits == self.partition)
+            ].reset_index(drop=True)
+        else:
+            self.new_df = self.annot_df[
+                (self.annot_df.xDim <= self.img_size)
+                & (self.annot_df.yDim <= self.img_size)
+                & (self.annot_df.zDim <= self.img_size)
+            ].reset_index(drop=True)
+
+        from sklearn import preprocessing
+
+        self.le = preprocessing.LabelEncoder()
+        self.le.fit(self.new_df["Treatment"].values)
 
     def __len__(self):
         return len(self.new_df)
 
     def __getitem__(self, idx):
         # read the image
         treatment = self.new_df.loc[idx, "Treatment"]
+        # class_id = self.new_df.loc[idx, "Class"]
         plate_num = "Plate" + str(self.new_df.loc[idx, "PlateNumber"])
         if self.num_points == 4096:
             num_str = "_4096"
         elif self.num_points == 1024:
             num_str = "_1024"
         else:
             num_str = ""
@@ -95,16 +111,16 @@
         image = (image - mean) / std
 
         # return the classical features as torch tensor
         feats = self.new_df.iloc[idx, 16:-4]
         feats = torch.tensor(feats)
 
         serial_number = self.new_df.loc[idx, "serialNumber"]
-
-        return image, treatment, feats, serial_number
+        enc_labels = torch.tensor(self.le.transform([treatment]))
+        return image, enc_labels, treatment, serial_number
 
 
 class GefGapDataset(Dataset):
     def __init__(
         self,
         annotations_file,
         img_dir,
```

### Comparing `cellshape-cloud-0.1.0rc0/cellshape_cloud/reports.py` & `cellshape-cloud-0.1.1rc0/cellshape_cloud/reports.py`

 * *Files identical despite different names*

### Comparing `cellshape-cloud-0.1.0rc0/cellshape_cloud/train_autoencoder.py` & `cellshape-cloud-0.1.1rc0/cellshape_cloud/train_autoencoder.py`

 * *Files identical despite different names*

### Comparing `cellshape-cloud-0.1.0rc0/cellshape_cloud/training_functions.py` & `cellshape-cloud-0.1.1rc0/cellshape_cloud/training_functions.py`

 * *Files identical despite different names*

### Comparing `cellshape-cloud-0.1.0rc0/cellshape_cloud/transformations.py` & `cellshape-cloud-0.1.1rc0/cellshape_cloud/transformations.py`

 * *Files identical despite different names*

### Comparing `cellshape-cloud-0.1.0rc0/cellshape_cloud/vendor/chamfer_distance.py` & `cellshape-cloud-0.1.1rc0/cellshape_cloud/vendor/chamfer_distance.py`

 * *Files identical despite different names*

### Comparing `cellshape-cloud-0.1.0rc0/cellshape_cloud/vendor/decoders.py` & `cellshape-cloud-0.1.1rc0/cellshape_cloud/vendor/decoders.py`

 * *Files identical despite different names*

### Comparing `cellshape-cloud-0.1.0rc0/cellshape_cloud/vendor/encoders.py` & `cellshape-cloud-0.1.1rc0/cellshape_cloud/vendor/encoders.py`

 * *Files identical despite different names*

### Comparing `cellshape-cloud-0.1.0rc0/cellshape_cloud/vendor/graph_functions.py` & `cellshape-cloud-0.1.1rc0/cellshape_cloud/vendor/graph_functions.py`

 * *Files identical despite different names*

### Comparing `cellshape-cloud-0.1.0rc0/cellshape_cloud.egg-info/PKG-INFO` & `cellshape-cloud-0.1.1rc0/cellshape_cloud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellshape-cloud
-Version: 0.1.0rc0
+Version: 0.1.1rc0
 Summary: 3D cell shape analysis using geometric deep learning on point clouds
 Author: Matt De Vries, Lucas Dent, Adam Tyson
 Author-email: mattdevries.ai@gmail.com
 Project-URL: Source Code, https://github.com/Sentinal4D/cellshape-cloud
 Project-URL: Bug Tracker, https://github.com/Sentinal4D/cellshape-cloud/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `cellshape-cloud-0.1.0rc0/cellshape_cloud.egg-info/SOURCES.txt` & `cellshape-cloud-0.1.1rc0/cellshape_cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cellshape-cloud-0.1.0rc0/setup.cfg` & `cellshape-cloud-0.1.1rc0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.1.0-rc0
+current_version = 0.1.1-rc0
 commit = True
 tag = True
 tag_name = {new_version}
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\-(?P<release>[a-z]+)(?P<rc>\d+))?
 serialize = 
 	{major}.{minor}.{patch}-{release}{rc}
 	{major}.{minor}.{patch}
```

### Comparing `cellshape-cloud-0.1.0rc0/setup.py` & `cellshape-cloud-0.1.1rc0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,19 +13,20 @@
     "numpy==1.21",
     "matplotlib",
     "tqdm",
     "datetime",
     "umap-learn",
     "scikit-learn",
     "tensorboard",
+    "h5py",
 ]
 
 setup(
     name="cellshape-cloud",
-    version="0.1.0-rc0",
+    version="0.1.1-rc0",
     description="3D cell shape analysis using geometric deep"
     " learning on point clouds",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=requirements,
     extras_require={
         "dev": [
```

