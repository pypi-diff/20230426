# Comparing `tmp/nua_autobuild-0.5.13.tar.gz` & `tmp/nua_autobuild-0.5.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nua_autobuild-0.5.13.tar", max compression
+gzip compressed data, was "nua_autobuild-0.5.14.tar", max compression
```

## Comparing `nua_autobuild-0.5.13.tar` & `nua_autobuild-0.5.14.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      805 2023-04-24 21:25:56.858863 nua_autobuild-0.5.13/README.md
--rw-r--r--   0        0        0     1489 2023-04-24 21:27:50.225404 nua_autobuild-0.5.13/pyproject.toml
--rw-r--r--   0        0        0      100 2022-12-12 07:55:21.315857 nua_autobuild-0.5.13/src/nua/autobuild/__init__.py
--rw-r--r--   0        0        0      209 2023-02-28 08:14:12.792663 nua_autobuild-0.5.13/src/nua/autobuild/builders/Dockerfile_nua_builder_node14
--rw-r--r--   0        0        0      209 2023-02-28 08:14:12.793610 nua_autobuild-0.5.13/src/nua/autobuild/builders/Dockerfile_nua_builder_node16
--rw-r--r--   0        0        0      208 2023-02-28 08:14:12.794118 nua_autobuild-0.5.13/src/nua/autobuild/builders/Dockerfile_nua_builder_ruby27
--rw-r--r--   0        0        0      208 2023-02-28 08:14:12.794341 nua_autobuild-0.5.13/src/nua/autobuild/builders/Dockerfile_nua_builder_ruby272
--rw-r--r--   0        0        0      208 2023-02-28 08:14:12.794590 nua_autobuild-0.5.13/src/nua/autobuild/builders/Dockerfile_nua_builder_ruby31
--rw-r--r--   0        0        0      208 2023-02-28 08:14:12.794704 nua_autobuild-0.5.13/src/nua/autobuild/builders/Dockerfile_nua_builder_ruby32
--rw-r--r--   0        0        0        0 2023-02-28 08:14:12.794746 nua_autobuild-0.5.13/src/nua/autobuild/builders/__init__.py
--rw-r--r--   0        0        0      309 2023-02-28 08:14:12.795139 nua_autobuild-0.5.13/src/nua/autobuild/builders/node14.json
--rw-r--r--   0        0        0      309 2023-02-28 08:14:12.795558 nua_autobuild-0.5.13/src/nua/autobuild/builders/node16.json
--rw-r--r--   0        0        0      245 2023-02-28 08:14:12.795648 nua_autobuild-0.5.13/src/nua/autobuild/builders/ruby27.json
--rw-r--r--   0        0        0      225 2023-02-28 08:14:12.795727 nua_autobuild-0.5.13/src/nua/autobuild/builders/ruby272.json
--rw-r--r--   0        0        0      245 2023-02-28 08:14:12.795791 nua_autobuild-0.5.13/src/nua/autobuild/builders/ruby31.json
--rw-r--r--   0        0        0      245 2023-02-28 08:14:12.795854 nua_autobuild-0.5.13/src/nua/autobuild/builders/ruby32.json
--rw-r--r--   0        0        0      340 2023-04-17 20:51:18.651586 nua_autobuild-0.5.13/src/nua/autobuild/constants.py
--rw-r--r--   0        0        0     6231 2023-04-24 21:25:56.860466 nua_autobuild-0.5.13/src/nua/autobuild/docker_build_utils.py
--rw-r--r--   0        0        0      225 2023-02-06 17:21:30.495528 nua_autobuild-0.5.13/src/nua/autobuild/dockerfiles/Dockerfile_nua_builder_slim
--rw-r--r--   0        0        0     1556 2022-12-12 07:55:21.316202 nua_autobuild-0.5.13/src/nua/autobuild/dockerfiles/Dockerfile_nua_python_slim
--rw-r--r--   0        0        0        0 2022-12-20 18:49:45.394740 nua_autobuild-0.5.13/src/nua/autobuild/dockerfiles/__init__.py
--rw-r--r--   0        0        0     1651 2023-04-16 21:09:47.366763 nua_autobuild-0.5.13/src/nua/autobuild/main.py
--rw-r--r--   0        0        0     6604 2023-04-16 21:09:47.366818 nua_autobuild-0.5.13/src/nua/autobuild/nua_image_builder.py
--rw-r--r--   0        0        0     5234 2023-04-16 10:25:52.984339 nua_autobuild-0.5.13/src/nua/autobuild/nua_wheel_builder.py
--rw-r--r--   0        0        0     3233 2023-04-24 21:25:56.860659 nua_autobuild-0.5.13/src/nua/autobuild/register_builders.py
--rw-r--r--   0        0        0       85 2022-12-12 07:55:21.316458 nua_autobuild-0.5.13/src/nua/autobuild/version.py
--rw-r--r--   0        0        0     1504 1970-01-01 00:00:00.000000 nua_autobuild-0.5.13/PKG-INFO
+-rw-r--r--   0        0        0      805 2023-04-24 21:25:56.858863 nua_autobuild-0.5.14/README.md
+-rw-r--r--   0        0        0     1489 2023-04-26 06:46:46.010889 nua_autobuild-0.5.14/pyproject.toml
+-rw-r--r--   0        0        0      100 2022-12-12 07:55:21.315857 nua_autobuild-0.5.14/src/nua/autobuild/__init__.py
+-rw-r--r--   0        0        0      209 2023-02-28 08:14:12.792663 nua_autobuild-0.5.14/src/nua/autobuild/builders/Dockerfile_nua_builder_node14
+-rw-r--r--   0        0        0      209 2023-02-28 08:14:12.793610 nua_autobuild-0.5.14/src/nua/autobuild/builders/Dockerfile_nua_builder_node16
+-rw-r--r--   0        0        0      208 2023-02-28 08:14:12.794118 nua_autobuild-0.5.14/src/nua/autobuild/builders/Dockerfile_nua_builder_ruby27
+-rw-r--r--   0        0        0      208 2023-02-28 08:14:12.794341 nua_autobuild-0.5.14/src/nua/autobuild/builders/Dockerfile_nua_builder_ruby272
+-rw-r--r--   0        0        0      208 2023-02-28 08:14:12.794590 nua_autobuild-0.5.14/src/nua/autobuild/builders/Dockerfile_nua_builder_ruby31
+-rw-r--r--   0        0        0      208 2023-02-28 08:14:12.794704 nua_autobuild-0.5.14/src/nua/autobuild/builders/Dockerfile_nua_builder_ruby32
+-rw-r--r--   0        0        0        0 2023-02-28 08:14:12.794746 nua_autobuild-0.5.14/src/nua/autobuild/builders/__init__.py
+-rw-r--r--   0        0        0      309 2023-02-28 08:14:12.795139 nua_autobuild-0.5.14/src/nua/autobuild/builders/node14.json
+-rw-r--r--   0        0        0      309 2023-02-28 08:14:12.795558 nua_autobuild-0.5.14/src/nua/autobuild/builders/node16.json
+-rw-r--r--   0        0        0      245 2023-02-28 08:14:12.795648 nua_autobuild-0.5.14/src/nua/autobuild/builders/ruby27.json
+-rw-r--r--   0        0        0      225 2023-02-28 08:14:12.795727 nua_autobuild-0.5.14/src/nua/autobuild/builders/ruby272.json
+-rw-r--r--   0        0        0      245 2023-02-28 08:14:12.795791 nua_autobuild-0.5.14/src/nua/autobuild/builders/ruby31.json
+-rw-r--r--   0        0        0      245 2023-02-28 08:14:12.795854 nua_autobuild-0.5.14/src/nua/autobuild/builders/ruby32.json
+-rw-r--r--   0        0        0      340 2023-04-17 20:51:18.651586 nua_autobuild-0.5.14/src/nua/autobuild/constants.py
+-rw-r--r--   0        0        0     6231 2023-04-24 21:25:56.860466 nua_autobuild-0.5.14/src/nua/autobuild/docker_build_utils.py
+-rw-r--r--   0        0        0      225 2023-02-06 17:21:30.495528 nua_autobuild-0.5.14/src/nua/autobuild/dockerfiles/Dockerfile_nua_builder_slim
+-rw-r--r--   0        0        0     1556 2022-12-12 07:55:21.316202 nua_autobuild-0.5.14/src/nua/autobuild/dockerfiles/Dockerfile_nua_python_slim
+-rw-r--r--   0        0        0        0 2022-12-20 18:49:45.394740 nua_autobuild-0.5.14/src/nua/autobuild/dockerfiles/__init__.py
+-rw-r--r--   0        0        0     1651 2023-04-16 21:09:47.366763 nua_autobuild-0.5.14/src/nua/autobuild/main.py
+-rw-r--r--   0        0        0     6604 2023-04-16 21:09:47.366818 nua_autobuild-0.5.14/src/nua/autobuild/nua_image_builder.py
+-rw-r--r--   0        0        0     5234 2023-04-16 10:25:52.984339 nua_autobuild-0.5.14/src/nua/autobuild/nua_wheel_builder.py
+-rw-r--r--   0        0        0     3233 2023-04-24 21:25:56.860659 nua_autobuild-0.5.14/src/nua/autobuild/register_builders.py
+-rw-r--r--   0        0        0       85 2022-12-12 07:55:21.316458 nua_autobuild-0.5.14/src/nua/autobuild/version.py
+-rw-r--r--   0        0        0     1504 1970-01-01 00:00:00.000000 nua_autobuild-0.5.14/PKG-INFO
```

### Comparing `nua_autobuild-0.5.13/README.md` & `nua_autobuild-0.5.14/README.md`

 * *Files identical despite different names*

### Comparing `nua_autobuild-0.5.13/pyproject.toml` & `nua_autobuild-0.5.14/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "nua-autobuild"
-version = "0.5.13"
+version = "0.5.14"
 description = "Nua self builder"
 authors = ["Stefane Fermigier <sf@abilian.com>", "Jerome Dumonteil <jd@abilian.com>"]
 license = "AGPL"
 readme = "README.md"
 packages = [
   { include = "nua", from = "src" }
 ]
 
 [tool.poetry.scripts]
 nua-self-build = "nua.autobuild.main:app"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 setuptools = "*"
-nua-lib = "=0.5.13"
-nua-agent = "=0.5.13"
+nua-lib = "=0.5.14"
+nua-agent = "=0.5.14"
 tomli = "^2.0.1"
 tomli-w = "^1.0.0"
 docker = "^6.0"
 paramiko = "*"
 typer = {version = "^0.7.0", extras = ["all"]}
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `nua_autobuild-0.5.13/src/nua/autobuild/docker_build_utils.py` & `nua_autobuild-0.5.14/src/nua/autobuild/docker_build_utils.py`

 * *Files identical despite different names*

### Comparing `nua_autobuild-0.5.13/src/nua/autobuild/dockerfiles/Dockerfile_nua_python_slim` & `nua_autobuild-0.5.14/src/nua/autobuild/dockerfiles/Dockerfile_nua_python_slim`

 * *Files identical despite different names*

### Comparing `nua_autobuild-0.5.13/src/nua/autobuild/main.py` & `nua_autobuild-0.5.14/src/nua/autobuild/main.py`

 * *Files identical despite different names*

### Comparing `nua_autobuild-0.5.13/src/nua/autobuild/nua_image_builder.py` & `nua_autobuild-0.5.14/src/nua/autobuild/nua_image_builder.py`

 * *Files identical despite different names*

### Comparing `nua_autobuild-0.5.13/src/nua/autobuild/nua_wheel_builder.py` & `nua_autobuild-0.5.14/src/nua/autobuild/nua_wheel_builder.py`

 * *Files identical despite different names*

### Comparing `nua_autobuild-0.5.13/src/nua/autobuild/register_builders.py` & `nua_autobuild-0.5.14/src/nua/autobuild/register_builders.py`

 * *Files identical despite different names*

### Comparing `nua_autobuild-0.5.13/PKG-INFO` & `nua_autobuild-0.5.14/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: nua-autobuild
-Version: 0.5.13
+Version: 0.5.14
 Summary: Nua self builder
 License: AGPL
 Author: Stefane Fermigier
 Author-email: sf@abilian.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: docker (>=6.0,<7.0)
-Requires-Dist: nua-agent (==0.5.13)
-Requires-Dist: nua-lib (==0.5.13)
+Requires-Dist: nua-agent (==0.5.14)
+Requires-Dist: nua-lib (==0.5.14)
 Requires-Dist: paramiko
 Requires-Dist: setuptools
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Requires-Dist: tomli-w (>=1.0.0,<2.0.0)
 Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
 Description-Content-Type: text/markdown
```

