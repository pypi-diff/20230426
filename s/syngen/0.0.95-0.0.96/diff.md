# Comparing `tmp/syngen-0.0.95.tar.gz` & `tmp/syngen-0.0.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syngen-0.0.95.tar", last modified: Mon Apr 24 07:03:08 2023, max compression
+gzip compressed data, was "syngen-0.0.96.tar", last modified: Tue Apr 25 15:53:52 2023, max compression
```

## Comparing `syngen-0.0.95.tar` & `syngen-0.0.96.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 07:03:08.776894 syngen-0.0.95/
--rw-r--r--   0 runner    (1001) docker     (122)      400 2023-04-24 07:01:37.000000 syngen-0.0.95/DESCRIPTION
--rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-04-24 07:01:37.000000 syngen-0.0.95/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      133 2023-04-24 07:01:37.000000 syngen-0.0.95/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    14888 2023-04-24 07:03:08.776894 syngen-0.0.95/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    14148 2023-04-24 07:01:37.000000 syngen-0.0.95/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       99 2023-04-24 07:01:37.000000 syngen-0.0.95/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)     1307 2023-04-24 07:03:08.776894 syngen-0.0.95/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 07:03:08.760894 syngen-0.0.95/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 07:03:08.764894 syngen-0.0.95/src/syngen/
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/VERSION
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2935 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/infer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 07:03:08.768894 syngen-0.0.95/src/syngen/ml/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/ml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 07:03:08.768894 syngen-0.0.95/src/syngen/ml/config/
--rw-r--r--   0 runner    (1001) docker     (122)      112 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/ml/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10094 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/ml/config/configurations.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 07:03:08.768894 syngen-0.0.95/src/syngen/ml/convertor/
--rw-r--r--   0 runner    (1001) docker     (122)      163 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/ml/convertor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2858 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/ml/convertor/convertor.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 07:03:08.768894 syngen-0.0.95/src/syngen/ml/data_loaders/
--rw-r--r--   0 runner    (1001) docker     (122)      172 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/ml/data_loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7294 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/ml/data_loaders/data_loaders.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 07:03:08.768894 syngen-0.0.95/src/syngen/ml/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)      751 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/ml/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 07:03:08.768894 syngen-0.0.95/src/syngen/ml/metrics/accuracy_test/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/ml/metrics/accuracy_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)   723100 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/ml/metrics/accuracy_test/accuracy_report.html
--rw-r--r--   0 runner    (1001) docker     (122)     5496 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/ml/metrics/accuracy_test/accuracy_test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 07:03:08.760894 syngen-0.0.95/src/syngen/ml/metrics/accuracy_test/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 07:03:08.768894 syngen-0.0.95/src/syngen/ml/metrics/accuracy_test/src/fonts/
--rw-r--r--   0 runner    (1001) docker     (122)   528976 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 07:03:08.772894 syngen-0.0.95/src/syngen/ml/metrics/metrics_classes/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/ml/metrics/metrics_classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    43412 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/ml/metrics/metrics_classes/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 07:03:08.772894 syngen-0.0.95/src/syngen/ml/metrics/sample_test/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/ml/metrics/sample_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)   708975 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/ml/metrics/sample_test/sample_report_template.html
--rw-r--r--   0 runner    (1001) docker     (122)     1958 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/ml/metrics/sample_test/sample_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1250 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/ml/metrics/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 07:03:08.772894 syngen-0.0.95/src/syngen/ml/reporters/
--rw-r--r--   0 runner    (1001) docker     (122)      224 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/ml/reporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6256 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/ml/reporters/reporters.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 07:03:08.772894 syngen-0.0.95/src/syngen/ml/strategies/
--rw-r--r--   0 runner    (1001) docker     (122)      169 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/ml/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6945 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/ml/strategies/strategies.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 07:03:08.772894 syngen-0.0.95/src/syngen/ml/train_chain/
--rw-r--r--   0 runner    (1001) docker     (122)      303 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/ml/train_chain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15923 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/ml/train_chain/train_chain.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 07:03:08.772894 syngen-0.0.95/src/syngen/ml/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/ml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5323 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/ml/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 07:03:08.772894 syngen-0.0.95/src/syngen/ml/vae/
--rw-r--r--   0 runner    (1001) docker     (122)      173 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/ml/vae/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 07:03:08.776894 syngen-0.0.95/src/syngen/ml/vae/models/
--rw-r--r--   0 runner    (1001) docker     (122)       49 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/ml/vae/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2085 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/ml/vae/models/custom_layers.py
--rw-r--r--   0 runner    (1001) docker     (122)    28464 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/ml/vae/models/dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)    24693 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/ml/vae/models/features.py
--rw-r--r--   0 runner    (1001) docker     (122)    10390 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/ml/vae/models/model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 07:03:08.776894 syngen-0.0.95/src/syngen/ml/vae/wrappers/
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/ml/vae/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11009 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/ml/vae/wrappers/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 07:03:08.776894 syngen-0.0.95/src/syngen/ml/validation_schema/
--rw-r--r--   0 runner    (1001) docker     (122)      153 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/ml/validation_schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1795 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/ml/validation_schema/validation_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 07:03:08.776894 syngen-0.0.95/src/syngen/ml/worker/
--rw-r--r--   0 runner    (1001) docker     (122)       43 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/ml/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13012 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/ml/worker/worker.py
--rw-r--r--   0 runner    (1001) docker     (122)     3976 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/train.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 07:03:08.768894 syngen-0.0.95/src/syngen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    14888 2023-04-24 07:03:08.000000 syngen-0.0.95/src/syngen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1902 2023-04-24 07:03:08.000000 syngen-0.0.95/src/syngen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-24 07:03:08.000000 syngen-0.0.95/src/syngen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       86 2023-04-24 07:03:08.000000 syngen-0.0.95/src/syngen.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      299 2023-04-24 07:03:08.000000 syngen-0.0.95/src/syngen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-04-24 07:03:08.000000 syngen-0.0.95/src/syngen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 15:53:52.656111 syngen-0.0.96/
+-rw-r--r--   0 runner    (1001) docker     (122)      400 2023-04-25 15:52:30.000000 syngen-0.0.96/DESCRIPTION
+-rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-04-25 15:52:30.000000 syngen-0.0.96/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      133 2023-04-25 15:52:30.000000 syngen-0.0.96/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    14888 2023-04-25 15:53:52.656111 syngen-0.0.96/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    14148 2023-04-25 15:52:30.000000 syngen-0.0.96/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       99 2023-04-25 15:52:30.000000 syngen-0.0.96/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     1307 2023-04-25 15:53:52.660111 syngen-0.0.96/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 15:53:52.632110 syngen-0.0.96/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 15:53:52.640111 syngen-0.0.96/src/syngen/
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/VERSION
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2935 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/infer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 15:53:52.644111 syngen-0.0.96/src/syngen/ml/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/ml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 15:53:52.644111 syngen-0.0.96/src/syngen/ml/config/
+-rw-r--r--   0 runner    (1001) docker     (122)      112 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/ml/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10053 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/ml/config/configurations.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 15:53:52.644111 syngen-0.0.96/src/syngen/ml/convertor/
+-rw-r--r--   0 runner    (1001) docker     (122)      163 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/ml/convertor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2872 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/ml/convertor/convertor.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 15:53:52.644111 syngen-0.0.96/src/syngen/ml/data_loaders/
+-rw-r--r--   0 runner    (1001) docker     (122)      172 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/ml/data_loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7274 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/ml/data_loaders/data_loaders.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 15:53:52.644111 syngen-0.0.96/src/syngen/ml/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)      751 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/ml/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 15:53:52.648111 syngen-0.0.96/src/syngen/ml/metrics/accuracy_test/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/ml/metrics/accuracy_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)   723100 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/ml/metrics/accuracy_test/accuracy_report.html
+-rw-r--r--   0 runner    (1001) docker     (122)     5496 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/ml/metrics/accuracy_test/accuracy_test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 15:53:52.636110 syngen-0.0.96/src/syngen/ml/metrics/accuracy_test/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 15:53:52.648111 syngen-0.0.96/src/syngen/ml/metrics/accuracy_test/src/fonts/
+-rw-r--r--   0 runner    (1001) docker     (122)   528976 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 15:53:52.648111 syngen-0.0.96/src/syngen/ml/metrics/metrics_classes/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/ml/metrics/metrics_classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    43412 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/ml/metrics/metrics_classes/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 15:53:52.652111 syngen-0.0.96/src/syngen/ml/metrics/sample_test/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/ml/metrics/sample_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)   708975 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/ml/metrics/sample_test/sample_report_template.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1958 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/ml/metrics/sample_test/sample_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1250 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/ml/metrics/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 15:53:52.652111 syngen-0.0.96/src/syngen/ml/reporters/
+-rw-r--r--   0 runner    (1001) docker     (122)      224 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/ml/reporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6388 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/ml/reporters/reporters.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 15:53:52.652111 syngen-0.0.96/src/syngen/ml/strategies/
+-rw-r--r--   0 runner    (1001) docker     (122)      169 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/ml/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6945 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/ml/strategies/strategies.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 15:53:52.652111 syngen-0.0.96/src/syngen/ml/train_chain/
+-rw-r--r--   0 runner    (1001) docker     (122)      303 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/ml/train_chain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14687 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/ml/train_chain/train_chain.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 15:53:52.652111 syngen-0.0.96/src/syngen/ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/ml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5323 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/ml/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 15:53:52.652111 syngen-0.0.96/src/syngen/ml/vae/
+-rw-r--r--   0 runner    (1001) docker     (122)      173 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/ml/vae/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 15:53:52.656111 syngen-0.0.96/src/syngen/ml/vae/models/
+-rw-r--r--   0 runner    (1001) docker     (122)       49 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/ml/vae/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2085 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/ml/vae/models/custom_layers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30208 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/ml/vae/models/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24693 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/ml/vae/models/features.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10439 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/ml/vae/models/model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 15:53:52.656111 syngen-0.0.96/src/syngen/ml/vae/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/ml/vae/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11045 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/ml/vae/wrappers/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 15:53:52.656111 syngen-0.0.96/src/syngen/ml/validation_schema/
+-rw-r--r--   0 runner    (1001) docker     (122)      153 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/ml/validation_schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1795 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/ml/validation_schema/validation_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 15:53:52.656111 syngen-0.0.96/src/syngen/ml/worker/
+-rw-r--r--   0 runner    (1001) docker     (122)       43 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/ml/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13012 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/ml/worker/worker.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3976 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/train.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 15:53:52.644111 syngen-0.0.96/src/syngen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    14888 2023-04-25 15:53:52.000000 syngen-0.0.96/src/syngen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1902 2023-04-25 15:53:52.000000 syngen-0.0.96/src/syngen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-25 15:53:52.000000 syngen-0.0.96/src/syngen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       86 2023-04-25 15:53:52.000000 syngen-0.0.96/src/syngen.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      299 2023-04-25 15:53:52.000000 syngen-0.0.96/src/syngen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-04-25 15:53:52.000000 syngen-0.0.96/src/syngen.egg-info/top_level.txt
```

### Comparing `syngen-0.0.95/LICENSE` & `syngen-0.0.96/LICENSE`

 * *Files identical despite different names*

### Comparing `syngen-0.0.95/PKG-INFO` & `syngen-0.0.96/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syngen
-Version: 0.0.95
+Version: 0.0.96
 Summary: The tool uncovers patterns, trends, and correlations hidden within your production datasets.
 Home-page: https://github.com/tdspora/syngen
 Author: EPAM Systems, Inc.
 Maintainer: Pavel Bobyrev
 License: GPLv3 License
 Keywords: data,generation,synthetic,vae,tabular
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: syngen Version: 0.0.95 Summary: The tool uncovers
+Metadata-Version: 2.1 Name: syngen Version: 0.0.96 Summary: The tool uncovers
 patterns, trends, and correlations hidden within your production datasets.
 Home-page: https://github.com/tdspora/syngen Author: EPAM Systems, Inc.
 Maintainer: Pavel Bobyrev License: GPLv3 License Keywords:
 data,generation,synthetic,vae,tabular Classifier: Development Status :: 5 -
 Production/Stable Classifier: Operating System :: POSIX :: Linux Classifier:
 Operating System :: Microsoft :: Windows Classifier: License :: OSI Approved ::
 GNU General Public License v3 (GPLv3) Classifier: Programming Language ::
```

### Comparing `syngen-0.0.95/README.md` & `syngen-0.0.96/README.md`

 * *Files identical despite different names*

### Comparing `syngen-0.0.95/setup.cfg` & `syngen-0.0.96/setup.cfg`

 * *Files identical despite different names*

### Comparing `syngen-0.0.95/src/syngen/infer.py` & `syngen-0.0.96/src/syngen/infer.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.95/src/syngen/ml/config/configurations.py` & `syngen-0.0.96/src/syngen/ml/config/configurations.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,25 +80,24 @@
         return data, dropped_cols
 
     @staticmethod
     def _mark_removed_columns(data: pd.DataFrame, schema: Optional[Dict], dropped_columns: Set) -> Dict:
         """
         Mark removed columns in the schema
         """
-        schema["fields"] = dict()
-        if schema.get("format") == "CSV" and dropped_columns:
+        if schema.get("format") == "CSV":
+            schema["fields"] = dict()
             schema["fields"] = {
                 column: "removed"
                 for column in dropped_columns
             }
         else:
             for column, data_type in schema.get("fields", {}).items():
                 if column not in data.columns:
                     schema["fields"][column] = "removed"
-                continue
         return schema
 
     def _extract_data(self) -> Tuple[pd.DataFrame, Dict]:
         """
         Extract data and schema necessary for training process
         """
         data, schema = self._load_source()
```

### Comparing `syngen-0.0.95/src/syngen/ml/convertor/convertor.py` & `syngen-0.0.96/src/syngen/ml/convertor/convertor.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
 @dataclass
 class CSVConvertor:
     """
     Class for supporting custom schema for csv files
     """
     df: pd.DataFrame()
-    schema = {"format": "CSV"}
+    schema = {"fields": {}, "format": "CSV"}
 
 
 class AvroConvertor(Convertor):
     """
     Class for converting fetched avro schema
     """
     def __init__(self, schema, df):
```

### Comparing `syngen-0.0.95/src/syngen/ml/data_loaders/data_loaders.py` & `syngen-0.0.96/src/syngen/ml/data_loaders/data_loaders.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,16 +122,16 @@
 
     def load_data(self, path: str, **kwargs) -> Tuple[pd.DataFrame, Dict]:
         """
         Load data in Avro format from AWS S3, Azure Storage or locally
 
         :param
         path:
-        str which should be should be in the next format for the connection to AWS S3: "s3://path/to/bucket"
-        str which should be should be in the next format for the connection to Azure Storage: "azure://{container_name}/{blob_name}"
+        str which should be in the next format for the connection to AWS S3: "s3://path/to/bucket"
+        str which should be in the next format for the connection to Azure Storage: "azure://{container_name}/{blob_name}"
         """
         try:
             with open(path, 'rb') as f:
                 df = self._load_df(f)
                 schema, preprocessed_df = self._load_schema(f, df)
                 return preprocessed_df, schema
         except FileNotFoundError as error:
```

### Comparing `syngen-0.0.95/src/syngen/ml/metrics/__init__.py` & `syngen-0.0.96/src/syngen/ml/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.95/src/syngen/ml/metrics/accuracy_test/accuracy_report.html` & `syngen-0.0.96/src/syngen/ml/metrics/accuracy_test/accuracy_report.html`

 * *Files identical despite different names*

### Comparing `syngen-0.0.95/src/syngen/ml/metrics/accuracy_test/accuracy_test.py` & `syngen-0.0.96/src/syngen/ml/metrics/accuracy_test/accuracy_test.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.95/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf` & `syngen-0.0.96/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf`

 * *Files identical despite different names*

### Comparing `syngen-0.0.95/src/syngen/ml/metrics/metrics_classes/metrics.py` & `syngen-0.0.96/src/syngen/ml/metrics/metrics_classes/metrics.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.95/src/syngen/ml/metrics/sample_test/sample_report_template.html` & `syngen-0.0.96/src/syngen/ml/metrics/sample_test/sample_report_template.html`

 * *Files identical despite different names*

### Comparing `syngen-0.0.95/src/syngen/ml/metrics/sample_test/sample_test.py` & `syngen-0.0.96/src/syngen/ml/metrics/sample_test/sample_test.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.95/src/syngen/ml/metrics/utils.py` & `syngen-0.0.96/src/syngen/ml/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.95/src/syngen/ml/reporters/reporters.py` & `syngen-0.0.96/src/syngen/ml/reporters/reporters.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,16 @@
         return original, synthetic
 
     def fetch_data_types(self):
         dataset = fetch_dataset(self.paths["dataset_pickle_path"])
         types = (
             dataset.str_columns, dataset.date_columns,
             dataset.int_columns, dataset.float_columns,
-            dataset.binary_columns, dataset.categ_columns
+            dataset.binary_columns, dataset.categ_columns,
+            dataset.long_text_columns
         )
         return types
 
     def preprocess_data(self):
         """
         Preprocess original and synthetic data.
         Return original data, synthetic data, float columns, integer columns, categorical columns
@@ -54,15 +55,16 @@
         missing_columns = set(original) - set(synthetic)
         for col in missing_columns:
             synthetic[col] = np.nan
         columns_nan_labels = get_nan_labels(original)
         original = nan_labels_to_float(original, columns_nan_labels)
         synthetic = nan_labels_to_float(synthetic, columns_nan_labels)
         types = self.fetch_data_types()
-        str_columns, date_columns, int_columns, float_columns, binary_columns, categ_columns = types
+        str_columns, date_columns, int_columns, float_columns, \
+            binary_columns, categ_columns, long_text_columns = types
         original = original[[
             col for col in original.columns
             if col in set().union(*types)
         ]]
         synthetic = synthetic[[
             col for col in synthetic.columns
             if col in set().union(*types)
@@ -72,24 +74,24 @@
                 map(lambda d: pd.Timestamp(d).value, original[date_col])
             )
             synthetic[date_col] = list(
                 map(lambda d: pd.Timestamp(d).value, synthetic[date_col])
             )
 
         int_columns = date_columns | int_columns
+        text_columns = str_columns | long_text_columns
+        original = text_to_continuous(original, text_columns).drop(text_columns, axis=1)
+        synthetic = text_to_continuous(synthetic, text_columns).drop(text_columns, axis=1)
 
-        original = text_to_continuous(original, str_columns).drop(str_columns, axis=1)
-        synthetic = text_to_continuous(synthetic, str_columns).drop(str_columns, axis=1)
-
-        for col in [i + "_word_count" for i in str_columns]:
+        for col in [i + "_word_count" for i in text_columns]:
             if original[col].nunique() < 50:  # ToDo check if we need this
                 categ_columns = categ_columns | {col}
             else:
                 int_columns = int_columns | {col}
-        int_columns = int_columns | {i + "_char_len" for i in str_columns}
+        int_columns = int_columns | {i + "_char_len" for i in text_columns}
 
         categ_columns = categ_columns | binary_columns
         
         for categ_col in categ_columns:
             original[categ_col] = original[categ_col].astype(str)
             synthetic[categ_col] = synthetic[categ_col].astype(str)
         return original, synthetic, float_columns, int_columns, categ_columns, date_columns
```

### Comparing `syngen-0.0.95/src/syngen/ml/strategies/strategies.py` & `syngen-0.0.96/src/syngen/ml/strategies/strategies.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,15 @@
         long_text_handler = LongTextsHandler(
             metadata=self.metadata,
             table_name=self.config.table_name,
             schema=self.config.schema,
             paths=self.config.paths
         )
 
-        root_handler.set_next(long_text_handler).set_next(vae_handler)
+        root_handler.set_next(vae_handler).set_next(long_text_handler)
 
         self.handler = root_handler
         return self
 
     def add_reporters(self, **kwargs):
         if self.config.print_report:
             sample_reporter = SampleAccuracyReporter(
```

### Comparing `syngen-0.0.95/src/syngen/ml/train_chain/train_chain.py` & `syngen-0.0.96/src/syngen/ml/train_chain/train_chain.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import dill
 from scipy.stats import gaussian_kde
 from collections import OrderedDict
 from tensorflow.keras.preprocessing.text import Tokenizer
 
 from syngen.ml.vae import *
 from syngen.ml.data_loaders import DataLoader
-from syngen.ml.utils import slugify_parameters
+from syngen.ml.utils import slugify_parameters, fetch_dataset
 
 
 class AbstractHandler(ABC):
     @abstractmethod
     def set_next(self, handler):
         pass
 
@@ -86,44 +86,25 @@
     def _save_no_ml_checkpoints(self, features: Dict):
         with open(f'{self.paths["no_ml_state_path"]}kde_params.pkl', "wb") as file:
             dill.dump(features, file)
 
     def handle(self, data: pd.DataFrame, **kwargs):
         self._prepare_dir()
 
-        def len_filter(x):
-            return (x.str.len() > 200).any()
+        dataset = fetch_dataset(self.paths["dataset_pickle_path"])
+        long_text_columns = dataset.long_text_columns
 
-        try:
-            if self.schema.get("format", "") == "CSV":
-                data_subset = data.select_dtypes(include=[pd.StringDtype(), "object"])
-            else:
-                text_columns = [
-                    col for col, data_type in self.schema.get("fields", {}).items()
-                    if data_type in ["string", "binary"]
-                ]
-                data_subset = data[text_columns]
-            data_subset = data_subset.loc[:, data_subset.apply(len_filter)]
-            columns = set(data_subset.columns)
-            if columns:
-                logger.info(
-                    f"Please note that the columns - {columns} contain long texts (> 200 symbols). "
-                    f"Such texts' handling consumes significant resources and results in poor quality content, "
-                    f"therefore this column(-s) will be generated using a simplified statistical approach.")
-        except (FileNotFoundError, pd.errors.EmptyDataError, ValueError):
-            data_subset = pd.DataFrame()
-
-        if len(data_subset.columns) > 0:
+        if len(long_text_columns) > 0:
             features = {}
-            for col in data_subset.columns:
+            for col in long_text_columns:
                 tokenizer = Tokenizer(lower=False, char_level=True)
-                if type(data_subset[col].dropna().values[0]) is bytes:
-                    text_col = data_subset[col].str.decode("utf-8", errors="ignore")
+                if type(data[col].dropna().values[0]) is bytes:
+                    text_col = data[col].str.decode("utf-8", errors="ignore")
                 else:
-                    text_col = data_subset[col]
+                    text_col = data[col]
                 text_col = text_col.fillna("")
                 tokenizer.fit_on_texts(text_col)
 
                 indexes = OrderedDict((k, v) for k, v in tokenizer.word_index.items() if k != ' ')
                 counts = OrderedDict((k, v) for k, v in tokenizer.word_counts.items() if k != ' ')
                 ordered_indexes = OrderedDict((k, indexes[k]) for k in counts.keys())
                 text_structure = np.array([text_col.str.len(),
@@ -178,34 +159,30 @@
             process="train"
         )
         self.model.batch_size = min(self.batch_size, len(data))
 
         logger.debug(
             f"Train model with parameters: epochs={self.epochs}, row_subset={self.row_subset}, "
             f"drop_null={self.drop_null}, batch_size={self.batch_size}")
+
+        self.model.prepare_dataset()
+
+        features = fetch_dataset(self.paths["dataset_pickle_path"]).features
+        if len(features) == 0:
+            logger.info("No features to train VAE on")
+            return
         self.model.fit_on_df(
             data,
             epochs=self.epochs,
         )
 
         self.model.save_state(self.paths["state_path"])
         logger.info("Finished VAE training")
 
     def handle(self, data: pd.DataFrame, **kwargs):
-        try:
-            with open(f'{self.paths["no_ml_state_path"]}kde_params.pkl', "rb") as file:
-                features = dill.load(file)
-            if len(set(features.keys()) ^ set(data.columns)) == 0:
-                logger.info("No columns to train with VAE")
-                return super().handle(data, **kwargs)
-            else:
-                data = data.drop(list(features.keys()), axis=1)
-        except Exception:
-            logger.info("There are no long texts columns")
-
         self.__fit_model(data)
         return super().handle(data, **kwargs)
 
 
 @dataclass
 class VaeInferHandler(BaseHandler):
     metadata_path: str
@@ -221,15 +198,15 @@
     has_no_ml: bool = field(init=False)
 
     def __post_init__(self):
         if self.random_seed:
             seed(self.random_seed)
         self.random_seeds_list = list()
         self.vae = None
-        self.has_vae = os.path.exists(self.paths["state_path"])
+        self.has_vae = len(fetch_dataset(self.paths["dataset_pickle_path"]).features) > 0
         self.has_no_ml = os.path.exists(f'{self.paths["path_to_no_ml"]}')
 
     @staticmethod
     def synth_word(size, indexes, counts):
         return ("".join(np.random.choice(np.array(list(indexes)),
                                          size=size,
                                          p=np.array(list(counts.values())) / sum(np.array(list(counts.values()))))))
```

### Comparing `syngen-0.0.95/src/syngen/ml/utils/utils.py` & `syngen-0.0.96/src/syngen/ml/utils/utils.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.95/src/syngen/ml/vae/models/custom_layers.py` & `syngen-0.0.96/src/syngen/ml/vae/models/custom_layers.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.95/src/syngen/ml/vae/models/dataset.py` & `syngen-0.0.96/src/syngen/ml/vae/models/dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -106,15 +106,17 @@
         """
         Set up list of data types of primary and unique keys
         """
         self.pk_uq_keys_types = {}
         for key_name, config in pk_uq_keys_mapping.items():
             key_columns = config.get("columns")
             for column in key_columns:
-                column_type = str if column in (self.str_columns | self.categ_columns | self.date_columns) else float
+                column_type = \
+                    str if column in (self.str_columns | self.categ_columns | self.date_columns | self.long_text_columns) \
+                    else float
                 self.pk_uq_keys_types[column] = column_type
 
     def __map_text_pk(self):
         for pk, pk_type in self.pk_uq_keys_types.items():
             if pk_type is str:
                 mapper = {k: n for n, k in enumerate(self.df[pk])}
                 with open(f"{self.fk_kde_path}{pk}_mapper.pkl", "wb") as file:
@@ -269,80 +271,114 @@
         """
         Set up the list of categorical columns
         """
         self._fetch_categorical_columns()
         self._define_categorical_columns(df)
         self._check_if_column_categorical(schema=schema)
 
+    def _set_long_text_columns(self, df: pd.DataFrame):
+        """
+        Set up the list of columns with long texts (> 200 symbols)
+        """
+        if self.schema.get("format", "") == "CSV":
+            data_subset = df.select_dtypes(include=[pd.StringDtype(), "object"])
+        else:
+            text_columns = [
+                col for col, data_type in self.schema.get("fields", {}).items()
+                if data_type == "string"
+            ]
+            data_subset = df[text_columns]
+        self.long_text_columns = set()
+        if not data_subset.empty:
+            data_subset = data_subset.loc[:, data_subset.apply(lambda x: (x.str.len() > 200).any())]
+            self.long_text_columns = set(data_subset.columns)
+            if self.long_text_columns:
+                logger.info(
+                    f"Please note that the columns - {self.long_text_columns} contain long texts (> 200 symbols). "
+                    f"Such texts' handling consumes significant resources and results in poor quality content, "
+                    f"therefore this column(-s) will be generated using a simplified statistical approach")
+
     def _general_data_pipeline(self, df: pd.DataFrame, schema: Dict, check_object_on_float: bool = False):
         """
         Divide columns in dataframe into groups - binary, categorical, integer, float, string, date
         in case metadata of the table is absent
         """
         if check_object_on_float:
             columns_nan_labels = get_nan_labels(df)
             df = nan_labels_to_float(df, columns_nan_labels)
 
         self._set_binary_columns(df)
         self._set_categorical_columns(df, schema)
+        self._set_long_text_columns(df)
         tmp_df = get_tmp_df(df)
         self.float_columns = set(tmp_df.select_dtypes(include=["float", "float64"]).columns)
         self.int_columns = set(tmp_df.select_dtypes(include=["int", "int64"]).columns)
 
         float_to_int_cols = set()
         for col in self.float_columns:
             if all(x.is_integer() for x in tmp_df[col]):
                 float_to_int_cols.add(col)
 
         self.int_columns = (self.int_columns | float_to_int_cols) - (self.categ_columns | self.binary_columns)
         self.float_columns = self.float_columns - self.categ_columns - self.int_columns - self.binary_columns
         self.str_columns = \
-            set(tmp_df.columns) - self.float_columns - self.categ_columns - self.int_columns - self.binary_columns
-        self.date_columns = get_date_columns(tmp_df, list(self.str_columns))
+            set(tmp_df.columns) - self.float_columns - self.categ_columns - \
+            self.int_columns - self.binary_columns - self.long_text_columns
+        self.categ_columns -= self.long_text_columns
+        self.date_columns = \
+            get_date_columns(df, list(self.str_columns)) - self.categ_columns - \
+            self.binary_columns - self.long_text_columns
         self.str_columns -= self.date_columns
 
     def _avro_data_pipeline(self, df, schema):
         """
         Divide columns in dataframe into groups - binary, categorical, integer, float, string, date
         in case metadata of the table in Avro format is present
         """
         logger.info(f"The schema of table - {self.table_name} was received")
         self._set_binary_columns(df)
         self._set_categorical_columns(df, schema)
+        self._set_long_text_columns(df)
         self.int_columns = set(column for column, data_type in schema.items() if data_type == 'int')
         self.int_columns = self.int_columns - self.categ_columns - self.binary_columns
         self.float_columns = set(column for column, data_type in schema.items() if data_type == 'float')
         self.float_columns = self.float_columns - self.categ_columns - self.binary_columns
         self.str_columns = set(column for column, data_type in schema.items() if data_type == 'string')
-        self.str_columns = self.str_columns - self.categ_columns - self.int_columns - self.binary_columns
-        self.date_columns = get_date_columns(df, list(self.str_columns)) - self.categ_columns - self.binary_columns
+        self.categ_columns -= self.long_text_columns
+        self.str_columns = \
+            self.str_columns - self.categ_columns - self.int_columns - self.binary_columns - self.long_text_columns
+        self.date_columns = \
+            get_date_columns(df, list(self.str_columns)) - self.categ_columns - \
+            self.binary_columns - self.long_text_columns
         self.str_columns -= self.date_columns
 
     def __data_pipeline(self, df: pd.DataFrame, schema: Optional[Dict]):
         if schema.get("format") == "CSV":
             self._general_data_pipeline(df, schema)
         elif schema.get("format") == 'Avro':
             schema = self._update_schema(schema, df)
             self._avro_data_pipeline(df, schema.get("fields"))
 
         assert len(self.str_columns) + \
                len(self.float_columns) + \
                len(self.int_columns) + \
                len(self.date_columns) + \
                len(self.categ_columns) + \
-               len(self.binary_columns) == len(df.columns), "According to number of columns with defined types, " \
-                                                            "column types are not identified correctly."
+               len(self.binary_columns) + \
+               len(self.long_text_columns) == len(df.columns), "According to number of columns with defined types, " \
+                                                               "column types are not identified correctly"
 
         logger.debug(
             f"Count of string columns: {len(self.str_columns)}; "
             + f"Count of float columns: {len(self.float_columns)}; "
             + f"Count of int columns: {len(self.int_columns)}; "
             + f"Count of categorical columns: {len(self.categ_columns)}; "
             + f"Count of date columns: {len(self.date_columns)}; "
             + f"Count of binary columns: {len(self.binary_columns)}"
+            + f"Count of long text columns: {len(self.long_text_columns)}"
         )
 
     def assign_feature(self, feature, columns):
         name = feature.original_name
 
         if name in self.features:
             raise Exception(f"{name} is already contained in features")
```

### Comparing `syngen-0.0.95/src/syngen/ml/vae/models/features.py` & `syngen-0.0.96/src/syngen/ml/vae/models/features.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.95/src/syngen/ml/vae/models/model.py` & `syngen-0.0.96/src/syngen/ml/vae/models/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -235,15 +235,15 @@
             log_likelihoods = self.latent_model.score_samples(latent_sample)
             sliced_latent_sample.append(pop_npoints(latent_sample, log_likelihoods))
 
         synthetic_prediction = self.generator_model.predict(sliced_latent_sample)
         return self.dataset.inverse_transform(synthetic_prediction)
 
     def __check_pk_numeric_convertability(self, column, key_type):
-        if key_type is str:
+        if key_type is str and column not in self.dataset.long_text_columns:
             return self.inverse_transformed_df[column].dropna().str.isnumeric().all()
         else:
             return False
 
     def __make_pk_uq_unique(self, pk_uq_keys_mapping):
         for key_name, config in pk_uq_keys_mapping.items():
             key_columns = config.get("columns")
```

### Comparing `syngen-0.0.95/src/syngen/ml/vae/wrappers/wrappers.py` & `syngen-0.0.96/src/syngen/ml/vae/wrappers/wrappers.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,15 +108,15 @@
         self.latent_components = latent_components
         self.metadata = metadata
         self.table_name = table_name
         self.vae_resources_path = paths["state_path"]
         self.dataset_pickle_path = paths["dataset_pickle_path"]
         self.fk_kde_path = paths["fk_kde_path"]
 
-    def __post__init(self):
+    def __post__init__(self):
         if self.process == "train":
             self.dataset = Dataset(
                 df=self.df,
                 schema=self.schema,
                 metadata=self.metadata,
                 table_name=self.table_name,
                 fk_kde_path=self.fk_kde_path
@@ -172,22 +172,24 @@
             df[column_name] = df[column_name].fillna(np.nan) if nan_label is None else df[column_name].fillna(nan_label)
         return df
 
     @abstractmethod
     def _init_model(self):
         pass
 
+    def prepare_dataset(self):
+        self.__post__init__()
+        self._pipeline()
+
     def fit_on_df(
         self,
         df: pd.DataFrame,
         epochs: int,
         columns_subset: List[str] = None,  # TODO columns_subset does not work
     ):
-        self.__post__init()
-        self._pipeline()
         self._init_model()
 
         if columns_subset is None:
             columns_subset = self.df.columns
         else:
             # if a column is in columns_subset, its null column should also be added if present
             columns_subset += [
```

### Comparing `syngen-0.0.95/src/syngen/ml/validation_schema/validation_schema.py` & `syngen-0.0.96/src/syngen/ml/validation_schema/validation_schema.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.95/src/syngen/ml/worker/worker.py` & `syngen-0.0.96/src/syngen/ml/worker/worker.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.95/src/syngen/train.py` & `syngen-0.0.96/src/syngen/train.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.95/src/syngen.egg-info/PKG-INFO` & `syngen-0.0.96/src/syngen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syngen
-Version: 0.0.95
+Version: 0.0.96
 Summary: The tool uncovers patterns, trends, and correlations hidden within your production datasets.
 Home-page: https://github.com/tdspora/syngen
 Author: EPAM Systems, Inc.
 Maintainer: Pavel Bobyrev
 License: GPLv3 License
 Keywords: data,generation,synthetic,vae,tabular
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: syngen Version: 0.0.95 Summary: The tool uncovers
+Metadata-Version: 2.1 Name: syngen Version: 0.0.96 Summary: The tool uncovers
 patterns, trends, and correlations hidden within your production datasets.
 Home-page: https://github.com/tdspora/syngen Author: EPAM Systems, Inc.
 Maintainer: Pavel Bobyrev License: GPLv3 License Keywords:
 data,generation,synthetic,vae,tabular Classifier: Development Status :: 5 -
 Production/Stable Classifier: Operating System :: POSIX :: Linux Classifier:
 Operating System :: Microsoft :: Windows Classifier: License :: OSI Approved ::
 GNU General Public License v3 (GPLv3) Classifier: Programming Language ::
```

### Comparing `syngen-0.0.95/src/syngen.egg-info/SOURCES.txt` & `syngen-0.0.96/src/syngen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

