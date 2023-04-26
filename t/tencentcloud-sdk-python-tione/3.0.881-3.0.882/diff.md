# Comparing `tmp/tencentcloud-sdk-python-tione-3.0.881.tar.gz` & `tmp/tencentcloud-sdk-python-tione-3.0.882.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tione-3.0.881.tar", last modified: Tue Apr 25 00:58:21 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tione-3.0.882.tar", last modified: Wed Apr 26 03:57:34 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tione-3.0.881.tar` & `tencentcloud-sdk-python-tione-3.0.882.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:58:21.000000 tencentcloud-sdk-python-tione-3.0.881/
--rw-r--r--   0 root         (0) root         (0)      743 2023-04-25 00:58:21.000000 tencentcloud-sdk-python-tione-3.0.881/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:58:21.000000 tencentcloud-sdk-python-tione-3.0.881/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-25 00:58:21.000000 tencentcloud-sdk-python-tione-3.0.881/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:58:21.000000 tencentcloud-sdk-python-tione-3.0.881/tencentcloud/tione/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 00:58:21.000000 tencentcloud-sdk-python-tione-3.0.881/tencentcloud/tione/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:58:21.000000 tencentcloud-sdk-python-tione-3.0.881/tencentcloud/tione/v20211111/
--rw-r--r--   0 root         (0) root         (0)    51024 2023-04-25 00:58:21.000000 tencentcloud-sdk-python-tione-3.0.881/tencentcloud/tione/v20211111/tione_client.py
--rw-r--r--   0 root         (0) root         (0)    10731 2023-04-25 00:58:21.000000 tencentcloud-sdk-python-tione-3.0.881/tencentcloud/tione/v20211111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 00:58:21.000000 tencentcloud-sdk-python-tione-3.0.881/tencentcloud/tione/v20211111/__init__.py
--rw-r--r--   0 root         (0) root         (0)   331524 2023-04-25 00:58:21.000000 tencentcloud-sdk-python-tione-3.0.881/tencentcloud/tione/v20211111/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:58:21.000000 tencentcloud-sdk-python-tione-3.0.881/tencentcloud/tione/v20191022/
--rw-r--r--   0 root         (0) root         (0)    22010 2023-04-25 00:58:21.000000 tencentcloud-sdk-python-tione-3.0.881/tencentcloud/tione/v20191022/tione_client.py
--rw-r--r--   0 root         (0) root         (0)     4465 2023-04-25 00:58:21.000000 tencentcloud-sdk-python-tione-3.0.881/tencentcloud/tione/v20191022/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 00:58:21.000000 tencentcloud-sdk-python-tione-3.0.881/tencentcloud/tione/v20191022/__init__.py
--rw-r--r--   0 root         (0) root         (0)    91250 2023-04-25 00:58:21.000000 tencentcloud-sdk-python-tione-3.0.881/tencentcloud/tione/v20191022/models.py
--rw-r--r--   0 root         (0) root         (0)     1669 2023-04-25 00:58:21.000000 tencentcloud-sdk-python-tione-3.0.881/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1010 2023-04-25 00:58:21.000000 tencentcloud-sdk-python-tione-3.0.881/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-25 00:58:21.000000 tencentcloud-sdk-python-tione-3.0.881/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:58:21.000000 tencentcloud-sdk-python-tione-3.0.881/tencentcloud_sdk_python_tione.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 00:58:21.000000 tencentcloud-sdk-python-tione-3.0.881/tencentcloud_sdk_python_tione.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      633 2023-04-25 00:58:21.000000 tencentcloud-sdk-python-tione-3.0.881/tencentcloud_sdk_python_tione.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-04-25 00:58:21.000000 tencentcloud-sdk-python-tione-3.0.881/tencentcloud_sdk_python_tione.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-25 00:58:21.000000 tencentcloud-sdk-python-tione-3.0.881/tencentcloud_sdk_python_tione.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:57:34.000000 tencentcloud-sdk-python-tione-3.0.882/
+-rw-r--r--   0 root         (0) root         (0)      743 2023-04-26 03:57:34.000000 tencentcloud-sdk-python-tione-3.0.882/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:57:34.000000 tencentcloud-sdk-python-tione-3.0.882/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-26 03:57:34.000000 tencentcloud-sdk-python-tione-3.0.882/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:57:34.000000 tencentcloud-sdk-python-tione-3.0.882/tencentcloud/tione/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 03:57:34.000000 tencentcloud-sdk-python-tione-3.0.882/tencentcloud/tione/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:57:34.000000 tencentcloud-sdk-python-tione-3.0.882/tencentcloud/tione/v20211111/
+-rw-r--r--   0 root         (0) root         (0)    51024 2023-04-26 03:57:34.000000 tencentcloud-sdk-python-tione-3.0.882/tencentcloud/tione/v20211111/tione_client.py
+-rw-r--r--   0 root         (0) root         (0)    10734 2023-04-26 03:57:34.000000 tencentcloud-sdk-python-tione-3.0.882/tencentcloud/tione/v20211111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 03:57:34.000000 tencentcloud-sdk-python-tione-3.0.882/tencentcloud/tione/v20211111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   331524 2023-04-26 03:57:34.000000 tencentcloud-sdk-python-tione-3.0.882/tencentcloud/tione/v20211111/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:57:34.000000 tencentcloud-sdk-python-tione-3.0.882/tencentcloud/tione/v20191022/
+-rw-r--r--   0 root         (0) root         (0)    22010 2023-04-26 03:57:34.000000 tencentcloud-sdk-python-tione-3.0.882/tencentcloud/tione/v20191022/tione_client.py
+-rw-r--r--   0 root         (0) root         (0)     4465 2023-04-26 03:57:34.000000 tencentcloud-sdk-python-tione-3.0.882/tencentcloud/tione/v20191022/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 03:57:34.000000 tencentcloud-sdk-python-tione-3.0.882/tencentcloud/tione/v20191022/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    91250 2023-04-26 03:57:34.000000 tencentcloud-sdk-python-tione-3.0.882/tencentcloud/tione/v20191022/models.py
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-04-26 03:57:34.000000 tencentcloud-sdk-python-tione-3.0.882/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-04-26 03:57:34.000000 tencentcloud-sdk-python-tione-3.0.882/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-26 03:57:34.000000 tencentcloud-sdk-python-tione-3.0.882/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:57:34.000000 tencentcloud-sdk-python-tione-3.0.882/tencentcloud_sdk_python_tione.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 03:57:34.000000 tencentcloud-sdk-python-tione-3.0.882/tencentcloud_sdk_python_tione.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      633 2023-04-26 03:57:34.000000 tencentcloud-sdk-python-tione-3.0.882/tencentcloud_sdk_python_tione.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-04-26 03:57:34.000000 tencentcloud-sdk-python-tione-3.0.882/tencentcloud_sdk_python_tione.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-26 03:57:34.000000 tencentcloud-sdk-python-tione-3.0.882/tencentcloud_sdk_python_tione.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-tione-3.0.881/README.rst` & `tencentcloud-sdk-python-tione-3.0.882/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.881/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tione-3.0.882/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tione-3.0.881/tencentcloud/tione/v20211111/tione_client.py` & `tencentcloud-sdk-python-tione-3.0.882/tencentcloud/tione/v20211111/tione_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.881/tencentcloud/tione/v20211111/errorcodes.py` & `tencentcloud-sdk-python-tione-3.0.882/tencentcloud/tione/v20211111/errorcodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -268,15 +268,15 @@
 
 # 操作被拒绝。
 OPERATIONDENIED = 'OperationDenied'
 
 # 余额不足，创建/更新失败。
 OPERATIONDENIED_BALANCEINSUFFICIENT = 'OperationDenied.BalanceInsufficient'
 
-# 后付费资源售罄。
+# 按量计费资源售罄。
 OPERATIONDENIED_BILLINGSTATUSRESOURCEINSUFFICIENT = 'OperationDenied.BillingStatusResourceInsufficient'
 
 # 觅影资源包余额不足，请先充值。
 OPERATIONDENIED_MIYINGBALANCEINSUFFICIENT = 'OperationDenied.MIYINGBalanceInsufficient'
 
 # 网段不合法。
 OPERATIONDENIED_NETWORKCIDRILLEGAL = 'OperationDenied.NetworkCidrIllegal'
```

### Comparing `tencentcloud-sdk-python-tione-3.0.881/tencentcloud/tione/v20211111/models.py` & `tencentcloud-sdk-python-tione-3.0.882/tencentcloud/tione/v20211111/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2991,15 +2991,15 @@
 
     """
 
     def __init__(self):
         r"""
         :param TaskType: 枚举值：TRAIN、NOTEBOOK、INFERENCE
         :type TaskType: str
-        :param ChargeType: 付费模式：POSTPAID_BY_HOUR按量付费、PREPAID包年包月
+        :param ChargeType: 付费模式：POSTPAID_BY_HOUR按量计费、PREPAID包年包月
         :type ChargeType: str
         :param ResourceType: 资源类型：CALC 计算资源、CPU CPU资源、GPU GPU资源、CBS云硬盘
         :type ResourceType: str
         """
         self.TaskType = None
         self.ChargeType = None
         self.ResourceType = None
```

### Comparing `tencentcloud-sdk-python-tione-3.0.881/tencentcloud/tione/v20191022/tione_client.py` & `tencentcloud-sdk-python-tione-3.0.882/tencentcloud/tione/v20191022/tione_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.881/tencentcloud/tione/v20191022/errorcodes.py` & `tencentcloud-sdk-python-tione-3.0.882/tencentcloud/tione/v20191022/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.881/tencentcloud/tione/v20191022/models.py` & `tencentcloud-sdk-python-tione-3.0.882/tencentcloud/tione/v20191022/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.881/PKG-INFO` & `tencentcloud-sdk-python-tione-3.0.882/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tione
-Version: 3.0.881
+Version: 3.0.882
 Summary: Tencent Cloud Tione SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tione-3.0.881/setup.py` & `tencentcloud-sdk-python-tione-3.0.882/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.881/tencentcloud_sdk_python_tione.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-tione-3.0.882/tencentcloud_sdk_python_tione.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.881/tencentcloud_sdk_python_tione.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tione-3.0.882/tencentcloud_sdk_python_tione.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tione
-Version: 3.0.881
+Version: 3.0.882
 Summary: Tencent Cloud Tione SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

