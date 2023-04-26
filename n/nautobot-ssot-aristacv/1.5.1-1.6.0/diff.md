# Comparing `tmp/nautobot_ssot_aristacv-1.5.1.tar.gz` & `tmp/nautobot_ssot_aristacv-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nautobot_ssot_aristacv-1.5.1.tar", max compression
+gzip compressed data, was "nautobot_ssot_aristacv-1.6.0.tar", max compression
```

## Comparing `nautobot_ssot_aristacv-1.5.1.tar` & `nautobot_ssot_aristacv-1.6.0.tar`

### file list

```diff
@@ -1,42 +1,43 @@
--rw-r--r--   0        0        0      591 2023-02-24 17:27:11.921222 nautobot_ssot_aristacv-1.5.1/LICENSE
--rw-r--r--   0        0        0    21422 2023-02-24 17:27:11.921222 nautobot_ssot_aristacv-1.5.1/README.md
--rw-r--r--   0        0        0     2059 2023-02-24 17:27:11.921222 nautobot_ssot_aristacv-1.5.1/nautobot_ssot_aristacv/__init__.py
--rw-r--r--   0        0        0       48 2023-02-24 17:27:11.921222 nautobot_ssot_aristacv-1.5.1/nautobot_ssot_aristacv/api/__init__.py
--rw-r--r--   0        0        0     2932 2023-02-24 17:27:11.921222 nautobot_ssot_aristacv-1.5.1/nautobot_ssot_aristacv/constant.py
--rw-r--r--   0        0        0       86 2023-02-24 17:27:11.921222 nautobot_ssot_aristacv-1.5.1/nautobot_ssot_aristacv/diffsync/adapters/__init__.py
--rw-r--r--   0        0        0    10371 2023-02-24 17:27:11.921222 nautobot_ssot_aristacv-1.5.1/nautobot_ssot_aristacv/diffsync/adapters/cloudvision.py
--rw-r--r--   0        0        0     6248 2023-02-24 17:27:11.921222 nautobot_ssot_aristacv-1.5.1/nautobot_ssot_aristacv/diffsync/adapters/nautobot.py
--rw-r--r--   0        0        0       65 2023-02-24 17:27:11.921222 nautobot_ssot_aristacv-1.5.1/nautobot_ssot_aristacv/diffsync/models/__init__.py
--rw-r--r--   0        0        0     1695 2023-02-24 17:27:11.921222 nautobot_ssot_aristacv-1.5.1/nautobot_ssot_aristacv/diffsync/models/base.py
--rw-r--r--   0        0        0     4926 2023-02-24 17:27:11.921222 nautobot_ssot_aristacv-1.5.1/nautobot_ssot_aristacv/diffsync/models/cloudvision.py
--rw-r--r--   0        0        0    13181 2023-02-24 17:27:11.921222 nautobot_ssot_aristacv-1.5.1/nautobot_ssot_aristacv/diffsync/models/nautobot.py
--rw-r--r--   0        0        0     8370 2023-02-24 17:27:11.921222 nautobot_ssot_aristacv-1.5.1/nautobot_ssot_aristacv/jobs.py
--rw-r--r--   0        0        0        0 2023-02-24 17:27:11.921222 nautobot_ssot_aristacv-1.5.1/nautobot_ssot_aristacv/migrations/__init__.py
--rw-r--r--   0        0        0     5002 2023-02-24 17:27:11.921222 nautobot_ssot_aristacv-1.5.1/nautobot_ssot_aristacv/signals.py
--rw-r--r--   0        0        0    48655 2023-02-24 17:27:11.925222 nautobot_ssot_aristacv-1.5.1/nautobot_ssot_aristacv/static/nautobot_ssot_aristacv/cvp_logo.png
--rw-r--r--   0        0        0       43 2023-02-24 17:27:11.925222 nautobot_ssot_aristacv-1.5.1/nautobot_ssot_aristacv/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-02-24 17:27:11.925222 nautobot_ssot_aristacv-1.5.1/nautobot_ssot_aristacv/tests/fixtures/__init__.py
--rw-r--r--   0        0        0     1361 2023-02-24 17:27:11.925222 nautobot_ssot_aristacv-1.5.1/nautobot_ssot_aristacv/tests/fixtures/fixtures.py
--rw-r--r--   0        0        0      556 2023-02-24 17:27:11.925222 nautobot_ssot_aristacv-1.5.1/nautobot_ssot_aristacv/tests/fixtures/get_devices_response.json
--rw-r--r--   0        0        0     8601 2023-02-24 17:27:11.925222 nautobot_ssot_aristacv-1.5.1/nautobot_ssot_aristacv/tests/fixtures/get_interface_description_client_query.json
--rw-r--r--   0        0        0    16993 2023-02-24 17:27:11.925222 nautobot_ssot_aristacv-1.5.1/nautobot_ssot_aristacv/tests/fixtures/get_interface_transceiver_eeprom_client_query.json
--rw-r--r--   0        0        0     7978 2023-02-24 17:27:11.925222 nautobot_ssot_aristacv-1.5.1/nautobot_ssot_aristacv/tests/fixtures/get_interface_transceiver_local_client_query.json
--rw-r--r--   0        0        0   367495 2023-02-24 17:27:11.925222 nautobot_ssot_aristacv-1.5.1/nautobot_ssot_aristacv/tests/fixtures/get_interfaces_chassis_client_query.json
--rw-r--r--   0        0        0     2805 2023-02-24 17:27:11.925222 nautobot_ssot_aristacv-1.5.1/nautobot_ssot_aristacv/tests/fixtures/get_interfaces_chassis_response.json
--rw-r--r--   0        0        0    21571 2023-02-24 17:27:11.925222 nautobot_ssot_aristacv-1.5.1/nautobot_ssot_aristacv/tests/fixtures/get_interfaces_fixed_client_query.json
--rw-r--r--   0        0        0      195 2023-02-24 17:27:11.925222 nautobot_ssot_aristacv-1.5.1/nautobot_ssot_aristacv/tests/fixtures/get_interfaces_fixed_response.json
--rw-r--r--   0        0        0     6371 2023-02-24 17:27:11.925222 nautobot_ssot_aristacv-1.5.1/nautobot_ssot_aristacv/tests/fixtures/get_ip_interfaces_client_query.json
--rw-r--r--   0        0        0      169 2023-02-24 17:27:11.925222 nautobot_ssot_aristacv-1.5.1/nautobot_ssot_aristacv/tests/fixtures/get_ip_interfaces_response.json
--rw-r--r--   0        0        0      982 2023-02-24 17:27:11.925222 nautobot_ssot_aristacv-1.5.1/nautobot_ssot_aristacv/tests/test_api.py
--rw-r--r--   0        0        0      617 2023-02-24 17:27:11.925222 nautobot_ssot_aristacv-1.5.1/nautobot_ssot_aristacv/tests/test_basic.py
--rw-r--r--   0        0        0     5459 2023-02-24 17:27:11.925222 nautobot_ssot_aristacv-1.5.1/nautobot_ssot_aristacv/tests/test_cloudvision_adapter.py
--rw-r--r--   0        0        0     7547 2023-02-24 17:27:11.925222 nautobot_ssot_aristacv-1.5.1/nautobot_ssot_aristacv/tests/test_jobs.py
--rw-r--r--   0        0        0     2488 2023-02-24 17:27:11.925222 nautobot_ssot_aristacv-1.5.1/nautobot_ssot_aristacv/tests/test_nautobot_adapter.py
--rw-r--r--   0        0        0    14645 2023-02-24 17:27:11.925222 nautobot_ssot_aristacv-1.5.1/nautobot_ssot_aristacv/tests/test_utils_cloudvision.py
--rw-r--r--   0        0        0     8379 2023-02-24 17:27:11.925222 nautobot_ssot_aristacv-1.5.1/nautobot_ssot_aristacv/tests/test_utils_nautobot.py
--rw-r--r--   0        0        0       64 2023-02-24 17:27:11.925222 nautobot_ssot_aristacv-1.5.1/nautobot_ssot_aristacv/utils/__init__.py
--rw-r--r--   0        0        0    25808 2023-02-24 17:27:11.925222 nautobot_ssot_aristacv-1.5.1/nautobot_ssot_aristacv/utils/cloudvision.py
--rw-r--r--   0        0        0     4854 2023-02-24 17:27:11.925222 nautobot_ssot_aristacv-1.5.1/nautobot_ssot_aristacv/utils/nautobot.py
--rw-r--r--   0        0        0     2458 2023-02-24 17:27:22.897322 nautobot_ssot_aristacv-1.5.1/pyproject.toml
--rw-r--r--   0        0        0    23061 1970-01-01 00:00:00.000000 nautobot_ssot_aristacv-1.5.1/setup.py
--rw-r--r--   0        0        0    22627 1970-01-01 00:00:00.000000 nautobot_ssot_aristacv-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0      591 2023-04-26 16:15:40.162519 nautobot_ssot_aristacv-1.6.0/LICENSE
+-rw-r--r--   0        0        0    21422 2023-04-26 16:15:40.162519 nautobot_ssot_aristacv-1.6.0/README.md
+-rw-r--r--   0        0        0     2058 2023-04-26 16:15:40.162519 nautobot_ssot_aristacv-1.6.0/nautobot_ssot_aristacv/__init__.py
+-rw-r--r--   0        0        0       48 2023-04-26 16:15:40.162519 nautobot_ssot_aristacv-1.6.0/nautobot_ssot_aristacv/api/__init__.py
+-rw-r--r--   0        0        0     2932 2023-04-26 16:15:40.162519 nautobot_ssot_aristacv-1.6.0/nautobot_ssot_aristacv/constant.py
+-rw-r--r--   0        0        0       86 2023-04-26 16:15:40.162519 nautobot_ssot_aristacv-1.6.0/nautobot_ssot_aristacv/diffsync/adapters/__init__.py
+-rw-r--r--   0        0        0    10371 2023-04-26 16:15:40.162519 nautobot_ssot_aristacv-1.6.0/nautobot_ssot_aristacv/diffsync/adapters/cloudvision.py
+-rw-r--r--   0        0        0     6248 2023-04-26 16:15:40.162519 nautobot_ssot_aristacv-1.6.0/nautobot_ssot_aristacv/diffsync/adapters/nautobot.py
+-rw-r--r--   0        0        0       65 2023-04-26 16:15:40.162519 nautobot_ssot_aristacv-1.6.0/nautobot_ssot_aristacv/diffsync/models/__init__.py
+-rw-r--r--   0        0        0     1695 2023-04-26 16:15:40.162519 nautobot_ssot_aristacv-1.6.0/nautobot_ssot_aristacv/diffsync/models/base.py
+-rw-r--r--   0        0        0     4926 2023-04-26 16:15:40.162519 nautobot_ssot_aristacv-1.6.0/nautobot_ssot_aristacv/diffsync/models/cloudvision.py
+-rw-r--r--   0        0        0    13181 2023-04-26 16:15:40.162519 nautobot_ssot_aristacv-1.6.0/nautobot_ssot_aristacv/diffsync/models/nautobot.py
+-rw-r--r--   0        0        0     8370 2023-04-26 16:15:40.162519 nautobot_ssot_aristacv-1.6.0/nautobot_ssot_aristacv/jobs.py
+-rw-r--r--   0        0        0        0 2023-04-26 16:15:40.162519 nautobot_ssot_aristacv-1.6.0/nautobot_ssot_aristacv/migrations/__init__.py
+-rw-r--r--   0        0        0     5002 2023-04-26 16:15:40.162519 nautobot_ssot_aristacv-1.6.0/nautobot_ssot_aristacv/signals.py
+-rw-r--r--   0        0        0    48655 2023-04-26 16:15:40.162519 nautobot_ssot_aristacv-1.6.0/nautobot_ssot_aristacv/static/nautobot_ssot_aristacv/cvp_logo.png
+-rw-r--r--   0        0        0       43 2023-04-26 16:15:40.162519 nautobot_ssot_aristacv-1.6.0/nautobot_ssot_aristacv/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-26 16:15:40.162519 nautobot_ssot_aristacv-1.6.0/nautobot_ssot_aristacv/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0     1609 2023-04-26 16:15:40.162519 nautobot_ssot_aristacv-1.6.0/nautobot_ssot_aristacv/tests/fixtures/fixtures.py
+-rw-r--r--   0        0        0      556 2023-04-26 16:15:40.166519 nautobot_ssot_aristacv-1.6.0/nautobot_ssot_aristacv/tests/fixtures/get_devices_response.json
+-rw-r--r--   0        0        0     8601 2023-04-26 16:15:40.166519 nautobot_ssot_aristacv-1.6.0/nautobot_ssot_aristacv/tests/fixtures/get_interface_description_client_query.json
+-rw-r--r--   0        0        0     6918 2023-04-26 16:15:40.166519 nautobot_ssot_aristacv-1.6.0/nautobot_ssot_aristacv/tests/fixtures/get_interface_mode_client_query_access.json
+-rw-r--r--   0        0        0     6952 2023-04-26 16:15:40.166519 nautobot_ssot_aristacv-1.6.0/nautobot_ssot_aristacv/tests/fixtures/get_interface_mode_client_query_trunk.json
+-rw-r--r--   0        0        0    16993 2023-04-26 16:15:40.166519 nautobot_ssot_aristacv-1.6.0/nautobot_ssot_aristacv/tests/fixtures/get_interface_transceiver_eeprom_client_query.json
+-rw-r--r--   0        0        0     7978 2023-04-26 16:15:40.166519 nautobot_ssot_aristacv-1.6.0/nautobot_ssot_aristacv/tests/fixtures/get_interface_transceiver_local_client_query.json
+-rw-r--r--   0        0        0   367495 2023-04-26 16:15:40.166519 nautobot_ssot_aristacv-1.6.0/nautobot_ssot_aristacv/tests/fixtures/get_interfaces_chassis_client_query.json
+-rw-r--r--   0        0        0     2805 2023-04-26 16:15:40.166519 nautobot_ssot_aristacv-1.6.0/nautobot_ssot_aristacv/tests/fixtures/get_interfaces_chassis_response.json
+-rw-r--r--   0        0        0    21571 2023-04-26 16:15:40.166519 nautobot_ssot_aristacv-1.6.0/nautobot_ssot_aristacv/tests/fixtures/get_interfaces_fixed_client_query.json
+-rw-r--r--   0        0        0      195 2023-04-26 16:15:40.166519 nautobot_ssot_aristacv-1.6.0/nautobot_ssot_aristacv/tests/fixtures/get_interfaces_fixed_response.json
+-rw-r--r--   0        0        0     6371 2023-04-26 16:15:40.166519 nautobot_ssot_aristacv-1.6.0/nautobot_ssot_aristacv/tests/fixtures/get_ip_interfaces_client_query.json
+-rw-r--r--   0        0        0      169 2023-04-26 16:15:40.166519 nautobot_ssot_aristacv-1.6.0/nautobot_ssot_aristacv/tests/fixtures/get_ip_interfaces_response.json
+-rw-r--r--   0        0        0      982 2023-04-26 16:15:40.166519 nautobot_ssot_aristacv-1.6.0/nautobot_ssot_aristacv/tests/test_api.py
+-rw-r--r--   0        0        0      617 2023-04-26 16:15:40.166519 nautobot_ssot_aristacv-1.6.0/nautobot_ssot_aristacv/tests/test_basic.py
+-rw-r--r--   0        0        0     5459 2023-04-26 16:15:40.166519 nautobot_ssot_aristacv-1.6.0/nautobot_ssot_aristacv/tests/test_cloudvision_adapter.py
+-rw-r--r--   0        0        0     7547 2023-04-26 16:15:40.166519 nautobot_ssot_aristacv-1.6.0/nautobot_ssot_aristacv/tests/test_jobs.py
+-rw-r--r--   0        0        0     2488 2023-04-26 16:15:40.166519 nautobot_ssot_aristacv-1.6.0/nautobot_ssot_aristacv/tests/test_nautobot_adapter.py
+-rw-r--r--   0        0        0    16284 2023-04-26 16:15:40.166519 nautobot_ssot_aristacv-1.6.0/nautobot_ssot_aristacv/tests/test_utils_cloudvision.py
+-rw-r--r--   0        0        0     8379 2023-04-26 16:15:40.166519 nautobot_ssot_aristacv-1.6.0/nautobot_ssot_aristacv/tests/test_utils_nautobot.py
+-rw-r--r--   0        0        0       64 2023-04-26 16:15:40.166519 nautobot_ssot_aristacv-1.6.0/nautobot_ssot_aristacv/utils/__init__.py
+-rw-r--r--   0        0        0    25704 2023-04-26 16:15:40.166519 nautobot_ssot_aristacv-1.6.0/nautobot_ssot_aristacv/utils/cloudvision.py
+-rw-r--r--   0        0        0     4854 2023-04-26 16:15:40.166519 nautobot_ssot_aristacv-1.6.0/nautobot_ssot_aristacv/utils/nautobot.py
+-rw-r--r--   0        0        0     2429 2023-04-26 16:15:53.794583 nautobot_ssot_aristacv-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0    22520 1970-01-01 00:00:00.000000 nautobot_ssot_aristacv-1.6.0/PKG-INFO
```

### Comparing `nautobot_ssot_aristacv-1.5.1/LICENSE` & `nautobot_ssot_aristacv-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_aristacv-1.5.1/README.md` & `nautobot_ssot_aristacv-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_aristacv-1.5.1/nautobot_ssot_aristacv/__init__.py` & `nautobot_ssot_aristacv-1.6.0/nautobot_ssot_aristacv/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 """Plugin declaration for aristacv_sync."""
+import os
+from django.conf import settings
+from django.db.models.signals import post_migrate
+from nautobot.extras.plugins import PluginConfig
 
 try:
     from importlib import metadata
 except ImportError:
     # Python version < 3.8
     import importlib_metadata as metadata
 
 __version__ = metadata.version(__name__)
 
-import os
-from django.conf import settings
-from django.db.models.signals import post_migrate
-from nautobot.extras.plugins import PluginConfig
-
 
 class NautobotSSOTAristaCVConfig(PluginConfig):
     """Plugin configuration for the nautobot_ssot_aristacv plugin."""
 
     name = "nautobot_ssot_aristacv"
     verbose_name = "Nautobot SSoT Arista CloudVision"
     version = __version__
     author = "Network to Code, LLC"
     description = "Nautobot SSoT Arista CloudVision."
     base_url = "nautobot-sot_aristacv"
     required_settings = []
-    min_version = "1.2.0"
+    min_version = "1.4.0"
     max_version = "1.9999"
     default_settings = {
         "cvp_host": os.getenv("NAUTOBOT_ARISTACV_HOST"),
         "cvp_user": os.getenv("NAUTOBOT_ARISTACV_USERNAME"),
         "cvp_password": os.getenv("NAUTOBOT_ARISTACV_PASSWORD"),
         "verify": os.getenv("NAUTOBOT_ARISTACVP_VERIFY"),
         "cvp_token": os.getenv("NAUTOBOT_ARISTACV_TOKEN"),
```

### Comparing `nautobot_ssot_aristacv-1.5.1/nautobot_ssot_aristacv/constant.py` & `nautobot_ssot_aristacv-1.6.0/nautobot_ssot_aristacv/constant.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_aristacv-1.5.1/nautobot_ssot_aristacv/diffsync/adapters/cloudvision.py` & `nautobot_ssot_aristacv-1.6.0/nautobot_ssot_aristacv/diffsync/adapters/cloudvision.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """DiffSync adapter for Arista CloudVision."""
 from django.conf import settings
 import distutils
 import re
 
-import arista.tag.v1 as TAG
+import arista.tag.v2 as TAG
 from diffsync import DiffSync
 from diffsync.exceptions import ObjectAlreadyExists, ObjectNotFound
 from nautobot_ssot_aristacv.diffsync.models.cloudvision import (
     CloudvisionCustomField,
     CloudvisionDevice,
     CloudvisionPort,
     CloudvisionIPAddress,
```

### Comparing `nautobot_ssot_aristacv-1.5.1/nautobot_ssot_aristacv/diffsync/adapters/nautobot.py` & `nautobot_ssot_aristacv-1.6.0/nautobot_ssot_aristacv/diffsync/adapters/nautobot.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_aristacv-1.5.1/nautobot_ssot_aristacv/diffsync/models/base.py` & `nautobot_ssot_aristacv-1.6.0/nautobot_ssot_aristacv/diffsync/models/base.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_aristacv-1.5.1/nautobot_ssot_aristacv/diffsync/models/cloudvision.py` & `nautobot_ssot_aristacv-1.6.0/nautobot_ssot_aristacv/diffsync/models/cloudvision.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_aristacv-1.5.1/nautobot_ssot_aristacv/diffsync/models/nautobot.py` & `nautobot_ssot_aristacv-1.6.0/nautobot_ssot_aristacv/diffsync/models/nautobot.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_aristacv-1.5.1/nautobot_ssot_aristacv/jobs.py` & `nautobot_ssot_aristacv-1.6.0/nautobot_ssot_aristacv/jobs.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_aristacv-1.5.1/nautobot_ssot_aristacv/signals.py` & `nautobot_ssot_aristacv-1.6.0/nautobot_ssot_aristacv/signals.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_aristacv-1.5.1/nautobot_ssot_aristacv/static/nautobot_ssot_aristacv/cvp_logo.png` & `nautobot_ssot_aristacv-1.6.0/nautobot_ssot_aristacv/static/nautobot_ssot_aristacv/cvp_logo.png`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_aristacv-1.5.1/nautobot_ssot_aristacv/tests/fixtures/fixtures.py` & `nautobot_ssot_aristacv-1.6.0/nautobot_ssot_aristacv/tests/fixtures/fixtures.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,9 +18,13 @@
     "./nautobot_ssot_aristacv/tests/fixtures/get_interface_transceiver_local_client_query.json"
 )
 FIXED_INTERFACE_FIXTURE = load_json("./nautobot_ssot_aristacv/tests/fixtures/get_interfaces_fixed_response.json")
 CHASSIS_INTERFACE_FIXTURE = load_json("./nautobot_ssot_aristacv/tests/fixtures/get_interfaces_chassis_response.json")
 INTF_DESCRIPTION_QUERY = load_json(
     "./nautobot_ssot_aristacv/tests/fixtures/get_interface_description_client_query.json"
 )
+TRUNK_INTF_MODE_QUERY = load_json("./nautobot_ssot_aristacv/tests/fixtures/get_interface_mode_client_query_trunk.json")
+ACCESS_INTF_MODE_QUERY = load_json(
+    "./nautobot_ssot_aristacv/tests/fixtures/get_interface_mode_client_query_access.json"
+)
 IP_INTF_QUERY = load_json("./nautobot_ssot_aristacv/tests/fixtures/get_ip_interfaces_client_query.json")
 IP_INTF_FIXTURE = load_json("./nautobot_ssot_aristacv/tests/fixtures/get_ip_interfaces_response.json")
```

### Comparing `nautobot_ssot_aristacv-1.5.1/nautobot_ssot_aristacv/tests/fixtures/get_devices_response.json` & `nautobot_ssot_aristacv-1.6.0/nautobot_ssot_aristacv/tests/fixtures/get_devices_response.json`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_aristacv-1.5.1/nautobot_ssot_aristacv/tests/fixtures/get_interface_description_client_query.json` & `nautobot_ssot_aristacv-1.6.0/nautobot_ssot_aristacv/tests/fixtures/get_interface_description_client_query.json`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_aristacv-1.5.1/nautobot_ssot_aristacv/tests/fixtures/get_interface_transceiver_eeprom_client_query.json` & `nautobot_ssot_aristacv-1.6.0/nautobot_ssot_aristacv/tests/fixtures/get_interface_transceiver_eeprom_client_query.json`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_aristacv-1.5.1/nautobot_ssot_aristacv/tests/fixtures/get_interface_transceiver_local_client_query.json` & `nautobot_ssot_aristacv-1.6.0/nautobot_ssot_aristacv/tests/fixtures/get_interface_transceiver_local_client_query.json`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_aristacv-1.5.1/nautobot_ssot_aristacv/tests/fixtures/get_interfaces_chassis_client_query.json` & `nautobot_ssot_aristacv-1.6.0/nautobot_ssot_aristacv/tests/fixtures/get_interfaces_chassis_client_query.json`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_aristacv-1.5.1/nautobot_ssot_aristacv/tests/fixtures/get_interfaces_chassis_response.json` & `nautobot_ssot_aristacv-1.6.0/nautobot_ssot_aristacv/tests/fixtures/get_interfaces_chassis_response.json`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_aristacv-1.5.1/nautobot_ssot_aristacv/tests/fixtures/get_interfaces_fixed_client_query.json` & `nautobot_ssot_aristacv-1.6.0/nautobot_ssot_aristacv/tests/fixtures/get_interfaces_fixed_client_query.json`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_aristacv-1.5.1/nautobot_ssot_aristacv/tests/fixtures/get_ip_interfaces_client_query.json` & `nautobot_ssot_aristacv-1.6.0/nautobot_ssot_aristacv/tests/fixtures/get_ip_interfaces_client_query.json`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_aristacv-1.5.1/nautobot_ssot_aristacv/tests/test_api.py` & `nautobot_ssot_aristacv-1.6.0/nautobot_ssot_aristacv/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_aristacv-1.5.1/nautobot_ssot_aristacv/tests/test_basic.py` & `nautobot_ssot_aristacv-1.6.0/nautobot_ssot_aristacv/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_aristacv-1.5.1/nautobot_ssot_aristacv/tests/test_cloudvision_adapter.py` & `nautobot_ssot_aristacv-1.6.0/nautobot_ssot_aristacv/tests/test_cloudvision_adapter.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_aristacv-1.5.1/nautobot_ssot_aristacv/tests/test_jobs.py` & `nautobot_ssot_aristacv-1.6.0/nautobot_ssot_aristacv/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_aristacv-1.5.1/nautobot_ssot_aristacv/tests/test_nautobot_adapter.py` & `nautobot_ssot_aristacv-1.6.0/nautobot_ssot_aristacv/tests/test_nautobot_adapter.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_aristacv-1.5.1/nautobot_ssot_aristacv/tests/test_utils_cloudvision.py` & `nautobot_ssot_aristacv-1.6.0/nautobot_ssot_aristacv/tests/test_utils_cloudvision.py`

 * *Files 7% similar despite different names*

```diff
@@ -104,30 +104,30 @@
 
         mock_tag = MagicMock()
         mock_tag.value.key.label.value = "test"
         mock_tag.value.key.value.value = "test"
         mock_tag.value.creator_type = 1
 
         device_tag_stub = MagicMock()
-        device_tag_stub.DeviceTagServiceStub.return_value.GetAll.return_value = [mock_tag]
+        device_tag_stub.TagServiceStub.return_value.GetAll.return_value = [mock_tag]
 
         with patch("nautobot_ssot_aristacv.utils.cloudvision.tag_services", device_tag_stub):
             results = cloudvision.get_tags_by_type(client=self.client)
         expected = [{"label": "test", "value": "test"}]
         self.assertEqual(results, expected)
 
     def test_get_device_tags(self):
         """Test get_device_tags method."""
         mock_tag = MagicMock()
         mock_tag.value.key.label.value = "ztp"
         mock_tag.value.key.value.value = "enabled"
         mock_tag.value.device_id.value = "JPE12345678"
 
         tag_stub = MagicMock()
-        tag_stub.DeviceTagAssignmentConfigServiceStub.return_value.GetAll.return_value = [mock_tag]
+        tag_stub.TagAssignmentConfigServiceStub.return_value.GetAll.return_value = [mock_tag]
 
         with patch("nautobot_ssot_aristacv.utils.cloudvision.tag_services", tag_stub):
             results = cloudvision.get_device_tags(client=self.client, device_id="JPE12345678")
         expected = [{"label": "ztp", "value": "enabled"}]
         self.assertEqual(results, expected)
 
     def test_unfreeze_frozen_dict(self):
@@ -190,15 +190,14 @@
             self.client.get.return_value = fixtures.FIXED_INTF_QUERY
             results = cloudvision.get_interfaces_fixed(client=self.client, dId="JPE12345678")
         expected = fixtures.FIXED_INTERFACE_FIXTURE
         self.assertEqual(results, expected)
 
     def test_get_interfaces_chassis(self):
         """Test get_interfaces_chassis method."""
-        self.maxDiff = None  # pylint:disable=invalid-name
         mock_query = MagicMock()
         mock_query.dataset.type = "device"
         mock_query.dataset.name = "JPE12345678"
         mock_query.paths.path_elements = [
             "\304\005Sysdb",
             "\304\tinterface",
             "\304\006status",
@@ -260,14 +259,54 @@
             self.client.get = MagicMock()
             self.client.get.return_value = fixtures.TRANSCEIVER_LOCAL_QUERY
             results = cloudvision.get_interface_transceiver(
                 client=self.client, dId="JPE12345678", interface="Ethernet1"
             )
         self.assertEqual(results, "xcvr1000BaseT")
 
+    def test_get_interface_mode_trunk(self):
+        """Test the get_interface_mode method for a trunk."""
+        mock_query = MagicMock()
+        mock_query.dataset.type = "device"
+        mock_query.dataset.name = "JPE12345678"
+        mock_query.paths.path_elements = [
+            "\304\005Sysdb",
+            "\304\010bridging",
+            "\304\020switchIntfConfig",
+            "\304\020switchIntfConfig",
+            "\304\tEthernet1",
+        ]
+
+        with patch("cloudvision.Connector.grpc_client.grpcClient.create_query", mock_query):
+            self.client.get = MagicMock()
+            self.client.get.return_value = fixtures.TRUNK_INTF_MODE_QUERY
+            results = cloudvision.get_interface_mode(client=self.client, dId="JPE12345678", interface="Ethernet1")
+        expected = "trunk"
+        self.assertEqual(results, expected)
+
+    def test_get_interface_mode_access(self):
+        """Test the get_interface_mode method for a access."""
+        mock_query = MagicMock()
+        mock_query.dataset.type = "device"
+        mock_query.dataset.name = "JPE12345678"
+        mock_query.paths.path_elements = [
+            "\304\005Sysdb",
+            "\304\010bridging",
+            "\304\020switchIntfConfig",
+            "\304\020switchIntfConfig",
+            "\304\tEthernet5",
+        ]
+
+        with patch("cloudvision.Connector.grpc_client.grpcClient.create_query", mock_query):
+            self.client.get = MagicMock()
+            self.client.get.return_value = fixtures.ACCESS_INTF_MODE_QUERY
+            results = cloudvision.get_interface_mode(client=self.client, dId="JPE12345678", interface="Ethernet5")
+        expected = "access"
+        self.assertEqual(results, expected)
+
     port_types = [
         ("built_in_gig", {"port_info": {}, "transceiver": "xcvr1000BaseT"}, "1000base-t"),
         ("build_in_10g_sr", {"port_info": {}, "transceiver": "xcvr10GBaseSr"}, "10gbase-x-xfp"),
         ("management_port", {"port_info": {"interface": "Management1"}, "transceiver": "Unknown"}, "1000base-t"),
         ("vlan_port", {"port_info": {"interface": "Vlan100"}, "transceiver": "Unknown"}, "virtual"),
         ("loopback_port", {"port_info": {"interface": "Loopback0"}, "transceiver": "Unknown"}, "virtual"),
         ("port_channel_port", {"port_info": {"interface": "Port-Channel10"}, "transceiver": "Unknown"}, "lag"),
```

### Comparing `nautobot_ssot_aristacv-1.5.1/nautobot_ssot_aristacv/tests/test_utils_nautobot.py` & `nautobot_ssot_aristacv-1.6.0/nautobot_ssot_aristacv/tests/test_utils_nautobot.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_aristacv-1.5.1/nautobot_ssot_aristacv/utils/cloudvision.py` & `nautobot_ssot_aristacv-1.6.0/nautobot_ssot_aristacv/utils/cloudvision.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 from datetime import datetime
 from typing import Any, Iterable, List, Optional, Tuple, Union
 
 import google.protobuf.timestamp_pb2 as pbts
 import grpc
 import requests
 from arista.inventory.v1 import models, services
-from arista.tag.v1 import models as tag_models
-from arista.tag.v1 import services as tag_services
+from arista.tag.v2 import models as tag_models
+from arista.tag.v2 import services as tag_services
+
 from django.conf import settings
 from google.protobuf.wrappers_pb2 import StringValue  # pylint: disable=no-name-in-module
 
 from cvprac.cvp_client import CvpClient
 from cvprac.cvp_client import CvpLoginError
 import cloudvision.Connector.gen.notification_pb2 as ntf
 import cloudvision.Connector.gen.router_pb2 as rtr
@@ -72,15 +73,15 @@
             else:
                 channel_creds = grpc.ssl_channel_credentials(
                     bytes(ssl.get_server_certificate((self.cvp_host, int(self.cvp_port))), "utf-8")
                 )
             if self.cvp_token:
                 call_creds = grpc.access_token_call_credentials(self.cvp_token)
             elif self.username != "" and self.password != "":  # nosec
-                response = requests.post(
+                response = requests.post(  # nosec
                     f"https://{self.cvp_host}/cvpservice/login/authenticate.do",
                     auth=(self.username, self.password),
                     verify=self.verify,
                 )
                 session_id = response.json().get("sessionId")
                 if not session_id:
                     error_code = response.json().get("errorCode")
@@ -288,34 +289,34 @@
         }
         devices.append(device)
     return devices
 
 
 def get_tags_by_type(client, creator_type: int = tag_models.CREATOR_TYPE_USER):
     """Get tags by creator type from CloudVision."""
-    tag_stub = tag_services.DeviceTagServiceStub(client)
-    req = tag_services.DeviceTagStreamRequest(partial_eq_filter=[tag_models.DeviceTag(creator_type=creator_type)])
+    tag_stub = tag_services.TagServiceStub(client)
+    req = tag_services.TagStreamRequest(partial_eq_filter=[tag_models.Tag(creator_type=creator_type)])
     responses = tag_stub.GetAll(req)
     tags = []
     for resp in responses:
         dev_tag = {
             "label": resp.value.key.label.value,
             "value": resp.value.key.value.value,
         }
         tags.append(dev_tag)
     return tags
 
 
 def get_device_tags(client, device_id: str):
     """Get tags for specific device."""
-    tag_stub = tag_services.DeviceTagAssignmentConfigServiceStub(client)
-    req = tag_services.DeviceTagAssignmentConfigStreamRequest(
+    tag_stub = tag_services.TagAssignmentConfigServiceStub(client)
+    req = tag_services.TagAssignmentConfigStreamRequest(
         partial_eq_filter=[
-            tag_models.DeviceTagAssignmentConfig(
-                key=tag_models.DeviceTagAssignmentKey(
+            tag_models.TagAssignmentConfig(
+                key=tag_models.TagAssignmentKey(
                     device_id=StringValue(value=device_id),
                 )
             )
         ]
     )
     responses = tag_stub.GetAll(req)
     tags = []
@@ -326,62 +327,62 @@
         }
         tags.append(dev_tag)
     return tags
 
 
 def create_tag(client, label: str, value: str):
     """Create user-defined tag in CloudVision."""
-    tag_stub = tag_services.DeviceTagConfigServiceStub(client)
-    req = tag_services.DeviceTagConfigSetRequest(
-        value=tag_models.DeviceTagConfig(
+    tag_stub = tag_services.TagConfigServiceStub(client)
+    req = tag_services.TagConfigSetRequest(
+        value=tag_models.TagConfig(
             key=tag_models.TagKey(label=StringValue(value=label), value=StringValue(value=value))
         )
     )
     try:
         tag_stub.Set(req)
     except grpc.RpcError as err:
         # Ignore RPC error if tag already exists for idempotency
         print(f"Failure to create tag: {err}")
         raise err
 
 
 def delete_tag(client, label: str, value: str):
     """Delete user-defined tag in CloudVision."""
-    tag_stub = tag_services.DeviceTagConfigServiceStub(client)
-    req = tag_services.DeviceTagConfigDeleteRequest(
+    tag_stub = tag_services.TagConfigServiceStub(client)
+    req = tag_services.TagConfigDeleteRequest(
         key=tag_models.TagKey(label=StringValue(value=label), value=StringValue(value=value))
     )
     try:
         tag_stub.Delete(req)
     # Skip error of tags that may be assigned to devices manually in CloudVision
     except grpc.RpcError as err:
         print(f"Failure to delete tag: {err}")
         raise err
 
 
 def assign_tag_to_device(client, device_id: str, label: str, value: str):
     """Assign user-defined tag to device in CloudVision."""
-    tag_stub = tag_services.DeviceTagAssignmentConfigServiceStub(client)
-    req = tag_services.DeviceTagAssignmentConfigSetRequest(
-        value=tag_models.DeviceTagAssignmentConfig(
-            key=tag_models.DeviceTagAssignmentKey(
+    tag_stub = tag_services.TagAssignmentConfigServiceStub(client)
+    req = tag_services.TagAssignmentConfigSetRequest(
+        value=tag_models.TagAssignmentConfig(
+            key=tag_models.TagAssignmentKey(
                 label=StringValue(value=label),
                 value=StringValue(value=value),
                 device_id=StringValue(value=device_id),
             )
         )
     )
     tag_stub.Set(req)
 
 
 def remove_tag_from_device(client, device_id: str, label: str, value: str):
     """Unassign a tag from a device in CloudVision."""
-    tag_stub = tag_services.DeviceTagAssignmentConfigServiceStub(client)
-    req = tag_services.DeviceTagAssignmentConfigDeleteRequest(
-        key=tag_models.DeviceTagAssignmentKey(
+    tag_stub = tag_services.TagAssignmentConfigServiceStub(client)
+    req = tag_services.TagAssignmentConfigDeleteRequest(
+        key=tag_models.TagAssignmentKey(
             label=StringValue(value=label),
             value=StringValue(value=value),
             device_id=StringValue(value=device_id),
         )
     )
     tag_stub.Delete(req, timeout=RPC_TIMEOUT)
```

### Comparing `nautobot_ssot_aristacv-1.5.1/nautobot_ssot_aristacv/utils/nautobot.py` & `nautobot_ssot_aristacv-1.6.0/nautobot_ssot_aristacv/utils/nautobot.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_aristacv-1.5.1/pyproject.toml` & `nautobot_ssot_aristacv-1.6.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nautobot-ssot-aristacv"
-version = "v1.5.1"
+version = "v1.6.0"
 description = "Nautobot SSoT Arista CloudVision"
 authors = ["Network to Code, LLC <info@networktocode.com>"]
 
 license = "Apache-2.0"
 
 readme = "README.md"
 homepage = "https://github.com/nautobot/nautobot-plugin-ssot-arista-cloudvision"
@@ -16,18 +16,17 @@
 ]
 packages = [
     { include = "nautobot_ssot_aristacv" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
-nautobot = "^1.2.0"
+nautobot = "^1.4.0"
 nautobot-ssot = "^1.0.1"
-cloudvision = "^1.5.0"
-nautobot-device-lifecycle-mgmt = {version = "^1.0.2", optional = true}
+cloudvision = "^1.9.0"
 cvprac = "^1.2.2"
 
 [tool.poetry.dev-dependencies]
 invoke = "*"
 black = "*"
 django-debug-toolbar = "*"
 yamllint = "*"
@@ -36,14 +35,15 @@
 pylint-django = "*"
 pydocstyle = "*"
 flake8 = "*"
 coverage = "*"
 mkdocs = "*"
 markdown-include = "*"
 parameterized = "^0.8.1"
+nautobot-device-lifecycle-mgmt = "^1.0.2"
 
 [tool.poetry.extras]
 nautobot = ["nautobot"]
 nautobot-device-lifecycle-mgmt = ["nautobot-device-lifecycle-mgmt"]
 
 [tool.black]
 line-length = 120
```

### Comparing `nautobot_ssot_aristacv-1.5.1/setup.py` & `nautobot_ssot_aristacv-1.6.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,44 +1,351 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: nautobot-ssot-aristacv
+Version: 1.6.0
+Summary: Nautobot SSoT Arista CloudVision
+Home-page: https://github.com/nautobot/nautobot-plugin-ssot-arista-cloudvision
+License: Apache-2.0
+Keywords: nautobot,nautobot-plugin
+Author: Network to Code, LLC
+Author-email: info@networktocode.com
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: nautobot
+Provides-Extra: nautobot-device-lifecycle-mgmt
+Requires-Dist: cloudvision (>=1.9.0,<2.0.0)
+Requires-Dist: cvprac (>=1.2.2,<2.0.0)
+Requires-Dist: nautobot (>=1.4.0,<2.0.0) ; extra == "nautobot"
+Requires-Dist: nautobot-ssot (>=1.0.1,<2.0.0)
+Project-URL: Repository, https://github.com/nautobot/nautobot-plugin-ssot-arista-cloudvision
+Description-Content-Type: text/markdown
 
-packages = \
-['nautobot_ssot_aristacv',
- 'nautobot_ssot_aristacv.api',
- 'nautobot_ssot_aristacv.diffsync.adapters',
- 'nautobot_ssot_aristacv.diffsync.models',
- 'nautobot_ssot_aristacv.migrations',
- 'nautobot_ssot_aristacv.tests',
- 'nautobot_ssot_aristacv.tests.fixtures',
- 'nautobot_ssot_aristacv.utils']
-
-package_data = \
-{'': ['*'], 'nautobot_ssot_aristacv': ['static/nautobot_ssot_aristacv/*']}
-
-install_requires = \
-['cloudvision>=1.5.0,<2.0.0',
- 'cvprac>=1.2.2,<2.0.0',
- 'nautobot-ssot>=1.0.1,<2.0.0']
-
-extras_require = \
-{':extra == "nautobot"': ['nautobot>=1.2.0,<2.0.0'],
- 'nautobot-device-lifecycle-mgmt': ['nautobot-device-lifecycle-mgmt>=1.0.2,<2.0.0']}
-
-setup_kwargs = {
-    'name': 'nautobot-ssot-aristacv',
-    'version': '1.5.1',
-    'description': 'Nautobot SSoT Arista CloudVision',
-    'long_description': '# Nautobot to Arista CloudVision Sync\n\nA plugin for [Nautobot](https://github.com/nautobot/nautobot) that allows synchronization of data directly between CloudVision and Nautobot. From Nautobot into CloudVision, it synchronizes user device tags. From CloudVision into Nautobot, it synchronizes devices, their interfaces, associated IP addresses, and their system tags. Here is a table showing the data mappings when syncing from CloudVision.\n\n| CloudVision System Tags | Nautobot Device Custom Field |\n| ----------------------- | ---------------------------- |\n| topology_network_type   | Topology Network Type        |\n| mlag                    | mlag                         |\n| mpls                    | mpls                         |\n| model                   | Device Type*                 |\n| systype                 | systype                      |\n| serialnumber            | Device Serial Number         |\n| pimbidir                | pimbidir                     |\n| sflow                   | sFlow                        |\n| eostrain                | EOS Train                    |\n| tapagg                  | TAP Aggregation              |\n| pim                     | pim                          |\n| bgp                     | bgp                          |\n| terminattr              | TerminAttr Version           |\n| ztp                     | ztp                          |\n| eos                     | EOS Version**                |\n| topology_type           | Topology Type                |\n> *The model system tag is mapped to the device type model in Nautobot.\n\n> **If the [Device Lifecycle plug-in](https://github.com/nautobot/nautobot-plugin-device-lifecycle-mgmt) is found to be installed, a matching Version will be created with a RelationshipAssociation connecting the device and that Version.\n\nWhen syncing User tags from Nautobot to CloudVision the data mappings are as follows:\n\n| Nautobot   | CloudVision   |\n| ---------- | ------------- |\n| Interface  | Interface     |\n| ---------- | ------------- |\n| Tags       | Device Tags   |\n\n> This plugin is an extension of the [Nautobot Single Source of Truth (SSoT)](https://github.com/nautobot/nautobot-plugin-ssot) and you must have that plugin installed before installing this extension.\n\n## Screenshots\n\nThis screenshot shows the CloudVision to Nautobot home page. This contains a list of all the system tags from CloudVision and how they map to custom fields in Nautobot. This also displays your plugin configuration and the sync history.\n\n![cv_to_naut](https://user-images.githubusercontent.com/38091261/124859726-03557800-df76-11eb-9622-af4c29ba8d40.PNG)\n\nThis screenshot shows the Nautobot to CloudVision home page. It also contains data mappings, plugin configuration and sync history.\n\n![naut_to_cv](https://user-images.githubusercontent.com/38091261/124859903-55969900-df76-11eb-87c4-64ca2616bffe.PNG)\n\n## Installation\n\nThe plugin is available as a Python package in PyPI and can be installed with pip\n\n```shell\npip install nautobot_ssot_aristacv\n```\n\n> The plugin is compatible with Nautobot 1.0.0 and higher\n\nTo ensure Nautobot to Arista CloudVision Sync is automatically re-installed during future upgrades, create a file named `local_requirements.txt` (if not already existing) in the Nautobot root directory (alongside `requirements.txt`) and list the `nautobot_ssot_aristacv` package:\n\n```no-highlight\n# echo nautobot_ssot_aristacv >> local_requirements.txt\n```\n\nOnce installed, the plugin needs to be enabled in your `nautobot_configuration.py` and plugin settings need to be defined.\n\n```python\n# In your configuration.py\nPLUGINS = ["nautobot_ssot", "nautobot_ssot_aristacv"]\n\nPLUGINS_CONFIG = {\n  "nautobot_ssot" : {\n    "hide_example_jobs": True,\n  },\n  "nautobot_ssot_aristacv": {\n    "cvp_token": os.getenv("NAUTOBOT_ARISTACV_TOKEN", ""),\n    "cvp_host": os.getenv("NAUTOBOT_ARISTACV_HOST", ""),\n    "cvp_port": os.getenv("NAUTOBOT_ARISTACV_PORT", 443),\n    "cvp_user": os.getenv("NAUTOBOT_ARISTACV_USERNAME", ""),\n    "cvp_password": os.getenv("NAUTOBOT_ARISTACV_PASSWORD", ""),\n    "verify": is_truthy(os.getenv("NAUTOBOT_ARISTACV_VERIFY", True)),\n    "from_cloudvision_default_site": "",\n    "from_cloudvision_default_device_role": "",\n    "from_cloudvision_default_device_role_color": "",\n    "delete_devices_on_sync": is_truthy(os.getenv("NAUTOBOT_ARISTACV_DELETE_ON_SYNC", False)),\n    "apply_import_tag": is_truthy(os.getenv("NAUTOBOT_ARISTACV_IMPORT_TAG", False)),\n    "import_active": is_truthy(os.getenv("NAUTOBOT_ARISTACV_IMPORT_ACTIVE", False)),\n    "create_controller": is_truthy(os.getenv("NAUTOBOT_ARISTACV_CREATE_CONTROLLER", False)),\n    "controller_site": os.getenv("NAUTOBOT_ARISTACV_CONTROLLER_SITE", ""),\n    "hostname_patterns": [""],\n    "site_mappings": {},\n    "role_mappings": {},\n  }\n}\n```\n\n> All plugin settings are defined in the picture above as an example. Only some will be needed as described below.\n\nUpon installation, this plugin creates the following custom fields in Nautobot:\n\n- `arista_bgp`\n- `arista_eos`\n- `arista_eostrain`\n- `arista_mlag`\n- `arista_mpls`\n- `arista_pim`\n- `arista_pimbidir`\n- `arista_sflow`\n- `arista_systype`\n- `arista_tapagg`\n- `arista_terminattr`\n- `arista_topology_network_type`\n- `arista_topology_type`\n- `arista_ztp`\n\n> While these contain the prefix "arista" in the custom field admin portal, when looking at them on a device the prefix is removed.\n\nOther custom fields may need to be created by the user. When a sync is run and a system tag for a device in CloudVision is found without a corresponding custom field, the sync log will display a message. To have that data synced, a custom field must be created in the Admin UI using the given name in the message.\n\n![Custom_Fields_Arista](https://user-images.githubusercontent.com/38091261/133857343-94ee262c-87ca-4e64-a3b2-c3d410755098.PNG)\n\nThe plugin can connect to either on-premise or a cloud instance of CloudVision. To connect to an on-premise instance, you must set the following variables in the Nautobot configuration file.\n\n| Configuration Variable | Type    | Usage                                                                                            |\n| ---------------------- | ------- | ------------------------------------------------------------------------------------------------ |\n| cvp_host               | string  | Hostname or ip address of the onprem instance of CloudVision.                                    |\n| cvp_port               | string  | gRPC port (defaults to 8443, but this port has changed to 443 as of CVP 2021.3.0)                |\n| cvp_user               | string  | The username used to connect to the on-prem instance of CloudVision.                             |\n| cvp_password           | string  | The password used by the user specified above.                                                   |\n| cvp_token              | string  | Token to be used when connecting to CloudVision.                                                 |\n| verify                 | boolean | If False, the plugin will download the certificate from CloudVision and trust it for gRPC calls. |\n\nTo connect to a cloud instance of CloudVision you must set the following variable:\n\n| Configuration Variable | Type   | Usage                                       | Default           |\n| ---------------------- | ------ | ------------------------------------------- | ----------------- |\n| cvaas_url              | string | URL used to connect to your CvaaS instance. | www.arista.io:443 |\n\nWhen syncing from CloudVision, this plugin will create new Arista devices that do not exist in Nautobot. When creating new devices in Nautobot, a site, device role, device role color, device status, and device are required. You may define which values to use by configuring the following values in your `nautobot_config.py` file. If you define a `default_device_role` and `default_device_status` that already exist, the default color value for both of those will be ignored as it will pull that information from Nautobot.\n\n| Configuration Variable                     | Type   | Usage                                                      | Default              |\n| ------------------------------------------ | ------ | ---------------------------------------------------------- | -------------------- |\n| from_cloudvision_default_site              | string | Default site created when syncing new devices to Nautobot. | cloudvision_imported |\n| from_cloudvision_default_device_role       | string | Default role created when syncing new devices to Nautobot. | network              |\n| from_cloudvision_default_device_role_color | string | Default role color used for default role.                  | ff0000               |\n\n> When these variables are not defined in the plugin settings, the plugin will use the default values mentioned.\n\nWhen an Arista device exists in Nautobot but not in CloudVision, this plugin can either delete or leave the device in Nautobot. That behavior can be set with the following variable in the `nautobot_config.py` file.\n\n| Configuration Variable | Type    | Usage                                                                                                                                                              | Default |\n| ---------------------- | ------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------- |\n| delete_devices_on_sync | boolean | If true, devices in Nautobot with device type manufacturer name set to Arista that do not exist in CloudVision but do exist in Nautobot upon sync will be deleted. | False   |\n\n> When this variable is not defined in the plugin settings, the plugin will default to using `False`.\n\nOptionally, an import tag with the name `cloudvision_imported` can be applied to devices that are imported from CloudVision.\n\n| Configuration Variable | Type    | Usage                                                  | Default |\n| ---------------------- | ------- | ------------------------------------------------------ | ------- |\n| apply_import_tag       | boolean | Apply import tag to devices imported from CloudVision. | False   |\n\n> If apply_import_tag is set to True, the tag value that is applied to devices is `cloudvision_imported`.\n\nIn addition, you can control whether only active devices are imported or whether all devices regardless of status are imported.\n\n| Configuration Variable | Type    | Usage                                        | Default |\n| ---------------------- | ------- | -------------------------------------------- | ------- |\n| import_active          | boolean | Only import active devices from CloudVision. | False   |\n\nThere is also the option of having your CloudVision instance created within Nautobot and linked to the Devices managed by the instance. If the `create_controller` setting is `True` then a CloudVision Device will be created and Relationships created to the imported Devices from CVP. The `controller_site` setting allows you to specify the name of the Site you wish the Device to be created in. If this setting is blank a new CloudVision Site will be created and the Device will be placed in it.\n\n| Configuration Variable | Type    | Usage                                         | Default |\n| ---------------------- | ------- | --------------------------------------------- | ------- |\n| create_controller      | boolean | Create CloudVision Device in Nautobot.        | False   |\n| controller_site        | string  | The Site to associate with CloudVision Device.| ""      |\n\nFinally, there is the option to parse device hostname\'s for codes that indicate the assigned site or device role. This is done through a combination of a few settings. First, the hostname_patterns setting defines a list of regex patterns that define your hostname structure. These patterns must include a named capture group using the `site` and `role` key to identify the portion of the hostname that indicates those pieces of data, ie `(?P<site>\\w+)` and `(?P<role>\\w+)`. Once those pieces are extracted they are then evaluated against the relevant map, ie the value for the `site` capture group is looked for in the `site_mappings` dictionary expecting the value to be a key with the map value being the name of the Site. If the Site doesn\'t exist it will be created in Staging status. For the Device Role, it will be created if it doesn\'t exist in Nautobot. Please note that the hostname is converted to all lowercase when the parsing is performed so the keys are expected to be all lowercase too.\n\n| Configuration Variable                       | Type    | Usage                                                      | Default              |\n|----------------------------------------------|---------|------------------------------------------------------------|----------------------|\n| hostname_patterns                            |List[str]| Define the portions of a hostname that indicate site/role. | []                   |\n| site_mappings                                |  dict   | Define the site name associated with code in hostname.     | {}                   |\n| role_mappings                                |  dict   | Define the role name associated with code in hostname.     | {}                   |\n\n> As the Device hostname is used as the identifier for Device objects any change in hostname implies a new Device and thus should trigger a deletion and creation of a new Device in Nautobot. For this reason, the hostname parsing feature is not done during updates and only at initial creation of the Device. If you need to correct the Site or Role for a Device after initial creation you will need to manually correct it or delete it and run the import Job again.\n\n## Usage\n\nThis extension can sync data both `to` and `from` Nautobot. Once the plugin has been installed successfully two new options are available under the [Nautobot Single Source of Truth (SSoT)](https://github.com/nautobot/nautobot-plugin-ssot) plugin.\n\n![Arista Extension](https://user-images.githubusercontent.com/38091261/124857275-9a6c0100-df71-11eb-8ace-2ddf67a2471f.PNG)\n\nPlease be aware that interfaces that are part of a breakout bundle, ie a 40G port broken out into 4x10G ports, will show the base interface SFP transceiver as the interface type. This is due to the way interfaces and transceivers are returned from CloudVision.\n\n### Syncing From CloudVision\n\n> When loading Nautobot data, this tool only loads devices with a device type that has a manufacturer of "Arista"\n\nWhen syncing data from CloudVision to Nautobot, devices along with their interfaces and tags are synchronized.  When a device exists in CloudVision that doesn\'t exist in Nautobot, this tool creates the device in Nautobot with the default values specified in the configuration file. When a device exists in Nautobot that does not exist in CloudVision, this tool can be configured to either delete or skip that device.\nYou can watch the below video for an example.\n\n![fromcv_sync](https://user-images.githubusercontent.com/38091261/126499331-e41946c4-4e61-4b5e-8b7f-73efb9cd8d3f.gif)\n\nWhen syncing data from Nautobot to CloudVision, the tag data in Nautobot is copied into User Tags in CloudVision. You can watch the video below for an example.\n\n![tocv_sync](https://user-images.githubusercontent.com/38091261/126499484-2e4c4feb-0492-4dc6-abb6-a092701c81ed.gif)\n\n## Contributing\n\nPull requests are welcomed and automatically built and tested against multiple versions of Python and multiple versions of Nautobot through GitHub Actions.\n\nThe project is packaged with a light development environment based on `docker-compose` to help with the local development of the project and to run the tests within a Docker container.\n\nThe project is following Network to Code software development guidelines and is leveraging:\n\n- Black, Pylint, Bandit and pydocstyle for Python linting and formatting.\n- Django unit test to ensure the plugin is working properly.\n\n### Development Environment\n\nThe development environment can be used in 2 ways. First, with a local poetry environment if you wish to develop outside of Docker. Second, inside of a docker container.\n\n#### Invoke tasks\n\nThe [PyInvoke](http://www.pyinvoke.org/) library is used to provide some helper commands based on the environment.  There are a few configuration parameters that can be passed to PyInvoke to override the default configuration:\n\n- `nautobot_ver`: the version of Nautobot to use as a base for any built docker containers (default: develop-latest)\n- `project_name`: the default docker compose project name (default: aristacv-sync)\n- `python_ver`: the version of Python to use as a base for any built docker containers (default: 3.6)\n- `local`: a boolean flag indicating if invoke tasks should be run on the host or inside the docker containers (default: False, commands will be run in docker containers)\n- `compose_dir`: the full path to a directory containing the project compose files\n- `compose_files`: a list of compose files applied in order (see [Multiple Compose files](https://docs.docker.com/compose/extends/#multiple-compose-files) for more information)\n\nUsing PyInvoke these configuration options can be overridden using [several methods](http://docs.pyinvoke.org/en/stable/concepts/configuration.html).  Perhaps the simplest is simply setting an environment variable `INVOKE_ARISTACV-SYNC_VARIABLE_NAME` where `VARIABLE_NAME` is the variable you are trying to override.  The only exception is `compose_files`, because it is a list it must be overridden in a YAML file.  There is an example `invoke.yml` in this directory which can be used as a starting point.\n\n#### Local Poetry Development Environment\n\n1. Copy `development/creds.example.env` to `development/creds.env` (This file will be ignored by git and docker)\n2. Uncomment the `POSTGRES_HOST`, `REDIS_HOST`, and `NAUTOBOT_ROOT` variables in `development/creds.env`\n3. Create an invoke.yml with the following contents at the root of the repo:\n\n```shell\n---\naristacv_sync:\n  local: true\n  compose_files:\n    - "docker-compose.requirements.yml"\n```\n\n4. Run the following commands:\n\n```shell\npoetry shell\npoetry install\nexport $(cat development/dev.env | xargs)\nexport $(cat development/creds.env | xargs)\n```\n\n5. You can now run nautobot-server commands as you would from the [Nautobot documentation](https://nautobot.readthedocs.io/en/latest/) for example to start the development server:\n\n```shell\nnautobot-server runserver 0.0.0.0:8080 --insecure\n```\n\nNautobot server can now be accessed at [http://localhost:8080](http://localhost:8080).\n\n#### Docker Development Environment\n\nThis project is managed by [Python Poetry](https://python-poetry.org/) and has a few requirements to setup your development environment:\n\n1. Install Poetry, see the [Poetry Documentation](https://python-poetry.org/docs/#installation) for your operating system.\n2. Install Docker, see the [Docker documentation](https://docs.docker.com/get-docker/) for your operating system.\n\nOnce you have Poetry and Docker installed you can run the following commands to install all other development dependencies in an isolated python virtual environment:\n\n```shell\npoetry shell\npoetry install\ninvoke start\n```\n\nNautobot server can now be accessed at [http://localhost:8080](http://localhost:8080).\n\n### CLI Helper Commands\n\nThe project is coming with a CLI helper based on [invoke](http://www.pyinvoke.org/) to help set up the development environment. The commands are listed below in 3 categories `dev environment`, `utility` and `testing`.\n\nEach command can be executed with `invoke <command>`. Environment variables `INVOKE_ARISTACV-SYNC_PYTHON_VER` and `INVOKE_ARISTACV-SYNC_NAUTOBOT_VER` may be specified to override the default versions. Each command also has its own help `invoke <command> --help`\n\n#### Docker dev environment\n\n```no-highlight\n  build            Build all docker images.\n  debug            Start Nautobot and its dependencies in debug mode.\n  destroy          Destroy all containers and volumes.\n  restart          Restart Nautobot and its dependencies.\n  start            Start Nautobot and its dependencies in detached mode.\n  stop             Stop Nautobot and its dependencies.\n```\n\n#### Utility\n\n```no-highlight\n  cli              Launch a bash shell inside the running Nautobot container.\n  create-user      Create a new user in django (default: admin), will prompt for password.\n  makemigrations   Run Make Migration in Django.\n  nbshell          Launch a nbshell session.\n```\n\n#### Testing\n\n```no-highlight\n  bandit           Run bandit to validate basic static code security analysis.\n  black            Run black to check that Python files adhere to its style standards.\n  flake8           This will run flake8 for the specified name and Python version.\n  pydocstyle       Run pydocstyle to validate docstring formatting adheres to NTC defined standards.\n  pylint           Run pylint code analysis.\n  tests            Run all tests for this plugin.\n  unittest         Run Django unit tests for the plugin.\n```\n\n## Questions\n\nFor any questions or comments, please check the [FAQ](FAQ.md) first and feel free to swing by the [Network to Code slack channel](https://networktocode.slack.com/) (channel #networktocode).\nSign up [here](http://slack.networktocode.com/)\n',
-    'author': 'Network to Code, LLC',
-    'author_email': 'info@networktocode.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/nautobot/nautobot-plugin-ssot-arista-cloudvision',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.7,<4.0',
+# Nautobot to Arista CloudVision Sync
+
+A plugin for [Nautobot](https://github.com/nautobot/nautobot) that allows synchronization of data directly between CloudVision and Nautobot. From Nautobot into CloudVision, it synchronizes user device tags. From CloudVision into Nautobot, it synchronizes devices, their interfaces, associated IP addresses, and their system tags. Here is a table showing the data mappings when syncing from CloudVision.
+
+| CloudVision System Tags | Nautobot Device Custom Field |
+| ----------------------- | ---------------------------- |
+| topology_network_type   | Topology Network Type        |
+| mlag                    | mlag                         |
+| mpls                    | mpls                         |
+| model                   | Device Type*                 |
+| systype                 | systype                      |
+| serialnumber            | Device Serial Number         |
+| pimbidir                | pimbidir                     |
+| sflow                   | sFlow                        |
+| eostrain                | EOS Train                    |
+| tapagg                  | TAP Aggregation              |
+| pim                     | pim                          |
+| bgp                     | bgp                          |
+| terminattr              | TerminAttr Version           |
+| ztp                     | ztp                          |
+| eos                     | EOS Version**                |
+| topology_type           | Topology Type                |
+> *The model system tag is mapped to the device type model in Nautobot.
+
+> **If the [Device Lifecycle plug-in](https://github.com/nautobot/nautobot-plugin-device-lifecycle-mgmt) is found to be installed, a matching Version will be created with a RelationshipAssociation connecting the device and that Version.
+
+When syncing User tags from Nautobot to CloudVision the data mappings are as follows:
+
+| Nautobot   | CloudVision   |
+| ---------- | ------------- |
+| Interface  | Interface     |
+| ---------- | ------------- |
+| Tags       | Device Tags   |
+
+> This plugin is an extension of the [Nautobot Single Source of Truth (SSoT)](https://github.com/nautobot/nautobot-plugin-ssot) and you must have that plugin installed before installing this extension.
+
+## Screenshots
+
+This screenshot shows the CloudVision to Nautobot home page. This contains a list of all the system tags from CloudVision and how they map to custom fields in Nautobot. This also displays your plugin configuration and the sync history.
+
+![cv_to_naut](https://user-images.githubusercontent.com/38091261/124859726-03557800-df76-11eb-9622-af4c29ba8d40.PNG)
+
+This screenshot shows the Nautobot to CloudVision home page. It also contains data mappings, plugin configuration and sync history.
+
+![naut_to_cv](https://user-images.githubusercontent.com/38091261/124859903-55969900-df76-11eb-87c4-64ca2616bffe.PNG)
+
+## Installation
+
+The plugin is available as a Python package in PyPI and can be installed with pip
+
+```shell
+pip install nautobot_ssot_aristacv
+```
+
+> The plugin is compatible with Nautobot 1.0.0 and higher
+
+To ensure Nautobot to Arista CloudVision Sync is automatically re-installed during future upgrades, create a file named `local_requirements.txt` (if not already existing) in the Nautobot root directory (alongside `requirements.txt`) and list the `nautobot_ssot_aristacv` package:
+
+```no-highlight
+# echo nautobot_ssot_aristacv >> local_requirements.txt
+```
+
+Once installed, the plugin needs to be enabled in your `nautobot_configuration.py` and plugin settings need to be defined.
+
+```python
+# In your configuration.py
+PLUGINS = ["nautobot_ssot", "nautobot_ssot_aristacv"]
+
+PLUGINS_CONFIG = {
+  "nautobot_ssot" : {
+    "hide_example_jobs": True,
+  },
+  "nautobot_ssot_aristacv": {
+    "cvp_token": os.getenv("NAUTOBOT_ARISTACV_TOKEN", ""),
+    "cvp_host": os.getenv("NAUTOBOT_ARISTACV_HOST", ""),
+    "cvp_port": os.getenv("NAUTOBOT_ARISTACV_PORT", 443),
+    "cvp_user": os.getenv("NAUTOBOT_ARISTACV_USERNAME", ""),
+    "cvp_password": os.getenv("NAUTOBOT_ARISTACV_PASSWORD", ""),
+    "verify": is_truthy(os.getenv("NAUTOBOT_ARISTACV_VERIFY", True)),
+    "from_cloudvision_default_site": "",
+    "from_cloudvision_default_device_role": "",
+    "from_cloudvision_default_device_role_color": "",
+    "delete_devices_on_sync": is_truthy(os.getenv("NAUTOBOT_ARISTACV_DELETE_ON_SYNC", False)),
+    "apply_import_tag": is_truthy(os.getenv("NAUTOBOT_ARISTACV_IMPORT_TAG", False)),
+    "import_active": is_truthy(os.getenv("NAUTOBOT_ARISTACV_IMPORT_ACTIVE", False)),
+    "create_controller": is_truthy(os.getenv("NAUTOBOT_ARISTACV_CREATE_CONTROLLER", False)),
+    "controller_site": os.getenv("NAUTOBOT_ARISTACV_CONTROLLER_SITE", ""),
+    "hostname_patterns": [""],
+    "site_mappings": {},
+    "role_mappings": {},
+  }
 }
+```
+
+> All plugin settings are defined in the picture above as an example. Only some will be needed as described below.
+
+Upon installation, this plugin creates the following custom fields in Nautobot:
+
+- `arista_bgp`
+- `arista_eos`
+- `arista_eostrain`
+- `arista_mlag`
+- `arista_mpls`
+- `arista_pim`
+- `arista_pimbidir`
+- `arista_sflow`
+- `arista_systype`
+- `arista_tapagg`
+- `arista_terminattr`
+- `arista_topology_network_type`
+- `arista_topology_type`
+- `arista_ztp`
+
+> While these contain the prefix "arista" in the custom field admin portal, when looking at them on a device the prefix is removed.
+
+Other custom fields may need to be created by the user. When a sync is run and a system tag for a device in CloudVision is found without a corresponding custom field, the sync log will display a message. To have that data synced, a custom field must be created in the Admin UI using the given name in the message.
+
+![Custom_Fields_Arista](https://user-images.githubusercontent.com/38091261/133857343-94ee262c-87ca-4e64-a3b2-c3d410755098.PNG)
+
+The plugin can connect to either on-premise or a cloud instance of CloudVision. To connect to an on-premise instance, you must set the following variables in the Nautobot configuration file.
+
+| Configuration Variable | Type    | Usage                                                                                            |
+| ---------------------- | ------- | ------------------------------------------------------------------------------------------------ |
+| cvp_host               | string  | Hostname or ip address of the onprem instance of CloudVision.                                    |
+| cvp_port               | string  | gRPC port (defaults to 8443, but this port has changed to 443 as of CVP 2021.3.0)                |
+| cvp_user               | string  | The username used to connect to the on-prem instance of CloudVision.                             |
+| cvp_password           | string  | The password used by the user specified above.                                                   |
+| cvp_token              | string  | Token to be used when connecting to CloudVision.                                                 |
+| verify                 | boolean | If False, the plugin will download the certificate from CloudVision and trust it for gRPC calls. |
+
+To connect to a cloud instance of CloudVision you must set the following variable:
+
+| Configuration Variable | Type   | Usage                                       | Default           |
+| ---------------------- | ------ | ------------------------------------------- | ----------------- |
+| cvaas_url              | string | URL used to connect to your CvaaS instance. | www.arista.io:443 |
+
+When syncing from CloudVision, this plugin will create new Arista devices that do not exist in Nautobot. When creating new devices in Nautobot, a site, device role, device role color, device status, and device are required. You may define which values to use by configuring the following values in your `nautobot_config.py` file. If you define a `default_device_role` and `default_device_status` that already exist, the default color value for both of those will be ignored as it will pull that information from Nautobot.
+
+| Configuration Variable                     | Type   | Usage                                                      | Default              |
+| ------------------------------------------ | ------ | ---------------------------------------------------------- | -------------------- |
+| from_cloudvision_default_site              | string | Default site created when syncing new devices to Nautobot. | cloudvision_imported |
+| from_cloudvision_default_device_role       | string | Default role created when syncing new devices to Nautobot. | network              |
+| from_cloudvision_default_device_role_color | string | Default role color used for default role.                  | ff0000               |
+
+> When these variables are not defined in the plugin settings, the plugin will use the default values mentioned.
+
+When an Arista device exists in Nautobot but not in CloudVision, this plugin can either delete or leave the device in Nautobot. That behavior can be set with the following variable in the `nautobot_config.py` file.
+
+| Configuration Variable | Type    | Usage                                                                                                                                                              | Default |
+| ---------------------- | ------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------- |
+| delete_devices_on_sync | boolean | If true, devices in Nautobot with device type manufacturer name set to Arista that do not exist in CloudVision but do exist in Nautobot upon sync will be deleted. | False   |
+
+> When this variable is not defined in the plugin settings, the plugin will default to using `False`.
+
+Optionally, an import tag with the name `cloudvision_imported` can be applied to devices that are imported from CloudVision.
+
+| Configuration Variable | Type    | Usage                                                  | Default |
+| ---------------------- | ------- | ------------------------------------------------------ | ------- |
+| apply_import_tag       | boolean | Apply import tag to devices imported from CloudVision. | False   |
+
+> If apply_import_tag is set to True, the tag value that is applied to devices is `cloudvision_imported`.
+
+In addition, you can control whether only active devices are imported or whether all devices regardless of status are imported.
+
+| Configuration Variable | Type    | Usage                                        | Default |
+| ---------------------- | ------- | -------------------------------------------- | ------- |
+| import_active          | boolean | Only import active devices from CloudVision. | False   |
+
+There is also the option of having your CloudVision instance created within Nautobot and linked to the Devices managed by the instance. If the `create_controller` setting is `True` then a CloudVision Device will be created and Relationships created to the imported Devices from CVP. The `controller_site` setting allows you to specify the name of the Site you wish the Device to be created in. If this setting is blank a new CloudVision Site will be created and the Device will be placed in it.
+
+| Configuration Variable | Type    | Usage                                         | Default |
+| ---------------------- | ------- | --------------------------------------------- | ------- |
+| create_controller      | boolean | Create CloudVision Device in Nautobot.        | False   |
+| controller_site        | string  | The Site to associate with CloudVision Device.| ""      |
+
+Finally, there is the option to parse device hostname's for codes that indicate the assigned site or device role. This is done through a combination of a few settings. First, the hostname_patterns setting defines a list of regex patterns that define your hostname structure. These patterns must include a named capture group using the `site` and `role` key to identify the portion of the hostname that indicates those pieces of data, ie `(?P<site>\w+)` and `(?P<role>\w+)`. Once those pieces are extracted they are then evaluated against the relevant map, ie the value for the `site` capture group is looked for in the `site_mappings` dictionary expecting the value to be a key with the map value being the name of the Site. If the Site doesn't exist it will be created in Staging status. For the Device Role, it will be created if it doesn't exist in Nautobot. Please note that the hostname is converted to all lowercase when the parsing is performed so the keys are expected to be all lowercase too.
+
+| Configuration Variable                       | Type    | Usage                                                      | Default              |
+|----------------------------------------------|---------|------------------------------------------------------------|----------------------|
+| hostname_patterns                            |List[str]| Define the portions of a hostname that indicate site/role. | []                   |
+| site_mappings                                |  dict   | Define the site name associated with code in hostname.     | {}                   |
+| role_mappings                                |  dict   | Define the role name associated with code in hostname.     | {}                   |
+
+> As the Device hostname is used as the identifier for Device objects any change in hostname implies a new Device and thus should trigger a deletion and creation of a new Device in Nautobot. For this reason, the hostname parsing feature is not done during updates and only at initial creation of the Device. If you need to correct the Site or Role for a Device after initial creation you will need to manually correct it or delete it and run the import Job again.
+
+## Usage
+
+This extension can sync data both `to` and `from` Nautobot. Once the plugin has been installed successfully two new options are available under the [Nautobot Single Source of Truth (SSoT)](https://github.com/nautobot/nautobot-plugin-ssot) plugin.
+
+![Arista Extension](https://user-images.githubusercontent.com/38091261/124857275-9a6c0100-df71-11eb-8ace-2ddf67a2471f.PNG)
+
+Please be aware that interfaces that are part of a breakout bundle, ie a 40G port broken out into 4x10G ports, will show the base interface SFP transceiver as the interface type. This is due to the way interfaces and transceivers are returned from CloudVision.
+
+### Syncing From CloudVision
+
+> When loading Nautobot data, this tool only loads devices with a device type that has a manufacturer of "Arista"
+
+When syncing data from CloudVision to Nautobot, devices along with their interfaces and tags are synchronized.  When a device exists in CloudVision that doesn't exist in Nautobot, this tool creates the device in Nautobot with the default values specified in the configuration file. When a device exists in Nautobot that does not exist in CloudVision, this tool can be configured to either delete or skip that device.
+You can watch the below video for an example.
+
+![fromcv_sync](https://user-images.githubusercontent.com/38091261/126499331-e41946c4-4e61-4b5e-8b7f-73efb9cd8d3f.gif)
+
+When syncing data from Nautobot to CloudVision, the tag data in Nautobot is copied into User Tags in CloudVision. You can watch the video below for an example.
+
+![tocv_sync](https://user-images.githubusercontent.com/38091261/126499484-2e4c4feb-0492-4dc6-abb6-a092701c81ed.gif)
+
+## Contributing
+
+Pull requests are welcomed and automatically built and tested against multiple versions of Python and multiple versions of Nautobot through GitHub Actions.
+
+The project is packaged with a light development environment based on `docker-compose` to help with the local development of the project and to run the tests within a Docker container.
+
+The project is following Network to Code software development guidelines and is leveraging:
+
+- Black, Pylint, Bandit and pydocstyle for Python linting and formatting.
+- Django unit test to ensure the plugin is working properly.
+
+### Development Environment
+
+The development environment can be used in 2 ways. First, with a local poetry environment if you wish to develop outside of Docker. Second, inside of a docker container.
+
+#### Invoke tasks
+
+The [PyInvoke](http://www.pyinvoke.org/) library is used to provide some helper commands based on the environment.  There are a few configuration parameters that can be passed to PyInvoke to override the default configuration:
+
+- `nautobot_ver`: the version of Nautobot to use as a base for any built docker containers (default: develop-latest)
+- `project_name`: the default docker compose project name (default: aristacv-sync)
+- `python_ver`: the version of Python to use as a base for any built docker containers (default: 3.6)
+- `local`: a boolean flag indicating if invoke tasks should be run on the host or inside the docker containers (default: False, commands will be run in docker containers)
+- `compose_dir`: the full path to a directory containing the project compose files
+- `compose_files`: a list of compose files applied in order (see [Multiple Compose files](https://docs.docker.com/compose/extends/#multiple-compose-files) for more information)
+
+Using PyInvoke these configuration options can be overridden using [several methods](http://docs.pyinvoke.org/en/stable/concepts/configuration.html).  Perhaps the simplest is simply setting an environment variable `INVOKE_ARISTACV-SYNC_VARIABLE_NAME` where `VARIABLE_NAME` is the variable you are trying to override.  The only exception is `compose_files`, because it is a list it must be overridden in a YAML file.  There is an example `invoke.yml` in this directory which can be used as a starting point.
+
+#### Local Poetry Development Environment
+
+1. Copy `development/creds.example.env` to `development/creds.env` (This file will be ignored by git and docker)
+2. Uncomment the `POSTGRES_HOST`, `REDIS_HOST`, and `NAUTOBOT_ROOT` variables in `development/creds.env`
+3. Create an invoke.yml with the following contents at the root of the repo:
+
+```shell
+---
+aristacv_sync:
+  local: true
+  compose_files:
+    - "docker-compose.requirements.yml"
+```
+
+4. Run the following commands:
+
+```shell
+poetry shell
+poetry install
+export $(cat development/dev.env | xargs)
+export $(cat development/creds.env | xargs)
+```
+
+5. You can now run nautobot-server commands as you would from the [Nautobot documentation](https://nautobot.readthedocs.io/en/latest/) for example to start the development server:
+
+```shell
+nautobot-server runserver 0.0.0.0:8080 --insecure
+```
+
+Nautobot server can now be accessed at [http://localhost:8080](http://localhost:8080).
+
+#### Docker Development Environment
+
+This project is managed by [Python Poetry](https://python-poetry.org/) and has a few requirements to setup your development environment:
+
+1. Install Poetry, see the [Poetry Documentation](https://python-poetry.org/docs/#installation) for your operating system.
+2. Install Docker, see the [Docker documentation](https://docs.docker.com/get-docker/) for your operating system.
+
+Once you have Poetry and Docker installed you can run the following commands to install all other development dependencies in an isolated python virtual environment:
+
+```shell
+poetry shell
+poetry install
+invoke start
+```
+
+Nautobot server can now be accessed at [http://localhost:8080](http://localhost:8080).
+
+### CLI Helper Commands
+
+The project is coming with a CLI helper based on [invoke](http://www.pyinvoke.org/) to help set up the development environment. The commands are listed below in 3 categories `dev environment`, `utility` and `testing`.
+
+Each command can be executed with `invoke <command>`. Environment variables `INVOKE_ARISTACV-SYNC_PYTHON_VER` and `INVOKE_ARISTACV-SYNC_NAUTOBOT_VER` may be specified to override the default versions. Each command also has its own help `invoke <command> --help`
+
+#### Docker dev environment
+
+```no-highlight
+  build            Build all docker images.
+  debug            Start Nautobot and its dependencies in debug mode.
+  destroy          Destroy all containers and volumes.
+  restart          Restart Nautobot and its dependencies.
+  start            Start Nautobot and its dependencies in detached mode.
+  stop             Stop Nautobot and its dependencies.
+```
+
+#### Utility
+
+```no-highlight
+  cli              Launch a bash shell inside the running Nautobot container.
+  create-user      Create a new user in django (default: admin), will prompt for password.
+  makemigrations   Run Make Migration in Django.
+  nbshell          Launch a nbshell session.
+```
+
+#### Testing
+
+```no-highlight
+  bandit           Run bandit to validate basic static code security analysis.
+  black            Run black to check that Python files adhere to its style standards.
+  flake8           This will run flake8 for the specified name and Python version.
+  pydocstyle       Run pydocstyle to validate docstring formatting adheres to NTC defined standards.
+  pylint           Run pylint code analysis.
+  tests            Run all tests for this plugin.
+  unittest         Run Django unit tests for the plugin.
+```
+
+## Questions
 
+For any questions or comments, please check the [FAQ](FAQ.md) first and feel free to swing by the [Network to Code slack channel](https://networktocode.slack.com/) (channel #networktocode).
+Sign up [here](http://slack.networktocode.com/)
 
-setup(**setup_kwargs)
```

