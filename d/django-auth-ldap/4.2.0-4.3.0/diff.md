# Comparing `tmp/django-auth-ldap-4.2.0.tar.gz` & `tmp/django-auth-ldap-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-auth-ldap-4.2.0.tar", last modified: Tue Mar 28 09:48:48 2023, max compression
+gzip compressed data, was "django-auth-ldap-4.3.0.tar", last modified: Wed Apr 26 19:45:49 2023, max compression
```

## Comparing `django-auth-ldap-4.2.0.tar` & `django-auth-ldap-4.3.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-03-28 09:48:48.396923 django-auth-ldap-4.2.0/
--rw-------   0 freitafr  (1000) freitafr  (1000)     1297 2020-12-14 12:14:26.000000 django-auth-ldap-4.2.0/LICENSE
--rw-------   0 freitafr  (1000) freitafr  (1000)       64 2023-03-28 09:44:55.000000 django-auth-ldap-4.2.0/MANIFEST.in
--rw-------   0 freitafr  (1000) freitafr  (1000)     7034 2023-03-28 09:48:48.396923 django-auth-ldap-4.2.0/PKG-INFO
--rw-------   0 freitafr  (1000) freitafr  (1000)     5484 2022-08-16 11:46:04.000000 django-auth-ldap-4.2.0/README.rst
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-03-28 09:48:48.396923 django-auth-ldap-4.2.0/django_auth_ldap/
--rw-------   0 freitafr  (1000) freitafr  (1000)      113 2021-05-05 13:49:26.000000 django-auth-ldap-4.2.0/django_auth_ldap/__init__.py
--rw-------   0 freitafr  (1000) freitafr  (1000)    32422 2022-06-13 12:14:29.000000 django-auth-ldap-4.2.0/django_auth_ldap/backend.py
--rw-------   0 freitafr  (1000) freitafr  (1000)    24980 2022-06-13 12:14:29.000000 django-auth-ldap-4.2.0/django_auth_ldap/config.py
--rw-------   0 freitafr  (1000) freitafr  (1000)      160 2023-03-28 09:48:48.000000 django-auth-ldap-4.2.0/django_auth_ldap/version.py
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-03-28 09:48:48.396923 django-auth-ldap-4.2.0/django_auth_ldap.egg-info/
--rw-------   0 freitafr  (1000) freitafr  (1000)     7034 2023-03-28 09:48:48.000000 django-auth-ldap-4.2.0/django_auth_ldap.egg-info/PKG-INFO
--rw-------   0 freitafr  (1000) freitafr  (1000)      793 2023-03-28 09:48:48.000000 django-auth-ldap-4.2.0/django_auth_ldap.egg-info/SOURCES.txt
--rw-------   0 freitafr  (1000) freitafr  (1000)        1 2023-03-28 09:48:48.000000 django-auth-ldap-4.2.0/django_auth_ldap.egg-info/dependency_links.txt
--rw-------   0 freitafr  (1000) freitafr  (1000)       29 2023-03-28 09:48:48.000000 django-auth-ldap-4.2.0/django_auth_ldap.egg-info/requires.txt
--rw-------   0 freitafr  (1000) freitafr  (1000)       17 2023-03-28 09:48:48.000000 django-auth-ldap-4.2.0/django_auth_ldap.egg-info/top_level.txt
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-03-28 09:48:48.396923 django-auth-ldap-4.2.0/docs/
--rw-------   0 freitafr  (1000) freitafr  (1000)      620 2020-12-14 12:14:26.000000 django-auth-ldap-4.2.0/docs/Makefile
--rw-------   0 freitafr  (1000) freitafr  (1000)     7313 2021-05-05 13:49:22.000000 django-auth-ldap-4.2.0/docs/authentication.rst
--rw-------   0 freitafr  (1000) freitafr  (1000)     8558 2022-01-12 14:50:13.000000 django-auth-ldap-4.2.0/docs/changes.rst
--rw-------   0 freitafr  (1000) freitafr  (1000)     5920 2022-06-13 12:14:29.000000 django-auth-ldap-4.2.0/docs/conf.py
--rw-------   0 freitafr  (1000) freitafr  (1000)      969 2023-03-28 09:38:27.000000 django-auth-ldap-4.2.0/docs/contributing.rst
--rw-------   0 freitafr  (1000) freitafr  (1000)     5051 2021-02-15 09:20:44.000000 django-auth-ldap-4.2.0/docs/custombehavior.rst
--rw-------   0 freitafr  (1000) freitafr  (1000)     2462 2021-02-15 09:20:44.000000 django-auth-ldap-4.2.0/docs/example.rst
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-03-28 09:48:48.396923 django-auth-ldap-4.2.0/docs/ext/
--rw-------   0 freitafr  (1000) freitafr  (1000)      196 2020-12-14 12:14:26.000000 django-auth-ldap-4.2.0/docs/ext/daldocs.py
--rw-------   0 freitafr  (1000) freitafr  (1000)     4248 2021-02-15 09:20:44.000000 django-auth-ldap-4.2.0/docs/groups.rst
--rw-------   0 freitafr  (1000) freitafr  (1000)      966 2022-06-13 12:14:29.000000 django-auth-ldap-4.2.0/docs/index.rst
--rw-------   0 freitafr  (1000) freitafr  (1000)     1591 2021-10-20 09:01:15.000000 django-auth-ldap-4.2.0/docs/install.rst
--rw-------   0 freitafr  (1000) freitafr  (1000)      639 2021-02-15 09:20:44.000000 django-auth-ldap-4.2.0/docs/logging.rst
--rw-------   0 freitafr  (1000) freitafr  (1000)     1748 2021-02-15 09:20:44.000000 django-auth-ldap-4.2.0/docs/multiconfig.rst
--rw-------   0 freitafr  (1000) freitafr  (1000)     1687 2020-12-14 12:14:26.000000 django-auth-ldap-4.2.0/docs/performance.rst
--rw-------   0 freitafr  (1000) freitafr  (1000)     3940 2020-12-14 12:14:26.000000 django-auth-ldap-4.2.0/docs/permissions.rst
--rw-------   0 freitafr  (1000) freitafr  (1000)    20968 2021-09-16 14:26:42.000000 django-auth-ldap-4.2.0/docs/reference.rst
--rw-------   0 freitafr  (1000) freitafr  (1000)       15 2021-05-05 13:49:26.000000 django-auth-ldap-4.2.0/docs/requirements.txt
--rw-------   0 freitafr  (1000) freitafr  (1000)     6560 2021-02-15 09:20:44.000000 django-auth-ldap-4.2.0/docs/users.rst
--rw-------   0 freitafr  (1000) freitafr  (1000)      189 2023-03-28 09:38:27.000000 django-auth-ldap-4.2.0/pyproject.toml
--rw-------   0 freitafr  (1000) freitafr  (1000)     1511 2023-03-28 09:48:48.396923 django-auth-ldap-4.2.0/setup.cfg
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-03-28 09:48:48.396923 django-auth-ldap-4.2.0/tests/
--rw-------   0 freitafr  (1000) freitafr  (1000)        0 2020-12-14 12:14:26.000000 django-auth-ldap-4.2.0/tests/__init__.py
--rw-------   0 freitafr  (1000) freitafr  (1000)      581 2021-02-15 09:20:44.000000 django-auth-ldap-4.2.0/tests/models.py
--rw-------   0 freitafr  (1000) freitafr  (1000)      322 2021-05-05 13:49:26.000000 django-auth-ldap-4.2.0/tests/settings.py
--rw-------   0 freitafr  (1000) freitafr  (1000)     4037 2020-12-14 12:14:26.000000 django-auth-ldap-4.2.0/tests/tests.ldif
--rw-------   0 freitafr  (1000) freitafr  (1000)    61622 2022-08-16 10:13:05.000000 django-auth-ldap-4.2.0/tests/tests.py
--rw-------   0 freitafr  (1000) freitafr  (1000)      920 2023-03-28 09:38:27.000000 django-auth-ldap-4.2.0/tox.ini
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 19:45:49.770546 django-auth-ldap-4.3.0/
+-rw-------   0 freitafr  (1000) freitafr  (1000)     1297 2020-12-14 12:14:26.000000 django-auth-ldap-4.3.0/LICENSE
+-rw-------   0 freitafr  (1000) freitafr  (1000)       64 2023-03-28 09:44:55.000000 django-auth-ldap-4.3.0/MANIFEST.in
+-rw-------   0 freitafr  (1000) freitafr  (1000)     7121 2023-04-26 19:45:49.770546 django-auth-ldap-4.3.0/PKG-INFO
+-rw-------   0 freitafr  (1000) freitafr  (1000)     5484 2022-08-16 11:46:04.000000 django-auth-ldap-4.3.0/README.rst
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 19:45:49.767212 django-auth-ldap-4.3.0/django_auth_ldap/
+-rw-------   0 freitafr  (1000) freitafr  (1000)      113 2021-05-05 13:49:26.000000 django-auth-ldap-4.3.0/django_auth_ldap/__init__.py
+-rw-------   0 freitafr  (1000) freitafr  (1000)    32422 2022-06-13 12:14:29.000000 django-auth-ldap-4.3.0/django_auth_ldap/backend.py
+-rw-------   0 freitafr  (1000) freitafr  (1000)    24980 2022-06-13 12:14:29.000000 django-auth-ldap-4.3.0/django_auth_ldap/config.py
+-rw-------   0 freitafr  (1000) freitafr  (1000)      160 2023-04-26 19:45:49.000000 django-auth-ldap-4.3.0/django_auth_ldap/version.py
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 19:45:49.767212 django-auth-ldap-4.3.0/django_auth_ldap.egg-info/
+-rw-------   0 freitafr  (1000) freitafr  (1000)     7121 2023-04-26 19:45:49.000000 django-auth-ldap-4.3.0/django_auth_ldap.egg-info/PKG-INFO
+-rw-------   0 freitafr  (1000) freitafr  (1000)      793 2023-04-26 19:45:49.000000 django-auth-ldap-4.3.0/django_auth_ldap.egg-info/SOURCES.txt
+-rw-------   0 freitafr  (1000) freitafr  (1000)        1 2023-04-26 19:45:49.000000 django-auth-ldap-4.3.0/django_auth_ldap.egg-info/dependency_links.txt
+-rw-------   0 freitafr  (1000) freitafr  (1000)       29 2023-04-26 19:45:49.000000 django-auth-ldap-4.3.0/django_auth_ldap.egg-info/requires.txt
+-rw-------   0 freitafr  (1000) freitafr  (1000)       17 2023-04-26 19:45:49.000000 django-auth-ldap-4.3.0/django_auth_ldap.egg-info/top_level.txt
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 19:45:49.770546 django-auth-ldap-4.3.0/docs/
+-rw-------   0 freitafr  (1000) freitafr  (1000)      620 2020-12-14 12:14:26.000000 django-auth-ldap-4.3.0/docs/Makefile
+-rw-------   0 freitafr  (1000) freitafr  (1000)     7313 2021-05-05 13:49:22.000000 django-auth-ldap-4.3.0/docs/authentication.rst
+-rw-------   0 freitafr  (1000) freitafr  (1000)     8558 2022-01-12 14:50:13.000000 django-auth-ldap-4.3.0/docs/changes.rst
+-rw-------   0 freitafr  (1000) freitafr  (1000)     5920 2022-06-13 12:14:29.000000 django-auth-ldap-4.3.0/docs/conf.py
+-rw-------   0 freitafr  (1000) freitafr  (1000)      969 2023-03-28 09:38:27.000000 django-auth-ldap-4.3.0/docs/contributing.rst
+-rw-------   0 freitafr  (1000) freitafr  (1000)     5051 2021-02-15 09:20:44.000000 django-auth-ldap-4.3.0/docs/custombehavior.rst
+-rw-------   0 freitafr  (1000) freitafr  (1000)     2462 2021-02-15 09:20:44.000000 django-auth-ldap-4.3.0/docs/example.rst
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 19:45:49.770546 django-auth-ldap-4.3.0/docs/ext/
+-rw-------   0 freitafr  (1000) freitafr  (1000)      196 2020-12-14 12:14:26.000000 django-auth-ldap-4.3.0/docs/ext/daldocs.py
+-rw-------   0 freitafr  (1000) freitafr  (1000)     4248 2021-02-15 09:20:44.000000 django-auth-ldap-4.3.0/docs/groups.rst
+-rw-------   0 freitafr  (1000) freitafr  (1000)      966 2022-06-13 12:14:29.000000 django-auth-ldap-4.3.0/docs/index.rst
+-rw-------   0 freitafr  (1000) freitafr  (1000)     1591 2021-10-20 09:01:15.000000 django-auth-ldap-4.3.0/docs/install.rst
+-rw-------   0 freitafr  (1000) freitafr  (1000)      639 2021-02-15 09:20:44.000000 django-auth-ldap-4.3.0/docs/logging.rst
+-rw-------   0 freitafr  (1000) freitafr  (1000)     1748 2021-02-15 09:20:44.000000 django-auth-ldap-4.3.0/docs/multiconfig.rst
+-rw-------   0 freitafr  (1000) freitafr  (1000)     1687 2020-12-14 12:14:26.000000 django-auth-ldap-4.3.0/docs/performance.rst
+-rw-------   0 freitafr  (1000) freitafr  (1000)     3940 2020-12-14 12:14:26.000000 django-auth-ldap-4.3.0/docs/permissions.rst
+-rw-------   0 freitafr  (1000) freitafr  (1000)    20968 2021-09-16 14:26:42.000000 django-auth-ldap-4.3.0/docs/reference.rst
+-rw-------   0 freitafr  (1000) freitafr  (1000)       15 2021-05-05 13:49:26.000000 django-auth-ldap-4.3.0/docs/requirements.txt
+-rw-------   0 freitafr  (1000) freitafr  (1000)     6560 2021-02-15 09:20:44.000000 django-auth-ldap-4.3.0/docs/users.rst
+-rw-------   0 freitafr  (1000) freitafr  (1000)      189 2023-03-28 09:38:27.000000 django-auth-ldap-4.3.0/pyproject.toml
+-rw-------   0 freitafr  (1000) freitafr  (1000)     1587 2023-04-26 19:45:49.770546 django-auth-ldap-4.3.0/setup.cfg
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 19:45:49.770546 django-auth-ldap-4.3.0/tests/
+-rw-------   0 freitafr  (1000) freitafr  (1000)        0 2020-12-14 12:14:26.000000 django-auth-ldap-4.3.0/tests/__init__.py
+-rw-------   0 freitafr  (1000) freitafr  (1000)      581 2021-02-15 09:20:44.000000 django-auth-ldap-4.3.0/tests/models.py
+-rw-------   0 freitafr  (1000) freitafr  (1000)      322 2021-05-05 13:49:26.000000 django-auth-ldap-4.3.0/tests/settings.py
+-rw-------   0 freitafr  (1000) freitafr  (1000)     4037 2020-12-14 12:14:26.000000 django-auth-ldap-4.3.0/tests/tests.ldif
+-rw-------   0 freitafr  (1000) freitafr  (1000)    61622 2022-08-16 10:13:05.000000 django-auth-ldap-4.3.0/tests/tests.py
+-rw-------   0 freitafr  (1000) freitafr  (1000)      920 2023-04-26 19:31:31.000000 django-auth-ldap-4.3.0/tox.ini
```

### Comparing `django-auth-ldap-4.2.0/LICENSE` & `django-auth-ldap-4.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-auth-ldap-4.2.0/PKG-INFO` & `django-auth-ldap-4.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: django-auth-ldap
-Version: 4.2.0
+Version: 4.3.0
 Summary: Django LDAP authentication backend.
 Home-page: https://github.com/django-auth-ldap/django-auth-ldap
 Author: Peter Sagerson
 Author-email: psagers@ignorare.net
 License: BSD
 Project-URL: Documentation, https://django-auth-ldap.readthedocs.io/
 Project-URL: Source, https://github.com/django-auth-ldap/django-auth-ldap
 Project-URL: Tracker, https://github.com/django-auth-ldap/django-auth-ldap/issues
+Project-URL: Changelog, https://github.com/django-auth-ldap/django-auth-ldap/releases/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `django-auth-ldap-4.2.0/README.rst` & `django-auth-ldap-4.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `django-auth-ldap-4.2.0/django_auth_ldap/backend.py` & `django-auth-ldap-4.3.0/django_auth_ldap/backend.py`

 * *Files identical despite different names*

### Comparing `django-auth-ldap-4.2.0/django_auth_ldap/config.py` & `django-auth-ldap-4.3.0/django_auth_ldap/config.py`

 * *Files identical despite different names*

### Comparing `django-auth-ldap-4.2.0/django_auth_ldap.egg-info/PKG-INFO` & `django-auth-ldap-4.3.0/django_auth_ldap.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: django-auth-ldap
-Version: 4.2.0
+Version: 4.3.0
 Summary: Django LDAP authentication backend.
 Home-page: https://github.com/django-auth-ldap/django-auth-ldap
 Author: Peter Sagerson
 Author-email: psagers@ignorare.net
 License: BSD
 Project-URL: Documentation, https://django-auth-ldap.readthedocs.io/
 Project-URL: Source, https://github.com/django-auth-ldap/django-auth-ldap
 Project-URL: Tracker, https://github.com/django-auth-ldap/django-auth-ldap/issues
+Project-URL: Changelog, https://github.com/django-auth-ldap/django-auth-ldap/releases/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `django-auth-ldap-4.2.0/django_auth_ldap.egg-info/SOURCES.txt` & `django-auth-ldap-4.3.0/django_auth_ldap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-auth-ldap-4.2.0/docs/Makefile` & `django-auth-ldap-4.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-auth-ldap-4.2.0/docs/authentication.rst` & `django-auth-ldap-4.3.0/docs/authentication.rst`

 * *Files identical despite different names*

### Comparing `django-auth-ldap-4.2.0/docs/changes.rst` & `django-auth-ldap-4.3.0/docs/changes.rst`

 * *Files identical despite different names*

### Comparing `django-auth-ldap-4.2.0/docs/conf.py` & `django-auth-ldap-4.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django-auth-ldap-4.2.0/docs/contributing.rst` & `django-auth-ldap-4.3.0/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `django-auth-ldap-4.2.0/docs/custombehavior.rst` & `django-auth-ldap-4.3.0/docs/custombehavior.rst`

 * *Files identical despite different names*

### Comparing `django-auth-ldap-4.2.0/docs/example.rst` & `django-auth-ldap-4.3.0/docs/example.rst`

 * *Files identical despite different names*

### Comparing `django-auth-ldap-4.2.0/docs/groups.rst` & `django-auth-ldap-4.3.0/docs/groups.rst`

 * *Files identical despite different names*

### Comparing `django-auth-ldap-4.2.0/docs/index.rst` & `django-auth-ldap-4.3.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `django-auth-ldap-4.2.0/docs/install.rst` & `django-auth-ldap-4.3.0/docs/install.rst`

 * *Files identical despite different names*

### Comparing `django-auth-ldap-4.2.0/docs/logging.rst` & `django-auth-ldap-4.3.0/docs/logging.rst`

 * *Files identical despite different names*

### Comparing `django-auth-ldap-4.2.0/docs/multiconfig.rst` & `django-auth-ldap-4.3.0/docs/multiconfig.rst`

 * *Files identical despite different names*

### Comparing `django-auth-ldap-4.2.0/docs/performance.rst` & `django-auth-ldap-4.3.0/docs/performance.rst`

 * *Files identical despite different names*

### Comparing `django-auth-ldap-4.2.0/docs/permissions.rst` & `django-auth-ldap-4.3.0/docs/permissions.rst`

 * *Files identical despite different names*

### Comparing `django-auth-ldap-4.2.0/docs/reference.rst` & `django-auth-ldap-4.3.0/docs/reference.rst`

 * *Files identical despite different names*

### Comparing `django-auth-ldap-4.2.0/docs/users.rst` & `django-auth-ldap-4.3.0/docs/users.rst`

 * *Files identical despite different names*

### Comparing `django-auth-ldap-4.2.0/setup.cfg` & `django-auth-ldap-4.3.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 url = https://github.com/django-auth-ldap/django-auth-ldap
 license = BSD
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Environment :: Web Environment
 	Framework :: Django
 	Framework :: Django :: 3.2
-	Framework :: Django :: 4.0
 	Framework :: Django :: 4.1
+	Framework :: Django :: 4.2
 	Intended Audience :: Developers
 	Intended Audience :: System Administrators
 	License :: OSI Approved :: BSD License
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.7
@@ -28,14 +28,15 @@
 	Topic :: Internet :: WWW/HTTP
 	Topic :: Software Development :: Libraries :: Python Modules
 	Topic :: System :: Systems Administration :: Authentication/Directory :: LDAP
 project_urls = 
 	Documentation = https://django-auth-ldap.readthedocs.io/
 	Source = https://github.com/django-auth-ldap/django-auth-ldap
 	Tracker = https://github.com/django-auth-ldap/django-auth-ldap/issues
+	Changelog = https://github.com/django-auth-ldap/django-auth-ldap/releases/
 
 [options]
 python_requires = >=3.7
 packages = django_auth_ldap
 install_requires = 
 	Django>=3.2
 	python-ldap>=3.1
```

### Comparing `django-auth-ldap-4.2.0/tests/models.py` & `django-auth-ldap-4.3.0/tests/models.py`

 * *Files identical despite different names*

### Comparing `django-auth-ldap-4.2.0/tests/tests.ldif` & `django-auth-ldap-4.3.0/tests/tests.ldif`

 * *Files identical despite different names*

### Comparing `django-auth-ldap-4.2.0/tests/tests.py` & `django-auth-ldap-4.3.0/tests/tests.py`

 * *Files identical despite different names*

### Comparing `django-auth-ldap-4.2.0/tox.ini` & `django-auth-ldap-4.3.0/tox.ini`

 * *Files 21% similar despite different names*

```diff
@@ -10,16 +10,16 @@
     djangomain
 isolated_build = true
 
 [testenv]
 commands = {envpython} -Wa -b -m django test --settings tests.settings
 deps =
     django32: Django>=3.2,<4.0
-    django40: Django>=4.0,<4.1
     django41: Django>=4.1,<4.2
+    django42: Django>=4.2,<4.3
     djangomain: https://github.com/django/django/archive/main.tar.gz
 
 [testenv:black]
 deps = black
 commands = black --check --diff .
 skip_install = true
```

