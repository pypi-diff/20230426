# Comparing `tmp/odoo12-addon-disable_login-12.0.1.0.1.dev1.tar.gz` & `tmp/odoo12-addon-disable_login-12.0.1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odoo12-addon-disable_login-12.0.1.0.1.dev1.tar", last modified: Wed Apr 26 15:22:45 2023, max compression
+gzip compressed data, was "odoo12-addon-disable_login-12.0.1.0.2.tar", last modified: Wed Apr 26 16:22:11 2023, max compression
```

## Comparing `odoo12-addon-disable_login-12.0.1.0.1.dev1.tar` & `odoo12-addon-disable_login-12.0.1.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-26 15:22:45.176638 odoo12-addon-disable_login-12.0.1.0.1.dev1/
--rw-r--r--   0 daniel    (1000) daniel    (1000)      434 2023-04-26 15:22:45.176638 odoo12-addon-disable_login-12.0.1.0.1.dev1/PKG-INFO
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-26 15:22:45.176638 odoo12-addon-disable_login-12.0.1.0.1.dev1/odoo/
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-26 15:22:45.176638 odoo12-addon-disable_login-12.0.1.0.1.dev1/odoo/addons/
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-26 15:22:45.176638 odoo12-addon-disable_login-12.0.1.0.1.dev1/odoo/addons/disable_login/
--rw-r--r--   0 daniel    (1000) daniel    (1000)       30 2023-04-26 14:30:48.000000 odoo12-addon-disable_login-12.0.1.0.1.dev1/odoo/addons/disable_login/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)      512 2023-04-26 15:22:34.000000 odoo12-addon-disable_login-12.0.1.0.1.dev1/odoo/addons/disable_login/__manifest__.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-26 15:22:45.176638 odoo12-addon-disable_login-12.0.1.0.1.dev1/odoo/addons/disable_login/controllers/
--rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2023-04-26 14:30:48.000000 odoo12-addon-disable_login-12.0.1.0.1.dev1/odoo/addons/disable_login/controllers/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)      641 2023-04-26 14:30:48.000000 odoo12-addon-disable_login-12.0.1.0.1.dev1/odoo/addons/disable_login/controllers/main.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-26 15:22:45.176638 odoo12-addon-disable_login-12.0.1.0.1.dev1/odoo/addons/disable_login/views/
--rw-r--r--   0 daniel    (1000) daniel    (1000)      717 2023-04-26 14:30:48.000000 odoo12-addon-disable_login-12.0.1.0.1.dev1/odoo/addons/disable_login/views/auth_templates.xml
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-26 15:22:45.176638 odoo12-addon-disable_login-12.0.1.0.1.dev1/odoo12_addon_disable_login.egg-info/
--rw-r--r--   0 daniel    (1000) daniel    (1000)      434 2023-04-26 15:22:44.000000 odoo12-addon-disable_login-12.0.1.0.1.dev1/odoo12_addon_disable_login.egg-info/PKG-INFO
--rw-r--r--   0 daniel    (1000) daniel    (1000)      533 2023-04-26 15:22:45.000000 odoo12-addon-disable_login-12.0.1.0.1.dev1/odoo12_addon_disable_login.egg-info/SOURCES.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2023-04-26 15:22:44.000000 odoo12-addon-disable_login-12.0.1.0.1.dev1/odoo12_addon_disable_login.egg-info/dependency_links.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2023-04-26 15:22:44.000000 odoo12-addon-disable_login-12.0.1.0.1.dev1/odoo12_addon_disable_login.egg-info/not-zip-safe
--rw-r--r--   0 daniel    (1000) daniel    (1000)       21 2023-04-26 15:22:44.000000 odoo12-addon-disable_login-12.0.1.0.1.dev1/odoo12_addon_disable_login.egg-info/requires.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)        5 2023-04-26 15:22:44.000000 odoo12-addon-disable_login-12.0.1.0.1.dev1/odoo12_addon_disable_login.egg-info/top_level.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)       38 2023-04-26 15:22:45.176638 odoo12-addon-disable_login-12.0.1.0.1.dev1/setup.cfg
--rw-r--r--   0 daniel    (1000) daniel    (1000)      100 2023-04-26 14:22:40.000000 odoo12-addon-disable_login-12.0.1.0.1.dev1/setup.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-26 16:22:11.918844 odoo12-addon-disable_login-12.0.1.0.2/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      429 2023-04-26 16:22:11.918844 odoo12-addon-disable_login-12.0.1.0.2/PKG-INFO
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-26 16:22:11.918844 odoo12-addon-disable_login-12.0.1.0.2/odoo/
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-26 16:22:11.918844 odoo12-addon-disable_login-12.0.1.0.2/odoo/addons/
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-26 16:22:11.918844 odoo12-addon-disable_login-12.0.1.0.2/odoo/addons/disable_login/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       30 2023-04-26 14:30:48.000000 odoo12-addon-disable_login-12.0.1.0.2/odoo/addons/disable_login/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      525 2023-04-26 16:21:33.000000 odoo12-addon-disable_login-12.0.1.0.2/odoo/addons/disable_login/__manifest__.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-26 16:22:11.918844 odoo12-addon-disable_login-12.0.1.0.2/odoo/addons/disable_login/controllers/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2023-04-26 14:30:48.000000 odoo12-addon-disable_login-12.0.1.0.2/odoo/addons/disable_login/controllers/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      641 2023-04-26 14:30:48.000000 odoo12-addon-disable_login-12.0.1.0.2/odoo/addons/disable_login/controllers/main.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-26 16:22:11.918844 odoo12-addon-disable_login-12.0.1.0.2/odoo/addons/disable_login/views/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      717 2023-04-26 14:30:48.000000 odoo12-addon-disable_login-12.0.1.0.2/odoo/addons/disable_login/views/auth_templates.xml
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-26 16:22:11.918844 odoo12-addon-disable_login-12.0.1.0.2/odoo12_addon_disable_login.egg-info/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      429 2023-04-26 16:22:11.000000 odoo12-addon-disable_login-12.0.1.0.2/odoo12_addon_disable_login.egg-info/PKG-INFO
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      533 2023-04-26 16:22:11.000000 odoo12-addon-disable_login-12.0.1.0.2/odoo12_addon_disable_login.egg-info/SOURCES.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2023-04-26 16:22:11.000000 odoo12-addon-disable_login-12.0.1.0.2/odoo12_addon_disable_login.egg-info/dependency_links.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2023-04-26 16:22:11.000000 odoo12-addon-disable_login-12.0.1.0.2/odoo12_addon_disable_login.egg-info/not-zip-safe
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       21 2023-04-26 16:22:11.000000 odoo12-addon-disable_login-12.0.1.0.2/odoo12_addon_disable_login.egg-info/requires.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        5 2023-04-26 16:22:11.000000 odoo12-addon-disable_login-12.0.1.0.2/odoo12_addon_disable_login.egg-info/top_level.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       38 2023-04-26 16:22:11.918844 odoo12-addon-disable_login-12.0.1.0.2/setup.cfg
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      100 2023-04-26 14:22:40.000000 odoo12-addon-disable_login-12.0.1.0.2/setup.py
```

### Comparing `odoo12-addon-disable_login-12.0.1.0.1.dev1/odoo/addons/disable_login/__manifest__.py` & `odoo12-addon-disable_login-12.0.1.0.2/odoo/addons/disable_login/__manifest__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright 2023-Coopdevs Treball SCCL (<https://coopdevs.org>)
 # License AGPL-3.0 or later (https://www.gnu.org/licenses/agpl.html).
 {
     "name": "Disable Odoo Login",
-    "version": "12.0.1.0.1",
-    "depends": ["base"],
+    "version": "12.0.1.0.2",
+    "depends": ["web", "auth_oauth"],
     "author": "Coopdevs Treball SCCL",
     "category": "Auth",
     "website": "https://coopdevs.org",
     "license": "AGPL-3",
     "summary": """
         Disable login template to force to use the OAuth login.
     """,
```

### Comparing `odoo12-addon-disable_login-12.0.1.0.1.dev1/odoo/addons/disable_login/controllers/main.py` & `odoo12-addon-disable_login-12.0.1.0.2/odoo/addons/disable_login/controllers/main.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-disable_login-12.0.1.0.1.dev1/odoo/addons/disable_login/views/auth_templates.xml` & `odoo12-addon-disable_login-12.0.1.0.2/odoo/addons/disable_login/views/auth_templates.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-disable_login-12.0.1.0.1.dev1/odoo12_addon_disable_login.egg-info/SOURCES.txt` & `odoo12-addon-disable_login-12.0.1.0.2/odoo12_addon_disable_login.egg-info/SOURCES.txt`

 * *Files identical despite different names*

