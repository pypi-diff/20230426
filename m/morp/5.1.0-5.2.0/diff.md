# Comparing `tmp/morp-5.1.0.tar.gz` & `tmp/morp-5.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morp-5.1.0.tar", last modified: Fri Mar 31 07:06:56 2023, max compression
+gzip compressed data, was "morp-5.2.0.tar", last modified: Tue Apr 25 19:02:12 2023, max compression
```

## Comparing `morp-5.1.0.tar` & `morp-5.2.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-03-31 07:06:56.094247 morp-5.1.0/
--rw-r--r--   0 jaymon     (501) staff       (20)     1079 2017-07-29 01:05:20.000000 morp-5.1.0/LICENSE.txt
--rw-r--r--   0 jaymon     (501) staff       (20)     3744 2023-03-31 07:06:56.094094 morp-5.1.0/PKG-INFO
--rw-r--r--   0 jaymon     (501) staff       (20)     3021 2023-03-03 20:29:34.000000 morp-5.1.0/README.md
-drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-03-31 07:06:56.092687 morp-5.1.0/morp/
--rw-r--r--   0 jaymon     (501) staff       (20)      347 2023-03-31 07:05:22.000000 morp-5.1.0/morp/__init__.py
--rw-r--r--   0 jaymon     (501) staff       (20)     6756 2023-02-05 20:04:47.000000 morp-5.1.0/morp/__main__.py
--rw-r--r--   0 jaymon     (501) staff       (20)       97 2023-02-07 07:17:53.000000 morp-5.1.0/morp/compat.py
--rw-r--r--   0 jaymon     (501) staff       (20)     4714 2023-03-31 06:52:48.000000 morp-5.1.0/morp/config.py
--rw-r--r--   0 jaymon     (501) staff       (20)     1022 2023-03-03 09:33:58.000000 morp-5.1.0/morp/exception.py
-drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-03-31 07:06:56.093903 morp-5.1.0/morp/interface/
--rw-r--r--   0 jaymon     (501) staff       (20)     2944 2023-02-07 07:11:11.000000 morp-5.1.0/morp/interface/__init__.py
--rw-r--r--   0 jaymon     (501) staff       (20)    11735 2023-03-03 09:01:56.000000 morp-5.1.0/morp/interface/base.py
--rw-r--r--   0 jaymon     (501) staff       (20)     4869 2023-03-03 20:33:14.000000 morp-5.1.0/morp/interface/dropfile.py
--rw-r--r--   0 jaymon     (501) staff       (20)    11113 2023-03-31 07:03:48.000000 morp-5.1.0/morp/interface/sqs.py
--rw-r--r--   0 jaymon     (501) staff       (20)    10350 2023-03-07 19:10:15.000000 morp-5.1.0/morp/message.py
-drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-03-31 07:06:56.093349 morp-5.1.0/morp.egg-info/
--rw-r--r--   0 jaymon     (501) staff       (20)     3744 2023-03-31 07:06:56.000000 morp-5.1.0/morp.egg-info/PKG-INFO
--rw-r--r--   0 jaymon     (501) staff       (20)      397 2023-03-31 07:06:56.000000 morp-5.1.0/morp.egg-info/SOURCES.txt
--rw-r--r--   0 jaymon     (501) staff       (20)        1 2023-03-31 07:06:56.000000 morp-5.1.0/morp.egg-info/dependency_links.txt
--rw-r--r--   0 jaymon     (501) staff       (20)       47 2023-03-31 07:06:56.000000 morp-5.1.0/morp.egg-info/entry_points.txt
--rw-r--r--   0 jaymon     (501) staff       (20)       38 2023-03-31 07:06:56.000000 morp-5.1.0/morp.egg-info/requires.txt
--rw-r--r--   0 jaymon     (501) staff       (20)        5 2023-03-31 07:06:56.000000 morp-5.1.0/morp.egg-info/top_level.txt
--rw-r--r--   0 jaymon     (501) staff       (20)       38 2023-03-31 07:06:56.094293 morp-5.1.0/setup.cfg
--rw-r--r--   0 jaymon     (501) staff       (20)     1815 2023-02-05 21:01:52.000000 morp-5.1.0/setup.py
+drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-04-25 19:02:12.666091 morp-5.2.0/
+-rw-r--r--   0 jaymon     (501) staff       (20)     1079 2017-07-29 01:05:20.000000 morp-5.2.0/LICENSE.txt
+-rw-r--r--   0 jaymon     (501) staff       (20)     3744 2023-04-25 19:02:12.665965 morp-5.2.0/PKG-INFO
+-rw-r--r--   0 jaymon     (501) staff       (20)     3021 2023-03-03 20:29:34.000000 morp-5.2.0/README.md
+drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-04-25 19:02:12.663828 morp-5.2.0/morp/
+-rw-r--r--   0 jaymon     (501) staff       (20)      347 2023-04-25 19:01:46.000000 morp-5.2.0/morp/__init__.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     6756 2023-02-05 20:04:47.000000 morp-5.2.0/morp/__main__.py
+-rw-r--r--   0 jaymon     (501) staff       (20)       97 2023-02-07 07:17:53.000000 morp-5.2.0/morp/compat.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     4714 2023-03-31 06:52:48.000000 morp-5.2.0/morp/config.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     1022 2023-03-03 09:33:58.000000 morp-5.2.0/morp/exception.py
+drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-04-25 19:02:12.665793 morp-5.2.0/morp/interface/
+-rw-r--r--   0 jaymon     (501) staff       (20)     2944 2023-02-07 07:11:11.000000 morp-5.2.0/morp/interface/__init__.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    11735 2023-03-03 09:01:56.000000 morp-5.2.0/morp/interface/base.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     4869 2023-03-03 20:33:14.000000 morp-5.2.0/morp/interface/dropfile.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    13537 2023-04-25 19:00:40.000000 morp-5.2.0/morp/interface/sqs.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    10350 2023-03-07 19:10:15.000000 morp-5.2.0/morp/message.py
+drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-04-25 19:02:12.664745 morp-5.2.0/morp.egg-info/
+-rw-r--r--   0 jaymon     (501) staff       (20)     3744 2023-04-25 19:02:12.000000 morp-5.2.0/morp.egg-info/PKG-INFO
+-rw-r--r--   0 jaymon     (501) staff       (20)      397 2023-04-25 19:02:12.000000 morp-5.2.0/morp.egg-info/SOURCES.txt
+-rw-r--r--   0 jaymon     (501) staff       (20)        1 2023-04-25 19:02:12.000000 morp-5.2.0/morp.egg-info/dependency_links.txt
+-rw-r--r--   0 jaymon     (501) staff       (20)       47 2023-04-25 19:02:12.000000 morp-5.2.0/morp.egg-info/entry_points.txt
+-rw-r--r--   0 jaymon     (501) staff       (20)       38 2023-04-25 19:02:12.000000 morp-5.2.0/morp.egg-info/requires.txt
+-rw-r--r--   0 jaymon     (501) staff       (20)        5 2023-04-25 19:02:12.000000 morp-5.2.0/morp.egg-info/top_level.txt
+-rw-r--r--   0 jaymon     (501) staff       (20)       38 2023-04-25 19:02:12.666135 morp-5.2.0/setup.cfg
+-rw-r--r--   0 jaymon     (501) staff       (20)     1815 2023-02-05 21:01:52.000000 morp-5.2.0/setup.py
```

### Comparing `morp-5.1.0/LICENSE.txt` & `morp-5.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `morp-5.1.0/PKG-INFO` & `morp-5.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morp
-Version: 5.1.0
+Version: 5.2.0
 Summary: Send and receive messages without thinking about it
 Home-page: http://github.com/Jaymon/morp
 Author: Jay Marcyes
 Author-email: jay@marcyes.com
 License: MIT
 Keywords: Amazon AWS SQS messages message-passing
 Classifier: Development Status :: 4 - Beta
```

### Comparing `morp-5.1.0/README.md` & `morp-5.2.0/README.md`

 * *Files identical despite different names*

### Comparing `morp-5.1.0/morp/__main__.py` & `morp-5.2.0/morp/__main__.py`

 * *Files identical despite different names*

### Comparing `morp-5.1.0/morp/config.py` & `morp-5.2.0/morp/config.py`

 * *Files identical despite different names*

### Comparing `morp-5.1.0/morp/exception.py` & `morp-5.2.0/morp/exception.py`

 * *Files identical despite different names*

### Comparing `morp-5.1.0/morp/interface/__init__.py` & `morp-5.2.0/morp/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `morp-5.1.0/morp/interface/base.py` & `morp-5.2.0/morp/interface/base.py`

 * *Files identical despite different names*

### Comparing `morp-5.1.0/morp/interface/dropfile.py` & `morp-5.2.0/morp/interface/dropfile.py`

 * *Files identical despite different names*

### Comparing `morp-5.1.0/morp/interface/sqs.py` & `morp-5.2.0/morp/interface/sqs.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 from contextlib import contextmanager
 import re
 import itertools
 import base64
 
 import boto3
 from botocore.exceptions import ClientError
+from botocore.credentials import RefreshableCredentials
+from botocore.session import get_session
 
 from ..compat import *
 from .base import Interface
 
 
 class Region(String):
     """Small wrapper that just makes sure the AWS region is valid"""
@@ -26,14 +28,102 @@
     @classmethod
     def names(cls):
         """Return all available regions for SQS"""
         session = boto3.Session()
         return session.get_available_regions("ec2")
 
 
+class RefreshableSession(boto3.Session):
+    """Boto Session wrapper which can use a refreshable session, this allows role
+    assumption to automatically refresh without the interface having to do anything
+
+    :Example:
+        session = RefreshableSession(connection_config)
+
+        # we now can cache this client object without worrying about expiring credentials
+        client = session.client("s3")
+
+    this is based off of this: https://stackoverflow.com/q/63724485
+    """
+    def __init__(self, connection_config):
+        """
+        :param connection_config: dict, this is the connection dict passed to the
+            interface, it should be just passed to this
+        """
+        self.connection_config = connection_config
+
+        # get refreshable credentials
+        refreshable_credentials = RefreshableCredentials.create_from_metadata(
+            metadata=self._get_credentials(),
+            refresh_using=self._get_credentials,
+            method="sts-assume-role",
+        )
+
+        # attach refreshable credentials current session
+        session = get_session()
+        session._credentials = refreshable_credentials
+        session.set_config_variable(
+            "region",
+            self.connection_config.options["region"]
+        )
+        super().__init__(botocore_session=session)
+
+    def _get_credentials(self):
+        """Get session credentials
+
+        This is a separate method because it will be used as a callback in the
+        refreshable credentials object that's created in __init__
+
+        :returns: dict
+        """
+        region = self.connection_config.options["region"]
+
+        session = boto3.Session(
+            region_name=region,
+            profile_name=self.connection_config.options.get("profile_name", None),
+        )
+
+        # if an sts arn is given, get credential by assuming given role
+        if arn := self.connection_config.options.get("arn", ""):
+            sts_client = session.client(
+                service_name="sts",
+                region_name=region,
+            )
+
+            response = sts_client.assume_role(
+                RoleArn=arn,
+                RoleSessionName=self.connection_config.options.get(
+                    "session_name",
+                    "morp"
+                ),
+                DurationSeconds=self.connection_config.options.get(
+                    "session_ttl",
+                    3600
+                ),
+            ).get("Credentials")
+
+            credentials = {
+                "access_key": response.get("AccessKeyId"),
+                "secret_key": response.get("SecretAccessKey"),
+                "token": response.get("SessionToken"),
+                "expiry_time": response.get("Expiration").isoformat(),
+            }
+
+        else:
+            session_credentials = session.get_credentials().__dict__
+            credentials = {
+                "access_key": session_credentials.get("access_key"),
+                "secret_key": session_credentials.get("secret_key"),
+                "token": session_credentials.get("token"),
+                "expiry_time": Datetime(seconds=self.session_ttl).isoformat(),
+            }
+
+        return credentials
+
+
 class SQS(Interface):
     """wraps amazon's SQS to make it work with our generic interface
 
     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html
     https://boto.readthedocs.org/en/latest/ref/sqs.html
     http://boto3.readthedocs.io/en/latest/guide/sqs.html
     http://michaelhallsmoore.com/blog/Python-Message-Queues-with-Amazon-Simple-Queue-Service
@@ -43,47 +133,24 @@
 
     def _connect(self, connection_config):
         self.connection_config.options['vtimeout_max'] = 43200 # 12 hours max (from Amazon)
 
         region = Region(self.connection_config.options.get('region', ''))
         self.connection_config.options['region'] = region
 
-        # https://boto3.amazonaws.com/v1/documentation/api/latest/guide/credentials.html
-        # https://github.com/boto/boto3/issues/2360#issuecomment-761526845
-        if arn := self.connection_config.options.get("arn", ""):
-            sts = boto3.client(
-                "sts",
-                aws_access_key_id=connection_config.username,
-                aws_secret_access_key=connection_config.password
-            )
+        session = RefreshableSession(self.connection_config)
 
-            role_info = sts.assume_role(
-                RoleArn=arn,
-                RoleSessionName="morp",
-            )
-            credentials = role_info["Credentials"]
+        boto_kwargs = {}
+        for opt in self.connection_config.options:
+            if opt.startswith("boto_"):
+                boto_kwargs[opt.replace("boto_", "")] = self.connection_config.options[opt]
+        if boto_kwargs:
+            self.log(f"SQS using boto kwargs: {boto_kwargs}")
 
-            self._connection = boto3.resource(
-                "sqs",
-                region_name=region,
-                aws_access_key_id=credentials["AccessKeyId"],
-                aws_secret_access_key=credentials["SecretAccessKey"],
-                aws_session_token=credentials["SessionToken"]
-            )
-
-            # we no longer need the sts client so clean it up
-            self._close_client(sts)
-
-        else:
-            self._connection = boto3.resource(
-                'sqs',
-                region_name=region,
-                aws_access_key_id=connection_config.username,
-                aws_secret_access_key=connection_config.password
-            )
+        self._connection = session.resource("sqs", **boto_kwargs)
 
         self.log("SQS connected to region {}", region)
 
     def get_connection(self):
         return self._connection
 
     def _close(self):
```

### Comparing `morp-5.1.0/morp/message.py` & `morp-5.2.0/morp/message.py`

 * *Files identical despite different names*

### Comparing `morp-5.1.0/morp.egg-info/PKG-INFO` & `morp-5.2.0/morp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morp
-Version: 5.1.0
+Version: 5.2.0
 Summary: Send and receive messages without thinking about it
 Home-page: http://github.com/Jaymon/morp
 Author: Jay Marcyes
 Author-email: jay@marcyes.com
 License: MIT
 Keywords: Amazon AWS SQS messages message-passing
 Classifier: Development Status :: 4 - Beta
```

### Comparing `morp-5.1.0/setup.py` & `morp-5.2.0/setup.py`

 * *Files identical despite different names*

