# Comparing `tmp/pv_evaluation-2.1.0.tar.gz` & `tmp/pv_evaluation-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pv_evaluation-2.1.0.tar", last modified: Mon Mar 27 22:01:23 2023, max compression
+gzip compressed data, was "pv_evaluation-2.1.1.tar", last modified: Tue Apr 25 15:29:38 2023, max compression
```

## Comparing `pv_evaluation-2.1.0.tar` & `pv_evaluation-2.1.1.tar`

### file list

```diff
@@ -1,56 +1,58 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-27 22:01:23.334209 pv_evaluation-2.1.0/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    35149 2022-11-23 20:45:03.000000 pv_evaluation-2.1.0/LICENSE.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      290 2022-12-02 16:28:47.000000 pv_evaluation-2.1.0/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6626 2023-03-27 22:01:23.334209 pv_evaluation-2.1.0/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6287 2023-03-27 21:06:38.000000 pv_evaluation-2.1.0/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-27 22:01:23.318209 pv_evaluation-2.1.0/pv_evaluation/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      113 2022-11-23 20:45:03.000000 pv_evaluation-2.1.0/pv_evaluation/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-27 22:01:23.318209 pv_evaluation-2.1.0/pv_evaluation/benchmark/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1512 2023-03-27 21:05:59.000000 pv_evaluation-2.1.0/pv_evaluation/benchmark/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10644 2023-03-27 21:05:34.000000 pv_evaluation-2.1.0/pv_evaluation/benchmark/data.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15909 2023-03-27 21:25:54.000000 pv_evaluation-2.1.0/pv_evaluation/benchmark/report.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-27 22:01:23.318209 pv_evaluation-2.1.0/pv_evaluation/data/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       27 2022-11-23 20:45:03.000000 pv_evaluation-2.1.0/pv_evaluation/data/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-27 22:01:23.318209 pv_evaluation-2.1.0/pv_evaluation/data/assignee/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-11-23 20:45:03.000000 pv_evaluation-2.1.0/pv_evaluation/data/assignee/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-27 22:01:23.322209 pv_evaluation-2.1.0/pv_evaluation/data/inventor/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-11-23 20:45:03.000000 pv_evaluation-2.1.0/pv_evaluation/data/inventor/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  4920202 2023-03-20 18:40:32.000000 pv_evaluation-2.1.0/pv_evaluation/data/inventor/als-inventors.csv
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   416200 2022-12-02 16:28:47.000000 pv_evaluation-2.1.0/pv_evaluation/data/inventor/binette-2022-inventors-benchmark.csv
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   350236 2023-03-20 18:39:42.000000 pv_evaluation-2.1.0/pv_evaluation/data/inventor/ens-inventors.csv
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   286379 2023-03-20 18:37:10.000000 pv_evaluation-2.1.0/pv_evaluation/data/inventor/israeli-inventors-benchmark.csv
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    41391 2023-03-20 18:38:51.000000 pv_evaluation-2.1.0/pv_evaluation/data/inventor/lai-2011-benchmark.csv
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2907 2023-03-20 18:38:00.000000 pv_evaluation-2.1.0/pv_evaluation/data/inventor/patentsview-inventors-benchmark.csv
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-27 22:01:23.326209 pv_evaluation-2.1.0/pv_evaluation/templates/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      149 2022-11-23 20:45:03.000000 pv_evaluation-2.1.0/pv_evaluation/templates/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-27 22:01:23.326209 pv_evaluation-2.1.0/pv_evaluation/templates/inventor/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      478 2022-12-02 16:28:47.000000 pv_evaluation-2.1.0/pv_evaluation/templates/inventor/0-report.qmd
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      590 2023-02-10 00:04:51.000000 pv_evaluation-2.1.0/pv_evaluation/templates/inventor/1-header.qmd
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2958 2023-02-10 00:04:52.000000 pv_evaluation-2.1.0/pv_evaluation/templates/inventor/2-summary.qmd
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4130 2022-12-02 16:28:47.000000 pv_evaluation-2.1.0/pv_evaluation/templates/inventor/3-benchmark.qmd
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-11-23 20:45:03.000000 pv_evaluation-2.1.0/pv_evaluation/templates/inventor/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-27 22:01:23.334209 pv_evaluation-2.1.0/pv_evaluation/templates/inventor/callouts/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-11-23 20:45:03.000000 pv_evaluation-2.1.0/pv_evaluation/templates/inventor/callouts/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      676 2022-11-23 20:45:03.000000 pv_evaluation-2.1.0/pv_evaluation/templates/inventor/callouts/between-cluster-tips.qmd
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      769 2022-11-23 20:45:03.000000 pv_evaluation-2.1.0/pv_evaluation/templates/inventor/callouts/cluster-errors-tips.qmd
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1224 2022-11-23 20:45:03.000000 pv_evaluation-2.1.0/pv_evaluation/templates/inventor/callouts/cluster-homogeneity-tips.qmd
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      747 2022-11-23 20:45:03.000000 pv_evaluation-2.1.0/pv_evaluation/templates/inventor/callouts/cluster-sizes-tips.qmd
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1815 2022-11-23 20:45:03.000000 pv_evaluation-2.1.0/pv_evaluation/templates/inventor/callouts/entropy-tips.qmd
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1472 2022-11-23 20:45:03.000000 pv_evaluation-2.1.0/pv_evaluation/templates/inventor/callouts/metrics-tips.qmd
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      476 2022-11-23 20:45:03.000000 pv_evaluation-2.1.0/pv_evaluation/templates/inventor/callouts/top-inventors-tips.qmd
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    45233 2022-11-23 20:45:03.000000 pv_evaluation-2.1.0/pv_evaluation/templates/inventor/footer.html
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      106 2022-11-23 20:45:03.000000 pv_evaluation-2.1.0/pv_evaluation/templates/inventor/header.html
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2133 2023-03-27 21:05:34.000000 pv_evaluation-2.1.0/pv_evaluation/templates/render.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-27 22:01:23.318209 pv_evaluation-2.1.0/pv_evaluation.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6626 2023-03-27 22:01:23.000000 pv_evaluation-2.1.0/pv_evaluation.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1789 2023-03-27 22:01:23.000000 pv_evaluation-2.1.0/pv_evaluation.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-03-27 22:01:23.000000 pv_evaluation-2.1.0/pv_evaluation.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      129 2023-03-27 22:01:23.000000 pv_evaluation-2.1.0/pv_evaluation.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       14 2023-03-27 22:01:23.000000 pv_evaluation-2.1.0/pv_evaluation.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-27 22:01:23.318209 pv_evaluation-2.1.0/scripts/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-27 22:01:23.334209 pv_evaluation-2.1.0/scripts/hand-disambiguation/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5885 2023-03-27 21:05:34.000000 pv_evaluation-2.1.0/scripts/hand-disambiguation/process-inventors-hand-disambiguation.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-03-27 22:01:23.334209 pv_evaluation-2.1.0/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1222 2023-03-27 22:00:31.000000 pv_evaluation-2.1.0/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-27 22:01:23.334209 pv_evaluation-2.1.0/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      161 2022-12-02 16:28:47.000000 pv_evaluation-2.1.0/tests/test_notebooks.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 15:29:38.864360 pv_evaluation-2.1.1/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    35149 2022-11-23 20:45:03.000000 pv_evaluation-2.1.1/LICENSE.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      332 2023-04-25 15:27:37.000000 pv_evaluation-2.1.1/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6626 2023-04-25 15:29:38.864360 pv_evaluation-2.1.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6287 2023-03-27 21:06:38.000000 pv_evaluation-2.1.1/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 15:29:38.844360 pv_evaluation-2.1.1/pv_evaluation/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      113 2022-11-23 20:45:03.000000 pv_evaluation-2.1.1/pv_evaluation/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 15:29:38.844360 pv_evaluation-2.1.1/pv_evaluation/benchmark/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1512 2023-03-27 21:05:59.000000 pv_evaluation-2.1.1/pv_evaluation/benchmark/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10644 2023-03-27 21:05:34.000000 pv_evaluation-2.1.1/pv_evaluation/benchmark/data.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15909 2023-03-27 21:25:54.000000 pv_evaluation-2.1.1/pv_evaluation/benchmark/report.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 15:29:38.844360 pv_evaluation-2.1.1/pv_evaluation/data/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       27 2022-11-23 20:45:03.000000 pv_evaluation-2.1.1/pv_evaluation/data/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 15:29:38.848360 pv_evaluation-2.1.1/pv_evaluation/data/assignee/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-11-23 20:45:03.000000 pv_evaluation-2.1.1/pv_evaluation/data/assignee/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000) 10128377 2023-03-20 18:41:09.000000 pv_evaluation-2.1.1/pv_evaluation/data/assignee/air-umass-assignees-benchmark.csv
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000) 15675077 2023-03-20 18:41:29.000000 pv_evaluation-2.1.1/pv_evaluation/data/assignee/nber-subset-assignees-benchmark.csv
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 15:29:38.864360 pv_evaluation-2.1.1/pv_evaluation/data/inventor/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-11-23 20:45:03.000000 pv_evaluation-2.1.1/pv_evaluation/data/inventor/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  4920202 2023-03-20 18:40:32.000000 pv_evaluation-2.1.1/pv_evaluation/data/inventor/als-inventors.csv
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   416200 2022-12-02 16:28:47.000000 pv_evaluation-2.1.1/pv_evaluation/data/inventor/binette-2022-inventors-benchmark.csv
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   350236 2023-03-20 18:39:42.000000 pv_evaluation-2.1.1/pv_evaluation/data/inventor/ens-inventors.csv
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   286379 2023-03-20 18:37:10.000000 pv_evaluation-2.1.1/pv_evaluation/data/inventor/israeli-inventors-benchmark.csv
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    41391 2023-03-20 18:38:51.000000 pv_evaluation-2.1.1/pv_evaluation/data/inventor/lai-2011-benchmark.csv
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2907 2023-03-20 18:38:00.000000 pv_evaluation-2.1.1/pv_evaluation/data/inventor/patentsview-inventors-benchmark.csv
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 15:29:38.864360 pv_evaluation-2.1.1/pv_evaluation/templates/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      149 2022-11-23 20:45:03.000000 pv_evaluation-2.1.1/pv_evaluation/templates/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 15:29:38.864360 pv_evaluation-2.1.1/pv_evaluation/templates/inventor/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      478 2022-12-02 16:28:47.000000 pv_evaluation-2.1.1/pv_evaluation/templates/inventor/0-report.qmd
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      590 2023-02-10 00:04:51.000000 pv_evaluation-2.1.1/pv_evaluation/templates/inventor/1-header.qmd
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2958 2023-02-10 00:04:52.000000 pv_evaluation-2.1.1/pv_evaluation/templates/inventor/2-summary.qmd
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4130 2022-12-02 16:28:47.000000 pv_evaluation-2.1.1/pv_evaluation/templates/inventor/3-benchmark.qmd
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-11-23 20:45:03.000000 pv_evaluation-2.1.1/pv_evaluation/templates/inventor/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 15:29:38.864360 pv_evaluation-2.1.1/pv_evaluation/templates/inventor/callouts/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-11-23 20:45:03.000000 pv_evaluation-2.1.1/pv_evaluation/templates/inventor/callouts/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      676 2022-11-23 20:45:03.000000 pv_evaluation-2.1.1/pv_evaluation/templates/inventor/callouts/between-cluster-tips.qmd
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      769 2022-11-23 20:45:03.000000 pv_evaluation-2.1.1/pv_evaluation/templates/inventor/callouts/cluster-errors-tips.qmd
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1224 2022-11-23 20:45:03.000000 pv_evaluation-2.1.1/pv_evaluation/templates/inventor/callouts/cluster-homogeneity-tips.qmd
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      747 2022-11-23 20:45:03.000000 pv_evaluation-2.1.1/pv_evaluation/templates/inventor/callouts/cluster-sizes-tips.qmd
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1815 2022-11-23 20:45:03.000000 pv_evaluation-2.1.1/pv_evaluation/templates/inventor/callouts/entropy-tips.qmd
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1472 2022-11-23 20:45:03.000000 pv_evaluation-2.1.1/pv_evaluation/templates/inventor/callouts/metrics-tips.qmd
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      476 2022-11-23 20:45:03.000000 pv_evaluation-2.1.1/pv_evaluation/templates/inventor/callouts/top-inventors-tips.qmd
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    45233 2022-11-23 20:45:03.000000 pv_evaluation-2.1.1/pv_evaluation/templates/inventor/footer.html
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      106 2022-11-23 20:45:03.000000 pv_evaluation-2.1.1/pv_evaluation/templates/inventor/header.html
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2133 2023-03-27 21:05:34.000000 pv_evaluation-2.1.1/pv_evaluation/templates/render.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 15:29:38.844360 pv_evaluation-2.1.1/pv_evaluation.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6626 2023-04-25 15:29:38.000000 pv_evaluation-2.1.1/pv_evaluation.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1915 2023-04-25 15:29:38.000000 pv_evaluation-2.1.1/pv_evaluation.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-25 15:29:38.000000 pv_evaluation-2.1.1/pv_evaluation.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      129 2023-04-25 15:29:38.000000 pv_evaluation-2.1.1/pv_evaluation.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       14 2023-04-25 15:29:38.000000 pv_evaluation-2.1.1/pv_evaluation.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 15:29:38.840360 pv_evaluation-2.1.1/scripts/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 15:29:38.864360 pv_evaluation-2.1.1/scripts/hand-disambiguation/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5885 2023-03-27 21:05:34.000000 pv_evaluation-2.1.1/scripts/hand-disambiguation/process-inventors-hand-disambiguation.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-04-25 15:29:38.864360 pv_evaluation-2.1.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1222 2023-04-25 15:28:48.000000 pv_evaluation-2.1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 15:29:38.864360 pv_evaluation-2.1.1/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      161 2022-12-02 16:28:47.000000 pv_evaluation-2.1.1/tests/test_notebooks.py
```

### Comparing `pv_evaluation-2.1.0/LICENSE.txt` & `pv_evaluation-2.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pv_evaluation-2.1.0/PKG-INFO` & `pv_evaluation-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pv_evaluation
-Version: 2.1.0
+Version: 2.1.1
 Summary: Tools to evaluate PatentsView's disambiguation algorithms
 Home-page: https://github.com/OlivierBinette/PatentsView-Evaluation
 Author: Olivier Binette, Sarvo Madhavan
 Author-email: olivier.binette@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `pv_evaluation-2.1.0/README.md` & `pv_evaluation-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pv_evaluation-2.1.0/pv_evaluation/benchmark/__init__.py` & `pv_evaluation-2.1.1/pv_evaluation/benchmark/__init__.py`

 * *Files identical despite different names*

### Comparing `pv_evaluation-2.1.0/pv_evaluation/benchmark/data.py` & `pv_evaluation-2.1.1/pv_evaluation/benchmark/data.py`

 * *Files identical despite different names*

### Comparing `pv_evaluation-2.1.0/pv_evaluation/benchmark/report.py` & `pv_evaluation-2.1.1/pv_evaluation/benchmark/report.py`

 * *Files identical despite different names*

### Comparing `pv_evaluation-2.1.0/pv_evaluation/data/inventor/als-inventors.csv` & `pv_evaluation-2.1.1/pv_evaluation/data/inventor/als-inventors.csv`

 * *Files identical despite different names*

### Comparing `pv_evaluation-2.1.0/pv_evaluation/data/inventor/binette-2022-inventors-benchmark.csv` & `pv_evaluation-2.1.1/pv_evaluation/data/inventor/binette-2022-inventors-benchmark.csv`

 * *Files identical despite different names*

### Comparing `pv_evaluation-2.1.0/pv_evaluation/data/inventor/ens-inventors.csv` & `pv_evaluation-2.1.1/pv_evaluation/data/inventor/ens-inventors.csv`

 * *Files identical despite different names*

### Comparing `pv_evaluation-2.1.0/pv_evaluation/data/inventor/israeli-inventors-benchmark.csv` & `pv_evaluation-2.1.1/pv_evaluation/data/inventor/israeli-inventors-benchmark.csv`

 * *Files identical despite different names*

### Comparing `pv_evaluation-2.1.0/pv_evaluation/data/inventor/lai-2011-benchmark.csv` & `pv_evaluation-2.1.1/pv_evaluation/data/inventor/lai-2011-benchmark.csv`

 * *Files identical despite different names*

### Comparing `pv_evaluation-2.1.0/pv_evaluation/data/inventor/patentsview-inventors-benchmark.csv` & `pv_evaluation-2.1.1/pv_evaluation/data/inventor/patentsview-inventors-benchmark.csv`

 * *Files identical despite different names*

### Comparing `pv_evaluation-2.1.0/pv_evaluation/templates/inventor/1-header.qmd` & `pv_evaluation-2.1.1/pv_evaluation/templates/inventor/1-header.qmd`

 * *Files identical despite different names*

### Comparing `pv_evaluation-2.1.0/pv_evaluation/templates/inventor/2-summary.qmd` & `pv_evaluation-2.1.1/pv_evaluation/templates/inventor/2-summary.qmd`

 * *Files identical despite different names*

### Comparing `pv_evaluation-2.1.0/pv_evaluation/templates/inventor/3-benchmark.qmd` & `pv_evaluation-2.1.1/pv_evaluation/templates/inventor/3-benchmark.qmd`

 * *Files identical despite different names*

### Comparing `pv_evaluation-2.1.0/pv_evaluation/templates/inventor/callouts/between-cluster-tips.qmd` & `pv_evaluation-2.1.1/pv_evaluation/templates/inventor/callouts/between-cluster-tips.qmd`

 * *Files identical despite different names*

### Comparing `pv_evaluation-2.1.0/pv_evaluation/templates/inventor/callouts/cluster-errors-tips.qmd` & `pv_evaluation-2.1.1/pv_evaluation/templates/inventor/callouts/cluster-errors-tips.qmd`

 * *Files identical despite different names*

### Comparing `pv_evaluation-2.1.0/pv_evaluation/templates/inventor/callouts/cluster-homogeneity-tips.qmd` & `pv_evaluation-2.1.1/pv_evaluation/templates/inventor/callouts/cluster-homogeneity-tips.qmd`

 * *Files identical despite different names*

### Comparing `pv_evaluation-2.1.0/pv_evaluation/templates/inventor/callouts/cluster-sizes-tips.qmd` & `pv_evaluation-2.1.1/pv_evaluation/templates/inventor/callouts/cluster-sizes-tips.qmd`

 * *Files identical despite different names*

### Comparing `pv_evaluation-2.1.0/pv_evaluation/templates/inventor/callouts/entropy-tips.qmd` & `pv_evaluation-2.1.1/pv_evaluation/templates/inventor/callouts/entropy-tips.qmd`

 * *Files identical despite different names*

### Comparing `pv_evaluation-2.1.0/pv_evaluation/templates/inventor/callouts/metrics-tips.qmd` & `pv_evaluation-2.1.1/pv_evaluation/templates/inventor/callouts/metrics-tips.qmd`

 * *Files identical despite different names*

### Comparing `pv_evaluation-2.1.0/pv_evaluation/templates/inventor/footer.html` & `pv_evaluation-2.1.1/pv_evaluation/templates/inventor/footer.html`

 * *Files identical despite different names*

### Comparing `pv_evaluation-2.1.0/pv_evaluation/templates/render.py` & `pv_evaluation-2.1.1/pv_evaluation/templates/render.py`

 * *Files identical despite different names*

### Comparing `pv_evaluation-2.1.0/pv_evaluation.egg-info/PKG-INFO` & `pv_evaluation-2.1.1/pv_evaluation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pv-evaluation
-Version: 2.1.0
+Version: 2.1.1
 Summary: Tools to evaluate PatentsView's disambiguation algorithms
 Home-page: https://github.com/OlivierBinette/PatentsView-Evaluation
 Author: Olivier Binette, Sarvo Madhavan
 Author-email: olivier.binette@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `pv_evaluation-2.1.0/pv_evaluation.egg-info/SOURCES.txt` & `pv_evaluation-2.1.1/pv_evaluation.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 pv_evaluation.egg-info/requires.txt
 pv_evaluation.egg-info/top_level.txt
 pv_evaluation/benchmark/__init__.py
 pv_evaluation/benchmark/data.py
 pv_evaluation/benchmark/report.py
 pv_evaluation/data/__init__.py
 pv_evaluation/data/assignee/__init__.py
+pv_evaluation/data/assignee/air-umass-assignees-benchmark.csv
+pv_evaluation/data/assignee/nber-subset-assignees-benchmark.csv
 pv_evaluation/data/inventor/__init__.py
 pv_evaluation/data/inventor/als-inventors.csv
 pv_evaluation/data/inventor/binette-2022-inventors-benchmark.csv
 pv_evaluation/data/inventor/ens-inventors.csv
 pv_evaluation/data/inventor/israeli-inventors-benchmark.csv
 pv_evaluation/data/inventor/lai-2011-benchmark.csv
 pv_evaluation/data/inventor/patentsview-inventors-benchmark.csv
```

### Comparing `pv_evaluation-2.1.0/scripts/hand-disambiguation/process-inventors-hand-disambiguation.py` & `pv_evaluation-2.1.1/scripts/hand-disambiguation/process-inventors-hand-disambiguation.py`

 * *Files identical despite different names*

### Comparing `pv_evaluation-2.1.0/setup.py` & `pv_evaluation-2.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 if __name__ == "__main__":
     setup(
         name="pv_evaluation",
-        version="2.1.0",
+        version="2.1.1",
         license_files=("LICENSE.txt",),
         author="Olivier Binette, Sarvo Madhavan",
         author_email="olivier.binette@gmail.com",
         description="Tools to evaluate PatentsView's disambiguation algorithms",
         long_description=long_description,
         long_description_content_type="text/markdown",
         url="https://github.com/OlivierBinette/PatentsView-Evaluation",
```

