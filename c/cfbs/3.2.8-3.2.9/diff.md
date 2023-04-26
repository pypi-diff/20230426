# Comparing `tmp/cfbs-3.2.8.tar.gz` & `tmp/cfbs-3.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfbs-3.2.8.tar", last modified: Thu Jan 12 13:47:55 2023, max compression
+gzip compressed data, was "cfbs-3.2.9.tar", last modified: Fri Mar 17 15:11:57 2023, max compression
```

## Comparing `cfbs-3.2.8.tar` & `cfbs-3.2.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-12 13:47:55.172213 cfbs-3.2.8/
--rw-r--r--   0 runner    (1001) docker     (122)     1070 2023-01-12 13:47:43.000000 cfbs-3.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    11667 2023-01-12 13:47:55.172213 cfbs-3.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    11218 2023-01-12 13:47:43.000000 cfbs-3.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-12 13:47:55.168213 cfbs-3.2.8/cfbs/
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-01-12 13:47:54.000000 cfbs-3.2.8/cfbs/VERSION
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-12 13:47:43.000000 cfbs-3.2.8/cfbs/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)      288 2023-01-12 13:47:43.000000 cfbs-3.2.8/cfbs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2442 2023-01-12 13:47:43.000000 cfbs-3.2.8/cfbs/args.py
--rw-r--r--   0 runner    (1001) docker     (122)     8156 2023-01-12 13:47:43.000000 cfbs-3.2.8/cfbs/build.py
--rw-r--r--   0 runner    (1001) docker     (122)    17388 2023-01-12 13:47:43.000000 cfbs-3.2.8/cfbs/cfbs_config.py
--rw-r--r--   0 runner    (1001) docker     (122)     3268 2023-01-12 13:47:43.000000 cfbs-3.2.8/cfbs/cfbs_json.py
--rw-r--r--   0 runner    (1001) docker     (122)    39883 2023-01-12 13:47:43.000000 cfbs-3.2.8/cfbs/commands.py
--rw-r--r--   0 runner    (1001) docker     (122)     5442 2023-01-12 13:47:43.000000 cfbs-3.2.8/cfbs/git.py
--rw-r--r--   0 runner    (1001) docker     (122)     4090 2023-01-12 13:47:43.000000 cfbs-3.2.8/cfbs/git_magic.py
--rw-r--r--   0 runner    (1001) docker     (122)     5451 2023-01-12 13:47:43.000000 cfbs-3.2.8/cfbs/index.py
--rw-r--r--   0 runner    (1001) docker     (122)     9100 2023-01-12 13:47:43.000000 cfbs-3.2.8/cfbs/internal_file_management.py
--rw-r--r--   0 runner    (1001) docker     (122)     5022 2023-01-12 13:47:43.000000 cfbs-3.2.8/cfbs/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     1992 2023-01-12 13:47:43.000000 cfbs-3.2.8/cfbs/module.py
--rw-r--r--   0 runner    (1001) docker     (122)     6843 2023-01-12 13:47:43.000000 cfbs-3.2.8/cfbs/pretty.py
--rw-r--r--   0 runner    (1001) docker     (122)     1300 2023-01-12 13:47:43.000000 cfbs-3.2.8/cfbs/prompts.py
--rw-r--r--   0 runner    (1001) docker     (122)      136 2023-01-12 13:47:43.000000 cfbs-3.2.8/cfbs/result.py
--rw-r--r--   0 runner    (1001) docker     (122)     8164 2023-01-12 13:47:43.000000 cfbs-3.2.8/cfbs/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     7103 2023-01-12 13:47:43.000000 cfbs-3.2.8/cfbs/validate.py
--rw-r--r--   0 runner    (1001) docker     (122)      279 2023-01-12 13:47:43.000000 cfbs-3.2.8/cfbs/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-12 13:47:55.168213 cfbs-3.2.8/cfbs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    11667 2023-01-12 13:47:55.000000 cfbs-3.2.8/cfbs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      632 2023-01-12 13:47:55.000000 cfbs-3.2.8/cfbs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-12 13:47:55.000000 cfbs-3.2.8/cfbs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       40 2023-01-12 13:47:55.000000 cfbs-3.2.8/cfbs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-01-12 13:47:55.000000 cfbs-3.2.8/cfbs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-01-12 13:47:55.172213 cfbs-3.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1562 2023-01-12 13:47:43.000000 cfbs-3.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-12 13:47:55.172213 cfbs-3.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-12 13:47:43.000000 cfbs-3.2.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      208 2023-01-12 13:47:43.000000 cfbs-3.2.8/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)      255 2023-01-12 13:47:43.000000 cfbs-3.2.8/tests/test_git.py
--rw-r--r--   0 runner    (1001) docker     (122)     5232 2023-01-12 13:47:43.000000 cfbs-3.2.8/tests/test_input.py
--rw-r--r--   0 runner    (1001) docker     (122)     2266 2023-01-12 13:47:43.000000 cfbs-3.2.8/tests/test_module.py
--rw-r--r--   0 runner    (1001) docker     (122)     9260 2023-01-12 13:47:43.000000 cfbs-3.2.8/tests/test_pretty.py
--rw-r--r--   0 runner    (1001) docker     (122)     2485 2023-01-12 13:47:43.000000 cfbs-3.2.8/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 15:11:57.467695 cfbs-3.2.9/
+-rw-r--r--   0 runner    (1001) docker     (122)     1070 2023-03-17 15:11:46.000000 cfbs-3.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    11667 2023-03-17 15:11:57.467695 cfbs-3.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    11218 2023-03-17 15:11:46.000000 cfbs-3.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 15:11:57.467695 cfbs-3.2.9/cfbs/
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-03-17 15:11:57.000000 cfbs-3.2.9/cfbs/VERSION
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-17 15:11:46.000000 cfbs-3.2.9/cfbs/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)      288 2023-03-17 15:11:46.000000 cfbs-3.2.9/cfbs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2442 2023-03-17 15:11:46.000000 cfbs-3.2.9/cfbs/args.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8156 2023-03-17 15:11:46.000000 cfbs-3.2.9/cfbs/build.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17388 2023-03-17 15:11:46.000000 cfbs-3.2.9/cfbs/cfbs_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3268 2023-03-17 15:11:46.000000 cfbs-3.2.9/cfbs/cfbs_json.py
+-rw-r--r--   0 runner    (1001) docker     (122)    39994 2023-03-17 15:11:46.000000 cfbs-3.2.9/cfbs/commands.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5442 2023-03-17 15:11:46.000000 cfbs-3.2.9/cfbs/git.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4090 2023-03-17 15:11:46.000000 cfbs-3.2.9/cfbs/git_magic.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5451 2023-03-17 15:11:46.000000 cfbs-3.2.9/cfbs/index.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9100 2023-03-17 15:11:46.000000 cfbs-3.2.9/cfbs/internal_file_management.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5022 2023-03-17 15:11:46.000000 cfbs-3.2.9/cfbs/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1992 2023-03-17 15:11:46.000000 cfbs-3.2.9/cfbs/module.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6843 2023-03-17 15:11:46.000000 cfbs-3.2.9/cfbs/pretty.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1300 2023-03-17 15:11:46.000000 cfbs-3.2.9/cfbs/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (122)      136 2023-03-17 15:11:46.000000 cfbs-3.2.9/cfbs/result.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8164 2023-03-17 15:11:46.000000 cfbs-3.2.9/cfbs/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7103 2023-03-17 15:11:46.000000 cfbs-3.2.9/cfbs/validate.py
+-rw-r--r--   0 runner    (1001) docker     (122)      279 2023-03-17 15:11:46.000000 cfbs-3.2.9/cfbs/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 15:11:57.467695 cfbs-3.2.9/cfbs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    11667 2023-03-17 15:11:57.000000 cfbs-3.2.9/cfbs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      632 2023-03-17 15:11:57.000000 cfbs-3.2.9/cfbs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-17 15:11:57.000000 cfbs-3.2.9/cfbs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       40 2023-03-17 15:11:57.000000 cfbs-3.2.9/cfbs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-03-17 15:11:57.000000 cfbs-3.2.9/cfbs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-17 15:11:57.467695 cfbs-3.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1562 2023-03-17 15:11:46.000000 cfbs-3.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 15:11:57.467695 cfbs-3.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-17 15:11:46.000000 cfbs-3.2.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      208 2023-03-17 15:11:46.000000 cfbs-3.2.9/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)      255 2023-03-17 15:11:46.000000 cfbs-3.2.9/tests/test_git.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5232 2023-03-17 15:11:46.000000 cfbs-3.2.9/tests/test_input.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2266 2023-03-17 15:11:46.000000 cfbs-3.2.9/tests/test_module.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9260 2023-03-17 15:11:46.000000 cfbs-3.2.9/tests/test_pretty.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2485 2023-03-17 15:11:46.000000 cfbs-3.2.9/tests/test_utils.py
```

### Comparing `cfbs-3.2.8/LICENSE` & `cfbs-3.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cfbs-3.2.8/PKG-INFO` & `cfbs-3.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfbs
-Version: 3.2.8
+Version: 3.2.9
 Summary: Tooling to build, manage and deploy CFEngine policy
 Home-page: https://github.com/cfengine/cfbs
 Author: Northern.tech, Inc.
 Author-email: contact@northern.tech
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cfbs-3.2.8/README.md` & `cfbs-3.2.9/README.md`

 * *Files identical despite different names*

### Comparing `cfbs-3.2.8/cfbs/args.py` & `cfbs-3.2.9/cfbs/args.py`

 * *Files identical despite different names*

### Comparing `cfbs-3.2.8/cfbs/build.py` & `cfbs-3.2.9/cfbs/build.py`

 * *Files identical despite different names*

### Comparing `cfbs-3.2.8/cfbs/cfbs_config.py` & `cfbs-3.2.9/cfbs/cfbs_config.py`

 * *Files identical despite different names*

### Comparing `cfbs-3.2.8/cfbs/cfbs_json.py` & `cfbs-3.2.9/cfbs/cfbs_json.py`

 * *Files identical despite different names*

### Comparing `cfbs-3.2.8/cfbs/commands.py` & `cfbs-3.2.9/cfbs/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -790,15 +790,19 @@
 
     if new_deps:
         objects = [index.get_module_object(d, new_deps_added_by[d]) for d in new_deps]
         config.add_with_dependencies(objects)
     config.save()
 
     if changes_made:
-        msg = "Updated %d module%s\n" % (len(updated), "s" if updated else "") + msg
+        if len(updated) > 1:
+            msg = "Updated %d modules\n" % len(updated) + msg
+        else:
+            # Remove the '\n - ' part of the message
+            msg = msg[len("\n - ") :]
         print("%s\n" % msg)
     else:
         print("Modules are already up to date")
 
     return Result(0, changes_made, msg, files)
```

### Comparing `cfbs-3.2.8/cfbs/git.py` & `cfbs-3.2.9/cfbs/git.py`

 * *Files identical despite different names*

### Comparing `cfbs-3.2.8/cfbs/git_magic.py` & `cfbs-3.2.9/cfbs/git_magic.py`

 * *Files identical despite different names*

### Comparing `cfbs-3.2.8/cfbs/index.py` & `cfbs-3.2.9/cfbs/index.py`

 * *Files identical despite different names*

### Comparing `cfbs-3.2.8/cfbs/internal_file_management.py` & `cfbs-3.2.9/cfbs/internal_file_management.py`

 * *Files identical despite different names*

### Comparing `cfbs-3.2.8/cfbs/main.py` & `cfbs-3.2.9/cfbs/main.py`

 * *Files identical despite different names*

### Comparing `cfbs-3.2.8/cfbs/module.py` & `cfbs-3.2.9/cfbs/module.py`

 * *Files identical despite different names*

### Comparing `cfbs-3.2.8/cfbs/pretty.py` & `cfbs-3.2.9/cfbs/pretty.py`

 * *Files identical despite different names*

### Comparing `cfbs-3.2.8/cfbs/prompts.py` & `cfbs-3.2.9/cfbs/prompts.py`

 * *Files identical despite different names*

### Comparing `cfbs-3.2.8/cfbs/utils.py` & `cfbs-3.2.9/cfbs/utils.py`

 * *Files identical despite different names*

### Comparing `cfbs-3.2.8/cfbs/validate.py` & `cfbs-3.2.9/cfbs/validate.py`

 * *Files identical despite different names*

### Comparing `cfbs-3.2.8/cfbs.egg-info/PKG-INFO` & `cfbs-3.2.9/cfbs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfbs
-Version: 3.2.8
+Version: 3.2.9
 Summary: Tooling to build, manage and deploy CFEngine policy
 Home-page: https://github.com/cfengine/cfbs
 Author: Northern.tech, Inc.
 Author-email: contact@northern.tech
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cfbs-3.2.8/cfbs.egg-info/SOURCES.txt` & `cfbs-3.2.9/cfbs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cfbs-3.2.8/setup.py` & `cfbs-3.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `cfbs-3.2.8/tests/test_input.py` & `cfbs-3.2.9/tests/test_input.py`

 * *Files identical despite different names*

### Comparing `cfbs-3.2.8/tests/test_module.py` & `cfbs-3.2.9/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `cfbs-3.2.8/tests/test_pretty.py` & `cfbs-3.2.9/tests/test_pretty.py`

 * *Files identical despite different names*

### Comparing `cfbs-3.2.8/tests/test_utils.py` & `cfbs-3.2.9/tests/test_utils.py`

 * *Files identical despite different names*

