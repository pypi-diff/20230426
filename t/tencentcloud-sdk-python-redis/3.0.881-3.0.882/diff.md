# Comparing `tmp/tencentcloud-sdk-python-redis-3.0.881.tar.gz` & `tmp/tencentcloud-sdk-python-redis-3.0.882.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-redis-3.0.881.tar", last modified: Tue Apr 25 00:49:44 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-redis-3.0.882.tar", last modified: Wed Apr 26 03:43:55 2023, max compression
```

## Comparing `tencentcloud-sdk-python-redis-3.0.881.tar` & `tencentcloud-sdk-python-redis-3.0.882.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:49:44.000000 tencentcloud-sdk-python-redis-3.0.881/
--rw-r--r--   0 root         (0) root         (0)      743 2023-04-25 00:49:44.000000 tencentcloud-sdk-python-redis-3.0.881/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:49:44.000000 tencentcloud-sdk-python-redis-3.0.881/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:49:44.000000 tencentcloud-sdk-python-redis-3.0.881/tencentcloud/redis/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:49:44.000000 tencentcloud-sdk-python-redis-3.0.881/tencentcloud/redis/v20180412/
--rw-r--r--   0 root         (0) root         (0)    86631 2023-04-25 00:49:44.000000 tencentcloud-sdk-python-redis-3.0.881/tencentcloud/redis/v20180412/redis_client.py
--rw-r--r--   0 root         (0) root         (0)    12423 2023-04-25 00:49:44.000000 tencentcloud-sdk-python-redis-3.0.881/tencentcloud/redis/v20180412/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 00:49:44.000000 tencentcloud-sdk-python-redis-3.0.881/tencentcloud/redis/v20180412/__init__.py
--rw-r--r--   0 root         (0) root         (0)   291083 2023-04-25 00:49:44.000000 tencentcloud-sdk-python-redis-3.0.881/tencentcloud/redis/v20180412/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 00:49:44.000000 tencentcloud-sdk-python-redis-3.0.881/tencentcloud/redis/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-25 00:49:44.000000 tencentcloud-sdk-python-redis-3.0.881/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1669 2023-04-25 00:49:44.000000 tencentcloud-sdk-python-redis-3.0.881/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1010 2023-04-25 00:49:44.000000 tencentcloud-sdk-python-redis-3.0.881/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-25 00:49:44.000000 tencentcloud-sdk-python-redis-3.0.881/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:49:44.000000 tencentcloud-sdk-python-redis-3.0.881/tencentcloud_sdk_python_redis.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 00:49:44.000000 tencentcloud-sdk-python-redis-3.0.881/tencentcloud_sdk_python_redis.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      465 2023-04-25 00:49:44.000000 tencentcloud-sdk-python-redis-3.0.881/tencentcloud_sdk_python_redis.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-04-25 00:49:44.000000 tencentcloud-sdk-python-redis-3.0.881/tencentcloud_sdk_python_redis.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-25 00:49:44.000000 tencentcloud-sdk-python-redis-3.0.881/tencentcloud_sdk_python_redis.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:43:55.000000 tencentcloud-sdk-python-redis-3.0.882/
+-rw-r--r--   0 root         (0) root         (0)      743 2023-04-26 03:43:54.000000 tencentcloud-sdk-python-redis-3.0.882/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:43:55.000000 tencentcloud-sdk-python-redis-3.0.882/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:43:55.000000 tencentcloud-sdk-python-redis-3.0.882/tencentcloud/redis/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:43:55.000000 tencentcloud-sdk-python-redis-3.0.882/tencentcloud/redis/v20180412/
+-rw-r--r--   0 root         (0) root         (0)    86631 2023-04-26 03:43:54.000000 tencentcloud-sdk-python-redis-3.0.882/tencentcloud/redis/v20180412/redis_client.py
+-rw-r--r--   0 root         (0) root         (0)    12423 2023-04-26 03:43:54.000000 tencentcloud-sdk-python-redis-3.0.882/tencentcloud/redis/v20180412/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 03:43:54.000000 tencentcloud-sdk-python-redis-3.0.882/tencentcloud/redis/v20180412/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   291086 2023-04-26 03:43:54.000000 tencentcloud-sdk-python-redis-3.0.882/tencentcloud/redis/v20180412/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 03:43:55.000000 tencentcloud-sdk-python-redis-3.0.882/tencentcloud/redis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-26 03:43:54.000000 tencentcloud-sdk-python-redis-3.0.882/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-04-26 03:43:55.000000 tencentcloud-sdk-python-redis-3.0.882/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-04-26 03:43:54.000000 tencentcloud-sdk-python-redis-3.0.882/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-26 03:43:55.000000 tencentcloud-sdk-python-redis-3.0.882/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:43:55.000000 tencentcloud-sdk-python-redis-3.0.882/tencentcloud_sdk_python_redis.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 03:43:55.000000 tencentcloud-sdk-python-redis-3.0.882/tencentcloud_sdk_python_redis.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      465 2023-04-26 03:43:55.000000 tencentcloud-sdk-python-redis-3.0.882/tencentcloud_sdk_python_redis.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-04-26 03:43:55.000000 tencentcloud-sdk-python-redis-3.0.882/tencentcloud_sdk_python_redis.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-26 03:43:55.000000 tencentcloud-sdk-python-redis-3.0.882/tencentcloud_sdk_python_redis.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-redis-3.0.881/README.rst` & `tencentcloud-sdk-python-redis-3.0.882/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-redis-3.0.881/tencentcloud/redis/v20180412/redis_client.py` & `tencentcloud-sdk-python-redis-3.0.882/tencentcloud/redis/v20180412/redis_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-redis-3.0.881/tencentcloud/redis/v20180412/errorcodes.py` & `tencentcloud-sdk-python-redis-3.0.882/tencentcloud/redis/v20180412/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-redis-3.0.881/tencentcloud/redis/v20180412/models.py` & `tencentcloud-sdk-python-redis-3.0.882/tencentcloud/redis/v20180412/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -6845,33 +6845,30 @@
 
     """
 
     def __init__(self):
         r"""
         :param StartTime: 备份开始时间。
         :type StartTime: str
-        :param BackupId: 备份ID。
+        :param BackupId: 备份任务ID。
         :type BackupId: str
         :param BackupType: 备份类型。
-
-- 1：用户发起的手动备份。
-- 0：凌晨系统发起的备份。
+- 1：凌晨系统发起的备份。
+- 0：用户发起的手动备份。
         :type BackupType: str
         :param Status: 备份状态。 
-
 - 1：备份被其它流程锁定。
 - 2：备份正常，没有被任何流程锁定。
 - -1：备份已过期。
 - 3：备份正在被导出。
 - 4：备份导出成功。
         :type Status: int
         :param Remark: 备份的备注信息。
         :type Remark: str
         :param Locked: 备份是否被锁定。
-
 - 0：未被锁定。
 - 1：已被锁定。
         :type Locked: int
         :param BackupSize: 内部字段，用户可忽略。
 注意：此字段可能返回 null，表示取不到有效值。
         :type BackupSize: int
         :param FullBackup: 内部字段，用户可忽略。
```

### Comparing `tencentcloud-sdk-python-redis-3.0.881/tencentcloud/__init__.py` & `tencentcloud-sdk-python-redis-3.0.882/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-redis-3.0.881/PKG-INFO` & `tencentcloud-sdk-python-redis-3.0.882/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-redis
-Version: 3.0.881
+Version: 3.0.882
 Summary: Tencent Cloud Redis SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-redis-3.0.881/setup.py` & `tencentcloud-sdk-python-redis-3.0.882/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-redis-3.0.881/tencentcloud_sdk_python_redis.egg-info/PKG-INFO` & `tencentcloud-sdk-python-redis-3.0.882/tencentcloud_sdk_python_redis.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-redis
-Version: 3.0.881
+Version: 3.0.882
 Summary: Tencent Cloud Redis SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

