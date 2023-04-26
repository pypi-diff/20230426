# Comparing `tmp/ocp-sso-token-1.1.0.tar.gz` & `tmp/ocp-sso-token-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocp-sso-token-1.1.0.tar", last modified: Wed Apr 26 11:26:03 2023, max compression
+gzip compressed data, was "ocp-sso-token-1.2.0.tar", last modified: Wed Apr 26 12:53:24 2023, max compression
```

## Comparing `ocp-sso-token-1.1.0.tar` & `ocp-sso-token-1.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 11:26:03.828873 ocp-sso-token-1.1.0/
--rw-rw-rw-   0 root         (0) root         (0)    35079 2023-04-26 11:25:52.000000 ocp-sso-token-1.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     8733 2023-04-26 11:26:03.828873 ocp-sso-token-1.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     8372 2023-04-26 11:25:52.000000 ocp-sso-token-1.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 11:26:03.824873 ocp-sso-token-1.1.0/ocp_sso_token/
--rw-rw-rw-   0 root         (0) root         (0)       93 2023-04-26 11:25:52.000000 ocp-sso-token-1.1.0/ocp_sso_token/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1633 2023-04-26 11:25:52.000000 ocp-sso-token-1.1.0/ocp_sso_token/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)     3389 2023-04-26 11:25:52.000000 ocp-sso-token-1.1.0/ocp_sso_token/kube_config.py
--rw-rw-rw-   0 root         (0) root         (0)     2726 2023-04-26 11:25:52.000000 ocp-sso-token-1.1.0/ocp_sso_token/ocp_oauth_login.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 11:26:03.827873 ocp-sso-token-1.1.0/ocp_sso_token.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8733 2023-04-26 11:26:03.000000 ocp-sso-token-1.1.0/ocp_sso_token.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      449 2023-04-26 11:26:03.000000 ocp-sso-token-1.1.0/ocp_sso_token.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 11:26:03.000000 ocp-sso-token-1.1.0/ocp_sso_token.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2023-04-26 11:26:03.000000 ocp-sso-token-1.1.0/ocp_sso_token.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      129 2023-04-26 11:26:03.000000 ocp-sso-token-1.1.0/ocp_sso_token.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-04-26 11:26:03.000000 ocp-sso-token-1.1.0/ocp_sso_token.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1019 2023-04-26 11:26:03.829874 ocp-sso-token-1.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       82 2023-04-26 11:25:52.000000 ocp-sso-token-1.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 11:26:03.828873 ocp-sso-token-1.1.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)    20456 2023-04-26 11:25:52.000000 ocp-sso-token-1.1.0/tests/test_kube_config.py
--rw-rw-rw-   0 root         (0) root         (0)     2397 2023-04-26 11:25:52.000000 ocp-sso-token-1.1.0/tests/test_main.py
--rw-rw-rw-   0 root         (0) root         (0)     1699 2023-04-26 11:25:52.000000 ocp-sso-token-1.1.0/tests/test_ocp_oauth_login.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:53:24.820193 ocp-sso-token-1.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)    35079 2023-04-26 12:53:13.000000 ocp-sso-token-1.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     8733 2023-04-26 12:53:24.820193 ocp-sso-token-1.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     8372 2023-04-26 12:53:13.000000 ocp-sso-token-1.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:53:24.817193 ocp-sso-token-1.2.0/ocp_sso_token/
+-rw-rw-rw-   0 root         (0) root         (0)       93 2023-04-26 12:53:13.000000 ocp-sso-token-1.2.0/ocp_sso_token/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1633 2023-04-26 12:53:13.000000 ocp-sso-token-1.2.0/ocp_sso_token/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3389 2023-04-26 12:53:13.000000 ocp-sso-token-1.2.0/ocp_sso_token/kube_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2726 2023-04-26 12:53:13.000000 ocp-sso-token-1.2.0/ocp_sso_token/ocp_oauth_login.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:53:24.819193 ocp-sso-token-1.2.0/ocp_sso_token.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8733 2023-04-26 12:53:24.000000 ocp-sso-token-1.2.0/ocp_sso_token.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      449 2023-04-26 12:53:24.000000 ocp-sso-token-1.2.0/ocp_sso_token.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 12:53:24.000000 ocp-sso-token-1.2.0/ocp_sso_token.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-04-26 12:53:24.000000 ocp-sso-token-1.2.0/ocp_sso_token.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      129 2023-04-26 12:53:24.000000 ocp-sso-token-1.2.0/ocp_sso_token.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-04-26 12:53:24.000000 ocp-sso-token-1.2.0/ocp_sso_token.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1019 2023-04-26 12:53:24.821193 ocp-sso-token-1.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       82 2023-04-26 12:53:13.000000 ocp-sso-token-1.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:53:24.820193 ocp-sso-token-1.2.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)    20456 2023-04-26 12:53:13.000000 ocp-sso-token-1.2.0/tests/test_kube_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2397 2023-04-26 12:53:13.000000 ocp-sso-token-1.2.0/tests/test_main.py
+-rw-rw-rw-   0 root         (0) root         (0)     1699 2023-04-26 12:53:13.000000 ocp-sso-token-1.2.0/tests/test_ocp_oauth_login.py
```

### Comparing `ocp-sso-token-1.1.0/LICENSE` & `ocp-sso-token-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ocp-sso-token-1.1.0/PKG-INFO` & `ocp-sso-token-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocp-sso-token
-Version: 1.1.0
+Version: 1.2.0
 Summary: Obtain an OCP OAuth token for an SSO IdP with Kerberos support
 Home-page: https://gitlab.com/cki-project/ocp-sso-token
 Author: CKI Team
 Author-email: cki-project@redhat.com
 License: GPLv3
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `ocp-sso-token-1.1.0/README.md` & `ocp-sso-token-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ocp-sso-token-1.1.0/ocp_sso_token/__main__.py` & `ocp-sso-token-1.2.0/ocp_sso_token/__main__.py`

 * *Files identical despite different names*

### Comparing `ocp-sso-token-1.1.0/ocp_sso_token/kube_config.py` & `ocp-sso-token-1.2.0/ocp_sso_token/kube_config.py`

 * *Files identical despite different names*

### Comparing `ocp-sso-token-1.1.0/ocp_sso_token/ocp_oauth_login.py` & `ocp-sso-token-1.2.0/ocp_sso_token/ocp_oauth_login.py`

 * *Files identical despite different names*

### Comparing `ocp-sso-token-1.1.0/ocp_sso_token.egg-info/PKG-INFO` & `ocp-sso-token-1.2.0/ocp_sso_token.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocp-sso-token
-Version: 1.1.0
+Version: 1.2.0
 Summary: Obtain an OCP OAuth token for an SSO IdP with Kerberos support
 Home-page: https://gitlab.com/cki-project/ocp-sso-token
 Author: CKI Team
 Author-email: cki-project@redhat.com
 License: GPLv3
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `ocp-sso-token-1.1.0/setup.cfg` & `ocp-sso-token-1.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `ocp-sso-token-1.1.0/tests/test_kube_config.py` & `ocp-sso-token-1.2.0/tests/test_kube_config.py`

 * *Files identical despite different names*

### Comparing `ocp-sso-token-1.1.0/tests/test_main.py` & `ocp-sso-token-1.2.0/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `ocp-sso-token-1.1.0/tests/test_ocp_oauth_login.py` & `ocp-sso-token-1.2.0/tests/test_ocp_oauth_login.py`

 * *Files identical despite different names*

