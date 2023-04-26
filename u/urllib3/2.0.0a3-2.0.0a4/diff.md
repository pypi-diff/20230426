# Comparing `tmp/urllib3-2.0.0a3.tar.gz` & `tmp/urllib3-2.0.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Wed Jan 11 12:49:50 2023, max compression
+gzip compressed data, last modified: Tue Apr 25 18:20:53 2023, max compression
```

## Comparing `urllib3-2.0.0a3.tar` & `urllib3-2.0.0a4.tar`

### file list

```diff
@@ -1,119 +1,119 @@
--rw-r--r--   0        0        0    58003 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/CHANGES.rst
--rw-r--r--   0        0        0      309 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/dev-requirements.txt
--rw-r--r--   0        0        0     4602 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/docs/Makefile
--rw-r--r--   0        0        0    21364 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/docs/advanced-usage.rst
--rw-r--r--   0        0        0       59 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/docs/changelog.rst
--rw-r--r--   0        0        0     3795 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/docs/conf.py
--rw-r--r--   0        0        0     9500 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/docs/contributing.rst
--rw-r--r--   0        0        0     3836 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/docs/index.rst
--rw-r--r--   0        0        0     4513 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/docs/make.bat
--rw-r--r--   0        0        0       72 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/docs/requirements.txt
--rw-r--r--   0        0        0     3098 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/docs/sponsors.rst
--rw-r--r--   0        0        0    16385 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/docs/user-guide.rst
--rw-r--r--   0        0        0    12495 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/docs/v2-migration-guide.rst
--rw-r--r--   0        0        0     1770 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/docs/_static/banner.svg
--rw-r--r--   0        0        0     3999 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/docs/_static/banner_github.svg
--rw-r--r--   0        0        0     1818 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/docs/_static/dark-logo.svg
--rw-r--r--   0        0        0     7872 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/docs/images/demo-button.png
--rw-r--r--   0        0        0      714 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/docs/images/favicon.png
--rw-r--r--   0        0        0     6226 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/docs/images/learn-more-button.png
--rw-r--r--   0        0        0     2165 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/docs/images/logo.png
--rw-r--r--   0        0        0      516 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/docs/images/logo.svg
--rw-r--r--   0        0        0      226 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/docs/reference/index.rst
--rw-r--r--   0        0        0      316 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/docs/reference/urllib3.connection.rst
--rw-r--r--   0        0        0      408 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/docs/reference/urllib3.connectionpool.rst
--rw-r--r--   0        0        0      185 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/docs/reference/urllib3.exceptions.rst
--rw-r--r--   0        0        0      350 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/docs/reference/urllib3.fields.rst
--rw-r--r--   0        0        0      338 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/docs/reference/urllib3.poolmanager.rst
--rw-r--r--   0        0        0       71 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/docs/reference/urllib3.request.rst
--rw-r--r--   0        0        0      788 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/docs/reference/urllib3.response.rst
--rw-r--r--   0        0        0      555 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/docs/reference/urllib3.util.rst
--rw-r--r--   0        0        0      233 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/docs/reference/contrib/index.rst
--rw-r--r--   0        0        0      295 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/docs/reference/contrib/pyopenssl.rst
--rw-r--r--   0        0        0     1431 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/docs/reference/contrib/securetransport.rst
--rw-r--r--   0        0        0      124 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/docs/reference/contrib/socks.rst
--rw-r--r--   0        0        0        0 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/dummyserver/__init__.py
--rw-r--r--   0        0        0    13109 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/dummyserver/handlers.py
--rwxr-xr-x   0        0        0     1198 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/dummyserver/https_proxy.py
--rwxr-xr-x   0        0        0     5420 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/dummyserver/proxy.py
--rwxr-xr-x   0        0        0     9011 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/dummyserver/server.py
--rw-r--r--   0        0        0    11172 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/dummyserver/testcase.py
--rw-r--r--   0        0        0      511 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/dummyserver/certs/README.rst
--rw-r--r--   0        0        0     1679 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/dummyserver/certs/cacert.key
--rw-r--r--   0        0        0     1273 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/dummyserver/certs/cacert.pem
--rw-r--r--   0        0        0     1265 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/dummyserver/certs/server.crt
--rw-r--r--   0        0        0     1679 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/dummyserver/certs/server.key
--rw-r--r--   0        0        0     5028 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/src/urllib3/__init__.py
--rw-r--r--   0        0        0     5651 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/src/urllib3/_base_connection.py
--rw-r--r--   0        0        0    15562 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/src/urllib3/_collections.py
--rw-r--r--   0        0        0     7756 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/src/urllib3/_request_methods.py
--rw-r--r--   0        0        0      100 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/src/urllib3/_version.py
--rw-r--r--   0        0        0    33301 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/src/urllib3/connection.py
--rw-r--r--   0        0        0    42963 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/src/urllib3/connectionpool.py
--rw-r--r--   0        0        0     9289 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/src/urllib3/exceptions.py
--rw-r--r--   0        0        0    11026 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/src/urllib3/fields.py
--rw-r--r--   0        0        0     2395 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/src/urllib3/filepost.py
--rw-r--r--   0        0        0    22161 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/src/urllib3/poolmanager.py
--rw-r--r--   0        0        0       93 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/src/urllib3/py.typed
--rw-r--r--   0        0        0    39726 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/src/urllib3/response.py
--rw-r--r--   0        0        0        0 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/src/urllib3/contrib/__init__.py
--rw-r--r--   0        0        0    19438 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/src/urllib3/contrib/pyopenssl.py
--rw-r--r--   0        0        0    34060 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/src/urllib3/contrib/securetransport.py
--rw-r--r--   0        0        0     7715 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/src/urllib3/contrib/socks.py
--rw-r--r--   0        0        0        0 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/src/urllib3/contrib/_securetransport/__init__.py
--rw-r--r--   0        0        0    14452 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/src/urllib3/contrib/_securetransport/bindings.py
--rw-r--r--   0        0        0    16220 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/src/urllib3/contrib/_securetransport/low_level.py
--rw-r--r--   0        0        0     1051 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/src/urllib3/util/__init__.py
--rw-r--r--   0        0        0     4462 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/src/urllib3/util/connection.py
--rw-r--r--   0        0        0     1148 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/src/urllib3/util/proxy.py
--rw-r--r--   0        0        0     8111 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/src/urllib3/util/request.py
--rw-r--r--   0        0        0     3374 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/src/urllib3/util/response.py
--rw-r--r--   0        0        0    17956 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/src/urllib3/util/retry.py
--rw-r--r--   0        0        0    18540 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/src/urllib3/util/ssl_.py
--rw-r--r--   0        0        0     5812 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/src/urllib3/util/ssl_match_hostname.py
--rw-r--r--   0        0        0     9046 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/src/urllib3/util/ssltransport.py
--rw-r--r--   0        0        0    10529 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/src/urllib3/util/timeout.py
--rw-r--r--   0        0        0    15246 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/src/urllib3/util/url.py
--rw-r--r--   0        0        0     1146 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/src/urllib3/util/util.py
--rw-r--r--   0        0        0     4423 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/src/urllib3/util/wait.py
--rw-r--r--   0        0        0    10748 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/test/__init__.py
--rw-r--r--   0        0        0    10925 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/test/conftest.py
--rw-r--r--   0        0        0     6222 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/test/port_helpers.py
--rw-r--r--   0        0        0    13035 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/test/test_collections.py
--rw-r--r--   0        0        0      692 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/test/test_compatibility.py
--rw-r--r--   0        0        0     9364 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/test/test_connection.py
--rw-r--r--   0        0        0    22772 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/test/test_connectionpool.py
--rw-r--r--   0        0        0     2153 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/test/test_exceptions.py
--rw-r--r--   0        0        0     4438 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/test/test_fields.py
--rw-r--r--   0        0        0     3751 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/test/test_filepost.py
--rw-r--r--   0        0        0      978 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/test/test_no_ssl.py
--rw-r--r--   0        0        0    17765 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/test/test_poolmanager.py
--rw-r--r--   0        0        0     3657 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/test/test_proxymanager.py
--rw-r--r--   0        0        0      761 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/test/test_queue_monkeypatch.py
--rw-r--r--   0        0        0    44434 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/test/test_response.py
--rw-r--r--   0        0        0    15531 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/test/test_retry.py
--rw-r--r--   0        0        0     6794 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/test/test_ssl.py
--rw-r--r--   0        0        0    20535 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/test/test_ssltransport.py
--rw-r--r--   0        0        0    43234 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/test/test_util.py
--rw-r--r--   0        0        0     5890 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/test/test_wait.py
--rw-r--r--   0        0        0     1211 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/test/tz_stub.py
--rw-r--r--   0        0        0        0 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/test/contrib/__init__.py
--rw-r--r--   0        0        0     1257 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/test/contrib/duplicate_san.pem
--rw-r--r--   0        0        0     3007 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/test/contrib/test_pyopenssl.py
--rw-r--r--   0        0        0     1988 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/test/contrib/test_pyopenssl_dependencies.py
--rw-r--r--   0        0        0     1690 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/test/contrib/test_securetransport.py
--rw-r--r--   0        0        0    25908 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/test/contrib/test_socks.py
--rw-r--r--   0        0        0        0 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/test/with_dummyserver/__init__.py
--rw-r--r--   0        0        0    10678 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/test/with_dummyserver/test_chunked_transfer.py
--rw-r--r--   0        0        0     3827 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/test/with_dummyserver/test_connection.py
--rw-r--r--   0        0        0    56861 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/test/with_dummyserver/test_connectionpool.py
--rw-r--r--   0        0        0    42323 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/test/with_dummyserver/test_https.py
--rw-r--r--   0        0        0      964 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/test/with_dummyserver/test_no_ssl.py
--rw-r--r--   0        0        0    22082 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/test/with_dummyserver/test_poolmanager.py
--rw-r--r--   0        0        0    33338 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/test/with_dummyserver/test_proxy_poolmanager.py
--rw-r--r--   0        0        0    81730 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/test/with_dummyserver/test_socketlevel.py
--rw-r--r--   0        0        0       85 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/.gitignore
--rw-r--r--   0        0        0     1115 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/LICENSE.txt
--rw-r--r--   0        0        0     4393 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/README.md
--rw-r--r--   0        0        0     4505 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/pyproject.toml
--rw-r--r--   0        0        0     6572 2023-01-11 12:49:50.000000 urllib3-2.0.0a3/PKG-INFO
+-rw-r--r--   0        0        0    59335 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/CHANGES.rst
+-rw-r--r--   0        0        0      328 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/dev-requirements.txt
+-rw-r--r--   0        0        0     4602 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/docs/Makefile
+-rw-r--r--   0        0        0    21359 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/docs/advanced-usage.rst
+-rw-r--r--   0        0        0       59 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/docs/changelog.rst
+-rw-r--r--   0        0        0     3795 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/docs/conf.py
+-rw-r--r--   0        0        0     9500 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/docs/contributing.rst
+-rw-r--r--   0        0        0     3836 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/docs/index.rst
+-rw-r--r--   0        0        0     4513 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/docs/make.bat
+-rw-r--r--   0        0        0       72 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/docs/requirements.txt
+-rw-r--r--   0        0        0     3098 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/docs/sponsors.rst
+-rw-r--r--   0        0        0    16385 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/docs/user-guide.rst
+-rw-r--r--   0        0        0    12502 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/docs/v2-migration-guide.rst
+-rw-r--r--   0        0        0     1770 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/docs/_static/banner.svg
+-rw-r--r--   0        0        0     3999 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/docs/_static/banner_github.svg
+-rw-r--r--   0        0        0     1818 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/docs/_static/dark-logo.svg
+-rw-r--r--   0        0        0     7872 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/docs/images/demo-button.png
+-rw-r--r--   0        0        0      714 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/docs/images/favicon.png
+-rw-r--r--   0        0        0     6226 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/docs/images/learn-more-button.png
+-rw-r--r--   0        0        0     2165 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/docs/images/logo.png
+-rw-r--r--   0        0        0      516 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/docs/images/logo.svg
+-rw-r--r--   0        0        0      226 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/docs/reference/index.rst
+-rw-r--r--   0        0        0      316 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/docs/reference/urllib3.connection.rst
+-rw-r--r--   0        0        0      408 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/docs/reference/urllib3.connectionpool.rst
+-rw-r--r--   0        0        0      185 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/docs/reference/urllib3.exceptions.rst
+-rw-r--r--   0        0        0      350 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/docs/reference/urllib3.fields.rst
+-rw-r--r--   0        0        0      338 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/docs/reference/urllib3.poolmanager.rst
+-rw-r--r--   0        0        0       71 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/docs/reference/urllib3.request.rst
+-rw-r--r--   0        0        0      788 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/docs/reference/urllib3.response.rst
+-rw-r--r--   0        0        0      555 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/docs/reference/urllib3.util.rst
+-rw-r--r--   0        0        0      233 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/docs/reference/contrib/index.rst
+-rw-r--r--   0        0        0      295 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/docs/reference/contrib/pyopenssl.rst
+-rw-r--r--   0        0        0     1431 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/docs/reference/contrib/securetransport.rst
+-rw-r--r--   0        0        0      124 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/docs/reference/contrib/socks.rst
+-rw-r--r--   0        0        0        0 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/dummyserver/__init__.py
+-rw-r--r--   0        0        0    13109 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/dummyserver/handlers.py
+-rwxr-xr-x   0        0        0     1198 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/dummyserver/https_proxy.py
+-rwxr-xr-x   0        0        0     5420 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/dummyserver/proxy.py
+-rwxr-xr-x   0        0        0     9839 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/dummyserver/server.py
+-rw-r--r--   0        0        0    11171 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/dummyserver/testcase.py
+-rw-r--r--   0        0        0      511 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/dummyserver/certs/README.rst
+-rw-r--r--   0        0        0     1679 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/dummyserver/certs/cacert.key
+-rw-r--r--   0        0        0     1273 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/dummyserver/certs/cacert.pem
+-rw-r--r--   0        0        0     1265 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/dummyserver/certs/server.crt
+-rw-r--r--   0        0        0     1679 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/dummyserver/certs/server.key
+-rw-r--r--   0        0        0     5028 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/src/urllib3/__init__.py
+-rw-r--r--   0        0        0     5651 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/src/urllib3/_base_connection.py
+-rw-r--r--   0        0        0    15561 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/src/urllib3/_collections.py
+-rw-r--r--   0        0        0     7756 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/src/urllib3/_request_methods.py
+-rw-r--r--   0        0        0      100 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/src/urllib3/_version.py
+-rw-r--r--   0        0        0    33299 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/src/urllib3/connection.py
+-rw-r--r--   0        0        0    42961 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/src/urllib3/connectionpool.py
+-rw-r--r--   0        0        0     9289 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/src/urllib3/exceptions.py
+-rw-r--r--   0        0        0    11026 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/src/urllib3/fields.py
+-rw-r--r--   0        0        0     2395 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/src/urllib3/filepost.py
+-rw-r--r--   0        0        0    22160 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/src/urllib3/poolmanager.py
+-rw-r--r--   0        0        0       93 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/src/urllib3/py.typed
+-rw-r--r--   0        0        0    39725 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/src/urllib3/response.py
+-rw-r--r--   0        0        0        0 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/src/urllib3/contrib/__init__.py
+-rw-r--r--   0        0        0    19437 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/src/urllib3/contrib/pyopenssl.py
+-rw-r--r--   0        0        0    34121 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/src/urllib3/contrib/securetransport.py
+-rw-r--r--   0        0        0     7715 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/src/urllib3/contrib/socks.py
+-rw-r--r--   0        0        0        0 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/src/urllib3/contrib/_securetransport/__init__.py
+-rw-r--r--   0        0        0    14452 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/src/urllib3/contrib/_securetransport/bindings.py
+-rw-r--r--   0        0        0    16220 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/src/urllib3/contrib/_securetransport/low_level.py
+-rw-r--r--   0        0        0     1051 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/src/urllib3/util/__init__.py
+-rw-r--r--   0        0        0     4462 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/src/urllib3/util/connection.py
+-rw-r--r--   0        0        0     1148 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/src/urllib3/util/proxy.py
+-rw-r--r--   0        0        0     8111 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/src/urllib3/util/request.py
+-rw-r--r--   0        0        0     3374 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/src/urllib3/util/response.py
+-rw-r--r--   0        0        0    18375 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/src/urllib3/util/retry.py
+-rw-r--r--   0        0        0    18540 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/src/urllib3/util/ssl_.py
+-rw-r--r--   0        0        0     5812 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/src/urllib3/util/ssl_match_hostname.py
+-rw-r--r--   0        0        0     9045 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/src/urllib3/util/ssltransport.py
+-rw-r--r--   0        0        0    10529 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/src/urllib3/util/timeout.py
+-rw-r--r--   0        0        0    15213 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/src/urllib3/util/url.py
+-rw-r--r--   0        0        0     1146 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/src/urllib3/util/util.py
+-rw-r--r--   0        0        0     4423 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/src/urllib3/util/wait.py
+-rw-r--r--   0        0        0    10763 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/test/__init__.py
+-rw-r--r--   0        0        0    11211 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/test/conftest.py
+-rw-r--r--   0        0        0     6222 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/test/port_helpers.py
+-rw-r--r--   0        0        0    13035 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/test/test_collections.py
+-rw-r--r--   0        0        0      692 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/test/test_compatibility.py
+-rw-r--r--   0        0        0     9484 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/test/test_connection.py
+-rw-r--r--   0        0        0    22772 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/test/test_connectionpool.py
+-rw-r--r--   0        0        0     2164 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/test/test_exceptions.py
+-rw-r--r--   0        0        0     4438 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/test/test_fields.py
+-rw-r--r--   0        0        0     3751 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/test/test_filepost.py
+-rw-r--r--   0        0        0      978 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/test/test_no_ssl.py
+-rw-r--r--   0        0        0    17765 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/test/test_poolmanager.py
+-rw-r--r--   0        0        0     3657 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/test/test_proxymanager.py
+-rw-r--r--   0        0        0      761 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/test/test_queue_monkeypatch.py
+-rw-r--r--   0        0        0    44750 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/test/test_response.py
+-rw-r--r--   0        0        0    16568 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/test/test_retry.py
+-rw-r--r--   0        0        0     7281 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/test/test_ssl.py
+-rw-r--r--   0        0        0    20750 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/test/test_ssltransport.py
+-rw-r--r--   0        0        0    43233 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/test/test_util.py
+-rw-r--r--   0        0        0     5999 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/test/test_wait.py
+-rw-r--r--   0        0        0     1211 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/test/tz_stub.py
+-rw-r--r--   0        0        0        0 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/test/contrib/__init__.py
+-rw-r--r--   0        0        0     1257 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/test/contrib/duplicate_san.pem
+-rw-r--r--   0        0        0     3007 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/test/contrib/test_pyopenssl.py
+-rw-r--r--   0        0        0     1988 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/test/contrib/test_pyopenssl_dependencies.py
+-rw-r--r--   0        0        0     1690 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/test/contrib/test_securetransport.py
+-rw-r--r--   0        0        0    25908 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/test/contrib/test_socks.py
+-rw-r--r--   0        0        0        0 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/test/with_dummyserver/__init__.py
+-rw-r--r--   0        0        0    10678 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/test/with_dummyserver/test_chunked_transfer.py
+-rw-r--r--   0        0        0     3827 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/test/with_dummyserver/test_connection.py
+-rw-r--r--   0        0        0    56860 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/test/with_dummyserver/test_connectionpool.py
+-rw-r--r--   0        0        0    43583 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/test/with_dummyserver/test_https.py
+-rw-r--r--   0        0        0     1104 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/test/with_dummyserver/test_no_ssl.py
+-rw-r--r--   0        0        0    22082 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/test/with_dummyserver/test_poolmanager.py
+-rw-r--r--   0        0        0    33489 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/test/with_dummyserver/test_proxy_poolmanager.py
+-rw-r--r--   0        0        0    84327 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/test/with_dummyserver/test_socketlevel.py
+-rw-r--r--   0        0        0       85 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/.gitignore
+-rw-r--r--   0        0        0     1115 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/LICENSE.txt
+-rw-r--r--   0        0        0     4393 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/README.md
+-rw-r--r--   0        0        0     4025 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/pyproject.toml
+-rw-r--r--   0        0        0     6572 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/PKG-INFO
```

### Comparing `urllib3-2.0.0a3/CHANGES.rst` & `urllib3-2.0.0a4/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,20 @@
-2.0.0a3 (2023-01-11)
+2.0.0a4 (2023-04-24)
 ====================
 
-Bugfixes
---------
+- Removed the ``setup.py`` shim, ``python setup.py install`` will print ``[Errno 2] No such file or directory`` instead of a warning to use pip (`#2975 <https://github.com/urllib3/urllib3/issues/2975>`__)
+- Added optional ``backoff_jitter`` parameter to ``Retry``. (`#2952 <https://github.com/urllib3/urllib3/issues/2952>`__)
+- Fixed URL encoding by removing '!' from the 'unreserved' character set specified in RFC 3986. (`#2899 <https://github.com/urllib3/urllib3/issues/2899>`__)
+- Fixed a sign error in a check for whether a character is in the ASCII range. (`#2901 <https://github.com/urllib3/urllib3/issues/2901>`__)
+- Fixed ``urllib3.contrib.pyopenssl.WrappedSocket`` and ``urllib3.contrib.securetransport.WrappedSocket`` close methods (`#2970 <https://github.com/urllib3/urllib3/issues/2970>`__)
 
-- Fix logging error when using ``add_stderr_logger``. (`#2839 <https://github.com/urllib3/urllib3/issues/2839>`__)
-- Fixed parsing of port 0 (zero) returning None, instead of 0. (`#2850 <https://github.com/urllib3/urllib3/issues/2850>`__)
-- Fixed the type hint of ``PoolKey.key_retries`` by adding ``bool`` to the union. (`#2865 <https://github.com/urllib3/urllib3/issues/2865>`__)
+2.0.0a3 (2023-01-11)
+====================
 
+* Fix logging error when using ``add_stderr_logger``. (`#2839 <https://github.com/urllib3/urllib3/issues/2839>`__)
 
 2.0.0a2 (2022-11-23)
 ====================
 
 Read the `v2.0 migration guide <https://urllib3.readthedocs.io/en/latest/v2-migration-guide.html>`__ for help upgrading to the latest version of urllib3.
 
 * Changed ``HTTPResponse.read()`` to raise an error when calling with ``decode_content=False`` after using ``decode_content=True`` to prevent data loss (`#2800 <https://github.com/urllib3/urllib3/issues/2800>`__).
@@ -124,14 +127,28 @@
   Instead now if ``HTTPConnection.timeout`` is updated before sending the next request the new timeout value will be used (`#2645 <https://github.com/urllib3/urllib3/issues/2645>`__).
 * Fixed ``socket.error.errno`` when raised from pyOpenSSL's ``OpenSSL.SSL.SysCallError`` (`#2118 <https://github.com/urllib3/urllib3/issues/2118>`__).
 * Fixed the default value of ``HTTPSConnection.socket_options`` to match ``HTTPConnection`` (`#2213 <https://github.com/urllib3/urllib3/issues/2213>`__).
 * Fixed a bug where ``headers`` would be modified by the ``remove_headers_on_redirect`` feature (`#2272 <https://github.com/urllib3/urllib3/issues/2272>`__).
 * Fixed a reference cycle bug in ``urllib3.util.connection.create_connection()`` (`#2277 <https://github.com/urllib3/urllib3/issues/2277>`__).
 * Fixed a socket leak if ``HTTPConnection.connect()`` fails (`#2571 <https://github.com/urllib3/urllib3/pull/2571>`__).
 
+1.26.15 (2023-03-10)
+--------------------
+
+* Fix socket timeout value when ``HTTPConnection`` is reused (`#2645 <https://github.com/urllib3/urllib3/issues/2645>`__)
+* Remove "!" character from the unreserved characters in IPv6 Zone ID parsing
+  (`#2899 <https://github.com/urllib3/urllib3/issues/2899>`__)
+* Fix IDNA handling of '\x80' byte (`#2901 <https://github.com/urllib3/urllib3/issues/2901>`__)
+
+1.26.14 (2023-01-11)
+--------------------
+
+* Fixed parsing of port 0 (zero) returning None, instead of 0. (`#2850 <https://github.com/urllib3/urllib3/issues/2850>`__)
+* Removed deprecated getheaders() calls in contrib module. Fixed the type hint of ``PoolKey.key_retries`` by adding ``bool`` to the union. (`#2865 <https://github.com/urllib3/urllib3/issues/2865>`__)
+
 1.26.13 (2022-11-23)
 --------------------
 
 * Deprecated the ``HTTPResponse.getheaders()`` and ``HTTPResponse.getheader()`` methods.
 * Fixed an issue where parsing a URL with leading zeroes in the port would be rejected
   even when the port number after removing the zeroes was valid.
 * Fixed a deprecation warning when using cryptography v39.0.0.
```

### Comparing `urllib3-2.0.0a3/docs/Makefile` & `urllib3-2.0.0a4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a3/docs/advanced-usage.rst` & `urllib3-2.0.0a4/docs/advanced-usage.rst`

 * *Files 1% similar despite different names*

```diff
@@ -615,15 +615,15 @@
 flag that isn't set by default, and then makes a HTTPS request:
 
 .. code-block:: python
 
     import ssl
 
     from urllib3 import PoolManager
-    from urllib3.util.ssl_ import create_urllib3_context
+    from urllib3.util import create_urllib3_context
 
     ctx = create_urllib3_context()
     ctx.load_default_certs()
     ctx.options |= ssl.OP_ENABLE_MIDDLEBOX_COMPAT
 
     with PoolManager(ssl_context=ctx) as pool:
         pool.request("GET", "https://www.google.com/")
```

### Comparing `urllib3-2.0.0a3/docs/conf.py` & `urllib3-2.0.0a4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a3/docs/contributing.rst` & `urllib3-2.0.0a4/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a3/docs/index.rst` & `urllib3-2.0.0a4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a3/docs/make.bat` & `urllib3-2.0.0a4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a3/docs/sponsors.rst` & `urllib3-2.0.0a4/docs/sponsors.rst`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a3/docs/user-guide.rst` & `urllib3-2.0.0a4/docs/user-guide.rst`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a3/docs/v2-migration-guide.rst` & `urllib3-2.0.0a4/docs/v2-migration-guide.rst`

 * *Files 2% similar despite different names*

```diff
@@ -85,15 +85,15 @@
     "urllib3>=1.26,<3"
   ]
 
 Next you should try installing urllib3 v2.0 locally and run your test suite.
 
 .. code-block:: bash
 
-  $ python -m pip install -U --pre 'urllib3>2'
+  $ python -m pip install -U --pre 'urllib3>=2.0.0a1'
 
 
 Because there are many ``DeprecationWarnings`` you should ensure that you're
 able to see those warnings when running your test suite. To do so you can add
 the following to your test setup to ensure even ``DeprecationWarnings`` are
 output to the terminal:
```

### Comparing `urllib3-2.0.0a3/docs/_static/banner.svg` & `urllib3-2.0.0a4/docs/_static/banner.svg`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a3/docs/_static/banner_github.svg` & `urllib3-2.0.0a4/docs/_static/banner_github.svg`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a3/docs/_static/dark-logo.svg` & `urllib3-2.0.0a4/docs/_static/dark-logo.svg`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a3/docs/images/demo-button.png` & `urllib3-2.0.0a4/docs/images/demo-button.png`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a3/docs/images/favicon.png` & `urllib3-2.0.0a4/docs/images/favicon.png`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a3/docs/images/learn-more-button.png` & `urllib3-2.0.0a4/docs/images/learn-more-button.png`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a3/docs/images/logo.png` & `urllib3-2.0.0a4/docs/images/logo.png`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a3/docs/images/logo.svg` & `urllib3-2.0.0a4/docs/images/logo.svg`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a3/docs/reference/urllib3.response.rst` & `urllib3-2.0.0a4/docs/reference/urllib3.response.rst`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a3/docs/reference/urllib3.util.rst` & `urllib3-2.0.0a4/docs/reference/urllib3.util.rst`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a3/docs/reference/contrib/securetransport.rst` & `urllib3-2.0.0a4/docs/reference/contrib/securetransport.rst`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a3/dummyserver/handlers.py` & `urllib3-2.0.0a4/dummyserver/handlers.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a3/dummyserver/https_proxy.py` & `urllib3-2.0.0a4/dummyserver/https_proxy.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a3/dummyserver/proxy.py` & `urllib3-2.0.0a4/dummyserver/proxy.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a3/dummyserver/server.py` & `urllib3-2.0.0a4/dummyserver/server.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 """
 
 from __future__ import annotations
 
 import asyncio
 import concurrent.futures
 import contextlib
+import errno
 import logging
 import os
 import socket
 import ssl
 import sys
 import threading
 import typing
@@ -195,15 +196,32 @@
     if scheme == "https":
         assert certs is not None
         ssl_opts = ssl_options_to_context(**certs)
         http_server = tornado.httpserver.HTTPServer(app, ssl_options=ssl_opts)
     else:
         http_server = tornado.httpserver.HTTPServer(app)
 
-    sockets = tornado.netutil.bind_sockets(None, address=host)  # type: ignore[arg-type]
+    # When we request a socket with host localhost and port zero (None in Python), then
+    # Tornado gets a free IPv4 port and requests that same port in IPv6. But that port
+    # could easily be taken with IPv6, especially in crowded CI environments. For this
+    # reason we put bind_sockets in a retry loop. Full details:
+    #  * https://github.com/urllib3/urllib3/issues/2171
+    #  * https://github.com/tornadoweb/tornado/issues/1860
+    for i in range(10):
+        try:
+            sockets = tornado.netutil.bind_sockets(None, address=host)  # type: ignore[arg-type]
+        except OSError as e:
+            if e.errno == errno.EADDRINUSE:
+                # TODO this should be a warning if there's a way for pytest to print it
+                print(
+                    f"Retrying bind_sockets({host}) after EADDRINUSE", file=sys.stderr
+                )
+                continue
+        break
+
     port = sockets[0].getsockname()[1]
     http_server.add_sockets(sockets)
     return http_server, port
 
 
 def get_unreachable_address() -> tuple[str, int]:
     # reserved as per rfc2606
```

### Comparing `urllib3-2.0.0a3/dummyserver/testcase.py` & `urllib3-2.0.0a4/dummyserver/testcase.py`

 * *Files 0% similar despite different names*

```diff
@@ -277,15 +277,14 @@
 @pytest.mark.skipif(not HAS_IPV6, reason="IPv6 not available")
 class IPv6HTTPDummyServerTestCase(HTTPDummyServerTestCase):
     host = "::1"
 
 
 @pytest.mark.skipif(not HAS_IPV6, reason="IPv6 not available")
 class IPv6HTTPDummyProxyTestCase(HTTPDummyProxyTestCase):
-
     http_host = "localhost"
     http_host_alt = "127.0.0.1"
 
     https_host = "localhost"
     https_host_alt = "127.0.0.1"
     https_certs = DEFAULT_CERTS
```

### Comparing `urllib3-2.0.0a3/dummyserver/certs/cacert.key` & `urllib3-2.0.0a4/dummyserver/certs/cacert.key`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a3/dummyserver/certs/cacert.pem` & `urllib3-2.0.0a4/dummyserver/certs/cacert.pem`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a3/dummyserver/certs/server.crt` & `urllib3-2.0.0a4/dummyserver/certs/server.crt`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a3/dummyserver/certs/server.key` & `urllib3-2.0.0a4/dummyserver/certs/server.key`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a3/src/urllib3/__init__.py` & `urllib3-2.0.0a4/src/urllib3/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a3/src/urllib3/_base_connection.py` & `urllib3-2.0.0a4/src/urllib3/_base_connection.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a3/src/urllib3/_collections.py` & `urllib3-2.0.0a4/src/urllib3/_collections.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import typing
 from collections import OrderedDict
 from enum import Enum, auto
 from threading import RLock
 
 if typing.TYPE_CHECKING:
-
     # We can only import Protocol if TYPE_CHECKING because it's a development
     # dependency, and is not available at runtime.
     from typing_extensions import Protocol
 
     class HasGettableStringKeys(Protocol):
         def keys(self) -> typing.Iterator[str]:
             ...
```

### Comparing `urllib3-2.0.0a3/src/urllib3/_request_methods.py` & `urllib3-2.0.0a4/src/urllib3/_request_methods.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a3/src/urllib3/connection.py` & `urllib3-2.0.0a4/src/urllib3/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -317,15 +317,14 @@
         headers: typing.Mapping[str, str] | None = None,
         *,
         chunked: bool = False,
         preload_content: bool = True,
         decode_content: bool = True,
         enforce_content_length: bool = True,
     ) -> None:
-
         # Update the inner socket's timeout value to send the request.
         # This only triggers if the connection is re-used.
         if self.sock is not None:
             self.sock.settimeout(self.timeout)
 
         # Store these values to be fed into the HTTPResponse
         # object later. TODO: Remove this in favor of a real
@@ -522,15 +521,14 @@
         ssl_minimum_version: int | None = None,
         ssl_maximum_version: int | None = None,
         ssl_version: int | str | None = None,  # Deprecated
         cert_file: str | None = None,
         key_file: str | None = None,
         key_password: str | None = None,
     ) -> None:
-
         super().__init__(
             host,
             port=port,
             timeout=timeout,
             source_address=source_address,
             blocksize=blocksize,
             socket_options=socket_options,
```

### Comparing `urllib3-2.0.0a3/src/urllib3/connectionpool.py` & `urllib3-2.0.0a4/src/urllib3/connectionpool.py`

 * *Files 0% similar despite different names*

```diff
@@ -312,15 +312,14 @@
             try:
                 self.pool.put(conn, block=False)
                 return  # Everything is dandy, done.
             except AttributeError:
                 # self.pool is None.
                 pass
             except queue.Full:
-
                 # Connection never got put back into the pool, close it.
                 if conn:
                     conn.close()
 
                 if self.block:
                     # This should never happen if you got the conn from self._get_conn
                     raise FullPoolError(
@@ -997,15 +996,14 @@
         ssl_minimum_version: ssl.TLSVersion | None = None,
         ssl_maximum_version: ssl.TLSVersion | None = None,
         assert_hostname: str | Literal[False] | None = None,
         assert_fingerprint: str | None = None,
         ca_cert_dir: str | None = None,
         **conn_kw: typing.Any,
     ) -> None:
-
         super().__init__(
             host,
             port,
             timeout,
             maxsize,
             block,
             headers,
```

### Comparing `urllib3-2.0.0a3/src/urllib3/exceptions.py` & `urllib3-2.0.0a4/src/urllib3/exceptions.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a3/src/urllib3/fields.py` & `urllib3-2.0.0a4/src/urllib3/fields.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a3/src/urllib3/filepost.py` & `urllib3-2.0.0a4/src/urllib3/filepost.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a3/src/urllib3/poolmanager.py` & `urllib3-2.0.0a4/src/urllib3/poolmanager.py`

 * *Files 0% similar despite different names*

```diff
@@ -539,15 +539,14 @@
         proxy_headers: typing.Mapping[str, str] | None = None,
         proxy_ssl_context: ssl.SSLContext | None = None,
         use_forwarding_for_https: bool = False,
         proxy_assert_hostname: None | str | Literal[False] = None,
         proxy_assert_fingerprint: str | None = None,
         **connection_pool_kw: typing.Any,
     ) -> None:
-
         if isinstance(proxy_url, HTTPConnectionPool):
             str_proxy_url = f"{proxy_url.scheme}://{proxy_url.host}:{proxy_url.port}"
         else:
             str_proxy_url = proxy_url
         proxy = parse_url(str_proxy_url)
 
         if proxy.scheme not in ("http", "https"):
```

### Comparing `urllib3-2.0.0a3/src/urllib3/response.py` & `urllib3-2.0.0a4/src/urllib3/response.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,14 @@
                 self._data = None  # type: ignore[assignment]
 
     def flush(self) -> bytes:
         return self._obj.flush()
 
 
 class GzipDecoderState:
-
     FIRST_MEMBER = 0
     OTHER_MEMBERS = 1
     SWALLOW_DATA = 2
 
 
 class GzipDecoder(ContentDecoder):
     def __init__(self) -> None:
```

### Comparing `urllib3-2.0.0a3/src/urllib3/contrib/pyopenssl.py` & `urllib3-2.0.0a4/src/urllib3/contrib/pyopenssl.py`

 * *Files 1% similar despite different names*

```diff
@@ -376,22 +376,23 @@
             total_sent += sent
 
     def shutdown(self) -> None:
         # FIXME rethrow compatible exceptions should we ever use this
         self.connection.shutdown()
 
     def close(self) -> None:
-        if self._io_refs < 1:
-            try:
-                self._closed = True
-                return self.connection.close()  # type: ignore[no-any-return]
-            except OpenSSL.SSL.Error:
-                return
-        else:
-            self._io_refs -= 1
+        self._closed = True
+        if self._io_refs <= 0:
+            self._real_close()
+
+    def _real_close(self) -> None:
+        try:
+            return self.connection.close()  # type: ignore[no-any-return]
+        except OpenSSL.SSL.Error:
+            return
 
     def getpeercert(
         self, binary_form: bool = False
     ) -> dict[str, list[typing.Any]] | None:
         x509 = self.connection.get_peer_certificate()
 
         if not x509:
```

### Comparing `urllib3-2.0.0a3/src/urllib3/contrib/securetransport.py` & `urllib3-2.0.0a4/src/urllib3/contrib/securetransport.py`

 * *Files 1% similar despite different names*

```diff
@@ -313,14 +313,15 @@
     """
 
     def __init__(self, socket: socket_cls) -> None:
         self.socket = socket
         self.context = None
         self._io_refs = 0
         self._closed = False
+        self._real_closed = False
         self._exception: Exception | None = None
         self._keychain = None
         self._keychain_dir: str | None = None
         self._client_cert_chain = None
 
         # We save off the previously-configured timeout and then set it to
         # zero. This is done because we use select and friends to handle the
@@ -344,15 +345,15 @@
 
         # We explicitly don't catch around this yield because in the unlikely
         # event that an exception was hit in the block we don't want to swallow
         # it.
         yield
         if self._exception is not None:
             exception, self._exception = self._exception, None
-            self.close()
+            self._real_close()
             raise exception
 
     def _set_alpn_protocols(self, protocols: list[bytes] | None) -> None:
         """
         Sets up the ALPN protocols on the context.
         """
         if not protocols:
@@ -394,15 +395,15 @@
         rec = _build_tls_unknown_ca_alert(self.version())
         self.socket.sendall(rec)
         # close the connection immediately
         # l_onoff = 1, activate linger
         # l_linger = 0, linger for 0 seoncds
         opts = struct.pack("ii", 1, 0)
         self.socket.setsockopt(socket.SOL_SOCKET, socket.SO_LINGER, opts)
-        self.close()
+        self._real_close()
         raise ssl.SSLError(f"certificate verify failed, {reason}") from exc
 
     def _evaluate_trust(self, trust_bundle: bytes) -> int:
         # We want data in memory, so load it up.
         if os.path.isfile(trust_bundle):
             with open(trust_bundle, "rb") as f:
                 trust_bundle = f.read()
@@ -549,15 +550,15 @@
         data = buffer[:bytes_read]
         return typing.cast(bytes, data)
 
     def recv_into(
         self, buffer: ctypes.Array[ctypes.c_char], nbytes: int | None = None
     ) -> int:
         # Read short on EOF.
-        if self._closed:
+        if self._real_closed:
             return 0
 
         if nbytes is None:
             nbytes = len(buffer)
 
         buffer = (ctypes.c_char * nbytes).from_buffer(buffer)
         processed_bytes = ctypes.c_size_t(0)
@@ -582,15 +583,15 @@
             SecurityConst.errSSLClosedGraceful,
             SecurityConst.errSSLClosedNoNotify,
         ):
             # The remote peer has closed this connection. We should do so as
             # well. Note that we don't actually return here because in
             # principle this could actually be fired along with return data.
             # It's unlikely though.
-            self.close()
+            self._real_close()
         else:
             _assert_no_error(result)
 
         # Ok, we read and probably succeeded. We should return whatever data
         # was actually read.
         return processed_bytes.value
 
@@ -624,31 +625,33 @@
             total_sent += sent
 
     def shutdown(self) -> None:
         with self._raise_on_error():
             Security.SSLClose(self.context)
 
     def close(self) -> None:
+        self._closed = True
         # TODO: should I do clean shutdown here? Do I have to?
-        if self._io_refs < 1:
-            self._closed = True
-            if self.context:
-                CoreFoundation.CFRelease(self.context)
-                self.context = None
-            if self._client_cert_chain:
-                CoreFoundation.CFRelease(self._client_cert_chain)
-                self._client_cert_chain = None
-            if self._keychain:
-                Security.SecKeychainDelete(self._keychain)
-                CoreFoundation.CFRelease(self._keychain)
-                shutil.rmtree(self._keychain_dir)
-                self._keychain = self._keychain_dir = None
-            return self.socket.close()
-        else:
-            self._io_refs -= 1
+        if self._io_refs <= 0:
+            self._real_close()
+
+    def _real_close(self) -> None:
+        self._real_closed = True
+        if self.context:
+            CoreFoundation.CFRelease(self.context)
+            self.context = None
+        if self._client_cert_chain:
+            CoreFoundation.CFRelease(self._client_cert_chain)
+            self._client_cert_chain = None
+        if self._keychain:
+            Security.SecKeychainDelete(self._keychain)
+            CoreFoundation.CFRelease(self._keychain)
+            shutil.rmtree(self._keychain_dir)
+            self._keychain = self._keychain_dir = None
+        return self.socket.close()
 
     def getpeercert(self, binary_form: bool = False) -> bytes | None:
         # Urgh, annoying.
         #
         # Here's how we do this:
         #
         # 1. Call SSLCopyPeerTrust to get hold of the trust object for this
```

### Comparing `urllib3-2.0.0a3/src/urllib3/contrib/socks.py` & `urllib3-2.0.0a4/src/urllib3/contrib/socks.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a3/src/urllib3/contrib/_securetransport/bindings.py` & `urllib3-2.0.0a4/src/urllib3/contrib/_securetransport/bindings.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a3/src/urllib3/contrib/_securetransport/low_level.py` & `urllib3-2.0.0a4/src/urllib3/contrib/_securetransport/low_level.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a3/src/urllib3/util/__init__.py` & `urllib3-2.0.0a4/src/urllib3/util/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a3/src/urllib3/util/connection.py` & `urllib3-2.0.0a4/src/urllib3/util/connection.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a3/src/urllib3/util/proxy.py` & `urllib3-2.0.0a4/src/urllib3/util/proxy.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a3/src/urllib3/util/request.py` & `urllib3-2.0.0a4/src/urllib3/util/request.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a3/src/urllib3/util/response.py` & `urllib3-2.0.0a4/src/urllib3/util/response.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a3/src/urllib3/util/retry.py` & `urllib3-2.0.0a4/src/urllib3/util/retry.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import email
 import logging
+import random
 import re
 import time
 import typing
 from itertools import takewhile
 from types import TracebackType
 
 from ..exceptions import (
@@ -140,19 +141,23 @@
     :param float backoff_factor:
         A backoff factor to apply between attempts after the second try
         (most errors are resolved immediately by a second try without a
         delay). urllib3 will sleep for::
 
             {backoff factor} * (2 ** ({number of total retries} - 1))
 
-        seconds. If the backoff_factor is 0.1, then :func:`Retry.sleep` will sleep
-        for [0.0s, 0.2s, 0.4s, ...] between retries. It will never be longer
-        than `backoff_max`.
+        seconds. If `backoff_jitter` is non-zero, this sleep is extended by::
 
-        By default, backoff is disabled (set to 0).
+            random.uniform(0, {backoff jitter})
+
+        seconds. For example, if the backoff_factor is 0.1, then :func:`Retry.sleep` will
+        sleep for [0.0s, 0.2s, 0.4s, 0.8s, ...] between retries. No backoff will ever
+        be longer than `backoff_max`.
+
+        By default, backoff is disabled (factor set to 0).
 
     :param bool raise_on_redirect: Whether, if the number of redirects is
         exhausted, to raise a MaxRetryError, or to return a response with a
         response code in the 3xx range.
 
     :param bool raise_on_status: Similar meaning to ``raise_on_redirect``:
         whether we should raise an exception, or return a response,
@@ -205,14 +210,15 @@
         raise_on_redirect: bool = True,
         raise_on_status: bool = True,
         history: tuple[RequestHistory, ...] | None = None,
         respect_retry_after_header: bool = True,
         remove_headers_on_redirect: typing.Collection[
             str
         ] = DEFAULT_REMOVE_HEADERS_ON_REDIRECT,
+        backoff_jitter: float = 0.0,
     ) -> None:
         self.total = total
         self.connect = connect
         self.read = read
         self.status = status
         self.other = other
 
@@ -228,14 +234,15 @@
         self.raise_on_redirect = raise_on_redirect
         self.raise_on_status = raise_on_status
         self.history = history or ()
         self.respect_retry_after_header = respect_retry_after_header
         self.remove_headers_on_redirect = frozenset(
             h.lower() for h in remove_headers_on_redirect
         )
+        self.backoff_jitter = backoff_jitter
 
     def new(self, **kw: typing.Any) -> Retry:
         params = dict(
             total=self.total,
             connect=self.connect,
             read=self.read,
             redirect=self.redirect,
@@ -246,14 +253,15 @@
             backoff_factor=self.backoff_factor,
             backoff_max=self.backoff_max,
             raise_on_redirect=self.raise_on_redirect,
             raise_on_status=self.raise_on_status,
             history=self.history,
             remove_headers_on_redirect=self.remove_headers_on_redirect,
             respect_retry_after_header=self.respect_retry_after_header,
+            backoff_jitter=self.backoff_jitter,
         )
 
         params.update(kw)
         return type(self)(**params)  # type: ignore[arg-type]
 
     @classmethod
     def from_int(
@@ -285,15 +293,17 @@
                 takewhile(lambda x: x.redirect_location is None, reversed(self.history))
             )
         )
         if consecutive_errors_len <= 1:
             return 0
 
         backoff_value = self.backoff_factor * (2 ** (consecutive_errors_len - 1))
-        return float(min(self.backoff_max, backoff_value))
+        if self.backoff_jitter != 0.0:
+            backoff_value += random.random() * self.backoff_jitter
+        return float(max(0, min(self.backoff_max, backoff_value)))
 
     def parse_retry_after(self, retry_after: str) -> float:
         seconds: float
         # Whitespace: https://tools.ietf.org/html/rfc7230#section-3.2.4
         if re.match(r"^\s*[0-9]+\s*$", retry_after):
             seconds = int(retry_after)
         else:
```

### Comparing `urllib3-2.0.0a3/src/urllib3/util/ssl_.py` & `urllib3-2.0.0a4/src/urllib3/util/ssl_.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a3/src/urllib3/util/ssl_match_hostname.py` & `urllib3-2.0.0a4/src/urllib3/util/ssl_match_hostname.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a3/src/urllib3/util/ssltransport.py` & `urllib3-2.0.0a4/src/urllib3/util/ssltransport.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import socket
 import ssl
 import typing
 
 from ..exceptions import ProxySchemeUnsupported
 
 if typing.TYPE_CHECKING:
-
     from typing_extensions import Literal
 
     from .ssl_ import _TYPE_PEER_CERT_RET, _TYPE_PEER_CERT_RET_DICT
 
 
 _SelfT = typing.TypeVar("_SelfT", bound="SSLTransport")
 _WriteBuffer = typing.Union[bytearray, memoryview]
```

### Comparing `urllib3-2.0.0a3/src/urllib3/util/timeout.py` & `urllib3-2.0.0a4/src/urllib3/util/timeout.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a3/src/urllib3/util/url.py` & `urllib3-2.0.0a4/src/urllib3/util/url.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,17 +44,15 @@
     "(?:(?:%(hex)s:){0,4}%(hex)s)?::%(ls32)s",
     # [ *5( h16 ":" ) h16 ] "::"              h16
     "(?:(?:%(hex)s:){0,5}%(hex)s)?::%(hex)s",
     # [ *6( h16 ":" ) h16 ] "::"
     "(?:(?:%(hex)s:){0,6}%(hex)s)?::",
 ]
 
-_UNRESERVED_PAT = (
-    r"ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789._!\-~"
-)
+_UNRESERVED_PAT = r"ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789._\-~"
 _IPV6_PAT = "(?:" + "|".join([x % _subs for x in _variations]) + ")"
 _ZONE_ID_PAT = "(?:%25|%)(?:[" + _UNRESERVED_PAT + "]|%[a-fA-F0-9]{2})+"
 _IPV6_ADDRZ_PAT = r"\[" + _IPV6_PAT + r"(?:" + _ZONE_ID_PAT + r")?\]"
 _REG_NAME_PAT = r"(?:[^\[\]%:/?#]|%[a-fA-F0-9]{2})*"
 _TARGET_RE = re.compile(r"^(/[^?#]*)(?:\?([^#]*))?(?:#.*)?$")
 
 _IPV4_RE = re.compile("^" + _IPV4_PAT + "$")
@@ -328,15 +326,15 @@
                     b".".join([_idna_encode(label) for label in host.split(".")]),
                     "ascii",
                 )
     return host
 
 
 def _idna_encode(name: str) -> bytes:
-    if name and any([ord(x) > 128 for x in name]):
+    if not name.isascii():
         try:
             import idna
         except ImportError:
             raise LocationParseError(
                 "Unable to parse URL without the 'idna' module"
             ) from None
```

### Comparing `urllib3-2.0.0a3/src/urllib3/util/util.py` & `urllib3-2.0.0a4/src/urllib3/util/util.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a3/src/urllib3/util/wait.py` & `urllib3-2.0.0a4/src/urllib3/util/wait.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a3/test/__init__.py` & `urllib3-2.0.0a4/test/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
     except socket.gaierror:
         return False
 
 
 def has_alpn(ctx_cls: type[ssl.SSLContext] | None = None) -> bool:
     """Detect if ALPN support is enabled."""
     ctx_cls = ctx_cls or util.SSLContext
-    ctx = ctx_cls(protocol=ssl_.PROTOCOL_TLS)  # type: ignore[misc]
+    ctx = ctx_cls(protocol=ssl_.PROTOCOL_TLS)  # type: ignore[misc, attr-defined]
     try:
         if hasattr(ctx, "set_alpn_protocols"):
             ctx.set_alpn_protocols(ssl_.ALPN_PROTOCOLS)
             return True
     except NotImplementedError:
         pass
     return False
@@ -214,17 +214,17 @@
 
     return pytest.mark.skipif(
         not _requires_network_has_route,
         reason="Can't run the test because the network is unreachable",
     )
 
 
-def requires_ssl_context_keyfile_password() -> typing.Callable[
-    [_TestFuncT], _TestFuncT
-]:
+def requires_ssl_context_keyfile_password() -> (
+    typing.Callable[[_TestFuncT], _TestFuncT]
+):
     return pytest.mark.skipif(
         lazy_condition(lambda: ssl_.IS_SECURETRANSPORT),
         reason="Test requires password parameter for SSLContext.load_cert_chain()",
     )
 
 
 def resolvesLocalhostFQDN() -> typing.Callable[[_TestFuncT], _TestFuncT]:
@@ -320,15 +320,14 @@
 
     def find_spec(
         self,
         fullname: str,
         path: Sequence[bytes | str] | None,
         target: ModuleType | None = None,
     ) -> ModuleSpec | None:
-
         loader = self.find_module(fullname, path)
         if loader is None:
             return None
 
         return importlib.util.spec_from_loader(fullname, loader)
```

### Comparing `urllib3-2.0.0a3/test/conftest.py` & `urllib3-2.0.0a4/test/conftest.py`

 * *Files 3% similar despite different names*

```diff
@@ -286,27 +286,32 @@
     # to test if the TLS version is not disabled by
     # OpenSSL config. Ubuntu 20.04 specifically
     # disables TLSv1 and TLSv1.1.
     tls_versions = set()
 
     _server = HTTPSDummyServerTestCase()
     _server._start_server()
-    for _ssl_version_name in (
-        "PROTOCOL_TLSv1",
-        "PROTOCOL_TLSv1_1",
-        "PROTOCOL_TLSv1_2",
-        "PROTOCOL_TLS",
+    for _ssl_version_name, min_max_version in (
+        ("PROTOCOL_TLSv1", ssl.TLSVersion.TLSv1),
+        ("PROTOCOL_TLSv1_1", ssl.TLSVersion.TLSv1_1),
+        ("PROTOCOL_TLSv1_2", ssl.TLSVersion.TLSv1_2),
+        ("PROTOCOL_TLS", None),
     ):
         _ssl_version = getattr(ssl, _ssl_version_name, 0)
         if _ssl_version == 0:
             continue
         _sock = socket.create_connection((_server.host, _server.port))
         try:
             _sock = ssl_.ssl_wrap_socket(
-                _sock, cert_reqs=ssl.CERT_NONE, ssl_version=_ssl_version
+                _sock,
+                ssl_context=ssl_.create_urllib3_context(
+                    cert_reqs=ssl.CERT_NONE,
+                    ssl_minimum_version=min_max_version,
+                    ssl_maximum_version=min_max_version,
+                ),
             )
         except ssl.SSLError:
             pass
         else:
             tls_versions.add(_sock.version())
         _sock.close()
     _server._stop_server()
```

### Comparing `urllib3-2.0.0a3/test/port_helpers.py` & `urllib3-2.0.0a4/test/port_helpers.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a3/test/test_collections.py` & `urllib3-2.0.0a4/test/test_collections.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a3/test/test_compatibility.py` & `urllib3-2.0.0a4/test/test_compatibility.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a3/test/test_connection.py` & `urllib3-2.0.0a4/test/test_connection.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,30 +58,30 @@
         except CertificateError as e:
             assert "hostname 'bar' doesn't match 'foo'" in str(e)
             mock_log.assert_called_once_with(
                 "Certificate did not match expected hostname: %s. Certificate: %s",
                 "bar",
                 {"subjectAltName": (("DNS", "foo"),)},
             )
-            assert e._peer_cert == cert
+            assert e._peer_cert == cert  # type: ignore[attr-defined]
 
     def test_match_hostname_no_dns(self) -> None:
         cert: _TYPE_PEER_CERT_RET_DICT = {"subjectAltName": (("DNS", ""),)}
         asserted_hostname = "bar"
         try:
             with mock.patch("urllib3.connection.log.warning") as mock_log:
                 _match_hostname(cert, asserted_hostname)
         except CertificateError as e:
             assert "hostname 'bar' doesn't match ''" in str(e)
             mock_log.assert_called_once_with(
                 "Certificate did not match expected hostname: %s. Certificate: %s",
                 "bar",
                 {"subjectAltName": (("DNS", ""),)},
             )
-            assert e._peer_cert == cert
+            assert e._peer_cert == cert  # type: ignore[attr-defined]
 
     def test_match_hostname_startwith_wildcard(self) -> None:
         cert: _TYPE_PEER_CERT_RET_DICT = {"subjectAltName": (("DNS", "*"),)}
         asserted_hostname = "foo"
         _match_hostname(cert, asserted_hostname)
 
     def test_match_hostname_dnsname(self) -> None:
@@ -133,15 +133,15 @@
         except CertificateError as e:
             assert "hostname '1.1.1.2' doesn't match '1.1.1.1'" in str(e)
             mock_log.assert_called_once_with(
                 "Certificate did not match expected hostname: %s. Certificate: %s",
                 "1.1.1.2",
                 {"subjectAltName": (("IP Address", "1.1.1.1"),)},
             )
-            assert e._peer_cert == cert
+            assert e._peer_cert == cert  # type: ignore[attr-defined]
 
     @pytest.mark.parametrize(
         ["asserted_hostname", "san_ip"],
         [
             ("1:2::3:4", "1:2:0:0:0:0:3:4"),
             ("1:2:0:0::3:4", "1:2:0:0:0:0:3:4"),
             ("::0.1.0.2", "0:0:0:0:0:0:1:2"),
@@ -167,15 +167,15 @@
         except CertificateError as e:
             assert "hostname '1:2::2:2' doesn't match '1:2::2:1'" in str(e)
             mock_log.assert_called_once_with(
                 "Certificate did not match expected hostname: %s. Certificate: %s",
                 "1:2::2:2",
                 {"subjectAltName": (("IP Address", "1:2::2:1"),)},
             )
-            assert e._peer_cert == cert
+            assert e._peer_cert == cert  # type: ignore[attr-defined]
 
     def test_match_hostname_dns_with_brackets_doesnt_match(self) -> None:
         cert: _TYPE_PEER_CERT_RET_DICT = {
             "subjectAltName": (
                 ("DNS", "localhost"),
                 ("IP Address", "localhost"),
             )
```

### Comparing `urllib3-2.0.0a3/test/test_connectionpool.py` & `urllib3-2.0.0a4/test/test_connectionpool.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a3/test/test_exceptions.py` & `urllib3-2.0.0a4/test/test_exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,17 +53,17 @@
         assert "unparsed_data" in str(hpe)
 
 
 class TestNewConnectionError:
     def test_pool_property_deprecation_warning(self) -> None:
         err = NewConnectionError(HTTPConnection("localhost"), "test")
         with pytest.warns(DeprecationWarning) as records:
-            err.pool
+            err_pool = err.pool
 
-        assert err.pool is err.conn
+        assert err_pool is err.conn
         msg = (
             "The 'pool' property is deprecated and will be removed "
             "in urllib3 v2.1.0. Use 'conn' instead."
         )
         record = records[0]
         assert isinstance(record.message, Warning)
         assert record.message.args[0] == msg
```

### Comparing `urllib3-2.0.0a3/test/test_fields.py` & `urllib3-2.0.0a4/test/test_fields.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a3/test/test_filepost.py` & `urllib3-2.0.0a4/test/test_filepost.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a3/test/test_no_ssl.py` & `urllib3-2.0.0a4/test/test_no_ssl.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a3/test/test_poolmanager.py` & `urllib3-2.0.0a4/test/test_poolmanager.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a3/test/test_proxymanager.py` & `urllib3-2.0.0a4/test/test_proxymanager.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a3/test/test_queue_monkeypatch.py` & `urllib3-2.0.0a4/test/test_queue_monkeypatch.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a3/test/test_response.py` & `urllib3-2.0.0a4/test/test_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -350,14 +350,23 @@
     @pytest.mark.parametrize("data", [b"foo", b"x" * 100])
     def test_decode_zstd_error(self, data: bytes) -> None:
         fp = BytesIO(data)
 
         with pytest.raises(DecodeError):
             HTTPResponse(fp, headers={"content-encoding": "zstd"})
 
+    @onlyZstd()
+    @pytest.mark.parametrize("data", [b"foo", b"x" * 100])
+    def test_decode_zstd_incomplete(self, data: bytes) -> None:
+        data = zstd.compress(data)
+        fp = BytesIO(data[:-1])
+
+        with pytest.raises(DecodeError):
+            HTTPResponse(fp, headers={"content-encoding": "zstd"})
+
     def test_multi_decoding_deflate_deflate(self) -> None:
         data = zlib.compress(zlib.compress(b"foo"))
 
         fp = BytesIO(data)
         r = HTTPResponse(fp, headers={"content-encoding": "deflate, deflate"})
 
         assert r.data == b"foo"
```

### Comparing `urllib3-2.0.0a3/test/test_retry.py` & `urllib3-2.0.0a4/test/test_retry.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 from test import DUMMY_POOL
 from unittest import mock
 
+import freezegun  # type: ignore[import]
 import pytest
 
 from urllib3.exceptions import (
     ConnectTimeoutError,
     InvalidHeader,
     MaxRetryError,
     ReadTimeoutError,
@@ -176,14 +177,43 @@
 
         retry = retry.increment(method="GET")
         assert retry.get_backoff_time() == max_backoff
 
         retry = retry.increment(method="GET")
         assert retry.get_backoff_time() == max_backoff
 
+    def test_backoff_jitter(self) -> None:
+        """Backoff with jitter is computed correctly"""
+        max_backoff = 1
+        jitter = 0.4
+        retry = Retry(
+            total=100,
+            backoff_factor=0.2,
+            backoff_max=max_backoff,
+            backoff_jitter=jitter,
+        )
+        assert retry.get_backoff_time() == 0  # First request
+
+        retry = retry.increment(method="GET")
+        assert retry.get_backoff_time() == 0  # First retry
+
+        retry = retry.increment(method="GET")
+        assert retry.backoff_factor == 0.2
+        assert retry.total == 98
+        assert 0.4 <= retry.get_backoff_time() <= 0.8  # Start backoff
+
+        retry = retry.increment(method="GET")
+        assert 0.8 <= retry.get_backoff_time() <= max_backoff
+
+        retry = retry.increment(method="GET")
+        assert retry.get_backoff_time() == max_backoff
+
+        retry = retry.increment(method="GET")
+        assert retry.get_backoff_time() == max_backoff
+
     def test_zero_backoff(self) -> None:
         retry = Retry()
         assert retry.get_backoff_time() == 0
         retry = retry.increment(method="GET")
         retry = retry.increment(method="GET")
         assert retry.get_backoff_time() == 0
 
@@ -324,20 +354,18 @@
         retry = Retry()
         assert retry.parse_retry_after(value) == expected
 
     @pytest.mark.parametrize("respect_retry_after_header", [True, False])
     def test_respect_retry_after_header_propagated(
         self, respect_retry_after_header: bool
     ) -> None:
-
         retry = Retry(respect_retry_after_header=respect_retry_after_header)
         new_retry = retry.new()
         assert new_retry.respect_retry_after_header == respect_retry_after_header
 
-    @pytest.mark.freeze_time("2019-06-03 11:00:00", tz_offset=0)
     @pytest.mark.parametrize(
         "retry_after_header,respect_retry_after_header,sleep_duration",
         [
             ("3600", True, 3600),
             ("3600", False, None),
             # Will sleep due to header is 1 hour in future
             ("Mon, 3 Jun 2019 12:00:00 UTC", True, 3600),
@@ -368,15 +396,17 @@
         self,
         retry_after_header: str,
         respect_retry_after_header: bool,
         sleep_duration: int | None,
     ) -> None:
         retry = Retry(respect_retry_after_header=respect_retry_after_header)
 
-        with mock.patch("time.sleep") as sleep_mock:
+        with freezegun.freeze_time("2019-06-03 11:00:00", tz_offset=0), mock.patch(
+            "time.sleep"
+        ) as sleep_mock:
             # for the default behavior, it must be in RETRY_AFTER_STATUS_CODES
             response = HTTPResponse(
                 status=503, headers={"Retry-After": retry_after_header}
             )
 
             retry.sleep(response)
```

### Comparing `urllib3-2.0.0a3/test/test_ssl.py` & `urllib3-2.0.0a4/test/test_ssl.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,15 +43,14 @@
     )
     def test_is_ipaddress_false(self, addr: bytes | str) -> None:
         assert not ssl_.is_ipaddress(addr)
 
     def test_create_urllib3_context_set_ciphers(
         self, monkeypatch: pytest.MonkeyPatch
     ) -> None:
-
         ciphers = "ECDH+AESGCM:ECDH+CHACHA20"
         context = mock.create_autospec(ssl_.SSLContext)
         context.set_ciphers = mock.Mock()
         context.options = 0
         monkeypatch.setattr(ssl_, "SSLContext", lambda *_, **__: context)
 
         assert ssl_.create_urllib3_context(ciphers=ciphers) is context
@@ -178,26 +177,41 @@
                 "ssl_version": ssl.PROTOCOL_TLS_CLIENT,
                 "ssl_minimum_version": ssl.TLSVersion.MINIMUM_SUPPORTED,
             },
             {
                 "ssl_version": None,
                 "ssl_minimum_version": ssl.TLSVersion.MINIMUM_SUPPORTED,
             },
+        ],
+    )
+    def test_create_urllib3_context_ssl_version_and_ssl_min_max_version_no_warning(
+        self, kwargs: dict[str, typing.Any]
+    ) -> None:
+        ssl_.create_urllib3_context(**kwargs)
+
+    @pytest.mark.parametrize(
+        "kwargs",
+        [
             {"ssl_version": ssl.PROTOCOL_TLSv1, "ssl_minimum_version": None},
             {"ssl_version": ssl.PROTOCOL_TLSv1, "ssl_maximum_version": None},
             {
                 "ssl_version": ssl.PROTOCOL_TLSv1,
                 "ssl_minimum_version": None,
                 "ssl_maximum_version": None,
             },
         ],
     )
     def test_create_urllib3_context_ssl_version_and_ssl_min_max_version_no_error(
         self, kwargs: dict[str, typing.Any]
     ) -> None:
-        ssl_.create_urllib3_context(**kwargs)
+        with pytest.warns(
+            DeprecationWarning,
+            match=r"'ssl_version' option is deprecated and will be removed in "
+            r"urllib3 v2\.1\.0\. Instead use 'ssl_minimum_version'",
+        ):
+            ssl_.create_urllib3_context(**kwargs)
 
     def test_assert_fingerprint_raises_exception_on_none_cert(self) -> None:
         with pytest.raises(SSLError):
             ssl_.assert_fingerprint(
                 cert=None, fingerprint="55:39:BF:70:05:12:43:FA:1F:D1:BF:4E:E8:1B:07:1D"
             )
```

### Comparing `urllib3-2.0.0a3/test/test_ssltransport.py` & `urllib3-2.0.0a4/test/test_ssltransport.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,14 @@
 ) -> None:
     assert provided_response is not None
     expected_response = sample_response(binary)
     assert provided_response == expected_response
 
 
 def validate_peercert(ssl_socket: SSLTransport) -> None:
-
     binary_cert = ssl_socket.getpeercert(binary_form=True)
     assert type(binary_cert) == bytes
     assert len(binary_cert) > 0
 
     cert = ssl_socket.getpeercert()
     assert type(cert) == dict
     assert "serialNumber" in cert
@@ -226,16 +225,19 @@
             assert type(cipher) == tuple
 
             # No chosen protocol through ALPN or NPN.
             assert ssock.selected_alpn_protocol() is None
             assert ssock.selected_npn_protocol() is None
 
             shared_ciphers = ssock.shared_ciphers()
-            assert type(shared_ciphers) == list
-            assert len(shared_ciphers) > 0
+            # SSLContext.shared_ciphers() changed behavior completely in a patch version.
+            # See: https://github.com/python/cpython/issues/96931
+            assert shared_ciphers is None or (
+                type(shared_ciphers) is list and len(shared_ciphers) > 0
+            )
 
             assert ssock.compression() is None
 
             validate_peercert(ssock)
 
             ssock.send(sample_request())
             response = consume_socket(ssock)
@@ -436,17 +438,16 @@
         )
         with self.client_context.wrap_socket(
             sock, server_hostname="localhost"
         ) as proxy_sock:
             with SSLTransport(
                 proxy_sock, self.client_context, server_hostname="localhost"
             ) as destination_sock:
-
                 file = destination_sock.makefile("rwb", buffering)
-                file.write(sample_request())  # type: ignore[arg-type]
+                file.write(sample_request())  # type: ignore[call-overload]
                 file.flush()
 
                 response = bytearray(65536)
                 wrote = file.readinto(response)  # type: ignore[union-attr]
                 assert wrote is not None
                 # Allocated response is bigger than the actual response, we
                 # rtrim remaining x00 bytes.
@@ -472,19 +473,18 @@
         )
         with self.client_context.wrap_socket(
             sock, server_hostname="localhost"
         ) as proxy_sock:
             with SSLTransport(
                 proxy_sock, self.client_context, server_hostname="localhost"
             ) as destination_sock:
-
                 read = destination_sock.makefile("r", encoding="utf-8")
                 write = destination_sock.makefile("w", encoding="utf-8")
 
-                write.write(sample_request(binary=False))  # type: ignore[arg-type]
+                write.write(sample_request(binary=False))  # type: ignore[arg-type, call-overload]
                 write.flush()
 
                 response = read.read()
                 assert isinstance(response, str)
                 if "\r" not in response:
                     # Carriage return will be removed when reading as a file on
                     # some platforms.  We add it before the comparison.
@@ -506,15 +506,14 @@
         )
         with self.client_context.wrap_socket(
             sock, server_hostname="localhost"
         ) as proxy_sock:
             with SSLTransport(
                 proxy_sock, self.client_context, server_hostname="localhost"
             ) as destination_sock:
-
                 destination_sock.sendall(sample_request())
                 response = bytearray(65536)
                 destination_sock.recv_into(response)
                 str_response = response.decode("utf-8").rstrip("\x00")
                 validate_response(str_response, binary=False)
```

### Comparing `urllib3-2.0.0a3/test/test_util.py` & `urllib3-2.0.0a4/test/test_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,14 @@
 # This number represents a time in seconds, it doesn't mean anything in
 # isolation. Setting to a high-ish value to avoid conflicts with the smaller
 # numbers used for timeouts
 TIMEOUT_EPOCH = 1000
 
 
 class TestUtil:
-
     url_host_map = [
         # Hosts
         ("http://google.com/mail", ("http", "google.com", None)),
         ("http://google.com/mail/", ("http", "google.com", None)),
         ("google.com/mail", ("http", "google.com", None)),
         ("http://google.com/", ("http", "google.com", None)),
         ("http://google.com", ("http", "google.com", None)),
```

### Comparing `urllib3-2.0.0a3/test/test_wait.py` & `urllib3-2.0.0a4/test/test_wait.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,16 +149,19 @@
         try:
             # Start delivering SIGALRM 1000 times per second,
             # to trigger race conditions such as
             # https://github.com/urllib3/urllib3/issues/1396.
             signal.setitimer(signal.ITIMER_REAL, 0.001, 0.001)
             # Hammer the system call for a while to trigger the
             # race.
+            end = time.monotonic() + 5
             for i in range(100000):
                 wfs(a, read=True, timeout=0)
+                if time.monotonic() >= end:
+                    break
         finally:
             # Stop delivering SIGALRM
             signal.setitimer(signal.ITIMER_REAL, 0)
     finally:
         signal.signal(signal.SIGALRM, old_handler)
 
     assert interrupt_count[0] > 0
```

### Comparing `urllib3-2.0.0a3/test/tz_stub.py` & `urllib3-2.0.0a4/test/tz_stub.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a3/test/contrib/duplicate_san.pem` & `urllib3-2.0.0a4/test/contrib/duplicate_san.pem`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a3/test/contrib/test_pyopenssl.py` & `urllib3-2.0.0a4/test/contrib/test_pyopenssl.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a3/test/contrib/test_pyopenssl_dependencies.py` & `urllib3-2.0.0a4/test/contrib/test_pyopenssl_dependencies.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a3/test/contrib/test_securetransport.py` & `urllib3-2.0.0a4/test/contrib/test_securetransport.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a3/test/contrib/test_socks.py` & `urllib3-2.0.0a4/test/contrib/test_socks.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a3/test/with_dummyserver/test_chunked_transfer.py` & `urllib3-2.0.0a4/test/with_dummyserver/test_chunked_transfer.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a3/test/with_dummyserver/test_connection.py` & `urllib3-2.0.0a4/test/with_dummyserver/test_connection.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a3/test/with_dummyserver/test_connectionpool.py` & `urllib3-2.0.0a4/test/with_dummyserver/test_connectionpool.py`

 * *Files 0% similar despite different names*

```diff
@@ -1056,15 +1056,14 @@
                 conn.request("GET", "/headers", headers=headers, chunked=chunked)
 
             assert headers == {"key": "val"}
 
     def test_request_chunked_is_deprecated(
         self,
     ) -> None:
-
         with HTTPConnectionPool(self.host, self.port) as pool:
             conn = pool._get_conn()
 
             with pytest.warns(DeprecationWarning) as w:
                 conn.request_chunked("GET", "/headers")  # type: ignore[attr-defined]
             assert len(w) == 1 and str(w[0].message) == (
                 "HTTPConnection.request_chunked() is deprecated and will be removed in urllib3 v2.1.0. "
```

### Comparing `urllib3-2.0.0a3/test/with_dummyserver/test_https.py` & `urllib3-2.0.0a4/test/with_dummyserver/test_https.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import contextlib
 import datetime
 import os.path
 import shutil
 import ssl
 import sys
 import tempfile
 import warnings
@@ -504,15 +505,14 @@
         with HTTPSConnectionPool(
             self.host,
             self.port,
             cert_reqs="CERT_REQUIRED",
             ca_certs=DEFAULT_CA,
             ssl_minimum_version=self.tls_version(),
         ) as https_pool:
-
             https_pool.assert_fingerprint = (
                 "AA:AA:AA:AA:AA:AAAA:AA:AAAA:AA:AA:AA:AA:AA:AA:AA:AA:AA:AA"
             )
             e = _test_request(https_pool)
             expected = "aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa"
             got = "728b554c9afc1e88a11cad1bb2e7cc3edbc8f98a"
             assert (
@@ -570,15 +570,14 @@
             https_pool.assert_fingerprint = (
                 "72:8B:55:4C:9A:FC:1E:88:A1:1C:AD:1B:B2:E7:CC:3E:DB:C8:F9:8A"
             )
             https_pool.request("GET", "/")
 
     @requires_network()
     def test_https_timeout(self) -> None:
-
         timeout = Timeout(total=None, connect=SHORT_TIMEOUT)
         with HTTPSConnectionPool(
             TARPIT_HOST,
             self.port,
             timeout=timeout,
             retries=False,
             cert_reqs="CERT_REQUIRED",
@@ -605,15 +604,16 @@
         with HTTPSConnectionPool(
             self.host,
             self.port,
             timeout=timeout,
             cert_reqs="CERT_NONE",
             ssl_minimum_version=self.tls_version(),
         ) as https_pool:
-            https_pool.request("GET", "/")
+            with pytest.warns(InsecureRequestWarning):
+                https_pool.request("GET", "/")
 
     def test_tunnel(self) -> None:
         """test the _tunnel behavior"""
         timeout = Timeout(total=None)
         with HTTPSConnectionPool(
             self.host,
             self.port,
@@ -623,15 +623,16 @@
         ) as https_pool:
             conn = https_pool._new_conn()
             try:
                 conn.set_tunnel(self.host, self.port)
                 with mock.patch.object(
                     conn, "_tunnel", create=True, return_value=None
                 ) as conn_tunnel:
-                    https_pool._make_request(conn, "GET", "/")
+                    with pytest.warns(InsecureRequestWarning):
+                        https_pool._make_request(conn, "GET", "/")
                 conn_tunnel.assert_called_once_with()
             finally:
                 conn.close()
 
     @requires_network()
     def test_enhanced_timeout(self) -> None:
         with HTTPSConnectionPool(
@@ -744,16 +745,27 @@
     def test_set_ssl_version_to_tls_version(self) -> None:
         if self.tls_protocol_name is None:
             pytest.skip("Skipping base test class")
 
         with HTTPSConnectionPool(
             self.host, self.port, ca_certs=DEFAULT_CA
         ) as https_pool:
-            https_pool.ssl_version = self.certs["ssl_version"]
-            r = https_pool.request("GET", "/")
+            https_pool.ssl_version = ssl_version = self.certs["ssl_version"]
+            if ssl_version is getattr(ssl, "PROTOCOL_TLS", object()):
+                cmgr: contextlib.AbstractContextManager[
+                    object
+                ] = contextlib.nullcontext()
+            else:
+                cmgr = pytest.warns(
+                    DeprecationWarning,
+                    match=r"'ssl_version' option is deprecated and will be removed "
+                    r"in urllib3 v2\.1\.0\. Instead use 'ssl_minimum_version'",
+                )
+            with cmgr:
+                r = https_pool.request("GET", "/")
             assert r.status == 200, r.data
 
     def test_set_cert_default_cert_required(self) -> None:
         conn = VerifiedHTTPSConnection(self.host, self.port)
         with pytest.warns(DeprecationWarning) as w:
             conn.set_cert()
         assert conn.cert_reqs == ssl.CERT_REQUIRED
@@ -806,15 +818,15 @@
             pytest.skip("Skipping base test class")
 
         with HTTPSConnectionPool(
             self.host, self.port, ca_certs=DEFAULT_CA, ssl_version=self.ssl_version()
         ) as https_pool:
             conn = https_pool._get_conn()
             try:
-                with warnings.catch_warnings(record=True) as w:
+                with pytest.warns(DeprecationWarning) as w:
                     conn.connect()
             finally:
                 conn.close()
 
         assert len(w) >= 1
         assert any(x.category == DeprecationWarning for x in w)
         assert any(
@@ -845,15 +857,15 @@
             conn = https_pool._get_conn()
             try:
                 with warnings.catch_warnings(record=True) as w:
                     conn.connect()
             finally:
                 conn.close()
 
-        assert [str(wm) for wm in w] == []
+        assert [str(wm) for wm in w if wm.category != ResourceWarning] == []
 
     def test_no_tls_version_deprecation_with_ssl_context(self) -> None:
         if self.tls_protocol_name is None:
             pytest.skip("Skipping base test class")
 
         ctx = util.ssl_.create_urllib3_context(ssl_minimum_version=self.tls_version())
 
@@ -866,15 +878,15 @@
             conn = https_pool._get_conn()
             try:
                 with warnings.catch_warnings(record=True) as w:
                     conn.connect()
             finally:
                 conn.close()
 
-        assert [str(wm) for wm in w] == []
+        assert [str(wm) for wm in w if wm.category != ResourceWarning] == []
 
     def test_tls_version_maximum_and_minimum(self) -> None:
         if self.tls_protocol_name is None:
             pytest.skip("Skipping base test class")
 
         from ssl import TLSVersion
 
@@ -958,26 +970,38 @@
             r = pool.request("GET", "/alpn_protocol", retries=0)
             assert r.status == 200
             assert r.data.decode("utf-8") == util.ALPN_PROTOCOLS[0]
 
     def test_default_ssl_context_ssl_min_max_versions(self) -> None:
         ctx = urllib3.util.ssl_.create_urllib3_context()
         assert ctx.minimum_version == ssl.TLSVersion.TLSv1_2
-        # urllib3 is not expected to change the maximum version, so the
-        # version should be the same as in a pure context. It will be
-        # either the `ssl.TLSVersion.MAXIMUM_SUPPORTED` magic constant
-        # or one of the exact versions if a system defines it.
+        # urllib3 sets a default maximum version only when it is
+        # injected with PyOpenSSL- or SecureTransport-backed
+        # SSL-support.
+        # Otherwise, the default maximum version is set by Python's
+        # `ssl.SSLContext`. The value respects OpenSSL configuration and
+        # can be different from `ssl.TLSVersion.MAXIMUM_SUPPORTED`.
         # https://github.com/urllib3/urllib3/issues/2477#issuecomment-1151452150
-        assert (
-            ctx.maximum_version
-            == ssl.SSLContext(ssl.PROTOCOL_TLS_CLIENT).maximum_version
-        )
+        if util.IS_PYOPENSSL or util.IS_SECURETRANSPORT:
+            expected_maximum_version = ssl.TLSVersion.MAXIMUM_SUPPORTED
+        else:
+            expected_maximum_version = ssl.SSLContext(
+                ssl.PROTOCOL_TLS_CLIENT
+            ).maximum_version
+        assert ctx.maximum_version == expected_maximum_version
 
     def test_ssl_context_ssl_version_uses_ssl_min_max_versions(self) -> None:
-        ctx = urllib3.util.ssl_.create_urllib3_context(ssl_version=self.ssl_version())
+        with pytest.warns(
+            DeprecationWarning,
+            match=r"'ssl_version' option is deprecated and will be removed in "
+            r"urllib3 v2\.1\.0\. Instead use 'ssl_minimum_version'",
+        ):
+            ctx = urllib3.util.ssl_.create_urllib3_context(
+                ssl_version=self.ssl_version()
+            )
         assert ctx.minimum_version == self.tls_version()
         assert ctx.maximum_version == self.tls_version()
 
 
 @pytest.mark.usefixtures("requires_tlsv1")
 class TestHTTPS_TLSv1(TestHTTPS):
     tls_protocol_name = "TLSv1"
```

### Comparing `urllib3-2.0.0a3/test/with_dummyserver/test_no_ssl.py` & `urllib3-2.0.0a4/test/with_dummyserver/test_no_ssl.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 """
 Test connections without the builtin ssl module
 
 Note: Import urllib3 inside the test functions to get the importblocker to work
 """
 from __future__ import annotations
 
+import pytest
+
 import urllib3
 from dummyserver.testcase import HTTPDummyServerTestCase, HTTPSDummyServerTestCase
+from urllib3.exceptions import InsecureRequestWarning
 
 from ..test_no_ssl import TestWithoutSSL
 
 
 class TestHTTPWithoutSSL(HTTPDummyServerTestCase, TestWithoutSSL):
     def test_simple(self) -> None:
         with urllib3.HTTPConnectionPool(self.host, self.port) as pool:
@@ -19,11 +22,12 @@
 
 
 class TestHTTPSWithoutSSL(HTTPSDummyServerTestCase, TestWithoutSSL):
     def test_simple(self) -> None:
         with urllib3.HTTPSConnectionPool(
             self.host, self.port, cert_reqs="NONE"
         ) as pool:
-            try:
-                pool.request("GET", "/")
-            except urllib3.exceptions.SSLError as e:
-                assert "SSL module is not available" in str(e)
+            with pytest.warns(InsecureRequestWarning):
+                try:
+                    pool.request("GET", "/")
+                except urllib3.exceptions.SSLError as e:
+                    assert "SSL module is not available" in str(e)
```

### Comparing `urllib3-2.0.0a3/test/with_dummyserver/test_poolmanager.py` & `urllib3-2.0.0a4/test/with_dummyserver/test_poolmanager.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a3/test/with_dummyserver/test_proxy_poolmanager.py` & `urllib3-2.0.0a4/test/with_dummyserver/test_proxy_poolmanager.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from dummyserver.testcase import HTTPDummyProxyTestCase, IPv6HTTPDummyProxyTestCase
 from urllib3 import HTTPResponse
 from urllib3._collections import HTTPHeaderDict
 from urllib3.connection import VerifiedHTTPSConnection
 from urllib3.connectionpool import connection_from_url
 from urllib3.exceptions import (
     ConnectTimeoutError,
+    InsecureRequestWarning,
     MaxRetryError,
     ProxyError,
     ProxySchemeUnknown,
     ProxySchemeUnsupported,
     ReadTimeoutError,
     SSLError,
 )
@@ -273,15 +274,14 @@
     def test_headers(self) -> None:
         with proxy_from_url(
             self.proxy_url,
             headers={"Foo": "bar"},
             proxy_headers={"Hickory": "dickory"},
             ca_certs=DEFAULT_CA,
         ) as http:
-
             r = http.request_encode_url("GET", f"{self.http_url}/headers")
             returned_headers = r.json()
             assert returned_headers.get("Foo") == "bar"
             assert returned_headers.get("Hickory") == "dickory"
             assert returned_headers.get("Host") == f"{self.http_host}:{self.http_port}"
 
             r = http.request_encode_url("GET", f"{self.http_url_alt}/headers")
@@ -349,15 +349,14 @@
     def test_https_headers(self) -> None:
         with proxy_from_url(
             self.https_proxy_url,
             headers={"Foo": "bar"},
             proxy_headers={"Hickory": "dickory"},
             ca_certs=DEFAULT_CA,
         ) as http:
-
             r = http.request_encode_url("GET", f"{self.http_url}/headers")
             returned_headers = r.json()
             assert returned_headers.get("Foo") == "bar"
             assert returned_headers.get("Hickory") == "dickory"
             assert returned_headers.get("Host") == f"{self.http_host}:{self.http_port}"
 
             r = http.request_encode_url("GET", f"{self.http_url_alt}/headers")
@@ -383,15 +382,14 @@
         with proxy_from_url(
             self.https_proxy_url,
             headers={"Foo": "bar"},
             proxy_headers={"Hickory": "dickory"},
             ca_certs=DEFAULT_CA,
             use_forwarding_for_https=True,
         ) as http:
-
             r = http.request_encode_url("GET", f"{self.https_url}/headers")
             returned_headers = r.json()
             assert returned_headers.get("Foo") == "bar"
             assert returned_headers.get("Hickory") == "dickory"
             assert (
                 returned_headers.get("Host") == f"{self.https_host}:{self.https_port}"
             )
@@ -417,19 +415,21 @@
             assert len(http.pools) == 1
 
             for x in range(2):
                 http.urlopen("GET", self.http_url_alt)
             assert len(http.pools) == 1
 
             for x in range(2):
-                http.urlopen("GET", self.https_url)
+                with pytest.warns(InsecureRequestWarning):
+                    http.urlopen("GET", self.https_url)
             assert len(http.pools) == 2
 
             for x in range(2):
-                http.urlopen("GET", self.https_url_alt)
+                with pytest.warns(InsecureRequestWarning):
+                    http.urlopen("GET", self.https_url_alt)
             assert len(http.pools) == 3
 
     def test_proxy_pooling_ext(self) -> None:
         with proxy_from_url(self.proxy_url) as http:
             hc1 = http.connection_from_url(self.http_url)
             hc2 = http.connection_from_host(self.http_host, self.http_port)
             hc3 = http.connection_from_url(self.http_url_alt)
```

### Comparing `urllib3-2.0.0a3/test/with_dummyserver/test_socketlevel.py` & `urllib3-2.0.0a4/test/with_dummyserver/test_socketlevel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # TODO: Break this module up into pieces. Maybe group by functionality tested
 # rather than the socket level-ness of it.
 from __future__ import annotations
 
+import contextlib
 import errno
 import io
 import os
 import os.path
 import select
 import shutil
 import socket
@@ -38,14 +39,15 @@
 )
 from dummyserver.testcase import SocketDummyServerTestCase, consume_socket
 from urllib3 import HTTPConnectionPool, HTTPSConnectionPool, ProxyManager, util
 from urllib3._collections import HTTPHeaderDict
 from urllib3.connection import HTTPConnection, _get_default_user_agent
 from urllib3.connectionpool import _url_from_pool
 from urllib3.exceptions import (
+    InsecureRequestWarning,
     MaxRetryError,
     ProtocolError,
     ProxyError,
     ReadTimeoutError,
     SSLError,
 )
 from urllib3.poolmanager import proxy_from_url
@@ -962,14 +964,71 @@
             assert response.connection is not None
 
             # Consume the data. This should put the connection back.
             response.read()
             assert pool.pool.qsize() == 1
             assert response.connection is None
 
+    def test_socket_close_socket_then_file(self) -> None:
+        def consume_ssl_socket(listener: socket.socket) -> None:
+            try:
+                with listener.accept()[0] as sock, original_ssl_wrap_socket(
+                    sock,
+                    server_side=True,
+                    keyfile=DEFAULT_CERTS["keyfile"],
+                    certfile=DEFAULT_CERTS["certfile"],
+                    ca_certs=DEFAULT_CA,
+                ) as ssl_sock:
+                    consume_socket(ssl_sock)
+            except (ConnectionResetError, ConnectionAbortedError, OSError):
+                pass
+
+        self._start_server(consume_ssl_socket)
+        with socket.create_connection(
+            (self.host, self.port)
+        ) as sock, contextlib.closing(
+            ssl_wrap_socket(sock, server_hostname=self.host, ca_certs=DEFAULT_CA)
+        ) as ssl_sock, ssl_sock.makefile(
+            "rb"
+        ) as f:
+            ssl_sock.close()
+            f.close()
+            # SecureTransport is supposed to raise OSError but raises
+            # ssl.SSLError when closed because ssl_sock.context is None
+            with pytest.raises((OSError, ssl.SSLError)):
+                ssl_sock.sendall(b"hello")
+            assert ssl_sock.fileno() == -1
+
+    def test_socket_close_stays_open_with_makefile_open(self) -> None:
+        def consume_ssl_socket(listener: socket.socket) -> None:
+            try:
+                with listener.accept()[0] as sock, original_ssl_wrap_socket(
+                    sock,
+                    server_side=True,
+                    keyfile=DEFAULT_CERTS["keyfile"],
+                    certfile=DEFAULT_CERTS["certfile"],
+                    ca_certs=DEFAULT_CA,
+                ) as ssl_sock:
+                    consume_socket(ssl_sock)
+            except (ConnectionResetError, ConnectionAbortedError, OSError):
+                pass
+
+        self._start_server(consume_ssl_socket)
+        with socket.create_connection(
+            (self.host, self.port)
+        ) as sock, contextlib.closing(
+            ssl_wrap_socket(sock, server_hostname=self.host, ca_certs=DEFAULT_CA)
+        ) as ssl_sock, ssl_sock.makefile(
+            "rb"
+        ):
+            ssl_sock.close()
+            ssl_sock.close()
+            ssl_sock.sendall(b"hello")
+            assert ssl_sock.fileno() > 0
+
 
 class TestProxyManager(SocketDummyServerTestCase):
     def test_simple(self) -> None:
         def echo_socket_handler(listener: socket.socket) -> None:
             sock = listener.accept()[0]
 
             buf = b""
@@ -1184,24 +1243,24 @@
         self._start_server(echo_socket_handler)
         base_url = f"http://{self.host}:{self.port}"
 
         with proxy_from_url(base_url, cert_reqs="NONE") as proxy:
             url = f"https://[{ipv6_addr}]"
             conn = proxy.connection_from_url(url)
             try:
-                r = conn.urlopen("GET", url, retries=0)
+                with pytest.warns(InsecureRequestWarning):
+                    r = conn.urlopen("GET", url, retries=0)
                 assert r.status == 200
             except MaxRetryError:
                 pytest.fail("Invalid IPv6 format in HTTP CONNECT request")
 
     @pytest.mark.parametrize("target_scheme", ["http", "https"])
     def test_https_proxymanager_connected_to_http_proxy(
         self, target_scheme: str
     ) -> None:
-
         errored = Event()
 
         def http_socket_handler(listener: socket.socket) -> None:
             sock = listener.accept()[0]
             sock.send(b"HTTP/1.0 501 Not Implemented\r\nConnection: close\r\n\r\n")
             errored.wait()
             sock.close()
@@ -1260,14 +1319,16 @@
 
     @notSecureTransport()
     def test_ssl_read_timeout(self) -> None:
         timed_out = Event()
 
         def socket_handler(listener: socket.socket) -> None:
             sock = listener.accept()[0]
+            # disable Nagle's algorithm so there's no delay in sending a partial body
+            sock.setsockopt(socket.IPPROTO_TCP, socket.TCP_NODELAY, True)
             ssl_sock = original_ssl_wrap_socket(
                 sock,
                 server_side=True,
                 keyfile=DEFAULT_CERTS["keyfile"],
                 certfile=DEFAULT_CERTS["certfile"],
             )
 
@@ -1478,15 +1539,14 @@
         with mock.patch("urllib3.util.ssl_.SSLContext", lambda *_, **__: context):
             for kwargs in [
                 {"ca_certs": "/a"},
                 {"ca_cert_dir": "/a"},
                 {"ca_certs": "a", "ca_cert_dir": "a"},
                 {"ssl_context": context},
             ]:
-
                 self._start_server(socket_handler)
 
                 with HTTPSConnectionPool(self.host, self.port, **kwargs) as pool:
                     with pytest.raises(Exception):
                         pool.request("GET", "/", timeout=SHORT_TIMEOUT)
                     context.load_default_certs.assert_not_called()
```

### Comparing `urllib3-2.0.0a3/LICENSE.txt` & `urllib3-2.0.0a4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a3/README.md` & `urllib3-2.0.0a4/README.md`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a3/pyproject.toml` & `urllib3-2.0.0a4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -83,18 +83,14 @@
 markers = ["limit_memory"]
 log_level = "DEBUG"
 filterwarnings = [
     "error",
     '''default:'urllib3\[secure\]' extra is deprecated and will be removed in urllib3 v2\.1\.0.*:DeprecationWarning''',
     '''default:'urllib3\.contrib\.pyopenssl' module is deprecated and will be removed in urllib3 v2\.1\.0.*:DeprecationWarning''',
     '''default:'urllib3\.contrib\.securetransport' module is deprecated and will be removed in urllib3 v2\.1\.0.*:DeprecationWarning''',
-    '''default:distutils Version classes are deprecated\. Use packaging\.version instead\.:DeprecationWarning''',
-    '''default:The 'pool' property is deprecated and will be removed in urllib3 v2\.1\.0\. use 'conn' instead:DeprecationWarning''',
-    '''default:'ssl_version' option is deprecated and will be removed in urllib3 v2\.1\.0\. Instead use 'ssl_minimum_version':DeprecationWarning''',
-    '''default:.*:urllib3.exceptions.InsecureRequestWarning''',
     '''default:No IPv6 support. Falling back to IPv4:urllib3.exceptions.HTTPWarning''',
     '''default:No IPv6 support. skipping:urllib3.exceptions.HTTPWarning''',
     '''default:ssl\.TLSVersion\.TLSv1 is deprecated:DeprecationWarning''',
     '''default:ssl\.PROTOCOL_TLS is deprecated:DeprecationWarning''',
     '''default:ssl\.PROTOCOL_TLSv1 is deprecated:DeprecationWarning''',
     '''default:ssl\.TLSVersion\.TLSv1_1 is deprecated:DeprecationWarning''',
     '''default:ssl\.PROTOCOL_TLSv1_1 is deprecated:DeprecationWarning''',
@@ -102,15 +98,14 @@
     '''default:unclosed .*:ResourceWarning''',
     '''default:ssl NPN is deprecated, use ALPN instead:DeprecationWarning''',
 ]
 
 [tool.isort]
 profile = "black"
 add_imports = "from __future__ import annotations"
-skip = ["setup.py"]
 
 [tool.mypy]
 mypy_path = "src"
 check_untyped_defs = true
 disallow_any_generics = true
 disallow_incomplete_defs = true
 disallow_subclassing_any = true
```

### Comparing `urllib3-2.0.0a3/PKG-INFO` & `urllib3-2.0.0a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: urllib3
-Version: 2.0.0a3
+Version: 2.0.0a4
 Summary: HTTP library with thread-safe connection pooling, file post, and more.
 Project-URL: Changelog, https://github.com/urllib3/urllib3/blob/main/CHANGES.rst
 Project-URL: Documentation, https://urllib3.readthedocs.io
 Project-URL: Code, https://github.com/urllib3/urllib3
 Project-URL: Issue tracker, https://github.com/urllib3/urllib3/issues
 Author-email: Andrey Petrov <andrey.petrov@shazow.net>
 Maintainer-email: Seth Michael Larson <sethmichaellarson@gmail.com>, Quentin Pradet <quentin@pradet.me>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: urllib3 Version: 2.0.0a3 Summary: HTTP library with
+Metadata-Version: 2.1 Name: urllib3 Version: 2.0.0a4 Summary: HTTP library with
 thread-safe connection pooling, file post, and more. Project-URL: Changelog,
 https://github.com/urllib3/urllib3/blob/main/CHANGES.rst Project-URL:
 Documentation, https://urllib3.readthedocs.io Project-URL: Code, https://
 github.com/urllib3/urllib3 Project-URL: Issue tracker, https://github.com/
 urllib3/urllib3/issues Author-email: Andrey Petrov
 petrov@shazow.net> Maintainer-email: Seth Michael Larson
 gmail.com>, Quentin Pradet
```

