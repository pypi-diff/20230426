# Comparing `tmp/hoppr-1.8.3.tar.gz` & `tmp/hoppr-1.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hoppr-1.8.3.tar", max compression
+gzip compressed data, was "hoppr-1.8.4.tar", max compression
```

## Comparing `hoppr-1.8.3.tar` & `hoppr-1.8.4.tar`

### file list

```diff
@@ -1,61 +1,61 @@
--rw-r--r--   0        0        0     1084 2023-04-24 21:09:54.000000 hoppr-1.8.3/LICENSE
--rw-r--r--   0        0        0     1214 2023-04-24 21:09:54.000000 hoppr-1.8.3/README.md
--rw-r--r--   0        0        0     1035 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/__init__.py
--rw-r--r--   0        0        0      161 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/__main__.py
--rw-r--r--   0        0        0        0 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/base_plugins/__init__.py
--rw-r--r--   0        0        0    10990 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/base_plugins/collector.py
--rw-r--r--   0        0        0    10732 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/base_plugins/hoppr.py
--rw-r--r--   0        0        0        0 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/base_plugins/py.typed
--rw-r--r--   0        0        0        0 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/cli/__init__.py
--rw-r--r--   0        0        0     6256 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/cli/hopctl.py
--rw-r--r--   0        0        0      563 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/constants.py
--rw-r--r--   0        0        0        0 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/core_plugins/__init__.py
--rw-r--r--   0        0        0     3046 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/core_plugins/bundle_tar.py
--rw-r--r--   0        0        0    12943 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/core_plugins/collect_apt_plugin.py
--rw-r--r--   0        0        0    10272 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/core_plugins/collect_dnf_plugin.py
--rw-r--r--   0        0        0     3321 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/core_plugins/collect_docker_plugin.py
--rw-r--r--   0        0        0     4664 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/core_plugins/collect_git_plugin.py
--rw-r--r--   0        0        0     3992 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/core_plugins/collect_helm_plugin.py
--rw-r--r--   0        0        0     6369 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/core_plugins/collect_maven_plugin.py
--rw-r--r--   0        0        0     7978 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/core_plugins/collect_nexus_search.py
--rw-r--r--   0        0        0     4418 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/core_plugins/collect_pypi_plugin.py
--rw-r--r--   0        0        0     3043 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/core_plugins/collect_raw_plugin.py
--rw-r--r--   0        0        0     3739 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/core_plugins/collect_yum_plugin.py
--rw-r--r--   0        0        0     4278 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/core_plugins/composite_collector.py
--rw-r--r--   0        0        0     5318 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/core_plugins/delta_sbom.py
--rw-r--r--   0        0        0     6885 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/core_plugins/oras_bundle.py
--rw-r--r--   0        0        0     5301 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/core_plugins/oras_registry.py
--rw-r--r--   0        0        0        0 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/core_plugins/py.typed
--rw-r--r--   0        0        0      202 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/core_plugins/report_generator/__init__.py
--rw-r--r--   0        0        0   126749 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/core_plugins/report_generator/assets/hoppr_hippo.png
--rw-r--r--   0        0        0     4577 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/core_plugins/report_generator/report_generator.py
--rw-r--r--   0        0        0    60554 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/core_plugins/report_generator/scripts/bootstrap.min.js
--rw-r--r--   0        0        0      518 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/core_plugins/report_generator/scripts/custom.js
--rw-r--r--   0        0        0   220780 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/core_plugins/report_generator/styles/bootstrap.min.css
--rw-r--r--   0        0        0     3562 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/core_plugins/report_generator/styles/custom.css
--rw-r--r--   0        0        0     4810 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/core_plugins/report_generator/templates/component_card.jinja2
--rw-r--r--   0        0        0     1230 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/core_plugins/report_generator/templates/general_summary.jinja2
--rw-r--r--   0        0        0     7246 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/core_plugins/report_generator/templates/index.jinja2
--rw-r--r--   0        0        0      458 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/exceptions.py
--rw-r--r--   0        0        0     6847 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/in_toto.py
--rw-r--r--   0        0        0     3074 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/main.py
--rw-r--r--   0        0        0     4106 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/mem_logger.py
--rw-r--r--   0        0        0     1708 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/models/__init__.py
--rw-r--r--   0        0        0     1602 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/models/__main__.py
--rw-r--r--   0        0        0     1409 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/models/base.py
--rw-r--r--   0        0        0     4001 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/models/credentials.py
--rw-r--r--   0        0        0    17452 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/models/manifest.py
--rw-r--r--   0        0        0        0 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/models/py.typed
--rw-r--r--   0        0        0     3975 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/models/transfer.py
--rw-r--r--   0        0        0     5071 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/models/types.py
--rw-r--r--   0        0        0     2335 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/net.py
--rw-r--r--   0        0        0     4323 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/oci_artifacts.py
--rw-r--r--   0        0        0     1332 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/plugin_utils.py
--rw-r--r--   0        0        0    25427 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/processor.py
--rw-r--r--   0        0        0        0 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/py.typed
--rw-r--r--   0        0        0    22579 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/resources/hoppr-hippo-large.ansi
--rw-r--r--   0        0        0    10419 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/resources/hoppr-hippo.ansi
--rw-r--r--   0        0        0     4036 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/result.py
--rw-r--r--   0        0        0     5791 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/utils.py
--rw-r--r--   0        0        0     3614 2023-04-24 21:09:54.000000 hoppr-1.8.3/pyproject.toml
--rw-r--r--   0        0        0     2686 1970-01-01 00:00:00.000000 hoppr-1.8.3/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-04-26 14:25:36.000000 hoppr-1.8.4/LICENSE
+-rw-r--r--   0        0        0     1214 2023-04-26 14:25:36.000000 hoppr-1.8.4/README.md
+-rw-r--r--   0        0        0     1035 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/__init__.py
+-rw-r--r--   0        0        0      161 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/__main__.py
+-rw-r--r--   0        0        0        0 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/base_plugins/__init__.py
+-rw-r--r--   0        0        0    10990 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/base_plugins/collector.py
+-rw-r--r--   0        0        0    10732 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/base_plugins/hoppr.py
+-rw-r--r--   0        0        0        0 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/base_plugins/py.typed
+-rw-r--r--   0        0        0        0 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/cli/__init__.py
+-rw-r--r--   0        0        0     6256 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/cli/hopctl.py
+-rw-r--r--   0        0        0      563 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/constants.py
+-rw-r--r--   0        0        0        0 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/core_plugins/__init__.py
+-rw-r--r--   0        0        0     3046 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/core_plugins/bundle_tar.py
+-rw-r--r--   0        0        0    12943 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/core_plugins/collect_apt_plugin.py
+-rw-r--r--   0        0        0    10272 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/core_plugins/collect_dnf_plugin.py
+-rw-r--r--   0        0        0     3321 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/core_plugins/collect_docker_plugin.py
+-rw-r--r--   0        0        0     4664 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/core_plugins/collect_git_plugin.py
+-rw-r--r--   0        0        0     3992 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/core_plugins/collect_helm_plugin.py
+-rw-r--r--   0        0        0     6369 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/core_plugins/collect_maven_plugin.py
+-rw-r--r--   0        0        0     7978 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/core_plugins/collect_nexus_search.py
+-rw-r--r--   0        0        0     4418 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/core_plugins/collect_pypi_plugin.py
+-rw-r--r--   0        0        0     3043 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/core_plugins/collect_raw_plugin.py
+-rw-r--r--   0        0        0     3739 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/core_plugins/collect_yum_plugin.py
+-rw-r--r--   0        0        0     4278 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/core_plugins/composite_collector.py
+-rw-r--r--   0        0        0     5673 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/core_plugins/delta_sbom.py
+-rw-r--r--   0        0        0     6885 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/core_plugins/oras_bundle.py
+-rw-r--r--   0        0        0     5301 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/core_plugins/oras_registry.py
+-rw-r--r--   0        0        0        0 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/core_plugins/py.typed
+-rw-r--r--   0        0        0      202 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/core_plugins/report_generator/__init__.py
+-rw-r--r--   0        0        0   126749 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/core_plugins/report_generator/assets/hoppr_hippo.png
+-rw-r--r--   0        0        0     4577 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/core_plugins/report_generator/report_generator.py
+-rw-r--r--   0        0        0    60554 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/core_plugins/report_generator/scripts/bootstrap.min.js
+-rw-r--r--   0        0        0      518 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/core_plugins/report_generator/scripts/custom.js
+-rw-r--r--   0        0        0   220780 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/core_plugins/report_generator/styles/bootstrap.min.css
+-rw-r--r--   0        0        0     3562 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/core_plugins/report_generator/styles/custom.css
+-rw-r--r--   0        0        0     4810 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/core_plugins/report_generator/templates/component_card.jinja2
+-rw-r--r--   0        0        0     1230 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/core_plugins/report_generator/templates/general_summary.jinja2
+-rw-r--r--   0        0        0     7246 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/core_plugins/report_generator/templates/index.jinja2
+-rw-r--r--   0        0        0      458 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/exceptions.py
+-rw-r--r--   0        0        0     6847 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/in_toto.py
+-rw-r--r--   0        0        0     3074 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/main.py
+-rw-r--r--   0        0        0     4106 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/mem_logger.py
+-rw-r--r--   0        0        0     1708 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/models/__init__.py
+-rw-r--r--   0        0        0     1602 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/models/__main__.py
+-rw-r--r--   0        0        0     1409 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/models/base.py
+-rw-r--r--   0        0        0     4001 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/models/credentials.py
+-rw-r--r--   0        0        0    17452 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/models/manifest.py
+-rw-r--r--   0        0        0        0 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/models/py.typed
+-rw-r--r--   0        0        0     3975 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/models/transfer.py
+-rw-r--r--   0        0        0     5071 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/models/types.py
+-rw-r--r--   0        0        0     2335 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/net.py
+-rw-r--r--   0        0        0     4323 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/oci_artifacts.py
+-rw-r--r--   0        0        0     1332 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/plugin_utils.py
+-rw-r--r--   0        0        0    25929 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/processor.py
+-rw-r--r--   0        0        0        0 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/py.typed
+-rw-r--r--   0        0        0    22579 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/resources/hoppr-hippo-large.ansi
+-rw-r--r--   0        0        0    10419 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/resources/hoppr-hippo.ansi
+-rw-r--r--   0        0        0     4036 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/result.py
+-rw-r--r--   0        0        0     5791 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/utils.py
+-rw-r--r--   0        0        0     3614 2023-04-26 14:25:36.000000 hoppr-1.8.4/pyproject.toml
+-rw-r--r--   0        0        0     2686 1970-01-01 00:00:00.000000 hoppr-1.8.4/PKG-INFO
```

### Comparing `hoppr-1.8.3/LICENSE` & `hoppr-1.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.3/README.md` & `hoppr-1.8.4/README.md`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.3/hoppr/__init__.py` & `hoppr-1.8.4/hoppr/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,8 +29,8 @@
     "Property",
     "PurlType",
     "Result",
     "Sbom",
     "Transfer",
 ]
 
-__version__ = "1.8.3"
+__version__ = "1.8.4"
```

### Comparing `hoppr-1.8.3/hoppr/base_plugins/collector.py` & `hoppr-1.8.4/hoppr/base_plugins/collector.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.3/hoppr/base_plugins/hoppr.py` & `hoppr-1.8.4/hoppr/base_plugins/hoppr.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.3/hoppr/cli/hopctl.py` & `hoppr-1.8.4/hoppr/cli/hopctl.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.3/hoppr/constants.py` & `hoppr-1.8.4/hoppr/constants.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.3/hoppr/core_plugins/bundle_tar.py` & `hoppr-1.8.4/hoppr/core_plugins/bundle_tar.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.3/hoppr/core_plugins/collect_apt_plugin.py` & `hoppr-1.8.4/hoppr/core_plugins/collect_apt_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.3/hoppr/core_plugins/collect_dnf_plugin.py` & `hoppr-1.8.4/hoppr/core_plugins/collect_dnf_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.3/hoppr/core_plugins/collect_docker_plugin.py` & `hoppr-1.8.4/hoppr/core_plugins/collect_docker_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.3/hoppr/core_plugins/collect_git_plugin.py` & `hoppr-1.8.4/hoppr/core_plugins/collect_git_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.3/hoppr/core_plugins/collect_helm_plugin.py` & `hoppr-1.8.4/hoppr/core_plugins/collect_helm_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.3/hoppr/core_plugins/collect_maven_plugin.py` & `hoppr-1.8.4/hoppr/core_plugins/collect_maven_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.3/hoppr/core_plugins/collect_nexus_search.py` & `hoppr-1.8.4/hoppr/core_plugins/collect_nexus_search.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.3/hoppr/core_plugins/collect_pypi_plugin.py` & `hoppr-1.8.4/hoppr/core_plugins/collect_pypi_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.3/hoppr/core_plugins/collect_raw_plugin.py` & `hoppr-1.8.4/hoppr/core_plugins/collect_raw_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.3/hoppr/core_plugins/collect_yum_plugin.py` & `hoppr-1.8.4/hoppr/core_plugins/collect_yum_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.3/hoppr/core_plugins/composite_collector.py` & `hoppr-1.8.4/hoppr/core_plugins/composite_collector.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.3/hoppr/core_plugins/delta_sbom.py` & `hoppr-1.8.4/hoppr/core_plugins/delta_sbom.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 class DeltaSbom(HopprPlugin):
     """
     Plugin to remove SBOM components that are specified by a "previous" SBOM
     """
 
     bom_access = BomAccess.FULL_ACCESS
+    products: list[str] = ["generic/_metadata_/_previous_bom.json"]
 
     def get_version(self) -> str:
         return __version__
 
     @hoppr_process
     def pre_stage_process(self):
         """
@@ -46,14 +47,20 @@
         if not Path(previous_source).exists():  # pyright: ignore[reportGeneralTypeIssues]
             return Result.fail(f"Previous source file \"{previous_source}\" not found.")
 
         self.get_logger().info(f"Creating delta/update SBOM, previous SBOM being retrieved from {previous_source}")
 
         previous_sbom = self._get_previous_bom(previous_source)  # pyright: ignore[reportGeneralTypeIssues]
 
+        target_dir = self.context.collect_root_dir / "generic" / "_metadata_"
+        target_dir.mkdir(parents=True, exist_ok=True)
+
+        with (target_dir / "_previous_bom.json").open(mode="w", encoding="utf-8") as bom_data:
+            bom_data.write(previous_sbom.json(exclude_none=True, by_alias=True, indent=2))
+
         delta_sbom = deepcopy(self.context.delivered_sbom)
         delta_sbom.components = []
 
         for new_comp in self.context.delivered_sbom.components or []:
             include_component = True
             for prev_comp in previous_sbom.components or []:
                 if DeltaSbom._component_match(new_comp, prev_comp):
@@ -82,15 +89,16 @@
         try:
             Manifest.load(Path(source))
             return Sbom.consolidated_sbom
         except (TypeError, UnicodeDecodeError):
             pass
 
         with tarfile.open(source) as tar:
-            buffer = tar.extractfile(tarfile.TarInfo(str(Path("generic") / "_metadata_" / "_consolidated_bom.json")))
+            buffer = tar.extractfile("./generic/_metadata_/_consolidated_bom.json")
+
             if buffer is None:
                 raise HopprError("Unable to extract BOM file from tar")
 
             with io.TextIOWrapper(buffer) as bom_file:
                 content: str = bom_file.read()
                 bom_dict = load_string(content)
                 if not isinstance(bom_dict, dict):
```

### Comparing `hoppr-1.8.3/hoppr/core_plugins/oras_bundle.py` & `hoppr-1.8.4/hoppr/core_plugins/oras_bundle.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.3/hoppr/core_plugins/oras_registry.py` & `hoppr-1.8.4/hoppr/core_plugins/oras_registry.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.3/hoppr/core_plugins/report_generator/assets/hoppr_hippo.png` & `hoppr-1.8.4/hoppr/core_plugins/report_generator/assets/hoppr_hippo.png`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.3/hoppr/core_plugins/report_generator/report_generator.py` & `hoppr-1.8.4/hoppr/core_plugins/report_generator/report_generator.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.3/hoppr/core_plugins/report_generator/scripts/bootstrap.min.js` & `hoppr-1.8.4/hoppr/core_plugins/report_generator/scripts/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.3/hoppr/core_plugins/report_generator/scripts/custom.js` & `hoppr-1.8.4/hoppr/core_plugins/report_generator/scripts/custom.js`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.3/hoppr/core_plugins/report_generator/styles/bootstrap.min.css` & `hoppr-1.8.4/hoppr/core_plugins/report_generator/styles/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.3/hoppr/core_plugins/report_generator/styles/custom.css` & `hoppr-1.8.4/hoppr/core_plugins/report_generator/styles/custom.css`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.3/hoppr/core_plugins/report_generator/templates/component_card.jinja2` & `hoppr-1.8.4/hoppr/core_plugins/report_generator/templates/component_card.jinja2`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.3/hoppr/core_plugins/report_generator/templates/general_summary.jinja2` & `hoppr-1.8.4/hoppr/core_plugins/report_generator/templates/general_summary.jinja2`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.3/hoppr/core_plugins/report_generator/templates/index.jinja2` & `hoppr-1.8.4/hoppr/core_plugins/report_generator/templates/index.jinja2`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.3/hoppr/in_toto.py` & `hoppr-1.8.4/hoppr/in_toto.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.3/hoppr/main.py` & `hoppr-1.8.4/hoppr/main.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.3/hoppr/mem_logger.py` & `hoppr-1.8.4/hoppr/mem_logger.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.3/hoppr/models/__init__.py` & `hoppr-1.8.4/hoppr/models/__init__.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.3/hoppr/models/__main__.py` & `hoppr-1.8.4/hoppr/models/__main__.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.3/hoppr/models/base.py` & `hoppr-1.8.4/hoppr/models/base.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.3/hoppr/models/credentials.py` & `hoppr-1.8.4/hoppr/models/credentials.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.3/hoppr/models/manifest.py` & `hoppr-1.8.4/hoppr/models/manifest.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.3/hoppr/models/transfer.py` & `hoppr-1.8.4/hoppr/models/transfer.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.3/hoppr/models/types.py` & `hoppr-1.8.4/hoppr/models/types.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.3/hoppr/net.py` & `hoppr-1.8.4/hoppr/net.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.3/hoppr/oci_artifacts.py` & `hoppr-1.8.4/hoppr/oci_artifacts.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.3/hoppr/plugin_utils.py` & `hoppr-1.8.4/hoppr/plugin_utils.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.3/hoppr/processor.py` & `hoppr-1.8.4/hoppr/processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -555,15 +555,15 @@
         result = Result.success()
 
         with tempfile.TemporaryDirectory() as collection_root, multiprocessing.Manager() as manager:
             logfile_lock = manager.RLock()
 
             self.context = HopprContext(
                 collect_root_dir=Path(collection_root).resolve(),
-                consolidated_sbom=Sbom.consolidated_sbom,
+                consolidated_sbom=deepcopy(Sbom.consolidated_sbom),
                 credential_required_services=getattr(self.credentials, "credential_required_services", None),
                 delivered_sbom=deepcopy(Sbom.consolidated_sbom),
                 log_level=self.log_level,
                 logfile_location=self.log_file,
                 logfile_lock=logfile_lock,
                 max_processes=self.transfer.max_processes or cpu_count(),
                 repositories=self.manifest.repositories,
@@ -586,14 +586,24 @@
 
             self.in_toto_links.set_collection_root(collection_root)
             self.in_toto_links.record_stage_start("_collect_metadata")
             self._collect_metadata()
             self._collect_consolidated_bom()
             self.in_toto_links.record_stage_stop("_collect_metadata")
 
+            # Reset some class variables (we should refactor to use instance variables, see issue
+            # https://gitlab.com/hoppr/hoppr/-/issues/230) so that:
+            #   1: The consolidated bom cannot be modified
+            #   2: Plug-ins may choose to load other manifests.
+            del Sbom.consolidated_sbom
+            Component.component_lookup = {}
+            Component.components = []
+            Component.properties = []
+            Manifest.loaded_manifests = {}
+
             msg = f"Beginning Hoppr Process execution, max_processes={self.context.max_processes}"
             self.logger.info(msg=msg)
             echo(message=msg)
 
             for stage_ref in self.transfer.stages:
                 msg = f" Beginning Stage {stage_ref.name} ".center(100, "=")
                 self.logger.info(msg)
```

### Comparing `hoppr-1.8.3/hoppr/resources/hoppr-hippo-large.ansi` & `hoppr-1.8.4/hoppr/resources/hoppr-hippo-large.ansi`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.3/hoppr/resources/hoppr-hippo.ansi` & `hoppr-1.8.4/hoppr/resources/hoppr-hippo.ansi`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.3/hoppr/result.py` & `hoppr-1.8.4/hoppr/result.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.3/hoppr/utils.py` & `hoppr-1.8.4/hoppr/utils.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.3/pyproject.toml` & `hoppr-1.8.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hoppr"
-version = "1.8.3"
+version = "1.8.4"
 description = "A tool for defining, verifying, and transferring software dependencies between environments."
 authors = ["LMCO Open Source <open.source@lmco.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://hoppr.dev"
 repository = "https://gitlab.com/hoppr/hoppr"
```

### Comparing `hoppr-1.8.3/PKG-INFO` & `hoppr-1.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hoppr
-Version: 1.8.3
+Version: 1.8.4
 Summary: A tool for defining, verifying, and transferring software dependencies between environments.
 Home-page: https://hoppr.dev
 License: MIT
 Keywords: packaging,reports,build dependencies,software bill of materials
 Author: LMCO Open Source
 Author-email: open.source@lmco.com
 Requires-Python: >=3.10,<4.0
```

