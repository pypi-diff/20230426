# Comparing `tmp/alibabacloud_config20200907-2.2.7.tar.gz` & `tmp/alibabacloud_config20200907-2.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_config20200907-2.2.7.tar", last modified: Wed Apr 12 15:13:45 2023, max compression
+gzip compressed data, was "dist/alibabacloud_config20200907-2.2.8.tar", last modified: Wed Apr 26 10:09:10 2023, max compression
```

## Comparing `alibabacloud_config20200907-2.2.7.tar` & `alibabacloud_config20200907-2.2.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 15:13:45.000000 alibabacloud_config20200907-2.2.7/
--rw-r--r--   0 root         (0) root         (0)      989 2023-04-12 15:13:45.000000 alibabacloud_config20200907-2.2.7/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-04-12 15:13:45.000000 alibabacloud_config20200907-2.2.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-04-12 15:13:45.000000 alibabacloud_config20200907-2.2.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2351 2023-04-12 15:13:45.000000 alibabacloud_config20200907-2.2.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1031 2023-04-12 15:13:45.000000 alibabacloud_config20200907-2.2.7/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1116 2023-04-12 15:13:45.000000 alibabacloud_config20200907-2.2.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 15:13:45.000000 alibabacloud_config20200907-2.2.7/alibabacloud_config20200907/
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-12 15:13:45.000000 alibabacloud_config20200907-2.2.7/alibabacloud_config20200907/__init__.py
--rw-r--r--   0 root         (0) root         (0)   575945 2023-04-12 15:13:45.000000 alibabacloud_config20200907-2.2.7/alibabacloud_config20200907/client.py
--rw-r--r--   0 root         (0) root         (0)  1139150 2023-04-12 15:13:45.000000 alibabacloud_config20200907-2.2.7/alibabacloud_config20200907/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 15:13:45.000000 alibabacloud_config20200907-2.2.7/alibabacloud_config20200907.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2351 2023-04-12 15:13:45.000000 alibabacloud_config20200907-2.2.7/alibabacloud_config20200907.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      444 2023-04-12 15:13:45.000000 alibabacloud_config20200907-2.2.7/alibabacloud_config20200907.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 15:13:45.000000 alibabacloud_config20200907-2.2.7/alibabacloud_config20200907.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-04-12 15:13:45.000000 alibabacloud_config20200907-2.2.7/alibabacloud_config20200907.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       28 2023-04-12 15:13:45.000000 alibabacloud_config20200907-2.2.7/alibabacloud_config20200907.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-04-12 15:13:45.000000 alibabacloud_config20200907-2.2.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2630 2023-04-12 15:13:45.000000 alibabacloud_config20200907-2.2.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 10:09:10.000000 alibabacloud_config20200907-2.2.8/
+-rw-r--r--   0 root         (0) root         (0)     1045 2023-04-26 10:09:10.000000 alibabacloud_config20200907-2.2.8/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-04-26 10:09:10.000000 alibabacloud_config20200907-2.2.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-26 10:09:10.000000 alibabacloud_config20200907-2.2.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2351 2023-04-26 10:09:10.000000 alibabacloud_config20200907-2.2.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1031 2023-04-26 10:09:10.000000 alibabacloud_config20200907-2.2.8/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1116 2023-04-26 10:09:10.000000 alibabacloud_config20200907-2.2.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 10:09:10.000000 alibabacloud_config20200907-2.2.8/alibabacloud_config20200907/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-26 10:09:10.000000 alibabacloud_config20200907-2.2.8/alibabacloud_config20200907/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   579579 2023-04-26 10:09:10.000000 alibabacloud_config20200907-2.2.8/alibabacloud_config20200907/client.py
+-rw-r--r--   0 root         (0) root         (0)  1158588 2023-04-26 10:09:10.000000 alibabacloud_config20200907-2.2.8/alibabacloud_config20200907/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 10:09:10.000000 alibabacloud_config20200907-2.2.8/alibabacloud_config20200907.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2351 2023-04-26 10:09:10.000000 alibabacloud_config20200907-2.2.8/alibabacloud_config20200907.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      444 2023-04-26 10:09:10.000000 alibabacloud_config20200907-2.2.8/alibabacloud_config20200907.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 10:09:10.000000 alibabacloud_config20200907-2.2.8/alibabacloud_config20200907.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-04-26 10:09:10.000000 alibabacloud_config20200907-2.2.8/alibabacloud_config20200907.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       28 2023-04-26 10:09:10.000000 alibabacloud_config20200907-2.2.8/alibabacloud_config20200907.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-26 10:09:10.000000 alibabacloud_config20200907-2.2.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2630 2023-04-26 10:09:10.000000 alibabacloud_config20200907-2.2.8/setup.py
```

### Comparing `alibabacloud_config20200907-2.2.7/ChangeLog.md` & `alibabacloud_config20200907-2.2.8/ChangeLog.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2023-04-12 Version: 2.2.7
+- Fix resourceOwnerId param.
+
 2022-12-27 Version: 2.2.3
 - Open Integrated Api.
 
 2022-11-29 Version: 2.2.2
 - Support ListRemediationExecutions.
 
 2022-11-02 Version: 2.2.1
```

### Comparing `alibabacloud_config20200907-2.2.7/LICENSE` & `alibabacloud_config20200907-2.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_config20200907-2.2.7/PKG-INFO` & `alibabacloud_config20200907-2.2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_config20200907
-Version: 2.2.7
+Version: 2.2.8
 Summary: Alibaba Cloud CloudConfig (20200907) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_config20200907-2.2.7/README-CN.md` & `alibabacloud_config20200907-2.2.8/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_config20200907-2.2.7/README.md` & `alibabacloud_config20200907-2.2.8/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_config20200907-2.2.7/alibabacloud_config20200907/client.py` & `alibabacloud_config20200907-2.2.8/alibabacloud_config20200907/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,16 @@
 
     def active_aggregate_config_rules_with_options(
         self,
         request: config_20200907_models.ActiveAggregateConfigRulesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.ActiveAggregateConfigRulesResponse:
         """
-        The sample request in this topic shows you how to enable the `cr-5772ba41209e007b***` rule in the `ca-a4e5626622af0079****` account group.
+        The ID of the rule. Separate multiple rule IDs with commas (,).
+        For more information about how to obtain the ID of a rule, see [ListAggregateConfigRules](~~264148~~).
         
         @param request: ActiveAggregateConfigRulesRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ActiveAggregateConfigRulesResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -84,15 +85,16 @@
 
     async def active_aggregate_config_rules_with_options_async(
         self,
         request: config_20200907_models.ActiveAggregateConfigRulesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.ActiveAggregateConfigRulesResponse:
         """
-        The sample request in this topic shows you how to enable the `cr-5772ba41209e007b***` rule in the `ca-a4e5626622af0079****` account group.
+        The ID of the rule. Separate multiple rule IDs with commas (,).
+        For more information about how to obtain the ID of a rule, see [ListAggregateConfigRules](~~264148~~).
         
         @param request: ActiveAggregateConfigRulesRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ActiveAggregateConfigRulesResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -120,28 +122,30 @@
         )
 
     def active_aggregate_config_rules(
         self,
         request: config_20200907_models.ActiveAggregateConfigRulesRequest,
     ) -> config_20200907_models.ActiveAggregateConfigRulesResponse:
         """
-        The sample request in this topic shows you how to enable the `cr-5772ba41209e007b***` rule in the `ca-a4e5626622af0079****` account group.
+        The ID of the rule. Separate multiple rule IDs with commas (,).
+        For more information about how to obtain the ID of a rule, see [ListAggregateConfigRules](~~264148~~).
         
         @param request: ActiveAggregateConfigRulesRequest
         @return: ActiveAggregateConfigRulesResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.active_aggregate_config_rules_with_options(request, runtime)
 
     async def active_aggregate_config_rules_async(
         self,
         request: config_20200907_models.ActiveAggregateConfigRulesRequest,
     ) -> config_20200907_models.ActiveAggregateConfigRulesResponse:
         """
-        The sample request in this topic shows you how to enable the `cr-5772ba41209e007b***` rule in the `ca-a4e5626622af0079****` account group.
+        The ID of the rule. Separate multiple rule IDs with commas (,).
+        For more information about how to obtain the ID of a rule, see [ListAggregateConfigRules](~~264148~~).
         
         @param request: ActiveAggregateConfigRulesRequest
         @return: ActiveAggregateConfigRulesResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.active_aggregate_config_rules_with_options_async(request, runtime)
 
@@ -803,17 +807,15 @@
 
     def create_aggregate_config_rule_with_options(
         self,
         tmp_req: config_20200907_models.CreateAggregateConfigRuleRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.CreateAggregateConfigRuleResponse:
         """
-        The sample request in this topic shows you how to create a rule based on the required-tags managed rule in the `ca-a4e5626622af0079***` account group. The return result shows that the rule is created and its ID is `cr-4e3d626622af0080****`.
-        ## Limits
-        A management account can contain up to 200 rules.
+        The description of the rule.
         
         @param tmp_req: CreateAggregateConfigRuleRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateAggregateConfigRuleResponse
         """
         UtilClient.validate_model(tmp_req)
         request = config_20200907_models.CreateAggregateConfigRuleShrinkRequest()
@@ -884,17 +886,15 @@
 
     async def create_aggregate_config_rule_with_options_async(
         self,
         tmp_req: config_20200907_models.CreateAggregateConfigRuleRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.CreateAggregateConfigRuleResponse:
         """
-        The sample request in this topic shows you how to create a rule based on the required-tags managed rule in the `ca-a4e5626622af0079***` account group. The return result shows that the rule is created and its ID is `cr-4e3d626622af0080****`.
-        ## Limits
-        A management account can contain up to 200 rules.
+        The description of the rule.
         
         @param tmp_req: CreateAggregateConfigRuleRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateAggregateConfigRuleResponse
         """
         UtilClient.validate_model(tmp_req)
         request = config_20200907_models.CreateAggregateConfigRuleShrinkRequest()
@@ -964,32 +964,28 @@
         )
 
     def create_aggregate_config_rule(
         self,
         request: config_20200907_models.CreateAggregateConfigRuleRequest,
     ) -> config_20200907_models.CreateAggregateConfigRuleResponse:
         """
-        The sample request in this topic shows you how to create a rule based on the required-tags managed rule in the `ca-a4e5626622af0079***` account group. The return result shows that the rule is created and its ID is `cr-4e3d626622af0080****`.
-        ## Limits
-        A management account can contain up to 200 rules.
+        The description of the rule.
         
         @param request: CreateAggregateConfigRuleRequest
         @return: CreateAggregateConfigRuleResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.create_aggregate_config_rule_with_options(request, runtime)
 
     async def create_aggregate_config_rule_async(
         self,
         request: config_20200907_models.CreateAggregateConfigRuleRequest,
     ) -> config_20200907_models.CreateAggregateConfigRuleResponse:
         """
-        The sample request in this topic shows you how to create a rule based on the required-tags managed rule in the `ca-a4e5626622af0079***` account group. The return result shows that the rule is created and its ID is `cr-4e3d626622af0080****`.
-        ## Limits
-        A management account can contain up to 200 rules.
+        The description of the rule.
         
         @param request: CreateAggregateConfigRuleRequest
         @return: CreateAggregateConfigRuleResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.create_aggregate_config_rule_with_options_async(request, runtime)
 
@@ -1991,15 +1987,16 @@
 
     def deactive_aggregate_config_rules_with_options(
         self,
         request: config_20200907_models.DeactiveAggregateConfigRulesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.DeactiveAggregateConfigRulesResponse:
         """
-        The sample request in this topic shows you how to disable the `cr-5772ba41209e007b***` rule in the `ca-04b3fd170e340007****` account group.
+        The ID of the rule. Separate multiple rule IDs with commas (,).
+        For more information about how to obtain the ID of a rule, see [ListAggregateConfigRules](~~264148~~).
         
         @param request: DeactiveAggregateConfigRulesRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeactiveAggregateConfigRulesResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -2028,15 +2025,16 @@
 
     async def deactive_aggregate_config_rules_with_options_async(
         self,
         request: config_20200907_models.DeactiveAggregateConfigRulesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.DeactiveAggregateConfigRulesResponse:
         """
-        The sample request in this topic shows you how to disable the `cr-5772ba41209e007b***` rule in the `ca-04b3fd170e340007****` account group.
+        The ID of the rule. Separate multiple rule IDs with commas (,).
+        For more information about how to obtain the ID of a rule, see [ListAggregateConfigRules](~~264148~~).
         
         @param request: DeactiveAggregateConfigRulesRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeactiveAggregateConfigRulesResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -2064,28 +2062,30 @@
         )
 
     def deactive_aggregate_config_rules(
         self,
         request: config_20200907_models.DeactiveAggregateConfigRulesRequest,
     ) -> config_20200907_models.DeactiveAggregateConfigRulesResponse:
         """
-        The sample request in this topic shows you how to disable the `cr-5772ba41209e007b***` rule in the `ca-04b3fd170e340007****` account group.
+        The ID of the rule. Separate multiple rule IDs with commas (,).
+        For more information about how to obtain the ID of a rule, see [ListAggregateConfigRules](~~264148~~).
         
         @param request: DeactiveAggregateConfigRulesRequest
         @return: DeactiveAggregateConfigRulesResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.deactive_aggregate_config_rules_with_options(request, runtime)
 
     async def deactive_aggregate_config_rules_async(
         self,
         request: config_20200907_models.DeactiveAggregateConfigRulesRequest,
     ) -> config_20200907_models.DeactiveAggregateConfigRulesResponse:
         """
-        The sample request in this topic shows you how to disable the `cr-5772ba41209e007b***` rule in the `ca-04b3fd170e340007****` account group.
+        The ID of the rule. Separate multiple rule IDs with commas (,).
+        For more information about how to obtain the ID of a rule, see [ListAggregateConfigRules](~~264148~~).
         
         @param request: DeactiveAggregateConfigRulesRequest
         @return: DeactiveAggregateConfigRulesResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.deactive_aggregate_config_rules_with_options_async(request, runtime)
 
@@ -2603,15 +2603,15 @@
 
     def delete_aggregators_with_options(
         self,
         request: config_20200907_models.DeleteAggregatorsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.DeleteAggregatorsResponse:
         """
-        In the example of this topic, a request is sent to delete the account group whose ID is `ca-9190626622af00a9***`.
+        The operation that you want to perform. Set the value to *DeleteAggregators**.
         
         @param request: DeleteAggregatorsRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteAggregatorsResponse
         """
         UtilClient.validate_model(request)
         body = {}
@@ -2640,15 +2640,15 @@
 
     async def delete_aggregators_with_options_async(
         self,
         request: config_20200907_models.DeleteAggregatorsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.DeleteAggregatorsResponse:
         """
-        In the example of this topic, a request is sent to delete the account group whose ID is `ca-9190626622af00a9***`.
+        The operation that you want to perform. Set the value to *DeleteAggregators**.
         
         @param request: DeleteAggregatorsRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteAggregatorsResponse
         """
         UtilClient.validate_model(request)
         body = {}
@@ -2676,28 +2676,28 @@
         )
 
     def delete_aggregators(
         self,
         request: config_20200907_models.DeleteAggregatorsRequest,
     ) -> config_20200907_models.DeleteAggregatorsResponse:
         """
-        In the example of this topic, a request is sent to delete the account group whose ID is `ca-9190626622af00a9***`.
+        The operation that you want to perform. Set the value to *DeleteAggregators**.
         
         @param request: DeleteAggregatorsRequest
         @return: DeleteAggregatorsResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.delete_aggregators_with_options(request, runtime)
 
     async def delete_aggregators_async(
         self,
         request: config_20200907_models.DeleteAggregatorsRequest,
     ) -> config_20200907_models.DeleteAggregatorsResponse:
         """
-        In the example of this topic, a request is sent to delete the account group whose ID is `ca-9190626622af00a9***`.
+        The operation that you want to perform. Set the value to *DeleteAggregators**.
         
         @param request: DeleteAggregatorsRequest
         @return: DeleteAggregatorsResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.delete_aggregators_with_options_async(request, runtime)
 
@@ -4467,15 +4467,16 @@
 
     def get_aggregate_discovered_resource_with_options(
         self,
         request: config_20200907_models.GetAggregateDiscoveredResourceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GetAggregateDiscoveredResourceResponse:
         """
-        The sample request in this topic shows you how to query the `new-bucket` resource in the `ca-5885626622af0008***` account group.
+        The type of the resource.
+        For more information about how to query the type of a resource, see [ListAggregateDiscoveredResources](~~411691~~).
         
         @param request: GetAggregateDiscoveredResourceRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: GetAggregateDiscoveredResourceResponse
         """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
@@ -4500,15 +4501,16 @@
 
     async def get_aggregate_discovered_resource_with_options_async(
         self,
         request: config_20200907_models.GetAggregateDiscoveredResourceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GetAggregateDiscoveredResourceResponse:
         """
-        The sample request in this topic shows you how to query the `new-bucket` resource in the `ca-5885626622af0008***` account group.
+        The type of the resource.
+        For more information about how to query the type of a resource, see [ListAggregateDiscoveredResources](~~411691~~).
         
         @param request: GetAggregateDiscoveredResourceRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: GetAggregateDiscoveredResourceResponse
         """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
@@ -4532,42 +4534,45 @@
         )
 
     def get_aggregate_discovered_resource(
         self,
         request: config_20200907_models.GetAggregateDiscoveredResourceRequest,
     ) -> config_20200907_models.GetAggregateDiscoveredResourceResponse:
         """
-        The sample request in this topic shows you how to query the `new-bucket` resource in the `ca-5885626622af0008***` account group.
+        The type of the resource.
+        For more information about how to query the type of a resource, see [ListAggregateDiscoveredResources](~~411691~~).
         
         @param request: GetAggregateDiscoveredResourceRequest
         @return: GetAggregateDiscoveredResourceResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.get_aggregate_discovered_resource_with_options(request, runtime)
 
     async def get_aggregate_discovered_resource_async(
         self,
         request: config_20200907_models.GetAggregateDiscoveredResourceRequest,
     ) -> config_20200907_models.GetAggregateDiscoveredResourceResponse:
         """
-        The sample request in this topic shows you how to query the `new-bucket` resource in the `ca-5885626622af0008***` account group.
+        The type of the resource.
+        For more information about how to query the type of a resource, see [ListAggregateDiscoveredResources](~~411691~~).
         
         @param request: GetAggregateDiscoveredResourceRequest
         @return: GetAggregateDiscoveredResourceResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.get_aggregate_discovered_resource_with_options_async(request, runtime)
 
     def get_aggregate_resource_compliance_by_config_rule_with_options(
         self,
         request: config_20200907_models.GetAggregateResourceComplianceByConfigRuleRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GetAggregateResourceComplianceByConfigRuleResponse:
         """
-        The sample request in this topic shows you how to query the compliance evaluation results based on the `cr-d369626622af008e***` rule in the `ca-a4e5626622af0079****` account group. The return result shows that a total of 10 resources are evaluated by the rule and five of them are evaluated as compliant.
+        The ID of the rule.
+        For more information about how to query the ID of a rule, see [ListAggregateConfigRules](~~264148~~).
         
         @param request: GetAggregateResourceComplianceByConfigRuleRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: GetAggregateResourceComplianceByConfigRuleResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -4602,15 +4607,16 @@
 
     async def get_aggregate_resource_compliance_by_config_rule_with_options_async(
         self,
         request: config_20200907_models.GetAggregateResourceComplianceByConfigRuleRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GetAggregateResourceComplianceByConfigRuleResponse:
         """
-        The sample request in this topic shows you how to query the compliance evaluation results based on the `cr-d369626622af008e***` rule in the `ca-a4e5626622af0079****` account group. The return result shows that a total of 10 resources are evaluated by the rule and five of them are evaluated as compliant.
+        The ID of the rule.
+        For more information about how to query the ID of a rule, see [ListAggregateConfigRules](~~264148~~).
         
         @param request: GetAggregateResourceComplianceByConfigRuleRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: GetAggregateResourceComplianceByConfigRuleResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -4644,28 +4650,30 @@
         )
 
     def get_aggregate_resource_compliance_by_config_rule(
         self,
         request: config_20200907_models.GetAggregateResourceComplianceByConfigRuleRequest,
     ) -> config_20200907_models.GetAggregateResourceComplianceByConfigRuleResponse:
         """
-        The sample request in this topic shows you how to query the compliance evaluation results based on the `cr-d369626622af008e***` rule in the `ca-a4e5626622af0079****` account group. The return result shows that a total of 10 resources are evaluated by the rule and five of them are evaluated as compliant.
+        The ID of the rule.
+        For more information about how to query the ID of a rule, see [ListAggregateConfigRules](~~264148~~).
         
         @param request: GetAggregateResourceComplianceByConfigRuleRequest
         @return: GetAggregateResourceComplianceByConfigRuleResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.get_aggregate_resource_compliance_by_config_rule_with_options(request, runtime)
 
     async def get_aggregate_resource_compliance_by_config_rule_async(
         self,
         request: config_20200907_models.GetAggregateResourceComplianceByConfigRuleRequest,
     ) -> config_20200907_models.GetAggregateResourceComplianceByConfigRuleResponse:
         """
-        The sample request in this topic shows you how to query the compliance evaluation results based on the `cr-d369626622af008e***` rule in the `ca-a4e5626622af0079****` account group. The return result shows that a total of 10 resources are evaluated by the rule and five of them are evaluated as compliant.
+        The ID of the rule.
+        For more information about how to query the ID of a rule, see [ListAggregateConfigRules](~~264148~~).
         
         @param request: GetAggregateResourceComplianceByConfigRuleRequest
         @return: GetAggregateResourceComplianceByConfigRuleResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.get_aggregate_resource_compliance_by_config_rule_with_options_async(request, runtime)
 
@@ -4911,15 +4919,15 @@
 
     def get_aggregate_resource_compliance_timeline_with_options(
         self,
         request: config_20200907_models.GetAggregateResourceComplianceTimelineRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GetAggregateResourceComplianceTimelineResponse:
         """
-        The sample request in this topic shows you how to query the compliance timeline of the `new-bucket` resource that resides in the `cn-hangzhou` region within the `100931896542***` member account of the `ca-5885626622af0008****` account group. The new-bucket resource is an Object Storage Service (OSS) bucket. The return result shows the following two timestamps on the compliance timeline: `1625200295276` and `1625200228510`. The first timestamp indicates 12:31:35 on July 2, 2021 (UTC+8), and the second timestamp indicates 12:30:28 on July 2, 2021 (UTC+8).
+        The operation that you want to perform. Set the value to *GetAggregateResourceComplianceTimeline**.
         
         @param request: GetAggregateResourceComplianceTimelineRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: GetAggregateResourceComplianceTimelineResponse
         """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
@@ -4944,15 +4952,15 @@
 
     async def get_aggregate_resource_compliance_timeline_with_options_async(
         self,
         request: config_20200907_models.GetAggregateResourceComplianceTimelineRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GetAggregateResourceComplianceTimelineResponse:
         """
-        The sample request in this topic shows you how to query the compliance timeline of the `new-bucket` resource that resides in the `cn-hangzhou` region within the `100931896542***` member account of the `ca-5885626622af0008****` account group. The new-bucket resource is an Object Storage Service (OSS) bucket. The return result shows the following two timestamps on the compliance timeline: `1625200295276` and `1625200228510`. The first timestamp indicates 12:31:35 on July 2, 2021 (UTC+8), and the second timestamp indicates 12:30:28 on July 2, 2021 (UTC+8).
+        The operation that you want to perform. Set the value to *GetAggregateResourceComplianceTimeline**.
         
         @param request: GetAggregateResourceComplianceTimelineRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: GetAggregateResourceComplianceTimelineResponse
         """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
@@ -4976,42 +4984,43 @@
         )
 
     def get_aggregate_resource_compliance_timeline(
         self,
         request: config_20200907_models.GetAggregateResourceComplianceTimelineRequest,
     ) -> config_20200907_models.GetAggregateResourceComplianceTimelineResponse:
         """
-        The sample request in this topic shows you how to query the compliance timeline of the `new-bucket` resource that resides in the `cn-hangzhou` region within the `100931896542***` member account of the `ca-5885626622af0008****` account group. The new-bucket resource is an Object Storage Service (OSS) bucket. The return result shows the following two timestamps on the compliance timeline: `1625200295276` and `1625200228510`. The first timestamp indicates 12:31:35 on July 2, 2021 (UTC+8), and the second timestamp indicates 12:30:28 on July 2, 2021 (UTC+8).
+        The operation that you want to perform. Set the value to *GetAggregateResourceComplianceTimeline**.
         
         @param request: GetAggregateResourceComplianceTimelineRequest
         @return: GetAggregateResourceComplianceTimelineResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.get_aggregate_resource_compliance_timeline_with_options(request, runtime)
 
     async def get_aggregate_resource_compliance_timeline_async(
         self,
         request: config_20200907_models.GetAggregateResourceComplianceTimelineRequest,
     ) -> config_20200907_models.GetAggregateResourceComplianceTimelineResponse:
         """
-        The sample request in this topic shows you how to query the compliance timeline of the `new-bucket` resource that resides in the `cn-hangzhou` region within the `100931896542***` member account of the `ca-5885626622af0008****` account group. The new-bucket resource is an Object Storage Service (OSS) bucket. The return result shows the following two timestamps on the compliance timeline: `1625200295276` and `1625200228510`. The first timestamp indicates 12:31:35 on July 2, 2021 (UTC+8), and the second timestamp indicates 12:30:28 on July 2, 2021 (UTC+8).
+        The operation that you want to perform. Set the value to *GetAggregateResourceComplianceTimeline**.
         
         @param request: GetAggregateResourceComplianceTimelineRequest
         @return: GetAggregateResourceComplianceTimelineResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.get_aggregate_resource_compliance_timeline_with_options_async(request, runtime)
 
     def get_aggregate_resource_configuration_timeline_with_options(
         self,
         request: config_20200907_models.GetAggregateResourceConfigurationTimelineRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GetAggregateResourceConfigurationTimelineResponse:
         """
-        The sample request in this topic shows you how to query the configuration timeline of the `new-bucket` resource that resides in the `cn-hangzhou` region within the `100931896542***` member account of the `ca-5885626622af0008****` account group. The new-bucket resource is an Object Storage Service (OSS) bucket. The return result shows that the timestamp when the resource configuration changes is `1624961112000`. The timestamp indicates 18:05:12 on June 29, 2021 (UTC+8).
+        The ID of the resource.
+        For more information about how to obtain the ID of a resource, see [ListAggregateDiscoveredResources](~~265983~~).
         
         @param request: GetAggregateResourceConfigurationTimelineRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: GetAggregateResourceConfigurationTimelineResponse
         """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
@@ -5036,15 +5045,16 @@
 
     async def get_aggregate_resource_configuration_timeline_with_options_async(
         self,
         request: config_20200907_models.GetAggregateResourceConfigurationTimelineRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GetAggregateResourceConfigurationTimelineResponse:
         """
-        The sample request in this topic shows you how to query the configuration timeline of the `new-bucket` resource that resides in the `cn-hangzhou` region within the `100931896542***` member account of the `ca-5885626622af0008****` account group. The new-bucket resource is an Object Storage Service (OSS) bucket. The return result shows that the timestamp when the resource configuration changes is `1624961112000`. The timestamp indicates 18:05:12 on June 29, 2021 (UTC+8).
+        The ID of the resource.
+        For more information about how to obtain the ID of a resource, see [ListAggregateDiscoveredResources](~~265983~~).
         
         @param request: GetAggregateResourceConfigurationTimelineRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: GetAggregateResourceConfigurationTimelineResponse
         """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
@@ -5068,42 +5078,45 @@
         )
 
     def get_aggregate_resource_configuration_timeline(
         self,
         request: config_20200907_models.GetAggregateResourceConfigurationTimelineRequest,
     ) -> config_20200907_models.GetAggregateResourceConfigurationTimelineResponse:
         """
-        The sample request in this topic shows you how to query the configuration timeline of the `new-bucket` resource that resides in the `cn-hangzhou` region within the `100931896542***` member account of the `ca-5885626622af0008****` account group. The new-bucket resource is an Object Storage Service (OSS) bucket. The return result shows that the timestamp when the resource configuration changes is `1624961112000`. The timestamp indicates 18:05:12 on June 29, 2021 (UTC+8).
+        The ID of the resource.
+        For more information about how to obtain the ID of a resource, see [ListAggregateDiscoveredResources](~~265983~~).
         
         @param request: GetAggregateResourceConfigurationTimelineRequest
         @return: GetAggregateResourceConfigurationTimelineResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.get_aggregate_resource_configuration_timeline_with_options(request, runtime)
 
     async def get_aggregate_resource_configuration_timeline_async(
         self,
         request: config_20200907_models.GetAggregateResourceConfigurationTimelineRequest,
     ) -> config_20200907_models.GetAggregateResourceConfigurationTimelineResponse:
         """
-        The sample request in this topic shows you how to query the configuration timeline of the `new-bucket` resource that resides in the `cn-hangzhou` region within the `100931896542***` member account of the `ca-5885626622af0008****` account group. The new-bucket resource is an Object Storage Service (OSS) bucket. The return result shows that the timestamp when the resource configuration changes is `1624961112000`. The timestamp indicates 18:05:12 on June 29, 2021 (UTC+8).
+        The ID of the resource.
+        For more information about how to obtain the ID of a resource, see [ListAggregateDiscoveredResources](~~265983~~).
         
         @param request: GetAggregateResourceConfigurationTimelineRequest
         @return: GetAggregateResourceConfigurationTimelineResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.get_aggregate_resource_configuration_timeline_with_options_async(request, runtime)
 
     def get_aggregate_resource_counts_group_by_region_with_options(
         self,
         request: config_20200907_models.GetAggregateResourceCountsGroupByRegionRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GetAggregateResourceCountsGroupByRegionResponse:
         """
-        This topic provides an example on how to query the statistics on the resources in an account group named `ca-a260626622af0005***` by region. The returned result shows that a total of `10` resources exist in the `cn-hangzhou` region.
+        The ID of the account group.
+        For more information about how to obtain the ID of an account group, see [ListAggregators](~~255797~~).
         
         @param request: GetAggregateResourceCountsGroupByRegionRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: GetAggregateResourceCountsGroupByRegionResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -5138,15 +5151,16 @@
 
     async def get_aggregate_resource_counts_group_by_region_with_options_async(
         self,
         request: config_20200907_models.GetAggregateResourceCountsGroupByRegionRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GetAggregateResourceCountsGroupByRegionResponse:
         """
-        This topic provides an example on how to query the statistics on the resources in an account group named `ca-a260626622af0005***` by region. The returned result shows that a total of `10` resources exist in the `cn-hangzhou` region.
+        The ID of the account group.
+        For more information about how to obtain the ID of an account group, see [ListAggregators](~~255797~~).
         
         @param request: GetAggregateResourceCountsGroupByRegionRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: GetAggregateResourceCountsGroupByRegionResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -5180,28 +5194,30 @@
         )
 
     def get_aggregate_resource_counts_group_by_region(
         self,
         request: config_20200907_models.GetAggregateResourceCountsGroupByRegionRequest,
     ) -> config_20200907_models.GetAggregateResourceCountsGroupByRegionResponse:
         """
-        This topic provides an example on how to query the statistics on the resources in an account group named `ca-a260626622af0005***` by region. The returned result shows that a total of `10` resources exist in the `cn-hangzhou` region.
+        The ID of the account group.
+        For more information about how to obtain the ID of an account group, see [ListAggregators](~~255797~~).
         
         @param request: GetAggregateResourceCountsGroupByRegionRequest
         @return: GetAggregateResourceCountsGroupByRegionResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.get_aggregate_resource_counts_group_by_region_with_options(request, runtime)
 
     async def get_aggregate_resource_counts_group_by_region_async(
         self,
         request: config_20200907_models.GetAggregateResourceCountsGroupByRegionRequest,
     ) -> config_20200907_models.GetAggregateResourceCountsGroupByRegionResponse:
         """
-        This topic provides an example on how to query the statistics on the resources in an account group named `ca-a260626622af0005***` by region. The returned result shows that a total of `10` resources exist in the `cn-hangzhou` region.
+        The ID of the account group.
+        For more information about how to obtain the ID of an account group, see [ListAggregators](~~255797~~).
         
         @param request: GetAggregateResourceCountsGroupByRegionRequest
         @return: GetAggregateResourceCountsGroupByRegionResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.get_aggregate_resource_counts_group_by_region_with_options_async(request, runtime)
 
@@ -6897,15 +6913,15 @@
 
     def get_resource_configuration_timeline_with_options(
         self,
         request: config_20200907_models.GetResourceConfigurationTimelineRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GetResourceConfigurationTimelineResponse:
         """
-        The sample request in this topic shows you how to query the configuration timeline of the `new-bucket` resource that resides in the `cn-hangzhou` region. The new-bucket resource is an Object Storage Service (OSS) bucket. The return result shows that the timestamp when the resource configuration changes is `1624961112000`. The timestamp indicates 18:05:12 on June 29, 2021 (UTC+8).
+        The timestamp that specifies the beginning of the time range to query. By default, Cloud Config retrieves the configuration changes in the last 30 days for the specified resource. Unit: milliseconds.
         
         @param request: GetResourceConfigurationTimelineRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: GetResourceConfigurationTimelineResponse
         """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
@@ -6930,15 +6946,15 @@
 
     async def get_resource_configuration_timeline_with_options_async(
         self,
         request: config_20200907_models.GetResourceConfigurationTimelineRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GetResourceConfigurationTimelineResponse:
         """
-        The sample request in this topic shows you how to query the configuration timeline of the `new-bucket` resource that resides in the `cn-hangzhou` region. The new-bucket resource is an Object Storage Service (OSS) bucket. The return result shows that the timestamp when the resource configuration changes is `1624961112000`. The timestamp indicates 18:05:12 on June 29, 2021 (UTC+8).
+        The timestamp that specifies the beginning of the time range to query. By default, Cloud Config retrieves the configuration changes in the last 30 days for the specified resource. Unit: milliseconds.
         
         @param request: GetResourceConfigurationTimelineRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: GetResourceConfigurationTimelineResponse
         """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
@@ -6962,28 +6978,28 @@
         )
 
     def get_resource_configuration_timeline(
         self,
         request: config_20200907_models.GetResourceConfigurationTimelineRequest,
     ) -> config_20200907_models.GetResourceConfigurationTimelineResponse:
         """
-        The sample request in this topic shows you how to query the configuration timeline of the `new-bucket` resource that resides in the `cn-hangzhou` region. The new-bucket resource is an Object Storage Service (OSS) bucket. The return result shows that the timestamp when the resource configuration changes is `1624961112000`. The timestamp indicates 18:05:12 on June 29, 2021 (UTC+8).
+        The timestamp that specifies the beginning of the time range to query. By default, Cloud Config retrieves the configuration changes in the last 30 days for the specified resource. Unit: milliseconds.
         
         @param request: GetResourceConfigurationTimelineRequest
         @return: GetResourceConfigurationTimelineResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.get_resource_configuration_timeline_with_options(request, runtime)
 
     async def get_resource_configuration_timeline_async(
         self,
         request: config_20200907_models.GetResourceConfigurationTimelineRequest,
     ) -> config_20200907_models.GetResourceConfigurationTimelineResponse:
         """
-        The sample request in this topic shows you how to query the configuration timeline of the `new-bucket` resource that resides in the `cn-hangzhou` region. The new-bucket resource is an Object Storage Service (OSS) bucket. The return result shows that the timestamp when the resource configuration changes is `1624961112000`. The timestamp indicates 18:05:12 on June 29, 2021 (UTC+8).
+        The timestamp that specifies the beginning of the time range to query. By default, Cloud Config retrieves the configuration changes in the last 30 days for the specified resource. Unit: milliseconds.
         
         @param request: GetResourceConfigurationTimelineRequest
         @return: GetResourceConfigurationTimelineResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.get_resource_configuration_timeline_with_options_async(request, runtime)
 
@@ -7679,15 +7695,15 @@
 
     def list_aggregate_discovered_resources_with_options(
         self,
         request: config_20200907_models.ListAggregateDiscoveredResourcesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.ListAggregateDiscoveredResourcesResponse:
         """
-        This example shows how to query the resources in the `ca-c560626622af0005***` account group. The response shows that the account group contains eight resources.
+        The token that you want to use to initiate the current request. If the response of the previous request is truncated, you can use this token to initiate another request and obtain the remaining entries.``
         
         @param request: ListAggregateDiscoveredResourcesRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ListAggregateDiscoveredResourcesResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -7730,15 +7746,15 @@
 
     async def list_aggregate_discovered_resources_with_options_async(
         self,
         request: config_20200907_models.ListAggregateDiscoveredResourcesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.ListAggregateDiscoveredResourcesResponse:
         """
-        This example shows how to query the resources in the `ca-c560626622af0005***` account group. The response shows that the account group contains eight resources.
+        The token that you want to use to initiate the current request. If the response of the previous request is truncated, you can use this token to initiate another request and obtain the remaining entries.``
         
         @param request: ListAggregateDiscoveredResourcesRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ListAggregateDiscoveredResourcesResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -7780,28 +7796,28 @@
         )
 
     def list_aggregate_discovered_resources(
         self,
         request: config_20200907_models.ListAggregateDiscoveredResourcesRequest,
     ) -> config_20200907_models.ListAggregateDiscoveredResourcesResponse:
         """
-        This example shows how to query the resources in the `ca-c560626622af0005***` account group. The response shows that the account group contains eight resources.
+        The token that you want to use to initiate the current request. If the response of the previous request is truncated, you can use this token to initiate another request and obtain the remaining entries.``
         
         @param request: ListAggregateDiscoveredResourcesRequest
         @return: ListAggregateDiscoveredResourcesResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.list_aggregate_discovered_resources_with_options(request, runtime)
 
     async def list_aggregate_discovered_resources_async(
         self,
         request: config_20200907_models.ListAggregateDiscoveredResourcesRequest,
     ) -> config_20200907_models.ListAggregateDiscoveredResourcesResponse:
         """
-        This example shows how to query the resources in the `ca-c560626622af0005***` account group. The response shows that the account group contains eight resources.
+        The token that you want to use to initiate the current request. If the response of the previous request is truncated, you can use this token to initiate another request and obtain the remaining entries.``
         
         @param request: ListAggregateDiscoveredResourcesRequest
         @return: ListAggregateDiscoveredResourcesResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.list_aggregate_discovered_resources_with_options_async(request, runtime)
 
@@ -8021,14 +8037,120 @@
         
         @param request: ListAggregateResourceEvaluationResultsRequest
         @return: ListAggregateResourceEvaluationResultsResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.list_aggregate_resource_evaluation_results_with_options_async(request, runtime)
 
+    def list_aggregate_resource_relations_with_options(
+        self,
+        request: config_20200907_models.ListAggregateResourceRelationsRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> config_20200907_models.ListAggregateResourceRelationsResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.aggregator_id):
+            query['AggregatorId'] = request.aggregator_id
+        if not UtilClient.is_unset(request.max_results):
+            query['MaxResults'] = request.max_results
+        if not UtilClient.is_unset(request.next_token):
+            query['NextToken'] = request.next_token
+        if not UtilClient.is_unset(request.region):
+            query['Region'] = request.region
+        if not UtilClient.is_unset(request.relation_type):
+            query['RelationType'] = request.relation_type
+        if not UtilClient.is_unset(request.resource_account_id):
+            query['ResourceAccountId'] = request.resource_account_id
+        if not UtilClient.is_unset(request.resource_id):
+            query['ResourceId'] = request.resource_id
+        if not UtilClient.is_unset(request.resource_type):
+            query['ResourceType'] = request.resource_type
+        if not UtilClient.is_unset(request.target_resource_id):
+            query['TargetResourceId'] = request.target_resource_id
+        if not UtilClient.is_unset(request.target_resource_type):
+            query['TargetResourceType'] = request.target_resource_type
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListAggregateResourceRelations',
+            version='2020-09-07',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            config_20200907_models.ListAggregateResourceRelationsResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def list_aggregate_resource_relations_with_options_async(
+        self,
+        request: config_20200907_models.ListAggregateResourceRelationsRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> config_20200907_models.ListAggregateResourceRelationsResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.aggregator_id):
+            query['AggregatorId'] = request.aggregator_id
+        if not UtilClient.is_unset(request.max_results):
+            query['MaxResults'] = request.max_results
+        if not UtilClient.is_unset(request.next_token):
+            query['NextToken'] = request.next_token
+        if not UtilClient.is_unset(request.region):
+            query['Region'] = request.region
+        if not UtilClient.is_unset(request.relation_type):
+            query['RelationType'] = request.relation_type
+        if not UtilClient.is_unset(request.resource_account_id):
+            query['ResourceAccountId'] = request.resource_account_id
+        if not UtilClient.is_unset(request.resource_id):
+            query['ResourceId'] = request.resource_id
+        if not UtilClient.is_unset(request.resource_type):
+            query['ResourceType'] = request.resource_type
+        if not UtilClient.is_unset(request.target_resource_id):
+            query['TargetResourceId'] = request.target_resource_id
+        if not UtilClient.is_unset(request.target_resource_type):
+            query['TargetResourceType'] = request.target_resource_type
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListAggregateResourceRelations',
+            version='2020-09-07',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            config_20200907_models.ListAggregateResourceRelationsResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def list_aggregate_resource_relations(
+        self,
+        request: config_20200907_models.ListAggregateResourceRelationsRequest,
+    ) -> config_20200907_models.ListAggregateResourceRelationsResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.list_aggregate_resource_relations_with_options(request, runtime)
+
+    async def list_aggregate_resource_relations_async(
+        self,
+        request: config_20200907_models.ListAggregateResourceRelationsRequest,
+    ) -> config_20200907_models.ListAggregateResourceRelationsResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.list_aggregate_resource_relations_with_options_async(request, runtime)
+
     def list_aggregators_with_options(
         self,
         request: config_20200907_models.ListAggregatorsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.ListAggregatorsResponse:
         """
         The sample request in this topic shows you how to query account groups. A maximum of 10 entries can be returned for the request. As shown in the responses, the account group returned is named as `Test_Group`, its description is `Test account group`, and it is of the `CUSTOM` type, which indicates a custom account group. The account group contains two member accounts.
@@ -8923,14 +9045,18 @@
         @param runtime: runtime options for this request RuntimeOptions
         @return: ListRemediationTemplatesResponse
         """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.managed_rule_identifier):
             query['ManagedRuleIdentifier'] = request.managed_rule_identifier
+        if not UtilClient.is_unset(request.page_number):
+            query['PageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.remediation_type):
             query['RemediationType'] = request.remediation_type
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListRemediationTemplates',
@@ -8960,14 +9086,18 @@
         @param runtime: runtime options for this request RuntimeOptions
         @return: ListRemediationTemplatesResponse
         """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.managed_rule_identifier):
             query['ManagedRuleIdentifier'] = request.managed_rule_identifier
+        if not UtilClient.is_unset(request.page_number):
+            query['PageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.remediation_type):
             query['RemediationType'] = request.remediation_type
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListRemediationTemplates',
@@ -9023,14 +9153,18 @@
         @param runtime: runtime options for this request RuntimeOptions
         @return: ListRemediationsResponse
         """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.config_rule_ids):
             query['ConfigRuleIds'] = request.config_rule_ids
+        if not UtilClient.is_unset(request.page_number):
+            query['PageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListRemediations',
             version='2020-09-07',
             protocol='HTTPS',
@@ -9058,14 +9192,18 @@
         @param runtime: runtime options for this request RuntimeOptions
         @return: ListRemediationsResponse
         """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.config_rule_ids):
             query['ConfigRuleIds'] = request.config_rule_ids
+        if not UtilClient.is_unset(request.page_number):
+            query['PageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListRemediations',
             version='2020-09-07',
             protocol='HTTPS',
@@ -9219,14 +9357,112 @@
         
         @param request: ListResourceEvaluationResultsRequest
         @return: ListResourceEvaluationResultsResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.list_resource_evaluation_results_with_options_async(request, runtime)
 
+    def list_resource_relations_with_options(
+        self,
+        request: config_20200907_models.ListResourceRelationsRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> config_20200907_models.ListResourceRelationsResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.max_results):
+            query['MaxResults'] = request.max_results
+        if not UtilClient.is_unset(request.next_token):
+            query['NextToken'] = request.next_token
+        if not UtilClient.is_unset(request.region):
+            query['Region'] = request.region
+        if not UtilClient.is_unset(request.relation_type):
+            query['RelationType'] = request.relation_type
+        if not UtilClient.is_unset(request.resource_id):
+            query['ResourceId'] = request.resource_id
+        if not UtilClient.is_unset(request.resource_type):
+            query['ResourceType'] = request.resource_type
+        if not UtilClient.is_unset(request.target_resource_id):
+            query['TargetResourceId'] = request.target_resource_id
+        if not UtilClient.is_unset(request.target_resource_type):
+            query['TargetResourceType'] = request.target_resource_type
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListResourceRelations',
+            version='2020-09-07',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            config_20200907_models.ListResourceRelationsResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def list_resource_relations_with_options_async(
+        self,
+        request: config_20200907_models.ListResourceRelationsRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> config_20200907_models.ListResourceRelationsResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.max_results):
+            query['MaxResults'] = request.max_results
+        if not UtilClient.is_unset(request.next_token):
+            query['NextToken'] = request.next_token
+        if not UtilClient.is_unset(request.region):
+            query['Region'] = request.region
+        if not UtilClient.is_unset(request.relation_type):
+            query['RelationType'] = request.relation_type
+        if not UtilClient.is_unset(request.resource_id):
+            query['ResourceId'] = request.resource_id
+        if not UtilClient.is_unset(request.resource_type):
+            query['ResourceType'] = request.resource_type
+        if not UtilClient.is_unset(request.target_resource_id):
+            query['TargetResourceId'] = request.target_resource_id
+        if not UtilClient.is_unset(request.target_resource_type):
+            query['TargetResourceType'] = request.target_resource_type
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListResourceRelations',
+            version='2020-09-07',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            config_20200907_models.ListResourceRelationsResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def list_resource_relations(
+        self,
+        request: config_20200907_models.ListResourceRelationsRequest,
+    ) -> config_20200907_models.ListResourceRelationsResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.list_resource_relations_with_options(request, runtime)
+
+    async def list_resource_relations_async(
+        self,
+        request: config_20200907_models.ListResourceRelationsRequest,
+    ) -> config_20200907_models.ListResourceRelationsResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.list_resource_relations_with_options_async(request, runtime)
+
     def list_tag_resources_with_options(
         self,
         tmp_req: config_20200907_models.ListTagResourcesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.ListTagResourcesResponse:
         UtilClient.validate_model(tmp_req)
         request = config_20200907_models.ListTagResourcesShrinkRequest()
@@ -11250,15 +11486,15 @@
     def update_delivery_channel_with_options(
         self,
         request: config_20200907_models.UpdateDeliveryChannelRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.UpdateDeliveryChannelResponse:
         """
         @deprecated : UpdateDeliveryChannel is deprecated, please use Config::2020-09-07::UpdateConfigDeliveryChannel,Config::2020-09-07::UpdateAggregateConfigDeliveryChannel instead.
-        In this example, the status of the delivery channel whose ID is `cdc-8e45ff4e06a3a8****` is changed to 0, which indicates that the delivery channel is disabled. After the delivery channel is disabled, Cloud Config retains the last delivery configuration and stops resource data delivery.
+        The operation that you want to perform. Set the value to **UpdateDeliveryChannel**.
         
         @param request: UpdateDeliveryChannelRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: UpdateDeliveryChannelResponse
         Deprecated
         """
         UtilClient.validate_model(request)
@@ -11309,15 +11545,15 @@
     async def update_delivery_channel_with_options_async(
         self,
         request: config_20200907_models.UpdateDeliveryChannelRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.UpdateDeliveryChannelResponse:
         """
         @deprecated : UpdateDeliveryChannel is deprecated, please use Config::2020-09-07::UpdateConfigDeliveryChannel,Config::2020-09-07::UpdateAggregateConfigDeliveryChannel instead.
-        In this example, the status of the delivery channel whose ID is `cdc-8e45ff4e06a3a8****` is changed to 0, which indicates that the delivery channel is disabled. After the delivery channel is disabled, Cloud Config retains the last delivery configuration and stops resource data delivery.
+        The operation that you want to perform. Set the value to **UpdateDeliveryChannel**.
         
         @param request: UpdateDeliveryChannelRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: UpdateDeliveryChannelResponse
         Deprecated
         """
         UtilClient.validate_model(request)
@@ -11367,30 +11603,30 @@
 
     def update_delivery_channel(
         self,
         request: config_20200907_models.UpdateDeliveryChannelRequest,
     ) -> config_20200907_models.UpdateDeliveryChannelResponse:
         """
         @deprecated : UpdateDeliveryChannel is deprecated, please use Config::2020-09-07::UpdateConfigDeliveryChannel,Config::2020-09-07::UpdateAggregateConfigDeliveryChannel instead.
-        In this example, the status of the delivery channel whose ID is `cdc-8e45ff4e06a3a8****` is changed to 0, which indicates that the delivery channel is disabled. After the delivery channel is disabled, Cloud Config retains the last delivery configuration and stops resource data delivery.
+        The operation that you want to perform. Set the value to **UpdateDeliveryChannel**.
         
         @param request: UpdateDeliveryChannelRequest
         @return: UpdateDeliveryChannelResponse
         Deprecated
         """
         runtime = util_models.RuntimeOptions()
         return self.update_delivery_channel_with_options(request, runtime)
 
     async def update_delivery_channel_async(
         self,
         request: config_20200907_models.UpdateDeliveryChannelRequest,
     ) -> config_20200907_models.UpdateDeliveryChannelResponse:
         """
         @deprecated : UpdateDeliveryChannel is deprecated, please use Config::2020-09-07::UpdateConfigDeliveryChannel,Config::2020-09-07::UpdateAggregateConfigDeliveryChannel instead.
-        In this example, the status of the delivery channel whose ID is `cdc-8e45ff4e06a3a8****` is changed to 0, which indicates that the delivery channel is disabled. After the delivery channel is disabled, Cloud Config retains the last delivery configuration and stops resource data delivery.
+        The operation that you want to perform. Set the value to **UpdateDeliveryChannel**.
         
         @param request: UpdateDeliveryChannelRequest
         @return: UpdateDeliveryChannelResponse
         Deprecated
         """
         runtime = util_models.RuntimeOptions()
         return await self.update_delivery_channel_with_options_async(request, runtime)
```

### Comparing `alibabacloud_config20200907-2.2.7/alibabacloud_config20200907/models.py` & `alibabacloud_config20200907-2.2.8/alibabacloud_config20200907/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,21 +71,17 @@
 
 class ActiveAggregateConfigRulesRequest(TeaModel):
     def __init__(
         self,
         aggregator_id: str = None,
         config_rule_ids: str = None,
     ):
-        # The ID of the account group.
-        # 
-        # For more information about how to obtain the ID of an account group, see [ListAggregators](~~255797~~).
+        # The result of the operation to enable the rule.
         self.aggregator_id = aggregator_id
-        # The ID of the rule. Separate multiple rule IDs with commas (,).
-        # 
-        # For more information about how to obtain the ID of a rule, see [ListAggregateConfigRules](~~264148~~).
+        # The results of the operations to enable the specified rules.
         self.config_rule_ids = config_rule_ids
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -111,25 +107,16 @@
 class ActiveAggregateConfigRulesResponseBodyOperateRuleResultOperateRuleItemList(TeaModel):
     def __init__(
         self,
         config_rule_id: str = None,
         error_code: str = None,
         success: bool = None,
     ):
-        # The ID of the rule.
         self.config_rule_id = config_rule_id
-        # The error code returned.
-        # 
-        # *   If the rule is enabled, no error code is returned.
-        # *   If the rule fails to be enabled, an error code is returned. For more information about error codes, visit the [API Error Center](https://error-center.alibabacloud.com/status/product/Config).
         self.error_code = error_code
-        # Indicates whether the operation is successful. Valid values:
-        # 
-        # *   true: The operation is successful.
-        # *   false: The operation fails.
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -157,15 +144,15 @@
 
 
 class ActiveAggregateConfigRulesResponseBodyOperateRuleResult(TeaModel):
     def __init__(
         self,
         operate_rule_item_list: List[ActiveAggregateConfigRulesResponseBodyOperateRuleResultOperateRuleItemList] = None,
     ):
-        # The result of the operation to enable the rule.
+        # The ID of the rule.
         self.operate_rule_item_list = operate_rule_item_list
 
     def validate(self):
         if self.operate_rule_item_list:
             for k in self.operate_rule_item_list:
                 if k:
                     k.validate()
@@ -194,17 +181,23 @@
 
 class ActiveAggregateConfigRulesResponseBody(TeaModel):
     def __init__(
         self,
         operate_rule_result: ActiveAggregateConfigRulesResponseBodyOperateRuleResult = None,
         request_id: str = None,
     ):
-        # The results of the operations to enable the specified rules.
+        # Indicates whether the operation is successful. Valid values:
+        # 
+        # *   true: The operation is successful.
+        # *   false: The operation fails.
         self.operate_rule_result = operate_rule_result
-        # The ID of the request.
+        # The error code returned.
+        # 
+        # *   If the rule is enabled, no error code is returned.
+        # *   If the rule fails to be enabled, an error code is returned. For more information about error codes, visit the [API Error Center](https://error-center.alibabacloud.com/status/product/Config).
         self.request_id = request_id
 
     def validate(self):
         if self.operate_rule_result:
             self.operate_rule_result.validate()
 
     def to_map(self):
@@ -1660,101 +1653,96 @@
         risk_level: int = None,
         source_identifier: str = None,
         source_owner: str = None,
         tag_key_logic_scope: str = None,
         tag_key_scope: str = None,
         tag_value_scope: str = None,
     ):
-        # The ID of the account group.
+        # The way in which the rule is to be created. Valid values:
         # 
-        # For more information about how to query the ID of an account group, see [ListAggregators](~~255797~~).
+        # *   ALIYUN: The rule is to be created based on a managed rule of Alibaba Cloud.
+        # *   CUSTOM_FC: The rule is a custom rule.
         self.aggregator_id = aggregator_id
-        # The client token that is used to ensure the idempotence of the request. You can use the client to generate the value, but you must make sure that it is unique among different requests. The token can contain only ASCII characters and cannot exceed 64 characters in length.
-        self.client_token = client_token
-        # The name of the rule.
-        self.config_rule_name = config_rule_name
-        # The trigger type of the rule. Valid values:
-        # 
-        # *   ConfigurationItemChangeNotification: The rule is triggered by configuration changes.
-        # *   ScheduledNotification: The rule is periodically triggered.
-        self.config_rule_trigger_types = config_rule_trigger_types
-        # The description of the rule.
-        self.description = description
-        # The ID of the member account to which the rule does not apply, which means that the resources within the member account are not evaluated based on the rule. Separate multiple member account IDs with commas (,).
-        # 
-        # >  This parameter applies only to a managed rule.
-        self.exclude_account_ids_scope = exclude_account_ids_scope
-        # The ID of the resource directory to which the rule does not apply, which means that the resources within member accounts in the resource directory are not evaluated based on the rule. Separate multiple resource directory IDs with commas (,).
-        # 
-        # > 
-        # *   This parameter applies only to a rule of a global account group.
-        # *   This parameter applies only to a managed rule.
-        self.exclude_folder_ids_scope = exclude_folder_ids_scope
-        # The ID of the resource to be excluded from the compliance evaluations performed by the rule. Separate multiple resource IDs with commas (,).
+        # The ID of the resource group to which the rule applies. Separate multiple resource group IDs with commas (,).
         # 
         # >  This parameter applies only to a managed rule.
-        self.exclude_resource_ids_scope = exclude_resource_ids_scope
-        # The ID of the resource directory to which the rule applies, which means that the resources within member accounts in the resource directory are evaluated based on the rule.
-        # 
-        # > 
-        # *   This parameter applies only to a rule of a global account group.
-        # *   This parameter applies only to a managed rule.
-        self.folder_ids_scope = folder_ids_scope
-        # The input parameters of the rule.
-        self.input_parameters = input_parameters
+        self.client_token = client_token
         # The intervals at which the rule is triggered. Valid values:
         # 
         # *   One_Hour: 1 hour.
         # *   Three_Hours: 3 hours.
         # *   Six_Hours: 6 hours.
         # *   Twelve_Hours: 12 hours.
         # *   TwentyFour_Hours: 24 hours. This is the default value.
         # 
         # >  This parameter is required if the `ConfigRuleTriggerTypes` parameter is set to `ScheduledNotification`.
-        self.maximum_execution_frequency = maximum_execution_frequency
-        # The ID of the region to which the rule applies. Separate multiple region IDs with commas (,).
-        # 
-        # >  This parameter applies only to a managed rule.
-        self.region_ids_scope = region_ids_scope
-        # The ID of the resource group to which the rule applies. Separate multiple resource group IDs with commas (,).
-        # 
-        # >  This parameter applies only to a managed rule.
-        self.resource_group_ids_scope = resource_group_ids_scope
+        self.config_rule_name = config_rule_name
+        # The client token that is used to ensure the idempotence of the request. You can use the client to generate the value, but you must make sure that it is unique among different requests. The token can contain only ASCII characters and cannot exceed 64 characters in length.
+        self.config_rule_trigger_types = config_rule_trigger_types
         # The type of the resource to be evaluated by the rule. Separate multiple resource types with commas (,).
-        self.resource_types_scope = resource_types_scope
+        self.description = description
+        self.exclude_account_ids_scope = exclude_account_ids_scope
+        self.exclude_folder_ids_scope = exclude_folder_ids_scope
+        # The tag value used to filter resources. The rule applies only to the resources with the specified tag value.
+        # 
+        # >  This parameter applies only to a managed rule. You must set the `TagKeyScope` and `TagValueScope` parameters at the same time.
+        self.exclude_resource_ids_scope = exclude_resource_ids_scope
+        # The ID of the request.
+        self.folder_ids_scope = folder_ids_scope
         # The risk level of the resources that are not compliant with the rule. Valid values:
         # 
         # *   1: high risk level
         # *   2: medium risk level
         # *   3: low risk level
-        self.risk_level = risk_level
+        self.input_parameters = input_parameters
+        # The ID of the region to which the rule applies. Separate multiple region IDs with commas (,).
+        # 
+        # >  This parameter applies only to a managed rule.
+        self.maximum_execution_frequency = maximum_execution_frequency
+        # The tag key used to filter resources. The rule applies only to the resources with the specified tag key. Separate multiple parameter values with commas (,).
+        # 
+        # >  This parameter applies only to a managed rule. You must set the `TagKeyScope` and `TagValueScope` parameters at the same time.
+        self.region_ids_scope = region_ids_scope
         # The identifier of the rule.
         # 
         # *   If the SourceOwner parameter is set to ALIYUN, set this parameter to the name of the managed rule.
         # *   If the SourceOwner parameter is set to CUSTOM_FC, set this parameter to the Alibaba Cloud Resource Name (ARN) of the relevant function in Function Compute.
         # 
         # For more information about how to query the name of a managed rule, see [Managed rules](~~127404~~).
+        self.resource_group_ids_scope = resource_group_ids_scope
+        # The ID of the resource to be excluded from the compliance evaluations performed by the rule. Separate multiple resource IDs with commas (,).
+        # 
+        # >  This parameter applies only to a managed rule.
+        self.resource_types_scope = resource_types_scope
+        # The ID of the account group.
+        # 
+        # For more information about how to query the ID of an account group, see [ListAggregators](~~255797~~).
+        self.risk_level = risk_level
+        # The ID of the member account to which the rule does not apply, which means that the resources within the member account are not evaluated based on the rule. Separate multiple member account IDs with commas (,).
+        # 
+        # >  This parameter applies only to a managed rule.
         self.source_identifier = source_identifier
-        # The way in which the rule is to be created. Valid values:
+        # The ID of the resource directory to which the rule does not apply, which means that the resources within member accounts in the resource directory are not evaluated based on the rule. Separate multiple resource directory IDs with commas (,).
         # 
-        # *   ALIYUN: The rule is to be created based on a managed rule of Alibaba Cloud.
-        # *   CUSTOM_FC: The rule is a custom rule.
+        # > 
+        # *   This parameter applies only to a rule of a global account group.
+        # *   This parameter applies only to a managed rule.
         self.source_owner = source_owner
+        # The ID of the rule.
+        self.tag_key_logic_scope = tag_key_logic_scope
         # The logical relationship among the tag keys if you specify multiple tag keys by using the `TagKeyScope` parameter. For example, if you set the `TagKeyScope` parameter to `ECS,OSS` and set the TagKeyLogicScope parameter to `AND`, the rule applies to resources with both the `ECS` and `OSS` tag keys. Valid values:
         # 
         # *   AND: the logical relationship of AND
         # *   OR: the logical relationship of OR
-        self.tag_key_logic_scope = tag_key_logic_scope
-        # The tag key used to filter resources. The rule applies only to the resources with the specified tag key. Separate multiple parameter values with commas (,).
-        # 
-        # >  This parameter applies only to a managed rule. You must set the `TagKeyScope` and `TagValueScope` parameters at the same time.
         self.tag_key_scope = tag_key_scope
-        # The tag value used to filter resources. The rule applies only to the resources with the specified tag value.
+        # The ID of the resource directory to which the rule applies, which means that the resources within member accounts in the resource directory are evaluated based on the rule.
         # 
-        # >  This parameter applies only to a managed rule. You must set the `TagKeyScope` and `TagValueScope` parameters at the same time.
+        # > 
+        # *   This parameter applies only to a rule of a global account group.
+        # *   This parameter applies only to a managed rule.
         self.tag_value_scope = tag_value_scope
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1869,101 +1857,96 @@
         risk_level: int = None,
         source_identifier: str = None,
         source_owner: str = None,
         tag_key_logic_scope: str = None,
         tag_key_scope: str = None,
         tag_value_scope: str = None,
     ):
-        # The ID of the account group.
+        # The way in which the rule is to be created. Valid values:
         # 
-        # For more information about how to query the ID of an account group, see [ListAggregators](~~255797~~).
+        # *   ALIYUN: The rule is to be created based on a managed rule of Alibaba Cloud.
+        # *   CUSTOM_FC: The rule is a custom rule.
         self.aggregator_id = aggregator_id
-        # The client token that is used to ensure the idempotence of the request. You can use the client to generate the value, but you must make sure that it is unique among different requests. The token can contain only ASCII characters and cannot exceed 64 characters in length.
-        self.client_token = client_token
-        # The name of the rule.
-        self.config_rule_name = config_rule_name
-        # The trigger type of the rule. Valid values:
-        # 
-        # *   ConfigurationItemChangeNotification: The rule is triggered by configuration changes.
-        # *   ScheduledNotification: The rule is periodically triggered.
-        self.config_rule_trigger_types = config_rule_trigger_types
-        # The description of the rule.
-        self.description = description
-        # The ID of the member account to which the rule does not apply, which means that the resources within the member account are not evaluated based on the rule. Separate multiple member account IDs with commas (,).
-        # 
-        # >  This parameter applies only to a managed rule.
-        self.exclude_account_ids_scope = exclude_account_ids_scope
-        # The ID of the resource directory to which the rule does not apply, which means that the resources within member accounts in the resource directory are not evaluated based on the rule. Separate multiple resource directory IDs with commas (,).
-        # 
-        # > 
-        # *   This parameter applies only to a rule of a global account group.
-        # *   This parameter applies only to a managed rule.
-        self.exclude_folder_ids_scope = exclude_folder_ids_scope
-        # The ID of the resource to be excluded from the compliance evaluations performed by the rule. Separate multiple resource IDs with commas (,).
+        # The ID of the resource group to which the rule applies. Separate multiple resource group IDs with commas (,).
         # 
         # >  This parameter applies only to a managed rule.
-        self.exclude_resource_ids_scope = exclude_resource_ids_scope
-        # The ID of the resource directory to which the rule applies, which means that the resources within member accounts in the resource directory are evaluated based on the rule.
-        # 
-        # > 
-        # *   This parameter applies only to a rule of a global account group.
-        # *   This parameter applies only to a managed rule.
-        self.folder_ids_scope = folder_ids_scope
-        # The input parameters of the rule.
-        self.input_parameters_shrink = input_parameters_shrink
+        self.client_token = client_token
         # The intervals at which the rule is triggered. Valid values:
         # 
         # *   One_Hour: 1 hour.
         # *   Three_Hours: 3 hours.
         # *   Six_Hours: 6 hours.
         # *   Twelve_Hours: 12 hours.
         # *   TwentyFour_Hours: 24 hours. This is the default value.
         # 
         # >  This parameter is required if the `ConfigRuleTriggerTypes` parameter is set to `ScheduledNotification`.
-        self.maximum_execution_frequency = maximum_execution_frequency
-        # The ID of the region to which the rule applies. Separate multiple region IDs with commas (,).
-        # 
-        # >  This parameter applies only to a managed rule.
-        self.region_ids_scope = region_ids_scope
-        # The ID of the resource group to which the rule applies. Separate multiple resource group IDs with commas (,).
-        # 
-        # >  This parameter applies only to a managed rule.
-        self.resource_group_ids_scope = resource_group_ids_scope
+        self.config_rule_name = config_rule_name
+        # The client token that is used to ensure the idempotence of the request. You can use the client to generate the value, but you must make sure that it is unique among different requests. The token can contain only ASCII characters and cannot exceed 64 characters in length.
+        self.config_rule_trigger_types = config_rule_trigger_types
         # The type of the resource to be evaluated by the rule. Separate multiple resource types with commas (,).
-        self.resource_types_scope_shrink = resource_types_scope_shrink
+        self.description = description
+        self.exclude_account_ids_scope = exclude_account_ids_scope
+        self.exclude_folder_ids_scope = exclude_folder_ids_scope
+        # The tag value used to filter resources. The rule applies only to the resources with the specified tag value.
+        # 
+        # >  This parameter applies only to a managed rule. You must set the `TagKeyScope` and `TagValueScope` parameters at the same time.
+        self.exclude_resource_ids_scope = exclude_resource_ids_scope
+        # The ID of the request.
+        self.folder_ids_scope = folder_ids_scope
         # The risk level of the resources that are not compliant with the rule. Valid values:
         # 
         # *   1: high risk level
         # *   2: medium risk level
         # *   3: low risk level
-        self.risk_level = risk_level
+        self.input_parameters_shrink = input_parameters_shrink
+        # The ID of the region to which the rule applies. Separate multiple region IDs with commas (,).
+        # 
+        # >  This parameter applies only to a managed rule.
+        self.maximum_execution_frequency = maximum_execution_frequency
+        # The tag key used to filter resources. The rule applies only to the resources with the specified tag key. Separate multiple parameter values with commas (,).
+        # 
+        # >  This parameter applies only to a managed rule. You must set the `TagKeyScope` and `TagValueScope` parameters at the same time.
+        self.region_ids_scope = region_ids_scope
         # The identifier of the rule.
         # 
         # *   If the SourceOwner parameter is set to ALIYUN, set this parameter to the name of the managed rule.
         # *   If the SourceOwner parameter is set to CUSTOM_FC, set this parameter to the Alibaba Cloud Resource Name (ARN) of the relevant function in Function Compute.
         # 
         # For more information about how to query the name of a managed rule, see [Managed rules](~~127404~~).
+        self.resource_group_ids_scope = resource_group_ids_scope
+        # The ID of the resource to be excluded from the compliance evaluations performed by the rule. Separate multiple resource IDs with commas (,).
+        # 
+        # >  This parameter applies only to a managed rule.
+        self.resource_types_scope_shrink = resource_types_scope_shrink
+        # The ID of the account group.
+        # 
+        # For more information about how to query the ID of an account group, see [ListAggregators](~~255797~~).
+        self.risk_level = risk_level
+        # The ID of the member account to which the rule does not apply, which means that the resources within the member account are not evaluated based on the rule. Separate multiple member account IDs with commas (,).
+        # 
+        # >  This parameter applies only to a managed rule.
         self.source_identifier = source_identifier
-        # The way in which the rule is to be created. Valid values:
+        # The ID of the resource directory to which the rule does not apply, which means that the resources within member accounts in the resource directory are not evaluated based on the rule. Separate multiple resource directory IDs with commas (,).
         # 
-        # *   ALIYUN: The rule is to be created based on a managed rule of Alibaba Cloud.
-        # *   CUSTOM_FC: The rule is a custom rule.
+        # > 
+        # *   This parameter applies only to a rule of a global account group.
+        # *   This parameter applies only to a managed rule.
         self.source_owner = source_owner
+        # The ID of the rule.
+        self.tag_key_logic_scope = tag_key_logic_scope
         # The logical relationship among the tag keys if you specify multiple tag keys by using the `TagKeyScope` parameter. For example, if you set the `TagKeyScope` parameter to `ECS,OSS` and set the TagKeyLogicScope parameter to `AND`, the rule applies to resources with both the `ECS` and `OSS` tag keys. Valid values:
         # 
         # *   AND: the logical relationship of AND
         # *   OR: the logical relationship of OR
-        self.tag_key_logic_scope = tag_key_logic_scope
-        # The tag key used to filter resources. The rule applies only to the resources with the specified tag key. Separate multiple parameter values with commas (,).
-        # 
-        # >  This parameter applies only to a managed rule. You must set the `TagKeyScope` and `TagValueScope` parameters at the same time.
         self.tag_key_scope = tag_key_scope
-        # The tag value used to filter resources. The rule applies only to the resources with the specified tag value.
+        # The ID of the resource directory to which the rule applies, which means that the resources within member accounts in the resource directory are evaluated based on the rule.
         # 
-        # >  This parameter applies only to a managed rule. You must set the `TagKeyScope` and `TagValueScope` parameters at the same time.
+        # > 
+        # *   This parameter applies only to a rule of a global account group.
+        # *   This parameter applies only to a managed rule.
         self.tag_value_scope = tag_value_scope
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2060,17 +2043,15 @@
 
 class CreateAggregateConfigRuleResponseBody(TeaModel):
     def __init__(
         self,
         config_rule_id: str = None,
         request_id: str = None,
     ):
-        # The ID of the rule.
         self.config_rule_id = config_rule_id
-        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4061,21 +4042,17 @@
 
 class DeactiveAggregateConfigRulesRequest(TeaModel):
     def __init__(
         self,
         aggregator_id: str = None,
         config_rule_ids: str = None,
     ):
-        # The ID of the account group.
-        # 
-        # For more information about how to obtain the ID of an account group, see [ListAggregators](~~255797~~).
+        # The result of the operation to disable the rule.
         self.aggregator_id = aggregator_id
-        # The ID of the rule. Separate multiple rule IDs with commas (,).
-        # 
-        # For more information about how to obtain the ID of a rule, see [ListAggregateConfigRules](~~264148~~).
+        # The results of the operations to disable the specified rules.
         self.config_rule_ids = config_rule_ids
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4101,25 +4078,16 @@
 class DeactiveAggregateConfigRulesResponseBodyOperateRuleResultOperateRuleItemList(TeaModel):
     def __init__(
         self,
         config_rule_id: str = None,
         error_code: str = None,
         success: bool = None,
     ):
-        # The ID of the rule.
         self.config_rule_id = config_rule_id
-        # The error code returned.
-        # 
-        # *   If the rule is disabled, no error code is returned.
-        # *   If the rule fails to be disabled, an error code is returned. For more information about error codes, visit the [API Error Center](https://error-center.alibabacloud.com/status/product/Config).
         self.error_code = error_code
-        # Indicates whether the operation is successful. Valid values:
-        # 
-        # *   true: The operation is successful.
-        # *   false: The operation fails.
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4147,15 +4115,15 @@
 
 
 class DeactiveAggregateConfigRulesResponseBodyOperateRuleResult(TeaModel):
     def __init__(
         self,
         operate_rule_item_list: List[DeactiveAggregateConfigRulesResponseBodyOperateRuleResultOperateRuleItemList] = None,
     ):
-        # The result of the operation to disable the rule.
+        # The ID of the rule.
         self.operate_rule_item_list = operate_rule_item_list
 
     def validate(self):
         if self.operate_rule_item_list:
             for k in self.operate_rule_item_list:
                 if k:
                     k.validate()
@@ -4184,17 +4152,23 @@
 
 class DeactiveAggregateConfigRulesResponseBody(TeaModel):
     def __init__(
         self,
         operate_rule_result: DeactiveAggregateConfigRulesResponseBodyOperateRuleResult = None,
         request_id: str = None,
     ):
-        # The results of the operations to disable the specified rules.
+        # Indicates whether the operation is successful. Valid values:
+        # 
+        # *   true: The operation is successful.
+        # *   false: The operation fails.
         self.operate_rule_result = operate_rule_result
-        # The ID of the request.
+        # The error code returned.
+        # 
+        # *   If the rule is disabled, no error code is returned.
+        # *   If the rule fails to be disabled, an error code is returned. For more information about error codes, visit the [API Error Center](https://error-center.alibabacloud.com/status/product/Config).
         self.request_id = request_id
 
     def validate(self):
         if self.operate_rule_result:
             self.operate_rule_result.validate()
 
     def to_map(self):
@@ -5181,17 +5155,17 @@
 
 class DeleteAggregatorsRequest(TeaModel):
     def __init__(
         self,
         aggregator_ids: str = None,
         client_token: str = None,
     ):
-        # The ID of the account group. Separate multiple IDs with commas (,).
-        self.aggregator_ids = aggregator_ids
         # The client token that is used to ensure the idempotence of the request. You can use the client to generate the value, but you must ensure that it is unique among different requests. ClientToken can contain only ASCII characters and cannot exceed 64 characters in length.
+        self.aggregator_ids = aggregator_ids
+        # The ID of the request.
         self.client_token = client_token
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5217,24 +5191,21 @@
 class DeleteAggregatorsResponseBodyOperateAggregatorsResultOperateAggregators(TeaModel):
     def __init__(
         self,
         aggregator_id: str = None,
         error_code: str = None,
         success: bool = None,
     ):
-        # The ID of the account group.
         self.aggregator_id = aggregator_id
-        # The error code.
-        # 
-        # >  No error code is returned for the account group if the account group is deleted.
-        self.error_code = error_code
         # Indicates whether the delete operation is successful. Valid values:
         # 
         # *   true: The account group is deleted.
         # *   false: The account group fails to be deleted.
+        self.error_code = error_code
+        # The ID of the account group.
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5262,15 +5233,17 @@
 
 
 class DeleteAggregatorsResponseBodyOperateAggregatorsResult(TeaModel):
     def __init__(
         self,
         operate_aggregators: List[DeleteAggregatorsResponseBodyOperateAggregatorsResultOperateAggregators] = None,
     ):
-        # The result for the account group.
+        # The error code.
+        # 
+        # >  No error code is returned for the account group if the account group is deleted.
         self.operate_aggregators = operate_aggregators
 
     def validate(self):
         if self.operate_aggregators:
             for k in self.operate_aggregators:
                 if k:
                     k.validate()
@@ -5299,17 +5272,17 @@
 
 class DeleteAggregatorsResponseBody(TeaModel):
     def __init__(
         self,
         operate_aggregators_result: DeleteAggregatorsResponseBodyOperateAggregatorsResult = None,
         request_id: str = None,
     ):
-        # The results of the delete operations.
+        # The result for the account group.
         self.operate_aggregators_result = operate_aggregators_result
-        # The ID of the request.
+        # The results of the delete operations.
         self.request_id = request_id
 
     def validate(self):
         if self.operate_aggregators_result:
             self.operate_aggregators_result.validate()
 
     def to_map(self):
@@ -9629,31 +9602,23 @@
         aggregator_id: str = None,
         region: str = None,
         resource_account_id: int = None,
         resource_id: str = None,
         resource_owner_id: int = None,
         resource_type: str = None,
     ):
-        # The ID of the account group.
-        # 
-        # For more information about how to query the ID of an account group, see [ListAggregators](~~255797~~).
+        # The type of the resource.
         self.aggregator_id = aggregator_id
-        # The ID of the region in which the resource resides.
-        # 
-        # For more information about how to query the region ID of a resource, see [ListAggregateDiscoveredResources](~~411691~~).
+        # The ID of the zone in which the resource resides.
         self.region = region
         self.resource_account_id = resource_account_id
-        # The ID of the resource.
-        # 
-        # For more information about how to query the ID of a resource, see [ListAggregateDiscoveredResources](~~411691~~).
+        # The ID of the request.
         self.resource_id = resource_id
         self.resource_owner_id = resource_owner_id
-        # The type of the resource.
-        # 
-        # For more information about how to query the type of a resource, see [ListAggregateDiscoveredResources](~~411691~~).
+        # The information about the resource.
         self.resource_type = resource_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9703,41 +9668,37 @@
         resource_deleted: int = None,
         resource_id: str = None,
         resource_name: str = None,
         resource_status: str = None,
         resource_type: str = None,
         tags: str = None,
     ):
-        # The ID of the Alibaba Cloud account to which the resource belongs.
+        # The status of the resource. The parameter value varies based on the resource type and may be left empty. Examples:
+        # 
+        # *   If the value of the ResourceType parameter is ACS::ECS::Instance, the resource is an Elastic Compute Service (ECS) instance that has a specific state. In this case, the valid values of this parameter are Running and Stopped.
+        # *   If the value of the ResourceType parameter is ACS::OSS::Bucket, the resource is an Object Storage Service (OSS) bucket that does not have a specific state. In this case, this parameter is left empty.
         self.account_id = account_id
-        # The ID of the zone in which the resource resides.
+        # The timestamp when the resource was created.
         self.availability_zone = availability_zone
-        # The configuration of the resource.
+        # The ID of the Alibaba Cloud account to which the resource belongs.
         self.configuration = configuration
-        # The ID of the region in which the resource resides.
+        # The ID of the resource.
         self.region = region
-        # The timestamp when the resource was created.
-        self.resource_creation_time = resource_creation_time
         # Indicates whether the resource is deleted. Valid values:
         # 
         # *   1: The resource is retained.
         # *   0: The resource is deleted.
+        self.resource_creation_time = resource_creation_time
         self.resource_deleted = resource_deleted
-        # The ID of the resource.
         self.resource_id = resource_id
-        # The name of the resource.
         self.resource_name = resource_name
-        # The status of the resource. The parameter value varies based on the resource type and may be left empty. Examples:
-        # 
-        # *   If the value of the ResourceType parameter is ACS::ECS::Instance, the resource is an Elastic Compute Service (ECS) instance that has a specific state. In this case, the valid values of this parameter are Running and Stopped.
-        # *   If the value of the ResourceType parameter is ACS::OSS::Bucket, the resource is an Object Storage Service (OSS) bucket that does not have a specific state. In this case, this parameter is left empty.
         self.resource_status = resource_status
-        # The type of the resource.
-        self.resource_type = resource_type
         # The tags of the resource.
+        self.resource_type = resource_type
+        # The name of the resource.
         self.tags = tags
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9798,17 +9759,17 @@
 
 class GetAggregateDiscoveredResourceResponseBody(TeaModel):
     def __init__(
         self,
         discovered_resource_detail: GetAggregateDiscoveredResourceResponseBodyDiscoveredResourceDetail = None,
         request_id: str = None,
     ):
-        # The information about the resource.
+        # The ID of the region in which the resource resides.
         self.discovered_resource_detail = discovered_resource_detail
-        # The ID of the request.
+        # The configuration of the resource.
         self.request_id = request_id
 
     def validate(self):
         if self.discovered_resource_detail:
             self.discovered_resource_detail.validate()
 
     def to_map(self):
@@ -9882,28 +9843,24 @@
         self,
         aggregator_id: str = None,
         compliance_type: str = None,
         config_rule_id: str = None,
         resource_account_id: int = None,
         resource_owner_id: int = None,
     ):
-        # The ID of the account group.
-        # 
-        # For more information about how to query the ID of an account group, see [ListAggregators](~~255797~~).
-        self.aggregator_id = aggregator_id
         # The compliance evaluation result of the resources. Valid values:
         # 
         # *   COMPLIANT: The resources are evaluated as compliant.
         # *   NON_COMPLIANT: The resources are evaluated as non-compliant.
         # *   NOT_APPLICABLE: The rule does not apply to your resources.
         # *   INSUFFICIENT_DATA: No resource data is available.
+        self.aggregator_id = aggregator_id
+        # The total number of evaluated resources.
         self.compliance_type = compliance_type
-        # The ID of the rule.
-        # 
-        # For more information about how to query the ID of a rule, see [ListAggregateConfigRules](~~264148~~).
+        # The compliance evaluation results returned.
         self.config_rule_id = config_rule_id
         self.resource_account_id = resource_account_id
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
         pass
 
@@ -9942,22 +9899,15 @@
 
 class GetAggregateResourceComplianceByConfigRuleResponseBodyComplianceResultCompliances(TeaModel):
     def __init__(
         self,
         compliance_type: str = None,
         count: int = None,
     ):
-        # The compliance evaluation result of the resources. Valid values:
-        # 
-        # *   COMPLIANT: The resources are evaluated as compliant.
-        # *   NON_COMPLIANT: The resources are evaluated as non-compliant.
-        # *   NOT_APPLICABLE: The rule does not apply to your resources.
-        # *   INSUFFICIENT_DATA: No resource data is available.
         self.compliance_type = compliance_type
-        # The number of resources that have the compliance evaluation result. For example, if the value of the `ComplianceType` parameter is `COMPLIANT`, this parameter value indicates the number of compliant resources.
         self.count = count
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9982,17 +9932,16 @@
 
 class GetAggregateResourceComplianceByConfigRuleResponseBodyComplianceResult(TeaModel):
     def __init__(
         self,
         compliances: List[GetAggregateResourceComplianceByConfigRuleResponseBodyComplianceResultCompliances] = None,
         total_count: int = None,
     ):
-        # The compliance evaluation results returned.
         self.compliances = compliances
-        # The total number of evaluated resources.
+        # The ID of the request.
         self.total_count = total_count
 
     def validate(self):
         if self.compliances:
             for k in self.compliances:
                 if k:
                     k.validate()
@@ -10025,17 +9974,16 @@
 
 class GetAggregateResourceComplianceByConfigRuleResponseBody(TeaModel):
     def __init__(
         self,
         compliance_result: GetAggregateResourceComplianceByConfigRuleResponseBodyComplianceResult = None,
         request_id: str = None,
     ):
-        # The return result of the request.
+        # The number of resources that have the compliance evaluation result. For example, if the value of the `ComplianceType` parameter is `COMPLIANT`, this parameter value indicates the number of compliant resources.
         self.compliance_result = compliance_result
-        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.compliance_result:
             self.compliance_result.validate()
 
     def to_map(self):
@@ -10268,15 +10216,17 @@
 
 class GetAggregateResourceComplianceGroupByRegionRequest(TeaModel):
     def __init__(
         self,
         aggregator_id: str = None,
         config_rule_ids: str = None,
     ):
+        # The ID of the account group.
         self.aggregator_id = aggregator_id
+        # The rule IDs. Separate multiple rule IDs with commas (,).
         self.config_rule_ids = config_rule_ids
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -10301,15 +10251,22 @@
 
 class GetAggregateResourceComplianceGroupByRegionResponseBodyComplianceResultComplianceResultListCompliances(TeaModel):
     def __init__(
         self,
         compliance_type: str = None,
         count: int = None,
     ):
+        # The evaluation result. Valid values:
+        # 
+        # *   COMPLIANT: The resource is evaluated as compliant.
+        # *   NON_COMPLIANT: The resource is evaluated as non-compliant.
+        # *   NOT_APPLICABLE: The rule does not apply to the resource.
+        # *   INSUFFICIENT_DATA: No data is available.
         self.compliance_type = compliance_type
+        # The total number of evaluation results.
         self.count = count
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -10334,15 +10291,17 @@
 
 class GetAggregateResourceComplianceGroupByRegionResponseBodyComplianceResultComplianceResultList(TeaModel):
     def __init__(
         self,
         compliances: List[GetAggregateResourceComplianceGroupByRegionResponseBodyComplianceResultComplianceResultListCompliances] = None,
         region_id: str = None,
     ):
+        # The queried evaluation results.
         self.compliances = compliances
+        # The region ID of the evaluated resource.
         self.region_id = region_id
 
     def validate(self):
         if self.compliances:
             for k in self.compliances:
                 if k:
                     k.validate()
@@ -10374,14 +10333,15 @@
 
 
 class GetAggregateResourceComplianceGroupByRegionResponseBodyComplianceResult(TeaModel):
     def __init__(
         self,
         compliance_result_list: List[GetAggregateResourceComplianceGroupByRegionResponseBodyComplianceResultComplianceResultList] = None,
     ):
+        # The evaluation results grouped by region.
         self.compliance_result_list = compliance_result_list
 
     def validate(self):
         if self.compliance_result_list:
             for k in self.compliance_result_list:
                 if k:
                     k.validate()
@@ -10410,15 +10370,17 @@
 
 class GetAggregateResourceComplianceGroupByRegionResponseBody(TeaModel):
     def __init__(
         self,
         compliance_result: GetAggregateResourceComplianceGroupByRegionResponseBodyComplianceResult = None,
         request_id: str = None,
     ):
+        # The queried evaluation results.
         self.compliance_result = compliance_result
+        # The request ID.
         self.request_id = request_id
 
     def validate(self):
         if self.compliance_result:
             self.compliance_result.validate()
 
     def to_map(self):
@@ -10489,15 +10451,17 @@
 
 class GetAggregateResourceComplianceGroupByResourceTypeRequest(TeaModel):
     def __init__(
         self,
         aggregator_id: str = None,
         config_rule_ids: str = None,
     ):
+        # The ID of the account group.
         self.aggregator_id = aggregator_id
+        # The ID of the rule. Separate multiple rule IDs with commas (,).
         self.config_rule_ids = config_rule_ids
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -10522,15 +10486,22 @@
 
 class GetAggregateResourceComplianceGroupByResourceTypeResponseBodyComplianceResultComplianceResultListCompliances(TeaModel):
     def __init__(
         self,
         compliance_type: str = None,
         count: int = None,
     ):
+        # The evaluation result. Valid values:
+        # 
+        # *   COMPLIANT: The resource is evaluated as compliant.
+        # *   NON_COMPLIANT: The resource is evaluated as non-compliant.
+        # *   NOT_APPLICABLE: The rule does not apply to the resource.
+        # *   INSUFFICIENT_DATA: No data is available.
         self.compliance_type = compliance_type
+        # The number of statistical results.
         self.count = count
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -10555,15 +10526,17 @@
 
 class GetAggregateResourceComplianceGroupByResourceTypeResponseBodyComplianceResultComplianceResultList(TeaModel):
     def __init__(
         self,
         compliances: List[GetAggregateResourceComplianceGroupByResourceTypeResponseBodyComplianceResultComplianceResultListCompliances] = None,
         resource_type: str = None,
     ):
+        # The queried evaluation results.
         self.compliances = compliances
+        # The type of the evaluated resource.
         self.resource_type = resource_type
 
     def validate(self):
         if self.compliances:
             for k in self.compliances:
                 if k:
                     k.validate()
@@ -10595,14 +10568,15 @@
 
 
 class GetAggregateResourceComplianceGroupByResourceTypeResponseBodyComplianceResult(TeaModel):
     def __init__(
         self,
         compliance_result_list: List[GetAggregateResourceComplianceGroupByResourceTypeResponseBodyComplianceResultComplianceResultList] = None,
     ):
+        # The evaluation results grouped by resource type.
         self.compliance_result_list = compliance_result_list
 
     def validate(self):
         if self.compliance_result_list:
             for k in self.compliance_result_list:
                 if k:
                     k.validate()
@@ -10631,15 +10605,17 @@
 
 class GetAggregateResourceComplianceGroupByResourceTypeResponseBody(TeaModel):
     def __init__(
         self,
         compliance_result: GetAggregateResourceComplianceGroupByResourceTypeResponseBodyComplianceResult = None,
         request_id: str = None,
     ):
+        # The queried evaluation results.
         self.compliance_result = compliance_result
+        # The request ID.
         self.request_id = request_id
 
     def validate(self):
         if self.compliance_result:
             self.compliance_result.validate()
 
     def to_map(self):
@@ -10718,39 +10694,31 @@
         region: str = None,
         resource_account_id: int = None,
         resource_id: str = None,
         resource_owner_id: int = None,
         resource_type: str = None,
         start_time: int = None,
     ):
-        # The ID of the account group.
-        # 
-        # For more information about how to obtain the ID of an account group, see [ListAggregators](~~255797~~).
+        # The tags of the resource.
         self.aggregator_id = aggregator_id
-        # The timestamp that specifies the end of the time range to query. The default value indicates the time when the GetAggregateResourceComplianceTimeline operation is called. Unit: milliseconds.
+        # The maximum number of entries returned for a single request.
         self.end_time = end_time
-        # The maximum number of entries to return for a single request. Valid values: 1 to 100.
+        # The compliance evaluation records on the compliance timeline.
         self.max_results = max_results
-        # The token that is used to initiate the next request. If the response of the current request is truncated, this token is used to initiate another request and obtain the remaining entries.
+        # The ID of the zone in which the resource resides.
         self.next_token = next_token
-        # The ID of the region in which the resource resides.
-        # 
-        # For more information about how to obtain the ID of a region, see [ListAggregateDiscoveredResources](~~265983~~).
+        # The ID of the Alibaba Cloud account to which the resource belongs.
         self.region = region
         self.resource_account_id = resource_account_id
-        # The ID of the resource.
-        # 
-        # For more information about how to obtain the ID of a resource, see [ListAggregateDiscoveredResources](~~265983~~).
+        # The information about the compliance timeline.
         self.resource_id = resource_id
         self.resource_owner_id = resource_owner_id
-        # The type of the resource.
-        # 
-        # For more information about how to obtain the type of a resource, see [ListAggregateDiscoveredResources](~~265983~~).
+        # The ID of the request.
         self.resource_type = resource_type
-        # The timestamp that specifies the beginning of the time range to query. By default, Cloud Config retrieves the compliance evaluations in the last 30 days for the specified resource. Unit: milliseconds.
+        # The token that is used to initiate the next request.
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -10817,40 +10785,32 @@
         resource_create_time: int = None,
         resource_id: str = None,
         resource_name: str = None,
         resource_status: str = None,
         resource_type: str = None,
         tags: str = None,
     ):
-        # The ID of the Alibaba Cloud account to which the resource belongs.
+        # The ID of the resource.
         self.account_id = account_id
-        # The ID of the zone in which the resource resides.
+        # The name of the resource.
         self.availability_zone = availability_zone
-        # The timestamp when the compliance evaluation was recorded. Unit: milliseconds.
         self.capture_time = capture_time
-        # The information about the rules that evaluated the resource and the compliance evaluation result.
         self.configuration = configuration
-        # The details of the resource change that triggered the compliance evaluation.
         self.configuration_diff = configuration_diff
-        # The ID of the region in which the resource resides.
         self.region = region
-        # The timestamp when the resource was created. Unit: milliseconds.
         self.resource_create_time = resource_create_time
-        # The ID of the resource.
         self.resource_id = resource_id
-        # The name of the resource.
         self.resource_name = resource_name
+        self.resource_status = resource_status
         # The status of the resource. The parameter value varies based on the resource type and may be left empty. Examples:
         # 
         # *   If the ResourceType parameter is set to ACS::ECS::Instance, the resource is an Elastic Compute Service (ECS) instance that has a specific state. In this case, the valid values of this parameter are Running and Stopped.
         # *   If the ResourceType parameter is set to ACS::OSS::Bucket, the resource is an OSS bucket that does not have a specific state. In this case, this parameter is left empty.
-        self.resource_status = resource_status
-        # The type of the resource.
         self.resource_type = resource_type
-        # The tags of the resource.
+        # The details of the resource change that triggered the compliance evaluation.
         self.tags = tags
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -10916,19 +10876,19 @@
 class GetAggregateResourceComplianceTimelineResponseBodyResourceComplianceTimeline(TeaModel):
     def __init__(
         self,
         compliance_list: List[GetAggregateResourceComplianceTimelineResponseBodyResourceComplianceTimelineComplianceList] = None,
         max_results: int = None,
         next_token: str = None,
     ):
-        # The compliance evaluation records on the compliance timeline.
+        # The timestamp when the compliance evaluation was recorded. Unit: milliseconds.
         self.compliance_list = compliance_list
-        # The maximum number of entries returned for a single request.
+        # The information about the rules that evaluated the resource and the compliance evaluation result.
         self.max_results = max_results
-        # The token that is used to initiate the next request.
+        # The ID of the region in which the resource resides.
         self.next_token = next_token
 
     def validate(self):
         if self.compliance_list:
             for k in self.compliance_list:
                 if k:
                     k.validate()
@@ -10965,17 +10925,17 @@
 
 class GetAggregateResourceComplianceTimelineResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         resource_compliance_timeline: GetAggregateResourceComplianceTimelineResponseBodyResourceComplianceTimeline = None,
     ):
-        # The ID of the request.
+        # The type of the resource.
         self.request_id = request_id
-        # The information about the compliance timeline.
+        # The timestamp when the resource was created. Unit: milliseconds.
         self.resource_compliance_timeline = resource_compliance_timeline
 
     def validate(self):
         if self.resource_compliance_timeline:
             self.resource_compliance_timeline.validate()
 
     def to_map(self):
@@ -11054,39 +11014,33 @@
         region: str = None,
         resource_account_id: int = None,
         resource_id: str = None,
         resource_owner_id: int = None,
         resource_type: str = None,
         start_time: int = None,
     ):
-        # The ID of the account group.
-        # 
-        # For more information about how to obtain the ID of an account group, see [ListAggregators](~~255797~~).
+        # The configuration changes on the configuration timeline.
         self.aggregator_id = aggregator_id
-        # The timestamp that specifies the end of the time range to query. The default value indicates the time when the GetAggregateResourceConfigurationTimeline operation is called. Unit: milliseconds.
+        # The ID of the request.
         self.end_time = end_time
-        # The maximum number of entries to return for a single request. Valid values: 1 to 100.
+        # The information about the configuration timeline.
         self.max_results = max_results
-        # The token that is used to initiate the next request. If the response of the current request is truncated, this token is used to initiate another request and obtain the remaining entries.
+        # The tags of the resource.
         self.next_token = next_token
-        # The ID of the region in which the resource resides.
-        # 
-        # For more information about how to obtain the ID of a region, see [ListAggregateDiscoveredResources](~~265983~~).
+        # The maximum number of entries returned for a single request.
         self.region = region
         self.resource_account_id = resource_account_id
-        # The ID of the resource.
+        # The ID of the account group.
         # 
-        # For more information about how to obtain the ID of a resource, see [ListAggregateDiscoveredResources](~~265983~~).
+        # For more information about how to obtain the ID of an account group, see [ListAggregators](~~255797~~).
         self.resource_id = resource_id
         self.resource_owner_id = resource_owner_id
-        # The type of the resource.
-        # 
-        # For more information about how to obtain the type of a resource, see [ListAggregateDiscoveredResources](~~265983~~).
+        # The token that is used to initiate the next request.
         self.resource_type = resource_type
-        # The timestamp that specifies the beginning of the time range to query. By default, Cloud Config retrieves the configuration changes in the last 30 days for the specified resource. Unit: milliseconds.
+        # The token that is used to initiate the next request. If the response of the current request is truncated, this token is used to initiate another request and obtain the remaining entries.
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -11152,45 +11106,29 @@
         resource_create_time: str = None,
         resource_event_type: str = None,
         resource_id: str = None,
         resource_name: str = None,
         resource_type: str = None,
         tags: str = None,
     ):
-        # The ID of the Alibaba Cloud account to which the resource belongs.
+        # The timestamp when the resource change snapshot was recorded. Unit: milliseconds.
         self.account_id = account_id
-        # The ID of the zone in which the resource resides.
+        # The ID of the resource.
         self.availability_zone = availability_zone
-        # The timestamp when the resource change snapshot was recorded. Unit: milliseconds.
         self.capture_time = capture_time
-        # The details of the resource change that triggered the compliance evaluation.
         self.configuration_diff = configuration_diff
-        # The ID of the region in which the resource resides.
         self.region = region
-        # The timestamp when the resource was created. Unit: milliseconds.
         self.resource_create_time = resource_create_time
-        # The type of the resource change event involved. Valid values:
-        # 
-        # *   DISCOVERED: A resource is created.
-        # *   DISCOVERED_REVISED: A resource is created by periodic remediation tasks.
-        # *   MODIFY: A resource is modified.
-        # *   MODIFY_REVISED: A resource is modified by periodic remediation tasks.
-        # *   REMOVE: A resource is deleted.
-        # 
-        # > 
-        # *   To ensure the integrity of resources, periodic remediation tasks are run to check data and generate events that indicate the creation of new resources. Such events are infrequent.
-        # *   The time when a resource change event is generated by a periodic remediation task is considered as the detection time of Cloud Config. The detection time is later than the time when the resource is modified.
+        # The details of the resource change that triggered the compliance evaluation.
         self.resource_event_type = resource_event_type
-        # The ID of the resource.
         self.resource_id = resource_id
-        # The name of the resource.
         self.resource_name = resource_name
-        # The type of the resource.
+        # The name of the resource.
         self.resource_type = resource_type
-        # The tags of the resource.
+        # The ID of the region in which the resource resides.
         self.tags = tags
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -11252,19 +11190,19 @@
 class GetAggregateResourceConfigurationTimelineResponseBodyResourceConfigurationTimeline(TeaModel):
     def __init__(
         self,
         configuration_list: List[GetAggregateResourceConfigurationTimelineResponseBodyResourceConfigurationTimelineConfigurationList] = None,
         max_results: int = None,
         next_token: str = None,
     ):
-        # The configuration changes on the configuration timeline.
+        # The timestamp when the resource was created. Unit: milliseconds.
         self.configuration_list = configuration_list
-        # The maximum number of entries returned for a single request.
+        # The type of the resource.
         self.max_results = max_results
-        # The token that is used to initiate the next request.
+        # The ID of the zone in which the resource resides.
         self.next_token = next_token
 
     def validate(self):
         if self.configuration_list:
             for k in self.configuration_list:
                 if k:
                     k.validate()
@@ -11301,17 +11239,27 @@
 
 class GetAggregateResourceConfigurationTimelineResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         resource_configuration_timeline: GetAggregateResourceConfigurationTimelineResponseBodyResourceConfigurationTimeline = None,
     ):
-        # The ID of the request.
+        # The ID of the Alibaba Cloud account to which the resource belongs.
         self.request_id = request_id
-        # The information about the configuration timeline.
+        # The type of the resource change event involved. Valid values:
+        # 
+        # *   DISCOVERED: A resource is created.
+        # *   DISCOVERED_REVISED: A resource is created by periodic remediation tasks.
+        # *   MODIFY: A resource is modified.
+        # *   MODIFY_REVISED: A resource is modified by periodic remediation tasks.
+        # *   REMOVE: A resource is deleted.
+        # 
+        # > 
+        # *   To ensure the integrity of resources, periodic remediation tasks are run to check data and generate events that indicate the creation of new resources. Such events are infrequent.
+        # *   The time when a resource change event is generated by a periodic remediation task is considered as the detection time of Cloud Config. The detection time is later than the time when the resource is modified.
         self.resource_configuration_timeline = resource_configuration_timeline
 
     def validate(self):
         if self.resource_configuration_timeline:
             self.resource_configuration_timeline.validate()
 
     def to_map(self):
@@ -11385,25 +11333,23 @@
         self,
         aggregator_id: str = None,
         folder_id: str = None,
         resource_account_id: int = None,
         resource_owner_id: int = None,
         resource_type: str = None,
     ):
-        # The ID of the account group.
-        # 
-        # For more information about how to obtain the ID of an account group, see [ListAggregators](~~255797~~).
+        # The total number of resources in the region.
         self.aggregator_id = aggregator_id
-        # The ID of the folder in the resource directory. For more information about how to obtain the ID of a folder, see [View the basic information of a folder](~~111223~~).
+        # The dimension by which statistics are collected.
+        # 
+        # >  In most cases, the `Region` parameter is returned instead of the GroupName parameter.
         self.folder_id = folder_id
         self.resource_account_id = resource_account_id
         self.resource_owner_id = resource_owner_id
-        # The type of the resource.
-        # 
-        # For more information about how to obtain the type of a resource, see [ListAggregateDiscoveredResources](~~265983~~).
+        # The statistics on resources.
         self.resource_type = resource_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -11441,21 +11387,16 @@
 class GetAggregateResourceCountsGroupByRegionResponseBodyDiscoveredResourceCountsSummary(TeaModel):
     def __init__(
         self,
         group_name: str = None,
         region: str = None,
         resource_count: int = None,
     ):
-        # The dimension by which statistics are collected.
-        # 
-        # >  In most cases, the `Region` parameter is returned instead of the GroupName parameter.
         self.group_name = group_name
-        # The ID of the region by which statistics are collected.
         self.region = region
-        # The total number of resources in the region.
         self.resource_count = resource_count
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -11484,17 +11425,16 @@
 
 class GetAggregateResourceCountsGroupByRegionResponseBody(TeaModel):
     def __init__(
         self,
         discovered_resource_counts_summary: List[GetAggregateResourceCountsGroupByRegionResponseBodyDiscoveredResourceCountsSummary] = None,
         request_id: str = None,
     ):
-        # The statistics on resources.
         self.discovered_resource_counts_summary = discovered_resource_counts_summary
-        # The ID of the request.
+        # The ID of the region by which statistics are collected.
         self.request_id = request_id
 
     def validate(self):
         if self.discovered_resource_counts_summary:
             for k in self.discovered_resource_counts_summary:
                 if k:
                     k.validate()
@@ -13176,14 +13116,41 @@
         if m.get('SourceDetails') is not None:
             for k in m.get('SourceDetails'):
                 temp_model = GetConfigRuleResponseBodyConfigRuleManagedRuleSourceDetails()
                 self.source_details.append(temp_model.from_map(k))
         return self
 
 
+class GetConfigRuleResponseBodyConfigRuleScope(TeaModel):
+    def __init__(
+        self,
+        compliance_resource_types: List[str] = None,
+    ):
+        self.compliance_resource_types = compliance_resource_types
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.compliance_resource_types is not None:
+            result['ComplianceResourceTypes'] = self.compliance_resource_types
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ComplianceResourceTypes') is not None:
+            self.compliance_resource_types = m.get('ComplianceResourceTypes')
+        return self
+
+
 class GetConfigRuleResponseBodyConfigRuleSourceSourceDetails(TeaModel):
     def __init__(
         self,
         event_source: str = None,
         maximum_execution_frequency: str = None,
         message_type: str = None,
     ):
@@ -13310,14 +13277,15 @@
         managed_rule: GetConfigRuleResponseBodyConfigRuleManagedRule = None,
         maximum_execution_frequency: str = None,
         modified_timestamp: int = None,
         region_ids_scope: str = None,
         resource_group_ids_scope: str = None,
         resource_types_scope: str = None,
         risk_level: int = None,
+        scope: GetConfigRuleResponseBodyConfigRuleScope = None,
         source: GetConfigRuleResponseBodyConfigRuleSource = None,
         tag_key_logic_scope: str = None,
         tag_key_scope: str = None,
         tag_value_scope: str = None,
     ):
         # The ID of the Alibaba Cloud account to which the rule belongs.
         self.account_id = account_id
@@ -13375,14 +13343,15 @@
         self.resource_types_scope = resource_types_scope
         # The risk level of the resources that are not compliant with the rule. Valid values:
         # 
         # *   1: high risk level
         # *   2: medium risk level
         # *   3: low risk level
         self.risk_level = risk_level
+        self.scope = scope
         # The information about how the rule was created.
         self.source = source
         # The ID of the member account to which the rule does not apply, which means that the resources within the member account are not evaluated based on the rule.
         # 
         # >  This parameter applies only to managed rules.
         self.tag_key_logic_scope = tag_key_logic_scope
         # The tag value used to filter resources. The rule applies only to the resources with the specified tag value.
@@ -13399,14 +13368,16 @@
             self.compliance.validate()
         if self.config_rule_evaluation_status:
             self.config_rule_evaluation_status.validate()
         if self.create_by:
             self.create_by.validate()
         if self.managed_rule:
             self.managed_rule.validate()
+        if self.scope:
+            self.scope.validate()
         if self.source:
             self.source.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -13448,14 +13419,16 @@
             result['RegionIdsScope'] = self.region_ids_scope
         if self.resource_group_ids_scope is not None:
             result['ResourceGroupIdsScope'] = self.resource_group_ids_scope
         if self.resource_types_scope is not None:
             result['ResourceTypesScope'] = self.resource_types_scope
         if self.risk_level is not None:
             result['RiskLevel'] = self.risk_level
+        if self.scope is not None:
+            result['Scope'] = self.scope.to_map()
         if self.source is not None:
             result['Source'] = self.source.to_map()
         if self.tag_key_logic_scope is not None:
             result['TagKeyLogicScope'] = self.tag_key_logic_scope
         if self.tag_key_scope is not None:
             result['TagKeyScope'] = self.tag_key_scope
         if self.tag_value_scope is not None:
@@ -13504,14 +13477,17 @@
             self.region_ids_scope = m.get('RegionIdsScope')
         if m.get('ResourceGroupIdsScope') is not None:
             self.resource_group_ids_scope = m.get('ResourceGroupIdsScope')
         if m.get('ResourceTypesScope') is not None:
             self.resource_types_scope = m.get('ResourceTypesScope')
         if m.get('RiskLevel') is not None:
             self.risk_level = m.get('RiskLevel')
+        if m.get('Scope') is not None:
+            temp_model = GetConfigRuleResponseBodyConfigRuleScope()
+            self.scope = temp_model.from_map(m['Scope'])
         if m.get('Source') is not None:
             temp_model = GetConfigRuleResponseBodyConfigRuleSource()
             self.source = temp_model.from_map(m['Source'])
         if m.get('TagKeyLogicScope') is not None:
             self.tag_key_logic_scope = m.get('TagKeyLogicScope')
         if m.get('TagKeyScope') is not None:
             self.tag_key_scope = m.get('TagKeyScope')
@@ -14708,15 +14684,15 @@
         request_id: str = None,
     ):
         # Indicates whether the product has been integrated. Valid values:
         # 
         # *   true
         # *   false
         self.data = data
-        # The ID of the request.
+        # The request ID.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -15432,14 +15408,15 @@
 
 
 class GetResourceComplianceGroupByRegionRequest(TeaModel):
     def __init__(
         self,
         config_rule_ids: str = None,
     ):
+        # The rule IDs. Separate multiple rule IDs with commas (,).
         self.config_rule_ids = config_rule_ids
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -15460,15 +15437,22 @@
 
 class GetResourceComplianceGroupByRegionResponseBodyComplianceResultComplianceResultListCompliances(TeaModel):
     def __init__(
         self,
         compliance_type: str = None,
         count: int = None,
     ):
+        # The evaluation result. Valid values:
+        # 
+        # *   COMPLIANT: The resource is evaluated as compliant.
+        # *   NON_COMPLIANT: The resource is evaluated as non-compliant.
+        # *   NOT_APPLICABLE: The rule does not apply to the resource.
+        # *   INSUFFICIENT_DATA: No data is available.
         self.compliance_type = compliance_type
+        # The total number of evaluation results.
         self.count = count
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -15493,15 +15477,17 @@
 
 class GetResourceComplianceGroupByRegionResponseBodyComplianceResultComplianceResultList(TeaModel):
     def __init__(
         self,
         compliances: List[GetResourceComplianceGroupByRegionResponseBodyComplianceResultComplianceResultListCompliances] = None,
         region_id: str = None,
     ):
+        # The queried evaluation results.
         self.compliances = compliances
+        # The region ID of the evaluated resource.
         self.region_id = region_id
 
     def validate(self):
         if self.compliances:
             for k in self.compliances:
                 if k:
                     k.validate()
@@ -15533,14 +15519,15 @@
 
 
 class GetResourceComplianceGroupByRegionResponseBodyComplianceResult(TeaModel):
     def __init__(
         self,
         compliance_result_list: List[GetResourceComplianceGroupByRegionResponseBodyComplianceResultComplianceResultList] = None,
     ):
+        # The evaluation results grouped by region.
         self.compliance_result_list = compliance_result_list
 
     def validate(self):
         if self.compliance_result_list:
             for k in self.compliance_result_list:
                 if k:
                     k.validate()
@@ -15569,15 +15556,17 @@
 
 class GetResourceComplianceGroupByRegionResponseBody(TeaModel):
     def __init__(
         self,
         compliance_result: GetResourceComplianceGroupByRegionResponseBodyComplianceResult = None,
         request_id: str = None,
     ):
+        # The queried evaluation results.
         self.compliance_result = compliance_result
+        # The request ID.
         self.request_id = request_id
 
     def validate(self):
         if self.compliance_result:
             self.compliance_result.validate()
 
     def to_map(self):
@@ -15647,14 +15636,15 @@
 
 
 class GetResourceComplianceGroupByResourceTypeRequest(TeaModel):
     def __init__(
         self,
         config_rule_ids: str = None,
     ):
+        # The rule IDs. Separate multiple rule IDs with commas (,).
         self.config_rule_ids = config_rule_ids
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -15675,15 +15665,22 @@
 
 class GetResourceComplianceGroupByResourceTypeResponseBodyComplianceResultComplianceResultListCompliances(TeaModel):
     def __init__(
         self,
         compliance_type: str = None,
         count: int = None,
     ):
+        # The evaluation result. Valid values:
+        # 
+        # *   COMPLIANT: The resource is evaluated as compliant.
+        # *   NON_COMPLIANT: The resource is evaluated as non-compliant.
+        # *   NOT_APPLICABLE: The rule does not apply to the resource.
+        # *   INSUFFICIENT_DATA: No data is available.
         self.compliance_type = compliance_type
+        # The total number of evaluation results.
         self.count = count
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -15708,15 +15705,17 @@
 
 class GetResourceComplianceGroupByResourceTypeResponseBodyComplianceResultComplianceResultList(TeaModel):
     def __init__(
         self,
         compliances: List[GetResourceComplianceGroupByResourceTypeResponseBodyComplianceResultComplianceResultListCompliances] = None,
         resource_type: str = None,
     ):
+        # The queried evaluation results.
         self.compliances = compliances
+        # The type of the evaluated resource.
         self.resource_type = resource_type
 
     def validate(self):
         if self.compliances:
             for k in self.compliances:
                 if k:
                     k.validate()
@@ -15748,14 +15747,15 @@
 
 
 class GetResourceComplianceGroupByResourceTypeResponseBodyComplianceResult(TeaModel):
     def __init__(
         self,
         compliance_result_list: List[GetResourceComplianceGroupByResourceTypeResponseBodyComplianceResultComplianceResultList] = None,
     ):
+        # The evaluation results grouped by resource type.
         self.compliance_result_list = compliance_result_list
 
     def validate(self):
         if self.compliance_result_list:
             for k in self.compliance_result_list:
                 if k:
                     k.validate()
@@ -15784,15 +15784,17 @@
 
 class GetResourceComplianceGroupByResourceTypeResponseBody(TeaModel):
     def __init__(
         self,
         compliance_result: GetResourceComplianceGroupByResourceTypeResponseBodyComplianceResult = None,
         request_id: str = None,
     ):
+        # The queried evaluation results.
         self.compliance_result = compliance_result
+        # The request ID.
         self.request_id = request_id
 
     def validate(self):
         if self.compliance_result:
             self.compliance_result.validate()
 
     def to_map(self):
@@ -16181,31 +16183,29 @@
         max_results: int = None,
         next_token: str = None,
         region: str = None,
         resource_id: str = None,
         resource_type: str = None,
         start_time: int = None,
     ):
-        # The timestamp that specifies the end of the time range to query. The default value is the time when the GetResourceConfigurationTimeline operation is called. Unit: milliseconds.
+        # The token that is used to initiate the next request. If the response of the current request is truncated, this token is used to initiate another request and obtain the remaining entries.
         self.end_time = end_time
-        # The maximum number of entries to return for a single request. Valid values: 1 to 100.
+        # The ID of the request.
         self.max_results = max_results
-        # The token that is used to initiate the next request. If the response of the current request is truncated, this token is used to initiate another request and obtain the remaining entries.
+        # The maximum number of entries returned for a single request.
         self.next_token = next_token
-        # The ID of the region in which the resource resides.
+        # The token that is used to initiate the next request.
         self.region = region
-        # The ID of the resource.
-        # 
-        # For more information about how to obtain the ID of a resource, see [ListDiscoveredResources](~~169620~~).
-        self.resource_id = resource_id
         # The type of the resource.
         # 
         # For more information about how to obtain the type of a resource, see [ListDiscoveredResources](~~169620~~).
+        self.resource_id = resource_id
+        # The information about the configuration timeline.
         self.resource_type = resource_type
-        # The timestamp that specifies the beginning of the time range to query. By default, Cloud Config retrieves the configuration changes in the last 30 days for the specified resource. Unit: milliseconds.
+        # The ID of the region in which the resource resides.
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -16261,49 +16261,35 @@
         resource_create_time: str = None,
         resource_event_type: str = None,
         resource_id: str = None,
         resource_name: str = None,
         resource_type: str = None,
         tags: str = None,
     ):
-        # The ID of the Alibaba Cloud account to which the resource belongs.
+        # The timestamp when the resource was created. Unit: milliseconds.
         self.account_id = account_id
-        # The ID of the zone.
-        self.availability_zone = availability_zone
         # The timestamp when the resource change snapshot was recorded. Unit: milliseconds.
+        self.availability_zone = availability_zone
+        # The details of each resource that is associated with the current resource, including the region ID, resource relationship, resource ID, and resource type.
         self.capture_time = capture_time
-        # The details of the resource change that triggered the compliance evaluation.
+        # The change records of the resource relationship.
         self.configuration_diff = configuration_diff
-        # The ID of the region in which the resource resides.
+        # The name of the resource.
         self.region = region
-        # The details of each resource that is associated with the current resource, including the region ID, resource relationship, resource ID, and resource type.
         self.relationship = relationship
-        # The change records of the resource relationship.
         self.relationship_diff = relationship_diff
-        # The timestamp when the resource was created. Unit: milliseconds.
+        # The ID of the resource.
         self.resource_create_time = resource_create_time
-        # The type of the resource change event involved. Valid values:
-        # 
-        # *   DISCOVERED: A resource is created.
-        # *   DISCOVERED_REVISED: A resource is created by periodic remediation tasks.
-        # *   MODIFY: A resource is modified.
-        # *   MODIFY_REVISED: A resource is modified by periodic remediation tasks.
-        # *   REMOVE: A resource is deleted.
-        # 
-        # > 
-        # *   To ensure the integrity of resources, periodic remediation tasks are executed to check data and generate events that indicate the creation of new resources. Such events are infrequent.
-        # *   The time when a resource change event is generated by a periodic remediation task is considered as the detection time of Cloud Config. The detection time is later than the time when the resource is modified.
+        # The ID of the region in which the resource resides.
         self.resource_event_type = resource_event_type
-        # The ID of the resource.
         self.resource_id = resource_id
-        # The name of the resource.
         self.resource_name = resource_name
-        # The type of the resource.
+        # The details of the resource change that triggered the compliance evaluation.
         self.resource_type = resource_type
-        # The tags of the resource.
+        # The type of the resource.
         self.tags = tags
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -16373,19 +16359,29 @@
 class GetResourceConfigurationTimelineResponseBodyResourceConfigurationTimeline(TeaModel):
     def __init__(
         self,
         configuration_list: List[GetResourceConfigurationTimelineResponseBodyResourceConfigurationTimelineConfigurationList] = None,
         max_results: int = None,
         next_token: str = None,
     ):
-        # The configuration changes on the configuration timeline.
+        # The ID of the zone.
         self.configuration_list = configuration_list
-        # The maximum number of entries returned for a single request.
+        # The type of the resource change event involved. Valid values:
+        # 
+        # *   DISCOVERED: A resource is created.
+        # *   DISCOVERED_REVISED: A resource is created by periodic remediation tasks.
+        # *   MODIFY: A resource is modified.
+        # *   MODIFY_REVISED: A resource is modified by periodic remediation tasks.
+        # *   REMOVE: A resource is deleted.
+        # 
+        # > 
+        # *   To ensure the integrity of resources, periodic remediation tasks are executed to check data and generate events that indicate the creation of new resources. Such events are infrequent.
+        # *   The time when a resource change event is generated by a periodic remediation task is considered as the detection time of Cloud Config. The detection time is later than the time when the resource is modified.
         self.max_results = max_results
-        # The token that is used to initiate the next request.
+        # The ID of the Alibaba Cloud account to which the resource belongs.
         self.next_token = next_token
 
     def validate(self):
         if self.configuration_list:
             for k in self.configuration_list:
                 if k:
                     k.validate()
@@ -16422,17 +16418,17 @@
 
 class GetResourceConfigurationTimelineResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         resource_configuration_timeline: GetResourceConfigurationTimelineResponseBodyResourceConfigurationTimeline = None,
     ):
-        # The ID of the request.
+        # The configuration changes on the configuration timeline.
         self.request_id = request_id
-        # The information about the configuration timeline.
+        # The tags of the resource.
         self.resource_configuration_timeline = resource_configuration_timeline
 
     def validate(self):
         if self.resource_configuration_timeline:
             self.resource_configuration_timeline.validate()
 
     def to_map(self):
@@ -18584,34 +18580,31 @@
         regions: str = None,
         resource_account_id: int = None,
         resource_deleted: int = None,
         resource_id: str = None,
         resource_owner_id: int = None,
         resource_types: str = None,
     ):
-        # The ID of the account group.
-        # 
-        # For more information about how to obtain the ID of an account group, see [ListAggregators](~~255797~~).
+        # The tags of the resource.
         self.aggregator_id = aggregator_id
-        # The maximum number of entries to return for a single request. Valid values: 1 to 100.
+        # The information about resources.
         self.max_results = max_results
-        # The token that you want to use to initiate the current request. If the response of the previous request is truncated, you can use this token to initiate another request and obtain the remaining entries.``
+        # The type of the resource.
         self.next_token = next_token
-        # The ID of the region where the resource resides. Separate multiple region IDs with commas (,).
+        # The timestamp when the resource was created. Unit: milliseconds.
         self.regions = regions
         self.resource_account_id = resource_account_id
-        # Indicates whether the resource is deleted. Valid values:
-        # 
-        # *   0: The resource is deleted.
-        # *   1: The resource is retained. This is the default value.
+        # The return result of the request.
         self.resource_deleted = resource_deleted
-        # The ID of the resource.
+        # The ID of the account group.
+        # 
+        # For more information about how to obtain the ID of an account group, see [ListAggregators](~~255797~~).
         self.resource_id = resource_id
         self.resource_owner_id = resource_owner_id
-        # The type of the resource. Separate multiple resource types with commas (,).
+        # The region ID.
         self.resource_types = resource_types
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -18674,43 +18667,41 @@
         resource_name: str = None,
         resource_owner_id: int = None,
         resource_status: str = None,
         resource_type: str = None,
         tags: str = None,
         version: int = None,
     ):
-        # The ID of the Alibaba Cloud account to which the resource belongs.
+        # The build version of the resource.
         self.account_id = account_id
-        # The ID of the zone where the resource resides.
         self.availability_zone = availability_zone
-        # The region ID.
-        self.region = region
-        # The timestamp when the resource was created. Unit: milliseconds.
-        self.resource_creation_time = resource_creation_time
         # Indicates whether the resource is deleted. Valid values:
         # 
         # *   0: The resource is deleted.
         # *   1: The resource is retained.
-        self.resource_deleted = resource_deleted
-        # The ID of the resource.
-        self.resource_id = resource_id
-        # The name of the resource.
-        self.resource_name = resource_name
-        # The ID of the Alibaba Cloud account to which the resources belong.
-        self.resource_owner_id = resource_owner_id
+        self.region = region
         # Indicates whether the resource is deleted. The value of this parameter varies based on the resource type and may be left empty. Example:
         # 
         # *   If the value of the ResourceType parameter is ACS::ECS::Instance, the resource is an Elastic Compute Service (ECS) instance that is in a specific state. In this case, the valid values of this parameter are Running and Stopped.
         # *   If the value of the ResourceType parameter is ACS::OSS::Bucket, the resource is an Object Storage Service (OSS) bucket that is not in a specific state. In this case, this parameter is left empty.
+        self.resource_creation_time = resource_creation_time
+        # The maximum number of entries returned on each page.
+        self.resource_deleted = resource_deleted
+        # The ID of the zone where the resource resides.
+        self.resource_id = resource_id
+        # The token that was used to initiate the next request.
+        self.resource_name = resource_name
+        # The ID of the request.
+        self.resource_owner_id = resource_owner_id
+        # The total number of resources.
         self.resource_status = resource_status
-        # The type of the resource.
+        # The name of the resource.
         self.resource_type = resource_type
-        # The tags of the resource.
+        # The ID of the Alibaba Cloud account to which the resources belong.
         self.tags = tags
-        # The build version of the resource.
         self.version = version
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -18777,21 +18768,18 @@
     def __init__(
         self,
         discovered_resource_profile_list: List[ListAggregateDiscoveredResourcesResponseBodyDiscoveredResourceProfilesDiscoveredResourceProfileList] = None,
         max_results: int = None,
         next_token: str = None,
         total_count: int = None,
     ):
-        # The information about resources.
+        # The ID of the resource.
         self.discovered_resource_profile_list = discovered_resource_profile_list
-        # The maximum number of entries returned on each page.
         self.max_results = max_results
-        # The token that was used to initiate the next request.
         self.next_token = next_token
-        # The total number of resources.
         self.total_count = total_count
 
     def validate(self):
         if self.discovered_resource_profile_list:
             for k in self.discovered_resource_profile_list:
                 if k:
                     k.validate()
@@ -18832,17 +18820,16 @@
 
 class ListAggregateDiscoveredResourcesResponseBody(TeaModel):
     def __init__(
         self,
         discovered_resource_profiles: ListAggregateDiscoveredResourcesResponseBodyDiscoveredResourceProfiles = None,
         request_id: str = None,
     ):
-        # The return result of the request.
+        # The ID of the Alibaba Cloud account to which the resource belongs.
         self.discovered_resource_profiles = discovered_resource_profiles
-        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.discovered_resource_profiles:
             self.discovered_resource_profiles.validate()
 
     def to_map(self):
@@ -19581,14 +19568,284 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ListAggregateResourceEvaluationResultsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ListAggregateResourceRelationsRequest(TeaModel):
+    def __init__(
+        self,
+        aggregator_id: str = None,
+        max_results: int = None,
+        next_token: str = None,
+        region: str = None,
+        relation_type: str = None,
+        resource_account_id: int = None,
+        resource_id: str = None,
+        resource_type: str = None,
+        target_resource_id: str = None,
+        target_resource_type: str = None,
+    ):
+        self.aggregator_id = aggregator_id
+        self.max_results = max_results
+        self.next_token = next_token
+        self.region = region
+        self.relation_type = relation_type
+        self.resource_account_id = resource_account_id
+        self.resource_id = resource_id
+        self.resource_type = resource_type
+        self.target_resource_id = target_resource_id
+        self.target_resource_type = target_resource_type
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.aggregator_id is not None:
+            result['AggregatorId'] = self.aggregator_id
+        if self.max_results is not None:
+            result['MaxResults'] = self.max_results
+        if self.next_token is not None:
+            result['NextToken'] = self.next_token
+        if self.region is not None:
+            result['Region'] = self.region
+        if self.relation_type is not None:
+            result['RelationType'] = self.relation_type
+        if self.resource_account_id is not None:
+            result['ResourceAccountId'] = self.resource_account_id
+        if self.resource_id is not None:
+            result['ResourceId'] = self.resource_id
+        if self.resource_type is not None:
+            result['ResourceType'] = self.resource_type
+        if self.target_resource_id is not None:
+            result['TargetResourceId'] = self.target_resource_id
+        if self.target_resource_type is not None:
+            result['TargetResourceType'] = self.target_resource_type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AggregatorId') is not None:
+            self.aggregator_id = m.get('AggregatorId')
+        if m.get('MaxResults') is not None:
+            self.max_results = m.get('MaxResults')
+        if m.get('NextToken') is not None:
+            self.next_token = m.get('NextToken')
+        if m.get('Region') is not None:
+            self.region = m.get('Region')
+        if m.get('RelationType') is not None:
+            self.relation_type = m.get('RelationType')
+        if m.get('ResourceAccountId') is not None:
+            self.resource_account_id = m.get('ResourceAccountId')
+        if m.get('ResourceId') is not None:
+            self.resource_id = m.get('ResourceId')
+        if m.get('ResourceType') is not None:
+            self.resource_type = m.get('ResourceType')
+        if m.get('TargetResourceId') is not None:
+            self.target_resource_id = m.get('TargetResourceId')
+        if m.get('TargetResourceType') is not None:
+            self.target_resource_type = m.get('TargetResourceType')
+        return self
+
+
+class ListAggregateResourceRelationsResponseBodyResourceRelationsResourceRelationList(TeaModel):
+    def __init__(
+        self,
+        account_id: int = None,
+        relation_type: str = None,
+        source_resource_id: str = None,
+        source_resource_region_id: str = None,
+        source_resource_type: str = None,
+        target_resource_id: str = None,
+        target_resource_type: str = None,
+    ):
+        self.account_id = account_id
+        self.relation_type = relation_type
+        self.source_resource_id = source_resource_id
+        self.source_resource_region_id = source_resource_region_id
+        self.source_resource_type = source_resource_type
+        self.target_resource_id = target_resource_id
+        self.target_resource_type = target_resource_type
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.account_id is not None:
+            result['AccountId'] = self.account_id
+        if self.relation_type is not None:
+            result['RelationType'] = self.relation_type
+        if self.source_resource_id is not None:
+            result['SourceResourceId'] = self.source_resource_id
+        if self.source_resource_region_id is not None:
+            result['SourceResourceRegionId'] = self.source_resource_region_id
+        if self.source_resource_type is not None:
+            result['SourceResourceType'] = self.source_resource_type
+        if self.target_resource_id is not None:
+            result['TargetResourceId'] = self.target_resource_id
+        if self.target_resource_type is not None:
+            result['TargetResourceType'] = self.target_resource_type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AccountId') is not None:
+            self.account_id = m.get('AccountId')
+        if m.get('RelationType') is not None:
+            self.relation_type = m.get('RelationType')
+        if m.get('SourceResourceId') is not None:
+            self.source_resource_id = m.get('SourceResourceId')
+        if m.get('SourceResourceRegionId') is not None:
+            self.source_resource_region_id = m.get('SourceResourceRegionId')
+        if m.get('SourceResourceType') is not None:
+            self.source_resource_type = m.get('SourceResourceType')
+        if m.get('TargetResourceId') is not None:
+            self.target_resource_id = m.get('TargetResourceId')
+        if m.get('TargetResourceType') is not None:
+            self.target_resource_type = m.get('TargetResourceType')
+        return self
+
+
+class ListAggregateResourceRelationsResponseBodyResourceRelations(TeaModel):
+    def __init__(
+        self,
+        max_results: int = None,
+        next_token: str = None,
+        resource_relation_list: List[ListAggregateResourceRelationsResponseBodyResourceRelationsResourceRelationList] = None,
+    ):
+        self.max_results = max_results
+        self.next_token = next_token
+        self.resource_relation_list = resource_relation_list
+
+    def validate(self):
+        if self.resource_relation_list:
+            for k in self.resource_relation_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.max_results is not None:
+            result['MaxResults'] = self.max_results
+        if self.next_token is not None:
+            result['NextToken'] = self.next_token
+        result['ResourceRelationList'] = []
+        if self.resource_relation_list is not None:
+            for k in self.resource_relation_list:
+                result['ResourceRelationList'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('MaxResults') is not None:
+            self.max_results = m.get('MaxResults')
+        if m.get('NextToken') is not None:
+            self.next_token = m.get('NextToken')
+        self.resource_relation_list = []
+        if m.get('ResourceRelationList') is not None:
+            for k in m.get('ResourceRelationList'):
+                temp_model = ListAggregateResourceRelationsResponseBodyResourceRelationsResourceRelationList()
+                self.resource_relation_list.append(temp_model.from_map(k))
+        return self
+
+
+class ListAggregateResourceRelationsResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+        resource_relations: ListAggregateResourceRelationsResponseBodyResourceRelations = None,
+    ):
+        self.request_id = request_id
+        self.resource_relations = resource_relations
+
+    def validate(self):
+        if self.resource_relations:
+            self.resource_relations.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.resource_relations is not None:
+            result['ResourceRelations'] = self.resource_relations.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('ResourceRelations') is not None:
+            temp_model = ListAggregateResourceRelationsResponseBodyResourceRelations()
+            self.resource_relations = temp_model.from_map(m['ResourceRelations'])
+        return self
+
+
+class ListAggregateResourceRelationsResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ListAggregateResourceRelationsResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ListAggregateResourceRelationsResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class ListAggregatorsRequest(TeaModel):
     def __init__(
         self,
         max_results: int = None,
         next_token: str = None,
     ):
         # The maximum number of entries to return for a single request. Valid values: 1 to 100.
@@ -22043,34 +22300,40 @@
     def __init__(
         self,
         config_rule_name: str = None,
         description: str = None,
         help_urls: str = None,
         identifier: str = None,
         labels: List[str] = None,
+        remediation_template_identifier: str = None,
+        remediation_template_name: str = None,
         risk_level: int = None,
         scope: ListManagedRulesResponseBodyManagedRulesManagedRuleListScope = None,
+        support_preview_managed_rule: bool = None,
     ):
         # The name of the managed rule.
         self.config_rule_name = config_rule_name
         # The description of the managed rule.
         self.description = description
         # The URL of the topic that describes how the managed rule remediates the incompliant configurations.
         self.help_urls = help_urls
         # The unique identifier of the managed rule.
         self.identifier = identifier
         # The tags of the managed rule.
         self.labels = labels
+        self.remediation_template_identifier = remediation_template_identifier
+        self.remediation_template_name = remediation_template_name
         # The risk level of the resources that do not comply with the managed rule. Valid values:
         # 
         # *   1: high risk level
         # *   2: medium risk level
         # *   3: low risk level
         self.risk_level = risk_level
         self.scope = scope
+        self.support_preview_managed_rule = support_preview_managed_rule
 
     def validate(self):
         if self.scope:
             self.scope.validate()
 
     def to_map(self):
         _map = super().to_map()
@@ -22084,37 +22347,49 @@
             result['Description'] = self.description
         if self.help_urls is not None:
             result['HelpUrls'] = self.help_urls
         if self.identifier is not None:
             result['Identifier'] = self.identifier
         if self.labels is not None:
             result['Labels'] = self.labels
+        if self.remediation_template_identifier is not None:
+            result['RemediationTemplateIdentifier'] = self.remediation_template_identifier
+        if self.remediation_template_name is not None:
+            result['RemediationTemplateName'] = self.remediation_template_name
         if self.risk_level is not None:
             result['RiskLevel'] = self.risk_level
         if self.scope is not None:
             result['Scope'] = self.scope.to_map()
+        if self.support_preview_managed_rule is not None:
+            result['SupportPreviewManagedRule'] = self.support_preview_managed_rule
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('ConfigRuleName') is not None:
             self.config_rule_name = m.get('ConfigRuleName')
         if m.get('Description') is not None:
             self.description = m.get('Description')
         if m.get('HelpUrls') is not None:
             self.help_urls = m.get('HelpUrls')
         if m.get('Identifier') is not None:
             self.identifier = m.get('Identifier')
         if m.get('Labels') is not None:
             self.labels = m.get('Labels')
+        if m.get('RemediationTemplateIdentifier') is not None:
+            self.remediation_template_identifier = m.get('RemediationTemplateIdentifier')
+        if m.get('RemediationTemplateName') is not None:
+            self.remediation_template_name = m.get('RemediationTemplateName')
         if m.get('RiskLevel') is not None:
             self.risk_level = m.get('RiskLevel')
         if m.get('Scope') is not None:
             temp_model = ListManagedRulesResponseBodyManagedRulesManagedRuleListScope()
             self.scope = temp_model.from_map(m['Scope'])
+        if m.get('SupportPreviewManagedRule') is not None:
+            self.support_preview_managed_rule = m.get('SupportPreviewManagedRule')
         return self
 
 
 class ListManagedRulesResponseBodyManagedRules(TeaModel):
     def __init__(
         self,
         managed_rule_list: List[ListManagedRulesResponseBodyManagedRulesManagedRuleList] = None,
@@ -22515,59 +22790,73 @@
         return self
 
 
 class ListRemediationTemplatesRequest(TeaModel):
     def __init__(
         self,
         managed_rule_identifier: str = None,
+        page_number: int = None,
+        page_size: int = None,
         remediation_type: str = None,
     ):
         # The identifier of the managed rule.
         # 
         # You can call the [ListCompliancePackTemplates](~~261176~~) operation to obtain the managed rule identifier.
         self.managed_rule_identifier = managed_rule_identifier
+        self.page_number = page_number
+        self.page_size = page_size
         # The type of the remediation template. Valid value: OOS, which stands for Operation Orchestration Service.
         self.remediation_type = remediation_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.managed_rule_identifier is not None:
             result['ManagedRuleIdentifier'] = self.managed_rule_identifier
+        if self.page_number is not None:
+            result['PageNumber'] = self.page_number
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
         if self.remediation_type is not None:
             result['RemediationType'] = self.remediation_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('ManagedRuleIdentifier') is not None:
             self.managed_rule_identifier = m.get('ManagedRuleIdentifier')
+        if m.get('PageNumber') is not None:
+            self.page_number = m.get('PageNumber')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
         if m.get('RemediationType') is not None:
             self.remediation_type = m.get('RemediationType')
         return self
 
 
 class ListRemediationTemplatesResponseBodyRemediationTemplates(TeaModel):
     def __init__(
         self,
         remediation_type: str = None,
         template_definition: str = None,
+        template_description: str = None,
         template_identifier: str = None,
         template_name: str = None,
     ):
         # The type of the remediation template. Valid value: OOS, which stands for Operation Orchestration Service.
         self.remediation_type = remediation_type
         # The configuration of the remediation template.
         self.template_definition = template_definition
+        self.template_description = template_description
         # The identifier of the remediation template.
         self.template_identifier = template_identifier
         # The name of the remediation template.
         self.template_name = template_name
 
     def validate(self):
         pass
@@ -22578,73 +22867,95 @@
             return _map
 
         result = dict()
         if self.remediation_type is not None:
             result['RemediationType'] = self.remediation_type
         if self.template_definition is not None:
             result['TemplateDefinition'] = self.template_definition
+        if self.template_description is not None:
+            result['TemplateDescription'] = self.template_description
         if self.template_identifier is not None:
             result['TemplateIdentifier'] = self.template_identifier
         if self.template_name is not None:
             result['TemplateName'] = self.template_name
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('RemediationType') is not None:
             self.remediation_type = m.get('RemediationType')
         if m.get('TemplateDefinition') is not None:
             self.template_definition = m.get('TemplateDefinition')
+        if m.get('TemplateDescription') is not None:
+            self.template_description = m.get('TemplateDescription')
         if m.get('TemplateIdentifier') is not None:
             self.template_identifier = m.get('TemplateIdentifier')
         if m.get('TemplateName') is not None:
             self.template_name = m.get('TemplateName')
         return self
 
 
 class ListRemediationTemplatesResponseBody(TeaModel):
     def __init__(
         self,
+        page_number: int = None,
+        page_size: int = None,
         remediation_templates: List[ListRemediationTemplatesResponseBodyRemediationTemplates] = None,
         request_id: str = None,
+        total_count: str = None,
     ):
+        self.page_number = page_number
+        self.page_size = page_size
         # The details of the remediation template.
         self.remediation_templates = remediation_templates
         # The ID of the request.
         self.request_id = request_id
+        self.total_count = total_count
 
     def validate(self):
         if self.remediation_templates:
             for k in self.remediation_templates:
                 if k:
                     k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.page_number is not None:
+            result['PageNumber'] = self.page_number
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
         result['RemediationTemplates'] = []
         if self.remediation_templates is not None:
             for k in self.remediation_templates:
                 result['RemediationTemplates'].append(k.to_map() if k else None)
         if self.request_id is not None:
             result['RequestId'] = self.request_id
+        if self.total_count is not None:
+            result['TotalCount'] = self.total_count
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('PageNumber') is not None:
+            self.page_number = m.get('PageNumber')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
         self.remediation_templates = []
         if m.get('RemediationTemplates') is not None:
             for k in m.get('RemediationTemplates'):
                 temp_model = ListRemediationTemplatesResponseBodyRemediationTemplates()
                 self.remediation_templates.append(temp_model.from_map(k))
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
+        if m.get('TotalCount') is not None:
+            self.total_count = m.get('TotalCount')
         return self
 
 
 class ListRemediationTemplatesResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
@@ -22688,37 +22999,49 @@
         return self
 
 
 class ListRemediationsRequest(TeaModel):
     def __init__(
         self,
         config_rule_ids: str = None,
+        page_number: int = None,
+        page_size: int = None,
     ):
         # The ID of the rule. If you want to specify multiple IDs, separate them with commas (,).
         # 
         # You can call the [ListConfigRules](~~169607~~) operation to obtain the rule ID.
         self.config_rule_ids = config_rule_ids
+        self.page_number = page_number
+        self.page_size = page_size
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.config_rule_ids is not None:
             result['ConfigRuleIds'] = self.config_rule_ids
+        if self.page_number is not None:
+            result['PageNumber'] = self.page_number
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('ConfigRuleIds') is not None:
             self.config_rule_ids = m.get('ConfigRuleIds')
+        if m.get('PageNumber') is not None:
+            self.page_number = m.get('PageNumber')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
         return self
 
 
 class ListRemediationsResponseBodyRemediations(TeaModel):
     def __init__(
         self,
         account_id: int = None,
@@ -22832,51 +23155,69 @@
             self.remediation_type = m.get('RemediationType')
         return self
 
 
 class ListRemediationsResponseBody(TeaModel):
     def __init__(
         self,
+        page_number: int = None,
+        page_size: int = None,
         remediations: List[ListRemediationsResponseBodyRemediations] = None,
         request_id: str = None,
+        total_count: str = None,
     ):
+        self.page_number = page_number
+        self.page_size = page_size
         # The remediation settings returned.
         self.remediations = remediations
         # The ID of the request.
         self.request_id = request_id
+        self.total_count = total_count
 
     def validate(self):
         if self.remediations:
             for k in self.remediations:
                 if k:
                     k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.page_number is not None:
+            result['PageNumber'] = self.page_number
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
         result['Remediations'] = []
         if self.remediations is not None:
             for k in self.remediations:
                 result['Remediations'].append(k.to_map() if k else None)
         if self.request_id is not None:
             result['RequestId'] = self.request_id
+        if self.total_count is not None:
+            result['TotalCount'] = self.total_count
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('PageNumber') is not None:
+            self.page_number = m.get('PageNumber')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
         self.remediations = []
         if m.get('Remediations') is not None:
             for k in m.get('Remediations'):
                 temp_model = ListRemediationsResponseBodyRemediations()
                 self.remediations.append(temp_model.from_map(k))
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
+        if m.get('TotalCount') is not None:
+            self.total_count = m.get('TotalCount')
         return self
 
 
 class ListRemediationsResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
@@ -23339,14 +23680,272 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ListResourceEvaluationResultsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ListResourceRelationsRequest(TeaModel):
+    def __init__(
+        self,
+        max_results: int = None,
+        next_token: str = None,
+        region: str = None,
+        relation_type: str = None,
+        resource_id: str = None,
+        resource_type: str = None,
+        target_resource_id: str = None,
+        target_resource_type: str = None,
+    ):
+        self.max_results = max_results
+        self.next_token = next_token
+        self.region = region
+        self.relation_type = relation_type
+        self.resource_id = resource_id
+        self.resource_type = resource_type
+        self.target_resource_id = target_resource_id
+        self.target_resource_type = target_resource_type
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.max_results is not None:
+            result['MaxResults'] = self.max_results
+        if self.next_token is not None:
+            result['NextToken'] = self.next_token
+        if self.region is not None:
+            result['Region'] = self.region
+        if self.relation_type is not None:
+            result['RelationType'] = self.relation_type
+        if self.resource_id is not None:
+            result['ResourceId'] = self.resource_id
+        if self.resource_type is not None:
+            result['ResourceType'] = self.resource_type
+        if self.target_resource_id is not None:
+            result['TargetResourceId'] = self.target_resource_id
+        if self.target_resource_type is not None:
+            result['TargetResourceType'] = self.target_resource_type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('MaxResults') is not None:
+            self.max_results = m.get('MaxResults')
+        if m.get('NextToken') is not None:
+            self.next_token = m.get('NextToken')
+        if m.get('Region') is not None:
+            self.region = m.get('Region')
+        if m.get('RelationType') is not None:
+            self.relation_type = m.get('RelationType')
+        if m.get('ResourceId') is not None:
+            self.resource_id = m.get('ResourceId')
+        if m.get('ResourceType') is not None:
+            self.resource_type = m.get('ResourceType')
+        if m.get('TargetResourceId') is not None:
+            self.target_resource_id = m.get('TargetResourceId')
+        if m.get('TargetResourceType') is not None:
+            self.target_resource_type = m.get('TargetResourceType')
+        return self
+
+
+class ListResourceRelationsResponseBodyResourceRelationsResourceRelationList(TeaModel):
+    def __init__(
+        self,
+        account_id: int = None,
+        relation_type: str = None,
+        source_resource_id: str = None,
+        source_resource_region_id: str = None,
+        source_resource_type: str = None,
+        target_resource_id: str = None,
+        target_resource_type: str = None,
+    ):
+        self.account_id = account_id
+        self.relation_type = relation_type
+        self.source_resource_id = source_resource_id
+        self.source_resource_region_id = source_resource_region_id
+        self.source_resource_type = source_resource_type
+        self.target_resource_id = target_resource_id
+        self.target_resource_type = target_resource_type
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.account_id is not None:
+            result['AccountId'] = self.account_id
+        if self.relation_type is not None:
+            result['RelationType'] = self.relation_type
+        if self.source_resource_id is not None:
+            result['SourceResourceId'] = self.source_resource_id
+        if self.source_resource_region_id is not None:
+            result['SourceResourceRegionId'] = self.source_resource_region_id
+        if self.source_resource_type is not None:
+            result['SourceResourceType'] = self.source_resource_type
+        if self.target_resource_id is not None:
+            result['TargetResourceId'] = self.target_resource_id
+        if self.target_resource_type is not None:
+            result['TargetResourceType'] = self.target_resource_type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AccountId') is not None:
+            self.account_id = m.get('AccountId')
+        if m.get('RelationType') is not None:
+            self.relation_type = m.get('RelationType')
+        if m.get('SourceResourceId') is not None:
+            self.source_resource_id = m.get('SourceResourceId')
+        if m.get('SourceResourceRegionId') is not None:
+            self.source_resource_region_id = m.get('SourceResourceRegionId')
+        if m.get('SourceResourceType') is not None:
+            self.source_resource_type = m.get('SourceResourceType')
+        if m.get('TargetResourceId') is not None:
+            self.target_resource_id = m.get('TargetResourceId')
+        if m.get('TargetResourceType') is not None:
+            self.target_resource_type = m.get('TargetResourceType')
+        return self
+
+
+class ListResourceRelationsResponseBodyResourceRelations(TeaModel):
+    def __init__(
+        self,
+        max_results: int = None,
+        next_token: str = None,
+        resource_relation_list: List[ListResourceRelationsResponseBodyResourceRelationsResourceRelationList] = None,
+    ):
+        self.max_results = max_results
+        self.next_token = next_token
+        self.resource_relation_list = resource_relation_list
+
+    def validate(self):
+        if self.resource_relation_list:
+            for k in self.resource_relation_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.max_results is not None:
+            result['MaxResults'] = self.max_results
+        if self.next_token is not None:
+            result['NextToken'] = self.next_token
+        result['ResourceRelationList'] = []
+        if self.resource_relation_list is not None:
+            for k in self.resource_relation_list:
+                result['ResourceRelationList'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('MaxResults') is not None:
+            self.max_results = m.get('MaxResults')
+        if m.get('NextToken') is not None:
+            self.next_token = m.get('NextToken')
+        self.resource_relation_list = []
+        if m.get('ResourceRelationList') is not None:
+            for k in m.get('ResourceRelationList'):
+                temp_model = ListResourceRelationsResponseBodyResourceRelationsResourceRelationList()
+                self.resource_relation_list.append(temp_model.from_map(k))
+        return self
+
+
+class ListResourceRelationsResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+        resource_relations: ListResourceRelationsResponseBodyResourceRelations = None,
+    ):
+        self.request_id = request_id
+        self.resource_relations = resource_relations
+
+    def validate(self):
+        if self.resource_relations:
+            self.resource_relations.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.resource_relations is not None:
+            result['ResourceRelations'] = self.resource_relations.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('ResourceRelations') is not None:
+            temp_model = ListResourceRelationsResponseBodyResourceRelations()
+            self.resource_relations = temp_model.from_map(m['ResourceRelations'])
+        return self
+
+
+class ListResourceRelationsResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ListResourceRelationsResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ListResourceRelationsResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class ListTagResourcesRequestTag(TeaModel):
     def __init__(
         self,
         key: str = None,
         value: str = None,
     ):
         # The tag keys of the resource.
@@ -24394,17 +24993,15 @@
 
 
 class StartRemediationRequest(TeaModel):
     def __init__(
         self,
         config_rule_id: str = None,
     ):
-        # The ID of the rule.
-        # 
-        # You can call the [ListConfigRules](~~169607~~) operation to obtain the rule ID.
+        # The ID of the request.
         self.config_rule_id = config_rule_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -24425,20 +25022,19 @@
 
 class StartRemediationResponseBody(TeaModel):
     def __init__(
         self,
         data: bool = None,
         request_id: str = None,
     ):
+        self.data = data
         # Indicates whether the call is successful. Valid values:
         # 
         # *   true: The call is successful.
         # *   false: The call fails.
-        self.data = data
-        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -27624,77 +28220,71 @@
         delivery_channel_name: str = None,
         delivery_channel_target_arn: str = None,
         description: str = None,
         non_compliant_notification: bool = None,
         oversized_data_osstarget_arn: str = None,
         status: int = None,
     ):
-        # The client token that you want to use to ensure the idempotency of the request. You can use the client to generate the value, but you must make sure that the value is unique among different requests.
-        # 
-        # The `ClientToken` value can contain only ASCII characters and cannot exceed 64 characters in length. For more information, see [Ensure idempotence](~~25693~~).
-        self.client_token = client_token
         # Specifies whether to deliver resource change logs to the specified destination. If you set this parameter to true, Cloud Config delivers resource change logs to OSS, Log Service, or MNS when the configurations of the resources change. Valid values:
         # 
         # *   true
         # *   false. This is the default value.
         # 
         # >  This parameter is applicable to delivery channels of the OSS, SLS, or MNS type.
+        self.client_token = client_token
+        # The ARN of the OSS bucket to which you want to transfer the delivery data when the size of the data exceeds the specified upper limit of the delivery channel. Format: `acs:oss:{RegionId}:{accountId}:{bucketName}`.
+        # 
+        # If you do not configure this parameter, Cloud Config delivers only summary data.
+        # 
+        # >  This parameter is available only for delivery channels of the SLS type or MNS type. The upper limit on the storage size of delivery channels of the SLS type is 1 MB, and the upper limit on the storage size of delivery channels of the MNS type is 64 KB.
         self.configuration_item_change_notification = configuration_item_change_notification
-        # Specifies whether to deliver scheduled resource snapshots to the OSS bucket. If the value of this parameter is true, the scheduled resource snapshots are delivered to the specified OSS bucket at 00:00:00 and 12:00:00 on a daily basis. Valid values:
+        # Specifies whether to deliver resource non-compliance events to the specified destination. If you set this parameter to true, Cloud Config delivers resource non-compliance events to Log Service or MNS when resources are considered incompliant. Valid values:
         # 
         # *   true
         # *   false. This is the default value.
         # 
-        # >  This parameter is applicable only to delivery channels of the OSS type.
+        # >  This parameter is applicable only to delivery channels of the SLS or MNS type.
         self.configuration_snapshot = configuration_snapshot
-        # The ARN of the role that you want to assign to the delivery channel. Specify the ARN in the following format: `acs:ram::{accountId}:role/aliyunserviceroleforconfig`.
+        # The description of the delivery channel.
         self.delivery_channel_assume_role_arn = delivery_channel_assume_role_arn
+        # The client token that you want to use to ensure the idempotency of the request. You can use the client to generate the value, but you must make sure that the value is unique among different requests.
+        # 
+        # The `ClientToken` value can contain only ASCII characters and cannot exceed 64 characters in length. For more information, see [Ensure idempotence](~~25693~~).
+        self.delivery_channel_condition = delivery_channel_condition
+        # The ID of the request.
+        self.delivery_channel_id = delivery_channel_id
+        # The ARN of the role that you want to assign to the delivery channel. Specify the ARN in the following format: `acs:ram::{accountId}:role/aliyunserviceroleforconfig`.
+        self.delivery_channel_name = delivery_channel_name
         # The rule that you want to attach to the delivery channel. This parameter is available only for delivery channels of the MNS type.
         # 
         # This parameter specifies the lowest risk level and the resource types for the events to which you want to subscribe.
         # 
         # *   The setting of the lowest risk level for the events to which you want to subscribe is in the following format: `{"filterType":"RuleRiskLevel","value":"1","multiple":false}`. The `value` field specifies the lowest risk level for the events to which you want to subscribe. Valid values: 1, 2, and 3, where 1 indicates the high risk level, 2 indicates the medium risk level, and 3 indicates the low risk level.
         # 
         # *   The setting of the resource types for the events to which you want to subscribe is in the following format: `{"filterType":"ResourceType","values":["ACS::ACK::Cluster","ACS::ActionTrail::Trail","ACS::CBWP::CommonBandwidthPackage"],"multiple":true}`. The `values` field specifies the resource types for which you want to subscribe to events. The value of the field is a JSON array.
         # 
         #     Example: `[{"filterType":"ResourceType","values":["ACS::ActionTrail::Trail","ACS::CBWP::CommonBandwidthPackage","ACS::CDN::Domain","ACS::CEN::CenBandwidthPackage","ACS::CEN::CenInstance","ACS::CEN::Flowlog","ACS::DdosCoo::Instance"],"multiple":true}]`
-        self.delivery_channel_condition = delivery_channel_condition
-        # The ID of the delivery channel.
-        # 
-        # For more information about how to obtain the ID of the delivery channel, see [DescribeDeliveryChannels](~~174466~~).
-        self.delivery_channel_id = delivery_channel_id
-        # The name of the delivery channel.
-        # 
-        # >  If you do not configure this parameter, this parameter is left empty.
-        self.delivery_channel_name = delivery_channel_name
-        # The ARN of the delivery destination. Valid values:
-        # 
-        # *   `acs:oss:{RegionId}:{accountId}:{bucketName}` if your delivery destination is an OSS bucket. Example: `acs:oss:cn-shanghai:100931896542****:new-bucket`.
-        # *   `acs:mns:{RegionId}:{accountId}:/topics/{topicName}` if your delivery destination is an MNS topic. Example: `acs:mns:cn-shanghai:100931896542****:/topics/topic1`.
-        # *   `acs:log:{RegionId}:{accountId}:project/{projectName}/logstore/{logstoreName}` if your delivery destination is a Log Service Logstore. Example: `acs:log:cn-shanghai:100931896542****:project/project1/logstore/logstore1`.
         self.delivery_channel_target_arn = delivery_channel_target_arn
-        # The description of the delivery channel.
-        self.description = description
-        # Specifies whether to deliver resource non-compliance events to the specified destination. If you set this parameter to true, Cloud Config delivers resource non-compliance events to Log Service or MNS when resources are considered incompliant. Valid values:
+        # Specifies whether to deliver scheduled resource snapshots to the OSS bucket. If the value of this parameter is true, the scheduled resource snapshots are delivered to the specified OSS bucket at 00:00:00 and 12:00:00 on a daily basis. Valid values:
         # 
         # *   true
         # *   false. This is the default value.
         # 
-        # >  This parameter is applicable only to delivery channels of the SLS or MNS type.
-        self.non_compliant_notification = non_compliant_notification
-        # The ARN of the OSS bucket to which you want to transfer the delivery data when the size of the data exceeds the specified upper limit of the delivery channel. Format: `acs:oss:{RegionId}:{accountId}:{bucketName}`.
-        # 
-        # If you do not configure this parameter, Cloud Config delivers only summary data.
+        # >  This parameter is applicable only to delivery channels of the OSS type.
+        self.description = description
+        # The ID of the delivery channel.
         # 
-        # >  This parameter is available only for delivery channels of the SLS type or MNS type. The upper limit on the storage size of delivery channels of the SLS type is 1 MB, and the upper limit on the storage size of delivery channels of the MNS type is 64 KB.
-        self.oversized_data_osstarget_arn = oversized_data_osstarget_arn
+        # For more information about how to obtain the ID of the delivery channel, see [DescribeDeliveryChannels](~~174466~~).
+        self.non_compliant_notification = non_compliant_notification
         # Specifies whether to disable the delivery channel. Valid values:
         # 
         # *   0: Cloud Config disables the delivery channel. Cloud Config retains the most recent delivery configuration and stops resource data delivery.
         # *   1: Cloud Config enables the delivery channel. This is the default value.
+        self.oversized_data_osstarget_arn = oversized_data_osstarget_arn
+        # The ID of the delivery channel.
         self.status = status
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -27759,17 +28349,15 @@
 
 class UpdateDeliveryChannelResponseBody(TeaModel):
     def __init__(
         self,
         delivery_channel_id: str = None,
         request_id: str = None,
     ):
-        # The ID of the delivery channel.
         self.delivery_channel_id = delivery_channel_id
-        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
```

### Comparing `alibabacloud_config20200907-2.2.7/alibabacloud_config20200907.egg-info/PKG-INFO` & `alibabacloud_config20200907-2.2.8/alibabacloud_config20200907.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-config20200907
-Version: 2.2.7
+Version: 2.2.8
 Summary: Alibaba Cloud CloudConfig (20200907) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_config20200907-2.2.7/setup.py` & `alibabacloud_config20200907-2.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_config20200907.
 
-Created on 12/04/2023
+Created on 26/04/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_config20200907"
 NAME = "alibabacloud_config20200907" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud CloudConfig (20200907) SDK Library for Python"
```

