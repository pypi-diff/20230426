# Comparing `tmp/iam-credential-rotation-0.2.0.tar.gz` & `tmp/iam-credential-rotation-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam-credential-rotation-0.2.0.tar", last modified: Wed Apr 26 19:50:45 2023, max compression
+gzip compressed data, was "iam-credential-rotation-0.2.1.tar", last modified: Wed Apr 26 20:05:02 2023, max compression
```

## Comparing `iam-credential-rotation-0.2.0.tar` & `iam-credential-rotation-0.2.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-26 19:50:45.171251 iam-credential-rotation-0.2.0/
-drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-26 19:50:45.167251 iam-credential-rotation-0.2.0/.circleci/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4159 2023-04-26 19:50:37.000000 iam-credential-rotation-0.2.0/.circleci/config.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)      114 2023-04-26 19:50:37.000000 iam-credential-rotation-0.2.0/.gitignore
--rw-r--r--   0 circleci  (3434) circleci  (3434)      831 2023-04-26 19:50:37.000000 iam-credential-rotation-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0 circleci  (3434) circleci  (3434)    18369 2023-04-26 19:50:37.000000 iam-credential-rotation-0.2.0/.pylintrc
--rw-r--r--   0 circleci  (3434) circleci  (3434)        6 2023-04-26 19:50:37.000000 iam-credential-rotation-0.2.0/.python-version
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1075 2023-04-26 19:50:37.000000 iam-credential-rotation-0.2.0/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)      544 2023-04-26 19:50:45.171251 iam-credential-rotation-0.2.0/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      436 2023-04-26 19:50:37.000000 iam-credential-rotation-0.2.0/Pipfile
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3795 2023-04-26 19:50:37.000000 iam-credential-rotation-0.2.0/README.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2590 2023-04-26 19:50:37.000000 iam-credential-rotation-0.2.0/discussion.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      246 2023-04-26 19:50:37.000000 iam-credential-rotation-0.2.0/op.env
--rw-r--r--   0 circleci  (3434) circleci  (3434)      828 2023-04-26 19:50:37.000000 iam-credential-rotation-0.2.0/pyproject.toml
--rw-r--r--   0 circleci  (3434) circleci  (3434)      182 2023-04-26 19:50:37.000000 iam-credential-rotation-0.2.0/requirements.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-04-26 19:50:45.171251 iam-credential-rotation-0.2.0/setup.cfg
-drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-26 19:50:45.167251 iam-credential-rotation-0.2.0/src/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-26 19:50:37.000000 iam-credential-rotation-0.2.0/src/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      160 2023-04-26 19:50:45.000000 iam-credential-rotation-0.2.0/src/_version.py
-drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-26 19:50:45.167251 iam-credential-rotation-0.2.0/src/iam_credential_rotation.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      544 2023-04-26 19:50:45.000000 iam-credential-rotation-0.2.0/src/iam_credential_rotation.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      646 2023-04-26 19:50:45.000000 iam-credential-rotation-0.2.0/src/iam_credential_rotation.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-04-26 19:50:45.000000 iam-credential-rotation-0.2.0/src/iam_credential_rotation.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       72 2023-04-26 19:50:45.000000 iam-credential-rotation-0.2.0/src/iam_credential_rotation.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       14 2023-04-26 19:50:45.000000 iam-credential-rotation-0.2.0/src/iam_credential_rotation.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       61 2023-04-26 19:50:45.000000 iam-credential-rotation-0.2.0/src/iam_credential_rotation.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      668 2023-04-26 19:50:37.000000 iam-credential-rotation-0.2.0/src/iam_credential_rotation.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2365 2023-04-26 19:50:37.000000 iam-credential-rotation-0.2.0/src/provider_aws.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1506 2023-04-26 19:50:37.000000 iam-credential-rotation-0.2.0/src/utils.py
-drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-26 19:50:45.171251 iam-credential-rotation-0.2.0/test/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      911 2023-04-26 19:50:37.000000 iam-credential-rotation-0.2.0/test/test_iam_credential_rotation.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2883 2023-04-26 19:50:37.000000 iam-credential-rotation-0.2.0/test/test_provider_aws.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1036 2023-04-26 19:50:37.000000 iam-credential-rotation-0.2.0/test/test_utils.py
+drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-26 20:05:02.835887 iam-credential-rotation-0.2.1/
+drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-26 20:05:02.831886 iam-credential-rotation-0.2.1/.circleci/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4159 2023-04-26 20:04:55.000000 iam-credential-rotation-0.2.1/.circleci/config.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      114 2023-04-26 20:04:55.000000 iam-credential-rotation-0.2.1/.gitignore
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      831 2023-04-26 20:04:55.000000 iam-credential-rotation-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    18369 2023-04-26 20:04:55.000000 iam-credential-rotation-0.2.1/.pylintrc
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        6 2023-04-26 20:04:55.000000 iam-credential-rotation-0.2.1/.python-version
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1075 2023-04-26 20:04:55.000000 iam-credential-rotation-0.2.1/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      544 2023-04-26 20:05:02.835887 iam-credential-rotation-0.2.1/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      436 2023-04-26 20:04:55.000000 iam-credential-rotation-0.2.1/Pipfile
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3795 2023-04-26 20:04:55.000000 iam-credential-rotation-0.2.1/README.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2590 2023-04-26 20:04:55.000000 iam-credential-rotation-0.2.1/discussion.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      246 2023-04-26 20:04:55.000000 iam-credential-rotation-0.2.1/op.env
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      888 2023-04-26 20:04:55.000000 iam-credential-rotation-0.2.1/pyproject.toml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      182 2023-04-26 20:04:55.000000 iam-credential-rotation-0.2.1/requirements.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-04-26 20:05:02.835887 iam-credential-rotation-0.2.1/setup.cfg
+drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-26 20:05:02.831886 iam-credential-rotation-0.2.1/src/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-26 20:04:55.000000 iam-credential-rotation-0.2.1/src/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      160 2023-04-26 20:05:02.000000 iam-credential-rotation-0.2.1/src/_version.py
+drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-26 20:05:02.835887 iam-credential-rotation-0.2.1/src/iam_credential_rotation.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      544 2023-04-26 20:05:02.000000 iam-credential-rotation-0.2.1/src/iam_credential_rotation.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      646 2023-04-26 20:05:02.000000 iam-credential-rotation-0.2.1/src/iam_credential_rotation.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-04-26 20:05:02.000000 iam-credential-rotation-0.2.1/src/iam_credential_rotation.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       72 2023-04-26 20:05:02.000000 iam-credential-rotation-0.2.1/src/iam_credential_rotation.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       56 2023-04-26 20:05:02.000000 iam-credential-rotation-0.2.1/src/iam_credential_rotation.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       61 2023-04-26 20:05:02.000000 iam-credential-rotation-0.2.1/src/iam_credential_rotation.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      668 2023-04-26 20:04:55.000000 iam-credential-rotation-0.2.1/src/iam_credential_rotation.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2365 2023-04-26 20:04:55.000000 iam-credential-rotation-0.2.1/src/provider_aws.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1506 2023-04-26 20:04:55.000000 iam-credential-rotation-0.2.1/src/utils.py
+drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-26 20:05:02.835887 iam-credential-rotation-0.2.1/test/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      911 2023-04-26 20:04:55.000000 iam-credential-rotation-0.2.1/test/test_iam_credential_rotation.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2883 2023-04-26 20:04:55.000000 iam-credential-rotation-0.2.1/test/test_provider_aws.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1036 2023-04-26 20:04:55.000000 iam-credential-rotation-0.2.1/test/test_utils.py
```

### Comparing `iam-credential-rotation-0.2.0/.circleci/config.yml` & `iam-credential-rotation-0.2.1/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `iam-credential-rotation-0.2.0/.pre-commit-config.yaml` & `iam-credential-rotation-0.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `iam-credential-rotation-0.2.0/.pylintrc` & `iam-credential-rotation-0.2.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `iam-credential-rotation-0.2.0/LICENSE` & `iam-credential-rotation-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `iam-credential-rotation-0.2.0/PKG-INFO` & `iam-credential-rotation-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-credential-rotation
-Version: 0.2.0
+Version: 0.2.1
 Summary: automated rotation for iam machine account programmatic credentials
 Author-email: Nic Cheneweth <nchenewe@thoughtworks.com>
 Project-URL: Homepage, https://github.com/ThoughtWorks-DPS/iam-credential-rotation
 Project-URL: Bug Tracker, https://github.com/ThoughtWorks-DPS/iam-credential-rotation/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `iam-credential-rotation-0.2.0/README.md` & `iam-credential-rotation-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `iam-credential-rotation-0.2.0/discussion.md` & `iam-credential-rotation-0.2.1/discussion.md`

 * *Files identical despite different names*

### Comparing `iam-credential-rotation-0.2.0/pyproject.toml` & `iam-credential-rotation-0.2.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -9,14 +9,16 @@
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
   "click >= 8.1, < 9",
+  "boto3 >= 1.26.120, < 2",
+  "pathvalidate >= 2.5.2, < 3",
 ]
 dynamic = ["version"]
 
 [project.urls]
 "Homepage" = "https://github.com/ThoughtWorks-DPS/iam-credential-rotation"
 "Bug Tracker" = "https://github.com/ThoughtWorks-DPS/iam-credential-rotation/issues"
```

### Comparing `iam-credential-rotation-0.2.0/src/iam_credential_rotation.egg-info/PKG-INFO` & `iam-credential-rotation-0.2.1/src/iam_credential_rotation.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-credential-rotation
-Version: 0.2.0
+Version: 0.2.1
 Summary: automated rotation for iam machine account programmatic credentials
 Author-email: Nic Cheneweth <nchenewe@thoughtworks.com>
 Project-URL: Homepage, https://github.com/ThoughtWorks-DPS/iam-credential-rotation
 Project-URL: Bug Tracker, https://github.com/ThoughtWorks-DPS/iam-credential-rotation/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `iam-credential-rotation-0.2.0/src/iam_credential_rotation.egg-info/SOURCES.txt` & `iam-credential-rotation-0.2.1/src/iam_credential_rotation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iam-credential-rotation-0.2.0/src/iam_credential_rotation.py` & `iam-credential-rotation-0.2.1/src/iam_credential_rotation.py`

 * *Files identical despite different names*

### Comparing `iam-credential-rotation-0.2.0/src/provider_aws.py` & `iam-credential-rotation-0.2.1/src/provider_aws.py`

 * *Files identical despite different names*

### Comparing `iam-credential-rotation-0.2.0/src/utils.py` & `iam-credential-rotation-0.2.1/src/utils.py`

 * *Files identical despite different names*

### Comparing `iam-credential-rotation-0.2.0/test/test_iam_credential_rotation.py` & `iam-credential-rotation-0.2.1/test/test_iam_credential_rotation.py`

 * *Files identical despite different names*

### Comparing `iam-credential-rotation-0.2.0/test/test_provider_aws.py` & `iam-credential-rotation-0.2.1/test/test_provider_aws.py`

 * *Files identical despite different names*

### Comparing `iam-credential-rotation-0.2.0/test/test_utils.py` & `iam-credential-rotation-0.2.1/test/test_utils.py`

 * *Files identical despite different names*

