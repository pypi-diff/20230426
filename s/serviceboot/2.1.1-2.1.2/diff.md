# Comparing `tmp/serviceboot-2.1.1.tar.gz` & `tmp/serviceboot-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/serviceboot-2.1.1.tar", last modified: Tue Apr  4 01:53:36 2023, max compression
+gzip compressed data, was "dist/serviceboot-2.1.2.tar", last modified: Wed Apr 26 02:56:32 2023, max compression
```

## Comparing `serviceboot-2.1.1.tar` & `serviceboot-2.1.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-04-04 01:53:36.000000 serviceboot-2.1.1/
--rw-rw-r--   0 hls       (1000) hls       (1000)     2579 2023-04-04 01:53:36.000000 serviceboot-2.1.1/PKG-INFO
--rw-rw-r--   0 hls       (1000) hls       (1000)     1395 2023-03-23 06:11:41.000000 serviceboot-2.1.1/README.md
-drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-04-04 01:53:36.000000 serviceboot-2.1.1/serviceboot/
--rw-rw-r--   0 hls       (1000) hls       (1000)        0 2022-11-15 06:17:47.000000 serviceboot-2.1.1/serviceboot/__init__.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     2764 2023-04-04 01:53:33.000000 serviceboot-2.1.1/serviceboot/build_docker.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     4167 2023-04-03 13:17:50.000000 serviceboot-2.1.1/serviceboot/build_zip.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     1376 2022-11-15 06:17:47.000000 serviceboot-2.1.1/serviceboot/command.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     4143 2022-11-15 06:17:47.000000 serviceboot-2.1.1/serviceboot/compile_python.py
--rw-rw-r--   0 hls       (1000) hls       (1000)      417 2022-11-15 06:17:47.000000 serviceboot-2.1.1/serviceboot/config_client.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     3010 2022-11-15 06:17:47.000000 serviceboot-2.1.1/serviceboot/consul_client.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     3171 2022-11-15 06:17:47.000000 serviceboot-2.1.1/serviceboot/oauth_client.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     2790 2022-11-15 06:17:47.000000 serviceboot-2.1.1/serviceboot/onboarding.py
--rw-rw-r--   0 hls       (1000) hls       (1000)      178 2022-11-15 06:17:47.000000 serviceboot-2.1.1/serviceboot/request_info.py
--rw-rw-r--   0 hls       (1000) hls       (1000)    21359 2023-03-23 06:11:41.000000 serviceboot-2.1.1/serviceboot/serviceboot.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     1144 2022-11-15 06:17:47.000000 serviceboot-2.1.1/serviceboot/token_service.py
-drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-04-04 01:53:36.000000 serviceboot-2.1.1/serviceboot.egg-info/
--rw-rw-r--   0 hls       (1000) hls       (1000)     2579 2023-04-04 01:53:35.000000 serviceboot-2.1.1/serviceboot.egg-info/PKG-INFO
--rw-rw-r--   0 hls       (1000) hls       (1000)      556 2023-04-04 01:53:36.000000 serviceboot-2.1.1/serviceboot.egg-info/SOURCES.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)        1 2023-04-04 01:53:35.000000 serviceboot-2.1.1/serviceboot.egg-info/dependency_links.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)       83 2023-04-04 01:53:35.000000 serviceboot-2.1.1/serviceboot.egg-info/entry_points.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)      101 2023-04-04 01:53:35.000000 serviceboot-2.1.1/serviceboot.egg-info/requires.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)       12 2023-04-04 01:53:35.000000 serviceboot-2.1.1/serviceboot.egg-info/top_level.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)       38 2023-04-04 01:53:36.000000 serviceboot-2.1.1/setup.cfg
--rw-rw-r--   0 hls       (1000) hls       (1000)     2446 2023-04-04 01:53:33.000000 serviceboot-2.1.1/setup.py
+drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-04-26 02:56:32.000000 serviceboot-2.1.2/
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2579 2023-04-26 02:56:32.000000 serviceboot-2.1.2/PKG-INFO
+-rw-rw-r--   0 hls       (1000) hls       (1000)     1395 2023-03-23 06:11:41.000000 serviceboot-2.1.2/README.md
+drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-04-26 02:56:32.000000 serviceboot-2.1.2/serviceboot/
+-rw-rw-r--   0 hls       (1000) hls       (1000)        0 2022-11-15 06:17:47.000000 serviceboot-2.1.2/serviceboot/__init__.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2764 2023-04-04 03:17:10.000000 serviceboot-2.1.2/serviceboot/build_docker.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     4167 2023-04-03 13:17:50.000000 serviceboot-2.1.2/serviceboot/build_zip.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     1376 2022-11-15 06:17:47.000000 serviceboot-2.1.2/serviceboot/command.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     4143 2022-11-15 06:17:47.000000 serviceboot-2.1.2/serviceboot/compile_python.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)      417 2022-11-15 06:17:47.000000 serviceboot-2.1.2/serviceboot/config_client.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     3010 2022-11-15 06:17:47.000000 serviceboot-2.1.2/serviceboot/consul_client.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     3171 2022-11-15 06:17:47.000000 serviceboot-2.1.2/serviceboot/oauth_client.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2790 2022-11-15 06:17:47.000000 serviceboot-2.1.2/serviceboot/onboarding.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)      178 2022-11-15 06:17:47.000000 serviceboot-2.1.2/serviceboot/request_info.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)    21359 2023-03-23 06:11:41.000000 serviceboot-2.1.2/serviceboot/serviceboot.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     1144 2022-11-15 06:17:47.000000 serviceboot-2.1.2/serviceboot/token_service.py
+drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-04-26 02:56:32.000000 serviceboot-2.1.2/serviceboot.egg-info/
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2579 2023-04-26 02:56:32.000000 serviceboot-2.1.2/serviceboot.egg-info/PKG-INFO
+-rw-rw-r--   0 hls       (1000) hls       (1000)      556 2023-04-26 02:56:32.000000 serviceboot-2.1.2/serviceboot.egg-info/SOURCES.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)        1 2023-04-26 02:56:32.000000 serviceboot-2.1.2/serviceboot.egg-info/dependency_links.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)       83 2023-04-26 02:56:32.000000 serviceboot-2.1.2/serviceboot.egg-info/entry_points.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)       93 2023-04-26 02:56:32.000000 serviceboot-2.1.2/serviceboot.egg-info/requires.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)       12 2023-04-26 02:56:32.000000 serviceboot-2.1.2/serviceboot.egg-info/top_level.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)       38 2023-04-26 02:56:32.000000 serviceboot-2.1.2/setup.cfg
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2438 2023-04-26 02:56:18.000000 serviceboot-2.1.2/setup.py
```

### Comparing `serviceboot-2.1.1/PKG-INFO` & `serviceboot-2.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serviceboot
-Version: 2.1.1
+Version: 2.1.2
 Summary: ServiceBoot云原生微服务引擎
 Home-page: https://openi.pcl.ac.cn/cubepy/serviceboot
 Author: cubeai
 Author-email: cubeai@163.com
 License: Apache License 2.0
 Description: # ServiceBoot云原生微服务引擎
```

### Comparing `serviceboot-2.1.1/README.md` & `serviceboot-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `serviceboot-2.1.1/serviceboot/build_docker.py` & `serviceboot-2.1.2/serviceboot/build_docker.py`

 * *Files identical despite different names*

### Comparing `serviceboot-2.1.1/serviceboot/build_zip.py` & `serviceboot-2.1.2/serviceboot/build_zip.py`

 * *Files identical despite different names*

### Comparing `serviceboot-2.1.1/serviceboot/command.py` & `serviceboot-2.1.2/serviceboot/command.py`

 * *Files identical despite different names*

### Comparing `serviceboot-2.1.1/serviceboot/compile_python.py` & `serviceboot-2.1.2/serviceboot/compile_python.py`

 * *Files identical despite different names*

### Comparing `serviceboot-2.1.1/serviceboot/consul_client.py` & `serviceboot-2.1.2/serviceboot/consul_client.py`

 * *Files identical despite different names*

### Comparing `serviceboot-2.1.1/serviceboot/oauth_client.py` & `serviceboot-2.1.2/serviceboot/oauth_client.py`

 * *Files identical despite different names*

### Comparing `serviceboot-2.1.1/serviceboot/onboarding.py` & `serviceboot-2.1.2/serviceboot/onboarding.py`

 * *Files identical despite different names*

### Comparing `serviceboot-2.1.1/serviceboot/serviceboot.py` & `serviceboot-2.1.2/serviceboot/serviceboot.py`

 * *Files identical despite different names*

### Comparing `serviceboot-2.1.1/serviceboot/token_service.py` & `serviceboot-2.1.2/serviceboot/token_service.py`

 * *Files identical despite different names*

### Comparing `serviceboot-2.1.1/serviceboot.egg-info/PKG-INFO` & `serviceboot-2.1.2/serviceboot.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serviceboot
-Version: 2.1.1
+Version: 2.1.2
 Summary: ServiceBoot云原生微服务引擎
 Home-page: https://openi.pcl.ac.cn/cubepy/serviceboot
 Author: cubeai
 Author-email: cubeai@163.com
 License: Apache License 2.0
 Description: # ServiceBoot云原生微服务引擎
```

### Comparing `serviceboot-2.1.1/serviceboot.egg-info/SOURCES.txt` & `serviceboot-2.1.2/serviceboot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `serviceboot-2.1.1/setup.py` & `serviceboot-2.1.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,25 +21,25 @@
 
 with open("README.md", "r", encoding='utf-8') as file:
     long_description = file.read()
 
 
 setup(
     name='serviceboot',
-    version='2.1.1',
+    version='2.1.2',
     author='cubeai',
     author_email='cubeai@163.com',
     description='ServiceBoot云原生微服务引擎',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='Apache License 2.0',
     packages=find_packages(),
     install_requires=[
         'cython==0.29.21',
-        'requests==2.24.0',
+        'requests',
         'tornado==6.0.4',
         'pyyaml==5.3.1',
         'python_jwt==3.2.6',
         'python-consul==1.1.0',
     ],
     classifiers=[
         'Development Status :: 4 - Beta',
```

