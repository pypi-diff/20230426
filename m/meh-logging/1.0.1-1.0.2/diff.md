# Comparing `tmp/meh_logging-1.0.1.tar.gz` & `tmp/meh_logging-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meh_logging-1.0.1.tar", last modified: Tue Nov 15 13:39:46 2022, max compression
+gzip compressed data, was "meh_logging-1.0.2.tar", last modified: Wed Apr 26 14:13:40 2023, max compression
```

## Comparing `meh_logging-1.0.1.tar` & `meh_logging-1.0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 jim.de.ronde (8935743) AD\Domain Users (1915133461)        0 2022-11-15 13:39:46.835120 meh_logging-1.0.1/
--rw-r--r--   0 jim.de.ronde (8935743) AD\Domain Users (1915133461)     1069 2022-11-11 15:10:55.000000 meh_logging-1.0.1/LICENSE
--rw-r--r--   0 jim.de.ronde (8935743) AD\Domain Users (1915133461)     1155 2022-11-15 13:39:46.834721 meh_logging-1.0.1/PKG-INFO
--rw-r--r--   0 jim.de.ronde (8935743) AD\Domain Users (1915133461)      582 2022-11-11 15:10:55.000000 meh_logging-1.0.1/README.md
--rw-r--r--   0 jim.de.ronde (8935743) AD\Domain Users (1915133461)      646 2022-11-15 13:37:03.000000 meh_logging-1.0.1/pyproject.toml
--rw-r--r--   0 jim.de.ronde (8935743) AD\Domain Users (1915133461)       38 2022-11-15 13:39:46.835176 meh_logging-1.0.1/setup.cfg
-drwxr-xr-x   0 jim.de.ronde (8935743) AD\Domain Users (1915133461)        0 2022-11-15 13:39:46.814693 meh_logging-1.0.1/src/
-drwxr-xr-x   0 jim.de.ronde (8935743) AD\Domain Users (1915133461)        0 2022-11-15 13:39:46.819504 meh_logging-1.0.1/src/meh_logging/
--rw-r--r--   0 jim.de.ronde (8935743) AD\Domain Users (1915133461)      305 2022-11-15 12:26:59.000000 meh_logging-1.0.1/src/meh_logging/__init__.py
-drwxr-xr-x   0 jim.de.ronde (8935743) AD\Domain Users (1915133461)        0 2022-11-15 13:39:46.830178 meh_logging-1.0.1/src/meh_logging/enums/
--rw-r--r--   0 jim.de.ronde (8935743) AD\Domain Users (1915133461)      283 2022-11-11 15:10:55.000000 meh_logging-1.0.1/src/meh_logging/enums/levels.py
-drwxr-xr-x   0 jim.de.ronde (8935743) AD\Domain Users (1915133461)        0 2022-11-15 13:39:46.831240 meh_logging-1.0.1/src/meh_logging/formatters/
--rw-r--r--   0 jim.de.ronde (8935743) AD\Domain Users (1915133461)        0 2022-11-11 15:10:55.000000 meh_logging-1.0.1/src/meh_logging/formatters/__init__.py
--rw-r--r--   0 jim.de.ronde (8935743) AD\Domain Users (1915133461)      563 2022-11-15 09:46:25.000000 meh_logging-1.0.1/src/meh_logging/formatters/json.py
--rw-r--r--   0 jim.de.ronde (8935743) AD\Domain Users (1915133461)     2196 2022-11-15 11:57:02.000000 meh_logging-1.0.1/src/meh_logging/logger.py
-drwxr-xr-x   0 jim.de.ronde (8935743) AD\Domain Users (1915133461)        0 2022-11-15 13:39:46.832422 meh_logging-1.0.1/src/meh_logging/transports/
--rw-r--r--   0 jim.de.ronde (8935743) AD\Domain Users (1915133461)       67 2022-11-11 15:10:55.000000 meh_logging-1.0.1/src/meh_logging/transports/__init__.py
--rw-r--r--   0 jim.de.ronde (8935743) AD\Domain Users (1915133461)      425 2022-11-11 15:10:55.000000 meh_logging-1.0.1/src/meh_logging/transports/stream.py
-drwxr-xr-x   0 jim.de.ronde (8935743) AD\Domain Users (1915133461)        0 2022-11-15 13:39:46.834215 meh_logging-1.0.1/src/meh_logging/utils/
--rw-r--r--   0 jim.de.ronde (8935743) AD\Domain Users (1915133461)        0 2022-11-11 15:10:55.000000 meh_logging-1.0.1/src/meh_logging/utils/__init__.py
--rw-r--r--   0 jim.de.ronde (8935743) AD\Domain Users (1915133461)      955 2022-11-15 09:46:25.000000 meh_logging-1.0.1/src/meh_logging/utils/package.py
--rw-r--r--   0 jim.de.ronde (8935743) AD\Domain Users (1915133461)      335 2022-11-11 15:10:55.000000 meh_logging-1.0.1/src/meh_logging/utils/read_package.py
-drwxr-xr-x   0 jim.de.ronde (8935743) AD\Domain Users (1915133461)        0 2022-11-15 13:39:46.829521 meh_logging-1.0.1/src/meh_logging.egg-info/
--rw-r--r--   0 jim.de.ronde (8935743) AD\Domain Users (1915133461)     1155 2022-11-15 13:39:46.000000 meh_logging-1.0.1/src/meh_logging.egg-info/PKG-INFO
--rw-r--r--   0 jim.de.ronde (8935743) AD\Domain Users (1915133461)      529 2022-11-15 13:39:46.000000 meh_logging-1.0.1/src/meh_logging.egg-info/SOURCES.txt
--rw-r--r--   0 jim.de.ronde (8935743) AD\Domain Users (1915133461)        1 2022-11-15 13:39:46.000000 meh_logging-1.0.1/src/meh_logging.egg-info/dependency_links.txt
--rw-r--r--   0 jim.de.ronde (8935743) AD\Domain Users (1915133461)       12 2022-11-15 13:39:46.000000 meh_logging-1.0.1/src/meh_logging.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 14:13:40.387883 meh_logging-1.0.2/
+-rw-rw-rw-   0 root         (0) root         (0)     1069 2023-04-26 14:13:21.000000 meh_logging-1.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2141 2023-04-26 14:13:40.387883 meh_logging-1.0.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1568 2023-04-26 14:13:21.000000 meh_logging-1.0.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      646 2023-04-26 14:13:21.000000 meh_logging-1.0.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-26 14:13:40.387883 meh_logging-1.0.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 14:13:40.387883 meh_logging-1.0.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 14:13:40.387883 meh_logging-1.0.2/src/meh_logging/
+-rw-rw-rw-   0 root         (0) root         (0)      305 2023-04-26 14:13:21.000000 meh_logging-1.0.2/src/meh_logging/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 14:13:40.387883 meh_logging-1.0.2/src/meh_logging/enums/
+-rw-rw-rw-   0 root         (0) root         (0)      283 2023-04-26 14:13:21.000000 meh_logging-1.0.2/src/meh_logging/enums/levels.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 14:13:40.387883 meh_logging-1.0.2/src/meh_logging/formatters/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-26 14:13:21.000000 meh_logging-1.0.2/src/meh_logging/formatters/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      563 2023-04-26 14:13:21.000000 meh_logging-1.0.2/src/meh_logging/formatters/json.py
+-rw-rw-rw-   0 root         (0) root         (0)     2196 2023-04-26 14:13:21.000000 meh_logging-1.0.2/src/meh_logging/logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 14:13:40.387883 meh_logging-1.0.2/src/meh_logging/transports/
+-rw-rw-rw-   0 root         (0) root         (0)       67 2023-04-26 14:13:21.000000 meh_logging-1.0.2/src/meh_logging/transports/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      425 2023-04-26 14:13:21.000000 meh_logging-1.0.2/src/meh_logging/transports/stream.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 14:13:40.387883 meh_logging-1.0.2/src/meh_logging/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-26 14:13:21.000000 meh_logging-1.0.2/src/meh_logging/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      957 2023-04-26 14:13:21.000000 meh_logging-1.0.2/src/meh_logging/utils/package.py
+-rw-rw-rw-   0 root         (0) root         (0)      335 2023-04-26 14:13:21.000000 meh_logging-1.0.2/src/meh_logging/utils/read_package.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 14:13:40.387883 meh_logging-1.0.2/src/meh_logging.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2141 2023-04-26 14:13:40.000000 meh_logging-1.0.2/src/meh_logging.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      529 2023-04-26 14:13:40.000000 meh_logging-1.0.2/src/meh_logging.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 14:13:40.000000 meh_logging-1.0.2/src/meh_logging.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-04-26 14:13:40.000000 meh_logging-1.0.2/src/meh_logging.egg-info/top_level.txt
```

### Comparing `meh_logging-1.0.1/LICENSE` & `meh_logging-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `meh_logging-1.0.1/pyproject.toml` & `meh_logging-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "meh_logging"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Jim de Ronde", email="jim.de.ronde@greenhousegroup.com" },
 ]
 description = "Custom logging package for MEH projects."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `meh_logging-1.0.1/src/meh_logging/formatters/json.py` & `meh_logging-1.0.2/src/meh_logging/formatters/json.py`

 * *Files identical despite different names*

### Comparing `meh_logging-1.0.1/src/meh_logging/logger.py` & `meh_logging-1.0.2/src/meh_logging/logger.py`

 * *Files identical despite different names*

### Comparing `meh_logging-1.0.1/src/meh_logging/utils/package.py` & `meh_logging-1.0.2/src/meh_logging/utils/package.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,22 +14,24 @@
 
 # Fallbacks
 FALLBACK_PACKAGE_NAME = "unknown-app"
 FALLBACK_PACKAGE_VERSION = "0.0.0"
 
 PYTHON_ENV = os.getenv("ENV", os.getenv("PYTHON_ENV", ""))
 
+
 def parse_app_name(name):
     if PYTHON_ENV == "acceptance":
         return re.sub("-acc$", "", name)
     elif PYTHON_ENV == "test":
         return re.sub("-test$", "", name)
 
     return name
 
+
 package = read_package_file()
 
 app_name = package.get("name", FALLBACK_PACKAGE_NAME)
 app_name = parse_app_name(app_name)
 app_version = package.get("version", FALLBACK_PACKAGE_VERSION)
 
 JSON_DEFAULTS = {
```

### Comparing `meh_logging-1.0.1/src/meh_logging.egg-info/SOURCES.txt` & `meh_logging-1.0.2/src/meh_logging.egg-info/SOURCES.txt`

 * *Files identical despite different names*

