# Comparing `tmp/pystools-0.0.7.tar.gz` & `tmp/pystools-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pystools-0.0.7.tar", last modified: Wed Apr 26 08:53:36 2023, max compression
+gzip compressed data, was "pystools-0.0.8.tar", last modified: Wed Apr 26 09:04:53 2023, max compression
```

## Comparing `pystools-0.0.7.tar` & `pystools-0.0.8.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-26 08:53:36.138898 pystools-0.0.7/
--rw-r--r--   0 steve      (501) staff       (20)        0 2023-04-16 08:21:09.000000 pystools-0.0.7/LICENSE
--rw-r--r--   0 steve      (501) staff       (20)      583 2023-04-26 08:53:36.138532 pystools-0.0.7/PKG-INFO
--rw-r--r--   0 steve      (501) staff       (20)      106 2023-04-26 05:41:53.000000 pystools-0.0.7/README.md
--rw-r--r--   0 steve      (501) staff       (20)      602 2023-04-26 08:53:16.000000 pystools-0.0.7/pyproject.toml
--rw-r--r--   0 steve      (501) staff       (20)       38 2023-04-26 08:53:36.139006 pystools-0.0.7/setup.cfg
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-26 08:53:36.123659 pystools-0.0.7/src/
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-26 08:53:36.127034 pystools-0.0.7/src/PysTools.egg-info/
--rw-r--r--   0 steve      (501) staff       (20)      583 2023-04-26 08:53:36.000000 pystools-0.0.7/src/PysTools.egg-info/PKG-INFO
--rw-r--r--   0 steve      (501) staff       (20)      709 2023-04-26 08:53:36.000000 pystools-0.0.7/src/PysTools.egg-info/SOURCES.txt
--rw-r--r--   0 steve      (501) staff       (20)        1 2023-04-26 08:53:36.000000 pystools-0.0.7/src/PysTools.egg-info/dependency_links.txt
--rw-r--r--   0 steve      (501) staff       (20)       38 2023-04-26 08:53:36.000000 pystools-0.0.7/src/PysTools.egg-info/requires.txt
--rw-r--r--   0 steve      (501) staff       (20)       18 2023-04-26 08:53:36.000000 pystools-0.0.7/src/PysTools.egg-info/top_level.txt
--rw-r--r--   0 steve      (501) staff       (20)        2 2023-04-26 03:57:58.000000 pystools-0.0.7/src/__init__.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-26 08:53:36.136386 pystools-0.0.7/src/pystools/
--rw-r--r--   0 steve      (501) staff       (20)     1278 2023-04-26 04:59:47.000000 pystools-0.0.7/src/pystools/BizResponse.py
--rw-r--r--   0 steve      (501) staff       (20)      537 2023-04-26 04:59:15.000000 pystools-0.0.7/src/pystools/BizResponseCode.py
--rwxr-xr-x   0 steve      (501) staff       (20)    27698 2023-04-26 08:53:10.000000 pystools-0.0.7/src/pystools/Feishu.py
--rw-r--r--   0 steve      (501) staff       (20)     1454 2023-04-26 05:07:11.000000 pystools-0.0.7/src/pystools/Jwt.py
--rw-r--r--   0 steve      (501) staff       (20)     1876 2023-04-26 05:34:33.000000 pystools-0.0.7/src/pystools/LexinSms.py
--rw-r--r--   0 steve      (501) staff       (20)     1535 2023-04-25 17:01:25.000000 pystools-0.0.7/src/pystools/Logger.py
--rw-r--r--   0 steve      (501) staff       (20)      259 2023-04-26 05:25:35.000000 pystools-0.0.7/src/pystools/MD5util.py
--rw-r--r--   0 steve      (501) staff       (20)     4013 2023-04-26 06:12:55.000000 pystools-0.0.7/src/pystools/TencentCos.py
--rwxr-xr-x   0 steve      (501) staff       (20)     5183 2023-04-26 07:17:47.000000 pystools-0.0.7/src/pystools/Xiumi.py
--rw-r--r--   0 steve      (501) staff       (20)        0 2023-04-26 03:57:35.000000 pystools-0.0.7/src/pystools/__init__.py
--rw-r--r--   0 steve      (501) staff       (20)       42 2023-04-16 08:20:17.000000 pystools-0.0.7/src/pystools/example.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-26 08:53:36.137899 pystools-0.0.7/src/pystools/test/
--rw-r--r--   0 steve      (501) staff       (20)        0 2023-04-26 04:53:20.000000 pystools-0.0.7/src/pystools/test/__init__.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-26 09:04:53.473257 pystools-0.0.8/
+-rw-r--r--   0 steve      (501) staff       (20)        0 2023-04-16 08:21:09.000000 pystools-0.0.8/LICENSE
+-rw-r--r--   0 steve      (501) staff       (20)      583 2023-04-26 09:04:53.471766 pystools-0.0.8/PKG-INFO
+-rw-r--r--   0 steve      (501) staff       (20)      106 2023-04-26 05:41:53.000000 pystools-0.0.8/README.md
+-rw-r--r--   0 steve      (501) staff       (20)      602 2023-04-26 09:04:32.000000 pystools-0.0.8/pyproject.toml
+-rw-r--r--   0 steve      (501) staff       (20)       38 2023-04-26 09:04:53.473528 pystools-0.0.8/setup.cfg
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-26 09:04:53.457816 pystools-0.0.8/src/
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-26 09:04:53.460207 pystools-0.0.8/src/PysTools.egg-info/
+-rw-r--r--   0 steve      (501) staff       (20)      583 2023-04-26 09:04:53.000000 pystools-0.0.8/src/PysTools.egg-info/PKG-INFO
+-rw-r--r--   0 steve      (501) staff       (20)      709 2023-04-26 09:04:53.000000 pystools-0.0.8/src/PysTools.egg-info/SOURCES.txt
+-rw-r--r--   0 steve      (501) staff       (20)        1 2023-04-26 09:04:53.000000 pystools-0.0.8/src/PysTools.egg-info/dependency_links.txt
+-rw-r--r--   0 steve      (501) staff       (20)       38 2023-04-26 09:04:53.000000 pystools-0.0.8/src/PysTools.egg-info/requires.txt
+-rw-r--r--   0 steve      (501) staff       (20)       18 2023-04-26 09:04:53.000000 pystools-0.0.8/src/PysTools.egg-info/top_level.txt
+-rw-r--r--   0 steve      (501) staff       (20)        2 2023-04-26 03:57:58.000000 pystools-0.0.8/src/__init__.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-26 09:04:53.468411 pystools-0.0.8/src/pystools/
+-rw-r--r--   0 steve      (501) staff       (20)     1278 2023-04-26 04:59:47.000000 pystools-0.0.8/src/pystools/BizResponse.py
+-rw-r--r--   0 steve      (501) staff       (20)      537 2023-04-26 04:59:15.000000 pystools-0.0.8/src/pystools/BizResponseCode.py
+-rwxr-xr-x   0 steve      (501) staff       (20)    28074 2023-04-26 09:03:30.000000 pystools-0.0.8/src/pystools/Feishu.py
+-rw-r--r--   0 steve      (501) staff       (20)     1454 2023-04-26 05:07:11.000000 pystools-0.0.8/src/pystools/Jwt.py
+-rw-r--r--   0 steve      (501) staff       (20)     1876 2023-04-26 05:34:33.000000 pystools-0.0.8/src/pystools/LexinSms.py
+-rw-r--r--   0 steve      (501) staff       (20)     1535 2023-04-25 17:01:25.000000 pystools-0.0.8/src/pystools/Logger.py
+-rw-r--r--   0 steve      (501) staff       (20)      259 2023-04-26 05:25:35.000000 pystools-0.0.8/src/pystools/MD5util.py
+-rw-r--r--   0 steve      (501) staff       (20)     4013 2023-04-26 06:12:55.000000 pystools-0.0.8/src/pystools/TencentCos.py
+-rwxr-xr-x   0 steve      (501) staff       (20)     5183 2023-04-26 07:17:47.000000 pystools-0.0.8/src/pystools/Xiumi.py
+-rw-r--r--   0 steve      (501) staff       (20)        0 2023-04-26 03:57:35.000000 pystools-0.0.8/src/pystools/__init__.py
+-rw-r--r--   0 steve      (501) staff       (20)       42 2023-04-16 08:20:17.000000 pystools-0.0.8/src/pystools/example.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-26 09:04:53.470422 pystools-0.0.8/src/pystools/test/
+-rw-r--r--   0 steve      (501) staff       (20)        0 2023-04-26 04:53:20.000000 pystools-0.0.8/src/pystools/test/__init__.py
```

### Comparing `pystools-0.0.7/PKG-INFO` & `pystools-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystools
-Version: 0.0.7
+Version: 0.0.8
 Summary: pystools
 Author-email: 木坦坦 <devzhao@126.com>
 Project-URL: Homepage, https://github.com/devzhaohan/HMTools
 Project-URL: Bug Tracker, https://github.com/devzhaohan/HMTools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pystools-0.0.7/pyproject.toml` & `pystools-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pystools"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="木坦坦", email="devzhao@126.com" },
 ]
 description = "pystools"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pystools-0.0.7/src/PysTools.egg-info/PKG-INFO` & `pystools-0.0.8/src/PysTools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystools
-Version: 0.0.7
+Version: 0.0.8
 Summary: pystools
 Author-email: 木坦坦 <devzhao@126.com>
 Project-URL: Homepage, https://github.com/devzhaohan/HMTools
 Project-URL: Bug Tracker, https://github.com/devzhaohan/HMTools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pystools-0.0.7/src/PysTools.egg-info/SOURCES.txt` & `pystools-0.0.8/src/PysTools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pystools-0.0.7/src/pystools/BizResponse.py` & `pystools-0.0.8/src/pystools/BizResponse.py`

 * *Files identical despite different names*

### Comparing `pystools-0.0.7/src/pystools/BizResponseCode.py` & `pystools-0.0.8/src/pystools/BizResponseCode.py`

 * *Files identical despite different names*

### Comparing `pystools-0.0.7/src/pystools/Feishu.py` & `pystools-0.0.8/src/pystools/Feishu.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 # 获取协作者列表
 DRIVE_PERMISSIONS_MEMBERS = '/open-apis/drive/v1/permissions/:token/members'
 
 BITABLE_RECORDS = "/open-apis/bitable/v1/apps/:app_token/tables/:table_id/records"
 
 # 删除记录
-BITABLE_RECORDS_DELETE = "/open-apis/bitable/v1/apps/:app_token/tables/:table_id/records/:record_id"
+BITABLE_RECORD = "/open-apis/bitable/v1/apps/:app_token/tables/:table_id/records/:record_id"
 
 # 下载素材
 MEDIAS_DOWNLOAD = "/open-apis/drive/v1/medias/:file_token/download"
 # 获取素材临时下载链接
 MEDIAS_BATCH_GET_TMP_DOWNLOAD_URL = "/open-apis/drive/v1/medias/batch_get_tmp_download_url"
 
 # 云文档/下载文件
@@ -269,21 +269,30 @@
         resp = self.req_feishu_api(action, url=url, req_body=req_body)
         return resp.get("data")
 
 
     def bitable_record_delete(self, file_token, table_id, record_id):
         self._authorize_tenant_access_token()
         url = "{}{}".format(
-            lark_host, BITABLE_RECORDS_DELETE
+            lark_host, BITABLE_RECORD
         ).replace(":app_token", file_token).replace(":table_id", table_id).replace(":record_id", record_id)
         action = "DELETE"
         resp = self.req_feishu_api(action, url=url)
         return resp.get("data")
 
 
+    def bitable_record(self, file_token, table_id, record_id):
+        self._authorize_tenant_access_token()
+        url = "{}{}".format(
+            lark_host, BITABLE_RECORD
+        ).replace(":app_token", file_token).replace(":table_id", table_id).replace(":record_id", record_id)
+        action = "GET"
+        resp = self.req_feishu_api(action, url=url)
+        return resp.get("data")
+
     def medias_download(self, file_token, param={}):
         file_res = self.medias_download_to_bytes(file_token, param={})
         file_bytes = file_res.get("file_bytes")
 
         subfix = file_res.get("content_type").split("/")[1]
         filename = file_token + "." + subfix
```

### Comparing `pystools-0.0.7/src/pystools/Jwt.py` & `pystools-0.0.8/src/pystools/Jwt.py`

 * *Files identical despite different names*

### Comparing `pystools-0.0.7/src/pystools/LexinSms.py` & `pystools-0.0.8/src/pystools/LexinSms.py`

 * *Files identical despite different names*

### Comparing `pystools-0.0.7/src/pystools/Logger.py` & `pystools-0.0.8/src/pystools/Logger.py`

 * *Files identical despite different names*

### Comparing `pystools-0.0.7/src/pystools/TencentCos.py` & `pystools-0.0.8/src/pystools/TencentCos.py`

 * *Files identical despite different names*

### Comparing `pystools-0.0.7/src/pystools/Xiumi.py` & `pystools-0.0.8/src/pystools/Xiumi.py`

 * *Files identical despite different names*

