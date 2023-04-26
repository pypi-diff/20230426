# Comparing `tmp/py-bdd-context-0.0.3.tar.gz` & `tmp/py-bdd-context-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-bdd-context-0.0.3.tar", max compression
+gzip compressed data, was "py-bdd-context-0.0.4.tar", max compression
```

## Comparing `py-bdd-context-0.0.3.tar` & `py-bdd-context-0.0.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      319 2023-01-26 17:55:25.636211 py-bdd-context-0.0.3/README.md
--rw-r--r--   0        0        0       93 2023-01-26 17:55:52.076469 py-bdd-context-0.0.3/py_bdd_context/__init__.py
--rw-r--r--   0        0        0     1923 2023-01-26 17:55:25.636211 py-bdd-context-0.0.3/py_bdd_context/bdd_context.py
--rw-r--r--   0        0        0     1305 2023-01-26 17:55:25.636211 py-bdd-context-0.0.3/py_bdd_context/test_case.py
--rw-r--r--   0        0        0     1835 2023-01-26 17:55:25.636211 py-bdd-context-0.0.3/py_bdd_context/test_file_helper.py
--rw-r--r--   0        0        0     1748 2023-01-26 17:55:52.040469 py-bdd-context-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      950 2023-01-26 17:55:52.671836 py-bdd-context-0.0.3/setup.py
--rw-r--r--   0        0        0     1358 2023-01-26 17:55:52.672193 py-bdd-context-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      319 2023-04-26 19:05:59.592963 py-bdd-context-0.0.4/README.md
+-rw-r--r--   0        0        0       93 2023-04-26 19:06:23.928951 py-bdd-context-0.0.4/py_bdd_context/__init__.py
+-rw-r--r--   0        0        0     1923 2023-04-26 19:05:59.592963 py-bdd-context-0.0.4/py_bdd_context/bdd_context.py
+-rw-r--r--   0        0        0     1334 2023-04-26 19:05:59.592963 py-bdd-context-0.0.4/py_bdd_context/test_case.py
+-rw-r--r--   0        0        0     1835 2023-04-26 19:05:59.592963 py-bdd-context-0.0.4/py_bdd_context/test_file_helper.py
+-rw-r--r--   0        0        0     1748 2023-04-26 19:06:23.892951 py-bdd-context-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      950 2023-04-26 19:06:24.434234 py-bdd-context-0.0.4/setup.py
+-rw-r--r--   0        0        0     1358 2023-04-26 19:06:24.434516 py-bdd-context-0.0.4/PKG-INFO
```

### Comparing `py-bdd-context-0.0.3/py_bdd_context/bdd_context.py` & `py-bdd-context-0.0.4/py_bdd_context/bdd_context.py`

 * *Files identical despite different names*

### Comparing `py-bdd-context-0.0.3/py_bdd_context/test_case.py` & `py-bdd-context-0.0.4/py_bdd_context/test_case.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,41 +5,41 @@
 
 
 class BDDContextTestCase(TestCase):
     given = given
     when = when
     then = then
 
-    def testDescriptionInfo(self):
+    def get_test_description_info(self):
         """
         Returns:
             list with infos about the test path and line number
         """
         test_lineno = TestFileHelper().get_test_method_line_number_for_test(
             self, self._testMethodName
         )
         return ["", f"{test_lineno} | teste"]
 
-    def bddDescriptionInfo(self):
+    def get_bdd_description_info(self):
         """
         Note:
             this method trusts on the injection of the attribute _aditional_bdd_description_infos in # noqa
             the test instance.
 
         Returns:
             list with infos about the BDD step
         """
         return getattr(self, "_aditional_bdd_description_infos", [])
 
-    def shortDescription(self):
+    def get_short_description(self):
         """
         Returns:
             test description with additional infos
         """
-        original_description = super().shortDescription()
+        original_description = super().get_short_description()
 
         if not isinstance(original_description, str):
             original_description = ""
 
-        infos = ["", *self.testDescriptionInfo(), *self.bddDescriptionInfo()]
+        infos = ["", *self.get_description_info(), *self.get_bdd_description_info()]
 
         return original_description + "\n".join(infos)
```

### Comparing `py-bdd-context-0.0.3/py_bdd_context/test_file_helper.py` & `py-bdd-context-0.0.4/py_bdd_context/test_file_helper.py`

 * *Files identical despite different names*

### Comparing `py-bdd-context-0.0.3/pyproject.toml` & `py-bdd-context-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 	"*/tests/*",
 	"*/examples/*",
 	"*/__init__.py"
 ]
 
 [tool.poetry]
 name = "py-bdd-context"
-version = "0.0.3"
+version = "0.0.4"
 description = "Biblioteca com Context Manager para facilitar os testes de Behavior Driven Development (BDD)"
 authors = ["Imobanco"]
 readme = "README.md"
 packages = [{include = "py_bdd_context/**/*.py"}]
 homepage = "https://github.com/imobanco/py-bdd-context"
 repository = "https://github.com/imobanco/py-bdd-context"
 license = "GPLv3"
```

### Comparing `py-bdd-context-0.0.3/setup.py` & `py-bdd-context-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['py_bdd_context']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'py-bdd-context',
-    'version': '0.0.3',
+    'version': '0.0.4',
     'description': 'Biblioteca com Context Manager para facilitar os testes de Behavior Driven Development (BDD)',
     'long_description': '# py-bdd-context\n\nLibrary with Context Manager to facilitate Behavior Driven Development (BDD) tests.\n\nThis library will help you organize your tests!\n\n## Using\nThere are examples of how to use the lib in the `examples` folder.\n\n\n## Installing\nhttps://pypi.org/project/py-bdd-context/\n```\npip install py-bdd-context\n```',
     'author': 'Imobanco',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/imobanco/py-bdd-context',
```

### Comparing `py-bdd-context-0.0.3/PKG-INFO` & `py-bdd-context-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-bdd-context
-Version: 0.0.3
+Version: 0.0.4
 Summary: Biblioteca com Context Manager para facilitar os testes de Behavior Driven Development (BDD)
 Home-page: https://github.com/imobanco/py-bdd-context
 License: GPLv3
 Keywords: BDD,Context Manager,tests
 Author: Imobanco
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
```

