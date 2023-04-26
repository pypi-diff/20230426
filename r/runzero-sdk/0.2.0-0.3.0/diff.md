# Comparing `tmp/runzero_sdk-0.2.0.tar.gz` & `tmp/runzero_sdk-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runzero_sdk-0.2.0.tar", max compression
+gzip compressed data, was "runzero_sdk-0.3.0.tar", max compression
```

## Comparing `runzero_sdk-0.2.0.tar` & `runzero_sdk-0.3.0.tar`

### file list

```diff
@@ -1,29 +1,33 @@
--rw-r--r--   0        0        0      193 2023-04-11 04:00:57.041114 runzero_sdk-0.2.0/LICENSE
--rw-r--r--   0        0        0     6467 2023-04-11 04:00:57.041114 runzero_sdk-0.2.0/README.md
--rw-r--r--   0        0        0     4402 2023-04-11 04:00:57.045113 runzero_sdk-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      507 2023-04-11 04:00:57.045113 runzero_sdk-0.2.0/runzero/__init__.py
--rw-r--r--   0        0        0      423 2023-04-11 04:00:57.045113 runzero_sdk-0.2.0/runzero/api/__init__.py
--rw-r--r--   0        0        0      346 2023-04-11 04:00:57.045113 runzero_sdk-0.2.0/runzero/api/admin/__init__.py
--rw-r--r--   0        0        0    11425 2023-04-11 04:00:57.045113 runzero_sdk-0.2.0/runzero/api/admin/_sdk_source_icon.py
--rw-r--r--   0        0        0     5728 2023-04-11 04:00:57.045113 runzero_sdk-0.2.0/runzero/api/admin/custom_integrations.py
--rw-r--r--   0        0        0     3462 2023-04-11 04:00:57.045113 runzero_sdk-0.2.0/runzero/api/admin/orgs.py
--rw-r--r--   0        0        0     2775 2023-04-11 04:00:57.045113 runzero_sdk-0.2.0/runzero/api/custom_integrations.py
--rw-r--r--   0        0        0      274 2023-04-11 04:00:57.045113 runzero_sdk-0.2.0/runzero/api/imports/__init__.py
--rw-r--r--   0        0        0     4675 2023-04-11 04:00:57.045113 runzero_sdk-0.2.0/runzero/api/imports/assets.py
--rw-r--r--   0        0        0     4409 2023-04-11 04:00:57.045113 runzero_sdk-0.2.0/runzero/api/sites.py
--rw-r--r--   0        0        0     3167 2023-04-11 04:00:57.045113 runzero_sdk-0.2.0/runzero/api/tasks.py
--rw-r--r--   0        0        0      441 2023-04-11 04:00:57.045113 runzero_sdk-0.2.0/runzero/client/__init__.py
--rw-r--r--   0        0        0      318 2023-04-11 04:00:57.045113 runzero_sdk-0.2.0/runzero/client/_http/__init__.py
--rw-r--r--   0        0        0     2496 2023-04-11 04:00:57.045113 runzero_sdk-0.2.0/runzero/client/_http/auth.py
--rw-r--r--   0        0        0     8637 2023-04-11 04:00:57.045113 runzero_sdk-0.2.0/runzero/client/_http/io.py
--rw-r--r--   0        0        0    11384 2023-04-11 04:00:57.045113 runzero_sdk-0.2.0/runzero/client/client.py
--rw-r--r--   0        0        0     6443 2023-04-11 04:00:57.045113 runzero_sdk-0.2.0/runzero/client/errors.py
--rw-r--r--   0        0        0     1077 2023-04-11 04:00:57.045113 runzero_sdk-0.2.0/runzero/errors.py
--rw-r--r--   0        0        0        0 2023-04-11 04:00:57.045113 runzero_sdk-0.2.0/runzero/py.typed
--rw-r--r--   0        0        0     1298 2023-04-11 04:00:57.045113 runzero_sdk-0.2.0/runzero/types/__init__.py
--rw-r--r--   0        0        0    18695 2023-04-11 04:00:57.045113 runzero_sdk-0.2.0/runzero/types/_data_models_gen.py
--rw-r--r--   0        0        0     2319 2023-04-11 04:00:57.045113 runzero_sdk-0.2.0/runzero/types/_rate_limit_information.py
--rw-r--r--   0        0        0     2126 2023-04-11 04:00:57.045113 runzero_sdk-0.2.0/runzero/types/_wrapped.py
--rw-r--r--   0        0        0      762 2023-04-11 04:00:57.045113 runzero_sdk-0.2.0/runzero/types/errors.py
--rw-r--r--   0        0        0       64 2023-04-11 04:00:57.045113 runzero_sdk-0.2.0/runzero/version.py
--rw-r--r--   0        0        0     7639 1970-01-01 00:00:00.000000 runzero_sdk-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      193 2023-04-26 01:02:34.446004 runzero_sdk-0.3.0/LICENSE
+-rw-r--r--   0        0        0     6504 2023-04-26 01:02:34.446004 runzero_sdk-0.3.0/README.md
+-rw-r--r--   0        0        0     4748 2023-04-26 01:02:34.450004 runzero_sdk-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      541 2023-04-26 01:02:34.450004 runzero_sdk-0.3.0/runzero/__init__.py
+-rw-r--r--   0        0        0      636 2023-04-26 01:02:34.450004 runzero_sdk-0.3.0/runzero/api/__init__.py
+-rw-r--r--   0        0        0      432 2023-04-26 01:02:34.450004 runzero_sdk-0.3.0/runzero/api/admin/__init__.py
+-rw-r--r--   0        0        0    11425 2023-04-26 01:02:34.450004 runzero_sdk-0.3.0/runzero/api/admin/_sdk_source_icon.py
+-rw-r--r--   0        0        0     5730 2023-04-26 01:02:34.450004 runzero_sdk-0.3.0/runzero/api/admin/custom_integrations.py
+-rw-r--r--   0        0        0     3423 2023-04-26 01:02:34.450004 runzero_sdk-0.3.0/runzero/api/admin/orgs.py
+-rw-r--r--   0        0        0     5651 2023-04-26 01:02:34.450004 runzero_sdk-0.3.0/runzero/api/admin/tasks.py
+-rw-r--r--   0        0        0     2769 2023-04-26 01:02:34.450004 runzero_sdk-0.3.0/runzero/api/custom_integrations.py
+-rw-r--r--   0        0        0     5059 2023-04-26 01:02:34.450004 runzero_sdk-0.3.0/runzero/api/explorers.py
+-rw-r--r--   0        0        0     2924 2023-04-26 01:02:34.450004 runzero_sdk-0.3.0/runzero/api/hosted_zones.py
+-rw-r--r--   0        0        0      274 2023-04-26 01:02:34.450004 runzero_sdk-0.3.0/runzero/api/imports/__init__.py
+-rw-r--r--   0        0        0     4950 2023-04-26 01:02:34.450004 runzero_sdk-0.3.0/runzero/api/imports/assets.py
+-rw-r--r--   0        0        0     1393 2023-04-26 01:02:34.450004 runzero_sdk-0.3.0/runzero/api/scans.py
+-rw-r--r--   0        0        0     4500 2023-04-26 01:02:34.450004 runzero_sdk-0.3.0/runzero/api/sites.py
+-rw-r--r--   0        0        0     4059 2023-04-26 01:02:34.450004 runzero_sdk-0.3.0/runzero/api/tasks.py
+-rw-r--r--   0        0        0      441 2023-04-26 01:02:34.450004 runzero_sdk-0.3.0/runzero/client/__init__.py
+-rw-r--r--   0        0        0      318 2023-04-26 01:02:34.450004 runzero_sdk-0.3.0/runzero/client/_http/__init__.py
+-rw-r--r--   0        0        0     2496 2023-04-26 01:02:34.450004 runzero_sdk-0.3.0/runzero/client/_http/auth.py
+-rw-r--r--   0        0        0     8120 2023-04-26 01:02:34.450004 runzero_sdk-0.3.0/runzero/client/_http/io.py
+-rw-r--r--   0        0        0    11384 2023-04-26 01:02:34.450004 runzero_sdk-0.3.0/runzero/client/client.py
+-rw-r--r--   0        0        0     7081 2023-04-26 01:02:34.450004 runzero_sdk-0.3.0/runzero/client/errors.py
+-rw-r--r--   0        0        0     1077 2023-04-26 01:02:34.450004 runzero_sdk-0.3.0/runzero/errors.py
+-rw-r--r--   0        0        0        0 2023-04-26 01:02:34.450004 runzero_sdk-0.3.0/runzero/py.typed
+-rw-r--r--   0        0        0     1687 2023-04-26 01:02:34.450004 runzero_sdk-0.3.0/runzero/types/__init__.py
+-rw-r--r--   0        0        0    36416 2023-04-26 01:02:34.450004 runzero_sdk-0.3.0/runzero/types/_data_models_gen.py
+-rw-r--r--   0        0        0     2319 2023-04-26 01:02:34.450004 runzero_sdk-0.3.0/runzero/types/_rate_limit_information.py
+-rw-r--r--   0        0        0     3410 2023-04-26 01:02:34.450004 runzero_sdk-0.3.0/runzero/types/_wrapped.py
+-rw-r--r--   0        0        0      762 2023-04-26 01:02:34.450004 runzero_sdk-0.3.0/runzero/types/errors.py
+-rw-r--r--   0        0        0      256 2023-04-26 01:02:34.450004 runzero_sdk-0.3.0/runzero/version.py
+-rw-r--r--   0        0        0     7748 1970-01-01 00:00:00.000000 runzero_sdk-0.3.0/PKG-INFO
```

### Comparing `runzero_sdk-0.2.0/README.md` & `runzero_sdk-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # runZero Python SDK
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/runzero-sdk)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/runzero-sdk)](https://pypi.org/project/runzero-sdk/)
 [![PyPI](https://img.shields.io/pypi/v/runzero-sdk)](https://pypi.org/project/runzero-sdk/)
 [![License](https://img.shields.io/badge/License-BSD_2--Clause-lightgrey.svg)](https://opensource.org/license/bsd-2-clause/)
 
 This project is currently in beta and subject to change.
 
 
 ## Overview
@@ -19,15 +19,15 @@
 discoverable, consistent, and easy to use. We want you to concentrate on working with runZero, not HTTP.
 
 
 ## Installation
 
 This project is [published to PyPI](https://pypi.org/project/runzero-sdk/) and can be installed using your local Python package manager.
 
-```commandline
+```console
 pip install runzero-sdk
 ```
 
 ## Usage
 
 There are several examples of using the SDK for common tasks under the `/examples` directory in the repo.
```

### Comparing `runzero_sdk-0.2.0/pyproject.toml` & `runzero_sdk-0.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 [tool.poetry]
 name = "runzero-sdk"
-version = "0.2.0"
+version = "0.3.0"
 description = "The runZero platform sdk"
 license = "BSD-2-Clause"
 authors = ["runZero <support@runzero.com>"]
 readme = "README.md"
 homepage = "https://runzero.com/"
+documentation = "https://runzeroinc.github.io/runzero-sdk-py"
 repository = "https://github.com/runZeroInc/runzero-sdk-py"
 keywords = ["runzero", "api", "sdk"]
 packages = [{include = "runzero"}]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Framework :: Pydantic",
   "Framework :: Pytest",
@@ -19,14 +20,17 @@
   "Topic :: Software Development :: Libraries :: Python Modules",
   "Topic :: System :: Systems Administration",
   "Typing :: Typed",
 ]
 
 [tool.poetry.group.codegen]
 
+[tool.poetry.group.docs]
+optional = true
+
 [tool.poetry.dependencies]
 python = "^3.8"
 pydantic = "^1.10.5"
 requests = "^2.28.2"
 # no standard mechanism to pin transitive deps
 # https://github.com/python-poetry/poetry/issues/4991
 certifi = ">=2022.12"
@@ -45,15 +49,15 @@
 pytest-integration = "^0.2.3"
 mypy-extensions = "^1.0.0"
 
 [tool.poetry.group.devlocal.dependencies]
 tox = "^4.4.7"
 
 [tool.poetry.group.codegen.dependencies]
-datamodel-code-generator = { version = "^0.17.1", extras = ["http"]}
+datamodel-code-generator = { version = ">=0.17.1,<0.19.0", extras = ["http"]}
 
 [tool.tox]
 legacy_tox_ini = """
     [tox]
     isolated_build = true
     env_list =
         py38
@@ -86,14 +90,27 @@
     commands_pre =
       poetry install
     commands =
       poetry run pytest --import-mode importlib --cov --with-integration --integration-cover
 
 """
 
+
+
+
+
+[tool.poetry.group.docs.dependencies]
+sphinx = "^6.1.3"
+myst_parser = "^1.0.0"
+pandoc = "^2.3"
+sphinx-last-updated-by-git = "^0.3.4"
+sphinx-codeautolink = ">=0.14.1,<0.16.0"
+sphinx-autoapi = "^2.1.0"
+furo = "^2023.3.27"
+
 [tool.deptry]
 extend_exclude = [
   # necessary until deptry can understand
   # that if TYPE_CHECKING means dev dep
   "runzero/client/_http/io.py"
 ]
 ignore_obsolete = [
@@ -158,15 +175,15 @@
 [tool.pydantic-mypy]
 init_forbid_extra = true
 init_typed = true
 warn_required_dynamic_aliases = true
 warn_untyped_fields = true
 
 [tool.pylint]
-ignore-patterns = ["_data_models_gen.py"]
+ignore-patterns = ["_data_models_gen.py", "docs"]
 
 [tool.pylint.code_style]
 max-line-length = 120
 
 [tool.pylint.'MESSAGES CONTROL']
 extension-pkg-whitelist = "pydantic"
 disable = [
```

### Comparing `runzero_sdk-0.2.0/runzero/api/admin/_sdk_source_icon.py` & `runzero_sdk-0.3.0/runzero/api/admin/_sdk_source_icon.py`

 * *Files identical despite different names*

### Comparing `runzero_sdk-0.2.0/runzero/api/admin/custom_integrations.py` & `runzero_sdk-0.3.0/runzero/api/admin/custom_integrations.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,16 +53,16 @@
 
     def get(
         self, name: Optional[str] = None, custom_integration_id: Optional[uuid.UUID] = None
     ) -> Optional[CustomIntegration]:
         """
         Retrieves runZero custom integrations with either the matching ID or Name.
 
-        :param name: Optional, name of the organization you want the UUID for
-        :param custom_integration_id: Optional, the id of the source you want returned
+        :param name: Optional, name of the custom integration to retrieve
+        :param custom_integration_id: Optional, the id of the custom integration to retrieve
         :raises AuthError, ClientError, ServerError
             ValueError if neither custom_integration_id nor name are provided.
         :return: The matching CustomIntegration or None
         """
         if name is None and custom_integration_id is None:
             raise ValueError("must provide custom_integration_id or source name")
         if custom_integration_id is not None:
```

### Comparing `runzero_sdk-0.2.0/runzero/api/admin/orgs.py` & `runzero_sdk-0.3.0/runzero/api/admin/orgs.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
-Management of asset custom integrations.
+Management of runZero organizations.
 """
+
 import uuid
 from typing import List, Optional
 
 from runzero.client import Client
 from runzero.types import Organization, OrgOptions
 
 
@@ -36,16 +37,16 @@
             result.append(Organization.parse_obj(org))
         return result
 
     def get(self, org_id: Optional[uuid.UUID] = None, name: Optional[str] = None) -> Optional[Organization]:
         """
         Retrieves the runZero Organization with the provided name or id, if it exists in your account.
 
-        :param org_id: Optional id of the organization you want returned
-        :param name: Optional name of the organization you want returned
+        :param org_id: Optional id of the organization to retrieve
+        :param name: Optional name of the organization to retrieve
         :return: Organization if found, or None
         :raises AuthError, ClientError, ServerError
         """
         if name is None and org_id is None:
             raise ValueError("must provide org_id or organization name")
         if org_id is not None:
             res = self._client.execute("GET", f"{self._ENDPOINT}/{str(org_id)}")
@@ -56,15 +57,15 @@
                 return org
         return None
 
     def create(self, org_options: OrgOptions) -> Optional[Organization]:
         """
         Creates a new organization in your account.
 
-        :param org_options: Description of organizaiton to create
+        :param org_options: Description of organization to create
         :return Organization created or None
         :raises AuthError, ClientError, ServerError
         """
         res = self._client.execute("PUT", self._ENDPOINT, data=org_options)
         obj = res.json_obj
         data_obj = obj.get("data", "")
         if data_obj:
@@ -72,24 +73,24 @@
 
         return Organization.parse_obj(obj)
 
     def update(self, org_id: uuid.UUID, org_options: OrgOptions) -> Optional[Organization]:
         """
         Updates an organization associated with your account.
 
-        :param org_id: The ID of the Organization to patch
+        :param org_id: The ID of the organization to patch
         :param org_options: Organization's updated values
         :return Organization updated or None
         :raises AuthError, ClientError, ServerError
         """
         res = self._client.execute("PATCH", f"{self._ENDPOINT}/{str(org_id)}", data=org_options)
         return Organization.parse_obj(res.json_obj)
 
     def delete(self, org_id: uuid.UUID) -> None:
         """
         Deletes an organization with provided ID from your account.
 
         :param org_id: The ID of the organization to operate against
-        :return Organization deleted or None
+        :return None
         :raises AuthError, ClientError, ServerError
         """
         self._client.execute("DELETE", f"{self._ENDPOINT}/{org_id}")
```

### Comparing `runzero_sdk-0.2.0/runzero/api/custom_integrations.py` & `runzero_sdk-0.3.0/runzero/api/custom_integrations.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         self, org_id: uuid.UUID, name: Optional[str] = None, custom_integration_id: Optional[uuid.UUID] = None
     ) -> Optional[CustomIntegration]:
         """
         Retrieves runZero custom integrations with either the matching ID or Name.
 
         :param org_id: The ID of the organization to operate against
         :param name: Optional, name of the organization you want the UUID for
-        :param custom_integration_id: Optional, the id of the source you want returned
+        :param custom_integration_id: Optional, the id of the source to retrieve
         :raises AuthError, ClientError, ServerError
             ValueError if neither custom_integration_id nor name are provided.
         :return: The matching CustomIntegration or None
         """
         params = {"_oid": str(org_id)}
         if name is None and custom_integration_id is None:
             raise ValueError("must provide custom_integration_id or source name")
```

### Comparing `runzero_sdk-0.2.0/runzero/api/imports/assets.py` & `runzero_sdk-0.3.0/runzero/api/imports/assets.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,14 +43,23 @@
         custom_integration_id: uuid.UUID,
         assets: List[ImportAsset],
         task_info: Optional[ImportTask] = None,
     ) -> Task:
         """
         Upload your custom assets to the runZero platform.
 
+        See the ImportAsset object for a description of the data that can be imported.
+
+        Assets are merged according to the merge logic in the release of the platform. This
+        involves fields other than the custom_properties dictionary.
+
+        If the runZero asset ID is known externally, it may be specified on any single
+        ImportAsset object to override all merge rules and force that object's data onto
+        the runZero asset with that ID.
+
         :param org_id: Organization ID to import these assets into
         :param site_id: ID of the Site to import these asstes into
         :param custom_integration_id: custom integration id for the provided Import Assets
         :param assets: A collection of ImportAssets to upload
         :param task_info: Descriptive information associated with the import
             task to be created. If omitted, a task name is generated for you
 
@@ -97,16 +106,13 @@
     tmp.seek(0)
     return tmp.read()
 
 
 def _create_custom_asset_request(
     site_id: uuid.UUID, custom_integration_id: uuid.UUID, assets: Iterable[ImportAsset], import_task: ImportTask
 ) -> NewAssetImport:
-    # TODO: We are disabling validation on all fields with .construct
-    # until openapi 'bytes' type and pydantic can agree on a file-like.
-    # See FastAPI implementation of UploadFile for ref
     return NewAssetImport(
-        siteId=site_id,
-        customIntegrationId=custom_integration_id,
-        importTask=import_task,
-        assetData=_import_assets_into_gzip_jsonl(assets),
+        site_id=site_id,
+        custom_integration_id=custom_integration_id,
+        import_task=import_task,
+        asset_data=_import_assets_into_gzip_jsonl(assets),
     )
```

### Comparing `runzero_sdk-0.2.0/runzero/api/sites.py` & `runzero_sdk-0.3.0/runzero/api/sites.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Management of an Organization's sites
+Management of an organization's sites.
 """
 
 import uuid
 from typing import List, Optional
 
 from runzero.client import Client
 from runzero.types import Site, SiteOptions
@@ -27,19 +27,19 @@
 
     def __init__(self, client: Client):
         """Constructor method"""
         self._client = client
 
     def get_all(self, org_id: uuid.UUID) -> List[Site]:
         """
-        Retrieves all runZero Sites available within the given Organization
+        Retrieves all runZero Sites available within the given organization
 
         :param org_id: The ID of the organization to operate against
 
-        :return: a list of all Sites available within the given Organization
+        :return: a list of all Sites available within the given organization
         :raises AuthError, ClientError, ServerError
 
         """
         params = {"_oid": str(org_id)}
         res = self._client.execute("GET", self._ENDPOINT, params=params)
         result: List[Site] = []
         for site in res.json_obj:
@@ -47,47 +47,47 @@
         return result
 
     def get(self, org_id: uuid.UUID, name: Optional[str] = None, site_id: Optional[uuid.UUID] = None) -> Optional[Site]:
         """
         Retrieves the runZero Site with the provided name or id, if it exists in your account
 
         :param org_id: The ID of the organization to operate against
+        :param name: Optional name of the site to retrieve. If not provided, must provide site_id.
+        :param site_id: Optional id of the site to retrieve. If not provided, must provide name.
 
-        :param name: Optional name of the site you want returned
-        :param site_id: the id of the site you want returned
         :return: site requested or None
         :raises AuthError, ClientError, ServerError,
             ValueError if neither site_id nor name are provided.
         """
         params = {"_oid": str(org_id)}
         if name is None and site_id is None:
             raise ValueError("must provide site_id or site name")
         if site_id is not None:
             res = self._client.execute("GET", f"{self._ENDPOINT}/{str(site_id)}", params=params)
             if not res:
                 return None
-            obj = res.json_obj
-            data_obj = obj.get("data", "")
+            site_obj = res.json_obj
+            data_obj = site_obj.get("data", "")
             if data_obj:
-                obj = data_obj
+                site_obj = data_obj
 
-            return Site.parse_obj(obj)
+            return Site.parse_obj(site_obj)
         # name
         for site in self.get_all(org_id):
             if site.name == name:
                 return site
         return None
 
     def create(self, org_id: uuid.UUID, site_options: SiteOptions) -> Optional[Site]:
         """
         Creates a new site in the given org.
 
         :param org_id: The ID of the organization to operate against
-
         :param site_options: Description of site to create
+
         :return Site created or None
         :raises AuthError, ClientError, ServerError
         """
         params = {"_oid": str(org_id)}
         res = self._client.execute("PUT", self._ENDPOINT, params=params, data=site_options)
         site_data = res.json_obj.get("data", "")
         if site_data:
@@ -95,17 +95,17 @@
         return Site.parse_obj(res.json_obj)
 
     def update(self, org_id: uuid.UUID, site_id: uuid.UUID, site_options: SiteOptions) -> Optional[Site]:
         """
         Updates a site associated with your organization.
 
         :param org_id: The ID of the organization to operate against
-
         :param site_id: The ID of the site to update.
         :param site_options: Site's updated values
+
         :return Site updated or None
         :raises AuthError, ClientError, ServerError
         """
         params = {"_oid": str(org_id)}
         res = self._client.execute("PATCH", f"{self._ENDPOINT}/{str(site_id)}", params=params, data=site_options)
         site_data = res.json_obj.get("data", "")
         if site_data:
@@ -113,14 +113,14 @@
         return Site.parse_obj(res.json_obj)
 
     def delete(self, org_id: uuid.UUID, site_id: uuid.UUID) -> None:
         """
         Deletes a site from your account.
 
         :param org_id: The ID of the organization to operate against
-
         :param site_id: Custom asset site id to delete
+
         :return None
         :raises AuthError, ClientError, ServerError
         """
         params = {"_oid": str(org_id)}
         self._client.execute("DELETE", f"{self._ENDPOINT}/{site_id}", params=params)
```

### Comparing `runzero_sdk-0.2.0/runzero/api/tasks.py` & `runzero_sdk-0.3.0/runzero/api/tasks.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Management of runZero tasks.
 """
 import uuid
 from typing import List, Optional
 
 from runzero.client import Client
-from runzero.types import Task
+from runzero.types import Task, TaskOptions
 
 
 class Tasks:
     """Management of runZero tasks.
 
     :param client: A handle to the :class:`runzero.Client` client which manages interactions
         with the runZero server.
@@ -17,43 +17,47 @@
 
     _ENDPOINT = "api/v1.0/org/tasks"
 
     def __init__(self, client: Client):
         """Constructor method"""
         self._client = client
 
-    def get_all(self, org_id: uuid.UUID, status: Optional[str] = None) -> List[Task]:
+    def get_all(self, org_id: uuid.UUID, status: Optional[str] = None, query: Optional[str] = None) -> List[Task]:
         """
         Retrieves all runZero Tasks available within the given Organization
 
         :param org_id: The unique ID of the organization to retrieve the tasks from.
         :param status: An optional status value to filter tasks by. This is a
             case-insensitive string match, stripped of surrounding whitespace.
+        :param query: An optional query to filter returned tasks.
+            Query string format is the same as in-UI search. See https://www.runzero.com/docs/search-query-tasks/
         :return: A list of all tasks
         """
         params = {"_oid": str(org_id)}
+        if query is not None:
+            params["search"] = query.strip()
+        if status is not None:
+            params["status"] = status.strip()
         res = self._client.execute("GET", self._ENDPOINT, params=params)
         result: List[Task] = []
         for obj in res.json_obj:
             task = Task.parse_obj(obj)
-            if status is not None and task.status is not None and task.status.strip().lower() != status.strip().lower():
-                continue
             result.append(task)
         return result
 
     def get(self, org_id: uuid.UUID, name: Optional[str] = None, task_id: Optional[uuid.UUID] = None) -> Optional[Task]:
         """
         Retrieves the runZero Task with the provided name or id, if it exists in your organization.
 
-        One of either name or id must be provided.
-
         :param org_id: ID of the organization the requested Task is in
-        :param name: Optional name of the task you want returned
-        :param task_id: Optional id of the task you want returned
-        :return: Task or None
+        :param name: Optional name of the task to retrieve. If not provided, must provide task_id.
+        :param task_id: Optional id of the task to retrieve. If not provided, must provide name.
+
+        :raises AuthError, ClientError, ServerError
+            ValueError if neither task_id nor name are provided.
         """
         params = {"_oid": str(org_id)}
         if name is None and task_id is None:
             raise ValueError("must provide either task_id or task name")
         if task_id is not None:
             res = self._client.execute("GET", f"{self._ENDPOINT}/{str(task_id)}", params=params)
             return Task.parse_obj(res.json_obj)
@@ -65,18 +69,31 @@
 
     def get_status(self, org_id: uuid.UUID, task_id: uuid.UUID) -> Optional[str]:
         """
         Retrieves the status of a runZero Task with the provided id, if it exists in your organization.
 
         The org_id should be provided if using an Account level api key.
 
-        :param task_id: ID of the Task you want the status for
-        :param org_id: Optional id of the organization the requested Task is in. This is
+        :param task_id: ID of the task you want the status for
+        :param org_id: ID of the organization the requested Task is in. This is
             necessary if you use an Auth token.
         :return: a string result indicating task status, or None
         """
         params = {"_oid": str(org_id)}
         res = self._client.execute("GET", f"{self._ENDPOINT}/{str(task_id)}", params=params)
         task = Task.parse_obj(res.json_obj)
         if task is None:
             return None
         return task.status
+
+    def update(self, org_id: uuid.UUID, task_id: uuid.UUID, task_options: TaskOptions) -> Task:
+        """
+        Updates task parameters with provided task options values.
+
+        :param task_id: task to modify
+        :param task_options: task values to update
+        :return Task which has been updated
+        :raises AuthError, ClientError, ServerError
+        """
+        params = {"_oid": str(org_id)}
+        res = self._client.execute("PATCH", f"{self._ENDPOINT}/{str(task_id)}", data=task_options, params=params)
+        return Task.parse_obj(res.json_obj)
```

### Comparing `runzero_sdk-0.2.0/runzero/client/_http/auth.py` & `runzero_sdk-0.3.0/runzero/client/_http/auth.py`

 * *Files identical despite different names*

### Comparing `runzero_sdk-0.2.0/runzero/client/_http/io.py` & `runzero_sdk-0.3.0/runzero/client/_http/io.py`

 * *Files 4% similar despite different names*

```diff
@@ -143,40 +143,14 @@
             raise ConnTimeoutError from exc
         except (RequestsConnectionError, ConnectionRefusedError) as exc:
             raise ConnError from exc
         except (RequestsHTTPError, ContentDecodingError) as exc:
             raise CommunicationError from exc
 
 
-def _generate_prepared_request(
-    method: str,
-    url: str,
-    headers: Dict[str, Any],
-    auth: BearerToken,
-    data: Any,
-    params: Dict[str, Any],
-    handlers: List[HandlerType],
-) -> PreparedRequest:
-    request = RequestsRequest(
-        method=method,
-        url=url,
-        headers=headers,
-        auth=auth,
-        data=data,
-        params=params,
-    )
-
-    handlers.append(_error_handler)
-
-    for handler in handlers:
-        request.register_hook("response", handler)
-
-    return request.prepare()
-
-
 def _error_handler(response: RequestsResponse, **kwargs: Any) -> RequestsResponse:
     # pylint: disable=unused-argument
     if not 400 <= response.status_code <= 599:
         return response
 
     try:
         body = response.json()
@@ -212,31 +186,32 @@
             content_type = response.headers.get("Content-Type", "")
         if content_type.startswith("application/json") or content_type.startswith("application/problem+json"):
             body = response.json().copy()
             # {"detail":"customIntegrationId UUID cannot be all zeroes","error":"request failed","status":"error",
             # "title":"request failed"}
             try:
                 error_info = ErrInfo(
-                    detail=body.pop("detail"),
-                    status=response.status_code,
                     title=body.pop("title"),
+                    status=response.status_code,
+                    detail=body.pop("detail", None),
                 )
             except KeyError:
                 pass
+
     except (KeyError, JSONDecodeError) as exc:
         raise UnknownAPIError(str(response), response.reason) from exc
 
     if 400 <= response.status_code <= 499:
         if response.status_code == 429:
             rate_limit = RateLimitInformation.from_headers(response.headers)
             remaining = rate_limit.usage_remaining
             if isinstance(remaining, int) and remaining < 1:
                 raise RateLimitError(rate_limit_information=rate_limit)
         raise ClientError(
-            unparsed_response=str(response),
+            unparsed_response=response.json(),
             message=f"The request was rejected by the server: {error_message}",
             error_info=error_info,
         )
 
     if 500 <= response.status_code <= 599:
         raise ServerError(
             unparsed_response=str(response),
```

### Comparing `runzero_sdk-0.2.0/runzero/client/client.py` & `runzero_sdk-0.3.0/runzero/client/client.py`

 * *Files identical despite different names*

### Comparing `runzero_sdk-0.2.0/runzero/client/errors.py` & `runzero_sdk-0.3.0/runzero/client/errors.py`

 * *Files 10% similar despite different names*

```diff
@@ -47,20 +47,29 @@
     def __init__(
         self,
         message: Optional[str] = None,
         unparsed_response: Optional[str] = None,
         error_info: Optional[ErrInfo] = None,
     ):
         """Constructor method"""
+        if message:
+            message = message.strip()
         if not message:
             message = "The request was rejected by the server."
         super().__init__(message)
         self.error_info: Optional[ErrInfo] = error_info
         self.unparsed_response: Optional[str] = unparsed_response
 
+    def __str__(self) -> str:
+        """Provide a friendly, printable error string. Otherwise, only 'message' is printed."""
+        out = f"{super().__str__()}".strip()
+        if self.error_info:
+            out = f"{out}: {self.error_info}"
+        return out
+
 
 class ServerError(APIError):
     """
     ServerError is a named Exception class for holding 500 level http status code messages.
 
     A ServerError indicates nothing about the way the request was performed. The server cannot
     complete the task. You should retry or abort.
@@ -79,20 +88,29 @@
     def __init__(
         self,
         message: Optional[str] = None,
         unparsed_response: Optional[str] = None,
         error_info: Optional[ErrInfo] = None,
     ):
         """Constructor method"""
+        if message:
+            message = message.strip()
         if not message:
             message = "The server encounter an error or is unable to process the request."
         super().__init__(message)
         self.error_info: Optional[ErrInfo] = error_info
         self.unparsed_response: Optional[str] = unparsed_response
 
+    def __str__(self) -> str:
+        """Provide a friendly, printable error string. Otherwise, only 'message' is printed."""
+        out = f"{super().__str__()}"
+        if self.error_info:
+            out = f"{out}: {self.error_info}"
+        return out
+
 
 class AuthError(APIError):
     """
     AuthError is a named Exception class for authentication issues with the runZero SDK client
 
     Common types of authentication issues are:
     * Incorrect credentials
```

### Comparing `runzero_sdk-0.2.0/runzero/errors.py` & `runzero_sdk-0.3.0/runzero/errors.py`

 * *Files identical despite different names*

### Comparing `runzero_sdk-0.2.0/runzero/types/__init__.py` & `runzero_sdk-0.3.0/runzero/types/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,47 +4,66 @@
 
 Public, SDK-supported runZero API types contained inside this package are made
 available here. Not all objects in the private module, which is generated from
 OpenAPI specs, are usable in this project today.
 """
 from ipaddress import IPv4Address, IPv6Address
 
+from runzero.types._data_models_gen import Agent as Explorer
+from runzero.types._data_models_gen import AgentSiteID as ExplorerSiteID
 from runzero.types._data_models_gen import (
     BaseCustomIntegration,
+    HostedZone,
     ImportAsset,
     ImportTask,
     NetworkInterface,
     NewAssetImport,
     NewCustomIntegration,
     Organization,
     OrgOptions,
     Problem,
     Site,
     SiteOptions,
     Task,
+    TaskOptions,
 )
 from runzero.types._rate_limit_information import RateLimitInformation
-from runzero.types._wrapped import CustomAttribute, CustomIntegration, Hostname, Tag
+from runzero.types._wrapped import (
+    CustomAttribute,
+    CustomIntegration,
+    Hostname,
+    ScanOptions,
+    ScanTemplate,
+    ScanTemplateOptions,
+    Tag,
+)
 from runzero.types.errors import ValidationError
 
 __all__ = [
     "CustomIntegration",
     "BaseCustomIntegration",
     "CustomAttribute",
+    "Explorer",
+    "ExplorerSiteID",
+    "HostedZone",
     "Hostname",
     "IPv4Address",
     "IPv6Address",
     "ImportAsset",
     "ImportTask",
     "NetworkInterface",
     "NewCustomIntegration",
     "NewAssetImport",
     "Organization",
     "OrgOptions",
     "Problem",
     "RateLimitInformation",
+    "ScanOptions",
+    "ScanTemplate",
+    "ScanTemplateOptions",
     "Site",
     "SiteOptions",
     "Tag",
     "Task",
+    "TaskOptions",
     "ValidationError",
 ]
```

### Comparing `runzero_sdk-0.2.0/runzero/types/_rate_limit_information.py` & `runzero_sdk-0.3.0/runzero/types/_rate_limit_information.py`

 * *Files identical despite different names*

### Comparing `runzero_sdk-0.2.0/runzero/types/errors.py` & `runzero_sdk-0.3.0/runzero/types/errors.py`

 * *Files identical despite different names*

### Comparing `runzero_sdk-0.2.0/PKG-INFO` & `runzero_sdk-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runzero-sdk
-Version: 0.2.0
+Version: 0.3.0
 Summary: The runZero platform sdk
 Home-page: https://runzero.com/
 License: BSD-2-Clause
 Keywords: runzero,api,sdk
 Author: runZero
 Author-email: support@runzero.com
 Requires-Python: >=3.8,<4.0
@@ -22,19 +22,20 @@
 Classifier: Topic :: Security
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Systems Administration
 Classifier: Typing :: Typed
 Requires-Dist: certifi (>=2022.12)
 Requires-Dist: pydantic (>=1.10.5,<2.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
+Project-URL: Documentation, https://runzeroinc.github.io/runzero-sdk-py
 Project-URL: Repository, https://github.com/runZeroInc/runzero-sdk-py
 Description-Content-Type: text/markdown
 
 # runZero Python SDK
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/runzero-sdk)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/runzero-sdk)](https://pypi.org/project/runzero-sdk/)
 [![PyPI](https://img.shields.io/pypi/v/runzero-sdk)](https://pypi.org/project/runzero-sdk/)
 [![License](https://img.shields.io/badge/License-BSD_2--Clause-lightgrey.svg)](https://opensource.org/license/bsd-2-clause/)
 
 This project is currently in beta and subject to change.
 
 
 ## Overview
@@ -50,15 +51,15 @@
 discoverable, consistent, and easy to use. We want you to concentrate on working with runZero, not HTTP.
 
 
 ## Installation
 
 This project is [published to PyPI](https://pypi.org/project/runzero-sdk/) and can be installed using your local Python package manager.
 
-```commandline
+```console
 pip install runzero-sdk
 ```
 
 ## Usage
 
 There are several examples of using the SDK for common tasks under the `/examples` directory in the repo.
```

