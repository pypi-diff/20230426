# Comparing `tmp/tencentcloud-sdk-python-mongodb-3.0.881.tar.gz` & `tmp/tencentcloud-sdk-python-mongodb-3.0.882.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-mongodb-3.0.881.tar", last modified: Tue Apr 25 00:45:20 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-mongodb-3.0.882.tar", last modified: Wed Apr 26 03:38:50 2023, max compression
```

## Comparing `tencentcloud-sdk-python-mongodb-3.0.881.tar` & `tencentcloud-sdk-python-mongodb-3.0.882.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:45:20.000000 tencentcloud-sdk-python-mongodb-3.0.881/
--rw-r--r--   0 root         (0) root         (0)      749 2023-04-25 00:45:20.000000 tencentcloud-sdk-python-mongodb-3.0.881/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:45:20.000000 tencentcloud-sdk-python-mongodb-3.0.881/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:45:20.000000 tencentcloud-sdk-python-mongodb-3.0.881/tencentcloud/mongodb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:45:20.000000 tencentcloud-sdk-python-mongodb-3.0.881/tencentcloud/mongodb/v20180408/
--rw-r--r--   0 root         (0) root         (0)    13571 2023-04-25 00:45:20.000000 tencentcloud-sdk-python-mongodb-3.0.881/tencentcloud/mongodb/v20180408/mongodb_client.py
--rw-r--r--   0 root         (0) root         (0)     3903 2023-04-25 00:45:20.000000 tencentcloud-sdk-python-mongodb-3.0.881/tencentcloud/mongodb/v20180408/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 00:45:20.000000 tencentcloud-sdk-python-mongodb-3.0.881/tencentcloud/mongodb/v20180408/__init__.py
--rw-r--r--   0 root         (0) root         (0)    46677 2023-04-25 00:45:20.000000 tencentcloud-sdk-python-mongodb-3.0.881/tencentcloud/mongodb/v20180408/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:45:20.000000 tencentcloud-sdk-python-mongodb-3.0.881/tencentcloud/mongodb/v20190725/
--rw-r--r--   0 root         (0) root         (0)    36443 2023-04-25 00:45:20.000000 tencentcloud-sdk-python-mongodb-3.0.881/tencentcloud/mongodb/v20190725/mongodb_client.py
--rw-r--r--   0 root         (0) root         (0)     7304 2023-04-25 00:45:20.000000 tencentcloud-sdk-python-mongodb-3.0.881/tencentcloud/mongodb/v20190725/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 00:45:20.000000 tencentcloud-sdk-python-mongodb-3.0.881/tencentcloud/mongodb/v20190725/__init__.py
--rw-r--r--   0 root         (0) root         (0)   149931 2023-04-25 00:45:20.000000 tencentcloud-sdk-python-mongodb-3.0.881/tencentcloud/mongodb/v20190725/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 00:45:20.000000 tencentcloud-sdk-python-mongodb-3.0.881/tencentcloud/mongodb/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-25 00:45:20.000000 tencentcloud-sdk-python-mongodb-3.0.881/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:45:20.000000 tencentcloud-sdk-python-mongodb-3.0.881/tencentcloud_sdk_python_mongodb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 00:45:20.000000 tencentcloud-sdk-python-mongodb-3.0.881/tencentcloud_sdk_python_mongodb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      663 2023-04-25 00:45:20.000000 tencentcloud-sdk-python-mongodb-3.0.881/tencentcloud_sdk_python_mongodb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-04-25 00:45:20.000000 tencentcloud-sdk-python-mongodb-3.0.881/tencentcloud_sdk_python_mongodb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-25 00:45:20.000000 tencentcloud-sdk-python-mongodb-3.0.881/tencentcloud_sdk_python_mongodb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-04-25 00:45:20.000000 tencentcloud-sdk-python-mongodb-3.0.881/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1014 2023-04-25 00:45:20.000000 tencentcloud-sdk-python-mongodb-3.0.881/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-25 00:45:20.000000 tencentcloud-sdk-python-mongodb-3.0.881/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:38:50.000000 tencentcloud-sdk-python-mongodb-3.0.882/
+-rw-r--r--   0 root         (0) root         (0)      749 2023-04-26 03:38:50.000000 tencentcloud-sdk-python-mongodb-3.0.882/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:38:50.000000 tencentcloud-sdk-python-mongodb-3.0.882/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:38:50.000000 tencentcloud-sdk-python-mongodb-3.0.882/tencentcloud/mongodb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:38:50.000000 tencentcloud-sdk-python-mongodb-3.0.882/tencentcloud/mongodb/v20180408/
+-rw-r--r--   0 root         (0) root         (0)    13571 2023-04-26 03:38:50.000000 tencentcloud-sdk-python-mongodb-3.0.882/tencentcloud/mongodb/v20180408/mongodb_client.py
+-rw-r--r--   0 root         (0) root         (0)     3903 2023-04-26 03:38:50.000000 tencentcloud-sdk-python-mongodb-3.0.882/tencentcloud/mongodb/v20180408/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 03:38:50.000000 tencentcloud-sdk-python-mongodb-3.0.882/tencentcloud/mongodb/v20180408/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    46677 2023-04-26 03:38:50.000000 tencentcloud-sdk-python-mongodb-3.0.882/tencentcloud/mongodb/v20180408/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:38:50.000000 tencentcloud-sdk-python-mongodb-3.0.882/tencentcloud/mongodb/v20190725/
+-rw-r--r--   0 root         (0) root         (0)    36443 2023-04-26 03:38:50.000000 tencentcloud-sdk-python-mongodb-3.0.882/tencentcloud/mongodb/v20190725/mongodb_client.py
+-rw-r--r--   0 root         (0) root         (0)     7304 2023-04-26 03:38:50.000000 tencentcloud-sdk-python-mongodb-3.0.882/tencentcloud/mongodb/v20190725/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 03:38:50.000000 tencentcloud-sdk-python-mongodb-3.0.882/tencentcloud/mongodb/v20190725/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   149931 2023-04-26 03:38:50.000000 tencentcloud-sdk-python-mongodb-3.0.882/tencentcloud/mongodb/v20190725/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 03:38:50.000000 tencentcloud-sdk-python-mongodb-3.0.882/tencentcloud/mongodb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-26 03:38:50.000000 tencentcloud-sdk-python-mongodb-3.0.882/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:38:50.000000 tencentcloud-sdk-python-mongodb-3.0.882/tencentcloud_sdk_python_mongodb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 03:38:50.000000 tencentcloud-sdk-python-mongodb-3.0.882/tencentcloud_sdk_python_mongodb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      663 2023-04-26 03:38:50.000000 tencentcloud-sdk-python-mongodb-3.0.882/tencentcloud_sdk_python_mongodb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-04-26 03:38:50.000000 tencentcloud-sdk-python-mongodb-3.0.882/tencentcloud_sdk_python_mongodb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-26 03:38:50.000000 tencentcloud-sdk-python-mongodb-3.0.882/tencentcloud_sdk_python_mongodb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-04-26 03:38:50.000000 tencentcloud-sdk-python-mongodb-3.0.882/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-04-26 03:38:50.000000 tencentcloud-sdk-python-mongodb-3.0.882/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-26 03:38:50.000000 tencentcloud-sdk-python-mongodb-3.0.882/setup.cfg
```

### Comparing `tencentcloud-sdk-python-mongodb-3.0.881/README.rst` & `tencentcloud-sdk-python-mongodb-3.0.882/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mongodb-3.0.881/tencentcloud/mongodb/v20180408/mongodb_client.py` & `tencentcloud-sdk-python-mongodb-3.0.882/tencentcloud/mongodb/v20180408/mongodb_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mongodb-3.0.881/tencentcloud/mongodb/v20180408/errorcodes.py` & `tencentcloud-sdk-python-mongodb-3.0.882/tencentcloud/mongodb/v20180408/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mongodb-3.0.881/tencentcloud/mongodb/v20180408/models.py` & `tencentcloud-sdk-python-mongodb-3.0.882/tencentcloud/mongodb/v20180408/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mongodb-3.0.881/tencentcloud/mongodb/v20190725/mongodb_client.py` & `tencentcloud-sdk-python-mongodb-3.0.882/tencentcloud/mongodb/v20190725/mongodb_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mongodb-3.0.881/tencentcloud/mongodb/v20190725/errorcodes.py` & `tencentcloud-sdk-python-mongodb-3.0.882/tencentcloud/mongodb/v20190725/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mongodb-3.0.881/tencentcloud/mongodb/v20190725/models.py` & `tencentcloud-sdk-python-mongodb-3.0.882/tencentcloud/mongodb/v20190725/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mongodb-3.0.881/tencentcloud/__init__.py` & `tencentcloud-sdk-python-mongodb-3.0.882/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-mongodb-3.0.881/tencentcloud_sdk_python_mongodb.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-mongodb-3.0.882/tencentcloud_sdk_python_mongodb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mongodb-3.0.881/tencentcloud_sdk_python_mongodb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-mongodb-3.0.882/tencentcloud_sdk_python_mongodb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-mongodb
-Version: 3.0.881
+Version: 3.0.882
 Summary: Tencent Cloud Mongodb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-mongodb-3.0.881/PKG-INFO` & `tencentcloud-sdk-python-mongodb-3.0.882/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-mongodb
-Version: 3.0.881
+Version: 3.0.882
 Summary: Tencent Cloud Mongodb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-mongodb-3.0.881/setup.py` & `tencentcloud-sdk-python-mongodb-3.0.882/setup.py`

 * *Files identical despite different names*

