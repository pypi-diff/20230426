# Comparing `tmp/adatoolbox-0.0.7.tar.gz` & `tmp/adatoolbox-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adatoolbox-0.0.7.tar", last modified: Fri Mar 31 20:17:22 2023, max compression
+gzip compressed data, was "adatoolbox-0.0.8.tar", last modified: Tue Apr 25 15:38:50 2023, max compression
```

## Comparing `adatoolbox-0.0.7.tar` & `adatoolbox-0.0.8.tar`

### file list

```diff
@@ -1,29 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 20:17:22.834891 adatoolbox-0.0.7/
--rw-r--r--   0 root         (0) root         (0)     1073 2023-03-27 19:16:17.000000 adatoolbox-0.0.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)      504 2023-03-31 20:17:22.817228 adatoolbox-0.0.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-27 19:16:17.000000 adatoolbox-0.0.7/README.md
--rw-r--r--   0 root         (0) root         (0)      716 2023-03-31 20:12:56.000000 adatoolbox-0.0.7/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-31 20:17:22.840520 adatoolbox-0.0.7/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 20:17:21.335983 adatoolbox-0.0.7/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 20:17:21.761206 adatoolbox-0.0.7/src/adatoolbox/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-27 19:16:17.000000 adatoolbox-0.0.7/src/adatoolbox/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 20:17:22.319537 adatoolbox-0.0.7/src/adatoolbox/database/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-27 19:16:17.000000 adatoolbox-0.0.7/src/adatoolbox/database/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1007 2023-03-27 19:16:17.000000 adatoolbox-0.0.7/src/adatoolbox/database/base_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 20:17:21.433802 adatoolbox-0.0.7/src/adatoolbox/domain/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 20:17:22.547274 adatoolbox-0.0.7/src/adatoolbox/domain/auth/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-28 12:54:11.000000 adatoolbox-0.0.7/src/adatoolbox/domain/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1343 2023-03-31 18:34:42.000000 adatoolbox-0.0.7/src/adatoolbox/domain/auth/base_authentication.py
--rw-r--r--   0 root         (0) root         (0)      235 2023-03-31 20:07:41.000000 adatoolbox-0.0.7/src/adatoolbox/domain/auth/base_permission.py
--rw-r--r--   0 root         (0) root         (0)       49 2023-03-29 16:16:00.000000 adatoolbox-0.0.7/src/adatoolbox/domain/auth/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 20:17:22.700482 adatoolbox-0.0.7/src/adatoolbox/domain/secret/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-31 11:56:09.000000 adatoolbox-0.0.7/src/adatoolbox/domain/secret/__init__.py
--rw-r--r--   0 root         (0) root         (0)      730 2023-03-31 12:07:26.000000 adatoolbox-0.0.7/src/adatoolbox/domain/secret/doppler.py
--rw-r--r--   0 root         (0) root         (0)       55 2023-03-31 12:06:28.000000 adatoolbox-0.0.7/src/adatoolbox/domain/secret/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 20:17:22.773826 adatoolbox-0.0.7/src/adatoolbox/utils/
--rw-r--r--   0 root         (0) root         (0)      293 2023-03-29 14:22:01.000000 adatoolbox-0.0.7/src/adatoolbox/utils/enum.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 20:17:22.008464 adatoolbox-0.0.7/src/adatoolbox.egg-info/
--rw-r--r--   0 root         (0) root         (0)      504 2023-03-31 20:17:20.000000 adatoolbox-0.0.7/src/adatoolbox.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      610 2023-03-31 20:17:21.000000 adatoolbox-0.0.7/src/adatoolbox.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-31 20:17:21.000000 adatoolbox-0.0.7/src/adatoolbox.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-03-31 20:17:21.000000 adatoolbox-0.0.7/src/adatoolbox.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 15:38:50.666183 adatoolbox-0.0.8/
+-rw-r--r--   0 root         (0) root         (0)     1073 2023-03-27 19:16:17.000000 adatoolbox-0.0.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      504 2023-04-25 15:38:50.633689 adatoolbox-0.0.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-27 19:16:17.000000 adatoolbox-0.0.8/README.md
+-rw-r--r--   0 root         (0) root         (0)      750 2023-04-25 15:38:35.000000 adatoolbox-0.0.8/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-25 15:38:50.734754 adatoolbox-0.0.8/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 15:38:44.828911 adatoolbox-0.0.8/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 15:38:45.849779 adatoolbox-0.0.8/src/adatoolbox/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-27 19:16:17.000000 adatoolbox-0.0.8/src/adatoolbox/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 15:38:46.934891 adatoolbox-0.0.8/src/adatoolbox/database/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-27 19:16:17.000000 adatoolbox-0.0.8/src/adatoolbox/database/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1007 2023-03-27 19:16:17.000000 adatoolbox-0.0.8/src/adatoolbox/database/base_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 15:38:45.101646 adatoolbox-0.0.8/src/adatoolbox/domain/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 15:38:48.367325 adatoolbox-0.0.8/src/adatoolbox/domain/auth/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-28 12:54:11.000000 adatoolbox-0.0.8/src/adatoolbox/domain/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1343 2023-03-31 18:34:42.000000 adatoolbox-0.0.8/src/adatoolbox/domain/auth/base_authentication.py
+-rw-r--r--   0 root         (0) root         (0)      236 2023-03-31 20:21:16.000000 adatoolbox-0.0.8/src/adatoolbox/domain/auth/base_permission.py
+-rw-r--r--   0 root         (0) root         (0)       48 2023-04-11 08:17:51.000000 adatoolbox-0.0.8/src/adatoolbox/domain/auth/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 15:38:48.625417 adatoolbox-0.0.8/src/adatoolbox/domain/event/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 14:28:16.000000 adatoolbox-0.0.8/src/adatoolbox/domain/event/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 15:38:49.348686 adatoolbox-0.0.8/src/adatoolbox/domain/event/adapters/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 14:40:22.000000 adatoolbox-0.0.8/src/adatoolbox/domain/event/adapters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      547 2023-04-25 15:37:42.000000 adatoolbox-0.0.8/src/adatoolbox/domain/event/adapters/mq_publisher_adapter.py
+-rw-r--r--   0 root         (0) root         (0)     1675 2023-04-25 15:34:52.000000 adatoolbox-0.0.8/src/adatoolbox/domain/event/adapters/pika_adapter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 15:38:50.150501 adatoolbox-0.0.8/src/adatoolbox/domain/secret/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-31 11:56:09.000000 adatoolbox-0.0.8/src/adatoolbox/domain/secret/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      730 2023-03-31 12:07:26.000000 adatoolbox-0.0.8/src/adatoolbox/domain/secret/doppler.py
+-rw-r--r--   0 root         (0) root         (0)       55 2023-03-31 12:06:28.000000 adatoolbox-0.0.8/src/adatoolbox/domain/secret/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 15:38:50.540109 adatoolbox-0.0.8/src/adatoolbox/utils/
+-rw-r--r--   0 root         (0) root         (0)      293 2023-03-29 14:22:01.000000 adatoolbox-0.0.8/src/adatoolbox/utils/enum.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 15:38:46.669119 adatoolbox-0.0.8/src/adatoolbox.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      504 2023-04-25 15:38:44.000000 adatoolbox-0.0.8/src/adatoolbox.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      813 2023-04-25 15:38:44.000000 adatoolbox-0.0.8/src/adatoolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 15:38:44.000000 adatoolbox-0.0.8/src/adatoolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-04-25 15:38:44.000000 adatoolbox-0.0.8/src/adatoolbox.egg-info/top_level.txt
```

### Comparing `adatoolbox-0.0.7/LICENSE` & `adatoolbox-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `adatoolbox-0.0.7/pyproject.toml` & `adatoolbox-0.0.8/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 [tool.poetry]
 authors = ["Isaias Santana <isaiassantana@alojasengecon.com.br>"]
 description = "Biblioteca Lojas Engecon."
 name = "adatoolbox"
-version = "0.0.7"
+version = "0.0.8"
 
 [project]
 authors = [
   {name = "Lojas Engecon", email = "tecnologia@lojasengecon.com.br"},
 ]
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
 ]
 description = "adatoolbox"
 name = "adatoolbox"
 readme = "README.md"
 requires-python = ">=3.7"
-version = "0.0.7"
+version = "0.0.8"
 
 [project.urls]
 "Bug Tracker" = "https://github.com/lojas-engecon/toolbox/issues"
 "Homepage" = "https://github.com/lojas-engecon/toolbox"
 
 [tool.poetry.dependencies]
 build = "*"
+loguru = "^0.7.0"
+pika = "^1.3.1"
 python = "^3.9"
 twine = "*"
```

### Comparing `adatoolbox-0.0.7/src/adatoolbox/database/base_model.py` & `adatoolbox-0.0.8/src/adatoolbox/database/base_model.py`

 * *Files identical despite different names*

### Comparing `adatoolbox-0.0.7/src/adatoolbox/domain/auth/base_authentication.py` & `adatoolbox-0.0.8/src/adatoolbox/domain/auth/base_authentication.py`

 * *Files identical despite different names*

### Comparing `adatoolbox-0.0.7/src/adatoolbox/domain/secret/doppler.py` & `adatoolbox-0.0.8/src/adatoolbox/domain/secret/doppler.py`

 * *Files identical despite different names*

### Comparing `adatoolbox-0.0.7/src/adatoolbox.egg-info/SOURCES.txt` & `adatoolbox-0.0.8/src/adatoolbox.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -8,11 +8,15 @@
 src/adatoolbox.egg-info/top_level.txt
 src/adatoolbox/database/__init__.py
 src/adatoolbox/database/base_model.py
 src/adatoolbox/domain/auth/__init__.py
 src/adatoolbox/domain/auth/base_authentication.py
 src/adatoolbox/domain/auth/base_permission.py
 src/adatoolbox/domain/auth/settings.py
+src/adatoolbox/domain/event/__init__.py
+src/adatoolbox/domain/event/adapters/__init__.py
+src/adatoolbox/domain/event/adapters/mq_publisher_adapter.py
+src/adatoolbox/domain/event/adapters/pika_adapter.py
 src/adatoolbox/domain/secret/__init__.py
 src/adatoolbox/domain/secret/doppler.py
 src/adatoolbox/domain/secret/settings.py
 src/adatoolbox/utils/enum.py
```

