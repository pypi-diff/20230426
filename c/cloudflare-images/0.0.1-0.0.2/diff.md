# Comparing `tmp/cloudflare_images-0.0.1.tar.gz` & `tmp/cloudflare_images-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudflare_images-0.0.1.tar", max compression
+gzip compressed data, was "cloudflare_images-0.0.2.tar", max compression
```

## Comparing `cloudflare_images-0.0.1.tar` & `cloudflare_images-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1491 2023-04-23 21:35:59.824537 cloudflare_images-0.0.1/LICENSE
--rw-r--r--   0        0        0      265 2023-04-23 22:17:07.618439 cloudflare_images-0.0.1/README.md
--rw-r--r--   0        0        0       22 2023-04-23 21:33:09.924925 cloudflare_images-0.0.1/cloudflare_images/__init__.py
--rw-r--r--   0        0        0     7741 2023-04-23 22:07:21.914048 cloudflare_images-0.0.1/cloudflare_images/api.py
--rw-r--r--   0        0        0     2484 2023-04-23 22:06:51.456257 cloudflare_images-0.0.1/cloudflare_images/django.py
--rw-r--r--   0        0        0     1550 2023-04-23 22:20:34.025252 cloudflare_images-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1231 1970-01-01 00:00:00.000000 cloudflare_images-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1491 2023-04-23 21:35:59.824537 cloudflare_images-0.0.2/LICENSE
+-rw-r--r--   0        0        0      265 2023-04-23 22:17:07.618439 cloudflare_images-0.0.2/README.md
+-rw-r--r--   0        0        0      112 2023-04-26 17:25:29.603974 cloudflare_images-0.0.2/cloudflare_images/__init__.py
+-rw-r--r--   0        0        0     7737 2023-04-23 22:59:59.288543 cloudflare_images-0.0.2/cloudflare_images/api.py
+-rw-r--r--   0        0        0     3827 2023-04-26 17:23:10.020196 cloudflare_images-0.0.2/cloudflare_images/django.py
+-rw-r--r--   0        0        0     1572 2023-04-26 17:24:56.870390 cloudflare_images-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1231 1970-01-01 00:00:00.000000 cloudflare_images-0.0.2/PKG-INFO
```

### Comparing `cloudflare_images-0.0.1/LICENSE` & `cloudflare_images-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudflare_images-0.0.1/cloudflare_images/api.py` & `cloudflare_images-0.0.2/cloudflare_images/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,27 +5,27 @@
 
 CF_API_URL: Final = "https://api.cloudflare.com"
 CF_DELIVER: Final = "https://imagedelivery.net"
 
 
 class CloudflareImagesAPIv1(BaseSettings):
     """
-    Need to setup a Cloudflare Images account to use. See Cloudflare Images [docs](https://developers.cloudflare.com/images/cloudflare-images/) API v4.
+    Need to setup a Cloudflare Images account to use. See Cloudflare Images [docs](https://developers.cloudflare.com/images/cloudflare-images/).
     With required variables secured:
 
     Field in .env | Cloudflare API Credential | Where credential found
     :--|:--:|:--
     `CF_IMG_ACCT` | Account ID |  `https://dash.cloudflare.com/<acct_id>/images/images`
     `CF_IMG_HASH` | Account Hash | `https://dash.cloudflare.com/<acct_id>/images/images`
     `CF_IMG_TOKEN` | API Secret | Generate / save via `https://dash.cloudflare.com/<acct_id>/profile/api-tokens`
 
     Add secrets to .env file and use as follows:
 
     Examples:
-    ```py title="Example Usage" linenums="1" hl_lines="5 18"
+    ```py title="Example Usage" linenums="1" hl_lines="4 14 23"
     >>> from pathlib import Path
     >>> import os
     >>> import io
     >>> cf = CloudflareImagesAPIv1() # will error out since missing key values
     Traceback (most recent call last):
     pydantic.error_wrappers.ValidationError: 3 validation errors for CloudflareImagesAPIv1
     acct_id
```

### Comparing `cloudflare_images-0.0.1/pyproject.toml` & `cloudflare_images-0.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "cloudflare-images"
 description = "Wrapper around Cloudflare Images API, usable custom Django storage class."
-version = "0.0.1"
+version = "0.0.2"
 authors = ["Marcelino G. Veloso III <mars@veloso.one>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://mv3.dev"
 repository = "https://github.com/justmars/cloudflare-images"
 documentation = "https://mv3.dev/cloudflare-images"
 classifiers = [
@@ -29,14 +29,15 @@
 pytest = "^7.2"
 pytest-datadir = "^1.4.1"
 pytest-cov = "^2.12.1"
 pre-commit = "^2.21"
 mkdocs = "^1.4.2"
 mkdocstrings = { extras = ["python"], version = "^0.20.0" }
 mkdocs-material = "^9.1"
+ipykernel = "^6.22.0"
 
 [tool.pytest.ini_options]
 minversion = "7.2"
 addopts = "-ra -q --doctest-modules --cov"
 filterwarnings = ["ignore::DeprecationWarning"]
 testpaths = ["tests"]
```

### Comparing `cloudflare_images-0.0.1/PKG-INFO` & `cloudflare_images-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudflare-images
-Version: 0.0.1
+Version: 0.0.2
 Summary: Wrapper around Cloudflare Images API, usable custom Django storage class.
 Home-page: https://mv3.dev
 License: MIT
 Author: Marcelino G. Veloso III
 Author-email: mars@veloso.one
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
```

