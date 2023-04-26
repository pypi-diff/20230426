# Comparing `tmp/croudtech-ecs-tools-1.0.3.tar.gz` & `tmp/croudtech-ecs-tools-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "croudtech-ecs-tools-1.0.3.tar", last modified: Tue Apr 25 09:43:27 2023, max compression
+gzip compressed data, was "croudtech-ecs-tools-1.0.4.tar", last modified: Wed Apr 26 11:01:24 2023, max compression
```

## Comparing `croudtech-ecs-tools-1.0.3.tar` & `croudtech-ecs-tools-1.0.4.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-25 09:43:27.417009 croudtech-ecs-tools-1.0.3/
--rw-r--r--   0 vsts      (1001) docker     (123)    11357 2023-04-25 09:42:46.000000 croudtech-ecs-tools-1.0.3/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (123)     2335 2023-04-25 09:43:27.417009 croudtech-ecs-tools-1.0.3/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     1370 2023-04-25 09:42:46.000000 croudtech-ecs-tools-1.0.3/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-25 09:43:27.417009 croudtech-ecs-tools-1.0.3/croudtech_ecs_tools/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-04-25 09:42:46.000000 croudtech-ecs-tools-1.0.3/croudtech_ecs_tools/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8136 2023-04-25 09:42:46.000000 croudtech-ecs-tools-1.0.3/croudtech_ecs_tools/cli.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9094 2023-04-25 09:42:46.000000 croudtech-ecs-tools-1.0.3/croudtech_ecs_tools/ecs.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-25 09:43:27.417009 croudtech-ecs-tools-1.0.3/croudtech_ecs_tools.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)     2335 2023-04-25 09:43:27.000000 croudtech-ecs-tools-1.0.3/croudtech_ecs_tools.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      372 2023-04-25 09:43:27.000000 croudtech-ecs-tools-1.0.3/croudtech_ecs_tools.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-25 09:43:27.000000 croudtech-ecs-tools-1.0.3/croudtech_ecs_tools.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       87 2023-04-25 09:43:27.000000 croudtech-ecs-tools-1.0.3/croudtech_ecs_tools.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (123)      430 2023-04-25 09:43:27.000000 croudtech-ecs-tools-1.0.3/croudtech_ecs_tools.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       20 2023-04-25 09:43:27.000000 croudtech-ecs-tools-1.0.3/croudtech_ecs_tools.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-04-25 09:43:27.417009 croudtech-ecs-tools-1.0.3/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1762 2023-04-25 09:42:46.000000 croudtech-ecs-tools-1.0.3/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-26 11:01:24.386139 croudtech-ecs-tools-1.0.4/
+-rw-r--r--   0 vsts      (1001) docker     (123)    11357 2023-04-26 11:00:52.000000 croudtech-ecs-tools-1.0.4/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (123)     2335 2023-04-26 11:01:24.386139 croudtech-ecs-tools-1.0.4/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     1370 2023-04-26 11:00:52.000000 croudtech-ecs-tools-1.0.4/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-26 11:01:24.386139 croudtech-ecs-tools-1.0.4/croudtech_ecs_tools/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-04-26 11:00:52.000000 croudtech-ecs-tools-1.0.4/croudtech_ecs_tools/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3972 2023-04-26 11:00:52.000000 croudtech-ecs-tools-1.0.4/croudtech_ecs_tools/cli.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3202 2023-04-26 11:00:52.000000 croudtech-ecs-tools-1.0.4/croudtech_ecs_tools/cloudfront.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    13810 2023-04-26 11:00:52.000000 croudtech-ecs-tools-1.0.4/croudtech_ecs_tools/ecs.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-26 11:01:24.386139 croudtech-ecs-tools-1.0.4/croudtech_ecs_tools.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     2335 2023-04-26 11:01:24.000000 croudtech-ecs-tools-1.0.4/croudtech_ecs_tools.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      406 2023-04-26 11:01:24.000000 croudtech-ecs-tools-1.0.4/croudtech_ecs_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-26 11:01:24.000000 croudtech-ecs-tools-1.0.4/croudtech_ecs_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       87 2023-04-26 11:01:24.000000 croudtech-ecs-tools-1.0.4/croudtech_ecs_tools.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)      430 2023-04-26 11:01:24.000000 croudtech-ecs-tools-1.0.4/croudtech_ecs_tools.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       20 2023-04-26 11:01:24.000000 croudtech-ecs-tools-1.0.4/croudtech_ecs_tools.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-04-26 11:01:24.386139 croudtech-ecs-tools-1.0.4/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1762 2023-04-26 11:00:52.000000 croudtech-ecs-tools-1.0.4/setup.py
```

### Comparing `croudtech-ecs-tools-1.0.3/LICENSE` & `croudtech-ecs-tools-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `croudtech-ecs-tools-1.0.3/PKG-INFO` & `croudtech-ecs-tools-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: croudtech-ecs-tools
-Version: 1.0.3
+Version: 1.0.4
 Summary: Tools for managing ECS Services and Tasks
 Home-page: https://github.com/CroudTech/croudtech-ecs-tools
 Author: Jim Robinson
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/CroudTech/croudtech-ecs-tools/issues
 Project-URL: CI, https://github.com/CroudTech/croudtech-ecs-tools/actions
 Project-URL: Changelog, https://github.com/CroudTech/croudtech-ecs-tools/releases
```

### Comparing `croudtech-ecs-tools-1.0.3/README.md` & `croudtech-ecs-tools-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `croudtech-ecs-tools-1.0.3/croudtech_ecs_tools/ecs.py` & `croudtech-ecs-tools-1.0.4/croudtech_ecs_tools/ecs.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     ECSClient = object
 
 from typing import List
 import json
 from datetime import datetime
 import click
 
+from botocore.config import Config as Boto3Config
 
 
 def parse_arn(arn):
     elements = arn.split(':')
     result = {'arn': elements[0],
             'partition': elements[1],
             'service': elements[2],
@@ -226,8 +227,147 @@
                     ])
                     self.ecs_client.update_service(service=service_arn, cluster=cluster_arn, desiredCount=int(desired_count))
                     click.echo(f"Scaled up {service_arn} to {desired_count}")
                 except KeyError:
                     pass
 
     def serviceTagsDict(self, service):
-        return {tag["key"]: tag["value"] for tag in service["tags"]}
+        return {tag["key"]: tag["value"] for tag in service["tags"]}
+
+class EcsTools:
+    _services = {}
+    _tasks = {}
+
+    def __init__(self, region):
+        self.region = region
+        print(self.region)
+        self.ecs_client = boto3.client("ecs", config=Boto3Config(
+            region_name= self.region
+        ))
+
+    @property
+    def clusters(self):
+        if not hasattr(self, "_clusters"):
+            paginator = self.ecs_client.get_paginator("list_clusters")
+            response_iterator = paginator.paginate(
+                PaginationConfig={
+                    "PageSize": 10,
+                }
+            )
+            self._clusters = []
+            for page in response_iterator:
+                for cluster in page["clusterArns"]:
+                    self._clusters.append(cluster.split("/").pop())
+            
+        return self._clusters
+    
+    def extractFromArn(self, arn):
+        arn_parts = arn.split(":")[-1].split("/")[1:]
+        return arn_parts
+
+    def get_services(self, cluster):
+        if cluster not in self._services:
+            self._services[cluster] = []
+            paginator = self.ecs_client.get_paginator("list_services")
+
+            response_iterator = paginator.paginate(
+                cluster=cluster,           
+                PaginationConfig={
+                    "PageSize": 50,
+                }
+            )
+            for page in response_iterator:
+                for service in page["serviceArns"]:
+                    self._services[cluster].append(service)
+        return self._services[cluster]
+
+    def get_tasks(self, cluster, service):
+        task_key = cluster+service
+        if task_key not in self._tasks:
+            self._tasks[task_key] = []
+            paginator = self.ecs_client.get_paginator("list_tasks")
+            response_iterator = paginator.paginate(
+                cluster=cluster,
+                serviceName=service,           
+                PaginationConfig={
+                    "PageSize": 50,
+                }
+            )
+            for page in response_iterator:
+                for task in page["taskArns"]:
+                    self._tasks[task_key].append(task)
+        return self._tasks[task_key]
+
+    def describe_task(self, cluster, task_arn):
+        response = self.ecs_client.describe_tasks(
+            cluster=cluster,
+            tasks=[
+                task_arn,
+            ],            
+        )
+        task = response["tasks"].pop()
+        return task
+
+    def execute_command(self,cluster, container, task_arn, command="bash"):
+        return self.ecs_client.execute_command(
+            cluster=cluster,
+            container=container["name"],
+            command=command,
+            interactive=True,
+            task=task_arn
+        )
+
+    def restart_service(self, service_arn, wait=False):
+        try:
+            cluster, service = self.extractFromArn(service_arn)
+        except ValueError as err:
+            click.echo(f"Invalid service ARN {service_arn}")
+            return
+        waiter = self.ecs_client.get_waiter('services_stable')
+        
+        self.ecs_client.update_service(
+            cluster=cluster,
+            service=service,
+            forceNewDeployment=True
+        )
+        if wait:
+            waiter.wait(
+                cluster=cluster,
+                services=[
+                    service,
+                ],            
+                WaiterConfig={
+                    'Delay': 5,
+                    'MaxAttempts': 100
+                }
+            )
+        return True
+
+    def get_task_containers(self, cluster, task_arn):
+        return self.describe_task(cluster, task_arn)["containers"]
+    
+    def get_service_options(self, cluster):
+        options = []
+        for index, option in enumerate(self.get_services(cluster)):
+            option_name = option.split("/").pop()
+            options.append(f"{index}: {option_name}")
+        return "\n".join(options)
+
+    def get_task_options(self, cluster, service):
+        options = []
+        for index, option in enumerate(self.get_tasks(cluster, service)):
+            option_name = option.split("/").pop()
+            options.append(f"{index}: {option_name}")
+        return "\n".join(options)
+
+    def get_task__container_options(self, cluster, task_arn):
+        options = []
+        for index, option in enumerate(self.get_task_containers(cluster, task_arn)):
+            option_name = option["name"]
+            options.append(f"{index}: {option_name}")
+        return "\n".join(options)
+
+    def get_cluster_options(self):
+        options = []
+        for index, option in enumerate(self.clusters):
+            options.append(f"{index}: {option}")
+        return "\n".join(options)
```

### Comparing `croudtech-ecs-tools-1.0.3/croudtech_ecs_tools.egg-info/PKG-INFO` & `croudtech-ecs-tools-1.0.4/croudtech_ecs_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: croudtech-ecs-tools
-Version: 1.0.3
+Version: 1.0.4
 Summary: Tools for managing ECS Services and Tasks
 Home-page: https://github.com/CroudTech/croudtech-ecs-tools
 Author: Jim Robinson
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/CroudTech/croudtech-ecs-tools/issues
 Project-URL: CI, https://github.com/CroudTech/croudtech-ecs-tools/actions
 Project-URL: Changelog, https://github.com/CroudTech/croudtech-ecs-tools/releases
```

### Comparing `croudtech-ecs-tools-1.0.3/setup.py` & `croudtech-ecs-tools-1.0.4/setup.py`

 * *Files identical despite different names*

