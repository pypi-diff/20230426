# Comparing `tmp/langpack-0.0.3-py2.py3-none-any.whl.zip` & `tmp/langpack-0.0.4-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 13027 bytes, number of entries: 12
+Zip file size: 15116 bytes, number of entries: 12
 -rw-rw-r--  2.0 unx        0 b- defN 23-Apr-09 18:39 langpack/__init__.py
 -rw-rw-r--  2.0 unx      857 b- defN 23-Apr-21 03:47 langpack/app_template.py
 -rw-rw-r--  2.0 unx      611 b- defN 23-Apr-21 04:02 langpack/client_template.py
 -rw-rw-r--  2.0 unx     2787 b- defN 23-Apr-20 22:07 langpack/index.html
 -rw-rw-r--  2.0 unx     7528 b- defN 23-Apr-21 05:17 langpack/tester.py
--rw-rw-r--  2.0 unx    21745 b- defN 23-Apr-21 06:43 langpack/tools.py
--rw-rw-r--  2.0 unx     7512 b- defN 23-Apr-24 16:47 langpack/utils.py
--rw-rw-r--  2.0 unx      871 b- defN 23-Apr-25 22:28 langpack-0.0.3.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 23-Apr-25 22:28 langpack-0.0.3.dist-info/WHEEL
--rw-rw-r--  2.0 unx       77 b- defN 23-Apr-25 22:28 langpack-0.0.3.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        9 b- defN 23-Apr-25 22:28 langpack-0.0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      934 b- defN 23-Apr-25 22:28 langpack-0.0.3.dist-info/RECORD
-12 files, 43041 bytes uncompressed, 11463 bytes compressed:  73.4%
+-rw-rw-r--  2.0 unx    26333 b- defN 23-Apr-26 18:51 langpack/tools.py
+-rw-rw-r--  2.0 unx    10404 b- defN 23-Apr-26 18:27 langpack/utils.py
+-rw-rw-r--  2.0 unx      905 b- defN 23-Apr-26 18:53 langpack-0.0.4.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 23-Apr-26 18:53 langpack-0.0.4.dist-info/WHEEL
+-rw-rw-r--  2.0 unx      200 b- defN 23-Apr-26 18:53 langpack-0.0.4.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        9 b- defN 23-Apr-26 18:53 langpack-0.0.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      936 b- defN 23-Apr-26 18:53 langpack-0.0.4.dist-info/RECORD
+12 files, 50680 bytes uncompressed, 13552 bytes compressed:  73.3%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: langpack/tools.py
 Comment: 
 
 Filename: langpack/utils.py
 Comment: 
 
-Filename: langpack-0.0.3.dist-info/METADATA
+Filename: langpack-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: langpack-0.0.3.dist-info/WHEEL
+Filename: langpack-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: langpack-0.0.3.dist-info/entry_points.txt
+Filename: langpack-0.0.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: langpack-0.0.3.dist-info/top_level.txt
+Filename: langpack-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: langpack-0.0.3.dist-info/RECORD
+Filename: langpack-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## langpack/tools.py

```diff
@@ -11,16 +11,28 @@
 import inspect
 import shutil
 import imp
 import pkgutil
 import importlib
 import inspect
 import argparse
-
-from langpack.utils import format, build_lib, find_obj_dynamic, launch_api
+import subprocess
+import logging
+import botocore
+
+from langpack.utils import (
+    build_lib,
+    find_obj_dynamic,
+    launch_api,
+    parse_env_file,
+    run_command,
+    run_docker_command,
+    zip_and_upload_to_s3,
+    download_and_unzip_file_from_s3,
+)
 
 agent_dir = "agent"
 chain_dir = "chain"
 embedding_dir = "embedding"
 request_wrapper_dir = "request_wrapper"
 vectorstore_dir = "vectorstore"
 static_dir = "static"
@@ -625,21 +637,146 @@
         print(app_config)
 
     dict_class = create_dict_deps("lib_" + app_config["source_name"])
 
     return _deserialize(app_config["dependency_dict"], dict_class)
 
 
-def deploy():
+def localtest():
     """
     Takes a package path and launch a flask backend service and a client to post request
     """
     parser = argparse.ArgumentParser()
     parser.add_argument("app_path", help="Python script file path")
     args = parser.parse_args()
 
     commands = [
         f"cd {args.app_path} && source $VIRTUAL_ENV/bin/activate && python app.py",
         f"cd {args.app_path} && source $VIRTUAL_ENV/bin/activate && python client.py",
     ]
 
     launch_api(commands)
+
+
+def push():
+    parser = argparse.ArgumentParser()
+    parser.add_argument("app_path", help="Local path of the app")
+    parser.add_argument(
+        "--instance",
+        type=str,
+        choices=["s3", "lambda"],
+        default="lambda",
+        help="Type of instance",
+    )
+    args = parser.parse_args()
+
+    if args.instance == "lambda":
+        lambda_cloud_key = os.environ["LAMBDA_CLOUD_KEY"]
+        remote_ip = os.environ["REMOTE_IP"]
+        if not lambda_cloud_key:
+            raise f"Please set the LAMBDA_CLOUD_KEY environment variable"
+        if not remote_ip:
+            raise f"Please set the REMOTE_IP environment variable"
+        command = f"scp -r -i {lambda_cloud_key} {args.app_path} {remote_ip}:~/"
+        run_command(command)
+    elif args.instance == "s3":
+        # # Enable debug logging
+        # logging.basicConfig(level=logging.DEBUG)
+
+        # # Enable debug logging for botocore
+        # botocore_session = botocore.session.Session()
+        # botocore_session.set_debug_logger()
+
+        destination_key = "langchain_apps/" + args.app_path.split("/")[-1] + ".zip"
+        zip_and_upload_to_s3(
+            args.app_path,
+            os.environ["AWS_S3_BUCKET"],
+            destination_key,
+            os.environ["AWS_S3_REGION"],
+        )
+    else:
+        raise f"Instance type {args.instance} is not supported"
+
+
+def deploy():
+    parser = argparse.ArgumentParser()
+    parser.add_argument(
+        "--instance",
+        type=str,
+        choices=["lambda"],
+        default="lambda",
+        help="Type of instance",
+    )
+    parser.add_argument("--app_url", default="", help="URL for fetching the app")
+    parser.add_argument("--app_path", default="", help="Path of app on the instance")
+    parser.add_argument(
+        "--environ_file",
+        type=str,
+        default="",
+        help="Path to env.list file that stores the environment variables like API keys",
+    )
+    args = parser.parse_args()
+
+    if not args.app_path and not args.app_url:
+        raise f"app_path and app_url are both missing. One of them needs to be set"
+
+    if args.environ_file:
+        env_str = parse_env_file(args.environ_file)
+    else:
+        env_str = ""
+
+    if args.instance == "lambda":
+        lambda_cloud_key = os.environ["LAMBDA_CLOUD_KEY"]
+        remote_ip = os.environ["REMOTE_IP"]
+        username = os.environ["USERNAME"]
+
+        if not lambda_cloud_key:
+            raise f"Please set the LAMBDA_CLOUD_KEY environment variable"
+        if not remote_ip:
+            raise f"Please set the REMOTE_IP environment variable"
+        if not username:
+            raise f"Please set the USERNAME environment variable"
+
+        if args.app_url:
+            # default path to save app on the remote instance
+            app_path = "/home/ubuntu/app"
+
+            # create an empty folder on remote server
+            command = f"ssh -i {lambda_cloud_key} {remote_ip} mkdir -p {app_path}"
+            run_command(command)
+
+            # download app to that folder
+            docker_command = f"sudo docker run --network host -v {app_path}:/app {env_str} chuanli11/langpack-ubuntu:22.04 download_app_from_s3 {args.app_url}"
+            run_docker_command(remote_ip, username, lambda_cloud_key, docker_command)
+
+        else:
+            # otherwise assuming the app is already downloaded on the
+            app_path = args.app_path
+
+        # Launch the app using docker
+        docker_command = f"sudo docker run --network host -v {app_path}:/app {env_str} -w /app chuanli11/langpack-ubuntu:22.04 python3 app.py"
+        run_docker_command(remote_ip, username, lambda_cloud_key, docker_command)
+
+    else:
+        raise f"Instance type {args.instance} is not supported"
+
+
+def download_app_from_s3():
+    parser = argparse.ArgumentParser()
+    parser.add_argument("s3_url", default="", help="S3 bucket URL for fetching the app")
+    args = parser.parse_args()
+
+    # download and unzip
+    cache_path = "/"
+    bucket_name = os.environ["AWS_S3_BUCKET"]
+    region = os.environ["AWS_S3_REGION"]
+    file_key = args.s3_url
+    target_file_path = os.path.join(cache_path, file_key.split("/")[-1])
+    print(target_file_path)
+    unzip_path = download_and_unzip_file_from_s3(
+        target_file_path, bucket_name, file_key, region
+    )
+
+    app_path = "/app"
+    shutil.move(unzip_path, app_path)
+
+    print(f"App successfully unzipped to {app_path}")
```

## langpack/utils.py

```diff
@@ -3,14 +3,16 @@
 import io
 import astpretty
 import astor
 import os
 import sys
 from types import FunctionType
 import subprocess
+import zipfile
+import boto3
 
 
 class Unparser(OriginalUnparser):
     def _Constant(self, t):
         if isinstance(t.value, str):
             self.write(repr(t.value))
         else:
@@ -248,7 +250,94 @@
     # Adjust the layout of the panes to 'even-horizontal'
     subprocess.run(["tmux", "select-layout", "-t", "api_session", "even-horizontal"])
 
     # Attach to the tmux session
     subprocess.run(
         ["gnome-terminal", "--", "tmux", "attach-session", "-t", "api_session"]
     )
+
+
+def parse_env_file(file_path):
+    with open(file_path, "r") as f:
+        lines = f.readlines()
+
+    env_vars = []
+    for line in lines:
+        line = line.strip()
+        if line:
+            key, value = line.split("=", 1)
+            env_vars.append(f'-e {key}="{value}"')
+
+    return " ".join(env_vars)
+
+
+def run_command(command):
+    result = subprocess.run(
+        command, stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True, text=True
+    )
+
+    if result.returncode == 0:
+        print(f"{command} completed successfully.")
+        print(result.stdout.strip())
+    else:
+        print(result.stderr.strip())
+        raise f"{command} failed."
+
+
+def run_docker_command(hostname, username, lambda_cloud_key, command):
+    ssh_command = f"ssh -i {lambda_cloud_key} {username}@{hostname} {command}"
+
+    with open(os.devnull, "w") as devnull:
+        result = subprocess.Popen(
+            ssh_command,
+            stdin=devnull,
+            stdout=devnull,
+            stderr=devnull,
+            shell=True,
+            start_new_session=True,
+        )
+
+    print(f"App launched at http://{hostname}:5000/predict")
+
+
+def zip_and_upload_to_s3(source_folder, destination_bucket, destination_key, region):
+    # Create a new zip file
+    zip_filename = source_folder + ".zip"
+    with zipfile.ZipFile(zip_filename, "w", zipfile.ZIP_DEFLATED) as zip_file:
+        # Add all files in the source folder to the zip file
+        for root, dirs, files in os.walk(source_folder):
+            for file in files:
+                file_path = os.path.join(root, file)
+                zip_file.write(file_path, file_path.replace(source_folder, "", 1))
+
+    # Upload the zip file to S3
+    s3_client = boto3.client("s3", region_name=region)
+    with open(zip_filename, "rb") as data:
+        s3_client.upload_fileobj(data, destination_bucket, destination_key)
+
+    # Clean up the temporary zip file
+    os.remove(zip_filename)
+
+
+def download_and_unzip_file_from_s3(target_file_path, bucket_name, file_key, region):
+    """
+    Download a file from an Amazon S3 bucket.
+
+    :param bucket_name: The name of the S3 bucket.
+    :param file_key: The key (path) of the file in the S3 bucket.
+    :param local_file_path: The local file path where the downloaded file will be saved.
+    """
+    s3 = boto3.client("s3", region_name=region)
+    try:
+        s3.download_file(bucket_name, file_key, target_file_path)
+        print(f"File downloaded successfully to {target_file_path}")
+
+        # Unzip the downloaded file
+        unzip_path = ".".join(target_file_path.split(".")[:-1])
+        with zipfile.ZipFile(target_file_path, "r") as zip_ref:
+            zip_ref.extractall(unzip_path)
+        print(f"File unzipped successfully to {unzip_path}")
+
+        return unzip_path
+
+    except Exception as e:
+        print(f"Error downloading or unzipping file: {e}")
```

## Comparing `langpack-0.0.3.dist-info/METADATA` & `langpack-0.0.4.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: langpack
-Version: 0.0.3
+Version: 0.0.4
 Summary: A library to pakcage and deploy langugage model apps
 Home-page: UNKNOWN
 Author: Chuan Li
 Author-email: c@lambdalabs.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Dist: apify-client (==1.0.0)
 Requires-Dist: astor (==0.8.1)
 Requires-Dist: astpretty (==3.0.0)
 Requires-Dist: astunparse (==1.6.3)
+Requires-Dist: boto3 (==1.26.120)
 Requires-Dist: chromadb (==0.3.21)
 Requires-Dist: faiss-cpu (==1.7.3)
 Requires-Dist: flask (==2.2.3)
 Requires-Dist: google-api-python-client (==2.85.0)
 Requires-Dist: google-search-results (==2.4.2)
 Requires-Dist: langchain (==0.0.139)
 Requires-Dist: numpy (<1.24.0)
```

## Comparing `langpack-0.0.3.dist-info/RECORD` & `langpack-0.0.4.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 langpack/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 langpack/app_template.py,sha256=Athx3xBnaw3twNdjtR_qbM37CRXj8-iL2e8CL0vjoaY,857
 langpack/client_template.py,sha256=76uiHaqX-YNpbl4yd62a-V1dXV5S0tcxbTXYOsGTQfI,611
 langpack/index.html,sha256=BQdpj0HZwhSfctr69ZeddzalBGHAp3WCb-LM6rkIzJM,2787
 langpack/tester.py,sha256=PoDgNQe_fis7y6ZsQOITTF6M1svBZ-Sp2cE5EqTRadU,7528
-langpack/tools.py,sha256=Yg6yrUoZ9fgNU7rMErYoTS5YCeP-m9adAkDZ5JvDeYY,21745
-langpack/utils.py,sha256=2fmcJwHpoSgnscrJ47ZFYXFToIEWazooo75VQNcbTP0,7512
-langpack-0.0.3.dist-info/METADATA,sha256=M_HUoqbnM00711-pDp14lkEkjb9H9eZw2kVGmo9YxWI,871
-langpack-0.0.3.dist-info/WHEEL,sha256=kGT74LWyRUZrL4VgLh6_g12IeVl_9u9ZVhadrgXZUEY,110
-langpack-0.0.3.dist-info/entry_points.txt,sha256=tr9PNRuctA7z6aoVqeR4pND15CtSHpq6v-Bmjfyipyw,77
-langpack-0.0.3.dist-info/top_level.txt,sha256=j92Fj-GurEfjdOLmRWAy5wdVGVoOFqkhz6grAYs19Yw,9
-langpack-0.0.3.dist-info/RECORD,,
+langpack/tools.py,sha256=Oxci81wbd1V8TmLcUHvfGqWWG6A-5OjqzEHCNv02vw4,26333
+langpack/utils.py,sha256=wB2UO64xwHXBGG1bKslPjIFinqANhX10T4_-YGct570,10404
+langpack-0.0.4.dist-info/METADATA,sha256=G5cVNZ-E8C2CUGy0HDhaWWlJyZ_zfMJ4hbL2bBkGYlw,905
+langpack-0.0.4.dist-info/WHEEL,sha256=kGT74LWyRUZrL4VgLh6_g12IeVl_9u9ZVhadrgXZUEY,110
+langpack-0.0.4.dist-info/entry_points.txt,sha256=75SUv2OYYKWRl1QtqkCrb1Kt0LbnrXOHG7Iy5e4E71M,200
+langpack-0.0.4.dist-info/top_level.txt,sha256=j92Fj-GurEfjdOLmRWAy5wdVGVoOFqkhz6grAYs19Yw,9
+langpack-0.0.4.dist-info/RECORD,,
```

