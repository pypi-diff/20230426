# Comparing `tmp/vellum_ai-0.0.3.tar.gz` & `tmp/vellum_ai-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vellum_ai-0.0.3.tar", max compression
+gzip compressed data, was "vellum_ai-0.0.5.tar", max compression
```

## Comparing `vellum_ai-0.0.3.tar` & `vellum_ai-0.0.5.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0      413 2023-04-22 04:52:43.354088 vellum_ai-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2619 2023-04-22 04:52:43.354088 vellum_ai-0.0.3/src/vellum/__init__.py
--rw-r--r--   0        0        0     8595 2023-04-22 04:52:43.354088 vellum_ai-0.0.3/src/vellum/client.py
--rw-r--r--   0        0        0      348 2023-04-22 04:52:43.354088 vellum_ai-0.0.3/src/vellum/core/__init__.py
--rw-r--r--   0        0        0      426 2023-04-22 04:52:43.354088 vellum_ai-0.0.3/src/vellum/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-04-22 04:52:43.354088 vellum_ai-0.0.3/src/vellum/core/datetime_utils.py
--rw-r--r--   0        0        0     3507 2023-04-22 04:52:43.354088 vellum_ai-0.0.3/src/vellum/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-04-22 04:52:43.354088 vellum_ai-0.0.3/src/vellum/core/remove_none_from_headers.py
--rw-r--r--   0        0        0      498 2023-04-22 04:52:43.354088 vellum_ai-0.0.3/src/vellum/environment.py
--rw-r--r--   0        0        0        0 2023-04-22 04:52:43.354088 vellum_ai-0.0.3/src/vellum/py.typed
--rw-r--r--   0        0        0      148 2023-04-22 04:52:43.354088 vellum_ai-0.0.3/src/vellum/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-04-22 04:52:43.354088 vellum_ai-0.0.3/src/vellum/resources/documents/__init__.py
--rw-r--r--   0        0        0     5513 2023-04-22 04:52:43.354088 vellum_ai-0.0.3/src/vellum/resources/documents/client.py
--rw-r--r--   0        0        0       65 2023-04-22 04:52:43.354088 vellum_ai-0.0.3/src/vellum/resources/model_versions/__init__.py
--rw-r--r--   0        0        0     2226 2023-04-22 04:52:43.354088 vellum_ai-0.0.3/src/vellum/resources/model_versions/client.py
--rw-r--r--   0        0        0     3803 2023-04-22 04:52:43.354088 vellum_ai-0.0.3/src/vellum/types/__init__.py
--rw-r--r--   0        0        0      830 2023-04-22 04:52:43.354088 vellum_ai-0.0.3/src/vellum/types/block_type_enum.py
--rw-r--r--   0        0        0      633 2023-04-22 04:52:43.354088 vellum_ai-0.0.3/src/vellum/types/chat_role_enum.py
--rw-r--r--   0        0        0     1117 2023-04-22 04:52:43.354088 vellum_ai-0.0.3/src/vellum/types/document.py
--rw-r--r--   0        0        0     1268 2023-04-22 04:52:43.354088 vellum_ai-0.0.3/src/vellum/types/document_document_to_document_index.py
--rw-r--r--   0        0        0     1714 2023-04-22 04:52:43.354088 vellum_ai-0.0.3/src/vellum/types/enriched_normalized_completion.py
--rw-r--r--   0        0        0      639 2023-04-22 04:52:43.354088 vellum_ai-0.0.3/src/vellum/types/finish_reason_enum.py
--rw-r--r--   0        0        0      831 2023-04-22 04:52:43.354088 vellum_ai-0.0.3/src/vellum/types/generate_error_response.py
--rw-r--r--   0        0        0      929 2023-04-22 04:52:43.354088 vellum_ai-0.0.3/src/vellum/types/generate_options_request.py
--rw-r--r--   0        0        0     1186 2023-04-22 04:52:43.354088 vellum_ai-0.0.3/src/vellum/types/generate_request.py
--rw-r--r--   0        0        0     1246 2023-04-22 04:52:43.354088 vellum_ai-0.0.3/src/vellum/types/generate_response.py
--rw-r--r--   0        0        0     1326 2023-04-22 04:52:43.354088 vellum_ai-0.0.3/src/vellum/types/generate_result.py
--rw-r--r--   0        0        0      992 2023-04-22 04:52:43.354088 vellum_ai-0.0.3/src/vellum/types/generate_result_data.py
--rw-r--r--   0        0        0      840 2023-04-22 04:52:43.354088 vellum_ai-0.0.3/src/vellum/types/generate_result_error.py
--rw-r--r--   0        0        0     1012 2023-04-22 04:52:43.354088 vellum_ai-0.0.3/src/vellum/types/indexing_state_enum.py
--rw-r--r--   0        0        0      435 2023-04-22 04:52:43.354088 vellum_ai-0.0.3/src/vellum/types/logprobs_enum.py
--rw-r--r--   0        0        0      483 2023-04-22 04:52:43.354088 vellum_ai-0.0.3/src/vellum/types/model_type_enum.py
--rw-r--r--   0        0        0     1241 2023-04-22 04:52:43.354088 vellum_ai-0.0.3/src/vellum/types/model_version_build_config.py
--rw-r--r--   0        0        0     1004 2023-04-22 04:52:43.354088 vellum_ai-0.0.3/src/vellum/types/model_version_exec_config_parameters.py
--rw-r--r--   0        0        0     1421 2023-04-22 04:52:43.354088 vellum_ai-0.0.3/src/vellum/types/model_version_exec_config_read.py
--rw-r--r--   0        0        0     2056 2023-04-22 04:52:43.354088 vellum_ai-0.0.3/src/vellum/types/model_version_read.py
--rw-r--r--   0        0        0      895 2023-04-22 04:52:43.358088 vellum_ai-0.0.3/src/vellum/types/model_version_read_status_enum.py
--rw-r--r--   0        0        0      934 2023-04-22 04:52:43.358088 vellum_ai-0.0.3/src/vellum/types/model_version_sandbox_snapshot.py
--rw-r--r--   0        0        0      873 2023-04-22 04:52:43.358088 vellum_ai-0.0.3/src/vellum/types/normalized_log_probs.py
--rw-r--r--   0        0        0      840 2023-04-22 04:52:43.358088 vellum_ai-0.0.3/src/vellum/types/normalized_token_log_probs.py
--rw-r--r--   0        0        0      939 2023-04-22 04:52:43.358088 vellum_ai-0.0.3/src/vellum/types/paginated_slim_document_list.py
--rw-r--r--   0        0        0      835 2023-04-22 04:52:43.358088 vellum_ai-0.0.3/src/vellum/types/processing_state_enum.py
--rw-r--r--   0        0        0      934 2023-04-22 04:52:43.358088 vellum_ai-0.0.3/src/vellum/types/prompt_template_block.py
--rw-r--r--   0        0        0      860 2023-04-22 04:52:43.358088 vellum_ai-0.0.3/src/vellum/types/prompt_template_block_data.py
--rw-r--r--   0        0        0      977 2023-04-22 04:52:43.358088 vellum_ai-0.0.3/src/vellum/types/prompt_template_block_properties.py
--rw-r--r--   0        0        0     1039 2023-04-22 04:52:43.358088 vellum_ai-0.0.3/src/vellum/types/provider_enum.py
--rw-r--r--   0        0        0      829 2023-04-22 04:52:43.358088 vellum_ai-0.0.3/src/vellum/types/search_error_response.py
--rw-r--r--   0        0        0      881 2023-04-22 04:52:43.358088 vellum_ai-0.0.3/src/vellum/types/search_filters_request.py
--rw-r--r--   0        0        0     1486 2023-04-22 04:52:43.358088 vellum_ai-0.0.3/src/vellum/types/search_request_options_request.py
--rw-r--r--   0        0        0      952 2023-04-22 04:52:43.358088 vellum_ai-0.0.3/src/vellum/types/search_response.py
--rw-r--r--   0        0        0     1157 2023-04-22 04:52:43.358088 vellum_ai-0.0.3/src/vellum/types/search_result.py
--rw-r--r--   0        0        0      834 2023-04-22 04:52:43.358088 vellum_ai-0.0.3/src/vellum/types/search_result_merging_request.py
--rw-r--r--   0        0        0      961 2023-04-22 04:52:43.358088 vellum_ai-0.0.3/src/vellum/types/search_weights_request.py
--rw-r--r--   0        0        0     2009 2023-04-22 04:52:43.358088 vellum_ai-0.0.3/src/vellum/types/slim_document.py
--rw-r--r--   0        0        0      351 2023-04-22 04:52:43.358088 vellum_ai-0.0.3/src/vellum/types/slim_document_status_enum.py
--rw-r--r--   0        0        0     1778 2023-04-22 04:52:43.358088 vellum_ai-0.0.3/src/vellum/types/submit_completion_actual_request.py
--rw-r--r--   0        0        0      772 2023-04-22 04:52:43.358088 vellum_ai-0.0.3/src/vellum/types/submit_completion_actuals_error_response.py
--rw-r--r--   0        0        0      763 2023-04-22 04:52:43.358088 vellum_ai-0.0.3/src/vellum/types/upload_document_error_response.py
--rw-r--r--   0        0        0      837 2023-04-22 04:52:43.358088 vellum_ai-0.0.3/src/vellum/types/upload_document_response.py
--rw-r--r--   0        0        0      556 1970-01-01 00:00:00.000000 vellum_ai-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      413 2023-04-26 01:08:16.267506 vellum_ai-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2619 2023-04-26 01:08:16.267506 vellum_ai-0.0.5/src/vellum/__init__.py
+-rw-r--r--   0        0        0     8763 2023-04-26 01:08:16.267506 vellum_ai-0.0.5/src/vellum/client.py
+-rw-r--r--   0        0        0      348 2023-04-26 01:08:16.267506 vellum_ai-0.0.5/src/vellum/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-04-26 01:08:16.267506 vellum_ai-0.0.5/src/vellum/core/api_error.py
+-rw-r--r--   0        0        0     1047 2023-04-26 01:08:16.267506 vellum_ai-0.0.5/src/vellum/core/datetime_utils.py
+-rw-r--r--   0        0        0     3507 2023-04-26 01:08:16.267506 vellum_ai-0.0.5/src/vellum/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-04-26 01:08:16.267506 vellum_ai-0.0.5/src/vellum/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      498 2023-04-26 01:08:16.267506 vellum_ai-0.0.5/src/vellum/environment.py
+-rw-r--r--   0        0        0        0 2023-04-26 01:08:16.267506 vellum_ai-0.0.5/src/vellum/py.typed
+-rw-r--r--   0        0        0      148 2023-04-26 01:08:16.267506 vellum_ai-0.0.5/src/vellum/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-04-26 01:08:16.267506 vellum_ai-0.0.5/src/vellum/resources/documents/__init__.py
+-rw-r--r--   0        0        0     5625 2023-04-26 01:08:16.267506 vellum_ai-0.0.5/src/vellum/resources/documents/client.py
+-rw-r--r--   0        0        0       65 2023-04-26 01:08:16.267506 vellum_ai-0.0.5/src/vellum/resources/model_versions/__init__.py
+-rw-r--r--   0        0        0     2282 2023-04-26 01:08:16.267506 vellum_ai-0.0.5/src/vellum/resources/model_versions/client.py
+-rw-r--r--   0        0        0     3803 2023-04-26 01:08:16.267506 vellum_ai-0.0.5/src/vellum/types/__init__.py
+-rw-r--r--   0        0        0      830 2023-04-26 01:08:16.267506 vellum_ai-0.0.5/src/vellum/types/block_type_enum.py
+-rw-r--r--   0        0        0      633 2023-04-26 01:08:16.267506 vellum_ai-0.0.5/src/vellum/types/chat_role_enum.py
+-rw-r--r--   0        0        0     1117 2023-04-26 01:08:16.267506 vellum_ai-0.0.5/src/vellum/types/document.py
+-rw-r--r--   0        0        0     1268 2023-04-26 01:08:16.267506 vellum_ai-0.0.5/src/vellum/types/document_document_to_document_index.py
+-rw-r--r--   0        0        0     1714 2023-04-26 01:08:16.267506 vellum_ai-0.0.5/src/vellum/types/enriched_normalized_completion.py
+-rw-r--r--   0        0        0      639 2023-04-26 01:08:16.267506 vellum_ai-0.0.5/src/vellum/types/finish_reason_enum.py
+-rw-r--r--   0        0        0      831 2023-04-26 01:08:16.271506 vellum_ai-0.0.5/src/vellum/types/generate_error_response.py
+-rw-r--r--   0        0        0      929 2023-04-26 01:08:16.271506 vellum_ai-0.0.5/src/vellum/types/generate_options_request.py
+-rw-r--r--   0        0        0     1186 2023-04-26 01:08:16.271506 vellum_ai-0.0.5/src/vellum/types/generate_request.py
+-rw-r--r--   0        0        0     1246 2023-04-26 01:08:16.271506 vellum_ai-0.0.5/src/vellum/types/generate_response.py
+-rw-r--r--   0        0        0     1326 2023-04-26 01:08:16.271506 vellum_ai-0.0.5/src/vellum/types/generate_result.py
+-rw-r--r--   0        0        0      992 2023-04-26 01:08:16.271506 vellum_ai-0.0.5/src/vellum/types/generate_result_data.py
+-rw-r--r--   0        0        0      840 2023-04-26 01:08:16.271506 vellum_ai-0.0.5/src/vellum/types/generate_result_error.py
+-rw-r--r--   0        0        0     1012 2023-04-26 01:08:16.271506 vellum_ai-0.0.5/src/vellum/types/indexing_state_enum.py
+-rw-r--r--   0        0        0      435 2023-04-26 01:08:16.271506 vellum_ai-0.0.5/src/vellum/types/logprobs_enum.py
+-rw-r--r--   0        0        0      483 2023-04-26 01:08:16.271506 vellum_ai-0.0.5/src/vellum/types/model_type_enum.py
+-rw-r--r--   0        0        0     1241 2023-04-26 01:08:16.271506 vellum_ai-0.0.5/src/vellum/types/model_version_build_config.py
+-rw-r--r--   0        0        0     1004 2023-04-26 01:08:16.271506 vellum_ai-0.0.5/src/vellum/types/model_version_exec_config_parameters.py
+-rw-r--r--   0        0        0     1421 2023-04-26 01:08:16.271506 vellum_ai-0.0.5/src/vellum/types/model_version_exec_config_read.py
+-rw-r--r--   0        0        0     2056 2023-04-26 01:08:16.271506 vellum_ai-0.0.5/src/vellum/types/model_version_read.py
+-rw-r--r--   0        0        0      895 2023-04-26 01:08:16.271506 vellum_ai-0.0.5/src/vellum/types/model_version_read_status_enum.py
+-rw-r--r--   0        0        0      934 2023-04-26 01:08:16.271506 vellum_ai-0.0.5/src/vellum/types/model_version_sandbox_snapshot.py
+-rw-r--r--   0        0        0      873 2023-04-26 01:08:16.271506 vellum_ai-0.0.5/src/vellum/types/normalized_log_probs.py
+-rw-r--r--   0        0        0      840 2023-04-26 01:08:16.271506 vellum_ai-0.0.5/src/vellum/types/normalized_token_log_probs.py
+-rw-r--r--   0        0        0      939 2023-04-26 01:08:16.271506 vellum_ai-0.0.5/src/vellum/types/paginated_slim_document_list.py
+-rw-r--r--   0        0        0      835 2023-04-26 01:08:16.271506 vellum_ai-0.0.5/src/vellum/types/processing_state_enum.py
+-rw-r--r--   0        0        0      934 2023-04-26 01:08:16.271506 vellum_ai-0.0.5/src/vellum/types/prompt_template_block.py
+-rw-r--r--   0        0        0      860 2023-04-26 01:08:16.271506 vellum_ai-0.0.5/src/vellum/types/prompt_template_block_data.py
+-rw-r--r--   0        0        0      977 2023-04-26 01:08:16.271506 vellum_ai-0.0.5/src/vellum/types/prompt_template_block_properties.py
+-rw-r--r--   0        0        0     1039 2023-04-26 01:08:16.271506 vellum_ai-0.0.5/src/vellum/types/provider_enum.py
+-rw-r--r--   0        0        0      829 2023-04-26 01:08:16.271506 vellum_ai-0.0.5/src/vellum/types/search_error_response.py
+-rw-r--r--   0        0        0      881 2023-04-26 01:08:16.271506 vellum_ai-0.0.5/src/vellum/types/search_filters_request.py
+-rw-r--r--   0        0        0     1486 2023-04-26 01:08:16.271506 vellum_ai-0.0.5/src/vellum/types/search_request_options_request.py
+-rw-r--r--   0        0        0      952 2023-04-26 01:08:16.271506 vellum_ai-0.0.5/src/vellum/types/search_response.py
+-rw-r--r--   0        0        0     1157 2023-04-26 01:08:16.271506 vellum_ai-0.0.5/src/vellum/types/search_result.py
+-rw-r--r--   0        0        0      834 2023-04-26 01:08:16.271506 vellum_ai-0.0.5/src/vellum/types/search_result_merging_request.py
+-rw-r--r--   0        0        0      961 2023-04-26 01:08:16.271506 vellum_ai-0.0.5/src/vellum/types/search_weights_request.py
+-rw-r--r--   0        0        0     2009 2023-04-26 01:08:16.271506 vellum_ai-0.0.5/src/vellum/types/slim_document.py
+-rw-r--r--   0        0        0      351 2023-04-26 01:08:16.271506 vellum_ai-0.0.5/src/vellum/types/slim_document_status_enum.py
+-rw-r--r--   0        0        0     1778 2023-04-26 01:08:16.271506 vellum_ai-0.0.5/src/vellum/types/submit_completion_actual_request.py
+-rw-r--r--   0        0        0      772 2023-04-26 01:08:16.271506 vellum_ai-0.0.5/src/vellum/types/submit_completion_actuals_error_response.py
+-rw-r--r--   0        0        0      763 2023-04-26 01:08:16.271506 vellum_ai-0.0.5/src/vellum/types/upload_document_error_response.py
+-rw-r--r--   0        0        0      837 2023-04-26 01:08:16.271506 vellum_ai-0.0.5/src/vellum/types/upload_document_response.py
+-rw-r--r--   0        0        0      556 1970-01-01 00:00:00.000000 vellum_ai-0.0.5/PKG-INFO
```

### Comparing `vellum_ai-0.0.3/src/vellum/__init__.py` & `vellum_ai-0.0.5/src/vellum/__init__.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.3/src/vellum/client.py` & `vellum_ai-0.0.5/src/vellum/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,15 @@
                     "deployment_id": deployment_id,
                     "deployment_name": deployment_name,
                     "requests": requests,
                     "options": options,
                 }
             ),
             headers=remove_none_from_headers({"X_API_KEY": self.api_key}),
+            timeout=None,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(GenerateResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
@@ -65,14 +66,15 @@
         options: typing.Optional[SearchRequestOptionsRequest] = None,
     ) -> SearchResponse:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.predict}/", "v1/search"),
             json=jsonable_encoder({"index_id": index_id, "index_name": index_name, "query": query, "options": options}),
             headers=remove_none_from_headers({"X_API_KEY": self.api_key}),
+            timeout=None,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(SearchResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
@@ -88,14 +90,15 @@
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.predict}/", "v1/submit-completion-actuals"),
             json=jsonable_encoder(
                 {"deployment_id": deployment_id, "deployment_name": deployment_name, "actuals": actuals}
             ),
             headers=remove_none_from_headers({"X_API_KEY": self.api_key}),
+            timeout=None,
         )
         if 200 <= _response.status_code < 300:
             return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
@@ -132,14 +135,15 @@
                         "deployment_id": deployment_id,
                         "deployment_name": deployment_name,
                         "requests": requests,
                         "options": options,
                     }
                 ),
                 headers=remove_none_from_headers({"X_API_KEY": self.api_key}),
+                timeout=None,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(GenerateResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
@@ -157,14 +161,15 @@
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.predict}/", "v1/search"),
                 json=jsonable_encoder(
                     {"index_id": index_id, "index_name": index_name, "query": query, "options": options}
                 ),
                 headers=remove_none_from_headers({"X_API_KEY": self.api_key}),
+                timeout=None,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(SearchResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
@@ -181,14 +186,15 @@
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.predict}/", "v1/submit-completion-actuals"),
                 json=jsonable_encoder(
                     {"deployment_id": deployment_id, "deployment_name": deployment_name, "actuals": actuals}
                 ),
                 headers=remove_none_from_headers({"X_API_KEY": self.api_key}),
+                timeout=None,
             )
         if 200 <= _response.status_code < 300:
             return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
```

### Comparing `vellum_ai-0.0.3/src/vellum/core/datetime_utils.py` & `vellum_ai-0.0.5/src/vellum/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.3/src/vellum/core/jsonable_encoder.py` & `vellum_ai-0.0.5/src/vellum/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.3/src/vellum/resources/documents/client.py` & `vellum_ai-0.0.5/src/vellum/resources/documents/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,14 +29,15 @@
         ordering: typing.Optional[str] = None,
     ) -> PaginatedSlimDocumentList:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.default}/", "v1/documents"),
             params={"document_index_id": document_index_id, "limit": limit, "offset": offset, "ordering": ordering},
             headers=remove_none_from_headers({"X_API_KEY": self.api_key}),
+            timeout=None,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedSlimDocumentList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
@@ -60,14 +61,15 @@
                     "external_id": external_id,
                     "label": label,
                     "keywords": keywords,
                 }
             ),
             files={"contents": contents},
             headers=remove_none_from_headers({"X_API_KEY": self.api_key}),
+            timeout=None,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(UploadDocumentResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
@@ -89,14 +91,15 @@
     ) -> PaginatedSlimDocumentList:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.default}/", "v1/documents"),
                 params={"document_index_id": document_index_id, "limit": limit, "offset": offset, "ordering": ordering},
                 headers=remove_none_from_headers({"X_API_KEY": self.api_key}),
+                timeout=None,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedSlimDocumentList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
@@ -121,14 +124,15 @@
                         "external_id": external_id,
                         "label": label,
                         "keywords": keywords,
                     }
                 ),
                 files={"contents": contents},
                 headers=remove_none_from_headers({"X_API_KEY": self.api_key}),
+                timeout=None,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(UploadDocumentResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
```

### Comparing `vellum_ai-0.0.3/src/vellum/resources/model_versions/client.py` & `vellum_ai-0.0.5/src/vellum/resources/model_versions/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,15 @@
         self.api_key = api_key
 
     def retrieve(self, id: str) -> ModelVersionRead:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.default}/", f"v1/model-versions/{id}"),
             headers=remove_none_from_headers({"X_API_KEY": self.api_key}),
+            timeout=None,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ModelVersionRead, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
@@ -39,14 +40,15 @@
 
     async def retrieve(self, id: str) -> ModelVersionRead:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.default}/", f"v1/model-versions/{id}"),
                 headers=remove_none_from_headers({"X_API_KEY": self.api_key}),
+                timeout=None,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ModelVersionRead, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
```

### Comparing `vellum_ai-0.0.3/src/vellum/types/__init__.py` & `vellum_ai-0.0.5/src/vellum/types/__init__.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.3/src/vellum/types/block_type_enum.py` & `vellum_ai-0.0.5/src/vellum/types/block_type_enum.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.3/src/vellum/types/chat_role_enum.py` & `vellum_ai-0.0.5/src/vellum/types/chat_role_enum.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.3/src/vellum/types/document.py` & `vellum_ai-0.0.5/src/vellum/types/document.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.3/src/vellum/types/document_document_to_document_index.py` & `vellum_ai-0.0.5/src/vellum/types/document_document_to_document_index.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.3/src/vellum/types/enriched_normalized_completion.py` & `vellum_ai-0.0.5/src/vellum/types/enriched_normalized_completion.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.3/src/vellum/types/finish_reason_enum.py` & `vellum_ai-0.0.5/src/vellum/types/finish_reason_enum.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.3/src/vellum/types/generate_error_response.py` & `vellum_ai-0.0.5/src/vellum/types/generate_error_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.3/src/vellum/types/generate_options_request.py` & `vellum_ai-0.0.5/src/vellum/types/generate_options_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.3/src/vellum/types/generate_request.py` & `vellum_ai-0.0.5/src/vellum/types/generate_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.3/src/vellum/types/generate_response.py` & `vellum_ai-0.0.5/src/vellum/types/generate_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.3/src/vellum/types/generate_result.py` & `vellum_ai-0.0.5/src/vellum/types/generate_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.3/src/vellum/types/generate_result_data.py` & `vellum_ai-0.0.5/src/vellum/types/generate_result_data.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.3/src/vellum/types/generate_result_error.py` & `vellum_ai-0.0.5/src/vellum/types/generate_result_error.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.3/src/vellum/types/indexing_state_enum.py` & `vellum_ai-0.0.5/src/vellum/types/indexing_state_enum.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.3/src/vellum/types/model_version_build_config.py` & `vellum_ai-0.0.5/src/vellum/types/model_version_build_config.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.3/src/vellum/types/model_version_exec_config_parameters.py` & `vellum_ai-0.0.5/src/vellum/types/model_version_exec_config_parameters.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.3/src/vellum/types/model_version_exec_config_read.py` & `vellum_ai-0.0.5/src/vellum/types/model_version_exec_config_read.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.3/src/vellum/types/model_version_read.py` & `vellum_ai-0.0.5/src/vellum/types/model_version_read.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.3/src/vellum/types/model_version_read_status_enum.py` & `vellum_ai-0.0.5/src/vellum/types/model_version_read_status_enum.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.3/src/vellum/types/model_version_sandbox_snapshot.py` & `vellum_ai-0.0.5/src/vellum/types/model_version_sandbox_snapshot.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.3/src/vellum/types/normalized_log_probs.py` & `vellum_ai-0.0.5/src/vellum/types/normalized_log_probs.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.3/src/vellum/types/normalized_token_log_probs.py` & `vellum_ai-0.0.5/src/vellum/types/normalized_token_log_probs.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.3/src/vellum/types/paginated_slim_document_list.py` & `vellum_ai-0.0.5/src/vellum/types/paginated_slim_document_list.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.3/src/vellum/types/processing_state_enum.py` & `vellum_ai-0.0.5/src/vellum/types/processing_state_enum.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.3/src/vellum/types/prompt_template_block.py` & `vellum_ai-0.0.5/src/vellum/types/prompt_template_block.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.3/src/vellum/types/prompt_template_block_data.py` & `vellum_ai-0.0.5/src/vellum/types/prompt_template_block_data.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.3/src/vellum/types/prompt_template_block_properties.py` & `vellum_ai-0.0.5/src/vellum/types/prompt_template_block_properties.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.3/src/vellum/types/provider_enum.py` & `vellum_ai-0.0.5/src/vellum/types/provider_enum.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.3/src/vellum/types/search_error_response.py` & `vellum_ai-0.0.5/src/vellum/types/search_error_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.3/src/vellum/types/search_filters_request.py` & `vellum_ai-0.0.5/src/vellum/types/search_filters_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.3/src/vellum/types/search_request_options_request.py` & `vellum_ai-0.0.5/src/vellum/types/search_request_options_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.3/src/vellum/types/search_response.py` & `vellum_ai-0.0.5/src/vellum/types/search_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.3/src/vellum/types/search_result.py` & `vellum_ai-0.0.5/src/vellum/types/search_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.3/src/vellum/types/search_result_merging_request.py` & `vellum_ai-0.0.5/src/vellum/types/search_result_merging_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.3/src/vellum/types/search_weights_request.py` & `vellum_ai-0.0.5/src/vellum/types/search_weights_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.3/src/vellum/types/slim_document.py` & `vellum_ai-0.0.5/src/vellum/types/slim_document.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.3/src/vellum/types/submit_completion_actual_request.py` & `vellum_ai-0.0.5/src/vellum/types/submit_completion_actual_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.3/src/vellum/types/submit_completion_actuals_error_response.py` & `vellum_ai-0.0.5/src/vellum/types/submit_completion_actuals_error_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.3/src/vellum/types/upload_document_error_response.py` & `vellum_ai-0.0.5/src/vellum/types/upload_document_error_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.3/src/vellum/types/upload_document_response.py` & `vellum_ai-0.0.5/src/vellum/types/upload_document_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.3/PKG-INFO` & `vellum_ai-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vellum-ai
-Version: 0.0.3
+Version: 0.0.5
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

