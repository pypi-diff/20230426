# Comparing `tmp/ads-pytest-parser-0.0.1.tar.gz` & `tmp/ads-pytest-parser-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ads-pytest-parser-0.0.1.tar", last modified: Mon Mar 13 14:34:48 2023, max compression
+gzip compressed data, was "ads-pytest-parser-0.0.2.tar", last modified: Wed Apr 26 15:02:03 2023, max compression
```

## Comparing `ads-pytest-parser-0.0.1.tar` & `ads-pytest-parser-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 aron       (501) staff       (20)        0 2023-03-13 14:34:48.121849 ads-pytest-parser-0.0.1/
--rw-r--r--   0 aron       (501) staff       (20)     1072 2023-03-10 11:45:49.000000 ads-pytest-parser-0.0.1/LICENSE
--rw-r--r--   0 aron       (501) staff       (20)     1398 2023-03-13 14:34:48.121931 ads-pytest-parser-0.0.1/PKG-INFO
--rw-r--r--   0 aron       (501) staff       (20)      771 2023-03-11 13:05:47.000000 ads-pytest-parser-0.0.1/README.md
--rw-r--r--   0 aron       (501) staff       (20)      813 2023-03-13 14:34:39.000000 ads-pytest-parser-0.0.1/pyproject.toml
--rw-r--r--   0 aron       (501) staff       (20)       79 2023-03-13 14:34:48.122247 ads-pytest-parser-0.0.1/setup.cfg
-drwxr-xr-x   0 aron       (501) staff       (20)        0 2023-03-13 14:34:48.119029 ads-pytest-parser-0.0.1/src/
-drwxr-xr-x   0 aron       (501) staff       (20)        0 2023-03-13 14:34:48.120474 ads-pytest-parser-0.0.1/src/ads_pytest_parser/
--rw-r--r--   0 aron       (501) staff       (20)        1 2023-03-13 12:50:48.000000 ads-pytest-parser-0.0.1/src/ads_pytest_parser/__init__.py
--rw-r--r--   0 aron       (501) staff       (20)     2817 2023-03-13 13:24:14.000000 ads-pytest-parser-0.0.1/src/ads_pytest_parser/assoc_devops_testcase_pytest_results.py
-drwxr-xr-x   0 aron       (501) staff       (20)        0 2023-03-13 14:34:48.121728 ads-pytest-parser-0.0.1/src/ads_pytest_parser.egg-info/
--rw-r--r--   0 aron       (501) staff       (20)     1398 2023-03-13 14:34:48.000000 ads-pytest-parser-0.0.1/src/ads_pytest_parser.egg-info/PKG-INFO
--rw-r--r--   0 aron       (501) staff       (20)      410 2023-03-13 14:34:48.000000 ads-pytest-parser-0.0.1/src/ads_pytest_parser.egg-info/SOURCES.txt
--rw-r--r--   0 aron       (501) staff       (20)        1 2023-03-13 14:34:48.000000 ads-pytest-parser-0.0.1/src/ads_pytest_parser.egg-info/dependency_links.txt
--rw-r--r--   0 aron       (501) staff       (20)       98 2023-03-13 14:34:48.000000 ads-pytest-parser-0.0.1/src/ads_pytest_parser.egg-info/entry_points.txt
--rw-r--r--   0 aron       (501) staff       (20)        9 2023-03-13 14:34:48.000000 ads-pytest-parser-0.0.1/src/ads_pytest_parser.egg-info/requires.txt
--rw-r--r--   0 aron       (501) staff       (20)       18 2023-03-13 14:34:48.000000 ads-pytest-parser-0.0.1/src/ads_pytest_parser.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:02:03.051289 ads-pytest-parser-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-26 15:01:43.000000 ads-pytest-parser-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-04-26 15:02:03.051289 ads-pytest-parser-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-26 15:01:43.000000 ads-pytest-parser-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-26 15:01:43.000000 ads-pytest-parser-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-26 15:02:03.051289 ads-pytest-parser-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:02:03.051289 ads-pytest-parser-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:02:03.051289 ads-pytest-parser-0.0.2/src/ads_pytest_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 15:01:43.000000 ads-pytest-parser-0.0.2/src/ads_pytest_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-04-26 15:01:43.000000 ads-pytest-parser-0.0.2/src/ads_pytest_parser/assoc_devops_testcase_pytest_results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:02:03.051289 ads-pytest-parser-0.0.2/src/ads_pytest_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-04-26 15:02:03.000000 ads-pytest-parser-0.0.2/src/ads_pytest_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-26 15:02:03.000000 ads-pytest-parser-0.0.2/src/ads_pytest_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 15:02:03.000000 ads-pytest-parser-0.0.2/src/ads_pytest_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-26 15:02:03.000000 ads-pytest-parser-0.0.2/src/ads_pytest_parser.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-26 15:02:03.000000 ads-pytest-parser-0.0.2/src/ads_pytest_parser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-26 15:02:03.000000 ads-pytest-parser-0.0.2/src/ads_pytest_parser.egg-info/top_level.txt
```

### Comparing `ads-pytest-parser-0.0.1/LICENSE` & `ads-pytest-parser-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ads-pytest-parser-0.0.1/PKG-INFO` & `ads-pytest-parser-0.0.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 Metadata-Version: 2.1
 Name: ads-pytest-parser
-Version: 0.0.1
+Version: 0.0.2
 Summary: Associate DevOps test cases with pytest XML results
 Author-email: VisualLabs Kft <aron.paljakab@visuallabs.hu>, Aron Pal-Jakab <aron.paljakab@visuallabs.hu>
 Project-URL: Homepage, https://github.com/VisualLabs-Kft/vl-ads-pytest-parser
 Project-URL: Bug Tracker, https://github.com/VisualLabs-Kft/vl-ads-pytest-parser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+![Version](https://img.shields.io/pypi/v/ads-pytest-parser.svg)
+
 # Pytest Parser to Azure DevOps Test Case
-Associate DevOps test cases with pytest XML results
+Associate DevOps test cases with pytest nunit XML results
 
 
 ## Usage
 The parser should be run on an Azure DevOps ```pytest-azurepipelines``` generated XML file, because it searches for the following attributes:
-- testcase
-  - name
-  - result
+- "test-case"
+  - "methodname"
+  - "result"
 
 The Python script requires the following arguments:
 - org: Azure DevOps organization name
 - project: Azure DevOps project name
 - plan: Azure DevOps test plan name
 - suite: Azure DevOps test suite name
 - auth: Azure DevOps personal access token
 - xml: pytest-azurepipelines generated XML file
 
+The test cases should be named in the following format: ```testcase_<DevOpsID>``` , i.e. ```def testcase_123456():```
+
 For example:
 ```
 ads-pytest-parser org project planID suiteID authToken test.xml
 ```
 
 The script will then associate the test cases with the test results - for the test cases the outcome will be set.
```

### Comparing `ads-pytest-parser-0.0.1/README.md` & `ads-pytest-parser-0.0.2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,28 @@
+![Version](https://img.shields.io/pypi/v/ads-pytest-parser.svg)
+
 # Pytest Parser to Azure DevOps Test Case
-Associate DevOps test cases with pytest XML results
+Associate DevOps test cases with pytest nunit XML results
 
 
 ## Usage
 The parser should be run on an Azure DevOps ```pytest-azurepipelines``` generated XML file, because it searches for the following attributes:
-- testcase
-  - name
-  - result
+- "test-case"
+  - "methodname"
+  - "result"
 
 The Python script requires the following arguments:
 - org: Azure DevOps organization name
 - project: Azure DevOps project name
 - plan: Azure DevOps test plan name
 - suite: Azure DevOps test suite name
 - auth: Azure DevOps personal access token
 - xml: pytest-azurepipelines generated XML file
 
+The test cases should be named in the following format: ```testcase_<DevOpsID>``` , i.e. ```def testcase_123456():```
+
 For example:
 ```
 ads-pytest-parser org project planID suiteID authToken test.xml
 ```
 
 The script will then associate the test cases with the test results - for the test cases the outcome will be set.
```

### Comparing `ads-pytest-parser-0.0.1/pyproject.toml` & `ads-pytest-parser-0.0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ads-pytest-parser"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="VisualLabs Kft", email="aron.paljakab@visuallabs.hu" },
   { name="Aron Pal-Jakab", email="aron.paljakab@visuallabs.hu" },
 ]
 description = "Associate DevOps test cases with pytest XML results"
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `ads-pytest-parser-0.0.1/src/ads_pytest_parser/assoc_devops_testcase_pytest_results.py` & `ads-pytest-parser-0.0.2/src/ads_pytest_parser/assoc_devops_testcase_pytest_results.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,15 +42,14 @@
     # Parse the JUnit XML file
     tree = ET.parse(XML_FILE)
     root = tree.getroot()
 
     # Construct the URL and the header
     URL = f"https://dev.azure.com/{ORGANIZATION}/{PROJECT}/_apis/testplan/Plans/{PLAN_ID}/Suites/{SUITE_ID}/TestPoint?api-version=7.0"
     headers = {
-        "Authorization": f"Basic {AUTH_TOKEN}",
         "Content-Type": "application/json",
     }
 
     body = []
 
     # Loop through each test case in the XML file
     for testcase in root.iter("test-case"):
@@ -73,9 +72,11 @@
 
         # create a json array
         body.append(test_case_json)
 
     print(body)
 
     # send an http request to the URL
-    response = requests.patch(URL, headers=headers, data=json.dumps(body))
+    response = requests.patch(
+        URL, headers=headers, auth=("", AUTH_TOKEN), data=json.dumps(body)
+    )
     print(response)
```

### Comparing `ads-pytest-parser-0.0.1/src/ads_pytest_parser.egg-info/PKG-INFO` & `ads-pytest-parser-0.0.2/src/ads_pytest_parser.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 Metadata-Version: 2.1
 Name: ads-pytest-parser
-Version: 0.0.1
+Version: 0.0.2
 Summary: Associate DevOps test cases with pytest XML results
 Author-email: VisualLabs Kft <aron.paljakab@visuallabs.hu>, Aron Pal-Jakab <aron.paljakab@visuallabs.hu>
 Project-URL: Homepage, https://github.com/VisualLabs-Kft/vl-ads-pytest-parser
 Project-URL: Bug Tracker, https://github.com/VisualLabs-Kft/vl-ads-pytest-parser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+![Version](https://img.shields.io/pypi/v/ads-pytest-parser.svg)
+
 # Pytest Parser to Azure DevOps Test Case
-Associate DevOps test cases with pytest XML results
+Associate DevOps test cases with pytest nunit XML results
 
 
 ## Usage
 The parser should be run on an Azure DevOps ```pytest-azurepipelines``` generated XML file, because it searches for the following attributes:
-- testcase
-  - name
-  - result
+- "test-case"
+  - "methodname"
+  - "result"
 
 The Python script requires the following arguments:
 - org: Azure DevOps organization name
 - project: Azure DevOps project name
 - plan: Azure DevOps test plan name
 - suite: Azure DevOps test suite name
 - auth: Azure DevOps personal access token
 - xml: pytest-azurepipelines generated XML file
 
+The test cases should be named in the following format: ```testcase_<DevOpsID>``` , i.e. ```def testcase_123456():```
+
 For example:
 ```
 ads-pytest-parser org project planID suiteID authToken test.xml
 ```
 
 The script will then associate the test cases with the test results - for the test cases the outcome will be set.
```

