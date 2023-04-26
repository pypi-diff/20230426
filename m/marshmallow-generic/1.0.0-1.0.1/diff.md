# Comparing `tmp/marshmallow-generic-1.0.0.tar.gz` & `tmp/marshmallow-generic-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marshmallow-generic-1.0.0.tar", last modified: Mon Mar 13 19:40:37 2023, max compression
+gzip compressed data, was "marshmallow-generic-1.0.1.tar", last modified: Wed Apr 26 15:21:09 2023, max compression
```

## Comparing `marshmallow-generic-1.0.0.tar` & `marshmallow-generic-1.0.1.tar`

### file list

```diff
@@ -1,42 +1,49 @@
-drwxr-xr-x   0 daniil    (1000) wheel      (998)        0 2023-03-13 19:40:37.292612 marshmallow-generic-1.0.0/
--rw-r--r--   0 daniil    (1000) wheel      (998)      279 2023-03-13 17:32:03.000000 marshmallow-generic-1.0.0/.gitignore
--rw-r--r--   0 daniil    (1000) wheel      (998)    11357 2023-03-11 15:23:21.000000 marshmallow-generic-1.0.0/LICENSE
--rw-r--r--   0 daniil    (1000) wheel      (998)     4326 2023-03-13 19:40:37.292612 marshmallow-generic-1.0.0/PKG-INFO
--rw-r--r--   0 daniil    (1000) wheel      (998)     3214 2023-03-13 17:51:26.000000 marshmallow-generic-1.0.0/README.md
-drwxr-xr-x   0 daniil    (1000) wheel      (998)        0 2023-03-13 19:40:37.292612 marshmallow-generic-1.0.0/docs/
-drwxr-xr-x   0 daniil    (1000) wheel      (998)        0 2023-03-13 19:40:37.292612 marshmallow-generic-1.0.0/docs/api_reference/
--rw-r--r--   0 daniil    (1000) wheel      (998)       34 2023-03-11 15:23:25.000000 marshmallow-generic-1.0.0/docs/api_reference/decorators.md
--rw-r--r--   0 daniil    (1000) wheel      (998)       31 2023-03-11 15:23:25.000000 marshmallow-generic-1.0.0/docs/api_reference/schema.md
-drwxr-xr-x   0 daniil    (1000) wheel      (998)        0 2023-03-13 19:40:37.292612 marshmallow-generic-1.0.0/docs/css/
--rw-r--r--   0 daniil    (1000) wheel      (998)        0 2023-03-11 15:23:21.000000 marshmallow-generic-1.0.0/docs/css/extra.css
-drwxr-xr-x   0 daniil    (1000) wheel      (998)        0 2023-03-13 19:40:37.292612 marshmallow-generic-1.0.0/docs/img/
--rw-r--r--   0 daniil    (1000) wheel      (998)    48529 2023-03-11 15:33:06.000000 marshmallow-generic-1.0.0/docs/img/ide_suggestion_user.png
--rw-r--r--   0 daniil    (1000) wheel      (998)     3214 2023-03-13 17:51:26.000000 marshmallow-generic-1.0.0/docs/index.md
--rw-r--r--   0 daniil    (1000) wheel      (998)     1318 2023-03-12 23:15:25.000000 marshmallow-generic-1.0.0/mkdocs.yaml
--rw-r--r--   0 daniil    (1000) wheel      (998)     3462 2023-03-13 19:40:15.000000 marshmallow-generic-1.0.0/pyproject.toml
-drwxr-xr-x   0 daniil    (1000) wheel      (998)        0 2023-03-13 19:40:37.292612 marshmallow-generic-1.0.0/requirements/
--rw-r--r--   0 daniil    (1000) wheel      (998)       11 2023-03-11 15:23:21.000000 marshmallow-generic-1.0.0/requirements/common.txt
--rw-r--r--   0 daniil    (1000) wheel      (998)       94 2023-03-11 15:23:25.000000 marshmallow-generic-1.0.0/requirements/dev.txt
-drwxr-xr-x   0 daniil    (1000) wheel      (998)        0 2023-03-13 19:40:37.292612 marshmallow-generic-1.0.0/scripts/
--rwxr-xr-x   0 daniil    (1000) wheel      (998)      473 2023-03-11 15:23:25.000000 marshmallow-generic-1.0.0/scripts/lint.sh
--rwxr-xr-x   0 daniil    (1000) wheel      (998)      750 2023-03-11 15:23:21.000000 marshmallow-generic-1.0.0/scripts/test.sh
--rw-r--r--   0 daniil    (1000) wheel      (998)       38 2023-03-13 19:40:37.292612 marshmallow-generic-1.0.0/setup.cfg
-drwxr-xr-x   0 daniil    (1000) wheel      (998)        0 2023-03-13 19:40:37.292612 marshmallow-generic-1.0.0/src/
-drwxr-xr-x   0 daniil    (1000) wheel      (998)        0 2023-03-13 19:40:37.292612 marshmallow-generic-1.0.0/src/marshmallow_generic/
--rw-r--r--   0 daniil    (1000) wheel      (998)     1519 2023-03-13 19:24:42.000000 marshmallow-generic-1.0.0/src/marshmallow_generic/__init__.py
--rw-r--r--   0 daniil    (1000) wheel      (998)     2876 2023-03-12 17:01:25.000000 marshmallow-generic-1.0.0/src/marshmallow_generic/_util.py
--rw-r--r--   0 daniil    (1000) wheel      (998)     2116 2023-03-11 15:23:25.000000 marshmallow-generic-1.0.0/src/marshmallow_generic/decorators.py
--rw-r--r--   0 daniil    (1000) wheel      (998)        0 2023-03-11 15:23:25.000000 marshmallow-generic-1.0.0/src/marshmallow_generic/py.typed
--rw-r--r--   0 daniil    (1000) wheel      (998)    13472 2023-03-13 14:46:22.000000 marshmallow-generic-1.0.0/src/marshmallow_generic/schema.py
-drwxr-xr-x   0 daniil    (1000) wheel      (998)        0 2023-03-13 19:40:37.292612 marshmallow-generic-1.0.0/src/marshmallow_generic.egg-info/
--rw-r--r--   0 daniil    (1000) wheel      (998)     4326 2023-03-13 19:40:37.000000 marshmallow-generic-1.0.0/src/marshmallow_generic.egg-info/PKG-INFO
--rw-r--r--   0 daniil    (1000) wheel      (998)      770 2023-03-13 19:40:37.000000 marshmallow-generic-1.0.0/src/marshmallow_generic.egg-info/SOURCES.txt
--rw-r--r--   0 daniil    (1000) wheel      (998)        1 2023-03-13 19:40:37.000000 marshmallow-generic-1.0.0/src/marshmallow_generic.egg-info/dependency_links.txt
--rw-r--r--   0 daniil    (1000) wheel      (998)      107 2023-03-13 19:40:37.000000 marshmallow-generic-1.0.0/src/marshmallow_generic.egg-info/requires.txt
--rw-r--r--   0 daniil    (1000) wheel      (998)       20 2023-03-13 19:40:37.000000 marshmallow-generic-1.0.0/src/marshmallow_generic.egg-info/top_level.txt
-drwxr-xr-x   0 daniil    (1000) wheel      (998)        0 2023-03-13 19:40:37.292612 marshmallow-generic-1.0.0/tests/
--rw-r--r--   0 daniil    (1000) wheel      (998)        0 2023-03-13 17:51:14.000000 marshmallow-generic-1.0.0/tests/__init__.py
--rw-r--r--   0 daniil    (1000) wheel      (998)      382 2023-03-11 15:23:25.000000 marshmallow-generic-1.0.0/tests/__main__.py
--rw-r--r--   0 daniil    (1000) wheel      (998)     3488 2023-03-12 17:01:44.000000 marshmallow-generic-1.0.0/tests/test__util.py
--rw-r--r--   0 daniil    (1000) wheel      (998)      962 2023-03-11 15:23:25.000000 marshmallow-generic-1.0.0/tests/test_decorators.py
--rw-r--r--   0 daniil    (1000) wheel      (998)     2971 2023-03-13 14:47:11.000000 marshmallow-generic-1.0.0/tests/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:21:09.160973 marshmallow-generic-1.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:21:09.156973 marshmallow-generic-1.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:21:09.156973 marshmallow-generic-1.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-26 15:20:48.000000 marshmallow-generic-1.0.1/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-26 15:20:48.000000 marshmallow-generic-1.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-26 15:20:48.000000 marshmallow-generic-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-04-26 15:21:09.160973 marshmallow-generic-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-04-26 15:20:48.000000 marshmallow-generic-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:21:09.156973 marshmallow-generic-1.0.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:21:09.156973 marshmallow-generic-1.0.1/docs/api_reference/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-26 15:20:48.000000 marshmallow-generic-1.0.1/docs/api_reference/decorators.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-26 15:20:48.000000 marshmallow-generic-1.0.1/docs/api_reference/schema.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:21:09.156973 marshmallow-generic-1.0.1/docs/css/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 15:20:48.000000 marshmallow-generic-1.0.1/docs/css/extra.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:21:09.156973 marshmallow-generic-1.0.1/docs/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    48529 2023-04-26 15:20:48.000000 marshmallow-generic-1.0.1/docs/img/ide_suggestion_user.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-04-26 15:20:48.000000 marshmallow-generic-1.0.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-04-26 15:20:48.000000 marshmallow-generic-1.0.1/mkdocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-04-26 15:20:48.000000 marshmallow-generic-1.0.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:21:09.156973 marshmallow-generic-1.0.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-26 15:20:48.000000 marshmallow-generic-1.0.1/requirements/common.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-26 15:20:48.000000 marshmallow-generic-1.0.1/requirements/dev.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:21:09.160973 marshmallow-generic-1.0.1/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      317 2023-04-26 15:20:48.000000 marshmallow-generic-1.0.1/scripts/ci.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      306 2023-04-26 15:20:48.000000 marshmallow-generic-1.0.1/scripts/cov.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      382 2023-04-26 15:20:48.000000 marshmallow-generic-1.0.1/scripts/lint.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      394 2023-04-26 15:20:48.000000 marshmallow-generic-1.0.1/scripts/test.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      129 2023-04-26 15:20:48.000000 marshmallow-generic-1.0.1/scripts/typecheck.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-26 15:20:48.000000 marshmallow-generic-1.0.1/scripts/util.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 15:21:09.160973 marshmallow-generic-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:21:09.156973 marshmallow-generic-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:21:09.160973 marshmallow-generic-1.0.1/src/marshmallow_generic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-04-26 15:20:48.000000 marshmallow-generic-1.0.1/src/marshmallow_generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-04-26 15:20:48.000000 marshmallow-generic-1.0.1/src/marshmallow_generic/_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-04-26 15:20:48.000000 marshmallow-generic-1.0.1/src/marshmallow_generic/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 15:20:48.000000 marshmallow-generic-1.0.1/src/marshmallow_generic/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    13579 2023-04-26 15:20:48.000000 marshmallow-generic-1.0.1/src/marshmallow_generic/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:21:09.160973 marshmallow-generic-1.0.1/src/marshmallow_generic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-04-26 15:21:09.000000 marshmallow-generic-1.0.1/src/marshmallow_generic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-04-26 15:21:09.000000 marshmallow-generic-1.0.1/src/marshmallow_generic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 15:21:09.000000 marshmallow-generic-1.0.1/src/marshmallow_generic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-26 15:21:09.000000 marshmallow-generic-1.0.1/src/marshmallow_generic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-26 15:21:09.000000 marshmallow-generic-1.0.1/src/marshmallow_generic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:21:09.160973 marshmallow-generic-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 15:20:48.000000 marshmallow-generic-1.0.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-26 15:20:48.000000 marshmallow-generic-1.0.1/tests/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-04-26 15:20:48.000000 marshmallow-generic-1.0.1/tests/test__util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-04-26 15:20:48.000000 marshmallow-generic-1.0.1/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-04-26 15:20:48.000000 marshmallow-generic-1.0.1/tests/test_schema.py
```

### Comparing `marshmallow-generic-1.0.0/LICENSE` & `marshmallow-generic-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `marshmallow-generic-1.0.0/PKG-INFO` & `marshmallow-generic-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: marshmallow-generic
-Version: 1.0.0
+Version: 1.0.1
 Summary: Generic schema with full typing support and minimal boilerplate
 Author-email: Daniil Fajnberg <mail@daniil.fajnberg.de>
 Maintainer-email: Daniil Fajnberg <mail@daniil.fajnberg.de>
 License: Apache Software License Version 2.0
-Project-URL: repository, https://github.com/daniil-berg/marshmallow-generic
-Project-URL: bug_tracker, https://github.com/daniil-berg/marshmallow-generic/issues
-Project-URL: documentation, http://daniil-berg.github.io/marshmallow-generic
+Project-URL: Repository, https://github.com/daniil-berg/marshmallow-generic
+Project-URL: Issue Tracker, https://github.com/daniil-berg/marshmallow-generic/issues
+Project-URL: Documentation, http://daniil-berg.github.io/marshmallow-generic
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Developers
 Classifier: Typing :: Typed
 Requires-Python: <4.0,>=3.9
 Description-Content-Type: text/markdown
-Provides-Extra: full
 Provides-Extra: dev
 License-File: LICENSE
 
 # marshmallow-generic
 
 **Generic schema with full typing support and minimal boilerplate**
```

### Comparing `marshmallow-generic-1.0.0/README.md` & `marshmallow-generic-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `marshmallow-generic-1.0.0/docs/img/ide_suggestion_user.png` & `marshmallow-generic-1.0.1/docs/img/ide_suggestion_user.png`

 * *Files identical despite different names*

### Comparing `marshmallow-generic-1.0.0/docs/index.md` & `marshmallow-generic-1.0.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `marshmallow-generic-1.0.0/mkdocs.yaml` & `marshmallow-generic-1.0.1/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `marshmallow-generic-1.0.0/pyproject.toml` & `marshmallow-generic-1.0.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -33,32 +33,29 @@
 dynamic = [
     "dependencies",
     "readme",
     "version",
 ]
 
 [project.optional-dependencies]
-full = [
-
-]
 dev = [
-    "black",
-    "build",
-    "coverage[toml]",
-    "isort",
-    "mkdocs-material",
-    "mkdocstrings[python]",
-    "mypy",
-    "ruff",
+    "black==23.3.0",
+    "build==0.10.0",
+    "coverage[toml]==7.2.3",
+    "isort==5.12.0",
+    "mkdocs-material==9.1.6",
+    "mkdocstrings[python]==0.21.2",
+    "mypy==1.2.0",
+    "ruff==0.0.262",
 ]
 
 [project.urls]
-repository = "https://github.com/daniil-berg/marshmallow-generic"
-bug_tracker = "https://github.com/daniil-berg/marshmallow-generic/issues"
-documentation = "http://daniil-berg.github.io/marshmallow-generic"
+"Repository" = "https://github.com/daniil-berg/marshmallow-generic"
+"Issue Tracker" = "https://github.com/daniil-berg/marshmallow-generic/issues"
+"Documentation" = "http://daniil-berg.github.io/marshmallow-generic"
 
 [tool.setuptools.dynamic]
 dependencies = { file = "requirements/common.txt" }
 readme = { file = ["README.md"], content-type = "text/markdown" }
 version = { attr = "marshmallow_generic.__version__" }
 
 #########################
```

### Comparing `marshmallow-generic-1.0.0/src/marshmallow_generic/__init__.py` & `marshmallow-generic-1.0.1/src/marshmallow_generic/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License."""
 
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 
 __doc__ = """
 Generic schema with full typing support and minimal boilerplate.
 """
 
 __all__ = [
     # Custom:
@@ -38,18 +38,16 @@
     # "post_load",
     "pprint",
     "ValidationError",
     "missing",
 ]
 
 from marshmallow import fields
-
-from marshmallow.decorators import (
+from marshmallow.decorators import (  # `post_load` overloaded
     post_dump,
-    # post_load,  # overloaded
     pre_dump,
     pre_load,
     validates,
     validates_schema,
 )
 from marshmallow.exceptions import ValidationError
 from marshmallow.schema import Schema, SchemaOpts
```

### Comparing `marshmallow-generic-1.0.0/src/marshmallow_generic/_util.py` & `marshmallow-generic-1.0.1/src/marshmallow_generic/_util.py`

 * *Files identical despite different names*

### Comparing `marshmallow-generic-1.0.0/src/marshmallow_generic/decorators.py` & `marshmallow-generic-1.0.1/src/marshmallow_generic/decorators.py`

 * *Files identical despite different names*

### Comparing `marshmallow-generic-1.0.0/src/marshmallow_generic/schema.py` & `marshmallow-generic-1.0.1/src/marshmallow_generic/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,19 @@
 from marshmallow import Schema
 
 from ._util import GenericInsightMixin1
 from .decorators import post_load
 
 Model = TypeVar("Model")
 
+MANY_SCHEMA_UNSAFE = (
+    "Changing `many` schema-wide breaks type safety. "
+    "Use the the `many` parameter of specific methods (like `load`) instead."
+)
+
 
 class GenericSchema(GenericInsightMixin1[Model], Schema):
     """
     Generic schema parameterized by a **`Model`** class.
 
     Data will always be deserialized to instances of that **`Model`** class.
 
@@ -96,37 +101,36 @@
                     will therefore trigger a warning. You should instead use
                     the method-specific `many` parameter, when calling
                     [`dump`][marshmallow_generic.GenericSchema.dump]/
                     [`dumps`][marshmallow_generic.GenericSchema.dumps] or
                     [`load`][marshmallow_generic.GenericSchema.load]/
                     [`loads`][marshmallow_generic.GenericSchema.loads].
         """
+        self._pre_init = True
         super().__init__(
             only=only,
             exclude=exclude,
             many=many,
             context=context,
             load_only=load_only,
             dump_only=dump_only,
             partial=partial,
             unknown=unknown,
         )
+        self._pre_init = False
 
     def __setattr__(self, name: str, value: Any) -> None:
         """
         Warns, when trying to set `many` to anything other than `False`.
 
         Otherwise the same the normal
         [`object.__setattr__`](https://docs.python.org/3/reference/datamodel.html#object.__setattr__).
         """
         if name == "many" and value is not False:
-            warn(
-                "Changing `many` schema-wide breaks type safety. Use the the "
-                "`many` parameter of specific methods (like `load`) instead."
-            )
+            warn(MANY_SCHEMA_UNSAFE, stacklevel=4 if self._pre_init else 2)
         super().__setattr__(name, value)
 
     @post_load
     def instantiate(self, data: dict[str, Any], **_kwargs: Any) -> Model:
         """
         Unpacks `data` into the constructor of the specified **`Model`**.
```

### Comparing `marshmallow-generic-1.0.0/src/marshmallow_generic.egg-info/PKG-INFO` & `marshmallow-generic-1.0.1/src/marshmallow_generic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: marshmallow-generic
-Version: 1.0.0
+Version: 1.0.1
 Summary: Generic schema with full typing support and minimal boilerplate
 Author-email: Daniil Fajnberg <mail@daniil.fajnberg.de>
 Maintainer-email: Daniil Fajnberg <mail@daniil.fajnberg.de>
 License: Apache Software License Version 2.0
-Project-URL: repository, https://github.com/daniil-berg/marshmallow-generic
-Project-URL: bug_tracker, https://github.com/daniil-berg/marshmallow-generic/issues
-Project-URL: documentation, http://daniil-berg.github.io/marshmallow-generic
+Project-URL: Repository, https://github.com/daniil-berg/marshmallow-generic
+Project-URL: Issue Tracker, https://github.com/daniil-berg/marshmallow-generic/issues
+Project-URL: Documentation, http://daniil-berg.github.io/marshmallow-generic
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Developers
 Classifier: Typing :: Typed
 Requires-Python: <4.0,>=3.9
 Description-Content-Type: text/markdown
-Provides-Extra: full
 Provides-Extra: dev
 License-File: LICENSE
 
 # marshmallow-generic
 
 **Generic schema with full typing support and minimal boilerplate**
```

### Comparing `marshmallow-generic-1.0.0/src/marshmallow_generic.egg-info/SOURCES.txt` & `marshmallow-generic-1.0.1/src/marshmallow_generic.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 .gitignore
 LICENSE
 README.md
 mkdocs.yaml
 pyproject.toml
+.github/workflows/ci.yaml
 docs/index.md
 docs/api_reference/decorators.md
 docs/api_reference/schema.md
 docs/css/extra.css
 docs/img/ide_suggestion_user.png
 requirements/common.txt
 requirements/dev.txt
+scripts/ci.sh
+scripts/cov.sh
 scripts/lint.sh
 scripts/test.sh
+scripts/typecheck.sh
+scripts/util.sh
 src/marshmallow_generic/__init__.py
 src/marshmallow_generic/_util.py
 src/marshmallow_generic/decorators.py
 src/marshmallow_generic/py.typed
 src/marshmallow_generic/schema.py
 src/marshmallow_generic.egg-info/PKG-INFO
 src/marshmallow_generic.egg-info/SOURCES.txt
```

### Comparing `marshmallow-generic-1.0.0/tests/test__util.py` & `marshmallow-generic-1.0.1/tests/test__util.py`

 * *Files identical despite different names*

### Comparing `marshmallow-generic-1.0.0/tests/test_decorators.py` & `marshmallow-generic-1.0.1/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `marshmallow-generic-1.0.0/tests/test_schema.py` & `marshmallow-generic-1.0.1/tests/test_schema.py`

 * *Files identical despite different names*

