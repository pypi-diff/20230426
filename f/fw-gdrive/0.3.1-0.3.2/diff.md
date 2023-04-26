# Comparing `tmp/fw_gdrive-0.3.1-py3-none-any.whl.zip` & `tmp/fw_gdrive-0.3.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 9073 bytes, number of entries: 7
+Zip file size: 9381 bytes, number of entries: 7
 -rw-r--r--  2.0 unx      316 b- defN 80-Jan-01 00:00 fw_gdrive/__init__.py
--rw-r--r--  2.0 unx    15681 b- defN 80-Jan-01 00:00 fw_gdrive/gapi.py
--rw-r--r--  2.0 unx     6571 b- defN 80-Jan-01 00:00 fw_gdrive/utils.py
--rw-r--r--  2.0 unx     1078 b- defN 80-Jan-01 00:00 fw_gdrive-0.3.1.dist-info/LICENSE
-?rw-r--r--  2.0 unx       83 b- defN 16-Jan-01 00:00 fw_gdrive-0.3.1.dist-info/WHEEL
-?rw-r--r--  2.0 unx     3172 b- defN 16-Jan-01 00:00 fw_gdrive-0.3.1.dist-info/METADATA
-?rw-r--r--  2.0 unx      529 b- defN 16-Jan-01 00:00 fw_gdrive-0.3.1.dist-info/RECORD
-7 files, 27430 bytes uncompressed, 8147 bytes compressed:  70.3%
+-rw-r--r--  2.0 unx    17796 b- defN 80-Jan-01 00:00 fw_gdrive/gapi.py
+-rw-r--r--  2.0 unx     6569 b- defN 80-Jan-01 00:00 fw_gdrive/utils.py
+-rw-r--r--  2.0 unx     1078 b- defN 80-Jan-01 00:00 fw_gdrive-0.3.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3223 b- defN 80-Jan-01 00:00 fw_gdrive-0.3.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fw_gdrive-0.3.2.dist-info/WHEEL
+?rw-r--r--  2.0 unx      529 b- defN 16-Jan-01 00:00 fw_gdrive-0.3.2.dist-info/RECORD
+7 files, 29599 bytes uncompressed, 8455 bytes compressed:  71.4%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: fw_gdrive/gapi.py
 Comment: 
 
 Filename: fw_gdrive/utils.py
 Comment: 
 
-Filename: fw_gdrive-0.3.1.dist-info/LICENSE
+Filename: fw_gdrive-0.3.2.dist-info/LICENSE
 Comment: 
 
-Filename: fw_gdrive-0.3.1.dist-info/WHEEL
+Filename: fw_gdrive-0.3.2.dist-info/METADATA
 Comment: 
 
-Filename: fw_gdrive-0.3.1.dist-info/METADATA
+Filename: fw_gdrive-0.3.2.dist-info/WHEEL
 Comment: 
 
-Filename: fw_gdrive-0.3.1.dist-info/RECORD
+Filename: fw_gdrive-0.3.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fw_gdrive/gapi.py

```diff
@@ -1,25 +1,24 @@
 """Google API, files and documents helpers."""
 import os
 import re
 import time
 import typing as t
 from pathlib import Path
 
-import googleapiclient.discovery as discovery
 import googleapiclient.errors as err
 import httplib2
 import oauth2client
+from googleapiclient import discovery
 from googleapiclient.errors import HttpError
 from googleapiclient.http import MediaFileUpload
 from httplib2 import Http
-from oauth2client.client import GoogleCredentials
 from oauth2client.service_account import ServiceAccountCredentials
 
-import fw_gdrive.utils as utils
+from fw_gdrive import utils
 
 DISCOVERY_DOC = "https://docs.googleapis.com/$discovery/rest?version=v1"
 
 
 class GoogleAPIClient:
     """Instantiate Google API Client for Google Drive and Google Documents services.
 
@@ -46,16 +45,16 @@
         """Initialize Google API client."""
         if service_cred_path is None:
             # Try to retrieve the path from env variable
             try:
                 service_cred_path = os.environ["SERVICE_ACCOUNT"]
             except KeyError:
                 raise RuntimeError(
-                    f"$SERVICE_ACCOUNT is not set up as an environment variable. "
-                    f"Unable to locate service cred path."
+                    "$SERVICE_ACCOUNT is not set up as an environment variable. "
+                    "Unable to locate service cred path."
                 )
 
         self.svc_acc_cred = utils.login(service_cred_path, scopes)
         self.drive_service = self._get_api_client(
             svc_acc_cred=self.svc_acc_cred, service="drive", version="v3"
         )
         self.doc_service = self._get_api_client(
@@ -351,50 +350,103 @@
                 raise RuntimeError("Uncaught Exception.") from exc
             else:
                 uploaded = True
                 file_id = file.get("id")
                 return GoogleDocsFile(file_id, self.api_client.doc_service)
         return None
 
-    def get_file_list(self) -> t.List[t.Dict]:
+    def get_file_list_from_folder(self, sub_folder_id: str = None) -> t.List[t.Dict]:
         """Retrieve a list of file object that is stored in the Google Drive Folder."""
         file_list = list()
         # Access the files in folder
-        query = f"parents in '{self.folder_id}'"
+        if not sub_folder_id:
+            # find files in the base level of the shared drive folder if not provided
+            sub_folder_id = self.folder_id
+        query = f"'{sub_folder_id}' in parents and mimeType = 'application/vnd.google-apps.file'"
+
         try:
             response = (
                 self.folder_cred.files()
-                .list(q=query, includeItemsFromAllDrives=True, supportsAllDrives=True)
+                .list(
+                    q=query,
+                    corpora="drive",
+                    driveId=self.folder_id,
+                    includeItemsFromAllDrives=True,
+                    supportsAllDrives=True,
+                )
                 .execute()
             )
 
             file_list = response.get("files")
             nextPageToken = response.get("nextPageToken")
 
             while nextPageToken:
                 response = (
                     self.folder_cred.files()
                     .list(
-                        q=query, includeItemsFromAllDrives=True, supportsAllDrives=True
+                        q=query,
+                        corpora="drive",
+                        driveId=self.folder_id,
+                        includeItemsFromAllDrives=True,
+                        supportsAllDrives=True,
                     )
                     .execute()
                 )
                 file_list.extend(response.get("files"))
                 nextPageToken = response.get("nextPageToken")
         except HttpError as e:
             reason = str(e._get_reason).split('"')[-2]
             raise RuntimeError(f"Error occurred. Reason: {reason}")
         except Exception as exc:
             raise Exception("Uncaught Exception.") from exc
 
         return file_list
 
-    def get_file_id_by_name(self, file_name: str) -> list:
+    def list_folders_in_folder(self, sub_folder_id: str = None):
+        folders_list = list()
+        # Access the files in folder
+        if not sub_folder_id:
+            # find files in original shared drive or shared folder if not provided
+            sub_folder_id = self.folder_id
+
+        query = f"'{sub_folder_id}' in parents and mimeType = 'application/vnd.google-apps.folder'"
+
+        page_token = None
+
+        while True:
+            try:
+                response = (
+                    self.folder_cred.files()
+                    .list(
+                        q=query,
+                        corpora="drive",
+                        driveId=self.folder_id,
+                        includeItemsFromAllDrives=True,
+                        supportsAllDrives=True,
+                        fields="nextPageToken, " "files(id, name, mimeType)",
+                        pageToken=page_token,
+                    )
+                    .execute()
+                )
+                folders_list.extend(response.get("files", []))
+                page_token = response.get("nextPageToken", None)
+                if page_token is None:
+                    break
+            except HttpError as e:
+                reason = str(e._get_reason).split('"')[-2]
+                raise RuntimeError(f"Error occurred. Reason: {reason}")
+            except Exception as exc:
+                raise Exception("Uncaught Exception.") from exc
+
+        return folders_list
+
+    def get_file_id_by_name(self, file_name: str, sub_folder_id: str = None) -> list:
         """Retrieve file ID based on provided file name."""
-        file_list = self.get_file_list()
+        # if sub_folder_id not provided it will look at the base level of the shared drive/folder (self.folder_id)
+        file_list = self.get_file_list_from_folder(sub_folder_id)
         f_ids = list()
         for file in file_list:
             if file.get("name") == file_name:
                 f_id = file.get("id")
                 f_ids.append(f_id)
         return f_ids
```

## fw_gdrive/utils.py

```diff
@@ -133,15 +133,14 @@
     return {"updateDocumentStyle": {"documentStyle": doc_style_dict, "fields": fields}}
 
 
 def insert_page_break(index: t.Union[int, str]) -> t.Dict:  # noqa: D103
     try:
         mod_index = int(index)
     except ValueError:
-
         raise ValueError(
             f"Invalid index. Expecting index to be number. Got {index} instead."
         )
     return {
         "insertPageBreak": {
             "location": {"index": mod_index},
         }
@@ -202,15 +201,14 @@
             raise ValueError(
                 f"{k} is not a valid key value. Only accept startIndex or endIndex. (case sensitive) "
             )
         if not isinstance(v, int):
             try:
                 mod_v = int(v)
             except ValueError:
-
                 raise ValueError(
                     f"Invalid index. Expecting index to be number. Got {v} instead."
                 )
             else:
                 range_dict_copy[k] = mod_v
 
     return range_dict_copy
```

## Comparing `fw_gdrive-0.3.1.dist-info/LICENSE` & `fw_gdrive-0.3.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fw_gdrive-0.3.1.dist-info/METADATA` & `fw_gdrive-0.3.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: fw-gdrive
-Version: 0.3.1
+Version: 0.3.2
 Summary: Flyweheel Google Drive Integration Tools
 Home-page: https://gitlab.com/flywheel-io/tools/lib/fw-gdrive
 License: MIT
 Keywords: Flywheel
 Author: Flywheel
 Author-email: support@flywheel.io
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: google-api-python-client (>=2.32.0,<3.0.0)
 Requires-Dist: oauth2client (>=4.1.3,<5.0.0)
 Project-URL: Documentation, https://gitlab.com/flywheel-io/tools/lib/fw-gdrive
 Project-URL: Repository, https://gitlab.com/flywheel-io/tools/lib/fw-gdrive
 Description-Content-Type: text/markdown
```

