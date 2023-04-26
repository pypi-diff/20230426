# Comparing `tmp/icepy4d-1.4.0.tar.gz` & `tmp/icepy4d-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icepy4d-1.4.0.tar", last modified: Thu Apr 20 08:54:14 2023, max compression
+gzip compressed data, was "icepy4d-1.6.2.tar", last modified: Tue Apr 25 16:21:23 2023, max compression
```

## Comparing `icepy4d-1.4.0.tar` & `icepy4d-1.6.2.tar`

### file list

```diff
@@ -1,132 +1,140 @@
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-20 08:54:14.992865 icepy4d-1.4.0/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1071 2022-11-10 18:54:33.000000 icepy4d-1.4.0/LICENSE.txt
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     3869 2023-04-20 08:54:14.992865 icepy4d-1.4.0/PKG-INFO
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2017 2023-04-20 08:51:29.000000 icepy4d-1.4.0/README.md
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1623 2023-04-20 08:53:52.000000 icepy4d-1.4.0/pyproject.toml
--rw-rw-r--   0 francesco  (1000) francesco  (1000)       38 2023-04-20 08:54:14.992865 icepy4d-1.4.0/setup.cfg
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-20 08:54:14.984865 icepy4d-1.4.0/src/
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-20 08:54:14.984865 icepy4d-1.4.0/src/icepy4d/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)       55 2023-04-20 08:00:10.000000 icepy4d-1.4.0/src/icepy4d/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      244 2023-04-20 07:59:46.000000 icepy4d-1.4.0/src/icepy4d/__main__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    13046 2023-04-04 14:17:37.000000 icepy4d-1.4.0/src/icepy4d/binned_stats.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-20 08:54:14.988865 icepy4d-1.4.0/src/icepy4d/classes/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      235 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/classes/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    17269 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/classes/camera.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1079 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/classes/dsm.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1079 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/classes/epoch.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    26531 2023-04-20 07:59:46.000000 icepy4d-1.4.0/src/icepy4d/classes/features.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    19126 2023-04-20 08:26:25.000000 icepy4d-1.4.0/src/icepy4d/classes/images.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1079 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/classes/ortophoto.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     6786 2023-04-20 08:36:17.000000 icepy4d-1.4.0/src/icepy4d/classes/point_cloud.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    18374 2023-04-20 07:59:46.000000 icepy4d-1.4.0/src/icepy4d/classes/points.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     3262 2023-04-20 07:59:46.000000 icepy4d-1.4.0/src/icepy4d/classes/solution.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    11317 2023-04-20 07:59:46.000000 icepy4d-1.4.0/src/icepy4d/classes/targets.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      789 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/classes/typed_dict_classes.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-20 08:54:14.988865 icepy4d-1.4.0/src/icepy4d/io/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)        0 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/io/__init__.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-20 08:54:14.988865 icepy4d-1.4.0/src/icepy4d/io/colmap_utils/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)        0 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/io/colmap_utils/__init__.py
--rwxrwxr-x   0 francesco  (1000) francesco  (1000)    22889 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/io/colmap_utils/build.py
--rwxrwxr-x   0 francesco  (1000) francesco  (1000)     3709 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/io/colmap_utils/build_windows_app.py
--rwxrwxr-x   0 francesco  (1000) francesco  (1000)     4731 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/io/colmap_utils/bundler_to_ply.py
--rwxrwxr-x   0 francesco  (1000) francesco  (1000)     2622 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/io/colmap_utils/clang_format_code.py
--rwxrwxr-x   0 francesco  (1000) francesco  (1000)     5565 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/io/colmap_utils/crawl_camera_specs.py
--rwxrwxr-x   0 francesco  (1000) francesco  (1000)    15026 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/io/colmap_utils/database.py
--rwxrwxr-x   0 francesco  (1000) francesco  (1000)     3389 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/io/colmap_utils/export_inlier_matches.py
--rwxrwxr-x   0 francesco  (1000) francesco  (1000)     3237 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/io/colmap_utils/export_inlier_pairs.py
--rwxrwxr-x   0 francesco  (1000) francesco  (1000)     6730 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/io/colmap_utils/export_to_bundler.py
--rwxrwxr-x   0 francesco  (1000) francesco  (1000)     6402 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/io/colmap_utils/export_to_visualsfm.py
--rwxrwxr-x   0 francesco  (1000) francesco  (1000)     6297 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/io/colmap_utils/flickr_downloader.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     5996 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/io/colmap_utils/h5_to_db.py
--rwxrwxr-x   0 francesco  (1000) francesco  (1000)     2692 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/io/colmap_utils/merge_ply_files.py
--rwxrwxr-x   0 francesco  (1000) francesco  (1000)     4743 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/io/colmap_utils/nvm_to_ply.py
--rwxrwxr-x   0 francesco  (1000) francesco  (1000)    25506 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/io/colmap_utils/plyfile.py
--rwxrwxr-x   0 francesco  (1000) francesco  (1000)     5172 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/io/colmap_utils/read_write_dense.py
--rwxrwxr-x   0 francesco  (1000) francesco  (1000)     5230 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/io/colmap_utils/read_write_fused_vis.py
--rwxrwxr-x   0 francesco  (1000) francesco  (1000)    22035 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/io/colmap_utils/read_write_model.py
--rwxrwxr-x   0 francesco  (1000) francesco  (1000)     7069 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/io/colmap_utils/visualize_model.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     8925 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/io/export2bundler.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2922 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/io/export2calge.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     4751 2023-04-20 08:06:11.000000 icepy4d-1.4.0/src/icepy4d/io/export2colmap.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2995 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/io/export2textfile.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1617 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/io/importing.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-20 08:54:14.988865 icepy4d-1.4.0/src/icepy4d/least_squares/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)        0 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/least_squares/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2845 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/least_squares/rototra3d.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2761 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/least_squares/utils.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-20 08:54:14.988865 icepy4d-1.4.0/src/icepy4d/matching/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)        0 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/matching/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    11728 2023-04-20 08:06:11.000000 icepy4d-1.4.0/src/icepy4d/matching/match_by_preselection.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    13680 2023-04-20 07:59:46.000000 icepy4d-1.4.0/src/icepy4d/matching/match_pairs.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     7602 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/matching/matching_base.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1656 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/matching/retrieve_matches_from_npz.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     4119 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/matching/superglue_match_simple_old.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    14758 2023-04-20 07:59:46.000000 icepy4d-1.4.0/src/icepy4d/matching/superglue_matcher.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    13567 2023-04-20 07:59:46.000000 icepy4d-1.4.0/src/icepy4d/matching/superglue_tracker.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    15735 2023-04-20 07:59:46.000000 icepy4d-1.4.0/src/icepy4d/matching/templatematch.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    16784 2023-04-20 07:59:46.000000 icepy4d-1.4.0/src/icepy4d/matching/track_matches.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    18740 2023-04-20 07:59:46.000000 icepy4d-1.4.0/src/icepy4d/matching/track_matches_bk.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     3440 2023-04-20 08:06:11.000000 icepy4d-1.4.0/src/icepy4d/matching/tracking_base.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     5879 2023-04-20 08:06:11.000000 icepy4d-1.4.0/src/icepy4d/matching/utils.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-20 08:54:14.988865 icepy4d-1.4.0/src/icepy4d/metashape/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)        0 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/metashape/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    20120 2023-04-20 08:37:45.000000 icepy4d-1.4.0/src/icepy4d/metashape/metashape.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    18631 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/metashape/ms_utils.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-20 08:54:14.988865 icepy4d-1.4.0/src/icepy4d/point_cloud_proc/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)        0 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/point_cloud_proc/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     7242 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/point_cloud_proc/cloudcompare_fun.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    12502 2023-04-20 07:59:46.000000 icepy4d-1.4.0/src/icepy4d/point_cloud_proc/open3d_fun.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      974 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/point_cloud_proc/utils.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-20 08:54:14.988865 icepy4d-1.4.0/src/icepy4d/sfm/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      218 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/sfm/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    14455 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/sfm/absolute_orientation.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     6506 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/sfm/geometry.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     4404 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/sfm/interpolate_colors.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1333 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/sfm/reconstruction.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     6342 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/sfm/triangulation.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     8073 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/sfm/two_view_geometry.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-20 08:54:14.988865 icepy4d-1.4.0/src/icepy4d/thirdparty/
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-20 08:54:14.988865 icepy4d-1.4.0/src/icepy4d/thirdparty/SuperGluePretrainedNetwork/
--rwxrwxr-x   0 francesco  (1000) francesco  (1000)    10683 2023-03-31 12:00:43.000000 icepy4d-1.4.0/src/icepy4d/thirdparty/SuperGluePretrainedNetwork/demo_superglue.py
--rwxrwxr-x   0 francesco  (1000) francesco  (1000)    18127 2023-03-31 12:00:43.000000 icepy4d-1.4.0/src/icepy4d/thirdparty/SuperGluePretrainedNetwork/match_pairs.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-20 08:54:14.988865 icepy4d-1.4.0/src/icepy4d/thirdparty/SuperGluePretrainedNetwork/models/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)        0 2023-03-31 12:00:43.000000 icepy4d-1.4.0/src/icepy4d/thirdparty/SuperGluePretrainedNetwork/models/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     3417 2023-03-31 12:00:43.000000 icepy4d-1.4.0/src/icepy4d/thirdparty/SuperGluePretrainedNetwork/models/matching.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    11781 2023-03-31 12:00:43.000000 icepy4d-1.4.0/src/icepy4d/thirdparty/SuperGluePretrainedNetwork/models/superglue.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     8142 2023-03-31 12:00:43.000000 icepy4d-1.4.0/src/icepy4d/thirdparty/SuperGluePretrainedNetwork/models/superpoint.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    20039 2023-03-31 12:00:43.000000 icepy4d-1.4.0/src/icepy4d/thirdparty/SuperGluePretrainedNetwork/models/utils.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)        0 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/thirdparty/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    11815 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/thirdparty/templatematch_pyimgraft.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    67149 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/thirdparty/transformations.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    10133 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/thirdparty/triangulation.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     7325 2023-04-20 07:59:46.000000 icepy4d-1.4.0/src/icepy4d/tiles.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    16090 2023-04-20 08:06:11.000000 icepy4d-1.4.0/src/icepy4d/tracking_features_utils.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-20 08:54:14.988865 icepy4d-1.4.0/src/icepy4d/utils/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      295 2023-04-20 08:50:34.000000 icepy4d-1.4.0/src/icepy4d/utils/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     7091 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/utils/dsm_orthophoto.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    12263 2023-04-20 08:30:14.000000 icepy4d-1.4.0/src/icepy4d/utils/initialization.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     5957 2023-04-20 07:59:46.000000 icepy4d-1.4.0/src/icepy4d/utils/logger.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     6355 2023-04-03 09:10:13.000000 icepy4d-1.4.0/src/icepy4d/utils/rototranslation.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1552 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/utils/sensor_width_database.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     3783 2023-04-20 07:59:46.000000 icepy4d-1.4.0/src/icepy4d/utils/spatial_funs.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1662 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/utils/timer.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     4893 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/utils/utils.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-20 08:54:14.988865 icepy4d-1.4.0/src/icepy4d/visualization/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)       29 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/visualization/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     6162 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/visualization/vis_o3d_advanced.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    27688 2023-04-20 07:59:46.000000 icepy4d-1.4.0/src/icepy4d/visualization/visualization.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-20 08:54:14.984865 icepy4d-1.4.0/src/icepy4d.egg-info/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     3869 2023-04-20 08:54:14.000000 icepy4d-1.4.0/src/icepy4d.egg-info/PKG-INFO
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     4254 2023-04-20 08:54:14.000000 icepy4d-1.4.0/src/icepy4d.egg-info/SOURCES.txt
--rw-rw-r--   0 francesco  (1000) francesco  (1000)        1 2023-04-20 08:54:14.000000 icepy4d-1.4.0/src/icepy4d.egg-info/dependency_links.txt
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      246 2023-04-20 08:54:14.000000 icepy4d-1.4.0/src/icepy4d.egg-info/requires.txt
--rw-rw-r--   0 francesco  (1000) francesco  (1000)        8 2023-04-20 08:54:14.000000 icepy4d-1.4.0/src/icepy4d.egg-info/top_level.txt
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-20 08:54:14.992865 icepy4d-1.4.0/tests/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     8220 2023-04-20 07:59:47.000000 icepy4d-1.4.0/tests/test_features.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1484 2023-04-20 07:59:47.000000 icepy4d-1.4.0/tests/test_image.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2394 2023-04-20 08:42:31.000000 icepy4d-1.4.0/tests/test_initialization.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      775 2023-04-20 07:59:47.000000 icepy4d-1.4.0/tests/test_matching.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2032 2023-04-20 07:59:47.000000 icepy4d-1.4.0/tests/test_point_cloud.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2742 2023-04-20 07:59:47.000000 icepy4d-1.4.0/tests/test_sfm_geometry.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      518 2023-04-20 07:59:47.000000 icepy4d-1.4.0/tests/test_utils.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1457 2023-04-20 07:59:47.000000 icepy4d-1.4.0/tests/test_utils_spatial.py
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-25 16:21:23.911137 icepy4d-1.6.2/
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     1558 2023-04-20 09:19:34.000000 icepy4d-1.6.2/LICENSE.txt
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     4168 2023-04-25 16:21:23.911137 icepy4d-1.6.2/PKG-INFO
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     1765 2023-04-25 16:19:58.000000 icepy4d-1.6.2/README.md
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     1623 2023-04-25 16:20:56.000000 icepy4d-1.6.2/pyproject.toml
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)       38 2023-04-25 16:21:23.911137 icepy4d-1.6.2/setup.cfg
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-25 16:21:23.903137 icepy4d-1.6.2/src/
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-25 16:21:23.903137 icepy4d-1.6.2/src/icepy4d/
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)       55 2023-04-25 16:20:56.000000 icepy4d-1.6.2/src/icepy4d/__init__.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)      244 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/__main__.py
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-25 16:21:23.907137 icepy4d-1.6.2/src/icepy4d/classes/
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)      235 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/classes/__init__.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    17269 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/classes/camera.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     1079 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/classes/dsm.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     1079 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/classes/epoch.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    26531 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/classes/features.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    19126 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/classes/images.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     1079 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/classes/ortophoto.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     6786 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/classes/point_cloud.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    18374 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/classes/points.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     3262 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/classes/solution.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    11317 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/classes/targets.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)      789 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/classes/typed_dict_classes.py
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-25 16:21:23.907137 icepy4d-1.6.2/src/icepy4d/io/
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)        0 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/io/__init__.py
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-25 16:21:23.907137 icepy4d-1.6.2/src/icepy4d/io/colmap_utils/
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)        0 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/io/colmap_utils/__init__.py
+-rwxrwxr-x   0 francesco  (1000) francesco  (1000)    22889 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/io/colmap_utils/build.py
+-rwxrwxr-x   0 francesco  (1000) francesco  (1000)     3709 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/io/colmap_utils/build_windows_app.py
+-rwxrwxr-x   0 francesco  (1000) francesco  (1000)     4731 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/io/colmap_utils/bundler_to_ply.py
+-rwxrwxr-x   0 francesco  (1000) francesco  (1000)     2622 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/io/colmap_utils/clang_format_code.py
+-rwxrwxr-x   0 francesco  (1000) francesco  (1000)     5565 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/io/colmap_utils/crawl_camera_specs.py
+-rwxrwxr-x   0 francesco  (1000) francesco  (1000)    15026 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/io/colmap_utils/database.py
+-rwxrwxr-x   0 francesco  (1000) francesco  (1000)     3389 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/io/colmap_utils/export_inlier_matches.py
+-rwxrwxr-x   0 francesco  (1000) francesco  (1000)     3237 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/io/colmap_utils/export_inlier_pairs.py
+-rwxrwxr-x   0 francesco  (1000) francesco  (1000)     6730 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/io/colmap_utils/export_to_bundler.py
+-rwxrwxr-x   0 francesco  (1000) francesco  (1000)     6402 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/io/colmap_utils/export_to_visualsfm.py
+-rwxrwxr-x   0 francesco  (1000) francesco  (1000)     6297 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/io/colmap_utils/flickr_downloader.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     5996 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/io/colmap_utils/h5_to_db.py
+-rwxrwxr-x   0 francesco  (1000) francesco  (1000)     2692 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/io/colmap_utils/merge_ply_files.py
+-rwxrwxr-x   0 francesco  (1000) francesco  (1000)     4743 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/io/colmap_utils/nvm_to_ply.py
+-rwxrwxr-x   0 francesco  (1000) francesco  (1000)    25506 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/io/colmap_utils/plyfile.py
+-rwxrwxr-x   0 francesco  (1000) francesco  (1000)     5172 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/io/colmap_utils/read_write_dense.py
+-rwxrwxr-x   0 francesco  (1000) francesco  (1000)     5230 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/io/colmap_utils/read_write_fused_vis.py
+-rwxrwxr-x   0 francesco  (1000) francesco  (1000)    22035 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/io/colmap_utils/read_write_model.py
+-rwxrwxr-x   0 francesco  (1000) francesco  (1000)     7069 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/io/colmap_utils/visualize_model.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     9057 2023-04-21 13:34:31.000000 icepy4d-1.6.2/src/icepy4d/io/export2bundler.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     2922 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/io/export2calge.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     4751 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/io/export2colmap.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     2995 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/io/export2textfile.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     1617 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/io/importing.py
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-25 16:21:23.907137 icepy4d-1.6.2/src/icepy4d/least_squares/
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)        0 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/least_squares/__init__.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     4184 2023-04-21 13:34:31.000000 icepy4d-1.6.2/src/icepy4d/least_squares/absolute_orientation.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     2845 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/least_squares/rototra3d.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     2761 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/least_squares/utils.py
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-25 16:21:23.907137 icepy4d-1.6.2/src/icepy4d/matching/
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)        0 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/matching/__init__.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    11728 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/matching/match_by_preselection.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    13660 2023-04-21 13:34:31.000000 icepy4d-1.6.2/src/icepy4d/matching/match_pairs.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     7602 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/matching/matching_base.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     1656 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/matching/retrieve_matches_from_npz.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     4096 2023-04-25 15:57:54.000000 icepy4d-1.6.2/src/icepy4d/matching/superglue_match_simple_old.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    14690 2023-04-21 13:34:31.000000 icepy4d-1.6.2/src/icepy4d/matching/superglue_matcher.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    13481 2023-04-25 15:57:54.000000 icepy4d-1.6.2/src/icepy4d/matching/superglue_tracker.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    15735 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/matching/templatematch.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    16743 2023-04-21 13:34:31.000000 icepy4d-1.6.2/src/icepy4d/matching/track_matches.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    18706 2023-04-21 13:34:31.000000 icepy4d-1.6.2/src/icepy4d/matching/track_matches_bk.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     3438 2023-04-21 13:34:31.000000 icepy4d-1.6.2/src/icepy4d/matching/tracking_base.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     5879 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/matching/utils.py
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-25 16:21:23.907137 icepy4d-1.6.2/src/icepy4d/metashape/
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)        0 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/metashape/__init__.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    20168 2023-04-25 16:04:33.000000 icepy4d-1.6.2/src/icepy4d/metashape/metashape.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    18623 2023-04-25 15:57:54.000000 icepy4d-1.6.2/src/icepy4d/metashape/metashape_core.py
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-25 16:21:23.907137 icepy4d-1.6.2/src/icepy4d/point_cloud_proc/
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)        0 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/point_cloud_proc/__init__.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     7242 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/point_cloud_proc/cloudcompare_fun.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    12502 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/point_cloud_proc/open3d_fun.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)      974 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/point_cloud_proc/utils.py
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-25 16:21:23.907137 icepy4d-1.6.2/src/icepy4d/sfm/
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)      218 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/sfm/__init__.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    10834 2023-04-21 13:34:31.000000 icepy4d-1.6.2/src/icepy4d/sfm/absolute_orientation.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     6506 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/sfm/geometry.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     4404 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/sfm/interpolate_colors.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     1333 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/sfm/reconstruction.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     6341 2023-04-21 13:34:31.000000 icepy4d-1.6.2/src/icepy4d/sfm/triangulation.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     8073 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/sfm/two_view_geometry.py
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-25 16:21:23.907137 icepy4d-1.6.2/src/icepy4d/thirdparty/
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-25 16:21:23.903137 icepy4d-1.6.2/src/icepy4d/thirdparty/SuperGlue/
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-25 16:21:23.911137 icepy4d-1.6.2/src/icepy4d/thirdparty/SuperGlue/models/
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)        0 2023-04-21 13:34:31.000000 icepy4d-1.6.2/src/icepy4d/thirdparty/SuperGlue/models/__init__.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     3419 2023-04-21 13:34:31.000000 icepy4d-1.6.2/src/icepy4d/thirdparty/SuperGlue/models/matching.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    11869 2023-04-21 13:34:31.000000 icepy4d-1.6.2/src/icepy4d/thirdparty/SuperGlue/models/superglue.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     8350 2023-04-21 13:34:31.000000 icepy4d-1.6.2/src/icepy4d/thirdparty/SuperGlue/models/superpoint.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    20648 2023-04-21 13:34:31.000000 icepy4d-1.6.2/src/icepy4d/thirdparty/SuperGlue/models/utils.py
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-25 16:21:23.911137 icepy4d-1.6.2/src/icepy4d/thirdparty/SuperGluePretrainedNetwork/
+-rwxrwxr-x   0 francesco  (1000) francesco  (1000)    10683 2023-03-31 12:00:43.000000 icepy4d-1.6.2/src/icepy4d/thirdparty/SuperGluePretrainedNetwork/demo_superglue.py
+-rwxrwxr-x   0 francesco  (1000) francesco  (1000)    18127 2023-03-31 12:00:43.000000 icepy4d-1.6.2/src/icepy4d/thirdparty/SuperGluePretrainedNetwork/match_pairs.py
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-25 16:21:23.911137 icepy4d-1.6.2/src/icepy4d/thirdparty/SuperGluePretrainedNetwork/models/
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)        0 2023-03-31 12:00:43.000000 icepy4d-1.6.2/src/icepy4d/thirdparty/SuperGluePretrainedNetwork/models/__init__.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     3417 2023-03-31 12:00:43.000000 icepy4d-1.6.2/src/icepy4d/thirdparty/SuperGluePretrainedNetwork/models/matching.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    11781 2023-03-31 12:00:43.000000 icepy4d-1.6.2/src/icepy4d/thirdparty/SuperGluePretrainedNetwork/models/superglue.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     8142 2023-03-31 12:00:43.000000 icepy4d-1.6.2/src/icepy4d/thirdparty/SuperGluePretrainedNetwork/models/superpoint.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    20039 2023-03-31 12:00:43.000000 icepy4d-1.6.2/src/icepy4d/thirdparty/SuperGluePretrainedNetwork/models/utils.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)        0 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/thirdparty/__init__.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    11815 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/thirdparty/templatematch_pyimgraft.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    67149 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/thirdparty/transformations.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    10133 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/thirdparty/triangulation.py
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-25 16:21:23.911137 icepy4d-1.6.2/src/icepy4d/utils/
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)      295 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/utils/__init__.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    13046 2023-04-21 13:34:31.000000 icepy4d-1.6.2/src/icepy4d/utils/binned_stats.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     7091 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/utils/dsm_orthophoto.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)      951 2023-04-21 13:34:31.000000 icepy4d-1.6.2/src/icepy4d/utils/homography.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    12345 2023-04-21 13:34:31.000000 icepy4d-1.6.2/src/icepy4d/utils/initialization.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     5957 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/utils/logger.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     3670 2023-04-21 13:34:31.000000 icepy4d-1.6.2/src/icepy4d/utils/math.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     1552 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/utils/sensor_width_database.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     3783 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/utils/spatial_funs.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     7325 2023-04-21 13:34:31.000000 icepy4d-1.6.2/src/icepy4d/utils/tiles.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     1662 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/utils/timer.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    16090 2023-04-21 13:34:31.000000 icepy4d-1.6.2/src/icepy4d/utils/tracking_features_utils.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     6354 2023-04-25 15:57:54.000000 icepy4d-1.6.2/src/icepy4d/utils/transformations.py
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-25 16:21:23.911137 icepy4d-1.6.2/src/icepy4d/visualization/
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)       29 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/visualization/__init__.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    27688 2023-04-20 09:18:56.000000 icepy4d-1.6.2/src/icepy4d/visualization/visualization.py
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-25 16:21:23.903137 icepy4d-1.6.2/src/icepy4d.egg-info/
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     4168 2023-04-25 16:21:23.000000 icepy4d-1.6.2/src/icepy4d.egg-info/PKG-INFO
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     4573 2023-04-25 16:21:23.000000 icepy4d-1.6.2/src/icepy4d.egg-info/SOURCES.txt
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)        1 2023-04-25 16:21:23.000000 icepy4d-1.6.2/src/icepy4d.egg-info/dependency_links.txt
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)      246 2023-04-25 16:21:23.000000 icepy4d-1.6.2/src/icepy4d.egg-info/requires.txt
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)        8 2023-04-25 16:21:23.000000 icepy4d-1.6.2/src/icepy4d.egg-info/top_level.txt
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-25 16:21:23.911137 icepy4d-1.6.2/tests/
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     8220 2023-04-20 09:18:56.000000 icepy4d-1.6.2/tests/test_features.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     1484 2023-04-20 09:18:56.000000 icepy4d-1.6.2/tests/test_image.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     2394 2023-04-20 09:18:56.000000 icepy4d-1.6.2/tests/test_initialization.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)      775 2023-04-20 09:18:56.000000 icepy4d-1.6.2/tests/test_matching.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     2032 2023-04-20 09:18:56.000000 icepy4d-1.6.2/tests/test_point_cloud.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     2742 2023-04-20 09:18:56.000000 icepy4d-1.6.2/tests/test_sfm_geometry.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)      518 2023-04-20 09:18:56.000000 icepy4d-1.6.2/tests/test_utils.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     1457 2023-04-20 09:18:56.000000 icepy4d-1.6.2/tests/test_utils_spatial.py
```

### Comparing `icepy4d-1.4.0/LICENSE.txt` & `icepy4d-1.6.2/src/icepy4d/classes/dsm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""
 MIT License
 
 Copyright (c) 2022 Francesco Ioli
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
@@ -15,7 +16,8 @@
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
+"""
```

### Comparing `icepy4d-1.4.0/PKG-INFO` & `icepy4d-1.6.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,33 +1,41 @@
 Metadata-Version: 2.1
 Name: icepy4d
-Version: 1.4.0
+Version: 1.6.2
 Summary: 4D Image-based Continuos monitoring of glaciers Evolution with low-cost stereo-cameras and Deep Learning photogrammetry.
 Author-email: Francesco Ioli <francesco.ioli@polimi.it>
-License: MIT License
+License: BSD 3-Clause License
         
-        Copyright (c) 2022 Francesco Ioli
+        Copyright (c) 2018, the respective contributors, as shown by the AUTHORS file.
+        All rights reserved.
         
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
+        Redistribution and use in source and binary forms, with or without
+        modification, are permitted provided that the following conditions are met:
+        
+        * Redistributions of source code must retain the above copyright notice, this
+          list of conditions and the following disclaimer.
+        
+        * Redistributions in binary form must reproduce the above copyright notice,
+          this list of conditions and the following disclaimer in the documentation
+          and/or other materials provided with the distribution.
+        
+        * Neither the name of the copyright holder nor the names of its
+          contributors may be used to endorse or promote products derived from
+          this software without specific prior written permission.
+        
+        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+        AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+        IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+        DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+        FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+        DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+        SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+        CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+        OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+        OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
         
 Project-URL: Homepage, https://github.com/franioli/icepy4d
 Keywords: sfm,4d-reconstruction,glaciers,deep-learning
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
@@ -37,84 +45,64 @@
 
 # Welcome to ICEpy4D
 
 4D Image-based Continuos monitoring of glaciers' Evolution with low-cost stereo-cameras and Deep Learning photogrammetry.
 
 `ICEpy4D` is a under active development.
 
-## Installation guide
-
-##### Requirements
+## Requirements
 
 - 64-bit Python `>= 3.8` but `< 3.10`
 - a NVIDIA graphic card with CUDA capability is strongly reccomended.
 
-##### Create Anaconda environment
-
-```bash
-conda create -n icepy4d python=3.8
-conda activate icepy4d
-```
-
-##### Install gdal for raster manipulation
-
-First, install `gdal`, which is required for building and manipulating orthophotos and DSMs. As the dependacies of `gdal`, are quite strict, it is suggested to install it first with conda. If you don't intend to build orthophotos and DSM, you can skip this step (be careful to remove rasterio from requirements.txt as well in order to avoid unsatisfied dependencies).
-
-```bash
-conda update -n base -c conda-forge conda
-conda install -c conda-forge gdal
-```
+## Installation guide
 
-Check that `gdal` is correctly installed with:
+Create a new Anaconda environment
 
 ```bash
-python -c "from osgeo import gdal"
+conda create -n icepy4d python=3.9
+conda activate icepy4d
 ```
 
-##### Install Pytorch
-
-Install pythorch following the official guidelines (<https://pytorch.org/get-started/locally/>). Be careful to select the correct CUDA version as that installed on your system.
+Install Icepy4D from PyPi repository
 
 ```bash
-pip3 install torch --extra-index-url https://download.pytorch.org/whl/cu116
-
+pip install icepy4d
 ```
 
-##### Install other required packages
+or install it from source by cloning the repository and installing it with `pip`
 
 ```bash
-pip3 install -r requirements.txt
+git clone https://github.com/franioli/icepy4d.git
+cd icepy4d
+pip install -e .
 ```
 
-##### Various
+In case of any error when installing `ICEpy4D` from PyPi, try to install it from source.
 
-- If you intend to use Jupyter Notebooks for running main scripts, install jupyterlab with
+Install Metashape Python API for Bundle Adjustment and Dense reconstruction.
+Metashape Python API can be downloaded from [https://www.agisoft.com/downloads/installer/](https://www.agisoft.com/downloads/installer/) or use `wget` (under Linux).
 
 ```bash
-pip3 install jupyterlab
+wget https://s3-eu-west-1.amazonaws.com/download.agisoft.com/Metashape-1.8.5-cp35.cp36.cp37.cp38-abi3-linux_x86_64.whl
+pip install Metashape-1.8.5-cp35.cp36.cp37.cp38-abi3-linux_x86_64.whl
 ```
 
-- When using VScode and Matplotlib, use TkAgg as interactive backend.
-
-##### Install ICEpy4D
-
-Install ICEpy4D package by running from the root folder
+You need to have a valid Metashape license to use the API and you need to activate it (see [https://github.com/franioli/metashape](https://github.com/franioli/metashape) for how to do it)
 
-```bash
-pip install -e .
-```
-
-and try to import it
+Try to import ICEpy4D package
 
 ```bash
 conda activate icepy4d
 python -c "import icepy4d"
 ```
 
-If no error is given, ICEpy4D is successfully installed and it can be imported with `import icepy4d`
+If no error is given, ICEpy4D is successfully installed and it can be imported within your script with `import icepy4d`
 
+### For contributing
 
-#### For contributing
-`bash
+Install additional requirements for development:
+
+```bash
 pip install -r requirements-dev.txt
 pre-commit install
-`
+```
```

### Comparing `icepy4d-1.4.0/README.md` & `icepy4d-1.6.2/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,83 +1,63 @@
 # Welcome to ICEpy4D
 
 4D Image-based Continuos monitoring of glaciers' Evolution with low-cost stereo-cameras and Deep Learning photogrammetry.
 
 `ICEpy4D` is a under active development.
 
-## Installation guide
-
-##### Requirements
+## Requirements
 
 - 64-bit Python `>= 3.8` but `< 3.10`
 - a NVIDIA graphic card with CUDA capability is strongly reccomended.
 
-##### Create Anaconda environment
-
-```bash
-conda create -n icepy4d python=3.8
-conda activate icepy4d
-```
-
-##### Install gdal for raster manipulation
+## Installation guide
 
-First, install `gdal`, which is required for building and manipulating orthophotos and DSMs. As the dependacies of `gdal`, are quite strict, it is suggested to install it first with conda. If you don't intend to build orthophotos and DSM, you can skip this step (be careful to remove rasterio from requirements.txt as well in order to avoid unsatisfied dependencies).
+Create a new Anaconda environment
 
 ```bash
-conda update -n base -c conda-forge conda
-conda install -c conda-forge gdal
+conda create -n icepy4d python=3.9
+conda activate icepy4d
 ```
 
-Check that `gdal` is correctly installed with:
+Install Icepy4D from PyPi repository
 
 ```bash
-python -c "from osgeo import gdal"
+pip install icepy4d
 ```
 
-##### Install Pytorch
-
-Install pythorch following the official guidelines (<https://pytorch.org/get-started/locally/>). Be careful to select the correct CUDA version as that installed on your system.
+or install it from source by cloning the repository and installing it with `pip`
 
 ```bash
-pip3 install torch --extra-index-url https://download.pytorch.org/whl/cu116
-
-```
-
-##### Install other required packages
-
-```bash
-pip3 install -r requirements.txt
+git clone https://github.com/franioli/icepy4d.git
+cd icepy4d
+pip install -e .
 ```
 
-##### Various
+In case of any error when installing `ICEpy4D` from PyPi, try to install it from source.
 
-- If you intend to use Jupyter Notebooks for running main scripts, install jupyterlab with
+Install Metashape Python API for Bundle Adjustment and Dense reconstruction.
+Metashape Python API can be downloaded from [https://www.agisoft.com/downloads/installer/](https://www.agisoft.com/downloads/installer/) or use `wget` (under Linux).
 
 ```bash
-pip3 install jupyterlab
+wget https://s3-eu-west-1.amazonaws.com/download.agisoft.com/Metashape-1.8.5-cp35.cp36.cp37.cp38-abi3-linux_x86_64.whl
+pip install Metashape-1.8.5-cp35.cp36.cp37.cp38-abi3-linux_x86_64.whl
 ```
 
-- When using VScode and Matplotlib, use TkAgg as interactive backend.
-
-##### Install ICEpy4D
-
-Install ICEpy4D package by running from the root folder
-
-```bash
-pip install -e .
-```
+You need to have a valid Metashape license to use the API and you need to activate it (see [https://github.com/franioli/metashape](https://github.com/franioli/metashape) for how to do it)
 
-and try to import it
+Try to import ICEpy4D package
 
 ```bash
 conda activate icepy4d
 python -c "import icepy4d"
 ```
 
-If no error is given, ICEpy4D is successfully installed and it can be imported with `import icepy4d`
+If no error is given, ICEpy4D is successfully installed and it can be imported within your script with `import icepy4d`
 
+### For contributing
 
-#### For contributing
-`bash
+Install additional requirements for development:
+
+```bash
 pip install -r requirements-dev.txt
 pre-commit install
-`
+```
```

### Comparing `icepy4d-1.4.0/pyproject.toml` & `icepy4d-1.6.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=65", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "icepy4d"
-version = "1.4.0"
+version = "1.6.2"
 description = "4D Image-based Continuos monitoring of glaciers Evolution with low-cost stereo-cameras and Deep Learning photogrammetry."
 readme = "README.md"
 authors = [{ name = "Francesco Ioli", email = "francesco.ioli@polimi.it" }]
 license = { file = "LICENSE.txt" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -45,15 +45,15 @@
 addopts = [
     "--import-mode=importlib",
 ]
 
 [tool.isort]
 profile = "black"
 [tool.bumpver]
-current_version = "1.4.0"
+current_version = "1.6.2"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `icepy4d-1.4.0/src/icepy4d/binned_stats.py` & `icepy4d-1.6.2/src/icepy4d/utils/binned_stats.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/classes/camera.py` & `icepy4d-1.6.2/src/icepy4d/classes/camera.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/classes/dsm.py` & `icepy4d-1.6.2/src/icepy4d/classes/epoch.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/classes/epoch.py` & `icepy4d-1.6.2/src/icepy4d/classes/ortophoto.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/classes/features.py` & `icepy4d-1.6.2/src/icepy4d/classes/features.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/classes/images.py` & `icepy4d-1.6.2/src/icepy4d/classes/images.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/classes/point_cloud.py` & `icepy4d-1.6.2/src/icepy4d/classes/point_cloud.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/classes/points.py` & `icepy4d-1.6.2/src/icepy4d/classes/points.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/classes/solution.py` & `icepy4d-1.6.2/src/icepy4d/classes/solution.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/classes/targets.py` & `icepy4d-1.6.2/src/icepy4d/classes/targets.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/classes/typed_dict_classes.py` & `icepy4d-1.6.2/src/icepy4d/classes/typed_dict_classes.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/io/colmap_utils/build.py` & `icepy4d-1.6.2/src/icepy4d/io/colmap_utils/build.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/io/colmap_utils/build_windows_app.py` & `icepy4d-1.6.2/src/icepy4d/io/colmap_utils/build_windows_app.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/io/colmap_utils/bundler_to_ply.py` & `icepy4d-1.6.2/src/icepy4d/io/colmap_utils/bundler_to_ply.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/io/colmap_utils/clang_format_code.py` & `icepy4d-1.6.2/src/icepy4d/io/colmap_utils/clang_format_code.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/io/colmap_utils/crawl_camera_specs.py` & `icepy4d-1.6.2/src/icepy4d/io/colmap_utils/crawl_camera_specs.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/io/colmap_utils/database.py` & `icepy4d-1.6.2/src/icepy4d/io/colmap_utils/database.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/io/colmap_utils/export_inlier_matches.py` & `icepy4d-1.6.2/src/icepy4d/io/colmap_utils/export_inlier_matches.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/io/colmap_utils/export_inlier_pairs.py` & `icepy4d-1.6.2/src/icepy4d/io/colmap_utils/export_inlier_pairs.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/io/colmap_utils/export_to_bundler.py` & `icepy4d-1.6.2/src/icepy4d/io/colmap_utils/export_to_bundler.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/io/colmap_utils/export_to_visualsfm.py` & `icepy4d-1.6.2/src/icepy4d/io/colmap_utils/export_to_visualsfm.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/io/colmap_utils/flickr_downloader.py` & `icepy4d-1.6.2/src/icepy4d/io/colmap_utils/flickr_downloader.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/io/colmap_utils/h5_to_db.py` & `icepy4d-1.6.2/src/icepy4d/io/colmap_utils/h5_to_db.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/io/colmap_utils/merge_ply_files.py` & `icepy4d-1.6.2/src/icepy4d/io/colmap_utils/merge_ply_files.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/io/colmap_utils/nvm_to_ply.py` & `icepy4d-1.6.2/src/icepy4d/io/colmap_utils/nvm_to_ply.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/io/colmap_utils/plyfile.py` & `icepy4d-1.6.2/src/icepy4d/io/colmap_utils/plyfile.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/io/colmap_utils/read_write_dense.py` & `icepy4d-1.6.2/src/icepy4d/io/colmap_utils/read_write_dense.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/io/colmap_utils/read_write_fused_vis.py` & `icepy4d-1.6.2/src/icepy4d/io/colmap_utils/read_write_fused_vis.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/io/colmap_utils/read_write_model.py` & `icepy4d-1.6.2/src/icepy4d/io/colmap_utils/read_write_model.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/io/colmap_utils/visualize_model.py` & `icepy4d-1.6.2/src/icepy4d/io/colmap_utils/visualize_model.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/io/export2bundler.py` & `icepy4d-1.6.2/src/icepy4d/io/export2bundler.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,18 +8,26 @@
 from typing import Union, List
 
 from ..classes.point_cloud import PointCloud
 from ..classes.points import Points
 from ..classes.targets import Targets
 from ..classes.typed_dict_classes import FeaturesDictEpoch, CamerasDictEpoch
 
-from ..utils.utils import create_directory
 from ..thirdparty.transformations import euler_from_matrix, euler_matrix
 
 
+def create_directory(path):
+    """
+    Creates a directory, if it does not exist.
+    """
+    path = Path(path)
+    path.mkdir(parents=True, exist_ok=True)
+    return path
+
+
 def write_bundler_out(
     export_dir: Union[str, Path],
     im_dict: dict,
     cameras: CamerasDictEpoch,
     features: FeaturesDictEpoch,
     points: Points,
     targets: Targets = None,
```

### Comparing `icepy4d-1.4.0/src/icepy4d/io/export2calge.py` & `icepy4d-1.6.2/src/icepy4d/io/export2calge.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/io/export2colmap.py` & `icepy4d-1.6.2/src/icepy4d/io/export2colmap.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/io/export2textfile.py` & `icepy4d-1.6.2/src/icepy4d/io/export2textfile.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/io/importing.py` & `icepy4d-1.6.2/src/icepy4d/io/importing.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/least_squares/rototra3d.py` & `icepy4d-1.6.2/src/icepy4d/least_squares/rototra3d.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/least_squares/utils.py` & `icepy4d-1.6.2/src/icepy4d/least_squares/utils.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/matching/match_by_preselection.py` & `icepy4d-1.6.2/src/icepy4d/matching/match_by_preselection.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/matching/match_pairs.py` & `icepy4d-1.6.2/src/icepy4d/matching/match_pairs.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,23 @@
-import numpy as np
-import matplotlib.cm as cm
-import torch
-import cv2
 import logging
-
 from pathlib import Path
 
-from icepy4d.utils import AverageTimer
+import cv2
+import matplotlib.cm as cm
+import numpy as np
+import torch
 
-from ..thirdparty.SuperGluePretrainedNetwork.models.matching import Matching
-from ..thirdparty.SuperGluePretrainedNetwork.models.utils import (
-    make_matching_plot,
+from icepy4d.thirdparty.SuperGlue.models.matching import Matching
+from icepy4d.thirdparty.SuperGlue.models.utils import (
     frame2tensor,
+    make_matching_plot,
     process_resize,
 )
-
-from ..tiles import generateTiles
-
+from icepy4d.utils import AverageTimer
+from icepy4d.utils.tiles import generateTiles
 
 torch.set_grad_enabled(False)
 
 # SuperPoint Parameters
 NMS_RADIUS = 3
 
 # SuperGlue Parameters
@@ -29,14 +26,15 @@
 # Processing parameters
 RESIZE_FLOAT = True
 VIZ_EXTENSION = "png"
 OPENCV_DISPLAY = False
 SHOW_KEYPOINTS = False
 CACHE = False
 
+
 # @TODO: This function is a duplicate of the one in track_matches!!!
 # It is a replacement of the SuperGlue one because of the different input parametets.
 # This must be fixed! Only ONE read_image function must exist!
 # (There is also read_image function implemented from scratch in icepy4d)
 def read_image(path, device, resize=-1, rotation=0, resize_float=True, crop=[]):
     image = cv2.imread(str(path), cv2.IMREAD_GRAYSCALE)
     if image is None:
@@ -58,15 +56,14 @@
         image = image[crop[1] : crop[3], crop[0] : crop[2]]
 
     inp = frame2tensor(image, device)
     return image, inp, scales
 
 
 def vizTileRes(viz_path, pred, image0, image1, matching, timer, opt):
-
     kpts0, kpts1 = pred["keypoints0"], pred["keypoints1"]
     matches0 = pred["matches0"]
     conf = pred["matching_scores0"]
 
     # Keep the matching keypoints and descriptors.
     valid = matches0 > -1
     mkpts0 = kpts0[valid]
@@ -107,15 +104,14 @@
         small_text,
     )
 
     timer.update("viz_match")
 
 
 def match_pair(pair, maskBB, opt):
-
     opt.resize_float = RESIZE_FLOAT
     opt.viz_extension = VIZ_EXTENSION
     opt.opencv_display = OPENCV_DISPLAY
     opt.show_keypoints = SHOW_KEYPOINTS
     opt.cache = CACHE
 
     assert not (
@@ -181,15 +177,14 @@
     )
     if image0 is None or image1 is None:
         logging.error("Problem reading image pair: {} {}".format(name0, name1))
         exit(1)
     timer.update("load_image")
 
     if opt.useTile:
-
         # Subdivide image in tiles and run a loop
         tiles0, limits0 = generateTiles(
             image0,
             rowDivisor=opt.rowDivisor,
             colDivisor=opt.colDivisor,
             overlap=opt.overlap,
             viz=opt.do_viz_tile,
```

### Comparing `icepy4d-1.4.0/src/icepy4d/matching/matching_base.py` & `icepy4d-1.6.2/src/icepy4d/matching/matching_base.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/matching/retrieve_matches_from_npz.py` & `icepy4d-1.6.2/src/icepy4d/matching/retrieve_matches_from_npz.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/matching/superglue_match_simple_old.py` & `icepy4d-1.6.2/src/icepy4d/matching/superglue_match_simple_old.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 from pathlib import Path
 import numpy as np
 import matplotlib.cm as cm
 import torch
 import json
 
-from ..thirdparty.SuperGluePretrainedNetwork.models.matching import Matching
-from ..thirdparty.SuperGluePretrainedNetwork.models.utils import (
+from icepy4d.thirdparty.SuperGlue.models.matching import Matching
+from icepy4d.thirdparty.SuperGlue.models.utils import (
     make_matching_plot,
     AverageTimer,
     read_image,
     frame2tensor,
     vizTileRes,
 )
 
 torch.set_grad_enabled(False)
 
 
 def match_pair(pair, image0, image1, maskBB, opt):
-
     # @TODO: implement all checks...
 
     # Parameters
     do_viz = opt["viz"]
 
     # Load the SuperPoint and SuperGlue models.
     device = "cuda" if torch.cuda.is_available() and not opt["force_cpu"] else "cpu"
```

### Comparing `icepy4d-1.4.0/src/icepy4d/matching/superglue_matcher.py` & `icepy4d-1.6.2/src/icepy4d/matching/superglue_matcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,18 +14,18 @@
 import importlib
 
 from easydict import EasyDict as edict
 from pathlib import Path
 
 from icepy4d.utils import AverageTimer
 
-from icepy4d.thirdparty.SuperGluePretrainedNetwork.models.superpoint import SuperPoint
-from icepy4d.thirdparty.SuperGluePretrainedNetwork.models.superglue import SuperGlue
-from icepy4d.thirdparty.SuperGluePretrainedNetwork.models.matching import Matching
-from icepy4d.thirdparty.SuperGluePretrainedNetwork.models.utils import (
+from icepy4d.thirdparty.SuperGlue.models.superpoint import SuperPoint
+from icepy4d.thirdparty.SuperGlue.models.superglue import SuperGlue
+from icepy4d.thirdparty.SuperGlue.models.matching import Matching
+from icepy4d.thirdparty.SuperGlue.models.utils import (
     make_matching_plot,
 )
 
 
 # SuperPoint Parameters
 NMS_RADIUS = 3
```

### Comparing `icepy4d-1.4.0/src/icepy4d/matching/superglue_tracker.py` & `icepy4d-1.6.2/src/icepy4d/matching/superglue_tracker.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,43 +2,34 @@
 The network was proposed in 'SuperGlue: Learning Feature Matching with Graph Neural Networks' and is implemented by wrapping over author's source-code.
 Note: the pretrained model only supports SuperPoint detections currently.
 References:
 - http://openaccess.thecvf.com/content_CVPR_2020/papers/Sarlin_SuperGlue_Learning_Feature_Matching_With_Graph_Neural_Networks_CVPR_2020_paper.pdf
 - https://github.com/magicleap/SuperGluePretrainedNetwork
 """
 
-import numpy as np
-import matplotlib.cm as cm
-import torch
-import logging
-import cv2
 import importlib
-
-from easydict import EasyDict as edict
+import logging
 from pathlib import Path
-from typing import Tuple, Union
-
-
-from ..classes.features import Features
-from ..classes.images import ImageDS
-from ..utils.initialization import parse_yaml_cfg
-from ..tiles import generateTiles
 
+import cv2
+import matplotlib.cm as cm
+import numpy as np
+import torch
+from easydict import EasyDict as edict
 
-from icepy4d.matching.utils import read_image, frame2tensor
+from icepy4d.classes.features import Features
+from icepy4d.classes.images import ImageDS
+from icepy4d.matching.utils import frame2tensor, read_image
+from icepy4d.thirdparty.SuperGlue.models.matching import Matching
+from icepy4d.thirdparty.SuperGlue.models.superglue import SuperGlue
+from icepy4d.thirdparty.SuperGlue.models.superpoint import SuperPoint
+from icepy4d.thirdparty.SuperGlue.models.utils import make_matching_plot
 from icepy4d.utils import AverageTimer
-
-
-from icepy4d.thirdparty.SuperGluePretrainedNetwork.models.superpoint import SuperPoint
-from icepy4d.thirdparty.SuperGluePretrainedNetwork.models.superglue import SuperGlue
-from icepy4d.thirdparty.SuperGluePretrainedNetwork.models.matching import Matching
-from icepy4d.thirdparty.SuperGluePretrainedNetwork.models.utils import (
-    make_matching_plot,
-)
-
+from icepy4d.utils.initialization import parse_yaml_cfg
+from icepy4d.utils.tiles import generateTiles
 
 # SuperPoint Parameters
 NMS_RADIUS = 3
 
 # SuperGlue Parameters
 SUPERGLUE_DESC_DIM = 256
 SINKHORN_ITERATIONS = 20
@@ -337,15 +328,14 @@
         #     }
         # )
 
         # return features
 
 
 if __name__ == "__main__":
-
     cfg_file = "config/config_base.yaml"
     cfg = parse_yaml_cfg(cfg_file)
 
     cams = cfg.paths.camera_names
 
     # Create Image Datastore objects
     images = dict.fromkeys(cams)
```

### Comparing `icepy4d-1.4.0/src/icepy4d/matching/templatematch.py` & `icepy4d-1.6.2/src/icepy4d/matching/templatematch.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/matching/track_matches.py` & `icepy4d-1.6.2/src/icepy4d/matching/track_matches.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 from pathlib import Path
 import numpy as np
 import matplotlib.cm as cm
 import torch
 import cv2
 import logging
 
-from ..thirdparty.SuperGluePretrainedNetwork.models.matching import Matching
-from ..thirdparty.SuperGluePretrainedNetwork.models.utils import (
+from icepy4d.thirdparty.SuperGlue.models.matching import Matching
+from icepy4d.thirdparty.SuperGlue.models.utils import (
     make_matching_plot,
     AverageTimer,
     process_resize,
     frame2tensor,
 )
-from ..tiles import generateTiles
-from ..utils.spatial_funs import point_in_rect
-
-from icepy4d import visualization
+from icepy4d.utils.tiles import generateTiles
+from icepy4d.utils.spatial_funs import point_in_rect
 
 torch.set_grad_enabled(False)
 
 # SuperPoint Parameters
 NMS_RADIUS = 3
 
 # SuperGlue Parameters
```

### Comparing `icepy4d-1.4.0/src/icepy4d/matching/track_matches_bk.py` & `icepy4d-1.6.2/src/icepy4d/matching/track_matches_bk.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from pathlib import Path
 import numpy as np
 import matplotlib.cm as cm
 import torch
 import cv2
 import logging
 
-from ..thirdparty.SuperGluePretrainedNetwork.models.matching import Matching
-from ..thirdparty.SuperGluePretrainedNetwork.models.utils import (
+from ..thirdparty.SuperGlue.models.matching import Matching
+from ..thirdparty.SuperGlue.models.utils import (
     make_matching_plot,
     AverageTimer,
     process_resize,
     frame2tensor,
 )
 from ..tiles import generateTiles
```

### Comparing `icepy4d-1.4.0/src/icepy4d/matching/tracking_base.py` & `icepy4d-1.6.2/src/icepy4d/matching/tracking_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,14 @@
     prev_features: icepy4d_classes.FeaturesDictEpoch,
     camera_names: List[str],
     epoch_dict: icepy4d_classes.EpochDict,
     epoch: int,
     cfg: edict,
     epoch_dir: Union[Path, str],
 ) -> icepy4d_classes.FeaturesDictEpoch:
-
     if not isinstance(cfg, dict):
         raise TypeError("opt must be a dictionary")
     required_keys = [
         "weights",
         "keypoint_threshold",
         "max_keypoints",
         "match_threshold",
@@ -62,15 +61,14 @@
     )
     prev_path = epoch_dir.parent / f"{epoch_dict[epoch-1]}/matching"
     fname = list(prev_path.glob("*.pickle"))
     try:
         with open(fname[0], "rb") as f:
             prev_features = pickle.load(f)
             logging.info("Previous features loaded.")
-
     except:
         raise FileNotFoundError(
             f"Invalid pickle file in {prev_path}. Skipping tracking from epoch {epoch_dict[epoch-1]} to {epoch_dict[epoch]}"
         )
 
     prevs = [prev_features[cam].get_features_as_dict() for cam in cams]
     prev_track_id = prev_features[cams[0]].get_track_ids()
```

### Comparing `icepy4d-1.4.0/src/icepy4d/matching/utils.py` & `icepy4d-1.6.2/src/icepy4d/matching/utils.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/metashape/metashape.py` & `icepy4d-1.6.2/src/icepy4d/metashape/metashape.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,53 +28,53 @@
 import logging
 
 from pathlib import Path
 from easydict import EasyDict as edict
 from xml.etree import ElementTree as ET
 from typing import List, Union
 
-from .ms_utils import (
+from .metashape_core import (
     create_new_project,
     save_project,
     cameras_from_bundler,
     add_markers,
     read_gcp_file,
 )
-from ..utils.timer import AverageTimer
-from ..io.importing import read_opencv_calibration
+from icepy4d.utils.timer import AverageTimer
+from icepy4d.io.importing import read_opencv_calibration
 
 REGION_RESIZE_FCT = 10.0
 
 
-def build_metashape_cfg(cfg: edict, epoch_dict: dict, epoch: int) -> edict:
+def build_metashape_cfg(cfg: edict, epoch_dict: dict, cur_epoch: int) -> edict:
     """
     # build_metashape_cfg Build metashape configuration dictionary, starting from global configuration dictionary.
 
     Args:
         cfg (edict): configuration dictionary for icepy4d
         epoch_dict (dict): dictionary containing the correspondings between epoch progressive numbers and dates
-        epoch (int): current epoch.
+        cur_epoch (int): current cur_epoch.
 
     Returns:
         edict: Metashape configuration dictionary
     """
     ms_cfg = edict()
 
     # Paths
-    ms_cfg.dir = cfg.paths.results_dir / f"{epoch_dict[epoch]}/metashape"
-    ms_cfg.project_path = ms_cfg.dir / f"{epoch_dict[epoch]}.psx"
+    ms_cfg.dir = cfg.paths.results_dir / f"{epoch_dict[cur_epoch]}/metashape"
+    ms_cfg.project_path = ms_cfg.dir / f"{epoch_dict[cur_epoch]}.psx"
     ms_cfg.im_path = ms_cfg.dir / "data/images"
     ms_cfg.im_ext = cfg.paths.image_extension
-    ms_cfg.bundler_file_path = ms_cfg.dir / f"data/{epoch_dict[epoch]}.out"
+    ms_cfg.bundler_file_path = ms_cfg.dir / f"data/{epoch_dict[cur_epoch]}.out"
     ms_cfg.bundler_im_list = ms_cfg.dir / "data/im_list.txt"
     ms_cfg.gcp_filename = ms_cfg.dir / "data/gcps.txt"
     ms_cfg.calib_filenames = cfg.metashape.calib_filenames
     ms_cfg.dense_path = cfg.paths.results_dir / "point_clouds"
-    ms_cfg.dense_name = f"dense_{epoch_dict[epoch]}.ply"
-    ms_cfg.mesh_name = f"mesh_{epoch_dict[epoch]}.ply"
+    ms_cfg.dense_name = f"dense_{epoch_dict[cur_epoch]}.ply"
+    ms_cfg.mesh_name = f"mesh_{epoch_dict[cur_epoch]}.ply"
 
     # Processing parameters
     ms_cfg.optimize_cameras = cfg.metashape.optimize_cameras
     ms_cfg.build_dense = cfg.metashape.build_dense
     ms_cfg.build_mesh = cfg.metashape.build_mesh
 
     # Camera location
@@ -101,15 +101,14 @@
 
 class MetashapeProject:
     def __init__(
         self,
         cfg: edict,
         timer: AverageTimer = None,
     ) -> None:
-
         self.cfg = cfg
         self.timer = timer
 
     @property
     def project_path(self) -> str:
         return str(self.cfg.project_path.name)
 
@@ -496,15 +495,14 @@
 
     def read_icepy4d_outputs(self) -> None:
         self.read_calibration_from_file()
         self.read_cameras_extrinsics()
 
 
 if __name__ == "__main__":
-
     from src.icepy4d.visualization.visualization import make_focal_length_variation_plot
 
     root_path = Path().absolute()
 
     # Process data
     # epoches_2_process = range(1)
     # for epoch in epoches_2_process:
```

### Comparing `icepy4d-1.4.0/src/icepy4d/metashape/ms_utils.py` & `icepy4d-1.6.2/src/icepy4d/metashape/metashape_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,14 @@
 
 
 def create_new_project(
     project_name: str,
     chunk_name: str = None,
     read_only: bool = False,
 ) -> Metashape.app.document:
-
     doc = Metashape.Document()
     doc.read_only = read_only
     create_new_chunk(doc, chunk_name)
     save_project(doc, project_name)
 
     return doc
 
@@ -325,15 +324,14 @@
     chunk: Metashape.Chunk,
     X: np.ndarray,
     projections: dict,
     label: str = None,
     enabled: bool = True,
     accuracy: Union[float, np.ndarray] = None,
 ) -> None:
-
     # Create Markers given its 3D object coordinates
     X = Metashape.Vector(X)
     X_ = chunk.transform.matrix.inv().mulp(X)
     marker = chunk.addMarker(X_)
 
     # Add projections on images given image coordinates in a  dictionary, as  {im_name: (x,y)}
     for k, v in projections.items():
@@ -538,15 +536,14 @@
 
 
 def copy_camera_estimated_to_reference(
     chunk: Metashape.Chunk,
     copy_rotations: bool = False,
     accuracy: List[float] = None,
 ) -> None:
-
     # Get Chunk transformation matrix
     T = chunk.transform.matrix
 
     if len(accuracy) == 1:
         accuracy = Metashape.Vector((accuracy, accuracy, accuracy))
     elif len(accuracy) != 3:
         logging.error(
@@ -578,15 +575,14 @@
 
 """ MISCELLANEOUS """
 
 
 def make_homogeneous(
     v: Metashape.Vector,
 ) -> Metashape.Vector:
-
     vh = Metashape.Vector([1.0 for x in range(v.size + 1)])
     for i, x in enumerate(v):
         vh[i] = x
 
     return vh
```

### Comparing `icepy4d-1.4.0/src/icepy4d/point_cloud_proc/cloudcompare_fun.py` & `icepy4d-1.6.2/src/icepy4d/point_cloud_proc/cloudcompare_fun.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/point_cloud_proc/open3d_fun.py` & `icepy4d-1.6.2/src/icepy4d/point_cloud_proc/open3d_fun.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/point_cloud_proc/utils.py` & `icepy4d-1.6.2/src/icepy4d/point_cloud_proc/utils.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/sfm/geometry.py` & `icepy4d-1.6.2/src/icepy4d/sfm/geometry.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/sfm/interpolate_colors.py` & `icepy4d-1.6.2/src/icepy4d/sfm/interpolate_colors.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/sfm/reconstruction.py` & `icepy4d-1.6.2/src/icepy4d/sfm/reconstruction.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/sfm/triangulation.py` & `icepy4d-1.6.2/src/icepy4d/sfm/triangulation.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 import logging
 
 from typing import List
 
 from .geometry import undistort_points
 from .interpolate_colors import interpolate_point_colors
 from ..classes.camera import Camera
-from ..utils.utils import (
+from ..utils.math import (
     convert_from_homogeneous,
     convert_to_homogeneous,
 )
 from ..thirdparty.triangulation import iterative_LS_triangulation
 
 """ Triangulation class """
```

### Comparing `icepy4d-1.4.0/src/icepy4d/sfm/two_view_geometry.py` & `icepy4d-1.6.2/src/icepy4d/sfm/two_view_geometry.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/thirdparty/SuperGluePretrainedNetwork/demo_superglue.py` & `icepy4d-1.6.2/src/icepy4d/thirdparty/SuperGluePretrainedNetwork/demo_superglue.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/thirdparty/SuperGluePretrainedNetwork/match_pairs.py` & `icepy4d-1.6.2/src/icepy4d/thirdparty/SuperGluePretrainedNetwork/match_pairs.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/thirdparty/SuperGluePretrainedNetwork/models/matching.py` & `icepy4d-1.6.2/src/icepy4d/thirdparty/SuperGluePretrainedNetwork/models/matching.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/thirdparty/SuperGluePretrainedNetwork/models/superglue.py` & `icepy4d-1.6.2/src/icepy4d/thirdparty/SuperGluePretrainedNetwork/models/superglue.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/thirdparty/SuperGluePretrainedNetwork/models/superpoint.py` & `icepy4d-1.6.2/src/icepy4d/thirdparty/SuperGluePretrainedNetwork/models/superpoint.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/thirdparty/SuperGluePretrainedNetwork/models/utils.py` & `icepy4d-1.6.2/src/icepy4d/thirdparty/SuperGluePretrainedNetwork/models/utils.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/thirdparty/templatematch_pyimgraft.py` & `icepy4d-1.6.2/src/icepy4d/thirdparty/templatematch_pyimgraft.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/thirdparty/transformations.py` & `icepy4d-1.6.2/src/icepy4d/thirdparty/transformations.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/thirdparty/triangulation.py` & `icepy4d-1.6.2/src/icepy4d/thirdparty/triangulation.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/tiles.py` & `icepy4d-1.6.2/src/icepy4d/utils/tiles.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/tracking_features_utils.py` & `icepy4d-1.6.2/src/icepy4d/utils/tracking_features_utils.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/utils/dsm_orthophoto.py` & `icepy4d-1.6.2/src/icepy4d/utils/dsm_orthophoto.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/utils/initialization.py` & `icepy4d-1.6.2/src/icepy4d/utils/initialization.py`

 * *Files 2% similar despite different names*

```diff
@@ -219,14 +219,20 @@
 
     Args:
         cfg (edict): A dictionary-like object containing the configuration parameters.
     """
     pprint(dict(cfg), indent=2)
 
 
+def download_model():
+    """
+    Download the model from the internet.
+    """
+
+
 class Inizializer:
     def __init__(
         self,
         cfg: edict,
     ) -> None:
         """
         __init__ initialization class
```

### Comparing `icepy4d-1.4.0/src/icepy4d/utils/logger.py` & `icepy4d-1.6.2/src/icepy4d/utils/logger.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/utils/rototranslation.py` & `icepy4d-1.6.2/src/icepy4d/utils/transformations.py`

 * *Files 0% similar despite different names*

```diff
@@ -166,12 +166,11 @@
         with open(fname, "w") as f:
             for row in self.T:
                 string = f"{sep}".join([f"{x}" for x in row])
                 f.write(f"{string}\n")
 
 
 if __name__ == "__main__":
-
     belv_rotra = Rotrotranslation(belvedere_loc2utm())
     # a = Rotrotranslation.read_T_from_file("scripts/rototranslation/BELV_LOC2UTM.txt")
 
     print("done")
```

### Comparing `icepy4d-1.4.0/src/icepy4d/utils/sensor_width_database.py` & `icepy4d-1.6.2/src/icepy4d/utils/sensor_width_database.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/utils/spatial_funs.py` & `icepy4d-1.6.2/src/icepy4d/utils/spatial_funs.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/utils/timer.py` & `icepy4d-1.6.2/src/icepy4d/utils/timer.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/visualization/visualization.py` & `icepy4d-1.6.2/src/icepy4d/visualization/visualization.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d.egg-info/PKG-INFO` & `icepy4d-1.6.2/src/icepy4d.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,33 +1,41 @@
 Metadata-Version: 2.1
 Name: icepy4d
-Version: 1.4.0
+Version: 1.6.2
 Summary: 4D Image-based Continuos monitoring of glaciers Evolution with low-cost stereo-cameras and Deep Learning photogrammetry.
 Author-email: Francesco Ioli <francesco.ioli@polimi.it>
-License: MIT License
+License: BSD 3-Clause License
         
-        Copyright (c) 2022 Francesco Ioli
+        Copyright (c) 2018, the respective contributors, as shown by the AUTHORS file.
+        All rights reserved.
         
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
+        Redistribution and use in source and binary forms, with or without
+        modification, are permitted provided that the following conditions are met:
+        
+        * Redistributions of source code must retain the above copyright notice, this
+          list of conditions and the following disclaimer.
+        
+        * Redistributions in binary form must reproduce the above copyright notice,
+          this list of conditions and the following disclaimer in the documentation
+          and/or other materials provided with the distribution.
+        
+        * Neither the name of the copyright holder nor the names of its
+          contributors may be used to endorse or promote products derived from
+          this software without specific prior written permission.
+        
+        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+        AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+        IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+        DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+        FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+        DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+        SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+        CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+        OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+        OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
         
 Project-URL: Homepage, https://github.com/franioli/icepy4d
 Keywords: sfm,4d-reconstruction,glaciers,deep-learning
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
@@ -37,84 +45,64 @@
 
 # Welcome to ICEpy4D
 
 4D Image-based Continuos monitoring of glaciers' Evolution with low-cost stereo-cameras and Deep Learning photogrammetry.
 
 `ICEpy4D` is a under active development.
 
-## Installation guide
-
-##### Requirements
+## Requirements
 
 - 64-bit Python `>= 3.8` but `< 3.10`
 - a NVIDIA graphic card with CUDA capability is strongly reccomended.
 
-##### Create Anaconda environment
-
-```bash
-conda create -n icepy4d python=3.8
-conda activate icepy4d
-```
-
-##### Install gdal for raster manipulation
-
-First, install `gdal`, which is required for building and manipulating orthophotos and DSMs. As the dependacies of `gdal`, are quite strict, it is suggested to install it first with conda. If you don't intend to build orthophotos and DSM, you can skip this step (be careful to remove rasterio from requirements.txt as well in order to avoid unsatisfied dependencies).
-
-```bash
-conda update -n base -c conda-forge conda
-conda install -c conda-forge gdal
-```
+## Installation guide
 
-Check that `gdal` is correctly installed with:
+Create a new Anaconda environment
 
 ```bash
-python -c "from osgeo import gdal"
+conda create -n icepy4d python=3.9
+conda activate icepy4d
 ```
 
-##### Install Pytorch
-
-Install pythorch following the official guidelines (<https://pytorch.org/get-started/locally/>). Be careful to select the correct CUDA version as that installed on your system.
+Install Icepy4D from PyPi repository
 
 ```bash
-pip3 install torch --extra-index-url https://download.pytorch.org/whl/cu116
-
+pip install icepy4d
 ```
 
-##### Install other required packages
+or install it from source by cloning the repository and installing it with `pip`
 
 ```bash
-pip3 install -r requirements.txt
+git clone https://github.com/franioli/icepy4d.git
+cd icepy4d
+pip install -e .
 ```
 
-##### Various
+In case of any error when installing `ICEpy4D` from PyPi, try to install it from source.
 
-- If you intend to use Jupyter Notebooks for running main scripts, install jupyterlab with
+Install Metashape Python API for Bundle Adjustment and Dense reconstruction.
+Metashape Python API can be downloaded from [https://www.agisoft.com/downloads/installer/](https://www.agisoft.com/downloads/installer/) or use `wget` (under Linux).
 
 ```bash
-pip3 install jupyterlab
+wget https://s3-eu-west-1.amazonaws.com/download.agisoft.com/Metashape-1.8.5-cp35.cp36.cp37.cp38-abi3-linux_x86_64.whl
+pip install Metashape-1.8.5-cp35.cp36.cp37.cp38-abi3-linux_x86_64.whl
 ```
 
-- When using VScode and Matplotlib, use TkAgg as interactive backend.
-
-##### Install ICEpy4D
-
-Install ICEpy4D package by running from the root folder
+You need to have a valid Metashape license to use the API and you need to activate it (see [https://github.com/franioli/metashape](https://github.com/franioli/metashape) for how to do it)
 
-```bash
-pip install -e .
-```
-
-and try to import it
+Try to import ICEpy4D package
 
 ```bash
 conda activate icepy4d
 python -c "import icepy4d"
 ```
 
-If no error is given, ICEpy4D is successfully installed and it can be imported with `import icepy4d`
+If no error is given, ICEpy4D is successfully installed and it can be imported within your script with `import icepy4d`
 
+### For contributing
 
-#### For contributing
-`bash
+Install additional requirements for development:
+
+```bash
 pip install -r requirements-dev.txt
 pre-commit install
-`
+```
```

### Comparing `icepy4d-1.4.0/src/icepy4d.egg-info/SOURCES.txt` & `icepy4d-1.6.2/src/icepy4d.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 LICENSE.txt
 README.md
 pyproject.toml
 src/icepy4d/__init__.py
 src/icepy4d/__main__.py
-src/icepy4d/binned_stats.py
-src/icepy4d/tiles.py
-src/icepy4d/tracking_features_utils.py
 src/icepy4d.egg-info/PKG-INFO
 src/icepy4d.egg-info/SOURCES.txt
 src/icepy4d.egg-info/dependency_links.txt
 src/icepy4d.egg-info/requires.txt
 src/icepy4d.egg-info/top_level.txt
 src/icepy4d/classes/__init__.py
 src/icepy4d/classes/camera.py
@@ -46,14 +43,15 @@
 src/icepy4d/io/colmap_utils/nvm_to_ply.py
 src/icepy4d/io/colmap_utils/plyfile.py
 src/icepy4d/io/colmap_utils/read_write_dense.py
 src/icepy4d/io/colmap_utils/read_write_fused_vis.py
 src/icepy4d/io/colmap_utils/read_write_model.py
 src/icepy4d/io/colmap_utils/visualize_model.py
 src/icepy4d/least_squares/__init__.py
+src/icepy4d/least_squares/absolute_orientation.py
 src/icepy4d/least_squares/rototra3d.py
 src/icepy4d/least_squares/utils.py
 src/icepy4d/matching/__init__.py
 src/icepy4d/matching/match_by_preselection.py
 src/icepy4d/matching/match_pairs.py
 src/icepy4d/matching/matching_base.py
 src/icepy4d/matching/retrieve_matches_from_npz.py
@@ -63,15 +61,15 @@
 src/icepy4d/matching/templatematch.py
 src/icepy4d/matching/track_matches.py
 src/icepy4d/matching/track_matches_bk.py
 src/icepy4d/matching/tracking_base.py
 src/icepy4d/matching/utils.py
 src/icepy4d/metashape/__init__.py
 src/icepy4d/metashape/metashape.py
-src/icepy4d/metashape/ms_utils.py
+src/icepy4d/metashape/metashape_core.py
 src/icepy4d/point_cloud_proc/__init__.py
 src/icepy4d/point_cloud_proc/cloudcompare_fun.py
 src/icepy4d/point_cloud_proc/open3d_fun.py
 src/icepy4d/point_cloud_proc/utils.py
 src/icepy4d/sfm/__init__.py
 src/icepy4d/sfm/absolute_orientation.py
 src/icepy4d/sfm/geometry.py
@@ -79,32 +77,40 @@
 src/icepy4d/sfm/reconstruction.py
 src/icepy4d/sfm/triangulation.py
 src/icepy4d/sfm/two_view_geometry.py
 src/icepy4d/thirdparty/__init__.py
 src/icepy4d/thirdparty/templatematch_pyimgraft.py
 src/icepy4d/thirdparty/transformations.py
 src/icepy4d/thirdparty/triangulation.py
+src/icepy4d/thirdparty/SuperGlue/models/__init__.py
+src/icepy4d/thirdparty/SuperGlue/models/matching.py
+src/icepy4d/thirdparty/SuperGlue/models/superglue.py
+src/icepy4d/thirdparty/SuperGlue/models/superpoint.py
+src/icepy4d/thirdparty/SuperGlue/models/utils.py
 src/icepy4d/thirdparty/SuperGluePretrainedNetwork/demo_superglue.py
 src/icepy4d/thirdparty/SuperGluePretrainedNetwork/match_pairs.py
 src/icepy4d/thirdparty/SuperGluePretrainedNetwork/models/__init__.py
 src/icepy4d/thirdparty/SuperGluePretrainedNetwork/models/matching.py
 src/icepy4d/thirdparty/SuperGluePretrainedNetwork/models/superglue.py
 src/icepy4d/thirdparty/SuperGluePretrainedNetwork/models/superpoint.py
 src/icepy4d/thirdparty/SuperGluePretrainedNetwork/models/utils.py
 src/icepy4d/utils/__init__.py
+src/icepy4d/utils/binned_stats.py
 src/icepy4d/utils/dsm_orthophoto.py
+src/icepy4d/utils/homography.py
 src/icepy4d/utils/initialization.py
 src/icepy4d/utils/logger.py
-src/icepy4d/utils/rototranslation.py
+src/icepy4d/utils/math.py
 src/icepy4d/utils/sensor_width_database.py
 src/icepy4d/utils/spatial_funs.py
+src/icepy4d/utils/tiles.py
 src/icepy4d/utils/timer.py
-src/icepy4d/utils/utils.py
+src/icepy4d/utils/tracking_features_utils.py
+src/icepy4d/utils/transformations.py
 src/icepy4d/visualization/__init__.py
-src/icepy4d/visualization/vis_o3d_advanced.py
 src/icepy4d/visualization/visualization.py
 tests/test_features.py
 tests/test_image.py
 tests/test_initialization.py
 tests/test_matching.py
 tests/test_point_cloud.py
 tests/test_sfm_geometry.py
```

### Comparing `icepy4d-1.4.0/tests/test_features.py` & `icepy4d-1.6.2/tests/test_features.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/tests/test_image.py` & `icepy4d-1.6.2/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/tests/test_initialization.py` & `icepy4d-1.6.2/tests/test_initialization.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/tests/test_matching.py` & `icepy4d-1.6.2/tests/test_matching.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/tests/test_point_cloud.py` & `icepy4d-1.6.2/tests/test_point_cloud.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/tests/test_sfm_geometry.py` & `icepy4d-1.6.2/tests/test_sfm_geometry.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/tests/test_utils.py` & `icepy4d-1.6.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/tests/test_utils_spatial.py` & `icepy4d-1.6.2/tests/test_utils_spatial.py`

 * *Files identical despite different names*

