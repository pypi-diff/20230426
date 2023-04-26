# Comparing `tmp/strongmind_deployment-0.0.7-py3-none-any.whl.zip` & `tmp/strongmind_deployment-0.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3797 bytes, number of entries: 7
+Zip file size: 4129 bytes, number of entries: 7
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 strongmind_deployment/__init__.py
--rw-r--r--  2.0 unx     2333 b- defN 20-Feb-02 00:00 strongmind_deployment/container.py
--rw-r--r--  2.0 unx     1786 b- defN 20-Feb-02 00:00 strongmind_deployment/rails.py
-?rw-r--r--  2.0 unx      646 b- defN 20-Feb-02 00:00 strongmind_deployment-0.0.7.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 strongmind_deployment-0.0.7.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1053 b- defN 20-Feb-02 00:00 strongmind_deployment-0.0.7.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx      623 b- defN 20-Feb-02 00:00 strongmind_deployment-0.0.7.dist-info/RECORD
-7 files, 6528 bytes uncompressed, 2675 bytes compressed:  59.0%
+-rw-r--r--  2.0 unx     2476 b- defN 20-Feb-02 00:00 strongmind_deployment/container.py
+-rw-r--r--  2.0 unx     3191 b- defN 20-Feb-02 00:00 strongmind_deployment/rails.py
+?rw-r--r--  2.0 unx      675 b- defN 20-Feb-02 00:00 strongmind_deployment-0.0.8.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 strongmind_deployment-0.0.8.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1053 b- defN 20-Feb-02 00:00 strongmind_deployment-0.0.8.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx      623 b- defN 20-Feb-02 00:00 strongmind_deployment-0.0.8.dist-info/RECORD
+7 files, 8105 bytes uncompressed, 3007 bytes compressed:  62.9%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: strongmind_deployment/container.py
 Comment: 
 
 Filename: strongmind_deployment/rails.py
 Comment: 
 
-Filename: strongmind_deployment-0.0.7.dist-info/METADATA
+Filename: strongmind_deployment-0.0.8.dist-info/METADATA
 Comment: 
 
-Filename: strongmind_deployment-0.0.7.dist-info/WHEEL
+Filename: strongmind_deployment-0.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: strongmind_deployment-0.0.7.dist-info/licenses/LICENSE
+Filename: strongmind_deployment-0.0.8.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: strongmind_deployment-0.0.7.dist-info/RECORD
+Filename: strongmind_deployment-0.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## strongmind_deployment/container.py

```diff
@@ -12,14 +12,15 @@
         super().__init__('strongmind:global_build:commons:container', name, None, opts)
 
         self.container_image = kwargs.get('container_image')
         self.app_path = kwargs.get('app_path') or './'
         self.container_port = kwargs.get('container_port') or 3000
         self.cpu = kwargs.get('cpu') or 256
         self.memory = kwargs.get("memory") or 512
+        self.env_vars = kwargs.get('env_vars', {})
 
         self.ecs_cluster = aws.ecs.Cluster("cluster",
                                            name=name,
                                            opts=pulumi.ResourceOptions(parent=self),
                                            )
         self.load_balancer = awsx.lb.ApplicationLoadBalancer("loadbalancer",
                                                              name=name,
@@ -34,14 +35,15 @@
                     memory=self.memory,
                     essential=True,
                     port_mappings=[awsx.ecs.TaskDefinitionPortMappingArgs(
                         container_port=self.container_port,
                         host_port=self.container_port,
                         target_group=self.load_balancer.default_target_group,
                     )],
+                    environment=[{"name": k, "value": v} for k, v in self.env_vars.items()]
                 )
             )
 
         self.fargate_service = awsx.ecs.FargateService(
             "service",
             name=f"{name}-service",
             cluster=self.ecs_cluster.arn,
```

## strongmind_deployment/rails.py

```diff
@@ -1,50 +1,78 @@
 import json
 
 import pulumi
+import pulumi_random as random
 import pulumi_aws as aws
+from pulumi import export, Output
 
 from strongmind_deployment.container import ContainerComponent
 
 
 class RailsComponent(pulumi.ComponentResource):
     def __init__(self, name, opts=None, **kwargs):
         super().__init__('strongmind:global_build:commons:rails', name, None, opts)
+        self.db_password = None
+        self.container = None
+        self.rds_serverless_cluster_instance = None
+        self.rds_serverless_cluster = None
         self.kwargs = kwargs
 
         self.rds(name)
 
         self.ecs(name)
 
         self.register_outputs({
             'rds_serverless_cluster': self.rds_serverless_cluster.cluster_identifier
         })
 
     def ecs(self, name):
+        if 'env_vars' not in self.kwargs:
+            self.kwargs['env_vars'] = {}
+
+        self.kwargs['env_vars']['DATABASE_HOST'] = self.rds_serverless_cluster.endpoint
+        self.kwargs['env_vars']['DB_USERNAME'] = self.rds_serverless_cluster.master_username
+        self.kwargs['env_vars']['DB_PASSWORD'] = self.rds_serverless_cluster.master_password
+        self.kwargs['env_vars']['DATABASE_URL'] = self.get_database_url()
         self.container = ContainerComponent(name,
                                             pulumi.ResourceOptions(parent=self),
                                             **self.kwargs
                                             )
 
     def rds(self, name):
+        self.db_password = random.RandomPassword("password",
+                                                 length=30,
+                                                 special=False)
         self.rds_serverless_cluster = aws.rds.Cluster(
             'rds_serverless_cluster',
             cluster_identifier=name,
             engine='aurora-postgresql',
             engine_mode='provisioned',
             engine_version='15.2',
             master_username=name.replace('-', '_'),
-            master_password="blahblahblah",
+            master_password=self.db_password.result,
             opts=pulumi.ResourceOptions(parent=self),
             serverlessv2_scaling_configuration=aws.rds.ClusterServerlessv2ScalingConfigurationArgs(
                 min_capacity=0.5,
                 max_capacity=16,
             )
         )
         self.rds_serverless_cluster_instance = aws.rds.ClusterInstance(
             'rds_serverless_cluster_instance',
             identifier=name,
             cluster_identifier=self.rds_serverless_cluster.cluster_identifier,
             instance_class='db.serverless',
             engine=self.rds_serverless_cluster.engine,
             engine_version=self.rds_serverless_cluster.engine_version,
         )
+
+        export("db_endpoint", Output.concat(self.rds_serverless_cluster.endpoint))
+
+    def get_database_url(self):
+        return Output.concat('postgres://',
+                             self.rds_serverless_cluster.master_username,
+                             ':',
+                             self.rds_serverless_cluster.master_password,
+                             '@',
+                             self.rds_serverless_cluster.endpoint,
+                             ':5432/',
+                             self.rds_serverless_cluster.master_username)
```

## Comparing `strongmind_deployment-0.0.7.dist-info/licenses/LICENSE` & `strongmind_deployment-0.0.8.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

