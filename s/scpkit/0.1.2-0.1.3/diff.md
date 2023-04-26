# Comparing `tmp/scpkit-0.1.2.tar.gz` & `tmp/scpkit-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scpkit-0.1.2.tar", last modified: Tue Apr 25 18:00:00 2023, max compression
+gzip compressed data, was "scpkit-0.1.3.tar", last modified: Wed Apr 26 20:54:30 2023, max compression
```

## Comparing `scpkit-0.1.2.tar` & `scpkit-0.1.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:00:00.870787 scpkit-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-25 17:59:51.000000 scpkit-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-04-25 18:00:00.870787 scpkit-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-04-25 17:59:51.000000 scpkit-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-25 17:59:51.000000 scpkit-0.1.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:00:00.866787 scpkit-0.1.2/scpkit/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-25 17:59:51.000000 scpkit-0.1.2/scpkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-25 17:59:51.000000 scpkit-0.1.2/scpkit/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:00:00.870787 scpkit-0.1.2/scpkit/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 17:59:51.000000 scpkit-0.1.2/scpkit/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-04-25 17:59:51.000000 scpkit-0.1.2/scpkit/src/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-04-25 17:59:51.000000 scpkit-0.1.2/scpkit/src/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-04-25 17:59:51.000000 scpkit-0.1.2/scpkit/src/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-25 17:59:51.000000 scpkit-0.1.2/scpkit/src/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:00:00.870787 scpkit-0.1.2/scpkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-04-25 18:00:00.000000 scpkit-0.1.2/scpkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-25 18:00:00.000000 scpkit-0.1.2/scpkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 18:00:00.000000 scpkit-0.1.2/scpkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-25 18:00:00.000000 scpkit-0.1.2/scpkit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 18:00:00.000000 scpkit-0.1.2/scpkit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-25 18:00:00.000000 scpkit-0.1.2/scpkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-25 18:00:00.000000 scpkit-0.1.2/scpkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-25 18:00:00.870787 scpkit-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 17:59:51.000000 scpkit-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:00:00.870787 scpkit-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-04-25 17:59:51.000000 scpkit-0.1.2/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:54:30.232133 scpkit-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-26 20:54:05.000000 scpkit-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-04-26 20:54:30.232133 scpkit-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-04-26 20:54:05.000000 scpkit-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-26 20:54:05.000000 scpkit-0.1.3/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:54:30.228132 scpkit-0.1.3/scpkit/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-26 20:54:05.000000 scpkit-0.1.3/scpkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-26 20:54:05.000000 scpkit-0.1.3/scpkit/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:54:30.232133 scpkit-0.1.3/scpkit/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 20:54:05.000000 scpkit-0.1.3/scpkit/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-04-26 20:54:05.000000 scpkit-0.1.3/scpkit/src/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-04-26 20:54:05.000000 scpkit-0.1.3/scpkit/src/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-04-26 20:54:05.000000 scpkit-0.1.3/scpkit/src/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-26 20:54:05.000000 scpkit-0.1.3/scpkit/src/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:54:30.228132 scpkit-0.1.3/scpkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-04-26 20:54:30.000000 scpkit-0.1.3/scpkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-26 20:54:30.000000 scpkit-0.1.3/scpkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 20:54:30.000000 scpkit-0.1.3/scpkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-26 20:54:30.000000 scpkit-0.1.3/scpkit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 20:54:30.000000 scpkit-0.1.3/scpkit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-26 20:54:30.000000 scpkit-0.1.3/scpkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-26 20:54:30.000000 scpkit-0.1.3/scpkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-26 20:54:30.232133 scpkit-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 20:54:05.000000 scpkit-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:54:30.232133 scpkit-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-04-26 20:54:05.000000 scpkit-0.1.3/tests/test.py
```

### Comparing `scpkit-0.1.2/LICENSE` & `scpkit-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `scpkit-0.1.2/PKG-INFO` & `scpkit-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scpkit
-Version: 0.1.2
+Version: 0.1.3
 Summary: This package helps consolidate service control policies in AWS
 Home-page: https://www.aquia.us
 Author: Aquia
 Author-email: info@aquia.us
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/aquia-inc/scpkit/issues
 Project-URL: Source, https://github.com/aquia-inc/scpkit
@@ -14,15 +14,15 @@
 # SCPkit
 [![GitHub Super-Linter](https://github.com/aquia-inc/scpkit/workflows/Lint%20Code%20Base/badge.svg)](https://github.com/aquia-inc/scpkit/actions/workflows/linter.yaml)
 
 ## Overview
 
 This project provides a python module to aid in Service Control Policy management in AWS accounts. See our release [blog](https://blog.aquia.us/blog/) for additional details.
 
-SCPs have a current limit of 5 total per entity, and a size limit on each of 5120 bytes. This tool will merge selected SCPs into the fewest amount of policies, and optionally remove whitespaces characters as they count toward the byte limit.
+SCPs have a current limit of 5 total per entity, and a size limit on each of 5120 bytes. This tool will merge selected SCPs into the fewest amount of policies, and optionally remove whitespace characters as they count toward the byte limit.
 
 
 ```mermaid
   stateDiagram-v2
       [SCPTool] --> Validate
       [SCPTool] --> Merge
       Merge --> Validate
@@ -69,22 +69,22 @@
 
 
 ## Local development
 From the root of the folder:
 ```
 python3 -m venv .venv
 source .venv/bin/activate
-pip install -r requirements
+pip install -r requirements.txt
 python -m scpkit.main validate --sourcefiles ./scps --profile yourawsprofile
 ```
 Install as a package
 ```
 python3 -m venv .venv
 source .venv/bin/activate
-pip3 install -U git+https://github.com/aquia-inc/scpkit.git
+pip install -U git+https://github.com/aquia-inc/scpkit.git
 ```
 
 ## References
 This project would not be possible without the contributions of the following:
 * https://summitroute.com/blog/2020/03/25/aws_scp_best_practices/
 * https://github.com/ScaleSec/terraform_aws_scp
 * https://docs.aws.amazon.com/organizations/latest/userguide/orgs_manage_policies_scps_examples.html
```

### Comparing `scpkit-0.1.2/README.md` & `scpkit-0.1.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # SCPkit
 [![GitHub Super-Linter](https://github.com/aquia-inc/scpkit/workflows/Lint%20Code%20Base/badge.svg)](https://github.com/aquia-inc/scpkit/actions/workflows/linter.yaml)
 
 ## Overview
 
 This project provides a python module to aid in Service Control Policy management in AWS accounts. See our release [blog](https://blog.aquia.us/blog/) for additional details.
 
-SCPs have a current limit of 5 total per entity, and a size limit on each of 5120 bytes. This tool will merge selected SCPs into the fewest amount of policies, and optionally remove whitespaces characters as they count toward the byte limit.
+SCPs have a current limit of 5 total per entity, and a size limit on each of 5120 bytes. This tool will merge selected SCPs into the fewest amount of policies, and optionally remove whitespace characters as they count toward the byte limit.
 
 
 ```mermaid
   stateDiagram-v2
       [SCPTool] --> Validate
       [SCPTool] --> Merge
       Merge --> Validate
@@ -56,22 +56,22 @@
 
 
 ## Local development
 From the root of the folder:
 ```
 python3 -m venv .venv
 source .venv/bin/activate
-pip install -r requirements
+pip install -r requirements.txt
 python -m scpkit.main validate --sourcefiles ./scps --profile yourawsprofile
 ```
 Install as a package
 ```
 python3 -m venv .venv
 source .venv/bin/activate
-pip3 install -U git+https://github.com/aquia-inc/scpkit.git
+pip install -U git+https://github.com/aquia-inc/scpkit.git
 ```
 
 ## References
 This project would not be possible without the contributions of the following:
 * https://summitroute.com/blog/2020/03/25/aws_scp_best_practices/
 * https://github.com/ScaleSec/terraform_aws_scp
 * https://docs.aws.amazon.com/organizations/latest/userguide/orgs_manage_policies_scps_examples.html
```

### Comparing `scpkit-0.1.2/scpkit/main.py` & `scpkit-0.1.3/scpkit/main.py`

 * *Files identical despite different names*

### Comparing `scpkit-0.1.2/scpkit/src/merge.py` & `scpkit-0.1.3/scpkit/src/merge.py`

 * *Files identical despite different names*

### Comparing `scpkit-0.1.2/scpkit/src/model.py` & `scpkit-0.1.3/scpkit/src/model.py`

 * *Files identical despite different names*

### Comparing `scpkit-0.1.2/scpkit/src/util.py` & `scpkit-0.1.3/scpkit/src/util.py`

 * *Files identical despite different names*

### Comparing `scpkit-0.1.2/scpkit/src/validate.py` & `scpkit-0.1.3/scpkit/src/validate.py`

 * *Files identical despite different names*

### Comparing `scpkit-0.1.2/scpkit.egg-info/PKG-INFO` & `scpkit-0.1.3/scpkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scpkit
-Version: 0.1.2
+Version: 0.1.3
 Summary: This package helps consolidate service control policies in AWS
 Home-page: https://www.aquia.us
 Author: Aquia
 Author-email: info@aquia.us
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/aquia-inc/scpkit/issues
 Project-URL: Source, https://github.com/aquia-inc/scpkit
@@ -14,15 +14,15 @@
 # SCPkit
 [![GitHub Super-Linter](https://github.com/aquia-inc/scpkit/workflows/Lint%20Code%20Base/badge.svg)](https://github.com/aquia-inc/scpkit/actions/workflows/linter.yaml)
 
 ## Overview
 
 This project provides a python module to aid in Service Control Policy management in AWS accounts. See our release [blog](https://blog.aquia.us/blog/) for additional details.
 
-SCPs have a current limit of 5 total per entity, and a size limit on each of 5120 bytes. This tool will merge selected SCPs into the fewest amount of policies, and optionally remove whitespaces characters as they count toward the byte limit.
+SCPs have a current limit of 5 total per entity, and a size limit on each of 5120 bytes. This tool will merge selected SCPs into the fewest amount of policies, and optionally remove whitespace characters as they count toward the byte limit.
 
 
 ```mermaid
   stateDiagram-v2
       [SCPTool] --> Validate
       [SCPTool] --> Merge
       Merge --> Validate
@@ -69,22 +69,22 @@
 
 
 ## Local development
 From the root of the folder:
 ```
 python3 -m venv .venv
 source .venv/bin/activate
-pip install -r requirements
+pip install -r requirements.txt
 python -m scpkit.main validate --sourcefiles ./scps --profile yourawsprofile
 ```
 Install as a package
 ```
 python3 -m venv .venv
 source .venv/bin/activate
-pip3 install -U git+https://github.com/aquia-inc/scpkit.git
+pip install -U git+https://github.com/aquia-inc/scpkit.git
 ```
 
 ## References
 This project would not be possible without the contributions of the following:
 * https://summitroute.com/blog/2020/03/25/aws_scp_best_practices/
 * https://github.com/ScaleSec/terraform_aws_scp
 * https://docs.aws.amazon.com/organizations/latest/userguide/orgs_manage_policies_scps_examples.html
```

### Comparing `scpkit-0.1.2/setup.cfg` & `scpkit-0.1.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 project_urls = 
 	Bug Tracker = https://github.com/aquia-inc/scpkit/issues
 	Source = https://github.com/aquia-inc/scpkit
 description = This package helps consolidate service control policies in AWS
 license = Apache License 2.0
 long_description = file: README.md
 long_description_content_type = text/markdown
-version = 0.1.2
+version = 0.1.3
 
 [options]
 zip_safe = False
 include_package_data = True
 packages = find:
 install_requires = file: requirements.txt
```

### Comparing `scpkit-0.1.2/tests/test.py` & `scpkit-0.1.3/tests/test.py`

 * *Files identical despite different names*

