# Comparing `tmp/dead_simple_framework-1.3.8.tar.gz` & `tmp/dead_simple_framework-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dead_simple_framework-1.3.8.tar", last modified: Tue Apr 25 22:27:13 2023, max compression
+gzip compressed data, was "dead_simple_framework-1.3.9.tar", last modified: Wed Apr 26 05:35:08 2023, max compression
```

## Comparing `dead_simple_framework-1.3.8.tar` & `dead_simple_framework-1.3.9.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 pswanson   (502) staff       (20)        0 2023-04-25 22:27:13.514059 dead_simple_framework-1.3.8/
--rw-r--r--   0 pswanson   (502) staff       (20)     5206 2023-04-25 22:27:13.513606 dead_simple_framework-1.3.8/PKG-INFO
--rw-r--r--   0 pswanson   (502) staff       (20)     4847 2023-04-25 22:27:12.000000 dead_simple_framework-1.3.8/README.md
-drwxr-xr-x   0 pswanson   (502) staff       (20)        0 2023-04-25 22:27:13.451849 dead_simple_framework-1.3.8/dead_simple_framework/
--rw-r--r--   0 pswanson   (502) staff       (20)      433 2023-04-25 22:27:12.000000 dead_simple_framework-1.3.8/dead_simple_framework/__init__.py
-drwxr-xr-x   0 pswanson   (502) staff       (20)        0 2023-04-25 22:27:13.462540 dead_simple_framework-1.3.8/dead_simple_framework/api/
--rw-r--r--   0 pswanson   (502) staff       (20)      139 2023-04-25 22:27:12.000000 dead_simple_framework-1.3.8/dead_simple_framework/api/__init__.py
--rw-r--r--   0 pswanson   (502) staff       (20)     4144 2023-04-25 22:27:12.000000 dead_simple_framework-1.3.8/dead_simple_framework/api/client.py
--rw-r--r--   0 pswanson   (502) staff       (20)     1146 2023-04-25 22:27:12.000000 dead_simple_framework-1.3.8/dead_simple_framework/api/errors.py
--rw-r--r--   0 pswanson   (502) staff       (20)    15354 2023-04-25 22:27:12.000000 dead_simple_framework-1.3.8/dead_simple_framework/api/main.py
--rw-r--r--   0 pswanson   (502) staff       (20)    10066 2023-04-25 22:27:12.000000 dead_simple_framework-1.3.8/dead_simple_framework/api/utils.py
-drwxr-xr-x   0 pswanson   (502) staff       (20)        0 2023-04-25 22:27:13.465889 dead_simple_framework-1.3.8/dead_simple_framework/cache/
--rw-r--r--   0 pswanson   (502) staff       (20)       23 2023-04-25 22:27:12.000000 dead_simple_framework-1.3.8/dead_simple_framework/cache/__init__.py
--rw-r--r--   0 pswanson   (502) staff       (20)     3670 2023-04-25 22:27:12.000000 dead_simple_framework-1.3.8/dead_simple_framework/cache/main.py
-drwxr-xr-x   0 pswanson   (502) staff       (20)        0 2023-04-25 22:27:13.471326 dead_simple_framework-1.3.8/dead_simple_framework/config/
--rw-r--r--   0 pswanson   (502) staff       (20)      422 2023-04-25 22:27:12.000000 dead_simple_framework-1.3.8/dead_simple_framework/config/__init__.py
--rw-r--r--   0 pswanson   (502) staff       (20)     1949 2023-04-25 22:27:12.000000 dead_simple_framework-1.3.8/dead_simple_framework/config/config.py
--rw-r--r--   0 pswanson   (502) staff       (20)     1743 2023-04-25 22:27:12.000000 dead_simple_framework-1.3.8/dead_simple_framework/config/route.py
--rw-r--r--   0 pswanson   (502) staff       (20)     3611 2023-04-25 22:27:12.000000 dead_simple_framework-1.3.8/dead_simple_framework/config/schema.py
-drwxr-xr-x   0 pswanson   (502) staff       (20)        0 2023-04-25 22:27:13.484132 dead_simple_framework-1.3.8/dead_simple_framework/config/settings/
--rw-r--r--   0 pswanson   (502) staff       (20)      305 2023-04-25 22:27:12.000000 dead_simple_framework-1.3.8/dead_simple_framework/config/settings/__init__.py
--rw-r--r--   0 pswanson   (502) staff       (20)     2422 2023-04-25 22:27:12.000000 dead_simple_framework-1.3.8/dead_simple_framework/config/settings/app_settings.py
--rw-r--r--   0 pswanson   (502) staff       (20)     1831 2023-04-25 22:27:12.000000 dead_simple_framework-1.3.8/dead_simple_framework/config/settings/jwt_settings.py
--rw-r--r--   0 pswanson   (502) staff       (20)     2385 2023-04-25 22:27:12.000000 dead_simple_framework-1.3.8/dead_simple_framework/config/settings/main.py
--rw-r--r--   0 pswanson   (502) staff       (20)     6280 2023-04-25 22:27:12.000000 dead_simple_framework-1.3.8/dead_simple_framework/config/settings/mongodb_settings.py
--rw-r--r--   0 pswanson   (502) staff       (20)     4085 2023-04-25 22:27:12.000000 dead_simple_framework-1.3.8/dead_simple_framework/config/settings/rabbitmq_settings.py
--rw-r--r--   0 pswanson   (502) staff       (20)     3048 2023-04-25 22:27:12.000000 dead_simple_framework-1.3.8/dead_simple_framework/config/settings/redis_settings.py
--rw-r--r--   0 pswanson   (502) staff       (20)     1587 2023-04-25 22:27:12.000000 dead_simple_framework-1.3.8/dead_simple_framework/config/settings/sentry_settings.py
--rw-r--r--   0 pswanson   (502) staff       (20)      558 2023-04-25 22:27:12.000000 dead_simple_framework-1.3.8/dead_simple_framework/config/settings/setting.py
--rw-r--r--   0 pswanson   (502) staff       (20)     1400 2023-04-25 22:27:12.000000 dead_simple_framework-1.3.8/dead_simple_framework/config/settings/slack_settings.py
--rw-r--r--   0 pswanson   (502) staff       (20)     1947 2023-04-25 22:27:12.000000 dead_simple_framework-1.3.8/dead_simple_framework/config/task.py
-drwxr-xr-x   0 pswanson   (502) staff       (20)        0 2023-04-25 22:27:13.490168 dead_simple_framework-1.3.8/dead_simple_framework/database/
--rw-r--r--   0 pswanson   (502) staff       (20)       91 2023-04-25 22:27:12.000000 dead_simple_framework-1.3.8/dead_simple_framework/database/__init__.py
--rw-r--r--   0 pswanson   (502) staff       (20)     1756 2023-04-25 22:27:12.000000 dead_simple_framework-1.3.8/dead_simple_framework/database/fixtures.py
--rw-r--r--   0 pswanson   (502) staff       (20)     3708 2023-04-25 22:27:12.000000 dead_simple_framework-1.3.8/dead_simple_framework/database/index.py
--rw-r--r--   0 pswanson   (502) staff       (20)     4295 2023-04-25 22:27:12.000000 dead_simple_framework-1.3.8/dead_simple_framework/database/main.py
--rw-r--r--   0 pswanson   (502) staff       (20)      568 2023-04-25 22:27:12.000000 dead_simple_framework-1.3.8/dead_simple_framework/database/utils.py
--rw-r--r--   0 pswanson   (502) staff       (20)      576 2023-04-25 22:27:12.000000 dead_simple_framework-1.3.8/dead_simple_framework/encoder.py
-drwxr-xr-x   0 pswanson   (502) staff       (20)        0 2023-04-25 22:27:13.502830 dead_simple_framework-1.3.8/dead_simple_framework/handlers/
--rw-r--r--   0 pswanson   (502) staff       (20)      288 2023-04-25 22:27:12.000000 dead_simple_framework-1.3.8/dead_simple_framework/handlers/__init__.py
--rw-r--r--   0 pswanson   (502) staff       (20)     1969 2023-04-25 22:27:12.000000 dead_simple_framework-1.3.8/dead_simple_framework/handlers/default.py
--rw-r--r--   0 pswanson   (502) staff       (20)     4775 2023-04-25 22:27:12.000000 dead_simple_framework-1.3.8/dead_simple_framework/handlers/login.py
--rw-r--r--   0 pswanson   (502) staff       (20)     3514 2023-04-25 22:27:12.000000 dead_simple_framework-1.3.8/dead_simple_framework/handlers/permissions.py
--rw-r--r--   0 pswanson   (502) staff       (20)     4483 2023-04-25 22:27:12.000000 dead_simple_framework-1.3.8/dead_simple_framework/handlers/users.py
--rw-r--r--   0 pswanson   (502) staff       (20)       61 2023-04-25 22:27:12.000000 dead_simple_framework-1.3.8/dead_simple_framework/jwt.py
--rw-r--r--   0 pswanson   (502) staff       (20)     4068 2023-04-25 22:27:12.000000 dead_simple_framework-1.3.8/dead_simple_framework/main.py
--rw-r--r--   0 pswanson   (502) staff       (20)     2685 2023-04-25 22:27:12.000000 dead_simple_framework-1.3.8/dead_simple_framework/router.py
--rw-r--r--   0 pswanson   (502) staff       (20)     4511 2023-04-25 22:27:12.000000 dead_simple_framework-1.3.8/dead_simple_framework/slack.py
-drwxr-xr-x   0 pswanson   (502) staff       (20)        0 2023-04-25 22:27:13.512555 dead_simple_framework-1.3.8/dead_simple_framework/tasks/
--rw-r--r--   0 pswanson   (502) staff       (20)       30 2023-04-25 22:27:12.000000 dead_simple_framework-1.3.8/dead_simple_framework/tasks/__init__.py
--rw-r--r--   0 pswanson   (502) staff       (20)    12468 2023-04-25 22:27:12.000000 dead_simple_framework-1.3.8/dead_simple_framework/tasks/main.py
--rw-r--r--   0 pswanson   (502) staff       (20)     3454 2023-04-25 22:27:12.000000 dead_simple_framework-1.3.8/dead_simple_framework/tasks/task.py
--rw-r--r--   0 pswanson   (502) staff       (20)     1306 2023-04-25 22:27:12.000000 dead_simple_framework-1.3.8/dead_simple_framework/tasks/utils.py
-drwxr-xr-x   0 pswanson   (502) staff       (20)        0 2023-04-25 22:27:13.457494 dead_simple_framework-1.3.8/dead_simple_framework.egg-info/
--rw-r--r--   0 pswanson   (502) staff       (20)     5206 2023-04-25 22:27:13.000000 dead_simple_framework-1.3.8/dead_simple_framework.egg-info/PKG-INFO
--rw-r--r--   0 pswanson   (502) staff       (20)     1984 2023-04-25 22:27:13.000000 dead_simple_framework-1.3.8/dead_simple_framework.egg-info/SOURCES.txt
--rw-r--r--   0 pswanson   (502) staff       (20)        1 2023-04-25 22:27:13.000000 dead_simple_framework-1.3.8/dead_simple_framework.egg-info/dependency_links.txt
--rw-r--r--   0 pswanson   (502) staff       (20)      146 2023-04-25 22:27:13.000000 dead_simple_framework-1.3.8/dead_simple_framework.egg-info/requires.txt
--rw-r--r--   0 pswanson   (502) staff       (20)       22 2023-04-25 22:27:13.000000 dead_simple_framework-1.3.8/dead_simple_framework.egg-info/top_level.txt
--rw-r--r--   0 pswanson   (502) staff       (20)       38 2023-04-25 22:27:13.514250 dead_simple_framework-1.3.8/setup.cfg
--rw-r--r--   0 pswanson   (502) staff       (20)      824 2023-04-25 22:27:01.000000 dead_simple_framework-1.3.8/setup.py
+drwxr-xr-x   0 pswanson   (502) staff       (20)        0 2023-04-26 05:35:08.215519 dead_simple_framework-1.3.9/
+-rw-r--r--   0 pswanson   (502) staff       (20)     5206 2023-04-26 05:35:08.214659 dead_simple_framework-1.3.9/PKG-INFO
+-rw-r--r--   0 pswanson   (502) staff       (20)     4847 2023-04-26 05:35:07.000000 dead_simple_framework-1.3.9/README.md
+drwxr-xr-x   0 pswanson   (502) staff       (20)        0 2023-04-26 05:35:08.159816 dead_simple_framework-1.3.9/dead_simple_framework/
+-rw-r--r--   0 pswanson   (502) staff       (20)      433 2023-04-26 05:35:07.000000 dead_simple_framework-1.3.9/dead_simple_framework/__init__.py
+drwxr-xr-x   0 pswanson   (502) staff       (20)        0 2023-04-26 05:35:08.174004 dead_simple_framework-1.3.9/dead_simple_framework/api/
+-rw-r--r--   0 pswanson   (502) staff       (20)      139 2023-04-26 05:35:07.000000 dead_simple_framework-1.3.9/dead_simple_framework/api/__init__.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     4144 2023-04-26 05:35:07.000000 dead_simple_framework-1.3.9/dead_simple_framework/api/client.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     1146 2023-04-26 05:35:07.000000 dead_simple_framework-1.3.9/dead_simple_framework/api/errors.py
+-rw-r--r--   0 pswanson   (502) staff       (20)    15481 2023-04-26 05:35:07.000000 dead_simple_framework-1.3.9/dead_simple_framework/api/main.py
+-rw-r--r--   0 pswanson   (502) staff       (20)    10066 2023-04-26 05:35:07.000000 dead_simple_framework-1.3.9/dead_simple_framework/api/utils.py
+drwxr-xr-x   0 pswanson   (502) staff       (20)        0 2023-04-26 05:35:08.175816 dead_simple_framework-1.3.9/dead_simple_framework/cache/
+-rw-r--r--   0 pswanson   (502) staff       (20)       23 2023-04-26 05:35:07.000000 dead_simple_framework-1.3.9/dead_simple_framework/cache/__init__.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     3670 2023-04-26 05:35:07.000000 dead_simple_framework-1.3.9/dead_simple_framework/cache/main.py
+drwxr-xr-x   0 pswanson   (502) staff       (20)        0 2023-04-26 05:35:08.184892 dead_simple_framework-1.3.9/dead_simple_framework/config/
+-rw-r--r--   0 pswanson   (502) staff       (20)      422 2023-04-26 05:35:07.000000 dead_simple_framework-1.3.9/dead_simple_framework/config/__init__.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     1949 2023-04-26 05:35:07.000000 dead_simple_framework-1.3.9/dead_simple_framework/config/config.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     1743 2023-04-26 05:35:07.000000 dead_simple_framework-1.3.9/dead_simple_framework/config/route.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     3611 2023-04-26 05:35:07.000000 dead_simple_framework-1.3.9/dead_simple_framework/config/schema.py
+drwxr-xr-x   0 pswanson   (502) staff       (20)        0 2023-04-26 05:35:08.193842 dead_simple_framework-1.3.9/dead_simple_framework/config/settings/
+-rw-r--r--   0 pswanson   (502) staff       (20)      305 2023-04-26 05:35:07.000000 dead_simple_framework-1.3.9/dead_simple_framework/config/settings/__init__.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     2422 2023-04-26 05:35:07.000000 dead_simple_framework-1.3.9/dead_simple_framework/config/settings/app_settings.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     1831 2023-04-26 05:35:07.000000 dead_simple_framework-1.3.9/dead_simple_framework/config/settings/jwt_settings.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     2385 2023-04-26 05:35:07.000000 dead_simple_framework-1.3.9/dead_simple_framework/config/settings/main.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     6280 2023-04-26 05:35:07.000000 dead_simple_framework-1.3.9/dead_simple_framework/config/settings/mongodb_settings.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     4085 2023-04-26 05:35:07.000000 dead_simple_framework-1.3.9/dead_simple_framework/config/settings/rabbitmq_settings.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     3048 2023-04-26 05:35:07.000000 dead_simple_framework-1.3.9/dead_simple_framework/config/settings/redis_settings.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     1587 2023-04-26 05:35:07.000000 dead_simple_framework-1.3.9/dead_simple_framework/config/settings/sentry_settings.py
+-rw-r--r--   0 pswanson   (502) staff       (20)      558 2023-04-26 05:35:07.000000 dead_simple_framework-1.3.9/dead_simple_framework/config/settings/setting.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     1400 2023-04-26 05:35:07.000000 dead_simple_framework-1.3.9/dead_simple_framework/config/settings/slack_settings.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     1947 2023-04-26 05:35:07.000000 dead_simple_framework-1.3.9/dead_simple_framework/config/task.py
+drwxr-xr-x   0 pswanson   (502) staff       (20)        0 2023-04-26 05:35:08.198765 dead_simple_framework-1.3.9/dead_simple_framework/database/
+-rw-r--r--   0 pswanson   (502) staff       (20)       91 2023-04-26 05:35:07.000000 dead_simple_framework-1.3.9/dead_simple_framework/database/__init__.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     1756 2023-04-26 05:35:07.000000 dead_simple_framework-1.3.9/dead_simple_framework/database/fixtures.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     3708 2023-04-26 05:35:07.000000 dead_simple_framework-1.3.9/dead_simple_framework/database/index.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     4295 2023-04-26 05:35:07.000000 dead_simple_framework-1.3.9/dead_simple_framework/database/main.py
+-rw-r--r--   0 pswanson   (502) staff       (20)      568 2023-04-26 05:35:07.000000 dead_simple_framework-1.3.9/dead_simple_framework/database/utils.py
+-rw-r--r--   0 pswanson   (502) staff       (20)      576 2023-04-26 05:35:07.000000 dead_simple_framework-1.3.9/dead_simple_framework/encoder.py
+drwxr-xr-x   0 pswanson   (502) staff       (20)        0 2023-04-26 05:35:08.203671 dead_simple_framework-1.3.9/dead_simple_framework/handlers/
+-rw-r--r--   0 pswanson   (502) staff       (20)      288 2023-04-26 05:35:07.000000 dead_simple_framework-1.3.9/dead_simple_framework/handlers/__init__.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     1981 2023-04-26 05:35:07.000000 dead_simple_framework-1.3.9/dead_simple_framework/handlers/default.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     4775 2023-04-26 05:35:07.000000 dead_simple_framework-1.3.9/dead_simple_framework/handlers/login.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     3514 2023-04-26 05:35:07.000000 dead_simple_framework-1.3.9/dead_simple_framework/handlers/permissions.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     4483 2023-04-26 05:35:07.000000 dead_simple_framework-1.3.9/dead_simple_framework/handlers/users.py
+-rw-r--r--   0 pswanson   (502) staff       (20)       61 2023-04-26 05:35:07.000000 dead_simple_framework-1.3.9/dead_simple_framework/jwt.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     4068 2023-04-26 05:35:07.000000 dead_simple_framework-1.3.9/dead_simple_framework/main.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     2685 2023-04-26 05:35:07.000000 dead_simple_framework-1.3.9/dead_simple_framework/router.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     4511 2023-04-26 05:35:07.000000 dead_simple_framework-1.3.9/dead_simple_framework/slack.py
+drwxr-xr-x   0 pswanson   (502) staff       (20)        0 2023-04-26 05:35:08.212978 dead_simple_framework-1.3.9/dead_simple_framework/tasks/
+-rw-r--r--   0 pswanson   (502) staff       (20)       30 2023-04-26 05:35:07.000000 dead_simple_framework-1.3.9/dead_simple_framework/tasks/__init__.py
+-rw-r--r--   0 pswanson   (502) staff       (20)    12468 2023-04-26 05:35:07.000000 dead_simple_framework-1.3.9/dead_simple_framework/tasks/main.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     3454 2023-04-26 05:35:07.000000 dead_simple_framework-1.3.9/dead_simple_framework/tasks/task.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     1306 2023-04-26 05:35:07.000000 dead_simple_framework-1.3.9/dead_simple_framework/tasks/utils.py
+drwxr-xr-x   0 pswanson   (502) staff       (20)        0 2023-04-26 05:35:08.166469 dead_simple_framework-1.3.9/dead_simple_framework.egg-info/
+-rw-r--r--   0 pswanson   (502) staff       (20)     5206 2023-04-26 05:35:07.000000 dead_simple_framework-1.3.9/dead_simple_framework.egg-info/PKG-INFO
+-rw-r--r--   0 pswanson   (502) staff       (20)     1984 2023-04-26 05:35:07.000000 dead_simple_framework-1.3.9/dead_simple_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 pswanson   (502) staff       (20)        1 2023-04-26 05:35:07.000000 dead_simple_framework-1.3.9/dead_simple_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 pswanson   (502) staff       (20)      146 2023-04-26 05:35:07.000000 dead_simple_framework-1.3.9/dead_simple_framework.egg-info/requires.txt
+-rw-r--r--   0 pswanson   (502) staff       (20)       22 2023-04-26 05:35:07.000000 dead_simple_framework-1.3.9/dead_simple_framework.egg-info/top_level.txt
+-rw-r--r--   0 pswanson   (502) staff       (20)       38 2023-04-26 05:35:08.216632 dead_simple_framework-1.3.9/setup.cfg
+-rw-r--r--   0 pswanson   (502) staff       (20)      824 2023-04-26 05:35:00.000000 dead_simple_framework-1.3.9/setup.py
```

### Comparing `dead_simple_framework-1.3.8/PKG-INFO` & `dead_simple_framework-1.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dead_simple_framework
-Version: 1.3.8
+Version: 1.3.9
 Summary: RESTful Flask framework with builtin MongoDB, Redis, Celery, Sentry and Slack integrations
 Home-page: https://github.com/Topazoo/dead_simple_framework
 Author: Peter Swanson
 Author-email: pswanson@ucdavis.edu
 License: MIT
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
```

### Comparing `dead_simple_framework-1.3.8/README.md` & `dead_simple_framework-1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.8/dead_simple_framework/api/client.py` & `dead_simple_framework-1.3.9/dead_simple_framework/api/client.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.8/dead_simple_framework/api/errors.py` & `dead_simple_framework-1.3.9/dead_simple_framework/api/errors.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.8/dead_simple_framework/api/main.py` & `dead_simple_framework-1.3.9/dead_simple_framework/api/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -238,14 +238,17 @@
         except API_Error as e:
             return JsonException('DELETE', e)
 
         except Exception as e:
             if App_Settings.APP_ENV == 'development': raise e
             return JsonException('DELETE', e)
 
+    @staticmethod
+    def OPTIONS(request:Request, payload:dict, collection:Collection) -> Response:
+        return Response()
 
     @staticmethod
     def _get_handler(method:str, route:Route) -> Callable:
         ''' Get the handler for the request on a given route or raise a 405 error '''
 
         handler = getattr(route.handler, method, None)
```

### Comparing `dead_simple_framework-1.3.8/dead_simple_framework/api/utils.py` & `dead_simple_framework-1.3.9/dead_simple_framework/api/utils.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.8/dead_simple_framework/cache/main.py` & `dead_simple_framework-1.3.9/dead_simple_framework/cache/main.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.8/dead_simple_framework/config/config.py` & `dead_simple_framework-1.3.9/dead_simple_framework/config/config.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.8/dead_simple_framework/config/route.py` & `dead_simple_framework-1.3.9/dead_simple_framework/config/route.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.8/dead_simple_framework/config/schema.py` & `dead_simple_framework-1.3.9/dead_simple_framework/config/schema.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.8/dead_simple_framework/config/settings/app_settings.py` & `dead_simple_framework-1.3.9/dead_simple_framework/config/settings/app_settings.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.8/dead_simple_framework/config/settings/jwt_settings.py` & `dead_simple_framework-1.3.9/dead_simple_framework/config/settings/jwt_settings.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.8/dead_simple_framework/config/settings/main.py` & `dead_simple_framework-1.3.9/dead_simple_framework/config/settings/main.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.8/dead_simple_framework/config/settings/mongodb_settings.py` & `dead_simple_framework-1.3.9/dead_simple_framework/config/settings/mongodb_settings.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.8/dead_simple_framework/config/settings/rabbitmq_settings.py` & `dead_simple_framework-1.3.9/dead_simple_framework/config/settings/rabbitmq_settings.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.8/dead_simple_framework/config/settings/redis_settings.py` & `dead_simple_framework-1.3.9/dead_simple_framework/config/settings/redis_settings.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.8/dead_simple_framework/config/settings/sentry_settings.py` & `dead_simple_framework-1.3.9/dead_simple_framework/config/settings/sentry_settings.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.8/dead_simple_framework/config/settings/setting.py` & `dead_simple_framework-1.3.9/dead_simple_framework/config/settings/setting.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.8/dead_simple_framework/config/settings/slack_settings.py` & `dead_simple_framework-1.3.9/dead_simple_framework/config/settings/slack_settings.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.8/dead_simple_framework/config/task.py` & `dead_simple_framework-1.3.9/dead_simple_framework/config/task.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.8/dead_simple_framework/database/fixtures.py` & `dead_simple_framework-1.3.9/dead_simple_framework/database/fixtures.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.8/dead_simple_framework/database/index.py` & `dead_simple_framework-1.3.9/dead_simple_framework/database/index.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.8/dead_simple_framework/database/main.py` & `dead_simple_framework-1.3.9/dead_simple_framework/database/main.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.8/dead_simple_framework/database/utils.py` & `dead_simple_framework-1.3.9/dead_simple_framework/database/utils.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.8/dead_simple_framework/encoder.py` & `dead_simple_framework-1.3.9/dead_simple_framework/encoder.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.8/dead_simple_framework/handlers/default.py` & `dead_simple_framework-1.3.9/dead_simple_framework/handlers/default.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,11 +35,11 @@
         '''
         
         if GET: self.GET = GET
         if POST: self.POST = POST
         if DELETE: self.DELETE = DELETE
         if PUT: self.PUT = PUT
         self.PATCH = PATCH
-        self.OPTIONS = OPTIONS
+        if OPTIONS: self.OPTIONS = OPTIONS
 
         if verifier: self.verifier = verifier
         self.methods = list(filter(lambda x: getattr(self,x) != None, self.SUPPORTED_HTTP_METHODS))
```

### Comparing `dead_simple_framework-1.3.8/dead_simple_framework/handlers/login.py` & `dead_simple_framework-1.3.9/dead_simple_framework/handlers/login.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.8/dead_simple_framework/handlers/permissions.py` & `dead_simple_framework-1.3.9/dead_simple_framework/handlers/permissions.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.8/dead_simple_framework/handlers/users.py` & `dead_simple_framework-1.3.9/dead_simple_framework/handlers/users.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.8/dead_simple_framework/main.py` & `dead_simple_framework-1.3.9/dead_simple_framework/main.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.8/dead_simple_framework/router.py` & `dead_simple_framework-1.3.9/dead_simple_framework/router.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.8/dead_simple_framework/slack.py` & `dead_simple_framework-1.3.9/dead_simple_framework/slack.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.8/dead_simple_framework/tasks/main.py` & `dead_simple_framework-1.3.9/dead_simple_framework/tasks/main.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.8/dead_simple_framework/tasks/task.py` & `dead_simple_framework-1.3.9/dead_simple_framework/tasks/task.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.8/dead_simple_framework/tasks/utils.py` & `dead_simple_framework-1.3.9/dead_simple_framework/tasks/utils.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.8/dead_simple_framework.egg-info/PKG-INFO` & `dead_simple_framework-1.3.9/dead_simple_framework.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dead-simple-framework
-Version: 1.3.8
+Version: 1.3.9
 Summary: RESTful Flask framework with builtin MongoDB, Redis, Celery, Sentry and Slack integrations
 Home-page: https://github.com/Topazoo/dead_simple_framework
 Author: Peter Swanson
 Author-email: pswanson@ucdavis.edu
 License: MIT
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
```

### Comparing `dead_simple_framework-1.3.8/dead_simple_framework.egg-info/SOURCES.txt` & `dead_simple_framework-1.3.9/dead_simple_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.8/setup.py` & `dead_simple_framework-1.3.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 setuptools.setup(
     author="Peter Swanson",
     author_email="pswanson@ucdavis.edu",
     name='dead_simple_framework',
     license="MIT",
     description='RESTful Flask framework with builtin MongoDB, Redis, Celery, Sentry and Slack integrations',
-    version='v1.3.8',
+    version='v1.3.9',
     long_description=README,
     url='https://github.com/Topazoo/dead_simple_framework',
     packages=setuptools.find_packages(),
     python_requires=">=3.5",
     install_requires=['flask', 'pymongo', 'celery', 'flask-cors', 'requests', 'redis', 'eventlet', 'pyOpenSSL', 'Flask-JWT-Extended', 'passlib', 'jsonschema', 'sentry-sdk[flask]', 'slack-sdk', 'Flask-PyMongo'],
     long_description_content_type='text/markdown',
     classifiers=[]
```

