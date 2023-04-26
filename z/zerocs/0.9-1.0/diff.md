# Comparing `tmp/zerocs-0.9.tar.gz` & `tmp/zerocs-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zerocs-0.9.tar", last modified: Wed Apr 26 13:46:46 2023, max compression
+gzip compressed data, was "zerocs-1.0.tar", last modified: Wed Apr 26 15:18:07 2023, max compression
```

## Comparing `zerocs-0.9.tar` & `zerocs-1.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-26 13:46:46.486051 zerocs-0.9/
--rw-r--r--   0 yanping   (1000) yanping   (1000)    18156 2023-04-26 13:46:46.486051 zerocs-0.9/PKG-INFO
--rw-r--r--   0 yanping   (1000) yanping   (1000)       38 2023-04-26 13:46:46.486051 zerocs-0.9/setup.cfg
--rw-r--r--   0 yanping   (1000) yanping   (1000)      867 2023-04-26 13:46:41.000000 zerocs-0.9/setup.py
-drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-26 13:46:46.486051 zerocs-0.9/zerocs/
--rw-r--r--   0 yanping   (1000) yanping   (1000)     4785 2023-04-22 02:58:49.000000 zerocs-0.9/zerocs/__init__.py
-drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-26 13:46:46.486051 zerocs-0.9/zerocs/base/
--rw-r--r--   0 yanping   (1000) yanping   (1000)      134 2023-04-20 04:53:25.000000 zerocs-0.9/zerocs/base/__init__.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)     1845 2023-04-20 04:53:25.000000 zerocs-0.9/zerocs/base/_base.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)     7208 2023-04-26 13:20:00.000000 zerocs-0.9/zerocs/base/_default_func.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)      496 2023-04-20 04:53:25.000000 zerocs-0.9/zerocs/base/_function.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)     2674 2023-04-19 11:33:05.000000 zerocs-0.9/zerocs/base/base_.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)      529 2023-04-26 13:20:00.000000 zerocs-0.9/zerocs/base/default_func_.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)      670 2023-04-19 11:33:05.000000 zerocs-0.9/zerocs/base/function_.py
-drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-26 13:46:46.486051 zerocs-0.9/zerocs/fork/
--rw-r--r--   0 yanping   (1000) yanping   (1000)       35 2023-04-20 04:53:25.000000 zerocs-0.9/zerocs/fork/__init__.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)     1993 2023-04-22 03:18:59.000000 zerocs-0.9/zerocs/fork/_func.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)     1115 2023-04-19 11:33:05.000000 zerocs-0.9/zerocs/fork/fork_.py
-drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-26 13:46:46.486051 zerocs-0.9/zerocs/logger/
--rw-r--r--   0 yanping   (1000) yanping   (1000)       41 2023-04-20 04:53:25.000000 zerocs-0.9/zerocs/logger/__init__.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)     1860 2023-04-20 04:53:25.000000 zerocs-0.9/zerocs/logger/_logger.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)      392 2023-04-19 11:33:05.000000 zerocs-0.9/zerocs/logger/logger_.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)     7354 2023-04-26 13:20:00.000000 zerocs-0.9/zerocs/mate.py
-drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-26 13:46:46.486051 zerocs-0.9/zerocs/network/
--rw-r--r--   0 yanping   (1000) yanping   (1000)       44 2023-04-20 04:53:25.000000 zerocs-0.9/zerocs/network/__init__.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)      425 2023-04-20 04:53:25.000000 zerocs-0.9/zerocs/network/_network.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)      508 2023-04-19 11:33:05.000000 zerocs-0.9/zerocs/network/network_.py
-drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-26 13:46:46.486051 zerocs-0.9/zerocs/rabbitmq/
--rw-r--r--   0 yanping   (1000) yanping   (1000)       47 2023-04-20 04:53:25.000000 zerocs-0.9/zerocs/rabbitmq/__init__.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)     1288 2023-04-20 04:53:25.000000 zerocs-0.9/zerocs/rabbitmq/_rabbitmq.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)     1293 2023-04-19 11:33:05.000000 zerocs-0.9/zerocs/rabbitmq/rabbitmq_.py
-drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-26 13:46:46.486051 zerocs-0.9/zerocs/script/
--rw-r--r--   0 yanping   (1000) yanping   (1000)       39 2023-04-20 04:53:25.000000 zerocs-0.9/zerocs/script/__init__.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)     1460 2023-04-26 13:20:00.000000 zerocs-0.9/zerocs/script/_queue.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)      708 2023-04-19 11:33:05.000000 zerocs-0.9/zerocs/script/queue_.py
-drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-26 13:46:46.486051 zerocs-0.9/zerocs/snowflakeId/
--rw-r--r--   0 yanping   (1000) yanping   (1000)       55 2023-04-20 04:53:25.000000 zerocs-0.9/zerocs/snowflakeId/__init__.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)     1918 2023-04-20 04:53:25.000000 zerocs-0.9/zerocs/snowflakeId/_snowflakeId.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)      469 2023-04-19 11:33:05.000000 zerocs-0.9/zerocs/snowflakeId/snowflakeId.py
-drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-26 13:46:46.486051 zerocs-0.9/zerocs/sqlite/
--rw-r--r--   0 yanping   (1000) yanping   (1000)       42 2023-04-20 04:53:25.000000 zerocs-0.9/zerocs/sqlite/__init__.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)     5529 2023-04-20 04:53:25.000000 zerocs-0.9/zerocs/sqlite/_sqlite.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)     3577 2023-04-20 03:18:43.000000 zerocs-0.9/zerocs/sqlite/sqlite3_.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)    11296 2023-04-26 13:20:22.000000 zerocs-0.9/zerocs/zerocs_.py
-drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-26 13:46:46.486051 zerocs-0.9/zerocs.egg-info/
--rw-r--r--   0 yanping   (1000) yanping   (1000)    18156 2023-04-26 13:46:46.000000 zerocs-0.9/zerocs.egg-info/PKG-INFO
--rw-r--r--   0 yanping   (1000) yanping   (1000)      943 2023-04-26 13:46:46.000000 zerocs-0.9/zerocs.egg-info/SOURCES.txt
--rw-r--r--   0 yanping   (1000) yanping   (1000)        1 2023-04-26 13:46:46.000000 zerocs-0.9/zerocs.egg-info/dependency_links.txt
--rw-r--r--   0 yanping   (1000) yanping   (1000)       12 2023-04-26 13:46:46.000000 zerocs-0.9/zerocs.egg-info/requires.txt
--rw-r--r--   0 yanping   (1000) yanping   (1000)        7 2023-04-26 13:46:46.000000 zerocs-0.9/zerocs.egg-info/top_level.txt
+drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-26 15:18:07.091022 zerocs-1.0/
+-rw-r--r--   0 yanping   (1000) yanping   (1000)    18156 2023-04-26 15:18:07.091022 zerocs-1.0/PKG-INFO
+-rw-r--r--   0 yanping   (1000) yanping   (1000)       38 2023-04-26 15:18:07.091022 zerocs-1.0/setup.cfg
+-rw-r--r--   0 yanping   (1000) yanping   (1000)      867 2023-04-26 15:17:55.000000 zerocs-1.0/setup.py
+drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-26 15:18:07.087022 zerocs-1.0/zerocs/
+-rw-r--r--   0 yanping   (1000) yanping   (1000)     4765 2023-04-26 13:53:23.000000 zerocs-1.0/zerocs/__init__.py
+drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-26 15:18:07.087022 zerocs-1.0/zerocs/base/
+-rw-r--r--   0 yanping   (1000) yanping   (1000)      134 2023-04-20 04:53:25.000000 zerocs-1.0/zerocs/base/__init__.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)     1845 2023-04-20 04:53:25.000000 zerocs-1.0/zerocs/base/_base.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)     7208 2023-04-26 13:20:00.000000 zerocs-1.0/zerocs/base/_default_func.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)      496 2023-04-20 04:53:25.000000 zerocs-1.0/zerocs/base/_function.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)     2674 2023-04-19 11:33:05.000000 zerocs-1.0/zerocs/base/base_.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)      529 2023-04-26 13:20:00.000000 zerocs-1.0/zerocs/base/default_func_.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)      670 2023-04-19 11:33:05.000000 zerocs-1.0/zerocs/base/function_.py
+drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-26 15:18:07.087022 zerocs-1.0/zerocs/fork/
+-rw-r--r--   0 yanping   (1000) yanping   (1000)       35 2023-04-20 04:53:25.000000 zerocs-1.0/zerocs/fork/__init__.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)     1993 2023-04-22 03:18:59.000000 zerocs-1.0/zerocs/fork/_func.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)     1115 2023-04-19 11:33:05.000000 zerocs-1.0/zerocs/fork/fork_.py
+drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-26 15:18:07.087022 zerocs-1.0/zerocs/logger/
+-rw-r--r--   0 yanping   (1000) yanping   (1000)       41 2023-04-20 04:53:25.000000 zerocs-1.0/zerocs/logger/__init__.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)     1860 2023-04-20 04:53:25.000000 zerocs-1.0/zerocs/logger/_logger.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)      392 2023-04-19 11:33:05.000000 zerocs-1.0/zerocs/logger/logger_.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)     7354 2023-04-26 13:20:00.000000 zerocs-1.0/zerocs/mate.py
+drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-26 15:18:07.091022 zerocs-1.0/zerocs/network/
+-rw-r--r--   0 yanping   (1000) yanping   (1000)       44 2023-04-20 04:53:25.000000 zerocs-1.0/zerocs/network/__init__.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)      425 2023-04-20 04:53:25.000000 zerocs-1.0/zerocs/network/_network.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)      508 2023-04-19 11:33:05.000000 zerocs-1.0/zerocs/network/network_.py
+drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-26 15:18:07.091022 zerocs-1.0/zerocs/rabbitmq/
+-rw-r--r--   0 yanping   (1000) yanping   (1000)       47 2023-04-20 04:53:25.000000 zerocs-1.0/zerocs/rabbitmq/__init__.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)     1288 2023-04-20 04:53:25.000000 zerocs-1.0/zerocs/rabbitmq/_rabbitmq.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)     1293 2023-04-19 11:33:05.000000 zerocs-1.0/zerocs/rabbitmq/rabbitmq_.py
+drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-26 15:18:07.091022 zerocs-1.0/zerocs/script/
+-rw-r--r--   0 yanping   (1000) yanping   (1000)       39 2023-04-20 04:53:25.000000 zerocs-1.0/zerocs/script/__init__.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)     1460 2023-04-26 13:20:00.000000 zerocs-1.0/zerocs/script/_queue.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)      708 2023-04-19 11:33:05.000000 zerocs-1.0/zerocs/script/queue_.py
+drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-26 15:18:07.091022 zerocs-1.0/zerocs/snowflakeId/
+-rw-r--r--   0 yanping   (1000) yanping   (1000)       55 2023-04-20 04:53:25.000000 zerocs-1.0/zerocs/snowflakeId/__init__.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)     1918 2023-04-20 04:53:25.000000 zerocs-1.0/zerocs/snowflakeId/_snowflakeId.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)      469 2023-04-19 11:33:05.000000 zerocs-1.0/zerocs/snowflakeId/snowflakeId.py
+drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-26 15:18:07.091022 zerocs-1.0/zerocs/sqlite/
+-rw-r--r--   0 yanping   (1000) yanping   (1000)       42 2023-04-20 04:53:25.000000 zerocs-1.0/zerocs/sqlite/__init__.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)     5529 2023-04-20 04:53:25.000000 zerocs-1.0/zerocs/sqlite/_sqlite.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)     3577 2023-04-20 03:18:43.000000 zerocs-1.0/zerocs/sqlite/sqlite3_.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)    11296 2023-04-26 13:20:22.000000 zerocs-1.0/zerocs/zerocs_.py
+drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-26 15:18:07.087022 zerocs-1.0/zerocs.egg-info/
+-rw-r--r--   0 yanping   (1000) yanping   (1000)    18156 2023-04-26 15:18:07.000000 zerocs-1.0/zerocs.egg-info/PKG-INFO
+-rw-r--r--   0 yanping   (1000) yanping   (1000)      943 2023-04-26 15:18:07.000000 zerocs-1.0/zerocs.egg-info/SOURCES.txt
+-rw-r--r--   0 yanping   (1000) yanping   (1000)        1 2023-04-26 15:18:07.000000 zerocs-1.0/zerocs.egg-info/dependency_links.txt
+-rw-r--r--   0 yanping   (1000) yanping   (1000)       12 2023-04-26 15:18:07.000000 zerocs-1.0/zerocs.egg-info/requires.txt
+-rw-r--r--   0 yanping   (1000) yanping   (1000)        7 2023-04-26 15:18:07.000000 zerocs-1.0/zerocs.egg-info/top_level.txt
```

### Comparing `zerocs-0.9/PKG-INFO` & `zerocs-1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zerocs
-Version: 0.9
+Version: 1.0
 Summary: zerocs
 Home-page: https://github.com/ZYPGITA/zerocs
 Author: YanPing
 Author-email: zyphhxx@foxmail.com
 Maintainer: YanPing
 Maintainer-email: zyphhxx@foxmail.com
 License: MIT License
```

### Comparing `zerocs-0.9/setup.py` & `zerocs-1.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='zerocs',
-    version='0.9',
+    version='1.0',
     description="zerocs",
     long_description=open('zerocs/README.rst').read(),
     # long_description_content_type='text/plain',
     include_package_data=True,
     author='YanPing',
     author_email='zyphhxx@foxmail.com',
     maintainer='YanPing',
```

### Comparing `zerocs-0.9/zerocs/__init__.py` & `zerocs-1.0/zerocs/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,19 +50,19 @@
                         Other file storage directories, it is recommended to store task data
 
         ZERO_FW_SERVICE_PATH：
                         service script path
 
         RABBITMQ_CONFIG_URL：
                         The interface for obtaining rabbitmq configuration information. The return information
-                        must include RM_CONFIG field: {'RM_CONFIG':{'AMQP_URI': 'admin@Rabbit*ads12@192.168.100.2'}}
+                        must include RM_CONFIG field: {'RM_CONFIG':{'AMQP_URI': 'admin@123456@127.0.0.1'}}
 
         RABBITMQ_CONFIG:
                         rabbitmq This field and RABBITMQ_CONFIG_URL must have one，
-                        Prioritize the use of this configuration item, e.g: admin@Rabbit*ads12@192.168.100.2
+                        Prioritize the use of this configuration item, e.g: admin@123456@127.0.0.1
 
         RABBITMQ_PORT:
                     rabbitmq port, default 5672
 
         ZERO_FW_NODE_MASTER:
                     zerocs service node type Master: True ,Slave: False
```

### Comparing `zerocs-0.9/zerocs/base/_base.py` & `zerocs-1.0/zerocs/base/_base.py`

 * *Files identical despite different names*

### Comparing `zerocs-0.9/zerocs/base/_default_func.py` & `zerocs-1.0/zerocs/base/_default_func.py`

 * *Files identical despite different names*

### Comparing `zerocs-0.9/zerocs/base/base_.py` & `zerocs-1.0/zerocs/base/base_.py`

 * *Files identical despite different names*

### Comparing `zerocs-0.9/zerocs/base/default_func_.py` & `zerocs-1.0/zerocs/base/default_func_.py`

 * *Files identical despite different names*

### Comparing `zerocs-0.9/zerocs/base/function_.py` & `zerocs-1.0/zerocs/base/function_.py`

 * *Files identical despite different names*

### Comparing `zerocs-0.9/zerocs/fork/_func.py` & `zerocs-1.0/zerocs/fork/_func.py`

 * *Files identical despite different names*

### Comparing `zerocs-0.9/zerocs/fork/fork_.py` & `zerocs-1.0/zerocs/fork/fork_.py`

 * *Files identical despite different names*

### Comparing `zerocs-0.9/zerocs/logger/_logger.py` & `zerocs-1.0/zerocs/logger/_logger.py`

 * *Files identical despite different names*

### Comparing `zerocs-0.9/zerocs/mate.py` & `zerocs-1.0/zerocs/mate.py`

 * *Files identical despite different names*

### Comparing `zerocs-0.9/zerocs/rabbitmq/_rabbitmq.py` & `zerocs-1.0/zerocs/rabbitmq/_rabbitmq.py`

 * *Files identical despite different names*

### Comparing `zerocs-0.9/zerocs/rabbitmq/rabbitmq_.py` & `zerocs-1.0/zerocs/rabbitmq/rabbitmq_.py`

 * *Files identical despite different names*

### Comparing `zerocs-0.9/zerocs/script/_queue.py` & `zerocs-1.0/zerocs/script/_queue.py`

 * *Files identical despite different names*

### Comparing `zerocs-0.9/zerocs/script/queue_.py` & `zerocs-1.0/zerocs/script/queue_.py`

 * *Files identical despite different names*

### Comparing `zerocs-0.9/zerocs/snowflakeId/_snowflakeId.py` & `zerocs-1.0/zerocs/snowflakeId/_snowflakeId.py`

 * *Files identical despite different names*

### Comparing `zerocs-0.9/zerocs/sqlite/_sqlite.py` & `zerocs-1.0/zerocs/sqlite/_sqlite.py`

 * *Files identical despite different names*

### Comparing `zerocs-0.9/zerocs/sqlite/sqlite3_.py` & `zerocs-1.0/zerocs/sqlite/sqlite3_.py`

 * *Files identical despite different names*

### Comparing `zerocs-0.9/zerocs/zerocs_.py` & `zerocs-1.0/zerocs/zerocs_.py`

 * *Files identical despite different names*

### Comparing `zerocs-0.9/zerocs.egg-info/PKG-INFO` & `zerocs-1.0/zerocs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zerocs
-Version: 0.9
+Version: 1.0
 Summary: zerocs
 Home-page: https://github.com/ZYPGITA/zerocs
 Author: YanPing
 Author-email: zyphhxx@foxmail.com
 Maintainer: YanPing
 Maintainer-email: zyphhxx@foxmail.com
 License: MIT License
```

### Comparing `zerocs-0.9/zerocs.egg-info/SOURCES.txt` & `zerocs-1.0/zerocs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

