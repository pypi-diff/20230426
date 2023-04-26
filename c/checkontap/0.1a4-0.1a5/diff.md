# Comparing `tmp/checkontap-0.1a4.tar.gz` & `tmp/checkontap-0.1a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "checkontap-0.1a4.tar", last modified: Mon Apr 24 14:10:37 2023, max compression
+gzip compressed data, was "checkontap-0.1a5.tar", last modified: Wed Apr 26 14:34:00 2023, max compression
```

## Comparing `checkontap-0.1a4.tar` & `checkontap-0.1a5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      223 2023-03-23 09:02:45.881436 checkontap-0.1a4/README.md
--rw-r--r--   0        0        0      926 2023-03-22 16:30:38.341339 checkontap-0.1a4/checkontap/__init__.py
--rw-r--r--   0        0        0     3431 2023-03-23 14:53:12.575066 checkontap-0.1a4/checkontap/cli.py
--rw-r--r--   0        0        0      756 2023-03-22 16:09:15.025609 checkontap-0.1a4/checkontap/ontapcmd/__init__.py
--rw-r--r--   0        0        0     2227 2023-04-21 14:48:25.623996 checkontap-0.1a4/checkontap/ontapcmd/about.py
--rw-r--r--   0        0        0     6945 2023-04-21 14:48:51.992608 checkontap-0.1a4/checkontap/ontapcmd/aggregateusage.py
--rw-r--r--   0        0        0     2894 2023-04-21 14:49:01.363591 checkontap-0.1a4/checkontap/ontapcmd/clusterhealth.py
--rw-r--r--   0        0        0     7694 2023-04-21 14:49:13.743682 checkontap-0.1a4/checkontap/ontapcmd/diskhealth.py
--rw-r--r--   0        0        0     4509 2023-04-21 14:49:23.573489 checkontap-0.1a4/checkontap/ontapcmd/hardwarehealth.py
--rw-r--r--   0        0        0     3875 2023-04-24 12:40:05.504428 checkontap-0.1a4/checkontap/ontapcmd/interfacehealth.py
--rw-r--r--   0        0        0     4994 2023-04-21 14:49:47.394778 checkontap-0.1a4/checkontap/ontapcmd/lunusage.py
--rw-r--r--   0        0        0     5079 2023-04-21 14:49:57.522947 checkontap-0.1a4/checkontap/ontapcmd/volumehealth.py
--rw-r--r--   0        0        0     8126 2023-04-21 14:48:07.213286 checkontap-0.1a4/checkontap/ontapcmd/volumeusage.py
--rw-r--r--   0        0        0      757 2023-03-22 16:09:25.201105 checkontap-0.1a4/checkontap/tools/__init__.py
--rw-r--r--   0        0        0     9543 2023-04-21 14:46:55.901090 checkontap-0.1a4/checkontap/tools/cli.py
--rw-r--r--   0        0        0     3108 2023-04-24 12:07:20.737893 checkontap-0.1a4/checkontap/tools/helper.py
--rw-r--r--   0        0        0      857 2023-04-24 14:04:36.718273 checkontap-0.1a4/pyproject.toml
--rw-r--r--   0        0        0      893 1970-01-01 00:00:00.000000 checkontap-0.1a4/PKG-INFO
+-rw-r--r--   0        0        0      223 2023-03-23 09:02:45.881436 checkontap-0.1a5/README.md
+-rw-r--r--   0        0        0      926 2023-03-22 16:30:38.341339 checkontap-0.1a5/checkontap/__init__.py
+-rw-r--r--   0        0        0     3431 2023-03-23 14:53:12.575066 checkontap-0.1a5/checkontap/cli.py
+-rw-r--r--   0        0        0      756 2023-03-22 16:09:15.025609 checkontap-0.1a5/checkontap/ontapcmd/__init__.py
+-rw-r--r--   0        0        0     2227 2023-04-21 14:48:25.623996 checkontap-0.1a5/checkontap/ontapcmd/about.py
+-rw-r--r--   0        0        0     6945 2023-04-21 14:48:51.992608 checkontap-0.1a5/checkontap/ontapcmd/aggregateusage.py
+-rw-r--r--   0        0        0     2886 2023-04-26 14:31:12.533831 checkontap-0.1a5/checkontap/ontapcmd/clusterhealth.py
+-rw-r--r--   0        0        0     7694 2023-04-21 14:49:13.743682 checkontap-0.1a5/checkontap/ontapcmd/diskhealth.py
+-rw-r--r--   0        0        0     4509 2023-04-21 14:49:23.573489 checkontap-0.1a5/checkontap/ontapcmd/hardwarehealth.py
+-rw-r--r--   0        0        0     3875 2023-04-24 12:40:05.504428 checkontap-0.1a5/checkontap/ontapcmd/interfacehealth.py
+-rw-r--r--   0        0        0     4994 2023-04-21 14:49:47.394778 checkontap-0.1a5/checkontap/ontapcmd/lunusage.py
+-rw-r--r--   0        0        0     5079 2023-04-21 14:49:57.522947 checkontap-0.1a5/checkontap/ontapcmd/volumehealth.py
+-rw-r--r--   0        0        0     8463 2023-04-26 12:55:43.724726 checkontap-0.1a5/checkontap/ontapcmd/volumeusage.py
+-rw-r--r--   0        0        0      757 2023-03-22 16:09:25.201105 checkontap-0.1a5/checkontap/tools/__init__.py
+-rw-r--r--   0        0        0     9565 2023-04-26 13:06:26.630474 checkontap-0.1a5/checkontap/tools/cli.py
+-rw-r--r--   0        0        0     3108 2023-04-24 12:07:20.737893 checkontap-0.1a5/checkontap/tools/helper.py
+-rw-r--r--   0        0        0      857 2023-04-26 14:32:23.061640 checkontap-0.1a5/pyproject.toml
+-rw-r--r--   0        0        0      893 1970-01-01 00:00:00.000000 checkontap-0.1a5/PKG-INFO
```

### Comparing `checkontap-0.1a4/checkontap/__init__.py` & `checkontap-0.1a5/checkontap/__init__.py`

 * *Files identical despite different names*

### Comparing `checkontap-0.1a4/checkontap/cli.py` & `checkontap-0.1a5/checkontap/cli.py`

 * *Files identical despite different names*

### Comparing `checkontap-0.1a4/checkontap/ontapcmd/__init__.py` & `checkontap-0.1a5/checkontap/ontapcmd/__init__.py`

 * *Files identical despite different names*

### Comparing `checkontap-0.1a4/checkontap/ontapcmd/about.py` & `checkontap-0.1a5/checkontap/ontapcmd/about.py`

 * *Files identical despite different names*

### Comparing `checkontap-0.1a4/checkontap/ontapcmd/aggregateusage.py` & `checkontap-0.1a5/checkontap/ontapcmd/aggregateusage.py`

 * *Files identical despite different names*

### Comparing `checkontap-0.1a4/checkontap/ontapcmd/clusterhealth.py` & `checkontap-0.1a5/checkontap/ontapcmd/clusterhealth.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,49 +25,49 @@
 __cmd__ = "cluster-health"
 
 """
 """
 def run():
     parser = cli.Parser()
     args = parser.get_args()
-    # Setup module logging 
+    # Setup module logging
     logger = logging.getLogger(__name__)
     logger.disabled=True
     if args.verbose:
         for log_name, log_obj in logging.Logger.manager.loggerDict.items():
             log_obj.disabled = False
             logging.getLogger(log_name).setLevel(severity(args.verbose))
 
     setup_connection(args.host, args.api_user, args.api_pass)
-    
+
     check = Check()
     # Cluster global state
     try:
         cluster = Cluster()
         cluster.get(fields="name,metric,version")
         logger.debug(f"Cluster info \n{cluster.__dict__}")
-        if 'ok' in cluster.metric.status:
-            check.add_message(Status.OK, "{}".format(cluster.version.full))
-        else:
+        if 'ok' not in cluster.metric.status.lower():
             check.add_message(Status.CRITICAL,"Cluster global status is {}".format(cluster.metric.status))
     except NetAppRestError as error:
         check.exit(Status.UNKNOWN, "Error => {}".format(error.http_err_response.http_response.text))
 
     # Cluster node states
+    Nodes = list(Node.get_collection(fields="name,state,membership,ha"))
     try:
-        for node in Node.get_collection(fields="name,state,membership,ha"):
+        for node in Nodes:
             logger.debug(f"Node info \n{node.__dict__}")
             m = "{} state {} as {}; giveback: {}; takeover: {}".format(node.name,node.state,node.membership,node.ha.giveback.state,node.ha.takeover.state)
-            if 'up' in node.state: 
+            if 'up' in node.state:
                 check.add_message(Status.OK, m)
             elif 'down' in node.state:
                 check.add_message(Status.CRITICAL, m)
             else:
                 check.add_message(Status.WARNING, m)
     except NetAppRestError as error:
         check.exit(Status.UNKNOWN, "Error => {}".format(error.http_err_response.http_response.text))
-    
+
+    short = f"Checked {len(Nodes)} Nodes"
     (code, message) = check.check_messages(separator="\n")
-    check.exit(code=code,message=message)
+    check.exit(code=code,message=f"{short}\n{message}")
 
 if __name__ == "__main__":
     run()
```

### Comparing `checkontap-0.1a4/checkontap/ontapcmd/diskhealth.py` & `checkontap-0.1a5/checkontap/ontapcmd/diskhealth.py`

 * *Files identical despite different names*

### Comparing `checkontap-0.1a4/checkontap/ontapcmd/hardwarehealth.py` & `checkontap-0.1a5/checkontap/ontapcmd/hardwarehealth.py`

 * *Files identical despite different names*

### Comparing `checkontap-0.1a4/checkontap/ontapcmd/interfacehealth.py` & `checkontap-0.1a5/checkontap/ontapcmd/interfacehealth.py`

 * *Files identical despite different names*

### Comparing `checkontap-0.1a4/checkontap/ontapcmd/lunusage.py` & `checkontap-0.1a5/checkontap/ontapcmd/lunusage.py`

 * *Files identical despite different names*

### Comparing `checkontap-0.1a4/checkontap/ontapcmd/volumehealth.py` & `checkontap-0.1a5/checkontap/ontapcmd/volumehealth.py`

 * *Files identical despite different names*

### Comparing `checkontap-0.1a4/checkontap/ontapcmd/volumeusage.py` & `checkontap-0.1a5/checkontap/ontapcmd/volumeusage.py`

 * *Files 11% similar despite different names*

```diff
@@ -107,31 +107,42 @@
 
     except NetAppRestError as error:
         check.exit(Status.UNKNOWN, "Error => {}".format(error.http_err_response.http_response.text))
 
     for vol in vols:
         v = {
             'name': f"{vol.svm.name}_{vol.name}",
-            'data_total': vol.space.afs_total,
             'space': {
                 'max': vol.space.size,
                 'used': vol.space.used,
                 'pct': to_percent(vol.space.size, vol.space.used)
             },
             'inodes': {
                 'max': vol.files.maximum,
                 'used': vol.files.used,
                 'pct': to_percent(vol.files.maximum, vol.files.used)
             },
-            'snapshot': {
+        }
+        if hasattr(vol.space, 'afs_total'):
+            v['data_total'] = vol.space.afs_total
+        else:
+            v['data_total'] = vol.space.size
+        if hasattr(vol.space.snapshot, 'reserve_size'):
+            v['snapshot'] = {
                 'max': vol.space.snapshot.reserve_size,
                 'used': vol.space.snapshot.used,
                 'pct': to_percent(vol.space.snapshot.reserve_size, vol.space.snapshot.used)
             }
-        }
+        else:
+            v['snapshot'] = {
+                'max': 0,
+                'used': vol.space.snapshot.used,
+                'pct': 0
+            }
+            
         # unchecked perfdata
         check.add_perfmultidata(v['name'], 'volume_usage', label="data_total",value=v['data_total'], uom="B")
         # Volume usage
         t = {}
         if args.unit and '%' in args.unit:
             t['warning'] = percent_to(v['space']['max'],args.warning)
             t['critical'] = percent_to(v['space']['max'],args.critical)
```

### Comparing `checkontap-0.1a4/checkontap/tools/__init__.py` & `checkontap-0.1a5/checkontap/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `checkontap-0.1a4/checkontap/tools/cli.py` & `checkontap-0.1a5/checkontap/tools/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -224,31 +224,31 @@
             'help': 'add performance data to Output',
         }
     }
     INODE_WARN = {
         'name_or_flags': ['--inode-warning'],
         'options': {
             'action': 'store',
-            'help': 'Inode warning threshold in %'
+            'help': 'Inode warning threshold in percent'
         }
     }
     INODE_CRIT = {
         'name_or_flags': ['--inode-critical'],
         'options': {
             'action': 'store',
-            'help': 'Inode critical threshold in %',
+            'help': 'Inode critical threshold in percent'
         }
     }
     SNAP_WARN = {
         'name_or_flags': ['--snapshot-warning'],
         'options': {
             'action': 'store',
-            'help': 'Snapshot used space warning threshold in %'
+            'help': 'Snapshot used space warning threshold in percent'
         }
     }
     SNAP_CRIT = {
         'name_or_flags': ['--snapshot-critical'],
         'options': {
             'action': 'store',
-            'help': 'Snapshot used space critical threshold in %',
+            'help': 'Snapshot used space critical threshold in percent'
         }
     }
```

### Comparing `checkontap-0.1a4/checkontap/tools/helper.py` & `checkontap-0.1a5/checkontap/tools/helper.py`

 * *Files identical despite different names*

### Comparing `checkontap-0.1a4/pyproject.toml` & `checkontap-0.1a5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 build-backend = "flit_core.buildapi"
 requires = ["flit_core >=3.2,<4"]
 
 [project]
 name = "checkontap"
 readme = "README.md"
 description = "check_ontap monitoring plugin"
-version = "0.1a4"
+version = "0.1a5"
 requires-python = ">= 3.6"
 authors = [
     { name = "Matthias Gallinger", email = "matthias.gallinger@consol.de" }
 ]
 dependencies = [
     "netapp-ontap >= 9.11.1.0",
     "monplugin >= 0.5",
```

### Comparing `checkontap-0.1a4/PKG-INFO` & `checkontap-0.1a5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: checkontap
-Version: 0.1a4
+Version: 0.1a5
 Summary: check_ontap monitoring plugin
 Author-email: Matthias Gallinger <matthias.gallinger@consol.de>
 Requires-Python: >= 3.6
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: System :: Monitoring
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

