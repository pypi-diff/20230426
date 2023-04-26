# Comparing `tmp/eos_downloader-0.8.0.tar.gz` & `tmp/eos_downloader-0.8.1.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eos_downloader-0.8.0.tar", last modified: Fri Apr 21 08:16:55 2023, max compression
+gzip compressed data, was "eos_downloader-0.8.1.dev1.tar", last modified: Wed Apr 26 09:37:25 2023, max compression
```

## Comparing `eos_downloader-0.8.0.tar` & `eos_downloader-0.8.1.dev1.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:16:55.809499 eos_downloader-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11403 2023-04-21 08:16:44.000000 eos_downloader-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20707 2023-04-21 08:16:55.809499 eos_downloader-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-04-21 08:16:44.000000 eos_downloader-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:16:55.809499 eos_downloader-0.8.0/eos_downloader/
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-04-21 08:16:44.000000 eos_downloader-0.8.0/eos_downloader/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:16:55.809499 eos_downloader-0.8.0/eos_downloader/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 08:16:44.000000 eos_downloader-0.8.0/eos_downloader/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-04-21 08:16:44.000000 eos_downloader-0.8.0/eos_downloader/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:16:55.809499 eos_downloader-0.8.0/eos_downloader/cli/debug/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 08:16:44.000000 eos_downloader-0.8.0/eos_downloader/cli/debug/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-04-21 08:16:44.000000 eos_downloader-0.8.0/eos_downloader/cli/debug/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:16:55.809499 eos_downloader-0.8.0/eos_downloader/cli/get/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 08:16:44.000000 eos_downloader-0.8.0/eos_downloader/cli/get/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-04-21 08:16:44.000000 eos_downloader-0.8.0/eos_downloader/cli/get/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:16:55.809499 eos_downloader-0.8.0/eos_downloader/cli/info/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 08:16:44.000000 eos_downloader-0.8.0/eos_downloader/cli/info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-04-21 08:16:44.000000 eos_downloader-0.8.0/eos_downloader/cli/info/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     8774 2023-04-21 08:16:44.000000 eos_downloader-0.8.0/eos_downloader/cvp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-04-21 08:16:44.000000 eos_downloader-0.8.0/eos_downloader/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-04-21 08:16:44.000000 eos_downloader-0.8.0/eos_downloader/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     6929 2023-04-21 08:16:44.000000 eos_downloader-0.8.0/eos_downloader/eos.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:16:55.809499 eos_downloader-0.8.0/eos_downloader/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 08:16:44.000000 eos_downloader-0.8.0/eos_downloader/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8060 2023-04-21 08:16:44.000000 eos_downloader-0.8.0/eos_downloader/models/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    18273 2023-04-21 08:16:44.000000 eos_downloader-0.8.0/eos_downloader/object_downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:16:55.809499 eos_downloader-0.8.0/eos_downloader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20707 2023-04-21 08:16:55.000000 eos_downloader-0.8.0/eos_downloader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-21 08:16:55.000000 eos_downloader-0.8.0/eos_downloader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 08:16:55.000000 eos_downloader-0.8.0/eos_downloader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-21 08:16:55.000000 eos_downloader-0.8.0/eos_downloader.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-21 08:16:55.000000 eos_downloader-0.8.0/eos_downloader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-21 08:16:55.000000 eos_downloader-0.8.0/eos_downloader.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-04-21 08:16:44.000000 eos_downloader-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 08:16:55.809499 eos_downloader-0.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:37:25.000287 eos_downloader-0.8.1.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11403 2023-04-26 09:37:12.000000 eos_downloader-0.8.1.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20718 2023-04-26 09:37:25.000287 eos_downloader-0.8.1.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6244 2023-04-26 09:37:12.000000 eos_downloader-0.8.1.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:37:24.996287 eos_downloader-0.8.1.dev1/eos_downloader/
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-04-26 09:37:12.000000 eos_downloader-0.8.1.dev1/eos_downloader/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:37:24.996287 eos_downloader-0.8.1.dev1/eos_downloader/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 09:37:12.000000 eos_downloader-0.8.1.dev1/eos_downloader/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-04-26 09:37:12.000000 eos_downloader-0.8.1.dev1/eos_downloader/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:37:24.996287 eos_downloader-0.8.1.dev1/eos_downloader/cli/debug/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 09:37:12.000000 eos_downloader-0.8.1.dev1/eos_downloader/cli/debug/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-04-26 09:37:12.000000 eos_downloader-0.8.1.dev1/eos_downloader/cli/debug/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:37:25.000287 eos_downloader-0.8.1.dev1/eos_downloader/cli/get/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 09:37:12.000000 eos_downloader-0.8.1.dev1/eos_downloader/cli/get/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-04-26 09:37:12.000000 eos_downloader-0.8.1.dev1/eos_downloader/cli/get/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:37:25.000287 eos_downloader-0.8.1.dev1/eos_downloader/cli/info/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 09:37:12.000000 eos_downloader-0.8.1.dev1/eos_downloader/cli/info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-04-26 09:37:12.000000 eos_downloader-0.8.1.dev1/eos_downloader/cli/info/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8861 2023-04-26 09:37:12.000000 eos_downloader-0.8.1.dev1/eos_downloader/cvp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-04-26 09:37:12.000000 eos_downloader-0.8.1.dev1/eos_downloader/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-04-26 09:37:12.000000 eos_downloader-0.8.1.dev1/eos_downloader/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-04-26 09:37:12.000000 eos_downloader-0.8.1.dev1/eos_downloader/eos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:37:25.000287 eos_downloader-0.8.1.dev1/eos_downloader/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 09:37:12.000000 eos_downloader-0.8.1.dev1/eos_downloader/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8993 2023-04-26 09:37:12.000000 eos_downloader-0.8.1.dev1/eos_downloader/models/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18478 2023-04-26 09:37:12.000000 eos_downloader-0.8.1.dev1/eos_downloader/object_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-26 09:37:12.000000 eos_downloader-0.8.1.dev1/eos_downloader/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:37:24.996287 eos_downloader-0.8.1.dev1/eos_downloader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20718 2023-04-26 09:37:24.000000 eos_downloader-0.8.1.dev1/eos_downloader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-26 09:37:24.000000 eos_downloader-0.8.1.dev1/eos_downloader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 09:37:24.000000 eos_downloader-0.8.1.dev1/eos_downloader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-26 09:37:24.000000 eos_downloader-0.8.1.dev1/eos_downloader.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-26 09:37:24.000000 eos_downloader-0.8.1.dev1/eos_downloader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-26 09:37:24.000000 eos_downloader-0.8.1.dev1/eos_downloader.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4451 2023-04-26 09:37:12.000000 eos_downloader-0.8.1.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 09:37:25.000287 eos_downloader-0.8.1.dev1/setup.cfg
```

### Comparing `eos_downloader-0.8.0/LICENSE` & `eos_downloader-0.8.1.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `eos_downloader-0.8.0/PKG-INFO` & `eos_downloader-0.8.1.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eos_downloader
-Version: 0.8.0
+Version: 0.8.1.dev1
 Summary: Arista EOS/CVP downloader script
 Author-email: Thomas Grimonet <thomas.grimonet@gmail.com>
 Maintainer-email: Thomas Grimonet <thomas.grimonet@gmail.com>
 License: Copyright (c) 2019, Arista Networks
         All rights reserved.
         
                                          Apache License
@@ -230,15 +230,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
- [![code-testing](https://github.com/titom73/eos-downloader/actions/workflows/pr-management.yml/badge.svg?event=push)](https://github.com/titom73/eos-downloader/actions/workflows/pr-management.yml) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/eos-downloader) ![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/titom73/arista-downloader) ![PyPI - Downloads](https://img.shields.io/pypi/dm/eos-downloader) ![Docker Image Size (tag)](https://img.shields.io/docker/image-size/titom73/eos-downloader/edge)
+ [![code-testing](https://github.com/titom73/eos-downloader/actions/workflows/pr-management.yml/badge.svg?event=push)](https://github.com/titom73/eos-downloader/actions/workflows/pr-management.yml) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/eos-downloader) ![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/titom73/arista-downloader) ![PyPI - Downloads/month](https://img.shields.io/pypi/dm/eos-downloader) ![Docker Image Size (tag)](https://img.shields.io/docker/image-size/titom73/eos-downloader/edge)
 
 # Arista Software Downloader
 
 Script to download Arista softwares to local folder, Cloudvision or EVE-NG.
 
 ```bash
 pip install eos-downloader
```

### Comparing `eos_downloader-0.8.0/README.md` & `eos_downloader-0.8.1.dev1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
- [![code-testing](https://github.com/titom73/eos-downloader/actions/workflows/pr-management.yml/badge.svg?event=push)](https://github.com/titom73/eos-downloader/actions/workflows/pr-management.yml) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/eos-downloader) ![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/titom73/arista-downloader) ![PyPI - Downloads](https://img.shields.io/pypi/dm/eos-downloader) ![Docker Image Size (tag)](https://img.shields.io/docker/image-size/titom73/eos-downloader/edge)
+ [![code-testing](https://github.com/titom73/eos-downloader/actions/workflows/pr-management.yml/badge.svg?event=push)](https://github.com/titom73/eos-downloader/actions/workflows/pr-management.yml) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/eos-downloader) ![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/titom73/arista-downloader) ![PyPI - Downloads/month](https://img.shields.io/pypi/dm/eos-downloader) ![Docker Image Size (tag)](https://img.shields.io/docker/image-size/titom73/eos-downloader/edge)
 
 # Arista Software Downloader
 
 Script to download Arista softwares to local folder, Cloudvision or EVE-NG.
 
 ```bash
 pip install eos-downloader
```

### Comparing `eos_downloader-0.8.0/eos_downloader/__init__.py` & `eos_downloader-0.8.1.dev1/eos_downloader/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding: utf-8 -*-
 
 """
 EOS Downloader module.
 """
 
 from __future__ import (absolute_import, division,
-                        print_function, unicode_literals)
+                        print_function, unicode_literals, annotations)
 import dataclasses
 from typing import Any
 import json
 import importlib.metadata
 
 __author__ = '@titom73'
 __email__ = 'tom@inetsix.net'
```

### Comparing `eos_downloader-0.8.0/eos_downloader/cli/cli.py` & `eos_downloader-0.8.1.dev1/eos_downloader/cli/cli.py`

 * *Files identical despite different names*

### Comparing `eos_downloader-0.8.0/eos_downloader/cli/debug/commands.py` & `eos_downloader-0.8.1.dev1/eos_downloader/cli/debug/commands.py`

 * *Files identical despite different names*

### Comparing `eos_downloader-0.8.0/eos_downloader/cli/get/commands.py` & `eos_downloader-0.8.1.dev1/eos_downloader/cli/get/commands.py`

 * *Files identical despite different names*

### Comparing `eos_downloader-0.8.0/eos_downloader/cli/info/commands.py` & `eos_downloader-0.8.1.dev1/eos_downloader/cli/info/commands.py`

 * *Files identical despite different names*

### Comparing `eos_downloader-0.8.0/eos_downloader/cvp.py` & `eos_downloader-0.8.1.dev1/eos_downloader/cvp.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,18 @@
 import os
 from typing import List, Optional, Any
 from dataclasses import dataclass
 from loguru import logger
 from cvprac.cvp_client import CvpClient
 from cvprac.cvp_client_errors import CvpLoginError
 
+# from eos_downloader.tools import exc_to_str
+
+# logger = logging.getLogger(__name__)
+
 
 @dataclass
 class CvpAuthenticationItem:
     """
      Data structure to represent Cloudvision Authentication
     """
     server: str
```

### Comparing `eos_downloader-0.8.0/eos_downloader/data.py` & `eos_downloader-0.8.1.dev1/eos_downloader/data.py`

 * *Files identical despite different names*

### Comparing `eos_downloader-0.8.0/eos_downloader/download.py` & `eos_downloader-0.8.1.dev1/eos_downloader/download.py`

 * *Files identical despite different names*

### Comparing `eos_downloader-0.8.0/eos_downloader/eos.py` & `eos_downloader-0.8.1.dev1/eos_downloader/eos.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 import rich
 from loguru import logger
 from rich import console
 
 from eos_downloader.models.version import BASE_BRANCH_STR, BASE_VERSION_STR, REGEX_EOS_VERSION, RTYPE_FEATURE, EosVersion
 from eos_downloader.object_downloader import ObjectDownloader
 
+# logger = logging.getLogger(__name__)
+
 console = rich.get_console()
 
 class EOSDownloader(ObjectDownloader):
     """
     EOSDownloader Object to download EOS images from Arista.com website
 
     Supercharge ObjectDownloader to support EOS specific actions
@@ -51,15 +53,15 @@
         os.system(f"rm -rf {raw_folder}")
         os.system(f"mkdir -p {raw_folder}")
         os.system(
             f'guestmount -a {os.path.join(file_path, "hda.qcow2")} -m /dev/sda2 {os.path.join(file_path, "raw")}')
         ztp_file = os.path.join(file_path, 'raw/zerotouch-config')
         with open(ztp_file, 'w', encoding='ascii') as zfile:
             zfile.write('DISABLE=True')
-        logger.info('Unmounting volume in {}', file_path)
+        logger.info(f'Unmounting volume in {file_path}')
         os.system(f"guestunmount {os.path.join(file_path, 'raw')}")
         os.system(f"rm -rf {os.path.join(file_path, 'raw')}")
         logger.info(f"Volume has been successfully unmounted at {file_path}")
 
     def _parse_xml_for_version(self,root_xml: ET.ElementTree, xpath: str = './/dir[@label="Active Releases"]/dir/dir/[@label]') -> List[EosVersion]:
         """
         Extract list of available EOS versions from Arista.com website
```

### Comparing `eos_downloader-0.8.0/eos_downloader/models/version.py` & `eos_downloader-0.8.1.dev1/eos_downloader/models/version.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,19 +3,23 @@
 
 """Module for EOS version management"""
 
 from __future__ import annotations
 
 import re
 import typing
-from typing import Any
+from typing import Any, Optional
 
 from loguru import logger
 from pydantic import BaseModel
 
+from eos_downloader.tools import exc_to_str
+
+# logger = logging.getLogger(__name__)
+
 BASE_VERSION_STR = '4.0.0F'
 BASE_BRANCH_STR = '4.0'
 
 RTYPE_FEATURE = 'F'
 RTYPE_MAINTENANCE = 'M'
 RTYPES = [RTYPE_FEATURE, RTYPE_MAINTENANCE]
 
@@ -54,15 +58,15 @@
 
     Args:
         BaseModel (Pydantic): Pydantic Base Model
     """
     major: int = 4
     minor: int = 0
     patch: int = 0
-    rtype: str = 'F'
+    rtype: Optional[str] = 'F'
     other: Any
 
     @classmethod
     def from_str(cls, eos_version: str) -> EosVersion:
         """
         Class constructor from a string representing EOS version
 
@@ -79,18 +83,20 @@
 
         Returns:
             EosVersion object
         """
         logger.debug(f'receiving version: {eos_version}')
         if REGEX_EOS_VERSION.match(eos_version):
             matches = REGEX_EOS_VERSION.match(eos_version)
+            # assert matches is not None
             assert matches is not None
             return cls(**matches.groupdict())
         if REGEX_EOS_BRANCH.match(eos_version):
             matches = REGEX_EOS_BRANCH.match(eos_version)
+            # assert matches is not None
             assert matches is not None
             return cls(**matches.groupdict())
         logger.error(f'Error occured with {eos_version}')
         return EosVersion()
 
     @property
     def branch(self) -> str:
@@ -133,21 +139,29 @@
 
         Returns:
             float: -1 if ver1 < ver2, 0 if ver1 == ver2, 1 if ver1 > ver2
         """
         if not isinstance(other, EosVersion):
             raise ValueError(f'could not compare {other} as it is not an EosVersion object')
         comparison_flag: float = 0
+        logger.warning(f'current version {self.__str__()} - other {str(other)}')   # pylint: disable = unnecessary-dunder-call
         for key, _ in self.dict().items():
+            if comparison_flag == 0 and self.dict()[key] is None or other.dict()[key] is None:
+                logger.debug(f'{key}: local None - remote None')
+                logger.debug(f'{key}: local {self.dict()} - remote {other.dict()}')
+                return comparison_flag
+            logger.debug(f'{key}: local {self.dict()[key]} - remote {other.dict()[key]}')
             if comparison_flag == 0 and self.dict()[key] < other.dict()[key]:
                 comparison_flag = -1
             if comparison_flag == 0 and self.dict()[key] > other.dict()[key]:
                 comparison_flag = 1
             if comparison_flag != 0:
+                logger.info(f'comparison result is {comparison_flag}')
                 return comparison_flag
+        logger.info(f'comparison result is {comparison_flag}')
         return comparison_flag
 
     @typing.no_type_check
     def __eq__(self, other):
         """ Implement __eq__ function (==) """
         return self._compare(other) == 0
 
@@ -245,11 +259,14 @@
         Args:
             branch_str (str): a string for EOS branch. It supports following formats 4.23 or 4.23.0
 
         Returns:
             bool: True if current version is in provided branch, otherwise False
         """
         try:
+            logger.debug(f'reading branch str:{branch_str}')
             branch = EosVersion.from_str(branch_str)
         except Exception as error:  # pylint: disable = broad-exception-caught
-            logger.error(error)
-        return self.major == branch.major and self.minor == branch.minor
+            logger.error(exc_to_str(error))
+        else:
+            return self.major == branch.major and self.minor == branch.minor
+        return False
```

### Comparing `eos_downloader-0.8.0/eos_downloader/object_downloader.py` & `eos_downloader-0.8.1.dev1/eos_downloader/object_downloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,22 +5,21 @@
 # pylint: disable=too-many-arguments
 
 """
 eos_downloader class definition
 """
 
 from __future__ import (absolute_import, division, print_function,
-                        unicode_literals)
+                        unicode_literals, annotations)
 
 import base64
 import glob
 import hashlib
 import json
 import os
-# from builtins import *
 import sys
 import xml.etree.ElementTree as ET
 from typing import Union
 
 import requests
 import rich
 from loguru import logger
@@ -29,14 +28,16 @@
 
 from eos_downloader import (ARISTA_DOWNLOAD_URL, ARISTA_GET_SESSION,
                             ARISTA_SOFTWARE_FOLDER_TREE, EVE_QEMU_FOLDER_PATH,
                             MSG_INVALID_DATA, MSG_TOKEN_EXPIRED)
 from eos_downloader.data import DATA_MAPPING
 from eos_downloader.download import DownloadProgressBar
 
+# logger = logging.getLogger(__name__)
+
 console = rich.get_console()
 
 
 class ObjectDownloader():
     """
     ObjectDownloader Generic Object to download from Arista.com
     """
@@ -70,14 +71,17 @@
         self.timeout = 5
         # Logging
         logger.debug(f'Filename built by _build_filename is {self.filename}')
 
     def __str__(self) -> str:
         return f'{self.software} - {self.image} - {self.version}'
 
+    # def __repr__(self):
+    #     return str(self.__dict__)
+
     @property
     def version(self) -> str:
         """Get version."""
         return self._version
 
     @version.setter
     def version(self, value: str) -> None:
@@ -94,19 +98,22 @@
         _build_filename Helper to build filename to search on arista.com
 
         Returns
         -------
         str:
             Filename to search for on Arista.com
         """
+        logger.info('start build')
         if self.software in DATA_MAPPING:
+            logger.info(f'software in data mapping: {self.software}')
             if self.image in DATA_MAPPING[self.software]:
+                logger.info(f'image in data mapping: {self.image}')
                 return f"{DATA_MAPPING[self.software][self.image]['prepend']}-{self.version}{DATA_MAPPING[self.software][self.image]['extension']}"
             return f"{DATA_MAPPING[self.software]['default']['prepend']}-{self.version}{DATA_MAPPING[self.software]['default']['extension']}"
-        return ''
+        raise ValueError(f'Incorrect value for software {self.software}')
 
     def _parse_xml_for_path(self, root_xml: ET.ElementTree, xpath: str, search_file: str) -> str:
         # sourcery skip: remove-unnecessary-cast
         """
         _parse_xml Read and extract data from XML using XPATH
 
         Get all interested nodes using XPATH and then get node that match search_file
@@ -129,17 +136,17 @@
         logger.debug(f'Search for file {search_file}')
         console.print(f'🔎  Searching file {search_file}')
         for node in root_xml.findall(xpath):
             # logger.debug('Found {}', node.text)
             if str(node.text).lower() == search_file.lower():
                 path = node.get('path')
                 console.print(f'    -> Found file at {path}')
-                logger.info('Found {} at {}', node.text, node.get('path'))
+                logger.info(f'Found {node.text} at {node.get("path")}')
                 return str(node.get('path')) if node.get('path') is not None else ''
-        logger.error('Requested file ({}) not found !', self.filename)
+        logger.error(f'Requested file ({self.filename}) not found !')
         return ''
 
     def _get_hash(self, file_path: str) -> str:
         """
         _get_hash Download HASH file from Arista server
 
         Parameters
@@ -182,19 +189,17 @@
         bool
             True if both are equal, False if not
         """
         hash_md5 = hashlib.md5()
         with open(file, "rb") as f:
             for chunk in iter(lambda: f.read(4096), b""):
                 hash_md5.update(chunk)
-        if str(hash_md5.hexdigest()) == hash_expected:
+        if hash_md5.hexdigest() == hash_expected:
             return True
-        logger.warning('Downloaded file is corrupt: local md5 ({}) is different to md5 from arista ({})',
-                       hash_md5.hexdigest(),
-                       hash_expected)
+        logger.warning(f'Downloaded file is corrupt: local md5 ({hash_md5.hexdigest()}) is different to md5 from arista ({hash_expected})')
         return False
 
     @staticmethod
     def _compute_hash_sh512sum(file: str, hash_expected: str) -> bool:
         """
         _compute_hash_sh512sum Compare SHA512 sum
 
@@ -212,19 +217,17 @@
         bool
             True if both are equal, False if not
         """
         hash_sha512 = hashlib.sha512()
         with open(file, "rb") as f:
             for chunk in iter(lambda: f.read(4096), b""):
                 hash_sha512.update(chunk)
-        if str(hash_sha512.hexdigest()) == hash_expected:
+        if hash_sha512.hexdigest() == hash_expected:
             return True
-        logger.warning('Downloaded file is corrupt: local sha512 ({}) is different to sha512 from arista ({})',
-                       hash_sha512.hexdigest(),
-                       hash_expected)
+        logger.warning(f'Downloaded file is corrupt: local sha512 ({hash_sha512.hexdigest()}) is different to sha512 from arista ({hash_expected})')
         return False
 
     def _get_folder_tree(self) -> ET.ElementTree:
         """
         _get_folder_tree Download XML tree from Arista server
 
         Returns
@@ -300,15 +303,15 @@
         if self.session_id is None:
             self.authenticate()
         jsonpost = {'sessionCode': self.session_id, 'filePath': remote_file_path}
         result = requests.post(ARISTA_DOWNLOAD_URL, data=json.dumps(jsonpost), timeout=self.timeout)
         if 'data' in result.json() and 'url' in result.json()['data']:
             # logger.debug('URL to download file is: {}', result.json())
             return result.json()["data"]["url"]
-        logger.critical('Server returns following message: {}', result.json())
+        logger.critical(f'Server returns following message: {result.json()}')
         return ''
 
     @staticmethod
     def _download_file_raw(url: str, file_path: str) -> str:
         """
         _download_file Helper to download file from Arista.com
 
@@ -334,23 +337,23 @@
                 if chunk:
                     pbar.update(len(chunk))
                 f.write(chunk)
         return file_path
 
     def _download_file(self, file_path: str, filename: str, rich_interface: bool = True) -> Union[None, str]:
         remote_file_path = self._get_remote_filepath()
-        logger.info('File found on arista server: {}', remote_file_path)
+        logger.info(f'File found on arista server: {remote_file_path}')
         file_url = self._get_url(remote_file_path=remote_file_path)
         if file_url is not False:
             if not rich_interface:
                 return self._download_file_raw(url=file_url, file_path=os.path.join(file_path, filename))
             rich_downloader = DownloadProgressBar()
             rich_downloader.download(urls=[file_url], dest_dir=file_path)
             return os.path.join(file_path, filename)
-        logger.error('Cannot download file {}', file_path)
+        logger.error(f'Cannot download file {file_path}')
         return None
 
     @staticmethod
     def _create_destination_folder(path: str) -> None:
         # os.makedirs(path, mode, exist_ok=True)
         os.system(f'mkdir -p {path}')
```

### Comparing `eos_downloader-0.8.0/eos_downloader.egg-info/PKG-INFO` & `eos_downloader-0.8.1.dev1/eos_downloader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eos-downloader
-Version: 0.8.0
+Version: 0.8.1.dev1
 Summary: Arista EOS/CVP downloader script
 Author-email: Thomas Grimonet <thomas.grimonet@gmail.com>
 Maintainer-email: Thomas Grimonet <thomas.grimonet@gmail.com>
 License: Copyright (c) 2019, Arista Networks
         All rights reserved.
         
                                          Apache License
@@ -230,15 +230,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
- [![code-testing](https://github.com/titom73/eos-downloader/actions/workflows/pr-management.yml/badge.svg?event=push)](https://github.com/titom73/eos-downloader/actions/workflows/pr-management.yml) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/eos-downloader) ![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/titom73/arista-downloader) ![PyPI - Downloads](https://img.shields.io/pypi/dm/eos-downloader) ![Docker Image Size (tag)](https://img.shields.io/docker/image-size/titom73/eos-downloader/edge)
+ [![code-testing](https://github.com/titom73/eos-downloader/actions/workflows/pr-management.yml/badge.svg?event=push)](https://github.com/titom73/eos-downloader/actions/workflows/pr-management.yml) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/eos-downloader) ![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/titom73/arista-downloader) ![PyPI - Downloads/month](https://img.shields.io/pypi/dm/eos-downloader) ![Docker Image Size (tag)](https://img.shields.io/docker/image-size/titom73/eos-downloader/edge)
 
 # Arista Software Downloader
 
 Script to download Arista softwares to local folder, Cloudvision or EVE-NG.
 
 ```bash
 pip install eos-downloader
```

### Comparing `eos_downloader-0.8.0/eos_downloader.egg-info/SOURCES.txt` & `eos_downloader-0.8.1.dev1/eos_downloader.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 pyproject.toml
 eos_downloader/__init__.py
 eos_downloader/cvp.py
 eos_downloader/data.py
 eos_downloader/download.py
 eos_downloader/eos.py
 eos_downloader/object_downloader.py
+eos_downloader/tools.py
 eos_downloader.egg-info/PKG-INFO
 eos_downloader.egg-info/SOURCES.txt
 eos_downloader.egg-info/dependency_links.txt
 eos_downloader.egg-info/entry_points.txt
 eos_downloader.egg-info/requires.txt
 eos_downloader.egg-info/top_level.txt
 eos_downloader/cli/__init__.py
```

### Comparing `eos_downloader-0.8.0/pyproject.toml` & `eos_downloader-0.8.1.dev1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=64.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "eos_downloader"
-version = "v0.8.0"
+version = "v0.8.1-dev1"
 readme = "README.md"
 authors = [{ name = "Thomas Grimonet", email = "thomas.grimonet@gmail.com" }]
 maintainers = [
   { name = "Thomas Grimonet", email = "thomas.grimonet@gmail.com" },
 ]
 description = "Arista EOS/CVP downloader script"
 license = { file = "LICENSE" }
@@ -144,15 +144,15 @@
   3.9: py39
   3.10: py310, lint, type, coverage
 
 [testenv]
 description = run the test driver with {basepython}
 extras = dev
 commands =
-   pytest  {tty:--color=yes}
+   pytest -rA -q --cov-report term:skip-covered --cov-report term:skip-covered --html=report.html --self-contained-html --cov-report=html --color yes --cov=eos_downloader
 
 [testenv:lint]
 description = check the code style
 commands =
   flake8 --max-line-length=165 --config=/dev/null eos_downloader
   pylint eos_downloader
 
@@ -172,15 +172,15 @@
 # add the following to make the report fail under some percentage
 # commands = coverage report --fail-under=80
 depends = py310
 
 """
 
 [tool.pytest.ini_options]
-addopts = "-ra -q -s -vv --capture=tee-sys --ignore=tests/scripts --cov --cov-append"
+addopts = "-ra -q -s -vv --capture=tee-sys --cov --cov-append"
 log_level = "INFO"
 log_cli = "True"
 
 [tool.coverage.run]
 source = ['eos_downloader']
 # omit = []
```

