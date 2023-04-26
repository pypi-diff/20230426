# Comparing `tmp/prefect-azure-0.2.6.tar.gz` & `tmp/prefect-azure-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/prefect-azure/prefect-azure/dist/.tmp-00ntg7f3/prefect-azure-0.2.6.tar", last modified: Fri Apr 21 00:06:36 2023, max compression
+gzip compressed data, was "/home/runner/work/prefect-azure/prefect-azure/dist/.tmp-xafqlomh/prefect-azure-0.2.7.tar", last modified: Tue Apr 25 20:23:42 2023, max compression
```

## Comparing `prefect-azure-0.2.6.tar` & `prefect-azure-0.2.7.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:06:36.000000 prefect-azure-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-04-21 00:04:40.000000 prefect-azure-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-21 00:04:40.000000 prefect-azure-0.2.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8043 2023-04-21 00:06:36.000000 prefect-azure-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7027 2023-04-21 00:04:40.000000 prefect-azure-0.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:06:36.000000 prefect-azure-0.2.6/prefect_azure/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-21 00:04:40.000000 prefect-azure-0.2.6/prefect_azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-21 00:06:36.000000 prefect-azure-0.2.6/prefect_azure/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6183 2023-04-21 00:04:40.000000 prefect-azure-0.2.6/prefect_azure/blob_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)    32501 2023-04-21 00:04:40.000000 prefect-azure-0.2.6/prefect_azure/container_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     7920 2023-04-21 00:04:40.000000 prefect-azure-0.2.6/prefect_azure/cosmos_db.py
--rw-r--r--   0 runner    (1001) docker     (123)    20976 2023-04-21 00:04:40.000000 prefect-azure-0.2.6/prefect_azure/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     9879 2023-04-21 00:04:40.000000 prefect-azure-0.2.6/prefect_azure/ml_datastore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:06:36.000000 prefect-azure-0.2.6/prefect_azure/workers/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-21 00:04:40.000000 prefect-azure-0.2.6/prefect_azure/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37219 2023-04-21 00:04:40.000000 prefect-azure-0.2.6/prefect_azure/workers/container_instance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:06:36.000000 prefect-azure-0.2.6/prefect_azure.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8043 2023-04-21 00:06:36.000000 prefect-azure-0.2.6/prefect_azure.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-21 00:06:36.000000 prefect-azure-0.2.6/prefect_azure.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 00:06:36.000000 prefect-azure-0.2.6/prefect_azure.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-21 00:06:36.000000 prefect-azure-0.2.6/prefect_azure.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-21 00:06:36.000000 prefect-azure-0.2.6/prefect_azure.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-21 00:06:36.000000 prefect-azure-0.2.6/prefect_azure.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-21 00:04:40.000000 prefect-azure-0.2.6/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-21 00:04:40.000000 prefect-azure-0.2.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-21 00:06:36.000000 prefect-azure-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-04-21 00:04:40.000000 prefect-azure-0.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:06:36.000000 prefect-azure-0.2.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    31854 2023-04-21 00:04:40.000000 prefect-azure-0.2.6/tests/test_aci_infrastructure.py
--rw-r--r--   0 runner    (1001) docker     (123)    37149 2023-04-21 00:04:40.000000 prefect-azure-0.2.6/tests/test_aci_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-04-21 00:04:40.000000 prefect-azure-0.2.6/tests/test_blob_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-21 00:04:40.000000 prefect-azure-0.2.6/tests/test_block_standards.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-04-21 00:04:40.000000 prefect-azure-0.2.6/tests/test_cosmos_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-04-21 00:04:40.000000 prefect-azure-0.2.6/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-04-21 00:04:40.000000 prefect-azure-0.2.6/tests/test_ml_datastore.py
--rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-04-21 00:04:40.000000 prefect-azure-0.2.6/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 20:23:42.000000 prefect-azure-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-04-25 20:21:59.000000 prefect-azure-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-25 20:21:59.000000 prefect-azure-0.2.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8043 2023-04-25 20:23:42.000000 prefect-azure-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7027 2023-04-25 20:21:59.000000 prefect-azure-0.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 20:23:42.000000 prefect-azure-0.2.7/prefect_azure/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-25 20:21:59.000000 prefect-azure-0.2.7/prefect_azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-25 20:23:42.000000 prefect-azure-0.2.7/prefect_azure/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6183 2023-04-25 20:21:59.000000 prefect-azure-0.2.7/prefect_azure/blob_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32501 2023-04-25 20:21:59.000000 prefect-azure-0.2.7/prefect_azure/container_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7920 2023-04-25 20:21:59.000000 prefect-azure-0.2.7/prefect_azure/cosmos_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20976 2023-04-25 20:21:59.000000 prefect-azure-0.2.7/prefect_azure/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9879 2023-04-25 20:21:59.000000 prefect-azure-0.2.7/prefect_azure/ml_datastore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 20:23:42.000000 prefect-azure-0.2.7/prefect_azure/workers/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-25 20:21:59.000000 prefect-azure-0.2.7/prefect_azure/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37699 2023-04-25 20:21:59.000000 prefect-azure-0.2.7/prefect_azure/workers/container_instance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 20:23:42.000000 prefect-azure-0.2.7/prefect_azure.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8043 2023-04-25 20:23:42.000000 prefect-azure-0.2.7/prefect_azure.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-25 20:23:42.000000 prefect-azure-0.2.7/prefect_azure.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 20:23:42.000000 prefect-azure-0.2.7/prefect_azure.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-25 20:23:42.000000 prefect-azure-0.2.7/prefect_azure.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-25 20:23:42.000000 prefect-azure-0.2.7/prefect_azure.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-25 20:23:42.000000 prefect-azure-0.2.7/prefect_azure.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-25 20:21:59.000000 prefect-azure-0.2.7/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-25 20:21:59.000000 prefect-azure-0.2.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-25 20:23:42.000000 prefect-azure-0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-04-25 20:21:59.000000 prefect-azure-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 20:23:42.000000 prefect-azure-0.2.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    31854 2023-04-25 20:21:59.000000 prefect-azure-0.2.7/tests/test_aci_infrastructure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37898 2023-04-25 20:21:59.000000 prefect-azure-0.2.7/tests/test_aci_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-04-25 20:21:59.000000 prefect-azure-0.2.7/tests/test_blob_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-25 20:21:59.000000 prefect-azure-0.2.7/tests/test_block_standards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-04-25 20:21:59.000000 prefect-azure-0.2.7/tests/test_cosmos_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-04-25 20:21:59.000000 prefect-azure-0.2.7/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-04-25 20:21:59.000000 prefect-azure-0.2.7/tests/test_ml_datastore.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-04-25 20:21:59.000000 prefect-azure-0.2.7/versioneer.py
```

### Comparing `prefect-azure-0.2.6/LICENSE` & `prefect-azure-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `prefect-azure-0.2.6/PKG-INFO` & `prefect-azure-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-azure
-Version: 0.2.6
+Version: 0.2.7
 Summary: Prefect tasks and subflows for interacting with Azure
 Home-page: https://github.com/PrefectHQ/prefect-azure
 Author: Prefect Technologies, Inc.
 Author-email: help@prefect.io
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
```

### Comparing `prefect-azure-0.2.6/README.md` & `prefect-azure-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `prefect-azure-0.2.6/prefect_azure/__init__.py` & `prefect-azure-0.2.7/prefect_azure/__init__.py`

 * *Files identical despite different names*

### Comparing `prefect-azure-0.2.6/prefect_azure/blob_storage.py` & `prefect-azure-0.2.7/prefect_azure/blob_storage.py`

 * *Files identical despite different names*

### Comparing `prefect-azure-0.2.6/prefect_azure/container_instance.py` & `prefect-azure-0.2.7/prefect_azure/container_instance.py`

 * *Files identical despite different names*

### Comparing `prefect-azure-0.2.6/prefect_azure/cosmos_db.py` & `prefect-azure-0.2.7/prefect_azure/cosmos_db.py`

 * *Files identical despite different names*

### Comparing `prefect-azure-0.2.6/prefect_azure/credentials.py` & `prefect-azure-0.2.7/prefect_azure/credentials.py`

 * *Files identical despite different names*

### Comparing `prefect-azure-0.2.6/prefect_azure/ml_datastore.py` & `prefect-azure-0.2.7/prefect_azure/ml_datastore.py`

 * *Files identical despite different names*

### Comparing `prefect-azure-0.2.6/prefect_azure/workers/container_instance.py` & `prefect-azure-0.2.7/prefect_azure/workers/container_instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 !!! example "Using a custom ARM template"
     To facilitate easy customization, the Azure Container worker provisions a
     containing group using an ARM template. The default ARM template is represented
     in YAML as follows:
     ```yaml
     ---
     arm_template:
-      "$schema": https://schema.management.azure.com/schemas/2022-09-01/deploymentTemplate.json#
+      "$schema": https://schema.management.azure.com/schemas/2019-08-01/deploymentTemplate.json#
       contentVersion: 1.0.0.0
       parameters:
         location:
           type: string
           defaultValue: "[resourceGroup().location]"
           metadata:
             description: Location for all resources.
@@ -127,15 +127,15 @@
 # check their Azure account for orphaned container groups.
 CONTAINER_GROUP_DELETION_TIMEOUT_SECONDS = 30
 
 
 def _get_default_arm_template():
     """Get the default ARM template for creating a container group."""
     return {
-        "$schema": "https://schema.management.azure.com/schemas/2022-09-01/deploymentTemplate.json#",  # noqa
+        "$schema": "https://schema.management.azure.com/schemas/2019-08-01/deploymentTemplate.json#",  # noqa
         "contentVersion": "1.0.0.0",
         "parameters": {
             "location": {
                 "type": "string",
                 "defaultValue": "[resourceGroup().location]",
                 "metadata": {"description": "Location for all resources."},
             },
@@ -151,15 +151,15 @@
                 "defaultValue": "[uniqueString(resourceGroup().id)]",
                 "metadata": {"description": "The name of the container to create."},
             },
         },
         "resources": [
             {
                 "type": "Microsoft.ContainerInstance/containerGroups",
-                "apiVersion": "2021-09-01",
+                "apiVersion": "2022-09-01",
                 "name": "[parameters('container_group_name')]",
                 "location": "[parameters('location')]",
                 "properties": {
                     "containers": [
                         {
                             "name": "[parameters('container_name')]",
                             "properties": {
@@ -203,25 +203,25 @@
 
 
 class AzureContainerJobConfiguration(BaseJobConfiguration):
     """
     Configuration for an Azure Container Instance flow run.
     """
 
-    image: Optional[str] = Field(default_factory=get_prefect_image_name)
+    image: str = Field(default_factory=get_prefect_image_name)
     resource_group_name: str = Field(default=...)
     subscription_id: SecretStr = Field(default=...)
     identities: Optional[List[str]] = Field(default=None)
     entrypoint: Optional[str] = Field(default=DEFAULT_CONTAINER_ENTRYPOINT)
     image_registry: Optional[
         Union[
             prefect.infrastructure.docker.DockerRegistry,
             ACRManagedIdentity,
         ]
-    ]
+    ] = Field(default=None)
     cpu: float = Field(default=ACI_DEFAULT_CPU)
     gpu_count: Optional[int] = Field(default=None)
     gpu_sku: Optional[str] = Field(default=None)
     memory: float = Field(default=ACI_DEFAULT_MEMORY)
     subnet_ids: Optional[List[str]] = Field(default=None)
     dns_servers: Optional[List[str]] = Field(default=None)
     stream_output: bool = Field(default=False)
@@ -255,14 +255,16 @@
         # set the container's environment variables
         container["properties"]["environmentVariables"] = self._get_arm_environment()
 
         # convert the command from a string to a list, because that's what ACI expects
         if self.command:
             container["properties"]["command"] = self.command.split(" ")
 
+        self._add_image()
+
         # Add the entrypoint if provided. Creating an ACI container with a
         # command overrides the container's built-in entrypoint. Prefect base images
         # use entrypoint.sh as the entrypoint, so we need to add to the beginning of
         # the command list to avoid breaking EXTRA_PIP_PACKAGES installation on
         # container startup.
         if self.entrypoint:
             container["properties"]["command"].insert(0, self.entrypoint)
@@ -275,14 +277,25 @@
 
         if self.subnet_ids:
             self._add_subnets(self.subnet_ids)
 
         if self.dns_servers:
             self._add_dns_servers(self.dns_servers)
 
+    def _add_image(self):
+        """
+        Add the image to the arm template.
+        """
+        try:
+            self.arm_template["resources"][0]["properties"]["containers"][0][
+                "properties"
+            ]["image"] = self.image
+        except KeyError:
+            raise ValueError("Unable to add image due to invalid job ARM template.")
+
     def _add_image_registry_credentials(
         self,
         image_registry: Union[
             prefect.infrastructure.docker.DockerRegistry,
             ACRManagedIdentity,
             None,
         ],
@@ -374,14 +387,15 @@
 
 class AzureContainerVariables(BaseVariables):
     """
     Variables for an Azure Container Instance flow run.
     """
 
     image: Optional[str] = Field(
+        default=None,
         description=(
             "The image to use for the Prefect container in the task. This value "
             "defaults to a Prefect base image matching your local versions."
         ),
     )
     resource_group_name: str = Field(
         default=...,
@@ -458,14 +472,15 @@
             "The amount of memory in gigabytes to provide to the ACI task. Valid "
             "amounts are specified in the Azure documentation. If not provided, a "
             f"default value of  {ACI_DEFAULT_MEMORY} will be used unless present "
             "on the task definition."
         ),
     )
     aci_credentials: AzureContainerInstanceCredentials = Field(
+        default_factory=AzureContainerInstanceCredentials,
         description=("The credentials to use to authenticate with Azure."),
     )
     stream_output: bool = Field(
         default=False,
         description=(
             "If `True`, logs will be streamed from the Prefect container to the local "
             "console."
```

### Comparing `prefect-azure-0.2.6/prefect_azure.egg-info/PKG-INFO` & `prefect-azure-0.2.7/prefect_azure.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-azure
-Version: 0.2.6
+Version: 0.2.7
 Summary: Prefect tasks and subflows for interacting with Azure
 Home-page: https://github.com/PrefectHQ/prefect-azure
 Author: Prefect Technologies, Inc.
 Author-email: help@prefect.io
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
```

### Comparing `prefect-azure-0.2.6/prefect_azure.egg-info/SOURCES.txt` & `prefect-azure-0.2.7/prefect_azure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prefect-azure-0.2.6/setup.cfg` & `prefect-azure-0.2.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `prefect-azure-0.2.6/setup.py` & `prefect-azure-0.2.7/setup.py`

 * *Files identical despite different names*

### Comparing `prefect-azure-0.2.6/tests/test_aci_infrastructure.py` & `prefect-azure-0.2.7/tests/test_aci_infrastructure.py`

 * *Files identical despite different names*

### Comparing `prefect-azure-0.2.6/tests/test_aci_worker.py` & `prefect-azure-0.2.7/tests/test_aci_worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import dateutil.parser
 import pytest
 from anyio.abc import TaskStatus
 from azure.core.exceptions import HttpResponseError, ResourceNotFoundError
 from azure.identity import ClientSecretCredential
 from azure.mgmt.resource import ResourceManagementClient
 from prefect.client.schemas import FlowRun
+from prefect.docker import get_prefect_image_name
 from prefect.exceptions import InfrastructureNotFound
 from prefect.infrastructure.docker import DockerRegistry
 from prefect.server.schemas.core import Flow
 from prefect.settings import get_current_settings
 from prefect.testing.utilities import AsyncMock
 from pydantic import SecretStr
 
@@ -936,14 +937,33 @@
     assert config.subscription_id.get_secret_value() == "my-subscription-id"
     assert config.aci_credentials.tenant_id == "my-tenant-id"
     assert config.aci_credentials.client_id == "my-client-id"
     assert config.aci_credentials.client_secret.get_secret_value() == "my-client-secret"
     assert type(config.arm_template) == dict
 
 
+async def test_image_populated_in_template_when_not_provided(worker_flow_run):
+    config = await AzureContainerJobConfiguration.from_template_and_values(
+        base_job_template=AzureContainerWorker.get_default_base_job_template(),
+        values=AzureContainerVariables(
+            subscription_id="my-subscription-id",
+            resource_group_name="my-resource-group",
+        ).dict(exclude_unset=True),
+    )
+    config.prepare_for_flow_run(worker_flow_run)
+
+    assert config.image == get_prefect_image_name()
+    assert (
+        config.arm_template["resources"][0]["properties"]["containers"][0][
+            "properties"
+        ]["image"]
+        == get_prefect_image_name()
+    )
+
+
 async def test_add_identities(
     raw_job_configuration, worker_flow_run, mock_aci_client, monkeypatch
 ):
     raw_job_configuration.identities = ["identity1", "identity2", "identity3"]
     raw_job_configuration.prepare_for_flow_run(worker_flow_run)
 
     container_group = raw_job_configuration.arm_template["resources"][0]
```

### Comparing `prefect-azure-0.2.6/tests/test_blob_storage.py` & `prefect-azure-0.2.7/tests/test_blob_storage.py`

 * *Files identical despite different names*

### Comparing `prefect-azure-0.2.6/tests/test_block_standards.py` & `prefect-azure-0.2.7/tests/test_block_standards.py`

 * *Files identical despite different names*

### Comparing `prefect-azure-0.2.6/tests/test_cosmos_db.py` & `prefect-azure-0.2.7/tests/test_cosmos_db.py`

 * *Files identical despite different names*

### Comparing `prefect-azure-0.2.6/tests/test_credentials.py` & `prefect-azure-0.2.7/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `prefect-azure-0.2.6/tests/test_ml_datastore.py` & `prefect-azure-0.2.7/tests/test_ml_datastore.py`

 * *Files identical despite different names*

### Comparing `prefect-azure-0.2.6/versioneer.py` & `prefect-azure-0.2.7/versioneer.py`

 * *Files identical despite different names*

