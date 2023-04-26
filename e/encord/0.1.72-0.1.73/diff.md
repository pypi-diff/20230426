# Comparing `tmp/encord-0.1.72.tar.gz` & `tmp/encord-0.1.73.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encord-0.1.72.tar", max compression
+gzip compressed data, was "encord-0.1.73.tar", max compression
```

## Comparing `encord-0.1.72.tar` & `encord-0.1.73.tar`

### file list

```diff
@@ -1,73 +1,73 @@
--rw-r--r--   0        0        0    11330 2023-04-06 09:37:05.100408 encord-0.1.72/LICENSE
--rw-r--r--   0        0        0     2595 2023-04-06 09:37:05.100408 encord-0.1.72/README.md
--rw-r--r--   0        0        0       84 2023-04-06 09:37:05.100408 encord-0.1.72/cord/__init__.py
--rw-r--r--   0        0        0      158 2023-04-06 09:37:05.112408 encord-0.1.72/encord/__init__.py
--rw-r--r--   0        0        0      214 2023-04-06 09:37:05.112408 encord-0.1.72/encord/_version.py
--rw-r--r--   0        0        0    47245 2023-04-06 09:37:05.116408 encord-0.1.72/encord/client.py
--rw-r--r--   0        0        0    10826 2023-04-06 09:37:05.116408 encord-0.1.72/encord/configs.py
--rw-r--r--   0        0        0        0 2023-04-06 09:37:05.116408 encord-0.1.72/encord/constants/__init__.py
--rw-r--r--   0        0        0      810 2023-04-06 09:37:05.116408 encord-0.1.72/encord/constants/enums.py
--rw-r--r--   0        0        0     3211 2023-04-06 09:37:05.116408 encord-0.1.72/encord/constants/model.py
--rw-r--r--   0        0        0     6068 2023-04-06 09:37:05.116408 encord-0.1.72/encord/constants/model_weights.py
--rw-r--r--   0        0        0     1119 2023-04-06 09:37:05.116408 encord-0.1.72/encord/constants/string_constants.py
--rw-r--r--   0        0        0        0 2023-04-06 09:37:05.116408 encord-0.1.72/encord/constants/test/__init__.py
--rw-r--r--   0        0        0      634 2023-04-06 09:37:05.116408 encord-0.1.72/encord/constants/test/test_enums.py
--rw-r--r--   0        0        0    16035 2023-04-06 09:37:05.116408 encord-0.1.72/encord/dataset.py
--rw-r--r--   0        0        0     5621 2023-04-06 09:37:05.116408 encord-0.1.72/encord/exceptions.py
--rw-r--r--   0        0        0        0 2023-04-06 09:37:05.116408 encord-0.1.72/encord/http/__init__.py
--rw-r--r--   0        0        0      535 2023-04-06 09:37:05.116408 encord-0.1.72/encord/http/constants.py
--rw-r--r--   0        0        0     6275 2023-04-06 09:37:05.116408 encord-0.1.72/encord/http/error_utils.py
--rw-r--r--   0        0        0     5999 2023-04-06 09:37:05.116408 encord-0.1.72/encord/http/querier.py
--rw-r--r--   0        0        0      697 2023-04-06 09:37:05.116408 encord-0.1.72/encord/http/query_methods.py
--rw-r--r--   0        0        0     1691 2023-04-06 09:37:05.116408 encord-0.1.72/encord/http/request.py
--rw-r--r--   0        0        0     5880 2023-04-06 09:37:05.116408 encord-0.1.72/encord/http/utils.py
--rw-r--r--   0        0        0      340 2023-04-06 09:37:05.116408 encord-0.1.72/encord/objects/__init__.py
--rw-r--r--   0        0        0      145 2023-04-06 09:37:05.116408 encord-0.1.72/encord/objects/classification.py
--rw-r--r--   0        0        0    29710 2023-04-06 09:37:05.116408 encord-0.1.72/encord/objects/common.py
--rw-r--r--   0        0        0      172 2023-04-06 09:37:05.116408 encord-0.1.72/encord/objects/constants.py
--rw-r--r--   0        0        0     5631 2023-04-06 09:37:05.116408 encord-0.1.72/encord/objects/coordinates.py
--rw-r--r--   0        0        0     3419 2023-04-06 09:37:05.116408 encord-0.1.72/encord/objects/frames.py
--rw-r--r--   0        0        0    21036 2023-04-06 09:37:05.116408 encord-0.1.72/encord/objects/internal_helpers.py
--rw-r--r--   0        0        0   132198 2023-04-06 09:37:05.116408 encord-0.1.72/encord/objects/ontology_labels_impl.py
--rw-r--r--   0        0        0      137 2023-04-06 09:37:05.116408 encord-0.1.72/encord/objects/ontology_object.py
--rw-r--r--   0        0        0      148 2023-04-06 09:37:05.116408 encord-0.1.72/encord/objects/ontology_structure.py
--rw-r--r--   0        0        0      549 2023-04-06 09:37:05.116408 encord-0.1.72/encord/objects/project.py
--rw-r--r--   0        0        0     1240 2023-04-06 09:37:05.116408 encord-0.1.72/encord/objects/utils.py
--rw-r--r--   0        0        0     3430 2023-04-06 09:37:05.116408 encord-0.1.72/encord/ontology.py
--rw-r--r--   0        0        0        0 2023-04-06 09:37:05.116408 encord-0.1.72/encord/orm/__init__.py
--rw-r--r--   0        0        0      982 2023-04-06 09:37:05.116408 encord-0.1.72/encord/orm/api_key.py
--rw-r--r--   0        0        0     5377 2023-04-06 09:37:05.116408 encord-0.1.72/encord/orm/base_orm.py
--rw-r--r--   0        0        0      111 2023-04-06 09:37:05.116408 encord-0.1.72/encord/orm/cloud_integration.py
--rw-r--r--   0        0        0    32208 2023-04-06 09:37:05.116408 encord-0.1.72/encord/orm/dataset.py
--rw-r--r--   0        0        0      828 2023-04-06 09:37:05.116408 encord-0.1.72/encord/orm/dataset_with_user_role.py
--rw-r--r--   0        0        0      201 2023-04-06 09:37:05.116408 encord-0.1.72/encord/orm/formatter.py
--rw-r--r--   0        0        0     1155 2023-04-06 09:37:05.116408 encord-0.1.72/encord/orm/label_log.py
--rw-r--r--   0        0        0    11122 2023-04-06 09:37:05.116408 encord-0.1.72/encord/orm/label_row.py
--rw-r--r--   0        0        0     1577 2023-04-06 09:37:05.116408 encord-0.1.72/encord/orm/labeling_algorithm.py
--rw-r--r--   0        0        0     6688 2023-04-06 09:37:05.116408 encord-0.1.72/encord/orm/model.py
--rw-r--r--   0        0        0      745 2023-04-06 09:37:05.116408 encord-0.1.72/encord/orm/ontology.py
--rw-r--r--   0        0        0     8844 2023-04-06 09:37:05.116408 encord-0.1.72/encord/orm/project.py
--rw-r--r--   0        0        0      625 2023-04-06 09:37:05.116408 encord-0.1.72/encord/orm/project_api_key.py
--rw-r--r--   0        0        0      828 2023-04-06 09:37:05.116408 encord-0.1.72/encord/orm/project_with_user_role.py
--rw-r--r--   0        0        0        0 2023-04-06 09:37:05.116408 encord-0.1.72/encord/orm/test/__init__.py
--rw-r--r--   0        0        0      570 2023-04-06 09:37:05.116408 encord-0.1.72/encord/orm/test/test_dataset.py
--rw-r--r--   0        0        0    38214 2023-04-06 09:37:05.116408 encord-0.1.72/encord/project.py
--rw-r--r--   0        0        0        0 2023-04-06 09:37:05.116408 encord-0.1.72/encord/project_ontology/__init__.py
--rw-r--r--   0        0        0     1316 2023-04-06 09:37:05.116408 encord-0.1.72/encord/project_ontology/classification_attribute.py
--rw-r--r--   0        0        0      525 2023-04-06 09:37:05.116408 encord-0.1.72/encord/project_ontology/classification_option.py
--rw-r--r--   0        0        0      357 2023-04-06 09:37:05.116408 encord-0.1.72/encord/project_ontology/classification_type.py
--rw-r--r--   0        0        0      237 2023-04-06 09:37:05.116408 encord-0.1.72/encord/project_ontology/object_type.py
--rw-r--r--   0        0        0     9526 2023-04-06 09:37:05.116408 encord-0.1.72/encord/project_ontology/ontology.py
--rw-r--r--   0        0        0      630 2023-04-06 09:37:05.116408 encord-0.1.72/encord/project_ontology/ontology_classification.py
--rw-r--r--   0        0        0      683 2023-04-06 09:37:05.116408 encord-0.1.72/encord/project_ontology/ontology_object.py
--rw-r--r--   0        0        0    27803 2023-04-06 09:37:05.116408 encord-0.1.72/encord/user_client.py
--rw-r--r--   0        0        0        0 2023-04-06 09:37:05.116408 encord-0.1.72/encord/utilities/__init__.py
--rw-r--r--   0        0        0     4231 2023-04-06 09:37:05.116408 encord-0.1.72/encord/utilities/client_utilities.py
--rw-r--r--   0        0        0      253 2023-04-06 09:37:05.116408 encord-0.1.72/encord/utilities/common.py
--rw-r--r--   0        0        0     3270 2023-04-06 09:37:05.116408 encord-0.1.72/encord/utilities/label_utilities.py
--rw-r--r--   0        0        0      343 2023-04-06 09:37:05.116408 encord-0.1.72/encord/utilities/ontology_user.py
--rw-r--r--   0        0        0      578 2023-04-06 09:37:05.116408 encord-0.1.72/encord/utilities/project_user.py
--rw-r--r--   0        0        0      467 2023-04-06 09:37:05.116408 encord-0.1.72/encord/utilities/project_utilities.py
--rw-r--r--   0        0        0     1835 2023-04-06 09:37:05.120408 encord-0.1.72/pyproject.toml
--rw-r--r--   0        0        0     3724 2023-04-06 09:38:22.446503 encord-0.1.72/setup.py
--rw-r--r--   0        0        0     3726 2023-04-06 09:38:22.446895 encord-0.1.72/PKG-INFO
+-rw-r--r--   0        0        0    11330 2023-04-26 13:30:18.704367 encord-0.1.73/LICENSE
+-rw-r--r--   0        0        0     2595 2023-04-26 13:30:18.704367 encord-0.1.73/README.md
+-rw-r--r--   0        0        0       84 2023-04-26 13:30:18.704367 encord-0.1.73/cord/__init__.py
+-rw-r--r--   0        0        0      158 2023-04-26 13:30:18.720368 encord-0.1.73/encord/__init__.py
+-rw-r--r--   0        0        0      214 2023-04-26 13:30:18.720368 encord-0.1.73/encord/_version.py
+-rw-r--r--   0        0        0    47245 2023-04-26 13:30:18.720368 encord-0.1.73/encord/client.py
+-rw-r--r--   0        0        0    10825 2023-04-26 13:30:18.720368 encord-0.1.73/encord/configs.py
+-rw-r--r--   0        0        0        0 2023-04-26 13:30:18.720368 encord-0.1.73/encord/constants/__init__.py
+-rw-r--r--   0        0        0      810 2023-04-26 13:30:18.720368 encord-0.1.73/encord/constants/enums.py
+-rw-r--r--   0        0        0     3211 2023-04-26 13:30:18.720368 encord-0.1.73/encord/constants/model.py
+-rw-r--r--   0        0        0     6068 2023-04-26 13:30:18.720368 encord-0.1.73/encord/constants/model_weights.py
+-rw-r--r--   0        0        0     1119 2023-04-26 13:30:18.720368 encord-0.1.73/encord/constants/string_constants.py
+-rw-r--r--   0        0        0        0 2023-04-26 13:30:18.720368 encord-0.1.73/encord/constants/test/__init__.py
+-rw-r--r--   0        0        0      634 2023-04-26 13:30:18.720368 encord-0.1.73/encord/constants/test/test_enums.py
+-rw-r--r--   0        0        0    16035 2023-04-26 13:30:18.720368 encord-0.1.73/encord/dataset.py
+-rw-r--r--   0        0        0     5621 2023-04-26 13:30:18.720368 encord-0.1.73/encord/exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-26 13:30:18.720368 encord-0.1.73/encord/http/__init__.py
+-rw-r--r--   0        0        0      535 2023-04-26 13:30:18.720368 encord-0.1.73/encord/http/constants.py
+-rw-r--r--   0        0        0     6275 2023-04-26 13:30:18.720368 encord-0.1.73/encord/http/error_utils.py
+-rw-r--r--   0        0        0     5999 2023-04-26 13:30:18.720368 encord-0.1.73/encord/http/querier.py
+-rw-r--r--   0        0        0      697 2023-04-26 13:30:18.720368 encord-0.1.73/encord/http/query_methods.py
+-rw-r--r--   0        0        0     1691 2023-04-26 13:30:18.720368 encord-0.1.73/encord/http/request.py
+-rw-r--r--   0        0        0     5880 2023-04-26 13:30:18.720368 encord-0.1.73/encord/http/utils.py
+-rw-r--r--   0        0        0      340 2023-04-26 13:30:18.720368 encord-0.1.73/encord/objects/__init__.py
+-rw-r--r--   0        0        0      145 2023-04-26 13:30:18.720368 encord-0.1.73/encord/objects/classification.py
+-rw-r--r--   0        0        0    29709 2023-04-26 13:30:18.720368 encord-0.1.73/encord/objects/common.py
+-rw-r--r--   0        0        0      172 2023-04-26 13:30:18.720368 encord-0.1.73/encord/objects/constants.py
+-rw-r--r--   0        0        0     5631 2023-04-26 13:30:18.720368 encord-0.1.73/encord/objects/coordinates.py
+-rw-r--r--   0        0        0     3419 2023-04-26 13:30:18.720368 encord-0.1.73/encord/objects/frames.py
+-rw-r--r--   0        0        0    21407 2023-04-26 13:30:18.720368 encord-0.1.73/encord/objects/internal_helpers.py
+-rw-r--r--   0        0        0   132196 2023-04-26 13:30:18.720368 encord-0.1.73/encord/objects/ontology_labels_impl.py
+-rw-r--r--   0        0        0      137 2023-04-26 13:30:18.720368 encord-0.1.73/encord/objects/ontology_object.py
+-rw-r--r--   0        0        0      148 2023-04-26 13:30:18.720368 encord-0.1.73/encord/objects/ontology_structure.py
+-rw-r--r--   0        0        0      549 2023-04-26 13:30:18.720368 encord-0.1.73/encord/objects/project.py
+-rw-r--r--   0        0        0     1240 2023-04-26 13:30:18.720368 encord-0.1.73/encord/objects/utils.py
+-rw-r--r--   0        0        0     3430 2023-04-26 13:30:18.720368 encord-0.1.73/encord/ontology.py
+-rw-r--r--   0        0        0        0 2023-04-26 13:30:18.720368 encord-0.1.73/encord/orm/__init__.py
+-rw-r--r--   0        0        0      982 2023-04-26 13:30:18.720368 encord-0.1.73/encord/orm/api_key.py
+-rw-r--r--   0        0        0     5377 2023-04-26 13:30:18.720368 encord-0.1.73/encord/orm/base_orm.py
+-rw-r--r--   0        0        0      111 2023-04-26 13:30:18.720368 encord-0.1.73/encord/orm/cloud_integration.py
+-rw-r--r--   0        0        0    32206 2023-04-26 13:30:18.720368 encord-0.1.73/encord/orm/dataset.py
+-rw-r--r--   0        0        0      828 2023-04-26 13:30:18.720368 encord-0.1.73/encord/orm/dataset_with_user_role.py
+-rw-r--r--   0        0        0      201 2023-04-26 13:30:18.720368 encord-0.1.73/encord/orm/formatter.py
+-rw-r--r--   0        0        0     1155 2023-04-26 13:30:18.720368 encord-0.1.73/encord/orm/label_log.py
+-rw-r--r--   0        0        0    11122 2023-04-26 13:30:18.720368 encord-0.1.73/encord/orm/label_row.py
+-rw-r--r--   0        0        0     1577 2023-04-26 13:30:18.720368 encord-0.1.73/encord/orm/labeling_algorithm.py
+-rw-r--r--   0        0        0     6687 2023-04-26 13:30:18.720368 encord-0.1.73/encord/orm/model.py
+-rw-r--r--   0        0        0      745 2023-04-26 13:30:18.720368 encord-0.1.73/encord/orm/ontology.py
+-rw-r--r--   0        0        0     8844 2023-04-26 13:30:18.720368 encord-0.1.73/encord/orm/project.py
+-rw-r--r--   0        0        0      625 2023-04-26 13:30:18.720368 encord-0.1.73/encord/orm/project_api_key.py
+-rw-r--r--   0        0        0      828 2023-04-26 13:30:18.720368 encord-0.1.73/encord/orm/project_with_user_role.py
+-rw-r--r--   0        0        0        0 2023-04-26 13:30:18.720368 encord-0.1.73/encord/orm/test/__init__.py
+-rw-r--r--   0        0        0      570 2023-04-26 13:30:18.720368 encord-0.1.73/encord/orm/test/test_dataset.py
+-rw-r--r--   0        0        0    38298 2023-04-26 13:30:18.720368 encord-0.1.73/encord/project.py
+-rw-r--r--   0        0        0        0 2023-04-26 13:30:18.720368 encord-0.1.73/encord/project_ontology/__init__.py
+-rw-r--r--   0        0        0     1316 2023-04-26 13:30:18.720368 encord-0.1.73/encord/project_ontology/classification_attribute.py
+-rw-r--r--   0        0        0      525 2023-04-26 13:30:18.720368 encord-0.1.73/encord/project_ontology/classification_option.py
+-rw-r--r--   0        0        0      357 2023-04-26 13:30:18.720368 encord-0.1.73/encord/project_ontology/classification_type.py
+-rw-r--r--   0        0        0      237 2023-04-26 13:30:18.724368 encord-0.1.73/encord/project_ontology/object_type.py
+-rw-r--r--   0        0        0     9526 2023-04-26 13:30:18.724368 encord-0.1.73/encord/project_ontology/ontology.py
+-rw-r--r--   0        0        0      630 2023-04-26 13:30:18.724368 encord-0.1.73/encord/project_ontology/ontology_classification.py
+-rw-r--r--   0        0        0      683 2023-04-26 13:30:18.724368 encord-0.1.73/encord/project_ontology/ontology_object.py
+-rw-r--r--   0        0        0    27801 2023-04-26 13:30:18.724368 encord-0.1.73/encord/user_client.py
+-rw-r--r--   0        0        0        0 2023-04-26 13:30:18.724368 encord-0.1.73/encord/utilities/__init__.py
+-rw-r--r--   0        0        0     4231 2023-04-26 13:30:18.724368 encord-0.1.73/encord/utilities/client_utilities.py
+-rw-r--r--   0        0        0      253 2023-04-26 13:30:18.724368 encord-0.1.73/encord/utilities/common.py
+-rw-r--r--   0        0        0     3270 2023-04-26 13:30:18.724368 encord-0.1.73/encord/utilities/label_utilities.py
+-rw-r--r--   0        0        0      343 2023-04-26 13:30:18.724368 encord-0.1.73/encord/utilities/ontology_user.py
+-rw-r--r--   0        0        0      578 2023-04-26 13:30:18.724368 encord-0.1.73/encord/utilities/project_user.py
+-rw-r--r--   0        0        0      467 2023-04-26 13:30:18.724368 encord-0.1.73/encord/utilities/project_utilities.py
+-rw-r--r--   0        0        0     1681 2023-04-26 13:30:18.724368 encord-0.1.73/pyproject.toml
+-rw-r--r--   0        0        0     3724 2023-04-26 13:31:35.974219 encord-0.1.73/setup.py
+-rw-r--r--   0        0        0     3726 2023-04-26 13:31:35.974603 encord-0.1.73/PKG-INFO
```

### Comparing `encord-0.1.72/LICENSE` & `encord-0.1.73/LICENSE`

 * *Files identical despite different names*

### Comparing `encord-0.1.72/README.md` & `encord-0.1.73/README.md`

 * *Files identical despite different names*

### Comparing `encord-0.1.72/encord/client.py` & `encord-0.1.73/encord/client.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.72/encord/configs.py` & `encord-0.1.73/encord/configs.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,15 +149,14 @@
         self,
         resource_id: Optional[str] = None,
         web_file_path: str = ENCORD_PUBLIC_PATH,
         domain: Optional[str] = None,
         websocket_endpoint: str = WEBSOCKET_ENDPOINT,
         requests_settings: RequestsSettings = DEFAULT_REQUESTS_SETTINGS,
     ):
-
         if resource_id is None:
             resource_id = get_env_resource_id()
 
         self.resource_id = resource_id
         self.websocket_endpoint = websocket_endpoint
         if domain is None:
             raise RuntimeError("`domain` must be specified")
```

### Comparing `encord-0.1.72/encord/constants/enums.py` & `encord-0.1.73/encord/constants/enums.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.72/encord/constants/model.py` & `encord-0.1.73/encord/constants/model.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.72/encord/constants/model_weights.py` & `encord-0.1.73/encord/constants/model_weights.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.72/encord/constants/string_constants.py` & `encord-0.1.73/encord/constants/string_constants.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.72/encord/constants/test/test_enums.py` & `encord-0.1.73/encord/constants/test/test_enums.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.72/encord/dataset.py` & `encord-0.1.73/encord/dataset.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.72/encord/exceptions.py` & `encord-0.1.73/encord/exceptions.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.72/encord/http/constants.py` & `encord-0.1.73/encord/http/constants.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.72/encord/http/error_utils.py` & `encord-0.1.73/encord/http/error_utils.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.72/encord/http/querier.py` & `encord-0.1.73/encord/http/querier.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.72/encord/http/query_methods.py` & `encord-0.1.73/encord/http/query_methods.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.72/encord/http/request.py` & `encord-0.1.73/encord/http/request.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.72/encord/http/utils.py` & `encord-0.1.73/encord/http/utils.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.72/encord/objects/common.py` & `encord-0.1.73/encord/objects/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -708,15 +708,14 @@
     cls: Type[OT],
     label: str,
     parent_uid: List[int],
     local_uid: Optional[int] = None,
     feature_node_hash: Optional[str] = None,
     value: Optional[str] = None,
 ) -> OT:
-
     local_uid, feature_node_hash = __build_identifiers(options, local_uid, feature_node_hash)
     if not value:
         value = re.sub(r"[\s]", "_", label).lower()
     option = cls(parent_uid + [local_uid], feature_node_hash, label, value)
     options.append(option)
     return option
```

### Comparing `encord-0.1.72/encord/objects/coordinates.py` & `encord-0.1.73/encord/objects/coordinates.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.72/encord/objects/frames.py` & `encord-0.1.73/encord/objects/frames.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.72/encord/objects/internal_helpers.py` & `encord-0.1.73/encord/objects/internal_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,21 +142,24 @@
             raise ValueError("Cannot set the value of a TextAnswer based on a different ontology attribute.")
 
         self._answered = True
         self.set(d["answers"])
         self.is_manual_annotation = d["manualAnnotation"]
 
     def __hash__(self):
-        return hash((self._value, type(self).__name__))
+        return hash((self._ontology_attribute.feature_node_hash, self._value, type(self).__name__))
 
     def __eq__(self, other: TextAnswer) -> bool:
         if not isinstance(other, TextAnswer):
             return False
         else:
-            return self._value == other._value
+            return (
+                self._ontology_attribute.feature_node_hash == other._ontology_attribute.feature_node_hash
+                and self._value == other._value
+            )
 
     def __repr__(self):
         return f"{self.__class__.__name__}({self._value})"
 
 
 @dataclass
 class RadioAnswer(Answer):
@@ -226,21 +229,24 @@
 
         answer = answers[0]
         nestable_option = _get_option_by_hash(answer["featureHash"], self.ontology_attribute.options)
         self.set(nestable_option)
         self.is_manual_annotation = d["manualAnnotation"]
 
     def __hash__(self):
-        return hash((self._value, type(self).__name__))
+        return hash((self.ontology_attribute.feature_node_hash, self._value, type(self).__name__))
 
     def __eq__(self, other: RadioAnswer) -> bool:
         if not isinstance(other, RadioAnswer):
             return False
         else:
-            return self._value == other._value
+            return (
+                self._ontology_attribute.feature_node_hash == other._ontology_attribute.feature_node_hash
+                and self._value == other._value
+            )
 
     def __repr__(self):
         return f"{self.__class__.__name__}({self._value})"
 
 
 @dataclass
 class ChecklistAnswer(Answer):
```

### Comparing `encord-0.1.72/encord/objects/ontology_labels_impl.py` & `encord-0.1.73/encord/objects/ontology_labels_impl.py`

 * *Files 0% similar despite different names*

```diff
@@ -1342,15 +1342,14 @@
         This class can be used to inspect what object/classification instances are on a given frame or
         what metadata, such as a image file size, is on a given frame.
         """
 
         def __init__(
             self, label_row: LabelRowV2, label_row_read_only_data: LabelRowV2.LabelRowReadOnlyData, frame: int
         ):
-
             self._label_row = label_row
             self._label_row_read_only_data = label_row_read_only_data
             self._frame = frame
 
         @property
         def image_hash(self) -> str:
             if self._label_row.data_type not in [DataType.IMAGE, DataType.IMG_GROUP]:
@@ -1985,15 +1984,14 @@
         self._add_static_answers_from_dict(classification_instance, answers_dict)
 
         return classification_instance
 
     def _add_static_answers_from_dict(
         self, classification_instance: ClassificationInstance, answers_list: List[dict]
     ) -> None:
-
         classification_instance.set_answer_from_list(answers_list)
 
     def _add_frames_to_classification_instance(self, frame_classification_label: dict, frame: int) -> None:
         object_hash = frame_classification_label["classificationHash"]
         classification_instance = self._classifications_map[object_hash]
         frame_view = ClassificationInstance.FrameData.from_dict(frame_classification_label)
```

### Comparing `encord-0.1.72/encord/objects/project.py` & `encord-0.1.73/encord/objects/project.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.72/encord/objects/utils.py` & `encord-0.1.73/encord/objects/utils.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.72/encord/ontology.py` & `encord-0.1.73/encord/ontology.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.72/encord/orm/api_key.py` & `encord-0.1.73/encord/orm/api_key.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.72/encord/orm/base_orm.py` & `encord-0.1.73/encord/orm/base_orm.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.72/encord/orm/dataset.py` & `encord-0.1.73/encord/orm/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,14 @@
         storage_location: StorageLocation,
         created_at: datetime,
         last_edited_at: datetime,
         width: int,
         signed_url: Optional[str],
         height: int,
     ):
-
         self._image_hash = image_hash
         self._title = title
         self._file_link = file_link
         self._file_type = file_type
         self._file_size = file_size
         self._storage_location = storage_location
         self._created_at = created_at
@@ -200,15 +199,14 @@
         client_metadata: Optional[dict],
         frames_per_second: Optional[int],
         duration: Optional[int],
         images_data: Optional[List[dict]],
         signed_url: Optional[str],
         is_optimised_image_group: Optional[bool],
     ):
-
         parsed_images = None
         if images_data is not None:
             parsed_images = [ImageData.from_dict(image_data) for image_data in images_data]
 
         super().__init__(
             {
                 "data_hash": uid,
```

### Comparing `encord-0.1.72/encord/orm/dataset_with_user_role.py` & `encord-0.1.73/encord/orm/dataset_with_user_role.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.72/encord/orm/label_log.py` & `encord-0.1.73/encord/orm/label_log.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.72/encord/orm/label_row.py` & `encord-0.1.73/encord/orm/label_row.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.72/encord/orm/labeling_algorithm.py` & `encord-0.1.73/encord/orm/labeling_algorithm.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.72/encord/orm/model.py` & `encord-0.1.73/encord/orm/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,14 @@
     """
 
     DB_FIELDS = OrderedDict([("model_operation", int), ("model_parameters", dict)])
 
 
 @dataclass
 class ModelConfiguration(Formatter):
-
     model_uid: str
     title: str
     description: str
     feature_node_hashes: List[str]
     """The corresponding feature node hashes of the ontology object"""
     model: AutomationModels
     model_iteration_uids: List[str]
```

### Comparing `encord-0.1.72/encord/orm/ontology.py` & `encord-0.1.73/encord/orm/ontology.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.72/encord/orm/project.py` & `encord-0.1.73/encord/orm/project.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.72/encord/orm/project_api_key.py` & `encord-0.1.73/encord/orm/project_api_key.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.72/encord/orm/project_with_user_role.py` & `encord-0.1.73/encord/orm/project_with_user_role.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.72/encord/orm/test/test_dataset.py` & `encord-0.1.73/encord/orm/test/test_dataset.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.72/encord/project.py` & `encord-0.1.73/encord/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -284,16 +284,15 @@
             AuthenticationError: If the project API key is invalid.
             AuthorisationError: If access to the specified resource is restricted.
             ResourceNotFoundError: If one or more datasets don't exist by the specified dataset_hashes.
             UnknownError: If an error occurs while adding the datasets to the project.
             OperationNotAllowed: If the write operation is not allowed by the API key.
         """
         res = self._client.add_datasets(dataset_hashes)
-        if res:
-            self._invalidate_project_instance()
+        self._invalidate_project_instance()
         return res
 
     def remove_datasets(self, dataset_hashes: List[str]) -> bool:
         """
         Remove datasets from project
 
         Args:
@@ -306,16 +305,15 @@
             AuthenticationError: If the project API key is invalid.
             AuthorisationError: If access to the specified resource is restricted.
             ResourceNotFoundError: If no dataset exists by the specified dataset_hash (uid).
             UnknownError: If an error occurs while removing the datasets from the project.
             OperationNotAllowed: If the operation is not allowed by the API key.
         """
         res = self._client.remove_datasets(dataset_hashes)
-        if res:
-            self._invalidate_project_instance()
+        self._invalidate_project_instance()
         return res
 
     def get_project_ontology(self) -> LegacyOntology:
         """
         DEPRECATED - prefer using the `ontology` property accessor instead.
         """
         return self._client.get_project_ontology()
@@ -336,15 +334,17 @@
         Raises:
             AuthenticationError: If the project API key is invalid.
             AuthorisationError: If access to the specified resource is restricted.
             UnknownError: If an error occurs while add te object to the project ontology
             OperationNotAllowed: If the operation is not allowed by the API key.
             ValueError: If invalid arguments are supplied in the function call
         """
-        return self._client.add_object(name, shape)
+        res = self._client.add_object(name, shape)
+        self._invalidate_project_instance()
+        return res
 
     def add_classification(
         self,
         name: str,
         classification_type: ClassificationType,
         required: bool,
         options: Optional[Iterable[str]] = None,
@@ -363,15 +363,17 @@
         Raises:
             AuthenticationError: If the project API key is invalid.
             AuthorisationError: If access to the specified resource is restricted.
             UnknownError: If an error occurs while add te classification to the project ontology
             OperationNotAllowed: If the operation is not allowed by the API key.
             ValueError: If invalid arguments are supplied in the function call
         """
-        return self._client.add_classification(name, classification_type, required, options)
+        res = self._client.add_classification(name, classification_type, required, options)
+        self._invalidate_project_instance()
+        return res
 
     def list_models(self) -> List[ModelConfiguration]:
         """
         List all models that are associated with the project. Use the
         :meth:`encord.project.Project.get_training_metadata` to get more metadata about each training instance.
 
         .. code::
```

### Comparing `encord-0.1.72/encord/project_ontology/classification_attribute.py` & `encord-0.1.73/encord/project_ontology/classification_attribute.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.72/encord/project_ontology/classification_option.py` & `encord-0.1.73/encord/project_ontology/classification_option.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.72/encord/project_ontology/ontology.py` & `encord-0.1.73/encord/project_ontology/ontology.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.72/encord/project_ontology/ontology_classification.py` & `encord-0.1.73/encord/project_ontology/ontology_classification.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.72/encord/project_ontology/ontology_object.py` & `encord-0.1.73/encord/project_ontology/ontology_object.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.72/encord/user_client.py` & `encord-0.1.73/encord/user_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -585,15 +585,15 @@
             raise ValueError("Filter should be a dictionary")
 
         valid_filters = set([f.value for f in ListingFilter])
 
         ret = dict()
 
         # be relaxed with what we receive: translate raw strings to enum values
-        for (clause, val) in properties_filter.items():
+        for clause, val in properties_filter.items():
             if val is None:
                 continue
 
             if isinstance(clause, str):
                 if clause in valid_filters:
                     clause = ListingFilter(clause)
                 else:
```

### Comparing `encord-0.1.72/encord/utilities/client_utilities.py` & `encord-0.1.73/encord/utilities/client_utilities.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.72/encord/utilities/label_utilities.py` & `encord-0.1.73/encord/utilities/label_utilities.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.72/encord/utilities/project_user.py` & `encord-0.1.73/encord/utilities/project_user.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.72/pyproject.toml` & `encord-0.1.73/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "encord"
-version = "0.1.72"
+version = "0.1.73"
 description = "Encord Python SDK Client"
 authors = ["Cord Technologies Limited <hello@encord.com>"]
 license = "Apache Software License"
 keywords = ["cord", "encord"]
 packages = [
     { include = "cord"},
     { include = "encord"},
@@ -25,28 +25,26 @@
 cryptography = "^3.4.8"
 tqdm = "^4.32.1"
 importlib_metadata = {version = "^6.1.0", python = "<3.8"}
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.1.2"
 pre-commit = "^2.16.0"
-black = "^21.12b0"
+black = "^23.3.0"
 sphinx-tabs = "^3.3.1"
 sphinx-autodoc-typehints = "1.15.2"
 sphinx-codeautolink = "^0.10.0"
 sphinx-copybutton = "^0.5.0"
 sphinx-toolbox = "^3.4.0"
 prettyprinter = "0.18.0"
 isort = "^5.10.1"
 pydata-sphinx-theme = "^0.8.1"
 Pillow = "^9.1.0"
 sphinx-gallery = "^0.10.1"
 matplotlib = "^3.5.2"
-# Pinning click to solve black issues https://stackoverflow.com/questions/71673404/importerror-cannot-import-name-unicodefun-from-click
-click = "8.0.2"
 deepdiff = "^6.2.1"
 
 
 [build-system]
 requires = ["poetry-core>=1.3.2"]
 build-backend = "poetry.core.masonry.api"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `encord-0.1.72/setup.py` & `encord-0.1.73/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
  'tqdm>=4.32.1,<5.0.0']
 
 extras_require = \
 {':python_version < "3.8"': ['importlib_metadata>=6.1.0,<7.0.0']}
 
 setup_kwargs = {
     'name': 'encord',
-    'version': '0.1.72',
+    'version': '0.1.73',
     'description': 'Encord Python SDK Client',
     'long_description': '<h1 align="center">\n  <p align="center">Encord Python API Client</p>\n  <a href="https://encord.com"><img src="./docs/_static/logo.svg" width="100" alt="Cord logo"/></a>\n</h1>\n\n[![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)\n\n***The data engine for computer vision***\n\n## 💻 Features\n\n- Minimal low-level Python client that allows you to interact with Encord\'s API\n- Supports Python: `3.7`, `3.8`, `3.9`, and `3.10`\n\n## ✨ Relevant Links\n* [Encord website](https://encord.com)\n* [Encord web app](https://app.encord.com)\n* [Encord documentation](https://docs.encord.com)\n\n## 💡 Getting Started\n\nFor full documentation, please visit [Encord Python SDK](https://python.docs.encord.com/).\n\nFirst, install Encord Python API Client using the [pip](https://pip.pypa.io/en/stable/installing) package manager:\n\n```bash\npip install encord\n```\n\nThen, create an API key for authentication via the [Encord web app](https://app.encord.com). Pass the resource ID and API key as environment variables or pass them explicitly when you initialise the EncordClient object.\n\n```bash\nexport ENCORD_PROJECT_ID="<project_id>"\nexport ENCORD_API_KEY="<project_api_key>"\n```\n\nPassing the resource ID and API key as environment variables, you can initialise the Encord client directly.\n\n```python\nfrom encord.client import EncordClient\n\nclient = EncordClient.initialise()\n```\n\nIf you want to avoid setting environment variables, you can initialise the Encord client by passing the resource ID and API key as strings.\n\n```python\nfrom encord.client import EncordClient\n\nclient = EncordClient.initialise("<resource_id>", "<resource_api_key>")\n```\n\nIf you wish to instantiate several client objects and avoid passing parameters each time, you can instantiate a EncordConfig object, pass the resource ID and API key as strings, and initialise the client with the config object.\n\n```py\nfrom encord.client import EncordClient\nfrom encord.client import EncordConfig\n\nconfig = EncordConfig("<resource_id>", "<resource_api_key>")\nclient = EncordClient.initialise_with_config(config)\n```\n\nOnce you have instantiated an Encord client, it is easy to fetch information associated with the given resource ID.\n\n```py\nfrom encord.client import EncordClient\n\nclient = EncordClient.initialise()\nproject = client.get_project()\n```\n\n## 🐛 Troubleshooting\n\nPlease report bugs to [GitHub Issues](https://github.com/encord-team/encord-client-python/issues). Just make sure you read the [Encord documentation](https://docs.encord.com) and search for related issues first.\n',
     'author': 'Cord Technologies Limited',
     'author_email': 'hello@encord.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/encord-team/encord-client-python',
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['cord',
 'encord', 'encord.constants', 'encord.constants.test', 'encord.http',
 'encord.objects', 'encord.orm', 'encord.orm.test', 'encord.project_ontology',
 'encord.utilities'] package_data = \ {'': ['*']} install_requires = \
 ['cryptography>=3.4.8,<4.0.0', 'python-dateutil>=2.8.2,<3.0.0',
 'requests>=2.25.0,<3.0.0', 'tqdm>=4.32.1,<5.0.0'] extras_require = \ {':
 python_version < "3.8"': ['importlib_metadata>=6.1.0,<7.0.0']} setup_kwargs =
-{ 'name': 'encord', 'version': '0.1.72', 'description': 'Encord Python SDK
+{ 'name': 'encord', 'version': '0.1.73', 'description': 'Encord Python SDK
 Client', 'long_description': '
            ****** \nEncord Python API Client\n [Cord_logo]\n ******
 \n\n[![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)]
 (https://opensource.org/licenses/Apache-2.0)\n\n***The data engine for computer
 vision***\n\n## ð» Features\n\n- Minimal low-level Python client that allows
 you to interact with Encord\'s API\n- Supports Python: `3.7`, `3.8`, `3.9`, and
 `3.10`\n\n## â¨ Relevant Links\n* [Encord website](https://encord.com)\n*
```

### Comparing `encord-0.1.72/PKG-INFO` & `encord-0.1.73/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: encord
-Version: 0.1.72
+Version: 0.1.73
 Summary: Encord Python SDK Client
 Home-page: https://github.com/encord-team/encord-client-python
 License: Apache Software License
 Keywords: cord,encord
 Author: Cord Technologies Limited
 Author-email: hello@encord.com
 Requires-Python: >=3.7,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: encord Version: 0.1.72 Summary: Encord Python SDK
+Metadata-Version: 2.1 Name: encord Version: 0.1.73 Summary: Encord Python SDK
 Client Home-page: https://github.com/encord-team/encord-client-python License:
 Apache Software License Keywords: cord,encord Author: Cord Technologies Limited
 Author-email: hello@encord.com Requires-Python: >=3.7,<4.0 Classifier: License
 :: OSI Approved :: Apache Software License Classifier: License :: Other/
 Proprietary License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.10 Classifier: Programming Language :: Python :: 3.7 Classifier:
```

