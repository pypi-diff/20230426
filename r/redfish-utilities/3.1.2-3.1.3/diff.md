# Comparing `tmp/redfish_utilities-3.1.2.tar.gz` & `tmp/redfish_utilities-3.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redfish_utilities-3.1.2.tar", last modified: Fri Jan 13 20:48:45 2023, max compression
+gzip compressed data, was "redfish_utilities-3.1.3.tar", last modified: Tue Apr 25 14:51:11 2023, max compression
```

## Comparing `redfish_utilities-3.1.2.tar` & `redfish_utilities-3.1.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 20:48:45.419177 redfish_utilities-3.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-01-13 20:48:34.000000 redfish_utilities-3.1.2/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-01-13 20:48:34.000000 redfish_utilities-3.1.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    37339 2023-01-13 20:48:45.419177 redfish_utilities-3.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    36795 2023-01-13 20:48:34.000000 redfish_utilities-3.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 20:48:45.415176 redfish_utilities-3.1.2/redfish_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-01-13 20:48:34.000000 redfish_utilities-3.1.2/redfish_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8116 2023-01-13 20:48:34.000000 redfish_utilities-3.1.2/redfish_utilities/accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-01-13 20:48:34.000000 redfish_utilities-3.1.2/redfish_utilities/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9051 2023-01-13 20:48:34.000000 redfish_utilities-3.1.2/redfish_utilities/event_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    17523 2023-01-13 20:48:34.000000 redfish_utilities-3.1.2/redfish_utilities/inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)    12228 2023-01-13 20:48:34.000000 redfish_utilities-3.1.2/redfish_utilities/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17900 2023-01-13 20:48:34.000000 redfish_utilities-3.1.2/redfish_utilities/managers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-01-13 20:48:34.000000 redfish_utilities-3.1.2/redfish_utilities/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-01-13 20:48:34.000000 redfish_utilities-3.1.2/redfish_utilities/resets.py
--rw-r--r--   0 runner    (1001) docker     (123)    22014 2023-01-13 20:48:34.000000 redfish_utilities-3.1.2/redfish_utilities/sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)    25851 2023-01-13 20:48:34.000000 redfish_utilities-3.1.2/redfish_utilities/systems.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-01-13 20:48:34.000000 redfish_utilities-3.1.2/redfish_utilities/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6002 2023-01-13 20:48:34.000000 redfish_utilities-3.1.2/redfish_utilities/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 20:48:45.415176 redfish_utilities-3.1.2/redfish_utilities.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    37339 2023-01-13 20:48:45.000000 redfish_utilities-3.1.2/redfish_utilities.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-01-13 20:48:45.000000 redfish_utilities-3.1.2/redfish_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-13 20:48:45.000000 redfish_utilities-3.1.2/redfish_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-01-13 20:48:45.000000 redfish_utilities-3.1.2/redfish_utilities.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-01-13 20:48:45.000000 redfish_utilities-3.1.2/redfish_utilities.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 20:48:45.419177 redfish_utilities-3.1.2/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-01-13 20:48:34.000000 redfish_utilities-3.1.2/scripts/rf_accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-01-13 20:48:34.000000 redfish_utilities-3.1.2/scripts/rf_bios_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-01-13 20:48:34.000000 redfish_utilities-3.1.2/scripts/rf_boot_override.py
--rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-01-13 20:48:34.000000 redfish_utilities-3.1.2/scripts/rf_diagnostic_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-01-13 20:48:34.000000 redfish_utilities-3.1.2/scripts/rf_discover.py
--rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-01-13 20:48:34.000000 redfish_utilities-3.1.2/scripts/rf_event_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-01-13 20:48:34.000000 redfish_utilities-3.1.2/scripts/rf_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7599 2023-01-13 20:48:34.000000 redfish_utilities-3.1.2/scripts/rf_manager_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-01-13 20:48:34.000000 redfish_utilities-3.1.2/scripts/rf_power_reset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-01-13 20:48:34.000000 redfish_utilities-3.1.2/scripts/rf_raw_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-01-13 20:48:34.000000 redfish_utilities-3.1.2/scripts/rf_sensor_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-01-13 20:48:34.000000 redfish_utilities-3.1.2/scripts/rf_sys_inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-01-13 20:48:34.000000 redfish_utilities-3.1.2/scripts/rf_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-01-13 20:48:34.000000 redfish_utilities-3.1.2/scripts/rf_virtual_media.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-13 20:48:45.419177 redfish_utilities-3.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-01-13 20:48:34.000000 redfish_utilities-3.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:51:11.717513 redfish_utilities-3.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-25 14:50:50.000000 redfish_utilities-3.1.3/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-04-25 14:50:50.000000 redfish_utilities-3.1.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    37487 2023-04-25 14:51:11.717513 redfish_utilities-3.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    36943 2023-04-25 14:50:50.000000 redfish_utilities-3.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:51:11.713513 redfish_utilities-3.1.3/redfish_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-04-25 14:50:50.000000 redfish_utilities-3.1.3/redfish_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8116 2023-04-25 14:50:50.000000 redfish_utilities-3.1.3/redfish_utilities/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-25 14:50:50.000000 redfish_utilities-3.1.3/redfish_utilities/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9051 2023-04-25 14:50:50.000000 redfish_utilities-3.1.3/redfish_utilities/event_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17523 2023-04-25 14:50:50.000000 redfish_utilities-3.1.3/redfish_utilities/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12228 2023-04-25 14:50:50.000000 redfish_utilities-3.1.3/redfish_utilities/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17900 2023-04-25 14:50:50.000000 redfish_utilities-3.1.3/redfish_utilities/managers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-04-25 14:50:50.000000 redfish_utilities-3.1.3/redfish_utilities/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-25 14:50:50.000000 redfish_utilities-3.1.3/redfish_utilities/resets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22014 2023-04-25 14:50:50.000000 redfish_utilities-3.1.3/redfish_utilities/sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25851 2023-04-25 14:50:50.000000 redfish_utilities-3.1.3/redfish_utilities/systems.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-04-25 14:50:50.000000 redfish_utilities-3.1.3/redfish_utilities/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6002 2023-04-25 14:50:50.000000 redfish_utilities-3.1.3/redfish_utilities/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:51:11.713513 redfish_utilities-3.1.3/redfish_utilities.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    37487 2023-04-25 14:51:11.000000 redfish_utilities-3.1.3/redfish_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-25 14:51:11.000000 redfish_utilities-3.1.3/redfish_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 14:51:11.000000 redfish_utilities-3.1.3/redfish_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-25 14:51:11.000000 redfish_utilities-3.1.3/redfish_utilities.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-25 14:51:11.000000 redfish_utilities-3.1.3/redfish_utilities.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:51:11.717513 redfish_utilities-3.1.3/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-04-25 14:50:50.000000 redfish_utilities-3.1.3/scripts/rf_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-04-25 14:50:50.000000 redfish_utilities-3.1.3/scripts/rf_bios_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-04-25 14:50:50.000000 redfish_utilities-3.1.3/scripts/rf_boot_override.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-04-25 14:50:50.000000 redfish_utilities-3.1.3/scripts/rf_diagnostic_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-04-25 14:50:50.000000 redfish_utilities-3.1.3/scripts/rf_discover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-04-25 14:50:50.000000 redfish_utilities-3.1.3/scripts/rf_event_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-04-25 14:50:50.000000 redfish_utilities-3.1.3/scripts/rf_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7599 2023-04-25 14:50:50.000000 redfish_utilities-3.1.3/scripts/rf_manager_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-04-25 14:50:50.000000 redfish_utilities-3.1.3/scripts/rf_power_reset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-04-25 14:50:50.000000 redfish_utilities-3.1.3/scripts/rf_raw_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-04-25 14:50:50.000000 redfish_utilities-3.1.3/scripts/rf_sensor_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-04-25 14:50:50.000000 redfish_utilities-3.1.3/scripts/rf_sys_inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-04-25 14:50:50.000000 redfish_utilities-3.1.3/scripts/rf_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-04-25 14:50:50.000000 redfish_utilities-3.1.3/scripts/rf_virtual_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 14:51:11.717513 redfish_utilities-3.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-04-25 14:50:50.000000 redfish_utilities-3.1.3/setup.py
```

### Comparing `redfish_utilities-3.1.2/LICENSE.md` & `redfish_utilities-3.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.2/PKG-INFO` & `redfish_utilities-3.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redfish_utilities
-Version: 3.1.2
+Version: 3.1.3
 Summary: Redfish Utilities
 Home-page: https://github.com/DMTF/Redfish-Tacklebox
 Author: DMTF, https://www.dmtf.org/standards/feedback
 License: BSD 3-clause "New" or "Revised License"
 Keywords: Redfish
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
@@ -798,15 +798,17 @@
                         The URI for the request
 
 optional arguments:
   -h, --help            show this help message and exit
   --method {GET,HEAD,POST,PATCH,PUT,DELETE}, -m {GET,HEAD,POST,PATCH,PUT,DELETE}
                         The HTTP method to perform; performs GET if not
                         specified
-  --body BODY, -b BODY  The body to provide with the request
+  --body BODY, -b BODY  The body to provide with the request; can be a JSON
+                        string for a JSON request, a filename to send binary
+                        data, or an unstructured string
   --verbose, -v         Indicates if HTTP response codes and headers are
                         displayed
 ```
 
 Example: `rf_raw_request.py -u root -p root -r https://192.168.1.100 -req /redfish/v1/Systems/1 -m PATCH -b '{"AssetTag": "New tag"}'`
 
 The tool will log into the service specified by the *rhost* argument using the credentials provided by the *user* and *password* arguments.
```

### Comparing `redfish_utilities-3.1.2/README.md` & `redfish_utilities-3.1.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -782,15 +782,17 @@
                         The URI for the request
 
 optional arguments:
   -h, --help            show this help message and exit
   --method {GET,HEAD,POST,PATCH,PUT,DELETE}, -m {GET,HEAD,POST,PATCH,PUT,DELETE}
                         The HTTP method to perform; performs GET if not
                         specified
-  --body BODY, -b BODY  The body to provide with the request
+  --body BODY, -b BODY  The body to provide with the request; can be a JSON
+                        string for a JSON request, a filename to send binary
+                        data, or an unstructured string
   --verbose, -v         Indicates if HTTP response codes and headers are
                         displayed
 ```
 
 Example: `rf_raw_request.py -u root -p root -r https://192.168.1.100 -req /redfish/v1/Systems/1 -m PATCH -b '{"AssetTag": "New tag"}'`
 
 The tool will log into the service specified by the *rhost* argument using the credentials provided by the *user* and *password* arguments.
```

### Comparing `redfish_utilities-3.1.2/redfish_utilities/__init__.py` & `redfish_utilities-3.1.3/redfish_utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.2/redfish_utilities/accounts.py` & `redfish_utilities-3.1.3/redfish_utilities/accounts.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.2/redfish_utilities/config.py` & `redfish_utilities-3.1.3/redfish_utilities/config.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.2/redfish_utilities/event_service.py` & `redfish_utilities-3.1.3/redfish_utilities/event_service.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.2/redfish_utilities/inventory.py` & `redfish_utilities-3.1.3/redfish_utilities/inventory.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.2/redfish_utilities/logs.py` & `redfish_utilities-3.1.3/redfish_utilities/logs.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.2/redfish_utilities/managers.py` & `redfish_utilities-3.1.3/redfish_utilities/managers.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.2/redfish_utilities/messages.py` & `redfish_utilities-3.1.3/redfish_utilities/messages.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.2/redfish_utilities/resets.py` & `redfish_utilities-3.1.3/redfish_utilities/resets.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.2/redfish_utilities/sensors.py` & `redfish_utilities-3.1.3/redfish_utilities/sensors.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.2/redfish_utilities/systems.py` & `redfish_utilities-3.1.3/redfish_utilities/systems.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.2/redfish_utilities/tasks.py` & `redfish_utilities-3.1.3/redfish_utilities/tasks.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.2/redfish_utilities/update.py` & `redfish_utilities-3.1.3/redfish_utilities/update.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.2/redfish_utilities.egg-info/PKG-INFO` & `redfish_utilities-3.1.3/redfish_utilities.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redfish-utilities
-Version: 3.1.2
+Version: 3.1.3
 Summary: Redfish Utilities
 Home-page: https://github.com/DMTF/Redfish-Tacklebox
 Author: DMTF, https://www.dmtf.org/standards/feedback
 License: BSD 3-clause "New" or "Revised License"
 Keywords: Redfish
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
@@ -798,15 +798,17 @@
                         The URI for the request
 
 optional arguments:
   -h, --help            show this help message and exit
   --method {GET,HEAD,POST,PATCH,PUT,DELETE}, -m {GET,HEAD,POST,PATCH,PUT,DELETE}
                         The HTTP method to perform; performs GET if not
                         specified
-  --body BODY, -b BODY  The body to provide with the request
+  --body BODY, -b BODY  The body to provide with the request; can be a JSON
+                        string for a JSON request, a filename to send binary
+                        data, or an unstructured string
   --verbose, -v         Indicates if HTTP response codes and headers are
                         displayed
 ```
 
 Example: `rf_raw_request.py -u root -p root -r https://192.168.1.100 -req /redfish/v1/Systems/1 -m PATCH -b '{"AssetTag": "New tag"}'`
 
 The tool will log into the service specified by the *rhost* argument using the credentials provided by the *user* and *password* arguments.
```

### Comparing `redfish_utilities-3.1.2/redfish_utilities.egg-info/SOURCES.txt` & `redfish_utilities-3.1.3/redfish_utilities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.2/scripts/rf_accounts.py` & `redfish_utilities-3.1.3/scripts/rf_accounts.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.2/scripts/rf_bios_settings.py` & `redfish_utilities-3.1.3/scripts/rf_bios_settings.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.2/scripts/rf_boot_override.py` & `redfish_utilities-3.1.3/scripts/rf_boot_override.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.2/scripts/rf_diagnostic_data.py` & `redfish_utilities-3.1.3/scripts/rf_diagnostic_data.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.2/scripts/rf_discover.py` & `redfish_utilities-3.1.3/scripts/rf_discover.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.2/scripts/rf_event_service.py` & `redfish_utilities-3.1.3/scripts/rf_event_service.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.2/scripts/rf_logs.py` & `redfish_utilities-3.1.3/scripts/rf_logs.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.2/scripts/rf_manager_config.py` & `redfish_utilities-3.1.3/scripts/rf_manager_config.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.2/scripts/rf_power_reset.py` & `redfish_utilities-3.1.3/scripts/rf_power_reset.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.2/scripts/rf_raw_request.py` & `redfish_utilities-3.1.3/scripts/rf_raw_request.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,35 +9,44 @@
 File : rf_raw_request.py
 
 Brief : This script performs a raw request specified by the user
 """
 
 import argparse
 import json
+import os
 import redfish
 
 # Get the input arguments
 argget = argparse.ArgumentParser( description = "A tool perform a raw request to a Redfish service" )
 argget.add_argument( "--user", "-u", type = str, required = True, help = "The user name for authentication" )
 argget.add_argument( "--password", "-p",  type = str, required = True, help = "The password for authentication" )
 argget.add_argument( "--rhost", "-r", type = str, required = True, help = "The address of the Redfish service (with scheme)" )
 argget.add_argument( "--method", "-m", type = str, required = False, help = "The HTTP method to perform; performs GET if not specified", default = "GET", choices = [ "GET", "HEAD", "POST", "PATCH", "PUT", "DELETE" ] )
 argget.add_argument( "--request", "-req", type = str, required = True, help = "The URI for the request" )
-argget.add_argument( "--body", "-b", type = str, required = False, help = "The body to provide with the request" )
+argget.add_argument( "--body", "-b", type = str, required = False, help = "The body to provide with the request; can be a JSON string for a JSON request, a filename to send binary data, or an unstructured string" )
 argget.add_argument( "--verbose", "-v", action = "store_true", help = "Indicates if HTTP response codes and headers are displayed", default = False )
 args = argget.parse_args()
 
 # Connect to the service
 with redfish.redfish_client( base_url = args.rhost, username = args.user, password = args.password ) as redfish_obj:
-    # Encode the body as a dictionary
-    try:
-        body = json.loads( args.body )
-    except:
-        # Not valid JSON; try passing it into the request as a string
-        body = args.body
+    # Encode the body
+    # If the body argument points to a file, load the file
+    if args.body is not None and os.path.isfile( args.body ):
+        with open( args.body, mode="rb" ) as file:
+            body = file.read()
+    else:
+        # Not a file; either JSON or a raw string
+        try:
+            body = json.loads( args.body )
+        except:
+            body = args.body
+    if body is None:
+        # Default case if nothing resolves (empty JSON object)
+        body = {}
 
     # Perform the requested operation
     if args.method == "HEAD":
         resp = redfish_obj.head( args.request )
     elif args.method == "POST":
         resp = redfish_obj.post( args.request, body = body )
     elif args.method == "PATCH":
@@ -53,12 +62,15 @@
     if args.verbose:
         print( "HTTP {}".format( resp.status ) )
         for header in resp.getheaders():
             print( "{}: {}".format( header[0], header[1] ) )
         print()
 
     # Print the response
-    try:
-        print( json.dumps( resp.dict, sort_keys = True, indent = 4, separators = ( ",", ": " ) ) )
-    except:
-        # The response is either malformed JSON or not JSON at all
-        print( resp.text )
+    if resp.status != 204:
+        try:
+            print( json.dumps( resp.dict, sort_keys = True, indent = 4, separators = ( ",", ": " ) ) )
+        except:
+            # The response is either malformed JSON or not JSON at all
+            print( resp.text )
+    else:
+        print( "No response body" )
```

### Comparing `redfish_utilities-3.1.2/scripts/rf_sensor_list.py` & `redfish_utilities-3.1.3/scripts/rf_sensor_list.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.2/scripts/rf_sys_inventory.py` & `redfish_utilities-3.1.3/scripts/rf_sys_inventory.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.2/scripts/rf_update.py` & `redfish_utilities-3.1.3/scripts/rf_update.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.2/scripts/rf_virtual_media.py` & `redfish_utilities-3.1.3/scripts/rf_virtual_media.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.2/setup.py` & `redfish_utilities-3.1.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from codecs import open
 
 with open( "README.md", "r", "utf-8" ) as f:
     long_description = f.read()
 
 setup(
     name = "redfish_utilities",
-    version = "3.1.2",
+    version = "3.1.3",
     description = "Redfish Utilities",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     author = "DMTF, https://www.dmtf.org/standards/feedback",
     license = "BSD 3-clause \"New\" or \"Revised License\"",
     classifiers = [
         "Development Status :: 5 - Production/Stable",
```

