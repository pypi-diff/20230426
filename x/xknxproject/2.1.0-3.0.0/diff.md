# Comparing `tmp/xknxproject-2.1.0.tar.gz` & `tmp/xknxproject-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xknxproject-2.1.0.tar", last modified: Fri Oct 14 19:23:39 2022, max compression
+gzip compressed data, was "xknxproject-3.0.0.tar", last modified: Tue Apr 25 21:17:44 2023, max compression
```

## Comparing `xknxproject-2.1.0.tar` & `xknxproject-3.0.0.tar`

### file list

```diff
@@ -1,45 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 19:23:39.068391 xknxproject-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)    18092 2022-10-14 19:23:27.000000 xknxproject-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-10-14 19:23:27.000000 xknxproject-2.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2607 2022-10-14 19:23:39.068391 xknxproject-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1996 2022-10-14 19:23:27.000000 xknxproject-2.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     2055 2022-10-14 19:23:27.000000 xknxproject-2.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      199 2022-10-14 19:23:39.068391 xknxproject-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1420 2022-10-14 19:23:27.000000 xknxproject-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 19:23:39.064391 xknxproject-2.1.0/test/
--rw-r--r--   0 runner    (1001) docker     (121)      397 2022-10-14 19:23:27.000000 xknxproject-2.1.0/test/test_knxproj.py
--rw-r--r--   0 runner    (1001) docker     (121)      702 2022-10-14 19:23:27.000000 xknxproject-2.1.0/test/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 19:23:39.064391 xknxproject-2.1.0/xknxproject/
--rw-r--r--   0 runner    (1001) docker     (121)      143 2022-10-14 19:23:27.000000 xknxproject-2.1.0/xknxproject/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-10-14 19:23:27.000000 xknxproject-2.1.0/xknxproject/__version__.py
--rw-r--r--   0 runner    (1001) docker     (121)      308 2022-10-14 19:23:27.000000 xknxproject-2.1.0/xknxproject/const.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 19:23:39.064391 xknxproject-2.1.0/xknxproject/exceptions/
--rw-r--r--   0 runner    (1001) docker     (121)      259 2022-10-14 19:23:27.000000 xknxproject-2.1.0/xknxproject/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      333 2022-10-14 19:23:27.000000 xknxproject-2.1.0/xknxproject/exceptions/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 19:23:39.068391 xknxproject-2.1.0/xknxproject/loader/
--rw-r--r--   0 runner    (1001) docker     (121)      356 2022-10-14 19:23:27.000000 xknxproject-2.1.0/xknxproject/loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5256 2022-10-14 19:23:27.000000 xknxproject-2.1.0/xknxproject/loader/application_program_loader.py
--rw-r--r--   0 runner    (1001) docker     (121)     2283 2022-10-14 19:23:27.000000 xknxproject-2.1.0/xknxproject/loader/hardware_loader.py
--rw-r--r--   0 runner    (1001) docker     (121)     1029 2022-10-14 19:23:27.000000 xknxproject-2.1.0/xknxproject/loader/manufacturer_loader.py
--rw-r--r--   0 runner    (1001) docker     (121)     8587 2022-10-14 19:23:27.000000 xknxproject-2.1.0/xknxproject/loader/project_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 19:23:39.068391 xknxproject-2.1.0/xknxproject/models/
--rw-r--r--   0 runner    (1001) docker     (121)      739 2022-10-14 19:23:27.000000 xknxproject-2.1.0/xknxproject/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1631 2022-10-14 19:23:27.000000 xknxproject-2.1.0/xknxproject/models/knxproject.py
--rw-r--r--   0 runner    (1001) docker     (121)     8911 2022-10-14 19:23:27.000000 xknxproject-2.1.0/xknxproject/models/models.py
--rw-r--r--   0 runner    (1001) docker     (121)      631 2022-10-14 19:23:27.000000 xknxproject-2.1.0/xknxproject/models/static.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-14 19:23:27.000000 xknxproject-2.1.0/xknxproject/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)      970 2022-10-14 19:23:27.000000 xknxproject-2.1.0/xknxproject/util.py
--rw-r--r--   0 runner    (1001) docker     (121)      912 2022-10-14 19:23:27.000000 xknxproject-2.1.0/xknxproject/xknxproj.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 19:23:39.068391 xknxproject-2.1.0/xknxproject/xml/
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-10-14 19:23:27.000000 xknxproject-2.1.0/xknxproject/xml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6877 2022-10-14 19:23:27.000000 xknxproject-2.1.0/xknxproject/xml/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 19:23:39.068391 xknxproject-2.1.0/xknxproject/zip/
--rw-r--r--   0 runner    (1001) docker     (121)      129 2022-10-14 19:23:27.000000 xknxproject-2.1.0/xknxproject/zip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4123 2022-10-14 19:23:27.000000 xknxproject-2.1.0/xknxproject/zip/extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 19:23:39.064391 xknxproject-2.1.0/xknxproject.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2607 2022-10-14 19:23:38.000000 xknxproject-2.1.0/xknxproject.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      949 2022-10-14 19:23:39.000000 xknxproject-2.1.0/xknxproject.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-14 19:23:38.000000 xknxproject-2.1.0/xknxproject.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-14 19:23:38.000000 xknxproject-2.1.0/xknxproject.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-10-14 19:23:38.000000 xknxproject-2.1.0/xknxproject.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-10-14 19:23:38.000000 xknxproject-2.1.0/xknxproject.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:17:44.387534 xknxproject-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-04-25 21:17:26.000000 xknxproject-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-25 21:17:26.000000 xknxproject-3.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    23615 2023-04-25 21:17:44.387534 xknxproject-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-04-25 21:17:26.000000 xknxproject-3.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-04-25 21:17:26.000000 xknxproject-3.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-25 21:17:44.387534 xknxproject-3.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:17:44.383534 xknxproject-3.0.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-25 21:17:26.000000 xknxproject-3.0.0/test/test_knxproj.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-25 21:17:26.000000 xknxproject-3.0.0/test/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:17:44.383534 xknxproject-3.0.0/xknxproject/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-25 21:17:26.000000 xknxproject-3.0.0/xknxproject/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-25 21:17:26.000000 xknxproject-3.0.0/xknxproject/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-25 21:17:26.000000 xknxproject-3.0.0/xknxproject/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:17:44.387534 xknxproject-3.0.0/xknxproject/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-25 21:17:26.000000 xknxproject-3.0.0/xknxproject/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-25 21:17:26.000000 xknxproject-3.0.0/xknxproject/exceptions/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:17:44.387534 xknxproject-3.0.0/xknxproject/loader/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-25 21:17:26.000000 xknxproject-3.0.0/xknxproject/loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8712 2023-04-25 21:17:26.000000 xknxproject-3.0.0/xknxproject/loader/application_program_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-04-25 21:17:26.000000 xknxproject-3.0.0/xknxproject/loader/hardware_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-04-25 21:17:26.000000 xknxproject-3.0.0/xknxproject/loader/knx_master_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10825 2023-04-25 21:17:26.000000 xknxproject-3.0.0/xknxproject/loader/project_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:17:44.387534 xknxproject-3.0.0/xknxproject/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-25 21:17:26.000000 xknxproject-3.0.0/xknxproject/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-04-25 21:17:26.000000 xknxproject-3.0.0/xknxproject/models/knxproject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9720 2023-04-25 21:17:26.000000 xknxproject-3.0.0/xknxproject/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-25 21:17:26.000000 xknxproject-3.0.0/xknxproject/models/static.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:17:26.000000 xknxproject-3.0.0/xknxproject/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-25 21:17:26.000000 xknxproject-3.0.0/xknxproject/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-04-25 21:17:26.000000 xknxproject-3.0.0/xknxproject/xknxproj.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:17:44.387534 xknxproject-3.0.0/xknxproject/xml/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-25 21:17:26.000000 xknxproject-3.0.0/xknxproject/xml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10199 2023-04-25 21:17:26.000000 xknxproject-3.0.0/xknxproject/xml/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:17:44.387534 xknxproject-3.0.0/xknxproject/zip/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-25 21:17:26.000000 xknxproject-3.0.0/xknxproject/zip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-04-25 21:17:26.000000 xknxproject-3.0.0/xknxproject/zip/extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:17:44.383534 xknxproject-3.0.0/xknxproject.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23615 2023-04-25 21:17:43.000000 xknxproject-3.0.0/xknxproject.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-04-25 21:17:44.000000 xknxproject-3.0.0/xknxproject.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 21:17:43.000000 xknxproject-3.0.0/xknxproject.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-25 21:17:44.000000 xknxproject-3.0.0/xknxproject.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-25 21:17:44.000000 xknxproject-3.0.0/xknxproject.egg-info/top_level.txt
```

### Comparing `xknxproject-2.1.0/LICENSE` & `xknxproject-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xknxproject-2.1.0/PKG-INFO` & `xknxproject-3.0.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: xknxproject
-Version: 2.1.0
-Summary: A library to gather information from ETS project files used for KNX
-Download-URL: https://github.com/XKNX/xknxproject/archive/2.1.0.zip
-Author: Marvin Wichmann
-Author-email: me@marvin-wichmann.de
-License: GNU GPL
-Keywords: knx eib ets ets5 ets6
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # (X)KNX Project
 
 [![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=f8b424)](https://github.com/pre-commit/pre-commit)
 [![Discord](https://img.shields.io/discord/338619021215924227?color=7289da&label=Discord&logo=discord&logoColor=7289da)](https://discord.gg/bkZe9m4zvw)
 [![codecov](https://codecov.io/gh/XKNX/xknxproject/branch/main/graph/badge.svg?token=LgPvZpKK3k)](https://codecov.io/gh/XKNX/xknxproject)
 
 Extracts KNX projects and parses the underlying XML.
@@ -33,27 +16,33 @@
 * CommunicationObjectInstance references for their devices (GA assignments)
 * Group Addresses and their DPT type if set
 * The application programs communication objects, their respective flags and the DPT Type
 * Location information of devices (in which rooms they are)
 
 Caution: Loading a middle-sized project with this tool takes about 1.5 seconds. For bigger projects this might as well be >3s.
 
+Not all supported languages are included in project / application data. If the configured language is not found, the default language will be used - which is manufacturer / product dependent.
+
 ## Installation
 
 `pip install xknxproject`
 
 ## Usage
 
 ```python
 """Extract and parse a KNX project file."""
 from xknxproject.models import KNXProject
 from xknxproject import XKNXProj
 
 
-knxproj: XKNXProj = XKNXProj("path/to/your/file.knxproj", "optional_password")
+knxproj: XKNXProj = XKNXProj(
+    path="path/to/your/file.knxproj",
+    password="password",  # optional
+    language="de-DE",  # optional
+)
 project: KNXProject = knxproj.parse()
 ```
 
-The `KNXProject` is a typed dictionary and can be used just like a dictionary, or can be exported as JSON.
+The resulting `KNXProject` is a typed dictionary and can be used just like a dictionary, or can be exported as JSON.
 You can find an example file (exported JSON) in our test suite under https://github.com/XKNX/xknxproject/tree/main/test/resources/stubs
 
 The full type definition can be found here: https://github.com/XKNX/xknxproject/blob/main/xknxproject/models/knxproject.py
```

### Comparing `xknxproject-2.1.0/pyproject.toml` & `xknxproject-3.0.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,64 @@
+[build-system]
+requires = ["setuptools~=62.3"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name         = "xknxproject"
+authors      = [
+    {name = "Marvin Wichmann", email = "me@marvin-wichmann.de"},
+    {name = "Matthias Alphart", email = "farmio@alphart.net"},
+]
+classifiers  = [
+    "Development Status :: 4 - Beta",
+    "Intended Audience :: Developers",
+    "Programming Language :: Python :: 3",
+]
+dependencies = [
+    "cryptography>=40.0.0",
+    "pyzipper>=0.3.6",
+]
+description  = "A library to gather information from ETS project files used for KNX"
+dynamic      = ["version"]
+keywords     = ["KNX", "ETS", "Home Assistant"]
+license      = {file = "LICENSE"}
+readme       = "README.md"
+requires-python = ">=3.9.0"
+
+[project.urls]
+homepage = "https://github.com/XKNX/xknxproject"
+
+
+[tool.setuptools.dynamic]
+version = {attr = "xknxproject.__version__.__version__"}
+
+[tool.setuptools.packages.find]
+include = ["xknxproject*"]
+
 [tool.black]
-target-version = ["py39", "py310"]
+target-version = ["py39", "py310", "py311"]
 exclude = "generated"
 
+
 [tool.isort]
 profile = "black"
 # will group `import x` and `from x import` of the same module.
 force_sort_within_sections = true
 combine_as_imports = true
 
+
 [tool.mypy]
 python_version = "3.9"
 strict = true
 show_error_codes = true
 ignore_missing_imports = true
 implicit_reexport = true
 warn_unreachable = true
 
+
 [tool.pylint.master]
 ignore = "test"
 persistent = "no"
 reports = "no"
 
 [tool.pylint.message_control]
 # Reasons disabled:
@@ -74,8 +113,7 @@
 [tool.pylint.reports]
 score = "no"
 output-format = "colorized"
 
 
 [tool.pytest.ini_options]
 testpaths = "test"
-asyncio_mode = "auto"
```

### Comparing `xknxproject-2.1.0/xknxproject/loader/project_loader.py` & `xknxproject-3.0.0/xknxproject/loader/project_loader.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,49 @@
 """Project file loader."""
 from __future__ import annotations
 
+import re
 from xml.etree import ElementTree
 
 from xknxproject.models import (
     ComObjectInstanceRef,
     DeviceInstance,
     SpaceType,
     XMLArea,
     XMLGroupAddress,
     XMLLine,
+    XMLProjectInformation,
     XMLSpace,
 )
-from xknxproject.util import parse_dpt_types, parse_xml_flag
+from xknxproject.util import parse_dpt_type, parse_xml_flag
 from xknxproject.zip import KNXProjContents
 
 
 class ProjectLoader:
     """Load Project file."""
 
     @staticmethod
     def load(
         knx_proj_contents: KNXProjContents,
+        space_usage_names: dict[str, str],
     ) -> tuple[
-        list[XMLGroupAddress], list[XMLArea], list[DeviceInstance], list[XMLSpace]
+        list[XMLGroupAddress],
+        list[XMLArea],
+        list[DeviceInstance],
+        list[XMLSpace],
+        XMLProjectInformation,
     ]:
         """Load topology mappings."""
         areas: list[XMLArea] = []
         devices: list[DeviceInstance] = []
         group_address_list: list[XMLGroupAddress] = []
         spaces: list[XMLSpace] = []
 
-        with knx_proj_contents.open_project_0() as project_file:
-            tree = ElementTree.parse(project_file)
+        with knx_proj_contents.open_project_0() as project_0_file:
+            tree = ElementTree.parse(project_0_file)
             for ga_element in tree.findall(
                 # `//` to ignore <GroupRange> tags to support different GA level formats
                 "{*}Project/{*}Installations/{*}Installation/{*}GroupAddresses//{*}GroupAddress"
             ):
                 group_address_list.append(
                     _GroupAddressLoader.load(group_address_element=ga_element),
                 )
@@ -49,33 +56,40 @@
             for area in areas:
                 for line in area.lines:
                     devices.extend(line.devices)
             for location_element in tree.findall(
                 "{*}Project/{*}Installations/{*}Installation/{*}Locations"
             ):
                 spaces.extend(
-                    _LocationLoader(devices).load(location_element=location_element),
+                    _LocationLoader(devices, space_usage_names).load(
+                        location_element=location_element
+                    ),
                 )
 
-        return group_address_list, areas, devices, spaces
+        with knx_proj_contents.open_project_meta() as project_file:
+            tree = ElementTree.parse(project_file)
+            project_info = load_project_info(tree)
+
+        return group_address_list, areas, devices, spaces, project_info
 
 
 class _GroupAddressLoader:
     """Load GroupAddress info from KNX XML."""
 
     @staticmethod
     def load(group_address_element: ElementTree.Element) -> XMLGroupAddress:
         """Load GroupAddress mappings."""
 
         return XMLGroupAddress(
             name=group_address_element.get("Name", ""),
             identifier=group_address_element.get("Id", ""),
             address=group_address_element.get("Address", ""),
-            dpt_type=group_address_element.get("DatapointType"),
+            project_uid=int(group_address_element.get("Puid")),  # type: ignore[arg-type]
             description=group_address_element.get("Description", ""),
+            dpt=parse_dpt_type(group_address_element.get("DatapointType")),
         )
 
 
 class _TopologyLoader:
     """Load topology from KNX XML."""
 
     @staticmethod
@@ -121,35 +135,31 @@
         return line
 
     @staticmethod
     def _create_device(
         device_element: ElementTree.Element, line: XMLLine
     ) -> DeviceInstance | None:
         """Create device."""
-        identifier: str = device_element.get("Id", "")
         address: str | None = device_element.get("Address")
-
         #  devices like power supplies do usually not have an IA.
         if address is None:
             return None
 
-        name: str = device_element.get("Name", "")
-        last_modified: str = device_element.get("LastModified", "")
-        _product_ref_parts = device_element.get("ProductRefId", "").split("_")
-        hardware_ref = _product_ref_parts[0] + "_" + _product_ref_parts[1]
-        hardware_program_ref = device_element.get("Hardware2ProgramRefId", "")
+        product_ref = device_element.get("ProductRefId", "")
         device: DeviceInstance = DeviceInstance(
-            identifier=identifier,
+            identifier=device_element.get("Id", ""),
             address=address,
-            name=name,
-            last_modified=last_modified,
-            hardware_ref=hardware_ref,
-            hardware_program_ref=hardware_program_ref,
+            project_uid=int(device_element.get("Puid")),  # type: ignore[arg-type]
+            name=device_element.get("Name", ""),
+            description=device_element.get("Description", ""),
+            last_modified=device_element.get("LastModified", ""),
+            product_ref=product_ref,
+            hardware_program_ref=device_element.get("Hardware2ProgramRefId", ""),
             line=line,
-            manufacturer=_product_ref_parts[0],
+            manufacturer=product_ref.split("_", 1)[0],
         )
 
         for sub_node in device_element:
             if sub_node.tag.endswith("AdditionalAddresses"):
                 for address_node in sub_node:
                     if _address := address_node.get("Address"):
                         device.additional_addresses.append(_address)
@@ -166,57 +176,101 @@
     def _create_com_object_instance(
         com_object: ElementTree.Element,
     ) -> ComObjectInstanceRef | None:
         """Create ComObjectInstanceRef."""
         if not (links := com_object.get("Links")):
             return None
 
-        _dpt_type = com_object.get("DatapointType")
-        datapoint_type = parse_dpt_types(_dpt_type.split(" ")) if _dpt_type else None
-
         return ComObjectInstanceRef(
             identifier=com_object.get("Id"),
             ref_id=com_object.get("RefId"),  # type: ignore[arg-type]
             text=com_object.get("Text"),
             function_text=com_object.get("FunctionText"),
             read_flag=parse_xml_flag(com_object.get("ReadFlag")),
             write_flag=parse_xml_flag(com_object.get("WriteFlag")),
             communication_flag=parse_xml_flag(com_object.get("CommunicationFlag")),
             transmit_flag=parse_xml_flag(com_object.get("TransmitFlag")),
             update_flag=parse_xml_flag(com_object.get("UpdateFlag")),
             read_on_init_flag=parse_xml_flag(com_object.get("ReadOnInitFlag")),
-            datapoint_type=datapoint_type,
+            datapoint_type=parse_dpt_type(com_object.get("DatapointType")),
             description=com_object.get("Description"),
             links=links.split(" "),
         )
 
 
 class _LocationLoader:
     """Load location infos from KNX XML."""
 
-    def __init__(self, devices: list[DeviceInstance]):
+    def __init__(
+        self,
+        devices: list[DeviceInstance],
+        space_usage_names: dict[str, str],
+    ):
         """Initialize the LocationLoader."""
         self.devices: dict[str, str] = {
             device.identifier: device.individual_address for device in devices
         }
+        self.space_usage_names = space_usage_names
 
     def load(self, location_element: ElementTree.Element) -> list[XMLSpace]:
         """Load Location mappings."""
         return [
             self.parse_space(space) for space in location_element.findall("{*}Space")
         ]
 
     def parse_space(self, node: ElementTree.Element) -> XMLSpace:
         """Parse a space from the document."""
-        name: str = node.get("Name", "")
-        space_type = SpaceType(node.get("Type"))
-        space: XMLSpace = XMLSpace([], space_type, name, [])
+        usage_id = node.get("Usage")
+        usage_text = self.space_usage_names.get(usage_id, "") if usage_id else ""
+        space: XMLSpace = XMLSpace(
+            identifier=node.get("Id"),  # type: ignore[arg-type]
+            name=node.get("Name"),  # type: ignore[arg-type]
+            space_type=SpaceType(node.get("Type")),
+            usage_id=usage_id,
+            usage_text=usage_text,
+            number=node.get("Number", ""),
+            description=node.get("Description", ""),
+            project_uid=int(node.get("Puid")),  # type: ignore[arg-type]
+            spaces=[],
+            devices=[],
+        )
 
         for sub_node in node:
             if sub_node.tag.endswith("Space"):
                 # recursively call parse space since this can be nested for an unbound time in the XSD
                 space.spaces.append(self.parse_space(sub_node))
             elif sub_node.tag.endswith("DeviceInstanceRef"):
                 if individual_address := self.devices.get(sub_node.get("RefId", "")):
                     space.devices.append(individual_address)
 
         return space
+
+
+def load_project_info(tree: ElementTree.ElementTree) -> XMLProjectInformation:
+    """Load project information."""
+    knx_root = tree.getroot()
+    _namespace_match = re.match(r"{.+\/project\/(.+)}", knx_root.tag)
+    schema_version = _namespace_match.group(1) if _namespace_match else ""
+    created_by = knx_root.get("CreatedBy", "")
+    tool_version = knx_root.get("ToolVersion", "")
+
+    try:
+        project_node: ElementTree.Element = tree.find("{*}Project")  # type: ignore[assignment]
+        identifier = project_node.get("Id", "")
+        info_node: ElementTree.Element = project_node.find("{*}ProjectInformation")  # type: ignore[assignment]
+        return XMLProjectInformation(
+            project_id=identifier,
+            name=info_node.get("Name", ""),
+            last_modified=info_node.get("LastModified"),
+            group_address_style=info_node.get("GroupAddressStyle"),  # type: ignore[arg-type]
+            guid=info_node.get("Guid"),  # type: ignore[arg-type]
+            created_by=created_by,
+            schema_version=schema_version,
+            tool_version=tool_version,
+        )
+    except AttributeError:
+        # Project or ProjectInformation tag not found
+        return XMLProjectInformation(
+            created_by=created_by,
+            schema_version=schema_version,
+            tool_version=tool_version,
+        )
```

### Comparing `xknxproject-2.1.0/xknxproject/models/__init__.py` & `xknxproject-3.0.0/xknxproject/models/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,53 @@
 """Xknxproj models."""
 from .knxproject import (
     Area,
     CommunicationObject,
     Device,
+    DPTType,
     Flags,
     GroupAddress,
     KNXProject,
     Line,
+    ProjectInfo,
     Space,
 )
 from .models import (
     ComObject,
     ComObjectInstanceRef,
     ComObjectRef,
     DeviceInstance,
-    Hardware,
+    HardwareToPrograms,
+    Product,
     XMLArea,
     XMLGroupAddress,
     XMLLine,
+    XMLProjectInformation,
     XMLSpace,
 )
 from .static import MEDIUM_TYPES, SpaceType
 
 __all__ = [
     "Area",
-    "Line",
     "CommunicationObject",
-    "GroupAddress",
     "Device",
+    "DPTType",
     "Flags",
+    "GroupAddress",
     "KNXProject",
-    "XMLArea",
+    "Line",
+    "ProjectInfo",
+    "Space",
     "ComObject",
     "ComObjectInstanceRef",
     "ComObjectRef",
-    "SpaceType",
-    "Space",
     "DeviceInstance",
+    "HardwareToPrograms",
+    "Product",
+    "XMLArea",
     "XMLGroupAddress",
     "XMLLine",
     "XMLSpace",
-    "Hardware",
+    "XMLProjectInformation",
     "MEDIUM_TYPES",
+    "SpaceType",
 ]
```

### Comparing `xknxproject-2.1.0/xknxproject/models/knxproject.py` & `xknxproject-3.0.0/xknxproject/models/knxproject.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 """Define output type for parsed KNX project."""
 from __future__ import annotations
 
-from typing import Any, TypedDict
+from typing import TypedDict
+
+
+class DPTType(TypedDict):
+    """DPT type dictionary."""
+
+    main: int
+    sub: int | None
 
 
 class Flags(TypedDict):
     """Flags for the group addresses and KOs."""
 
     read: bool
     write: bool
@@ -14,29 +21,35 @@
     update: bool
     read_on_init: bool
 
 
 class CommunicationObject(TypedDict):
     """Communication object dictionary."""
 
-    name: str | None
+    name: str
+    number: int
+    text: str
+    function_text: str
+    description: str
     device_address: str
-    dpt_type: dict[str, int]
+    dpt: DPTType | None
+    object_size: str
     group_address_links: list[str]
     flags: Flags
 
 
 class Device(TypedDict):
     """Devices dictionary."""
 
     name: str
-    product_name: str
+    hardware_name: str
     description: str
     manufacturer_name: str
     individual_address: str
+    project_uid: int
     communication_object_ids: list[str]
 
 
 class Line(TypedDict):
     """Line typed dict."""
 
     name: str
@@ -56,29 +69,52 @@
 class GroupAddress(TypedDict):
     """GroupAddress typed dict."""
 
     name: str
     identifier: str
     raw_address: int
     address: str
-    dpt_type: dict[str, int] | None
+    project_uid: int
+    dpt: DPTType | None
     communication_object_ids: list[str]
     description: str
 
 
 class Space(TypedDict):
     """Space typed dict."""
 
     type: str
+    identifier: str
+    name: str
+    usage_id: str | None
+    usage_text: str
+    number: str
+    description: str
+    project_uid: int
     devices: list[str]
-    spaces: dict[str, Any]
+    spaces: dict[str, Space]
+
+
+class ProjectInfo(TypedDict):
+    """Information about the project."""
+
+    project_id: str
+    name: str
+    last_modified: str | None
+    group_address_style: str
+    guid: str
+    created_by: str
+    schema_version: str
+    tool_version: str
+    xknxproject_version: str
+    language_code: str | None
 
 
 class KNXProject(TypedDict):
     """KNXProject typed dictionary."""
 
-    version: str
+    info: ProjectInfo
     communication_objects: dict[str, CommunicationObject]
     devices: dict[str, Device]
     topology: dict[str, Area]
     locations: dict[str, Space]
     group_addresses: dict[str, GroupAddress]
```

### Comparing `xknxproject-2.1.0/xknxproject/models/models.py` & `xknxproject-3.0.0/xknxproject/models/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,49 +1,51 @@
 """Handles Group adresses."""
 from __future__ import annotations
 
 from dataclasses import dataclass
 import re
 
+from xknxproject.models.knxproject import DPTType
 from xknxproject.models.static import SpaceType
-from xknxproject.util import parse_dpt_types
 
 
 class XMLGroupAddress:
     """Class that represents a group address."""
 
     def __init__(
         self,
         name: str,
         identifier: str,
         address: str,
+        project_uid: int,
         description: str,
-        dpt_type: str | None,
+        dpt: DPTType | None,
     ):
         """Initialize a group address."""
         self.name = name
         self.identifier = identifier.split("_")[1]
         self.raw_address = int(address)
+        self.project_uid = project_uid
         self.description = description
-        self.dpt_type = (
-            None if dpt_type is None else parse_dpt_types(dpt_type.split(" "))
-        )
+        self.dpt = dpt
 
         self.address = self._parse_address()
 
     def _parse_address(self) -> str:
         """Parse a given address and returns a string representation of it."""
         main = (self.raw_address & 0b1111100000000000) >> 11
         middle = (self.raw_address & 0b11100000000) >> 8
         sub = self.raw_address & 0b11111111
         return f"{main}/{middle}/{sub}"
 
     def __repr__(self) -> str:
         """Return string representation."""
-        return f"{self.address} ({self.name}) - [DPT: {self.dpt_type}, ID: {self.identifier}]"
+        return (
+            f"{self.address} ({self.name}) - [DPT: {self.dpt}, ID: {self.identifier}]"
+        )
 
 
 @dataclass
 class XMLArea:
     """Class that represents a area."""
 
     address: int
@@ -68,30 +70,34 @@
     """Class that represents a device instance."""
 
     def __init__(
         self,
         *,
         identifier: str,
         address: str,
+        project_uid: int,
         name: str,
+        description: str,
         last_modified: str,
-        hardware_ref: str,
+        product_ref: str,
         hardware_program_ref: str,
         line: XMLLine,
         manufacturer: str,
         additional_addresses: list[str] | None = None,
         com_object_instance_refs: list[ComObjectInstanceRef] | None = None,
         com_objects: list[ComObject] | None = None,
     ):
         """Initialize a Device Instance."""
         self.identifier = identifier
         self.address = address
         self.name = name
+        self.description = description
+        self.project_uid = project_uid
         self.last_modified = last_modified
-        self.hardware_ref = hardware_ref
+        self.product_ref = product_ref
         self.hardware_program_ref = hardware_program_ref
         self.line = line
         self.manufacturer = manufacturer
         self.additional_addresses = additional_addresses or []
         self.com_object_instance_refs = com_object_instance_refs or []
         self.com_objects = com_objects or []
         self.application_program_ref: str | None = None
@@ -126,28 +132,31 @@
     function_text: str | None  # "FunctionText"
     read_flag: bool | None  # "ReadFlag" - knx:Enable_t
     write_flag: bool | None  # "WriteFlag" - knx:Enable_t
     communication_flag: bool | None  # "CommunicationFlag" - knx:Enable_t
     transmit_flag: bool | None  # "TransmitFlag" - knx:Enable_t
     update_flag: bool | None  # "UpdateFlag" - knx:Enable_t
     read_on_init_flag: bool | None  # "ReadOnInitFlag" - knx:Enable_t
-    datapoint_type: dict[str, int] | None  # "DataPointType" - knx:IDREFS
+    datapoint_type: DPTType | None  # "DataPointType" - knx:IDREFS
     description: str | None  # "Description" - language dependent
     links: list[str] | None  # "Links" - knx:RELIDREFS
 
+    # resolved via Hardware.xml from the containing DeviceInstance
+    com_object_ref_id: str | None = None
+
     # only available form ComObject and ComObjectRef
     name: str | None = None
     number: int | None = None
     object_size: str | None = None
 
-    def update_ref_id(self, application_program_ref: str) -> None:
+    def resolve_com_object_ref_id(self, application_program_ref: str) -> None:
         """Prepend the ref_id with the application program ref."""
         # Remove module and ModuleInstance occurence as they will not be in the application program directly
-        self.ref_id = re.sub(r"(M-\d+?_MI-\d+?_)", "", self.ref_id)
-        self.ref_id = f"{application_program_ref}_{self.ref_id}"
+        ref_id = re.sub(r"(M-\d+?_MI-\d+?_)", "", self.ref_id)
+        self.com_object_ref_id = f"{application_program_ref}_{ref_id}"
 
     def merge_from_application(self, com_object: ComObject | ComObjectRef) -> None:
         """Fill missing information with information parsed from the application program."""
         if self.name is None:
             self.name = com_object.name
         if self.text is None:
             self.text = com_object.text
@@ -169,15 +178,15 @@
             self.read_on_init_flag = com_object.read_on_init_flag
         if self.datapoint_type is None:
             self.datapoint_type = com_object.datapoint_type
         if isinstance(com_object, ComObject):
             self.number = com_object.number
 
 
-@dataclass(frozen=True)
+@dataclass
 class ComObject:
     """Class that represents a ComObject instance."""
 
     __slots__ = (
         "identifier",
         "name",
         "text",
@@ -202,18 +211,18 @@
     object_size: str  # "ObjectSize" - knx:ComObjectSize_t
     read_flag: bool  # "ReadFlag" - knx:Enable_t
     write_flag: bool  # "WriteFlag" - knx:Enable_t
     communication_flag: bool  # "CommunicationFlag" - knx:Enable_t
     transmit_flag: bool  # "TransmitFlag" - knx:Enable_t
     update_flag: bool  # "UpdateFlag" - knx:Enable_t
     read_on_init_flag: bool  # "ReadOnInitFlag" - knx:Enable_t
-    datapoint_type: dict[str, int] | None  # "DataPointType" - knx:IDREFS - optional
+    datapoint_type: DPTType | None  # "DataPointType" - knx:IDREFS - optional
 
 
-@dataclass(frozen=True)
+@dataclass
 class ComObjectRef:
     """Class that represents a ComObjectRef instance."""
 
     __slots__ = (
         "identifier",
         "ref_id",
         "name",
@@ -237,30 +246,51 @@
     object_size: str | None  # "ObjectSize" - knx:ComObjectSize_t
     read_flag: bool | None  # "ReadFlag" - knx:Enable_t
     write_flag: bool | None  # "WriteFlag" - knx:Enable_t
     communication_flag: bool | None  # "CommunicationFlag" - knx:Enable_t
     transmit_flag: bool | None  # "TransmitFlag" - knx:Enable_t
     update_flag: bool | None  # "UpdateFlag" - knx:Enable_t
     read_on_init_flag: bool | None  # "ReadOnInitFlag" - knx:Enable_t
-    datapoint_type: dict[str, int] | None  # "DataPointType" - knx:IDREFS
+    datapoint_type: DPTType | None  # "DataPointType" - knx:IDREFS
 
 
 @dataclass
 class XMLSpace:
     """A space in the location XML."""
 
-    spaces: list[XMLSpace]
-    type: SpaceType
+    identifier: str
     name: str
-    devices: list[str]
+    space_type: SpaceType
+    usage_id: str | None  # SU-<int> resolved from knx_master.xml (with translation)
+    usage_text: str  # default to "" - translated
+    number: str  # default to ""
+    description: str  # default to ""
+    project_uid: int
+    spaces: list[XMLSpace]
+    devices: list[str]  # [DeviceInstance.individual_address]
 
 
 @dataclass
-class Hardware:
-    """Model a Hardware instance."""
+class Product:
+    """Model a Product instance."""
 
     identifier: str
-    name: str
-    product_name: str
-    application_program_refs: dict[
-        str, str
-    ]  # {Hardware2ProgramRefID: ApplicationProgramRef}
+    text: str
+    hardware_name: str = ""
+
+
+HardwareToPrograms = dict[str, str]
+
+
+@dataclass
+class XMLProjectInformation:
+    """Model a ProjectInformation instance."""
+
+    # ProjectInformation tag is not required in XSD, thus everything is optional
+    project_id: str = ""
+    name: str = ""
+    last_modified: str | None = None
+    group_address_style: str = ""
+    guid: str = ""
+    created_by: str = ""
+    schema_version: str = ""
+    tool_version: str = ""
```

### Comparing `xknxproject-2.1.0/xknxproject/models/static.py` & `xknxproject-3.0.0/xknxproject/models/static.py`

 * *Files identical despite different names*

### Comparing `xknxproject-2.1.0/xknxproject/util.py` & `xknxproject-3.0.0/xknxproject/util.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,41 @@
 """XML utilities."""
 from __future__ import annotations
 
+import logging
 from typing import overload
 
 from xknxproject.const import MAIN_AND_SUB_DPT, MAIN_DPT
+from xknxproject.models import DPTType
 
+_LOGGER = logging.getLogger("xknxproject.log")
 
-def parse_dpt_types(dpt_types: list[str]) -> dict[str, int]:
-    """Parse the DPT types from the KNX project to main and sub types."""
-    if len(dpt_types) == 0:
-        return {}
-
-    dpt_type: str = dpt_types[-1]
-    if MAIN_DPT in dpt_type:
-        return {"main": int(dpt_type.split("-")[1])}
-    if MAIN_AND_SUB_DPT in dpt_type:
-        return {"main": int(dpt_type.split("-")[1]), "sub": int(dpt_type.split("-")[2])}
 
-    return {}
+def parse_dpt_type(dpt_string: str | None) -> DPTType | None:
+    """Parse a DPT type from the XML representation to main and sub types."""
+    if not dpt_string:
+        return None
+
+    last_dpt: str = dpt_string.split(" ")[-1]
+    dpt_parts = last_dpt.split("-")
+    try:
+        if MAIN_DPT == dpt_parts[0]:
+            return DPTType(
+                main=int(dpt_parts[1]),
+                sub=None,
+            )
+        if MAIN_AND_SUB_DPT == dpt_parts[0]:
+            return DPTType(
+                main=int(dpt_parts[1]),
+                sub=int(dpt_parts[2]),
+            )
+    except (IndexError, ValueError):
+        pass
+    _LOGGER.warning('Could not parse DPTType from: "%s"', dpt_string)
+    return None
 
 
 @overload
 def parse_xml_flag(flag: str | None, default: bool) -> bool:
     ...
```

### Comparing `xknxproject-2.1.0/xknxproject/xknxproj.py` & `xknxproject-3.0.0/xknxproject/xknxproj.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,49 @@
 """ETS Project Parser is a library to parse ETS project files."""
 from __future__ import annotations
 
 import logging
 from pathlib import Path
+import time
 
-from xknxproject import __version__
+from xknxproject.__version__ import __version__
 from xknxproject.models import KNXProject
 from xknxproject.xml import XMLParser
 from xknxproject.zip.extractor import extract
 
-logger = logging.getLogger("xknxproject.log")
+_LOGGER = logging.getLogger("xknxproject.log")
 
 
 class XKNXProj:
     """Class for parsing ETS project files."""
 
     def __init__(
         self,
-        archive_name: str | Path,
-        archive_password: str | None = None,
+        path: str | Path,
+        password: str | None = None,
+        language: str | None = None,
     ):
         """Initialize a KNXProjParser."""
-        self.archive_path = Path(archive_name)
-        self.password = archive_password
-
-        self.version = __version__
+        self.path = Path(path)
+        self.password = password
+        self.language = language
 
     def parse(self) -> KNXProject:
         """Parse the KNX project."""
-        with extract(self.archive_path, self.password) as knx_project_content:
-            return XMLParser(knx_project_content).parse()
+        _LOGGER.info(
+            'Xknxproject version %s parsing "%s" with%s password...',
+            __version__,
+            self.path,
+            "" if self.password else "out",
+        )
+        _start = time.time()
+        with extract(self.path, self.password) as knx_project_content:
+            project = XMLParser(knx_project_content).parse(self.language)
+
+        _LOGGER.info("Parsing took %s seconds", time.time() - _start)
+        _LOGGER.info(
+            "Found %s group addresses, %s devices and %s used communication objects",
+            len(project["group_addresses"]),
+            len(project["devices"]),
+            len(project["communication_objects"]),
+        )
+        return project
```

### Comparing `xknxproject-2.1.0/xknxproject.egg-info/SOURCES.txt` & `xknxproject-3.0.0/xknxproject.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
-setup.py
 test/test_knxproj.py
 test/test_util.py
 xknxproject/__init__.py
 xknxproject/__version__.py
 xknxproject/const.py
 xknxproject/py.typed
 xknxproject/util.py
 xknxproject/xknxproj.py
 xknxproject.egg-info/PKG-INFO
 xknxproject.egg-info/SOURCES.txt
 xknxproject.egg-info/dependency_links.txt
-xknxproject.egg-info/not-zip-safe
 xknxproject.egg-info/requires.txt
 xknxproject.egg-info/top_level.txt
 xknxproject/exceptions/__init__.py
 xknxproject/exceptions/exceptions.py
 xknxproject/loader/__init__.py
 xknxproject/loader/application_program_loader.py
 xknxproject/loader/hardware_loader.py
-xknxproject/loader/manufacturer_loader.py
+xknxproject/loader/knx_master_loader.py
 xknxproject/loader/project_loader.py
 xknxproject/models/__init__.py
 xknxproject/models/knxproject.py
 xknxproject/models/models.py
 xknxproject/models/static.py
 xknxproject/xml/__init__.py
 xknxproject/xml/parser.py
```

