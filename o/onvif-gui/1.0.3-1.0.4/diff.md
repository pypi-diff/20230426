# Comparing `tmp/onvif-gui-1.0.3.tar.gz` & `tmp/onvif-gui-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onvif-gui-1.0.3.tar", last modified: Sun Apr 23 02:57:19 2023, max compression
+gzip compressed data, was "onvif-gui-1.0.4.tar", last modified: Tue Apr 25 16:18:44 2023, max compression
```

## Comparing `onvif-gui-1.0.3.tar` & `onvif-gui-1.0.4.tar`

### file list

```diff
@@ -1,271 +1,270 @@
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:57:19.759837 onvif-gui-1.0.3/
--rw-r--r--   0 stephen   (1000) stephen   (1000)    11357 2023-04-21 03:11:06.000000 onvif-gui-1.0.3/LICENSE
--rw-r--r--   0 stephen   (1000) stephen   (1000)       65 2023-04-22 12:44:29.000000 onvif-gui-1.0.3/MANIFEST.in
--rw-r--r--   0 stephen   (1000) stephen   (1000)     8710 2023-04-23 02:57:19.759837 onvif-gui-1.0.3/PKG-INFO
--rw-r--r--   0 stephen   (1000) stephen   (1000)     8171 2023-04-23 02:28:18.000000 onvif-gui-1.0.3/README.md
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:57:19.723837 onvif-gui-1.0.3/onvif_gui/
--rw-r--r--   0 stephen   (1000) stephen   (1000)       28 2023-04-21 01:55:37.000000 onvif-gui-1.0.3/onvif_gui/__init__.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:57:19.723837 onvif-gui-1.0.3/onvif_gui/components/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      196 2023-04-21 00:50:17.000000 onvif-gui-1.0.3/onvif_gui/components/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1743 2023-04-21 18:19:18.000000 onvif-gui-1.0.3/onvif_gui/components/comboselector.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     2236 2023-04-21 18:19:18.000000 onvif-gui-1.0.3/onvif_gui/components/fileselector.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     5320 2023-04-21 18:19:18.000000 onvif-gui-1.0.3/onvif_gui/components/labelselector.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     4073 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/components/progress.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1143 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/components/thresholdslider.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:57:19.723837 onvif-gui-1.0.3/onvif_gui/detectron2/
--rw-r--r--   0 stephen   (1000) stephen   (1000)       67 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/__init__.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:57:19.727837 onvif-gui-1.0.3/onvif_gui/detectron2/checkpoint/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      347 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/checkpoint/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    17770 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/checkpoint/c2_model_loading.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     5685 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/checkpoint/catalog.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     5258 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/checkpoint/detection_checkpoint.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:57:19.727837 onvif-gui-1.0.3/onvif_gui/detectron2/config/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      599 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/config/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     7890 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/config/compat.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     9211 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/config/config.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    29512 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/config/defaults.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     3015 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/config/instantiate.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    15378 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/config/lazy.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:57:19.727837 onvif-gui-1.0.3/onvif_gui/detectron2/configs/
--rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-04-20 14:25:53.000000 onvif-gui-1.0.3/onvif_gui/detectron2/configs/__init__.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:57:19.727837 onvif-gui-1.0.3/onvif_gui/detectron2/data/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      644 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/data/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     7378 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/data/benchmark.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    21231 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/data/build.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     7224 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/data/catalog.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     9162 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/data/common.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     8169 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/data/dataset_mapper.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:57:19.731837 onvif-gui-1.0.3/onvif_gui/detectron2/data/datasets/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      523 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/data/datasets/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    10174 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/data/datasets/builtin.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    21841 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/data/datasets/builtin_meta.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    13167 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/data/datasets/cityscapes.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     7821 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/data/datasets/cityscapes_panoptic.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    23465 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/data/datasets/coco.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     8977 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/data/datasets/coco_panoptic.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     9623 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/data/datasets/lvis.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)   223757 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/data/datasets/lvis_v0_5_categories.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)   219177 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/data/datasets/lvis_v1_categories.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    39414 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/data/datasets/lvis_v1_category_image_count.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     3128 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/data/datasets/pascal_voc.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)      169 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/data/datasets/register_coco.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    22841 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/data/detection_utils.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:57:19.731837 onvif-gui-1.0.3/onvif_gui/detectron2/data/samplers/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      412 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/data/samplers/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    11789 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/data/samplers/distributed_sampler.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1944 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/data/samplers/grouped_batch_sampler.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:57:19.731837 onvif-gui-1.0.3/onvif_gui/detectron2/data/transforms/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      466 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/data/transforms/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    14112 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/data/transforms/augmentation.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    23069 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/data/transforms/augmentation_impl.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    12629 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/data/transforms/transform.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:57:19.735837 onvif-gui-1.0.3/onvif_gui/detectron2/layers/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      874 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/layers/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     5764 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/layers/aspp.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    12131 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/layers/batch_norm.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     3024 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/layers/blocks.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    16978 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/layers/deform_conv.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     4202 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/layers/losses.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    10879 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/layers/mask_ops.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     6490 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/layers/nms.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     3098 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/layers/roi_align.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     3302 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/layers/roi_align_rotated.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)      652 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/layers/rotated_boxes.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)      537 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/layers/shape_spec.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     5123 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/layers/wrappers.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:57:19.735837 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1568 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    15439 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/anchor_generator.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:57:19.735837 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/backbone/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      598 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/backbone/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     2512 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/backbone/backbone.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1015 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/backbone/build.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    10360 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/backbone/fpn.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    15988 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/backbone/mvit.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    16656 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/backbone/regnet.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    23658 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/backbone/resnet.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    25095 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/backbone/swin.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     6360 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/backbone/utils.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    19338 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/backbone/vit.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    15123 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/box_regression.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     6264 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/matcher.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:57:19.739837 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/meta_arch/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      508 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/meta_arch/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)      814 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/meta_arch/build.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    11651 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/meta_arch/dense_detector.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    13213 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/meta_arch/fcos.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    10407 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/meta_arch/panoptic_fpn.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    13896 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/meta_arch/rcnn.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    18265 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/meta_arch/retinanet.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     9906 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/meta_arch/semantic_seg.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    10832 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/mmdet_wrapper.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    11316 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/poolers.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     4045 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/postprocessing.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:57:19.739837 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/proposal_generator/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      231 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/proposal_generator/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)      836 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/proposal_generator/build.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     8128 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/proposal_generator/proposal_utils.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    23814 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/proposal_generator/rpn.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     8807 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/proposal_generator/rrpn.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:57:19.739837 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/roi_heads/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      768 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/roi_heads/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     4077 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/roi_heads/box_head.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    12990 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/roi_heads/cascade_rcnn.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    25390 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/roi_heads/fast_rcnn.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    11156 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/roi_heads/keypoint_head.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    12169 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/roi_heads/mask_head.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    37701 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/roi_heads/roi_heads.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    11175 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/roi_heads/rotated_fast_rcnn.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     2334 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/sampling.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    12416 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/test_time_augmentation.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1780 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/predictor.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:57:19.739837 onvif-gui-1.0.3/onvif_gui/detectron2/structures/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      645 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/structures/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    14429 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/structures/boxes.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     5520 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/structures/image_list.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     6613 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/structures/instances.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     9030 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/structures/keypoints.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    19802 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/structures/masks.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    18853 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/structures/rotated_boxes.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     2707 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/tracker.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:57:19.743837 onvif-gui-1.0.3/onvif_gui/detectron2/utils/
--rw-r--r--   0 stephen   (1000) stephen   (1000)       51 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/utils/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     6017 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/utils/analysis.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     8391 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/utils/collect_env.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     4096 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/utils/colormap.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     5608 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/utils/comm.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1852 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/utils/develop.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     5644 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/utils/env.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    17022 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/utils/events.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1189 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/utils/file_io.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     7807 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/utils/logger.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     2583 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/utils/memory.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1874 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/utils/registry.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1064 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/utils/serialize.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    18113 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/utils/testing.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    11319 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/utils/video_visualizer.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    51159 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/utils/visualizer.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1996 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/glwidget.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    11956 2023-04-23 02:50:48.000000 onvif-gui-1.0.3/onvif_gui/main.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:57:19.743837 onvif-gui-1.0.3/onvif_gui/modules/
--rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-04-20 01:38:46.000000 onvif-gui-1.0.3/onvif_gui/modules/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     5981 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/modules/keypoint.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     4215 2023-04-21 18:19:18.000000 onvif-gui-1.0.3/onvif_gui/modules/retinanet.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     3006 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/modules/sample.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     6542 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/modules/segment.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    10603 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/modules/yolox.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:57:19.747837 onvif-gui-1.0.3/onvif_gui/onvif/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      191 2023-04-21 00:45:40.000000 onvif-gui-1.0.3/onvif_gui/onvif/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     5739 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/onvif/admintab.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     3955 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/onvif/imagetab.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     2421 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/onvif/logindialog.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     5243 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/onvif/networktab.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     5114 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/onvif/ptztab.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     4523 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/onvif/videotab.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:57:19.747837 onvif-gui-1.0.3/onvif_gui/panels/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      147 2023-04-21 01:42:06.000000 onvif-gui-1.0.3/onvif_gui/panels/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    13464 2023-04-21 18:25:08.000000 onvif-gui-1.0.3/onvif_gui/panels/camerapanel.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    14489 2023-04-22 12:51:02.000000 onvif-gui-1.0.3/onvif_gui/panels/filepanel.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     2737 2023-04-21 03:48:23.000000 onvif-gui-1.0.3/onvif_gui/panels/modulepanel.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    13192 2023-04-21 18:19:18.000000 onvif-gui-1.0.3/onvif_gui/panels/settingspanel.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:57:19.759837 onvif-gui-1.0.3/onvif_gui/resources/
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1126 2023-04-21 18:19:18.000000 onvif-gui-1.0.3/onvif_gui/resources/LICENSE
--rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-04-20 14:25:24.000000 onvif-gui-1.0.3/onvif_gui/resources/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)      252 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/apply.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      245 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/apply_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      244 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/apply_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      911 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/audio.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      536 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/audio_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      920 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/audio_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      203 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/branch_closed.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      219 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/branch_closed_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      211 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/branch_closed_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      199 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/branch_open.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      168 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/branch_open_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      172 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/branch_open_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      267 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/checked.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      235 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/checked_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      246 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/checked_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)    11948 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/darkstyle.qss
--rw-r--r--   0 stephen   (1000) stephen   (1000)      910 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/discover.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      849 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/discover_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      937 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/discover_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      425 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/fast-forward.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      253 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/fast-forward_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      433 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/fast-forward_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      641 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/mute.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      346 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/mute_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      618 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/mute_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      347 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/next.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      225 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/next_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      348 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/next_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)    46084 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/onvif_gui.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      172 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/pause.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      144 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/pause_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      149 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/pause_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      321 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/play.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      209 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/play_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      316 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/play_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      349 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/previous.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      232 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/previous_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      348 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/previous_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      324 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/radio-off.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      250 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/radio-off_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      324 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/radio-off_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      350 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/radio-on.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      263 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/radio-on_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      343 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/radio-on_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      395 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/record.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      394 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/record_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      425 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/record_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      408 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/recording.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      435 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/recording_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      532 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/recording_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)     2005 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/resources.qrc
--rw-r--r--   0 stephen   (1000) stephen   (1000)   120051 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/resources.rcc
--rw-r--r--   0 stephen   (1000) stephen   (1000)      454 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/rewind.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      250 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/rewind_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      457 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/rewind_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      187 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/small_arrow_left.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      183 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/small_arrow_left_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      189 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/small_arrow_left_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      162 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/small_arrow_up.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      160 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/small_arrow_up_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      161 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/small_arrow_up_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      158 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/stop.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      140 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/stop_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      151 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/stop_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      143 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/unchecked.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      142 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/unchecked_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      143 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/unchecked_lo.png
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:57:19.759837 onvif-gui-1.0.3/onvif_gui/yolox/
--rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-04-20 01:35:42.000000 onvif-gui-1.0.3/onvif_gui/yolox/__init__.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:57:19.759837 onvif-gui-1.0.3/onvif_gui/yolox/models/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      936 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/yolox/models/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     4894 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/yolox/models/build.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     6647 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/yolox/models/darknet.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     2305 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/yolox/models/losses.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     6720 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/yolox/models/network_blocks.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     3104 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/yolox/models/yolo_fpn.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    25526 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/yolox/models/yolo_head.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     4158 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/yolox/models/yolo_pafpn.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1992 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/yolox/models/yolox.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:57:19.759837 onvif-gui-1.0.3/onvif_gui/yolox/tracker/
--rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-04-20 14:24:51.000000 onvif-gui-1.0.3/onvif_gui/yolox/tracker/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)      951 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/yolox/tracker/basetrack.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    12172 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/yolox/tracker/byte_tracker.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     9547 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/yolox/tracker/kalman_filter.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     6158 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/yolox/tracker/matching.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:57:19.759837 onvif-gui-1.0.3/onvif_gui/yolox/utils/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      126 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/yolox/utils/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1580 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/yolox/utils/utils.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:57:19.723837 onvif-gui-1.0.3/onvif_gui.egg-info/
--rw-r--r--   0 stephen   (1000) stephen   (1000)     8710 2023-04-23 02:57:19.000000 onvif-gui-1.0.3/onvif_gui.egg-info/PKG-INFO
--rw-r--r--   0 stephen   (1000) stephen   (1000)     9466 2023-04-23 02:57:19.000000 onvif-gui-1.0.3/onvif_gui.egg-info/SOURCES.txt
--rw-r--r--   0 stephen   (1000) stephen   (1000)        1 2023-04-23 02:57:19.000000 onvif-gui-1.0.3/onvif_gui.egg-info/dependency_links.txt
--rw-r--r--   0 stephen   (1000) stephen   (1000)       45 2023-04-23 02:57:19.000000 onvif-gui-1.0.3/onvif_gui.egg-info/entry_points.txt
--rw-r--r--   0 stephen   (1000) stephen   (1000)       47 2023-04-23 02:57:19.000000 onvif-gui-1.0.3/onvif_gui.egg-info/requires.txt
--rw-r--r--   0 stephen   (1000) stephen   (1000)       10 2023-04-23 02:57:19.000000 onvif-gui-1.0.3/onvif_gui.egg-info/top_level.txt
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1523 2023-04-23 02:56:42.000000 onvif-gui-1.0.3/pyproject.toml
--rw-r--r--   0 stephen   (1000) stephen   (1000)       38 2023-04-23 02:57:19.759837 onvif-gui-1.0.3/setup.cfg
--rw-r--r--   0 stephen   (1000) stephen   (1000)      740 2023-04-23 02:56:51.000000 onvif-gui-1.0.3/setup.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-25 16:18:44.159205 onvif-gui-1.0.4/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    11357 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/LICENSE
+-rw-r--r--   0 stephen   (1000) stephen   (1000)       59 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/MANIFEST.in
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     8849 2023-04-25 16:18:44.159205 onvif-gui-1.0.4/PKG-INFO
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     8170 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/README.md
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-25 16:18:44.135205 onvif-gui-1.0.4/detectron2/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)       67 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/__init__.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-25 16:18:44.135205 onvif-gui-1.0.4/detectron2/checkpoint/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      347 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/checkpoint/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    17770 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/checkpoint/c2_model_loading.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     5685 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/checkpoint/catalog.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     5258 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/checkpoint/detection_checkpoint.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-25 16:18:44.135205 onvif-gui-1.0.4/detectron2/config/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      599 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/config/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     7890 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/config/compat.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     9211 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/config/config.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    29512 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/config/defaults.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     3015 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/config/instantiate.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    15378 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/config/lazy.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-25 16:18:44.135205 onvif-gui-1.0.4/detectron2/configs/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/configs/__init__.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-25 16:18:44.135205 onvif-gui-1.0.4/detectron2/data/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      644 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/data/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     7378 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/data/benchmark.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    21231 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/data/build.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     7224 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/data/catalog.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     9162 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/data/common.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     8169 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/data/dataset_mapper.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-25 16:18:44.139205 onvif-gui-1.0.4/detectron2/data/datasets/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      523 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/data/datasets/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    10174 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/data/datasets/builtin.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    21841 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/data/datasets/builtin_meta.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    13167 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/data/datasets/cityscapes.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     7821 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/data/datasets/cityscapes_panoptic.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    23465 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/data/datasets/coco.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     8977 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/data/datasets/coco_panoptic.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     9623 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/data/datasets/lvis.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)   223757 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/data/datasets/lvis_v0_5_categories.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)   219177 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/data/datasets/lvis_v1_categories.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    39414 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/data/datasets/lvis_v1_category_image_count.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     3128 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/data/datasets/pascal_voc.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      169 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/data/datasets/register_coco.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    22841 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/data/detection_utils.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-25 16:18:44.139205 onvif-gui-1.0.4/detectron2/data/samplers/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      412 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/data/samplers/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    11789 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/data/samplers/distributed_sampler.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1944 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/data/samplers/grouped_batch_sampler.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-25 16:18:44.139205 onvif-gui-1.0.4/detectron2/data/transforms/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      466 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/data/transforms/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    14112 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/data/transforms/augmentation.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    23069 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/data/transforms/augmentation_impl.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    12629 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/data/transforms/transform.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-25 16:18:44.139205 onvif-gui-1.0.4/detectron2/layers/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      874 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/layers/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     5764 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/layers/aspp.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    12131 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/layers/batch_norm.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     3024 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/layers/blocks.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    16978 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/layers/deform_conv.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     4202 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/layers/losses.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    10879 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/layers/mask_ops.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     6490 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/layers/nms.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     3098 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/layers/roi_align.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     3302 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/layers/roi_align_rotated.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      652 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/layers/rotated_boxes.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      537 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/layers/shape_spec.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     5123 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/layers/wrappers.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-25 16:18:44.139205 onvif-gui-1.0.4/detectron2/modeling/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1568 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/modeling/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    15439 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/modeling/anchor_generator.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-25 16:18:44.143205 onvif-gui-1.0.4/detectron2/modeling/backbone/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      598 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/modeling/backbone/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     2512 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/modeling/backbone/backbone.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1015 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/modeling/backbone/build.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    10360 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/modeling/backbone/fpn.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    15988 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/modeling/backbone/mvit.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    16656 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/modeling/backbone/regnet.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    23658 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/modeling/backbone/resnet.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    25095 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/modeling/backbone/swin.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     6360 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/modeling/backbone/utils.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    19338 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/modeling/backbone/vit.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    15123 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/modeling/box_regression.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     6264 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/modeling/matcher.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-25 16:18:44.143205 onvif-gui-1.0.4/detectron2/modeling/meta_arch/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      508 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/modeling/meta_arch/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      814 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/modeling/meta_arch/build.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    11651 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/modeling/meta_arch/dense_detector.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    13213 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/modeling/meta_arch/fcos.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    10407 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/modeling/meta_arch/panoptic_fpn.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    13896 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/modeling/meta_arch/rcnn.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    18265 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/modeling/meta_arch/retinanet.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     9906 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/modeling/meta_arch/semantic_seg.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    10832 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/modeling/mmdet_wrapper.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    11316 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/modeling/poolers.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     4045 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/modeling/postprocessing.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-25 16:18:44.143205 onvif-gui-1.0.4/detectron2/modeling/proposal_generator/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      231 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/modeling/proposal_generator/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      836 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/modeling/proposal_generator/build.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     8128 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/modeling/proposal_generator/proposal_utils.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    23814 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/modeling/proposal_generator/rpn.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     8807 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/modeling/proposal_generator/rrpn.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-25 16:18:44.147205 onvif-gui-1.0.4/detectron2/modeling/roi_heads/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      768 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/modeling/roi_heads/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     4077 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/modeling/roi_heads/box_head.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    12990 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/modeling/roi_heads/cascade_rcnn.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    25390 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/modeling/roi_heads/fast_rcnn.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    11156 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/modeling/roi_heads/keypoint_head.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    12169 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/modeling/roi_heads/mask_head.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    37701 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/modeling/roi_heads/roi_heads.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    11175 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/modeling/roi_heads/rotated_fast_rcnn.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     2334 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/modeling/sampling.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    12416 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/modeling/test_time_augmentation.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1780 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/predictor.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-25 16:18:44.147205 onvif-gui-1.0.4/detectron2/structures/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      645 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/structures/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    14429 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/structures/boxes.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     5520 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/structures/image_list.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     6613 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/structures/instances.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     9030 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/structures/keypoints.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    19802 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/structures/masks.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    18853 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/structures/rotated_boxes.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     2707 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/tracker.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-25 16:18:44.147205 onvif-gui-1.0.4/detectron2/utils/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)       51 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/utils/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     6017 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/utils/analysis.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     8391 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/utils/collect_env.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     4096 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/utils/colormap.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     5608 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/utils/comm.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1852 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/utils/develop.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     5644 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/utils/env.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    17022 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/utils/events.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1189 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/utils/file_io.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     7807 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/utils/logger.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     2583 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/utils/memory.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1874 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/utils/registry.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1064 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/utils/serialize.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    18113 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/utils/testing.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    11319 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/utils/video_visualizer.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    51159 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/detectron2/utils/visualizer.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-25 16:18:44.147205 onvif-gui-1.0.4/gui/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)       28 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/gui/__init__.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-25 16:18:44.151205 onvif-gui-1.0.4/gui/components/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      245 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/gui/components/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1738 2023-04-25 14:47:13.000000 onvif-gui-1.0.4/gui/components/comboselector.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     2397 2023-04-25 14:47:26.000000 onvif-gui-1.0.4/gui/components/directoryselector.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     2118 2023-04-25 14:47:40.000000 onvif-gui-1.0.4/gui/components/fileselector.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     5315 2023-04-25 14:47:52.000000 onvif-gui-1.0.4/gui/components/labelselector.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     4077 2023-04-25 14:48:14.000000 onvif-gui-1.0.4/gui/components/progress.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1918 2023-04-25 14:49:36.000000 onvif-gui-1.0.4/gui/components/thresholdslider.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1996 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/gui/glwidget.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    12084 2023-04-25 16:12:20.000000 onvif-gui-1.0.4/gui/main.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-25 16:18:44.151205 onvif-gui-1.0.4/gui/onvif/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      191 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/gui/onvif/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     5743 2023-04-25 14:50:44.000000 onvif-gui-1.0.4/gui/onvif/admintab.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     3959 2023-04-25 14:51:01.000000 onvif-gui-1.0.4/gui/onvif/imagetab.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     2425 2023-04-25 14:51:17.000000 onvif-gui-1.0.4/gui/onvif/logindialog.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     5247 2023-04-25 14:51:28.000000 onvif-gui-1.0.4/gui/onvif/networktab.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     5118 2023-04-25 14:51:38.000000 onvif-gui-1.0.4/gui/onvif/ptztab.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     4527 2023-04-25 14:51:47.000000 onvif-gui-1.0.4/gui/onvif/videotab.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-25 16:18:44.151205 onvif-gui-1.0.4/gui/panels/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      147 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/gui/panels/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    13463 2023-04-25 14:52:02.000000 onvif-gui-1.0.4/gui/panels/camerapanel.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    14445 2023-04-25 14:52:14.000000 onvif-gui-1.0.4/gui/panels/filepanel.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     3538 2023-04-25 14:52:21.000000 onvif-gui-1.0.4/gui/panels/modulepanel.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    12043 2023-04-25 14:52:31.000000 onvif-gui-1.0.4/gui/panels/settingspanel.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-25 16:18:44.155205 onvif-gui-1.0.4/gui/resources/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1936 2023-04-25 15:08:17.000000 onvif-gui-1.0.4/gui/resources/LICENSE
+-rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/gui/resources/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      252 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/gui/resources/apply.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      245 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/gui/resources/apply_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      244 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/gui/resources/apply_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      911 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/gui/resources/audio.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      536 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/gui/resources/audio_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      920 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/gui/resources/audio_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      203 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/gui/resources/branch_closed.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      219 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/gui/resources/branch_closed_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      211 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/gui/resources/branch_closed_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      199 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/gui/resources/branch_open.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      168 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/gui/resources/branch_open_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      172 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/gui/resources/branch_open_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      267 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/gui/resources/checked.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      235 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/gui/resources/checked_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      246 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/gui/resources/checked_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    12716 2023-04-25 14:59:19.000000 onvif-gui-1.0.4/gui/resources/darkstyle.qss
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      910 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/gui/resources/discover.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      849 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/gui/resources/discover_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      937 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/gui/resources/discover_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      425 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/gui/resources/fast-forward.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      253 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/gui/resources/fast-forward_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      433 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/gui/resources/fast-forward_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      641 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/gui/resources/mute.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      346 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/gui/resources/mute_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      618 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/gui/resources/mute_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      347 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/gui/resources/next.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      225 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/gui/resources/next_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      348 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/gui/resources/next_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    46084 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/gui/resources/onvif-gui.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      172 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/gui/resources/pause.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      144 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/gui/resources/pause_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      149 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/gui/resources/pause_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      321 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/gui/resources/play.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      209 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/gui/resources/play_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      316 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/gui/resources/play_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      349 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/gui/resources/previous.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      232 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/gui/resources/previous_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      348 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/gui/resources/previous_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      324 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/gui/resources/radio-off.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      250 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/gui/resources/radio-off_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      324 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/gui/resources/radio-off_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      350 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/gui/resources/radio-on.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      263 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/gui/resources/radio-on_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      343 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/gui/resources/radio-on_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      395 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/gui/resources/record.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      394 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/gui/resources/record_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      425 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/gui/resources/record_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      408 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/gui/resources/recording.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      435 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/gui/resources/recording_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      532 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/gui/resources/recording_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      454 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/gui/resources/rewind.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      250 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/gui/resources/rewind_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      457 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/gui/resources/rewind_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      187 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/gui/resources/small_arrow_left.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      183 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/gui/resources/small_arrow_left_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      189 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/gui/resources/small_arrow_left_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      162 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/gui/resources/small_arrow_up.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      160 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/gui/resources/small_arrow_up_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      161 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/gui/resources/small_arrow_up_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      158 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/gui/resources/stop.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      140 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/gui/resources/stop_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      151 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/gui/resources/stop_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      143 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/gui/resources/unchecked.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      142 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/gui/resources/unchecked_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      143 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/gui/resources/unchecked_lo.png
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-25 16:18:44.159205 onvif-gui-1.0.4/modules/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/modules/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     6508 2023-04-25 03:15:34.000000 onvif-gui-1.0.4/modules/keypoint.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     4780 2023-04-25 02:02:02.000000 onvif-gui-1.0.4/modules/retinanet.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     3000 2023-04-25 14:46:07.000000 onvif-gui-1.0.4/modules/sample.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     7096 2023-04-25 02:45:28.000000 onvif-gui-1.0.4/modules/segment.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    11735 2023-04-25 14:46:22.000000 onvif-gui-1.0.4/modules/yolox.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-25 16:18:44.159205 onvif-gui-1.0.4/onvif_gui.egg-info/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     8849 2023-04-25 16:18:44.000000 onvif-gui-1.0.4/onvif_gui.egg-info/PKG-INFO
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     7506 2023-04-25 16:18:44.000000 onvif-gui-1.0.4/onvif_gui.egg-info/SOURCES.txt
+-rw-r--r--   0 stephen   (1000) stephen   (1000)        1 2023-04-25 16:18:44.000000 onvif-gui-1.0.4/onvif_gui.egg-info/dependency_links.txt
+-rw-r--r--   0 stephen   (1000) stephen   (1000)       39 2023-04-25 16:18:44.000000 onvif-gui-1.0.4/onvif_gui.egg-info/entry_points.txt
+-rw-r--r--   0 stephen   (1000) stephen   (1000)       47 2023-04-25 16:18:44.000000 onvif-gui-1.0.4/onvif_gui.egg-info/requires.txt
+-rw-r--r--   0 stephen   (1000) stephen   (1000)       29 2023-04-25 16:18:44.000000 onvif-gui-1.0.4/onvif_gui.egg-info/top_level.txt
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1659 2023-04-25 16:01:52.000000 onvif-gui-1.0.4/pyproject.toml
+-rw-r--r--   0 stephen   (1000) stephen   (1000)       38 2023-04-25 16:18:44.159205 onvif-gui-1.0.4/setup.cfg
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1504 2023-04-25 16:01:42.000000 onvif-gui-1.0.4/setup.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-25 16:18:44.159205 onvif-gui-1.0.4/yolox/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/yolox/__init__.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-25 16:18:44.159205 onvif-gui-1.0.4/yolox/models/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      936 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/yolox/models/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     4894 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/yolox/models/build.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     6647 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/yolox/models/darknet.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     2305 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/yolox/models/losses.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     6720 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/yolox/models/network_blocks.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     3104 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/yolox/models/yolo_fpn.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    25526 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/yolox/models/yolo_head.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     4158 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/yolox/models/yolo_pafpn.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1992 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/yolox/models/yolox.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-25 16:18:44.159205 onvif-gui-1.0.4/yolox/tracker/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/yolox/tracker/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      951 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/yolox/tracker/basetrack.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    12172 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/yolox/tracker/byte_tracker.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     9547 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/yolox/tracker/kalman_filter.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     6158 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/yolox/tracker/matching.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-25 16:18:44.159205 onvif-gui-1.0.4/yolox/utils/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      126 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/yolox/utils/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1580 2023-04-24 20:43:33.000000 onvif-gui-1.0.4/yolox/utils/utils.py
```

### Comparing `onvif-gui-1.0.3/LICENSE` & `onvif-gui-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/PKG-INFO` & `onvif-gui-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: onvif-gui
-Version: 1.0.3
+Version: 1.0.4
 Summary: A client gui for Onvif
 Author: Stephen Rhodes
 Author-email: Stephen Rhodes <sr99622@gmail.com>
+Project-URL: Homepage, https://github.com/sr99622/libonvif
+Project-URL: Bug Reports, https://github.com/sr99622/libonvif/issues
 Keywords: sample,setuptools,development
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # onvif-gui
 
@@ -47,21 +49,21 @@
 ```
 pip install onvif-gui
 ```
 
 Modules
 -----------------
 
-onvif_gui has a facility for incorporating python programs to operate on the
+onvif-gui has a facility for incorporating python programs to operate on the
 video stream.  The Modules tab is the user interface for this feature.  There
 is a minimal example program called sample.py that demonstrates how data is 
 trsansferred from the main program to the python module and it's GUI interface
 implementation.
 
-There is included with onvif_gui a full implementation of the YOLOX algorithm
+There is included with onvif-gui a full implementation of the YOLOX algorithm
 along with an associated tracking algorithm known as ByteTrack.  These algorithms 
 are implemented using pytorch, which requires some specific configuration. Note
 that ByteTrack currently is available only on Windows.
 
 Note on Running PyTorch Modules
 --------------------------------
 
@@ -77,29 +79,29 @@
 
 
 Onvif GUI Program
 -----------------
 
 NAME 
 
-    onvif_gui
+    onvif-gui
 
 SYNOPSIS
 
-    onvif_gui is a python program.  
+    onvif-gui is a python program.  
     
     The program requires the following modules:
 
     pip install pyqt6 opencv-python numpy loguru
     
 
     To run the program:
 
-    cd ../onvif_gui
-    python3 main.py
+    cd ../onvif-gui
+    python3 run.py
 
     These instructions are intended for quick setup to verify the program.  To use the 
     library in other python programs, it is advised to install the onvif and avio
     python modules.
 
     cd ../libonvif
     python3 setup.py install
```

### Comparing `onvif-gui-1.0.3/README.md` & `onvif-gui-1.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -31,21 +31,21 @@
 ```
 pip install onvif-gui
 ```
 
 Modules
 -----------------
 
-onvif_gui has a facility for incorporating python programs to operate on the
+onvif-gui has a facility for incorporating python programs to operate on the
 video stream.  The Modules tab is the user interface for this feature.  There
 is a minimal example program called sample.py that demonstrates how data is 
 trsansferred from the main program to the python module and it's GUI interface
 implementation.
 
-There is included with onvif_gui a full implementation of the YOLOX algorithm
+There is included with onvif-gui a full implementation of the YOLOX algorithm
 along with an associated tracking algorithm known as ByteTrack.  These algorithms 
 are implemented using pytorch, which requires some specific configuration. Note
 that ByteTrack currently is available only on Windows.
 
 Note on Running PyTorch Modules
 --------------------------------
 
@@ -61,29 +61,29 @@
 
 
 Onvif GUI Program
 -----------------
 
 NAME 
 
-    onvif_gui
+    onvif-gui
 
 SYNOPSIS
 
-    onvif_gui is a python program.  
+    onvif-gui is a python program.  
     
     The program requires the following modules:
 
     pip install pyqt6 opencv-python numpy loguru
     
 
     To run the program:
 
-    cd ../onvif_gui
-    python3 main.py
+    cd ../onvif-gui
+    python3 run.py
 
     These instructions are intended for quick setup to verify the program.  To use the 
     library in other python programs, it is advised to install the onvif and avio
     python modules.
 
     cd ../libonvif
     python3 setup.py install
```

### Comparing `onvif-gui-1.0.3/onvif_gui/components/comboselector.py` & `onvif-gui-1.0.4/gui/components/comboselector.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #*******************************************************************************
-# libonvif/onvif_gui/components/comboselector.py
+# onvif-gui/gui/components/comboselector.py
 #
 # Copyright (c) 2023 Stephen Rhodes 
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `onvif-gui-1.0.3/onvif_gui/components/fileselector.py` & `onvif-gui-1.0.4/gui/components/fileselector.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #*******************************************************************************
-# libonvif/onvif_gui/components/fileselector.py
+# onvif-gui/gui/components/fileselector.py
 #
 # Copyright (c) 2023 Stephen Rhodes 
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -27,28 +27,26 @@
         self.filenameKey = "Module/" + name + "/filename"
 
         self.txtFilename = QLineEdit()
         self.txtFilename.setText(self.mw.settings.value(self.filenameKey))
         self.txtFilename.textEdited.connect(self.txtFilenameChanged)
         self.btnSelect = QPushButton("...")
         self.btnSelect.clicked.connect(self.btnSelectClicked)
-        self.btnSelect.setMaximumWidth(36)
         lblSelect = QLabel("Model")
 
         lytMain = QGridLayout(self)
         lytMain.addWidget(lblSelect,          0, 0, 1, 1)
         lytMain.addWidget(self.txtFilename,   0, 1, 1, 1)
         lytMain.addWidget(self.btnSelect,     0, 2, 1, 1)
+        lytMain.setColumnStretch(1, 10)
         lytMain.setContentsMargins(0, 0, 0, 0)
 
     def btnSelectClicked(self):
-        print("btnSelctClicked")
-        filename = QFileDialog.getOpenFileName(self, "Select Model File", 
-                                               self.txtFilename.text())[0]
-        print(filename)
+        filename = QFileDialog.getOpenFileName(self, "Select File", self.txtFilename.text())[0]
+
         if len(filename) > 0:
             self.txtFilename.setText(filename)
             self.mw.settings.setValue(self.filenameKey, filename)
 
     def txtFilenameChanged(self, text):
         self.mw.settings.setValue(self.filenameKey, text)
```

### Comparing `onvif-gui-1.0.3/onvif_gui/components/labelselector.py` & `onvif-gui-1.0.4/gui/components/labelselector.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #*******************************************************************************
-# libonvif/onvif_gui/components/labelselector.py
+# onvif-gui/gui/components/labelselector.py
 #
 # Copyright (c) 2023 Stephen Rhodes 
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `onvif-gui-1.0.3/onvif_gui/components/progress.py` & `onvif-gui-1.0.4/gui/components/progress.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #********************************************************************
-# libavio/samples/pyqt/progress.py
+# onvif-gui/gui/components/progress.py
 #
 # Copyright (c) 2023  Stephen Rhodes
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/checkpoint/c2_model_loading.py` & `onvif-gui-1.0.4/detectron2/checkpoint/c2_model_loading.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/checkpoint/catalog.py` & `onvif-gui-1.0.4/detectron2/checkpoint/catalog.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/checkpoint/detection_checkpoint.py` & `onvif-gui-1.0.4/detectron2/checkpoint/detection_checkpoint.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/config/__init__.py` & `onvif-gui-1.0.4/detectron2/config/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/config/compat.py` & `onvif-gui-1.0.4/detectron2/config/compat.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/config/config.py` & `onvif-gui-1.0.4/detectron2/config/config.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/config/defaults.py` & `onvif-gui-1.0.4/detectron2/config/defaults.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/config/instantiate.py` & `onvif-gui-1.0.4/detectron2/config/instantiate.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/config/lazy.py` & `onvif-gui-1.0.4/detectron2/config/lazy.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/data/__init__.py` & `onvif-gui-1.0.4/detectron2/data/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/data/benchmark.py` & `onvif-gui-1.0.4/detectron2/data/benchmark.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/data/build.py` & `onvif-gui-1.0.4/detectron2/data/build.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/data/catalog.py` & `onvif-gui-1.0.4/detectron2/data/catalog.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/data/common.py` & `onvif-gui-1.0.4/detectron2/data/common.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/data/dataset_mapper.py` & `onvif-gui-1.0.4/detectron2/data/dataset_mapper.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/data/datasets/__init__.py` & `onvif-gui-1.0.4/detectron2/data/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/data/datasets/builtin.py` & `onvif-gui-1.0.4/detectron2/data/datasets/builtin.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/data/datasets/builtin_meta.py` & `onvif-gui-1.0.4/detectron2/data/datasets/builtin_meta.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/data/datasets/cityscapes.py` & `onvif-gui-1.0.4/detectron2/data/datasets/cityscapes.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/data/datasets/cityscapes_panoptic.py` & `onvif-gui-1.0.4/detectron2/data/datasets/cityscapes_panoptic.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/data/datasets/coco.py` & `onvif-gui-1.0.4/detectron2/data/datasets/coco.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/data/datasets/coco_panoptic.py` & `onvif-gui-1.0.4/detectron2/data/datasets/coco_panoptic.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/data/datasets/lvis.py` & `onvif-gui-1.0.4/detectron2/data/datasets/lvis.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/data/datasets/lvis_v0_5_categories.py` & `onvif-gui-1.0.4/detectron2/data/datasets/lvis_v0_5_categories.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/data/datasets/lvis_v1_categories.py` & `onvif-gui-1.0.4/detectron2/data/datasets/lvis_v1_categories.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/data/datasets/lvis_v1_category_image_count.py` & `onvif-gui-1.0.4/detectron2/data/datasets/lvis_v1_category_image_count.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/data/datasets/pascal_voc.py` & `onvif-gui-1.0.4/detectron2/data/datasets/pascal_voc.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/data/detection_utils.py` & `onvif-gui-1.0.4/detectron2/data/detection_utils.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/data/samplers/distributed_sampler.py` & `onvif-gui-1.0.4/detectron2/data/samplers/distributed_sampler.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/data/samplers/grouped_batch_sampler.py` & `onvif-gui-1.0.4/detectron2/data/samplers/grouped_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/data/transforms/augmentation.py` & `onvif-gui-1.0.4/detectron2/data/transforms/augmentation.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/data/transforms/augmentation_impl.py` & `onvif-gui-1.0.4/detectron2/data/transforms/augmentation_impl.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/data/transforms/transform.py` & `onvif-gui-1.0.4/detectron2/data/transforms/transform.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/layers/__init__.py` & `onvif-gui-1.0.4/detectron2/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/layers/aspp.py` & `onvif-gui-1.0.4/detectron2/layers/aspp.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/layers/batch_norm.py` & `onvif-gui-1.0.4/detectron2/layers/batch_norm.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/layers/blocks.py` & `onvif-gui-1.0.4/detectron2/layers/blocks.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/layers/deform_conv.py` & `onvif-gui-1.0.4/detectron2/layers/deform_conv.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/layers/losses.py` & `onvif-gui-1.0.4/detectron2/layers/losses.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/layers/mask_ops.py` & `onvif-gui-1.0.4/detectron2/layers/mask_ops.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/layers/nms.py` & `onvif-gui-1.0.4/detectron2/layers/nms.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/layers/roi_align.py` & `onvif-gui-1.0.4/detectron2/layers/roi_align.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/layers/roi_align_rotated.py` & `onvif-gui-1.0.4/detectron2/layers/roi_align_rotated.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/layers/rotated_boxes.py` & `onvif-gui-1.0.4/detectron2/layers/rotated_boxes.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/layers/shape_spec.py` & `onvif-gui-1.0.4/detectron2/layers/shape_spec.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/layers/wrappers.py` & `onvif-gui-1.0.4/detectron2/layers/wrappers.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/modeling/__init__.py` & `onvif-gui-1.0.4/detectron2/modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/modeling/anchor_generator.py` & `onvif-gui-1.0.4/detectron2/modeling/anchor_generator.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/modeling/backbone/__init__.py` & `onvif-gui-1.0.4/detectron2/modeling/backbone/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/modeling/backbone/backbone.py` & `onvif-gui-1.0.4/detectron2/modeling/backbone/backbone.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/modeling/backbone/build.py` & `onvif-gui-1.0.4/detectron2/modeling/backbone/build.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/modeling/backbone/fpn.py` & `onvif-gui-1.0.4/detectron2/modeling/backbone/fpn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/modeling/backbone/mvit.py` & `onvif-gui-1.0.4/detectron2/modeling/backbone/mvit.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/modeling/backbone/regnet.py` & `onvif-gui-1.0.4/detectron2/modeling/backbone/regnet.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/modeling/backbone/resnet.py` & `onvif-gui-1.0.4/detectron2/modeling/backbone/resnet.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/modeling/backbone/swin.py` & `onvif-gui-1.0.4/detectron2/modeling/backbone/swin.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/modeling/backbone/utils.py` & `onvif-gui-1.0.4/detectron2/modeling/backbone/utils.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/modeling/backbone/vit.py` & `onvif-gui-1.0.4/detectron2/modeling/backbone/vit.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/modeling/box_regression.py` & `onvif-gui-1.0.4/detectron2/modeling/box_regression.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/modeling/matcher.py` & `onvif-gui-1.0.4/detectron2/modeling/matcher.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/modeling/meta_arch/build.py` & `onvif-gui-1.0.4/detectron2/modeling/meta_arch/build.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/modeling/meta_arch/dense_detector.py` & `onvif-gui-1.0.4/detectron2/modeling/meta_arch/dense_detector.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/modeling/meta_arch/fcos.py` & `onvif-gui-1.0.4/detectron2/modeling/meta_arch/fcos.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/modeling/meta_arch/panoptic_fpn.py` & `onvif-gui-1.0.4/detectron2/modeling/meta_arch/panoptic_fpn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/modeling/meta_arch/rcnn.py` & `onvif-gui-1.0.4/detectron2/modeling/meta_arch/rcnn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/modeling/meta_arch/retinanet.py` & `onvif-gui-1.0.4/detectron2/modeling/meta_arch/retinanet.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/modeling/meta_arch/semantic_seg.py` & `onvif-gui-1.0.4/detectron2/modeling/meta_arch/semantic_seg.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/modeling/mmdet_wrapper.py` & `onvif-gui-1.0.4/detectron2/modeling/mmdet_wrapper.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/modeling/poolers.py` & `onvif-gui-1.0.4/detectron2/modeling/poolers.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/modeling/postprocessing.py` & `onvif-gui-1.0.4/detectron2/modeling/postprocessing.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/modeling/proposal_generator/build.py` & `onvif-gui-1.0.4/detectron2/modeling/proposal_generator/build.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/modeling/proposal_generator/proposal_utils.py` & `onvif-gui-1.0.4/detectron2/modeling/proposal_generator/proposal_utils.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/modeling/proposal_generator/rpn.py` & `onvif-gui-1.0.4/detectron2/modeling/proposal_generator/rpn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/modeling/proposal_generator/rrpn.py` & `onvif-gui-1.0.4/detectron2/modeling/proposal_generator/rrpn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/modeling/roi_heads/__init__.py` & `onvif-gui-1.0.4/detectron2/modeling/roi_heads/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/modeling/roi_heads/box_head.py` & `onvif-gui-1.0.4/detectron2/modeling/roi_heads/box_head.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/modeling/roi_heads/cascade_rcnn.py` & `onvif-gui-1.0.4/detectron2/modeling/roi_heads/cascade_rcnn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/modeling/roi_heads/fast_rcnn.py` & `onvif-gui-1.0.4/detectron2/modeling/roi_heads/fast_rcnn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/modeling/roi_heads/keypoint_head.py` & `onvif-gui-1.0.4/detectron2/modeling/roi_heads/keypoint_head.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/modeling/roi_heads/mask_head.py` & `onvif-gui-1.0.4/detectron2/modeling/roi_heads/mask_head.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/modeling/roi_heads/roi_heads.py` & `onvif-gui-1.0.4/detectron2/modeling/roi_heads/roi_heads.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/modeling/roi_heads/rotated_fast_rcnn.py` & `onvif-gui-1.0.4/detectron2/modeling/roi_heads/rotated_fast_rcnn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/modeling/sampling.py` & `onvif-gui-1.0.4/detectron2/modeling/sampling.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/modeling/test_time_augmentation.py` & `onvif-gui-1.0.4/detectron2/modeling/test_time_augmentation.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/predictor.py` & `onvif-gui-1.0.4/detectron2/predictor.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/structures/__init__.py` & `onvif-gui-1.0.4/detectron2/structures/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/structures/boxes.py` & `onvif-gui-1.0.4/detectron2/structures/boxes.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/structures/image_list.py` & `onvif-gui-1.0.4/detectron2/structures/image_list.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/structures/instances.py` & `onvif-gui-1.0.4/detectron2/structures/instances.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/structures/keypoints.py` & `onvif-gui-1.0.4/detectron2/structures/keypoints.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/structures/masks.py` & `onvif-gui-1.0.4/detectron2/structures/masks.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/structures/rotated_boxes.py` & `onvif-gui-1.0.4/detectron2/structures/rotated_boxes.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/tracker.py` & `onvif-gui-1.0.4/detectron2/tracker.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/utils/analysis.py` & `onvif-gui-1.0.4/detectron2/utils/analysis.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/utils/collect_env.py` & `onvif-gui-1.0.4/detectron2/utils/collect_env.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/utils/colormap.py` & `onvif-gui-1.0.4/detectron2/utils/colormap.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/utils/comm.py` & `onvif-gui-1.0.4/detectron2/utils/comm.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/utils/develop.py` & `onvif-gui-1.0.4/detectron2/utils/develop.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/utils/env.py` & `onvif-gui-1.0.4/detectron2/utils/env.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/utils/events.py` & `onvif-gui-1.0.4/detectron2/utils/events.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/utils/file_io.py` & `onvif-gui-1.0.4/detectron2/utils/file_io.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/utils/logger.py` & `onvif-gui-1.0.4/detectron2/utils/logger.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/utils/memory.py` & `onvif-gui-1.0.4/detectron2/utils/memory.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/utils/registry.py` & `onvif-gui-1.0.4/detectron2/utils/registry.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/utils/serialize.py` & `onvif-gui-1.0.4/detectron2/utils/serialize.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/utils/testing.py` & `onvif-gui-1.0.4/detectron2/utils/testing.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/utils/video_visualizer.py` & `onvif-gui-1.0.4/detectron2/utils/video_visualizer.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/detectron2/utils/visualizer.py` & `onvif-gui-1.0.4/detectron2/utils/visualizer.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/glwidget.py` & `onvif-gui-1.0.4/gui/glwidget.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/main.py` & `onvif-gui-1.0.4/gui/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,20 +17,21 @@
 #
 #*********************************************************************/
 
 import os
 import sys
 import time
 import importlib.util
+from pathlib import Path
 from PyQt6.QtWidgets import QApplication, QMainWindow, QLabel, QSplitter, \
 QTabWidget, QMessageBox
 from PyQt6.QtCore import pyqtSignal, QObject, QSettings, QDir, QSize, QByteArray
 from PyQt6.QtGui import QIcon
-from onvif_gui.panels import CameraPanel, FilePanel, SettingsPanel, ModulePanel
-from onvif_gui.glwidget import GLWidget
+from gui.panels import CameraPanel, FilePanel, SettingsPanel, ModulePanel
+from gui.glwidget import GLWidget
 from loguru import logger
 
 sys.path.append("../build/libavio")
 sys.path.append("../build/libavio/Release")
 import avio
 
 FORCE_DIRECT_RENDER = False
@@ -48,19 +49,19 @@
     def sizeHint(self):
         return QSize(640, 480)
 
 class MainWindow(QMainWindow):
     def __init__(self, clear_settings=False):
         super().__init__()
         os.environ["QT_FILESYSTEMMODEL_WATCH_FILES"] = "ON"
-        QDir.addSearchPath("image", self.getLocation() + "/resources/")
+        QDir.addSearchPath("image", self.getLocation() + "/gui/resources/")
         self.style()
-        self.program_name = "onvif gui version 2.0.0"
+        self.program_name = "onvif gui version 1.0.4"
         self.setWindowTitle(self.program_name)
-        self.setWindowIcon(QIcon('image:onvif_gui.png'))
+        self.setWindowIcon(QIcon('image:onvif-gui.png'))
         self.settings = QSettings("onvif", "gui")
         if clear_settings:
             self.settings.clear()
         self.volumeKey = "MainWindow/volume"
         self.muteKey = "MainWindow/mute"
         self.geometryKey = "MainWindow/geometry"
         self.tabIndexKey = "MainWindow/tabIndex"
@@ -128,23 +129,23 @@
             self.loadWorker(workerName)
             self.loadConfigure(workerName)
 
         if splitterState is not None:
             self.split.restoreState(splitterState)
 
     def loadConfigure(self, workerName):
-        spec = importlib.util.spec_from_file_location("Configure", self.getLocation() + "/modules/" + workerName)
+        spec = importlib.util.spec_from_file_location("Configure", self.modulePanel.dirModules.text() + "/" + workerName)
         hook = importlib.util.module_from_spec(spec)
         sys.modules["Configure"] = hook
         spec.loader.exec_module(hook)
         self.configure = hook.Configure(self)
         self.modulePanel.setPanel(self.configure)
 
     def loadWorker(self, workerName):
-        spec = importlib.util.spec_from_file_location("Worker", self.getLocation() + "/modules/" + workerName)
+        spec = importlib.util.spec_from_file_location("Worker", self.modulePanel.dirModules.text() + "/" + workerName)
         self.hook = importlib.util.module_from_spec(spec)
         sys.modules["Worker"] = self.hook
         spec.loader.exec_module(self.hook)
         self.worker = None
 
     def pythonCallback(self, F):
         if self.modulePanel.chkEngage.isChecked():
@@ -268,30 +269,32 @@
         self.filePanel.control.setBtnRecord()
         self.cameraPanel.setEnabled(True)
 
     def splitterMoved(self, pos, index):
         self.settings.setValue(self.splitKey, self.split.saveState())
 
     def getLocation(self):
-        return os.path.dirname(__file__)
+        path = Path(os.path.dirname(__file__))
+        return str(path.parent.absolute())
+        #return os.path.dirname(__file__)
 
     def style(self):
         #blDefault = "#566170"
         blDefault = "#5B5B5B"
         #bmDefault = "#3E4754"
         bmDefault = "#4B4B4B"
         #bdDefault = "#283445"
         bdDefault = "#3B3B3B"
         flDefault = "#C6D9F2"
         fmDefault = "#9DADC2"
         fdDefault = "#808D9E"
         slDefault = "#FFFFFF"
         smDefault = "#DDEEFF"
         sdDefault = "#306294"
-        strStyle = open(self.getLocation() + "/resources/darkstyle.qss", "r").read()
+        strStyle = open(self.getLocation() + "/gui/resources/darkstyle.qss", "r").read()
         strStyle = strStyle.replace("background_light",  blDefault)
         strStyle = strStyle.replace("background_medium", bmDefault)
         strStyle = strStyle.replace("background_dark",   bdDefault)
         strStyle = strStyle.replace("foreground_light",  flDefault)
         strStyle = strStyle.replace("foreground_medium", fmDefault)
         strStyle = strStyle.replace("foreground_dark",   fdDefault)
         strStyle = strStyle.replace("selection_light",   slDefault)
```

### Comparing `onvif-gui-1.0.3/onvif_gui/modules/keypoint.py` & `onvif-gui-1.0.4/modules/keypoint.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 # Copyright (c) Facebook, Inc. and its affiliates.
-import numpy as np
-import torch
-import cv2
-import math
-import os
-from loguru import logger
-from sys import platform
-from pathlib import Path
-from detectron2.config import get_cfg
-from detectron2.predictor import Predictor
-from detectron2.tracker import DetectedInstance, SimpleTracker
-from PyQt6.QtWidgets import QWidget, QGridLayout, QLabel
-from components import ThresholdSlider
 
-# constants
-CONFIDENCE_THRESHOLD = 0.50
+IMPORT_ERROR = ""
+try:
+    import numpy as np
+    import cv2
+    import math
+    import os
+    from loguru import logger
+    from sys import platform
+    from pathlib import Path
+    from PyQt6.QtWidgets import QWidget, QGridLayout, QLabel, QMessageBox
+    from gui.components import ThresholdSlider
+
+    import torch
+    from detectron2.config import get_cfg
+    from detectron2.predictor import Predictor
+    from detectron2.tracker import DetectedInstance, SimpleTracker
+except ModuleNotFoundError as ex:
+    IMPORT_ERROR = str(ex)
+    print("Import Error has occurred, missing modules need to be installed, please consult documentation: ", ex)
+
 MODULE_NAME = "detectron2/keypoint"
 
 class Configure(QWidget):
     def __init__(self, mw):
         try:
             super().__init__()
             self.mw = mw
@@ -30,27 +35,33 @@
             lytMain.setRowStretch(1, 10)
 
             self.mw.signals.started.connect(self.disableThresholdSlider)
             self.mw.signals.stopped.connect(self.enableThresholdSlider)
             if self.mw.playing:
                 self.sldThreshold.setEnabled(False)
 
+            if len(IMPORT_ERROR) > 0:
+                QMessageBox.critical(None, "Detectron2 Import Error", "Modules required for running this function are missing: " + IMPORT_ERROR)
+
         except:
             logger.exception("keypoints configuration load error")
 
     def disableThresholdSlider(self):
         self.sldThreshold.setEnabled(False)
 
     def enableThresholdSlider(self):
         self.sldThreshold.setEnabled(True)
 
 class Worker:
     def __init__(self, mw):
+        self.mw = mw
+        self.last_ex = ""
+        self.CONFIDENCE_THRESHOLD = self.mw.configure.sldThreshold.value()
+
         try:
-            self.mw = mw
             ckpt_file = "auto"
             fp16 = True
             self.no_back = True
             self.simple = True
 
             if ckpt_file is not None:
                 if ckpt_file.lower() == "auto":
@@ -60,19 +71,18 @@
 
                     if not cache.is_file():
                         cache.parent.mkdir(parents=True, exist_ok=True)
                         torch.hub.download_url_to_file("https://dl.fbaipublicfiles.com/detectron2/COCO-Keypoints/keypoint_rcnn_R_50_FPN_3x/137849621/model_final_a6e10b.pkl", ckpt_file)
 
             cfg = get_cfg()
             cfg.merge_from_file('./detectron2/configs/COCO-Keypoints/keypoint_rcnn_R_50_FPN_3x.yaml')
-            cfg.MODEL.RETINANET.SCORE_THRESH_TEST = CONFIDENCE_THRESHOLD
-            cfg.MODEL.ROI_HEADS.SCORE_THRESH_TEST = CONFIDENCE_THRESHOLD
-            #cfg.MODEL.WEIGHTS = './detectron2/models/COCO-Keypoints/model_final_a6e10b.pkl'
+            cfg.MODEL.RETINANET.SCORE_THRESH_TEST = self.CONFIDENCE_THRESHOLD
+            cfg.MODEL.ROI_HEADS.SCORE_THRESH_TEST = self.CONFIDENCE_THRESHOLD
             cfg.MODEL.WEIGHTS = ckpt_file
-            cfg.MODEL.PANOPTIC_FPN.COMBINE.INSTANCES_CONFIDENCE_THRESH = CONFIDENCE_THRESHOLD
+            cfg.MODEL.PANOPTIC_FPN.COMBINE.INSTANCES_CONFIDENCE_THRESH = self.CONFIDENCE_THRESHOLD
             cfg.freeze()
 
             self.tracker = SimpleTracker()
             self.predictor = Predictor(cfg, fp16)
         except:
             logger.exception("Keypoints initialization error")
 
@@ -99,16 +109,18 @@
 
             if len(detected):
                 colors = np.asarray(self.tracker.assign_colors(detected)) * 255
                 colors = colors.astype(np.int32)
                 for idx, keypoint in enumerate(keypoints):
                     self.draw_keypoint(img, keypoint, colors[idx])
 
-        except:
-            logger.exception("Keypoints runtime error")
+        except Exception as ex:
+            if self.last_ex != str(ex):
+                logger.exception("Keypoints runtime error")
+            self.last_ex = str(ex)
 
     def get_auto_ckpt_filename(self):
         filename = None
         if platform == "win32":
             filename = os.environ['HOMEPATH'] + "/.cache/torch/hub/checkpoints/model_final_a6e10b.pkl"
         else:
             filename = os.environ['HOME'] + "/.cache/torch/hub/checkpoints/model_final_a6e10b.pkl"
```

### Comparing `onvif-gui-1.0.3/onvif_gui/modules/retinanet.py` & `onvif-gui-1.0.4/modules/retinanet.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #/********************************************************************
-# libonvif/onvif_gui/modules/retinanet.py 
+#libonvif/gui/modules/retinanet.py 
 #
 # Copyright (c) 2023  Stephen Rhodes
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -13,28 +13,34 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 #*********************************************************************/
 
-import cv2
-import torchvision
-import torch
-import numpy as np
-from loguru import logger
-import torchvision.transforms as transforms
-from PyQt6.QtWidgets import QGridLayout, QWidget, QLabel
-from PyQt6.QtCore import Qt
-from components.thresholdslider import ThresholdSlider
-from components.labelselector import LabelSelector
-
-transform = transforms.Compose([
-    transforms.ToTensor(),
-])
+IMPORT_ERROR = ""
+try:
+    import cv2
+    import numpy as np
+    from loguru import logger
+    from PyQt6.QtWidgets import QGridLayout, QWidget, QLabel, QMessageBox
+    from PyQt6.QtCore import Qt
+    from gui.components.thresholdslider import ThresholdSlider
+    from gui.components.labelselector import LabelSelector
+
+    import torch
+    import torchvision
+    import torchvision.transforms as transforms
+
+    transform = transforms.Compose([
+        transforms.ToTensor(),
+    ])
+except ModuleNotFoundError as ex:
+    IMPORT_ERROR = str(ex)
+    print("Import Error has occurred, missing modules need to be installed, please consult documentation: ", ex)
 
 MODULE_NAME = "retinanet"
 
 class Configure(QWidget):
     def __init__(self, mw):
         try:
             super().__init__()
@@ -58,21 +64,26 @@
             lytLabels.setContentsMargins(0, 0, 0, 0)
 
             lytMain = QGridLayout(self)
             lytMain.addWidget(self.sldThreshold,        0, 0, 1, 1)
             lytMain.addWidget(pnlLabels,                1, 0, 1, 1)
             lytMain.addWidget(QLabel(""),               2, 0, 1, 1)
             lytMain.setRowStretch(2, 10)
+
+            if len(IMPORT_ERROR) > 0:
+                QMessageBox.critical(None, "Retinanet Import Error", "Modules required for running this function are missing: " + IMPORT_ERROR)
+
         except:
             logger.exception("retinanet configuration load error")
 
 class Worker:
     def __init__(self, mw):
+        self.mw = mw
+        self.last_ex = ""
         try:
-            self.mw = mw
             self.model = torchvision.models.detection.retinanet_resnet50_fpn(weights=torchvision.models.detection.RetinaNet_ResNet50_FPN_Weights.DEFAULT)            
             self.device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')
             self.model.eval().to(self.device)
         except:
             logger.exception("retinanet worker load error")
 
     def __call__(self, F):
@@ -102,10 +113,12 @@
                     g = lbl.color()[1]
                     b = lbl.color()[2]
                     lbl.setCount(lbl_boxes.shape[0])
 
                     for box in lbl_boxes:
                         cv2.rectangle(img, (box[0], box[1]), (box[2], box[3]), (r, g, b), 2)
 
-        except:
-            logger.exception("retinanet worker call error")
+        except Exception as ex:
+            if self.last_ex != str(ex):
+                logger.exception("retinanet worker call error")
+            self.last_ex = str(ex)
```

### Comparing `onvif-gui-1.0.3/onvif_gui/modules/sample.py` & `onvif-gui-1.0.4/modules/sample.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #/********************************************************************
-# libonvif/python/modules/sample.py 
+# onvif-gui/modules/sample.py 
 #
 # Copyright (c) 2023  Stephen Rhodes
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `onvif-gui-1.0.3/onvif_gui/modules/segment.py` & `onvif-gui-1.0.4/modules/segment.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 # Copyright (c) Facebook, Inc. and its affiliates.
-import numpy as np
-import torch
-import os
-import cv2
-from loguru import logger
-from sys import platform
-from pathlib import Path
-from detectron2.config import get_cfg
-from detectron2.predictor import Predictor
-from detectron2.tracker import DetectedInstance, SimpleTracker
-from PyQt6.QtWidgets import QWidget, QGridLayout, QLabel
-from PyQt6.QtCore import Qt
-from components import ThresholdSlider, LabelSelector
 
-# constants
+IMPORT_ERROR = ""
+try:
+    import numpy as np
+    import os
+    import cv2
+    from loguru import logger
+    from sys import platform
+    from pathlib import Path
+    from PyQt6.QtWidgets import QWidget, QGridLayout, QLabel, QMessageBox
+    from PyQt6.QtCore import Qt
+    from gui.components import ThresholdSlider, LabelSelector
+
+    import torch
+    from detectron2.config import get_cfg
+    from detectron2.predictor import Predictor
+    from detectron2.tracker import DetectedInstance, SimpleTracker
+except ModuleNotFoundError as ex:
+    IMPORT_ERROR = str(ex)
+    print("Import Error has occurred, missing modules need to be installed, please consult documentation: ", ex)
+
 MODULE_NAME = "detectron2/segment"
 
 class Configure(QWidget):
     def __init__(self, mw):
         try:
             super().__init__()
             self.mw = mw
@@ -47,27 +53,33 @@
             lytMain.setRowStretch(2, 10)
 
             self.mw.signals.started.connect(self.disableThresholdSlider)
             self.mw.signals.stopped.connect(self.enableThresholdSlider)
             if self.mw.playing:
                 self.sldThreshold.setEnabled(False)
 
+            if len(IMPORT_ERROR) > 0:
+                QMessageBox.critical(None, "Detectron2 Import Error", "Modules required for running this function are missing: " + IMPORT_ERROR)
+
         except:
             logger.exception("instance segmentation configuration load error")
 
     def disableThresholdSlider(self):
         self.sldThreshold.setEnabled(False)
 
     def enableThresholdSlider(self):
         self.sldThreshold.setEnabled(True)
 
 class Worker:
     def __init__(self, mw):
+        self.mw = mw
+        self.last_ex = ""
+        self.CONFIDENCE_THRESHOLD = self.mw.configure.sldThreshold.value()
+
         try:
-            self.mw = mw
             ckpt_file = 'auto'
             fp16 = True
             self.simple = True
             self.draw_overlay = False
             self.first_pass = True
 
             if ckpt_file is not None:
@@ -80,15 +92,14 @@
                         cache.parent.mkdir(parents=True, exist_ok=True)
                         torch.hub.download_url_to_file("https://dl.fbaipublicfiles.com/detectron2/COCO-InstanceSegmentation/mask_rcnn_R_50_FPN_3x/137849600/model_final_f10217.pkl", ckpt_file)
 
             cfg = get_cfg()
             cfg.merge_from_file('./detectron2/configs/COCO-InstanceSegmentation/mask_rcnn_R_50_FPN_3x.yaml')
             cfg.MODEL.WEIGHTS = ckpt_file
 
-            self.CONFIDENCE_THRESHOLD = self.mw.configure.sldThreshold.value()
             cfg.MODEL.RETINANET.SCORE_THRESH_TEST = self.CONFIDENCE_THRESHOLD
             cfg.MODEL.ROI_HEADS.SCORE_THRESH_TEST = self.CONFIDENCE_THRESHOLD
             cfg.MODEL.PANOPTIC_FPN.COMBINE.INSTANCES_CONFIDENCE_THRESH = self.CONFIDENCE_THRESHOLD
             cfg.freeze()
 
             self.tracker = SimpleTracker()
             self.predictor = Predictor(cfg, fp16)
@@ -152,16 +163,18 @@
             img *= composite
 
             for index, box in enumerate(boxes):
                 color = (colors[index] * 255).astype(int).tolist()
                 #cv2.rectangle(img, (box[0], box[1]), (box[2], box[3]), color, 2)
                 cv2.line(img, (box[0], box[3]), (box[2], box[3]), color, 2)
 
-        except:
-            logger.exception("Instance Segmentation runtime error")
+        except Exception as ex:
+            if self.last_ex != str(ex):
+                logger.exception("Instance Segmentation runtime error")
+            self.last_ex = str(ex)
 
     def get_auto_ckpt_filename(self):
         filename = None
         if platform == "win32":
             filename = os.environ['HOMEPATH'] + "/.cache/torch/hub/checkpoints/model_final_f10217.pkl"
         else:
             filename = os.environ['HOME'] + "/.cache/torch/hub/checkpoints/model_final_f10217.pkl"
```

### Comparing `onvif-gui-1.0.3/onvif_gui/modules/yolox.py` & `onvif-gui-1.0.4/modules/yolox.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,50 @@
-import cv2
-import torch
-import os
-import sys
-import numpy as np
-from pathlib import Path
-from loguru import logger
-from torchvision.transforms import functional
-import torch.nn as nn
-
-from yolox.models import YOLOX, YOLOPAFPN, YOLOXHead
-from yolox.utils import postprocess
-from components import ComboSelector, FileSelector, LabelSelector, ThresholdSlider
-from PyQt6.QtWidgets import QWidget, QGridLayout, QLabel, QCheckBox
-from PyQt6.QtCore import Qt
+#/********************************************************************
+# onvif-gui/modules/yolox.py 
+#
+# Copyright (c) 2023  Stephen Rhodes
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#    http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+#*********************************************************************/
+
+IMPORT_ERROR = ""
+try:
+    import cv2
+    import os
+    import sys
+    import numpy as np
+    from pathlib import Path
+    from loguru import logger
+
+    from gui.components import ComboSelector, FileSelector, LabelSelector, ThresholdSlider
+    from PyQt6.QtWidgets import QWidget, QGridLayout, QLabel, QCheckBox, QMessageBox
+    from PyQt6.QtCore import Qt
+
+    import torch
+    from torchvision.transforms import functional
+    import torch.nn as nn
+
+    from yolox.models import YOLOX, YOLOPAFPN, YOLOXHead
+    from yolox.utils import postprocess
+    from yolox.tracker.byte_tracker import BYTETracker
+
+except ModuleNotFoundError as ex:
+    IMPORT_ERROR = str(ex)
+    print("Import Error has occurred, missing modules need to be installed, please consult documentation: ", ex)
 
 os.environ['KMP_DUPLICATE_LIB_OK']='True'
 MODULE_NAME = "yolox"
 
 class Configure(QWidget):
     def __init__(self, mw):
         try:
@@ -38,20 +66,16 @@
             self.cmbType = ComboSelector(mw, "Model Name", ("yolox_s", "yolox_m", "yolox_l", "yolox_x"), "yolox_s", MODULE_NAME)
 
             self.chkFP16 = QCheckBox("Use half precision math")
             self.chkFP16.setChecked(int(self.mw.settings.value(self.fp16Key, 1)))
             self.chkFP16.stateChanged.connect(self.chkFP16Clicked)
 
             self.chkTrack = QCheckBox("Track Objects")
-            if sys.platform == "win32":
-                self.chkTrack.setChecked(int(self.mw.settings.value(self.trackKey, 0)))
-                self.chkTrack.stateChanged.connect(self.chkTrackClicked)
-            else:
-                self.chkTrack.setChecked(False)
-                self.chkTrack.setEnabled(False)
+            self.chkTrack.setChecked(int(self.mw.settings.value(self.trackKey, 0)))
+            self.chkTrack.stateChanged.connect(self.chkTrackClicked)
 
             self.sldConfThre = ThresholdSlider(mw, MODULE_NAME + "/confidence", "Confidence", 25)
             self.sldConfThre.setEnabled(not self.chkTrack.isChecked())
 
             number_of_labels = 5
             self.labels = []
             for i in range(number_of_labels):
@@ -73,14 +97,17 @@
             lytMain.addWidget(self.sldConfThre,  4, 0, 1, 1)
             lytMain.addWidget(self.chkFP16,      5, 0, 1, 1)
             lytMain.addWidget(self.chkTrack,     6, 0, 1, 1)
             lytMain.addWidget(pnlLabels,         7, 0, 1, 1)
             lytMain.addWidget(QLabel(),          8, 0, 1, 1)
             lytMain.setRowStretch(8, 10)
 
+            if len(IMPORT_ERROR) > 0:
+                QMessageBox.critical(None, "YOLOX Import Error", "Modules required for running this function are missing: " + IMPORT_ERROR)
+
         except:
             logger.exception("yolox configure failed to load")
 
     def chkAutoClicked(self, state):
         self.mw.settings.setValue(self.autoKey, state)
         self.txtFilename.setEnabled(not self.chkAuto.isChecked())
 
@@ -91,14 +118,15 @@
         self.mw.settings.setValue(self.trackKey, state)
         self.sldConfThre.setEnabled(not self.chkTrack.isChecked())
 
 class Worker:
     def __init__(self, mw):
         try:
             self.mw = mw
+            self.last_ex = ""
             device_name = "cpu"
             if torch.cuda.is_available():
                 device_name = "cuda"
             self.device = torch.device(device_name)
 
             self.num_classes = 80
 
@@ -133,17 +161,15 @@
                 self.ckpt_file = self.mw.configure.txtFilename.text()
 
             self.model.load_state_dict(torch.load(self.ckpt_file, map_location="cpu")["model"])
 
             if self.fp16:
                 self.model = self.model.half()
 
-            if self.track:
-                from yolox.tracker.byte_tracker import BYTETracker
-                self.tracker = BYTETracker(track_thresh, track_buffer, match_thresh)
+            self.tracker = BYTETracker(track_thresh, track_buffer, match_thresh)
 
         except:
             logger.exception("yolox initialization failure")
 
     def __call__(self, F):
         try:
             img = np.array(F, copy=False)
@@ -200,16 +226,18 @@
                     mask = np.in1d(labels, label_filter)
                     output = output[mask]
                     online_targets = self.tracker.update(output, [img.shape[0], img.shape[1]], test_size)
                     self.draw_track_boxes(img, online_targets)
                 else:
                     self.draw_plain_boxes(img, output, ratio)
 
-        except:
-            logger.exception("yolox runtime error")
+        except Exception as ex:
+            if self.last_ex != str(ex):
+                logger.exception("yolox runtime error")
+            self.last_ex = str(ex)
 
     def draw_plain_boxes(self, img, output, ratio):
         boxes = output[:, 0:4] / ratio
         labels = output[:, 6].numpy().astype(int)
         for lbl in self.mw.configure.labels:
             if lbl.chkBox.isChecked():
                 lbl_boxes = boxes[labels == lbl.label()].numpy().astype(int)
```

### Comparing `onvif-gui-1.0.3/onvif_gui/onvif/admintab.py` & `onvif-gui-1.0.4/gui/onvif/admintab.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #/********************************************************************
-# libonvif/python/admintab.py 
+# onvif-gui/gui/onvif/admintab.py 
 #
 # Copyright (c) 2023  Stephen Rhodes
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `onvif-gui-1.0.3/onvif_gui/onvif/imagetab.py` & `onvif-gui-1.0.4/gui/onvif/imagetab.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #/********************************************************************
-# libonvif/python/imagetab.py 
+# onvif-gui/gui/onvif/imagetab.py 
 #
 # Copyright (c) 2023  Stephen Rhodes
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `onvif-gui-1.0.3/onvif_gui/onvif/logindialog.py` & `onvif-gui-1.0.4/gui/onvif/logindialog.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #/********************************************************************
-# libonvif/python/logindialog.py 
+# onvif-gui/gui/onvif/logindialog.py 
 #
 # Copyright (c) 2023  Stephen Rhodes
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `onvif-gui-1.0.3/onvif_gui/onvif/networktab.py` & `onvif-gui-1.0.4/gui/onvif/networktab.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #/********************************************************************
-# libonvif/python/networktab.py 
+# onvif-gui/gui/onvif/networktab.py 
 #
 # Copyright (c) 2023  Stephen Rhodes
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `onvif-gui-1.0.3/onvif_gui/onvif/ptztab.py` & `onvif-gui-1.0.4/gui/onvif/ptztab.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #/********************************************************************
-# libonvif/python/ptztab.py 
+# onvif-gui/gui/onvif/ptztab.py 
 #
 # Copyright (c) 2023  Stephen Rhodes
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `onvif-gui-1.0.3/onvif_gui/onvif/videotab.py` & `onvif-gui-1.0.4/gui/onvif/videotab.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #/********************************************************************
-# libonvif/python/videotab.py 
+# onvif-gui/gui/onvif/videotab.py 
 #
 # Copyright (c) 2023  Stephen Rhodes
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `onvif-gui-1.0.3/onvif_gui/panels/camerapanel.py` & `onvif-gui-1.0.4/gui/panels/camerapanel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #/********************************************************************
-# libonvif/python/camerapanel.py 
+# onvif-gui/gui/panels/camerapanel.py 
 #
 # Copyright (c) 2023  Stephen Rhodes
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -20,15 +20,15 @@
 import sys
 from time import sleep
 import datetime
 from PyQt6.QtWidgets import QPushButton, QGridLayout, QWidget, QSlider, \
 QListWidget, QTabWidget, QMessageBox
 from PyQt6.QtGui import QIcon
 from PyQt6.QtCore import Qt, pyqtSignal, QObject, QSettings, QTimer
-from onvif_gui.onvif import AdminTab, NetworkTab, ImageTab, VideoTab, PTZTab, LoginDialog
+from gui.onvif import AdminTab, NetworkTab, ImageTab, VideoTab, PTZTab, LoginDialog
 
 sys.path.append("../build/libonvif")
 sys.path.append("../build/libonvif/Release")
 import libonvif as onvif
 
 ICON_SIZE = 26
```

### Comparing `onvif-gui-1.0.3/onvif_gui/panels/filepanel.py` & `onvif-gui-1.0.4/gui/panels/filepanel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #/********************************************************************
-# libonvif/python/filepanel.py 
+# onvif-gui/gui/panels/filepanel.py 
 #
 # Copyright (c) 2023  Stephen Rhodes
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -20,15 +20,15 @@
 import sys
 import datetime
 from PyQt6.QtWidgets import QLineEdit, QPushButton, \
 QGridLayout, QWidget, QSlider, QLabel, QMessageBox, \
 QTreeView, QFileDialog, QMenu
 from PyQt6.QtGui import QFileSystemModel, QAction
 from PyQt6.QtCore import Qt, QStandardPaths, QFile
-from onvif_gui.components import Progress
+from gui.components import Progress
 
 sys.path.append("../build/libavio")
 sys.path.append("../build/libavio/Release")
 import avio
 
 ICON_SIZE = 26
 
@@ -49,15 +49,14 @@
     
 class DirectorySetter(QWidget):
     def __init__(self, mw):
         super().__init__()
         self.mw = mw
         self.txtDirectory = QLineEdit()
         self.btnSelect = QPushButton("...")
-        self.btnSelect.setMaximumWidth(52)
         self.btnSelect.clicked.connect(self.btnSelectClicked)
         self.dlgFile = QFileDialog()
         lytMain = QGridLayout(self)
         lytMain.setContentsMargins(0, 0, 0, 0)
         lytMain.addWidget(self.txtDirectory,   0, 0, 1, 1)
         lytMain.addWidget(self.btnSelect,      0, 1, 1, 1)
         lytMain.setColumnStretch(0, 10)
@@ -280,15 +279,15 @@
         index = self.tree.indexAt(pos)
         if index.isValid():
             self.menu.exec(self.mapToGlobal(pos))
 
     def onMenuRemove(self):
         index = self.tree.currentIndex()
         if index.isValid():
-            ret = QMessageBox.warning(self, "onvif_gui",
+            ret = QMessageBox.warning(self, "onvif-gui",
                                         "You are about to delete this file.\n"
                                         "Are you sure you want to continue?",
                                         QMessageBox.StandardButton.Ok | QMessageBox.StandardButton.Cancel)
 
             if ret == QMessageBox.StandardButton.Ok:
                 QFile.remove(self.model.filePath(self.tree.currentIndex()))
```

### Comparing `onvif-gui-1.0.3/onvif_gui/panels/modulepanel.py` & `onvif-gui-1.0.4/gui/panels/modulepanel.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #/********************************************************************
-# libonvif/python/modulepanel.py 
+# onvif-gui/gui/panels/modulepanel.py 
 #
 # Copyright (c) 2023  Stephen Rhodes
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -16,57 +16,77 @@
 # limitations under the License.
 #
 #*********************************************************************/
 
 import os
 from PyQt6.QtWidgets import QGridLayout, QWidget, QCheckBox, \
     QLabel, QComboBox, QVBoxLayout
+from gui.components import DirectorySelector
 
 class ModulePanel(QWidget):
     def __init__(self, mw):
         super().__init__()
         self.mw = mw
         self.panel = None
         self.layout = QVBoxLayout(self)
         self.workerKey = "Modules/worker"
         self.engageKey = "Modules/engage"
+        self.directoryKey = "Modules/directory"
+        self.cmbWorkerConnected = True
+
+        stdLocation = mw.getLocation() + "/modules"
+        self.dirModules = DirectorySelector(mw, self.directoryKey, "Modules Dir", stdLocation)
+        self.dirModules.signals.dirChanged.connect(self.dirModulesChanged)
 
         self.cmbWorker = QComboBox()
-        workers = os.listdir(mw.getLocation() + "/modules")
-        for worker in workers:
-            if not worker.endswith(".py"):
-                workers.remove(worker)
-        self.cmbWorker.addItems(workers)
+        self.fillModules()
         self.cmbWorker.setCurrentText(mw.settings.value(self.workerKey, "sample.py"))
         self.cmbWorker.currentTextChanged.connect(self.cmbWorkerChanged)
         lblWorkers = QLabel("Python Worker")
 
         self.chkEngage = QCheckBox("Engage")
         self.chkEngage.setChecked(int(mw.settings.value(self.engageKey, 0)))
         self.chkEngage.stateChanged.connect(self.chkEngageClicked)
 
         self.lblElapsed = QLabel()
 
         fixedPanel = QWidget()
         lytFixed = QGridLayout(fixedPanel)
-        lytFixed.addWidget(lblWorkers,       0, 0, 1, 1)
-        lytFixed.addWidget(self.cmbWorker,   0, 1, 1, 1)
-        lytFixed.addWidget(self.chkEngage,   1, 0, 1, 1)
-        lytFixed.addWidget(self.lblElapsed,  1, 1, 1, 1)
+        lytFixed.addWidget(self.dirModules,  0, 0, 1, 2)
+        lytFixed.addWidget(lblWorkers,       1, 0, 1, 1)
+        lytFixed.addWidget(self.cmbWorker,   1, 1, 1, 1)
+        lytFixed.addWidget(self.chkEngage,   2, 0, 1, 1)
+        lytFixed.addWidget(self.lblElapsed,  2, 1, 1, 1)
         lytFixed.setColumnStretch(1, 10)
         self.layout.addWidget(fixedPanel)
 
+    def fillModules(self):
+        workers = os.listdir(self.dirModules.text())
+        for worker in workers:
+            if not worker.endswith(".py") or worker == "__init__.py":
+                workers.remove(worker)
+        workers.sort()
+        self.cmbWorker.clear()
+        self.cmbWorker.addItems(workers)
+
     def setPanel(self, panel):
         if self.panel is not None:
             self.layout.removeWidget(self.panel)
         self.panel = panel
         self.panel.setMaximumWidth(self.mw.tab.width())
         self.layout.addWidget(panel)
         self.layout.setStretch(1, 10)
 
     def cmbWorkerChanged(self, worker):
-        self.mw.settings.setValue(self.workerKey, worker)
-        self.mw.loadConfigure(worker)
-        self.mw.loadWorker(worker)
+        if self.cmbWorkerConnected:
+            self.mw.settings.setValue(self.workerKey, worker)
+            self.mw.loadConfigure(worker)
+            self.mw.loadWorker(worker)
 
     def chkEngageClicked(self, state):
-        self.mw.settings.setValue(self.engageKey, state)
+        self.mw.settings.setValue(self.engageKey, state)
+
+    def dirModulesChanged(self, path):
+        self.cmbWorkerConnected = False
+        self.fillModules()
+        self.cmbWorkerConnected = True
+        self.cmbWorkerChanged(self.cmbWorker.currentText())
```

### Comparing `onvif-gui-1.0.3/onvif_gui/panels/settingspanel.py` & `onvif-gui-1.0.4/gui/panels/settingspanel.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #/********************************************************************
-# libonvif/python/settingspanel.py 
+# onvif-gui/gui/panels/settingspanel.py 
 #
 # Copyright (c) 2023  Stephen Rhodes
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -68,24 +68,14 @@
         
         self.cmbDecoder = QComboBox()
         self.cmbDecoder.addItems(decoders)
         self.cmbDecoder.setCurrentText(mw.settings.value(self.decoderKey, "NONE"))
         self.cmbDecoder.currentTextChanged.connect(self.cmbDecoderChanged)
         lblDecoders = QLabel("Hardware Decoder")
 
-        #self.cmbWorker = QComboBox()
-        #workers = os.listdir("modules")
-        #for worker in workers:
-        #    if not worker.endswith(".py"):
-        #        workers.remove(worker)
-        #self.cmbWorker.addItems(workers)
-        #self.cmbWorker.setCurrentText(mw.settings.value(self.workerKey, "sample.py"))
-        #self.cmbWorker.currentTextChanged.connect(self.cmbWorkerChanged)
-        #lblWorkers = QLabel("Python Worker")
-        
         self.chkDirectRender = QCheckBox("Direct Rendering")
         self.render = int(mw.settings.value(self.renderKey, 0))
         self.chkDirectRender.setChecked(self.render)
         self.chkDirectRender.clicked.connect(self.directRenderChecked)
 
         if sys.platform == "win32":
             self.chkDirectRender.setEnabled(True)
@@ -116,31 +106,26 @@
         self.chkPostEncode.stateChanged.connect(self.postEncodeChecked)
 
         self.chkHardwareEncode = QCheckBox("Hardware Encode")
         self.chkHardwareEncode.setChecked(int(mw.settings.value(self.hardwareEncodeKey, 0)))
         self.chkHardwareEncode.setEnabled(self.chkPostEncode.isChecked())
         self.chkHardwareEncode.stateChanged.connect(self.hardwareEncodeChecked)
 
-        #self.chkProcessFrame = QCheckBox("Process Frame")
-        #self.chkProcessFrame.setChecked(int(mw.settings.value(self.processFrameKey, 0)))
-        #self.chkProcessFrame.stateChanged.connect(self.processFrameChecked)
-
         self.chkLowLatency = QCheckBox("Low Latency")
         self.chkLowLatency.setChecked(int(mw.settings.value(self.latencyKey, 0)))
         self.chkLowLatency.stateChanged.connect(self.lowLatencyChecked)
 
         pnlChecks = QWidget()
         lytChecks = QGridLayout(pnlChecks)
         lytChecks.addWidget(self.chkDirectRender,   0, 0, 1, 1)
         lytChecks.addWidget(self.chkConvert2RGB,    0, 1, 1, 1)
         lytChecks.addWidget(self.chkDisableAudio,   1, 0, 1, 1)
         lytChecks.addWidget(self.chkDisableVideo,   1, 1, 1, 1)
         lytChecks.addWidget(self.chkPostEncode,     2, 0, 1, 1)
         lytChecks.addWidget(self.chkHardwareEncode, 2, 1, 1, 1)
-        #lytChecks.addWidget(self.chkProcessFrame,   3, 0, 1, 1)
         lytChecks.addWidget(self.chkLowLatency,     3, 1, 1, 1)
 
         self.spnCacheSize = QSpinBox()
         self.spnCacheSize.setMinimum(1)
         self.spnCacheSize.setMaximum(10)
         self.spnCacheSize.setMaximumWidth(80)
         self.spnCacheSize.setValue(int(self.mw.settings.value(self.cacheSizeKey, 1)))
@@ -183,43 +168,36 @@
         lytMain.addWidget(self.chkAutoDiscover,   0, 0, 1, 2)
         lytMain.addWidget(lblUsername,            1, 0, 1, 1)
         lytMain.addWidget(self.txtUsername,       1, 1, 1, 1)
         lytMain.addWidget(lblPassword,            2, 0, 1, 1)
         lytMain.addWidget(self.txtPassword,       2, 1, 1, 1)
         lytMain.addWidget(lblDecoders,            3, 0, 1, 1)
         lytMain.addWidget(self.cmbDecoder,        3, 1, 1, 1)
-        #lytMain.addWidget(lblWorkers,             4, 0, 1, 1)
-        #lytMain.addWidget(self.cmbWorker,         4, 1, 1, 1)
-        lytMain.addWidget(pnlFilter,              5, 0, 1, 3)
-        lytMain.addWidget(pnlChecks,              6, 0, 1, 3)
-        lytMain.addWidget(lblCacheSize,           7, 0, 1, 1)
-        lytMain.addWidget(self.spnCacheSize,      7, 1, 1, 1)
-        lytMain.addWidget(pnlInterface,           8, 0, 1, 3)
-        lytMain.addWidget(QLabel(""),             9, 0, 1, 3)
-        lytMain.setRowStretch(9, 10)
+        lytMain.addWidget(pnlFilter,              6, 0, 1, 3)
+        lytMain.addWidget(pnlChecks,              7, 0, 1, 3)
+        lytMain.addWidget(lblCacheSize,           8, 0, 1, 1)
+        lytMain.addWidget(self.spnCacheSize,      8, 1, 1, 1)
+        lytMain.addWidget(pnlInterface,           9, 0, 1, 3)
+        lytMain.addWidget(QLabel(""),            10, 0, 1, 3)
+        lytMain.setRowStretch(10, 10)
 
     def autoDiscoverChecked(self, state):
         self.mw.settings.setValue(self.autoDiscoverKey, state)
 
     def usernameChanged(self, username):
         self.mw.settings.setValue(self.usernameKey, username)
 
     def passwordChanged(self, password):
         self.mw.settings.setValue(self.passwordKey, password)
 
     def cmbDecoderChanged(self, decoder):
         self.mw.settings.setValue(self.decoderKey, decoder)
 
-    #def cmbWorkerChanged(self, worker):
-    #    self.mw.settings.setValue(self.workerKey, worker)
-    #    self.mw.loadConfigure(worker)
-    #    self.mw.loadWorker(worker)
-
     def directRenderChecked(self):
-        ret = QMessageBox.warning(self, "onvif_gui",
+        ret = QMessageBox.warning(self, "onvif-gui",
                                     "Application must restart to enact change.\n"
                                     "Are you sure you want to continue?",
                                     QMessageBox.StandardButton.Ok | QMessageBox.StandardButton.Cancel)
         if ret == QMessageBox.StandardButton.Ok:
             if self.render == 1:
                 self.mw.settings.setValue(self.renderKey, 0)
             else:
@@ -257,17 +235,14 @@
         if state == 0:
             self.chkHardwareEncode.setChecked(False)
         self.chkHardwareEncode.setEnabled(state)
 
     def hardwareEncodeChecked(self, state):
         self.mw.settings.setValue(self.hardwareEncodeKey, state)
 
-    #def processFrameChecked(self, state):
-    #    self.mw.settings.setValue(self.processFrameKey, state)
-
     def lowLatencyChecked(self, state):
         self.mw.settings.setValue(self.latencyKey, state)
 
     def radioFilenameChecked(self):
         if self.radGenerateFilename.isChecked():
             self.mw.settings.setValue(self.generateKey, 1)
         else:
```

### Comparing `onvif-gui-1.0.3/onvif_gui/resources/audio.png` & `onvif-gui-1.0.4/gui/resources/audio.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/resources/audio_hi.png` & `onvif-gui-1.0.4/gui/resources/audio_hi.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/resources/audio_lo.png` & `onvif-gui-1.0.4/gui/resources/audio_lo.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/resources/darkstyle.qss` & `onvif-gui-1.0.4/gui/resources/darkstyle.qss`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+/********************************************************************
+* onvif-gui/gui/resources/darkstyle.qss
+*
+* Copyright (c) 2023  Stephen Rhodes
+*
+* Licensed under the Apache License, Version 2.0 (the "License");
+* you may not use this file except in compliance with the License.
+* You may obtain a copy of the License at
+*
+*    http://www.apache.org/licenses/LICENSE-2.0
+*
+* Unless required by applicable law or agreed to in writing, software
+* distributed under the License is distributed on an "AS IS" BASIS,
+* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+* See the License for the specific language governing permissions and
+* limitations under the License.
+*
+*********************************************************************/
+
 QWidget {
     background-color : background_dark;
     color : foreground_light;
 }
 
 QMenuBar::item:selected {
     background-color : background_medium;
```

### Comparing `onvif-gui-1.0.3/onvif_gui/resources/discover.png` & `onvif-gui-1.0.4/gui/resources/discover.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/resources/discover_hi.png` & `onvif-gui-1.0.4/gui/resources/discover_hi.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/resources/discover_lo.png` & `onvif-gui-1.0.4/gui/resources/discover_lo.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/resources/mute.png` & `onvif-gui-1.0.4/gui/resources/mute.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/resources/mute_lo.png` & `onvif-gui-1.0.4/gui/resources/mute_lo.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/resources/onvif_gui.png` & `onvif-gui-1.0.4/gui/resources/onvif-gui.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/resources/recording_lo.png` & `onvif-gui-1.0.4/gui/resources/recording_lo.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/yolox/models/__init__.py` & `onvif-gui-1.0.4/yolox/models/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/yolox/models/build.py` & `onvif-gui-1.0.4/yolox/models/build.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/yolox/models/darknet.py` & `onvif-gui-1.0.4/yolox/models/darknet.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/yolox/models/losses.py` & `onvif-gui-1.0.4/yolox/models/losses.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/yolox/models/network_blocks.py` & `onvif-gui-1.0.4/yolox/models/network_blocks.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/yolox/models/yolo_fpn.py` & `onvif-gui-1.0.4/yolox/models/yolo_fpn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/yolox/models/yolo_head.py` & `onvif-gui-1.0.4/yolox/models/yolo_head.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/yolox/models/yolo_pafpn.py` & `onvif-gui-1.0.4/yolox/models/yolo_pafpn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/yolox/models/yolox.py` & `onvif-gui-1.0.4/yolox/models/yolox.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/yolox/tracker/basetrack.py` & `onvif-gui-1.0.4/yolox/tracker/basetrack.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/yolox/tracker/byte_tracker.py` & `onvif-gui-1.0.4/yolox/tracker/byte_tracker.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/yolox/tracker/kalman_filter.py` & `onvif-gui-1.0.4/yolox/tracker/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/yolox/tracker/matching.py` & `onvif-gui-1.0.4/yolox/tracker/matching.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui/yolox/utils/utils.py` & `onvif-gui-1.0.4/yolox/utils/utils.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.3/onvif_gui.egg-info/PKG-INFO` & `onvif-gui-1.0.4/onvif_gui.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: onvif-gui
-Version: 1.0.3
+Version: 1.0.4
 Summary: A client gui for Onvif
 Author: Stephen Rhodes
 Author-email: Stephen Rhodes <sr99622@gmail.com>
+Project-URL: Homepage, https://github.com/sr99622/libonvif
+Project-URL: Bug Reports, https://github.com/sr99622/libonvif/issues
 Keywords: sample,setuptools,development
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # onvif-gui
 
@@ -47,21 +49,21 @@
 ```
 pip install onvif-gui
 ```
 
 Modules
 -----------------
 
-onvif_gui has a facility for incorporating python programs to operate on the
+onvif-gui has a facility for incorporating python programs to operate on the
 video stream.  The Modules tab is the user interface for this feature.  There
 is a minimal example program called sample.py that demonstrates how data is 
 trsansferred from the main program to the python module and it's GUI interface
 implementation.
 
-There is included with onvif_gui a full implementation of the YOLOX algorithm
+There is included with onvif-gui a full implementation of the YOLOX algorithm
 along with an associated tracking algorithm known as ByteTrack.  These algorithms 
 are implemented using pytorch, which requires some specific configuration. Note
 that ByteTrack currently is available only on Windows.
 
 Note on Running PyTorch Modules
 --------------------------------
 
@@ -77,29 +79,29 @@
 
 
 Onvif GUI Program
 -----------------
 
 NAME 
 
-    onvif_gui
+    onvif-gui
 
 SYNOPSIS
 
-    onvif_gui is a python program.  
+    onvif-gui is a python program.  
     
     The program requires the following modules:
 
     pip install pyqt6 opencv-python numpy loguru
     
 
     To run the program:
 
-    cd ../onvif_gui
-    python3 main.py
+    cd ../onvif-gui
+    python3 run.py
 
     These instructions are intended for quick setup to verify the program.  To use the 
     library in other python programs, it is advised to install the onvif and avio
     python modules.
 
     cd ../libonvif
     python3 setup.py install
```

