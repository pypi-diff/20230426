# Comparing `tmp/dp-accounting-0.4.0.tar.gz` & `tmp/dp-accounting-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dp-accounting-0.4.0.tar", last modified: Thu Mar 30 18:20:58 2023, max compression
+gzip compressed data, was "dp-accounting-0.4.1.tar", last modified: Wed Apr 26 18:20:44 2023, max compression
```

## Comparing `dp-accounting-0.4.0.tar` & `dp-accounting-0.4.1.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-x---   0 pritishk (568285) primarygroup (89939)        0 2023-03-30 18:20:58.410115 dp-accounting-0.4.0/
--rw-r-----   0 pritishk (568285) primarygroup (89939)     1589 2023-03-30 18:20:58.410115 dp-accounting-0.4.0/PKG-INFO
--rw-r-----   0 pritishk (568285) primarygroup (89939)     1806 2023-03-30 18:20:03.000000 dp-accounting-0.4.0/README.md
-drwxr-x---   0 pritishk (568285) primarygroup (89939)        0 2023-03-30 18:20:58.402114 dp-accounting-0.4.0/dp_accounting/
--rw-r-----   0 pritishk (568285) primarygroup (89939)     1800 2023-03-30 18:20:03.000000 dp-accounting-0.4.0/dp_accounting/__init__.py
--rw-r-----   0 pritishk (568285) primarygroup (89939)     9166 2023-03-30 18:20:03.000000 dp-accounting-0.4.0/dp_accounting/dp_event.py
--rw-r-----   0 pritishk (568285) primarygroup (89939)     2833 2023-03-30 18:20:03.000000 dp-accounting-0.4.0/dp_accounting/dp_event_builder.py
--rw-r-----   0 pritishk (568285) primarygroup (89939)     3054 2023-03-30 18:20:03.000000 dp-accounting-0.4.0/dp_accounting/dp_event_builder_test.py
--rw-r-----   0 pritishk (568285) primarygroup (89939)     8640 2023-03-30 18:20:03.000000 dp-accounting-0.4.0/dp_accounting/mechanism_calibration.py
--rw-r-----   0 pritishk (568285) primarygroup (89939)     8539 2023-03-30 18:20:03.000000 dp-accounting-0.4.0/dp_accounting/mechanism_calibration_test.py
-drwxr-x---   0 pritishk (568285) primarygroup (89939)        0 2023-03-30 18:20:58.406115 dp-accounting-0.4.0/dp_accounting/pld/
--rw-r-----   0 pritishk (568285) primarygroup (89939)      675 2023-03-30 18:20:03.000000 dp-accounting-0.4.0/dp_accounting/pld/__init__.py
--rw-r-----   0 pritishk (568285) primarygroup (89939)    13306 2023-03-30 18:20:03.000000 dp-accounting-0.4.0/dp_accounting/pld/accountant.py
--rw-r-----   0 pritishk (568285) primarygroup (89939)     8424 2023-03-30 18:20:03.000000 dp-accounting-0.4.0/dp_accounting/pld/accountant_test.py
--rw-r-----   0 pritishk (568285) primarygroup (89939)    12372 2023-03-30 18:20:03.000000 dp-accounting-0.4.0/dp_accounting/pld/common.py
--rw-r-----   0 pritishk (568285) primarygroup (89939)     8948 2023-03-30 18:20:03.000000 dp-accounting-0.4.0/dp_accounting/pld/common_test.py
--rw-r-----   0 pritishk (568285) primarygroup (89939)    32711 2023-03-30 18:20:03.000000 dp-accounting-0.4.0/dp_accounting/pld/pld_pmf.py
--rw-r-----   0 pritishk (568285) primarygroup (89939)    28136 2023-03-30 18:20:03.000000 dp-accounting-0.4.0/dp_accounting/pld/pld_pmf_test.py
--rw-r-----   0 pritishk (568285) primarygroup (89939)     5662 2023-03-30 18:20:03.000000 dp-accounting-0.4.0/dp_accounting/pld/pld_privacy_accountant.py
--rw-r-----   0 pritishk (568285) primarygroup (89939)     6085 2023-03-30 18:20:03.000000 dp-accounting-0.4.0/dp_accounting/pld/pld_privacy_accountant_test.py
--rw-r-----   0 pritishk (568285) primarygroup (89939)    63971 2023-03-30 18:20:03.000000 dp-accounting-0.4.0/dp_accounting/pld/privacy_loss_distribution.py
--rw-r-----   0 pritishk (568285) primarygroup (89939)     2548 2023-03-30 18:20:03.000000 dp-accounting-0.4.0/dp_accounting/pld/privacy_loss_distribution_basic_example.py
--rw-r-----   0 pritishk (568285) primarygroup (89939)    52970 2023-03-30 18:20:03.000000 dp-accounting-0.4.0/dp_accounting/pld/privacy_loss_distribution_test.py
--rw-r-----   0 pritishk (568285) primarygroup (89939)    70692 2023-03-30 18:20:03.000000 dp-accounting-0.4.0/dp_accounting/pld/privacy_loss_mechanism.py
--rw-r-----   0 pritishk (568285) primarygroup (89939)    58248 2023-03-30 18:20:03.000000 dp-accounting-0.4.0/dp_accounting/pld/privacy_loss_mechanism_test.py
--rw-r-----   0 pritishk (568285) primarygroup (89939)     3054 2023-03-30 18:20:03.000000 dp-accounting-0.4.0/dp_accounting/pld/test_util.py
--rw-r-----   0 pritishk (568285) primarygroup (89939)     3647 2023-03-30 18:20:03.000000 dp-accounting-0.4.0/dp_accounting/pld/test_util_test.py
--rw-r-----   0 pritishk (568285) primarygroup (89939)     5579 2023-03-30 18:20:03.000000 dp-accounting-0.4.0/dp_accounting/privacy_accountant.py
--rw-r-----   0 pritishk (568285) primarygroup (89939)     4351 2023-03-30 18:20:03.000000 dp-accounting-0.4.0/dp_accounting/privacy_accountant_test.py
-drwxr-x---   0 pritishk (568285) primarygroup (89939)        0 2023-03-30 18:20:58.410115 dp-accounting-0.4.0/dp_accounting/rdp/
--rw-r-----   0 pritishk (568285) primarygroup (89939)      744 2023-03-30 18:20:03.000000 dp-accounting-0.4.0/dp_accounting/rdp/__init__.py
--rw-r-----   0 pritishk (568285) primarygroup (89939)    33535 2023-03-30 18:20:03.000000 dp-accounting-0.4.0/dp_accounting/rdp/rdp_privacy_accountant.py
--rw-r-----   0 pritishk (568285) primarygroup (89939)    28704 2023-03-30 18:20:03.000000 dp-accounting-0.4.0/dp_accounting/rdp/rdp_privacy_accountant_test.py
-drwxr-x---   0 pritishk (568285) primarygroup (89939)        0 2023-03-30 18:20:58.402114 dp-accounting-0.4.0/dp_accounting.egg-info/
--rw-r-----   0 pritishk (568285) primarygroup (89939)     1589 2023-03-30 18:20:58.000000 dp-accounting-0.4.0/dp_accounting.egg-info/PKG-INFO
--rw-r-----   0 pritishk (568285) primarygroup (89939)     1246 2023-03-30 18:20:58.000000 dp-accounting-0.4.0/dp_accounting.egg-info/SOURCES.txt
--rw-r-----   0 pritishk (568285) primarygroup (89939)        1 2023-03-30 18:20:58.000000 dp-accounting-0.4.0/dp_accounting.egg-info/dependency_links.txt
--rw-r-----   0 pritishk (568285) primarygroup (89939)       68 2023-03-30 18:20:58.000000 dp-accounting-0.4.0/dp_accounting.egg-info/requires.txt
--rw-r-----   0 pritishk (568285) primarygroup (89939)       14 2023-03-30 18:20:58.000000 dp-accounting-0.4.0/dp_accounting.egg-info/top_level.txt
--rw-r-----   0 pritishk (568285) primarygroup (89939)       38 2023-03-30 18:20:58.410115 dp-accounting-0.4.0/setup.cfg
--rw-r-----   0 pritishk (568285) primarygroup (89939)     2576 2023-03-30 18:20:03.000000 dp-accounting-0.4.0/setup.py
+drwxr-x---   0 galenandrew (404454) primarygroup (89939)        0 2023-04-26 18:20:44.118154 dp-accounting-0.4.1/
+-rw-r-----   0 galenandrew (404454) primarygroup (89939)     1589 2023-04-26 18:20:44.118154 dp-accounting-0.4.1/PKG-INFO
+-rw-r-----   0 galenandrew (404454) primarygroup (89939)     1806 2023-04-26 18:17:04.000000 dp-accounting-0.4.1/README.md
+drwxr-x---   0 galenandrew (404454) primarygroup (89939)        0 2023-04-26 18:20:44.114154 dp-accounting-0.4.1/dp_accounting/
+-rw-r-----   0 galenandrew (404454) primarygroup (89939)     1800 2023-04-26 18:17:04.000000 dp-accounting-0.4.1/dp_accounting/__init__.py
+-rw-r-----   0 galenandrew (404454) primarygroup (89939)    13802 2023-04-26 18:17:04.000000 dp-accounting-0.4.1/dp_accounting/dp_event.py
+-rw-r-----   0 galenandrew (404454) primarygroup (89939)     2833 2023-04-26 18:17:04.000000 dp-accounting-0.4.1/dp_accounting/dp_event_builder.py
+-rw-r-----   0 galenandrew (404454) primarygroup (89939)     3054 2023-04-26 18:17:04.000000 dp-accounting-0.4.1/dp_accounting/dp_event_builder_test.py
+-rw-r-----   0 galenandrew (404454) primarygroup (89939)     3688 2023-04-26 18:17:04.000000 dp-accounting-0.4.1/dp_accounting/dp_event_test.py
+-rw-r-----   0 galenandrew (404454) primarygroup (89939)     8640 2023-04-26 18:17:04.000000 dp-accounting-0.4.1/dp_accounting/mechanism_calibration.py
+-rw-r-----   0 galenandrew (404454) primarygroup (89939)     8539 2023-04-26 18:17:04.000000 dp-accounting-0.4.1/dp_accounting/mechanism_calibration_test.py
+drwxr-x---   0 galenandrew (404454) primarygroup (89939)        0 2023-04-26 18:20:44.118154 dp-accounting-0.4.1/dp_accounting/pld/
+-rw-r-----   0 galenandrew (404454) primarygroup (89939)      675 2023-04-26 18:17:04.000000 dp-accounting-0.4.1/dp_accounting/pld/__init__.py
+-rw-r-----   0 galenandrew (404454) primarygroup (89939)    13306 2023-04-26 18:17:04.000000 dp-accounting-0.4.1/dp_accounting/pld/accountant.py
+-rw-r-----   0 galenandrew (404454) primarygroup (89939)     8424 2023-04-26 18:17:04.000000 dp-accounting-0.4.1/dp_accounting/pld/accountant_test.py
+-rw-r-----   0 galenandrew (404454) primarygroup (89939)    12372 2023-04-26 18:17:04.000000 dp-accounting-0.4.1/dp_accounting/pld/common.py
+-rw-r-----   0 galenandrew (404454) primarygroup (89939)     8948 2023-04-26 18:17:04.000000 dp-accounting-0.4.1/dp_accounting/pld/common_test.py
+-rw-r-----   0 galenandrew (404454) primarygroup (89939)    32711 2023-04-26 18:17:04.000000 dp-accounting-0.4.1/dp_accounting/pld/pld_pmf.py
+-rw-r-----   0 galenandrew (404454) primarygroup (89939)    28136 2023-04-26 18:17:04.000000 dp-accounting-0.4.1/dp_accounting/pld/pld_pmf_test.py
+-rw-r-----   0 galenandrew (404454) primarygroup (89939)     5662 2023-04-26 18:17:04.000000 dp-accounting-0.4.1/dp_accounting/pld/pld_privacy_accountant.py
+-rw-r-----   0 galenandrew (404454) primarygroup (89939)     6085 2023-04-26 18:17:04.000000 dp-accounting-0.4.1/dp_accounting/pld/pld_privacy_accountant_test.py
+-rw-r-----   0 galenandrew (404454) primarygroup (89939)    63971 2023-04-26 18:17:04.000000 dp-accounting-0.4.1/dp_accounting/pld/privacy_loss_distribution.py
+-rw-r-----   0 galenandrew (404454) primarygroup (89939)     2548 2023-04-26 18:17:04.000000 dp-accounting-0.4.1/dp_accounting/pld/privacy_loss_distribution_basic_example.py
+-rw-r-----   0 galenandrew (404454) primarygroup (89939)    52970 2023-04-26 18:17:04.000000 dp-accounting-0.4.1/dp_accounting/pld/privacy_loss_distribution_test.py
+-rw-r-----   0 galenandrew (404454) primarygroup (89939)    70692 2023-04-26 18:17:04.000000 dp-accounting-0.4.1/dp_accounting/pld/privacy_loss_mechanism.py
+-rw-r-----   0 galenandrew (404454) primarygroup (89939)    58248 2023-04-26 18:17:04.000000 dp-accounting-0.4.1/dp_accounting/pld/privacy_loss_mechanism_test.py
+-rw-r-----   0 galenandrew (404454) primarygroup (89939)     3054 2023-04-26 18:17:04.000000 dp-accounting-0.4.1/dp_accounting/pld/test_util.py
+-rw-r-----   0 galenandrew (404454) primarygroup (89939)     3647 2023-04-26 18:17:04.000000 dp-accounting-0.4.1/dp_accounting/pld/test_util_test.py
+-rw-r-----   0 galenandrew (404454) primarygroup (89939)     5579 2023-04-26 18:17:04.000000 dp-accounting-0.4.1/dp_accounting/privacy_accountant.py
+-rw-r-----   0 galenandrew (404454) primarygroup (89939)     4351 2023-04-26 18:17:04.000000 dp-accounting-0.4.1/dp_accounting/privacy_accountant_test.py
+drwxr-x---   0 galenandrew (404454) primarygroup (89939)        0 2023-04-26 18:20:44.118154 dp-accounting-0.4.1/dp_accounting/rdp/
+-rw-r-----   0 galenandrew (404454) primarygroup (89939)      744 2023-04-26 18:17:04.000000 dp-accounting-0.4.1/dp_accounting/rdp/__init__.py
+-rw-r-----   0 galenandrew (404454) primarygroup (89939)    33535 2023-04-26 18:17:04.000000 dp-accounting-0.4.1/dp_accounting/rdp/rdp_privacy_accountant.py
+-rw-r-----   0 galenandrew (404454) primarygroup (89939)    28704 2023-04-26 18:17:04.000000 dp-accounting-0.4.1/dp_accounting/rdp/rdp_privacy_accountant_test.py
+drwxr-x---   0 galenandrew (404454) primarygroup (89939)        0 2023-04-26 18:20:44.114154 dp-accounting-0.4.1/dp_accounting.egg-info/
+-rw-r-----   0 galenandrew (404454) primarygroup (89939)     1589 2023-04-26 18:20:44.000000 dp-accounting-0.4.1/dp_accounting.egg-info/PKG-INFO
+-rw-r-----   0 galenandrew (404454) primarygroup (89939)     1277 2023-04-26 18:20:44.000000 dp-accounting-0.4.1/dp_accounting.egg-info/SOURCES.txt
+-rw-r-----   0 galenandrew (404454) primarygroup (89939)        1 2023-04-26 18:20:44.000000 dp-accounting-0.4.1/dp_accounting.egg-info/dependency_links.txt
+-rw-r-----   0 galenandrew (404454) primarygroup (89939)       83 2023-04-26 18:20:44.000000 dp-accounting-0.4.1/dp_accounting.egg-info/requires.txt
+-rw-r-----   0 galenandrew (404454) primarygroup (89939)       14 2023-04-26 18:20:44.000000 dp-accounting-0.4.1/dp_accounting.egg-info/top_level.txt
+-rw-r-----   0 galenandrew (404454) primarygroup (89939)       38 2023-04-26 18:20:44.118154 dp-accounting-0.4.1/setup.cfg
+-rw-r-----   0 galenandrew (404454) primarygroup (89939)     2576 2023-04-26 18:17:04.000000 dp-accounting-0.4.1/setup.py
```

### Comparing `dp-accounting-0.4.0/PKG-INFO` & `dp-accounting-0.4.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dp-accounting
-Version: 0.4.0
+Version: 0.4.1
 Summary: Tools for tracking differential privacy budgets
 Home-page: https://github.com/google/differential-privacy/
 Author: Google Differential Privacy Team
 Author-email: dp-open-source@google.com
 License: Apache 2.0
 Keywords: differential-privacy accounting
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `dp-accounting-0.4.0/README.md` & `dp-accounting-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `dp-accounting-0.4.0/dp_accounting/__init__.py` & `dp-accounting-0.4.1/dp_accounting/__init__.py`

 * *Files identical despite different names*

### Comparing `dp-accounting-0.4.0/dp_accounting/dp_event_builder.py` & `dp-accounting-0.4.1/dp_accounting/dp_event_builder.py`

 * *Files identical despite different names*

### Comparing `dp-accounting-0.4.0/dp_accounting/dp_event_builder_test.py` & `dp-accounting-0.4.1/dp_accounting/dp_event_builder_test.py`

 * *Files identical despite different names*

### Comparing `dp-accounting-0.4.0/dp_accounting/mechanism_calibration.py` & `dp-accounting-0.4.1/dp_accounting/mechanism_calibration.py`

 * *Files identical despite different names*

### Comparing `dp-accounting-0.4.0/dp_accounting/mechanism_calibration_test.py` & `dp-accounting-0.4.1/dp_accounting/mechanism_calibration_test.py`

 * *Files identical despite different names*

### Comparing `dp-accounting-0.4.0/dp_accounting/pld/__init__.py` & `dp-accounting-0.4.1/dp_accounting/pld/__init__.py`

 * *Files identical despite different names*

### Comparing `dp-accounting-0.4.0/dp_accounting/pld/accountant.py` & `dp-accounting-0.4.1/dp_accounting/pld/accountant.py`

 * *Files identical despite different names*

### Comparing `dp-accounting-0.4.0/dp_accounting/pld/accountant_test.py` & `dp-accounting-0.4.1/dp_accounting/pld/accountant_test.py`

 * *Files identical despite different names*

### Comparing `dp-accounting-0.4.0/dp_accounting/pld/common.py` & `dp-accounting-0.4.1/dp_accounting/pld/common.py`

 * *Files identical despite different names*

### Comparing `dp-accounting-0.4.0/dp_accounting/pld/common_test.py` & `dp-accounting-0.4.1/dp_accounting/pld/common_test.py`

 * *Files identical despite different names*

### Comparing `dp-accounting-0.4.0/dp_accounting/pld/pld_pmf.py` & `dp-accounting-0.4.1/dp_accounting/pld/pld_pmf.py`

 * *Files identical despite different names*

### Comparing `dp-accounting-0.4.0/dp_accounting/pld/pld_pmf_test.py` & `dp-accounting-0.4.1/dp_accounting/pld/pld_pmf_test.py`

 * *Files identical despite different names*

### Comparing `dp-accounting-0.4.0/dp_accounting/pld/pld_privacy_accountant.py` & `dp-accounting-0.4.1/dp_accounting/pld/pld_privacy_accountant.py`

 * *Files identical despite different names*

### Comparing `dp-accounting-0.4.0/dp_accounting/pld/pld_privacy_accountant_test.py` & `dp-accounting-0.4.1/dp_accounting/pld/pld_privacy_accountant_test.py`

 * *Files identical despite different names*

### Comparing `dp-accounting-0.4.0/dp_accounting/pld/privacy_loss_distribution.py` & `dp-accounting-0.4.1/dp_accounting/pld/privacy_loss_distribution.py`

 * *Files identical despite different names*

### Comparing `dp-accounting-0.4.0/dp_accounting/pld/privacy_loss_distribution_basic_example.py` & `dp-accounting-0.4.1/dp_accounting/pld/privacy_loss_distribution_basic_example.py`

 * *Files identical despite different names*

### Comparing `dp-accounting-0.4.0/dp_accounting/pld/privacy_loss_distribution_test.py` & `dp-accounting-0.4.1/dp_accounting/pld/privacy_loss_distribution_test.py`

 * *Files identical despite different names*

### Comparing `dp-accounting-0.4.0/dp_accounting/pld/privacy_loss_mechanism.py` & `dp-accounting-0.4.1/dp_accounting/pld/privacy_loss_mechanism.py`

 * *Files identical despite different names*

### Comparing `dp-accounting-0.4.0/dp_accounting/pld/privacy_loss_mechanism_test.py` & `dp-accounting-0.4.1/dp_accounting/pld/privacy_loss_mechanism_test.py`

 * *Files identical despite different names*

### Comparing `dp-accounting-0.4.0/dp_accounting/pld/test_util.py` & `dp-accounting-0.4.1/dp_accounting/pld/test_util.py`

 * *Files identical despite different names*

### Comparing `dp-accounting-0.4.0/dp_accounting/pld/test_util_test.py` & `dp-accounting-0.4.1/dp_accounting/pld/test_util_test.py`

 * *Files identical despite different names*

### Comparing `dp-accounting-0.4.0/dp_accounting/privacy_accountant.py` & `dp-accounting-0.4.1/dp_accounting/privacy_accountant.py`

 * *Files identical despite different names*

### Comparing `dp-accounting-0.4.0/dp_accounting/privacy_accountant_test.py` & `dp-accounting-0.4.1/dp_accounting/privacy_accountant_test.py`

 * *Files identical despite different names*

### Comparing `dp-accounting-0.4.0/dp_accounting/rdp/__init__.py` & `dp-accounting-0.4.1/dp_accounting/rdp/__init__.py`

 * *Files identical despite different names*

### Comparing `dp-accounting-0.4.0/dp_accounting/rdp/rdp_privacy_accountant.py` & `dp-accounting-0.4.1/dp_accounting/rdp/rdp_privacy_accountant.py`

 * *Files identical despite different names*

### Comparing `dp-accounting-0.4.0/dp_accounting/rdp/rdp_privacy_accountant_test.py` & `dp-accounting-0.4.1/dp_accounting/rdp/rdp_privacy_accountant_test.py`

 * *Files identical despite different names*

### Comparing `dp-accounting-0.4.0/dp_accounting.egg-info/PKG-INFO` & `dp-accounting-0.4.1/dp_accounting.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dp-accounting
-Version: 0.4.0
+Version: 0.4.1
 Summary: Tools for tracking differential privacy budgets
 Home-page: https://github.com/google/differential-privacy/
 Author: Google Differential Privacy Team
 Author-email: dp-open-source@google.com
 License: Apache 2.0
 Keywords: differential-privacy accounting
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `dp-accounting-0.4.0/dp_accounting.egg-info/SOURCES.txt` & `dp-accounting-0.4.1/dp_accounting.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 README.md
 setup.py
 dp_accounting/__init__.py
 dp_accounting/dp_event.py
 dp_accounting/dp_event_builder.py
 dp_accounting/dp_event_builder_test.py
+dp_accounting/dp_event_test.py
 dp_accounting/mechanism_calibration.py
 dp_accounting/mechanism_calibration_test.py
 dp_accounting/privacy_accountant.py
 dp_accounting/privacy_accountant_test.py
 dp_accounting.egg-info/PKG-INFO
 dp_accounting.egg-info/SOURCES.txt
 dp_accounting.egg-info/dependency_links.txt
```

### Comparing `dp-accounting-0.4.0/setup.py` & `dp-accounting-0.4.1/setup.py`

 * *Files identical despite different names*

