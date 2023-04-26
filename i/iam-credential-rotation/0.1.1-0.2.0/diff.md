# Comparing `tmp/iam-credential-rotation-0.1.1.tar.gz` & `tmp/iam-credential-rotation-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam-credential-rotation-0.1.1.tar", last modified: Thu Mar  9 07:52:39 2023, max compression
+gzip compressed data, was "iam-credential-rotation-0.2.0.tar", last modified: Wed Apr 26 19:50:45 2023, max compression
```

## Comparing `iam-credential-rotation-0.1.1.tar` & `iam-credential-rotation-0.2.0.tar`

### file list

```diff
@@ -1,35 +1,33 @@
-drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-09 07:52:39.844890 iam-credential-rotation-0.1.1/
-drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-09 07:52:39.844890 iam-credential-rotation-0.1.1/.circleci/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4159 2023-03-09 07:52:34.000000 iam-credential-rotation-0.1.1/.circleci/config.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)      263 2023-03-09 07:52:34.000000 iam-credential-rotation-0.1.1/.codeclimate.yaml
--rw-r--r--   0 circleci  (3434) circleci  (3434)       29 2023-03-09 07:52:34.000000 iam-credential-rotation-0.1.1/.gitattributes
--rw-r--r--   0 circleci  (3434) circleci  (3434)      100 2023-03-09 07:52:34.000000 iam-credential-rotation-0.1.1/.gitignore
--rw-r--r--   0 circleci  (3434) circleci  (3434)      866 2023-03-09 07:52:34.000000 iam-credential-rotation-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0 circleci  (3434) circleci  (3434)    18369 2023-03-09 07:52:34.000000 iam-credential-rotation-0.1.1/.pylintrc
--rw-r--r--   0 circleci  (3434) circleci  (3434)        7 2023-03-09 07:52:34.000000 iam-credential-rotation-0.1.1/.python-version
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1075 2023-03-09 07:52:34.000000 iam-credential-rotation-0.1.1/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4006 2023-03-09 07:52:39.844890 iam-credential-rotation-0.1.1/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      424 2023-03-09 07:52:34.000000 iam-credential-rotation-0.1.1/Pipfile
--rw-r--r--   0 circleci  (3434) circleci  (3434)    63593 2023-03-09 07:52:34.000000 iam-credential-rotation-0.1.1/Pipfile.lock
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3298 2023-03-09 07:52:34.000000 iam-credential-rotation-0.1.1/README.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2590 2023-03-09 07:52:34.000000 iam-credential-rotation-0.1.1/discussion.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      246 2023-03-09 07:52:34.000000 iam-credential-rotation-0.1.1/op.env
--rw-r--r--   0 circleci  (3434) circleci  (3434)      772 2023-03-09 07:52:34.000000 iam-credential-rotation-0.1.1/pyproject.toml
--rw-r--r--   0 circleci  (3434) circleci  (3434)      266 2023-03-09 07:52:34.000000 iam-credential-rotation-0.1.1/requirements.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-03-09 07:52:39.844890 iam-credential-rotation-0.1.1/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)      860 2023-03-09 07:52:34.000000 iam-credential-rotation-0.1.1/setup.py
-drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-09 07:52:39.844890 iam-credential-rotation-0.1.1/src/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-09 07:52:34.000000 iam-credential-rotation-0.1.1/src/__init__.py
-drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-09 07:52:39.844890 iam-credential-rotation-0.1.1/src/iam_credential_rotation.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4006 2023-03-09 07:52:39.000000 iam-credential-rotation-0.1.1/src/iam_credential_rotation.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      635 2023-03-09 07:52:39.000000 iam-credential-rotation-0.1.1/src/iam_credential_rotation.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-03-09 07:52:39.000000 iam-credential-rotation-0.1.1/src/iam_credential_rotation.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       72 2023-03-09 07:52:39.000000 iam-credential-rotation-0.1.1/src/iam_credential_rotation.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-03-09 07:52:39.000000 iam-credential-rotation-0.1.1/src/iam_credential_rotation.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      668 2023-03-09 07:52:34.000000 iam-credential-rotation-0.1.1/src/iam_credential_rotation.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2365 2023-03-09 07:52:34.000000 iam-credential-rotation-0.1.1/src/provider_aws.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1506 2023-03-09 07:52:34.000000 iam-credential-rotation-0.1.1/src/utils.py
-drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-09 07:52:39.844890 iam-credential-rotation-0.1.1/test/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      911 2023-03-09 07:52:34.000000 iam-credential-rotation-0.1.1/test/test_iam_credential_rotation.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2883 2023-03-09 07:52:34.000000 iam-credential-rotation-0.1.1/test/test_provider_aws.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1036 2023-03-09 07:52:34.000000 iam-credential-rotation-0.1.1/test/test_utils.py
+drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-26 19:50:45.171251 iam-credential-rotation-0.2.0/
+drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-26 19:50:45.167251 iam-credential-rotation-0.2.0/.circleci/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4159 2023-04-26 19:50:37.000000 iam-credential-rotation-0.2.0/.circleci/config.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      114 2023-04-26 19:50:37.000000 iam-credential-rotation-0.2.0/.gitignore
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      831 2023-04-26 19:50:37.000000 iam-credential-rotation-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    18369 2023-04-26 19:50:37.000000 iam-credential-rotation-0.2.0/.pylintrc
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        6 2023-04-26 19:50:37.000000 iam-credential-rotation-0.2.0/.python-version
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1075 2023-04-26 19:50:37.000000 iam-credential-rotation-0.2.0/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      544 2023-04-26 19:50:45.171251 iam-credential-rotation-0.2.0/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      436 2023-04-26 19:50:37.000000 iam-credential-rotation-0.2.0/Pipfile
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3795 2023-04-26 19:50:37.000000 iam-credential-rotation-0.2.0/README.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2590 2023-04-26 19:50:37.000000 iam-credential-rotation-0.2.0/discussion.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      246 2023-04-26 19:50:37.000000 iam-credential-rotation-0.2.0/op.env
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      828 2023-04-26 19:50:37.000000 iam-credential-rotation-0.2.0/pyproject.toml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      182 2023-04-26 19:50:37.000000 iam-credential-rotation-0.2.0/requirements.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-04-26 19:50:45.171251 iam-credential-rotation-0.2.0/setup.cfg
+drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-26 19:50:45.167251 iam-credential-rotation-0.2.0/src/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-26 19:50:37.000000 iam-credential-rotation-0.2.0/src/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      160 2023-04-26 19:50:45.000000 iam-credential-rotation-0.2.0/src/_version.py
+drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-26 19:50:45.167251 iam-credential-rotation-0.2.0/src/iam_credential_rotation.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      544 2023-04-26 19:50:45.000000 iam-credential-rotation-0.2.0/src/iam_credential_rotation.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      646 2023-04-26 19:50:45.000000 iam-credential-rotation-0.2.0/src/iam_credential_rotation.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-04-26 19:50:45.000000 iam-credential-rotation-0.2.0/src/iam_credential_rotation.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       72 2023-04-26 19:50:45.000000 iam-credential-rotation-0.2.0/src/iam_credential_rotation.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       14 2023-04-26 19:50:45.000000 iam-credential-rotation-0.2.0/src/iam_credential_rotation.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       61 2023-04-26 19:50:45.000000 iam-credential-rotation-0.2.0/src/iam_credential_rotation.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      668 2023-04-26 19:50:37.000000 iam-credential-rotation-0.2.0/src/iam_credential_rotation.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2365 2023-04-26 19:50:37.000000 iam-credential-rotation-0.2.0/src/provider_aws.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1506 2023-04-26 19:50:37.000000 iam-credential-rotation-0.2.0/src/utils.py
+drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-26 19:50:45.171251 iam-credential-rotation-0.2.0/test/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      911 2023-04-26 19:50:37.000000 iam-credential-rotation-0.2.0/test/test_iam_credential_rotation.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2883 2023-04-26 19:50:37.000000 iam-credential-rotation-0.2.0/test/test_provider_aws.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1036 2023-04-26 19:50:37.000000 iam-credential-rotation-0.2.0/test/test_utils.py
```

### Comparing `iam-credential-rotation-0.1.1/.circleci/config.yml` & `iam-credential-rotation-0.2.0/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `iam-credential-rotation-0.1.1/.pre-commit-config.yaml` & `iam-credential-rotation-0.2.0/.pre-commit-config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,14 @@
       - id: check-added-large-files
       - id: check-json
       - id: check-yaml
         args: [--allow-multiple-documents]
         exclude: ^chart/
       - id: forbid-new-submodules
       - id: detect-private-key
-      - id: detect-aws-credentials
       - id: end-of-file-fixer
       - id: trailing-whitespace
         args: [--markdown-linebreak-ext=md]
   - repo: local
     hooks:
       - id: git-secrets
         name: git-secrets
```

### Comparing `iam-credential-rotation-0.1.1/.pylintrc` & `iam-credential-rotation-0.2.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `iam-credential-rotation-0.1.1/LICENSE` & `iam-credential-rotation-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `iam-credential-rotation-0.1.1/PKG-INFO` & `iam-credential-rotation-0.2.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: iam-credential-rotation
-Version: 0.1.1
-Summary: automated rotation for iam machine account programmatic credentials
-Home-page: https://github.com/ThoughtWorks-DPS/iam-credential-rotatation
-Author: Nic Cheneweth
-Author-email: Nic Cheneweth <nchenewe@thoughtworks.com>
-Project-URL: Homepage, https://github.com/ThoughtWorks-DPS/iam-credential-rotatation
-Project-URL: Bug Tracker, https://github.com/ThoughtWorks-DPS/iam-credential-rotatation/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <div align="center">
 	<p>
 		<img alt="Thoughtworks Logo" src="https://raw.githubusercontent.com/ThoughtWorks-DPS/static/master/thoughtworks_flamingo_wave.png?sanitize=true" width=200 />
     <br />
 		<img alt="DPS Title" src="https://raw.githubusercontent.com/ThoughtWorks-DPS/static/master/EMPCPlatformStarterKitsImage.png?sanitize=true" width=350/>
 	</p>
   <br />
@@ -72,16 +56,34 @@
 
 ### Development
 
 The pipeline uses `requirements.txt` but there is also a Pipfile if you prefer pipenv for local development.  
 
 **Pipenv setup**  
 ```
-$ pipenv --python 3.10  
-$ pipenv shell  
-$ pipenv install --dev  
+echo '3.11.3' > .python-version    # using pyenv for version selection
+pipenv --python 3.11               # pipenv creates the virtual env  
+pipenv shell  
+pipenv install --dev  
 ```
+For the build pipeline, the packages build dependencies are also maintained in a `requirements.txt` file since (currently) the generic python build environment already exists on the build executor.  
+
 **Run unit tests**  
 ```
-$ PYTHONPATH=.:./src coverage run -m pytest -vv -l  
-$ coverage report  
+PYTHONPATH=.:./src coverage run -m pytest -vv -l  
+coverage report  
+```
+
+**build**  
+```
+python -m build
+```
+
+**install locally during development**  
+```
+pip install --editable .
+```
+
+** check setuptools-scm dynamic version**
+```
+python -m setuptools_scm
 ```
```

#### html2text {}

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1 Name: iam-credential-rotation Version: 0.1.1 Summary:
-automated rotation for iam machine account programmatic credentials Home-page:
-https://github.com/ThoughtWorks-DPS/iam-credential-rotatation Author: Nic
-Cheneweth Author-email: Nic Cheneweth
-thoughtworks.com> Project-URL: Homepage, https://github.com/ThoughtWorks-DPS/
-iam-credential-rotatation Project-URL: Bug Tracker, https://github.com/
-ThoughtWorks-DPS/iam-credential-rotatation/issues Classifier: Programming
-Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent Requires-Python: >=3.10
-Description-Content-Type: text/markdown License-File: LICENSE
                              [Thoughtworks Logo]
                                   [DPS Title]
 
                        **** iam-credential-rotation ****
  [https://dl.circleci.com/status-badge/img/gh/ThoughtWorks-DPS/iam-credential-
  rotatation/tree/main.svg?style=shield] [https://img.shields.io/badge/license-
                                  MIT-blue.svg]
@@ -42,10 +32,16 @@
 write the new credentials into a Secrets store._ ``` $ iam-credential-rotation
 PSKServiceAccounts { "PSKNonprodServiceAccount": { "AccessKeyId":
 "AKIARKL**************", "SecretAccessKey":
 "bCFqIBZUo****************************" }, "PSKProdServiceAccount":
 { "AccessKeyId": "AKIARKLI**************", "SecretAccessKey":
 "cVSkOhunYxS****************************" } } ``` ### Development The pipeline
 uses `requirements.txt` but there is also a Pipfile if you prefer pipenv for
-local development. **Pipenv setup** ``` $ pipenv --python 3.10 $ pipenv shell $
-pipenv install --dev ``` **Run unit tests** ``` $ PYTHONPATH=.:./src coverage
-run -m pytest -vv -l $ coverage report ```
+local development. **Pipenv setup** ``` echo '3.11.3' > .python-version # using
+pyenv for version selection pipenv --python 3.11 # pipenv creates the virtual
+env pipenv shell pipenv install --dev ``` For the build pipeline, the packages
+build dependencies are also maintained in a `requirements.txt` file since
+(currently) the generic python build environment already exists on the build
+executor. **Run unit tests** ``` PYTHONPATH=.:./src coverage run -m pytest -vv
+-l coverage report ``` **build** ``` python -m build ``` **install locally
+during development** ``` pip install --editable . ``` ** check setuptools-scm
+dynamic version** ``` python -m setuptools_scm ```
```

### Comparing `iam-credential-rotation-0.1.1/discussion.md` & `iam-credential-rotation-0.2.0/discussion.md`

 * *Files identical despite different names*

### Comparing `iam-credential-rotation-0.1.1/pyproject.toml` & `iam-credential-rotation-0.2.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,31 @@
-[build-system]
-requires = ["setuptools>=67.0", "setuptools_scm[toml]>=7.1"]
-build-backend = "setuptools.build_meta"
-
 [project]
 name = "iam-credential-rotation"
-dynamic = ["version"]
+description = "automated rotation for iam machine account programmatic credentials"
+
 authors = [
   { name="Nic Cheneweth", email="nchenewe@thoughtworks.com" },
 ]
-description = "automated rotation for iam machine account programmatic credentials"
-readme = "README.md"
-requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
-[tool.setuptools_scm]
-write_to = "src/_version.py"
+dependencies = [
+  "click >= 8.1, < 9",
+]
+dynamic = ["version"]
 
 [project.urls]
-"Homepage" = "https://github.com/ThoughtWorks-DPS/iam-credential-rotatation"
-"Bug Tracker" = "https://github.com/ThoughtWorks-DPS/iam-credential-rotatation/issues"
+"Homepage" = "https://github.com/ThoughtWorks-DPS/iam-credential-rotation"
+"Bug Tracker" = "https://github.com/ThoughtWorks-DPS/iam-credential-rotation/issues"
+
+[build-system]
+requires = ["setuptools", "setuptools_scm[toml]"]
+build-backend = "setuptools.build_meta"
+
+[project.scripts]
+iam-credential-rotation = "iam_credential_rotation:cli"
+
+[tool.setuptools_scm]
+write_to = "src/_version.py"
```

### Comparing `iam-credential-rotation-0.1.1/src/iam_credential_rotation.py` & `iam-credential-rotation-0.2.0/src/iam_credential_rotation.py`

 * *Files identical despite different names*

### Comparing `iam-credential-rotation-0.1.1/src/provider_aws.py` & `iam-credential-rotation-0.2.0/src/provider_aws.py`

 * *Files identical despite different names*

### Comparing `iam-credential-rotation-0.1.1/src/utils.py` & `iam-credential-rotation-0.2.0/src/utils.py`

 * *Files identical despite different names*

### Comparing `iam-credential-rotation-0.1.1/test/test_iam_credential_rotation.py` & `iam-credential-rotation-0.2.0/test/test_iam_credential_rotation.py`

 * *Files identical despite different names*

### Comparing `iam-credential-rotation-0.1.1/test/test_provider_aws.py` & `iam-credential-rotation-0.2.0/test/test_provider_aws.py`

 * *Files identical despite different names*

### Comparing `iam-credential-rotation-0.1.1/test/test_utils.py` & `iam-credential-rotation-0.2.0/test/test_utils.py`

 * *Files identical despite different names*

