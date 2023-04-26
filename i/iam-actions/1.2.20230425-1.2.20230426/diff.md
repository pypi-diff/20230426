# Comparing `tmp/iam_actions-1.2.20230425.tar.gz` & `tmp/iam_actions-1.2.20230426.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20230425.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20230426.tar", max compression
```

## Comparing `iam_actions-1.2.20230425.tar` & `iam_actions-1.2.20230426.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-04-25 02:26:46.216415 iam_actions-1.2.20230425/LICENSE
--rw-r--r--   0        0        0     2302 2023-04-25 02:26:46.216415 iam_actions-1.2.20230425/README.md
--rw-r--r--   0        0        0      228 2023-04-25 02:26:46.216415 iam_actions-1.2.20230425/iam_actions/__init__.py
--rw-r--r--   0        0        0  4224168 2023-04-25 02:28:28.258005 iam_actions-1.2.20230425/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2023-04-25 02:26:46.216415 iam_actions-1.2.20230425/iam_actions/data.py
--rw-r--r--   0        0        0       80 2023-04-25 02:26:46.216415 iam_actions-1.2.20230425/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2023-04-25 02:26:46.216415 iam_actions-1.2.20230425/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2023-04-25 02:26:46.216415 iam_actions-1.2.20230425/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2023-04-25 02:26:46.216415 iam_actions-1.2.20230425/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2023-04-25 02:26:46.216415 iam_actions-1.2.20230425/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2023-04-25 02:26:46.220415 iam_actions-1.2.20230425/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2023-04-25 02:26:46.220415 iam_actions-1.2.20230425/iam_actions/generate/services.py
--rw-r--r--   0        0        0   543743 2023-04-25 02:28:28.258005 iam_actions-1.2.20230425/iam_actions/policies.json
--rw-r--r--   0        0        0   190303 2023-04-25 02:28:28.258005 iam_actions-1.2.20230425/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   527319 2023-04-25 02:28:28.258005 iam_actions-1.2.20230425/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2023-04-25 02:28:29.046018 iam_actions-1.2.20230425/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230425/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230425/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-26 02:30:56.313800 iam_actions-1.2.20230426/LICENSE
+-rw-r--r--   0        0        0     2302 2023-04-26 02:30:56.313800 iam_actions-1.2.20230426/README.md
+-rw-r--r--   0        0        0      228 2023-04-26 02:30:56.313800 iam_actions-1.2.20230426/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4224370 2023-04-26 02:32:19.336893 iam_actions-1.2.20230426/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2023-04-26 02:30:56.313800 iam_actions-1.2.20230426/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2023-04-26 02:30:56.317800 iam_actions-1.2.20230426/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2023-04-26 02:30:56.317800 iam_actions-1.2.20230426/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2023-04-26 02:30:56.317800 iam_actions-1.2.20230426/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2023-04-26 02:30:56.317800 iam_actions-1.2.20230426/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2023-04-26 02:30:56.317800 iam_actions-1.2.20230426/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2023-04-26 02:30:56.317800 iam_actions-1.2.20230426/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2023-04-26 02:30:56.317800 iam_actions-1.2.20230426/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   543474 2023-04-26 02:32:19.336893 iam_actions-1.2.20230426/iam_actions/policies.json
+-rw-r--r--   0        0        0   190303 2023-04-26 02:32:19.336893 iam_actions-1.2.20230426/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   527056 2023-04-26 02:32:19.336893 iam_actions-1.2.20230426/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2023-04-26 02:32:20.132886 iam_actions-1.2.20230426/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230426/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230426/PKG-INFO
```

### Comparing `iam_actions-1.2.20230425/LICENSE` & `iam_actions-1.2.20230426/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230425/README.md` & `iam_actions-1.2.20230426/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230425/iam_actions/actions.json` & `iam_actions-1.2.20230426/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999896728354263%*

 * *Differences: {"'aws-marketplace'": "{'GetResourcePolicy': {'access_level': 'Read', 'description': 'Grants "*

 * *                      "permission to get the resource policy of an existing entity', 'resources': "*

 * *                      "['Entity']}, 'PutResourcePolicy': {'access_level': 'Permissions "*

 * *                      "management', 'description': 'Grants permission to attach a resource policy "*

 * *                      "to an existing entity', 'resources': ['Entity']}, 'DeleteResourcePolicy': "*

 * *                      "{'acce […]*

```diff
@@ -10013,20 +10013,22 @@
             "action": "CreatePrivateMarketplaceRequests",
             "condition_keys": [],
             "description": "Grants permission to create a new request for a product or products to be associated with the Private Marketplace. This action can be performed by any account in an in an AWS Organization, provided the user has permissions to do so, and the Organization's Service Control Policies allow it",
             "orphan": false,
             "resources": []
         },
         "DeleteResourcePolicy": {
-            "access_level": "Undocumented",
+            "access_level": "Permissions management",
             "action": "DeleteResourcePolicy",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to delete the resource policy of an existing entity",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "Entity"
+            ]
         },
         "DescribeAgreement": {
             "access_level": "Read",
             "action": "DescribeAgreement",
             "condition_keys": [],
             "description": "Grants permission to users to describe the metadata about the agreement",
             "orphan": false,
@@ -10121,20 +10123,22 @@
             "action": "GetEntitlements",
             "condition_keys": [],
             "description": "Retrieves entitlement values for a given product. The results can be filtered based on customer identifier or product dimensions",
             "orphan": false,
             "resources": []
         },
         "GetResourcePolicy": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetResourcePolicy",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to get the resource policy of an existing entity",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "Entity"
+            ]
         },
         "GetSellerDashboard": {
             "access_level": "Read",
             "action": "GetSellerDashboard",
             "condition_keys": [],
             "description": "Grants permission to view a seller dashboard",
             "orphan": false,
@@ -10238,20 +10242,22 @@
             "action": "PutProcurementSystemConfiguration",
             "condition_keys": [],
             "description": "Grants permission to create or update the Procurement System integration configuration (e.g. Coupa) for the individual account, or for the entire AWS Organization if one exists. This action can only be performed by the master account if using an AWS Organization",
             "orphan": false,
             "resources": []
         },
         "PutResourcePolicy": {
-            "access_level": "Undocumented",
+            "access_level": "Permissions management",
             "action": "PutResourcePolicy",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to attach a resource policy to an existing entity",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "Entity"
+            ]
         },
         "RegisterUsage": {
             "access_level": "Write",
             "action": "RegisterUsage",
             "condition_keys": [],
             "description": "Grants permission to to verify that the customer running your paid software is subscribed to your product on AWS Marketplace, enabling you to guard against unauthorized use. Meters software use per ECS task, per hour, with usage prorated to the second",
             "orphan": false,
```

### Comparing `iam_actions-1.2.20230425/iam_actions/generate/action_map.py` & `iam_actions-1.2.20230426/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230425/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20230426/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230425/iam_actions/generate/generate.py` & `iam_actions-1.2.20230426/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230425/iam_actions/generate/notifier.py` & `iam_actions-1.2.20230426/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230425/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20230426/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230425/iam_actions/generate/services.py` & `iam_actions-1.2.20230426/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230425/iam_actions/policies.json` & `iam_actions-1.2.20230426/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999902256478999%*

 * *Differences: {"'serviceMap'": "{'AWS User Notifications Contacts': {'conditionKeys': {delete: [3]}}, 'AWS User "*

 * *                 "Notifications': {'conditionKeys': {delete: [7, 6, 5, 4, 3]}}}"}*

```diff
@@ -8968,20 +8968,15 @@
                 "UpdateNotificationConfiguration"
             ],
             "HasResource": true,
             "StringPrefix": "notifications",
             "conditionKeys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:ResourceTag/${TagKey}",
-                "aws:TagKeys",
-                "notifications:ChannelArn",
-                "notifications:ChannelNotificationConfigurationArn",
-                "notifications:EventRuleArn",
-                "notifications:NotificationConfigurationArn",
-                "notifications:NotificationEventArn"
+                "aws:TagKeys"
             ]
         },
         "AWS User Notifications Contacts": {
             "ARNFormat": "arn:aws:notifications-contacts::${Account}:${ResourceType}/${ResourceId}",
             "ARNRegex": "^arn:aws:notifications-contacts::.+:.+",
             "Actions": [
                 "ActivateEmailContact",
@@ -8995,16 +8990,15 @@
                 "UntagResource"
             ],
             "HasResource": true,
             "StringPrefix": "notifications-contacts",
             "conditionKeys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:ResourceTag/${TagKey}",
-                "aws:TagKeys",
-                "notifications-contacts:EmailContactResourceArn"
+                "aws:TagKeys"
             ]
         },
         "AWS WAF": {
             "ARNFormat": "arn:aws:waf::${Account}:${ResourceId}/${Id}",
             "ARNRegex": "^arn:aws:waf::[0-9]+:.+/.+",
             "Actions": [
                 "CreateByteMatchSet",
```

### Comparing `iam_actions-1.2.20230425/iam_actions/resourcetypes.json` & `iam_actions-1.2.20230426/iam_actions/resourcetypes.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230425/iam_actions/services.json` & `iam_actions-1.2.20230426/iam_actions/services.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998975889513108%*

 * *Differences: {"'notifications'": "{'ConditionKeys': {delete: [7, 6, 5, 4, 3]}}",*

 * * "'notifications-contacts'": "{'ConditionKeys': {delete: [3]}}"}*

```diff
@@ -14185,20 +14185,15 @@
             "UntagResource",
             "UpdateEventRule",
             "UpdateNotificationConfiguration"
         ],
         "ConditionKeys": [
             "aws:RequestTag/${TagKey}",
             "aws:ResourceTag/${TagKey}",
-            "aws:TagKeys",
-            "notifications:ChannelArn",
-            "notifications:ChannelNotificationConfigurationArn",
-            "notifications:EventRuleArn",
-            "notifications:NotificationConfigurationArn",
-            "notifications:NotificationEventArn"
+            "aws:TagKeys"
         ],
         "HasResource": true,
         "ServiceNames": [
             "AWS User Notifications"
         ]
     },
     "notifications-contacts": {
@@ -14218,16 +14213,15 @@
             "SendActivationCode",
             "TagResource",
             "UntagResource"
         ],
         "ConditionKeys": [
             "aws:RequestTag/${TagKey}",
             "aws:ResourceTag/${TagKey}",
-            "aws:TagKeys",
-            "notifications-contacts:EmailContactResourceArn"
+            "aws:TagKeys"
         ],
         "HasResource": true,
         "ServiceNames": [
             "AWS User Notifications Contacts"
         ]
     },
     "oam": {
```

### Comparing `iam_actions-1.2.20230425/pyproject.toml` & `iam_actions-1.2.20230426/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20230425"
+version = "1.2.20230426"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20230425/setup.py` & `iam_actions-1.2.20230426/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20230425',
+    'version': '1.2.20230426',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20230425/PKG-INFO` & `iam_actions-1.2.20230426/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20230425
+Version: 1.2.20230426
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

