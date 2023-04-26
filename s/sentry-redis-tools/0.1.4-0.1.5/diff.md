# Comparing `tmp/sentry-redis-tools-0.1.4.tar.gz` & `tmp/sentry-redis-tools-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentry-redis-tools-0.1.4.tar", last modified: Thu Apr 20 15:13:19 2023, max compression
+gzip compressed data, was "sentry-redis-tools-0.1.5.tar", last modified: Wed Apr 26 19:05:01 2023, max compression
```

## Comparing `sentry-redis-tools-0.1.4.tar` & `sentry-redis-tools-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:13:19.563357 sentry-redis-tools-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-04-20 15:13:15.000000 sentry-redis-tools-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-20 15:13:19.563357 sentry-redis-tools-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-20 15:13:15.000000 sentry-redis-tools-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:13:19.563357 sentry-redis-tools-0.1.4/sentry_redis_tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 15:13:15.000000 sentry-redis-tools-0.1.4/sentry_redis_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-04-20 15:13:15.000000 sentry-redis-tools-0.1.4/sentry_redis_tools/failover_redis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:13:19.563357 sentry-redis-tools-0.1.4/sentry_redis_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-20 15:13:19.000000 sentry-redis-tools-0.1.4/sentry_redis_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-20 15:13:19.000000 sentry-redis-tools-0.1.4/sentry_redis_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 15:13:19.000000 sentry-redis-tools-0.1.4/sentry_redis_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 15:13:19.000000 sentry-redis-tools-0.1.4/sentry_redis_tools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-20 15:13:19.000000 sentry-redis-tools-0.1.4/sentry_redis_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-20 15:13:19.000000 sentry-redis-tools-0.1.4/sentry_redis_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 15:13:19.563357 sentry-redis-tools-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-20 15:13:15.000000 sentry-redis-tools-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:05:01.142792 sentry-redis-tools-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-04-26 19:04:55.000000 sentry-redis-tools-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-26 19:05:01.142792 sentry-redis-tools-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-26 19:04:55.000000 sentry-redis-tools-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:05:01.142792 sentry-redis-tools-0.1.5/sentry_redis_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 19:04:55.000000 sentry-redis-tools-0.1.5/sentry_redis_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19656 2023-04-26 19:04:55.000000 sentry-redis-tools-0.1.5/sentry_redis_tools/cardinality_limiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-26 19:04:55.000000 sentry-redis-tools-0.1.5/sentry_redis_tools/clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-04-26 19:04:55.000000 sentry-redis-tools-0.1.5/sentry_redis_tools/failover_redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-26 19:04:55.000000 sentry-redis-tools-0.1.5/sentry_redis_tools/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14200 2023-04-26 19:04:55.000000 sentry-redis-tools-0.1.5/sentry_redis_tools/sliding_windows_rate_limiter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:05:01.142792 sentry-redis-tools-0.1.5/sentry_redis_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-26 19:05:00.000000 sentry-redis-tools-0.1.5/sentry_redis_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-26 19:05:01.000000 sentry-redis-tools-0.1.5/sentry_redis_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 19:05:00.000000 sentry-redis-tools-0.1.5/sentry_redis_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 19:05:00.000000 sentry-redis-tools-0.1.5/sentry_redis_tools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-26 19:05:00.000000 sentry-redis-tools-0.1.5/sentry_redis_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-26 19:05:00.000000 sentry-redis-tools-0.1.5/sentry_redis_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 19:05:01.142792 sentry-redis-tools-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-26 19:04:55.000000 sentry-redis-tools-0.1.5/setup.py
```

### Comparing `sentry-redis-tools-0.1.4/LICENSE` & `sentry-redis-tools-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sentry-redis-tools-0.1.4/sentry_redis_tools/failover_redis.py` & `sentry-redis-tools-0.1.5/sentry_redis_tools/failover_redis.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import random
 import time
 from typing import Any
 
-from redis.client import StrictRedis
+from sentry_redis_tools.clients import StrictRedis
 from redis.exceptions import (
     ConnectionError,
     ReadOnlyError,
     TimeoutError,
 )
```

### Comparing `sentry-redis-tools-0.1.4/setup.py` & `sentry-redis-tools-0.1.5/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 from typing import Sequence
 
 
 setup(
     name="sentry-redis-tools",
-    version="0.1.4",
+    version="0.1.5",
     author="Sentry",
     author_email="oss@sentry.io",
     url="https://github.com/getsentry/sentry-redis-tools",
     description="Common utilities related to how Sentry uses Redis",
     zip_safe=False,
     install_requires=['redis>=3.0'],
     packages=find_packages(exclude=("tests", "tests.*")),
```

