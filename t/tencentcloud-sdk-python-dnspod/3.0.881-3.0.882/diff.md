# Comparing `tmp/tencentcloud-sdk-python-dnspod-3.0.881.tar.gz` & `tmp/tencentcloud-sdk-python-dnspod-3.0.882.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-dnspod-3.0.881.tar", last modified: Tue Apr 25 00:35:51 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-dnspod-3.0.882.tar", last modified: Wed Apr 26 03:18:05 2023, max compression
```

## Comparing `tencentcloud-sdk-python-dnspod-3.0.881.tar` & `tencentcloud-sdk-python-dnspod-3.0.882.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:35:51.000000 tencentcloud-sdk-python-dnspod-3.0.881/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:35:51.000000 tencentcloud-sdk-python-dnspod-3.0.881/tencentcloud_sdk_python_dnspod.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 00:35:51.000000 tencentcloud-sdk-python-dnspod-3.0.881/tencentcloud_sdk_python_dnspod.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      475 2023-04-25 00:35:51.000000 tencentcloud-sdk-python-dnspod-3.0.881/tencentcloud_sdk_python_dnspod.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-04-25 00:35:51.000000 tencentcloud-sdk-python-dnspod-3.0.881/tencentcloud_sdk_python_dnspod.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-25 00:35:51.000000 tencentcloud-sdk-python-dnspod-3.0.881/tencentcloud_sdk_python_dnspod.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      746 2023-04-25 00:35:51.000000 tencentcloud-sdk-python-dnspod-3.0.881/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:35:51.000000 tencentcloud-sdk-python-dnspod-3.0.881/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:35:51.000000 tencentcloud-sdk-python-dnspod-3.0.881/tencentcloud/dnspod/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:35:51.000000 tencentcloud-sdk-python-dnspod-3.0.881/tencentcloud/dnspod/v20210323/
--rw-r--r--   0 root         (0) root         (0)    23568 2023-04-25 00:35:51.000000 tencentcloud-sdk-python-dnspod-3.0.881/tencentcloud/dnspod/v20210323/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 00:35:51.000000 tencentcloud-sdk-python-dnspod-3.0.881/tencentcloud/dnspod/v20210323/__init__.py
--rw-r--r--   0 root         (0) root         (0)   201880 2023-04-25 00:35:51.000000 tencentcloud-sdk-python-dnspod-3.0.881/tencentcloud/dnspod/v20210323/models.py
--rw-r--r--   0 root         (0) root         (0)    58917 2023-04-25 00:35:51.000000 tencentcloud-sdk-python-dnspod-3.0.881/tencentcloud/dnspod/v20210323/dnspod_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 00:35:51.000000 tencentcloud-sdk-python-dnspod-3.0.881/tencentcloud/dnspod/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-25 00:35:51.000000 tencentcloud-sdk-python-dnspod-3.0.881/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1674 2023-04-25 00:35:51.000000 tencentcloud-sdk-python-dnspod-3.0.881/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1012 2023-04-25 00:35:51.000000 tencentcloud-sdk-python-dnspod-3.0.881/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-25 00:35:51.000000 tencentcloud-sdk-python-dnspod-3.0.881/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:18:05.000000 tencentcloud-sdk-python-dnspod-3.0.882/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:18:05.000000 tencentcloud-sdk-python-dnspod-3.0.882/tencentcloud_sdk_python_dnspod.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 03:18:05.000000 tencentcloud-sdk-python-dnspod-3.0.882/tencentcloud_sdk_python_dnspod.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      475 2023-04-26 03:18:05.000000 tencentcloud-sdk-python-dnspod-3.0.882/tencentcloud_sdk_python_dnspod.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-04-26 03:18:05.000000 tencentcloud-sdk-python-dnspod-3.0.882/tencentcloud_sdk_python_dnspod.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-26 03:18:05.000000 tencentcloud-sdk-python-dnspod-3.0.882/tencentcloud_sdk_python_dnspod.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      746 2023-04-26 03:18:04.000000 tencentcloud-sdk-python-dnspod-3.0.882/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:18:05.000000 tencentcloud-sdk-python-dnspod-3.0.882/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:18:05.000000 tencentcloud-sdk-python-dnspod-3.0.882/tencentcloud/dnspod/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:18:05.000000 tencentcloud-sdk-python-dnspod-3.0.882/tencentcloud/dnspod/v20210323/
+-rw-r--r--   0 root         (0) root         (0)    23568 2023-04-26 03:18:04.000000 tencentcloud-sdk-python-dnspod-3.0.882/tencentcloud/dnspod/v20210323/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 03:18:04.000000 tencentcloud-sdk-python-dnspod-3.0.882/tencentcloud/dnspod/v20210323/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   202833 2023-04-26 03:18:04.000000 tencentcloud-sdk-python-dnspod-3.0.882/tencentcloud/dnspod/v20210323/models.py
+-rw-r--r--   0 root         (0) root         (0)    58917 2023-04-26 03:18:04.000000 tencentcloud-sdk-python-dnspod-3.0.882/tencentcloud/dnspod/v20210323/dnspod_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 03:18:04.000000 tencentcloud-sdk-python-dnspod-3.0.882/tencentcloud/dnspod/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-26 03:18:04.000000 tencentcloud-sdk-python-dnspod-3.0.882/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-04-26 03:18:05.000000 tencentcloud-sdk-python-dnspod-3.0.882/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-04-26 03:18:04.000000 tencentcloud-sdk-python-dnspod-3.0.882/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-26 03:18:05.000000 tencentcloud-sdk-python-dnspod-3.0.882/setup.cfg
```

### Comparing `tencentcloud-sdk-python-dnspod-3.0.881/tencentcloud_sdk_python_dnspod.egg-info/PKG-INFO` & `tencentcloud-sdk-python-dnspod-3.0.882/tencentcloud_sdk_python_dnspod.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dnspod
-Version: 3.0.881
+Version: 3.0.882
 Summary: Tencent Cloud Dnspod SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dnspod-3.0.881/README.rst` & `tencentcloud-sdk-python-dnspod-3.0.882/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dnspod-3.0.881/tencentcloud/dnspod/v20210323/errorcodes.py` & `tencentcloud-sdk-python-dnspod-3.0.882/tencentcloud/dnspod/v20210323/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dnspod-3.0.881/tencentcloud/dnspod/v20210323/models.py` & `tencentcloud-sdk-python-dnspod-3.0.882/tencentcloud/dnspod/v20210323/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -3243,22 +3243,26 @@
 
     def __init__(self):
         r"""
         :param Id: 域名别名ID
         :type Id: int
         :param DomainAlias: 域名别名
         :type DomainAlias: str
+        :param Status: 别名状态：1-DNS不正确；2-正常；3-封禁。
+        :type Status: int
         """
         self.Id = None
         self.DomainAlias = None
+        self.Status = None
 
 
     def _deserialize(self, params):
         self.Id = params.get("Id")
         self.DomainAlias = params.get("DomainAlias")
+        self.Status = params.get("Status")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -5447,24 +5451,33 @@
         r"""
         :param Domain: 域名
         :type Domain: str
         :param SnapshotId: 快照记录 ID
         :type SnapshotId: str
         :param DomainId: 域名 ID 。参数 DomainId 优先级比参数 Domain 高，如果传递参数 DomainId 将忽略参数 Domain 。
         :type DomainId: int
+        :param RecordList: 指定需要回滚的记录
+        :type RecordList: list of SnapshotRecord
         """
         self.Domain = None
         self.SnapshotId = None
         self.DomainId = None
+        self.RecordList = None
 
 
     def _deserialize(self, params):
         self.Domain = params.get("Domain")
         self.SnapshotId = params.get("SnapshotId")
         self.DomainId = params.get("DomainId")
+        if params.get("RecordList") is not None:
+            self.RecordList = []
+            for item in params.get("RecordList"):
+                obj = SnapshotRecord()
+                obj._deserialize(item)
+                self.RecordList.append(obj)
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -5625,32 +5638,42 @@
         :param TTL: TTL(秒)
         :type TTL: str
         :param RecordId: 解析记录 ID
         :type RecordId: str
         :param MX: MX优先级
 注意：此字段可能返回 null，表示取不到有效值。
         :type MX: str
+        :param Weight: 权重
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Weight: str
+        :param Reason: 失败原因
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Reason: str
         """
         self.SubDomain = None
         self.RecordType = None
         self.RecordLine = None
         self.Value = None
         self.TTL = None
         self.RecordId = None
         self.MX = None
+        self.Weight = None
+        self.Reason = None
 
 
     def _deserialize(self, params):
         self.SubDomain = params.get("SubDomain")
         self.RecordType = params.get("RecordType")
         self.RecordLine = params.get("RecordLine")
         self.Value = params.get("Value")
         self.TTL = params.get("TTL")
         self.RecordId = params.get("RecordId")
         self.MX = params.get("MX")
+        self.Weight = params.get("Weight")
+        self.Reason = params.get("Reason")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-dnspod-3.0.881/tencentcloud/dnspod/v20210323/dnspod_client.py` & `tencentcloud-sdk-python-dnspod-3.0.882/tencentcloud/dnspod/v20210323/dnspod_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dnspod-3.0.881/tencentcloud/__init__.py` & `tencentcloud-sdk-python-dnspod-3.0.882/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-dnspod-3.0.881/PKG-INFO` & `tencentcloud-sdk-python-dnspod-3.0.882/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dnspod
-Version: 3.0.881
+Version: 3.0.882
 Summary: Tencent Cloud Dnspod SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dnspod-3.0.881/setup.py` & `tencentcloud-sdk-python-dnspod-3.0.882/setup.py`

 * *Files identical despite different names*

