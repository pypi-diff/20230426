# Comparing `tmp/pyIndego-2.0.9.tar.gz` & `tmp/pyIndego-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyIndego-2.0.9.tar", last modified: Wed Jun 24 06:48:09 2020, max compression
+gzip compressed data, was "pyIndego-3.0.0.tar", last modified: Wed Apr 26 19:31:14 2023, max compression
```

## Comparing `pyIndego-2.0.9.tar` & `pyIndego-3.0.0.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxrwxrwx   0        0        0        0 2020-06-24 06:48:09.098214 pyIndego-2.0.9/
--rw-rw-rw-   0        0        0    17492 2020-06-24 06:48:09.097206 pyIndego-2.0.9/PKG-INFO
--rw-rw-rw-   0        0        0    13466 2020-06-24 06:41:13.000000 pyIndego-2.0.9/README.md
-drwxrwxrwx   0        0        0        0 2020-06-24 06:48:09.028959 pyIndego-2.0.9/pyIndego/
--rw-rw-rw-   0        0        0      416 2020-06-16 19:20:07.000000 pyIndego-2.0.9/pyIndego/__init__.py
--rw-rw-rw-   0        0        0    10154 2020-06-23 13:00:31.000000 pyIndego-2.0.9/pyIndego/const.py
--rw-rw-rw-   0        0        0      929 2020-06-21 13:10:05.000000 pyIndego-2.0.9/pyIndego/helpers.py
--rw-rw-rw-   0        0        0     7990 2020-06-20 16:06:15.000000 pyIndego-2.0.9/pyIndego/indego_async_client.py
--rw-rw-rw-   0        0        0     7025 2020-06-24 06:38:58.000000 pyIndego-2.0.9/pyIndego/indego_base_client.py
--rw-rw-rw-   0        0        0     8462 2020-06-24 06:37:32.000000 pyIndego-2.0.9/pyIndego/indego_client.py
--rw-rw-rw-   0        0        0    51099 2020-06-16 19:20:07.000000 pyIndego-2.0.9/pyIndego/old_init.py
--rw-rw-rw-   0        0        0     5763 2020-06-21 11:34:04.000000 pyIndego-2.0.9/pyIndego/states.py
-drwxrwxrwx   0        0        0        0 2020-06-24 06:48:09.094181 pyIndego-2.0.9/pyIndego.egg-info/
--rw-rw-rw-   0        0        0    17492 2020-06-24 06:48:08.000000 pyIndego-2.0.9/pyIndego.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      365 2020-06-24 06:48:08.000000 pyIndego-2.0.9/pyIndego.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-06-24 06:48:08.000000 pyIndego-2.0.9/pyIndego.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2020-06-24 06:48:08.000000 pyIndego-2.0.9/pyIndego.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2020-06-24 06:48:08.000000 pyIndego-2.0.9/pyIndego.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2020-06-24 06:48:09.098214 pyIndego-2.0.9/setup.cfg
--rw-rw-rw-   0        0        0      662 2020-06-24 06:45:44.000000 pyIndego-2.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 19:31:14.851857 pyIndego-3.0.0/
+-rw-rw-rw-   0        0        0     1091 2023-04-26 19:17:02.000000 pyIndego-3.0.0/LICENSE.txt
+-rw-rw-rw-   0        0        0    21551 2023-04-26 19:31:14.851857 pyIndego-3.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0    21113 2023-04-26 19:17:02.000000 pyIndego-3.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-26 19:31:14.819347 pyIndego-3.0.0/pyIndego/
+-rw-rw-rw-   0        0        0      397 2023-04-26 19:17:02.000000 pyIndego-3.0.0/pyIndego/__init__.py
+-rw-rw-rw-   0        0        0     6589 2023-04-26 19:22:15.000000 pyIndego-3.0.0/pyIndego/const.py
+-rw-rw-rw-   0        0        0     2301 2023-04-26 19:17:02.000000 pyIndego-3.0.0/pyIndego/helpers.py
+-rw-rw-rw-   0        0        0    22250 2023-04-26 19:17:02.000000 pyIndego-3.0.0/pyIndego/indego_async_client.py
+-rw-rw-rw-   0        0        0    14888 2023-04-26 19:17:02.000000 pyIndego-3.0.0/pyIndego/indego_base_client.py
+-rw-rw-rw-   0        0        0    17567 2023-04-26 19:17:02.000000 pyIndego-3.0.0/pyIndego/indego_client.py
+-rw-rw-rw-   0        0        0     9103 2023-04-26 19:17:02.000000 pyIndego-3.0.0/pyIndego/states.py
+drwxrwxrwx   0        0        0        0 2023-04-26 19:31:14.846847 pyIndego-3.0.0/pyIndego.egg-info/
+-rw-rw-rw-   0        0        0    21551 2023-04-26 19:31:14.000000 pyIndego-3.0.0/pyIndego.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      395 2023-04-26 19:31:14.000000 pyIndego-3.0.0/pyIndego.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 19:31:14.000000 pyIndego-3.0.0/pyIndego.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       86 2023-04-26 19:31:14.000000 pyIndego-3.0.0/pyIndego.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-26 19:31:14.000000 pyIndego-3.0.0/pyIndego.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-26 19:31:14.851857 pyIndego-3.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      809 2023-04-26 19:30:25.000000 pyIndego-3.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 19:31:14.846847 pyIndego-3.0.0/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-26 19:17:02.000000 pyIndego-3.0.0/tests/__init__.py
+-rw-rw-rw-   0        0        0    39869 2023-04-26 19:17:02.000000 pyIndego-3.0.0/tests/test_indego.py
```

