# Comparing `tmp/wasabit-0.2.tar.gz` & `tmp/wasabit-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wasabit-0.2.tar", last modified: Wed Apr 26 02:38:38 2023, max compression
+gzip compressed data, was "wasabit-0.2.1.tar", last modified: Wed Apr 26 18:17:25 2023, max compression
```

## Comparing `wasabit-0.2.tar` & `wasabit-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 02:38:38.551702 wasabit-0.2/
--rw-rw-rw-   0        0        0     1111 2023-02-07 10:10:53.000000 wasabit-0.2/LICENSE
--rw-rw-rw-   0        0        0      395 2023-04-26 02:38:38.549720 wasabit-0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1172 2023-04-17 04:24:02.000000 wasabit-0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-04-26 02:38:38.551702 wasabit-0.2/setup.cfg
--rw-rw-rw-   0        0        0      745 2023-04-26 02:37:16.000000 wasabit-0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-26 02:38:38.524715 wasabit-0.2/wasabit/
--rw-rw-rw-   0        0        0        2 2023-02-07 10:12:01.000000 wasabit-0.2/wasabit/__init__.py
--rw-rw-rw-   0        0        0     1113 2023-02-14 12:21:20.000000 wasabit-0.2/wasabit/wasabi_auth.py
--rw-rw-rw-   0        0        0     1626 2023-01-11 11:10:04.000000 wasabit-0.2/wasabit/wasabi_download.py
--rw-rw-rw-   0        0        0     6346 2023-04-26 02:36:19.000000 wasabit-0.2/wasabit/wasabi_upload.py
-drwxrwxrwx   0        0        0        0 2023-04-26 02:38:38.545703 wasabit-0.2/wasabit.egg-info/
--rw-rw-rw-   0        0        0      395 2023-04-26 02:38:37.000000 wasabit-0.2/wasabit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      275 2023-04-26 02:38:38.000000 wasabit-0.2/wasabit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 02:38:37.000000 wasabit-0.2/wasabit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      119 2023-04-26 02:38:37.000000 wasabit-0.2/wasabit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-26 02:38:37.000000 wasabit-0.2/wasabit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-26 18:17:25.584054 wasabit-0.2.1/
+-rw-rw-rw-   0        0        0     1111 2023-02-07 10:10:53.000000 wasabit-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0      397 2023-04-26 18:17:25.581698 wasabit-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1172 2023-04-17 04:24:02.000000 wasabit-0.2.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-26 18:17:25.584054 wasabit-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      747 2023-04-26 18:16:42.000000 wasabit-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 18:17:25.540445 wasabit-0.2.1/wasabit/
+-rw-rw-rw-   0        0        0        2 2023-02-07 10:12:01.000000 wasabit-0.2.1/wasabit/__init__.py
+-rw-rw-rw-   0        0        0     1113 2023-02-14 12:21:20.000000 wasabit-0.2.1/wasabit/wasabi_auth.py
+-rw-rw-rw-   0        0        0     1626 2023-01-11 11:10:04.000000 wasabit-0.2.1/wasabit/wasabi_download.py
+-rw-rw-rw-   0        0        0     6631 2023-04-26 18:10:49.000000 wasabit-0.2.1/wasabit/wasabi_upload.py
+drwxrwxrwx   0        0        0        0 2023-04-26 18:17:25.578544 wasabit-0.2.1/wasabit.egg-info/
+-rw-rw-rw-   0        0        0      397 2023-04-26 18:17:25.000000 wasabit-0.2.1/wasabit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      275 2023-04-26 18:17:25.000000 wasabit-0.2.1/wasabit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 18:17:25.000000 wasabit-0.2.1/wasabit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      119 2023-04-26 18:17:25.000000 wasabit-0.2.1/wasabit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-26 18:17:25.000000 wasabit-0.2.1/wasabit.egg-info/top_level.txt
```

### Comparing `wasabit-0.2/LICENSE` & `wasabit-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wasabit-0.2/README.md` & `wasabit-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `wasabit-0.2/setup.py` & `wasabit-0.2.1/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='wasabit',
-    version='0.2',
+    version='0.2.1',
     description='This package offers a solution for uploading files, creating folders, and authenticating with Wasabi',
     author='Saurabh Harak',
     author_email='saurabh_harak@isb.edu',
     packages=find_packages(),
     classifiers=[
          "Programming Language :: Python :: 3",
          "License :: OSI Approved :: MIT License",
```

### Comparing `wasabit-0.2/wasabit/wasabi_auth.py` & `wasabit-0.2.1/wasabit/wasabi_auth.py`

 * *Files identical despite different names*

### Comparing `wasabit-0.2/wasabit/wasabi_download.py` & `wasabit-0.2.1/wasabit/wasabi_download.py`

 * *Files identical despite different names*

### Comparing `wasabit-0.2/wasabit/wasabi_upload.py` & `wasabit-0.2.1/wasabit/wasabi_upload.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 # import json
 import boto3
 from boto3.s3.transfer import TransferConfig
 from botocore.exceptions import NoCredentialsError, ClientError
 from wasabit.wasabi_auth import wasabi_auth
 import os
 from botocore.exceptions import NoCredentialsError
-
-import os
 from pathlib import Path
-from typing import Optional
-import boto3
 
 
 
 def upload_to_wasabi(folder_path: str, bucket_name: str, wasabi_path: str, access_key = None, secret_key = None) -> None:
     """
     Uploads all files present in a specific folder to a specified Wasabi bucket and subfolder or prefix.
     :param folder_path: The path of the folder containing the files to be uploaded.
@@ -48,14 +44,16 @@
         else:
             print(f'An error occurred: {e}')
     except Exception as e:
         print(f'An error occurred: {e}')
 
         
 
+
+
 def file_upload_to_wasabi(csv_file_path: str, bucket_name: str, wasabi_path: str, access_key, secret_key) -> None:
     """
     Uploads a specific CSV file to a specified Wasabi bucket and subfolder or prefix.
     :param csv_file_path: The full path of the CSV file to be uploaded.
     :param bucket_name: The name of the Wasabi bucket where the file will be uploaded.
     :param wasabi_path: The prefix or subfolder within the bucket where the file will be uploaded.
     :param access_key: The Wasabi access key.
@@ -67,15 +65,15 @@
         num_download_attempts=10,
     )
     try:
         # create an S3 client
         s3 = wasabi_auth(access_key,secret_key)
         # get the file name from the full path
         file_name = os.path.basename(csv_file_path)
-        remote_file = wasabi_path + file_name
+        remote_file = os.path.join(wasabi_path, file_name)
         # upload the file
         s3.upload_file(csv_file_path, bucket_name, remote_file, Config=transfer_config)
         print(f'{csv_file_path} is uploaded to {remote_file}')
     except NoCredentialsError as e:
         print("Credentials not found, please check your access key and secret key.")
     except ClientError as e:
         if e.response['Error']['Code'] == "InvalidAccessKeyId":
@@ -84,14 +82,21 @@
             print("Invalid secret key, please check your secret key.")
         else:
             print(f'An error occurred: {e}')
     except Exception as e:
         print(f'An error occurred: {e}')
 
 
+
+import os
+import boto3
+from botocore.exceptions import NoCredentialsError, ClientError
+from pathlib import Path
+
+
 def upload_folder_to_wasabi(local_folder_path: str, bucket_name: str, wasabi_path: str, access_key: str, secret_key: str) -> None:
     """
     Recursively uploads all files present in a specific folder to a specified Wasabi bucket and subfolder or prefix.
     :param local_folder_path: The path of the local folder containing the files to be uploaded.
     :param bucket_name: The name of the Wasabi bucket where the files will be uploaded.
     :param wasabi_path: The prefix or subfolder within the bucket where the files will be uploaded. Optional.
     :param access_key: The Wasabi access key.
@@ -114,14 +119,18 @@
         for root, dirs, files in os.walk(local_folder_path):
             for file in files:
                 # get local file path and remote file path
                 local_file_path = os.path.join(root, file)
                 relative_path = os.path.relpath(local_file_path, local_folder_path)
                 remote_file_path = os.path.join(wasabi_path, relative_path).replace(os.sep, '/')
                 
+                # create the target folder if it does not already exist
+                if wasabi_path:
+                    s3.put_object(Bucket=bucket_name, Key=f"{wasabi_path}/")
+                
                 # upload the file
                 s3.upload_file(local_file_path, bucket_name, remote_file_path, Config=transfer_config)
                 print(f'{local_file_path} is uploaded to {remote_file_path}')
     except NoCredentialsError as e:
         print("Credentials not found, please check your access key and secret key.")
     except ClientError as e:
         if e.response['Error']['Code'] == "InvalidAccessKeyId":
```

