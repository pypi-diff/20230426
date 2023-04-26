# Comparing `tmp/falra_run_github-0.1.0.tar.gz` & `tmp/falra_run_github-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/falra_run_github-0.1.0.tar", last modified: Sat Apr 22 00:36:52 2023, max compression
+gzip compressed data, was "dist/falra_run_github-0.1.1.tar", last modified: Wed Apr 26 15:02:59 2023, max compression
```

## Comparing `falra_run_github-0.1.0.tar` & `falra_run_github-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 wengroy    (501) staff       (20)        0 2023-04-22 00:36:52.501617 falra_run_github-0.1.0/
--rw-r--r--   0 wengroy    (501) staff       (20)      190 2023-04-22 00:36:52.501343 falra_run_github-0.1.0/PKG-INFO
--rw-r--r--   0 wengroy    (501) staff       (20)      984 2023-04-13 18:39:23.000000 falra_run_github-0.1.0/README.md
-drwxr-xr-x   0 wengroy    (501) staff       (20)        0 2023-04-22 00:36:52.496372 falra_run_github-0.1.0/falra_run_github/
--rw-r--r--   0 wengroy    (501) staff       (20)        0 2023-03-09 00:23:54.000000 falra_run_github-0.1.0/falra_run_github/__init__.py
--rw-r--r--   0 wengroy    (501) staff       (20)       78 2023-04-13 18:03:18.000000 falra_run_github-0.1.0/falra_run_github/__main__.py
--rwxr-xr-x   0 wengroy    (501) staff       (20)    11129 2023-04-21 10:45:35.000000 falra_run_github-0.1.0/falra_run_github/main.py
-drwxr-xr-x   0 wengroy    (501) staff       (20)        0 2023-04-22 00:36:52.500928 falra_run_github-0.1.0/falra_run_github.egg-info/
--rw-r--r--   0 wengroy    (501) staff       (20)      190 2023-04-22 00:36:52.000000 falra_run_github-0.1.0/falra_run_github.egg-info/PKG-INFO
--rw-r--r--   0 wengroy    (501) staff       (20)      343 2023-04-22 00:36:52.000000 falra_run_github-0.1.0/falra_run_github.egg-info/SOURCES.txt
--rw-r--r--   0 wengroy    (501) staff       (20)        1 2023-04-22 00:36:52.000000 falra_run_github-0.1.0/falra_run_github.egg-info/dependency_links.txt
--rw-r--r--   0 wengroy    (501) staff       (20)       62 2023-04-22 00:36:52.000000 falra_run_github-0.1.0/falra_run_github.egg-info/entry_points.txt
--rw-r--r--   0 wengroy    (501) staff       (20)      600 2023-04-22 00:36:52.000000 falra_run_github-0.1.0/falra_run_github.egg-info/requires.txt
--rw-r--r--   0 wengroy    (501) staff       (20)       17 2023-04-22 00:36:52.000000 falra_run_github-0.1.0/falra_run_github.egg-info/top_level.txt
--rw-r--r--   0 wengroy    (501) staff       (20)       38 2023-04-22 00:36:52.501702 falra_run_github-0.1.0/setup.cfg
--rwxr-xr-x   0 wengroy    (501) staff       (20)      439 2023-04-21 10:47:18.000000 falra_run_github-0.1.0/setup.py
+drwxr-xr-x   0 wengroy    (501) staff       (20)        0 2023-04-26 15:02:59.902256 falra_run_github-0.1.1/
+-rw-r--r--   0 wengroy    (501) staff       (20)      190 2023-04-26 15:02:59.901967 falra_run_github-0.1.1/PKG-INFO
+-rw-r--r--   0 wengroy    (501) staff       (20)      984 2023-04-13 18:39:23.000000 falra_run_github-0.1.1/README.md
+drwxr-xr-x   0 wengroy    (501) staff       (20)        0 2023-04-26 15:02:59.897884 falra_run_github-0.1.1/falra_run_github/
+-rw-r--r--   0 wengroy    (501) staff       (20)        0 2023-03-09 00:23:54.000000 falra_run_github-0.1.1/falra_run_github/__init__.py
+-rw-r--r--   0 wengroy    (501) staff       (20)       78 2023-04-13 18:03:18.000000 falra_run_github-0.1.1/falra_run_github/__main__.py
+-rwxr-xr-x   0 wengroy    (501) staff       (20)     8790 2023-04-26 14:56:03.000000 falra_run_github-0.1.1/falra_run_github/main.py
+drwxr-xr-x   0 wengroy    (501) staff       (20)        0 2023-04-26 15:02:59.901517 falra_run_github-0.1.1/falra_run_github.egg-info/
+-rw-r--r--   0 wengroy    (501) staff       (20)      190 2023-04-26 15:02:59.000000 falra_run_github-0.1.1/falra_run_github.egg-info/PKG-INFO
+-rw-r--r--   0 wengroy    (501) staff       (20)      343 2023-04-26 15:02:59.000000 falra_run_github-0.1.1/falra_run_github.egg-info/SOURCES.txt
+-rw-r--r--   0 wengroy    (501) staff       (20)        1 2023-04-26 15:02:59.000000 falra_run_github-0.1.1/falra_run_github.egg-info/dependency_links.txt
+-rw-r--r--   0 wengroy    (501) staff       (20)       62 2023-04-26 15:02:59.000000 falra_run_github-0.1.1/falra_run_github.egg-info/entry_points.txt
+-rw-r--r--   0 wengroy    (501) staff       (20)      600 2023-04-26 15:02:59.000000 falra_run_github-0.1.1/falra_run_github.egg-info/requires.txt
+-rw-r--r--   0 wengroy    (501) staff       (20)       17 2023-04-26 15:02:59.000000 falra_run_github-0.1.1/falra_run_github.egg-info/top_level.txt
+-rw-r--r--   0 wengroy    (501) staff       (20)       38 2023-04-26 15:02:59.902355 falra_run_github-0.1.1/setup.cfg
+-rwxr-xr-x   0 wengroy    (501) staff       (20)      439 2023-04-26 14:57:49.000000 falra_run_github-0.1.1/setup.py
```

### Comparing `falra_run_github-0.1.0/README.md` & `falra_run_github-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `falra_run_github-0.1.0/falra_run_github/main.py` & `falra_run_github-0.1.1/falra_run_github/main.py`

 * *Files 23% similar despite different names*

```diff
@@ -34,46 +34,38 @@
     try:
         if not is_git_installed():
             print("Git is not installed！ Trigger auto git install from apt-get..")
             install_git()
         else:
             print("Git installed！")
     except Exception as e:
-        print(f"""[init()] git install check fail.. skip! error:{e}""")
+        print(f"""[download_files_from_github] git install check fail.. skip! error:{e}""")
 
-    # 檢查本地路徑是否存在，如果不存在則創建
+    # 檢查本地路徑是否存在，如果不存在則創建，存在則刪除乾淨
     if not os.path.exists(local_path):
         os.makedirs(local_path)
+    else:
+        clean_user_repo(repo_path=local_path)
 
     # 將存儲庫URL更改為使用訪問令牌
     repo_url = repo_url.replace("https://", f"https://{token}@")
 
-    # 執行 git clone
-    subprocess.run(["git", "clone", repo_url, local_path])
+    try:
+        # 執行 git clone
+        print("Git clone ...start")
+        os.system(f"""git clone {repo_url} {local_path}""")
+        print("Git clone ...success")
+    except Exception as e:
+        print(f"""[download_files_from_github] git clone fail.. skip! error:{e}""")
 
 
 def download_github_repo(repo_url, access_token, repo_name="repo"):
     # 解析出 repo 的 owner 和 name
     _, owner, name = repo_url.rstrip('/').rsplit('/', 2)
 
-    '''
-    # 設置 API 請求頭部，添加授權欄位
-    #headers = {
-    #    'Authorization': f'Token {access_token}',
-    #    'Accept': 'application/vnd.github.v3+json'
-    #}
-    # 請求 repo 的內容
-    #repo_api_url = f'https://api.github.com/repos/{owner}/{name}/contents/'
-    #github_url = f'https://github.com/{owner}/{name}/'
-    #response = requests.get(repo_url, headers=headers)
-
-    # 將內容轉換為 JSON 格式
-    #repo_contents = response.json()
-    '''
-
     # 創建新目錄來存儲 repo 的內容
     if not os.path.exists("user-repo"):
         os.mkdir("user-repo")
     repo_name = os.path.join("user-repo", repo_name)
     if not os.path.exists(repo_name):
         os.mkdir(repo_name)
 
@@ -97,27 +89,14 @@
 def run_main_py(repo_name, output_file="falra_output.txt", py_name="main.py", arg=[]):
     # 獲取 main.py 的路徑
     repo_name = os.path.join("user-repo", repo_name)
     # 已經更改為進入 repo 子資料夾去執行 main.py
     main_path = py_name
     #main_path = os.path.join(repo_name, py_name)
 
-    '''
-    # 檢查 main.py 是否存在
-    if not os.path.exists(main_path):
-        print("Error: main.py not found")
-        return
-
-    # 清除上一次的 falra_output.txt
-    output_file = f"""{repo_name}/falra_output.txt"""
-    output_file = os.path.join(os.getcwd(), output_file)  # 取絕對路徑
-    if os.path.exists(output_file):
-        os.remove(output_file)
-    '''
-
     # 設置子資料夾的路徑
     sub_dir = repo_name
 
     # 儲存當前工作目錄
     current_dir = os.getcwd()
 
     # 更改工作目錄到子資料夾
@@ -128,101 +107,42 @@
         print("Error: main.py not found")
         return
 
     # 清除上一次的 falra_output.txt
     if os.path.exists(output_file):
         os.remove(output_file)
     # 執行命令
-    print(f" debug 001 python version.....")
+    print(f" 003-1 python version.....")
     result = subprocess.run(['python3', '--version'])
     print(result.stdout)
-    print(f" debug 002 pwd.....")
+    print(f" 003-2 pwd.....")
     result = subprocess.run(['pwd'], capture_output=True, text=True)
     print(result.stdout)
 
-    #print(f" debug 003 pwd.....")
-    #result = subprocess.run(['python3', 'main_bytesio_stream.py'])
-    #print(result.stdout)
-
-
-    # 執行 main.py
-    #python_command_list = ["python3", main_path]
-    #python_commandlist = python_command_list + arg
-
     python_arg_str = ' '.join(arg)
     python_command_str = f"""python3 {main_path} {python_arg_str}"""
     python_command_str: str = f"""{python_command_str} >> {output_file}"""
 
     try:
         # for security, prevent code injection
         python_command_str.replace(";","").replace("|","")
         print(f"""============ python_command==========  {python_command_str}""")
 
         # 使用 os.system 去執行指令
         # 好處：字串指令執行即可
         # 缺點：無法讀取 stdoutput ，替代方案： cmd > output.txt
         os.system(python_command_str)
 
-
         # 打印命令的輸出
         print(f"Output: {output_file}")
 
-        '''
-        #output = subprocess.run(python_command, capture_output=True, text=True)
-
-        print(f"""subprocess.Popen running""")
-        # 使用 subprocess.Popen 並將 stdout 設置為 subprocess.PIPE
-        #process = subprocess.Popen(python_command, text=True, shell=True)
-
-        # 使用subprocess.Popen執行命令
-        process = subprocess.Popen(python_command, stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True)
-
-        # 獲取命令的輸出和錯誤
-        output, error = process.communicate()
-
-        # 檢查錯誤，如果有錯誤則打印
-        if error:
-            print(f"Error: {error.decode('utf-8')}")
-        else:
-            # 打印命令的輸出
-            print(f"Output: {output.decode('utf-8')}")
-            with open(output_file, "a") as f:
-                f.write(f"""{output}\n""")
-
-        print(f"""subprocess.Popen running 2""")
-        '''
-
-        '''
-        # 這將持續從 process 輸出 stdout
-        while True:
-            print(f"""subprocess.Popen get output loop...""")
-            output = process.stdout.readline()
-            if output == "" and process.poll() is not None:
-                break
-            if output:
-                sys.stdout.write(output)
-                sys.stdout.flush()
-                with open(output_file, "a") as f:
-                    f.write(f"""{output}\n""")
-
-        # 獲取 process 的結束碼
-        return_code = process.poll()
-        print(f"Return code: {return_code}")
-        '''
-
-        '''
-        # 將輸出寫入檔案
-        with open(output_file, "a") as f:
-            f.write(output.stdout.strip())
-        '''
-
     except Exception as e:
         # 如果 subprocess 產生錯誤，將錯誤訊息寫到檔案中
-        print(f"""=[python command ERROR!!] python_command:  {python_command}""")
-        error_msg = f"ERROR while running '{py_name}', python_command:  {python_command}. ERROR_msg：{e}"
+        print(f"""=[python command ERROR!!] python_command:  {python_command_str}""")
+        error_msg = f"ERROR while running '{py_name}', python_command:  {python_command_str}. ERROR_msg：{e}"
         print(error_msg)
         with open(output_file, "a") as f:
             f.write(error_msg)
 
     # 恢復到原始工作目錄
     os.chdir(current_dir)
 
@@ -235,42 +155,40 @@
     with open(output_file_path, 'r') as f:
         contents = f.read()
         print(contents)
         # 返回結果
         return contents
 
 
-def clean_user_repo(repo_name=""):
+def clean_user_repo(repo_path=""):
     folder_path = 'user-repo'
 
-    if repo_name:
-        folder_path = os.path.join(folder_path, repo_name)
+    if repo_path:
+        folder_path = repo_path
 
     for root, dirs, files in os.walk(folder_path, topdown=False):
         for file in files:
             os.remove(os.path.join(root, file))
         for dir in dirs:
             shutil.rmtree(os.path.join(root, dir))
 
 def main_run_github(repo_url, access_token, repo_name, py_name, arg_str):
-
-    #repo_url = sys.argv[1] # "https://github.com/my-account/my-repo"
-    #access_token = sys.argv[2] # "access_token
-    #repo_name = sys.argv[3] # 'my-repo'
-    #py_name = sys.argv[4] # 'main.py'
+    # repo_url = sys.argv[1] # "https://github.com/my-account/my-repo"
+    # access_token = sys.argv[2] # "access_token
+    # repo_name = sys.argv[3] # 'my-repo'
+    # py_name = sys.argv[4] # 'main.py'
+    # arg_str = sys.argv[5] # "['argument']"
 
     # read parameters
     arg = []
-    #arg_str = sys.argv[5] # "['argument']"
     # 將字符串轉換為 list
     arg = ast.literal_eval(arg_str)
 
     # Download GitHub repo and save to local directory user-repo
     print("002 download_github_repo..")
-    #clean_user_repo(repo_name=repo_name)
     download_github_repo(repo_url, access_token, repo_name)
 
     # 創建 output 目錄來存儲執行結果
     #if not os.path.exists(repo_name):
     #    os.mkdir(repo_name)
     # 創建 output 目錄來存儲執行結果
     #output_dir = f"""{repo_name}/output"""
@@ -289,29 +207,35 @@
 
 
 def main():
     parser = argparse.ArgumentParser(description='GitHub Executor')
     parser.add_argument('--action', type=str, required=True, choices=['start', 'output', 'clean'], help="The actions to execute")
     parser.add_argument('--repo_url', metavar='repo_url', type=str, help='URL of the GitHub repository')
     parser.add_argument('--access_token', metavar='access_token', type=str, help='Access token for the GitHub API')
+    parser.add_argument('--user_id', metavar='user_id', type=str, help='user_id as string')
     parser.add_argument('--repo_name', metavar='repo_name', type=str, help='Name of the repository')
     parser.add_argument('--py_name', metavar='py_name', type=str, help='Name of the Python file to execute')
     parser.add_argument('--argument', metavar='argument', type=str, help='Arguments of the Python to execute as string')
 
     args = parser.parse_args()
 
     print(f"""Action = {args.action}""")
 
     if args.action == "start":
         if not args.repo_url:
             parser.error("Executing run_github requires --repo_url parameter")
         print(f"""001 start falra_run_github..""")
+
+        repo_path = args.repo_name
+        if args.user_id :
+            repo_path = f"""{args.user_id}_{args.repo_name}"""
+
         main_run_github(repo_url=args.repo_url,
                         access_token=args.access_token,
-                        repo_name=args.repo_name,
+                        repo_name=repo_path,
                         py_name=args.py_name,
                         arg_str=args.argument,
                         )
     elif args.action == "output":
         if not args.repo_name:
             parser.error("Executing output query requires --repo_name parameter")
         query_output(args.repo_name)
```

### Comparing `falra_run_github-0.1.0/falra_run_github.egg-info/requires.txt` & `falra_run_github-0.1.1/falra_run_github.egg-info/requires.txt`

 * *Files identical despite different names*

