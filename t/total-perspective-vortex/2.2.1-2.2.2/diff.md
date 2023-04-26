# Comparing `tmp/total-perspective-vortex-2.2.1.tar.gz` & `tmp/total-perspective-vortex-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "total-perspective-vortex-2.2.1.tar", last modified: Thu Mar 30 10:53:20 2023, max compression
+gzip compressed data, was "total-perspective-vortex-2.2.2.tar", last modified: Tue Apr 25 14:42:11 2023, max compression
```

## Comparing `total-perspective-vortex-2.2.1.tar` & `total-perspective-vortex-2.2.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:53:20.542865 total-perspective-vortex-2.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-03-30 10:53:09.000000 total-perspective-vortex-2.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-03-30 10:53:20.542865 total-perspective-vortex-2.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-03-30 10:53:09.000000 total-perspective-vortex-2.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-03-30 10:53:20.542865 total-perspective-vortex-2.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-03-30 10:53:09.000000 total-perspective-vortex-2.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:53:20.534865 total-perspective-vortex-2.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:53:09.000000 total-perspective-vortex-2.2.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-03-30 10:53:09.000000 total-perspective-vortex-2.2.1/tests/test_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-03-30 10:53:09.000000 total-perspective-vortex-2.2.1/tests/test_mapper_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-03-30 10:53:09.000000 total-perspective-vortex-2.2.1/tests/test_mapper_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    10683 2023-03-30 10:53:09.000000 total-perspective-vortex-2.2.1/tests/test_mapper_destinations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-03-30 10:53:09.000000 total-perspective-vortex-2.2.1/tests/test_mapper_inheritance.py
--rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-03-30 10:53:09.000000 total-perspective-vortex-2.2.1/tests/test_mapper_merge_multiple.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-03-30 10:53:09.000000 total-perspective-vortex-2.2.1/tests/test_mapper_params_specific.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-03-30 10:53:09.000000 total-perspective-vortex-2.2.1/tests/test_mapper_rank.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-03-30 10:53:09.000000 total-perspective-vortex-2.2.1/tests/test_mapper_resubmit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-03-30 10:53:09.000000 total-perspective-vortex-2.2.1/tests/test_mapper_role.py
--rw-r--r--   0 runner    (1001) docker     (123)    11792 2023-03-30 10:53:09.000000 total-perspective-vortex-2.2.1/tests/test_mapper_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-03-30 10:53:09.000000 total-perspective-vortex-2.2.1/tests/test_mapper_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-03-30 10:53:09.000000 total-perspective-vortex-2.2.1/tests/test_mapper_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    14778 2023-03-30 10:53:09.000000 total-perspective-vortex-2.2.1/tests/test_scenarios.py
--rw-r--r--   0 runner    (1001) docker     (123)    15754 2023-03-30 10:53:09.000000 total-perspective-vortex-2.2.1/tests/test_shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:53:20.538865 total-perspective-vortex-2.2.1/total_perspective_vortex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-03-30 10:53:20.000000 total-perspective-vortex-2.2.1/total_perspective_vortex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-03-30 10:53:20.000000 total-perspective-vortex-2.2.1/total_perspective_vortex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 10:53:20.000000 total-perspective-vortex-2.2.1/total_perspective_vortex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-30 10:53:20.000000 total-perspective-vortex-2.2.1/total_perspective_vortex.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-03-30 10:53:20.000000 total-perspective-vortex-2.2.1/total_perspective_vortex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-30 10:53:20.000000 total-perspective-vortex-2.2.1/total_perspective_vortex.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:53:20.538865 total-perspective-vortex-2.2.1/tpv/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-03-30 10:53:09.000000 total-perspective-vortex-2.2.1/tpv/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:53:20.538865 total-perspective-vortex-2.2.1/tpv/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:53:09.000000 total-perspective-vortex-2.2.1/tpv/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-03-30 10:53:09.000000 total-perspective-vortex-2.2.1/tpv/commands/dryrunner.py
--rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-03-30 10:53:09.000000 total-perspective-vortex-2.2.1/tpv/commands/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-03-30 10:53:09.000000 total-perspective-vortex-2.2.1/tpv/commands/linter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-03-30 10:53:09.000000 total-perspective-vortex-2.2.1/tpv/commands/shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:53:20.538865 total-perspective-vortex-2.2.1/tpv/commands/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:53:09.000000 total-perspective-vortex-2.2.1/tpv/commands/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-03-30 10:53:09.000000 total-perspective-vortex-2.2.1/tpv/commands/test/mock_galaxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:53:20.542865 total-perspective-vortex-2.2.1/tpv/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:53:09.000000 total-perspective-vortex-2.2.1/tpv/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34869 2023-03-30 10:53:09.000000 total-perspective-vortex-2.2.1/tpv/core/entities.py
--rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-03-30 10:53:09.000000 total-perspective-vortex-2.2.1/tpv/core/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-03-30 10:53:09.000000 total-perspective-vortex-2.2.1/tpv/core/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6916 2023-03-30 10:53:09.000000 total-perspective-vortex-2.2.1/tpv/core/mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-03-30 10:53:09.000000 total-perspective-vortex-2.2.1/tpv/core/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:53:20.542865 total-perspective-vortex-2.2.1/tpv/rules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:53:09.000000 total-perspective-vortex-2.2.1/tpv/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-03-30 10:53:09.000000 total-perspective-vortex-2.2.1/tpv/rules/gateway.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:42:11.209328 total-perspective-vortex-2.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-25 14:41:57.000000 total-perspective-vortex-2.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-04-25 14:42:11.209328 total-perspective-vortex-2.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-04-25 14:41:57.000000 total-perspective-vortex-2.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-25 14:42:11.209328 total-perspective-vortex-2.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-04-25 14:41:57.000000 total-perspective-vortex-2.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:42:11.205328 total-perspective-vortex-2.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:41:57.000000 total-perspective-vortex-2.2.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-25 14:41:57.000000 total-perspective-vortex-2.2.2/tests/test_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-04-25 14:41:57.000000 total-perspective-vortex-2.2.2/tests/test_mapper_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-04-25 14:41:57.000000 total-perspective-vortex-2.2.2/tests/test_mapper_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11240 2023-04-25 14:41:57.000000 total-perspective-vortex-2.2.2/tests/test_mapper_destinations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-04-25 14:41:57.000000 total-perspective-vortex-2.2.2/tests/test_mapper_inheritance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-04-25 14:41:57.000000 total-perspective-vortex-2.2.2/tests/test_mapper_merge_multiple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-04-25 14:41:57.000000 total-perspective-vortex-2.2.2/tests/test_mapper_params_specific.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-04-25 14:41:57.000000 total-perspective-vortex-2.2.2/tests/test_mapper_rank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-04-25 14:41:57.000000 total-perspective-vortex-2.2.2/tests/test_mapper_resubmit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-04-25 14:41:57.000000 total-perspective-vortex-2.2.2/tests/test_mapper_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13750 2023-04-25 14:41:57.000000 total-perspective-vortex-2.2.2/tests/test_mapper_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-25 14:41:57.000000 total-perspective-vortex-2.2.2/tests/test_mapper_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-04-25 14:41:57.000000 total-perspective-vortex-2.2.2/tests/test_mapper_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14778 2023-04-25 14:41:57.000000 total-perspective-vortex-2.2.2/tests/test_scenarios.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15774 2023-04-25 14:41:57.000000 total-perspective-vortex-2.2.2/tests/test_shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:42:11.205328 total-perspective-vortex-2.2.2/total_perspective_vortex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-04-25 14:42:11.000000 total-perspective-vortex-2.2.2/total_perspective_vortex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-25 14:42:11.000000 total-perspective-vortex-2.2.2/total_perspective_vortex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 14:42:11.000000 total-perspective-vortex-2.2.2/total_perspective_vortex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-25 14:42:11.000000 total-perspective-vortex-2.2.2/total_perspective_vortex.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-25 14:42:11.000000 total-perspective-vortex-2.2.2/total_perspective_vortex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-25 14:42:11.000000 total-perspective-vortex-2.2.2/total_perspective_vortex.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:42:11.205328 total-perspective-vortex-2.2.2/tpv/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-25 14:41:57.000000 total-perspective-vortex-2.2.2/tpv/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:42:11.205328 total-perspective-vortex-2.2.2/tpv/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:41:57.000000 total-perspective-vortex-2.2.2/tpv/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-25 14:41:57.000000 total-perspective-vortex-2.2.2/tpv/commands/dryrunner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-25 14:41:57.000000 total-perspective-vortex-2.2.2/tpv/commands/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-04-25 14:41:57.000000 total-perspective-vortex-2.2.2/tpv/commands/linter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-04-25 14:41:57.000000 total-perspective-vortex-2.2.2/tpv/commands/shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:42:11.205328 total-perspective-vortex-2.2.2/tpv/commands/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:41:57.000000 total-perspective-vortex-2.2.2/tpv/commands/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-04-25 14:41:57.000000 total-perspective-vortex-2.2.2/tpv/commands/test/mock_galaxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:42:11.209328 total-perspective-vortex-2.2.2/tpv/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:41:57.000000 total-perspective-vortex-2.2.2/tpv/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34887 2023-04-25 14:41:57.000000 total-perspective-vortex-2.2.2/tpv/core/entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-04-25 14:41:57.000000 total-perspective-vortex-2.2.2/tpv/core/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-04-25 14:41:57.000000 total-perspective-vortex-2.2.2/tpv/core/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6916 2023-04-25 14:41:57.000000 total-perspective-vortex-2.2.2/tpv/core/mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-25 14:41:57.000000 total-perspective-vortex-2.2.2/tpv/core/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:42:11.209328 total-perspective-vortex-2.2.2/tpv/rules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:41:57.000000 total-perspective-vortex-2.2.2/tpv/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-04-25 14:41:57.000000 total-perspective-vortex-2.2.2/tpv/rules/gateway.py
```

### Comparing `total-perspective-vortex-2.2.1/LICENSE` & `total-perspective-vortex-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.1/PKG-INFO` & `total-perspective-vortex-2.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: total-perspective-vortex
-Version: 2.2.1
+Version: 2.2.2
 Summary: A library for routing entities (jobs, users or groups) to destinations in Galaxy
 Home-page: https://github.com/galaxyproject/total-perspective-vortex
 Author: Galaxy and GVL projects
 Author-email: help@genome.edu.au
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
```

### Comparing `total-perspective-vortex-2.2.1/README.md` & `total-perspective-vortex-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.1/setup.py` & `total-perspective-vortex-2.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.1/tests/test_entity.py` & `total-perspective-vortex-2.2.2/tests/test_entity.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.1/tests/test_mapper_basic.py` & `total-perspective-vortex-2.2.2/tests/test_mapper_basic.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.1/tests/test_mapper_context.py` & `total-perspective-vortex-2.2.2/tests/test_mapper_context.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.1/tests/test_mapper_destinations.py` & `total-perspective-vortex-2.2.2/tests/test_mapper_destinations.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,7 +172,17 @@
         destination = self._map_to_destination(tool, user, datasets, tpv_config_paths=[config])
         self.assertEqual(destination.id, "destination_without_min_mem_accepted")
 
         # second tool should match the min requirements for the destination
         tool = mock_galaxy.Tool('tool_for_testing_min_mem_acceptance_match')
         destination = self._map_to_destination(tool, user, datasets, tpv_config_paths=[config])
         self.assertEqual(destination.id, "destination_with_min_mem_accepted")
+
+    def test_user_map_to_destination_accepting_offline(self):
+        user = mock_galaxy.User('albo', 'pulsar_canberra_user@act.au')
+
+        config = os.path.join(os.path.dirname(__file__), 'fixtures/mapping-destinations.yml')
+
+        tool = mock_galaxy.Tool('toolshed_hifiasm')
+        datasets = [mock_galaxy.DatasetAssociation("test", mock_galaxy.Dataset("test.txt", file_size=12 * 1024 ** 3))]
+        destination = self._map_to_destination(tool, user, datasets, tpv_config_paths=[config])
+        self.assertEqual(destination.id, "pulsar-canberra")
```

### Comparing `total-perspective-vortex-2.2.1/tests/test_mapper_inheritance.py` & `total-perspective-vortex-2.2.2/tests/test_mapper_inheritance.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.1/tests/test_mapper_merge_multiple.py` & `total-perspective-vortex-2.2.2/tests/test_mapper_merge_multiple.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.1/tests/test_mapper_params_specific.py` & `total-perspective-vortex-2.2.2/tests/test_mapper_params_specific.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.1/tests/test_mapper_rank.py` & `total-perspective-vortex-2.2.2/tests/test_mapper_rank.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.1/tests/test_mapper_resubmit.py` & `total-perspective-vortex-2.2.2/tests/test_mapper_resubmit.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.1/tests/test_mapper_role.py` & `total-perspective-vortex-2.2.2/tests/test_mapper_role.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.1/tests/test_mapper_rules.py` & `total-perspective-vortex-2.2.2/tests/test_mapper_rules.py`

 * *Files 24% similar despite different names*

```diff
@@ -222,7 +222,46 @@
         create_job(app, user_eccentrica, tool_total_limit_3)
         create_job(app, user_eccentrica, tool_total_limit_3)
 
         # roosta cannot create another repenrich job
         with self.assertRaises(JobNotReadyException):
             tpv_config = os.path.join(os.path.dirname(__file__), 'fixtures/mapping-rule-tool-limits.yml')
             self._map_to_destination(tool_total_limit_3, user_roosta, datasets, tpv_config_files=[tpv_config], app=app)
+
+    def test_tool_version_comparison_helpers(self):
+        tpv_config = os.path.join(os.path.dirname(__file__), 'fixtures/mapping-rule-tool-limits.yml')
+        user = mock_galaxy.User('ford', 'prefect@vortex.org')
+        datasets = [mock_galaxy.DatasetAssociation("test", mock_galaxy.Dataset("test.txt", file_size=1*1024**3))]
+
+        def mock_trinity_with_version(version):
+            return mock_galaxy.Tool(
+                id=f'toolshed.g2.bx.psu.edu/repos/iuc/trinity/trinity/{version}',
+                version=version
+            )
+
+        env_keys = [ # env keys that may be added by cooked trinity rules
+            'version_gte_2.15.1+galaxy0',
+            'version_gt_2.15.1+galaxy0',
+            'version_lt_2.10.1+galaxy7',
+            'version_lte_2.10.1+galaxy7',
+        ]
+        # trinity version 3.15.1+galaxy0
+        tool = mock_trinity_with_version('3.15.1+galaxy0')
+        destination = self._map_to_destination(tool, user, datasets, tpv_config_files=[tpv_config])
+        self.assertCountEqual(
+            [e.get('name') for e in destination.env if e.get('name') in env_keys],
+            ['version_gte_2.15.1+galaxy0', 'version_gt_2.15.1+galaxy0'],
+        )
+        # trinity version 2.15.1+galaxy0
+        tool = mock_trinity_with_version('2.15.1+galaxy0')
+        destination = self._map_to_destination(tool, user, datasets, tpv_config_files=[tpv_config])
+        self.assertCountEqual(
+            [e.get('name') for e in destination.env if e.get('name') in env_keys],
+            ['version_gte_2.15.1+galaxy0'],
+        )
+        # trinity version 2.10.1+galaxy6
+        tool = mock_trinity_with_version('2.10.1+galaxy6')
+        destination = self._map_to_destination(tool, user, datasets, tpv_config_files=[tpv_config])
+        self.assertCountEqual(
+            [e.get('name') for e in destination.env if e.get('name') in env_keys],
+            ['version_lt_2.10.1+galaxy7', 'version_lte_2.10.1+galaxy7'],
+        )
```

### Comparing `total-perspective-vortex-2.2.1/tests/test_mapper_sample.py` & `total-perspective-vortex-2.2.2/tests/test_mapper_sample.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.1/tests/test_mapper_user.py` & `total-perspective-vortex-2.2.2/tests/test_mapper_user.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.1/tests/test_scenarios.py` & `total-perspective-vortex-2.2.2/tests/test_scenarios.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.1/tests/test_shell.py` & `total-perspective-vortex-2.2.2/tests/test_shell.py`

 * *Files 1% similar despite different names*

```diff
@@ -281,11 +281,11 @@
             self.call_shell_command(
                 "tpv", "dry-run", "--job-conf", job_config, "--tool", "bwa", "--input-size", "20", tpv_config)
 
     def test_dry_run_user_email(self):
         job_config = os.path.join(os.path.dirname(__file__), 'fixtures/job_conf_dry_run.yml')
         tpv_config = os.path.join(os.path.dirname(__file__), 'fixtures/mapping-rules.yml')
         output = self.call_shell_command(
-            "tpv", "dry-run", "--job-conf", job_config, "--input-size", "6", "--user", "fairycake@vortex.org",
+            "tpv", "dry-run", "--job-conf", job_config, "--input-size", "6", "--user", "krikkitrobot@planetkrikkit.org",
             tpv_config)
-        self.assertTrue("name: TEST_JOB_SLOTS" in output,
-                        f"Expected 'name: TEST_JOB_SLOTS' in destination\n{output}")
+        self.assertTrue("name: TEST_JOB_SLOTS_USER" in output,
+                        f"Expected 'name: TEST_JOB_SLOTS_USER' in destination\n{output}")
```

### Comparing `total-perspective-vortex-2.2.1/total_perspective_vortex.egg-info/PKG-INFO` & `total-perspective-vortex-2.2.2/total_perspective_vortex.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: total-perspective-vortex
-Version: 2.2.1
+Version: 2.2.2
 Summary: A library for routing entities (jobs, users or groups) to destinations in Galaxy
 Home-page: https://github.com/galaxyproject/total-perspective-vortex
 Author: Galaxy and GVL projects
 Author-email: help@genome.edu.au
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
```

### Comparing `total-perspective-vortex-2.2.1/total_perspective_vortex.egg-info/SOURCES.txt` & `total-perspective-vortex-2.2.2/total_perspective_vortex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.1/tpv/commands/dryrunner.py` & `total-perspective-vortex-2.2.2/tpv/commands/dryrunner.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,19 +19,16 @@
         gateway.ACTIVE_DESTINATION_MAPPER = None
         return gateway.map_tool_to_destination(self.galaxy_app, self.job, self.tool, self.user,
                                                tpv_config_files=self.tpv_config_files)
 
     @staticmethod
     def from_params(job_conf, user=None, tool=None, tpv_confs=None, input_size=None):
         if user is not None:
-            if '@' in user:
-                username, email = user.split('@', 1)
-            else:
-                username, email = (user, 'example.org')
-            user = mock_galaxy.User(username, email)
+            email = user
+            user = mock_galaxy.User('gargravarr', email)
         else:
             user = None
 
         if tool:
             tool = mock_galaxy.Tool(tool)
         else:
             tool = None
```

### Comparing `total-perspective-vortex-2.2.1/tpv/commands/formatter.py` & `total-perspective-vortex-2.2.2/tpv/commands/formatter.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,14 +76,15 @@
             return dict_to_sort
 
     def format(self):
         default_inherits = self.yaml_dict.get('global', {}).get('default_inherits') or 'default'
 
         basic_entity_sort_order = {
             'id': {},
+            'inherits': {},
             'if': {},
             'context': {},
             'gpus': {},
             'cores': {},
             'mem': {},
             'env': {
                 '*': {}
```

### Comparing `total-perspective-vortex-2.2.1/tpv/commands/linter.py` & `total-perspective-vortex-2.2.2/tpv/commands/linter.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.1/tpv/commands/shell.py` & `total-perspective-vortex-2.2.2/tpv/commands/shell.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.1/tpv/commands/test/mock_galaxy.py` & `total-perspective-vortex-2.2.2/tpv/commands/test/mock_galaxy.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,17 +40,18 @@
         self.counter += 1
         self.file_name = file_name
         self.file_size = file_size
 
 
 # Tool mock and helpers=========================================
 class Tool:
-    def __init__(self, id):
+    def __init__(self, id, version=None):
         self.id = id
         self.old_id = id
+        self.version = version
         self.installed_tool_dependencies = []
 
 
 # App mock=======================================================
 class App:
     def __init__(self, job_conf=None, create_model=False):
         self.config = bunch.Bunch(
```

### Comparing `total-perspective-vortex-2.2.1/tpv/core/entities.py` & `total-perspective-vortex-2.2.2/tpv/core/entities.py`

 * *Files 1% similar despite different names*

```diff
@@ -481,17 +481,17 @@
     def evaluate(self, context):
         new_entity = copy.deepcopy(self)
         context.update(new_entity.context or {})
         for rule in self.rules.values():
             if rule.is_matching(context):
                 rule = rule.evaluate(context)
                 new_entity = rule.inherit(new_entity)
-                new_entity.gpus = rule.gpus or self.gpus
-                new_entity.cores = rule.cores or self.cores
-                new_entity.mem = rule.mem or self.mem
+                new_entity.gpus = rule.gpus or new_entity.gpus
+                new_entity.cores = rule.cores or new_entity.cores
+                new_entity.mem = rule.mem or new_entity.mem
                 new_entity.id = f"{new_entity.id}, Rule: {rule.id}"
                 context.update({
                     'entity': new_entity
                 })
         return super(EntityWithRules, new_entity).evaluate(context)
 
     def __repr__(self):
```

### Comparing `total-perspective-vortex-2.2.1/tpv/core/helpers.py` & `total-perspective-vortex-2.2.2/tpv/core/helpers.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import packaging.version
 import random
 from functools import reduce
 from galaxy import model
 
 GIGABYTES = 1024.0**3
 
 
@@ -81,7 +82,23 @@
 def tag_values_match(entity, match_tag_values=[], exclude_tag_values=[]):
     # Return true if an entity has require/prefer/accept tags in the match_tags_values list
     # and no require/prefer/accept tags in the exclude_tag_values list
     return (
         all([any(entity.tpv_tags.filter(tag_value=tag_value)) for tag_value in match_tag_values])
         and not any([any(entity.tpv_tags.filter(tag_value=tag_value)) for tag_value in exclude_tag_values])
     )
+
+
+def tool_version_lte(tool, version):
+    return packaging.version.parse(tool.version) <= packaging.version.parse(version)
+
+
+def tool_version_lt(tool, version):
+    return packaging.version.parse(tool.version) < packaging.version.parse(version)
+
+
+def tool_version_gte(tool, version):
+    return packaging.version.parse(tool.version) >= packaging.version.parse(version)
+
+
+def tool_version_gt(tool, version):
+    return packaging.version.parse(tool.version) > packaging.version.parse(version)
```

### Comparing `total-perspective-vortex-2.2.1/tpv/core/loader.py` & `total-perspective-vortex-2.2.2/tpv/core/loader.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.1/tpv/core/mapper.py` & `total-perspective-vortex-2.2.2/tpv/core/mapper.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.1/tpv/rules/gateway.py` & `total-perspective-vortex-2.2.2/tpv/rules/gateway.py`

 * *Files identical despite different names*

