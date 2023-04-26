# Comparing `tmp/kaslcred-0.1.1.tar.gz` & `tmp/kaslcred-0.1.2.tar.gz`

## Comparing `kaslcred-0.1.1.tar` & `kaslcred-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 kaslcred-0.1.1/.DS_Store
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaslcred-0.1.1/.projectile
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 kaslcred-0.1.1/Dockerfile
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 kaslcred-0.1.1/Makefile
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 kaslcred-0.1.1/requirements.txt
--rw-r--r--   0        0        0     5409 2020-02-02 00:00:00.000000 kaslcred-0.1.1/sample_schemas/hello-acdc-chain-schema.json
--rw-r--r--   0        0        0     6074 2020-02-02 00:00:00.000000 kaslcred-0.1.1/sample_schemas/hello-admit-schema.json
--rw-r--r--   0        0        0     6370 2020-02-02 00:00:00.000000 kaslcred-0.1.1/sample_schemas/hello-attend-schema.json
--rw-r--r--   0        0        0     4247 2020-02-02 00:00:00.000000 kaslcred-0.1.1/sample_schemas/hello-keri-schema.json
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 kaslcred-0.1.1/sample_schemas/single-schema-map.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaslcred-0.1.1/src/kaslcred/__init__.py
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 kaslcred-0.1.1/src/kaslcred/__main__.py
--rw-r--r--   0        0        0    11484 2020-02-02 00:00:00.000000 kaslcred-0.1.1/src/kaslcred/link.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 kaslcred-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 kaslcred-0.1.1/tests/test_link.py
--rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 kaslcred-0.1.1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 kaslcred-0.1.1/LICENSE
--rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 kaslcred-0.1.1/README.md
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 kaslcred-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 kaslcred-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 kaslcred-0.1.2/.DS_Store
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaslcred-0.1.2/.projectile
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 kaslcred-0.1.2/Dockerfile
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 kaslcred-0.1.2/Makefile
+-rw-r--r--   0        0        0    40144 2020-02-02 00:00:00.000000 kaslcred-0.1.2/Pipfile.lock
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 kaslcred-0.1.2/requirements.txt
+-rw-r--r--   0        0        0     5409 2020-02-02 00:00:00.000000 kaslcred-0.1.2/sample_schemas/hello-acdc-chain-schema.json
+-rw-r--r--   0        0        0     6074 2020-02-02 00:00:00.000000 kaslcred-0.1.2/sample_schemas/hello-admit-schema.json
+-rw-r--r--   0        0        0     6370 2020-02-02 00:00:00.000000 kaslcred-0.1.2/sample_schemas/hello-attend-schema.json
+-rw-r--r--   0        0        0     4247 2020-02-02 00:00:00.000000 kaslcred-0.1.2/sample_schemas/hello-keri-schema.json
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 kaslcred-0.1.2/sample_schemas/single-schema-map.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaslcred-0.1.2/src/kaslcred/__init__.py
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 kaslcred-0.1.2/src/kaslcred/__main__.py
+-rw-r--r--   0        0        0    11484 2020-02-02 00:00:00.000000 kaslcred-0.1.2/src/kaslcred/link.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 kaslcred-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 kaslcred-0.1.2/tests/test_link.py
+-rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 kaslcred-0.1.2/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 kaslcred-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 kaslcred-0.1.2/README.md
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 kaslcred-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 kaslcred-0.1.2/PKG-INFO
```

### Comparing `kaslcred-0.1.1/.DS_Store` & `kaslcred-0.1.2/.DS_Store`

 * *Files identical despite different names*

### Comparing `kaslcred-0.1.1/Dockerfile` & `kaslcred-0.1.2/Dockerfile`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-FROM python:3.11.2-buster
+FROM python:3.10-buster
 
 ARG DEBIAN_FRONTEND=noninteractive
 
 RUN apt-get update && apt-get dist-upgrade -y
 
 # Install dependencies and required tools
 RUN apt-get install -y \
```

### Comparing `kaslcred-0.1.1/sample_schemas/hello-acdc-chain-schema.json` & `kaslcred-0.1.2/sample_schemas/hello-acdc-chain-schema.json`

 * *Files identical despite different names*

### Comparing `kaslcred-0.1.1/sample_schemas/hello-admit-schema.json` & `kaslcred-0.1.2/sample_schemas/hello-admit-schema.json`

 * *Files identical despite different names*

### Comparing `kaslcred-0.1.1/sample_schemas/hello-attend-schema.json` & `kaslcred-0.1.2/sample_schemas/hello-attend-schema.json`

 * *Files identical despite different names*

### Comparing `kaslcred-0.1.1/sample_schemas/hello-keri-schema.json` & `kaslcred-0.1.2/sample_schemas/hello-keri-schema.json`

 * *Files identical despite different names*

### Comparing `kaslcred-0.1.1/src/kaslcred/link.py` & `kaslcred-0.1.2/src/kaslcred/link.py`

 * *Files identical despite different names*

### Comparing `kaslcred-0.1.1/tests/test_link.py` & `kaslcred-0.1.2/tests/test_link.py`

 * *Files identical despite different names*

### Comparing `kaslcred-0.1.1/.gitignore` & `kaslcred-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `kaslcred-0.1.1/LICENSE` & `kaslcred-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kaslcred-0.1.1/README.md` & `kaslcred-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `kaslcred-0.1.1/pyproject.toml` & `kaslcred-0.1.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "kaslcred"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
     {name="Kent Bull", email="kent@tetraveda.com"},
     {name="Kevin Griffin", email="griffin.kev@gmail.com"}
 ]
 description = "A credential schema linker for the KERI and ACDC ecosystem."
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `kaslcred-0.1.1/PKG-INFO` & `kaslcred-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaslcred
-Version: 0.1.1
+Version: 0.1.2
 Summary: A credential schema linker for the KERI and ACDC ecosystem.
 Project-URL: Homepage, https://github.com/tetraveda/kaslcred
 Author-email: Kent Bull <kent@tetraveda.com>, Kevin Griffin <griffin.kev@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

