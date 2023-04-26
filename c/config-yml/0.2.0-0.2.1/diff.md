# Comparing `tmp/config_yml-0.2.0.tar.gz` & `tmp/config_yml-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "config_yml-0.2.0.tar", last modified: Thu Apr 13 06:58:50 2023, max compression
+gzip compressed data, was "config_yml-0.2.1.tar", last modified: Wed Apr 26 06:12:07 2023, max compression
```

## Comparing `config_yml-0.2.0.tar` & `config_yml-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 06:58:50.457719 config_yml-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-13 06:58:50.457719 config_yml-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-13 06:58:40.000000 config_yml-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 06:58:50.457719 config_yml-0.2.0/config_yml/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-13 06:58:40.000000 config_yml-0.2.0/config_yml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5333 2023-04-13 06:58:40.000000 config_yml-0.2.0/config_yml/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 06:58:50.457719 config_yml-0.2.0/config_yml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-13 06:58:50.000000 config_yml-0.2.0/config_yml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-13 06:58:50.000000 config_yml-0.2.0/config_yml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 06:58:50.000000 config_yml-0.2.0/config_yml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-13 06:58:50.000000 config_yml-0.2.0/config_yml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-13 06:58:50.000000 config_yml-0.2.0/config_yml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 06:58:50.457719 config_yml-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-13 06:58:40.000000 config_yml-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 06:58:50.457719 config_yml-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 06:58:40.000000 config_yml-0.2.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 06:58:50.457719 config_yml-0.2.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 06:58:40.000000 config_yml-0.2.0/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-13 06:58:40.000000 config_yml-0.2.0/tests/data/config_existing.yml
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-13 06:58:40.000000 config_yml-0.2.0/tests/data/config_template.yml
--rw-r--r--   0 runner    (1001) docker     (123)     6041 2023-04-13 06:58:40.000000 config_yml-0.2.0/tests/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:12:07.398057 config_yml-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-26 06:12:07.398057 config_yml-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-26 06:11:57.000000 config_yml-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:12:07.394057 config_yml-0.2.1/config_yml/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-26 06:11:57.000000 config_yml-0.2.1/config_yml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6090 2023-04-26 06:11:57.000000 config_yml-0.2.1/config_yml/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:12:07.398057 config_yml-0.2.1/config_yml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-26 06:12:07.000000 config_yml-0.2.1/config_yml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-26 06:12:07.000000 config_yml-0.2.1/config_yml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 06:12:07.000000 config_yml-0.2.1/config_yml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-26 06:12:07.000000 config_yml-0.2.1/config_yml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-26 06:12:07.000000 config_yml-0.2.1/config_yml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 06:12:07.398057 config_yml-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-26 06:11:57.000000 config_yml-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:12:07.398057 config_yml-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:11:57.000000 config_yml-0.2.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:12:07.398057 config_yml-0.2.1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:11:57.000000 config_yml-0.2.1/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-26 06:11:57.000000 config_yml-0.2.1/tests/data/config_existing.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-26 06:11:57.000000 config_yml-0.2.1/tests/data/config_template.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6041 2023-04-26 06:11:57.000000 config_yml-0.2.1/tests/test_config.py
```

### Comparing `config_yml-0.2.0/PKG-INFO` & `config_yml-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: config_yml
-Version: 0.2.0
+Version: 0.2.1
 Summary: Utility modules for Class management
 Home-page: https://github.com/Phornee/config_yml
 Author: Ismael Raya
 Author-email: phornee@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `config_yml-0.2.0/config_yml/config.py` & `config_yml-0.2.1/config_yml/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         self.homevar = os.path.join(str(Path.home()), 'var', package_name)
 
         if not os.path.exists(self.homevar):
             os.makedirs(self.homevar)
 
         self.config = {}
 
-        self._read_config()
+        self.read_config()
 
     def __getitem__(self, key):
         return self.config.get(key, None)
 
     @staticmethod
     def get_config_path(package_name: str, config_file_name: str) -> str:
         """Get the path for the config, inside the homevar path
@@ -56,15 +56,20 @@
     def get_dict_copy(self) -> dict:
         """Returns a copy of the dictionary
         Returns:
             dict: Copy of the config
         """
         return copy.deepcopy(self.config)
 
-    def _read_config(self):
+    def read_config(self):
+        """ Reads the configuration yml. 
+            First, it reads the template if provided to setup default values. That way, new default values can be
+            added to the package template, without the need of modifying all the config files already deployed.
+            Then modifies it with the specified config.yml
+        """
         # First get default values from template config file
         try:
             # First try to get the template
             with open(self._template_path, 'r', encoding="utf-8") as config_template_file:
                 template_config = yaml.load(config_template_file, Loader=yaml.FullLoader)
         except OSError:
             # No template
@@ -85,18 +90,27 @@
             else:
                 self.config = config
         else:  # No previous config
             if template_config:  # If config file doesn´t exist, but template does, write config with template content
                 self.update(template_config)
                 self.write()
 
-    def refresh(self):
-        """Force to read again the config file (and template)
+        self._after_reading()
+
+    def _after_reading(self):
+        """ Postprocess to adapt the yaml conig recently read
+        """
+
+    def _before_writting(self):
+        """ By default, it makes nothing and just return a reference to the original member config
+            If needed, it can modify the data before reading, and return a copy instead
+        Returns:
+            dict: Copy of the modified config, or the original one (by default)
         """
-        self._read_config()
+        return self.config
 
     @staticmethod
     def _merge_config(source_config: dict, dest_config: dict):
         """Merges one config dictionaty into another
 
         Args:
             source_config (dict): Source dictionary to merge
@@ -132,18 +146,19 @@
         """
         # Update keys
         self._merge_config(config_update, self.config)
 
     def write(self):
         """Write to disk the memory config 
         """
+        prepared_config = self._before_writting()
         config_yml_path = os.path.join(self.homevar, self._config_file_name)
         try:
             with open(config_yml_path, 'w', encoding="utf-8") as config_file:
-                yaml.dump(self.config, config_file)
+                yaml.dump(prepared_config, config_file)
         except OSError:
             pass
 
     def delete(self):
         """ Delete the config file """
         config_yml_path = os.path.join(self.homevar, self._config_file_name)
         try:
```

### Comparing `config_yml-0.2.0/config_yml.egg-info/PKG-INFO` & `config_yml-0.2.1/config_yml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: config-yml
-Version: 0.2.0
+Version: 0.2.1
 Summary: Utility modules for Class management
 Home-page: https://github.com/Phornee/config_yml
 Author: Ismael Raya
 Author-email: phornee@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `config_yml-0.2.0/setup.py` & `config_yml-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="config_yml",
-    version="0.2.0",
+    version="0.2.1",
     author="Ismael Raya",
     author_email="phornee@gmail.com",
     description="Utility modules for Class management",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Phornee/config_yml",
     packages=setuptools.find_packages(),
```

### Comparing `config_yml-0.2.0/tests/test_config.py` & `config_yml-0.2.1/tests/test_config.py`

 * *Files identical despite different names*

