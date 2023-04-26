# Comparing `tmp/tencentcloud-sdk-python-teo-3.0.881.tar.gz` & `tmp/tencentcloud-sdk-python-teo-3.0.882.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-teo-3.0.881.tar", last modified: Tue Apr 25 00:57:25 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-teo-3.0.882.tar", last modified: Wed Apr 26 03:51:22 2023, max compression
```

## Comparing `tencentcloud-sdk-python-teo-3.0.881.tar` & `tencentcloud-sdk-python-teo-3.0.882.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:57:25.000000 tencentcloud-sdk-python-teo-3.0.881/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-25 00:57:24.000000 tencentcloud-sdk-python-teo-3.0.881/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:57:25.000000 tencentcloud-sdk-python-teo-3.0.881/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:57:25.000000 tencentcloud-sdk-python-teo-3.0.881/tencentcloud/teo/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:57:25.000000 tencentcloud-sdk-python-teo-3.0.881/tencentcloud/teo/v20220106/
--rw-r--r--   0 root         (0) root         (0)     2192 2023-04-25 00:57:24.000000 tencentcloud-sdk-python-teo-3.0.881/tencentcloud/teo/v20220106/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 00:57:24.000000 tencentcloud-sdk-python-teo-3.0.881/tencentcloud/teo/v20220106/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24724 2023-04-25 00:57:24.000000 tencentcloud-sdk-python-teo-3.0.881/tencentcloud/teo/v20220106/models.py
--rw-r--r--   0 root         (0) root         (0)     5379 2023-04-25 00:57:24.000000 tencentcloud-sdk-python-teo-3.0.881/tencentcloud/teo/v20220106/teo_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 00:57:24.000000 tencentcloud-sdk-python-teo-3.0.881/tencentcloud/teo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:57:25.000000 tencentcloud-sdk-python-teo-3.0.881/tencentcloud/teo/v20220901/
--rw-r--r--   0 root         (0) root         (0)    21701 2023-04-25 00:57:24.000000 tencentcloud-sdk-python-teo-3.0.881/tencentcloud/teo/v20220901/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 00:57:24.000000 tencentcloud-sdk-python-teo-3.0.881/tencentcloud/teo/v20220901/__init__.py
--rw-r--r--   0 root         (0) root         (0)   504804 2023-04-25 00:57:24.000000 tencentcloud-sdk-python-teo-3.0.881/tencentcloud/teo/v20220901/models.py
--rw-r--r--   0 root         (0) root         (0)    81864 2023-04-25 00:57:24.000000 tencentcloud-sdk-python-teo-3.0.881/tencentcloud/teo/v20220901/teo_client.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-25 00:57:24.000000 tencentcloud-sdk-python-teo-3.0.881/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-25 00:57:25.000000 tencentcloud-sdk-python-teo-3.0.881/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:57:25.000000 tencentcloud-sdk-python-teo-3.0.881/tencentcloud_sdk_python_teo.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 00:57:25.000000 tencentcloud-sdk-python-teo-3.0.881/tencentcloud_sdk_python_teo.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      603 2023-04-25 00:57:25.000000 tencentcloud-sdk-python-teo-3.0.881/tencentcloud_sdk_python_teo.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-25 00:57:25.000000 tencentcloud-sdk-python-teo-3.0.881/tencentcloud_sdk_python_teo.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-25 00:57:25.000000 tencentcloud-sdk-python-teo-3.0.881/tencentcloud_sdk_python_teo.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-25 00:57:24.000000 tencentcloud-sdk-python-teo-3.0.881/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-25 00:57:25.000000 tencentcloud-sdk-python-teo-3.0.881/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:51:22.000000 tencentcloud-sdk-python-teo-3.0.882/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-26 03:51:22.000000 tencentcloud-sdk-python-teo-3.0.882/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:51:22.000000 tencentcloud-sdk-python-teo-3.0.882/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:51:22.000000 tencentcloud-sdk-python-teo-3.0.882/tencentcloud/teo/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:51:22.000000 tencentcloud-sdk-python-teo-3.0.882/tencentcloud/teo/v20220106/
+-rw-r--r--   0 root         (0) root         (0)     2192 2023-04-26 03:51:22.000000 tencentcloud-sdk-python-teo-3.0.882/tencentcloud/teo/v20220106/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 03:51:22.000000 tencentcloud-sdk-python-teo-3.0.882/tencentcloud/teo/v20220106/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24724 2023-04-26 03:51:22.000000 tencentcloud-sdk-python-teo-3.0.882/tencentcloud/teo/v20220106/models.py
+-rw-r--r--   0 root         (0) root         (0)     5379 2023-04-26 03:51:22.000000 tencentcloud-sdk-python-teo-3.0.882/tencentcloud/teo/v20220106/teo_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 03:51:22.000000 tencentcloud-sdk-python-teo-3.0.882/tencentcloud/teo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:51:22.000000 tencentcloud-sdk-python-teo-3.0.882/tencentcloud/teo/v20220901/
+-rw-r--r--   0 root         (0) root         (0)    21826 2023-04-26 03:51:22.000000 tencentcloud-sdk-python-teo-3.0.882/tencentcloud/teo/v20220901/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 03:51:22.000000 tencentcloud-sdk-python-teo-3.0.882/tencentcloud/teo/v20220901/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   512047 2023-04-26 03:51:22.000000 tencentcloud-sdk-python-teo-3.0.882/tencentcloud/teo/v20220901/models.py
+-rw-r--r--   0 root         (0) root         (0)    84601 2023-04-26 03:51:22.000000 tencentcloud-sdk-python-teo-3.0.882/tencentcloud/teo/v20220901/teo_client.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-26 03:51:22.000000 tencentcloud-sdk-python-teo-3.0.882/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-26 03:51:22.000000 tencentcloud-sdk-python-teo-3.0.882/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:51:22.000000 tencentcloud-sdk-python-teo-3.0.882/tencentcloud_sdk_python_teo.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 03:51:22.000000 tencentcloud-sdk-python-teo-3.0.882/tencentcloud_sdk_python_teo.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      603 2023-04-26 03:51:22.000000 tencentcloud-sdk-python-teo-3.0.882/tencentcloud_sdk_python_teo.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-26 03:51:22.000000 tencentcloud-sdk-python-teo-3.0.882/tencentcloud_sdk_python_teo.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-26 03:51:22.000000 tencentcloud-sdk-python-teo-3.0.882/tencentcloud_sdk_python_teo.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-26 03:51:22.000000 tencentcloud-sdk-python-teo-3.0.882/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-26 03:51:22.000000 tencentcloud-sdk-python-teo-3.0.882/setup.cfg
```

### Comparing `tencentcloud-sdk-python-teo-3.0.881/README.rst` & `tencentcloud-sdk-python-teo-3.0.882/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.881/tencentcloud/teo/v20220106/errorcodes.py` & `tencentcloud-sdk-python-teo-3.0.882/tencentcloud/teo/v20220106/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.881/tencentcloud/teo/v20220106/models.py` & `tencentcloud-sdk-python-teo-3.0.882/tencentcloud/teo/v20220106/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.881/tencentcloud/teo/v20220106/teo_client.py` & `tencentcloud-sdk-python-teo-3.0.882/tencentcloud/teo/v20220106/teo_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.881/tencentcloud/teo/v20220901/errorcodes.py` & `tencentcloud-sdk-python-teo-3.0.882/tencentcloud/teo/v20220901/errorcodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -517,14 +517,17 @@
 
 # 资源不足。
 RESOURCEINSUFFICIENT = 'ResourceInsufficient'
 
 # 资源不存在。
 RESOURCENOTFOUND = 'ResourceNotFound'
 
+# 最大上传大小额度未配置
+RESOURCENOTFOUND_POSTMAXSIZEQUOTANOTFOUND = 'ResourceNotFound.PostMaxSizeQuotaNotFound'
+
 # 资源不可用。
 RESOURCEUNAVAILABLE = 'ResourceUnavailable'
 
 # 证书不存在或未授权。
 RESOURCEUNAVAILABLE_CERTNOTFOUND = 'ResourceUnavailable.CertNotFound'
 
 # 当前域名已接入EdgeOne，如确认需要接入到当前账号，请进行域名找回。
```

### Comparing `tencentcloud-sdk-python-teo-3.0.881/tencentcloud/teo/v20220901/models.py` & `tencentcloud-sdk-python-teo-3.0.882/tencentcloud/teo/v20220901/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,40 @@
 # limitations under the License.
 
 import warnings
 
 from tencentcloud.common.abstract_model import AbstractModel
 
 
+class AccelerateMainland(AbstractModel):
+    """中国大陆加速优化配置。
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Switch: 是否开启中国大陆加速优化配置，取值有：
+<li>on：开启；</li>
+<li>off：关闭。</li>
+        :type Switch: str
+        """
+        self.Switch = None
+
+
+    def _deserialize(self, params):
+        self.Switch = params.get("Switch")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class AccelerateType(AbstractModel):
     """加速类型
 
     """
 
     def __init__(self):
         r"""
@@ -1418,15 +1444,15 @@
 注意：此字段可能返回 null，表示取不到有效值。
         :type FullUrlCache: str
         :param IgnoreCase: 是否忽略大小写缓存，取值有：
 <li>on：忽略；</li>
 <li>off：不忽略。</li>
 注意：此字段可能返回 null，表示取不到有效值。
         :type IgnoreCase: str
-        :param QueryString: CacheKey中包含请求参数。
+        :param QueryString: CacheKey 中包含请求参数。
 注意：此字段可能返回 null，表示取不到有效值。
         :type QueryString: :class:`tencentcloud.teo.v20220901.models.QueryString`
         """
         self.FullUrlCache = None
         self.IgnoreCase = None
         self.QueryString = None
 
@@ -1529,15 +1555,15 @@
 
     def __init__(self):
         r"""
         :param Switch: 配置开关，取值有：
 <li>on：开启；</li>
 <li>off：关闭。</li>
         :type Switch: str
-        :param HeaderName: 存放客户端IP所属地域信息的请求头名称，当Switch=on时有效。
+        :param HeaderName: 存放客户端 IP 所属地域信息的请求头名称，当 Switch=on 时有效。
 为空则使用默认值：EO-Client-IPCountry。
         :type HeaderName: str
         """
         self.Switch = None
         self.HeaderName = None
 
 
@@ -1560,15 +1586,15 @@
 
     def __init__(self):
         r"""
         :param Switch: 配置开关，取值有：
 <li>on：开启；</li>
 <li>off：关闭。</li>
         :type Switch: str
-        :param HeaderName: 回源时，存放客户端IP的请求头名称。
+        :param HeaderName: 回源时，存放客户端 IP 的请求头名称。
 为空则使用默认值：X-Forwarded-IP。
 注意：此字段可能返回 null，表示取不到有效值。
         :type HeaderName: str
         """
         self.Switch = None
         self.HeaderName = None
 
@@ -1900,18 +1926,18 @@
 class CreateApplicationProxyRequest(AbstractModel):
     """CreateApplicationProxy请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param ZoneId: 站点ID。
+        :param ZoneId: 站点 ID。
         :type ZoneId: str
-        :param ProxyName: 当ProxyType=hostname时，表示域名或子域名；
-当ProxyType=instance时，表示代理名称。
+        :param ProxyName: 当 ProxyType=hostname 时，表示域名或子域名；
+当 ProxyType=instance 时，表示代理名称。
         :type ProxyName: str
         :param PlatType: 调度模式，取值有：
 <li>ip：表示Anycast IP调度；</li>
 <li>domain：表示CNAME调度。</li>
         :type PlatType: str
         :param SecurityType: 是否开启安全，取值有：
 <li>0：关闭安全；</li>
@@ -1924,30 +1950,33 @@
         :param ProxyType: 四层代理模式，取值有：
 <li>hostname：表示子域名模式；</li>
 <li>instance：表示实例模式。</li>不填写使用默认值instance。
         :type ProxyType: str
         :param SessionPersistTime: 会话保持时间，取值范围：30-3600，单位：秒。
 不填写使用默认值600。
         :type SessionPersistTime: int
-        :param Ipv6: Ipv6访问配置。
-不填写表示关闭Ipv6访问。
+        :param Ipv6: Ipv6 访问配置。
+不填写表示关闭 Ipv6 访问。
         :type Ipv6: :class:`tencentcloud.teo.v20220901.models.Ipv6`
         :param ApplicationProxyRules: 规则详细信息。
 不填写则不创建规则。
         :type ApplicationProxyRules: list of ApplicationProxyRule
+        :param AccelerateMainland: 中国大陆加速优化配置。不填写表示关闭中国大陆加速优化。
+        :type AccelerateMainland: :class:`tencentcloud.teo.v20220901.models.AccelerateMainland`
         """
         self.ZoneId = None
         self.ProxyName = None
         self.PlatType = None
         self.SecurityType = None
         self.AccelerateType = None
         self.ProxyType = None
         self.SessionPersistTime = None
         self.Ipv6 = None
         self.ApplicationProxyRules = None
+        self.AccelerateMainland = None
 
 
     def _deserialize(self, params):
         self.ZoneId = params.get("ZoneId")
         self.ProxyName = params.get("ProxyName")
         self.PlatType = params.get("PlatType")
         self.SecurityType = params.get("SecurityType")
@@ -1959,14 +1988,17 @@
             self.Ipv6._deserialize(params.get("Ipv6"))
         if params.get("ApplicationProxyRules") is not None:
             self.ApplicationProxyRules = []
             for item in params.get("ApplicationProxyRules"):
                 obj = ApplicationProxyRule()
                 obj._deserialize(item)
                 self.ApplicationProxyRules.append(obj)
+        if params.get("AccelerateMainland") is not None:
+            self.AccelerateMainland = AccelerateMainland()
+            self.AccelerateMainland._deserialize(params.get("AccelerateMainland"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -2524,14 +2556,65 @@
 
 
     def _deserialize(self, params):
         self.RuleId = params.get("RuleId")
         self.RequestId = params.get("RequestId")
 
 
+class CreateSecurityIPGroupRequest(AbstractModel):
+    """CreateSecurityIPGroup请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ZoneId: 站点 Id。
+        :type ZoneId: str
+        :param IPGroup: IP 组信息。
+        :type IPGroup: :class:`tencentcloud.teo.v20220901.models.IPGroup`
+        """
+        self.ZoneId = None
+        self.IPGroup = None
+
+
+    def _deserialize(self, params):
+        self.ZoneId = params.get("ZoneId")
+        if params.get("IPGroup") is not None:
+            self.IPGroup = IPGroup()
+            self.IPGroup._deserialize(params.get("IPGroup"))
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class CreateSecurityIPGroupResponse(AbstractModel):
+    """CreateSecurityIPGroup返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param GroupId: IP 组 Id。
+        :type GroupId: int
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.GroupId = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.GroupId = params.get("GroupId")
+        self.RequestId = params.get("RequestId")
+
+
 class CreateSpeedTestingRequest(AbstractModel):
     """CreateSpeedTesting请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -3132,14 +3215,59 @@
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
 
 
+class DeleteSecurityIPGroupRequest(AbstractModel):
+    """DeleteSecurityIPGroup请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ZoneId: 站点 Id。
+        :type ZoneId: str
+        :param GroupId: IP 组 Id。
+        :type GroupId: int
+        """
+        self.ZoneId = None
+        self.GroupId = None
+
+
+    def _deserialize(self, params):
+        self.ZoneId = params.get("ZoneId")
+        self.GroupId = params.get("GroupId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DeleteSecurityIPGroupResponse(AbstractModel):
+    """DeleteSecurityIPGroup返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
 class DeleteZoneRequest(AbstractModel):
     """DeleteZone请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -7501,15 +7629,15 @@
 class Grpc(AbstractModel):
     """Grpc配置项
 
     """
 
     def __init__(self):
         r"""
-        :param Switch: 是否开启Grpc配置，取值有：
+        :param Switch: 是否开启 Grpc 配置，取值有：
 <li>on：开启；</li>
 <li>off：关闭。</li>
         :type Switch: str
         """
         self.Switch = None
 
 
@@ -7559,15 +7687,15 @@
 
     def __init__(self):
         r"""
         :param Switch: 是否开启，取值有：
 <li>on：开启；</li>
 <li>off：关闭。</li>
         :type Switch: str
-        :param MaxAge: MaxAge数值。单位为秒，最大值为1天。
+        :param MaxAge: MaxAge 数值。单位为秒，最大值为1天。
 注意：此字段可能返回 null，表示取不到有效值。
         :type MaxAge: int
         :param IncludeSubDomains: 是否包含子域名，取值有：
 <li>on：开启；</li>
 <li>off：关闭。</li>
 注意：此字段可能返回 null，表示取不到有效值。
         :type IncludeSubDomains: str
@@ -7610,15 +7738,15 @@
 注意：此字段可能返回 null，表示取不到有效值。
         :type Http2: str
         :param OcspStapling: OCSP 配置开关，取值有：
 <li>on：开启；</li>
 <li>off：关闭。</li>
 注意：此字段可能返回 null，表示取不到有效值。
         :type OcspStapling: str
-        :param TlsVersion: Tls版本设置，取值有：
+        :param TlsVersion: Tls 版本设置，取值有：
 <li>TLSv1：TLSv1版本；</li>
 <li>TLSV1.1：TLSv1.1版本；</li>
 <li>TLSV1.2：TLSv1.2版本；</li>
 <li>TLSv1.3：TLSv1.3版本。</li>修改时必须开启连续的版本。
 注意：此字段可能返回 null，表示取不到有效值。
         :type TlsVersion: list of str
         :param Hsts: HSTS 配置。
@@ -7668,14 +7796,46 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class IPGroup(AbstractModel):
+    """IP 网段组
+
+    """
+
+    def __init__(self):
+        r"""
+        :param GroupId: 组 Id，创建时填 0 即可。
+        :type GroupId: int
+        :param Name: 组名称。
+        :type Name: str
+        :param Content: IP 组内容，可以填入 IP 及 IP 掩码。
+        :type Content: list of str
+        """
+        self.GroupId = None
+        self.Name = None
+        self.Content = None
+
+
+    def _deserialize(self, params):
+        self.GroupId = params.get("GroupId")
+        self.Name = params.get("Name")
+        self.Content = params.get("Content")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class IPWhitelist(AbstractModel):
     """源站防护IP白名单
 
     """
 
     def __init__(self):
         r"""
@@ -8019,15 +8179,15 @@
 class Ipv6(AbstractModel):
     """Ipv6访问配置
 
     """
 
     def __init__(self):
         r"""
-        :param Switch: Ipv6访问功能配置，取值有：
+        :param Switch: Ipv6 访问功能配置，取值有：
 <li>on：开启Ipv6访问功能；</li>
 <li>off：关闭Ipv6访问功能。</li>
         :type Switch: str
         """
         self.Switch = None
 
 
@@ -8426,48 +8586,54 @@
 class ModifyApplicationProxyRequest(AbstractModel):
     """ModifyApplicationProxy请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param ZoneId: 站点ID。
+        :param ZoneId: 站点 ID。
         :type ZoneId: str
-        :param ProxyId: 代理ID。
+        :param ProxyId: 代理 ID。
         :type ProxyId: str
-        :param ProxyName: 当ProxyType=hostname时，表示域名或子域名；
-当ProxyType=instance时，表示代理名称。
+        :param ProxyName: 当 ProxyType=hostname 时，表示域名或子域名；
+当 ProxyType=instance 时，表示代理名称。
         :type ProxyName: str
         :param SessionPersistTime: 会话保持时间，取值范围：30-3600，单位：秒。
 不填写保持原有配置。
         :type SessionPersistTime: int
         :param ProxyType: 四层代理模式，取值有：
 <li>hostname：表示子域名模式；</li>
 <li>instance：表示实例模式。</li>不填写保持原有配置。
         :type ProxyType: str
-        :param Ipv6: Ipv6访问配置，不填写保持原有配置。
+        :param Ipv6: Ipv6 访问配置，不填写保持原有配置。
         :type Ipv6: :class:`tencentcloud.teo.v20220901.models.Ipv6`
+        :param AccelerateMainland: 中国大陆加速优化配置。 不填写表示保持原有配置。
+        :type AccelerateMainland: :class:`tencentcloud.teo.v20220901.models.AccelerateMainland`
         """
         self.ZoneId = None
         self.ProxyId = None
         self.ProxyName = None
         self.SessionPersistTime = None
         self.ProxyType = None
         self.Ipv6 = None
+        self.AccelerateMainland = None
 
 
     def _deserialize(self, params):
         self.ZoneId = params.get("ZoneId")
         self.ProxyId = params.get("ProxyId")
         self.ProxyName = params.get("ProxyName")
         self.SessionPersistTime = params.get("SessionPersistTime")
         self.ProxyType = params.get("ProxyType")
         if params.get("Ipv6") is not None:
             self.Ipv6 = Ipv6()
             self.Ipv6._deserialize(params.get("Ipv6"))
+        if params.get("AccelerateMainland") is not None:
+            self.AccelerateMainland = AccelerateMainland()
+            self.AccelerateMainland._deserialize(params.get("AccelerateMainland"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -8992,14 +9158,68 @@
 
 
     def _deserialize(self, params):
         self.RuleId = params.get("RuleId")
         self.RequestId = params.get("RequestId")
 
 
+class ModifySecurityIPGroupRequest(AbstractModel):
+    """ModifySecurityIPGroup请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ZoneId: 站点 Id。
+        :type ZoneId: str
+        :param IPGroup: IP 组配置。
+        :type IPGroup: :class:`tencentcloud.teo.v20220901.models.IPGroup`
+        :param Mode: 操作类型，取值有：
+<li> append: 向 IPGroup 中追加 Content 参数中内容；</li>
+<li> remove: 从 IPGroup 中删除 Content 参数中内容；</li>
+<li> update: 全量替换 IPGroup 内容，并可修改 IPGroup 名称。 </li>
+        :type Mode: str
+        """
+        self.ZoneId = None
+        self.IPGroup = None
+        self.Mode = None
+
+
+    def _deserialize(self, params):
+        self.ZoneId = params.get("ZoneId")
+        if params.get("IPGroup") is not None:
+            self.IPGroup = IPGroup()
+            self.IPGroup._deserialize(params.get("IPGroup"))
+        self.Mode = params.get("Mode")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class ModifySecurityIPGroupResponse(AbstractModel):
+    """ModifySecurityIPGroup返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
 class ModifySecurityPolicyRequest(AbstractModel):
     """ModifySecurityPolicy请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -9202,70 +9422,73 @@
 class ModifyZoneSettingRequest(AbstractModel):
     """ModifyZoneSetting请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param ZoneId: 待变更的站点ID。
+        :param ZoneId: 待变更的站点 ID。
         :type ZoneId: str
         :param CacheConfig: 缓存过期时间配置。
 不填写表示保持原有配置。
         :type CacheConfig: :class:`tencentcloud.teo.v20220901.models.CacheConfig`
         :param CacheKey: 节点缓存键配置。
 不填写表示保持原有配置。
         :type CacheKey: :class:`tencentcloud.teo.v20220901.models.CacheKey`
         :param MaxAge: 浏览器缓存配置。
 不填写表示保持原有配置。
         :type MaxAge: :class:`tencentcloud.teo.v20220901.models.MaxAge`
         :param OfflineCache: 离线缓存配置。
 不填写表示保持原有配置。
         :type OfflineCache: :class:`tencentcloud.teo.v20220901.models.OfflineCache`
-        :param Quic: Quic访问配置。
+        :param Quic: Quic 访问配置。
 不填写表示保持原有配置。
         :type Quic: :class:`tencentcloud.teo.v20220901.models.Quic`
-        :param PostMaxSize: Post请求传输配置。
+        :param PostMaxSize: Post 请求传输配置。
 不填写表示保持原有配置。
         :type PostMaxSize: :class:`tencentcloud.teo.v20220901.models.PostMaxSize`
         :param Compression: 智能压缩配置。
 不填写表示保持原有配置。
         :type Compression: :class:`tencentcloud.teo.v20220901.models.Compression`
-        :param UpstreamHttp2: Http2回源配置。
+        :param UpstreamHttp2: Http2 回源配置。
 不填写表示保持原有配置。
         :type UpstreamHttp2: :class:`tencentcloud.teo.v20220901.models.UpstreamHttp2`
-        :param ForceRedirect: 访问协议强制Https跳转配置。
+        :param ForceRedirect: 访问协议强制 Https 跳转配置。
 不填写表示保持原有配置。
         :type ForceRedirect: :class:`tencentcloud.teo.v20220901.models.ForceRedirect`
-        :param Https: Https加速配置。
+        :param Https: Https 加速配置。
 不填写表示保持原有配置。
         :type Https: :class:`tencentcloud.teo.v20220901.models.Https`
         :param Origin: 源站配置。
 不填写表示保持原有配置。
         :type Origin: :class:`tencentcloud.teo.v20220901.models.Origin`
         :param SmartRouting: 智能加速配置。
 不填写表示保持原有配置。
         :type SmartRouting: :class:`tencentcloud.teo.v20220901.models.SmartRouting`
-        :param WebSocket: WebSocket配置。
+        :param WebSocket: WebSocket 配置。
 不填写表示保持原有配置。
         :type WebSocket: :class:`tencentcloud.teo.v20220901.models.WebSocket`
-        :param ClientIpHeader: 客户端IP回源请求头配置。
+        :param ClientIpHeader: 客户端 IP 回源请求头配置。
 不填写表示保持原有配置。
         :type ClientIpHeader: :class:`tencentcloud.teo.v20220901.models.ClientIpHeader`
         :param CachePrefresh: 缓存预刷新配置。
 不填写表示保持原有配置。
         :type CachePrefresh: :class:`tencentcloud.teo.v20220901.models.CachePrefresh`
-        :param Ipv6: Ipv6访问配置。
+        :param Ipv6: Ipv6 访问配置。
 不填写表示保持原有配置。
         :type Ipv6: :class:`tencentcloud.teo.v20220901.models.Ipv6`
-        :param ClientIpCountry: 回源时是否携带客户端IP所属地域信息的配置。
+        :param ClientIpCountry: 回源时是否携带客户端 IP 所属地域信息的配置。
 不填写表示保持原有配置。
         :type ClientIpCountry: :class:`tencentcloud.teo.v20220901.models.ClientIpCountry`
-        :param Grpc: Grpc协议支持配置。
+        :param Grpc: Grpc 协议支持配置。
 不填写表示保持原有配置。
         :type Grpc: :class:`tencentcloud.teo.v20220901.models.Grpc`
+        :param ImageOptimize: 图片优化配置。
+不填写表示关闭。
+        :type ImageOptimize: :class:`tencentcloud.teo.v20220901.models.ImageOptimize`
         """
         self.ZoneId = None
         self.CacheConfig = None
         self.CacheKey = None
         self.MaxAge = None
         self.OfflineCache = None
         self.Quic = None
@@ -9278,14 +9501,15 @@
         self.SmartRouting = None
         self.WebSocket = None
         self.ClientIpHeader = None
         self.CachePrefresh = None
         self.Ipv6 = None
         self.ClientIpCountry = None
         self.Grpc = None
+        self.ImageOptimize = None
 
 
     def _deserialize(self, params):
         self.ZoneId = params.get("ZoneId")
         if params.get("CacheConfig") is not None:
             self.CacheConfig = CacheConfig()
             self.CacheConfig._deserialize(params.get("CacheConfig"))
@@ -9336,14 +9560,17 @@
             self.Ipv6._deserialize(params.get("Ipv6"))
         if params.get("ClientIpCountry") is not None:
             self.ClientIpCountry = ClientIpCountry()
             self.ClientIpCountry._deserialize(params.get("ClientIpCountry"))
         if params.get("Grpc") is not None:
             self.Grpc = Grpc()
             self.Grpc._deserialize(params.get("Grpc"))
+        if params.get("ImageOptimize") is not None:
+            self.ImageOptimize = ImageOptimize()
+            self.ImageOptimize._deserialize(params.get("ImageOptimize"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -9552,15 +9779,15 @@
         :type BackupOrigins: list of str
         :param OriginPullProtocol: 回源协议配置，取值有：
 <li>http：强制 http 回源；</li>
 <li>follow：协议跟随回源；</li>
 <li>https：强制 https 回源。</li>
 注意：此字段可能返回 null，表示取不到有效值。
         :type OriginPullProtocol: str
-        :param CosPrivateAccess: 源站为腾讯云COS时，是否为私有访问bucket，取值有：
+        :param CosPrivateAccess: 源站为腾讯云 COS 时，是否为私有访问 bucket，取值有：
 <li>on：私有访问；</li>
 <li>off：公共访问。</li>
 注意：此字段可能返回 null，表示取不到有效值。
         :type CosPrivateAccess: str
         """
         self.Origins = None
         self.BackupOrigins = None
@@ -10006,15 +10233,15 @@
 class PostMaxSize(AbstractModel):
     """POST请求上传文件流式传输最大限制
 
     """
 
     def __init__(self):
         r"""
-        :param Switch: 是否开启POST请求上传文件限制，平台默认为限制为32MB，取值有：
+        :param Switch: 是否开启 POST 请求上传文件限制，平台默认为限制为32MB，取值有：
 <li>on：开启限制；</li>
 <li>off：关闭限制。</li>
         :type Switch: str
         :param MaxSize: 最大限制，取值在1MB和500MB之间。单位字节。
 注意：此字段可能返回 null，表示取不到有效值。
         :type MaxSize: int
         """
@@ -10145,15 +10372,15 @@
 class Quic(AbstractModel):
     """Quic配置项
 
     """
 
     def __init__(self):
         r"""
-        :param Switch: 是否开启Quic配置，取值有：
+        :param Switch: 是否开启 Quic 配置，取值有：
 <li>on：开启；</li>
 <li>off：关闭。</li>
         :type Switch: str
         """
         self.Switch = None
 
 
@@ -12747,15 +12974,15 @@
 class UpstreamHttp2(AbstractModel):
     """Http2回源配置
 
     """
 
     def __init__(self):
         r"""
-        :param Switch: http2回源配置开关，取值有：
+        :param Switch: http2 回源配置开关，取值有：
 <li>on：开启；</li>
 <li>off：关闭。</li>
         :type Switch: str
         """
         self.Switch = None
```

### Comparing `tencentcloud-sdk-python-teo-3.0.881/tencentcloud/teo/v20220901/teo_client.py` & `tencentcloud-sdk-python-teo-3.0.882/tencentcloud/teo/v20220901/teo_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -321,14 +321,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def CreateSecurityIPGroup(self, request):
+        """创建安全 IP 组
+
+        :param request: Request instance for CreateSecurityIPGroup.
+        :type request: :class:`tencentcloud.teo.v20220901.models.CreateSecurityIPGroupRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.CreateSecurityIPGroupResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CreateSecurityIPGroup", params, headers=headers)
+            response = json.loads(body)
+            model = models.CreateSecurityIPGroupResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def CreateSpeedTesting(self, request):
         """对用户指定的域名进行一次站点拨测
 
         :param request: Request instance for CreateSpeedTesting.
         :type request: :class:`tencentcloud.teo.v20220901.models.CreateSpeedTestingRequest`
         :rtype: :class:`tencentcloud.teo.v20220901.models.CreateSpeedTestingResponse`
 
@@ -505,14 +528,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DeleteSecurityIPGroup(self, request):
+        """删除指定 IP 组，如果有规则引用了 IP 组情况，则不允许删除。
+
+        :param request: Request instance for DeleteSecurityIPGroup.
+        :type request: :class:`tencentcloud.teo.v20220901.models.DeleteSecurityIPGroupRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.DeleteSecurityIPGroupResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DeleteSecurityIPGroup", params, headers=headers)
+            response = json.loads(body)
+            model = models.DeleteSecurityIPGroupResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DeleteZone(self, request):
         """删除站点。
 
         :param request: Request instance for DeleteZone.
         :type request: :class:`tencentcloud.teo.v20220901.models.DeleteZoneRequest`
         :rtype: :class:`tencentcloud.teo.v20220901.models.DeleteZoneResponse`
 
@@ -1860,14 +1906,37 @@
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
+
+
+    def ModifySecurityIPGroup(self, request):
+        """修改安全 IP 组。
+
+        :param request: Request instance for ModifySecurityIPGroup.
+        :type request: :class:`tencentcloud.teo.v20220901.models.ModifySecurityIPGroupRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.ModifySecurityIPGroupResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("ModifySecurityIPGroup", params, headers=headers)
+            response = json.loads(body)
+            model = models.ModifySecurityIPGroupResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
 
 
     def ModifySecurityPolicy(self, request):
         """修改Web&Bot安全配置。
 
         :param request: Request instance for ModifySecurityPolicy.
         :type request: :class:`tencentcloud.teo.v20220901.models.ModifySecurityPolicyRequest`
```

### Comparing `tencentcloud-sdk-python-teo-3.0.881/tencentcloud/__init__.py` & `tencentcloud-sdk-python-teo-3.0.882/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-teo-3.0.881/PKG-INFO` & `tencentcloud-sdk-python-teo-3.0.882/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-teo
-Version: 3.0.881
+Version: 3.0.882
 Summary: Tencent Cloud Teo SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-teo-3.0.881/tencentcloud_sdk_python_teo.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-teo-3.0.882/tencentcloud_sdk_python_teo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.881/tencentcloud_sdk_python_teo.egg-info/PKG-INFO` & `tencentcloud-sdk-python-teo-3.0.882/tencentcloud_sdk_python_teo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-teo
-Version: 3.0.881
+Version: 3.0.882
 Summary: Tencent Cloud Teo SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-teo-3.0.881/setup.py` & `tencentcloud-sdk-python-teo-3.0.882/setup.py`

 * *Files identical despite different names*

