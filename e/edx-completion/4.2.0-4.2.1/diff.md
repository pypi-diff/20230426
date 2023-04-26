# Comparing `tmp/edx-completion-4.2.0.tar.gz` & `tmp/edx-completion-4.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-completion-4.2.0.tar", last modified: Mon Feb 14 13:53:01 2022, max compression
+gzip compressed data, was "edx-completion-4.2.1.tar", last modified: Wed Apr 26 14:44:47 2023, max compression
```

## Comparing `edx-completion-4.2.0.tar` & `edx-completion-4.2.1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-14 13:53:01.472533 edx-completion-4.2.0/
--rw-r--r--   0 runner    (1001) docker     (121)     7859 2022-02-14 13:52:56.000000 edx-completion-4.2.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)    34520 2022-02-14 13:52:56.000000 edx-completion-4.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      230 2022-02-14 13:52:56.000000 edx-completion-4.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    13126 2022-02-14 13:53:01.472533 edx-completion-4.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4529 2022-02-14 13:52:56.000000 edx-completion-4.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-14 13:53:01.468532 edx-completion-4.2.0/completion/
--rw-r--r--   0 runner    (1001) docker     (121)      138 2022-02-14 13:52:56.000000 edx-completion-4.2.0/completion/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-14 13:53:01.468532 edx-completion-4.2.0/completion/api/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-14 13:52:56.000000 edx-completion-4.2.0/completion/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1635 2022-02-14 13:52:56.000000 edx-completion-4.2.0/completion/api/permissions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-14 13:53:01.468532 edx-completion-4.2.0/completion/api/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-14 13:52:56.000000 edx-completion-4.2.0/completion/api/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3728 2022-02-14 13:52:56.000000 edx-completion-4.2.0/completion/api/tests/test_permissions.py
--rw-r--r--   0 runner    (1001) docker     (121)      212 2022-02-14 13:52:56.000000 edx-completion-4.2.0/completion/api/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-14 13:53:01.472533 edx-completion-4.2.0/completion/api/v1/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-14 13:52:56.000000 edx-completion-4.2.0/completion/api/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-14 13:53:01.472533 edx-completion-4.2.0/completion/api/v1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-14 13:52:56.000000 edx-completion-4.2.0/completion/api/v1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      632 2022-02-14 13:52:56.000000 edx-completion-4.2.0/completion/api/v1/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)     9219 2022-02-14 13:52:56.000000 edx-completion-4.2.0/completion/api/v1/views.py
--rw-r--r--   0 runner    (1001) docker     (121)     1156 2022-02-14 13:52:56.000000 edx-completion-4.2.0/completion/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)      438 2022-02-14 13:52:56.000000 edx-completion-4.2.0/completion/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1819 2022-02-14 13:52:56.000000 edx-completion-4.2.0/completion/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-14 13:53:01.472533 edx-completion-4.2.0/completion/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-02-14 13:52:56.000000 edx-completion-4.2.0/completion/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)      312 2022-02-14 13:52:56.000000 edx-completion-4.2.0/completion/migrations/0002_auto_20180125_1510.py
--rw-r--r--   0 runner    (1001) docker     (121)     1309 2022-02-14 13:52:56.000000 edx-completion-4.2.0/completion/migrations/0003_learning_context.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-14 13:52:56.000000 edx-completion-4.2.0/completion/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12622 2022-02-14 13:52:56.000000 edx-completion-4.2.0/completion/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     8087 2022-02-14 13:52:56.000000 edx-completion-4.2.0/completion/services.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-14 13:53:01.472533 edx-completion-4.2.0/completion/settings/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-14 13:52:56.000000 edx-completion-4.2.0/completion/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1109 2022-02-14 13:52:56.000000 edx-completion-4.2.0/completion/settings/common.py
--rw-r--r--   0 runner    (1001) docker     (121)      475 2022-02-14 13:52:56.000000 edx-completion-4.2.0/completion/settings/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     3689 2022-02-14 13:52:56.000000 edx-completion-4.2.0/completion/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-14 13:53:01.472533 edx-completion-4.2.0/completion/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-14 13:52:56.000000 edx-completion-4.2.0/completion/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8889 2022-02-14 13:52:56.000000 edx-completion-4.2.0/completion/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (121)     9545 2022-02-14 13:52:56.000000 edx-completion-4.2.0/completion/tests/test_services.py
--rw-r--r--   0 runner    (1001) docker     (121)     1511 2022-02-14 13:52:56.000000 edx-completion-4.2.0/completion/tests/test_utilities.py
--rw-r--r--   0 runner    (1001) docker     (121)      927 2022-02-14 13:52:56.000000 edx-completion-4.2.0/completion/utilities.py
--rw-r--r--   0 runner    (1001) docker     (121)      924 2022-02-14 13:52:56.000000 edx-completion-4.2.0/completion/waffle.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-14 13:53:01.472533 edx-completion-4.2.0/edx_completion.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    13126 2022-02-14 13:53:01.000000 edx-completion-4.2.0/edx_completion.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1275 2022-02-14 13:53:01.000000 edx-completion-4.2.0/edx_completion.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-14 13:53:01.000000 edx-completion-4.2.0/edx_completion.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-02-14 13:53:01.000000 edx-completion-4.2.0/edx_completion.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-14 13:53:01.000000 edx-completion-4.2.0/edx_completion.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      127 2022-02-14 13:53:01.000000 edx-completion-4.2.0/edx_completion.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-02-14 13:53:01.000000 edx-completion-4.2.0/edx_completion.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-14 13:53:01.472533 edx-completion-4.2.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (121)      202 2022-02-14 13:52:56.000000 edx-completion-4.2.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (121)      444 2022-02-14 13:52:56.000000 edx-completion-4.2.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (121)      526 2022-02-14 13:52:56.000000 edx-completion-4.2.0/requirements/test.in
--rw-r--r--   0 runner    (1001) docker     (121)      264 2022-02-14 13:53:01.472533 edx-completion-4.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     5369 2022-02-14 13:52:56.000000 edx-completion-4.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 14:44:47.952363 edx-completion-4.2.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     8091 2023-04-26 14:44:41.000000 edx-completion-4.2.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    34520 2023-04-26 14:44:41.000000 edx-completion-4.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      230 2023-04-26 14:44:41.000000 edx-completion-4.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    13239 2023-04-26 14:44:47.952363 edx-completion-4.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4426 2023-04-26 14:44:41.000000 edx-completion-4.2.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 14:44:47.944363 edx-completion-4.2.1/completion/
+-rw-r--r--   0 runner    (1001) docker     (122)      138 2023-04-26 14:44:41.000000 edx-completion-4.2.1/completion/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 14:44:47.944363 edx-completion-4.2.1/completion/api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-26 14:44:41.000000 edx-completion-4.2.1/completion/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1635 2023-04-26 14:44:41.000000 edx-completion-4.2.1/completion/api/permissions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 14:44:47.944363 edx-completion-4.2.1/completion/api/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-26 14:44:41.000000 edx-completion-4.2.1/completion/api/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3728 2023-04-26 14:44:41.000000 edx-completion-4.2.1/completion/api/tests/test_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      212 2023-04-26 14:44:41.000000 edx-completion-4.2.1/completion/api/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 14:44:47.948363 edx-completion-4.2.1/completion/api/v1/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-26 14:44:41.000000 edx-completion-4.2.1/completion/api/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 14:44:47.948363 edx-completion-4.2.1/completion/api/v1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-26 14:44:41.000000 edx-completion-4.2.1/completion/api/v1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      632 2023-04-26 14:44:41.000000 edx-completion-4.2.1/completion/api/v1/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9219 2023-04-26 14:44:41.000000 edx-completion-4.2.1/completion/api/v1/views.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1156 2023-04-26 14:44:41.000000 edx-completion-4.2.1/completion/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)      438 2023-04-26 14:44:41.000000 edx-completion-4.2.1/completion/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1828 2023-04-26 14:44:41.000000 edx-completion-4.2.1/completion/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 14:44:47.948363 edx-completion-4.2.1/completion/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     1648 2023-04-26 14:44:41.000000 edx-completion-4.2.1/completion/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)      312 2023-04-26 14:44:41.000000 edx-completion-4.2.1/completion/migrations/0002_auto_20180125_1510.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1309 2023-04-26 14:44:41.000000 edx-completion-4.2.1/completion/migrations/0003_learning_context.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-26 14:44:41.000000 edx-completion-4.2.1/completion/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12622 2023-04-26 14:44:41.000000 edx-completion-4.2.1/completion/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8289 2023-04-26 14:44:41.000000 edx-completion-4.2.1/completion/services.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 14:44:47.948363 edx-completion-4.2.1/completion/settings/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-26 14:44:41.000000 edx-completion-4.2.1/completion/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1113 2023-04-26 14:44:41.000000 edx-completion-4.2.1/completion/settings/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)      475 2023-04-26 14:44:41.000000 edx-completion-4.2.1/completion/settings/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3775 2023-04-26 14:44:41.000000 edx-completion-4.2.1/completion/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 14:44:47.948363 edx-completion-4.2.1/completion/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-26 14:44:41.000000 edx-completion-4.2.1/completion/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8889 2023-04-26 14:44:41.000000 edx-completion-4.2.1/completion/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9545 2023-04-26 14:44:41.000000 edx-completion-4.2.1/completion/tests/test_services.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1511 2023-04-26 14:44:41.000000 edx-completion-4.2.1/completion/tests/test_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (122)      927 2023-04-26 14:44:41.000000 edx-completion-4.2.1/completion/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (122)      924 2023-04-26 14:44:41.000000 edx-completion-4.2.1/completion/waffle.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 14:44:47.952363 edx-completion-4.2.1/edx_completion.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    13239 2023-04-26 14:44:47.000000 edx-completion-4.2.1/edx_completion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1275 2023-04-26 14:44:47.000000 edx-completion-4.2.1/edx_completion.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-26 14:44:47.000000 edx-completion-4.2.1/edx_completion.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       65 2023-04-26 14:44:47.000000 edx-completion-4.2.1/edx_completion.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-26 14:44:47.000000 edx-completion-4.2.1/edx_completion.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      127 2023-04-26 14:44:47.000000 edx-completion-4.2.1/edx_completion.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-04-26 14:44:47.000000 edx-completion-4.2.1/edx_completion.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 14:44:47.952363 edx-completion-4.2.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      202 2023-04-26 14:44:41.000000 edx-completion-4.2.1/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      615 2023-04-26 14:44:41.000000 edx-completion-4.2.1/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      526 2023-04-26 14:44:41.000000 edx-completion-4.2.1/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (122)      264 2023-04-26 14:44:47.952363 edx-completion-4.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     5373 2023-04-26 14:44:41.000000 edx-completion-4.2.1/setup.py
```

### Comparing `edx-completion-4.2.0/CHANGELOG.rst` & `edx-completion-4.2.1/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,20 @@
    This project adheres to Semantic Versioning (http://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
 
+[4.2.1]- 2023-04-26
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+* Support ``get_child_blocks`` along with ``get_child_descriptors``.
+* Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
+  deprecated
+
 [4.1.0]- 2021-07-19
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 * Add Django 3.0, 3.1 & 3.2 Support
 
 [4.0.4]- 2021-02-04
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 * Update ``get_key_to_last_completed_block`` to return ``full_block_key`` instead of ``block_key``
```

### Comparing `edx-completion-4.2.0/LICENSE` & `edx-completion-4.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `edx-completion-4.2.0/PKG-INFO` & `edx-completion-4.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: edx-completion
-Version: 4.2.0
+Version: 4.2.1
 Summary: A library for tracking completion of blocks by learners in edX courses.
-Home-page: https://github.com/edx/completion
+Home-page: https://github.com/openedx/completion
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Django edx
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Natural Language :: English
@@ -49,34 +48,32 @@
 Please see ``LICENSE.txt`` for details.
 
 How To Contribute
 -----------------
 
 Contributions are very welcome.
 
-Please read `How To Contribute <https://github.com/edx/edx-platform/blob/master/CONTRIBUTING.rst>`_ for details.
+Please read `How To Contribute <https://github.com/openedx/.github/blob/master/CONTRIBUTING.md>`_ for details.
 
-Even though they were written with ``edx-platform`` in mind, the guidelines
-should be followed for Open edX code in general.
 
 PR description template should be automatically applied if you are sending PR from github interface; otherwise you
-can find it it at `PULL_REQUEST_TEMPLATE.md <https://github.com/edx/completion/blob/master/.github/PULL_REQUEST_TEMPLATE.md>`_
+can find it it at `PULL_REQUEST_TEMPLATE.md <https://github.com/openedx/completion/blob/master/.github/PULL_REQUEST_TEMPLATE.md>`_
 
 Issue report template should be automatically applied if you are sending it from github UI as well; otherwise you
-can find it at `ISSUE_TEMPLATE.md <https://github.com/edx/completion/blob/master/.github/ISSUE_TEMPLATE.md>`_
+can find it at `ISSUE_TEMPLATE.md <https://github.com/openedx/completion/blob/master/.github/ISSUE_TEMPLATE.md>`_
 
 Reporting Security Issues
 -------------------------
 
 Please do not report security issues in public. Please email security@edx.org.
 
 Using with Docker Devstack
 --------------------------
 
-Prerequisite: Have your Open edX `Devstack <https://github.com/edx/devstack>`_ properly installed.
+Prerequisite: Have your Open edX `Devstack <https://github.com/openedx/devstack>`_ properly installed.
 
 Note: When you see "from inside the lms" below, it means that you've run ``make lms-shell`` from your devstack
 directory and are on a command prompt inside the LMS container.
 
 #. Clone this repo into ``../src/`` directory (relative to your "devstack" repo location). This will mount the
    directory in a way that is accessible to the lms container.
 
@@ -106,16 +103,16 @@
 .. _list of resources: https://open.edx.org/getting-help
 
 
 .. |pypi-badge| image:: https://img.shields.io/pypi/v/edx-completion.svg
     :target: https://pypi.python.org/pypi/edx-completion/
     :alt: PyPI
 
-.. |CI| image:: https://github.com/edx/completion/workflows/Python%20CI/badge.svg?branch=master
-    :target: https://github.com/edx/completion/actions?query=workflow%3A%22Python+CI%22
+.. |CI| image:: https://github.com/openedx/completion/workflows/Python%20CI/badge.svg?branch=master
+    :target: https://github.com/openedx/completion/actions?query=workflow%3A%22Python+CI%22
     :alt: CI
 
 .. |codecov-badge| image:: http://codecov.io/github/edx/completion/coverage.svg?branch=master
     :target: http://codecov.io/github/edx/completion?branch=master
     :alt: Codecov
 
 .. |doc-badge| image:: https://readthedocs.org/projects/completion/badge/?version=latest
@@ -123,15 +120,15 @@
     :alt: Documentation
 
 .. |pyversions-badge| image:: https://img.shields.io/pypi/pyversions/edx-completion.svg
     :target: https://pypi.python.org/pypi/edx-completion/
     :alt: Supported Python versions
 
 .. |license-badge| image:: https://img.shields.io/github/license/edx/completion.svg
-    :target: https://github.com/edx/completion/blob/master/LICENSE.txt
+    :target: https://github.com/openedx/completion/blob/master/LICENSE.txt
     :alt: License
 
 
 Change Log
 ----------
 
 ..
@@ -143,14 +140,20 @@
    This project adheres to Semantic Versioning (http://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
 
+[4.2.1]- 2023-04-26
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+* Support ``get_child_blocks`` along with ``get_child_descriptors``.
+* Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
+  deprecated
+
 [4.1.0]- 2021-07-19
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 * Add Django 3.0, 3.1 & 3.2 Support
 
 [4.0.4]- 2021-02-04
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 * Update ``get_key_to_last_completed_block`` to return ``full_block_key`` instead of ``block_key``
@@ -315,9 +318,7 @@
 [0.0.2] - 2018-01-31
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 * Fix up edx-lint requirements shenanigans.
 
 [0.0.1] - 2018-01-31
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 * Initial release
-
-
```

### Comparing `edx-completion-4.2.0/README.rst` & `edx-completion-4.2.1/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -28,34 +28,32 @@
 Please see ``LICENSE.txt`` for details.
 
 How To Contribute
 -----------------
 
 Contributions are very welcome.
 
-Please read `How To Contribute <https://github.com/edx/edx-platform/blob/master/CONTRIBUTING.rst>`_ for details.
+Please read `How To Contribute <https://github.com/openedx/.github/blob/master/CONTRIBUTING.md>`_ for details.
 
-Even though they were written with ``edx-platform`` in mind, the guidelines
-should be followed for Open edX code in general.
 
 PR description template should be automatically applied if you are sending PR from github interface; otherwise you
-can find it it at `PULL_REQUEST_TEMPLATE.md <https://github.com/edx/completion/blob/master/.github/PULL_REQUEST_TEMPLATE.md>`_
+can find it it at `PULL_REQUEST_TEMPLATE.md <https://github.com/openedx/completion/blob/master/.github/PULL_REQUEST_TEMPLATE.md>`_
 
 Issue report template should be automatically applied if you are sending it from github UI as well; otherwise you
-can find it at `ISSUE_TEMPLATE.md <https://github.com/edx/completion/blob/master/.github/ISSUE_TEMPLATE.md>`_
+can find it at `ISSUE_TEMPLATE.md <https://github.com/openedx/completion/blob/master/.github/ISSUE_TEMPLATE.md>`_
 
 Reporting Security Issues
 -------------------------
 
 Please do not report security issues in public. Please email security@edx.org.
 
 Using with Docker Devstack
 --------------------------
 
-Prerequisite: Have your Open edX `Devstack <https://github.com/edx/devstack>`_ properly installed.
+Prerequisite: Have your Open edX `Devstack <https://github.com/openedx/devstack>`_ properly installed.
 
 Note: When you see "from inside the lms" below, it means that you've run ``make lms-shell`` from your devstack
 directory and are on a command prompt inside the LMS container.
 
 #. Clone this repo into ``../src/`` directory (relative to your "devstack" repo location). This will mount the
    directory in a way that is accessible to the lms container.
 
@@ -85,16 +83,16 @@
 .. _list of resources: https://open.edx.org/getting-help
 
 
 .. |pypi-badge| image:: https://img.shields.io/pypi/v/edx-completion.svg
     :target: https://pypi.python.org/pypi/edx-completion/
     :alt: PyPI
 
-.. |CI| image:: https://github.com/edx/completion/workflows/Python%20CI/badge.svg?branch=master
-    :target: https://github.com/edx/completion/actions?query=workflow%3A%22Python+CI%22
+.. |CI| image:: https://github.com/openedx/completion/workflows/Python%20CI/badge.svg?branch=master
+    :target: https://github.com/openedx/completion/actions?query=workflow%3A%22Python+CI%22
     :alt: CI
 
 .. |codecov-badge| image:: http://codecov.io/github/edx/completion/coverage.svg?branch=master
     :target: http://codecov.io/github/edx/completion?branch=master
     :alt: Codecov
 
 .. |doc-badge| image:: https://readthedocs.org/projects/completion/badge/?version=latest
@@ -102,9 +100,9 @@
     :alt: Documentation
 
 .. |pyversions-badge| image:: https://img.shields.io/pypi/pyversions/edx-completion.svg
     :target: https://pypi.python.org/pypi/edx-completion/
     :alt: Supported Python versions
 
 .. |license-badge| image:: https://img.shields.io/github/license/edx/completion.svg
-    :target: https://github.com/edx/completion/blob/master/LICENSE.txt
+    :target: https://github.com/openedx/completion/blob/master/LICENSE.txt
     :alt: License
```

### Comparing `edx-completion-4.2.0/completion/api/permissions.py` & `edx-completion-4.2.1/completion/api/permissions.py`

 * *Files identical despite different names*

### Comparing `edx-completion-4.2.0/completion/api/tests/test_permissions.py` & `edx-completion-4.2.1/completion/api/tests/test_permissions.py`

 * *Files identical despite different names*

### Comparing `edx-completion-4.2.0/completion/api/v1/urls.py` & `edx-completion-4.2.1/completion/api/v1/urls.py`

 * *Files identical despite different names*

### Comparing `edx-completion-4.2.0/completion/api/v1/views.py` & `edx-completion-4.2.1/completion/api/v1/views.py`

 * *Files identical despite different names*

### Comparing `edx-completion-4.2.0/completion/apps.py` & `edx-completion-4.2.1/completion/apps.py`

 * *Files identical despite different names*

### Comparing `edx-completion-4.2.0/completion/handlers.py` & `edx-completion-4.2.1/completion/handlers.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     When a problem is scored, submit a new BlockCompletion for that block.
     """
     if not waffle.ENABLE_COMPLETION_TRACKING_SWITCH.is_enabled():
         return
     try:
         block_key = UsageKey.from_string(kwargs['usage_id'])
     except InvalidKeyError:
-        log.exception("Unable to parse XBlock usage_id for completion: %s", block_key)
+        log.exception("Unable to parse XBlock usage_id for completion: %s", kwargs['usage_id'])
         return
 
     if block_key.context_key.is_course and block_key.context_key.run is None:
         # In the case of old mongo courses, the context_key cannot be derived
         # from the block key alone since it will be missing run info:
         course_key_with_run = LearningContextKey.from_string(kwargs['course_id'])
         block_key = block_key.replace(course_key=course_key_with_run)
```

### Comparing `edx-completion-4.2.0/completion/migrations/0001_initial.py` & `edx-completion-4.2.1/completion/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edx-completion-4.2.0/completion/migrations/0003_learning_context.py` & `edx-completion-4.2.1/completion/migrations/0003_learning_context.py`

 * *Files identical despite different names*

### Comparing `edx-completion-4.2.0/completion/models.py` & `edx-completion-4.2.1/completion/models.py`

 * *Files identical despite different names*

### Comparing `edx-completion-4.2.0/completion/services.py` & `edx-completion-4.2.1/completion/services.py`

 * *Files 3% similar despite different names*

```diff
@@ -89,15 +89,17 @@
 
         Note: The nodes passed in should have already taken the user into
         account so the proper blocks are shown for this user.
         """
         user_children = []
         mode = XBlockCompletionMode.get_mode(node)
         if mode == XBlockCompletionMode.AGGREGATOR:
+            # TODO: `get_child_descriptors` will be renamed to `get_child_blocks` in the Redwood release.
             node_children = ((hasattr(node, 'get_child_descriptors') and node.get_child_descriptors())
+                             or (hasattr(node, 'get_child_blocks') and node.get_child_blocks())
                              or (hasattr(node, 'get_children') and node.get_children()))
             for child in node_children:
                 user_children.extend(self.get_completable_children(child))
         elif node and mode == XBlockCompletionMode.COMPLETABLE:
             user_children = [node]
         return user_children
```

### Comparing `edx-completion-4.2.0/completion/settings/common.py` & `edx-completion-4.2.1/completion/settings/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,14 @@
 
 SECRET_KEY = 'insecure-secret-key'
 
 
 def plugin_settings(settings):  # pylint: disable=unused-argument
     """
     Defines completion-specific settings when app is used as a plugin to edx-platform.
-    See: https://github.com/edx/edx-platform/blob/master/openedx/core/djangoapps/plugins/README.rst
+    See: https://github.com/openedx/edx-platform/blob/master/openedx/core/djangoapps/plugins/README.rst
     """
     # Once a complete-by-viewing (e.g. HTML) block has been visible on-screen for this many ms, mark it complete
     settings.COMPLETION_BY_VIEWING_DELAY_MS = 5000
     # Once a user has watched this percentage of a video, mark it as complete:
     # (0.0 = 0%, 1.0 = 100%)
     settings.COMPLETION_VIDEO_COMPLETE_PERCENTAGE = 0.95
```

### Comparing `edx-completion-4.2.0/completion/test_utils.py` & `edx-completion-4.2.1/completion/test_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         for the course of the test.
         Parameters:
             override (bool): True if tracking should be enabled.
         """
         _waffle_overrider = override_waffle_switch(
             waffle.ENABLE_COMPLETION_TRACKING_SWITCH, override
         )
-        _waffle_overrider.__enter__()
+        _waffle_overrider.__enter__()  # pylint: disable=unnecessary-dunder-call
         self.addCleanup(_waffle_overrider.__exit__, None, None, None)
 
 
 class CompletionSetUpMixin:
     """
     Mixin to provide set_up_completion() function to child TestCase classes.
     """
@@ -84,15 +84,15 @@
 
     @classmethod
     def setUpClass(cls):
         super().setUpClass()
         cls.waffle_patcher = override_waffle_switch(
             waffle.ENABLE_COMPLETION_TRACKING_SWITCH, cls.COMPLETION_SWITCH_ENABLED
         )
-        cls.waffle_patcher.__enter__()
+        cls.waffle_patcher.__enter__()  # pylint: disable=unnecessary-dunder-call
 
     @classmethod
     def tearDownClass(cls):
         super().tearDownClass()
         cls.waffle_patcher.__exit__(None, None, None)
 
     def setUp(self):
```

### Comparing `edx-completion-4.2.0/completion/tests/test_models.py` & `edx-completion-4.2.1/completion/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `edx-completion-4.2.0/completion/tests/test_services.py` & `edx-completion-4.2.1/completion/tests/test_services.py`

 * *Files identical despite different names*

### Comparing `edx-completion-4.2.0/completion/tests/test_utilities.py` & `edx-completion-4.2.1/completion/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `edx-completion-4.2.0/completion/utilities.py` & `edx-completion-4.2.1/completion/utilities.py`

 * *Files identical despite different names*

### Comparing `edx-completion-4.2.0/completion/waffle.py` & `edx-completion-4.2.1/completion/waffle.py`

 * *Files identical despite different names*

### Comparing `edx-completion-4.2.0/edx_completion.egg-info/PKG-INFO` & `edx-completion-4.2.1/edx_completion.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: edx-completion
-Version: 4.2.0
+Version: 4.2.1
 Summary: A library for tracking completion of blocks by learners in edX courses.
-Home-page: https://github.com/edx/completion
+Home-page: https://github.com/openedx/completion
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Django edx
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Natural Language :: English
@@ -49,34 +48,32 @@
 Please see ``LICENSE.txt`` for details.
 
 How To Contribute
 -----------------
 
 Contributions are very welcome.
 
-Please read `How To Contribute <https://github.com/edx/edx-platform/blob/master/CONTRIBUTING.rst>`_ for details.
+Please read `How To Contribute <https://github.com/openedx/.github/blob/master/CONTRIBUTING.md>`_ for details.
 
-Even though they were written with ``edx-platform`` in mind, the guidelines
-should be followed for Open edX code in general.
 
 PR description template should be automatically applied if you are sending PR from github interface; otherwise you
-can find it it at `PULL_REQUEST_TEMPLATE.md <https://github.com/edx/completion/blob/master/.github/PULL_REQUEST_TEMPLATE.md>`_
+can find it it at `PULL_REQUEST_TEMPLATE.md <https://github.com/openedx/completion/blob/master/.github/PULL_REQUEST_TEMPLATE.md>`_
 
 Issue report template should be automatically applied if you are sending it from github UI as well; otherwise you
-can find it at `ISSUE_TEMPLATE.md <https://github.com/edx/completion/blob/master/.github/ISSUE_TEMPLATE.md>`_
+can find it at `ISSUE_TEMPLATE.md <https://github.com/openedx/completion/blob/master/.github/ISSUE_TEMPLATE.md>`_
 
 Reporting Security Issues
 -------------------------
 
 Please do not report security issues in public. Please email security@edx.org.
 
 Using with Docker Devstack
 --------------------------
 
-Prerequisite: Have your Open edX `Devstack <https://github.com/edx/devstack>`_ properly installed.
+Prerequisite: Have your Open edX `Devstack <https://github.com/openedx/devstack>`_ properly installed.
 
 Note: When you see "from inside the lms" below, it means that you've run ``make lms-shell`` from your devstack
 directory and are on a command prompt inside the LMS container.
 
 #. Clone this repo into ``../src/`` directory (relative to your "devstack" repo location). This will mount the
    directory in a way that is accessible to the lms container.
 
@@ -106,16 +103,16 @@
 .. _list of resources: https://open.edx.org/getting-help
 
 
 .. |pypi-badge| image:: https://img.shields.io/pypi/v/edx-completion.svg
     :target: https://pypi.python.org/pypi/edx-completion/
     :alt: PyPI
 
-.. |CI| image:: https://github.com/edx/completion/workflows/Python%20CI/badge.svg?branch=master
-    :target: https://github.com/edx/completion/actions?query=workflow%3A%22Python+CI%22
+.. |CI| image:: https://github.com/openedx/completion/workflows/Python%20CI/badge.svg?branch=master
+    :target: https://github.com/openedx/completion/actions?query=workflow%3A%22Python+CI%22
     :alt: CI
 
 .. |codecov-badge| image:: http://codecov.io/github/edx/completion/coverage.svg?branch=master
     :target: http://codecov.io/github/edx/completion?branch=master
     :alt: Codecov
 
 .. |doc-badge| image:: https://readthedocs.org/projects/completion/badge/?version=latest
@@ -123,15 +120,15 @@
     :alt: Documentation
 
 .. |pyversions-badge| image:: https://img.shields.io/pypi/pyversions/edx-completion.svg
     :target: https://pypi.python.org/pypi/edx-completion/
     :alt: Supported Python versions
 
 .. |license-badge| image:: https://img.shields.io/github/license/edx/completion.svg
-    :target: https://github.com/edx/completion/blob/master/LICENSE.txt
+    :target: https://github.com/openedx/completion/blob/master/LICENSE.txt
     :alt: License
 
 
 Change Log
 ----------
 
 ..
@@ -143,14 +140,20 @@
    This project adheres to Semantic Versioning (http://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
 
+[4.2.1]- 2023-04-26
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+* Support ``get_child_blocks`` along with ``get_child_descriptors``.
+* Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
+  deprecated
+
 [4.1.0]- 2021-07-19
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 * Add Django 3.0, 3.1 & 3.2 Support
 
 [4.0.4]- 2021-02-04
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 * Update ``get_key_to_last_completed_block`` to return ``full_block_key`` instead of ``block_key``
@@ -315,9 +318,7 @@
 [0.0.2] - 2018-01-31
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 * Fix up edx-lint requirements shenanigans.
 
 [0.0.1] - 2018-01-31
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 * Initial release
-
-
```

### Comparing `edx-completion-4.2.0/edx_completion.egg-info/SOURCES.txt` & `edx-completion-4.2.1/edx_completion.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edx-completion-4.2.0/requirements/test.in` & `edx-completion-4.2.1/requirements/test.in`

 * *Files identical despite different names*

### Comparing `edx-completion-4.2.0/setup.py` & `edx-completion-4.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
 setup(
     name='edx-completion',
     version=VERSION,
     description="""A library for tracking completion of blocks by learners in edX courses.""",
     long_description=README + '\n\n' + CHANGELOG,
     author='edX',
     author_email='oscm@edx.org',
-    url='https://github.com/edx/completion',
+    url='https://github.com/openedx/completion',
     packages=[
         'completion',
     ],
     entry_points={
         'lms.djangoapp': [
             'completion = completion.apps:CompletionAppConfig',
         ],
```

