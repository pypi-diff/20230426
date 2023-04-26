# Comparing `tmp/tencentcloud-sdk-python-cvm-3.0.881.tar.gz` & `tmp/tencentcloud-sdk-python-cvm-3.0.882.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cvm-3.0.881.tar", last modified: Tue Apr 25 00:34:25 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cvm-3.0.882.tar", last modified: Wed Apr 26 03:09:20 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cvm-3.0.881.tar` & `tencentcloud-sdk-python-cvm-3.0.882.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:34:25.000000 tencentcloud-sdk-python-cvm-3.0.881/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-25 00:34:25.000000 tencentcloud-sdk-python-cvm-3.0.881/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:34:25.000000 tencentcloud-sdk-python-cvm-3.0.881/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:34:25.000000 tencentcloud-sdk-python-cvm-3.0.881/tencentcloud/cvm/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:34:25.000000 tencentcloud-sdk-python-cvm-3.0.881/tencentcloud/cvm/v20170312/
--rw-r--r--   0 root         (0) root         (0)   119282 2023-04-25 00:34:25.000000 tencentcloud-sdk-python-cvm-3.0.881/tencentcloud/cvm/v20170312/cvm_client.py
--rw-r--r--   0 root         (0) root         (0)    42810 2023-04-25 00:34:25.000000 tencentcloud-sdk-python-cvm-3.0.881/tencentcloud/cvm/v20170312/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 00:34:25.000000 tencentcloud-sdk-python-cvm-3.0.881/tencentcloud/cvm/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)   429673 2023-04-25 00:34:25.000000 tencentcloud-sdk-python-cvm-3.0.881/tencentcloud/cvm/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 00:34:25.000000 tencentcloud-sdk-python-cvm-3.0.881/tencentcloud/cvm/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-25 00:34:25.000000 tencentcloud-sdk-python-cvm-3.0.881/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-25 00:34:25.000000 tencentcloud-sdk-python-cvm-3.0.881/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-25 00:34:25.000000 tencentcloud-sdk-python-cvm-3.0.881/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-25 00:34:25.000000 tencentcloud-sdk-python-cvm-3.0.881/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:34:25.000000 tencentcloud-sdk-python-cvm-3.0.881/tencentcloud_sdk_python_cvm.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 00:34:25.000000 tencentcloud-sdk-python-cvm-3.0.881/tencentcloud_sdk_python_cvm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-25 00:34:25.000000 tencentcloud-sdk-python-cvm-3.0.881/tencentcloud_sdk_python_cvm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-25 00:34:25.000000 tencentcloud-sdk-python-cvm-3.0.881/tencentcloud_sdk_python_cvm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-25 00:34:25.000000 tencentcloud-sdk-python-cvm-3.0.881/tencentcloud_sdk_python_cvm.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:09:20.000000 tencentcloud-sdk-python-cvm-3.0.882/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-26 03:09:19.000000 tencentcloud-sdk-python-cvm-3.0.882/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:09:20.000000 tencentcloud-sdk-python-cvm-3.0.882/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:09:20.000000 tencentcloud-sdk-python-cvm-3.0.882/tencentcloud/cvm/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:09:20.000000 tencentcloud-sdk-python-cvm-3.0.882/tencentcloud/cvm/v20170312/
+-rw-r--r--   0 root         (0) root         (0)   119282 2023-04-26 03:09:19.000000 tencentcloud-sdk-python-cvm-3.0.882/tencentcloud/cvm/v20170312/cvm_client.py
+-rw-r--r--   0 root         (0) root         (0)    42810 2023-04-26 03:09:19.000000 tencentcloud-sdk-python-cvm-3.0.882/tencentcloud/cvm/v20170312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 03:09:19.000000 tencentcloud-sdk-python-cvm-3.0.882/tencentcloud/cvm/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   429673 2023-04-26 03:09:19.000000 tencentcloud-sdk-python-cvm-3.0.882/tencentcloud/cvm/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 03:09:19.000000 tencentcloud-sdk-python-cvm-3.0.882/tencentcloud/cvm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-26 03:09:19.000000 tencentcloud-sdk-python-cvm-3.0.882/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-26 03:09:20.000000 tencentcloud-sdk-python-cvm-3.0.882/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-26 03:09:19.000000 tencentcloud-sdk-python-cvm-3.0.882/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-26 03:09:20.000000 tencentcloud-sdk-python-cvm-3.0.882/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:09:20.000000 tencentcloud-sdk-python-cvm-3.0.882/tencentcloud_sdk_python_cvm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 03:09:20.000000 tencentcloud-sdk-python-cvm-3.0.882/tencentcloud_sdk_python_cvm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-26 03:09:20.000000 tencentcloud-sdk-python-cvm-3.0.882/tencentcloud_sdk_python_cvm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-26 03:09:20.000000 tencentcloud-sdk-python-cvm-3.0.882/tencentcloud_sdk_python_cvm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-26 03:09:20.000000 tencentcloud-sdk-python-cvm-3.0.882/tencentcloud_sdk_python_cvm.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-cvm-3.0.881/README.rst` & `tencentcloud-sdk-python-cvm-3.0.882/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cvm-3.0.881/tencentcloud/cvm/v20170312/cvm_client.py` & `tencentcloud-sdk-python-cvm-3.0.882/tencentcloud/cvm/v20170312/cvm_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cvm-3.0.881/tencentcloud/cvm/v20170312/errorcodes.py` & `tencentcloud-sdk-python-cvm-3.0.882/tencentcloud/cvm/v20170312/errorcodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -922,15 +922,15 @@
 
 # 该操作仅支持预付费账户
 UNSUPPORTEDOPERATION_ONLYFORPREPAIDACCOUNT = 'UnsupportedOperation.OnlyForPrepaidAccount'
 
 # 无效的原机型。
 UNSUPPORTEDOPERATION_ORIGINALINSTANCETYPEINVALID = 'UnsupportedOperation.OriginalInstanceTypeInvalid'
 
-# 你的账户不支持镜像预热
+# 您的账户不支持镜像预热
 UNSUPPORTEDOPERATION_PREHEATIMAGE = 'UnsupportedOperation.PreheatImage'
 
 # 公共镜像或市场镜像不支持导出。
 UNSUPPORTEDOPERATION_PUBLICIMAGEEXPORTUNSUPPORTED = 'UnsupportedOperation.PublicImageExportUnsupported'
 
 # 当前镜像不支持对该实例的重装操作。
 UNSUPPORTEDOPERATION_RAWLOCALDISKINSREINSTALLTOQCOW2 = 'UnsupportedOperation.RawLocalDiskInsReinstalltoQcow2'
```

### Comparing `tencentcloud-sdk-python-cvm-3.0.881/tencentcloud/cvm/v20170312/models.py` & `tencentcloud-sdk-python-cvm-3.0.882/tencentcloud/cvm/v20170312/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cvm-3.0.881/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cvm-3.0.882/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cvm-3.0.881/PKG-INFO` & `tencentcloud-sdk-python-cvm-3.0.882/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cvm
-Version: 3.0.881
+Version: 3.0.882
 Summary: Tencent Cloud Cvm SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cvm-3.0.881/setup.py` & `tencentcloud-sdk-python-cvm-3.0.882/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cvm-3.0.881/tencentcloud_sdk_python_cvm.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cvm-3.0.882/tencentcloud_sdk_python_cvm.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cvm
-Version: 3.0.881
+Version: 3.0.882
 Summary: Tencent Cloud Cvm SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

