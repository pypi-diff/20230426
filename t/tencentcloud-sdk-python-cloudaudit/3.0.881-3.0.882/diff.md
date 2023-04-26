# Comparing `tmp/tencentcloud-sdk-python-cloudaudit-3.0.881.tar.gz` & `tmp/tencentcloud-sdk-python-cloudaudit-3.0.882.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cloudaudit-3.0.881.tar", last modified: Tue Apr 25 00:30:15 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cloudaudit-3.0.882.tar", last modified: Wed Apr 26 03:08:04 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cloudaudit-3.0.881.tar` & `tencentcloud-sdk-python-cloudaudit-3.0.882.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:30:15.000000 tencentcloud-sdk-python-cloudaudit-3.0.881/
--rw-r--r--   0 root         (0) root         (0)      758 2023-04-25 00:30:15.000000 tencentcloud-sdk-python-cloudaudit-3.0.881/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:30:15.000000 tencentcloud-sdk-python-cloudaudit-3.0.881/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:30:15.000000 tencentcloud-sdk-python-cloudaudit-3.0.881/tencentcloud/cloudaudit/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:30:15.000000 tencentcloud-sdk-python-cloudaudit-3.0.881/tencentcloud/cloudaudit/v20190319/
--rw-r--r--   0 root         (0) root         (0)    18502 2023-04-25 00:30:15.000000 tencentcloud-sdk-python-cloudaudit-3.0.881/tencentcloud/cloudaudit/v20190319/cloudaudit_client.py
--rw-r--r--   0 root         (0) root         (0)     6753 2023-04-25 00:30:15.000000 tencentcloud-sdk-python-cloudaudit-3.0.881/tencentcloud/cloudaudit/v20190319/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 00:30:15.000000 tencentcloud-sdk-python-cloudaudit-3.0.881/tencentcloud/cloudaudit/v20190319/__init__.py
--rw-r--r--   0 root         (0) root         (0)    57444 2023-04-25 00:30:15.000000 tencentcloud-sdk-python-cloudaudit-3.0.881/tencentcloud/cloudaudit/v20190319/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 00:30:15.000000 tencentcloud-sdk-python-cloudaudit-3.0.881/tencentcloud/cloudaudit/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-25 00:30:15.000000 tencentcloud-sdk-python-cloudaudit-3.0.881/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1694 2023-04-25 00:30:15.000000 tencentcloud-sdk-python-cloudaudit-3.0.881/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1020 2023-04-25 00:30:15.000000 tencentcloud-sdk-python-cloudaudit-3.0.881/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-25 00:30:15.000000 tencentcloud-sdk-python-cloudaudit-3.0.881/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:30:15.000000 tencentcloud-sdk-python-cloudaudit-3.0.881/tencentcloud_sdk_python_cloudaudit.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 00:30:15.000000 tencentcloud-sdk-python-cloudaudit-3.0.881/tencentcloud_sdk_python_cloudaudit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      515 2023-04-25 00:30:15.000000 tencentcloud-sdk-python-cloudaudit-3.0.881/tencentcloud_sdk_python_cloudaudit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1694 2023-04-25 00:30:15.000000 tencentcloud-sdk-python-cloudaudit-3.0.881/tencentcloud_sdk_python_cloudaudit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-25 00:30:15.000000 tencentcloud-sdk-python-cloudaudit-3.0.881/tencentcloud_sdk_python_cloudaudit.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:08:04.000000 tencentcloud-sdk-python-cloudaudit-3.0.882/
+-rw-r--r--   0 root         (0) root         (0)      758 2023-04-26 03:08:04.000000 tencentcloud-sdk-python-cloudaudit-3.0.882/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:08:04.000000 tencentcloud-sdk-python-cloudaudit-3.0.882/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:08:04.000000 tencentcloud-sdk-python-cloudaudit-3.0.882/tencentcloud/cloudaudit/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:08:04.000000 tencentcloud-sdk-python-cloudaudit-3.0.882/tencentcloud/cloudaudit/v20190319/
+-rw-r--r--   0 root         (0) root         (0)    18502 2023-04-26 03:08:04.000000 tencentcloud-sdk-python-cloudaudit-3.0.882/tencentcloud/cloudaudit/v20190319/cloudaudit_client.py
+-rw-r--r--   0 root         (0) root         (0)     6753 2023-04-26 03:08:04.000000 tencentcloud-sdk-python-cloudaudit-3.0.882/tencentcloud/cloudaudit/v20190319/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 03:08:04.000000 tencentcloud-sdk-python-cloudaudit-3.0.882/tencentcloud/cloudaudit/v20190319/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    57444 2023-04-26 03:08:04.000000 tencentcloud-sdk-python-cloudaudit-3.0.882/tencentcloud/cloudaudit/v20190319/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 03:08:04.000000 tencentcloud-sdk-python-cloudaudit-3.0.882/tencentcloud/cloudaudit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-26 03:08:04.000000 tencentcloud-sdk-python-cloudaudit-3.0.882/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-04-26 03:08:04.000000 tencentcloud-sdk-python-cloudaudit-3.0.882/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-04-26 03:08:04.000000 tencentcloud-sdk-python-cloudaudit-3.0.882/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-26 03:08:04.000000 tencentcloud-sdk-python-cloudaudit-3.0.882/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:08:04.000000 tencentcloud-sdk-python-cloudaudit-3.0.882/tencentcloud_sdk_python_cloudaudit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 03:08:04.000000 tencentcloud-sdk-python-cloudaudit-3.0.882/tencentcloud_sdk_python_cloudaudit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      515 2023-04-26 03:08:04.000000 tencentcloud-sdk-python-cloudaudit-3.0.882/tencentcloud_sdk_python_cloudaudit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-04-26 03:08:04.000000 tencentcloud-sdk-python-cloudaudit-3.0.882/tencentcloud_sdk_python_cloudaudit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-26 03:08:04.000000 tencentcloud-sdk-python-cloudaudit-3.0.882/tencentcloud_sdk_python_cloudaudit.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-cloudaudit-3.0.881/README.rst` & `tencentcloud-sdk-python-cloudaudit-3.0.882/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cloudaudit-3.0.881/tencentcloud/cloudaudit/v20190319/cloudaudit_client.py` & `tencentcloud-sdk-python-cloudaudit-3.0.882/tencentcloud/cloudaudit/v20190319/cloudaudit_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cloudaudit-3.0.881/tencentcloud/cloudaudit/v20190319/errorcodes.py` & `tencentcloud-sdk-python-cloudaudit-3.0.882/tencentcloud/cloudaudit/v20190319/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cloudaudit-3.0.881/tencentcloud/cloudaudit/v20190319/models.py` & `tencentcloud-sdk-python-cloudaudit-3.0.882/tencentcloud/cloudaudit/v20190319/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cloudaudit-3.0.881/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cloudaudit-3.0.882/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cloudaudit-3.0.881/PKG-INFO` & `tencentcloud-sdk-python-cloudaudit-3.0.882/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cloudaudit
-Version: 3.0.881
+Version: 3.0.882
 Summary: Tencent Cloud Cloudaudit SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cloudaudit-3.0.881/setup.py` & `tencentcloud-sdk-python-cloudaudit-3.0.882/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cloudaudit-3.0.881/tencentcloud_sdk_python_cloudaudit.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-cloudaudit-3.0.882/tencentcloud_sdk_python_cloudaudit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cloudaudit-3.0.881/tencentcloud_sdk_python_cloudaudit.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cloudaudit-3.0.882/tencentcloud_sdk_python_cloudaudit.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cloudaudit
-Version: 3.0.881
+Version: 3.0.882
 Summary: Tencent Cloud Cloudaudit SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```
