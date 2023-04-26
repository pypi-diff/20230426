# Comparing `tmp/django-admin-csvexport-2.1.tar.gz` & `tmp/django-admin-csvexport-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/thomas/django/django-admin-csvexport/dist/.tmp-0j4zmh17/django-admin-csvexport-2.1.tar", last modified: Wed Mar 22 12:19:25 2023, max compression
+gzip compressed data, was "django-admin-csvexport-2.2.tar", last modified: Wed Apr 26 10:03:10 2023, max compression
```

## Comparing `django-admin-csvexport-2.1.tar` & `django-admin-csvexport-2.2.tar`

### file list

```diff
@@ -1,27 +1,48 @@
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-03-22 12:19:25.000000 django-admin-csvexport-2.1/
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1521 2020-08-31 18:53:49.000000 django-admin-csvexport-2.1/LICENCE
--rw-r--r--   0 thomas    (1000) thomas    (1000)      112 2021-01-11 14:56:37.000000 django-admin-csvexport-2.1/MANIFEST.in
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     5659 2023-03-22 12:19:25.000000 django-admin-csvexport-2.1/PKG-INFO
--rw-r--r--   0 thomas    (1000) thomas    (1000)     4348 2023-03-22 12:13:17.000000 django-admin-csvexport-2.1/README.rst
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-03-22 12:19:25.000000 django-admin-csvexport-2.1/csvexport/
--rw-r--r--   0 thomas    (1000) thomas    (1000)       59 2023-03-22 12:14:33.000000 django-admin-csvexport-2.1/csvexport/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     7645 2023-03-22 12:13:17.000000 django-admin-csvexport-2.1/csvexport/actions.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)       93 2020-08-31 18:53:49.000000 django-admin-csvexport-2.1/csvexport/apps.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     2929 2020-12-08 09:31:11.000000 django-admin-csvexport-2.1/csvexport/forms.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)      829 2023-03-22 12:11:12.000000 django-admin-csvexport-2.1/csvexport/settings.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-03-22 12:19:25.000000 django-admin-csvexport-2.1/csvexport/static/
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-03-22 12:19:25.000000 django-admin-csvexport-2.1/csvexport/static/csvexport/
--rw-r--r--   0 thomas    (1000) thomas    (1000)      375 2020-08-31 18:53:49.000000 django-admin-csvexport-2.1/csvexport/static/csvexport/checkbox_select_all.js
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-03-22 12:19:25.000000 django-admin-csvexport-2.1/csvexport/templates/
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-03-22 12:19:25.000000 django-admin-csvexport-2.1/csvexport/templates/csvexport/
--rw-r--r--   0 thomas    (1000) thomas    (1000)      223 2020-08-31 18:53:49.000000 django-admin-csvexport-2.1/csvexport/templates/csvexport/checkbox_select_all.html
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1050 2020-12-08 09:37:56.000000 django-admin-csvexport-2.1/csvexport/templates/csvexport/csvexport.html
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-03-22 12:19:25.000000 django-admin-csvexport-2.1/django_admin_csvexport.egg-info/
--rw-r--r--   0 thomas    (1000) thomas    (1000)     5659 2023-03-22 12:19:25.000000 django-admin-csvexport-2.1/django_admin_csvexport.egg-info/PKG-INFO
--rw-r--r--   0 thomas    (1000) thomas    (1000)      561 2023-03-22 12:19:25.000000 django-admin-csvexport-2.1/django_admin_csvexport.egg-info/SOURCES.txt
--rw-r--r--   0 thomas    (1000) thomas    (1000)        1 2023-03-22 12:19:25.000000 django-admin-csvexport-2.1/django_admin_csvexport.egg-info/dependency_links.txt
--rw-r--r--   0 thomas    (1000) thomas    (1000)       34 2023-03-22 12:19:25.000000 django-admin-csvexport-2.1/django_admin_csvexport.egg-info/requires.txt
--rw-r--r--   0 thomas    (1000) thomas    (1000)       10 2023-03-22 12:19:25.000000 django-admin-csvexport-2.1/django_admin_csvexport.egg-info/top_level.txt
--rw-r--r--   0 thomas    (1000) thomas    (1000)        1 2020-08-31 18:53:49.000000 django-admin-csvexport-2.1/django_admin_csvexport.egg-info/zip-safe
--rw-rw-r--   0 thomas    (1000) thomas    (1000)       38 2023-03-22 12:19:25.000000 django-admin-csvexport-2.1/setup.cfg
--rw-r--r--   0 thomas    (1000) thomas    (1000)     2040 2023-03-20 23:09:37.000000 django-admin-csvexport-2.1/setup.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-04-26 10:03:10.987725 django-admin-csvexport-2.2/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1521 2020-08-31 18:53:49.000000 django-admin-csvexport-2.2/LICENCE
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      112 2021-01-11 14:56:37.000000 django-admin-csvexport-2.2/MANIFEST.in
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     5698 2023-04-26 10:03:10.987725 django-admin-csvexport-2.2/PKG-INFO
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     4348 2023-04-26 09:50:57.000000 django-admin-csvexport-2.2/README.rst
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-04-26 10:03:10.979725 django-admin-csvexport-2.2/csvexport/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)       59 2023-04-26 09:55:26.000000 django-admin-csvexport-2.2/csvexport/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     7676 2023-04-26 09:42:42.000000 django-admin-csvexport-2.2/csvexport/actions.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)       93 2020-08-31 18:53:49.000000 django-admin-csvexport-2.2/csvexport/apps.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     2929 2020-12-08 09:31:11.000000 django-admin-csvexport-2.2/csvexport/forms.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      829 2023-03-22 12:11:12.000000 django-admin-csvexport-2.2/csvexport/settings.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-04-26 10:03:10.975725 django-admin-csvexport-2.2/csvexport/static/
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-04-26 10:03:10.979725 django-admin-csvexport-2.2/csvexport/static/csvexport/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      375 2020-08-31 18:53:49.000000 django-admin-csvexport-2.2/csvexport/static/csvexport/checkbox_select_all.js
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-04-26 10:03:10.975725 django-admin-csvexport-2.2/csvexport/templates/
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-04-26 10:03:10.979725 django-admin-csvexport-2.2/csvexport/templates/csvexport/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      223 2020-08-31 18:53:49.000000 django-admin-csvexport-2.2/csvexport/templates/csvexport/checkbox_select_all.html
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1050 2020-12-08 09:37:56.000000 django-admin-csvexport-2.2/csvexport/templates/csvexport/csvexport.html
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-04-26 10:03:10.983725 django-admin-csvexport-2.2/django_admin_csvexport.egg-info/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     5698 2023-04-26 10:03:10.000000 django-admin-csvexport-2.2/django_admin_csvexport.egg-info/PKG-INFO
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1051 2023-04-26 10:03:10.000000 django-admin-csvexport-2.2/django_admin_csvexport.egg-info/SOURCES.txt
+-rw-r--r--   0 thomas    (1000) thomas    (1000)        1 2023-04-26 10:03:10.000000 django-admin-csvexport-2.2/django_admin_csvexport.egg-info/dependency_links.txt
+-rw-r--r--   0 thomas    (1000) thomas    (1000)       34 2023-04-26 10:03:10.000000 django-admin-csvexport-2.2/django_admin_csvexport.egg-info/requires.txt
+-rw-r--r--   0 thomas    (1000) thomas    (1000)       27 2023-04-26 10:03:10.000000 django-admin-csvexport-2.2/django_admin_csvexport.egg-info/top_level.txt
+-rw-r--r--   0 thomas    (1000) thomas    (1000)        1 2020-08-31 18:53:49.000000 django-admin-csvexport-2.2/django_admin_csvexport.egg-info/zip-safe
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)       38 2023-04-26 10:03:10.987725 django-admin-csvexport-2.2/setup.cfg
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     2098 2023-04-26 10:02:57.000000 django-admin-csvexport-2.2/setup.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-04-26 10:03:10.975725 django-admin-csvexport-2.2/tests/
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-04-26 10:03:10.983725 django-admin-csvexport-2.2/tests/testapp/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)        0 2020-08-31 19:25:50.000000 django-admin-csvexport-2.2/tests/testapp/__init__.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1053 2023-03-22 12:13:17.000000 django-admin-csvexport-2.2/tests/testapp/admin.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      114 2020-09-04 20:31:04.000000 django-admin-csvexport-2.2/tests/testapp/apps.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-04-26 10:03:10.983725 django-admin-csvexport-2.2/tests/testapp/management/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)        0 2020-08-31 19:25:50.000000 django-admin-csvexport-2.2/tests/testapp/management/__init__.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-04-26 10:03:10.983725 django-admin-csvexport-2.2/tests/testapp/management/commands/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)        0 2020-08-31 19:25:50.000000 django-admin-csvexport-2.2/tests/testapp/management/commands/__init__.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1933 2023-03-22 10:18:19.000000 django-admin-csvexport-2.2/tests/testapp/management/commands/testapp.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-04-26 10:03:10.983725 django-admin-csvexport-2.2/tests/testapp/migrations/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     5895 2020-08-31 19:25:50.000000 django-admin-csvexport-2.2/tests/testapp/migrations/0001_initial.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     2620 2020-08-31 19:50:40.000000 django-admin-csvexport-2.2/tests/testapp/migrations/0002_auto_20200831_1950.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)        0 2020-08-31 19:25:50.000000 django-admin-csvexport-2.2/tests/testapp/migrations/__init__.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     2150 2023-02-12 18:12:28.000000 django-admin-csvexport-2.2/tests/testapp/models.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     3165 2021-03-13 11:42:07.000000 django-admin-csvexport-2.2/tests/testapp/settings.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-04-26 10:03:10.983725 django-admin-csvexport-2.2/tests/testapp/tests/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)        0 2020-08-31 19:25:50.000000 django-admin-csvexport-2.2/tests/testapp/tests/__init__.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)    10290 2023-03-22 12:13:17.000000 django-admin-csvexport-2.2/tests/testapp/tests/test_export.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      758 2023-02-12 20:07:56.000000 django-admin-csvexport-2.2/tests/testapp/urls.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      391 2020-08-31 19:25:50.000000 django-admin-csvexport-2.2/tests/testapp/wsgi.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-admin-csvexport-2.1/LICENCE` & `django-admin-csvexport-2.2/LICENCE`

 * *Files identical despite different names*

### Comparing `django-admin-csvexport-2.1/PKG-INFO` & `django-admin-csvexport-2.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: django-admin-csvexport
-Version: 2.1
+Version: 2.2
 Summary: Django-admin-action to export items as csv-formatted data.
 Home-page: https://github.com/thomst/django-admin-csvexport
 Author: Thomas Leichtfuß
 Author-email: thomas.leichtfuss@posteo.de
 License: BSD License
 Platform: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -38,21 +39,21 @@
    :target: https://github.com/thomst/django-admin-csvexport/actions/workflows/ci.yml
    :alt: Run tests for django-admin-csvexport
 
 .. image:: https://coveralls.io/repos/github/thomst/django-admin-csvexport/badge.svg?branch=master
    :target: https://coveralls.io/github/thomst/django-admin-csvexport?branch=master
    :alt: coveralls badge
 
-.. image:: https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue
-   :target: https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue
-   :alt: python: 3.6, 3.7, 3.8, 3.9,3.9,3.10
-
-.. image:: https://img.shields.io/badge/django-2.2%20%7C%203.0%20%7C%203.1%20%7C%203.2%20%7C%204.0%20%7C%204.1-orange
-   :target: https://img.shields.io/badge/django-2.2%20%7C%203.0%20%7C%203.1%20%7C%203.2%20%7C%204.0%20%7C%204.1-orange
-   :alt: django: 2.2, 3.0, 3.1, 3.2, 4.0, 4.1
+.. image:: https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue
+   :target: https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue
+   :alt: python: 3.7, 3.8, 3.9,3.9,3.10
+
+.. image:: https://img.shields.io/badge/django-2.2%20%7C%203.0%20%7C%203.1%20%7C%203.2%20%7C%204.0%20%7C%204.1%20%7C%204.2-orange
+   :target: https://img.shields.io/badge/django-2.2%20%7C%203.0%20%7C%203.1%20%7C%203.2%20%7C%204.0%20%7C%204.1%20%7C%204.2-orange
+   :alt: django: 2.2, 3.0, 3.1, 3.2, 4.0, 4.1, 4.2
 
 
 Description
 ===========
 Django-admin-csvexport is a django-admin-action, that allows you to export the
 items of your django-admin changelist as csv-formatted data.
```

### Comparing `django-admin-csvexport-2.1/README.rst` & `django-admin-csvexport-2.2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -6,21 +6,21 @@
    :target: https://github.com/thomst/django-admin-csvexport/actions/workflows/ci.yml
    :alt: Run tests for django-admin-csvexport
 
 .. image:: https://coveralls.io/repos/github/thomst/django-admin-csvexport/badge.svg?branch=master
    :target: https://coveralls.io/github/thomst/django-admin-csvexport?branch=master
    :alt: coveralls badge
 
-.. image:: https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue
-   :target: https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue
-   :alt: python: 3.6, 3.7, 3.8, 3.9,3.9,3.10
-
-.. image:: https://img.shields.io/badge/django-2.2%20%7C%203.0%20%7C%203.1%20%7C%203.2%20%7C%204.0%20%7C%204.1-orange
-   :target: https://img.shields.io/badge/django-2.2%20%7C%203.0%20%7C%203.1%20%7C%203.2%20%7C%204.0%20%7C%204.1-orange
-   :alt: django: 2.2, 3.0, 3.1, 3.2, 4.0, 4.1
+.. image:: https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue
+   :target: https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue
+   :alt: python: 3.7, 3.8, 3.9,3.9,3.10
+
+.. image:: https://img.shields.io/badge/django-2.2%20%7C%203.0%20%7C%203.1%20%7C%203.2%20%7C%204.0%20%7C%204.1%20%7C%204.2-orange
+   :target: https://img.shields.io/badge/django-2.2%20%7C%203.0%20%7C%203.1%20%7C%203.2%20%7C%204.0%20%7C%204.1%20%7C%204.2-orange
+   :alt: django: 2.2, 3.0, 3.1, 3.2, 4.0, 4.1, 4.2
 
 
 Description
 ===========
 Django-admin-csvexport is a django-admin-action, that allows you to export the
 items of your django-admin changelist as csv-formatted data.
```

### Comparing `django-admin-csvexport-2.1/csvexport/actions.py` & `django-admin-csvexport-2.2/csvexport/actions.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 class BaseModelTree(ModelTree):
     """
     A node per model to map their relations and access their fields.
     """
     export_fields = list()
     selected_fields = list()
 
+    FOLLOW_ACROSS_APPS = True
+
     RELATION_TYPES = [
         'one_to_one',
         'many_to_one',
     ]
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
```

### Comparing `django-admin-csvexport-2.1/csvexport/forms.py` & `django-admin-csvexport-2.2/csvexport/forms.py`

 * *Files identical despite different names*

### Comparing `django-admin-csvexport-2.1/csvexport/settings.py` & `django-admin-csvexport-2.2/csvexport/settings.py`

 * *Files identical despite different names*

### Comparing `django-admin-csvexport-2.1/csvexport/templates/csvexport/csvexport.html` & `django-admin-csvexport-2.2/csvexport/templates/csvexport/csvexport.html`

 * *Files identical despite different names*

### Comparing `django-admin-csvexport-2.1/django_admin_csvexport.egg-info/PKG-INFO` & `django-admin-csvexport-2.2/django_admin_csvexport.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: django-admin-csvexport
-Version: 2.1
+Version: 2.2
 Summary: Django-admin-action to export items as csv-formatted data.
 Home-page: https://github.com/thomst/django-admin-csvexport
 Author: Thomas Leichtfuß
 Author-email: thomas.leichtfuss@posteo.de
 License: BSD License
 Platform: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -38,21 +39,21 @@
    :target: https://github.com/thomst/django-admin-csvexport/actions/workflows/ci.yml
    :alt: Run tests for django-admin-csvexport
 
 .. image:: https://coveralls.io/repos/github/thomst/django-admin-csvexport/badge.svg?branch=master
    :target: https://coveralls.io/github/thomst/django-admin-csvexport?branch=master
    :alt: coveralls badge
 
-.. image:: https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue
-   :target: https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue
-   :alt: python: 3.6, 3.7, 3.8, 3.9,3.9,3.10
-
-.. image:: https://img.shields.io/badge/django-2.2%20%7C%203.0%20%7C%203.1%20%7C%203.2%20%7C%204.0%20%7C%204.1-orange
-   :target: https://img.shields.io/badge/django-2.2%20%7C%203.0%20%7C%203.1%20%7C%203.2%20%7C%204.0%20%7C%204.1-orange
-   :alt: django: 2.2, 3.0, 3.1, 3.2, 4.0, 4.1
+.. image:: https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue
+   :target: https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue
+   :alt: python: 3.7, 3.8, 3.9,3.9,3.10
+
+.. image:: https://img.shields.io/badge/django-2.2%20%7C%203.0%20%7C%203.1%20%7C%203.2%20%7C%204.0%20%7C%204.1%20%7C%204.2-orange
+   :target: https://img.shields.io/badge/django-2.2%20%7C%203.0%20%7C%203.1%20%7C%203.2%20%7C%204.0%20%7C%204.1%20%7C%204.2-orange
+   :alt: django: 2.2, 3.0, 3.1, 3.2, 4.0, 4.1, 4.2
 
 
 Description
 ===========
 Django-admin-csvexport is a django-admin-action, that allows you to export the
 items of your django-admin changelist as csv-formatted data.
```

### Comparing `django-admin-csvexport-2.1/setup.py` & `django-admin-csvexport-2.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 
 import os
 from setuptools import setup
-from setuptools import find_packages
+from setuptools import find_namespace_packages
 
 
 def read(filename):
     path = os.path.join(os.path.dirname(__file__), filename)
     with open(path, encoding="utf-8") as file:
         return file.read()
 
@@ -26,29 +26,30 @@
     description="Django-admin-action to export items as csv-formatted data.",
     long_description=read("README.rst"),
     author="Thomas Leichtfuß",
     author_email="thomas.leichtfuss@posteo.de",
     url="https://github.com/thomst/django-admin-csvexport",
     license="BSD License",
     platforms=["OS Independent"],
-    packages=find_packages(exclude=["tests"]),
+    packages=find_namespace_packages(exclude=["tests"]),
     include_package_data=True,
     install_requires=[
         "Django>=2.2",
         "django-modeltree>=0.3",
     ],
     classifiers=[
         dev_status,
         "Framework :: Django",
         "Framework :: Django :: 2.2",
         "Framework :: Django :: 3.0",
         "Framework :: Django :: 3.1",
         "Framework :: Django :: 3.2",
         "Framework :: Django :: 4.0",
         "Framework :: Django :: 4.1",
+        "Framework :: Django :: 4.2",
         "Environment :: Web Environment",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
```

