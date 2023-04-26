# Comparing `tmp/odoo14-addon-odoo_instance-14.0.1.1.1.tar.gz` & `tmp/odoo14-addon-odoo_instance-14.0.1.1.2.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odoo14-addon-odoo_instance-14.0.1.1.1.tar", last modified: Tue Apr 25 22:45:02 2023, max compression
+gzip compressed data, was "odoo14-addon-odoo_instance-14.0.1.1.2.dev2.tar", last modified: Wed Apr 26 15:57:34 2023, max compression
```

## Comparing `odoo14-addon-odoo_instance-14.0.1.1.1.tar` & `odoo14-addon-odoo_instance-14.0.1.1.2.dev2.tar`

### file list

```diff
@@ -1,75 +1,76 @@
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 22:45:02.626143 odoo14-addon-odoo_instance-14.0.1.1.1/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     4011 2023-04-25 22:45:02.626143 odoo14-addon-odoo_instance-14.0.1.1.1/PKG-INFO
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 22:45:02.619476 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 22:45:02.619476 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 22:45:02.619476 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     3599 2023-04-25 22:42:55.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/README.rst
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)       43 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/__init__.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1325 2023-04-25 20:41:20.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/__manifest__.py
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 22:45:02.622809 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/data/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      217 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/data/calendar_tags.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1389 2023-04-25 16:24:52.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/data/ir_cron.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)    95199 2023-04-24 19:27:51.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/data/odoo12_core_modules_data.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     9484 2023-04-24 19:27:51.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/data/odoo14_core_modules_app_data.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      705 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/data/odoo_version_data.xml
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 22:45:02.622809 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/models/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      273 2023-04-25 15:10:06.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/models/__init__.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      208 2023-04-25 15:10:06.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/models/calendar_event.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      484 2023-04-25 15:10:06.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/models/import_requirements_wizard.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)    17875 2023-04-25 19:58:28.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/models/odoo_instance.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     3078 2023-04-25 22:38:06.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/models/odoo_instance_module.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1345 2023-04-25 15:10:06.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/models/odoo_instance_process.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1791 2023-04-25 15:10:06.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/models/odoo_instance_window.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      452 2023-04-25 15:10:06.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/models/odoo_release.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      283 2023-04-25 15:10:06.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/models/odoo_version.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      475 2023-04-25 15:10:06.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/models/process_module_rel.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      183 2023-04-25 15:10:06.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/models/project_project.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      182 2023-04-25 15:10:06.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/models/res_partner.py
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 22:45:02.622809 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/readme/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1254 2023-04-24 17:29:42.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/readme/DESCRIPTION.rst
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      619 2023-04-25 22:42:50.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/readme/HISTORY.rst
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 22:45:02.622809 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/readme/newsfragments/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)       12 2023-04-24 18:45:09.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/readme/newsfragments/.gitignore
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 22:45:02.622809 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/security/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)       24 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/security/__init__.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1654 2023-04-25 10:24:56.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/security/ir.model.access.csv
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      383 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/security/security_groups.xml
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 22:45:02.619476 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/static/
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 22:45:02.622809 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/static/description/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)    13625 2023-04-25 22:42:55.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/static/description/index.html
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 22:45:02.619476 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/static/src/
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 22:45:02.622809 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/static/src/css/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)        0 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/static/src/css/project_instance.css
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 22:45:02.622809 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/static/src/img/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)    33659 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/static/src/img/icon.png
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 22:45:02.622809 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/static/src/js/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)        0 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/static/src/js/project_instance.js
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 22:45:02.622809 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/tests/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)        0 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/tests/__init__.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)        0 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/tests/test_project_instance.py
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 22:45:02.622809 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/views/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1049 2023-04-24 19:27:51.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/views/import_requirements_wizard_view.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     3617 2023-04-25 20:59:22.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/views/odoo_instance_actions.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     2679 2023-04-25 20:06:20.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/views/odoo_instance_menuitems.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1396 2023-04-25 19:54:54.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/views/odoo_instance_module_version_views.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     4622 2023-04-25 20:37:02.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/views/odoo_instance_searches.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)    19771 2023-04-25 22:36:30.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/views/odoo_instance_view.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      971 2023-04-24 19:32:46.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/views/odoo_instance_window_wizard_view.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     3311 2023-04-25 20:56:12.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/views/odoo_module_view.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1688 2023-04-25 20:43:09.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/views/odoo_process_view.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     2254 2023-04-25 10:24:49.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/views/odoo_release_view.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1113 2023-04-25 10:24:49.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/views/odoo_version_view.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      920 2023-04-24 18:27:56.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/views/project_project_view.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1083 2023-04-24 20:15:25.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/views/res_partner_view.xml
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 22:45:02.622809 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/wizards/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)       94 2023-04-24 19:55:35.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/wizards/__init__.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     2291 2023-04-25 15:10:06.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/wizards/odoo_instance_window_wizard.py
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 22:45:02.626143 odoo14-addon-odoo_instance-14.0.1.1.1/odoo14_addon_odoo_instance.egg-info/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     4011 2023-04-25 22:45:02.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo14_addon_odoo_instance.egg-info/PKG-INFO
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     2840 2023-04-25 22:45:02.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo14_addon_odoo_instance.egg-info/SOURCES.txt
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)        1 2023-04-25 22:45:02.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo14_addon_odoo_instance.egg-info/dependency_links.txt
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)        1 2023-04-25 22:45:02.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo14_addon_odoo_instance.egg-info/not-zip-safe
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)       50 2023-04-25 22:45:02.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo14_addon_odoo_instance.egg-info/requires.txt
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)        5 2023-04-25 22:45:02.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo14_addon_odoo_instance.egg-info/top_level.txt
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)       38 2023-04-25 22:45:02.626143 odoo14-addon-odoo_instance-14.0.1.1.1/setup.cfg
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      100 2023-04-25 22:44:55.000000 odoo14-addon-odoo_instance-14.0.1.1.1/setup.py
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-26 15:57:34.484701 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     4100 2023-04-26 15:57:34.484701 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/PKG-INFO
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-26 15:57:34.484701 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-26 15:57:34.484701 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-26 15:57:34.484701 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     3683 2023-04-25 23:36:38.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/README.rst
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)       43 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/__init__.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1325 2023-04-26 01:22:03.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/__manifest__.py
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-26 15:57:34.484701 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/data/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      217 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/data/calendar_tags.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1389 2023-04-25 16:24:52.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/data/ir_cron.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)    95199 2023-04-24 19:27:51.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/data/odoo12_core_modules_data.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     9484 2023-04-24 19:27:51.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/data/odoo14_core_modules_app_data.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      705 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/data/odoo_version_data.xml
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-26 15:57:34.484701 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/models/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      310 2023-04-26 01:22:03.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/models/__init__.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      208 2023-04-25 15:10:06.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/models/calendar_event.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      484 2023-04-25 15:10:06.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/models/import_requirements_wizard.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)    19822 2023-04-26 15:57:11.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/models/odoo_instance.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      370 2023-04-25 23:19:33.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/models/odoo_instance_database.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     3078 2023-04-25 22:38:06.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/models/odoo_instance_module.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1345 2023-04-25 15:10:06.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/models/odoo_instance_process.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1791 2023-04-25 15:10:06.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/models/odoo_instance_window.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      452 2023-04-25 15:10:06.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/models/odoo_release.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      283 2023-04-25 15:10:06.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/models/odoo_version.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      475 2023-04-25 15:10:06.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/models/process_module_rel.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      183 2023-04-25 15:10:06.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/models/project_project.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      182 2023-04-25 15:10:06.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/models/res_partner.py
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-26 15:57:34.484701 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/readme/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1254 2023-04-24 17:29:42.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/readme/DESCRIPTION.rst
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      703 2023-04-25 23:36:22.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/readme/HISTORY.rst
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-26 15:57:34.484701 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/readme/newsfragments/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)       12 2023-04-24 18:45:09.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/readme/newsfragments/.gitignore
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-26 15:57:34.484701 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/security/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)       24 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/security/__init__.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1783 2023-04-26 01:22:03.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/security/ir.model.access.csv
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      383 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/security/security_groups.xml
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-26 15:57:34.484701 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/static/
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-26 15:57:34.484701 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/static/description/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)    13912 2023-04-25 23:36:38.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/static/description/index.html
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-26 15:57:34.484701 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/static/src/
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-26 15:57:34.484701 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/static/src/css/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)        0 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/static/src/css/project_instance.css
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-26 15:57:34.484701 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/static/src/img/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)    33659 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/static/src/img/icon.png
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-26 15:57:34.484701 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/static/src/js/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)        0 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/static/src/js/project_instance.js
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-26 15:57:34.484701 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/tests/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)        0 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/tests/__init__.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)        0 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/tests/test_project_instance.py
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-26 15:57:34.484701 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/views/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1049 2023-04-24 19:27:51.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/views/import_requirements_wizard_view.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     3617 2023-04-26 01:22:03.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/views/odoo_instance_actions.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     2679 2023-04-25 20:06:20.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/views/odoo_instance_menuitems.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1396 2023-04-25 19:54:54.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/views/odoo_instance_module_version_views.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     4622 2023-04-25 20:37:02.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/views/odoo_instance_searches.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)    20295 2023-04-26 01:22:03.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/views/odoo_instance_view.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      971 2023-04-24 19:32:46.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/views/odoo_instance_window_wizard_view.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     3311 2023-04-25 20:56:12.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/views/odoo_module_view.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1688 2023-04-25 20:43:09.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/views/odoo_process_view.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     2254 2023-04-25 10:24:49.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/views/odoo_release_view.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1113 2023-04-25 10:24:49.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/views/odoo_version_view.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      920 2023-04-24 18:27:56.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/views/project_project_view.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1083 2023-04-24 20:15:25.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/views/res_partner_view.xml
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-26 15:57:34.484701 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/wizards/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)       94 2023-04-26 01:22:03.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/wizards/__init__.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     2291 2023-04-25 15:10:06.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/wizards/odoo_instance_window_wizard.py
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-26 15:57:34.484701 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo14_addon_odoo_instance.egg-info/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     4100 2023-04-26 15:57:34.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo14_addon_odoo_instance.egg-info/PKG-INFO
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     2899 2023-04-26 15:57:34.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo14_addon_odoo_instance.egg-info/SOURCES.txt
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)        1 2023-04-26 15:57:34.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo14_addon_odoo_instance.egg-info/dependency_links.txt
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)        1 2023-04-26 15:57:34.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo14_addon_odoo_instance.egg-info/not-zip-safe
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)       50 2023-04-26 15:57:34.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo14_addon_odoo_instance.egg-info/requires.txt
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)        5 2023-04-26 15:57:34.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo14_addon_odoo_instance.egg-info/top_level.txt
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)       38 2023-04-26 15:57:34.484701 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/setup.cfg
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      100 2023-04-25 22:51:42.000000 odoo14-addon-odoo_instance-14.0.1.1.2.dev2/setup.py
```

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.1/PKG-INFO` & `odoo14-addon-odoo_instance-14.0.1.1.2.dev2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo14-addon-odoo_instance
-Version: 14.0.1.1.1
+Version: 14.0.1.1.2.dev2
 Summary: Manage Odoo instances with relevant information
 Home-page: https://www.coopdevs.org
 Author: Coopdevs
 License: AGPL-3
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 14.0
@@ -50,14 +50,22 @@
 
 .. contents::
    :local:
 
 Changelog
 =========
 
+14.0.1.2.0 (2023-04-26)
+~~~~~~~~~~~~~~~~~~~~~~~
+
+**Features**
+
+- Manage databases
+
+
 14.0.1.1.1 (2023-04-25)
 ~~~~~~~~~~~~~~~~~~~~~~~
 
 **Bugfixes**
 
 - Upcrate module versions
 - Show installed module versions only in instance view
```

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/README.rst` & `odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo14_addon_odoo_instance.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: odoo14-addon-odoo-instance
+Version: 14.0.1.1.2.dev2
+Summary: Manage Odoo instances with relevant information
+Home-page: https://www.coopdevs.org
+Author: Coopdevs
+License: AGPL-3
+Classifier: Programming Language :: Python
+Classifier: Framework :: Odoo
+Classifier: Framework :: Odoo :: 14.0
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3
+Requires-Python: >=3.6
+
 =============
 Odoo Instance
 =============
 
 .. !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
    !! This file is generated by oca-gen-addon-readme !!
    !! changes will be overwritten.                   !!
@@ -37,14 +50,22 @@
 
 .. contents::
    :local:
 
 Changelog
 =========
 
+14.0.1.2.0 (2023-04-26)
+~~~~~~~~~~~~~~~~~~~~~~~
+
+**Features**
+
+- Manage databases
+
+
 14.0.1.1.1 (2023-04-25)
 ~~~~~~~~~~~~~~~~~~~~~~~
 
 **Bugfixes**
 
 - Upcrate module versions
 - Show installed module versions only in instance view
```

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/__manifest__.py` & `odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/__manifest__.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/data/ir_cron.xml` & `odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/data/ir_cron.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/data/odoo12_core_modules_data.xml` & `odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/data/odoo12_core_modules_data.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/data/odoo14_core_modules_app_data.xml` & `odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/data/odoo14_core_modules_app_data.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/data/odoo_version_data.xml` & `odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/data/odoo_version_data.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/models/odoo_instance.py` & `odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/models/odoo_instance.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 import re
 from datetime import datetime, time, timedelta
-
+from urllib.parse import urlparse
 import pytz
 import requests
 import yaml
 
 from odoo import api, fields, models
 from odoo.exceptions import UserError
 
@@ -18,28 +18,31 @@
     _inherit = ['mail.thread', 'mail.activity.mixin']
     # General Information
 
     name = fields.Char(string='Instance Name', required=True)
     description = fields.Text(string='Instance Description')
     start_date = fields.Date(string='Start Date')
 
-    project_id = fields.Many2one('project.project', string='Project', ondelete='set null')
-    helpdesk_team_id = fields.Many2one('helpdesk.team', string='Helpdesk Team', ondelete='set null')
+    project_id = fields.Many2one(
+        'project.project', string='Project', ondelete='set null')
+    helpdesk_team_id = fields.Many2one(
+        'helpdesk.team', string='Helpdesk Team', ondelete='set null')
     instance_url = fields.Char(string='Instance URL')
 
     partner_id = fields.Many2one('res.partner', string='Client', required=True)
     client_contact_id = fields.Many2one(
         'res.partner', string='Client Contact', domain=[('type', '=', 'contact')])
 
     technician_ids = fields.Many2many(
         'res.users', string='Technicians', relation='odoo_instance_technician_rel')
     functional_ids = fields.Many2many(
         'res.users', string='Functional Experts', relation='odoo_instance_functional_rel')
 
-    odoo_version_id = fields.Many2one('odoo.version', string="Odoo Version", required=True)
+    odoo_version_id = fields.Many2one(
+        'odoo.version', string="Odoo Version", required=True)
 
     state = fields.Selection([
         ('in_progress', 'In Progress'),
         ('running', 'Running'),
         ('paused', 'Paused'),
         ('cancelled', 'Terminated')
     ], string='State', default='in_progress')
@@ -76,18 +79,22 @@
         ('cpx31', 'cpx31'),
         ('cx41', 'cx41'),
         ('cpx41', 'cpx41'),
         ('cx51', 'cx51'),
         ('cpx51', 'cpx51'),
     ], string="Server Type")
 
-    troubleshooting_ids = fields.One2many('odoo.instance.troubleshooting', 'instance_id', string='Troubleshooting')
+    troubleshooting_ids = fields.One2many(
+        'odoo.instance.troubleshooting', 'instance_id', string='Troubleshooting')
     deploy_duration = fields.Float(
         string='Deploy Duration', default=1.0, help="Duration in hours")
 
+    database_ids = fields.One2many(
+        'odoo.instance.database', 'instance_id', string='Databases')
+
     # Functional Information
     process_ids = fields.Many2many(
         'odoo.instance.process',
         'odoo_instance_process_rel',
         'instance_id',
         'process_id',
         string='Processes'
@@ -105,20 +112,102 @@
     implementation_contract_id = fields.Char(
         string='Contrato de Implementación')
 
     # maintenance_contract_ids = fields.Many2many('contract.contract', string='Contratos de Mantenimiento', relation='odoo_instance_maintenance_contract_rel')
     # support_contract_ids = fields.Many2many('contract.contract', string='Contratos de Soporte', relation='odoo_instance_support_contract_rel')
     # implementation_contract_id = fields.Many2one('contract.contract', string='Contrato de Implementación', relation='odoo_instance_implementation_contract_rel')
 
+    def _strip_protocol_and_port(self):
+        parsed_url = urlparse(self.instance_url)
+        return parsed_url.hostname
+
+    def _get_instance_config_yaml(self, url):
+        # Get the YAML content
+        response = requests.get(url)
+        if response.status_code != 200:
+            return {}
+        response.raise_for_status()
+        return yaml.safe_load(response.text)
+
+    def _update_instance_dbs(self):
+        base_url = self.inventory_url
+        branch = self.branch
+        instance_url = self._strip_protocol_and_port()
+        urls = {
+            'host_vars': f"{base_url}/-/raw/{branch}/inventory/host_vars/{instance_url}/config.yml",
+            'group_vars': f"{base_url}/-/raw/{branch}/inventory/group_vars/all.yml",
+        }
+
+        for url in urls.values():
+            yaml_content = self._get_instance_config_yaml(url)
+            odoo_dbs = yaml_content.get("odoo_role_odoo_dbs", [])
+            test_dbs = yaml_content.get("odoo_role_test_dbs", [])
+
+            instance_dbs_info = []
+            self.database_ids.unlink()
+
+        for db in odoo_dbs:
+            self.database_ids.create({
+                'name': db,
+                'is_test': False,
+                'instance_id': self.id,
+            })
+
+        for test_db in test_dbs:
+            self.database_ids.create({
+                'name': test_db,
+                'is_test': True,
+                'instance_id': self.id,
+            })
+
+    def update_odoo_release(self):
+        inventory_url = self.inventory_url
+        branch = self.branch
+        raw_inventory_url = f"{inventory_url}/-/raw/{branch}/inventory/group_vars/all.yml"
+        response = requests.get(raw_inventory_url)
+
+        if response.status_code == 200:
+            inventory_data = yaml.safe_load(response.text)
+            odoo_release_str = inventory_data.get('odoo_role_odoo_release')
+
+            if odoo_release_str:
+                odoo_version, release_date_str = odoo_release_str.split('_')
+                release_date = fields.Date.from_string(release_date_str)
+
+                odoo_version_id = self.env['odoo.version'].search(
+                    [('name', '=', odoo_version)], limit=1)
+                if odoo_version_id:
+                    odoo_release = self.env['odoo.release'].search([
+                        ('name', '=', odoo_release_str),
+                        ('odoo_version_id', '=', odoo_version_id.id)
+                    ], limit=1)
+
+                    if not odoo_release:
+                        odoo_release = self.env['odoo.release'].create({
+                            'name': odoo_release_str,
+                            'release_date': release_date,
+                            'odoo_version_id': odoo_version_id.id,
+                        })
+
+                    self.odoo_release_id = odoo_release
+
+    def update_instance_info(self):
+        for instance in self:
+            # Update Odoo Release
+            instance.update_odoo_release()
+
+            # Update Instance DBs
+            instance._update_instance_dbs()
+
     def toggle_state(self):
         state_order = ['in_progress', 'running', 'paused', 'cancelled']
-        next_state_index = (state_order.index(self.state) + 1) % len(state_order)
+        next_state_index = (state_order.index(
+            self.state) + 1) % len(state_order)
         self.state = state_order[next_state_index]
 
-
     def download_and_process_requirements_txt(self):
         if not self.requirements_url:
             return
         response = requests.get(self.requirements_url)
         if response.status_code == 200:
             requirements_txt = response.text
             self.import_requirements_txt(requirements_txt)
@@ -183,15 +272,16 @@
             version_record = ModuleVersion.search([
                 ('name', '=', version),
                 ('module_id', '=', module.id),
             ], limit=1)
 
             if version_record:
                 # Update the existing version record by adding the instance
-                _logger.critical("Version found %s", version_record.instance_ids)
+                _logger.critical("Version found %s",
+                                 version_record.instance_ids)
                 version_record.instance_ids |= self
             else:
                 # Create a new version record
                 _logger.critical("Version not found, creating it")
                 version_record = ModuleVersion.create({
                     'name': version,
                     'module_id': module.id,
@@ -227,15 +317,16 @@
             if module_data['is_odoo_module']:
                 # Check if the module is Odoo core or OCA
                 if 'oca' in module_data['home_page'].lower():
                     module_data['module_type'] = 'OCA'
 
                 # extract odoo version from version key. Example: version	"14.0.1.0.3"
                 odoo_version_pattern = r"(\d{1,2}\.\d{1,2})"
-                match = re.search(odoo_version_pattern, data['info']['version'])
+                match = re.search(odoo_version_pattern,
+                                  data['info']['version'])
                 if match:
                     module_data['odoo_version'] = match.group(1)
                     module_data['odoo_version_id'] = self.env['odoo.version'].search([('name', '=', match.group(1))],
                                                                                      limit=1).id
 
         else:
             _logger.warning(
@@ -256,34 +347,39 @@
             for i in range(7):
                 current_date = now_local.date() + timedelta(days=i)
                 current_weekday = str(current_date.weekday())
 
                 unavailable_periods = []
                 for schedule in instance.unavailable_windows:
                     if schedule.day_of_week == current_weekday:
-                        unavailable_periods.append(schedule.get_unavailable_periods(current_date, user_tz))
+                        unavailable_periods.append(
+                            schedule.get_unavailable_periods(current_date, user_tz))
 
                 unavailable_periods.sort()
-                available_start_time = user_tz.localize(datetime.combine(current_date, time(0, 0)))
+                available_start_time = user_tz.localize(
+                    datetime.combine(current_date, time(0, 0)))
 
                 for period_start, period_end in unavailable_periods:
                     if period_start > available_start_time:
-                        deploy_end_time = period_start - timedelta(hours=instance.deploy_duration)
+                        deploy_end_time = period_start - \
+                            timedelta(hours=instance.deploy_duration)
                         if deploy_end_time > available_start_time:
                             instance.available_windows.create({
                                 'instance_id': instance.id,
                                 'start_time': available_start_time.astimezone(pytz.utc).replace(tzinfo=None),
                                 'end_time': deploy_end_time.astimezone(pytz.utc).replace(tzinfo=None),
                             })
 
                     available_start_time = period_end
 
-                available_end_time = user_tz.localize(datetime.combine(current_date, time.max))
+                available_end_time = user_tz.localize(
+                    datetime.combine(current_date, time.max))
                 if available_end_time > available_start_time:
-                    deploy_end_time = available_end_time - timedelta(hours=instance.deploy_duration)
+                    deploy_end_time = available_end_time - \
+                        timedelta(hours=instance.deploy_duration)
                     if deploy_end_time > available_start_time:
                         instance.available_windows.create({
                             'instance_id': instance.id,
                             'start_time': available_start_time.astimezone(pytz.utc).replace(tzinfo=None),
                             'end_time': deploy_end_time.astimezone(pytz.utc).replace(tzinfo=None),
                         })
             instance.action_delete_past_or_orphan_windows()
@@ -310,49 +406,20 @@
             raise UserError(("No hay URL para esta instancia."))
         return {
             'type': 'ir.actions.act_url',
             'url': self.instance_url,
             'target': 'new',
         }
 
-    def update_odoo_release(self):
-        for instance in self:
-            inventory_url = instance.inventory_url
-            branch = instance.branch
-            raw_inventory_url = f"{inventory_url}/-/raw/{branch}/inventory/group_vars/all.yml"
-            response = requests.get(raw_inventory_url)
-
-            if response.status_code == 200:
-                inventory_data = yaml.safe_load(response.text)
-                odoo_release_str = inventory_data.get('odoo_role_odoo_release')
-
-                if odoo_release_str:
-                    odoo_version, release_date_str = odoo_release_str.split('_')
-                    release_date = fields.Date.from_string(release_date_str)
-
-                    odoo_version_id = self.env['odoo.version'].search([('name', '=', odoo_version)], limit=1)
-                    if odoo_version_id:
-                        odoo_release = self.env['odoo.release'].search([
-                            ('name', '=', odoo_release_str),
-                            ('odoo_version_id', '=', odoo_version_id.id)
-                        ], limit=1)
-
-                        if not odoo_release:
-                            odoo_release = self.env['odoo.release'].create({
-                                'name': odoo_release_str,
-                                'release_date': release_date,
-                                'odoo_version_id': odoo_version_id.id,
-                            })
-
-                        instance.odoo_release_id = odoo_release
     def action_delete_past_or_orphan_windows(self):
-        self.env["odoo.instance.window"].delete_past_or_orphan_windows()                        
-    def action_clear_windows(self):        
-        self.env['odoo.instance.window'].search([('instance_id', '=', self.id)]).unlink()
+        self.env["odoo.instance.window"].delete_past_or_orphan_windows()
 
+    def action_clear_windows(self):
+        self.env['odoo.instance.window'].search(
+            [('instance_id', '=', self.id)]).unlink()
 
 
 class OdooInstanceSchedule(models.Model):
     _name = 'odoo.instance.schedule'
     _description = 'Deploy Schedule'
 
     instance_id = fields.Many2one('odoo.instance', string="Instance")
@@ -395,15 +462,16 @@
     url = fields.Char(string='URL')
     type = fields.Selection([
         ('postmortem', 'Post Mortem'),
         ('config', 'Configuration'),
         ('other', 'Other')
     ], string='Type', default='config', required=True)
 
-    instance_id = fields.Many2one('odoo.instance', string='Instance', ondelete='cascade')
+    instance_id = fields.Many2one(
+        'odoo.instance', string='Instance', ondelete='cascade')
 
 
 class OdooInstanceUnavailableSchedule(models.Model):
     _name = 'odoo.instance.unavailable_schedule'
     _description = 'Unavailable Deploy Schedule'
 
     instance_id = fields.Many2one('odoo.instance', string="Instance")
@@ -423,11 +491,13 @@
         schedule_hour = int(self.start_time)
         schedule_minute = int((self.start_time % 1) * 60)
         schedule_time = time(schedule_hour, schedule_minute, 0)
         schedule_end_hour = int(self.end_time)
         schedule_end_minute = int((self.end_time % 1) * 60)
         schedule_end_time = time(schedule_end_hour, schedule_end_minute, 0)
 
-        start_time = user_tz.localize(datetime.combine(current_date, schedule_time))
-        end_time = user_tz.localize(datetime.combine(current_date, schedule_end_time))
+        start_time = user_tz.localize(
+            datetime.combine(current_date, schedule_time))
+        end_time = user_tz.localize(
+            datetime.combine(current_date, schedule_end_time))
 
         return (start_time, end_time)
```

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/models/odoo_instance_module.py` & `odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/models/odoo_instance_module.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/models/odoo_instance_process.py` & `odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/models/odoo_instance_process.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/models/odoo_instance_window.py` & `odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/models/odoo_instance_window.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/readme/DESCRIPTION.rst` & `odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/readme/DESCRIPTION.rst`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/readme/HISTORY.rst` & `odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/readme/HISTORY.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+14.0.1.2.0 (2023-04-26)
+~~~~~~~~~~~~~~~~~~~~~~~
+
+**Features**
+
+- Manage databases
+
+
 14.0.1.1.1 (2023-04-25)
 ~~~~~~~~~~~~~~~~~~~~~~~
 
 **Bugfixes**
 
 - Upcrate module versions
 - Show installed module versions only in instance view
```

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/security/ir.model.access.csv` & `odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/security/ir.model.access.csv`

 * *Files 1% similar despite different names*

```diff
@@ -7,7 +7,8 @@
 access_odoo_instance_unavailabe_schedule,odoo.instance.unavailable_schedule,model_odoo_instance_unavailable_schedule,odoo_instance.group_odoo_instance_user,1,1,1,1
 access_odoo_instance_functional_requirement,odoo.instance.functional.requirement,model_odoo_instance_functional_requirement,odoo_instance.group_odoo_instance_user,1,1,1,1
 access_odoo_instance_window,odoo.instance.window,model_odoo_instance_window,odoo_instance.group_odoo_instance_user,1,1,1,1
 access_odoo_instance_window_wizard,odoo.instance.window.wizard,model_odoo_instance_window_wizard,odoo_instance.group_odoo_instance_user,1,1,1,1
 access_odoo_instance_troubleshooting,odoo.instance.troubleshooting,model_odoo_instance_troubleshooting,odoo_instance.group_odoo_instance_user,1,1,1,1
 access_odoo_version,odoo.version,model_odoo_version,odoo_instance.group_odoo_instance_user,1,1,0,0
 access_odoo_release,odoo.release,model_odoo_release,odoo_instance.group_odoo_instance_user,1,1,1,1
+access_odoo_instance_database,odoo.instance.database,model_odoo_instance_database,odoo_instance.group_odoo_instance_user,1,1,1,1
```

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/static/description/index.html` & `odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/static/description/index.html`

 * *Files 2% similar despite different names*

#### Comparing `odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/static/description/index.html` & `odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/static/description/index.html`

```diff
@@ -394,146 +394,160 @@
       </blockquote>
       <p>
         <strong>Table of contents</strong>
       </p>
       <div class="contents local topic" id="contents">
         <ul class="simple">
           <li>
-            <a class="reference internal" href="#changelog" id="id6">Changelog</a>
+            <a class="reference internal" href="#changelog" id="id7">Changelog</a>
             <ul>
               <li>
-                <a class="reference internal" href="#id1" id="id7">14.0.1.1.1 (2023-04-25)</a>
+                <a class="reference internal" href="#id1" id="id8">14.0.1.2.0 (2023-04-26)</a>
               </li>
               <li>
-                <a class="reference internal" href="#id2" id="id8">14.0.1.1.0 (2023-04-25)</a>
+                <a class="reference internal" href="#id2" id="id9">14.0.1.1.1 (2023-04-25)</a>
               </li>
               <li>
-                <a class="reference internal" href="#id3" id="id9">14.0.1.0.1 (2023-04-25)</a>
+                <a class="reference internal" href="#id3" id="id10">14.0.1.1.0 (2023-04-25)</a>
               </li>
               <li>
-                <a class="reference internal" href="#id4" id="id10">14.0.1.0.0 (2023-04-24)</a>
+                <a class="reference internal" href="#id4" id="id11">14.0.1.0.1 (2023-04-25)</a>
               </li>
               <li>
-                <a class="reference internal" href="#id5" id="id11">14.0.0.2.0 (2023-04-24)</a>
+                <a class="reference internal" href="#id5" id="id12">14.0.1.0.0 (2023-04-24)</a>
+              </li>
+              <li>
+                <a class="reference internal" href="#id6" id="id13">14.0.0.2.0 (2023-04-24)</a>
               </li>
             </ul>
           </li>
           <li>
-            <a class="reference internal" href="#bug-tracker" id="id12">Bug Tracker</a>
+            <a class="reference internal" href="#bug-tracker" id="id14">Bug Tracker</a>
           </li>
           <li>
-            <a class="reference internal" href="#credits" id="id13">Credits</a>
+            <a class="reference internal" href="#credits" id="id15">Credits</a>
             <ul>
               <li>
-                <a class="reference internal" href="#authors" id="id14">Authors</a>
+                <a class="reference internal" href="#authors" id="id16">Authors</a>
               </li>
               <li>
-                <a class="reference internal" href="#maintainers" id="id15">Maintainers</a>
+                <a class="reference internal" href="#maintainers" id="id17">Maintainers</a>
               </li>
             </ul>
           </li>
         </ul>
       </div>
       <div class="section" id="changelog">
         <h1>
-          <a class="toc-backref" href="#id6">Changelog</a>
+          <a class="toc-backref" href="#id7">Changelog</a>
         </h1>
         <div class="section" id="id1">
           <h2>
-            <a class="toc-backref" href="#id7">14.0.1.1.1 (2023-04-25)</a>
+            <a class="toc-backref" href="#id8">14.0.1.2.0 (2023-04-26)</a>
+          </h2>
+          <p>
+            <strong>Features</strong>
+          </p>
+          <ul class="simple">
+            <li>Manage databases</li>
+          </ul>
+        </div>
+        <div class="section" id="id2">
+          <h2>
+            <a class="toc-backref" href="#id9">14.0.1.1.1 (2023-04-25)</a>
           </h2>
           <p>
             <strong>Bugfixes</strong>
           </p>
           <ul class="simple">
             <li>Upcrate module versions</li>
             <li>Show installed module versions only in instance view</li>
           </ul>
         </div>
-        <div class="section" id="id2">
+        <div class="section" id="id3">
           <h2>
-            <a class="toc-backref" href="#id8">14.0.1.1.0 (2023-04-25)</a>
+            <a class="toc-backref" href="#id10">14.0.1.1.0 (2023-04-25)</a>
           </h2>
           <p>
             <strong>Features</strong>
           </p>
           <ul class="simple">
             <li>Handle odoo releases</li>
           </ul>
         </div>
-        <div class="section" id="id3">
+        <div class="section" id="id4">
           <h2>
-            <a class="toc-backref" href="#id9">14.0.1.0.1 (2023-04-25)</a>
+            <a class="toc-backref" href="#id11">14.0.1.0.1 (2023-04-25)</a>
           </h2>
           <p>
             <strong>Features</strong>
           </p>
           <ul class="simple">
             <li>Improved UX: Searches, filters, grouping…</li>
           </ul>
           <p>
             <strong>Bugfixes</strong>
           </p>
           <ul class="simple">
             <li>Removed forgotten debug statementes</li>
           </ul>
         </div>
-        <div class="section" id="id4">
+        <div class="section" id="id5">
           <h2>
-            <a class="toc-backref" href="#id10">14.0.1.0.0 (2023-04-24)</a>
+            <a class="toc-backref" href="#id12">14.0.1.0.0 (2023-04-24)</a>
           </h2>
           <p>
             <strong>Features</strong>
           </p>
           <ul class="simple">
             <li>Rename models and split logic in files</li>
           </ul>
         </div>
-        <div class="section" id="id5">
+        <div class="section" id="id6">
           <h2>
-            <a class="toc-backref" href="#id11">14.0.0.2.0 (2023-04-24)</a>
+            <a class="toc-backref" href="#id13">14.0.0.2.0 (2023-04-24)</a>
           </h2>
           <p>
             <strong>Features</strong>
           </p>
           <ul class="simple">
             <li>Add instance relations to project and res.partner</li>
           </ul>
         </div>
       </div>
       <div class="section" id="bug-tracker">
         <h1>
-          <a class="toc-backref" href="#id12">Bug Tracker</a>
+          <a class="toc-backref" href="#id14">Bug Tracker</a>
         </h1>
         <p>
           Bugs are tracked on
           <a class="reference external" href="https://github.com/coopdevs/odoo14-addons/issues">GitHub Issues</a>
           .
 In case of trouble, please check there if your issue has already been reported.
 If you spotted it first, help us smashing it by providing a detailed and welcomed
           <a class="reference external" href="https://github.com/coopdevs/odoo14-addons/issues/new?body=module:%20odoo_instance%0Aversion:%2014.0%0A%0A**Steps%20to%20reproduce**%0A-%20...%0A%0A**Current%20behavior**%0A%0A**Expected%20behavior**">feedback</a>
           .
         </p>
         <p>Do not contact contributors directly about support or help with technical issues.</p>
       </div>
       <div class="section" id="credits">
         <h1>
-          <a class="toc-backref" href="#id13">Credits</a>
+          <a class="toc-backref" href="#id15">Credits</a>
         </h1>
         <div class="section" id="authors">
           <h2>
-            <a class="toc-backref" href="#id14">Authors</a>
+            <a class="toc-backref" href="#id16">Authors</a>
           </h2>
           <ul class="simple">
             <li>Coopdevs</li>
           </ul>
         </div>
         <div class="section" id="maintainers">
           <h2>
-            <a class="toc-backref" href="#id15">Maintainers</a>
+            <a class="toc-backref" href="#id17">Maintainers</a>
           </h2>
           <p>
             This module is part of the
             <a class="reference external" href="https://github.com/coopdevs/odoo14-addons/tree/14.0/odoo_instance">coopdevs/odoo14-addons</a>
             project on GitHub.
           </p>
           <p>You are welcome to contribute.</p>
```

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/static/src/img/icon.png` & `odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/static/src/img/icon.png`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/views/import_requirements_wizard_view.xml` & `odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/views/import_requirements_wizard_view.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/views/odoo_instance_actions.xml` & `odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/views/odoo_instance_actions.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/views/odoo_instance_menuitems.xml` & `odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/views/odoo_instance_menuitems.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/views/odoo_instance_module_version_views.xml` & `odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/views/odoo_instance_module_version_views.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/views/odoo_instance_searches.xml` & `odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/views/odoo_instance_searches.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/views/odoo_instance_view.xml` & `odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/views/odoo_instance_view.xml`

 * *Files 2% similar despite different names*

#### Comparing `odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/views/odoo_instance_view.xml` & `odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/views/odoo_instance_view.xml`

```diff
@@ -91,19 +91,21 @@
                       <field name="name"/>
                       <field name="status"/>
                     </tree>
                   </field>
                 </group>
               </page>
               <page string="Technic">
+                <group name="update_info" string="Update info" class="oe_edit_only">
+                  <button name="update_instance_info" type="object" string="Get from YAML" class="btn-secondary" icon="fa-cloud-download"/>
+                </group>
                 <group>
                   <field name="inventory_url" widget="url"/>
                   <field name="branch"/>
-                  <field name="odoo_release_id" options="{'no_create': True}" domain="[('odoo_version_id', '=', odoo_version_id)]"/>
-                  <button name="update_odoo_release" type="object" string="Get from YAML" class="btn-secondary oe_edit_only" icon="fa-cloud-download"/>
+                  <field name="odoo_release_id" options="{'no_create': True}" domain="[('odoo_version_id', '=', odoo_version_id)]" widget="badge"/>
                 </group>
                 <group>
                   <field name="server_information"/>
                   <field name="server_type"/>
                 </group>
                 <group string="Planned Deploys">
                   <field name="deploy_duration" widget="float_time"/>
@@ -122,14 +124,22 @@
                 <field name="available_windows" nolabel="1">
                   <tree editable="top" create="false" delete="false">
                     <field name="start_time" widget="datetime"/>
                     <field name="end_time" widget="datetime" string="Last deploy"/>
                     <button name="open_calendar_event_wizard" string="Plan Deploy" type="object"/>
                   </tree>
                 </field>
+                <group name="databases" string="Databases">
+                  <field name="database_ids" nolabel="1">
+                    <tree>
+                      <field name="name"/>
+                      <field name="is_test"/>
+                    </tree>
+                  </field>
+                </group>
                 <group string="Requirements">
                   <field name="requirements_url" widget="url" nolabel="1"/>
                   <group>
                     <button name="download_and_process_requirements_txt" string="Update Modules from URL" type="object" class="btn btn-secondary" icon="fa-refresh"/>
                   </group>
                   <field name="module_ids" nolabel="1" context="{'module_instance_ids': active_id}">
                     <tree editable="false" create="false" delete="false">
```

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/views/odoo_instance_window_wizard_view.xml` & `odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/views/odoo_instance_window_wizard_view.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/views/odoo_module_view.xml` & `odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/views/odoo_module_view.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/views/odoo_process_view.xml` & `odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/views/odoo_process_view.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/views/odoo_release_view.xml` & `odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/views/odoo_release_view.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/views/odoo_version_view.xml` & `odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/views/odoo_version_view.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/views/project_project_view.xml` & `odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/views/project_project_view.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/views/res_partner_view.xml` & `odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/views/res_partner_view.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/wizards/odoo_instance_window_wizard.py` & `odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/wizards/odoo_instance_window_wizard.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.1/odoo14_addon_odoo_instance.egg-info/PKG-INFO` & `odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo/addons/odoo_instance/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: odoo14-addon-odoo-instance
-Version: 14.0.1.1.1
-Summary: Manage Odoo instances with relevant information
-Home-page: https://www.coopdevs.org
-Author: Coopdevs
-License: AGPL-3
-Classifier: Programming Language :: Python
-Classifier: Framework :: Odoo
-Classifier: Framework :: Odoo :: 14.0
-Classifier: License :: OSI Approved :: GNU Affero General Public License v3
-Requires-Python: >=3.6
-
 =============
 Odoo Instance
 =============
 
 .. !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
    !! This file is generated by oca-gen-addon-readme !!
    !! changes will be overwritten.                   !!
@@ -50,14 +37,22 @@
 
 .. contents::
    :local:
 
 Changelog
 =========
 
+14.0.1.2.0 (2023-04-26)
+~~~~~~~~~~~~~~~~~~~~~~~
+
+**Features**
+
+- Manage databases
+
+
 14.0.1.1.1 (2023-04-25)
 ~~~~~~~~~~~~~~~~~~~~~~~
 
 **Bugfixes**
 
 - Upcrate module versions
 - Show installed module versions only in instance view
```

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.1/odoo14_addon_odoo_instance.egg-info/SOURCES.txt` & `odoo14-addon-odoo_instance-14.0.1.1.2.dev2/odoo14_addon_odoo_instance.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 odoo/addons/odoo_instance/data/odoo12_core_modules_data.xml
 odoo/addons/odoo_instance/data/odoo14_core_modules_app_data.xml
 odoo/addons/odoo_instance/data/odoo_version_data.xml
 odoo/addons/odoo_instance/models/__init__.py
 odoo/addons/odoo_instance/models/calendar_event.py
 odoo/addons/odoo_instance/models/import_requirements_wizard.py
 odoo/addons/odoo_instance/models/odoo_instance.py
+odoo/addons/odoo_instance/models/odoo_instance_database.py
 odoo/addons/odoo_instance/models/odoo_instance_module.py
 odoo/addons/odoo_instance/models/odoo_instance_process.py
 odoo/addons/odoo_instance/models/odoo_instance_window.py
 odoo/addons/odoo_instance/models/odoo_release.py
 odoo/addons/odoo_instance/models/odoo_version.py
 odoo/addons/odoo_instance/models/process_module_rel.py
 odoo/addons/odoo_instance/models/project_project.py
```

