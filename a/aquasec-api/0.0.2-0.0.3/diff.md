# Comparing `tmp/aquasec-api-0.0.2.tar.gz` & `tmp/aquasec-api-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aquasec-api-0.0.2.tar", last modified: Fri Mar 31 18:54:15 2023, max compression
+gzip compressed data, was "aquasec-api-0.0.3.tar", last modified: Tue Apr 25 18:40:28 2023, max compression
```

## Comparing `aquasec-api-0.0.2.tar` & `aquasec-api-0.0.3.tar`

### file list

```diff
@@ -1,28 +1,34 @@
-drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-03-31 18:54:15.620047 aquasec-api-0.0.2/
--rw-rw-r--   0 adamt      (501) staff       (20)    35129 2023-03-31 18:51:16.000000 aquasec-api-0.0.2/LICENSE
--rw-rw-r--   0 adamt      (501) staff       (20)       78 2023-03-31 18:51:16.000000 aquasec-api-0.0.2/MANIFEST.in
--rw-r--r--   0 adamt      (501) staff       (20)     9479 2023-03-31 18:54:15.619413 aquasec-api-0.0.2/PKG-INFO
--rw-rw-r--   0 adamt      (501) staff       (20)     9097 2023-03-31 18:51:16.000000 aquasec-api-0.0.2/README.md
-drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-03-31 18:54:15.615537 aquasec-api-0.0.2/aquasec/
--rw-rw-r--   0 adamt      (501) staff       (20)     4281 2023-03-31 18:51:16.000000 aquasec-api-0.0.2/aquasec/__init__.py
--rw-rw-r--   0 adamt      (501) staff       (20)       37 2023-03-31 18:51:16.000000 aquasec-api-0.0.2/aquasec/_version.py
--rw-rw-r--   0 adamt      (501) staff       (20)     3684 2023-03-31 18:51:16.000000 aquasec-api-0.0.2/aquasec/api.py
--rw-rw-r--   0 adamt      (501) staff       (20)     6621 2023-03-31 18:51:16.000000 aquasec-api-0.0.2/aquasec/auth.py
--rw-rw-r--   0 adamt      (501) staff       (20)     1202 2023-03-31 18:51:16.000000 aquasec-api-0.0.2/aquasec/configs.py
--rw-rw-r--   0 adamt      (501) staff       (20)      447 2023-03-31 18:51:16.000000 aquasec-api-0.0.2/aquasec/exceptions.py
--rw-rw-r--   0 adamt      (501) staff       (20)     7452 2023-03-31 18:51:16.000000 aquasec-api-0.0.2/aquasec/get.py
--rw-rw-r--   0 adamt      (501) staff       (20)     3708 2023-03-31 18:51:16.000000 aquasec-api-0.0.2/aquasec/logging.py
--rw-rw-r--   0 adamt      (501) staff       (20)      475 2023-03-31 18:51:16.000000 aquasec-api-0.0.2/aquasec/post.py
--rw-rw-r--   0 adamt      (501) staff       (20)     6325 2023-03-31 18:51:16.000000 aquasec-api-0.0.2/aquasec/requestapi.py
--rw-rw-r--   0 adamt      (501) staff       (20)      103 2023-03-31 18:51:16.000000 aquasec-api-0.0.2/aquasec/statics.py
--rw-rw-r--   0 adamt      (501) staff       (20)     1003 2023-03-31 18:51:16.000000 aquasec-api-0.0.2/aquasec/utilities.py
-drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-03-31 18:54:15.618682 aquasec-api-0.0.2/aquasec_api.egg-info/
--rw-r--r--   0 adamt      (501) staff       (20)     9479 2023-03-31 18:54:15.000000 aquasec-api-0.0.2/aquasec_api.egg-info/PKG-INFO
--rw-r--r--   0 adamt      (501) staff       (20)      465 2023-03-31 18:54:15.000000 aquasec-api-0.0.2/aquasec_api.egg-info/SOURCES.txt
--rw-r--r--   0 adamt      (501) staff       (20)        1 2023-03-31 18:54:15.000000 aquasec-api-0.0.2/aquasec_api.egg-info/dependency_links.txt
--rw-r--r--   0 adamt      (501) staff       (20)       52 2023-03-31 18:54:15.000000 aquasec-api-0.0.2/aquasec_api.egg-info/requires.txt
--rw-r--r--   0 adamt      (501) staff       (20)        8 2023-03-31 18:54:15.000000 aquasec-api-0.0.2/aquasec_api.egg-info/top_level.txt
--rw-rw-r--   0 adamt      (501) staff       (20)       52 2023-03-31 18:51:16.000000 aquasec-api-0.0.2/requirements.txt
--rw-rw-r--   0 adamt      (501) staff       (20)      125 2023-03-31 18:51:16.000000 aquasec-api-0.0.2/sample.yaml
--rw-r--r--   0 adamt      (501) staff       (20)       38 2023-03-31 18:54:15.620232 aquasec-api-0.0.2/setup.cfg
--rw-rw-r--   0 adamt      (501) staff       (20)     1122 2023-03-31 18:51:16.000000 aquasec-api-0.0.2/setup.py
+drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-04-25 18:40:28.270132 aquasec-api-0.0.3/
+-rw-rw-r--   0 adamt      (501) staff       (20)    35129 2023-04-25 18:38:14.000000 aquasec-api-0.0.3/LICENSE
+-rw-rw-r--   0 adamt      (501) staff       (20)       78 2023-04-25 18:38:14.000000 aquasec-api-0.0.3/MANIFEST.in
+-rw-r--r--   0 adamt      (501) staff       (20)    10017 2023-04-25 18:40:28.269550 aquasec-api-0.0.3/PKG-INFO
+-rw-rw-r--   0 adamt      (501) staff       (20)     9635 2023-04-25 18:38:14.000000 aquasec-api-0.0.3/README.md
+drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-04-25 18:40:28.266155 aquasec-api-0.0.3/aquasec/
+-rw-rw-r--   0 adamt      (501) staff       (20)     4281 2023-04-25 18:38:14.000000 aquasec-api-0.0.3/aquasec/__init__.py
+-rw-rw-r--   0 adamt      (501) staff       (20)       37 2023-04-25 18:38:14.000000 aquasec-api-0.0.3/aquasec/_version.py
+-rw-rw-r--   0 adamt      (501) staff       (20)     4157 2023-04-25 18:38:14.000000 aquasec-api-0.0.3/aquasec/api.py
+-rw-rw-r--   0 adamt      (501) staff       (20)     6621 2023-04-25 18:38:14.000000 aquasec-api-0.0.3/aquasec/auth.py
+-rw-rw-r--   0 adamt      (501) staff       (20)     1202 2023-04-25 18:38:14.000000 aquasec-api-0.0.3/aquasec/configs.py
+-rw-rw-r--   0 adamt      (501) staff       (20)     1694 2023-04-25 18:38:14.000000 aquasec-api-0.0.3/aquasec/delete.py
+-rw-rw-r--   0 adamt      (501) staff       (20)      447 2023-04-25 18:38:14.000000 aquasec-api-0.0.3/aquasec/exceptions.py
+-rw-rw-r--   0 adamt      (501) staff       (20)     7431 2023-04-25 18:38:14.000000 aquasec-api-0.0.3/aquasec/get.py
+-rw-rw-r--   0 adamt      (501) staff       (20)     3708 2023-04-25 18:38:14.000000 aquasec-api-0.0.3/aquasec/logging.py
+drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-04-25 18:40:28.266807 aquasec-api-0.0.3/aquasec/orchestration/
+-rw-rw-r--   0 adamt      (501) staff       (20)        0 2023-04-25 18:38:14.000000 aquasec-api-0.0.3/aquasec/orchestration/__init__.py
+-rw-rw-r--   0 adamt      (501) staff       (20)     3723 2023-04-25 18:38:14.000000 aquasec-api-0.0.3/aquasec/orchestration/bench_report.py
+-rw-rw-r--   0 adamt      (501) staff       (20)     2128 2023-04-25 18:38:14.000000 aquasec-api-0.0.3/aquasec/post.py
+-rw-rw-r--   0 adamt      (501) staff       (20)     1163 2023-04-25 18:38:14.000000 aquasec-api-0.0.3/aquasec/put.py
+-rw-rw-r--   0 adamt      (501) staff       (20)     7764 2023-04-25 18:38:14.000000 aquasec-api-0.0.3/aquasec/requestapi.py
+-rw-rw-r--   0 adamt      (501) staff       (20)      200 2023-04-25 18:38:14.000000 aquasec-api-0.0.3/aquasec/statics.py
+-rw-rw-r--   0 adamt      (501) staff       (20)     1713 2023-04-25 18:38:14.000000 aquasec-api-0.0.3/aquasec/structures.py
+-rw-rw-r--   0 adamt      (501) staff       (20)     2400 2023-04-25 18:38:14.000000 aquasec-api-0.0.3/aquasec/utilities.py
+drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-04-25 18:40:28.268845 aquasec-api-0.0.3/aquasec_api.egg-info/
+-rw-r--r--   0 adamt      (501) staff       (20)    10017 2023-04-25 18:40:28.000000 aquasec-api-0.0.3/aquasec_api.egg-info/PKG-INFO
+-rw-r--r--   0 adamt      (501) staff       (20)      592 2023-04-25 18:40:28.000000 aquasec-api-0.0.3/aquasec_api.egg-info/SOURCES.txt
+-rw-r--r--   0 adamt      (501) staff       (20)        1 2023-04-25 18:40:28.000000 aquasec-api-0.0.3/aquasec_api.egg-info/dependency_links.txt
+-rw-r--r--   0 adamt      (501) staff       (20)       84 2023-04-25 18:40:28.000000 aquasec-api-0.0.3/aquasec_api.egg-info/requires.txt
+-rw-r--r--   0 adamt      (501) staff       (20)        8 2023-04-25 18:40:28.000000 aquasec-api-0.0.3/aquasec_api.egg-info/top_level.txt
+-rw-rw-r--   0 adamt      (501) staff       (20)       84 2023-04-25 18:38:14.000000 aquasec-api-0.0.3/requirements.txt
+-rw-rw-r--   0 adamt      (501) staff       (20)      125 2023-04-25 18:38:14.000000 aquasec-api-0.0.3/sample.yaml
+-rw-r--r--   0 adamt      (501) staff       (20)       38 2023-04-25 18:40:28.270296 aquasec-api-0.0.3/setup.cfg
+-rw-rw-r--   0 adamt      (501) staff       (20)     1122 2023-04-25 18:38:14.000000 aquasec-api-0.0.3/setup.py
```

### Comparing `aquasec-api-0.0.2/LICENSE` & `aquasec-api-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aquasec-api-0.0.2/PKG-INFO` & `aquasec-api-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aquasec-api
-Version: 0.0.2
+Version: 0.0.3
 Summary: Aqua Security SDK to pull data from Aquasec Tenant and CSPM for auditing
 Home-page: https://github.com/atav928/aquasec-api
 Author: atav928
 Author-email: dev@tavnets.com
 Maintainer-email: dev@tavnets.com
 Keywords: aquasec,aqua security,workload protection
 Description-Content-Type: text/markdown
@@ -208,14 +208,23 @@
     >>> disa_stig_report = api.get.bench_reports(report_type='disa_stig')
     # Full CIS Benchmark Report on all Hosts
     >>> full_cis_report = api.get.bench_reports(report_type='all')
     ```
 
 ## Release Info
 
+### v0.0.3
+
+* Added ability to POST
+* Adding PUT
+* Additional Datastructures
+* Additional Delete Functionality
+* Introducing Orchestration on Actions
+* Bug in response code when we POST and possibly PUT an object; no json is returned just a 204. This breaks the standard return expectation. Raised issue with AquaSec. Till than buillt a way to handle it safely and introducted a message response to those responses.
+
 ### v0.0.2
 
 * added retrieve_full_list() which allows get to retrieve all items.
 * if _"get_all"_ is specified in api.get.workload_protection() the variable will retrieve all possible values.
 * updates to README.md, fixed a few typos.
 * added ability to retrieve CIS bench reports directly without the need to run mulitple calls.
 * Fixed issue with _"get_all"_ where it would go into an infinant loop since the count return did not always match the results.
@@ -244,9 +253,10 @@
 | __0.0.1__ | __rc4__ | issues with dataclasses and requirements |
 | __0.0.1__ | __rc8__ | final release that solves how the auth works for CSPM and Workload Protection |
 | __0.0.2__ | __a1__ | Updated readme testing some additional modeling and possible integration scripts |
 | __0.0.2__ | __a2__ | Added ability to retrieve all functions leveraging paging |
 | __0.0.2__ | __a3__ | Added CIS benchmark reports, Fix bug with infinate get_all |
 | __0.0.2__ | __rc1__ | Bug with providing direct api information into api function with WorkloadAuth |
 | __0.0.2__ | __final__ | completed orchestration of bench report and standard get workload checks |
+| __0.0.3__ | __a1__ | Intro to POST, PUT, DELETE and adding some datastructures for creating and manipluating AquaSec |
 
 __NOTE:__ Use at your own risk!!!! API as is and building on it.
```

### Comparing `aquasec-api-0.0.2/README.md` & `aquasec-api-0.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -196,14 +196,23 @@
     >>> disa_stig_report = api.get.bench_reports(report_type='disa_stig')
     # Full CIS Benchmark Report on all Hosts
     >>> full_cis_report = api.get.bench_reports(report_type='all')
     ```
 
 ## Release Info
 
+### v0.0.3
+
+* Added ability to POST
+* Adding PUT
+* Additional Datastructures
+* Additional Delete Functionality
+* Introducing Orchestration on Actions
+* Bug in response code when we POST and possibly PUT an object; no json is returned just a 204. This breaks the standard return expectation. Raised issue with AquaSec. Till than buillt a way to handle it safely and introducted a message response to those responses.
+
 ### v0.0.2
 
 * added retrieve_full_list() which allows get to retrieve all items.
 * if _"get_all"_ is specified in api.get.workload_protection() the variable will retrieve all possible values.
 * updates to README.md, fixed a few typos.
 * added ability to retrieve CIS bench reports directly without the need to run mulitple calls.
 * Fixed issue with _"get_all"_ where it would go into an infinant loop since the count return did not always match the results.
@@ -232,9 +241,10 @@
 | __0.0.1__ | __rc4__ | issues with dataclasses and requirements |
 | __0.0.1__ | __rc8__ | final release that solves how the auth works for CSPM and Workload Protection |
 | __0.0.2__ | __a1__ | Updated readme testing some additional modeling and possible integration scripts |
 | __0.0.2__ | __a2__ | Added ability to retrieve all functions leveraging paging |
 | __0.0.2__ | __a3__ | Added CIS benchmark reports, Fix bug with infinate get_all |
 | __0.0.2__ | __rc1__ | Bug with providing direct api information into api function with WorkloadAuth |
 | __0.0.2__ | __final__ | completed orchestration of bench report and standard get workload checks |
+| __0.0.3__ | __a1__ | Intro to POST, PUT, DELETE and adding some datastructures for creating and manipluating AquaSec |
 
 __NOTE:__ Use at your own risk!!!! API as is and building on it.
```

### Comparing `aquasec-api-0.0.2/aquasec/__init__.py` & `aquasec-api-0.0.3/aquasec/__init__.py`

 * *Files identical despite different names*

### Comparing `aquasec-api-0.0.2/aquasec/api.py` & `aquasec-api-0.0.3/aquasec/api.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 # pylint: disable=missing-class-docstring,too-few-public-methods
 """API"""
 
 from aquasec import logger, config, return_workload_auth
 from aquasec.get import Get
 from aquasec.post import Post
+from aquasec.delete import Delete
+from aquasec.put import Put
 from aquasec.utilities import reformat_exception
 from aquasec.exceptions import (AquaSecPermission, AquaSecAPIError)
 
 logger.addLogger(__name__)
 aqua_logger = logger.getLogger(__name__)
 if not config.SET_LOG:
     aqua_logger.disabled = True
 
 
 class API:
     """_summary_
     """
     cloudsploit_url: str = "https://api.cloudsploit.com/{}/{}"
     workload_url: str = "{}/api/{}/{}"
-    api_version: str = "" # set on initialization
+    api_version: str = ""  # set on initialization
     # Endpoints for CSPM going away from this
     # TODO: Remove the endpoint capability and just use the direct csmp get()
     endpoint_alerts: str = "alerts"
     endpoint_apikeys: str = "apikeys"
     endpoint_auditlogs: str = "auditlogs"
     # Testing workload and endpoint types.. this should eventually go away
     # TODO: figure out how to get all the actual endpoints listed some how and their params
@@ -52,14 +54,16 @@
             'api_version') else config.API_VERSION
         self.supported_urls: dict = self.list_supported_urls()
 
         # Bind API method classes to this object
         subclasses = self._subclass_container()
         self.get = subclasses['get']()
         self.post = subclasses['post']()
+        self.put = subclasses['put']()
+        self.delete = subclasses['delete']()
 
     def list_supported_urls(self) -> dict:
         """Create a dictionary of supported endpoint URLs
 
         Returns:
             dict: _description_
         """
@@ -86,8 +90,18 @@
                 self._parent_class = _parent_class
         return_object['get'] = GetWrapper
 
         class PostWrapper(Post):
             def __init__(self):
                 self._parent_class = _parent_class
         return_object['post'] = PostWrapper
+
+        class PutWrapper(Put):
+            def __inti__(self):
+                self._parent_class = _parent_class
+        return_object['put'] = PutWrapper
+
+        class DeleteWrapper(Delete):
+            def __init__(self):
+                self._parent_class = _parent_class
+        return_object['delete'] = DeleteWrapper
         return return_object
```

### Comparing `aquasec-api-0.0.2/aquasec/auth.py` & `aquasec-api-0.0.3/aquasec/auth.py`

 * *Files identical despite different names*

### Comparing `aquasec-api-0.0.2/aquasec/configs.py` & `aquasec-api-0.0.3/aquasec/configs.py`

 * *Files identical despite different names*

### Comparing `aquasec-api-0.0.2/aquasec/get.py` & `aquasec-api-0.0.3/aquasec/get.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+# pylint: disable=line-too-long
 """Get Method"""
 
 from aquasec import config, logger
 
 from aquasec.auth import (refresh_workload_token, WorkloadAuth)
 from aquasec.statics import BENCH_REPORTS
 from aquasec.requestapi import (aqua_cloudsploit_request, aqua_workload_request, retrieve_full_list)
-from aquasec.utilities import reformat_exception
+from aquasec.utilities import (reformat_exception, UrlUtils)
 from aquasec.exceptions import (AquaSecWrongParam, AquaSecAPIError)
 
 logger.addLogger(__name__)
 aquasec_logger = logger.getLogger(__name__)
 if not config.SET_LOG:
     aquasec_logger.disabled = True
 
@@ -58,29 +59,29 @@
         try:
             api_version: str = kwargs.pop(
                 'api_version', self._parent_class.workload_auth.api_version)  # type:ignore
             get_all: bool = kwargs.pop('get_all', False)
         except KeyError as err:
             error = reformat_exception(err)
             aquasec_logger.error("AquaSecMissingParam: %s", error)
-        url = Get._create_workload_url(self._parent_class.workload_auth,  # type: ignore
-                                       self._parent_class.workload_url,  # type:ignore
-                                       url_path=url_path,
-                                       api_version=api_version)  # type: ignore
+        url = UrlUtils.create_workload_url(self._parent_class.workload_auth,  # type: ignore
+                                           self._parent_class.workload_url,  # type:ignore
+                                           url_path=url_path,
+                                           api_version=api_version)  # type: ignore
         aquasec_logger.info("Created Workload URL=%s", url)
-        if not get_all:
-            response = aqua_workload_request(self._parent_class.workload_auth,  # type: ignore
-                                             url=url,
-                                             method=self.method,
-                                             **kwargs)
-        else:
-            response = retrieve_full_list(self._parent_class.workload_auth,  # type: ignore
-                                          url=url,
-                                          method=self.method,
-                                          **kwargs)
+        # retrieve response either for a single page, or entire result through a looping function
+        response = aqua_workload_request(self._parent_class.workload_auth,  # type: ignore
+                                         url=url,
+                                         method=self.method,
+                                         # type: ignore
+                                         **kwargs) if not get_all else retrieve_full_list(self._parent_class.workload_auth,
+                                                                                          url=url,
+                                                                                          method=self.method,
+                                                                                          **kwargs)
+        # Log out entry
         aquasec_logger.info("Retrieved Inforomation from Workload Protection")
         return response
 
     def bench_reports(self, report_type: str, **kwargs) -> dict:
         """_summary_
 
         Args:
@@ -165,15 +166,7 @@
         Returns:
             str: _description_
         """
         api_version: str = kwargs.pop(
             'api_version', self._parent_class.api_version)  # type: ignore # type :ignore
         url = self._parent_class.cloudsploit_url.format(api_version, url_path)  # type: ignore
         return url
-
-    @staticmethod
-    @refresh_workload_token
-    def _create_workload_url(
-            workload_auth: WorkloadAuth, workload_url: str, url_path: str, api_version: str) -> str:
-        url = workload_url.format(workload_auth.aqua_url, api_version, url_path)
-        aquasec_logger.debug("Created url %s", url)
-        return url
```

### Comparing `aquasec-api-0.0.2/aquasec/logging.py` & `aquasec-api-0.0.3/aquasec/logging.py`

 * *Files identical despite different names*

### Comparing `aquasec-api-0.0.2/aquasec/requestapi.py` & `aquasec-api-0.0.3/aquasec/requestapi.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Request API"""
+import json
 from typing import Any, Dict
 import requests
 from requests import Response
 
 from aquasec import config, logger, create_cspm_headers
 from aquasec.auth import WorkloadAuth, refresh_workload_token
 from aquasec.exceptions import (AquaSecAPIError, AquaSecMissingParam, AquaSecPermission)
@@ -37,33 +38,40 @@
     """
     try:
         method: str = kwargs.pop('method')
         url: str = kwargs.pop('url')
         timeout: int = kwargs.pop('timeout', 60)
         verify = kwargs.pop('verify', config.CERT)
         params: dict = kwargs.pop('params', {})
+        data: dict = kwargs.pop('data', None)
     except KeyError as err:
         error = reformat_exception(err)
         aquasec_logger.error("AquaSecMissingParam: %s", error)
         raise AquaSecMissingParam(error)  # pylint: disable=raise-missing-from
+    if data:
+        data = json.dumps(data)
     response = requests.request(method=method,
                                 url=url,
                                 headers=workload_auth.headers,
-                                # data=data,
+                                data=data,
                                 params=params,
                                 verify=verify,
                                 timeout=timeout)
     aquasec_logger.debug("Response Code=%s|Full Response=%s",
                          str(response.status_code), response.text.rstrip())
     api_raise_error(response=response)
-    return response.json()
+    if response.status_code == 204:
+        json_response = {"message": "Data Created", "code": response.status_code}
+    else:
+        json_response = response.json()
+    return json_response
 
 
 def retrieve_full_list(workload_auth: WorkloadAuth, **kwargs):
-    """_summary_
+    """Retrieves fulll list of requirements based on multiple calls
 
     Args:
         workload_auth (WorkloadAuth): _description_
         url (str): url to call
         method (str): Requests Type
 
     Raises:
@@ -96,15 +104,16 @@
             response = aqua_workload_request(workload_auth=workload_auth,
                                              url=url,
                                              method=method,
                                              params=params,
                                              **kwargs)
             if response['result']:
                 result = result + response['result']
-                aquasec_logger.debug("result_length=%s|result_count=%s", str(len(result)), str(response["count"]))
+                aquasec_logger.debug("result_length=%s|result_count=%s",
+                                     str(len(result)), str(response["count"]))
             if not response['result']:
                 break
             params = {**params, **{"page": params["page"] + 1}}
             iterations += 1
         except Exception as err:  # pylint: disable=broad-exception-caught
             error = reformat_exception(err)
             aquasec_logger.error("Unable to get %s data error=%s", url, error)
@@ -156,7 +165,28 @@
         message = response.json().get("message", "Permission Denied")
         aquasec_logger.error("AquaSecPermission: %s", message)
         raise AquaSecPermission(message)
     if not (response.status_code >= 200 and response.status_code < 299):
         aquasec_logger.error("Status Code: %s| Error: %s", str(
             response.status_code), response.json())
         raise AquaSecAPIError(response.json())
+
+
+Traceback (most recent call last):
+  File "/.env/lib/python3.8/site-packages/requests/models.py", line 971, in json
+    return complexjson.loads(self.text, **kwargs)
+  File "/Users/adamt/.pyenv/versions/3.8.15/lib/python3.8/json/__init__.py", line 357, in loads
+    return _default_decoder.decode(s)
+  File "/Users/adamt/.pyenv/versions/3.8.15/lib/python3.8/json/decoder.py", line 337, in decode
+    obj, end = self.raw_decode(s, idx=_w(s, 0).end())
+  File "/Users/adamt/.pyenv/versions/3.8.15/lib/python3.8/json/decoder.py", line 355, in raw_decode
+    raise JSONDecodeError("Expecting value", s, err.value) from None
+json.decoder.JSONDecodeError: Expecting value: line 1 column 1 (char 0)
+
+During handling of the above exception, another exception occurred:
+
+Traceback (most recent call last):
+  File "test_call.py", line 41, in <module>
+    print(response.json())
+  File "/.env/lib/python3.8/site-packages/requests/models.py", line 975, in json
+    raise RequestsJSONDecodeError(e.msg, e.doc, e.pos)
+requests.exceptions.JSONDecodeError: Expecting value: line 1 column 1 (char 0)
```

### Comparing `aquasec-api-0.0.2/aquasec_api.egg-info/PKG-INFO` & `aquasec-api-0.0.3/aquasec_api.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aquasec-api
-Version: 0.0.2
+Version: 0.0.3
 Summary: Aqua Security SDK to pull data from Aquasec Tenant and CSPM for auditing
 Home-page: https://github.com/atav928/aquasec-api
 Author: atav928
 Author-email: dev@tavnets.com
 Maintainer-email: dev@tavnets.com
 Keywords: aquasec,aqua security,workload protection
 Description-Content-Type: text/markdown
@@ -208,14 +208,23 @@
     >>> disa_stig_report = api.get.bench_reports(report_type='disa_stig')
     # Full CIS Benchmark Report on all Hosts
     >>> full_cis_report = api.get.bench_reports(report_type='all')
     ```
 
 ## Release Info
 
+### v0.0.3
+
+* Added ability to POST
+* Adding PUT
+* Additional Datastructures
+* Additional Delete Functionality
+* Introducing Orchestration on Actions
+* Bug in response code when we POST and possibly PUT an object; no json is returned just a 204. This breaks the standard return expectation. Raised issue with AquaSec. Till than buillt a way to handle it safely and introducted a message response to those responses.
+
 ### v0.0.2
 
 * added retrieve_full_list() which allows get to retrieve all items.
 * if _"get_all"_ is specified in api.get.workload_protection() the variable will retrieve all possible values.
 * updates to README.md, fixed a few typos.
 * added ability to retrieve CIS bench reports directly without the need to run mulitple calls.
 * Fixed issue with _"get_all"_ where it would go into an infinant loop since the count return did not always match the results.
@@ -244,9 +253,10 @@
 | __0.0.1__ | __rc4__ | issues with dataclasses and requirements |
 | __0.0.1__ | __rc8__ | final release that solves how the auth works for CSPM and Workload Protection |
 | __0.0.2__ | __a1__ | Updated readme testing some additional modeling and possible integration scripts |
 | __0.0.2__ | __a2__ | Added ability to retrieve all functions leveraging paging |
 | __0.0.2__ | __a3__ | Added CIS benchmark reports, Fix bug with infinate get_all |
 | __0.0.2__ | __rc1__ | Bug with providing direct api information into api function with WorkloadAuth |
 | __0.0.2__ | __final__ | completed orchestration of bench report and standard get workload checks |
+| __0.0.3__ | __a1__ | Intro to POST, PUT, DELETE and adding some datastructures for creating and manipluating AquaSec |
 
 __NOTE:__ Use at your own risk!!!! API as is and building on it.
```

### Comparing `aquasec-api-0.0.2/setup.py` & `aquasec-api-0.0.3/setup.py`

 * *Files identical despite different names*

