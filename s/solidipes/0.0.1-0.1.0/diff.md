# Comparing `tmp/solidipes-0.0.1.tar.gz` & `tmp/solidipes-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solidipes-0.0.1.tar", max compression
+gzip compressed data, was "solidipes-0.1.0.tar", max compression
```

## Comparing `solidipes-0.0.1.tar` & `solidipes-0.1.0.tar`

### file list

```diff
@@ -1,12 +1,43 @@
--rw-r--r--   0        0        0      371 2023-02-13 08:33:42.911733 solidipes-0.0.1/README.md
--rw-r--r--   0        0        0     1081 2023-02-13 08:33:52.497503 solidipes-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      213 2023-02-13 08:33:42.913733 solidipes-0.0.1/solidipes/__init__.py
--rw-r--r--   0        0        0       91 2023-02-13 08:33:42.913733 solidipes-0.0.1/solidipes/__main__.py
--rw-r--r--   0        0        0      561 2023-02-13 08:33:42.913733 solidipes-0.0.1/solidipes/converters.py
--rw-r--r--   0        0        0      662 2023-02-13 08:33:42.913733 solidipes-0.0.1/solidipes/datas.py
--rw-r--r--   0        0        0     1333 2023-02-13 08:33:42.913733 solidipes-0.0.1/solidipes/files.py
--rw-r--r--   0        0        0        0 2023-02-13 08:33:42.913733 solidipes-0.0.1/solidipes/scripts/__init__.py
--rw-r--r--   0        0        0      393 2023-02-13 08:33:42.913733 solidipes-0.0.1/solidipes/singleton.py
--rw-r--r--   0        0        0     1794 2023-02-13 08:33:42.913733 solidipes-0.0.1/solidipes/viewerBackends.py
--rw-r--r--   0        0        0     1109 2023-02-13 08:33:42.914733 solidipes-0.0.1/solidipes/viewers.py
--rw-r--r--   0        0        0      988 1970-01-01 00:00:00.000000 solidipes-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-04-26 08:20:35.882224 solidipes-0.1.0/README.md
+-rw-r--r--   0        0        0     1933 2023-04-26 10:58:20.785076 solidipes-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      163 2023-04-26 10:58:20.785076 solidipes-0.1.0/solidipes/__init__.py
+-rw-r--r--   0        0        0      505 2023-04-26 08:20:35.886224 solidipes-0.1.0/solidipes/config.py
+-rw-r--r--   0        0        0      446 2023-04-26 08:20:35.886224 solidipes-0.1.0/solidipes/loaders/__init__.py
+-rw-r--r--   0        0        0      559 2023-04-26 08:20:35.886224 solidipes-0.1.0/solidipes/loaders/binary.py
+-rw-r--r--   0        0        0      384 2023-04-26 08:20:35.886224 solidipes-0.1.0/solidipes/loaders/code_snippet.py
+-rw-r--r--   0        0        0     4220 2023-04-26 08:20:35.886224 solidipes-0.1.0/solidipes/loaders/data_container.py
+-rw-r--r--   0        0        0     2419 2023-04-26 08:20:35.886224 solidipes-0.1.0/solidipes/loaders/file.py
+-rw-r--r--   0        0        0      386 2023-04-26 08:42:13.550032 solidipes-0.1.0/solidipes/loaders/geof_mesh.py
+-rw-r--r--   0        0        0      427 2023-04-26 08:20:35.886224 solidipes-0.1.0/solidipes/loaders/image.py
+-rw-r--r--   0        0        0      337 2023-04-26 08:20:35.886224 solidipes-0.1.0/solidipes/loaders/meshio.py
+-rw-r--r--   0        0        0    75141 2023-04-26 08:20:35.886224 solidipes-0.1.0/solidipes/loaders/mime_types.py
+-rw-r--r--   0        0        0     6583 2023-04-26 08:20:35.886224 solidipes-0.1.0/solidipes/loaders/parse_inp.py
+-rw-r--r--   0        0        0     5175 2023-04-26 08:20:35.886224 solidipes-0.1.0/solidipes/loaders/pyvista_mesh.py
+-rw-r--r--   0        0        0     1660 2023-04-26 08:20:35.886224 solidipes-0.1.0/solidipes/loaders/table.py
+-rw-r--r--   0        0        0      791 2023-04-26 08:20:35.886224 solidipes-0.1.0/solidipes/loaders/text.py
+-rw-r--r--   0        0        0        0 2023-04-26 10:58:10.988837 solidipes-0.1.0/solidipes/reports/__init__.py
+-rw-r--r--   0        0        0     2559 2023-04-26 09:27:37.848878 solidipes-0.1.0/solidipes/reports/curation.py
+-rw-r--r--   0        0        0     6516 2023-04-26 08:20:35.886224 solidipes-0.1.0/solidipes/reports/jtcam.py
+-rw-r--r--   0        0        0     8405 2023-04-26 08:20:35.886224 solidipes-0.1.0/solidipes/reports/jtcam_small_logo.png
+-rw-r--r--   0        0        0    28449 2023-04-26 08:20:35.890224 solidipes-0.1.0/solidipes/reports/jupyter_logo.png
+-rw-r--r--   0        0        0    28462 2023-04-26 08:20:35.890224 solidipes-0.1.0/solidipes/reports/web_report.py
+-rw-r--r--   0        0        0     2314 2023-04-26 08:20:35.890224 solidipes-0.1.0/solidipes/scanners/scanner.py
+-rw-r--r--   0        0        0        0 2023-04-26 10:58:10.988837 solidipes-0.1.0/solidipes/scripts/__init__.py
+-rw-r--r--   0        0        0     2655 2023-04-26 08:20:35.890224 solidipes-0.1.0/solidipes/scripts/download.py
+-rw-r--r--   0        0        0     1275 2023-04-26 08:20:35.890224 solidipes-0.1.0/solidipes/scripts/generate_report.py
+-rw-r--r--   0        0        0     3145 2023-04-26 08:20:35.890224 solidipes-0.1.0/solidipes/scripts/init.py
+-rw-r--r--   0        0        0      990 2023-04-26 08:20:35.890224 solidipes-0.1.0/solidipes/scripts/main.py
+-rw-r--r--   0        0        0      817 2023-04-26 08:20:35.890224 solidipes-0.1.0/solidipes/scripts/quick_view.py
+-rw-r--r--   0        0        0     8574 2023-04-26 08:20:35.890224 solidipes-0.1.0/solidipes/scripts/upload.py
+-rw-r--r--   0        0        0     4858 2023-04-26 08:20:35.890224 solidipes-0.1.0/solidipes/utils.py
+-rw-r--r--   0        0        0     1528 2023-04-26 08:20:35.890224 solidipes-0.1.0/solidipes/viewer_backends.py
+-rw-r--r--   0        0        0      355 2023-04-26 08:20:35.890224 solidipes-0.1.0/solidipes/viewers/__init__.py
+-rw-r--r--   0        0        0     1256 2023-04-26 08:20:35.890224 solidipes-0.1.0/solidipes/viewers/binary.py
+-rw-r--r--   0        0        0      916 2023-04-26 08:20:35.890224 solidipes-0.1.0/solidipes/viewers/code_snippet.py
+-rw-r--r--   0        0        0      830 2023-04-26 08:20:35.890224 solidipes-0.1.0/solidipes/viewers/image.py
+-rw-r--r--   0        0        0     3819 2023-04-26 08:20:35.890224 solidipes-0.1.0/solidipes/viewers/pyvista_plotter.py
+-rw-r--r--   0        0        0     3090 2023-04-26 08:20:35.890224 solidipes-0.1.0/solidipes/viewers/table.py
+-rw-r--r--   0        0        0     1670 2023-04-26 08:20:35.890224 solidipes-0.1.0/solidipes/viewers/text.py
+-rw-r--r--   0        0        0     2223 2023-04-26 08:20:35.890224 solidipes-0.1.0/solidipes/viewers/viewer.py
+-rw-r--r--   0        0        0     7510 2023-04-26 08:20:35.890224 solidipes-0.1.0/solidipes/zenodo_utils.py
+-rw-r--r--   0        0        0     2775 1970-01-01 00:00:00.000000 solidipes-0.1.0/PKG-INFO
```

