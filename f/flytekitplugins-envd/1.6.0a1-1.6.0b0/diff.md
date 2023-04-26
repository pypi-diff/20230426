# Comparing `tmp/flytekitplugins-envd-1.6.0a1.tar.gz` & `tmp/flytekitplugins-envd-1.6.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-envd-1.6.0a1.tar", last modified: Wed Apr 26 20:37:25 2023, max compression
+gzip compressed data, was "flytekitplugins-envd-1.6.0b0.tar", last modified: Wed Apr 19 20:54:29 2023, max compression
```

## Comparing `flytekitplugins-envd-1.6.0a1.tar` & `flytekitplugins-envd-1.6.0b0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:37:25.825407 flytekitplugins-envd-1.6.0a1/
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-26 20:37:25.825407 flytekitplugins-envd-1.6.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-26 20:36:40.000000 flytekitplugins-envd-1.6.0a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:37:25.821407 flytekitplugins-envd-1.6.0a1/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:37:25.825407 flytekitplugins-envd-1.6.0a1/flytekitplugins/envd/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-26 20:36:40.000000 flytekitplugins-envd-1.6.0a1/flytekitplugins/envd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-04-26 20:36:40.000000 flytekitplugins-envd-1.6.0a1/flytekitplugins/envd/image_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:37:25.825407 flytekitplugins-envd-1.6.0a1/flytekitplugins_envd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-26 20:37:25.000000 flytekitplugins-envd-1.6.0a1/flytekitplugins_envd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-26 20:37:25.000000 flytekitplugins-envd-1.6.0a1/flytekitplugins_envd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 20:37:25.000000 flytekitplugins-envd-1.6.0a1/flytekitplugins_envd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-26 20:37:25.000000 flytekitplugins-envd-1.6.0a1/flytekitplugins_envd.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-26 20:37:25.000000 flytekitplugins-envd-1.6.0a1/flytekitplugins_envd.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-26 20:37:25.000000 flytekitplugins-envd-1.6.0a1/flytekitplugins_envd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-26 20:37:25.000000 flytekitplugins-envd-1.6.0a1/flytekitplugins_envd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 20:37:25.825407 flytekitplugins-envd-1.6.0a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-26 20:37:20.000000 flytekitplugins-envd-1.6.0a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:29.355070 flytekitplugins-envd-1.6.0b0/
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-19 20:54:29.355070 flytekitplugins-envd-1.6.0b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-19 20:54:06.000000 flytekitplugins-envd-1.6.0b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:29.351070 flytekitplugins-envd-1.6.0b0/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:29.351070 flytekitplugins-envd-1.6.0b0/flytekitplugins/envd/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-19 20:54:06.000000 flytekitplugins-envd-1.6.0b0/flytekitplugins/envd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-04-19 20:54:06.000000 flytekitplugins-envd-1.6.0b0/flytekitplugins/envd/image_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:29.355070 flytekitplugins-envd-1.6.0b0/flytekitplugins_envd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-19 20:54:29.000000 flytekitplugins-envd-1.6.0b0/flytekitplugins_envd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-19 20:54:29.000000 flytekitplugins-envd-1.6.0b0/flytekitplugins_envd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 20:54:29.000000 flytekitplugins-envd-1.6.0b0/flytekitplugins_envd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-19 20:54:29.000000 flytekitplugins-envd-1.6.0b0/flytekitplugins_envd.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-19 20:54:29.000000 flytekitplugins-envd-1.6.0b0/flytekitplugins_envd.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-19 20:54:29.000000 flytekitplugins-envd-1.6.0b0/flytekitplugins_envd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-19 20:54:29.000000 flytekitplugins-envd-1.6.0b0/flytekitplugins_envd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 20:54:29.355070 flytekitplugins-envd-1.6.0b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-19 20:54:25.000000 flytekitplugins-envd-1.6.0b0/setup.py
```

### Comparing `flytekitplugins-envd-1.6.0a1/PKG-INFO` & `flytekitplugins-envd-1.6.0b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-envd
-Version: 1.6.0a1
+Version: 1.6.0b0
 Summary: This package enables users to easily build a Docker image for tasks or workflows.
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-envd-1.6.0a1/README.md` & `flytekitplugins-envd-1.6.0b0/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins-envd-1.6.0a1/flytekitplugins/envd/image_builder.py` & `flytekitplugins-envd-1.6.0b0/flytekitplugins/envd/image_builder.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,17 +34,16 @@
             )
 
 
 def create_envd_config(image_spec: ImageSpec) -> str:
     base_image = DefaultImages.default_image() if image_spec.base_image is None else image_spec.base_image
     packages = [] if image_spec.packages is None else image_spec.packages
     apt_packages = [] if image_spec.apt_packages is None else image_spec.apt_packages
-    env = {"PYTHONPATH": "/root"}
-    if image_spec.env:
-        env.update(image_spec.env)
+    env = {} if image_spec.env is None else image_spec.env
+    env.update({"PYTHONPATH": "/root"})
 
     envd_config = f"""# syntax=v1
 
 def build():
     base(image="{base_image}", dev=False)
     install.python_packages(name = [{', '.join(map(str, map(lambda x: f'"{x}"', packages)))}])
     install.apt_packages(name = [{', '.join(map(str, map(lambda x: f'"{x}"', apt_packages)))}])
```

### Comparing `flytekitplugins-envd-1.6.0a1/flytekitplugins_envd.egg-info/PKG-INFO` & `flytekitplugins-envd-1.6.0b0/flytekitplugins_envd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-envd
-Version: 1.6.0a1
+Version: 1.6.0b0
 Summary: This package enables users to easily build a Docker image for tasks or workflows.
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-envd-1.6.0a1/setup.py` & `flytekitplugins-envd-1.6.0b0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "envd"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["flytekit", "envd"]
 
-__version__ = "1.6.0a1"
+__version__ = "1.6.0b0"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="This package enables users to easily build a Docker image for tasks or workflows.",
```

