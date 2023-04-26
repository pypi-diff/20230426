# Comparing `tmp/wasabit-0.1.tar.gz` & `tmp/wasabit-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wasabit-0.1.tar", last modified: Tue Feb 14 11:08:34 2023, max compression
+gzip compressed data, was "wasabit-0.2.tar", last modified: Wed Apr 26 02:38:38 2023, max compression
```

## Comparing `wasabit-0.1.tar` & `wasabit-0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-02-14 11:08:34.315777 wasabit-0.1/
--rw-rw-rw-   0        0        0     1111 2023-02-07 10:10:53.000000 wasabit-0.1/LICENSE
--rw-rw-rw-   0        0        0      246 2023-02-14 11:08:34.313772 wasabit-0.1/PKG-INFO
--rw-rw-rw-   0        0        0      985 2023-02-07 15:56:58.000000 wasabit-0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-02-14 11:08:34.316773 wasabit-0.1/setup.cfg
--rw-rw-rw-   0        0        0      568 2023-02-14 11:08:23.000000 wasabit-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-14 11:08:34.286775 wasabit-0.1/wasabit/
--rw-rw-rw-   0        0        0        2 2023-02-07 10:12:01.000000 wasabit-0.1/wasabit/__init__.py
--rw-rw-rw-   0        0        0     1129 2023-02-14 10:46:58.000000 wasabit-0.1/wasabit/wasabi_auth.py
--rw-rw-rw-   0        0        0     1626 2023-01-11 11:10:04.000000 wasabit-0.1/wasabit/wasabi_download.py
--rw-rw-rw-   0        0        0     5480 2023-02-14 10:51:11.000000 wasabit-0.1/wasabit/wasabi_upload.py
-drwxrwxrwx   0        0        0        0 2023-02-14 11:08:34.310784 wasabit-0.1/wasabit.egg-info/
--rw-rw-rw-   0        0        0      246 2023-02-14 11:08:33.000000 wasabit-0.1/wasabit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      275 2023-02-14 11:08:33.000000 wasabit-0.1/wasabit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-14 11:08:33.000000 wasabit-0.1/wasabit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      119 2023-02-14 11:08:33.000000 wasabit-0.1/wasabit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-02-14 11:08:33.000000 wasabit-0.1/wasabit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-26 02:38:38.551702 wasabit-0.2/
+-rw-rw-rw-   0        0        0     1111 2023-02-07 10:10:53.000000 wasabit-0.2/LICENSE
+-rw-rw-rw-   0        0        0      395 2023-04-26 02:38:38.549720 wasabit-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1172 2023-04-17 04:24:02.000000 wasabit-0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-26 02:38:38.551702 wasabit-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      745 2023-04-26 02:37:16.000000 wasabit-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 02:38:38.524715 wasabit-0.2/wasabit/
+-rw-rw-rw-   0        0        0        2 2023-02-07 10:12:01.000000 wasabit-0.2/wasabit/__init__.py
+-rw-rw-rw-   0        0        0     1113 2023-02-14 12:21:20.000000 wasabit-0.2/wasabit/wasabi_auth.py
+-rw-rw-rw-   0        0        0     1626 2023-01-11 11:10:04.000000 wasabit-0.2/wasabit/wasabi_download.py
+-rw-rw-rw-   0        0        0     6346 2023-04-26 02:36:19.000000 wasabit-0.2/wasabit/wasabi_upload.py
+drwxrwxrwx   0        0        0        0 2023-04-26 02:38:38.545703 wasabit-0.2/wasabit.egg-info/
+-rw-rw-rw-   0        0        0      395 2023-04-26 02:38:37.000000 wasabit-0.2/wasabit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      275 2023-04-26 02:38:38.000000 wasabit-0.2/wasabit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 02:38:37.000000 wasabit-0.2/wasabit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      119 2023-04-26 02:38:37.000000 wasabit-0.2/wasabit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-26 02:38:37.000000 wasabit-0.2/wasabit.egg-info/top_level.txt
```

### Comparing `wasabit-0.1/LICENSE` & `wasabit-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wasabit-0.1/README.md` & `wasabit-0.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -3,28 +3,32 @@
 This package offers a solution for uploading files, creating folders, and authenticating with Wasabi. It contains scripts to simplify file uploads, folder creation, and authentication to the Wasabi environment. Streamline your Wasabi workflows with this package as a starting point for further customization and development.
 
 ## Installation
 
 Use the package manager [pip](https://github.com/bippisb/wasabit.git) to install wasabit.
 
 ```bash
-pip install git+https://github.com/bippisb/wasabit.git
+pip install wasabit
 ```
 
 ## Usage
 
 ```python
 from wasabit.wasabi_auth import wasabi_auth
 from wasabit.wasabi_upload import upload_to_wasabi
 
-# returns 's3 client'
-s3 = wasabi_auth()
+ACCESS_KEY = "YOUR WASABI_ACCESS_KEY"
+WASABI_SECRET = "YOUR WASABI_SECRET_KEY"
+
+bucket_name = 'dev-data'
+wasabi_path = 'DGCIS_EXPORT_ALL_HS/processed/Final/'
+folder_path = "D:/Saurabh/data/processed/Final/"
 
 # 'upload data to wasabi'
-upload_to_wasabi(folder_path, bucket_name,wasabi_path)
+upload_to_wasabi(folder_path, bucket_name,wasabi_path,access_key = ACCESS_KEY, secret_key = WASABI_SECRET)
 
 ```
 
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first
 to discuss what you would like to change.
```

### Comparing `wasabit-0.1/wasabit/wasabi_auth.py` & `wasabit-0.2/wasabit/wasabi_auth.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import json
 import os
 import boto3
 
 # from botocore.exceptions import NoCredentialsError
 
 
-import boto3
-
 def wasabi_auth(ACCESS_KEY, WASABI_SECRET):
     """
     Creates an authenticated client for interacting with an S3 bucket hosted on the Wasabi cloud storage service.
     
     Args:
     ACCESS_KEY (str): Wasabi Access Key
     WASABI_SECRET (str): Wasabi Secret Key
```

### Comparing `wasabit-0.1/wasabit/wasabi_download.py` & `wasabit-0.2/wasabit/wasabi_download.py`

 * *Files identical despite different names*

### Comparing `wasabit-0.1/wasabit/wasabi_upload.py` & `wasabit-0.2/wasabit/wasabi_upload.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,54 +2,18 @@
 import boto3
 from boto3.s3.transfer import TransferConfig
 from botocore.exceptions import NoCredentialsError, ClientError
 from wasabit.wasabi_auth import wasabi_auth
 import os
 from botocore.exceptions import NoCredentialsError
 
-
-def wasabi_upload(s3, bucket_name, wasabi_path, local_file_path):
-    """
-    function to upload files from local to wasabi, it will create folder path for the dataset that we
-    are wroking on and add the files from local path.
-
-    params:
-    s3 : Element which returns after authentication using wasabi_auth function
-    bucket_name: dev-data or prod-data
-    wasabi_path: dataset_name + (data path from monorepo) | Ex: agcensus/raw/andhra_pradesh/anantapur/data.csv
-    local_file_path: path of file in the system in which processing is being done.
-    """
-    for bucket in s3.list_buckets()["Buckets"]:
-        if bucket["Name"] == bucket_name:
-            print(bucket_name + " bucket already exists")
-            wasabi_bucket = bucket_name
-            pass
-        else:
-            wasabi_bucket = s3.create_bucket(Bucket=bucket_name)
-
-    def upload_to_wasabi(file_name, bucket, data):
-        """
-        Function to upload a dataset on to the wasabi cloud
-        """
-        try:
-            s3.put_object(Bucket=bucket_name, Key=file_name, Body=data)
-            print("Upload Successful")
-            return True
-        except FileNotFoundError:
-            print("The file was not found")
-            return False
-        except NoCredentialsError:
-            print("Credentials not available")
-            return False
-
-    data = open(local_file_path, "rb")
-    wasabi_bucket = bucket_name
-    # invoking the upload function to wasabi or amazon s3.
-    upload_to_wasabi(wasabi_path, wasabi_bucket, data)
-    print("file uploaded to wasabi on this path: ", wasabi_path)
+import os
+from pathlib import Path
+from typing import Optional
+import boto3
 
 
 
 def upload_to_wasabi(folder_path: str, bucket_name: str, wasabi_path: str, access_key = None, secret_key = None) -> None:
     """
     Uploads all files present in a specific folder to a specified Wasabi bucket and subfolder or prefix.
     :param folder_path: The path of the folder containing the files to be uploaded.
@@ -117,8 +81,54 @@
         if e.response['Error']['Code'] == "InvalidAccessKeyId":
             print("Invalid access key, please check your access key.")
         elif e.response['Error']['Code'] == "SignatureDoesNotMatch":
             print("Invalid secret key, please check your secret key.")
         else:
             print(f'An error occurred: {e}')
     except Exception as e:
-        print(f'An error occurred: {e}')
+        print(f'An error occurred: {e}')
+
+
+def upload_folder_to_wasabi(local_folder_path: str, bucket_name: str, wasabi_path: str, access_key: str, secret_key: str) -> None:
+    """
+    Recursively uploads all files present in a specific folder to a specified Wasabi bucket and subfolder or prefix.
+    :param local_folder_path: The path of the local folder containing the files to be uploaded.
+    :param bucket_name: The name of the Wasabi bucket where the files will be uploaded.
+    :param wasabi_path: The prefix or subfolder within the bucket where the files will be uploaded. Optional.
+    :param access_key: The Wasabi access key.
+    :param secret_key: The Wasabi secret key.
+    """
+    transfer_config = TransferConfig(
+        multipart_threshold=1024 * 25,  # 25MB
+        max_concurrency=10,
+        num_download_attempts=10,
+    )
+    try:
+        # create an S3 client
+        s3 = boto3.client('s3',
+                          endpoint_url='https://s3.ap-southeast-1.wasabisys.com',
+                          aws_access_key_id=access_key,
+                          aws_secret_access_key=secret_key)
+
+        # convert folder path to platform-independent path
+        local_folder_path = Path(local_folder_path).resolve()
+        for root, dirs, files in os.walk(local_folder_path):
+            for file in files:
+                # get local file path and remote file path
+                local_file_path = os.path.join(root, file)
+                relative_path = os.path.relpath(local_file_path, local_folder_path)
+                remote_file_path = os.path.join(wasabi_path, relative_path).replace(os.sep, '/')
+                
+                # upload the file
+                s3.upload_file(local_file_path, bucket_name, remote_file_path, Config=transfer_config)
+                print(f'{local_file_path} is uploaded to {remote_file_path}')
+    except NoCredentialsError as e:
+        print("Credentials not found, please check your access key and secret key.")
+    except ClientError as e:
+        if e.response['Error']['Code'] == "InvalidAccessKeyId":
+            print("Invalid access key, please check your access key.")
+        elif e.response['Error']['Code'] == "SignatureDoesNotMatch":
+            print("Invalid secret key, please check your secret key.")
+        else:
+            print(f'An error occurred: {e}')
+    except Exception as e:
+        print(f'An error occurred: {e}')
```

