# Comparing `tmp/vdk-gdp-execution-id-0.0.841725879.tar.gz` & `tmp/vdk-gdp-execution-id-0.0.848464550.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vdk-gdp-execution-id-0.0.841725879.tar", last modified: Wed Apr 19 07:51:22 2023, max compression
+gzip compressed data, was "vdk-gdp-execution-id-0.0.848464550.tar", last modified: Tue Apr 25 14:42:02 2023, max compression
```

## Comparing `vdk-gdp-execution-id-0.0.841725879.tar` & `vdk-gdp-execution-id-0.0.848464550.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 07:51:22.394838 vdk-gdp-execution-id-0.0.841725879/
--rw-r--r--   0 root         (0) root         (0)     3622 2023-04-19 07:51:22.394838 vdk-gdp-execution-id-0.0.841725879/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2937 2023-04-19 07:51:09.000000 vdk-gdp-execution-id-0.0.841725879/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-19 07:51:22.394838 vdk-gdp-execution-id-0.0.841725879/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1229 2023-04-19 07:51:13.000000 vdk-gdp-execution-id-0.0.841725879/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 07:51:22.394838 vdk-gdp-execution-id-0.0.841725879/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 07:51:22.394838 vdk-gdp-execution-id-0.0.841725879/src/vdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 07:51:22.394838 vdk-gdp-execution-id-0.0.841725879/src/vdk/plugin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 07:51:22.394838 vdk-gdp-execution-id-0.0.841725879/src/vdk/plugin/gdp/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 07:51:22.394838 vdk-gdp-execution-id-0.0.841725879/src/vdk/plugin/gdp/execution_id/
--rw-rw-rw-   0 root         (0) root         (0)      824 2023-04-19 07:51:09.000000 vdk-gdp-execution-id-0.0.841725879/src/vdk/plugin/gdp/execution_id/gdp_execution_id_configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     2362 2023-04-19 07:51:09.000000 vdk-gdp-execution-id-0.0.841725879/src/vdk/plugin/gdp/execution_id/gdp_execution_id_plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 07:51:22.394838 vdk-gdp-execution-id-0.0.841725879/src/vdk_gdp_execution_id.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3622 2023-04-19 07:51:22.000000 vdk-gdp-execution-id-0.0.841725879/src/vdk_gdp_execution_id.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      433 2023-04-19 07:51:22.000000 vdk-gdp-execution-id-0.0.841725879/src/vdk_gdp_execution_id.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 07:51:22.000000 vdk-gdp-execution-id-0.0.841725879/src/vdk_gdp_execution_id.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       92 2023-04-19 07:51:22.000000 vdk-gdp-execution-id-0.0.841725879/src/vdk_gdp_execution_id.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-04-19 07:51:22.000000 vdk-gdp-execution-id-0.0.841725879/src/vdk_gdp_execution_id.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-04-19 07:51:22.000000 vdk-gdp-execution-id-0.0.841725879/src/vdk_gdp_execution_id.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 14:42:02.588134 vdk-gdp-execution-id-0.0.848464550/
+-rw-r--r--   0 root         (0) root         (0)     3622 2023-04-25 14:42:02.588134 vdk-gdp-execution-id-0.0.848464550/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2937 2023-04-25 14:41:49.000000 vdk-gdp-execution-id-0.0.848464550/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-25 14:42:02.588134 vdk-gdp-execution-id-0.0.848464550/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1229 2023-04-25 14:41:53.000000 vdk-gdp-execution-id-0.0.848464550/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 14:42:02.588134 vdk-gdp-execution-id-0.0.848464550/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 14:42:02.588134 vdk-gdp-execution-id-0.0.848464550/src/vdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 14:42:02.588134 vdk-gdp-execution-id-0.0.848464550/src/vdk/plugin/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 14:42:02.588134 vdk-gdp-execution-id-0.0.848464550/src/vdk/plugin/gdp/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 14:42:02.588134 vdk-gdp-execution-id-0.0.848464550/src/vdk/plugin/gdp/execution_id/
+-rw-rw-rw-   0 root         (0) root         (0)      824 2023-04-25 14:41:49.000000 vdk-gdp-execution-id-0.0.848464550/src/vdk/plugin/gdp/execution_id/gdp_execution_id_configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     2322 2023-04-25 14:41:49.000000 vdk-gdp-execution-id-0.0.848464550/src/vdk/plugin/gdp/execution_id/gdp_execution_id_plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 14:42:02.588134 vdk-gdp-execution-id-0.0.848464550/src/vdk_gdp_execution_id.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3622 2023-04-25 14:42:02.000000 vdk-gdp-execution-id-0.0.848464550/src/vdk_gdp_execution_id.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      433 2023-04-25 14:42:02.000000 vdk-gdp-execution-id-0.0.848464550/src/vdk_gdp_execution_id.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 14:42:02.000000 vdk-gdp-execution-id-0.0.848464550/src/vdk_gdp_execution_id.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       92 2023-04-25 14:42:02.000000 vdk-gdp-execution-id-0.0.848464550/src/vdk_gdp_execution_id.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-04-25 14:42:02.000000 vdk-gdp-execution-id-0.0.848464550/src/vdk_gdp_execution_id.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-04-25 14:42:02.000000 vdk-gdp-execution-id-0.0.848464550/src/vdk_gdp_execution_id.egg-info/top_level.txt
```

### Comparing `vdk-gdp-execution-id-0.0.841725879/PKG-INFO` & `vdk-gdp-execution-id-0.0.848464550/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-gdp-execution-id
-Version: 0.0.841725879
+Version: 0.0.848464550
 Summary: This Versatile Data Kit SDK plugin is a Generative Data Pack, that expands each ingested dataset with the execution ID detected during data job run.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `vdk-gdp-execution-id-0.0.841725879/README.md` & `vdk-gdp-execution-id-0.0.848464550/README.md`

 * *Files identical despite different names*

### Comparing `vdk-gdp-execution-id-0.0.841725879/setup.py` & `vdk-gdp-execution-id-0.0.848464550/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import pathlib
 
 import setuptools
 
-__version__ = "0.0.841725879"
+__version__ = "0.0.848464550"
 
 setuptools.setup(
     name="vdk-gdp-execution-id",
     version=__version__,
     url="https://github.com/vmware/versatile-data-kit",
     description="This Versatile Data Kit SDK plugin is a Generative Data Pack, that expands each ingested dataset "
     "with the execution ID detected during data job run.",
```

### Comparing `vdk-gdp-execution-id-0.0.841725879/src/vdk/plugin/gdp/execution_id/gdp_execution_id_configuration.py` & `vdk-gdp-execution-id-0.0.848464550/src/vdk/plugin/gdp/execution_id/gdp_execution_id_configuration.py`

 * *Files identical despite different names*

### Comparing `vdk-gdp-execution-id-0.0.841725879/src/vdk/plugin/gdp/execution_id/gdp_execution_id_plugin.py` & `vdk-gdp-execution-id-0.0.848464550/src/vdk/plugin/gdp/execution_id/gdp_execution_id_plugin.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 from vdk.internal.builtin_plugins.run.job_context import JobContext
 from vdk.internal.core.config import ConfigurationBuilder
 from vdk.internal.core.statestore import CommonStoreKeys
 from vdk.plugin.gdp.execution_id.gdp_execution_id_configuration import add_definitions
 from vdk.plugin.gdp.execution_id.gdp_execution_id_configuration import (
     GdpExecutionIdPluginConfiguration,
 )
-from vdk.plugin.test_utils.ingest_util_plugins import IngestionMetadata
 
 GDP_EXECUTION_ID_MICRO_DIMENSION_NAME = "GDP_EXECUTION_ID_MICRO_DIMENSION_NAME"
 
 log = logging.getLogger(__name__)
 
 
 class GdpExecutionIdPlugin(IIngesterPlugin):
@@ -30,16 +29,16 @@
 
     def pre_ingest_process(
         self,
         payload: List[dict],
         destination_table: Optional[str] = None,
         target: Optional[str] = None,
         collection_id: Optional[str] = None,
-        metadata: Optional[IngestionMetadata] = None,
-    ) -> Tuple[List[Dict], Optional[IngestionMetadata]]:
+        metadata: Optional[IIngesterPlugin.IngestionMetadata] = None,
+    ) -> Tuple[List[Dict], Optional[IIngesterPlugin.IngestionMetadata]]:
         for p in payload:
             p.update({self._plugin_config.micro_dimension_name(): self.__execution_id})
         return payload, metadata
 
     @hookimpl
     def initialize_job(self, context: JobContext) -> None:
         log.info("Initialize data job with GDP Execution ID Plugin.")
```

### Comparing `vdk-gdp-execution-id-0.0.841725879/src/vdk_gdp_execution_id.egg-info/PKG-INFO` & `vdk-gdp-execution-id-0.0.848464550/src/vdk_gdp_execution_id.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-gdp-execution-id
-Version: 0.0.841725879
+Version: 0.0.848464550
 Summary: This Versatile Data Kit SDK plugin is a Generative Data Pack, that expands each ingested dataset with the execution ID detected during data job run.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

