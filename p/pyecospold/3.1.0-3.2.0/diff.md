# Comparing `tmp/pyecospold-3.1.0.tar.gz` & `tmp/pyecospold-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyecospold-3.1.0.tar", last modified: Mon Apr 24 13:29:58 2023, max compression
+gzip compressed data, was "pyecospold-3.2.0.tar", last modified: Wed Apr 26 00:17:22 2023, max compression
```

## Comparing `pyecospold-3.1.0.tar` & `pyecospold-3.2.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:29:58.056487 pyecospold-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-04-24 13:29:46.000000 pyecospold-3.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-24 13:29:46.000000 pyecospold-3.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-04-24 13:29:58.056487 pyecospold-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-04-24 13:29:46.000000 pyecospold-3.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:29:58.052487 pyecospold-3.1.0/pyecospold/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-24 13:29:46.000000 pyecospold-3.1.0/pyecospold/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-24 13:29:46.000000 pyecospold-3.1.0/pyecospold/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-04-24 13:29:46.000000 pyecospold-3.1.0/pyecospold/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9407 2023-04-24 13:29:46.000000 pyecospold-3.1.0/pyecospold/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-04-24 13:29:46.000000 pyecospold-3.1.0/pyecospold/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    58157 2023-04-24 13:29:46.000000 pyecospold-3.1.0/pyecospold/model_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)    94861 2023-04-24 13:29:46.000000 pyecospold-3.1.0/pyecospold/model_v2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:29:58.040488 pyecospold-3.1.0/pyecospold/schemas/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:29:58.048488 pyecospold-3.1.0/pyecospold/schemas/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-04-24 13:29:46.000000 pyecospold-3.1.0/pyecospold/schemas/v1/EcoInventCategories.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-04-24 13:29:46.000000 pyecospold-3.1.0/pyecospold/schemas/v1/EcoInventCompanyCodes.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-04-24 13:29:46.000000 pyecospold-3.1.0/pyecospold/schemas/v1/EcoInventRegionalCodes.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-04-24 13:29:46.000000 pyecospold-3.1.0/pyecospold/schemas/v1/EcoInventUnits.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    23151 2023-04-24 13:29:46.000000 pyecospold-3.1.0/pyecospold/schemas/v1/EcoSpold01DataTypes.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    16759 2023-04-24 13:29:46.000000 pyecospold-3.1.0/pyecospold/schemas/v1/EcoSpold01Dataset.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    11858 2023-04-24 13:29:46.000000 pyecospold-3.1.0/pyecospold/schemas/v1/EcoSpold01ElementaryDataset.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    23965 2023-04-24 13:29:46.000000 pyecospold-3.1.0/pyecospold/schemas/v1/EcoSpold01FlowData.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    15813 2023-04-24 13:29:46.000000 pyecospold-3.1.0/pyecospold/schemas/v1/EcoSpold01ImpactDataset.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    59234 2023-04-24 13:29:46.000000 pyecospold-3.1.0/pyecospold/schemas/v1/EcoSpold01MetaInformation.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-04-24 13:29:46.000000 pyecospold-3.1.0/pyecospold/schemas/v1/XmlNamespace.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:29:58.052487 pyecospold-3.1.0/pyecospold/schemas/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-04-24 13:29:46.000000 pyecospold-3.1.0/pyecospold/schemas/v2/EcoSpold02.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    19919 2023-04-24 13:29:46.000000 pyecospold-3.1.0/pyecospold/schemas/v2/EcoSpold02Activity.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    20082 2023-04-24 13:29:46.000000 pyecospold-3.1.0/pyecospold/schemas/v2/EcoSpold02ChildActivity.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    50218 2023-04-24 13:29:46.000000 pyecospold-3.1.0/pyecospold/schemas/v2/EcoSpold02ChildDataTypes.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    52466 2023-04-24 13:29:46.000000 pyecospold-3.1.0/pyecospold/schemas/v2/EcoSpold02ChildFlowData.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    70861 2023-04-24 13:29:46.000000 pyecospold-3.1.0/pyecospold/schemas/v2/EcoSpold02ChildMetaInformation.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    49965 2023-04-24 13:29:46.000000 pyecospold-3.1.0/pyecospold/schemas/v2/EcoSpold02DataTypes.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    52230 2023-04-24 13:29:46.000000 pyecospold-3.1.0/pyecospold/schemas/v2/EcoSpold02FlowData.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    70813 2023-04-24 13:29:46.000000 pyecospold-3.1.0/pyecospold/schemas/v2/EcoSpold02MetaInformation.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-04-24 13:29:46.000000 pyecospold-3.1.0/pyecospold/schemas/v2/XmlNamespace.xsd
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-24 13:29:46.000000 pyecospold-3.1.0/pyecospold/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:29:58.056487 pyecospold-3.1.0/pyecospold.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-04-24 13:29:58.000000 pyecospold-3.1.0/pyecospold.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-04-24 13:29:58.000000 pyecospold-3.1.0/pyecospold.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 13:29:58.000000 pyecospold-3.1.0/pyecospold.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 13:29:57.000000 pyecospold-3.1.0/pyecospold.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-24 13:29:58.000000 pyecospold-3.1.0/pyecospold.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-24 13:29:58.000000 pyecospold-3.1.0/pyecospold.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-24 13:29:46.000000 pyecospold-3.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-04-24 13:29:58.056487 pyecospold-3.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:29:58.056487 pyecospold-3.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-24 13:29:46.000000 pyecospold-3.1.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-04-24 13:29:46.000000 pyecospold-3.1.0/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-24 13:29:46.000000 pyecospold-3.1.0/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18094 2023-04-24 13:29:46.000000 pyecospold-3.1.0/tests/test_model_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)    30087 2023-04-24 13:29:46.000000 pyecospold-3.1.0/tests/test_model_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 00:17:22.283358 pyecospold-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-04-26 00:17:13.000000 pyecospold-3.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-26 00:17:13.000000 pyecospold-3.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-04-26 00:17:22.283358 pyecospold-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-04-26 00:17:13.000000 pyecospold-3.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 00:17:22.279358 pyecospold-3.2.0/pyecospold/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-26 00:17:13.000000 pyecospold-3.2.0/pyecospold/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-26 00:17:13.000000 pyecospold-3.2.0/pyecospold/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-04-26 00:17:13.000000 pyecospold-3.2.0/pyecospold/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9407 2023-04-26 00:17:13.000000 pyecospold-3.2.0/pyecospold/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-04-26 00:17:13.000000 pyecospold-3.2.0/pyecospold/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58157 2023-04-26 00:17:13.000000 pyecospold-3.2.0/pyecospold/model_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    96181 2023-04-26 00:17:13.000000 pyecospold-3.2.0/pyecospold/model_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 00:17:22.267358 pyecospold-3.2.0/pyecospold/schemas/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 00:17:22.275358 pyecospold-3.2.0/pyecospold/schemas/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-04-26 00:17:13.000000 pyecospold-3.2.0/pyecospold/schemas/v1/EcoInventCategories.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-04-26 00:17:13.000000 pyecospold-3.2.0/pyecospold/schemas/v1/EcoInventCompanyCodes.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-04-26 00:17:13.000000 pyecospold-3.2.0/pyecospold/schemas/v1/EcoInventRegionalCodes.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-04-26 00:17:13.000000 pyecospold-3.2.0/pyecospold/schemas/v1/EcoInventUnits.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    23151 2023-04-26 00:17:13.000000 pyecospold-3.2.0/pyecospold/schemas/v1/EcoSpold01DataTypes.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    16759 2023-04-26 00:17:13.000000 pyecospold-3.2.0/pyecospold/schemas/v1/EcoSpold01Dataset.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    11858 2023-04-26 00:17:13.000000 pyecospold-3.2.0/pyecospold/schemas/v1/EcoSpold01ElementaryDataset.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    23965 2023-04-26 00:17:13.000000 pyecospold-3.2.0/pyecospold/schemas/v1/EcoSpold01FlowData.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    15813 2023-04-26 00:17:13.000000 pyecospold-3.2.0/pyecospold/schemas/v1/EcoSpold01ImpactDataset.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    59234 2023-04-26 00:17:13.000000 pyecospold-3.2.0/pyecospold/schemas/v1/EcoSpold01MetaInformation.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-04-26 00:17:13.000000 pyecospold-3.2.0/pyecospold/schemas/v1/XmlNamespace.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 00:17:22.279358 pyecospold-3.2.0/pyecospold/schemas/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-04-26 00:17:13.000000 pyecospold-3.2.0/pyecospold/schemas/v2/EcoSpold02.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    19919 2023-04-26 00:17:13.000000 pyecospold-3.2.0/pyecospold/schemas/v2/EcoSpold02Activity.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    20082 2023-04-26 00:17:13.000000 pyecospold-3.2.0/pyecospold/schemas/v2/EcoSpold02ChildActivity.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    50218 2023-04-26 00:17:13.000000 pyecospold-3.2.0/pyecospold/schemas/v2/EcoSpold02ChildDataTypes.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    52466 2023-04-26 00:17:13.000000 pyecospold-3.2.0/pyecospold/schemas/v2/EcoSpold02ChildFlowData.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    70861 2023-04-26 00:17:13.000000 pyecospold-3.2.0/pyecospold/schemas/v2/EcoSpold02ChildMetaInformation.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    49965 2023-04-26 00:17:13.000000 pyecospold-3.2.0/pyecospold/schemas/v2/EcoSpold02DataTypes.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    52230 2023-04-26 00:17:13.000000 pyecospold-3.2.0/pyecospold/schemas/v2/EcoSpold02FlowData.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    70813 2023-04-26 00:17:13.000000 pyecospold-3.2.0/pyecospold/schemas/v2/EcoSpold02MetaInformation.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-04-26 00:17:13.000000 pyecospold-3.2.0/pyecospold/schemas/v2/XmlNamespace.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-26 00:17:13.000000 pyecospold-3.2.0/pyecospold/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 00:17:22.279358 pyecospold-3.2.0/pyecospold.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-04-26 00:17:22.000000 pyecospold-3.2.0/pyecospold.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-04-26 00:17:22.000000 pyecospold-3.2.0/pyecospold.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 00:17:22.000000 pyecospold-3.2.0/pyecospold.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 00:17:22.000000 pyecospold-3.2.0/pyecospold.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-26 00:17:22.000000 pyecospold-3.2.0/pyecospold.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-26 00:17:22.000000 pyecospold-3.2.0/pyecospold.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-26 00:17:13.000000 pyecospold-3.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-04-26 00:17:22.283358 pyecospold-3.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 00:17:22.283358 pyecospold-3.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-26 00:17:13.000000 pyecospold-3.2.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-04-26 00:17:13.000000 pyecospold-3.2.0/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-26 00:17:13.000000 pyecospold-3.2.0/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18094 2023-04-26 00:17:13.000000 pyecospold-3.2.0/tests/test_model_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27945 2023-04-26 00:17:13.000000 pyecospold-3.2.0/tests/test_model_v2.py
```

### Comparing `pyecospold-3.1.0/LICENSE` & `pyecospold-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyecospold-3.1.0/PKG-INFO` & `pyecospold-3.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyecospold
-Version: 3.1.0
+Version: 3.2.0
 Summary: A Python package that converts ecospold XML formats to their Python equivalents and export the same data back to XML.
 Home-page: https://github.com/sami-m-g/pyecospold
 Author: Mina Sami
 Author-email: <sami.mg@outlook.com>
 Maintainer: Mina Sami
 Maintainer-email: <sami.mg@outlook.com>
 License: BSD license
```

### Comparing `pyecospold-3.1.0/README.md` & `pyecospold-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pyecospold-3.1.0/pyecospold/config.py` & `pyecospold-3.2.0/pyecospold/config.py`

 * *Files identical despite different names*

### Comparing `pyecospold-3.1.0/pyecospold/core.py` & `pyecospold-3.2.0/pyecospold/core.py`

 * *Files identical despite different names*

### Comparing `pyecospold-3.1.0/pyecospold/helpers.py` & `pyecospold-3.2.0/pyecospold/helpers.py`

 * *Files identical despite different names*

### Comparing `pyecospold-3.1.0/pyecospold/model_v1.py` & `pyecospold-3.2.0/pyecospold/model_v1.py`

 * *Files identical despite different names*

### Comparing `pyecospold-3.1.0/pyecospold/model_v2.py` & `pyecospold-3.2.0/pyecospold/model_v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1103,21 +1103,21 @@
     OUTPUT_GROUP_MAP: Dict[int, str] = {
         0: "ReferenceProduct",
         2: "By-product",
         3: "MaterialForTreatment",
         5: "Stock Additions",
     }
 
-    inputGroup = create_element_text_v2("inputGroup", int)
+    _inputGroup = create_element_text_v2("inputGroup", int)
     """int: Indicates the kind of input flow. The codes are: 1=Materials/Fuels,
     2=Electricity/Heat, 3=Services, 5=From Technosphere (unspecified). For each
     exchange only an inputGroup or outputGroup shall exist. This indicates the
     direction of the flow."""
 
-    outputGroup = create_element_text_v2("outputGroup", int)
+    _outputGroup = create_element_text_v2("outputGroup", int)
     """int: Indicates the kind of output flow. The codes are: 0=ReferenceProduct,
     2=By-product, 3=MaterialForTreatment, 5=Stock Additions. For each exchange only
     an inputGroup or outputGroup shall exist. This indicates the direction of the
     flow."""
 
     productionVolumeComments = create_attribute_list_v2("productionVolumeComments", str)
     """lits[str]: A general comment can be made on the data source, assumptions and
@@ -1192,25 +1192,45 @@
     )
     """str: Indicates the first author by surname and abbreviated name
     (e.g., Einstein A.). In case of measurement on site, oral communication, personal
     written communication and questionnaries ('sourceType'=4, 5, 6, 7) the name of the
     communicating person is"""
 
     @property
-    def inputGroupStr(self) -> str:
-        """String representation for inputGroup. See inputGroup for explanations.
+    def _inputGroupStr(self) -> str:
+        """String representation for _inputGroup. See _inputGroup for explanations.
         1=Materials/Fuels, 2=Electricity/Heat, 3=Services, 5=From Technosphere
         (unspecified)."""
-        return self.INPUT_GROUP_MAP[self.inputGroup]
+        return self.INPUT_GROUP_MAP[self._inputGroup]
 
     @property
-    def outputGroupStr(self) -> str:
-        """String representation for outputGroup. See outputGroup for explanations.
+    def _outputGroupStr(self) -> str:
+        """String representation for _outputGroup. See _outputGroup for explanations.
         0=ReferenceProduct, 2=By-product, 3=MaterialForTreatment, 5=Stock Additions."""
-        return self.OUTPUT_GROUP_MAP[self.outputGroup]
+        return self.OUTPUT_GROUP_MAP[self._outputGroup]
+
+    @property
+    def group(self) -> List[int]:
+        """Choice between _inputGroup and _outputGroup. Check their documentation
+        for more information."""
+        return (
+            self._inputGroup
+            if self.find("inputGroup", self.nsmap) is not None
+            else self._outputGroup
+        )
+
+    @property
+    def groupStr(self) -> List[str]:
+        """Choice between _inputGroupStr and _outputGroupStr. Check their
+        documentation for more information."""
+        return (
+            self._inputGroupStr
+            if self.find("inputGroup", self.nsmap) is not None
+            else self._outputGroupStr
+        )
 
     @property
     def productionVolumeUncertainties(self) -> List["Uncertainty"]:
         """Uncertainty information in the form of distribution functions and their
         parameters and/or pedigree data."""
         return get_element_list(self, "productionVolumeUncertainty")
 
@@ -1220,21 +1240,21 @@
         return get_element_list(self, "classification")
 
 
 class ElementaryExchange(CustomExchange):
     """Comprises elementary inputs and outputs (exchanges with the environment)
     for the activity."""
 
-    inputGroup = create_element_text_v2("inputGroup", int)
+    _inputGroup = create_element_text_v2("inputGroup", int)
     """int: Indicates the kind of input flow. The codes are: 4=From Environment
     For each exchange only an inputGroup or outputGroup shall exist. This
     indicates the direction of the flow. This field is the equivalent of field
     1500 with a different set of valid values."""
 
-    outputGroup = create_element_text_v2("outputGroup", int)
+    _outputGroup = create_element_text_v2("outputGroup", int)
     """int: Indicates the kind of output flow. The codes are: 4=ToEnvironment
     For each exchange only an inputGroup or outputGroup shall exist. This
     indicates the direction of the flow. This field is the equivalent of field
     1510 with a different set of valid values."""
 
     elementaryExchangeId = create_attribute_v2("elementaryExchangeId", str)
     """str: Reference to the master data entry for this elementary exchange"""
@@ -1253,25 +1273,45 @@
     def compartment(self) -> "Compartment":
         """Name of the compartment and subcompartment of the exchange.
         The xml document referenced by validCompartments contains definitions
         of valid compartment/subcompartment pairs for a given language."""
         return get_element(self, "compartment")
 
     @property
-    def inputGroupStr(self) -> str:
-        """String representation for inputGroup. See inputGroup for
+    def _inputGroupStr(self) -> str:
+        """String representation for _inputGroup. See _inputGroup for
         explanations. 4=FromEnvironment"""
         return "FromEnvironment"
 
     @property
-    def outputGroupStr(self) -> str:
-        """String representation for outputGroup. See outputGroup for
+    def _outputGroupStr(self) -> str:
+        """String representation for _outputGroup. See _outputGroup for
         explanations. 4=ToEnvironment"""
         return "ToEnvironment"
 
+    @property
+    def group(self) -> List[int]:
+        """Choice between _inputGroup and _outputGroup. Check their documentation
+        for more information."""
+        return (
+            self._inputGroup
+            if self.find("inputGroup", self.nsmap) is not None
+            else self._outputGroup
+        )
+
+    @property
+    def groupStr(self) -> List[str]:
+        """Choice between _inputGroupStr and _outputGroupStr. Check their
+        documentation for more information."""
+        return (
+            self._inputGroupStr
+            if self.find("inputGroup", self.nsmap) is not None
+            else self._outputGroupStr
+        )
+
 
 class Parameter(etree.ElementBase):
     """Comprises all parameters of the activity."""
 
     names = create_attribute_list_v2("name", str)
     """list[str]: Descriptive name of the parameter."""
```

### Comparing `pyecospold-3.1.0/pyecospold/schemas/v1/EcoInventCategories.xsd` & `pyecospold-3.2.0/pyecospold/schemas/v1/EcoInventCategories.xsd`

 * *Files identical despite different names*

### Comparing `pyecospold-3.1.0/pyecospold/schemas/v1/EcoInventCompanyCodes.xsd` & `pyecospold-3.2.0/pyecospold/schemas/v1/EcoInventCompanyCodes.xsd`

 * *Files identical despite different names*

### Comparing `pyecospold-3.1.0/pyecospold/schemas/v1/EcoInventRegionalCodes.xsd` & `pyecospold-3.2.0/pyecospold/schemas/v1/EcoInventRegionalCodes.xsd`

 * *Files identical despite different names*

### Comparing `pyecospold-3.1.0/pyecospold/schemas/v1/EcoInventUnits.xsd` & `pyecospold-3.2.0/pyecospold/schemas/v1/EcoInventUnits.xsd`

 * *Files identical despite different names*

### Comparing `pyecospold-3.1.0/pyecospold/schemas/v1/EcoSpold01DataTypes.xsd` & `pyecospold-3.2.0/pyecospold/schemas/v1/EcoSpold01DataTypes.xsd`

 * *Files identical despite different names*

### Comparing `pyecospold-3.1.0/pyecospold/schemas/v1/EcoSpold01Dataset.xsd` & `pyecospold-3.2.0/pyecospold/schemas/v1/EcoSpold01Dataset.xsd`

 * *Files identical despite different names*

### Comparing `pyecospold-3.1.0/pyecospold/schemas/v1/EcoSpold01ElementaryDataset.xsd` & `pyecospold-3.2.0/pyecospold/schemas/v1/EcoSpold01ElementaryDataset.xsd`

 * *Files identical despite different names*

### Comparing `pyecospold-3.1.0/pyecospold/schemas/v1/EcoSpold01FlowData.xsd` & `pyecospold-3.2.0/pyecospold/schemas/v1/EcoSpold01FlowData.xsd`

 * *Files identical despite different names*

### Comparing `pyecospold-3.1.0/pyecospold/schemas/v1/EcoSpold01ImpactDataset.xsd` & `pyecospold-3.2.0/pyecospold/schemas/v1/EcoSpold01ImpactDataset.xsd`

 * *Files identical despite different names*

### Comparing `pyecospold-3.1.0/pyecospold/schemas/v1/EcoSpold01MetaInformation.xsd` & `pyecospold-3.2.0/pyecospold/schemas/v1/EcoSpold01MetaInformation.xsd`

 * *Files identical despite different names*

### Comparing `pyecospold-3.1.0/pyecospold/schemas/v1/XmlNamespace.xsd` & `pyecospold-3.2.0/pyecospold/schemas/v1/XmlNamespace.xsd`

 * *Files identical despite different names*

### Comparing `pyecospold-3.1.0/pyecospold/schemas/v2/EcoSpold02.xsd` & `pyecospold-3.2.0/pyecospold/schemas/v2/EcoSpold02.xsd`

 * *Files identical despite different names*

### Comparing `pyecospold-3.1.0/pyecospold/schemas/v2/EcoSpold02Activity.xsd` & `pyecospold-3.2.0/pyecospold/schemas/v2/EcoSpold02Activity.xsd`

 * *Files identical despite different names*

### Comparing `pyecospold-3.1.0/pyecospold/schemas/v2/EcoSpold02ChildActivity.xsd` & `pyecospold-3.2.0/pyecospold/schemas/v2/EcoSpold02ChildActivity.xsd`

 * *Files identical despite different names*

### Comparing `pyecospold-3.1.0/pyecospold/schemas/v2/EcoSpold02ChildDataTypes.xsd` & `pyecospold-3.2.0/pyecospold/schemas/v2/EcoSpold02ChildDataTypes.xsd`

 * *Files identical despite different names*

### Comparing `pyecospold-3.1.0/pyecospold/schemas/v2/EcoSpold02ChildFlowData.xsd` & `pyecospold-3.2.0/pyecospold/schemas/v2/EcoSpold02ChildFlowData.xsd`

 * *Files identical despite different names*

### Comparing `pyecospold-3.1.0/pyecospold/schemas/v2/EcoSpold02ChildMetaInformation.xsd` & `pyecospold-3.2.0/pyecospold/schemas/v2/EcoSpold02ChildMetaInformation.xsd`

 * *Files identical despite different names*

### Comparing `pyecospold-3.1.0/pyecospold/schemas/v2/EcoSpold02DataTypes.xsd` & `pyecospold-3.2.0/pyecospold/schemas/v2/EcoSpold02DataTypes.xsd`

 * *Files identical despite different names*

### Comparing `pyecospold-3.1.0/pyecospold/schemas/v2/EcoSpold02FlowData.xsd` & `pyecospold-3.2.0/pyecospold/schemas/v2/EcoSpold02FlowData.xsd`

 * *Files identical despite different names*

### Comparing `pyecospold-3.1.0/pyecospold/schemas/v2/EcoSpold02MetaInformation.xsd` & `pyecospold-3.2.0/pyecospold/schemas/v2/EcoSpold02MetaInformation.xsd`

 * *Files identical despite different names*

### Comparing `pyecospold-3.1.0/pyecospold/schemas/v2/XmlNamespace.xsd` & `pyecospold-3.2.0/pyecospold/schemas/v2/XmlNamespace.xsd`

 * *Files identical despite different names*

### Comparing `pyecospold-3.1.0/pyecospold/version.py` & `pyecospold-3.2.0/pyecospold/version.py`

 * *Files identical despite different names*

### Comparing `pyecospold-3.1.0/pyecospold.egg-info/PKG-INFO` & `pyecospold-3.2.0/pyecospold.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyecospold
-Version: 3.1.0
+Version: 3.2.0
 Summary: A Python package that converts ecospold XML formats to their Python equivalents and export the same data back to XML.
 Home-page: https://github.com/sami-m-g/pyecospold
 Author: Mina Sami
 Author-email: <sami.mg@outlook.com>
 Maintainer: Mina Sami
 Maintainer-email: <sami.mg@outlook.com>
 License: BSD license
```

### Comparing `pyecospold-3.1.0/pyecospold.egg-info/SOURCES.txt` & `pyecospold-3.2.0/pyecospold.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyecospold-3.1.0/setup.cfg` & `pyecospold-3.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyecospold-3.1.0/tests/test_config.py` & `pyecospold-3.2.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `pyecospold-3.1.0/tests/test_core.py` & `pyecospold-3.2.0/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `pyecospold-3.1.0/tests/test_helpers.py` & `pyecospold-3.2.0/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `pyecospold-3.1.0/tests/test_model_v1.py` & `pyecospold-3.2.0/tests/test_model_v1.py`

 * *Files identical despite different names*

### Comparing `pyecospold-3.1.0/tests/test_model_v2.py` & `pyecospold-3.2.0/tests/test_model_v2.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,14 @@
     FileAttributes,
     FlowData,
     Geography,
     IntermediateExchange,
     MacroEconomicScenario,
     ModellingAndValidation,
     Parameter,
-    Property,
     Representativeness,
     Technology,
     TextAndImage,
     TimePeriod,
     Uncertainty,
 )
 
@@ -292,103 +291,61 @@
     )
     assert macroEconomicScenario.names == names
     assert macroEconomicScenario.comments == comments
 
 
 def test_parse_file_v2_intermediate_exchange(eco_spold: EcoSpold) -> None:
     """It parses attributes correctly."""
-    exchangeID = "2592e17c-df72-4446-91f5-fa1f1e0e8042"
-    unitId = "487df68b-4994-4027-8fdc-a4dc298257b7"
-    unitContextId = ""
-    variableName = "water_deionised_input"
-    casNumber = "007732-18-5"
-    amount = 0.6
-    isCalculatedAmount = False
-    mathematicalRelation = ""
-    sourceId = ""
-    sourceIdOverwrittenByChild = False
-    sourceContextId = ""
-    sourceYear = ""
-    sourceFirstAuthor = ""
-    pageNumbers = ""
-    specificAllocationPropertyId = ""
-    specificAllocationPropertyIdOverwrittenByChild = False
-    specificAllocationPropertyContextId = ""
-    names = ["water, deionised, from tap water, at user"]
-    unitNames = ["kg"]
-    comments = ["EcoSpold01Location=CH", "Literature value."]
-    synonyms = []
-    tags = []
-    intermediateExchangeId = "360e2eb0-f81c-4e4b-ba6b-c7a690f31275"
-    activityLinkId = "cd1f547f-577f-4e1b-bd23-fb73d53497eb"
-    transferCoefficientsLen = 0
+    exchangeID = "336dd4ef-cece-4c49-b412-5fe565ec8b8f"
+    unitId = "980b811e-3905-4797-82a5-173f5568bc7e"
+    amount = 0
+    productionVolumeAmount = 0
+    names = ["heat, district or industrial, natural gas"]
+    unitNames = ["MJ"]
+    comments = ["Literature value."]
+    intermediateExchangeId = "1125e767-7b5d-442e-81d6-9b0d3e1919ac"
+    group = 5
+    groupStr = "From Technosphere (unspecified)"
+    outGroup = 0
+    outGroupStr = "ReferenceProduct"
     classificationsLen = 1
     productionVolumeUncertaintiesLen = 0
-    intermediateExchange = eco_spold.activityDataset.flowData.intermediateExchanges[0]
+    intermediateExchanges = eco_spold.activityDataset.flowData.intermediateExchanges
+    intermediateExchange = intermediateExchanges[1]
+    intermediateExchangeOut = intermediateExchanges[6]
 
     assert intermediateExchange.id == exchangeID
     assert intermediateExchange.unitId == unitId
-    assert intermediateExchange.unitContextId == unitContextId
-    assert intermediateExchange.variableName == variableName
-    assert intermediateExchange.casNumber == casNumber
     assert intermediateExchange.amount == amount
-    assert intermediateExchange.isCalculatedAmount == isCalculatedAmount
-    assert intermediateExchange.mathematicalRelation == mathematicalRelation
-    assert intermediateExchange.sourceId == sourceId
-    assert intermediateExchange.sourceIdOverwrittenByChild == sourceIdOverwrittenByChild
-    assert intermediateExchange.sourceContextId == sourceContextId
-    assert intermediateExchange.sourceYear == sourceYear
-    assert intermediateExchange.sourceFirstAuthor == sourceFirstAuthor
-    assert intermediateExchange.pageNumbers == pageNumbers
-    assert (
-        intermediateExchange.specificAllocationPropertyId
-        == specificAllocationPropertyId
-    )
-    assert (
-        intermediateExchange.specificAllocationPropertyIdOverwrittenByChild
-        == specificAllocationPropertyIdOverwrittenByChild
-    )
-    assert (
-        intermediateExchange.specificAllocationPropertyContextId
-        == specificAllocationPropertyContextId
-    )
+    assert intermediateExchange.productionVolumeAmount == productionVolumeAmount
     assert intermediateExchange.intermediateExchangeId == intermediateExchangeId
-    assert intermediateExchange.activityLinkId == activityLinkId
+    assert intermediateExchange.group == group
+    assert intermediateExchange.groupStr == groupStr
     assert intermediateExchange.names == names
     assert intermediateExchange.unitNames == unitNames
     assert intermediateExchange.comments == comments
-    assert intermediateExchange.synonyms == synonyms
-    assert intermediateExchange.tags == tags
+
+    assert intermediateExchangeOut.group == outGroup
+    assert intermediateExchangeOut.groupStr == outGroupStr
 
     assert isinstance(intermediateExchange.uncertainties[0], Uncertainty)
-    assert isinstance(intermediateExchange.properties[0], Property)
-    assert len(intermediateExchange.transferCoefficients) == transferCoefficientsLen
     assert len(intermediateExchange.classifications) == classificationsLen
     assert (
         len(intermediateExchange.productionVolumeUncertainties)
         == productionVolumeUncertaintiesLen
     )
 
 
 def test_parse_file_v2_elementary_exchange(eco_spold: EcoSpold) -> None:
     """It parses attributes correctly."""
     exchangeID = "719770d0-4b1e-4c44-bd9e-72c4687a6ee0"
     unitId = "487df68b-4994-4027-8fdc-a4dc298257b7"
-    unitContextId = ""
-    variableName = ""
-    casNumber = ""
     amount = 0.0011
     isCalculatedAmount = False
-    mathematicalRelation = ""
-    sourceId = ""
     sourceIdOverwrittenByChild = False
-    sourceContextId = ""
-    sourceYear = ""
-    sourceFirstAuthor = ""
-    pageNumbers = ""
     specificAllocationPropertyId = ""
     specificAllocationPropertyIdOverwrittenByChild = False
     specificAllocationPropertyContextId = ""
     elementaryExchangeId = "70d467b6-115e-43c5-add2-441de9411348"
     names = ["BOD5, Biological Oxygen Demand"]
     unitNames = ["kg"]
     comments = [
@@ -396,37 +353,31 @@
         + "the treated waste water assuming a carbon conversion of 96% for COD. "
         + "The worst case scenario, BOD=COD, was used. "
         + "It is assumed that the manufacturing plant is located in an "
         + "urban/industrial area and consequently the emissions are categorised as "
         + "emanating in a high population density area. The emissions into water are "
         + "assumed to be emitted into rivers."
     ]
-    outputGroup = 4
-    outputGroupStr = "ToEnvironment"
-    inputGroupStr = "FromEnvironment"
+    group = 4
+    groupStr = "ToEnvironment"
+    inGroup = 4
+    inGroupStr = "FromEnvironment"
     synonyms = []
     tags = []
     propertiesLen = 0
     transferCoefficientsLen = 0
-    elementaryExchange = eco_spold.activityDataset.flowData.elementaryExchanges[0]
+    elementaryExchanges = eco_spold.activityDataset.flowData.elementaryExchanges
+    elementaryExchange = elementaryExchanges[0]
+    elementaryExchangeIn = elementaryExchanges[1]
 
     assert elementaryExchange.id == exchangeID
     assert elementaryExchange.unitId == unitId
-    assert elementaryExchange.unitContextId == unitContextId
-    assert elementaryExchange.variableName == variableName
-    assert elementaryExchange.casNumber == casNumber
     assert elementaryExchange.amount == amount
     assert elementaryExchange.isCalculatedAmount == isCalculatedAmount
-    assert elementaryExchange.mathematicalRelation == mathematicalRelation
-    assert elementaryExchange.sourceId == sourceId
     assert elementaryExchange.sourceIdOverwrittenByChild == sourceIdOverwrittenByChild
-    assert elementaryExchange.sourceContextId == sourceContextId
-    assert elementaryExchange.sourceYear == sourceYear
-    assert elementaryExchange.sourceFirstAuthor == sourceFirstAuthor
-    assert elementaryExchange.pageNumbers == pageNumbers
     assert (
         elementaryExchange.specificAllocationPropertyId == specificAllocationPropertyId
     )
     assert (
         elementaryExchange.specificAllocationPropertyIdOverwrittenByChild
         == specificAllocationPropertyIdOverwrittenByChild
     )
@@ -434,20 +385,22 @@
         elementaryExchange.specificAllocationPropertyContextId
         == specificAllocationPropertyContextId
     )
     assert elementaryExchange.elementaryExchangeId == elementaryExchangeId
     assert elementaryExchange.names == names
     assert elementaryExchange.unitNames == unitNames
     assert elementaryExchange.comments == comments
-    assert elementaryExchange.outputGroup == outputGroup
-    assert elementaryExchange.outputGroupStr == outputGroupStr
-    assert elementaryExchange.inputGroupStr == inputGroupStr
+    assert elementaryExchange.group == group
+    assert elementaryExchange.groupStr == groupStr
     assert elementaryExchange.synonyms == synonyms
     assert elementaryExchange.tags == tags
 
+    assert elementaryExchangeIn.group == inGroup
+    assert elementaryExchangeIn.groupStr == inGroupStr
+
     assert isinstance(elementaryExchange.uncertainties[0], Uncertainty)
     assert len(elementaryExchange.properties) == propertiesLen
     assert len(elementaryExchange.transferCoefficients) == transferCoefficientsLen
 
 
 def test_parse_file_v2_uncertainty(eco_spold: EcoSpold) -> None:
     """It parses attributes correctly."""
```

