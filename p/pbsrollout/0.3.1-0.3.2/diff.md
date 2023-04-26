# Comparing `tmp/pbsrollout-0.3.1.tar.gz` & `tmp/pbsrollout-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pbsrollout-0.3.1.tar", max compression
+gzip compressed data, was "pbsrollout-0.3.2.tar", max compression
```

## Comparing `pbsrollout-0.3.1.tar` & `pbsrollout-0.3.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0        0 2022-07-21 03:13:41.658475 pbsrollout-0.3.1/LICENSE
--rw-r--r--   0        0        0        0 2022-07-14 16:06:49.043912 pbsrollout-0.3.1/pbsrollout/__init__.py
--rw-r--r--   0        0        0        0 2023-04-05 21:41:28.936936 pbsrollout-0.3.1/pbsrollout/internal/__init__.py
--rw-r--r--   0        0        0     1231 2023-04-13 22:21:13.072224 pbsrollout-0.3.1/pbsrollout/internal/aws_utils.py
--rw-r--r--   0        0        0     2829 2023-04-05 21:42:20.098114 pbsrollout-0.3.1/pbsrollout/internal/check_cluster_ready.py
--rw-r--r--   0        0        0     3733 2023-02-23 22:56:56.612903 pbsrollout-0.3.1/pbsrollout/internal/k8s_utils.py
--rw-r--r--   0        0        0     9181 2023-04-05 21:42:20.105536 pbsrollout-0.3.1/pbsrollout/internal/process_cluster.py
--rw-r--r--   0        0        0      208 2023-04-13 22:19:08.544564 pbsrollout-0.3.1/pbsrollout/internal/test_aws_utils.py
--rw-r--r--   0        0        0     1217 2023-04-05 21:42:20.110740 pbsrollout-0.3.1/pbsrollout/internal/test_k8s_utils.py
--rw-r--r--   0        0        0      444 2023-04-05 21:42:20.121783 pbsrollout-0.3.1/pbsrollout/internal/test_process_cluster.py
--rw-r--r--   0        0        0      925 2022-07-27 23:18:57.505345 pbsrollout-0.3.1/pbsrollout/internal/utils.py
--rw-r--r--   0        0        0     4667 2023-04-17 22:04:49.560368 pbsrollout-0.3.1/pbsrollout/main.py
--rw-r--r--   0        0        0        0 2023-04-05 21:40:57.190004 pbsrollout-0.3.1/pbsrollout/pbs_release/__init__.py
--rw-r--r--   0        0        0     9374 2023-04-05 21:59:04.793955 pbsrollout-0.3.1/pbsrollout/pbs_release/main_view.py
--rw-r--r--   0        0        0        0 2023-04-05 21:40:57.190004 pbsrollout-0.3.1/pbsrollout/stg_release/__init__.py
--rw-r--r--   0        0        0     5907 2023-04-13 22:27:23.574087 pbsrollout-0.3.1/pbsrollout/stg_release/main_view.py
--rw-r--r--   0        0        0      522 2023-04-17 22:05:10.459171 pbsrollout-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      649 1970-01-01 00:00:00.000000 pbsrollout-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2022-07-21 03:13:41.658475 pbsrollout-0.3.2/LICENSE
+-rw-r--r--   0        0        0        0 2022-07-14 16:06:49.043912 pbsrollout-0.3.2/pbsrollout/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-05 21:41:28.936936 pbsrollout-0.3.2/pbsrollout/internal/__init__.py
+-rw-r--r--   0        0        0     1231 2023-04-13 22:21:13.072224 pbsrollout-0.3.2/pbsrollout/internal/aws_utils.py
+-rw-r--r--   0        0        0     2829 2023-04-05 21:42:20.098114 pbsrollout-0.3.2/pbsrollout/internal/check_cluster_ready.py
+-rw-r--r--   0        0        0     3733 2023-02-23 22:56:56.612903 pbsrollout-0.3.2/pbsrollout/internal/k8s_utils.py
+-rw-r--r--   0        0        0     9181 2023-04-05 21:42:20.105536 pbsrollout-0.3.2/pbsrollout/internal/process_cluster.py
+-rw-r--r--   0        0        0      208 2023-04-13 22:19:08.544564 pbsrollout-0.3.2/pbsrollout/internal/test_aws_utils.py
+-rw-r--r--   0        0        0     1217 2023-04-05 21:42:20.110740 pbsrollout-0.3.2/pbsrollout/internal/test_k8s_utils.py
+-rw-r--r--   0        0        0      444 2023-04-05 21:42:20.121783 pbsrollout-0.3.2/pbsrollout/internal/test_process_cluster.py
+-rw-r--r--   0        0        0      925 2022-07-27 23:18:57.505345 pbsrollout-0.3.2/pbsrollout/internal/utils.py
+-rw-r--r--   0        0        0     4667 2023-04-17 22:04:49.560368 pbsrollout-0.3.2/pbsrollout/main.py
+-rw-r--r--   0        0        0        0 2023-04-05 21:40:57.190004 pbsrollout-0.3.2/pbsrollout/pbs_release/__init__.py
+-rw-r--r--   0        0        0     9374 2023-04-05 21:59:04.793955 pbsrollout-0.3.2/pbsrollout/pbs_release/main_view.py
+-rw-r--r--   0        0        0        0 2023-04-05 21:40:57.190004 pbsrollout-0.3.2/pbsrollout/stg_release/__init__.py
+-rw-r--r--   0        0        0     5927 2023-04-25 16:48:05.489162 pbsrollout-0.3.2/pbsrollout/stg_release/main_view.py
+-rw-r--r--   0        0        0      522 2023-04-25 16:49:47.310209 pbsrollout-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      649 1970-01-01 00:00:00.000000 pbsrollout-0.3.2/PKG-INFO
```

### Comparing `pbsrollout-0.3.1/pbsrollout/internal/aws_utils.py` & `pbsrollout-0.3.2/pbsrollout/internal/aws_utils.py`

 * *Files identical despite different names*

### Comparing `pbsrollout-0.3.1/pbsrollout/internal/check_cluster_ready.py` & `pbsrollout-0.3.2/pbsrollout/internal/check_cluster_ready.py`

 * *Files identical despite different names*

### Comparing `pbsrollout-0.3.1/pbsrollout/internal/k8s_utils.py` & `pbsrollout-0.3.2/pbsrollout/internal/k8s_utils.py`

 * *Files identical despite different names*

### Comparing `pbsrollout-0.3.1/pbsrollout/internal/process_cluster.py` & `pbsrollout-0.3.2/pbsrollout/internal/process_cluster.py`

 * *Files identical despite different names*

### Comparing `pbsrollout-0.3.1/pbsrollout/internal/test_k8s_utils.py` & `pbsrollout-0.3.2/pbsrollout/internal/test_k8s_utils.py`

 * *Files identical despite different names*

### Comparing `pbsrollout-0.3.1/pbsrollout/internal/utils.py` & `pbsrollout-0.3.2/pbsrollout/internal/utils.py`

 * *Files identical despite different names*

### Comparing `pbsrollout-0.3.1/pbsrollout/main.py` & `pbsrollout-0.3.2/pbsrollout/main.py`

 * *Files identical despite different names*

### Comparing `pbsrollout-0.3.1/pbsrollout/pbs_release/main_view.py` & `pbsrollout-0.3.2/pbsrollout/pbs_release/main_view.py`

 * *Files identical despite different names*

### Comparing `pbsrollout-0.3.1/pbsrollout/stg_release/main_view.py` & `pbsrollout-0.3.2/pbsrollout/stg_release/main_view.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     menu_entry_index = terminal_menu.show()
     tag = images[menu_entry_index]
 
     # put it in the file
     dir_path = go_path + '/src/github.com/publica-project/prebid-kube-manifests/namespace/stg/'
     for stg in stg_idx:
         console.print(f"Updating tag to [bold blue_violet]{tag}[/bold blue_violet] in file:")
-        for pod in ['pod', 'logger', 'console-api']:
+        for pod in ['pbs', 'logger', 'console-api']:
             tag_file_path = dir_path + f"z{stg}-{pod}.tag"
             console.print(f"[bold light_steel_blue1]{tag_file_path}[/bold light_steel_blue1]")
             with open(tag_file_path, "w") as f:
                 f.write(tag)
 
     # step 2: release pods
     for stg in stg_idx:
@@ -96,15 +96,15 @@
 def sync_staging_db(console: Console, stg_idx: List[str], go_path: str):
     for stg in stg_idx:
         dir_path = go_path + '/src/github.com/publica-project/prebid-kube-manifests/aws.us-east-1-eks-27-v3/'
         with Dir(dir_path):
             print(f'\tSyncing staging db for stg: {stg}')
             # run make clean deploy-new-pbs-prod
             cmd = f"direnv exec . ../scripts/sync-staging-db {stg.lstrip('0')}"
-            ret = subprocess.run(cmd.split(" "), stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True, timeout=90)
+            ret = subprocess.run(cmd.split(" "), stderr=subprocess.PIPE, text=True, timeout=90)
             ret.stderr = clean_stderr(ret.stderr)
             if ret.returncode != 0 or ret.stderr != "":
                 print_error_body(f"ERROR:\n\nstdout:\n{ret.stdout}\nstderr:\n{ret.stderr}")
                 return False
 
 
 def choose_another_staging_idx(console: Console, stg_idx: List[str], go_path: str) -> List[str]:
@@ -126,13 +126,14 @@
     stg_idx = choose_staging_idx(console)
     while True:
         terminal_menu = TerminalMenu([o[0] for o in actions],
                                      title=f"What do you want to do for staging: {' '.join(stg_idx)}?",
                                      raise_error_on_interrupt=True)
         menu_entry_index = terminal_menu.show()
 
-        if actions[menu_entry_index][0] == 'exit':
+        if actions[menu_entry_index][0] == '' \
+                                           '':
             return
 
         ret = actions[menu_entry_index][1](console, stg_idx, go_path)
         if actions[menu_entry_index][0] == 'choose another staging idx':
             stg_idx = ret
```

### Comparing `pbsrollout-0.3.1/pyproject.toml` & `pbsrollout-0.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pbsrollout"
-version = "0.3.1"
+version = "0.3.2"
 description = ""
 authors = ["dimitri <dimitriwyzlic@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 shellpy = "^0.5.1"
 kubernetes = "^24.2.0"
```

### Comparing `pbsrollout-0.3.1/PKG-INFO` & `pbsrollout-0.3.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pbsrollout
-Version: 0.3.1
+Version: 0.3.2
 Summary: 
 Author: dimitri
 Author-email: dimitriwyzlic@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

