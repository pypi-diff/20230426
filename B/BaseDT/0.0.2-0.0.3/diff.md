# Comparing `tmp/BaseDT-0.0.2.tar.gz` & `tmp/BaseDT-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/BaseDT-0.0.2.tar", last modified: Thu Apr  6 03:46:24 2023, max compression
+gzip compressed data, was "dist/BaseDT-0.0.3.tar", last modified: Wed Apr 26 07:41:42 2023, max compression
```

## Comparing `BaseDT-0.0.2.tar` & `BaseDT-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-04-06 03:46:24.000000 BaseDT-0.0.2/
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-04-06 03:46:24.000000 BaseDT-0.0.2/BaseDT/
--rw-rw-r--   0 user      (1001) user      (1001)        0 2023-03-31 03:16:28.000000 BaseDT-0.0.2/BaseDT/__init__.py
--rw-rw-r--   0 user      (1001) user      (1001)    16855 2023-03-31 03:16:28.000000 BaseDT-0.0.2/BaseDT/data.py
--rw-rw-r--   0 user      (1001) user      (1001)    12037 2023-03-31 03:16:28.000000 BaseDT-0.0.2/BaseDT/data_image.py
--rw-rw-r--   0 user      (1001) user      (1001)    31309 2023-03-31 03:16:28.000000 BaseDT-0.0.2/BaseDT/dataset.py
--rw-rw-r--   0 user      (1001) user      (1001)     1020 2023-03-31 03:16:28.000000 BaseDT-0.0.2/BaseDT/io.py
--rw-rw-r--   0 user      (1001) user      (1001)     5409 2023-03-31 03:16:28.000000 BaseDT-0.0.2/BaseDT/plot.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-04-06 03:46:24.000000 BaseDT-0.0.2/BaseDT.egg-info/
--rw-rw-r--   0 user      (1001) user      (1001)      314 2023-04-06 03:46:24.000000 BaseDT-0.0.2/BaseDT.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1001) user      (1001)      316 2023-04-06 03:46:24.000000 BaseDT-0.0.2/BaseDT.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1001) user      (1001)        1 2023-04-06 03:46:24.000000 BaseDT-0.0.2/BaseDT.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1001) user      (1001)       30 2023-04-06 03:46:24.000000 BaseDT-0.0.2/BaseDT.egg-info/requires.txt
--rw-rw-r--   0 user      (1001) user      (1001)        7 2023-04-06 03:46:24.000000 BaseDT-0.0.2/BaseDT.egg-info/top_level.txt
--rw-rw-r--   0 user      (1001) user      (1001)        1 2023-02-02 07:26:47.000000 BaseDT-0.0.2/BaseDT.egg-info/zip-safe
--rw-rw-r--   0 user      (1001) user      (1001)       40 2023-04-06 03:45:54.000000 BaseDT-0.0.2/MANIFEST.in
--rw-rw-r--   0 user      (1001) user      (1001)      314 2023-04-06 03:46:24.000000 BaseDT-0.0.2/PKG-INFO
--rw-rw-r--   0 user      (1001) user      (1001)       30 2023-02-02 07:23:17.000000 BaseDT-0.0.2/install_requires.txt
--rw-rw-r--   0 user      (1001) user      (1001)       38 2023-04-06 03:46:24.000000 BaseDT-0.0.2/setup.cfg
--rw-rw-r--   0 user      (1001) user      (1001)     4245 2023-04-06 03:45:24.000000 BaseDT-0.0.2/setup.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-04-26 07:41:42.000000 BaseDT-0.0.3/
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-04-26 07:41:42.000000 BaseDT-0.0.3/BaseDT/
+-rw-rw-r--   0 user      (1001) user      (1001)        0 2023-04-26 07:17:02.000000 BaseDT-0.0.3/BaseDT/__init__.py
+-rw-rw-r--   0 user      (1001) user      (1001)    16851 2023-04-26 07:17:02.000000 BaseDT-0.0.3/BaseDT/data.py
+-rw-rw-r--   0 user      (1001) user      (1001)    12037 2023-04-26 07:17:02.000000 BaseDT-0.0.3/BaseDT/data_image.py
+-rw-rw-r--   0 user      (1001) user      (1001)    31309 2023-04-26 07:17:02.000000 BaseDT-0.0.3/BaseDT/dataset.py
+-rw-rw-r--   0 user      (1001) user      (1001)     1020 2023-04-26 07:17:02.000000 BaseDT-0.0.3/BaseDT/io.py
+-rw-rw-r--   0 user      (1001) user      (1001)     6986 2023-04-26 07:19:34.000000 BaseDT-0.0.3/BaseDT/plot.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-04-26 07:41:42.000000 BaseDT-0.0.3/BaseDT.egg-info/
+-rw-rw-r--   0 user      (1001) user      (1001)      314 2023-04-26 07:41:41.000000 BaseDT-0.0.3/BaseDT.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1001) user      (1001)      316 2023-04-26 07:41:41.000000 BaseDT-0.0.3/BaseDT.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1001) user      (1001)        1 2023-04-26 07:41:41.000000 BaseDT-0.0.3/BaseDT.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1001) user      (1001)       30 2023-04-26 07:41:41.000000 BaseDT-0.0.3/BaseDT.egg-info/requires.txt
+-rw-rw-r--   0 user      (1001) user      (1001)        7 2023-04-26 07:41:41.000000 BaseDT-0.0.3/BaseDT.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1001) user      (1001)        1 2023-02-02 07:26:47.000000 BaseDT-0.0.3/BaseDT.egg-info/zip-safe
+-rw-rw-r--   0 user      (1001) user      (1001)       40 2023-04-06 03:45:54.000000 BaseDT-0.0.3/MANIFEST.in
+-rw-rw-r--   0 user      (1001) user      (1001)      314 2023-04-26 07:41:42.000000 BaseDT-0.0.3/PKG-INFO
+-rw-rw-r--   0 user      (1001) user      (1001)       30 2023-02-02 07:23:17.000000 BaseDT-0.0.3/install_requires.txt
+-rw-rw-r--   0 user      (1001) user      (1001)       38 2023-04-26 07:41:42.000000 BaseDT-0.0.3/setup.cfg
+-rw-rw-r--   0 user      (1001) user      (1001)     4245 2023-04-26 07:40:56.000000 BaseDT-0.0.3/setup.py
```

### Comparing `BaseDT-0.0.2/BaseDT/data.py` & `BaseDT-0.0.3/BaseDT/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -397,15 +397,15 @@
         pass
    
 class ModelData(object):
 
     def __init__(self, path):
         self.path = path
 
-    def extract_labels(self):
+    def get_labels(self):
         assert isinstance(self.path, str)
         file_path = self.path
         class_name = []
         key = 'CLASSES'
         if file_path[-3:] == 'txt':
             with open(file_path, 'r') as f:
                 class_name = [tag.strip() for tag in f.readlines()]
```

### Comparing `BaseDT-0.0.2/BaseDT/data_image.py` & `BaseDT-0.0.3/BaseDT/data_image.py`

 * *Files identical despite different names*

### Comparing `BaseDT-0.0.2/BaseDT/dataset.py` & `BaseDT-0.0.3/BaseDT/dataset.py`

 * *Files identical despite different names*

### Comparing `BaseDT-0.0.2/BaseDT/io.py` & `BaseDT-0.0.3/BaseDT/io.py`

 * *Files identical despite different names*

### Comparing `BaseDT-0.0.2/BaseDT/plot.py` & `BaseDT-0.0.3/BaseDT/plot.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import cv2
 import numpy as np
 from enum import Enum
 import matplotlib.pyplot as plt
+import json
 # def draw_boxes(image, boxes, labels = None, color=(0, 0, 255), thickness=2):
 #     font_scale = image.shape[0] / 500
 #     font = cv2.FONT_HERSHEY_SIMPLEX
 #     for box, label in zip(boxes, labels):
 #         x1, y1, x2, y2 = box
 #         cv2.rectangle(image, (x1, y1), (x2, y2), color, thickness)
 #         text_size = cv2.getTextSize(label, font, font_scale, thickness)[0]
@@ -79,16 +80,15 @@
                 if closed or ret != -1:
                     break
         else:
             ret = cv2.waitKey(wait_time)
     else:
         plt.imshow(img)
         plt.show()
-
-
+        
 def imshow_det_bboxes(img,
                       bboxes,
                       labels,
                       class_names=None,
                       score_thr=0,
                       bbox_color=None,
                       text_color=None,
@@ -117,15 +117,17 @@
     """
     bboxes = np.array(bboxes)
     labels = np.array(labels)
     assert bboxes.ndim == 2
     assert labels.ndim == 1
     assert bboxes.shape[0] == labels.shape[0]
     assert bboxes.shape[1] == 4 or bboxes.shape[1] == 5
-    img = cv2.imread(img)
+    assert isinstance(img,str) or isinstance(img, np.ndarray)
+    if isinstance(img, str):
+        img = cv2.imread(img)
     img = np.ascontiguousarray(img)
 
     if score_thr > 0:
         assert bboxes.shape[1] == 5
         scores = bboxes[:, -1]
         inds = scores > score_thr
         bboxes = bboxes[inds, :]
@@ -150,8 +152,55 @@
         if len(bbox) > 4:
             label_text += f'|{bbox[-1]:.02f}'
         cv2.putText(img, label_text, (bbox_int[0], bbox_int[1] - 2),
                     cv2.FONT_HERSHEY_COMPLEX, font_scale, text_color[idx])
 
     if show:
         imshow(img, win_name, wait_time)
-    return img
+    return img
+
+def plot_log(log, title='Loss Graph', plot_list='loss'):
+
+    if isinstance(plot_list, str):
+        plot_list = [plot_list]
+    elif isinstance(plot_list, (list, tuple)):
+        assert len(plot_list) == len(set(plot_list)), (
+            'Find duplicate elements in "plot_list".')
+    for key in plot_list:
+        assert key in ['loss','loss_cls','loss_bbox']
+
+    iter = []
+    loss_dict = {
+        'loss': [],
+        'loss_cls':[],
+        'loss_bbox':[]
+    }
+
+    iter_num = 0
+
+    if isinstance(log, str):
+        with open(log,'r') as f:
+            content = [json.loads(line) for line in f.readlines()]
+    elif isinstance(log, list):
+        content = log
+    
+    assert isinstance(content, list)
+    for log in content:
+        if 'mode' in log.keys() and log["mode"] == 'train':
+            iter_num += 10
+            iter.append(iter_num)
+            non_empty_keys = log.keys()
+            for axis_y in plot_list:
+                loss_dict[axis_y].append(log[axis_y])
+
+    plt.figure(figsize=(8,6))
+    for axis_y in plot_list:
+        plt.plot(iter,loss_dict[axis_y],'',label=axis_y)
+    plt.title(title)
+    plt.legend(loc='upper right')
+    plt.xlabel('iter')
+    plt.ylabel('')
+    plt.grid(True)
+    plt.show()
+    non_empty_keys = [key for key in non_empty_keys if key.startswith('loss')]
+    print('The loss function graph is drawn. If you want to add y-axis parameters,'
+          f' please set `{non_empty_keys}` in the plot_list')
```

### Comparing `BaseDT-0.0.2/setup.py` & `BaseDT-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
                 yield item
 
     packages = list(gen_packages_items())
     return packages
 
 setup(
     name='BaseDT',
-    version='0.0.2',
+    version='0.0.3',
     # version='0.0.1rc1',
     description='BaseDT is a data-processing  tool including data, dataset, io and plot.',
     license='MIT License',
     author='OpenXLab',
     author_email='wangbolun@pjlab.org.cn',
     url='https://github.com/OpenXLab-Edu/OpenMMLab-Edu',
     packages=find_packages(),
```

