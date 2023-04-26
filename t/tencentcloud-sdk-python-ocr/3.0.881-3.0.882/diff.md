# Comparing `tmp/tencentcloud-sdk-python-ocr-3.0.881.tar.gz` & `tmp/tencentcloud-sdk-python-ocr-3.0.882.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ocr-3.0.881.tar", last modified: Tue Apr 25 00:46:30 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ocr-3.0.882.tar", last modified: Wed Apr 26 03:39:55 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ocr-3.0.881.tar` & `tencentcloud-sdk-python-ocr-3.0.882.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:46:30.000000 tencentcloud-sdk-python-ocr-3.0.881/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:46:30.000000 tencentcloud-sdk-python-ocr-3.0.881/tencentcloud_sdk_python_ocr.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 00:46:30.000000 tencentcloud-sdk-python-ocr-3.0.881/tencentcloud_sdk_python_ocr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-25 00:46:30.000000 tencentcloud-sdk-python-ocr-3.0.881/tencentcloud_sdk_python_ocr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-25 00:46:30.000000 tencentcloud-sdk-python-ocr-3.0.881/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-25 00:46:30.000000 tencentcloud-sdk-python-ocr-3.0.881/tencentcloud_sdk_python_ocr.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-25 00:46:30.000000 tencentcloud-sdk-python-ocr-3.0.881/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:46:30.000000 tencentcloud-sdk-python-ocr-3.0.881/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:46:30.000000 tencentcloud-sdk-python-ocr-3.0.881/tencentcloud/ocr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:46:30.000000 tencentcloud-sdk-python-ocr-3.0.881/tencentcloud/ocr/v20181119/
--rw-r--r--   0 root         (0) root         (0)   107564 2023-04-25 00:46:30.000000 tencentcloud-sdk-python-ocr-3.0.881/tencentcloud/ocr/v20181119/ocr_client.py
--rw-r--r--   0 root         (0) root         (0)     5764 2023-04-25 00:46:30.000000 tencentcloud-sdk-python-ocr-3.0.881/tencentcloud/ocr/v20181119/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 00:46:30.000000 tencentcloud-sdk-python-ocr-3.0.881/tencentcloud/ocr/v20181119/__init__.py
--rw-r--r--   0 root         (0) root         (0)   415162 2023-04-25 00:46:30.000000 tencentcloud-sdk-python-ocr-3.0.881/tencentcloud/ocr/v20181119/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 00:46:30.000000 tencentcloud-sdk-python-ocr-3.0.881/tencentcloud/ocr/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-25 00:46:30.000000 tencentcloud-sdk-python-ocr-3.0.881/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-25 00:46:30.000000 tencentcloud-sdk-python-ocr-3.0.881/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-25 00:46:30.000000 tencentcloud-sdk-python-ocr-3.0.881/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-25 00:46:30.000000 tencentcloud-sdk-python-ocr-3.0.881/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:39:55.000000 tencentcloud-sdk-python-ocr-3.0.882/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:39:55.000000 tencentcloud-sdk-python-ocr-3.0.882/tencentcloud_sdk_python_ocr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 03:39:55.000000 tencentcloud-sdk-python-ocr-3.0.882/tencentcloud_sdk_python_ocr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-26 03:39:55.000000 tencentcloud-sdk-python-ocr-3.0.882/tencentcloud_sdk_python_ocr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-26 03:39:55.000000 tencentcloud-sdk-python-ocr-3.0.882/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-26 03:39:55.000000 tencentcloud-sdk-python-ocr-3.0.882/tencentcloud_sdk_python_ocr.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-26 03:39:55.000000 tencentcloud-sdk-python-ocr-3.0.882/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:39:55.000000 tencentcloud-sdk-python-ocr-3.0.882/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:39:55.000000 tencentcloud-sdk-python-ocr-3.0.882/tencentcloud/ocr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:39:55.000000 tencentcloud-sdk-python-ocr-3.0.882/tencentcloud/ocr/v20181119/
+-rw-r--r--   0 root         (0) root         (0)   107569 2023-04-26 03:39:55.000000 tencentcloud-sdk-python-ocr-3.0.882/tencentcloud/ocr/v20181119/ocr_client.py
+-rw-r--r--   0 root         (0) root         (0)     5764 2023-04-26 03:39:55.000000 tencentcloud-sdk-python-ocr-3.0.882/tencentcloud/ocr/v20181119/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 03:39:55.000000 tencentcloud-sdk-python-ocr-3.0.882/tencentcloud/ocr/v20181119/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   415162 2023-04-26 03:39:55.000000 tencentcloud-sdk-python-ocr-3.0.882/tencentcloud/ocr/v20181119/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 03:39:55.000000 tencentcloud-sdk-python-ocr-3.0.882/tencentcloud/ocr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-26 03:39:55.000000 tencentcloud-sdk-python-ocr-3.0.882/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-26 03:39:55.000000 tencentcloud-sdk-python-ocr-3.0.882/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-26 03:39:55.000000 tencentcloud-sdk-python-ocr-3.0.882/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-26 03:39:55.000000 tencentcloud-sdk-python-ocr-3.0.882/setup.cfg
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.881/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ocr-3.0.882/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ocr
-Version: 3.0.881
+Version: 3.0.882
 Summary: Tencent Cloud Ocr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.881/README.rst` & `tencentcloud-sdk-python-ocr-3.0.882/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ocr-3.0.881/tencentcloud/ocr/v20181119/ocr_client.py` & `tencentcloud-sdk-python-ocr-3.0.882/tencentcloud/ocr/v20181119/ocr_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1551,15 +1551,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def RecognizePhilippinesSssIDOCR(self, request):
-        """菲律宾SSSID识别
+        """菲律宾SSSID/UMID识别
 
         :param request: Request instance for RecognizePhilippinesSssIDOCR.
         :type request: :class:`tencentcloud.ocr.v20181119.models.RecognizePhilippinesSssIDOCRRequest`
         :rtype: :class:`tencentcloud.ocr.v20181119.models.RecognizePhilippinesSssIDOCRResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.881/tencentcloud/ocr/v20181119/errorcodes.py` & `tencentcloud-sdk-python-ocr-3.0.882/tencentcloud/ocr/v20181119/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ocr-3.0.881/tencentcloud/ocr/v20181119/models.py` & `tencentcloud-sdk-python-ocr-3.0.882/tencentcloud/ocr/v20181119/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ocr-3.0.881/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ocr-3.0.882/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ocr-3.0.881/PKG-INFO` & `tencentcloud-sdk-python-ocr-3.0.882/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ocr
-Version: 3.0.881
+Version: 3.0.882
 Summary: Tencent Cloud Ocr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.881/setup.py` & `tencentcloud-sdk-python-ocr-3.0.882/setup.py`

 * *Files identical despite different names*

