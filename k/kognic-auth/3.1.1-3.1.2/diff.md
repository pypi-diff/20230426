# Comparing `tmp/kognic-auth-3.1.1.tar.gz` & `tmp/kognic-auth-3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kognic-auth-3.1.1.tar", last modified: Tue Apr 25 13:45:57 2023, max compression
+gzip compressed data, was "kognic-auth-3.1.2.tar", last modified: Tue Apr 25 14:01:21 2023, max compression
```

## Comparing `kognic-auth-3.1.1.tar` & `kognic-auth-3.1.2.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:45:57.380508 kognic-auth-3.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:45:57.372508 kognic-auth-3.1.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-25 13:45:44.000000 kognic-auth-3.1.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:45:57.372508 kognic-auth-3.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-04-25 13:45:44.000000 kognic-auth-3.1.1/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-25 13:45:44.000000 kognic-auth-3.1.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-25 13:45:44.000000 kognic-auth-3.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-04-25 13:45:57.380508 kognic-auth-3.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-04-25 13:45:44.000000 kognic-auth-3.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-25 13:45:44.000000 kognic-auth-3.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 13:45:57.380508 kognic-auth-3.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:45:57.372508 kognic-auth-3.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:45:57.368508 kognic-auth-3.1.1/src/kognic/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:45:57.376508 kognic-auth-3.1.1/src/kognic/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-25 13:45:44.000000 kognic-auth-3.1.1/src/kognic/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-25 13:45:57.000000 kognic-auth-3.1.1/src/kognic/auth/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:45:57.376508 kognic-auth-3.1.1/src/kognic/auth/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 13:45:44.000000 kognic-auth-3.1.1/src/kognic/auth/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-25 13:45:44.000000 kognic-auth-3.1.1/src/kognic/auth/base/auth_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-04-25 13:45:44.000000 kognic-auth-3.1.1/src/kognic/auth/credentials_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:45:57.376508 kognic-auth-3.1.1/src/kognic/auth/httpx/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 13:45:44.000000 kognic-auth-3.1.1/src/kognic/auth/httpx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-04-25 13:45:44.000000 kognic-auth-3.1.1/src/kognic/auth/httpx/async_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:45:57.376508 kognic-auth-3.1.1/src/kognic/auth/requests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 13:45:44.000000 kognic-auth-3.1.1/src/kognic/auth/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-04-25 13:45:44.000000 kognic-auth-3.1.1/src/kognic/auth/requests/auth_session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:45:57.376508 kognic-auth-3.1.1/src/kognic_auth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-04-25 13:45:57.000000 kognic-auth-3.1.1/src/kognic_auth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-25 13:45:57.000000 kognic-auth-3.1.1/src/kognic_auth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 13:45:57.000000 kognic-auth-3.1.1/src/kognic_auth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-25 13:45:57.000000 kognic-auth-3.1.1/src/kognic_auth.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-25 13:45:57.000000 kognic-auth-3.1.1/src/kognic_auth.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:45:57.380508 kognic-auth-3.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-25 13:45:44.000000 kognic-auth-3.1.1/tests/credentials_parser_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:01:21.001928 kognic-auth-3.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:01:20.997928 kognic-auth-3.1.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-25 14:01:06.000000 kognic-auth-3.1.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:01:20.997928 kognic-auth-3.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-04-25 14:01:06.000000 kognic-auth-3.1.2/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-25 14:01:06.000000 kognic-auth-3.1.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-25 14:01:06.000000 kognic-auth-3.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-25 14:01:06.000000 kognic-auth-3.1.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-04-25 14:01:21.001928 kognic-auth-3.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-04-25 14:01:06.000000 kognic-auth-3.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-25 14:01:06.000000 kognic-auth-3.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 14:01:21.001928 kognic-auth-3.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:01:20.997928 kognic-auth-3.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:01:20.997928 kognic-auth-3.1.2/src/kognic/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:01:20.997928 kognic-auth-3.1.2/src/kognic/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-25 14:01:06.000000 kognic-auth-3.1.2/src/kognic/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-25 14:01:20.000000 kognic-auth-3.1.2/src/kognic/auth/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:01:21.001928 kognic-auth-3.1.2/src/kognic/auth/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:01:06.000000 kognic-auth-3.1.2/src/kognic/auth/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-25 14:01:06.000000 kognic-auth-3.1.2/src/kognic/auth/base/auth_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-04-25 14:01:06.000000 kognic-auth-3.1.2/src/kognic/auth/credentials_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:01:21.001928 kognic-auth-3.1.2/src/kognic/auth/httpx/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:01:06.000000 kognic-auth-3.1.2/src/kognic/auth/httpx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-04-25 14:01:06.000000 kognic-auth-3.1.2/src/kognic/auth/httpx/async_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:01:21.001928 kognic-auth-3.1.2/src/kognic/auth/requests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:01:06.000000 kognic-auth-3.1.2/src/kognic/auth/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-04-25 14:01:06.000000 kognic-auth-3.1.2/src/kognic/auth/requests/auth_session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:01:21.001928 kognic-auth-3.1.2/src/kognic_auth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-04-25 14:01:20.000000 kognic-auth-3.1.2/src/kognic_auth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-25 14:01:20.000000 kognic-auth-3.1.2/src/kognic_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 14:01:20.000000 kognic-auth-3.1.2/src/kognic_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-25 14:01:20.000000 kognic-auth-3.1.2/src/kognic_auth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-25 14:01:20.000000 kognic-auth-3.1.2/src/kognic_auth.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:01:21.001928 kognic-auth-3.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-25 14:01:06.000000 kognic-auth-3.1.2/tests/credentials_parser_tests.py
```

### Comparing `kognic-auth-3.1.1/.github/workflows/python-package.yml` & `kognic-auth-3.1.2/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `kognic-auth-3.1.1/.github/workflows/python-publish.yml` & `kognic-auth-3.1.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `kognic-auth-3.1.1/PKG-INFO` & `kognic-auth-3.1.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kognic-auth
-Version: 3.1.1
+Version: 3.1.2
 Summary: Kognic Authentication
 Author-email: Kognic <michel.edkrantz@kognic.com>
 License: MIT
 Project-URL: homepage, https://github.com/annotell/kognic-auth-python
 Keywords: Kognic,API
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -44,37 +44,8 @@
 sess = RequestsAuthSession()
 
 # make call to some Kognic service with your token. Use default requests 
 sess.get("https://api.app.kognic.com")
 ```
 
 ## Changelog
-
-### 3.0.2 (2022-12-07)
-- Support read credentials from dict
-
-### 3.0.0 (2022-09-26)
-- Rebranded from Annotell to Kognic. 
-- Dropped deprecated `FaultTolerantAuthRequestSession`
-
-### 2.0.0 (2022-05-02)
-Refactor for backend separation, with optional dependencies for either `httpx` or `requests`. 
-
-### 1.8.0 (2022-04-12)
-- Initial support for httpx (BETA). Solves refresh token expiry by reset without the `FaultTolerantAuthRequestSession`  
-- The library will be refactored by a breaking 2.0 release, and make the same changes to the requests version. 
-The `authsession` module backed by `requests` is untouched for now.   
-
-### 1.7.0 (2022-04-11)
-- Fix compatibility issue with authlib >= 1.0.0. Resetting the auth session failed, when the refresh token had expired.   
-
-### 1.6.0 (2021-02-21)
-- Expose underlying `requests.Session` on `FaultTolerantAuthRequestSession`
-- Fix some thread locks
-
-### 1.5.0 (2020-10-20)
-- Add `FaultTolerantAuthRequestSession` that handles token refresh on long running sessions. 
-
-### 1.4.0 (2020-04-16)
-- Add support for `auth` parameter, with path to credentials file or `AnnotellCredentials` object
-- Drop support for legacy API token
-
+See Github releases from v3.1.0, historic changelog is available in CHANGELOG.md
```

### Comparing `kognic-auth-3.1.1/README.md` & `kognic-auth-3.1.2/src/kognic_auth.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: kognic-auth
+Version: 3.1.2
+Summary: Kognic Authentication
+Author-email: Kognic <michel.edkrantz@kognic.com>
+License: MIT
+Project-URL: homepage, https://github.com/annotell/kognic-auth-python
+Keywords: Kognic,API
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+Provides-Extra: httpx
+Provides-Extra: requests
+Provides-Extra: full
+
 # Kognic Authentication
 
 Python 3 library providing foundations for Kognic Authentication
 on top of the `requests` or `httpx` libraries.
 
 Install with `pip install kognic-auth[requests]` or `pip install kognic-auth[httpx]` 
 
@@ -26,37 +44,8 @@
 sess = RequestsAuthSession()
 
 # make call to some Kognic service with your token. Use default requests 
 sess.get("https://api.app.kognic.com")
 ```
 
 ## Changelog
-
-### 3.0.2 (2022-12-07)
-- Support read credentials from dict
-
-### 3.0.0 (2022-09-26)
-- Rebranded from Annotell to Kognic. 
-- Dropped deprecated `FaultTolerantAuthRequestSession`
-
-### 2.0.0 (2022-05-02)
-Refactor for backend separation, with optional dependencies for either `httpx` or `requests`. 
-
-### 1.8.0 (2022-04-12)
-- Initial support for httpx (BETA). Solves refresh token expiry by reset without the `FaultTolerantAuthRequestSession`  
-- The library will be refactored by a breaking 2.0 release, and make the same changes to the requests version. 
-The `authsession` module backed by `requests` is untouched for now.   
-
-### 1.7.0 (2022-04-11)
-- Fix compatibility issue with authlib >= 1.0.0. Resetting the auth session failed, when the refresh token had expired.   
-
-### 1.6.0 (2021-02-21)
-- Expose underlying `requests.Session` on `FaultTolerantAuthRequestSession`
-- Fix some thread locks
-
-### 1.5.0 (2020-10-20)
-- Add `FaultTolerantAuthRequestSession` that handles token refresh on long running sessions. 
-
-### 1.4.0 (2020-04-16)
-- Add support for `auth` parameter, with path to credentials file or `AnnotellCredentials` object
-- Drop support for legacy API token
-
+See Github releases from v3.1.0, historic changelog is available in CHANGELOG.md
```

### Comparing `kognic-auth-3.1.1/pyproject.toml` & `kognic-auth-3.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kognic-auth-3.1.1/src/kognic/auth/base/auth_client.py` & `kognic-auth-3.1.2/src/kognic/auth/base/auth_client.py`

 * *Files identical despite different names*

### Comparing `kognic-auth-3.1.1/src/kognic/auth/credentials_parser.py` & `kognic-auth-3.1.2/src/kognic/auth/credentials_parser.py`

 * *Files identical despite different names*

### Comparing `kognic-auth-3.1.1/src/kognic/auth/httpx/async_client.py` & `kognic-auth-3.1.2/src/kognic/auth/httpx/async_client.py`

 * *Files identical despite different names*

### Comparing `kognic-auth-3.1.1/src/kognic/auth/requests/auth_session.py` & `kognic-auth-3.1.2/src/kognic/auth/requests/auth_session.py`

 * *Files identical despite different names*

### Comparing `kognic-auth-3.1.1/src/kognic_auth.egg-info/SOURCES.txt` & `kognic-auth-3.1.2/src/kognic_auth.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 .gitignore
+CHANGELOG.md
 README.md
 pyproject.toml
 .github/dependabot.yml
 .github/workflows/python-package.yml
 .github/workflows/python-publish.yml
 src/kognic/auth/__init__.py
 src/kognic/auth/_version.py
```

### Comparing `kognic-auth-3.1.1/tests/credentials_parser_tests.py` & `kognic-auth-3.1.2/tests/credentials_parser_tests.py`

 * *Files identical despite different names*

