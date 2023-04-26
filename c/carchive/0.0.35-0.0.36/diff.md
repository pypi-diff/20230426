# Comparing `tmp/carchive-0.0.35.tar.gz` & `tmp/carchive-0.0.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carchive-0.0.35.tar", last modified: Wed Feb 15 05:36:10 2023, max compression
+gzip compressed data, was "carchive-0.0.36.tar", last modified: Tue Apr 25 14:12:31 2023, max compression
```

## Comparing `carchive-0.0.35.tar` & `carchive-0.0.36.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 05:36:10.172708 carchive-0.0.35/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-02-15 05:36:05.000000 carchive-0.0.35/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-02-15 05:36:10.168708 carchive-0.0.35/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-02-15 05:36:05.000000 carchive-0.0.35/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 05:36:10.168708 carchive-0.0.35/carchive/
--rwxr-xr-x   0 runner    (1001) docker     (123)    18463 2023-02-15 05:36:05.000000 carchive-0.0.35/carchive/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 05:36:10.168708 carchive-0.0.35/carchive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-02-15 05:36:10.000000 carchive-0.0.35/carchive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-02-15 05:36:10.000000 carchive-0.0.35/carchive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-15 05:36:10.000000 carchive-0.0.35/carchive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-15 05:36:10.000000 carchive-0.0.35/carchive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-15 05:36:10.000000 carchive-0.0.35/carchive.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-15 05:36:10.172708 carchive-0.0.35/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3191 2023-02-15 05:36:05.000000 carchive-0.0.35/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:12:31.573751 carchive-0.0.36/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-25 14:12:28.000000 carchive-0.0.36/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-25 14:12:31.573751 carchive-0.0.36/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-25 14:12:28.000000 carchive-0.0.36/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:12:31.573751 carchive-0.0.36/carchive/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16455 2023-04-25 14:12:28.000000 carchive-0.0.36/carchive/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:12:31.573751 carchive-0.0.36/carchive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-25 14:12:31.000000 carchive-0.0.36/carchive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-25 14:12:31.000000 carchive-0.0.36/carchive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 14:12:31.000000 carchive-0.0.36/carchive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-25 14:12:31.000000 carchive-0.0.36/carchive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-25 14:12:31.000000 carchive-0.0.36/carchive.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 14:12:31.573751 carchive-0.0.36/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3205 2023-04-25 14:12:28.000000 carchive-0.0.36/setup.py
```

### Comparing `carchive-0.0.35/LICENSE` & `carchive-0.0.36/LICENSE`

 * *Files identical despite different names*

### Comparing `carchive-0.0.35/carchive/__init__.py` & `carchive-0.0.36/carchive/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,24 @@
 import os, requests, json, base64, hashlib, time, contextlib, funbelts as ut, requests, sys, datetime
 try:
     from ghapi.all import GhApi
+    import mystring
 except:
-    os.system(f"{sys.executable} -m pip install ghapi")
+    os.system(f"{sys.executable} -m pip install --upgrade ghapi mystring")
+    from ghapi.all import GhApi
+    import mystring
 from waybackpy import WaybackMachineSaveAPI as checkpoint
 
+def set_gh_token(token):
+    os.environ['GH_TOKEN'] = token
+    try:
+        with open("~/.bashrc","a+") as writer:
+            writer.write("GH_TOKEN={0}".format(token))
+    except: pass
+
 def live_link(url: str):
     response = False
     with contextlib.suppress(Exception):
         response_type = requests.get(url)
         response = response_type.status_code < 400
         time.sleep(2)
     return response
@@ -69,59 +79,48 @@
     baseurl = "https://github.com/{0}/blob/{1}/{2}".format(repo,commit,filepath.replace(str(reponame)+"/",'',1))
     if lineno:
         baseurl += "#L{0}".format(int(lineno))
     
     return baseurl
 
 class githuburl(object):
-  def __init__(self,token=None,verify=True,wait_lambda=None,logging_lambda=None):
+  def __init__(self,token=None,verify=True,wait_lambda=None):
     self.token = token
     self.verify=verify
     self.remaining = None
     self.total = None
     self.wait_until = None
     self.wait_lambda = wait_lambda
-    self.logging_lambda = logging_lambda
-    if self.logging_lambda is None:
-      def temp(*args, **kargs):
-        return 
-      self.logging_lambda = temp
-
     self.timing
 
   def __call__(self,url,verify=True, return_error=False, json=True, baserun=False):
-      self.logging_lambda(func="Call", step="Start", message="URL:> {}".format(url))
       if not baserun:
         self.timing
 
       output = {}
       headers = {}
 
       if self.token is not None:
         headers['Authorization'] = 'Bearer {}'.format(self.token)
 
       try:
           output['data'] = requests.get(url, verify=verify and self.verify, headers=headers)
           if json:
-              self.logging_lambda(func="Call", step="Success")
               output['data'] = output['data'].json()
       except Exception as e:
           if return_error:
               output["Error"] = e
           output['data'] = None
-          self.logging_lambda(func="Call", step="Failure", message=e)
 
       return output
 
   @property
-  def status(self):
-    self.logging_lambda(func="Status", step="Start")                                                                                              
+  def status(self):                                                                                      
     # curl -I https://api.github.com/users/octocat|grep x-ratelimit-reset
     cur_status, now = self("https://api.github.com/users/octocat", json=False, baserun=True)['data'].headers, datetime.datetime.now()
-    self.logging_lambda(func="Status", step="Completed", message=cur_status)
     return {
       'Reset': cur_status['X-RateLimit-Reset'],
       'Used': cur_status['X-RateLimit-Used'],
       'Total': cur_status['X-RateLimit-Limit'],
       'Remaining': cur_status['X-RateLimit-Remaining'],
       'RemainingDate':datetime.datetime.fromtimestamp(int(cur_status['X-RateLimit-Reset'])),
       'WaitFor':datetime.datetime.fromtimestamp(int(cur_status['X-RateLimit-Reset'])) - now,
@@ -146,22 +145,14 @@
         time_to_sleep=self.wait_until()
         for itr in range(time_to_sleep):
           print("{}/{}".format(itr,time_to_sleep))
           time.sleep(1)
       self.remaining = None
       self.timing
 
-
-def set_gh_token(token):
-    os.environ['GH_TOKEN'] = token
-    try:
-        with open("~/.bashrc","a+") as writer:
-            writer.write("GH_TOKEN={0}".format(token))
-    except: pass
-
 def find(repo,asset_check=None,verify=True, accept="application/vnd.github+json", auth=None, print_info=False):
 	if asset_check is None:
 		asset_check = lambda x:False
 
 	def req(string, verify=verify, accept=accept, auth=auth, print_info=print_info):
 		try:
 			output = requests.get(string, verify=verify, headers={
@@ -221,68 +212,65 @@
     Sample usage:
     with GRepo("https://github.com/owner/repo","v1","hash") as repo:
         os.path.exists(repo.reponame) #TRUE
     """
     def __init__(self, repo: str, tag: str = None, commit: str = None, delete: bool = True, local_dir: bool = False, jsonl_file: str = None, exclude_extensions: list = [],self_archive_wait = 5*60, git_base_string="git"):
         self.inipath = os.path.abspath(os.curdir)
         self.delete = delete
-        self.tag = None
-        self.commit = commit or None
-        self.cloneurl = None
         self.jsonl_file = jsonl_file
         self.repo = repo
         self.exclude_extensions = exclude_extensions
         self.self_archive_wait=self_archive_wait
         self.git_base_string = git_base_string
+        self.tag = mystring.string(tag)
+        self.commit = mystring.string(commit).trim
+
         self.local_dir = None
+        self.cloneurl = None
+        self.gh_api = None
 
         if local_dir:
             self.url = f"file://{self.repo}"
             self.full_url = repo
-            self.api = None
             self.local_dir = local_dir
+            self.api = None
         else:
             repo = repo.replace('http://', 'https://').replace('.git','')
             if repo.endswith("/"):
                 repo = repo[:-1]
-            self.local_dir = str(repo.split("/")[-1])
+
             self.url = repo
             self.full_url = repo
-            #self.cloneurl = "--depth 1"
+            self.local_dir = str(repo.split("/")[-1])
+
             if ut.is_not_empty(tag):
                 self.tag = tag
                 self.cloneurl += f" --branch {tag}"
                 self.full_url += f"<b>{tag}"
             if ut.is_not_empty(self.commit):
                 self.full_url += f"<#>{self.commit}"
 
             gh_api = GhApi()
             splitzies = self.url.replace('https://github.com/','').split('/')
             owner,corerepo = splitzies[0], splitzies[1]
 
-            branches = []
-            main_branch = None
-            try:
+            branches, main_branch = [], None
+            with contextlib.suppress(Exception):
                 #https://docs.github.com/en/rest/branches/branches#list-branches
                 for branch in requests.get(f"https://api.github.com/repos/{owner}/{corerepo}/branches").json():
                     branches += [branch['name']]
-                    if branch['name'] in ['main','master'] and main_branch is None:
+                    if branch['name'].lower() in ['main','master'] and main_branch is None:
                         main_branch = "heads/"+branch['name']
-            except Exception as e:
-                print(f"Error getting branches: {e}")
-                pass
-
             if main_branch is None and len(branches) > 0:
                 main_branch = "heads/"+branches[0]
 
-            try:
+
+            with contextlib.suppress(Exception):
                 self.gh_api = gh_api.git.get_ref(owner=owner, repo=corerepo, ref=main_branch)
-            except Exception as e:
-                self.gh_api = None
-                print(e)
+
             if self.gh_api is not None:
                 self.gh_api.owner = owner
                 self.gh_api.repo = corerepo
                 self.gh_api.commit = self.gh_api['object']['sha']
                 self.gh_api.commit_url = '/'.join([
                     "https://github.com",
                     self.gh_api.owner,
@@ -296,14 +284,15 @@
                     self.gh_api.repo,
                     "archive",
                     str(self.gh_api.commit)+".zip"
                 ])
 
         if self.url.endswith("/"):
             self.url = self.url[:-1]
+
         self.reponame = self.url.split('/')[-1].replace('.git','')
         self.webarchive_url_base = None
         self.zip_url_base = None
         self.reponame = self.reponame or repo.split('/')[-1]
         self.cloned = False
 
 
@@ -311,20 +300,18 @@
         if not self.cloned: #not os.path.exists(self.reponame) and self.url.startswith("https://github.com/"):
             print("Waiting between scanning projects to ensure GitHub Doesn't get angry")
             ut.wait_for(5)
             cmd = "{} clone {}".format(self.git_base_string,self.url)#,'--' if 'gh' in self.git_base_string.lower() else '',self.cloneurl)
             print(cmd);ut.run(cmd)
 
             if ut.is_not_empty(self.commit):
-                os.chdir(self.reponame)
-                #cmd = f"cd {self.reponame} && git checkout {self.commit} && cd ../"
-                print(os.path.abspath(os.curdir))
-                cmd = f"git checkout {self.commit}"
-                print(cmd);ut.run(cmd)
-                os.chdir(self.inipath)
+                with mystring.foldentre()(self.reponame):
+                    print(os.path.abspath(os.curdir))
+                    cmd = f"git checkout {self.commit}"
+                    print(cmd);ut.run(cmd)
             self.cloned = True
 
     def __enter__(self):
         self.__clone()
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
@@ -410,44 +397,28 @@
                 'Commit':self.commit or self.gh_api.commit,
                 'FullUrl':self.full_url,
                 'CloneUrl':self.cloneurl,
                 'ZipUrl':self.zip_url,
                 'WebArchiveSaveUrl':self.webarchive_save_url
             }
 
-    def is_bin_file(self,foil):
-        #https://stackoverflow.com/questions/898669/how-can-i-detect-if-a-file-is-binary-non-text-in-python
-        textchars = bytearray({7,8,9,10,12,13,27} | set(range(0x20, 0x100)) - {0x7f})
-        is_binary_string = lambda bytes: bool(bytes.translate(None, textchars))
-        return is_binary_string(open(foil, 'rb').read(1024))
-
     @property
     def jsonl(self):
         try:
             with open(self.jsonl_file, 'w+') as writer:
                 writer.write(str(json.dumps({**{'header':True},**self.info})) + "\n")
                 self.__clone()
                 for root, directories, filenames in os.walk(self.reponame):
                     for filename in filenames:
                             foil = os.path.join(root, filename)
                             ext = foil.split('.')[-1].lower()
 
                             if "/.git/" not in foil and (self.exclude_extensions is None or ext not in self.exclude_extensions):
                                 try:
-                                    try:
-                                        mini = file_to_base_64(foil)
-                                    except:
-                                        mini = None
-                                    current_file_info = {
-                                        'header':False,
-                                        'file':foil,
-                                        'hash':hash(foil),
-                                        'base64':mini
-                                    }
-                                    writer.write(str(json.dumps(current_file_info)) + "\n")
+                                    writer.write(mystring.foil(foil).structured()+ "\n")
                                 except Exception as e:
                                     print(">: "+str(e))
                                     pass
         except Exception as e:
             print(f"Issue with creating the jsonl file: {e}")
 
         return self.jsonl_file
@@ -460,31 +431,17 @@
             for root, directories, filenames in os.walk(self.reponame):
                 for filename in filenames:
                     foil = os.path.join(root, filename)
                     ext = foil.split('.')[-1].lower()
 
                     if "/.git/" not in foil and (self.exclude_extensions is None or ext not in self.exclude_extensions):
                         try:
-                            try:
-                                mini = file_to_base_64(foil)
-                            except:
-                                mini = None
-
-
-                            current_file_info = {
-                                'header':False,
-                                'file':foil,
-                                'hash':hash(foil),
-                                'base64':mini
-                            }
-
                             contents += [
-                                str(json.dumps(current_file_info))
+                                mystring.foil(foil).structured()
                             ]
-
                         except Exception as e:
                             print(">: "+str(e))
                             pass
         except Exception as e:
             print(f"Issue with creating the jsonl file: {e}")
 
         return contents
```

### Comparing `carchive-0.0.35/setup.py` & `carchive-0.0.36/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 DESCRIPTION = 'My short description for my project.'
 GH_NAME = "franceme"
 URL = f"https://github.com/{GH_NAME}/{NAME}"
 long_description = pathlib.Path(f"{here}/README.md").read_text(encoding='utf-8')
 REQUIRES_PYTHON = '>=3.8.0'
 RELEASE = "?"
 entry_point = f"src.{NAME}"
-VERSION = "0.0.35"
+VERSION = "0.0.36"
 
 def zip_program(outputName:str = f"{NAME}.zip"):
 	#http://blog.ablepear.com/2012/10/bundling-python-files-into-stand-alone.html
 	if os.path.exists(outputName):
 		os.system(f"rm {outputName}")
 
 	zipf = zipfile.ZipFile(outputName, 'w', zipfile.ZIP_DEFLATED)
@@ -104,14 +104,15 @@
 		exclude=["tests", "*.tests", "*.tests.*", "tests.*"]),
 	entry_points={
 	},
 	install_requires=[
 		"funbelts",
 		"waybackpy",
 		"ghapi",
+		"mystring",
 	],
 	include_package_data=True,
 	classifiers=[
 		'Programming Language :: Python',
 		'Programming Language :: Python :: 3',
 		'Programming Language :: Python :: 3.8',
 	],
```

