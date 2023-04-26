# Comparing `tmp/GPTCovLet-0.1.1.tar.gz` & `tmp/GPTCovLet-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GPTCovLet-0.1.1.tar", last modified: Wed Apr  5 20:57:48 2023, max compression
+gzip compressed data, was "GPTCovLet-0.1.2.tar", last modified: Wed Apr 26 19:23:57 2023, max compression
```

## Comparing `GPTCovLet-0.1.1.tar` & `GPTCovLet-0.1.2.tar`

### file list

```diff
@@ -1,25 +1,31 @@
-drwxr-xr-x   0 jaesungpark   (501) staff       (20)        0 2023-04-05 20:57:48.527601 GPTCovLet-0.1.1/
--rw-r--r--   0 jaesungpark   (501) staff       (20)      254 2023-04-05 19:56:22.000000 GPTCovLet-0.1.1/CONTRIBUTING.md
-drwxr-xr-x   0 jaesungpark   (501) staff       (20)        0 2023-04-05 20:57:48.524540 GPTCovLet-0.1.1/GPTCovLet.egg-info/
--rw-r--r--   0 jaesungpark   (501) staff       (20)      122 2023-04-05 20:57:48.000000 GPTCovLet-0.1.1/GPTCovLet.egg-info/PKG-INFO
--rw-r--r--   0 jaesungpark   (501) staff       (20)      429 2023-04-05 20:57:48.000000 GPTCovLet-0.1.1/GPTCovLet.egg-info/SOURCES.txt
--rw-r--r--   0 jaesungpark   (501) staff       (20)        1 2023-04-05 20:57:48.000000 GPTCovLet-0.1.1/GPTCovLet.egg-info/dependency_links.txt
--rw-r--r--   0 jaesungpark   (501) staff       (20)      116 2023-04-05 20:57:48.000000 GPTCovLet-0.1.1/GPTCovLet.egg-info/requires.txt
--rw-r--r--   0 jaesungpark   (501) staff       (20)       12 2023-04-05 20:57:48.000000 GPTCovLet-0.1.1/GPTCovLet.egg-info/top_level.txt
-drwxr-xr-x   0 jaesungpark   (501) staff       (20)        0 2023-04-05 20:57:48.525191 GPTCovLet-0.1.1/GPT_Cov_Let/
--rw-r--r--   0 jaesungpark   (501) staff       (20)        0 2023-03-08 23:59:27.000000 GPTCovLet-0.1.1/GPT_Cov_Let/__init__.py
--rw-r--r--   0 jaesungpark   (501) staff       (20)      280 2023-03-21 21:12:21.000000 GPTCovLet-0.1.1/GPT_Cov_Let/__main__.py
--rw-r--r--   0 jaesungpark   (501) staff       (20)       22 2023-04-05 20:05:43.000000 GPTCovLet-0.1.1/GPT_Cov_Let/_version.py
--rw-r--r--   0 jaesungpark   (501) staff       (20)     2287 2023-03-21 21:25:06.000000 GPTCovLet-0.1.1/GPT_Cov_Let/scrapeToGPT.py
-drwxr-xr-x   0 jaesungpark   (501) staff       (20)        0 2023-04-05 20:57:48.527224 GPTCovLet-0.1.1/GPT_Cov_Let/tests/
--rw-r--r--   0 jaesungpark   (501) staff       (20)   628396 2023-03-02 01:28:42.000000 GPTCovLet-0.1.1/GPT_Cov_Let/tests/staticPageUnitTest.html
--rw-r--r--   0 jaesungpark   (501) staff       (20)     1561 2023-03-28 01:59:24.000000 GPTCovLet-0.1.1/GPT_Cov_Let/tests/test_all.py
--rw-r--r--   0 jaesungpark   (501) staff       (20)     1069 2023-04-03 02:20:06.000000 GPTCovLet-0.1.1/LICENSE
--rw-r--r--   0 jaesungpark   (501) staff       (20)      661 2023-04-05 20:31:03.000000 GPTCovLet-0.1.1/MANIFEST.in
--rw-r--r--   0 jaesungpark   (501) staff       (20)      786 2023-03-28 21:31:08.000000 GPTCovLet-0.1.1/Makefile
--rw-r--r--   0 jaesungpark   (501) staff       (20)      122 2023-04-05 20:57:48.527478 GPTCovLet-0.1.1/PKG-INFO
--rw-r--r--   0 jaesungpark   (501) staff       (20)      571 2023-04-05 19:56:22.000000 GPTCovLet-0.1.1/README.md
--rw-r--r--   0 jaesungpark   (501) staff       (20)      397 2023-03-10 20:00:37.000000 GPTCovLet-0.1.1/bumpversion.cfg
--rw-r--r--   0 jaesungpark   (501) staff       (20)      476 2023-04-05 20:24:45.000000 GPTCovLet-0.1.1/pyproject.toml
--rw-r--r--   0 jaesungpark   (501) staff       (20)       38 2023-04-05 20:57:48.527642 GPTCovLet-0.1.1/setup.cfg
--rw-r--r--   0 jaesungpark   (501) staff       (20)       39 2023-03-08 22:03:42.000000 GPTCovLet-0.1.1/setup.py
+drwxr-xr-x   0 jaesungpark   (501) staff       (20)        0 2023-04-26 19:23:57.435224 GPTCovLet-0.1.2/
+-rw-r--r--   0 jaesungpark   (501) staff       (20)      254 2023-04-05 19:56:22.000000 GPTCovLet-0.1.2/CONTRIBUTING.md
+drwxr-xr-x   0 jaesungpark   (501) staff       (20)        0 2023-04-26 19:23:57.430865 GPTCovLet-0.1.2/GPTCovLet.egg-info/
+-rw-r--r--   0 jaesungpark   (501) staff       (20)      122 2023-04-26 19:23:57.000000 GPTCovLet-0.1.2/GPTCovLet.egg-info/PKG-INFO
+-rw-r--r--   0 jaesungpark   (501) staff       (20)      499 2023-04-26 19:23:57.000000 GPTCovLet-0.1.2/GPTCovLet.egg-info/SOURCES.txt
+-rw-r--r--   0 jaesungpark   (501) staff       (20)        1 2023-04-26 19:23:57.000000 GPTCovLet-0.1.2/GPTCovLet.egg-info/dependency_links.txt
+-rw-r--r--   0 jaesungpark   (501) staff       (20)      116 2023-04-26 19:23:57.000000 GPTCovLet-0.1.2/GPTCovLet.egg-info/requires.txt
+-rw-r--r--   0 jaesungpark   (501) staff       (20)        1 2023-04-26 19:23:57.000000 GPTCovLet-0.1.2/GPTCovLet.egg-info/top_level.txt
+drwxr-xr-x   0 jaesungpark   (501) staff       (20)        0 2023-04-26 19:23:57.431629 GPTCovLet-0.1.2/GPT_Cov_Let/
+-rw-r--r--   0 jaesungpark   (501) staff       (20)        0 2023-03-08 23:59:27.000000 GPTCovLet-0.1.2/GPT_Cov_Let/__init__.py
+-rw-r--r--   0 jaesungpark   (501) staff       (20)      280 2023-03-21 21:12:21.000000 GPTCovLet-0.1.2/GPT_Cov_Let/__main__.py
+-rw-r--r--   0 jaesungpark   (501) staff       (20)       22 2023-04-26 01:58:47.000000 GPTCovLet-0.1.2/GPT_Cov_Let/_version.py
+-rw-r--r--   0 jaesungpark   (501) staff       (20)     3880 2023-04-26 01:58:47.000000 GPTCovLet-0.1.2/GPT_Cov_Let/scrapeToGPT.py
+drwxr-xr-x   0 jaesungpark   (501) staff       (20)        0 2023-04-26 19:23:57.433704 GPTCovLet-0.1.2/GPT_Cov_Let/tests/
+-rw-r--r--   0 jaesungpark   (501) staff       (20)   628396 2023-03-02 01:28:42.000000 GPTCovLet-0.1.2/GPT_Cov_Let/tests/staticPageUnitTest.html
+-rw-r--r--   0 jaesungpark   (501) staff       (20)     1561 2023-03-28 01:59:24.000000 GPTCovLet-0.1.2/GPT_Cov_Let/tests/test_all.py
+-rw-r--r--   0 jaesungpark   (501) staff       (20)     1069 2023-04-03 02:20:06.000000 GPTCovLet-0.1.2/LICENSE
+-rw-r--r--   0 jaesungpark   (501) staff       (20)      779 2023-04-25 20:30:39.000000 GPTCovLet-0.1.2/MANIFEST.in
+-rw-r--r--   0 jaesungpark   (501) staff       (20)      786 2023-03-28 21:31:08.000000 GPTCovLet-0.1.2/Makefile
+-rw-r--r--   0 jaesungpark   (501) staff       (20)      122 2023-04-26 19:23:57.435046 GPTCovLet-0.1.2/PKG-INFO
+-rw-r--r--   0 jaesungpark   (501) staff       (20)      977 2023-04-26 01:58:47.000000 GPTCovLet-0.1.2/README.md
+-rw-r--r--   0 jaesungpark   (501) staff       (20)      397 2023-04-26 01:58:47.000000 GPTCovLet-0.1.2/bumpversion.cfg
+drwxr-xr-x   0 jaesungpark   (501) staff       (20)        0 2023-04-26 19:23:57.434265 GPTCovLet-0.1.2/docs/
+-rw-r--r--   0 jaesungpark   (501) staff       (20)      638 2023-04-13 20:59:44.000000 GPTCovLet-0.1.2/docs/Makefile
+-rw-r--r--   0 jaesungpark   (501) staff       (20)      804 2023-04-13 20:59:44.000000 GPTCovLet-0.1.2/docs/make.bat
+drwxr-xr-x   0 jaesungpark   (501) staff       (20)        0 2023-04-26 19:23:57.434737 GPTCovLet-0.1.2/docs/source/
+-rw-r--r--   0 jaesungpark   (501) staff       (20)     1080 2023-04-13 21:19:43.000000 GPTCovLet-0.1.2/docs/source/conf.py
+-rw-r--r--   0 jaesungpark   (501) staff       (20)      498 2023-04-13 21:23:23.000000 GPTCovLet-0.1.2/docs/source/index.rst
+-rw-r--r--   0 jaesungpark   (501) staff       (20)      510 2023-04-26 01:58:47.000000 GPTCovLet-0.1.2/pyproject.toml
+-rw-r--r--   0 jaesungpark   (501) staff       (20)       38 2023-04-26 19:23:57.435271 GPTCovLet-0.1.2/setup.cfg
+-rw-r--r--   0 jaesungpark   (501) staff       (20)       39 2023-03-08 22:03:42.000000 GPTCovLet-0.1.2/setup.py
```

### Comparing `GPTCovLet-0.1.1/GPT_Cov_Let/tests/staticPageUnitTest.html` & `GPTCovLet-0.1.2/GPT_Cov_Let/tests/staticPageUnitTest.html`

 * *Files identical despite different names*

### Comparing `GPTCovLet-0.1.1/GPT_Cov_Let/tests/test_all.py` & `GPTCovLet-0.1.2/GPT_Cov_Let/tests/test_all.py`

 * *Files identical despite different names*

### Comparing `GPTCovLet-0.1.1/LICENSE` & `GPTCovLet-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `GPTCovLet-0.1.1/MANIFEST.in` & `GPTCovLet-0.1.2/MANIFEST.in`

 * *Files 22% similar despite different names*

```diff
@@ -27,7 +27,11 @@
 recursive-include GPT_Cov_Let *.js
 recursive-include GPT_Cov_Let *.swp
 recursive-include build *.html
 recursive-include build *.js
 recursive-include build *.py
 recursive-include build *.swp
 
+recursive-include docs *.bat
+recursive-include docs *.py
+recursive-include docs *.rst
+recursive-include docs Makefile
```

### Comparing `GPTCovLet-0.1.1/Makefile` & `GPTCovLet-0.1.2/Makefile`

 * *Files identical despite different names*

