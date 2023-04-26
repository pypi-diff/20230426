# Comparing `tmp/pyproject-parser-0.9.0b1.tar.gz` & `tmp/pyproject-parser-0.9.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyproject-parser-0.9.0b1.tar", last modified: Tue Apr 25 08:02:41 2023, max compression
+gzip compressed data, was "pyproject-parser-0.9.0b2.tar", last modified: Tue Apr 25 21:22:24 2023, max compression
```

## Comparing `pyproject-parser-0.9.0b1.tar` & `pyproject-parser-0.9.0b2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:02:41.654429 pyproject-parser-0.9.0b1/
--rw-r--r--   0 runner    (1001) docker     (122)     1064 2023-04-25 08:02:08.000000 pyproject-parser-0.9.0b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      160 2023-04-25 08:02:08.000000 pyproject-parser-0.9.0b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     8395 2023-04-25 08:02:41.654429 pyproject-parser-0.9.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5474 2023-04-25 08:02:08.000000 pyproject-parser-0.9.0b1/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)      383 2023-04-25 08:02:08.000000 pyproject-parser-0.9.0b1/__pkginfo__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5706 2023-04-25 08:02:08.000000 pyproject-parser-0.9.0b1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:02:41.650429 pyproject-parser-0.9.0b1/pyproject_parser/
--rw-r--r--   0 runner    (1001) docker     (122)    10945 2023-04-25 08:02:08.000000 pyproject-parser-0.9.0b1/pyproject_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9433 2023-04-25 08:02:08.000000 pyproject-parser-0.9.0b1/pyproject_parser/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10154 2023-04-25 08:02:08.000000 pyproject-parser-0.9.0b1/pyproject_parser/classes.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:02:41.650429 pyproject-parser-0.9.0b1/pyproject_parser/cli/
--rw-r--r--   0 runner    (1001) docker     (122)     6393 2023-04-25 08:02:08.000000 pyproject-parser-0.9.0b1/pyproject_parser/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2452 2023-04-25 08:02:08.000000 pyproject-parser-0.9.0b1/pyproject_parser/cli/_json_encoders.py
--rw-r--r--   0 runner    (1001) docker     (122)    35674 2023-04-25 08:02:08.000000 pyproject-parser-0.9.0b1/pyproject_parser/parsers.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-25 08:02:08.000000 pyproject-parser-0.9.0b1/pyproject_parser/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)     3778 2023-04-25 08:02:08.000000 pyproject-parser-0.9.0b1/pyproject_parser/type_hints.py
--rw-r--r--   0 runner    (1001) docker     (122)     5500 2023-04-25 08:02:08.000000 pyproject-parser-0.9.0b1/pyproject_parser/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:02:41.650429 pyproject-parser-0.9.0b1/pyproject_parser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     8395 2023-04-25 08:02:41.000000 pyproject-parser-0.9.0b1/pyproject_parser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      804 2023-04-25 08:02:41.000000 pyproject-parser-0.9.0b1/pyproject_parser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-25 08:02:41.000000 pyproject-parser-0.9.0b1/pyproject_parser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      217 2023-04-25 08:02:41.000000 pyproject-parser-0.9.0b1/pyproject_parser.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-25 08:02:41.000000 pyproject-parser-0.9.0b1/pyproject_parser.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      403 2023-04-25 08:02:41.000000 pyproject-parser-0.9.0b1/pyproject_parser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       17 2023-04-25 08:02:41.000000 pyproject-parser-0.9.0b1/pyproject_parser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      204 2023-04-25 08:02:08.000000 pyproject-parser-0.9.0b1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1746 2023-04-25 08:02:41.654429 pyproject-parser-0.9.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      648 2023-04-25 08:02:08.000000 pyproject-parser-0.9.0b1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:02:41.654429 pyproject-parser-0.9.0b1/tests/
--rw-r--r--   0 runner    (1001) docker     (122)    10428 2023-04-25 08:02:08.000000 pyproject-parser-0.9.0b1/tests/test_classes.py
--rw-r--r--   0 runner    (1001) docker     (122)    15102 2023-04-25 08:02:08.000000 pyproject-parser-0.9.0b1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (122)     3793 2023-04-25 08:02:08.000000 pyproject-parser-0.9.0b1/tests/test_cli_module.py
--rw-r--r--   0 runner    (1001) docker     (122)    12953 2023-04-25 08:02:08.000000 pyproject-parser-0.9.0b1/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (122)     5900 2023-04-25 08:02:08.000000 pyproject-parser-0.9.0b1/tests/test_dumping.py
--rw-r--r--   0 runner    (1001) docker     (122)     9107 2023-04-25 08:02:08.000000 pyproject-parser-0.9.0b1/tests/test_pyproject_class.py
--rw-r--r--   0 runner    (1001) docker     (122)     1859 2023-04-25 08:02:08.000000 pyproject-parser-0.9.0b1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 21:22:24.227481 pyproject-parser-0.9.0b2/
+-rw-r--r--   0 runner    (1001) docker     (122)     1064 2023-04-25 21:21:48.000000 pyproject-parser-0.9.0b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-04-25 21:21:48.000000 pyproject-parser-0.9.0b2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     8395 2023-04-25 21:22:24.227481 pyproject-parser-0.9.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5474 2023-04-25 21:21:48.000000 pyproject-parser-0.9.0b2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      383 2023-04-25 21:21:48.000000 pyproject-parser-0.9.0b2/__pkginfo__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5706 2023-04-25 21:21:48.000000 pyproject-parser-0.9.0b2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 21:22:24.223481 pyproject-parser-0.9.0b2/pyproject_parser/
+-rw-r--r--   0 runner    (1001) docker     (122)    10945 2023-04-25 21:21:48.000000 pyproject-parser-0.9.0b2/pyproject_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9433 2023-04-25 21:21:48.000000 pyproject-parser-0.9.0b2/pyproject_parser/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10154 2023-04-25 21:21:48.000000 pyproject-parser-0.9.0b2/pyproject_parser/classes.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 21:22:24.227481 pyproject-parser-0.9.0b2/pyproject_parser/cli/
+-rw-r--r--   0 runner    (1001) docker     (122)     6393 2023-04-25 21:21:48.000000 pyproject-parser-0.9.0b2/pyproject_parser/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2452 2023-04-25 21:21:48.000000 pyproject-parser-0.9.0b2/pyproject_parser/cli/_json_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36419 2023-04-25 21:21:48.000000 pyproject-parser-0.9.0b2/pyproject_parser/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-25 21:21:48.000000 pyproject-parser-0.9.0b2/pyproject_parser/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     3778 2023-04-25 21:21:48.000000 pyproject-parser-0.9.0b2/pyproject_parser/type_hints.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5500 2023-04-25 21:21:48.000000 pyproject-parser-0.9.0b2/pyproject_parser/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 21:22:24.223481 pyproject-parser-0.9.0b2/pyproject_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     8395 2023-04-25 21:22:24.000000 pyproject-parser-0.9.0b2/pyproject_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      804 2023-04-25 21:22:24.000000 pyproject-parser-0.9.0b2/pyproject_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-25 21:22:24.000000 pyproject-parser-0.9.0b2/pyproject_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      217 2023-04-25 21:22:24.000000 pyproject-parser-0.9.0b2/pyproject_parser.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-25 21:22:24.000000 pyproject-parser-0.9.0b2/pyproject_parser.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      403 2023-04-25 21:22:24.000000 pyproject-parser-0.9.0b2/pyproject_parser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-04-25 21:22:24.000000 pyproject-parser-0.9.0b2/pyproject_parser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      204 2023-04-25 21:21:48.000000 pyproject-parser-0.9.0b2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1746 2023-04-25 21:22:24.227481 pyproject-parser-0.9.0b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      648 2023-04-25 21:21:48.000000 pyproject-parser-0.9.0b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 21:22:24.227481 pyproject-parser-0.9.0b2/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)    10428 2023-04-25 21:21:48.000000 pyproject-parser-0.9.0b2/tests/test_classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15102 2023-04-25 21:21:48.000000 pyproject-parser-0.9.0b2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3793 2023-04-25 21:21:48.000000 pyproject-parser-0.9.0b2/tests/test_cli_module.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16879 2023-04-25 21:21:48.000000 pyproject-parser-0.9.0b2/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5900 2023-04-25 21:21:48.000000 pyproject-parser-0.9.0b2/tests/test_dumping.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9107 2023-04-25 21:21:48.000000 pyproject-parser-0.9.0b2/tests/test_pyproject_class.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1859 2023-04-25 21:21:48.000000 pyproject-parser-0.9.0b2/tests/test_utils.py
```

### Comparing `pyproject-parser-0.9.0b1/LICENSE` & `pyproject-parser-0.9.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyproject-parser-0.9.0b1/PKG-INFO` & `pyproject-parser-0.9.0b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyproject-parser
-Version: 0.9.0b1
+Version: 0.9.0b2
 Summary: Parser for 'pyproject.toml'
 Home-page: https://github.com/repo-helper/pyproject-parser
 Author: Dominic Davis-Foster
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 License: Copyright (c) 2021 Dominic Davis-Foster
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -156,15 +156,15 @@
 .. |license| image:: https://img.shields.io/github/license/repo-helper/pyproject-parser
 	:target: https://github.com/repo-helper/pyproject-parser/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/repo-helper/pyproject-parser
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/pyproject-parser/v0.9.0b1
+.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/pyproject-parser/v0.9.0b2
 	:target: https://github.com/repo-helper/pyproject-parser/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/repo-helper/pyproject-parser
 	:target: https://github.com/repo-helper/pyproject-parser/commit/master
 	:alt: GitHub last commit
```

### Comparing `pyproject-parser-0.9.0b1/README.rst` & `pyproject-parser-0.9.0b2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 .. |license| image:: https://img.shields.io/github/license/repo-helper/pyproject-parser
 	:target: https://github.com/repo-helper/pyproject-parser/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/repo-helper/pyproject-parser
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/pyproject-parser/v0.9.0b1
+.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/pyproject-parser/v0.9.0b2
 	:target: https://github.com/repo-helper/pyproject-parser/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/repo-helper/pyproject-parser
 	:target: https://github.com/repo-helper/pyproject-parser/commit/master
 	:alt: GitHub last commit
```

### Comparing `pyproject-parser-0.9.0b1/pyproject.toml` & `pyproject-parser-0.9.0b2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools!=61.*,>=40.6.0", "wheel>=0.34.2",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyproject-parser"
-version = "0.9.0b1"
+version = "0.9.0b2"
 description = "Parser for 'pyproject.toml'"
 readme = "README.rst"
 requires-python = ">=3.6.1"
 keywords = [ "metadata", "packaging", "pep518", "pep621", "pyproject", "toml",]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
```

### Comparing `pyproject-parser-0.9.0b1/pyproject_parser/__init__.py` & `pyproject-parser-0.9.0b2/pyproject_parser/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 		_PyProjectAsTomlDict
 		)
 from pyproject_parser.utils import _load_toml
 
 __author__: str = "Dominic Davis-Foster"
 __copyright__: str = "2021 Dominic Davis-Foster"
 __license__: str = "MIT License"
-__version__: str = "0.9.0b1"
+__version__: str = "0.9.0b2"
 __email__: str = "dominic@davis-foster.co.uk"
 
 __all__ = ["PyProject", "PyProjectTomlEncoder", "_PP"]
 
 _PP = TypeVar("_PP", bound="PyProject")
```

### Comparing `pyproject-parser-0.9.0b1/pyproject_parser/__main__.py` & `pyproject-parser-0.9.0b2/pyproject_parser/__main__.py`

 * *Files identical despite different names*

### Comparing `pyproject-parser-0.9.0b1/pyproject_parser/classes.py` & `pyproject-parser-0.9.0b2/pyproject_parser/classes.py`

 * *Files identical despite different names*

### Comparing `pyproject-parser-0.9.0b1/pyproject_parser/cli/__init__.py` & `pyproject-parser-0.9.0b2/pyproject_parser/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `pyproject-parser-0.9.0b1/pyproject_parser/cli/_json_encoders.py` & `pyproject-parser-0.9.0b2/pyproject_parser/cli/_json_encoders.py`

 * *Files identical despite different names*

### Comparing `pyproject-parser-0.9.0b1/pyproject_parser/parsers.py` & `pyproject-parser-0.9.0b2/pyproject_parser/parsers.py`

 * *Files 4% similar despite different names*

```diff
@@ -151,14 +151,24 @@
 
 	table_name: ClassVar[str] = "build-system"
 	required_keys: ClassVar[List[str]] = ["requires"]
 	keys: ClassVar[List[str]] = ["requires", "build-backend", "backend-path"]
 	factories: ClassVar[Dict[str, Callable[..., Any]]] = {"requires": list}
 	defaults: ClassVar[Dict[str, Any]] = {"build-backend": None, "backend-path": None}
 
+	@staticmethod
+	def normalize_requirement_name(name: str) -> str:
+		"""
+		Function to normalize a requirement name per e.g. :pep:`503` (where underscores are replaced by hyphens).
+
+		.. versionadded:: 0.9.0
+		"""
+
+		return normalize(name)
+
 	@_documentation_url("https://peps.python.org/pep-0518/")
 	def parse_requires(self, config: Dict[str, TOML_TYPES]) -> List[ComparableRequirement]:
 		"""
 		Parse the :pep:`requires <518#build-system-table>` key.
 
 		:param config: The unparsed TOML config for the :pep:`build-system table <518#build-system-table>`.
 		"""  # noqa: RST399
@@ -177,15 +187,15 @@
 				e.args = (f"{raw_requirement!r}\n    {str(e)}", )
 				e.note = "requirements must follow PEP 508"  # type: ignore[attr-defined]
 				e.documentation = "https://peps.python.org/pep-0508/"  # type: ignore[attr-defined]
 				raise
 
 			parsed_dependencies.add(requirement)
 
-		return sorted(combine_requirements(parsed_dependencies))
+		return sorted(combine_requirements(parsed_dependencies, normalize_func=self.normalize_requirement_name))
 
 	@_documentation_url("https://peps.python.org/pep-0517/")
 	def parse_build_backend(self, config: Dict[str, TOML_TYPES]) -> str:
 		"""
 		Parse the ``build_backend`` key defined by :pep:`517`.
 
 		:param config: The unparsed TOML config for the :pep:`build-system table <518#build-system-table>`.
@@ -914,14 +924,24 @@
 						)
 
 			for name, func in sub_table.items():
 				self.assert_value_type(func, str, ["project", "entry-points", group, name])
 
 		return entry_points
 
+	@staticmethod
+	def normalize_requirement_name(name: str) -> str:
+		"""
+		Function to normalize a requirement name per e.g. :pep:`503` (where underscores are replaced by hyphens).
+
+		.. versionadded:: 0.9.0
+		"""
+
+		return normalize(name)
+
 	@_documentation_url("https://whey.readthedocs.io/en/latest/configuration.html#tconf-project.dependencies")
 	def parse_dependencies(self, config: Dict[str, TOML_TYPES]) -> List[ComparableRequirement]:
 		"""
 		Parse the :pep621:`dependencies` key, giving the dependencies of the project.
 
 		* **Format**: :toml:`Array` of :pep:`508` strings
 		* **Core Metadata**: :core-meta:`Requires-Dist`
@@ -958,15 +978,18 @@
 				e.args = (f"{raw_requirement!r}\n    {str(e)}", )
 				e.note = "requirements must follow PEP 508"  # type: ignore[attr-defined]
 				e.documentation = "https://peps.python.org/pep-0508/"  # type: ignore[attr-defined]
 				raise
 
 			parsed_dependencies.add(requirement)
 
-		return sorted(combine_requirements(parsed_dependencies))
+		return sorted(combine_requirements(
+				parsed_dependencies,
+				normalize_func=self.normalize_requirement_name,
+				))
 
 	@_documentation_url(
 			"https://whey.readthedocs.io/en/latest/configuration.html#tconf-project.optional-dependencies"
 			)
 	def parse_optional_dependencies(
 			self,
 			config: Dict[str, TOML_TYPES],
@@ -1064,15 +1087,21 @@
 					parsed_optional_dependencies[extra].add(requirement)
 				else:
 					raise TypeError(
 							f"Invalid type for 'project.optional-dependencies.{extra}[{idx}]': "
 							f"expected {str!r}, got {type(dep)!r}"
 							)
 
-		return {e: sorted(combine_requirements(d)) for e, d in parsed_optional_dependencies.items()}
+		combined_requirements = {}
+		for extra, deps in parsed_optional_dependencies.items():
+			combined_requirements[extra] = sorted(
+					combine_requirements(deps, normalize_func=self.normalize_requirement_name)
+					)
+
+		return combined_requirements
 
 	def parse(  # type: ignore[override]
 		self,
 		config: Dict[str, TOML_TYPES],
 		set_defaults: bool = False,
 		) -> ProjectDict:
 		"""
```

### Comparing `pyproject-parser-0.9.0b1/pyproject_parser/type_hints.py` & `pyproject-parser-0.9.0b2/pyproject_parser/type_hints.py`

 * *Files identical despite different names*

### Comparing `pyproject-parser-0.9.0b1/pyproject_parser/utils.py` & `pyproject-parser-0.9.0b2/pyproject_parser/utils.py`

 * *Files identical despite different names*

### Comparing `pyproject-parser-0.9.0b1/pyproject_parser.egg-info/PKG-INFO` & `pyproject-parser-0.9.0b2/pyproject_parser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyproject-parser
-Version: 0.9.0b1
+Version: 0.9.0b2
 Summary: Parser for 'pyproject.toml'
 Home-page: https://github.com/repo-helper/pyproject-parser
 Author: Dominic Davis-Foster
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 License: Copyright (c) 2021 Dominic Davis-Foster
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -156,15 +156,15 @@
 .. |license| image:: https://img.shields.io/github/license/repo-helper/pyproject-parser
 	:target: https://github.com/repo-helper/pyproject-parser/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/repo-helper/pyproject-parser
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/pyproject-parser/v0.9.0b1
+.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/pyproject-parser/v0.9.0b2
 	:target: https://github.com/repo-helper/pyproject-parser/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/repo-helper/pyproject-parser
 	:target: https://github.com/repo-helper/pyproject-parser/commit/master
 	:alt: GitHub last commit
```

### Comparing `pyproject-parser-0.9.0b1/pyproject_parser.egg-info/SOURCES.txt` & `pyproject-parser-0.9.0b2/pyproject_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyproject-parser-0.9.0b1/setup.cfg` & `pyproject-parser-0.9.0b2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyproject-parser
-version = 0.9.0b1
+version = 0.9.0b2
 author = Dominic Davis-Foster
 author_email = dominic@davis-foster.co.uk
 license = MIT License
 keywords = pep518, pep621, pyproject, toml, metadata, packaging
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 platforms = Windows, macOS, Linux
```

### Comparing `pyproject-parser-0.9.0b1/setup.py` & `pyproject-parser-0.9.0b2/setup.py`

 * *Files identical despite different names*

### Comparing `pyproject-parser-0.9.0b1/tests/test_classes.py` & `pyproject-parser-0.9.0b2/tests/test_classes.py`

 * *Files identical despite different names*

### Comparing `pyproject-parser-0.9.0b1/tests/test_cli.py` & `pyproject-parser-0.9.0b2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `pyproject-parser-0.9.0b1/tests/test_cli_module.py` & `pyproject-parser-0.9.0b2/tests/test_cli_module.py`

 * *Files identical despite different names*

### Comparing `pyproject-parser-0.9.0b1/tests/test_config.py` & `pyproject-parser-0.9.0b2/tests/test_config.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 # stdlib
 from textwrap import dedent
 from typing import Type
 
 # 3rd party
-import dom_toml
 import pytest
 from coincidence.regressions import AdvancedDataRegressionFixture
 from dom_toml.parser import BadConfigError
 from domdf_python_tools.paths import PathPlus, in_directory
 from pyproject_examples import (
 		OPTIONAL_DEPENDENCIES,
 		bad_buildsystem_config,
 		bad_pep621_config,
 		valid_buildsystem_config,
 		valid_pep621_config
 		)
+from pyproject_examples.example_configs import MINIMAL_CONFIG
+from shippinglabel import normalize_keep_dot
 
 # this package
 from pyproject_parser.parsers import BuildSystemParser, PEP621Parser, RequiredKeysConfigParser
 from pyproject_parser.utils import PyProjectDeprecationWarning, _load_toml
 
 
 @pytest.mark.parametrize("set_defaults", [True, False])
@@ -62,14 +63,86 @@
 
 	with in_directory(tmp_pathplus):
 		config = ReducedPEP621Parser().parse(_load_toml(tmp_pathplus / "pyproject.toml")["project"])
 
 	advanced_data_regression.check(config)
 
 
+class NormalizingPEP621Parser(PEP621Parser, inherit_defaults=True):
+	keys = ["name", "dependencies", "optional-dependencies"]
+
+
+class NormalizingWithDotPEP621Parser(PEP621Parser, inherit_defaults=True):
+	keys = ["name", "dependencies", "optional-dependencies"]
+
+	@staticmethod
+	def normalize_requirement_name(name: str) -> str:
+		return normalize_keep_dot(name)
+
+
+class UnNormalizingPEP621Parser(PEP621Parser, inherit_defaults=True):
+	keys = ["name", "dependencies", "optional-dependencies"]
+
+	@staticmethod
+	def normalize_requirement_name(name: str) -> str:
+		return name
+
+
+pep621_config_for_normalize_test = [
+		MINIMAL_CONFIG,
+		'dependencies = ["whey", "A.b", "domdf_python_tools"]',
+		'',
+		"[project.optional-dependencies]",
+		"test = [",
+		'  "Pytest",',
+		'  "d.e.f",',
+		'  "chemistry_tools",',
+		']'
+		]
+
+
+def test_pep621_unnormalized(
+		tmp_pathplus: PathPlus,
+		advanced_data_regression: AdvancedDataRegressionFixture,
+		):
+
+	(tmp_pathplus / "pyproject.toml").write_lines(pep621_config_for_normalize_test)
+
+	with in_directory(tmp_pathplus):
+		config = UnNormalizingPEP621Parser().parse(_load_toml(tmp_pathplus / "pyproject.toml")["project"])
+
+	advanced_data_regression.check(config)
+
+
+def test_pep621_normalize(
+		tmp_pathplus: PathPlus,
+		advanced_data_regression: AdvancedDataRegressionFixture,
+		):
+
+	(tmp_pathplus / "pyproject.toml").write_lines(pep621_config_for_normalize_test)
+
+	with in_directory(tmp_pathplus):
+		config = NormalizingPEP621Parser().parse(_load_toml(tmp_pathplus / "pyproject.toml")["project"])
+
+	advanced_data_regression.check(config)
+
+
+def test_pep621_normalize_keep_dot(
+		tmp_pathplus: PathPlus,
+		advanced_data_regression: AdvancedDataRegressionFixture,
+		):
+
+	(tmp_pathplus / "pyproject.toml").write_lines(pep621_config_for_normalize_test)
+
+	with in_directory(tmp_pathplus):
+		config = NormalizingWithDotPEP621Parser().parse(_load_toml(tmp_pathplus / "pyproject.toml")["project"])
+
+	advanced_data_regression.check(config)
+
+
 @pytest.mark.parametrize("filename", ["README.rst", "README.md", "INTRODUCTION.md", "readme.txt"])
 def test_pep621_class_valid_config_readme(
 		filename: str,
 		tmp_pathplus: PathPlus,
 		advanced_data_regression: AdvancedDataRegressionFixture,
 		):
 
@@ -393,14 +466,86 @@
 def test_buildsystem_parser_errors(config: str, expects: Type[Exception], match: str, tmp_pathplus: PathPlus):
 	(tmp_pathplus / "pyproject.toml").write_clean(config)
 
 	with in_directory(tmp_pathplus), pytest.raises(expects, match=match):
 		BuildSystemParser().parse(_load_toml(tmp_pathplus / "pyproject.toml")["build-system"])
 
 
+class NormalizingBuildSystemParser(BuildSystemParser, inherit_defaults=True):
+	keys = ["requires"]
+
+
+class NormalizingWithDotBuildSystemParser(BuildSystemParser, inherit_defaults=True):
+	keys = ["requires"]
+
+	@staticmethod
+	def normalize_requirement_name(name: str) -> str:
+		return normalize_keep_dot(name)
+
+
+class UnNormalizingBuildSystemParser(BuildSystemParser, inherit_defaults=True):
+	keys = ["requires"]
+
+	@staticmethod
+	def normalize_requirement_name(name: str) -> str:
+		return name
+
+
+def test_buildsystem_normalize(
+		tmp_pathplus: PathPlus,
+		advanced_data_regression: AdvancedDataRegressionFixture,
+		):
+
+	(tmp_pathplus / "pyproject.toml").write_lines([
+			"[build-system]",
+			'requires = ["whey", "Foo.bar", "domdf_python_tools"]',
+			])
+
+	with in_directory(tmp_pathplus):
+		config = NormalizingBuildSystemParser().parse(_load_toml(tmp_pathplus / "pyproject.toml")["build-system"])
+
+	advanced_data_regression.check(config)
+
+
+def test_buildsystem_normalize_keep_dot(
+		tmp_pathplus: PathPlus,
+		advanced_data_regression: AdvancedDataRegressionFixture,
+		):
+
+	(tmp_pathplus / "pyproject.toml").write_lines([
+			"[build-system]",
+			'requires = ["whey", "Foo.bar", "domdf_python_tools"]',
+			])
+
+	with in_directory(tmp_pathplus):
+		config = NormalizingWithDotBuildSystemParser().parse(
+				_load_toml(tmp_pathplus / "pyproject.toml")["build-system"]
+				)
+
+	advanced_data_regression.check(config)
+
+
+def test_buildsystem_unnormalized(
+		tmp_pathplus: PathPlus,
+		advanced_data_regression: AdvancedDataRegressionFixture,
+		):
+
+	(tmp_pathplus / "pyproject.toml").write_lines([
+			"[build-system]",
+			'requires = ["whey", "Foo.bar", "domdf_python_tools"]',
+			])
+
+	with in_directory(tmp_pathplus):
+		config = UnNormalizingBuildSystemParser().parse(
+				_load_toml(tmp_pathplus / "pyproject.toml")["build-system"]
+				)
+
+	advanced_data_regression.check(config)
+
+
 def test_RequiredKeysConfigParser():
 
 	class MyConfigParser(RequiredKeysConfigParser):
 		table_name = "my_table"
 		required_keys = ["foo"]
 		keys = ["foo", "bar"]
 		defaults = {"foo": "foo-default", "bar": "bar-defaults"}
```

### Comparing `pyproject-parser-0.9.0b1/tests/test_dumping.py` & `pyproject-parser-0.9.0b2/tests/test_dumping.py`

 * *Files identical despite different names*

### Comparing `pyproject-parser-0.9.0b1/tests/test_pyproject_class.py` & `pyproject-parser-0.9.0b2/tests/test_pyproject_class.py`

 * *Files identical despite different names*

### Comparing `pyproject-parser-0.9.0b1/tests/test_utils.py` & `pyproject-parser-0.9.0b2/tests/test_utils.py`

 * *Files identical despite different names*

