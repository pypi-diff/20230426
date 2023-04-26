# Comparing `tmp/PinPointClient-0.0.8.tar.gz` & `tmp/PinPointClient-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PinPointClient-0.0.8.tar", last modified: Thu Feb  9 21:52:53 2023, max compression
+gzip compressed data, was "PinPointClient-0.0.9.tar", last modified: Thu Feb  9 23:12:49 2023, max compression
```

## Comparing `PinPointClient-0.0.8.tar` & `PinPointClient-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-02-09 21:52:53.771244 PinPointClient-0.0.8/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1071 2022-10-16 19:39:29.000000 PinPointClient-0.0.8/LICENSE
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     2273 2023-02-09 21:52:53.771117 PinPointClient-0.0.8/PKG-INFO
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-02-09 21:52:53.769718 PinPointClient-0.0.8/PinPointClient.egg-info/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     2273 2023-02-09 21:52:53.000000 PinPointClient-0.0.8/PinPointClient.egg-info/PKG-INFO
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      307 2023-02-09 21:52:53.000000 PinPointClient-0.0.8/PinPointClient.egg-info/SOURCES.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        1 2023-02-09 21:52:53.000000 PinPointClient-0.0.8/PinPointClient.egg-info/dependency_links.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        6 2023-02-09 21:52:53.000000 PinPointClient-0.0.8/PinPointClient.egg-info/requires.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        9 2023-02-09 21:52:53.000000 PinPointClient-0.0.8/PinPointClient.egg-info/top_level.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1725 2022-11-20 12:42:35.000000 PinPointClient-0.0.8/README.md
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-02-09 21:52:53.770799 PinPointClient-0.0.8/pinpoint/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      140 2023-02-09 21:45:19.000000 PinPointClient-0.0.8/pinpoint/__init__.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      703 2023-02-09 21:48:43.000000 PinPointClient-0.0.8/pinpoint/exception.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     3502 2023-02-09 21:49:24.000000 PinPointClient-0.0.8/pinpoint/mail_service.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     3327 2022-11-20 12:56:24.000000 PinPointClient-0.0.8/pinpoint/sms_service.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)       38 2023-02-09 21:52:53.771290 PinPointClient-0.0.8/setup.cfg
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      866 2023-02-09 21:52:48.000000 PinPointClient-0.0.8/setup.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-02-09 23:12:49.625860 PinPointClient-0.0.9/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1071 2022-10-16 19:39:29.000000 PinPointClient-0.0.9/LICENSE
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     2387 2023-02-09 23:12:49.625717 PinPointClient-0.0.9/PKG-INFO
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-02-09 23:12:49.624073 PinPointClient-0.0.9/PinPointClient.egg-info/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     2387 2023-02-09 23:12:49.000000 PinPointClient-0.0.9/PinPointClient.egg-info/PKG-INFO
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      307 2023-02-09 23:12:49.000000 PinPointClient-0.0.9/PinPointClient.egg-info/SOURCES.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        1 2023-02-09 23:12:49.000000 PinPointClient-0.0.9/PinPointClient.egg-info/dependency_links.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        6 2023-02-09 23:12:49.000000 PinPointClient-0.0.9/PinPointClient.egg-info/requires.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        9 2023-02-09 23:12:49.000000 PinPointClient-0.0.9/PinPointClient.egg-info/top_level.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1839 2023-02-09 21:53:49.000000 PinPointClient-0.0.9/README.md
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-02-09 23:12:49.625273 PinPointClient-0.0.9/pinpoint/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      140 2023-02-09 23:08:51.000000 PinPointClient-0.0.9/pinpoint/__init__.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      703 2023-02-09 21:48:43.000000 PinPointClient-0.0.9/pinpoint/exception.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     2325 2023-02-09 23:12:33.000000 PinPointClient-0.0.9/pinpoint/mail_service.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     3327 2022-11-20 12:56:24.000000 PinPointClient-0.0.9/pinpoint/sms_service.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)       38 2023-02-09 23:12:49.625908 PinPointClient-0.0.9/setup.cfg
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      866 2023-02-09 23:08:46.000000 PinPointClient-0.0.9/setup.py
```

### Comparing `PinPointClient-0.0.8/LICENSE` & `PinPointClient-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `PinPointClient-0.0.8/PKG-INFO` & `PinPointClient-0.0.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: PinPointClient
-Version: 0.0.8
+Version: 0.0.9
 Summary: PinPoint Aws Pinpoint SMS/Mail Client Python package
 Home-page: https://github.com/blueromans/PinPointClient.git
 Author: Yaşar Özyurt
 Author-email: blueromans@gmail.com
 Project-URL: Bug Tracker, https://github.com/blueromans/PinPointClient/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+[![PyPI version](https://img.shields.io/pypi/v/PinPointClient.svg)](https://pypi.python.org/pypi/PinPointClient)
+
 # PinPointClient Python PyPackage
 
 PinPoint is Aws Sms Service. PinPointClient is a Python library to access services quickly.
 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install foobar.
```

### Comparing `PinPointClient-0.0.8/PinPointClient.egg-info/PKG-INFO` & `PinPointClient-0.0.9/PinPointClient.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: PinPointClient
-Version: 0.0.8
+Version: 0.0.9
 Summary: PinPoint Aws Pinpoint SMS/Mail Client Python package
 Home-page: https://github.com/blueromans/PinPointClient.git
 Author: Yaşar Özyurt
 Author-email: blueromans@gmail.com
 Project-URL: Bug Tracker, https://github.com/blueromans/PinPointClient/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+[![PyPI version](https://img.shields.io/pypi/v/PinPointClient.svg)](https://pypi.python.org/pypi/PinPointClient)
+
 # PinPointClient Python PyPackage
 
 PinPoint is Aws Sms Service. PinPointClient is a Python library to access services quickly.
 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install foobar.
```

### Comparing `PinPointClient-0.0.8/README.md` & `PinPointClient-0.0.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+[![PyPI version](https://img.shields.io/pypi/v/PinPointClient.svg)](https://pypi.python.org/pypi/PinPointClient)
+
 # PinPointClient Python PyPackage
 
 PinPoint is Aws Sms Service. PinPointClient is a Python library to access services quickly.
 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install foobar.
```

### Comparing `PinPointClient-0.0.8/pinpoint/exception.py` & `PinPointClient-0.0.9/pinpoint/exception.py`

 * *Files identical despite different names*

### Comparing `PinPointClient-0.0.8/pinpoint/mail_service.py` & `PinPointClient-0.0.9/pinpoint/sms_service.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,80 +1,66 @@
 import os
 
 import boto3
 from botocore.exceptions import ClientError
 from pinpoint.exception import PinPointException, ErrorCodes
 
 
-class EMailService:
+class GsmService:
     region = "eu-central-1"
-    channel_type = "EMAIL"
+    message_type = "TRANSACTIONAL"
+    channel_type = "SMS"
     applicationId = None
     aws_access_key_id = None
     aws_secret_access_key = None
     address_dict = dict()
     message_configuration = dict()
-    template_configuration = dict()
     message_request = dict()
     response = None
-    destinationAddresses = None
+    destinationNumber = None
     message = None
-    sender = None
 
-    def __init__(self, region='eu-central-1', channel_type='EMAIL', sender=None,
+    def __init__(self, region='eu-central-1', message_type='TRANSACTIONAL', channel_type='SMS',
                  applicationId=None, aws_access=None, aws_secret=None):
         self.region = os.environ.get('REGION', region)
+        self.message_type = os.environ.get('PINPOINT_MESSAGE_TYPE', message_type)
         self.applicationId = os.environ.get('PINPOINT_APPLICATION_ID', applicationId)
         if self.applicationId is None:
             raise ValueError(ErrorCodes.APPLICATION_ID_ERROR)
         self.aws_access_key_id = os.environ.get('AWS_ACCESS', aws_access)
         if self.aws_access_key_id is None:
             raise ValueError(ErrorCodes.AWS_ACCESS_KEY_ERROR)
         self.aws_secret_access_key = os.environ.get('AWS_SECRET', aws_secret)
         if self.aws_secret_access_key is None:
             raise ValueError(ErrorCodes.AWS_SECRET_KEY_ERROR)
-        self.sender = os.environ.get('EMAIL_SENDER', sender)
-        if self.sender is None:
-            raise ValueError(ErrorCodes.MAIL_SENDER_ERROR)
         self.channel_type = os.environ.get('CHANNEL_TYPE', channel_type)
-        self.is_mail_send = False
-        self.error_message = ErrorCodes.MAIL_SEND_ERROR
+        self.is_sms_send = False
+        self.error_message = ErrorCodes.SMS_SEND_ERROR
         self.client = boto3.client('pinpoint', region_name=self.region, aws_access_key_id=self.aws_access_key_id,
                                    aws_secret_access_key=self.aws_secret_access_key)
 
-    def send(self, to_addresses, message=None, template_name=None, template_version=None):
+    def send(self, phone, message):
         try:
-            self.destinationAddresses = to_addresses
-            if self.destinationAddresses is None:
-                raise ValueError(ErrorCodes.DESTINATION_ADDRESS_ERROR)
+            self.destinationNumber = phone
+            if self.destinationNumber is None:
+                raise ValueError(ErrorCodes.DESTINATION_NUMBER_ERROR)
             self.message = message
             if self.message is None:
                 raise ValueError(ErrorCodes.MESSAGE_ERROR)
-
-            self.address_dict = {
-                to_address: {
-                    'ChannelType': 'EMAIL'
-                } for to_address in to_addresses
-            }
-            self.message_configuration = {'EmailMessage': {'FromAddress': self.sender}}
-            self.template_configuration = {
-                'EmailTemplate': {
-                    'Name': template_name,
-                    'Version': template_version
-                }
-            }
-            self.message_request = {'Addresses': self.address_dict, 'MessageConfiguration': self.message_configuration,
-                                    'TemplateConfiguration': self.template_configuration}
+            self.address_dict = {self.destinationNumber: {'ChannelType': self.channel_type}}
+            self.message_configuration = {'SMSMessage': {'Body': self.message, 'MessageType': self.message_type}}
+            self.message_request = {'Addresses': self.address_dict, 'MessageConfiguration': self.message_configuration}
             self.response = self.client.send_messages(ApplicationId=self.applicationId,
                                                       MessageRequest=self.message_request)
-
-            self.is_mail_send = self.check_mail_status()
-            if self.is_mail_send is False:
+            self.is_sms_send = self.check_sms_status()
+            if self.is_sms_send is False:
                 raise PinPointException(self.error_message)
         except ClientError as e:
             raise PinPointException(e.response['Error']['Message'])
 
-    def check_mail_status(self):
-        return {
-            to_address: message['MessageId'] for
-            to_address, message in self.response['MessageResponse']['Result'].items()
-        }
+    def check_sms_status(self):
+        return self.response is not None and 'MessageResponse' in self.response and 'Result' in self.response[
+            'MessageResponse'] and self.destinationNumber in self.response['MessageResponse'][
+                   'Result'] and 'DeliveryStatus' in self.response['MessageResponse']['Result'][
+                   self.destinationNumber] and \
+               self.response['MessageResponse']['Result'][self.destinationNumber][
+                   'DeliveryStatus'] == 'SUCCESSFUL'
```

### Comparing `PinPointClient-0.0.8/pinpoint/sms_service.py` & `PinPointClient-0.0.9/pinpoint/mail_service.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,66 +1,48 @@
+import json
 import os
 
 import boto3
 from botocore.exceptions import ClientError
 from pinpoint.exception import PinPointException, ErrorCodes
 
 
-class GsmService:
+class EMailService:
     region = "eu-central-1"
-    message_type = "TRANSACTIONAL"
-    channel_type = "SMS"
-    applicationId = None
+    channel_type = "EMAIL"
     aws_access_key_id = None
     aws_secret_access_key = None
-    address_dict = dict()
-    message_configuration = dict()
-    message_request = dict()
     response = None
-    destinationNumber = None
-    message = None
+    sender = None
 
-    def __init__(self, region='eu-central-1', message_type='TRANSACTIONAL', channel_type='SMS',
-                 applicationId=None, aws_access=None, aws_secret=None):
+    def __init__(self, region='eu-central-1', channel_type='EMAIL', sender=None, aws_access=None, aws_secret=None):
         self.region = os.environ.get('REGION', region)
-        self.message_type = os.environ.get('PINPOINT_MESSAGE_TYPE', message_type)
-        self.applicationId = os.environ.get('PINPOINT_APPLICATION_ID', applicationId)
-        if self.applicationId is None:
-            raise ValueError(ErrorCodes.APPLICATION_ID_ERROR)
         self.aws_access_key_id = os.environ.get('AWS_ACCESS', aws_access)
         if self.aws_access_key_id is None:
             raise ValueError(ErrorCodes.AWS_ACCESS_KEY_ERROR)
         self.aws_secret_access_key = os.environ.get('AWS_SECRET', aws_secret)
         if self.aws_secret_access_key is None:
             raise ValueError(ErrorCodes.AWS_SECRET_KEY_ERROR)
+        self.sender = os.environ.get('EMAIL_SENDER', sender)
+        if self.sender is None:
+            raise ValueError(ErrorCodes.MAIL_SENDER_ERROR)
         self.channel_type = os.environ.get('CHANNEL_TYPE', channel_type)
-        self.is_sms_send = False
-        self.error_message = ErrorCodes.SMS_SEND_ERROR
-        self.client = boto3.client('pinpoint', region_name=self.region, aws_access_key_id=self.aws_access_key_id,
+        self.client = boto3.client('pinpoint-email', region_name=self.region, aws_access_key_id=self.aws_access_key_id,
                                    aws_secret_access_key=self.aws_secret_access_key)
 
-    def send(self, phone, message):
+    def send_via_template(self, to_addresses=None, template_arn=None, data=None):
         try:
-            self.destinationNumber = phone
-            if self.destinationNumber is None:
-                raise ValueError(ErrorCodes.DESTINATION_NUMBER_ERROR)
-            self.message = message
-            if self.message is None:
+            if to_addresses is None or not isinstance(to_addresses, list) or len(to_addresses) == 0:
+                raise ValueError(ErrorCodes.DESTINATION_ADDRESS_ERROR)
+            if data is None:
                 raise ValueError(ErrorCodes.MESSAGE_ERROR)
-            self.address_dict = {self.destinationNumber: {'ChannelType': self.channel_type}}
-            self.message_configuration = {'SMSMessage': {'Body': self.message, 'MessageType': self.message_type}}
-            self.message_request = {'Addresses': self.address_dict, 'MessageConfiguration': self.message_configuration}
-            self.response = self.client.send_messages(ApplicationId=self.applicationId,
-                                                      MessageRequest=self.message_request)
-            self.is_sms_send = self.check_sms_status()
-            if self.is_sms_send is False:
-                raise PinPointException(self.error_message)
+            destination = {'ToAddresses': to_addresses}
+            content = {'Template': {'TemplateArn': template_arn, 'TemplateData': json.dumps(data)}}
+            self.response = self.client.send_email(FromEmailAddress=self.sender, Destination=destination,
+                                                   Content=content)
+            if self.check_send_via_template_status() is False:
+                raise PinPointException(ErrorCodes.MAIL_SEND_ERROR)
         except ClientError as e:
             raise PinPointException(e.response['Error']['Message'])
 
-    def check_sms_status(self):
-        return self.response is not None and 'MessageResponse' in self.response and 'Result' in self.response[
-            'MessageResponse'] and self.destinationNumber in self.response['MessageResponse'][
-                   'Result'] and 'DeliveryStatus' in self.response['MessageResponse']['Result'][
-                   self.destinationNumber] and \
-               self.response['MessageResponse']['Result'][self.destinationNumber][
-                   'DeliveryStatus'] == 'SUCCESSFUL'
+    def check_send_via_template_status(self):
+        return self.response is not None and 'MessageId' in self.response
```

### Comparing `PinPointClient-0.0.8/setup.py` & `PinPointClient-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name='PinPointClient',
-    version="0.0.8",
+    version="0.0.9",
     author="Yaşar Özyurt",
     author_email="blueromans@gmail.com",
     description='PinPoint Aws Pinpoint SMS/Mail Client Python package',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/blueromans/PinPointClient.git',
     project_urls={
```

