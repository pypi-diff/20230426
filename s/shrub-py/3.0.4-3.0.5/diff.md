# Comparing `tmp/shrub.py-3.0.4.tar.gz` & `tmp/shrub_py-3.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shrub.py-3.0.4.tar", max compression
+gzip compressed data, was "shrub_py-3.0.5.tar", max compression
```

## Comparing `shrub.py-3.0.4.tar` & `shrub_py-3.0.5.tar`

### file list

```diff
@@ -1,26 +1,25 @@
--rw-r--r--   0        0        0    11536 2022-06-17 19:25:08.586081 shrub.py-3.0.4/LICENSE
--rw-r--r--   0        0        0     1285 2022-06-17 19:25:08.586081 shrub.py-3.0.4/README.md
--rw-r--r--   0        0        0      818 2022-06-17 19:25:08.586081 shrub.py-3.0.4/pyproject.toml
--rw-r--r--   0        0        0        0 2022-06-17 19:25:08.586081 shrub.py-3.0.4/src/shrub/__init__.py
--rw-r--r--   0        0        0     1531 2022-06-17 19:25:08.586081 shrub.py-3.0.4/src/shrub/base.py
--rw-r--r--   0        0        0     6189 2022-06-17 19:25:08.586081 shrub.py-3.0.4/src/shrub/command.py
--rw-r--r--   0        0        0     7208 2022-06-17 19:25:08.586081 shrub.py-3.0.4/src/shrub/config.py
--rw-r--r--   0        0        0    28873 2022-06-17 19:25:08.586081 shrub.py-3.0.4/src/shrub/operations.py
--rw-r--r--   0        0        0        0 2022-06-17 19:25:08.586081 shrub.py-3.0.4/src/shrub/py.typed
--rw-r--r--   0        0        0     8804 2022-06-17 19:25:08.586081 shrub.py-3.0.4/src/shrub/task.py
--rw-r--r--   0        0        0      266 2022-06-17 19:25:08.586081 shrub.py-3.0.4/src/shrub/v2/__init__.py
--rw-r--r--   0        0        0    22752 2022-06-17 19:25:08.586081 shrub.py-3.0.4/src/shrub/v2/command.py
--rw-r--r--   0        0        0      992 2022-06-17 19:25:08.586081 shrub.py-3.0.4/src/shrub/v2/dict_creation_util.py
--rw-r--r--   0        0        0     2386 2022-06-17 19:25:08.586081 shrub.py-3.0.4/src/shrub/v2/project.py
--rw-r--r--   0        0        0     5561 2022-06-17 19:25:08.586081 shrub.py-3.0.4/src/shrub/v2/task.py
--rw-r--r--   0        0        0     9495 2022-06-17 19:25:08.586081 shrub.py-3.0.4/src/shrub/v2/variant.py
--rw-r--r--   0        0        0        0 2022-06-17 19:25:08.586081 shrub.py-3.0.4/src/shrub/v3/__init__.py
--rw-r--r--   0        0        0     1439 2022-06-17 19:25:08.586081 shrub.py-3.0.4/src/shrub/v3/evg_build_variant.py
--rw-r--r--   0        0        0    33046 2022-06-17 19:25:08.586081 shrub.py-3.0.4/src/shrub/v3/evg_command.py
--rw-r--r--   0        0        0     3187 2022-06-17 19:25:08.586081 shrub.py-3.0.4/src/shrub/v3/evg_project.py
--rw-r--r--   0        0        0     1663 2022-06-17 19:25:08.586081 shrub.py-3.0.4/src/shrub/v3/evg_task.py
--rw-r--r--   0        0        0     1968 2022-06-17 19:25:08.586081 shrub.py-3.0.4/src/shrub/v3/evg_task_group.py
--rw-r--r--   0        0        0      921 2022-06-17 19:25:08.586081 shrub.py-3.0.4/src/shrub/v3/shrub_service.py
--rw-r--r--   0        0        0     8223 2022-06-17 19:25:08.586081 shrub.py-3.0.4/src/shrub/variant.py
--rw-r--r--   0        0        0     2312 2022-06-17 19:25:35.741433 shrub.py-3.0.4/setup.py
--rw-r--r--   0        0        0     2230 2022-06-17 19:25:35.741870 shrub.py-3.0.4/PKG-INFO
+-rw-r--r--   0        0        0    11536 2023-04-26 16:50:29.661012 shrub_py-3.0.5/LICENSE
+-rw-r--r--   0        0        0     1285 2023-04-26 16:50:29.661012 shrub_py-3.0.5/README.md
+-rw-r--r--   0        0        0      818 2023-04-26 16:50:29.661012 shrub_py-3.0.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-26 16:50:29.661012 shrub_py-3.0.5/src/shrub/__init__.py
+-rw-r--r--   0        0        0     1723 2023-04-26 16:50:29.661012 shrub_py-3.0.5/src/shrub/base.py
+-rw-r--r--   0        0        0     6189 2023-04-26 16:50:29.661012 shrub_py-3.0.5/src/shrub/command.py
+-rw-r--r--   0        0        0     7208 2023-04-26 16:50:29.661012 shrub_py-3.0.5/src/shrub/config.py
+-rw-r--r--   0        0        0    28873 2023-04-26 16:50:29.661012 shrub_py-3.0.5/src/shrub/operations.py
+-rw-r--r--   0        0        0        0 2023-04-26 16:50:29.661012 shrub_py-3.0.5/src/shrub/py.typed
+-rw-r--r--   0        0        0     9305 2023-04-26 16:50:29.661012 shrub_py-3.0.5/src/shrub/task.py
+-rw-r--r--   0        0        0      266 2023-04-26 16:50:29.661012 shrub_py-3.0.5/src/shrub/v2/__init__.py
+-rw-r--r--   0        0        0    22752 2023-04-26 16:50:29.661012 shrub_py-3.0.5/src/shrub/v2/command.py
+-rw-r--r--   0        0        0      992 2023-04-26 16:50:29.661012 shrub_py-3.0.5/src/shrub/v2/dict_creation_util.py
+-rw-r--r--   0        0        0     2386 2023-04-26 16:50:29.661012 shrub_py-3.0.5/src/shrub/v2/project.py
+-rw-r--r--   0        0        0     5561 2023-04-26 16:50:29.661012 shrub_py-3.0.5/src/shrub/v2/task.py
+-rw-r--r--   0        0        0     9495 2023-04-26 16:50:29.661012 shrub_py-3.0.5/src/shrub/v2/variant.py
+-rw-r--r--   0        0        0        0 2023-04-26 16:50:29.661012 shrub_py-3.0.5/src/shrub/v3/__init__.py
+-rw-r--r--   0        0        0     1439 2023-04-26 16:50:29.661012 shrub_py-3.0.5/src/shrub/v3/evg_build_variant.py
+-rw-r--r--   0        0        0    33046 2023-04-26 16:50:29.661012 shrub_py-3.0.5/src/shrub/v3/evg_command.py
+-rw-r--r--   0        0        0     3187 2023-04-26 16:50:29.661012 shrub_py-3.0.5/src/shrub/v3/evg_project.py
+-rw-r--r--   0        0        0     1663 2023-04-26 16:50:29.661012 shrub_py-3.0.5/src/shrub/v3/evg_task.py
+-rw-r--r--   0        0        0     1968 2023-04-26 16:50:29.661012 shrub_py-3.0.5/src/shrub/v3/evg_task_group.py
+-rw-r--r--   0        0        0      921 2023-04-26 16:50:29.661012 shrub_py-3.0.5/src/shrub/v3/shrub_service.py
+-rw-r--r--   0        0        0     9253 2023-04-26 16:50:29.661012 shrub_py-3.0.5/src/shrub/variant.py
+-rw-r--r--   0        0        0     2282 1970-01-01 00:00:00.000000 shrub_py-3.0.5/PKG-INFO
```

### Comparing `shrub.py-3.0.4/LICENSE` & `shrub_py-3.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `shrub.py-3.0.4/README.md` & `shrub_py-3.0.5/README.md`

 * *Files identical despite different names*

### Comparing `shrub.py-3.0.4/pyproject.toml` & `shrub_py-3.0.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shrub.py"
-version = "3.0.4"
+version = "3.0.5"
 description = "Library for creating evergreen configurations"
 authors = [
     "David Bradford <david.bradford@mongodb.com>",
     "Lydia Stepanek <lydia.stepanek@mongodb.com>",
     "Tausif Rahman <tausif.rahman@mongodb.com>"
 ]
 license = "Apache-2.0"
```

### Comparing `shrub.py-3.0.4/src/shrub/base.py` & `shrub_py-3.0.5/src/shrub/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,18 @@
         obj = {}
         self._add_defined_attribs(obj, self._yaml_map().keys())
         return obj
 
     def _add_if_defined(self, obj, prop):
         """Add the specified property to the given object if it exists."""
         value = getattr(self, prop)
-        if value:
+
+        # We can't just use the falsiness of value because false is a value
+        # with semantic meaning different from undefined in some keys.
+        if value is not None and value != [] and value != {}:
             if self._yaml_map()[prop][RECURSE_KEY]:
                 if isinstance(value, collections.abc.Sequence):
                     value = [v.to_map() for v in value]
                 else:
                     value = value.to_map()
             obj[self._yaml_map()[prop][NAME_KEY]] = value
```

### Comparing `shrub.py-3.0.4/src/shrub/command.py` & `shrub_py-3.0.5/src/shrub/command.py`

 * *Files identical despite different names*

### Comparing `shrub.py-3.0.4/src/shrub/config.py` & `shrub_py-3.0.5/src/shrub/config.py`

 * *Files identical despite different names*

### Comparing `shrub.py-3.0.4/src/shrub/operations.py` & `shrub_py-3.0.5/src/shrub/operations.py`

 * *Files identical despite different names*

### Comparing `shrub.py-3.0.4/src/shrub/task.py` & `shrub_py-3.0.5/src/shrub/task.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,22 +13,24 @@
             raise TypeError("Task only accepts a str")
 
         self._name = name
         self._priority = None
         self._dependencies = []
         self._requires = []
         self._commands = CommandSequence()
+        self._activate = None
 
     def _yaml_map(self):
         return {
             "_name": {NAME_KEY: "name", RECURSE_KEY: False},
             "_commands": {NAME_KEY: "commands", RECURSE_KEY: True},
             "_priority": {NAME_KEY: "priority", RECURSE_KEY: False},
             "_dependencies": {NAME_KEY: "depends_on", RECURSE_KEY: True},
             "_requires": {NAME_KEY: "requires", RECURSE_KEY: True},
+            "_activate": {NAME_KEY: "activate", RECURSE_KEY: False},
         }
 
     def get_name(self):
         """@:returns The name of the task."""
         return self._name
 
     def priority(self, value):
@@ -140,14 +142,27 @@
 
         if not isinstance(var_map, dict):
             raise TypeError("function_with_vars only accepts a dict")
 
         self._commands.add(CommandDefinition().function(fn).vars(var_map))
         return self
 
+    def activate(self, activate):
+        """
+        Specify whether this task should be activated.
+
+        :param activate: whether to activate this task.
+        :return: instance of task spec.
+        """
+        if not isinstance(activate, bool) and activate is not None:
+            raise TypeError("activate only accepts a bool or None")
+
+        self._activate = activate
+        return self
+
 
 class TaskDependency(EvergreenBuilder):
     """A dependency a task has on another task."""
 
     def __init__(self, name):
         """
         Create a task dependency.
```

### Comparing `shrub.py-3.0.4/src/shrub/v2/command.py` & `shrub_py-3.0.5/src/shrub/v2/command.py`

 * *Files identical despite different names*

### Comparing `shrub.py-3.0.4/src/shrub/v2/dict_creation_util.py` & `shrub_py-3.0.5/src/shrub/v2/dict_creation_util.py`

 * *Files identical despite different names*

### Comparing `shrub.py-3.0.4/src/shrub/v2/project.py` & `shrub_py-3.0.5/src/shrub/v2/project.py`

 * *Files identical despite different names*

### Comparing `shrub.py-3.0.4/src/shrub/v2/task.py` & `shrub_py-3.0.5/src/shrub/v2/task.py`

 * *Files identical despite different names*

### Comparing `shrub.py-3.0.4/src/shrub/v2/variant.py` & `shrub_py-3.0.5/src/shrub/v2/variant.py`

 * *Files identical despite different names*

### Comparing `shrub.py-3.0.4/src/shrub/v3/evg_build_variant.py` & `shrub_py-3.0.5/src/shrub/v3/evg_build_variant.py`

 * *Files identical despite different names*

### Comparing `shrub.py-3.0.4/src/shrub/v3/evg_command.py` & `shrub_py-3.0.5/src/shrub/v3/evg_command.py`

 * *Files identical despite different names*

### Comparing `shrub.py-3.0.4/src/shrub/v3/evg_project.py` & `shrub_py-3.0.5/src/shrub/v3/evg_project.py`

 * *Files identical despite different names*

### Comparing `shrub.py-3.0.4/src/shrub/v3/evg_task.py` & `shrub_py-3.0.5/src/shrub/v3/evg_task.py`

 * *Files identical despite different names*

### Comparing `shrub.py-3.0.4/src/shrub/v3/evg_task_group.py` & `shrub_py-3.0.5/src/shrub/v3/evg_task_group.py`

 * *Files identical despite different names*

### Comparing `shrub.py-3.0.4/src/shrub/v3/shrub_service.py` & `shrub_py-3.0.5/src/shrub/v3/shrub_service.py`

 * *Files identical despite different names*

### Comparing `shrub.py-3.0.4/src/shrub/variant.py` & `shrub_py-3.0.5/src/shrub/variant.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,25 +19,27 @@
         self._build_display_name = None
         self._batch_time_secs = None
         self._task_specs = []
         self._distro_run_on = []
         self._expansions = {}
         self._display_task_specs = []
         self._modules = []
+        self._activate = None
 
     def _yaml_map(self):
         return {
             "_build_name": {NAME_KEY: "name", RECURSE_KEY: False},
             "_build_display_name": {NAME_KEY: "display_name", RECURSE_KEY: False},
             "_batch_time_secs": {NAME_KEY: "batchtime", RECURSE_KEY: False},
             "_task_specs": {NAME_KEY: "tasks", RECURSE_KEY: True},
             "_distro_run_on": {NAME_KEY: "run_on", RECURSE_KEY: False},
             "_expansions": {NAME_KEY: "expansions", RECURSE_KEY: False},
             "_display_task_specs": {NAME_KEY: "display_tasks", RECURSE_KEY: True},
             "_modules": {NAME_KEY: "modules", RECURSE_KEY: False},
+            "_activate": {NAME_KEY: "activate", RECURSE_KEY: False},
         }
 
     def get_name(self):
         """
         Get the name of this build variant.
         :return: name of build variant.
         """
@@ -191,33 +193,48 @@
             raise TypeError("display_tasks only accepts a list")
 
         for dt in display_task_list:
             self.display_task(dt)
 
         return self
 
+    def activate(self, activate):
+        """
+        Specify whether the tasks in this variant should be activated.
+
+        :param activate: whether to activate tasks in this variant.
+        :return: instance of task spec.
+        """
+        if not isinstance(activate, bool) and activate is not None:
+            raise TypeError("activate only accepts a bool or None")
+
+        self._activate = activate
+        return self
+
 
 class TaskSpec(EvergreenBuilder):
     """A spec for adding a task to a variant."""
 
     def __init__(self, name):
         """
         Create a task spec.
 
         :param name: name of task.
         """
         self._name = name
         self._stepback = None
         self._distro = []
+        self._activate = None
 
     def _yaml_map(self):
         return {
             "_name": {NAME_KEY: "name", RECURSE_KEY: False},
             "_stepback": {NAME_KEY: "stepback", RECURSE_KEY: False},
             "_distro": {NAME_KEY: "distros", RECURSE_KEY: False},
+            "_activate": {NAME_KEY: "activate", RECURSE_KEY: False},
         }
 
     def stepback(self):
         """
         Enable stepback for this task.
         :return:
         """
@@ -233,14 +250,27 @@
         """
         if not isinstance(distro, str):
             raise TypeError("distro only accepts a str")
 
         self._distro = [distro]
         return self
 
+    def activate(self, activate):
+        """
+        Specify whether this task should be activated.
+
+        :param activate: whether to activate this task.
+        :return: instance of task spec.
+        """
+        if not isinstance(activate, bool) and activate is not None:
+            raise TypeError("activate only accepts a bool or None")
+
+        self._activate = activate
+        return self
+
 
 class DisplayTaskDefinition(EvergreenBuilder):
     """Defines a display task for evergreen."""
 
     def __init__(self, name):
         """
         Create a display task definition.
```

### Comparing `shrub.py-3.0.4/PKG-INFO` & `shrub_py-3.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
-Name: shrub.py
-Version: 3.0.4
+Name: shrub-py
+Version: 3.0.5
 Summary: Library for creating evergreen configurations
 Home-page: https://github.com/evergreen-ci/shrub.py
 License: Apache-2.0
 Author: David Bradford
 Author-email: david.bradford@mongodb.com
 Requires-Python: >3.6.1
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyYaml (>=5.1,<6.0)
-Requires-Dist: dataclasses (>=0.7,<0.8); python_full_version >= "3.6.0" and python_full_version < "3.7.0"
+Requires-Dist: dataclasses (>=0.7,<0.8) ; python_full_version >= "3.6.0" and python_full_version < "3.7.0"
 Requires-Dist: git-url-parse (>=1,<2)
 Requires-Dist: pydantic (>=1.8,<2.0)
 Requires-Dist: typing-extensions (>=4,<5)
 Project-URL: Repository, https://github.com/evergreen-ci/shrub.py
 Description-Content-Type: text/markdown
 
 # shrub.py
```

