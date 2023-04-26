# Comparing `tmp/pytest-operator-0.9.0.tar.gz` & `tmp/pytest-operator-1.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-operator-0.9.0.tar", last modified: Tue Oct 26 17:45:56 2021, max compression
+gzip compressed data, was "pytest-operator-1.0.0b1.tar", last modified: Wed Sep 28 13:27:31 2022, max compression
```

## Comparing `pytest-operator-0.9.0.tar` & `pytest-operator-1.0.0b1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxr-x   0 johnsca   (1000) johnsca   (1000)        0 2021-10-26 17:45:56.672141 pytest-operator-0.9.0/
--rw-rw-r--   0 johnsca   (1000) johnsca   (1000)    11357 2021-02-04 16:38:27.000000 pytest-operator-0.9.0/LICENSE
--rw-rw-r--   0 johnsca   (1000) johnsca   (1000)     1969 2021-10-26 17:45:56.672141 pytest-operator-0.9.0/PKG-INFO
--rw-rw-r--   0 johnsca   (1000) johnsca   (1000)     1325 2021-07-23 18:13:09.000000 pytest-operator-0.9.0/README.md
-drwxrwxr-x   0 johnsca   (1000) johnsca   (1000)        0 2021-10-26 17:45:56.672141 pytest-operator-0.9.0/pytest_operator/
--rw-rw-r--   0 johnsca   (1000) johnsca   (1000)       28 2021-03-16 21:05:43.000000 pytest-operator-0.9.0/pytest_operator/__init__.py
--rw-rw-r--   0 johnsca   (1000) johnsca   (1000)    22564 2021-10-26 17:44:53.000000 pytest-operator-0.9.0/pytest_operator/plugin.py
--rw-rw-r--   0 johnsca   (1000) johnsca   (1000)      277 2021-02-10 15:49:44.000000 pytest-operator-0.9.0/pytest_operator/shims.py
-drwxrwxr-x   0 johnsca   (1000) johnsca   (1000)        0 2021-10-26 17:45:56.672141 pytest-operator-0.9.0/pytest_operator.egg-info/
--rw-rw-r--   0 johnsca   (1000) johnsca   (1000)     1969 2021-10-26 17:45:56.000000 pytest-operator-0.9.0/pytest_operator.egg-info/PKG-INFO
--rw-rw-r--   0 johnsca   (1000) johnsca   (1000)      375 2021-10-26 17:45:56.000000 pytest-operator-0.9.0/pytest_operator.egg-info/SOURCES.txt
--rw-rw-r--   0 johnsca   (1000) johnsca   (1000)        1 2021-10-26 17:45:56.000000 pytest-operator-0.9.0/pytest_operator.egg-info/dependency_links.txt
--rw-rw-r--   0 johnsca   (1000) johnsca   (1000)       53 2021-10-26 17:45:56.000000 pytest-operator-0.9.0/pytest_operator.egg-info/entry_points.txt
--rw-rw-r--   0 johnsca   (1000) johnsca   (1000)       46 2021-10-26 17:45:56.000000 pytest-operator-0.9.0/pytest_operator.egg-info/requires.txt
--rw-rw-r--   0 johnsca   (1000) johnsca   (1000)       16 2021-10-26 17:45:56.000000 pytest-operator-0.9.0/pytest_operator.egg-info/top_level.txt
--rw-rw-r--   0 johnsca   (1000) johnsca   (1000)        1 2021-07-23 19:04:57.000000 pytest-operator-0.9.0/pytest_operator.egg-info/zip-safe
--rw-rw-r--   0 johnsca   (1000) johnsca   (1000)       38 2021-10-26 17:45:56.672141 pytest-operator-0.9.0/setup.cfg
--rw-rw-r--   0 johnsca   (1000) johnsca   (1000)     1210 2021-10-26 17:45:22.000000 pytest-operator-0.9.0/setup.py
+drwxrwxr-x   0 addyess   (1000) addyess   (1000)        0 2022-09-28 13:27:31.714097 pytest-operator-1.0.0b1/
+-rw-rw-r--   0 addyess   (1000) addyess   (1000)    11357 2022-01-18 21:07:11.000000 pytest-operator-1.0.0b1/LICENSE
+-rw-rw-r--   0 addyess   (1000) addyess   (1000)     3283 2022-09-28 13:27:31.714097 pytest-operator-1.0.0b1/PKG-INFO
+-rw-rw-r--   0 addyess   (1000) addyess   (1000)     2657 2022-02-14 22:37:15.000000 pytest-operator-1.0.0b1/README.md
+drwxrwxr-x   0 addyess   (1000) addyess   (1000)        0 2022-09-28 13:27:31.714097 pytest-operator-1.0.0b1/pytest_operator/
+-rw-rw-r--   0 addyess   (1000) addyess   (1000)       28 2022-01-18 21:07:11.000000 pytest-operator-1.0.0b1/pytest_operator/__init__.py
+-rw-rw-r--   0 addyess   (1000) addyess   (1000)    53599 2022-09-23 13:45:23.000000 pytest-operator-1.0.0b1/pytest_operator/plugin.py
+-rw-rw-r--   0 addyess   (1000) addyess   (1000)        0 2022-08-17 14:56:02.000000 pytest-operator-1.0.0b1/pytest_operator/py.typed
+-rw-rw-r--   0 addyess   (1000) addyess   (1000)      353 2022-09-20 21:34:51.000000 pytest-operator-1.0.0b1/pytest_operator/shims.py
+drwxrwxr-x   0 addyess   (1000) addyess   (1000)        0 2022-09-28 13:27:31.714097 pytest-operator-1.0.0b1/pytest_operator.egg-info/
+-rw-rw-r--   0 addyess   (1000) addyess   (1000)     3283 2022-09-28 13:27:31.000000 pytest-operator-1.0.0b1/pytest_operator.egg-info/PKG-INFO
+-rw-rw-r--   0 addyess   (1000) addyess   (1000)      400 2022-09-28 13:27:31.000000 pytest-operator-1.0.0b1/pytest_operator.egg-info/SOURCES.txt
+-rw-rw-r--   0 addyess   (1000) addyess   (1000)        1 2022-09-28 13:27:31.000000 pytest-operator-1.0.0b1/pytest_operator.egg-info/dependency_links.txt
+-rw-rw-r--   0 addyess   (1000) addyess   (1000)       52 2022-09-28 13:27:31.000000 pytest-operator-1.0.0b1/pytest_operator.egg-info/entry_points.txt
+-rw-rw-r--   0 addyess   (1000) addyess   (1000)       46 2022-09-28 13:27:31.000000 pytest-operator-1.0.0b1/pytest_operator.egg-info/requires.txt
+-rw-rw-r--   0 addyess   (1000) addyess   (1000)       16 2022-09-28 13:27:31.000000 pytest-operator-1.0.0b1/pytest_operator.egg-info/top_level.txt
+-rw-rw-r--   0 addyess   (1000) addyess   (1000)        1 2022-05-25 15:01:57.000000 pytest-operator-1.0.0b1/pytest_operator.egg-info/zip-safe
+-rw-rw-r--   0 addyess   (1000) addyess   (1000)       38 2022-09-28 13:27:31.714097 pytest-operator-1.0.0b1/setup.cfg
+-rw-rw-r--   0 addyess   (1000) addyess   (1000)     1265 2022-09-21 13:51:35.000000 pytest-operator-1.0.0b1/setup.py
```

### Comparing `pytest-operator-0.9.0/LICENSE` & `pytest-operator-1.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-operator-0.9.0/setup.py` & `pytest-operator-1.0.0b1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -19,16 +19,17 @@
         "Programming Language :: Python :: 3.9",
     ],
     license="MIT license",
     include_package_data=True,
     keywords=["pytest", "py.test", "operators", "yaml", "asyncio"],
     name="pytest-operator",
     packages=find_packages(include=["pytest_operator"]),
+    package_data={'pytest_operator': ['py.typed']},
     url="https://github.com/charmed-kubernetes/pytest-operator",
-    version="0.9.0",
+    version="1.0.0.b1",
     zip_safe=True,
     install_requires=[
         "ipdb",
         "pytest",
         "pytest-asyncio",
         "pyyaml",
         "juju",
```

