# Comparing `tmp/pyaprilaire-0.6.0b0.tar.gz` & `tmp/pyaprilaire-0.6.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaprilaire-0.6.0b0.tar", last modified: Tue Apr 25 23:57:20 2023, max compression
+gzip compressed data, was "pyaprilaire-0.6.0b1.tar", last modified: Wed Apr 26 00:23:50 2023, max compression
```

## Comparing `pyaprilaire-0.6.0b0.tar` & `pyaprilaire-0.6.0b1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:57:20.980825 pyaprilaire-0.6.0b0/
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-25 23:57:09.000000 pyaprilaire-0.6.0b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-25 23:57:09.000000 pyaprilaire-0.6.0b0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-04-25 23:57:20.976825 pyaprilaire-0.6.0b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-04-25 23:57:09.000000 pyaprilaire-0.6.0b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:57:20.976825 pyaprilaire-0.6.0b0/pyaprilaire/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 23:57:09.000000 pyaprilaire-0.6.0b0/pyaprilaire/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16820 2023-04-25 23:57:09.000000 pyaprilaire-0.6.0b0/pyaprilaire/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-25 23:57:09.000000 pyaprilaire-0.6.0b0/pyaprilaire/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    26633 2023-04-25 23:57:09.000000 pyaprilaire-0.6.0b0/pyaprilaire/mock_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    18195 2023-04-25 23:57:09.000000 pyaprilaire-0.6.0b0/pyaprilaire/packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-04-25 23:57:09.000000 pyaprilaire-0.6.0b0/pyaprilaire/socket_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:57:20.976825 pyaprilaire-0.6.0b0/pyaprilaire.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-04-25 23:57:20.000000 pyaprilaire-0.6.0b0/pyaprilaire.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-25 23:57:20.000000 pyaprilaire-0.6.0b0/pyaprilaire.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 23:57:20.000000 pyaprilaire-0.6.0b0/pyaprilaire.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-25 23:57:20.000000 pyaprilaire-0.6.0b0/pyaprilaire.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-25 23:57:20.000000 pyaprilaire-0.6.0b0/pyaprilaire.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-25 23:57:09.000000 pyaprilaire-0.6.0b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 23:57:20.980825 pyaprilaire-0.6.0b0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:57:20.976825 pyaprilaire-0.6.0b0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    18477 2023-04-25 23:57:09.000000 pyaprilaire-0.6.0b0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13337 2023-04-25 23:57:09.000000 pyaprilaire-0.6.0b0/tests/test_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6201 2023-04-25 23:57:09.000000 pyaprilaire-0.6.0b0/tests/test_socket_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 00:23:50.262863 pyaprilaire-0.6.0b1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-26 00:23:36.000000 pyaprilaire-0.6.0b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-26 00:23:36.000000 pyaprilaire-0.6.0b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-04-26 00:23:50.262863 pyaprilaire-0.6.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-04-26 00:23:36.000000 pyaprilaire-0.6.0b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 00:23:50.258863 pyaprilaire-0.6.0b1/pyaprilaire/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 00:23:36.000000 pyaprilaire-0.6.0b1/pyaprilaire/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16821 2023-04-26 00:23:36.000000 pyaprilaire-0.6.0b1/pyaprilaire/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-26 00:23:36.000000 pyaprilaire-0.6.0b1/pyaprilaire/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26633 2023-04-26 00:23:36.000000 pyaprilaire-0.6.0b1/pyaprilaire/mock_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18195 2023-04-26 00:23:36.000000 pyaprilaire-0.6.0b1/pyaprilaire/packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-04-26 00:23:36.000000 pyaprilaire-0.6.0b1/pyaprilaire/socket_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 00:23:50.262863 pyaprilaire-0.6.0b1/pyaprilaire.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-04-26 00:23:50.000000 pyaprilaire-0.6.0b1/pyaprilaire.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-26 00:23:50.000000 pyaprilaire-0.6.0b1/pyaprilaire.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 00:23:50.000000 pyaprilaire-0.6.0b1/pyaprilaire.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-26 00:23:50.000000 pyaprilaire-0.6.0b1/pyaprilaire.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-26 00:23:50.000000 pyaprilaire-0.6.0b1/pyaprilaire.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-26 00:23:36.000000 pyaprilaire-0.6.0b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 00:23:50.262863 pyaprilaire-0.6.0b1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 00:23:50.262863 pyaprilaire-0.6.0b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    18477 2023-04-26 00:23:36.000000 pyaprilaire-0.6.0b1/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13337 2023-04-26 00:23:36.000000 pyaprilaire-0.6.0b1/tests/test_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6201 2023-04-26 00:23:36.000000 pyaprilaire-0.6.0b1/tests/test_socket_client.py
```

### Comparing `pyaprilaire-0.6.0b0/LICENSE` & `pyaprilaire-0.6.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyaprilaire-0.6.0b0/PKG-INFO` & `pyaprilaire-0.6.0b1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaprilaire
-Version: 0.6.0b0
+Version: 0.6.0b1
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # pyaprilaire
 
 pyaprilaire is a library to interact with Aprilaire thermostats.
```

### Comparing `pyaprilaire-0.6.0b0/README.md` & `pyaprilaire-0.6.0b1/README.md`

 * *Files identical despite different names*

### Comparing `pyaprilaire-0.6.0b0/pyaprilaire/client.py` & `pyaprilaire-0.6.0b1/pyaprilaire/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -305,21 +305,21 @@
                 raw_data=[
                     1,  # Installer Thermostat Settings
                     0,  # Contractor Information
                     0,  # Air Cleaning Installer Variable
                     0,  # Humidity Control Installer Settings
                     0,  # Fresh Air Installer Settings
                     1,  # Thermostat Setpoint & Mode Settings
-                    0,  # Dehumidification Setpoint
-                    0,  # Humidification Setpoint
-                    0,  # Fresh Air Setting
-                    0,  # Air Cleaning Settings
+                    1,  # Dehumidification Setpoint
+                    1,  # Humidification Setpoint
+                    1,  # Fresh Air Settings
+                    1,  # Air Cleaning Settings
                     1,  # Thermostat IAQ Available
                     0,  # Schedule Settings
-                    0,  # Away Settings
+                    1,  # Away Settings
                     0,  # Schedule Day
                     1,  # Schedule Hold
                     0,  # Heat Blast
                     0,  # Service Reminders Status
                     0,  # Alerts Status
                     0,  # Alerts Settings
                     0,  # Backlight Settings
```

### Comparing `pyaprilaire-0.6.0b0/pyaprilaire/const.py` & `pyaprilaire-0.6.0b1/pyaprilaire/const.py`

 * *Files identical despite different names*

### Comparing `pyaprilaire-0.6.0b0/pyaprilaire/mock_server.py` & `pyaprilaire-0.6.0b1/pyaprilaire/mock_server.py`

 * *Files identical despite different names*

### Comparing `pyaprilaire-0.6.0b0/pyaprilaire/packet.py` & `pyaprilaire-0.6.0b1/pyaprilaire/packet.py`

 * *Files identical despite different names*

### Comparing `pyaprilaire-0.6.0b0/pyaprilaire/socket_client.py` & `pyaprilaire-0.6.0b1/pyaprilaire/socket_client.py`

 * *Files identical despite different names*

### Comparing `pyaprilaire-0.6.0b0/pyaprilaire.egg-info/PKG-INFO` & `pyaprilaire-0.6.0b1/pyaprilaire.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaprilaire
-Version: 0.6.0b0
+Version: 0.6.0b1
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # pyaprilaire
 
 pyaprilaire is a library to interact with Aprilaire thermostats.
```

### Comparing `pyaprilaire-0.6.0b0/pyproject.toml` & `pyaprilaire-0.6.0b1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyaprilaire"
-version = "0.6.0b0"
+version = "0.6.0b1"
 readme = "README.md"
 dependencies = [
     "crc >= 4"
 ]
 
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pip-tools", "coverage"]
 
 [tool.bumpver]
-current_version = "0.6.0b0"
+current_version = "0.6.0b1"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `pyaprilaire-0.6.0b0/tests/test_client.py` & `pyaprilaire-0.6.0b1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `pyaprilaire-0.6.0b0/tests/test_packet.py` & `pyaprilaire-0.6.0b1/tests/test_packet.py`

 * *Files identical despite different names*

### Comparing `pyaprilaire-0.6.0b0/tests/test_socket_client.py` & `pyaprilaire-0.6.0b1/tests/test_socket_client.py`

 * *Files identical despite different names*

