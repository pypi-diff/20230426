# Comparing `tmp/layabauth-6.0.0.tar.gz` & `tmp/layabauth-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "layabauth-6.0.0.tar", last modified: Thu Dec  9 23:19:22 2021, max compression
+gzip compressed data, was "layabauth-7.0.0.tar", last modified: Wed Apr 26 15:29:18 2023, max compression
```

## Comparing `layabauth-6.0.0.tar` & `layabauth-7.0.0.tar`

### file list

```diff
@@ -1,20 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-09 23:19:22.031239 layabauth-6.0.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2021-12-09 23:19:07.000000 layabauth-6.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     6427 2021-12-09 23:19:22.031239 layabauth-6.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5095 2021-12-09 23:19:07.000000 layabauth-6.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-09 23:19:22.031239 layabauth-6.0.0/layabauth/
--rw-r--r--   0 runner    (1001) docker     (121)      111 2021-12-09 23:19:07.000000 layabauth-6.0.0/layabauth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      910 2021-12-09 23:19:07.000000 layabauth-6.0.0/layabauth/_http.py
--rw-r--r--   0 runner    (1001) docker     (121)      776 2021-12-09 23:19:07.000000 layabauth-6.0.0/layabauth/_openapi.py
--rw-r--r--   0 runner    (1001) docker     (121)     3143 2021-12-09 23:19:07.000000 layabauth-6.0.0/layabauth/flask.py
--rw-r--r--   0 runner    (1001) docker     (121)     2120 2021-12-09 23:19:07.000000 layabauth-6.0.0/layabauth/starlette.py
--rw-r--r--   0 runner    (1001) docker     (121)      567 2021-12-09 23:19:07.000000 layabauth-6.0.0/layabauth/testing.py
--rw-r--r--   0 runner    (1001) docker     (121)      371 2021-12-09 23:19:07.000000 layabauth-6.0.0/layabauth/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-09 23:19:22.031239 layabauth-6.0.0/layabauth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6427 2021-12-09 23:19:22.000000 layabauth-6.0.0/layabauth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      337 2021-12-09 23:19:22.000000 layabauth-6.0.0/layabauth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-09 23:19:22.000000 layabauth-6.0.0/layabauth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      148 2021-12-09 23:19:22.000000 layabauth-6.0.0/layabauth.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2021-12-09 23:19:22.000000 layabauth-6.0.0/layabauth.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-12-09 23:19:22.031239 layabauth-6.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2356 2021-12-09 23:19:07.000000 layabauth-6.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:29:18.572916 layabauth-7.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-26 15:28:55.000000 layabauth-7.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7377 2023-04-26 15:29:18.572916 layabauth-7.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5095 2023-04-26 15:28:55.000000 layabauth-7.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:29:18.572916 layabauth-7.0.0/layabauth/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-26 15:28:55.000000 layabauth-7.0.0/layabauth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-26 15:28:55.000000 layabauth-7.0.0/layabauth/_http.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-26 15:28:55.000000 layabauth-7.0.0/layabauth/_openapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-04-26 15:28:55.000000 layabauth-7.0.0/layabauth/flask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-04-26 15:28:55.000000 layabauth-7.0.0/layabauth/starlette.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-26 15:28:55.000000 layabauth-7.0.0/layabauth/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-26 15:28:55.000000 layabauth-7.0.0/layabauth/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:29:18.572916 layabauth-7.0.0/layabauth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7377 2023-04-26 15:29:18.000000 layabauth-7.0.0/layabauth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-26 15:29:18.000000 layabauth-7.0.0/layabauth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 15:29:18.000000 layabauth-7.0.0/layabauth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-26 15:29:18.000000 layabauth-7.0.0/layabauth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-26 15:29:18.000000 layabauth-7.0.0/layabauth.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 15:29:18.572916 layabauth-7.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-04-26 15:28:55.000000 layabauth-7.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:29:18.572916 layabauth-7.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    18862 2023-04-26 15:28:55.000000 layabauth-7.0.0/tests/test_flask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-26 15:28:55.000000 layabauth-7.0.0/tests/test_flask_without_expected_scopes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-26 15:28:55.000000 layabauth-7.0.0/tests/test_flask_without_scopes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-26 15:28:55.000000 layabauth-7.0.0/tests/test_openapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11571 2023-04-26 15:28:55.000000 layabauth-7.0.0/tests/test_starlette.py
```

### Comparing `layabauth-6.0.0/LICENSE` & `layabauth-7.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `layabauth-6.0.0/README.md` & `layabauth-7.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -109,12 +109,12 @@
 
 def test_authentication(auth_mock, client):
     response = client.get("/my_endpoint", headers={"Authentication": "Bearer mocked_token"})
     assert response.text == "TEST@email.com"
 ```
 
 ## How to install
-1. [python 3.6+](https://www.python.org/downloads/) must be installed
+1. [python 3.7+](https://www.python.org/downloads/) must be installed
 2. Use pip to install module:
 ```sh
 python -m pip install layabauth
 ```
```

### Comparing `layabauth-6.0.0/layabauth/_http.py` & `layabauth-7.0.0/layabauth/_http.py`

 * *Files identical despite different names*

### Comparing `layabauth-6.0.0/layabauth/_openapi.py` & `layabauth-7.0.0/layabauth/_openapi.py`

 * *Files identical despite different names*

### Comparing `layabauth-6.0.0/layabauth/flask.py` & `layabauth-7.0.0/layabauth/flask.py`

 * *Files identical despite different names*

### Comparing `layabauth-6.0.0/layabauth/starlette.py` & `layabauth-7.0.0/layabauth/starlette.py`

 * *Files identical despite different names*

### Comparing `layabauth-6.0.0/layabauth/testing.py` & `layabauth-7.0.0/layabauth/testing.py`

 * *Files identical despite different names*

### Comparing `layabauth-6.0.0/setup.py` & `layabauth-7.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,44 +23,44 @@
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Software Development :: Build Tools",
     ],
     keywords=["flask", "starlette", "auth"],
     packages=find_packages(exclude=["tests*"]),
     install_requires=[
         # Used to request JWKs (keys)
-        "httpx==0.21.*",
+        "httpx==0.24.*",
         # Used to manage authentication
         "python-jose==3.*",
     ],
     extras_require={
         "testing": [
             # Used to test flask application
-            "flask_restx==0.5.*",
+            "flask_restx==1.1.*",
             "pytest-flask==1.*",
             # Used to test starlette authentication
             "starlette==0.17.*",
             "requests==2.*",
             # Used to mock requests sent to check keys
-            "pytest-httpx==0.15.*",
+            "pytest-httpx==0.22.*",
             # Used to check coverage
             "pytest-cov==3.*",
         ]
     },
-    python_requires=">=3.6",
+    python_requires=">=3.7",
     project_urls={
         "GitHub": "https://github.com/Colin-b/layabauth",
         "Changelog": "https://github.com/Colin-b/layabauth/blob/master/CHANGELOG.md",
         "Issues": "https://github.com/Colin-b/layabauth/issues",
     },
     platforms=["Windows", "Linux"],
 )
```

