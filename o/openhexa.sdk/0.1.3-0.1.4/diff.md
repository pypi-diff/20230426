# Comparing `tmp/openhexa.sdk-0.1.3.tar.gz` & `tmp/openhexa.sdk-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openhexa.sdk-0.1.3.tar", last modified: Wed Apr 26 12:24:08 2023, max compression
+gzip compressed data, was "openhexa.sdk-0.1.4.tar", last modified: Wed Apr 26 12:52:01 2023, max compression
```

## Comparing `openhexa.sdk-0.1.3.tar` & `openhexa.sdk-0.1.4.tar`

### file list

```diff
@@ -1,40 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 12:24:08.884614 openhexa.sdk-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-26 12:23:49.000000 openhexa.sdk-0.1.3/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-04-26 12:24:08.884614 openhexa.sdk-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-04-26 12:23:49.000000 openhexa.sdk-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 12:24:08.872614 openhexa.sdk-0.1.3/openhexa/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-26 12:23:49.000000 openhexa.sdk-0.1.3/openhexa/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 12:24:08.880614 openhexa.sdk-0.1.3/openhexa/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-26 12:23:49.000000 openhexa.sdk-0.1.3/openhexa/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-04-26 12:23:49.000000 openhexa.sdk-0.1.3/openhexa/cli/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10061 2023-04-26 12:23:49.000000 openhexa.sdk-0.1.3/openhexa/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 12:24:08.880614 openhexa.sdk-0.1.3/openhexa/sdk/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-26 12:23:49.000000 openhexa.sdk-0.1.3/openhexa/sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 12:24:08.884614 openhexa.sdk-0.1.3/openhexa/sdk/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-26 12:23:49.000000 openhexa.sdk-0.1.3/openhexa/sdk/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-04-26 12:23:49.000000 openhexa.sdk-0.1.3/openhexa/sdk/pipelines/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-04-26 12:23:49.000000 openhexa.sdk-0.1.3/openhexa/sdk/pipelines/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-04-26 12:23:49.000000 openhexa.sdk-0.1.3/openhexa/sdk/pipelines/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-04-26 12:23:49.000000 openhexa.sdk-0.1.3/openhexa/sdk/pipelines/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-04-26 12:23:49.000000 openhexa.sdk-0.1.3/openhexa/sdk/pipelines/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-04-26 12:23:49.000000 openhexa.sdk-0.1.3/openhexa/sdk/pipelines/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 12:23:49.000000 openhexa.sdk-0.1.3/openhexa/sdk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 12:24:08.884614 openhexa.sdk-0.1.3/openhexa/sdk/workspaces/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-26 12:23:49.000000 openhexa.sdk-0.1.3/openhexa/sdk/workspaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-26 12:23:49.000000 openhexa.sdk-0.1.3/openhexa/sdk/workspaces/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-04-26 12:23:49.000000 openhexa.sdk-0.1.3/openhexa/sdk/workspaces/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 12:24:08.876614 openhexa.sdk-0.1.3/openhexa.sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-04-26 12:24:08.000000 openhexa.sdk-0.1.3/openhexa.sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-26 12:24:08.000000 openhexa.sdk-0.1.3/openhexa.sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 12:24:08.000000 openhexa.sdk-0.1.3/openhexa.sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-26 12:24:08.000000 openhexa.sdk-0.1.3/openhexa.sdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-26 12:24:08.000000 openhexa.sdk-0.1.3/openhexa.sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-26 12:24:08.000000 openhexa.sdk-0.1.3/openhexa.sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 12:23:56.000000 openhexa.sdk-0.1.3/openhexa.sdk.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-26 12:23:49.000000 openhexa.sdk-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-26 12:24:08.884614 openhexa.sdk-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-26 12:23:49.000000 openhexa.sdk-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 12:24:08.884614 openhexa.sdk-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 12:23:49.000000 openhexa.sdk-0.1.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7394 2023-04-26 12:23:49.000000 openhexa.sdk-0.1.3/tests/test_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-04-26 12:23:49.000000 openhexa.sdk-0.1.3/tests/test_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 12:52:01.963214 openhexa.sdk-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-26 12:51:45.000000 openhexa.sdk-0.1.4/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-26 12:51:45.000000 openhexa.sdk-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-04-26 12:52:01.963214 openhexa.sdk-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-04-26 12:51:45.000000 openhexa.sdk-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 12:52:01.955214 openhexa.sdk-0.1.4/openhexa/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-26 12:51:45.000000 openhexa.sdk-0.1.4/openhexa/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 12:52:01.959214 openhexa.sdk-0.1.4/openhexa/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-26 12:51:45.000000 openhexa.sdk-0.1.4/openhexa/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-04-26 12:51:45.000000 openhexa.sdk-0.1.4/openhexa/cli/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10130 2023-04-26 12:51:45.000000 openhexa.sdk-0.1.4/openhexa/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 12:52:01.959214 openhexa.sdk-0.1.4/openhexa/cli/skeleton/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-26 12:51:45.000000 openhexa.sdk-0.1.4/openhexa/cli/skeleton/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-26 12:51:45.000000 openhexa.sdk-0.1.4/openhexa/cli/skeleton/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-26 12:51:45.000000 openhexa.sdk-0.1.4/openhexa/cli/skeleton/workspace.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 12:52:01.959214 openhexa.sdk-0.1.4/openhexa/sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-26 12:51:45.000000 openhexa.sdk-0.1.4/openhexa/sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 12:52:01.963214 openhexa.sdk-0.1.4/openhexa/sdk/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-26 12:51:45.000000 openhexa.sdk-0.1.4/openhexa/sdk/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-04-26 12:51:45.000000 openhexa.sdk-0.1.4/openhexa/sdk/pipelines/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-04-26 12:51:45.000000 openhexa.sdk-0.1.4/openhexa/sdk/pipelines/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-04-26 12:51:45.000000 openhexa.sdk-0.1.4/openhexa/sdk/pipelines/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-04-26 12:51:45.000000 openhexa.sdk-0.1.4/openhexa/sdk/pipelines/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-04-26 12:51:45.000000 openhexa.sdk-0.1.4/openhexa/sdk/pipelines/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-04-26 12:51:45.000000 openhexa.sdk-0.1.4/openhexa/sdk/pipelines/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 12:51:45.000000 openhexa.sdk-0.1.4/openhexa/sdk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 12:52:01.963214 openhexa.sdk-0.1.4/openhexa/sdk/workspaces/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-26 12:51:45.000000 openhexa.sdk-0.1.4/openhexa/sdk/workspaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-26 12:51:45.000000 openhexa.sdk-0.1.4/openhexa/sdk/workspaces/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-04-26 12:51:45.000000 openhexa.sdk-0.1.4/openhexa/sdk/workspaces/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 12:52:01.955214 openhexa.sdk-0.1.4/openhexa.sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-04-26 12:52:01.000000 openhexa.sdk-0.1.4/openhexa.sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-26 12:52:01.000000 openhexa.sdk-0.1.4/openhexa.sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 12:52:01.000000 openhexa.sdk-0.1.4/openhexa.sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-26 12:52:01.000000 openhexa.sdk-0.1.4/openhexa.sdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-26 12:52:01.000000 openhexa.sdk-0.1.4/openhexa.sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-26 12:52:01.000000 openhexa.sdk-0.1.4/openhexa.sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 12:51:51.000000 openhexa.sdk-0.1.4/openhexa.sdk.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-26 12:51:45.000000 openhexa.sdk-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-26 12:52:01.967214 openhexa.sdk-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-26 12:51:45.000000 openhexa.sdk-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 12:52:01.963214 openhexa.sdk-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 12:51:45.000000 openhexa.sdk-0.1.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7394 2023-04-26 12:51:45.000000 openhexa.sdk-0.1.4/tests/test_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-04-26 12:51:45.000000 openhexa.sdk-0.1.4/tests/test_pipeline.py
```

### Comparing `openhexa.sdk-0.1.3/LICENCE` & `openhexa.sdk-0.1.4/LICENCE`

 * *Files identical despite different names*

### Comparing `openhexa.sdk-0.1.3/PKG-INFO` & `openhexa.sdk-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openhexa.sdk
-Version: 0.1.3
+Version: 0.1.4
 Summary: OpenHexa SDK
 Home-page: https://github.com/BLSQ/openhexa-sdk-python
 Author: Bluesquare
 Author-email: dev@bluesquarehub.com
 License: MIT License
 Keywords: openhexa,pipelines
 Classifier: Programming Language :: Python :: 3
```

### Comparing `openhexa.sdk-0.1.3/README.md` & `openhexa.sdk-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `openhexa.sdk-0.1.3/openhexa/cli/api.py` & `openhexa.sdk-0.1.4/openhexa/cli/api.py`

 * *Files identical despite different names*

### Comparing `openhexa.sdk-0.1.3/openhexa/cli/cli.py` & `openhexa.sdk-0.1.4/openhexa/cli/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,14 +177,18 @@
     if ctx.invoked_subcommand is None:
         ctx.forward(pipelines_list)
 
 
 @pipelines.command("init")
 @click.argument("name", type=str)
 def pipelines_init(name: str):
+    """
+    Initialize a new pipeline in a fresh directory.
+    """
+
     new_pipeline_directory_name = stringcase.snakecase(name)
     new_pipeline_path = Path.cwd() / Path(stringcase.snakecase(name))
     if new_pipeline_path.exists():
         click.echo(
             f"There is already a {name} directory in the current directory. Please choose a new name "
             f"for your pipeline.",
             err=True,
```

### Comparing `openhexa.sdk-0.1.3/openhexa/sdk/pipelines/parameter.py` & `openhexa.sdk-0.1.4/openhexa/sdk/pipelines/parameter.py`

 * *Files identical despite different names*

### Comparing `openhexa.sdk-0.1.3/openhexa/sdk/pipelines/pipeline.py` & `openhexa.sdk-0.1.4/openhexa/sdk/pipelines/pipeline.py`

 * *Files identical despite different names*

### Comparing `openhexa.sdk-0.1.3/openhexa/sdk/pipelines/run.py` & `openhexa.sdk-0.1.4/openhexa/sdk/pipelines/run.py`

 * *Files identical despite different names*

### Comparing `openhexa.sdk-0.1.3/openhexa/sdk/pipelines/runtime.py` & `openhexa.sdk-0.1.4/openhexa/sdk/pipelines/runtime.py`

 * *Files identical despite different names*

### Comparing `openhexa.sdk-0.1.3/openhexa/sdk/pipelines/task.py` & `openhexa.sdk-0.1.4/openhexa/sdk/pipelines/task.py`

 * *Files identical despite different names*

### Comparing `openhexa.sdk-0.1.3/openhexa/sdk/pipelines/utils.py` & `openhexa.sdk-0.1.4/openhexa/sdk/pipelines/utils.py`

 * *Files identical despite different names*

### Comparing `openhexa.sdk-0.1.3/openhexa/sdk/workspaces/workspace.py` & `openhexa.sdk-0.1.4/openhexa/sdk/workspaces/workspace.py`

 * *Files identical despite different names*

### Comparing `openhexa.sdk-0.1.3/openhexa.sdk.egg-info/PKG-INFO` & `openhexa.sdk-0.1.4/openhexa.sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openhexa.sdk
-Version: 0.1.3
+Version: 0.1.4
 Summary: OpenHexa SDK
 Home-page: https://github.com/BLSQ/openhexa-sdk-python
 Author: Bluesquare
 Author-email: dev@bluesquarehub.com
 License: MIT License
 Keywords: openhexa,pipelines
 Classifier: Programming Language :: Python :: 3
```

### Comparing `openhexa.sdk-0.1.3/openhexa.sdk.egg-info/SOURCES.txt` & `openhexa.sdk-0.1.4/openhexa.sdk.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 LICENCE
+MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 openhexa/__init__.py
 openhexa.sdk.egg-info/PKG-INFO
 openhexa.sdk.egg-info/SOURCES.txt
@@ -10,14 +11,17 @@
 openhexa.sdk.egg-info/entry_points.txt
 openhexa.sdk.egg-info/requires.txt
 openhexa.sdk.egg-info/top_level.txt
 openhexa.sdk.egg-info/zip-safe
 openhexa/cli/__init__.py
 openhexa/cli/api.py
 openhexa/cli/cli.py
+openhexa/cli/skeleton/.gitignore
+openhexa/cli/skeleton/pipeline.py
+openhexa/cli/skeleton/workspace.yaml
 openhexa/sdk/__init__.py
 openhexa/sdk/utils.py
 openhexa/sdk/pipelines/__init__.py
 openhexa/sdk/pipelines/parameter.py
 openhexa/sdk/pipelines/pipeline.py
 openhexa/sdk/pipelines/run.py
 openhexa/sdk/pipelines/runtime.py
```

### Comparing `openhexa.sdk-0.1.3/pyproject.toml` & `openhexa.sdk-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `openhexa.sdk-0.1.3/setup.cfg` & `openhexa.sdk-0.1.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `openhexa.sdk-0.1.3/tests/test_parameter.py` & `openhexa.sdk-0.1.4/tests/test_parameter.py`

 * *Files identical despite different names*

### Comparing `openhexa.sdk-0.1.3/tests/test_pipeline.py` & `openhexa.sdk-0.1.4/tests/test_pipeline.py`

 * *Files identical despite different names*

