# Comparing `tmp/vault-dump-0.0.2.tar.gz` & `tmp/vault-dump-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vault-dump-0.0.2.tar", last modified: Mon Apr 24 23:31:27 2023, max compression
+gzip compressed data, was "vault-dump-0.0.4.tar", last modified: Wed Apr 26 16:00:49 2023, max compression
```

## Comparing `vault-dump-0.0.2.tar` & `vault-dump-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:31:27.200563 vault-dump-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-24 23:31:19.000000 vault-dump-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-24 23:31:27.200563 vault-dump-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-24 23:31:19.000000 vault-dump-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 23:31:27.200563 vault-dump-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-24 23:31:19.000000 vault-dump-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:31:27.200563 vault-dump-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7595 2023-04-24 23:31:19.000000 vault-dump-0.0.2/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-04-24 23:31:19.000000 vault-dump-0.0.2/tests/test_vault_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:31:27.200563 vault-dump-0.0.2/vault_dump/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 23:31:19.000000 vault-dump-0.0.2/vault_dump/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11810 2023-04-24 23:31:19.000000 vault-dump-0.0.2/vault_dump/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:31:27.200563 vault-dump-0.0.2/vault_dump.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-24 23:31:27.000000 vault-dump-0.0.2/vault_dump.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-24 23:31:27.000000 vault-dump-0.0.2/vault_dump.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 23:31:27.000000 vault-dump-0.0.2/vault_dump.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-24 23:31:27.000000 vault-dump-0.0.2/vault_dump.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-24 23:31:27.000000 vault-dump-0.0.2/vault_dump.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:00:49.674745 vault-dump-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-26 16:00:40.000000 vault-dump-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-26 16:00:49.674745 vault-dump-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-26 16:00:40.000000 vault-dump-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 16:00:49.674745 vault-dump-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-26 16:00:40.000000 vault-dump-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:00:49.674745 vault-dump-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7595 2023-04-26 16:00:40.000000 vault-dump-0.0.4/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-04-26 16:00:40.000000 vault-dump-0.0.4/tests/test_vault_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:00:49.674745 vault-dump-0.0.4/vault_dump/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 16:00:40.000000 vault-dump-0.0.4/vault_dump/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11810 2023-04-26 16:00:40.000000 vault-dump-0.0.4/vault_dump/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:00:49.674745 vault-dump-0.0.4/vault_dump.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-26 16:00:49.000000 vault-dump-0.0.4/vault_dump.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-26 16:00:49.000000 vault-dump-0.0.4/vault_dump.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 16:00:49.000000 vault-dump-0.0.4/vault_dump.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-26 16:00:49.000000 vault-dump-0.0.4/vault_dump.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-26 16:00:49.000000 vault-dump-0.0.4/vault_dump.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-26 16:00:49.000000 vault-dump-0.0.4/vault_dump.egg-info/top_level.txt
```

### Comparing `vault-dump-0.0.2/LICENSE` & `vault-dump-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vault-dump-0.0.2/PKG-INFO` & `vault-dump-0.0.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vault-dump
-Version: 0.0.2
+Version: 0.0.4
 Summary: A package to dump the configuration settings for a running hashicorp vault instance
 Home-page: https://github.com/danielpops/vault-dump
 Author: Daniel Popescu
 Author-email: danielpops@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `vault-dump-0.0.2/setup.py` & `vault-dump-0.0.4/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,20 +3,26 @@
 with open("README.md", "r") as readme_file:
     readme = readme_file.read()
 
 requirements = ["requests"]
 
 setup(
     name="vault-dump",
-    version="0.0.2",
+    version="0.0.4",
     author="Daniel Popescu",
     author_email="danielpops@gmail.com",
     description="A package to dump the configuration settings for a running hashicorp vault instance",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/danielpops/vault-dump",
     packages=find_packages(),
     install_requires=requirements,
     classifiers=[
         "Programming Language :: Python :: 3.7",
     ],
+    entry_points = {
+        "console_scripts": [
+            "vault-dump=vault_dump.main:main"
+        ]
+    },
 )
+
```

### Comparing `vault-dump-0.0.2/tests/test_main.py` & `vault-dump-0.0.4/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `vault-dump-0.0.2/tests/test_vault_integration.py` & `vault-dump-0.0.4/tests/test_vault_integration.py`

 * *Files identical despite different names*

### Comparing `vault-dump-0.0.2/vault_dump/main.py` & `vault-dump-0.0.4/vault_dump/main.py`

 * *Files identical despite different names*

### Comparing `vault-dump-0.0.2/vault_dump.egg-info/PKG-INFO` & `vault-dump-0.0.4/vault_dump.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vault-dump
-Version: 0.0.2
+Version: 0.0.4
 Summary: A package to dump the configuration settings for a running hashicorp vault instance
 Home-page: https://github.com/danielpops/vault-dump
 Author: Daniel Popescu
 Author-email: danielpops@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

