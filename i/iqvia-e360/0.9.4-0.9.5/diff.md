# Comparing `tmp/iqvia_e360-0.9.4-py3-none-any.whl.zip` & `tmp/iqvia_e360-0.9.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 12223 bytes, number of entries: 10
--rw-r--r--  2.0 unx     1020 b- defN 22-Dec-16 12:46 iqvia_e360/__init__.py
--rw-r--r--  2.0 unx    16251 b- defN 22-Dec-20 13:31 iqvia_e360/e360_context.py
--rw-r--r--  2.0 unx       46 b- defN 22-Jul-26 10:49 iqvia_e360/exceptions.py
--rw-r--r--  2.0 unx     8212 b- defN 22-Aug-17 15:14 iqvia_e360/models.py
--rw-r--r--  2.0 unx     2134 b- defN 22-Jul-26 10:49 iqvia_e360/settings.py
--rw-rw-rw-  2.0 unx      575 b- defN 22-Dec-20 13:53 iqvia_e360-0.9.4.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx    14607 b- defN 22-Dec-20 13:53 iqvia_e360-0.9.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Dec-20 13:53 iqvia_e360-0.9.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 22-Dec-20 13:53 iqvia_e360-0.9.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      803 b- defN 22-Dec-20 13:53 iqvia_e360-0.9.4.dist-info/RECORD
-10 files, 43751 bytes uncompressed, 10857 bytes compressed:  75.2%
+Zip file size: 12413 bytes, number of entries: 10
+-rw-r--r--  2.0 unx     1020 b- defN 23-Apr-24 17:19 iqvia_e360/__init__.py
+-rw-r--r--  2.0 unx    16251 b- defN 23-Apr-21 12:25 iqvia_e360/e360_context.py
+-rw-r--r--  2.0 unx       46 b- defN 23-Apr-21 12:25 iqvia_e360/exceptions.py
+-rw-r--r--  2.0 unx     8212 b- defN 23-Apr-21 12:25 iqvia_e360/models.py
+-rw-r--r--  2.0 unx     2134 b- defN 23-Apr-21 12:25 iqvia_e360/settings.py
+-rw-rw-rw-  2.0 unx      575 b- defN 23-Apr-26 15:31 iqvia_e360-0.9.5.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx    15456 b- defN 23-Apr-26 15:31 iqvia_e360-0.9.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-26 15:31 iqvia_e360-0.9.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Apr-26 15:31 iqvia_e360-0.9.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      803 b- defN 23-Apr-26 15:31 iqvia_e360-0.9.5.dist-info/RECORD
+10 files, 44600 bytes uncompressed, 11047 bytes compressed:  75.2%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: iqvia_e360/models.py
 Comment: 
 
 Filename: iqvia_e360/settings.py
 Comment: 
 
-Filename: iqvia_e360-0.9.4.dist-info/LICENSE.txt
+Filename: iqvia_e360-0.9.5.dist-info/LICENSE.txt
 Comment: 
 
-Filename: iqvia_e360-0.9.4.dist-info/METADATA
+Filename: iqvia_e360-0.9.5.dist-info/METADATA
 Comment: 
 
-Filename: iqvia_e360-0.9.4.dist-info/WHEEL
+Filename: iqvia_e360-0.9.5.dist-info/WHEEL
 Comment: 
 
-Filename: iqvia_e360-0.9.4.dist-info/top_level.txt
+Filename: iqvia_e360-0.9.5.dist-info/top_level.txt
 Comment: 
 
-Filename: iqvia_e360-0.9.4.dist-info/RECORD
+Filename: iqvia_e360-0.9.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## iqvia_e360/__init__.py

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.9.4"
+__version__ = "0.9.5"
 
 __all__ = [
     "E360Context",
     "Settings",
     "AnalyticDatasetModel",
     "AnalyticDatasetDefinitionModel",
     "Granularity",
```

## Comparing `iqvia_e360-0.9.4.dist-info/LICENSE.txt` & `iqvia_e360-0.9.5.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `iqvia_e360-0.9.4.dist-info/METADATA` & `iqvia_e360-0.9.5.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iqvia-e360
-Version: 0.9.4
+Version: 0.9.5
 Summary: E360 Clients Wrapper for Python
 Author: IQVIA
 Author-email: e360pypi@iqvia.com
 License: Apache License 2.0
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -46,17 +46,16 @@
 ## Features
 * Authentication using OIDC (internal network only) and Api Gateway (internal and external network)
 * Handles the creation of E360 clients
 * Provides convenient functions for the following use-cases:
     * List ADT reports
     * Download an ADT report
     * Upload an ADT
-    * List workspace containers
-    * Create a workspace container
-    * Create a workspace asset
+    * List workspaces, folders and assets
+    * Create workspaces, folders and assets
     * Upload a document to workspaces
     * Move and rename a workspace asset
     * Create an E360 visualisation from a Plotly figure
 
 ## API Key
 
 To get started you will need to get an API token from your E360™ _Manage Account_ page. You may download a settings file, which will contains the API key and the API Gateway information needed to connect. See documentation for more details how to use the settings file.
@@ -117,16 +116,16 @@
 
 ## _class_ `iqvia_e360.E360Context(**kwargs)`
 
 The main class for retrieving E360™ microservice clients, for interacting  with E360 Workspace assets.
 
 > To facilitate initializing class instances, use of the class methods below is highly recommended.
 
-### _classmethod_ `E360Context.create_from_settings(path: pathlib.Path)`
-Create an instance from a settings file.
+### _classmethod_ `E360Context.create_from_settings(settings_path: pathlib.Path|str) -> E360Context`
+Create an E360Context instance from a settings file.
 
 The settings file can be created with the following content:
 
 ```ini
 [e360]
 api_gateway_url = https://api-gateway-url.com
 api_gateway_key = my-key
@@ -147,14 +146,17 @@
 
 Returns a list of `AdtReportAssetModel` instances.
 
 >The keyword `filters` represents an unpacked a mapping with the following values:
 >
 >- `metadata_key` (Optional): A metadata key to filter by; must be provided together with metadata_value
 >- `metadata_value` (Optional): A metadata value to filter by
+>- `embed` (Optional): A asset embed value to filter by - `parent`, `metadata` or `datasetInfo`
+>- `fields` (Optional): A list of fields to filter by
+>- `sort` (Optional): A sort field value to filter by (defaults to `-created`)
 
 Example:
 ```python
 context.get_adt_reports(metadata_key='mykey', metadata_value='myvalue')
 ```
 
 ### _method_ `.get_adt_report_by_id(id: str) -> AdtReportAssetModel`
@@ -165,20 +167,20 @@
 Returns a list of `AdtReportAssetModel` instances filtered by _name_ in the asset.
 
 
 ### _method_ `.get_workspace_containers(name: str = None, include_folders: bool = False) -> List[ContainerAssetModel]`
 Returns a list of `ContainerAssetModel` instances optionally filtered by _name_ and if it should include folders.
 
 > Args:
-> - _name_: The name of the container.
+> - _name_ (Optional): The name of the container/folder.
 > - _include\_folders_ (Optional): A boolean indicating if folders should be retrieved as well as workspaces. 
 
 
 ### _method_ `.move_workspace_asset(asset: AssetModel|str, target_container: ContainerAssetModel|str, new_name: str = None, hidden: bool = False) -> AssetModel`
-Change location of a workspace asset. Also allows to optionally rename, and to make an asset visibe or hidden. Returns a moved `AssetModel` instance.
+Change location of a workspace asset. Also allows to optionally rename, and to make an asset visible or hidden. Returns a moved `AssetModel` instance.
 
 > Args:
 > - _asset_: The id of the asset to move, or an instance of iqvia_360.AssetModel
 > - _target\_container_: The id of the container the asset is being moved to, or an instance of iqvia_360.ContainerAssetModel
 > - _new_name_ (Optional): The new name of the asset.
 > - _hidden_ (Optional): A boolean indicating if the asset should not be visible in workspaces.
 
@@ -204,15 +206,15 @@
 ### _method_ `.download_adt_report_by_id(report_id: str, location: pathlib.Path | str, content_type: str) -> pathlib.Path | None`
 Download the requested analytic dataset report to the local environment. The format of the report is pre-determined at the time of generation from its definition.
 Returns a `Path` object pointing to the downloaded report, or `None` if the download failed.
 
 >Args:
 >- _report_id_: The id of the analytic dataset report to download.
 >- _location_: The directory where the report should be downloaded.
->- _content_type_: They content type of the download request. Needs to be one of text/csv, application/vnd.apache.parquet or application/zip
+>- _content_type_: They content type of the download request. Needs to be one of `text/csv`, `application/vnd.apache.parquet` or `application/zip`
 
 
 ### _method_ `.create_workspace_asset(asset: AssetModel) -> AssetModel`
 Given an instance of `AssetModel`, create it on workspaces.
 Returns the instance of the `asset`.
 
 
@@ -231,28 +233,29 @@
 Upload a local document file into E360 workspaces.
 Returns an instance of `AnalyticDatasetModel` for the newly created report.
 
 >Args:
 >- _target_container_: The id of the container the ADT asset is created in, or an instance of iqvia_360.ContainerAssetModel
 >- _file_path_: The path to report that will be uploaded
 >- _name_: The asset name for the uploaded report
->- _granularity_: The granularity of the data. Values can be selected from `iqvia_e360.Granularity`
->- _format__: The format of the data uploaded. Values can be selected from `iqvia_e360.AnalyticDatasetFormat`
+>- _granularity_: The granularity of the data. Values can be selected from `adt_clients.models.Granularity` - please look at the specific adt_clients package version to get the list of supported values.
+>- _format__: The format of the data uploaded. Values can be selected from `adt_clients.models.AnalyticDatasetFormat` - please look at the specific adt_clients package version to get the list of supported values.
 >- _dataset_release_id_ (Optional): The dataset_release_id that should be associated with this data.
 
 
-### _method_ `.create_plotly_visualization(self, vis_payload: dict, target_container: ContainerModel|str, name: str, description: str = "") -> AssetModel`
+### _method_ `.create_plotly_visualization(vis_payload: dict, target_container: ContainerModel|str, name: str, description: str = "", from_plotly: bool = True) -> AssetModel`
 Provided a plotly figure object, create an E360 visualisation.
 Returns an `AssetModel` for the newly created asset.
 
 >Args:
 >- vis_payload: A plotly figure object.
 >- _target_container_: The id of the container the visualisation asset is created in, or an instance of `ContainerAssetModel`
 >- _name_: The asset name for the uploaded visualisation
 >- _description_ (Optional): An asset description for the uploaded visualisation
+>- _from_plotly_ (Optional): Flag to convert from a plotly payload to a VRS payload structure
 
 Example: create a simple Plotly object, and create a visualisation in the first container:
 ```python
 import plotly.graph_objects as go
 from iqvia_e360 import E360Context
 
 context = E360Context.create_from_settings(...)
@@ -290,19 +293,19 @@
 ```
 
 
 ## Models
 
 Models help keep E360 Assets organised and encapsulate their desired features.
 
-## _class_ `AssetModel`
+## _class_ `AssetModel(BaseModel)`
 A model from `workspace_clients.AssetModel`, which is commonly used to store metadata to assets in the workspaces.
 
 
-## _class_ `ClientStoreAssetModel`
+## _class_ `ClientStoreAssetModel(AssetModel)`
 Base class model, from which all other model classes inherit from.
 
 ### _method_ `.delete(purge: bool = False) -> bool`
 Deletes the asset from the Workspaces. Set `purge` to `True` to delete any child assets.
 
 
 ## _class_ `ContainerAssetModel(ClientStoreAssetModel)`
@@ -311,16 +314,16 @@
 ### _method_ `.upload_adt_file(file_path: pathlib.Path|str, name: str, granularity: Granularity, format_: AnalyticDatasetFormat, dataset_release_id: str = None) -> AnalyticDatasetModel`
 Uploads a tabular file as an ADT report asset file into container.
 Returns an instance of `AnalyticDatasetModel` for the newly created report.
 
 >Args:
 >- _file_path_: The path to report that will be uploaded
 >- _name_: The asset name for the uploaded report
->- _granularity_: The granularity of the data. Values can be selected from `iqvia_e360.Granularity`
->- _format__: The format of the data uploaded. Values can be selected from `iqvia_e360.AnalyticDatasetFormat`
+>- _granularity_: The granularity of the data. Values can be selected from `adt_clients.models.Granularity` - please look at the specific adt_clients package version to get the list of supported values.
+>- _format__: The format of the data uploaded. Values can be selected from `adt_clients.models.AnalyticDatasetFormat` - please look at the specific adt_clients package version to get the list of supported values.
 >- _dataset_release_id_ (Optional): The dataset_release_id that should be associated with this data.
 
 Example:
 ```python
 container = ContainerAssetModel(...)
 my_adt = container.upload_adt_file('my_file.csv', 'My File', 'csv', 'patient')
 ```
@@ -341,14 +344,14 @@
 ## _class_ `AdtDefinitionAssetModel(ClientStoreAssetModel)`
 Model class used to represent ADT definition asset metadata.
 
 
 ## _class_ `AdtReportAssetModel(ClientStoreAssetModel)`
 Model class used to represent ADT report asset metadata.
 
-### _method_ `.download(location: pathlib.Path|str) -> pathlib.Path`
-Downloads the ADT report to the `location` path specified.
+### _method_ `.download(location: pathlib.Path|str = None) -> pathlib.Path`
+Downloads the ADT report to the `location` path specified (optional).
 
 
 # Support
 
 If you are having issues with using this library, please contact our E360 support team.
```

## Comparing `iqvia_e360-0.9.4.dist-info/RECORD` & `iqvia_e360-0.9.5.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-iqvia_e360/__init__.py,sha256=zFj7fk0tGN-FexR0qVIdoubLH7nws-5K4TRS5rEY-tA,1020
+iqvia_e360/__init__.py,sha256=D0BPRkeVzPdzs1kauvsBNeXyRdZpWPKVkdRYXNvQDd8,1020
 iqvia_e360/e360_context.py,sha256=m19de0PUmxPhQnWzu06t0J5WliTI4wXcmjD5c15v-nE,16251
 iqvia_e360/exceptions.py,sha256=Cp-_7l8ua_KQOe3hezR6Q4aTtO9wyjZW0y_OewQilB4,46
 iqvia_e360/models.py,sha256=_YEtljmdFEXs4RJ4EDfRs5k9tznXb5M2atdNNIYxu38,8212
 iqvia_e360/settings.py,sha256=ULzhKligNseb-2tvX2M9B0F93EY9r2gAG5aJOfcKI5E,2134
-iqvia_e360-0.9.4.dist-info/LICENSE.txt,sha256=I7qhxQ9AQQRmqxoonhxW1b4hE1pOxxnyWE9WbrX5E4A,575
-iqvia_e360-0.9.4.dist-info/METADATA,sha256=mX26N4u7VxOkrKY-mxYKaBUBhzirINHLt6VK1KGK-vM,14607
-iqvia_e360-0.9.4.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-iqvia_e360-0.9.4.dist-info/top_level.txt,sha256=rDG5kahPvmmbxdzalYuRpengVgnW-0gCOIs7In0iWEY,11
-iqvia_e360-0.9.4.dist-info/RECORD,,
+iqvia_e360-0.9.5.dist-info/LICENSE.txt,sha256=I7qhxQ9AQQRmqxoonhxW1b4hE1pOxxnyWE9WbrX5E4A,575
+iqvia_e360-0.9.5.dist-info/METADATA,sha256=idAtquaX1tBH8LFGG43bqxGxmVXlBPTqnikyzYa88CE,15456
+iqvia_e360-0.9.5.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+iqvia_e360-0.9.5.dist-info/top_level.txt,sha256=rDG5kahPvmmbxdzalYuRpengVgnW-0gCOIs7In0iWEY,11
+iqvia_e360-0.9.5.dist-info/RECORD,,
```

