# Comparing `tmp/typical-2.8.0.tar.gz` & `tmp/typical-2.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typical-2.8.0.tar", max compression
+gzip compressed data, was "typical-2.8.1.tar", max compression
```

## Comparing `typical-2.8.0.tar` & `typical-2.8.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0     1080 2021-12-23 15:19:21.465273 typical-2.8.0/LICENSE
--rw-r--r--   0        0        0     5591 2021-12-23 15:19:21.465541 typical-2.8.0/README.md
--rw-r--r--   0        0        0     5591 2021-12-23 15:19:21.469222 typical-2.8.0/docs/index.md
--rw-r--r--   0        0        0     4762 2021-12-23 15:19:21.485257 typical-2.8.0/pyproject.toml
--rw-r--r--   0        0        0      289 2021-12-23 15:19:21.496113 typical-2.8.0/typic/__init__.py
--rw-r--r--   0        0        0    22076 2021-12-23 15:19:21.496630 typical-2.8.0/typic/api.py
--rw-r--r--   0        0        0    20293 2021-12-23 15:19:21.497744 typical-2.8.0/typic/checks.py
--rw-r--r--   0        0        0     2369 2021-12-23 15:19:21.498080 typical-2.8.0/typic/common.py
--rw-r--r--   0        0        0     4775 2021-12-23 15:19:21.498331 typical-2.8.0/typic/compat.py
--rw-r--r--   0        0        0     1232 2021-12-23 15:19:21.498728 typical-2.8.0/typic/constraints/__init__.py
--rw-r--r--   0        0        0     7991 2021-12-23 15:19:21.499112 typical-2.8.0/typic/constraints/array.py
--rw-r--r--   0        0        0    21806 2021-12-23 15:19:21.499565 typical-2.8.0/typic/constraints/common.py
--rw-r--r--   0        0        0      243 2021-12-23 15:19:21.499925 typical-2.8.0/typic/constraints/error.py
--rw-r--r--   0        0        0    13171 2021-12-23 15:19:21.500597 typical-2.8.0/typic/constraints/factory.py
--rw-r--r--   0        0        0    12037 2021-12-23 15:19:21.501739 typical-2.8.0/typic/constraints/mapping.py
--rw-r--r--   0        0        0     7614 2021-12-23 15:19:21.526640 typical-2.8.0/typic/constraints/number.py
--rw-r--r--   0        0        0     3022 2021-12-23 15:19:21.527199 typical-2.8.0/typic/constraints/text.py
--rw-r--r--   0        0        0     4167 2021-12-23 15:19:21.527624 typical-2.8.0/typic/env.py
--rw-r--r--   0        0        0        0 2021-12-23 15:19:21.527914 typical-2.8.0/typic/ext/__init__.py
--rw-r--r--   0        0        0     2613 2021-12-23 15:19:21.528099 typical-2.8.0/typic/ext/json.py
--rw-r--r--   0        0        0      104 2021-12-23 15:19:21.528505 typical-2.8.0/typic/ext/schema/__init__.py
--rw-r--r--   0        0        0      174 2021-12-23 15:19:21.528788 typical-2.8.0/typic/ext/schema/compat.py
--rw-r--r--   0        0        0    11698 2021-12-23 15:19:21.529025 typical-2.8.0/typic/ext/schema/field.py
--rw-r--r--   0        0        0    17588 2021-12-23 15:19:21.529433 typical-2.8.0/typic/ext/schema/schema.py
--rw-r--r--   0        0        0     9349 2021-12-23 15:19:21.529766 typical-2.8.0/typic/gen.py
--rw-r--r--   0        0        0     6436 2021-12-23 15:19:21.530076 typical-2.8.0/typic/klass.py
--rw-r--r--   0        0        0    11557 2021-12-23 15:19:21.530411 typical-2.8.0/typic/mypy.py
--rw-r--r--   0        0        0        0 2021-12-23 15:19:21.530518 typical-2.8.0/typic/py.typed
--rw-r--r--   0        0        0        0 2021-12-23 15:19:21.530699 typical-2.8.0/typic/serde/__init__.py
--rw-r--r--   0        0        0     9272 2021-12-23 15:19:21.530887 typical-2.8.0/typic/serde/binder.py
--rw-r--r--   0        0        0    17140 2021-12-23 15:19:21.531308 typical-2.8.0/typic/serde/common.py
--rw-r--r--   0        0        0    34862 2021-12-23 15:19:21.531904 typical-2.8.0/typic/serde/des.py
--rw-r--r--   0        0        0    28890 2021-12-23 15:19:21.532528 typical-2.8.0/typic/serde/resolver.py
--rw-r--r--   0        0        0    16544 2021-12-23 15:19:21.532903 typical-2.8.0/typic/serde/ser.py
--rw-r--r--   0        0        0    10309 2021-12-23 15:19:21.533173 typical-2.8.0/typic/serde/translator.py
--rw-r--r--   0        0        0     2093 2021-12-23 15:19:21.533588 typical-2.8.0/typic/strict.py
--rw-r--r--   0        0        0      190 2021-12-23 15:19:21.534130 typical-2.8.0/typic/types/__init__.py
--rw-r--r--   0        0        0     6878 2021-12-23 15:19:21.534466 typical-2.8.0/typic/types/dsn.py
--rw-r--r--   0        0        0     5578 2021-12-23 15:19:21.534781 typical-2.8.0/typic/types/email.py
--rw-r--r--   0        0        0     4506 2021-12-23 15:19:21.535099 typical-2.8.0/typic/types/frozendict.py
--rw-r--r--   0        0        0     1109 2021-12-23 15:19:21.535484 typical-2.8.0/typic/types/path.py
--rw-r--r--   0        0        0     2295 2021-12-23 15:19:21.535721 typical-2.8.0/typic/types/secret.py
--rw-r--r--   0        0        0    12240 2021-12-23 15:19:21.536036 typical-2.8.0/typic/types/url.py
--rw-r--r--   0        0        0    23668 2021-12-23 15:19:21.536471 typical-2.8.0/typic/util.py
--rw-r--r--   0        0        0     7953 2021-12-23 15:22:19.383323 typical-2.8.0/setup.py
--rw-r--r--   0        0        0     8696 2021-12-23 15:22:19.384013 typical-2.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-04-26 17:03:16.952060 typical-2.8.1/LICENSE
+-rw-r--r--   0        0        0     5591 2023-04-26 17:03:16.952378 typical-2.8.1/README.md
+-rw-r--r--   0        0        0     5591 2023-04-26 17:03:16.957100 typical-2.8.1/docs/index.md
+-rw-r--r--   0        0        0     4768 2023-04-26 17:03:16.974669 typical-2.8.1/pyproject.toml
+-rw-r--r--   0        0        0      289 2023-04-26 17:03:16.985628 typical-2.8.1/typic/__init__.py
+-rw-r--r--   0        0        0    22076 2023-04-26 17:03:16.985933 typical-2.8.1/typic/api.py
+-rw-r--r--   0        0        0    20293 2023-04-26 17:03:16.986353 typical-2.8.1/typic/checks.py
+-rw-r--r--   0        0        0     2369 2023-04-26 17:03:16.986625 typical-2.8.1/typic/common.py
+-rw-r--r--   0        0        0     5692 2023-04-26 17:03:16.986859 typical-2.8.1/typic/compat.py
+-rw-r--r--   0        0        0     1232 2023-04-26 17:03:16.987196 typical-2.8.1/typic/constraints/__init__.py
+-rw-r--r--   0        0        0     7991 2023-04-26 17:03:16.987454 typical-2.8.1/typic/constraints/array.py
+-rw-r--r--   0        0        0    21806 2023-04-26 17:03:16.987775 typical-2.8.1/typic/constraints/common.py
+-rw-r--r--   0        0        0      243 2023-04-26 17:03:16.988031 typical-2.8.1/typic/constraints/error.py
+-rw-r--r--   0        0        0    13171 2023-04-26 17:03:16.988313 typical-2.8.1/typic/constraints/factory.py
+-rw-r--r--   0        0        0    12037 2023-04-26 17:03:16.988683 typical-2.8.1/typic/constraints/mapping.py
+-rw-r--r--   0        0        0     7614 2023-04-26 17:03:16.988991 typical-2.8.1/typic/constraints/number.py
+-rw-r--r--   0        0        0     3022 2023-04-26 17:03:16.989277 typical-2.8.1/typic/constraints/text.py
+-rw-r--r--   0        0        0     4167 2023-04-26 17:03:16.989527 typical-2.8.1/typic/env.py
+-rw-r--r--   0        0        0        0 2023-04-26 17:03:16.989757 typical-2.8.1/typic/ext/__init__.py
+-rw-r--r--   0        0        0     2613 2023-04-26 17:03:16.989951 typical-2.8.1/typic/ext/json.py
+-rw-r--r--   0        0        0      104 2023-04-26 17:03:16.990262 typical-2.8.1/typic/ext/schema/__init__.py
+-rw-r--r--   0        0        0      174 2023-04-26 17:03:16.990507 typical-2.8.1/typic/ext/schema/compat.py
+-rw-r--r--   0        0        0    11698 2023-04-26 17:03:16.990801 typical-2.8.1/typic/ext/schema/field.py
+-rw-r--r--   0        0        0    17588 2023-04-26 17:03:16.991118 typical-2.8.1/typic/ext/schema/schema.py
+-rw-r--r--   0        0        0     9450 2023-04-26 17:03:16.991757 typical-2.8.1/typic/gen.py
+-rw-r--r--   0        0        0     6436 2023-04-26 17:03:16.992413 typical-2.8.1/typic/klass.py
+-rw-r--r--   0        0        0    11557 2023-04-26 17:03:16.992710 typical-2.8.1/typic/mypy.py
+-rw-r--r--   0        0        0        0 2023-04-26 17:03:16.992841 typical-2.8.1/typic/py.typed
+-rw-r--r--   0        0        0        0 2023-04-26 17:03:16.993106 typical-2.8.1/typic/serde/__init__.py
+-rw-r--r--   0        0        0     9272 2023-04-26 17:03:16.993314 typical-2.8.1/typic/serde/binder.py
+-rw-r--r--   0        0        0    17140 2023-04-26 17:03:16.993778 typical-2.8.1/typic/serde/common.py
+-rw-r--r--   0        0        0    34862 2023-04-26 17:03:16.994295 typical-2.8.1/typic/serde/des.py
+-rw-r--r--   0        0        0    28948 2023-04-26 17:03:16.995117 typical-2.8.1/typic/serde/resolver.py
+-rw-r--r--   0        0        0    16544 2023-04-26 17:03:16.995653 typical-2.8.1/typic/serde/ser.py
+-rw-r--r--   0        0        0    10309 2023-04-26 17:03:16.995988 typical-2.8.1/typic/serde/translator.py
+-rw-r--r--   0        0        0     2093 2023-04-26 17:03:16.996231 typical-2.8.1/typic/strict.py
+-rw-r--r--   0        0        0      190 2023-04-26 17:03:16.996524 typical-2.8.1/typic/types/__init__.py
+-rw-r--r--   0        0        0     6878 2023-04-26 17:03:16.996783 typical-2.8.1/typic/types/dsn.py
+-rw-r--r--   0        0        0     5578 2023-04-26 17:03:16.997103 typical-2.8.1/typic/types/email.py
+-rw-r--r--   0        0        0     4506 2023-04-26 17:03:16.997403 typical-2.8.1/typic/types/frozendict.py
+-rw-r--r--   0        0        0     1109 2023-04-26 17:03:16.997641 typical-2.8.1/typic/types/path.py
+-rw-r--r--   0        0        0     2295 2023-04-26 17:03:16.997861 typical-2.8.1/typic/types/secret.py
+-rw-r--r--   0        0        0    12240 2023-04-26 17:03:16.998119 typical-2.8.1/typic/types/url.py
+-rw-r--r--   0        0        0    23668 2023-04-26 17:03:16.998806 typical-2.8.1/typic/util.py
+-rw-r--r--   0        0        0     7944 2023-04-26 17:03:37.318316 typical-2.8.1/setup.py
+-rw-r--r--   0        0        0     8687 2023-04-26 17:03:37.319141 typical-2.8.1/PKG-INFO
```

### Comparing `typical-2.8.0/LICENSE` & `typical-2.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `typical-2.8.0/README.md` & `typical-2.8.1/README.md`

 * *Files identical despite different names*

### Comparing `typical-2.8.0/docs/index.md` & `typical-2.8.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `typical-2.8.0/pyproject.toml` & `typical-2.8.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "typical"
 packages = [{include = "typic"}]
-version = "2.8.0"
+version = "2.8.1"
 description = "Typical: Python's Typing Toolkit."
 authors = ["Sean Stewart <sean_stewart@me.com>"]
 license = "MIT"
 readme = "docs/index.md"
 repository = "https://github.com/seandstewart/typical"
 keywords = ["typing", "data", "annotations", "validation", "json-schema"]
 classifiers = [
@@ -31,15 +31,15 @@
 # package
 python = "^3.7"
 inflection = "^0.5"
 pendulum = "^2.1"
 fastjsonschema = {version = "^2.14", optional = true}
 ujson = {version = ">=2.0", optional = true}
 orjson = {version = "^3.6.3", optional = true}
-typing-extensions = {version = "^3.10.0", python = "<3.10"}
+typing-extensions = {version = "^4", python = "<3.10"}
 # tests
 pytest = {version = "^6.2", optional = true}
 pytest-cov = {version = "^2.8", optional = true}
 pandas = {version = "^1.1.3", python = ">=3.7.1,<=3.9", optional = true}
 sqlalchemy = {version = "^1.3.13", optional = true}
 # benchmarks
 pytest-benchmark = {version = "^3.2", extras = ["histogram"], optional = true}
@@ -150,19 +150,19 @@
   | buck-out
   | build
   | dist
 )/
 '''
 
 [build-system]
-requires = ["poetry>=0.12"]
-build-backend = "poetry.masonry.api"
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
 
 [bumpver]
-current_version = "v2.8.0"
+current_version = "v2.8.1"
 version_pattern = "vMAJOR.MINOR.PATCH[-TAGNUM]"
 commit_message = "bump version to {new_version} [ci skip]"
 tag = false
 push = true
 commit = true
 
 [bumpver.file_patterns]
```

### Comparing `typical-2.8.0/typic/api.py` & `typical-2.8.1/typic/api.py`

 * *Files identical despite different names*

### Comparing `typical-2.8.0/typic/checks.py` & `typical-2.8.1/typic/checks.py`

 * *Files identical despite different names*

### Comparing `typical-2.8.0/typic/common.py` & `typical-2.8.1/typic/common.py`

 * *Files identical despite different names*

### Comparing `typical-2.8.0/typic/constraints/__init__.py` & `typical-2.8.1/typic/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `typical-2.8.0/typic/constraints/array.py` & `typical-2.8.1/typic/constraints/array.py`

 * *Files identical despite different names*

### Comparing `typical-2.8.0/typic/constraints/common.py` & `typical-2.8.1/typic/constraints/common.py`

 * *Files identical despite different names*

### Comparing `typical-2.8.0/typic/constraints/factory.py` & `typical-2.8.1/typic/constraints/factory.py`

 * *Files identical despite different names*

### Comparing `typical-2.8.0/typic/constraints/mapping.py` & `typical-2.8.1/typic/constraints/mapping.py`

 * *Files identical despite different names*

### Comparing `typical-2.8.0/typic/constraints/number.py` & `typical-2.8.1/typic/constraints/number.py`

 * *Files identical despite different names*

### Comparing `typical-2.8.0/typic/constraints/text.py` & `typical-2.8.1/typic/constraints/text.py`

 * *Files identical despite different names*

### Comparing `typical-2.8.0/typic/env.py` & `typical-2.8.1/typic/env.py`

 * *Files identical despite different names*

### Comparing `typical-2.8.0/typic/ext/json.py` & `typical-2.8.1/typic/ext/json.py`

 * *Files identical despite different names*

### Comparing `typical-2.8.0/typic/ext/schema/field.py` & `typical-2.8.1/typic/ext/schema/field.py`

 * *Files identical despite different names*

### Comparing `typical-2.8.0/typic/ext/schema/schema.py` & `typical-2.8.1/typic/ext/schema/schema.py`

 * *Files identical despite different names*

### Comparing `typical-2.8.0/typic/gen.py` & `typical-2.8.1/typic/gen.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,14 +27,20 @@
     DEF = "def"
     CLS = "class"
     AST = "assert"
     IMP = "import"
     FRM = "from"
     DEC = "@"
 
+    def __str__(self):
+        return self.value
+
+    def __repr__(self):
+        return self.value
+
 
 @slotted(dict=False)
 @dataclasses.dataclass(frozen=True)
 class Line:
     INDENT = "    "
     code: str
     level: int
```

### Comparing `typical-2.8.0/typic/klass.py` & `typical-2.8.1/typic/klass.py`

 * *Files identical despite different names*

### Comparing `typical-2.8.0/typic/mypy.py` & `typical-2.8.1/typic/mypy.py`

 * *Files identical despite different names*

### Comparing `typical-2.8.0/typic/serde/binder.py` & `typical-2.8.1/typic/serde/binder.py`

 * *Files identical despite different names*

### Comparing `typical-2.8.0/typic/serde/common.py` & `typical-2.8.1/typic/serde/common.py`

 * *Files identical despite different names*

### Comparing `typical-2.8.0/typic/serde/des.py` & `typical-2.8.1/typic/serde/des.py`

 * *Files identical despite different names*

### Comparing `typical-2.8.0/typic/serde/resolver.py` & `typical-2.8.1/typic/serde/resolver.py`

 * *Files 1% similar despite different names*

```diff
@@ -771,14 +771,16 @@
         hints = util.cached_type_hints(obj)
         params = util.safe_get_params(obj)
         fields: Mapping[str, dataclasses.Field] = {}
         if dataclasses.is_dataclass(obj):
             fields = {f.name: f for f in dataclasses.fields(obj)}
         ann = {}
         for name in params.keys() | hints.keys():
+            if name == "return":
+                continue
             param = params.get(name)
             hint = hints.get(name)
             field = fields.get(name)
             annotation = hint or param.annotation  # type: ignore
             annotation = util.resolve_supertype(annotation)
             param = param or inspect.Parameter(
                 name,
```

### Comparing `typical-2.8.0/typic/serde/ser.py` & `typical-2.8.1/typic/serde/ser.py`

 * *Files identical despite different names*

### Comparing `typical-2.8.0/typic/serde/translator.py` & `typical-2.8.1/typic/serde/translator.py`

 * *Files identical despite different names*

### Comparing `typical-2.8.0/typic/strict.py` & `typical-2.8.1/typic/strict.py`

 * *Files identical despite different names*

### Comparing `typical-2.8.0/typic/types/dsn.py` & `typical-2.8.1/typic/types/dsn.py`

 * *Files identical despite different names*

### Comparing `typical-2.8.0/typic/types/email.py` & `typical-2.8.1/typic/types/email.py`

 * *Files identical despite different names*

### Comparing `typical-2.8.0/typic/types/frozendict.py` & `typical-2.8.1/typic/types/frozendict.py`

 * *Files identical despite different names*

### Comparing `typical-2.8.0/typic/types/path.py` & `typical-2.8.1/typic/types/path.py`

 * *Files identical despite different names*

### Comparing `typical-2.8.0/typic/types/secret.py` & `typical-2.8.1/typic/types/secret.py`

 * *Files identical despite different names*

### Comparing `typical-2.8.0/typic/types/url.py` & `typical-2.8.1/typic/types/url.py`

 * *Files identical despite different names*

### Comparing `typical-2.8.0/typic/util.py` & `typical-2.8.1/typic/util.py`

 * *Files identical despite different names*

### Comparing `typical-2.8.0/setup.py` & `typical-2.8.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['future-typing>=0.4.1,<0.5.0', 'inflection>=0.5,<0.6', 'pendulum>=2.1,<3.0']
 
 extras_require = \
-{':python_version < "3.10"': ['typing-extensions>=3.10.0,<4.0.0'],
+{':python_version < "3.10"': ['typing-extensions>=4,<5'],
  'benchmarks': ['sqlalchemy>=1.3.13,<2.0.0',
                 'pytest-benchmark[histogram]>=3.2,<4.0',
                 'marshmallow>=3.2,<4.0',
                 'toastedmarshmallow>=2.15,<3.0',
                 'djangorestframework>=3.10,<4.0',
                 'pydantic[email]>=1.0,<2.0',
                 'pydantic[email]>=1.0,<2.0',
@@ -47,15 +47,15 @@
            'sqlalchemy>=1.3.13,<2.0.0',
            'pydantic[email]>=1.0,<2.0',
            'mypy>=0.910,<0.911'],
  'tests:python_full_version >= "3.7.1" and python_version <= "3.9"': ['pandas>=1.1.3,<2.0.0']}
 
 setup_kwargs = {
     'name': 'typical',
-    'version': '2.8.0',
+    'version': '2.8.1',
     'description': "Typical: Python's Typing Toolkit.",
     'long_description': '# typical: Python\'s Typing Toolkit\n[![image](https://img.shields.io/pypi/v/typical.svg)](https://pypi.org/project/typical/)\n[![image](https://img.shields.io/pypi/l/typical.svg)](https://pypi.org/project/typical/)\n[![image](https://img.shields.io/pypi/pyversions/typical.svg)](https://pypi.org/project/typical/)\n[![image](https://img.shields.io/github/languages/code-size/seandstewart/typical.svg?style=flat)](https://github.com/seandstewart/typical)\n[![Test & Lint](https://github.com/seandstewart/typical/workflows/Test%20&%20Lint/badge.svg)](https://github.com/seandstewart/typical/actions)\n[![Coverage](https://codecov.io/gh/seandstewart/typical/branch/master/graph/badge.svg)](https://codecov.io/gh/seandstewart/typical)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)\n[![Netlify Status](https://api.netlify.com/api/v1/badges/982a0ced-bb7f-4391-87e8-1957071d2f66/deploy-status)](https://app.netlify.com/sites/typical-python/deploys)\n\n![How Typical](static/typical.png)\n\n## Introduction\n\nTypical is a library devoted to runtime analysis, inference,\nvalidation, and enforcement of Python types,\n[PEP 484](https://www.python.org/dev/peps/pep-0484/) Type Hints, and\ncustom user-defined data-types.\n\nTypical is fully compliant with the following Python Typing PEPs:\n\n- [PEP 484 -- Type Hints](https://www.python.org/dev/peps/pep-0484/)\n- [PEP 563 -- Postponed Evaluation of Annotations](https://www.python.org/dev/peps/pep-0563/)\n- [PEP 585 -- Type Hinting Generics In Standard Collections](https://www.python.org/dev/peps/pep-0585/)\n- [PEP 586 -- Literal Types](https://www.python.org/dev/peps/pep-0586/)\n- [PEP 589 -- TypedDict: Type Hints for Dictionaries with a Fixed Set of Keys](https://www.python.org/dev/peps/pep-0589/)\n- [PEP 604 -- Allow writing union types as X | Y](https://www.python.org/dev/peps/pep-0604/)\n\nIt provides a high-level Protocol API, Functional API, and Object API to suit most any\noccasion.\n\n## Getting Started\n\nInstallation is as simple as `pip install -U typical`.\n## Help\n\nThe latest documentation is hosted at\n[python-typical.org](https://python-typical.org/).\n\n> Starting with version 2.0, All documentation is hand-crafted\n> markdown & versioned documentation can be found at typical\'s\n> [Git Repo](https://github.com/seandstewart/typical/tree/master/docs).\n> (Versioned documentation is still in-the-works directly on our\n> domain.)\n\n## A Typical Use-Case\n\nThe decorator that started it all:\n\n### `typic.al(...)`\n\n```python\nimport typic\n\n\n@typic.al\ndef hard_math(a: int, b: int, *c: int) -> int:\n    return a + b + sum(c)\n\nhard_math(1, "3")\n#> 4\n\n\n@typic.al(strict=True)\ndef strict_math(a: int, b: int, *c: int) -> int:\n    return a + b + sum(c)\n\nstrict_math(1, 2, 3, "4")\n#> Traceback (most recent call last):\n#>  ...\n#> typic.constraints.error.ConstraintValueError: Given value <\'4\'> fails constraints: (type=int, nullable=False, coerce=False)\n  \n```\n\nTypical has both a high-level *Object API* and high-level\n*Functional API*. In general, any method registered to one API is also\navailable to the other.\n\n### The Protocol API\n\n```python\nimport dataclasses\nfrom typing import Iterable\n\nimport typic\n\n\n@typic.constrained(ge=1)\nclass ID(int):\n    ...\n\n\n@typic.constrained(max_length=280)\nclass Tweet(str):\n    ...\n\n\n@dataclasses.dataclass # or typing.TypedDict or typing.NamedTuple or annotated class...\nclass Tweeter:\n    id: ID\n    tweets: Iterable[Tweet]\n\n\njson = \'{"id":1,"tweets":["I don\\\'t understand Twitter"]}\'\nprotocol = typic.protocol(Tweeter)\n\nt = protocol.transmute(json)\nprint(t)\n#> Tweeter(id=1, tweets=["I don\'t understand Twitter"])\n\nprint(protocol.tojson(t))\n#> \'{"id":1,"tweets":["I don\\\'t understand Twitter"]}\'\n\nprotocol.validate({"id": 0, "tweets": []})\n#> Traceback (most recent call last):\n#>  ...\n#> typic.constraints.error.ConstraintValueError: Tweeter.id: value <0> fails constraints: (type=int, nullable=False, coerce=False, ge=1)\n```\n\n### The Functional API\n\n```python\nimport dataclasses\nfrom typing import Iterable\n\nimport typic\n\n\n@typic.constrained(ge=1)\nclass ID(int):\n    ...\n\n\n@typic.constrained(max_length=280)\nclass Tweet(str):\n    ...\n\n\n@dataclasses.dataclass # or typing.TypedDict or typing.NamedTuple or annotated class...\nclass Tweeter:\n    id: ID\n    tweets: Iterable[Tweet]\n\n\njson = \'{"id":1,"tweets":["I don\\\'t understand Twitter"]}\'\n\nt = typic.transmute(Tweeter, json)\nprint(t)\n#> Tweeter(id=1, tweets=["I don\'t understand Twitter"])\n\nprint(typic.tojson(t))\n#> \'{"id":1,"tweets":["I don\\\'t understand Twitter"]}\'\n\ntypic.validate(Tweeter, {"id": 0, "tweets": []})\n#> Traceback (most recent call last):\n#>  ...\n#> typic.constraints.error.ConstraintValueError: Tweeter.id: value <0> fails constraints: (type=int, nullable=False, coerce=False, ge=1)\n```\n\n### The Object API\n\n```python\nfrom typing import Iterable\n\nimport typic\n\n\n@typic.constrained(ge=1)\nclass ID(int):\n    ...\n\n\n@typic.constrained(max_length=280)\nclass Tweet(str):\n    ...\n\n\n@typic.klass\nclass Tweeter:\n    id: ID\n    tweets: Iterable[Tweet]\n    \n\njson = \'{"id":1,"tweets":["I don\\\'t understand Twitter"]}\'\nt = Tweeter.transmute(json)\n\nprint(t)\n#> Tweeter(id=1, tweets=["I don\'t understand Twitter"])\n\nprint(t.tojson())\n#> \'{"id":1,"tweets":["I don\\\'t understand Twitter"]}\'\n\nTweeter.validate({"id": 0, "tweets": []})\n#> Traceback (most recent call last):\n#>  ...\n#> typic.constraints.error.ConstraintValueError: Given value <0> fails constraints: (type=int, nullable=False, coerce=False, ge=1)\n```\n\n\n## Changelog\n\nSee our\n[Releases](https://github.com/seandstewart/typical/releases).\n',
     'author': 'Sean Stewart',
     'author_email': 'sean_stewart@me.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/seandstewart/typical',
```

### Comparing `typical-2.8.0/PKG-INFO` & `typical-2.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typical
-Version: 2.8.0
+Version: 2.8.1
 Summary: Typical: Python's Typing Toolkit.
 Home-page: https://github.com/seandstewart/typical
 License: MIT
 Keywords: typing,data,annotations,validation,json-schema
 Author: Sean Stewart
 Author-email: sean_stewart@me.com
 Requires-Python: >=3.7,<4.0
@@ -52,15 +52,15 @@
 Requires-Dist: sqlalchemy (>=1.3.13,<2.0.0); extra == "tests" or extra == "benchmarks"
 Requires-Dist: toastedmarshmallow (>=2.15,<3.0); extra == "benchmarks"
 Requires-Dist: types-python-dateutil; extra == "lint"
 Requires-Dist: types-setuptools; extra == "lint"
 Requires-Dist: types-toml; extra == "lint"
 Requires-Dist: types-typed-ast; extra == "lint"
 Requires-Dist: types-ujson; extra == "lint"
-Requires-Dist: typing-extensions (>=3.10.0,<4.0.0); python_version < "3.10"
+Requires-Dist: typing-extensions (>=4,<5); python_version < "3.10"
 Requires-Dist: ujson (>=2.0); extra == "json" or extra == "tests"
 Project-URL: Repository, https://github.com/seandstewart/typical
 Description-Content-Type: text/markdown
 
 # typical: Python's Typing Toolkit
 [![image](https://img.shields.io/pypi/v/typical.svg)](https://pypi.org/project/typical/)
 [![image](https://img.shields.io/pypi/l/typical.svg)](https://pypi.org/project/typical/)
```

