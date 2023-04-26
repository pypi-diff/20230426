# Comparing `tmp/img2table-0.1.0.tar.gz` & `tmp/img2table-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/img2table-0.1.0.tar", last modified: Thu Apr 20 06:49:02 2023, max compression
+gzip compressed data, was "dist/img2table-0.1.1.tar", last modified: Tue Apr 25 21:53:46 2023, max compression
```

## Comparing `img2table-0.1.0.tar` & `img2table-0.1.1.tar`

### file list

```diff
@@ -1,276 +1,275 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-20 06:47:06.000000 img2table-0.1.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-20 06:47:06.000000 img2table-0.1.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-20 06:47:06.000000 img2table-0.1.0/.github/workflows/test_workflow.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-20 06:47:06.000000 img2table-0.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-20 06:47:06.000000 img2table-0.1.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    19971 2023-04-20 06:49:02.000000 img2table-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15939 2023-04-20 06:47:06.000000 img2table-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-20 06:47:06.000000 img2table-0.1.0/activate_venv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)    46045 2023-04-20 06:47:06.000000 img2table-0.1.0/examples/Basic_usage.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    33194 2023-04-20 06:47:06.000000 img2table-0.1.0/examples/Implicit_rows.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    18538 2023-04-20 06:47:06.000000 img2table-0.1.0/examples/borderless.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/examples/data/
--rw-r--r--   0 runner    (1001) docker     (123)    71022 2023-04-20 06:47:06.000000 img2table-0.1.0/examples/data/borderless_aws.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   690012 2023-04-20 06:47:06.000000 img2table-0.1.0/examples/data/borderless_ocr.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    16285 2023-04-20 06:47:06.000000 img2table-0.1.0/examples/data/implicit.png
--rw-r--r--   0 runner    (1001) docker     (123)   170804 2023-04-20 06:47:06.000000 img2table-0.1.0/examples/data/tables.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-20 06:47:06.000000 img2table-0.1.0/examples/data/tables.png
--rw-r--r--   0 runner    (1001) docker     (123)     7815 2023-04-20 06:47:06.000000 img2table-0.1.0/examples/data/tables.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-20 06:47:06.000000 img2table-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-20 06:47:06.000000 img2table-0.1.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-20 06:47:06.000000 img2table-0.1.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-20 06:47:06.000000 img2table-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-20 06:49:02.000000 img2table-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-20 06:47:06.000000 img2table-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/src/img2table/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/src/img2table/document/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/document/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/src/img2table/document/base/
--rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/document/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8907 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/document/base/rotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/document/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/document/pdf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/src/img2table/ocr/
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/ocr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/ocr/aws_textract.py
--rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/ocr/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/ocr/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/ocr/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     9906 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/ocr/google_vision.py
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/ocr/paddle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/ocr/pdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/ocr/tesseract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/src/img2table/tables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6113 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/tables/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/tables/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/src/img2table/tables/objects/
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/tables/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/tables/objects/cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/tables/objects/extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/tables/objects/line.py
--rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/tables/objects/row.py
--rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/tables/objects/table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/src/img2table/tables/processing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/tables/processing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/src/img2table/tables/processing/bordered_tables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/tables/processing/bordered_tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/src/img2table/tables/processing/bordered_tables/cells/
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/tables/processing/bordered_tables/cells/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/tables/processing/bordered_tables/cells/deduplication.py
--rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/tables/processing/bordered_tables/cells/identification.py
--rw-r--r--   0 runner    (1001) docker     (123)     9033 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/tables/processing/bordered_tables/lines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/src/img2table/tables/processing/bordered_tables/tables/
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/tables/processing/bordered_tables/tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/tables/processing/bordered_tables/tables/cell_clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/tables/processing/bordered_tables/tables/implicit_rows.py
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/tables/processing/bordered_tables/tables/table_creation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/src/img2table/tables/processing/borderless_tables/
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/tables/processing/borderless_tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10001 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/tables/processing/borderless_tables/column_delimiters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/tables/processing/borderless_tables/lines.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/tables/processing/borderless_tables/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5036 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/tables/processing/borderless_tables/segment_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/src/img2table/tables/processing/borderless_tables/table/
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/tables/processing/borderless_tables/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/tables/processing/borderless_tables/table/headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/tables/processing/borderless_tables/table/table_creation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7411 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/tables/processing/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/tables/processing/prepare_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/src/img2table/tables/processing/text/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/tables/processing/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/tables/processing/text/titles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/src/img2table.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19971 2023-04-20 06:49:02.000000 img2table-0.1.0/src/img2table.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9196 2023-04-20 06:49:02.000000 img2table-0.1.0/src/img2table.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 06:49:02.000000 img2table-0.1.0/src/img2table.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 06:49:02.000000 img2table-0.1.0/src/img2table.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-20 06:49:02.000000 img2table-0.1.0/src/img2table.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-20 06:49:02.000000 img2table-0.1.0/src/img2table.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-20 06:49:02.000000 img2table-0.1.0/src/img2table.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/_mock_data/
--rw-r--r--   0 runner    (1001) docker     (123)    11590 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/_mock_data/azure.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    12108 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/_mock_data/tesseract_hocr.html
--rw-r--r--   0 runner    (1001) docker     (123)    48862 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/_mock_data/textract.json
--rw-r--r--   0 runner    (1001) docker     (123)    61360 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/_mock_data/vision.json
--rw-r--r--   0 runner    (1001) docker     (123)    15221 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/_mock_data/vision.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/document/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/document/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/document/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/document/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/document/base/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/document/base/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/document/base/test_rotation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/document/image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/document/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/document/image/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/document/image/test_data/blank.png
--rw-r--r--   0 runner    (1001) docker     (123)   346353 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/document/image/test_data/dark.png
--rw-r--r--   0 runner    (1001) docker     (123)     6176 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/document/image/test_data/expected.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/document/image/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/document/image/test_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/document/pdf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/document/pdf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/document/pdf/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)   170804 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/document/pdf/test_data/test.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/document/pdf/test_pdf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/ocr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/ocr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/ocr/aws_textract/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/ocr/aws_textract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/ocr/aws_textract/test_aws_textract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/ocr/aws_textract/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    14178 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/ocr/aws_textract/test_data/content.json
--rw-r--r--   0 runner    (1001) docker     (123)     7428 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/ocr/aws_textract/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/ocr/aws_textract/test_data/test.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/ocr/azure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/ocr/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/ocr/azure/test_azure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/ocr/azure/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/ocr/azure/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/ocr/azure/test_data/test.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/ocr/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/ocr/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/ocr/data/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/ocr/data/test_data/expected_table.json
--rw-r--r--   0 runner    (1001) docker     (123)    53989 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/ocr/data/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/ocr/data/test_data/table.json
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/ocr/data/test_ocr_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/ocr/google_vision/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/ocr/google_vision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/ocr/google_vision/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    11094 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/ocr/google_vision/test_data/expected_content.json
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/ocr/google_vision/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/ocr/google_vision/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/ocr/google_vision/test_google_vision.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/ocr/paddle/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/ocr/paddle/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/ocr/paddle/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/ocr/paddle/test_data/hocr.json
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/ocr/paddle/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/ocr/paddle/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/ocr/paddle/test_paddle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/ocr/pdf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/ocr/pdf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/ocr/pdf/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    34981 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/ocr/pdf/test_data/content.json
--rw-r--r--   0 runner    (1001) docker     (123)    13327 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/ocr/pdf/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)   170804 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/ocr/pdf/test_data/test.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/ocr/pdf/test_pdf_ocr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/ocr/tesseract/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/ocr/tesseract/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/ocr/tesseract/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/ocr/tesseract/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/ocr/tesseract/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/ocr/tesseract/test_tesseract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/tables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/tables/image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/tables/image/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/image/test_data/blank.png
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/image/test_data/expected_tables.json
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/image/test_data/ocr.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/image/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/image/test_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/image/test_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/tables/objects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/objects/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/tables/objects/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/objects/test_data/expected_tables.json
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/objects/test_data/ocr.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/objects/test_data/tables.json
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/objects/test_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/objects/test_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/objects/test_row.py
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/objects/test_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/tables/processing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/tables/processing/bordered_tables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/bordered_tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/tables/processing/bordered_tables/cells/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/bordered_tables/cells/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/bordered_tables/cells/test_cells.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/tables/processing/bordered_tables/cells/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/bordered_tables/cells/test_data/expected.csv
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/bordered_tables/cells/test_data/expected_ident_cells.csv
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/bordered_tables/cells/test_data/expected_potential_cells.csv
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/bordered_tables/cells/test_data/expected_vertical_dedup.csv
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/bordered_tables/cells/test_data/lines.json
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/bordered_tables/cells/test_deduplication_cells.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/bordered_tables/cells/test_identification_cells.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/tables/processing/bordered_tables/lines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/bordered_tables/lines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/tables/processing/bordered_tables/lines/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/bordered_tables/lines/test_data/contours.json
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/bordered_tables/lines/test_data/expected.json
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/bordered_tables/lines/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/bordered_tables/lines/test_lines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/tables/processing/bordered_tables/tables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/bordered_tables/tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/bordered_tables/tables/test_cell_clustering.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/tables/processing/bordered_tables/tables/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/bordered_tables/tables/test_data/cell_clusters_normalized.json
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/bordered_tables/tables/test_data/cells.json
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/bordered_tables/tables/test_data/cells_clustered.json
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/bordered_tables/tables/test_data/expected.json
--rw-r--r--   0 runner    (1001) docker     (123)    11661 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/bordered_tables/tables/test_data/implicit.png
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/bordered_tables/tables/test_data/implicit_table.json
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/bordered_tables/tables/test_data/tables_from_cells.json
--rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/bordered_tables/tables/test_data/word_image.png
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/bordered_tables/tables/test_implicit_rows.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/bordered_tables/tables/test_table_creation.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/bordered_tables/tables/test_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/tables/processing/borderless_tables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/borderless_tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/tables/processing/borderless_tables/borderless_table/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/borderless_tables/borderless_table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/borderless_tables/borderless_table/test_borderless_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/tables/processing/borderless_tables/borderless_table/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/borderless_tables/borderless_table/test_data/lines.json
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/borderless_tables/borderless_table/test_data/test.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/tables/processing/borderless_tables/column_delimiters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/borderless_tables/column_delimiters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/borderless_tables/column_delimiters/test_column_delimiters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/tables/processing/borderless_tables/lines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/borderless_tables/lines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/tables/processing/borderless_tables/lines/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/borderless_tables/lines/test_data/image_segment.json
--rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/borderless_tables/lines/test_lines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/tables/processing/borderless_tables/segment_image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/borderless_tables/segment_image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/tables/processing/borderless_tables/segment_image/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/borderless_tables/segment_image/test_data/lines.json
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/borderless_tables/segment_image/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/borderless_tables/segment_image/test_segment_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/tables/processing/borderless_tables/table/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/borderless_tables/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12264 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/borderless_tables/table/test_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/borderless_tables/table/test_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/borderless_tables/table/test_table_creation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/tables/processing/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/common/test_common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/tables/processing/common/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    29496 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/common/test_data/test.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/tables/processing/prepare_image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/prepare_image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/tables/processing/prepare_image/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    20769 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/prepare_image/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/prepare_image/test_prepare_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/tables/processing/text/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/text/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/tables/processing/text/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    17822 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/text/test_data/ocr.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/text/test_data/table.json
--rw-r--r--   0 runner    (1001) docker     (123)   219573 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/text/test_data/test.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/text/test_titles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:53:46.000000 img2table-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:53:46.000000 img2table-0.1.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-25 21:51:05.000000 img2table-0.1.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:53:46.000000 img2table-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-25 21:51:05.000000 img2table-0.1.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-25 21:51:05.000000 img2table-0.1.1/.github/workflows/test_workflow.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-25 21:51:05.000000 img2table-0.1.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-25 21:51:05.000000 img2table-0.1.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    19699 2023-04-25 21:53:46.000000 img2table-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15723 2023-04-25 21:51:05.000000 img2table-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-25 21:51:05.000000 img2table-0.1.1/activate_venv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:53:46.000000 img2table-0.1.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    46045 2023-04-25 21:51:05.000000 img2table-0.1.1/examples/Basic_usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    33194 2023-04-25 21:51:05.000000 img2table-0.1.1/examples/Implicit_rows.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    18538 2023-04-25 21:51:05.000000 img2table-0.1.1/examples/borderless.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:53:46.000000 img2table-0.1.1/examples/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    71022 2023-04-25 21:51:05.000000 img2table-0.1.1/examples/data/borderless_aws.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   690012 2023-04-25 21:51:05.000000 img2table-0.1.1/examples/data/borderless_ocr.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    16285 2023-04-25 21:51:05.000000 img2table-0.1.1/examples/data/implicit.png
+-rw-r--r--   0 runner    (1001) docker     (123)   170804 2023-04-25 21:51:05.000000 img2table-0.1.1/examples/data/tables.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-25 21:51:05.000000 img2table-0.1.1/examples/data/tables.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7815 2023-04-25 21:51:05.000000 img2table-0.1.1/examples/data/tables.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-25 21:51:05.000000 img2table-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-25 21:51:05.000000 img2table-0.1.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-25 21:51:05.000000 img2table-0.1.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-25 21:51:05.000000 img2table-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-25 21:53:46.000000 img2table-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-25 21:51:05.000000 img2table-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:53:46.000000 img2table-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:53:46.000000 img2table-0.1.1/src/img2table/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-25 21:51:05.000000 img2table-0.1.1/src/img2table/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:53:46.000000 img2table-0.1.1/src/img2table/document/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-25 21:51:05.000000 img2table-0.1.1/src/img2table/document/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:53:46.000000 img2table-0.1.1/src/img2table/document/base/
+-rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-04-25 21:51:05.000000 img2table-0.1.1/src/img2table/document/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9009 2023-04-25 21:51:05.000000 img2table-0.1.1/src/img2table/document/base/rotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-04-25 21:51:05.000000 img2table-0.1.1/src/img2table/document/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-04-25 21:51:05.000000 img2table-0.1.1/src/img2table/document/pdf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:53:46.000000 img2table-0.1.1/src/img2table/ocr/
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-25 21:51:05.000000 img2table-0.1.1/src/img2table/ocr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-04-25 21:51:05.000000 img2table-0.1.1/src/img2table/ocr/aws_textract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-04-25 21:51:05.000000 img2table-0.1.1/src/img2table/ocr/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-25 21:51:05.000000 img2table-0.1.1/src/img2table/ocr/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-04-25 21:51:05.000000 img2table-0.1.1/src/img2table/ocr/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9906 2023-04-25 21:51:05.000000 img2table-0.1.1/src/img2table/ocr/google_vision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-04-25 21:51:05.000000 img2table-0.1.1/src/img2table/ocr/paddle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-04-25 21:51:05.000000 img2table-0.1.1/src/img2table/ocr/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-04-25 21:51:05.000000 img2table-0.1.1/src/img2table/ocr/tesseract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:53:46.000000 img2table-0.1.1/src/img2table/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:51:05.000000 img2table-0.1.1/src/img2table/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6113 2023-04-25 21:51:05.000000 img2table-0.1.1/src/img2table/tables/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5700 2023-04-25 21:51:05.000000 img2table-0.1.1/src/img2table/tables/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:53:46.000000 img2table-0.1.1/src/img2table/tables/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-25 21:51:05.000000 img2table-0.1.1/src/img2table/tables/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-25 21:51:05.000000 img2table-0.1.1/src/img2table/tables/objects/cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-04-25 21:51:05.000000 img2table-0.1.1/src/img2table/tables/objects/extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-25 21:51:05.000000 img2table-0.1.1/src/img2table/tables/objects/line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-04-25 21:51:05.000000 img2table-0.1.1/src/img2table/tables/objects/row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-04-25 21:51:05.000000 img2table-0.1.1/src/img2table/tables/objects/table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:53:46.000000 img2table-0.1.1/src/img2table/tables/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:51:05.000000 img2table-0.1.1/src/img2table/tables/processing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:53:46.000000 img2table-0.1.1/src/img2table/tables/processing/bordered_tables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:51:05.000000 img2table-0.1.1/src/img2table/tables/processing/bordered_tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:53:46.000000 img2table-0.1.1/src/img2table/tables/processing/bordered_tables/cells/
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-25 21:51:05.000000 img2table-0.1.1/src/img2table/tables/processing/bordered_tables/cells/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-04-25 21:51:05.000000 img2table-0.1.1/src/img2table/tables/processing/bordered_tables/cells/deduplication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-04-25 21:51:05.000000 img2table-0.1.1/src/img2table/tables/processing/bordered_tables/cells/identification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11387 2023-04-25 21:51:05.000000 img2table-0.1.1/src/img2table/tables/processing/bordered_tables/lines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:53:46.000000 img2table-0.1.1/src/img2table/tables/processing/bordered_tables/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-04-25 21:51:05.000000 img2table-0.1.1/src/img2table/tables/processing/bordered_tables/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-04-25 21:51:05.000000 img2table-0.1.1/src/img2table/tables/processing/bordered_tables/tables/cell_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-04-25 21:51:05.000000 img2table-0.1.1/src/img2table/tables/processing/bordered_tables/tables/implicit_rows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-04-25 21:51:05.000000 img2table-0.1.1/src/img2table/tables/processing/bordered_tables/tables/table_creation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:53:46.000000 img2table-0.1.1/src/img2table/tables/processing/borderless_tables/
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-04-25 21:51:05.000000 img2table-0.1.1/src/img2table/tables/processing/borderless_tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10001 2023-04-25 21:51:05.000000 img2table-0.1.1/src/img2table/tables/processing/borderless_tables/column_delimiters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-04-25 21:51:05.000000 img2table-0.1.1/src/img2table/tables/processing/borderless_tables/lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-04-25 21:51:05.000000 img2table-0.1.1/src/img2table/tables/processing/borderless_tables/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5036 2023-04-25 21:51:05.000000 img2table-0.1.1/src/img2table/tables/processing/borderless_tables/segment_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:53:46.000000 img2table-0.1.1/src/img2table/tables/processing/borderless_tables/table/
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-04-25 21:51:05.000000 img2table-0.1.1/src/img2table/tables/processing/borderless_tables/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-04-25 21:51:05.000000 img2table-0.1.1/src/img2table/tables/processing/borderless_tables/table/headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-04-25 21:51:05.000000 img2table-0.1.1/src/img2table/tables/processing/borderless_tables/table/table_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7411 2023-04-25 21:51:05.000000 img2table-0.1.1/src/img2table/tables/processing/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-04-25 21:51:05.000000 img2table-0.1.1/src/img2table/tables/processing/prepare_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:53:46.000000 img2table-0.1.1/src/img2table/tables/processing/text/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:51:05.000000 img2table-0.1.1/src/img2table/tables/processing/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-04-25 21:51:05.000000 img2table-0.1.1/src/img2table/tables/processing/text/titles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:53:46.000000 img2table-0.1.1/src/img2table.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19699 2023-04-25 21:53:46.000000 img2table-0.1.1/src/img2table.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9146 2023-04-25 21:53:46.000000 img2table-0.1.1/src/img2table.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 21:53:46.000000 img2table-0.1.1/src/img2table.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 21:53:46.000000 img2table-0.1.1/src/img2table.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-25 21:53:46.000000 img2table-0.1.1/src/img2table.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-25 21:53:46.000000 img2table-0.1.1/src/img2table.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-25 21:53:46.000000 img2table-0.1.1/src/img2table.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:53:46.000000 img2table-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:53:46.000000 img2table-0.1.1/tests/_mock_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    11590 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/_mock_data/azure.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    12108 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/_mock_data/tesseract_hocr.html
+-rw-r--r--   0 runner    (1001) docker     (123)    48862 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/_mock_data/textract.json
+-rw-r--r--   0 runner    (1001) docker     (123)    61360 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/_mock_data/vision.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15221 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/_mock_data/vision.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:53:46.000000 img2table-0.1.1/tests/document/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/document/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:53:46.000000 img2table-0.1.1/tests/document/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/document/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:53:46.000000 img2table-0.1.1/tests/document/base/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/document/base/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/document/base/test_rotation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:53:46.000000 img2table-0.1.1/tests/document/image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/document/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:53:46.000000 img2table-0.1.1/tests/document/image/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/document/image/test_data/blank.png
+-rw-r--r--   0 runner    (1001) docker     (123)   346353 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/document/image/test_data/dark.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6176 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/document/image/test_data/expected.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/document/image/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/document/image/test_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:53:46.000000 img2table-0.1.1/tests/document/pdf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/document/pdf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:53:46.000000 img2table-0.1.1/tests/document/pdf/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)   170804 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/document/pdf/test_data/test.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/document/pdf/test_pdf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:53:46.000000 img2table-0.1.1/tests/ocr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/ocr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:53:46.000000 img2table-0.1.1/tests/ocr/aws_textract/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/ocr/aws_textract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/ocr/aws_textract/test_aws_textract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:53:46.000000 img2table-0.1.1/tests/ocr/aws_textract/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    14178 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/ocr/aws_textract/test_data/content.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7428 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/ocr/aws_textract/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/ocr/aws_textract/test_data/test.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:53:46.000000 img2table-0.1.1/tests/ocr/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/ocr/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/ocr/azure/test_azure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:53:46.000000 img2table-0.1.1/tests/ocr/azure/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/ocr/azure/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/ocr/azure/test_data/test.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:53:46.000000 img2table-0.1.1/tests/ocr/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/ocr/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:53:46.000000 img2table-0.1.1/tests/ocr/data/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/ocr/data/test_data/expected_table.json
+-rw-r--r--   0 runner    (1001) docker     (123)    53989 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/ocr/data/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/ocr/data/test_data/table.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/ocr/data/test_ocr_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:53:46.000000 img2table-0.1.1/tests/ocr/google_vision/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/ocr/google_vision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:53:46.000000 img2table-0.1.1/tests/ocr/google_vision/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    11094 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/ocr/google_vision/test_data/expected_content.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/ocr/google_vision/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/ocr/google_vision/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/ocr/google_vision/test_google_vision.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:53:46.000000 img2table-0.1.1/tests/ocr/paddle/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/ocr/paddle/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:53:46.000000 img2table-0.1.1/tests/ocr/paddle/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/ocr/paddle/test_data/hocr.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/ocr/paddle/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/ocr/paddle/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/ocr/paddle/test_paddle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:53:46.000000 img2table-0.1.1/tests/ocr/pdf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/ocr/pdf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:53:46.000000 img2table-0.1.1/tests/ocr/pdf/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    34981 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/ocr/pdf/test_data/content.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13327 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/ocr/pdf/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   170804 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/ocr/pdf/test_data/test.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/ocr/pdf/test_pdf_ocr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:53:46.000000 img2table-0.1.1/tests/ocr/tesseract/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/ocr/tesseract/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:53:46.000000 img2table-0.1.1/tests/ocr/tesseract/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/ocr/tesseract/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/ocr/tesseract/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/ocr/tesseract/test_tesseract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:53:46.000000 img2table-0.1.1/tests/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:53:46.000000 img2table-0.1.1/tests/tables/image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/tables/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:53:46.000000 img2table-0.1.1/tests/tables/image/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/tables/image/test_data/blank.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/tables/image/test_data/ocr.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/tables/image/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/tables/image/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/tables/image/test_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:53:46.000000 img2table-0.1.1/tests/tables/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/tables/objects/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:53:46.000000 img2table-0.1.1/tests/tables/objects/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/tables/objects/test_data/expected_tables.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/tables/objects/test_data/ocr.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/tables/objects/test_data/tables.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/tables/objects/test_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/tables/objects/test_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/tables/objects/test_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/tables/objects/test_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:53:46.000000 img2table-0.1.1/tests/tables/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/tables/processing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:53:46.000000 img2table-0.1.1/tests/tables/processing/bordered_tables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/tables/processing/bordered_tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:53:46.000000 img2table-0.1.1/tests/tables/processing/bordered_tables/cells/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/tables/processing/bordered_tables/cells/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/tables/processing/bordered_tables/cells/test_cells.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:53:46.000000 img2table-0.1.1/tests/tables/processing/bordered_tables/cells/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/tables/processing/bordered_tables/cells/test_data/expected.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/tables/processing/bordered_tables/cells/test_data/expected_ident_cells.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/tables/processing/bordered_tables/cells/test_data/expected_potential_cells.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/tables/processing/bordered_tables/cells/test_data/expected_vertical_dedup.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/tables/processing/bordered_tables/cells/test_data/lines.json
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/tables/processing/bordered_tables/cells/test_deduplication_cells.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/tables/processing/bordered_tables/cells/test_identification_cells.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:53:46.000000 img2table-0.1.1/tests/tables/processing/bordered_tables/lines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/tables/processing/bordered_tables/lines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:53:46.000000 img2table-0.1.1/tests/tables/processing/bordered_tables/lines/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/tables/processing/bordered_tables/lines/test_data/contours.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/tables/processing/bordered_tables/lines/test_data/expected.json
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/tables/processing/bordered_tables/lines/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/tables/processing/bordered_tables/lines/test_lines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:53:46.000000 img2table-0.1.1/tests/tables/processing/bordered_tables/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/tables/processing/bordered_tables/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/tables/processing/bordered_tables/tables/test_cell_clustering.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:53:46.000000 img2table-0.1.1/tests/tables/processing/bordered_tables/tables/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/tables/processing/bordered_tables/tables/test_data/cell_clusters_normalized.json
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/tables/processing/bordered_tables/tables/test_data/cells.json
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/tables/processing/bordered_tables/tables/test_data/cells_clustered.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/tables/processing/bordered_tables/tables/test_data/expected.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11661 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/tables/processing/bordered_tables/tables/test_data/implicit.png
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/tables/processing/bordered_tables/tables/test_data/implicit_table.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/tables/processing/bordered_tables/tables/test_data/tables_from_cells.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/tables/processing/bordered_tables/tables/test_data/word_image.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/tables/processing/bordered_tables/tables/test_implicit_rows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/tables/processing/bordered_tables/tables/test_table_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/tables/processing/bordered_tables/tables/test_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:53:46.000000 img2table-0.1.1/tests/tables/processing/borderless_tables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/tables/processing/borderless_tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:53:46.000000 img2table-0.1.1/tests/tables/processing/borderless_tables/borderless_table/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/tables/processing/borderless_tables/borderless_table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/tables/processing/borderless_tables/borderless_table/test_borderless_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:53:46.000000 img2table-0.1.1/tests/tables/processing/borderless_tables/borderless_table/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/tables/processing/borderless_tables/borderless_table/test_data/lines.json
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/tables/processing/borderless_tables/borderless_table/test_data/test.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:53:46.000000 img2table-0.1.1/tests/tables/processing/borderless_tables/column_delimiters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/tables/processing/borderless_tables/column_delimiters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/tables/processing/borderless_tables/column_delimiters/test_column_delimiters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:53:46.000000 img2table-0.1.1/tests/tables/processing/borderless_tables/lines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/tables/processing/borderless_tables/lines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:53:46.000000 img2table-0.1.1/tests/tables/processing/borderless_tables/lines/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/tables/processing/borderless_tables/lines/test_data/image_segment.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/tables/processing/borderless_tables/lines/test_lines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:53:46.000000 img2table-0.1.1/tests/tables/processing/borderless_tables/segment_image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/tables/processing/borderless_tables/segment_image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:53:46.000000 img2table-0.1.1/tests/tables/processing/borderless_tables/segment_image/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/tables/processing/borderless_tables/segment_image/test_data/lines.json
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/tables/processing/borderless_tables/segment_image/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/tables/processing/borderless_tables/segment_image/test_segment_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:53:46.000000 img2table-0.1.1/tests/tables/processing/borderless_tables/table/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/tables/processing/borderless_tables/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12264 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/tables/processing/borderless_tables/table/test_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/tables/processing/borderless_tables/table/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/tables/processing/borderless_tables/table/test_table_creation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:53:46.000000 img2table-0.1.1/tests/tables/processing/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/tables/processing/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/tables/processing/common/test_common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:53:46.000000 img2table-0.1.1/tests/tables/processing/common/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    29496 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/tables/processing/common/test_data/test.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:53:46.000000 img2table-0.1.1/tests/tables/processing/prepare_image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/tables/processing/prepare_image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:53:46.000000 img2table-0.1.1/tests/tables/processing/prepare_image/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    20769 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/tables/processing/prepare_image/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/tables/processing/prepare_image/test_prepare_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:53:46.000000 img2table-0.1.1/tests/tables/processing/text/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/tables/processing/text/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:53:46.000000 img2table-0.1.1/tests/tables/processing/text/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    17822 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/tables/processing/text/test_data/ocr.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/tables/processing/text/test_data/table.json
+-rw-r--r--   0 runner    (1001) docker     (123)   219573 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/tables/processing/text/test_data/test.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-25 21:51:05.000000 img2table-0.1.1/tests/tables/processing/text/test_titles.py
```

### Comparing `img2table-0.1.0/LICENSE.txt` & `img2table-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/Makefile` & `img2table-0.1.1/Makefile`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/PKG-INFO` & `img2table-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: img2table
-Version: 0.1.0
+Version: 0.1.1
 Summary: img2table is a table identification and extraction Python Library for PDF and images, based on OpenCV image processing
 Home-page: https://github.com/xavctn/img2table
 Author: Xavier Canton
 License: MIT
 Description: # img2table
         
         `img2table` is a simple, easy to use, table identification and extraction Python Library based on [OpenCV](https://opencv.org/) image 
@@ -12,26 +12,19 @@
         
         Thanks to its design, it provides a practical and lighter alternative to Neural Networks based solutions, especially for usage on CPU.
         
         ## Table of contents
         * [Installation](#installation)
         * [Features](#features)
         * [Supported file formats](#supported-file-formats)
-           * [Images](#images-formats)
-           * [PDF](#pdf-formats)
         * [Usage](#usage)
            * [Documents](#documents)
               * [Images](#images-doc)
               * [PDF](#pdf-doc)
-           * [OCR](#ocr)
-              * [Tesseract](#tesseract)
-              * [PaddleOCR](#paddle)
-              * [Google Vision](#vision)
-              * [AWS Textract](#textract)
-              * [Azure Cognitive Services](#azure)
+           * [Supported OCRs](#ocr)
            * [Table extraction](#table-extract)
            * [Excel export](#xlsx)
         * [Examples](#examples)
         * [Caveats / FYI](#fyi)
         
         
         ## Installation <a name="installation"></a>
```

#### html2text {}

```diff
@@ -1,38 +1,36 @@
-Metadata-Version: 2.1 Name: img2table Version: 0.1.0 Summary: img2table is a
+Metadata-Version: 2.1 Name: img2table Version: 0.1.1 Summary: img2table is a
 table identification and extraction Python Library for PDF and images, based on
 OpenCV image processing Home-page: https://github.com/xavctn/img2table Author:
 Xavier Canton License: MIT Description: # img2table `img2table` is a simple,
 easy to use, table identification and extraction Python Library based on
 [OpenCV](https://opencv.org/) image processing that supports most common image
 file formats as well as PDF files. Thanks to its design, it provides a
 practical and lighter alternative to Neural Networks based solutions,
 especially for usage on CPU. ## Table of contents * [Installation]
 (#installation) * [Features](#features) * [Supported file formats](#supported-
-file-formats) * [Images](#images-formats) * [PDF](#pdf-formats) * [Usage]
-(#usage) * [Documents](#documents) * [Images](#images-doc) * [PDF](#pdf-doc) *
-[OCR](#ocr) * [Tesseract](#tesseract) * [PaddleOCR](#paddle) * [Google Vision]
-(#vision) * [AWS Textract](#textract) * [Azure Cognitive Services](#azure) *
-[Table extraction](#table-extract) * [Excel export](#xlsx) * [Examples]
-(#examples) * [Caveats / FYI](#fyi) ## Installation  The library can be
-installed via pip. ```python # Standard installation, supporting Tesseract pip
-install img2table # For usage with Paddle OCR (Python <= 3.10 only) pip install
-img2table[paddle] # For usage with Paddle OCR - GPU (CUDA 9 / CUDA 10) (Python
-<= 3.10 only) pip install img2table[paddle-gpu] # For usage with Google Vision
-OCR pip install img2table[gcp] # For usage with AWS Textract OCR pip install
-img2table[aws] # For usage with Azure Cognitive Services OCR pip install
-img2table[azure] ``` ## Features  * Table identification for images and PDF
-files, including bounding boxes at the table cell level * Handling of complex
-table structures such as merged cells * Handling of implicit rows - see
-[example](/examples/Implicit_rows.ipynb) * Table content extraction by
-providing support for OCR services / tools * Extracted tables are returned as a
-simple object, including a Pandas DataFrame representation * Export extracted
-tables to an Excel file, preserving their original structure ## Supported file
-formats  ### Images  Images are loaded using the `opencv-python` library,
-supported formats are listed below.  Supported image formats
+file-formats) * [Usage](#usage) * [Documents](#documents) * [Images](#images-
+doc) * [PDF](#pdf-doc) * [Supported OCRs](#ocr) * [Table extraction](#table-
+extract) * [Excel export](#xlsx) * [Examples](#examples) * [Caveats / FYI]
+(#fyi) ## Installation  The library can be installed via pip. ```python #
+Standard installation, supporting Tesseract pip install img2table # For usage
+with Paddle OCR (Python <= 3.10 only) pip install img2table[paddle] # For usage
+with Paddle OCR - GPU (CUDA 9 / CUDA 10) (Python <= 3.10 only) pip install
+img2table[paddle-gpu] # For usage with Google Vision OCR pip install img2table
+[gcp] # For usage with AWS Textract OCR pip install img2table[aws] # For usage
+with Azure Cognitive Services OCR pip install img2table[azure] ``` ## Features
+* Table identification for images and PDF files, including bounding boxes at
+the table cell level * Handling of complex table structures such as merged
+cells * Handling of implicit rows - see [example](/examples/
+Implicit_rows.ipynb) * Table content extraction by providing support for OCR
+services / tools * Extracted tables are returned as a simple object, including
+a Pandas DataFrame representation * Export extracted tables to an Excel file,
+preserving their original structure ## Supported file formats  ### Images
+Images are loaded using the `opencv-python` library, supported formats are
+listed below.  Supported image formats
          * Windows bitmaps - .bmp,.dib
          * JPEG files - .jpeg,.jpg, *.jpe
          * JPEG 2000 files - *.jp2
          * Portable Network Graphics - *.png
          * WebP - *.webp
          * Portable image format - .pbm,.pgm, .ppm.pxm, *.pnm
          * PFM files - *.pfm
```

### Comparing `img2table-0.1.0/README.md` & `img2table-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -5,26 +5,19 @@
 
 Thanks to its design, it provides a practical and lighter alternative to Neural Networks based solutions, especially for usage on CPU.
 
 ## Table of contents
 * [Installation](#installation)
 * [Features](#features)
 * [Supported file formats](#supported-file-formats)
-   * [Images](#images-formats)
-   * [PDF](#pdf-formats)
 * [Usage](#usage)
    * [Documents](#documents)
       * [Images](#images-doc)
       * [PDF](#pdf-doc)
-   * [OCR](#ocr)
-      * [Tesseract](#tesseract)
-      * [PaddleOCR](#paddle)
-      * [Google Vision](#vision)
-      * [AWS Textract](#textract)
-      * [Azure Cognitive Services](#azure)
+   * [Supported OCRs](#ocr)
    * [Table extraction](#table-extract)
    * [Excel export](#xlsx)
 * [Examples](#examples)
 * [Caveats / FYI](#fyi)
 
 
 ## Installation <a name="installation"></a>
```

#### html2text {}

```diff
@@ -1,34 +1,32 @@
 # img2table `img2table` is a simple, easy to use, table identification and
 extraction Python Library based on [OpenCV](https://opencv.org/) image
 processing that supports most common image file formats as well as PDF files.
 Thanks to its design, it provides a practical and lighter alternative to Neural
 Networks based solutions, especially for usage on CPU. ## Table of contents *
 [Installation](#installation) * [Features](#features) * [Supported file
-formats](#supported-file-formats) * [Images](#images-formats) * [PDF](#pdf-
-formats) * [Usage](#usage) * [Documents](#documents) * [Images](#images-doc) *
-[PDF](#pdf-doc) * [OCR](#ocr) * [Tesseract](#tesseract) * [PaddleOCR](#paddle)
-* [Google Vision](#vision) * [AWS Textract](#textract) * [Azure Cognitive
-Services](#azure) * [Table extraction](#table-extract) * [Excel export](#xlsx)
-* [Examples](#examples) * [Caveats / FYI](#fyi) ## Installation  The library
-can be installed via pip. ```python # Standard installation, supporting
-Tesseract pip install img2table # For usage with Paddle OCR (Python <= 3.10
-only) pip install img2table[paddle] # For usage with Paddle OCR - GPU (CUDA 9 /
-CUDA 10) (Python <= 3.10 only) pip install img2table[paddle-gpu] # For usage
-with Google Vision OCR pip install img2table[gcp] # For usage with AWS Textract
-OCR pip install img2table[aws] # For usage with Azure Cognitive Services OCR
-pip install img2table[azure] ``` ## Features  * Table identification for images
-and PDF files, including bounding boxes at the table cell level * Handling of
-complex table structures such as merged cells * Handling of implicit rows - see
-[example](/examples/Implicit_rows.ipynb) * Table content extraction by
-providing support for OCR services / tools * Extracted tables are returned as a
-simple object, including a Pandas DataFrame representation * Export extracted
-tables to an Excel file, preserving their original structure ## Supported file
-formats  ### Images  Images are loaded using the `opencv-python` library,
-supported formats are listed below.  Supported image formats
+formats](#supported-file-formats) * [Usage](#usage) * [Documents](#documents) *
+[Images](#images-doc) * [PDF](#pdf-doc) * [Supported OCRs](#ocr) * [Table
+extraction](#table-extract) * [Excel export](#xlsx) * [Examples](#examples) *
+[Caveats / FYI](#fyi) ## Installation  The library can be installed via pip.
+```python # Standard installation, supporting Tesseract pip install img2table #
+For usage with Paddle OCR (Python <= 3.10 only) pip install img2table[paddle] #
+For usage with Paddle OCR - GPU (CUDA 9 / CUDA 10) (Python <= 3.10 only) pip
+install img2table[paddle-gpu] # For usage with Google Vision OCR pip install
+img2table[gcp] # For usage with AWS Textract OCR pip install img2table[aws] #
+For usage with Azure Cognitive Services OCR pip install img2table[azure] ``` ##
+Features  * Table identification for images and PDF files, including bounding
+boxes at the table cell level * Handling of complex table structures such as
+merged cells * Handling of implicit rows - see [example](/examples/
+Implicit_rows.ipynb) * Table content extraction by providing support for OCR
+services / tools * Extracted tables are returned as a simple object, including
+a Pandas DataFrame representation * Export extracted tables to an Excel file,
+preserving their original structure ## Supported file formats  ### Images
+Images are loaded using the `opencv-python` library, supported formats are
+listed below.  Supported image formats
          * Windows bitmaps - .bmp,.dib
          * JPEG files - .jpeg,.jpg, *.jpe
          * JPEG 2000 files - *.jp2
          * Portable Network Graphics - *.png
          * WebP - *.webp
          * Portable image format - .pbm,.pgm, .ppm.pxm, *.pnm
          * PFM files - *.pfm
```

### Comparing `img2table-0.1.0/examples/Basic_usage.ipynb` & `img2table-0.1.1/examples/Basic_usage.ipynb`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/examples/Implicit_rows.ipynb` & `img2table-0.1.1/examples/Implicit_rows.ipynb`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/examples/borderless.ipynb` & `img2table-0.1.1/examples/borderless.ipynb`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/examples/data/borderless_aws.jpg` & `img2table-0.1.1/examples/data/borderless_aws.jpg`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/examples/data/borderless_ocr.jpg` & `img2table-0.1.1/examples/data/borderless_ocr.jpg`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/examples/data/implicit.png` & `img2table-0.1.1/examples/data/implicit.png`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/examples/data/tables.pdf` & `img2table-0.1.1/examples/data/tables.pdf`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/examples/data/tables.png` & `img2table-0.1.1/examples/data/tables.png`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/examples/data/tables.xlsx` & `img2table-0.1.1/examples/data/tables.xlsx`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/setup.cfg` & `img2table-0.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/src/img2table/__init__.py` & `img2table-0.1.1/src/img2table/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/src/img2table/document/base/__init__.py` & `img2table-0.1.1/src/img2table/document/base/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/src/img2table/document/base/rotation.py` & `img2table-0.1.1/src/img2table/document/base/rotation.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     df_cross = (df_centroids.join(df_centroids, how='cross')
                 .filter(pl.col('x1') != pl.col('x1_right'))
                 .filter((pl.col('y1') - pl.col('y1_right')).abs() <= 10 * ref_height)
                 )
 
     # Compute slopes and angles
     df_angles = (df_cross.with_columns(((pl.col('y1') - pl.col('y1_right')) / (pl.col('x1') - pl.col('x1_right'))
-                                        ).alias('slope'))
+                                        ).round(3).alias('slope'))
                  .with_columns((pl.col('slope').arctan() * 180 / np.pi).alias('angle'))
                  .with_columns(pl.when(pl.col('angle').abs() <= 45)
                                .then(pl.col('angle'))
                                .otherwise(pl.min(pl.col('angle') + 90, 90 - pl.col('angle')) * -pl.col('angle').sign())
                                .alias('angle')
                                )
                  )
@@ -91,16 +91,19 @@
                           .count()
                           .sort(by=['count', pl.col('angle').abs()], descending=[True, False])
                           .limit(n_max)
                           .collect(streaming=True)
                           .to_dicts()
                           )
 
-    return sorted(list(set([angle.get('angle') for angle in most_likely_angles
-                            if angle.get('count') >= 0.25 * max([a.get('count') for a in most_likely_angles])])))
+    if most_likely_angles[0].get('angle') == 0:
+        return [0]
+    else:
+        return sorted(list(set([angle.get('angle') for angle in most_likely_angles
+                                if angle.get('count') >= 0.25 * max([a.get('count') for a in most_likely_angles])])))
 
 
 def angle_dixon_q_test(angles: List[float], confidence: float = 0.9) -> float:
     """
     Compute best angle according to Dixon Q test
     :param angles: list of possible angles
     :param confidence: confidence level for outliers (0.9, 0.95, 0.99)
@@ -230,12 +233,12 @@
         return img
 
     # Compute most likely angles from connected components
     angles = get_relevant_angles(centroids=cc_centroids, ref_height=ref_height)
     # Estimate skew
     skew_angle = estimate_skew(angles=angles, thresh=thresh)
 
-    if skew_angle != 0:
+    if abs(skew_angle) >= 0.25:
         # Rotate image with borders
         return rotate_img_with_border(img=img, angle=skew_angle)
 
     return img
```

### Comparing `img2table-0.1.0/src/img2table/document/image.py` & `img2table-0.1.1/src/img2table/document/image.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/src/img2table/document/pdf.py` & `img2table-0.1.1/src/img2table/document/pdf.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/src/img2table/ocr/aws_textract.py` & `img2table-0.1.1/src/img2table/ocr/aws_textract.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/src/img2table/ocr/azure.py` & `img2table-0.1.1/src/img2table/ocr/azure.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/src/img2table/ocr/base.py` & `img2table-0.1.1/src/img2table/ocr/base.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/src/img2table/ocr/data.py` & `img2table-0.1.1/src/img2table/ocr/data.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/src/img2table/ocr/google_vision.py` & `img2table-0.1.1/src/img2table/ocr/google_vision.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/src/img2table/ocr/paddle.py` & `img2table-0.1.1/src/img2table/ocr/paddle.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/src/img2table/ocr/pdf.py` & `img2table-0.1.1/src/img2table/ocr/pdf.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/src/img2table/ocr/tesseract.py` & `img2table-0.1.1/src/img2table/ocr/tesseract.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/src/img2table/tables/image.py` & `img2table-0.1.1/src/img2table/tables/image.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/src/img2table/tables/metrics.py` & `img2table-0.1.1/src/img2table/tables/metrics.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,21 +36,26 @@
     median_width = np.median(stats[:, cv2.CC_STAT_WIDTH])
     median_height = np.median(stats[:, cv2.CC_STAT_HEIGHT])
 
     # Compute bbox area bounds
     upper_bound = 4 * median_width * median_height
     lower_bound = 0.25 * median_width * median_height
 
+    # Filter components based on aspect ratio
+    mask_lower_ar = 0.2 < stats[:, cv2.CC_STAT_WIDTH] / stats[:, cv2.CC_STAT_HEIGHT]
+    mask_upper_ar = 5 > stats[:, cv2.CC_STAT_WIDTH] / stats[:, cv2.CC_STAT_HEIGHT]
+    mask_ar = mask_lower_ar & mask_upper_ar
+
     # Filter connected components according to their area
     mask_lower_area = lower_bound < stats[:, cv2.CC_STAT_WIDTH] * stats[:, cv2.CC_STAT_HEIGHT]
     mask_upper_area = upper_bound > stats[:, cv2.CC_STAT_WIDTH] * stats[:, cv2.CC_STAT_HEIGHT]
     mask_area = mask_lower_area & mask_upper_area
 
     # Filter connected components from mask
-    stats = stats[mask_img & mask_area]
+    stats = stats[mask_img & mask_area & mask_ar]
 
     if len(stats) > 0:
         # Compute average character length
         char_length = np.mean(stats[:, cv2.CC_STAT_WIDTH])
 
         return char_length, stats
     else:
```

### Comparing `img2table-0.1.0/src/img2table/tables/objects/__init__.py` & `img2table-0.1.1/src/img2table/tables/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/src/img2table/tables/objects/extraction.py` & `img2table-0.1.1/src/img2table/tables/objects/extraction.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/src/img2table/tables/objects/line.py` & `img2table-0.1.1/src/img2table/tables/objects/line.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/src/img2table/tables/objects/row.py` & `img2table-0.1.1/src/img2table/tables/objects/row.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/src/img2table/tables/objects/table.py` & `img2table-0.1.1/src/img2table/tables/objects/table.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/src/img2table/tables/processing/bordered_tables/cells/__init__.py` & `img2table-0.1.1/src/img2table/tables/processing/bordered_tables/cells/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/src/img2table/tables/processing/bordered_tables/cells/deduplication.py` & `img2table-0.1.1/src/img2table/tables/processing/bordered_tables/cells/deduplication.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/src/img2table/tables/processing/bordered_tables/cells/identification.py` & `img2table-0.1.1/src/img2table/tables/processing/bordered_tables/cells/identification.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/src/img2table/tables/processing/bordered_tables/lines.py` & `img2table-0.1.1/src/img2table/tables/processing/bordered_tables/lines.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # coding: utf-8
+from itertools import groupby
+from operator import itemgetter
 from typing import List, Optional
 
 import cv2
 import numpy as np
 import polars as pl
 
 from img2table.tables.objects.cell import Cell
@@ -36,14 +38,62 @@
         margin = int(char_length)
         if min(w, h) > 2 * margin and w * h / np.prod(img.shape[:2]) < 0.9:
             thresh[y+margin:y+h-margin, x+margin:x+w-margin] = binary_thresh[y+margin:y+h-margin, x+margin:x+w-margin]
 
     return thresh
 
 
+def dilate_dotted_lines(thresh: np.ndarray, char_length: float) -> np.ndarray:
+    """
+    Dilate specific rows/columns of the threshold image in order to detect dotted lines
+    :param thresh: threshold image array
+    :param char_length: average character length in image
+    :return: threshold image with dilated dotted lines
+    """
+    ### Horizontal case
+    # Create dilated image
+    h_dilated = cv2.dilate(thresh, cv2.getStructuringElement(cv2.MORPH_RECT, (int(char_length // 2), 1)))
+
+    # Get rows with at least 2 times the average number of white pixels
+    white_rows = np.where(np.mean(thresh, axis=1) > 2 * np.mean(thresh))[0].tolist()
+
+    # Split into consecutive groups of rows and keep only small ones to avoid targeting text rows
+    white_rows_cl = [list(map(itemgetter(1), g))
+                     for k, g in groupby(enumerate(white_rows), lambda i_x: i_x[0] - i_x[1])]
+    white_rows_final = [idx for cl in white_rows_cl for idx in cl if len(cl) < char_length / 3]
+
+    # Keep only dilated image on specific rows
+    mask = np.ones(thresh.shape[0], dtype=bool)
+    mask[white_rows_final] = False
+    h_dilated[mask, :] = 0
+
+    # Update threshold image
+    thresh = np.maximum(thresh, h_dilated)
+
+    ### Vertical case
+    # Create dilated image
+    v_dilated = cv2.dilate(thresh, cv2.getStructuringElement(cv2.MORPH_RECT, (1, int(char_length // 2))))
+
+    # Get columns with at least 2 times the average number of white pixels
+    white_cols = np.where(np.mean(thresh, axis=0) > 2 * np.mean(thresh))[0].tolist()
+
+    # Split into consecutive groups of columns and keep only small ones to avoid targeting text columns
+    white_cols_cl = [list(map(itemgetter(1), g))
+                     for k, g in groupby(enumerate(white_cols), lambda i_x: i_x[0] - i_x[1])]
+    white_cols_final = [idx for cl in white_cols_cl for idx in cl if len(cl) < char_length / 3]
+
+    # Keep only dilated image on specific columns
+    mask = np.ones(thresh.shape[1], dtype=bool)
+    mask[white_cols_final] = False
+    v_dilated[:, mask] = 0
+
+    # Update threshold image
+    return np.maximum(thresh, v_dilated)
+
+
 def overlapping_filter(lines: List[Line], max_gap: int = 5) -> List[Line]:
     """
     Process lines to merge close lines
     :param lines: lines
     :param max_gap: maximum gap used to merge lines
     :return: list of filtered lines
     """
@@ -185,14 +235,18 @@
     """
     # Create copy of image
     img = image.copy()
 
     # Apply thresholding
     thresh = threshold_dark_areas(img=img, char_length=char_length)
 
+    if char_length is not None:
+        # Process threshold image in order to detect dotted lines
+        thresh = dilate_dotted_lines(thresh=thresh, char_length=char_length)
+
     # Identify both vertical and horizontal lines
     for kernel_tup, gap in [((kernel_size, 1), 2 * maxLineGap), ((1, kernel_size), maxLineGap)]:
         # Apply masking on image
         kernel = cv2.getStructuringElement(cv2.MORPH_RECT, kernel_tup)
         mask = cv2.morphologyEx(thresh, cv2.MORPH_OPEN, kernel, iterations=1)
 
         # Compute Hough lines on image and get lines
```

### Comparing `img2table-0.1.0/src/img2table/tables/processing/bordered_tables/tables/__init__.py` & `img2table-0.1.1/src/img2table/tables/processing/bordered_tables/tables/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/src/img2table/tables/processing/bordered_tables/tables/cell_clustering.py` & `img2table-0.1.1/src/img2table/tables/processing/bordered_tables/tables/cell_clustering.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/src/img2table/tables/processing/bordered_tables/tables/implicit_rows.py` & `img2table-0.1.1/src/img2table/tables/processing/bordered_tables/tables/implicit_rows.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/src/img2table/tables/processing/bordered_tables/tables/table_creation.py` & `img2table-0.1.1/src/img2table/tables/processing/bordered_tables/tables/table_creation.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/src/img2table/tables/processing/borderless_tables/__init__.py` & `img2table-0.1.1/src/img2table/tables/processing/borderless_tables/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/src/img2table/tables/processing/borderless_tables/column_delimiters.py` & `img2table-0.1.1/src/img2table/tables/processing/borderless_tables/column_delimiters.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/src/img2table/tables/processing/borderless_tables/lines.py` & `img2table-0.1.1/src/img2table/tables/processing/borderless_tables/lines.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/src/img2table/tables/processing/borderless_tables/model.py` & `img2table-0.1.1/src/img2table/tables/processing/borderless_tables/model.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/src/img2table/tables/processing/borderless_tables/segment_image.py` & `img2table-0.1.1/src/img2table/tables/processing/borderless_tables/segment_image.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/src/img2table/tables/processing/borderless_tables/table/__init__.py` & `img2table-0.1.1/src/img2table/tables/processing/borderless_tables/table/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/src/img2table/tables/processing/borderless_tables/table/headers.py` & `img2table-0.1.1/src/img2table/tables/processing/borderless_tables/table/headers.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/src/img2table/tables/processing/borderless_tables/table/table_creation.py` & `img2table-0.1.1/src/img2table/tables/processing/borderless_tables/table/table_creation.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/src/img2table/tables/processing/common.py` & `img2table-0.1.1/src/img2table/tables/processing/common.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/src/img2table/tables/processing/prepare_image.py` & `img2table-0.1.1/src/img2table/tables/processing/prepare_image.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/src/img2table/tables/processing/text/titles.py` & `img2table-0.1.1/src/img2table/tables/processing/text/titles.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/src/img2table.egg-info/PKG-INFO` & `img2table-0.1.1/src/img2table.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: img2table
-Version: 0.1.0
+Version: 0.1.1
 Summary: img2table is a table identification and extraction Python Library for PDF and images, based on OpenCV image processing
 Home-page: https://github.com/xavctn/img2table
 Author: Xavier Canton
 License: MIT
 Description: # img2table
         
         `img2table` is a simple, easy to use, table identification and extraction Python Library based on [OpenCV](https://opencv.org/) image 
@@ -12,26 +12,19 @@
         
         Thanks to its design, it provides a practical and lighter alternative to Neural Networks based solutions, especially for usage on CPU.
         
         ## Table of contents
         * [Installation](#installation)
         * [Features](#features)
         * [Supported file formats](#supported-file-formats)
-           * [Images](#images-formats)
-           * [PDF](#pdf-formats)
         * [Usage](#usage)
            * [Documents](#documents)
               * [Images](#images-doc)
               * [PDF](#pdf-doc)
-           * [OCR](#ocr)
-              * [Tesseract](#tesseract)
-              * [PaddleOCR](#paddle)
-              * [Google Vision](#vision)
-              * [AWS Textract](#textract)
-              * [Azure Cognitive Services](#azure)
+           * [Supported OCRs](#ocr)
            * [Table extraction](#table-extract)
            * [Excel export](#xlsx)
         * [Examples](#examples)
         * [Caveats / FYI](#fyi)
         
         
         ## Installation <a name="installation"></a>
```

#### html2text {}

```diff
@@ -1,38 +1,36 @@
-Metadata-Version: 2.1 Name: img2table Version: 0.1.0 Summary: img2table is a
+Metadata-Version: 2.1 Name: img2table Version: 0.1.1 Summary: img2table is a
 table identification and extraction Python Library for PDF and images, based on
 OpenCV image processing Home-page: https://github.com/xavctn/img2table Author:
 Xavier Canton License: MIT Description: # img2table `img2table` is a simple,
 easy to use, table identification and extraction Python Library based on
 [OpenCV](https://opencv.org/) image processing that supports most common image
 file formats as well as PDF files. Thanks to its design, it provides a
 practical and lighter alternative to Neural Networks based solutions,
 especially for usage on CPU. ## Table of contents * [Installation]
 (#installation) * [Features](#features) * [Supported file formats](#supported-
-file-formats) * [Images](#images-formats) * [PDF](#pdf-formats) * [Usage]
-(#usage) * [Documents](#documents) * [Images](#images-doc) * [PDF](#pdf-doc) *
-[OCR](#ocr) * [Tesseract](#tesseract) * [PaddleOCR](#paddle) * [Google Vision]
-(#vision) * [AWS Textract](#textract) * [Azure Cognitive Services](#azure) *
-[Table extraction](#table-extract) * [Excel export](#xlsx) * [Examples]
-(#examples) * [Caveats / FYI](#fyi) ## Installation  The library can be
-installed via pip. ```python # Standard installation, supporting Tesseract pip
-install img2table # For usage with Paddle OCR (Python <= 3.10 only) pip install
-img2table[paddle] # For usage with Paddle OCR - GPU (CUDA 9 / CUDA 10) (Python
-<= 3.10 only) pip install img2table[paddle-gpu] # For usage with Google Vision
-OCR pip install img2table[gcp] # For usage with AWS Textract OCR pip install
-img2table[aws] # For usage with Azure Cognitive Services OCR pip install
-img2table[azure] ``` ## Features  * Table identification for images and PDF
-files, including bounding boxes at the table cell level * Handling of complex
-table structures such as merged cells * Handling of implicit rows - see
-[example](/examples/Implicit_rows.ipynb) * Table content extraction by
-providing support for OCR services / tools * Extracted tables are returned as a
-simple object, including a Pandas DataFrame representation * Export extracted
-tables to an Excel file, preserving their original structure ## Supported file
-formats  ### Images  Images are loaded using the `opencv-python` library,
-supported formats are listed below.  Supported image formats
+file-formats) * [Usage](#usage) * [Documents](#documents) * [Images](#images-
+doc) * [PDF](#pdf-doc) * [Supported OCRs](#ocr) * [Table extraction](#table-
+extract) * [Excel export](#xlsx) * [Examples](#examples) * [Caveats / FYI]
+(#fyi) ## Installation  The library can be installed via pip. ```python #
+Standard installation, supporting Tesseract pip install img2table # For usage
+with Paddle OCR (Python <= 3.10 only) pip install img2table[paddle] # For usage
+with Paddle OCR - GPU (CUDA 9 / CUDA 10) (Python <= 3.10 only) pip install
+img2table[paddle-gpu] # For usage with Google Vision OCR pip install img2table
+[gcp] # For usage with AWS Textract OCR pip install img2table[aws] # For usage
+with Azure Cognitive Services OCR pip install img2table[azure] ``` ## Features
+* Table identification for images and PDF files, including bounding boxes at
+the table cell level * Handling of complex table structures such as merged
+cells * Handling of implicit rows - see [example](/examples/
+Implicit_rows.ipynb) * Table content extraction by providing support for OCR
+services / tools * Extracted tables are returned as a simple object, including
+a Pandas DataFrame representation * Export extracted tables to an Excel file,
+preserving their original structure ## Supported file formats  ### Images
+Images are loaded using the `opencv-python` library, supported formats are
+listed below.  Supported image formats
          * Windows bitmaps - .bmp,.dib
          * JPEG files - .jpeg,.jpg, *.jpe
          * JPEG 2000 files - *.jp2
          * Portable Network Graphics - *.png
          * WebP - *.webp
          * Portable image format - .pbm,.pgm, .ppm.pxm, *.pnm
          * PFM files - *.pfm
```

### Comparing `img2table-0.1.0/src/img2table.egg-info/SOURCES.txt` & `img2table-0.1.1/src/img2table.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -128,15 +128,14 @@
 tests/ocr/tesseract/test_data/ocr_df.csv
 tests/ocr/tesseract/test_data/test.png
 tests/tables/__init__.py
 tests/tables/image/__init__.py
 tests/tables/image/test_image.py
 tests/tables/image/test_metrics.py
 tests/tables/image/test_data/blank.png
-tests/tables/image/test_data/expected_tables.json
 tests/tables/image/test_data/ocr.csv
 tests/tables/image/test_data/test.png
 tests/tables/objects/__init__.py
 tests/tables/objects/test_extraction.py
 tests/tables/objects/test_line.py
 tests/tables/objects/test_row.py
 tests/tables/objects/test_table.py
```

### Comparing `img2table-0.1.0/tests/_mock_data/azure.pkl` & `img2table-0.1.1/tests/_mock_data/azure.pkl`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/_mock_data/tesseract_hocr.html` & `img2table-0.1.1/tests/_mock_data/tesseract_hocr.html`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/_mock_data/textract.json` & `img2table-0.1.1/tests/_mock_data/textract.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/_mock_data/vision.json` & `img2table-0.1.1/tests/_mock_data/vision.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/_mock_data/vision.pkl` & `img2table-0.1.1/tests/_mock_data/vision.pkl`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/conftest.py` & `img2table-0.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/document/base/test_data/test.png` & `img2table-0.1.1/tests/document/base/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/document/base/test_rotation.py` & `img2table-0.1.1/tests/document/base/test_rotation.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/document/image/test_data/blank.png` & `img2table-0.1.1/tests/document/image/test_data/blank.png`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/document/image/test_data/dark.png` & `img2table-0.1.1/tests/document/image/test_data/dark.png`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/document/image/test_data/expected.xlsx` & `img2table-0.1.1/tests/document/image/test_data/expected.xlsx`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/document/image/test_data/test.png` & `img2table-0.1.1/tests/document/image/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/document/image/test_image.py` & `img2table-0.1.1/tests/document/image/test_image.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 
     assert result[0].title is None
     assert result[0].bbox == BBox(x1=35, y1=20, x2=770, y2=327)
     assert len(result[0].content) == 6
     assert len(result[0].content[0]) == 3
 
     assert result[1].title is None
-    assert result[1].bbox == BBox(x1=962, y1=21, x2=1154, y2=123)
+    assert result[1].bbox == BBox(x1=962, y1=20, x2=1154, y2=123)
     assert len(result[1].content) == 2
     assert len(result[1].content[0]) == 2
 
 
 def test_no_ocr():
     img = Image(src="test_data/dark.png",
                 detect_rotation=True)
```

### Comparing `img2table-0.1.0/tests/document/pdf/test_data/test.pdf` & `img2table-0.1.1/tests/document/pdf/test_data/test.pdf`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/document/pdf/test_pdf.py` & `img2table-0.1.1/tests/document/pdf/test_pdf.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     ocr = TesseractOCR()
     pdf = PDF(src="test_data/test.pdf")
 
     result = pdf.extract_tables(ocr=ocr, implicit_rows=True, min_confidence=50)
 
     assert result[0][0].title == "Example of Data Table 1"
     if sys.version_info.minor < 11:
-        assert result[0][0].bbox == BBox(x1=236, y1=249, x2=1442, y2=543)
+        assert result[0][0].bbox == BBox(x1=235, y1=249, x2=1442, y2=543)
     assert (len(result[0][0].content), len(result[0][0].content[0])) == (5, 4)
 
     assert result[0][1].title == "Example of Data Table 2"
     if sys.version_info.minor < 11:
         assert result[0][1].bbox == BBox(x1=235, y1=671, x2=1451, y2=971)
     assert (len(result[0][1].content), len(result[0][1].content[0])) == (5, 4)
```

### Comparing `img2table-0.1.0/tests/ocr/aws_textract/test_aws_textract.py` & `img2table-0.1.1/tests/ocr/aws_textract/test_aws_textract.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/ocr/aws_textract/test_data/content.json` & `img2table-0.1.1/tests/ocr/aws_textract/test_data/content.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/ocr/aws_textract/test_data/ocr_df.csv` & `img2table-0.1.1/tests/ocr/aws_textract/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/ocr/aws_textract/test_data/test.png` & `img2table-0.1.1/tests/ocr/aws_textract/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/ocr/azure/test_azure.py` & `img2table-0.1.1/tests/ocr/azure/test_azure.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/ocr/azure/test_data/ocr_df.csv` & `img2table-0.1.1/tests/ocr/azure/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/ocr/azure/test_data/test.png` & `img2table-0.1.1/tests/ocr/azure/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/ocr/data/test_data/expected_table.json` & `img2table-0.1.1/tests/ocr/data/test_data/expected_table.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/ocr/data/test_data/ocr_df.csv` & `img2table-0.1.1/tests/ocr/data/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/ocr/data/test_ocr_data.py` & `img2table-0.1.1/tests/ocr/data/test_ocr_data.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/ocr/google_vision/test_data/expected_content.json` & `img2table-0.1.1/tests/ocr/google_vision/test_data/expected_content.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/ocr/google_vision/test_data/ocr_df.csv` & `img2table-0.1.1/tests/ocr/google_vision/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/ocr/google_vision/test_data/test.png` & `img2table-0.1.1/tests/ocr/google_vision/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/ocr/google_vision/test_google_vision.py` & `img2table-0.1.1/tests/ocr/google_vision/test_google_vision.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/ocr/paddle/test_data/hocr.json` & `img2table-0.1.1/tests/ocr/paddle/test_data/hocr.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/ocr/paddle/test_data/ocr_df.csv` & `img2table-0.1.1/tests/ocr/paddle/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/ocr/paddle/test_data/test.png` & `img2table-0.1.1/tests/ocr/paddle/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/ocr/paddle/test_paddle.py` & `img2table-0.1.1/tests/ocr/paddle/test_paddle.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/ocr/pdf/test_data/content.json` & `img2table-0.1.1/tests/ocr/pdf/test_data/content.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/ocr/pdf/test_data/ocr_df.csv` & `img2table-0.1.1/tests/ocr/pdf/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/ocr/pdf/test_data/test.pdf` & `img2table-0.1.1/tests/ocr/pdf/test_data/test.pdf`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/ocr/pdf/test_pdf_ocr.py` & `img2table-0.1.1/tests/ocr/pdf/test_pdf_ocr.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/ocr/tesseract/test_data/ocr_df.csv` & `img2table-0.1.1/tests/ocr/tesseract/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/ocr/tesseract/test_data/test.png` & `img2table-0.1.1/tests/ocr/tesseract/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/ocr/tesseract/test_tesseract.py` & `img2table-0.1.1/tests/ocr/tesseract/test_tesseract.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/tables/image/test_data/blank.png` & `img2table-0.1.1/tests/tables/image/test_data/blank.png`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/tables/image/test_data/expected_tables.json` & `img2table-0.1.1/tests/tables/objects/test_data/expected_tables.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9055555555555556%*

 * *Differences: {'0': "{0: {0: {'y2': 71}, 1: {'y2': 71}, 2: {'y2': 71}}, 1: {0: {'y1': 71}, 1: {'y1': 71}, 2: "*

 * *      "{'y1': 71}}, 2: {0: {'y2': 173}, 1: {'y2': 275}, 2: {'y2': 173}}, 3: {0: {'y1': 173, 'y2': "*

 * *      "225}, 1: {'y2': 275}, 2: {'y1': 173, 'y2': 225}}, 4: {0: {'y1': 225, 'y2': 275}, 1: {'y2': "*

 * *      "275}, 2: {'y1': 225, 'y2': 275}}, 5: {0: {'y1': 275, 'y2': 326}, 1: {'y1': 275, 'y2': 326}, "*

 * *      "2: {'y1': 275, 'y2': 326}}}",*

 * * '1': "{0: {0: {'x1': 961}}, 1: {0: {'x1': 961}}}"}*

```diff
@@ -2,152 +2,152 @@
     [
         [
             {
                 "content": "Title",
                 "x1": 35,
                 "x2": 770,
                 "y1": 20,
-                "y2": 72
+                "y2": 71
             },
             {
                 "content": "Title",
                 "x1": 35,
                 "x2": 770,
                 "y1": 20,
-                "y2": 72
+                "y2": 71
             },
             {
                 "content": "Title",
                 "x1": 35,
                 "x2": 770,
                 "y1": 20,
-                "y2": 72
+                "y2": 71
             }
         ],
         [
             {
                 "content": "Line 1-Col 1",
                 "x1": 35,
                 "x2": 276,
-                "y1": 72,
+                "y1": 71,
                 "y2": 123
             },
             {
                 "content": "Line Col 2",
                 "x1": 276,
                 "x2": 494,
-                "y1": 72,
+                "y1": 71,
                 "y2": 123
             },
             {
                 "content": "Line 1-Col 3",
                 "x1": 494,
                 "x2": 770,
-                "y1": 72,
+                "y1": 71,
                 "y2": 123
             }
         ],
         [
             {
                 "content": "Line Col 1",
                 "x1": 35,
                 "x2": 276,
                 "y1": 123,
-                "y2": 174
+                "y2": 173
             },
             {
                 "content": "Merged Cells",
                 "x1": 276,
                 "x2": 494,
                 "y1": 123,
-                "y2": 276
+                "y2": 275
             },
             {
                 "content": "Line 2-Col3",
                 "x1": 494,
                 "x2": 770,
                 "y1": 123,
-                "y2": 174
+                "y2": 173
             }
         ],
         [
             {
                 "content": "Line 3-Col1",
                 "x1": 35,
                 "x2": 276,
-                "y1": 174,
-                "y2": 224
+                "y1": 173,
+                "y2": 225
             },
             {
                 "content": "Merged Cells",
                 "x1": 276,
                 "x2": 494,
                 "y1": 123,
-                "y2": 276
+                "y2": 275
             },
             {
                 "content": "Line 3-Col3",
                 "x1": 494,
                 "x2": 770,
-                "y1": 174,
-                "y2": 224
+                "y1": 173,
+                "y2": 225
             }
         ],
         [
             {
                 "content": "Line 4-Col1",
                 "x1": 35,
                 "x2": 276,
-                "y1": 224,
-                "y2": 276
+                "y1": 225,
+                "y2": 275
             },
             {
                 "content": "Merged Cells",
                 "x1": 276,
                 "x2": 494,
                 "y1": 123,
-                "y2": 276
+                "y2": 275
             },
             {
                 "content": "Line 4-Col3",
                 "x1": 494,
                 "x2": 770,
-                "y1": 224,
-                "y2": 276
+                "y1": 225,
+                "y2": 275
             }
         ],
         [
             {
                 "content": "Line",
                 "x1": 35,
                 "x2": 276,
-                "y1": 276,
-                "y2": 327
+                "y1": 275,
+                "y2": 326
             },
             {
                 "content": "Line 5-Col2",
                 "x1": 276,
                 "x2": 494,
-                "y1": 276,
-                "y2": 327
+                "y1": 275,
+                "y2": 326
             },
             {
                 "content": "Line 3",
                 "x1": 494,
                 "x2": 770,
-                "y1": 276,
-                "y2": 327
+                "y1": 275,
+                "y2": 326
             }
         ]
     ],
     [
         [
             {
                 "content": "Test 1",
-                "x1": 962,
+                "x1": 961,
                 "x2": 1058,
                 "y1": 21,
                 "y2": 71
             },
             {
                 "content": "Test 2",
                 "x1": 1058,
@@ -155,15 +155,15 @@
                 "y1": 21,
                 "y2": 71
             }
         ],
         [
             {
                 "content": "Test 3",
-                "x1": 962,
+                "x1": 961,
                 "x2": 1058,
                 "y1": 71,
                 "y2": 123
             },
             {
                 "content": "Test 4",
                 "x1": 1058,
```

### Comparing `img2table-0.1.0/tests/tables/image/test_data/ocr.csv` & `img2table-0.1.1/tests/tables/image/test_data/ocr.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/tables/image/test_data/test.png` & `img2table-0.1.1/tests/tables/image/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/tables/image/test_image.py` & `img2table-0.1.1/tests/tables/objects/test_extraction.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 # coding: utf-8
 import json
+from io import BytesIO
 
-import cv2
-import polars as pl
+from xlsxwriter import Workbook
 
-from img2table.ocr.data import OCRDataframe
-from img2table.tables.image import TableImage
 from img2table.tables.objects.cell import Cell
 from img2table.tables.objects.row import Row
 from img2table.tables.objects.table import Table
 
 
-def test_table_image():
-    image = cv2.imread("test_data/test.png", cv2.IMREAD_GRAYSCALE)
-    ocr_df = OCRDataframe(pl.read_csv("test_data/ocr.csv", separator=";", encoding="utf-8").lazy())
-
-    tb_image = TableImage(img=image,
-                          dpi=200,
-                          ocr_df=ocr_df,
-                          min_confidence=50)
-
-    result = tb_image.extract_tables(implicit_rows=True)
-
+def test_extracted_table_worksheet():
     with open("test_data/expected_tables.json", "r") as f:
-        expected = [Table(rows=[Row(cells=[Cell(**el) for el in row]) for row in tb]).extracted_table
-                    for tb in json.load(f)]
+        tables = [Table(rows=[Row(cells=[Cell(**el) for el in row]) for row in tb])
+                  for tb in json.load(f)]
+
+    wb = Workbook(BytesIO())
+    for table in tables:
+        ws = wb.add_worksheet()
+        extracted_table = table.extracted_table
+        extracted_table._to_worksheet(sheet=ws)
+
+        assert ws.dim_colmax + 1 == table.nb_columns
+        assert ws.dim_rowmax + 1 == table.nb_rows
+
+        str_map = {v: k for k, v in ws.str_table.string_table.items()}
+        ws_values = sorted([str_map.get(c.string) for row in ws.table.values() for c in row.values()])
+        table_values = sorted(set([c.value for row in extracted_table.content.values()
+                                   for c in row]))
+        assert ws_values == table_values
 
-    assert result == expected
+    wb.close()
```

### Comparing `img2table-0.1.0/tests/tables/image/test_metrics.py` & `img2table-0.1.1/tests/tables/image/test_metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from img2table.tables.metrics import compute_char_length, compute_median_line_sep, compute_img_metrics
 
 
 def test_compute_char_length():
     image = cv2.imread("test_data/test.png", cv2.IMREAD_GRAYSCALE)
 
     char_length, cc_array = compute_char_length(img=image)
-    assert round(char_length, 2) == 8.44
-    assert len(cc_array) == 117
+    assert round(char_length, 2) == 8.50
+    assert len(cc_array) == 116
 
     image = cv2.imread("test_data/blank.png", cv2.IMREAD_GRAYSCALE)
     assert compute_char_length(img=image) == (None, None)
 
 
 def test_compute_median_line_sep():
     image = cv2.imread("test_data/test.png", cv2.IMREAD_GRAYSCALE)
@@ -25,13 +25,13 @@
     assert len(contours) == 43
 
 
 def test_compute_img_metrics():
     image = cv2.imread("test_data/test.png", cv2.IMREAD_GRAYSCALE)
     char_length, median_line_sep, contours = compute_img_metrics(img=image)
 
-    assert round(char_length, 2) == 8.44
+    assert round(char_length, 2) == 8.5
     assert round(median_line_sep, 2) == 51
     assert len(contours) == 43
 
     image = cv2.imread("test_data/blank.png", cv2.IMREAD_GRAYSCALE)
     assert compute_img_metrics(img=image) == (None, None, None)
```

### Comparing `img2table-0.1.0/tests/tables/objects/test_data/ocr.csv` & `img2table-0.1.1/tests/tables/objects/test_data/ocr.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/tables/objects/test_data/tables.json` & `img2table-0.1.1/tests/tables/objects/test_data/tables.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/tables/objects/test_line.py` & `img2table-0.1.1/tests/tables/objects/test_line.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/tables/objects/test_row.py` & `img2table-0.1.1/tests/tables/objects/test_row.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/tables/objects/test_table.py` & `img2table-0.1.1/tests/tables/objects/test_table.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/tables/processing/bordered_tables/cells/test_cells.py` & `img2table-0.1.1/tests/tables/processing/bordered_tables/cells/test_cells.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/tables/processing/bordered_tables/cells/test_data/expected.csv` & `img2table-0.1.1/tests/tables/processing/bordered_tables/cells/test_data/expected.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/tables/processing/bordered_tables/cells/test_data/lines.json` & `img2table-0.1.1/tests/tables/processing/bordered_tables/cells/test_data/lines.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/tables/processing/bordered_tables/cells/test_deduplication_cells.py` & `img2table-0.1.1/tests/tables/processing/bordered_tables/cells/test_deduplication_cells.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/tables/processing/bordered_tables/cells/test_identification_cells.py` & `img2table-0.1.1/tests/tables/processing/bordered_tables/cells/test_identification_cells.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/tables/processing/bordered_tables/lines/test_data/contours.json` & `img2table-0.1.1/tests/tables/processing/bordered_tables/lines/test_data/contours.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/tables/processing/bordered_tables/lines/test_data/expected.json` & `img2table-0.1.1/tests/tables/processing/borderless_tables/borderless_table/test_data/lines.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/tables/processing/bordered_tables/lines/test_data/test.png` & `img2table-0.1.1/tests/tables/processing/bordered_tables/lines/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/tables/processing/bordered_tables/lines/test_lines.py` & `img2table-0.1.1/tests/tables/processing/bordered_tables/lines/test_lines.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/tables/processing/bordered_tables/tables/test_cell_clustering.py` & `img2table-0.1.1/tests/tables/processing/bordered_tables/tables/test_cell_clustering.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/tables/processing/bordered_tables/tables/test_data/cell_clusters_normalized.json` & `img2table-0.1.1/tests/tables/processing/bordered_tables/tables/test_data/cell_clusters_normalized.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/tables/processing/bordered_tables/tables/test_data/cells.json` & `img2table-0.1.1/tests/tables/processing/bordered_tables/tables/test_data/cells.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/tables/processing/bordered_tables/tables/test_data/cells_clustered.json` & `img2table-0.1.1/tests/tables/processing/bordered_tables/tables/test_data/cells_clustered.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/tables/processing/bordered_tables/tables/test_data/expected.json` & `img2table-0.1.1/tests/tables/processing/bordered_tables/tables/test_data/expected.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/tables/processing/bordered_tables/tables/test_data/implicit.png` & `img2table-0.1.1/tests/tables/processing/bordered_tables/tables/test_data/implicit.png`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/tables/processing/bordered_tables/tables/test_data/tables_from_cells.json` & `img2table-0.1.1/tests/tables/processing/bordered_tables/tables/test_data/tables_from_cells.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/tables/processing/bordered_tables/tables/test_data/word_image.png` & `img2table-0.1.1/tests/tables/processing/bordered_tables/tables/test_data/word_image.png`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/tables/processing/bordered_tables/tables/test_implicit_rows.py` & `img2table-0.1.1/tests/tables/processing/bordered_tables/tables/test_implicit_rows.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/tables/processing/bordered_tables/tables/test_table_creation.py` & `img2table-0.1.1/tests/tables/processing/bordered_tables/tables/test_table_creation.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/tables/processing/bordered_tables/tables/test_tables.py` & `img2table-0.1.1/tests/tables/processing/bordered_tables/tables/test_tables.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/tables/processing/borderless_tables/borderless_table/test_borderless_table.py` & `img2table-0.1.1/tests/tables/processing/borderless_tables/borderless_table/test_borderless_table.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/tables/processing/borderless_tables/borderless_table/test_data/lines.json` & `img2table-0.1.1/tests/tables/processing/borderless_tables/segment_image/test_data/lines.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/tables/processing/borderless_tables/borderless_table/test_data/test.png` & `img2table-0.1.1/tests/tables/processing/borderless_tables/borderless_table/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/tables/processing/borderless_tables/column_delimiters/test_column_delimiters.py` & `img2table-0.1.1/tests/tables/processing/borderless_tables/column_delimiters/test_column_delimiters.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/tables/processing/borderless_tables/lines/test_data/image_segment.json` & `img2table-0.1.1/tests/tables/processing/borderless_tables/lines/test_data/image_segment.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/tables/processing/borderless_tables/lines/test_lines.py` & `img2table-0.1.1/tests/tables/processing/borderless_tables/lines/test_lines.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/tables/processing/borderless_tables/segment_image/test_data/lines.json` & `img2table-0.1.1/tests/tables/processing/bordered_tables/lines/test_data/expected.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9538461538461539%*

 * *Differences: {"'h_lines'": "{1: {'x1': 966}, 2: {'y1': 72, 'y2': 72}, 3: {'y1': 72, 'y2': 72}, 4: {'y1': 122, "*

 * *              "'y2': 122}, 5: {'x1': 961}, 10: {'y1': 225, 'y2': 225}, 11: {'y1': 276, 'y2': 276}, "*

 * *              "12: {'y1': 327, 'y2': 327}, insert: [(8, OrderedDict([('x1', 417), ('y1', 199), "*

 * *              "('x2', 446), ('y2', 199), ('thickness', 1)]))]}"}*

```diff
@@ -5,43 +5,43 @@
             "x1": 35,
             "x2": 772,
             "y1": 20,
             "y2": 20
         },
         {
             "thickness": 3,
-            "x1": 961,
+            "x1": 966,
             "x2": 1156,
             "y1": 21,
             "y2": 21
         },
         {
             "thickness": 3,
             "x1": 36,
             "x2": 771,
-            "y1": 71,
-            "y2": 71
+            "y1": 72,
+            "y2": 72
         },
         {
             "thickness": 3,
             "x1": 962,
             "x2": 1156,
-            "y1": 71,
-            "y2": 71
+            "y1": 72,
+            "y2": 72
         },
         {
             "thickness": 3,
             "x1": 36,
             "x2": 771,
-            "y1": 123,
-            "y2": 123
+            "y1": 122,
+            "y2": 122
         },
         {
             "thickness": 3,
-            "x1": 962,
+            "x1": 961,
             "x2": 1156,
             "y1": 123,
             "y2": 123
         },
         {
             "thickness": 3,
             "x1": 36,
@@ -53,40 +53,47 @@
             "thickness": 3,
             "x1": 495,
             "x2": 771,
             "y1": 174,
             "y2": 174
         },
         {
+            "thickness": 1,
+            "x1": 417,
+            "x2": 446,
+            "y1": 199,
+            "y2": 199
+        },
+        {
             "thickness": 3,
             "x1": 36,
             "x2": 277,
             "y1": 225,
             "y2": 225
         },
         {
             "thickness": 3,
             "x1": 495,
             "x2": 771,
-            "y1": 224,
-            "y2": 224
+            "y1": 225,
+            "y2": 225
         },
         {
             "thickness": 3,
             "x1": 36,
             "x2": 772,
-            "y1": 275,
-            "y2": 275
+            "y1": 276,
+            "y2": 276
         },
         {
             "thickness": 3,
             "x1": 35,
             "x2": 772,
-            "y1": 326,
-            "y2": 326
+            "y1": 327,
+            "y2": 327
         }
     ],
     "v_lines": [
         {
             "thickness": 3,
             "x1": 35,
             "x2": 35,
```

### Comparing `img2table-0.1.0/tests/tables/processing/borderless_tables/segment_image/test_data/test.png` & `img2table-0.1.1/tests/tables/processing/borderless_tables/segment_image/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/tables/processing/borderless_tables/segment_image/test_segment_image.py` & `img2table-0.1.1/tests/tables/processing/borderless_tables/segment_image/test_segment_image.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/tables/processing/borderless_tables/table/test_headers.py` & `img2table-0.1.1/tests/tables/processing/borderless_tables/table/test_headers.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/tables/processing/borderless_tables/table/test_table.py` & `img2table-0.1.1/tests/tables/processing/borderless_tables/table/test_table.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/tables/processing/borderless_tables/table/test_table_creation.py` & `img2table-0.1.1/tests/tables/processing/borderless_tables/table/test_table_creation.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/tables/processing/common/test_common.py` & `img2table-0.1.1/tests/tables/processing/common/test_common.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/tables/processing/common/test_data/test.jpg` & `img2table-0.1.1/tests/tables/processing/common/test_data/test.jpg`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/tables/processing/prepare_image/test_data/test.png` & `img2table-0.1.1/tests/tables/processing/prepare_image/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/tables/processing/text/test_data/ocr.csv` & `img2table-0.1.1/tests/tables/processing/text/test_data/ocr.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/tables/processing/text/test_data/table.json` & `img2table-0.1.1/tests/tables/processing/text/test_data/table.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/tables/processing/text/test_data/test.jpg` & `img2table-0.1.1/tests/tables/processing/text/test_data/test.jpg`

 * *Files identical despite different names*

### Comparing `img2table-0.1.0/tests/tables/processing/text/test_titles.py` & `img2table-0.1.1/tests/tables/processing/text/test_titles.py`

 * *Files identical despite different names*

