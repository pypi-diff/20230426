# Comparing `tmp/nua_agent-0.5.13.tar.gz` & `tmp/nua_agent-0.5.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nua_agent-0.5.13.tar", max compression
+gzip compressed data, was "nua_agent-0.5.14.tar", max compression
```

## Comparing `nua_agent-0.5.13.tar` & `nua_agent-0.5.14.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      793 2023-04-24 21:25:56.856175 nua_agent-0.5.13/README.md
--rw-r--r--   0        0        0     1436 2023-04-24 21:27:45.984067 nua_agent-0.5.13/pyproject.toml
--rw-r--r--   0        0        0      330 2023-04-06 11:40:42.165489 nua_agent-0.5.13/src/nua/agent/__init__.py
--rw-r--r--   0        0        0     1699 2023-04-24 21:25:56.857554 nua_agent-0.5.13/src/nua/agent/auto_install.py
--rw-r--r--   0        0        0      346 2023-02-28 08:14:12.790866 nua_agent-0.5.13/src/nua/agent/constants.py
--rw-r--r--   0        0        0        0 2023-02-06 17:21:30.492413 nua_agent-0.5.13/src/nua/agent/db/__init__.py
--rw-r--r--   0        0        0     1437 2023-02-06 17:21:30.492736 nua_agent-0.5.13/src/nua/agent/db/db_manager.py
--rw-r--r--   0        0        0     6233 2023-02-13 14:04:49.212138 nua_agent-0.5.13/src/nua/agent/db/mariadb_manager.py
--rw-r--r--   0        0        0     8651 2023-04-14 13:29:17.685138 nua_agent-0.5.13/src/nua/agent/db/postgres_manager.py
--rw-r--r--   0        0        0     2203 2023-02-15 19:18:03.537136 nua_agent-0.5.13/src/nua/agent/db/sqlite_manager.py
--rw-r--r--   0        0        0        0 2023-02-06 17:21:30.493328 nua_agent-0.5.13/src/nua/agent/deps/__init__.py
--rw-r--r--   0        0        0       75 2023-02-06 17:21:30.493417 nua_agent-0.5.13/src/nua/agent/deps/meta_packages.json
--rw-r--r--   0        0        0        0 2023-04-24 21:25:56.857636 nua_agent-0.5.13/src/nua/agent/detectors/__init__.py
--rw-r--r--   0        0        0     1114 2023-04-24 21:25:56.857882 nua_agent-0.5.13/src/nua/agent/detectors/base_detector.py
--rw-r--r--   0        0        0      950 2023-04-24 21:25:56.857950 nua_agent-0.5.13/src/nua/agent/detectors/nodejs_yarn.py
--rw-r--r--   0        0        0      646 2023-04-24 21:25:56.858041 nua_agent-0.5.13/src/nua/agent/detectors/python_source.py
--rw-r--r--   0        0        0      567 2023-04-24 21:25:56.858137 nua_agent-0.5.13/src/nua/agent/detectors/python_wheels.py
--rw-r--r--   0        0        0      497 2023-03-03 15:29:31.726769 nua_agent-0.5.13/src/nua/agent/meta_packages.py
--rw-r--r--   0        0        0    13027 2023-04-24 21:25:56.858265 nua_agent-0.5.13/src/nua/agent/nua_config.py
--rw-r--r--   0        0        0      544 2023-04-04 16:08:31.312095 nua_agent-0.5.13/src/nua/agent/nua_tag.py
--rw-r--r--   0        0        0        0 2023-02-06 17:21:30.493877 nua_agent-0.5.13/src/nua/agent/scripts/__init__.py
--rw-r--r--   0        0        0    11212 2023-04-24 21:25:56.858401 nua_agent-0.5.13/src/nua/agent/scripts/app_builder.py
--rw-r--r--   0        0        0     1583 2023-04-08 16:31:17.756437 nua_agent-0.5.13/src/nua/agent/templates.py
--rw-r--r--   0        0        0       81 2023-02-06 17:21:30.494088 nua_agent-0.5.13/src/nua/agent/version.py
--rw-r--r--   0        0        0     1363 1970-01-01 00:00:00.000000 nua_agent-0.5.13/PKG-INFO
+-rw-r--r--   0        0        0      793 2023-04-24 21:25:56.856175 nua_agent-0.5.14/README.md
+-rw-r--r--   0        0        0     1436 2023-04-26 06:46:41.656673 nua_agent-0.5.14/pyproject.toml
+-rw-r--r--   0        0        0      330 2023-04-06 11:40:42.165489 nua_agent-0.5.14/src/nua/agent/__init__.py
+-rw-r--r--   0        0        0     1699 2023-04-24 21:25:56.857554 nua_agent-0.5.14/src/nua/agent/auto_install.py
+-rw-r--r--   0        0        0      346 2023-02-28 08:14:12.790866 nua_agent-0.5.14/src/nua/agent/constants.py
+-rw-r--r--   0        0        0        0 2023-02-06 17:21:30.492413 nua_agent-0.5.14/src/nua/agent/db/__init__.py
+-rw-r--r--   0        0        0     1437 2023-02-06 17:21:30.492736 nua_agent-0.5.14/src/nua/agent/db/db_manager.py
+-rw-r--r--   0        0        0     6233 2023-02-13 14:04:49.212138 nua_agent-0.5.14/src/nua/agent/db/mariadb_manager.py
+-rw-r--r--   0        0        0     8651 2023-04-14 13:29:17.685138 nua_agent-0.5.14/src/nua/agent/db/postgres_manager.py
+-rw-r--r--   0        0        0     2203 2023-02-15 19:18:03.537136 nua_agent-0.5.14/src/nua/agent/db/sqlite_manager.py
+-rw-r--r--   0        0        0        0 2023-02-06 17:21:30.493328 nua_agent-0.5.14/src/nua/agent/deps/__init__.py
+-rw-r--r--   0        0        0       75 2023-02-06 17:21:30.493417 nua_agent-0.5.14/src/nua/agent/deps/meta_packages.json
+-rw-r--r--   0        0        0        0 2023-04-24 21:25:56.857636 nua_agent-0.5.14/src/nua/agent/detectors/__init__.py
+-rw-r--r--   0        0        0     1114 2023-04-24 21:25:56.857882 nua_agent-0.5.14/src/nua/agent/detectors/base_detector.py
+-rw-r--r--   0        0        0      950 2023-04-24 21:25:56.857950 nua_agent-0.5.14/src/nua/agent/detectors/nodejs_yarn.py
+-rw-r--r--   0        0        0      646 2023-04-24 21:25:56.858041 nua_agent-0.5.14/src/nua/agent/detectors/python_source.py
+-rw-r--r--   0        0        0      567 2023-04-24 21:25:56.858137 nua_agent-0.5.14/src/nua/agent/detectors/python_wheels.py
+-rw-r--r--   0        0        0      497 2023-03-03 15:29:31.726769 nua_agent-0.5.14/src/nua/agent/meta_packages.py
+-rw-r--r--   0        0        0    13027 2023-04-24 21:25:56.858265 nua_agent-0.5.14/src/nua/agent/nua_config.py
+-rw-r--r--   0        0        0      544 2023-04-04 16:08:31.312095 nua_agent-0.5.14/src/nua/agent/nua_tag.py
+-rw-r--r--   0        0        0        0 2023-02-06 17:21:30.493877 nua_agent-0.5.14/src/nua/agent/scripts/__init__.py
+-rw-r--r--   0        0        0    11212 2023-04-24 21:25:56.858401 nua_agent-0.5.14/src/nua/agent/scripts/app_builder.py
+-rw-r--r--   0        0        0     1583 2023-04-08 16:31:17.756437 nua_agent-0.5.14/src/nua/agent/templates.py
+-rw-r--r--   0        0        0       81 2023-02-06 17:21:30.494088 nua_agent-0.5.14/src/nua/agent/version.py
+-rw-r--r--   0        0        0     1363 1970-01-01 00:00:00.000000 nua_agent-0.5.14/PKG-INFO
```

### Comparing `nua_agent-0.5.13/README.md` & `nua_agent-0.5.14/README.md`

 * *Files identical despite different names*

### Comparing `nua_agent-0.5.13/pyproject.toml` & `nua_agent-0.5.14/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nua-agent"
-version = "0.5.13"
+version = "0.5.14"
 description = "Nua agent"
 authors = [
     "Stefane Fermigier <sf@abilian.com>",
     "Jerome Dumonteil <jd@abilian.com>",
 ]
 license = "AGPL"
 readme = "README.md"
@@ -12,15 +12,15 @@
     { include = "nua", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 setuptools = "*"
 packaging = "*"
-nua-lib = "=0.5.13"
+nua-lib = "=0.5.14"
 tomli = "^2.0.1"
 pyyaml = "^6.0"
 
 [tool.poetry.group.dev.dependencies]
 abilian-devtools = "*"
 nox = "*"
 types-setuptools = "*"
```

### Comparing `nua_agent-0.5.13/src/nua/agent/auto_install.py` & `nua_agent-0.5.14/src/nua/agent/auto_install.py`

 * *Files identical despite different names*

### Comparing `nua_agent-0.5.13/src/nua/agent/db/db_manager.py` & `nua_agent-0.5.14/src/nua/agent/db/db_manager.py`

 * *Files identical despite different names*

### Comparing `nua_agent-0.5.13/src/nua/agent/db/mariadb_manager.py` & `nua_agent-0.5.14/src/nua/agent/db/mariadb_manager.py`

 * *Files identical despite different names*

### Comparing `nua_agent-0.5.13/src/nua/agent/db/postgres_manager.py` & `nua_agent-0.5.14/src/nua/agent/db/postgres_manager.py`

 * *Files identical despite different names*

### Comparing `nua_agent-0.5.13/src/nua/agent/db/sqlite_manager.py` & `nua_agent-0.5.14/src/nua/agent/db/sqlite_manager.py`

 * *Files identical despite different names*

### Comparing `nua_agent-0.5.13/src/nua/agent/detectors/base_detector.py` & `nua_agent-0.5.14/src/nua/agent/detectors/base_detector.py`

 * *Files identical despite different names*

### Comparing `nua_agent-0.5.13/src/nua/agent/detectors/nodejs_yarn.py` & `nua_agent-0.5.14/src/nua/agent/detectors/nodejs_yarn.py`

 * *Files identical despite different names*

### Comparing `nua_agent-0.5.13/src/nua/agent/detectors/python_source.py` & `nua_agent-0.5.14/src/nua/agent/detectors/python_source.py`

 * *Files identical despite different names*

### Comparing `nua_agent-0.5.13/src/nua/agent/detectors/python_wheels.py` & `nua_agent-0.5.14/src/nua/agent/detectors/python_wheels.py`

 * *Files identical despite different names*

### Comparing `nua_agent-0.5.13/src/nua/agent/nua_config.py` & `nua_agent-0.5.14/src/nua/agent/nua_config.py`

 * *Files identical despite different names*

### Comparing `nua_agent-0.5.13/src/nua/agent/nua_tag.py` & `nua_agent-0.5.14/src/nua/agent/nua_tag.py`

 * *Files identical despite different names*

### Comparing `nua_agent-0.5.13/src/nua/agent/scripts/app_builder.py` & `nua_agent-0.5.14/src/nua/agent/scripts/app_builder.py`

 * *Files identical despite different names*

### Comparing `nua_agent-0.5.13/src/nua/agent/templates.py` & `nua_agent-0.5.14/src/nua/agent/templates.py`

 * *Files identical despite different names*

### Comparing `nua_agent-0.5.13/PKG-INFO` & `nua_agent-0.5.14/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: nua-agent
-Version: 0.5.13
+Version: 0.5.14
 Summary: Nua agent
 License: AGPL
 Author: Stefane Fermigier
 Author-email: sf@abilian.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: nua-lib (==0.5.13)
+Requires-Dist: nua-lib (==0.5.14)
 Requires-Dist: packaging
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: setuptools
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Nua Agent
```

