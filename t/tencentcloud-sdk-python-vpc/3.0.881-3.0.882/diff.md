# Comparing `tmp/tencentcloud-sdk-python-vpc-3.0.881.tar.gz` & `tmp/tencentcloud-sdk-python-vpc-3.0.882.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-vpc-3.0.881.tar", last modified: Tue Apr 25 01:00:59 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-vpc-3.0.882.tar", last modified: Wed Apr 26 03:59:54 2023, max compression
```

## Comparing `tencentcloud-sdk-python-vpc-3.0.881.tar` & `tencentcloud-sdk-python-vpc-3.0.882.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 01:00:59.000000 tencentcloud-sdk-python-vpc-3.0.881/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 01:00:59.000000 tencentcloud-sdk-python-vpc-3.0.881/tencentcloud_sdk_python_vpc.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 01:00:59.000000 tencentcloud-sdk-python-vpc-3.0.881/tencentcloud_sdk_python_vpc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-25 01:00:59.000000 tencentcloud-sdk-python-vpc-3.0.881/tencentcloud_sdk_python_vpc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-25 01:00:59.000000 tencentcloud-sdk-python-vpc-3.0.881/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-25 01:00:59.000000 tencentcloud-sdk-python-vpc-3.0.881/tencentcloud_sdk_python_vpc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-25 01:00:59.000000 tencentcloud-sdk-python-vpc-3.0.881/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 01:00:59.000000 tencentcloud-sdk-python-vpc-3.0.881/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 01:00:59.000000 tencentcloud-sdk-python-vpc-3.0.881/tencentcloud/vpc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 01:00:59.000000 tencentcloud-sdk-python-vpc-3.0.881/tencentcloud/vpc/v20170312/
--rw-r--r--   0 root         (0) root         (0)   327723 2023-04-25 01:00:59.000000 tencentcloud-sdk-python-vpc-3.0.881/tencentcloud/vpc/v20170312/vpc_client.py
--rw-r--r--   0 root         (0) root         (0)    40497 2023-04-25 01:00:59.000000 tencentcloud-sdk-python-vpc-3.0.881/tencentcloud/vpc/v20170312/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 01:00:59.000000 tencentcloud-sdk-python-vpc-3.0.881/tencentcloud/vpc/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)   836460 2023-04-25 01:00:59.000000 tencentcloud-sdk-python-vpc-3.0.881/tencentcloud/vpc/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 01:00:59.000000 tencentcloud-sdk-python-vpc-3.0.881/tencentcloud/vpc/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-25 01:00:59.000000 tencentcloud-sdk-python-vpc-3.0.881/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-25 01:00:59.000000 tencentcloud-sdk-python-vpc-3.0.881/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-25 01:00:59.000000 tencentcloud-sdk-python-vpc-3.0.881/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-25 01:00:59.000000 tencentcloud-sdk-python-vpc-3.0.881/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:59:54.000000 tencentcloud-sdk-python-vpc-3.0.882/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:59:54.000000 tencentcloud-sdk-python-vpc-3.0.882/tencentcloud_sdk_python_vpc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 03:59:54.000000 tencentcloud-sdk-python-vpc-3.0.882/tencentcloud_sdk_python_vpc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-26 03:59:54.000000 tencentcloud-sdk-python-vpc-3.0.882/tencentcloud_sdk_python_vpc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-26 03:59:54.000000 tencentcloud-sdk-python-vpc-3.0.882/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-26 03:59:54.000000 tencentcloud-sdk-python-vpc-3.0.882/tencentcloud_sdk_python_vpc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-26 03:59:54.000000 tencentcloud-sdk-python-vpc-3.0.882/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:59:54.000000 tencentcloud-sdk-python-vpc-3.0.882/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:59:54.000000 tencentcloud-sdk-python-vpc-3.0.882/tencentcloud/vpc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:59:54.000000 tencentcloud-sdk-python-vpc-3.0.882/tencentcloud/vpc/v20170312/
+-rw-r--r--   0 root         (0) root         (0)   328818 2023-04-26 03:59:54.000000 tencentcloud-sdk-python-vpc-3.0.882/tencentcloud/vpc/v20170312/vpc_client.py
+-rw-r--r--   0 root         (0) root         (0)    40497 2023-04-26 03:59:54.000000 tencentcloud-sdk-python-vpc-3.0.882/tencentcloud/vpc/v20170312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 03:59:54.000000 tencentcloud-sdk-python-vpc-3.0.882/tencentcloud/vpc/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   838070 2023-04-26 03:59:54.000000 tencentcloud-sdk-python-vpc-3.0.882/tencentcloud/vpc/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 03:59:54.000000 tencentcloud-sdk-python-vpc-3.0.882/tencentcloud/vpc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-26 03:59:54.000000 tencentcloud-sdk-python-vpc-3.0.882/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-26 03:59:54.000000 tencentcloud-sdk-python-vpc-3.0.882/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-26 03:59:54.000000 tencentcloud-sdk-python-vpc-3.0.882/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-26 03:59:54.000000 tencentcloud-sdk-python-vpc-3.0.882/setup.cfg
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.881/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-vpc-3.0.882/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vpc
-Version: 3.0.881
+Version: 3.0.882
 Summary: Tencent Cloud Vpc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.881/README.rst` & `tencentcloud-sdk-python-vpc-3.0.882/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vpc-3.0.881/tencentcloud/vpc/v20170312/vpc_client.py` & `tencentcloud-sdk-python-vpc-3.0.882/tencentcloud/vpc/v20170312/vpc_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -5123,14 +5123,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def GenerateVpnConnectionDefaultHealthCheckIp(self, request):
+        """本接口（GenerateVpnConnectionDefaultHealthCheckIp）用于获取一对VPN通道健康检查地址。
+
+        :param request: Request instance for GenerateVpnConnectionDefaultHealthCheckIp.
+        :type request: :class:`tencentcloud.vpc.v20170312.models.GenerateVpnConnectionDefaultHealthCheckIpRequest`
+        :rtype: :class:`tencentcloud.vpc.v20170312.models.GenerateVpnConnectionDefaultHealthCheckIpResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("GenerateVpnConnectionDefaultHealthCheckIp", params, headers=headers)
+            response = json.loads(body)
+            model = models.GenerateVpnConnectionDefaultHealthCheckIpResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def GetCcnRegionBandwidthLimits(self, request):
         """本接口（GetCcnRegionBandwidthLimits）用于查询云联网相关地域带宽信息，其中预付费模式的云联网仅支持地域间限速，后付费模式的云联网支持地域间限速和地域出口限速。
 
         :param request: Request instance for GetCcnRegionBandwidthLimits.
         :type request: :class:`tencentcloud.vpc.v20170312.models.GetCcnRegionBandwidthLimitsRequest`
         :rtype: :class:`tencentcloud.vpc.v20170312.models.GetCcnRegionBandwidthLimitsResponse`
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.881/tencentcloud/vpc/v20170312/errorcodes.py` & `tencentcloud-sdk-python-vpc-3.0.882/tencentcloud/vpc/v20170312/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vpc-3.0.881/tencentcloud/vpc/v20170312/models.py` & `tencentcloud-sdk-python-vpc-3.0.882/tencentcloud/vpc/v20170312/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -14999,14 +14999,63 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class GenerateVpnConnectionDefaultHealthCheckIpRequest(AbstractModel):
+    """GenerateVpnConnectionDefaultHealthCheckIp请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param VpnGatewayId: VPN网关id， 例如：vpngw-1w9tue3d
+        :type VpnGatewayId: str
+        """
+        self.VpnGatewayId = None
+
+
+    def _deserialize(self, params):
+        self.VpnGatewayId = params.get("VpnGatewayId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class GenerateVpnConnectionDefaultHealthCheckIpResponse(AbstractModel):
+    """GenerateVpnConnectionDefaultHealthCheckIp返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param HealthCheckLocalIp: VPN通道健康检查本端ip
+        :type HealthCheckLocalIp: str
+        :param HealthCheckRemoteIp: VPN通道健康检查对端ip
+        :type HealthCheckRemoteIp: str
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.HealthCheckLocalIp = None
+        self.HealthCheckRemoteIp = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.HealthCheckLocalIp = params.get("HealthCheckLocalIp")
+        self.HealthCheckRemoteIp = params.get("HealthCheckRemoteIp")
+        self.RequestId = params.get("RequestId")
+
+
 class GetCcnRegionBandwidthLimitsRequest(AbstractModel):
     """GetCcnRegionBandwidthLimits请求参数结构体
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.881/tencentcloud/__init__.py` & `tencentcloud-sdk-python-vpc-3.0.882/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-vpc-3.0.881/PKG-INFO` & `tencentcloud-sdk-python-vpc-3.0.882/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vpc
-Version: 3.0.881
+Version: 3.0.882
 Summary: Tencent Cloud Vpc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.881/setup.py` & `tencentcloud-sdk-python-vpc-3.0.882/setup.py`

 * *Files identical despite different names*

