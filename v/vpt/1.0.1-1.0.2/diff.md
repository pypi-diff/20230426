# Comparing `tmp/vpt-1.0.1.tar.gz` & `tmp/vpt-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vpt-1.0.1.tar", max compression
+gzip compressed data, was "vpt-1.0.2.tar", max compression
```

## Comparing `vpt-1.0.1.tar` & `vpt-1.0.2.tar`

### file list

```diff
@@ -1,126 +1,125 @@
--rw-r--r--   0        0        0    11357 2023-01-24 21:08:43.642309 vpt-1.0.1/LICENSE.md
--rw-r--r--   0        0        0     5273 2023-01-24 21:08:43.642309 vpt-1.0.1/README.md
--rw-r--r--   0        0        0     2298 2023-01-24 21:12:24.599746 vpt-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      355 2023-01-24 21:08:43.646309 vpt-1.0.1/src/vpt/__init__.py
--rw-r--r--   0        0        0        0 2023-01-24 21:08:43.646309 vpt-1.0.1/src/vpt/app/__init__.py
--rw-r--r--   0        0        0     5736 2023-01-24 21:08:43.646309 vpt-1.0.1/src/vpt/app/context.py
--rw-r--r--   0        0        0      161 2023-01-24 21:08:43.646309 vpt-1.0.1/src/vpt/app/empty.py
--rw-r--r--   0        0        0      324 2023-01-24 21:08:43.646309 vpt-1.0.1/src/vpt/app/task.py
--rw-r--r--   0        0        0     7960 2023-01-24 21:08:43.646309 vpt-1.0.1/src/vpt/cmd_args.py
--rw-r--r--   0        0        0      295 2023-01-24 21:08:43.646309 vpt-1.0.1/src/vpt/compile_tile_segmentation/__init__.py
--rw-r--r--   0        0        0     1864 2023-01-24 21:08:43.646309 vpt-1.0.1/src/vpt/compile_tile_segmentation/cmd_args.py
--rw-r--r--   0        0        0     3574 2023-01-24 21:08:43.646309 vpt-1.0.1/src/vpt/compile_tile_segmentation/main.py
--rw-r--r--   0        0        0     1708 2023-01-24 21:08:43.646309 vpt-1.0.1/src/vpt/compile_tile_segmentation/parameters.py
--rw-r--r--   0        0        0      270 2023-01-24 21:08:43.646309 vpt-1.0.1/src/vpt/convert_geometry/__init__.py
--rw-r--r--   0        0        0     6077 2023-01-24 21:08:43.646309 vpt-1.0.1/src/vpt/convert_geometry/cmd_args.py
--rw-r--r--   0        0        0        0 2023-01-24 21:08:43.646309 vpt-1.0.1/src/vpt/convert_geometry/converters/__init__.py
--rw-r--r--   0        0        0      398 2023-01-24 21:08:43.646309 vpt-1.0.1/src/vpt/convert_geometry/converters/entity_id_generator.py
--rw-r--r--   0        0        0     2963 2023-01-24 21:08:43.646309 vpt-1.0.1/src/vpt/convert_geometry/converters/hdf5_converter.py
--rw-r--r--   0        0        0     2222 2023-01-24 21:08:43.646309 vpt-1.0.1/src/vpt/convert_geometry/converters/old_parquet_converter.py
--rw-r--r--   0        0        0     1849 2023-01-24 21:08:43.646309 vpt-1.0.1/src/vpt/convert_geometry/converters/qpath_geojson_converter.py
--rw-r--r--   0        0        0     1463 2023-01-24 21:08:43.646309 vpt-1.0.1/src/vpt/convert_geometry/factory.py
--rw-r--r--   0        0        0     3088 2023-01-24 21:08:43.646309 vpt-1.0.1/src/vpt/convert_geometry/main.py
--rw-r--r--   0        0        0      488 2023-01-24 21:08:43.646309 vpt-1.0.1/src/vpt/convert_to_ome/__init__.py
--rw-r--r--   0        0        0     2472 2023-01-24 21:08:43.646309 vpt-1.0.1/src/vpt/convert_to_ome/cmd_args.py
--rw-r--r--   0        0        0     1847 2023-01-24 21:08:43.646309 vpt-1.0.1/src/vpt/convert_to_ome/main.py
--rw-r--r--   0        0        0     2033 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/convert_to_ome/main_rgb.py
--rw-r--r--   0        0        0     2618 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/convert_to_ome/rgb_cmd_args.py
--rw-r--r--   0        0        0     3993 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/convert_to_ome/tiffutils.py
--rw-r--r--   0        0        0      305 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/derive_cell_metadata/__init__.py
--rw-r--r--   0        0        0      217 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/derive_cell_metadata/__main__.py
--rw-r--r--   0        0        0     4580 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/derive_cell_metadata/cell_metadata.py
--rw-r--r--   0        0        0     1956 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/derive_cell_metadata/cmd_args.py
--rw-r--r--   0        0        0     1200 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/derive_cell_metadata/run_derive_cell_metadata.py
--rw-r--r--   0        0        0      197 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/filesystem/__init__.py
--rw-r--r--   0        0        0     4765 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/filesystem/vzgfs.py
--rw-r--r--   0        0        0     2031 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/log.py
--rw-r--r--   0        0        0      310 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/partition_transcripts/__init__.py
--rw-r--r--   0        0        0      222 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/partition_transcripts/__main__.py
--rw-r--r--   0        0        0     4496 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/partition_transcripts/cell_x_gene.py
--rw-r--r--   0        0        0     3290 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/partition_transcripts/cmd_args.py
--rw-r--r--   0        0        0     1409 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/partition_transcripts/run_partition_transcripts.py
--rw-r--r--   0        0        0      283 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/prepare_segmentation/__init__.py
--rw-r--r--   0        0        0     3859 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/prepare_segmentation/cmd_args.py
--rw-r--r--   0        0        0       53 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/prepare_segmentation/constants.py
--rw-r--r--   0        0        0     1407 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/prepare_segmentation/input_tools.py
--rw-r--r--   0        0        0     3658 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/prepare_segmentation/main.py
--rw-r--r--   0        0        0      510 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/prepare_segmentation/output_tools.py
--rw-r--r--   0        0        0      814 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/prepare_segmentation/tiles.py
--rw-r--r--   0        0        0     2143 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/prepare_segmentation/validate.py
--rw-r--r--   0        0        0     1280 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/profiler.py
--rw-r--r--   0        0        0      259 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/run_segmentation/__init__.py
--rw-r--r--   0        0        0     4451 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/run_segmentation/cmd_args.py
--rw-r--r--   0        0        0     1643 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/run_segmentation/main.py
--rw-r--r--   0        0        0      291 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/run_segmentation_on_tile/__init__.py
--rw-r--r--   0        0        0       90 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/run_segmentation_on_tile/__main__.py
--rw-r--r--   0        0        0     2109 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/run_segmentation_on_tile/cmd_args.py
--rw-r--r--   0        0        0     3046 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/run_segmentation_on_tile/image.py
--rw-r--r--   0        0        0     5175 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/run_segmentation_on_tile/input_utils.py
--rw-r--r--   0        0        0     4574 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/run_segmentation_on_tile/main.py
--rw-r--r--   0        0        0     3241 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/run_segmentation_on_tile/output_utils.py
--rw-r--r--   0        0        0        0 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/segmentation/__init__.py
--rw-r--r--   0        0        0        0 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/segmentation/cellpose/__init__.py
--rw-r--r--   0        0        0     3022 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/segmentation/cellpose/segmentation.py
--rw-r--r--   0        0        0      594 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/segmentation/cellpose/validate.py
--rw-r--r--   0        0        0      327 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/segmentation/entity.py
--rw-r--r--   0        0        0     1395 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/segmentation/factory.py
--rw-r--r--   0        0        0        0 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/segmentation/filters/__init__.py
--rw-r--r--   0        0        0      362 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/segmentation/filters/description.py
--rw-r--r--   0        0        0     3144 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/segmentation/filters/factory.py
--rw-r--r--   0        0        0        0 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/segmentation/stardist/__init__.py
--rw-r--r--   0        0        0     3916 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/segmentation/stardist/seeds.py
--rw-r--r--   0        0        0      132 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/segmentation/stardist/star.py
--rw-r--r--   0        0        0      330 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/segmentation/types.py
--rw-r--r--   0        0        0        0 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/segmentation/utils/__init__.py
--rw-r--r--   0        0        0     2625 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/segmentation/utils/fuse.py
--rw-r--r--   0        0        0     5481 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/segmentation/utils/polygon_utils.py
--rw-r--r--   0        0        0    19569 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/segmentation/utils/seg_result.py
--rw-r--r--   0        0        0      120 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/segmentation/watershed/__init__.py
--rw-r--r--   0        0        0     3835 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/segmentation/watershed/seeds.py
--rw-r--r--   0        0        0     5440 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/segmentation/watershed/segmentation.py
--rw-r--r--   0        0        0     1350 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/segmentation/watershed/validate.py
--rw-r--r--   0        0        0      225 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/sum_signals/__init__.py
--rw-r--r--   0        0        0     2681 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/sum_signals/cmd_args.py
--rw-r--r--   0        0        0     6401 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/sum_signals/main.py
--rw-r--r--   0        0        0      462 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/sum_signals/validate.py
--rw-r--r--   0        0        0      428 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/update_vzg/__init__.py
--rw-r--r--   0        0        0      132 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/update_vzg/__main__.py
--rw-r--r--   0        0        0      169 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/update_vzg/assemble/__init__.py
--rw-r--r--   0        0        0     3581 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/update_vzg/assemble/cell_coloring.py
--rw-r--r--   0        0        0     2260 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/update_vzg/assemble/dataset_assemble.py
--rw-r--r--   0        0        0     6011 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/update_vzg/assemble/expression_matrix.py
--rw-r--r--   0        0        0     2435 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/update_vzg/cell_metadata.py
--rw-r--r--   0        0        0     2444 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/update_vzg/cmd_args.py
--rw-r--r--   0        0        0      346 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/update_vzg/imageparams.py
--rw-r--r--   0        0        0     2563 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/update_vzg/manifestgen.py
--rw-r--r--   0        0        0     8924 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/update_vzg/polygon_transfer.py
--rw-r--r--   0        0        0        0 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/update_vzg/polygons/__init__.py
--rw-r--r--   0        0        0     5463 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/update_vzg/polygons/packedfanpolygon.py
--rw-r--r--   0        0        0     1743 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/update_vzg/polygons/packedpolygon.py
--rw-r--r--   0        0        0     5794 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/update_vzg/polygons/packedstarpolygon.py
--rw-r--r--   0        0        0    10801 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/update_vzg/polygons/poly_partition.py
--rw-r--r--   0        0        0    15845 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/update_vzg/polygons/polygonset.py
--rw-r--r--   0        0        0     1883 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/update_vzg/polygons/polystructers.py
--rw-r--r--   0        0        0     4679 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/update_vzg/polygons/vector_operations.py
--rw-r--r--   0        0        0     5210 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/update_vzg/run_update_vzg.py
--rw-r--r--   0        0        0        0 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/utils/__init__.py
--rw-r--r--   0        0        0      593 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/utils/boundaries.py
--rw-r--r--   0        0        0     3371 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/utils/cellsreader.py
--rw-r--r--   0        0        0     2780 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/utils/general_data.py
--rw-r--r--   0        0        0      866 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/utils/input_utils.py
--rw-r--r--   0        0        0     2954 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/utils/output_tools.py
--rw-r--r--   0        0        0      845 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/utils/raw_cell.py
--rw-r--r--   0        0        0     2908 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/utils/regex_tools.py
--rw-r--r--   0        0        0        0 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/utils/seg_json_generator/__init__.py
--rw-r--r--   0        0        0     1066 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/utils/seg_json_generator/cmd_args.py
--rw-r--r--   0        0        0     3257 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/utils/seg_json_generator/input_utils.py
--rw-r--r--   0        0        0     1499 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/utils/seg_json_generator/main.py
--rw-r--r--   0        0        0     3459 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/utils/seg_json_generator/templates/cellpose_default.json
--rw-r--r--   0        0        0     1699 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/utils/seg_json_generator/templates/watershed_default.json
--rw-r--r--   0        0        0     1969 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/utils/seg_json_generator/templates/watershed_m.json
--rw-r--r--   0        0        0     2181 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/utils/seg_json_generator/templates/watershed_m_downsample.json
--rw-r--r--   0        0        0      991 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/utils/validate.py
--rw-r--r--   0        0        0     5451 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/utils/vzgrepacker.py
--rw-r--r--   0        0        0     2435 2023-01-24 21:08:43.650309 vpt-1.0.1/src/vpt/vizgen_postprocess.py
--rw-r--r--   0        0        0     7486 1970-01-01 00:00:00.000000 vpt-1.0.1/setup.py
--rw-r--r--   0        0        0     7311 1970-01-01 00:00:00.000000 vpt-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11558 2023-01-23 20:24:29.923288 vpt-1.0.2/LICENSE.md
+-rw-r--r--   0        0        0     2380 2023-04-26 02:39:39.506493 vpt-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5400 2023-04-25 20:01:30.745480 vpt-1.0.2/README.md
+-rw-r--r--   0        0        0      369 2023-01-23 18:29:43.604418 vpt-1.0.2/src/vpt/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-23 18:29:43.604418 vpt-1.0.2/src/vpt/app/__init__.py
+-rw-r--r--   0        0        0     5909 2023-01-23 18:29:43.605419 vpt-1.0.2/src/vpt/app/context.py
+-rw-r--r--   0        0        0      170 2023-01-23 18:29:43.605419 vpt-1.0.2/src/vpt/app/empty.py
+-rw-r--r--   0        0        0      339 2023-01-23 18:29:43.606419 vpt-1.0.2/src/vpt/app/task.py
+-rw-r--r--   0        0        0     8086 2023-01-23 18:29:43.606419 vpt-1.0.2/src/vpt/cmd_args.py
+-rw-r--r--   0        0        0      305 2023-01-23 18:29:43.607420 vpt-1.0.2/src/vpt/compile_tile_segmentation/__init__.py
+-rw-r--r--   0        0        0     1907 2023-01-23 18:29:43.607420 vpt-1.0.2/src/vpt/compile_tile_segmentation/cmd_args.py
+-rw-r--r--   0        0        0     3670 2023-01-23 18:29:43.608421 vpt-1.0.2/src/vpt/compile_tile_segmentation/main.py
+-rw-r--r--   0        0        0     1752 2023-01-23 18:29:43.608421 vpt-1.0.2/src/vpt/compile_tile_segmentation/parameters.py
+-rw-r--r--   0        0        0      280 2023-01-23 18:29:43.609847 vpt-1.0.2/src/vpt/convert_geometry/__init__.py
+-rw-r--r--   0        0        0     6189 2023-01-23 18:29:43.610258 vpt-1.0.2/src/vpt/convert_geometry/cmd_args.py
+-rw-r--r--   0        0        0        0 2023-01-23 18:29:43.610258 vpt-1.0.2/src/vpt/convert_geometry/converters/__init__.py
+-rw-r--r--   0        0        0      419 2023-01-23 18:29:43.611264 vpt-1.0.2/src/vpt/convert_geometry/converters/entity_id_generator.py
+-rw-r--r--   0        0        0     3036 2023-01-23 18:29:43.611264 vpt-1.0.2/src/vpt/convert_geometry/converters/hdf5_converter.py
+-rw-r--r--   0        0        0     2272 2023-01-23 18:29:43.612265 vpt-1.0.2/src/vpt/convert_geometry/converters/old_parquet_converter.py
+-rw-r--r--   0        0        0     1892 2023-01-23 18:29:43.612265 vpt-1.0.2/src/vpt/convert_geometry/converters/qpath_geojson_converter.py
+-rw-r--r--   0        0        0     1502 2023-01-23 18:29:43.613264 vpt-1.0.2/src/vpt/convert_geometry/factory.py
+-rw-r--r--   0        0        0     3166 2023-01-23 18:29:43.613264 vpt-1.0.2/src/vpt/convert_geometry/main.py
+-rw-r--r--   0        0        0      505 2023-01-23 18:29:43.613264 vpt-1.0.2/src/vpt/convert_to_ome/__init__.py
+-rw-r--r--   0        0        0     2526 2023-01-23 18:29:43.614264 vpt-1.0.2/src/vpt/convert_to_ome/cmd_args.py
+-rw-r--r--   0        0        0     1896 2023-01-23 18:29:43.614264 vpt-1.0.2/src/vpt/convert_to_ome/main.py
+-rw-r--r--   0        0        0     2090 2023-01-23 18:29:43.614264 vpt-1.0.2/src/vpt/convert_to_ome/main_rgb.py
+-rw-r--r--   0        0        0     2680 2023-01-23 18:29:43.615263 vpt-1.0.2/src/vpt/convert_to_ome/rgb_cmd_args.py
+-rw-r--r--   0        0        0     4113 2023-01-23 18:29:43.615263 vpt-1.0.2/src/vpt/convert_to_ome/tiffutils.py
+-rw-r--r--   0        0        0      315 2023-01-23 18:29:43.616265 vpt-1.0.2/src/vpt/derive_cell_metadata/__init__.py
+-rw-r--r--   0        0        0      222 2023-01-23 18:29:43.616265 vpt-1.0.2/src/vpt/derive_cell_metadata/__main__.py
+-rw-r--r--   0        0        0     4720 2023-01-23 18:29:43.616265 vpt-1.0.2/src/vpt/derive_cell_metadata/cell_metadata.py
+-rw-r--r--   0        0        0     2002 2023-01-23 18:29:43.617264 vpt-1.0.2/src/vpt/derive_cell_metadata/cmd_args.py
+-rw-r--r--   0        0        0     1234 2023-01-23 18:29:43.617264 vpt-1.0.2/src/vpt/derive_cell_metadata/run_derive_cell_metadata.py
+-rw-r--r--   0        0        0      203 2023-01-23 18:29:43.618264 vpt-1.0.2/src/vpt/filesystem/__init__.py
+-rw-r--r--   0        0        0     4923 2023-01-23 18:29:43.618264 vpt-1.0.2/src/vpt/filesystem/vzgfs.py
+-rw-r--r--   0        0        0     2124 2023-01-23 18:29:43.618264 vpt-1.0.2/src/vpt/log.py
+-rw-r--r--   0        0        0      320 2023-01-23 18:29:43.619264 vpt-1.0.2/src/vpt/partition_transcripts/__init__.py
+-rw-r--r--   0        0        0      227 2023-01-23 18:29:43.619264 vpt-1.0.2/src/vpt/partition_transcripts/__main__.py
+-rw-r--r--   0        0        0     4619 2023-01-23 18:29:43.620264 vpt-1.0.2/src/vpt/partition_transcripts/cell_x_gene.py
+-rw-r--r--   0        0        0     3358 2023-01-23 18:29:43.620264 vpt-1.0.2/src/vpt/partition_transcripts/cmd_args.py
+-rw-r--r--   0        0        0     1448 2023-01-23 18:29:43.621265 vpt-1.0.2/src/vpt/partition_transcripts/run_partition_transcripts.py
+-rw-r--r--   0        0        0      293 2023-01-23 18:29:43.622264 vpt-1.0.2/src/vpt/prepare_segmentation/__init__.py
+-rw-r--r--   0        0        0     3932 2023-01-23 18:29:43.622264 vpt-1.0.2/src/vpt/prepare_segmentation/cmd_args.py
+-rw-r--r--   0        0        0       54 2023-01-23 18:29:43.622264 vpt-1.0.2/src/vpt/prepare_segmentation/constants.py
+-rw-r--r--   0        0        0     1465 2023-01-23 18:29:43.623264 vpt-1.0.2/src/vpt/prepare_segmentation/input_tools.py
+-rw-r--r--   0        0        0     3740 2023-01-23 18:29:43.623264 vpt-1.0.2/src/vpt/prepare_segmentation/main.py
+-rw-r--r--   0        0        0      528 2023-01-23 18:29:43.624265 vpt-1.0.2/src/vpt/prepare_segmentation/output_tools.py
+-rw-r--r--   0        0        0      840 2023-01-23 18:29:43.624265 vpt-1.0.2/src/vpt/prepare_segmentation/tiles.py
+-rw-r--r--   0        0        0     2186 2023-01-23 18:29:43.624265 vpt-1.0.2/src/vpt/prepare_segmentation/validate.py
+-rw-r--r--   0        0        0     1336 2023-01-23 18:29:43.625264 vpt-1.0.2/src/vpt/profiler.py
+-rw-r--r--   0        0        0      269 2023-01-23 18:29:43.625264 vpt-1.0.2/src/vpt/run_segmentation/__init__.py
+-rw-r--r--   0        0        0     4533 2023-01-23 18:29:43.626264 vpt-1.0.2/src/vpt/run_segmentation/cmd_args.py
+-rw-r--r--   0        0        0     1686 2023-01-23 18:29:43.626264 vpt-1.0.2/src/vpt/run_segmentation/main.py
+-rw-r--r--   0        0        0      301 2023-01-23 18:29:43.626264 vpt-1.0.2/src/vpt/run_segmentation_on_tile/__init__.py
+-rw-r--r--   0        0        0       94 2023-01-23 18:29:43.627264 vpt-1.0.2/src/vpt/run_segmentation_on_tile/__main__.py
+-rw-r--r--   0        0        0     2161 2023-01-23 18:29:43.627264 vpt-1.0.2/src/vpt/run_segmentation_on_tile/cmd_args.py
+-rw-r--r--   0        0        0     3121 2023-01-23 18:29:43.627264 vpt-1.0.2/src/vpt/run_segmentation_on_tile/image.py
+-rw-r--r--   0        0        0     5309 2023-01-23 18:29:43.628264 vpt-1.0.2/src/vpt/run_segmentation_on_tile/input_utils.py
+-rw-r--r--   0        0        0     4680 2023-01-23 18:29:43.628264 vpt-1.0.2/src/vpt/run_segmentation_on_tile/main.py
+-rw-r--r--   0        0        0     3316 2023-01-23 18:29:43.629264 vpt-1.0.2/src/vpt/run_segmentation_on_tile/output_utils.py
+-rw-r--r--   0        0        0        0 2023-01-23 18:29:43.629264 vpt-1.0.2/src/vpt/segmentation/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-23 18:29:43.630264 vpt-1.0.2/src/vpt/segmentation/cellpose/__init__.py
+-rw-r--r--   0        0        0     3103 2023-01-23 18:29:43.630264 vpt-1.0.2/src/vpt/segmentation/cellpose/segmentation.py
+-rw-r--r--   0        0        0      610 2023-01-23 18:29:43.630264 vpt-1.0.2/src/vpt/segmentation/cellpose/validate.py
+-rw-r--r--   0        0        0      343 2023-01-23 18:29:43.631264 vpt-1.0.2/src/vpt/segmentation/entity.py
+-rw-r--r--   0        0        0     1431 2023-01-23 18:29:43.631264 vpt-1.0.2/src/vpt/segmentation/factory.py
+-rw-r--r--   0        0        0        0 2023-01-23 18:29:43.631264 vpt-1.0.2/src/vpt/segmentation/filters/__init__.py
+-rw-r--r--   0        0        0      379 2023-01-23 18:29:43.632264 vpt-1.0.2/src/vpt/segmentation/filters/description.py
+-rw-r--r--   0        0        0     3237 2023-01-23 18:29:43.632264 vpt-1.0.2/src/vpt/segmentation/filters/factory.py
+-rw-r--r--   0        0        0        0 2023-01-23 18:29:43.632264 vpt-1.0.2/src/vpt/segmentation/stardist/__init__.py
+-rw-r--r--   0        0        0     4017 2023-01-23 18:29:43.633264 vpt-1.0.2/src/vpt/segmentation/stardist/seeds.py
+-rw-r--r--   0        0        0      141 2023-01-23 18:29:43.633264 vpt-1.0.2/src/vpt/segmentation/stardist/star.py
+-rw-r--r--   0        0        0      345 2023-01-23 18:29:43.633264 vpt-1.0.2/src/vpt/segmentation/types.py
+-rw-r--r--   0        0        0        0 2023-01-23 18:29:43.636280 vpt-1.0.2/src/vpt/segmentation/utils/__init__.py
+-rw-r--r--   0        0        0     2689 2023-01-23 18:29:43.636280 vpt-1.0.2/src/vpt/segmentation/utils/fuse.py
+-rw-r--r--   0        0        0     5619 2023-01-23 18:29:43.636280 vpt-1.0.2/src/vpt/segmentation/utils/polygon_utils.py
+-rw-r--r--   0        0        0    19978 2023-01-23 18:29:43.638287 vpt-1.0.2/src/vpt/segmentation/utils/seg_result.py
+-rw-r--r--   0        0        0      123 2023-01-23 18:29:43.639267 vpt-1.0.2/src/vpt/segmentation/watershed/__init__.py
+-rw-r--r--   0        0        0     3938 2023-01-23 18:29:43.639267 vpt-1.0.2/src/vpt/segmentation/watershed/seeds.py
+-rw-r--r--   0        0        0     5580 2023-01-23 18:29:43.639267 vpt-1.0.2/src/vpt/segmentation/watershed/segmentation.py
+-rw-r--r--   0        0        0     1385 2023-01-23 18:29:43.640266 vpt-1.0.2/src/vpt/segmentation/watershed/validate.py
+-rw-r--r--   0        0        0      235 2023-01-23 18:29:43.641267 vpt-1.0.2/src/vpt/sum_signals/__init__.py
+-rw-r--r--   0        0        0     2739 2023-01-23 18:29:43.641267 vpt-1.0.2/src/vpt/sum_signals/cmd_args.py
+-rw-r--r--   0        0        0     6567 2023-01-23 18:29:43.642266 vpt-1.0.2/src/vpt/sum_signals/main.py
+-rw-r--r--   0        0        0      476 2023-01-23 18:29:43.642266 vpt-1.0.2/src/vpt/sum_signals/validate.py
+-rw-r--r--   0        0        0      447 2023-01-23 18:29:43.643267 vpt-1.0.2/src/vpt/update_vzg/__init__.py
+-rw-r--r--   0        0        0      136 2023-01-23 18:29:43.643267 vpt-1.0.2/src/vpt/update_vzg/__main__.py
+-rw-r--r--   0        0        0      176 2023-01-23 18:29:43.643267 vpt-1.0.2/src/vpt/update_vzg/assemble/__init__.py
+-rw-r--r--   0        0        0     3669 2023-01-23 18:29:43.644264 vpt-1.0.2/src/vpt/update_vzg/assemble/cell_coloring.py
+-rw-r--r--   0        0        0     2312 2023-01-23 18:29:43.644264 vpt-1.0.2/src/vpt/update_vzg/assemble/dataset_assemble.py
+-rw-r--r--   0        0        0     6152 2023-01-23 18:29:43.645265 vpt-1.0.2/src/vpt/update_vzg/assemble/expression_matrix.py
+-rw-r--r--   0        0        0     2502 2023-01-23 18:29:43.645265 vpt-1.0.2/src/vpt/update_vzg/cell_metadata.py
+-rw-r--r--   0        0        0     2573 2023-04-25 12:11:18.307193 vpt-1.0.2/src/vpt/update_vzg/cmd_args.py
+-rw-r--r--   0        0        0      355 2023-01-23 18:29:43.646267 vpt-1.0.2/src/vpt/update_vzg/imageparams.py
+-rw-r--r--   0        0        0     2644 2023-01-23 18:29:43.647266 vpt-1.0.2/src/vpt/update_vzg/manifestgen.py
+-rw-r--r--   0        0        0     9149 2023-01-23 18:29:43.647266 vpt-1.0.2/src/vpt/update_vzg/polygon_transfer.py
+-rw-r--r--   0        0        0        0 2023-01-23 18:29:43.648267 vpt-1.0.2/src/vpt/update_vzg/polygons/__init__.py
+-rw-r--r--   0        0        0     5610 2023-01-23 18:29:43.648267 vpt-1.0.2/src/vpt/update_vzg/polygons/packedfanpolygon.py
+-rw-r--r--   0        0        0     1795 2023-01-23 18:29:43.648267 vpt-1.0.2/src/vpt/update_vzg/polygons/packedpolygon.py
+-rw-r--r--   0        0        0     5936 2023-01-23 18:29:43.649267 vpt-1.0.2/src/vpt/update_vzg/polygons/packedstarpolygon.py
+-rw-r--r--   0        0        0    11060 2023-01-23 18:29:43.649267 vpt-1.0.2/src/vpt/update_vzg/polygons/poly_partition.py
+-rw-r--r--   0        0        0    16279 2023-01-23 18:29:43.650268 vpt-1.0.2/src/vpt/update_vzg/polygons/polygonset.py
+-rw-r--r--   0        0        0     1936 2023-01-23 18:29:43.650268 vpt-1.0.2/src/vpt/update_vzg/polygons/polystructers.py
+-rw-r--r--   0        0        0     4821 2023-01-23 18:29:43.650268 vpt-1.0.2/src/vpt/update_vzg/polygons/vector_operations.py
+-rw-r--r--   0        0        0     5335 2023-01-23 18:29:43.651266 vpt-1.0.2/src/vpt/update_vzg/run_update_vzg.py
+-rw-r--r--   0        0        0        0 2023-01-23 18:29:43.651266 vpt-1.0.2/src/vpt/utils/__init__.py
+-rw-r--r--   0        0        0      612 2023-01-23 18:29:43.651266 vpt-1.0.2/src/vpt/utils/boundaries.py
+-rw-r--r--   0        0        0     3484 2023-01-23 18:29:43.652268 vpt-1.0.2/src/vpt/utils/cellsreader.py
+-rw-r--r--   0        0        0     2872 2023-01-23 18:29:43.652268 vpt-1.0.2/src/vpt/utils/general_data.py
+-rw-r--r--   0        0        0      900 2023-01-23 18:29:43.653267 vpt-1.0.2/src/vpt/utils/input_utils.py
+-rw-r--r--   0        0        0     3050 2023-01-23 18:29:43.653267 vpt-1.0.2/src/vpt/utils/output_tools.py
+-rw-r--r--   0        0        0      873 2023-01-23 18:29:43.653267 vpt-1.0.2/src/vpt/utils/raw_cell.py
+-rw-r--r--   0        0        0     3004 2023-01-23 18:29:43.654267 vpt-1.0.2/src/vpt/utils/regex_tools.py
+-rw-r--r--   0        0        0        0 2023-01-23 18:29:43.655265 vpt-1.0.2/src/vpt/utils/seg_json_generator/__init__.py
+-rw-r--r--   0        0        0     1099 2023-01-23 18:29:43.655265 vpt-1.0.2/src/vpt/utils/seg_json_generator/cmd_args.py
+-rw-r--r--   0        0        0     3354 2023-01-23 18:29:43.655265 vpt-1.0.2/src/vpt/utils/seg_json_generator/input_utils.py
+-rw-r--r--   0        0        0     1537 2023-01-23 18:29:43.656266 vpt-1.0.2/src/vpt/utils/seg_json_generator/main.py
+-rw-r--r--   0        0        0     3593 2023-01-23 18:29:43.656266 vpt-1.0.2/src/vpt/utils/seg_json_generator/templates/cellpose_default.json
+-rw-r--r--   0        0        0     1765 2023-01-23 18:29:43.657266 vpt-1.0.2/src/vpt/utils/seg_json_generator/templates/watershed_default.json
+-rw-r--r--   0        0        0     2063 2023-01-23 18:29:43.657266 vpt-1.0.2/src/vpt/utils/seg_json_generator/templates/watershed_m.json
+-rw-r--r--   0        0        0     2284 2023-01-23 18:29:43.657266 vpt-1.0.2/src/vpt/utils/seg_json_generator/templates/watershed_m_downsample.json
+-rw-r--r--   0        0        0     1019 2023-01-23 18:29:43.658266 vpt-1.0.2/src/vpt/utils/validate.py
+-rw-r--r--   0        0        0     5593 2023-01-23 18:29:43.658266 vpt-1.0.2/src/vpt/utils/vzgrepacker.py
+-rw-r--r--   0        0        0     2513 2023-01-23 18:29:43.658266 vpt-1.0.2/src/vpt/vizgen_postprocess.py
+-rw-r--r--   0        0        0     7302 1970-01-01 00:00:00.000000 vpt-1.0.2/PKG-INFO
```

### Comparing `vpt-1.0.1/LICENSE.md` & `vpt-1.0.2/LICENSE.md`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `vpt-1.0.1/README.md` & `vpt-1.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,136 +1,136 @@
-[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
-![PyPI](https://img.shields.io/pypi/v/vpt)
-[![Coverage Status](https://coveralls.io/repos/github/Vizgen/vizgen-postprocessing/badge.svg?branch=develop&t=EsWr25)](https://coveralls.io/github/Vizgen/vizgen-postprocessing?branch=develop)
-
-# Vizgen Post-processing Tool
-
-The Vizgen Post-processing Tool (VPT) enables users to reprocess and refine the single-cell results of MERSCOPE experiments. 
-VPT is a command line tool that emphasizes scalable, reproducible analysis, and can be run on a workstation, a cluster, or 
-be deployed in a cloud computing environment.
-
-
-## Features
-- Perform cell segmentation
-    - Reproduce standard Vizgen segmentation options
-    - Perform reproducible custom segmentation
-- Import cell segmentation from other tools
-    - Supports geojson and hdf5 formats
-- Regenerate single cell data with new segmentation
-    - Cell by gene matrix
-    - Cell spatial metadata
-    - Image intensity in each cell
-    - Update MERSCOPE Vizualizer file (vzg)
-- Image format conversion
-    - Convert large tiff files to single or multi-channel Pyramidal OME-TIFF files
-- Nextflow compatible, example pipeline provided
-
-
-## Installation
-
-Install the tool through your choice of 
-- [pip](https://pip.pypa.io/en/stable/getting-started/)
-- [Docker](https://docs.docker.com/desktop/extensions-sdk/quickstart/)
-- [poetry](https://python-poetry.org/)
-
-To access in-utility help documentation run the process below in the installed environment.
-```bash
-  vpt --help
-```
-    
-## Usage
-
-VPT accepts two types of inputs to specify how to run segmentation:
-- Command line parameters
-    - relate to where to find the input data and are expected to vary with each experiment
-- Segmentation algorithm .json file parameters
-    - describes a series of steps to perform on the input data
-
-Using the same segmentation algorithm on a series of experiments ensures that they are processed identically and reproducibly.
-
-In addition to the user guide, several working segmentation algorithm .json files are provided that can serve either as a 
-robust segmentation definition or as a template for a custom workflow.
-
-## Quick start commands:
-
-
-run-segmentation    ​
-- Top-level interface for vpt which invokes the segmentation functionality of the tool.​
-
-prepare-segmentation​
- - Generates a segmentation specification json file to be used for cell segmentation tasks. ​
-
-run-segmentation-on-tile​
- - Executes the segmentation algorithm on a specific tile of the mosaic images.​
-
-compile-tile-segmentation​
-- Combines the per-tile segmentation outputs into a single, internally-consistent parquet file containing all of the 
-segmentation boundaries found in the experiment.​
-
-derive-entity-metadata​
-- Uses the segmentation boundaries to calculate the geometric attributes of each Entity​
-
-partition-transcripts​
-- Uses the segmentation boundaries to determine which Entity, if any, contains each detected transcript.​
-
-sum-signals​
-- Uses the segmentation boundaries to find the intensity of each mosaic image in each Entity.​
-
-update-vzg​
-- Updates an existing .vzg file with new segmentation boundaries and the corresponding expression matrix.​
-
-convert-geometry​
-- Converts Entity boundaries produced by a different tool into a vpt compatible parquet file.​
-
-convert-to-ome​
-- Transforms the large 16-bit mosaic tiff images produced by the MERSCOPE into a OME pyramidal tiff.​
-
-convert-to-rgb-ome​
-- Converts up to three flat tiff images into rgb OME-tiff pyramidal images.​
-
-For more detail on commands and arguments, please see the user guide.
-
-## Documentation
-
-[User Guide](https://vizgen.github.io/vizgen-postprocessing/)
-
-## Feedback
-
-If you encounter issues or bugs, let us know by [submitting an issue!](https://github.com/Vizgen/vizgen-postprocessing/issues)
-Please include:
-
-- A quick issue summary
-- Steps that caused it to occur
-- The exception generated by the code, if applicable
-- Specific lines of code, if indicated in the error message
-
-
-If you have any other feedback or issues, please reach out to your regional Vizgen field application scientist and CC: Vizgen 
-Tech Support at techsupport@vizgen.com.
-
-Please include VPT in your subject line along with the above information in the body.
-
-## Contributing & Code of Conduct
-
-We welcome code contributions! Please refer to the [contribution guide](CONTRIBUTING.md) before getting started.
-
-## Authors
-
-- [Vizgen](https://vizgen.com/)
-
-![Logo](https://vizgen.com/wp-content/uploads/2022/12/Vizgen-Logo_Vizgen-BlackColor-.png)
-
-## License
-
-   Copyright 2022 Vizgen, Inc. All Rights Reserved
-   
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
+![PyPI](https://img.shields.io/pypi/v/vpt)
+[![Coverage Status](https://coveralls.io/repos/github/Vizgen/vizgen-postprocessing/badge.svg?branch=develop)](https://coveralls.io/github/Vizgen/vizgen-postprocessing?branch=develop)
+
+# Vizgen Post-processing Tool
+
+The Vizgen Post-processing Tool (VPT) enables users to reprocess and refine the single-cell results of MERSCOPE experiments. 
+VPT is a command line tool that emphasizes scalable, reproducible analysis, and can be run on a workstation, a cluster, or 
+be deployed in a cloud computing environment.
+
+
+## Features
+- Perform cell segmentation
+    - Reproduce standard Vizgen segmentation options
+    - Perform reproducible custom segmentation
+- Import cell segmentation from other tools
+    - Supports geojson and hdf5 formats
+- Regenerate single cell data with new segmentation
+    - Cell by gene matrix
+    - Cell spatial metadata
+    - Image intensity in each cell
+    - Update MERSCOPE Vizualizer file (vzg)
+- Image format conversion
+    - Convert large tiff files to single or multi-channel Pyramidal OME-TIFF files
+- Nextflow compatible, example pipeline provided
+
+
+## Installation
+
+Install the tool through your choice of 
+- [pip](https://pip.pypa.io/en/stable/getting-started/)
+- [Docker](https://docs.docker.com/desktop/extensions-sdk/quickstart/)
+- [poetry](https://python-poetry.org/)
+
+To access in-utility help documentation run the process below in the installed environment.
+```bash
+  vpt --help
+```
+    
+## Usage
+
+VPT accepts two types of inputs to specify how to run segmentation:
+- Command line parameters
+    - relate to where to find the input data and are expected to vary with each experiment
+- Segmentation algorithm .json file parameters
+    - describes a series of steps to perform on the input data
+
+Using the same segmentation algorithm on a series of experiments ensures that they are processed identically and reproducibly.
+
+In addition to the user guide, several working segmentation algorithm .json files are provided that can serve either as a 
+robust segmentation definition or as a template for a custom workflow.
+
+## Quick start commands:
+
+
+run-segmentation    ​
+- Top-level interface for vpt which invokes the segmentation functionality of the tool.​
+
+prepare-segmentation​
+ - Generates a segmentation specification json file to be used for cell segmentation tasks. ​
+
+run-segmentation-on-tile​
+ - Executes the segmentation algorithm on a specific tile of the mosaic images.​
+
+compile-tile-segmentation​
+- Combines the per-tile segmentation outputs into a single, internally-consistent parquet file containing all of the 
+segmentation boundaries found in the experiment.​
+
+derive-entity-metadata​
+- Uses the segmentation boundaries to calculate the geometric attributes of each Entity​
+
+partition-transcripts​
+- Uses the segmentation boundaries to determine which Entity, if any, contains each detected transcript.​
+
+sum-signals​
+- Uses the segmentation boundaries to find the intensity of each mosaic image in each Entity.​
+
+update-vzg​
+- Updates an existing .vzg file with new segmentation boundaries and the corresponding expression matrix.​
+
+convert-geometry​
+- Converts Entity boundaries produced by a different tool into a vpt compatible parquet file.​
+
+convert-to-ome​
+- Transforms the large 16-bit mosaic tiff images produced by the MERSCOPE into a OME pyramidal tiff.​
+
+convert-to-rgb-ome​
+- Converts up to three flat tiff images into rgb OME-tiff pyramidal images.​
+
+For more detail on commands and arguments, please see the user guide.
+
+## Documentation
+
+[User Guide](https://vizgen.github.io/vizgen-postprocessing/)
+
+## Feedback
+
+If you encounter issues or bugs, let us know by [submitting an issue!](https://github.com/Vizgen/vizgen-postprocessing/issues)
+Please include:
+
+- A quick issue summary
+- Steps that caused it to occur
+- The exception generated by the code, if applicable
+- Specific lines of code, if indicated in the error message
+
+
+If you have any other feedback or issues, please reach out to your regional Vizgen field application scientist and CC: Vizgen 
+Tech Support at techsupport@vizgen.com.
+
+Please include VPT in your subject line along with the above information in the body.
+
+## Contributing & Code of Conduct
+
+We welcome code contributions! Please refer to the [contribution guide](CONTRIBUTING.md) before getting started.
+
+## Authors
+
+- [Vizgen](https://vizgen.com/)
+
+![Logo](https://vizgen.com/wp-content/uploads/2022/12/Vizgen-Logo_Vizgen-BlackColor-.png)
+
+## License
+
+   Copyright 2022 Vizgen, Inc. All Rights Reserved
+   
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `vpt-1.0.1/pyproject.toml` & `vpt-1.0.2/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,82 +1,82 @@
-[tool.poetry]
-name = "vpt"
-version = "1.0.1"
-description = "Command line tool for highly parallelized processing of Vizgen data"
-license = "Apache-2.0"
-authors = ["Vizgen <techsupport@vizgen.com>"]
-maintainers = ["Timothy Wiggin <timothy.wiggin@vizgen.com>"]
-readme = "README.md"
-# homepage = ""
-repository = "https://github.com/Vizgen/vizgen-postprocessing"
-documentation = "https://vizgen.github.io/vizgen-postprocessing/"
-# keywords = ""
-classifiers = ["Development Status :: 5 - Production/Stable",
-    "Natural Language :: English",
-    "Operating System :: POSIX :: Linux",
-    "Operating System :: MacOS :: MacOS X",
-    "Operating System :: Microsoft :: Windows",
-    "License :: OSI Approved :: Apache Software License",
-    "Topic :: Scientific/Engineering :: Image Processing",
-    "Topic :: Scientific/Engineering :: Bio-Informatics",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10"
-]
-packages = [{include = "vpt*", from = "src"}]
-include = ["src/vpt/utils/seg_json_generator/templates/*"]
-
-[tool.poetry.scripts]
-vpt = "vpt.vizgen_postprocess:entry_point"
-
-[tool.poetry.dependencies]
-python = ">=3.9,<3.11"
-boto3 = "1.17"
-cellpose = "1.0.2"
-dask = "2022.9.0"
-distributed = "2022.9.0"
-fsspec = "2021.10.0"
-geojson = "2.5.0"
-geopandas = "0.12.1"
-gcsfs = "2021.10.0"
-h5py = "3.7.0"
-numpy = "1.22.4"
-opencv-python-headless = "4.6.0.66"
-pandas = "1.4.3"
-pyarrow = "8.0.0"
-pyclustering = "0.10.1.2"
-python-dotenv = "0.20.0"
-pyvips = "2.2.1"
-rasterio = "1.3.0"
-s3fs = "2021.10.0"
-scikit-image = "0.19.3"
-scipy = "1.8.1"
-shapely = "2.0"
-stardist = "0.8.3"
-tensorflow = "2.9.1"
-
-[tool.poetry.group.dev.dependencies]
-pytest = "^7.2.0"
-pytest-cov = "^4.0.0"
-flake8 = "^6.0.0"
-
-[tool.poetry.group.deploy.dependencies]
-python-semantic-release = "^7.32.2"
-sphinx-argparse = "^0.4.0"
-sphinx-view = "^0.3.1"
-myst-nb = {version = "^0.17.1", python = "^3.9"}
-sphinx-autoapi = "^2.0.0"
-sphinx-rtd-theme = "^1.1.1"
-
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
-
-[tool.semantic_release]
-version_variable = "pyproject.toml:version"
-branch = "develop"
-changelog_file = "CHANGELOG.md"
-build_command = "poetry build"
-dist_path = "dist/"
-upload_to_release = true
-upload_to_pypi = false
-remove_dist = false
-patch_without_tag = true
+[tool.poetry]
+name = "vpt"
+version = "1.0.2"
+description = "Command line tool for highly parallelized processing of Vizgen data"
+license = "Apache-2.0"
+authors = ["Vizgen <techsupport@vizgen.com>"]
+maintainers = ["Timothy Wiggin <timothy.wiggin@vizgen.com>"]
+readme = "README.md"
+# homepage = ""
+repository = "https://github.com/Vizgen/vizgen-postprocessing"
+documentation = "https://vizgen.github.io/vizgen-postprocessing/"
+# keywords = ""
+classifiers = ["Development Status :: 5 - Production/Stable",
+    "Natural Language :: English",
+    "Operating System :: POSIX :: Linux",
+    "Operating System :: MacOS :: MacOS X",
+    "Operating System :: Microsoft :: Windows",
+    "License :: OSI Approved :: Apache Software License",
+    "Topic :: Scientific/Engineering :: Image Processing",
+    "Topic :: Scientific/Engineering :: Bio-Informatics",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10"
+]
+packages = [{include = "vpt*", from = "src"}]
+include = ["src/vpt/utils/seg_json_generator/templates/*"]
+
+[tool.poetry.scripts]
+vpt = "vpt.vizgen_postprocess:entry_point"
+
+[tool.poetry.dependencies]
+python = ">=3.9,<3.11"
+boto3 = "1.17"
+cellpose = "1.0.2"
+dask = "2022.9.0"
+distributed = "2022.9.0"
+fsspec = "2021.10.0"
+geojson = "2.5.0"
+geopandas = "0.12.1"
+gcsfs = "2021.10.0"
+h5py = "3.7.0"
+numpy = "1.22.4"
+opencv-python-headless = "4.6.0.66"
+pandas = "1.4.3"
+pyarrow = "8.0.0"
+pyclustering = "0.10.1.2"
+python-dotenv = "0.20.0"
+pyvips = "2.2.1"
+rasterio = "1.3.0"
+s3fs = "2021.10.0"
+scikit-image = "0.19.3"
+scipy = "1.8.1"
+shapely = "2.0"
+stardist = "0.8.3"
+tensorflow = "2.9.1"
+
+[tool.poetry.group.dev.dependencies]
+pytest = "^7.2.0"
+pytest-cov = "^4.0.0"
+flake8 = "^6.0.0"
+
+[tool.poetry.group.deploy.dependencies]
+python-semantic-release = "^7.32.2"
+sphinx-argparse = "^0.4.0"
+sphinx-view = "^0.3.1"
+myst-nb = {version = "^0.17.1", python = "^3.9"}
+sphinx-autoapi = "^2.0.0"
+sphinx-rtd-theme = "^1.1.1"
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
+
+[tool.semantic_release]
+version_variable = "pyproject.toml:version"
+branch = "develop"
+changelog_file = "CHANGELOG.md"
+build_command = "poetry build"
+dist_path = "dist/"
+upload_to_release = true
+upload_to_pypi = false
+remove_dist = false
+patch_without_tag = true
```

### Comparing `vpt-1.0.1/src/vpt/app/context.py` & `vpt-1.0.2/src/vpt/app/context.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,173 +1,173 @@
-from pathlib import Path
-from typing import List, Callable, Dict, Iterable, Optional
-
-import vpt.log as log
-from vpt.app.empty import Empty
-from vpt.app.task import Task
-from vpt.filesystem import initialize_filesystem
-from vpt import profiler
-import copy
-
-_contexts = []
-
-
-class Context:
-    name: str
-    dask_args: Dict
-    fs_args: Dict
-    log_args: Dict
-    prof_args: Dict
-
-    def __init__(self,
-                 name: str = None,
-                 dask_args: Dict = None,
-                 fs_args: Dict = None,
-                 log_args: Dict = None,
-                 prof_args: Dict = None):
-        self.name = name if name else '.'
-        self.dask_args = dask_args
-        self.fs_args = fs_args
-        self.prof_args = prof_args
-        self.log_args = log_args
-
-    def __enter__(self):
-        log.set_process_name(self.name)
-        if self.log_args:
-            log.initialize_logger(**self.log_args)
-        if self.fs_args:
-            initialize_filesystem(**self.fs_args)
-        else:
-            initialize_filesystem()
-
-        if self.prof_args:
-            profiler.initialize_profiler(**self.prof_args)
-            profiler.enable()
-        _contexts.append(self)
-        return self
-
-    def __exit__(self, exc_type, exc_val, exc_tb):
-        if exc_val is not None:
-            log.exception(f"exception of type {exc_type} thrown: {exc_val}")
-
-        log.release_logger()
-        profiler.disable()
-        profiler.export_data()
-        _contexts.pop()
-
-    def update_with_children(self, ctx_args: Iterable[Dict]):
-        # append profiler results
-        for child in ctx_args:
-            sub_prof = self._get_profile_name(child)
-            if sub_prof:
-                profiler.append_with_file(sub_prof)
-
-    def arguments(self) -> Dict:
-        return {'name': self.name,
-                'dask_args': self.dask_args,
-                'fs_args': self.fs_args,
-                'log_args': self.log_args,
-                'prof_args': self.prof_args}
-
-    @staticmethod
-    def _get_profile_name(args: Dict) -> Optional[str]:
-        pa = args.get('prof_args', None)
-        return pa['profile_file'] if pa else None
-
-    @staticmethod
-    def _set_profile_name(args: Dict, name: str):
-        args['prof_args']['profile_file'] = name
-
-    @staticmethod
-    def modify_context_as_sub(cnt_args: Dict, ind: int) -> Dict:
-        ret = copy.deepcopy(cnt_args)
-        pname = Context._get_profile_name(ret)
-        ret["name"] = f"{cnt_args['name']}/task-{ind}"
-        if pname:
-            parent = Path(pname)
-            Context._set_profile_name(ret, str(parent.with_stem(f"{parent.stem}_{ind}")))
-        return ret
-
-    def is_distributed(self) -> bool:
-        return self.dask_args is not None and self.dask_args.get('address', None)
-
-    def dask_client(self):
-        from dask.distributed import Client
-        return Client(self.dask_args['address'])
-
-    def run(self, proc: Callable, *args):
-
-        if not self.is_distributed():
-            proc(*args)
-        else:
-            def remote_run(ctx: Dict, proc: Callable, *args):
-                with Context(**ctx):
-                    proc(*args)
-
-            with self.dask_client() as c:
-                _ = c.submit(remote_run, self.arguments(), proc, *args).result()
-                log.info("contex.run.distributed finished!")
-
-    def get_workers_count(self) -> int:
-        if self.dask_args is not None:
-            if self.dask_args.get('address', None):
-                return len(self.dask_client().scheduler_info()['workers'])
-            else:
-                return self.dask_args.get('workers', 1)
-        else:
-            return 1
-
-    def get_cluster(self):
-        if self.is_distributed():
-            return Empty()
-        else:
-            from dask.distributed import LocalCluster
-            return LocalCluster(
-                n_workers=self.get_workers_count(),
-                threads_per_worker=1,
-                dashboard_address=None)
-
-    def get_client(self, cluster):
-        if self.is_distributed():
-            return self.dask_client()
-        from dask.distributed import Client
-        return Client(cluster)
-
-    def parallel_run(self, tasks: Iterable[Task]) -> List:
-        if self.get_workers_count() == 1:
-            return [t.proc(t.args) for t in tasks]
-        else:
-            import dask.bag as db
-            from dask.distributed import progress
-
-            # Initializes a Dask local cluster with the correct number of workers
-            with self.get_cluster() as cluster:
-                with self.get_client(cluster):
-                    cnt_args = self.arguments()
-                    children = [{'task': t,
-                                 'cnt_args': Context.modify_context_as_sub(cnt_args, i)
-                                 } for i, t in enumerate(tasks)]
-                    mp_bag = db.from_sequence(children)
-
-                    def _context_wrapper(task: Task, cnt_args):
-                        with Context(**cnt_args):
-                            return task.proc(task.args)
-
-                    # Runs processing using the Dask local cluster initialized above
-                    mp_bag = mp_bag.map(lambda b: _context_wrapper(**b))
-                    if log.is_verbose():
-                        progress(mp_bag)
-                    result = mp_bag.compute()
-                    self.update_with_children([x['cnt_args'] for x in children])
-
-                    return result
-
-
-def current_context() -> Context:
-    return _contexts[-1] if len(_contexts) > 0 else None
-
-
-def parallel_run(tasks: Iterable[Task]) -> List:
-    if current_context():
-        return current_context().parallel_run(tasks)
-    else:
-        return [t.proc(t.args) for t in tasks]
+from pathlib import Path
+from typing import List, Callable, Dict, Iterable, Optional
+
+import vpt.log as log
+from vpt.app.empty import Empty
+from vpt.app.task import Task
+from vpt.filesystem import initialize_filesystem
+from vpt import profiler
+import copy
+
+_contexts = []
+
+
+class Context:
+    name: str
+    dask_args: Dict
+    fs_args: Dict
+    log_args: Dict
+    prof_args: Dict
+
+    def __init__(self,
+                 name: str = None,
+                 dask_args: Dict = None,
+                 fs_args: Dict = None,
+                 log_args: Dict = None,
+                 prof_args: Dict = None):
+        self.name = name if name else '.'
+        self.dask_args = dask_args
+        self.fs_args = fs_args
+        self.prof_args = prof_args
+        self.log_args = log_args
+
+    def __enter__(self):
+        log.set_process_name(self.name)
+        if self.log_args:
+            log.initialize_logger(**self.log_args)
+        if self.fs_args:
+            initialize_filesystem(**self.fs_args)
+        else:
+            initialize_filesystem()
+
+        if self.prof_args:
+            profiler.initialize_profiler(**self.prof_args)
+            profiler.enable()
+        _contexts.append(self)
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        if exc_val is not None:
+            log.exception(f"exception of type {exc_type} thrown: {exc_val}")
+
+        log.release_logger()
+        profiler.disable()
+        profiler.export_data()
+        _contexts.pop()
+
+    def update_with_children(self, ctx_args: Iterable[Dict]):
+        # append profiler results
+        for child in ctx_args:
+            sub_prof = self._get_profile_name(child)
+            if sub_prof:
+                profiler.append_with_file(sub_prof)
+
+    def arguments(self) -> Dict:
+        return {'name': self.name,
+                'dask_args': self.dask_args,
+                'fs_args': self.fs_args,
+                'log_args': self.log_args,
+                'prof_args': self.prof_args}
+
+    @staticmethod
+    def _get_profile_name(args: Dict) -> Optional[str]:
+        pa = args.get('prof_args', None)
+        return pa['profile_file'] if pa else None
+
+    @staticmethod
+    def _set_profile_name(args: Dict, name: str):
+        args['prof_args']['profile_file'] = name
+
+    @staticmethod
+    def modify_context_as_sub(cnt_args: Dict, ind: int) -> Dict:
+        ret = copy.deepcopy(cnt_args)
+        pname = Context._get_profile_name(ret)
+        ret["name"] = f"{cnt_args['name']}/task-{ind}"
+        if pname:
+            parent = Path(pname)
+            Context._set_profile_name(ret, str(parent.with_stem(f"{parent.stem}_{ind}")))
+        return ret
+
+    def is_distributed(self) -> bool:
+        return self.dask_args is not None and self.dask_args.get('address', None)
+
+    def dask_client(self):
+        from dask.distributed import Client
+        return Client(self.dask_args['address'])
+
+    def run(self, proc: Callable, *args):
+
+        if not self.is_distributed():
+            proc(*args)
+        else:
+            def remote_run(ctx: Dict, proc: Callable, *args):
+                with Context(**ctx):
+                    proc(*args)
+
+            with self.dask_client() as c:
+                _ = c.submit(remote_run, self.arguments(), proc, *args).result()
+                log.info("contex.run.distributed finished!")
+
+    def get_workers_count(self) -> int:
+        if self.dask_args is not None:
+            if self.dask_args.get('address', None):
+                return len(self.dask_client().scheduler_info()['workers'])
+            else:
+                return self.dask_args.get('workers', 1)
+        else:
+            return 1
+
+    def get_cluster(self):
+        if self.is_distributed():
+            return Empty()
+        else:
+            from dask.distributed import LocalCluster
+            return LocalCluster(
+                n_workers=self.get_workers_count(),
+                threads_per_worker=1,
+                dashboard_address=None)
+
+    def get_client(self, cluster):
+        if self.is_distributed():
+            return self.dask_client()
+        from dask.distributed import Client
+        return Client(cluster)
+
+    def parallel_run(self, tasks: Iterable[Task]) -> List:
+        if self.get_workers_count() == 1:
+            return [t.proc(t.args) for t in tasks]
+        else:
+            import dask.bag as db
+            from dask.distributed import progress
+
+            # Initializes a Dask local cluster with the correct number of workers
+            with self.get_cluster() as cluster:
+                with self.get_client(cluster):
+                    cnt_args = self.arguments()
+                    children = [{'task': t,
+                                 'cnt_args': Context.modify_context_as_sub(cnt_args, i)
+                                 } for i, t in enumerate(tasks)]
+                    mp_bag = db.from_sequence(children)
+
+                    def _context_wrapper(task: Task, cnt_args):
+                        with Context(**cnt_args):
+                            return task.proc(task.args)
+
+                    # Runs processing using the Dask local cluster initialized above
+                    mp_bag = mp_bag.map(lambda b: _context_wrapper(**b))
+                    if log.is_verbose():
+                        progress(mp_bag)
+                    result = mp_bag.compute()
+                    self.update_with_children([x['cnt_args'] for x in children])
+
+                    return result
+
+
+def current_context() -> Context:
+    return _contexts[-1] if len(_contexts) > 0 else None
+
+
+def parallel_run(tasks: Iterable[Task]) -> List:
+    if current_context():
+        return current_context().parallel_run(tasks)
+    else:
+        return [t.proc(t.args) for t in tasks]
```

### Comparing `vpt-1.0.1/src/vpt/cmd_args.py` & `vpt-1.0.2/src/vpt/cmd_args.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,126 +1,126 @@
-from argparse import ArgumentParser, Namespace
-from typing import Callable
-
-from vpt.compile_tile_segmentation import get_parser as get_compile_tile_segmentation_parser, \
-    run as compile_tile_segmentation
-from vpt.convert_geometry import get_parser as get_convert_geometry_parser, run_conversion as convert_geometry
-from vpt.convert_to_ome import get_parser as get_convert_to_ome_parser, run_ome as convert_to_ome
-from vpt.convert_to_ome import get_parser_rgb as get_convert_to_rgb_ome_parser, run_ome_rgb as convert_to_rgb_ome
-from vpt.derive_cell_metadata import get_parser as get_derive_cell_metadata_parser, run as derive_cell_metadata
-from vpt.partition_transcripts import get_parser as get_partition_transcripts_parser, run as partition_transcripts
-from vpt.prepare_segmentation import get_parser as get_prepare_seg_parser, run as prepare_segmentation
-from vpt.run_segmentation import get_parser as get_run_segmentation_parser, run as run_segmentation
-from vpt.run_segmentation_on_tile import get_parser as get_run_seg_on_tile_parser, run as run_segmentation_on_tile
-from vpt.sum_signals import get_parser as get_sum_signals_parser, run as run_sum_signals
-from vpt.update_vzg import get_parser as get_update_vzg_parser, run as update_vzg
-
-
-def get_postprocess_parser() -> ArgumentParser:
-    parser = ArgumentParser(description='', usage='vpt [OPTIONS] COMMAND [arguments]', add_help=False,
-                            epilog="Run 'vpt COMMAND --help' for more information on a command.")
-    parser.add_argument('--processes', type=int, default=1, required=False,
-                        help='Number of parallel processes to use when executing locally')
-    parser.add_argument('--aws-profile-name', type=str, required=False,
-                        help="Named profile for AWS access")
-    parser.add_argument('--aws-access-key', type=str, required=False,
-                        help="AWS access key from key / secret pair")
-    parser.add_argument('--aws-secret-key', type=str, required=False,
-                        help="AWS secret from key / secret pair")
-    parser.add_argument('--gcs-service-account-key', type=str, required=False,
-                        help='Path to a google service account key json file. Not needed if google '
-                             'authentication is performed using gcloud')
-    parser.add_argument('--verbose', action='store_true', default=False, required=False,
-                        help='Display progress messages during execution')
-    parser.add_argument('--profile-execution-time', type=str, default=None, required=False,
-                        help='Path to profiler output file')
-    parser.add_argument('--log-level', type=int, default=1, required=False,
-                        help='Log level value. Level is specified as a number from 1 - 5, corresponding '
-                             'to debug, info, warning, error, crit')
-    parser.add_argument('--log-file', type=str, default=None, required=False,
-                        help='Path to log output file. If not provided, logs are written to standard output')
-    parser.add_argument("-h", "--help", action="help",
-                        help='Show this help message and exit')
-
-    parser._optionals.title = 'Options'
-    parser._positionals.title = 'Commands'
-
-    subparsers = parser.add_subparsers(dest='subparser_name', metavar='')
-
-    subparsers.add_parser('run-segmentation', parents=[get_run_segmentation_parser()], add_help=False,
-                          help=get_run_segmentation_parser().description,
-                          usage='vpt [OPTIONS] run-segmentation [arguments]',
-                          description=get_run_segmentation_parser().description)
-
-    subparsers.add_parser('prepare-segmentation', parents=[get_prepare_seg_parser()], add_help=False,
-                          help=get_prepare_seg_parser().description,
-                          usage='vpt [OPTIONS] prepare-segmentation [arguments]',
-                          description=get_prepare_seg_parser().description)
-
-    subparsers.add_parser('run-segmentation-on-tile', parents=[get_run_seg_on_tile_parser()], add_help=False,
-                          help=get_run_seg_on_tile_parser().description,
-                          usage='vpt [OPTIONS] run-segmentation-on-tile [arguments]',
-                          description=get_run_seg_on_tile_parser().description)
-
-    subparsers.add_parser('compile-tile-segmentation', parents=[get_compile_tile_segmentation_parser()], add_help=False,
-                          help=get_compile_tile_segmentation_parser().description,
-                          usage='vpt [OPTIONS] compile-tile-segmentation [arguments]',
-                          description=get_compile_tile_segmentation_parser().description)
-
-    subparsers.add_parser('derive-entity-metadata', parents=[get_derive_cell_metadata_parser()], add_help=False,
-                          help=get_derive_cell_metadata_parser().description,
-                          usage='vpt [OPTIONS] derive-entity-metadata [arguments]',
-                          description=get_derive_cell_metadata_parser().description)
-
-    subparsers.add_parser('partition-transcripts', parents=[get_partition_transcripts_parser()], add_help=False,
-                          help=get_partition_transcripts_parser().description,
-                          usage='vpt [OPTIONS] partition-transcripts [arguments]',
-                          description=get_partition_transcripts_parser().description)
-
-    subparsers.add_parser('sum-signals', parents=[get_sum_signals_parser()], add_help=False,
-                          help=get_sum_signals_parser().description,
-                          usage='vpt [OPTIONS] sum-signals [arguments]',
-                          description=get_sum_signals_parser().description)
-
-    subparsers.add_parser('update-vzg', parents=[get_update_vzg_parser()], add_help=False,
-                          help=get_update_vzg_parser().description,
-                          usage='vpt [OPTIONS] update-vzg [arguments]',
-                          description=get_update_vzg_parser().description)
-
-    subparsers.add_parser('convert-geometry', parents=[get_convert_geometry_parser()], add_help=False,
-                          help=get_convert_geometry_parser().description,
-                          usage='vpt [OPTIONS] convert-geometry [arguments]',
-                          description=get_convert_geometry_parser().description)
-
-    subparsers.add_parser('convert-to-ome', parents=[get_convert_to_ome_parser()], add_help=False,
-                          help=get_convert_to_ome_parser().description,
-                          usage='vpt [OPTIONS] convert-to-ome [arguments]',
-                          description=get_convert_to_ome_parser().description)
-
-    subparsers.add_parser('convert-to-rgb-ome', parents=[get_convert_to_rgb_ome_parser()], add_help=False,
-                          help=get_convert_to_rgb_ome_parser().description,
-                          usage='vpt [OPTIONS] convert-to-rgb-ome [arguments]',
-                          description=get_convert_to_rgb_ome_parser().description)
-
-    return parser
-
-
-def get_cmd_entrypoint(cmd: str) -> Callable[[Namespace], None]:
-    subparsers = {
-        'run-segmentation': run_segmentation,
-        'prepare-segmentation': prepare_segmentation,
-        'run-segmentation-on-tile': run_segmentation_on_tile,
-        'compile-tile-segmentation': compile_tile_segmentation,
-        'convert-to-ome': convert_to_ome,
-        'convert-to-rgb-ome': convert_to_rgb_ome,
-        'derive-entity-metadata': derive_cell_metadata,
-        'update-vzg': update_vzg,
-        'sum-signals': run_sum_signals,
-        'partition-transcripts': partition_transcripts,
-        'convert-geometry': convert_geometry
-    }
-
-    if cmd not in subparsers.keys():
-        return lambda x: print(
-            "Command or option not recognized. Run 'vpt --help' for more information.")
-
-    return subparsers[cmd]
+from argparse import ArgumentParser, Namespace
+from typing import Callable
+
+from vpt.compile_tile_segmentation import get_parser as get_compile_tile_segmentation_parser, \
+    run as compile_tile_segmentation
+from vpt.convert_geometry import get_parser as get_convert_geometry_parser, run_conversion as convert_geometry
+from vpt.convert_to_ome import get_parser as get_convert_to_ome_parser, run_ome as convert_to_ome
+from vpt.convert_to_ome import get_parser_rgb as get_convert_to_rgb_ome_parser, run_ome_rgb as convert_to_rgb_ome
+from vpt.derive_cell_metadata import get_parser as get_derive_cell_metadata_parser, run as derive_cell_metadata
+from vpt.partition_transcripts import get_parser as get_partition_transcripts_parser, run as partition_transcripts
+from vpt.prepare_segmentation import get_parser as get_prepare_seg_parser, run as prepare_segmentation
+from vpt.run_segmentation import get_parser as get_run_segmentation_parser, run as run_segmentation
+from vpt.run_segmentation_on_tile import get_parser as get_run_seg_on_tile_parser, run as run_segmentation_on_tile
+from vpt.sum_signals import get_parser as get_sum_signals_parser, run as run_sum_signals
+from vpt.update_vzg import get_parser as get_update_vzg_parser, run as update_vzg
+
+
+def get_postprocess_parser() -> ArgumentParser:
+    parser = ArgumentParser(description='', usage='vpt [OPTIONS] COMMAND [arguments]', add_help=False,
+                            epilog="Run 'vpt COMMAND --help' for more information on a command.")
+    parser.add_argument('--processes', type=int, default=1, required=False,
+                        help='Number of parallel processes to use when executing locally')
+    parser.add_argument('--aws-profile-name', type=str, required=False,
+                        help="Named profile for AWS access")
+    parser.add_argument('--aws-access-key', type=str, required=False,
+                        help="AWS access key from key / secret pair")
+    parser.add_argument('--aws-secret-key', type=str, required=False,
+                        help="AWS secret from key / secret pair")
+    parser.add_argument('--gcs-service-account-key', type=str, required=False,
+                        help='Path to a google service account key json file. Not needed if google '
+                             'authentication is performed using gcloud')
+    parser.add_argument('--verbose', action='store_true', default=False, required=False,
+                        help='Display progress messages during execution')
+    parser.add_argument('--profile-execution-time', type=str, default=None, required=False,
+                        help='Path to profiler output file')
+    parser.add_argument('--log-level', type=int, default=1, required=False,
+                        help='Log level value. Level is specified as a number from 1 - 5, corresponding '
+                             'to debug, info, warning, error, crit')
+    parser.add_argument('--log-file', type=str, default=None, required=False,
+                        help='Path to log output file. If not provided, logs are written to standard output')
+    parser.add_argument("-h", "--help", action="help",
+                        help='Show this help message and exit')
+
+    parser._optionals.title = 'Options'
+    parser._positionals.title = 'Commands'
+
+    subparsers = parser.add_subparsers(dest='subparser_name', metavar='')
+
+    subparsers.add_parser('run-segmentation', parents=[get_run_segmentation_parser()], add_help=False,
+                          help=get_run_segmentation_parser().description,
+                          usage='vpt [OPTIONS] run-segmentation [arguments]',
+                          description=get_run_segmentation_parser().description)
+
+    subparsers.add_parser('prepare-segmentation', parents=[get_prepare_seg_parser()], add_help=False,
+                          help=get_prepare_seg_parser().description,
+                          usage='vpt [OPTIONS] prepare-segmentation [arguments]',
+                          description=get_prepare_seg_parser().description)
+
+    subparsers.add_parser('run-segmentation-on-tile', parents=[get_run_seg_on_tile_parser()], add_help=False,
+                          help=get_run_seg_on_tile_parser().description,
+                          usage='vpt [OPTIONS] run-segmentation-on-tile [arguments]',
+                          description=get_run_seg_on_tile_parser().description)
+
+    subparsers.add_parser('compile-tile-segmentation', parents=[get_compile_tile_segmentation_parser()], add_help=False,
+                          help=get_compile_tile_segmentation_parser().description,
+                          usage='vpt [OPTIONS] compile-tile-segmentation [arguments]',
+                          description=get_compile_tile_segmentation_parser().description)
+
+    subparsers.add_parser('derive-entity-metadata', parents=[get_derive_cell_metadata_parser()], add_help=False,
+                          help=get_derive_cell_metadata_parser().description,
+                          usage='vpt [OPTIONS] derive-entity-metadata [arguments]',
+                          description=get_derive_cell_metadata_parser().description)
+
+    subparsers.add_parser('partition-transcripts', parents=[get_partition_transcripts_parser()], add_help=False,
+                          help=get_partition_transcripts_parser().description,
+                          usage='vpt [OPTIONS] partition-transcripts [arguments]',
+                          description=get_partition_transcripts_parser().description)
+
+    subparsers.add_parser('sum-signals', parents=[get_sum_signals_parser()], add_help=False,
+                          help=get_sum_signals_parser().description,
+                          usage='vpt [OPTIONS] sum-signals [arguments]',
+                          description=get_sum_signals_parser().description)
+
+    subparsers.add_parser('update-vzg', parents=[get_update_vzg_parser()], add_help=False,
+                          help=get_update_vzg_parser().description,
+                          usage='vpt [OPTIONS] update-vzg [arguments]',
+                          description=get_update_vzg_parser().description)
+
+    subparsers.add_parser('convert-geometry', parents=[get_convert_geometry_parser()], add_help=False,
+                          help=get_convert_geometry_parser().description,
+                          usage='vpt [OPTIONS] convert-geometry [arguments]',
+                          description=get_convert_geometry_parser().description)
+
+    subparsers.add_parser('convert-to-ome', parents=[get_convert_to_ome_parser()], add_help=False,
+                          help=get_convert_to_ome_parser().description,
+                          usage='vpt [OPTIONS] convert-to-ome [arguments]',
+                          description=get_convert_to_ome_parser().description)
+
+    subparsers.add_parser('convert-to-rgb-ome', parents=[get_convert_to_rgb_ome_parser()], add_help=False,
+                          help=get_convert_to_rgb_ome_parser().description,
+                          usage='vpt [OPTIONS] convert-to-rgb-ome [arguments]',
+                          description=get_convert_to_rgb_ome_parser().description)
+
+    return parser
+
+
+def get_cmd_entrypoint(cmd: str) -> Callable[[Namespace], None]:
+    subparsers = {
+        'run-segmentation': run_segmentation,
+        'prepare-segmentation': prepare_segmentation,
+        'run-segmentation-on-tile': run_segmentation_on_tile,
+        'compile-tile-segmentation': compile_tile_segmentation,
+        'convert-to-ome': convert_to_ome,
+        'convert-to-rgb-ome': convert_to_rgb_ome,
+        'derive-entity-metadata': derive_cell_metadata,
+        'update-vzg': update_vzg,
+        'sum-signals': run_sum_signals,
+        'partition-transcripts': partition_transcripts,
+        'convert-geometry': convert_geometry
+    }
+
+    if cmd not in subparsers.keys():
+        return lambda x: print(
+            "Command or option not recognized. Run 'vpt --help' for more information.")
+
+    return subparsers[cmd]
```

### Comparing `vpt-1.0.1/src/vpt/compile_tile_segmentation/cmd_args.py` & `vpt-1.0.2/src/vpt/compile_tile_segmentation/cmd_args.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-from argparse import ArgumentParser
-from dataclasses import dataclass
-
-from vpt.utils.output_tools import MIN_ROW_GROUP_SIZE
-from vpt.utils.validate import validate_exists
-
-
-@dataclass
-class CompileTileSegmentationArgs:
-    parameters_json_path: str
-    max_row_group_size: int
-    overwrite: bool
-
-
-def validate_cmd_args(args: CompileTileSegmentationArgs):
-    validate_exists(args.parameters_json_path)
-    if args.max_row_group_size < MIN_ROW_GROUP_SIZE:
-        raise ValueError(f'Row group size should be at least {MIN_ROW_GROUP_SIZE}')
-
-
-def get_parser():
-    parser = ArgumentParser(description='Combines the per-tile segmentation outputs into a single, internally-consistent '
-                            'parquet file containing all of the segmentation boundaries found in the experiment.',
-                            add_help=False
-                            )
-    required = parser.add_argument_group('Required arguments')
-    required.add_argument('--input-segmentation-parameters', type=str, required=True,
-                          help='Json file generated by prepare-segmentation that fully '
-                               'specifies the segmentation to run.')
-
-    opt = parser.add_argument_group('Optional arguments')
-    opt.add_argument('--max-row-group-size', type=int, default=17500, required=False,
-                     help='Maximum number of rows in row groups inside output parquet files. Cannot be less '
-                          f'than {MIN_ROW_GROUP_SIZE}')
-    opt.add_argument('--overwrite', action='store_true', default=False, required=False,
-                     help='Set flag if you want to use non empty directory and agree that files can be over-written.')
-    opt.add_argument("--help", action="help", help="Show this help message and exit")
-
-    return parser
-
-
-def parse_cmd_args():
-    return get_parser().parse_args()
+from argparse import ArgumentParser
+from dataclasses import dataclass
+
+from vpt.utils.output_tools import MIN_ROW_GROUP_SIZE
+from vpt.utils.validate import validate_exists
+
+
+@dataclass
+class CompileTileSegmentationArgs:
+    parameters_json_path: str
+    max_row_group_size: int
+    overwrite: bool
+
+
+def validate_cmd_args(args: CompileTileSegmentationArgs):
+    validate_exists(args.parameters_json_path)
+    if args.max_row_group_size < MIN_ROW_GROUP_SIZE:
+        raise ValueError(f'Row group size should be at least {MIN_ROW_GROUP_SIZE}')
+
+
+def get_parser():
+    parser = ArgumentParser(description='Combines the per-tile segmentation outputs into a single, internally-consistent '
+                            'parquet file containing all of the segmentation boundaries found in the experiment.',
+                            add_help=False
+                            )
+    required = parser.add_argument_group('Required arguments')
+    required.add_argument('--input-segmentation-parameters', type=str, required=True,
+                          help='Json file generated by prepare-segmentation that fully '
+                               'specifies the segmentation to run.')
+
+    opt = parser.add_argument_group('Optional arguments')
+    opt.add_argument('--max-row-group-size', type=int, default=17500, required=False,
+                     help='Maximum number of rows in row groups inside output parquet files. Cannot be less '
+                          f'than {MIN_ROW_GROUP_SIZE}')
+    opt.add_argument('--overwrite', action='store_true', default=False, required=False,
+                     help='Set flag if you want to use non empty directory and agree that files can be over-written.')
+    opt.add_argument("--help", action="help", help="Show this help message and exit")
+
+    return parser
+
+
+def parse_cmd_args():
+    return get_parser().parse_args()
```

### Comparing `vpt-1.0.1/src/vpt/compile_tile_segmentation/main.py` & `vpt-1.0.2/src/vpt/compile_tile_segmentation/main.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,96 +1,96 @@
-import json
-import warnings
-from typing import Callable
-
-import geopandas as gpd
-import numpy as np
-
-import vpt.log as log
-from vpt.compile_tile_segmentation.cmd_args import parse_cmd_args, CompileTileSegmentationArgs, validate_cmd_args
-from vpt.compile_tile_segmentation.parameters import CompileParameters, IOPaths, extract_parameters_from_spec
-from vpt.filesystem.vzgfs import filesystem_path_split, initialize_filesystem, vzg_open
-from vpt.run_segmentation_on_tile.output_utils import make_output_filename
-from vpt.segmentation.utils.seg_result import SegmentationResult
-from vpt.utils.output_tools import save_segmentation_results
-from vpt.utils.validate import validate_does_not_exist
-
-AdapterType = Callable[[int], SegmentationResult]
-
-
-def compile_dataframe(get_tile_results: AdapterType, params: CompileParameters) -> SegmentationResult:
-    seg_list = []
-
-    log.info('Loading segmentation results')
-
-    for tile_index in log.show_progress(range(params.num_tiles)):
-        gdf = get_tile_results(tile_index)
-        seg_list.append(gdf)
-    log.info(f'Loaded results for {params.num_tiles} tiles')
-
-    seg_compiled = SegmentationResult.combine_segmentations(seg_list)
-    log.info('Concatenated dataframes')
-
-    mosaic_to_micron = np.linalg.inv(params.micron_to_mosaic_matrix)
-    x_scale, y_scale = mosaic_to_micron[0, 0], mosaic_to_micron[1, 1]
-
-    min_final_area = params.min_final_area * x_scale * y_scale
-    min_distance = params.min_distance * x_scale
-
-    seg_compiled.make_non_overlapping_polys(min_distance, min_final_area, log_progress=True)
-    seg_compiled.set_column(SegmentationResult.detection_id_field, np.arange(len(seg_compiled.df), dtype=np.int64))
-
-    log.info('Resolved overlapping in the compiled dataframe')
-    return seg_compiled
-
-
-def adapter_from_paths(paths: IOPaths) -> AdapterType:
-    fs, input_dir = filesystem_path_split(paths.input_dir)
-
-    def read(tile_index: int) -> SegmentationResult:
-        path = fs.sep.join([input_dir, make_output_filename(tile_index)])
-
-        result = None
-
-        with fs.open(path, 'rb') as f:
-            result = SegmentationResult(dataframe=gpd.read_parquet(f))
-
-        return result
-
-    return read
-
-
-def compile_tile_segmentation(args):
-    # Suppress parquet / Arrow warnings
-    warnings.filterwarnings('ignore', category=UserWarning)
-
-    args = CompileTileSegmentationArgs(args.input_segmentation_parameters, args.max_row_group_size, args.overwrite)
-    validate_cmd_args(args)
-    log.info('Compile tile segmentation started')
-
-    with vzg_open(args.parameters_json_path, 'r') as f:
-        spec_raw = json.load(f)
-
-    etype_to_paths, params = extract_parameters_from_spec(spec_raw)
-
-    if not args.overwrite:
-        for _, io_paths in etype_to_paths.items():
-            validate_does_not_exist(io_paths.micron_output_file)
-            validate_does_not_exist(io_paths.mosaic_output_file)
-
-    for entity_type, io_paths in etype_to_paths.items():
-        compiled = compile_dataframe(adapter_from_paths(io_paths), params)
-
-        save_segmentation_results(compiled.df, io_paths.micron_output_file, args.max_row_group_size)
-        log.info('Saved compiled dataframe in micron space')
-
-        compiled.transform_geoms(params.micron_to_mosaic_matrix)
-
-        save_segmentation_results(compiled.df, io_paths.mosaic_output_file, args.max_row_group_size)
-        log.info('Saved compiled dataframe in mosaic space')
-
-    log.info('Compile tile segmentation finished')
-
-
-if __name__ == '__main__':
-    initialize_filesystem()
-    compile_tile_segmentation(parse_cmd_args())
+import json
+import warnings
+from typing import Callable
+
+import geopandas as gpd
+import numpy as np
+
+import vpt.log as log
+from vpt.compile_tile_segmentation.cmd_args import parse_cmd_args, CompileTileSegmentationArgs, validate_cmd_args
+from vpt.compile_tile_segmentation.parameters import CompileParameters, IOPaths, extract_parameters_from_spec
+from vpt.filesystem.vzgfs import filesystem_path_split, initialize_filesystem, vzg_open
+from vpt.run_segmentation_on_tile.output_utils import make_output_filename
+from vpt.segmentation.utils.seg_result import SegmentationResult
+from vpt.utils.output_tools import save_segmentation_results
+from vpt.utils.validate import validate_does_not_exist
+
+AdapterType = Callable[[int], SegmentationResult]
+
+
+def compile_dataframe(get_tile_results: AdapterType, params: CompileParameters) -> SegmentationResult:
+    seg_list = []
+
+    log.info('Loading segmentation results')
+
+    for tile_index in log.show_progress(range(params.num_tiles)):
+        gdf = get_tile_results(tile_index)
+        seg_list.append(gdf)
+    log.info(f'Loaded results for {params.num_tiles} tiles')
+
+    seg_compiled = SegmentationResult.combine_segmentations(seg_list)
+    log.info('Concatenated dataframes')
+
+    mosaic_to_micron = np.linalg.inv(params.micron_to_mosaic_matrix)
+    x_scale, y_scale = mosaic_to_micron[0, 0], mosaic_to_micron[1, 1]
+
+    min_final_area = params.min_final_area * x_scale * y_scale
+    min_distance = params.min_distance * x_scale
+
+    seg_compiled.make_non_overlapping_polys(min_distance, min_final_area, log_progress=True)
+    seg_compiled.set_column(SegmentationResult.detection_id_field, np.arange(len(seg_compiled.df), dtype=np.int64))
+
+    log.info('Resolved overlapping in the compiled dataframe')
+    return seg_compiled
+
+
+def adapter_from_paths(paths: IOPaths) -> AdapterType:
+    fs, input_dir = filesystem_path_split(paths.input_dir)
+
+    def read(tile_index: int) -> SegmentationResult:
+        path = fs.sep.join([input_dir, make_output_filename(tile_index)])
+
+        result = None
+
+        with fs.open(path, 'rb') as f:
+            result = SegmentationResult(dataframe=gpd.read_parquet(f))
+
+        return result
+
+    return read
+
+
+def compile_tile_segmentation(args):
+    # Suppress parquet / Arrow warnings
+    warnings.filterwarnings('ignore', category=UserWarning)
+
+    args = CompileTileSegmentationArgs(args.input_segmentation_parameters, args.max_row_group_size, args.overwrite)
+    validate_cmd_args(args)
+    log.info('Compile tile segmentation started')
+
+    with vzg_open(args.parameters_json_path, 'r') as f:
+        spec_raw = json.load(f)
+
+    etype_to_paths, params = extract_parameters_from_spec(spec_raw)
+
+    if not args.overwrite:
+        for _, io_paths in etype_to_paths.items():
+            validate_does_not_exist(io_paths.micron_output_file)
+            validate_does_not_exist(io_paths.mosaic_output_file)
+
+    for entity_type, io_paths in etype_to_paths.items():
+        compiled = compile_dataframe(adapter_from_paths(io_paths), params)
+
+        save_segmentation_results(compiled.df, io_paths.micron_output_file, args.max_row_group_size)
+        log.info('Saved compiled dataframe in micron space')
+
+        compiled.transform_geoms(params.micron_to_mosaic_matrix)
+
+        save_segmentation_results(compiled.df, io_paths.mosaic_output_file, args.max_row_group_size)
+        log.info('Saved compiled dataframe in mosaic space')
+
+    log.info('Compile tile segmentation finished')
+
+
+if __name__ == '__main__':
+    initialize_filesystem()
+    compile_tile_segmentation(parse_cmd_args())
```

### Comparing `vpt-1.0.1/src/vpt/compile_tile_segmentation/parameters.py` & `vpt-1.0.2/src/vpt/compile_tile_segmentation/parameters.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-from dataclasses import dataclass
-from typing import Dict, Tuple
-
-import numpy as np
-
-from vpt.filesystem.vzgfs import filesystem_path_split
-
-
-@dataclass
-class IOPaths:
-    input_dir: str
-    mosaic_output_file: str
-    micron_output_file: str
-
-
-@dataclass
-class CompileParameters:
-    num_tiles: int
-    micron_to_mosaic_matrix: np.ndarray
-    min_final_area: int
-    min_distance: int
-
-
-def extract_parameters_from_spec(spec: Dict) -> Tuple[Dict[str, IOPaths], CompileParameters]:
-    output_root = spec['input_args']['output_path']
-    output_fs, _ = filesystem_path_split(output_root)
-
-    num_tiles = spec['window_grid']['num_tiles']
-
-    entity_type_to_paths_mapping = {
-        entity_type: IOPaths(input_dir=output_fs.sep.join([output_root, record['files']['run_on_tile_dir']]),
-                             mosaic_output_file=output_fs.sep.join(
-                                 [output_root, record['files']['mosaic_geometry_file']]),
-                             micron_output_file=output_fs.sep.join(
-                                 [output_root, record['files']['micron_geometry_file']]))
-        for record in spec['segmentation_algorithm']['output_files'] for entity_type in record['entity_types_output']
-    }
-    m2m_tform = np.array(spec['input_data']['micron_to_mosaic_tform'])
-    polys_postprocessing = spec['segmentation_algorithm']['segmentation_task_fusion']
-    polys_postprocessing = polys_postprocessing['fused_polygon_postprocessing_parameters']
-    min_area = polys_postprocessing['min_final_area']
-    min_distance = polys_postprocessing['min_distance_between_entities']
-
-    return entity_type_to_paths_mapping, CompileParameters(num_tiles, m2m_tform, min_area, min_distance)
+from dataclasses import dataclass
+from typing import Dict, Tuple
+
+import numpy as np
+
+from vpt.filesystem.vzgfs import filesystem_path_split
+
+
+@dataclass
+class IOPaths:
+    input_dir: str
+    mosaic_output_file: str
+    micron_output_file: str
+
+
+@dataclass
+class CompileParameters:
+    num_tiles: int
+    micron_to_mosaic_matrix: np.ndarray
+    min_final_area: int
+    min_distance: int
+
+
+def extract_parameters_from_spec(spec: Dict) -> Tuple[Dict[str, IOPaths], CompileParameters]:
+    output_root = spec['input_args']['output_path']
+    output_fs, _ = filesystem_path_split(output_root)
+
+    num_tiles = spec['window_grid']['num_tiles']
+
+    entity_type_to_paths_mapping = {
+        entity_type: IOPaths(input_dir=output_fs.sep.join([output_root, record['files']['run_on_tile_dir']]),
+                             mosaic_output_file=output_fs.sep.join(
+                                 [output_root, record['files']['mosaic_geometry_file']]),
+                             micron_output_file=output_fs.sep.join(
+                                 [output_root, record['files']['micron_geometry_file']]))
+        for record in spec['segmentation_algorithm']['output_files'] for entity_type in record['entity_types_output']
+    }
+    m2m_tform = np.array(spec['input_data']['micron_to_mosaic_tform'])
+    polys_postprocessing = spec['segmentation_algorithm']['segmentation_task_fusion']
+    polys_postprocessing = polys_postprocessing['fused_polygon_postprocessing_parameters']
+    min_area = polys_postprocessing['min_final_area']
+    min_distance = polys_postprocessing['min_distance_between_entities']
+
+    return entity_type_to_paths_mapping, CompileParameters(num_tiles, m2m_tform, min_area, min_distance)
```

### Comparing `vpt-1.0.1/src/vpt/convert_geometry/cmd_args.py` & `vpt-1.0.2/src/vpt/convert_geometry/cmd_args.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,112 +1,112 @@
-from argparse import ArgumentParser
-from dataclasses import dataclass
-from typing import Optional
-
-from vpt.convert_geometry.factory import get_conversion_type, SegmentationFileType
-from vpt.filesystem import filesystem_path_split
-from vpt.utils.output_tools import MIN_ROW_GROUP_SIZE
-from vpt.utils.validate import validate_does_not_exist
-
-
-@dataclass
-class ConvertGeometryArgs:
-    input_boundaries: str
-    output_boundaries: str
-    convert_to_3D: bool
-    number_z_planes: Optional[int]
-    spacing_z_planes: Optional[float]
-    output_entity_type: str
-    entity_fusion_strategy: str
-    id_mapping_file: str
-    max_row_group_size: int
-    overwrite: bool
-
-
-def validate_args_with_input(args: ConvertGeometryArgs, input_path: str):
-    input_type = get_conversion_type(input_path)
-    if input_type in [SegmentationFileType.QPATH, SegmentationFileType.PARQUET]:
-        if args.convert_to_3D:
-            if args.number_z_planes is None or args.spacing_z_planes is None:
-                raise ValueError('To convert 2D segmentation to 3D parquet segmentation the number of z planes '
-                                 'and spacing between them should be specified')
-            elif args.number_z_planes <= 0:
-                raise ValueError('The number of z planes should be positive integer')
-            elif args.spacing_z_planes <= 0:
-                raise ValueError('The spacing between z planes should be positive')
-        else:
-            if args.number_z_planes is not None or args.spacing_z_planes is not None:
-                raise ValueError('Number of z planes and spacing can be specified only if "--convert-to-3D" argument '
-                                 'is passed')
-
-    elif input_type == SegmentationFileType.HDF5:
-        if args.convert_to_3D or args.number_z_planes is not None or args.spacing_z_planes is not None:
-            raise ValueError('The conversion from 2D hdf5 segmentation to 3D parquet segmentation is not supported')
-    else:
-        raise ValueError('Type of the passed input file is not supported')
-
-
-def validate_cmd_args(args: ConvertGeometryArgs):
-    if not args.overwrite:
-        validate_does_not_exist(args.output_boundaries)
-        if args.id_mapping_file:
-            validate_does_not_exist(args.id_mapping_file)
-
-    fs, path_inside_fs = filesystem_path_split(args.output_boundaries)
-    if fs.exists(path_inside_fs) and not fs.isfile(path_inside_fs):
-        raise ValueError('Provided path should be a file')
-
-    if args.max_row_group_size < MIN_ROW_GROUP_SIZE:
-        raise ValueError(f'Row group size should be at least {MIN_ROW_GROUP_SIZE}')
-
-    if args.id_mapping_file:
-        fs, path_inside_fs = filesystem_path_split(args.id_mapping_file)
-        if fs.exists(path_inside_fs) and not fs.isfile(path_inside_fs):
-            raise ValueError('Provided path should be a file')
-
-
-def get_parser():
-    parser = ArgumentParser(description='Converts entity boundaries produced by a different tool into a '
-                            'vpt compatible parquet file. In the process, each of the input'
-                            ' entities is checked for geometric validity, overlap with'
-                            ' other geometries, and assigned a globally-unique EntityID '
-                            'to facilitate other processing steps.',
-                            add_help=False
-                            )
-
-    required = parser.add_argument_group('Required arguments')
-    required.add_argument('--input-boundaries', type=str, required=True,
-                          help='Regular expression that matches all input segmentation files (geojson or hdf5) that '
-                               'will be processed.')
-    required.add_argument('--output-boundaries', type=str, required=True,
-                          help='The path to the parquet file where segmentation compatible with vpt will be saved.')
-
-    opt = parser.add_argument_group('Optional arguments')
-    opt.add_argument('--convert-to-3D', action='store_true', default=False, required=False,
-                     help='Pass if segmentation should be converted from 2D to 3D by replication. Only possible for '
-                          'geojson and parquet input formats.')
-    opt.add_argument('--number-z-planes', type=int, default=None, required=False,
-                     help='The number of z planes that should be produced during the conversion from 2D to 3D. Should '
-                          'be specified only if the "--convert-to-3D" argument is passed')
-    opt.add_argument('--spacing-z-planes', type=float, default=None, required=False,
-                     help='Step size between z-planes, assuming that z-index 0 is 1 “step” above zero. Should be '
-                          'specified only if the "--convert-to-3D" argument is passed')
-    opt.add_argument('--output-entity-type', type=str, default='cell',
-                     help='String with entity type name. For example: cell, nuclei. Default: cell')
-    opt.add_argument('--id-mapping-file', type=str, required=False,
-                     help='Path to csv file where map from source segmentation entity id to EntityID in result '
-                          'will be saved.')
-    opt.add_argument('--entity-fusion-strategy', type=str, default='harmonize',
-                     help='String with entity fusion strategy name. One from list: harmonize, union, larger. '
-                          'Default: harmonize')
-    opt.add_argument('--max-row-group-size', type=int, default=17500, required=False,
-                     help=f'Maximum number of rows in row groups inside output parquet files. Cannot be less '
-                          f'than {MIN_ROW_GROUP_SIZE}')
-    opt.add_argument('--overwrite', action='store_true', default=False, required=False,
-                     help='Set flag if you want to use non empty directory and agree that files can be over-written.')
-    opt.add_argument("-h", "--help", action="help", help="Show this help message and exit")
-
-    return parser
-
-
-def parse_cmd_args():
-    return get_parser().parse_args()
+from argparse import ArgumentParser
+from dataclasses import dataclass
+from typing import Optional
+
+from vpt.convert_geometry.factory import get_conversion_type, SegmentationFileType
+from vpt.filesystem import filesystem_path_split
+from vpt.utils.output_tools import MIN_ROW_GROUP_SIZE
+from vpt.utils.validate import validate_does_not_exist
+
+
+@dataclass
+class ConvertGeometryArgs:
+    input_boundaries: str
+    output_boundaries: str
+    convert_to_3D: bool
+    number_z_planes: Optional[int]
+    spacing_z_planes: Optional[float]
+    output_entity_type: str
+    entity_fusion_strategy: str
+    id_mapping_file: str
+    max_row_group_size: int
+    overwrite: bool
+
+
+def validate_args_with_input(args: ConvertGeometryArgs, input_path: str):
+    input_type = get_conversion_type(input_path)
+    if input_type in [SegmentationFileType.QPATH, SegmentationFileType.PARQUET]:
+        if args.convert_to_3D:
+            if args.number_z_planes is None or args.spacing_z_planes is None:
+                raise ValueError('To convert 2D segmentation to 3D parquet segmentation the number of z planes '
+                                 'and spacing between them should be specified')
+            elif args.number_z_planes <= 0:
+                raise ValueError('The number of z planes should be positive integer')
+            elif args.spacing_z_planes <= 0:
+                raise ValueError('The spacing between z planes should be positive')
+        else:
+            if args.number_z_planes is not None or args.spacing_z_planes is not None:
+                raise ValueError('Number of z planes and spacing can be specified only if "--convert-to-3D" argument '
+                                 'is passed')
+
+    elif input_type == SegmentationFileType.HDF5:
+        if args.convert_to_3D or args.number_z_planes is not None or args.spacing_z_planes is not None:
+            raise ValueError('The conversion from 2D hdf5 segmentation to 3D parquet segmentation is not supported')
+    else:
+        raise ValueError('Type of the passed input file is not supported')
+
+
+def validate_cmd_args(args: ConvertGeometryArgs):
+    if not args.overwrite:
+        validate_does_not_exist(args.output_boundaries)
+        if args.id_mapping_file:
+            validate_does_not_exist(args.id_mapping_file)
+
+    fs, path_inside_fs = filesystem_path_split(args.output_boundaries)
+    if fs.exists(path_inside_fs) and not fs.isfile(path_inside_fs):
+        raise ValueError('Provided path should be a file')
+
+    if args.max_row_group_size < MIN_ROW_GROUP_SIZE:
+        raise ValueError(f'Row group size should be at least {MIN_ROW_GROUP_SIZE}')
+
+    if args.id_mapping_file:
+        fs, path_inside_fs = filesystem_path_split(args.id_mapping_file)
+        if fs.exists(path_inside_fs) and not fs.isfile(path_inside_fs):
+            raise ValueError('Provided path should be a file')
+
+
+def get_parser():
+    parser = ArgumentParser(description='Converts entity boundaries produced by a different tool into a '
+                            'vpt compatible parquet file. In the process, each of the input'
+                            ' entities is checked for geometric validity, overlap with'
+                            ' other geometries, and assigned a globally-unique EntityID '
+                            'to facilitate other processing steps.',
+                            add_help=False
+                            )
+
+    required = parser.add_argument_group('Required arguments')
+    required.add_argument('--input-boundaries', type=str, required=True,
+                          help='Regular expression that matches all input segmentation files (geojson or hdf5) that '
+                               'will be processed.')
+    required.add_argument('--output-boundaries', type=str, required=True,
+                          help='The path to the parquet file where segmentation compatible with vpt will be saved.')
+
+    opt = parser.add_argument_group('Optional arguments')
+    opt.add_argument('--convert-to-3D', action='store_true', default=False, required=False,
+                     help='Pass if segmentation should be converted from 2D to 3D by replication. Only possible for '
+                          'geojson and parquet input formats.')
+    opt.add_argument('--number-z-planes', type=int, default=None, required=False,
+                     help='The number of z planes that should be produced during the conversion from 2D to 3D. Should '
+                          'be specified only if the "--convert-to-3D" argument is passed')
+    opt.add_argument('--spacing-z-planes', type=float, default=None, required=False,
+                     help='Step size between z-planes, assuming that z-index 0 is 1 “step” above zero. Should be '
+                          'specified only if the "--convert-to-3D" argument is passed')
+    opt.add_argument('--output-entity-type', type=str, default='cell',
+                     help='String with entity type name. For example: cell, nuclei. Default: cell')
+    opt.add_argument('--id-mapping-file', type=str, required=False,
+                     help='Path to csv file where map from source segmentation entity id to EntityID in result '
+                          'will be saved.')
+    opt.add_argument('--entity-fusion-strategy', type=str, default='harmonize',
+                     help='String with entity fusion strategy name. One from list: harmonize, union, larger. '
+                          'Default: harmonize')
+    opt.add_argument('--max-row-group-size', type=int, default=17500, required=False,
+                     help=f'Maximum number of rows in row groups inside output parquet files. Cannot be less '
+                          f'than {MIN_ROW_GROUP_SIZE}')
+    opt.add_argument('--overwrite', action='store_true', default=False, required=False,
+                     help='Set flag if you want to use non empty directory and agree that files can be over-written.')
+    opt.add_argument("-h", "--help", action="help", help="Show this help message and exit")
+
+    return parser
+
+
+def parse_cmd_args():
+    return get_parser().parse_args()
```

### Comparing `vpt-1.0.1/src/vpt/convert_geometry/converters/hdf5_converter.py` & `vpt-1.0.2/src/vpt/convert_geometry/converters/hdf5_converter.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,73 +1,73 @@
-from typing import Tuple, Dict
-
-import h5py
-import numpy as np
-from h5py import Group
-from shapely import geometry
-from shapely.validation import make_valid
-
-from vpt.convert_geometry.converters.entity_id_generator import set_process_id, get_id
-from vpt.filesystem import vzg_open
-from vpt.segmentation.utils.polygon_utils import convert_to_multipoly
-from vpt.segmentation.utils.seg_result import SegmentationResult
-
-
-def read_segmentation_result(input_path: str, entity_type: str) -> Tuple[SegmentationResult, Dict]:
-    set_process_id()
-    entity_ids_map = {}
-    segmentations = []
-    try:
-        with vzg_open(input_path, 'rb') as f:
-            h = h5py.File(f, 'r')
-            group = h.require_group('featuredata')
-            for k in group.keys():
-                entity_id = get_id()
-                segmentations.append(load_feature_from_hdf5_group(group[k], entity_id))
-                entity_ids_map[group[k].attrs['id']] = entity_id
-    except Exception as err:
-        raise ValueError(f'Hdf5 file structure is wrong and is not compatible with '
-                         f'merlin output hdf5 segmentation. {err}')
-    res = SegmentationResult.combine_segmentations(segmentations)
-    res.set_entity_type(entity_type)
-    res.set_column(SegmentationResult.entity_name_field, res.entity_type)
-
-    set_none = ['Name', 'ParentID', 'ParentType']
-    for column_name in set_none:
-        res.set_column(column_name, None)
-    return res, entity_ids_map
-
-
-def load_geometry_from_hdf5_group(h5Group: Group):
-    geometry_params = {'type': h5Group.attrs['type'].decode(),
-                       'coordinates': np.array(h5Group['coordinates'])}
-    return convert_to_multipoly(make_valid(geometry.shape(geometry_params)))
-
-
-def load_feature_from_hdf5_group(h5Group: Group, cell_id: np.int64):
-    zCount = len([x for x in h5Group.keys() if x.startswith('zIndex_')])
-    polys_data = []
-    idx = 0
-    for z in range(zCount):
-        zGroup = h5Group['zIndex_' + str(z)]
-        pCount = len([x for x in zGroup.keys() if x[:2] == 'p_'])
-        if pCount == 0:
-            continue
-        multipolys = [load_geometry_from_hdf5_group(zGroup['p_' + str(p)]) for p in range(pCount)]
-        multipoly: geometry.MultiPolygon = multipolys[0]
-        for poly in multipolys[1:]:
-            multipoly = convert_to_multipoly(make_valid(multipoly.union(poly)))
-
-        polys_data.append(
-            {
-                SegmentationResult.detection_id_field: idx,
-                SegmentationResult.cell_id_field: cell_id,
-                SegmentationResult.z_index_field: z,
-                SegmentationResult.geometry_field: multipoly,
-                'ZLevel': h5Group['z_coordinates'][z]
-            }
-        )
-        idx += 1
-    seg_res = SegmentationResult(list_data=polys_data)
-    seg_res.set_column('ZLevel', seg_res.df[SegmentationResult.z_index_field])
-    seg_res.update_column('ZLevel', lambda x: h5Group['z_coordinates'][x])
-    return seg_res
+from typing import Tuple, Dict
+
+import h5py
+import numpy as np
+from h5py import Group
+from shapely import geometry
+from shapely.validation import make_valid
+
+from vpt.convert_geometry.converters.entity_id_generator import set_process_id, get_id
+from vpt.filesystem import vzg_open
+from vpt.segmentation.utils.polygon_utils import convert_to_multipoly
+from vpt.segmentation.utils.seg_result import SegmentationResult
+
+
+def read_segmentation_result(input_path: str, entity_type: str) -> Tuple[SegmentationResult, Dict]:
+    set_process_id()
+    entity_ids_map = {}
+    segmentations = []
+    try:
+        with vzg_open(input_path, 'rb') as f:
+            h = h5py.File(f, 'r')
+            group = h.require_group('featuredata')
+            for k in group.keys():
+                entity_id = get_id()
+                segmentations.append(load_feature_from_hdf5_group(group[k], entity_id))
+                entity_ids_map[group[k].attrs['id']] = entity_id
+    except Exception as err:
+        raise ValueError(f'Hdf5 file structure is wrong and is not compatible with '
+                         f'merlin output hdf5 segmentation. {err}')
+    res = SegmentationResult.combine_segmentations(segmentations)
+    res.set_entity_type(entity_type)
+    res.set_column(SegmentationResult.entity_name_field, res.entity_type)
+
+    set_none = ['Name', 'ParentID', 'ParentType']
+    for column_name in set_none:
+        res.set_column(column_name, None)
+    return res, entity_ids_map
+
+
+def load_geometry_from_hdf5_group(h5Group: Group):
+    geometry_params = {'type': h5Group.attrs['type'].decode(),
+                       'coordinates': np.array(h5Group['coordinates'])}
+    return convert_to_multipoly(make_valid(geometry.shape(geometry_params)))
+
+
+def load_feature_from_hdf5_group(h5Group: Group, cell_id: np.int64):
+    zCount = len([x for x in h5Group.keys() if x.startswith('zIndex_')])
+    polys_data = []
+    idx = 0
+    for z in range(zCount):
+        zGroup = h5Group['zIndex_' + str(z)]
+        pCount = len([x for x in zGroup.keys() if x[:2] == 'p_'])
+        if pCount == 0:
+            continue
+        multipolys = [load_geometry_from_hdf5_group(zGroup['p_' + str(p)]) for p in range(pCount)]
+        multipoly: geometry.MultiPolygon = multipolys[0]
+        for poly in multipolys[1:]:
+            multipoly = convert_to_multipoly(make_valid(multipoly.union(poly)))
+
+        polys_data.append(
+            {
+                SegmentationResult.detection_id_field: idx,
+                SegmentationResult.cell_id_field: cell_id,
+                SegmentationResult.z_index_field: z,
+                SegmentationResult.geometry_field: multipoly,
+                'ZLevel': h5Group['z_coordinates'][z]
+            }
+        )
+        idx += 1
+    seg_res = SegmentationResult(list_data=polys_data)
+    seg_res.set_column('ZLevel', seg_res.df[SegmentationResult.z_index_field])
+    seg_res.update_column('ZLevel', lambda x: h5Group['z_coordinates'][x])
+    return seg_res
```

### Comparing `vpt-1.0.1/src/vpt/convert_geometry/converters/old_parquet_converter.py` & `vpt-1.0.2/src/vpt/convert_geometry/converters/old_parquet_converter.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-from typing import Tuple, Dict
-
-import geopandas as gpd
-
-from vpt.convert_geometry.converters.entity_id_generator import set_process_id, get_id
-from vpt.filesystem import vzg_open
-from vpt.segmentation.utils.seg_result import SegmentationResult
-
-
-def read_segmentation_result(input_path: str, entity_type: str, z_planes_number: int = 0,
-                             spacing: float = 1.5) -> Tuple[SegmentationResult, Dict]:
-    set_process_id()
-    with vzg_open(input_path, 'rb') as f:
-        pq = gpd.read_parquet(f)
-
-    if SegmentationResult.cell_id_field not in pq.columns:
-        pq = pq.assign(**{SegmentationResult.cell_id_field: list(range(len(pq)))})
-    entity_ids_map = {i: get_id() for i in pq[SegmentationResult.cell_id_field].unique()}
-
-    seg_res = SegmentationResult(dataframe=pq)
-    seg_res.update_column(SegmentationResult.cell_id_field, entity_ids_map.get)
-
-    seg_res.set_entity_type(entity_type)
-    if seg_res.entity_name_field not in seg_res.df.columns:
-        seg_res.set_column(SegmentationResult.entity_name_field, entity_type)
-
-    if seg_res.detection_id_field not in seg_res.df.columns:
-        seg_res.set_column(SegmentationResult.detection_id_field, list(range(len(pq))))
-
-    if seg_res.z_index_field not in seg_res.df.columns:
-        seg_res.set_column(SegmentationResult.z_index_field, 0)
-
-    if z_planes_number > 0:
-        if len(seg_res.df[seg_res.z_index_field].unique()) > 1:
-            raise ValueError('The input segmentation is already 3D. The conversion to 3D only possible for 2D '
-                             'segmentation')
-
-        z_planes = list(range(z_planes_number))
-        if not set(z_planes).issuperset(seg_res.df[seg_res.z_index_field].unique()):
-            raise ValueError('The z plane set of the input segmentation should be a subset of the requested set of '
-                             'output z planes')
-
-        seg_res.replicate_across_z(z_planes)
-        seg_res.set_z_levels([spacing + (x * spacing) for x in z_planes], 'ZLevel')
-
-    set_none = ['Name', 'ParentID', 'ParentType']
-    for column_name in set_none:
-        if column_name not in seg_res.df:
-            seg_res.set_column(column_name, None)
-    return seg_res, entity_ids_map
+from typing import Tuple, Dict
+
+import geopandas as gpd
+
+from vpt.convert_geometry.converters.entity_id_generator import set_process_id, get_id
+from vpt.filesystem import vzg_open
+from vpt.segmentation.utils.seg_result import SegmentationResult
+
+
+def read_segmentation_result(input_path: str, entity_type: str, z_planes_number: int = 0,
+                             spacing: float = 1.5) -> Tuple[SegmentationResult, Dict]:
+    set_process_id()
+    with vzg_open(input_path, 'rb') as f:
+        pq = gpd.read_parquet(f)
+
+    if SegmentationResult.cell_id_field not in pq.columns:
+        pq = pq.assign(**{SegmentationResult.cell_id_field: list(range(len(pq)))})
+    entity_ids_map = {i: get_id() for i in pq[SegmentationResult.cell_id_field].unique()}
+
+    seg_res = SegmentationResult(dataframe=pq)
+    seg_res.update_column(SegmentationResult.cell_id_field, entity_ids_map.get)
+
+    seg_res.set_entity_type(entity_type)
+    if seg_res.entity_name_field not in seg_res.df.columns:
+        seg_res.set_column(SegmentationResult.entity_name_field, entity_type)
+
+    if seg_res.detection_id_field not in seg_res.df.columns:
+        seg_res.set_column(SegmentationResult.detection_id_field, list(range(len(pq))))
+
+    if seg_res.z_index_field not in seg_res.df.columns:
+        seg_res.set_column(SegmentationResult.z_index_field, 0)
+
+    if z_planes_number > 0:
+        if len(seg_res.df[seg_res.z_index_field].unique()) > 1:
+            raise ValueError('The input segmentation is already 3D. The conversion to 3D only possible for 2D '
+                             'segmentation')
+
+        z_planes = list(range(z_planes_number))
+        if not set(z_planes).issuperset(seg_res.df[seg_res.z_index_field].unique()):
+            raise ValueError('The z plane set of the input segmentation should be a subset of the requested set of '
+                             'output z planes')
+
+        seg_res.replicate_across_z(z_planes)
+        seg_res.set_z_levels([spacing + (x * spacing) for x in z_planes], 'ZLevel')
+
+    set_none = ['Name', 'ParentID', 'ParentType']
+    for column_name in set_none:
+        if column_name not in seg_res.df:
+            seg_res.set_column(column_name, None)
+    return seg_res, entity_ids_map
```

### Comparing `vpt-1.0.1/src/vpt/convert_geometry/converters/qpath_geojson_converter.py` & `vpt-1.0.2/src/vpt/convert_geometry/converters/qpath_geojson_converter.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-from typing import Tuple, Dict
-
-import geopandas as gpd
-from shapely import geometry
-from shapely.validation import make_valid
-
-from vpt.convert_geometry.converters.entity_id_generator import set_process_id, get_id
-from vpt.filesystem import vzg_open
-from vpt.segmentation.utils.seg_result import SegmentationResult
-
-
-def read_segmentation_result(input_path: str, entity_type: str, z_planes_number: int = 1,
-                             spacing: float = 1.5) -> Tuple[SegmentationResult, Dict]:
-    set_process_id()
-    entity_ids_map = {}
-    res = SegmentationResult()
-    with vzg_open(str(input_path), 'r') as f:
-        df = gpd.read_file(f)
-        df.crs = None
-
-        df.drop(columns=[col_name for col_name in df.columns if col_name != 'geometry'], inplace=True)
-        df.rename(columns={'geometry': SegmentationResult.geometry_field}, inplace=True)
-
-        entity_ids_map = {i: get_id() for i in range(len(df.index))}
-        df = df.assign(**{SegmentationResult.cell_id_field: [entity_ids_map[i] for i in range(len(df))]})
-
-        res = SegmentationResult(dataframe=df)
-        res.update_geometry(lambda x:
-                            make_valid(geometry.Polygon(x)) if isinstance(x, geometry.LineString)
-                            else make_valid(x))
-
-        res.set_entity_type(entity_type)
-        res.set_column(SegmentationResult.entity_name_field, entity_type)
-        res.set_column(SegmentationResult.detection_id_field, range(len(df)))
-        res.set_column(SegmentationResult.z_index_field, 0)
-
-        res.replicate_across_z(list(range(z_planes_number)))
-        res.set_z_levels([spacing + (x * spacing) for x in range(z_planes_number)], 'ZLevel')
-
-        set_none = ['Name', 'ParentID', 'ParentType']
-        for column_name in set_none:
-            res.set_column(column_name, None)
-    return res, entity_ids_map
+from typing import Tuple, Dict
+
+import geopandas as gpd
+from shapely import geometry
+from shapely.validation import make_valid
+
+from vpt.convert_geometry.converters.entity_id_generator import set_process_id, get_id
+from vpt.filesystem import vzg_open
+from vpt.segmentation.utils.seg_result import SegmentationResult
+
+
+def read_segmentation_result(input_path: str, entity_type: str, z_planes_number: int = 1,
+                             spacing: float = 1.5) -> Tuple[SegmentationResult, Dict]:
+    set_process_id()
+    entity_ids_map = {}
+    res = SegmentationResult()
+    with vzg_open(str(input_path), 'r') as f:
+        df = gpd.read_file(f)
+        df.crs = None
+
+        df.drop(columns=[col_name for col_name in df.columns if col_name != 'geometry'], inplace=True)
+        df.rename(columns={'geometry': SegmentationResult.geometry_field}, inplace=True)
+
+        entity_ids_map = {i: get_id() for i in range(len(df.index))}
+        df = df.assign(**{SegmentationResult.cell_id_field: [entity_ids_map[i] for i in range(len(df))]})
+
+        res = SegmentationResult(dataframe=df)
+        res.update_geometry(lambda x:
+                            make_valid(geometry.Polygon(x)) if isinstance(x, geometry.LineString)
+                            else make_valid(x))
+
+        res.set_entity_type(entity_type)
+        res.set_column(SegmentationResult.entity_name_field, entity_type)
+        res.set_column(SegmentationResult.detection_id_field, range(len(df)))
+        res.set_column(SegmentationResult.z_index_field, 0)
+
+        res.replicate_across_z(list(range(z_planes_number)))
+        res.set_z_levels([spacing + (x * spacing) for x in range(z_planes_number)], 'ZLevel')
+
+        set_none = ['Name', 'ParentID', 'ParentType']
+        for column_name in set_none:
+            res.set_column(column_name, None)
+    return res, entity_ids_map
```

### Comparing `vpt-1.0.1/src/vpt/convert_geometry/factory.py` & `vpt-1.0.2/src/vpt/convert_geometry/factory.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-from enum import Enum
-from typing import Tuple, Dict
-
-from vpt.convert_geometry.converters.hdf5_converter import read_segmentation_result as hdf5_reader
-from vpt.convert_geometry.converters.old_parquet_converter import read_segmentation_result as parquet_reader
-from vpt.convert_geometry.converters.qpath_geojson_converter import read_segmentation_result as qpath_reader
-from vpt.filesystem import filesystem_path_split
-from vpt.segmentation.utils.seg_result import SegmentationResult
-
-
-class SegmentationFileType(Enum):
-    HDF5 = 0
-    QPATH = 1
-    PARQUET = 2
-    OTHER = 3
-
-
-def get_conversion_type(input_path: str) -> SegmentationFileType:
-    fs, path = filesystem_path_split(input_path)
-    ext = path.split(fs.sep)[-1].split('.')[-1]
-    if ext == 'hdf5':
-        return SegmentationFileType.HDF5
-    if ext == 'geojson':
-        return SegmentationFileType.QPATH
-    if ext == 'parquet':
-        return SegmentationFileType.PARQUET
-    return SegmentationFileType.OTHER
-
-
-def read_segmentation_result(input_path: str, **kwargs) -> Tuple[SegmentationResult, Dict]:
-    converters = {
-        SegmentationFileType.HDF5: hdf5_reader,
-        SegmentationFileType.QPATH: qpath_reader,
-        SegmentationFileType.PARQUET: parquet_reader,
-    }
-    file_type = get_conversion_type(input_path)
-    if file_type == SegmentationFileType.OTHER:
-        raise ValueError('input file type is not supported')
-    return converters[file_type](input_path, **kwargs)
+from enum import Enum
+from typing import Tuple, Dict
+
+from vpt.convert_geometry.converters.hdf5_converter import read_segmentation_result as hdf5_reader
+from vpt.convert_geometry.converters.old_parquet_converter import read_segmentation_result as parquet_reader
+from vpt.convert_geometry.converters.qpath_geojson_converter import read_segmentation_result as qpath_reader
+from vpt.filesystem import filesystem_path_split
+from vpt.segmentation.utils.seg_result import SegmentationResult
+
+
+class SegmentationFileType(Enum):
+    HDF5 = 0
+    QPATH = 1
+    PARQUET = 2
+    OTHER = 3
+
+
+def get_conversion_type(input_path: str) -> SegmentationFileType:
+    fs, path = filesystem_path_split(input_path)
+    ext = path.split(fs.sep)[-1].split('.')[-1]
+    if ext == 'hdf5':
+        return SegmentationFileType.HDF5
+    if ext == 'geojson':
+        return SegmentationFileType.QPATH
+    if ext == 'parquet':
+        return SegmentationFileType.PARQUET
+    return SegmentationFileType.OTHER
+
+
+def read_segmentation_result(input_path: str, **kwargs) -> Tuple[SegmentationResult, Dict]:
+    converters = {
+        SegmentationFileType.HDF5: hdf5_reader,
+        SegmentationFileType.QPATH: qpath_reader,
+        SegmentationFileType.PARQUET: parquet_reader,
+    }
+    file_type = get_conversion_type(input_path)
+    if file_type == SegmentationFileType.OTHER:
+        raise ValueError('input file type is not supported')
+    return converters[file_type](input_path, **kwargs)
```

### Comparing `vpt-1.0.1/src/vpt/convert_to_ome/cmd_args.py` & `vpt-1.0.2/src/vpt/convert_to_ome/cmd_args.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-from argparse import ArgumentParser
-from dataclasses import dataclass
-
-from vpt.filesystem import filesystem_path_split
-from vpt.utils.validate import validate_exists, validate_does_not_exist
-
-
-@dataclass
-class ConvertToOmeArgs:
-    input_path: str
-    output_path: str
-    overwrite: bool
-
-
-def validate_args(args: ConvertToOmeArgs):
-    input_fs, input_path_inside_fs = filesystem_path_split(args.input_path)
-    output_fs, output_path_inside_fs = filesystem_path_split(args.output_path)
-
-    validate_exists(args.input_path)
-
-    if input_fs.isdir(input_path_inside_fs):
-        if output_fs.isfile(output_path_inside_fs):
-            raise ValueError('Output path should be a directory since the provided input path is a directory')
-        if not args.overwrite:
-            for path in input_fs.glob(input_fs.sep.join([input_path_inside_fs, '*.tif'])):
-                stem = path.split(input_fs.sep)[-1].split('.')[0]
-                output_file = output_fs.sep.join([output_path_inside_fs, f'{stem}.ome.tif'])
-                if output_fs.exists(output_file):
-                    raise ValueError(f'Output file already exists: {output_file}')
-
-    if input_fs.isfile(input_path_inside_fs):
-        if output_fs.isdir(output_path_inside_fs):
-            raise ValueError('Output path should be a file since the provided input path is a file')
-        if not args.overwrite:
-            validate_does_not_exist(args.output_path)
-
-
-def get_parser() -> ArgumentParser:
-    parser = ArgumentParser(description='Transforms the large 16-bit mosaic tiff images produced by the MERSCOPE '
-                            'into a OME pyramidal tiff.',
-                            add_help=False
-                            )
-    required = parser.add_argument_group('Required arguments')
-    required.add_argument('--input-image', type=str, required=True,
-                          help='Either a path to a directory or a path to a specific file.')
-
-    opt = parser.add_argument_group('Optional arguments')
-    opt.add_argument('--output-image', type=str, required=True,
-                     help='Either a path to a directory or a path to a specific file.')
-    opt.add_argument('--overwrite', action='store_true', default=False, required=False,
-                     help='Set flag if you want to use non empty directory and agree that files can be over-written.')
-    opt.add_argument("-h", "--help", action="help", help="Show this help message and exit")
-
-    return parser
+from argparse import ArgumentParser
+from dataclasses import dataclass
+
+from vpt.filesystem import filesystem_path_split
+from vpt.utils.validate import validate_exists, validate_does_not_exist
+
+
+@dataclass
+class ConvertToOmeArgs:
+    input_path: str
+    output_path: str
+    overwrite: bool
+
+
+def validate_args(args: ConvertToOmeArgs):
+    input_fs, input_path_inside_fs = filesystem_path_split(args.input_path)
+    output_fs, output_path_inside_fs = filesystem_path_split(args.output_path)
+
+    validate_exists(args.input_path)
+
+    if input_fs.isdir(input_path_inside_fs):
+        if output_fs.isfile(output_path_inside_fs):
+            raise ValueError('Output path should be a directory since the provided input path is a directory')
+        if not args.overwrite:
+            for path in input_fs.glob(input_fs.sep.join([input_path_inside_fs, '*.tif'])):
+                stem = path.split(input_fs.sep)[-1].split('.')[0]
+                output_file = output_fs.sep.join([output_path_inside_fs, f'{stem}.ome.tif'])
+                if output_fs.exists(output_file):
+                    raise ValueError(f'Output file already exists: {output_file}')
+
+    if input_fs.isfile(input_path_inside_fs):
+        if output_fs.isdir(output_path_inside_fs):
+            raise ValueError('Output path should be a file since the provided input path is a file')
+        if not args.overwrite:
+            validate_does_not_exist(args.output_path)
+
+
+def get_parser() -> ArgumentParser:
+    parser = ArgumentParser(description='Transforms the large 16-bit mosaic tiff images produced by the MERSCOPE '
+                            'into a OME pyramidal tiff.',
+                            add_help=False
+                            )
+    required = parser.add_argument_group('Required arguments')
+    required.add_argument('--input-image', type=str, required=True,
+                          help='Either a path to a directory or a path to a specific file.')
+
+    opt = parser.add_argument_group('Optional arguments')
+    opt.add_argument('--output-image', type=str, required=True,
+                     help='Either a path to a directory or a path to a specific file.')
+    opt.add_argument('--overwrite', action='store_true', default=False, required=False,
+                     help='Set flag if you want to use non empty directory and agree that files can be over-written.')
+    opt.add_argument("-h", "--help", action="help", help="Show this help message and exit")
+
+    return parser
```

### Comparing `vpt-1.0.1/src/vpt/convert_to_ome/main.py` & `vpt-1.0.2/src/vpt/convert_to_ome/main.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-import argparse
-
-from vpt.convert_to_ome.cmd_args import get_parser, ConvertToOmeArgs, validate_args
-from vpt.convert_to_ome.tiffutils import add_ome_metadata, read_image, save_as_pyramidal_image, \
-    extract_channel_from_filename
-from vpt.filesystem import initialize_filesystem, filesystem_path_split
-import vpt.log as log
-
-
-def convert_file(input_path: str, output_path: str) -> None:
-    log.info(f'processing file:{input_path}')
-    with read_image(input_path) as im:
-        channel_name = extract_channel_from_filename(input_path)
-
-        add_ome_metadata(im, im.width, im.height, im.format, 1, [channel_name])
-
-        save_as_pyramidal_image(im, output_path)
-
-
-def convert_dir(input_path: str, output_path: str) -> None:
-    input_fs, input_path_inside_fs = filesystem_path_split(input_path)
-    output_fs, output_path_inside_fs = filesystem_path_split(output_path)
-    log.info(f'processing dir:{input_path}')
-
-    for input_image_path in input_fs.glob(input_fs.sep.join([input_path_inside_fs, '*.tif'])):
-        filename = input_image_path.split(input_fs.sep)[-1]
-        stem = filename.split('.')[0]
-        output_image_path = output_fs.sep.join([output_path_inside_fs, f'{stem}.ome.tif'])
-
-        convert_file(input_image_path, output_image_path)
-
-
-def convert_to_ome(args: argparse.Namespace):
-    args = ConvertToOmeArgs(args.input_image, args.output_image, args.overwrite)
-    validate_args(args)
-    log.info("convert to ome started")
-
-    input_fs, input_path_inside_fs = filesystem_path_split(args.input_path)
-
-    if input_fs.isfile(input_path_inside_fs):
-        convert_file(args.input_path, args.output_path)
-    else:
-        convert_dir(args.input_path, args.output_path)
-    log.info("convert to ome finished")
-
-
-if __name__ == '__main__':
-    initialize_filesystem()
-    convert_to_ome(get_parser().parse_args())
+import argparse
+
+from vpt.convert_to_ome.cmd_args import get_parser, ConvertToOmeArgs, validate_args
+from vpt.convert_to_ome.tiffutils import add_ome_metadata, read_image, save_as_pyramidal_image, \
+    extract_channel_from_filename
+from vpt.filesystem import initialize_filesystem, filesystem_path_split
+import vpt.log as log
+
+
+def convert_file(input_path: str, output_path: str) -> None:
+    log.info(f'processing file:{input_path}')
+    with read_image(input_path) as im:
+        channel_name = extract_channel_from_filename(input_path)
+
+        add_ome_metadata(im, im.width, im.height, im.format, 1, [channel_name])
+
+        save_as_pyramidal_image(im, output_path)
+
+
+def convert_dir(input_path: str, output_path: str) -> None:
+    input_fs, input_path_inside_fs = filesystem_path_split(input_path)
+    output_fs, output_path_inside_fs = filesystem_path_split(output_path)
+    log.info(f'processing dir:{input_path}')
+
+    for input_image_path in input_fs.glob(input_fs.sep.join([input_path_inside_fs, '*.tif'])):
+        filename = input_image_path.split(input_fs.sep)[-1]
+        stem = filename.split('.')[0]
+        output_image_path = output_fs.sep.join([output_path_inside_fs, f'{stem}.ome.tif'])
+
+        convert_file(input_image_path, output_image_path)
+
+
+def convert_to_ome(args: argparse.Namespace):
+    args = ConvertToOmeArgs(args.input_image, args.output_image, args.overwrite)
+    validate_args(args)
+    log.info("convert to ome started")
+
+    input_fs, input_path_inside_fs = filesystem_path_split(args.input_path)
+
+    if input_fs.isfile(input_path_inside_fs):
+        convert_file(args.input_path, args.output_path)
+    else:
+        convert_dir(args.input_path, args.output_path)
+    log.info("convert to ome finished")
+
+
+if __name__ == '__main__':
+    initialize_filesystem()
+    convert_to_ome(get_parser().parse_args())
```

### Comparing `vpt-1.0.1/src/vpt/convert_to_ome/main_rgb.py` & `vpt-1.0.2/src/vpt/convert_to_ome/main_rgb.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-import argparse
-import contextlib
-import os
-
-from vpt.convert_to_ome.rgb_cmd_args import get_parser, ConvertToRGBOmeArgs, validate_args
-from vpt.convert_to_ome.tiffutils import read_image, add_ome_metadata, save_as_pyramidal_image, \
-    extract_channel_from_filename
-from vpt.filesystem import initialize_filesystem
-
-import pyvips # noqa
-
-env_path_list = os.environ['PATH'].split(';')
-vips = [x for x in env_path_list if os.path.exists(os.path.join(x, 'vips.exe'))]
-if len(vips) > 0:
-    os.environ['PATH'] = vips[0] + ";" + os.environ['PATH']
-
-
-def convert_to_ome_rgb(args: argparse.Namespace):
-    args = ConvertToRGBOmeArgs(args.input_image_red, args.input_image_green,
-                               args.input_image_blue, args.output_image, args.overwrite)
-    validate_args(args)
-
-    inputs = []
-    channel_names = []
-
-    with contextlib.ExitStack() as stack:
-        images = []
-        for input_path in args.input_path_red, args.input_path_green, args.input_path_blue:
-            if input_path is None:
-                inputs.append(None)
-                channel_names.append(None)
-            else:
-                images.append(stack.enter_context(read_image(input_path)))
-                image = pyvips.Image.arrayjoin(images[-1].bandsplit(), across=1)
-                inputs.append(image)
-
-                channel_names.append(extract_channel_from_filename(input_path))
-
-        # Find a non-none channel image
-        img = next(inp for inp in inputs if inp is not None)
-        image_type = img.format
-        image_width, image_height = img.width, img.height
-
-        for i in range(len(inputs)):
-            if inputs[i] is None:
-                inputs[i] = pyvips.Image.black(image_width, image_height)
-
-        rgb = pyvips.Image.arrayjoin(inputs, across=1)
-
-        add_ome_metadata(rgb, image_width, image_height, image_type, 3, channel_names)
-
-        save_as_pyramidal_image(rgb, args.output_path)
-
-
-if __name__ == '__main__':
-    initialize_filesystem()
-    convert_to_ome_rgb(get_parser().parse_args())
+import argparse
+import contextlib
+import os
+
+from vpt.convert_to_ome.rgb_cmd_args import get_parser, ConvertToRGBOmeArgs, validate_args
+from vpt.convert_to_ome.tiffutils import read_image, add_ome_metadata, save_as_pyramidal_image, \
+    extract_channel_from_filename
+from vpt.filesystem import initialize_filesystem
+
+import pyvips # noqa
+
+env_path_list = os.environ['PATH'].split(';')
+vips = [x for x in env_path_list if os.path.exists(os.path.join(x, 'vips.exe'))]
+if len(vips) > 0:
+    os.environ['PATH'] = vips[0] + ";" + os.environ['PATH']
+
+
+def convert_to_ome_rgb(args: argparse.Namespace):
+    args = ConvertToRGBOmeArgs(args.input_image_red, args.input_image_green,
+                               args.input_image_blue, args.output_image, args.overwrite)
+    validate_args(args)
+
+    inputs = []
+    channel_names = []
+
+    with contextlib.ExitStack() as stack:
+        images = []
+        for input_path in args.input_path_red, args.input_path_green, args.input_path_blue:
+            if input_path is None:
+                inputs.append(None)
+                channel_names.append(None)
+            else:
+                images.append(stack.enter_context(read_image(input_path)))
+                image = pyvips.Image.arrayjoin(images[-1].bandsplit(), across=1)
+                inputs.append(image)
+
+                channel_names.append(extract_channel_from_filename(input_path))
+
+        # Find a non-none channel image
+        img = next(inp for inp in inputs if inp is not None)
+        image_type = img.format
+        image_width, image_height = img.width, img.height
+
+        for i in range(len(inputs)):
+            if inputs[i] is None:
+                inputs[i] = pyvips.Image.black(image_width, image_height)
+
+        rgb = pyvips.Image.arrayjoin(inputs, across=1)
+
+        add_ome_metadata(rgb, image_width, image_height, image_type, 3, channel_names)
+
+        save_as_pyramidal_image(rgb, args.output_path)
+
+
+if __name__ == '__main__':
+    initialize_filesystem()
+    convert_to_ome_rgb(get_parser().parse_args())
```

### Comparing `vpt-1.0.1/src/vpt/convert_to_ome/rgb_cmd_args.py` & `vpt-1.0.2/src/vpt/convert_to_ome/rgb_cmd_args.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,62 +1,62 @@
-from argparse import ArgumentParser
-from dataclasses import dataclass
-from typing import Optional
-
-from vpt.filesystem import filesystem_path_split
-from vpt.utils.validate import validate_does_not_exist
-
-
-@dataclass
-class ConvertToRGBOmeArgs:
-    input_path_red: Optional[str]
-    input_path_green: Optional[str]
-    input_path_blue: Optional[str]
-    output_path: str
-    overwrite: bool
-
-
-def validate_args(args: ConvertToRGBOmeArgs):
-    if all(path is None for path in (args.input_path_red,
-                                     args.input_path_green,
-                                     args.input_path_blue)):
-        raise ValueError('Image for least one of the channels should be specified')
-
-    for input_path in args.input_path_red, args.input_path_green, args.input_path_blue:
-        if input_path is None:
-            continue
-
-        input_fs, input_path_inside_fs = filesystem_path_split(input_path)
-
-        if not input_fs.isfile(input_path_inside_fs):
-            raise ValueError(f'Input is not a file: {input_path}')
-
-    output_fs, output_path_inside_fs = filesystem_path_split(args.output_path)
-
-    if output_fs.isdir(output_path_inside_fs):
-        raise ValueError('Output should be a file')
-
-    if not args.overwrite:
-        validate_does_not_exist(args.output_path)
-
-
-def get_parser() -> ArgumentParser:
-    parser = ArgumentParser(description='Converts up to three flat tiff images into a rgb OME-tiff pyramidal images. '
-                            'If a rgb channel input isn’t specified, the channel will be dark (all 0’s).',
-                            add_help=False
-                            )
-    required = parser.add_argument_group('Required arguments')
-    required.add_argument('--output-image', type=str, required=True,
-                          help='Either a path to a directory or a path to a specific file')
-
-    opt = parser.add_argument_group('Optional arguments')
-    opt.add_argument('--input-image-red', type=str, required=False,
-                     help='Either a path to a directory or a path to a specific file')
-    opt.add_argument('--input-image-green', type=str, required=False,
-                     help='Either a path to a directory or a path to a specific file')
-    opt.add_argument('--input-image-blue', type=str, required=False,
-                     help='Either a path to a directory or a path to a specific file')
-    opt.add_argument('--overwrite', action='store_true', default=False, required=False,
-                     help='')
-    opt.add_argument("-h", "--help", action="help", help="Show this help message and exit")
-
-    return parser
+from argparse import ArgumentParser
+from dataclasses import dataclass
+from typing import Optional
+
+from vpt.filesystem import filesystem_path_split
+from vpt.utils.validate import validate_does_not_exist
+
+
+@dataclass
+class ConvertToRGBOmeArgs:
+    input_path_red: Optional[str]
+    input_path_green: Optional[str]
+    input_path_blue: Optional[str]
+    output_path: str
+    overwrite: bool
+
+
+def validate_args(args: ConvertToRGBOmeArgs):
+    if all(path is None for path in (args.input_path_red,
+                                     args.input_path_green,
+                                     args.input_path_blue)):
+        raise ValueError('Image for least one of the channels should be specified')
+
+    for input_path in args.input_path_red, args.input_path_green, args.input_path_blue:
+        if input_path is None:
+            continue
+
+        input_fs, input_path_inside_fs = filesystem_path_split(input_path)
+
+        if not input_fs.isfile(input_path_inside_fs):
+            raise ValueError(f'Input is not a file: {input_path}')
+
+    output_fs, output_path_inside_fs = filesystem_path_split(args.output_path)
+
+    if output_fs.isdir(output_path_inside_fs):
+        raise ValueError('Output should be a file')
+
+    if not args.overwrite:
+        validate_does_not_exist(args.output_path)
+
+
+def get_parser() -> ArgumentParser:
+    parser = ArgumentParser(description='Converts up to three flat tiff images into a rgb OME-tiff pyramidal images. '
+                            'If a rgb channel input isn’t specified, the channel will be dark (all 0’s).',
+                            add_help=False
+                            )
+    required = parser.add_argument_group('Required arguments')
+    required.add_argument('--output-image', type=str, required=True,
+                          help='Either a path to a directory or a path to a specific file')
+
+    opt = parser.add_argument_group('Optional arguments')
+    opt.add_argument('--input-image-red', type=str, required=False,
+                     help='Either a path to a directory or a path to a specific file')
+    opt.add_argument('--input-image-green', type=str, required=False,
+                     help='Either a path to a directory or a path to a specific file')
+    opt.add_argument('--input-image-blue', type=str, required=False,
+                     help='Either a path to a directory or a path to a specific file')
+    opt.add_argument('--overwrite', action='store_true', default=False, required=False,
+                     help='')
+    opt.add_argument("-h", "--help", action="help", help="Show this help message and exit")
+
+    return parser
```

### Comparing `vpt-1.0.1/src/vpt/convert_to_ome/tiffutils.py` & `vpt-1.0.2/src/vpt/convert_to_ome/tiffutils.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,120 +1,120 @@
-import contextlib
-import os
-import re
-import tempfile
-from typing import List
-
-import numpy as np
-
-from vpt.filesystem.vzgfs import protocol_path_split, Protocol, filesystem_for_protocol, filesystem_path_split
-
-env_path_list = os.environ['PATH'].split(';')
-vips = [x for x in env_path_list if os.path.exists(os.path.join(x, 'vips.exe'))]
-if len(vips) > 0:
-    os.environ['PATH'] = vips[0] + ";" + os.environ['PATH']
-
-import pyvips # noqa
-
-format_to_dtype = {
-    'uchar': np.uint8,
-    'char': np.int8,
-    'ushort': np.uint16,
-    'short': np.int16,
-    'uint': np.uint32,
-    'int': np.int32,
-    'float': np.float32,
-    'double': np.float64,
-    'complex': np.complex64,
-    'dpcomplex': np.complex128,
-}
-
-
-def add_ome_metadata(im: pyvips.Image, image_width: int, image_height: int,
-                     image_type: str, num_channels: int, channel_names: List) -> None:
-    channel_name_attribs = ['' if name is None else f' Name="{name}"' for name in channel_names]
-    channel_tags = '\n'.join(f'<Channel ID="Channel:0:{i}" SamplesPerPixel="1"{channel_name_attribs[i]}/>'
-                             for i in range(num_channels))
-    tiffdata_tags = f'<TiffData IFD="0" PlaneCount="{num_channels}"/>'
-
-    im.set_type(pyvips.GValue.gint_type, "page-height", image_height)
-    im.set_type(pyvips.GValue.gstr_type, "image-description",
-                f"""<?xml version="1.0" encoding="UTF-8"?>
-    <OME xmlns="http://www.openmicroscopy.org/Schemas/OME/2016-06"
-        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
-        xsi:schemaLocation="http://www.openmicroscopy.org/Schemas/OME/2016-06 \
-        http://www.openmicroscopy.org/Schemas/OME/2016-06/ome.xsd">
-        <Image ID="Image:0">
-            <Pixels DimensionOrder="XYCZT"
-                    ID="Pixels:0"
-                    SizeC="{num_channels}"
-                    SizeT="1"
-                    SizeX="{image_width}"
-                    SizeY="{image_height}"
-                    SizeZ="1"
-                    Type="{np.dtype(format_to_dtype[image_type]).name}">
-                    {channel_tags}
-                    {tiffdata_tags}
-            </Pixels>
-        </Image>
-    </OME>""")
-
-
-def extract_channel_from_filename(path):
-    fs, path_inside_fs = filesystem_path_split(path)
-    match = re.match('mosaic_(?P<name>.+?)_z[0-9]+', path_inside_fs.split(fs.sep)[-1].rsplit('.')[0])
-    try:
-        channel_name = match.group('name')
-    except (IndexError, AttributeError):
-        channel_name = None
-    return channel_name
-
-
-@contextlib.contextmanager
-def read_image(path: str, **kwargs) -> pyvips.Image:
-    kwargs.pop('access', None)
-
-    protocol, path_inside_fs = protocol_path_split(path)
-
-    if protocol == Protocol.LOCAL:
-        im = pyvips.Image.new_from_file(path, access='sequential', **kwargs)
-        yield im.copy()
-    else:
-        tempdir = tempfile.mkdtemp()
-        fs = filesystem_for_protocol(protocol)
-        filename = path_inside_fs.split(fs.sep)[-1]
-
-        local_path = os.path.join(tempdir, filename)
-
-        fs.get_file(path_inside_fs, local_path)
-
-        im = pyvips.Image.new_from_file(local_path, access='sequential', **kwargs)
-
-        yield im.copy()
-
-        os.unlink(local_path)
-
-
-def write_to_local_file(im: pyvips.Image, path: str):
-    im.write_to_file(path, pyramid=True, tile=True, subifd=True, compression='deflate', bigtiff=True)
-
-
-def save_as_pyramidal_image(im: pyvips.Image, path: str) -> None:
-    protocol, path_inside_fs = protocol_path_split(path)
-    fs = filesystem_for_protocol(protocol)
-
-    parent_dir = fs.sep.join(path_inside_fs.split(fs.sep)[:-1])
-    fs.mkdirs(parent_dir, exist_ok=True)
-
-    if protocol == Protocol.LOCAL:
-        write_to_local_file(im, path)
-    else:
-        tempdir = tempfile.mkdtemp()
-        filename = path_inside_fs.split(fs.sep)[-1]
-
-        local_path = os.path.join(tempdir, filename)
-
-        write_to_local_file(im, local_path)
-
-        fs.put_file(local_path, path_inside_fs)
-
-        os.unlink(local_path)
+import contextlib
+import os
+import re
+import tempfile
+from typing import List
+
+import numpy as np
+
+from vpt.filesystem.vzgfs import protocol_path_split, Protocol, filesystem_for_protocol, filesystem_path_split
+
+env_path_list = os.environ['PATH'].split(';')
+vips = [x for x in env_path_list if os.path.exists(os.path.join(x, 'vips.exe'))]
+if len(vips) > 0:
+    os.environ['PATH'] = vips[0] + ";" + os.environ['PATH']
+
+import pyvips # noqa
+
+format_to_dtype = {
+    'uchar': np.uint8,
+    'char': np.int8,
+    'ushort': np.uint16,
+    'short': np.int16,
+    'uint': np.uint32,
+    'int': np.int32,
+    'float': np.float32,
+    'double': np.float64,
+    'complex': np.complex64,
+    'dpcomplex': np.complex128,
+}
+
+
+def add_ome_metadata(im: pyvips.Image, image_width: int, image_height: int,
+                     image_type: str, num_channels: int, channel_names: List) -> None:
+    channel_name_attribs = ['' if name is None else f' Name="{name}"' for name in channel_names]
+    channel_tags = '\n'.join(f'<Channel ID="Channel:0:{i}" SamplesPerPixel="1"{channel_name_attribs[i]}/>'
+                             for i in range(num_channels))
+    tiffdata_tags = f'<TiffData IFD="0" PlaneCount="{num_channels}"/>'
+
+    im.set_type(pyvips.GValue.gint_type, "page-height", image_height)
+    im.set_type(pyvips.GValue.gstr_type, "image-description",
+                f"""<?xml version="1.0" encoding="UTF-8"?>
+    <OME xmlns="http://www.openmicroscopy.org/Schemas/OME/2016-06"
+        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
+        xsi:schemaLocation="http://www.openmicroscopy.org/Schemas/OME/2016-06 \
+        http://www.openmicroscopy.org/Schemas/OME/2016-06/ome.xsd">
+        <Image ID="Image:0">
+            <Pixels DimensionOrder="XYCZT"
+                    ID="Pixels:0"
+                    SizeC="{num_channels}"
+                    SizeT="1"
+                    SizeX="{image_width}"
+                    SizeY="{image_height}"
+                    SizeZ="1"
+                    Type="{np.dtype(format_to_dtype[image_type]).name}">
+                    {channel_tags}
+                    {tiffdata_tags}
+            </Pixels>
+        </Image>
+    </OME>""")
+
+
+def extract_channel_from_filename(path):
+    fs, path_inside_fs = filesystem_path_split(path)
+    match = re.match('mosaic_(?P<name>.+?)_z[0-9]+', path_inside_fs.split(fs.sep)[-1].rsplit('.')[0])
+    try:
+        channel_name = match.group('name')
+    except (IndexError, AttributeError):
+        channel_name = None
+    return channel_name
+
+
+@contextlib.contextmanager
+def read_image(path: str, **kwargs) -> pyvips.Image:
+    kwargs.pop('access', None)
+
+    protocol, path_inside_fs = protocol_path_split(path)
+
+    if protocol == Protocol.LOCAL:
+        im = pyvips.Image.new_from_file(path, access='sequential', **kwargs)
+        yield im.copy()
+    else:
+        tempdir = tempfile.mkdtemp()
+        fs = filesystem_for_protocol(protocol)
+        filename = path_inside_fs.split(fs.sep)[-1]
+
+        local_path = os.path.join(tempdir, filename)
+
+        fs.get_file(path_inside_fs, local_path)
+
+        im = pyvips.Image.new_from_file(local_path, access='sequential', **kwargs)
+
+        yield im.copy()
+
+        os.unlink(local_path)
+
+
+def write_to_local_file(im: pyvips.Image, path: str):
+    im.write_to_file(path, pyramid=True, tile=True, subifd=True, compression='deflate', bigtiff=True)
+
+
+def save_as_pyramidal_image(im: pyvips.Image, path: str) -> None:
+    protocol, path_inside_fs = protocol_path_split(path)
+    fs = filesystem_for_protocol(protocol)
+
+    parent_dir = fs.sep.join(path_inside_fs.split(fs.sep)[:-1])
+    fs.mkdirs(parent_dir, exist_ok=True)
+
+    if protocol == Protocol.LOCAL:
+        write_to_local_file(im, path)
+    else:
+        tempdir = tempfile.mkdtemp()
+        filename = path_inside_fs.split(fs.sep)[-1]
+
+        local_path = os.path.join(tempdir, filename)
+
+        write_to_local_file(im, local_path)
+
+        fs.put_file(local_path, path_inside_fs)
+
+        os.unlink(local_path)
```

### Comparing `vpt-1.0.1/src/vpt/derive_cell_metadata/cell_metadata.py` & `vpt-1.0.2/src/vpt/derive_cell_metadata/cell_metadata.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,140 +1,140 @@
-from typing import List
-
-import numpy as np
-import pandas as pd
-from shapely import geometry
-
-from vpt.utils.boundaries import Boundaries
-import vpt.log as log
-
-
-def polygons_generator(geometries):
-    for planeGeometry in geometries:
-        yield from planeGeometry.geoms
-
-
-def anisotropy_calculation(multi_poly):
-    bounding_rectangle = multi_poly.minimum_rotated_rectangle
-    rectangle_points = list(zip(*bounding_rectangle.exterior.xy))
-
-    sides = []
-    for p1, p2 in zip(rectangle_points[:-1], rectangle_points[1:]):
-        distance = np.sqrt((p1[0] - p2[0]) ** 2 + (p1[1] - p2[1]) ** 2)
-        sides.append(distance)
-
-    major_axis = np.max(sides)
-    minor_axis = np.min(sides)
-    anisotropy = major_axis / minor_axis
-    return anisotropy
-
-
-def create_metadata_table(
-        bnds: Boundaries,
-        zDepthList: List or np.ndarray,
-        barcodesCountPerCell: np.ndarray or None = None
-) -> pd.DataFrame:
-    cell_metadata = []
-    min_x, min_y, max_x, max_y, center_x, center_y = 0, 0, 0, 0, 0, 0
-
-    for featureIdx, feature in enumerate(bnds.features):
-        barcodeCount = np.nan if barcodesCountPerCell is None else barcodesCountPerCell[featureIdx]
-        cell_volume = 0
-        firstPoly = True
-        polysCount = 0
-        paRatio = 0
-        for polyIdx, poly in enumerate(feature.shapes):
-            if poly is None or poly.is_empty or poly.area < 1e-9:
-                continue
-            if firstPoly:
-                min_x = poly.bounds[0]
-                min_y = poly.bounds[1]
-                max_x = poly.bounds[2]
-                max_y = poly.bounds[3]
-                center_x = poly.centroid.x
-                center_y = poly.centroid.y
-                firstPoly = False
-            else:
-                min_x = min(min_x, poly.bounds[0])
-                min_y = min(min_y, poly.bounds[1])
-                max_x = max(max_x, poly.bounds[2])
-                max_y = max(max_y, poly.bounds[3])
-                center_x += poly.centroid.x
-                center_y += poly.centroid.y
-
-            cell_volume += poly.area * zDepthList[polyIdx]
-            paRatio += poly.length / poly.area
-            polysCount += 1
-
-        # If an empty feature is found, append a blank row to the output
-        if polysCount == 0:
-            meta = {
-                "fov": np.nan,
-                "EntityID": np.int64(feature.get_feature_id()),
-                "volume": np.nan,
-                "center_x": np.nan,
-                "center_y": np.nan,
-                "min_x": np.nan,
-                "min_y": np.nan,
-                "max_x": np.nan,
-                "max_y": np.nan,
-                "anisotropy": np.nan,
-                "transcript_count": np.nan,
-                "perimeter_area_ratio": np.nan,
-                "solidity": np.nan
-            }
-            cell_metadata.append(meta)
-            continue
-
-        allPlanesMultipolygon = geometry.MultiPolygon(polygons_generator(feature.get_true_polygons()))
-
-        try:
-            anisotropy = anisotropy_calculation(allPlanesMultipolygon)
-        except AttributeError:
-            log.info(f"Anisotropy of Entity {feature.get_feature_id()} could not be calculated")
-            anisotropy = np.nan
-
-        try:
-            solidity = allPlanesMultipolygon.area / allPlanesMultipolygon.convex_hull.area
-        except ZeroDivisionError:
-            log.info(f"Solidity of Entity {feature.get_feature_id()} could not be calculated")
-            solidity = np.nan
-
-        meta = {
-            "fov": np.nan,
-            "EntityID": np.int64(feature.get_feature_id()),
-            "volume": cell_volume,
-            "center_x": center_x / polysCount,
-            "center_y": center_y / polysCount,
-            "min_x": min_x,
-            "min_y": min_y,
-            "max_x": max_x,
-            "max_y": max_y,
-            "anisotropy": anisotropy,
-            "transcript_count": barcodeCount,
-            "perimeter_area_ratio": paRatio / polysCount,
-            "solidity": solidity
-        }
-        cell_metadata.append(meta)
-
-    if cell_metadata:
-        output = pd.DataFrame(cell_metadata)
-    else:
-        output = pd.DataFrame(columns=[
-            "fov",
-            "EntityID",
-            "volume",
-            "center_x",
-            "center_y",
-            "min_x",
-            "min_y",
-            "max_x",
-            "max_y",
-            "anisotropy",
-            "transcript_count",
-            "perimeter_area_ratio",
-            "solidity"
-        ])
-
-    output.set_index("EntityID", inplace=True)
-    output = output.sort_index()
-    return output
+from typing import List
+
+import numpy as np
+import pandas as pd
+from shapely import geometry
+
+from vpt.utils.boundaries import Boundaries
+import vpt.log as log
+
+
+def polygons_generator(geometries):
+    for planeGeometry in geometries:
+        yield from planeGeometry.geoms
+
+
+def anisotropy_calculation(multi_poly):
+    bounding_rectangle = multi_poly.minimum_rotated_rectangle
+    rectangle_points = list(zip(*bounding_rectangle.exterior.xy))
+
+    sides = []
+    for p1, p2 in zip(rectangle_points[:-1], rectangle_points[1:]):
+        distance = np.sqrt((p1[0] - p2[0]) ** 2 + (p1[1] - p2[1]) ** 2)
+        sides.append(distance)
+
+    major_axis = np.max(sides)
+    minor_axis = np.min(sides)
+    anisotropy = major_axis / minor_axis
+    return anisotropy
+
+
+def create_metadata_table(
+        bnds: Boundaries,
+        zDepthList: List or np.ndarray,
+        barcodesCountPerCell: np.ndarray or None = None
+) -> pd.DataFrame:
+    cell_metadata = []
+    min_x, min_y, max_x, max_y, center_x, center_y = 0, 0, 0, 0, 0, 0
+
+    for featureIdx, feature in enumerate(bnds.features):
+        barcodeCount = np.nan if barcodesCountPerCell is None else barcodesCountPerCell[featureIdx]
+        cell_volume = 0
+        firstPoly = True
+        polysCount = 0
+        paRatio = 0
+        for polyIdx, poly in enumerate(feature.shapes):
+            if poly is None or poly.is_empty or poly.area < 1e-9:
+                continue
+            if firstPoly:
+                min_x = poly.bounds[0]
+                min_y = poly.bounds[1]
+                max_x = poly.bounds[2]
+                max_y = poly.bounds[3]
+                center_x = poly.centroid.x
+                center_y = poly.centroid.y
+                firstPoly = False
+            else:
+                min_x = min(min_x, poly.bounds[0])
+                min_y = min(min_y, poly.bounds[1])
+                max_x = max(max_x, poly.bounds[2])
+                max_y = max(max_y, poly.bounds[3])
+                center_x += poly.centroid.x
+                center_y += poly.centroid.y
+
+            cell_volume += poly.area * zDepthList[polyIdx]
+            paRatio += poly.length / poly.area
+            polysCount += 1
+
+        # If an empty feature is found, append a blank row to the output
+        if polysCount == 0:
+            meta = {
+                "fov": np.nan,
+                "EntityID": np.int64(feature.get_feature_id()),
+                "volume": np.nan,
+                "center_x": np.nan,
+                "center_y": np.nan,
+                "min_x": np.nan,
+                "min_y": np.nan,
+                "max_x": np.nan,
+                "max_y": np.nan,
+                "anisotropy": np.nan,
+                "transcript_count": np.nan,
+                "perimeter_area_ratio": np.nan,
+                "solidity": np.nan
+            }
+            cell_metadata.append(meta)
+            continue
+
+        allPlanesMultipolygon = geometry.MultiPolygon(polygons_generator(feature.get_true_polygons()))
+
+        try:
+            anisotropy = anisotropy_calculation(allPlanesMultipolygon)
+        except AttributeError:
+            log.info(f"Anisotropy of Entity {feature.get_feature_id()} could not be calculated")
+            anisotropy = np.nan
+
+        try:
+            solidity = allPlanesMultipolygon.area / allPlanesMultipolygon.convex_hull.area
+        except ZeroDivisionError:
+            log.info(f"Solidity of Entity {feature.get_feature_id()} could not be calculated")
+            solidity = np.nan
+
+        meta = {
+            "fov": np.nan,
+            "EntityID": np.int64(feature.get_feature_id()),
+            "volume": cell_volume,
+            "center_x": center_x / polysCount,
+            "center_y": center_y / polysCount,
+            "min_x": min_x,
+            "min_y": min_y,
+            "max_x": max_x,
+            "max_y": max_y,
+            "anisotropy": anisotropy,
+            "transcript_count": barcodeCount,
+            "perimeter_area_ratio": paRatio / polysCount,
+            "solidity": solidity
+        }
+        cell_metadata.append(meta)
+
+    if cell_metadata:
+        output = pd.DataFrame(cell_metadata)
+    else:
+        output = pd.DataFrame(columns=[
+            "fov",
+            "EntityID",
+            "volume",
+            "center_x",
+            "center_y",
+            "min_x",
+            "min_y",
+            "max_x",
+            "max_y",
+            "anisotropy",
+            "transcript_count",
+            "perimeter_area_ratio",
+            "solidity"
+        ])
+
+    output.set_index("EntityID", inplace=True)
+    output = output.sort_index()
+    return output
```

### Comparing `vpt-1.0.1/src/vpt/derive_cell_metadata/cmd_args.py` & `vpt-1.0.2/src/vpt/derive_cell_metadata/cmd_args.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-from argparse import ArgumentParser, Namespace
-from dataclasses import dataclass
-from typing import Optional, Sequence
-
-from vpt.utils.validate import validate_exists, validate_does_not_exist
-
-
-@dataclass
-class DeriveMetadataArgs:
-    input_boundaries: str
-    output_metadata: str
-    input_entity_by_gene: str
-    overwrite: bool
-
-
-def validate_args(args: DeriveMetadataArgs):
-    validate_exists(args.input_boundaries)
-    if args.input_entity_by_gene:
-        validate_exists(args.input_entity_by_gene)
-    if not args.overwrite:
-        validate_does_not_exist(args.output_metadata)
-
-
-def get_parser() -> ArgumentParser:
-    parser = ArgumentParser(description='Uses the segmentation boundaries to calculate the geometric attributes '
-                            'of each Entity. These attributes include the position, volume, and morphological features.',
-                            add_help=False
-                            )
-    required = parser.add_argument_group('Required arguments')
-    required.add_argument('--input-boundaries', required=True, type=str,
-                          help='Path to a micron-space parquet boundary file.')
-    required.add_argument('--output-metadata', required=True, type=str,
-                          help='Path to the output csv file where the entity metadata will be stored.')
-
-    opt = parser.add_argument_group('Optional arguments')
-    opt.add_argument('--input-entity-by-gene', required=False, type=str,
-                     help='Path to an existing entity by gene csv.')
-    opt.add_argument('--overwrite', action='store_true', default=False, required=False,
-                     help='Set flag if you want to use non empty directory and agree that files can be over-written.')
-    opt.add_argument("-h", "--help", action="help", help="Show this help message and exit")
-
-    return parser
-
-
-def parse_args(args: Optional[Sequence[str]] = None) -> Namespace:
-    return get_parser().parse_args(args)
+from argparse import ArgumentParser, Namespace
+from dataclasses import dataclass
+from typing import Optional, Sequence
+
+from vpt.utils.validate import validate_exists, validate_does_not_exist
+
+
+@dataclass
+class DeriveMetadataArgs:
+    input_boundaries: str
+    output_metadata: str
+    input_entity_by_gene: str
+    overwrite: bool
+
+
+def validate_args(args: DeriveMetadataArgs):
+    validate_exists(args.input_boundaries)
+    if args.input_entity_by_gene:
+        validate_exists(args.input_entity_by_gene)
+    if not args.overwrite:
+        validate_does_not_exist(args.output_metadata)
+
+
+def get_parser() -> ArgumentParser:
+    parser = ArgumentParser(description='Uses the segmentation boundaries to calculate the geometric attributes '
+                            'of each Entity. These attributes include the position, volume, and morphological features.',
+                            add_help=False
+                            )
+    required = parser.add_argument_group('Required arguments')
+    required.add_argument('--input-boundaries', required=True, type=str,
+                          help='Path to a micron-space parquet boundary file.')
+    required.add_argument('--output-metadata', required=True, type=str,
+                          help='Path to the output csv file where the entity metadata will be stored.')
+
+    opt = parser.add_argument_group('Optional arguments')
+    opt.add_argument('--input-entity-by-gene', required=False, type=str,
+                     help='Path to an existing entity by gene csv.')
+    opt.add_argument('--overwrite', action='store_true', default=False, required=False,
+                     help='Set flag if you want to use non empty directory and agree that files can be over-written.')
+    opt.add_argument("-h", "--help", action="help", help="Show this help message and exit")
+
+    return parser
+
+
+def parse_args(args: Optional[Sequence[str]] = None) -> Namespace:
+    return get_parser().parse_args(args)
```

### Comparing `vpt-1.0.1/src/vpt/derive_cell_metadata/run_derive_cell_metadata.py` & `vpt-1.0.2/src/vpt/derive_cell_metadata/run_derive_cell_metadata.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-import argparse
-
-import pandas as pd
-import numpy as np
-from vpt.filesystem.vzgfs import vzg_open
-from vpt.utils.boundaries import Boundaries
-from vpt.derive_cell_metadata.cell_metadata import create_metadata_table
-from vpt.utils.cellsreader import CellsReader, cell_reader_factory
-from vpt.utils.output_tools import make_parent_dirs
-from vpt.derive_cell_metadata.cmd_args import validate_args
-import vpt.log as log
-
-
-def main_derive_cell_metadata(args: argparse.Namespace) -> None:
-    validate_args(args)
-
-    log.info('Derive cell metadata started')
-    barcodesSumList = None
-    if args.input_entity_by_gene:
-        with vzg_open(args.input_entity_by_gene, 'r') as f:
-            cellByGeneDf = pd.read_csv(f)
-        cellByGeneNp = cellByGeneDf.to_numpy()
-        barcodesSumList = [np.sum(row[1:]) for row in cellByGeneNp]
-
-    cellsReader: CellsReader = cell_reader_factory(args.input_boundaries)
-    bnds = Boundaries(cellsReader)
-
-    meta = create_metadata_table(bnds, cellsReader.get_z_levels(), barcodesSumList)
-
-    make_parent_dirs(args.output_metadata)
-    with vzg_open(args.output_metadata, 'w') as f:
-        meta.to_csv(f, sep=',')
-
-    log.info('Derive cell metadata finished')
+import argparse
+
+import pandas as pd
+import numpy as np
+from vpt.filesystem.vzgfs import vzg_open
+from vpt.utils.boundaries import Boundaries
+from vpt.derive_cell_metadata.cell_metadata import create_metadata_table
+from vpt.utils.cellsreader import CellsReader, cell_reader_factory
+from vpt.utils.output_tools import make_parent_dirs
+from vpt.derive_cell_metadata.cmd_args import validate_args
+import vpt.log as log
+
+
+def main_derive_cell_metadata(args: argparse.Namespace) -> None:
+    validate_args(args)
+
+    log.info('Derive cell metadata started')
+    barcodesSumList = None
+    if args.input_entity_by_gene:
+        with vzg_open(args.input_entity_by_gene, 'r') as f:
+            cellByGeneDf = pd.read_csv(f)
+        cellByGeneNp = cellByGeneDf.to_numpy()
+        barcodesSumList = [np.sum(row[1:]) for row in cellByGeneNp]
+
+    cellsReader: CellsReader = cell_reader_factory(args.input_boundaries)
+    bnds = Boundaries(cellsReader)
+
+    meta = create_metadata_table(bnds, cellsReader.get_z_levels(), barcodesSumList)
+
+    make_parent_dirs(args.output_metadata)
+    with vzg_open(args.output_metadata, 'w') as f:
+        meta.to_csv(f, sep=',')
+
+    log.info('Derive cell metadata finished')
```

### Comparing `vpt-1.0.1/src/vpt/filesystem/vzgfs.py` & `vpt-1.0.2/src/vpt/filesystem/vzgfs.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,158 +1,158 @@
-import json
-import os
-from enum import Enum
-from typing import Optional, Tuple
-
-import gcsfs
-import rasterio.session
-from fsspec import AbstractFileSystem
-from fsspec.implementations.local import LocalFileSystem
-from gcsfs import GCSFileSystem
-from s3fs import S3FileSystem
-
-import vpt.log as log
-
-import warnings
-from rasterio.errors import NotGeoreferencedWarning
-
-from vpt import AWS_PROFILE_NAME_VAR, GCS_SERVICE_ACCOUNT_KEY_VAR, AWS_SECRET_KEY_VAR, AWS_ACCESS_KEY_VAR
-
-
-class Protocol(Enum):
-    LOCAL = 0
-    S3 = 1
-    GCS = 2
-
-
-AWS_PROFILE_NAME = None
-AWS_ACCESS_KEY = None
-AWS_SECRET_KEY = None
-
-GCS_SERVICE_ACCOUNT_KEY = None
-
-
-def initialize_filesystem(
-        aws_access_key=None,
-        aws_secret_key=None,
-        aws_profile_name=None,
-        gcs_service_account_key=None
-):
-    global AWS_PROFILE_NAME, AWS_ACCESS_KEY, AWS_SECRET_KEY, GCS_SERVICE_ACCOUNT_KEY
-
-    if all([aws_profile_name, aws_access_key, aws_secret_key]):
-        log.warning('Both AWS profile name and access key/secret key pair are specified.')
-
-    AWS_PROFILE_NAME = aws_profile_name if aws_profile_name else os.environ.get(AWS_PROFILE_NAME_VAR)
-    AWS_ACCESS_KEY = aws_access_key if aws_access_key else os.environ.get(AWS_ACCESS_KEY_VAR)
-    AWS_SECRET_KEY = aws_secret_key if aws_secret_key else os.environ.get(AWS_SECRET_KEY_VAR)
-
-    if gcs_service_account_key:
-        GCS_SERVICE_ACCOUNT_KEY = gcs_service_account_key
-    else:
-        GCS_SERVICE_ACCOUNT_KEY = os.environ.get(GCS_SERVICE_ACCOUNT_KEY_VAR)
-        try:
-            GCS_SERVICE_ACCOUNT_KEY = json.loads(GCS_SERVICE_ACCOUNT_KEY)
-        except Exception:
-            pass
-
-
-def filesystem_for_protocol(protocol: Protocol) -> Optional[AbstractFileSystem]:
-    global AWS_PROFILE_NAME, AWS_ACCESS_KEY, AWS_SECRET_KEY, GCS_SERVICE_ACCOUNT_KEY
-
-    if protocol == Protocol.LOCAL:
-        return LocalFileSystem()
-    elif protocol == Protocol.S3:
-        return S3FileSystem(
-            key=AWS_ACCESS_KEY,
-            secret=AWS_SECRET_KEY,
-            profile=AWS_PROFILE_NAME
-        )
-    elif protocol == Protocol.GCS:
-        return GCSFileSystem(token=GCS_SERVICE_ACCOUNT_KEY)
-
-    raise NotImplementedError(f'Protocol {protocol} is not supported')
-
-
-def prefix_for_protocol(protocol: Protocol) -> str:
-    if protocol == Protocol.LOCAL:
-        return ''
-    elif protocol == Protocol.S3:
-        return 's3://'
-    elif protocol == Protocol.GCS:
-        return 'gcs://'
-
-
-def protocol_path_split(uri: str) -> Tuple[Protocol, str]:
-    if uri.startswith('s3://'):
-        split = Protocol.S3, uri[5:]
-    elif uri.startswith('gcs://'):
-        split = Protocol.GCS, uri[6:]
-    elif uri.startswith('gs://'):
-        split = Protocol.GCS, uri[5:]
-    else:
-        split = Protocol.LOCAL, uri
-    check_access_to_uri(filesystem_for_protocol(split[0]), split[1])
-    return split
-
-
-def check_access_to_uri(fs: AbstractFileSystem, path: str):
-    try:
-        fs.exists(path)
-    except gcsfs.retry.HttpError as e:
-        raise ValueError(f'{e.message}. Pass credentials or run the command "gcloud auth application-default login" '
-                         f'to authenticate')
-
-
-def filesystem_path_split(uri: str) -> Tuple[AbstractFileSystem, str]:
-    protocol, path = protocol_path_split(uri)
-    fs = filesystem_for_protocol(protocol)
-
-    assert fs is not None
-
-    check_access_to_uri(fs, path)
-
-    return fs, path
-
-
-def vzg_open(uri: str, mode: str):
-    protocol, path = protocol_path_split(uri)
-    fs = filesystem_for_protocol(protocol)
-
-    assert fs is not None
-
-    return fs.open(path, mode)
-
-
-def __get_rasterio_session(uri: str):
-    warnings.filterwarnings('ignore', category=NotGeoreferencedWarning)
-    global AWS_PROFILE_NAME, AWS_ACCESS_KEY, AWS_SECRET_KEY, GCS_SERVICE_ACCOUNT_KEY
-
-    protocol, _ = protocol_path_split(uri)
-
-    if protocol == Protocol.LOCAL:
-        return rasterio.session.DummySession()
-    elif protocol == Protocol.S3:
-        return rasterio.session.AWSSession(
-            aws_access_key_id=AWS_ACCESS_KEY,
-            aws_secret_access_key=AWS_SECRET_KEY,
-            profile_name=AWS_PROFILE_NAME
-        )
-    elif protocol == Protocol.GCS:
-        return rasterio.session.GSSession(
-            google_application_credentials=GCS_SERVICE_ACCOUNT_KEY
-        )
-
-    raise NotImplementedError(f'Protocol {protocol} is not supported')
-
-
-def rasterio_open(uri: str):
-    protocol, path = protocol_path_split(uri)
-
-    prefix = '/vsigs/' if protocol == Protocol.GCS else prefix_for_protocol(protocol)
-    rasterio_path = prefix + path
-
-    return rasterio.open(rasterio_path)
-
-
-def get_rasterio_environment(uri: str, gdal_cache_size: int = 512000000) -> rasterio.Env:
-    return rasterio.Env(__get_rasterio_session(uri), GDAL_CACHEMAX=gdal_cache_size)
+import json
+import os
+from enum import Enum
+from typing import Optional, Tuple
+
+import gcsfs
+import rasterio.session
+from fsspec import AbstractFileSystem
+from fsspec.implementations.local import LocalFileSystem
+from gcsfs import GCSFileSystem
+from s3fs import S3FileSystem
+
+import vpt.log as log
+
+import warnings
+from rasterio.errors import NotGeoreferencedWarning
+
+from vpt import AWS_PROFILE_NAME_VAR, GCS_SERVICE_ACCOUNT_KEY_VAR, AWS_SECRET_KEY_VAR, AWS_ACCESS_KEY_VAR
+
+
+class Protocol(Enum):
+    LOCAL = 0
+    S3 = 1
+    GCS = 2
+
+
+AWS_PROFILE_NAME = None
+AWS_ACCESS_KEY = None
+AWS_SECRET_KEY = None
+
+GCS_SERVICE_ACCOUNT_KEY = None
+
+
+def initialize_filesystem(
+        aws_access_key=None,
+        aws_secret_key=None,
+        aws_profile_name=None,
+        gcs_service_account_key=None
+):
+    global AWS_PROFILE_NAME, AWS_ACCESS_KEY, AWS_SECRET_KEY, GCS_SERVICE_ACCOUNT_KEY
+
+    if all([aws_profile_name, aws_access_key, aws_secret_key]):
+        log.warning('Both AWS profile name and access key/secret key pair are specified.')
+
+    AWS_PROFILE_NAME = aws_profile_name if aws_profile_name else os.environ.get(AWS_PROFILE_NAME_VAR)
+    AWS_ACCESS_KEY = aws_access_key if aws_access_key else os.environ.get(AWS_ACCESS_KEY_VAR)
+    AWS_SECRET_KEY = aws_secret_key if aws_secret_key else os.environ.get(AWS_SECRET_KEY_VAR)
+
+    if gcs_service_account_key:
+        GCS_SERVICE_ACCOUNT_KEY = gcs_service_account_key
+    else:
+        GCS_SERVICE_ACCOUNT_KEY = os.environ.get(GCS_SERVICE_ACCOUNT_KEY_VAR)
+        try:
+            GCS_SERVICE_ACCOUNT_KEY = json.loads(GCS_SERVICE_ACCOUNT_KEY)
+        except Exception:
+            pass
+
+
+def filesystem_for_protocol(protocol: Protocol) -> Optional[AbstractFileSystem]:
+    global AWS_PROFILE_NAME, AWS_ACCESS_KEY, AWS_SECRET_KEY, GCS_SERVICE_ACCOUNT_KEY
+
+    if protocol == Protocol.LOCAL:
+        return LocalFileSystem()
+    elif protocol == Protocol.S3:
+        return S3FileSystem(
+            key=AWS_ACCESS_KEY,
+            secret=AWS_SECRET_KEY,
+            profile=AWS_PROFILE_NAME
+        )
+    elif protocol == Protocol.GCS:
+        return GCSFileSystem(token=GCS_SERVICE_ACCOUNT_KEY)
+
+    raise NotImplementedError(f'Protocol {protocol} is not supported')
+
+
+def prefix_for_protocol(protocol: Protocol) -> str:
+    if protocol == Protocol.LOCAL:
+        return ''
+    elif protocol == Protocol.S3:
+        return 's3://'
+    elif protocol == Protocol.GCS:
+        return 'gcs://'
+
+
+def protocol_path_split(uri: str) -> Tuple[Protocol, str]:
+    if uri.startswith('s3://'):
+        split = Protocol.S3, uri[5:]
+    elif uri.startswith('gcs://'):
+        split = Protocol.GCS, uri[6:]
+    elif uri.startswith('gs://'):
+        split = Protocol.GCS, uri[5:]
+    else:
+        split = Protocol.LOCAL, uri
+    check_access_to_uri(filesystem_for_protocol(split[0]), split[1])
+    return split
+
+
+def check_access_to_uri(fs: AbstractFileSystem, path: str):
+    try:
+        fs.exists(path)
+    except gcsfs.retry.HttpError as e:
+        raise ValueError(f'{e.message}. Pass credentials or run the command "gcloud auth application-default login" '
+                         f'to authenticate')
+
+
+def filesystem_path_split(uri: str) -> Tuple[AbstractFileSystem, str]:
+    protocol, path = protocol_path_split(uri)
+    fs = filesystem_for_protocol(protocol)
+
+    assert fs is not None
+
+    check_access_to_uri(fs, path)
+
+    return fs, path
+
+
+def vzg_open(uri: str, mode: str):
+    protocol, path = protocol_path_split(uri)
+    fs = filesystem_for_protocol(protocol)
+
+    assert fs is not None
+
+    return fs.open(path, mode)
+
+
+def __get_rasterio_session(uri: str):
+    warnings.filterwarnings('ignore', category=NotGeoreferencedWarning)
+    global AWS_PROFILE_NAME, AWS_ACCESS_KEY, AWS_SECRET_KEY, GCS_SERVICE_ACCOUNT_KEY
+
+    protocol, _ = protocol_path_split(uri)
+
+    if protocol == Protocol.LOCAL:
+        return rasterio.session.DummySession()
+    elif protocol == Protocol.S3:
+        return rasterio.session.AWSSession(
+            aws_access_key_id=AWS_ACCESS_KEY,
+            aws_secret_access_key=AWS_SECRET_KEY,
+            profile_name=AWS_PROFILE_NAME
+        )
+    elif protocol == Protocol.GCS:
+        return rasterio.session.GSSession(
+            google_application_credentials=GCS_SERVICE_ACCOUNT_KEY
+        )
+
+    raise NotImplementedError(f'Protocol {protocol} is not supported')
+
+
+def rasterio_open(uri: str):
+    protocol, path = protocol_path_split(uri)
+
+    prefix = '/vsigs/' if protocol == Protocol.GCS else prefix_for_protocol(protocol)
+    rasterio_path = prefix + path
+
+    return rasterio.open(rasterio_path)
+
+
+def get_rasterio_environment(uri: str, gdal_cache_size: int = 512000000) -> rasterio.Env:
+    return rasterio.Env(__get_rasterio_session(uri), GDAL_CACHEMAX=gdal_cache_size)
```

### Comparing `vpt-1.0.1/src/vpt/log.py` & `vpt-1.0.2/src/vpt/log.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,93 +1,93 @@
-import logging
-import pathlib
-import sys
-
-from tqdm import tqdm
-
-_t_id = '/'
-
-
-class VPTFormatter(logging.Formatter):
-    def format(self, record: logging.LogRecord) -> str:
-        record.tid = _t_id
-        return super().format(record)
-
-
-vpt_logger = logging.getLogger('vpt')
-logger: logging.Logger = vpt_logger
-h_stdout = logging.StreamHandler(sys.stdout)
-formatter = VPTFormatter('%(asctime)s - %(tid)s - %(levelname)s - %(message)s')
-h_stdout.setFormatter(formatter)
-
-
-def set_logger(user_logger: logging.Logger):
-    global logger, vpt_logger
-    vpt_logger = logger
-    logger = user_logger
-    set_verbose(True)
-
-
-def release_logger():
-    global logger, vpt_logger
-    logger = vpt_logger
-
-
-def set_process_name(proc_name: str):
-    global _t_id
-    _t_id = proc_name
-
-
-def initialize_logger(fname: str, lvl: int = 1, verbose: bool = False) -> None:
-    logger.setLevel(lvl * 10)
-    if fname:
-        pathlib.Path(fname).parent.mkdir(parents=True, exist_ok=True)
-        set_log_file(fname)
-    set_verbose(verbose)
-
-
-def set_log_file(fname: str) -> None:
-    fh = logging.FileHandler(filename=fname)
-    fh.setFormatter(formatter)
-    logger.addHandler(fh)
-
-
-def set_verbose(v: bool = True) -> None:
-    std_in = is_verbose()
-    if std_in == v:
-        return
-    if v:
-        logger.addHandler(h_stdout)
-    else:
-        logger.removeHandler(h_stdout)
-
-
-def is_verbose() -> bool:
-    return h_stdout in logger.handlers
-
-
-def show_progress(iterable, *args, **kwargs):
-    return iterable if not is_verbose() else tqdm(iterable, *args, **kwargs)
-
-
-def debug(msg, *args, **kwargs):
-    logger.debug(msg, *args, **kwargs)
-
-
-def info(msg, *args, **kwargs):
-    logger.info(msg, *args, **kwargs)
-
-
-def warning(msg, *args, **kwargs):
-    logger.warning(msg, *args, **kwargs)
-
-
-def error(msg, *args, **kwargs):
-    logger.error(msg, *args, **kwargs)
-
-
-def exception(msg, *args, **kwargs):
-    logger.error(msg, *args, exc_info=True, **kwargs)
-
-
-def critical(msg, *args, **kwargs):
-    logger.critical(msg, *args, **kwargs)
+import logging
+import pathlib
+import sys
+
+from tqdm import tqdm
+
+_t_id = '/'
+
+
+class VPTFormatter(logging.Formatter):
+    def format(self, record: logging.LogRecord) -> str:
+        record.tid = _t_id
+        return super().format(record)
+
+
+vpt_logger = logging.getLogger('vpt')
+logger: logging.Logger = vpt_logger
+h_stdout = logging.StreamHandler(sys.stdout)
+formatter = VPTFormatter('%(asctime)s - %(tid)s - %(levelname)s - %(message)s')
+h_stdout.setFormatter(formatter)
+
+
+def set_logger(user_logger: logging.Logger):
+    global logger, vpt_logger
+    vpt_logger = logger
+    logger = user_logger
+    set_verbose(True)
+
+
+def release_logger():
+    global logger, vpt_logger
+    logger = vpt_logger
+
+
+def set_process_name(proc_name: str):
+    global _t_id
+    _t_id = proc_name
+
+
+def initialize_logger(fname: str, lvl: int = 1, verbose: bool = False) -> None:
+    logger.setLevel(lvl * 10)
+    if fname:
+        pathlib.Path(fname).parent.mkdir(parents=True, exist_ok=True)
+        set_log_file(fname)
+    set_verbose(verbose)
+
+
+def set_log_file(fname: str) -> None:
+    fh = logging.FileHandler(filename=fname)
+    fh.setFormatter(formatter)
+    logger.addHandler(fh)
+
+
+def set_verbose(v: bool = True) -> None:
+    std_in = is_verbose()
+    if std_in == v:
+        return
+    if v:
+        logger.addHandler(h_stdout)
+    else:
+        logger.removeHandler(h_stdout)
+
+
+def is_verbose() -> bool:
+    return h_stdout in logger.handlers
+
+
+def show_progress(iterable, *args, **kwargs):
+    return iterable if not is_verbose() else tqdm(iterable, *args, **kwargs)
+
+
+def debug(msg, *args, **kwargs):
+    logger.debug(msg, *args, **kwargs)
+
+
+def info(msg, *args, **kwargs):
+    logger.info(msg, *args, **kwargs)
+
+
+def warning(msg, *args, **kwargs):
+    logger.warning(msg, *args, **kwargs)
+
+
+def error(msg, *args, **kwargs):
+    logger.error(msg, *args, **kwargs)
+
+
+def exception(msg, *args, **kwargs):
+    logger.error(msg, *args, exc_info=True, **kwargs)
+
+
+def critical(msg, *args, **kwargs):
+    logger.critical(msg, *args, **kwargs)
```

### Comparing `vpt-1.0.1/src/vpt/partition_transcripts/cell_x_gene.py` & `vpt-1.0.2/src/vpt/partition_transcripts/cell_x_gene.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,123 +1,123 @@
-import numpy as np
-import pandas as pd
-import shapely
-
-from vpt.filesystem import vzg_open
-from vpt.utils.boundaries import Boundaries
-
-
-def process_chunk(chunk_df, shapely_list, z_planes_count, cell_id_list, needs_new_dt: bool = False):
-    genes_detected = chunk_df["gene"].unique()
-    grouped = chunk_df.groupby(chunk_df["gene"])
-
-    gene_df_list = []
-    transcripts_list = []
-    for gene in genes_detected:
-        one_gene = grouped.get_group(gene)
-        one_gene_partition_list = []
-        for z in range(z_planes_count):
-            one_gene_z = one_gene.loc[one_gene["global_z"] == z]
-            points = shapely.points(one_gene_z["global_x"], one_gene_z["global_y"])
-            one_gene_tree = shapely.STRtree(points)
-            one_gene_partition_z = one_gene_tree.query(shapely_list[z], predicate='contains')
-            one_gene_partition_list.append(one_gene_partition_z)
-
-            if needs_new_dt:
-                out = np.full(len(one_gene_z), -1, dtype=np.int64)
-                if len(one_gene_partition_z[0]) > 0:
-                    cell_id_vectorize = np.vectorize(lambda t: cell_id_list[t])
-                    out[one_gene_partition_z[1]] = cell_id_vectorize(one_gene_partition_z[0])
-
-                one_gene_z = one_gene_z.assign(cell_id=out)
-
-                transcripts_list.append(one_gene_z)
-
-        if one_gene_partition_list:
-            one_gene_partition = np.concatenate(one_gene_partition_list, axis=1)
-        else:
-            one_gene_partition = np.array([[], []])
-
-        cell_x_one_gene = pd.DataFrame(
-            one_gene_partition.T,
-            columns=["cell_id", gene]
-        ).groupby(
-            "cell_id"
-        ).count()
-        gene_df_list.append(cell_x_one_gene)
-
-    cell_x_gene = pd.DataFrame(
-        index=range(len(cell_id_list))
-    ).join(
-        gene_df_list
-    ).fillna(0)
-    cell_x_gene['cell'] = pd.to_numeric(cell_id_list)
-    return cell_x_gene, transcripts_list
-
-
-def construct_cell_x_gene(
-        transcripts,
-        geometry_list,
-        z_planes_count: int,
-        cell_id_list,
-        outputTranscripts: str or None = None
-) -> pd.DataFrame:
-    cell_by_gene = pd.DataFrame(
-        {'cell': pd.to_numeric(cell_id_list)}
-    )
-    barcode_id_name_df = pd.DataFrame(columns=['barcode_id', 'gene'])
-
-    first_chunk = True
-    for chunk_df in transcripts:
-        chunk_cell_by_gene, transcripts_list = \
-            process_chunk(chunk_df, geometry_list, z_planes_count, cell_id_list, outputTranscripts)
-
-        cell_by_gene = pd.concat([cell_by_gene, chunk_cell_by_gene]).groupby('cell'). \
-            sum(min_count=1).fillna(0).reset_index()
-
-        barcode_id_name_df = pd.concat([barcode_id_name_df, chunk_df[['barcode_id', 'gene']]]
-                                       ).drop_duplicates(subset='barcode_id')
-        if outputTranscripts is None or len(transcripts_list) == 0:
-            continue
-
-        transcripts_df = pd.concat(transcripts_list).loc[chunk_df.index]
-        transcripts_df = transcripts_df.rename(columns={transcripts_df.columns[0]: ''})
-        if first_chunk:
-            with vzg_open(outputTranscripts, 'w') as f:
-                transcripts_df.to_csv(f, mode='w', index=False, header=True)
-            first_chunk = False
-            continue
-
-        with vzg_open(outputTranscripts, 'a') as f:
-            transcripts_df.to_csv(f, mode='a', index=False, header=False)
-
-    cell_by_gene.set_index('cell', inplace=True, drop=True)
-    cell_by_gene.index = cell_by_gene.index.astype(np.int64)
-    cell_by_gene.index.name = 'cell'
-    cell_by_gene = cell_by_gene.sort_index()
-
-    barcode_id_name_df = barcode_id_name_df.set_index('barcode_id')
-    barcode_id_name_df.sort_index(inplace=True)
-    cell_by_gene = cell_by_gene.reindex(list(barcode_id_name_df['gene']), axis=1)
-    return cell_by_gene.astype("int")
-
-
-def cell_by_gene_matrix(bnds: Boundaries, transcripts: pd.DataFrame,
-                        outputTranscripts: str or None = None) -> pd.DataFrame:
-    idList = []
-    geomList = []
-    for z in range(bnds.get_z_planes_count()):
-        geomList.append([])
-    for feature in bnds.features:
-        idList.append(np.int64(feature.get_feature_id()))
-        for zIdx, poly in enumerate(feature.get_full_cell()):
-            geomList[zIdx].append(poly)
-
-    cell_x_gene = construct_cell_x_gene(
-        transcripts,
-        np.array(geomList),
-        bnds.get_z_planes_count(),
-        idList,
-        outputTranscripts
-    )
-
-    return cell_x_gene
+import numpy as np
+import pandas as pd
+import shapely
+
+from vpt.filesystem import vzg_open
+from vpt.utils.boundaries import Boundaries
+
+
+def process_chunk(chunk_df, shapely_list, z_planes_count, cell_id_list, needs_new_dt: bool = False):
+    genes_detected = chunk_df["gene"].unique()
+    grouped = chunk_df.groupby(chunk_df["gene"])
+
+    gene_df_list = []
+    transcripts_list = []
+    for gene in genes_detected:
+        one_gene = grouped.get_group(gene)
+        one_gene_partition_list = []
+        for z in range(z_planes_count):
+            one_gene_z = one_gene.loc[one_gene["global_z"] == z]
+            points = shapely.points(one_gene_z["global_x"], one_gene_z["global_y"])
+            one_gene_tree = shapely.STRtree(points)
+            one_gene_partition_z = one_gene_tree.query(shapely_list[z], predicate='contains')
+            one_gene_partition_list.append(one_gene_partition_z)
+
+            if needs_new_dt:
+                out = np.full(len(one_gene_z), -1, dtype=np.int64)
+                if len(one_gene_partition_z[0]) > 0:
+                    cell_id_vectorize = np.vectorize(lambda t: cell_id_list[t])
+                    out[one_gene_partition_z[1]] = cell_id_vectorize(one_gene_partition_z[0])
+
+                one_gene_z = one_gene_z.assign(cell_id=out)
+
+                transcripts_list.append(one_gene_z)
+
+        if one_gene_partition_list:
+            one_gene_partition = np.concatenate(one_gene_partition_list, axis=1)
+        else:
+            one_gene_partition = np.array([[], []])
+
+        cell_x_one_gene = pd.DataFrame(
+            one_gene_partition.T,
+            columns=["cell_id", gene]
+        ).groupby(
+            "cell_id"
+        ).count()
+        gene_df_list.append(cell_x_one_gene)
+
+    cell_x_gene = pd.DataFrame(
+        index=range(len(cell_id_list))
+    ).join(
+        gene_df_list
+    ).fillna(0)
+    cell_x_gene['cell'] = pd.to_numeric(cell_id_list)
+    return cell_x_gene, transcripts_list
+
+
+def construct_cell_x_gene(
+        transcripts,
+        geometry_list,
+        z_planes_count: int,
+        cell_id_list,
+        outputTranscripts: str or None = None
+) -> pd.DataFrame:
+    cell_by_gene = pd.DataFrame(
+        {'cell': pd.to_numeric(cell_id_list)}
+    )
+    barcode_id_name_df = pd.DataFrame(columns=['barcode_id', 'gene'])
+
+    first_chunk = True
+    for chunk_df in transcripts:
+        chunk_cell_by_gene, transcripts_list = \
+            process_chunk(chunk_df, geometry_list, z_planes_count, cell_id_list, outputTranscripts)
+
+        cell_by_gene = pd.concat([cell_by_gene, chunk_cell_by_gene]).groupby('cell'). \
+            sum(min_count=1).fillna(0).reset_index()
+
+        barcode_id_name_df = pd.concat([barcode_id_name_df, chunk_df[['barcode_id', 'gene']]]
+                                       ).drop_duplicates(subset='barcode_id')
+        if outputTranscripts is None or len(transcripts_list) == 0:
+            continue
+
+        transcripts_df = pd.concat(transcripts_list).loc[chunk_df.index]
+        transcripts_df = transcripts_df.rename(columns={transcripts_df.columns[0]: ''})
+        if first_chunk:
+            with vzg_open(outputTranscripts, 'w') as f:
+                transcripts_df.to_csv(f, mode='w', index=False, header=True)
+            first_chunk = False
+            continue
+
+        with vzg_open(outputTranscripts, 'a') as f:
+            transcripts_df.to_csv(f, mode='a', index=False, header=False)
+
+    cell_by_gene.set_index('cell', inplace=True, drop=True)
+    cell_by_gene.index = cell_by_gene.index.astype(np.int64)
+    cell_by_gene.index.name = 'cell'
+    cell_by_gene = cell_by_gene.sort_index()
+
+    barcode_id_name_df = barcode_id_name_df.set_index('barcode_id')
+    barcode_id_name_df.sort_index(inplace=True)
+    cell_by_gene = cell_by_gene.reindex(list(barcode_id_name_df['gene']), axis=1)
+    return cell_by_gene.astype("int")
+
+
+def cell_by_gene_matrix(bnds: Boundaries, transcripts: pd.DataFrame,
+                        outputTranscripts: str or None = None) -> pd.DataFrame:
+    idList = []
+    geomList = []
+    for z in range(bnds.get_z_planes_count()):
+        geomList.append([])
+    for feature in bnds.features:
+        idList.append(np.int64(feature.get_feature_id()))
+        for zIdx, poly in enumerate(feature.get_full_cell()):
+            geomList[zIdx].append(poly)
+
+    cell_x_gene = construct_cell_x_gene(
+        transcripts,
+        np.array(geomList),
+        bnds.get_z_planes_count(),
+        idList,
+        outputTranscripts
+    )
+
+    return cell_x_gene
```

### Comparing `vpt-1.0.1/src/vpt/partition_transcripts/cmd_args.py` & `vpt-1.0.2/src/vpt/partition_transcripts/cmd_args.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,68 +1,68 @@
-from argparse import ArgumentParser
-from dataclasses import dataclass
-
-from vpt.utils.validate import validate_exists, validate_does_not_exist
-from vpt.filesystem import vzg_open
-
-
-@dataclass
-class PartitionTranscriptsArgs:
-    input_boundaries: str
-    input_transcripts: str
-    output_entity_by_gene: str
-    chunk_size: int
-    output_transcripts: str
-    overwrite: bool
-
-
-def validate_args(args: PartitionTranscriptsArgs):
-    validate_exists(args.input_boundaries)
-    validate_exists(args.input_transcripts)
-
-    if not args.overwrite:
-        validate_does_not_exist(args.output_entity_by_gene)
-        if args.output_transcripts:
-            validate_does_not_exist(args.output_transcripts)
-
-    if args.chunk_size <= 0:
-        raise ValueError('Chunk size should be a positive integer')
-
-    transcripts_header = {'gene', 'global_x', 'global_y', 'global_z'}
-    with vzg_open(args.input_transcripts, 'r') as f:
-        header = f.readline()
-        header = header.replace('\n', '').split(',')
-        if not transcripts_header.issubset(header):
-            raise ValueError(f'Expected columns {transcripts_header.difference(header)} were not found in the '
-                             f'input-transcripts file. Input transcript file contained columns: {header}')
-
-
-def get_parser() -> ArgumentParser:
-    parser = ArgumentParser(description='Uses the segmentation boundaries to determine which Entity, if any, contains each '
-                            'detected transcript. Outputs an Entity by gene matrix, and may optionally output '
-                            'a detected transcript csv with an additional column indicating the containing Entity.',
-                            add_help=False
-                            )
-    required = parser.add_argument_group('Required arguments')
-    required.add_argument('--input-boundaries', required=True, type=str,
-                          help='Path to a micron-space parquet boundary file.')
-    required.add_argument('--input-transcripts', required=True, type=str,
-                          help='Path to an existing transcripts csv file.')
-    required.add_argument('--output-entity-by-gene', required=True, type=str,
-                          help='Path to output the Entity by gene matrix csv file.')
-
-    opt = parser.add_argument_group('Optional arguments')
-    opt.add_argument('--chunk-size', required=False, type=int, default=10000000,
-                     help='Number of transcript file lines to be loaded in memory at once. Default: 10,000,000')
-    opt.add_argument('--output-transcripts', required=False, type=str,
-                     help='If a filename is provided, a copy of the detected transcripts file will be written '
-                     'with an additional column with the EntityID of the cell or other Entity that contains '
-                     'each transcript (or -1 if the transcript is not contained by any Entity).')
-    opt.add_argument('--overwrite', action='store_true', default=False, required=False,
-                     help='Set flag if you want to use non empty directory and agree that files can be over-written.')
-    opt.add_argument("-h", "--help", action="help", help="Show this help message and exit")
-
-    return parser
-
-
-def parse_args():
-    return get_parser().parse_args()
+from argparse import ArgumentParser
+from dataclasses import dataclass
+
+from vpt.utils.validate import validate_exists, validate_does_not_exist
+from vpt.filesystem import vzg_open
+
+
+@dataclass
+class PartitionTranscriptsArgs:
+    input_boundaries: str
+    input_transcripts: str
+    output_entity_by_gene: str
+    chunk_size: int
+    output_transcripts: str
+    overwrite: bool
+
+
+def validate_args(args: PartitionTranscriptsArgs):
+    validate_exists(args.input_boundaries)
+    validate_exists(args.input_transcripts)
+
+    if not args.overwrite:
+        validate_does_not_exist(args.output_entity_by_gene)
+        if args.output_transcripts:
+            validate_does_not_exist(args.output_transcripts)
+
+    if args.chunk_size <= 0:
+        raise ValueError('Chunk size should be a positive integer')
+
+    transcripts_header = {'gene', 'global_x', 'global_y', 'global_z'}
+    with vzg_open(args.input_transcripts, 'r') as f:
+        header = f.readline()
+        header = header.replace('\n', '').split(',')
+        if not transcripts_header.issubset(header):
+            raise ValueError(f'Expected columns {transcripts_header.difference(header)} were not found in the '
+                             f'input-transcripts file. Input transcript file contained columns: {header}')
+
+
+def get_parser() -> ArgumentParser:
+    parser = ArgumentParser(description='Uses the segmentation boundaries to determine which Entity, if any, contains each '
+                            'detected transcript. Outputs an Entity by gene matrix, and may optionally output '
+                            'a detected transcript csv with an additional column indicating the containing Entity.',
+                            add_help=False
+                            )
+    required = parser.add_argument_group('Required arguments')
+    required.add_argument('--input-boundaries', required=True, type=str,
+                          help='Path to a micron-space parquet boundary file.')
+    required.add_argument('--input-transcripts', required=True, type=str,
+                          help='Path to an existing transcripts csv file.')
+    required.add_argument('--output-entity-by-gene', required=True, type=str,
+                          help='Path to output the Entity by gene matrix csv file.')
+
+    opt = parser.add_argument_group('Optional arguments')
+    opt.add_argument('--chunk-size', required=False, type=int, default=10000000,
+                     help='Number of transcript file lines to be loaded in memory at once. Default: 10,000,000')
+    opt.add_argument('--output-transcripts', required=False, type=str,
+                     help='If a filename is provided, a copy of the detected transcripts file will be written '
+                     'with an additional column with the EntityID of the cell or other Entity that contains '
+                     'each transcript (or -1 if the transcript is not contained by any Entity).')
+    opt.add_argument('--overwrite', action='store_true', default=False, required=False,
+                     help='Set flag if you want to use non empty directory and agree that files can be over-written.')
+    opt.add_argument("-h", "--help", action="help", help="Show this help message and exit")
+
+    return parser
+
+
+def parse_args():
+    return get_parser().parse_args()
```

### Comparing `vpt-1.0.1/src/vpt/partition_transcripts/run_partition_transcripts.py` & `vpt-1.0.2/src/vpt/partition_transcripts/run_partition_transcripts.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-import argparse
-import warnings
-import pandas as pd
-
-from vpt.filesystem import vzg_open
-from vpt.partition_transcripts.cell_x_gene import cell_by_gene_matrix
-from vpt.partition_transcripts.cmd_args import validate_args
-from vpt.utils.boundaries import Boundaries
-from vpt.utils.cellsreader import CellsReader, cell_reader_factory
-from vpt.utils.output_tools import make_parent_dirs
-import vpt.log as log
-
-
-def main_partition_transcripts(args: argparse.Namespace) -> None:
-    # Suppress parquet / Arrow warnings
-    warnings.filterwarnings('ignore', category=UserWarning)
-
-    validate_args(args)
-    log.info('Partition transcripts started')
-
-    cellsReader: CellsReader = cell_reader_factory(args.input_boundaries)
-    bnds = Boundaries(cellsReader)
-
-    with vzg_open(args.input_transcripts, 'r') as f:
-        chunks = pd.read_csv(f, chunksize=args.chunk_size)
-        if args.output_transcripts:
-            make_parent_dirs(args.output_transcripts)
-
-        cell_x_gene = cell_by_gene_matrix(bnds, chunks, args.output_transcripts)
-
-    make_parent_dirs(args.output_entity_by_gene)
-    with vzg_open(args.output_entity_by_gene, "w") as f:
-        cell_x_gene.to_csv(f)
-    log.info(f'cell by gene matrix saved as {args.output_entity_by_gene}')
-
-    if args.output_transcripts:
-        log.info(f'detected transcripts saved as {args.output_transcripts}')
-
-    log.info('Partition transcripts finished')
+import argparse
+import warnings
+import pandas as pd
+
+from vpt.filesystem import vzg_open
+from vpt.partition_transcripts.cell_x_gene import cell_by_gene_matrix
+from vpt.partition_transcripts.cmd_args import validate_args
+from vpt.utils.boundaries import Boundaries
+from vpt.utils.cellsreader import CellsReader, cell_reader_factory
+from vpt.utils.output_tools import make_parent_dirs
+import vpt.log as log
+
+
+def main_partition_transcripts(args: argparse.Namespace) -> None:
+    # Suppress parquet / Arrow warnings
+    warnings.filterwarnings('ignore', category=UserWarning)
+
+    validate_args(args)
+    log.info('Partition transcripts started')
+
+    cellsReader: CellsReader = cell_reader_factory(args.input_boundaries)
+    bnds = Boundaries(cellsReader)
+
+    with vzg_open(args.input_transcripts, 'r') as f:
+        chunks = pd.read_csv(f, chunksize=args.chunk_size)
+        if args.output_transcripts:
+            make_parent_dirs(args.output_transcripts)
+
+        cell_x_gene = cell_by_gene_matrix(bnds, chunks, args.output_transcripts)
+
+    make_parent_dirs(args.output_entity_by_gene)
+    with vzg_open(args.output_entity_by_gene, "w") as f:
+        cell_x_gene.to_csv(f)
+    log.info(f'cell by gene matrix saved as {args.output_entity_by_gene}')
+
+    if args.output_transcripts:
+        log.info(f'detected transcripts saved as {args.output_transcripts}')
+
+    log.info('Partition transcripts finished')
```

### Comparing `vpt-1.0.1/src/vpt/prepare_segmentation/cmd_args.py` & `vpt-1.0.2/src/vpt/prepare_segmentation/cmd_args.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,73 +1,73 @@
-from argparse import ArgumentParser
-from dataclasses import dataclass
-
-from vpt.filesystem.vzgfs import filesystem_path_split
-from vpt.prepare_segmentation.constants import OUTPUT_FILE_NAME
-from vpt.utils.validate import validate_exists, validate_does_not_exist
-
-
-@dataclass(frozen=True)
-class PrepareSegmentationArgs:
-    segmentation_algorithm: str
-    input_images: str
-    input_micron_to_mosaic: str
-    tile_size: int
-    tile_overlap: int
-    output_path: str
-    overwrite: bool
-
-
-def validate_prepare_segmentation_args(args: PrepareSegmentationArgs):
-    validate_exists(args.input_micron_to_mosaic)
-
-    if args.tile_size <= 0:
-        raise ValueError('Tile size should be positive')
-    if args.tile_overlap < 0 or args.tile_overlap > args.tile_size:
-        raise ValueError('Tile overlap should be in [0, tile-size] range')
-
-    if not args.overwrite:
-        fs, path_inside_fs = filesystem_path_split(args.output_path)
-        if fs.exists(path_inside_fs):
-            validate_does_not_exist(args.output_path + '/' + OUTPUT_FILE_NAME)
-
-
-def get_parser() -> ArgumentParser:
-    parser = ArgumentParser(description='Generates a segmentation specification json file to be used for cell segmentation '
-                            'tasks. The segmentation specification json includes specification for the algorithm to run, '
-                            'the paths for all images for each stain for each z index, the micron to mosaic pixel '
-                            'transformation matrix, the number of tiles, and the window coordinates for each tile.',
-                            add_help=False
-                            )
-
-    required = parser.add_argument_group('Required arguments')
-    required.add_argument('--segmentation-algorithm', type=str, required=True,
-                          help='Path to a json file that fully specifies the segmentation algorithm to use, '
-                               'including algorithm name, any algorithm specific parameters '
-                               '(including path to weights for new model), stains corresponding to each channel '
-                               'in the algorithm.')
-    required.add_argument('--input-images', type=str, required=True,
-                          help=r'Regular expression containing path that indicates the images to use '
-                               r'for the segmentation. The regular expressions can indicate the z index '
-                               r'(indicated by (?P<z>[0-9]+)) and/or multiple stains (indicated by '
-                               r'(?P<stain>[\w|-]+)). Here, <stain> must match the stains specified in the '
-                               r'segmentation algorithm.')
-    required.add_argument('--output-path', type=str, required=True,
-                          help='Path where the segmentation specification json file will be saved.')
-    required.add_argument('--input-micron-to-mosaic', type=str, required=True,
-                          help='Path to the micron to mosaic pixel transformation matrix.')
-
-    opt = parser.add_argument_group('Optional arguments')
-    opt.add_argument('--tile-size', type=int, default=4096,
-                     help='Number of pixels for the width and height of each tile. '
-                          'Each tile is created as a square. Default is 4096.')
-    opt.add_argument('--tile-overlap', type=int, required=False,
-                     help='Overlap between adjacent tiles. Default is 10%% of tile-size.')
-    opt.add_argument('--overwrite', action='store_true', default=False, required=False,
-                     help='Set flag if you want to use non empty directory and agree that files can be over-written.')
-    opt.add_argument("-h", "--help", action="help", help="Show this help message and exit")
-
-    return parser
-
-
-def parse_args():
-    return get_parser().parse_args()
+from argparse import ArgumentParser
+from dataclasses import dataclass
+
+from vpt.filesystem.vzgfs import filesystem_path_split
+from vpt.prepare_segmentation.constants import OUTPUT_FILE_NAME
+from vpt.utils.validate import validate_exists, validate_does_not_exist
+
+
+@dataclass(frozen=True)
+class PrepareSegmentationArgs:
+    segmentation_algorithm: str
+    input_images: str
+    input_micron_to_mosaic: str
+    tile_size: int
+    tile_overlap: int
+    output_path: str
+    overwrite: bool
+
+
+def validate_prepare_segmentation_args(args: PrepareSegmentationArgs):
+    validate_exists(args.input_micron_to_mosaic)
+
+    if args.tile_size <= 0:
+        raise ValueError('Tile size should be positive')
+    if args.tile_overlap < 0 or args.tile_overlap > args.tile_size:
+        raise ValueError('Tile overlap should be in [0, tile-size] range')
+
+    if not args.overwrite:
+        fs, path_inside_fs = filesystem_path_split(args.output_path)
+        if fs.exists(path_inside_fs):
+            validate_does_not_exist(args.output_path + '/' + OUTPUT_FILE_NAME)
+
+
+def get_parser() -> ArgumentParser:
+    parser = ArgumentParser(description='Generates a segmentation specification json file to be used for cell segmentation '
+                            'tasks. The segmentation specification json includes specification for the algorithm to run, '
+                            'the paths for all images for each stain for each z index, the micron to mosaic pixel '
+                            'transformation matrix, the number of tiles, and the window coordinates for each tile.',
+                            add_help=False
+                            )
+
+    required = parser.add_argument_group('Required arguments')
+    required.add_argument('--segmentation-algorithm', type=str, required=True,
+                          help='Path to a json file that fully specifies the segmentation algorithm to use, '
+                               'including algorithm name, any algorithm specific parameters '
+                               '(including path to weights for new model), stains corresponding to each channel '
+                               'in the algorithm.')
+    required.add_argument('--input-images', type=str, required=True,
+                          help=r'Regular expression containing path that indicates the images to use '
+                               r'for the segmentation. The regular expressions can indicate the z index '
+                               r'(indicated by (?P<z>[0-9]+)) and/or multiple stains (indicated by '
+                               r'(?P<stain>[\w|-]+)). Here, <stain> must match the stains specified in the '
+                               r'segmentation algorithm.')
+    required.add_argument('--output-path', type=str, required=True,
+                          help='Path where the segmentation specification json file will be saved.')
+    required.add_argument('--input-micron-to-mosaic', type=str, required=True,
+                          help='Path to the micron to mosaic pixel transformation matrix.')
+
+    opt = parser.add_argument_group('Optional arguments')
+    opt.add_argument('--tile-size', type=int, default=4096,
+                     help='Number of pixels for the width and height of each tile. '
+                          'Each tile is created as a square. Default is 4096.')
+    opt.add_argument('--tile-overlap', type=int, required=False,
+                     help='Overlap between adjacent tiles. Default is 10%% of tile-size.')
+    opt.add_argument('--overwrite', action='store_true', default=False, required=False,
+                     help='Set flag if you want to use non empty directory and agree that files can be over-written.')
+    opt.add_argument("-h", "--help", action="help", help="Show this help message and exit")
+
+    return parser
+
+
+def parse_args():
+    return get_parser().parse_args()
```

### Comparing `vpt-1.0.1/src/vpt/prepare_segmentation/input_tools.py` & `vpt-1.0.2/src/vpt/prepare_segmentation/input_tools.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-import json
-from dataclasses import dataclass
-from typing import List, Dict, Set
-
-from vpt.filesystem.vzgfs import vzg_open
-
-
-@dataclass(frozen=True)
-class OutputFiles:
-    run_on_tile_dir: str
-    mosaic_geometry_file: str
-    micron_geometry_file: str
-    cell_metadata_file: str
-
-
-@dataclass(frozen=True)
-class AlgInfo:
-    raw: Dict
-    stains: Set[str]
-    z_layers: Set[int]
-    output_files: List[OutputFiles]
-
-
-def get_stain_set(alg_raw: Dict) -> Set[str]:
-    stains = set()
-
-    for task in alg_raw['segmentation_tasks']:
-        for data_instance in task['task_input_data']:
-            stains.add(data_instance['image_channel'])
-
-    return stains
-
-
-def get_z_layers_set(alg_raw: Dict) -> Set[int]:
-    layers = set()
-
-    for task in alg_raw['segmentation_tasks']:
-        layers |= set(task['z_layers'])
-
-    return layers
-
-
-def get_output_files(alg_raw: Dict) -> List[OutputFiles]:
-    return [OutputFiles(**files['files']) for files in alg_raw['output_files']]
-
-
-def read_algorithm_json(path: str) -> Dict:
-    with vzg_open(path, 'r') as f:
-        data = json.load(f)
-    return data
-
-
-def parse_algorithm_json(algorithm_json: Dict) -> AlgInfo:
-    stains = get_stain_set(algorithm_json)
-    z_layers = get_z_layers_set(algorithm_json)
-    output_files = get_output_files(algorithm_json)
-
-    return AlgInfo(raw=algorithm_json, stains=stains, z_layers=z_layers, output_files=output_files)
+import json
+from dataclasses import dataclass
+from typing import List, Dict, Set
+
+from vpt.filesystem.vzgfs import vzg_open
+
+
+@dataclass(frozen=True)
+class OutputFiles:
+    run_on_tile_dir: str
+    mosaic_geometry_file: str
+    micron_geometry_file: str
+    cell_metadata_file: str
+
+
+@dataclass(frozen=True)
+class AlgInfo:
+    raw: Dict
+    stains: Set[str]
+    z_layers: Set[int]
+    output_files: List[OutputFiles]
+
+
+def get_stain_set(alg_raw: Dict) -> Set[str]:
+    stains = set()
+
+    for task in alg_raw['segmentation_tasks']:
+        for data_instance in task['task_input_data']:
+            stains.add(data_instance['image_channel'])
+
+    return stains
+
+
+def get_z_layers_set(alg_raw: Dict) -> Set[int]:
+    layers = set()
+
+    for task in alg_raw['segmentation_tasks']:
+        layers |= set(task['z_layers'])
+
+    return layers
+
+
+def get_output_files(alg_raw: Dict) -> List[OutputFiles]:
+    return [OutputFiles(**files['files']) for files in alg_raw['output_files']]
+
+
+def read_algorithm_json(path: str) -> Dict:
+    with vzg_open(path, 'r') as f:
+        data = json.load(f)
+    return data
+
+
+def parse_algorithm_json(algorithm_json: Dict) -> AlgInfo:
+    stains = get_stain_set(algorithm_json)
+    z_layers = get_z_layers_set(algorithm_json)
+    output_files = get_output_files(algorithm_json)
+
+    return AlgInfo(raw=algorithm_json, stains=stains, z_layers=z_layers, output_files=output_files)
```

### Comparing `vpt-1.0.1/src/vpt/prepare_segmentation/main.py` & `vpt-1.0.2/src/vpt/prepare_segmentation/main.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,82 +1,82 @@
-from datetime import datetime
-from typing import Dict
-
-import numpy as np
-
-from vpt.prepare_segmentation.cmd_args import PrepareSegmentationArgs, validate_prepare_segmentation_args, parse_args
-from vpt.prepare_segmentation.input_tools import read_algorithm_json, parse_algorithm_json
-from vpt.prepare_segmentation.output_tools import save_to_json
-from vpt.segmentation.utils.seg_result import SegmentationResult
-from vpt.utils.input_utils import read_micron_to_mosaic_transform
-from vpt.utils.regex_tools import parse_regex
-from vpt.prepare_segmentation.tiles import make_tiles
-from vpt.prepare_segmentation.validate import validate_regex_and_alg_match, validate_alg_info
-import vpt.log as log
-
-
-def run_prepare_segmentation(args):
-    if args.tile_overlap is None:
-        args.tile_overlap = int(0.1 * args.tile_size)
-    args = PrepareSegmentationArgs(**vars(args))
-    log.info('prepare segmentation started')
-    validate_prepare_segmentation_args(args)
-
-    algorithm_json = read_algorithm_json(args.segmentation_algorithm)
-
-    m2m_transform = read_micron_to_mosaic_transform(args.input_micron_to_mosaic)
-
-    seg_spec = get_segmentation_spec(algorithm_json, args.input_images, m2m_transform, args.tile_size,
-                                     args.tile_overlap, args.segmentation_algorithm, args.input_micron_to_mosaic,
-                                     args.output_path, args.overwrite)
-
-    save_to_json(seg_spec, args.output_path)
-    log.info('prepare segmentation finished')
-
-
-def get_segmentation_spec(algorithm_json: Dict, input_images_regex: str, micron_to_mosaic_matrix: np.array,
-                          tile_size: int, tile_overlap: int, algorithm_path: str, micron_to_mosaic_path: str,
-                          output_path: str, overwrite: bool = False):
-    alg_info = parse_algorithm_json(algorithm_json)
-    validate_alg_info(alg_info, output_path, overwrite)
-
-    regex_info = parse_regex(input_images_regex)
-    validate_regex_and_alg_match(regex_info, alg_info)
-
-    timestamp = datetime.now().timestamp()
-
-    tile_info = make_tiles(regex_info.image_width, regex_info.image_height, tile_size, tile_overlap)
-    if len(tile_info) > SegmentationResult.MAX_TILE_ID:
-        raise OverflowError(f'Number of tiles in experiment could not be greater than {SegmentationResult.MAX_TILE_ID}')
-    return {
-        'timestamp': timestamp,
-        'input_args': {
-            "segmentation_algorithm": algorithm_path,
-            "input_path": input_images_regex,
-            "input_micron_to_mosaic_path": micron_to_mosaic_path,
-            "output_path": output_path,
-            "tile_size": tile_size,
-            "tile_overlap": tile_overlap
-        },
-        'input_data': {
-            'micron_to_mosaic_tform': micron_to_mosaic_matrix,
-            'z_layers': list(alg_info.z_layers),
-            'channels': list(alg_info.stains),
-            'images': [{'channel': image.channel,
-                        'z_layer': image.z_layer,
-                        'full_path': image.full_path}
-                       for image in regex_info.images if
-                       image.channel in alg_info.stains and image.z_layer in alg_info.z_layers]
-        },
-        'window_grid': {
-            'mosaic_size': [regex_info.image_width, regex_info.image_height],
-            'tile_size': [tile_size, tile_size],
-            'tile_overlap': tile_overlap,
-            'num_tiles': len(tile_info),
-            'windows': [[tile.top_left_x, tile.top_left_y, tile.size, tile.size] for tile in tile_info]
-        },
-        'segmentation_algorithm': alg_info.raw
-    }
-
-
-if __name__ == '__main__':
-    run_prepare_segmentation(parse_args())
+from datetime import datetime
+from typing import Dict
+
+import numpy as np
+
+from vpt.prepare_segmentation.cmd_args import PrepareSegmentationArgs, validate_prepare_segmentation_args, parse_args
+from vpt.prepare_segmentation.input_tools import read_algorithm_json, parse_algorithm_json
+from vpt.prepare_segmentation.output_tools import save_to_json
+from vpt.segmentation.utils.seg_result import SegmentationResult
+from vpt.utils.input_utils import read_micron_to_mosaic_transform
+from vpt.utils.regex_tools import parse_regex
+from vpt.prepare_segmentation.tiles import make_tiles
+from vpt.prepare_segmentation.validate import validate_regex_and_alg_match, validate_alg_info
+import vpt.log as log
+
+
+def run_prepare_segmentation(args):
+    if args.tile_overlap is None:
+        args.tile_overlap = int(0.1 * args.tile_size)
+    args = PrepareSegmentationArgs(**vars(args))
+    log.info('prepare segmentation started')
+    validate_prepare_segmentation_args(args)
+
+    algorithm_json = read_algorithm_json(args.segmentation_algorithm)
+
+    m2m_transform = read_micron_to_mosaic_transform(args.input_micron_to_mosaic)
+
+    seg_spec = get_segmentation_spec(algorithm_json, args.input_images, m2m_transform, args.tile_size,
+                                     args.tile_overlap, args.segmentation_algorithm, args.input_micron_to_mosaic,
+                                     args.output_path, args.overwrite)
+
+    save_to_json(seg_spec, args.output_path)
+    log.info('prepare segmentation finished')
+
+
+def get_segmentation_spec(algorithm_json: Dict, input_images_regex: str, micron_to_mosaic_matrix: np.array,
+                          tile_size: int, tile_overlap: int, algorithm_path: str, micron_to_mosaic_path: str,
+                          output_path: str, overwrite: bool = False):
+    alg_info = parse_algorithm_json(algorithm_json)
+    validate_alg_info(alg_info, output_path, overwrite)
+
+    regex_info = parse_regex(input_images_regex)
+    validate_regex_and_alg_match(regex_info, alg_info)
+
+    timestamp = datetime.now().timestamp()
+
+    tile_info = make_tiles(regex_info.image_width, regex_info.image_height, tile_size, tile_overlap)
+    if len(tile_info) > SegmentationResult.MAX_TILE_ID:
+        raise OverflowError(f'Number of tiles in experiment could not be greater than {SegmentationResult.MAX_TILE_ID}')
+    return {
+        'timestamp': timestamp,
+        'input_args': {
+            "segmentation_algorithm": algorithm_path,
+            "input_path": input_images_regex,
+            "input_micron_to_mosaic_path": micron_to_mosaic_path,
+            "output_path": output_path,
+            "tile_size": tile_size,
+            "tile_overlap": tile_overlap
+        },
+        'input_data': {
+            'micron_to_mosaic_tform': micron_to_mosaic_matrix,
+            'z_layers': list(alg_info.z_layers),
+            'channels': list(alg_info.stains),
+            'images': [{'channel': image.channel,
+                        'z_layer': image.z_layer,
+                        'full_path': image.full_path}
+                       for image in regex_info.images if
+                       image.channel in alg_info.stains and image.z_layer in alg_info.z_layers]
+        },
+        'window_grid': {
+            'mosaic_size': [regex_info.image_width, regex_info.image_height],
+            'tile_size': [tile_size, tile_size],
+            'tile_overlap': tile_overlap,
+            'num_tiles': len(tile_info),
+            'windows': [[tile.top_left_x, tile.top_left_y, tile.size, tile.size] for tile in tile_info]
+        },
+        'segmentation_algorithm': alg_info.raw
+    }
+
+
+if __name__ == '__main__':
+    run_prepare_segmentation(parse_args())
```

### Comparing `vpt-1.0.1/src/vpt/prepare_segmentation/tiles.py` & `vpt-1.0.2/src/vpt/prepare_segmentation/tiles.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from dataclasses import dataclass
-from typing import List
-
-
-@dataclass(frozen=True)
-class TileInfo:
-    top_left_x: int
-    top_left_y: int
-    size: int
-
-
-def make_tiles(image_width: int, image_height: int, tile_size: int, tile_overlap: int) -> List[TileInfo]:
-    window_size = tile_size + 2 * tile_overlap
-    window_overlap = tile_overlap
-
-    def one_dim_cut(start, end):
-        points = [start]
-        while points[-1] + 2 * window_size - window_overlap <= end:
-            points.append(points[-1] + window_size - window_overlap)
-        if points[-1] + window_size < end:
-            points.append(end - window_size)
-        return points
-
-    x_points = one_dim_cut(0, image_width)
-    y_points = one_dim_cut(0, image_height)
-    return [TileInfo(x, y, window_size) for y in y_points for x in x_points]
+from dataclasses import dataclass
+from typing import List
+
+
+@dataclass(frozen=True)
+class TileInfo:
+    top_left_x: int
+    top_left_y: int
+    size: int
+
+
+def make_tiles(image_width: int, image_height: int, tile_size: int, tile_overlap: int) -> List[TileInfo]:
+    window_size = tile_size + 2 * tile_overlap
+    window_overlap = tile_overlap
+
+    def one_dim_cut(start, end):
+        points = [start]
+        while points[-1] + 2 * window_size - window_overlap <= end:
+            points.append(points[-1] + window_size - window_overlap)
+        if points[-1] + window_size < end:
+            points.append(end - window_size)
+        return points
+
+    x_points = one_dim_cut(0, image_width)
+    y_points = one_dim_cut(0, image_height)
+    return [TileInfo(x, y, window_size) for y in y_points for x in x_points]
```

### Comparing `vpt-1.0.1/src/vpt/prepare_segmentation/validate.py` & `vpt-1.0.2/src/vpt/prepare_segmentation/validate.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-from typing import List
-
-from vpt.filesystem import filesystem_path_split
-from vpt.prepare_segmentation.input_tools import AlgInfo, OutputFiles
-from vpt.segmentation.factory import get_task_validator
-from vpt.segmentation.utils.seg_result import SegmentationResult
-from vpt.utils.regex_tools import RegexInfo
-from vpt.utils.validate import validate_does_not_exist, validate_directory_empty
-
-
-def validate_regex_and_alg_match(regex_info: RegexInfo, alg_info: AlgInfo):
-    parsed_z = set(image.z_layer for image in regex_info.images)
-    if not parsed_z.issuperset(alg_info.z_layers):
-        raise ValueError(f'Z planes from algorithm specification {alg_info.z_layers} do not match '
-                         f'z planes extracted from regular expression {parsed_z}')
-    parsed_stain = set(image.channel for image in regex_info.images)
-    if not parsed_stain.issuperset(alg_info.stains):
-        raise ValueError(f'Stains from algorithm specification {alg_info.stains} do not match '
-                         f'stains from the regular expression{parsed_stain}')
-
-
-def validate_output_files_do_not_exist(output_root: str, output_files: List[OutputFiles]):
-    output_fs, _ = filesystem_path_split(output_root)
-
-    for files in output_files:
-        for file in (files.cell_metadata_file,
-                     files.micron_geometry_file,
-                     files.mosaic_geometry_file):
-            validate_does_not_exist(output_fs.sep.join([output_root, file]))
-
-        validate_directory_empty(output_fs.sep.join([output_root, files.run_on_tile_dir]))
-
-
-# todo: return valid, do not change input
-def validate_alg_info(alg_info: AlgInfo, output_path: str, overwrite: bool):
-    if len(alg_info.raw['segmentation_tasks']) > SegmentationResult.MAX_TASK_ID:
-        raise OverflowError(f'More than {SegmentationResult.MAX_TASK_ID} tasks could not be specified')
-
-    alg_info.raw['segmentation_tasks'] = [get_task_validator(t['segmentation_family'])(t) for t in
-                                          alg_info.raw['segmentation_tasks']]
-
-    if not overwrite:
-        validate_output_files_do_not_exist(output_path, alg_info.output_files)
+from typing import List
+
+from vpt.filesystem import filesystem_path_split
+from vpt.prepare_segmentation.input_tools import AlgInfo, OutputFiles
+from vpt.segmentation.factory import get_task_validator
+from vpt.segmentation.utils.seg_result import SegmentationResult
+from vpt.utils.regex_tools import RegexInfo
+from vpt.utils.validate import validate_does_not_exist, validate_directory_empty
+
+
+def validate_regex_and_alg_match(regex_info: RegexInfo, alg_info: AlgInfo):
+    parsed_z = set(image.z_layer for image in regex_info.images)
+    if not parsed_z.issuperset(alg_info.z_layers):
+        raise ValueError(f'Z planes from algorithm specification {alg_info.z_layers} do not match '
+                         f'z planes extracted from regular expression {parsed_z}')
+    parsed_stain = set(image.channel for image in regex_info.images)
+    if not parsed_stain.issuperset(alg_info.stains):
+        raise ValueError(f'Stains from algorithm specification {alg_info.stains} do not match '
+                         f'stains from the regular expression{parsed_stain}')
+
+
+def validate_output_files_do_not_exist(output_root: str, output_files: List[OutputFiles]):
+    output_fs, _ = filesystem_path_split(output_root)
+
+    for files in output_files:
+        for file in (files.cell_metadata_file,
+                     files.micron_geometry_file,
+                     files.mosaic_geometry_file):
+            validate_does_not_exist(output_fs.sep.join([output_root, file]))
+
+        validate_directory_empty(output_fs.sep.join([output_root, files.run_on_tile_dir]))
+
+
+# todo: return valid, do not change input
+def validate_alg_info(alg_info: AlgInfo, output_path: str, overwrite: bool):
+    if len(alg_info.raw['segmentation_tasks']) > SegmentationResult.MAX_TASK_ID:
+        raise OverflowError(f'More than {SegmentationResult.MAX_TASK_ID} tasks could not be specified')
+
+    alg_info.raw['segmentation_tasks'] = [get_task_validator(t['segmentation_family'])(t) for t in
+                                          alg_info.raw['segmentation_tasks']]
+
+    if not overwrite:
+        validate_output_files_do_not_exist(output_path, alg_info.output_files)
```

### Comparing `vpt-1.0.1/src/vpt/profiler.py` & `vpt-1.0.2/src/vpt/profiler.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-import cProfile
-import marshal
-import pstats
-from pathlib import Path
-from typing import Optional
-
-from vpt import log
-from vpt.filesystem import vzg_open
-
-main_profiler = None
-all_stat = None
-profiler_output = None
-
-
-def initialize_profiler(profile_file: Optional[str]):
-    global main_profiler, profiler_output
-    if profile_file:
-        main_profiler = cProfile.Profile()
-        profiler_output = profile_file
-
-
-def append_stat(statistic_container):
-    global all_stat
-    if all_stat is None:
-        all_stat = pstats.Stats(statistic_container)
-    else:
-        all_stat.add(statistic_container)
-
-
-def enable():
-    if main_profiler:
-        main_profiler.enable()
-
-
-def disable():
-    if main_profiler:
-        main_profiler.disable()
-
-
-def export_data():
-    global all_stat, main_profiler
-    if main_profiler:
-        stats = pstats.Stats(main_profiler)
-        if all_stat:
-            stats.add(all_stat)
-        with vzg_open(profiler_output, 'wb') as f:
-            marshal.dump(stats.stats, f)
-
-
-def append_with_file(fname: str, remove: bool = True):
-    if Path(fname).exists():
-        append_stat(fname)
-        if remove:
-            Path(fname).unlink(missing_ok=True)
-    else:
-        log.warning(f"appending profiling stats failed: {fname} not found")
+import cProfile
+import marshal
+import pstats
+from pathlib import Path
+from typing import Optional
+
+from vpt import log
+from vpt.filesystem import vzg_open
+
+main_profiler = None
+all_stat = None
+profiler_output = None
+
+
+def initialize_profiler(profile_file: Optional[str]):
+    global main_profiler, profiler_output
+    if profile_file:
+        main_profiler = cProfile.Profile()
+        profiler_output = profile_file
+
+
+def append_stat(statistic_container):
+    global all_stat
+    if all_stat is None:
+        all_stat = pstats.Stats(statistic_container)
+    else:
+        all_stat.add(statistic_container)
+
+
+def enable():
+    if main_profiler:
+        main_profiler.enable()
+
+
+def disable():
+    if main_profiler:
+        main_profiler.disable()
+
+
+def export_data():
+    global all_stat, main_profiler
+    if main_profiler:
+        stats = pstats.Stats(main_profiler)
+        if all_stat:
+            stats.add(all_stat)
+        with vzg_open(profiler_output, 'wb') as f:
+            marshal.dump(stats.stats, f)
+
+
+def append_with_file(fname: str, remove: bool = True):
+    if Path(fname).exists():
+        append_stat(fname)
+        if remove:
+            Path(fname).unlink(missing_ok=True)
+    else:
+        log.warning(f"appending profiling stats failed: {fname} not found")
```

### Comparing `vpt-1.0.1/src/vpt/run_segmentation/cmd_args.py` & `vpt-1.0.2/src/vpt/run_segmentation/cmd_args.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,82 +1,82 @@
-from argparse import ArgumentParser
-from dataclasses import dataclass
-
-from vpt.filesystem import filesystem_path_split
-from vpt.prepare_segmentation.constants import OUTPUT_FILE_NAME
-from vpt.utils.output_tools import MIN_ROW_GROUP_SIZE
-from vpt.utils.validate import validate_exists, validate_does_not_exist
-
-# The maximum number of parallel processes that may be launched by run-segmentation
-MAX_PROCESSES = 512
-
-
-@dataclass
-class RunSegmentationArgs:
-    segmentation_algorithm: str
-    input_images: str
-    input_micron_to_mosaic: str
-    tile_size: int
-    tile_overlap: int
-    output_path: str
-    max_row_group_size: int
-    overwrite: bool
-
-
-def validate_args(args: RunSegmentationArgs):
-    validate_exists(args.input_micron_to_mosaic)
-
-    if args.tile_size <= 0:
-        raise ValueError('Tile size should be positive')
-    if args.tile_overlap is not None:
-        if args.tile_overlap < 0 or args.tile_overlap > args.tile_size:
-            raise ValueError('Tile overlap should be in [0, tile-size] range')
-
-    if args.max_row_group_size < MIN_ROW_GROUP_SIZE:
-        raise ValueError(f'Row group size should be at least {MIN_ROW_GROUP_SIZE}')
-
-    if not args.overwrite:
-        fs, path_inside_fs = filesystem_path_split(args.output_path)
-        if fs.exists(path_inside_fs):
-            validate_does_not_exist(args.output_path + '/' + OUTPUT_FILE_NAME)
-
-
-def get_parser() -> ArgumentParser:
-    parser = ArgumentParser(description='Top-level interface for this CLI which invokes the segmentation '
-                            'functionality of the tool. It is intended for users who would like to run '
-                            'the program with minimal additional configuration. Specifically, it executes: '
-                            'prepare-segmentation, run-segmentation-on-tile, and compile-tile-segmentation.',
-                            add_help=False
-                            )
-
-    required = parser.add_argument_group('Required arguments')
-    required.add_argument('--segmentation-algorithm', type=str, required=True,
-                          help='Path to a json file that fully specifies the segmentation algorithm to use, '
-                               'including algorithm name, any algorithm specific parameters '
-                               '(including path to weights for new model), stains corresponding to each channel '
-                               'in the algorithm.')
-    required.add_argument('--input-images', type=str, required=True,
-                          help=r'Regular expression containing path that indicates the images to use '
-                               r'for the segmentation. The regular expressions can indicate the z index '
-                               r'(indicated by (?P<z>[0-9]+)) and/or multiple stains (indicated by (?P<stain>[\w|-]+)). '
-                               r'Here, <stain> must match the stains specified in the segmentation algorithm.')
-    required.add_argument('--input-micron-to-mosaic', type=str, required=True,
-                          help='Path to the micron to mosaic pixel transformation matrix.')
-    required.add_argument('--output-path', type=str, required=True,
-                          help='Directory where the segmentation specification json file '
-                               'will be saved as segmentation_specification.json and where '
-                               'the final segmentation results will be saved.')
-
-    opt = parser.add_argument_group('Optional arguments')
-    opt.add_argument('--tile-size', type=int, default=4096,
-                     help='Number of pixels for the width and height of each tile. '
-                          'Each tile is created as a square. Default: 4096.')
-    opt.add_argument('--tile-overlap', type=int, required=False,
-                     help='Overlap between adjacent tiles. Default: 10%% of tile size.')
-    opt.add_argument('--max-row-group-size', type=int, default=17500, required=False,
-                     help='Maximum number of rows in row groups inside output parquet files. '
-                          f'Cannot be less than {MIN_ROW_GROUP_SIZE}')
-    opt.add_argument('--overwrite', action='store_true', default=False, required=False,
-                     help='Set flag if you want to use non empty directory and agree that files can be over-written.')
-    opt.add_argument("-h", "--help", action="help", help="Show this help message and exit")
-
-    return parser
+from argparse import ArgumentParser
+from dataclasses import dataclass
+
+from vpt.filesystem import filesystem_path_split
+from vpt.prepare_segmentation.constants import OUTPUT_FILE_NAME
+from vpt.utils.output_tools import MIN_ROW_GROUP_SIZE
+from vpt.utils.validate import validate_exists, validate_does_not_exist
+
+# The maximum number of parallel processes that may be launched by run-segmentation
+MAX_PROCESSES = 512
+
+
+@dataclass
+class RunSegmentationArgs:
+    segmentation_algorithm: str
+    input_images: str
+    input_micron_to_mosaic: str
+    tile_size: int
+    tile_overlap: int
+    output_path: str
+    max_row_group_size: int
+    overwrite: bool
+
+
+def validate_args(args: RunSegmentationArgs):
+    validate_exists(args.input_micron_to_mosaic)
+
+    if args.tile_size <= 0:
+        raise ValueError('Tile size should be positive')
+    if args.tile_overlap is not None:
+        if args.tile_overlap < 0 or args.tile_overlap > args.tile_size:
+            raise ValueError('Tile overlap should be in [0, tile-size] range')
+
+    if args.max_row_group_size < MIN_ROW_GROUP_SIZE:
+        raise ValueError(f'Row group size should be at least {MIN_ROW_GROUP_SIZE}')
+
+    if not args.overwrite:
+        fs, path_inside_fs = filesystem_path_split(args.output_path)
+        if fs.exists(path_inside_fs):
+            validate_does_not_exist(args.output_path + '/' + OUTPUT_FILE_NAME)
+
+
+def get_parser() -> ArgumentParser:
+    parser = ArgumentParser(description='Top-level interface for this CLI which invokes the segmentation '
+                            'functionality of the tool. It is intended for users who would like to run '
+                            'the program with minimal additional configuration. Specifically, it executes: '
+                            'prepare-segmentation, run-segmentation-on-tile, and compile-tile-segmentation.',
+                            add_help=False
+                            )
+
+    required = parser.add_argument_group('Required arguments')
+    required.add_argument('--segmentation-algorithm', type=str, required=True,
+                          help='Path to a json file that fully specifies the segmentation algorithm to use, '
+                               'including algorithm name, any algorithm specific parameters '
+                               '(including path to weights for new model), stains corresponding to each channel '
+                               'in the algorithm.')
+    required.add_argument('--input-images', type=str, required=True,
+                          help=r'Regular expression containing path that indicates the images to use '
+                               r'for the segmentation. The regular expressions can indicate the z index '
+                               r'(indicated by (?P<z>[0-9]+)) and/or multiple stains (indicated by (?P<stain>[\w|-]+)). '
+                               r'Here, <stain> must match the stains specified in the segmentation algorithm.')
+    required.add_argument('--input-micron-to-mosaic', type=str, required=True,
+                          help='Path to the micron to mosaic pixel transformation matrix.')
+    required.add_argument('--output-path', type=str, required=True,
+                          help='Directory where the segmentation specification json file '
+                               'will be saved as segmentation_specification.json and where '
+                               'the final segmentation results will be saved.')
+
+    opt = parser.add_argument_group('Optional arguments')
+    opt.add_argument('--tile-size', type=int, default=4096,
+                     help='Number of pixels for the width and height of each tile. '
+                          'Each tile is created as a square. Default: 4096.')
+    opt.add_argument('--tile-overlap', type=int, required=False,
+                     help='Overlap between adjacent tiles. Default: 10%% of tile size.')
+    opt.add_argument('--max-row-group-size', type=int, default=17500, required=False,
+                     help='Maximum number of rows in row groups inside output parquet files. '
+                          f'Cannot be less than {MIN_ROW_GROUP_SIZE}')
+    opt.add_argument('--overwrite', action='store_true', default=False, required=False,
+                     help='Set flag if you want to use non empty directory and agree that files can be over-written.')
+    opt.add_argument("-h", "--help", action="help", help="Show this help message and exit")
+
+    return parser
```

### Comparing `vpt-1.0.1/src/vpt/run_segmentation/main.py` & `vpt-1.0.2/src/vpt/run_segmentation/main.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-import argparse
-import json
-
-import vpt.log as log
-from vpt.app.task import pipeline_to_tasks
-from vpt.app.context import parallel_run
-from vpt.compile_tile_segmentation import run as compile_tile_segmentation
-from vpt.filesystem import vzg_open
-from vpt.prepare_segmentation import run as run_prepare_segmentation
-from vpt.prepare_segmentation.constants import OUTPUT_FILE_NAME
-from vpt.run_segmentation.cmd_args import RunSegmentationArgs, validate_args
-
-
-def run_segmentation(args: argparse.Namespace):
-    def to_prepare_segmentation_args(rsargs: RunSegmentationArgs) -> argparse.Namespace:
-        prep_args = dict(vars(rsargs))
-        prep_args.pop('max_row_group_size')
-        return argparse.Namespace(**prep_args)
-
-    args = RunSegmentationArgs(**vars(args))
-    validate_args(args)
-    log.info('run_segmentation started')
-    run_prepare_segmentation(to_prepare_segmentation_args(args))
-
-    spec_path = '/'.join([args.output_path, OUTPUT_FILE_NAME])
-
-    with vzg_open(spec_path, 'r') as f:
-        spec_json = json.load(f)
-
-    num_tiles = spec_json['window_grid']['num_tiles']
-
-    rot_args = [argparse.Namespace(input_segmentation_parameters=spec_path, tile_index=i, overwrite=args.overwrite)
-                for i in range(num_tiles)]
-
-    parallel_run(pipeline_to_tasks('run-segmentation-on-tile', rot_args))
-
-    compile_args = argparse.Namespace(input_segmentation_parameters=spec_path,
-                                      max_row_group_size=args.max_row_group_size,
-                                      overwrite=args.overwrite)
-
-    compile_tile_segmentation(compile_args)
-
-    log.info('run_segmentation finished')
+import argparse
+import json
+
+import vpt.log as log
+from vpt.app.task import pipeline_to_tasks
+from vpt.app.context import parallel_run
+from vpt.compile_tile_segmentation import run as compile_tile_segmentation
+from vpt.filesystem import vzg_open
+from vpt.prepare_segmentation import run as run_prepare_segmentation
+from vpt.prepare_segmentation.constants import OUTPUT_FILE_NAME
+from vpt.run_segmentation.cmd_args import RunSegmentationArgs, validate_args
+
+
+def run_segmentation(args: argparse.Namespace):
+    def to_prepare_segmentation_args(rsargs: RunSegmentationArgs) -> argparse.Namespace:
+        prep_args = dict(vars(rsargs))
+        prep_args.pop('max_row_group_size')
+        return argparse.Namespace(**prep_args)
+
+    args = RunSegmentationArgs(**vars(args))
+    validate_args(args)
+    log.info('run_segmentation started')
+    run_prepare_segmentation(to_prepare_segmentation_args(args))
+
+    spec_path = '/'.join([args.output_path, OUTPUT_FILE_NAME])
+
+    with vzg_open(spec_path, 'r') as f:
+        spec_json = json.load(f)
+
+    num_tiles = spec_json['window_grid']['num_tiles']
+
+    rot_args = [argparse.Namespace(input_segmentation_parameters=spec_path, tile_index=i, overwrite=args.overwrite)
+                for i in range(num_tiles)]
+
+    parallel_run(pipeline_to_tasks('run-segmentation-on-tile', rot_args))
+
+    compile_args = argparse.Namespace(input_segmentation_parameters=spec_path,
+                                      max_row_group_size=args.max_row_group_size,
+                                      overwrite=args.overwrite)
+
+    compile_tile_segmentation(compile_args)
+
+    log.info('run_segmentation finished')
```

### Comparing `vpt-1.0.1/src/vpt/run_segmentation_on_tile/cmd_args.py` & `vpt-1.0.2/src/vpt/run_segmentation_on_tile/cmd_args.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-from argparse import ArgumentParser
-from dataclasses import dataclass
-from typing import Dict
-
-from vpt.segmentation.utils.seg_result import SegmentationResult
-from vpt.utils.validate import validate_exists
-
-
-@dataclass
-class RunOnTileCmdArgs:
-    input_segmentation_parameters: str
-    tile_index: int
-    overwrite: bool
-
-
-def validate_cmd_args(args: RunOnTileCmdArgs):
-    validate_exists(args.input_segmentation_parameters)
-
-    if args.tile_index < 0:
-        raise ValueError('Tile index should be a positive integer')
-
-    if args.tile_index > SegmentationResult.MAX_TILE_ID:
-        raise ValueError(f'Tile index should be less than {SegmentationResult.MAX_TILE_ID}')
-
-
-def get_parser():
-    parser = ArgumentParser(description='Executes the segmentation algorithm on a specific tile '
-                            'of the mosaic images. This functionality is intended both for visualizing '
-                            'a preview of the segmentation (run only one tile), and for distributing '
-                            'jobs using an orchestration tool such as Nextflow.',
-                            add_help=False
-                            )
-
-    required = parser.add_argument_group('Required arguments')
-    required.add_argument('--input-segmentation-parameters', type=str, required=True,
-                          help='Json file generate by --prepare-segmentation that fully '
-                               'specifies the segmentation to run')
-    required.add_argument('--tile-index', type=int, required=True,
-                          help='Index of the tile to run the segmentation on')
-
-    opt = parser.add_argument_group('Optional arguments')
-    opt.add_argument('--overwrite', action='store_true', default=False, required=False,
-                     help='Set flag if you want to use non empty directory and agree that files can be over-written.')
-    opt.add_argument("-h", "--help", action="help", help="Show this help message and exit")
-
-    return parser
-
-
-def parse_cmd_args() -> Dict:
-    parser = get_parser()
-    namespace = parser.parse_args()
-    return vars(namespace)
+from argparse import ArgumentParser
+from dataclasses import dataclass
+from typing import Dict
+
+from vpt.segmentation.utils.seg_result import SegmentationResult
+from vpt.utils.validate import validate_exists
+
+
+@dataclass
+class RunOnTileCmdArgs:
+    input_segmentation_parameters: str
+    tile_index: int
+    overwrite: bool
+
+
+def validate_cmd_args(args: RunOnTileCmdArgs):
+    validate_exists(args.input_segmentation_parameters)
+
+    if args.tile_index < 0:
+        raise ValueError('Tile index should be a positive integer')
+
+    if args.tile_index > SegmentationResult.MAX_TILE_ID:
+        raise ValueError(f'Tile index should be less than {SegmentationResult.MAX_TILE_ID}')
+
+
+def get_parser():
+    parser = ArgumentParser(description='Executes the segmentation algorithm on a specific tile '
+                            'of the mosaic images. This functionality is intended both for visualizing '
+                            'a preview of the segmentation (run only one tile), and for distributing '
+                            'jobs using an orchestration tool such as Nextflow.',
+                            add_help=False
+                            )
+
+    required = parser.add_argument_group('Required arguments')
+    required.add_argument('--input-segmentation-parameters', type=str, required=True,
+                          help='Json file generate by --prepare-segmentation that fully '
+                               'specifies the segmentation to run')
+    required.add_argument('--tile-index', type=int, required=True,
+                          help='Index of the tile to run the segmentation on')
+
+    opt = parser.add_argument_group('Optional arguments')
+    opt.add_argument('--overwrite', action='store_true', default=False, required=False,
+                     help='Set flag if you want to use non empty directory and agree that files can be over-written.')
+    opt.add_argument("-h", "--help", action="help", help="Show this help message and exit")
+
+    return parser
+
+
+def parse_cmd_args() -> Dict:
+    parser = get_parser()
+    namespace = parser.parse_args()
+    return vars(namespace)
```

### Comparing `vpt-1.0.1/src/vpt/run_segmentation_on_tile/image.py` & `vpt-1.0.2/src/vpt/run_segmentation_on_tile/image.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,75 +1,75 @@
-from typing import Tuple, List, Dict, Set
-
-import numpy as np
-import rasterio
-
-from vpt.filesystem.vzgfs import get_rasterio_environment, rasterio_open
-from vpt.run_segmentation_on_tile.input_utils import ImageInfo
-from vpt.segmentation.filters.factory import create_filter_by_sequence
-from vpt.segmentation.types import SegTask
-
-
-class ImageSet(Dict[str, Dict[int, np.ndarray]]):
-    def z_levels(self) -> Set[int]:
-        return set().union(*self.values())
-
-    def as_list(self, key: str) -> List[np.ndarray]:
-        return list(self.get(key, {}).values())
-
-    def as_stack(self, order: List[str] = None):
-        if not order:
-            return np.array([np.stack([z_stack[z] for z_stack in self.values()], axis=-1) for z in self.z_levels()])
-        return np.array([np.stack([self[k][z] for k in order], axis=-1) for z in self.z_levels()])
-
-
-def read_tile(window: Tuple[int, int, int, int], path: str,
-              num_tries: int = 5) -> np.ndarray:
-    num_retries = num_tries - 1
-
-    for try_number in range(1, num_tries + 1):
-        try:
-            with get_rasterio_environment(path):
-                with rasterio_open(path) as file:
-                    image = file.read(1, window=rasterio.windows.Window(window[0], window[1],
-                                                                        window[2], window[3]))
-        except OSError:
-            if try_number + 1 <= num_tries:
-                print(f'Failed to read {path} at {window}. Retrying {try_number}/{num_retries}.')
-            continue
-        break
-    else:
-        raise IOError(f'Failed to read {path} at {window}')
-
-    return np.squeeze(image)
-
-
-def get_segmentation_images(images_info: List[ImageInfo],
-                            window_info: Tuple[int, int, int]) -> ImageSet:
-    images = ImageSet()
-    for image_info in images_info:
-        if not images.get(image_info.channel):
-            images[image_info.channel] = {}
-        images[image_info.channel][image_info.z_layer] = read_tile(window_info, image_info.full_path)
-    return images
-
-
-def get_prepared_images(task: SegTask, images: ImageSet) -> Tuple[ImageSet, Tuple[int, int]]:
-    cur_images = ImageSet()
-    result_shape, scale = None, (1, 1)
-    for input_info in task.task_input_data:
-        cur_images[input_info.image_channel] = {}
-        image_filter = create_filter_by_sequence(input_info.image_preprocessing)
-        for z, im in images[input_info.image_channel].items():
-            if z not in task.z_layers:
-                continue
-
-            cur_im = image_filter(im)
-            if result_shape is None:
-                result_shape = cur_im.shape[:2]
-                scale = (im.shape[0] / cur_im.shape[0], im.shape[1] / cur_im.shape[1])
-            elif result_shape[:2] != cur_im.shape[:2]:
-                raise ValueError('Invalid preprocessing scale: input images for segmentation after postprocessing '
-                                 'should have same sizes')
-            cur_images[input_info.image_channel][z] = cur_im
-
-    return cur_images, scale
+from typing import Tuple, List, Dict, Set
+
+import numpy as np
+import rasterio
+
+from vpt.filesystem.vzgfs import get_rasterio_environment, rasterio_open
+from vpt.run_segmentation_on_tile.input_utils import ImageInfo
+from vpt.segmentation.filters.factory import create_filter_by_sequence
+from vpt.segmentation.types import SegTask
+
+
+class ImageSet(Dict[str, Dict[int, np.ndarray]]):
+    def z_levels(self) -> Set[int]:
+        return set().union(*self.values())
+
+    def as_list(self, key: str) -> List[np.ndarray]:
+        return list(self.get(key, {}).values())
+
+    def as_stack(self, order: List[str] = None):
+        if not order:
+            return np.array([np.stack([z_stack[z] for z_stack in self.values()], axis=-1) for z in self.z_levels()])
+        return np.array([np.stack([self[k][z] for k in order], axis=-1) for z in self.z_levels()])
+
+
+def read_tile(window: Tuple[int, int, int, int], path: str,
+              num_tries: int = 5) -> np.ndarray:
+    num_retries = num_tries - 1
+
+    for try_number in range(1, num_tries + 1):
+        try:
+            with get_rasterio_environment(path):
+                with rasterio_open(path) as file:
+                    image = file.read(1, window=rasterio.windows.Window(window[0], window[1],
+                                                                        window[2], window[3]))
+        except OSError:
+            if try_number + 1 <= num_tries:
+                print(f'Failed to read {path} at {window}. Retrying {try_number}/{num_retries}.')
+            continue
+        break
+    else:
+        raise IOError(f'Failed to read {path} at {window}')
+
+    return np.squeeze(image)
+
+
+def get_segmentation_images(images_info: List[ImageInfo],
+                            window_info: Tuple[int, int, int]) -> ImageSet:
+    images = ImageSet()
+    for image_info in images_info:
+        if not images.get(image_info.channel):
+            images[image_info.channel] = {}
+        images[image_info.channel][image_info.z_layer] = read_tile(window_info, image_info.full_path)
+    return images
+
+
+def get_prepared_images(task: SegTask, images: ImageSet) -> Tuple[ImageSet, Tuple[int, int]]:
+    cur_images = ImageSet()
+    result_shape, scale = None, (1, 1)
+    for input_info in task.task_input_data:
+        cur_images[input_info.image_channel] = {}
+        image_filter = create_filter_by_sequence(input_info.image_preprocessing)
+        for z, im in images[input_info.image_channel].items():
+            if z not in task.z_layers:
+                continue
+
+            cur_im = image_filter(im)
+            if result_shape is None:
+                result_shape = cur_im.shape[:2]
+                scale = (im.shape[0] / cur_im.shape[0], im.shape[1] / cur_im.shape[1])
+            elif result_shape[:2] != cur_im.shape[:2]:
+                raise ValueError('Invalid preprocessing scale: input images for segmentation after postprocessing '
+                                 'should have same sizes')
+            cur_images[input_info.image_channel][z] = cur_im
+
+    return cur_images, scale
```

### Comparing `vpt-1.0.1/src/vpt/run_segmentation_on_tile/input_utils.py` & `vpt-1.0.2/src/vpt/run_segmentation_on_tile/input_utils.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,134 +1,134 @@
-import json
-import os
-from dataclasses import dataclass
-from typing import Union, List, Dict, Set
-
-from vpt.filesystem import vzg_open, filesystem_path_split
-from vpt.run_segmentation_on_tile.output_utils import make_output_filename
-from vpt.segmentation.filters.description import Header
-from vpt.segmentation.types import SegTask
-from vpt.segmentation.utils.fuse import SegFusion
-from vpt.utils.validate import validate_exists, validate_does_not_exist
-
-
-@dataclass
-class InputData:
-    image_channel: str
-    image_preprocessing: List[Header]
-
-    def __init__(self, image_channel: str, image_preprocessing: List[dict]):
-        self.image_channel = image_channel
-        self.image_preprocessing = [Header(**x) for x in image_preprocessing]
-
-
-@dataclass(frozen=True)
-class SegProp:
-    all_z_indexes: List[int]
-    z_positions_um: List[float]
-
-
-@dataclass(frozen=True)
-class ImageInfo:
-    channel: str
-    z_layer: int
-    full_path: Union[str, os.PathLike]
-
-
-@dataclass(frozen=True)
-class SegSpec:
-    timestamp: float
-    output_paths: Dict[str, str]
-    segmentation_tasks: List[SegTask]
-    segmentation_task_fusion: SegFusion
-    experiment_properties: SegProp
-    image_windows: List[List[int]]
-    micron_to_mosaic_tform: List[List[float]]
-    images: List[ImageInfo]
-
-
-def validate_micron_to_mosaic_tform(matrix: List[List[float]]):
-    if len(matrix) != 3:
-        raise ValueError('Micron to mosaic transform matrix should have 3x3 shape')
-    for row in matrix:
-        if len(row) != 3:
-            raise ValueError('Micron to mosaic transform matrix should have 3x3 shape')
-
-
-def validate_output_path(path: Union[str, os.PathLike], check_empty=True):
-    if check_empty:
-        validate_does_not_exist(path)
-
-
-def validate_task(task_data: SegTask, channels: Set[str], z: Set[int]):
-    if not set(task_data.z_layers).issubset(z):
-        raise ValueError('The segmentation task contains invalid values of the z plane')
-    for image_info in task_data.task_input_data:
-        if image_info.image_channel not in channels:
-            raise ValueError('The segmentation task contains invalid values of the image channel')
-
-
-def validate_seg_spec(seg_spec: SegSpec, tile_index: int, overwrite_files=False):
-    for output_directory in seg_spec.output_paths.values():
-        fs, _ = filesystem_path_split(output_directory)
-        output_file = fs.sep.join([output_directory, make_output_filename(tile_index)])
-        validate_output_path(output_file, not overwrite_files)
-
-    z, channels = set(), set()
-    z_chanel = set()
-    for image_info in seg_spec.images:
-        validate_exists(image_info.full_path)
-        if (image_info.z_layer, image_info.channel) in z_chanel:
-            raise ValueError('Several images are associated with the same z_plane and channel')
-        z_chanel.add((image_info.z_layer, image_info.channel))
-        z.add(image_info.z_layer)
-        channels.add(image_info.channel)
-
-    validate_micron_to_mosaic_tform(seg_spec.micron_to_mosaic_tform)
-    if not set(seg_spec.experiment_properties.all_z_indexes).issuperset(z):
-        raise ValueError('Experiment_properties all_z_indexes does not contain all tasks z_planes')
-    for task in seg_spec.segmentation_tasks:
-        validate_task(task, channels, z)
-
-
-def create_seg_task(**kwargs):
-    data = dict(**kwargs)
-    data['task_input_data'] = [InputData(**input_info) for input_info in kwargs['task_input_data']]
-    data['entity_types_detected'] = data['entity_types_detected'][0]
-    return SegTask(**data)
-
-
-def get_output_directory_dict(output_files: List[Dict]):
-    result = {}
-    for output_info in output_files:
-        for entity_name in output_info['entity_types_output']:
-            result[entity_name] = output_info['files']['run_on_tile_dir']
-    return result
-
-
-def dict_to_segmentation_specification(data: dict) -> SegSpec:
-    output_root = data['input_args']['output_path']
-
-    output_fs, _ = filesystem_path_split(output_root)
-    rel_output_dict = get_output_directory_dict(data['segmentation_algorithm']['output_files'])
-
-    seg_spec_dict = {
-        'timestamp': data['timestamp'],
-        'output_paths': {etype: output_fs.sep.join([output_root, path]) for etype, path in rel_output_dict.items()},
-        'micron_to_mosaic_tform': data['input_data']['micron_to_mosaic_tform'],
-        'images': [ImageInfo(**info) for info in data['input_data']['images']],
-        'image_windows': data['window_grid']['windows'],
-        'segmentation_tasks': [create_seg_task(**task) for task in
-                               data['segmentation_algorithm']['segmentation_tasks']],
-        'segmentation_task_fusion': SegFusion(**data['segmentation_algorithm']['segmentation_task_fusion']),
-        'experiment_properties': SegProp(**data['segmentation_algorithm']['experiment_properties'])
-    }
-    return SegSpec(**seg_spec_dict)
-
-
-def read_seg_spec(json_path: Union[str, os.PathLike], overwrite_files=False) -> SegSpec:
-    with vzg_open(str(json_path), 'r') as f:
-        data = json.load(f)
-    try:
-        return dict_to_segmentation_specification(data)
-    except AttributeError:
-        raise ValueError('Incorrect segmentation specification json')
+import json
+import os
+from dataclasses import dataclass
+from typing import Union, List, Dict, Set
+
+from vpt.filesystem import vzg_open, filesystem_path_split
+from vpt.run_segmentation_on_tile.output_utils import make_output_filename
+from vpt.segmentation.filters.description import Header
+from vpt.segmentation.types import SegTask
+from vpt.segmentation.utils.fuse import SegFusion
+from vpt.utils.validate import validate_exists, validate_does_not_exist
+
+
+@dataclass
+class InputData:
+    image_channel: str
+    image_preprocessing: List[Header]
+
+    def __init__(self, image_channel: str, image_preprocessing: List[dict]):
+        self.image_channel = image_channel
+        self.image_preprocessing = [Header(**x) for x in image_preprocessing]
+
+
+@dataclass(frozen=True)
+class SegProp:
+    all_z_indexes: List[int]
+    z_positions_um: List[float]
+
+
+@dataclass(frozen=True)
+class ImageInfo:
+    channel: str
+    z_layer: int
+    full_path: Union[str, os.PathLike]
+
+
+@dataclass(frozen=True)
+class SegSpec:
+    timestamp: float
+    output_paths: Dict[str, str]
+    segmentation_tasks: List[SegTask]
+    segmentation_task_fusion: SegFusion
+    experiment_properties: SegProp
+    image_windows: List[List[int]]
+    micron_to_mosaic_tform: List[List[float]]
+    images: List[ImageInfo]
+
+
+def validate_micron_to_mosaic_tform(matrix: List[List[float]]):
+    if len(matrix) != 3:
+        raise ValueError('Micron to mosaic transform matrix should have 3x3 shape')
+    for row in matrix:
+        if len(row) != 3:
+            raise ValueError('Micron to mosaic transform matrix should have 3x3 shape')
+
+
+def validate_output_path(path: Union[str, os.PathLike], check_empty=True):
+    if check_empty:
+        validate_does_not_exist(path)
+
+
+def validate_task(task_data: SegTask, channels: Set[str], z: Set[int]):
+    if not set(task_data.z_layers).issubset(z):
+        raise ValueError('The segmentation task contains invalid values of the z plane')
+    for image_info in task_data.task_input_data:
+        if image_info.image_channel not in channels:
+            raise ValueError('The segmentation task contains invalid values of the image channel')
+
+
+def validate_seg_spec(seg_spec: SegSpec, tile_index: int, overwrite_files=False):
+    for output_directory in seg_spec.output_paths.values():
+        fs, _ = filesystem_path_split(output_directory)
+        output_file = fs.sep.join([output_directory, make_output_filename(tile_index)])
+        validate_output_path(output_file, not overwrite_files)
+
+    z, channels = set(), set()
+    z_chanel = set()
+    for image_info in seg_spec.images:
+        validate_exists(image_info.full_path)
+        if (image_info.z_layer, image_info.channel) in z_chanel:
+            raise ValueError('Several images are associated with the same z_plane and channel')
+        z_chanel.add((image_info.z_layer, image_info.channel))
+        z.add(image_info.z_layer)
+        channels.add(image_info.channel)
+
+    validate_micron_to_mosaic_tform(seg_spec.micron_to_mosaic_tform)
+    if not set(seg_spec.experiment_properties.all_z_indexes).issuperset(z):
+        raise ValueError('Experiment_properties all_z_indexes does not contain all tasks z_planes')
+    for task in seg_spec.segmentation_tasks:
+        validate_task(task, channels, z)
+
+
+def create_seg_task(**kwargs):
+    data = dict(**kwargs)
+    data['task_input_data'] = [InputData(**input_info) for input_info in kwargs['task_input_data']]
+    data['entity_types_detected'] = data['entity_types_detected'][0]
+    return SegTask(**data)
+
+
+def get_output_directory_dict(output_files: List[Dict]):
+    result = {}
+    for output_info in output_files:
+        for entity_name in output_info['entity_types_output']:
+            result[entity_name] = output_info['files']['run_on_tile_dir']
+    return result
+
+
+def dict_to_segmentation_specification(data: dict) -> SegSpec:
+    output_root = data['input_args']['output_path']
+
+    output_fs, _ = filesystem_path_split(output_root)
+    rel_output_dict = get_output_directory_dict(data['segmentation_algorithm']['output_files'])
+
+    seg_spec_dict = {
+        'timestamp': data['timestamp'],
+        'output_paths': {etype: output_fs.sep.join([output_root, path]) for etype, path in rel_output_dict.items()},
+        'micron_to_mosaic_tform': data['input_data']['micron_to_mosaic_tform'],
+        'images': [ImageInfo(**info) for info in data['input_data']['images']],
+        'image_windows': data['window_grid']['windows'],
+        'segmentation_tasks': [create_seg_task(**task) for task in
+                               data['segmentation_algorithm']['segmentation_tasks']],
+        'segmentation_task_fusion': SegFusion(**data['segmentation_algorithm']['segmentation_task_fusion']),
+        'experiment_properties': SegProp(**data['segmentation_algorithm']['experiment_properties'])
+    }
+    return SegSpec(**seg_spec_dict)
+
+
+def read_seg_spec(json_path: Union[str, os.PathLike], overwrite_files=False) -> SegSpec:
+    with vzg_open(str(json_path), 'r') as f:
+        data = json.load(f)
+    try:
+        return dict_to_segmentation_specification(data)
+    except AttributeError:
+        raise ValueError('Incorrect segmentation specification json')
```

### Comparing `vpt-1.0.1/src/vpt/run_segmentation_on_tile/main.py` & `vpt-1.0.2/src/vpt/run_segmentation_on_tile/main.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,106 +1,106 @@
-from typing import List
-
-import numpy as np
-from vpt.run_segmentation_on_tile.cmd_args import parse_cmd_args, RunOnTileCmdArgs, validate_cmd_args
-from vpt.run_segmentation_on_tile.image import get_prepared_images, get_segmentation_images
-from vpt.run_segmentation_on_tile.input_utils import read_seg_spec, validate_seg_spec, SegSpec
-from vpt.run_segmentation_on_tile.output_utils import save_to_parquet
-from vpt.segmentation.utils.fuse import fuse_task_polygons
-from vpt.segmentation.factory import run_segmentation
-from vpt.segmentation.utils.polygon_utils import get_upscale_matrix
-from vpt.segmentation.utils.seg_result import SegmentationResult
-import vpt.log as log
-
-
-def add_task_to_entity_id(old_id, task_number) -> int:
-    entity_str_len = len(str(SegmentationResult.MAX_ENTITY_ID))
-    task_str_len = len(str(SegmentationResult.MAX_TASK_ID))
-
-    old_id_str = str(old_id).zfill(entity_str_len)
-    task_str = str(task_number + 1).zfill(task_str_len)
-
-    if len(old_id_str) > entity_str_len or len(task_str) > task_str_len:
-        raise OverflowError('EntityID is out of the int64 type range')
-    return np.int64(''.join([task_str, old_id_str]))
-
-
-def reindex_by_task(tasks_results: List[SegmentationResult], tasks_numbers: List[int]):
-    for task_i in range(len(tasks_results)):
-        tasks_results[task_i].update_column(SegmentationResult.cell_id_field, add_task_to_entity_id,
-                                            task_number=tasks_numbers[task_i])
-    return tasks_results
-
-
-def get_tile_segmentation(
-    seg_spec: SegSpec,
-    window_info: List[int]
-):
-    tasks_result, tasks_numbers = [], []
-    fusion_info = seg_spec.segmentation_task_fusion
-    seg_properties = seg_spec.experiment_properties
-
-    for task in seg_spec.segmentation_tasks:
-        # Perform segmentation, returns a SegmentationResult set of polygons
-        images = get_segmentation_images(seg_spec.images, window_info)
-        images, scale = get_prepared_images(task, images)
-        seg_result = run_segmentation(images, task)
-
-        # Remove images from memory once the geometries are produced
-        del images
-
-        # Process raw geometry into final segmentation output
-        log.info(f"raw segmentation result contains {len(seg_result.df.index)} rows")
-        if task.segmentation_properties['model_dimensions'] == '2D':
-            log.info("fuze across z")
-            seg_result.update_column(SegmentationResult.z_index_field, lambda i: task.z_layers[i])
-            seg_result.fuse_across_z(fusion_info.fused_polygon_postprocessing_parameters)
-            seg_result.replicate_across_z(seg_properties.all_z_indexes)
-
-        seg_result.transform_geoms(get_upscale_matrix(scale[0], scale[1]))
-        log.info("remove edge polys")
-        seg_result.remove_edge_polys((window_info[2],) * 2)
-        seg_result.set_entity_type(task.entity_types_detected)
-
-        if seg_result.df[seg_result.cell_id_field].gt(seg_result.MAX_ENTITY_ID).any():
-            raise OverflowError(f'Tile segmentation could not have more than {seg_result.MAX_ENTITY_ID} entities')
-
-        tasks_result.append(seg_result)
-        tasks_numbers.append(task.task_id)
-
-    tasks_result = reindex_by_task(tasks_result, tasks_numbers)
-
-    return tasks_result
-
-
-def segmentation_on_tile(seg_spec: SegSpec, tile_index: int) -> List[SegmentationResult]:
-    window_info = seg_spec.image_windows[tile_index]
-    log.info(f"Tile {tile_index} {window_info}")
-
-    tasks_result = get_tile_segmentation(seg_spec, window_info)
-
-    fused_result = fuse_task_polygons(tasks_result, seg_spec.segmentation_task_fusion)
-    mosaic_to_micron_matrix = np.linalg.inv(seg_spec.micron_to_mosaic_tform)
-    for i in range(len(fused_result)):
-        fused_result[i].translate_geoms(window_info[0], window_info[1])
-        fused_result[i].transform_geoms(mosaic_to_micron_matrix)
-    return fused_result
-
-
-def run_segmentation_on_tile(parsed_args):
-    args = RunOnTileCmdArgs(**vars(parsed_args))
-    validate_cmd_args(args)
-    log.info(f"Run segmentation on tile {args.tile_index} started")
-
-    seg_spec = read_seg_spec(args.input_segmentation_parameters, args.overwrite)
-    validate_seg_spec(seg_spec, args.tile_index, args.overwrite)
-
-    result = segmentation_on_tile(seg_spec, args.tile_index)
-
-    save_to_parquet(result, args.tile_index, seg_spec.timestamp, seg_spec.experiment_properties.z_positions_um,
-                    seg_spec.output_paths)
-    log.info(f"Run segmentation on tile {args.tile_index} finished")
-
-
-def main():
-    args = parse_cmd_args()
-    run_segmentation_on_tile(args)
+from typing import List
+
+import numpy as np
+from vpt.run_segmentation_on_tile.cmd_args import parse_cmd_args, RunOnTileCmdArgs, validate_cmd_args
+from vpt.run_segmentation_on_tile.image import get_prepared_images, get_segmentation_images
+from vpt.run_segmentation_on_tile.input_utils import read_seg_spec, validate_seg_spec, SegSpec
+from vpt.run_segmentation_on_tile.output_utils import save_to_parquet
+from vpt.segmentation.utils.fuse import fuse_task_polygons
+from vpt.segmentation.factory import run_segmentation
+from vpt.segmentation.utils.polygon_utils import get_upscale_matrix
+from vpt.segmentation.utils.seg_result import SegmentationResult
+import vpt.log as log
+
+
+def add_task_to_entity_id(old_id, task_number) -> int:
+    entity_str_len = len(str(SegmentationResult.MAX_ENTITY_ID))
+    task_str_len = len(str(SegmentationResult.MAX_TASK_ID))
+
+    old_id_str = str(old_id).zfill(entity_str_len)
+    task_str = str(task_number + 1).zfill(task_str_len)
+
+    if len(old_id_str) > entity_str_len or len(task_str) > task_str_len:
+        raise OverflowError('EntityID is out of the int64 type range')
+    return np.int64(''.join([task_str, old_id_str]))
+
+
+def reindex_by_task(tasks_results: List[SegmentationResult], tasks_numbers: List[int]):
+    for task_i in range(len(tasks_results)):
+        tasks_results[task_i].update_column(SegmentationResult.cell_id_field, add_task_to_entity_id,
+                                            task_number=tasks_numbers[task_i])
+    return tasks_results
+
+
+def get_tile_segmentation(
+    seg_spec: SegSpec,
+    window_info: List[int]
+):
+    tasks_result, tasks_numbers = [], []
+    fusion_info = seg_spec.segmentation_task_fusion
+    seg_properties = seg_spec.experiment_properties
+
+    for task in seg_spec.segmentation_tasks:
+        # Perform segmentation, returns a SegmentationResult set of polygons
+        images = get_segmentation_images(seg_spec.images, window_info)
+        images, scale = get_prepared_images(task, images)
+        seg_result = run_segmentation(images, task)
+
+        # Remove images from memory once the geometries are produced
+        del images
+
+        # Process raw geometry into final segmentation output
+        log.info(f"raw segmentation result contains {len(seg_result.df.index)} rows")
+        if task.segmentation_properties['model_dimensions'] == '2D':
+            log.info("fuze across z")
+            seg_result.update_column(SegmentationResult.z_index_field, lambda i: task.z_layers[i])
+            seg_result.fuse_across_z(fusion_info.fused_polygon_postprocessing_parameters)
+            seg_result.replicate_across_z(seg_properties.all_z_indexes)
+
+        seg_result.transform_geoms(get_upscale_matrix(scale[0], scale[1]))
+        log.info("remove edge polys")
+        seg_result.remove_edge_polys((window_info[2],) * 2)
+        seg_result.set_entity_type(task.entity_types_detected)
+
+        if seg_result.df[seg_result.cell_id_field].gt(seg_result.MAX_ENTITY_ID).any():
+            raise OverflowError(f'Tile segmentation could not have more than {seg_result.MAX_ENTITY_ID} entities')
+
+        tasks_result.append(seg_result)
+        tasks_numbers.append(task.task_id)
+
+    tasks_result = reindex_by_task(tasks_result, tasks_numbers)
+
+    return tasks_result
+
+
+def segmentation_on_tile(seg_spec: SegSpec, tile_index: int) -> List[SegmentationResult]:
+    window_info = seg_spec.image_windows[tile_index]
+    log.info(f"Tile {tile_index} {window_info}")
+
+    tasks_result = get_tile_segmentation(seg_spec, window_info)
+
+    fused_result = fuse_task_polygons(tasks_result, seg_spec.segmentation_task_fusion)
+    mosaic_to_micron_matrix = np.linalg.inv(seg_spec.micron_to_mosaic_tform)
+    for i in range(len(fused_result)):
+        fused_result[i].translate_geoms(window_info[0], window_info[1])
+        fused_result[i].transform_geoms(mosaic_to_micron_matrix)
+    return fused_result
+
+
+def run_segmentation_on_tile(parsed_args):
+    args = RunOnTileCmdArgs(**vars(parsed_args))
+    validate_cmd_args(args)
+    log.info(f"Run segmentation on tile {args.tile_index} started")
+
+    seg_spec = read_seg_spec(args.input_segmentation_parameters, args.overwrite)
+    validate_seg_spec(seg_spec, args.tile_index, args.overwrite)
+
+    result = segmentation_on_tile(seg_spec, args.tile_index)
+
+    save_to_parquet(result, args.tile_index, seg_spec.timestamp, seg_spec.experiment_properties.z_positions_um,
+                    seg_spec.output_paths)
+    log.info(f"Run segmentation on tile {args.tile_index} finished")
+
+
+def main():
+    args = parse_cmd_args()
+    run_segmentation_on_tile(args)
```

### Comparing `vpt-1.0.1/src/vpt/run_segmentation_on_tile/output_utils.py` & `vpt-1.0.2/src/vpt/run_segmentation_on_tile/output_utils.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,75 +1,75 @@
-from datetime import datetime
-from typing import List, Dict
-
-import geopandas
-import pandas as pd
-import numpy as np
-
-from vpt.filesystem import vzg_open, filesystem_path_split
-from vpt.segmentation.utils.seg_result import SegmentationResult
-
-
-def make_output_filename(tile_index: int) -> str:
-    return f'{tile_index}.parquet'
-
-
-def get_entity_type_code(entity_type_name: str) -> int:
-    type_codes = {'cell': 100, 'cells': 100, 'nuclei': 200, 'nucleus': 200}
-    code = type_codes.get(entity_type_name)
-    if code is None:
-        # type code for undefined entity type
-        return 300
-    return code
-
-
-def update_entity_id(old_id: int, tile: str, time: str, entity_type: int):
-    err_m = 'Entity id can not be constructed'
-    if old_id > (1e7 - 1) or old_id < 1e5:
-        raise ValueError(f'{err_m}: segmented entity has id = {old_id} with more than 6 digits')
-    if len(time) != 8:
-        raise ValueError(f'{err_m}: timestamp should have 8 digits')
-    if entity_type > 1e5:
-        raise ValueError(f'{err_m}: entity type code could not be greater than {1e5}')
-
-    seconds = int(time[-5:])
-    old_id_fill = len(str(SegmentationResult.MAX_TASK_ID)) + len(str(SegmentationResult.MAX_ENTITY_ID))
-    return np.int64(f'{time[:-5]}{str(seconds + entity_type)}{tile}{str(old_id).zfill(old_id_fill)}')
-
-
-def save_to_parquet(results: List[SegmentationResult], tile_id: int, timestamp: float, z_positions_um: List[float],
-                    output_paths: Dict[str, str]):
-    tile_id_len = len(str(SegmentationResult.MAX_TILE_ID))
-    tile_id_str = str(tile_id).zfill(tile_id_len)
-
-    year_day = str(int(datetime.fromtimestamp(timestamp).strftime('%j')) + 100)
-    day_time = datetime.fromtimestamp(timestamp).strftime('%H%M%S')
-    day_second = str(int(day_time[:2]) * 60 ** 2 + int(day_time[2:4]) * 60 + int(day_time[4:])).zfill(5)
-    timestamp_str = ''.join([year_day, day_second])
-
-    for i in range(len(results)):
-        results[i].set_column(SegmentationResult.entity_name_field, results[i].entity_type)
-        results[i].update_column(SegmentationResult.cell_id_field, update_entity_id, tile=tile_id_str,
-                                 time=timestamp_str, entity_type=get_entity_type_code(results[i].entity_type))
-
-    dataframes = {}
-    set_none = ['Name', 'ParentID', 'ParentType']
-    if z_positions_um is None:
-        set_none.append('ZLevel')
-    else:
-        for i in range(len(results)):
-            results[i].set_z_levels(z_positions_um, 'ZLevel')
-    for entity_type, output_dir in output_paths.items():
-        data = SegmentationResult.combine_segmentations([seg for seg in results if seg.entity_type == entity_type])
-        for column_name in set_none:
-            data.set_column(column_name, None)
-        if not dataframes.get(output_dir):
-            dataframes[output_dir] = []
-        dataframes[output_dir].append(data.df)
-
-    for output_dir, dataframe in dataframes.items():
-        fs, output_dir_inside_fs = filesystem_path_split(output_dir)
-        fs.mkdirs(output_dir_inside_fs, exist_ok=True)
-
-        gdf_compiled = geopandas.GeoDataFrame(pd.concat(dataframe))
-        with vzg_open(f'{output_dir}/{make_output_filename(tile_id)}', 'wb') as f:
-            gdf_compiled.to_parquet(f)
+from datetime import datetime
+from typing import List, Dict
+
+import geopandas
+import pandas as pd
+import numpy as np
+
+from vpt.filesystem import vzg_open, filesystem_path_split
+from vpt.segmentation.utils.seg_result import SegmentationResult
+
+
+def make_output_filename(tile_index: int) -> str:
+    return f'{tile_index}.parquet'
+
+
+def get_entity_type_code(entity_type_name: str) -> int:
+    type_codes = {'cell': 100, 'cells': 100, 'nuclei': 200, 'nucleus': 200}
+    code = type_codes.get(entity_type_name)
+    if code is None:
+        # type code for undefined entity type
+        return 300
+    return code
+
+
+def update_entity_id(old_id: int, tile: str, time: str, entity_type: int):
+    err_m = 'Entity id can not be constructed'
+    if old_id > (1e7 - 1) or old_id < 1e5:
+        raise ValueError(f'{err_m}: segmented entity has id = {old_id} with more than 6 digits')
+    if len(time) != 8:
+        raise ValueError(f'{err_m}: timestamp should have 8 digits')
+    if entity_type > 1e5:
+        raise ValueError(f'{err_m}: entity type code could not be greater than {1e5}')
+
+    seconds = int(time[-5:])
+    old_id_fill = len(str(SegmentationResult.MAX_TASK_ID)) + len(str(SegmentationResult.MAX_ENTITY_ID))
+    return np.int64(f'{time[:-5]}{str(seconds + entity_type)}{tile}{str(old_id).zfill(old_id_fill)}')
+
+
+def save_to_parquet(results: List[SegmentationResult], tile_id: int, timestamp: float, z_positions_um: List[float],
+                    output_paths: Dict[str, str]):
+    tile_id_len = len(str(SegmentationResult.MAX_TILE_ID))
+    tile_id_str = str(tile_id).zfill(tile_id_len)
+
+    year_day = str(int(datetime.fromtimestamp(timestamp).strftime('%j')) + 100)
+    day_time = datetime.fromtimestamp(timestamp).strftime('%H%M%S')
+    day_second = str(int(day_time[:2]) * 60 ** 2 + int(day_time[2:4]) * 60 + int(day_time[4:])).zfill(5)
+    timestamp_str = ''.join([year_day, day_second])
+
+    for i in range(len(results)):
+        results[i].set_column(SegmentationResult.entity_name_field, results[i].entity_type)
+        results[i].update_column(SegmentationResult.cell_id_field, update_entity_id, tile=tile_id_str,
+                                 time=timestamp_str, entity_type=get_entity_type_code(results[i].entity_type))
+
+    dataframes = {}
+    set_none = ['Name', 'ParentID', 'ParentType']
+    if z_positions_um is None:
+        set_none.append('ZLevel')
+    else:
+        for i in range(len(results)):
+            results[i].set_z_levels(z_positions_um, 'ZLevel')
+    for entity_type, output_dir in output_paths.items():
+        data = SegmentationResult.combine_segmentations([seg for seg in results if seg.entity_type == entity_type])
+        for column_name in set_none:
+            data.set_column(column_name, None)
+        if not dataframes.get(output_dir):
+            dataframes[output_dir] = []
+        dataframes[output_dir].append(data.df)
+
+    for output_dir, dataframe in dataframes.items():
+        fs, output_dir_inside_fs = filesystem_path_split(output_dir)
+        fs.mkdirs(output_dir_inside_fs, exist_ok=True)
+
+        gdf_compiled = geopandas.GeoDataFrame(pd.concat(dataframe))
+        with vzg_open(f'{output_dir}/{make_output_filename(tile_id)}', 'wb') as f:
+            gdf_compiled.to_parquet(f)
```

### Comparing `vpt-1.0.1/src/vpt/segmentation/cellpose/segmentation.py` & `vpt-1.0.2/src/vpt/segmentation/cellpose/segmentation.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,81 +1,81 @@
-import warnings
-from dataclasses import dataclass
-from typing import Dict, Optional
-
-import numpy as np
-
-from vpt.run_segmentation_on_tile.image import ImageSet
-from vpt.segmentation.entity import Entity
-from vpt.segmentation.utils.polygon_utils import generate_polygons_from_mask
-from vpt.segmentation.utils.seg_result import SegmentationResult
-
-
-@dataclass(frozen=True)
-class CellposeSegProperties:
-    model: str
-    model_dimensions: str
-    version: str
-    custom_weights: Optional[str] = None
-
-
-@dataclass(frozen=True)
-class CellposeSegParameters:
-    nuclear_channel: str
-    entity_fill_channel: str
-    diameter: int
-    flow_threshold: float
-    mask_threshold: float
-    minimum_mask_size: int
-
-
-def cellpose_polygons_masks(images: ImageSet, segmentation_properties: Dict,
-                            segmentation_parameters: Dict) -> np.ndarray:
-    warnings.filterwarnings('ignore', message='.*the `scipy.ndimage.filters` namespace is deprecated.*')
-    from cellpose import models
-
-    properties = CellposeSegProperties(**segmentation_properties)
-    parameters = CellposeSegParameters(**segmentation_parameters)
-
-    is_valid_channels = parameters.nuclear_channel and parameters.entity_fill_channel
-    image = images.as_stack([parameters.nuclear_channel, parameters.entity_fill_channel]) \
-        if is_valid_channels else images.as_stack()
-
-    empty_z_levels = set()
-    for z_i, z_plane in enumerate(image):
-        for channel_i in range(z_plane.shape[-1]):
-            if z_plane[..., channel_i].std() < 0.1:
-                empty_z_levels.add(z_i)
-    if len(empty_z_levels) == image.shape[0]:
-        return np.zeros((image.shape[0],) + image.shape[1:-1])
-
-    if properties.custom_weights:
-        model = models.CellposeModel(gpu=False, pretrained_model=properties.custom_weights, net_avg=False)
-    else:
-        model = models.Cellpose(gpu=False, model_type=properties.model, net_avg=False)
-
-    to_segment_z = list(set(range(image.shape[0])).difference(empty_z_levels))
-    mask = model.eval(
-        image[to_segment_z, ...],
-        z_axis=0,
-        channel_axis=len(image.shape) - 1,
-        diameter=parameters.diameter,
-        flow_threshold=parameters.flow_threshold,
-        mask_threshold=parameters.mask_threshold,
-        resample=False,
-        min_size=parameters.minimum_mask_size,
-        tile=True,
-        do_3D=(properties.model_dimensions == '3D')
-    )[0]
-    mask = mask.reshape((len(to_segment_z),) + image.shape[1:-1])
-    for i in empty_z_levels:
-        mask = np.insert(mask, i, np.zeros(image.shape[1:-1]), axis=0)
-    return mask
-
-
-def run_segmentation(images: ImageSet, segmentation_properties: Dict, segmentation_parameters: Dict,
-                     polygon_parameters: Dict, result: Entity) -> SegmentationResult:
-
-    masks = cellpose_polygons_masks(images, segmentation_properties, segmentation_parameters)
-    CellposeSegProperties(**segmentation_properties)
-    # todo: different entity
-    return generate_polygons_from_mask(masks, polygon_parameters)
+import warnings
+from dataclasses import dataclass
+from typing import Dict, Optional
+
+import numpy as np
+
+from vpt.run_segmentation_on_tile.image import ImageSet
+from vpt.segmentation.entity import Entity
+from vpt.segmentation.utils.polygon_utils import generate_polygons_from_mask
+from vpt.segmentation.utils.seg_result import SegmentationResult
+
+
+@dataclass(frozen=True)
+class CellposeSegProperties:
+    model: str
+    model_dimensions: str
+    version: str
+    custom_weights: Optional[str] = None
+
+
+@dataclass(frozen=True)
+class CellposeSegParameters:
+    nuclear_channel: str
+    entity_fill_channel: str
+    diameter: int
+    flow_threshold: float
+    mask_threshold: float
+    minimum_mask_size: int
+
+
+def cellpose_polygons_masks(images: ImageSet, segmentation_properties: Dict,
+                            segmentation_parameters: Dict) -> np.ndarray:
+    warnings.filterwarnings('ignore', message='.*the `scipy.ndimage.filters` namespace is deprecated.*')
+    from cellpose import models
+
+    properties = CellposeSegProperties(**segmentation_properties)
+    parameters = CellposeSegParameters(**segmentation_parameters)
+
+    is_valid_channels = parameters.nuclear_channel and parameters.entity_fill_channel
+    image = images.as_stack([parameters.nuclear_channel, parameters.entity_fill_channel]) \
+        if is_valid_channels else images.as_stack()
+
+    empty_z_levels = set()
+    for z_i, z_plane in enumerate(image):
+        for channel_i in range(z_plane.shape[-1]):
+            if z_plane[..., channel_i].std() < 0.1:
+                empty_z_levels.add(z_i)
+    if len(empty_z_levels) == image.shape[0]:
+        return np.zeros((image.shape[0],) + image.shape[1:-1])
+
+    if properties.custom_weights:
+        model = models.CellposeModel(gpu=False, pretrained_model=properties.custom_weights, net_avg=False)
+    else:
+        model = models.Cellpose(gpu=False, model_type=properties.model, net_avg=False)
+
+    to_segment_z = list(set(range(image.shape[0])).difference(empty_z_levels))
+    mask = model.eval(
+        image[to_segment_z, ...],
+        z_axis=0,
+        channel_axis=len(image.shape) - 1,
+        diameter=parameters.diameter,
+        flow_threshold=parameters.flow_threshold,
+        mask_threshold=parameters.mask_threshold,
+        resample=False,
+        min_size=parameters.minimum_mask_size,
+        tile=True,
+        do_3D=(properties.model_dimensions == '3D')
+    )[0]
+    mask = mask.reshape((len(to_segment_z),) + image.shape[1:-1])
+    for i in empty_z_levels:
+        mask = np.insert(mask, i, np.zeros(image.shape[1:-1]), axis=0)
+    return mask
+
+
+def run_segmentation(images: ImageSet, segmentation_properties: Dict, segmentation_parameters: Dict,
+                     polygon_parameters: Dict, result: Entity) -> SegmentationResult:
+
+    masks = cellpose_polygons_masks(images, segmentation_properties, segmentation_parameters)
+    CellposeSegProperties(**segmentation_properties)
+    # todo: different entity
+    return generate_polygons_from_mask(masks, polygon_parameters)
```

### Comparing `vpt-1.0.1/src/vpt/segmentation/cellpose/validate.py` & `vpt-1.0.2/src/vpt/segmentation/cellpose/validate.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from typing import Dict
-
-
-def validate_task(task: Dict) -> Dict:
-    nuclear_channel = task['segmentation_parameters'].get('nuclear_channel', None)
-    fill_channel = task['segmentation_parameters'].get('entity_fill_channel', None)
-
-    channels = [input_data['image_channel'] for input_data in task['task_input_data']]
-
-    if nuclear_channel and nuclear_channel not in channels:
-        raise ValueError(f'{nuclear_channel} is not in input channels')
-
-    if fill_channel and fill_channel not in channels:
-        raise ValueError(f'{fill_channel} is not in input channels')
-
-    return task
+from typing import Dict
+
+
+def validate_task(task: Dict) -> Dict:
+    nuclear_channel = task['segmentation_parameters'].get('nuclear_channel', None)
+    fill_channel = task['segmentation_parameters'].get('entity_fill_channel', None)
+
+    channels = [input_data['image_channel'] for input_data in task['task_input_data']]
+
+    if nuclear_channel and nuclear_channel not in channels:
+        raise ValueError(f'{nuclear_channel} is not in input channels')
+
+    if fill_channel and fill_channel not in channels:
+        raise ValueError(f'{fill_channel} is not in input channels')
+
+    return task
```

### Comparing `vpt-1.0.1/src/vpt/segmentation/factory.py` & `vpt-1.0.2/src/vpt/segmentation/factory.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-from typing import Callable, Dict
-
-from vpt.run_segmentation_on_tile.image import ImageSet
-from vpt.run_segmentation_on_tile.input_utils import SegTask
-
-from vpt.segmentation.entity import parse_entity
-from vpt.segmentation.utils.seg_result import SegmentationResult
-
-
-def empty_validator(x: Dict) -> Dict:
-    return x
-
-
-def get_task_validator(segmentation_family: str) -> Callable[[Dict], Dict]:
-    key = segmentation_family.upper()
-    if key == 'CELLPOSE':
-        from vpt.segmentation.cellpose.validate import validate_task as validate_cellpose_task
-        return validate_cellpose_task
-    if key == 'WATERSHED':
-        from vpt.segmentation.watershed.validate import validate_task as validate_watershed_task
-        return validate_watershed_task
-    return empty_validator
-
-
-def run_segmentation(image: ImageSet, task: SegTask) -> SegmentationResult:
-    key = task.segmentation_family.upper()
-    runner = None
-    if key == 'CELLPOSE':
-        from vpt.segmentation.cellpose.segmentation import run_segmentation as run_cellpose
-        runner = run_cellpose
-    if key == 'WATERSHED':
-        from vpt.segmentation.watershed.segmentation import run_segmentation as run_watershed
-        runner = run_watershed
-
-    return runner(image, task.segmentation_properties, task.segmentation_parameters,
-                  task.polygon_parameters, parse_entity(task.entity_types_detected))
+from typing import Callable, Dict
+
+from vpt.run_segmentation_on_tile.image import ImageSet
+from vpt.run_segmentation_on_tile.input_utils import SegTask
+
+from vpt.segmentation.entity import parse_entity
+from vpt.segmentation.utils.seg_result import SegmentationResult
+
+
+def empty_validator(x: Dict) -> Dict:
+    return x
+
+
+def get_task_validator(segmentation_family: str) -> Callable[[Dict], Dict]:
+    key = segmentation_family.upper()
+    if key == 'CELLPOSE':
+        from vpt.segmentation.cellpose.validate import validate_task as validate_cellpose_task
+        return validate_cellpose_task
+    if key == 'WATERSHED':
+        from vpt.segmentation.watershed.validate import validate_task as validate_watershed_task
+        return validate_watershed_task
+    return empty_validator
+
+
+def run_segmentation(image: ImageSet, task: SegTask) -> SegmentationResult:
+    key = task.segmentation_family.upper()
+    runner = None
+    if key == 'CELLPOSE':
+        from vpt.segmentation.cellpose.segmentation import run_segmentation as run_cellpose
+        runner = run_cellpose
+    if key == 'WATERSHED':
+        from vpt.segmentation.watershed.segmentation import run_segmentation as run_watershed
+        runner = run_watershed
+
+    return runner(image, task.segmentation_properties, task.segmentation_parameters,
+                  task.polygon_parameters, parse_entity(task.entity_types_detected))
```

### Comparing `vpt-1.0.1/src/vpt/segmentation/stardist/seeds.py` & `vpt-1.0.2/src/vpt/segmentation/stardist/seeds.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,101 +1,101 @@
-from typing import Tuple, List
-
-import numpy as np
-import os
-import cv2
-
-from vpt.filesystem import filesystem_path_split
-from vpt.segmentation.entity import Entity
-
-os.environ['TF_CPP_MIN_LOG_LEVEL'] = '3'
-from vpt.segmentation.stardist.star import StarPolygon  # noqa
-from vpt.utils.output_tools import suppress_output  # noqa
-
-
-def normalize(image: np.ndarray, pmin: float, pmax: float):
-    if image[image > 0].size > 0:
-        [mi, ma] = np.percentile(image[image > 0], [pmin, pmax], axis=None)
-        return (image.astype(np.float32) - mi) / (ma - mi + 1e-20)
-    else:
-        return image.astype(np.float32)
-
-
-StardistResult = List[StarPolygon]
-
-
-class StardistSeedsExtractor:
-
-    def __init__(self, model_path: str,
-                 normalization_range: Tuple[float, float] = (1, 99.8),
-                 min_size: int = 16,
-                 max_size: int = 256):
-
-        with suppress_output():
-            from stardist.models import StarDist2D
-
-            fs, path = filesystem_path_split(model_path)
-            assert fs.protocol == 'file'  # Stardist only supports local filesystem
-            path_parts = path.split(fs.sep)
-            parent_path, model_name = fs.sep.join(path_parts[:-1]), path_parts[-1]
-
-            self.model = StarDist2D(None, model_name, parent_path)
-            if not self.model:
-                raise ValueError("Invalid stardist model")
-
-        self.min_size = min_size
-        self.max_size = max_size
-        self.nrm_range = normalization_range
-        self.stars = None
-
-    def run_prediction(self, image) -> StardistResult:
-        normalized_image = normalize(image, self.nrm_range[0], self.nrm_range[1])
-        with suppress_output():
-            n_tiles = None if image.shape[0] < 1024 else (2, 2)
-            _, details = self.model.predict_instances(normalized_image, n_tiles=n_tiles)
-        points, center = details['coord'], details['points']
-        result: List[StarPolygon] = []
-        # filter results
-        for i in range(len(center)):
-            box = [[np.min(points[i][0]), np.max(points[i][0])], [np.min(points[i][1]), np.max(points[i][1])]]
-            h = box[0][1] - box[0][0]
-            w = box[1][1] - box[1][0]
-            if h > image.shape[0] or w > image.shape[1]:
-                # invalid image, return nothing
-                return []
-
-            # filter by bbox size
-            if h > self.min_size and h < self.max_size and w > self.min_size and w < self.max_size:
-                result.append(StarPolygon(center=center[i], points=points[i]))
-
-        return result
-
-    @staticmethod
-    def result_to_mask(shape, results: StardistResult, star_scale: float = 0.6):
-        target = np.zeros(shape, dtype=np.uint8)
-
-        for star in results:
-            triangles = []
-            center = star.center
-            points = star.points
-
-            c = np.array([center[1], center[0]])
-            for j in range(len(points[0]) >> 1):  # half number of points, for speed
-                i1 = j + j
-                i2 = (i1 + 2) % len(points[0])
-                p1 = np.array([points[1][i1], points[0][i1]]) - c
-                p2 = np.array([points[1][i2], points[0][i2]]) - c
-                triangles.append([p1 * star_scale + c, p2 * star_scale + c, c])
-            cv2.fillPoly(target, np.array(triangles, dtype=np.int32), (255, 255, 255))
-        return target != 0
-
-    def extract_seeds(self, seed_images: np.ndarray, entity: Entity) -> Tuple[List[StardistResult], np.ndarray]:
-        vector = [self.run_prediction(x) for x in seed_images]
-        shape = seed_images[0].shape
-        rastr = np.array([StardistSeedsExtractor.result_to_mask(shape, x) for x in vector])
-
-        # If the nuclear polygons are not needed, clear the data
-        # A dummy array is created for logging
-        if entity & Entity.Cells:
-            vector = [[StarPolygon] * len(x) for x in vector]
-
-        return vector, rastr
+from typing import Tuple, List
+
+import numpy as np
+import os
+import cv2
+
+from vpt.filesystem import filesystem_path_split
+from vpt.segmentation.entity import Entity
+
+os.environ['TF_CPP_MIN_LOG_LEVEL'] = '3'
+from vpt.segmentation.stardist.star import StarPolygon  # noqa
+from vpt.utils.output_tools import suppress_output  # noqa
+
+
+def normalize(image: np.ndarray, pmin: float, pmax: float):
+    if image[image > 0].size > 0:
+        [mi, ma] = np.percentile(image[image > 0], [pmin, pmax], axis=None)
+        return (image.astype(np.float32) - mi) / (ma - mi + 1e-20)
+    else:
+        return image.astype(np.float32)
+
+
+StardistResult = List[StarPolygon]
+
+
+class StardistSeedsExtractor:
+
+    def __init__(self, model_path: str,
+                 normalization_range: Tuple[float, float] = (1, 99.8),
+                 min_size: int = 16,
+                 max_size: int = 256):
+
+        with suppress_output():
+            from stardist.models import StarDist2D
+
+            fs, path = filesystem_path_split(model_path)
+            assert fs.protocol == 'file'  # Stardist only supports local filesystem
+            path_parts = path.split(fs.sep)
+            parent_path, model_name = fs.sep.join(path_parts[:-1]), path_parts[-1]
+
+            self.model = StarDist2D(None, model_name, parent_path)
+            if not self.model:
+                raise ValueError("Invalid stardist model")
+
+        self.min_size = min_size
+        self.max_size = max_size
+        self.nrm_range = normalization_range
+        self.stars = None
+
+    def run_prediction(self, image) -> StardistResult:
+        normalized_image = normalize(image, self.nrm_range[0], self.nrm_range[1])
+        with suppress_output():
+            n_tiles = None if image.shape[0] < 1024 else (2, 2)
+            _, details = self.model.predict_instances(normalized_image, n_tiles=n_tiles)
+        points, center = details['coord'], details['points']
+        result: List[StarPolygon] = []
+        # filter results
+        for i in range(len(center)):
+            box = [[np.min(points[i][0]), np.max(points[i][0])], [np.min(points[i][1]), np.max(points[i][1])]]
+            h = box[0][1] - box[0][0]
+            w = box[1][1] - box[1][0]
+            if h > image.shape[0] or w > image.shape[1]:
+                # invalid image, return nothing
+                return []
+
+            # filter by bbox size
+            if h > self.min_size and h < self.max_size and w > self.min_size and w < self.max_size:
+                result.append(StarPolygon(center=center[i], points=points[i]))
+
+        return result
+
+    @staticmethod
+    def result_to_mask(shape, results: StardistResult, star_scale: float = 0.6):
+        target = np.zeros(shape, dtype=np.uint8)
+
+        for star in results:
+            triangles = []
+            center = star.center
+            points = star.points
+
+            c = np.array([center[1], center[0]])
+            for j in range(len(points[0]) >> 1):  # half number of points, for speed
+                i1 = j + j
+                i2 = (i1 + 2) % len(points[0])
+                p1 = np.array([points[1][i1], points[0][i1]]) - c
+                p2 = np.array([points[1][i2], points[0][i2]]) - c
+                triangles.append([p1 * star_scale + c, p2 * star_scale + c, c])
+            cv2.fillPoly(target, np.array(triangles, dtype=np.int32), (255, 255, 255))
+        return target != 0
+
+    def extract_seeds(self, seed_images: np.ndarray, entity: Entity) -> Tuple[List[StardistResult], np.ndarray]:
+        vector = [self.run_prediction(x) for x in seed_images]
+        shape = seed_images[0].shape
+        rastr = np.array([StardistSeedsExtractor.result_to_mask(shape, x) for x in vector])
+
+        # If the nuclear polygons are not needed, clear the data
+        # A dummy array is created for logging
+        if entity & Entity.Cells:
+            vector = [[StarPolygon] * len(x) for x in vector]
+
+        return vector, rastr
```

### Comparing `vpt-1.0.1/src/vpt/segmentation/utils/fuse.py` & `vpt-1.0.2/src/vpt/segmentation/utils/fuse.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,64 +1,64 @@
-from dataclasses import dataclass, field
-from enum import Enum
-from typing import List, Dict
-
-from vpt.segmentation.utils.seg_result import SegmentationResult
-import vpt.log as log
-
-import warnings
-from shapely.errors import ShapelyDeprecationWarning
-
-
-@dataclass(frozen=True)
-class SegFusion:
-    entity_fusion_strategy: str
-    fused_polygon_postprocessing_parameters: Dict = field(default_factory=lambda: {
-        "min_final_area": 0,
-        "min_distance_between_entities": 2})
-
-
-def run_harmonization(segmentations: List[SegmentationResult], min_distance: int, min_area: int):
-    segmentation: SegmentationResult = SegmentationResult.combine_segmentations(segmentations)
-    segmentation.make_non_overlapping_polys(min_distance, min_area)
-    return segmentation
-
-
-def run_union_fusion(segmentations: List[SegmentationResult], min_distance: int, min_area: int):
-    segmentation: SegmentationResult = SegmentationResult.combine_segmentations(segmentations)
-    segmentation.union_intersections(min_distance, min_area)
-    return segmentation
-
-
-def run_larger_fusion(segmentations: List[SegmentationResult], min_distance: int, min_area: int):
-    segmentation: SegmentationResult = SegmentationResult.combine_segmentations(segmentations)
-    segmentation.larger_resolve_intersections(min_distance, min_area)
-    return segmentation
-
-
-class FusionCallbacks(Enum):
-    HARMONIZE = ('harmonize', run_harmonization)
-    LARGER = ('larger', run_larger_fusion)
-    UNION = ('union', run_union_fusion)
-
-
-def fuse_task_polygons(segmentation_results: List[SegmentationResult], fusion_parameters: SegFusion):
-    log.info("fuse_task_polygons")
-    warnings.filterwarnings('ignore', category=ShapelyDeprecationWarning)
-    results = []
-    tasks_entities = [res.entity_type for res in segmentation_results]
-    parameters = fusion_parameters.fused_polygon_postprocessing_parameters
-    strategy_key = fusion_parameters.entity_fusion_strategy.upper()
-    if strategy_key not in FusionCallbacks.__members__:
-        raise Exception("Invalid fusion strategy")
-
-    for entity_type in set(tasks_entities):
-        cur_results = [seg_res for i, seg_res in enumerate(segmentation_results) if tasks_entities[i] == entity_type]
-        if len(cur_results) <= 1:
-            results.append(cur_results[0])
-            continue
-        seg_result = FusionCallbacks[strategy_key].value[1](cur_results, parameters['min_distance_between_entities'],
-                                                            parameters['min_final_area'])
-        seg_result.set_entity_type(entity_type)
-        results.append(seg_result)
-
-    return results
+from dataclasses import dataclass, field
+from enum import Enum
+from typing import List, Dict
+
+from vpt.segmentation.utils.seg_result import SegmentationResult
+import vpt.log as log
+
+import warnings
+from shapely.errors import ShapelyDeprecationWarning
+
+
+@dataclass(frozen=True)
+class SegFusion:
+    entity_fusion_strategy: str
+    fused_polygon_postprocessing_parameters: Dict = field(default_factory=lambda: {
+        "min_final_area": 0,
+        "min_distance_between_entities": 2})
+
+
+def run_harmonization(segmentations: List[SegmentationResult], min_distance: int, min_area: int):
+    segmentation: SegmentationResult = SegmentationResult.combine_segmentations(segmentations)
+    segmentation.make_non_overlapping_polys(min_distance, min_area)
+    return segmentation
+
+
+def run_union_fusion(segmentations: List[SegmentationResult], min_distance: int, min_area: int):
+    segmentation: SegmentationResult = SegmentationResult.combine_segmentations(segmentations)
+    segmentation.union_intersections(min_distance, min_area)
+    return segmentation
+
+
+def run_larger_fusion(segmentations: List[SegmentationResult], min_distance: int, min_area: int):
+    segmentation: SegmentationResult = SegmentationResult.combine_segmentations(segmentations)
+    segmentation.larger_resolve_intersections(min_distance, min_area)
+    return segmentation
+
+
+class FusionCallbacks(Enum):
+    HARMONIZE = ('harmonize', run_harmonization)
+    LARGER = ('larger', run_larger_fusion)
+    UNION = ('union', run_union_fusion)
+
+
+def fuse_task_polygons(segmentation_results: List[SegmentationResult], fusion_parameters: SegFusion):
+    log.info("fuse_task_polygons")
+    warnings.filterwarnings('ignore', category=ShapelyDeprecationWarning)
+    results = []
+    tasks_entities = [res.entity_type for res in segmentation_results]
+    parameters = fusion_parameters.fused_polygon_postprocessing_parameters
+    strategy_key = fusion_parameters.entity_fusion_strategy.upper()
+    if strategy_key not in FusionCallbacks.__members__:
+        raise Exception("Invalid fusion strategy")
+
+    for entity_type in set(tasks_entities):
+        cur_results = [seg_res for i, seg_res in enumerate(segmentation_results) if tasks_entities[i] == entity_type]
+        if len(cur_results) <= 1:
+            results.append(cur_results[0])
+            continue
+        seg_result = FusionCallbacks[strategy_key].value[1](cur_results, parameters['min_distance_between_entities'],
+                                                            parameters['min_final_area'])
+        seg_result.set_entity_type(entity_type)
+        results.append(seg_result)
+
+    return results
```

### Comparing `vpt-1.0.1/src/vpt/segmentation/utils/polygon_utils.py` & `vpt-1.0.2/src/vpt/segmentation/utils/polygon_utils.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,138 +1,138 @@
-from dataclasses import dataclass
-from typing import Dict
-
-import cv2
-import numpy as np
-from shapely import geometry
-from shapely.validation import make_valid
-import vpt.log as log
-from vpt.segmentation.utils.seg_result import SegmentationResult
-
-
-@dataclass(frozen=True)
-class PolygonCreationParameters:
-    simplification_tol: int
-    smoothing_radius: int
-    minimum_final_area: int
-
-
-def generate_polygons_from_mask(mask: np.ndarray, polygon_parameters: Dict) -> SegmentationResult:
-    log.info("generate_polygons_from_mask")
-    parameters = PolygonCreationParameters(**polygon_parameters)
-    seg_result = get_polygons_from_mask(mask, parameters.smoothing_radius, parameters.simplification_tol)
-    seg_result.remove_polys(lambda poly: poly.area < parameters.minimum_final_area)
-    return seg_result
-
-
-def make_polygons_from_label_matrix(entity_id, label_matrix):
-    '''
-    Creates a list of Polygon objects from a label matrix
-    '''
-    contours, _ = cv2.findContours((label_matrix == entity_id).astype("uint8"), cv2.RETR_LIST, cv2.CHAIN_APPROX_SIMPLE)
-    polys = []
-    for c in contours:
-        if c.shape[0] < 4:
-            continue
-
-        # Create a valid polygon object
-        p = geometry.Polygon(c[:, 0, :]).buffer(0)
-        p = largest_geometry(p)
-        if p.is_empty:
-            continue
-        polys.append(p)
-
-    return polys
-
-
-def get_polygons_from_mask(mask: np.ndarray, smoothing_radius, simplification_tolerance) -> SegmentationResult:
-    '''
-    Accepts either a 2D or 3D numpy array label matrix, returns a SegmentationResult of
-    MultiPolygons surrounding each label/mask. Performs smoothing and simplification of
-    Polygons before returning.
-    '''
-
-    # If passed 2D data, expand axes so that z-level indexing will work
-    if len(mask.shape) == 2:
-        mask = np.expand_dims(mask, axis=0)
-
-    polys_data = []
-    for z in range(mask.shape[0]):
-        list_of_mask_ids = np.unique(mask[z, :, :])
-        log.info(f"get_polygons_from_mask: z={z}, labels:{len(list_of_mask_ids)}")
-        for idx, mask_id in enumerate(list_of_mask_ids):
-            # Value of zero is background, skip
-            if mask_id == 0:
-                continue
-
-            try:
-                # Convert each region of the entity into a polygon
-                raw_polys = make_polygons_from_label_matrix(mask_id, mask[z, :, :])
-
-                polys = [smooth_and_simplify(raw_poly, smoothing_radius, simplification_tolerance) for raw_poly in raw_polys]
-                polys = [poly for poly in polys if not poly.is_empty]
-
-                # If smoothing and simplifying eliminated all polygons, don't add them to the output
-                if len(polys) == 0:
-                    continue
-
-                # Transform the list of 1 or more mask polygons into a multipolygon
-                multi_poly = convert_to_multipoly(make_valid(geometry.MultiPolygon(polys)))
-                polys_data.append(
-                    {
-                        SegmentationResult.detection_id_field: idx + 1,
-                        SegmentationResult.cell_id_field: mask_id,
-                        SegmentationResult.z_index_field: z,
-                        SegmentationResult.geometry_field: multi_poly
-                    }
-                )
-            except ValueError:
-                # If the MultiPolygon is not created properly, it is probably because the
-                # geometry is low quality or otherwise strange. In that situation, it's ok
-                # to discard the geometry by catching the exception and not appending the
-                # geometry to the output.
-                log.info(f"Mask id {mask_id} could not be converted to a polygon.")
-
-    return SegmentationResult(list_data=polys_data)
-
-
-def get_upscale_matrix(scale_x: int, scale_y: int) -> np.ndarray:
-    return np.array([[scale_x, 0, 0], [0, scale_y, 0], [0, 0, 1]])
-
-
-def smooth_and_simplify(poly, radius, tol):
-    if isinstance(poly, geometry.MultiPolygon):
-        buffered_shapes = (p.buffer(-radius).buffer(radius * 2).buffer(-radius) for p in poly.geoms)
-        buffered_multipolygons = (p if type(p) is geometry.MultiPolygon else geometry.MultiPolygon([p]) for p in
-                                  buffered_shapes)
-        buffered_polygons = (p for mp in buffered_multipolygons for p in mp.geoms)
-        poly = geometry.MultiPolygon(buffered_polygons)
-    elif isinstance(poly, geometry.Polygon):
-        poly = poly.buffer(-radius).buffer(radius * 2).buffer(-radius)
-    return largest_geometry(poly.simplify(tolerance=tol))
-
-
-def largest_geometry(shape):
-    '''
-    If passed a Polygon, returns the Polygon.
-    If passed a MultiPolygon, returns the largest Polygon region.
-    Else throws TypeError
-    '''
-    if type(shape) is geometry.Polygon:
-        return shape
-    elif type(shape) is geometry.MultiPolygon:
-        sizes = np.array([(idx, g.area) for idx, g in enumerate(shape.geoms)])
-        idx_largest = sizes[sizes[:, 1].argmax(), 0]
-        return shape.geoms[int(idx_largest)]
-    else:
-        raise TypeError(f"Objects of type {type(shape)} are not supported")
-
-
-def convert_to_multipoly(shape):
-    if type(shape) is geometry.Polygon:
-        return geometry.multipolygon.MultiPolygon([shape])
-    elif type(shape) is geometry.MultiPolygon:
-        return shape
-    else:
-        # If type is not Polygon or Multipolygon, the shape
-        # is strange / small and should be rejected
-        return geometry.MultiPolygon()
+from dataclasses import dataclass
+from typing import Dict
+
+import cv2
+import numpy as np
+from shapely import geometry
+from shapely.validation import make_valid
+import vpt.log as log
+from vpt.segmentation.utils.seg_result import SegmentationResult
+
+
+@dataclass(frozen=True)
+class PolygonCreationParameters:
+    simplification_tol: int
+    smoothing_radius: int
+    minimum_final_area: int
+
+
+def generate_polygons_from_mask(mask: np.ndarray, polygon_parameters: Dict) -> SegmentationResult:
+    log.info("generate_polygons_from_mask")
+    parameters = PolygonCreationParameters(**polygon_parameters)
+    seg_result = get_polygons_from_mask(mask, parameters.smoothing_radius, parameters.simplification_tol)
+    seg_result.remove_polys(lambda poly: poly.area < parameters.minimum_final_area)
+    return seg_result
+
+
+def make_polygons_from_label_matrix(entity_id, label_matrix):
+    '''
+    Creates a list of Polygon objects from a label matrix
+    '''
+    contours, _ = cv2.findContours((label_matrix == entity_id).astype("uint8"), cv2.RETR_LIST, cv2.CHAIN_APPROX_SIMPLE)
+    polys = []
+    for c in contours:
+        if c.shape[0] < 4:
+            continue
+
+        # Create a valid polygon object
+        p = geometry.Polygon(c[:, 0, :]).buffer(0)
+        p = largest_geometry(p)
+        if p.is_empty:
+            continue
+        polys.append(p)
+
+    return polys
+
+
+def get_polygons_from_mask(mask: np.ndarray, smoothing_radius, simplification_tolerance) -> SegmentationResult:
+    '''
+    Accepts either a 2D or 3D numpy array label matrix, returns a SegmentationResult of
+    MultiPolygons surrounding each label/mask. Performs smoothing and simplification of
+    Polygons before returning.
+    '''
+
+    # If passed 2D data, expand axes so that z-level indexing will work
+    if len(mask.shape) == 2:
+        mask = np.expand_dims(mask, axis=0)
+
+    polys_data = []
+    for z in range(mask.shape[0]):
+        list_of_mask_ids = np.unique(mask[z, :, :])
+        log.info(f"get_polygons_from_mask: z={z}, labels:{len(list_of_mask_ids)}")
+        for idx, mask_id in enumerate(list_of_mask_ids):
+            # Value of zero is background, skip
+            if mask_id == 0:
+                continue
+
+            try:
+                # Convert each region of the entity into a polygon
+                raw_polys = make_polygons_from_label_matrix(mask_id, mask[z, :, :])
+
+                polys = [smooth_and_simplify(raw_poly, smoothing_radius, simplification_tolerance) for raw_poly in raw_polys]
+                polys = [poly for poly in polys if not poly.is_empty]
+
+                # If smoothing and simplifying eliminated all polygons, don't add them to the output
+                if len(polys) == 0:
+                    continue
+
+                # Transform the list of 1 or more mask polygons into a multipolygon
+                multi_poly = convert_to_multipoly(make_valid(geometry.MultiPolygon(polys)))
+                polys_data.append(
+                    {
+                        SegmentationResult.detection_id_field: idx + 1,
+                        SegmentationResult.cell_id_field: mask_id,
+                        SegmentationResult.z_index_field: z,
+                        SegmentationResult.geometry_field: multi_poly
+                    }
+                )
+            except ValueError:
+                # If the MultiPolygon is not created properly, it is probably because the
+                # geometry is low quality or otherwise strange. In that situation, it's ok
+                # to discard the geometry by catching the exception and not appending the
+                # geometry to the output.
+                log.info(f"Mask id {mask_id} could not be converted to a polygon.")
+
+    return SegmentationResult(list_data=polys_data)
+
+
+def get_upscale_matrix(scale_x: int, scale_y: int) -> np.ndarray:
+    return np.array([[scale_x, 0, 0], [0, scale_y, 0], [0, 0, 1]])
+
+
+def smooth_and_simplify(poly, radius, tol):
+    if isinstance(poly, geometry.MultiPolygon):
+        buffered_shapes = (p.buffer(-radius).buffer(radius * 2).buffer(-radius) for p in poly.geoms)
+        buffered_multipolygons = (p if type(p) is geometry.MultiPolygon else geometry.MultiPolygon([p]) for p in
+                                  buffered_shapes)
+        buffered_polygons = (p for mp in buffered_multipolygons for p in mp.geoms)
+        poly = geometry.MultiPolygon(buffered_polygons)
+    elif isinstance(poly, geometry.Polygon):
+        poly = poly.buffer(-radius).buffer(radius * 2).buffer(-radius)
+    return largest_geometry(poly.simplify(tolerance=tol))
+
+
+def largest_geometry(shape):
+    '''
+    If passed a Polygon, returns the Polygon.
+    If passed a MultiPolygon, returns the largest Polygon region.
+    Else throws TypeError
+    '''
+    if type(shape) is geometry.Polygon:
+        return shape
+    elif type(shape) is geometry.MultiPolygon:
+        sizes = np.array([(idx, g.area) for idx, g in enumerate(shape.geoms)])
+        idx_largest = sizes[sizes[:, 1].argmax(), 0]
+        return shape.geoms[int(idx_largest)]
+    else:
+        raise TypeError(f"Objects of type {type(shape)} are not supported")
+
+
+def convert_to_multipoly(shape):
+    if type(shape) is geometry.Polygon:
+        return geometry.multipolygon.MultiPolygon([shape])
+    elif type(shape) is geometry.MultiPolygon:
+        return shape
+    else:
+        # If type is not Polygon or Multipolygon, the shape
+        # is strange / small and should be rejected
+        return geometry.MultiPolygon()
```

### Comparing `vpt-1.0.1/src/vpt/segmentation/watershed/seeds.py` & `vpt-1.0.2/src/vpt/segmentation/watershed/seeds.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,103 +1,103 @@
-from typing import Tuple
-
-import numpy as np
-from pyclustering.cluster import kmedoids
-from scipy import ndimage
-from skimage import filters
-from skimage import morphology, measure
-
-"""
-This module contains utility functions for preparing images for
-watershed segmentation.
-"""
-
-
-def separate_merged_seeds(seedsIn: np.ndarray, morph_r: int = 20) -> np.ndarray:
-    """Separate seeds that are merged in 3 dimensions but are separated
-    in some 2 dimensional slices.
-
-    Args:
-        seedsIn: a 3 dimensional binary numpy array arranged as (z,x,y) where
-            True indicates the pixel corresponds with a seed.
-    Returns: a 3 dimensional binary numpy array of the same size as seedsIn
-        indicating the positions of seeds after processing.
-    """
-
-    def create_region_image(shape, c):
-        region = np.zeros(shape, dtype=np.uint8)
-        for x in c.coords:
-            region[x[0], x[1], x[2]] = 1
-        return region
-
-    diskStruct = morphology.disk(morph_r)
-
-    components = measure.regionprops(measure.label(seedsIn))
-    seeds = np.zeros(seedsIn.shape, dtype=np.uint8)
-    for c in components:
-        seedImage = create_region_image(seeds.shape, c)
-        localProps = [measure.regionprops(measure.label(x)) for x in seedImage]
-        seedCounts = [len(x) for x in localProps]
-
-        if all([x < 2 for x in seedCounts]):
-            goodFrames = [i for i, x in enumerate(seedCounts) if x == 1]
-            goodProperties = [y for x in goodFrames for y in localProps[x]]
-            seedPositions = np.round([np.median(
-                [x.centroid for x in goodProperties], axis=0)]).astype(int)
-        else:
-            goodFrames = [i for i, x in enumerate(seedCounts) if x > 1]
-            goodProperties = [y for x in goodFrames for y in localProps[x]]
-            goodCentroids = [x.centroid for x in goodProperties]
-            km = kmedoids.kmedoids(
-                goodCentroids,
-                np.random.choice(np.arange(len(goodCentroids)),
-                                 size=np.max(seedCounts)))
-            km.process()
-            seedPositions = np.round(
-                [goodCentroids[x] for x in km.get_medoids()]).astype(int)
-
-        for s in seedPositions:
-            for f in goodFrames:
-                seeds[f, s[0], s[1]] = 1
-
-    seeds = ndimage.binary_dilation(
-        seeds, structure=ndimage.generate_binary_structure(3, 1))
-    seeds = np.array([ndimage.binary_dilation(
-        x, structure=diskStruct) for x in seeds])
-
-    return seeds
-
-
-def prepare_watershed_images(watershedImageStack: np.ndarray
-                             ) -> Tuple[np.ndarray, np.ndarray]:
-    """Prepare the given images as the input image for watershedding.
-
-    A watershed mask is determined using an adaptive threshold and the watershed
-    images are inverted so the largest values in the watershed images become
-    minima and then the image stack is normalized to have values between 0
-    and 1.
-
-    Args:
-        watershedImageStack: a 3 dimensional numpy array containing the images
-            arranged as (z, x, y).
-    Returns: a tuple containing the normalized watershed images and the
-        calculated watershed mask
-    """
-    filterSize = int(2 * np.floor(watershedImageStack.shape[1] / 16) + 1)
-
-    watershedMask = np.array(
-        [
-            ndimage.binary_fill_holes(x > filters.threshold_local(x, filterSize, method='mean', mode='wrap'))
-            for x in watershedImageStack
-        ]
-    )
-
-    img_min, img_max = np.min(watershedImageStack), np.max(watershedImageStack)
-
-    if img_max > img_min:
-        normalizedWatershed = 1 - (watershedImageStack - img_min) / (img_max - img_min)
-    else:
-        normalizedWatershed = 1 - watershedImageStack
-
-    normalizedWatershed[np.invert(watershedMask)] = 1
-
-    return normalizedWatershed, watershedMask
+from typing import Tuple
+
+import numpy as np
+from pyclustering.cluster import kmedoids
+from scipy import ndimage
+from skimage import filters
+from skimage import morphology, measure
+
+"""
+This module contains utility functions for preparing images for
+watershed segmentation.
+"""
+
+
+def separate_merged_seeds(seedsIn: np.ndarray, morph_r: int = 20) -> np.ndarray:
+    """Separate seeds that are merged in 3 dimensions but are separated
+    in some 2 dimensional slices.
+
+    Args:
+        seedsIn: a 3 dimensional binary numpy array arranged as (z,x,y) where
+            True indicates the pixel corresponds with a seed.
+    Returns: a 3 dimensional binary numpy array of the same size as seedsIn
+        indicating the positions of seeds after processing.
+    """
+
+    def create_region_image(shape, c):
+        region = np.zeros(shape, dtype=np.uint8)
+        for x in c.coords:
+            region[x[0], x[1], x[2]] = 1
+        return region
+
+    diskStruct = morphology.disk(morph_r)
+
+    components = measure.regionprops(measure.label(seedsIn))
+    seeds = np.zeros(seedsIn.shape, dtype=np.uint8)
+    for c in components:
+        seedImage = create_region_image(seeds.shape, c)
+        localProps = [measure.regionprops(measure.label(x)) for x in seedImage]
+        seedCounts = [len(x) for x in localProps]
+
+        if all([x < 2 for x in seedCounts]):
+            goodFrames = [i for i, x in enumerate(seedCounts) if x == 1]
+            goodProperties = [y for x in goodFrames for y in localProps[x]]
+            seedPositions = np.round([np.median(
+                [x.centroid for x in goodProperties], axis=0)]).astype(int)
+        else:
+            goodFrames = [i for i, x in enumerate(seedCounts) if x > 1]
+            goodProperties = [y for x in goodFrames for y in localProps[x]]
+            goodCentroids = [x.centroid for x in goodProperties]
+            km = kmedoids.kmedoids(
+                goodCentroids,
+                np.random.choice(np.arange(len(goodCentroids)),
+                                 size=np.max(seedCounts)))
+            km.process()
+            seedPositions = np.round(
+                [goodCentroids[x] for x in km.get_medoids()]).astype(int)
+
+        for s in seedPositions:
+            for f in goodFrames:
+                seeds[f, s[0], s[1]] = 1
+
+    seeds = ndimage.binary_dilation(
+        seeds, structure=ndimage.generate_binary_structure(3, 1))
+    seeds = np.array([ndimage.binary_dilation(
+        x, structure=diskStruct) for x in seeds])
+
+    return seeds
+
+
+def prepare_watershed_images(watershedImageStack: np.ndarray
+                             ) -> Tuple[np.ndarray, np.ndarray]:
+    """Prepare the given images as the input image for watershedding.
+
+    A watershed mask is determined using an adaptive threshold and the watershed
+    images are inverted so the largest values in the watershed images become
+    minima and then the image stack is normalized to have values between 0
+    and 1.
+
+    Args:
+        watershedImageStack: a 3 dimensional numpy array containing the images
+            arranged as (z, x, y).
+    Returns: a tuple containing the normalized watershed images and the
+        calculated watershed mask
+    """
+    filterSize = int(2 * np.floor(watershedImageStack.shape[1] / 16) + 1)
+
+    watershedMask = np.array(
+        [
+            ndimage.binary_fill_holes(x > filters.threshold_local(x, filterSize, method='mean', mode='wrap'))
+            for x in watershedImageStack
+        ]
+    )
+
+    img_min, img_max = np.min(watershedImageStack), np.max(watershedImageStack)
+
+    if img_max > img_min:
+        normalizedWatershed = 1 - (watershedImageStack - img_min) / (img_max - img_min)
+    else:
+        normalizedWatershed = 1 - watershedImageStack
+
+    normalizedWatershed[np.invert(watershedMask)] = 1
+
+    return normalizedWatershed, watershedMask
```

### Comparing `vpt-1.0.1/src/vpt/segmentation/watershed/segmentation.py` & `vpt-1.0.2/src/vpt/segmentation/watershed/segmentation.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,140 +1,140 @@
-from typing import Dict, List, Tuple
-
-import numpy as np
-from shapely.geometry import Polygon, MultiPolygon
-from skimage import measure
-from skimage.segmentation import watershed
-
-from vpt.run_segmentation_on_tile.image import ImageSet
-from vpt.segmentation.entity import Entity
-from vpt.segmentation.stardist.seeds import StardistSeedsExtractor, StardistResult
-from vpt.segmentation.utils.polygon_utils import generate_polygons_from_mask, smooth_and_simplify, \
-    PolygonCreationParameters
-from vpt.segmentation.utils.seg_result import SegmentationResult
-from vpt.segmentation.watershed import key_stardist_model, key_seed_channel, key_entity_fill_channel
-from vpt.segmentation.watershed.seeds import prepare_watershed_images, separate_merged_seeds
-import vpt.log as log
-
-import warnings
-
-
-def to_sd_extractor_params(params: Dict) -> Dict:
-    return {
-        'normalization_range': params.get('normalization_range', (1, 99.8)),
-        'min_size': params.get('min_diameter', 16),
-        'max_size': params.get('max_diameter', 256)
-    }
-
-
-def get_watershed_seeds(
-    images: ImageSet,
-    segmentation_parameters: Dict,
-    entity: Entity
-):
-    # Load the seed image
-    seeds = np.array(images.as_list(segmentation_parameters.get(key_seed_channel, "")))
-    if seeds.size == 0:
-        raise AttributeError(
-            f'{key_seed_channel} and {key_entity_fill_channel} must be specified in segmentation_parameters')
-
-    log.info("stardist initialization")
-    extractor = StardistSeedsExtractor(
-        segmentation_parameters[key_stardist_model],
-        **to_sd_extractor_params(segmentation_parameters)
-    )
-
-    log.info("extracting seeds")
-    nuclei, seeds = extractor.extract_seeds(seeds, entity)
-    log.info(f"detected seeds on each level: {str(',').join((str(len(x)) for x in nuclei))}")
-
-    log.info("separate_merged_seeds")
-    morph_r = segmentation_parameters.get('morphology_r', 20)
-    seeds = separate_merged_seeds(seeds, morph_r)
-    seeds = measure.label(seeds)
-
-    return nuclei, seeds
-
-
-def run_watershed(
-        images: ImageSet,
-        segmentation_parameters: Dict,
-        entity: Entity) -> Tuple[List[StardistResult], np.ndarray]:
-    warnings.filterwarnings('ignore', message='.*deprecated and will be removed in Pillow 10.*')  # shapely
-    warnings.filterwarnings('ignore', message='.*the `scipy.ndimage.morphology` namespace is deprecated.*')
-    warnings.filterwarnings('ignore', message='.*the `scipy.ndimage.measurements` namespace is deprecated.*')
-
-    # Use the nuclear channel to derive the seeds for watershed
-    nuclei, seeds = get_watershed_seeds(images, segmentation_parameters, entity)
-
-    # If exporting nuceli, return early with the nuclear output
-    if entity & Entity.Nucleus:
-        result = np.zeros(seeds.shape, dtype=np.uint8)
-        return nuclei, result
-
-    # Load the cyto images
-    cyto_images = np.array(images.as_list(segmentation_parameters.get(key_entity_fill_channel, "")))
-
-    if key_entity_fill_channel in segmentation_parameters and cyto_images.size == 0:
-        raise ValueError('Unable to find images in task data for the specified fill channel')
-
-    # If no cyto images, return early with an empty result
-    if cyto_images.size == 0:
-        result = np.zeros(seeds.shape, dtype=np.uint8)
-        return nuclei, result
-
-    # Preprocess cyto channel to dmap and mask images
-    log.info("prepare_watershed_images")
-    dmap, watershed_mask = prepare_watershed_images(cyto_images)
-    seeds[np.invert(watershed_mask)] = 0
-
-    # Run 3D watershed
-    log.info("watershed")
-    result = watershed(
-        dmap,
-        seeds,
-        mask=watershed_mask,
-        connectivity=np.ones((3, 3, 3)),
-        watershed_line=True
-    )
-
-    log.info("watershed finished")
-
-    return nuclei, result
-
-
-def polygons_from_stardist(sd_results: List[StardistResult], polygon_parameters: Dict) -> SegmentationResult:
-    polys_data = []
-    for z in range(len(sd_results)):
-        for idx, star in enumerate(sd_results[z]):
-            p = Polygon(np.fliplr(np.swapaxes(star.points, 0, 1)))
-            polys_data.append(
-                {
-                    SegmentationResult.detection_id_field: idx + 1,
-                    SegmentationResult.cell_id_field: idx,
-                    SegmentationResult.z_index_field: z,
-                    SegmentationResult.geometry_field: MultiPolygon([p])
-                }
-            )
-
-    seg_result = SegmentationResult(list_data=polys_data)
-    parameters = PolygonCreationParameters(**polygon_parameters)
-    seg_result.update_geometry(smooth_and_simplify, radius=parameters.smoothing_radius,
-                               tol=parameters.simplification_tol)
-    seg_result.remove_polys(lambda poly: poly.area < parameters.minimum_final_area)
-    return seg_result
-
-
-# todo: return multiple results, 1 for each entity
-def run_segmentation(images: ImageSet, segmentation_properties: Dict,
-                     segmentation_parameters: Dict, polygon_parameters: Dict,
-                     entity: Entity) -> SegmentationResult:
-
-    if entity & Entity.Nucleus:
-        nucleus, _ = run_watershed(images, segmentation_parameters, entity)
-        return polygons_from_stardist(nucleus, polygon_parameters)
-
-    if entity & Entity.Cells:
-        _, cells = run_watershed(images, segmentation_parameters, entity)
-        return generate_polygons_from_mask(cells, polygon_parameters)
-
-    return SegmentationResult()
+from typing import Dict, List, Tuple
+
+import numpy as np
+from shapely.geometry import Polygon, MultiPolygon
+from skimage import measure
+from skimage.segmentation import watershed
+
+from vpt.run_segmentation_on_tile.image import ImageSet
+from vpt.segmentation.entity import Entity
+from vpt.segmentation.stardist.seeds import StardistSeedsExtractor, StardistResult
+from vpt.segmentation.utils.polygon_utils import generate_polygons_from_mask, smooth_and_simplify, \
+    PolygonCreationParameters
+from vpt.segmentation.utils.seg_result import SegmentationResult
+from vpt.segmentation.watershed import key_stardist_model, key_seed_channel, key_entity_fill_channel
+from vpt.segmentation.watershed.seeds import prepare_watershed_images, separate_merged_seeds
+import vpt.log as log
+
+import warnings
+
+
+def to_sd_extractor_params(params: Dict) -> Dict:
+    return {
+        'normalization_range': params.get('normalization_range', (1, 99.8)),
+        'min_size': params.get('min_diameter', 16),
+        'max_size': params.get('max_diameter', 256)
+    }
+
+
+def get_watershed_seeds(
+    images: ImageSet,
+    segmentation_parameters: Dict,
+    entity: Entity
+):
+    # Load the seed image
+    seeds = np.array(images.as_list(segmentation_parameters.get(key_seed_channel, "")))
+    if seeds.size == 0:
+        raise AttributeError(
+            f'{key_seed_channel} and {key_entity_fill_channel} must be specified in segmentation_parameters')
+
+    log.info("stardist initialization")
+    extractor = StardistSeedsExtractor(
+        segmentation_parameters[key_stardist_model],
+        **to_sd_extractor_params(segmentation_parameters)
+    )
+
+    log.info("extracting seeds")
+    nuclei, seeds = extractor.extract_seeds(seeds, entity)
+    log.info(f"detected seeds on each level: {str(',').join((str(len(x)) for x in nuclei))}")
+
+    log.info("separate_merged_seeds")
+    morph_r = segmentation_parameters.get('morphology_r', 20)
+    seeds = separate_merged_seeds(seeds, morph_r)
+    seeds = measure.label(seeds)
+
+    return nuclei, seeds
+
+
+def run_watershed(
+        images: ImageSet,
+        segmentation_parameters: Dict,
+        entity: Entity) -> Tuple[List[StardistResult], np.ndarray]:
+    warnings.filterwarnings('ignore', message='.*deprecated and will be removed in Pillow 10.*')  # shapely
+    warnings.filterwarnings('ignore', message='.*the `scipy.ndimage.morphology` namespace is deprecated.*')
+    warnings.filterwarnings('ignore', message='.*the `scipy.ndimage.measurements` namespace is deprecated.*')
+
+    # Use the nuclear channel to derive the seeds for watershed
+    nuclei, seeds = get_watershed_seeds(images, segmentation_parameters, entity)
+
+    # If exporting nuceli, return early with the nuclear output
+    if entity & Entity.Nucleus:
+        result = np.zeros(seeds.shape, dtype=np.uint8)
+        return nuclei, result
+
+    # Load the cyto images
+    cyto_images = np.array(images.as_list(segmentation_parameters.get(key_entity_fill_channel, "")))
+
+    if key_entity_fill_channel in segmentation_parameters and cyto_images.size == 0:
+        raise ValueError('Unable to find images in task data for the specified fill channel')
+
+    # If no cyto images, return early with an empty result
+    if cyto_images.size == 0:
+        result = np.zeros(seeds.shape, dtype=np.uint8)
+        return nuclei, result
+
+    # Preprocess cyto channel to dmap and mask images
+    log.info("prepare_watershed_images")
+    dmap, watershed_mask = prepare_watershed_images(cyto_images)
+    seeds[np.invert(watershed_mask)] = 0
+
+    # Run 3D watershed
+    log.info("watershed")
+    result = watershed(
+        dmap,
+        seeds,
+        mask=watershed_mask,
+        connectivity=np.ones((3, 3, 3)),
+        watershed_line=True
+    )
+
+    log.info("watershed finished")
+
+    return nuclei, result
+
+
+def polygons_from_stardist(sd_results: List[StardistResult], polygon_parameters: Dict) -> SegmentationResult:
+    polys_data = []
+    for z in range(len(sd_results)):
+        for idx, star in enumerate(sd_results[z]):
+            p = Polygon(np.fliplr(np.swapaxes(star.points, 0, 1)))
+            polys_data.append(
+                {
+                    SegmentationResult.detection_id_field: idx + 1,
+                    SegmentationResult.cell_id_field: idx,
+                    SegmentationResult.z_index_field: z,
+                    SegmentationResult.geometry_field: MultiPolygon([p])
+                }
+            )
+
+    seg_result = SegmentationResult(list_data=polys_data)
+    parameters = PolygonCreationParameters(**polygon_parameters)
+    seg_result.update_geometry(smooth_and_simplify, radius=parameters.smoothing_radius,
+                               tol=parameters.simplification_tol)
+    seg_result.remove_polys(lambda poly: poly.area < parameters.minimum_final_area)
+    return seg_result
+
+
+# todo: return multiple results, 1 for each entity
+def run_segmentation(images: ImageSet, segmentation_properties: Dict,
+                     segmentation_parameters: Dict, polygon_parameters: Dict,
+                     entity: Entity) -> SegmentationResult:
+
+    if entity & Entity.Nucleus:
+        nucleus, _ = run_watershed(images, segmentation_parameters, entity)
+        return polygons_from_stardist(nucleus, polygon_parameters)
+
+    if entity & Entity.Cells:
+        _, cells = run_watershed(images, segmentation_parameters, entity)
+        return generate_polygons_from_mask(cells, polygon_parameters)
+
+    return SegmentationResult()
```

### Comparing `vpt-1.0.1/src/vpt/sum_signals/cmd_args.py` & `vpt-1.0.2/src/vpt/sum_signals/cmd_args.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-from argparse import ArgumentParser
-from dataclasses import dataclass
-
-from vpt.utils.validate import validate_exists, validate_does_not_exist
-
-# The maximum number of parallel processes that may be launched by sum-signals
-MAX_PROCESSES = 512
-
-
-@dataclass
-class SumSignalsArgs:
-    input_images: str
-    input_boundaries: str
-    input_micron_to_mosaic: str
-    output_csv: str
-    overwrite: bool
-
-
-def validate_args(args: SumSignalsArgs):
-    validate_exists(args.input_boundaries)
-    validate_exists(args.input_micron_to_mosaic)
-
-    if not args.overwrite:
-        validate_does_not_exist(args.output_csv)
-
-
-def get_parser() -> ArgumentParser:
-    parser = ArgumentParser(description='Uses the segmentation boundaries to find the intensity of each '
-                            'mosaic image in each Entity. Outputs both the summed intensity of the raw '
-                            'images and the summed intensity of high-pass filtered images (reduces the '
-                            'effect of background fluorescence).',
-                            add_help=False
-                            )
-
-    required = parser.add_argument_group('Required arguments')
-    required.add_argument('--input-images', type=str, required=True,
-                          help=r'Path to images containing regular expressions to indicate the z index (indicated '
-                               r'by (?P<z>[0-9]+)) and/or multiple stains (indicated by (?P<stain>[\w|-]+)). '
-                               r'If only a subset of the mosaic tiffs should be quantified, modify the regular '
-                               r'expression accordingly. For example, "mosaic_(?P<stain>DAPI)_z(?P<z>[0-9]+)).tif" '
-                               r'would match only DAPI images.')
-    required.add_argument('--input-boundaries', type=str, required=True,
-                          help='Path to a micron-space .parquet boundary file.')
-    required.add_argument('--input-micron-to-mosaic', type=str, required=True,
-                          help='Path to the micron to mosaic pixel transformation matrix.')
-    required.add_argument('--output-csv', type=str, required=True,
-                          help='Path to the csv file where the sum intensities will be stored.')
-
-    opt = parser.add_argument_group('Optional arguments')
-    opt.add_argument('--overwrite', action='store_true', default=False, required=False,
-                     help='Set true if you want to use non empty directory and agree that files can be overwritten.')
-    opt.add_argument("-h", "--help", action="help", help="Show this help message and exit")
-
-    return parser
-
-
-def parse_args():
-    return get_parser().parse_args()
+from argparse import ArgumentParser
+from dataclasses import dataclass
+
+from vpt.utils.validate import validate_exists, validate_does_not_exist
+
+# The maximum number of parallel processes that may be launched by sum-signals
+MAX_PROCESSES = 512
+
+
+@dataclass
+class SumSignalsArgs:
+    input_images: str
+    input_boundaries: str
+    input_micron_to_mosaic: str
+    output_csv: str
+    overwrite: bool
+
+
+def validate_args(args: SumSignalsArgs):
+    validate_exists(args.input_boundaries)
+    validate_exists(args.input_micron_to_mosaic)
+
+    if not args.overwrite:
+        validate_does_not_exist(args.output_csv)
+
+
+def get_parser() -> ArgumentParser:
+    parser = ArgumentParser(description='Uses the segmentation boundaries to find the intensity of each '
+                            'mosaic image in each Entity. Outputs both the summed intensity of the raw '
+                            'images and the summed intensity of high-pass filtered images (reduces the '
+                            'effect of background fluorescence).',
+                            add_help=False
+                            )
+
+    required = parser.add_argument_group('Required arguments')
+    required.add_argument('--input-images', type=str, required=True,
+                          help=r'Path to images containing regular expressions to indicate the z index (indicated '
+                               r'by (?P<z>[0-9]+)) and/or multiple stains (indicated by (?P<stain>[\w|-]+)). '
+                               r'If only a subset of the mosaic tiffs should be quantified, modify the regular '
+                               r'expression accordingly. For example, "mosaic_(?P<stain>DAPI)_z(?P<z>[0-9]+)).tif" '
+                               r'would match only DAPI images.')
+    required.add_argument('--input-boundaries', type=str, required=True,
+                          help='Path to a micron-space .parquet boundary file.')
+    required.add_argument('--input-micron-to-mosaic', type=str, required=True,
+                          help='Path to the micron to mosaic pixel transformation matrix.')
+    required.add_argument('--output-csv', type=str, required=True,
+                          help='Path to the csv file where the sum intensities will be stored.')
+
+    opt = parser.add_argument_group('Optional arguments')
+    opt.add_argument('--overwrite', action='store_true', default=False, required=False,
+                     help='Set true if you want to use non empty directory and agree that files can be overwritten.')
+    opt.add_argument("-h", "--help", action="help", help="Show this help message and exit")
+
+    return parser
+
+
+def parse_args():
+    return get_parser().parse_args()
```

### Comparing `vpt-1.0.1/src/vpt/sum_signals/main.py` & `vpt-1.0.2/src/vpt/sum_signals/main.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,166 +1,166 @@
-import argparse
-from collections import defaultdict
-from typing import Iterable, Tuple
-
-import numpy as np
-import pandas as pd
-import rasterio
-from rasterio.features import rasterize
-from scipy import ndimage
-from shapely.affinity import translate, affine_transform
-from shapely.geometry.base import BaseGeometry
-
-import vpt.log as log
-from vpt.app.task import Task
-from vpt.app.context import parallel_run, current_context
-from vpt.filesystem.vzgfs import get_rasterio_environment, filesystem_path_split, vzg_open, initialize_filesystem, \
-    rasterio_open
-from vpt.log import show_progress
-from vpt.sum_signals.cmd_args import parse_args, SumSignalsArgs, validate_args
-from vpt.sum_signals.validate import validate_z_layers_number
-from vpt.utils.input_utils import read_micron_to_mosaic_transform, read_geodataframe
-from vpt.utils.regex_tools import parse_regex
-
-
-def get_cell_brightness_in_image(
-        image_path: str,
-        entities: Iterable[Tuple[int, BaseGeometry]]) -> tuple:
-    cell_raw_brightness = []
-    cell_filtered_brightness = []
-    indexes = []
-
-    with get_rasterio_environment(image_path):
-        with rasterio_open(image_path) as file:
-            for cell_id, cell in entities:
-                if cell is None or cell.is_empty:
-                    continue
-
-                # Define an image area to read
-                rasterio_window = [
-                    cell.bounds[0],
-                    cell.bounds[1],
-                    cell.bounds[2] - cell.bounds[0] + 1,
-                    cell.bounds[3] - cell.bounds[1] + 1
-                ]
-
-                # Read the image area and convert to 2D numpy array
-                rasterio_window = [int(x) for x in rasterio_window]
-                image_data = file.read(1, window=rasterio.windows.Window(*rasterio_window))
-
-                high_pass_input = image_data
-                cell_fft = np.fft.fft2(high_pass_input)
-                filtered_fft = ndimage.fourier_uniform(cell_fft, size=10)
-                inverse_filtered_fft = np.fft.ifft2(filtered_fft)
-                high_pass_image = high_pass_input - inverse_filtered_fft.real
-                high_pass_image = np.maximum(high_pass_image, 0)
-
-                # Create a polygon at the origin to use to mask an image
-                selector_poly = translate(cell, xoff=-cell.bounds[0], yoff=-cell.bounds[1])
-
-                # Create the mask
-                bounding_box = [int(x) for x in selector_poly.bounds]
-                if (min(bounding_box[:2]) < 0 or
-                        bounding_box[2] >= image_data.shape[1] or
-                        bounding_box[3] >= image_data.shape[0]):
-                    raise ValueError(f'Cell is beyond image boundaries: {cell}')
-
-                mask_shape = (bounding_box[3] + 1, bounding_box[2] + 1)
-                cell_mask = rasterize([selector_poly], out_shape=mask_shape, all_touched=True)
-
-                # Add the signal from this z-plane to the overall brightness
-                cell_raw_brightness.append(np.sum(image_data * cell_mask))
-                cell_filtered_brightness.append(np.sum(high_pass_image * cell_mask))
-                indexes.append(cell_id)
-
-    return (pd.Series(cell_raw_brightness, index=indexes),
-            pd.Series(cell_filtered_brightness, index=indexes))
-
-
-def calculate(args):
-    img, fn_boundaries, transform = args.img, args.boundaries, args.transform
-    log.info(f"sum_signals.calculate for {img.full_path} started")
-    boundaries = read_geodataframe(fn_boundaries)
-    idx = boundaries['ZIndex'] == img.z_layer
-
-    def iterator() -> Iterable[Tuple[int, BaseGeometry]]:
-        for _, row in boundaries.loc[idx].iterrows():
-            entity_id = row['EntityID']
-            geom = row['Geometry']
-            yield (entity_id, affine_transform(geom, transform))
-
-    res = get_cell_brightness_in_image(img.full_path, iterator())
-    return img.channel, res
-
-
-def validate_and_prepare_ids(images, fn_boundary):
-    boundaries = read_geodataframe(fn_boundary)
-    validate_z_layers_number(images, boundaries)
-    return boundaries['EntityID'].unique()
-
-
-def get_cell_brightnesses(images, fn_boundary, transform):
-    ids = validate_and_prepare_ids(images, fn_boundary)
-
-    def default_value():
-        return pd.Series(np.zeros(len(ids)), index=ids)
-
-    results_raw, results_high_pass = defaultdict(default_value), defaultdict(default_value)
-    log.info("output structures prepared")
-    results = parallel_run(
-        [Task(calculate, argparse.Namespace(img=img, boundaries=fn_boundary, transform=transform)) for img in images])
-
-    def combine_results(jobs, progress=False):
-        if progress:
-            jobs = show_progress(jobs, total=len(results))
-        log.info("all jobs finished")
-        for channel, (intensities_raw, intensities_high_pass) in jobs:
-            results_raw[channel][intensities_raw.index] += intensities_raw
-            results_high_pass[channel][intensities_high_pass.index] += intensities_high_pass
-
-    ctx = current_context()
-    combine_results(results, progress=ctx is None or ctx.get_workers_count() == 1)
-    log.info("results combined")
-
-    assert set(results_raw.keys()) == set(results_high_pass.keys())
-
-    sum_signals_data = {}
-    for stain in results_raw.keys():
-        sum_signals_data[f"{stain}_raw"] = results_raw[stain]
-        sum_signals_data[f"{stain}_high_pass"] = results_high_pass[stain]
-
-    df = pd.DataFrame(sum_signals_data)
-    df.sort_index(inplace=True)
-
-    return df
-
-
-def save_df(df, path: str):
-    fs, fs_path = filesystem_path_split(path)
-    try:
-        parent, _ = fs_path.rsplit(fs.sep, maxsplit=1)  # raises ValueError if the path only contains a filename
-        fs.mkdirs(parent, exist_ok=True)
-    except ValueError:
-        pass
-
-    with vzg_open(path, 'w') as f:
-        df.to_csv(f)
-
-
-def sum_signals(args: argparse.Namespace):
-    args = SumSignalsArgs(**vars(args))
-    validate_args(args)
-    log.info("Sum signals started")
-    regex_info = parse_regex(args.input_images)
-
-    m2m = np.array(read_micron_to_mosaic_transform(args.input_micron_to_mosaic))
-    tform_flat = [*m2m[:2, :2].flatten(), *m2m[:2, 2].flatten()]
-
-    df = get_cell_brightnesses(regex_info.images, args.input_boundaries, tform_flat)
-
-    save_df(df, args.output_csv)
-    log.info("Sum signals finished")
-
-
-if __name__ == '__main__':
-    initialize_filesystem()
-    sum_signals(parse_args())
+import argparse
+from collections import defaultdict
+from typing import Iterable, Tuple
+
+import numpy as np
+import pandas as pd
+import rasterio
+from rasterio.features import rasterize
+from scipy import ndimage
+from shapely.affinity import translate, affine_transform
+from shapely.geometry.base import BaseGeometry
+
+import vpt.log as log
+from vpt.app.task import Task
+from vpt.app.context import parallel_run, current_context
+from vpt.filesystem.vzgfs import get_rasterio_environment, filesystem_path_split, vzg_open, initialize_filesystem, \
+    rasterio_open
+from vpt.log import show_progress
+from vpt.sum_signals.cmd_args import parse_args, SumSignalsArgs, validate_args
+from vpt.sum_signals.validate import validate_z_layers_number
+from vpt.utils.input_utils import read_micron_to_mosaic_transform, read_geodataframe
+from vpt.utils.regex_tools import parse_regex
+
+
+def get_cell_brightness_in_image(
+        image_path: str,
+        entities: Iterable[Tuple[int, BaseGeometry]]) -> tuple:
+    cell_raw_brightness = []
+    cell_filtered_brightness = []
+    indexes = []
+
+    with get_rasterio_environment(image_path):
+        with rasterio_open(image_path) as file:
+            for cell_id, cell in entities:
+                if cell is None or cell.is_empty:
+                    continue
+
+                # Define an image area to read
+                rasterio_window = [
+                    cell.bounds[0],
+                    cell.bounds[1],
+                    cell.bounds[2] - cell.bounds[0] + 1,
+                    cell.bounds[3] - cell.bounds[1] + 1
+                ]
+
+                # Read the image area and convert to 2D numpy array
+                rasterio_window = [int(x) for x in rasterio_window]
+                image_data = file.read(1, window=rasterio.windows.Window(*rasterio_window))
+
+                high_pass_input = image_data
+                cell_fft = np.fft.fft2(high_pass_input)
+                filtered_fft = ndimage.fourier_uniform(cell_fft, size=10)
+                inverse_filtered_fft = np.fft.ifft2(filtered_fft)
+                high_pass_image = high_pass_input - inverse_filtered_fft.real
+                high_pass_image = np.maximum(high_pass_image, 0)
+
+                # Create a polygon at the origin to use to mask an image
+                selector_poly = translate(cell, xoff=-cell.bounds[0], yoff=-cell.bounds[1])
+
+                # Create the mask
+                bounding_box = [int(x) for x in selector_poly.bounds]
+                if (min(bounding_box[:2]) < 0 or
+                        bounding_box[2] >= image_data.shape[1] or
+                        bounding_box[3] >= image_data.shape[0]):
+                    raise ValueError(f'Cell is beyond image boundaries: {cell}')
+
+                mask_shape = (bounding_box[3] + 1, bounding_box[2] + 1)
+                cell_mask = rasterize([selector_poly], out_shape=mask_shape, all_touched=True)
+
+                # Add the signal from this z-plane to the overall brightness
+                cell_raw_brightness.append(np.sum(image_data * cell_mask))
+                cell_filtered_brightness.append(np.sum(high_pass_image * cell_mask))
+                indexes.append(cell_id)
+
+    return (pd.Series(cell_raw_brightness, index=indexes),
+            pd.Series(cell_filtered_brightness, index=indexes))
+
+
+def calculate(args):
+    img, fn_boundaries, transform = args.img, args.boundaries, args.transform
+    log.info(f"sum_signals.calculate for {img.full_path} started")
+    boundaries = read_geodataframe(fn_boundaries)
+    idx = boundaries['ZIndex'] == img.z_layer
+
+    def iterator() -> Iterable[Tuple[int, BaseGeometry]]:
+        for _, row in boundaries.loc[idx].iterrows():
+            entity_id = row['EntityID']
+            geom = row['Geometry']
+            yield (entity_id, affine_transform(geom, transform))
+
+    res = get_cell_brightness_in_image(img.full_path, iterator())
+    return img.channel, res
+
+
+def validate_and_prepare_ids(images, fn_boundary):
+    boundaries = read_geodataframe(fn_boundary)
+    validate_z_layers_number(images, boundaries)
+    return boundaries['EntityID'].unique()
+
+
+def get_cell_brightnesses(images, fn_boundary, transform):
+    ids = validate_and_prepare_ids(images, fn_boundary)
+
+    def default_value():
+        return pd.Series(np.zeros(len(ids)), index=ids)
+
+    results_raw, results_high_pass = defaultdict(default_value), defaultdict(default_value)
+    log.info("output structures prepared")
+    results = parallel_run(
+        [Task(calculate, argparse.Namespace(img=img, boundaries=fn_boundary, transform=transform)) for img in images])
+
+    def combine_results(jobs, progress=False):
+        if progress:
+            jobs = show_progress(jobs, total=len(results))
+        log.info("all jobs finished")
+        for channel, (intensities_raw, intensities_high_pass) in jobs:
+            results_raw[channel][intensities_raw.index] += intensities_raw
+            results_high_pass[channel][intensities_high_pass.index] += intensities_high_pass
+
+    ctx = current_context()
+    combine_results(results, progress=ctx is None or ctx.get_workers_count() == 1)
+    log.info("results combined")
+
+    assert set(results_raw.keys()) == set(results_high_pass.keys())
+
+    sum_signals_data = {}
+    for stain in results_raw.keys():
+        sum_signals_data[f"{stain}_raw"] = results_raw[stain]
+        sum_signals_data[f"{stain}_high_pass"] = results_high_pass[stain]
+
+    df = pd.DataFrame(sum_signals_data)
+    df.sort_index(inplace=True)
+
+    return df
+
+
+def save_df(df, path: str):
+    fs, fs_path = filesystem_path_split(path)
+    try:
+        parent, _ = fs_path.rsplit(fs.sep, maxsplit=1)  # raises ValueError if the path only contains a filename
+        fs.mkdirs(parent, exist_ok=True)
+    except ValueError:
+        pass
+
+    with vzg_open(path, 'w') as f:
+        df.to_csv(f)
+
+
+def sum_signals(args: argparse.Namespace):
+    args = SumSignalsArgs(**vars(args))
+    validate_args(args)
+    log.info("Sum signals started")
+    regex_info = parse_regex(args.input_images)
+
+    m2m = np.array(read_micron_to_mosaic_transform(args.input_micron_to_mosaic))
+    tform_flat = [*m2m[:2, :2].flatten(), *m2m[:2, 2].flatten()]
+
+    df = get_cell_brightnesses(regex_info.images, args.input_boundaries, tform_flat)
+
+    save_df(df, args.output_csv)
+    log.info("Sum signals finished")
+
+
+if __name__ == '__main__':
+    initialize_filesystem()
+    sum_signals(parse_args())
```

### Comparing `vpt-1.0.1/src/vpt/update_vzg/assemble/cell_coloring.py` & `vpt-1.0.2/src/vpt/update_vzg/assemble/cell_coloring.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,88 +1,88 @@
-from copy import deepcopy
-from typing import List
-import numpy as np
-
-from vpt.update_vzg.assemble.expression_matrix import GeneExprMatrix, ExpressionMetric
-
-
-def create_bytearray(array_l, array_type=np.float32) -> bytearray:
-    output_btr = bytearray()
-    for element in array_l:
-        output_btr.extend(array_type(element))
-
-    return output_btr
-
-
-class CellColoring:
-    def __init__(self, matrix: GeneExprMatrix):
-        self._matrix = matrix
-        self._normalized_matrix = None
-        self._cellsMetricsList: List = []
-
-        self._metricExtr = []
-        for i in range(ExpressionMetric.ItemsCount.value):
-            self._cellsMetricsList.append(np.zeros(matrix.lines_cells, np.float32))
-            self._metricExtr.append(np.zeros(2, np.float32))
-            self._metricExtr[i][0] = float('inf')
-            self._metricExtr[i][1] = float('-inf')
-
-        self._outputNameBtrDict: dict = {}
-
-    def _make_cell_lists(self):
-        data = self._matrix.data
-        sigma_genes = []
-        for genes_column in self._matrix.data.T:
-            sigma_genes.append(np.std(genes_column))
-
-        self._metricExtr[ExpressionMetric.Count.value][0] = data.min()
-        self._metricExtr[ExpressionMetric.Count.value][1] = data.max()
-
-        for i, row_transcripts in enumerate(data):
-            self._cellsMetricsList[ExpressionMetric.Count.value][i] = np.sum(row_transcripts)
-
-        self._normalized_matrix: GeneExprMatrix = deepcopy(self._matrix)
-        self._normalized_matrix.change_matrix_data_from_origin(ExpressionMetric.Normalized)
-        normalized_data = self._normalized_matrix.data
-        normalized_sigma_genes = []
-
-        self._metricExtr[ExpressionMetric.Normalized.value][0] = normalized_data.min()
-        self._metricExtr[ExpressionMetric.Normalized.value][1] = normalized_data.max()
-
-        for genes_column in self._normalized_matrix.data.T:
-            normalized_sigma_genes.append(np.std(genes_column))
-
-        for i, row_transcripts in enumerate(normalized_data):
-            self._cellsMetricsList[ExpressionMetric.Normalized.value][i] = np.sum(row_transcripts)
-
-        self._outputNameBtrDict: dict = {
-            'genes_mean': create_bytearray(self._matrix.average_genes),
-            'genes_sigma': create_bytearray(sigma_genes),
-            'normalized_genes_mean': create_bytearray(
-                self._normalized_matrix.average_genes),
-            'normalized_genes_sigma': create_bytearray(normalized_sigma_genes)
-        }
-
-    def calculate_coloring_arrays(self):
-        file_names = {
-            ExpressionMetric.Count: 'cell_count',
-            ExpressionMetric.Normalized: 'cell_normalized',
-        }
-
-        self._make_cell_lists()
-        statisticsVariablesBtr = bytearray()
-
-        for metric in file_names.keys():
-            cell_metric_btr = bytearray()  # t[i]
-            for i in range(self._matrix.lines_cells):
-                cell_metric_btr.extend(np.float32(self._cellsMetricsList[metric.value][i]))
-
-            statisticsVariablesBtr.extend(np.float32(np.min(self._cellsMetricsList[metric.value])))
-            statisticsVariablesBtr.extend(np.float32(np.max(self._cellsMetricsList[metric.value])))
-            self._outputNameBtrDict[file_names[metric]] = cell_metric_btr
-
-        for metric in file_names.keys():
-            statisticsVariablesBtr.extend(self._metricExtr[metric.value][0])
-            statisticsVariablesBtr.extend(self._metricExtr[metric.value][1])
-
-        self._outputNameBtrDict['statistics_variables'] = statisticsVariablesBtr
-        return self._outputNameBtrDict
+from copy import deepcopy
+from typing import List
+import numpy as np
+
+from vpt.update_vzg.assemble.expression_matrix import GeneExprMatrix, ExpressionMetric
+
+
+def create_bytearray(array_l, array_type=np.float32) -> bytearray:
+    output_btr = bytearray()
+    for element in array_l:
+        output_btr.extend(array_type(element))
+
+    return output_btr
+
+
+class CellColoring:
+    def __init__(self, matrix: GeneExprMatrix):
+        self._matrix = matrix
+        self._normalized_matrix = None
+        self._cellsMetricsList: List = []
+
+        self._metricExtr = []
+        for i in range(ExpressionMetric.ItemsCount.value):
+            self._cellsMetricsList.append(np.zeros(matrix.lines_cells, np.float32))
+            self._metricExtr.append(np.zeros(2, np.float32))
+            self._metricExtr[i][0] = float('inf')
+            self._metricExtr[i][1] = float('-inf')
+
+        self._outputNameBtrDict: dict = {}
+
+    def _make_cell_lists(self):
+        data = self._matrix.data
+        sigma_genes = []
+        for genes_column in self._matrix.data.T:
+            sigma_genes.append(np.std(genes_column))
+
+        self._metricExtr[ExpressionMetric.Count.value][0] = data.min()
+        self._metricExtr[ExpressionMetric.Count.value][1] = data.max()
+
+        for i, row_transcripts in enumerate(data):
+            self._cellsMetricsList[ExpressionMetric.Count.value][i] = np.sum(row_transcripts)
+
+        self._normalized_matrix: GeneExprMatrix = deepcopy(self._matrix)
+        self._normalized_matrix.change_matrix_data_from_origin(ExpressionMetric.Normalized)
+        normalized_data = self._normalized_matrix.data
+        normalized_sigma_genes = []
+
+        self._metricExtr[ExpressionMetric.Normalized.value][0] = normalized_data.min()
+        self._metricExtr[ExpressionMetric.Normalized.value][1] = normalized_data.max()
+
+        for genes_column in self._normalized_matrix.data.T:
+            normalized_sigma_genes.append(np.std(genes_column))
+
+        for i, row_transcripts in enumerate(normalized_data):
+            self._cellsMetricsList[ExpressionMetric.Normalized.value][i] = np.sum(row_transcripts)
+
+        self._outputNameBtrDict: dict = {
+            'genes_mean': create_bytearray(self._matrix.average_genes),
+            'genes_sigma': create_bytearray(sigma_genes),
+            'normalized_genes_mean': create_bytearray(
+                self._normalized_matrix.average_genes),
+            'normalized_genes_sigma': create_bytearray(normalized_sigma_genes)
+        }
+
+    def calculate_coloring_arrays(self):
+        file_names = {
+            ExpressionMetric.Count: 'cell_count',
+            ExpressionMetric.Normalized: 'cell_normalized',
+        }
+
+        self._make_cell_lists()
+        statisticsVariablesBtr = bytearray()
+
+        for metric in file_names.keys():
+            cell_metric_btr = bytearray()  # t[i]
+            for i in range(self._matrix.lines_cells):
+                cell_metric_btr.extend(np.float32(self._cellsMetricsList[metric.value][i]))
+
+            statisticsVariablesBtr.extend(np.float32(np.min(self._cellsMetricsList[metric.value])))
+            statisticsVariablesBtr.extend(np.float32(np.max(self._cellsMetricsList[metric.value])))
+            self._outputNameBtrDict[file_names[metric]] = cell_metric_btr
+
+        for metric in file_names.keys():
+            statisticsVariablesBtr.extend(self._metricExtr[metric.value][0])
+            statisticsVariablesBtr.extend(self._metricExtr[metric.value][1])
+
+        self._outputNameBtrDict['statistics_variables'] = statisticsVariablesBtr
+        return self._outputNameBtrDict
```

### Comparing `vpt-1.0.1/src/vpt/update_vzg/assemble/dataset_assemble.py` & `vpt-1.0.2/src/vpt/update_vzg/assemble/dataset_assemble.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-import os
-from typing import Optional
-
-import pandas
-
-from vpt.update_vzg.assemble.cell_coloring import CellColoring
-from vpt.update_vzg.assemble.expression_matrix import GeneExprMatrix
-from vpt.filesystem import vzg_open
-from vpt.update_vzg.cell_metadata import CellMetadata
-from vpt.utils.general_data import write_file
-
-
-def run_dataset_assembling(exprMatrixPath: str, outputDatasetPath: str,
-                           cellMetadata: CellMetadata,
-                           genes: Optional[list[str]] = None):
-    with vzg_open(exprMatrixPath, 'r') as f:
-        exprMatrixDF: pandas.DataFrame = pandas.read_csv(f, index_col=0)
-
-    # Sort cell by gene matrix by EntityID if it isn't already sorted
-    exprMatrixDF = exprMatrixDF.sort_index()
-
-    if genes:
-        exprMatrixDF = exprMatrixDF.assign(**{g: 0 for g in set(genes) - set(exprMatrixDF.columns)})
-        exprMatrixDF = exprMatrixDF.reindex(columns=genes)
-
-    exprMatrix = GeneExprMatrix(exprMatrixDF, cellMetadata)
-
-    print('Start calculating expression matrices')
-    exprMatrixFolder = os.path.join('assemble', 'expression_matrix')
-    transcripts_gene_number_btr, transcripts_gene_indices_btr =\
-        exprMatrix.generate_sparse_gene_expr_matrix_data()
-    write_file(outputDatasetPath, transcripts_gene_number_btr,
-               'sparse_gene_expr_matrix.bin', exprMatrixFolder)
-    write_file(outputDatasetPath, transcripts_gene_indices_btr,
-               'expr_matrix_gene_indices.bin', exprMatrixFolder)
-
-    transcripts_cell_number_btr, transcripts_cell_indices_btr =\
-        exprMatrix.generate_sparse_cell_expr_matrix_data()
-    write_file(outputDatasetPath, transcripts_cell_number_btr,
-               'sparse_cell_expr_matrix.bin', exprMatrixFolder)
-    write_file(outputDatasetPath, transcripts_cell_indices_btr,
-               'expr_matrix_cell_indices.bin', exprMatrixFolder)
-
-    print('Start calculating coloring arrays')
-    cellColoring = CellColoring(exprMatrix)
-    nameBtrDict = cellColoring.calculate_coloring_arrays()
-
-    cellColoringFolder = os.path.join('assemble', 'coloring_arrays')
-    for fileName, resultBtr in nameBtrDict.items():
-        write_file(outputDatasetPath, resultBtr, f'{fileName}.bin', cellColoringFolder)
-
-    print('Finish calculating')
+import os
+from typing import Optional
+
+import pandas
+
+from vpt.update_vzg.assemble.cell_coloring import CellColoring
+from vpt.update_vzg.assemble.expression_matrix import GeneExprMatrix
+from vpt.filesystem import vzg_open
+from vpt.update_vzg.cell_metadata import CellMetadata
+from vpt.utils.general_data import write_file
+
+
+def run_dataset_assembling(exprMatrixPath: str, outputDatasetPath: str,
+                           cellMetadata: CellMetadata,
+                           genes: Optional[list[str]] = None):
+    with vzg_open(exprMatrixPath, 'r') as f:
+        exprMatrixDF: pandas.DataFrame = pandas.read_csv(f, index_col=0)
+
+    # Sort cell by gene matrix by EntityID if it isn't already sorted
+    exprMatrixDF = exprMatrixDF.sort_index()
+
+    if genes:
+        exprMatrixDF = exprMatrixDF.assign(**{g: 0 for g in set(genes) - set(exprMatrixDF.columns)})
+        exprMatrixDF = exprMatrixDF.reindex(columns=genes)
+
+    exprMatrix = GeneExprMatrix(exprMatrixDF, cellMetadata)
+
+    print('Start calculating expression matrices')
+    exprMatrixFolder = os.path.join('assemble', 'expression_matrix')
+    transcripts_gene_number_btr, transcripts_gene_indices_btr =\
+        exprMatrix.generate_sparse_gene_expr_matrix_data()
+    write_file(outputDatasetPath, transcripts_gene_number_btr,
+               'sparse_gene_expr_matrix.bin', exprMatrixFolder)
+    write_file(outputDatasetPath, transcripts_gene_indices_btr,
+               'expr_matrix_gene_indices.bin', exprMatrixFolder)
+
+    transcripts_cell_number_btr, transcripts_cell_indices_btr =\
+        exprMatrix.generate_sparse_cell_expr_matrix_data()
+    write_file(outputDatasetPath, transcripts_cell_number_btr,
+               'sparse_cell_expr_matrix.bin', exprMatrixFolder)
+    write_file(outputDatasetPath, transcripts_cell_indices_btr,
+               'expr_matrix_cell_indices.bin', exprMatrixFolder)
+
+    print('Start calculating coloring arrays')
+    cellColoring = CellColoring(exprMatrix)
+    nameBtrDict = cellColoring.calculate_coloring_arrays()
+
+    cellColoringFolder = os.path.join('assemble', 'coloring_arrays')
+    for fileName, resultBtr in nameBtrDict.items():
+        write_file(outputDatasetPath, resultBtr, f'{fileName}.bin', cellColoringFolder)
+
+    print('Finish calculating')
```

### Comparing `vpt-1.0.1/src/vpt/update_vzg/assemble/expression_matrix.py` & `vpt-1.0.2/src/vpt/update_vzg/assemble/expression_matrix.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,141 +1,141 @@
-from enum import Enum
-from typing import Union
-
-import numpy as np
-import pandas
-
-from vpt.update_vzg.cell_metadata import CellMetadata
-
-
-class ExpressionMetric(Enum):
-    Count = 0  # Genes Sum
-    Normalized = 1  # divided on cell volume
-    ItemsCount = 2
-
-
-class GeneExprMatrix:
-    """
-        Original expression matrix looks like (schema 1):
-            Gene0   |   Gene1   |   Gene2   |   Gene3   |   Gene4  |   Gene5   |   Gene6
-    Cell0|    0     |     5     |     0     |     0     |     3    |     0     |    0
-    Cell1|    2     |     1     |     0     |     0     |     0    |     5     |    0
-    Cell2|    0     |     0     |     4     |     3     |     0    |     8     |    7
-    """
-
-    def __init__(self, exprMatrix: pandas.DataFrame, cellMetadata: CellMetadata):
-        self._cellMetaData = cellMetadata
-        self.data = np.zeros(0)
-        self.columns_genes = 0
-        self.lines_cells = 0
-
-        self.average_sum = None  # μ
-        self.std = None  # σ
-        self.average_genes = None
-
-        self._load_matrix_data(exprMatrix)
-
-    def _calculate_statistic_variables(self):
-        self.average_sum = np.mean(self.data)  # μ
-        self.std = np.std(self.data)  # σ
-        self.average_genes = np.array(self.columns_genes)
-
-        self.average_genes = np.mean(self.data, 0)
-
-    def _load_matrix_data(self, exprMatrix):
-
-        exprMatrix = exprMatrix.sort_index()
-        self.data = exprMatrix.to_numpy()
-        self.lines_cells = len(self.data)
-        self.columns_genes = len(self.data[0])
-
-        self._calculate_statistic_variables()
-
-    def change_matrix_data_from_origin(self, creation: ExpressionMetric):
-        if creation == ExpressionMetric.Normalized:
-            self._normalize_data_by_cell_volume(self.data)
-            self._calculate_statistic_variables()
-
-    def _normalize_data_by_cell_volume(self, origin_data):
-        volume_np = self._cellMetaData.get_volume_array()
-
-        self.lines_cells, self.columns_genes = len(origin_data), len(origin_data[0])
-
-        self.data = np.zeros((self.lines_cells, self.columns_genes), np.float32)
-        for cell_number, cell_row in enumerate(self.data):
-            cell_volume = volume_np[cell_number]
-            self.data[cell_number] = origin_data[cell_number] / cell_volume
-
-    def generate_sparse_gene_expr_matrix_data(self) -> Union[bytearray, bytearray]:
-        """
-            Original matrix is rather sparse, so we need to store data efficiently, this function generate 3 arrays,
-        that determine information that we use from original matrix (example from scheme 1):
-            1. An array of the number of gene transcripts in cells and their gene numbers :
-            |   5   |   3   |   2   |   1   |   5   |   4   |   3   |   8   |   7   |
-            |   1   |   4   |   0   |   1   |   5   |   2   |   3   |   5   |   6   |
-            2. Array of cell indices:
-            |   0   |   2   |   5   |
-            3. An array of maximum numbers of gene transcripts in cells:
-            |   2   |   5   |   4   |   3   |   3   |   8   |   7   |
-        """
-        transcripts_gene_number_btr = bytearray()
-        transcripts_gene_indices_btr = bytearray()
-        genesCountList = []
-        genesArrayList = []
-        geneIndexList = []
-
-        writen_element_id = 0
-        for cell_line in range(self.lines_cells):
-            first_gene = True
-            genesCountList.append(
-                str(cell_line) + ' ' + str(np.sum(self.data[cell_line])) + '\n')
-            for gene_number in range(self.columns_genes):
-                transcripts_count = self.data[cell_line][gene_number]
-                if transcripts_count != 0:
-                    if first_gene:
-                        transcripts_gene_indices_btr.extend(np.uint32(writen_element_id))
-                        first_gene = False
-                        geneIndexList.append(str(writen_element_id) + '\n')
-
-                    transcripts_gene_number_btr.extend(np.uint32(transcripts_count))
-                    transcripts_gene_number_btr.extend(np.uint32(gene_number))
-                    genesArrayList.append(
-                        str(transcripts_count) + ' ' + str(gene_number) + '\n')
-                    writen_element_id += 1
-
-            if first_gene:
-                transcripts_gene_indices_btr.extend(np.uint32(writen_element_id))
-                geneIndexList.append(str(writen_element_id) + '\n')
-
-        return transcripts_gene_number_btr, transcripts_gene_indices_btr
-
-    def generate_sparse_cell_expr_matrix_data(self):
-        """
-        Function makes 2 arrays from original expression matrix, unlike generate_sparse_cell_expr_matrix_data it is made
-        along the Y (cell) axis.
-        1. Non-zero matrix elements are ordered in the array by genes :
-        |   2   |   5   |   1   |   4   |   3   |   3   |   5   |   8   |   7   |
-        |   1   |   0   |   1   |   2   |   2   |   0   |   1   |   2   |   2   |
-        2. Array of indices:
-        |   0   |   1   |   3   |   4   |   5   |   6   |   8   |
-        """
-        transcripts_cell_number_btr = bytearray()
-        transcripts_cell_indices_btr = bytearray()
-
-        writen_element_id = 0
-        for gene_column in range(self.columns_genes):
-            first_cell = True
-            for cell_line in range(self.lines_cells):
-                transcripts_count = self.data[cell_line][gene_column]
-                if transcripts_count != 0:
-                    if first_cell:
-                        transcripts_cell_indices_btr.extend(np.uint32(writen_element_id))
-                        first_cell = False
-
-                    transcripts_cell_number_btr.extend(np.uint32(transcripts_count))
-                    transcripts_cell_number_btr.extend(np.uint32(cell_line))
-                    writen_element_id += 1
-
-            if first_cell:
-                transcripts_cell_indices_btr.extend(np.uint32(writen_element_id))
-
-        return transcripts_cell_number_btr, transcripts_cell_indices_btr
+from enum import Enum
+from typing import Union
+
+import numpy as np
+import pandas
+
+from vpt.update_vzg.cell_metadata import CellMetadata
+
+
+class ExpressionMetric(Enum):
+    Count = 0  # Genes Sum
+    Normalized = 1  # divided on cell volume
+    ItemsCount = 2
+
+
+class GeneExprMatrix:
+    """
+        Original expression matrix looks like (schema 1):
+            Gene0   |   Gene1   |   Gene2   |   Gene3   |   Gene4  |   Gene5   |   Gene6
+    Cell0|    0     |     5     |     0     |     0     |     3    |     0     |    0
+    Cell1|    2     |     1     |     0     |     0     |     0    |     5     |    0
+    Cell2|    0     |     0     |     4     |     3     |     0    |     8     |    7
+    """
+
+    def __init__(self, exprMatrix: pandas.DataFrame, cellMetadata: CellMetadata):
+        self._cellMetaData = cellMetadata
+        self.data = np.zeros(0)
+        self.columns_genes = 0
+        self.lines_cells = 0
+
+        self.average_sum = None  # μ
+        self.std = None  # σ
+        self.average_genes = None
+
+        self._load_matrix_data(exprMatrix)
+
+    def _calculate_statistic_variables(self):
+        self.average_sum = np.mean(self.data)  # μ
+        self.std = np.std(self.data)  # σ
+        self.average_genes = np.array(self.columns_genes)
+
+        self.average_genes = np.mean(self.data, 0)
+
+    def _load_matrix_data(self, exprMatrix):
+
+        exprMatrix = exprMatrix.sort_index()
+        self.data = exprMatrix.to_numpy()
+        self.lines_cells = len(self.data)
+        self.columns_genes = len(self.data[0])
+
+        self._calculate_statistic_variables()
+
+    def change_matrix_data_from_origin(self, creation: ExpressionMetric):
+        if creation == ExpressionMetric.Normalized:
+            self._normalize_data_by_cell_volume(self.data)
+            self._calculate_statistic_variables()
+
+    def _normalize_data_by_cell_volume(self, origin_data):
+        volume_np = self._cellMetaData.get_volume_array()
+
+        self.lines_cells, self.columns_genes = len(origin_data), len(origin_data[0])
+
+        self.data = np.zeros((self.lines_cells, self.columns_genes), np.float32)
+        for cell_number, cell_row in enumerate(self.data):
+            cell_volume = volume_np[cell_number]
+            self.data[cell_number] = origin_data[cell_number] / cell_volume
+
+    def generate_sparse_gene_expr_matrix_data(self) -> Union[bytearray, bytearray]:
+        """
+            Original matrix is rather sparse, so we need to store data efficiently, this function generate 3 arrays,
+        that determine information that we use from original matrix (example from scheme 1):
+            1. An array of the number of gene transcripts in cells and their gene numbers :
+            |   5   |   3   |   2   |   1   |   5   |   4   |   3   |   8   |   7   |
+            |   1   |   4   |   0   |   1   |   5   |   2   |   3   |   5   |   6   |
+            2. Array of cell indices:
+            |   0   |   2   |   5   |
+            3. An array of maximum numbers of gene transcripts in cells:
+            |   2   |   5   |   4   |   3   |   3   |   8   |   7   |
+        """
+        transcripts_gene_number_btr = bytearray()
+        transcripts_gene_indices_btr = bytearray()
+        genesCountList = []
+        genesArrayList = []
+        geneIndexList = []
+
+        writen_element_id = 0
+        for cell_line in range(self.lines_cells):
+            first_gene = True
+            genesCountList.append(
+                str(cell_line) + ' ' + str(np.sum(self.data[cell_line])) + '\n')
+            for gene_number in range(self.columns_genes):
+                transcripts_count = self.data[cell_line][gene_number]
+                if transcripts_count != 0:
+                    if first_gene:
+                        transcripts_gene_indices_btr.extend(np.uint32(writen_element_id))
+                        first_gene = False
+                        geneIndexList.append(str(writen_element_id) + '\n')
+
+                    transcripts_gene_number_btr.extend(np.uint32(transcripts_count))
+                    transcripts_gene_number_btr.extend(np.uint32(gene_number))
+                    genesArrayList.append(
+                        str(transcripts_count) + ' ' + str(gene_number) + '\n')
+                    writen_element_id += 1
+
+            if first_gene:
+                transcripts_gene_indices_btr.extend(np.uint32(writen_element_id))
+                geneIndexList.append(str(writen_element_id) + '\n')
+
+        return transcripts_gene_number_btr, transcripts_gene_indices_btr
+
+    def generate_sparse_cell_expr_matrix_data(self):
+        """
+        Function makes 2 arrays from original expression matrix, unlike generate_sparse_cell_expr_matrix_data it is made
+        along the Y (cell) axis.
+        1. Non-zero matrix elements are ordered in the array by genes :
+        |   2   |   5   |   1   |   4   |   3   |   3   |   5   |   8   |   7   |
+        |   1   |   0   |   1   |   2   |   2   |   0   |   1   |   2   |   2   |
+        2. Array of indices:
+        |   0   |   1   |   3   |   4   |   5   |   6   |   8   |
+        """
+        transcripts_cell_number_btr = bytearray()
+        transcripts_cell_indices_btr = bytearray()
+
+        writen_element_id = 0
+        for gene_column in range(self.columns_genes):
+            first_cell = True
+            for cell_line in range(self.lines_cells):
+                transcripts_count = self.data[cell_line][gene_column]
+                if transcripts_count != 0:
+                    if first_cell:
+                        transcripts_cell_indices_btr.extend(np.uint32(writen_element_id))
+                        first_cell = False
+
+                    transcripts_cell_number_btr.extend(np.uint32(transcripts_count))
+                    transcripts_cell_number_btr.extend(np.uint32(cell_line))
+                    writen_element_id += 1
+
+            if first_cell:
+                transcripts_cell_indices_btr.extend(np.uint32(writen_element_id))
+
+        return transcripts_cell_number_btr, transcripts_cell_indices_btr
```

### Comparing `vpt-1.0.1/src/vpt/update_vzg/cell_metadata.py` & `vpt-1.0.2/src/vpt/update_vzg/cell_metadata.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-import numpy as np
-import pandas
-
-from vpt.update_vzg.imageparams import ImageParams
-from vpt.utils.general_data import extend_btr_by_fixed_str
-
-
-class PointTransform:
-    def __init__(self, imageParams: ImageParams):
-        self._texture_width, self._texture_height = imageParams.textureSize
-        self._t_m = imageParams.micronToPixelMatrix
-
-    def make_transform(self, x, y) -> tuple:
-        x_texture = x * self._t_m[0][0] + self._t_m[0][2]
-        y_texture = y * self._t_m[1][1] + self._t_m[1][2]
-
-        x_world = x_texture / self._texture_width
-        y_world = (1.0 - y_texture / self._texture_height)
-
-        return x_world, y_world
-
-
-class CellMetadata:
-
-    MAX_BYTE_ID = 40
-
-    def __init__(self, metadataDF: pandas.DataFrame, imageParams: ImageParams = None):
-        self._volume_np: np.array
-        self._centroid_np: np.array
-        self._id_l: np.chararray
-
-        self._cells_count = 0
-        self._load(metadataDF, imageParams)
-
-    def _load(self, metadataDF, imageParams: ImageParams):
-        metadataDF = metadataDF.sort_index()
-        self._id_l = list(map(str, metadataDF.index.tolist()))
-        self._cells_count = len(self._id_l)
-        self._volume_np = metadataDF.loc[:, 'volume'].values.tolist()
-        centersMicrons = metadataDF.loc[:, ['center_x', 'center_y']].values.tolist()
-
-        if imageParams is not None:
-            point_transform = PointTransform(imageParams)
-            self._centroid_np = [point_transform.make_transform(coord[0], coord[1]) for coord in centersMicrons]
-
-    def get_volume_array(self) -> np.array:
-        return self._volume_np
-
-    def get_names_array(self) -> np.array:
-        return self._id_l
-
-    def get_cell_metadata_array(self) -> bytearray:
-        cell_metadata_btr = bytearray()
-        for cell_idx in range(self._cells_count):
-            extend_btr_by_fixed_str(cell_metadata_btr, self._id_l[cell_idx], self.MAX_BYTE_ID)
-            cell_metadata_btr.extend(np.float32(self._volume_np[cell_idx]))
-
-            cell_metadata_btr.extend(np.float32(self._centroid_np[cell_idx][0]))
-            cell_metadata_btr.extend(np.float32(self._centroid_np[cell_idx][1]))
-
-        # write
-        output_btr = bytearray()
-        output_btr.extend(np.uint32(self._cells_count))  # cell count
-        output_btr.extend(np.uint32(self.MAX_BYTE_ID))  # Size in bytes of one name
-
-        output_btr.extend(cell_metadata_btr)
-        return output_btr
+import numpy as np
+import pandas
+
+from vpt.update_vzg.imageparams import ImageParams
+from vpt.utils.general_data import extend_btr_by_fixed_str
+
+
+class PointTransform:
+    def __init__(self, imageParams: ImageParams):
+        self._texture_width, self._texture_height = imageParams.textureSize
+        self._t_m = imageParams.micronToPixelMatrix
+
+    def make_transform(self, x, y) -> tuple:
+        x_texture = x * self._t_m[0][0] + self._t_m[0][2]
+        y_texture = y * self._t_m[1][1] + self._t_m[1][2]
+
+        x_world = x_texture / self._texture_width
+        y_world = (1.0 - y_texture / self._texture_height)
+
+        return x_world, y_world
+
+
+class CellMetadata:
+
+    MAX_BYTE_ID = 40
+
+    def __init__(self, metadataDF: pandas.DataFrame, imageParams: ImageParams = None):
+        self._volume_np: np.array
+        self._centroid_np: np.array
+        self._id_l: np.chararray
+
+        self._cells_count = 0
+        self._load(metadataDF, imageParams)
+
+    def _load(self, metadataDF, imageParams: ImageParams):
+        metadataDF = metadataDF.sort_index()
+        self._id_l = list(map(str, metadataDF.index.tolist()))
+        self._cells_count = len(self._id_l)
+        self._volume_np = metadataDF.loc[:, 'volume'].values.tolist()
+        centersMicrons = metadataDF.loc[:, ['center_x', 'center_y']].values.tolist()
+
+        if imageParams is not None:
+            point_transform = PointTransform(imageParams)
+            self._centroid_np = [point_transform.make_transform(coord[0], coord[1]) for coord in centersMicrons]
+
+    def get_volume_array(self) -> np.array:
+        return self._volume_np
+
+    def get_names_array(self) -> np.array:
+        return self._id_l
+
+    def get_cell_metadata_array(self) -> bytearray:
+        cell_metadata_btr = bytearray()
+        for cell_idx in range(self._cells_count):
+            extend_btr_by_fixed_str(cell_metadata_btr, self._id_l[cell_idx], self.MAX_BYTE_ID)
+            cell_metadata_btr.extend(np.float32(self._volume_np[cell_idx]))
+
+            cell_metadata_btr.extend(np.float32(self._centroid_np[cell_idx][0]))
+            cell_metadata_btr.extend(np.float32(self._centroid_np[cell_idx][1]))
+
+        # write
+        output_btr = bytearray()
+        output_btr.extend(np.uint32(self._cells_count))  # cell count
+        output_btr.extend(np.uint32(self.MAX_BYTE_ID))  # Size in bytes of one name
+
+        output_btr.extend(cell_metadata_btr)
+        return output_btr
```

### Comparing `vpt-1.0.1/src/vpt/update_vzg/cmd_args.py` & `vpt-1.0.2/src/vpt/update_vzg/cmd_args.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,57 +1,58 @@
-from argparse import ArgumentParser
-from dataclasses import dataclass
-import os
-
-from vpt.utils.validate import validate_exists, validate_does_not_exist
-
-# The maximum number of parallel processes that may be launched by update-vzg
-MAX_PROCESSES = 512
-
-
-@dataclass
-class UpdateVzgArgs:
-    input_vzg: str
-    input_boundaries: str
-    input_entity_by_gene: str
-    output_vzg: str
-    input_metadata: str
-    temp_path: str
-    overwrite: bool
-
-
-def validate_args(args: UpdateVzgArgs):
-    validate_exists(args.input_vzg)
-    validate_exists(args.input_boundaries)
-    validate_exists(args.input_entity_by_gene)
-
-    if not args.overwrite:
-        validate_does_not_exist(args.output_vzg)
-
-
-def get_parser() -> ArgumentParser:
-    parser = ArgumentParser(description='Updates an existing .vzg file with new segmentation boundaries and the '
-                            'corresponding expression matrix. NOTE: This functionality requires '
-                            'enough disk space to unpack the existing .vzg file.',
-                            add_help=False
-                            )
-
-    required = parser.add_argument_group('Required arguments')
-    required.add_argument('--input-vzg', required=True, type=str,
-                          help='Path to an existing vzg file.')
-    required.add_argument('--input-boundaries', required=True, type=str,
-                          help='Path to a micron-space parquet boundary file.')
-    required.add_argument('--input-entity-by-gene', required=True, type=str,
-                          help='Path to the Entity by gene csv file.')
-    required.add_argument('--output-vzg', required=True, type=str,
-                          help='Path where the updated vzg should be saved.')
-
-    opt = parser.add_argument_group('Optional arguments')
-    opt.add_argument('--input-metadata', required=False, type=str,
-                     help='Path to an existing entity metadata file.')
-    opt.add_argument('--temp-path', required=False, type=str, default=os.path.join(os.getcwd(), 'vzg_build_temp'),
-                     help='Path for temporary folder for unzipping vzg file.')
-    opt.add_argument('--overwrite', action='store_true', default=False, required=False,
-                     help='Set flag if you want to use non empty directory and agree that files can be over-written.')
-    opt.add_argument("-h", "--help", action="help", help="Show this help message and exit")
-
-    return parser
+from argparse import ArgumentParser
+from dataclasses import dataclass
+import os
+
+from vpt.utils.validate import validate_exists, validate_does_not_exist, validate_directory_empty
+
+# The maximum number of parallel processes that may be launched by update-vzg
+MAX_PROCESSES = 512
+
+
+@dataclass
+class UpdateVzgArgs:
+    input_vzg: str
+    input_boundaries: str
+    input_entity_by_gene: str
+    output_vzg: str
+    input_metadata: str
+    temp_path: str
+    overwrite: bool
+
+
+def validate_args(args: UpdateVzgArgs):
+    validate_exists(args.input_vzg)
+    validate_exists(args.input_boundaries)
+    validate_exists(args.input_entity_by_gene)
+    validate_directory_empty(args.temp_path)
+
+    if not args.overwrite:
+        validate_does_not_exist(args.output_vzg)
+
+
+def get_parser() -> ArgumentParser:
+    parser = ArgumentParser(description='Updates an existing .vzg file with new segmentation boundaries and the '
+                            'corresponding expression matrix. NOTE: This functionality requires '
+                            'enough disk space to unpack the existing .vzg file.',
+                            add_help=False
+                            )
+
+    required = parser.add_argument_group('Required arguments')
+    required.add_argument('--input-vzg', required=True, type=str,
+                          help='Path to an existing vzg file.')
+    required.add_argument('--input-boundaries', required=True, type=str,
+                          help='Path to a micron-space parquet boundary file.')
+    required.add_argument('--input-entity-by-gene', required=True, type=str,
+                          help='Path to the Entity by gene csv file.')
+    required.add_argument('--output-vzg', required=True, type=str,
+                          help='Path where the updated vzg should be saved.')
+
+    opt = parser.add_argument_group('Optional arguments')
+    opt.add_argument('--input-metadata', required=False, type=str,
+                     help='Path to an existing entity metadata file.')
+    opt.add_argument('--temp-path', required=False, type=str, default=os.path.join(os.getcwd(), 'vzg_build_temp'),
+                     help='Path for temporary folder for unzipping vzg file.')
+    opt.add_argument('--overwrite', action='store_true', default=False, required=False,
+                     help='Set flag if you want to use non empty directory and agree that files can be over-written.')
+    opt.add_argument("-h", "--help", action="help", help="Show this help message and exit")
+
+    return parser
```

### Comparing `vpt-1.0.1/src/vpt/update_vzg/polygon_transfer.py` & `vpt-1.0.2/src/vpt/update_vzg/polygon_transfer.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,225 +1,225 @@
-import numpy as np
-from typing import List, Dict, Tuple
-import math
-
-from vpt.update_vzg.cell_metadata import CellMetadata
-from vpt.update_vzg.imageparams import ImageParams
-
-from vpt.update_vzg.polygons.packedfanpolygon import PackedFanPolygon
-from vpt.update_vzg.polygons.packedpolygon import LodLevel
-from vpt.update_vzg.polygons.packedstarpolygon import PackedStarPolygon
-from vpt.update_vzg.polygons.polygonset import PolygonSet
-from vpt.utils.raw_cell import Feature
-from vpt.utils.general_data import grid_size_calculate
-
-
-class CellTransfer:
-    """Class for transferring spatialFeature objects to PolygonSet objects.
-    """
-
-    def __init__(self, imageParams: ImageParams):
-
-        self._mtpMatrix = imageParams.micronToPixelMatrix
-        self._textureSize = imageParams.textureSize
-
-        self._expBbox = (self._textureSize[0] / self._mtpMatrix[0][0],
-                         self._textureSize[1] / self._mtpMatrix[1][1])
-        self._gridSize = grid_size_calculate(self._textureSize, self._mtpMatrix)
-        self.gridPolyCounts = self._gridSize[0] * self._gridSize[1]
-
-    def process_cells(self,
-                      rawCellsList: List[Feature],
-                      fovIdx: int
-                      ) -> List[PolygonSet]:
-        """Transfer points: thinning out, transformation to the new domain"""
-        polygonsList = []
-        for rawCell in rawCellsList:
-            for z_slice, zSlicePoly in enumerate(rawCell.shapes):
-                if zSlicePoly is None or zSlicePoly.is_empty:
-                    continue
-                poly = zSlicePoly.geoms[0]
-                rawId = rawCell.get_feature_id()
-                x_center, y_center = poly.centroid.x, poly.centroid.y
-
-                true_coords = np.column_stack(poly.exterior.coords.xy)
-                polygon = PolygonSet(z_slice, x_center, y_center, rawId)
-                poly_relevant_reduce = polygon.points_transform(
-                    true_coords, self._mtpMatrix, self._textureSize,
-                    self._gridSize, self._expBbox)
-
-                if poly_relevant_reduce:
-                    polygonsList.append(polygon)
-
-        print(f'Done fov {fovIdx}')
-        return polygonsList
-
-
-class CellsTransfer:
-    def __init__(self, cellMetadata: CellMetadata, zCount: int, imageParams: ImageParams):
-        self._zCount = zCount
-        self.grid: List[Dict[int:List[PolygonSet]]] = []
-
-        self._cellMetadata = cellMetadata
-        self._cellsIdDict: Dict[str: int] = \
-            {name: i for i, name in enumerate(cellMetadata.get_names_array())}
-
-        self._cellsCount = len(self._cellsIdDict)
-        self.pointersToPolys = None
-
-        self._mtpMatrix = imageParams.micronToPixelMatrix
-        self._textureSize = imageParams.textureSize
-        self._gridSize = grid_size_calculate(imageParams.textureSize, imageParams.micronToPixelMatrix)
-        self._init_grid()
-
-    def get_z_panes_count(self):
-        return self._zCount
-
-    def _init_grid(self):
-        for z_slice in range(self._zCount):
-            self.grid.append({})
-            for key in range(self._gridSize[0] * self._gridSize[1]):
-                self.grid[z_slice][key] = []
-
-    def fill_grid(self, polyList):
-        """Associate voxels with cells"""
-        gridSize = self._gridSize[0] * self._gridSize[1]
-        mtpMatrix = self._mtpMatrix
-        for polySet in polyList:
-            p: PolygonSet = polySet
-            (cx, cy, z) = p.get_center()
-            spatId = p.get_spatial_id()
-            p.set_cell_id(self._cellsIdDict[spatId])
-            x_ind: int = math.floor(
-                (cx * mtpMatrix[0][0] + mtpMatrix[0][2]) / self._textureSize[0] * self._gridSize[0])
-            y_ind: int = math.floor(
-                (1.0 - (cy * mtpMatrix[1][1] + mtpMatrix[1][2]) / self._textureSize[1]) * self._gridSize[1])
-
-            gridNumber = y_ind * self._gridSize[0] + x_ind
-            if gridNumber < 0 or gridNumber >= gridSize:
-                print(f'Poly with coordinates {cx} and {cy} is out of the area. Z is {z}, id: {spatId}.'
-                      f' Getting grid coordinates {x_ind} and {y_ind}')
-                continue
-            self.grid[z][gridNumber].append(polySet)
-
-    def get_cells_by_lod(self, lodLevel: LodLevel) -> list:
-        """
-        Returns:
-             List of bytearrays of transferred-cells for current lod_level.
-        """
-        self.pointersToPolys = np.zeros((self._cellsCount, self._zCount, 2), dtype=np.uint32)
-
-        cellsLodList = []
-        for z_slice in range(self._zCount):
-            packedPolygonsDict = [[], [], [], []]
-            blocksCount = np.zeros(4, np.uint32)
-            polyVoxelGrid: List = \
-                [bytearray(), bytearray(), bytearray(), bytearray()]
-            # Step 5. Fill output buffers
-            self._make_points_buffer(lodLevel, z_slice,
-                                     packedPolygonsDict,
-                                     polyVoxelGrid,
-                                     blocksCount)
-
-            cellsLodList.append(self._build_cells_btr(
-                lodLevel, packedPolygonsDict, polyVoxelGrid))
-
-        return cellsLodList
-
-    def _make_points_buffer(self, lodLevel, zSlice, packedPolygonsDict,
-                            polyVoxelGrid,
-                            blocksCount):
-        polyIdx = [0, 0, 0, 0]
-
-        for polygons in self.grid[zSlice].values():
-            polyInVoxel = [0, 0, 0, 0]
-
-            for packSize in range(4):
-                polyVoxelGrid[packSize].extend(np.int32(polyIdx[packSize]))
-
-            for curr_poly in polygons:  # type: PolygonSet
-                cellId = curr_poly.get_cell_id()
-                polyType, packedPolygonsBytes = \
-                    curr_poly.get_packed_bytes(lodLevel)
-
-                if polyType >= 0:
-                    packedPolygonsDict[polyType].append(
-                        packedPolygonsBytes)
-
-                    polyInVoxel[polyType] += 1
-
-                    self.pointersToPolys[cellId][zSlice][0] = polyType + 1
-                    if lodLevel == LodLevel.Min:
-                        self.pointersToPolys[cellId][zSlice][0] = 1
-
-                    self.pointersToPolys[cellId][zSlice][1] = \
-                        blocksCount[polyType]
-                    blocksCount[polyType] += 1
-
-            for packSize in range(4):
-                polyVoxelGrid[packSize].extend(np.int32(polyInVoxel[packSize]))
-                polyIdx[packSize] += polyInVoxel[packSize]
-
-    @staticmethod
-    def _build_cells_btr(
-            lodLevel, packedPolygonsDict, polyVoxelGrid) -> bytearray:
-        output_btr = bytearray()
-        # ----  Header ----
-        packedPolyBtrDict = {}
-
-        for packSizeType in range(3):
-            if lodLevel == LodLevel.Min:
-                output_btr.extend(np.uint32(0))
-                continue
-
-            packedPolyBtrDict[packSizeType] = \
-                b''.join(packedPolygonsDict[packSizeType])
-            packedPolySize = PackedStarPolygon.get_bytes_count(
-                lodLevel, packSizeType)
-            if packedPolySize != 0:
-                output_btr.extend(np.uint32(len(packedPolyBtrDict[packSizeType])
-                                            / packedPolySize))
-            else:
-                output_btr.extend(np.uint32(0))
-
-        packedFanPolygons = b''.join(packedPolygonsDict[3])
-        packedPolySize = PackedFanPolygon.Bytes_Count[lodLevel.value]
-        if packedPolySize != 0:
-            output_btr.extend(np.uint32(
-                len(packedFanPolygons) / packedPolySize))
-        else:
-            output_btr.extend(np.uint32(0))
-
-        # ----  Data ----
-        if not lodLevel == LodLevel.Min:
-            for packSize in range(3):
-                output_btr.extend(packedPolyBtrDict[packSize])
-        output_btr.extend(packedFanPolygons)
-
-        if not lodLevel == LodLevel.Min:
-            for packSize in range(3):
-                output_btr.extend(polyVoxelGrid[packSize])
-        output_btr.extend(polyVoxelGrid[3])
-
-        return output_btr
-
-    def get_poly_pointer_arrays(self) -> Tuple[bytearray, bytearray]:
-        """
-        Returns:
-             (cell-array bytearray, polygon-pointer-array bytearrays).
-        """
-        pointersToPolyBtr = bytearray()
-        cellArray = bytearray()
-        cellIndex = 0
-        for _, cell in enumerate(self.pointersToPolys):
-            zSliceCount = 0
-            for zSlice, zSliceData in enumerate(cell):
-                if zSliceData[0] != 0:
-                    pointersToPolyBtr.extend(np.uint32(zSliceData[1]))
-                    pointersToPolyBtr.extend(np.int16(zSliceData[0] - 1))
-                    pointersToPolyBtr.extend(np.int16(zSlice))
-                    zSliceCount += 1
-            cellArray.extend(np.uint32(cellIndex))
-            cellArray.extend(np.int32(zSliceCount))
-            cellIndex += zSliceCount
-
-        return pointersToPolyBtr, cellArray
+import numpy as np
+from typing import List, Dict, Tuple
+import math
+
+from vpt.update_vzg.cell_metadata import CellMetadata
+from vpt.update_vzg.imageparams import ImageParams
+
+from vpt.update_vzg.polygons.packedfanpolygon import PackedFanPolygon
+from vpt.update_vzg.polygons.packedpolygon import LodLevel
+from vpt.update_vzg.polygons.packedstarpolygon import PackedStarPolygon
+from vpt.update_vzg.polygons.polygonset import PolygonSet
+from vpt.utils.raw_cell import Feature
+from vpt.utils.general_data import grid_size_calculate
+
+
+class CellTransfer:
+    """Class for transferring spatialFeature objects to PolygonSet objects.
+    """
+
+    def __init__(self, imageParams: ImageParams):
+
+        self._mtpMatrix = imageParams.micronToPixelMatrix
+        self._textureSize = imageParams.textureSize
+
+        self._expBbox = (self._textureSize[0] / self._mtpMatrix[0][0],
+                         self._textureSize[1] / self._mtpMatrix[1][1])
+        self._gridSize = grid_size_calculate(self._textureSize, self._mtpMatrix)
+        self.gridPolyCounts = self._gridSize[0] * self._gridSize[1]
+
+    def process_cells(self,
+                      rawCellsList: List[Feature],
+                      fovIdx: int
+                      ) -> List[PolygonSet]:
+        """Transfer points: thinning out, transformation to the new domain"""
+        polygonsList = []
+        for rawCell in rawCellsList:
+            for z_slice, zSlicePoly in enumerate(rawCell.shapes):
+                if zSlicePoly is None or zSlicePoly.is_empty:
+                    continue
+                poly = zSlicePoly.geoms[0]
+                rawId = rawCell.get_feature_id()
+                x_center, y_center = poly.centroid.x, poly.centroid.y
+
+                true_coords = np.column_stack(poly.exterior.coords.xy)
+                polygon = PolygonSet(z_slice, x_center, y_center, rawId)
+                poly_relevant_reduce = polygon.points_transform(
+                    true_coords, self._mtpMatrix, self._textureSize,
+                    self._gridSize, self._expBbox)
+
+                if poly_relevant_reduce:
+                    polygonsList.append(polygon)
+
+        print(f'Done fov {fovIdx}')
+        return polygonsList
+
+
+class CellsTransfer:
+    def __init__(self, cellMetadata: CellMetadata, zCount: int, imageParams: ImageParams):
+        self._zCount = zCount
+        self.grid: List[Dict[int:List[PolygonSet]]] = []
+
+        self._cellMetadata = cellMetadata
+        self._cellsIdDict: Dict[str: int] = \
+            {name: i for i, name in enumerate(cellMetadata.get_names_array())}
+
+        self._cellsCount = len(self._cellsIdDict)
+        self.pointersToPolys = None
+
+        self._mtpMatrix = imageParams.micronToPixelMatrix
+        self._textureSize = imageParams.textureSize
+        self._gridSize = grid_size_calculate(imageParams.textureSize, imageParams.micronToPixelMatrix)
+        self._init_grid()
+
+    def get_z_panes_count(self):
+        return self._zCount
+
+    def _init_grid(self):
+        for z_slice in range(self._zCount):
+            self.grid.append({})
+            for key in range(self._gridSize[0] * self._gridSize[1]):
+                self.grid[z_slice][key] = []
+
+    def fill_grid(self, polyList):
+        """Associate voxels with cells"""
+        gridSize = self._gridSize[0] * self._gridSize[1]
+        mtpMatrix = self._mtpMatrix
+        for polySet in polyList:
+            p: PolygonSet = polySet
+            (cx, cy, z) = p.get_center()
+            spatId = p.get_spatial_id()
+            p.set_cell_id(self._cellsIdDict[spatId])
+            x_ind: int = math.floor(
+                (cx * mtpMatrix[0][0] + mtpMatrix[0][2]) / self._textureSize[0] * self._gridSize[0])
+            y_ind: int = math.floor(
+                (1.0 - (cy * mtpMatrix[1][1] + mtpMatrix[1][2]) / self._textureSize[1]) * self._gridSize[1])
+
+            gridNumber = y_ind * self._gridSize[0] + x_ind
+            if gridNumber < 0 or gridNumber >= gridSize:
+                print(f'Poly with coordinates {cx} and {cy} is out of the area. Z is {z}, id: {spatId}.'
+                      f' Getting grid coordinates {x_ind} and {y_ind}')
+                continue
+            self.grid[z][gridNumber].append(polySet)
+
+    def get_cells_by_lod(self, lodLevel: LodLevel) -> list:
+        """
+        Returns:
+             List of bytearrays of transferred-cells for current lod_level.
+        """
+        self.pointersToPolys = np.zeros((self._cellsCount, self._zCount, 2), dtype=np.uint32)
+
+        cellsLodList = []
+        for z_slice in range(self._zCount):
+            packedPolygonsDict = [[], [], [], []]
+            blocksCount = np.zeros(4, np.uint32)
+            polyVoxelGrid: List = \
+                [bytearray(), bytearray(), bytearray(), bytearray()]
+            # Step 5. Fill output buffers
+            self._make_points_buffer(lodLevel, z_slice,
+                                     packedPolygonsDict,
+                                     polyVoxelGrid,
+                                     blocksCount)
+
+            cellsLodList.append(self._build_cells_btr(
+                lodLevel, packedPolygonsDict, polyVoxelGrid))
+
+        return cellsLodList
+
+    def _make_points_buffer(self, lodLevel, zSlice, packedPolygonsDict,
+                            polyVoxelGrid,
+                            blocksCount):
+        polyIdx = [0, 0, 0, 0]
+
+        for polygons in self.grid[zSlice].values():
+            polyInVoxel = [0, 0, 0, 0]
+
+            for packSize in range(4):
+                polyVoxelGrid[packSize].extend(np.int32(polyIdx[packSize]))
+
+            for curr_poly in polygons:  # type: PolygonSet
+                cellId = curr_poly.get_cell_id()
+                polyType, packedPolygonsBytes = \
+                    curr_poly.get_packed_bytes(lodLevel)
+
+                if polyType >= 0:
+                    packedPolygonsDict[polyType].append(
+                        packedPolygonsBytes)
+
+                    polyInVoxel[polyType] += 1
+
+                    self.pointersToPolys[cellId][zSlice][0] = polyType + 1
+                    if lodLevel == LodLevel.Min:
+                        self.pointersToPolys[cellId][zSlice][0] = 1
+
+                    self.pointersToPolys[cellId][zSlice][1] = \
+                        blocksCount[polyType]
+                    blocksCount[polyType] += 1
+
+            for packSize in range(4):
+                polyVoxelGrid[packSize].extend(np.int32(polyInVoxel[packSize]))
+                polyIdx[packSize] += polyInVoxel[packSize]
+
+    @staticmethod
+    def _build_cells_btr(
+            lodLevel, packedPolygonsDict, polyVoxelGrid) -> bytearray:
+        output_btr = bytearray()
+        # ----  Header ----
+        packedPolyBtrDict = {}
+
+        for packSizeType in range(3):
+            if lodLevel == LodLevel.Min:
+                output_btr.extend(np.uint32(0))
+                continue
+
+            packedPolyBtrDict[packSizeType] = \
+                b''.join(packedPolygonsDict[packSizeType])
+            packedPolySize = PackedStarPolygon.get_bytes_count(
+                lodLevel, packSizeType)
+            if packedPolySize != 0:
+                output_btr.extend(np.uint32(len(packedPolyBtrDict[packSizeType])
+                                            / packedPolySize))
+            else:
+                output_btr.extend(np.uint32(0))
+
+        packedFanPolygons = b''.join(packedPolygonsDict[3])
+        packedPolySize = PackedFanPolygon.Bytes_Count[lodLevel.value]
+        if packedPolySize != 0:
+            output_btr.extend(np.uint32(
+                len(packedFanPolygons) / packedPolySize))
+        else:
+            output_btr.extend(np.uint32(0))
+
+        # ----  Data ----
+        if not lodLevel == LodLevel.Min:
+            for packSize in range(3):
+                output_btr.extend(packedPolyBtrDict[packSize])
+        output_btr.extend(packedFanPolygons)
+
+        if not lodLevel == LodLevel.Min:
+            for packSize in range(3):
+                output_btr.extend(polyVoxelGrid[packSize])
+        output_btr.extend(polyVoxelGrid[3])
+
+        return output_btr
+
+    def get_poly_pointer_arrays(self) -> Tuple[bytearray, bytearray]:
+        """
+        Returns:
+             (cell-array bytearray, polygon-pointer-array bytearrays).
+        """
+        pointersToPolyBtr = bytearray()
+        cellArray = bytearray()
+        cellIndex = 0
+        for _, cell in enumerate(self.pointersToPolys):
+            zSliceCount = 0
+            for zSlice, zSliceData in enumerate(cell):
+                if zSliceData[0] != 0:
+                    pointersToPolyBtr.extend(np.uint32(zSliceData[1]))
+                    pointersToPolyBtr.extend(np.int16(zSliceData[0] - 1))
+                    pointersToPolyBtr.extend(np.int16(zSlice))
+                    zSliceCount += 1
+            cellArray.extend(np.uint32(cellIndex))
+            cellArray.extend(np.int32(zSliceCount))
+            cellIndex += zSliceCount
+
+        return pointersToPolyBtr, cellArray
```

### Comparing `vpt-1.0.1/src/vpt/update_vzg/polygons/packedpolygon.py` & `vpt-1.0.2/src/vpt/update_vzg/polygons/packedpolygon.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-import numpy as np
-from enum import Enum
-
-
-class LodLevel(Enum):
-    """Enum class of levels of details (lods) type depended on vertex count."""
-    Max = 0
-    Middle = 1
-    Min = 2
-    Count = 3
-
-
-class PackedPolygon:
-    """Abstract class for getting packed polygons."""
-    BASE_SIZE = {
-        LodLevel.Max: 12,
-        LodLevel.Middle: 8
-    }
-
-    BYTE_ON_POINT = {
-        LodLevel.Max: 3,
-        LodLevel.Middle: 2
-    }
-    DELTA_PACK_FACTOR = np.uint32(1 << 12)
-
-    CENTER_POINT_PACK_FACTOR = np.uint32(1 << 20)
-
-    def __init__(self, points):
-        self._points = points
-
-    @staticmethod
-    def _unsigned_float_to_n_bits(float_value, pack_factor):
-        return np.uint32(float_value * np.uint32(1 << pack_factor))
-
-    def _pack4_points(self, start_idx, support_point, scale_factor, points_count=4) -> bytearray:
-        packed_byte_array = bytearray()
-        offsets = np.zeros(4, dtype=np.uint32)
-
-        for point_idx in range(start_idx, start_idx + points_count):
-            delta_x = (self._points[point_idx][0] - support_point[0]) * scale_factor[0] * 0.5 + 0.5
-            delta_y = (self._points[point_idx][1] - support_point[1]) * scale_factor[1] * 0.5 + 0.5
-
-            delta_x = max(min(1 - 1 / (1 << 12), delta_x), 0)
-            delta_y = max(min(1 - 1 / (1 << 12), delta_y), 0)
-
-            offsets[point_idx - start_idx] = \
-                np.uint32(np.uint32(delta_x * (1 << 12)) << 12) + np.uint32(delta_y * (1 << 12))
-
-        packed_byte_array.extend(np.uint32((offsets[0] << 8) + (offsets[1] >> 16)))
-        packed_byte_array.extend(np.uint32((offsets[1] << 16) + (offsets[2] >> 8)))
-        packed_byte_array.extend(np.uint32((offsets[2] << 24) + offsets[3]))
-        return packed_byte_array
+import numpy as np
+from enum import Enum
+
+
+class LodLevel(Enum):
+    """Enum class of levels of details (lods) type depended on vertex count."""
+    Max = 0
+    Middle = 1
+    Min = 2
+    Count = 3
+
+
+class PackedPolygon:
+    """Abstract class for getting packed polygons."""
+    BASE_SIZE = {
+        LodLevel.Max: 12,
+        LodLevel.Middle: 8
+    }
+
+    BYTE_ON_POINT = {
+        LodLevel.Max: 3,
+        LodLevel.Middle: 2
+    }
+    DELTA_PACK_FACTOR = np.uint32(1 << 12)
+
+    CENTER_POINT_PACK_FACTOR = np.uint32(1 << 20)
+
+    def __init__(self, points):
+        self._points = points
+
+    @staticmethod
+    def _unsigned_float_to_n_bits(float_value, pack_factor):
+        return np.uint32(float_value * np.uint32(1 << pack_factor))
+
+    def _pack4_points(self, start_idx, support_point, scale_factor, points_count=4) -> bytearray:
+        packed_byte_array = bytearray()
+        offsets = np.zeros(4, dtype=np.uint32)
+
+        for point_idx in range(start_idx, start_idx + points_count):
+            delta_x = (self._points[point_idx][0] - support_point[0]) * scale_factor[0] * 0.5 + 0.5
+            delta_y = (self._points[point_idx][1] - support_point[1]) * scale_factor[1] * 0.5 + 0.5
+
+            delta_x = max(min(1 - 1 / (1 << 12), delta_x), 0)
+            delta_y = max(min(1 - 1 / (1 << 12), delta_y), 0)
+
+            offsets[point_idx - start_idx] = \
+                np.uint32(np.uint32(delta_x * (1 << 12)) << 12) + np.uint32(delta_y * (1 << 12))
+
+        packed_byte_array.extend(np.uint32((offsets[0] << 8) + (offsets[1] >> 16)))
+        packed_byte_array.extend(np.uint32((offsets[1] << 16) + (offsets[2] >> 8)))
+        packed_byte_array.extend(np.uint32((offsets[2] << 24) + offsets[3]))
+        return packed_byte_array
```

### Comparing `vpt-1.0.1/src/vpt/update_vzg/polygons/packedstarpolygon.py` & `vpt-1.0.2/src/vpt/update_vzg/polygons/packedstarpolygon.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,142 +1,142 @@
-from typing import Tuple
-import numpy as np
-
-from vpt.update_vzg.polygons.packedpolygon import PackedPolygon, LodLevel
-
-
-class PackedStarPolygon(PackedPolygon):
-    """Class for getting packed star polygon.
-
-    Packing information (B - byte, 1b - bit):
-    |1B|3B|20b|12b|20b|12b|12b|12b|..|12b|12b|..
-    |k |N | X |dX0| Y |dY0|dX1|dY1|..|dXk|dYk|..
-    Here:
-        k is the real number point of the polygon.
-        N is the number of the polygon.
-        X, Y are the coordinates of the first point of the polygon.
-        dX0, dY0 is the displacement from the center to the first polygon point.
-        dXk, dYk is the displacement from the center to the point k (k > 0).
-    """
-
-    LOD_POINTS = [
-        [17, 33, 57],
-        [8, 16, 32],
-        [0, 0, 0]
-    ]
-
-    def __init__(self, points, gridSize: Tuple[float, float], lodLevel=LodLevel.Max):
-        super().__init__(points)
-        self._gridSize = gridSize
-        self._lodLevel = lodLevel
-
-    def get_packed_bytes(self, cellId) -> Tuple[int, bytes]:
-        """Transfer star polygon into packed block.
-        Returns:
-             (poly size type index(0, 1, 2), packed block).
-        """
-        pointsCount = len(self._points)
-        packedPolyBtr = bytearray()
-
-        polyType, packedPointCount = self._define_packed_points(pointsCount)
-        packedPolyBtr.extend(np.uint32(
-            np.uint32(np.uint32(pointsCount - 1) << 24) + np.uint32(cellId)))
-
-        centerPoint = self._points.mean(0)
-
-        firstPointDeltaX = (self._points[0][0] - centerPoint[0]) * self._gridSize[0] * 0.5 + 0.5
-        firstPointDeltaY = (self._points[0][1] - centerPoint[1]) * self._gridSize[1] * 0.5 + 0.5
-
-        bitsCenterX = np.uint32(np.uint32(centerPoint[0] *
-                                          self.CENTER_POINT_PACK_FACTOR) << 12)
-        bitsFirstPointDeltaX = np.uint32(firstPointDeltaX * (1 << 12))
-        packedPolyBtr.extend(np.uint32(bitsCenterX + bitsFirstPointDeltaX))
-
-        bitsCenterY = np.uint32(np.uint32(centerPoint[1] *
-                                          self.CENTER_POINT_PACK_FACTOR) << 12)
-        bitsFirstPointDeltaY = np.uint32(firstPointDeltaY * (1 << 12))
-        packedPolyBtr.extend(np.uint32(bitsCenterY + bitsFirstPointDeltaY))
-
-        lastPointsCount = (pointsCount - 1) % 4
-        multipled4Points = pointsCount - 1 - lastPointsCount
-        for pointInd in range(1, multipled4Points, 4):
-            packedPolyBtr.extend(
-                self._pack4_points(pointInd, centerPoint, self._gridSize))
-
-        if lastPointsCount != 0:
-            packedPolyBtr.extend(self._pack4_points(
-                multipled4Points + 1, centerPoint, self._gridSize,
-                lastPointsCount))
-            multipled4Points += 4
-
-        for _ in range(multipled4Points, packedPointCount - 1, 4):
-            packedPolyBtr.extend(np.zeros(3, dtype=np.uint32))
-
-        return polyType, bytes(packedPolyBtr)
-
-    def _define_packed_points(self, pointsCount):
-        for i, threshold in enumerate(self.LOD_POINTS[self._lodLevel.value]):
-            if pointsCount <= threshold:
-                return i, threshold
-
-        return 0, 0
-
-    def get_packed_bytes_middle(self, cellId):
-        """Transfer middle-lod star polygon into packed block.
-        Returns:
-             (poly size type index(0, 1, 2), packed block).
-        """
-        pointsCount = len(self._points)
-        packedPolyBtr = bytearray()
-
-        packedPolyBtr.extend(np.uint32(
-            np.uint32(np.uint32(pointsCount - 1) << 24) + np.uint32(cellId)))
-
-        polyType, packedPointCount = self._define_packed_points(pointsCount)
-        centerPoint = self._points.mean(0)
-        packedPolyBtr.extend(
-            np.uint16(self._unsigned_float_to_n_bits(centerPoint[0], 16)))
-        packedPolyBtr.extend(
-            np.uint16(self._unsigned_float_to_n_bits(centerPoint[1], 16)))
-
-        blocks8Count = 0
-        for startPointIdx in range(0, pointsCount, 8):
-            pointDelta = pointsCount - startPointIdx
-            packSize = 8 if pointDelta > 8 else pointDelta
-            self._pack8_points(
-                startPointIdx, centerPoint, packedPolyBtr, packSize)
-            blocks8Count += 1
-
-        for _ in range(packedPointCount - blocks8Count * 8):
-            packedPolyBtr.extend(np.uint16(0))
-
-        return polyType, bytes(packedPolyBtr)
-
-    @staticmethod
-    def get_bytes_count(level: LodLevel, packSizeType) -> int:
-        """Returns Block bytes count depended on LodLevel and packSizeType.
-        Args:
-            level: LodLevel.
-            packSizeType: index (0, 1, 2) to get points count  in
-            LOD_POINTS[LodLevel].
-        Returns:
-            (int): Block bytes count.
-        """
-        packSize = PackedStarPolygon.LOD_POINTS[level.value][packSizeType]
-        if level == LodLevel.Max:
-            return PackedPolygon.BASE_SIZE[level] + \
-                   PackedPolygon.BYTE_ON_POINT[level] * (packSize - 1)
-        else:  # level == LodLevel.Middle
-            return PackedPolygon.BASE_SIZE[level] \
-                   + PackedPolygon.BYTE_ON_POINT[level] * packSize
-
-    def _pack8_points(self, startInd, centerPoint, packedPolyBtr,
-                      pointsCount=8):
-        offsets = np.zeros(8, dtype=np.uint32)
-        for pointIdx in range(pointsCount):
-            deltaX = (self._points[startInd + pointIdx][0] - centerPoint[0]) * self._gridSize[0] * 0.5 + 0.5
-            deltaY = (self._points[startInd + pointIdx][1] - centerPoint[1]) * self._gridSize[1] * 0.5 + 0.5
-            offsets[pointIdx] = np.uint32(np.uint32(deltaX * (1 << 8)) << 8) + np.uint32(deltaY * (1 << 8))
-
-        for i in range(4):
-            packedPolyBtr.extend(np.uint16(offsets[2 * i + 1]))
-            packedPolyBtr.extend(np.uint16(offsets[2 * i]))
+from typing import Tuple
+import numpy as np
+
+from vpt.update_vzg.polygons.packedpolygon import PackedPolygon, LodLevel
+
+
+class PackedStarPolygon(PackedPolygon):
+    """Class for getting packed star polygon.
+
+    Packing information (B - byte, 1b - bit):
+    |1B|3B|20b|12b|20b|12b|12b|12b|..|12b|12b|..
+    |k |N | X |dX0| Y |dY0|dX1|dY1|..|dXk|dYk|..
+    Here:
+        k is the real number point of the polygon.
+        N is the number of the polygon.
+        X, Y are the coordinates of the first point of the polygon.
+        dX0, dY0 is the displacement from the center to the first polygon point.
+        dXk, dYk is the displacement from the center to the point k (k > 0).
+    """
+
+    LOD_POINTS = [
+        [17, 33, 57],
+        [8, 16, 32],
+        [0, 0, 0]
+    ]
+
+    def __init__(self, points, gridSize: Tuple[float, float], lodLevel=LodLevel.Max):
+        super().__init__(points)
+        self._gridSize = gridSize
+        self._lodLevel = lodLevel
+
+    def get_packed_bytes(self, cellId) -> Tuple[int, bytes]:
+        """Transfer star polygon into packed block.
+        Returns:
+             (poly size type index(0, 1, 2), packed block).
+        """
+        pointsCount = len(self._points)
+        packedPolyBtr = bytearray()
+
+        polyType, packedPointCount = self._define_packed_points(pointsCount)
+        packedPolyBtr.extend(np.uint32(
+            np.uint32(np.uint32(pointsCount - 1) << 24) + np.uint32(cellId)))
+
+        centerPoint = self._points.mean(0)
+
+        firstPointDeltaX = (self._points[0][0] - centerPoint[0]) * self._gridSize[0] * 0.5 + 0.5
+        firstPointDeltaY = (self._points[0][1] - centerPoint[1]) * self._gridSize[1] * 0.5 + 0.5
+
+        bitsCenterX = np.uint32(np.uint32(centerPoint[0] *
+                                          self.CENTER_POINT_PACK_FACTOR) << 12)
+        bitsFirstPointDeltaX = np.uint32(firstPointDeltaX * (1 << 12))
+        packedPolyBtr.extend(np.uint32(bitsCenterX + bitsFirstPointDeltaX))
+
+        bitsCenterY = np.uint32(np.uint32(centerPoint[1] *
+                                          self.CENTER_POINT_PACK_FACTOR) << 12)
+        bitsFirstPointDeltaY = np.uint32(firstPointDeltaY * (1 << 12))
+        packedPolyBtr.extend(np.uint32(bitsCenterY + bitsFirstPointDeltaY))
+
+        lastPointsCount = (pointsCount - 1) % 4
+        multipled4Points = pointsCount - 1 - lastPointsCount
+        for pointInd in range(1, multipled4Points, 4):
+            packedPolyBtr.extend(
+                self._pack4_points(pointInd, centerPoint, self._gridSize))
+
+        if lastPointsCount != 0:
+            packedPolyBtr.extend(self._pack4_points(
+                multipled4Points + 1, centerPoint, self._gridSize,
+                lastPointsCount))
+            multipled4Points += 4
+
+        for _ in range(multipled4Points, packedPointCount - 1, 4):
+            packedPolyBtr.extend(np.zeros(3, dtype=np.uint32))
+
+        return polyType, bytes(packedPolyBtr)
+
+    def _define_packed_points(self, pointsCount):
+        for i, threshold in enumerate(self.LOD_POINTS[self._lodLevel.value]):
+            if pointsCount <= threshold:
+                return i, threshold
+
+        return 0, 0
+
+    def get_packed_bytes_middle(self, cellId):
+        """Transfer middle-lod star polygon into packed block.
+        Returns:
+             (poly size type index(0, 1, 2), packed block).
+        """
+        pointsCount = len(self._points)
+        packedPolyBtr = bytearray()
+
+        packedPolyBtr.extend(np.uint32(
+            np.uint32(np.uint32(pointsCount - 1) << 24) + np.uint32(cellId)))
+
+        polyType, packedPointCount = self._define_packed_points(pointsCount)
+        centerPoint = self._points.mean(0)
+        packedPolyBtr.extend(
+            np.uint16(self._unsigned_float_to_n_bits(centerPoint[0], 16)))
+        packedPolyBtr.extend(
+            np.uint16(self._unsigned_float_to_n_bits(centerPoint[1], 16)))
+
+        blocks8Count = 0
+        for startPointIdx in range(0, pointsCount, 8):
+            pointDelta = pointsCount - startPointIdx
+            packSize = 8 if pointDelta > 8 else pointDelta
+            self._pack8_points(
+                startPointIdx, centerPoint, packedPolyBtr, packSize)
+            blocks8Count += 1
+
+        for _ in range(packedPointCount - blocks8Count * 8):
+            packedPolyBtr.extend(np.uint16(0))
+
+        return polyType, bytes(packedPolyBtr)
+
+    @staticmethod
+    def get_bytes_count(level: LodLevel, packSizeType) -> int:
+        """Returns Block bytes count depended on LodLevel and packSizeType.
+        Args:
+            level: LodLevel.
+            packSizeType: index (0, 1, 2) to get points count  in
+            LOD_POINTS[LodLevel].
+        Returns:
+            (int): Block bytes count.
+        """
+        packSize = PackedStarPolygon.LOD_POINTS[level.value][packSizeType]
+        if level == LodLevel.Max:
+            return PackedPolygon.BASE_SIZE[level] + \
+                   PackedPolygon.BYTE_ON_POINT[level] * (packSize - 1)
+        else:  # level == LodLevel.Middle
+            return PackedPolygon.BASE_SIZE[level] \
+                   + PackedPolygon.BYTE_ON_POINT[level] * packSize
+
+    def _pack8_points(self, startInd, centerPoint, packedPolyBtr,
+                      pointsCount=8):
+        offsets = np.zeros(8, dtype=np.uint32)
+        for pointIdx in range(pointsCount):
+            deltaX = (self._points[startInd + pointIdx][0] - centerPoint[0]) * self._gridSize[0] * 0.5 + 0.5
+            deltaY = (self._points[startInd + pointIdx][1] - centerPoint[1]) * self._gridSize[1] * 0.5 + 0.5
+            offsets[pointIdx] = np.uint32(np.uint32(deltaX * (1 << 8)) << 8) + np.uint32(deltaY * (1 << 8))
+
+        for i in range(4):
+            packedPolyBtr.extend(np.uint16(offsets[2 * i + 1]))
+            packedPolyBtr.extend(np.uint16(offsets[2 * i]))
```

### Comparing `vpt-1.0.1/src/vpt/update_vzg/polygons/poly_partition.py` & `vpt-1.0.2/src/vpt/update_vzg/polygons/poly_partition.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,259 +1,259 @@
-import numpy as np
-
-from vpt.update_vzg.polygons.polystructers import PointsIndices, IndexedPolygon
-from vpt.update_vzg.polygons.vector_operations import pseudo_scalar, point_line_side, \
-    ray_segment_intersect, dot_2d, find_bisector, segment_outline_intersect, point_in_sector
-
-
-class PolyPartition:
-    """Class for part original polygon into fan polygons. """
-    def __init__(self, originPoints: np.array):
-        """Args:
-            originPoints: List[np.array] - list of 2-dims (numpy array) points
-        """
-        self._originPoints = originPoints.copy()
-        self._originPointsLen = len(self._originPoints)
-
-    def _find_concave_point(
-            self, pointsIdx: list, startPointIdx=0) -> list:
-
-        origins = self._originPoints
-        concavePointsIdxList = []
-        n = len(pointsIdx)
-        pointA = origins[pointsIdx[(n - 1 + startPointIdx) % n]]
-        for pointIdx in range(n):
-            pointB = origins[pointsIdx[(pointIdx + startPointIdx) % n]]
-            pointC = origins[pointsIdx[(pointIdx + startPointIdx + 1) % n]]
-
-            # check for "bad" (concave) point
-            if pseudo_scalar(pointA - pointB, pointC - pointB) > 0:
-                concavePointsIdxList.append(
-                    (pointIdx + startPointIdx) % n)
-
-            pointA = pointB
-
-        return concavePointsIdxList
-
-    def get_origins(self):
-        """Returns original polygon coordinates."""
-        return self._originPoints
-
-    def _find_intersect_segment(self, pointsIdx, supportPointIdx, ABCBisector):
-        n = len(pointsIdx)
-        B = self._originPoints[pointsIdx[supportPointIdx]]
-        BB = B + ABCBisector
-        minDistance = float('inf')
-        segmentAIdx, segmentBIdx = -1, -1
-        minDistPointIdx = -1
-        minDistBetweenPoints = 10e10
-        leftPoint = self._originPoints[pointsIdx[(supportPointIdx - 1) % n]]
-        rightPoint = self._originPoints[pointsIdx[(supportPointIdx + 1) % n]]
-        for i in range(n - 2):
-            indE = (supportPointIdx + i + 1) % n
-            indF = (supportPointIdx + i + 2) % n
-            E = self._originPoints[pointsIdx[indE]]
-            F = self._originPoints[pointsIdx[indF]]
-            lineSideLeftPoint = point_line_side(F, B, leftPoint)
-            lineSideRightPoint = point_line_side(F, B, rightPoint)
-
-            if (not (lineSideLeftPoint >= 0 and lineSideRightPoint <= 0)) \
-                    and i != n - 3:
-                distBetweenPoints = np.linalg.norm(B - F)
-                if minDistBetweenPoints > distBetweenPoints:
-                    minDistBetweenPoints = distBetweenPoints
-                    minDistPointIdx = indF
-
-            if point_line_side(E, B, BB) <= 0 and \
-                    point_line_side(F, B, BB) >= 0:
-                p = ray_segment_intersect(B, ABCBisector, E, F)
-                vp = p - B
-                if dot_2d(vp, ABCBisector) > 0:
-                    dist2 = dot_2d(vp, vp)
-                    if minDistance > dist2:
-                        minDistance = dist2
-                        segmentAIdx = indF
-                        segmentBIdx = indE
-
-        return segmentAIdx, segmentBIdx, minDistPointIdx
-
-    def _cut_from_concave_point(self, pointsIndices: PointsIndices, ind: int):
-        pointsIdx = pointsIndices.polyIndices
-        origins = self._originPoints
-        n = len(pointsIdx)
-        pointA = origins[pointsIdx[(ind - 1) % n]]
-        pointB = origins[pointsIdx[ind]]
-        pointC = origins[pointsIdx[(ind + 1) % n]]
-        ABVec = pointB - pointA
-        CBVec = pointB - pointC
-
-        # find the bisector
-        ABCBisector = find_bisector(ABVec, CBVec)
-
-        # find intersects segment
-        segmentAIdx, segmentBIdx, minDistPointIdx = \
-            self._find_intersect_segment(pointsIdx, ind, ABCBisector)
-        if segmentAIdx < 0 or segmentBIdx < 0 or minDistPointIdx < 0:
-            raise IndexError
-
-        intersectAVec = origins[pointsIdx[segmentAIdx]] - pointB
-        if point_in_sector(intersectAVec, CBVec, ABVec) \
-                and not segment_outline_intersect(origins, ind, segmentAIdx, pointsIdx, False):
-
-            # create new polygons
-            leftPoly, rightPoly = \
-                pointsIndices.polygon_partition(ind, segmentAIdx)
-        else:
-            intersectBVec = origins[pointsIdx[segmentBIdx]] - pointB
-            if point_in_sector(intersectBVec, CBVec, ABVec) \
-                    and not segment_outline_intersect(origins, ind, segmentBIdx, pointsIdx):
-                # create new polygons
-                leftPoly, rightPoly = \
-                    pointsIndices.polygon_partition(ind, segmentBIdx)
-            else:
-                # create new polygons
-                leftPoly, rightPoly = \
-                    pointsIndices.polygon_partition(ind, minDistPointIdx)
-
-        return leftPoly, rightPoly
-
-    def _get_single_result_from_list(self, pointsIdx: PointsIndices):
-        concavePointsIdx = self._find_concave_point(pointsIdx.polyIndices)
-        if len(concavePointsIdx) == 0:
-            return concavePointsIdx, IndexedPolygon(
-                'convex', pointsIdx.polyIndices, pointsIdx.includePoints, -1)
-
-        if len(concavePointsIdx) == 1:
-            return concavePointsIdx, IndexedPolygon(
-                'fan', pointsIdx.polyIndices, pointsIdx.includePoints,
-                concavePointsIdx[0])
-
-        for ci in concavePointsIdx:
-            if self._is_all_edges_visible(
-                    self._originPoints[pointsIdx.polyIndices[ci]],
-                    pointsIdx.polyIndices):
-                return concavePointsIdx, IndexedPolygon(
-                    'fan', pointsIdx.polyIndices, pointsIdx.includePoints, ci)
-
-        return concavePointsIdx, None
-
-    def run_partition(self, out):
-        """Runs full pipeline of polygon partition, including split polygon
-        into fans polygons, and merge them into bigger fan polygons,
-        if it is possible.
-        """
-        pointsIndices = PointsIndices(list(range(len(self._originPoints))))
-        self.split_polygon(pointsIndices, out)
-        self.merge_postproces(out)
-
-    def split_polygon(self, pointsIdx: PointsIndices, out, depth=0):
-        """Recursive splits polygons while they are not fan polygons
-        Args:
-            pointsIdx: indices in self._originPoints,
-            of current considered polygon
-            out: list of already parted fan polygons (only indices)
-            depth: recursion depth.
-        """
-        if depth > 20:  # we get stuck because of wrong origin poly
-            raise TimeoutError
-
-        (concavePoints, one) = self._get_single_result_from_list(pointsIdx)
-
-        if one is not None:
-            out.append(one)
-        else:
-            cidx = concavePoints[len(concavePoints) // 2]
-            (l, r) = self._cut_from_concave_point(pointsIdx, cidx)
-            self.split_polygon(l, out, depth + 1)
-            self.split_polygon(r, out, depth + 1)
-
-    def _merge_results(self, p1, p2, i1, i2):
-        polyIndices = p1.polyIndices[:i1] + p2.polyIndices[i2 + 1:] \
-                      + p2.polyIndices[:i2] + p1.polyIndices[i1 + 1:]
-
-        includeIndices1 = p1.includeIndices.copy()
-        includeIndices2 = p2.includeIndices.copy()
-        includeIndices1[i1] = True
-        includeIndices2[i2] = True
-
-        includePoints = includeIndices1[:i1] + includeIndices2[i2 + 1:] + includeIndices2[:i2] + includeIndices1[i1 + 1:]
-
-        pointsIdx = PointsIndices(polyIndices, includePoints)
-
-        if p1.type == "convex" and p2.type == "convex":
-            return IndexedPolygon(
-                'fan', pointsIdx.polyIndices, pointsIdx.includePoints, i1)
-        (_, ret) = self._get_single_result_from_list(pointsIdx)
-        return ret
-
-    def merge_postproces(self, results: list):
-        """Merge fan polygons into bigger fan polygons if it is possible."""
-        concavePoints = self._find_concave_point(
-            list(range(len(self._originPoints))))
-
-        for cindex in concavePoints:
-            candidates = []
-            for rindex, res in enumerate(results):
-                for i, pIdx in enumerate(res.polyIndices):
-                    if cindex == pIdx:
-                        candidates.append((rindex, i))
-                        break
-            merged = []
-            for fi in range(len(candidates) - 1):
-                fpointsIdx = results[candidates[fi][0]].polyIndices
-                findex = candidates[fi][1]
-                for si in range(fi + 1, len(candidates)):
-                    if candidates[si][0] in merged or\
-                            candidates[fi][0] in merged:
-                        continue
-
-                    spointsIdx = results[candidates[si][0]].polyIndices
-                    sindex = candidates[si][1]
-                    mresult = None
-                    if fpointsIdx[(findex - 1) % len(fpointsIdx)] == \
-                            spointsIdx[(sindex + 1) % len(spointsIdx)]:
-                        mresult = self._merge_results(
-                            results[candidates[fi][0]],
-                            results[candidates[si][0]],
-                            (findex - 1) % len(fpointsIdx),
-                            sindex)
-
-                    elif fpointsIdx[(findex + 1) % len(fpointsIdx)] == \
-                            spointsIdx[(sindex - 1) % len(spointsIdx)]:
-
-                        mresult = self._merge_results(
-                            results[candidates[fi][0]],
-                            results[candidates[si][0]],
-                            findex,
-                            (sindex - 1) % len(spointsIdx))
-                    if mresult is not None:
-                        merged.append(candidates[fi][0])
-                        merged.append(candidates[si][0])
-                        results.append(mresult)
-
-            # clean merged
-            for index in sorted(merged, reverse=True):
-                del results[index]
-
-    @staticmethod
-    def _get_bbox(points):
-        return [np.min(points, axis=0), np.max(points, axis=0)]
-
-    def _is_all_edges_visible(self, point, pointsIdx) -> bool:
-        pointsLen = len(pointsIdx)
-        a = self._originPoints[pointsIdx[len(pointsIdx) - 1]]
-        for i in range(pointsLen):
-            b = self._originPoints[pointsIdx[i]]
-            s = point_line_side(point, a, b)
-            if s < 0:
-                return False
-            a = b
-        return True
-
-    def _get_star_center(self, pointsIdx):
-        bbox = PolyPartition._get_bbox(list(self._originPoints[i] for i in
-                                            pointsIdx))
-        center = (bbox[0] + bbox[1]) * 0.5
-        n = len(pointsIdx)
-        if n < 4 or self._is_all_edges_visible(center, pointsIdx):
-            return center
-        return None
+import numpy as np
+
+from vpt.update_vzg.polygons.polystructers import PointsIndices, IndexedPolygon
+from vpt.update_vzg.polygons.vector_operations import pseudo_scalar, point_line_side, \
+    ray_segment_intersect, dot_2d, find_bisector, segment_outline_intersect, point_in_sector
+
+
+class PolyPartition:
+    """Class for part original polygon into fan polygons. """
+    def __init__(self, originPoints: np.array):
+        """Args:
+            originPoints: List[np.array] - list of 2-dims (numpy array) points
+        """
+        self._originPoints = originPoints.copy()
+        self._originPointsLen = len(self._originPoints)
+
+    def _find_concave_point(
+            self, pointsIdx: list, startPointIdx=0) -> list:
+
+        origins = self._originPoints
+        concavePointsIdxList = []
+        n = len(pointsIdx)
+        pointA = origins[pointsIdx[(n - 1 + startPointIdx) % n]]
+        for pointIdx in range(n):
+            pointB = origins[pointsIdx[(pointIdx + startPointIdx) % n]]
+            pointC = origins[pointsIdx[(pointIdx + startPointIdx + 1) % n]]
+
+            # check for "bad" (concave) point
+            if pseudo_scalar(pointA - pointB, pointC - pointB) > 0:
+                concavePointsIdxList.append(
+                    (pointIdx + startPointIdx) % n)
+
+            pointA = pointB
+
+        return concavePointsIdxList
+
+    def get_origins(self):
+        """Returns original polygon coordinates."""
+        return self._originPoints
+
+    def _find_intersect_segment(self, pointsIdx, supportPointIdx, ABCBisector):
+        n = len(pointsIdx)
+        B = self._originPoints[pointsIdx[supportPointIdx]]
+        BB = B + ABCBisector
+        minDistance = float('inf')
+        segmentAIdx, segmentBIdx = -1, -1
+        minDistPointIdx = -1
+        minDistBetweenPoints = 10e10
+        leftPoint = self._originPoints[pointsIdx[(supportPointIdx - 1) % n]]
+        rightPoint = self._originPoints[pointsIdx[(supportPointIdx + 1) % n]]
+        for i in range(n - 2):
+            indE = (supportPointIdx + i + 1) % n
+            indF = (supportPointIdx + i + 2) % n
+            E = self._originPoints[pointsIdx[indE]]
+            F = self._originPoints[pointsIdx[indF]]
+            lineSideLeftPoint = point_line_side(F, B, leftPoint)
+            lineSideRightPoint = point_line_side(F, B, rightPoint)
+
+            if (not (lineSideLeftPoint >= 0 and lineSideRightPoint <= 0)) \
+                    and i != n - 3:
+                distBetweenPoints = np.linalg.norm(B - F)
+                if minDistBetweenPoints > distBetweenPoints:
+                    minDistBetweenPoints = distBetweenPoints
+                    minDistPointIdx = indF
+
+            if point_line_side(E, B, BB) <= 0 and \
+                    point_line_side(F, B, BB) >= 0:
+                p = ray_segment_intersect(B, ABCBisector, E, F)
+                vp = p - B
+                if dot_2d(vp, ABCBisector) > 0:
+                    dist2 = dot_2d(vp, vp)
+                    if minDistance > dist2:
+                        minDistance = dist2
+                        segmentAIdx = indF
+                        segmentBIdx = indE
+
+        return segmentAIdx, segmentBIdx, minDistPointIdx
+
+    def _cut_from_concave_point(self, pointsIndices: PointsIndices, ind: int):
+        pointsIdx = pointsIndices.polyIndices
+        origins = self._originPoints
+        n = len(pointsIdx)
+        pointA = origins[pointsIdx[(ind - 1) % n]]
+        pointB = origins[pointsIdx[ind]]
+        pointC = origins[pointsIdx[(ind + 1) % n]]
+        ABVec = pointB - pointA
+        CBVec = pointB - pointC
+
+        # find the bisector
+        ABCBisector = find_bisector(ABVec, CBVec)
+
+        # find intersects segment
+        segmentAIdx, segmentBIdx, minDistPointIdx = \
+            self._find_intersect_segment(pointsIdx, ind, ABCBisector)
+        if segmentAIdx < 0 or segmentBIdx < 0 or minDistPointIdx < 0:
+            raise IndexError
+
+        intersectAVec = origins[pointsIdx[segmentAIdx]] - pointB
+        if point_in_sector(intersectAVec, CBVec, ABVec) \
+                and not segment_outline_intersect(origins, ind, segmentAIdx, pointsIdx, False):
+
+            # create new polygons
+            leftPoly, rightPoly = \
+                pointsIndices.polygon_partition(ind, segmentAIdx)
+        else:
+            intersectBVec = origins[pointsIdx[segmentBIdx]] - pointB
+            if point_in_sector(intersectBVec, CBVec, ABVec) \
+                    and not segment_outline_intersect(origins, ind, segmentBIdx, pointsIdx):
+                # create new polygons
+                leftPoly, rightPoly = \
+                    pointsIndices.polygon_partition(ind, segmentBIdx)
+            else:
+                # create new polygons
+                leftPoly, rightPoly = \
+                    pointsIndices.polygon_partition(ind, minDistPointIdx)
+
+        return leftPoly, rightPoly
+
+    def _get_single_result_from_list(self, pointsIdx: PointsIndices):
+        concavePointsIdx = self._find_concave_point(pointsIdx.polyIndices)
+        if len(concavePointsIdx) == 0:
+            return concavePointsIdx, IndexedPolygon(
+                'convex', pointsIdx.polyIndices, pointsIdx.includePoints, -1)
+
+        if len(concavePointsIdx) == 1:
+            return concavePointsIdx, IndexedPolygon(
+                'fan', pointsIdx.polyIndices, pointsIdx.includePoints,
+                concavePointsIdx[0])
+
+        for ci in concavePointsIdx:
+            if self._is_all_edges_visible(
+                    self._originPoints[pointsIdx.polyIndices[ci]],
+                    pointsIdx.polyIndices):
+                return concavePointsIdx, IndexedPolygon(
+                    'fan', pointsIdx.polyIndices, pointsIdx.includePoints, ci)
+
+        return concavePointsIdx, None
+
+    def run_partition(self, out):
+        """Runs full pipeline of polygon partition, including split polygon
+        into fans polygons, and merge them into bigger fan polygons,
+        if it is possible.
+        """
+        pointsIndices = PointsIndices(list(range(len(self._originPoints))))
+        self.split_polygon(pointsIndices, out)
+        self.merge_postproces(out)
+
+    def split_polygon(self, pointsIdx: PointsIndices, out, depth=0):
+        """Recursive splits polygons while they are not fan polygons
+        Args:
+            pointsIdx: indices in self._originPoints,
+            of current considered polygon
+            out: list of already parted fan polygons (only indices)
+            depth: recursion depth.
+        """
+        if depth > 20:  # we get stuck because of wrong origin poly
+            raise TimeoutError
+
+        (concavePoints, one) = self._get_single_result_from_list(pointsIdx)
+
+        if one is not None:
+            out.append(one)
+        else:
+            cidx = concavePoints[len(concavePoints) // 2]
+            (l, r) = self._cut_from_concave_point(pointsIdx, cidx)
+            self.split_polygon(l, out, depth + 1)
+            self.split_polygon(r, out, depth + 1)
+
+    def _merge_results(self, p1, p2, i1, i2):
+        polyIndices = p1.polyIndices[:i1] + p2.polyIndices[i2 + 1:] \
+                      + p2.polyIndices[:i2] + p1.polyIndices[i1 + 1:]
+
+        includeIndices1 = p1.includeIndices.copy()
+        includeIndices2 = p2.includeIndices.copy()
+        includeIndices1[i1] = True
+        includeIndices2[i2] = True
+
+        includePoints = includeIndices1[:i1] + includeIndices2[i2 + 1:] + includeIndices2[:i2] + includeIndices1[i1 + 1:]
+
+        pointsIdx = PointsIndices(polyIndices, includePoints)
+
+        if p1.type == "convex" and p2.type == "convex":
+            return IndexedPolygon(
+                'fan', pointsIdx.polyIndices, pointsIdx.includePoints, i1)
+        (_, ret) = self._get_single_result_from_list(pointsIdx)
+        return ret
+
+    def merge_postproces(self, results: list):
+        """Merge fan polygons into bigger fan polygons if it is possible."""
+        concavePoints = self._find_concave_point(
+            list(range(len(self._originPoints))))
+
+        for cindex in concavePoints:
+            candidates = []
+            for rindex, res in enumerate(results):
+                for i, pIdx in enumerate(res.polyIndices):
+                    if cindex == pIdx:
+                        candidates.append((rindex, i))
+                        break
+            merged = []
+            for fi in range(len(candidates) - 1):
+                fpointsIdx = results[candidates[fi][0]].polyIndices
+                findex = candidates[fi][1]
+                for si in range(fi + 1, len(candidates)):
+                    if candidates[si][0] in merged or\
+                            candidates[fi][0] in merged:
+                        continue
+
+                    spointsIdx = results[candidates[si][0]].polyIndices
+                    sindex = candidates[si][1]
+                    mresult = None
+                    if fpointsIdx[(findex - 1) % len(fpointsIdx)] == \
+                            spointsIdx[(sindex + 1) % len(spointsIdx)]:
+                        mresult = self._merge_results(
+                            results[candidates[fi][0]],
+                            results[candidates[si][0]],
+                            (findex - 1) % len(fpointsIdx),
+                            sindex)
+
+                    elif fpointsIdx[(findex + 1) % len(fpointsIdx)] == \
+                            spointsIdx[(sindex - 1) % len(spointsIdx)]:
+
+                        mresult = self._merge_results(
+                            results[candidates[fi][0]],
+                            results[candidates[si][0]],
+                            findex,
+                            (sindex - 1) % len(spointsIdx))
+                    if mresult is not None:
+                        merged.append(candidates[fi][0])
+                        merged.append(candidates[si][0])
+                        results.append(mresult)
+
+            # clean merged
+            for index in sorted(merged, reverse=True):
+                del results[index]
+
+    @staticmethod
+    def _get_bbox(points):
+        return [np.min(points, axis=0), np.max(points, axis=0)]
+
+    def _is_all_edges_visible(self, point, pointsIdx) -> bool:
+        pointsLen = len(pointsIdx)
+        a = self._originPoints[pointsIdx[len(pointsIdx) - 1]]
+        for i in range(pointsLen):
+            b = self._originPoints[pointsIdx[i]]
+            s = point_line_side(point, a, b)
+            if s < 0:
+                return False
+            a = b
+        return True
+
+    def _get_star_center(self, pointsIdx):
+        bbox = PolyPartition._get_bbox(list(self._originPoints[i] for i in
+                                            pointsIdx))
+        center = (bbox[0] + bbox[1]) * 0.5
+        n = len(pointsIdx)
+        if n < 4 or self._is_all_edges_visible(center, pointsIdx):
+            return center
+        return None
```

### Comparing `vpt-1.0.1/src/vpt/update_vzg/polygons/polystructers.py` & `vpt-1.0.2/src/vpt/update_vzg/polygons/polystructers.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,53 +1,53 @@
-from typing import Tuple
-from collections import namedtuple
-
-IndexedPolygon = namedtuple(
-    'IndexedPolygon', 'type polyIndices includeIndices ind')
-
-
-class PointsIndices:
-    """Class for storing list of indices of original poly, that represent
-    some parted polygon."""
-
-    def __init__(self, polyIndices, includePoints=None):
-        self.polyIndices = polyIndices
-        if includePoints is not None:
-            self.includePoints = includePoints
-        else:
-            self.includePoints = [True] * len(polyIndices)
-
-    def polygon_partition(self, startIdx, endIdx) -> Tuple['PointsIndices', 'PointsIndices']:
-        """Parts this polygon into 2 new polygons.
-        Args:
-            startIdx: index in this polygon that will be 0-index in the
-            left new polygon.
-            endIdx: index in this polygon that will be the last index in the
-            left new polygon.
-        Returns:
-             (left new polygon, right new polygon).
-        """
-        leftPolyIndices = []
-        rightPolyIndices = []
-
-        leftPolyIncludes = []
-        rightPolyIncludes = []
-
-        n = len(self.polyIndices)
-        idx = startIdx
-        while idx != endIdx:
-            rightPolyIndices.append(self.polyIndices[idx])
-            rightPolyIncludes.append(self.includePoints[idx])
-            idx = (idx + 1) % n
-        rightPolyIndices.append(self.polyIndices[endIdx])
-        rightPolyIncludes.append(False)
-
-        idx = endIdx
-        while idx != startIdx:
-            leftPolyIndices.append(self.polyIndices[idx])
-            leftPolyIncludes.append(self.includePoints[idx])
-            idx = (idx + 1) % n
-        leftPolyIndices.append(self.polyIndices[startIdx])
-        leftPolyIncludes.append(False)
-
-        return PointsIndices(leftPolyIndices, leftPolyIncludes), \
-               PointsIndices(rightPolyIndices, rightPolyIncludes) # noqa
+from typing import Tuple
+from collections import namedtuple
+
+IndexedPolygon = namedtuple(
+    'IndexedPolygon', 'type polyIndices includeIndices ind')
+
+
+class PointsIndices:
+    """Class for storing list of indices of original poly, that represent
+    some parted polygon."""
+
+    def __init__(self, polyIndices, includePoints=None):
+        self.polyIndices = polyIndices
+        if includePoints is not None:
+            self.includePoints = includePoints
+        else:
+            self.includePoints = [True] * len(polyIndices)
+
+    def polygon_partition(self, startIdx, endIdx) -> Tuple['PointsIndices', 'PointsIndices']:
+        """Parts this polygon into 2 new polygons.
+        Args:
+            startIdx: index in this polygon that will be 0-index in the
+            left new polygon.
+            endIdx: index in this polygon that will be the last index in the
+            left new polygon.
+        Returns:
+             (left new polygon, right new polygon).
+        """
+        leftPolyIndices = []
+        rightPolyIndices = []
+
+        leftPolyIncludes = []
+        rightPolyIncludes = []
+
+        n = len(self.polyIndices)
+        idx = startIdx
+        while idx != endIdx:
+            rightPolyIndices.append(self.polyIndices[idx])
+            rightPolyIncludes.append(self.includePoints[idx])
+            idx = (idx + 1) % n
+        rightPolyIndices.append(self.polyIndices[endIdx])
+        rightPolyIncludes.append(False)
+
+        idx = endIdx
+        while idx != startIdx:
+            leftPolyIndices.append(self.polyIndices[idx])
+            leftPolyIncludes.append(self.includePoints[idx])
+            idx = (idx + 1) % n
+        leftPolyIndices.append(self.polyIndices[startIdx])
+        leftPolyIncludes.append(False)
+
+        return PointsIndices(leftPolyIndices, leftPolyIncludes), \
+               PointsIndices(rightPolyIndices, rightPolyIncludes) # noqa
```

### Comparing `vpt-1.0.1/src/vpt/utils/cellsreader.py` & `vpt-1.0.2/src/vpt/utils/cellsreader.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,113 +1,113 @@
-from abc import ABC, abstractmethod
-import math
-from typing import List
-
-import numpy as np
-from geopandas import GeoDataFrame, gpd
-
-from vpt.filesystem import vzg_open
-from vpt.utils.raw_cell import Feature
-
-
-class CellsReader(ABC):
-    @abstractmethod
-    def get_fovs_count(self):
-        pass
-
-    @abstractmethod
-    def read_fov(self, fov: int) -> List[Feature]:
-        pass
-
-    @abstractmethod
-    def get_z_planes_count(self) -> int:
-        pass
-
-    @abstractmethod
-    def get_z_levels(self) -> np.ndarray:
-        pass
-
-
-class CellsGeoReader(CellsReader):
-    CELLS_PER_FOV = 10000
-
-    def __init__(self, data: GeoDataFrame):
-        data = data.sort_values(by=['EntityID'])
-        self._data = data
-
-        polyInCellCont = list(data['EntityID'].value_counts().sort_index())
-
-        prevFovIdx = 0
-        fovStartIdxList = [prevFovIdx]
-        i = 0
-        n = len(polyInCellCont)
-        while i < n:
-            prevFovIdx += sum(polyInCellCont[i:  min(n, i + self.CELLS_PER_FOV)])
-            fovStartIdxList.append(prevFovIdx)
-            i += self.CELLS_PER_FOV
-
-        self._fovsStartIdx = fovStartIdxList
-        self._nameList = data['EntityID'].unique()
-
-        zLevels = data['ZLevel'].unique()
-        zLevels.sort()
-        self._zLevelsDiffer = np.diff(zLevels, prepend=0)
-
-        self._zPlanesCount = self._zPlanesCount = 0 if len(data['ZIndex']) == 0 else data['ZIndex'].max() + 1
-
-        self._cellsCount = len(self._nameList)
-        self._fovsCount = int(math.ceil(self._cellsCount / self.CELLS_PER_FOV))
-
-    def get_z_levels(self) -> np.ndarray:
-        return self._zLevelsDiffer
-
-    def get_fovs_count(self):
-        return self._fovsCount
-
-    def read_fov(self, fov: int) -> List[Feature]:
-        rawCellsList = []
-
-        polyList = [None] * self._zPlanesCount
-        prevEntityIdx = self._data.iloc[self._fovsStartIdx[fov]]['EntityID']
-        for rowPolyIdx in range(self._fovsStartIdx[fov], self._fovsStartIdx[fov + 1]):
-            rowPoly = self._data.iloc[rowPolyIdx]
-
-            entityIdx = rowPoly['EntityID']
-            if prevEntityIdx != entityIdx:
-                rawCellsList.append(Feature(str(prevEntityIdx), polyList))
-                prevEntityIdx = entityIdx
-                polyList = [None] * self._zPlanesCount
-
-            polyGeometry = rowPoly['Geometry']
-            if polyGeometry is not None:
-                polyList[rowPoly['ZIndex']] = polyGeometry
-            continue
-
-        rawCellsList.append(Feature(str(prevEntityIdx), polyList))  # last cell
-        return rawCellsList
-
-    def read(self):
-        features = []
-
-        for fovIndex in range(self.get_fovs_count()):
-            features.extend(self.read_fov(fovIndex))
-
-        return features
-
-    def get_z_planes_count(self) -> int:
-        return self._zPlanesCount
-
-
-def cell_reader_factory(pathToFile) -> CellsReader:
-    if pathToFile.endswith('.parquet'):
-        with vzg_open(pathToFile, 'rb') as f:
-            data: GeoDataFrame = gpd.read_parquet(f)
-        return CellsGeoReader(data)
-
-    elif pathToFile.endswith('.geojson'):
-        with vzg_open(pathToFile, 'rb') as f:
-            data: GeoDataFrame = gpd.read_file(f)
-        data = data.rename(columns={'geometry': 'Geometry'})
-        return CellsGeoReader(data)
-
-    else:
-        raise ValueError("Input geometry has an unsupported file extension")
+from abc import ABC, abstractmethod
+import math
+from typing import List
+
+import numpy as np
+from geopandas import GeoDataFrame, gpd
+
+from vpt.filesystem import vzg_open
+from vpt.utils.raw_cell import Feature
+
+
+class CellsReader(ABC):
+    @abstractmethod
+    def get_fovs_count(self):
+        pass
+
+    @abstractmethod
+    def read_fov(self, fov: int) -> List[Feature]:
+        pass
+
+    @abstractmethod
+    def get_z_planes_count(self) -> int:
+        pass
+
+    @abstractmethod
+    def get_z_levels(self) -> np.ndarray:
+        pass
+
+
+class CellsGeoReader(CellsReader):
+    CELLS_PER_FOV = 10000
+
+    def __init__(self, data: GeoDataFrame):
+        data = data.sort_values(by=['EntityID'])
+        self._data = data
+
+        polyInCellCont = list(data['EntityID'].value_counts().sort_index())
+
+        prevFovIdx = 0
+        fovStartIdxList = [prevFovIdx]
+        i = 0
+        n = len(polyInCellCont)
+        while i < n:
+            prevFovIdx += sum(polyInCellCont[i:  min(n, i + self.CELLS_PER_FOV)])
+            fovStartIdxList.append(prevFovIdx)
+            i += self.CELLS_PER_FOV
+
+        self._fovsStartIdx = fovStartIdxList
+        self._nameList = data['EntityID'].unique()
+
+        zLevels = data['ZLevel'].unique()
+        zLevels.sort()
+        self._zLevelsDiffer = np.diff(zLevels, prepend=0)
+
+        self._zPlanesCount = self._zPlanesCount = 0 if len(data['ZIndex']) == 0 else data['ZIndex'].max() + 1
+
+        self._cellsCount = len(self._nameList)
+        self._fovsCount = int(math.ceil(self._cellsCount / self.CELLS_PER_FOV))
+
+    def get_z_levels(self) -> np.ndarray:
+        return self._zLevelsDiffer
+
+    def get_fovs_count(self):
+        return self._fovsCount
+
+    def read_fov(self, fov: int) -> List[Feature]:
+        rawCellsList = []
+
+        polyList = [None] * self._zPlanesCount
+        prevEntityIdx = self._data.iloc[self._fovsStartIdx[fov]]['EntityID']
+        for rowPolyIdx in range(self._fovsStartIdx[fov], self._fovsStartIdx[fov + 1]):
+            rowPoly = self._data.iloc[rowPolyIdx]
+
+            entityIdx = rowPoly['EntityID']
+            if prevEntityIdx != entityIdx:
+                rawCellsList.append(Feature(str(prevEntityIdx), polyList))
+                prevEntityIdx = entityIdx
+                polyList = [None] * self._zPlanesCount
+
+            polyGeometry = rowPoly['Geometry']
+            if polyGeometry is not None:
+                polyList[rowPoly['ZIndex']] = polyGeometry
+            continue
+
+        rawCellsList.append(Feature(str(prevEntityIdx), polyList))  # last cell
+        return rawCellsList
+
+    def read(self):
+        features = []
+
+        for fovIndex in range(self.get_fovs_count()):
+            features.extend(self.read_fov(fovIndex))
+
+        return features
+
+    def get_z_planes_count(self) -> int:
+        return self._zPlanesCount
+
+
+def cell_reader_factory(pathToFile) -> CellsReader:
+    if pathToFile.endswith('.parquet'):
+        with vzg_open(pathToFile, 'rb') as f:
+            data: GeoDataFrame = gpd.read_parquet(f)
+        return CellsGeoReader(data)
+
+    elif pathToFile.endswith('.geojson'):
+        with vzg_open(pathToFile, 'rb') as f:
+            data: GeoDataFrame = gpd.read_file(f)
+        data = data.rename(columns={'geometry': 'Geometry'})
+        return CellsGeoReader(data)
+
+    else:
+        raise ValueError("Input geometry has an unsupported file extension")
```

### Comparing `vpt-1.0.1/src/vpt/utils/general_data.py` & `vpt-1.0.2/src/vpt/utils/general_data.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,92 +1,92 @@
-from typing import Tuple, List, Dict
-import math
-from pathlib import Path
-
-import numpy as np
-import os
-from enum import Enum
-import json
-
-GRID_HEIGHT = 16
-
-GRID_WIDTH = 16
-
-SCALE_X = 16.0
-
-SCALE_Y = 16.0
-
-PACK_FACTOR = 2 ** 24
-
-
-def grid_size_calculate(textureSize, transformationMatrix) -> Tuple[int, int]:
-    """Calculate voxel grid count based on experiment size.
-        400 microns - is maximum that voxel side could be for proper
-        visualization.
-    """
-    expWidth = textureSize[0] / transformationMatrix[0][0]
-    expHeight = textureSize[1] / transformationMatrix[1][1]
-
-    return math.ceil(expWidth / 400), math.ceil(expHeight / 400)
-
-
-def load_texture_coords(datasetPath: str) -> List:
-    with open(os.path.join(datasetPath, 'pictures', 'manifest.json'), 'r') as read_file:
-        picture_manifest_json = json.load(read_file)
-    return [picture_manifest_json['mosaic_width_pixels'], picture_manifest_json['mosaic_height_pixels']]
-
-
-def load_images_manifest(datasetPath: str) -> Dict:
-    with open(os.path.join(datasetPath, 'pictures', 'manifest.json'), 'r') as read_file:
-        picture_manifest_json = json.load(read_file)
-    return picture_manifest_json
-
-
-def load_texture_matrix(raw_dataset_path: str) -> List:
-    import csv
-    matrix = []
-    with open(os.path.join(raw_dataset_path, 'pictures', 'micron_to_mosaic_pixel_transform.csv'),
-              newline='\n') as csvfile:
-        matrix_file = csv.reader(csvfile, delimiter=' ', quotechar='|')
-
-        for row in matrix_file:
-            matrix_row = []
-            for column in row:
-                matrix_row.append(float(column))
-            matrix.append(matrix_row)
-
-    return matrix
-
-
-class FileType(Enum):
-    Experiment = 0
-    Dataset = 1
-
-
-def write_file(exp_path: str, buffer, file_name, relative_file_path=''):
-    if os.path.isabs(exp_path):
-        file_path = os.path.join(exp_path, relative_file_path)
-    else:
-        file_path = os.path.join(os.path.dirname(__file__), exp_path, relative_file_path)
-
-    Path(file_path).mkdir(parents=True, exist_ok=True)
-    with open(os.path.join(file_path, file_name), 'bw') as file:
-        file.write(buffer)
-
-
-def write_json_file(analysisResult, exp_path: str, output_filename):
-    if os.path.isabs(exp_path):
-        file_path = exp_path
-    else:
-        file_path = os.path.join(os.path.dirname(__file__), exp_path)
-
-    Path(file_path).mkdir(parents=True, exist_ok=True)
-    with open(os.path.join(file_path, output_filename), 'w') as f:
-        json.dump(analysisResult, f, indent=4)
-
-
-def extend_btr_by_fixed_str(btr: bytearray, string: str, max_bytes_count: int):
-    name_len = len(string)
-    btr.extend(str.encode(string))
-    delta = max_bytes_count - name_len
-    for i in range(delta):
-        btr.extend(np.int8(0))
+from typing import Tuple, List, Dict
+import math
+from pathlib import Path
+
+import numpy as np
+import os
+from enum import Enum
+import json
+
+GRID_HEIGHT = 16
+
+GRID_WIDTH = 16
+
+SCALE_X = 16.0
+
+SCALE_Y = 16.0
+
+PACK_FACTOR = 2 ** 24
+
+
+def grid_size_calculate(textureSize, transformationMatrix) -> Tuple[int, int]:
+    """Calculate voxel grid count based on experiment size.
+        400 microns - is maximum that voxel side could be for proper
+        visualization.
+    """
+    expWidth = textureSize[0] / transformationMatrix[0][0]
+    expHeight = textureSize[1] / transformationMatrix[1][1]
+
+    return math.ceil(expWidth / 400), math.ceil(expHeight / 400)
+
+
+def load_texture_coords(datasetPath: str) -> List:
+    with open(os.path.join(datasetPath, 'pictures', 'manifest.json'), 'r') as read_file:
+        picture_manifest_json = json.load(read_file)
+    return [picture_manifest_json['mosaic_width_pixels'], picture_manifest_json['mosaic_height_pixels']]
+
+
+def load_images_manifest(datasetPath: str) -> Dict:
+    with open(os.path.join(datasetPath, 'pictures', 'manifest.json'), 'r') as read_file:
+        picture_manifest_json = json.load(read_file)
+    return picture_manifest_json
+
+
+def load_texture_matrix(raw_dataset_path: str) -> List:
+    import csv
+    matrix = []
+    with open(os.path.join(raw_dataset_path, 'pictures', 'micron_to_mosaic_pixel_transform.csv'),
+              newline='\n') as csvfile:
+        matrix_file = csv.reader(csvfile, delimiter=' ', quotechar='|')
+
+        for row in matrix_file:
+            matrix_row = []
+            for column in row:
+                matrix_row.append(float(column))
+            matrix.append(matrix_row)
+
+    return matrix
+
+
+class FileType(Enum):
+    Experiment = 0
+    Dataset = 1
+
+
+def write_file(exp_path: str, buffer, file_name, relative_file_path=''):
+    if os.path.isabs(exp_path):
+        file_path = os.path.join(exp_path, relative_file_path)
+    else:
+        file_path = os.path.join(os.path.dirname(__file__), exp_path, relative_file_path)
+
+    Path(file_path).mkdir(parents=True, exist_ok=True)
+    with open(os.path.join(file_path, file_name), 'bw') as file:
+        file.write(buffer)
+
+
+def write_json_file(analysisResult, exp_path: str, output_filename):
+    if os.path.isabs(exp_path):
+        file_path = exp_path
+    else:
+        file_path = os.path.join(os.path.dirname(__file__), exp_path)
+
+    Path(file_path).mkdir(parents=True, exist_ok=True)
+    with open(os.path.join(file_path, output_filename), 'w') as f:
+        json.dump(analysisResult, f, indent=4)
+
+
+def extend_btr_by_fixed_str(btr: bytearray, string: str, max_bytes_count: int):
+    name_len = len(string)
+    btr.extend(str.encode(string))
+    delta = max_bytes_count - name_len
+    for i in range(delta):
+        btr.extend(np.int8(0))
```

### Comparing `vpt-1.0.1/src/vpt/utils/raw_cell.py` & `vpt-1.0.2/src/vpt/utils/raw_cell.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-from typing import List
-
-from shapely import geometry
-
-
-class Feature:
-    def __init__(self, rawCellId: str, rawPolysGeometryList: List[List[geometry.shape]]):
-        self.shapes: List[geometry.shape or None] = rawPolysGeometryList
-        self.id = rawCellId
-
-    def get_feature_id(self):
-        return self.id
-
-    def get_boundaries(self, zPlane: int = 0):
-        return self.shapes[zPlane]
-
-    def get_true_polygons(self):
-        return list(filter(lambda shape: shape is not None, self.shapes))
-
-    def get_full_cell(self) -> List:
-        """Add empty polygon on z planes without polygons"""
-        output = []
-        for shape in self.shapes:
-            if shape is not None:
-                output.append(shape)
-            else:
-                output.append(geometry.Polygon(((0, 0), (0, 0), (0, 0))))
-        return output
+from typing import List
+
+from shapely import geometry
+
+
+class Feature:
+    def __init__(self, rawCellId: str, rawPolysGeometryList: List[List[geometry.shape]]):
+        self.shapes: List[geometry.shape or None] = rawPolysGeometryList
+        self.id = rawCellId
+
+    def get_feature_id(self):
+        return self.id
+
+    def get_boundaries(self, zPlane: int = 0):
+        return self.shapes[zPlane]
+
+    def get_true_polygons(self):
+        return list(filter(lambda shape: shape is not None, self.shapes))
+
+    def get_full_cell(self) -> List:
+        """Add empty polygon on z planes without polygons"""
+        output = []
+        for shape in self.shapes:
+            if shape is not None:
+                output.append(shape)
+            else:
+                output.append(geometry.Polygon(((0, 0), (0, 0), (0, 0))))
+        return output
```

### Comparing `vpt-1.0.1/src/vpt/utils/regex_tools.py` & `vpt-1.0.2/src/vpt/utils/regex_tools.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,96 +1,96 @@
-import re
-from dataclasses import dataclass
-from typing import Set, List
-
-from vpt import log
-from vpt.filesystem.vzgfs import protocol_path_split, filesystem_for_protocol, \
-    prefix_for_protocol, get_rasterio_environment, rasterio_open
-
-
-@dataclass(frozen=True)
-class ImagePath:
-    channel: str
-    z_layer: int
-    full_path: str
-
-
-@dataclass(frozen=True)
-class RegexInfo:
-    image_width: int
-    image_height: int
-    images: Set[ImagePath]
-
-
-def get_paths_by_regex(regex: str) -> List[str]:
-    protocol, regex = protocol_path_split(regex)
-    fs = filesystem_for_protocol(protocol)
-    parts = regex.split(fs.sep)
-
-    for i in range(len(parts)):
-        if '?' in parts[i]:
-            break
-
-    root = fs.sep.join(parts[:i])
-    parts = parts[i:]
-
-    def walk_req(rootdir, path_regex):
-        if len(path_regex) == 0:
-            return [rootdir]
-        res = []
-
-        try:
-            _, dirs, files = next(fs.walk(rootdir, maxdepth=1))
-        except StopIteration:
-            return res
-
-        if len(path_regex) == 1:
-            for filename in files:
-                if re.match(path_regex[0], filename):
-                    res.append(filename)
-            return res
-
-        for dirname in dirs:
-            if re.match(path_regex[0], dirname):
-                walk_res = walk_req(fs.sep.join([rootdir, dirname]), path_regex[1:])
-                for p in walk_res:
-                    res.append(fs.sep.join([dirname, p]))
-
-        return res
-
-    paths = [fs.sep.join([root, path]) if root else path for path in walk_req(root, parts)]
-    return [path for path in paths if fs.isfile(path)]
-
-
-def parse_regex(regex: str) -> RegexInfo:
-    width, height = 0, 0
-    images = set()
-
-    if '?P<stain>' not in regex or '?P<z>' not in regex:
-        raise ValueError('Bad regular expression: named group "z" or "stain" is missed')
-
-    paths = get_paths_by_regex(regex)
-    protocol, regex = protocol_path_split(regex)
-    fs = filesystem_for_protocol(protocol)
-
-    for path in paths:
-        match = re.match(regex, path)
-        try:
-            z = int(match.group('z'))
-            stain = match.group('stain')
-        except IndexError:
-            log.warning(f'Regular expression should contain groups "z" and "stain". Path {path} has not that groups '
-                        f'and will be skipped.')
-            continue
-
-        full_path = prefix_for_protocol(protocol) + fs.info(path)['name']
-
-        with get_rasterio_environment(full_path):
-            with rasterio_open(full_path) as tif:
-                im_height, im_width = tif.height, tif.width
-                if width and height and (im_width != width or im_height != height):
-                    raise ValueError('Images sizes are not equal')
-                width = im_width
-                height = im_height
-
-        images.add(ImagePath(stain, z, full_path))
-    return RegexInfo(width, height, images)
+import re
+from dataclasses import dataclass
+from typing import Set, List
+
+from vpt import log
+from vpt.filesystem.vzgfs import protocol_path_split, filesystem_for_protocol, \
+    prefix_for_protocol, get_rasterio_environment, rasterio_open
+
+
+@dataclass(frozen=True)
+class ImagePath:
+    channel: str
+    z_layer: int
+    full_path: str
+
+
+@dataclass(frozen=True)
+class RegexInfo:
+    image_width: int
+    image_height: int
+    images: Set[ImagePath]
+
+
+def get_paths_by_regex(regex: str) -> List[str]:
+    protocol, regex = protocol_path_split(regex)
+    fs = filesystem_for_protocol(protocol)
+    parts = regex.split(fs.sep)
+
+    for i in range(len(parts)):
+        if '?' in parts[i]:
+            break
+
+    root = fs.sep.join(parts[:i])
+    parts = parts[i:]
+
+    def walk_req(rootdir, path_regex):
+        if len(path_regex) == 0:
+            return [rootdir]
+        res = []
+
+        try:
+            _, dirs, files = next(fs.walk(rootdir, maxdepth=1))
+        except StopIteration:
+            return res
+
+        if len(path_regex) == 1:
+            for filename in files:
+                if re.match(path_regex[0], filename):
+                    res.append(filename)
+            return res
+
+        for dirname in dirs:
+            if re.match(path_regex[0], dirname):
+                walk_res = walk_req(fs.sep.join([rootdir, dirname]), path_regex[1:])
+                for p in walk_res:
+                    res.append(fs.sep.join([dirname, p]))
+
+        return res
+
+    paths = [fs.sep.join([root, path]) if root else path for path in walk_req(root, parts)]
+    return [path for path in paths if fs.isfile(path)]
+
+
+def parse_regex(regex: str) -> RegexInfo:
+    width, height = 0, 0
+    images = set()
+
+    if '?P<stain>' not in regex or '?P<z>' not in regex:
+        raise ValueError('Bad regular expression: named group "z" or "stain" is missed')
+
+    paths = get_paths_by_regex(regex)
+    protocol, regex = protocol_path_split(regex)
+    fs = filesystem_for_protocol(protocol)
+
+    for path in paths:
+        match = re.match(regex, path)
+        try:
+            z = int(match.group('z'))
+            stain = match.group('stain')
+        except IndexError:
+            log.warning(f'Regular expression should contain groups "z" and "stain". Path {path} has not that groups '
+                        f'and will be skipped.')
+            continue
+
+        full_path = prefix_for_protocol(protocol) + fs.info(path)['name']
+
+        with get_rasterio_environment(full_path):
+            with rasterio_open(full_path) as tif:
+                im_height, im_width = tif.height, tif.width
+                if width and height and (im_width != width or im_height != height):
+                    raise ValueError('Images sizes are not equal')
+                width = im_width
+                height = im_height
+
+        images.add(ImagePath(stain, z, full_path))
+    return RegexInfo(width, height, images)
```

### Comparing `vpt-1.0.1/src/vpt/utils/seg_json_generator/cmd_args.py` & `vpt-1.0.2/src/vpt/utils/seg_json_generator/cmd_args.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-from argparse import ArgumentParser
-from dataclasses import dataclass
-
-from vpt.utils.validate import validate_exists, validate_does_not_exist
-
-
-@dataclass(frozen=True)
-class GenerateJsonArgs:
-    input_analysis_spec: str
-    output_path: str
-    overwrite: bool
-
-
-def validate_args(args: GenerateJsonArgs):
-    validate_exists(args.input_analysis_spec)
-    if not args.overwrite:
-        validate_does_not_exist(args.output_path)
-
-
-def get_parser() -> ArgumentParser:
-    parser = ArgumentParser()
-
-    parser.add_argument('--input-analysis-spec', type=str, required=True,
-                        help='Path to a json with analysis arguments for template segmentation specification')
-    parser.add_argument('--output-path', type=str, required=True,
-                        help='Path to the json file where the generated segmentation specification will be stored')
-    parser.add_argument('--overwrite', action='store_true', default=False, required=False,
-                        help='')
-    return parser
-
-
-def parse_args():
-    return get_parser().parse_args()
+from argparse import ArgumentParser
+from dataclasses import dataclass
+
+from vpt.utils.validate import validate_exists, validate_does_not_exist
+
+
+@dataclass(frozen=True)
+class GenerateJsonArgs:
+    input_analysis_spec: str
+    output_path: str
+    overwrite: bool
+
+
+def validate_args(args: GenerateJsonArgs):
+    validate_exists(args.input_analysis_spec)
+    if not args.overwrite:
+        validate_does_not_exist(args.output_path)
+
+
+def get_parser() -> ArgumentParser:
+    parser = ArgumentParser()
+
+    parser.add_argument('--input-analysis-spec', type=str, required=True,
+                        help='Path to a json with analysis arguments for template segmentation specification')
+    parser.add_argument('--output-path', type=str, required=True,
+                        help='Path to the json file where the generated segmentation specification will be stored')
+    parser.add_argument('--overwrite', action='store_true', default=False, required=False,
+                        help='')
+    return parser
+
+
+def parse_args():
+    return get_parser().parse_args()
```

### Comparing `vpt-1.0.1/src/vpt/utils/seg_json_generator/main.py` & `vpt-1.0.2/src/vpt/utils/seg_json_generator/main.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-import json
-import os.path
-from dataclasses import asdict
-from typing import Dict
-
-from vpt.filesystem import vzg_open
-from vpt.utils.seg_json_generator.cmd_args import GenerateJsonArgs, parse_args
-from vpt.utils.seg_json_generator.input_utils import read_parameters_json, fill_template_json, AlgorithmParameters
-from vpt.utils.validate import validate_exists
-
-
-def run_generator(args):
-    args = GenerateJsonArgs(**vars(args))
-    algorithm_params = read_parameters_json(args.input_analysis_spec)
-    data = generate_segmentation_spec(**asdict(algorithm_params))
-    with vzg_open(args.output_path, 'w') as f:
-        json.dump(data, f)
-
-
-def generate_segmentation_spec(template_name: str,
-                               template_parameters: Dict,
-                               custom_parameters: Dict = None) -> Dict:
-    path = f'{os.path.dirname(os.path.abspath(__file__))}/templates/{template_name}.json'
-    validate_exists(path)
-    # update default arguments
-    if custom_parameters is None:
-        custom_parameters = {}
-    template_parameters = template_parameters.copy()
-    if 'all_z' not in template_parameters:
-        template_parameters['all_z'] = [0, 1, 2, 3, 4, 5, 6]
-    if 'z_um' not in template_parameters:
-        template_parameters['z_um'] = [(x + 1) * 1.5 for x in template_parameters['all_z']]
-
-    return fill_template_json(path, AlgorithmParameters(template_name, template_parameters, custom_parameters))
-
-
-if __name__ == '__main__':
-    run_generator(parse_args())
+import json
+import os.path
+from dataclasses import asdict
+from typing import Dict
+
+from vpt.filesystem import vzg_open
+from vpt.utils.seg_json_generator.cmd_args import GenerateJsonArgs, parse_args
+from vpt.utils.seg_json_generator.input_utils import read_parameters_json, fill_template_json, AlgorithmParameters
+from vpt.utils.validate import validate_exists
+
+
+def run_generator(args):
+    args = GenerateJsonArgs(**vars(args))
+    algorithm_params = read_parameters_json(args.input_analysis_spec)
+    data = generate_segmentation_spec(**asdict(algorithm_params))
+    with vzg_open(args.output_path, 'w') as f:
+        json.dump(data, f)
+
+
+def generate_segmentation_spec(template_name: str,
+                               template_parameters: Dict,
+                               custom_parameters: Dict = None) -> Dict:
+    path = f'{os.path.dirname(os.path.abspath(__file__))}/templates/{template_name}.json'
+    validate_exists(path)
+    # update default arguments
+    if custom_parameters is None:
+        custom_parameters = {}
+    template_parameters = template_parameters.copy()
+    if 'all_z' not in template_parameters:
+        template_parameters['all_z'] = [0, 1, 2, 3, 4, 5, 6]
+    if 'z_um' not in template_parameters:
+        template_parameters['z_um'] = [(x + 1) * 1.5 for x in template_parameters['all_z']]
+
+    return fill_template_json(path, AlgorithmParameters(template_name, template_parameters, custom_parameters))
+
+
+if __name__ == '__main__':
+    run_generator(parse_args())
```

### Comparing `vpt-1.0.1/src/vpt/utils/validate.py` & `vpt-1.0.2/src/vpt/utils/validate.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-from typing import List
-
-from vpt.filesystem.vzgfs import filesystem_path_split
-
-
-def validate_does_not_exist(path: str):
-    fs, path_inside_fs = filesystem_path_split(path)
-    if fs.exists(path_inside_fs):
-        raise ValueError(f'Object already exists: {path}')
-
-
-def validate_exists(path: str):
-    fs, path_inside_fs = filesystem_path_split(path)
-    if not fs.exists(path_inside_fs):
-        from pathlib import Path
-        raise ValueError(f'Object does not exist: {path} {str(Path(path).absolute())}')
-
-
-def validate_directory_empty(path: str):
-    fs, path_inside_fs = filesystem_path_split(path)
-
-    if fs.exists(path_inside_fs) and len(fs.listdir(path_inside_fs, detail=False)) > 0:
-        raise ValueError(f'Directory is not empty {path}')
-
-
-def validate_micron_to_mosaic_transform(transform: List[List[float]]):
-    if len(transform) != 3 or not all(map(lambda row: len(row) == 3, transform)):
-        raise ValueError('Micron to mosaic transform should be a 3x3 matrix')
+from typing import List
+
+from vpt.filesystem.vzgfs import filesystem_path_split
+
+
+def validate_does_not_exist(path: str):
+    fs, path_inside_fs = filesystem_path_split(path)
+    if fs.exists(path_inside_fs):
+        raise ValueError(f'Object already exists: {path}')
+
+
+def validate_exists(path: str):
+    fs, path_inside_fs = filesystem_path_split(path)
+    if not fs.exists(path_inside_fs):
+        from pathlib import Path
+        raise ValueError(f'Object does not exist: {path} {str(Path(path).absolute())}')
+
+
+def validate_directory_empty(path: str):
+    fs, path_inside_fs = filesystem_path_split(path)
+
+    if fs.exists(path_inside_fs) and len(fs.listdir(path_inside_fs, detail=False)) > 0:
+        raise ValueError(f'Directory is not empty {path}')
+
+
+def validate_micron_to_mosaic_transform(transform: List[List[float]]):
+    if len(transform) != 3 or not all(map(lambda row: len(row) == 3, transform)):
+        raise ValueError('Micron to mosaic transform should be a 3x3 matrix')
```

### Comparing `vpt-1.0.1/src/vpt/utils/vzgrepacker.py` & `vpt-1.0.2/src/vpt/utils/vzgrepacker.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,142 +1,142 @@
-import json
-import os
-import shutil
-import zipfile
-from distutils.dir_util import remove_tree
-
-from vpt.filesystem import vzg_open
-from vpt.filesystem.vzgfs import protocol_path_split, Protocol, filesystem_for_protocol
-from vpt.update_vzg.imageparams import ImageParams
-from vpt.update_vzg.manifestgen import ManifestGenerator
-from vpt.utils.general_data import load_images_manifest, write_json_file
-
-
-def create_manifest(datasetName: str,
-                    datasetPath: str,
-                    zPlanes: int,
-                    imageParams: ImageParams
-                    ):
-    manifest = ManifestGenerator(
-        imageParams.textureSize, imageParams.micronToPixelMatrix, datasetName)
-
-    manifest.set_planes_count(zPlanes)
-    manifest.set_cells_status(True)
-    manifest.set_transcripts_status(True)
-
-    pyrMosaicDict = load_images_manifest(datasetPath)['mosaic_pyramid_files']
-
-    imageDict = parse_picture_manifest(pyrMosaicDict)
-    manifest.set_image_dict(imageDict)
-    manifest_data = manifest.create_json_manifest()
-
-    write_json_file(manifest_data, f'{datasetPath}', 'manifest.json')
-
-
-def parse_picture_manifest(pictureManifestJson) -> dict:
-    pictureManifestDict = {}
-
-    for mosaic in pictureManifestJson:
-        tagName = mosaic['stain']
-        if tagName not in pictureManifestDict:
-            pictureManifestDict[tagName] = {'Files': []}
-
-        zPlane = int(mosaic['z'])
-        pictureManifestDict[tagName]['Files'].append({"zPlane": zPlane, "Name": mosaic['file_name']})
-
-    return pictureManifestDict
-
-
-class VzgRepacker:
-    def __init__(self, originVzgPath: str, tempBuildFolderPath):
-        self._originVzgPath: str = originVzgPath
-        self._datasetName: str = os.path.basename(self._originVzgPath)[:-4]
-        self._tempBuildFolderPath = tempBuildFolderPath
-        self._tempVzgFolderPath = os.path.join(tempBuildFolderPath, self._datasetName)
-
-        self._z_planes_count = -1
-
-    def get_dataset_folder(self):
-        return self._tempVzgFolderPath
-
-    def read_dataset_z_planes_count(self) -> int:
-        if self._z_planes_count > 0:
-            return self._z_planes_count
-
-        imageManifestPath = os.path.join(self._tempVzgFolderPath, 'pictures', 'manifest.json')
-        with open(imageManifestPath, 'r') as f:
-            imageManifest = json.load(f)
-
-        zPlanesNumbers = []
-        for tiffDescription in imageManifest['mosaic_files']:
-            zPlanesNumbers.append(tiffDescription['z'])
-
-        self._z_planes_count = max(zPlanesNumbers) + 1
-        return self._z_planes_count
-
-    def unpack_vzg(self):
-        protocol, path_inside_fs = protocol_path_split(self._originVzgPath)
-        if protocol != Protocol.LOCAL:  # Protocol.S3 or Protocol.GCS
-            fs = filesystem_for_protocol(protocol)
-            vzgInputPath = os.path.join(self._tempBuildFolderPath, f'{self._datasetName}.vzg')
-            fs.get(self._originVzgPath, vzgInputPath)
-        else:  # Protocol.LOCAL
-            vzgInputPath = self._originVzgPath
-
-        with vzg_open(vzgInputPath, 'rb') as f:
-            with zipfile.ZipFile(f) as zip_ref:
-                zip_ref.extractall(self._tempVzgFolderPath)
-
-        print(f'{self._originVzgPath} unpacked!')
-
-    def repack_vzg_file(self, outputVzgFilePath: str, imageParams: ImageParams):
-        maxZPlane = self.read_dataset_z_planes_count()
-
-        vzgRootFolder = os.listdir(self._tempVzgFolderPath)
-        manifestExist = False
-        for file in vzgRootFolder:
-            if file in ('manifest.xml', 'manifest.json'):
-                manifestExist = True
-                if file == 'manifest.json':
-                    self._add_cells_flag_to_manifest()
-                break
-
-        if not manifestExist:
-            create_manifest(self._datasetName, self._tempVzgFolderPath, maxZPlane, imageParams)
-            print('New manifest created')
-
-        if os.path.exists(f'{outputVzgFilePath}.vzg'):
-            os.remove(f'{outputVzgFilePath}.vzg')
-
-        protocol, path_inside_fs = protocol_path_split(outputVzgFilePath)
-        if protocol != Protocol.LOCAL:  # Protocol.S3 or Protocol.GCS
-            tempNewVzgPath = os.path.join(self._tempBuildFolderPath, os.path.basename(outputVzgFilePath))
-            shutil.make_archive(tempNewVzgPath, 'zip', self._tempVzgFolderPath)
-            os.rename(f'{tempNewVzgPath}.zip', f'{tempNewVzgPath}.vzg')
-
-            fs = filesystem_for_protocol(protocol)
-            fs.put(f'{tempNewVzgPath}.vzg', f'{path_inside_fs}.vzg')
-        else:
-            shutil.make_archive(outputVzgFilePath, 'zip', self._tempVzgFolderPath)
-            os.rename(f'{outputVzgFilePath}.zip', f'{outputVzgFilePath}.vzg')
-        print('new vzg file created')
-
-        if os.path.exists(self._tempBuildFolderPath):
-            remove_tree(self._tempBuildFolderPath)
-        print('temp files deleted')
-
-    def _add_cells_flag_to_manifest(self):
-        manifestPath = os.path.join(self._tempVzgFolderPath, 'manifest.json')
-        with open(manifestPath, 'r') as f:
-            manifestData = json.load(f)
-            manifestData['Cells'] = True
-
-        with open(manifestPath, 'w') as f:
-            json.dump(manifestData, f, indent=4)
-
-    def read_genes_info_array(self) -> dict:
-        gene_info_path = os.path.join(self._tempVzgFolderPath, 'genes', 'genes_info_array.json')
-
-        with open(gene_info_path, 'r') as f:
-            gene_info_data = json.load(f)
-
-        return gene_info_data
+import json
+import os
+import shutil
+import zipfile
+from distutils.dir_util import remove_tree
+
+from vpt.filesystem import vzg_open
+from vpt.filesystem.vzgfs import protocol_path_split, Protocol, filesystem_for_protocol
+from vpt.update_vzg.imageparams import ImageParams
+from vpt.update_vzg.manifestgen import ManifestGenerator
+from vpt.utils.general_data import load_images_manifest, write_json_file
+
+
+def create_manifest(datasetName: str,
+                    datasetPath: str,
+                    zPlanes: int,
+                    imageParams: ImageParams
+                    ):
+    manifest = ManifestGenerator(
+        imageParams.textureSize, imageParams.micronToPixelMatrix, datasetName)
+
+    manifest.set_planes_count(zPlanes)
+    manifest.set_cells_status(True)
+    manifest.set_transcripts_status(True)
+
+    pyrMosaicDict = load_images_manifest(datasetPath)['mosaic_pyramid_files']
+
+    imageDict = parse_picture_manifest(pyrMosaicDict)
+    manifest.set_image_dict(imageDict)
+    manifest_data = manifest.create_json_manifest()
+
+    write_json_file(manifest_data, f'{datasetPath}', 'manifest.json')
+
+
+def parse_picture_manifest(pictureManifestJson) -> dict:
+    pictureManifestDict = {}
+
+    for mosaic in pictureManifestJson:
+        tagName = mosaic['stain']
+        if tagName not in pictureManifestDict:
+            pictureManifestDict[tagName] = {'Files': []}
+
+        zPlane = int(mosaic['z'])
+        pictureManifestDict[tagName]['Files'].append({"zPlane": zPlane, "Name": mosaic['file_name']})
+
+    return pictureManifestDict
+
+
+class VzgRepacker:
+    def __init__(self, originVzgPath: str, tempBuildFolderPath):
+        self._originVzgPath: str = originVzgPath
+        self._datasetName: str = os.path.basename(self._originVzgPath)[:-4]
+        self._tempBuildFolderPath = tempBuildFolderPath
+        self._tempVzgFolderPath = os.path.join(tempBuildFolderPath, self._datasetName)
+
+        self._z_planes_count = -1
+
+    def get_dataset_folder(self):
+        return self._tempVzgFolderPath
+
+    def read_dataset_z_planes_count(self) -> int:
+        if self._z_planes_count > 0:
+            return self._z_planes_count
+
+        imageManifestPath = os.path.join(self._tempVzgFolderPath, 'pictures', 'manifest.json')
+        with open(imageManifestPath, 'r') as f:
+            imageManifest = json.load(f)
+
+        zPlanesNumbers = []
+        for tiffDescription in imageManifest['mosaic_files']:
+            zPlanesNumbers.append(tiffDescription['z'])
+
+        self._z_planes_count = max(zPlanesNumbers) + 1
+        return self._z_planes_count
+
+    def unpack_vzg(self):
+        protocol, path_inside_fs = protocol_path_split(self._originVzgPath)
+        if protocol != Protocol.LOCAL:  # Protocol.S3 or Protocol.GCS
+            fs = filesystem_for_protocol(protocol)
+            vzgInputPath = os.path.join(self._tempBuildFolderPath, f'{self._datasetName}.vzg')
+            fs.get(self._originVzgPath, vzgInputPath)
+        else:  # Protocol.LOCAL
+            vzgInputPath = self._originVzgPath
+
+        with vzg_open(vzgInputPath, 'rb') as f:
+            with zipfile.ZipFile(f) as zip_ref:
+                zip_ref.extractall(self._tempVzgFolderPath)
+
+        print(f'{self._originVzgPath} unpacked!')
+
+    def repack_vzg_file(self, outputVzgFilePath: str, imageParams: ImageParams):
+        maxZPlane = self.read_dataset_z_planes_count()
+
+        vzgRootFolder = os.listdir(self._tempVzgFolderPath)
+        manifestExist = False
+        for file in vzgRootFolder:
+            if file in ('manifest.xml', 'manifest.json'):
+                manifestExist = True
+                if file == 'manifest.json':
+                    self._add_cells_flag_to_manifest()
+                break
+
+        if not manifestExist:
+            create_manifest(self._datasetName, self._tempVzgFolderPath, maxZPlane, imageParams)
+            print('New manifest created')
+
+        if os.path.exists(f'{outputVzgFilePath}.vzg'):
+            os.remove(f'{outputVzgFilePath}.vzg')
+
+        protocol, path_inside_fs = protocol_path_split(outputVzgFilePath)
+        if protocol != Protocol.LOCAL:  # Protocol.S3 or Protocol.GCS
+            tempNewVzgPath = os.path.join(self._tempBuildFolderPath, os.path.basename(outputVzgFilePath))
+            shutil.make_archive(tempNewVzgPath, 'zip', self._tempVzgFolderPath)
+            os.rename(f'{tempNewVzgPath}.zip', f'{tempNewVzgPath}.vzg')
+
+            fs = filesystem_for_protocol(protocol)
+            fs.put(f'{tempNewVzgPath}.vzg', f'{path_inside_fs}.vzg')
+        else:
+            shutil.make_archive(outputVzgFilePath, 'zip', self._tempVzgFolderPath)
+            os.rename(f'{outputVzgFilePath}.zip', f'{outputVzgFilePath}.vzg')
+        print('new vzg file created')
+
+        if os.path.exists(self._tempBuildFolderPath):
+            remove_tree(self._tempBuildFolderPath)
+        print('temp files deleted')
+
+    def _add_cells_flag_to_manifest(self):
+        manifestPath = os.path.join(self._tempVzgFolderPath, 'manifest.json')
+        with open(manifestPath, 'r') as f:
+            manifestData = json.load(f)
+            manifestData['Cells'] = True
+
+        with open(manifestPath, 'w') as f:
+            json.dump(manifestData, f, indent=4)
+
+    def read_genes_info_array(self) -> dict:
+        gene_info_path = os.path.join(self._tempVzgFolderPath, 'genes', 'genes_info_array.json')
+
+        with open(gene_info_path, 'r') as f:
+            gene_info_data = json.load(f)
+
+        return gene_info_data
```

### Comparing `vpt-1.0.1/setup.py` & `vpt-1.0.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,83 +1,188 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: vpt
+Version: 1.0.2
+Summary: Command line tool for highly parallelized processing of Vizgen data
+Home-page: https://github.com/Vizgen/vizgen-postprocessing
+License: Apache-2.0
+Author: Vizgen
+Author-email: techsupport@vizgen.com
+Maintainer: Timothy Wiggin
+Maintainer-email: timothy.wiggin@vizgen.com
+Requires-Python: >=3.9,<3.11
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Natural Language :: English
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Classifier: Topic :: Scientific/Engineering :: Image Processing
+Requires-Dist: boto3 (==1.17)
+Requires-Dist: cellpose (==1.0.2)
+Requires-Dist: dask (==2022.9.0)
+Requires-Dist: distributed (==2022.9.0)
+Requires-Dist: fsspec (==2021.10.0)
+Requires-Dist: gcsfs (==2021.10.0)
+Requires-Dist: geojson (==2.5.0)
+Requires-Dist: geopandas (==0.12.1)
+Requires-Dist: h5py (==3.7.0)
+Requires-Dist: numpy (==1.22.4)
+Requires-Dist: opencv-python-headless (==4.6.0.66)
+Requires-Dist: pandas (==1.4.3)
+Requires-Dist: pyarrow (==8.0.0)
+Requires-Dist: pyclustering (==0.10.1.2)
+Requires-Dist: python-dotenv (==0.20.0)
+Requires-Dist: pyvips (==2.2.1)
+Requires-Dist: rasterio (==1.3.0)
+Requires-Dist: s3fs (==2021.10.0)
+Requires-Dist: scikit-image (==0.19.3)
+Requires-Dist: scipy (==1.8.1)
+Requires-Dist: shapely (==2.0)
+Requires-Dist: stardist (==0.8.3)
+Requires-Dist: tensorflow (==2.9.1)
+Project-URL: Documentation, https://vizgen.github.io/vizgen-postprocessing/
+Project-URL: Repository, https://github.com/Vizgen/vizgen-postprocessing
+Description-Content-Type: text/markdown
+
+[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
+![PyPI](https://img.shields.io/pypi/v/vpt)
+[![Coverage Status](https://coveralls.io/repos/github/Vizgen/vizgen-postprocessing/badge.svg?branch=develop)](https://coveralls.io/github/Vizgen/vizgen-postprocessing?branch=develop)
+
+# Vizgen Post-processing Tool
+
+The Vizgen Post-processing Tool (VPT) enables users to reprocess and refine the single-cell results of MERSCOPE experiments. 
+VPT is a command line tool that emphasizes scalable, reproducible analysis, and can be run on a workstation, a cluster, or 
+be deployed in a cloud computing environment.
+
+
+## Features
+- Perform cell segmentation
+    - Reproduce standard Vizgen segmentation options
+    - Perform reproducible custom segmentation
+- Import cell segmentation from other tools
+    - Supports geojson and hdf5 formats
+- Regenerate single cell data with new segmentation
+    - Cell by gene matrix
+    - Cell spatial metadata
+    - Image intensity in each cell
+    - Update MERSCOPE Vizualizer file (vzg)
+- Image format conversion
+    - Convert large tiff files to single or multi-channel Pyramidal OME-TIFF files
+- Nextflow compatible, example pipeline provided
+
+
+## Installation
+
+Install the tool through your choice of 
+- [pip](https://pip.pypa.io/en/stable/getting-started/)
+- [Docker](https://docs.docker.com/desktop/extensions-sdk/quickstart/)
+- [poetry](https://python-poetry.org/)
+
+To access in-utility help documentation run the process below in the installed environment.
+```bash
+  vpt --help
+```
+    
+## Usage
+
+VPT accepts two types of inputs to specify how to run segmentation:
+- Command line parameters
+    - relate to where to find the input data and are expected to vary with each experiment
+- Segmentation algorithm .json file parameters
+    - describes a series of steps to perform on the input data
+
+Using the same segmentation algorithm on a series of experiments ensures that they are processed identically and reproducibly.
+
+In addition to the user guide, several working segmentation algorithm .json files are provided that can serve either as a 
+robust segmentation definition or as a template for a custom workflow.
+
+## Quick start commands:
+
+
+run-segmentation    ​
+- Top-level interface for vpt which invokes the segmentation functionality of the tool.​
+
+prepare-segmentation​
+ - Generates a segmentation specification json file to be used for cell segmentation tasks. ​
+
+run-segmentation-on-tile​
+ - Executes the segmentation algorithm on a specific tile of the mosaic images.​
+
+compile-tile-segmentation​
+- Combines the per-tile segmentation outputs into a single, internally-consistent parquet file containing all of the 
+segmentation boundaries found in the experiment.​
+
+derive-entity-metadata​
+- Uses the segmentation boundaries to calculate the geometric attributes of each Entity​
+
+partition-transcripts​
+- Uses the segmentation boundaries to determine which Entity, if any, contains each detected transcript.​
+
+sum-signals​
+- Uses the segmentation boundaries to find the intensity of each mosaic image in each Entity.​
+
+update-vzg​
+- Updates an existing .vzg file with new segmentation boundaries and the corresponding expression matrix.​
+
+convert-geometry​
+- Converts Entity boundaries produced by a different tool into a vpt compatible parquet file.​
+
+convert-to-ome​
+- Transforms the large 16-bit mosaic tiff images produced by the MERSCOPE into a OME pyramidal tiff.​
+
+convert-to-rgb-ome​
+- Converts up to three flat tiff images into rgb OME-tiff pyramidal images.​
+
+For more detail on commands and arguments, please see the user guide.
+
+## Documentation
+
+[User Guide](https://vizgen.github.io/vizgen-postprocessing/)
+
+## Feedback
+
+If you encounter issues or bugs, let us know by [submitting an issue!](https://github.com/Vizgen/vizgen-postprocessing/issues)
+Please include:
+
+- A quick issue summary
+- Steps that caused it to occur
+- The exception generated by the code, if applicable
+- Specific lines of code, if indicated in the error message
+
+
+If you have any other feedback or issues, please reach out to your regional Vizgen field application scientist and CC: Vizgen 
+Tech Support at techsupport@vizgen.com.
+
+Please include VPT in your subject line along with the above information in the body.
+
+## Contributing & Code of Conduct
+
+We welcome code contributions! Please refer to the [contribution guide](CONTRIBUTING.md) before getting started.
+
+## Authors
+
+- [Vizgen](https://vizgen.com/)
+
+![Logo](https://vizgen.com/wp-content/uploads/2022/12/Vizgen-Logo_Vizgen-BlackColor-.png)
+
+## License
+
+   Copyright 2022 Vizgen, Inc. All Rights Reserved
+   
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
 
-package_dir = \
-{'': 'src'}
-
-packages = \
-['vpt',
- 'vpt.app',
- 'vpt.compile_tile_segmentation',
- 'vpt.convert_geometry',
- 'vpt.convert_geometry.converters',
- 'vpt.convert_to_ome',
- 'vpt.derive_cell_metadata',
- 'vpt.filesystem',
- 'vpt.partition_transcripts',
- 'vpt.prepare_segmentation',
- 'vpt.run_segmentation',
- 'vpt.run_segmentation_on_tile',
- 'vpt.segmentation',
- 'vpt.segmentation.cellpose',
- 'vpt.segmentation.filters',
- 'vpt.segmentation.stardist',
- 'vpt.segmentation.utils',
- 'vpt.segmentation.watershed',
- 'vpt.sum_signals',
- 'vpt.update_vzg',
- 'vpt.update_vzg.assemble',
- 'vpt.update_vzg.polygons',
- 'vpt.utils',
- 'vpt.utils.seg_json_generator']
-
-package_data = \
-{'': ['*'], 'vpt.utils.seg_json_generator': ['templates/*']}
-
-install_requires = \
-['boto3==1.17',
- 'cellpose==1.0.2',
- 'dask==2022.9.0',
- 'distributed==2022.9.0',
- 'fsspec==2021.10.0',
- 'gcsfs==2021.10.0',
- 'geojson==2.5.0',
- 'geopandas==0.12.1',
- 'h5py==3.7.0',
- 'numpy==1.22.4',
- 'opencv-python-headless==4.6.0.66',
- 'pandas==1.4.3',
- 'pyarrow==8.0.0',
- 'pyclustering==0.10.1.2',
- 'python-dotenv==0.20.0',
- 'pyvips==2.2.1',
- 'rasterio==1.3.0',
- 's3fs==2021.10.0',
- 'scikit-image==0.19.3',
- 'scipy==1.8.1',
- 'shapely==2.0',
- 'stardist==0.8.3',
- 'tensorflow==2.9.1']
-
-entry_points = \
-{'console_scripts': ['vpt = vpt.vizgen_postprocess:entry_point']}
-
-setup_kwargs = {
-    'name': 'vpt',
-    'version': '1.0.1',
-    'description': 'Command line tool for highly parallelized processing of Vizgen data',
-    'long_description': '[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)\n![PyPI](https://img.shields.io/pypi/v/vpt)\n[![Coverage Status](https://coveralls.io/repos/github/Vizgen/vizgen-postprocessing/badge.svg?branch=develop&t=EsWr25)](https://coveralls.io/github/Vizgen/vizgen-postprocessing?branch=develop)\n\n# Vizgen Post-processing Tool\n\nThe Vizgen Post-processing Tool (VPT) enables users to reprocess and refine the single-cell results of MERSCOPE experiments. \nVPT is a command line tool that emphasizes scalable, reproducible analysis, and can be run on a workstation, a cluster, or \nbe deployed in a cloud computing environment.\n\n\n## Features\n- Perform cell segmentation\n    - Reproduce standard Vizgen segmentation options\n    - Perform reproducible custom segmentation\n- Import cell segmentation from other tools\n    - Supports geojson and hdf5 formats\n- Regenerate single cell data with new segmentation\n    - Cell by gene matrix\n    - Cell spatial metadata\n    - Image intensity in each cell\n    - Update MERSCOPE Vizualizer file (vzg)\n- Image format conversion\n    - Convert large tiff files to single or multi-channel Pyramidal OME-TIFF files\n- Nextflow compatible, example pipeline provided\n\n\n## Installation\n\nInstall the tool through your choice of \n- [pip](https://pip.pypa.io/en/stable/getting-started/)\n- [Docker](https://docs.docker.com/desktop/extensions-sdk/quickstart/)\n- [poetry](https://python-poetry.org/)\n\nTo access in-utility help documentation run the process below in the installed environment.\n```bash\n  vpt --help\n```\n    \n## Usage\n\nVPT accepts two types of inputs to specify how to run segmentation:\n- Command line parameters\n    - relate to where to find the input data and are expected to vary with each experiment\n- Segmentation algorithm .json file parameters\n    - describes a series of steps to perform on the input data\n\nUsing the same segmentation algorithm on a series of experiments ensures that they are processed identically and reproducibly.\n\nIn addition to the user guide, several working segmentation algorithm .json files are provided that can serve either as a \nrobust segmentation definition or as a template for a custom workflow.\n\n## Quick start commands:\n\n\nrun-segmentation    \u200b\n- Top-level interface for vpt which invokes the segmentation functionality of the tool.\u200b\n\nprepare-segmentation\u200b\n - Generates a segmentation specification json file to be used for cell segmentation tasks. \u200b\n\nrun-segmentation-on-tile\u200b\n - Executes the segmentation algorithm on a specific tile of the mosaic images.\u200b\n\ncompile-tile-segmentation\u200b\n- Combines the per-tile segmentation outputs into a single, internally-consistent parquet file containing all of the \nsegmentation boundaries found in the experiment.\u200b\n\nderive-entity-metadata\u200b\n- Uses the segmentation boundaries to calculate the geometric attributes of each Entity\u200b\n\npartition-transcripts\u200b\n- Uses the segmentation boundaries to determine which Entity, if any, contains each detected transcript.\u200b\n\nsum-signals\u200b\n- Uses the segmentation boundaries to find the intensity of each mosaic image in each Entity.\u200b\n\nupdate-vzg\u200b\n- Updates an existing .vzg file with new segmentation boundaries and the corresponding expression matrix.\u200b\n\nconvert-geometry\u200b\n- Converts Entity boundaries produced by a different tool into a vpt compatible parquet file.\u200b\n\nconvert-to-ome\u200b\n- Transforms the large 16-bit mosaic tiff images produced by the MERSCOPE into a OME pyramidal tiff.\u200b\n\nconvert-to-rgb-ome\u200b\n- Converts up to three flat tiff images into rgb OME-tiff pyramidal images.\u200b\n\nFor more detail on commands and arguments, please see the user guide.\n\n## Documentation\n\n[User Guide](https://vizgen.github.io/vizgen-postprocessing/)\n\n## Feedback\n\nIf you encounter issues or bugs, let us know by [submitting an issue!](https://github.com/Vizgen/vizgen-postprocessing/issues)\nPlease include:\n\n- A quick issue summary\n- Steps that caused it to occur\n- The exception generated by the code, if applicable\n- Specific lines of code, if indicated in the error message\n\n\nIf you have any other feedback or issues, please reach out to your regional Vizgen field application scientist and CC: Vizgen \nTech Support at techsupport@vizgen.com.\n\nPlease include VPT in your subject line along with the above information in the body.\n\n## Contributing & Code of Conduct\n\nWe welcome code contributions! Please refer to the [contribution guide](CONTRIBUTING.md) before getting started.\n\n## Authors\n\n- [Vizgen](https://vizgen.com/)\n\n![Logo](https://vizgen.com/wp-content/uploads/2022/12/Vizgen-Logo_Vizgen-BlackColor-.png)\n\n## License\n\n   Copyright 2022 Vizgen, Inc. All Rights Reserved\n   \n   Licensed under the Apache License, Version 2.0 (the "License");\n   you may not use this file except in compliance with the License.\n   You may obtain a copy of the License at\n\n       http://www.apache.org/licenses/LICENSE-2.0\n\n   Unless required by applicable law or agreed to in writing, software\n   distributed under the License is distributed on an "AS IS" BASIS,\n   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.\n   See the License for the specific language governing permissions and\n   limitations under the License.\n',
-    'author': 'Vizgen',
-    'author_email': 'techsupport@vizgen.com',
-    'maintainer': 'Timothy Wiggin',
-    'maintainer_email': 'timothy.wiggin@vizgen.com',
-    'url': 'https://github.com/Vizgen/vizgen-postprocessing',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.9,<3.11',
-}
-
-
-setup(**setup_kwargs)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

