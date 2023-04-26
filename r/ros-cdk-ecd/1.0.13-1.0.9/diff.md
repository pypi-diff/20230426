# Comparing `tmp/ros-cdk-ecd-1.0.13.tar.gz` & `tmp/ros-cdk-ecd-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-ecd-1.0.13.tar", last modified: Wed Apr 26 07:24:04 2023, max compression
+gzip compressed data, was "dist/ros-cdk-ecd-1.0.9.tar", last modified: Fri Sep 23 12:05:44 2022, max compression
```

## Comparing `ros-cdk-ecd-1.0.13.tar` & `ros-cdk-ecd-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:24:04.000000 ros-cdk-ecd-1.0.13/
--rw-r--r--   0 root         (0) root         (0)    10279 2023-04-26 07:24:03.000000 ros-cdk-ecd-1.0.13/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2023-04-26 07:24:03.000000 ros-cdk-ecd-1.0.13/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2023-04-26 07:24:03.000000 ros-cdk-ecd-1.0.13/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1292 2023-04-26 07:24:04.000000 ros-cdk-ecd-1.0.13/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      179 2023-04-26 07:24:03.000000 ros-cdk-ecd-1.0.13/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2023-04-26 07:24:03.000000 ros-cdk-ecd-1.0.13/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-26 07:24:04.000000 ros-cdk-ecd-1.0.13/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1875 2023-04-26 07:24:03.000000 ros-cdk-ecd-1.0.13/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:24:04.000000 ros-cdk-ecd-1.0.13/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:24:04.000000 ros-cdk-ecd-1.0.13/src/ros_cdk_ecd/
--rw-r--r--   0 root         (0) root         (0)    92737 2023-04-26 07:24:03.000000 ros-cdk-ecd-1.0.13/src/ros_cdk_ecd/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:24:04.000000 ros-cdk-ecd-1.0.13/src/ros_cdk_ecd/_jsii/
--rw-r--r--   0 root         (0) root         (0)      406 2023-04-26 07:24:03.000000 ros-cdk-ecd-1.0.13/src/ros_cdk_ecd/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    48193 2023-04-26 07:24:03.000000 ros-cdk-ecd-1.0.13/src/ros_cdk_ecd/_jsii/ros-cdk-ecd@1.0.13.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 07:24:03.000000 ros-cdk-ecd-1.0.13/src/ros_cdk_ecd/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:24:04.000000 ros-cdk-ecd-1.0.13/src/ros_cdk_ecd.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1292 2023-04-26 07:24:04.000000 ros-cdk-ecd-1.0.13/src/ros_cdk_ecd.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      401 2023-04-26 07:24:04.000000 ros-cdk-ecd-1.0.13/src/ros_cdk_ecd.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 07:24:04.000000 ros-cdk-ecd-1.0.13/src/ros_cdk_ecd.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      109 2023-04-26 07:24:04.000000 ros-cdk-ecd-1.0.13/src/ros_cdk_ecd.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-04-26 07:24:04.000000 ros-cdk-ecd-1.0.13/src/ros_cdk_ecd.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:05:44.000000 ros-cdk-ecd-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)    10279 2022-09-23 12:05:44.000000 ros-cdk-ecd-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-09-23 12:05:44.000000 ros-cdk-ecd-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2022-09-23 12:05:44.000000 ros-cdk-ecd-1.0.9/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1240 2022-09-23 12:05:44.000000 ros-cdk-ecd-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      179 2022-09-23 12:05:44.000000 ros-cdk-ecd-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      236 2022-09-23 12:05:44.000000 ros-cdk-ecd-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-09-23 12:05:44.000000 ros-cdk-ecd-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1823 2022-09-23 12:05:44.000000 ros-cdk-ecd-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:05:44.000000 ros-cdk-ecd-1.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:05:44.000000 ros-cdk-ecd-1.0.9/src/ros_cdk_ecd/
+-rw-r--r--   0 root         (0) root         (0)    77818 2022-09-23 12:05:44.000000 ros-cdk-ecd-1.0.9/src/ros_cdk_ecd/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:05:44.000000 ros-cdk-ecd-1.0.9/src/ros_cdk_ecd/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      404 2022-09-23 12:05:44.000000 ros-cdk-ecd-1.0.9/src/ros_cdk_ecd/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    47917 2022-09-23 12:05:44.000000 ros-cdk-ecd-1.0.9/src/ros_cdk_ecd/_jsii/ros-cdk-ecd@1.0.9.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 12:05:44.000000 ros-cdk-ecd-1.0.9/src/ros_cdk_ecd/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:05:44.000000 ros-cdk-ecd-1.0.9/src/ros_cdk_ecd.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1240 2022-09-23 12:05:44.000000 ros-cdk-ecd-1.0.9/src/ros_cdk_ecd.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      400 2022-09-23 12:05:44.000000 ros-cdk-ecd-1.0.9/src/ros_cdk_ecd.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 12:05:44.000000 ros-cdk-ecd-1.0.9/src/ros_cdk_ecd.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2022-09-23 12:05:44.000000 ros-cdk-ecd-1.0.9/src/ros_cdk_ecd.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2022-09-23 12:05:44.000000 ros-cdk-ecd-1.0.9/src/ros_cdk_ecd.egg-info/top_level.txt
```

### Comparing `ros-cdk-ecd-1.0.13/LICENSE` & `ros-cdk-ecd-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-ecd-1.0.13/PKG-INFO` & `ros-cdk-ecd-1.0.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-ecd
-Version: 1.0.13
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS ECD Construct Library
         
@@ -19,13 +19,12 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
```

### Comparing `ros-cdk-ecd-1.0.13/setup.py` & `ros-cdk-ecd-1.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-ecd",
-    "version": "1.0.13",
+    "version": "1.0.9",
     "description": "Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com",
     "license": "Apache-2.0",
     "url": "https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git",
     "long_description_content_type": "text/markdown",
     "author": "ROS Development Team",
     "bdist_wheel": {
         "universal": true
@@ -22,38 +22,37 @@
     },
     "packages": [
         "ros_cdk_ecd",
         "ros_cdk_ecd._jsii"
     ],
     "package_data": {
         "ros_cdk_ecd._jsii": [
-            "ros-cdk-ecd@1.0.13.jsii.tgz"
+            "ros-cdk-ecd@1.0.9.jsii.tgz"
         ],
         "ros_cdk_ecd": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "constructs>=3.0.4, <4.0.0",
-        "jsii>=1.80.0, <2.0.0",
+        "jsii>=1.68.0, <2.0.0",
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
-        "Programming Language :: Python :: 3.11",
         "Typing :: Typed",
         "License :: OSI Approved",
         "Programming Language :: Python :: 3"
     ],
     "scripts": []
 }
 """
```

### Comparing `ros-cdk-ecd-1.0.13/src/ros_cdk_ecd/__init__.py` & `ros-cdk-ecd-1.0.9/src/ros_cdk_ecd/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,68 +17,68 @@
 import publication
 import typing_extensions
 
 from typeguard import check_type
 
 from ._jsii import *
 
-import ros_cdk_core as _ros_cdk_core_7adfd82f
+import ros_cdk_core
 
 
 class Desktops(
-    _ros_cdk_core_7adfd82f.Resource,
+    ros_cdk_core.Resource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-ecd.Desktops",
 ):
     '''A ROS resource type:  ``ALIYUN::ECD::Desktops``.'''
 
     def __init__(
         self,
-        scope: _ros_cdk_core_7adfd82f.Construct,
+        scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: typing.Union["DesktopsProps", typing.Dict[builtins.str, typing.Any]],
+        props: typing.Union["DesktopsProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::ECD::Desktops``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__ec37c66f272ac3085a407b8d35ffcaba92b80787d8d0d51b5c7359202f24a177)
+            type_hints = typing.get_type_hints(Desktops.__init__)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
             check_type(argname="argument props", value=props, expected_type=type_hints["props"])
             check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
     @builtins.property
     @jsii.member(jsii_name="attrDesktopId")
-    def attr_desktop_id(self) -> _ros_cdk_core_7adfd82f.IResolvable:
+    def attr_desktop_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute DesktopId: The ID of the cloud desktop.
 
         If multiple cloud desktops are created in a call, the
         IDs of the cloud desktops are returned.
         '''
-        return typing.cast(_ros_cdk_core_7adfd82f.IResolvable, jsii.get(self, "attrDesktopId"))
+        return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDesktopId"))
 
     @builtins.property
     @jsii.member(jsii_name="attrOrderId")
-    def attr_order_id(self) -> _ros_cdk_core_7adfd82f.IResolvable:
+    def attr_order_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute OrderId: The ID of the order.
 
         Note This parameter is returned only when the ChargeType parameter is set to PrePaid.
         '''
-        return typing.cast(_ros_cdk_core_7adfd82f.IResolvable, jsii.get(self, "attrOrderId"))
+        return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrOrderId"))
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-ecd.DesktopsProps",
     jsii_struct_bases=[],
     name_mapping={
         "bundle_id": "bundleId",
@@ -105,36 +105,36 @@
         "vpc_id": "vpcId",
     },
 )
 class DesktopsProps:
     def __init__(
         self,
         *,
-        bundle_id: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
-        office_site_id: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
-        policy_group_id: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
-        amount: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-        auto_pay: typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-        auto_renew: typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-        charge_type: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-        desktop_name: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-        desktop_name_suffix: typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-        directory_id: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-        end_user_id: typing.Optional[typing.Union[typing.Sequence[typing.Any], _ros_cdk_core_7adfd82f.IResolvable]] = None,
-        group_id: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-        hostname: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-        period: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-        period_unit: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-        promotion_id: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-        tags: typing.Optional[typing.Sequence[typing.Union["RosDesktops.TagsProperty", typing.Dict[builtins.str, typing.Any]]]] = None,
-        user_assign_mode: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-        user_name: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-        volume_encryption_enabled: typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-        volume_encryption_key: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-        vpc_id: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+        bundle_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
+        office_site_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
+        policy_group_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
+        amount: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
+        auto_pay: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
+        auto_renew: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
+        charge_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
+        desktop_name: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
+        desktop_name_suffix: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
+        directory_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
+        end_user_id: typing.Optional[typing.Union[typing.Sequence[typing.Any], ros_cdk_core.IResolvable]] = None,
+        group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
+        hostname: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
+        period: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
+        period_unit: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
+        promotion_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union["RosDesktops.TagsProperty", typing.Dict[str, typing.Any]]]] = None,
+        user_assign_mode: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
+        user_name: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
+        volume_encryption_enabled: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
+        volume_encryption_key: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
+        vpc_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::ECD::Desktops``.
 
         :param bundle_id: Property bundleId: The ID of the cloud desktop template.
         :param office_site_id: Property officeSiteId: The ID of the workspace.
         :param policy_group_id: Property policyGroupId: The ID of the policy.
         :param amount: Property amount: The number of cloud desktops that you want to create. Valid values: 1 to 300. Default value: 1.
@@ -154,15 +154,15 @@
         :param user_assign_mode: Property userAssignMode: The assignment mode of the cloud desktop. Default value: ALL. ALL: If you specify the EndUserId parameter, the cloud desktops that you create are assigned to each regular user that you specify. PER_USER: If you specify the EndUserId parameter, the cloud desktops that you create are evenly assigned to all regular users that you specify. In this case, you must make sure that the value of the Amount parameter can be divided by the N value of the EndUserId.N parameter that you specify. Note If you do not specify the EndUserId parameter, the cloud desktop that you create is not assigned to regular users.
         :param user_name: Property userName: This parameter is not open for use.
         :param volume_encryption_enabled: Property volumeEncryptionEnabled: Whether to enable disk encryption.
         :param volume_encryption_key: Property volumeEncryptionKey: The key ID of the KMS used when disk encryption is enabled. It can be obtained through the ListKeys interface.
         :param vpc_id: Property vpcId: This parameter is not open for use.
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__5332608fe20f2b15df3518e820c058e964555fd1f537a8c2ee1a652ea3eccf1f)
+            type_hints = typing.get_type_hints(DesktopsProps.__init__)
             check_type(argname="argument bundle_id", value=bundle_id, expected_type=type_hints["bundle_id"])
             check_type(argname="argument office_site_id", value=office_site_id, expected_type=type_hints["office_site_id"])
             check_type(argname="argument policy_group_id", value=policy_group_id, expected_type=type_hints["policy_group_id"])
             check_type(argname="argument amount", value=amount, expected_type=type_hints["amount"])
             check_type(argname="argument auto_pay", value=auto_pay, expected_type=type_hints["auto_pay"])
             check_type(argname="argument auto_renew", value=auto_renew, expected_type=type_hints["auto_renew"])
             check_type(argname="argument charge_type", value=charge_type, expected_type=type_hints["charge_type"])
@@ -177,15 +177,15 @@
             check_type(argname="argument promotion_id", value=promotion_id, expected_type=type_hints["promotion_id"])
             check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
             check_type(argname="argument user_assign_mode", value=user_assign_mode, expected_type=type_hints["user_assign_mode"])
             check_type(argname="argument user_name", value=user_name, expected_type=type_hints["user_name"])
             check_type(argname="argument volume_encryption_enabled", value=volume_encryption_enabled, expected_type=type_hints["volume_encryption_enabled"])
             check_type(argname="argument volume_encryption_key", value=volume_encryption_key, expected_type=type_hints["volume_encryption_key"])
             check_type(argname="argument vpc_id", value=vpc_id, expected_type=type_hints["vpc_id"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "bundle_id": bundle_id,
             "office_site_id": office_site_id,
             "policy_group_id": policy_group_id,
         }
         if amount is not None:
             self._values["amount"] = amount
         if auto_pay is not None:
@@ -222,156 +222,150 @@
             self._values["volume_encryption_enabled"] = volume_encryption_enabled
         if volume_encryption_key is not None:
             self._values["volume_encryption_key"] = volume_encryption_key
         if vpc_id is not None:
             self._values["vpc_id"] = vpc_id
 
     @builtins.property
-    def bundle_id(
-        self,
-    ) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+    def bundle_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''Property bundleId: The ID of the cloud desktop template.'''
         result = self._values.get("bundle_id")
         assert result is not None, "Required property 'bundle_id' is missing"
-        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], result)
+        return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], result)
 
     @builtins.property
-    def office_site_id(
-        self,
-    ) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+    def office_site_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''Property officeSiteId: The ID of the workspace.'''
         result = self._values.get("office_site_id")
         assert result is not None, "Required property 'office_site_id' is missing"
-        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], result)
+        return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], result)
 
     @builtins.property
-    def policy_group_id(
-        self,
-    ) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+    def policy_group_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''Property policyGroupId: The ID of the policy.'''
         result = self._values.get("policy_group_id")
         assert result is not None, "Required property 'policy_group_id' is missing"
-        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], result)
+        return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], result)
 
     @builtins.property
     def amount(
         self,
-    ) -> typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]]:
+    ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''Property amount: The number of cloud desktops that you want to create.
 
         Valid values: 1 to 300. Default
         value: 1.
         '''
         result = self._values.get("amount")
-        return typing.cast(typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]], result)
+        return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], result)
 
     @builtins.property
     def auto_pay(
         self,
-    ) -> typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]]:
+    ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''Property autoPay: Specifies whether to enable automatic payment.
 
         Valid values:
         true: enables automatic payment. You must make sure that your Alibaba Cloud account
         has sufficient balance. If your Alibaba Cloud account does not have sufficient balance,
         abnormal orders are generated.
         false: disables automatic payment. In this case, an order is generated, and no payment
         is automatically made. You can log on to the EDS console and complete the payment
         based on the order ID on the Orders page.
         Default value: true.
         '''
         result = self._values.get("auto_pay")
-        return typing.cast(typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]], result)
+        return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], result)
 
     @builtins.property
     def auto_renew(
         self,
-    ) -> typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]]:
+    ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''Property autoRenew: Specifies whether to enable auto-renewal for the cloud desktop.
 
         This parameter takes
         effect only when the ChargeType parameter is set to PrePaid.
         Valid values:
         true: enables auto-renewal. The renewal duration is the same as the subscription duration
         that you specified for the Period parameter when you purchased the cloud desktop.
         false: does not enable auto-renewal.
         Default value: false.
         '''
         result = self._values.get("auto_renew")
-        return typing.cast(typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]], result)
+        return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], result)
 
     @builtins.property
     def charge_type(
         self,
-    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+    ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''Property chargeType: The billing method of the cloud desktop.
 
         Valid values:
         PostPaid: pay-as-you-go
         PrePaid: subscription
         Default value: PostPaid.
         '''
         result = self._values.get("charge_type")
-        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], result)
+        return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], result)
 
     @builtins.property
     def desktop_name(
         self,
-    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+    ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''Property desktopName: The name of the cloud desktop.'''
         result = self._values.get("desktop_name")
-        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], result)
+        return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], result)
 
     @builtins.property
     def desktop_name_suffix(
         self,
-    ) -> typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]]:
+    ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''Property desktopNameSuffix: Specifies whether to automatically add a suffix to the cloud desktop name when you create multiple cloud desktops at a time.
 
         True: automatically adds a suffix.
         False: does not add a suffix.
         '''
         result = self._values.get("desktop_name_suffix")
-        return typing.cast(typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]], result)
+        return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], result)
 
     @builtins.property
     def directory_id(
         self,
-    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+    ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''Property directoryId: This parameter is not open for use.'''
         result = self._values.get("directory_id")
-        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], result)
+        return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], result)
 
     @builtins.property
     def end_user_id(
         self,
-    ) -> typing.Optional[typing.Union[typing.List[typing.Any], _ros_cdk_core_7adfd82f.IResolvable]]:
+    ) -> typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]]:
         '''Property endUserId: The user ID that authorizes the use of the cloud desktop, 1~100 can be set.
 
         During the same period, only one user can use the desktop.
         If EndUserId is not set, the created cloud desktop will not be assigned to any user.
         '''
         result = self._values.get("end_user_id")
-        return typing.cast(typing.Optional[typing.Union[typing.List[typing.Any], _ros_cdk_core_7adfd82f.IResolvable]], result)
+        return typing.cast(typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]], result)
 
     @builtins.property
     def group_id(
         self,
-    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+    ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''Property groupId: desktop group ID。 Note that the desktop group function is currently in the invitation test.
 
         If you want to experience it, please submit a work order application.
         '''
         result = self._values.get("group_id")
-        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], result)
+        return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], result)
 
     @builtins.property
     def hostname(
         self,
-    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+    ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''Property hostname: The custom hostname that you specify for the cloud desktop.
 
         You can only specify the
         hostname of a Windows cloud desktop in the workspace of the enterprise AD account
         type.
         The hostname must meet the following requirements:
         The hostname must be 2 to 15 characters in length.
@@ -383,149 +377,149 @@
         name_prefix: the prefix of the hostname.
         [begin_number,bits]: the ordered numbers in the hostname. begin_number: the start number. Valid values:
         0 to 999999. Default value: 0. bits: the digit. Valid values: 1 to 6. Default value:
         6.
         name_suffix: the suffix of the hostname.
         '''
         result = self._values.get("hostname")
-        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], result)
+        return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], result)
 
     @builtins.property
     def period(
         self,
-    ) -> typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]]:
+    ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''Property period: The subscription duration.
 
         The unit of the value is specified by the PeriodUnit parameter. This parameter takes effect and is required only when the ChargeType parameter is set to PrePaid.
         If PeriodUnit is month, the valid range is 1, 2, 3, 6, 12, 24, 36, 48,60
         If periodUnit is year, the valid range is 1 to 5
         '''
         result = self._values.get("period")
-        return typing.cast(typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]], result)
+        return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], result)
 
     @builtins.property
     def period_unit(
         self,
-    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+    ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''Property periodUnit: The unit of the subscription duration.
 
         Valid values:
         Month
         Year
         Default value: Month.
         '''
         result = self._values.get("period_unit")
-        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], result)
+        return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], result)
 
     @builtins.property
     def promotion_id(
         self,
-    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+    ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''Property promotionId: promotion id.'''
         result = self._values.get("promotion_id")
-        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], result)
+        return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], result)
 
     @builtins.property
     def tags(self) -> typing.Optional[typing.List["RosDesktops.TagsProperty"]]:
         '''Property tags: The list of desktops tags in the form of key/value pairs.
 
         You can define a maximum of 20 tags for each desktops.
         '''
         result = self._values.get("tags")
         return typing.cast(typing.Optional[typing.List["RosDesktops.TagsProperty"]], result)
 
     @builtins.property
     def user_assign_mode(
         self,
-    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+    ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''Property userAssignMode: The assignment mode of the cloud desktop.
 
         Default value: ALL.
         ALL: If you specify the EndUserId parameter, the cloud desktops that you create are
         assigned to each regular user that you specify.
         PER_USER: If you specify the EndUserId parameter, the cloud desktops that you create
         are evenly assigned to all regular users that you specify. In this case, you must
         make sure that the value of the Amount parameter can be divided by the N value of
         the EndUserId.N parameter that you specify.
         Note If you do not specify the EndUserId parameter, the cloud desktop that you create is
         not assigned to regular users.
         '''
         result = self._values.get("user_assign_mode")
-        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], result)
+        return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], result)
 
     @builtins.property
     def user_name(
         self,
-    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+    ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''Property userName: This parameter is not open for use.'''
         result = self._values.get("user_name")
-        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], result)
+        return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], result)
 
     @builtins.property
     def volume_encryption_enabled(
         self,
-    ) -> typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]]:
+    ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''Property volumeEncryptionEnabled: Whether to enable disk encryption.'''
         result = self._values.get("volume_encryption_enabled")
-        return typing.cast(typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]], result)
+        return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], result)
 
     @builtins.property
     def volume_encryption_key(
         self,
-    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+    ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''Property volumeEncryptionKey: The key ID of the KMS used when disk encryption is enabled.
 
         It can be obtained through the ListKeys interface.
         '''
         result = self._values.get("volume_encryption_key")
-        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], result)
+        return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], result)
 
     @builtins.property
     def vpc_id(
         self,
-    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+    ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''Property vpcId: This parameter is not open for use.'''
         result = self._values.get("vpc_id")
-        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], result)
+        return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
         return "DesktopsProps(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 class RosDesktops(
-    _ros_cdk_core_7adfd82f.RosResource,
+    ros_cdk_core.RosResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-ecd.RosDesktops",
 ):
     '''A ROS template type:  ``ALIYUN::ECD::Desktops``.'''
 
     def __init__(
         self,
-        scope: _ros_cdk_core_7adfd82f.Construct,
+        scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: typing.Union["RosDesktopsProps", typing.Dict[builtins.str, typing.Any]],
+        props: typing.Union["RosDesktopsProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::ECD::Desktops``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__417ba7a4919468974fae3406c865d7692c3a1a949d5b355c09b558638caceafa)
+            type_hints = typing.get_type_hints(RosDesktops.__init__)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
             check_type(argname="argument props", value=props, expected_type=type_hints["props"])
             check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
     @jsii.member(jsii_name="renderProperties")
@@ -533,346 +527,340 @@
         self,
         props: typing.Mapping[builtins.str, typing.Any],
     ) -> typing.Mapping[builtins.str, typing.Any]:
         '''
         :param props: -
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__b624a05db13321856dd462567d9a3ad708c91bb6c198de57d60f45c71a4870a7)
+            type_hints = typing.get_type_hints(RosDesktops._render_properties)
             check_type(argname="argument props", value=props, expected_type=type_hints["props"])
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.invoke(self, "renderProperties", [props]))
 
     @jsii.python.classproperty
     @jsii.member(jsii_name="ROS_RESOURCE_TYPE_NAME")
     def ROS_RESOURCE_TYPE_NAME(cls) -> builtins.str:
         '''The resource type name for this resource class.'''
         return typing.cast(builtins.str, jsii.sget(cls, "ROS_RESOURCE_TYPE_NAME"))
 
     @builtins.property
     @jsii.member(jsii_name="attrDesktopId")
-    def attr_desktop_id(self) -> _ros_cdk_core_7adfd82f.IResolvable:
+    def attr_desktop_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute:
 
         DesktopId: The ID of the cloud desktop. If multiple cloud desktops are created in a call, the
         IDs of the cloud desktops are returned.
         '''
-        return typing.cast(_ros_cdk_core_7adfd82f.IResolvable, jsii.get(self, "attrDesktopId"))
+        return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDesktopId"))
 
     @builtins.property
     @jsii.member(jsii_name="attrOrderId")
-    def attr_order_id(self) -> _ros_cdk_core_7adfd82f.IResolvable:
+    def attr_order_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute:
 
         OrderId: The ID of the order.
         Note This parameter is returned only when the ChargeType parameter is set to PrePaid.
         '''
-        return typing.cast(_ros_cdk_core_7adfd82f.IResolvable, jsii.get(self, "attrOrderId"))
+        return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrOrderId"))
 
     @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
     @builtins.property
     @jsii.member(jsii_name="bundleId")
-    def bundle_id(
-        self,
-    ) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+    def bundle_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: bundleId: The ID of the cloud desktop template.
         '''
-        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], jsii.get(self, "bundleId"))
+        return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "bundleId"))
 
     @bundle_id.setter
     def bundle_id(
         self,
-        value: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+        value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__048b5d93ea8fc94711fe40ab7cf22c025c4ee6ff7683ef25515076bbb2be14bb)
+            type_hints = typing.get_type_hints(getattr(RosDesktops, "bundle_id").fset)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "bundleId", value)
 
     @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__53c97614d89ca8bff4b5f500d1195b274c82ced15a9c6526f7bb7501a8b284ff)
+            type_hints = typing.get_type_hints(getattr(RosDesktops, "enable_resource_property_constraint").fset)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
     @builtins.property
     @jsii.member(jsii_name="officeSiteId")
-    def office_site_id(
-        self,
-    ) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+    def office_site_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: officeSiteId: The ID of the workspace.
         '''
-        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], jsii.get(self, "officeSiteId"))
+        return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "officeSiteId"))
 
     @office_site_id.setter
     def office_site_id(
         self,
-        value: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+        value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__813dc4087bed123200c90e6001e5b59681e81e158701e1f799745da3bf0b494a)
+            type_hints = typing.get_type_hints(getattr(RosDesktops, "office_site_id").fset)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "officeSiteId", value)
 
     @builtins.property
     @jsii.member(jsii_name="policyGroupId")
-    def policy_group_id(
-        self,
-    ) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+    def policy_group_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: policyGroupId: The ID of the policy.
         '''
-        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], jsii.get(self, "policyGroupId"))
+        return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "policyGroupId"))
 
     @policy_group_id.setter
     def policy_group_id(
         self,
-        value: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+        value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__6dcfd566820091b1c87bdee82e9d2372f9bd9c71f5f368af8c3082894cd2c6ca)
+            type_hints = typing.get_type_hints(getattr(RosDesktops, "policy_group_id").fset)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "policyGroupId", value)
 
     @builtins.property
     @jsii.member(jsii_name="amount")
     def amount(
         self,
-    ) -> typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]]:
+    ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
         amount: The number of cloud desktops that you want to create. Valid values: 1 to 300. Default
         value: 1.
         '''
-        return typing.cast(typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]], jsii.get(self, "amount"))
+        return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "amount"))
 
     @amount.setter
     def amount(
         self,
-        value: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]],
+        value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__a676556ac09d4910dab532df18cdebcc18e642ba62cc02850c6fae39a3f2ae5e)
+            type_hints = typing.get_type_hints(getattr(RosDesktops, "amount").fset)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "amount", value)
 
     @builtins.property
     @jsii.member(jsii_name="autoPay")
     def auto_pay(
         self,
-    ) -> typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]]:
+    ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
         autoPay: Specifies whether to enable automatic payment. Valid values:
         true: enables automatic payment. You must make sure that your Alibaba Cloud account
         has sufficient balance. If your Alibaba Cloud account does not have sufficient balance,
         abnormal orders are generated.
         false: disables automatic payment. In this case, an order is generated, and no payment
         is automatically made. You can log on to the EDS console and complete the payment
         based on the order ID on the Orders page.
         Default value: true.
         '''
-        return typing.cast(typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]], jsii.get(self, "autoPay"))
+        return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "autoPay"))
 
     @auto_pay.setter
     def auto_pay(
         self,
-        value: typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]],
+        value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__7bc2c01e82d9da5faf2c641d27e431bb87309d64cae517485ebc64f7f2058746)
+            type_hints = typing.get_type_hints(getattr(RosDesktops, "auto_pay").fset)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "autoPay", value)
 
     @builtins.property
     @jsii.member(jsii_name="autoRenew")
     def auto_renew(
         self,
-    ) -> typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]]:
+    ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
         autoRenew: Specifies whether to enable auto-renewal for the cloud desktop. This parameter takes
         effect only when the ChargeType parameter is set to PrePaid.
         Valid values:
         true: enables auto-renewal. The renewal duration is the same as the subscription duration
         that you specified for the Period parameter when you purchased the cloud desktop.
         false: does not enable auto-renewal.
         Default value: false.
         '''
-        return typing.cast(typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]], jsii.get(self, "autoRenew"))
+        return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "autoRenew"))
 
     @auto_renew.setter
     def auto_renew(
         self,
-        value: typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]],
+        value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__a01a9833dcc516e65e558219e84f6025560a064385c6b0682c09ec036609a73f)
+            type_hints = typing.get_type_hints(getattr(RosDesktops, "auto_renew").fset)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "autoRenew", value)
 
     @builtins.property
     @jsii.member(jsii_name="chargeType")
     def charge_type(
         self,
-    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+    ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
         chargeType: The billing method of the cloud desktop. Valid values:
         PostPaid: pay-as-you-go
         PrePaid: subscription
         Default value: PostPaid.
         '''
-        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], jsii.get(self, "chargeType"))
+        return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "chargeType"))
 
     @charge_type.setter
     def charge_type(
         self,
-        value: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]],
+        value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__620ea32e2bebfb20528329b3ae5831f322597d95dd5795fc6ce5bee4e33fbec1)
+            type_hints = typing.get_type_hints(getattr(RosDesktops, "charge_type").fset)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "chargeType", value)
 
     @builtins.property
     @jsii.member(jsii_name="desktopName")
     def desktop_name(
         self,
-    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+    ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: desktopName: The name of the cloud desktop.
         '''
-        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], jsii.get(self, "desktopName"))
+        return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "desktopName"))
 
     @desktop_name.setter
     def desktop_name(
         self,
-        value: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]],
+        value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__ba1aef65181db1a0051b7cc3e0f5210af5f1dbd8fa8c013e17672a3e3097bfb8)
+            type_hints = typing.get_type_hints(getattr(RosDesktops, "desktop_name").fset)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "desktopName", value)
 
     @builtins.property
     @jsii.member(jsii_name="desktopNameSuffix")
     def desktop_name_suffix(
         self,
-    ) -> typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]]:
+    ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
         desktopNameSuffix: Specifies whether to automatically add a suffix to the cloud desktop name when you
         create multiple cloud desktops at a time.
         True: automatically adds a suffix.
         False: does not add a suffix.
         '''
-        return typing.cast(typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]], jsii.get(self, "desktopNameSuffix"))
+        return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "desktopNameSuffix"))
 
     @desktop_name_suffix.setter
     def desktop_name_suffix(
         self,
-        value: typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]],
+        value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__cb9b2fc5b5c218d0643028d9afe2982405bb6181e5f40c3fac2ab6ef84a213c3)
+            type_hints = typing.get_type_hints(getattr(RosDesktops, "desktop_name_suffix").fset)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "desktopNameSuffix", value)
 
     @builtins.property
     @jsii.member(jsii_name="directoryId")
     def directory_id(
         self,
-    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+    ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: directoryId: This parameter is not open for use.
         '''
-        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], jsii.get(self, "directoryId"))
+        return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "directoryId"))
 
     @directory_id.setter
     def directory_id(
         self,
-        value: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]],
+        value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__299e31b65fffb8bf0e3c2a70ffef743e730d8ee5a59d2a19eb5338e5074f6af1)
+            type_hints = typing.get_type_hints(getattr(RosDesktops, "directory_id").fset)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "directoryId", value)
 
     @builtins.property
     @jsii.member(jsii_name="endUserId")
     def end_user_id(
         self,
-    ) -> typing.Optional[typing.Union[typing.List[typing.Any], _ros_cdk_core_7adfd82f.IResolvable]]:
+    ) -> typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
         endUserId: The user ID that authorizes the use of the cloud desktop, 1~100 can be set.
         During the same period, only one user can use the desktop.
         If EndUserId is not set, the created cloud desktop will not be assigned to any user.
         '''
-        return typing.cast(typing.Optional[typing.Union[typing.List[typing.Any], _ros_cdk_core_7adfd82f.IResolvable]], jsii.get(self, "endUserId"))
+        return typing.cast(typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]], jsii.get(self, "endUserId"))
 
     @end_user_id.setter
     def end_user_id(
         self,
-        value: typing.Optional[typing.Union[typing.List[typing.Any], _ros_cdk_core_7adfd82f.IResolvable]],
+        value: typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]],
     ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__5d4b497cb011a6133f7608707bb91cac249a69db83f38626801318f3f6e9392e)
+            type_hints = typing.get_type_hints(getattr(RosDesktops, "end_user_id").fset)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "endUserId", value)
 
     @builtins.property
     @jsii.member(jsii_name="groupId")
     def group_id(
         self,
-    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+    ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
         groupId: desktop group ID。
         Note that the desktop group function is currently in the invitation test.
         If you want to experience it, please submit a work order application.
         '''
-        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], jsii.get(self, "groupId"))
+        return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "groupId"))
 
     @group_id.setter
     def group_id(
         self,
-        value: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]],
+        value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__c8b32d925398e6519b7f4d80de38a1bf3f7de314b43ee6ba21765eb8ae7a1dbc)
+            type_hints = typing.get_type_hints(getattr(RosDesktops, "group_id").fset)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "groupId", value)
 
     @builtins.property
     @jsii.member(jsii_name="hostname")
     def hostname(
         self,
-    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+    ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
         hostname: The custom hostname that you specify for the cloud desktop. You can only specify the
         hostname of a Windows cloud desktop in the workspace of the enterprise AD account
         type.
         The hostname must meet the following requirements:
@@ -884,92 +872,92 @@
         the second cloud desktop is ecd-0002-test. The rest may be deduced by analogy.
         name_prefix: the prefix of the hostname.
         [begin_number,bits]: the ordered numbers in the hostname. begin_number: the start number. Valid values:
         0 to 999999. Default value: 0. bits: the digit. Valid values: 1 to 6. Default value:
         6.
         name_suffix: the suffix of the hostname.
         '''
-        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], jsii.get(self, "hostname"))
+        return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "hostname"))
 
     @hostname.setter
     def hostname(
         self,
-        value: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]],
+        value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__86cc34c87e1c2d81e79d6309023c565598f2d9c44110b32f00b9d82daf639295)
+            type_hints = typing.get_type_hints(getattr(RosDesktops, "hostname").fset)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "hostname", value)
 
     @builtins.property
     @jsii.member(jsii_name="period")
     def period(
         self,
-    ) -> typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]]:
+    ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
         period: The subscription duration. The unit of the value is specified by the PeriodUnit parameter. This parameter takes effect and is required only when the ChargeType parameter is set to PrePaid.
         If PeriodUnit is month, the valid range is 1, 2, 3, 6, 12, 24, 36, 48,60
         If periodUnit is year, the valid range is 1 to 5
         '''
-        return typing.cast(typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]], jsii.get(self, "period"))
+        return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "period"))
 
     @period.setter
     def period(
         self,
-        value: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]],
+        value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__d6bd5b5fa770c89aa3aa5866d160c1a2a08ba6b88c074843c007d66a8a937f27)
+            type_hints = typing.get_type_hints(getattr(RosDesktops, "period").fset)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "period", value)
 
     @builtins.property
     @jsii.member(jsii_name="periodUnit")
     def period_unit(
         self,
-    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+    ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
         periodUnit: The unit of the subscription duration. Valid values:
         Month
         Year
         Default value: Month.
         '''
-        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], jsii.get(self, "periodUnit"))
+        return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "periodUnit"))
 
     @period_unit.setter
     def period_unit(
         self,
-        value: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]],
+        value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__fdef60d1614d2f3601a4bd4bd6a28252405455eace4fce908fdd14f9197fc70c)
+            type_hints = typing.get_type_hints(getattr(RosDesktops, "period_unit").fset)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "periodUnit", value)
 
     @builtins.property
     @jsii.member(jsii_name="promotionId")
     def promotion_id(
         self,
-    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+    ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: promotionId: promotion id.
         '''
-        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], jsii.get(self, "promotionId"))
+        return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "promotionId"))
 
     @promotion_id.setter
     def promotion_id(
         self,
-        value: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]],
+        value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__efbba2fa69ae3743174c96210025457253685466a96aa6f91227befb135ab991)
+            type_hints = typing.get_type_hints(getattr(RosDesktops, "promotion_id").fset)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "promotionId", value)
 
     @builtins.property
     @jsii.member(jsii_name="tags")
     def tags(self) -> typing.Optional[typing.List["RosDesktops.TagsProperty"]]:
         '''
@@ -982,172 +970,172 @@
 
     @tags.setter
     def tags(
         self,
         value: typing.Optional[typing.List["RosDesktops.TagsProperty"]],
     ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__0fc2002b918d8a09ef269bd8d5b1d1168a20bed25d8494172f6e04a152020f7c)
+            type_hints = typing.get_type_hints(getattr(RosDesktops, "tags").fset)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "tags", value)
 
     @builtins.property
     @jsii.member(jsii_name="userAssignMode")
     def user_assign_mode(
         self,
-    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+    ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
         userAssignMode: The assignment mode of the cloud desktop. Default value: ALL.
         ALL: If you specify the EndUserId parameter, the cloud desktops that you create are
         assigned to each regular user that you specify.
         PER_USER: If you specify the EndUserId parameter, the cloud desktops that you create
         are evenly assigned to all regular users that you specify. In this case, you must
         make sure that the value of the Amount parameter can be divided by the N value of
         the EndUserId.N parameter that you specify.
         Note If you do not specify the EndUserId parameter, the cloud desktop that you create is
         not assigned to regular users.
         '''
-        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], jsii.get(self, "userAssignMode"))
+        return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "userAssignMode"))
 
     @user_assign_mode.setter
     def user_assign_mode(
         self,
-        value: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]],
+        value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__b55294dbcbbf93862814b175eed541beb9ed8c6f90030c0bff94c21b4e032dcb)
+            type_hints = typing.get_type_hints(getattr(RosDesktops, "user_assign_mode").fset)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "userAssignMode", value)
 
     @builtins.property
     @jsii.member(jsii_name="userName")
     def user_name(
         self,
-    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+    ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: userName: This parameter is not open for use.
         '''
-        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], jsii.get(self, "userName"))
+        return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "userName"))
 
     @user_name.setter
     def user_name(
         self,
-        value: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]],
+        value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__441b1f7f1911342bb501926092bcdd57fbd727f261eb2e95b2cb2b03000004d0)
+            type_hints = typing.get_type_hints(getattr(RosDesktops, "user_name").fset)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "userName", value)
 
     @builtins.property
     @jsii.member(jsii_name="volumeEncryptionEnabled")
     def volume_encryption_enabled(
         self,
-    ) -> typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]]:
+    ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: volumeEncryptionEnabled: Whether to enable disk encryption.
         '''
-        return typing.cast(typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]], jsii.get(self, "volumeEncryptionEnabled"))
+        return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "volumeEncryptionEnabled"))
 
     @volume_encryption_enabled.setter
     def volume_encryption_enabled(
         self,
-        value: typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]],
+        value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__0a1a5e8e1790c293746b5cbcd705b50d46a2e3226ad2e9bb108b7dea7e08ce38)
+            type_hints = typing.get_type_hints(getattr(RosDesktops, "volume_encryption_enabled").fset)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "volumeEncryptionEnabled", value)
 
     @builtins.property
     @jsii.member(jsii_name="volumeEncryptionKey")
     def volume_encryption_key(
         self,
-    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+    ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: volumeEncryptionKey: The key ID of the KMS used when disk encryption is enabled. It can be obtained through the ListKeys interface.
         '''
-        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], jsii.get(self, "volumeEncryptionKey"))
+        return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "volumeEncryptionKey"))
 
     @volume_encryption_key.setter
     def volume_encryption_key(
         self,
-        value: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]],
+        value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__ea253ea2de3b46b0c52b024882e98593a0f3db8d76aad1bdef1c6a287691d8d2)
+            type_hints = typing.get_type_hints(getattr(RosDesktops, "volume_encryption_key").fset)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "volumeEncryptionKey", value)
 
     @builtins.property
     @jsii.member(jsii_name="vpcId")
     def vpc_id(
         self,
-    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+    ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: vpcId: This parameter is not open for use.
         '''
-        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], jsii.get(self, "vpcId"))
+        return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "vpcId"))
 
     @vpc_id.setter
     def vpc_id(
         self,
-        value: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]],
+        value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__5918b28308ae69a157e646d5f2548396236583e56234b899cd34e36fd21b1135)
+            type_hints = typing.get_type_hints(getattr(RosDesktops, "vpc_id").fset)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vpcId", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-ecd.RosDesktops.TagsProperty",
         jsii_struct_bases=[],
         name_mapping={"key": "key", "value": "value"},
     )
     class TagsProperty:
         def __init__(
             self,
             *,
-            key: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
-            value: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+            key: typing.Union[builtins.str, ros_cdk_core.IResolvable],
+            value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param key: 
             :param value: 
             '''
             if __debug__:
-                type_hints = typing.get_type_hints(_typecheckingstub__48fd99c9a5d8546f63f43773ca78e43bd2cc5755d095e4d38619a14d3db9b8f1)
+                type_hints = typing.get_type_hints(RosDesktops.TagsProperty.__init__)
                 check_type(argname="argument key", value=key, expected_type=type_hints["key"])
                 check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-            self._values: typing.Dict[builtins.str, typing.Any] = {
+            self._values: typing.Dict[str, typing.Any] = {
                 "key": key,
             }
             if value is not None:
                 self._values["value"] = value
 
         @builtins.property
-        def key(self) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+        def key(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
             '''
             :Property: key: The keyword of the tag.
             '''
             result = self._values.get("key")
             assert result is not None, "Required property 'key' is missing"
-            return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], result)
+            return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], result)
 
         @builtins.property
         def value(
             self,
-        ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+        ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
             '''
             :Property: value: The value of the tag.
             '''
             result = self._values.get("value")
-            return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], result)
+            return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], result)
 
         def __eq__(self, rhs: typing.Any) -> builtins.bool:
             return isinstance(rhs, self.__class__) and rhs._values == self._values
 
         def __ne__(self, rhs: typing.Any) -> builtins.bool:
             return not (rhs == self)
 
@@ -1185,36 +1173,36 @@
         "vpc_id": "vpcId",
     },
 )
 class RosDesktopsProps:
     def __init__(
         self,
         *,
-        bundle_id: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
-        office_site_id: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
-        policy_group_id: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
-        amount: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-        auto_pay: typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-        auto_renew: typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-        charge_type: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-        desktop_name: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-        desktop_name_suffix: typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-        directory_id: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-        end_user_id: typing.Optional[typing.Union[typing.Sequence[typing.Any], _ros_cdk_core_7adfd82f.IResolvable]] = None,
-        group_id: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-        hostname: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-        period: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-        period_unit: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-        promotion_id: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-        tags: typing.Optional[typing.Sequence[typing.Union[RosDesktops.TagsProperty, typing.Dict[builtins.str, typing.Any]]]] = None,
-        user_assign_mode: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-        user_name: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-        volume_encryption_enabled: typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-        volume_encryption_key: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-        vpc_id: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+        bundle_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
+        office_site_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
+        policy_group_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
+        amount: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
+        auto_pay: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
+        auto_renew: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
+        charge_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
+        desktop_name: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
+        desktop_name_suffix: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
+        directory_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
+        end_user_id: typing.Optional[typing.Union[typing.Sequence[typing.Any], ros_cdk_core.IResolvable]] = None,
+        group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
+        hostname: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
+        period: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
+        period_unit: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
+        promotion_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union[RosDesktops.TagsProperty, typing.Dict[str, typing.Any]]]] = None,
+        user_assign_mode: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
+        user_name: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
+        volume_encryption_enabled: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
+        volume_encryption_key: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
+        vpc_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::ECD::Desktops``.
 
         :param bundle_id: 
         :param office_site_id: 
         :param policy_group_id: 
         :param amount: 
@@ -1234,15 +1222,15 @@
         :param user_assign_mode: 
         :param user_name: 
         :param volume_encryption_enabled: 
         :param volume_encryption_key: 
         :param vpc_id: 
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__ddb9eda05360ff5e245c21204f4b5593d4fe63b0f051e3b57ab14f3bed3fa3e9)
+            type_hints = typing.get_type_hints(RosDesktopsProps.__init__)
             check_type(argname="argument bundle_id", value=bundle_id, expected_type=type_hints["bundle_id"])
             check_type(argname="argument office_site_id", value=office_site_id, expected_type=type_hints["office_site_id"])
             check_type(argname="argument policy_group_id", value=policy_group_id, expected_type=type_hints["policy_group_id"])
             check_type(argname="argument amount", value=amount, expected_type=type_hints["amount"])
             check_type(argname="argument auto_pay", value=auto_pay, expected_type=type_hints["auto_pay"])
             check_type(argname="argument auto_renew", value=auto_renew, expected_type=type_hints["auto_renew"])
             check_type(argname="argument charge_type", value=charge_type, expected_type=type_hints["charge_type"])
@@ -1257,15 +1245,15 @@
             check_type(argname="argument promotion_id", value=promotion_id, expected_type=type_hints["promotion_id"])
             check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
             check_type(argname="argument user_assign_mode", value=user_assign_mode, expected_type=type_hints["user_assign_mode"])
             check_type(argname="argument user_name", value=user_name, expected_type=type_hints["user_name"])
             check_type(argname="argument volume_encryption_enabled", value=volume_encryption_enabled, expected_type=type_hints["volume_encryption_enabled"])
             check_type(argname="argument volume_encryption_key", value=volume_encryption_key, expected_type=type_hints["volume_encryption_key"])
             check_type(argname="argument vpc_id", value=vpc_id, expected_type=type_hints["vpc_id"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "bundle_id": bundle_id,
             "office_site_id": office_site_id,
             "policy_group_id": policy_group_id,
         }
         if amount is not None:
             self._values["amount"] = amount
         if auto_pay is not None:
@@ -1302,178 +1290,172 @@
             self._values["volume_encryption_enabled"] = volume_encryption_enabled
         if volume_encryption_key is not None:
             self._values["volume_encryption_key"] = volume_encryption_key
         if vpc_id is not None:
             self._values["vpc_id"] = vpc_id
 
     @builtins.property
-    def bundle_id(
-        self,
-    ) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+    def bundle_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: bundleId: The ID of the cloud desktop template.
         '''
         result = self._values.get("bundle_id")
         assert result is not None, "Required property 'bundle_id' is missing"
-        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], result)
+        return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], result)
 
     @builtins.property
-    def office_site_id(
-        self,
-    ) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+    def office_site_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: officeSiteId: The ID of the workspace.
         '''
         result = self._values.get("office_site_id")
         assert result is not None, "Required property 'office_site_id' is missing"
-        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], result)
+        return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], result)
 
     @builtins.property
-    def policy_group_id(
-        self,
-    ) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+    def policy_group_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: policyGroupId: The ID of the policy.
         '''
         result = self._values.get("policy_group_id")
         assert result is not None, "Required property 'policy_group_id' is missing"
-        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], result)
+        return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], result)
 
     @builtins.property
     def amount(
         self,
-    ) -> typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]]:
+    ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
         amount: The number of cloud desktops that you want to create. Valid values: 1 to 300. Default
         value: 1.
         '''
         result = self._values.get("amount")
-        return typing.cast(typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]], result)
+        return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], result)
 
     @builtins.property
     def auto_pay(
         self,
-    ) -> typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]]:
+    ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
         autoPay: Specifies whether to enable automatic payment. Valid values:
         true: enables automatic payment. You must make sure that your Alibaba Cloud account
         has sufficient balance. If your Alibaba Cloud account does not have sufficient balance,
         abnormal orders are generated.
         false: disables automatic payment. In this case, an order is generated, and no payment
         is automatically made. You can log on to the EDS console and complete the payment
         based on the order ID on the Orders page.
         Default value: true.
         '''
         result = self._values.get("auto_pay")
-        return typing.cast(typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]], result)
+        return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], result)
 
     @builtins.property
     def auto_renew(
         self,
-    ) -> typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]]:
+    ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
         autoRenew: Specifies whether to enable auto-renewal for the cloud desktop. This parameter takes
         effect only when the ChargeType parameter is set to PrePaid.
         Valid values:
         true: enables auto-renewal. The renewal duration is the same as the subscription duration
         that you specified for the Period parameter when you purchased the cloud desktop.
         false: does not enable auto-renewal.
         Default value: false.
         '''
         result = self._values.get("auto_renew")
-        return typing.cast(typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]], result)
+        return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], result)
 
     @builtins.property
     def charge_type(
         self,
-    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+    ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
         chargeType: The billing method of the cloud desktop. Valid values:
         PostPaid: pay-as-you-go
         PrePaid: subscription
         Default value: PostPaid.
         '''
         result = self._values.get("charge_type")
-        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], result)
+        return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], result)
 
     @builtins.property
     def desktop_name(
         self,
-    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+    ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: desktopName: The name of the cloud desktop.
         '''
         result = self._values.get("desktop_name")
-        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], result)
+        return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], result)
 
     @builtins.property
     def desktop_name_suffix(
         self,
-    ) -> typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]]:
+    ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
         desktopNameSuffix: Specifies whether to automatically add a suffix to the cloud desktop name when you
         create multiple cloud desktops at a time.
         True: automatically adds a suffix.
         False: does not add a suffix.
         '''
         result = self._values.get("desktop_name_suffix")
-        return typing.cast(typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]], result)
+        return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], result)
 
     @builtins.property
     def directory_id(
         self,
-    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+    ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: directoryId: This parameter is not open for use.
         '''
         result = self._values.get("directory_id")
-        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], result)
+        return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], result)
 
     @builtins.property
     def end_user_id(
         self,
-    ) -> typing.Optional[typing.Union[typing.List[typing.Any], _ros_cdk_core_7adfd82f.IResolvable]]:
+    ) -> typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
         endUserId: The user ID that authorizes the use of the cloud desktop, 1~100 can be set.
         During the same period, only one user can use the desktop.
         If EndUserId is not set, the created cloud desktop will not be assigned to any user.
         '''
         result = self._values.get("end_user_id")
-        return typing.cast(typing.Optional[typing.Union[typing.List[typing.Any], _ros_cdk_core_7adfd82f.IResolvable]], result)
+        return typing.cast(typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]], result)
 
     @builtins.property
     def group_id(
         self,
-    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+    ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
         groupId: desktop group ID。
         Note that the desktop group function is currently in the invitation test.
         If you want to experience it, please submit a work order application.
         '''
         result = self._values.get("group_id")
-        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], result)
+        return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], result)
 
     @builtins.property
     def hostname(
         self,
-    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+    ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
         hostname: The custom hostname that you specify for the cloud desktop. You can only specify the
         hostname of a Windows cloud desktop in the workspace of the enterprise AD account
         type.
         The hostname must meet the following requirements:
@@ -1486,54 +1468,54 @@
         name_prefix: the prefix of the hostname.
         [begin_number,bits]: the ordered numbers in the hostname. begin_number: the start number. Valid values:
         0 to 999999. Default value: 0. bits: the digit. Valid values: 1 to 6. Default value:
         6.
         name_suffix: the suffix of the hostname.
         '''
         result = self._values.get("hostname")
-        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], result)
+        return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], result)
 
     @builtins.property
     def period(
         self,
-    ) -> typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]]:
+    ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
         period: The subscription duration. The unit of the value is specified by the PeriodUnit parameter. This parameter takes effect and is required only when the ChargeType parameter is set to PrePaid.
         If PeriodUnit is month, the valid range is 1, 2, 3, 6, 12, 24, 36, 48,60
         If periodUnit is year, the valid range is 1 to 5
         '''
         result = self._values.get("period")
-        return typing.cast(typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]], result)
+        return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], result)
 
     @builtins.property
     def period_unit(
         self,
-    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+    ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
         periodUnit: The unit of the subscription duration. Valid values:
         Month
         Year
         Default value: Month.
         '''
         result = self._values.get("period_unit")
-        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], result)
+        return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], result)
 
     @builtins.property
     def promotion_id(
         self,
-    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+    ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: promotionId: promotion id.
         '''
         result = self._values.get("promotion_id")
-        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], result)
+        return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], result)
 
     @builtins.property
     def tags(self) -> typing.Optional[typing.List[RosDesktops.TagsProperty]]:
         '''
         :Property:
 
         tags: The list of desktops tags in the form of key/value pairs.
@@ -1541,70 +1523,70 @@
         '''
         result = self._values.get("tags")
         return typing.cast(typing.Optional[typing.List[RosDesktops.TagsProperty]], result)
 
     @builtins.property
     def user_assign_mode(
         self,
-    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+    ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
         userAssignMode: The assignment mode of the cloud desktop. Default value: ALL.
         ALL: If you specify the EndUserId parameter, the cloud desktops that you create are
         assigned to each regular user that you specify.
         PER_USER: If you specify the EndUserId parameter, the cloud desktops that you create
         are evenly assigned to all regular users that you specify. In this case, you must
         make sure that the value of the Amount parameter can be divided by the N value of
         the EndUserId.N parameter that you specify.
         Note If you do not specify the EndUserId parameter, the cloud desktop that you create is
         not assigned to regular users.
         '''
         result = self._values.get("user_assign_mode")
-        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], result)
+        return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], result)
 
     @builtins.property
     def user_name(
         self,
-    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+    ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: userName: This parameter is not open for use.
         '''
         result = self._values.get("user_name")
-        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], result)
+        return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], result)
 
     @builtins.property
     def volume_encryption_enabled(
         self,
-    ) -> typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]]:
+    ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: volumeEncryptionEnabled: Whether to enable disk encryption.
         '''
         result = self._values.get("volume_encryption_enabled")
-        return typing.cast(typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]], result)
+        return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], result)
 
     @builtins.property
     def volume_encryption_key(
         self,
-    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+    ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: volumeEncryptionKey: The key ID of the KMS used when disk encryption is enabled. It can be obtained through the ListKeys interface.
         '''
         result = self._values.get("volume_encryption_key")
-        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], result)
+        return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], result)
 
     @builtins.property
     def vpc_id(
         self,
-    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+    ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: vpcId: This parameter is not open for use.
         '''
         result = self._values.get("vpc_id")
-        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], result)
+        return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
@@ -1618,233 +1600,7 @@
     "Desktops",
     "DesktopsProps",
     "RosDesktops",
     "RosDesktopsProps",
 ]
 
 publication.publish()
-
-def _typecheckingstub__ec37c66f272ac3085a407b8d35ffcaba92b80787d8d0d51b5c7359202f24a177(
-    scope: _ros_cdk_core_7adfd82f.Construct,
-    id: builtins.str,
-    props: typing.Union[DesktopsProps, typing.Dict[builtins.str, typing.Any]],
-    enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__5332608fe20f2b15df3518e820c058e964555fd1f537a8c2ee1a652ea3eccf1f(
-    *,
-    bundle_id: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
-    office_site_id: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
-    policy_group_id: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
-    amount: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-    auto_pay: typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-    auto_renew: typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-    charge_type: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-    desktop_name: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-    desktop_name_suffix: typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-    directory_id: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-    end_user_id: typing.Optional[typing.Union[typing.Sequence[typing.Any], _ros_cdk_core_7adfd82f.IResolvable]] = None,
-    group_id: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-    hostname: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-    period: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-    period_unit: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-    promotion_id: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-    tags: typing.Optional[typing.Sequence[typing.Union[RosDesktops.TagsProperty, typing.Dict[builtins.str, typing.Any]]]] = None,
-    user_assign_mode: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-    user_name: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-    volume_encryption_enabled: typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-    volume_encryption_key: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-    vpc_id: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__417ba7a4919468974fae3406c865d7692c3a1a949d5b355c09b558638caceafa(
-    scope: _ros_cdk_core_7adfd82f.Construct,
-    id: builtins.str,
-    props: typing.Union[RosDesktopsProps, typing.Dict[builtins.str, typing.Any]],
-    enable_resource_property_constraint: builtins.bool,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__b624a05db13321856dd462567d9a3ad708c91bb6c198de57d60f45c71a4870a7(
-    props: typing.Mapping[builtins.str, typing.Any],
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__048b5d93ea8fc94711fe40ab7cf22c025c4ee6ff7683ef25515076bbb2be14bb(
-    value: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__53c97614d89ca8bff4b5f500d1195b274c82ced15a9c6526f7bb7501a8b284ff(
-    value: builtins.bool,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__813dc4087bed123200c90e6001e5b59681e81e158701e1f799745da3bf0b494a(
-    value: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__6dcfd566820091b1c87bdee82e9d2372f9bd9c71f5f368af8c3082894cd2c6ca(
-    value: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__a676556ac09d4910dab532df18cdebcc18e642ba62cc02850c6fae39a3f2ae5e(
-    value: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]],
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__7bc2c01e82d9da5faf2c641d27e431bb87309d64cae517485ebc64f7f2058746(
-    value: typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]],
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__a01a9833dcc516e65e558219e84f6025560a064385c6b0682c09ec036609a73f(
-    value: typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]],
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__620ea32e2bebfb20528329b3ae5831f322597d95dd5795fc6ce5bee4e33fbec1(
-    value: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]],
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__ba1aef65181db1a0051b7cc3e0f5210af5f1dbd8fa8c013e17672a3e3097bfb8(
-    value: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]],
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__cb9b2fc5b5c218d0643028d9afe2982405bb6181e5f40c3fac2ab6ef84a213c3(
-    value: typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]],
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__299e31b65fffb8bf0e3c2a70ffef743e730d8ee5a59d2a19eb5338e5074f6af1(
-    value: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]],
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__5d4b497cb011a6133f7608707bb91cac249a69db83f38626801318f3f6e9392e(
-    value: typing.Optional[typing.Union[typing.List[typing.Any], _ros_cdk_core_7adfd82f.IResolvable]],
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__c8b32d925398e6519b7f4d80de38a1bf3f7de314b43ee6ba21765eb8ae7a1dbc(
-    value: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]],
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__86cc34c87e1c2d81e79d6309023c565598f2d9c44110b32f00b9d82daf639295(
-    value: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]],
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__d6bd5b5fa770c89aa3aa5866d160c1a2a08ba6b88c074843c007d66a8a937f27(
-    value: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]],
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__fdef60d1614d2f3601a4bd4bd6a28252405455eace4fce908fdd14f9197fc70c(
-    value: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]],
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__efbba2fa69ae3743174c96210025457253685466a96aa6f91227befb135ab991(
-    value: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]],
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__0fc2002b918d8a09ef269bd8d5b1d1168a20bed25d8494172f6e04a152020f7c(
-    value: typing.Optional[typing.List[RosDesktops.TagsProperty]],
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__b55294dbcbbf93862814b175eed541beb9ed8c6f90030c0bff94c21b4e032dcb(
-    value: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]],
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__441b1f7f1911342bb501926092bcdd57fbd727f261eb2e95b2cb2b03000004d0(
-    value: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]],
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__0a1a5e8e1790c293746b5cbcd705b50d46a2e3226ad2e9bb108b7dea7e08ce38(
-    value: typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]],
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__ea253ea2de3b46b0c52b024882e98593a0f3db8d76aad1bdef1c6a287691d8d2(
-    value: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]],
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__5918b28308ae69a157e646d5f2548396236583e56234b899cd34e36fd21b1135(
-    value: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]],
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__48fd99c9a5d8546f63f43773ca78e43bd2cc5755d095e4d38619a14d3db9b8f1(
-    *,
-    key: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
-    value: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__ddb9eda05360ff5e245c21204f4b5593d4fe63b0f051e3b57ab14f3bed3fa3e9(
-    *,
-    bundle_id: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
-    office_site_id: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
-    policy_group_id: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
-    amount: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-    auto_pay: typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-    auto_renew: typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-    charge_type: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-    desktop_name: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-    desktop_name_suffix: typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-    directory_id: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-    end_user_id: typing.Optional[typing.Union[typing.Sequence[typing.Any], _ros_cdk_core_7adfd82f.IResolvable]] = None,
-    group_id: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-    hostname: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-    period: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-    period_unit: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-    promotion_id: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-    tags: typing.Optional[typing.Sequence[typing.Union[RosDesktops.TagsProperty, typing.Dict[builtins.str, typing.Any]]]] = None,
-    user_assign_mode: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-    user_name: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-    volume_encryption_enabled: typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-    volume_encryption_key: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-    vpc_id: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
```

### Comparing `ros-cdk-ecd-1.0.13/src/ros_cdk_ecd.egg-info/PKG-INFO` & `ros-cdk-ecd-1.0.9/src/ros_cdk_ecd.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-ecd
-Version: 1.0.13
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS ECD Construct Library
         
@@ -19,13 +19,12 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
```

