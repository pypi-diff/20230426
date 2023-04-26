# Comparing `tmp/avassa-client-0.0.1.tar.gz` & `tmp/avassa-client-2023.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/avassa-client-0.0.1.tar", last modified: Fri Jan  8 09:09:06 2021, max compression
+gzip compressed data, was "avassa-client-2023.4.0.tar", last modified: Tue Apr 25 11:23:57 2023, max compression
```

## Comparing `avassa-client-0.0.1.tar` & `avassa-client-2023.4.0.tar`

### file list

```diff
@@ -1,10 +1,15 @@
-drwxrwxr-x   0 frja      (1001) frja      (1001)        0 2021-01-08 09:09:06.009025 avassa-client-0.0.1/
--rw-rw-r--   0 frja      (1001) frja      (1001)      454 2021-01-08 09:09:06.009025 avassa-client-0.0.1/PKG-INFO
--rw-rw-r--   0 frja      (1001) frja      (1001)       14 2021-01-08 08:47:51.000000 avassa-client-0.0.1/README.md
-drwxrwxr-x   0 frja      (1001) frja      (1001)        0 2021-01-08 09:09:06.009025 avassa-client-0.0.1/avassa_client.egg-info/
--rw-rw-r--   0 frja      (1001) frja      (1001)      454 2021-01-08 09:09:05.000000 avassa-client-0.0.1/avassa_client.egg-info/PKG-INFO
--rw-rw-r--   0 frja      (1001) frja      (1001)      166 2021-01-08 09:09:05.000000 avassa-client-0.0.1/avassa_client.egg-info/SOURCES.txt
--rw-rw-r--   0 frja      (1001) frja      (1001)        1 2021-01-08 09:09:05.000000 avassa-client-0.0.1/avassa_client.egg-info/dependency_links.txt
--rw-rw-r--   0 frja      (1001) frja      (1001)        1 2021-01-08 09:09:05.000000 avassa-client-0.0.1/avassa_client.egg-info/top_level.txt
--rw-rw-r--   0 frja      (1001) frja      (1001)       38 2021-01-08 09:09:06.009025 avassa-client-0.0.1/setup.cfg
--rw-rw-r--   0 frja      (1001) frja      (1001)      663 2021-01-08 09:09:03.000000 avassa-client-0.0.1/setup.py
+drwxr-xr-x   0 frja       (501) staff       (20)        0 2023-04-25 11:23:57.831779 avassa-client-2023.4.0/
+-rw-r--r--   0 frja       (501) staff       (20)    11343 2023-04-25 10:38:10.000000 avassa-client-2023.4.0/LICENSE
+-rw-r--r--   0 frja       (501) staff       (20)    13996 2023-04-25 11:23:57.831560 avassa-client-2023.4.0/PKG-INFO
+-rw-r--r--   0 frja       (501) staff       (20)      548 2023-04-25 10:38:10.000000 avassa-client-2023.4.0/README.md
+drwxr-xr-x   0 frja       (501) staff       (20)        0 2023-04-25 11:23:57.830717 avassa-client-2023.4.0/avassa_client/
+-rw-r--r--   0 frja       (501) staff       (20)     9244 2023-04-25 10:38:10.000000 avassa-client-2023.4.0/avassa_client/__init__.py
+-rw-r--r--   0 frja       (501) staff       (20)    16409 2023-04-25 10:38:10.000000 avassa-client-2023.4.0/avassa_client/volga.py
+drwxr-xr-x   0 frja       (501) staff       (20)        0 2023-04-25 11:23:57.831329 avassa-client-2023.4.0/avassa_client.egg-info/
+-rw-r--r--   0 frja       (501) staff       (20)    13996 2023-04-25 11:23:57.000000 avassa-client-2023.4.0/avassa_client.egg-info/PKG-INFO
+-rw-r--r--   0 frja       (501) staff       (20)      265 2023-04-25 11:23:57.000000 avassa-client-2023.4.0/avassa_client.egg-info/SOURCES.txt
+-rw-r--r--   0 frja       (501) staff       (20)        1 2023-04-25 11:23:57.000000 avassa-client-2023.4.0/avassa_client.egg-info/dependency_links.txt
+-rw-r--r--   0 frja       (501) staff       (20)       15 2023-04-25 11:23:57.000000 avassa-client-2023.4.0/avassa_client.egg-info/requires.txt
+-rw-r--r--   0 frja       (501) staff       (20)       14 2023-04-25 11:23:57.000000 avassa-client-2023.4.0/avassa_client.egg-info/top_level.txt
+-rw-r--r--   0 frja       (501) staff       (20)      654 2023-04-25 11:21:14.000000 avassa-client-2023.4.0/pyproject.toml
+-rw-r--r--   0 frja       (501) staff       (20)       38 2023-04-25 11:23:57.831819 avassa-client-2023.4.0/setup.cfg
```

