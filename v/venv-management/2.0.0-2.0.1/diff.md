# Comparing `tmp/venv-management-2.0.0.tar.gz` & `tmp/venv-management-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "venv-management-2.0.0.tar", last modified: Wed Apr 26 09:59:34 2023, max compression
+gzip compressed data, was "venv-management-2.0.1.tar", last modified: Wed Apr 26 11:49:40 2023, max compression
```

## Comparing `venv-management-2.0.0.tar` & `venv-management-2.0.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:59:34.814178 venv-management-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-04-26 09:59:23.000000 venv-management-2.0.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6987 2023-04-26 09:59:34.814178 venv-management-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-04-26 09:59:23.000000 venv-management-2.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-26 09:59:23.000000 venv-management-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-04-26 09:59:34.818178 venv-management-2.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:59:34.810178 venv-management-2.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:59:34.814178 venv-management-2.0.0/src/venv_management/
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-26 09:59:23.000000 venv-management-2.0.0/src/venv_management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9102 2023-04-26 09:59:23.000000 venv-management-2.0.0/src/venv_management/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6060 2023-04-26 09:59:23.000000 venv-management-2.0.0/src/venv_management/driver.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-26 09:59:23.000000 venv-management-2.0.0/src/venv_management/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:59:34.814178 venv-management-2.0.0/src/venv_management/ext/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 09:59:23.000000 venv-management-2.0.0/src/venv_management/ext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:59:34.814178 venv-management-2.0.0/src/venv_management/ext/drivers/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 09:59:23.000000 venv-management-2.0.0/src/venv_management/ext/drivers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:59:34.814178 venv-management-2.0.0/src/venv_management/ext/drivers/pyenv_virtualenv/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-26 09:59:23.000000 venv-management-2.0.0/src/venv_management/ext/drivers/pyenv_virtualenv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-04-26 09:59:23.000000 venv-management-2.0.0/src/venv_management/ext/drivers/pyenv_virtualenv/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:59:34.814178 venv-management-2.0.0/src/venv_management/ext/drivers/virtualenv_sh/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-26 09:59:23.000000 venv-management-2.0.0/src/venv_management/ext/drivers/virtualenv_sh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-04-26 09:59:23.000000 venv-management-2.0.0/src/venv_management/ext/drivers/virtualenv_sh/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:59:34.814178 venv-management-2.0.0/src/venv_management/ext/drivers/virtualenvwrapper/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-26 09:59:23.000000 venv-management-2.0.0/src/venv_management/ext/drivers/virtualenvwrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-04-26 09:59:23.000000 venv-management-2.0.0/src/venv_management/ext/drivers/virtualenvwrapper/driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-04-26 09:59:23.000000 venv-management-2.0.0/src/venv_management/extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-04-26 09:59:23.000000 venv-management-2.0.0/src/venv_management/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-26 09:59:23.000000 venv-management-2.0.0/src/venv_management/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:59:34.814178 venv-management-2.0.0/src/venv_management.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6987 2023-04-26 09:59:34.000000 venv-management-2.0.0/src/venv_management.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-26 09:59:34.000000 venv-management-2.0.0/src/venv_management.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 09:59:34.000000 venv-management-2.0.0/src/venv_management.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-26 09:59:34.000000 venv-management-2.0.0/src/venv_management.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-26 09:59:34.000000 venv-management-2.0.0/src/venv_management.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-26 09:59:34.000000 venv-management-2.0.0/src/venv_management.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 09:59:34.000000 venv-management-2.0.0/src/venv_management.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:59:34.814178 venv-management-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-26 09:59:23.000000 venv-management-2.0.0/tests/test_check_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-26 09:59:23.000000 venv-management-2.0.0/tests/test_discard_virtual_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-26 09:59:23.000000 venv-management-2.0.0/tests/test_ensure_virtual_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-26 09:59:23.000000 venv-management-2.0.0/tests/test_has_virtualenvwrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-26 09:59:23.000000 venv-management-2.0.0/tests/test_list_virtual_envs.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-26 09:59:23.000000 venv-management-2.0.0/tests/test_make_virtual_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-26 09:59:23.000000 venv-management-2.0.0/tests/test_remove_virtual_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-26 09:59:23.000000 venv-management-2.0.0/tests/test_resolve_virtual_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-26 09:59:23.000000 venv-management-2.0.0/tests/test_virtual_env_context_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:49:40.091928 venv-management-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-04-26 11:49:26.000000 venv-management-2.0.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6987 2023-04-26 11:49:40.095928 venv-management-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-04-26 11:49:26.000000 venv-management-2.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-26 11:49:26.000000 venv-management-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-04-26 11:49:40.095928 venv-management-2.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:49:40.071927 venv-management-2.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:49:40.083927 venv-management-2.0.1/src/venv_management/
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-26 11:49:26.000000 venv-management-2.0.1/src/venv_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9102 2023-04-26 11:49:26.000000 venv-management-2.0.1/src/venv_management/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6060 2023-04-26 11:49:26.000000 venv-management-2.0.1/src/venv_management/driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-26 11:49:26.000000 venv-management-2.0.1/src/venv_management/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:49:40.087928 venv-management-2.0.1/src/venv_management/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 11:49:26.000000 venv-management-2.0.1/src/venv_management/ext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:49:40.087928 venv-management-2.0.1/src/venv_management/ext/drivers/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 11:49:26.000000 venv-management-2.0.1/src/venv_management/ext/drivers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:49:40.087928 venv-management-2.0.1/src/venv_management/ext/drivers/pyenv_virtualenv/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-26 11:49:26.000000 venv-management-2.0.1/src/venv_management/ext/drivers/pyenv_virtualenv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7717 2023-04-26 11:49:26.000000 venv-management-2.0.1/src/venv_management/ext/drivers/pyenv_virtualenv/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:49:40.087928 venv-management-2.0.1/src/venv_management/ext/drivers/virtualenv_sh/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-26 11:49:26.000000 venv-management-2.0.1/src/venv_management/ext/drivers/virtualenv_sh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-04-26 11:49:26.000000 venv-management-2.0.1/src/venv_management/ext/drivers/virtualenv_sh/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:49:40.087928 venv-management-2.0.1/src/venv_management/ext/drivers/virtualenvwrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-26 11:49:26.000000 venv-management-2.0.1/src/venv_management/ext/drivers/virtualenvwrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-04-26 11:49:26.000000 venv-management-2.0.1/src/venv_management/ext/drivers/virtualenvwrapper/driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-04-26 11:49:26.000000 venv-management-2.0.1/src/venv_management/extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-04-26 11:49:26.000000 venv-management-2.0.1/src/venv_management/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-26 11:49:26.000000 venv-management-2.0.1/src/venv_management/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:49:40.083927 venv-management-2.0.1/src/venv_management.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6987 2023-04-26 11:49:40.000000 venv-management-2.0.1/src/venv_management.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-26 11:49:40.000000 venv-management-2.0.1/src/venv_management.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 11:49:40.000000 venv-management-2.0.1/src/venv_management.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-26 11:49:40.000000 venv-management-2.0.1/src/venv_management.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-26 11:49:40.000000 venv-management-2.0.1/src/venv_management.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-26 11:49:40.000000 venv-management-2.0.1/src/venv_management.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 11:49:39.000000 venv-management-2.0.1/src/venv_management.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:49:40.091928 venv-management-2.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-26 11:49:26.000000 venv-management-2.0.1/tests/test_check_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-26 11:49:26.000000 venv-management-2.0.1/tests/test_discard_virtual_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-26 11:49:26.000000 venv-management-2.0.1/tests/test_ensure_virtual_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-26 11:49:26.000000 venv-management-2.0.1/tests/test_has_virtualenvwrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-26 11:49:26.000000 venv-management-2.0.1/tests/test_list_virtual_envs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-26 11:49:26.000000 venv-management-2.0.1/tests/test_make_virtual_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-26 11:49:26.000000 venv-management-2.0.1/tests/test_remove_virtual_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-26 11:49:26.000000 venv-management-2.0.1/tests/test_resolve_virtual_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-26 11:49:26.000000 venv-management-2.0.1/tests/test_virtual_env_context_manager.py
```

### Comparing `venv-management-2.0.0/LICENSE.txt` & `venv-management-2.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `venv-management-2.0.0/PKG-INFO` & `venv-management-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: venv-management
-Version: 2.0.0
+Version: 2.0.1
 Summary: A Python package for programmatic creation of Python virtual environments
 Home-page: https://github.com/sixty-north/venv-management
 Author: Sixty North AS
 Author-email: systems+venv_management@sixty-north.com
 License: MIT License
 Keywords: virtual-environment
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `venv-management-2.0.0/README.rst` & `venv-management-2.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `venv-management-2.0.0/setup.cfg` & `venv-management-2.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `venv-management-2.0.0/src/venv_management/__init__.py` & `venv-management-2.0.1/src/venv_management/__init__.py`

 * *Files identical despite different names*

### Comparing `venv-management-2.0.0/src/venv_management/api.py` & `venv-management-2.0.1/src/venv_management/api.py`

 * *Files identical despite different names*

### Comparing `venv-management-2.0.0/src/venv_management/driver.py` & `venv-management-2.0.1/src/venv_management/driver.py`

 * *Files identical despite different names*

### Comparing `venv-management-2.0.0/src/venv_management/ext/drivers/pyenv_virtualenv/driver.py` & `venv-management-2.0.1/src/venv_management/ext/drivers/pyenv_virtualenv/driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,17 @@
         list_virtual_envs_command = "pyenv virtualenvs --bare"
         command = sub_shell_command(list_virtual_envs_command)
         logger.debug(f"Running command: {command}")
         status, output = get_status_output(command)
         if status == 0:
             return output.splitlines(keepends=False)
         logger.error(output)
-        if status == 127:
+        if status == 127:  # Pyenv is not installed
+            raise CommandNotFound(output)
+        if status == 1:  # The subcommand passed to Pyenv is not recognized
             raise CommandNotFound(output)
         raise RuntimeError(output)
 
     def make_virtual_env(
             self,
             name,
             *,
```

### Comparing `venv-management-2.0.0/src/venv_management/ext/drivers/virtualenv_sh/driver.py` & `venv-management-2.0.1/src/venv_management/ext/drivers/virtualenv_sh/driver.py`

 * *Files identical despite different names*

### Comparing `venv-management-2.0.0/src/venv_management/ext/drivers/virtualenvwrapper/driver.py` & `venv-management-2.0.1/src/venv_management/ext/drivers/virtualenvwrapper/driver.py`

 * *Files identical despite different names*

### Comparing `venv-management-2.0.0/src/venv_management/extension.py` & `venv-management-2.0.1/src/venv_management/extension.py`

 * *Files identical despite different names*

### Comparing `venv-management-2.0.0/src/venv_management/utilities.py` & `venv-management-2.0.1/src/venv_management/utilities.py`

 * *Files identical despite different names*

### Comparing `venv-management-2.0.0/src/venv_management.egg-info/PKG-INFO` & `venv-management-2.0.1/src/venv_management.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: venv-management
-Version: 2.0.0
+Version: 2.0.1
 Summary: A Python package for programmatic creation of Python virtual environments
 Home-page: https://github.com/sixty-north/venv-management
 Author: Sixty North AS
 Author-email: systems+venv_management@sixty-north.com
 License: MIT License
 Keywords: virtual-environment
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `venv-management-2.0.0/src/venv_management.egg-info/SOURCES.txt` & `venv-management-2.0.1/src/venv_management.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `venv-management-2.0.0/tests/test_discard_virtual_env.py` & `venv-management-2.0.1/tests/test_discard_virtual_env.py`

 * *Files identical despite different names*

### Comparing `venv-management-2.0.0/tests/test_ensure_virtual_env.py` & `venv-management-2.0.1/tests/test_ensure_virtual_env.py`

 * *Files identical despite different names*

### Comparing `venv-management-2.0.0/tests/test_make_virtual_env.py` & `venv-management-2.0.1/tests/test_make_virtual_env.py`

 * *Files identical despite different names*

### Comparing `venv-management-2.0.0/tests/test_remove_virtual_env.py` & `venv-management-2.0.1/tests/test_remove_virtual_env.py`

 * *Files identical despite different names*

### Comparing `venv-management-2.0.0/tests/test_resolve_virtual_env.py` & `venv-management-2.0.1/tests/test_resolve_virtual_env.py`

 * *Files identical despite different names*

