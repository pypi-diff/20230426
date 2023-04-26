# Comparing `tmp/pywrapid-0.2.7.tar.gz` & `tmp/pywrapid-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywrapid-0.2.7.tar", last modified: Thu Apr 20 11:59:05 2023, max compression
+gzip compressed data, was "pywrapid-0.2.8.tar", last modified: Tue Apr 25 14:08:42 2023, max compression
```

## Comparing `pywrapid-0.2.7.tar` & `pywrapid-0.2.8.tar`

### file list

```diff
@@ -1,61 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:05.251779 pywrapid-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-20 11:58:52.000000 pywrapid-0.2.7/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:05.247779 pywrapid-0.2.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:05.247779 pywrapid-0.2.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-04-20 11:58:52.000000 pywrapid-0.2.7/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-20 11:58:52.000000 pywrapid-0.2.7/.github/workflows/dependency-review.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-20 11:58:52.000000 pywrapid-0.2.7/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-04-20 11:58:52.000000 pywrapid-0.2.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-04-20 11:58:52.000000 pywrapid-0.2.7/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-20 11:58:52.000000 pywrapid-0.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5986 2023-04-20 11:59:05.251779 pywrapid-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-04-20 11:58:52.000000 pywrapid-0.2.7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:05.247779 pywrapid-0.2.7/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:05.247779 pywrapid-0.2.7/docs/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-04-20 11:58:52.000000 pywrapid-0.2.7/docs/src/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-20 11:58:52.000000 pywrapid-0.2.7/docs/src/developer-guide.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:05.247779 pywrapid-0.2.7/docs/src/features/
--rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-04-20 11:58:52.000000 pywrapid-0.2.7/docs/src/features/config.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6096 2023-04-20 11:58:52.000000 pywrapid-0.2.7/docs/src/features/log.rst
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-20 11:58:52.000000 pywrapid-0.2.7/docs/src/features/utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-04-20 11:58:52.000000 pywrapid-0.2.7/docs/src/features/webclient.rst
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-20 11:58:52.000000 pywrapid-0.2.7/docs/src/features.rst
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-20 11:58:52.000000 pywrapid-0.2.7/docs/src/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-20 11:58:52.000000 pywrapid-0.2.7/docs/src/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-04-20 11:58:52.000000 pywrapid-0.2.7/docs/src/user-guide.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-04-20 11:58:52.000000 pywrapid-0.2.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-20 11:58:52.000000 pywrapid-0.2.7/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-20 11:58:52.000000 pywrapid-0.2.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 11:59:05.251779 pywrapid-0.2.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:05.247779 pywrapid-0.2.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:05.247779 pywrapid-0.2.7/src/pywrapid/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-20 11:58:52.000000 pywrapid-0.2.7/src/pywrapid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:05.251779 pywrapid-0.2.7/src/pywrapid/config/
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-20 11:58:52.000000 pywrapid-0.2.7/src/pywrapid/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10107 2023-04-20 11:58:52.000000 pywrapid-0.2.7/src/pywrapid/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-20 11:58:52.000000 pywrapid-0.2.7/src/pywrapid/config/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-20 11:58:52.000000 pywrapid-0.2.7/src/pywrapid/config/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:05.251779 pywrapid-0.2.7/src/pywrapid/log/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-20 11:58:52.000000 pywrapid-0.2.7/src/pywrapid/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-04-20 11:58:52.000000 pywrapid-0.2.7/src/pywrapid/log/application_log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:05.251779 pywrapid-0.2.7/src/pywrapid/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-20 11:58:52.000000 pywrapid-0.2.7/src/pywrapid/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-04-20 11:58:52.000000 pywrapid-0.2.7/src/pywrapid/utils/dict_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-20 11:58:52.000000 pywrapid-0.2.7/src/pywrapid/utils/file_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:05.251779 pywrapid-0.2.7/src/pywrapid/webclient/
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-20 11:58:52.000000 pywrapid-0.2.7/src/pywrapid/webclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-04-20 11:58:52.000000 pywrapid-0.2.7/src/pywrapid/webclient/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-20 11:58:52.000000 pywrapid-0.2.7/src/pywrapid/webclient/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    13714 2023-04-20 11:58:52.000000 pywrapid-0.2.7/src/pywrapid/webclient/web.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:05.251779 pywrapid-0.2.7/src/pywrapid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5986 2023-04-20 11:59:05.000000 pywrapid-0.2.7/src/pywrapid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-04-20 11:59:05.000000 pywrapid-0.2.7/src/pywrapid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 11:59:05.000000 pywrapid-0.2.7/src/pywrapid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-20 11:59:05.000000 pywrapid-0.2.7/src/pywrapid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-20 11:59:05.000000 pywrapid-0.2.7/src/pywrapid.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:05.251779 pywrapid-0.2.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-20 11:58:52.000000 pywrapid-0.2.7/tests/test_conf_ok.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-04-20 11:58:52.000000 pywrapid-0.2.7/tests/test_pywrapid_config_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7643 2023-04-20 11:58:52.000000 pywrapid-0.2.7/tests/test_pywrapid_logging_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     7709 2023-04-20 11:58:52.000000 pywrapid-0.2.7/tests/test_pywrapid_webclient_web.py
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-04-20 11:58:52.000000 pywrapid-0.2.7/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:08:42.406487 pywrapid-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-25 14:08:31.000000 pywrapid-0.2.8/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:08:42.398487 pywrapid-0.2.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:08:42.402487 pywrapid-0.2.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-04-25 14:08:31.000000 pywrapid-0.2.8/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-25 14:08:31.000000 pywrapid-0.2.8/.github/workflows/dependency-review.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-25 14:08:31.000000 pywrapid-0.2.8/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-04-25 14:08:31.000000 pywrapid-0.2.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-04-25 14:08:31.000000 pywrapid-0.2.8/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-25 14:08:31.000000 pywrapid-0.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5986 2023-04-25 14:08:42.406487 pywrapid-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-04-25 14:08:31.000000 pywrapid-0.2.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:08:42.398487 pywrapid-0.2.8/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:08:42.402487 pywrapid-0.2.8/docs/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-04-25 14:08:31.000000 pywrapid-0.2.8/docs/src/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-25 14:08:31.000000 pywrapid-0.2.8/docs/src/developer-guide.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:08:42.402487 pywrapid-0.2.8/docs/src/features/
+-rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-04-25 14:08:31.000000 pywrapid-0.2.8/docs/src/features/config.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6096 2023-04-25 14:08:31.000000 pywrapid-0.2.8/docs/src/features/log.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-25 14:08:31.000000 pywrapid-0.2.8/docs/src/features/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-04-25 14:08:31.000000 pywrapid-0.2.8/docs/src/features/webclient.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-25 14:08:31.000000 pywrapid-0.2.8/docs/src/features.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-25 14:08:31.000000 pywrapid-0.2.8/docs/src/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-25 14:08:31.000000 pywrapid-0.2.8/docs/src/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-04-25 14:08:31.000000 pywrapid-0.2.8/docs/src/user-guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-04-25 14:08:31.000000 pywrapid-0.2.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-25 14:08:31.000000 pywrapid-0.2.8/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-25 14:08:31.000000 pywrapid-0.2.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 14:08:42.406487 pywrapid-0.2.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:08:42.398487 pywrapid-0.2.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:08:42.402487 pywrapid-0.2.8/src/pywrapid/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-25 14:08:31.000000 pywrapid-0.2.8/src/pywrapid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:08:42.402487 pywrapid-0.2.8/src/pywrapid/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-25 14:08:31.000000 pywrapid-0.2.8/src/pywrapid/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10150 2023-04-25 14:08:31.000000 pywrapid-0.2.8/src/pywrapid/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-25 14:08:31.000000 pywrapid-0.2.8/src/pywrapid/config/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-25 14:08:31.000000 pywrapid-0.2.8/src/pywrapid/config/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:08:42.402487 pywrapid-0.2.8/src/pywrapid/log/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-25 14:08:31.000000 pywrapid-0.2.8/src/pywrapid/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-04-25 14:08:31.000000 pywrapid-0.2.8/src/pywrapid/log/application_log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:08:42.402487 pywrapid-0.2.8/src/pywrapid/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-25 14:08:31.000000 pywrapid-0.2.8/src/pywrapid/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-04-25 14:08:31.000000 pywrapid-0.2.8/src/pywrapid/utils/dict_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7516 2023-04-25 14:08:31.000000 pywrapid-0.2.8/src/pywrapid/utils/file_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:08:42.402487 pywrapid-0.2.8/src/pywrapid/webclient/
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-25 14:08:31.000000 pywrapid-0.2.8/src/pywrapid/webclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-04-25 14:08:31.000000 pywrapid-0.2.8/src/pywrapid/webclient/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-25 14:08:31.000000 pywrapid-0.2.8/src/pywrapid/webclient/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    13740 2023-04-25 14:08:31.000000 pywrapid-0.2.8/src/pywrapid/webclient/web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:08:42.402487 pywrapid-0.2.8/src/pywrapid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5986 2023-04-25 14:08:42.000000 pywrapid-0.2.8/src/pywrapid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-25 14:08:42.000000 pywrapid-0.2.8/src/pywrapid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 14:08:42.000000 pywrapid-0.2.8/src/pywrapid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-25 14:08:42.000000 pywrapid-0.2.8/src/pywrapid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-25 14:08:42.000000 pywrapid-0.2.8/src/pywrapid.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:08:42.402487 pywrapid-0.2.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-25 14:08:31.000000 pywrapid-0.2.8/tests/test_conf_ok.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-04-25 14:08:31.000000 pywrapid-0.2.8/tests/test_pywrapid_config_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7643 2023-04-25 14:08:31.000000 pywrapid-0.2.8/tests/test_pywrapid_logging_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12134 2023-04-25 14:08:31.000000 pywrapid-0.2.8/tests/test_pywrapid_utils_file_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7709 2023-04-25 14:08:31.000000 pywrapid-0.2.8/tests/test_pywrapid_webclient_web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-04-25 14:08:31.000000 pywrapid-0.2.8/tox.ini
```

### Comparing `pywrapid-0.2.7/.github/workflows/codeql.yml` & `pywrapid-0.2.8/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `pywrapid-0.2.7/.github/workflows/dependency-review.yml` & `pywrapid-0.2.8/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `pywrapid-0.2.7/.github/workflows/python-publish.yml` & `pywrapid-0.2.8/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pywrapid-0.2.7/.gitignore` & `pywrapid-0.2.8/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 nosetests.xml
 coverage.xml
 *.cover
 *.py,cover
 .hypothesis/
 .pytest_cache/
 pynguin-report/
+junit/
 
 # Translations
 *.mo
 *.pot
 
 # Django stuff:
 *.log
```

### Comparing `pywrapid-0.2.7/CODE_OF_CONDUCT.md` & `pywrapid-0.2.8/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pywrapid-0.2.7/LICENSE` & `pywrapid-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pywrapid-0.2.7/PKG-INFO` & `pywrapid-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywrapid
-Version: 0.2.7
+Version: 0.2.8
 Summary: Collection of wrapper libraries for rapid development of python applications
 Author-email: Jonas Werme <jonas.werme@nsahq.se>, Marcus Wallgren <marcus.wallgren@nsahq.se>
 Maintainer-email: Jonas Werme <jonas.werme@nsahq.se>, Marcus Wallgren <marcus.wallgren@nsahq.se>
 License: MIT License
         
         Copyright (c) 2022 NSAHQ
```

### Comparing `pywrapid-0.2.7/README.rst` & `pywrapid-0.2.8/README.rst`

 * *Files identical despite different names*

### Comparing `pywrapid-0.2.7/docs/src/conf.py` & `pywrapid-0.2.8/docs/src/conf.py`

 * *Files identical despite different names*

### Comparing `pywrapid-0.2.7/docs/src/developer-guide.rst` & `pywrapid-0.2.8/docs/src/developer-guide.rst`

 * *Files identical despite different names*

### Comparing `pywrapid-0.2.7/docs/src/features/config.rst` & `pywrapid-0.2.8/docs/src/features/config.rst`

 * *Files identical despite different names*

### Comparing `pywrapid-0.2.7/docs/src/features/log.rst` & `pywrapid-0.2.8/docs/src/features/log.rst`

 * *Files identical despite different names*

### Comparing `pywrapid-0.2.7/docs/src/features/webclient.rst` & `pywrapid-0.2.8/docs/src/features/webclient.rst`

 * *Files identical despite different names*

### Comparing `pywrapid-0.2.7/docs/src/user-guide.rst` & `pywrapid-0.2.8/docs/src/user-guide.rst`

 * *Files identical despite different names*

### Comparing `pywrapid-0.2.7/pyproject.toml` & `pywrapid-0.2.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pywrapid-0.2.7/src/pywrapid/config/config.py` & `pywrapid-0.2.8/src/pywrapid/config/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -237,16 +237,17 @@
         try:
             with open(config, "r", encoding="utf-8-sig") as file:
                 cfg = yaml.safe_load(file)
 
             if expected_keys != []:
                 self.validate_keys(expected_keys, allow_empty)
 
-        except FileNotFoundError:
-            ConfigurationFileNotFoundError(f"Configuration file not found: {config}")
+        except FileNotFoundError as error:
+            raise ConfigurationFileNotFoundError(
+                f"Configuration file not found: {config}") from error
         except ValueError as error:
             raise ConfigurationError(f"Configuration value error for {config}: {error}") from error
         except Exception as error:
             raise ConfigurationError(f"File error for {config}: {error}") from error
 
         return cfg
```

### Comparing `pywrapid-0.2.7/src/pywrapid/config/exceptions.py` & `pywrapid-0.2.8/src/pywrapid/config/exceptions.py`

 * *Files identical despite different names*

### Comparing `pywrapid-0.2.7/src/pywrapid/log/application_log.py` & `pywrapid-0.2.8/src/pywrapid/log/application_log.py`

 * *Files identical despite different names*

### Comparing `pywrapid-0.2.7/src/pywrapid/utils/dict_tools.py` & `pywrapid-0.2.8/src/pywrapid/utils/dict_tools.py`

 * *Files identical despite different names*

### Comparing `pywrapid-0.2.7/src/pywrapid/webclient/__init__.py` & `pywrapid-0.2.8/src/pywrapid/webclient/__init__.py`

 * *Files identical despite different names*

### Comparing `pywrapid-0.2.7/src/pywrapid/webclient/exceptions.py` & `pywrapid-0.2.8/src/pywrapid/webclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `pywrapid-0.2.7/src/pywrapid/webclient/web.py` & `pywrapid-0.2.8/src/pywrapid/webclient/web.py`

 * *Files 0% similar despite different names*

```diff
@@ -240,15 +240,15 @@
             self._config = wrapid_config.cfg
         elif dict_config:
             self._config = dict_config
 
         self._authorization_type = authorization_type
 
         if credentials:
-            self._credential_options: dict = dict(**credentials.options)
+            self._credential_options: dict = dict(**credentials.options)  #  pylint: disable=R1735
             self._login_url = str(credentials.login_url)
         self._authorization_expiry = datetime.now()
         self._access_token = ""  # nosec
 
         try:
             AuthorizationType(authorization_type).name
         except ValueError as error:
```

### Comparing `pywrapid-0.2.7/src/pywrapid.egg-info/PKG-INFO` & `pywrapid-0.2.8/src/pywrapid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywrapid
-Version: 0.2.7
+Version: 0.2.8
 Summary: Collection of wrapper libraries for rapid development of python applications
 Author-email: Jonas Werme <jonas.werme@nsahq.se>, Marcus Wallgren <marcus.wallgren@nsahq.se>
 Maintainer-email: Jonas Werme <jonas.werme@nsahq.se>, Marcus Wallgren <marcus.wallgren@nsahq.se>
 License: MIT License
         
         Copyright (c) 2022 NSAHQ
```

### Comparing `pywrapid-0.2.7/src/pywrapid.egg-info/SOURCES.txt` & `pywrapid-0.2.8/src/pywrapid.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -38,8 +38,9 @@
 src/pywrapid/webclient/__init__.py
 src/pywrapid/webclient/exceptions.py
 src/pywrapid/webclient/requirements.txt
 src/pywrapid/webclient/web.py
 tests/test_conf_ok.yml
 tests/test_pywrapid_config_config.py
 tests/test_pywrapid_logging_logging.py
+tests/test_pywrapid_utils_file_tools.py
 tests/test_pywrapid_webclient_web.py
```

### Comparing `pywrapid-0.2.7/tests/test_pywrapid_config_config.py` & `pywrapid-0.2.8/tests/test_pywrapid_config_config.py`

 * *Files identical despite different names*

### Comparing `pywrapid-0.2.7/tests/test_pywrapid_logging_logging.py` & `pywrapid-0.2.8/tests/test_pywrapid_logging_logging.py`

 * *Files identical despite different names*

### Comparing `pywrapid-0.2.7/tests/test_pywrapid_webclient_web.py` & `pywrapid-0.2.8/tests/test_pywrapid_webclient_web.py`

 * *Files identical despite different names*

### Comparing `pywrapid-0.2.7/tox.ini` & `pywrapid-0.2.8/tox.ini`

 * *Files 17% similar despite different names*

```diff
@@ -12,24 +12,21 @@
     pyjwt
 
 [testenv:coverage]
 deps =
     coverage
     {[testenv]deps}
 commands =
-    coverage run -m pytest {posargs}
-    coverage combine
-    coverage report
-    coverage html -d docs/build/coverage
+    coverage run -m pytest --cov={envsitepackagesdir}/pywrapid --cov-report html {posargs}
 
 [testenv:tests]
 deps =
     {[testenv]deps}
 commands =
-    python -m pytest {posargs}
+    python -m pytest --junitxml=junit/junit-{envname}.xml {posargs}
 
 [testenv:flake8]
 basepython = python3
 skip_install = true
 deps =
     flake8
 commands =
@@ -106,35 +103,36 @@
     setuptools
     build
 commands =
     python -m build
 
 [testenv:docs]
 basepython = python3
+allowlist_externals = coverage
 deps =
     -r{toxinidir}/docs/src/requirements.txt
-    {[testenv:coverage]deps}
 commands =
     sphinx-build -E -W -c docs/src/ -b singlehtml docs/src/ docs/build/html
     #sphinx-build -E -W -c docs/src/ -b man docs/src/ docs/build/man
-    {[testenv:coverage]commands}
-
 
 [coverage:paths]
 source =
     src/
     **/site-packages/
 tests =
     tests
 
+[coverage:html]
+directory = docs/build/coverage/
+
 [coverage:run]
 branch = True
 parallel = true
 source =
-    tests
+    src/
 omit =
     */__init__.py
     */__main__.py
 
 [coverage:report]
 show_missing = True
 sort = Cover
@@ -145,8 +143,8 @@
 
     # Debug
     def __repr__
     if self\.debug
 
     # Non-runnable
     if 0:
-    if __name__ == .__main__.:
+    if __name__ == .__main__.:
```

