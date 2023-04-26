# Comparing `tmp/openapi_to_fastapi-0.7.0.tar.gz` & `tmp/openapi_to_fastapi-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openapi_to_fastapi-0.7.0.tar", max compression
+gzip compressed data, was "openapi_to_fastapi-0.8.0.tar", max compression
```

## Comparing `openapi_to_fastapi-0.7.0.tar` & `openapi_to_fastapi-0.8.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1519 2023-03-13 13:21:55.363878 openapi_to_fastapi-0.7.0/LICENSE
--rw-r--r--   0        0        0     7087 2023-03-13 13:21:55.363878 openapi_to_fastapi-0.7.0/README.md
--rw-r--r--   0        0        0        0 2023-03-13 13:21:55.363878 openapi_to_fastapi-0.7.0/openapi_to_fastapi/__init__.py
--rw-r--r--   0        0        0     2945 2023-03-13 13:21:55.363878 openapi_to_fastapi-0.7.0/openapi_to_fastapi/cli.py
--rw-r--r--   0        0        0       88 2023-03-13 13:21:55.363878 openapi_to_fastapi-0.7.0/openapi_to_fastapi/logger.py
--rw-r--r--   0        0        0     2922 2023-03-13 13:21:55.363878 openapi_to_fastapi-0.7.0/openapi_to_fastapi/model_generator.py
--rw-r--r--   0        0        0      394 2023-03-13 13:21:55.363878 openapi_to_fastapi-0.7.0/openapi_to_fastapi/models.py
--rw-r--r--   0        0        0     3620 2023-03-13 13:21:55.363878 openapi_to_fastapi-0.7.0/openapi_to_fastapi/parser.py
--rw-r--r--   0        0        0     6992 2023-03-13 13:21:55.363878 openapi_to_fastapi-0.7.0/openapi_to_fastapi/routes.py
--rw-r--r--   0        0        0        0 2023-03-13 13:21:55.363878 openapi_to_fastapi-0.7.0/openapi_to_fastapi/tests/__init__.py
--rw-r--r--   0        0        0      576 2023-03-13 13:21:55.363878 openapi_to_fastapi-0.7.0/openapi_to_fastapi/tests/conftest.py
--rw-r--r--   0        0        0     3863 2023-03-13 13:21:55.363878 openapi_to_fastapi-0.7.0/openapi_to_fastapi/tests/data/ihan/CompanyBasicInfo.json
--rw-r--r--   0        0        0     5201 2023-03-13 13:21:55.363878 openapi_to_fastapi-0.7.0/openapi_to_fastapi/tests/data/ihan/WeatherCurrentMetric.json
--rw-r--r--   0        0        0     3845 2023-03-13 13:21:55.363878 openapi_to_fastapi-0.7.0/openapi_to_fastapi/tests/data/pet_store/pet_store.json
--rw-r--r--   0        0        0        0 2023-03-13 13:21:55.363878 openapi_to_fastapi-0.7.0/openapi_to_fastapi/tests/snapshots/__init__.py
--rw-r--r--   0        0        0     1381 2023-03-13 13:21:55.363878 openapi_to_fastapi-0.7.0/openapi_to_fastapi/tests/snapshots/snap_test_router.py
--rw-r--r--   0        0        0     5841 2023-03-13 13:21:55.363878 openapi_to_fastapi-0.7.0/openapi_to_fastapi/tests/test_ihan_standards.py
--rw-r--r--   0        0        0     6460 2023-03-13 13:21:55.363878 openapi_to_fastapi-0.7.0/openapi_to_fastapi/tests/test_router.py
--rw-r--r--   0        0        0     1265 2023-03-13 13:21:55.363878 openapi_to_fastapi-0.7.0/openapi_to_fastapi/utils.py
--rw-r--r--   0        0        0      140 2023-03-13 13:21:55.363878 openapi_to_fastapi-0.7.0/openapi_to_fastapi/validator/__init__.py
--rw-r--r--   0        0        0     1070 2023-03-13 13:21:55.363878 openapi_to_fastapi-0.7.0/openapi_to_fastapi/validator/core.py
--rw-r--r--   0        0        0     3478 2023-03-13 13:21:55.363878 openapi_to_fastapi-0.7.0/openapi_to_fastapi/validator/ihan_standards.py
--rw-r--r--   0        0        0      934 2023-03-13 13:21:55.363878 openapi_to_fastapi-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     8038 1970-01-01 00:00:00.000000 openapi_to_fastapi-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1496 2023-04-26 13:10:57.743727 openapi_to_fastapi-0.8.0/LICENSE
+-rw-r--r--   0        0        0     7087 2023-04-26 13:10:57.743727 openapi_to_fastapi-0.8.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-26 13:10:57.743727 openapi_to_fastapi-0.8.0/openapi_to_fastapi/__init__.py
+-rw-r--r--   0        0        0     2945 2023-04-26 13:10:57.743727 openapi_to_fastapi-0.8.0/openapi_to_fastapi/cli.py
+-rw-r--r--   0        0        0       88 2023-04-26 13:10:57.743727 openapi_to_fastapi-0.8.0/openapi_to_fastapi/logger.py
+-rw-r--r--   0        0        0     2922 2023-04-26 13:10:57.743727 openapi_to_fastapi-0.8.0/openapi_to_fastapi/model_generator.py
+-rw-r--r--   0        0        0      513 2023-04-26 13:10:57.743727 openapi_to_fastapi-0.8.0/openapi_to_fastapi/models.py
+-rw-r--r--   0        0        0     3855 2023-04-26 13:10:57.743727 openapi_to_fastapi-0.8.0/openapi_to_fastapi/parser.py
+-rw-r--r--   0        0        0     7565 2023-04-26 13:10:57.743727 openapi_to_fastapi-0.8.0/openapi_to_fastapi/routes.py
+-rw-r--r--   0        0        0        0 2023-04-26 13:10:57.743727 openapi_to_fastapi-0.8.0/openapi_to_fastapi/tests/__init__.py
+-rw-r--r--   0        0        0      576 2023-04-26 13:10:57.743727 openapi_to_fastapi-0.8.0/openapi_to_fastapi/tests/conftest.py
+-rw-r--r--   0        0        0     3863 2023-04-26 13:10:57.743727 openapi_to_fastapi-0.8.0/openapi_to_fastapi/tests/data/ihan/CompanyBasicInfo.json
+-rw-r--r--   0        0        0     5201 2023-04-26 13:10:57.743727 openapi_to_fastapi-0.8.0/openapi_to_fastapi/tests/data/ihan/WeatherCurrentMetric.json
+-rw-r--r--   0        0        0     3845 2023-04-26 13:10:57.743727 openapi_to_fastapi-0.8.0/openapi_to_fastapi/tests/data/pet_store/pet_store.json
+-rw-r--r--   0        0        0        0 2023-04-26 13:10:57.743727 openapi_to_fastapi-0.8.0/openapi_to_fastapi/tests/snapshots/__init__.py
+-rw-r--r--   0        0        0     1381 2023-04-26 13:10:57.743727 openapi_to_fastapi-0.8.0/openapi_to_fastapi/tests/snapshots/snap_test_router.py
+-rw-r--r--   0        0        0     5841 2023-04-26 13:10:57.743727 openapi_to_fastapi-0.8.0/openapi_to_fastapi/tests/test_ihan_standards.py
+-rw-r--r--   0        0        0     7022 2023-04-26 13:10:57.743727 openapi_to_fastapi-0.8.0/openapi_to_fastapi/tests/test_router.py
+-rw-r--r--   0        0        0     1265 2023-04-26 13:10:57.743727 openapi_to_fastapi-0.8.0/openapi_to_fastapi/utils.py
+-rw-r--r--   0        0        0      140 2023-04-26 13:10:57.743727 openapi_to_fastapi-0.8.0/openapi_to_fastapi/validator/__init__.py
+-rw-r--r--   0        0        0     1070 2023-04-26 13:10:57.743727 openapi_to_fastapi-0.8.0/openapi_to_fastapi/validator/core.py
+-rw-r--r--   0        0        0     3478 2023-04-26 13:10:57.743727 openapi_to_fastapi-0.8.0/openapi_to_fastapi/validator/ihan_standards.py
+-rw-r--r--   0        0        0      911 2023-04-26 13:10:57.747727 openapi_to_fastapi-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     8015 1970-01-01 00:00:00.000000 openapi_to_fastapi-0.8.0/PKG-INFO
```

### Comparing `openapi_to_fastapi-0.7.0/LICENSE` & `openapi_to_fastapi-0.8.0/LICENSE`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2020, Digital Living International Ltd
+Copyright (c) 2020, IOXIO Ltd
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `openapi_to_fastapi-0.7.0/README.md` & `openapi_to_fastapi-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `openapi_to_fastapi-0.7.0/openapi_to_fastapi/cli.py` & `openapi_to_fastapi-0.8.0/openapi_to_fastapi/cli.py`

 * *Files identical despite different names*

### Comparing `openapi_to_fastapi-0.7.0/openapi_to_fastapi/model_generator.py` & `openapi_to_fastapi-0.8.0/openapi_to_fastapi/model_generator.py`

 * *Files identical despite different names*

### Comparing `openapi_to_fastapi-0.7.0/openapi_to_fastapi/parser.py` & `openapi_to_fastapi-0.8.0/openapi_to_fastapi/parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Dict, List, Optional
 
 from fastapi.openapi import models as oas
 
-from .models import Operation, PathItem
+from .models import Header, Operation, PathItem
 from .validator import MissingParameter
 
 
 def parse_parameters(spec: dict) -> List[oas.Parameter]:
     """
     Create Parameter structure from the OpenAPI spec. Loads what kind of parameters
     are used in the request and which of them are required
@@ -56,15 +56,15 @@
     :return: Operation item, if it exists
     """
 
     if not spec.get(name):
         return None
 
     data = spec[name]
-    operation = Operation(responses={}, responseModels={})
+    operation = Operation(responses={}, responseModels={}, headers={})
     operation.parameters = parse_parameters(spec[name])  # type: ignore
 
     operation.summary = data.get("summary")
     operation.description = data.get("description")
 
     request_body_model = get_model_name_from_ref(data.get("requestBody", {}))
     if request_body_model:
@@ -75,14 +75,20 @@
         if not resp_code.isdigit():
             continue
         code = int(resp_code)
         model_name = get_model_name_from_ref(resp_data)
         if model_name:
             operation.responseModels[code] = model_name
 
+    operation.headers = {
+        parameter["name"].lower(): Header(**parameter)
+        for parameter in data.get("parameters", {})
+        if "name" in parameter and parameter.get("in").lower() == "header"
+    }
+
     return operation
 
 
 def parse_openapi_spec(spec: dict) -> Dict[str, PathItem]:
     """
     Create PathItem structures from the OpenAPI spec. It contains required
     information for setting up routing
```

### Comparing `openapi_to_fastapi-0.7.0/openapi_to_fastapi/routes.py` & `openapi_to_fastapi-0.8.0/openapi_to_fastapi/routes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import json
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from pathlib import Path
 from typing import Any, Callable, Dict, List, Optional, Type, Union
 
 import pydantic
 from fastapi import APIRouter
+from fastapi.openapi import models as oas
 
 from .model_generator import load_models
 from .parser import parse_openapi_spec
 from .utils import add_annotation_to_first_argument, copy_function
 from .validator.core import BaseValidator, DefaultValidator
 
 
@@ -33,14 +34,15 @@
     response_description: str = "Successful response"
     tags: Optional[List[str]] = None
     summary: Optional[str] = None
 
     request_model: Optional[Type[pydantic.BaseModel]] = None
     response_model: Optional[Type[pydantic.BaseModel]] = None
     responses: Optional[Dict[Union[int, str], Dict[str, Any]]] = None
+    headers: Dict[str, oas.Header] = field(default_factory=dict)
     handler: Callable = dummy_route
 
     def merge_with(self, another_route: "RouteInfo"):
         for v in vars(self).keys():
             another_value = getattr(another_route, v)
             if another_value is not None:
                 setattr(self, v, another_value)
@@ -62,14 +64,28 @@
     ):
         self._validators = [DefaultValidator] + (validators or [])  # type: ignore
         self._routes = RoutesMapping(post_map={}, get_map={})
 
         self.specs_path = Path(specs_path)
         self._validate_and_parse_specs()
 
+    @property
+    def get_map(self) -> Optional[Dict[str, RouteInfo]]:
+        """
+        Get a mapping of parsed paths to route info for GET routes.
+        """
+        return self._routes.get_map
+
+    @property
+    def post_map(self) -> Optional[Dict[str, RouteInfo]]:
+        """
+        Get a mapping of parsed paths to route info for POST routes.
+        """
+        return self._routes.post_map
+
     def _validate_and_parse_specs(self):
         """
         Validate OpenAPI specs and parse required information from them
         """
         if self.specs_path.is_file():
             specs = [self.specs_path]  # for CLI usage
         else:
@@ -86,14 +102,15 @@
                 post = path_item.post
                 if post:
                     req_model = getattr(models, post.requestBodyModel, EmptyBody)
                     route_info = RouteInfo(
                         request_model=req_model,
                         description=post.description,
                         summary=path_item.post.summary,
+                        headers=path_item.post.headers,
                     )
                     if post.responseModels and post.responseModels.get(200):
                         resp_model = getattr(models, post.responseModels[200])
                         route_info.response_model = resp_model
                     self._routes.post_map[path] = route_info
 
     def get_response_model(
```

### Comparing `openapi_to_fastapi-0.7.0/openapi_to_fastapi/tests/conftest.py` & `openapi_to_fastapi-0.8.0/openapi_to_fastapi/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `openapi_to_fastapi-0.7.0/openapi_to_fastapi/tests/data/ihan/CompanyBasicInfo.json` & `openapi_to_fastapi-0.8.0/openapi_to_fastapi/tests/data/ihan/CompanyBasicInfo.json`

 * *Files identical despite different names*

### Comparing `openapi_to_fastapi-0.7.0/openapi_to_fastapi/tests/data/ihan/WeatherCurrentMetric.json` & `openapi_to_fastapi-0.8.0/openapi_to_fastapi/tests/data/ihan/WeatherCurrentMetric.json`

 * *Files identical despite different names*

### Comparing `openapi_to_fastapi-0.7.0/openapi_to_fastapi/tests/data/pet_store/pet_store.json` & `openapi_to_fastapi-0.8.0/openapi_to_fastapi/tests/data/pet_store/pet_store.json`

 * *Files identical despite different names*

### Comparing `openapi_to_fastapi-0.7.0/openapi_to_fastapi/tests/snapshots/snap_test_router.py` & `openapi_to_fastapi-0.8.0/openapi_to_fastapi/tests/snapshots/snap_test_router.py`

 * *Files identical despite different names*

### Comparing `openapi_to_fastapi-0.7.0/openapi_to_fastapi/tests/test_ihan_standards.py` & `openapi_to_fastapi-0.8.0/openapi_to_fastapi/tests/test_ihan_standards.py`

 * *Files identical despite different names*

### Comparing `openapi_to_fastapi-0.7.0/openapi_to_fastapi/tests/test_router.py` & `openapi_to_fastapi-0.8.0/openapi_to_fastapi/tests/test_router.py`

 * *Files 4% similar despite different names*

```diff
@@ -185,7 +185,21 @@
     assert route.name == "Company/BasicInfo"
     assert route.description == "Information about the company"
     assert route.summary == "Company/BasicInfo Data Product"
 
     # test that generating OpenAPI still works
     app.include_router(router)
     assert app.openapi()
+
+
+def test_headers_in_route_info_post(app, client, specs_root):
+    spec_router = SpecRouter(specs_root / "ihan")
+
+    post_map = spec_router.post_map
+    company_basic_info_headers = post_map["/Company/BasicInfo"].headers
+    assert "authorization" in company_basic_info_headers
+    assert "x-authorization-provider" in company_basic_info_headers
+
+    weather_headers = post_map["/Weather/Current/Metric"].headers
+    assert "authorization" in weather_headers
+    assert "x-authorization-provider" in weather_headers
+    assert "x-signature" in weather_headers
```

### Comparing `openapi_to_fastapi-0.7.0/openapi_to_fastapi/utils.py` & `openapi_to_fastapi-0.8.0/openapi_to_fastapi/utils.py`

 * *Files identical despite different names*

### Comparing `openapi_to_fastapi-0.7.0/openapi_to_fastapi/validator/core.py` & `openapi_to_fastapi-0.8.0/openapi_to_fastapi/validator/core.py`

 * *Files identical despite different names*

### Comparing `openapi_to_fastapi-0.7.0/openapi_to_fastapi/validator/ihan_standards.py` & `openapi_to_fastapi-0.8.0/openapi_to_fastapi/validator/ihan_standards.py`

 * *Files identical despite different names*

### Comparing `openapi_to_fastapi-0.7.0/pyproject.toml` & `openapi_to_fastapi-0.8.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "openapi-to-fastapi"
-version = "0.7.0"
+version = "0.8.0"
 description = "Create FastAPI routes from OpenAPI spec"
-authors = ["Digital Living International Ltd"]
+authors = ["IOXIO Ltd"]
 license = "BSD-3-Clause"
 readme = "README.md"
 repository = "https://github.com/ioxiocom/openapi-to-fastapi"
 packages = [
     {include="openapi_to_fastapi", from="."}
 ]
```

### Comparing `openapi_to_fastapi-0.7.0/PKG-INFO` & `openapi_to_fastapi-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: openapi-to-fastapi
-Version: 0.7.0
+Version: 0.8.0
 Summary: Create FastAPI routes from OpenAPI spec
 Home-page: https://github.com/ioxiocom/openapi-to-fastapi
 License: BSD-3-Clause
-Author: Digital Living International Ltd
+Author: IOXIO Ltd
 Requires-Python: >=3.7,<4.0.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

