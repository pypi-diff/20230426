# Comparing `tmp/threatingestor-1.0.3.tar.gz` & `tmp/threatingestor-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threatingestor-1.0.3.tar", last modified: Mon Feb 20 11:54:35 2023, max compression
+gzip compressed data, was "threatingestor-1.1.0.tar", last modified: Wed Apr 26 13:27:30 2023, max compression
```

## Comparing `threatingestor-1.0.3.tar` & `threatingestor-1.1.0.tar`

### file list

```diff
@@ -1,79 +1,78 @@
-drwxr-xr-x   0 azazel     (501) staff       (20)        0 2023-02-20 11:54:35.671560 threatingestor-1.0.3/
--rw-r--r--   0 azazel     (501) staff       (20)    18046 2023-02-08 03:48:03.000000 threatingestor-1.0.3/LICENSE
--rw-r--r--   0 azazel     (501) staff       (20)       93 2023-02-08 03:48:03.000000 threatingestor-1.0.3/MANIFEST.in
--rw-r--r--   0 azazel     (501) staff       (20)     8930 2023-02-20 11:54:35.671256 threatingestor-1.0.3/PKG-INFO
--rw-r--r--   0 azazel     (501) staff       (20)     7979 2023-02-08 03:48:03.000000 threatingestor-1.0.3/README.rst
--rw-r--r--   0 azazel     (501) staff       (20)      184 2023-02-14 23:09:31.000000 threatingestor-1.0.3/requirements-testing.txt
--rw-r--r--   0 azazel     (501) staff       (20)      168 2023-02-14 23:09:31.000000 threatingestor-1.0.3/requirements.txt
--rw-r--r--   0 azazel     (501) staff       (20)       38 2023-02-20 11:54:35.671606 threatingestor-1.0.3/setup.cfg
--rw-r--r--   0 azazel     (501) staff       (20)     2049 2023-02-20 10:48:57.000000 threatingestor-1.0.3/setup.py
-drwxr-xr-x   0 azazel     (501) staff       (20)        0 2023-02-20 11:54:35.662152 threatingestor-1.0.3/tests/
--rw-r--r--   0 azazel     (501) staff       (20)    18862 2023-02-08 03:48:03.000000 threatingestor-1.0.3/tests/test_artifacts.py
--rw-r--r--   0 azazel     (501) staff       (20)     8942 2023-02-08 03:48:03.000000 threatingestor-1.0.3/tests/test_config.py
--rw-r--r--   0 azazel     (501) staff       (20)     2468 2023-02-08 03:48:03.000000 threatingestor-1.0.3/tests/test_ingestor.py
--rw-r--r--   0 azazel     (501) staff       (20)     7191 2023-02-08 03:48:03.000000 threatingestor-1.0.3/tests/test_operators.py
--rw-r--r--   0 azazel     (501) staff       (20)     4234 2023-02-08 03:48:03.000000 threatingestor-1.0.3/tests/test_operators_abstract_json.py
--rw-r--r--   0 azazel     (501) staff       (20)      562 2023-02-08 03:48:03.000000 threatingestor-1.0.3/tests/test_operators_beanstalk.py
--rw-r--r--   0 azazel     (501) staff       (20)     1069 2023-02-08 03:48:03.000000 threatingestor-1.0.3/tests/test_operators_csv.py
--rw-r--r--   0 azazel     (501) staff       (20)     4728 2023-02-08 03:48:03.000000 threatingestor-1.0.3/tests/test_operators_misp.py
--rw-r--r--   0 azazel     (501) staff       (20)     1397 2023-02-08 03:48:03.000000 threatingestor-1.0.3/tests/test_operators_mysql.py
--rw-r--r--   0 azazel     (501) staff       (20)     3486 2023-02-08 03:48:03.000000 threatingestor-1.0.3/tests/test_operators_sqlite.py
--rw-r--r--   0 azazel     (501) staff       (20)     4051 2023-02-08 03:48:03.000000 threatingestor-1.0.3/tests/test_operators_sqs.py
--rw-r--r--   0 azazel     (501) staff       (20)     2112 2023-02-08 03:48:03.000000 threatingestor-1.0.3/tests/test_operators_threatkb.py
--rw-r--r--   0 azazel     (501) staff       (20)     3465 2023-02-08 03:48:03.000000 threatingestor-1.0.3/tests/test_operators_twitter.py
--rw-r--r--   0 azazel     (501) staff       (20)     6991 2023-02-08 03:48:03.000000 threatingestor-1.0.3/tests/test_sources.py
--rw-r--r--   0 azazel     (501) staff       (20)      834 2023-02-08 03:48:03.000000 threatingestor-1.0.3/tests/test_sources_beanstalk.py
--rw-r--r--   0 azazel     (501) staff       (20)     3899 2023-02-08 03:48:03.000000 threatingestor-1.0.3/tests/test_sources_git.py
--rw-r--r--   0 azazel     (501) staff       (20)     3283 2023-02-08 03:48:03.000000 threatingestor-1.0.3/tests/test_sources_github.py
--rw-r--r--   0 azazel     (501) staff       (20)     2118 2023-02-08 03:48:03.000000 threatingestor-1.0.3/tests/test_sources_json.py
--rw-r--r--   0 azazel     (501) staff       (20)     6835 2023-02-08 03:48:03.000000 threatingestor-1.0.3/tests/test_sources_rss.py
--rw-r--r--   0 azazel     (501) staff       (20)      893 2023-02-08 03:48:03.000000 threatingestor-1.0.3/tests/test_sources_sqs.py
--rw-r--r--   0 azazel     (501) staff       (20)     6382 2023-02-08 03:48:03.000000 threatingestor-1.0.3/tests/test_sources_twitter.py
--rw-r--r--   0 azazel     (501) staff       (20)     2653 2023-02-08 03:48:03.000000 threatingestor-1.0.3/tests/test_sources_web.py
--rw-r--r--   0 azazel     (501) staff       (20)     1089 2023-02-08 03:48:03.000000 threatingestor-1.0.3/tests/test_state.py
--rw-r--r--   0 azazel     (501) staff       (20)      459 2023-02-08 03:48:03.000000 threatingestor-1.0.3/tests/test_whitelist.py
-drwxr-xr-x   0 azazel     (501) staff       (20)        0 2023-02-20 11:54:35.663643 threatingestor-1.0.3/threatingestor/
--rw-r--r--   0 azazel     (501) staff       (20)     6886 2023-02-08 03:48:03.000000 threatingestor-1.0.3/threatingestor/__init__.py
--rw-r--r--   0 azazel     (501) staff       (20)    10006 2023-02-08 03:48:03.000000 threatingestor-1.0.3/threatingestor/artifacts.py
--rw-r--r--   0 azazel     (501) staff       (20)     5493 2023-02-08 03:48:03.000000 threatingestor-1.0.3/threatingestor/config.py
--rw-r--r--   0 azazel     (501) staff       (20)      221 2023-02-08 03:48:03.000000 threatingestor-1.0.3/threatingestor/exceptions.py
-drwxr-xr-x   0 azazel     (501) staff       (20)        0 2023-02-20 11:54:35.665269 threatingestor-1.0.3/threatingestor/extras/
--rw-r--r--   0 azazel     (501) staff       (20)        0 2023-02-08 03:48:03.000000 threatingestor-1.0.3/threatingestor/extras/__init__.py
--rw-r--r--   0 azazel     (501) staff       (20)     1231 2023-02-08 03:48:03.000000 threatingestor-1.0.3/threatingestor/extras/fswatcher.py
--rw-r--r--   0 azazel     (501) staff       (20)     1086 2023-02-08 03:48:03.000000 threatingestor-1.0.3/threatingestor/extras/pasteprocessor.py
--rw-r--r--   0 azazel     (501) staff       (20)     4922 2023-02-08 03:48:03.000000 threatingestor-1.0.3/threatingestor/extras/queueworker.py
--rw-r--r--   0 azazel     (501) staff       (20)     2902 2023-02-08 03:48:03.000000 threatingestor-1.0.3/threatingestor/extras/webapp.py
-drwxr-xr-x   0 azazel     (501) staff       (20)        0 2023-02-20 11:54:35.668093 threatingestor-1.0.3/threatingestor/operators/
--rw-r--r--   0 azazel     (501) staff       (20)     2848 2023-02-08 03:48:03.000000 threatingestor-1.0.3/threatingestor/operators/__init__.py
--rw-r--r--   0 azazel     (501) staff       (20)      929 2023-02-08 03:48:03.000000 threatingestor-1.0.3/threatingestor/operators/abstract_json.py
--rw-r--r--   0 azazel     (501) staff       (20)     1132 2023-02-08 03:48:03.000000 threatingestor-1.0.3/threatingestor/operators/beanstalk.py
--rw-r--r--   0 azazel     (501) staff       (20)     1077 2023-02-08 03:48:03.000000 threatingestor-1.0.3/threatingestor/operators/csv.py
--rw-r--r--   0 azazel     (501) staff       (20)     4883 2023-02-08 03:48:03.000000 threatingestor-1.0.3/threatingestor/operators/misp.py
--rw-r--r--   0 azazel     (501) staff       (20)     3586 2023-02-08 03:48:03.000000 threatingestor-1.0.3/threatingestor/operators/mysql.py
--rw-r--r--   0 azazel     (501) staff       (20)     2297 2023-02-08 03:48:03.000000 threatingestor-1.0.3/threatingestor/operators/sqlite.py
--rw-r--r--   0 azazel     (501) staff       (20)     1393 2023-02-08 03:48:03.000000 threatingestor-1.0.3/threatingestor/operators/sqs.py
--rw-r--r--   0 azazel     (501) staff       (20)     3281 2023-02-08 03:48:03.000000 threatingestor-1.0.3/threatingestor/operators/threatkb.py
--rw-r--r--   0 azazel     (501) staff       (20)     2082 2023-02-08 03:48:03.000000 threatingestor-1.0.3/threatingestor/operators/twitter.py
-drwxr-xr-x   0 azazel     (501) staff       (20)        0 2023-02-20 11:54:35.670966 threatingestor-1.0.3/threatingestor/sources/
--rw-r--r--   0 azazel     (501) staff       (20)     6580 2023-02-08 03:48:03.000000 threatingestor-1.0.3/threatingestor/sources/__init__.py
--rw-r--r--   0 azazel     (501) staff       (20)     1656 2023-02-08 03:48:03.000000 threatingestor-1.0.3/threatingestor/sources/abstract_json.py
--rw-r--r--   0 azazel     (501) staff       (20)     1307 2023-02-08 03:48:03.000000 threatingestor-1.0.3/threatingestor/sources/beanstalk.py
--rw-r--r--   0 azazel     (501) staff       (20)     3652 2023-02-08 03:48:03.000000 threatingestor-1.0.3/threatingestor/sources/git.py
--rw-r--r--   0 azazel     (501) staff       (20)     2235 2023-02-08 03:48:03.000000 threatingestor-1.0.3/threatingestor/sources/github.py
--rw-r--r--   0 azazel     (501) staff       (20)     1634 2023-02-20 09:38:14.000000 threatingestor-1.0.3/threatingestor/sources/github_gist.py
--rw-r--r--   0 azazel     (501) staff       (20)     2166 2023-02-08 03:48:03.000000 threatingestor-1.0.3/threatingestor/sources/image.py
--rw-r--r--   0 azazel     (501) staff       (20)     2326 2023-02-20 09:55:32.000000 threatingestor-1.0.3/threatingestor/sources/rss.py
--rw-r--r--   0 azazel     (501) staff       (20)     3347 2023-02-14 23:09:31.000000 threatingestor-1.0.3/threatingestor/sources/sitemap.py
--rw-r--r--   0 azazel     (501) staff       (20)     1135 2023-02-08 03:48:03.000000 threatingestor-1.0.3/threatingestor/sources/sqs.py
--rw-r--r--   0 azazel     (501) staff       (20)     3675 2023-02-20 10:38:47.000000 threatingestor-1.0.3/threatingestor/sources/twitter.py
--rw-r--r--   0 azazel     (501) staff       (20)     4027 2023-02-20 09:58:12.000000 threatingestor-1.0.3/threatingestor/sources/twitter_follow_links.py
--rw-r--r--   0 azazel     (501) staff       (20)     1444 2023-02-08 03:48:03.000000 threatingestor-1.0.3/threatingestor/sources/web.py
--rw-r--r--   0 azazel     (501) staff       (20)     1254 2023-02-08 03:48:03.000000 threatingestor-1.0.3/threatingestor/state.py
--rw-r--r--   0 azazel     (501) staff       (20)      848 2023-02-08 03:48:03.000000 threatingestor-1.0.3/threatingestor/whitelist.py
-drwxr-xr-x   0 azazel     (501) staff       (20)        0 2023-02-20 11:54:35.664502 threatingestor-1.0.3/threatingestor.egg-info/
--rw-r--r--   0 azazel     (501) staff       (20)     8930 2023-02-20 11:54:35.000000 threatingestor-1.0.3/threatingestor.egg-info/PKG-INFO
--rw-r--r--   0 azazel     (501) staff       (20)     2118 2023-02-20 11:54:35.000000 threatingestor-1.0.3/threatingestor.egg-info/SOURCES.txt
--rw-r--r--   0 azazel     (501) staff       (20)        1 2023-02-20 11:54:35.000000 threatingestor-1.0.3/threatingestor.egg-info/dependency_links.txt
--rw-r--r--   0 azazel     (501) staff       (20)       55 2023-02-20 11:54:35.000000 threatingestor-1.0.3/threatingestor.egg-info/entry_points.txt
--rw-r--r--   0 azazel     (501) staff       (20)      527 2023-02-20 11:54:35.000000 threatingestor-1.0.3/threatingestor.egg-info/requires.txt
--rw-r--r--   0 azazel     (501) staff       (20)       15 2023-02-20 11:54:35.000000 threatingestor-1.0.3/threatingestor.egg-info/top_level.txt
+drwxr-xr-x   0 azazel     (501) staff       (20)        0 2023-04-26 13:27:30.770909 threatingestor-1.1.0/
+-rw-r--r--   0 azazel     (501) staff       (20)    18046 2023-04-26 13:26:17.000000 threatingestor-1.1.0/LICENSE
+-rw-r--r--   0 azazel     (501) staff       (20)       92 2023-04-26 13:27:18.000000 threatingestor-1.1.0/MANIFEST.in
+-rw-r--r--   0 azazel     (501) staff       (20)     8311 2023-04-26 13:27:30.770720 threatingestor-1.1.0/PKG-INFO
+-rw-r--r--   0 azazel     (501) staff       (20)     7320 2023-04-26 13:27:18.000000 threatingestor-1.1.0/README.md
+-rw-r--r--   0 azazel     (501) staff       (20)      184 2023-04-26 13:26:17.000000 threatingestor-1.1.0/requirements-testing.txt
+-rw-r--r--   0 azazel     (501) staff       (20)      144 2023-04-26 13:27:18.000000 threatingestor-1.1.0/requirements.txt
+-rw-r--r--   0 azazel     (501) staff       (20)       38 2023-04-26 13:27:30.770951 threatingestor-1.1.0/setup.cfg
+-rw-r--r--   0 azazel     (501) staff       (20)     2082 2023-04-26 13:27:18.000000 threatingestor-1.1.0/setup.py
+drwxr-xr-x   0 azazel     (501) staff       (20)        0 2023-04-26 13:27:30.766080 threatingestor-1.1.0/tests/
+-rw-r--r--   0 azazel     (501) staff       (20)    18861 2023-04-26 13:27:18.000000 threatingestor-1.1.0/tests/test_artifacts.py
+-rw-r--r--   0 azazel     (501) staff       (20)     8942 2023-04-26 13:26:17.000000 threatingestor-1.1.0/tests/test_config.py
+-rw-r--r--   0 azazel     (501) staff       (20)     2468 2023-04-26 13:26:17.000000 threatingestor-1.1.0/tests/test_ingestor.py
+-rw-r--r--   0 azazel     (501) staff       (20)     7191 2023-04-26 13:26:17.000000 threatingestor-1.1.0/tests/test_operators.py
+-rw-r--r--   0 azazel     (501) staff       (20)     4234 2023-04-26 13:26:17.000000 threatingestor-1.1.0/tests/test_operators_abstract_json.py
+-rw-r--r--   0 azazel     (501) staff       (20)      562 2023-04-26 13:26:17.000000 threatingestor-1.1.0/tests/test_operators_beanstalk.py
+-rw-r--r--   0 azazel     (501) staff       (20)     1069 2023-04-26 13:26:17.000000 threatingestor-1.1.0/tests/test_operators_csv.py
+-rw-r--r--   0 azazel     (501) staff       (20)     4728 2023-04-26 13:26:17.000000 threatingestor-1.1.0/tests/test_operators_misp.py
+-rw-r--r--   0 azazel     (501) staff       (20)     1397 2023-04-26 13:26:17.000000 threatingestor-1.1.0/tests/test_operators_mysql.py
+-rw-r--r--   0 azazel     (501) staff       (20)     3486 2023-04-26 13:26:17.000000 threatingestor-1.1.0/tests/test_operators_sqlite.py
+-rw-r--r--   0 azazel     (501) staff       (20)     4051 2023-04-26 13:26:17.000000 threatingestor-1.1.0/tests/test_operators_sqs.py
+-rw-r--r--   0 azazel     (501) staff       (20)     2112 2023-04-26 13:26:17.000000 threatingestor-1.1.0/tests/test_operators_threatkb.py
+-rw-r--r--   0 azazel     (501) staff       (20)     3465 2023-04-26 13:26:17.000000 threatingestor-1.1.0/tests/test_operators_twitter.py
+-rw-r--r--   0 azazel     (501) staff       (20)     6991 2023-04-26 13:26:17.000000 threatingestor-1.1.0/tests/test_sources.py
+-rw-r--r--   0 azazel     (501) staff       (20)      834 2023-04-26 13:26:17.000000 threatingestor-1.1.0/tests/test_sources_beanstalk.py
+-rw-r--r--   0 azazel     (501) staff       (20)     3899 2023-04-26 13:26:17.000000 threatingestor-1.1.0/tests/test_sources_git.py
+-rw-r--r--   0 azazel     (501) staff       (20)     3283 2023-04-26 13:26:17.000000 threatingestor-1.1.0/tests/test_sources_github.py
+-rw-r--r--   0 azazel     (501) staff       (20)     2118 2023-04-26 13:26:17.000000 threatingestor-1.1.0/tests/test_sources_json.py
+-rw-r--r--   0 azazel     (501) staff       (20)      893 2023-04-26 13:26:17.000000 threatingestor-1.1.0/tests/test_sources_sqs.py
+-rw-r--r--   0 azazel     (501) staff       (20)     6382 2023-04-26 13:26:17.000000 threatingestor-1.1.0/tests/test_sources_twitter.py
+-rw-r--r--   0 azazel     (501) staff       (20)     2653 2023-04-26 13:26:17.000000 threatingestor-1.1.0/tests/test_sources_web.py
+-rw-r--r--   0 azazel     (501) staff       (20)     1089 2023-04-26 13:26:17.000000 threatingestor-1.1.0/tests/test_state.py
+-rw-r--r--   0 azazel     (501) staff       (20)      459 2023-04-26 13:26:17.000000 threatingestor-1.1.0/tests/test_whitelist.py
+drwxr-xr-x   0 azazel     (501) staff       (20)        0 2023-04-26 13:27:30.766722 threatingestor-1.1.0/threatingestor/
+-rw-r--r--   0 azazel     (501) staff       (20)     6885 2023-04-26 13:27:18.000000 threatingestor-1.1.0/threatingestor/__init__.py
+-rw-r--r--   0 azazel     (501) staff       (20)    10377 2023-04-26 13:27:18.000000 threatingestor-1.1.0/threatingestor/artifacts.py
+-rw-r--r--   0 azazel     (501) staff       (20)     5490 2023-04-26 13:27:18.000000 threatingestor-1.1.0/threatingestor/config.py
+-rw-r--r--   0 azazel     (501) staff       (20)      221 2023-04-26 13:26:17.000000 threatingestor-1.1.0/threatingestor/exceptions.py
+drwxr-xr-x   0 azazel     (501) staff       (20)        0 2023-04-26 13:27:30.767803 threatingestor-1.1.0/threatingestor/extras/
+-rw-r--r--   0 azazel     (501) staff       (20)        0 2023-04-26 13:26:17.000000 threatingestor-1.1.0/threatingestor/extras/__init__.py
+-rw-r--r--   0 azazel     (501) staff       (20)     1227 2023-04-26 13:27:18.000000 threatingestor-1.1.0/threatingestor/extras/fswatcher.py
+-rw-r--r--   0 azazel     (501) staff       (20)     1116 2023-04-26 13:27:18.000000 threatingestor-1.1.0/threatingestor/extras/pasteprocessor.py
+-rw-r--r--   0 azazel     (501) staff       (20)     4918 2023-04-26 13:27:18.000000 threatingestor-1.1.0/threatingestor/extras/queueworker.py
+-rw-r--r--   0 azazel     (501) staff       (20)     2899 2023-04-26 13:27:18.000000 threatingestor-1.1.0/threatingestor/extras/webapp.py
+drwxr-xr-x   0 azazel     (501) staff       (20)        0 2023-04-26 13:27:30.769111 threatingestor-1.1.0/threatingestor/operators/
+-rw-r--r--   0 azazel     (501) staff       (20)     2846 2023-04-26 13:27:18.000000 threatingestor-1.1.0/threatingestor/operators/__init__.py
+-rw-r--r--   0 azazel     (501) staff       (20)      929 2023-04-26 13:26:17.000000 threatingestor-1.1.0/threatingestor/operators/abstract_json.py
+-rw-r--r--   0 azazel     (501) staff       (20)     1129 2023-04-26 13:27:18.000000 threatingestor-1.1.0/threatingestor/operators/beanstalk.py
+-rw-r--r--   0 azazel     (501) staff       (20)     1076 2023-04-26 13:27:18.000000 threatingestor-1.1.0/threatingestor/operators/csv.py
+-rw-r--r--   0 azazel     (501) staff       (20)     4881 2023-04-26 13:27:18.000000 threatingestor-1.1.0/threatingestor/operators/misp.py
+-rw-r--r--   0 azazel     (501) staff       (20)     3584 2023-04-26 13:27:18.000000 threatingestor-1.1.0/threatingestor/operators/mysql.py
+-rw-r--r--   0 azazel     (501) staff       (20)     2296 2023-04-26 13:27:18.000000 threatingestor-1.1.0/threatingestor/operators/sqlite.py
+-rw-r--r--   0 azazel     (501) staff       (20)     1390 2023-04-26 13:27:18.000000 threatingestor-1.1.0/threatingestor/operators/sqs.py
+-rw-r--r--   0 azazel     (501) staff       (20)     3278 2023-04-26 13:27:18.000000 threatingestor-1.1.0/threatingestor/operators/threatkb.py
+-rw-r--r--   0 azazel     (501) staff       (20)     2078 2023-04-26 13:27:18.000000 threatingestor-1.1.0/threatingestor/operators/twitter.py
+drwxr-xr-x   0 azazel     (501) staff       (20)        0 2023-04-26 13:27:30.770532 threatingestor-1.1.0/threatingestor/sources/
+-rw-r--r--   0 azazel     (501) staff       (20)     6931 2023-04-26 13:27:18.000000 threatingestor-1.1.0/threatingestor/sources/__init__.py
+-rw-r--r--   0 azazel     (501) staff       (20)     1654 2023-04-26 13:27:18.000000 threatingestor-1.1.0/threatingestor/sources/abstract_json.py
+-rw-r--r--   0 azazel     (501) staff       (20)     1303 2023-04-26 13:27:18.000000 threatingestor-1.1.0/threatingestor/sources/beanstalk.py
+-rw-r--r--   0 azazel     (501) staff       (20)     3646 2023-04-26 13:27:18.000000 threatingestor-1.1.0/threatingestor/sources/git.py
+-rw-r--r--   0 azazel     (501) staff       (20)     2235 2023-04-26 13:26:17.000000 threatingestor-1.1.0/threatingestor/sources/github.py
+-rw-r--r--   0 azazel     (501) staff       (20)     1634 2023-04-26 13:26:17.000000 threatingestor-1.1.0/threatingestor/sources/github_gist.py
+-rw-r--r--   0 azazel     (501) staff       (20)     2775 2023-04-26 13:27:18.000000 threatingestor-1.1.0/threatingestor/sources/image.py
+-rw-r--r--   0 azazel     (501) staff       (20)     3822 2023-04-26 13:27:18.000000 threatingestor-1.1.0/threatingestor/sources/rss.py
+-rw-r--r--   0 azazel     (501) staff       (20)     3909 2023-04-26 13:27:18.000000 threatingestor-1.1.0/threatingestor/sources/sitemap.py
+-rw-r--r--   0 azazel     (501) staff       (20)     1133 2023-04-26 13:27:18.000000 threatingestor-1.1.0/threatingestor/sources/sqs.py
+-rw-r--r--   0 azazel     (501) staff       (20)     6447 2023-04-26 13:27:18.000000 threatingestor-1.1.0/threatingestor/sources/twitter.py
+-rw-r--r--   0 azazel     (501) staff       (20)     4249 2023-04-26 13:27:18.000000 threatingestor-1.1.0/threatingestor/sources/twitter_follow_links.py
+-rw-r--r--   0 azazel     (501) staff       (20)     1442 2023-04-26 13:27:18.000000 threatingestor-1.1.0/threatingestor/sources/web.py
+-rw-r--r--   0 azazel     (501) staff       (20)     1252 2023-04-26 13:27:18.000000 threatingestor-1.1.0/threatingestor/state.py
+-rw-r--r--   0 azazel     (501) staff       (20)      848 2023-04-26 13:27:18.000000 threatingestor-1.1.0/threatingestor/whitelist.py
+drwxr-xr-x   0 azazel     (501) staff       (20)        0 2023-04-26 13:27:30.767320 threatingestor-1.1.0/threatingestor.egg-info/
+-rw-r--r--   0 azazel     (501) staff       (20)     8311 2023-04-26 13:27:30.000000 threatingestor-1.1.0/threatingestor.egg-info/PKG-INFO
+-rw-r--r--   0 azazel     (501) staff       (20)     2091 2023-04-26 13:27:30.000000 threatingestor-1.1.0/threatingestor.egg-info/SOURCES.txt
+-rw-r--r--   0 azazel     (501) staff       (20)        1 2023-04-26 13:27:30.000000 threatingestor-1.1.0/threatingestor.egg-info/dependency_links.txt
+-rw-r--r--   0 azazel     (501) staff       (20)       55 2023-04-26 13:27:30.000000 threatingestor-1.1.0/threatingestor.egg-info/entry_points.txt
+-rw-r--r--   0 azazel     (501) staff       (20)      503 2023-04-26 13:27:30.000000 threatingestor-1.1.0/threatingestor.egg-info/requires.txt
+-rw-r--r--   0 azazel     (501) staff       (20)       15 2023-04-26 13:27:30.000000 threatingestor-1.1.0/threatingestor.egg-info/top_level.txt
```

### Comparing `threatingestor-1.0.3/LICENSE` & `threatingestor-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `threatingestor-1.0.3/PKG-INFO` & `threatingestor-1.1.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threatingestor
-Version: 1.0.3
+Version: 1.1.0
 Summary: Extract and aggregate IOCs from threat feeds.
 Home-page: https://github.com/InQuest/ThreatIngestor
 Author: InQuest Labs
 Author-email: labs@inquest.net
 License: GPL
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
@@ -12,173 +12,170 @@
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Security
 Classifier: Topic :: Internet
+Description-Content-Type: text/markdown
 Provides-Extra: twitter
 Provides-Extra: rss
 Provides-Extra: misp
 Provides-Extra: threatkb
 Provides-Extra: beanstalk
 Provides-Extra: sqs
 Provides-Extra: mysql
 Provides-Extra: extras
 Provides-Extra: all
 License-File: LICENSE
 
-ThreatIngestor
-==============
+# ThreatIngestor
 
-.. image:: https://inquest.net/images/inquest-badge.svg
-    :target: https://inquest.net/
-    :alt: Developed by InQuest
-.. image:: https://travis-ci.org/InQuest/ThreatIngestor.svg?branch=master
-    :target: https://travis-ci.org/InQuest/ThreatIngestor
-    :alt: Build Status (Travis CI)
-
-.. Change ?branch=develop to ?branch=master when merging into master
-.. image:: https://github.com/InQuest/ThreatIngestor/workflows/threatingestor-workflow/badge.svg?branch=develop
-    :target: https://github.com/InQuest/ThreatIngestor/actions
-    :alt: Build Status (GitHub Workflow)
-
-.. image:: https://readthedocs.org/projects/threatingestor/badge/?version=latest
-    :target: http://inquest.readthedocs.io/projects/threatingestor/en/latest/?badge=latest
-    :alt: Documentation Status
-.. .. image:: https://api.codacy.com/project/badge/Grade/a989bb12e9604d5a9577ce71848e7a2a
-..     :target: https://app.codacy.com/app/InQuest/ThreatIngestor
-..     :alt: Code Health
-.. .. image:: https://api.codacy.com/project/badge/Coverage/a989bb12e9604d5a9577ce71848e7a2a
-..     :target: https://app.codacy.com/app/InQuest/ThreatIngestor
-..     :alt: Test Coverage
-.. image:: http://img.shields.io/pypi/v/ThreatIngestor.svg
-    :target: https://pypi.python.org/pypi/ThreatIngestor
-    :alt: PyPi Version
-
-An extendable tool to extract and aggregate IOCs_ from threat feeds.
-
-Integrates out-of-the-box with ThreatKB_ and MISP_, and can fit seamlessly into any existing workflow with SQS_, Beanstalk_, and `custom plugins`_.
-
-Currently used by InQuest Labs IOC-DB: https://labs.inquest.net/iocdb.
-
-Overview
---------
-
-ThreatIngestor can be configured to watch Twitter, RSS feeds, or other sources, extract meaningful information such as malicious IPs/domains and YARA signatures, and send that information to another system for analysis.
-
-.. image:: https://inquest.readthedocs.io/projects/threatingestor/en/latest/_images/mermaid-multiple-operators.png
-    :target: https://inquest.readthedocs.io/projects/threatingestor/en/latest/workflows.html
-    :alt: ThreatIngestor flowchart with several sources feeding into multiple operators.
+![Build Status](https://github.com/InQuest/ThreatIngestor/workflows/threatingestor-workflow/badge.svg?branch=master)
+![Developed by InQuest](https://inquest.net/images/inquest-badge.svg)
 
-Try it out now with this `quick walkthrough`_, read more `ThreatIngestor walkthroughs`_ on the InQuest blog, and check out `labs.inquest.net/iocdb`_, an IOC aggregation and querying tool powered by ThreatIngestor.
+![Documentation Status](https://readthedocs.org/projects/threatingestor/badge/?version=latest)
+![PyPI Version](http://img.shields.io/pypi/v/ThreatIngestor.svg)
 
-Installation
-------------
+An extendable tool to extract and aggregate [IOCs](https://en.wikipedia.org/wiki/Indicator_of_compromise) from threat feeds.
+
+Integrates out-of-the-box with [ThreatKB](https://github.com/InQuest/ThreatKB) and [MISP](https://www.misp-project.org/), and can fit seamlessly into any existing workflow with [SQS](https://aws.amazon.com/sqs/), [Beanstalk](https://beanstalkd.github.io/), and [custom plugins](https://inquest.readthedocs.io/projects/threatingestor/en/latest/developing.html).
+
+Currently used by InQuest Labs IOC-DB: https://labs.inquest.net/iocdb
+
+## Overview
+
+ThreatIngestor can be configured to watch Twitter, RSS feeds, sitemap (XML) feeds, or other sources, extract meaningful information such as malicious IPs/domains and YARA signatures, and send that information to another system for analysis.
+
+![ThreatIngestor flowchart with several sources feeding into multiple operators](https://inquest.readthedocs.io/projects/threatingestor/en/latest/_images/mermaid-multiple-operators.png)
+
+Try it out now with this [quick walkthrough](https://inquest.readthedocs.io/projects/threatingestor/en/latest/welcome.html#try-it-out), read more [ThreatIngestor walkthroughs](https://inquest.net/taxonomy/term/42) on the InQuest blog, and check out [labs.inquest.net/iocdb](https://labs.inquest.net/iocdb), an IOC aggregation and querying tool powered by ThreatIngestor.
+
+## Installation
 
 ThreatIngestor requires Python 3.6+, with development headers.
 
-Install ThreatIngestor from PyPI::
+Install ThreatIngestor from PyPI:
 
-    pip install threatingestor
+```bash
+pip install threatingestor
+```
 
-Install optional dependencies for using some plugins, as needed::
+Install optional dependencies for using some plugins, as needed:
 
-    pip install threatingestor[all]
+```bash
+pip install threatingestor[all]
+```
 
-View the `full installation instructions`_ for more information.
+View the [full installation instructions](https://inquest.readthedocs.io/projects/threatingestor/en/latest/installation.html) for more information.
 
-Usage
------
+## Usage
 
-Create a new ``config.yml`` file, and configure each source and operator module you want to use. (See ``config.example.yml`` for layout.) Then run the script::
+Create a new ``config.yml`` file, and configure each source and operator module you want to use. (See ``config.example.yml`` for layout.) Then run the script:
 
-    threatingestor config.yml
+```bash
+threatingestor config.yml
+```
 
 By default, it will run forever, polling each configured source every 15 minutes.
 
-View the `full ThreatIngestor documentation`_ for more information.
+If you'd like to run the image extraction source, or include the image extraction functionality for other sources, you will need to be running Python 3.7 >= due to the dependencies:
 
-Plugins
--------
+```bash
+pip install opencv-python pytesseract numpy
+```
+
+View the [full ThreatIngestor documentation](https://inquest.readthedocs.io/projects/threatingestor/) for more information.
+
+## Plugins
 
 ThreatIngestor uses a plugin architecture with "source" (input) and "operator" (output) plugins. The currently supported integrations are:
 
-Sources
-~~~~~~~
+### Sources
 
-* `Beanstalk work queues <https://inquest.readthedocs.io/projects/threatingestor/en/latest/sources/beanstalk.html>`__
-* `Git repositories <https://inquest.readthedocs.io/projects/threatingestor/en/latest/sources/git.html>`__
-* `GitHub repository search <https://inquest.readthedocs.io/projects/threatingestor/en/latest/sources/github.html>`__
-* `Gists by username <https://inquest.readthedocs.io/projects/threatingestor/en/latest/sources/github_gist.html>`__
-* `RSS feeds <https://inquest.readthedocs.io/projects/threatingestor/en/latest/sources/rss.html>`__
-* `Sitemap blogs <https://inquest.readthedocs.io/projects/threatingestor/en/latest/sources/sitemap.html>`__
-* `Image extraction <https://inquest.readthedocs.io/projects/threatingestor/en/latest/sources/image.html>`__
-* `Amazon SQS queues <https://inquest.readthedocs.io/projects/threatingestor/en/latest/sources/sqs.html>`__
-* `Twitter <https://inquest.readthedocs.io/projects/threatingestor/en/latest/sources/twitter.html>`__
-* `Generic web pages <https://inquest.readthedocs.io/projects/threatingestor/en/latest/sources/web.html>`__
-
-Operators
-~~~~~~~~~
-
-* `Beanstalk work queues <https://inquest.readthedocs.io/projects/threatingestor/en/latest/operators/beanstalk.html>`__
-* `CSV files <https://inquest.readthedocs.io/projects/threatingestor/en/latest/operators/csv.html>`__
-* `MISP <https://inquest.readthedocs.io/projects/threatingestor/en/latest/operators/misp.html>`__
-* `MySQL table <https://inquest.readthedocs.io/projects/threatingestor/en/latest/operators/mysql.html>`__
-* `SQLite database <https://inquest.readthedocs.io/projects/threatingestor/en/latest/operators/sqlite.html>`__
-* `Amazon SQS queues <https://inquest.readthedocs.io/projects/threatingestor/en/latest/operators/sqs.html>`__
-* `ThreatKB <https://inquest.readthedocs.io/projects/threatingestor/en/latest/operators/threatkb.html>`__
-* `Twitter <https://inquest.readthedocs.io/projects/threatingestor/en/latest/operators/twitter.html>`__
+- [Git repositories](https://inquest.readthedocs.io/projects/threatingestor/en/latest/sources/git.html)
+- [GitHub repository search](https://inquest.readthedocs.io/projects/threatingestor/en/latest/sources/github.html)
+- [Gists by username](https://inquest.readthedocs.io/projects/threatingestor/en/latest/sources/github_gist.html)
+- [RSS feeds](https://inquest.readthedocs.io/projects/threatingestor/en/latest/sources/rss.html)
+- [Sitemap feeds](https://inquest.readthedocs.io/projects/threatingestor/en/latest/sources/sitemap.html)
+- [Image extraction](https://inquest.readthedocs.io/projects/threatingestor/en/latest/sources/image.html)
+- [Amazon SQS queues](https://inquest.readthedocs.io/projects/threatingestor/en/latest/sources/sqs.html)
+- [Twitter](https://inquest.readthedocs.io/projects/threatingestor/en/latest/sources/twitter.html)
+- [Generic web pages](https://inquest.readthedocs.io/projects/threatingestor/en/latest/sources/web.html)
+
+### Operators
+
+- [CSV files](https://inquest.readthedocs.io/projects/threatingestor/en/latest/operators/csv.html)
+- [MISP](https://inquest.readthedocs.io/projects/threatingestor/en/latest/operators/misp.html)
+- [MySQL table](https://inquest.readthedocs.io/projects/threatingestor/en/latest/operators/mysql.html)
+- [SQLite database](https://inquest.readthedocs.io/projects/threatingestor/en/latest/operators/sqlite.html)
+- [Amazon SQS queues](https://inquest.readthedocs.io/projects/threatingestor/en/latest/operators/sqs.html)
+- [ThreatKB](https://inquest.readthedocs.io/projects/threatingestor/en/latest/operators/threatkb.html)
+- [Twitter](https://inquest.readthedocs.io/projects/threatingestor/en/latest/operators/twitter.html)
 
-View the `full ThreatIngestor documentation`_ for more information on included plugins, and how to create your own.
+View the [full ThreatIngestor documentation](https://inquest.readthedocs.io/projects/threatingestor/) for more information on included plugins, and how to create your own.
 
-Threat Intel Sources
---------------------
+## Threat Intel Sources
 
 Looking for some threat intel sources to get started? InQuest has a Twitter List with several accounts that post C2 domains and IPs: https://twitter.com/InQuest/lists/ioc-feed. Note that you will need to apply for a Twitter developer account to use the ThreatIngestor Twitter Source. Take a look at ``config.example.yml`` to see how to set this list up as a source.
 
-For quicker setup, RSS feeds can be a great source of intelligence. Check out this example `RSS config file`_ for a few pre-configured security blogs.
+For quicker setup, RSS feeds can be a great source of intelligence. Check out this example [RSS config file](https://github.com/InQuest/ThreatIngestor/blob/master/rss.example.yml) for a few pre-configured security blogs.
 
-Support
--------
+## Support
 
-If you need help getting set up, or run into any issues, feel free to open an Issue_. You can also reach out to `@InQuest`_ on Twitter or read more about us on the web at https://www.inquest.net.
+If you need help getting set up, or run into any issues, feel free to open an [issue](https://github.com/InQuest/ThreatIngestor/issues). You can also reach out to [@InQuest](https://twitter.com/InQuest) on Twitter or read more about us on the web at https://www.inquest.net.
 
 We'd love to hear any feedback you have on ThreatIngestor, its documentation, or how you're putting it to work for you!
 
-Contributing
-------------
+## Contributing
+
+Issues and pull requests are welcomed. Please keep Python code PEP8 compliant. By submitting a pull request you agree to release your submissions under the terms of the [LICENSE](https://github.com/InQuest/ThreatIngestor/blob/master/LICENSE).
+
+## Docker
+
+
+### Production
+
+A `Dockerfile` is available for running ThreatIngestor within a Docker container.
+
+First, you'll need to build the container:
+
+```bash
+docker build . -t threatingestor
+```
+
+After that, you can mount the container by using this command:
+
+```bash
+docker run -it --mount type=bind,source=/,target=/dock threatingestor /bin/bash
+```
+
+After you've mounted the container and you're inside the `/bin/bash` shell, you can run ThreatIngestor like normal:
+
+```bash
+threatingestor config.yml
+```
+
+### Development
+
+There is also a Dockerfile.dev for building a development version of ThreatIngestor. All you need is an available .whl file, which can be generated with the following command:
+
+```bash
+python3 -m build 
+```
+
+After you've built the project, you can build the container:
+
+```bash
+docker build . -t threatingestor -f Dockerfile.dev
+```
 
-Issues and pull requests are welcomed. Please keep Python code PEP8 compliant. By submitting a pull request you agree to release your submissions under the terms of the LICENSE_.
+NOTE: If you run into any issues while building the development environment or running ThreatIngestor within the container, you may need to comment out the following lines in `Dockerfile.dev` to work properly:
 
-.. _ThreatKB: https://github.com/InQuest/ThreatKB
-.. _LICENSE: https://github.com/InQuest/threat-ingestors/blob/master/LICENSE
-.. _full ThreatIngestor Documentation: https://inquest.readthedocs.io/projects/threatingestor/
-.. _SQS: https://aws.amazon.com/sqs/
-.. _Beanstalk: https://beanstalkd.github.io/
-.. _MISP: https://www.misp-project.org/
-.. _custom plugins: https://inquest.readthedocs.io/projects/threatingestor/en/latest/developing.html
-.. _IOCs: https://en.wikipedia.org/wiki/Indicator_of_compromise
-.. _full installation instructions: https://inquest.readthedocs.io/projects/threatingestor/en/latest/installation.html
-.. _Issue: https://github.com/InQuest/ThreatIngestor/issues
-.. _@InQuest: https://twitter.com/InQuest
-.. _quick walkthrough: https://inquest.readthedocs.io/projects/threatingestor/en/latest/welcome.html#try-it-out
-.. _ThreatIngestor walkthroughs: https://inquest.net/taxonomy/term/42
-.. _RSS config file: https://github.com/InQuest/ThreatIngestor/blob/master/rss.example.yml
-.. _labs.inquest.net/iocdb: https://labs.inquest.net/iocdb
-
-Docker Container
-----------------
-
-A Dockerfile is now available for running ThreatIngestor within a Docker container.
-
-First, you'll need to build the container::
-
-    docker build . -t threat
-
-After that, you can mount the container for use using this command::
-
-    docker run -it --mount type=bind,source=/,target=/dock threat /bin/bash
-
-After you've mounted the container, and you're inside of the `/bin/bash` shell, you can run the threatingestor like normal::
-    
-    threatingestor config.yml
+```
+FROM ubuntu:18.04
+...
+# RUN apt-get install tesseract-ocr -y
+...
+# RUN pip3 install opencv-python pytesseract numpy
+...
+```
```

### Comparing `threatingestor-1.0.3/README.rst` & `threatingestor-1.1.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,155 +1,151 @@
-ThreatIngestor
-==============
+# ThreatIngestor
 
-.. image:: https://inquest.net/images/inquest-badge.svg
-    :target: https://inquest.net/
-    :alt: Developed by InQuest
-.. image:: https://travis-ci.org/InQuest/ThreatIngestor.svg?branch=master
-    :target: https://travis-ci.org/InQuest/ThreatIngestor
-    :alt: Build Status (Travis CI)
-
-.. Change ?branch=develop to ?branch=master when merging into master
-.. image:: https://github.com/InQuest/ThreatIngestor/workflows/threatingestor-workflow/badge.svg?branch=develop
-    :target: https://github.com/InQuest/ThreatIngestor/actions
-    :alt: Build Status (GitHub Workflow)
-
-.. image:: https://readthedocs.org/projects/threatingestor/badge/?version=latest
-    :target: http://inquest.readthedocs.io/projects/threatingestor/en/latest/?badge=latest
-    :alt: Documentation Status
-.. .. image:: https://api.codacy.com/project/badge/Grade/a989bb12e9604d5a9577ce71848e7a2a
-..     :target: https://app.codacy.com/app/InQuest/ThreatIngestor
-..     :alt: Code Health
-.. .. image:: https://api.codacy.com/project/badge/Coverage/a989bb12e9604d5a9577ce71848e7a2a
-..     :target: https://app.codacy.com/app/InQuest/ThreatIngestor
-..     :alt: Test Coverage
-.. image:: http://img.shields.io/pypi/v/ThreatIngestor.svg
-    :target: https://pypi.python.org/pypi/ThreatIngestor
-    :alt: PyPi Version
-
-An extendable tool to extract and aggregate IOCs_ from threat feeds.
-
-Integrates out-of-the-box with ThreatKB_ and MISP_, and can fit seamlessly into any existing workflow with SQS_, Beanstalk_, and `custom plugins`_.
-
-Currently used by InQuest Labs IOC-DB: https://labs.inquest.net/iocdb.
-
-Overview
---------
-
-ThreatIngestor can be configured to watch Twitter, RSS feeds, or other sources, extract meaningful information such as malicious IPs/domains and YARA signatures, and send that information to another system for analysis.
-
-.. image:: https://inquest.readthedocs.io/projects/threatingestor/en/latest/_images/mermaid-multiple-operators.png
-    :target: https://inquest.readthedocs.io/projects/threatingestor/en/latest/workflows.html
-    :alt: ThreatIngestor flowchart with several sources feeding into multiple operators.
+![Build Status](https://github.com/InQuest/ThreatIngestor/workflows/threatingestor-workflow/badge.svg?branch=master)
+![Developed by InQuest](https://inquest.net/images/inquest-badge.svg)
 
-Try it out now with this `quick walkthrough`_, read more `ThreatIngestor walkthroughs`_ on the InQuest blog, and check out `labs.inquest.net/iocdb`_, an IOC aggregation and querying tool powered by ThreatIngestor.
+![Documentation Status](https://readthedocs.org/projects/threatingestor/badge/?version=latest)
+![PyPI Version](http://img.shields.io/pypi/v/ThreatIngestor.svg)
 
-Installation
-------------
+An extendable tool to extract and aggregate [IOCs](https://en.wikipedia.org/wiki/Indicator_of_compromise) from threat feeds.
+
+Integrates out-of-the-box with [ThreatKB](https://github.com/InQuest/ThreatKB) and [MISP](https://www.misp-project.org/), and can fit seamlessly into any existing workflow with [SQS](https://aws.amazon.com/sqs/), [Beanstalk](https://beanstalkd.github.io/), and [custom plugins](https://inquest.readthedocs.io/projects/threatingestor/en/latest/developing.html).
+
+Currently used by InQuest Labs IOC-DB: https://labs.inquest.net/iocdb
+
+## Overview
+
+ThreatIngestor can be configured to watch Twitter, RSS feeds, sitemap (XML) feeds, or other sources, extract meaningful information such as malicious IPs/domains and YARA signatures, and send that information to another system for analysis.
+
+![ThreatIngestor flowchart with several sources feeding into multiple operators](https://inquest.readthedocs.io/projects/threatingestor/en/latest/_images/mermaid-multiple-operators.png)
+
+Try it out now with this [quick walkthrough](https://inquest.readthedocs.io/projects/threatingestor/en/latest/welcome.html#try-it-out), read more [ThreatIngestor walkthroughs](https://inquest.net/taxonomy/term/42) on the InQuest blog, and check out [labs.inquest.net/iocdb](https://labs.inquest.net/iocdb), an IOC aggregation and querying tool powered by ThreatIngestor.
+
+## Installation
 
 ThreatIngestor requires Python 3.6+, with development headers.
 
-Install ThreatIngestor from PyPI::
+Install ThreatIngestor from PyPI:
 
-    pip install threatingestor
+```bash
+pip install threatingestor
+```
 
-Install optional dependencies for using some plugins, as needed::
+Install optional dependencies for using some plugins, as needed:
 
-    pip install threatingestor[all]
+```bash
+pip install threatingestor[all]
+```
 
-View the `full installation instructions`_ for more information.
+View the [full installation instructions](https://inquest.readthedocs.io/projects/threatingestor/en/latest/installation.html) for more information.
 
-Usage
------
+## Usage
 
-Create a new ``config.yml`` file, and configure each source and operator module you want to use. (See ``config.example.yml`` for layout.) Then run the script::
+Create a new ``config.yml`` file, and configure each source and operator module you want to use. (See ``config.example.yml`` for layout.) Then run the script:
 
-    threatingestor config.yml
+```bash
+threatingestor config.yml
+```
 
 By default, it will run forever, polling each configured source every 15 minutes.
 
-View the `full ThreatIngestor documentation`_ for more information.
+If you'd like to run the image extraction source, or include the image extraction functionality for other sources, you will need to be running Python 3.7 >= due to the dependencies:
 
-Plugins
--------
+```bash
+pip install opencv-python pytesseract numpy
+```
+
+View the [full ThreatIngestor documentation](https://inquest.readthedocs.io/projects/threatingestor/) for more information.
+
+## Plugins
 
 ThreatIngestor uses a plugin architecture with "source" (input) and "operator" (output) plugins. The currently supported integrations are:
 
-Sources
-~~~~~~~
+### Sources
 
-* `Beanstalk work queues <https://inquest.readthedocs.io/projects/threatingestor/en/latest/sources/beanstalk.html>`__
-* `Git repositories <https://inquest.readthedocs.io/projects/threatingestor/en/latest/sources/git.html>`__
-* `GitHub repository search <https://inquest.readthedocs.io/projects/threatingestor/en/latest/sources/github.html>`__
-* `Gists by username <https://inquest.readthedocs.io/projects/threatingestor/en/latest/sources/github_gist.html>`__
-* `RSS feeds <https://inquest.readthedocs.io/projects/threatingestor/en/latest/sources/rss.html>`__
-* `Sitemap blogs <https://inquest.readthedocs.io/projects/threatingestor/en/latest/sources/sitemap.html>`__
-* `Image extraction <https://inquest.readthedocs.io/projects/threatingestor/en/latest/sources/image.html>`__
-* `Amazon SQS queues <https://inquest.readthedocs.io/projects/threatingestor/en/latest/sources/sqs.html>`__
-* `Twitter <https://inquest.readthedocs.io/projects/threatingestor/en/latest/sources/twitter.html>`__
-* `Generic web pages <https://inquest.readthedocs.io/projects/threatingestor/en/latest/sources/web.html>`__
-
-Operators
-~~~~~~~~~
-
-* `Beanstalk work queues <https://inquest.readthedocs.io/projects/threatingestor/en/latest/operators/beanstalk.html>`__
-* `CSV files <https://inquest.readthedocs.io/projects/threatingestor/en/latest/operators/csv.html>`__
-* `MISP <https://inquest.readthedocs.io/projects/threatingestor/en/latest/operators/misp.html>`__
-* `MySQL table <https://inquest.readthedocs.io/projects/threatingestor/en/latest/operators/mysql.html>`__
-* `SQLite database <https://inquest.readthedocs.io/projects/threatingestor/en/latest/operators/sqlite.html>`__
-* `Amazon SQS queues <https://inquest.readthedocs.io/projects/threatingestor/en/latest/operators/sqs.html>`__
-* `ThreatKB <https://inquest.readthedocs.io/projects/threatingestor/en/latest/operators/threatkb.html>`__
-* `Twitter <https://inquest.readthedocs.io/projects/threatingestor/en/latest/operators/twitter.html>`__
+- [Git repositories](https://inquest.readthedocs.io/projects/threatingestor/en/latest/sources/git.html)
+- [GitHub repository search](https://inquest.readthedocs.io/projects/threatingestor/en/latest/sources/github.html)
+- [Gists by username](https://inquest.readthedocs.io/projects/threatingestor/en/latest/sources/github_gist.html)
+- [RSS feeds](https://inquest.readthedocs.io/projects/threatingestor/en/latest/sources/rss.html)
+- [Sitemap feeds](https://inquest.readthedocs.io/projects/threatingestor/en/latest/sources/sitemap.html)
+- [Image extraction](https://inquest.readthedocs.io/projects/threatingestor/en/latest/sources/image.html)
+- [Amazon SQS queues](https://inquest.readthedocs.io/projects/threatingestor/en/latest/sources/sqs.html)
+- [Twitter](https://inquest.readthedocs.io/projects/threatingestor/en/latest/sources/twitter.html)
+- [Generic web pages](https://inquest.readthedocs.io/projects/threatingestor/en/latest/sources/web.html)
+
+### Operators
+
+- [CSV files](https://inquest.readthedocs.io/projects/threatingestor/en/latest/operators/csv.html)
+- [MISP](https://inquest.readthedocs.io/projects/threatingestor/en/latest/operators/misp.html)
+- [MySQL table](https://inquest.readthedocs.io/projects/threatingestor/en/latest/operators/mysql.html)
+- [SQLite database](https://inquest.readthedocs.io/projects/threatingestor/en/latest/operators/sqlite.html)
+- [Amazon SQS queues](https://inquest.readthedocs.io/projects/threatingestor/en/latest/operators/sqs.html)
+- [ThreatKB](https://inquest.readthedocs.io/projects/threatingestor/en/latest/operators/threatkb.html)
+- [Twitter](https://inquest.readthedocs.io/projects/threatingestor/en/latest/operators/twitter.html)
 
-View the `full ThreatIngestor documentation`_ for more information on included plugins, and how to create your own.
+View the [full ThreatIngestor documentation](https://inquest.readthedocs.io/projects/threatingestor/) for more information on included plugins, and how to create your own.
 
-Threat Intel Sources
---------------------
+## Threat Intel Sources
 
 Looking for some threat intel sources to get started? InQuest has a Twitter List with several accounts that post C2 domains and IPs: https://twitter.com/InQuest/lists/ioc-feed. Note that you will need to apply for a Twitter developer account to use the ThreatIngestor Twitter Source. Take a look at ``config.example.yml`` to see how to set this list up as a source.
 
-For quicker setup, RSS feeds can be a great source of intelligence. Check out this example `RSS config file`_ for a few pre-configured security blogs.
+For quicker setup, RSS feeds can be a great source of intelligence. Check out this example [RSS config file](https://github.com/InQuest/ThreatIngestor/blob/master/rss.example.yml) for a few pre-configured security blogs.
 
-Support
--------
+## Support
 
-If you need help getting set up, or run into any issues, feel free to open an Issue_. You can also reach out to `@InQuest`_ on Twitter or read more about us on the web at https://www.inquest.net.
+If you need help getting set up, or run into any issues, feel free to open an [issue](https://github.com/InQuest/ThreatIngestor/issues). You can also reach out to [@InQuest](https://twitter.com/InQuest) on Twitter or read more about us on the web at https://www.inquest.net.
 
 We'd love to hear any feedback you have on ThreatIngestor, its documentation, or how you're putting it to work for you!
 
-Contributing
-------------
+## Contributing
+
+Issues and pull requests are welcomed. Please keep Python code PEP8 compliant. By submitting a pull request you agree to release your submissions under the terms of the [LICENSE](https://github.com/InQuest/ThreatIngestor/blob/master/LICENSE).
+
+## Docker
+
+
+### Production
+
+A `Dockerfile` is available for running ThreatIngestor within a Docker container.
+
+First, you'll need to build the container:
+
+```bash
+docker build . -t threatingestor
+```
+
+After that, you can mount the container by using this command:
+
+```bash
+docker run -it --mount type=bind,source=/,target=/dock threatingestor /bin/bash
+```
+
+After you've mounted the container and you're inside the `/bin/bash` shell, you can run ThreatIngestor like normal:
+
+```bash
+threatingestor config.yml
+```
+
+### Development
+
+There is also a Dockerfile.dev for building a development version of ThreatIngestor. All you need is an available .whl file, which can be generated with the following command:
+
+```bash
+python3 -m build 
+```
+
+After you've built the project, you can build the container:
+
+```bash
+docker build . -t threatingestor -f Dockerfile.dev
+```
 
-Issues and pull requests are welcomed. Please keep Python code PEP8 compliant. By submitting a pull request you agree to release your submissions under the terms of the LICENSE_.
+NOTE: If you run into any issues while building the development environment or running ThreatIngestor within the container, you may need to comment out the following lines in `Dockerfile.dev` to work properly:
 
-.. _ThreatKB: https://github.com/InQuest/ThreatKB
-.. _LICENSE: https://github.com/InQuest/threat-ingestors/blob/master/LICENSE
-.. _full ThreatIngestor Documentation: https://inquest.readthedocs.io/projects/threatingestor/
-.. _SQS: https://aws.amazon.com/sqs/
-.. _Beanstalk: https://beanstalkd.github.io/
-.. _MISP: https://www.misp-project.org/
-.. _custom plugins: https://inquest.readthedocs.io/projects/threatingestor/en/latest/developing.html
-.. _IOCs: https://en.wikipedia.org/wiki/Indicator_of_compromise
-.. _full installation instructions: https://inquest.readthedocs.io/projects/threatingestor/en/latest/installation.html
-.. _Issue: https://github.com/InQuest/ThreatIngestor/issues
-.. _@InQuest: https://twitter.com/InQuest
-.. _quick walkthrough: https://inquest.readthedocs.io/projects/threatingestor/en/latest/welcome.html#try-it-out
-.. _ThreatIngestor walkthroughs: https://inquest.net/taxonomy/term/42
-.. _RSS config file: https://github.com/InQuest/ThreatIngestor/blob/master/rss.example.yml
-.. _labs.inquest.net/iocdb: https://labs.inquest.net/iocdb
-
-Docker Container
-----------------
-
-A Dockerfile is now available for running ThreatIngestor within a Docker container.
-
-First, you'll need to build the container::
-
-    docker build . -t threat
-
-After that, you can mount the container for use using this command::
-
-    docker run -it --mount type=bind,source=/,target=/dock threat /bin/bash
-
-After you've mounted the container, and you're inside of the `/bin/bash` shell, you can run the threatingestor like normal::
-    
-    threatingestor config.yml
+```
+FROM ubuntu:18.04
+...
+# RUN apt-get install tesseract-ocr -y
+...
+# RUN pip3 install opencv-python pytesseract numpy
+...
+```
```

### Comparing `threatingestor-1.0.3/setup.py` & `threatingestor-1.1.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 from setuptools import setup, find_packages
 
-README = open(os.path.join(os.path.dirname(__file__), 'README.rst')).read()
+with open("README.md", "r") as fh:
+    README = fh.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 requirements = open(os.path.join(os.path.dirname(__file__),
             'requirements.txt')).read()
 requires = requirements.strip().split('\n')
@@ -16,15 +17,15 @@
 if not isinstance(extra_requires, list):
     print("requirements-testing.txt was not parsed correctly.")
     extra_requires = []
 
 
 setup(
     name='threatingestor',
-    version='1.0.3',
+    version='1.1.0',
     include_package_data=True,
     install_requires=requires,
     extras_require={
         'twitter': ['twitter'],
         'rss': ['feedparser'],
         'misp': ['PyMISP'],
         'threatkb': ['threatkb'],
@@ -38,14 +39,15 @@
           'console_scripts': [
               'threatingestor = threatingestor:main'
           ]
     },
     license='GPL',
     description='Extract and aggregate IOCs from threat feeds.',
     long_description=README,
+    long_description_content_type='text/markdown',
     url='https://github.com/InQuest/ThreatIngestor',
     author='InQuest Labs',
     author_email='labs@inquest.net',
     packages=find_packages(),
     classifiers=[
         'Intended Audience :: Developers',
         'Intended Audience :: Information Technology',
```

### Comparing `threatingestor-1.0.3/tests/test_artifacts.py` & `threatingestor-1.1.0/tests/test_artifacts.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         self.assertFalse(threatingestor.artifacts.URL('tcp://[fdc4:2581:575b:5a72:0000:0000:0000:0001]:80/path', '').is_ipv4())
         self.assertFalse(threatingestor.artifacts.URL('http://example.com:80/path', '').is_ipv4())
 
     def test_url_ipv6(self):
         self.assertTrue(threatingestor.artifacts.URL('http://fdc4:2581:575b:5a72:0000:0000:0000:0001', '').is_ipv6())
         self.assertTrue(threatingestor.artifacts.URL('http://[fdc4:2581:575b:5a72:0000:0000:0000:0001]:80/path', '').is_ipv6())
         self.assertTrue(threatingestor.artifacts.URL('[fdc4:2581:575b:5a72:0000:0000:0000:0001]:80/path', '').is_ipv6())
-        # self.assertTrue(threatingestor.artifacts.URL('fdc4:2581:575b:5a72:0000:0000:0000:0001', '').is_ipv6())
+        self.assertFalse(threatingestor.artifacts.URL('fdc4:2581:575b:5a72:0000:0000:0000:0001', '').is_ipv6())
         self.assertTrue(threatingestor.artifacts.URL('tcp://[fdc4:2581:575b:5a72:0000:0000:0000:0001]:80/path', '').is_ipv6())
         self.assertFalse(threatingestor.artifacts.URL('tcp://192[.]168[.]0[.]1:80/path', '').is_ipv6())
         self.assertFalse(threatingestor.artifacts.URL('http://example.com:80/path', '').is_ipv6())
 
     def test_url_deobfuscation(self):
         self.assertEqual(threatingestor.artifacts.URL('http://example.com/', '').deobfuscated(), 'http://example.com/')
         self.assertEqual(threatingestor.artifacts.URL('http://example[.]com/', '').deobfuscated(), 'http://example.com/')
```

### Comparing `threatingestor-1.0.3/tests/test_config.py` & `threatingestor-1.1.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `threatingestor-1.0.3/tests/test_ingestor.py` & `threatingestor-1.1.0/tests/test_ingestor.py`

 * *Files identical despite different names*

### Comparing `threatingestor-1.0.3/tests/test_operators.py` & `threatingestor-1.1.0/tests/test_operators.py`

 * *Files identical despite different names*

### Comparing `threatingestor-1.0.3/tests/test_operators_abstract_json.py` & `threatingestor-1.1.0/tests/test_operators_abstract_json.py`

 * *Files identical despite different names*

### Comparing `threatingestor-1.0.3/tests/test_operators_beanstalk.py` & `threatingestor-1.1.0/tests/test_operators_beanstalk.py`

 * *Files identical despite different names*

### Comparing `threatingestor-1.0.3/tests/test_operators_csv.py` & `threatingestor-1.1.0/tests/test_operators_csv.py`

 * *Files identical despite different names*

### Comparing `threatingestor-1.0.3/tests/test_operators_misp.py` & `threatingestor-1.1.0/tests/test_operators_misp.py`

 * *Files identical despite different names*

### Comparing `threatingestor-1.0.3/tests/test_operators_mysql.py` & `threatingestor-1.1.0/tests/test_operators_mysql.py`

 * *Files identical despite different names*

### Comparing `threatingestor-1.0.3/tests/test_operators_sqlite.py` & `threatingestor-1.1.0/tests/test_operators_sqlite.py`

 * *Files identical despite different names*

### Comparing `threatingestor-1.0.3/tests/test_operators_sqs.py` & `threatingestor-1.1.0/tests/test_operators_sqs.py`

 * *Files identical despite different names*

### Comparing `threatingestor-1.0.3/tests/test_operators_threatkb.py` & `threatingestor-1.1.0/tests/test_operators_threatkb.py`

 * *Files identical despite different names*

### Comparing `threatingestor-1.0.3/tests/test_operators_twitter.py` & `threatingestor-1.1.0/tests/test_operators_twitter.py`

 * *Files identical despite different names*

### Comparing `threatingestor-1.0.3/tests/test_sources.py` & `threatingestor-1.1.0/tests/test_sources.py`

 * *Files identical despite different names*

### Comparing `threatingestor-1.0.3/tests/test_sources_beanstalk.py` & `threatingestor-1.1.0/tests/test_sources_beanstalk.py`

 * *Files identical despite different names*

### Comparing `threatingestor-1.0.3/tests/test_sources_git.py` & `threatingestor-1.1.0/tests/test_sources_git.py`

 * *Files identical despite different names*

### Comparing `threatingestor-1.0.3/tests/test_sources_github.py` & `threatingestor-1.1.0/tests/test_sources_github.py`

 * *Files identical despite different names*

### Comparing `threatingestor-1.0.3/tests/test_sources_json.py` & `threatingestor-1.1.0/tests/test_sources_json.py`

 * *Files identical despite different names*

### Comparing `threatingestor-1.0.3/tests/test_sources_sqs.py` & `threatingestor-1.1.0/tests/test_sources_sqs.py`

 * *Files identical despite different names*

### Comparing `threatingestor-1.0.3/tests/test_sources_twitter.py` & `threatingestor-1.1.0/tests/test_sources_twitter.py`

 * *Files identical despite different names*

### Comparing `threatingestor-1.0.3/tests/test_sources_web.py` & `threatingestor-1.1.0/tests/test_sources_web.py`

 * *Files identical despite different names*

### Comparing `threatingestor-1.0.3/tests/test_state.py` & `threatingestor-1.1.0/tests/test_state.py`

 * *Files identical despite different names*

### Comparing `threatingestor-1.0.3/threatingestor/__init__.py` & `threatingestor-1.1.0/threatingestor/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 import sys
 import time
 import collections
 
 from loguru import logger
 import statsd
+
 try:
     import notifiers
     from notifiers.logging import NotificationHandler
 except ImportError:
     logger.info("Notifiers is not installed.")
     notifiers = None
 
-
 import threatingestor.config
 import threatingestor.state
 import threatingestor.exceptions
 import threatingestor.whitelist
 
-
 class Ingestor:
     """ThreatIngestor main work logic.
 
     Handles reading the config file, calling sources, maintaining state, and
     sending artifacts to operators.
     """
     def __init__(self, config_file):
```

### Comparing `threatingestor-1.0.3/threatingestor/artifacts.py` & `threatingestor-1.1.0/threatingestor/artifacts.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import re
 import ipaddress
-from urllib.parse import urlparse
-
-
 import iocextract
 
+from urllib.parse import urlparse
 
 class Artifact(object):
     """Artifact base class."""
     def __init__(self, artifact, source_name, reference_link=None, reference_text=None):
         self.artifact = artifact
         self.source_name = source_name
         self.reference_link = reference_link or ''
@@ -114,48 +112,48 @@
         * {url}
         * {defanged}
         * {domain}
         * All supported variables from Artifact.format_message
         """
         return super(URL, self).format_message(message, url=str(self),
                                                domain=self.domain(),
-                                               defanged=iocextract.defang(str(self)))
+                                               defanged=iocextract.defang_data(str(self)))
 
 
     def _stringify(self):
         """Always returns deobfuscated URL."""
-        return iocextract.refang_url(self.artifact)
+        return iocextract.refang_data(self.artifact)
 
 
     def is_obfuscated(self):
         """Boolean: is an obfuscated URL?"""
         stringlike = self._stringify()
         if stringlike != self.artifact:
             # don't treat "example.com" as obfuscated
             if stringlike != 'http://' + self.artifact:
                 return True
         return False
 
 
     def is_ipv4(self):
         """Boolean: URL network location is an IPv4 address, not a domain?"""
-        parsed = urlparse(iocextract.refang_url(self.artifact))
+        parsed = urlparse(iocextract.refang_data(self.artifact))
 
         try:
             ipaddress.IPv4Address(parsed.netloc.split(':')[0].replace('[', '').replace(']', '').replace(',', '.'))
         except ValueError:
             return False
 
         return True
 
 
     def is_ipv6(self):
         """Boolean: URL network location is an IPv6 address, not a domain?"""
         # fix urlparse exception
-        parsed = urlparse(iocextract.refang_url(self.artifact))
+        parsed = urlparse(iocextract.refang_data(self.artifact))
 
         # Handle RFC 2732 IPv6 URLs with and without port, as well as non-RFC IPv6 URLs
         if ']:' in parsed.netloc:
             ipv6 = ':'.join(parsed.netloc.split(':')[:-1])
         else:
             ipv6 = parsed.netloc
 
@@ -205,15 +203,15 @@
         Supported variables:
 
         * {ipaddress}
         * {defanged}
         * All supported variables from Artifact.format_message
         """
         return super(IPAddress, self).format_message(message, ipaddress=str(self),
-                                                     defanged=iocextract.defang(str(self)))
+                                                     defanged=iocextract.defang_data(str(self)))
 
 
     def _stringify(self):
         """Always returns deobfuscated IP."""
         return self.artifact.replace('[', '').replace(']', '').split('/')[0].split(':')[0].split(' ')[0]
 
 
@@ -248,15 +246,15 @@
         Supported variables:
 
         * {domain}
         * {defanged}
         * All supported variables from Artifact.format_message
         """
         return super(Domain, self).format_message(message, domain=str(self),
-                                                  defanged=iocextract.defang(str(self)))
+                                                  defanged=iocextract.defang_data(str(self)))
 
 
 class Hash(Artifact):
     """Hash artifact abstraction."""
     # Types
     MD5 = 'md5'
     SHA1 = 'sha1'
@@ -297,17 +295,32 @@
         """Allow string interpolation with artifact contents.
 
         Supported variables:
 
         * {yarasignature}
         * All supported variables from Artifact.format_message
         """
-        return super(YARASignature, self).format_message(message,
-                                                         yarasignature=str(self))
+        return super(YARASignature, self).format_message(message, yarasignature=str(self))
+
+class Email(Artifact):
+    """
+    Email artifact abstraction.
+    """
+
+    def format_message(self, message, **kwargs):
+        """
+        Allow string interpolation with artifact contents.
+
+        Supported variables:
+
+        * {email}
+        * All supported variables from Artifact.format_message
+        """
 
+        return super(Email, self).format_message(message, email=str(self))
 
 class Task(Artifact):
     """Generic Task artifact abstraction."""
     def format_message(self, message, **kwargs):
         """Allow string interpolation with artifact contents.
 
         Supported variables:
@@ -322,9 +335,10 @@
 # At the bottom because it uses the classes we just defined.
 STRING_MAP = {
     'url': URL,
     'ipaddress': IPAddress,
     'domain': Domain,
     'hash': Hash,
     'yarasignature': YARASignature,
+    'email': Email,
     'task': Task,
 }
```

### Comparing `threatingestor-1.0.3/threatingestor/config.py` & `threatingestor-1.1.0/threatingestor/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 import io
 import importlib
-
-
 import yaml
-from loguru import logger
 
+from loguru import logger
 
 from threatingestor.exceptions import IngestorError, PluginError
 import threatingestor.artifacts
 
-
 SOURCE = 'threatingestor.sources'
 OPERATOR = 'threatingestor.operators'
 
 INTERNAL_OPTIONS = [
     'saved_state',
     'module',
     'credentials',
```

### Comparing `threatingestor-1.0.3/threatingestor/extras/fswatcher.py` & `threatingestor-1.1.0/threatingestor/extras/fswatcher.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 import io
 import sys
 import time
-
-
 import watchdog.events
 import watchdog.observers
 
-
 import threatingestor.extras.queueworker
 
-
 class FSWatcher(
         watchdog.events.PatternMatchingEventHandler,
         threatingestor.extras.queueworker.QueueWorker):
     """Watch a directory for YARA rule changes.
 
     Send contents of the changed rule files to the queue.
     """
```

### Comparing `threatingestor-1.0.3/threatingestor/extras/pasteprocessor.py` & `threatingestor-1.1.0/threatingestor/extras/pasteprocessor.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 import sys
-
-
 import requests
-
-
 import threatingestor.extras.queueworker
 
-
 class PasteProcessor(threatingestor.extras.queueworker.QueueWorker):
-    """Read pastebin URLs from a queue, write raw content to a queue."""
+    """
+    Read pastebin URLs from a queue, write raw content to a queue.
+    """
 
     def do_work(self, job):
-        """From a paste URL, get the raw contents."""
+        """
+        From a paste URL, get the raw contents.
+        """
+        
         try:
             url = job['url']
-
         except KeyError:
             print(f"Bad job: {job}")
             return
 
         # Pastebin.com
         if url.startswith("https://pastebin.com/raw/"):
             pass
@@ -27,19 +26,19 @@
             start, end = url.split['.com/']
             url = '.com/raw/'.join([start, end])
 
         # Gist
         elif url.startswith("https://gist.github.com/") and not 'raw' in url:
             url = url + '/raw'
 
-        # Fetch and return.
+        # Fetch and return
         response = requests.get(url)
+
         return {
             'content': response.content,
             'reference': response.url,
         }
 
-
 if __name__ == "__main__":
     worker = PasteProcessor()
     worker.read_config(sys.argv[1])
     worker.run_forever()
```

### Comparing `threatingestor-1.0.3/threatingestor/extras/queueworker.py` & `threatingestor-1.1.0/threatingestor/extras/queueworker.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 import io
-import json
 import yaml
-
-
-import greenstalk
+import json
 import boto3
-
+import greenstalk
 
 import threatingestor.config
 import threatingestor.exceptions
 
-
 class QueueWorker:
     """Abstract base class for Queue Workers.
 
     Override do_work to implement child classes.
     """
     def __init__(self):
         self.config = {}
```

### Comparing `threatingestor-1.0.3/threatingestor/extras/webapp.py` & `threatingestor-1.1.0/threatingestor/extras/webapp.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 import sqlite3
-
-
 import hug
 
-
 DATABASE = 'artifacts.db'
 
 
 INDEX_HTML = """
 <html>
 <head>
     <script
```

### Comparing `threatingestor-1.0.3/threatingestor/operators/__init__.py` & `threatingestor-1.1.0/threatingestor/operators/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 import re
-
-
 from loguru import logger
 
 
 class Operator:
     """Base class for all Operator plugins.
 
     Note: This is an abstract class. You must extend ``__init__`` and call
```

### Comparing `threatingestor-1.0.3/threatingestor/operators/abstract_json.py` & `threatingestor-1.1.0/threatingestor/operators/abstract_json.py`

 * *Files identical despite different names*

### Comparing `threatingestor-1.0.3/threatingestor/operators/beanstalk.py` & `threatingestor-1.1.0/threatingestor/operators/beanstalk.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 import json
 
-
-from threatingestor.exceptions import DependencyError
 import threatingestor.artifacts
 from threatingestor.operators import abstract_json
-
+from threatingestor.exceptions import DependencyError
 
 try:
     import greenstalk
 except ImportError:
     raise DependencyError("Dependency greenstalk required for Beanstalk operator is not installed")
 
-
 class Plugin(abstract_json.AbstractPlugin):
     """Operator for Beanstalk work queue."""
     def __init__(self, host, port, queue_name, artifact_types=None,
             filter_string=None, allowed_sources=None, **kwargs):
         """Beanstalk operator."""
         self.queue = greenstalk.Client(host, port, use=queue_name)
```

### Comparing `threatingestor-1.0.3/threatingestor/operators/csv.py` & `threatingestor-1.1.0/threatingestor/operators/csv.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from __future__ import absolute_import
-import csv
 
+import csv
 
 import threatingestor.artifacts
 from threatingestor.operators import Operator
 
-
 class Plugin(Operator):
     """Operator for output to flat CSV file."""
     def __init__(self, filename, artifact_types=None, filter_string=None, allowed_sources=None):
         """CSV operator."""
         self.filename = filename
 
         super(Plugin, self).__init__(artifact_types, filter_string, allowed_sources)
```

### Comparing `threatingestor-1.0.3/threatingestor/operators/misp.py` & `threatingestor-1.1.0/threatingestor/operators/misp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 from __future__ import absolute_import
 
-
 import threatingestor.artifacts
 from threatingestor.operators import Operator
 from threatingestor.exceptions import DependencyError
 
-
 try:
     import pymisp
 except ImportError:
     raise DependencyError(
         "Dependency PyMISP required for MISP operator is not installed"
     )
```

### Comparing `threatingestor-1.0.3/threatingestor/operators/mysql.py` & `threatingestor-1.1.0/threatingestor/operators/mysql.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 import threatingestor.artifacts
 from threatingestor.operators import Operator
 from threatingestor.exceptions import DependencyError
 
-
 try:
     import pymysql
 except ImportError:
     raise DependencyError("Dependency pymysql required for MySQL operator is not installed")
 
-
 class Plugin(Operator):
     """Operator for MySQL."""
     def __init__(self, host, database, table, user=None, password='', port=3306,
                  artifact_types=None, filter_string=None, allowed_sources=None):
         """MySQL operator."""
         super(Plugin, self).__init__(artifact_types, filter_string, allowed_sources)
         self.artifact_types = artifact_types or [
```

### Comparing `threatingestor-1.0.3/threatingestor/operators/sqlite.py` & `threatingestor-1.1.0/threatingestor/operators/sqlite.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from __future__ import absolute_import
-import sqlite3
 
+import sqlite3
 
 import threatingestor.artifacts
 from threatingestor.operators import Operator
 
-
 class Plugin(Operator):
     """Operator for SQLite3."""
     def __init__(self, filename, artifact_types=None, filter_string=None, allowed_sources=None):
         """SQLite3 operator."""
         super(Plugin, self).__init__(artifact_types, filter_string, allowed_sources)
         self.artifact_types = artifact_types or [
             threatingestor.artifacts.Domain,
```

### Comparing `threatingestor-1.0.3/threatingestor/operators/sqs.py` & `threatingestor-1.1.0/threatingestor/operators/sqs.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 import json
 
-
 from threatingestor.exceptions import DependencyError
 import threatingestor.artifacts
 from threatingestor.operators import abstract_json
 
-
 try:
     import boto3
 except ImportError:
     raise DependencyError("Dependency boto3 required for SQS operator is not installed")
 
-
 class Plugin(abstract_json.AbstractPlugin):
     """Operator for Amazon SQS."""
     def __init__(self, aws_access_key_id, aws_secret_access_key, aws_region, queue_name,
             artifact_types=None, filter_string=None, allowed_sources=None, **kwargs):
         """SQS operator."""
         self.sqs = boto3.client('sqs', region_name=aws_region, aws_access_key_id=aws_access_key_id, aws_secret_access_key=aws_secret_access_key)
         self.queue_url = self.sqs.get_queue_url(QueueName=queue_name)['QueueUrl']
```

### Comparing `threatingestor-1.0.3/threatingestor/operators/threatkb.py` & `threatingestor-1.1.0/threatingestor/operators/threatkb.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 from __future__ import absolute_import
 
-
 import threatingestor.artifacts
 from threatingestor.operators import Operator
 from threatingestor.exceptions import DependencyError
 
-
 try:
     import threatkb
 except ImportError:
     raise DependencyError("Dependency threatkb required for ThreatKB operator is not installed")
 
-
 class Plugin(Operator):
     """Operator for InQuest ThreatKB."""
     def __init__(self, url, token, secret_key, state, artifact_types=None, filter_string=None, allowed_sources=None, use_https=False):
         """ThreatKB operator."""
         self.state = state
         self.api = threatkb.ThreatKB(url, token, secret_key, use_https=use_https)
```

### Comparing `threatingestor-1.0.3/threatingestor/operators/twitter.py` & `threatingestor-1.1.0/threatingestor/operators/twitter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 from __future__ import absolute_import
-import re
-
 
+import re
 import twitter
 from loguru import logger
 
-
 from threatingestor.operators import Operator
 import threatingestor.artifacts
 import threatingestor.exceptions
 
-
 TWEET_URL = re.compile(r'https://twitter\.com/\w{1,15}/status/\d+')
 
-
 class Plugin(Operator):
     """Operator for Twitter."""
     def __init__(self, api_key, api_secret_key, access_token, access_token_secret, status, **kwargs):
         self.api = twitter.Twitter(auth=twitter.OAuth(access_token, access_token_secret, api_key, api_secret_key))
         self.status = status
 
         # Validate status, for better error handling.
```

### Comparing `threatingestor-1.0.3/threatingestor/sources/__init__.py` & `threatingestor-1.1.0/threatingestor/sources/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,17 @@
 import re
 from urllib.parse import urlparse
 import itertools
-
-
 import iocextract
 from loguru import logger
 
-
 import threatingestor.artifacts
 
-
 TRUNCATE_LENGTH = 140
 
-
 class Source:
     """Base class for all Source plugins.
 
     Note: This is an abstract class. You must override ``__init__`` and ``run``
     in child classes. You should not override ``process_element``. When adding
     additional methods to child classes, consider prefixing the method name
     with an underscore to denote a ``_private_method``.
@@ -68,14 +63,15 @@
         artifact_type_count = {
             'domain': 0,
             'hash': 0,
             'ipaddress': 0,
             'task': 0,
             'url': 0,
             'yarasignature': 0,
+            'email': 0,
         }
 
         # Collect URLs and domains.
         scraped = itertools.chain(
             iocextract.extract_unencoded_urls(content),
             # Decode encoded URLs, since we can't operate on encoded ones.
             iocextract.extract_encoded_urls(content, refang=True),
@@ -148,14 +144,22 @@
             artifact = threatingestor.artifacts.Hash(hash_, self.name,
                                                      reference_link=reference_link,
                                                      reference_text=reference_text)
 
             artifact_list.append(artifact)
             artifact_type_count['hash'] += 1
 
+        # Collect emails.
+        scraped = itertools.chain(iocextract.extract_emails(content))
+
+        for email in scraped:
+            artifact_list.append(threatingestor.artifacts.Email(email, self.name, reference_link=reference_link, reference_text=reference_text))
+            
+            artifact_type_count['email'] += 1
+
         # Generate generic task.
         title = f"Manual Task: {reference_link}"
         description = f"URL: {reference_link}\nTask autogenerated by ThreatIngestor from source: {self.name}"
         artifact = threatingestor.artifacts.Task(title, self.name,
                                                  reference_link=reference_link,
                                                  reference_text=description)
         artifact_list.append(artifact)
```

### Comparing `threatingestor-1.0.3/threatingestor/sources/abstract_json.py` & `threatingestor-1.1.0/threatingestor/sources/abstract_json.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import jsonpath_rw
 
-
 from threatingestor.sources import Source
 
-
 class AbstractPlugin(Source):
 
     def __init__(self, name, paths, reference=None, **kwargs):
         """Set up JSON path expressions.
 
         Extend in child class.
         """
```

### Comparing `threatingestor-1.0.3/threatingestor/sources/beanstalk.py` & `threatingestor-1.1.0/threatingestor/sources/beanstalk.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 import json
 
-
 from threatingestor.exceptions import DependencyError
 from threatingestor.sources import abstract_json
 
-
 try:
     import greenstalk
 except ImportError:
     raise DependencyError("Dependency greenstalk required for Beastalk operator is not installed")
 
-
 BATCH_SIZE = 10
 
-
 class Plugin(abstract_json.AbstractPlugin):
     """Source for Beanstalk work queue."""
     def __init__(self, name, host, port, queue_name, paths, reference=None):
         """Beanstalk source."""
         super(Plugin, self).__init__(name, paths, reference)
         self.queue = greenstalk.Client(host, port, watch=queue_name)
```

### Comparing `threatingestor-1.0.3/threatingestor/sources/git.py` & `threatingestor-1.1.0/threatingestor/sources/git.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,30 @@
 import os
 import io
 import subprocess
-
-
 from loguru import logger
 
-
 from threatingestor.sources import Source
 from threatingestor.exceptions import DependencyError
 
-
 try:
     subprocess.check_output('git')
 except FileNotFoundError:
     raise DependencyError("System dependency Git required for Git source is not installed")
 except subprocess.CalledProcessError:
     # Non-zero exit codes are fine.
     pass
 
-
 YARA_FILE_EXTS = [
     '.rule',
     '.yar',
     '.yara',
     '.rules',
 ]
 
-
 class Plugin(Source):
 
     def __init__(self, name, url, local_path):
         self.name = name
         self.url = url
         self.local_path = local_path
```

### Comparing `threatingestor-1.0.3/threatingestor/sources/github.py` & `threatingestor-1.1.0/threatingestor/sources/github.py`

 * *Files identical despite different names*

### Comparing `threatingestor-1.0.3/threatingestor/sources/github_gist.py` & `threatingestor-1.1.0/threatingestor/sources/github_gist.py`

 * *Files identical despite different names*

### Comparing `threatingestor-1.0.3/threatingestor/sources/image.py` & `threatingestor-1.1.0/threatingestor/sources/image.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,62 +1,89 @@
-import cv2
-import pytesseract
-import iocextract
+import os
+import sys
+import string
+import random
 import requests
 import datetime
-import os
+import iocextract
 import numpy as np
+from loguru import logger
+
+try:
+    import numpy as np
+except ImportError:
+    logger.error("Missing the following package(s): numpy")
+    sys.exit()
+
+try:
+    import cv2
+except ImportError:
+    logger.error("Missing the following package(s): opencv-python")
+    sys.exit()
+
+try:
+    import pytesseract
+except ImportError:
+    logger.error("Missing the following package(s): pytesseract")
+    sys.exit()
 
 from threatingestor.sources import Source
 import threatingestor.artifacts
 
+# Creates a random string with a length of 5
+def tmp_name():
+    return "".join(random.choice(string.ascii_lowercase) for _ in range(5))
+
+tmp_file = str(tmp_name())
+
 class Plugin(Source):
     """
     Image text extraction using Google's OCR Tesseract engine and computer vision
     """
 
     def __init__(self, name, img=""):
         self.name = name
         self.img = img
 
         if "http" in img:
-            with open("/tmp/data.png", "wb") as i:
+            with open(f"/tmp/{tmp_file}", "wb") as i:
                 i.write(requests.get(str(self.img)).content)
 
     def run(self, saved_state):
         saved_state = datetime.datetime.utcnow().isoformat()[:-7] + "Z"
 
-        if os.path.exists("/tmp/data.png"):
-            data = cv2.imread("/tmp/data.png")
+        if os.path.exists(f"/tmp/{tmp_file}"):
+            data = cv2.imread(f"/tmp/{tmp_file}")
         else:
-            data = cv2.imread(self.img)
+            # No image is present
+            try:
+                data = cv2.imread(self.img)
+            except TypeError:
+                pass
 
         try:
             # Helps with preprocessing by converting to a grayscale
             grayscale_img = cv2.cvtColor(data, cv2.COLOR_BGR2GRAY)
 
-            # Creates a binary image by using the proper threshold from cv
-            binary_img = cv2.threshold(grayscale_img, 130, 255, cv2.THRESH_BINARY + cv2.THRESH_OTSU)[1]
-
-            # Inverts the binary
-            invert_img = cv2.bitwise_not(binary_img)
+            # Creates a binary image by using the proper threshold from cv and inverts the binary
+            invert_img = cv2.bitwise_not(cv2.threshold(grayscale_img, 130, 255, cv2.THRESH_BINARY + cv2.THRESH_OTSU)[1])
 
             # Helps with cleanup
-            noise_reduction = np.ones((2,2), np.uint8)
-            process_iter = cv2.erode(invert_img, noise_reduction, iterations = 1)
-            process_iter = cv2.dilate(process_iter, noise_reduction, iterations = 1)
+            process_iter = cv2.dilate(cv2.erode(invert_img, np.ones((2,2), np.uint8), iterations=1), np.ones((2,2), np.uint8), iterations=1)
 
             # Converts image data to a string
             img_data = pytesseract.image_to_string(process_iter)
 
             artifact_list = []
 
             title = "Image: {0}".format(self.img)
             description = 'URL: {u}\nTask autogenerated by ThreatIngestor from source: {s}'
             description = description.format(s=self.name, u=list(iocextract.extract_urls(img_data)))
             artifact = threatingestor.artifacts.Task(title, self.name, reference_link=str(list(iocextract.extract_urls(img_data))), reference_text=description)
             artifact_list.append(artifact)
+
+            os.remove(f"/tmp/{tmp_file}")
                 
         except cv2.error:
             raise FileNotFoundError
 
         return saved_state, artifact_list
```

### Comparing `threatingestor-1.0.3/threatingestor/sources/sqs.py` & `threatingestor-1.1.0/threatingestor/sources/sqs.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import json
 
-
 from threatingestor.exceptions import DependencyError
 from threatingestor.sources import abstract_json
 
-
 try:
     import boto3
 except ImportError:
     raise DependencyError("Dependency boto3 required for SQS operator is not installed")
 
 
 class Plugin(abstract_json.AbstractPlugin):
```

### Comparing `threatingestor-1.0.3/threatingestor/sources/twitter_follow_links.py` & `threatingestor-1.1.0/threatingestor/sources/twitter_follow_links.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 from __future__ import absolute_import
 
 import re
 import requests
 import twitter
+
 from loguru import logger
+from pyshorteners import Shortener, exceptions
 
 from threatingestor.sources import Source
-from threatingestor.utils.url_controller import UrlController
 
 TWEET_URL = 'https://twitter.com/{user}/status/{id}'
 WHITELIST_DOMAINS = r"pastebin\.com"
 
+s = Shortener()
+
 class Plugin(Source):
 
     def __init__(self, name, api_key, api_secret_key, access_token, access_token_secret, defanged_only=True, **kwargs):
         self.name = name
         self.api = twitter.Twitter(auth=twitter.OAuth(access_token, access_token_secret, api_key, api_secret_key))
 
         # Let the user decide whether to include non-obfuscated URLs or not.
@@ -91,15 +94,20 @@
                         req = requests.get(location)
                         saved_state = tweet['id']
                         artifacts += self.process_element(req.text, location, include_nonobfuscated=True)
 
                         logger.log('NOTIFY', f"Discovered paste: {location}")
 
                 except KeyError:
+                    
                     # Attempts to expand the URL if not available through Twitter
-                    tweet['content'] = tweet['content'].replace(url['url'], UrlController.expand_url(url['url']))
+                    try:
+                        tweet['content'] = tweet['content'].replace(url['url'], str(s.tinyurl.expand(url['url'])))
+                    except exceptions.ExpandingErrorException:
+                        # If unable to expand the URL, this exception is thrown
+                        pass
 
         return saved_state, artifacts
```

### Comparing `threatingestor-1.0.3/threatingestor/sources/web.py` & `threatingestor-1.1.0/threatingestor/sources/web.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import requests
 
-
 from threatingestor.sources import Source
 
-
 class Plugin(Source):
 
     def __init__(self, name, url):
         self.name = name
         self.url = url
```

### Comparing `threatingestor-1.0.3/threatingestor/state.py` & `threatingestor-1.1.0/threatingestor/state.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import sqlite3
 from loguru import logger
 
-
 import threatingestor.exceptions
 
-
 class State:
     """State DB management."""
     def __init__(self, dbname):
         """Set up a connection to the state DB."""
         try:
             self.conn = sqlite3.connect(dbname)
             self.cursor = self.conn.cursor()
```

### Comparing `threatingestor-1.0.3/threatingestor/whitelist.py` & `threatingestor-1.1.0/threatingestor/whitelist.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
+
 from pathlib import Path
 from typing import List, Set
-
 from loguru import logger
 
 class Whitelist:
     """Base class for Whitelist plugin."""
 
     def __init__(self, paths: List[str]):
         self.paths = paths
```

### Comparing `threatingestor-1.0.3/threatingestor.egg-info/PKG-INFO` & `threatingestor-1.1.0/threatingestor.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threatingestor
-Version: 1.0.3
+Version: 1.1.0
 Summary: Extract and aggregate IOCs from threat feeds.
 Home-page: https://github.com/InQuest/ThreatIngestor
 Author: InQuest Labs
 Author-email: labs@inquest.net
 License: GPL
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
@@ -12,173 +12,170 @@
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Security
 Classifier: Topic :: Internet
+Description-Content-Type: text/markdown
 Provides-Extra: twitter
 Provides-Extra: rss
 Provides-Extra: misp
 Provides-Extra: threatkb
 Provides-Extra: beanstalk
 Provides-Extra: sqs
 Provides-Extra: mysql
 Provides-Extra: extras
 Provides-Extra: all
 License-File: LICENSE
 
-ThreatIngestor
-==============
+# ThreatIngestor
 
-.. image:: https://inquest.net/images/inquest-badge.svg
-    :target: https://inquest.net/
-    :alt: Developed by InQuest
-.. image:: https://travis-ci.org/InQuest/ThreatIngestor.svg?branch=master
-    :target: https://travis-ci.org/InQuest/ThreatIngestor
-    :alt: Build Status (Travis CI)
-
-.. Change ?branch=develop to ?branch=master when merging into master
-.. image:: https://github.com/InQuest/ThreatIngestor/workflows/threatingestor-workflow/badge.svg?branch=develop
-    :target: https://github.com/InQuest/ThreatIngestor/actions
-    :alt: Build Status (GitHub Workflow)
-
-.. image:: https://readthedocs.org/projects/threatingestor/badge/?version=latest
-    :target: http://inquest.readthedocs.io/projects/threatingestor/en/latest/?badge=latest
-    :alt: Documentation Status
-.. .. image:: https://api.codacy.com/project/badge/Grade/a989bb12e9604d5a9577ce71848e7a2a
-..     :target: https://app.codacy.com/app/InQuest/ThreatIngestor
-..     :alt: Code Health
-.. .. image:: https://api.codacy.com/project/badge/Coverage/a989bb12e9604d5a9577ce71848e7a2a
-..     :target: https://app.codacy.com/app/InQuest/ThreatIngestor
-..     :alt: Test Coverage
-.. image:: http://img.shields.io/pypi/v/ThreatIngestor.svg
-    :target: https://pypi.python.org/pypi/ThreatIngestor
-    :alt: PyPi Version
-
-An extendable tool to extract and aggregate IOCs_ from threat feeds.
-
-Integrates out-of-the-box with ThreatKB_ and MISP_, and can fit seamlessly into any existing workflow with SQS_, Beanstalk_, and `custom plugins`_.
-
-Currently used by InQuest Labs IOC-DB: https://labs.inquest.net/iocdb.
-
-Overview
---------
-
-ThreatIngestor can be configured to watch Twitter, RSS feeds, or other sources, extract meaningful information such as malicious IPs/domains and YARA signatures, and send that information to another system for analysis.
-
-.. image:: https://inquest.readthedocs.io/projects/threatingestor/en/latest/_images/mermaid-multiple-operators.png
-    :target: https://inquest.readthedocs.io/projects/threatingestor/en/latest/workflows.html
-    :alt: ThreatIngestor flowchart with several sources feeding into multiple operators.
+![Build Status](https://github.com/InQuest/ThreatIngestor/workflows/threatingestor-workflow/badge.svg?branch=master)
+![Developed by InQuest](https://inquest.net/images/inquest-badge.svg)
 
-Try it out now with this `quick walkthrough`_, read more `ThreatIngestor walkthroughs`_ on the InQuest blog, and check out `labs.inquest.net/iocdb`_, an IOC aggregation and querying tool powered by ThreatIngestor.
+![Documentation Status](https://readthedocs.org/projects/threatingestor/badge/?version=latest)
+![PyPI Version](http://img.shields.io/pypi/v/ThreatIngestor.svg)
 
-Installation
-------------
+An extendable tool to extract and aggregate [IOCs](https://en.wikipedia.org/wiki/Indicator_of_compromise) from threat feeds.
+
+Integrates out-of-the-box with [ThreatKB](https://github.com/InQuest/ThreatKB) and [MISP](https://www.misp-project.org/), and can fit seamlessly into any existing workflow with [SQS](https://aws.amazon.com/sqs/), [Beanstalk](https://beanstalkd.github.io/), and [custom plugins](https://inquest.readthedocs.io/projects/threatingestor/en/latest/developing.html).
+
+Currently used by InQuest Labs IOC-DB: https://labs.inquest.net/iocdb
+
+## Overview
+
+ThreatIngestor can be configured to watch Twitter, RSS feeds, sitemap (XML) feeds, or other sources, extract meaningful information such as malicious IPs/domains and YARA signatures, and send that information to another system for analysis.
+
+![ThreatIngestor flowchart with several sources feeding into multiple operators](https://inquest.readthedocs.io/projects/threatingestor/en/latest/_images/mermaid-multiple-operators.png)
+
+Try it out now with this [quick walkthrough](https://inquest.readthedocs.io/projects/threatingestor/en/latest/welcome.html#try-it-out), read more [ThreatIngestor walkthroughs](https://inquest.net/taxonomy/term/42) on the InQuest blog, and check out [labs.inquest.net/iocdb](https://labs.inquest.net/iocdb), an IOC aggregation and querying tool powered by ThreatIngestor.
+
+## Installation
 
 ThreatIngestor requires Python 3.6+, with development headers.
 
-Install ThreatIngestor from PyPI::
+Install ThreatIngestor from PyPI:
 
-    pip install threatingestor
+```bash
+pip install threatingestor
+```
 
-Install optional dependencies for using some plugins, as needed::
+Install optional dependencies for using some plugins, as needed:
 
-    pip install threatingestor[all]
+```bash
+pip install threatingestor[all]
+```
 
-View the `full installation instructions`_ for more information.
+View the [full installation instructions](https://inquest.readthedocs.io/projects/threatingestor/en/latest/installation.html) for more information.
 
-Usage
------
+## Usage
 
-Create a new ``config.yml`` file, and configure each source and operator module you want to use. (See ``config.example.yml`` for layout.) Then run the script::
+Create a new ``config.yml`` file, and configure each source and operator module you want to use. (See ``config.example.yml`` for layout.) Then run the script:
 
-    threatingestor config.yml
+```bash
+threatingestor config.yml
+```
 
 By default, it will run forever, polling each configured source every 15 minutes.
 
-View the `full ThreatIngestor documentation`_ for more information.
+If you'd like to run the image extraction source, or include the image extraction functionality for other sources, you will need to be running Python 3.7 >= due to the dependencies:
 
-Plugins
--------
+```bash
+pip install opencv-python pytesseract numpy
+```
+
+View the [full ThreatIngestor documentation](https://inquest.readthedocs.io/projects/threatingestor/) for more information.
+
+## Plugins
 
 ThreatIngestor uses a plugin architecture with "source" (input) and "operator" (output) plugins. The currently supported integrations are:
 
-Sources
-~~~~~~~
+### Sources
 
-* `Beanstalk work queues <https://inquest.readthedocs.io/projects/threatingestor/en/latest/sources/beanstalk.html>`__
-* `Git repositories <https://inquest.readthedocs.io/projects/threatingestor/en/latest/sources/git.html>`__
-* `GitHub repository search <https://inquest.readthedocs.io/projects/threatingestor/en/latest/sources/github.html>`__
-* `Gists by username <https://inquest.readthedocs.io/projects/threatingestor/en/latest/sources/github_gist.html>`__
-* `RSS feeds <https://inquest.readthedocs.io/projects/threatingestor/en/latest/sources/rss.html>`__
-* `Sitemap blogs <https://inquest.readthedocs.io/projects/threatingestor/en/latest/sources/sitemap.html>`__
-* `Image extraction <https://inquest.readthedocs.io/projects/threatingestor/en/latest/sources/image.html>`__
-* `Amazon SQS queues <https://inquest.readthedocs.io/projects/threatingestor/en/latest/sources/sqs.html>`__
-* `Twitter <https://inquest.readthedocs.io/projects/threatingestor/en/latest/sources/twitter.html>`__
-* `Generic web pages <https://inquest.readthedocs.io/projects/threatingestor/en/latest/sources/web.html>`__
-
-Operators
-~~~~~~~~~
-
-* `Beanstalk work queues <https://inquest.readthedocs.io/projects/threatingestor/en/latest/operators/beanstalk.html>`__
-* `CSV files <https://inquest.readthedocs.io/projects/threatingestor/en/latest/operators/csv.html>`__
-* `MISP <https://inquest.readthedocs.io/projects/threatingestor/en/latest/operators/misp.html>`__
-* `MySQL table <https://inquest.readthedocs.io/projects/threatingestor/en/latest/operators/mysql.html>`__
-* `SQLite database <https://inquest.readthedocs.io/projects/threatingestor/en/latest/operators/sqlite.html>`__
-* `Amazon SQS queues <https://inquest.readthedocs.io/projects/threatingestor/en/latest/operators/sqs.html>`__
-* `ThreatKB <https://inquest.readthedocs.io/projects/threatingestor/en/latest/operators/threatkb.html>`__
-* `Twitter <https://inquest.readthedocs.io/projects/threatingestor/en/latest/operators/twitter.html>`__
+- [Git repositories](https://inquest.readthedocs.io/projects/threatingestor/en/latest/sources/git.html)
+- [GitHub repository search](https://inquest.readthedocs.io/projects/threatingestor/en/latest/sources/github.html)
+- [Gists by username](https://inquest.readthedocs.io/projects/threatingestor/en/latest/sources/github_gist.html)
+- [RSS feeds](https://inquest.readthedocs.io/projects/threatingestor/en/latest/sources/rss.html)
+- [Sitemap feeds](https://inquest.readthedocs.io/projects/threatingestor/en/latest/sources/sitemap.html)
+- [Image extraction](https://inquest.readthedocs.io/projects/threatingestor/en/latest/sources/image.html)
+- [Amazon SQS queues](https://inquest.readthedocs.io/projects/threatingestor/en/latest/sources/sqs.html)
+- [Twitter](https://inquest.readthedocs.io/projects/threatingestor/en/latest/sources/twitter.html)
+- [Generic web pages](https://inquest.readthedocs.io/projects/threatingestor/en/latest/sources/web.html)
+
+### Operators
+
+- [CSV files](https://inquest.readthedocs.io/projects/threatingestor/en/latest/operators/csv.html)
+- [MISP](https://inquest.readthedocs.io/projects/threatingestor/en/latest/operators/misp.html)
+- [MySQL table](https://inquest.readthedocs.io/projects/threatingestor/en/latest/operators/mysql.html)
+- [SQLite database](https://inquest.readthedocs.io/projects/threatingestor/en/latest/operators/sqlite.html)
+- [Amazon SQS queues](https://inquest.readthedocs.io/projects/threatingestor/en/latest/operators/sqs.html)
+- [ThreatKB](https://inquest.readthedocs.io/projects/threatingestor/en/latest/operators/threatkb.html)
+- [Twitter](https://inquest.readthedocs.io/projects/threatingestor/en/latest/operators/twitter.html)
 
-View the `full ThreatIngestor documentation`_ for more information on included plugins, and how to create your own.
+View the [full ThreatIngestor documentation](https://inquest.readthedocs.io/projects/threatingestor/) for more information on included plugins, and how to create your own.
 
-Threat Intel Sources
---------------------
+## Threat Intel Sources
 
 Looking for some threat intel sources to get started? InQuest has a Twitter List with several accounts that post C2 domains and IPs: https://twitter.com/InQuest/lists/ioc-feed. Note that you will need to apply for a Twitter developer account to use the ThreatIngestor Twitter Source. Take a look at ``config.example.yml`` to see how to set this list up as a source.
 
-For quicker setup, RSS feeds can be a great source of intelligence. Check out this example `RSS config file`_ for a few pre-configured security blogs.
+For quicker setup, RSS feeds can be a great source of intelligence. Check out this example [RSS config file](https://github.com/InQuest/ThreatIngestor/blob/master/rss.example.yml) for a few pre-configured security blogs.
 
-Support
--------
+## Support
 
-If you need help getting set up, or run into any issues, feel free to open an Issue_. You can also reach out to `@InQuest`_ on Twitter or read more about us on the web at https://www.inquest.net.
+If you need help getting set up, or run into any issues, feel free to open an [issue](https://github.com/InQuest/ThreatIngestor/issues). You can also reach out to [@InQuest](https://twitter.com/InQuest) on Twitter or read more about us on the web at https://www.inquest.net.
 
 We'd love to hear any feedback you have on ThreatIngestor, its documentation, or how you're putting it to work for you!
 
-Contributing
-------------
+## Contributing
+
+Issues and pull requests are welcomed. Please keep Python code PEP8 compliant. By submitting a pull request you agree to release your submissions under the terms of the [LICENSE](https://github.com/InQuest/ThreatIngestor/blob/master/LICENSE).
+
+## Docker
+
+
+### Production
+
+A `Dockerfile` is available for running ThreatIngestor within a Docker container.
+
+First, you'll need to build the container:
+
+```bash
+docker build . -t threatingestor
+```
+
+After that, you can mount the container by using this command:
+
+```bash
+docker run -it --mount type=bind,source=/,target=/dock threatingestor /bin/bash
+```
+
+After you've mounted the container and you're inside the `/bin/bash` shell, you can run ThreatIngestor like normal:
+
+```bash
+threatingestor config.yml
+```
+
+### Development
+
+There is also a Dockerfile.dev for building a development version of ThreatIngestor. All you need is an available .whl file, which can be generated with the following command:
+
+```bash
+python3 -m build 
+```
+
+After you've built the project, you can build the container:
+
+```bash
+docker build . -t threatingestor -f Dockerfile.dev
+```
 
-Issues and pull requests are welcomed. Please keep Python code PEP8 compliant. By submitting a pull request you agree to release your submissions under the terms of the LICENSE_.
+NOTE: If you run into any issues while building the development environment or running ThreatIngestor within the container, you may need to comment out the following lines in `Dockerfile.dev` to work properly:
 
-.. _ThreatKB: https://github.com/InQuest/ThreatKB
-.. _LICENSE: https://github.com/InQuest/threat-ingestors/blob/master/LICENSE
-.. _full ThreatIngestor Documentation: https://inquest.readthedocs.io/projects/threatingestor/
-.. _SQS: https://aws.amazon.com/sqs/
-.. _Beanstalk: https://beanstalkd.github.io/
-.. _MISP: https://www.misp-project.org/
-.. _custom plugins: https://inquest.readthedocs.io/projects/threatingestor/en/latest/developing.html
-.. _IOCs: https://en.wikipedia.org/wiki/Indicator_of_compromise
-.. _full installation instructions: https://inquest.readthedocs.io/projects/threatingestor/en/latest/installation.html
-.. _Issue: https://github.com/InQuest/ThreatIngestor/issues
-.. _@InQuest: https://twitter.com/InQuest
-.. _quick walkthrough: https://inquest.readthedocs.io/projects/threatingestor/en/latest/welcome.html#try-it-out
-.. _ThreatIngestor walkthroughs: https://inquest.net/taxonomy/term/42
-.. _RSS config file: https://github.com/InQuest/ThreatIngestor/blob/master/rss.example.yml
-.. _labs.inquest.net/iocdb: https://labs.inquest.net/iocdb
-
-Docker Container
-----------------
-
-A Dockerfile is now available for running ThreatIngestor within a Docker container.
-
-First, you'll need to build the container::
-
-    docker build . -t threat
-
-After that, you can mount the container for use using this command::
-
-    docker run -it --mount type=bind,source=/,target=/dock threat /bin/bash
-
-After you've mounted the container, and you're inside of the `/bin/bash` shell, you can run the threatingestor like normal::
-    
-    threatingestor config.yml
+```
+FROM ubuntu:18.04
+...
+# RUN apt-get install tesseract-ocr -y
+...
+# RUN pip3 install opencv-python pytesseract numpy
+...
+```
```

### Comparing `threatingestor-1.0.3/threatingestor.egg-info/SOURCES.txt` & `threatingestor-1.1.0/threatingestor.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 LICENSE
 MANIFEST.in
-README.rst
+README.md
 requirements-testing.txt
 requirements.txt
 setup.py
 tests/test_artifacts.py
 tests/test_config.py
 tests/test_ingestor.py
 tests/test_operators.py
@@ -18,15 +18,14 @@
 tests/test_operators_threatkb.py
 tests/test_operators_twitter.py
 tests/test_sources.py
 tests/test_sources_beanstalk.py
 tests/test_sources_git.py
 tests/test_sources_github.py
 tests/test_sources_json.py
-tests/test_sources_rss.py
 tests/test_sources_sqs.py
 tests/test_sources_twitter.py
 tests/test_sources_web.py
 tests/test_state.py
 tests/test_whitelist.py
 threatingestor/__init__.py
 threatingestor/artifacts.py
```

