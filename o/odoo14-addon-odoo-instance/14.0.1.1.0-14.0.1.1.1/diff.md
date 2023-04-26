# Comparing `tmp/odoo14-addon-odoo_instance-14.0.1.1.0.tar.gz` & `tmp/odoo14-addon-odoo_instance-14.0.1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odoo14-addon-odoo_instance-14.0.1.1.0.tar", last modified: Tue Apr 25 10:26:32 2023, max compression
+gzip compressed data, was "odoo14-addon-odoo_instance-14.0.1.1.1.tar", last modified: Tue Apr 25 22:45:02 2023, max compression
```

## Comparing `odoo14-addon-odoo_instance-14.0.1.1.0.tar` & `odoo14-addon-odoo_instance-14.0.1.1.1.tar`

### file list

```diff
@@ -1,74 +1,75 @@
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 10:26:32.225697 odoo14-addon-odoo_instance-14.0.1.1.0/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     3865 2023-04-25 10:26:32.225697 odoo14-addon-odoo_instance-14.0.1.1.0/PKG-INFO
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 10:26:32.219030 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 10:26:32.219030 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 10:26:32.222364 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     3453 2023-04-25 10:24:56.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/README.rst
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)       43 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/__init__.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1277 2023-04-25 10:24:56.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/__manifest__.py
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 10:26:32.222364 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/data/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      217 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/data/calendar_tags.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1396 2023-04-24 19:32:46.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/data/ir_cron.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)    95199 2023-04-24 19:27:51.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/data/odoo12_core_modules_data.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     9484 2023-04-24 19:27:51.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/data/odoo14_core_modules_app_data.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      705 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/data/odoo_version_data.xml
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 10:26:32.222364 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/models/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      273 2023-04-25 10:24:49.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/models/__init__.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      208 2023-04-24 19:27:51.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/models/calendar_event.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      488 2023-04-24 19:32:46.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/models/import_requirements_wizard.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)    21016 2023-04-25 10:24:49.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/models/odoo_instance.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     2469 2023-04-24 23:30:49.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/models/odoo_instance_module.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1377 2023-04-24 22:28:12.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/models/odoo_instance_process.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1790 2023-04-24 19:27:51.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/models/odoo_instance_window.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      456 2023-04-25 10:24:49.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/models/odoo_release.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      282 2023-04-25 10:24:49.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/models/odoo_version.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      474 2023-04-24 19:27:51.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/models/process_module_rel.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      182 2023-04-24 19:27:51.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/models/project_project.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      182 2023-04-24 19:27:51.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/models/res_partner.py
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 10:26:32.222364 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/readme/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1254 2023-04-24 17:29:42.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/readme/DESCRIPTION.rst
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      473 2023-04-25 10:24:56.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/readme/HISTORY.rst
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 10:26:32.222364 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/readme/newsfragments/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)       12 2023-04-24 18:45:09.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/readme/newsfragments/.gitignore
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 10:26:32.225697 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/security/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)       24 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/security/__init__.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1654 2023-04-25 10:24:56.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/security/ir.model.access.csv
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      383 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/security/security_groups.xml
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 10:26:32.222364 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/static/
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 10:26:32.225697 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/static/description/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)    13269 2023-04-25 10:24:56.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/static/description/index.html
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 10:26:32.222364 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/static/src/
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 10:26:32.225697 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/static/src/css/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)        0 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/static/src/css/project_instance.css
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 10:26:32.225697 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/static/src/img/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)    33659 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/static/src/img/icon.png
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 10:26:32.225697 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/static/src/js/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)        0 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/static/src/js/project_instance.js
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 10:26:32.225697 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/tests/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)        0 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/tests/__init__.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)        0 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/tests/test_project_instance.py
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 10:26:32.225697 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/views/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1049 2023-04-24 19:27:51.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/views/import_requirements_wizard_view.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     3034 2023-04-24 22:37:43.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/views/odoo_instance_actions.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1964 2023-04-25 10:24:49.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/views/odoo_instance_menuitems.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     4622 2023-04-25 10:24:49.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/views/odoo_instance_searches.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)    19080 2023-04-25 10:24:49.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/views/odoo_instance_view.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      971 2023-04-24 19:32:46.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/views/odoo_instance_window_wizard_view.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     3029 2023-04-25 00:00:05.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/views/odoo_module_view.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1674 2023-04-24 23:58:59.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/views/odoo_process_view.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     2254 2023-04-25 10:24:49.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/views/odoo_release_view.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1113 2023-04-25 10:24:49.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/views/odoo_version_view.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      920 2023-04-24 18:27:56.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/views/project_project_view.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1083 2023-04-24 20:15:25.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/views/res_partner_view.xml
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 10:26:32.225697 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/wizards/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)       94 2023-04-24 19:55:35.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/wizards/__init__.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     2309 2023-04-24 23:39:11.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/wizards/odoo_instance_window_wizard.py
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 10:26:32.225697 odoo14-addon-odoo_instance-14.0.1.1.0/odoo14_addon_odoo_instance.egg-info/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     3865 2023-04-25 10:26:32.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo14_addon_odoo_instance.egg-info/PKG-INFO
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     2769 2023-04-25 10:26:32.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo14_addon_odoo_instance.egg-info/SOURCES.txt
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)        1 2023-04-25 10:26:32.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo14_addon_odoo_instance.egg-info/dependency_links.txt
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)        1 2023-04-25 10:26:32.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo14_addon_odoo_instance.egg-info/not-zip-safe
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)       50 2023-04-25 10:26:32.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo14_addon_odoo_instance.egg-info/requires.txt
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)        5 2023-04-25 10:26:32.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo14_addon_odoo_instance.egg-info/top_level.txt
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)       38 2023-04-25 10:26:32.225697 odoo14-addon-odoo_instance-14.0.1.1.0/setup.cfg
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      100 2023-04-25 08:47:29.000000 odoo14-addon-odoo_instance-14.0.1.1.0/setup.py
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 22:45:02.626143 odoo14-addon-odoo_instance-14.0.1.1.1/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     4011 2023-04-25 22:45:02.626143 odoo14-addon-odoo_instance-14.0.1.1.1/PKG-INFO
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 22:45:02.619476 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 22:45:02.619476 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 22:45:02.619476 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     3599 2023-04-25 22:42:55.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/README.rst
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)       43 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/__init__.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1325 2023-04-25 20:41:20.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/__manifest__.py
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 22:45:02.622809 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/data/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      217 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/data/calendar_tags.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1389 2023-04-25 16:24:52.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/data/ir_cron.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)    95199 2023-04-24 19:27:51.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/data/odoo12_core_modules_data.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     9484 2023-04-24 19:27:51.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/data/odoo14_core_modules_app_data.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      705 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/data/odoo_version_data.xml
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 22:45:02.622809 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/models/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      273 2023-04-25 15:10:06.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/models/__init__.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      208 2023-04-25 15:10:06.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/models/calendar_event.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      484 2023-04-25 15:10:06.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/models/import_requirements_wizard.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)    17875 2023-04-25 19:58:28.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/models/odoo_instance.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     3078 2023-04-25 22:38:06.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/models/odoo_instance_module.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1345 2023-04-25 15:10:06.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/models/odoo_instance_process.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1791 2023-04-25 15:10:06.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/models/odoo_instance_window.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      452 2023-04-25 15:10:06.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/models/odoo_release.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      283 2023-04-25 15:10:06.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/models/odoo_version.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      475 2023-04-25 15:10:06.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/models/process_module_rel.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      183 2023-04-25 15:10:06.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/models/project_project.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      182 2023-04-25 15:10:06.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/models/res_partner.py
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 22:45:02.622809 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/readme/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1254 2023-04-24 17:29:42.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/readme/DESCRIPTION.rst
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      619 2023-04-25 22:42:50.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/readme/HISTORY.rst
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 22:45:02.622809 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/readme/newsfragments/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)       12 2023-04-24 18:45:09.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/readme/newsfragments/.gitignore
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 22:45:02.622809 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/security/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)       24 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/security/__init__.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1654 2023-04-25 10:24:56.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/security/ir.model.access.csv
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      383 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/security/security_groups.xml
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 22:45:02.619476 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/static/
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 22:45:02.622809 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/static/description/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)    13625 2023-04-25 22:42:55.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/static/description/index.html
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 22:45:02.619476 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/static/src/
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 22:45:02.622809 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/static/src/css/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)        0 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/static/src/css/project_instance.css
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 22:45:02.622809 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/static/src/img/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)    33659 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/static/src/img/icon.png
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 22:45:02.622809 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/static/src/js/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)        0 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/static/src/js/project_instance.js
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 22:45:02.622809 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/tests/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)        0 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/tests/__init__.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)        0 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/tests/test_project_instance.py
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 22:45:02.622809 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/views/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1049 2023-04-24 19:27:51.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/views/import_requirements_wizard_view.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     3617 2023-04-25 20:59:22.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/views/odoo_instance_actions.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     2679 2023-04-25 20:06:20.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/views/odoo_instance_menuitems.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1396 2023-04-25 19:54:54.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/views/odoo_instance_module_version_views.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     4622 2023-04-25 20:37:02.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/views/odoo_instance_searches.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)    19771 2023-04-25 22:36:30.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/views/odoo_instance_view.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      971 2023-04-24 19:32:46.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/views/odoo_instance_window_wizard_view.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     3311 2023-04-25 20:56:12.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/views/odoo_module_view.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1688 2023-04-25 20:43:09.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/views/odoo_process_view.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     2254 2023-04-25 10:24:49.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/views/odoo_release_view.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1113 2023-04-25 10:24:49.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/views/odoo_version_view.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      920 2023-04-24 18:27:56.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/views/project_project_view.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1083 2023-04-24 20:15:25.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/views/res_partner_view.xml
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 22:45:02.622809 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/wizards/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)       94 2023-04-24 19:55:35.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/wizards/__init__.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     2291 2023-04-25 15:10:06.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/wizards/odoo_instance_window_wizard.py
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 22:45:02.626143 odoo14-addon-odoo_instance-14.0.1.1.1/odoo14_addon_odoo_instance.egg-info/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     4011 2023-04-25 22:45:02.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo14_addon_odoo_instance.egg-info/PKG-INFO
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     2840 2023-04-25 22:45:02.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo14_addon_odoo_instance.egg-info/SOURCES.txt
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)        1 2023-04-25 22:45:02.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo14_addon_odoo_instance.egg-info/dependency_links.txt
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)        1 2023-04-25 22:45:02.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo14_addon_odoo_instance.egg-info/not-zip-safe
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)       50 2023-04-25 22:45:02.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo14_addon_odoo_instance.egg-info/requires.txt
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)        5 2023-04-25 22:45:02.000000 odoo14-addon-odoo_instance-14.0.1.1.1/odoo14_addon_odoo_instance.egg-info/top_level.txt
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)       38 2023-04-25 22:45:02.626143 odoo14-addon-odoo_instance-14.0.1.1.1/setup.cfg
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      100 2023-04-25 22:44:55.000000 odoo14-addon-odoo_instance-14.0.1.1.1/setup.py
```

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.0/PKG-INFO` & `odoo14-addon-odoo_instance-14.0.1.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo14-addon-odoo_instance
-Version: 14.0.1.1.0
+Version: 14.0.1.1.1
 Summary: Manage Odoo instances with relevant information
 Home-page: https://www.coopdevs.org
 Author: Coopdevs
 License: AGPL-3
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 14.0
@@ -50,14 +50,23 @@
 
 .. contents::
    :local:
 
 Changelog
 =========
 
+14.0.1.1.1 (2023-04-25)
+~~~~~~~~~~~~~~~~~~~~~~~
+
+**Bugfixes**
+
+- Upcrate module versions
+- Show installed module versions only in instance view
+
+
 14.0.1.1.0 (2023-04-25)
 ~~~~~~~~~~~~~~~~~~~~~~~
 
 **Features**
 
 - Handle odoo releases
```

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/README.rst` & `odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -37,14 +37,23 @@
 
 .. contents::
    :local:
 
 Changelog
 =========
 
+14.0.1.1.1 (2023-04-25)
+~~~~~~~~~~~~~~~~~~~~~~~
+
+**Bugfixes**
+
+- Upcrate module versions
+- Show installed module versions only in instance view
+
+
 14.0.1.1.0 (2023-04-25)
 ~~~~~~~~~~~~~~~~~~~~~~~
 
 **Features**
 
 - Handle odoo releases
```

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/__manifest__.py` & `odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/__manifest__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 {
     'name': 'Odoo Instance',
-    'version': '14.0.1.1.0',
+    'version': '14.0.1.1.1',
     'category': 'Project',
     'summary': 'Manage Odoo instances with relevant information',
     'author': 'Coopdevs',
     'website': 'https://www.coopdevs.org',
     'depends': ['base', 'contract', 'project', 'calendar'],
     'data': [
         'security/security_groups.xml',
         'security/ir.model.access.csv',
-        'views/odoo_instance_view.xml',        
+        'views/odoo_instance_view.xml',
         'views/odoo_module_view.xml',
         'views/odoo_instance_window_wizard_view.xml',
         'views/odoo_version_view.xml',
         'views/odoo_process_view.xml',
         'views/odoo_release_view.xml',
         'views/res_partner_view.xml',
         'views/project_project_view.xml',
+        'views/odoo_instance_module_version_views.xml',
         'views/odoo_instance_actions.xml',
         'views/odoo_instance_menuitems.xml',
         'views/odoo_instance_searches.xml',
         'data/ir_cron.xml',
         'data/calendar_tags.xml',
         'data/odoo_version_data.xml',
         'data/odoo14_core_modules_app_data.xml',
```

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/data/ir_cron.xml` & `odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/data/ir_cron.xml`

 * *Files 7% similar despite different names*

#### Comparing `odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/data/ir_cron.xml` & `odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/data/ir_cron.xml`

```diff
@@ -1,21 +1,21 @@
 <?xml version="1.0" encoding="utf-8"?>
 <odoo>
-  <!-- <record id="delete_past_orphan_windows_cron" model="ir.cron">
-        <field name="name">Delete past or orphan odoo.instance.window</field>
-        <field name="model_id" ref="model_odoo_instance_window"/>
-        <field name="state">code</field>
-        <field name="code">model.delete_past_or_orphan_windows()</field>
-        <field name="user_id" ref="base.user_root"/>
-        <field name="interval_number">1</field>
-        <field name="interval_type">days</field>
-        <field name="numbercall">-1</field>
-        <field name="doall" eval="False"/>
-        <field name="active" eval="True"/>
-    </record> -->
+  <record id="delete_past_orphan_windows_cron" model="ir.cron">
+    <field name="name">Delete past or orphan odoo.instance.window</field>
+    <field name="model_id" ref="model_odoo_instance_window"/>
+    <field name="state">code</field>
+    <field name="code">model.delete_past_or_orphan_windows()</field>
+    <field name="user_id" ref="base.user_root"/>
+    <field name="interval_number">1</field>
+    <field name="interval_type">days</field>
+    <field name="numbercall">-1</field>
+    <field name="doall" eval="False"/>
+    <field name="active" eval="True"/>
+  </record>
   <record id="cron_archive_or_delete_unassociated_module_versions" model="ir.cron">
     <field name="name">Archive or Delete Unassociated Module Versions</field>
     <field name="model_id" ref="model_odoo_instance_module_version"/>
     <field name="state">code</field>
     <field name="code">model.archive_or_delete_unassociated_module_versions()</field>
     <field name="user_id" ref="base.user_root"/>
     <field name="interval_number">1</field>
```

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/data/odoo12_core_modules_data.xml` & `odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/data/odoo12_core_modules_data.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/data/odoo14_core_modules_app_data.xml` & `odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/data/odoo14_core_modules_app_data.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/data/odoo_version_data.xml` & `odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/data/odoo_version_data.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/models/odoo_instance.py` & `odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/models/odoo_instance.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,36 @@
+import logging
+import re
 from datetime import datetime, time, timedelta
-from odoo import api, fields, models
-from odoo.exceptions import UserError
+
+import pytz
 import requests
-import logging
 import yaml
-import pytz
-import re
+
+from odoo import api, fields, models
+from odoo.exceptions import UserError
+
 _logger = logging.getLogger(__name__)
 
 
 class OdooInstance(models.Model):
     _name = 'odoo.instance'
     _description = 'Odoo Instance'
     _inherit = ['mail.thread', 'mail.activity.mixin']
     # General Information
 
     name = fields.Char(string='Instance Name', required=True)
     description = fields.Text(string='Instance Description')
     start_date = fields.Date(string='Start Date')
-    
+
     project_id = fields.Many2one('project.project', string='Project', ondelete='set null')
-    helpdesk_team_id = fields.Many2one('helpdesk.team', string='Helpdesk Team', ondelete='set null')    
+    helpdesk_team_id = fields.Many2one('helpdesk.team', string='Helpdesk Team', ondelete='set null')
     instance_url = fields.Char(string='Instance URL')
 
-    partner_id = fields.Many2one('res.partner', string='Client', required=True)                                
+    partner_id = fields.Many2one('res.partner', string='Client', required=True)
     client_contact_id = fields.Many2one(
         'res.partner', string='Client Contact', domain=[('type', '=', 'contact')])
 
     technician_ids = fields.Many2many(
         'res.users', string='Technicians', relation='odoo_instance_technician_rel')
     functional_ids = fields.Many2many(
         'res.users', string='Functional Experts', relation='odoo_instance_functional_rel')
@@ -38,26 +41,26 @@
         ('in_progress', 'In Progress'),
         ('running', 'Running'),
         ('paused', 'Paused'),
         ('cancelled', 'Terminated')
     ], string='State', default='in_progress')
 
     # Technical Information
-    
+
     inventory_url = fields.Char(string='Inventory URL')
     branch = fields.Char(string='Branch', required=True)
     odoo_release_id = fields.Many2one('odoo.release', string='Odoo Release')
     instance_type = fields.Selection([
         ('test', 'Test'),
         ('production', 'Production'),
     ], string="Instance Type", required=True)
 
     deploy_schedule = fields.One2many(
         'odoo.instance.schedule', 'instance_id', string="Deploy Schedule")
-    
+
     unavailable_windows = fields.One2many(
         'odoo.instance.unavailable_schedule', 'instance_id', string='Unavailable Windows')
 
     deploy_event_ids = fields.One2many(
         'calendar.event', 'instance_id', string='Deploy Events')
 
     server_information = fields.Text(string='Server Information')
@@ -77,60 +80,43 @@
         ('cpx51', 'cpx51'),
     ], string="Server Type")
 
     troubleshooting_ids = fields.One2many('odoo.instance.troubleshooting', 'instance_id', string='Troubleshooting')
     deploy_duration = fields.Float(
         string='Deploy Duration', default=1.0, help="Duration in hours")
 
-
-
     # Functional Information
     process_ids = fields.Many2many(
         'odoo.instance.process',
         'odoo_instance_process_rel',
         'instance_id',
         'process_id',
         string='Processes'
     )
     available_windows = fields.One2many(
         'odoo.instance.window', 'instance_id', string='Available Windows')
 
     functional_requirement_ids = fields.One2many(
         'odoo.instance.functional_requirement', 'odoo_instance_id', string='Functional Requirements')
 
-
     # Commercial Information
     contact_role_id = fields.Many2one('res.partner', string='Rol de Contacto')
     maintenance_contract_ids = fields.Char(string='Contratos de Mantenimiento')
     support_contract_ids = fields.Char(string='Contratos de Soporte')
     implementation_contract_id = fields.Char(
         string='Contrato de Implementación')
 
-
     # maintenance_contract_ids = fields.Many2many('contract.contract', string='Contratos de Mantenimiento', relation='odoo_instance_maintenance_contract_rel')
     # support_contract_ids = fields.Many2many('contract.contract', string='Contratos de Soporte', relation='odoo_instance_support_contract_rel')
     # implementation_contract_id = fields.Many2one('contract.contract', string='Contrato de Implementación', relation='odoo_instance_implementation_contract_rel')
 
     def toggle_state(self):
-            state_order = ['in_progress', 'running', 'paused', 'cancelled']
-            next_state_index = (state_order.index(self.state) + 1) % len(state_order)
-            self.state = state_order[next_state_index]
-
-    @api.depends('state')
-    def _compute_state_color(self):
-        color_map = {
-            'in_progress': 'o_status_warning',
-            'running': 'o_status_success',
-            'paused': 'o_status_secondary',
-            'cancelled': 'o_status_danger',
-        }
-        for record in self:
-            record.state_color = color_map[record.state]
-
-    state_color = fields.Char(compute='_compute_state_color', store=True)    
+        state_order = ['in_progress', 'running', 'paused', 'cancelled']
+        next_state_index = (state_order.index(self.state) + 1) % len(state_order)
+        self.state = state_order[next_state_index]
 
 
     def download_and_process_requirements_txt(self):
         if not self.requirements_url:
             return
         response = requests.get(self.requirements_url)
         if response.status_code == 200:
@@ -157,61 +143,64 @@
             'target': 'new',
         }
 
     def import_requirements_txt(self, file_content):
         """Parse a requirements.txt file and update the modules field."""
         Module = self.env['odoo.instance.module']
         ModuleVersion = self.env['odoo.instance.module.version']
-        modules_to_link = []        
+        modules_to_link = []
 
         current_versions = ModuleVersion.search([
-                ('instance_ids', 'in', [self.id]),
-            ], limit=1)
+            ('instance_ids', 'in', [self.id]),
+        ], limit=1)
         for version in current_versions:
             # delete the instance in the version
             version.instance_ids = [(3, self.id)]
             # if the version is not used by any instance, delete it
             if not version.instance_ids:
                 version.unlink()
-        
+
         for line in file_content.splitlines():
             line = line.strip()
             if not line or '==' not in line:
                 continue
 
             module_name, version = line.split('==')
             module = Module.search(
                 [('technical_name', '=', module_name)], limit=1)
 
             if not module:
                 module_data = self.get_module_name_from_pypi(module_name)
-        
+
                 module = Module.create({
                     'technical_name': module_data['technical_name'],
                     'name': module_data['name'],
-                    'module_type': module_data['module_type'],                    
-                    #assign odoo_version_id only if odoo_version_id.d is a int
+                    'module_type': module_data['module_type'],
                     'odoo_version_id': module_data['odoo_version_id'],
-                    #'odoo_version_id': module_data['odoo_version_id'].id,
                     'pypi_url': f'https://pypi.org/project/{module_name}/',
                     'is_odoo_module': module_data['is_odoo_module'],
                 })
 
             version_record = ModuleVersion.search([
                 ('name', '=', version),
                 ('module_id', '=', module.id),
-                ('instance_ids', 'in', [self.id]),
             ], limit=1)
 
-            if not version_record:
+            if version_record:
+                # Update the existing version record by adding the instance
+                _logger.critical("Version found %s", version_record.instance_ids)
+                version_record.instance_ids |= self
+            else:
+                # Create a new version record
+                _logger.critical("Version not found, creating it")
                 version_record = ModuleVersion.create({
                     'name': version,
                     'module_id': module.id,
+                    'instance_ids': [(4, self.id)],
                 })
-                version_record.instance_ids |= self
 
             modules_to_link.append(module.id)
 
         self.module_ids = [(6, 0, modules_to_link)]
         ModuleVersion.archive_or_delete_unassociated_module_versions()
 
     def get_module_name_from_pypi(self, technical_name):
@@ -236,21 +225,21 @@
                 module_data['is_odoo_module'] = True
 
             if module_data['is_odoo_module']:
                 # Check if the module is Odoo core or OCA
                 if 'oca' in module_data['home_page'].lower():
                     module_data['module_type'] = 'OCA'
 
-
                 # extract odoo version from version key. Example: version	"14.0.1.0.3"
                 odoo_version_pattern = r"(\d{1,2}\.\d{1,2})"
                 match = re.search(odoo_version_pattern, data['info']['version'])
                 if match:
                     module_data['odoo_version'] = match.group(1)
-                    module_data['odoo_version_id'] = self.env['odoo.version'].search([('name', '=', match.group(1))], limit=1).id
+                    module_data['odoo_version_id'] = self.env['odoo.version'].search([('name', '=', match.group(1))],
+                                                                                     limit=1).id
 
         else:
             _logger.warning(
                 f'Error fetching module name from pypi.org for {technical_name}')
 
         return module_data
 
@@ -293,14 +282,15 @@
                     deploy_end_time = available_end_time - timedelta(hours=instance.deploy_duration)
                     if deploy_end_time > available_start_time:
                         instance.available_windows.create({
                             'instance_id': instance.id,
                             'start_time': available_start_time.astimezone(pytz.utc).replace(tzinfo=None),
                             'end_time': deploy_end_time.astimezone(pytz.utc).replace(tzinfo=None),
                         })
+            instance.action_delete_past_or_orphan_windows()
 
     @api.onchange('odoo_version_id')
     def _onchange_odoo_version_id(self):
         if self.odoo_version_id:
             self.module_ids = False
             return {
                 'domain': {
@@ -310,115 +300,60 @@
         else:
             return {
                 'domain': {
                     'module_ids': []
                 }
             }
 
-    def find_next_available_window(instance, now_local, required_duration):
-        user_tz = pytz.timezone(instance.env.user.tz or 'UTC')
-        now_utc = now_local.astimezone(pytz.utc)
-
-        for i in range(7):
-            current_date = now_utc.date() + timedelta(days=i)
-            current_weekday = str(current_date.weekday())
-
-            unavailable_periods = []
-            for schedule in instance.unavailable_windows:
-                if schedule.day_of_week == current_weekday:
-                    schedule_hour = int(schedule.start_time)
-                    schedule_minute = int((schedule.start_time % 1) * 60)
-                    schedule_time = time(schedule_hour, schedule_minute, 0)
-                    schedule_end_hour = int(schedule.end_time)
-                    schedule_end_minute = int((schedule.end_time % 1) * 60)
-                    schedule_end_time = time(schedule_end_hour, schedule_end_minute, 0)
-
-                    start_time = user_tz.localize(
-                        datetime.combine(current_date, schedule_time))
-                    end_time = user_tz.localize(
-                        datetime.combine(current_date, schedule_end_time))
-
-                    unavailable_periods.append((start_time, end_time))
-
-            available_start_time = datetime.combine(current_date, time.min).replace(tzinfo=pytz.utc)
-            available_end_time = datetime.combine(current_date, time.max).replace(tzinfo=pytz.utc)
-
-            if not unavailable_periods:
-                duration = (available_end_time - available_start_time).total_seconds() / 3600
-                if duration >= required_duration:
-                    return available_start_time
-
-            unavailable_periods.sort()
-
-        for period_start, period_end in unavailable_periods:
-            if period_start > available_start_time:
-                duration = (period_start - available_start_time).total_seconds() / 3600
-                if duration >= required_duration:
-                    return available_start_time
-
-            available_start_time = period_end
-
-        if available_end_time > available_start_time:
-            duration = (available_end_time - available_start_time).total_seconds() / 3600
-            if duration >= required_duration:
-                return available_start_time
-
-        return None
-
-    def get_available_window_from_schedule(self, schedule, current_date, user_tz):
-        schedule_hour = int(schedule.start_time)
-        schedule_minute = int((schedule.start_time % 1) * 60)
-        schedule_time = time(schedule_hour, schedule_minute, 0)
-        schedule_end_hour = int(schedule.end_time)
-        schedule_end_minute = int((schedule.end_time % 1) * 60)
-        schedule_end_time = time(schedule_end_hour, schedule_end_minute, 0)
-
-        start_time = user_tz.localize(datetime.combine(current_date, schedule_time))
-        end_time = user_tz.localize(datetime.combine(current_date, schedule_end_time))
-
-        return start_time, end_time
     def open_instance_url(self):
-            self.ensure_one()
-            if not self.instance_url:
-                raise UserError(("No hay URL para esta instancia."))
-            return {
-                'type': 'ir.actions.act_url',
-                'url': self.instance_url,
-                'target': 'new',
-            }
+        self.ensure_one()
+        if not self.instance_url:
+            raise UserError(("No hay URL para esta instancia."))
+        return {
+            'type': 'ir.actions.act_url',
+            'url': self.instance_url,
+            'target': 'new',
+        }
+
     def update_odoo_release(self):
-            for instance in self:
-                inventory_url = instance.inventory_url
-                branch = instance.branch
-                raw_inventory_url = f"{inventory_url}/-/raw/{branch}/inventory/group_vars/all.yml"
-                response = requests.get(raw_inventory_url)
-
-                if response.status_code == 200:
-                    inventory_data = yaml.safe_load(response.text)
-                    odoo_release_str = inventory_data.get('odoo_role_odoo_release')
-
-                    if odoo_release_str:
-                        odoo_version, release_date_str = odoo_release_str.split('_')
-                        release_date = fields.Date.from_string(release_date_str)
-
-                        odoo_version_id = self.env['odoo.version'].search([('name', '=', odoo_version)], limit=1)
-                        if odoo_version_id:
-                            odoo_release = self.env['odoo.release'].search([
-                                ('name', '=', odoo_release_str),
-                                ('odoo_version_id', '=', odoo_version_id.id)
-                            ], limit=1)
-
-                            if not odoo_release:
-                                odoo_release = self.env['odoo.release'].create({
-                                    'name': odoo_release_str,
-                                    'release_date': release_date,
-                                    'odoo_version_id': odoo_version_id.id,
-                                })
+        for instance in self:
+            inventory_url = instance.inventory_url
+            branch = instance.branch
+            raw_inventory_url = f"{inventory_url}/-/raw/{branch}/inventory/group_vars/all.yml"
+            response = requests.get(raw_inventory_url)
+
+            if response.status_code == 200:
+                inventory_data = yaml.safe_load(response.text)
+                odoo_release_str = inventory_data.get('odoo_role_odoo_release')
+
+                if odoo_release_str:
+                    odoo_version, release_date_str = odoo_release_str.split('_')
+                    release_date = fields.Date.from_string(release_date_str)
+
+                    odoo_version_id = self.env['odoo.version'].search([('name', '=', odoo_version)], limit=1)
+                    if odoo_version_id:
+                        odoo_release = self.env['odoo.release'].search([
+                            ('name', '=', odoo_release_str),
+                            ('odoo_version_id', '=', odoo_version_id.id)
+                        ], limit=1)
+
+                        if not odoo_release:
+                            odoo_release = self.env['odoo.release'].create({
+                                'name': odoo_release_str,
+                                'release_date': release_date,
+                                'odoo_version_id': odoo_version_id.id,
+                            })
+
+                        instance.odoo_release_id = odoo_release
+    def action_delete_past_or_orphan_windows(self):
+        self.env["odoo.instance.window"].delete_past_or_orphan_windows()                        
+    def action_clear_windows(self):        
+        self.env['odoo.instance.window'].search([('instance_id', '=', self.id)]).unlink()
+
 
-                            instance.odoo_release_id = odoo_release
 
 class OdooInstanceSchedule(models.Model):
     _name = 'odoo.instance.schedule'
     _description = 'Deploy Schedule'
 
     instance_id = fields.Many2one('odoo.instance', string="Instance")
     day_of_week = fields.Selection([
@@ -462,14 +397,15 @@
         ('postmortem', 'Post Mortem'),
         ('config', 'Configuration'),
         ('other', 'Other')
     ], string='Type', default='config', required=True)
 
     instance_id = fields.Many2one('odoo.instance', string='Instance', ondelete='cascade')
 
+
 class OdooInstanceUnavailableSchedule(models.Model):
     _name = 'odoo.instance.unavailable_schedule'
     _description = 'Unavailable Deploy Schedule'
 
     instance_id = fields.Many2one('odoo.instance', string="Instance")
     day_of_week = fields.Selection([
         ('0', 'Monday'),
@@ -480,18 +416,18 @@
         ('5', 'Saturday'),
         ('6', 'Sunday'),
     ], string="Day of the Week", required=True)
     start_time = fields.Float(string="Start Time", required=True)
     end_time = fields.Float(string="End Time", required=True)
 
     def get_unavailable_periods(self, current_date, user_tz):
-            schedule_hour = int(self.start_time)
-            schedule_minute = int((self.start_time % 1) * 60)
-            schedule_time = time(schedule_hour, schedule_minute, 0)
-            schedule_end_hour = int(self.end_time)
-            schedule_end_minute = int((self.end_time % 1) * 60)
-            schedule_end_time = time(schedule_end_hour, schedule_end_minute, 0)
+        schedule_hour = int(self.start_time)
+        schedule_minute = int((self.start_time % 1) * 60)
+        schedule_time = time(schedule_hour, schedule_minute, 0)
+        schedule_end_hour = int(self.end_time)
+        schedule_end_minute = int((self.end_time % 1) * 60)
+        schedule_end_time = time(schedule_end_hour, schedule_end_minute, 0)
 
-            start_time = user_tz.localize(datetime.combine(current_date, schedule_time))
-            end_time = user_tz.localize(datetime.combine(current_date, schedule_end_time))
+        start_time = user_tz.localize(datetime.combine(current_date, schedule_time))
+        end_time = user_tz.localize(datetime.combine(current_date, schedule_end_time))
 
-            return (start_time, end_time)    
+        return (start_time, end_time)
```

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/models/odoo_instance_module.py` & `odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/models/odoo_instance_module.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,68 +1,88 @@
+import logging
+
+import requests
 
 from odoo import api, fields, models
 
-import requests
-import logging
 _logger = logging.getLogger(__name__)
 
+
 class OdooInstanceModule(models.Model):
     _name = 'odoo.instance.module'
     _description = 'Odoo Instance Module'
 
     name = fields.Char(string='Name', required=True)
     technical_name = fields.Char(string='Technical Name', required=True)
     is_odoo_module = fields.Boolean(string='Is Odoo Module', default=True)
     pypi_url = fields.Char(string='PyPI URL')
     version_ids = fields.One2many(
         'odoo.instance.module.version', 'module_id', string='Versions')
     odoo_version_id = fields.Many2one('odoo.version', string="Odoo Version")
     module_type = fields.Selection([
         ('core', 'Odoo Core'),
         ('OCA', 'OCA'),
-        ('custom', 'Custom'),        
+        ('custom', 'Custom'),
         ('other', 'Other'),
         ('dep', 'Dependency')
     ], string='Module Type', default='custom')
 
     instance_ids = fields.Many2many(
-            'odoo.instance', string='Instances',
-            compute='_compute_instance_ids', readonly=True, store=True)
+        'odoo.instance', string='Instances',
+        compute='_compute_instance_ids', readonly=True, store=True)
 
+    process_ids = fields.Many2many(
+        "odoo.instance.process",
+        "process_module_rel",
+        "module_id",
+        "process_id",
+        string="Processes"
+    )
+
+    @api.onchange('version_ids.instance_ids')
     @api.depends('version_ids.instance_ids')
     def _compute_instance_ids(self):
         for record in self:
             instance_ids = self.env['odoo.instance']
             for version in record.version_ids:
                 instance_ids |= version.instance_ids
             record.instance_ids = instance_ids
 
-
     def fetch_pypi_information(self):
         package_info_url = f'https://pypi.org/pypi/{self.name}/json'
         response = requests.get(package_info_url)
         if response.status_code == 200:
             package_data = response.json()
             self.display_name = package_data['info']['name']
             self.is_odoo_module = 'odoo' in package_data['info']['keywords'].lower(
             )
 
-
 class OdooInstanceModuleVersion(models.Model):
     _name = 'odoo.instance.module.version'
     _description = 'Odoo Instance Module Version'
 
     name = fields.Char(string='Version', required=True)
     module_id = fields.Many2one(
         'odoo.instance.module', string='Module', required=True, ondelete='cascade')
     instance_ids = fields.Many2many(
         "odoo.instance",
         "module_version_instance_rel",
         "version_id",
         "instance_id",
         string="Instances",
     )
-    @api.model  
+
+    @api.model
     def archive_or_delete_unassociated_module_versions(self):
-        unassociated_module_versions = self.search([('instance_ids', '=', False)])
+        unassociated_module_versions = self.search(
+            [('instance_ids', '=', False)])
         unassociated_module_versions.unlink()
-
+        
+    @api.model
+    def search(self, args, offset=0, limit=None, order=None, count=False):
+        context_instance_id = self._context.get("module_instance_ids")
+        if context_instance_id:
+            args.append(("instance_ids", "in", [context_instance_id]))
+
+        return super(OdooInstanceModuleVersion, self).search(
+            args, offset, limit, order, count
+        )
```

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/models/odoo_instance_process.py` & `odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/models/odoo_instance_process.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,37 @@
-from odoo import fields, models, api
 import logging
 
+from odoo import fields, models, api
+
+
 class OdooInstanceProcess(models.Model):
     _logger = logging.getLogger(__name__)
     _name = 'odoo.instance.process'
     _description = 'Instance Process'
 
     name = fields.Char(string="Name", required=True)
     description = fields.Text(string="Description")
     module_ids = fields.Many2many(
         "odoo.instance.module",
         "process_module_rel",
         "process_id",
         "module_id",
         string="Related Modules",
         search=['|', ('name', 'ilike', '%search%'),
-                    ('technical_name', 'ilike', '%search%')]
+                ('technical_name', 'ilike', '%search%')]
     )
-    handbook_url = fields.Char(string="Handbook URL")    
+    handbook_url = fields.Char(string="Handbook URL")
     odoo_version_id = fields.Many2one("odoo.version", string="Odoo Version", required=True)
     instance_ids = fields.Many2many(
-            'odoo.instance', 
-            compute='compute_instance_ids', 
-            string='Instances',
-            search='search_instance_ids'
-        )
-    
+        'odoo.instance',
+        compute='compute_instance_ids',
+        string='Instances',
+        search='search_instance_ids'
+    )
+
     def compute_instance_ids(self):
         for record in self:
             instance_ids = self.env['odoo.instance'].search([('process_ids', 'in', record.id)])
             record.instance_ids = instance_ids.ids
 
     @api.model
     def search_instance_ids(self, operator, value):
```

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/models/odoo_instance_window.py` & `odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/models/odoo_instance_window.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+import logging
+
 from odoo import api, fields, models
 from odoo.exceptions import ValidationError
-import logging
 
 _logger = logging.getLogger(__name__)
 
 
 class OdooInstanceWindow(models.Model):
     _name = 'odoo.instance.window'
     _description = 'Available Deployment Window'
```

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/readme/DESCRIPTION.rst` & `odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/readme/DESCRIPTION.rst`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/security/ir.model.access.csv` & `odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/security/ir.model.access.csv`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/static/description/index.html` & `odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/static/description/index.html`

 * *Files 2% similar despite different names*

#### Comparing `odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/static/description/index.html` & `odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/static/description/index.html`

```diff
@@ -394,131 +394,146 @@
       </blockquote>
       <p>
         <strong>Table of contents</strong>
       </p>
       <div class="contents local topic" id="contents">
         <ul class="simple">
           <li>
-            <a class="reference internal" href="#changelog" id="id5">Changelog</a>
+            <a class="reference internal" href="#changelog" id="id6">Changelog</a>
             <ul>
               <li>
-                <a class="reference internal" href="#id1" id="id6">14.0.1.1.0 (2023-04-25)</a>
+                <a class="reference internal" href="#id1" id="id7">14.0.1.1.1 (2023-04-25)</a>
               </li>
               <li>
-                <a class="reference internal" href="#id2" id="id7">14.0.1.0.1 (2023-04-25)</a>
+                <a class="reference internal" href="#id2" id="id8">14.0.1.1.0 (2023-04-25)</a>
               </li>
               <li>
-                <a class="reference internal" href="#id3" id="id8">14.0.1.0.0 (2023-04-24)</a>
+                <a class="reference internal" href="#id3" id="id9">14.0.1.0.1 (2023-04-25)</a>
               </li>
               <li>
-                <a class="reference internal" href="#id4" id="id9">14.0.0.2.0 (2023-04-24)</a>
+                <a class="reference internal" href="#id4" id="id10">14.0.1.0.0 (2023-04-24)</a>
+              </li>
+              <li>
+                <a class="reference internal" href="#id5" id="id11">14.0.0.2.0 (2023-04-24)</a>
               </li>
             </ul>
           </li>
           <li>
-            <a class="reference internal" href="#bug-tracker" id="id10">Bug Tracker</a>
+            <a class="reference internal" href="#bug-tracker" id="id12">Bug Tracker</a>
           </li>
           <li>
-            <a class="reference internal" href="#credits" id="id11">Credits</a>
+            <a class="reference internal" href="#credits" id="id13">Credits</a>
             <ul>
               <li>
-                <a class="reference internal" href="#authors" id="id12">Authors</a>
+                <a class="reference internal" href="#authors" id="id14">Authors</a>
               </li>
               <li>
-                <a class="reference internal" href="#maintainers" id="id13">Maintainers</a>
+                <a class="reference internal" href="#maintainers" id="id15">Maintainers</a>
               </li>
             </ul>
           </li>
         </ul>
       </div>
       <div class="section" id="changelog">
         <h1>
-          <a class="toc-backref" href="#id5">Changelog</a>
+          <a class="toc-backref" href="#id6">Changelog</a>
         </h1>
         <div class="section" id="id1">
           <h2>
-            <a class="toc-backref" href="#id6">14.0.1.1.0 (2023-04-25)</a>
+            <a class="toc-backref" href="#id7">14.0.1.1.1 (2023-04-25)</a>
+          </h2>
+          <p>
+            <strong>Bugfixes</strong>
+          </p>
+          <ul class="simple">
+            <li>Upcrate module versions</li>
+            <li>Show installed module versions only in instance view</li>
+          </ul>
+        </div>
+        <div class="section" id="id2">
+          <h2>
+            <a class="toc-backref" href="#id8">14.0.1.1.0 (2023-04-25)</a>
           </h2>
           <p>
             <strong>Features</strong>
           </p>
           <ul class="simple">
             <li>Handle odoo releases</li>
           </ul>
         </div>
-        <div class="section" id="id2">
+        <div class="section" id="id3">
           <h2>
-            <a class="toc-backref" href="#id7">14.0.1.0.1 (2023-04-25)</a>
+            <a class="toc-backref" href="#id9">14.0.1.0.1 (2023-04-25)</a>
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
-        <div class="section" id="id3">
+        <div class="section" id="id4">
           <h2>
-            <a class="toc-backref" href="#id8">14.0.1.0.0 (2023-04-24)</a>
+            <a class="toc-backref" href="#id10">14.0.1.0.0 (2023-04-24)</a>
           </h2>
           <p>
             <strong>Features</strong>
           </p>
           <ul class="simple">
             <li>Rename models and split logic in files</li>
           </ul>
         </div>
-        <div class="section" id="id4">
+        <div class="section" id="id5">
           <h2>
-            <a class="toc-backref" href="#id9">14.0.0.2.0 (2023-04-24)</a>
+            <a class="toc-backref" href="#id11">14.0.0.2.0 (2023-04-24)</a>
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
-          <a class="toc-backref" href="#id10">Bug Tracker</a>
+          <a class="toc-backref" href="#id12">Bug Tracker</a>
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
-          <a class="toc-backref" href="#id11">Credits</a>
+          <a class="toc-backref" href="#id13">Credits</a>
         </h1>
         <div class="section" id="authors">
           <h2>
-            <a class="toc-backref" href="#id12">Authors</a>
+            <a class="toc-backref" href="#id14">Authors</a>
           </h2>
           <ul class="simple">
             <li>Coopdevs</li>
           </ul>
         </div>
         <div class="section" id="maintainers">
           <h2>
-            <a class="toc-backref" href="#id13">Maintainers</a>
+            <a class="toc-backref" href="#id15">Maintainers</a>
           </h2>
           <p>
             This module is part of the
             <a class="reference external" href="https://github.com/coopdevs/odoo14-addons/tree/14.0/odoo_instance">coopdevs/odoo14-addons</a>
             project on GitHub.
           </p>
           <p>You are welcome to contribute.</p>
```

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/static/src/img/icon.png` & `odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/static/src/img/icon.png`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/views/import_requirements_wizard_view.xml` & `odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/views/import_requirements_wizard_view.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/views/odoo_instance_actions.xml` & `odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/views/odoo_instance_actions.xml`

 * *Files 24% similar despite different names*

#### Comparing `odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/views/odoo_instance_actions.xml` & `odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/views/odoo_instance_actions.xml`

```diff
@@ -18,24 +18,24 @@
       <field name="context">{'search_default_my_instances': 1}</field>
     </record>
     <!-- Action for odoo.instance.module -->
     <record id="odoo_instance_module_action" model="ir.actions.act_window">
       <field name="name">Modules</field>
       <field name="type">ir.actions.act_window</field>
       <field name="res_model">odoo.instance.module</field>
-      <field name="view_mode">tree,form</field>
+      <field name="view_mode">tree,form,kanban</field>
       <field name="view_id" ref="odoo_instance_module_tree"/>
       <field name="context">{'search_default_is_odoo_module': 1}</field>
     </record>
     <!-- Action for odoo.instance.process -->
     <record id="odoo_instance_process_action" model="ir.actions.act_window">
       <field name="name">Processes</field>
       <field name="type">ir.actions.act_window</field>
       <field name="res_model">odoo.instance.process</field>
-      <field name="view_mode">tree,form</field>
+      <field name="view_mode">tree,form,kanban</field>
       <field name="view_id" ref="odoo_instance_process_tree"/>
     </record>
     <!-- Action for odoo.instance.process -->
     <record id="odoo_version_action" model="ir.actions.act_window">
       <field name="name">Odoo Versions</field>
       <field name="type">ir.actions.act_window</field>
       <field name="res_model">odoo.version</field>
@@ -50,9 +50,18 @@
     </record>
     <record id="odoo_instance_v14_action" model="ir.actions.act_window">
       <field name="name">Odoo 14.0 Instances</field>
       <field name="res_model">odoo.instance</field>
       <field name="view_mode">tree,form</field>
       <field name="domain">[('odoo_version_id.name', '=', '14.0')]</field>
     </record>
+    <!-- Action for odoo.instance.module.version -->
+    <record id="action_odoo_instance_module_version" model="ir.actions.act_window">
+      <field name="name">Odoo Instance Module Versions</field>
+      <field name="res_model">odoo.instance.module.version</field>
+      <field name="view_mode">tree,form</field>
+      <field name="help" type="html">
+        <p class="oe_view_nocontent_create">Click to create a new Odoo Instance Module Version.</p>
+      </field>
+    </record>
   </data>
 </odoo>
```

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/views/odoo_instance_menuitems.xml` & `odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/views/odoo_instance_menuitems.xml`

 * *Files 22% similar despite different names*

#### Comparing `odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/views/odoo_instance_menuitems.xml` & `odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/views/odoo_instance_menuitems.xml`

```diff
@@ -4,23 +4,37 @@
     <!-- Menu item for odoo.instance -->
     <menuitem id="odoo_instance_menu" name="Odoo Instances" action="odoo_instance_action" web_icon="odoo_instance,static/src/img/icon.png"/>
     <!-- Menu item for odoo.instance folded -->
     <menuitem id="odoo_instances_menu_versions" name="Instances" parent="odoo_instance_menu" sequence="10"/>
     <!-- Menu item for odoo.instance.process -->
     <menuitem id="menu_odoo_instance_process" name="Processes" parent="odoo_instance_menu" sequence="20" action="odoo_instance_process_action"/>
     <!-- Menu item for odoo.instance.module -->
-    <menuitem id="menu_odoo_instance_module" name="Modules" parent="odoo_instance_menu" sequence="30" action="odoo_instance_module_action"/>
+    <menuitem id="menu_odoo_instance_modules" name="Modules" parent="odoo_instance_menu" sequence="30"/>
     <!-- Menu item for odoo.instance.version -->
     <menuitem id="menu_odoo_version" name="Odoo Versions" parent="odoo_instance_menu" sequence="40" action="odoo_version_action"/>
     <!-- Menu item for 12.0 instances -->
     <menuitem id="odoo_instance_v12_menu" name="Odoo 12.0 Instances" parent="odoo_instances_menu_versions" action="odoo_instance_v12_action" sequence="10"/>
     <!-- Menu item for 14.0 instances -->
     <menuitem id="odoo_instance_v14_menu" name="Odoo 14.0 Instances" parent="odoo_instances_menu_versions" action="odoo_instance_v14_action" sequence="20"/>
     <!-- Odoo Release menu item -->
     <record id="menu_odoo_release" model="ir.ui.menu">
       <field name="name">Odoo Releases</field>
       <field name="parent_id" ref="odoo_instance_menu"/>
       <field name="action" ref="action_odoo_release"/>
       <field name="sequence" eval="50"/>
     </record>
+    <!-- Menu for odoo.instance.module -->
+    <record id="menu_odoo_instance_module" model="ir.ui.menu">
+      <field name="name">Modules</field>
+      <field name="sequence">10</field>
+      <field name="parent_id" ref="menu_odoo_instance_modules"/>
+      <field name="action" ref="odoo_instance_module_action"/>
+    </record>
+    <!-- Menu for odoo.instance.module.version -->
+    <record id="menu_odoo_instance_module_version" model="ir.ui.menu">
+      <field name="name">Module Versions</field>
+      <field name="sequence">20</field>
+      <field name="parent_id" ref="menu_odoo_instance_modules"/>
+      <field name="action" ref="action_odoo_instance_module_version"/>
+    </record>
   </data>
 </odoo>
```

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/views/odoo_instance_searches.xml` & `odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/views/odoo_instance_searches.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/views/odoo_instance_view.xml` & `odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/views/odoo_instance_view.xml`

 * *Files 3% similar despite different names*

#### Comparing `odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/views/odoo_instance_view.xml` & `odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/views/odoo_instance_view.xml`

```diff
@@ -30,28 +30,28 @@
             <group>
               <field name="instance_url" class="oe_edit_only" edit_only="1"/>
               <group>
                 <field name="project_id"/>
                 <field name="helpdesk_team_id"/>
               </group>
               <group>
-                <field name="partner_id"/>
+                <field name="partner_id" widget="res_partner_many2one"/>
                 <field name="client_contact_id"/>
               </group>
               <group>
                 <field name="odoo_version_id"/>
               </group>
               <group>
                 <field name="state"/>
                 <field name="instance_type"/>
                 <!-- <field name="contact_role_id" /> -->
               </group>
               <group string="Instance Roles">
-                <field name="technician_ids" widget="many2many_tags"/>
-                <field name="functional_ids" widget="many2many_tags"/>
+                <field name="technician_ids" widget="many2many_tags_avatar"/>
+                <field name="functional_ids" widget="many2many_tags_avatar"/>
               </group>
             </group>
             <div>
               <!-- <h4>
                                 <field name="next_window" />
                             </h4> -->
             </div>
@@ -94,16 +94,16 @@
                   </field>
                 </group>
               </page>
               <page string="Technic">
                 <group>
                   <field name="inventory_url" widget="url"/>
                   <field name="branch"/>
-                  <field name="odoo_release_id"/>
-                  <button name="update_odoo_release" type="object" string="Import YAML" class="btn-secondary oe_edit_only"/>
+                  <field name="odoo_release_id" options="{'no_create': True}" domain="[('odoo_version_id', '=', odoo_version_id)]"/>
+                  <button name="update_odoo_release" type="object" string="Get from YAML" class="btn-secondary oe_edit_only" icon="fa-cloud-download"/>
                 </group>
                 <group>
                   <field name="server_information"/>
                   <field name="server_type"/>
                 </group>
                 <group string="Planned Deploys">
                   <field name="deploy_duration" widget="float_time"/>
@@ -112,29 +112,30 @@
                       <field name="name"/>
                       <field name="start"/>
                       <field name="description"/>
                     </tree>
                   </field>
                 </group>
                 <group string="Available Windows">
-                  <button name="compute_available_windows" string="Calculate Available Windows" type="object" class="oe_highlight"/>
+                  <button name="compute_available_windows" string="Calculate Available Windows" type="object" class="btn btn-secondary" icon="fa-calendar"/>
+                  <button string="Clear computed windows" name="action_clear_windows" type="object" class="btn btn-seconday" icon="fa-trash-o"/>
                 </group>
                 <field name="available_windows" nolabel="1">
                   <tree editable="top" create="false" delete="false">
                     <field name="start_time" widget="datetime"/>
                     <field name="end_time" widget="datetime" string="Last deploy"/>
                     <button name="open_calendar_event_wizard" string="Plan Deploy" type="object"/>
                   </tree>
                 </field>
                 <group string="Requirements">
-                  <field name="requirements_url" widget="url"/>
+                  <field name="requirements_url" widget="url" nolabel="1"/>
                   <group>
-                    <button name="download_and_process_requirements_txt" string="Update Modules from URL" type="object" class="btn-primary"/>
+                    <button name="download_and_process_requirements_txt" string="Update Modules from URL" type="object" class="btn btn-secondary" icon="fa-refresh"/>
                   </group>
-                  <field name="module_ids" nolabel="1">
+                  <field name="module_ids" nolabel="1" context="{'module_instance_ids': active_id}">
                     <tree editable="false" create="false" delete="false">
                       <field name="name"/>
                       <field name="technical_name"/>
                       <field name="is_odoo_module"/>
                       <field name="module_type"/>
                       <field name="version_ids" widget="many2many_tags"/>
                     </tree>
```

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/views/odoo_instance_window_wizard_view.xml` & `odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/views/odoo_instance_window_wizard_view.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/views/odoo_module_view.xml` & `odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/views/odoo_module_view.xml`

 * *Files 4% similar despite different names*

#### Comparing `odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/views/odoo_module_view.xml` & `odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/views/odoo_module_view.xml`

```diff
@@ -55,13 +55,22 @@
                   <field name="name"/>
                   <field name="odoo_version_id"/>
                   <field name="instance_type"/>
                   <field name="partner_id"/>
                 </tree>
               </field>
             </page>
+            <page string="Process">
+              <field name="process_ids" widget="table">
+                <tree>
+                  <field name="name"/>
+                  <field name="description"/>
+                  <field name="handbook_url" widget="url"/>
+                </tree>
+              </field>
+            </page>
           </notebook>
         </sheet>
       </form>
     </field>
   </record>
 </odoo>
```

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/views/odoo_process_view.xml` & `odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/views/odoo_process_view.xml`

 * *Format-specific differences are supported for XML files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: XML 1.0 document, ASCII text*

 * *Files 6% similar despite different names*

```diff
@@ -23,83 +23,84 @@
 00000160: 7322 3e0a 2020 2020 2020 2020 2020 2020  s">.            
 00000170: 2020 2020 3c66 6965 6c64 206e 616d 653d      <field name=
 00000180: 226e 616d 6522 202f 3e0a 2020 2020 2020  "name" />.      
 00000190: 2020 2020 2020 2020 2020 3c66 6965 6c64            <field
 000001a0: 206e 616d 653d 226f 646f 6f5f 7665 7273   name="odoo_vers
 000001b0: 696f 6e5f 6964 2220 6f70 7469 6f6e 733d  ion_id" options=
 000001c0: 227b 276e 6f5f 6372 6561 7465 273a 2054  "{'no_create': T
-000001d0: 7275 657d 222f 3e0a 2020 2020 2020 2020  rue}"/>.        
-000001e0: 2020 2020 2020 2020 3c66 6965 6c64 206e          <field n
-000001f0: 616d 653d 226d 6f64 756c 655f 6964 7322  ame="module_ids"
-00000200: 2077 6964 6765 743d 226d 616e 7932 6d61   widget="many2ma
-00000210: 6e79 5f74 6167 7322 202f 3e0a 2020 2020  ny_tags" />.    
-00000220: 2020 2020 2020 2020 2020 2020 3c66 6965              <fie
-00000230: 6c64 206e 616d 653d 2269 6e73 7461 6e63  ld name="instanc
-00000240: 655f 6964 7322 2077 6964 6765 743d 226d  e_ids" widget="m
-00000250: 616e 7932 6d61 6e79 5f74 6167 7322 202f  any2many_tags" /
-00000260: 3e20 2020 2020 2020 2020 2020 2020 2020  >               
-00000270: 200a 2020 2020 2020 2020 2020 2020 3c2f   .            </
-00000280: 7472 6565 3e0a 2020 2020 2020 2020 3c2f  tree>.        </
-00000290: 6669 656c 643e 0a20 2020 203c 2f72 6563  field>.    </rec
-000002a0: 6f72 643e 0a0a 2020 2020 3c21 2d2d 2046  ord>..    <!-- F
-000002b0: 6f72 6d20 7669 6577 2066 6f72 206f 646f  orm view for odo
-000002c0: 6f2e 696e 7374 616e 6365 2e70 726f 6365  o.instance.proce
-000002d0: 7373 202d 2d3e 0a20 2020 203c 7265 636f  ss -->.    <reco
-000002e0: 7264 2069 643d 226f 646f 6f5f 696e 7374  rd id="odoo_inst
-000002f0: 616e 6365 5f70 726f 6365 7373 5f66 6f72  ance_process_for
-00000300: 6d22 206d 6f64 656c 3d22 6972 2e75 692e  m" model="ir.ui.
-00000310: 7669 6577 223e 0a20 2020 2020 2020 203c  view">.        <
-00000320: 6669 656c 6420 6e61 6d65 3d22 6e61 6d65  field name="name
-00000330: 223e 6f64 6f6f 2e69 6e73 7461 6e63 652e  ">odoo.instance.
-00000340: 7072 6f63 6573 732e 666f 726d 3c2f 6669  process.form</fi
-00000350: 656c 643e 0a20 2020 2020 2020 203c 6669  eld>.        <fi
-00000360: 656c 6420 6e61 6d65 3d22 6d6f 6465 6c22  eld name="model"
-00000370: 3e6f 646f 6f2e 696e 7374 616e 6365 2e70  >odoo.instance.p
-00000380: 726f 6365 7373 3c2f 6669 656c 643e 0a20  rocess</field>. 
-00000390: 2020 2020 2020 203c 6669 656c 6420 6e61         <field na
-000003a0: 6d65 3d22 6172 6368 2220 7479 7065 3d22  me="arch" type="
-000003b0: 786d 6c22 3e0a 2020 2020 2020 2020 2020  xml">.          
-000003c0: 2020 3c66 6f72 6d20 7374 7269 6e67 3d22    <form string="
-000003d0: 5072 6f63 6573 7322 3e0a 2020 2020 2020  Process">.      
-000003e0: 2020 2020 2020 2020 2020 3c73 6865 6574            <sheet
-000003f0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00000400: 2020 2020 2020 3c67 726f 7570 3e0a 2020        <group>.  
-00000410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000420: 2020 2020 2020 3c66 6965 6c64 206e 616d        <field nam
-00000430: 653d 226e 616d 6522 202f 3e0a 2020 2020  e="name" />.    
-00000440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000450: 2020 2020 3c66 6965 6c64 206e 616d 653d      <field name=
-00000460: 226f 646f 6f5f 7665 7273 696f 6e5f 6964  "odoo_version_id
-00000470: 2220 2f3e 0a20 2020 2020 2020 2020 2020  " />.           
-00000480: 2020 2020 2020 2020 2020 2020 203c 6669               <fi
-00000490: 656c 6420 6e61 6d65 3d22 6d6f 6475 6c65  eld name="module
-000004a0: 5f69 6473 2220 7769 6467 6574 3d22 6d61  _ids" widget="ma
-000004b0: 6e79 326d 616e 795f 7461 6773 220a 2020  ny2many_tags".  
-000004c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000004d0: 2020 2020 2020 2020 2020 6f70 7469 6f6e            option
-000004e0: 733d 227b 276e 6f5f 6372 6561 7465 273a  s="{'no_create':
-000004f0: 2054 7275 657d 2220 646f 6d61 696e 3d22   True}" domain="
-00000500: 5b28 276f 646f 6f5f 7665 7273 696f 6e5f  [('odoo_version_
-00000510: 6964 272c 2027 3d27 2c20 6f64 6f6f 5f76  id', '=', odoo_v
-00000520: 6572 7369 6f6e 5f69 6429 5d22 2f3e 0a20  ersion_id)]"/>. 
-00000530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000540: 2020 2020 2020 203c 6669 656c 6420 6e61         <field na
-00000550: 6d65 3d22 6465 7363 7269 7074 696f 6e22  me="description"
-00000560: 2077 6964 6765 743d 2274 6578 7422 202f   widget="text" /
-00000570: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00000580: 2020 2020 2020 2020 2020 3c66 6965 6c64            <field
-00000590: 206e 616d 653d 2268 616e 6462 6f6f 6b5f   name="handbook_
-000005a0: 7572 6c22 2077 6964 6765 743d 2275 726c  url" widget="url
-000005b0: 2220 2f3e 0a20 2020 2020 2020 2020 2020  " />.           
-000005c0: 2020 2020 2020 2020 2020 2020 203c 6669               <fi
-000005d0: 656c 6420 6e61 6d65 3d22 696e 7374 616e  eld name="instan
-000005e0: 6365 5f69 6473 2220 7769 6467 6574 3d22  ce_ids" widget="
-000005f0: 6d61 6e79 326d 616e 795f 7461 6773 2220  many2many_tags" 
-00000600: 636c 6173 733d 226f 655f 7265 6164 5f6f  class="oe_read_o
-00000610: 6e6c 7922 202f 3e0a 0a20 2020 2020 2020  nly" />..       
-00000620: 2020 2020 2020 2020 2020 2020 203c 2f67               </g
-00000630: 726f 7570 3e0a 2020 2020 2020 2020 2020  roup>.          
-00000640: 2020 2020 2020 3c2f 7368 6565 743e 0a20        </sheet>. 
-00000650: 2020 2020 2020 2020 2020 203c 2f66 6f72             </for
-00000660: 6d3e 0a20 2020 2020 2020 203c 2f66 6965  m>.        </fie
-00000670: 6c64 3e0a 2020 2020 3c2f 7265 636f 7264  ld>.    </record
-00000680: 3e0a 3c2f 6f64 6f6f 3e0a                 >.</odoo>.
+000001d0: 7275 657d 2220 2f3e 0a20 2020 2020 2020  rue}" />.       
+000001e0: 2020 2020 2020 2020 203c 6669 656c 6420           <field 
+000001f0: 6e61 6d65 3d22 6d6f 6475 6c65 5f69 6473  name="module_ids
+00000200: 2220 7769 6467 6574 3d22 6d61 6e79 326d  " widget="many2m
+00000210: 616e 795f 7461 6773 2220 2f3e 0a20 2020  any_tags" />.   
+00000220: 2020 2020 2020 2020 2020 2020 203c 6669               <fi
+00000230: 656c 6420 6e61 6d65 3d22 696e 7374 616e  eld name="instan
+00000240: 6365 5f69 6473 2220 7769 6467 6574 3d22  ce_ids" widget="
+00000250: 6d61 6e79 326d 616e 795f 7461 6773 2220  many2many_tags" 
+00000260: 2f3e 0a20 2020 2020 2020 2020 2020 203c  />.            <
+00000270: 2f74 7265 653e 0a20 2020 2020 2020 203c  /tree>.        <
+00000280: 2f66 6965 6c64 3e0a 2020 2020 3c2f 7265  /field>.    </re
+00000290: 636f 7264 3e0a 0a20 2020 203c 212d 2d20  cord>..    <!-- 
+000002a0: 466f 726d 2076 6965 7720 666f 7220 6f64  Form view for od
+000002b0: 6f6f 2e69 6e73 7461 6e63 652e 7072 6f63  oo.instance.proc
+000002c0: 6573 7320 2d2d 3e0a 2020 2020 3c72 6563  ess -->.    <rec
+000002d0: 6f72 6420 6964 3d22 6f64 6f6f 5f69 6e73  ord id="odoo_ins
+000002e0: 7461 6e63 655f 7072 6f63 6573 735f 666f  tance_process_fo
+000002f0: 726d 2220 6d6f 6465 6c3d 2269 722e 7569  rm" model="ir.ui
+00000300: 2e76 6965 7722 3e0a 2020 2020 2020 2020  .view">.        
+00000310: 3c66 6965 6c64 206e 616d 653d 226e 616d  <field name="nam
+00000320: 6522 3e6f 646f 6f2e 696e 7374 616e 6365  e">odoo.instance
+00000330: 2e70 726f 6365 7373 2e66 6f72 6d3c 2f66  .process.form</f
+00000340: 6965 6c64 3e0a 2020 2020 2020 2020 3c66  ield>.        <f
+00000350: 6965 6c64 206e 616d 653d 226d 6f64 656c  ield name="model
+00000360: 223e 6f64 6f6f 2e69 6e73 7461 6e63 652e  ">odoo.instance.
+00000370: 7072 6f63 6573 733c 2f66 6965 6c64 3e0a  process</field>.
+00000380: 2020 2020 2020 2020 3c66 6965 6c64 206e          <field n
+00000390: 616d 653d 2261 7263 6822 2074 7970 653d  ame="arch" type=
+000003a0: 2278 6d6c 223e 0a20 2020 2020 2020 2020  "xml">.         
+000003b0: 2020 203c 666f 726d 2073 7472 696e 673d     <form string=
+000003c0: 2250 726f 6365 7373 223e 0a20 2020 2020  "Process">.     
+000003d0: 2020 2020 2020 2020 2020 203c 7368 6565             <shee
+000003e0: 743e 0a20 2020 2020 2020 2020 2020 2020  t>.             
+000003f0: 2020 2020 2020 203c 6772 6f75 703e 0a20         <group>. 
+00000400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000410: 2020 2020 2020 203c 6669 656c 6420 6e61         <field na
+00000420: 6d65 3d22 6e61 6d65 2220 2f3e 0a20 2020  me="name" />.   
+00000430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000440: 2020 2020 203c 6669 656c 6420 6e61 6d65       <field name
+00000450: 3d22 6f64 6f6f 5f76 6572 7369 6f6e 5f69  ="odoo_version_i
+00000460: 6422 202f 3e0a 2020 2020 2020 2020 2020  d" />.          
+00000470: 2020 2020 2020 2020 2020 2020 2020 3c66                <f
+00000480: 6965 6c64 206e 616d 653d 226d 6f64 756c  ield name="modul
+00000490: 655f 6964 7322 2077 6964 6765 743d 226d  e_ids" widget="m
+000004a0: 616e 7932 6d61 6e79 5f74 6167 7322 0a20  any2many_tags". 
+000004b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000004c0: 2020 2020 2020 2020 2020 206f 7074 696f             optio
+000004d0: 6e73 3d22 7b27 6e6f 5f63 7265 6174 6527  ns="{'no_create'
+000004e0: 3a20 5472 7565 7d22 0a20 2020 2020 2020  : True}".       
+000004f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000500: 2020 2020 2064 6f6d 6169 6e3d 225b 2827       domain="[('
+00000510: 6f64 6f6f 5f76 6572 7369 6f6e 5f69 6427  odoo_version_id'
+00000520: 2c20 273d 272c 206f 646f 6f5f 7665 7273  , '=', odoo_vers
+00000530: 696f 6e5f 6964 295d 2220 2f3e 0a20 2020  ion_id)]" />.   
+00000540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000550: 2020 2020 203c 6669 656c 6420 6e61 6d65       <field name
+00000560: 3d22 6465 7363 7269 7074 696f 6e22 2077  ="description" w
+00000570: 6964 6765 743d 2274 6578 7422 202f 3e0a  idget="text" />.
+00000580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000590: 2020 2020 2020 2020 3c66 6965 6c64 206e          <field n
+000005a0: 616d 653d 2268 616e 6462 6f6f 6b5f 7572  ame="handbook_ur
+000005b0: 6c22 2077 6964 6765 743d 2275 726c 2220  l" widget="url" 
+000005c0: 2f3e 0a20 2020 2020 2020 2020 2020 2020  />.             
+000005d0: 2020 2020 2020 2020 2020 203c 6669 656c             <fiel
+000005e0: 6420 6e61 6d65 3d22 696e 7374 616e 6365  d name="instance
+000005f0: 5f69 6473 2220 7769 6467 6574 3d22 6d61  _ids" widget="ma
+00000600: 6e79 326d 616e 795f 7461 6773 2220 636c  ny2many_tags" cl
+00000610: 6173 733d 226f 655f 7265 6164 5f6f 6e6c  ass="oe_read_onl
+00000620: 7922 202f 3e0a 0a20 2020 2020 2020 2020  y" />..         
+00000630: 2020 2020 2020 2020 2020 203c 2f67 726f             </gro
+00000640: 7570 3e0a 2020 2020 2020 2020 2020 2020  up>.            
+00000650: 2020 2020 3c2f 7368 6565 743e 0a20 2020      </sheet>.   
+00000660: 2020 2020 2020 2020 203c 2f66 6f72 6d3e           </form>
+00000670: 0a20 2020 2020 2020 203c 2f66 6965 6c64  .        </field
+00000680: 3e0a 2020 2020 3c2f 7265 636f 7264 3e0a  >.    </record>.
+00000690: 3c2f 6f64 6f6f 3e0a                      </odoo>.
```

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/views/odoo_release_view.xml` & `odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/views/odoo_release_view.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/views/odoo_version_view.xml` & `odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/views/odoo_version_view.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/views/project_project_view.xml` & `odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/views/project_project_view.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/views/res_partner_view.xml` & `odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/views/res_partner_view.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/wizards/odoo_instance_window_wizard.py` & `odoo14-addon-odoo_instance-14.0.1.1.1/odoo/addons/odoo_instance/wizards/odoo_instance_window_wizard.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,15 @@
-from odoo import models, fields, api
-from datetime import timedelta
 import logging
+from datetime import timedelta
+
+from odoo import models, fields
+
 _logger = logging.getLogger(__name__)
 
+
 class OdooInstanceWindowWizard(models.TransientModel):
     _name = 'odoo.instance.window.wizard'
     _description = 'Wizard for creating deployment events'
 
     start_time = fields.Datetime('Start Time', required=True)
     end_time = fields.Datetime('End Time', required=True)
     description = fields.Text('Description')
@@ -15,15 +18,15 @@
     duration = fields.Float('Duration', required=True)
     available_windows = fields.Text('Available Windows', readonly=True)
 
     def create_calendar_event(self):
         self.ensure_one()
         CalendarEvent = self.env['calendar.event']
         event_name = f"[{self._context.get('instance_name', 'Instance')}] Deploy"
-        
+
         # Agregar técnicos como participantes del evento
         attendee_ids = [(0, 0, {'partner_id': user.partner_id.id}) for user in self.attendee_ids]
         end_hour = self.start_time + timedelta(hours=self.duration)
         deploy_tag = self.env['calendar.event.type'].search([('name', '=', 'Deploy')], limit=1)
         _logger.debug(f"Creating event with name: {event_name}")
         _logger.debug(f"Attendees: {attendee_ids}")
         _logger.debug(f"Instance: {self.instance_id}")
@@ -46,8 +49,7 @@
             'type': 'ir.actions.act_window',
             'res_model': 'calendar.event',
             'res_id': event.id,
             'view_mode': 'form',
             'target': 'current',
             'flags': {'form': {'action_buttons': True, 'options': {'mode': 'edit'}}},
         }
-
```

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.0/odoo14_addon_odoo_instance.egg-info/PKG-INFO` & `odoo14-addon-odoo_instance-14.0.1.1.1/odoo14_addon_odoo_instance.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo14-addon-odoo-instance
-Version: 14.0.1.1.0
+Version: 14.0.1.1.1
 Summary: Manage Odoo instances with relevant information
 Home-page: https://www.coopdevs.org
 Author: Coopdevs
 License: AGPL-3
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 14.0
@@ -50,14 +50,23 @@
 
 .. contents::
    :local:
 
 Changelog
 =========
 
+14.0.1.1.1 (2023-04-25)
+~~~~~~~~~~~~~~~~~~~~~~~
+
+**Bugfixes**
+
+- Upcrate module versions
+- Show installed module versions only in instance view
+
+
 14.0.1.1.0 (2023-04-25)
 ~~~~~~~~~~~~~~~~~~~~~~~
 
 **Features**
 
 - Handle odoo releases
```

### Comparing `odoo14-addon-odoo_instance-14.0.1.1.0/odoo14_addon_odoo_instance.egg-info/SOURCES.txt` & `odoo14-addon-odoo_instance-14.0.1.1.1/odoo14_addon_odoo_instance.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 odoo/addons/odoo_instance/static/src/img/icon.png
 odoo/addons/odoo_instance/static/src/js/project_instance.js
 odoo/addons/odoo_instance/tests/__init__.py
 odoo/addons/odoo_instance/tests/test_project_instance.py
 odoo/addons/odoo_instance/views/import_requirements_wizard_view.xml
 odoo/addons/odoo_instance/views/odoo_instance_actions.xml
 odoo/addons/odoo_instance/views/odoo_instance_menuitems.xml
+odoo/addons/odoo_instance/views/odoo_instance_module_version_views.xml
 odoo/addons/odoo_instance/views/odoo_instance_searches.xml
 odoo/addons/odoo_instance/views/odoo_instance_view.xml
 odoo/addons/odoo_instance/views/odoo_instance_window_wizard_view.xml
 odoo/addons/odoo_instance/views/odoo_module_view.xml
 odoo/addons/odoo_instance/views/odoo_process_view.xml
 odoo/addons/odoo_instance/views/odoo_release_view.xml
 odoo/addons/odoo_instance/views/odoo_version_view.xml
```

