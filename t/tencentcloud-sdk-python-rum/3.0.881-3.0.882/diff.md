# Comparing `tmp/tencentcloud-sdk-python-rum-3.0.881.tar.gz` & `tmp/tencentcloud-sdk-python-rum-3.0.882.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-rum-3.0.881.tar", last modified: Tue Apr 25 00:50:15 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-rum-3.0.882.tar", last modified: Wed Apr 26 03:44:22 2023, max compression
```

## Comparing `tencentcloud-sdk-python-rum-3.0.881.tar` & `tencentcloud-sdk-python-rum-3.0.882.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:50:15.000000 tencentcloud-sdk-python-rum-3.0.881/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-25 00:50:14.000000 tencentcloud-sdk-python-rum-3.0.881/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:50:15.000000 tencentcloud-sdk-python-rum-3.0.881/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:50:15.000000 tencentcloud-sdk-python-rum-3.0.881/tencentcloud/rum/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:50:15.000000 tencentcloud-sdk-python-rum-3.0.881/tencentcloud/rum/v20210622/
--rw-r--r--   0 root         (0) root         (0)    59777 2023-04-25 00:50:14.000000 tencentcloud-sdk-python-rum-3.0.881/tencentcloud/rum/v20210622/rum_client.py
--rw-r--r--   0 root         (0) root         (0)     2530 2023-04-25 00:50:14.000000 tencentcloud-sdk-python-rum-3.0.881/tencentcloud/rum/v20210622/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 00:50:14.000000 tencentcloud-sdk-python-rum-3.0.881/tencentcloud/rum/v20210622/__init__.py
--rw-r--r--   0 root         (0) root         (0)   171124 2023-04-25 00:50:14.000000 tencentcloud-sdk-python-rum-3.0.881/tencentcloud/rum/v20210622/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 00:50:14.000000 tencentcloud-sdk-python-rum-3.0.881/tencentcloud/rum/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-25 00:50:14.000000 tencentcloud-sdk-python-rum-3.0.881/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-25 00:50:15.000000 tencentcloud-sdk-python-rum-3.0.881/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:50:15.000000 tencentcloud-sdk-python-rum-3.0.881/tencentcloud_sdk_python_rum.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 00:50:15.000000 tencentcloud-sdk-python-rum-3.0.881/tencentcloud_sdk_python_rum.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-25 00:50:15.000000 tencentcloud-sdk-python-rum-3.0.881/tencentcloud_sdk_python_rum.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-25 00:50:15.000000 tencentcloud-sdk-python-rum-3.0.881/tencentcloud_sdk_python_rum.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-25 00:50:15.000000 tencentcloud-sdk-python-rum-3.0.881/tencentcloud_sdk_python_rum.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-25 00:50:14.000000 tencentcloud-sdk-python-rum-3.0.881/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-25 00:50:15.000000 tencentcloud-sdk-python-rum-3.0.881/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:44:22.000000 tencentcloud-sdk-python-rum-3.0.882/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-26 03:44:21.000000 tencentcloud-sdk-python-rum-3.0.882/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:44:22.000000 tencentcloud-sdk-python-rum-3.0.882/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:44:22.000000 tencentcloud-sdk-python-rum-3.0.882/tencentcloud/rum/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:44:22.000000 tencentcloud-sdk-python-rum-3.0.882/tencentcloud/rum/v20210622/
+-rw-r--r--   0 root         (0) root         (0)    59777 2023-04-26 03:44:21.000000 tencentcloud-sdk-python-rum-3.0.882/tencentcloud/rum/v20210622/rum_client.py
+-rw-r--r--   0 root         (0) root         (0)     2530 2023-04-26 03:44:21.000000 tencentcloud-sdk-python-rum-3.0.882/tencentcloud/rum/v20210622/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 03:44:21.000000 tencentcloud-sdk-python-rum-3.0.882/tencentcloud/rum/v20210622/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   171586 2023-04-26 03:44:21.000000 tencentcloud-sdk-python-rum-3.0.882/tencentcloud/rum/v20210622/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 03:44:21.000000 tencentcloud-sdk-python-rum-3.0.882/tencentcloud/rum/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-26 03:44:21.000000 tencentcloud-sdk-python-rum-3.0.882/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-26 03:44:22.000000 tencentcloud-sdk-python-rum-3.0.882/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:44:22.000000 tencentcloud-sdk-python-rum-3.0.882/tencentcloud_sdk_python_rum.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 03:44:22.000000 tencentcloud-sdk-python-rum-3.0.882/tencentcloud_sdk_python_rum.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-26 03:44:22.000000 tencentcloud-sdk-python-rum-3.0.882/tencentcloud_sdk_python_rum.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-26 03:44:22.000000 tencentcloud-sdk-python-rum-3.0.882/tencentcloud_sdk_python_rum.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-26 03:44:22.000000 tencentcloud-sdk-python-rum-3.0.882/tencentcloud_sdk_python_rum.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-26 03:44:21.000000 tencentcloud-sdk-python-rum-3.0.882/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-26 03:44:22.000000 tencentcloud-sdk-python-rum-3.0.882/setup.cfg
```

### Comparing `tencentcloud-sdk-python-rum-3.0.881/README.rst` & `tencentcloud-sdk-python-rum-3.0.882/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-rum-3.0.881/tencentcloud/rum/v20210622/rum_client.py` & `tencentcloud-sdk-python-rum-3.0.882/tencentcloud/rum/v20210622/rum_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-rum-3.0.881/tencentcloud/rum/v20210622/errorcodes.py` & `tencentcloud-sdk-python-rum-3.0.882/tencentcloud/rum/v20210622/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-rum-3.0.881/tencentcloud/rum/v20210622/models.py` & `tencentcloud-sdk-python-rum-3.0.882/tencentcloud/rum/v20210622/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -341,26 +341,29 @@
         :type PeriodRetain: str
         :param BuyingChannel: 实例购买渠道("cdn" 等)
         :type BuyingChannel: str
         :param ResourcePackageType: 预付费资源包类型(仅预付费需要)
         :type ResourcePackageType: int
         :param ResourcePackageNum: 预付费资源包数量(仅预付费需要)
         :type ResourcePackageNum: int
+        :param InstanceType: 实例类型 1:原web相关类型 2:app端类型
+        :type InstanceType: int
         """
         self.AreaId = None
         self.ChargeType = None
         self.DataRetentionDays = None
         self.InstanceName = None
         self.Tags = None
         self.InstanceDesc = None
         self.CountNum = None
         self.PeriodRetain = None
         self.BuyingChannel = None
         self.ResourcePackageType = None
         self.ResourcePackageNum = None
+        self.InstanceType = None
 
 
     def _deserialize(self, params):
         self.AreaId = params.get("AreaId")
         self.ChargeType = params.get("ChargeType")
         self.DataRetentionDays = params.get("DataRetentionDays")
         self.InstanceName = params.get("InstanceName")
@@ -372,14 +375,15 @@
                 self.Tags.append(obj)
         self.InstanceDesc = params.get("InstanceDesc")
         self.CountNum = params.get("CountNum")
         self.PeriodRetain = params.get("PeriodRetain")
         self.BuyingChannel = params.get("BuyingChannel")
         self.ResourcePackageType = params.get("ResourcePackageType")
         self.ResourcePackageNum = params.get("ResourcePackageNum")
+        self.InstanceType = params.get("InstanceType")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -5127,27 +5131,31 @@
         :type UpdatedAt: str
         :param DataRetentionDays: 数据保留时间(天)
         :type DataRetentionDays: int
         :param InstanceName: 实例名称
         :type InstanceName: str
         :param CreatedAt: 创建时间
         :type CreatedAt: str
+        :param InstanceType: 实例类型 1:原web相关类型 2:app端类型
+注意：此字段可能返回 null，表示取不到有效值。
+        :type InstanceType: int
         """
         self.InstanceStatus = None
         self.AreaId = None
         self.Tags = None
         self.InstanceId = None
         self.ClusterId = None
         self.InstanceDesc = None
         self.ChargeStatus = None
         self.ChargeType = None
         self.UpdatedAt = None
         self.DataRetentionDays = None
         self.InstanceName = None
         self.CreatedAt = None
+        self.InstanceType = None
 
 
     def _deserialize(self, params):
         self.InstanceStatus = params.get("InstanceStatus")
         self.AreaId = params.get("AreaId")
         if params.get("Tags") is not None:
             self.Tags = []
@@ -5160,14 +5168,15 @@
         self.InstanceDesc = params.get("InstanceDesc")
         self.ChargeStatus = params.get("ChargeStatus")
         self.ChargeType = params.get("ChargeType")
         self.UpdatedAt = params.get("UpdatedAt")
         self.DataRetentionDays = params.get("DataRetentionDays")
         self.InstanceName = params.get("InstanceName")
         self.CreatedAt = params.get("CreatedAt")
+        self.InstanceType = params.get("InstanceType")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-rum-3.0.881/tencentcloud/__init__.py` & `tencentcloud-sdk-python-rum-3.0.882/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.881'
+__version__ = '3.0.882'
```

### Comparing `tencentcloud-sdk-python-rum-3.0.881/PKG-INFO` & `tencentcloud-sdk-python-rum-3.0.882/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-rum
-Version: 3.0.881
+Version: 3.0.882
 Summary: Tencent Cloud Rum SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-rum-3.0.881/tencentcloud_sdk_python_rum.egg-info/PKG-INFO` & `tencentcloud-sdk-python-rum-3.0.882/tencentcloud_sdk_python_rum.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-rum
-Version: 3.0.881
+Version: 3.0.882
 Summary: Tencent Cloud Rum SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-rum-3.0.881/setup.py` & `tencentcloud-sdk-python-rum-3.0.882/setup.py`

 * *Files identical despite different names*

