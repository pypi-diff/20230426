# Comparing `tmp/docile_benchmark-0.3.0.tar.gz` & `tmp/docile_benchmark-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docile_benchmark-0.3.0.tar", max compression
+gzip compressed data, was "docile_benchmark-0.3.1.tar", max compression
```

## Comparing `docile_benchmark-0.3.0.tar` & `docile_benchmark-0.3.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1063 2023-01-31 09:21:21.708117 docile_benchmark-0.3.0/LICENSE
--rw-r--r--   0        0        0    13189 2023-03-10 10:09:39.881418 docile_benchmark-0.3.0/README.md
--rw-r--r--   0        0        0       72 2022-10-27 11:49:12.996264 docile_benchmark-0.3.0/docile/__init__.py
--rw-r--r--   0        0        0        0 2023-01-28 01:11:25.613980 docile_benchmark-0.3.0/docile/cli/__init__.py
--rw-r--r--   0        0        0     8513 2023-02-06 15:40:06.226062 docile_benchmark-0.3.0/docile/cli/evaluate.py
--rw-r--r--   0        0        0     1901 2023-01-31 09:21:21.709835 docile_benchmark-0.3.0/docile/dataset/__init__.py
--rw-r--r--   0        0        0     2801 2023-02-28 10:54:40.307559 docile_benchmark-0.3.0/docile/dataset/bbox.py
--rw-r--r--   0        0        0     3265 2023-02-01 14:12:45.594310 docile_benchmark-0.3.0/docile/dataset/cached_object.py
--rw-r--r--   0        0        0    10718 2023-02-28 10:54:40.307946 docile_benchmark-0.3.0/docile/dataset/dataset.py
--rw-r--r--   0        0        0     6876 2023-02-01 14:12:45.594945 docile_benchmark-0.3.0/docile/dataset/document.py
--rw-r--r--   0        0        0     5487 2023-01-31 09:21:24.269777 docile_benchmark-0.3.0/docile/dataset/document_annotation.py
--rw-r--r--   0        0        0     2584 2023-01-28 01:11:25.618383 docile_benchmark-0.3.0/docile/dataset/document_images.py
--rw-r--r--   0        0        0    15593 2023-01-31 09:21:24.270032 docile_benchmark-0.3.0/docile/dataset/document_ocr.py
--rw-r--r--   0        0        0     3594 2023-03-01 15:01:34.991739 docile_benchmark-0.3.0/docile/dataset/field.py
--rw-r--r--   0        0        0     4543 2023-01-28 01:11:25.620029 docile_benchmark-0.3.0/docile/dataset/paths.py
--rw-r--r--   0        0        0     3699 2023-01-28 01:11:25.620482 docile_benchmark-0.3.0/docile/dataset/table_grid.py
--rw-r--r--   0        0        0      111 2022-10-31 14:20:17.990237 docile_benchmark-0.3.0/docile/dataset/types.py
--rw-r--r--   0        0        0      384 2023-02-06 15:40:06.226863 docile_benchmark-0.3.0/docile/evaluation/__init__.py
--rw-r--r--   0        0        0     2686 2023-02-06 15:40:06.227346 docile_benchmark-0.3.0/docile/evaluation/average_precision.py
--rw-r--r--   0        0        0    22420 2023-02-28 10:54:40.309820 docile_benchmark-0.3.0/docile/evaluation/evaluate.py
--rw-r--r--   0        0        0     5244 2023-02-09 20:51:36.153427 docile_benchmark-0.3.0/docile/evaluation/evaluation_subsets.py
--rw-r--r--   0        0        0     7594 2023-01-28 01:11:25.624182 docile_benchmark-0.3.0/docile/evaluation/line_item_matching.py
--rw-r--r--   0        0        0     3343 2023-01-31 14:29:38.638822 docile_benchmark-0.3.0/docile/evaluation/pcc.py
--rw-r--r--   0        0        0     8495 2023-01-30 07:58:03.976133 docile_benchmark-0.3.0/docile/evaluation/pcc_field_matching.py
--rw-r--r--   0        0        0        0 2023-01-28 01:11:25.625296 docile_benchmark-0.3.0/docile/tools/__init__.py
--rw-r--r--   0        0        0     3789 2023-03-15 12:22:16.980395 docile_benchmark-0.3.0/docile/tools/dataset_browser.ipynb
--rw-r--r--   0        0        0    17062 2023-03-01 15:01:34.992185 docile_benchmark-0.3.0/docile/tools/dataset_browser.py
--rw-r--r--   0        0        0     4496 2023-03-10 10:09:39.883315 docile_benchmark-0.3.0/docile/tools/print_results.py
--rw-r--r--   0        0        0     3678 2023-03-15 12:16:41.151828 docile_benchmark-0.3.0/pyproject.toml
--rw-r--r--   0        0        0    15387 1970-01-01 00:00:00.000000 docile_benchmark-0.3.0/setup.py
--rw-r--r--   0        0        0    15167 1970-01-01 00:00:00.000000 docile_benchmark-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-01-31 09:21:21.708117 docile_benchmark-0.3.1/LICENSE
+-rw-r--r--   0        0        0    13284 2023-04-26 20:33:05.937773 docile_benchmark-0.3.1/README.md
+-rw-r--r--   0        0        0       72 2022-10-27 11:49:12.996264 docile_benchmark-0.3.1/docile/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-28 01:11:25.613980 docile_benchmark-0.3.1/docile/cli/__init__.py
+-rw-r--r--   0        0        0     8513 2023-02-06 15:40:06.226062 docile_benchmark-0.3.1/docile/cli/evaluate.py
+-rw-r--r--   0        0        0     1901 2023-01-31 09:21:21.709835 docile_benchmark-0.3.1/docile/dataset/__init__.py
+-rw-r--r--   0        0        0     2801 2023-02-28 10:54:40.307559 docile_benchmark-0.3.1/docile/dataset/bbox.py
+-rw-r--r--   0        0        0     3265 2023-02-01 14:12:45.594310 docile_benchmark-0.3.1/docile/dataset/cached_object.py
+-rw-r--r--   0        0        0    10718 2023-02-28 10:54:40.307946 docile_benchmark-0.3.1/docile/dataset/dataset.py
+-rw-r--r--   0        0        0     6876 2023-02-01 14:12:45.594945 docile_benchmark-0.3.1/docile/dataset/document.py
+-rw-r--r--   0        0        0     5487 2023-01-31 09:21:24.269777 docile_benchmark-0.3.1/docile/dataset/document_annotation.py
+-rw-r--r--   0        0        0     2584 2023-01-28 01:11:25.618383 docile_benchmark-0.3.1/docile/dataset/document_images.py
+-rw-r--r--   0        0        0    15593 2023-01-31 09:21:24.270032 docile_benchmark-0.3.1/docile/dataset/document_ocr.py
+-rw-r--r--   0        0        0     3594 2023-03-01 15:01:34.991739 docile_benchmark-0.3.1/docile/dataset/field.py
+-rw-r--r--   0        0        0     4543 2023-01-28 01:11:25.620029 docile_benchmark-0.3.1/docile/dataset/paths.py
+-rw-r--r--   0        0        0     3699 2023-01-28 01:11:25.620482 docile_benchmark-0.3.1/docile/dataset/table_grid.py
+-rw-r--r--   0        0        0      111 2022-10-31 14:20:17.990237 docile_benchmark-0.3.1/docile/dataset/types.py
+-rw-r--r--   0        0        0      384 2023-02-06 15:40:06.226863 docile_benchmark-0.3.1/docile/evaluation/__init__.py
+-rw-r--r--   0        0        0     2686 2023-02-06 15:40:06.227346 docile_benchmark-0.3.1/docile/evaluation/average_precision.py
+-rw-r--r--   0        0        0    22420 2023-02-28 10:54:40.309820 docile_benchmark-0.3.1/docile/evaluation/evaluate.py
+-rw-r--r--   0        0        0     5244 2023-02-09 20:51:36.153427 docile_benchmark-0.3.1/docile/evaluation/evaluation_subsets.py
+-rw-r--r--   0        0        0     7594 2023-01-28 01:11:25.624182 docile_benchmark-0.3.1/docile/evaluation/line_item_matching.py
+-rw-r--r--   0        0        0     3343 2023-01-31 14:29:38.638822 docile_benchmark-0.3.1/docile/evaluation/pcc.py
+-rw-r--r--   0        0        0     8495 2023-01-30 07:58:03.976133 docile_benchmark-0.3.1/docile/evaluation/pcc_field_matching.py
+-rw-r--r--   0        0        0        0 2023-01-28 01:11:25.625296 docile_benchmark-0.3.1/docile/tools/__init__.py
+-rw-r--r--   0        0        0     3544 2023-04-25 13:41:50.143608 docile_benchmark-0.3.1/docile/tools/dataset_browser.ipynb
+-rw-r--r--   0        0        0    17474 2023-04-26 20:13:27.093421 docile_benchmark-0.3.1/docile/tools/dataset_browser.py
+-rw-r--r--   0        0        0     4496 2023-03-10 10:09:39.883315 docile_benchmark-0.3.1/docile/tools/print_results.py
+-rw-r--r--   0        0        0     3678 2023-04-26 21:49:33.368271 docile_benchmark-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0    15482 1970-01-01 00:00:00.000000 docile_benchmark-0.3.1/setup.py
+-rw-r--r--   0        0        0    15262 1970-01-01 00:00:00.000000 docile_benchmark-0.3.1/PKG-INFO
```

### Comparing `docile_benchmark-0.3.0/LICENSE` & `docile_benchmark-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `docile_benchmark-0.3.0/README.md` & `docile_benchmark-0.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,32 +4,32 @@
 
 Repository to work with the [DocILE dataset and benchmark](https://docile.rossum.ai/), used in the DocILE'23 CLEF Lab and ICDAR Competition.
 The competition deadline is on May 10, 2023 and comes with a **$9000 prize pool**.
 
 The repository consists of:
 * A python library, `docile`, making it easy to load the dataset, work with its annotations, pdfs and pre-computed OCR and run the evaluation.
 * An interactive [dataset browser notebook](docile/tools/dataset_browser.ipynb) to visualize the document annotations, predictions and evaluation results.
-* Baseline methods (will appear soon).
+* Training and inference scripts for [Baseline methods](baselines/) provided together with pretrained checkpoints and results on test and validation sets.
+* [Tutorials](tutorials/) to get quickly started with the repo.
 
 Table of Contents:
 * [Download the dataset](#download-the-dataset)
 * [Installation](#installation)
 * [Predictions format and running evaluation](#predictions-format-and-running-evaluation)
 * [Tasks and evaluation metrics](#tasks-and-evaluation-metrics)
 * [Pre-computed OCR](#pre-computed-ocr)
 * [Development instructions](#development-instructions)
 * [Dataset and benchmark paper](#dataset-and-benchmark-paper)
 
-Also check [Tutorials](tutorials/) to get quickly started with the repo and [Baselines](baselines/) for the provided baseline solutions.
-
 ## Download the dataset
 
 First you need to obtain a secret token by following the instructions at https://docile.rossum.ai/. Then download and unzip the dataset by running:
 ```bash
 ./download_dataset.sh TOKEN annotated-trainval data/docile --unzip
+./download_dataset.sh TOKEN test data/docile --unzip
 ./download_dataset.sh TOKEN synthetic data/docile --unzip
 ./download_dataset.sh TOKEN unlabeled data/docile --unzip
 ```
 
 Run `./download_dataset.sh --help` for more options, including how to only show urls (to download
 with a different tool than curl), how to download smaller unlabeled/synthetic chunks or unlabeled
 dataset without pdfs (with pre-computed OCR only).
```

### Comparing `docile_benchmark-0.3.0/docile/cli/evaluate.py` & `docile_benchmark-0.3.1/docile/cli/evaluate.py`

 * *Files identical despite different names*

### Comparing `docile_benchmark-0.3.0/docile/dataset/__init__.py` & `docile_benchmark-0.3.1/docile/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `docile_benchmark-0.3.0/docile/dataset/bbox.py` & `docile_benchmark-0.3.1/docile/dataset/bbox.py`

 * *Files identical despite different names*

### Comparing `docile_benchmark-0.3.0/docile/dataset/cached_object.py` & `docile_benchmark-0.3.1/docile/dataset/cached_object.py`

 * *Files identical despite different names*

### Comparing `docile_benchmark-0.3.0/docile/dataset/dataset.py` & `docile_benchmark-0.3.1/docile/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `docile_benchmark-0.3.0/docile/dataset/document.py` & `docile_benchmark-0.3.1/docile/dataset/document.py`

 * *Files identical despite different names*

### Comparing `docile_benchmark-0.3.0/docile/dataset/document_annotation.py` & `docile_benchmark-0.3.1/docile/dataset/document_annotation.py`

 * *Files identical despite different names*

### Comparing `docile_benchmark-0.3.0/docile/dataset/document_images.py` & `docile_benchmark-0.3.1/docile/dataset/document_images.py`

 * *Files identical despite different names*

### Comparing `docile_benchmark-0.3.0/docile/dataset/document_ocr.py` & `docile_benchmark-0.3.1/docile/dataset/document_ocr.py`

 * *Files identical despite different names*

### Comparing `docile_benchmark-0.3.0/docile/dataset/field.py` & `docile_benchmark-0.3.1/docile/dataset/field.py`

 * *Files identical despite different names*

### Comparing `docile_benchmark-0.3.0/docile/dataset/paths.py` & `docile_benchmark-0.3.1/docile/dataset/paths.py`

 * *Files identical despite different names*

### Comparing `docile_benchmark-0.3.0/docile/dataset/table_grid.py` & `docile_benchmark-0.3.1/docile/dataset/table_grid.py`

 * *Files identical despite different names*

### Comparing `docile_benchmark-0.3.0/docile/evaluation/average_precision.py` & `docile_benchmark-0.3.1/docile/evaluation/average_precision.py`

 * *Files identical despite different names*

### Comparing `docile_benchmark-0.3.0/docile/evaluation/evaluate.py` & `docile_benchmark-0.3.1/docile/evaluation/evaluate.py`

 * *Files identical despite different names*

### Comparing `docile_benchmark-0.3.0/docile/evaluation/evaluation_subsets.py` & `docile_benchmark-0.3.1/docile/evaluation/evaluation_subsets.py`

 * *Files identical despite different names*

### Comparing `docile_benchmark-0.3.0/docile/evaluation/line_item_matching.py` & `docile_benchmark-0.3.1/docile/evaluation/line_item_matching.py`

 * *Files identical despite different names*

### Comparing `docile_benchmark-0.3.0/docile/evaluation/pcc.py` & `docile_benchmark-0.3.1/docile/evaluation/pcc.py`

 * *Files identical despite different names*

### Comparing `docile_benchmark-0.3.0/docile/evaluation/pcc_field_matching.py` & `docile_benchmark-0.3.1/docile/evaluation/pcc_field_matching.py`

 * *Files identical despite different names*

### Comparing `docile_benchmark-0.3.0/docile/tools/dataset_browser.ipynb` & `docile_benchmark-0.3.1/docile/tools/dataset_browser.ipynb`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9918650793650794%*

 * *Differences: {"'cells'": "{0: {'execution_count': None, 'metadata': {replace: OrderedDict()}}, 1: "*

 * *            "{'execution_count': None, 'metadata': {replace: OrderedDict()}, 'outputs': [], "*

 * *            '\'source\': {insert: [(1, \'dataset = Dataset("val", DATASET_PATH)\')], delete: '*

 * *            '[1]}}}',*

 * * "'metadata'": "{'language_info': {'version': '3.10.9'}}"}*

```diff
@@ -1,44 +1,32 @@
 {
     "cells": [
         {
             "cell_type": "code",
-            "execution_count": 1,
+            "execution_count": null,
             "id": "bcdaf56f-c860-430b-937d-ea072cae88b6",
-            "metadata": {
-                "tags": []
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
                 "import json\n",
                 "from pathlib import Path\n",
                 "from docile.dataset import Dataset\n",
                 "from docile.dataset import Field\n",
                 "from docile.tools.dataset_browser import DatasetBrowser"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": null,
             "id": "b367b0d2-5397-4910-b592-15079933deb5",
-            "metadata": {
-                "tags": []
-            },
-            "outputs": [
-                {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "Loading documents for docile:train: 100%|\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588| 5180/5180 [01:01<00:00, 84.05it/s] \n"
-                    ]
-                }
-            ],
+            "metadata": {},
+            "outputs": [],
             "source": [
                 "DATASET_PATH = Path(\"/app/data/docile/\")\n",
-                "dataset = Dataset(\"train\", DATASET_PATH)"
+                "dataset = Dataset(\"val\", DATASET_PATH)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "025ba00e",
             "metadata": {},
             "source": [
@@ -142,13 +130,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.10"
+            "version": "3.10.9"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `docile_benchmark-0.3.0/docile/tools/dataset_browser.py` & `docile_benchmark-0.3.1/docile/tools/dataset_browser.py`

 * *Files 6% similar despite different names*

```diff
@@ -279,15 +279,18 @@
                 )
 
     def get_all_displayboxes(self) -> List[DisplayBox]:
         annotation = self.dataset[self.doc_i].annotation
 
         display_boxes = []
 
-        table_grid = annotation.get_table_grid(self.page_i)
+        try:
+            table_grid = annotation.get_table_grid(self.page_i)
+        except KeyError:
+            table_grid = None
         if table_grid is not None:
             display_boxes.append(
                 DisplayBox(table_grid.bbox, "[Table area]", DisplayType.TABLE_AREA)
             )
             if self.display_grid:
                 display_boxes.extend(
                     [
@@ -332,17 +335,21 @@
                     [
                         (m.gold, DisplayType.ANNOTATION_MATCHED)
                         for m in self.kile_matching[self.docid].matches
                         if m.gold.page == self.page_i
                     ]
                 )
         else:
-            fields_types.extend(
-                [(f, DisplayType.ANNOTATION) for f in annotation.page_fields(self.page_i)]
-            )
+            try:
+                fields_types.extend(
+                    [(f, DisplayType.ANNOTATION) for f in annotation.page_fields(self.page_i)]
+                )
+            except KeyError:
+                # annotations not available, this can happen for test set or unlabeled set
+                pass
             if self.kile_predictions is not None:
                 fields_types.extend(
                     [
                         (f, DisplayType.PREDICTION)
                         for f in self.kile_predictions.get(self.docid, [])
                         if f.page == self.page_i
                     ]
@@ -379,17 +386,21 @@
                             DisplayType.ANNOTATION_MATCHED,
                         )
                         for m in self.lir_matching[self.docid].matches
                         if m.gold.page == self.page_i
                     ]
                 )
         else:
-            fields_types.extend(
-                [(f, DisplayType.ANNOTATION) for f in annotation.page_li_fields(self.page_i)]
-            )
+            try:
+                fields_types.extend(
+                    [(f, DisplayType.ANNOTATION) for f in annotation.page_li_fields(self.page_i)]
+                )
+            except KeyError:
+                # annotations not available, this can happen for test set or unlabeled set
+                pass
             if self.lir_predictions is not None:
                 fields_types.extend(
                     [
                         (f, DisplayType.PREDICTION)
                         for f in self.lir_predictions.get(self.docid, [])
                         if f.page == self.page_i
                     ]
```

### Comparing `docile_benchmark-0.3.0/docile/tools/print_results.py` & `docile_benchmark-0.3.1/docile/tools/print_results.py`

 * *Files identical despite different names*

### Comparing `docile_benchmark-0.3.0/pyproject.toml` & `docile_benchmark-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "docile-benchmark"
-version = "0.3.0"
+version = "0.3.1"
 description = "Tools to work with the DocILE dataset and benchmark"
 authors = [
     "Stepan Simsa <stepan.simsa@rossum.ai>",
     "Matyas Skalicky <matyas.skalicky@rossum.ai>",
     "Milan Sulc <milan.sulc@rossum.ai>",
     "Michal Uricar <michal.uricar@rossum.ai>",
     "Matej Kocian <matej.kocian@rossum.ai>",
```

### Comparing `docile_benchmark-0.3.0/setup.py` & `docile_benchmark-0.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,17 +38,17 @@
 entry_points = \
 {'console_scripts': ['docile_evaluate = docile.cli.evaluate:evaluate',
                      'docile_print_evaluation_report = '
                      'docile.cli.evaluate:print_evaluation_report']}
 
 setup_kwargs = {
     'name': 'docile-benchmark',
-    'version': '0.3.0',
+    'version': '0.3.1',
     'description': 'Tools to work with the DocILE dataset and benchmark',
-    'long_description': '# DocILE: Document Information Localization and Extraction Benchmark\n[![Tests](https://github.com/rossumai/docile/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/rossumai/docile/actions/workflows/tests.yml)\n[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)\n\nRepository to work with the [DocILE dataset and benchmark](https://docile.rossum.ai/), used in the DocILE\'23 CLEF Lab and ICDAR Competition.\nThe competition deadline is on May 10, 2023 and comes with a **$9000 prize pool**.\n\nThe repository consists of:\n* A python library, `docile`, making it easy to load the dataset, work with its annotations, pdfs and pre-computed OCR and run the evaluation.\n* An interactive [dataset browser notebook](docile/tools/dataset_browser.ipynb) to visualize the document annotations, predictions and evaluation results.\n* Baseline methods (will appear soon).\n\nTable of Contents:\n* [Download the dataset](#download-the-dataset)\n* [Installation](#installation)\n* [Predictions format and running evaluation](#predictions-format-and-running-evaluation)\n* [Tasks and evaluation metrics](#tasks-and-evaluation-metrics)\n* [Pre-computed OCR](#pre-computed-ocr)\n* [Development instructions](#development-instructions)\n* [Dataset and benchmark paper](#dataset-and-benchmark-paper)\n\nAlso check [Tutorials](tutorials/) to get quickly started with the repo and [Baselines](baselines/) for the provided baseline solutions.\n\n## Download the dataset\n\nFirst you need to obtain a secret token by following the instructions at https://docile.rossum.ai/. Then download and unzip the dataset by running:\n```bash\n./download_dataset.sh TOKEN annotated-trainval data/docile --unzip\n./download_dataset.sh TOKEN synthetic data/docile --unzip\n./download_dataset.sh TOKEN unlabeled data/docile --unzip\n```\n\nRun `./download_dataset.sh --help` for more options, including how to only show urls (to download\nwith a different tool than curl), how to download smaller unlabeled/synthetic chunks or unlabeled\ndataset without pdfs (with pre-computed OCR only).\n\nYou can also work with the zipped datasets when you turn off image caching (check [Load and sample dataset](tutorials/load_and_sample_dataset.md) tutorial for details).\n\n## Installation\n\n### Option 1: Install as a library\nInstall the library with:\n```shell\npip install docile-benchmark\n```\n\nTo convert pdfs into images, the library uses https://github.com/Belval/pdf2image. On linux you might need to install:\n```shell\napt install poppler-utils\n```\nAnd on macOS:\n\n```shell\nbrew install poppler\n```\n\nNow you have all dependencies to work with the dataset annotations, pdfs, pre-comptued OCR and to run the evaluation. You can install extra dependencies by running the following (although using one of the provided dockerfiles, as explained below, might be easier in this case):\n```shell\npip install "docile-benchmark[interactive]"\npip install "docile-benchmark[ocr]"\n```\n\nThe first line installs additional dependencies allowing you to use the interactive dataset browser in [docile/tools/dataset_browser.py](docile/tools/dataset_browser.py) and the [tutorials](tutorials/). The second line let\'s you rerun the OCR predictions from scratch (e.g., if you\'d like to run it with different parameters) but to make it work, you might need additional dependencies on your system. Check https://github.com/mindee/doctr for the installation instructions (for pytorch).\n\n### Option 2: Use docker\nThere are two Dockerfiles available with the dependencies preinstalled:\n\n* `Dockerfile` is a lighter, CPU-only, version with all necessary dependencies to use the dataset with the pre-computed OCR and interactive browser.\n* `Dockerfile.gpu` has CUDA GPU support and contains additional dependencies needed to recompute OCR predictions from scratch (not needed for standard usage).\n\nYou can use docker compose to manage the docker images. First update the settings in `docker-compose.yml` and the port for jupyter lab in `.env`. Then build the image with:\n```shell\ndocker compose build jupyter[-gpu]\n```\nwhere `jupyter` uses `Dockerfile` and `jupyter-gpu` uses `Dockerfile.gpu`. You can then start the jupyter server:\n```shell\ndocker compose up -d jupyter[-gpu]\n```\n\nJupyter lab can be then accessed at `https://127.0.0.1:${JUPYTER_PORT}` (retrieve the token from logs with `docker compose logs jupyter[-gpu]`). You can also login to the container with:\n```shell\ndocker compose exec jupyter bash\n```\nAfter that run `poetry shell` to activate the virtual environment with the `docile` library and its dependencies installed.\n\n## Predictions format and running evaluation\n\nTo evaluate predictions for tasks KILE or LIR on the test set, you have to make a submission to the benchmark on the [Robust Reading Competition](https://rrc.cvc.uab.es/?ch=26) website. To evaluate on the validation set, use the following command:\n```bash\ndocile_evaluate \\\n  --task LIR \\\n  --dataset-path path/to/dataset[.zip] \\\n  --split val \\\n  --predictions path/to/predictions.json \\\n  --evaluate-x-shot-subsets "0,1-3,4+" \\  # default, show evaluation for 0-shot, few-shot and many-shot layout clusters\n  --evaluate-synthetic-subsets \\  # optional, show evaluation on layout clusters with available synthetic data\n  --evaluate-fieldtypes \\  # optional, show breakdown per fieldtype\n  --evaluate-also-text \\  # optional, evaluate if the text prediction is correct\n  --store-evaluation-result LIR_val_eval.json  # optional, it can be loaded in the dataset browser\n```\n\nRun `docile_evaluate --help` for more information on the options. You can also run `docile_print_evaluation_report --evaluation-result-path LIR_val_eval.json` to print the results of a previously computed evaluation. It is also possible to run evaluation or load the evaluation result directly from code which provides even more options, such as computing metrics just for a single document, specific subset of documents (i.e., documents belonging to the same layout cluster) etc. Check [docile/evaluation/evaluate.py](docile/evaluation/evaluate.py) module for more details.\n\nPredictions need to be stored in a single json file (for each task separately) containing a mapping from `docid` to the predictions for that document, i.e.:\n```json\n{\n    "docid1": [\n        {\n            "page": 0,\n            "bbox": [0.2, 0.1, 0.4, 0.5],\n            "fieldtype": "line_item_order_id",\n            "line_item_id": 3,\n            "score": 0.8,\n            "text": "Order 38",\n            "use_only_for_ap": true\n        },\n        "..."\n    ],\n    "docid2": [{"...": "..."}, "..."],\n    "..."\n}\n```\nExplanation of the individual fields of the predictions:\n  * `page`: page index (from zero) the prediction belongs to\n  * `bbox`: relative coordinates (from 0 to 1) representing the `left`, `top`, `right`, `bottom` sides of the bbox, respectively\n  * `fieldtype`: the fieldtype (sometimes called category or key) of the prediction\n  * `line_item_id`: ID of the line item. This should be a different number for each line item, the order does not matter. Omit for KILE predictions.\n  * `score` [optional]: the confidence for this prediction, can be omitted (in that case predictions are taken in the order in which they are stored in the list)\n  * `text` [optional]: text of the prediction, evaluated in a secondary metric only (when `--evaluate-also-text` is used)\n  * `use_only_for_ap` [optional, default is False]: only use the prediction for AP metric computation, not for f1, precision and recall (useful for less confident predictions).\n\nYou can use [Field class](docile/dataset/field.py) to work with the predictions in code, in which case you can store them in a json file in the required format by using the `docile.dataset.store_predictions` function. You can also use the [BBox class](docile/dataset/bbox.py) to easily convert between relative and absolute coordinates (relative coordinates are used everywhere by default).\n\nUse [docile/tools/print_results.py](docile/tools/print_results.py) to display results of your predictions formatted in a table (choosing from table styles like github, latex or csv).\n\n## Tasks and evaluation metrics\n\nThe DocILE benchmark comes with two tracks, Key Information Localization and Extraction (KILE) and Line Item Recognition (LIR), as described in the [dataset and benchmark paper](#dataset-and-benchmark-paper). In both tracks, the goal is to localize key information of pre-defined categories, i.e., for each document, detect fields with their `fieldtype`, location (`page` and `bbox`) and optionally `text`. For LIR, fields have to be additionally grouped into line items. A Line Item (LI) is a tuple of fields (e.g., description, quantity, and price) describing a single object instance to be extracted, e.g., a row in a table.\n\nEvaluated metrics are Average Precision (AP), F1, precision and recall, computed over all fields across all documents and field types (micro-average). A predicted and a ground truth field can be matched if they have the same `fieldtype` and if they are in the same location, which is decided by the overlap of their bounding boxes with the [provided OCR words](#pre-computed-ocr), described more precisely in the [dataset and benchmark paper](#dataset-and-benchmark-paper):\n\n<img width="500" alt="Definition of Pseudo-Character-Centers and correct localization." src="https://user-images.githubusercontent.com/1220288/222190727-e851a1d9-9c91-438e-bb8d-7ca2066620a4.png">\n\nFor LIR, the fields have to additionally belong to corresponding Line Items. The mapping between `line_item_id` for predicted and ground truth fields is decided by taking the maximum matching which maximizes the total number of matched fields, when considering only fields with `use_only_for_ap=False` (because `use_only_for_ap=True` can be used to include also less confident predictions for AP computation which could negatively affect this matching).\n\nFor both KILE and LIR, the metrics are then computed like this:\n\n* For each document page, find matching between predicted and ground truth fields. If more predicted fields match the same ground truth field, the one with higher `score` is used (but primarily the one with `use_only_for_ap=False`).\n* Order all predictions by descending `score` (but again, predictions with `use_only_for_ap=True` come last). Break ties by the original order in which predictions were provided. See [evaluate.py](docile/evaluation/evaluate.py) for the precise ordering rules. Notice that the order does not influence F1, precision and recall but it influences AP.\n* Compute F1, precision and recall by counting number of true positives and false positives/negatives and AP by iteratively adding predictions and updating precision and recall. We use the COCO style of AP where "gaps are filled", i.e., the precision-recall curve becomes non-increasing.\n\n## Pre-computed OCR\n\nPre-computed OCR is provided with the dataset. The prediction was done using the [DocTR](https://github.com/mindee/doctr) library. On top of that, word boxes were snapped to text (check the code in [docile/dataset/document_ocr.py](docile/dataset/document_ocr.py)). These snapped word boxes are used in evaluation.\n\nTo get the OCR words for a single page, call `document.ocr.get_all_words(page)`, optionally passing `snapped=True` to get the snapped bounding boxes. In some rare cases, the list of words might be empty (when the page is blank). Also notice the predicted words are grouped into blocks. For some models it might be beneficial to re-order the words primarily by lines.\n\nWhile it should not be needed, it is possible to (re)generate OCR from scratch (including the snapping) with the provided `Dockerfile.gpu`. Just delete `DATASET_PATH/ocr` directory and then access the ocr for each document and page with `document.ocr.get_all_words(page, snapped=True)`.\n\n## Development instructions\n\nFor development, install [poetry](https://python-poetry.org/docs/) and run `poetry install`. Start a shell with the virtual environment activated with `poetry shell`. No other dependencies are needed to run pre-commit and the tests. It\'s recommended to use docker (as explained above) if you need the extra (interactive or ocr) dependencies.\n\nInstall pre-commit with `pre-commit install` (don\'t forget you need to prepend all commands with `poetry run ...` if you did not run `poetry shell` first).\n\nRun tests by calling `pytest tests`.\n\n## Dataset and benchmark paper\nThe dataset, the benchmark tasks and the evaluation criteria are described in detail in the [dataset paper](https://arxiv.org/abs/2302.05658). To cite the dataset, please use the following BibTeX entry:\n```\n@misc{simsa2023docile,\n    title={{DocILE} Benchmark for Document Information Localization and Extraction},\n    author={{\\v{S}}imsa, {\\v{S}}t{\\v{e}}p{\\\'a}n and {\\v{S}}ulc, Milan and U{\\v{r}}i{\\v{c}}{\\\'a}{\\v{r}}, Michal and Patel, Yash and Hamdi, Ahmed and Koci{\\\'a}n, Mat{\\v{e}}j and Skalick{\\`y}, Maty{\\\'a}{\\v{s}} and Matas, Ji{\\v{r}}{\\\'\\i} and Doucet, Antoine and Coustaty, Micka{\\"e}l and Karatzas, Dimosthenis},\n    url = {https://arxiv.org/abs/2302.05658},\n    journal={arXiv preprint arXiv:2302.05658},\n    year={2023}\n}\n```\n',
+    'long_description': '# DocILE: Document Information Localization and Extraction Benchmark\n[![Tests](https://github.com/rossumai/docile/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/rossumai/docile/actions/workflows/tests.yml)\n[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)\n\nRepository to work with the [DocILE dataset and benchmark](https://docile.rossum.ai/), used in the DocILE\'23 CLEF Lab and ICDAR Competition.\nThe competition deadline is on May 10, 2023 and comes with a **$9000 prize pool**.\n\nThe repository consists of:\n* A python library, `docile`, making it easy to load the dataset, work with its annotations, pdfs and pre-computed OCR and run the evaluation.\n* An interactive [dataset browser notebook](docile/tools/dataset_browser.ipynb) to visualize the document annotations, predictions and evaluation results.\n* Training and inference scripts for [Baseline methods](baselines/) provided together with pretrained checkpoints and results on test and validation sets.\n* [Tutorials](tutorials/) to get quickly started with the repo.\n\nTable of Contents:\n* [Download the dataset](#download-the-dataset)\n* [Installation](#installation)\n* [Predictions format and running evaluation](#predictions-format-and-running-evaluation)\n* [Tasks and evaluation metrics](#tasks-and-evaluation-metrics)\n* [Pre-computed OCR](#pre-computed-ocr)\n* [Development instructions](#development-instructions)\n* [Dataset and benchmark paper](#dataset-and-benchmark-paper)\n\n## Download the dataset\n\nFirst you need to obtain a secret token by following the instructions at https://docile.rossum.ai/. Then download and unzip the dataset by running:\n```bash\n./download_dataset.sh TOKEN annotated-trainval data/docile --unzip\n./download_dataset.sh TOKEN test data/docile --unzip\n./download_dataset.sh TOKEN synthetic data/docile --unzip\n./download_dataset.sh TOKEN unlabeled data/docile --unzip\n```\n\nRun `./download_dataset.sh --help` for more options, including how to only show urls (to download\nwith a different tool than curl), how to download smaller unlabeled/synthetic chunks or unlabeled\ndataset without pdfs (with pre-computed OCR only).\n\nYou can also work with the zipped datasets when you turn off image caching (check [Load and sample dataset](tutorials/load_and_sample_dataset.md) tutorial for details).\n\n## Installation\n\n### Option 1: Install as a library\nInstall the library with:\n```shell\npip install docile-benchmark\n```\n\nTo convert pdfs into images, the library uses https://github.com/Belval/pdf2image. On linux you might need to install:\n```shell\napt install poppler-utils\n```\nAnd on macOS:\n\n```shell\nbrew install poppler\n```\n\nNow you have all dependencies to work with the dataset annotations, pdfs, pre-comptued OCR and to run the evaluation. You can install extra dependencies by running the following (although using one of the provided dockerfiles, as explained below, might be easier in this case):\n```shell\npip install "docile-benchmark[interactive]"\npip install "docile-benchmark[ocr]"\n```\n\nThe first line installs additional dependencies allowing you to use the interactive dataset browser in [docile/tools/dataset_browser.py](docile/tools/dataset_browser.py) and the [tutorials](tutorials/). The second line let\'s you rerun the OCR predictions from scratch (e.g., if you\'d like to run it with different parameters) but to make it work, you might need additional dependencies on your system. Check https://github.com/mindee/doctr for the installation instructions (for pytorch).\n\n### Option 2: Use docker\nThere are two Dockerfiles available with the dependencies preinstalled:\n\n* `Dockerfile` is a lighter, CPU-only, version with all necessary dependencies to use the dataset with the pre-computed OCR and interactive browser.\n* `Dockerfile.gpu` has CUDA GPU support and contains additional dependencies needed to recompute OCR predictions from scratch (not needed for standard usage).\n\nYou can use docker compose to manage the docker images. First update the settings in `docker-compose.yml` and the port for jupyter lab in `.env`. Then build the image with:\n```shell\ndocker compose build jupyter[-gpu]\n```\nwhere `jupyter` uses `Dockerfile` and `jupyter-gpu` uses `Dockerfile.gpu`. You can then start the jupyter server:\n```shell\ndocker compose up -d jupyter[-gpu]\n```\n\nJupyter lab can be then accessed at `https://127.0.0.1:${JUPYTER_PORT}` (retrieve the token from logs with `docker compose logs jupyter[-gpu]`). You can also login to the container with:\n```shell\ndocker compose exec jupyter bash\n```\nAfter that run `poetry shell` to activate the virtual environment with the `docile` library and its dependencies installed.\n\n## Predictions format and running evaluation\n\nTo evaluate predictions for tasks KILE or LIR on the test set, you have to make a submission to the benchmark on the [Robust Reading Competition](https://rrc.cvc.uab.es/?ch=26) website. To evaluate on the validation set, use the following command:\n```bash\ndocile_evaluate \\\n  --task LIR \\\n  --dataset-path path/to/dataset[.zip] \\\n  --split val \\\n  --predictions path/to/predictions.json \\\n  --evaluate-x-shot-subsets "0,1-3,4+" \\  # default, show evaluation for 0-shot, few-shot and many-shot layout clusters\n  --evaluate-synthetic-subsets \\  # optional, show evaluation on layout clusters with available synthetic data\n  --evaluate-fieldtypes \\  # optional, show breakdown per fieldtype\n  --evaluate-also-text \\  # optional, evaluate if the text prediction is correct\n  --store-evaluation-result LIR_val_eval.json  # optional, it can be loaded in the dataset browser\n```\n\nRun `docile_evaluate --help` for more information on the options. You can also run `docile_print_evaluation_report --evaluation-result-path LIR_val_eval.json` to print the results of a previously computed evaluation. It is also possible to run evaluation or load the evaluation result directly from code which provides even more options, such as computing metrics just for a single document, specific subset of documents (i.e., documents belonging to the same layout cluster) etc. Check [docile/evaluation/evaluate.py](docile/evaluation/evaluate.py) module for more details.\n\nPredictions need to be stored in a single json file (for each task separately) containing a mapping from `docid` to the predictions for that document, i.e.:\n```json\n{\n    "docid1": [\n        {\n            "page": 0,\n            "bbox": [0.2, 0.1, 0.4, 0.5],\n            "fieldtype": "line_item_order_id",\n            "line_item_id": 3,\n            "score": 0.8,\n            "text": "Order 38",\n            "use_only_for_ap": true\n        },\n        "..."\n    ],\n    "docid2": [{"...": "..."}, "..."],\n    "..."\n}\n```\nExplanation of the individual fields of the predictions:\n  * `page`: page index (from zero) the prediction belongs to\n  * `bbox`: relative coordinates (from 0 to 1) representing the `left`, `top`, `right`, `bottom` sides of the bbox, respectively\n  * `fieldtype`: the fieldtype (sometimes called category or key) of the prediction\n  * `line_item_id`: ID of the line item. This should be a different number for each line item, the order does not matter. Omit for KILE predictions.\n  * `score` [optional]: the confidence for this prediction, can be omitted (in that case predictions are taken in the order in which they are stored in the list)\n  * `text` [optional]: text of the prediction, evaluated in a secondary metric only (when `--evaluate-also-text` is used)\n  * `use_only_for_ap` [optional, default is False]: only use the prediction for AP metric computation, not for f1, precision and recall (useful for less confident predictions).\n\nYou can use [Field class](docile/dataset/field.py) to work with the predictions in code, in which case you can store them in a json file in the required format by using the `docile.dataset.store_predictions` function. You can also use the [BBox class](docile/dataset/bbox.py) to easily convert between relative and absolute coordinates (relative coordinates are used everywhere by default).\n\nUse [docile/tools/print_results.py](docile/tools/print_results.py) to display results of your predictions formatted in a table (choosing from table styles like github, latex or csv).\n\n## Tasks and evaluation metrics\n\nThe DocILE benchmark comes with two tracks, Key Information Localization and Extraction (KILE) and Line Item Recognition (LIR), as described in the [dataset and benchmark paper](#dataset-and-benchmark-paper). In both tracks, the goal is to localize key information of pre-defined categories, i.e., for each document, detect fields with their `fieldtype`, location (`page` and `bbox`) and optionally `text`. For LIR, fields have to be additionally grouped into line items. A Line Item (LI) is a tuple of fields (e.g., description, quantity, and price) describing a single object instance to be extracted, e.g., a row in a table.\n\nEvaluated metrics are Average Precision (AP), F1, precision and recall, computed over all fields across all documents and field types (micro-average). A predicted and a ground truth field can be matched if they have the same `fieldtype` and if they are in the same location, which is decided by the overlap of their bounding boxes with the [provided OCR words](#pre-computed-ocr), described more precisely in the [dataset and benchmark paper](#dataset-and-benchmark-paper):\n\n<img width="500" alt="Definition of Pseudo-Character-Centers and correct localization." src="https://user-images.githubusercontent.com/1220288/222190727-e851a1d9-9c91-438e-bb8d-7ca2066620a4.png">\n\nFor LIR, the fields have to additionally belong to corresponding Line Items. The mapping between `line_item_id` for predicted and ground truth fields is decided by taking the maximum matching which maximizes the total number of matched fields, when considering only fields with `use_only_for_ap=False` (because `use_only_for_ap=True` can be used to include also less confident predictions for AP computation which could negatively affect this matching).\n\nFor both KILE and LIR, the metrics are then computed like this:\n\n* For each document page, find matching between predicted and ground truth fields. If more predicted fields match the same ground truth field, the one with higher `score` is used (but primarily the one with `use_only_for_ap=False`).\n* Order all predictions by descending `score` (but again, predictions with `use_only_for_ap=True` come last). Break ties by the original order in which predictions were provided. See [evaluate.py](docile/evaluation/evaluate.py) for the precise ordering rules. Notice that the order does not influence F1, precision and recall but it influences AP.\n* Compute F1, precision and recall by counting number of true positives and false positives/negatives and AP by iteratively adding predictions and updating precision and recall. We use the COCO style of AP where "gaps are filled", i.e., the precision-recall curve becomes non-increasing.\n\n## Pre-computed OCR\n\nPre-computed OCR is provided with the dataset. The prediction was done using the [DocTR](https://github.com/mindee/doctr) library. On top of that, word boxes were snapped to text (check the code in [docile/dataset/document_ocr.py](docile/dataset/document_ocr.py)). These snapped word boxes are used in evaluation.\n\nTo get the OCR words for a single page, call `document.ocr.get_all_words(page)`, optionally passing `snapped=True` to get the snapped bounding boxes. In some rare cases, the list of words might be empty (when the page is blank). Also notice the predicted words are grouped into blocks. For some models it might be beneficial to re-order the words primarily by lines.\n\nWhile it should not be needed, it is possible to (re)generate OCR from scratch (including the snapping) with the provided `Dockerfile.gpu`. Just delete `DATASET_PATH/ocr` directory and then access the ocr for each document and page with `document.ocr.get_all_words(page, snapped=True)`.\n\n## Development instructions\n\nFor development, install [poetry](https://python-poetry.org/docs/) and run `poetry install`. Start a shell with the virtual environment activated with `poetry shell`. No other dependencies are needed to run pre-commit and the tests. It\'s recommended to use docker (as explained above) if you need the extra (interactive or ocr) dependencies.\n\nInstall pre-commit with `pre-commit install` (don\'t forget you need to prepend all commands with `poetry run ...` if you did not run `poetry shell` first).\n\nRun tests by calling `pytest tests`.\n\n## Dataset and benchmark paper\nThe dataset, the benchmark tasks and the evaluation criteria are described in detail in the [dataset paper](https://arxiv.org/abs/2302.05658). To cite the dataset, please use the following BibTeX entry:\n```\n@misc{simsa2023docile,\n    title={{DocILE} Benchmark for Document Information Localization and Extraction},\n    author={{\\v{S}}imsa, {\\v{S}}t{\\v{e}}p{\\\'a}n and {\\v{S}}ulc, Milan and U{\\v{r}}i{\\v{c}}{\\\'a}{\\v{r}}, Michal and Patel, Yash and Hamdi, Ahmed and Koci{\\\'a}n, Mat{\\v{e}}j and Skalick{\\`y}, Maty{\\\'a}{\\v{s}} and Matas, Ji{\\v{r}}{\\\'\\i} and Doucet, Antoine and Coustaty, Micka{\\"e}l and Karatzas, Dimosthenis},\n    url = {https://arxiv.org/abs/2302.05658},\n    journal={arXiv preprint arXiv:2302.05658},\n    year={2023}\n}\n```\n',
     'author': 'Stepan Simsa',
     'author_email': 'stepan.simsa@rossum.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://docile.rossum.ai/',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `docile_benchmark-0.3.0/PKG-INFO` & `docile_benchmark-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docile-benchmark
-Version: 0.3.0
+Version: 0.3.1
 Summary: Tools to work with the DocILE dataset and benchmark
 Home-page: https://docile.rossum.ai/
 Author: Stepan Simsa
 Author-email: stepan.simsa@rossum.ai
 Requires-Python: >=3.8.2,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -44,32 +44,32 @@
 
 Repository to work with the [DocILE dataset and benchmark](https://docile.rossum.ai/), used in the DocILE'23 CLEF Lab and ICDAR Competition.
 The competition deadline is on May 10, 2023 and comes with a **$9000 prize pool**.
 
 The repository consists of:
 * A python library, `docile`, making it easy to load the dataset, work with its annotations, pdfs and pre-computed OCR and run the evaluation.
 * An interactive [dataset browser notebook](docile/tools/dataset_browser.ipynb) to visualize the document annotations, predictions and evaluation results.
-* Baseline methods (will appear soon).
+* Training and inference scripts for [Baseline methods](baselines/) provided together with pretrained checkpoints and results on test and validation sets.
+* [Tutorials](tutorials/) to get quickly started with the repo.
 
 Table of Contents:
 * [Download the dataset](#download-the-dataset)
 * [Installation](#installation)
 * [Predictions format and running evaluation](#predictions-format-and-running-evaluation)
 * [Tasks and evaluation metrics](#tasks-and-evaluation-metrics)
 * [Pre-computed OCR](#pre-computed-ocr)
 * [Development instructions](#development-instructions)
 * [Dataset and benchmark paper](#dataset-and-benchmark-paper)
 
-Also check [Tutorials](tutorials/) to get quickly started with the repo and [Baselines](baselines/) for the provided baseline solutions.
-
 ## Download the dataset
 
 First you need to obtain a secret token by following the instructions at https://docile.rossum.ai/. Then download and unzip the dataset by running:
 ```bash
 ./download_dataset.sh TOKEN annotated-trainval data/docile --unzip
+./download_dataset.sh TOKEN test data/docile --unzip
 ./download_dataset.sh TOKEN synthetic data/docile --unzip
 ./download_dataset.sh TOKEN unlabeled data/docile --unzip
 ```
 
 Run `./download_dataset.sh --help` for more options, including how to only show urls (to download
 with a different tool than curl), how to download smaller unlabeled/synthetic chunks or unlabeled
 dataset without pdfs (with pre-computed OCR only).
```

