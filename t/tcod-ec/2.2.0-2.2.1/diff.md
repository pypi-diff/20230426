# Comparing `tmp/tcod-ec-2.2.0.tar.gz` & `tmp/tcod-ec-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tcod-ec-2.2.0.tar", last modified: Wed Mar 22 00:56:54 2023, max compression
+gzip compressed data, was "tcod-ec-2.2.1.tar", last modified: Wed Apr 26 21:54:05 2023, max compression
```

## Comparing `tcod-ec-2.2.0.tar` & `tcod-ec-2.2.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      110 2022-12-09 23:27:48.971884 tcod-ec-2.2.0/.flake8
--rw-r--r--   0        0        0     2450 2022-12-09 22:01:20.751676 tcod-ec-2.2.0/.gitattributes
--rw-r--r--   0        0        0      188 2022-12-07 02:28:46.295094 tcod-ec-2.2.0/.github/FUNDING.yml
--rw-r--r--   0        0        0     1536 2023-01-05 04:25:13.030030 tcod-ec-2.2.0/.github/workflows/python-package.yml
--rw-r--r--   0        0        0     4357 2022-12-09 22:01:22.138004 tcod-ec-2.2.0/.gitignore
--rw-r--r--   0        0        0     1324 2023-01-05 05:28:02.835000 tcod-ec-2.2.0/.vscode/launch.json
--rw-r--r--   0        0        0     1452 2023-03-18 22:22:07.261134 tcod-ec-2.2.0/.vscode/settings.json
--rw-r--r--   0        0        0     1237 2023-01-05 05:27:39.701584 tcod-ec-2.2.0/.vscode/tasks.json
--rw-r--r--   0        0        0     1791 2023-03-22 00:18:16.654552 tcod-ec-2.2.0/CHANGELOG.md
--rw-r--r--   0        0        0     1100 2023-01-04 05:48:36.113939 tcod-ec-2.2.0/LICENSE
--rw-r--r--   0        0        0     4718 2023-03-18 22:28:28.989146 tcod-ec-2.2.0/README.md
--rw-r--r--   0        0        0      634 2022-12-10 22:58:25.072843 tcod-ec-2.2.0/docs/Makefile
--rw-r--r--   0        0        0      114 2023-01-06 20:04:17.700637 tcod-ec-2.2.0/docs/api.rst
--rw-r--r--   0        0        0     2044 2023-01-06 20:03:54.860093 tcod-ec-2.2.0/docs/conf.py
--rw-r--r--   0        0        0       32 2022-12-10 23:30:30.594162 tcod-ec-2.2.0/docs/head.md
--rw-r--r--   0        0        0      255 2023-01-06 20:05:00.073778 tcod-ec-2.2.0/docs/index.rst
--rwxr-xr-x   0        0        0      800 2022-12-10 22:58:25.073843 tcod-ec-2.2.0/docs/make.bat
--rw-r--r--   0        0        0       53 2023-01-06 20:15:12.123667 tcod-ec-2.2.0/docs/requirements.txt
--rw-r--r--   0        0        0     3403 2023-03-21 19:57:13.143403 tcod-ec-2.2.0/pyproject.toml
--rw-r--r--   0        0        0    19888 2023-03-22 00:17:56.820392 tcod-ec-2.2.0/tcod/ec/__init__.py
--rw-r--r--   0        0        0        0 2023-01-06 07:57:43.433195 tcod-ec-2.2.0/tcod/ec/py.typed
--rw-r--r--   0        0        0     7484 2023-03-17 06:36:21.430935 tcod-ec-2.2.0/tcod/ec/test_ec.py
--rw-r--r--   0        0        0     5732 1970-01-01 00:00:00.000000 tcod-ec-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0      110 2022-12-09 23:27:48.971884 tcod-ec-2.2.1/.flake8
+-rw-r--r--   0        0        0     2450 2022-12-09 22:01:20.751676 tcod-ec-2.2.1/.gitattributes
+-rw-r--r--   0        0        0      188 2022-12-07 02:28:46.295094 tcod-ec-2.2.1/.github/FUNDING.yml
+-rw-r--r--   0        0        0     1536 2023-01-05 04:25:13.030030 tcod-ec-2.2.1/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0     4357 2022-12-09 22:01:22.138004 tcod-ec-2.2.1/.gitignore
+-rw-r--r--   0        0        0     1324 2023-01-05 05:28:02.835000 tcod-ec-2.2.1/.vscode/launch.json
+-rw-r--r--   0        0        0     1475 2023-04-26 21:37:33.240299 tcod-ec-2.2.1/.vscode/settings.json
+-rw-r--r--   0        0        0     1237 2023-01-05 05:27:39.701584 tcod-ec-2.2.1/.vscode/tasks.json
+-rw-r--r--   0        0        0     1914 2023-04-26 21:49:44.912422 tcod-ec-2.2.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1100 2023-01-04 05:48:36.113939 tcod-ec-2.2.1/LICENSE
+-rw-r--r--   0        0        0     4718 2023-03-18 22:28:28.989146 tcod-ec-2.2.1/README.md
+-rw-r--r--   0        0        0      634 2022-12-10 22:58:25.072843 tcod-ec-2.2.1/docs/Makefile
+-rw-r--r--   0        0        0      114 2023-01-06 20:04:17.700637 tcod-ec-2.2.1/docs/api.rst
+-rw-r--r--   0        0        0     2044 2023-01-06 20:03:54.860093 tcod-ec-2.2.1/docs/conf.py
+-rw-r--r--   0        0        0       32 2022-12-10 23:30:30.594162 tcod-ec-2.2.1/docs/head.md
+-rw-r--r--   0        0        0      255 2023-01-06 20:05:00.073778 tcod-ec-2.2.1/docs/index.rst
+-rwxr-xr-x   0        0        0      800 2022-12-10 22:58:25.073843 tcod-ec-2.2.1/docs/make.bat
+-rw-r--r--   0        0        0       53 2023-01-06 20:15:12.123667 tcod-ec-2.2.1/docs/requirements.txt
+-rw-r--r--   0        0        0     3403 2023-03-21 19:57:13.143403 tcod-ec-2.2.1/pyproject.toml
+-rw-r--r--   0        0        0    20632 2023-04-26 21:47:56.463855 tcod-ec-2.2.1/tcod/ec/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-06 07:57:43.433195 tcod-ec-2.2.1/tcod/ec/py.typed
+-rw-r--r--   0        0        0     7489 2023-04-26 21:38:18.709993 tcod-ec-2.2.1/tcod/ec/test_ec.py
+-rw-r--r--   0        0        0     5732 1970-01-01 00:00:00.000000 tcod-ec-2.2.1/PKG-INFO
```

### Comparing `tcod-ec-2.2.0/.gitattributes` & `tcod-ec-2.2.1/.gitattributes`

 * *Files identical despite different names*

### Comparing `tcod-ec-2.2.0/.github/workflows/python-package.yml` & `tcod-ec-2.2.1/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `tcod-ec-2.2.0/.gitignore` & `tcod-ec-2.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `tcod-ec-2.2.0/.vscode/launch.json` & `tcod-ec-2.2.1/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `tcod-ec-2.2.0/.vscode/settings.json` & `tcod-ec-2.2.1/.vscode/settings.json`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
         "PAGEDOWN",
         "PAGEUP",
         "pytest",
         "quickstart",
         "RMASK",
         "rtype",
         "scancode",
+        "setdefault",
         "tcod",
         "toctree",
         "typehints",
         "undoc",
         "unpickle",
         "WASD",
         "WAXD",
```

### Comparing `tcod-ec-2.2.0/.vscode/tasks.json` & `tcod-ec-2.2.1/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `tcod-ec-2.2.0/CHANGELOG.md` & `tcod-ec-2.2.1/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [2.2.1] - 2023-04-26
+### Fixed
+- Corrected the type-hinting of `ComponentDict.get` and `ComponentDict.setdefault`.
+
 ## [2.2.0] - 2023-03-21
 ### Added
 - `ComponentDict` is now a `MutableMapping` subclass.
   It can now do everything expected of a dict-like object, such as the `.values()` method.
   Keep in mind it still uses identity comparison.
 - Added local component observers to `ComponentDict`.
```

### Comparing `tcod-ec-2.2.0/LICENSE` & `tcod-ec-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tcod-ec-2.2.0/README.md` & `tcod-ec-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `tcod-ec-2.2.0/docs/Makefile` & `tcod-ec-2.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tcod-ec-2.2.0/docs/conf.py` & `tcod-ec-2.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tcod-ec-2.2.0/docs/make.bat` & `tcod-ec-2.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `tcod-ec-2.2.0/pyproject.toml` & `tcod-ec-2.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tcod-ec-2.2.0/tcod/ec/__init__.py` & `tcod-ec-2.2.1/tcod/ec/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 """Entity/Component containers for implementing composition over inheritance.
 
 Unlike with ECS, these containers are standalone.
 This makes them simpler to use but they have fewer features.
 """
 from __future__ import annotations
 
-__version__ = "2.2.0"
+__version__ = "2.2.1"
 
 import reprlib
 from typing import (
+    TYPE_CHECKING,
     Any,
     Callable,
     ClassVar,
     DefaultDict,
     Iterable,
     Iterator,
     MutableMapping,
     Optional,
     Sequence,
     Type,
     TypeVar,
+    overload,
 )
 
 from typing_extensions import Self
 
 T = TypeVar("T")
 
 
@@ -341,14 +343,32 @@
     def __repr__(self) -> str:
         """Return the representation of this ComponentDict."""
         params = [f"[{', '.join(repr(component) for component in self._components.values())}]"]
         if self.observers:
             params.append(f"observers={self.observers!r}")
         return f"{self.__class__.__name__}({', '.join(params)})"
 
+    if TYPE_CHECKING:
+
+        @overload
+        def get(self, __key: type[T]) -> T | None:
+            ...
+
+        @overload
+        def get(self, __key: type[T], __default: T) -> T:
+            ...
+
+        def get(self, __key: type[T], __default: T | None = None) -> T | None:
+            """Return a component, returns None or a default value when the component is missing."""
+            # Type-hinted get override.
+
+        def setdefault(self, __key: type[T], __default: T) -> T:  # type: ignore[override]
+            """Assign a default value if a component is missing, then returns the current value."""
+            # Type-hinted setdefault override, None is not a valid default.
+
 
 class Composite:
     """A collection of multiple components organized by their inheritance tree.
 
     Allows multiple components for the same class and allows accessing components using a shared parent class.
 
     The order of components is preserved.
```

### Comparing `tcod-ec-2.2.0/tcod/ec/test_ec.py` & `tcod-ec-2.2.1/tcod/ec/test_ec.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import Iterable, TypeVar
 
 import attrs
 import pytest
 
 import tcod.ec
 
-# ruff: noqa: D100 D101 D103 D107
+# ruff: noqa: D100 D101 D103 D107 S301
 
 T = TypeVar("T")
 
 
 class ComponentDictNode(tcod.ec.ComponentDict):
     """Complex subclass for testing pickle."""
```

### Comparing `tcod-ec-2.2.0/PKG-INFO` & `tcod-ec-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tcod-ec
-Version: 2.2.0
+Version: 2.2.1
 Summary: Entity/Component containers for implementing composition over inheritance.
 Author-email: Kyle Benesch <4b796c65+github@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

