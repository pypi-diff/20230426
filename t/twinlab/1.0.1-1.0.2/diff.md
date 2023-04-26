# Comparing `tmp/twinlab-1.0.1.tar.gz` & `tmp/twinlab-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twinlab-1.0.1.tar", max compression
+gzip compressed data, was "twinlab-1.0.2.tar", max compression
```

## Comparing `twinlab-1.0.1.tar` & `twinlab-1.0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1048 2023-04-11 12:00:19.210453 twinlab-1.0.1/README.md
--rw-r--r--   0        0        0      599 2023-04-20 12:03:06.858031 twinlab-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      528 2023-04-19 16:13:39.405689 twinlab-1.0.1/twinlab/__init__.py
--rw-r--r--   0        0        0     4811 2023-04-20 11:59:57.583783 twinlab-1.0.1/twinlab/client.py
--rw-r--r--   0        0        0      505 2023-04-13 16:09:18.757239 twinlab-1.0.1/twinlab/plotting.py
--rw-r--r--   0        0        0      532 2023-04-11 15:58:49.585681 twinlab-1.0.1/twinlab/settings.py
--rw-r--r--   0        0        0     3864 2023-04-19 16:13:39.406342 twinlab-1.0.1/twinlab/utils.py
--rw-r--r--   0        0        0     1624 1970-01-01 00:00:00.000000 twinlab-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1048 2023-04-11 12:00:19.210453 twinlab-1.0.2/README.md
+-rw-r--r--   0        0        0      599 2023-04-26 15:55:35.645951 twinlab-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      528 2023-04-19 16:13:39.405689 twinlab-1.0.2/twinlab/__init__.py
+-rw-r--r--   0        0        0     4804 2023-04-26 15:55:35.648121 twinlab-1.0.2/twinlab/client.py
+-rw-r--r--   0        0        0      505 2023-04-13 16:09:18.757239 twinlab-1.0.2/twinlab/plotting.py
+-rw-r--r--   0        0        0      532 2023-04-11 15:58:49.585681 twinlab-1.0.2/twinlab/settings.py
+-rw-r--r--   0        0        0     3955 2023-04-26 15:55:35.648860 twinlab-1.0.2/twinlab/utils.py
+-rw-r--r--   0        0        0     1624 1970-01-01 00:00:00.000000 twinlab-1.0.2/PKG-INFO
```

### Comparing `twinlab-1.0.1/README.md` & `twinlab-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `twinlab-1.0.1/pyproject.toml` & `twinlab-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "twinlab"
-version = "1.0.1"
+version = "1.0.2"
 description = "Client interface for twinLab"
 authors = ["Alexander Mead <alexander@digilab.co.uk>", "Freddy Wordingham <freddy@digilab.co.uk>"]
 repository = "https://github.com/digiLab-ai/twinLab-client"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.10"
```

### Comparing `twinlab-1.0.1/twinlab/__init__.py` & `twinlab-1.0.2/twinlab/__init__.py`

 * *Files identical despite different names*

### Comparing `twinlab-1.0.1/twinlab/client.py` & `twinlab-1.0.2/twinlab/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 
 ### Dataset functions ###
 
 
 def upload_dataset(filepath: str, server="cloud", verbose=False) -> None:
     """
     Upload big dataset
-    TODO: Replace upload_dataset with this?
     """
     lambda_url = utils.get_server_url(server) + "/generate_upload_url"
     headers = utils.STANDARD_HEADERS.copy()  #  TODO: Is .copy() necessary?
     headers["X-Dataset"] = filepath
     r = requests.get(lambda_url, headers=headers)
     utils.check_response(r)
     if verbose:
@@ -80,26 +79,28 @@
 
 ### Campaign functions ###
 
 
 def train_campaign(params: dict, campaign: str, server="cloud", verbose=False) -> None:
     """
     Train campaign
-    TODO: Set default train_test_split?
     """
-    url = utils.get_server_url(server) + "/train_campaign"
+    if server == "cloud":
+        url = utils.TRAIN_CAMPAIGN_CLOUD_URL
+    else:
+        url = utils.get_server_url(server) + "/train_campaign"
     headers = utils.STANDARD_HEADERS.copy()
     headers["X-Campaign"] = campaign
     r = requests.post(url, json=params, headers=headers)
     utils.check_response(r)
     if verbose:
         utils.print_response_message(r)
 
 
-def query_campaign(campaign: str, server="cloud", verbose=False) -> pd.DataFrame:
+def query_campaign(campaign: str, server="cloud", verbose=False) -> dict:
     """
     Query campaign
     """
     url = utils.get_server_url(server) + "/query_campaign"
     headers = utils.STANDARD_HEADERS.copy()
     headers["X-Campaign"] = campaign
     r = requests.get(url, headers=headers)
```

### Comparing `twinlab-1.0.1/twinlab/settings.py` & `twinlab-1.0.2/twinlab/settings.py`

 * *Files identical despite different names*

### Comparing `twinlab-1.0.1/twinlab/utils.py` & `twinlab-1.0.2/twinlab/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 from .settings import ENV
 
 STANDARD_HEADERS = {
     "X-Group": ENV.GROUP_NAME,
     "X-User": ENV.USER_NAME,
 }
 
+TRAIN_CAMPAIGN_CLOUD_URL = "https://4qpjawhm6wlrwe47kigbt2q7j40miizi.lambda-url.eu-west-2.on.aws/"
+
 ### Utility functions ###
 
 
 # def unwrap_payload(event: dict) -> dict:
 #     """
 #     Return payload and decode if it is base64 encoded
 #     TODO: Not used yet...
@@ -96,15 +98,15 @@
     """
     body = response.json()  # Get the body of the response as a dictionary
     data = body[name]  # Get the entry corresponding to the field name
     df = pd.read_json(data, orient="split")
     return df
 
 
-def extract_item_from_response(response: requests.Response, name: str) -> pd.DataFrame:
+def extract_item_from_response(response: requests.Response, name: str) -> any:
     """
     Extract CSV from response
     """
     body = response.json()  # Get the body of the response as a dictionary
     item = body[name]  # Get the entry corresponding to the field name
     return item
```

### Comparing `twinlab-1.0.1/PKG-INFO` & `twinlab-1.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twinlab
-Version: 1.0.1
+Version: 1.0.2
 Summary: Client interface for twinLab
 Home-page: https://github.com/digiLab-ai/twinLab-client
 Author: Alexander Mead
 Author-email: alexander@digilab.co.uk
 Requires-Python: >=3.9,<3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

