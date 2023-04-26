# Comparing `tmp/efficientbioai-0.0.5.tar.gz` & `tmp/efficientbioai-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "efficientbioai-0.0.5.tar", last modified: Tue Apr 25 16:16:20 2023, max compression
+gzip compressed data, was "efficientbioai-0.0.6.tar", last modified: Tue Apr 25 16:29:35 2023, max compression
```

## Comparing `efficientbioai-0.0.5.tar` & `efficientbioai-0.0.6.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:20.837324 efficientbioai-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-25 16:16:09.000000 efficientbioai-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-25 16:16:20.837324 efficientbioai-0.0.5/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     2424 2023-04-25 16:16:09.000000 efficientbioai-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:20.833324 efficientbioai-0.0.5/efficientbioai/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-25 16:16:09.000000 efficientbioai-0.0.5/efficientbioai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-04-25 16:16:09.000000 efficientbioai-0.0.5/efficientbioai/compress.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:20.837324 efficientbioai-0.0.5/efficientbioai/compress_ppl/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-25 16:16:09.000000 efficientbioai-0.0.5/efficientbioai/compress_ppl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6204 2023-04-25 16:16:09.000000 efficientbioai-0.0.5/efficientbioai/compress_ppl/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-04-25 16:16:09.000000 efficientbioai-0.0.5/efficientbioai/compress_ppl/pruner.py
--rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-04-25 16:16:09.000000 efficientbioai-0.0.5/efficientbioai/compress_ppl/quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:20.837324 efficientbioai-0.0.5/efficientbioai/infer/
--rwxr-xr-x   0 runner    (1001) docker     (123)      127 2023-04-25 16:16:09.000000 efficientbioai-0.0.5/efficientbioai/infer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:20.837324 efficientbioai-0.0.5/efficientbioai/infer/backend/
--rwxr-xr-x   0 runner    (1001) docker     (123)       82 2023-04-25 16:16:09.000000 efficientbioai-0.0.5/efficientbioai/infer/backend/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1628 2023-04-25 16:16:09.000000 efficientbioai-0.0.5/efficientbioai/infer/backend/openvino.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3800 2023-04-25 16:16:09.000000 efficientbioai-0.0.5/efficientbioai/infer/backend/tensorrt.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3786 2023-04-25 16:16:09.000000 efficientbioai-0.0.5/efficientbioai/infer/base.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9046 2023-04-25 16:16:09.000000 efficientbioai-0.0.5/efficientbioai/infer/mmv_im2im.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2459 2023-04-25 16:16:09.000000 efficientbioai-0.0.5/efficientbioai/infer/omnipose.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1103 2023-04-25 16:16:09.000000 efficientbioai-0.0.5/efficientbioai/inference.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3996 2023-04-25 16:16:09.000000 efficientbioai-0.0.5/efficientbioai/onnx2trt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:20.837324 efficientbioai-0.0.5/efficientbioai/parse_info/
--rwxr-xr-x   0 runner    (1001) docker     (123)       49 2023-04-25 16:16:09.000000 efficientbioai-0.0.5/efficientbioai/parse_info/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      383 2023-04-25 16:16:09.000000 efficientbioai-0.0.5/efficientbioai/parse_info/base.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4014 2023-04-25 16:16:09.000000 efficientbioai-0.0.5/efficientbioai/parse_info/mmv_im2im.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3058 2023-04-25 16:16:09.000000 efficientbioai-0.0.5/efficientbioai/parse_info/omnipose.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2837 2023-04-25 16:16:09.000000 efficientbioai-0.0.5/efficientbioai/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:20.837324 efficientbioai-0.0.5/efficientbioai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-25 16:16:20.000000 efficientbioai-0.0.5/efficientbioai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-25 16:16:20.000000 efficientbioai-0.0.5/efficientbioai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 16:16:20.000000 efficientbioai-0.0.5/efficientbioai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 16:16:20.000000 efficientbioai-0.0.5/efficientbioai.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-25 16:16:20.000000 efficientbioai-0.0.5/efficientbioai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-25 16:16:20.000000 efficientbioai-0.0.5/efficientbioai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-25 16:16:20.841324 efficientbioai-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-25 16:16:09.000000 efficientbioai-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:29:35.818927 efficientbioai-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-25 16:29:27.000000 efficientbioai-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-04-25 16:29:35.818927 efficientbioai-0.0.6/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2424 2023-04-25 16:29:27.000000 efficientbioai-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:29:35.818927 efficientbioai-0.0.6/efficientbioai/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-25 16:29:27.000000 efficientbioai-0.0.6/efficientbioai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-04-25 16:29:27.000000 efficientbioai-0.0.6/efficientbioai/compress.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:29:35.818927 efficientbioai-0.0.6/efficientbioai/compress_ppl/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-25 16:29:27.000000 efficientbioai-0.0.6/efficientbioai/compress_ppl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6204 2023-04-25 16:29:27.000000 efficientbioai-0.0.6/efficientbioai/compress_ppl/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-04-25 16:29:27.000000 efficientbioai-0.0.6/efficientbioai/compress_ppl/pruner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-04-25 16:29:27.000000 efficientbioai-0.0.6/efficientbioai/compress_ppl/quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:29:35.818927 efficientbioai-0.0.6/efficientbioai/infer/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      127 2023-04-25 16:29:27.000000 efficientbioai-0.0.6/efficientbioai/infer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:29:35.818927 efficientbioai-0.0.6/efficientbioai/infer/backend/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       82 2023-04-25 16:29:27.000000 efficientbioai-0.0.6/efficientbioai/infer/backend/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1628 2023-04-25 16:29:27.000000 efficientbioai-0.0.6/efficientbioai/infer/backend/openvino.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3800 2023-04-25 16:29:27.000000 efficientbioai-0.0.6/efficientbioai/infer/backend/tensorrt.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3786 2023-04-25 16:29:27.000000 efficientbioai-0.0.6/efficientbioai/infer/base.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9046 2023-04-25 16:29:27.000000 efficientbioai-0.0.6/efficientbioai/infer/mmv_im2im.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2459 2023-04-25 16:29:27.000000 efficientbioai-0.0.6/efficientbioai/infer/omnipose.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1103 2023-04-25 16:29:27.000000 efficientbioai-0.0.6/efficientbioai/inference.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3996 2023-04-25 16:29:27.000000 efficientbioai-0.0.6/efficientbioai/onnx2trt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:29:35.818927 efficientbioai-0.0.6/efficientbioai/parse_info/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       49 2023-04-25 16:29:27.000000 efficientbioai-0.0.6/efficientbioai/parse_info/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      383 2023-04-25 16:29:27.000000 efficientbioai-0.0.6/efficientbioai/parse_info/base.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4014 2023-04-25 16:29:27.000000 efficientbioai-0.0.6/efficientbioai/parse_info/mmv_im2im.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3058 2023-04-25 16:29:27.000000 efficientbioai-0.0.6/efficientbioai/parse_info/omnipose.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2837 2023-04-25 16:29:27.000000 efficientbioai-0.0.6/efficientbioai/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:29:35.818927 efficientbioai-0.0.6/efficientbioai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-04-25 16:29:35.000000 efficientbioai-0.0.6/efficientbioai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-25 16:29:35.000000 efficientbioai-0.0.6/efficientbioai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 16:29:35.000000 efficientbioai-0.0.6/efficientbioai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 16:29:35.000000 efficientbioai-0.0.6/efficientbioai.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-25 16:29:35.000000 efficientbioai-0.0.6/efficientbioai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-25 16:29:35.000000 efficientbioai-0.0.6/efficientbioai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-25 16:29:35.822927 efficientbioai-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-04-25 16:29:27.000000 efficientbioai-0.0.6/setup.py
```

### Comparing `efficientbioai-0.0.5/LICENSE` & `efficientbioai-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `efficientbioai-0.0.5/README.md` & `efficientbioai-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `efficientbioai-0.0.5/efficientbioai/compress.py` & `efficientbioai-0.0.6/efficientbioai/compress.py`

 * *Files identical despite different names*

### Comparing `efficientbioai-0.0.5/efficientbioai/compress_ppl/pipeline.py` & `efficientbioai-0.0.6/efficientbioai/compress_ppl/pipeline.py`

 * *Files identical despite different names*

### Comparing `efficientbioai-0.0.5/efficientbioai/compress_ppl/pruner.py` & `efficientbioai-0.0.6/efficientbioai/compress_ppl/pruner.py`

 * *Files identical despite different names*

### Comparing `efficientbioai-0.0.5/efficientbioai/compress_ppl/quantizer.py` & `efficientbioai-0.0.6/efficientbioai/compress_ppl/quantizer.py`

 * *Files identical despite different names*

### Comparing `efficientbioai-0.0.5/efficientbioai/infer/backend/openvino.py` & `efficientbioai-0.0.6/efficientbioai/infer/backend/openvino.py`

 * *Files identical despite different names*

### Comparing `efficientbioai-0.0.5/efficientbioai/infer/backend/tensorrt.py` & `efficientbioai-0.0.6/efficientbioai/infer/backend/tensorrt.py`

 * *Files identical despite different names*

### Comparing `efficientbioai-0.0.5/efficientbioai/infer/base.py` & `efficientbioai-0.0.6/efficientbioai/infer/base.py`

 * *Files identical despite different names*

### Comparing `efficientbioai-0.0.5/efficientbioai/infer/mmv_im2im.py` & `efficientbioai-0.0.6/efficientbioai/infer/mmv_im2im.py`

 * *Files identical despite different names*

### Comparing `efficientbioai-0.0.5/efficientbioai/infer/omnipose.py` & `efficientbioai-0.0.6/efficientbioai/infer/omnipose.py`

 * *Files identical despite different names*

### Comparing `efficientbioai-0.0.5/efficientbioai/inference.py` & `efficientbioai-0.0.6/efficientbioai/inference.py`

 * *Files identical despite different names*

### Comparing `efficientbioai-0.0.5/efficientbioai/onnx2trt.py` & `efficientbioai-0.0.6/efficientbioai/onnx2trt.py`

 * *Files identical despite different names*

### Comparing `efficientbioai-0.0.5/efficientbioai/parse_info/mmv_im2im.py` & `efficientbioai-0.0.6/efficientbioai/parse_info/mmv_im2im.py`

 * *Files identical despite different names*

### Comparing `efficientbioai-0.0.5/efficientbioai/parse_info/omnipose.py` & `efficientbioai-0.0.6/efficientbioai/parse_info/omnipose.py`

 * *Files identical despite different names*

### Comparing `efficientbioai-0.0.5/efficientbioai/utils.py` & `efficientbioai-0.0.6/efficientbioai/utils.py`

 * *Files identical despite different names*

### Comparing `efficientbioai-0.0.5/efficientbioai.egg-info/SOURCES.txt` & `efficientbioai-0.0.6/efficientbioai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `efficientbioai-0.0.5/setup.py` & `efficientbioai-0.0.6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 from setuptools import setup, find_packages
 
+with open("README.md") as readme_file:
+    readme = readme_file.read()
+
 setup_requirements = [
     "pytest-runner>=5.2",
 ]
 
 requirements = [
     "numpy",
     "codecarbon",  # for measuring energy consumption
@@ -39,15 +42,17 @@
     "test": test_requirements,
 }
 
 setup(
     name="efficientbioai",
     keywords="deep learning, quantization, microscopy model compression",
     description="efficientbioai is a python package for efficient deep learning in bioimaging",
-    version="0.0.5",
+    long_description=readme,
+    long_description_content_type="text/markdown",
+    version="0.0.6",
     author="mmv_lab team",
     author_email="yu.zhou@isas.de",
     packages=find_packages(),
     python_requires=">=3.8",
     install_requires=requirements,
     tests_require=test_requirements,
     extras_require=extra_requirements,  # install use: pip install efficientbioai[tensorrt/openvino/all]
```

