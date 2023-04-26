# Comparing `tmp/ros-cdk-lindorm-1.0.12.tar.gz` & `tmp/ros-cdk-lindorm-1.0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-lindorm-1.0.12.tar", last modified: Tue Feb 14 09:53:05 2023, max compression
+gzip compressed data, was "dist/ros-cdk-lindorm-1.0.13.tar", last modified: Wed Apr 26 07:38:26 2023, max compression
```

## Comparing `ros-cdk-lindorm-1.0.12.tar` & `ros-cdk-lindorm-1.0.13.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-14 09:53:05.000000 ros-cdk-lindorm-1.0.12/
--rw-r--r--   0 root         (0) root         (0)    10279 2023-02-14 09:53:04.000000 ros-cdk-lindorm-1.0.12/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2023-02-14 09:53:04.000000 ros-cdk-lindorm-1.0.12/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2023-02-14 09:53:04.000000 ros-cdk-lindorm-1.0.12/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1257 2023-02-14 09:53:05.000000 ros-cdk-lindorm-1.0.12/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      191 2023-02-14 09:53:04.000000 ros-cdk-lindorm-1.0.12/README.md
--rw-r--r--   0 root         (0) root         (0)      236 2023-02-14 09:53:04.000000 ros-cdk-lindorm-1.0.12/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-14 09:53:05.000000 ros-cdk-lindorm-1.0.12/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1849 2023-02-14 09:53:04.000000 ros-cdk-lindorm-1.0.12/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-14 09:53:05.000000 ros-cdk-lindorm-1.0.12/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-14 09:53:05.000000 ros-cdk-lindorm-1.0.12/src/ros_cdk_lindorm/
--rw-r--r--   0 root         (0) root         (0)   225484 2023-02-14 09:53:04.000000 ros-cdk-lindorm-1.0.12/src/ros_cdk_lindorm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-14 09:53:05.000000 ros-cdk-lindorm-1.0.12/src/ros_cdk_lindorm/_jsii/
--rw-r--r--   0 root         (0) root         (0)      427 2023-02-14 09:53:04.000000 ros-cdk-lindorm-1.0.12/src/ros_cdk_lindorm/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    63665 2023-02-14 09:53:04.000000 ros-cdk-lindorm-1.0.12/src/ros_cdk_lindorm/_jsii/ros-cdk-lindorm@1.0.12.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-14 09:53:04.000000 ros-cdk-lindorm-1.0.12/src/ros_cdk_lindorm/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-14 09:53:05.000000 ros-cdk-lindorm-1.0.12/src/ros_cdk_lindorm.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1257 2023-02-14 09:53:05.000000 ros-cdk-lindorm-1.0.12/src/ros_cdk_lindorm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      441 2023-02-14 09:53:05.000000 ros-cdk-lindorm-1.0.12/src/ros_cdk_lindorm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-14 09:53:05.000000 ros-cdk-lindorm-1.0.12/src/ros_cdk_lindorm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      109 2023-02-14 09:53:05.000000 ros-cdk-lindorm-1.0.12/src/ros_cdk_lindorm.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-02-14 09:53:05.000000 ros-cdk-lindorm-1.0.12/src/ros_cdk_lindorm.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:38:26.000000 ros-cdk-lindorm-1.0.13/
+-rw-r--r--   0 root         (0) root         (0)    10279 2023-04-26 07:38:25.000000 ros-cdk-lindorm-1.0.13/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2023-04-26 07:38:25.000000 ros-cdk-lindorm-1.0.13/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2023-04-26 07:38:25.000000 ros-cdk-lindorm-1.0.13/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1308 2023-04-26 07:38:26.000000 ros-cdk-lindorm-1.0.13/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      191 2023-04-26 07:38:25.000000 ros-cdk-lindorm-1.0.13/README.md
+-rw-r--r--   0 root         (0) root         (0)      234 2023-04-26 07:38:25.000000 ros-cdk-lindorm-1.0.13/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-26 07:38:26.000000 ros-cdk-lindorm-1.0.13/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1899 2023-04-26 07:38:25.000000 ros-cdk-lindorm-1.0.13/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:38:26.000000 ros-cdk-lindorm-1.0.13/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:38:26.000000 ros-cdk-lindorm-1.0.13/src/ros_cdk_lindorm/
+-rw-r--r--   0 root         (0) root         (0)   243836 2023-04-26 07:38:25.000000 ros-cdk-lindorm-1.0.13/src/ros_cdk_lindorm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:38:26.000000 ros-cdk-lindorm-1.0.13/src/ros_cdk_lindorm/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      427 2023-04-26 07:38:25.000000 ros-cdk-lindorm-1.0.13/src/ros_cdk_lindorm/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    66639 2023-04-26 07:38:25.000000 ros-cdk-lindorm-1.0.13/src/ros_cdk_lindorm/_jsii/ros-cdk-lindorm@1.0.13.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 07:38:25.000000 ros-cdk-lindorm-1.0.13/src/ros_cdk_lindorm/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:38:26.000000 ros-cdk-lindorm-1.0.13/src/ros_cdk_lindorm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1308 2023-04-26 07:38:25.000000 ros-cdk-lindorm-1.0.13/src/ros_cdk_lindorm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      441 2023-04-26 07:38:25.000000 ros-cdk-lindorm-1.0.13/src/ros_cdk_lindorm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 07:38:25.000000 ros-cdk-lindorm-1.0.13/src/ros_cdk_lindorm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2023-04-26 07:38:25.000000 ros-cdk-lindorm-1.0.13/src/ros_cdk_lindorm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-04-26 07:38:25.000000 ros-cdk-lindorm-1.0.13/src/ros_cdk_lindorm.egg-info/top_level.txt
```

### Comparing `ros-cdk-lindorm-1.0.12/LICENSE` & `ros-cdk-lindorm-1.0.13/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-lindorm-1.0.12/PKG-INFO` & `ros-cdk-lindorm-1.0.13/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-lindorm
-Version: 1.0.12
+Version: 1.0.13
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS LINDORM Construct Library
         
@@ -19,12 +19,13 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
```

### Comparing `ros-cdk-lindorm-1.0.12/setup.py` & `ros-cdk-lindorm-1.0.13/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-lindorm",
-    "version": "1.0.12",
+    "version": "1.0.13",
     "description": "Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com",
     "license": "Apache-2.0",
     "url": "https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git",
     "long_description_content_type": "text/markdown",
     "author": "ROS Development Team",
     "bdist_wheel": {
         "universal": true
@@ -22,37 +22,38 @@
     },
     "packages": [
         "ros_cdk_lindorm",
         "ros_cdk_lindorm._jsii"
     ],
     "package_data": {
         "ros_cdk_lindorm._jsii": [
-            "ros-cdk-lindorm@1.0.12.jsii.tgz"
+            "ros-cdk-lindorm@1.0.13.jsii.tgz"
         ],
         "ros_cdk_lindorm": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "constructs>=3.0.4, <4.0.0",
-        "jsii>=1.74.0, <2.0.0",
+        "jsii>=1.80.0, <2.0.0",
         "publication>=0.0.3",
         "ros-cdk-core>=1.0.6, <2.0.0",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Typing :: Typed",
         "License :: OSI Approved",
         "Programming Language :: Python :: 3"
     ],
     "scripts": []
 }
 """
```

### Comparing `ros-cdk-lindorm-1.0.12/src/ros_cdk_lindorm/__init__.py` & `ros-cdk-lindorm-1.0.13/src/ros_cdk_lindorm/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -87,14 +87,16 @@
         "lindorm_spec": "lindormSpec",
         "period": "period",
         "period_unit": "periodUnit",
         "resource_group_id": "resourceGroupId",
         "security_ip_list": "securityIpList",
         "solr_num": "solrNum",
         "solr_spec": "solrSpec",
+        "stream_num": "streamNum",
+        "stream_spec": "streamSpec",
         "tsdb_num": "tsdbNum",
         "tsdb_spec": "tsdbSpec",
         "v_switch_id": "vSwitchId",
         "zone_id": "zoneId",
     },
 )
 class InstanceProps:
@@ -114,14 +116,16 @@
         lindorm_spec: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
         period: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
         period_unit: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
         resource_group_id: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
         security_ip_list: typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Sequence[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]]] = None,
         solr_num: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
         solr_spec: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+        stream_num: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+        stream_spec: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
         tsdb_num: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
         tsdb_spec: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
         v_switch_id: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
         zone_id: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::Lindorm::Instance``.
 
@@ -138,14 +142,16 @@
         :param lindorm_spec: Property lindormSpec: The specification of LindormTable nodes in the instance. Valid values: lindorm.g.xlarge: Each node has 4 dedicated CPU cores and 16 GB of dedicated memory. lindorm.g.2xlarge: Each node has 8 dedicated CPU cores and 32 GB of dedicated memory. lindorm.g.4xlarge: Each node has 16 dedicated CPU cores and 64 GB of dedicated memory. lindorm.g.8xlarge: Each node has 32 dedicated CPU cores and 128 GB of dedicated memory. lindorm.c.xlarge: Each node has 4 dedicated CPU cores and 8 GB of dedicated memory. lindorm.c.2xlarge: Each node has 8 dedicated CPU cores and 16 GB of dedicated memory. lindorm.c.4xlarge: Each node has 16 dedicated CPU cores and 32 GB of dedicated memory. lindorm.c.8xlarge: Each node has 32 dedicated CPU cores and 64 GB of dedicated memory.
         :param period: Property period: The subscription period of the instance. The valid values of this parameter depend on the value of the PeriodUnit parameter. If PeriodUnit is set to Month, Valid values are 1,2,3,4,5,6,7,8,9,12,24,36. If PeriodUnit is set to Year, set this parameter to an integer that ranges from 1 to 3. NoteThis parameter is available and required when the PayType parameter is set to PREPAY.
         :param period_unit: Property periodUnit: The period based on which you are charged for the instance. Valid values: Month: You are charged for the instance on a monthly basis. Year: You are charged for the instance on a yearly basis. NoteThis parameter is available and required when the PayType parameter is set to PREPAY.
         :param resource_group_id: Property resourceGroupId: The ID of the resource group to which the Lindorm instance belongs.
         :param security_ip_list: Property securityIpList: The ip white list of instance.
         :param solr_num: Property solrNum: The number of LindormSearch nodes in the instance. Valid values: integers from 0 to 60.
         :param solr_spec: Property solrSpec: The specification of the LindormSearch nodes in the instance. Valid values: lindorm.g.xlarge: Each node has 4 dedicated CPU cores and 16 GB of dedicated memory. lindorm.g.2xlarge: Each node has 8 dedicated CPU cores and 32 GB of dedicated memory. lindorm.g.4xlarge: Each node has 16 dedicated CPU cores and 64 GB of dedicated memory. lindorm.g.8xlarge: Each node has 32 dedicated CPU cores and 128 GB of dedicated memory.
+        :param stream_num: Property streamNum: The number of LindormStream nodes in the instance. Valid values: integers from 0 to 90.
+        :param stream_spec: Property streamSpec: The specification of LindormStream nodes in the instance. Valid values: lindorm.g.xlarge: Each node has 4 dedicated CPU cores and 16 GB of dedicated memory. lindorm.g.2xlarge: Each node has 8 dedicated CPU cores and 32 GB of dedicated memory. lindorm.g.4xlarge: Each node has 16 dedicated CPU cores and 64 GB of dedicated memory. lindorm.g.8xlarge: Each node has 32 dedicated CPU cores and 128 GB of dedicated memory. lindorm.c.xlarge: Each node has 4 dedicated CPU cores and 8 GB of dedicated memory. lindorm.c.2xlarge: Each node has 8 dedicated CPU cores and 16 GB of dedicated memory. lindorm.c.4xlarge: Each node has 16 dedicated CPU cores and 32 GB of dedicated memory. lindorm.c.8xlarge: Each node has 32 dedicated CPU cores and 64 GB of dedicated memory.
         :param tsdb_num: Property tsdbNum: The number of the LindormTSDB nodes in the instance. The valid values of this parameter depend on the value of the PayType parameter. If the PayType parameter is set to PREPAY, set this parameter to an integer that ranges from 0 to 24. If the PayType parameter is set to POSTPAY, set this parameter to an integer that ranges from 0 to 32.
         :param tsdb_spec: Property tsdbSpec: The specification of the LindormTSDB nodes in the instance. Valid values: lindorm.g.xlarge: Each node has 4 dedicated CPU cores and 16 GB of dedicated memory. lindorm.g.2xlarge: Each node has 8 dedicated CPU cores and 32 GB of dedicated memory. lindorm.g.4xlarge: Each node has 16 dedicated CPU cores and 64 GB of dedicated memory. lindorm.g.8xlarge: Each node has 32 dedicated CPU cores and 128 GB of dedicated memory.
         :param v_switch_id: Property vSwitchId: The ID of the vSwitch to which you want the instance to connect.
         :param zone_id: Property zoneId: The ID of the zone in which you want to create the instance.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__ccd9c78cafd91c7c644f059a6f3ca0d97ce09800ea122f0813f8135e0c40680c)
@@ -162,14 +168,16 @@
             check_type(argname="argument lindorm_spec", value=lindorm_spec, expected_type=type_hints["lindorm_spec"])
             check_type(argname="argument period", value=period, expected_type=type_hints["period"])
             check_type(argname="argument period_unit", value=period_unit, expected_type=type_hints["period_unit"])
             check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
             check_type(argname="argument security_ip_list", value=security_ip_list, expected_type=type_hints["security_ip_list"])
             check_type(argname="argument solr_num", value=solr_num, expected_type=type_hints["solr_num"])
             check_type(argname="argument solr_spec", value=solr_spec, expected_type=type_hints["solr_spec"])
+            check_type(argname="argument stream_num", value=stream_num, expected_type=type_hints["stream_num"])
+            check_type(argname="argument stream_spec", value=stream_spec, expected_type=type_hints["stream_spec"])
             check_type(argname="argument tsdb_num", value=tsdb_num, expected_type=type_hints["tsdb_num"])
             check_type(argname="argument tsdb_spec", value=tsdb_spec, expected_type=type_hints["tsdb_spec"])
             check_type(argname="argument v_switch_id", value=v_switch_id, expected_type=type_hints["v_switch_id"])
             check_type(argname="argument zone_id", value=zone_id, expected_type=type_hints["zone_id"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "disk_category": disk_category,
             "instance_name": instance_name,
@@ -199,14 +207,18 @@
             self._values["resource_group_id"] = resource_group_id
         if security_ip_list is not None:
             self._values["security_ip_list"] = security_ip_list
         if solr_num is not None:
             self._values["solr_num"] = solr_num
         if solr_spec is not None:
             self._values["solr_spec"] = solr_spec
+        if stream_num is not None:
+            self._values["stream_num"] = stream_num
+        if stream_spec is not None:
+            self._values["stream_spec"] = stream_spec
         if tsdb_num is not None:
             self._values["tsdb_num"] = tsdb_num
         if tsdb_spec is not None:
             self._values["tsdb_spec"] = tsdb_spec
         if v_switch_id is not None:
             self._values["v_switch_id"] = v_switch_id
         if zone_id is not None:
@@ -424,14 +436,44 @@
         lindorm.g.4xlarge: Each node has 16 dedicated CPU cores and 64 GB of dedicated memory.
         lindorm.g.8xlarge: Each node has 32 dedicated CPU cores and 128 GB of dedicated memory.
         '''
         result = self._values.get("solr_spec")
         return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], result)
 
     @builtins.property
+    def stream_num(
+        self,
+    ) -> typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]]:
+        '''Property streamNum: The number of LindormStream nodes in the instance.
+
+        Valid values: integers from 0 to 90.
+        '''
+        result = self._values.get("stream_num")
+        return typing.cast(typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]], result)
+
+    @builtins.property
+    def stream_spec(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+        '''Property streamSpec: The specification of LindormStream nodes in the instance.
+
+        Valid values:
+        lindorm.g.xlarge: Each node has 4 dedicated CPU cores and 16 GB of dedicated memory.
+        lindorm.g.2xlarge: Each node has 8 dedicated CPU cores and 32 GB of dedicated memory.
+        lindorm.g.4xlarge: Each node has 16 dedicated CPU cores and 64 GB of dedicated memory.
+        lindorm.g.8xlarge: Each node has 32 dedicated CPU cores and 128 GB of dedicated memory.
+        lindorm.c.xlarge: Each node has 4 dedicated CPU cores and 8 GB of dedicated memory.
+        lindorm.c.2xlarge: Each node has 8 dedicated CPU cores and 16 GB of dedicated memory.
+        lindorm.c.4xlarge: Each node has 16 dedicated CPU cores and 32 GB of dedicated memory.
+        lindorm.c.8xlarge: Each node has 32 dedicated CPU cores and 64 GB of dedicated memory.
+        '''
+        result = self._values.get("stream_spec")
+        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], result)
+
+    @builtins.property
     def tsdb_num(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]]:
         '''Property tsdbNum: The number of the LindormTSDB nodes in the instance.
 
         The valid values of this parameter depend on the value of the PayType parameter.
         If the PayType parameter is set to PREPAY, set this parameter to an integer that ranges from 0 to 24.
@@ -557,14 +599,16 @@
         "primary_zone_id": "primaryZoneId",
         "resource_group_id": "resourceGroupId",
         "security_ip_list": "securityIpList",
         "solr_num": "solrNum",
         "solr_spec": "solrSpec",
         "standby_v_switch_id": "standbyVSwitchId",
         "standby_zone_id": "standbyZoneId",
+        "stream_num": "streamNum",
+        "stream_spec": "streamSpec",
         "tsdb_num": "tsdbNum",
         "tsdb_spec": "tsdbSpec",
     },
 )
 class MultiZoneInstanceProps:
     def __init__(
         self,
@@ -593,14 +637,16 @@
         primary_zone_id: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
         resource_group_id: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
         security_ip_list: typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Sequence[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]]] = None,
         solr_num: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
         solr_spec: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
         standby_v_switch_id: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
         standby_zone_id: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+        stream_num: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+        stream_spec: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
         tsdb_num: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
         tsdb_spec: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::Lindorm::MultiZoneInstance``.
 
         :param disk_category: Property diskCategory: The storage type of the instance. Valid values: cloud_efficiency: This instance uses the Standard type of storage. cloud_ssd: This instance uses the Performance type of storage. capacity_cloud_storage: This instance uses the Capacity type of storage. local_ssd_pro: This instance uses local SSDs. local_hdd_pro: This instance uses local HDDs.
         :param instance_name: Property instanceName: The name of the instance that you want to create.
@@ -626,14 +672,16 @@
         :param primary_zone_id: Property primaryZoneId: For many available zone instances, the available area ID of the main available area.If you need to create a multi -available area example, this parameter must be filled.
         :param resource_group_id: Property resourceGroupId: The ID of the resource group to which the Lindorm instance belongs.
         :param security_ip_list: Property securityIpList: The ip white list of instance.
         :param solr_num: Property solrNum: The number of LindormSearch nodes in the instance. Valid values: integers from 0 to 60.
         :param solr_spec: Property solrSpec: The specification of the LindormSearch nodes in the instance. Valid values: lindorm.g.xlarge: Each node has 4 dedicated CPU cores and 16 GB of dedicated memory. lindorm.g.2xlarge: Each node has 8 dedicated CPU cores and 32 GB of dedicated memory. lindorm.g.4xlarge: Each node has 16 dedicated CPU cores and 64 GB of dedicated memory. lindorm.g.8xlarge: Each node has 32 dedicated CPU cores and 128 GB of dedicated memory.
         :param standby_v_switch_id: Property standbyVSwitchId: The ID of the vSwitch that is specified for the secondary zone of the instance. The vSwitch must be deployed in the zone specified by the StandbyZoneId parameter. **This parameter is required if you want to create a multi-zone instance.
         :param standby_zone_id: Property standbyZoneId: The ID of the secondary zone of the instance. **This parameter is required if you want to create a multi-zone instance.
+        :param stream_num: Property streamNum: The number of LindormStream nodes in the instance. Valid values: integers from 0 to 90.
+        :param stream_spec: Property streamSpec: The specification of LindormStream nodes in the instance. Valid values: lindorm.g.xlarge: Each node has 4 dedicated CPU cores and 16 GB of dedicated memory. lindorm.g.2xlarge: Each node has 8 dedicated CPU cores and 32 GB of dedicated memory. lindorm.g.4xlarge: Each node has 16 dedicated CPU cores and 64 GB of dedicated memory. lindorm.g.8xlarge: Each node has 32 dedicated CPU cores and 128 GB of dedicated memory. lindorm.c.xlarge: Each node has 4 dedicated CPU cores and 8 GB of dedicated memory. lindorm.c.2xlarge: Each node has 8 dedicated CPU cores and 16 GB of dedicated memory. lindorm.c.4xlarge: Each node has 16 dedicated CPU cores and 32 GB of dedicated memory. lindorm.c.8xlarge: Each node has 32 dedicated CPU cores and 64 GB of dedicated memory.
         :param tsdb_num: Property tsdbNum: The number of the LindormTSDB nodes in the instance. The valid values of this parameter depend on the value of the PayType parameter. If the PayType parameter is set to PREPAY, set this parameter to an integer that ranges from 0 to 24. If the PayType parameter is set to POSTPAY, set this parameter to an integer that ranges from 0 to 32.
         :param tsdb_spec: Property tsdbSpec: The specification of the LindormTSDB nodes in the instance. Valid values: lindorm.g.xlarge: Each node has 4 dedicated CPU cores and 16 GB of dedicated memory. lindorm.g.2xlarge: Each node has 8 dedicated CPU cores and 32 GB of dedicated memory. lindorm.g.4xlarge: Each node has 16 dedicated CPU cores and 64 GB of dedicated memory. lindorm.g.8xlarge: Each node has 32 dedicated CPU cores and 128 GB of dedicated memory.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__26dc8ab7d23f58bb8f757e018142fdce047c83bfa1362bce523a9f6fcfdecf44)
             check_type(argname="argument disk_category", value=disk_category, expected_type=type_hints["disk_category"])
             check_type(argname="argument instance_name", value=instance_name, expected_type=type_hints["instance_name"])
@@ -659,14 +707,16 @@
             check_type(argname="argument primary_zone_id", value=primary_zone_id, expected_type=type_hints["primary_zone_id"])
             check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
             check_type(argname="argument security_ip_list", value=security_ip_list, expected_type=type_hints["security_ip_list"])
             check_type(argname="argument solr_num", value=solr_num, expected_type=type_hints["solr_num"])
             check_type(argname="argument solr_spec", value=solr_spec, expected_type=type_hints["solr_spec"])
             check_type(argname="argument standby_v_switch_id", value=standby_v_switch_id, expected_type=type_hints["standby_v_switch_id"])
             check_type(argname="argument standby_zone_id", value=standby_zone_id, expected_type=type_hints["standby_zone_id"])
+            check_type(argname="argument stream_num", value=stream_num, expected_type=type_hints["stream_num"])
+            check_type(argname="argument stream_spec", value=stream_spec, expected_type=type_hints["stream_spec"])
             check_type(argname="argument tsdb_num", value=tsdb_num, expected_type=type_hints["tsdb_num"])
             check_type(argname="argument tsdb_spec", value=tsdb_spec, expected_type=type_hints["tsdb_spec"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "disk_category": disk_category,
             "instance_name": instance_name,
             "vpc_id": vpc_id,
         }
@@ -716,14 +766,18 @@
             self._values["solr_num"] = solr_num
         if solr_spec is not None:
             self._values["solr_spec"] = solr_spec
         if standby_v_switch_id is not None:
             self._values["standby_v_switch_id"] = standby_v_switch_id
         if standby_zone_id is not None:
             self._values["standby_zone_id"] = standby_zone_id
+        if stream_num is not None:
+            self._values["stream_num"] = stream_num
+        if stream_spec is not None:
+            self._values["stream_spec"] = stream_spec
         if tsdb_num is not None:
             self._values["tsdb_num"] = tsdb_num
         if tsdb_spec is not None:
             self._values["tsdb_spec"] = tsdb_spec
 
     @builtins.property
     def disk_category(
@@ -1069,14 +1123,44 @@
 
         **This parameter is required if you want to create a multi-zone instance.
         '''
         result = self._values.get("standby_zone_id")
         return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], result)
 
     @builtins.property
+    def stream_num(
+        self,
+    ) -> typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]]:
+        '''Property streamNum: The number of LindormStream nodes in the instance.
+
+        Valid values: integers from 0 to 90.
+        '''
+        result = self._values.get("stream_num")
+        return typing.cast(typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]], result)
+
+    @builtins.property
+    def stream_spec(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+        '''Property streamSpec: The specification of LindormStream nodes in the instance.
+
+        Valid values:
+        lindorm.g.xlarge: Each node has 4 dedicated CPU cores and 16 GB of dedicated memory.
+        lindorm.g.2xlarge: Each node has 8 dedicated CPU cores and 32 GB of dedicated memory.
+        lindorm.g.4xlarge: Each node has 16 dedicated CPU cores and 64 GB of dedicated memory.
+        lindorm.g.8xlarge: Each node has 32 dedicated CPU cores and 128 GB of dedicated memory.
+        lindorm.c.xlarge: Each node has 4 dedicated CPU cores and 8 GB of dedicated memory.
+        lindorm.c.2xlarge: Each node has 8 dedicated CPU cores and 16 GB of dedicated memory.
+        lindorm.c.4xlarge: Each node has 16 dedicated CPU cores and 32 GB of dedicated memory.
+        lindorm.c.8xlarge: Each node has 32 dedicated CPU cores and 64 GB of dedicated memory.
+        '''
+        result = self._values.get("stream_spec")
+        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], result)
+
+    @builtins.property
     def tsdb_num(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]]:
         '''Property tsdbNum: The number of the LindormTSDB nodes in the instance.
 
         The valid values of this parameter depend on the value of the PayType parameter.
         If the PayType parameter is set to PREPAY, set this parameter to an integer that ranges from 0 to 24.
@@ -1586,14 +1670,64 @@
     ) -> None:
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__7050bded188f218006bc64f861a891922641755eec0f856c8a74884c27b636bc)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "solrSpec", value)
 
     @builtins.property
+    @jsii.member(jsii_name="streamNum")
+    def stream_num(
+        self,
+    ) -> typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]]:
+        '''
+        :Property: streamNum: The number of LindormStream nodes in the instance. Valid values: integers from 0 to 90.
+        '''
+        return typing.cast(typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]], jsii.get(self, "streamNum"))
+
+    @stream_num.setter
+    def stream_num(
+        self,
+        value: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__cff9beb1b952eadb780012da5a270ba24852867d1480e869e736ed63a533f6d8)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "streamNum", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="streamSpec")
+    def stream_spec(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+        '''
+        :Property:
+
+        streamSpec: The specification of LindormStream nodes in the instance. Valid values:
+        lindorm.g.xlarge: Each node has 4 dedicated CPU cores and 16 GB of dedicated memory.
+        lindorm.g.2xlarge: Each node has 8 dedicated CPU cores and 32 GB of dedicated memory.
+        lindorm.g.4xlarge: Each node has 16 dedicated CPU cores and 64 GB of dedicated memory.
+        lindorm.g.8xlarge: Each node has 32 dedicated CPU cores and 128 GB of dedicated memory.
+        lindorm.c.xlarge: Each node has 4 dedicated CPU cores and 8 GB of dedicated memory.
+        lindorm.c.2xlarge: Each node has 8 dedicated CPU cores and 16 GB of dedicated memory.
+        lindorm.c.4xlarge: Each node has 16 dedicated CPU cores and 32 GB of dedicated memory.
+        lindorm.c.8xlarge: Each node has 32 dedicated CPU cores and 64 GB of dedicated memory.
+        '''
+        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], jsii.get(self, "streamSpec"))
+
+    @stream_spec.setter
+    def stream_spec(
+        self,
+        value: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__953336a96f30f18e90987becc756cf008fe8232b7a0f5653a7a11b9c9a3d303d)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "streamSpec", value)
+
+    @builtins.property
     @jsii.member(jsii_name="tsdbNum")
     def tsdb_num(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]]:
         '''
         :Property:
 
@@ -1697,14 +1831,16 @@
         "lindorm_spec": "lindormSpec",
         "period": "period",
         "period_unit": "periodUnit",
         "resource_group_id": "resourceGroupId",
         "security_ip_list": "securityIpList",
         "solr_num": "solrNum",
         "solr_spec": "solrSpec",
+        "stream_num": "streamNum",
+        "stream_spec": "streamSpec",
         "tsdb_num": "tsdbNum",
         "tsdb_spec": "tsdbSpec",
         "v_switch_id": "vSwitchId",
         "zone_id": "zoneId",
     },
 )
 class RosInstanceProps:
@@ -1724,14 +1860,16 @@
         lindorm_spec: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
         period: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
         period_unit: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
         resource_group_id: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
         security_ip_list: typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Sequence[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]]] = None,
         solr_num: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
         solr_spec: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+        stream_num: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+        stream_spec: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
         tsdb_num: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
         tsdb_spec: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
         v_switch_id: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
         zone_id: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::Lindorm::Instance``.
 
@@ -1748,14 +1886,16 @@
         :param lindorm_spec: 
         :param period: 
         :param period_unit: 
         :param resource_group_id: 
         :param security_ip_list: 
         :param solr_num: 
         :param solr_spec: 
+        :param stream_num: 
+        :param stream_spec: 
         :param tsdb_num: 
         :param tsdb_spec: 
         :param v_switch_id: 
         :param zone_id: 
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__a57d16250ebff774e42262d8e93442c4bbc789278542c5c03b635ac424b1f47e)
@@ -1772,14 +1912,16 @@
             check_type(argname="argument lindorm_spec", value=lindorm_spec, expected_type=type_hints["lindorm_spec"])
             check_type(argname="argument period", value=period, expected_type=type_hints["period"])
             check_type(argname="argument period_unit", value=period_unit, expected_type=type_hints["period_unit"])
             check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
             check_type(argname="argument security_ip_list", value=security_ip_list, expected_type=type_hints["security_ip_list"])
             check_type(argname="argument solr_num", value=solr_num, expected_type=type_hints["solr_num"])
             check_type(argname="argument solr_spec", value=solr_spec, expected_type=type_hints["solr_spec"])
+            check_type(argname="argument stream_num", value=stream_num, expected_type=type_hints["stream_num"])
+            check_type(argname="argument stream_spec", value=stream_spec, expected_type=type_hints["stream_spec"])
             check_type(argname="argument tsdb_num", value=tsdb_num, expected_type=type_hints["tsdb_num"])
             check_type(argname="argument tsdb_spec", value=tsdb_spec, expected_type=type_hints["tsdb_spec"])
             check_type(argname="argument v_switch_id", value=v_switch_id, expected_type=type_hints["v_switch_id"])
             check_type(argname="argument zone_id", value=zone_id, expected_type=type_hints["zone_id"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "disk_category": disk_category,
             "instance_name": instance_name,
@@ -1809,14 +1951,18 @@
             self._values["resource_group_id"] = resource_group_id
         if security_ip_list is not None:
             self._values["security_ip_list"] = security_ip_list
         if solr_num is not None:
             self._values["solr_num"] = solr_num
         if solr_spec is not None:
             self._values["solr_spec"] = solr_spec
+        if stream_num is not None:
+            self._values["stream_num"] = stream_num
+        if stream_spec is not None:
+            self._values["stream_spec"] = stream_spec
         if tsdb_num is not None:
             self._values["tsdb_num"] = tsdb_num
         if tsdb_spec is not None:
             self._values["tsdb_spec"] = tsdb_spec
         if v_switch_id is not None:
             self._values["v_switch_id"] = v_switch_id
         if zone_id is not None:
@@ -2048,14 +2194,44 @@
         lindorm.g.4xlarge: Each node has 16 dedicated CPU cores and 64 GB of dedicated memory.
         lindorm.g.8xlarge: Each node has 32 dedicated CPU cores and 128 GB of dedicated memory.
         '''
         result = self._values.get("solr_spec")
         return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], result)
 
     @builtins.property
+    def stream_num(
+        self,
+    ) -> typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]]:
+        '''
+        :Property: streamNum: The number of LindormStream nodes in the instance. Valid values: integers from 0 to 90.
+        '''
+        result = self._values.get("stream_num")
+        return typing.cast(typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]], result)
+
+    @builtins.property
+    def stream_spec(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+        '''
+        :Property:
+
+        streamSpec: The specification of LindormStream nodes in the instance. Valid values:
+        lindorm.g.xlarge: Each node has 4 dedicated CPU cores and 16 GB of dedicated memory.
+        lindorm.g.2xlarge: Each node has 8 dedicated CPU cores and 32 GB of dedicated memory.
+        lindorm.g.4xlarge: Each node has 16 dedicated CPU cores and 64 GB of dedicated memory.
+        lindorm.g.8xlarge: Each node has 32 dedicated CPU cores and 128 GB of dedicated memory.
+        lindorm.c.xlarge: Each node has 4 dedicated CPU cores and 8 GB of dedicated memory.
+        lindorm.c.2xlarge: Each node has 8 dedicated CPU cores and 16 GB of dedicated memory.
+        lindorm.c.4xlarge: Each node has 16 dedicated CPU cores and 32 GB of dedicated memory.
+        lindorm.c.8xlarge: Each node has 32 dedicated CPU cores and 64 GB of dedicated memory.
+        '''
+        result = self._values.get("stream_spec")
+        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], result)
+
+    @builtins.property
     def tsdb_num(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]]:
         '''
         :Property:
 
         tsdbNum: The number of the LindormTSDB nodes in the instance. The valid values of this parameter depend on the value of the PayType parameter.
@@ -2830,14 +3006,64 @@
     ) -> None:
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__52cdc404db2b884d5cb78cda159a1edbfe9d7ea9207e5d2bf661cd7eb0d655f1)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "standbyZoneId", value)
 
     @builtins.property
+    @jsii.member(jsii_name="streamNum")
+    def stream_num(
+        self,
+    ) -> typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]]:
+        '''
+        :Property: streamNum: The number of LindormStream nodes in the instance. Valid values: integers from 0 to 90.
+        '''
+        return typing.cast(typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]], jsii.get(self, "streamNum"))
+
+    @stream_num.setter
+    def stream_num(
+        self,
+        value: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__d0f10592ffb397497a284d6087ca91d03e311fab91f29a4ad5c6a3fbf81f2794)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "streamNum", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="streamSpec")
+    def stream_spec(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+        '''
+        :Property:
+
+        streamSpec: The specification of LindormStream nodes in the instance. Valid values:
+        lindorm.g.xlarge: Each node has 4 dedicated CPU cores and 16 GB of dedicated memory.
+        lindorm.g.2xlarge: Each node has 8 dedicated CPU cores and 32 GB of dedicated memory.
+        lindorm.g.4xlarge: Each node has 16 dedicated CPU cores and 64 GB of dedicated memory.
+        lindorm.g.8xlarge: Each node has 32 dedicated CPU cores and 128 GB of dedicated memory.
+        lindorm.c.xlarge: Each node has 4 dedicated CPU cores and 8 GB of dedicated memory.
+        lindorm.c.2xlarge: Each node has 8 dedicated CPU cores and 16 GB of dedicated memory.
+        lindorm.c.4xlarge: Each node has 16 dedicated CPU cores and 32 GB of dedicated memory.
+        lindorm.c.8xlarge: Each node has 32 dedicated CPU cores and 64 GB of dedicated memory.
+        '''
+        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], jsii.get(self, "streamSpec"))
+
+    @stream_spec.setter
+    def stream_spec(
+        self,
+        value: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__9d037fcec3463b73ae3798cc316d06ddbcae5a1515a9a1df1712e55aeec0fc34)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "streamSpec", value)
+
+    @builtins.property
     @jsii.member(jsii_name="tsdbNum")
     def tsdb_num(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]]:
         '''
         :Property:
 
@@ -2912,14 +3138,16 @@
         "primary_zone_id": "primaryZoneId",
         "resource_group_id": "resourceGroupId",
         "security_ip_list": "securityIpList",
         "solr_num": "solrNum",
         "solr_spec": "solrSpec",
         "standby_v_switch_id": "standbyVSwitchId",
         "standby_zone_id": "standbyZoneId",
+        "stream_num": "streamNum",
+        "stream_spec": "streamSpec",
         "tsdb_num": "tsdbNum",
         "tsdb_spec": "tsdbSpec",
     },
 )
 class RosMultiZoneInstanceProps:
     def __init__(
         self,
@@ -2948,14 +3176,16 @@
         primary_zone_id: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
         resource_group_id: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
         security_ip_list: typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Sequence[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]]] = None,
         solr_num: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
         solr_spec: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
         standby_v_switch_id: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
         standby_zone_id: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+        stream_num: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+        stream_spec: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
         tsdb_num: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
         tsdb_spec: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::Lindorm::MultiZoneInstance``.
 
         :param disk_category: 
         :param instance_name: 
@@ -2981,14 +3211,16 @@
         :param primary_zone_id: 
         :param resource_group_id: 
         :param security_ip_list: 
         :param solr_num: 
         :param solr_spec: 
         :param standby_v_switch_id: 
         :param standby_zone_id: 
+        :param stream_num: 
+        :param stream_spec: 
         :param tsdb_num: 
         :param tsdb_spec: 
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__2001a5ccf709cbf3cad610cd92556fbc91a201c31965ce3a1926903ce0ffacc0)
             check_type(argname="argument disk_category", value=disk_category, expected_type=type_hints["disk_category"])
             check_type(argname="argument instance_name", value=instance_name, expected_type=type_hints["instance_name"])
@@ -3014,14 +3246,16 @@
             check_type(argname="argument primary_zone_id", value=primary_zone_id, expected_type=type_hints["primary_zone_id"])
             check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
             check_type(argname="argument security_ip_list", value=security_ip_list, expected_type=type_hints["security_ip_list"])
             check_type(argname="argument solr_num", value=solr_num, expected_type=type_hints["solr_num"])
             check_type(argname="argument solr_spec", value=solr_spec, expected_type=type_hints["solr_spec"])
             check_type(argname="argument standby_v_switch_id", value=standby_v_switch_id, expected_type=type_hints["standby_v_switch_id"])
             check_type(argname="argument standby_zone_id", value=standby_zone_id, expected_type=type_hints["standby_zone_id"])
+            check_type(argname="argument stream_num", value=stream_num, expected_type=type_hints["stream_num"])
+            check_type(argname="argument stream_spec", value=stream_spec, expected_type=type_hints["stream_spec"])
             check_type(argname="argument tsdb_num", value=tsdb_num, expected_type=type_hints["tsdb_num"])
             check_type(argname="argument tsdb_spec", value=tsdb_spec, expected_type=type_hints["tsdb_spec"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "disk_category": disk_category,
             "instance_name": instance_name,
             "vpc_id": vpc_id,
         }
@@ -3071,14 +3305,18 @@
             self._values["solr_num"] = solr_num
         if solr_spec is not None:
             self._values["solr_spec"] = solr_spec
         if standby_v_switch_id is not None:
             self._values["standby_v_switch_id"] = standby_v_switch_id
         if standby_zone_id is not None:
             self._values["standby_zone_id"] = standby_zone_id
+        if stream_num is not None:
+            self._values["stream_num"] = stream_num
+        if stream_spec is not None:
+            self._values["stream_spec"] = stream_spec
         if tsdb_num is not None:
             self._values["tsdb_num"] = tsdb_num
         if tsdb_spec is not None:
             self._values["tsdb_spec"] = tsdb_spec
 
     @builtins.property
     def disk_category(
@@ -3439,14 +3677,44 @@
         '''
         :Property: standbyZoneId: The ID of the secondary zone of the instance. **This parameter is required if you want to create a multi-zone instance.
         '''
         result = self._values.get("standby_zone_id")
         return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], result)
 
     @builtins.property
+    def stream_num(
+        self,
+    ) -> typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]]:
+        '''
+        :Property: streamNum: The number of LindormStream nodes in the instance. Valid values: integers from 0 to 90.
+        '''
+        result = self._values.get("stream_num")
+        return typing.cast(typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]], result)
+
+    @builtins.property
+    def stream_spec(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+        '''
+        :Property:
+
+        streamSpec: The specification of LindormStream nodes in the instance. Valid values:
+        lindorm.g.xlarge: Each node has 4 dedicated CPU cores and 16 GB of dedicated memory.
+        lindorm.g.2xlarge: Each node has 8 dedicated CPU cores and 32 GB of dedicated memory.
+        lindorm.g.4xlarge: Each node has 16 dedicated CPU cores and 64 GB of dedicated memory.
+        lindorm.g.8xlarge: Each node has 32 dedicated CPU cores and 128 GB of dedicated memory.
+        lindorm.c.xlarge: Each node has 4 dedicated CPU cores and 8 GB of dedicated memory.
+        lindorm.c.2xlarge: Each node has 8 dedicated CPU cores and 16 GB of dedicated memory.
+        lindorm.c.4xlarge: Each node has 16 dedicated CPU cores and 32 GB of dedicated memory.
+        lindorm.c.8xlarge: Each node has 32 dedicated CPU cores and 64 GB of dedicated memory.
+        '''
+        result = self._values.get("stream_spec")
+        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], result)
+
+    @builtins.property
     def tsdb_num(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]]:
         '''
         :Property:
 
         tsdbNum: The number of the LindormTSDB nodes in the instance. The valid values of this parameter depend on the value of the PayType parameter.
@@ -3521,14 +3789,16 @@
     lindorm_spec: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
     period: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
     period_unit: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
     resource_group_id: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
     security_ip_list: typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Sequence[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]]] = None,
     solr_num: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
     solr_spec: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+    stream_num: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+    stream_spec: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
     tsdb_num: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
     tsdb_spec: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
     v_switch_id: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
     zone_id: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
@@ -3568,14 +3838,16 @@
     primary_zone_id: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
     resource_group_id: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
     security_ip_list: typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Sequence[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]]] = None,
     solr_num: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
     solr_spec: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
     standby_v_switch_id: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
     standby_zone_id: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+    stream_num: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+    stream_spec: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
     tsdb_num: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
     tsdb_spec: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__44c2aef5450c841af44256a0fa84092e35023aa91ea2a17b4f43b5fa5b9ea2ab(
@@ -3697,14 +3969,26 @@
 
 def _typecheckingstub__7050bded188f218006bc64f861a891922641755eec0f856c8a74884c27b636bc(
     value: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]],
 ) -> None:
     """Type checking stubs"""
     pass
 
+def _typecheckingstub__cff9beb1b952eadb780012da5a270ba24852867d1480e869e736ed63a533f6d8(
+    value: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__953336a96f30f18e90987becc756cf008fe8232b7a0f5653a7a11b9c9a3d303d(
+    value: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]],
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__c5871cf034970d0c27561a3ddcbdffe693acb6009b28ce5c2019db28969b89eb(
     value: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]],
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__fab6233a734dc447ba67d4d89a3cea4fe76a00d5e9b39b97fb4ec2463f432603(
@@ -3740,14 +4024,16 @@
     lindorm_spec: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
     period: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
     period_unit: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
     resource_group_id: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
     security_ip_list: typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Sequence[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]]] = None,
     solr_num: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
     solr_spec: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+    stream_num: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+    stream_spec: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
     tsdb_num: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
     tsdb_spec: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
     v_switch_id: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
     zone_id: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
@@ -3937,14 +4223,26 @@
 
 def _typecheckingstub__52cdc404db2b884d5cb78cda159a1edbfe9d7ea9207e5d2bf661cd7eb0d655f1(
     value: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]],
 ) -> None:
     """Type checking stubs"""
     pass
 
+def _typecheckingstub__d0f10592ffb397497a284d6087ca91d03e311fab91f29a4ad5c6a3fbf81f2794(
+    value: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__9d037fcec3463b73ae3798cc316d06ddbcae5a1515a9a1df1712e55aeec0fc34(
+    value: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]],
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__c6b978a8c66f18dda16bc8beb91c81255ea725660b285e9621e249c8744fa317(
     value: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]],
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__689e2d503c0aace650f9a520a5f82753eebf04a022531e884ecd58f3b33f1478(
@@ -3979,12 +4277,14 @@
     primary_zone_id: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
     resource_group_id: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
     security_ip_list: typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Sequence[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]]] = None,
     solr_num: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
     solr_spec: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
     standby_v_switch_id: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
     standby_zone_id: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+    stream_num: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+    stream_spec: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
     tsdb_num: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
     tsdb_spec: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
```

### Comparing `ros-cdk-lindorm-1.0.12/src/ros_cdk_lindorm.egg-info/PKG-INFO` & `ros-cdk-lindorm-1.0.13/src/ros_cdk_lindorm.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-lindorm
-Version: 1.0.12
+Version: 1.0.13
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS LINDORM Construct Library
         
@@ -19,12 +19,13 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
```

