# Comparing `tmp/medcam3d-0.0.1.tar.gz` & `tmp/medcam3d-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medcam3d-0.0.1.tar", last modified: Wed Apr 26 17:03:36 2023, max compression
+gzip compressed data, was "medcam3d-0.0.3.tar", last modified: Wed Apr 26 17:36:57 2023, max compression
```

## Comparing `medcam3d-0.0.1.tar` & `medcam3d-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 jjia      (1592) afd_b     (1487)        0 2023-04-26 17:03:36.000000 medcam3d-0.0.1/
--rw-r--r--   0 jjia      (1592) afd_b     (1487)     1072 2023-04-23 14:18:38.000000 medcam3d-0.0.1/LICENSE
--rw-r--r--   0 jjia      (1592) afd_b     (1487)     1853 2023-04-26 17:03:36.000000 medcam3d-0.0.1/PKG-INFO
--rw-r--r--   0 jjia      (1592) afd_b     (1487)     1343 2023-04-26 16:56:47.000000 medcam3d-0.0.1/README.md
-drwxr-xr-x   0 jjia      (1592) afd_b     (1487)        0 2023-04-26 17:03:36.000000 medcam3d-0.0.1/medcam3d/
--rw-r--r--   0 jjia      (1592) afd_b     (1487)       39 2023-04-23 21:52:28.000000 medcam3d-0.0.1/medcam3d/__init__.py
--rw-r--r--   0 jjia      (1592) afd_b     (1487)     1932 2023-04-24 16:43:09.000000 medcam3d-0.0.1/medcam3d/activations_and_gradients.py
--rw-r--r--   0 jjia      (1592) afd_b     (1487)    12375 2023-04-26 16:52:13.000000 medcam3d-0.0.1/medcam3d/base_medcam3d.py
--rw-r--r--   0 jjia      (1592) afd_b     (1487)      927 2023-04-26 16:18:10.000000 medcam3d-0.0.1/medcam3d/grad_cam3d.py
-drwxr-xr-x   0 jjia      (1592) afd_b     (1487)        0 2023-04-26 17:03:36.000000 medcam3d-0.0.1/medcam3d.egg-info/
--rw-r--r--   0 jjia      (1592) afd_b     (1487)     1853 2023-04-26 17:03:36.000000 medcam3d-0.0.1/medcam3d.egg-info/PKG-INFO
--rw-r--r--   0 jjia      (1592) afd_b     (1487)      293 2023-04-26 17:03:36.000000 medcam3d-0.0.1/medcam3d.egg-info/SOURCES.txt
--rw-r--r--   0 jjia      (1592) afd_b     (1487)        1 2023-04-26 17:03:36.000000 medcam3d-0.0.1/medcam3d.egg-info/dependency_links.txt
--rw-r--r--   0 jjia      (1592) afd_b     (1487)       94 2023-04-26 17:03:36.000000 medcam3d-0.0.1/medcam3d.egg-info/requires.txt
--rw-r--r--   0 jjia      (1592) afd_b     (1487)        9 2023-04-26 17:03:36.000000 medcam3d-0.0.1/medcam3d.egg-info/top_level.txt
--rw-r--r--   0 jjia      (1592) afd_b     (1487)       38 2023-04-26 17:03:36.000000 medcam3d-0.0.1/setup.cfg
--rw-r--r--   0 jjia      (1592) afd_b     (1487)      914 2023-04-23 14:16:53.000000 medcam3d-0.0.1/setup.py
+drwxr-xr-x   0 jjia      (1592) afd_b     (1487)        0 2023-04-26 17:36:57.000000 medcam3d-0.0.3/
+-rw-r--r--   0 jjia      (1592) afd_b     (1487)     1072 2023-04-23 14:18:38.000000 medcam3d-0.0.3/LICENSE
+-rw-r--r--   0 jjia      (1592) afd_b     (1487)     4117 2023-04-26 17:36:57.000000 medcam3d-0.0.3/PKG-INFO
+-rw-r--r--   0 jjia      (1592) afd_b     (1487)     3607 2023-04-26 17:34:19.000000 medcam3d-0.0.3/README.md
+drwxr-xr-x   0 jjia      (1592) afd_b     (1487)        0 2023-04-26 17:36:57.000000 medcam3d-0.0.3/medcam3d/
+-rw-r--r--   0 jjia      (1592) afd_b     (1487)       39 2023-04-23 21:52:28.000000 medcam3d-0.0.3/medcam3d/__init__.py
+-rw-r--r--   0 jjia      (1592) afd_b     (1487)     1932 2023-04-24 16:43:09.000000 medcam3d-0.0.3/medcam3d/activations_and_gradients.py
+-rw-r--r--   0 jjia      (1592) afd_b     (1487)    12375 2023-04-26 16:52:13.000000 medcam3d-0.0.3/medcam3d/base_medcam3d.py
+-rw-r--r--   0 jjia      (1592) afd_b     (1487)      927 2023-04-26 16:18:10.000000 medcam3d-0.0.3/medcam3d/grad_cam3d.py
+drwxr-xr-x   0 jjia      (1592) afd_b     (1487)        0 2023-04-26 17:36:57.000000 medcam3d-0.0.3/medcam3d.egg-info/
+-rw-r--r--   0 jjia      (1592) afd_b     (1487)     4117 2023-04-26 17:36:56.000000 medcam3d-0.0.3/medcam3d.egg-info/PKG-INFO
+-rw-r--r--   0 jjia      (1592) afd_b     (1487)      293 2023-04-26 17:36:57.000000 medcam3d-0.0.3/medcam3d.egg-info/SOURCES.txt
+-rw-r--r--   0 jjia      (1592) afd_b     (1487)        1 2023-04-26 17:36:56.000000 medcam3d-0.0.3/medcam3d.egg-info/dependency_links.txt
+-rw-r--r--   0 jjia      (1592) afd_b     (1487)       94 2023-04-26 17:36:56.000000 medcam3d-0.0.3/medcam3d.egg-info/requires.txt
+-rw-r--r--   0 jjia      (1592) afd_b     (1487)        9 2023-04-26 17:36:56.000000 medcam3d-0.0.3/medcam3d.egg-info/top_level.txt
+-rw-r--r--   0 jjia      (1592) afd_b     (1487)       38 2023-04-26 17:36:57.000000 medcam3d-0.0.3/setup.cfg
+-rw-r--r--   0 jjia      (1592) afd_b     (1487)      914 2023-04-26 17:36:01.000000 medcam3d-0.0.3/setup.py
```

### Comparing `medcam3d-0.0.1/LICENSE` & `medcam3d-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `medcam3d-0.0.1/medcam3d/activations_and_gradients.py` & `medcam3d-0.0.3/medcam3d/activations_and_gradients.py`

 * *Files identical despite different names*

### Comparing `medcam3d-0.0.1/medcam3d/base_medcam3d.py` & `medcam3d-0.0.3/medcam3d/base_medcam3d.py`

 * *Files identical despite different names*

### Comparing `medcam3d-0.0.1/medcam3d/grad_cam3d.py` & `medcam3d-0.0.3/medcam3d/grad_cam3d.py`

 * *Files identical despite different names*

### Comparing `medcam3d-0.0.1/setup.py` & `medcam3d-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open("requirements.txt", "r") as f:
     requirements = f.readlines()
 
 setuptools.setup(
     name='medcam3d',
-    version='0.0.1',
+    version='0.0.3',
     author='Jingnan Jia',
     author_email='jiajingnan2222@gmail.com',
     description='CAM for 3D medical image networks',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/Jingnan-Jia/medcam3d',
     project_urls={
```

