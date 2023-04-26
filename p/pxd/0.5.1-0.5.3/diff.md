# Comparing `tmp/pxd-0.5.1-py3-none-any.whl.zip` & `tmp/pxd-0.5.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 79705 bytes, number of entries: 60
+Zip file size: 79832 bytes, number of entries: 60
 -rw-r--r--  2.0 unx      622 b- defN 22-Mar-14 02:39 deployer/__init__.py
 -rw-r--r--  2.0 unx      790 b- defN 22-Mar-14 02:39 deployer/_repo.py
 -rw-r--r--  2.0 unx      733 b- defN 22-Mar-14 02:39 deployer/logging.yaml
--rw-r--r--  2.0 unx     6887 b- defN 23-Apr-04 02:13 deployer/pxd.py
--rw-r--r--  2.0 unx       23 b- defN 23-Apr-04 02:16 deployer/version.txt
+-rw-r--r--  2.0 unx     6887 b- defN 23-Apr-14 03:25 deployer/pxd.py
+-rw-r--r--  2.0 unx       44 b- defN 23-Apr-26 08:20 deployer/version.txt
 -rw-r--r--  2.0 unx      622 b- defN 22-Mar-14 02:39 deployer/config/__init__.py
--rw-r--r--  2.0 unx     5304 b- defN 23-Jan-05 09:05 deployer/config/config.py
+-rw-r--r--  2.0 unx     5308 b- defN 23-Apr-26 08:13 deployer/config/config.py
 -rw-r--r--  2.0 unx     1313 b- defN 22-Mar-14 02:39 deployer/config/log_config.py
 -rw-r--r--  2.0 unx     1080 b- defN 22-Jul-04 02:46 deployer/config/metadb_config.py
 -rw-r--r--  2.0 unx      622 b- defN 22-Mar-14 02:39 deployer/constant/__init__.py
 -rw-r--r--  2.0 unx     1195 b- defN 23-Mar-23 05:37 deployer/constant/constant.py
 -rw-r--r--  2.0 unx      715 b- defN 22-Mar-14 02:39 deployer/constant/table_field.py
 -rw-r--r--  2.0 unx      622 b- defN 22-Mar-14 02:39 deployer/core/__init__.py
 -rw-r--r--  2.0 unx      991 b- defN 22-Mar-14 02:39 deployer/core/context.py
@@ -20,16 +20,16 @@
 -rw-r--r--  2.0 unx     2202 b- defN 23-Mar-23 05:37 deployer/decorator/decorators.py
 -rw-r--r--  2.0 unx      622 b- defN 23-Mar-23 05:37 deployer/download/__init__.py
 -rw-r--r--  2.0 unx     1219 b- defN 23-Apr-03 01:57 deployer/download/constant.py
 -rw-r--r--  2.0 unx    10463 b- defN 23-Mar-31 01:44 deployer/download/polardbx_download.py
 -rw-r--r--  2.0 unx      622 b- defN 22-Mar-14 02:39 deployer/pcn/__init__.py
 -rw-r--r--  2.0 unx      622 b- defN 22-Mar-14 02:39 deployer/pxc/__init__.py
 -rw-r--r--  2.0 unx     1070 b- defN 22-Mar-14 02:39 deployer/pxc/gms_consts.py
--rw-r--r--  2.0 unx    42120 b- defN 23-Feb-21 02:14 deployer/pxc/polardbx_cluster.py
--rw-r--r--  2.0 unx     3944 b- defN 22-Dec-14 07:49 deployer/pxc/polardbx_manager.py
+-rw-r--r--  2.0 unx    42226 b- defN 23-Apr-14 02:10 deployer/pxc/polardbx_cluster.py
+-rw-r--r--  2.0 unx     4024 b- defN 23-Apr-14 03:13 deployer/pxc/polardbx_manager.py
 -rw-r--r--  2.0 unx      930 b- defN 22-Mar-14 02:39 deployer/pxc/polardbx_topology.py
 -rw-r--r--  2.0 unx     1257 b- defN 22-Jul-04 02:46 deployer/pxc/pxc_user.py
 -rw-r--r--  2.0 unx      622 b- defN 22-Mar-14 02:39 deployer/resources/__init__.py
 -rw-r--r--  2.0 unx      260 b- defN 23-Mar-23 05:37 deployer/resources/download/scripts/load_image.sh
 -rw-r--r--  2.0 unx     7330 b- defN 22-Mar-14 02:39 deployer/resources/sql/gms_init.sql
 -rw-r--r--  2.0 unx     2137 b- defN 22-Mar-14 02:39 deployer/resources/sql/sqlite_init.sql
 -rw-r--r--  2.0 unx     4872 b- defN 22-Mar-14 02:39 deployer/resources/template/my-8.0.cnf
@@ -41,22 +41,22 @@
 -rw-r--r--  2.0 unx      622 b- defN 22-Jul-04 02:46 deployer/sqlite/__init__.py
 -rw-r--r--  2.0 unx     5922 b- defN 22-Dec-14 07:49 deployer/sqlite/dbapi.py
 -rw-r--r--  2.0 unx     3181 b- defN 22-Jul-04 02:46 deployer/sqlite/sqlite_manager.py
 -rw-r--r--  2.0 unx      622 b- defN 22-Mar-14 02:39 deployer/tests/__init__.py
 -rw-r--r--  2.0 unx      622 b- defN 22-Mar-14 02:39 deployer/tryout/__init__.py
 -rw-r--r--  2.0 unx     1201 b- defN 22-Mar-14 02:39 deployer/tryout/install.py
 -rw-r--r--  2.0 unx      622 b- defN 22-Mar-14 02:39 deployer/util/__init__.py
--rw-r--r--  2.0 unx     3579 b- defN 22-Dec-14 07:49 deployer/util/file_manager.py
+-rw-r--r--  2.0 unx     3578 b- defN 23-Apr-14 03:23 deployer/util/file_manager.py
 -rw-r--r--  2.0 unx     2110 b- defN 22-Mar-14 02:39 deployer/util/mysql_manager.py
 -rw-r--r--  2.0 unx      784 b- defN 22-Mar-14 02:39 deployer/util/network_util.py
 -rw-r--r--  2.0 unx     1494 b- defN 23-Feb-21 02:14 deployer/util/password_util.py
 -rw-r--r--  2.0 unx     2376 b- defN 22-Mar-14 02:39 deployer/util/sqlite_manager.py
 -rw-r--r--  2.0 unx     2585 b- defN 22-Jan-03 07:42 deployer/util/yaml_util.py
 -rw-r--r--  2.0 unx      622 b- defN 22-Mar-14 02:39 deployer/xdb/__init__.py
--rw-r--r--  2.0 unx    22187 b- defN 23-Mar-23 05:37 deployer/xdb/xdb.py
--rw-r--r--  2.0 unx    11358 b- defN 23-Apr-04 03:26 pxd-0.5.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     4541 b- defN 23-Apr-04 03:26 pxd-0.5.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-04 03:26 pxd-0.5.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       73 b- defN 23-Apr-04 03:26 pxd-0.5.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 23-Apr-04 03:26 pxd-0.5.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     5101 b- defN 23-Apr-04 03:26 pxd-0.5.1.dist-info/RECORD
-60 files, 223102 bytes uncompressed, 71601 bytes compressed:  67.9%
+-rw-r--r--  2.0 unx    22469 b- defN 23-Apr-14 02:35 deployer/xdb/xdb.py
+-rw-r--r--  2.0 unx    11358 b- defN 23-Apr-26 08:21 pxd-0.5.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4541 b- defN 23-Apr-26 08:21 pxd-0.5.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-26 08:21 pxd-0.5.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       73 b- defN 23-Apr-26 08:21 pxd-0.5.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 23-Apr-26 08:21 pxd-0.5.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     5101 b- defN 23-Apr-26 08:21 pxd-0.5.3.dist-info/RECORD
+60 files, 223594 bytes uncompressed, 71728 bytes compressed:  67.9%
```

## zipnote {}

```diff
@@ -156,26 +156,26 @@
 
 Filename: deployer/xdb/__init__.py
 Comment: 
 
 Filename: deployer/xdb/xdb.py
 Comment: 
 
-Filename: pxd-0.5.1.dist-info/LICENSE
+Filename: pxd-0.5.3.dist-info/LICENSE
 Comment: 
 
-Filename: pxd-0.5.1.dist-info/METADATA
+Filename: pxd-0.5.3.dist-info/METADATA
 Comment: 
 
-Filename: pxd-0.5.1.dist-info/WHEEL
+Filename: pxd-0.5.3.dist-info/WHEEL
 Comment: 
 
-Filename: pxd-0.5.1.dist-info/entry_points.txt
+Filename: pxd-0.5.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: pxd-0.5.1.dist-info/top_level.txt
+Filename: pxd-0.5.3.dist-info/top_level.txt
 Comment: 
 
-Filename: pxd-0.5.1.dist-info/RECORD
+Filename: pxd-0.5.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## deployer/version.txt

```diff
@@ -1,2 +1,4 @@
 [default]
-version=0.5.1
+version = 0.5.3
+commit = dbdb8ed
+
```

## deployer/config/config.py

```diff
@@ -25,15 +25,15 @@
 
 class Config:
     _instance = None
 
     DOCKER_REPO_URL = "polardbx/"
 
     CN_IMAGE_NAME = "polardbx-sql"
-    DN_IMAGE_NAME = "polardbx-engine"
+    DN_IMAGE_NAME = "polardbx-engine-2.0"
     CDC_IMAGE_NAME = "polardbx-cdc"
 
     CN_IMAGE_VERSION = 'latest'
     DN_IMAGE_VERSION = "latest"
     CDC_IMAGE_VERSION = "latest"
 
     CN_TOOL_IMAGE_NAME = "polardbx-init"
```

## deployer/pxc/polardbx_cluster.py

```diff
@@ -384,17 +384,18 @@
                         "data_id, status, op_version, extras) " \
                         "VALUES (NULL, NOW(), NOW(), '%s', 0, 0, NULL);" % PRIVILEGE_INFO_DATA_ID)
 
         sql_list.append(f"insert into inst_config (inst_id, param_key,param_val) "
                         f"values ('{self.pxc_name}','CONN_POOL_XPROTO_META_DB_PORT',"
                         f"'0')")
 
+        cdc_startup_mode = '1' if self.cdc_replica > 0 else '0'
         sql_list.append(f"insert into inst_config (inst_id, param_key,param_val) "
                         f"values ('{self.pxc_name}','CDC_STARTUP_MODE',"
-                        f"'0')")
+                        f"'{cdc_startup_mode}')")
 
         for (key, value) in CN_DEFAULT_PARAMS.items():
             sql_list.append(f"replace into inst_config (inst_id, param_key,param_val) "
                             f"values ('{self.pxc_name}','{key}',"
                             f"'{value}')")
         MySQLManager.execute_update(self.gms, sql_list)
 
@@ -854,15 +855,15 @@
         container.remove(v=True, force=True)
     except docker.errors.NotFound:
         click.echo('container: %s is not existing at %s.' % (container_id, host))
 
 
 def rm_volumes_if_needed(host, volumes):
     for dir in volumes.keys():
-        if "mysql" not in dir and "shared" not in dir:
+        if "mysql" not in dir and "shared" not in dir and "polarx"  not in dir:
             continue
         if FileManager.exists(host, dir):
             logger.info("rm directory: %s at: %s" % (dir, host))
             FileManager.rmdir(host, dir)
 
 
 def exec_cmd_for_cn(host, container_name, container_id, cmd):
```

## deployer/pxc/polardbx_manager.py

```diff
@@ -93,8 +93,9 @@
 
 
 def print_pxd_version():
     Config.instance().load_config()
     version_file = repo_dir.joinpath("deployer/version.txt")
     config = configparser.RawConfigParser()
     config.read(version_file)
-    click.echo('pxd version: ' + config.get('default', 'version'))
+    click.echo('pxd version: ' + config.get('default', 'version').strip())
+    click.echo('commit id: ' + config.get('default', 'commit').strip())
```

## deployer/util/file_manager.py

```diff
@@ -16,15 +16,14 @@
 import shutil
 
 import spur
 import spurplus
 
 from deployer.config.config import Config
 
-
 def _is_localhost(host):
     return host == '127.0.0.1' or host == 'localhost'
 
 
 """
 This is a util class to handle file operation.
 If host is local, directly access file, otherwise access remote file based on Paramiko
```

## deployer/xdb/xdb.py

```diff
@@ -219,14 +219,15 @@
                 logger.info("%s" % log)
 
     @xdb_create_task(task_name='start xdb containers')
     def _start_xdb_container(self):
         for node in self.nodes:
             volumes = self._generate_xdb_volumes(node)
             self._create_volume_dirs_if_needed(volumes)
+            volumes.update(self._generate_system_volumes())
             self._write_pod_info(node)
             ports = self._generate_xdb_export_ports(node)
             command = self._generate_xdb_container_command()
             mem_limit = self._generate_xdb_node_mem_limit(node)
             env = self._generate_xdb_env(node)
             client = DockerManager.get_client(node.host)
             if Config.instance().host_network_support():
@@ -272,14 +273,20 @@
             data_dir: {'bind': '/data/mysql', 'mode': 'rw'},
             shared_channel_file: {'bind': '/data/shared', 'mode': 'ro'},
             template_dir: {'bind': '/data/template', 'mode': 'ro'},
             podinfo_dir: {'bind': '/etc/podinfo', 'mode': 'ro'},
             mysqllog_dir: {'bind': '/data/mysql-log', 'mode': 'rw'}
         }
 
+    def _generate_system_volumes(self):
+        return {
+            '/etc/localtime': {'bind': '/etc/localtime', 'mode': 'ro'},
+            '/usr/share/zoneinfo': {'bind': '/usr/share/zoneinfo', 'mode': 'ro'},
+        }
+
     def _create_volume_dirs_if_needed(self, volumes):
         for host in self.hosts:
             FileManager.mkdirs(host, volumes.keys())
 
     def _generate_xdb_node_mem_limit(self, node):
         if node.role == 'Logger':
             return min(int(self.mem_limit), constant.LOGGER_MAX_MEM)
```

## Comparing `pxd-0.5.1.dist-info/LICENSE` & `pxd-0.5.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pxd-0.5.1.dist-info/METADATA` & `pxd-0.5.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pxd
-Version: 0.5.1
+Version: 0.5.3
 Summary: This is a tool to download and install PolarDB-X
 Home-page: UNKNOWN
 Author: polardbx
 Author-email: vettal.wd@alibaba-inc.com
 License: UNKNOWN
 Platform: all
 Classifier: Programming Language :: Python
```

## Comparing `pxd-0.5.1.dist-info/RECORD` & `pxd-0.5.3.dist-info/RECORD`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 deployer/__init__.py,sha256=KOPBclqMVKfeguAHku6DZHy0C95GLGko03sSt87DBaY,622
 deployer/_repo.py,sha256=VMggl-rwEKx9t-J_GI9RG4qLj2SaXKiAmAxj1coEzkE,790
 deployer/logging.yaml,sha256=2LLVJUa2gjfxf-WZT9l2doNyMflxftLJ0TaKa2L5A9I,733
 deployer/pxd.py,sha256=j7pyz90LHKlZcc-ic89otv_tcRsS0CJM9iOw-NORff0,6887
-deployer/version.txt,sha256=Zw0qtL8Dpw1r2cI2DtwSILzL9Wz1bovfi4Kdq5ZYa58,23
+deployer/version.txt,sha256=UP85xPZtgR4IVBTEKjZZG8ENLk_HN2tvVmm89Klx2kM,44
 deployer/config/__init__.py,sha256=KOPBclqMVKfeguAHku6DZHy0C95GLGko03sSt87DBaY,622
-deployer/config/config.py,sha256=P-PbBaRKB2rfgDZgT0xD-5kwRVVGwXptCYZxfH9cFqc,5304
+deployer/config/config.py,sha256=vJbXoOnUAfGcKWX2iMH4nvRCF0tkZraZsvP9Cqum9Bk,5308
 deployer/config/log_config.py,sha256=wOyxszPQtN4i--ePMSU2MNUm6KW8IYfA0rMSRezTTyo,1313
 deployer/config/metadb_config.py,sha256=Uv4M1azARRYIk09qPD4AXZgzFNzNLm4h2d0AEdEMsks,1080
 deployer/constant/__init__.py,sha256=KOPBclqMVKfeguAHku6DZHy0C95GLGko03sSt87DBaY,622
 deployer/constant/constant.py,sha256=z39ZTUSAw6H1BJHjs6ixtL1y9Zc-EhFgx2tgTh90xQM,1195
 deployer/constant/table_field.py,sha256=qcrYPTeJbz-rhAhxqhlbLz0hA-LPakLplHqkweAlqEc,715
 deployer/core/__init__.py,sha256=KOPBclqMVKfeguAHku6DZHy0C95GLGko03sSt87DBaY,622
 deployer/core/context.py,sha256=19Jf75z0vmu5Q27QnkzCo6PXVEXCgI8Mrr9Yff8Fw5g,991
@@ -19,16 +19,16 @@
 deployer/decorator/decorators.py,sha256=dlGmBdzoAmuIu4cabsv0l4RKRzNY0R0uRGqDNr625eU,2202
 deployer/download/__init__.py,sha256=KOPBclqMVKfeguAHku6DZHy0C95GLGko03sSt87DBaY,622
 deployer/download/constant.py,sha256=r8PAS4deCjpPqxukj5v2txr7HVpaQeF--Pzmgfb15Io,1219
 deployer/download/polardbx_download.py,sha256=bU4NQ4YJ97djyy7mb9M1JRMJB6emDRTN24KW0Q28bO0,10463
 deployer/pcn/__init__.py,sha256=KOPBclqMVKfeguAHku6DZHy0C95GLGko03sSt87DBaY,622
 deployer/pxc/__init__.py,sha256=KOPBclqMVKfeguAHku6DZHy0C95GLGko03sSt87DBaY,622
 deployer/pxc/gms_consts.py,sha256=swwK1mhn7-uHWcXNilbm0efksyumoYszkwyP79BoD9Y,1070
-deployer/pxc/polardbx_cluster.py,sha256=sxMMQbtBLsUFQbxEzduw-IWiPXqMnmWDfwzhBO8IrLQ,42120
-deployer/pxc/polardbx_manager.py,sha256=qAlcYip6GKha5lGQ2930XU7tVNofeJZKWgLCJEAwSfM,3944
+deployer/pxc/polardbx_cluster.py,sha256=ZXvMHSEGLjBkgyM4hlBm5-Q5q_fmmzo8VF1sZBxpAmQ,42226
+deployer/pxc/polardbx_manager.py,sha256=j0BkFx4JdmzVA1um4tdi7Ry_sf-3uUDbT6Awqy-FqM4,4024
 deployer/pxc/polardbx_topology.py,sha256=Bb3sUS25ZczHb8MVVE3CgskBOxJC8MH7NO9ubQhLFvc,930
 deployer/pxc/pxc_user.py,sha256=cNmzwcib2t3Bdx2NTgMfQy-brNnFfya-wyTrPk7cSk4,1257
 deployer/resources/__init__.py,sha256=KOPBclqMVKfeguAHku6DZHy0C95GLGko03sSt87DBaY,622
 deployer/resources/download/scripts/load_image.sh,sha256=X7ZheHT5dCfyndmfp0ZV_MDWICy0-pu9ZSAhfdXYqiQ,260
 deployer/resources/sql/gms_init.sql,sha256=i_z249y27cMYewtS72cemWcKF0X6FlGk9c7vid_20xs,7330
 deployer/resources/sql/sqlite_init.sql,sha256=aRlR_zoiAio4NXz385WfrCz2nVy647f3VpP6YDfqbbk,2137
 deployer/resources/template/my-8.0.cnf,sha256=4Z2L1g97__AF-Eb-eEzNeeZCcRX8N2da-tUqTFMHbVU,4872
@@ -40,21 +40,21 @@
 deployer/sqlite/__init__.py,sha256=KOPBclqMVKfeguAHku6DZHy0C95GLGko03sSt87DBaY,622
 deployer/sqlite/dbapi.py,sha256=gsQnJOAxa4OB6bXk97LpthkyV5Xz5FJBcfnjs4Czejw,5922
 deployer/sqlite/sqlite_manager.py,sha256=XAUuhQWIg_JSiKmaYwoMKMReoE0mP5QAZoGsbIO4Sy0,3181
 deployer/tests/__init__.py,sha256=KOPBclqMVKfeguAHku6DZHy0C95GLGko03sSt87DBaY,622
 deployer/tryout/__init__.py,sha256=KOPBclqMVKfeguAHku6DZHy0C95GLGko03sSt87DBaY,622
 deployer/tryout/install.py,sha256=lSrL_WYbfmiFIHwlVG0yvBNj6JuKwBqmQxenH5Vol6M,1201
 deployer/util/__init__.py,sha256=KOPBclqMVKfeguAHku6DZHy0C95GLGko03sSt87DBaY,622
-deployer/util/file_manager.py,sha256=s1fAaivhPRf-TYs3kOsC_u4KA0SLTfFLbKWyWcCSTX4,3579
+deployer/util/file_manager.py,sha256=aquq6ALCZJSsQv4gEBMJRmldf3YgpGEgp0VDLxveyP0,3578
 deployer/util/mysql_manager.py,sha256=TRnHe70bIjGbEnFsGjQAc9MY9wUMvRrFI7CFHRFUR4Q,2110
 deployer/util/network_util.py,sha256=n1vT1RicjJ3Mb75ygZq8yzgYBOS60XXjKyLmKNok_co,784
 deployer/util/password_util.py,sha256=Qcxr2kJ0gOA5Z2NO50m0NTt05v6gbwnM5WE1cUyIMXM,1494
 deployer/util/sqlite_manager.py,sha256=8_ZvNi0UGBHyhJfngb0PYr_fA3_Wgp_jXqNkXSvqSO4,2376
 deployer/util/yaml_util.py,sha256=ndvgjVg0op0fU4p-Yk38rLnniRTK-Z2F0s4bOgFw6vA,2585
 deployer/xdb/__init__.py,sha256=KOPBclqMVKfeguAHku6DZHy0C95GLGko03sSt87DBaY,622
-deployer/xdb/xdb.py,sha256=djmRho2KToW8FeQuLzvdSWDs-TPKSLCsy_WjjtiLTB0,22187
-pxd-0.5.1.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
-pxd-0.5.1.dist-info/METADATA,sha256=HrkED_gvnOm1YPb7V6vDnAd5ARD7bf68YVbnHRhjK1g,4541
-pxd-0.5.1.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-pxd-0.5.1.dist-info/entry_points.txt,sha256=CX2PKoQHoIv95UwHGVgCkAjTqK27EjXv6mb1v2l16U4,73
-pxd-0.5.1.dist-info/top_level.txt,sha256=TwI8aV0C_V0Au2_1ouGA25hHdF5_e7_RjipVDY1w0lk,9
-pxd-0.5.1.dist-info/RECORD,,
+deployer/xdb/xdb.py,sha256=fjwFHi9rgrsLhuCXyXX9uCczJCft6l1jFe9Rkr5r0SI,22469
+pxd-0.5.3.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
+pxd-0.5.3.dist-info/METADATA,sha256=FyILey8t02tJxrlj5xiZb9A4KVC6q5kVamLna9cnpDU,4541
+pxd-0.5.3.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+pxd-0.5.3.dist-info/entry_points.txt,sha256=CX2PKoQHoIv95UwHGVgCkAjTqK27EjXv6mb1v2l16U4,73
+pxd-0.5.3.dist-info/top_level.txt,sha256=TwI8aV0C_V0Au2_1ouGA25hHdF5_e7_RjipVDY1w0lk,9
+pxd-0.5.3.dist-info/RECORD,,
```

