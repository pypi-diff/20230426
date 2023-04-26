# Comparing `tmp/plone.app.caching-3.0.5.tar.gz` & `tmp/plone.app.caching-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.app.caching-3.0.5.tar", last modified: Thu Apr 13 23:32:45 2023, max compression
+gzip compressed data, was "plone.app.caching-3.1.0.tar", last modified: Wed Apr 26 21:46:53 2023, max compression
```

## Comparing `plone.app.caching-3.0.5.tar` & `plone.app.caching-3.1.0.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:32:45.017500 plone.app.caching-3.0.5/
--rw-r--r--   0 maurits    (501) staff       (20)    14892 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/CHANGES.md
--rw-r--r--   0 maurits    (501) staff       (20)      162 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    18955 2023-04-13 23:32:45.017643 plone.app.caching-3.0.5/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     3056 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/README.md
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:32:44.997074 plone.app.caching-3.0.5/docs/
--rw-r--r--   0 maurits    (501) staff       (20)    15220 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      674 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/docs/LICENSE.txt
--rw-r--r--   0 maurits    (501) staff       (20)      308 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/docs/changelog_template.jinja
--rw-r--r--   0 maurits    (501) staff       (20)      230 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/lint-requirements.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:32:44.997375 plone.app.caching-3.0.5/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:32:45.000164 plone.app.caching-3.0.5/plone/app/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:32:45.003755 plone.app.caching-3.0.5/plone/app/caching/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:32:45.006962 plone.app.caching-3.0.5/plone/app/caching/browser/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/browser/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1119 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/browser/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)    41005 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/browser/controlpanel.pt
--rw-r--r--   0 maurits    (501) staff       (20)    21546 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/browser/controlpanel.py
--rw-r--r--   0 maurits    (501) staff       (20)      656 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/browser/edit.pt
--rw-r--r--   0 maurits    (501) staff       (20)     9575 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/browser/edit.py
--rw-r--r--   0 maurits    (501) staff       (20)     5523 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/browser/import.pt
--rw-r--r--   0 maurits    (501) staff       (20)      155 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/browser/plone.app.caching.gif
--rw-r--r--   0 maurits    (501) staff       (20)     6307 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/browser/purge.pt
--rw-r--r--   0 maurits    (501) staff       (20)     4622 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/browser/ramcache.pt
--rw-r--r--   0 maurits    (501) staff       (20)     4468 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/caching.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1751 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     3021 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)     3867 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/lastmodified.py
--rw-r--r--   0 maurits    (501) staff       (20)     3985 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/lookup.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:32:45.008716 plone.app.caching-3.0.5/plone/app/caching/operations/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/operations/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     2783 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/operations/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)    13297 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/operations/default.py
--rw-r--r--   0 maurits    (501) staff       (20)     8040 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/operations/etags.py
--rw-r--r--   0 maurits    (501) staff       (20)     1725 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/operations/ramcache.py
--rw-r--r--   0 maurits    (501) staff       (20)    24136 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/operations/utils.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:32:44.993223 plone.app.caching-3.0.5/plone/app/caching/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:32:45.009676 plone.app.caching-3.0.5/plone/app/caching/profiles/default/
--rw-r--r--   0 maurits    (501) staff       (20)      594 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/profiles/default/controlpanel.xml
--rw-r--r--   0 maurits    (501) staff       (20)      184 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/profiles/default/metadata.xml
--rw-r--r--   0 maurits    (501) staff       (20)       13 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/profiles/default/plone.app.caching.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:32:45.011475 plone.app.caching-3.0.5/plone/app/caching/profiles/default/registry/
--rw-r--r--   0 maurits    (501) staff       (20)     1934 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/profiles/default/registry/basesettings.xml
--rw-r--r--   0 maurits    (501) staff       (20)     2318 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/profiles/default/registry/generic.xml
--rw-r--r--   0 maurits    (501) staff       (20)     2137 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/profiles/default/registry/moderate.xml
--rw-r--r--   0 maurits    (501) staff       (20)     2486 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/profiles/default/registry/strong.xml
--rw-r--r--   0 maurits    (501) staff       (20)     2414 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/profiles/default/registry/terse.xml
--rw-r--r--   0 maurits    (501) staff       (20)     1792 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/profiles/default/registry/weak.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:32:44.992892 plone.app.caching-3.0.5/plone/app/caching/profiles/v2/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:32:45.011779 plone.app.caching-3.0.5/plone/app/caching/profiles/v2/registry/
--rw-r--r--   0 maurits    (501) staff       (20)     2414 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/profiles/v2/registry/terse.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:32:45.012088 plone.app.caching-3.0.5/plone/app/caching/profiles/with-caching-proxy/
--rw-r--r--   0 maurits    (501) staff       (20)     4971 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/profiles/with-caching-proxy/registry.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:32:45.012390 plone.app.caching-3.0.5/plone/app/caching/profiles/without-caching-proxy/
--rw-r--r--   0 maurits    (501) staff       (20)     4581 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/profiles/without-caching-proxy/registry.xml
--rw-r--r--   0 maurits    (501) staff       (20)     1504 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/profiles.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     8396 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/purge.py
--rw-r--r--   0 maurits    (501) staff       (20)     1038 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/setuphandlers.py
--rw-r--r--   0 maurits    (501) staff       (20)     2171 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/testing.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:32:45.016693 plone.app.caching-3.0.5/plone/app/caching/tests/
--rw-r--r--   0 maurits    (501) staff       (20)      668 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/tests/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:32:45.017272 plone.app.caching-3.0.5/plone/app/caching/tests/data/
--rw-r--r--   0 maurits    (501) staff       (20)     9819 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/tests/data/plone-app-caching.jpg
--rw-r--r--   0 maurits    (501) staff       (20)      189 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/tests/data/testfile.csv
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/tests/test.css
--rw-r--r--   0 maurits    (501) staff       (20)      155 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/tests/test.gif
--rw-r--r--   0 maurits    (501) staff       (20)    11871 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/tests/test_etags.py
--rw-r--r--   0 maurits    (501) staff       (20)     9866 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/tests/test_integration.py
--rw-r--r--   0 maurits    (501) staff       (20)     7101 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/tests/test_lastmodified.py
--rw-r--r--   0 maurits    (501) staff       (20)    10537 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/tests/test_lookup.py
--rw-r--r--   0 maurits    (501) staff       (20)     2992 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/tests/test_operation_default.py
--rw-r--r--   0 maurits    (501) staff       (20)     6912 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/tests/test_operation_parameters.py
--rw-r--r--   0 maurits    (501) staff       (20)    55900 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/tests/test_operation_utils.py
--rw-r--r--   0 maurits    (501) staff       (20)    25361 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/tests/test_profile_with_caching_proxy.py
--rw-r--r--   0 maurits    (501) staff       (20)    22166 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/tests/test_profile_without_caching_proxy.py
--rw-r--r--   0 maurits    (501) staff       (20)    13490 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/tests/test_purge.py
--rw-r--r--   0 maurits    (501) staff       (20)     5674 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/tests/test_utils.py
--rw-r--r--   0 maurits    (501) staff       (20)     2123 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/utils.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:32:44.999863 plone.app.caching-3.0.5/plone.app.caching.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    18955 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone.app.caching.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     2887 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone.app.caching.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone.app.caching.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       40 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone.app.caching.egg-info/entry_points.txt
--rw-r--r--   0 maurits    (501) staff       (20)       16 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone.app.caching.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone.app.caching.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      695 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone.app.caching.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone.app.caching.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1136 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)       13 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/requirements.txt
--rw-r--r--   0 maurits    (501) staff       (20)      326 2023-04-13 23:32:45.018220 plone.app.caching-3.0.5/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     2775 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:46:53.923525 plone.app.caching-3.1.0/
+-rw-r--r--   0 maurits    (501) staff       (20)    15150 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/CHANGES.md
+-rw-r--r--   0 maurits    (501) staff       (20)      162 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    19213 2023-04-26 21:46:53.923672 plone.app.caching-3.1.0/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     3056 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/README.md
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:46:53.903506 plone.app.caching-3.1.0/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)    15220 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/docs/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      674 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/docs/LICENSE.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      308 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/docs/changelog_template.jinja
+-rw-r--r--   0 maurits    (501) staff       (20)      230 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/lint-requirements.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:46:53.903795 plone.app.caching-3.1.0/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:46:53.906554 plone.app.caching-3.1.0/plone/app/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:46:53.909945 plone.app.caching-3.1.0/plone/app/caching/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:46:53.913079 plone.app.caching-3.1.0/plone/app/caching/browser/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/browser/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1119 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/browser/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)    41005 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/browser/controlpanel.pt
+-rw-r--r--   0 maurits    (501) staff       (20)    21546 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/browser/controlpanel.py
+-rw-r--r--   0 maurits    (501) staff       (20)      656 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/browser/edit.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     9575 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/browser/edit.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5523 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/browser/import.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      155 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/browser/plone.app.caching.gif
+-rw-r--r--   0 maurits    (501) staff       (20)     6307 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/browser/purge.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     4622 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/browser/ramcache.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     4468 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/caching.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     1751 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     3021 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3867 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/lastmodified.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3985 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/lookup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:46:53.914815 plone.app.caching-3.1.0/plone/app/caching/operations/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/operations/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2783 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/operations/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)    13297 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/operations/default.py
+-rw-r--r--   0 maurits    (501) staff       (20)     7731 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/operations/etags.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1725 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/operations/ramcache.py
+-rw-r--r--   0 maurits    (501) staff       (20)    24136 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/operations/utils.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:46:53.899882 plone.app.caching-3.1.0/plone/app/caching/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:46:53.915773 plone.app.caching-3.1.0/plone/app/caching/profiles/default/
+-rw-r--r--   0 maurits    (501) staff       (20)      594 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/profiles/default/controlpanel.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      184 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/profiles/default/metadata.xml
+-rw-r--r--   0 maurits    (501) staff       (20)       13 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/profiles/default/plone.app.caching.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:46:53.917553 plone.app.caching-3.1.0/plone/app/caching/profiles/default/registry/
+-rw-r--r--   0 maurits    (501) staff       (20)     1934 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/profiles/default/registry/basesettings.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     2318 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/profiles/default/registry/generic.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     2137 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/profiles/default/registry/moderate.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     2486 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/profiles/default/registry/strong.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     2414 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/profiles/default/registry/terse.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     1792 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/profiles/default/registry/weak.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:46:53.899559 plone.app.caching-3.1.0/plone/app/caching/profiles/v2/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:46:53.917846 plone.app.caching-3.1.0/plone/app/caching/profiles/v2/registry/
+-rw-r--r--   0 maurits    (501) staff       (20)     2414 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/profiles/v2/registry/terse.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:46:53.918139 plone.app.caching-3.1.0/plone/app/caching/profiles/with-caching-proxy/
+-rw-r--r--   0 maurits    (501) staff       (20)     4971 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/profiles/with-caching-proxy/registry.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:46:53.918432 plone.app.caching-3.1.0/plone/app/caching/profiles/without-caching-proxy/
+-rw-r--r--   0 maurits    (501) staff       (20)     4581 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/profiles/without-caching-proxy/registry.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     1504 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/profiles.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     8396 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/purge.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1038 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/setuphandlers.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2171 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/testing.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:46:53.922695 plone.app.caching-3.1.0/plone/app/caching/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)      668 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/tests/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:46:53.923285 plone.app.caching-3.1.0/plone/app/caching/tests/data/
+-rw-r--r--   0 maurits    (501) staff       (20)     9819 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/tests/data/plone-app-caching.jpg
+-rw-r--r--   0 maurits    (501) staff       (20)      189 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/tests/data/testfile.csv
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/tests/test.css
+-rw-r--r--   0 maurits    (501) staff       (20)      155 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/tests/test.gif
+-rw-r--r--   0 maurits    (501) staff       (20)    11871 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/tests/test_etags.py
+-rw-r--r--   0 maurits    (501) staff       (20)     9866 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/tests/test_integration.py
+-rw-r--r--   0 maurits    (501) staff       (20)     7101 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/tests/test_lastmodified.py
+-rw-r--r--   0 maurits    (501) staff       (20)    10537 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/tests/test_lookup.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2992 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/tests/test_operation_default.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6912 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/tests/test_operation_parameters.py
+-rw-r--r--   0 maurits    (501) staff       (20)    55900 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/tests/test_operation_utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)    25538 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/tests/test_profile_with_caching_proxy.py
+-rw-r--r--   0 maurits    (501) staff       (20)    22468 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/tests/test_profile_without_caching_proxy.py
+-rw-r--r--   0 maurits    (501) staff       (20)    13490 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/tests/test_purge.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5674 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/tests/test_utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2123 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/utils.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:46:53.906258 plone.app.caching-3.1.0/plone.app.caching.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    19213 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone.app.caching.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     2887 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone.app.caching.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone.app.caching.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       40 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone.app.caching.egg-info/entry_points.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       16 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone.app.caching.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone.app.caching.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      695 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone.app.caching.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone.app.caching.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1136 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)       13 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/requirements.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      326 2023-04-26 21:46:53.924218 plone.app.caching-3.1.0/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     2775 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/setup.py
```

### Comparing `plone.app.caching-3.0.5/CHANGES.md` & `plone.app.caching-3.1.0/CHANGES.md`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,25 @@
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 -->
 
 <!-- towncrier release notes start -->
 
+## 3.1.0 (2023-04-26)
+
+
+### New features:
+
+- Update the resourceRegistries ETag to use the config registry modification time.
+  This time is set since Plone 6.0.4.
+  Fixes `issue 93 <https://github.com/plone/plone.app.caching/issues/93>`_.
+  [maurits] #93
+
+
 ## 3.0.5 (2023-04-14)
 
 
 ### Bug fixes:
 
 - Fix spelling error.
   [gforcada] #124
```

### Comparing `plone.app.caching-3.0.5/PKG-INFO` & `plone.app.caching-3.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.caching
-Version: 3.0.5
+Version: 3.1.0
 Summary: Plone UI and default rules for plone.caching/z3c.caching
 Home-page: https://github.com/plone/plone.app.caching
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: plone caching
 Classifier: Development Status :: 5 - Production/Stable
@@ -108,14 +108,25 @@
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 -->
 
 <!-- towncrier release notes start -->
 
+## 3.1.0 (2023-04-26)
+
+
+### New features:
+
+- Update the resourceRegistries ETag to use the config registry modification time.
+  This time is set since Plone 6.0.4.
+  Fixes `issue 93 <https://github.com/plone/plone.app.caching/issues/93>`_.
+  [maurits] #93
+
+
 ## 3.0.5 (2023-04-14)
 
 
 ### Bug fixes:
 
 - Fix spelling error.
   [gforcada] #124
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: plone.app.caching Version: 3.0.5 Summary: Plone UI
+Metadata-Version: 2.1 Name: plone.app.caching Version: 3.1.0 Summary: Plone UI
 and default rules for plone.caching/z3c.caching Home-page: https://github.com/
 plone/plone.app.caching Author: Plone Foundation Author-email: plone-
 developers@lists.sourceforge.net License: GPL version 2 Keywords: plone caching
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
 :: Web Environment Classifier: Framework :: Plone Classifier: Framework ::
 Plone :: 6.0 Classifier: Framework :: Plone :: Core Classifier: Framework ::
 Zope :: 5 Classifier: License :: OSI Approved :: GNU General Public License v2
@@ -18,14 +18,44 @@
 pypi.org/project/plone.app.caching/) [![PyPI - License](https://img.shields.io/
 pypi/l/plone.app.caching)](https://pypi.org/project/plone.app.caching/) [![PyPI
    - Status](https://img.shields.io/pypi/status/plone.app.caching)](https://
      pypi.org/project/plone.app.caching/) [![GitHub contributors](https://
      img.shields.io/github/contributors/plone/plone.app.caching)](https://
        github.com/plone/plone.app.caching) ![GitHub Repo stars](https://
     img.shields.io/github/stars/plone/plone.app.caching?style=flat-square)
+## Introduction This package provides a Plone UI and default rules for managing
+HTTP response caching in Plone. It builds on [z3c.caching](https://github.com/
+zopefoundation/z3c.caching), [plone.caching](https://github.com/plone/
+plone.caching) and [plone.cachepurging](https://github.com/plone/
+plone.cachepurging). ### Compatibility | Version | Plone | |------|-----| | 3.x
+| 6.0 or above | | 2.x | 5.2 | | 1.x | 5.1, 5.0, 4.3, 4.2, 4.1 | ##
+Installation `plone.app.caching` is shipped as a dependency of the *Plone*
+package, and it should be available on all Plone installations, but Caching is
+**not enabled by default**, although it is highly recommended to configure
+caching for every new Plone site. After creating a new Plone site, go to `Site
+Setup`, then `Addons` and install `HTTP caching support`. Under the Advanced
+header, look for the Caching control panel -- currently only supported on the
+Classic UI. ### Troubleshooting When the Caching control panel is not there,
+there can be various reasons for this: - If your installation does not load the
+`Plone` package, but only `Products.CMFPlone`, then `plone.app.caching` is not
+included. - If the package *is* included, but you add a Plone Site using the
+advanced form and disable caching, then the control panel is not there. If you
+want to install it in an existing Plone Site: 1. Make sure the package is
+available in the Plone instance, by adding `plone.app.caching` or `Plone` to
+your installation. 2. From the Plone Site Setup go to the ZMI (Zope Management
+Interface). 3. Go to ``portal_setup``, and then to the Import tab. 4. Select
+the HTTP caching support profile, perhaps easiest by id: `profile-
+plone.app.caching:default`. 5. Click 'Import all steps'. ## Source Code
+Contributors, please read the document [Process for Plone core's development]
+(https://5.docs.plone.org/develop/coredev/docs/index.html) Sources are at the
+[Plone code repository hosted at Github ](https://github.com/plone/
+plone.app.caching). ## This project is supported by [Plone_Logo] ## License The
+project is licensed under GPLv2. # Changelog   ## 3.1.0 (2023-04-26) ### New
+features: - Update the resourceRegistries ETag to use the config registry
+modification time. This time is set since Plone 6.0.4. Fixes `issue 93
 ` in controlpanel. [petschki] (#112) - Revert changes to tests to work with the
 Zope security fix. We must have an empty byte, not text, otherwise it is an
 indication that we get a possibly wrong Content-Type in a 304 status. See `Zope
 issue 1089
 github.com/zopefoundation/Zope/issues/1089>`_. [maurits] (#1089) ## 3.0.1
 (2022-12-21) ### Bug fixes: - Fix tests to work with the Zope security fix.
 [maurits] (#106) ## 3.0.0 (2022-11-14) ### Bug fixes: - Add missing quotation
```

### Comparing `plone.app.caching-3.0.5/README.md` & `plone.app.caching-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.5/docs/LICENSE.GPL` & `plone.app.caching-3.1.0/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.5/docs/LICENSE.txt` & `plone.app.caching-3.1.0/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.5/plone/app/caching/browser/configure.zcml` & `plone.app.caching-3.1.0/plone/app/caching/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.5/plone/app/caching/browser/controlpanel.pt` & `plone.app.caching-3.1.0/plone/app/caching/browser/controlpanel.pt`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.5/plone/app/caching/browser/controlpanel.py` & `plone.app.caching-3.1.0/plone/app/caching/browser/controlpanel.py`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.5/plone/app/caching/browser/edit.pt` & `plone.app.caching-3.1.0/plone/app/caching/browser/edit.pt`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.5/plone/app/caching/browser/edit.py` & `plone.app.caching-3.1.0/plone/app/caching/browser/edit.py`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.5/plone/app/caching/browser/import.pt` & `plone.app.caching-3.1.0/plone/app/caching/browser/import.pt`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.5/plone/app/caching/browser/purge.pt` & `plone.app.caching-3.1.0/plone/app/caching/browser/purge.pt`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.5/plone/app/caching/browser/ramcache.pt` & `plone.app.caching-3.1.0/plone/app/caching/browser/ramcache.pt`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.5/plone/app/caching/caching.zcml` & `plone.app.caching-3.1.0/plone/app/caching/caching.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.5/plone/app/caching/configure.zcml` & `plone.app.caching-3.1.0/plone/app/caching/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.5/plone/app/caching/interfaces.py` & `plone.app.caching-3.1.0/plone/app/caching/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.5/plone/app/caching/lastmodified.py` & `plone.app.caching-3.1.0/plone/app/caching/lastmodified.py`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.5/plone/app/caching/lookup.py` & `plone.app.caching-3.1.0/plone/app/caching/lookup.py`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.5/plone/app/caching/operations/configure.zcml` & `plone.app.caching-3.1.0/plone/app/caching/operations/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.5/plone/app/caching/operations/default.py` & `plone.app.caching-3.1.0/plone/app/caching/operations/default.py`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.5/plone/app/caching/operations/etags.py` & `plone.app.caching-3.1.0/plone/app/caching/operations/etags.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 from Acquisition import aq_base
 from Acquisition import aq_inner
 from plone.app.caching.interfaces import IETagValue
 from plone.app.caching.operations.utils import getContext
 from plone.app.caching.operations.utils import getLastModifiedAnnotation
 from plone.base.utils import safe_hasattr
+from plone.registry.interfaces import IRegistry
 from Products.CMFCore.interfaces import ICatalogTool
 from Products.CMFCore.interfaces import IMembershipTool
 from Products.CMFCore.utils import getToolByName
-from Products.CMFPlone.resources.utils import get_override_directory
-from Products.CMFPlone.resources.utils import PRODUCTION_RESOURCE_DIRECTORY
 from zope.component import adapter
 from zope.component import queryMultiAdapter
 from zope.component import queryUtility
 from zope.interface import implementer
 from zope.interface import Interface
 
 import random
 import time
 
 
+try:
+    # available since Plone 6.0.4
+    from Products.CMFPlone.resources.browser.resource import _RESOURCE_REGISTRY_MTIME
+except ImportError:
+    _RESOURCE_REGISTRY_MTIME = None
+
+
 @implementer(IETagValue)
 @adapter(Interface, Interface)
 class UserID:
     """The ``userid`` etag component, returning the current user's id"""
 
     def __init__(self, published, request):
         self.published = published
@@ -235,30 +241,23 @@
     """
 
     def __init__(self, published, request):
         self.published = published
         self.request = request
 
     def __call__(self):
-        context = getContext(self.published)
-        container = get_override_directory(context)
-        if PRODUCTION_RESOURCE_DIRECTORY not in container:
+        if _RESOURCE_REGISTRY_MTIME is None:
             return ""
-        production_folder = container[PRODUCTION_RESOURCE_DIRECTORY]
-        filename = "timestamp.txt"
-        if filename not in production_folder:
+        registry = queryUtility(IRegistry)
+        if registry is None:
             return ""
-        timestamp = production_folder.readFile(filename)
-        if not timestamp:
+        mtime = getattr(registry, _RESOURCE_REGISTRY_MTIME, None)
+        if mtime is None:
             return ""
-        # timestamp is in bytes, and we must return a string.
-        # On Python 2 this is the same, but not on Python 3.
-        if not isinstance(timestamp, str):
-            timestamp = timestamp.decode("utf-8")
-        return timestamp
+        return str(mtime)
 
 
 @implementer(IETagValue)
 @adapter(Interface, Interface)
 class Layout:
     """The 'layout' etag component, returning they layout of a content item."""
```

### Comparing `plone.app.caching-3.0.5/plone/app/caching/operations/ramcache.py` & `plone.app.caching-3.1.0/plone/app/caching/operations/ramcache.py`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.5/plone/app/caching/operations/utils.py` & `plone.app.caching-3.1.0/plone/app/caching/operations/utils.py`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.5/plone/app/caching/profiles/default/controlpanel.xml` & `plone.app.caching-3.1.0/plone/app/caching/profiles/default/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.5/plone/app/caching/profiles/default/registry/basesettings.xml` & `plone.app.caching-3.1.0/plone/app/caching/profiles/default/registry/basesettings.xml`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.5/plone/app/caching/profiles/default/registry/generic.xml` & `plone.app.caching-3.1.0/plone/app/caching/profiles/default/registry/generic.xml`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.5/plone/app/caching/profiles/default/registry/moderate.xml` & `plone.app.caching-3.1.0/plone/app/caching/profiles/default/registry/moderate.xml`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.5/plone/app/caching/profiles/default/registry/strong.xml` & `plone.app.caching-3.1.0/plone/app/caching/profiles/default/registry/strong.xml`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.5/plone/app/caching/profiles/default/registry/terse.xml` & `plone.app.caching-3.1.0/plone/app/caching/profiles/default/registry/terse.xml`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.5/plone/app/caching/profiles/default/registry/weak.xml` & `plone.app.caching-3.1.0/plone/app/caching/profiles/default/registry/weak.xml`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.5/plone/app/caching/profiles/v2/registry/terse.xml` & `plone.app.caching-3.1.0/plone/app/caching/profiles/v2/registry/terse.xml`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.5/plone/app/caching/profiles/with-caching-proxy/registry.xml` & `plone.app.caching-3.1.0/plone/app/caching/profiles/with-caching-proxy/registry.xml`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.5/plone/app/caching/profiles/without-caching-proxy/registry.xml` & `plone.app.caching-3.1.0/plone/app/caching/profiles/without-caching-proxy/registry.xml`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.5/plone/app/caching/profiles.zcml` & `plone.app.caching-3.1.0/plone/app/caching/profiles.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.5/plone/app/caching/purge.py` & `plone.app.caching-3.1.0/plone/app/caching/purge.py`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.5/plone/app/caching/setuphandlers.py` & `plone.app.caching-3.1.0/plone/app/caching/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.5/plone/app/caching/testing.py` & `plone.app.caching-3.1.0/plone/app/caching/testing.py`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.5/plone/app/caching/tests/__init__.py` & `plone.app.caching-3.1.0/plone/app/caching/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.5/plone/app/caching/tests/data/plone-app-caching.jpg` & `plone.app.caching-3.1.0/plone/app/caching/tests/data/plone-app-caching.jpg`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.5/plone/app/caching/tests/test_etags.py` & `plone.app.caching-3.1.0/plone/app/caching/tests/test_etags.py`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.5/plone/app/caching/tests/test_integration.py` & `plone.app.caching-3.1.0/plone/app/caching/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.5/plone/app/caching/tests/test_lastmodified.py` & `plone.app.caching-3.1.0/plone/app/caching/tests/test_lastmodified.py`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.5/plone/app/caching/tests/test_lookup.py` & `plone.app.caching-3.1.0/plone/app/caching/tests/test_lookup.py`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.5/plone/app/caching/tests/test_operation_default.py` & `plone.app.caching-3.1.0/plone/app/caching/tests/test_operation_default.py`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.5/plone/app/caching/tests/test_operation_parameters.py` & `plone.app.caching-3.1.0/plone/app/caching/tests/test_operation_parameters.py`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.5/plone/app/caching/tests/test_operation_utils.py` & `plone.app.caching-3.1.0/plone/app/caching/tests/test_operation_utils.py`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.5/plone/app/caching/tests/test_profile_with_caching_proxy.py` & `plone.app.caching-3.1.0/plone/app/caching/tests/test_profile_with_caching_proxy.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,20 +69,20 @@
         setRequest(None)
 
     def test_composite_viewsxx(self):
         # This is a clone of the same test for 'without-caching-proxy'
         # Can we just call that test from this context?
 
         catalog = self.portal["portal_catalog"]
-        skins_tool = self.portal["portal_skins"]
+        default_skin = self.portal["portal_skins"].default_skin
 
         # Add folder content
         setRoles(self.portal, TEST_USER_ID, ("Manager",))
         self.portal.invokeFactory("Folder", "f1")
-        self.portal["f1"].title = "one"
+        self.portal["f1"].title = "Folder one"
         self.portal["f1"].description = "Folder one description"
         self.portal["f1"].reindexObject()
 
         # Add page content
         self.portal["f1"].invokeFactory("Document", "d1")
         self.portal["f1"]["d1"].title = "Document one"
         self.portal["f1"]["d1"].description = "Document one description"
@@ -101,17 +101,24 @@
         # Should we set up the etag components?
         # - set member?  No
         # - reset catalog counter?  Maybe
         # - set server language?
         # - turn on gzip?
         # - set skin?  Maybe
         # - leave status unlocked
-        #
+        # - set the mod date on the resource registries?  Probably.
         transaction.commit()
 
+        # Since Plone 6.0.4 we have a modification date on the registry.
+        from Products.CMFPlone.resources.browser.resource import (
+            _RESOURCE_REGISTRY_MTIME,
+        )
+
+        mtime = str(getattr(self.registry, _RESOURCE_REGISTRY_MTIME))
+
         # Request the authenticated folder
         now = stable_now()
         browser = Browser(self.app)
         browser.addHeader(
             "Authorization",
             f"Basic {TEST_USER_NAME}:{TEST_USER_PASSWORD}",
         )
@@ -120,35 +127,31 @@
         self.assertEqual(
             "plone.app.caching.weakCaching", browser.headers["X-Cache-Operation"]
         )
         # This should use cacheInBrowser
         self.assertEqual(
             "max-age=0, must-revalidate, private", browser.headers["Cache-Control"]
         )
-        self.assertEqual(
-            f'"|test_user_1_|{catalog.getCounter()}|en|{skins_tool.default_skin}|0|0|"',
-            normalize_etag(browser.headers["ETag"]),
-        )
+        tag = f'"|test_user_1_|{catalog.getCounter()}|en|{default_skin}|0|0|{mtime}"'
+        self.assertEqual(tag, normalize_etag(browser.headers["ETag"]))
         self.assertGreater(now, dateutil.parser.parse(browser.headers["Expires"]))
 
         # Set the copy/cut cookie and then request the folder view again
         browser.cookies.create("__cp", "xxx")
         browser.open(self.portal["f1"].absolute_url())
         # The response should be the same as before except for the etag
         self.assertEqual("plone.content.folderView", browser.headers["X-Cache-Rule"])
         self.assertEqual(
             "plone.app.caching.weakCaching", browser.headers["X-Cache-Operation"]
         )
         self.assertEqual(
             "max-age=0, must-revalidate, private", browser.headers["Cache-Control"]
         )
-        self.assertEqual(
-            f'"|test_user_1_|{catalog.getCounter()}|en|{skins_tool.default_skin}|0|1|"',
-            normalize_etag(browser.headers["ETag"]),
-        )
+        tag = f'"|test_user_1_|{catalog.getCounter()}|en|{default_skin}|0|1|{mtime}"'
+        self.assertEqual(tag, normalize_etag(browser.headers["ETag"]))
 
         # Request the authenticated page
         now = stable_now()
         browser = Browser(self.app)
         browser.addHeader(
             "Authorization",
             f"Basic {TEST_USER_NAME}:{TEST_USER_PASSWORD}",
@@ -159,18 +162,16 @@
         self.assertEqual(
             "plone.app.caching.weakCaching", browser.headers["X-Cache-Operation"]
         )
         # This should use cacheInBrowser
         self.assertEqual(
             "max-age=0, must-revalidate, private", browser.headers["Cache-Control"]
         )
-        self.assertEqual(
-            f'"|test_user_1_|{catalog.getCounter()}|en|{skins_tool.default_skin}|0|"',
-            normalize_etag(browser.headers["ETag"]),
-        )
+        tag = f'"|test_user_1_|{catalog.getCounter()}|en|{default_skin}|0|{mtime}"'
+        self.assertEqual(tag, normalize_etag(browser.headers["ETag"]))
         self.assertGreater(now, dateutil.parser.parse(browser.headers["Expires"]))
 
         # Request the authenticated page again -- to test RAM cache.
         browser = Browser(self.app)
         browser.addHeader(
             "Authorization",
             f"Basic {TEST_USER_NAME}:{TEST_USER_PASSWORD}",
@@ -201,28 +202,25 @@
         # See https://github.com/zopefoundation/Zope/issues/1089.
         self.assertEqual(b"", browser.contents)
         self.assertFalse(browser.headers["Content-Type"])
 
         # Request the anonymous folder
         now = stable_now()
         browser = Browser(self.app)
-        browser.handleErrors = False
         browser.open(self.portal["f1"].absolute_url())
         self.assertEqual("plone.content.folderView", browser.headers["X-Cache-Rule"])
         self.assertEqual(
             "plone.app.caching.weakCaching", browser.headers["X-Cache-Operation"]
         )
         # This should use cacheInBrowser
         self.assertEqual(
             "max-age=0, must-revalidate, private", browser.headers["Cache-Control"]
         )
-        self.assertEqual(
-            f'"||{catalog.getCounter()}|en|{skins_tool.default_skin}|0|0|"',
-            normalize_etag(browser.headers["ETag"]),
-        )
+        tag = f'"||{catalog.getCounter()}|en|{default_skin}|0|0|{mtime}"'
+        self.assertEqual(tag, normalize_etag(browser.headers["ETag"]))
         self.assertGreater(now, dateutil.parser.parse(browser.headers["Expires"]))
 
         # Request the anonymous page
         now = stable_now()
         browser = Browser(self.app)
         browser.open(self.portal["f1"]["d1"].absolute_url())
         self.assertEqual("plone.content.itemView", browser.headers["X-Cache-Rule"])
@@ -230,18 +228,16 @@
             "plone.app.caching.weakCaching", browser.headers["X-Cache-Operation"]
         )
         self.assertIn(testText, browser.contents)
         # This should use cacheInBrowser
         self.assertEqual(
             "max-age=0, must-revalidate, private", browser.headers["Cache-Control"]
         )
-        self.assertEqual(
-            f'"||{catalog.getCounter()}|en|{skins_tool.default_skin}|0|"',
-            normalize_etag(browser.headers["ETag"]),
-        )
+        tag = f'"||{catalog.getCounter()}|en|{default_skin}|0|{mtime}"'
+        self.assertEqual(tag, normalize_etag(browser.headers["ETag"]))
         self.assertGreater(now, dateutil.parser.parse(browser.headers["Expires"]))
 
         # Request the anonymous page again -- to test RAM cache.
         # Anonymous should be RAM cached
         now = stable_now()
         browser = Browser(self.app)
         browser.open(self.portal["f1"]["d1"].absolute_url())
@@ -253,18 +249,16 @@
         self.assertEqual(
             "plone.app.caching.operations.ramcache", browser.headers["X-RAMCache"]
         )
         self.assertIn(testText, browser.contents)
         self.assertEqual(
             "max-age=0, must-revalidate, private", browser.headers["Cache-Control"]
         )
-        self.assertEqual(
-            f'"||{catalog.getCounter()}|en|{skins_tool.default_skin}|0|"',
-            normalize_etag(browser.headers["ETag"]),
-        )
+        tag = f'"||{catalog.getCounter()}|en|{default_skin}|0|{mtime}"'
+        self.assertEqual(tag, normalize_etag(browser.headers["ETag"]))
         self.assertGreater(now, dateutil.parser.parse(browser.headers["Expires"]))
 
         # Request the anonymous page again -- with an INM header to test 304.
         etag = browser.headers["ETag"]
         browser = Browser(self.app)
         browser.raiseHttpErrors = False
         browser.addHeader("If-None-Match", etag)
```

### Comparing `plone.app.caching-3.0.5/plone/app/caching/tests/test_profile_without_caching_proxy.py` & `plone.app.caching-3.1.0/plone/app/caching/tests/test_profile_without_caching_proxy.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,14 +88,21 @@
         # - set server language?
         # - turn on gzip?
         # - set skin?  Maybe
         # - leave status unlocked
         # - set the mod date on the resource registries?  Probably.
         transaction.commit()
 
+        # Since Plone 6.0.4 we have a modification date on the registry.
+        from Products.CMFPlone.resources.browser.resource import (
+            _RESOURCE_REGISTRY_MTIME,
+        )
+
+        mtime = str(getattr(self.registry, _RESOURCE_REGISTRY_MTIME))
+
         # Request the authenticated folder
         now = stable_now()
         browser = Browser(self.app)
         browser.addHeader(
             "Authorization",
             f"Basic {TEST_USER_NAME}:{TEST_USER_PASSWORD}",
         )
@@ -104,30 +111,30 @@
         self.assertEqual(
             "plone.app.caching.weakCaching", browser.headers["X-Cache-Operation"]
         )
         # This should use cacheInBrowser
         self.assertEqual(
             "max-age=0, must-revalidate, private", browser.headers["Cache-Control"]
         )
-        tag = f'"|test_user_1_|{catalog.getCounter()}|en|{default_skin}|0|0|"'
+        tag = f'"|test_user_1_|{catalog.getCounter()}|en|{default_skin}|0|0|{mtime}"'
         self.assertEqual(tag, normalize_etag(browser.headers["ETag"]))
         self.assertGreater(now, dateutil.parser.parse(browser.headers["Expires"]))
 
         # Set the copy/cut cookie and then request the folder view again
         browser.cookies.create("__cp", "xxx")
         browser.open(self.portal["f1"].absolute_url())
         # The response should be the same as before except for the etag
         self.assertEqual("plone.content.folderView", browser.headers["X-Cache-Rule"])
         self.assertEqual(
             "plone.app.caching.weakCaching", browser.headers["X-Cache-Operation"]
         )
         self.assertEqual(
             "max-age=0, must-revalidate, private", browser.headers["Cache-Control"]
         )
-        tag = f'"|test_user_1_|{catalog.getCounter()}|en|{default_skin}|0|1|"'
+        tag = f'"|test_user_1_|{catalog.getCounter()}|en|{default_skin}|0|1|{mtime}"'
         self.assertEqual(tag, normalize_etag(browser.headers["ETag"]))
 
         # Request the authenticated page
         now = stable_now()
         browser = Browser(self.app)
         browser.addHeader(
             "Authorization",
@@ -139,15 +146,15 @@
         self.assertEqual(
             "plone.app.caching.weakCaching", browser.headers["X-Cache-Operation"]
         )
         # This should use cacheInBrowser
         self.assertEqual(
             "max-age=0, must-revalidate, private", browser.headers["Cache-Control"]
         )
-        tag = f'"|test_user_1_|{catalog.getCounter()}|en|{default_skin}|0|"'
+        tag = f'"|test_user_1_|{catalog.getCounter()}|en|{default_skin}|0|{mtime}"'
         self.assertEqual(tag, normalize_etag(browser.headers["ETag"]))
         self.assertGreater(now, dateutil.parser.parse(browser.headers["Expires"]))
 
         # Request the authenticated page again -- to test RAM cache.
         browser = Browser(self.app)
         browser.addHeader(
             "Authorization",
@@ -188,15 +195,15 @@
         self.assertEqual(
             "plone.app.caching.weakCaching", browser.headers["X-Cache-Operation"]
         )
         # This should use cacheInBrowser
         self.assertEqual(
             "max-age=0, must-revalidate, private", browser.headers["Cache-Control"]
         )
-        tag = f'"||{catalog.getCounter()}|en|{default_skin}|0|0|"'
+        tag = f'"||{catalog.getCounter()}|en|{default_skin}|0|0|{mtime}"'
         self.assertEqual(tag, normalize_etag(browser.headers["ETag"]))
         self.assertGreater(now, dateutil.parser.parse(browser.headers["Expires"]))
 
         # Request the anonymous page
         now = stable_now()
         browser = Browser(self.app)
         browser.open(self.portal["f1"]["d1"].absolute_url())
@@ -205,15 +212,15 @@
             "plone.app.caching.weakCaching", browser.headers["X-Cache-Operation"]
         )
         self.assertIn(testText, browser.contents)
         # This should use cacheInBrowser
         self.assertEqual(
             "max-age=0, must-revalidate, private", browser.headers["Cache-Control"]
         )
-        tag = f'"||{catalog.getCounter()}|en|{default_skin}|0|"'
+        tag = f'"||{catalog.getCounter()}|en|{default_skin}|0|{mtime}"'
         self.assertEqual(tag, normalize_etag(browser.headers["ETag"]))
         self.assertGreater(now, dateutil.parser.parse(browser.headers["Expires"]))
 
         # Request the anonymous page again -- to test RAM cache.
         # Anonymous should be RAM cached
         now = stable_now()
         browser = Browser(self.app)
@@ -226,15 +233,15 @@
         self.assertEqual(
             "plone.app.caching.operations.ramcache", browser.headers["X-RAMCache"]
         )
         self.assertIn(testText, browser.contents)
         self.assertEqual(
             "max-age=0, must-revalidate, private", browser.headers["Cache-Control"]
         )
-        tag = f'"||{catalog.getCounter()}|en|{default_skin}|0|"'
+        tag = f'"||{catalog.getCounter()}|en|{default_skin}|0|{mtime}"'
         self.assertEqual(tag, normalize_etag(browser.headers["ETag"]))
         self.assertGreater(now, dateutil.parser.parse(browser.headers["Expires"]))
 
         # Request the anonymous page again -- with an INM header to test 304.
         etag = browser.headers["ETag"]
         browser = Browser(self.app)
         browser.raiseHttpErrors = False
```

### Comparing `plone.app.caching-3.0.5/plone/app/caching/tests/test_purge.py` & `plone.app.caching-3.1.0/plone/app/caching/tests/test_purge.py`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.5/plone/app/caching/tests/test_utils.py` & `plone.app.caching-3.1.0/plone/app/caching/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.5/plone/app/caching/utils.py` & `plone.app.caching-3.1.0/plone/app/caching/utils.py`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.5/plone.app.caching.egg-info/PKG-INFO` & `plone.app.caching-3.1.0/plone.app.caching.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.caching
-Version: 3.0.5
+Version: 3.1.0
 Summary: Plone UI and default rules for plone.caching/z3c.caching
 Home-page: https://github.com/plone/plone.app.caching
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: plone caching
 Classifier: Development Status :: 5 - Production/Stable
@@ -108,14 +108,25 @@
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 -->
 
 <!-- towncrier release notes start -->
 
+## 3.1.0 (2023-04-26)
+
+
+### New features:
+
+- Update the resourceRegistries ETag to use the config registry modification time.
+  This time is set since Plone 6.0.4.
+  Fixes `issue 93 <https://github.com/plone/plone.app.caching/issues/93>`_.
+  [maurits] #93
+
+
 ## 3.0.5 (2023-04-14)
 
 
 ### Bug fixes:
 
 - Fix spelling error.
   [gforcada] #124
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: plone.app.caching Version: 3.0.5 Summary: Plone UI
+Metadata-Version: 2.1 Name: plone.app.caching Version: 3.1.0 Summary: Plone UI
 and default rules for plone.caching/z3c.caching Home-page: https://github.com/
 plone/plone.app.caching Author: Plone Foundation Author-email: plone-
 developers@lists.sourceforge.net License: GPL version 2 Keywords: plone caching
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
 :: Web Environment Classifier: Framework :: Plone Classifier: Framework ::
 Plone :: 6.0 Classifier: Framework :: Plone :: Core Classifier: Framework ::
 Zope :: 5 Classifier: License :: OSI Approved :: GNU General Public License v2
@@ -18,14 +18,44 @@
 pypi.org/project/plone.app.caching/) [![PyPI - License](https://img.shields.io/
 pypi/l/plone.app.caching)](https://pypi.org/project/plone.app.caching/) [![PyPI
    - Status](https://img.shields.io/pypi/status/plone.app.caching)](https://
      pypi.org/project/plone.app.caching/) [![GitHub contributors](https://
      img.shields.io/github/contributors/plone/plone.app.caching)](https://
        github.com/plone/plone.app.caching) ![GitHub Repo stars](https://
     img.shields.io/github/stars/plone/plone.app.caching?style=flat-square)
+## Introduction This package provides a Plone UI and default rules for managing
+HTTP response caching in Plone. It builds on [z3c.caching](https://github.com/
+zopefoundation/z3c.caching), [plone.caching](https://github.com/plone/
+plone.caching) and [plone.cachepurging](https://github.com/plone/
+plone.cachepurging). ### Compatibility | Version | Plone | |------|-----| | 3.x
+| 6.0 or above | | 2.x | 5.2 | | 1.x | 5.1, 5.0, 4.3, 4.2, 4.1 | ##
+Installation `plone.app.caching` is shipped as a dependency of the *Plone*
+package, and it should be available on all Plone installations, but Caching is
+**not enabled by default**, although it is highly recommended to configure
+caching for every new Plone site. After creating a new Plone site, go to `Site
+Setup`, then `Addons` and install `HTTP caching support`. Under the Advanced
+header, look for the Caching control panel -- currently only supported on the
+Classic UI. ### Troubleshooting When the Caching control panel is not there,
+there can be various reasons for this: - If your installation does not load the
+`Plone` package, but only `Products.CMFPlone`, then `plone.app.caching` is not
+included. - If the package *is* included, but you add a Plone Site using the
+advanced form and disable caching, then the control panel is not there. If you
+want to install it in an existing Plone Site: 1. Make sure the package is
+available in the Plone instance, by adding `plone.app.caching` or `Plone` to
+your installation. 2. From the Plone Site Setup go to the ZMI (Zope Management
+Interface). 3. Go to ``portal_setup``, and then to the Import tab. 4. Select
+the HTTP caching support profile, perhaps easiest by id: `profile-
+plone.app.caching:default`. 5. Click 'Import all steps'. ## Source Code
+Contributors, please read the document [Process for Plone core's development]
+(https://5.docs.plone.org/develop/coredev/docs/index.html) Sources are at the
+[Plone code repository hosted at Github ](https://github.com/plone/
+plone.app.caching). ## This project is supported by [Plone_Logo] ## License The
+project is licensed under GPLv2. # Changelog   ## 3.1.0 (2023-04-26) ### New
+features: - Update the resourceRegistries ETag to use the config registry
+modification time. This time is set since Plone 6.0.4. Fixes `issue 93
 ` in controlpanel. [petschki] (#112) - Revert changes to tests to work with the
 Zope security fix. We must have an empty byte, not text, otherwise it is an
 indication that we get a possibly wrong Content-Type in a 304 status. See `Zope
 issue 1089
 github.com/zopefoundation/Zope/issues/1089>`_. [maurits] (#1089) ## 3.0.1
 (2022-12-21) ### Bug fixes: - Fix tests to work with the Zope security fix.
 [maurits] (#106) ## 3.0.0 (2022-11-14) ### Bug fixes: - Add missing quotation
```

### Comparing `plone.app.caching-3.0.5/plone.app.caching.egg-info/SOURCES.txt` & `plone.app.caching-3.1.0/plone.app.caching.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.5/plone.app.caching.egg-info/requires.txt` & `plone.app.caching-3.1.0/plone.app.caching.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.5/pyproject.toml` & `plone.app.caching-3.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.5/setup.py` & `plone.app.caching-3.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pathlib import Path
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "3.0.5"
+version = "3.1.0"
 
 long_description = f"""
 {Path("README.md").read_text()}\n
 {Path("CHANGES.md").read_text()}\n
 """
 
 setup(
```

