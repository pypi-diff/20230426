# Comparing `tmp/veritastool-2.0.1.tar.gz` & `tmp/veritastool-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "veritastool-2.0.1.tar", last modified: Tue Apr  4 06:44:44 2023, max compression
+gzip compressed data, was "veritastool-2.0.2.tar", last modified: Wed Apr 26 08:42:23 2023, max compression
```

## Comparing `veritastool-2.0.1.tar` & `veritastool-2.0.2.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 06:44:44.414006 veritastool-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-04 06:44:32.000000 veritastool-2.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10080 2023-04-04 06:44:44.414006 veritastool-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9787 2023-04-04 06:44:32.000000 veritastool-2.0.1/README.MD
--rw-r--r--   0 runner    (1001) docker     (123)    11361 2023-04-04 06:44:32.000000 veritastool-2.0.1/license.txt
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-04 06:44:32.000000 veritastool-2.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-04 06:44:44.418006 veritastool-2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-04 06:44:32.000000 veritastool-2.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 06:44:44.410006 veritastool-2.0.1/veritastool/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 06:44:44.410006 veritastool-2.0.1/veritastool/config/
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-04 06:44:32.000000 veritastool-2.0.1/veritastool/config/config.ini
--rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-04-04 06:44:32.000000 veritastool-2.0.1/veritastool/config/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 06:44:44.410006 veritastool-2.0.1/veritastool/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-04 06:44:32.000000 veritastool-2.0.1/veritastool/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   109465 2023-04-04 06:44:32.000000 veritastool-2.0.1/veritastool/metrics/fairness_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    11006 2023-04-04 06:44:32.000000 veritastool-2.0.1/veritastool/metrics/modelrates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-04-04 06:44:32.000000 veritastool-2.0.1/veritastool/metrics/newmetric.py
--rw-r--r--   0 runner    (1001) docker     (123)    57171 2023-04-04 06:44:32.000000 veritastool-2.0.1/veritastool/metrics/performance_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    29541 2023-04-04 06:44:32.000000 veritastool-2.0.1/veritastool/metrics/tradeoff.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 06:44:44.414006 veritastool-2.0.1/veritastool/model/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-04 06:44:32.000000 veritastool-2.0.1/veritastool/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36726 2023-04-04 06:44:32.000000 veritastool-2.0.1/veritastool/model/model_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     8960 2023-04-04 06:44:32.000000 veritastool-2.0.1/veritastool/model/modelwrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 06:44:44.414006 veritastool-2.0.1/veritastool/principles/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-04 06:44:32.000000 veritastool-2.0.1/veritastool/principles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   192297 2023-04-04 06:44:32.000000 veritastool-2.0.1/veritastool/principles/fairness.py
--rw-r--r--   0 runner    (1001) docker     (123)    62136 2023-04-04 06:44:32.000000 veritastool-2.0.1/veritastool/principles/transparency.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 06:44:44.410006 veritastool-2.0.1/veritastool/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 06:44:44.414006 veritastool-2.0.1/veritastool/resources/data/
--rw-r--r--   0 runner    (1001) docker     (123)   202555 2023-04-04 06:44:32.000000 veritastool-2.0.1/veritastool/resources/data/credit_score_dict.pickle
--rw-r--r--   0 runner    (1001) docker     (123)     8530 2023-04-04 06:44:32.000000 veritastool-2.0.1/veritastool/resources/data/credit_score_sample.pickle
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 06:44:44.414006 veritastool-2.0.1/veritastool/resources/widget/
--rw-r--r--   0 runner    (1001) docker     (123)    61782 2023-04-04 06:44:32.000000 veritastool-2.0.1/veritastool/resources/widget/fair_class_jpg.JPG
--rw-r--r--   0 runner    (1001) docker     (123)    25865 2023-04-04 06:44:32.000000 veritastool-2.0.1/veritastool/resources/widget/fair_regression_jpg.JPG
--rw-r--r--   0 runner    (1001) docker     (123)    23058 2023-04-04 06:44:32.000000 veritastool-2.0.1/veritastool/resources/widget/fair_uplift_jpg.JPG
--rw-r--r--   0 runner    (1001) docker     (123)    92350 2023-04-04 06:44:32.000000 veritastool-2.0.1/veritastool/resources/widget/perf_class_jpg.JPG
--rw-r--r--   0 runner    (1001) docker     (123)    32848 2023-04-04 06:44:32.000000 veritastool-2.0.1/veritastool/resources/widget/perf_regression_jpg.JPG
--rw-r--r--   0 runner    (1001) docker     (123)    62376 2023-04-04 06:44:33.000000 veritastool-2.0.1/veritastool/resources/widget/perf_uplift_jpg.JPG
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 06:44:44.414006 veritastool-2.0.1/veritastool/usecases/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-04 06:44:33.000000 veritastool-2.0.1/veritastool/usecases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10178 2023-04-04 06:44:33.000000 veritastool-2.0.1/veritastool/usecases/base_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)    15168 2023-04-04 06:44:33.000000 veritastool-2.0.1/veritastool/usecases/base_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)    24577 2023-04-04 06:44:33.000000 veritastool-2.0.1/veritastool/usecases/credit_scoring.py
--rw-r--r--   0 runner    (1001) docker     (123)    24079 2023-04-04 06:44:33.000000 veritastool-2.0.1/veritastool/usecases/customer_marketing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8877 2023-04-04 06:44:33.000000 veritastool-2.0.1/veritastool/usecases/predictive_underwriting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 06:44:44.414006 veritastool-2.0.1/veritastool/util/
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-04-04 06:44:33.000000 veritastool-2.0.1/veritastool/util/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    23494 2023-04-04 06:44:33.000000 veritastool-2.0.1/veritastool/util/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 06:44:44.410006 veritastool-2.0.1/veritastool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10080 2023-04-04 06:44:44.000000 veritastool-2.0.1/veritastool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-04-04 06:44:44.000000 veritastool-2.0.1/veritastool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 06:44:44.000000 veritastool-2.0.1/veritastool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 06:44:44.000000 veritastool-2.0.1/veritastool.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-04 06:44:44.000000 veritastool-2.0.1/veritastool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-04 06:44:44.000000 veritastool-2.0.1/veritastool.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:42:23.292351 veritastool-2.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-26 08:42:03.000000 veritastool-2.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10080 2023-04-26 08:42:23.292351 veritastool-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9787 2023-04-26 08:42:03.000000 veritastool-2.0.2/README.MD
+-rw-r--r--   0 runner    (1001) docker     (123)    11361 2023-04-26 08:42:03.000000 veritastool-2.0.2/license.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-26 08:42:03.000000 veritastool-2.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-26 08:42:23.292351 veritastool-2.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-26 08:42:03.000000 veritastool-2.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:42:23.284350 veritastool-2.0.2/veritastool/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:42:23.288350 veritastool-2.0.2/veritastool/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-26 08:42:03.000000 veritastool-2.0.2/veritastool/config/config.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-04-26 08:42:03.000000 veritastool-2.0.2/veritastool/config/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:42:23.288350 veritastool-2.0.2/veritastool/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-26 08:42:03.000000 veritastool-2.0.2/veritastool/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   110429 2023-04-26 08:42:03.000000 veritastool-2.0.2/veritastool/metrics/fairness_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11006 2023-04-26 08:42:03.000000 veritastool-2.0.2/veritastool/metrics/modelrates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-04-26 08:42:03.000000 veritastool-2.0.2/veritastool/metrics/newmetric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57171 2023-04-26 08:42:03.000000 veritastool-2.0.2/veritastool/metrics/performance_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29541 2023-04-26 08:42:03.000000 veritastool-2.0.2/veritastool/metrics/tradeoff.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:42:23.288350 veritastool-2.0.2/veritastool/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-26 08:42:03.000000 veritastool-2.0.2/veritastool/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36726 2023-04-26 08:42:03.000000 veritastool-2.0.2/veritastool/model/model_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8960 2023-04-26 08:42:03.000000 veritastool-2.0.2/veritastool/model/modelwrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:42:23.288350 veritastool-2.0.2/veritastool/principles/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-26 08:42:03.000000 veritastool-2.0.2/veritastool/principles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   192297 2023-04-26 08:42:03.000000 veritastool-2.0.2/veritastool/principles/fairness.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62136 2023-04-26 08:42:03.000000 veritastool-2.0.2/veritastool/principles/transparency.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:42:23.284350 veritastool-2.0.2/veritastool/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:42:23.292351 veritastool-2.0.2/veritastool/resources/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   202555 2023-04-26 08:42:03.000000 veritastool-2.0.2/veritastool/resources/data/credit_score_dict.pickle
+-rw-r--r--   0 runner    (1001) docker     (123)     8530 2023-04-26 08:42:03.000000 veritastool-2.0.2/veritastool/resources/data/credit_score_sample.pickle
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:42:23.292351 veritastool-2.0.2/veritastool/resources/widget/
+-rw-r--r--   0 runner    (1001) docker     (123)    61782 2023-04-26 08:42:03.000000 veritastool-2.0.2/veritastool/resources/widget/fair_class_jpg.JPG
+-rw-r--r--   0 runner    (1001) docker     (123)    25865 2023-04-26 08:42:03.000000 veritastool-2.0.2/veritastool/resources/widget/fair_regression_jpg.JPG
+-rw-r--r--   0 runner    (1001) docker     (123)    23058 2023-04-26 08:42:03.000000 veritastool-2.0.2/veritastool/resources/widget/fair_uplift_jpg.JPG
+-rw-r--r--   0 runner    (1001) docker     (123)    92350 2023-04-26 08:42:03.000000 veritastool-2.0.2/veritastool/resources/widget/perf_class_jpg.JPG
+-rw-r--r--   0 runner    (1001) docker     (123)    32848 2023-04-26 08:42:03.000000 veritastool-2.0.2/veritastool/resources/widget/perf_regression_jpg.JPG
+-rw-r--r--   0 runner    (1001) docker     (123)    62376 2023-04-26 08:42:03.000000 veritastool-2.0.2/veritastool/resources/widget/perf_uplift_jpg.JPG
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:42:23.292351 veritastool-2.0.2/veritastool/usecases/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-26 08:42:03.000000 veritastool-2.0.2/veritastool/usecases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10178 2023-04-26 08:42:03.000000 veritastool-2.0.2/veritastool/usecases/base_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15168 2023-04-26 08:42:03.000000 veritastool-2.0.2/veritastool/usecases/base_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24577 2023-04-26 08:42:03.000000 veritastool-2.0.2/veritastool/usecases/credit_scoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24079 2023-04-26 08:42:03.000000 veritastool-2.0.2/veritastool/usecases/customer_marketing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8877 2023-04-26 08:42:03.000000 veritastool-2.0.2/veritastool/usecases/predictive_underwriting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:42:23.292351 veritastool-2.0.2/veritastool/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-04-26 08:42:03.000000 veritastool-2.0.2/veritastool/util/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23494 2023-04-26 08:42:03.000000 veritastool-2.0.2/veritastool/util/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:42:23.288350 veritastool-2.0.2/veritastool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10080 2023-04-26 08:42:23.000000 veritastool-2.0.2/veritastool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-04-26 08:42:23.000000 veritastool-2.0.2/veritastool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 08:42:23.000000 veritastool-2.0.2/veritastool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 08:42:23.000000 veritastool-2.0.2/veritastool.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-26 08:42:23.000000 veritastool-2.0.2/veritastool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-26 08:42:23.000000 veritastool-2.0.2/veritastool.egg-info/top_level.txt
```

### Comparing `veritastool-2.0.1/PKG-INFO` & `veritastool-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: veritastool
-Version: 2.0.1
+Version: 2.0.2
 Summary: Veritas Diagnosis tool for fairness & transparency assessment.
 Author: MAS Veritas
 License: Apache 2.0
 Project-URL: Documentation, https://htmlpreview.github.io/?https://github.com/mas-veritas2/veritastool/blob/main/veritastool/resources/specs/API_Specs_final.html
 Project-URL: Source Code, https://github.com/veritas-project/diagnosis-tool
 Requires-Python: >=3.8.0,<=3.10.10
 Description-Content-Type: text/markdown
```

### Comparing `veritastool-2.0.1/README.MD` & `veritastool-2.0.2/README.MD`

 * *Files identical despite different names*

### Comparing `veritastool-2.0.1/license.txt` & `veritastool-2.0.2/license.txt`

 * *Files identical despite different names*

### Comparing `veritastool-2.0.1/setup.cfg` & `veritastool-2.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `veritastool-2.0.1/setup.py` & `veritastool-2.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,12 +8,12 @@
 with io.open(op.join(here, "requirements.txt"), encoding="utf-8") as f:
     all_reqs = f.read().split("\n")
     if platform.system() == "Windows":
         all_reqs.append("pywin32")
 
 install_requires = [x.strip() for x in all_reqs]
 
-setup(name='veritastool',version='2.0.1',description ='Veritas Diagnosis tool for fairness & transparency assessment.',author='MAS Veritas',
+setup(name='veritastool',version='2.0.2',description ='Veritas Diagnosis tool for fairness & transparency assessment.',author='MAS Veritas',
 install_requires=install_requires,python_requires='>=3.8.0,<=3.10.10',
 packages=['veritastool.model','veritastool.principles','veritastool.metrics','veritastool.config','veritastool.util','veritastool.resources','veritastool.usecases'],
 include_package_data=True,
 zip_safe=False)
```

### Comparing `veritastool-2.0.1/veritastool/config/config.ini` & `veritastool-2.0.2/veritastool/config/config.ini`

 * *Files identical despite different names*

### Comparing `veritastool-2.0.1/veritastool/config/constants.py` & `veritastool-2.0.2/veritastool/config/constants.py`

 * *Files identical despite different names*

### Comparing `veritastool-2.0.1/veritastool/metrics/fairness_metrics.py` & `veritastool-2.0.2/veritastool/metrics/fairness_metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -444,15 +444,15 @@
                     metric_obj.tp_ps += tp_ps
                     metric_obj.fp_ps += fp_ps
                     metric_obj.tn_ps += tn_ps
                     metric_obj.fn_ps += fn_ps
                     metric_obj.tp_us += tp_us
                     metric_obj.fp_us += fp_us
                     metric_obj.tn_us += tn_us
-                    metric_obj.tp_us += tp_us
+                    metric_obj.fn_us += fn_us
 
             else:
                 
                 metric_obj.tp_ps, metric_obj.fp_ps, metric_obj.tn_ps, metric_obj.fn_ps, metric_obj.tp_us, metric_obj.fp_us, metric_obj.tn_us, metric_obj.fn_us = \
                     metric_obj.use_case_object._get_confusion_matrix_optimized(
                             metric_obj.y_trues,
                             metric_obj.y_preds, 
@@ -1157,16 +1157,16 @@
         y_pred = self.y_pred[0]
         if 'y_pred_new' in kwargs:
             y_pred=kwargs['y_pred_new'][0]
         y_true = y_true[maskFilter]
         y_pred = y_pred[maskFilter]
         
         if self.sample_weight[0] is not None: 
-            sample_weight_p = np.array(self.sample_weight[0])[mask]
-            sample_weight_u = np.array(self.sample_weight[0])[~mask]
+            sample_weight_p = np.array(self.sample_weight[0][maskFilter])[mask]
+            sample_weight_u = np.array(self.sample_weight[0][maskFilter])[~mask]
         else:
             sample_weight_p = None
             sample_weight_u = None
         
         rmse_p = mean_squared_error(y_true=np.array(y_true)[mask], y_pred=np.array(y_pred)[mask], sample_weight=sample_weight_p) ** 0.5
         rmse_u = mean_squared_error(y_true=np.array(y_true)[~mask], y_pred=np.array(y_pred)[~mask], sample_weight=sample_weight_u) ** 0.5
         return (rmse_p - rmse_u, rmse_p)
@@ -1192,16 +1192,16 @@
         y_pred = self.y_pred[0]
         if 'y_pred_new' in kwargs:
             y_pred=kwargs['y_pred_new'][0]
         y_true = y_true[maskFilter]
         y_pred = y_pred[maskFilter]
         
         if self.sample_weight[0] is not None: 
-            sample_weight_p = np.array(self.sample_weight[0])[mask]
-            sample_weight_u = np.array(self.sample_weight[0])[~mask]
+            sample_weight_p = np.array(self.sample_weight[0][maskFilter])[mask]
+            sample_weight_u = np.array(self.sample_weight[0][maskFilter])[~mask]
         else:
             sample_weight_p = None
             sample_weight_u = None
         
         rmse_p = mean_squared_error(y_true=np.array(y_true)[mask], y_pred=np.array(y_pred)[mask], sample_weight=sample_weight_p) ** 0.5
         rmse_u = mean_squared_error(y_true=np.array(y_true)[~mask], y_pred=np.array(y_pred)[~mask], sample_weight=sample_weight_u) ** 0.5
         return (rmse_p/rmse_u, rmse_p)
@@ -1227,16 +1227,16 @@
         y_pred = self.y_pred[0]
         if 'y_pred_new' in kwargs:
             y_pred=kwargs['y_pred_new'][0]
         y_true = y_true[maskFilter]
         y_pred = y_pred[maskFilter]
             
         if self.sample_weight[0] is not None: 
-            sample_weight_p = np.array(self.sample_weight[0])[mask]
-            sample_weight_u = np.array(self.sample_weight[0])[~mask]
+            sample_weight_p = np.array(self.sample_weight[0][maskFilter])[mask]
+            sample_weight_u = np.array(self.sample_weight[0][maskFilter])[~mask]
         else:
             sample_weight_p = None
             sample_weight_u = None
 
         mape_p = mean_absolute_percentage_error(y_true=np.array(y_true)[mask], y_pred=np.array(y_pred)[mask], sample_weight=sample_weight_p)
         mape_u = mean_absolute_percentage_error(y_true=np.array(y_true)[~mask], y_pred=np.array(y_pred)[~mask], sample_weight=sample_weight_u)
 
@@ -1263,16 +1263,16 @@
         y_pred = self.y_pred[0]
         if 'y_pred_new' in kwargs:
             y_pred=kwargs['y_pred_new'][0]
         y_true = y_true[maskFilter]
         y_pred = y_pred[maskFilter]
             
         if self.sample_weight[0] is not None: 
-            sample_weight_p = np.array(self.sample_weight[0])[mask]
-            sample_weight_u = np.array(self.sample_weight[0])[~mask]
+            sample_weight_p = np.array(self.sample_weight[0][maskFilter])[mask]
+            sample_weight_u = np.array(self.sample_weight[0][maskFilter])[~mask]
         else:
             sample_weight_p = None
             sample_weight_u = None
 
         mape_p = mean_absolute_percentage_error(y_true=np.array(y_true)[mask], y_pred=np.array(y_pred)[mask], sample_weight=sample_weight_p)
         mape_u = mean_absolute_percentage_error(y_true=np.array(y_true)[~mask], y_pred=np.array(y_pred)[~mask], sample_weight=sample_weight_u)
 
@@ -1297,17 +1297,24 @@
         mask= mask[maskFilter].astype(bool)
         y_true = self.y_true[0]
         y_pred = self.y_pred[0]
         if 'y_pred_new' in kwargs:
             y_pred=kwargs['y_pred_new'][0]
         y_true = y_true[maskFilter]
         y_pred = y_pred[maskFilter]
+        
+        if self.sample_weight[0] is not None: 
+            sample_weight_p = np.array(self.sample_weight[0][maskFilter])[mask]
+            sample_weight_u = np.array(self.sample_weight[0][maskFilter])[~mask]
+        else:
+            sample_weight_p = np.ones(y_true.shape)[mask]
+            sample_weight_u = np.ones(y_true.shape)[~mask]
     
-        wape_p = np.sum(np.absolute(np.subtract(y_true[mask], y_pred[mask])))/ np.sum(y_true[mask])
-        wape_u = np.sum(np.absolute(np.subtract(y_true[~mask], y_pred[~mask])))/ np.sum(y_true[~mask])
+        wape_p = np.sum(np.absolute(np.subtract(y_true[mask], y_pred[mask]))*sample_weight_p)/ np.sum(np.absolute(y_true[mask])*sample_weight_p)
+        wape_u = np.sum(np.absolute(np.subtract(y_true[~mask], y_pred[~mask]))*sample_weight_u)/ np.sum(np.absolute(y_true[~mask])*sample_weight_u)
             
         return (wape_p - wape_u, wape_p)
 
     def _compute_wape_ratio(self, **kwargs):
         """
         Computes the ratio of weighted average percentage error between the privileged and unprivileged groups
     
@@ -1326,17 +1333,24 @@
         mask= mask[maskFilter].astype(bool)
         y_true = self.y_true[0]
         y_pred = self.y_pred[0]
         if 'y_pred_new' in kwargs:
             y_pred=kwargs['y_pred_new'][0]
         y_true = y_true[maskFilter]
         y_pred = y_pred[maskFilter]
+
+        if self.sample_weight[0] is not None: 
+            sample_weight_p = np.array(self.sample_weight[0][maskFilter])[mask]
+            sample_weight_u = np.array(self.sample_weight[0][maskFilter])[~mask]
+        else:
+            sample_weight_p = np.ones(y_true.shape)[mask]
+            sample_weight_u = np.ones(y_true.shape)[~mask]
     
-        wape_p = np.sum(np.absolute(np.subtract(y_true[mask], y_pred[mask])))/ np.sum(y_true[mask])
-        wape_u = np.sum(np.absolute(np.subtract(y_true[~mask], y_pred[~mask])))/ np.sum(y_true[~mask])
+        wape_p = np.sum(np.absolute(np.subtract(y_true[mask], y_pred[mask]))*sample_weight_p)/ np.sum(np.absolute(y_true[mask])*sample_weight_p)
+        wape_u = np.sum(np.absolute(np.subtract(y_true[~mask], y_pred[~mask]))*sample_weight_u)/ np.sum(np.absolute(y_true[~mask])*sample_weight_u)
             
         return (wape_p/wape_u, wape_p)
 
     def _compute_log_loss_score(self, y_true, y_prob, mask, multiclass=False):
         """
         Computes log loss score for privileged and unprivileged groups based on multiclass flag.
```

### Comparing `veritastool-2.0.1/veritastool/metrics/modelrates.py` & `veritastool-2.0.2/veritastool/metrics/modelrates.py`

 * *Files identical despite different names*

### Comparing `veritastool-2.0.1/veritastool/metrics/newmetric.py` & `veritastool-2.0.2/veritastool/metrics/newmetric.py`

 * *Files identical despite different names*

### Comparing `veritastool-2.0.1/veritastool/metrics/performance_metrics.py` & `veritastool-2.0.2/veritastool/metrics/performance_metrics.py`

 * *Files identical despite different names*

### Comparing `veritastool-2.0.1/veritastool/metrics/tradeoff.py` & `veritastool-2.0.2/veritastool/metrics/tradeoff.py`

 * *Files identical despite different names*

### Comparing `veritastool-2.0.1/veritastool/model/model_container.py` & `veritastool-2.0.2/veritastool/model/model_container.py`

 * *Files identical despite different names*

### Comparing `veritastool-2.0.1/veritastool/model/modelwrapper.py` & `veritastool-2.0.2/veritastool/model/modelwrapper.py`

 * *Files identical despite different names*

### Comparing `veritastool-2.0.1/veritastool/principles/fairness.py` & `veritastool-2.0.2/veritastool/principles/fairness.py`

 * *Files identical despite different names*

### Comparing `veritastool-2.0.1/veritastool/principles/transparency.py` & `veritastool-2.0.2/veritastool/principles/transparency.py`

 * *Files identical despite different names*

### Comparing `veritastool-2.0.1/veritastool/resources/data/credit_score_dict.pickle` & `veritastool-2.0.2/veritastool/resources/data/credit_score_dict.pickle`

 * *Files identical despite different names*

### Comparing `veritastool-2.0.1/veritastool/resources/data/credit_score_sample.pickle` & `veritastool-2.0.2/veritastool/resources/data/credit_score_sample.pickle`

 * *Files identical despite different names*

### Comparing `veritastool-2.0.1/veritastool/resources/widget/fair_class_jpg.JPG` & `veritastool-2.0.2/veritastool/resources/widget/fair_class_jpg.JPG`

 * *Files identical despite different names*

### Comparing `veritastool-2.0.1/veritastool/resources/widget/fair_regression_jpg.JPG` & `veritastool-2.0.2/veritastool/resources/widget/fair_regression_jpg.JPG`

 * *Files identical despite different names*

### Comparing `veritastool-2.0.1/veritastool/resources/widget/fair_uplift_jpg.JPG` & `veritastool-2.0.2/veritastool/resources/widget/fair_uplift_jpg.JPG`

 * *Files identical despite different names*

### Comparing `veritastool-2.0.1/veritastool/resources/widget/perf_class_jpg.JPG` & `veritastool-2.0.2/veritastool/resources/widget/perf_class_jpg.JPG`

 * *Files identical despite different names*

### Comparing `veritastool-2.0.1/veritastool/resources/widget/perf_regression_jpg.JPG` & `veritastool-2.0.2/veritastool/resources/widget/perf_regression_jpg.JPG`

 * *Files identical despite different names*

### Comparing `veritastool-2.0.1/veritastool/resources/widget/perf_uplift_jpg.JPG` & `veritastool-2.0.2/veritastool/resources/widget/perf_uplift_jpg.JPG`

 * *Files identical despite different names*

### Comparing `veritastool-2.0.1/veritastool/usecases/base_classification.py` & `veritastool-2.0.2/veritastool/usecases/base_classification.py`

 * *Files identical despite different names*

### Comparing `veritastool-2.0.1/veritastool/usecases/base_regression.py` & `veritastool-2.0.2/veritastool/usecases/base_regression.py`

 * *Files identical despite different names*

### Comparing `veritastool-2.0.1/veritastool/usecases/credit_scoring.py` & `veritastool-2.0.2/veritastool/usecases/credit_scoring.py`

 * *Files identical despite different names*

### Comparing `veritastool-2.0.1/veritastool/usecases/customer_marketing.py` & `veritastool-2.0.2/veritastool/usecases/customer_marketing.py`

 * *Files identical despite different names*

### Comparing `veritastool-2.0.1/veritastool/usecases/predictive_underwriting.py` & `veritastool-2.0.2/veritastool/usecases/predictive_underwriting.py`

 * *Files identical despite different names*

### Comparing `veritastool-2.0.1/veritastool/util/errors.py` & `veritastool-2.0.2/veritastool/util/errors.py`

 * *Files identical despite different names*

### Comparing `veritastool-2.0.1/veritastool/util/utility.py` & `veritastool-2.0.2/veritastool/util/utility.py`

 * *Files identical despite different names*

### Comparing `veritastool-2.0.1/veritastool.egg-info/PKG-INFO` & `veritastool-2.0.2/veritastool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: veritastool
-Version: 2.0.1
+Version: 2.0.2
 Summary: Veritas Diagnosis tool for fairness & transparency assessment.
 Author: MAS Veritas
 License: Apache 2.0
 Project-URL: Documentation, https://htmlpreview.github.io/?https://github.com/mas-veritas2/veritastool/blob/main/veritastool/resources/specs/API_Specs_final.html
 Project-URL: Source Code, https://github.com/veritas-project/diagnosis-tool
 Requires-Python: >=3.8.0,<=3.10.10
 Description-Content-Type: text/markdown
```

### Comparing `veritastool-2.0.1/veritastool.egg-info/SOURCES.txt` & `veritastool-2.0.2/veritastool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

