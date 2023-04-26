# Comparing `tmp/raga-cli-0.1.2.tar.gz` & `tmp/raga-cli-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raga-cli-0.1.2.tar", last modified: Tue Apr 25 11:58:15 2023, max compression
+gzip compressed data, was "raga-cli-0.1.3.tar", last modified: Wed Apr 26 13:57:32 2023, max compression
```

## Comparing `raga-cli-0.1.2.tar` & `raga-cli-0.1.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-25 11:58:15.063135 raga-cli-0.1.2/
--rw-r--r--   0 manabroy   (501) staff       (20)      741 2023-04-10 13:07:16.000000 raga-cli-0.1.2/.gitignore
--rw-r--r--   0 manabroy   (501) staff       (20)    11350 2023-04-10 13:07:16.000000 raga-cli-0.1.2/LICENSE
--rw-r--r--   0 manabroy   (501) staff       (20)      957 2023-04-25 11:58:15.062850 raga-cli-0.1.2/PKG-INFO
--rw-r--r--   0 manabroy   (501) staff       (20)        0 2023-04-10 13:07:16.000000 raga-cli-0.1.2/README.rst
--rw-r--r--   0 manabroy   (501) staff       (20)     2482 2023-04-25 11:57:59.000000 raga-cli-0.1.2/pyproject.toml
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-25 11:58:15.057372 raga-cli-0.1.2/raga_cli.egg-info/
--rw-r--r--   0 manabroy   (501) staff       (20)      957 2023-04-25 11:58:15.000000 raga-cli-0.1.2/raga_cli.egg-info/PKG-INFO
--rw-r--r--   0 manabroy   (501) staff       (20)      612 2023-04-25 11:58:15.000000 raga-cli-0.1.2/raga_cli.egg-info/SOURCES.txt
--rw-r--r--   0 manabroy   (501) staff       (20)        1 2023-04-25 11:58:15.000000 raga-cli-0.1.2/raga_cli.egg-info/dependency_links.txt
--rw-r--r--   0 manabroy   (501) staff       (20)       35 2023-04-25 11:58:15.000000 raga-cli-0.1.2/raga_cli.egg-info/entry_points.txt
--rw-r--r--   0 manabroy   (501) staff       (20)     1014 2023-04-25 11:58:15.000000 raga-cli-0.1.2/raga_cli.egg-info/requires.txt
--rw-r--r--   0 manabroy   (501) staff       (20)        3 2023-04-25 11:58:15.000000 raga-cli-0.1.2/raga_cli.egg-info/top_level.txt
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-25 11:58:15.058019 raga-cli-0.1.2/rc/
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-25 11:58:15.059229 raga-cli-0.1.2/rc/cli/
--rw-r--r--   0 manabroy   (501) staff       (20)     3473 2023-04-25 11:42:11.000000 raga-cli-0.1.2/rc/cli/__init__.py
--rw-r--r--   0 manabroy   (501) staff       (20)      292 2023-04-12 12:54:24.000000 raga-cli-0.1.2/rc/cli/command.py
--rw-r--r--   0 manabroy   (501) staff       (20)     2074 2023-04-12 11:10:34.000000 raga-cli-0.1.2/rc/cli/parser.py
--rw-r--r--   0 manabroy   (501) staff       (20)     9802 2023-04-25 07:39:29.000000 raga-cli-0.1.2/rc/cli/utils.py
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-25 11:58:15.060395 raga-cli-0.1.2/rc/commands/
--rw-r--r--   0 manabroy   (501) staff       (20)     3226 2023-04-10 13:07:16.000000 raga-cli-0.1.2/rc/commands/get.py
--rw-r--r--   0 manabroy   (501) staff       (20)     1634 2023-04-12 11:10:34.000000 raga-cli-0.1.2/rc/commands/list.py
--rw-r--r--   0 manabroy   (501) staff       (20)     1735 2023-04-13 04:42:45.000000 raga-cli-0.1.2/rc/commands/put.py
--rw-r--r--   0 manabroy   (501) staff       (20)     7752 2023-04-25 11:55:43.000000 raga-cli-0.1.2/rc/commands/repo.py
--rw-r--r--   0 manabroy   (501) staff       (20)     9835 2023-04-10 13:07:16.000000 raga-cli-0.1.2/rc/exceptions.py
--rw-r--r--   0 manabroy   (501) staff       (20)     1298 2023-04-10 13:07:16.000000 raga-cli-0.1.2/rc/prompt.py
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-25 11:58:15.061226 raga-cli-0.1.2/rc/repo/
--rw-r--r--   0 manabroy   (501) staff       (20)      938 2023-04-10 13:07:16.000000 raga-cli-0.1.2/rc/repo/get.py
--rw-r--r--   0 manabroy   (501) staff       (20)     5180 2023-04-25 07:42:51.000000 raga-cli-0.1.2/rc/repo/put.py
--rw-r--r--   0 manabroy   (501) staff       (20)        1 2023-04-10 13:07:16.000000 raga-cli-0.1.2/rc/repo/repo.py
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-25 11:58:15.061457 raga-cli-0.1.2/rc/stage/
--rw-r--r--   0 manabroy   (501) staff       (20)       85 2023-04-10 13:07:16.000000 raga-cli-0.1.2/rc/stage/exceptions.py
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-25 11:58:15.062495 raga-cli-0.1.2/rc/utils/
--rw-r--r--   0 manabroy   (501) staff       (20)     1855 2023-04-10 13:07:16.000000 raga-cli-0.1.2/rc/utils/__init__.py
--rw-r--r--   0 manabroy   (501) staff       (20)        0 2023-04-10 13:07:16.000000 raga-cli-0.1.2/rc/utils/auditLog.py
--rw-r--r--   0 manabroy   (501) staff       (20)       46 2023-04-10 13:07:16.000000 raga-cli-0.1.2/rc/utils/fileLog.py
--rw-r--r--   0 manabroy   (501) staff       (20)     6464 2023-04-19 07:04:43.000000 raga-cli-0.1.2/rc/utils/request.py
--rw-r--r--   0 manabroy   (501) staff       (20)     2924 2023-04-10 13:07:16.000000 raga-cli-0.1.2/rc/utils/sshKeyGen.py
--rw-r--r--   0 manabroy   (501) staff       (20)      248 2023-04-10 13:07:16.000000 raga-cli-0.1.2/rc/version.py
--rw-r--r--   0 manabroy   (501) staff       (20)       38 2023-04-25 11:58:15.063197 raga-cli-0.1.2/setup.cfg
--rw-r--r--   0 manabroy   (501) staff       (20)       47 2023-04-10 13:07:16.000000 raga-cli-0.1.2/setup.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-26 13:57:32.920738 raga-cli-0.1.3/
+-rw-r--r--   0 manabroy   (501) staff       (20)      741 2023-04-10 13:07:16.000000 raga-cli-0.1.3/.gitignore
+-rw-r--r--   0 manabroy   (501) staff       (20)    11350 2023-04-10 13:07:16.000000 raga-cli-0.1.3/LICENSE
+-rw-r--r--   0 manabroy   (501) staff       (20)      957 2023-04-26 13:57:32.920167 raga-cli-0.1.3/PKG-INFO
+-rw-r--r--   0 manabroy   (501) staff       (20)        0 2023-04-10 13:07:16.000000 raga-cli-0.1.3/README.rst
+-rw-r--r--   0 manabroy   (501) staff       (20)     2482 2023-04-26 13:57:18.000000 raga-cli-0.1.3/pyproject.toml
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-26 13:57:32.913833 raga-cli-0.1.3/raga_cli.egg-info/
+-rw-r--r--   0 manabroy   (501) staff       (20)      957 2023-04-26 13:57:32.000000 raga-cli-0.1.3/raga_cli.egg-info/PKG-INFO
+-rw-r--r--   0 manabroy   (501) staff       (20)      612 2023-04-26 13:57:32.000000 raga-cli-0.1.3/raga_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 manabroy   (501) staff       (20)        1 2023-04-26 13:57:32.000000 raga-cli-0.1.3/raga_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 manabroy   (501) staff       (20)       35 2023-04-26 13:57:32.000000 raga-cli-0.1.3/raga_cli.egg-info/entry_points.txt
+-rw-r--r--   0 manabroy   (501) staff       (20)     1014 2023-04-26 13:57:32.000000 raga-cli-0.1.3/raga_cli.egg-info/requires.txt
+-rw-r--r--   0 manabroy   (501) staff       (20)        3 2023-04-26 13:57:32.000000 raga-cli-0.1.3/raga_cli.egg-info/top_level.txt
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-26 13:57:32.914587 raga-cli-0.1.3/rc/
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-26 13:57:32.915845 raga-cli-0.1.3/rc/cli/
+-rw-r--r--   0 manabroy   (501) staff       (20)     3473 2023-04-25 11:42:11.000000 raga-cli-0.1.3/rc/cli/__init__.py
+-rw-r--r--   0 manabroy   (501) staff       (20)      292 2023-04-12 12:54:24.000000 raga-cli-0.1.3/rc/cli/command.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     2074 2023-04-12 11:10:34.000000 raga-cli-0.1.3/rc/cli/parser.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     9804 2023-04-26 13:39:58.000000 raga-cli-0.1.3/rc/cli/utils.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-26 13:57:32.917109 raga-cli-0.1.3/rc/commands/
+-rw-r--r--   0 manabroy   (501) staff       (20)     3226 2023-04-10 13:07:16.000000 raga-cli-0.1.3/rc/commands/get.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     1634 2023-04-12 11:10:34.000000 raga-cli-0.1.3/rc/commands/list.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     1735 2023-04-13 04:42:45.000000 raga-cli-0.1.3/rc/commands/put.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     8399 2023-04-26 13:52:50.000000 raga-cli-0.1.3/rc/commands/repo.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     9835 2023-04-10 13:07:16.000000 raga-cli-0.1.3/rc/exceptions.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     1298 2023-04-10 13:07:16.000000 raga-cli-0.1.3/rc/prompt.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-26 13:57:32.917831 raga-cli-0.1.3/rc/repo/
+-rw-r--r--   0 manabroy   (501) staff       (20)      938 2023-04-10 13:07:16.000000 raga-cli-0.1.3/rc/repo/get.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     5345 2023-04-26 13:51:01.000000 raga-cli-0.1.3/rc/repo/put.py
+-rw-r--r--   0 manabroy   (501) staff       (20)        1 2023-04-10 13:07:16.000000 raga-cli-0.1.3/rc/repo/repo.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-26 13:57:32.918094 raga-cli-0.1.3/rc/stage/
+-rw-r--r--   0 manabroy   (501) staff       (20)       85 2023-04-10 13:07:16.000000 raga-cli-0.1.3/rc/stage/exceptions.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-26 13:57:32.919285 raga-cli-0.1.3/rc/utils/
+-rw-r--r--   0 manabroy   (501) staff       (20)     1855 2023-04-10 13:07:16.000000 raga-cli-0.1.3/rc/utils/__init__.py
+-rw-r--r--   0 manabroy   (501) staff       (20)        0 2023-04-10 13:07:16.000000 raga-cli-0.1.3/rc/utils/auditLog.py
+-rw-r--r--   0 manabroy   (501) staff       (20)       46 2023-04-10 13:07:16.000000 raga-cli-0.1.3/rc/utils/fileLog.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     6463 2023-04-26 13:39:34.000000 raga-cli-0.1.3/rc/utils/request.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     2924 2023-04-10 13:07:16.000000 raga-cli-0.1.3/rc/utils/sshKeyGen.py
+-rw-r--r--   0 manabroy   (501) staff       (20)      248 2023-04-10 13:07:16.000000 raga-cli-0.1.3/rc/version.py
+-rw-r--r--   0 manabroy   (501) staff       (20)       38 2023-04-26 13:57:32.920833 raga-cli-0.1.3/setup.cfg
+-rw-r--r--   0 manabroy   (501) staff       (20)       47 2023-04-10 13:07:16.000000 raga-cli-0.1.3/setup.py
```

### Comparing `raga-cli-0.1.2/.gitignore` & `raga-cli-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `raga-cli-0.1.2/LICENSE` & `raga-cli-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `raga-cli-0.1.2/PKG-INFO` & `raga-cli-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raga-cli
-Version: 0.1.2
+Version: 0.1.3
 Summary: Git for data scientists - manage your code and data together
 Author-email: Manab Roy <manabr@observancegroup.com>
 Maintainer-email: Manab Roy <support@observancegroup.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Keywords: data-science,data-version-control,machine-learning,git,developer-tools,reproducibility,collaboration,ai,raga
```

### Comparing `raga-cli-0.1.2/pyproject.toml` & `raga-cli-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61", "setuptools_scm[toml]>=7"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "raga-cli"
-version = "0.1.2"
+version = "0.1.3"
 description = "Git for data scientists - manage your code and data together"
 readme = "README.rst"
 requires-python = ">=3.7"
 keywords = [
     "data-science",
     "data-version-control",
     "machine-learning",
```

### Comparing `raga-cli-0.1.2/raga_cli.egg-info/PKG-INFO` & `raga-cli-0.1.3/raga_cli.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raga-cli
-Version: 0.1.2
+Version: 0.1.3
 Summary: Git for data scientists - manage your code and data together
 Author-email: Manab Roy <manabr@observancegroup.com>
 Maintainer-email: Manab Roy <support@observancegroup.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Keywords: data-science,data-version-control,machine-learning,git,developer-tools,reproducibility,collaboration,ai,raga
```

### Comparing `raga-cli-0.1.2/raga_cli.egg-info/SOURCES.txt` & `raga-cli-0.1.3/raga_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `raga-cli-0.1.2/raga_cli.egg-info/requires.txt` & `raga-cli-0.1.3/raga_cli.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `raga-cli-0.1.2/rc/cli/__init__.py` & `raga-cli-0.1.3/rc/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.1.2/rc/cli/parser.py` & `raga-cli-0.1.3/rc/cli/parser.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.1.2/rc/cli/utils.py` & `raga-cli-0.1.3/rc/cli/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,14 +53,16 @@
     return False
 
 def get_new_dvc_data_status(path):
     if not get_dvc_data_status(path) and not compare_dot_dvc_file(path):
         return True
     return False
 
+
+
 def dataset_current_version(paths, repo):
     current_version = 0 if not get_repo_version(repo) else int(get_repo_version(repo))
     for path in paths:
         if not compare_dot_dvc_file(path):
             return current_version+1
         if get_dvc_data_status(path):
             return current_version+1
```

### Comparing `raga-cli-0.1.2/rc/commands/get.py` & `raga-cli-0.1.3/rc/commands/get.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.1.2/rc/commands/list.py` & `raga-cli-0.1.3/rc/commands/list.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.1.2/rc/commands/put.py` & `raga-cli-0.1.3/rc/commands/put.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.1.2/rc/commands/repo.py` & `raga-cli-0.1.3/rc/commands/repo.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,14 +60,17 @@
             run_command_on_subprocess("git add README.md", repo_name)      
             run_command_on_subprocess("git commit -m '{0}' -a".format("Model repo init"), repo_name)  
             run_command_on_subprocess("git branch -M {0}".format(self.GIT_BRANCH), repo_name)    
             run_command_on_subprocess("git push --set-upstream origin {0}".format(self.GIT_BRANCH), repo_name)    
 
     
     def create_repo(self, args):
+        if self.check_git_init():
+            print("The cloning process inside the repository is not possible.")
+            sys.exit(50)
         print("Repo creating...")   
         logger.debug(f"START CREATE REPO COMMAND")
         repository_name = args.name       
         repository_tag = args.tag  
         if repository_tag not in self.TAGS:
             logger.error("'{0}' tag is not available. Please select from {1}".format(repository_tag, self.TAGS))
             sys.exit(50)                      
@@ -94,16 +97,27 @@
             logger.debug(req_body)
 
         create_repository(req_body)
         create_repo_lock(json.dumps({"repo_name":repository_name, "user_name":self.created_by, "locked":False}))
 
         print("Repository has been created. `cd {}`".format(repository_name))    
         logger.debug(f"END CREATE REPO COMMAND")
+    
+    def check_git_init(self):
+        current_dir = os.getcwd()
+        while current_dir != '/':  # Stop when we reach the root directory
+            if os.path.exists(os.path.join(current_dir, '.git')):
+                return True  # .git folder exists, so project has been initialized
+            current_dir = os.path.dirname(current_dir)
+        return False
 
     def clone_repo(self, args):
+        if self.check_git_init():
+            print("The cloning process inside the repository is not possible.")
+            sys.exit(50)
         start = timer()
         repository_name = args.name     
         print('Cloning...')
         run_command_on_subprocess("git clone git@github.com:{0}/{1}.git".format(self.GIT_ORG, repository_name), None, True)    
         tag = get_repository(repository_name)
         if tag == "dataset":
             run_command_on_subprocess("dvc pull", repository_name, True)
```

### Comparing `raga-cli-0.1.2/rc/exceptions.py` & `raga-cli-0.1.3/rc/exceptions.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.1.2/rc/prompt.py` & `raga-cli-0.1.3/rc/prompt.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.1.2/rc/repo/get.py` & `raga-cli-0.1.3/rc/repo/get.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.1.2/rc/repo/put.py` & `raga-cli-0.1.3/rc/repo/put.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import logging
 import threading
 import time
 
 from rc.cli.utils import compare_dot_dvc_file, run_command_on_subprocess
 from timeit import default_timer as timer
 from rc.cli.utils import *
-from rc.utils.request import is_repo_lock, update_repo_commit_id, update_repo_lock, insert_repo_commit, get_repository
+from rc.utils.request import get_commit_version, is_repo_lock, update_repo_commit_id, update_repo_lock, insert_repo_commit, get_repository
 
 logger = logging.getLogger(__name__)
 repo_commit_ids = []
 pool_time = 10
 
 def dir_add(path):
     start = timer()
@@ -55,16 +55,20 @@
         if not stop_checking_elastic_process:
             time.sleep(pool_time)
     return True
 
 def model_upload(message, repo, model_version):
     update_repo_lock(repo, json.dumps({"locked":True}))
     print("Model files uploading...")
-    branchName = current_branch()
     commit_hash = current_commit_hash()
+    commit_hash = current_commit_hash()
+    if get_commit_version(commit_hash):
+        print("The latest commit is unchanged.")
+        sys.exit(50)
+    branchName = current_branch()
     branchName = current_branch()
     request_payload = {
                 "commit_message" : message,
                 "repo" : repo,
                 "commit_id":commit_hash,
                 "version":model_version,
                 "branch":branchName
@@ -101,15 +105,14 @@
     print("Files uploaded successfully")
 
 def put(args):
     start = timer()
     message = args.message      
     paths = args.path   
     repo = get_repo()     
-    
     # print("VERSION", current_version)
     # print("CHECK ELASTIC PROCESS", server_repo_commit_status(repo_commit_ids))
     # return
 
     tag = get_repository(repo)
     is_repo_lock(repo)
```

### Comparing `raga-cli-0.1.2/rc/utils/__init__.py` & `raga-cli-0.1.3/rc/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.1.2/rc/utils/request.py` & `raga-cli-0.1.3/rc/utils/request.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,15 +151,15 @@
     if response['success']:
         if 'data' not in response.keys():
             raise RctlValidRequestError("HTTP response `data` keyword not found.")
     if not response['data']:
         return False
     else:
         logger.debug("RESPONSE VALUE FROM URL: {0} --- VALUE : {1}".format(url, response['data']))
-        return response['data']["version"]  
+        return response['data']["version"] 
 
 def get_repository(obj):
     url = f"{BASE_URL}/repos-name?repoName={obj}"
     response = valid_response(make_request(url, "GET"))
     data = response['data']['tag']
     logger.debug("RESPONSE VALUE FROM URL: {0} --- VALUE : {1}".format(url, data))
     return data
```

### Comparing `raga-cli-0.1.2/rc/utils/sshKeyGen.py` & `raga-cli-0.1.3/rc/utils/sshKeyGen.py`

 * *Files identical despite different names*

