# Comparing `tmp/aws_toolset-0.0.5.tar.gz` & `tmp/aws_toolset-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_toolset-0.0.5.tar", last modified: Tue Apr 25 23:14:08 2023, max compression
+gzip compressed data, was "aws_toolset-0.0.6.tar", last modified: Wed Apr 26 00:08:06 2023, max compression
```

## Comparing `aws_toolset-0.0.5.tar` & `aws_toolset-0.0.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 coopmaster  (1000) coopmaster  (1000)        0 2023-04-25 23:14:08.708454 aws_toolset-0.0.5/
--rw-rw-r--   0 coopmaster  (1000) coopmaster  (1000)    35149 2023-03-09 22:12:16.000000 aws_toolset-0.0.5/LICENSE
--rw-rw-r--   0 coopmaster  (1000) coopmaster  (1000)     3924 2023-04-25 23:14:08.708454 aws_toolset-0.0.5/PKG-INFO
--rw-rw-r--   0 coopmaster  (1000) coopmaster  (1000)     3465 2023-04-25 22:58:24.000000 aws_toolset-0.0.5/README.md
-drwxrwxr-x   0 coopmaster  (1000) coopmaster  (1000)        0 2023-04-25 23:14:08.704454 aws_toolset-0.0.5/aws_toolset/
--rw-rw-r--   0 coopmaster  (1000) coopmaster  (1000)       26 2023-04-03 21:51:46.000000 aws_toolset-0.0.5/aws_toolset/__init__.py
--rw-rw-r--   0 coopmaster  (1000) coopmaster  (1000)       93 2023-04-03 21:51:46.000000 aws_toolset-0.0.5/aws_toolset/__main__.py
--rw-rw-r--   0 coopmaster  (1000) coopmaster  (1000)     1541 2023-04-25 23:02:06.000000 aws_toolset-0.0.5/aws_toolset/aws_toolset.py
-drwxrwxr-x   0 coopmaster  (1000) coopmaster  (1000)        0 2023-04-25 23:14:08.704454 aws_toolset-0.0.5/aws_toolset/modules/
--rw-rw-r--   0 coopmaster  (1000) coopmaster  (1000)      141 2023-04-25 19:24:07.000000 aws_toolset-0.0.5/aws_toolset/modules/__init__.py
--rwxrwxr-x   0 coopmaster  (1000) coopmaster  (1000)     9665 2023-04-09 02:54:37.000000 aws_toolset-0.0.5/aws_toolset/modules/create_codestar_notifications.py
--rw-rw-r--   0 coopmaster  (1000) coopmaster  (1000)     6537 2023-04-25 22:58:24.000000 aws_toolset-0.0.5/aws_toolset/modules/generate_ecs_execute_command.py
--rw-rw-r--   0 coopmaster  (1000) coopmaster  (1000)     6732 2023-04-25 23:11:16.000000 aws_toolset-0.0.5/aws_toolset/modules/get_ec2_ecs_info.py
--rw-rw-r--   0 coopmaster  (1000) coopmaster  (1000)     7623 2023-04-25 22:58:24.000000 aws_toolset-0.0.5/aws_toolset/modules/utils.py
-drwxrwxr-x   0 coopmaster  (1000) coopmaster  (1000)        0 2023-04-25 23:14:08.704454 aws_toolset-0.0.5/aws_toolset.egg-info/
--rw-rw-r--   0 coopmaster  (1000) coopmaster  (1000)     3924 2023-04-25 23:14:08.000000 aws_toolset-0.0.5/aws_toolset.egg-info/PKG-INFO
--rw-rw-r--   0 coopmaster  (1000) coopmaster  (1000)      519 2023-04-25 23:14:08.000000 aws_toolset-0.0.5/aws_toolset.egg-info/SOURCES.txt
--rw-rw-r--   0 coopmaster  (1000) coopmaster  (1000)        1 2023-04-25 23:14:08.000000 aws_toolset-0.0.5/aws_toolset.egg-info/dependency_links.txt
--rw-rw-r--   0 coopmaster  (1000) coopmaster  (1000)       61 2023-04-25 23:14:08.000000 aws_toolset-0.0.5/aws_toolset.egg-info/entry_points.txt
--rw-rw-r--   0 coopmaster  (1000) coopmaster  (1000)       15 2023-04-25 23:14:08.000000 aws_toolset-0.0.5/aws_toolset.egg-info/requires.txt
--rw-rw-r--   0 coopmaster  (1000) coopmaster  (1000)       12 2023-04-25 23:14:08.000000 aws_toolset-0.0.5/aws_toolset.egg-info/top_level.txt
--rw-rw-r--   0 coopmaster  (1000) coopmaster  (1000)       38 2023-04-25 23:14:08.708454 aws_toolset-0.0.5/setup.cfg
--rw-rw-r--   0 coopmaster  (1000) coopmaster  (1000)      829 2023-04-25 23:13:56.000000 aws_toolset-0.0.5/setup.py
+drwxrwxr-x   0 coopmaster  (1000) coopmaster  (1000)        0 2023-04-26 00:08:06.598450 aws_toolset-0.0.6/
+-rw-rw-r--   0 coopmaster  (1000) coopmaster  (1000)    35149 2023-03-09 22:12:16.000000 aws_toolset-0.0.6/LICENSE
+-rw-rw-r--   0 coopmaster  (1000) coopmaster  (1000)     3924 2023-04-26 00:08:06.598450 aws_toolset-0.0.6/PKG-INFO
+-rw-rw-r--   0 coopmaster  (1000) coopmaster  (1000)     3465 2023-04-25 22:58:24.000000 aws_toolset-0.0.6/README.md
+drwxrwxr-x   0 coopmaster  (1000) coopmaster  (1000)        0 2023-04-26 00:08:06.594450 aws_toolset-0.0.6/aws_toolset/
+-rw-rw-r--   0 coopmaster  (1000) coopmaster  (1000)       26 2023-04-03 21:51:46.000000 aws_toolset-0.0.6/aws_toolset/__init__.py
+-rw-rw-r--   0 coopmaster  (1000) coopmaster  (1000)       93 2023-04-03 21:51:46.000000 aws_toolset-0.0.6/aws_toolset/__main__.py
+-rw-rw-r--   0 coopmaster  (1000) coopmaster  (1000)     1541 2023-04-25 23:02:06.000000 aws_toolset-0.0.6/aws_toolset/aws_toolset.py
+drwxrwxr-x   0 coopmaster  (1000) coopmaster  (1000)        0 2023-04-26 00:08:06.598450 aws_toolset-0.0.6/aws_toolset/modules/
+-rw-rw-r--   0 coopmaster  (1000) coopmaster  (1000)      141 2023-04-25 19:24:07.000000 aws_toolset-0.0.6/aws_toolset/modules/__init__.py
+-rwxrwxr-x   0 coopmaster  (1000) coopmaster  (1000)     9665 2023-04-09 02:54:37.000000 aws_toolset-0.0.6/aws_toolset/modules/create_codestar_notifications.py
+-rw-rw-r--   0 coopmaster  (1000) coopmaster  (1000)     6537 2023-04-25 22:58:24.000000 aws_toolset-0.0.6/aws_toolset/modules/generate_ecs_execute_command.py
+-rw-rw-r--   0 coopmaster  (1000) coopmaster  (1000)     6810 2023-04-26 00:07:51.000000 aws_toolset-0.0.6/aws_toolset/modules/get_ec2_ecs_info.py
+-rw-rw-r--   0 coopmaster  (1000) coopmaster  (1000)     7623 2023-04-25 22:58:24.000000 aws_toolset-0.0.6/aws_toolset/modules/utils.py
+drwxrwxr-x   0 coopmaster  (1000) coopmaster  (1000)        0 2023-04-26 00:08:06.598450 aws_toolset-0.0.6/aws_toolset.egg-info/
+-rw-rw-r--   0 coopmaster  (1000) coopmaster  (1000)     3924 2023-04-26 00:08:06.000000 aws_toolset-0.0.6/aws_toolset.egg-info/PKG-INFO
+-rw-rw-r--   0 coopmaster  (1000) coopmaster  (1000)      519 2023-04-26 00:08:06.000000 aws_toolset-0.0.6/aws_toolset.egg-info/SOURCES.txt
+-rw-rw-r--   0 coopmaster  (1000) coopmaster  (1000)        1 2023-04-26 00:08:06.000000 aws_toolset-0.0.6/aws_toolset.egg-info/dependency_links.txt
+-rw-rw-r--   0 coopmaster  (1000) coopmaster  (1000)       61 2023-04-26 00:08:06.000000 aws_toolset-0.0.6/aws_toolset.egg-info/entry_points.txt
+-rw-rw-r--   0 coopmaster  (1000) coopmaster  (1000)       15 2023-04-26 00:08:06.000000 aws_toolset-0.0.6/aws_toolset.egg-info/requires.txt
+-rw-rw-r--   0 coopmaster  (1000) coopmaster  (1000)       12 2023-04-26 00:08:06.000000 aws_toolset-0.0.6/aws_toolset.egg-info/top_level.txt
+-rw-rw-r--   0 coopmaster  (1000) coopmaster  (1000)       38 2023-04-26 00:08:06.598450 aws_toolset-0.0.6/setup.cfg
+-rw-rw-r--   0 coopmaster  (1000) coopmaster  (1000)      829 2023-04-26 00:07:51.000000 aws_toolset-0.0.6/setup.py
```

### Comparing `aws_toolset-0.0.5/LICENSE` & `aws_toolset-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `aws_toolset-0.0.5/PKG-INFO` & `aws_toolset-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws_toolset
-Version: 0.0.5
+Version: 0.0.6
 Summary: AWS Toolset for AWS Devs
 Home-page: https://github.com/sgcooper78/aws_toolset
 Author: Scott Cooper
 Author-email: sgcooper78@gmail.com
 Keywords: python,aws,boto3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `aws_toolset-0.0.5/README.md` & `aws_toolset-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `aws_toolset-0.0.5/aws_toolset/aws_toolset.py` & `aws_toolset-0.0.6/aws_toolset/aws_toolset.py`

 * *Files identical despite different names*

### Comparing `aws_toolset-0.0.5/aws_toolset/modules/create_codestar_notifications.py` & `aws_toolset-0.0.6/aws_toolset/modules/create_codestar_notifications.py`

 * *Files identical despite different names*

### Comparing `aws_toolset-0.0.5/aws_toolset/modules/generate_ecs_execute_command.py` & `aws_toolset-0.0.6/aws_toolset/modules/generate_ecs_execute_command.py`

 * *Files identical despite different names*

### Comparing `aws_toolset-0.0.5/aws_toolset/modules/get_ec2_ecs_info.py` & `aws_toolset-0.0.6/aws_toolset/modules/get_ec2_ecs_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,25 +119,28 @@
 
     ec2_container_instances_arns = get_all_resource_names("ecs","ecs_container_instances",{"cluster" : args.Cluster})
 
     ec2_container_instances = ecs_client.describe_container_instances(
         cluster=args.Cluster,
         containerInstances=ec2_container_instances_arns
     )
-
+    
     for instance in ec2_container_instances['containerInstances']:
             # Describe tasks
         instance['tasks'] = []
         instance['containerNames'] = []
 
         t_list_response = ecs_client.list_tasks(
             cluster=args.Cluster,
             containerInstance=instance['containerInstanceArn']
         )
 
+        if not t_list_response['taskArns']:
+            continue
+        
         task_descriptions_response = ecs_client.describe_tasks(
             cluster=args.Cluster,
             tasks=t_list_response['taskArns']
         )
         instance['tasks'].append(task_descriptions_response)
 
         for task in task_descriptions_response['tasks']:
```

### Comparing `aws_toolset-0.0.5/aws_toolset/modules/utils.py` & `aws_toolset-0.0.6/aws_toolset/modules/utils.py`

 * *Files identical despite different names*

### Comparing `aws_toolset-0.0.5/aws_toolset.egg-info/PKG-INFO` & `aws_toolset-0.0.6/aws_toolset.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-toolset
-Version: 0.0.5
+Version: 0.0.6
 Summary: AWS Toolset for AWS Devs
 Home-page: https://github.com/sgcooper78/aws_toolset
 Author: Scott Cooper
 Author-email: sgcooper78@gmail.com
 Keywords: python,aws,boto3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `aws_toolset-0.0.5/aws_toolset.egg-info/SOURCES.txt` & `aws_toolset-0.0.6/aws_toolset.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aws_toolset-0.0.5/setup.py` & `aws_toolset-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as fh:
     long_description = fh.read()
 
 setup(
     name="aws_toolset",
-    version="0.0.5",
+    version="0.0.6",
     url='https://github.com/sgcooper78/aws_toolset',
     author="Scott Cooper",
     author_email="sgcooper78@gmail.com",
     description="AWS Toolset for AWS Devs",
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
```

