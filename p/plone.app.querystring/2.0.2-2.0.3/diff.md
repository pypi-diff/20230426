# Comparing `tmp/plone.app.querystring-2.0.2.tar.gz` & `tmp/plone.app.querystring-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.app.querystring-2.0.2.tar", last modified: Tue Mar 21 22:44:22 2023, max compression
+gzip compressed data, was "plone.app.querystring-2.0.3.tar", last modified: Wed Apr 26 21:58:25 2023, max compression
```

## Comparing `plone.app.querystring-2.0.2.tar` & `plone.app.querystring-2.0.3.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 22:44:22.165848 plone.app.querystring-2.0.2/
--rw-r--r--   0 maurits    (501) staff       (20)    12162 2023-03-21 22:44:21.000000 plone.app.querystring-2.0.2/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2023-03-21 22:44:21.000000 plone.app.querystring-2.0.2/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      149 2023-03-21 22:44:21.000000 plone.app.querystring-2.0.2/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    14053 2023-03-21 22:44:22.165968 plone.app.querystring-2.0.2/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)      966 2023-03-21 22:44:21.000000 plone.app.querystring-2.0.2/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 22:44:22.149962 plone.app.querystring-2.0.2/docs/
--rw-r--r--   0 maurits    (501) staff       (20)    15220 2023-03-21 22:44:21.000000 plone.app.querystring-2.0.2/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      683 2023-03-21 22:44:21.000000 plone.app.querystring-2.0.2/docs/LICENSE.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 22:44:22.150232 plone.app.querystring-2.0.2/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-03-21 22:44:21.000000 plone.app.querystring-2.0.2/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 22:44:22.153390 plone.app.querystring-2.0.2/plone/app/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-03-21 22:44:21.000000 plone.app.querystring-2.0.2/plone/app/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 22:44:22.157424 plone.app.querystring-2.0.2/plone/app/querystring/
--rw-r--r--   0 maurits    (501) staff       (20)        2 2023-03-21 22:44:21.000000 plone.app.querystring-2.0.2/plone/app/querystring/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1692 2023-03-21 22:44:21.000000 plone.app.querystring-2.0.2/plone/app/querystring/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1020 2023-03-21 22:44:21.000000 plone.app.querystring-2.0.2/plone/app/querystring/hiddenprofiles.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 22:44:22.158266 plone.app.querystring-2.0.2/plone/app/querystring/indexmodifiers/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-03-21 22:44:21.000000 plone.app.querystring-2.0.2/plone/app/querystring/indexmodifiers/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1240 2023-03-21 22:44:21.000000 plone.app.querystring-2.0.2/plone/app/querystring/indexmodifiers/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     2644 2023-03-21 22:44:21.000000 plone.app.querystring-2.0.2/plone/app/querystring/indexmodifiers/query_index_modifiers.py
--rw-r--r--   0 maurits    (501) staff       (20)     1562 2023-03-21 22:44:21.000000 plone.app.querystring-2.0.2/plone/app/querystring/interfaces.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 22:44:22.144687 plone.app.querystring-2.0.2/plone/app/querystring/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 22:44:22.159014 plone.app.querystring-2.0.2/plone/app/querystring/profiles/default/
--rw-r--r--   0 maurits    (501) staff       (20)      185 2023-03-21 22:44:21.000000 plone.app.querystring-2.0.2/plone/app/querystring/profiles/default/metadata.xml
--rw-r--r--   0 maurits    (501) staff       (20)    32950 2023-03-21 22:44:21.000000 plone.app.querystring-2.0.2/plone/app/querystring/profiles/default/registry.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 22:44:22.146189 plone.app.querystring-2.0.2/plone/app/querystring/profiles/upgrades/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 22:44:22.159324 plone.app.querystring-2.0.2/plone/app/querystring/profiles/upgrades/to_10/
--rw-r--r--   0 maurits    (501) staff       (20)      539 2023-03-21 22:44:21.000000 plone.app.querystring-2.0.2/plone/app/querystring/profiles/upgrades/to_10/registry.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 22:44:22.159577 plone.app.querystring-2.0.2/plone/app/querystring/profiles/upgrades/to_11/
--rw-r--r--   0 maurits    (501) staff       (20)     3366 2023-03-21 22:44:21.000000 plone.app.querystring-2.0.2/plone/app/querystring/profiles/upgrades/to_11/registry.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 22:44:22.159820 plone.app.querystring-2.0.2/plone/app/querystring/profiles/upgrades/to_14/
--rw-r--r--   0 maurits    (501) staff       (20)     2961 2023-03-21 22:44:21.000000 plone.app.querystring-2.0.2/plone/app/querystring/profiles/upgrades/to_14/registry.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 22:44:22.160188 plone.app.querystring-2.0.2/plone/app/querystring/profiles/upgrades/to_3/
--rw-r--r--   0 maurits    (501) staff       (20)     1411 2023-03-21 22:44:21.000000 plone.app.querystring-2.0.2/plone/app/querystring/profiles/upgrades/to_3/registry.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 22:44:22.160434 plone.app.querystring-2.0.2/plone/app/querystring/profiles/upgrades/to_5/
--rw-r--r--   0 maurits    (501) staff       (20)     1819 2023-03-21 22:44:21.000000 plone.app.querystring-2.0.2/plone/app/querystring/profiles/upgrades/to_5/registry.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 22:44:22.160681 plone.app.querystring-2.0.2/plone/app/querystring/profiles/upgrades/to_6/
--rw-r--r--   0 maurits    (501) staff       (20)     1772 2023-03-21 22:44:21.000000 plone.app.querystring-2.0.2/plone/app/querystring/profiles/upgrades/to_6/registry.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 22:44:22.160927 plone.app.querystring-2.0.2/plone/app/querystring/profiles/upgrades/to_7/
--rw-r--r--   0 maurits    (501) staff       (20)      339 2023-03-21 22:44:21.000000 plone.app.querystring-2.0.2/plone/app/querystring/profiles/upgrades/to_7/registry.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 22:44:22.161180 plone.app.querystring-2.0.2/plone/app/querystring/profiles/upgrades/to_8/
--rw-r--r--   0 maurits    (501) staff       (20)     1818 2023-03-21 22:44:21.000000 plone.app.querystring-2.0.2/plone/app/querystring/profiles/upgrades/to_8/registry.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 22:44:22.161555 plone.app.querystring-2.0.2/plone/app/querystring/profiles/upgrades/to_9/
--rw-r--r--   0 maurits    (501) staff       (20)     1060 2023-03-21 22:44:21.000000 plone.app.querystring-2.0.2/plone/app/querystring/profiles/upgrades/to_9/registry.xml
--rw-r--r--   0 maurits    (501) staff       (20)     2785 2023-03-21 22:44:21.000000 plone.app.querystring-2.0.2/plone/app/querystring/profiles.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     9157 2023-03-21 22:44:21.000000 plone.app.querystring-2.0.2/plone/app/querystring/querybuilder.py
--rw-r--r--   0 maurits    (501) staff       (20)      715 2023-03-21 22:44:21.000000 plone.app.querystring-2.0.2/plone/app/querystring/querymodifiers.py
--rw-r--r--   0 maurits    (501) staff       (20)    10546 2023-03-21 22:44:21.000000 plone.app.querystring-2.0.2/plone/app/querystring/queryparser.py
--rw-r--r--   0 maurits    (501) staff       (20)     5128 2023-03-21 22:44:21.000000 plone.app.querystring-2.0.2/plone/app/querystring/registryreader.py
--rw-r--r--   0 maurits    (501) staff       (20)     4662 2023-03-21 22:44:21.000000 plone.app.querystring-2.0.2/plone/app/querystring/results.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2205 2023-03-21 22:44:21.000000 plone.app.querystring-2.0.2/plone/app/querystring/testing.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 22:44:22.165008 plone.app.querystring-2.0.2/plone/app/querystring/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-03-21 22:44:21.000000 plone.app.querystring-2.0.2/plone/app/querystring/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      481 2023-03-21 22:44:21.000000 plone.app.querystring-2.0.2/plone/app/querystring/tests/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      863 2023-03-21 22:44:21.000000 plone.app.querystring-2.0.2/plone/app/querystring/tests/index_testmodifier.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 22:44:22.146734 plone.app.querystring-2.0.2/plone/app/querystring/tests/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 22:44:22.165651 plone.app.querystring-2.0.2/plone/app/querystring/tests/profiles/registry/
--rw-r--r--   0 maurits    (501) staff       (20)      184 2023-03-21 22:44:21.000000 plone.app.querystring-2.0.2/plone/app/querystring/tests/profiles/registry/metadata.xml
--rw-r--r--   0 maurits    (501) staff       (20)     1283 2023-03-21 22:44:21.000000 plone.app.querystring-2.0.2/plone/app/querystring/tests/profiles/registry/registry.xml
--rw-r--r--   0 maurits    (501) staff       (20)     2202 2023-03-21 22:44:21.000000 plone.app.querystring-2.0.2/plone/app/querystring/tests/registry_minimal_correct.xml
--rw-r--r--   0 maurits    (501) staff       (20)      984 2023-03-21 22:44:21.000000 plone.app.querystring-2.0.2/plone/app/querystring/tests/registry_test_missing_operator.xml
--rw-r--r--   0 maurits    (501) staff       (20)     1000 2023-03-21 22:44:21.000000 plone.app.querystring-2.0.2/plone/app/querystring/tests/registry_test_vocabulary.xml
--rw-r--r--   0 maurits    (501) staff       (20)     2806 2023-03-21 22:44:21.000000 plone.app.querystring-2.0.2/plone/app/querystring/tests/registry_testdata.py
--rw-r--r--   0 maurits    (501) staff       (20)     2405 2023-03-21 22:44:21.000000 plone.app.querystring-2.0.2/plone/app/querystring/tests/testIndexmodifiers.py
--rw-r--r--   0 maurits    (501) staff       (20)    15001 2023-03-21 22:44:21.000000 plone.app.querystring-2.0.2/plone/app/querystring/tests/testQueryBuilder.py
--rw-r--r--   0 maurits    (501) staff       (20)     3515 2023-03-21 22:44:21.000000 plone.app.querystring-2.0.2/plone/app/querystring/tests/testQueryBuilderModifiers.py
--rw-r--r--   0 maurits    (501) staff       (20)    21787 2023-03-21 22:44:21.000000 plone.app.querystring-2.0.2/plone/app/querystring/tests/testQueryParser.py
--rw-r--r--   0 maurits    (501) staff       (20)     2941 2023-03-21 22:44:21.000000 plone.app.querystring-2.0.2/plone/app/querystring/tests/testRegistryIntegration.py
--rw-r--r--   0 maurits    (501) staff       (20)     5653 2023-03-21 22:44:21.000000 plone.app.querystring-2.0.2/plone/app/querystring/tests/testRegistryReader.py
--rw-r--r--   0 maurits    (501) staff       (20)     2178 2023-03-21 22:44:21.000000 plone.app.querystring-2.0.2/plone/app/querystring/upgrades.py
--rw-r--r--   0 maurits    (501) staff       (20)     5147 2023-03-21 22:44:21.000000 plone.app.querystring-2.0.2/plone/app/querystring/upgrades.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 22:44:22.153051 plone.app.querystring-2.0.2/plone.app.querystring.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    14053 2023-03-21 22:44:22.000000 plone.app.querystring-2.0.2/plone.app.querystring.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     2579 2023-03-21 22:44:22.000000 plone.app.querystring-2.0.2/plone.app.querystring.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-03-21 22:44:22.000000 plone.app.querystring-2.0.2/plone.app.querystring.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       40 2023-03-21 22:44:22.000000 plone.app.querystring-2.0.2/plone.app.querystring.egg-info/entry_points.txt
--rw-r--r--   0 maurits    (501) staff       (20)       16 2023-03-21 22:44:22.000000 plone.app.querystring-2.0.2/plone.app.querystring.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-03-21 22:44:22.000000 plone.app.querystring-2.0.2/plone.app.querystring.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      291 2023-03-21 22:44:22.000000 plone.app.querystring-2.0.2/plone.app.querystring.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-03-21 22:44:22.000000 plone.app.querystring-2.0.2/plone.app.querystring.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1690 2023-03-21 22:44:21.000000 plone.app.querystring-2.0.2/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)      217 2023-03-21 22:44:22.166459 plone.app.querystring-2.0.2/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     1990 2023-03-21 22:44:21.000000 plone.app.querystring-2.0.2/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:58:25.265349 plone.app.querystring-2.0.3/
+-rw-r--r--   0 maurits    (501) staff       (20)    12307 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      149 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    14198 2023-04-26 21:58:25.265502 plone.app.querystring-2.0.3/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)      966 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:58:25.243237 plone.app.querystring-2.0.3/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)    15220 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/docs/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      683 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/docs/LICENSE.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:58:25.243541 plone.app.querystring-2.0.3/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:58:25.247624 plone.app.querystring-2.0.3/plone/app/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:58:25.254094 plone.app.querystring-2.0.3/plone/app/querystring/
+-rw-r--r--   0 maurits    (501) staff       (20)        2 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1692 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     1020 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/hiddenprofiles.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:58:25.255499 plone.app.querystring-2.0.3/plone/app/querystring/indexmodifiers/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/indexmodifiers/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1240 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/indexmodifiers/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     2644 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/indexmodifiers/query_index_modifiers.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1562 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/interfaces.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:58:25.238587 plone.app.querystring-2.0.3/plone/app/querystring/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:58:25.256503 plone.app.querystring-2.0.3/plone/app/querystring/profiles/default/
+-rw-r--r--   0 maurits    (501) staff       (20)      185 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/profiles/default/metadata.xml
+-rw-r--r--   0 maurits    (501) staff       (20)    32950 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/profiles/default/registry.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:58:25.240017 plone.app.querystring-2.0.3/plone/app/querystring/profiles/upgrades/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:58:25.257157 plone.app.querystring-2.0.3/plone/app/querystring/profiles/upgrades/to_10/
+-rw-r--r--   0 maurits    (501) staff       (20)      539 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/profiles/upgrades/to_10/registry.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:58:25.257680 plone.app.querystring-2.0.3/plone/app/querystring/profiles/upgrades/to_11/
+-rw-r--r--   0 maurits    (501) staff       (20)     3366 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/profiles/upgrades/to_11/registry.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:58:25.258242 plone.app.querystring-2.0.3/plone/app/querystring/profiles/upgrades/to_14/
+-rw-r--r--   0 maurits    (501) staff       (20)     2961 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/profiles/upgrades/to_14/registry.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:58:25.258736 plone.app.querystring-2.0.3/plone/app/querystring/profiles/upgrades/to_3/
+-rw-r--r--   0 maurits    (501) staff       (20)     1411 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/profiles/upgrades/to_3/registry.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:58:25.259098 plone.app.querystring-2.0.3/plone/app/querystring/profiles/upgrades/to_5/
+-rw-r--r--   0 maurits    (501) staff       (20)     1819 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/profiles/upgrades/to_5/registry.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:58:25.259434 plone.app.querystring-2.0.3/plone/app/querystring/profiles/upgrades/to_6/
+-rw-r--r--   0 maurits    (501) staff       (20)     1772 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/profiles/upgrades/to_6/registry.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:58:25.259775 plone.app.querystring-2.0.3/plone/app/querystring/profiles/upgrades/to_7/
+-rw-r--r--   0 maurits    (501) staff       (20)      339 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/profiles/upgrades/to_7/registry.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:58:25.260093 plone.app.querystring-2.0.3/plone/app/querystring/profiles/upgrades/to_8/
+-rw-r--r--   0 maurits    (501) staff       (20)     1818 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/profiles/upgrades/to_8/registry.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:58:25.260413 plone.app.querystring-2.0.3/plone/app/querystring/profiles/upgrades/to_9/
+-rw-r--r--   0 maurits    (501) staff       (20)     1060 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/profiles/upgrades/to_9/registry.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     2785 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/profiles.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     9157 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/querybuilder.py
+-rw-r--r--   0 maurits    (501) staff       (20)      715 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/querymodifiers.py
+-rw-r--r--   0 maurits    (501) staff       (20)    10543 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/queryparser.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5128 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/registryreader.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4662 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/results.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     2205 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/testing.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:58:25.264479 plone.app.querystring-2.0.3/plone/app/querystring/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      481 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/tests/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      863 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/tests/index_testmodifier.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:58:25.240488 plone.app.querystring-2.0.3/plone/app/querystring/tests/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:58:25.265090 plone.app.querystring-2.0.3/plone/app/querystring/tests/profiles/registry/
+-rw-r--r--   0 maurits    (501) staff       (20)      184 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/tests/profiles/registry/metadata.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     1283 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/tests/profiles/registry/registry.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     2202 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/tests/registry_minimal_correct.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      984 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/tests/registry_test_missing_operator.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     1000 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/tests/registry_test_vocabulary.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     2806 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/tests/registry_testdata.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2405 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/tests/testIndexmodifiers.py
+-rw-r--r--   0 maurits    (501) staff       (20)    15001 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/tests/testQueryBuilder.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3515 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/tests/testQueryBuilderModifiers.py
+-rw-r--r--   0 maurits    (501) staff       (20)    21787 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/tests/testQueryParser.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2941 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/tests/testRegistryIntegration.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5653 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/tests/testRegistryReader.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2178 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/upgrades.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5147 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/upgrades.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:58:25.247137 plone.app.querystring-2.0.3/plone.app.querystring.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    14198 2023-04-26 21:58:25.000000 plone.app.querystring-2.0.3/plone.app.querystring.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     2579 2023-04-26 21:58:25.000000 plone.app.querystring-2.0.3/plone.app.querystring.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-26 21:58:25.000000 plone.app.querystring-2.0.3/plone.app.querystring.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       40 2023-04-26 21:58:25.000000 plone.app.querystring-2.0.3/plone.app.querystring.egg-info/entry_points.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       16 2023-04-26 21:58:25.000000 plone.app.querystring-2.0.3/plone.app.querystring.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-26 21:58:25.000000 plone.app.querystring-2.0.3/plone.app.querystring.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      274 2023-04-26 21:58:25.000000 plone.app.querystring-2.0.3/plone.app.querystring.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-04-26 21:58:25.000000 plone.app.querystring-2.0.3/plone.app.querystring.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1690 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)      217 2023-04-26 21:58:25.266117 plone.app.querystring-2.0.3/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     1962 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/setup.py
```

### Comparing `plone.app.querystring-2.0.2/CHANGES.rst` & `plone.app.querystring-2.0.3/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+2.0.3 (2023-04-26)
+------------------
+
+Bug fixes:
+
+
+- Fix cyclic dependency, do not depend on `plone.app.layout`.
+  [@jensens] (rm-cyclic-dep)
+
+
 2.0.2 (2023-03-21)
 ------------------
 
 Bug fixes:
 
 
 - Housecleaning: pyupgrade, isort, black, remove six, move imports from CMFPlone to plone.base, copy munge_search_terms from CMFPlone to here to avoid dependency on CMFPlone.
```

### Comparing `plone.app.querystring-2.0.2/PKG-INFO` & `plone.app.querystring-2.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.querystring
-Version: 2.0.2
+Version: 2.0.3
 Summary: A queryparser, querybuilder and extra helper tools, to parse stored queries to actual results, used in new style Plone collections
 Home-page: https://github.com/plone/plone.app.querystring
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: collection queries
 Classifier: Development Status :: 5 - Production/Stable
@@ -59,14 +59,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+2.0.3 (2023-04-26)
+------------------
+
+Bug fixes:
+
+
+- Fix cyclic dependency, do not depend on `plone.app.layout`.
+  [@jensens] (rm-cyclic-dep)
+
+
 2.0.2 (2023-03-21)
 ------------------
 
 Bug fixes:
 
 
 - Housecleaning: pyupgrade, isort, black, remove six, move imports from CMFPlone to plone.base, copy munge_search_terms from CMFPlone to here to avoid dependency on CMFPlone.
```

### Comparing `plone.app.querystring-2.0.2/README.rst` & `plone.app.querystring-2.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.2/docs/LICENSE.GPL` & `plone.app.querystring-2.0.3/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.2/docs/LICENSE.txt` & `plone.app.querystring-2.0.3/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.2/plone/app/querystring/configure.zcml` & `plone.app.querystring-2.0.3/plone/app/querystring/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.2/plone/app/querystring/hiddenprofiles.py` & `plone.app.querystring-2.0.3/plone/app/querystring/hiddenprofiles.py`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.2/plone/app/querystring/indexmodifiers/configure.zcml` & `plone.app.querystring-2.0.3/plone/app/querystring/indexmodifiers/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.2/plone/app/querystring/indexmodifiers/query_index_modifiers.py` & `plone.app.querystring-2.0.3/plone/app/querystring/indexmodifiers/query_index_modifiers.py`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.2/plone/app/querystring/interfaces.py` & `plone.app.querystring-2.0.3/plone/app/querystring/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.2/plone/app/querystring/profiles/default/registry.xml` & `plone.app.querystring-2.0.3/plone/app/querystring/profiles/default/registry.xml`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.2/plone/app/querystring/profiles/upgrades/to_10/registry.xml` & `plone.app.querystring-2.0.3/plone/app/querystring/profiles/upgrades/to_10/registry.xml`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.2/plone/app/querystring/profiles/upgrades/to_11/registry.xml` & `plone.app.querystring-2.0.3/plone/app/querystring/profiles/upgrades/to_11/registry.xml`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.2/plone/app/querystring/profiles/upgrades/to_14/registry.xml` & `plone.app.querystring-2.0.3/plone/app/querystring/profiles/upgrades/to_14/registry.xml`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.2/plone/app/querystring/profiles/upgrades/to_3/registry.xml` & `plone.app.querystring-2.0.3/plone/app/querystring/profiles/upgrades/to_3/registry.xml`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.2/plone/app/querystring/profiles/upgrades/to_5/registry.xml` & `plone.app.querystring-2.0.3/plone/app/querystring/profiles/upgrades/to_5/registry.xml`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.2/plone/app/querystring/profiles/upgrades/to_6/registry.xml` & `plone.app.querystring-2.0.3/plone/app/querystring/profiles/upgrades/to_6/registry.xml`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.2/plone/app/querystring/profiles/upgrades/to_8/registry.xml` & `plone.app.querystring-2.0.3/plone/app/querystring/profiles/upgrades/to_8/registry.xml`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.2/plone/app/querystring/profiles/upgrades/to_9/registry.xml` & `plone.app.querystring-2.0.3/plone/app/querystring/profiles/upgrades/to_9/registry.xml`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.2/plone/app/querystring/profiles.zcml` & `plone.app.querystring-2.0.3/plone/app/querystring/profiles.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.2/plone/app/querystring/querybuilder.py` & `plone.app.querystring-2.0.3/plone/app/querystring/querybuilder.py`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.2/plone/app/querystring/querymodifiers.py` & `plone.app.querystring-2.0.3/plone/app/querystring/querymodifiers.py`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.2/plone/app/querystring/queryparser.py` & `plone.app.querystring-2.0.3/plone/app/querystring/queryparser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from Acquisition import aq_parent
 from collections import namedtuple
 from DateTime import DateTime
 from DateTime.interfaces import DateTimeError
-from plone.app.layout.navigation.root import getNavigationRoot
 from plone.base.interfaces import IPloneSiteRoot
+from plone.base.navigationroot import get_navigation_root
 from plone.base.utils import base_hasattr
 from plone.registry.interfaces import IRegistry
 from plone.uuid.interfaces import IUUID
 from Products.CMFCore.utils import getToolByName
 from zope.component import getUtility
 from zope.dottedname.resolve import resolve
 
@@ -320,15 +320,15 @@
     portal_url = getToolByName(context, "portal_url")
     portal = portal_url.getPortalObject()
     root = "/".join(portal.getPhysicalPath())
     return _pathByRoot(root, context, row)
 
 
 def _navigationPath(context, row):
-    return _pathByRoot(getNavigationRoot(context), context, row)
+    return _pathByRoot(get_navigation_root(context), context, row)
 
 
 def _relativePath(context, row):
     # Walk through the tree
     obj = context
     values = row.values
     depthstr = ""
```

### Comparing `plone.app.querystring-2.0.2/plone/app/querystring/registryreader.py` & `plone.app.querystring-2.0.3/plone/app/querystring/registryreader.py`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.2/plone/app/querystring/results.pt` & `plone.app.querystring-2.0.3/plone/app/querystring/results.pt`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.2/plone/app/querystring/testing.py` & `plone.app.querystring-2.0.3/plone/app/querystring/testing.py`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.2/plone/app/querystring/tests/index_testmodifier.py` & `plone.app.querystring-2.0.3/plone/app/querystring/tests/index_testmodifier.py`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.2/plone/app/querystring/tests/profiles/registry/registry.xml` & `plone.app.querystring-2.0.3/plone/app/querystring/tests/profiles/registry/registry.xml`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.2/plone/app/querystring/tests/registry_minimal_correct.xml` & `plone.app.querystring-2.0.3/plone/app/querystring/tests/registry_minimal_correct.xml`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.2/plone/app/querystring/tests/registry_test_missing_operator.xml` & `plone.app.querystring-2.0.3/plone/app/querystring/tests/registry_test_missing_operator.xml`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.2/plone/app/querystring/tests/registry_test_vocabulary.xml` & `plone.app.querystring-2.0.3/plone/app/querystring/tests/registry_test_vocabulary.xml`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.2/plone/app/querystring/tests/registry_testdata.py` & `plone.app.querystring-2.0.3/plone/app/querystring/tests/registry_testdata.py`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.2/plone/app/querystring/tests/testIndexmodifiers.py` & `plone.app.querystring-2.0.3/plone/app/querystring/tests/testIndexmodifiers.py`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.2/plone/app/querystring/tests/testQueryBuilder.py` & `plone.app.querystring-2.0.3/plone/app/querystring/tests/testQueryBuilder.py`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.2/plone/app/querystring/tests/testQueryBuilderModifiers.py` & `plone.app.querystring-2.0.3/plone/app/querystring/tests/testQueryBuilderModifiers.py`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.2/plone/app/querystring/tests/testQueryParser.py` & `plone.app.querystring-2.0.3/plone/app/querystring/tests/testQueryParser.py`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.2/plone/app/querystring/tests/testRegistryIntegration.py` & `plone.app.querystring-2.0.3/plone/app/querystring/tests/testRegistryIntegration.py`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.2/plone/app/querystring/tests/testRegistryReader.py` & `plone.app.querystring-2.0.3/plone/app/querystring/tests/testRegistryReader.py`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.2/plone/app/querystring/upgrades.py` & `plone.app.querystring-2.0.3/plone/app/querystring/upgrades.py`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.2/plone/app/querystring/upgrades.zcml` & `plone.app.querystring-2.0.3/plone/app/querystring/upgrades.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.2/plone.app.querystring.egg-info/PKG-INFO` & `plone.app.querystring-2.0.3/plone.app.querystring.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.querystring
-Version: 2.0.2
+Version: 2.0.3
 Summary: A queryparser, querybuilder and extra helper tools, to parse stored queries to actual results, used in new style Plone collections
 Home-page: https://github.com/plone/plone.app.querystring
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: collection queries
 Classifier: Development Status :: 5 - Production/Stable
@@ -59,14 +59,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+2.0.3 (2023-04-26)
+------------------
+
+Bug fixes:
+
+
+- Fix cyclic dependency, do not depend on `plone.app.layout`.
+  [@jensens] (rm-cyclic-dep)
+
+
 2.0.2 (2023-03-21)
 ------------------
 
 Bug fixes:
 
 
 - Housecleaning: pyupgrade, isort, black, remove six, move imports from CMFPlone to plone.base, copy munge_search_terms from CMFPlone to here to avoid dependency on CMFPlone.
```

### Comparing `plone.app.querystring-2.0.2/plone.app.querystring.egg-info/SOURCES.txt` & `plone.app.querystring-2.0.3/plone.app.querystring.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.2/pyproject.toml` & `plone.app.querystring-2.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.2/setup.py` & `plone.app.querystring-2.0.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "2.0.2"
+version = "2.0.3"
 
 long_description = open("README.rst").read() + "\n"
 long_description += open("CHANGES.rst").read()
 
 setup(
     name="plone.app.querystring",
     version=version,
@@ -37,15 +37,14 @@
     namespace_packages=["plone", "plone.app"],
     include_package_data=True,
     zip_safe=False,
     python_requires=">=3.8",
     install_requires=[
         "setuptools",
         "plone.app.contentlisting",
-        "plone.app.layout",
         "plone.app.registry>=1.1",
         "plone.base",
         "plone.batching",
         "plone.i18n",
         "plone.registry",
         "plone.uuid",
         "Products.GenericSetup",
```

