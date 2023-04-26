# Comparing `tmp/declarative_argparse-0.0.5.tar.gz` & `tmp/declarative_argparse-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "declarative_argparse-0.0.5.tar", max compression
+gzip compressed data, was "declarative_argparse-0.0.6.tar", max compression
```

## Comparing `declarative_argparse-0.0.5.tar` & `declarative_argparse-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0     1072 2023-01-11 06:04:32.924578 declarative_argparse-0.0.5/LICENSE
--rw-r--r--   0        0        0     1089 2023-01-11 06:05:50.200137 declarative_argparse-0.0.5/README.md
--rw-r--r--   0        0        0     4113 2022-06-16 23:14:01.159307 declarative_argparse-0.0.5/declarative_argparse/__init__.py
--rw-r--r--   0        0        0        0 2022-06-01 23:15:42.706503 declarative_argparse-0.0.5/declarative_argparse/options/__init__.py
--rw-r--r--   0        0        0     4391 2022-06-16 22:56:58.844790 declarative_argparse-0.0.5/declarative_argparse/options/abc.py
--rw-r--r--   0        0        0      662 2022-06-15 23:32:48.744143 declarative_argparse-0.0.5/declarative_argparse/options/bool.py
--rw-r--r--   0        0        0      670 2022-06-02 00:13:46.999859 declarative_argparse-0.0.5/declarative_argparse/options/float.py
--rw-r--r--   0        0        0      654 2022-06-02 00:13:51.719829 declarative_argparse-0.0.5/declarative_argparse/options/int.py
--rw-r--r--   0        0        0     1020 2022-06-16 23:11:20.432204 declarative_argparse-0.0.5/declarative_argparse/options/stores.py
--rw-r--r--   0        0        0      654 2022-06-02 00:14:24.511623 declarative_argparse-0.0.5/declarative_argparse/options/str.py
--rw-r--r--   0        0        0      561 2023-01-11 06:03:19.509000 declarative_argparse-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1819 1970-01-01 00:00:00.000000 declarative_argparse-0.0.5/setup.py
--rw-r--r--   0        0        0     1764 1970-01-01 00:00:00.000000 declarative_argparse-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-01-11 06:04:32.924578 declarative_argparse-0.0.6/LICENSE
+-rw-r--r--   0        0        0     1089 2023-01-11 06:05:50.200137 declarative_argparse-0.0.6/README.md
+-rw-r--r--   0        0        0     4653 2023-04-26 04:47:36.662095 declarative_argparse-0.0.6/declarative_argparse/__init__.py
+-rw-r--r--   0        0        0        0 2022-06-01 23:15:42.706503 declarative_argparse-0.0.6/declarative_argparse/options/__init__.py
+-rw-r--r--   0        0        0     4391 2023-01-30 05:14:40.435771 declarative_argparse-0.0.6/declarative_argparse/options/abc.py
+-rw-r--r--   0        0        0      662 2022-06-15 23:32:48.744143 declarative_argparse-0.0.6/declarative_argparse/options/bool.py
+-rw-r--r--   0        0        0      670 2022-06-02 00:13:46.999859 declarative_argparse-0.0.6/declarative_argparse/options/float.py
+-rw-r--r--   0        0        0      654 2022-06-02 00:13:51.719829 declarative_argparse-0.0.6/declarative_argparse/options/int.py
+-rw-r--r--   0        0        0     2096 2023-04-26 04:45:28.570788 declarative_argparse-0.0.6/declarative_argparse/options/path.py
+-rw-r--r--   0        0        0     1020 2022-06-16 23:11:20.432204 declarative_argparse-0.0.6/declarative_argparse/options/stores.py
+-rw-r--r--   0        0        0      654 2023-04-26 04:41:24.720174 declarative_argparse-0.0.6/declarative_argparse/options/str.py
+-rw-r--r--   0        0        0      689 2023-04-26 04:38:11.505362 declarative_argparse-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1819 1970-01-01 00:00:00.000000 declarative_argparse-0.0.6/setup.py
+-rw-r--r--   0        0        0     1764 1970-01-01 00:00:00.000000 declarative_argparse-0.0.6/PKG-INFO
```

### Comparing `declarative_argparse-0.0.5/LICENSE` & `declarative_argparse-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `declarative_argparse-0.0.5/README.md` & `declarative_argparse-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `declarative_argparse-0.0.5/declarative_argparse/__init__.py` & `declarative_argparse-0.0.6/declarative_argparse/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,18 +3,20 @@
 import argparse
 from typing import Dict, List, Optional, Sequence, Type, cast
 
 from declarative_argparse.options.abc import IDeclarativeOption
 from declarative_argparse.options.bool import BoolArrayDO, BoolDO
 from declarative_argparse.options.float import FloatArrayDO, FloatDO
 from declarative_argparse.options.int import IntArrayDO, IntDO
+from declarative_argparse.options.path import PathArrayDO, PathDO
 from declarative_argparse.options.stores import StoreFalseDO, StoreTrueDO
 from declarative_argparse.options.str import StrArrayDO, StrDO
 
-__version__ = '0.0.4'
+__version__ = '0.0.6'
+
 __all__ = [
     'BoolArrayDO',
     'BoolDO',
     'DeclarativeOptionParser',
     'FloatArrayDO',
     'FloatDO',
     'IntArrayDO',
@@ -28,15 +30,15 @@
 
 class DeclarativeOptionParser:
     def __init__(self, argp: Optional[argparse.ArgumentParser]) -> None:
         self.argp = argp or argparse.ArgumentParser()
         self.allOpts: List[IDeclarativeOption] = []
         self.allOptsByID: Dict[str, IDeclarativeOption] = {}
 
-        #self.verbose: BoolDO = self.addBool('quiet', 'q', 'Removes verbosity of output')
+        # self.verbose: BoolDO = self.addBool('quiet', 'q', 'Removes verbosity of output')
     def bindToNamespace(self, args: argparse.Namespace) -> None:
         [x._bindToNamespace(args) for x in self.allOpts]
 
     def parseArguments(self, args: Optional[Sequence[str]] = None) -> None:
         for arg in self.allOpts:
             arg.add_to_argparser(self.argp)
         self.bindToNamespace(self.argp.parse_args(args))
@@ -99,7 +101,18 @@
         return cast(StrDO, self.add(StrDO, *flags, description=description))
 
     def addStrArray(self,
                     *flags: List[str],
                     nargs: str,
                     description: Optional[str] = None) -> StrArrayDO:
         return cast(StrArrayDO, self.add(StrArrayDO, *flags, description=description)).setNArgs(nargs)
+
+    def addPath(self,
+               *flags: List[str],
+               description: Optional[str] = None) -> PathDO:
+        return cast(PathDO, self.add(PathDO, *flags, description=description))
+
+    def addPathArray(self,
+                    *flags: List[str],
+                    nargs: str,
+                    description: Optional[str] = None) -> PathArrayDO:
+        return cast(PathArrayDO, self.add(PathArrayDO, *flags, description=description)).setNArgs(nargs)
```

### Comparing `declarative_argparse-0.0.5/declarative_argparse/options/abc.py` & `declarative_argparse-0.0.6/declarative_argparse/options/abc.py`

 * *Files identical despite different names*

### Comparing `declarative_argparse-0.0.5/declarative_argparse/options/bool.py` & `declarative_argparse-0.0.6/declarative_argparse/options/bool.py`

 * *Files identical despite different names*

### Comparing `declarative_argparse-0.0.5/declarative_argparse/options/float.py` & `declarative_argparse-0.0.6/declarative_argparse/options/float.py`

 * *Files identical despite different names*

### Comparing `declarative_argparse-0.0.5/declarative_argparse/options/int.py` & `declarative_argparse-0.0.6/declarative_argparse/options/int.py`

 * *Files identical despite different names*

### Comparing `declarative_argparse-0.0.5/declarative_argparse/options/stores.py` & `declarative_argparse-0.0.6/declarative_argparse/options/stores.py`

 * *Files identical despite different names*

### Comparing `declarative_argparse-0.0.5/declarative_argparse/options/str.py` & `declarative_argparse-0.0.6/declarative_argparse/options/str.py`

 * *Files identical despite different names*

### Comparing `declarative_argparse-0.0.5/pyproject.toml` & `declarative_argparse-0.0.6/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 [tool.poetry]
 name = "declarative_argparse"
-version = "0.0.5"
+version = "0.0.6"
 description = "A simple wrapper around argparse to permit declarative construction and argument retrieval."
 authors = ["Rob Nelson <nexisentertainment@gmail.com>"]
 readme="README.md"
 repository="https://gitlab.com/N3X15/declarative_argparse"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.2.0"
-mypy = "^0.991"
-autopep8 = "^2.0.1"
-isort = "^5.11.4"
+pytest = "^7.3.1"
+mypy = "^1.2.0"
+autopep8 = "^2.0.2"
+isort = "^5.12.0"
 twine = "^4.0.2"
 
+[tool.poetry.group.dev.dependencies]
+mypy = {extras = ["d"], version = "^1.2.0"}
+black = {extras = ["d"], version = "^23.3.0"}
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `declarative_argparse-0.0.5/setup.py` & `declarative_argparse-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['declarative_argparse', 'declarative_argparse.options']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'declarative-argparse',
-    'version': '0.0.5',
+    'version': '0.0.6',
     'description': 'A simple wrapper around argparse to permit declarative construction and argument retrieval.',
     'long_description': "# Declarative Argparse\n\nThis project introduces a wrapper argound the built-in `argparse` module that permits one to make a declarative parser for options.\n\n[[_TOC_]]\n\n## Example\n\n```python\nimport argparse\nfrom declarative_argparse import DeclarativeOptionParser\nfrom declarative_argparse.options.int import IntDO\nfrom declarative_argparse.options.str import StrDO\nclass DAPExample(DeclarativeOptionParser):\n    def __init__(self) -> None:\n        super().__init__(argp=argparse.ArgumentParser())\n        self.x: IntDO = self.addInt('--x', '-x', description='X coordinate')\n        self.y: IntDO = self.addInt('--y', '-y', description='Y coordinate')\n        self.name: StrDO = self.addStr('--name', description='Change tile name').setNArgs('?')\n        self.id: StrDO = self.addStr('id', description='specify tile ID')\n\n# ...\n\nargs = DAPExample()\nargs.parseArguments(['--x=0', '-y', '1', 'abc1'])\nassert args.x.get_value() == 0\nassert args.y.get_value() == 1\nassert args.name.get_value() is None\nassert args.id.get_value() == 'abc1'\n```\n\n## License\n\nMIT\n\nContributions are always welcome.",
     'author': 'Rob Nelson',
     'author_email': 'nexisentertainment@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://gitlab.com/N3X15/declarative_argparse',
```

### Comparing `declarative_argparse-0.0.5/PKG-INFO` & `declarative_argparse-0.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: declarative-argparse
-Version: 0.0.5
+Version: 0.0.6
 Summary: A simple wrapper around argparse to permit declarative construction and argument retrieval.
 Home-page: https://gitlab.com/N3X15/declarative_argparse
 Author: Rob Nelson
 Author-email: nexisentertainment@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

