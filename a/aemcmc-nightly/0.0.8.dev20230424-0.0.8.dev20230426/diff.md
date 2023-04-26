# Comparing `tmp/aemcmc-nightly-0.0.8.dev20230424.tar.gz` & `tmp/aemcmc-nightly-0.0.8.dev20230426.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aemcmc-nightly-0.0.8.dev20230424.tar", last modified: Mon Apr 24 00:59:20 2023, max compression
+gzip compressed data, was "aemcmc-nightly-0.0.8.dev20230426.tar", last modified: Wed Apr 26 00:57:29 2023, max compression
```

## Comparing `aemcmc-nightly-0.0.8.dev20230424.tar` & `aemcmc-nightly-0.0.8.dev20230426.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:59:20.046281 aemcmc-nightly-0.0.8.dev20230424/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-24 00:59:04.000000 aemcmc-nightly-0.0.8.dev20230424/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-24 00:59:04.000000 aemcmc-nightly-0.0.8.dev20230424/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-04-24 00:59:20.046281 aemcmc-nightly-0.0.8.dev20230424/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7042 2023-04-24 00:59:04.000000 aemcmc-nightly-0.0.8.dev20230424/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:59:20.046281 aemcmc-nightly-0.0.8.dev20230424/aemcmc/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-24 00:59:04.000000 aemcmc-nightly-0.0.8.dev20230424/aemcmc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-24 00:59:20.046281 aemcmc-nightly-0.0.8.dev20230424/aemcmc/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-04-24 00:59:04.000000 aemcmc-nightly-0.0.8.dev20230424/aemcmc/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     8277 2023-04-24 00:59:04.000000 aemcmc-nightly-0.0.8.dev20230424/aemcmc/conjugates.py
--rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-04-24 00:59:04.000000 aemcmc-nightly-0.0.8.dev20230424/aemcmc/dists.py
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-04-24 00:59:04.000000 aemcmc-nightly-0.0.8.dev20230424/aemcmc/ffbs.py
--rw-r--r--   0 runner    (1001) docker     (123)    24238 2023-04-24 00:59:04.000000 aemcmc-nightly-0.0.8.dev20230424/aemcmc/gibbs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7289 2023-04-24 00:59:04.000000 aemcmc-nightly-0.0.8.dev20230424/aemcmc/nuts.py
--rw-r--r--   0 runner    (1001) docker     (123)    13350 2023-04-24 00:59:04.000000 aemcmc-nightly-0.0.8.dev20230424/aemcmc/rewriting.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-24 00:59:04.000000 aemcmc-nightly-0.0.8.dev20230424/aemcmc/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-04-24 00:59:04.000000 aemcmc-nightly-0.0.8.dev20230424/aemcmc/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-04-24 00:59:04.000000 aemcmc-nightly-0.0.8.dev20230424/aemcmc/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-04-24 00:59:04.000000 aemcmc-nightly-0.0.8.dev20230424/aemcmc/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:59:20.042281 aemcmc-nightly-0.0.8.dev20230424/aemcmc_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-04-24 00:59:20.000000 aemcmc-nightly-0.0.8.dev20230424/aemcmc_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-24 00:59:20.000000 aemcmc-nightly-0.0.8.dev20230424/aemcmc_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 00:59:20.000000 aemcmc-nightly-0.0.8.dev20230424/aemcmc_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 00:59:19.000000 aemcmc-nightly-0.0.8.dev20230424/aemcmc_nightly.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-24 00:59:20.000000 aemcmc-nightly-0.0.8.dev20230424/aemcmc_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-24 00:59:20.000000 aemcmc-nightly-0.0.8.dev20230424/aemcmc_nightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-04-24 00:59:20.046281 aemcmc-nightly-0.0.8.dev20230424/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-04-24 00:59:04.000000 aemcmc-nightly-0.0.8.dev20230424/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:59:20.046281 aemcmc-nightly-0.0.8.dev20230424/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6907 2023-04-24 00:59:04.000000 aemcmc-nightly-0.0.8.dev20230424/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-04-24 00:59:04.000000 aemcmc-nightly-0.0.8.dev20230424/tests/test_conjugates.py
--rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-04-24 00:59:04.000000 aemcmc-nightly-0.0.8.dev20230424/tests/test_dists.py
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-04-24 00:59:04.000000 aemcmc-nightly-0.0.8.dev20230424/tests/test_ffbs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11323 2023-04-24 00:59:04.000000 aemcmc-nightly-0.0.8.dev20230424/tests/test_gibbs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-24 00:59:04.000000 aemcmc-nightly-0.0.8.dev20230424/tests/test_nuts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-04-24 00:59:04.000000 aemcmc-nightly-0.0.8.dev20230424/tests/test_rewriting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-24 00:59:04.000000 aemcmc-nightly-0.0.8.dev20230424/tests/test_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-04-24 00:59:04.000000 aemcmc-nightly-0.0.8.dev20230424/tests/test_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-24 00:59:04.000000 aemcmc-nightly-0.0.8.dev20230424/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    80044 2023-04-24 00:59:04.000000 aemcmc-nightly-0.0.8.dev20230424/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 00:57:29.384829 aemcmc-nightly-0.0.8.dev20230426/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-26 00:57:18.000000 aemcmc-nightly-0.0.8.dev20230426/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-26 00:57:18.000000 aemcmc-nightly-0.0.8.dev20230426/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-04-26 00:57:29.384829 aemcmc-nightly-0.0.8.dev20230426/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7042 2023-04-26 00:57:18.000000 aemcmc-nightly-0.0.8.dev20230426/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 00:57:29.384829 aemcmc-nightly-0.0.8.dev20230426/aemcmc/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-26 00:57:18.000000 aemcmc-nightly-0.0.8.dev20230426/aemcmc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-26 00:57:29.384829 aemcmc-nightly-0.0.8.dev20230426/aemcmc/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-04-26 00:57:18.000000 aemcmc-nightly-0.0.8.dev20230426/aemcmc/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8277 2023-04-26 00:57:18.000000 aemcmc-nightly-0.0.8.dev20230426/aemcmc/conjugates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-04-26 00:57:18.000000 aemcmc-nightly-0.0.8.dev20230426/aemcmc/dists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-04-26 00:57:18.000000 aemcmc-nightly-0.0.8.dev20230426/aemcmc/ffbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24238 2023-04-26 00:57:18.000000 aemcmc-nightly-0.0.8.dev20230426/aemcmc/gibbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7289 2023-04-26 00:57:18.000000 aemcmc-nightly-0.0.8.dev20230426/aemcmc/nuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13350 2023-04-26 00:57:18.000000 aemcmc-nightly-0.0.8.dev20230426/aemcmc/rewriting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-26 00:57:18.000000 aemcmc-nightly-0.0.8.dev20230426/aemcmc/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-04-26 00:57:18.000000 aemcmc-nightly-0.0.8.dev20230426/aemcmc/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-04-26 00:57:18.000000 aemcmc-nightly-0.0.8.dev20230426/aemcmc/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-04-26 00:57:18.000000 aemcmc-nightly-0.0.8.dev20230426/aemcmc/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 00:57:29.384829 aemcmc-nightly-0.0.8.dev20230426/aemcmc_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-04-26 00:57:29.000000 aemcmc-nightly-0.0.8.dev20230426/aemcmc_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-26 00:57:29.000000 aemcmc-nightly-0.0.8.dev20230426/aemcmc_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 00:57:29.000000 aemcmc-nightly-0.0.8.dev20230426/aemcmc_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 00:57:29.000000 aemcmc-nightly-0.0.8.dev20230426/aemcmc_nightly.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-26 00:57:29.000000 aemcmc-nightly-0.0.8.dev20230426/aemcmc_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-26 00:57:29.000000 aemcmc-nightly-0.0.8.dev20230426/aemcmc_nightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-04-26 00:57:29.384829 aemcmc-nightly-0.0.8.dev20230426/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-04-26 00:57:18.000000 aemcmc-nightly-0.0.8.dev20230426/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 00:57:29.384829 aemcmc-nightly-0.0.8.dev20230426/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6907 2023-04-26 00:57:18.000000 aemcmc-nightly-0.0.8.dev20230426/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-04-26 00:57:18.000000 aemcmc-nightly-0.0.8.dev20230426/tests/test_conjugates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-04-26 00:57:18.000000 aemcmc-nightly-0.0.8.dev20230426/tests/test_dists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-04-26 00:57:18.000000 aemcmc-nightly-0.0.8.dev20230426/tests/test_ffbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11323 2023-04-26 00:57:18.000000 aemcmc-nightly-0.0.8.dev20230426/tests/test_gibbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-26 00:57:18.000000 aemcmc-nightly-0.0.8.dev20230426/tests/test_nuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-04-26 00:57:18.000000 aemcmc-nightly-0.0.8.dev20230426/tests/test_rewriting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-26 00:57:18.000000 aemcmc-nightly-0.0.8.dev20230426/tests/test_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-04-26 00:57:18.000000 aemcmc-nightly-0.0.8.dev20230426/tests/test_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-26 00:57:18.000000 aemcmc-nightly-0.0.8.dev20230426/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80044 2023-04-26 00:57:18.000000 aemcmc-nightly-0.0.8.dev20230426/versioneer.py
```

### Comparing `aemcmc-nightly-0.0.8.dev20230424/LICENSE` & `aemcmc-nightly-0.0.8.dev20230426/LICENSE`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230424/PKG-INFO` & `aemcmc-nightly-0.0.8.dev20230426/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aemcmc-nightly
-Version: 0.0.8.dev20230424
+Version: 0.0.8.dev20230426
 Summary: Miscellaneous MCMC samplers written in Aesara
 Home-page: http://github.com/aesara-devs/aemcmc
 Author: aesara-devs
 Author-email: aesara.devs@gmail.com
 Keywords: math,probability,numerical,symbolic,MCMC
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `aemcmc-nightly-0.0.8.dev20230424/README.md` & `aemcmc-nightly-0.0.8.dev20230426/README.md`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230424/aemcmc/basic.py` & `aemcmc-nightly-0.0.8.dev20230426/aemcmc/basic.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230424/aemcmc/conjugates.py` & `aemcmc-nightly-0.0.8.dev20230426/aemcmc/conjugates.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230424/aemcmc/dists.py` & `aemcmc-nightly-0.0.8.dev20230426/aemcmc/dists.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230424/aemcmc/ffbs.py` & `aemcmc-nightly-0.0.8.dev20230426/aemcmc/ffbs.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230424/aemcmc/gibbs.py` & `aemcmc-nightly-0.0.8.dev20230426/aemcmc/gibbs.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230424/aemcmc/nuts.py` & `aemcmc-nightly-0.0.8.dev20230426/aemcmc/nuts.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230424/aemcmc/rewriting.py` & `aemcmc-nightly-0.0.8.dev20230426/aemcmc/rewriting.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230424/aemcmc/sample.py` & `aemcmc-nightly-0.0.8.dev20230426/aemcmc/sample.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230424/aemcmc/transforms.py` & `aemcmc-nightly-0.0.8.dev20230426/aemcmc/transforms.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230424/aemcmc/types.py` & `aemcmc-nightly-0.0.8.dev20230426/aemcmc/types.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230424/aemcmc/utils.py` & `aemcmc-nightly-0.0.8.dev20230426/aemcmc/utils.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230424/aemcmc_nightly.egg-info/PKG-INFO` & `aemcmc-nightly-0.0.8.dev20230426/aemcmc_nightly.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aemcmc-nightly
-Version: 0.0.8.dev20230424
+Version: 0.0.8.dev20230426
 Summary: Miscellaneous MCMC samplers written in Aesara
 Home-page: http://github.com/aesara-devs/aemcmc
 Author: aesara-devs
 Author-email: aesara.devs@gmail.com
 Keywords: math,probability,numerical,symbolic,MCMC
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `aemcmc-nightly-0.0.8.dev20230424/aemcmc_nightly.egg-info/SOURCES.txt` & `aemcmc-nightly-0.0.8.dev20230426/aemcmc_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230424/setup.cfg` & `aemcmc-nightly-0.0.8.dev20230426/setup.cfg`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230424/setup.py` & `aemcmc-nightly-0.0.8.dev20230426/setup.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230424/tests/test_basic.py` & `aemcmc-nightly-0.0.8.dev20230426/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230424/tests/test_conjugates.py` & `aemcmc-nightly-0.0.8.dev20230426/tests/test_conjugates.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230424/tests/test_dists.py` & `aemcmc-nightly-0.0.8.dev20230426/tests/test_dists.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230424/tests/test_ffbs.py` & `aemcmc-nightly-0.0.8.dev20230426/tests/test_ffbs.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230424/tests/test_gibbs.py` & `aemcmc-nightly-0.0.8.dev20230426/tests/test_gibbs.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230424/tests/test_nuts.py` & `aemcmc-nightly-0.0.8.dev20230426/tests/test_nuts.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230424/tests/test_rewriting.py` & `aemcmc-nightly-0.0.8.dev20230426/tests/test_rewriting.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230424/tests/test_sample.py` & `aemcmc-nightly-0.0.8.dev20230426/tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230424/tests/test_transforms.py` & `aemcmc-nightly-0.0.8.dev20230426/tests/test_transforms.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230424/tests/test_utils.py` & `aemcmc-nightly-0.0.8.dev20230426/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230424/versioneer.py` & `aemcmc-nightly-0.0.8.dev20230426/versioneer.py`

 * *Files identical despite different names*

