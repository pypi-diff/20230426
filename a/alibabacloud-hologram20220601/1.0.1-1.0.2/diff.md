# Comparing `tmp/alibabacloud_hologram20220601-1.0.1.tar.gz` & `tmp/alibabacloud_hologram20220601-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_hologram20220601-1.0.1.tar", last modified: Wed Apr 19 07:17:57 2023, max compression
+gzip compressed data, was "dist/alibabacloud_hologram20220601-1.0.2.tar", last modified: Wed Apr 26 09:32:29 2023, max compression
```

## Comparing `alibabacloud_hologram20220601-1.0.1.tar` & `alibabacloud_hologram20220601-1.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 07:17:57.000000 alibabacloud_hologram20220601-1.0.1/
--rw-r--r--   0 root         (0) root         (0)       46 2023-04-19 07:17:57.000000 alibabacloud_hologram20220601-1.0.1/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-04-19 07:17:57.000000 alibabacloud_hologram20220601-1.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-04-19 07:17:57.000000 alibabacloud_hologram20220601-1.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2358 2023-04-19 07:17:57.000000 alibabacloud_hologram20220601-1.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1037 2023-04-19 07:17:57.000000 alibabacloud_hologram20220601-1.0.1/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1122 2023-04-19 07:17:57.000000 alibabacloud_hologram20220601-1.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 07:17:57.000000 alibabacloud_hologram20220601-1.0.1/alibabacloud_hologram20220601/
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-19 07:17:57.000000 alibabacloud_hologram20220601-1.0.1/alibabacloud_hologram20220601/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25012 2023-04-19 07:17:57.000000 alibabacloud_hologram20220601-1.0.1/alibabacloud_hologram20220601/client.py
--rw-r--r--   0 root         (0) root         (0)    49882 2023-04-19 07:17:57.000000 alibabacloud_hologram20220601-1.0.1/alibabacloud_hologram20220601/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 07:17:57.000000 alibabacloud_hologram20220601-1.0.1/alibabacloud_hologram20220601.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2358 2023-04-19 07:17:57.000000 alibabacloud_hologram20220601-1.0.1/alibabacloud_hologram20220601.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      460 2023-04-19 07:17:57.000000 alibabacloud_hologram20220601-1.0.1/alibabacloud_hologram20220601.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 07:17:57.000000 alibabacloud_hologram20220601-1.0.1/alibabacloud_hologram20220601.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-04-19 07:17:57.000000 alibabacloud_hologram20220601-1.0.1/alibabacloud_hologram20220601.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2023-04-19 07:17:57.000000 alibabacloud_hologram20220601-1.0.1/alibabacloud_hologram20220601.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-04-19 07:17:57.000000 alibabacloud_hologram20220601-1.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2635 2023-04-19 07:17:57.000000 alibabacloud_hologram20220601-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:32:29.000000 alibabacloud_hologram20220601-1.0.2/
+-rw-r--r--   0 root         (0) root         (0)       92 2023-04-26 09:32:28.000000 alibabacloud_hologram20220601-1.0.2/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-04-26 09:32:28.000000 alibabacloud_hologram20220601-1.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-26 09:32:28.000000 alibabacloud_hologram20220601-1.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2358 2023-04-26 09:32:29.000000 alibabacloud_hologram20220601-1.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1037 2023-04-26 09:32:28.000000 alibabacloud_hologram20220601-1.0.2/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1122 2023-04-26 09:32:28.000000 alibabacloud_hologram20220601-1.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:32:29.000000 alibabacloud_hologram20220601-1.0.2/alibabacloud_hologram20220601/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-26 09:32:28.000000 alibabacloud_hologram20220601-1.0.2/alibabacloud_hologram20220601/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21836 2023-04-26 09:32:28.000000 alibabacloud_hologram20220601-1.0.2/alibabacloud_hologram20220601/client.py
+-rw-r--r--   0 root         (0) root         (0)    47357 2023-04-26 09:32:28.000000 alibabacloud_hologram20220601-1.0.2/alibabacloud_hologram20220601/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:32:29.000000 alibabacloud_hologram20220601-1.0.2/alibabacloud_hologram20220601.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2358 2023-04-26 09:32:29.000000 alibabacloud_hologram20220601-1.0.2/alibabacloud_hologram20220601.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      460 2023-04-26 09:32:29.000000 alibabacloud_hologram20220601-1.0.2/alibabacloud_hologram20220601.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 09:32:29.000000 alibabacloud_hologram20220601-1.0.2/alibabacloud_hologram20220601.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-04-26 09:32:29.000000 alibabacloud_hologram20220601-1.0.2/alibabacloud_hologram20220601.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2023-04-26 09:32:29.000000 alibabacloud_hologram20220601-1.0.2/alibabacloud_hologram20220601.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-26 09:32:29.000000 alibabacloud_hologram20220601-1.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2635 2023-04-26 09:32:28.000000 alibabacloud_hologram20220601-1.0.2/setup.py
```

### Comparing `alibabacloud_hologram20220601-1.0.1/LICENSE` & `alibabacloud_hologram20220601-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_hologram20220601-1.0.1/PKG-INFO` & `alibabacloud_hologram20220601-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_hologram20220601
-Version: 1.0.1
+Version: 1.0.2
 Summary: Alibaba Cloud Hologres (20220601) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_hologram20220601-1.0.1/README-CN.md` & `alibabacloud_hologram20220601-1.0.2/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_hologram20220601-1.0.1/README.md` & `alibabacloud_hologram20220601-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_hologram20220601-1.0.1/alibabacloud_hologram20220601/client.py` & `alibabacloud_hologram20220601-1.0.2/alibabacloud_hologram20220601/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -124,25 +124,21 @@
     def list_instances_with_options(
         self,
         request: hologram_20220601_models.ListInstancesRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> hologram_20220601_models.ListInstancesResponse:
         UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
         body = {}
         if not UtilClient.is_unset(request.resource_group_id):
             body['resourceGroupId'] = request.resource_group_id
         if not UtilClient.is_unset(request.tag):
             body['tag'] = request.tag
         req = open_api_models.OpenApiRequest(
             headers=headers,
-            query=OpenApiUtilClient.query(query),
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='ListInstances',
             version='2022-06-01',
             protocol='HTTPS',
             pathname=f'/api/v1/instances',
@@ -160,25 +156,21 @@
     async def list_instances_with_options_async(
         self,
         request: hologram_20220601_models.ListInstancesRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> hologram_20220601_models.ListInstancesResponse:
         UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
         body = {}
         if not UtilClient.is_unset(request.resource_group_id):
             body['resourceGroupId'] = request.resource_group_id
         if not UtilClient.is_unset(request.tag):
             body['tag'] = request.tag
         req = open_api_models.OpenApiRequest(
             headers=headers,
-            query=OpenApiUtilClient.query(query),
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='ListInstances',
             version='2022-06-01',
             protocol='HTTPS',
             pathname=f'/api/v1/instances',
@@ -208,25 +200,19 @@
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.list_instances_with_options_async(request, headers, runtime)
 
     def restart_instance_with_options(
         self,
         instance_id: str,
-        request: hologram_20220601_models.RestartInstanceRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> hologram_20220601_models.RestartInstanceResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
-            headers=headers,
-            query=OpenApiUtilClient.query(query)
+            headers=headers
         )
         params = open_api_models.Params(
             action='RestartInstance',
             version='2022-06-01',
             protocol='HTTPS',
             pathname=f'/api/v1/instances/{OpenApiUtilClient.get_encode_param(instance_id)}/restart',
             method='POST',
@@ -239,25 +225,19 @@
             hologram_20220601_models.RestartInstanceResponse(),
             self.call_api(params, req, runtime)
         )
 
     async def restart_instance_with_options_async(
         self,
         instance_id: str,
-        request: hologram_20220601_models.RestartInstanceRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> hologram_20220601_models.RestartInstanceResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
-            headers=headers,
-            query=OpenApiUtilClient.query(query)
+            headers=headers
         )
         params = open_api_models.Params(
             action='RestartInstance',
             version='2022-06-01',
             protocol='HTTPS',
             pathname=f'/api/v1/instances/{OpenApiUtilClient.get_encode_param(instance_id)}/restart',
             method='POST',
@@ -270,43 +250,35 @@
             hologram_20220601_models.RestartInstanceResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
     def restart_instance(
         self,
         instance_id: str,
-        request: hologram_20220601_models.RestartInstanceRequest,
     ) -> hologram_20220601_models.RestartInstanceResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.restart_instance_with_options(instance_id, request, headers, runtime)
+        return self.restart_instance_with_options(instance_id, headers, runtime)
 
     async def restart_instance_async(
         self,
         instance_id: str,
-        request: hologram_20220601_models.RestartInstanceRequest,
     ) -> hologram_20220601_models.RestartInstanceResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.restart_instance_with_options_async(instance_id, request, headers, runtime)
+        return await self.restart_instance_with_options_async(instance_id, headers, runtime)
 
     def resume_instance_with_options(
         self,
         instance_id: str,
-        request: hologram_20220601_models.ResumeInstanceRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> hologram_20220601_models.ResumeInstanceResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
-            headers=headers,
-            query=OpenApiUtilClient.query(query)
+            headers=headers
         )
         params = open_api_models.Params(
             action='ResumeInstance',
             version='2022-06-01',
             protocol='HTTPS',
             pathname=f'/api/v1/instances/{OpenApiUtilClient.get_encode_param(instance_id)}/resume',
             method='POST',
@@ -319,25 +291,19 @@
             hologram_20220601_models.ResumeInstanceResponse(),
             self.call_api(params, req, runtime)
         )
 
     async def resume_instance_with_options_async(
         self,
         instance_id: str,
-        request: hologram_20220601_models.ResumeInstanceRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> hologram_20220601_models.ResumeInstanceResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
-            headers=headers,
-            query=OpenApiUtilClient.query(query)
+            headers=headers
         )
         params = open_api_models.Params(
             action='ResumeInstance',
             version='2022-06-01',
             protocol='HTTPS',
             pathname=f'/api/v1/instances/{OpenApiUtilClient.get_encode_param(instance_id)}/resume',
             method='POST',
@@ -350,43 +316,35 @@
             hologram_20220601_models.ResumeInstanceResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
     def resume_instance(
         self,
         instance_id: str,
-        request: hologram_20220601_models.ResumeInstanceRequest,
     ) -> hologram_20220601_models.ResumeInstanceResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.resume_instance_with_options(instance_id, request, headers, runtime)
+        return self.resume_instance_with_options(instance_id, headers, runtime)
 
     async def resume_instance_async(
         self,
         instance_id: str,
-        request: hologram_20220601_models.ResumeInstanceRequest,
     ) -> hologram_20220601_models.ResumeInstanceResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.resume_instance_with_options_async(instance_id, request, headers, runtime)
+        return await self.resume_instance_with_options_async(instance_id, headers, runtime)
 
     def stop_instance_with_options(
         self,
         instance_id: str,
-        request: hologram_20220601_models.StopInstanceRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> hologram_20220601_models.StopInstanceResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
-            headers=headers,
-            query=OpenApiUtilClient.query(query)
+            headers=headers
         )
         params = open_api_models.Params(
             action='StopInstance',
             version='2022-06-01',
             protocol='HTTPS',
             pathname=f'/api/v1/instances/{OpenApiUtilClient.get_encode_param(instance_id)}/stop',
             method='POST',
@@ -399,25 +357,19 @@
             hologram_20220601_models.StopInstanceResponse(),
             self.call_api(params, req, runtime)
         )
 
     async def stop_instance_with_options_async(
         self,
         instance_id: str,
-        request: hologram_20220601_models.StopInstanceRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> hologram_20220601_models.StopInstanceResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
-            headers=headers,
-            query=OpenApiUtilClient.query(query)
+            headers=headers
         )
         params = open_api_models.Params(
             action='StopInstance',
             version='2022-06-01',
             protocol='HTTPS',
             pathname=f'/api/v1/instances/{OpenApiUtilClient.get_encode_param(instance_id)}/stop',
             method='POST',
@@ -430,46 +382,40 @@
             hologram_20220601_models.StopInstanceResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
     def stop_instance(
         self,
         instance_id: str,
-        request: hologram_20220601_models.StopInstanceRequest,
     ) -> hologram_20220601_models.StopInstanceResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.stop_instance_with_options(instance_id, request, headers, runtime)
+        return self.stop_instance_with_options(instance_id, headers, runtime)
 
     async def stop_instance_async(
         self,
         instance_id: str,
-        request: hologram_20220601_models.StopInstanceRequest,
     ) -> hologram_20220601_models.StopInstanceResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.stop_instance_with_options_async(instance_id, request, headers, runtime)
+        return await self.stop_instance_with_options_async(instance_id, headers, runtime)
 
     def update_instance_name_with_options(
         self,
         instance_id: str,
         request: hologram_20220601_models.UpdateInstanceNameRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> hologram_20220601_models.UpdateInstanceNameResponse:
         UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
         body = {}
         if not UtilClient.is_unset(request.instance_name):
             body['instanceName'] = request.instance_name
         req = open_api_models.OpenApiRequest(
             headers=headers,
-            query=OpenApiUtilClient.query(query),
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='UpdateInstanceName',
             version='2022-06-01',
             protocol='HTTPS',
             pathname=f'/api/v1/instances/{OpenApiUtilClient.get_encode_param(instance_id)}/instanceName',
@@ -488,23 +434,19 @@
         self,
         instance_id: str,
         request: hologram_20220601_models.UpdateInstanceNameRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> hologram_20220601_models.UpdateInstanceNameResponse:
         UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
         body = {}
         if not UtilClient.is_unset(request.instance_name):
             body['instanceName'] = request.instance_name
         req = open_api_models.OpenApiRequest(
             headers=headers,
-            query=OpenApiUtilClient.query(query),
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='UpdateInstanceName',
             version='2022-06-01',
             protocol='HTTPS',
             pathname=f'/api/v1/instances/{OpenApiUtilClient.get_encode_param(instance_id)}/instanceName',
@@ -541,17 +483,14 @@
         self,
         instance_id: str,
         request: hologram_20220601_models.UpdateInstanceNetworkTypeRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> hologram_20220601_models.UpdateInstanceNetworkTypeResponse:
         UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
         body = {}
         if not UtilClient.is_unset(request.any_tunnel_to_single_tunnel):
             body['anyTunnelToSingleTunnel'] = request.any_tunnel_to_single_tunnel
         if not UtilClient.is_unset(request.network_types):
             body['networkTypes'] = request.network_types
         if not UtilClient.is_unset(request.v_switch_id):
             body['vSwitchId'] = request.v_switch_id
@@ -559,15 +498,14 @@
             body['vpcId'] = request.vpc_id
         if not UtilClient.is_unset(request.vpc_owner_id):
             body['vpcOwnerId'] = request.vpc_owner_id
         if not UtilClient.is_unset(request.vpc_region_id):
             body['vpcRegionId'] = request.vpc_region_id
         req = open_api_models.OpenApiRequest(
             headers=headers,
-            query=OpenApiUtilClient.query(query),
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='UpdateInstanceNetworkType',
             version='2022-06-01',
             protocol='HTTPS',
             pathname=f'/api/v1/instances/{OpenApiUtilClient.get_encode_param(instance_id)}/network',
@@ -586,17 +524,14 @@
         self,
         instance_id: str,
         request: hologram_20220601_models.UpdateInstanceNetworkTypeRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> hologram_20220601_models.UpdateInstanceNetworkTypeResponse:
         UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
         body = {}
         if not UtilClient.is_unset(request.any_tunnel_to_single_tunnel):
             body['anyTunnelToSingleTunnel'] = request.any_tunnel_to_single_tunnel
         if not UtilClient.is_unset(request.network_types):
             body['networkTypes'] = request.network_types
         if not UtilClient.is_unset(request.v_switch_id):
             body['vSwitchId'] = request.v_switch_id
@@ -604,15 +539,14 @@
             body['vpcId'] = request.vpc_id
         if not UtilClient.is_unset(request.vpc_owner_id):
             body['vpcOwnerId'] = request.vpc_owner_id
         if not UtilClient.is_unset(request.vpc_region_id):
             body['vpcRegionId'] = request.vpc_region_id
         req = open_api_models.OpenApiRequest(
             headers=headers,
-            query=OpenApiUtilClient.query(query),
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='UpdateInstanceNetworkType',
             version='2022-06-01',
             protocol='HTTPS',
             pathname=f'/api/v1/instances/{OpenApiUtilClient.get_encode_param(instance_id)}/network',
```

### Comparing `alibabacloud_hologram20220601-1.0.1/alibabacloud_hologram20220601/models.py` & `alibabacloud_hologram20220601-1.0.2/alibabacloud_hologram20220601/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -440,19 +440,17 @@
             self.value = m.get('value')
         return self
 
 
 class ListInstancesRequest(TeaModel):
     def __init__(
         self,
-        region_id: str = None,
         resource_group_id: str = None,
         tag: List[ListInstancesRequestTag] = None,
     ):
-        self.region_id = region_id
         self.resource_group_id = resource_group_id
         self.tag = tag
 
     def validate(self):
         if self.tag:
             for k in self.tag:
                 if k:
@@ -460,28 +458,24 @@
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.region_id is not None:
-            result['RegionId'] = self.region_id
         if self.resource_group_id is not None:
             result['resourceGroupId'] = self.resource_group_id
         result['tag'] = []
         if self.tag is not None:
             for k in self.tag:
                 result['tag'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('RegionId') is not None:
-            self.region_id = m.get('RegionId')
         if m.get('resourceGroupId') is not None:
             self.resource_group_id = m.get('resourceGroupId')
         self.tag = []
         if m.get('tag') is not None:
             for k in m.get('tag'):
                 temp_model = ListInstancesRequestTag()
                 self.tag.append(temp_model.from_map(k))
@@ -813,41 +807,14 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ListInstancesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class RestartInstanceRequest(TeaModel):
-    def __init__(
-        self,
-        region_id: str = None,
-    ):
-        self.region_id = region_id
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.region_id is not None:
-            result['RegionId'] = self.region_id
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('RegionId') is not None:
-            self.region_id = m.get('RegionId')
-        return self
-
-
 class RestartInstanceResponseBody(TeaModel):
     def __init__(
         self,
         data: bool = None,
         error_code: str = None,
         error_message: str = None,
         http_status_code: str = None,
@@ -942,41 +909,14 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = RestartInstanceResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class ResumeInstanceRequest(TeaModel):
-    def __init__(
-        self,
-        region_id: str = None,
-    ):
-        self.region_id = region_id
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.region_id is not None:
-            result['RegionId'] = self.region_id
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('RegionId') is not None:
-            self.region_id = m.get('RegionId')
-        return self
-
-
 class ResumeInstanceResponseBody(TeaModel):
     def __init__(
         self,
         data: bool = None,
         error_code: str = None,
         error_message: str = None,
         http_status_code: str = None,
@@ -1071,41 +1011,14 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ResumeInstanceResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class StopInstanceRequest(TeaModel):
-    def __init__(
-        self,
-        region_id: str = None,
-    ):
-        self.region_id = region_id
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.region_id is not None:
-            result['RegionId'] = self.region_id
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('RegionId') is not None:
-            self.region_id = m.get('RegionId')
-        return self
-
-
 class StopInstanceResponseBody(TeaModel):
     def __init__(
         self,
         data: bool = None,
         error_code: str = None,
         error_message: str = None,
         http_status_code: str = None,
@@ -1203,39 +1116,33 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class UpdateInstanceNameRequest(TeaModel):
     def __init__(
         self,
-        region_id: str = None,
         instance_name: str = None,
     ):
-        self.region_id = region_id
         self.instance_name = instance_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.region_id is not None:
-            result['RegionId'] = self.region_id
         if self.instance_name is not None:
             result['instanceName'] = self.instance_name
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('RegionId') is not None:
-            self.region_id = m.get('RegionId')
         if m.get('instanceName') is not None:
             self.instance_name = m.get('instanceName')
         return self
 
 
 class UpdateInstanceNameResponseBody(TeaModel):
     def __init__(
@@ -1338,23 +1245,21 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class UpdateInstanceNetworkTypeRequest(TeaModel):
     def __init__(
         self,
-        region_id: str = None,
         any_tunnel_to_single_tunnel: str = None,
         network_types: str = None,
         v_switch_id: str = None,
         vpc_id: str = None,
         vpc_owner_id: str = None,
         vpc_region_id: str = None,
     ):
-        self.region_id = region_id
         self.any_tunnel_to_single_tunnel = any_tunnel_to_single_tunnel
         self.network_types = network_types
         self.v_switch_id = v_switch_id
         # VPC ID。
         self.vpc_id = vpc_id
         self.vpc_owner_id = vpc_owner_id
         # vpc regionId。
@@ -1365,16 +1270,14 @@
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.region_id is not None:
-            result['RegionId'] = self.region_id
         if self.any_tunnel_to_single_tunnel is not None:
             result['anyTunnelToSingleTunnel'] = self.any_tunnel_to_single_tunnel
         if self.network_types is not None:
             result['networkTypes'] = self.network_types
         if self.v_switch_id is not None:
             result['vSwitchId'] = self.v_switch_id
         if self.vpc_id is not None:
@@ -1383,16 +1286,14 @@
             result['vpcOwnerId'] = self.vpc_owner_id
         if self.vpc_region_id is not None:
             result['vpcRegionId'] = self.vpc_region_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('RegionId') is not None:
-            self.region_id = m.get('RegionId')
         if m.get('anyTunnelToSingleTunnel') is not None:
             self.any_tunnel_to_single_tunnel = m.get('anyTunnelToSingleTunnel')
         if m.get('networkTypes') is not None:
             self.network_types = m.get('networkTypes')
         if m.get('vSwitchId') is not None:
             self.v_switch_id = m.get('vSwitchId')
         if m.get('vpcId') is not None:
```

### Comparing `alibabacloud_hologram20220601-1.0.1/alibabacloud_hologram20220601.egg-info/PKG-INFO` & `alibabacloud_hologram20220601-1.0.2/alibabacloud_hologram20220601.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-hologram20220601
-Version: 1.0.1
+Version: 1.0.2
 Summary: Alibaba Cloud Hologres (20220601) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_hologram20220601-1.0.1/setup.py` & `alibabacloud_hologram20220601-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_hologram20220601.
 
-Created on 19/04/2023
+Created on 26/04/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_hologram20220601"
 NAME = "alibabacloud_hologram20220601" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Hologres (20220601) SDK Library for Python"
```

