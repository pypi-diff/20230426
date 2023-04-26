# Comparing `tmp/use_case_registry-1.4.9.tar.gz` & `tmp/use_case_registry-1.5.0.tar.gz`

## Comparing `use_case_registry-1.4.9.tar` & `use_case_registry-1.5.0.tar`

### file list

```diff
@@ -1,53 +1,51 @@
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/.tool-versions
--rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/Makefile
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/mkdocs.yml
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/.github/CODEOWNERS
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/.github/workflows/audit.yml
--rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/.github/workflows/coverage.yml
--rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/.github/workflows/release.yml
--rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/.github/workflows/test.yml
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/.github/workflows/update_docs.yml
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/.vscode/settings.json
--rw-r--r--   0        0        0     4123 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/docs/index.md
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/docs/general-thoughts/clean-architecture/index.md
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/docs/general-thoughts/error-handling/index.md
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/docs/general-thoughts/one-use-case-one-workflow/index.md
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/requirements/core.txt
--rw-r--r--   0        0        0     4612 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/requirements/dev.txt
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/requirements/sqlalchemy.txt
--rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/scripts/release_github.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/tests/__init__.py
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/tests/test_enums.py
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/tests/test_registry.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/tests/assets/templates/target-based/config-1.yml
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/tests/assets/templates/target-based/config-2.yml
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/tests/assets/templates/target-based/config-3.yml
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/tests/assets/templates/target-based/config-4.yml
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/tests/assets/templates/target-based/config-5.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/tests/base/__init__.py
--rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/tests/base/test_command.py
--rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/tests/base/test_repository.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/tests/parsers/__init__.py
--rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/tests/parsers/test_target_based.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/use_case_registry/__about__.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/use_case_registry/__init__.py
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/use_case_registry/enums.py
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/use_case_registry/errors.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/use_case_registry/py.typed
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/use_case_registry/registry.py
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/use_case_registry/base/__init__.py
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/use_case_registry/base/command.py
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/use_case_registry/base/repository.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/use_case_registry/base/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/use_case_registry/internals/__init__.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/use_case_registry/internals/errors.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/use_case_registry/pasers/__init__.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/use_case_registry/pasers/macros.py
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/use_case_registry/pasers/target_based.py
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/.gitignore
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/LICENSE.txt
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/README.md
--rw-r--r--   0        0        0     3978 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/pyproject.toml
--rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 use_case_registry-1.4.9/PKG-INFO
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 use_case_registry-1.5.0/.tool-versions
+-rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 use_case_registry-1.5.0/Makefile
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 use_case_registry-1.5.0/mkdocs.yml
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 use_case_registry-1.5.0/.github/CODEOWNERS
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 use_case_registry-1.5.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 use_case_registry-1.5.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 use_case_registry-1.5.0/.github/workflows/audit.yml
+-rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 use_case_registry-1.5.0/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 use_case_registry-1.5.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 use_case_registry-1.5.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 use_case_registry-1.5.0/.github/workflows/update_docs.yml
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 use_case_registry-1.5.0/.vscode/settings.json
+-rw-r--r--   0        0        0     4123 2020-02-02 00:00:00.000000 use_case_registry-1.5.0/docs/index.md
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 use_case_registry-1.5.0/docs/general-thoughts/clean-architecture/index.md
+-rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 use_case_registry-1.5.0/docs/general-thoughts/error-handling/index.md
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 use_case_registry-1.5.0/docs/general-thoughts/one-use-case-one-workflow/index.md
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 use_case_registry-1.5.0/requirements/core.txt
+-rw-r--r--   0        0        0     4612 2020-02-02 00:00:00.000000 use_case_registry-1.5.0/requirements/dev.txt
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 use_case_registry-1.5.0/requirements/sqlalchemy.txt
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 use_case_registry-1.5.0/scripts/release_github.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.5.0/tests/__init__.py
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 use_case_registry-1.5.0/tests/test_enums.py
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 use_case_registry-1.5.0/tests/test_registry.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 use_case_registry-1.5.0/tests/assets/templates/raw/config-1.yml
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 use_case_registry-1.5.0/tests/assets/templates/raw/config-2.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.5.0/tests/base/__init__.py
+-rw-r--r--   0        0        0     2921 2020-02-02 00:00:00.000000 use_case_registry-1.5.0/tests/base/test_command.py
+-rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 use_case_registry-1.5.0/tests/base/test_repository.py
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 use_case_registry-1.5.0/tests/base/test_schema_validator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.5.0/tests/parsers/__init__.py
+-rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 use_case_registry-1.5.0/tests/parsers/test_raw.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 use_case_registry-1.5.0/use_case_registry/__about__.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 use_case_registry-1.5.0/use_case_registry/__init__.py
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 use_case_registry-1.5.0/use_case_registry/enums.py
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 use_case_registry-1.5.0/use_case_registry/errors.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.5.0/use_case_registry/py.typed
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 use_case_registry-1.5.0/use_case_registry/registry.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.5.0/use_case_registry/base/__init__.py
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 use_case_registry-1.5.0/use_case_registry/base/command.py
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 use_case_registry-1.5.0/use_case_registry/base/repository.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 use_case_registry-1.5.0/use_case_registry/base/schema_validator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.5.0/use_case_registry/internals/__init__.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 use_case_registry-1.5.0/use_case_registry/internals/errors.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.5.0/use_case_registry/pasers/__init__.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 use_case_registry-1.5.0/use_case_registry/pasers/macros.py
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 use_case_registry-1.5.0/use_case_registry/pasers/raw.py
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 use_case_registry-1.5.0/.gitignore
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 use_case_registry-1.5.0/LICENSE.txt
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 use_case_registry-1.5.0/README.md
+-rw-r--r--   0        0        0     3978 2020-02-02 00:00:00.000000 use_case_registry-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 use_case_registry-1.5.0/PKG-INFO
```

### Comparing `use_case_registry-1.4.9/Makefile` & `use_case_registry-1.5.0/Makefile`

 * *Files 3% similar despite different names*

```diff
@@ -65,10 +65,14 @@
 serve-docs: ## Serve project documentation
 	@mkdocs serve
 
 .PHONY: build-docs
 build-docs:
 	@mkdocs build
 
+.PHONY: reload-settings
+reload-settings: ## Reload settings from pyproject.toml
+	@touch pyproject.toml
+
 .PHONY: help
 help:
 	@grep -h -E '^[a-zA-Z_-]+:.*?## .*$$' $(MAKEFILE_LIST) | awk 'BEGIN {FS = ":.*?## "}; {printf "\033[36m%-10s\033[0m %s\n", $$1, $$2}'
```

### Comparing `use_case_registry-1.4.9/mkdocs.yml` & `use_case_registry-1.5.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.9/.github/ISSUE_TEMPLATE/bug_report.md` & `use_case_registry-1.5.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.9/.github/ISSUE_TEMPLATE/feature_request.md` & `use_case_registry-1.5.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.9/.github/workflows/audit.yml` & `use_case_registry-1.5.0/.github/workflows/audit.yml`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.9/.github/workflows/coverage.yml` & `use_case_registry-1.5.0/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.9/.github/workflows/release.yml` & `use_case_registry-1.5.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.9/.github/workflows/test.yml` & `use_case_registry-1.5.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.9/.vscode/settings.json` & `use_case_registry-1.5.0/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.9/docs/index.md` & `use_case_registry-1.5.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.9/docs/general-thoughts/clean-architecture/index.md` & `use_case_registry-1.5.0/docs/general-thoughts/clean-architecture/index.md`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.9/docs/general-thoughts/error-handling/index.md` & `use_case_registry-1.5.0/docs/general-thoughts/error-handling/index.md`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.9/docs/general-thoughts/one-use-case-one-workflow/index.md` & `use_case_registry-1.5.0/docs/general-thoughts/one-use-case-one-workflow/index.md`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.9/requirements/core.txt` & `use_case_registry-1.5.0/requirements/core.txt`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.9/requirements/dev.txt` & `use_case_registry-1.5.0/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.9/requirements/sqlalchemy.txt` & `use_case_registry-1.5.0/requirements/sqlalchemy.txt`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.9/scripts/release_github.py` & `use_case_registry-1.5.0/scripts/release_github.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.9/tests/test_registry.py` & `use_case_registry-1.5.0/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.9/tests/base/test_repository.py` & `use_case_registry-1.5.0/tests/base/test_repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from typing import Any
 
 import pytest
 from result import Result
 
 from use_case_registry import UseCaseRegistry
-from use_case_registry.base import IRepository
+from use_case_registry.base.repository import IRepository
 from use_case_registry.errors import CommitTransactionsError
 
 
 class TestICommand:
     """Test definition for ICommand."""
 
     def test_cannot_be_instantiated(self) -> None:
```

### Comparing `use_case_registry-1.4.9/tests/parsers/test_target_based.py` & `use_case_registry-1.5.0/tests/parsers/test_raw.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,96 +1,97 @@
 """Test target-based parser."""
 import os
 import pathlib
 from typing import Any
 from unittest import mock
 
 import pytest
-from pydantic import BaseModel
 
-from use_case_registry.errors import CommandInputValidationError, EnvVarMissingError
-from use_case_registry.pasers.target_based import TargetBasedConfigParser
+from use_case_registry.base.schema_validator import SchemaValidator
+from use_case_registry.errors import EnvVarMissingError
+from use_case_registry.pasers.raw import RawConfigParser
 
 
-class _Schema(BaseModel):
+class _Schema(SchemaValidator):
     name: str
     last_name: str
 
 
-class _OtherSchema(BaseModel):
+class _OtherSchema(SchemaValidator):
     other: str
 
 
 class TestTargetBasedConfigParser:  # noqa: D101
     @mock.patch.dict(
         os.environ,
-        {
-            "EXECUTION_ENV_MOCKED": "mock",
-        },
+        {},
         clear=True,
     )
     @pytest.mark.parametrize(
         argnames=["template", "expected_result"],
         argvalues=[
             (
                 "config-1.yml",
                 {
                     "name": "t",
                     "last_name": "p",
                 },
             ),
-            (
-                "config-4.yml",
-                {
-                    "name": "t",
-                    "last_name": "p",
-                },
-            ),
         ],
     )
     def test_parse_works(self, template: str, expected_result: dict[str, Any]) -> None:
         """Test parse works as expected."""
-        folder = pathlib.Path().cwd().joinpath("tests/assets/templates/target-based/")
-        parser = TargetBasedConfigParser(path_to_folder=folder)
-        result = parser.parse(template=template, schema=_Schema)
+        folder = pathlib.Path().cwd().joinpath("tests/assets/templates/raw/")
+        parser = RawConfigParser(path_to_folder=folder)
+        result = parser.parse(template=template).unwrap()
+        _Schema(**result)
         assert result == expected_result
 
+    @mock.patch.dict(
+        os.environ,
+        {
+            "NAME": "tomas",
+            "LAST_NAME": "perez",
+        },
+        clear=True,
+    )
     @pytest.mark.parametrize(
-        argnames=["template", "schema"],
+        argnames=["template", "expected_result"],
         argvalues=[
             (
-                "config-2.yml",
-                _Schema,
-            ),
-            (
-                "config-5.yml",
-                _Schema,
-            ),
-            (
                 "config-1.yml",
-                _OtherSchema,
+                {
+                    "name": "tomas",
+                    "last_name": "perez",
+                },
             ),
         ],
     )
-    def test_parse_fails_validation(
+    def test_parse_works_using_env_variables(
         self,
         template: str,
-        schema: type[BaseModel],
+        expected_result: dict[str, Any],
     ) -> None:
         """Test parse works as expected."""
-        folder = pathlib.Path().cwd().joinpath("tests/assets/templates/target-based/")
-        parser = TargetBasedConfigParser(path_to_folder=folder)
-        with pytest.raises(CommandInputValidationError):
-            parser.parse(template=template, schema=schema)
+        folder = pathlib.Path().cwd().joinpath("tests/assets/templates/raw/")
+        parser = RawConfigParser(path_to_folder=folder)
+        result = parser.parse(template=template).unwrap()
+        _Schema(**result)
+        assert result == expected_result
 
     @pytest.mark.parametrize(
         argnames="template",
         argvalues=[
-            "config-3.yml",
+            "config-2.yml",
         ],
     )
-    def test_parse_fails_missing_env_var(self, template: str) -> None:
+    def test_parse_env_var_missing(
+        self,
+        template: str,
+    ) -> None:
         """Test parse works as expected."""
-        folder = pathlib.Path().cwd().joinpath("tests/assets/templates/target-based/")
-        parser = TargetBasedConfigParser(path_to_folder=folder)
-        with pytest.raises(EnvVarMissingError):
-            parser.parse(template=template, schema=_Schema)
+        folder = pathlib.Path().cwd().joinpath("tests/assets/templates/raw/")
+        parser = RawConfigParser(path_to_folder=folder)
+
+        parse_err = parser.parse(template=template).err()
+
+        assert isinstance(parse_err, EnvVarMissingError)
```

### Comparing `use_case_registry-1.4.9/use_case_registry/enums.py` & `use_case_registry-1.5.0/use_case_registry/enums.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.9/use_case_registry/errors.py` & `use_case_registry-1.5.0/use_case_registry/errors.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,49 +1,42 @@
 """Custom defined errors."""
 
-import pathlib
-from typing import TYPE_CHECKING, Any, Union
 
-from use_case_registry import UseCaseRegistry
-
-if TYPE_CHECKING:
-    from pydantic.error_wrappers import ErrorDict
 
 
 class CommandInputValidationError(Exception):
     """Raised when command input values does pass validation check."""
 
-    def __init__(self, msg: Union[str, list["ErrorDict"]]) -> None:
+    def __init__(self, msg: str) -> None:
         """Construct class."""
         super().__init__(msg)
 
 
 class UseCaseExecutionError(Exception):
     """Raised when there's an error executing a workflow."""
 
     def __init__(self, error: Exception) -> None:
         """Construct class."""
-        super().__init__(f"Error executing a use case {error}")
+        super().__init__(f"{error}")
 
 
 class CommitTransactionsError(Exception):
     """Raised when there's an error committing a set of transactions."""
 
-    def __init__(self, transactions: UseCaseRegistry[Any]) -> None:
+    def __init__(self) -> None:
         """Construct class."""
-        super().__init__(f"Error commiting transactions {transactions}")
+        super().__init__("Error commiting transactions")
 
 
 class EnvVarMissingError(Exception):
     """Raised when a required enviroment variable is not set."""
 
     def __init__(self, env_var: str) -> None:
         """Construct class."""
         super().__init__(f"Env var required but not provided {env_var}")
 
 
-class SchemaNotFoundError(Exception):
-    """Raised when schema not found."""
+class NotIndentifiedError(Exception):
+    """Raised when a not-indetified error happens."""
 
-    def __init__(self, path: pathlib.Path) -> None:
-        """Construct class."""
-        super().__init__(f"Schema not found {path}")
+    def __init__(self, unkown_err: Exception) -> None:  # noqa: D107
+        super().__init__(unkown_err)
```

### Comparing `use_case_registry-1.4.9/use_case_registry/registry.py` & `use_case_registry-1.5.0/use_case_registry/registry.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.9/use_case_registry/base/command.py` & `use_case_registry-1.5.0/use_case_registry/base/command.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Interface for concrete commands."""
 import abc
 from dataclasses import dataclass
-from typing import Any
+from typing import Any, Union
 
 from mashumaro.mixins.orjson import DataClassORJSONMixin
 from result import Result
 
 from use_case_registry import UseCaseRegistry
-from use_case_registry.errors import UseCaseExecutionError
+from use_case_registry.errors import CommandInputValidationError, UseCaseExecutionError
 
 
 @dataclass(
     frozen=True,
 )
 class ICommandInput(DataClassORJSONMixin):
     """ICommandInput."""
@@ -20,9 +20,20 @@
 class BaseCommand(abc.ABC):
     """Command abstract class."""
 
     @abc.abstractmethod
     def execute(
         self,
         write_ops_registry: UseCaseRegistry[Any],
-    ) -> Result[Any, UseCaseExecutionError]:
+    ) -> Result[Any, Union[CommandInputValidationError, UseCaseExecutionError]]:
+        """Workflow execution command to complete the use case."""
+
+
+class AsyncBaseCommand(abc.ABC):
+    """Async command abstract class."""
+
+    @abc.abstractmethod
+    async def execute(
+        self,
+        write_ops_registry: UseCaseRegistry[Any],
+    ) -> Result[Any, Union[CommandInputValidationError, UseCaseExecutionError]]:
         """Workflow execution command to complete the use case."""
```

### Comparing `use_case_registry-1.4.9/use_case_registry/base/repository.py` & `use_case_registry-1.5.0/use_case_registry/base/repository.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.9/use_case_registry/internals/errors.py` & `use_case_registry-1.5.0/use_case_registry/internals/errors.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.9/use_case_registry/pasers/macros.py` & `use_case_registry-1.5.0/use_case_registry/pasers/macros.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.9/.gitignore` & `use_case_registry-1.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.9/LICENSE.txt` & `use_case_registry-1.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.9/README.md` & `use_case_registry-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.9/pyproject.toml` & `use_case_registry-1.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.9/PKG-INFO` & `use_case_registry-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: use_case_registry
-Version: 1.4.9
+Version: 1.5.0
 Summary: Registry class for Use Case implementation. They are basically meaningfull lists with some constraints.
 Project-URL: Homepage, https://github.com/Tomperez98/use-case-registry
 Project-URL: Documentation, https://tomperez98.github.io/use-case-registry/
 Project-URL: Issues, https://github.com/Tomperez98/use-case-registry/issues
 Project-URL: Source, https://github.com/Tomperez98/use-case-registry
 Author-email: Tomas Perez Alvarez <tomasperezalvarez@gmail.com>
 License-Expression: MIT
```

