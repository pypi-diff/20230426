# Comparing `tmp/scalems-0.0.0a1.tar.gz` & `tmp/scalems-0.0.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scalems-0.0.0a1.tar", last modified: Fri Feb  3 13:58:27 2023, max compression
+gzip compressed data, was "scalems-0.0.1b1.tar", last modified: Wed Apr 26 17:22:55 2023, max compression
```

## Comparing `scalems-0.0.0a1.tar` & `scalems-0.0.1b1.tar`

### file list

```diff
@@ -1,58 +1,69 @@
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-02-03 13:58:27.973515 scalems-0.0.0a1/
--rw-r--r--   0 eric       (501) staff       (20)    26526 2022-10-13 13:53:44.000000 scalems-0.0.0a1/LICENSE
--rw-r--r--   0 eric       (501) staff       (20)     3547 2023-02-03 13:58:27.973203 scalems-0.0.0a1/PKG-INFO
--rw-r--r--   0 eric       (501) staff       (20)     2970 2022-12-15 15:31:32.000000 scalems-0.0.0a1/README.md
--rw-r--r--   0 eric       (501) staff       (20)     1974 2023-02-03 13:57:51.000000 scalems-0.0.0a1/pyproject.toml
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-02-03 13:58:27.944806 scalems-0.0.0a1/scalems.egg-info/
--rw-r--r--   0 eric       (501) staff       (20)     3547 2023-02-03 13:58:27.000000 scalems-0.0.0a1/scalems.egg-info/PKG-INFO
--rw-r--r--   0 eric       (501) staff       (20)     1161 2023-02-03 13:58:27.000000 scalems-0.0.0a1/scalems.egg-info/SOURCES.txt
--rw-r--r--   0 eric       (501) staff       (20)        1 2023-02-03 13:58:27.000000 scalems-0.0.0a1/scalems.egg-info/dependency_links.txt
--rw-r--r--   0 eric       (501) staff       (20)       68 2023-02-03 13:58:27.000000 scalems-0.0.0a1/scalems.egg-info/entry_points.txt
--rw-r--r--   0 eric       (501) staff       (20)        1 2022-12-05 14:25:19.000000 scalems-0.0.0a1/scalems.egg-info/not-zip-safe
--rw-r--r--   0 eric       (501) staff       (20)      132 2023-02-03 13:58:27.000000 scalems-0.0.0a1/scalems.egg-info/requires.txt
--rw-r--r--   0 eric       (501) staff       (20)        8 2023-02-03 13:58:27.000000 scalems-0.0.0a1/scalems.egg-info/top_level.txt
--rw-r--r--   0 eric       (501) staff       (20)       38 2023-02-03 13:58:27.973622 scalems-0.0.0a1/setup.cfg
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-02-03 13:58:27.936316 scalems-0.0.0a1/src/
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-02-03 13:58:27.957619 scalems-0.0.0a1/src/scalems/
--rw-r--r--   0 eric       (501) staff       (20)     2995 2023-01-09 11:13:55.000000 scalems-0.0.0a1/src/scalems/__init__.py
--rw-r--r--   0 eric       (501) staff       (20)      553 2022-12-15 15:31:32.000000 scalems-0.0.0a1/src/scalems/_types.py
--rw-r--r--   0 eric       (501) staff       (20)       24 2023-02-03 13:58:27.000000 scalems-0.0.0a1/src/scalems/_version.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-02-03 13:58:27.959092 scalems-0.0.0a1/src/scalems/call/
--rw-r--r--   0 eric       (501) staff       (20)    15786 2023-02-03 08:03:49.000000 scalems-0.0.0a1/src/scalems/call/__init__.py
--rw-r--r--   0 eric       (501) staff       (20)      102 2023-01-24 14:08:03.000000 scalems-0.0.0a1/src/scalems/call/__main__.py
--rw-r--r--   0 eric       (501) staff       (20)    10755 2023-01-04 17:26:04.000000 scalems-0.0.0a1/src/scalems/commands.py
--rw-r--r--   0 eric       (501) staff       (20)     1647 2023-01-16 14:03:10.000000 scalems-0.0.0a1/src/scalems/compat.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-02-03 13:58:27.959831 scalems-0.0.0a1/src/scalems/context/
--rw-r--r--   0 eric       (501) staff       (20)     1879 2023-01-16 14:23:26.000000 scalems-0.0.0a1/src/scalems/context/__init__.py
--rw-r--r--   0 eric       (501) staff       (20)     2873 2023-01-09 11:14:17.000000 scalems-0.0.0a1/src/scalems/exceptions.py
--rw-r--r--   0 eric       (501) staff       (20)    26812 2023-02-03 07:57:33.000000 scalems-0.0.0a1/src/scalems/execution.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-02-03 13:58:27.960598 scalems-0.0.0a1/src/scalems/file/
--rw-r--r--   0 eric       (501) staff       (20)     8205 2023-01-16 11:21:08.000000 scalems-0.0.0a1/src/scalems/file/__init__.py
--rw-r--r--   0 eric       (501) staff       (20)    13542 2023-01-15 11:20:23.000000 scalems-0.0.0a1/src/scalems/identifiers.py
--rw-r--r--   0 eric       (501) staff       (20)    13081 2023-02-03 07:58:33.000000 scalems-0.0.0a1/src/scalems/invocation.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-02-03 13:58:27.962811 scalems-0.0.0a1/src/scalems/local/
--rw-r--r--   0 eric       (501) staff       (20)    10510 2023-01-09 10:58:38.000000 scalems-0.0.0a1/src/scalems/local/__init__.py
--rw-r--r--   0 eric       (501) staff       (20)      247 2022-12-15 15:31:32.000000 scalems-0.0.0a1/src/scalems/local/__main__.py
--rw-r--r--   0 eric       (501) staff       (20)    11347 2023-01-04 17:26:04.000000 scalems-0.0.0a1/src/scalems/local/operations.py
--rw-r--r--   0 eric       (501) staff       (20)     1906 2023-01-04 17:21:23.000000 scalems-0.0.0a1/src/scalems/logger.py
--rw-r--r--   0 eric       (501) staff       (20)    10204 2022-12-15 15:31:32.000000 scalems-0.0.0a1/src/scalems/messages.py
--rw-r--r--   0 eric       (501) staff       (20)       47 2021-08-27 15:59:17.000000 scalems-0.0.0a1/src/scalems/py.typed
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-02-03 13:58:27.965057 scalems-0.0.0a1/src/scalems/radical/
--rw-r--r--   0 eric       (501) staff       (20)     2733 2023-01-25 13:30:48.000000 scalems-0.0.0a1/src/scalems/radical/__init__.py
--rw-r--r--   0 eric       (501) staff       (20)      336 2023-01-18 10:57:59.000000 scalems-0.0.0a1/src/scalems/radical/__main__.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-02-03 13:58:27.966354 scalems-0.0.0a1/src/scalems/radical/raptor/
--rw-r--r--   0 eric       (501) staff       (20)    62196 2023-01-25 12:06:44.000000 scalems-0.0.0a1/src/scalems/radical/raptor/__init__.py
--rw-r--r--   0 eric       (501) staff       (20)    81520 2023-02-03 08:03:49.000000 scalems-0.0.0a1/src/scalems/radical/runtime.py
--rw-r--r--   0 eric       (501) staff       (20)    22734 2022-12-15 15:31:32.000000 scalems-0.0.0a1/src/scalems/serialization.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-02-03 13:58:27.968569 scalems-0.0.0a1/src/scalems/store/
--rw-r--r--   0 eric       (501) staff       (20)    33876 2023-02-03 13:57:51.000000 scalems-0.0.0a1/src/scalems/store/__init__.py
--rw-r--r--   0 eric       (501) staff       (20)     5541 2023-01-15 11:20:23.000000 scalems-0.0.0a1/src/scalems/store/_lock.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-02-03 13:58:27.969740 scalems-0.0.0a1/src/scalems/subprocess/
--rw-r--r--   0 eric       (501) staff       (20)     1161 2022-12-15 15:31:32.000000 scalems-0.0.0a1/src/scalems/subprocess/__init__.py
--rw-r--r--   0 eric       (501) staff       (20)    18420 2023-02-03 07:58:33.000000 scalems-0.0.0a1/src/scalems/subprocess/_subprocess.py
--rw-r--r--   0 eric       (501) staff       (20)      658 2023-01-04 17:26:04.000000 scalems-0.0.0a1/src/scalems/unique.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-02-03 13:58:27.970765 scalems-0.0.0a1/src/scalems/workflow/
--rw-r--r--   0 eric       (501) staff       (20)    62292 2023-02-03 13:57:51.000000 scalems-0.0.0a1/src/scalems/workflow/__init__.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-02-03 13:58:27.972538 scalems-0.0.0a1/src/scalems/wrappers/
--rw-r--r--   0 eric       (501) staff       (20)     8282 2021-09-07 15:49:13.000000 scalems-0.0.0a1/src/scalems/wrappers/__init__.py
--rw-r--r--   0 eric       (501) staff       (20)     7787 2023-01-04 17:26:04.000000 scalems-0.0.0a1/src/scalems/wrappers/gromacs.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-26 17:22:55.888139 scalems-0.0.1b1/
+-rw-r--r--   0 eric       (501) staff       (20)    26526 2022-10-13 13:53:44.000000 scalems-0.0.1b1/LICENSE
+-rw-r--r--   0 eric       (501) staff       (20)     3547 2023-04-26 17:22:55.887364 scalems-0.0.1b1/PKG-INFO
+-rw-r--r--   0 eric       (501) staff       (20)     2970 2022-12-15 15:31:32.000000 scalems-0.0.1b1/README.md
+-rw-r--r--   0 eric       (501) staff       (20)     1980 2023-04-25 16:19:05.000000 scalems-0.0.1b1/pyproject.toml
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-26 17:22:55.842546 scalems-0.0.1b1/scalems.egg-info/
+-rw-r--r--   0 eric       (501) staff       (20)     3547 2023-04-26 17:22:55.000000 scalems-0.0.1b1/scalems.egg-info/PKG-INFO
+-rw-r--r--   0 eric       (501) staff       (20)     1424 2023-04-26 17:22:55.000000 scalems-0.0.1b1/scalems.egg-info/SOURCES.txt
+-rw-r--r--   0 eric       (501) staff       (20)        1 2023-04-26 17:22:55.000000 scalems-0.0.1b1/scalems.egg-info/dependency_links.txt
+-rw-r--r--   0 eric       (501) staff       (20)       68 2023-04-26 17:22:55.000000 scalems-0.0.1b1/scalems.egg-info/entry_points.txt
+-rw-r--r--   0 eric       (501) staff       (20)        1 2022-12-05 14:25:19.000000 scalems-0.0.1b1/scalems.egg-info/not-zip-safe
+-rw-r--r--   0 eric       (501) staff       (20)      132 2023-04-26 17:22:55.000000 scalems-0.0.1b1/scalems.egg-info/requires.txt
+-rw-r--r--   0 eric       (501) staff       (20)        8 2023-04-26 17:22:55.000000 scalems-0.0.1b1/scalems.egg-info/top_level.txt
+-rw-r--r--   0 eric       (501) staff       (20)       38 2023-04-26 17:22:55.888369 scalems-0.0.1b1/setup.cfg
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-26 17:22:55.832113 scalems-0.0.1b1/src/
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-26 17:22:55.854713 scalems-0.0.1b1/src/scalems/
+-rw-r--r--   0 eric       (501) staff       (20)     2995 2023-01-09 11:13:55.000000 scalems-0.0.1b1/src/scalems/__init__.py
+-rw-r--r--   0 eric       (501) staff       (20)      553 2022-12-15 15:31:32.000000 scalems-0.0.1b1/src/scalems/_types.py
+-rw-r--r--   0 eric       (501) staff       (20)       24 2023-04-26 17:22:55.000000 scalems-0.0.1b1/src/scalems/_version.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-26 17:22:55.856716 scalems-0.0.1b1/src/scalems/call/
+-rw-r--r--   0 eric       (501) staff       (20)    17659 2023-04-25 16:17:43.000000 scalems-0.0.1b1/src/scalems/call/__init__.py
+-rw-r--r--   0 eric       (501) staff       (20)      102 2023-03-08 08:35:01.000000 scalems-0.0.1b1/src/scalems/call/__main__.py
+-rw-r--r--   0 eric       (501) staff       (20)    10755 2023-01-04 17:26:04.000000 scalems-0.0.1b1/src/scalems/commands.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-26 17:22:55.857789 scalems-0.0.1b1/src/scalems/context/
+-rw-r--r--   0 eric       (501) staff       (20)     1879 2023-03-27 14:38:51.000000 scalems-0.0.1b1/src/scalems/context/__init__.py
+-rw-r--r--   0 eric       (501) staff       (20)     2873 2023-01-09 11:14:17.000000 scalems-0.0.1b1/src/scalems/exceptions.py
+-rw-r--r--   0 eric       (501) staff       (20)    27014 2023-04-25 15:56:49.000000 scalems-0.0.1b1/src/scalems/execution.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-26 17:22:55.858753 scalems-0.0.1b1/src/scalems/file/
+-rw-r--r--   0 eric       (501) staff       (20)     8407 2023-04-25 15:55:46.000000 scalems-0.0.1b1/src/scalems/file/__init__.py
+-rw-r--r--   0 eric       (501) staff       (20)    13542 2023-01-15 11:20:23.000000 scalems-0.0.1b1/src/scalems/identifiers.py
+-rw-r--r--   0 eric       (501) staff       (20)    12930 2023-03-27 14:14:03.000000 scalems-0.0.1b1/src/scalems/invocation.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-26 17:22:55.864549 scalems-0.0.1b1/src/scalems/local/
+-rw-r--r--   0 eric       (501) staff       (20)    10510 2023-03-22 15:39:49.000000 scalems-0.0.1b1/src/scalems/local/__init__.py
+-rw-r--r--   0 eric       (501) staff       (20)      247 2022-12-15 15:31:32.000000 scalems-0.0.1b1/src/scalems/local/__main__.py
+-rw-r--r--   0 eric       (501) staff       (20)    11347 2023-01-04 17:26:04.000000 scalems-0.0.1b1/src/scalems/local/operations.py
+-rw-r--r--   0 eric       (501) staff       (20)     1906 2023-01-04 17:21:23.000000 scalems-0.0.1b1/src/scalems/logger.py
+-rw-r--r--   0 eric       (501) staff       (20)    10204 2022-12-15 15:31:32.000000 scalems-0.0.1b1/src/scalems/messages.py
+-rw-r--r--   0 eric       (501) staff       (20)       47 2021-08-27 15:59:17.000000 scalems-0.0.1b1/src/scalems/py.typed
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-26 17:22:55.867459 scalems-0.0.1b1/src/scalems/radical/
+-rw-r--r--   0 eric       (501) staff       (20)     2552 2023-03-27 14:14:03.000000 scalems-0.0.1b1/src/scalems/radical/__init__.py
+-rw-r--r--   0 eric       (501) staff       (20)      336 2023-01-18 10:57:59.000000 scalems-0.0.1b1/src/scalems/radical/__main__.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-26 17:22:55.868488 scalems-0.0.1b1/src/scalems/radical/raptor/
+-rw-r--r--   0 eric       (501) staff       (20)    62350 2023-04-25 16:17:43.000000 scalems-0.0.1b1/src/scalems/radical/raptor/__init__.py
+-rw-r--r--   0 eric       (501) staff       (20)    90832 2023-04-25 16:17:43.000000 scalems-0.0.1b1/src/scalems/radical/runtime.py
+-rw-r--r--   0 eric       (501) staff       (20)    22734 2022-12-15 15:31:32.000000 scalems-0.0.1b1/src/scalems/serialization.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-26 17:22:55.870496 scalems-0.0.1b1/src/scalems/store/
+-rw-r--r--   0 eric       (501) staff       (20)    34546 2023-04-25 15:55:46.000000 scalems-0.0.1b1/src/scalems/store/__init__.py
+-rw-r--r--   0 eric       (501) staff       (20)     5541 2023-01-15 11:20:23.000000 scalems-0.0.1b1/src/scalems/store/_lock.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-26 17:22:55.872703 scalems-0.0.1b1/src/scalems/subprocess/
+-rw-r--r--   0 eric       (501) staff       (20)     1161 2022-12-15 15:31:32.000000 scalems-0.0.1b1/src/scalems/subprocess/__init__.py
+-rw-r--r--   0 eric       (501) staff       (20)    18289 2023-03-27 14:38:09.000000 scalems-0.0.1b1/src/scalems/subprocess/_subprocess.py
+-rw-r--r--   0 eric       (501) staff       (20)      658 2023-01-04 17:26:04.000000 scalems-0.0.1b1/src/scalems/unique.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-26 17:22:55.873780 scalems-0.0.1b1/src/scalems/workflow/
+-rw-r--r--   0 eric       (501) staff       (20)    62304 2023-04-25 16:17:37.000000 scalems-0.0.1b1/src/scalems/workflow/__init__.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-26 17:22:55.875788 scalems-0.0.1b1/src/scalems/wrappers/
+-rw-r--r--   0 eric       (501) staff       (20)     8282 2021-09-07 15:49:13.000000 scalems-0.0.1b1/src/scalems/wrappers/__init__.py
+-rw-r--r--   0 eric       (501) staff       (20)     7787 2023-01-04 17:26:04.000000 scalems-0.0.1b1/src/scalems/wrappers/gromacs.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-26 17:22:55.886387 scalems-0.0.1b1/tests/
+-rw-r--r--   0 eric       (501) staff       (20)     3167 2023-03-08 08:35:01.000000 scalems-0.0.1b1/tests/test_call.py
+-rw-r--r--   0 eric       (501) staff       (20)     7488 2023-04-25 15:55:46.000000 scalems-0.0.1b1/tests/test_context_datastore.py
+-rw-r--r--   0 eric       (501) staff       (20)    12569 2022-12-15 15:31:32.000000 scalems-0.0.1b1/tests/test_datamodel.py
+-rw-r--r--   0 eric       (501) staff       (20)    10029 2023-04-25 15:55:46.000000 scalems-0.0.1b1/tests/test_filereference.py
+-rw-r--r--   0 eric       (501) staff       (20)      677 2022-12-15 15:31:32.000000 scalems-0.0.1b1/tests/test_messages.py
+-rw-r--r--   0 eric       (501) staff       (20)     5894 2023-03-31 10:56:59.000000 scalems-0.0.1b1/tests/test_radical_runtime.py
+-rw-r--r--   0 eric       (501) staff       (20)     3667 2023-04-25 15:56:02.000000 scalems-0.0.1b1/tests/test_raptor_utilities.py
+-rwxr-xr-x   0 eric       (501) staff       (20)    22121 2023-04-25 16:17:43.000000 scalems-0.0.1b1/tests/test_rp_exec.py
+-rwxr-xr-x   0 eric       (501) staff       (20)     4147 2023-03-27 14:14:03.000000 scalems-0.0.1b1/tests/test_rp_future.py
+-rwxr-xr-x   0 eric       (501) staff       (20)     9938 2023-03-27 11:39:58.000000 scalems-0.0.1b1/tests/test_rp_venv.py
+-rw-r--r--   0 eric       (501) staff       (20)     3057 2023-04-25 15:55:46.000000 scalems-0.0.1b1/tests/test_subprocess_exec.py
```

### Comparing `scalems-0.0.0a1/LICENSE` & `scalems-0.0.1b1/LICENSE`

 * *Files identical despite different names*

### Comparing `scalems-0.0.0a1/PKG-INFO` & `scalems-0.0.1b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scalems
-Version: 0.0.0a1
+Version: 0.0.1b1
 Summary: Reference implementation of the SCALE-MS data flow scripting and graph execution API for molecular science computational research protocols.
 Author-email: SCALE-MS team <info@scalems.org>
 License: LGPL 2.1
 Project-URL: Source, https://github.com/SCALE-MS/scale-ms/
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
```

### Comparing `scalems-0.0.0a1/README.md` & `scalems-0.0.1b1/README.md`

 * *Files identical despite different names*

### Comparing `scalems-0.0.0a1/pyproject.toml` & `scalems-0.0.1b1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -14,28 +14,28 @@
     "License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)",
     "Programming Language :: Python :: 3"
 ]
 dependencies = [
     "dill",
     "mpi4py",
     "packaging",
-    "radical.pilot >= 1.20"
+    "radical.pilot >= 1.22"
 ]
 
 [project.urls]
 "Source" = "https://github.com/SCALE-MS/scale-ms/"
 
 [project.optional-dependencies]
 test = [
     "build",
     "packaging",
     "pytest >= 6.1.2 ",
     "pytest-asyncio >= 0.14",
     "pytest-env",
-    "radical.pilot >= 1.20"
+    "radical.pilot >= 1.22"
 ]
 
 [project.scripts]
 scalems_rp_master = "scalems.radical.raptor:master"
 
 [tool.setuptools]
 zip-safe = false
@@ -45,15 +45,15 @@
 
 [tool.setuptools.package-data]
 scalems = [
     "py.typed"
 ]
 
 [tool.versioningit]
-default-version = "0+unknown"
+default-version = "0.0.1b1+unknown"
 
 [tool.versioningit.format]
 distance = "{base_version}+{distance}.{vcs}{rev}"
 dirty = "{base_version}+{distance}.{vcs}{rev}.dirty"
 distance-dirty = "{base_version}+{distance}.{vcs}{rev}.dirty"
 
 [tool.versioningit.vcs]
```

### Comparing `scalems-0.0.0a1/scalems.egg-info/PKG-INFO` & `scalems-0.0.1b1/scalems.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scalems
-Version: 0.0.0a1
+Version: 0.0.1b1
 Summary: Reference implementation of the SCALE-MS data flow scripting and graph execution API for molecular science computational research protocols.
 Author-email: SCALE-MS team <info@scalems.org>
 License: LGPL 2.1
 Project-URL: Source, https://github.com/SCALE-MS/scale-ms/
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
```

### Comparing `scalems-0.0.0a1/src/scalems/__init__.py` & `scalems-0.0.1b1/src/scalems/__init__.py`

 * *Files identical despite different names*

### Comparing `scalems-0.0.0a1/src/scalems/_types.py` & `scalems-0.0.1b1/src/scalems/_types.py`

 * *Files identical despite different names*

### Comparing `scalems-0.0.0a1/src/scalems/call/__init__.py` & `scalems-0.0.1b1/src/scalems/call/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 """Support command line execution of scalems packaged function calls.
 
 Example:
     python -m scalems.call record.json
 
 Note that this whole module is a workaround to avoid using RP raptor.
-We don't really need to reconcile the divergent notions of "Subprocess".
+:file:`scalems/call/__main__.py` provides command line behavior for a
+`radical.pilot.Task` *executable* and *arguments*, with which we execute a
+serialized representation of a function call, pending restoration of full
+"raptor" support.
+
+We don't really need to reconcile the divergent notions of "Subprocess",
+if we can remove the need for this entry point.
 But we _do_ need to formalize our serialized representation of a function call,
 and the task lifecycle and artifacts management.
 """
 __all__ = ("CallResult", "main", "cli", "serialize_call", "deserialize_result")
 
 import dataclasses
 import functools
@@ -221,15 +227,38 @@
     arguments: tuple[str, ...]
     requirements: dict = dataclasses.field(default_factory=dict)
 
 
 async def function_call_to_subprocess(
     func: typing.Callable, *, label: str, args: tuple = (), kwargs: dict = None, manager, requirements: dict = None
 ) -> _Subprocess:
-    """Wrap a function call in a command line based on `scalems.call`."""
+    """
+    Wrap a function call in a command line based on `scalems.call`.
+
+    Args:
+        func: A callable Python object.
+        label: Name (prefix) for identifying tasks and artifacts.
+        args: Positional arguments for *func*.
+        kwargs: Key word arguments for *func*.
+        manager: workflow manager instance.
+        requirements: run time requirements (passed through to execution backend).
+
+    Returns:
+        Serializable representation of the executable task.
+
+    Warnings:
+        This is a temporary utility while we explore use cases and prepare to migrate
+        back to :py:mod:`radical.pilot.raptor`. A user-facing tool should return a
+        view on a workflow item, whereas this function produces even lower-level details.
+
+    See Also:
+        * :py:func:`scalems.radical.runtime.subprocess_to_rp_task()`
+        * https://github.com/SCALE-MS/scale-ms/discussions/302
+
+    """
     if kwargs is None:
         kwargs = dict()
     if requirements is None:
         requirements = dict()
 
     # TODO: FileStore should probably provide a new_file() method.
     #   Possibly an overload to get_file_reference() for IOStreams or buffers,
@@ -257,14 +286,16 @@
         else:
             assert isinstance(value, str)
             arguments.append(f"-X{key}={value}")
 
     # TODO: Validate with argparse, once scalems.call.__main__ has a real parser.
     if "ranks" in requirements:
         arguments.extend(("-m", "mpi4py"))
+    # If this wrapper doesn't go away soon, we should abstract this so path arguments
+    # can be generated at the execution site.
     arguments.extend(("-m", "scalems.call", input_filename, output_filename))
 
     return _Subprocess(
         uid=uid,
         input_filenames={input_filename: file_ref},
         output_filenames=(output_filename,),
         executable=executable,
@@ -291,14 +322,15 @@
         logger.debug("Adding *exception* to outputs for internal use.")
         outputs.append("exception")
 
     # Note: we are already running inside a RP executable Task by the time we
     # reach this point, so we are relying on call.environment and call.skeleton
     # to have been handled by the caller.
     cwd = pathlib.Path(os.getcwd())
+    logger.info(f"scalems.call executing {func} in working directory {cwd}")
     result_fields = dict(directory=cwd.as_uri())
 
     # Note: For RP Raptor, the MPIWorker will be providing our wrapped function
     # with an mpi4py.MPI.Comm according to the task requirements. For this CLI
     # utility, RP will have used an appropriate launch method, so the parallelization
     # libraries should be able to initialize themselves from the environment.
     # TODO: Check that *e.g. gromacs* properly detects resources as prepared by RP.
@@ -314,15 +346,29 @@
     return result
 
 
 def cli(*argv: str):
     """Command line entry point.
 
     Invoke with ``python -m scalems.call <args>``
+
+    TODO: Configurable log level.
     """
+    logger.setLevel(logging.DEBUG)
+    character_stream = logging.StreamHandler()
+    character_stream.setLevel(logging.DEBUG)
+    formatter = logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s")
+    character_stream.setFormatter(formatter)
+    logger.addHandler(character_stream)
+
+    file_logger = logging.FileHandler("scalems.call.log")
+    file_logger.setLevel(logging.DEBUG)
+    file_logger.setFormatter(formatter)
+    logging.getLogger("scalems").addHandler(file_logger)
+
     logger.debug(f"scalems.call got args: {', '.join(str(arg) for arg in argv)}")
     # TODO: Consider an argparse parser for clarity.
     if len(argv) < 3:
         raise RuntimeError("Arguments are required.")
     # argv[0] will be the __main__.py script. Arguments to `call` are at argv[1:]
     call_path = pathlib.Path(argv[1])
     result_path = pathlib.Path(argv[2])
```

### Comparing `scalems-0.0.0a1/src/scalems/commands.py` & `scalems-0.0.1b1/src/scalems/commands.py`

 * *Files identical despite different names*

### Comparing `scalems-0.0.0a1/src/scalems/context/__init__.py` & `scalems-0.0.1b1/src/scalems/context/__init__.py`

 * *Files identical despite different names*

### Comparing `scalems-0.0.0a1/src/scalems/exceptions.py` & `scalems-0.0.1b1/src/scalems/exceptions.py`

 * *Files identical despite different names*

### Comparing `scalems-0.0.0a1/src/scalems/execution.py` & `scalems-0.0.1b1/src/scalems/execution.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,14 +89,15 @@
 
 import abc
 import asyncio
 import contextlib
 import logging
 import typing
 
+import scalems.exceptions
 from scalems.exceptions import APIError
 from scalems.exceptions import DispatchError
 from scalems.exceptions import InternalError
 from scalems.exceptions import MissingImplementationError
 from scalems.exceptions import ProtocolError
 from scalems.messages import QueueItem
 from scalems.store import FileStore
@@ -180,14 +181,16 @@
 
     A RuntimeManager is instantiated within the scope of the
     `scalems.workflow.WorkflowManager.dispatch` context manager using the
     :py:meth:`scalems.workflow.WorkflowManager._executor_factory`.
     """
 
     get_edit_item: typing.Callable[[], typing.Callable]
+    """Get the function that creates a WorkflowItem editing context."""
+
     datastore: FileStore
     submitted_tasks: typing.MutableSet[asyncio.Task]
 
     _runtime_configuration: _BackendT
 
     _command_queue: asyncio.Queue
     _dispatcher_lock: asyncio.Lock
@@ -231,15 +234,15 @@
 
         # TODO: Only hold a queue in an active context manager.
         self._command_queue = asyncio.Queue()
         self._exception = None
         self._loop: asyncio.AbstractEventLoop = loop
 
         if editor_factory is None or not callable(editor_factory):
-            raise TypeError("Provide a callable that produces an edit_item " "interface.")
+            raise TypeError("Provide a callable that produces an edit_item interface.")
         self.get_edit_item = editor_factory
 
         if datastore is None:
             raise TypeError("Provide a datastore.")
         self.datastore = datastore
 
         # TODO: Consider relying on module ContextVars and contextvars.Context scope.
@@ -249,14 +252,23 @@
             raise TypeError("An asyncio.Lock is required to control dispatcher state.")
         self._dispatcher_lock = dispatcher_lock
 
     def configuration(self) -> _BackendT:
         return self._runtime_configuration
 
     @staticmethod
+    async def cpi(command: str, runtime):
+        """Dispatcher for CPI messages.
+
+        TODO: Return value? We probably want to be able to capture something we can
+            query for the result of the CPI message.
+        """
+        logger.debug(f"Null CPI handler received command {command}.")
+
+    @staticmethod
     def runtime_shutdown(runtime):
         """Shutdown hook for runtime facilities.
 
         Called while exiting the context manager. Allows specialized handling of
         runtime backends in terms of the RuntimeManager instance and an abstract
         *Runtime* object, presumably acquired while entering the context manager
         through the *runtime_startup* hook.
@@ -482,14 +494,17 @@
         In a conservative first draft, we can simply throw an exception if
         a non-`async def` function attempts to call a scalems workflow command like
         "add_item" while in an executing context.)
 
     """
     queue = executor.queue()
     updater = executor.updater()
+    # Get a reference to the runtime, since it is removed from the executor before
+    # RuntimeManager.__aexit__() shuts down this task.
+    runtime = executor.runtime
 
     # Acknowledge that the coroutine is running and will immediately begin processing
     # queue items.
     processing_state.set()
     # Note that if an exception is raised here, the queue will never be processed.
 
     # Could also accept a "stop" Event object for the loop conditional,
@@ -509,46 +524,42 @@
     #         else:
     #             command: QueueItem = queue_getter.result()
     #         ...
     #         queue_getter = asyncio.create_task(command_queue.get())
     #         waiter = asyncio.create_task(asyncio(wait((signal_task, queue_getter),
     #         return_when=FIRST_COMPLETED))
     #
-    while True:
-        # Note: If the function exits at this line, the queue may be missing a call
-        #  to task_done() and should not be `join()`ed. It does not seem completely
-        #  clear whether the `get()` will have completed if the task for this function
-        #  is canceled or a Task.send() or Task.throw() is used. Alternatively, we could
-        #  include the `get()` in the `try` block and catch a possible ValueError at the
-        #  task_done() call, in case we arrive there without Queue.get() having completed.
-        #  However, that could allow a Queue.join() to complete early by accident.
-        command: QueueItem = await queue.get()
+    command: QueueItem
+    while command := await queue.get():
         # Developer note: The preceding line and the following try/finally block are
         # coupled!
         # Once we have awaited asyncio.Queue.get(), we _must_ have a corresponding
         # asyncio.Queue.task_done(). For tidiness, we immediately enter a `try` block
         # with a `finally` suite. Don't separate these without considering the Queue
         # protocol.
 
         try:
             if not len(command.items()) == 1:
                 raise ProtocolError("Expected a single key-value pair.")
             logger.debug(f"Processing command {repr(command)}")
 
-            # TODO: Use formal RPC protocol.
+            # TODO(#23): Use formal RPC protocol.
             if "control" in command:
+                logger.debug(f"Execution manager received {command['control']} command for {runtime}.")
+                try:
+                    await executor.cpi(command["control"], runtime)
+                except scalems.exceptions.ScopeError as e:
+                    logger.debug(
+                        f"Control command \"{command['control']}\" ignored due to inactive RuntimeManager.", exc_info=e
+                    )
+                    # We should probably break here, too, right?
+                    # TODO: Handle command results and take appropriate action on failures.
                 if command["control"] == "stop":
-                    logger.debug("Execution manager received stop command.")
-                    # This effectively breaks the `while True` loop, but may not be
-                    # obvious.
-                    # Consider explicit `break` to clarify that we want to run off the end
-                    # of the function.
-                    return
-                else:
-                    raise ProtocolError("Unknown command: {}".format(command["control"]))
+                    # End queue processing.
+                    break
             if "add_item" not in command:
                 # This will end queue processing. Tasks already submitted may still
                 # complete. Tasks subsequently added will update the static part of
                 # the workflow (WorkflowManager) and be eligible for dispatching in
                 # another dispatching session.
                 # If we need to begin to address the remaining queued items before
                 # this (the queue processor) task is awaited, we could insert a
@@ -570,15 +581,15 @@
                 # tasks.
 
                 # Bind the WorkflowManager item to an RP Task.
                 task = await updater.submit(item=item)
 
                 if task.done():
                     # Stop processing the queue if task was cancelled or errored.
-                    # TODO: Test this logical branch.
+                    # TODO: Test this logical branch or consider removing it.
                     if task.cancelled():
                         logger.info(f"Stopping queue processing after unexpected cancellation of task {task}")
                         return
                     else:
                         exc = task.exception()
                         if exc:
                             logger.error(f"Task {task} failed much to fast. Stopping execution.")
```

### Comparing `scalems-0.0.0a1/src/scalems/file/__init__.py` & `scalems-0.0.1b1/src/scalems/file/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 We distinguish between *File* and *FileReference* types.
 
 A *File* is a concrete representation of a local filesystem object.
 
 A *FileReference* is more general. It may represent a non-local object
 (accessible by a URI). We currently use *FileReference* objects exclusively for
 resources managed by scalems. (See `scalems.store.FileStore`.)
+
+This module has minimal dependencies on other scalems implementation details so
+that it can be included easily by scalems modules without circular dependencies.
 """
 
 __all__ = (
     "AbstractFileReference",
     "AbstractFile",
     "AccessFlags",
     "BaseBinary",
@@ -56,21 +59,23 @@
         handle: scalems.file.AbstractFileReference = filestore.add_file(...)
     """
 
     @abc.abstractmethod
     def __fspath__(self) -> str:
         """Represent the local filesystem path, if possible.
 
+        Support `os.PathLike`.
+
         Returns:
             str: representation of the filesystem path if the referenced file is
-            available locally.
+                available locally.
 
         Raises:
             DataLocalizationError: if the file has not been transferred to the local
-            file store.
+                file store.
         """
         raise NotImplementedError
 
     @abc.abstractmethod
     def is_local(self, context=None) -> bool:
         """Check for file existence in a given context.
```

### Comparing `scalems-0.0.0a1/src/scalems/identifiers.py` & `scalems-0.0.1b1/src/scalems/identifiers.py`

 * *Files identical despite different names*

### Comparing `scalems-0.0.0a1/src/scalems/invocation.py` & `scalems-0.0.1b1/src/scalems/invocation.py`

 * *Files 3% similar despite different names*

```diff
@@ -253,19 +253,15 @@
                 exitcode = 1
         if exitcode != 0:
             raise SystemExit(exitcode)
     finally:
         _reentrance_guard.release()
 
 
-# TODO(Python 3.9): Use functools.cache instead of lru_cache when Py 3.9 is required.
-_cache = getattr(functools, "cache", functools.lru_cache(maxsize=None))
-
-
-@_cache
+@functools.cache
 def base_parser(add_help=False):
     """Get the base scalems argument parser.
 
     Provides a base argument parser for scripts or other module parsers.
 
     By default, the returned ArgumentParser is created with ``add_help=False``
     to avoid conflicts when used as a *parent* for a parser more local to the caller.
```

### Comparing `scalems-0.0.0a1/src/scalems/local/__init__.py` & `scalems-0.0.1b1/src/scalems/local/__init__.py`

 * *Files identical despite different names*

### Comparing `scalems-0.0.0a1/src/scalems/local/operations.py` & `scalems-0.0.1b1/src/scalems/local/operations.py`

 * *Files identical despite different names*

### Comparing `scalems-0.0.0a1/src/scalems/logger.py` & `scalems-0.0.1b1/src/scalems/logger.py`

 * *Files identical despite different names*

### Comparing `scalems-0.0.0a1/src/scalems/messages.py` & `scalems-0.0.1b1/src/scalems/messages.py`

 * *Files identical despite different names*

### Comparing `scalems-0.0.0a1/src/scalems/radical/__init__.py` & `scalems-0.0.1b1/src/scalems/radical/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -33,31 +33,24 @@
 """
 # TODO: Consider converting to a namespace package to improve modularity of
 #  implementation.
 
 __all__ = ["configuration", "parser", "workflow_manager"]
 
 import asyncio
-import functools
 import logging
 
 import scalems.workflow
 from ..invocation import make_parser as _make_parser
 from .runtime import configuration
 from .runtime import parser as _runtime_parser
 
 logger = logging.getLogger(__name__)
 logger.debug("Importing {}".format(__name__))
 
-try:
-    cache = functools.cache
-except AttributeError:
-    # Note: functools.cache does not appear until Python 3.9
-    cache = functools.lru_cache(maxsize=None)
-
 parser = _make_parser(__package__, parents=[_runtime_parser()])
 
 
 def workflow_manager(loop: asyncio.AbstractEventLoop, directory=None):
     """Manage a workflow context for RADICAL Pilot work loads.
 
     The rp.Session is created when the Python Context Manager is "entered",
```

### Comparing `scalems-0.0.0a1/src/scalems/radical/raptor/__init__.py` & `scalems-0.0.1b1/src/scalems/radical/raptor/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -256,15 +256,15 @@
     "master",
     "worker_requirements",
     "worker_description",
     "SoftwareCompatibilityError",
     "ScaleMSWorker",
     "ScaleMSMaster",
     "ScalemsRaptorWorkItem",
-    "WorkerDescriptionDict",
+    "WorkerDescription",
     "RaptorWorkerConfig",
 )
 
 import abc
 import argparse
 import asyncio
 import contextlib
@@ -278,37 +278,33 @@
 import tempfile
 import typing
 import warnings
 import weakref
 import zlib
 from importlib.machinery import ModuleSpec
 from importlib.util import find_spec
-
-try:
-    from mpi4py.MPI import Comm
-except ImportError:
-    Comm = None
-
-# TODO(Python 3.9): Remove this conditional when we require Python >= 3.9
-if sys.version_info.minor < 9:
-    from typing import Generator
-else:
-    from collections.abc import Generator
+from collections.abc import Generator
 
 import packaging.version
 
+if typing.TYPE_CHECKING:
+    try:
+        from mpi4py.MPI import Comm
+    except ImportError:
+        Comm = None
+
+
 # We import rp before `logging` to avoid warnings when rp monkey-patches the
 # logging module. This `try` suite helps prevent auto-code-formatters from
 # rearranging the import order of built-in versus third-party modules.
 try:
     import radical.pilot as rp
 except (ImportError,):
     warnings.warn("RADICAL Pilot installation not found.")
 
-import scalems.compat
 import scalems.exceptions
 import scalems.radical
 import scalems.messages
 import scalems.file as _file
 import scalems.store as _store
 
 # QUESTION: How should we approach logging? To what degree can/should we integrate
@@ -323,22 +319,16 @@
 # but only to the Master itself for the worker task.
 # We should probably either add a specific LogHandler or integrate with the
 # RP logging and Component based log files.
 # See also
 # * https://github.com/SCALE-MS/scale-ms/discussions/261
 # * https://github.com/SCALE-MS/scale-ms/issues/255
 
-try:
-    cache = functools.cache
-except AttributeError:
-    # Note: functools.cache does not appear until Python 3.9
-    cache = functools.lru_cache(maxsize=None)
-
 
-@dataclasses.dataclass
+@dataclasses.dataclass(frozen=True)
 class BackendVersion:
     """Identifying information for the computing backend."""
 
     name: str
     """Identifying name (presumably a module name)."""
 
     version: str
@@ -403,14 +393,15 @@
     @classmethod
     def command_class(cls) -> str:
         return scalems.messages.StopCommand.__qualname__
 
     @classmethod
     def launch(cls, manager: ScaleMSMaster, task: TaskDictionary):
         logger.debug("CPI STOP issued.")
+        # TODO: Wait for pending tasks to complete and shut down Worker(s)
         task["stderr"] = ""
         task["stdout"] = ""
         task["exit_code"] = 0
         manager.cpi_finalize(task)
 
     @classmethod
     def result_hook(cls, manager: ScaleMSMaster, task: TaskDictionary):
@@ -423,14 +414,15 @@
 
     @classmethod
     def launch(cls, manager: ScaleMSMaster, task: TaskDictionary):
         logger.debug("CPI HELLO in progress.")
         task["stderr"] = ""
         task["exit_code"] = 0
         task["stdout"] = repr(backend_version)
+        # TODO: scalems object encoding.
         task["return_value"] = dataclasses.asdict(backend_version)
         logger.debug("Finalizing...")
         manager.cpi_finalize(task)
 
     @classmethod
     def result_hook(cls, manager: ScaleMSMaster, task: TaskDictionary):
         logger.debug(f"Finalized {str(task)}.")
@@ -515,16 +507,19 @@
                 metadata=None,
                 mode=rp.TASK_FUNCTION,
                 function="run_in_worker",
                 args=[],
                 kwargs={"work_item": work_item},
             )
         )
-        scalems_task = manager.submit_tasks(scalems_task_description)
-        logger.debug(f"Submitted {str(scalems_task)} in support of {str(task)}.")
+        # Note: There is no `Task` object returned from `Master.submit_tasks()`
+        # `Task` objects are currently only available on the client side;
+        # the agent side handles task dicts---which the master will receive through the *request_cb()*.
+        manager.submit_tasks(scalems_task_description)
+        logger.debug(f"Submitted {str(scalems_task_description)} in support of {str(task)}.")
 
         # Record task metadata and track.
         task["return_value"] = scalems_task_id
         task["stdout"] = scalems_task_id
         task["exit_code"] = 0
         manager.cpi_finalize(task)
 
@@ -565,27 +560,46 @@
 
 
 # @object_encoder.register
 # def _(obj: rp.TaskDescription) -> dict:
 #     return obj.as_dict()
 
 
-@dataclasses.dataclass
+@dataclasses.dataclass(frozen=True)
 class ClientWorkerRequirements:
     """Client-side details to inform worker provisioning.
 
     This structure is part of the `scalems.radical.raptor.MasterTaskConfiguration`
     provided to the master script. The master script uses this information
     when calling `worker_description()`.
+
+    Use the :py:func:`worker_requirements()` creation function for a stable interface.
     """
 
-    named_env: str
-    pre_exec: typing.Iterable[str] = ()
-    cpu_processes: int = None
-    gpus_per_process: int = None
+    cpu_processes: int
+    """Number of ranks in the Worker MPI context.
+
+    TODO: We need to account for cores-per-process.
+    """
+
+    gpus_per_process: int = 0
+    """GPUs per Worker rank.
+
+    TODO: Reconcile with upcoming support for fractional ratios.
+    """
+
+    pre_exec: tuple[str] = ()
+    """Lines of shell expressions to be evaluated before launching the worker process."""
+
+    named_env: str = None
+    """A registered virtual environment known to the raptor manager.
+
+    Warnings:
+        Not tested. Support has been delayed indefinitely.
+    """
 
 
 class _MasterTaskConfigurationDict(typing.TypedDict):
     """A `MasterTaskConfiguration` encoded as a `dict`."""
 
     worker: dict  # dict-encoded ClientWorkerRequirements.
     versioned_modules: typing.List[typing.Tuple[str, str]]
@@ -622,15 +636,15 @@
 
 
 @object_encoder.register
 def _(obj: MasterTaskConfiguration) -> dict:
     return dataclasses.asdict(obj)
 
 
-@cache
+@functools.cache
 def master_script() -> str:
     """Get the name of the RP raptor master script.
 
     The script to run a RP Task based on a rp.raptor.Master is installed
     with :py:mod`scalems`. Installation configures an "entry point" script
     named ``scalems_rp_master``, but for generality this function should
     be used to get the entry point name.
@@ -706,36 +720,43 @@
         await asyncio.wait((add_file_task,), return_when=asyncio.FIRST_EXCEPTION)
         assert add_file_task.done()
         try:
             tmpdir_manager.cleanup()
         except OSError:
             logger.exception(f"Errors occurred while cleaning up {tmpdir}.")
     if isinstance(add_file_task.exception(), scalems.exceptions.DuplicateKeyError):
-        checksum = await scalems.compat.get_to_thread()(file_description.fingerprint)
+        checksum = await asyncio.to_thread(file_description.fingerprint)
         key = checksum.hex()
         # Note: the DuplicateKeyError could theoretically be the result of a
         # pre-existing file with the same internal path but a different key, but
         # such a condition would probably represent an internal error (bug).
+        # TODO: Migrate away from container behavior of FileStore.
         return filestore[key]
     else:
         return add_file_task.result()
 
 
-def worker_requirements(*, pre_exec: list, worker_venv: str) -> ClientWorkerRequirements:
-    """Get the requirements for the work load as known to the client.
+def worker_requirements(*, pre_exec: typing.Iterable[str], worker_venv: str) -> ClientWorkerRequirements:
+    """Get the requirements for the work load, as known to the client.
 
     TODO: Inspect workflow to optimize reusability of the initial Worker submission.
     """
-    # num_workers = 1
+    # TODO: calculate cores.
+    # rp_config = scalems.radical.configuration()
+    # pilot_description = rp_config.rp_resource_params["PilotDescription"]
+    # available_cores = pilot_description.get("cores")
+    # if not available_cores:
+    #     cores_per_node =
+    #     ...
     cores_per_worker = 1
     gpus_per_worker = 0
 
     workload_metadata = ClientWorkerRequirements(
         named_env=worker_venv,
-        pre_exec=pre_exec,
+        pre_exec=tuple(pre_exec),
         cpu_processes=cores_per_worker,
         gpus_per_process=gpus_per_worker,
     )
 
     return workload_metadata
 
 
@@ -851,46 +872,38 @@
 
     _master = ScaleMSMaster(configuration)
     logger.debug(f"Created {repr(_master)}.")
 
     requirements = configuration.worker
 
     try:
-        with _master.configure_worker(requirements=requirements) as worker_submission:
-            assert os.path.isabs(worker_submission["descr"]["worker_file"])
-            assert os.path.exists(worker_submission["descr"]["worker_file"])
-            logger.debug(f"Submitting {worker_submission['count']} {worker_submission['descr']}")
-            _master.submit_workers(**worker_submission)
+        with _master.configure_worker(requirements=requirements) as configs:
+            assert len(configs) == 1
+            worker_submission: rp.TaskDescription = configs[0]
+            assert os.path.isabs(worker_submission.raptor_file)
+            assert os.path.exists(worker_submission.raptor_file)
+            logger.debug(f"Submitting {len(configs)} {worker_submission.as_dict()}")
+            _master.submit_workers(descriptions=configs)
             message = "Submitted workers: "
             message += ", ".join(_master.workers.keys())
             logger.info(message)
 
             _master.start()
             logger.debug("Master started.")
 
-            if rp_version >= packaging.version.parse("1.21"):
-                # Make sure at least one worker comes online.
-                _master.wait(count=1)
-                logger.debug("Ready to submit raptor tasks.")
-                # Confirm all workers start successfully or produce useful error
-                #  (then release temporary file).
-                _master.wait()
-            for uid, worker in _master.workers.items():
-                logger.info(f"Worker {uid} in state {worker['status']}.")
-            # TODO(#253): Confirm that workers started successfully and notify client
-            # See also https://github.com/radical-cybertools/radical.pilot/issues/2643
-            # relevant worker states _master.workers['uid']['status']
-            # * 'NEW' -> 'ACTIVE' -> 'DONE'
-            # Note: Until we integrate with ZMQ, there is not a good mechanism to provide feedback
-            # to the client that the raptor session is active, but we could add some sort of status
-            # check to the CPI.
-            # TODO(#253): Confirm workers start successfully or produce useful error, then release temporary file.
-            # Until then, we can't safely exit this `with` block until after `join`.
-            _master.join()
-            logger.debug("Master joined.")
+            # Make sure at least one worker comes online.
+            _master.wait_workers(count=1)
+            logger.debug("Ready to submit raptor tasks.")
+            # Confirm all workers start successfully or produce useful error
+            #  (then release temporary file).
+            _master.wait_workers()
+        for uid, worker in _master.workers.items():
+            logger.info(f"Worker {uid} in state {worker['status']}.")
+        _master.join()
+        logger.debug("Master joined.")
     finally:
         if sys.exc_info() != (None, None, None):
             logger.exception("Master task encountered exception.")
         logger.debug("Completed master task.")
 
 
 def _configure_worker(*, requirements: ClientWorkerRequirements, filename: str) -> RaptorWorkerConfig:
@@ -899,25 +912,25 @@
     Provide an abstraction for the submit_workers signature and parameter types,
     which may still be evolving.
 
     See also https://github.com/radical-cybertools/radical.pilot/issues/2731
     """
     assert os.path.exists(filename)
     # TODO(#248): Consider a "debug-mode" option to do a trial import from *filename*
+    # TODO(#302): Number of workers should be chosen after inspecting the requirements of the work load.
     num_workers = 1
-    kwargs = dict(
+    descr = worker_description(
         named_env=requirements.named_env,
         worker_file=filename,
         pre_exec=requirements.pre_exec,
         cpu_processes=requirements.cpu_processes,
         gpus_per_process=requirements.gpus_per_process,
     )
-    descr = worker_description(**kwargs)
 
-    config = RaptorWorkerConfig(count=num_workers, descr=descr)
+    config: RaptorWorkerConfig = [descr] * num_workers
     return config
 
 
 class SoftwareCompatibilityError(RuntimeError):
     """Incompatible package versions or software interfaces."""
 
 
@@ -1194,14 +1207,15 @@
     def _scalems_handle_requests(self, tasks: typing.Sequence[TaskDictionary]):
         for task in tasks:
             _finalized = False
             try:
                 mode = task["description"]["mode"]
                 # Allow non-scalems work to be handled normally.
                 if mode != CPI_MESSAGE:
+                    logger.debug(f"Deferring {str(task)} to regular RP handling.")
                     yield task
                     continue
                 else:
                     command = scalems.messages.Command.decode(task["description"]["metadata"])
                     logger.debug(f"Received message {command} in {str(task)}")
 
                     impl: typing.Type[CpiCommand] = CpiCommand.get(command)
@@ -1237,14 +1251,15 @@
 
         We perform special handling for two types of tasks.
         1. Tasks submitted throughcompleted by the collaborating Worker(s).
         2. Tasks intercepted and resolved entirely by the Master (CPI calls).
         """
         # Note: At least as of RP 1.18, exceptions from result_cb() are suppressed.
         for task in tasks:
+            logger.debug(f'Result callback for {task["description"]["mode"]} task {task["uid"]}: {task}')
             mode = task["description"]["mode"]
             # Allow non-scalems work to be handled normally.
             if mode == CPI_MESSAGE:
                 command = scalems.messages.Command.decode(task["description"]["metadata"])
                 logger.debug(f"Finalizing {command} in {str(task)}")
 
                 impl: typing.Type[CpiCommand] = CpiCommand.get(command)
@@ -1283,69 +1298,56 @@
             #     for req in self._workload:
             #         # TODO: create raptor method
             #         req['task']['target_state'] = rp.DONE
             #         self.advance(req['task'], rp.AGENT_STAGING_OUTPUT_PENDING,
             #                      publish=True, push=True)
 
 
-class WorkerDescriptionDict(typing.TypedDict):
+class WorkerDescription(rp.TaskDescription):
     """Worker description.
 
     See Also:
         * :py:meth:`~radical.pilot.raptor.Master.submit_workers()`
         * https://github.com/radical-cybertools/radical.pilot/issues/2731
 
     """
 
     cores_per_rank: typing.Optional[int]
-    environment: typing.Optional[dict]
+    environment: typing.Optional[dict[str, str]]
     gpus_per_rank: typing.Optional[int]
     named_env: typing.Optional[str]
-    pre_exec: typing.Optional[list]
+    pre_exec: typing.Optional[list[str]]
     ranks: int
-    worker_class: typing.Optional[str]
-    worker_file: typing.Optional[str]
-
-
-class RaptorWorkerConfig(typing.TypedDict):
-    """Container for the raptor worker parameters.
+    raptor_class: str
+    raptor_file: str
+    mode: str  # rp.RAPTOR_WORKER
 
-    Expanded with the ``**`` operator, serves as the arguments to
-    :py:meth:`radical.pilot.raptor.Master.submit_workers`
 
-    The *descr* member represents the *descr* parameter of
-    :py:meth:`~radical.pilot.raptor.Master.submit_workers()`,
-    pending further documentation.
+RaptorWorkerConfig = list[WorkerDescription]
+"""Client-specified Worker requirements.
 
-    Created internally with :py:func:`_configure_worker()`.
-    """
-
-    descr: WorkerDescriptionDict
-    """Client-specified Worker requirements.
+Used by master script when calling `worker_description()`.
+Created internally with :py:func:`_configure_worker()`.
 
-    Used by master script when calling `worker_description()`.
+See Also:
+    :py:mod:`scalems.radical.raptor.ClientWorkerRequirements`
 
-    See Also:
-        :py:mod:`scalems.radical.raptor.ClientWorkerRequirements`
-    """
-
-    count: typing.Optional[int]
-    """Number of workers to launch."""
+"""
 
 
 def worker_description(
     *,
     named_env: str,
     worker_file: str,
     cores_per_process: int = None,
     cpu_processes: int = None,
     gpus_per_process: int = None,
     pre_exec: typing.Iterable[str] = (),
     environment: typing.Optional[typing.Mapping[str, str]] = None,
-) -> WorkerDescriptionDict:
+) -> WorkerDescription:
     """Get a worker description for Master.submit_workers().
 
     Parameters:
         cores_per_process (int, optional): See `radical.pilot.TaskDescription.cores_per_rank`
         cpu_processes (int, optional): See `radical.pilot.TaskDescription.ranks`
         environment (dict, optional): Environment variables to set in the Worker task.
         gpus_per_process (int, optional): See `radical.pilot.TaskDescription.gpus_per_rank`
@@ -1355,27 +1357,30 @@
         worker_file (str): Standalone module from which to import ScaleMSWorker.
 
     *worker_file* is generated for the master script by the caller.
     See :py:mod:`scalems.radical.raptor`
 
     The *uid* for the Worker task is defined by the Master.submit_workers().
     """
-    kwargs = dict(
-        cores_per_rank=cores_per_process,
-        environment=environment,
-        gpus_per_rank=gpus_per_process,
-        named_env=None,
-        pre_exec=list(pre_exec),
-        ranks=cpu_processes,
-        worker_class="ScaleMSWorker",
-        worker_file=worker_file,
-    )
-    # Avoid assumption about how default values in TaskDescription are checked or applied.
-    kwargs = {key: value for key, value in kwargs.items() if value is not None}
-    descr = WorkerDescriptionDict(**kwargs)
+    descr = WorkerDescription()
+    if cores_per_process is not None:
+        descr.cores_per_rank = cores_per_process
+    if environment is not None:
+        descr.environment = environment
+    if gpus_per_process is not None:
+        descr.gpus_per_rank = gpus_per_process
+    if named_env is not None:
+        # descr.named_env=None
+        logger.debug(f"Ignoring named_env={named_env}. Parameter is currently unused.")
+    descr.pre_exec = list(pre_exec)
+    if cpu_processes is not None:
+        descr.ranks = cpu_processes
+    descr.raptor_class = "ScaleMSWorker"
+    descr.raptor_file = worker_file
+    descr.mode = rp.RAPTOR_WORKER
     return descr
 
 
 class RaptorTaskExecutor(typing.Protocol):
     """Represent the signature of executor functions for rp.raptor.MPIWorker."""
 
     def __call__(self, *args, comm: Comm, **kwargs) -> Encodable:
```

### Comparing `scalems-0.0.0a1/src/scalems/radical/runtime.py` & `scalems-0.0.1b1/src/scalems/radical/runtime.py`

 * *Files 3% similar despite different names*

```diff
@@ -158,19 +158,19 @@
 
 import packaging.version
 import radical.saga
 import radical.utils
 from radical import pilot as rp
 
 import scalems.call
-import scalems.compat
 import scalems.exceptions
 import scalems.execution
 import scalems.file
 import scalems.invocation
+import scalems.messages
 import scalems.radical
 import scalems.radical.raptor
 import scalems.store
 import scalems.subprocess
 import scalems.workflow
 from scalems.exceptions import APIError
 from scalems.exceptions import DispatchError
@@ -190,30 +190,32 @@
 logger.debug("Importing {}".format(__name__))
 
 # TODO: Consider scoping for these context variables.
 # Need to review PEP-567 and PEP-568 to consider where and how to scope the Context
 # with respect to the dispatching scope.
 _configuration = contextvars.ContextVar("_configuration")
 
-try:
-    cache = functools.cache
-except AttributeError:
-    # Note: functools.cache does not appear until Python 3.9
-    cache = functools.lru_cache(maxsize=None)
+
+if typing.TYPE_CHECKING:
+    import radical.utils as ru
 
 
 def _parse_option(arg: str) -> tuple:
     if not isinstance(arg, str):
         raise InternalError("Bug: This function should only be called with a str.")
     if arg.count("=") != 1:
         raise argparse.ArgumentTypeError('Expected a key/value pair delimited by "=".')
     return tuple(arg.split("="))
 
 
-@cache
+class RPConfigurationError(ScaleMSError):
+    """Unusable RADICAL Pilot configuration."""
+
+
+@functools.cache
 def parser(add_help=False):
     """Get the module-specific argument parser.
 
     Provides a base argument parser for scripts using the scalems.radical backend.
 
     By default, the returned ArgumentParser is created with ``add_help=False``
     to avoid conflicts when used as a *parent* for a parser more local to the caller.
@@ -285,63 +287,104 @@
     .. todo:: Consider merging with module Runtime state container.
 
     """
 
     # Note that the use cases for this dataclass interact with module ContextVars,
     # pending refinement.
     datastore: FileStore = None
-    # TODO: Check that the resource is defined.
     execution_target: str = "local.localhost"
     rp_resource_params: dict = dataclasses.field(default_factory=dict)
     target_venv: str = None
     enable_raptor: bool = False
 
+    def __post_init__(self):
+        hpc_platform_label = self.execution_target
+        access = self.rp_resource_params["PilotDescription"].get("access_schema")
+        try:
+            job_endpoint: ru.Url = rp.utils.misc.get_resource_job_url(hpc_platform_label, schema=access)
+        except (TypeError, KeyError) as e:
+            raise RPConfigurationError(f"Could not resolve {access} access for {hpc_platform_label}") from e
+
+        if self.enable_raptor:
+            # scalems uses the RP MPIWorker, which can have problems in "local" execution modes.
+            launch_scheme = job_endpoint.scheme
+            if launch_scheme == "fork":
+                message = f"RP Raptor MPI Worker not supported for '{launch_scheme}' launch method."
+                message += f" '{access}' access for {hpc_platform_label}: {job_endpoint}"
+                raise RPConfigurationError(message)
+
 
 class Runtime:
     """Container for scalems.radical runtime state data.
 
     Note:
         This class is almost exclusively a container. Lifetime management is assumed
         to be handled externally.
 
-    .. todo:: Consider either merging with `scalems.radical.runtime.Configuration` or
-        explicitly encapsulating the responsibilities of `RPDispatchingExecutor.runtime_startup()`
+    .. todo:: Let `scalems.radical.runtime.Configuration` holds the run time invariant.
+        And let this become more than a container, explicitly encapsulating
+        the responsibilities of `RPDispatchingExecutor.runtime_startup()`
         and `RPDispatchingExecutor.runtime_shutdown()`.
 
     See Also:
         :py:attr:`scalems.radical.runtime.RPDispatchingExecutor.runtime`
 
     """
 
     _session: rp.Session
+
     scheduler: typing.Optional[rp.Task] = None
+    """The active raptor scheduler task, if any."""
+
+    resources: typing.Optional[asyncio.Task[dict]] = None
+    """The active Pilot resources, if any.
+
+    The runtime_startup routine schedules a Task to get a copy of
+    the Pilot.resource_details['rm_info'] dictionary, once the Pilot
+    reaches state PMGR_ACTIVE.
+    """
 
     _pilot_manager: typing.Optional[rp.PilotManager] = None
     _pilot: typing.Optional[rp.Pilot] = None
     _task_manager: typing.Optional[rp.TaskManager] = None
 
     def __init__(self, session: rp.Session):
         if not isinstance(session, rp.Session) or session.closed:
             raise ValueError("*session* must be an active RADICAL Pilot Session.")
         self._session = session
 
+    def __repr__(self):
+        if session := self._session:
+            session = session.uid
+        if pilot := self._pilot:
+            pilot = pilot.uid
+        if scheduler := self.scheduler:
+            scheduler = scheduler.uid
+        representation = f'<Runtime session:"{session}" pilot:"{pilot}" raptor:"{scheduler}">'
+        return representation
+
     def reset(self, session: rp.Session):
         """Reset the runtime state.
 
         Close any existing resources and revert to a new Runtime state containing only
         the provided *session*.
         """
         if not isinstance(session, rp.Session) or session.closed:
             raise ValueError("*session* must be an active RADICAL Pilot Session.")
+        if self.resources is not None:
+            self.resources.cancel()
+            self.resources = None
         self._session.close()
         # Warning: This is not quite right.
         # The attribute values are deferred to the class dict from initialization. The
         # following lines actually leave the instance members in place with None values
         # rather than removing them, but the logic of checking for and removing the
         # instance values seems a little harder to read.
+        # TODO: Properly close previous session. This includes sending a "stop" to the
+        #     raptor scheduler instead of letting it get a `Task.cancel()` (i.e. a SIGTERM).
         self.scheduler = None
         self._pilot = None
         self._task_manager = None
         self._pilot_manager = None
         self._session = session
 
     @property
@@ -569,28 +612,26 @@
             "action": rp.TRANSFER,
         }
     ]
     td.arguments.append(config_file_name)
 
     task_metadata = {"uid": td.uid, "task_manager": task_manager.uid}
 
-    to_thread = scalems.compat.get_to_thread()
-
-    await asyncio.create_task(to_thread(filestore.add_task, master_identity, **task_metadata), name="add-task")
+    await asyncio.create_task(asyncio.to_thread(filestore.add_task, master_identity, **task_metadata), name="add-task")
     # filestore.add_task(master_identity, **task_metadata)
 
     logger.debug(f"Launching RP raptor scheduling. Submitting {td}.")
 
-    _task = asyncio.create_task(to_thread(task_manager.submit_tasks, td), name="submit-Master")
+    _task = asyncio.create_task(asyncio.to_thread(task_manager.submit_tasks, td), name="submit-Master")
     scheduler: rp.Task = await _task
 
     # WARNING: rp.Task.wait() *state* parameter does not handle tuples, but does not
     # check type.
     _task = asyncio.create_task(
-        to_thread(scheduler.wait, state=[rp.states.AGENT_EXECUTING] + rp.FINAL),
+        asyncio.to_thread(scheduler.wait, state=[rp.states.AGENT_EXECUTING] + rp.FINAL),
         name="check-Master-started",
     )
     await _task
     logger.debug(f"Scheduler in state {scheduler.state}.")
     # TODO: Generalize the exit status checker for the Master task and perform this
     #  this check at the call site.
     if scheduler.state in rp.FINAL:
@@ -599,15 +640,15 @@
             logger.error(f"scheduler.stderr: {scheduler.stderr}")
         raise DispatchError(f"Master Task unexpectedly reached {scheduler.state} during launch.")
     return scheduler
 
 
 # functools can't cache this function while Configuration is unhashable (due to
 # unhashable dict member).
-# @cache
+# @functools.cache
 def get_pre_exec(conf: Configuration) -> tuple:
     """Get the sequence of pre_exec commands for tasks on the currently configured execution target.
 
     Warning:
         Use cases may require a `list` object. Caller is responsible for converting
         the returned tuple if appropriate.
 
@@ -686,16 +727,14 @@
 async def new_session():
     """Start a new RADICAL Pilot Session.
 
     Returns:
         Runtime instance.
 
     """
-    to_thread = scalems.compat.get_to_thread()
-
     # Note that we cannot resolve the full _resource config until we have a Session
     # object.
     # We cannot get the default session config until after creating the Session,
     # so we don't have a template for allowed, required, or default values.
     # Question: does the provided *cfg* need to be complete? Or will it be merged
     # with default values from some internal definition, such as by dict.update()?
     # I don't remember what the use cases are for overriding the default session
@@ -708,15 +747,15 @@
     # Note: radical.pilot.Session creation causes several deprecation warnings.
     # Ref https://github.com/radical-cybertools/radical.pilot/issues/2185
     with warnings.catch_warnings():
         warnings.simplefilter("ignore", category=DeprecationWarning)
         # This would be a good time to `await`, if an event-loop friendly
         # Session creation function becomes available.
         session_args = dict(uid=session_id, cfg=session_config)
-        _task = asyncio.create_task(to_thread(rp.Session, (), **session_args), name="create-Session")
+        _task = asyncio.create_task(asyncio.to_thread(rp.Session, (), **session_args), name="create-Session")
         session = await _task
         runtime = Runtime(session=session)
     return runtime
 
 
 @functools.singledispatch
 def normalize(hint: object, value):
@@ -814,37 +853,62 @@
     task_manager = runtime.task_manager()
     if not pilot_manager or not task_manager:
         raise ProtocolError(f"Runtime {runtime} is not ready to use.")
 
     # Note: Consider fetching through the Runtime instance.
     config: Configuration = configuration()
 
-    to_thread = scalems.compat.get_to_thread()
-
     # Warning: The Pilot ID needs to be unique within the Session.
     pilot_description = {"uid": f"pilot.{str(uuid.uuid4())}"}
     pilot_description.update(config.rp_resource_params.get("PilotDescription", {}))
     pilot_description.update({"resource": config.execution_target})
 
     # TODO: Pilot venv (#90, #94).
     # Currently, Pilot venv must be specified in the JSON file for resource
     # definitions.
     pilot_description = rp.PilotDescription(pilot_description)
     logger.debug("Submitting PilotDescription {}".format(repr(pilot_description.as_dict())))
     pilot: rp.Pilot = await asyncio.create_task(
-        to_thread(pilot_manager.submit_pilots, pilot_description), name="submit_pilots"
+        asyncio.to_thread(pilot_manager.submit_pilots, pilot_description), name="submit_pilots"
     )
     logger.debug(f"Got Pilot {pilot.uid}: {pilot.as_dict()}")
     runtime.pilot(pilot)
 
-    await asyncio.create_task(to_thread(task_manager.add_pilots, pilot), name="add_pilots")
+    await asyncio.create_task(asyncio.to_thread(task_manager.add_pilots, pilot), name="add_pilots")
 
     return pilot
 
 
+async def get_pilot_resources(pilot: rp.Pilot):
+    def log_pilot_state(fut: asyncio.Task[str]):
+        # Task callbacks do not get called for cancelled Tasks.
+        assert not fut.cancelled()
+        if e := fut.exception():
+            logger.exception("Exception while watching for Pilot to become active.", exc_info=e)
+        logger.info(f"Pilot {pilot.uid} in state {pilot.state}.")
+
+    logger.info("Waiting for an active Pilot.")
+    # Wait for Pilot to be in state PMGR_ACTIVE. (There is no reasonable
+    # choice of a timeout because we are waiting for the HPC queuing system.)
+    # Then, query Pilot.resource_details['rm_info']['requested_cores'] and 'requested_gpus'.
+    pilot_state = asyncio.create_task(
+        asyncio.to_thread(pilot.wait, state=rp.PMGR_ACTIVE, timeout=None), name="pilot_state_waiter"
+    )
+
+    pilot_state.add_done_callback(log_pilot_state)
+    await pilot_state
+    rm_info: dict = pilot.resource_details.get("rm_info")
+    logger.debug(f"Pilot {pilot.uid} resources: {str(rm_info)}")
+    if rm_info is not None:
+        assert isinstance(rm_info, dict)
+        assert "requested_cores" in rm_info and isinstance(rm_info["requested_cores"], int)
+        assert "requested_gpus" in rm_info and isinstance(rm_info["requested_gpus"], typing.SupportsFloat)
+        return rm_info.copy()
+
+
 class RPDispatchingExecutor(RuntimeManager):
     """Client side manager for work dispatched through RADICAL Pilot.
 
     Configuration points:
 
     * resource config
     * pilot config
@@ -963,14 +1027,26 @@
             async with instance:
                 ...
 
         Raises:
             DispatchError: if task dispatching could not be set up.
             asyncio.CancelledError: if parent `asyncio.Task` is cancelled while executing.
 
+        TODO: More concurrency.
+            The rp.Pilot and raptor task can be separately awaited, and we should allow
+            input data staging to begin as soon as we have enough run time details to do it.
+            We need to clarify which tasks should be in which state to consider the
+            asynchronous context manager to have been successfully "entered". I expect
+            that success includes a Pilot in state PMGR_ACTIVE, and a raptor Task in
+            state AGENT_EXECUTING, and asyncio.Task handles available for other aspects,
+            like synchronization of metadata and initiation of input data staging.
+            However, we may prefer that the workflow script can continue evaluation on
+            the client side while waiting for the Pilot job, and that we avoid blocking
+            until we absolutely have to (presumably when exiting the dispatching context).
+
         """
         config: Configuration = configuration()
 
         # TODO: Check that we have a FileStore.
 
         # We try to wrap rp UI calls in separate threads. Note, though, that
         #   * The rp.Session needs to be created in the root thread to be able to correctly
@@ -984,16 +1060,18 @@
         #  that we can raise in an appropriate task. However, we should make sure that we
         #  account for the signal handling that RP expects to be able to do.
         #  See https://github.com/SCALE-MS/randowtal/issues/1
         #  We should also make sure that scalems and RP together handle keyboard interrupts
         #  as a user would expect.
         # Note that PilotDescription can use `'exit_on_error': False` to suppress the SIGINT,
         # but we have not fully explored the consequences of doing so.
+        # Note also that RP Task.cancel() issues a SIGTERM in Task processes,
+        # which we would normally be even more cautious about trapping, so we should
+        # avoid explicitly or implicitly allowing Task.cancel().
 
-        to_thread = scalems.compat.get_to_thread()
         try:
             #
             # Start the Session.
             #
 
             # Note: the current implementation implies that only one Task for the dispatcher
             # will exist at a time. We are further assuming that there will probably only
@@ -1006,23 +1084,23 @@
             session_id = _runtime.session.uid
             # Do we want to log this somewhere?
             # session_config = copy.deepcopy(self.session.cfg.as_dict())
             logger.debug("RP dispatcher acquired session {}".format(session_id))
 
             logger.debug("Launching PilotManager.")
             pilot_manager = await asyncio.create_task(
-                to_thread(rp.PilotManager, session=_runtime.session),
+                asyncio.to_thread(rp.PilotManager, session=_runtime.session),
                 name="get-PilotManager",
             )
             logger.debug("Got PilotManager {}.".format(pilot_manager.uid))
             _runtime.pilot_manager(pilot_manager)
 
             logger.debug("Launching TaskManager.")
             task_manager = await asyncio.create_task(
-                to_thread(rp.TaskManager, session=_runtime.session),
+                asyncio.to_thread(rp.TaskManager, session=_runtime.session),
                 name="get-TaskManager",
             )
             logger.debug(("Got TaskManager {}".format(task_manager.uid)))
             _runtime.task_manager(task_manager)
 
             #
             # Get a Pilot
@@ -1034,19 +1112,27 @@
             # but it seems like a good chance to start bootstrapping the agent environment.
             #
             # How and when should we update the pilot description?
 
             pilot = await add_pilot(runtime=_runtime)
             logger.debug("Added Pilot {} to task manager {}.".format(pilot.uid, _runtime.task_manager().uid))
 
+            # TODO: Asynchronous data staging optimization.
+            #  Allow input data staging to begin before scheduler is in state EXECUTING and
+            #  before Pilot is in state PMGR_ACTIVE.
+
+            # Note: This could take hours or days depending on the queuing system.
+            # Can we report some more useful information, like job ID?
+            _runtime.resources = asyncio.create_task(get_pilot_resources(pilot))
+
             assert _runtime.scheduler is None
 
             # Get a scheduler task IFF raptor is explicitly enabled.
             if config.enable_raptor:
-                # Note that _get_scheduler is a coroutine that, itself, returns a Task.
+                # Note that _get_scheduler is a coroutine that, itself, returns a rp.Task.
                 # We await the result of _get_scheduler, then store the scheduler Task.
                 _runtime.scheduler = await asyncio.create_task(
                     _get_scheduler(
                         pre_exec=list(get_pre_exec(config)),
                         task_manager=task_manager,
                         filestore=config.datastore,
                         scalems_env="scalems_venv",
@@ -1073,14 +1159,69 @@
         runner_task = asyncio.create_task(scalems.execution.manage_execution(self, processing_state=runner_started))
         await runner_started.wait()
         # TODO: Note the expected scope of the runner_task lifetime with respect to
         #  the global state changes (i.e. ContextVars and locks).
         return runner_task
 
     @staticmethod
+    async def cpi(command: str, runtime: Runtime):
+        """Send a control command to the raptor scheduler.
+
+        Implements :py:func:`scalems.execution.RuntimeManager.cpi()`
+
+        TODO: Unify with new raptor cpi feature.
+        """
+        timeout = 180
+
+        logger.debug(f'Received command "{command}" for runtime {runtime}.')
+        if runtime is None:
+            raise scalems.exceptions.ScopeError("Cannot issue control commands without an active RuntimeManager.")
+        scheduler: rp.Task = runtime.scheduler
+        logger.debug(f"Preparing command for {repr(scheduler)}.")
+        if scheduler is None:
+            raise scalems.exceptions.ScopeError(
+                f"Cannot issue control commands without an active RuntimeManager. {runtime}"
+            )
+        if scheduler.state in rp.FINAL:
+            raise scalems.exceptions.ScopeError(f"Raptor scheduler is not available. {repr(scheduler)}")
+        assert scheduler.uid
+        message = scalems.messages.Control.create(command)
+        td = rp.TaskDescription(
+            from_dict={
+                "scheduler": scheduler.uid,
+                "mode": scalems.radical.raptor.CPI_MESSAGE,
+                "metadata": message.encode(),
+                "uid": EphemeralIdentifier(),
+            }
+        )
+        logger.debug(f"Submitting {str(td.as_dict())}")
+        (task,) = await asyncio.to_thread(runtime.task_manager().submit_tasks, [td])
+        logger.debug(f"Submitted {str(task.as_dict())}. Waiting...")
+        # Warning: we can't wait on the final state of such an rp.Task unless we
+        # _also_ watch the scheduler itself, because there are various circumstances
+        # in which the Task may never reach a rp.FINAL state.
+
+        command_watcher = asyncio.create_task(
+            asyncio.to_thread(task.wait, state=rp.FINAL, timeout=timeout), name="cpi-watcher"
+        )
+
+        scheduler_watcher = asyncio.create_task(
+            asyncio.to_thread(scheduler.wait, state=rp.FINAL, timeout=timeout), name="scheduler-watcher"
+        )
+        # If master task fails, command-watcher will never complete.
+        done, pending = await asyncio.wait(
+            (command_watcher, scheduler_watcher), timeout=timeout, return_when=asyncio.FIRST_COMPLETED
+        )
+        if scheduler_watcher in done and command_watcher in pending:
+            command_watcher.cancel()
+        logger.debug(str(task.as_dict()))
+        # WARNING: Dropping the Task reference will cause its deletion.
+        return command_watcher
+
+    @staticmethod
     def runtime_shutdown(runtime: Runtime):
         """Manage tear down of the RADICAL Pilot Session and resources.
 
         Several aspects of the RP runtime interface use blocking calls.
         This method should be run in a non-root thread (concurrent.futures.Future)
         that the event loop can manage as an asyncio-wrapped task.
 
@@ -1091,30 +1232,32 @@
             raise scalems.exceptions.APIError(f"No Session in {runtime}.")
         if session.closed:
             logger.error("Runtime Session is already closed?!")
         else:
             if runtime.scheduler is not None:
                 # Note: The __aexit__ for the RuntimeManager makes sure that a `stop`
                 # is issued after the work queue is drained, if the scheduler task has
-                # not already ended.
-                runtime.scheduler.wait(rp.FINAL, timeout=10)
+                # not already ended. We could check the status of this stop message...
+                if runtime.scheduler.state not in rp.FINAL:
+                    logger.info(f"Waiting for RP Raptor master task {runtime.scheduler.uid} to complete...")
+                    runtime.scheduler.wait(rp.FINAL, timeout=60)
                 if runtime.scheduler.state not in rp.FINAL:
                     # Cancel the master.
-                    logger.debug("Canceling the master scheduling task.")
+                    logger.warning("Canceling the master scheduling task.")
                     # Note: the effect of CANCEL is to send SIGTERM to the shell that
                     # launched the task process.
                     # TODO: Report incomplete tasks and handle the consequences of terminating the
                     #  Raptor processes early.
                     task_manager = runtime.task_manager()
                     task_manager.cancel_tasks(uids=runtime.scheduler.uid)
                 # As of https://github.com/radical-cybertools/radical.pilot/pull/2702,
                 # we do not expect `cancel` to block, so we must wait for the
                 # cancellation to succeed. It shouldn't take long, but it is not
                 # instantaneous or synchronous. We hope that a minute is enough.
-                final_state = runtime.scheduler.wait(state=rp.FINAL, timeout=60)
+                final_state = runtime.scheduler.wait(state=rp.FINAL, timeout=10)
                 logger.debug(f"Final state: {final_state}")
                 logger.info(f"Master scheduling task state {runtime.scheduler.state}: {repr(runtime.scheduler)}.")
                 if runtime.scheduler.stdout:
                     # TODO(#229): Fetch actual stdout file.
                     logger.debug(runtime.scheduler.stdout)
                 if runtime.scheduler.stderr:
                     # TODO(#229): Fetch actual stderr file.
@@ -1721,24 +1864,27 @@
         *executable* RP tasks from Python tasks managed with raptor functionality.
     """
 
     uid: str
     """:py:attr:`radical.pilot.Task.uid` identifier."""
 
     task_dict: dict
-    """Dictionary representation from `radical.pilot.Task.as_dict()`."""
+    """Dictionary representation from :py:func:`radical.pilot.Task.as_dict()`."""
 
     exit_code: int
     """Exit code of the executable task."""
 
     final_state: str
     """Final state of the `radical.pilot.Task`."""
 
     directory: radical.utils.Url
-    """Resource location information for the Task working directory."""
+    """Resource location information for the Task working directory.
+
+    Constructed from the filesystem_endpoint. See :doc:`design/localization`.
+    """
 
     directory_archive: Awaitable[scalems.store.FileReference]
     """An archive of the task working directory.
 
     This result is separately awaitable to allow elision of unnecessary transfers.
     The exact implementation is not strongly specified; a Future usually implies
     that the result will eventually be produced, whereas a more general "awaitable"
@@ -1750,69 +1896,92 @@
     TODO: In the next iteration, use a non-local FileReference or (TBD) DirectoryReference.
     """
 
 
 async def subprocess_to_rp_task(
     call_handle: scalems.call._Subprocess, dispatcher: RPDispatchingExecutor
 ) -> RPTaskResult:
-    """Dispatch a subprocess task through the scalems.rp execution backend.
+    """Dispatch a subprocess task through the `scalems.radical` execution backend.
 
     Get a Future for a RPTaskResult (a collection representing a completed rp.Task).
 
     Schedule a RP Task and wrap with asyncio. Subscribe a dependent asyncio.Task
     that can provide the intended result type and return it as the Future.
     Schedule a call-back to clean up temporary files.
 
+    Args:
+        call_handle (scalems.call._Subprocess): result of a ``await`` on a
+            :py:func:`scalems.call.function_call_to_subprocess()`
+        dispatcher (RPDispatchingExecutor): An active execution manager.
+
     TODO:
-        This logic should be integrated into the `WorkflowManager.submit()` stack
+        This logic should be integrated into a :py:func:`WorkflowManager.submit()`
+        stack (currently :py:func:`WorkflowManager.add_item()`)
         and `manage_execution` loop. We really should have special handling for
-        wrapped function calls as distinguished from command line executables.
+        wrapped function calls as distinguished from command line executables
+        through "overloads" (dispatching) of the task submission.
+        Also, we should not be exposing the *dispatcher* to the user.
     """
     subprocess_dict = dict(
         stage_on_error=True,
         uid=call_handle.uid,
         executable=call_handle.executable,
         arguments=list(call_handle.arguments),
         pre_exec=list(get_pre_exec(dispatcher.configuration())),
+        mode=rp.TASK_EXECUTABLE,
     )
-
+    if configuration().enable_raptor:
+        subprocess_dict["scheduler"] = dispatcher.runtime.scheduler.uid
     # Capturing stdout/stderr is a potentially unusual or unexpected behavior for
     # a Python function runner, and may collide with user assumptions or native
     # behaviors of third party tools. We will specify distinctive names for the RP
     # output capture files in the hope of clarifying the component responsible for
     # these files.
     subprocess_dict["stdout"] = "_scalems_stdout.txt"
     subprocess_dict["stderr"] = "_scalems_stderr.txt"
 
-    # TODO: Localize the files directly to the execution site, instead, and use the
-    #   (remotely valid) URI (with a COPY or LINK action).
-    #   Perform transfers concurrently and await successful transfer
-    #   before the submit_tasks call.
+    # Note: We could save wall time in the job by pre-staging files, but we are
+    # deferring that for future optimization.
+    # Ref: https://github.com/SCALE-MS/scale-ms/issues/316
     await asyncio.gather(*tuple(ref.localize() for ref in call_handle.input_filenames.values()))
     subprocess_dict["input_staging"] = [
         {
             "source": ref.as_uri(),
             # TODO: Find a programmatic mechanism to translate between URI and CLI arg for robustness.
-            "target": "task:///" + name,
+            "target": f"task:///{name}",
             "action": rp.TRANSFER,
         }
         for name, ref in call_handle.input_filenames.items()
     ]
 
+    # We just pass the user-provided requirements through, but we have to reject
+    # any that collide with parameters we expect to generate.
     for param, value in call_handle.requirements.items():
         if param in subprocess_dict:
             raise ValueError(f"Cannot overwrite {param}. Task['{param}'] is {subprocess_dict[param]}")
         else:
             subprocess_dict[param] = value
 
     try:
         subprocess_task_description = rp.TaskDescription(from_dict=subprocess_dict).verify()
     except radical.utils.typeddict.TDKeyError as e:
         raise ValueError("Invalid attribute for RP TaskDescription.") from e
 
+    task_cores = subprocess_task_description.cores_per_rank * subprocess_task_description.cpu_processes
+    rm_info = await dispatcher.runtime.resources
+    pilot_cores = rm_info["requested_cores"]
+    # TODO: Account for Worker cores.
+    if configuration().enable_raptor:
+        raptor_task: rp.Task = dispatcher.runtime.scheduler
+        raptor_cores = raptor_task.description["ranks"] * raptor_task.description["cores_per_rank"]
+    else:
+        raptor_cores = 0
+    if task_cores > (available_cores := pilot_cores - raptor_cores):
+        raise ValueError(f"Requested {task_cores} for {call_handle.uid}, but at most {available_cores} are available.")
+
     # TODO: Find a better way to express these three lines.
     # This seems like it should be a subscription by the local workflow context to the
     # RP dispatching workflow context. Something like
     #     supporting_task = await rp_manager.add_task(task_description)
     #     supporting_task.add_done_callback(...)
     task_manager = dispatcher.runtime.task_manager()
     (submitted_task,) = await asyncio.to_thread(task_manager.submit_tasks, [subprocess_task_description])
@@ -1855,14 +2024,28 @@
     )
     return result
 
 
 async def wrapped_function_result_from_rp_task(
     subprocess: scalems.call._Subprocess, rp_task_result: RPTaskResult
 ) -> scalems.call.CallResult:
+    """
+
+    Once `subprocess_to_rp_task` has produced a `RPTaskResult`
+    for a `scalems.call._Subprocess`,
+    we produce a `scalems.call.CallResult` with the help of some file transfers.
+
+    Args:
+        subprocess: the result of a `scalems.call.function_call_to_subprocess`
+        rp_task_result: the result of a `subprocess_to_rp_task` for the *subprocess*
+
+    Returns:
+        localized result from :py:func:`scalems.call.function_call_to_subprocess()`
+
+    """
     if rp_task_result.final_state != rp.DONE:
         # Note: it is possible that the executable task could fail for reasons other than a Python Exception.
         logger.info(f"Task for {subprocess.uid} in final state {rp_task_result.final_state}.")
         logger.debug(repr(rp_task_result))
     # It looks like this should be encapsulated with the workflow management details
     # of the dispatched work item or further specialized for this specific task type.
     # It doesn't make sense that we should need both the _Subprocess and
```

### Comparing `scalems-0.0.0a1/src/scalems/serialization.py` & `scalems-0.0.1b1/src/scalems/serialization.py`

 * *Files identical despite different names*

### Comparing `scalems-0.0.0a1/src/scalems/store/__init__.py` & `scalems-0.0.1b1/src/scalems/store/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """Manage non-volatile data for SCALE-MS in a filesystem context.
 
+Implement several interfaces from `scalems.file`.
+
 The data store must be active before attempting any manipulation of the managed workflow.
 The data store must be closed by the time control returns to the interpreter after
 leaving a managed workflow scope (and releasing a WorkflowManager instance).
 
 We prefer to do this with the Python context manager protocol, since we already rely on
 `scalems.workflow.scope()`.
 
@@ -18,16 +20,19 @@
 __all__ = (
     "StaleFileStore",
     "filestore_generator",
     "get_file_reference",
     "FileReference",
     "FileStore",
     "FileStoreManager",
+    "FilesView",
+    "Metadata",
 )
 
+import asyncio
 import contextvars
 import dataclasses
 import functools
 import json
 import logging
 import os
 import pathlib
@@ -37,15 +42,14 @@
 import typing
 import weakref
 
 import scalems.exceptions as _exceptions
 from . import _lock
 from .. import file as _file
 from .. import identifiers as _identifiers
-from .. import compat as _compat
 
 logger = logging.getLogger(__name__)
 logger.debug("Importing {}".format(__name__))
 
 _data_subdirectory = "scalems_0_0"
 """Subdirectory name to use for managed filestore."""
 
@@ -120,16 +124,14 @@
         for key in self._files:
             yield _identifiers.ResourceIdentifier(bytes.fromhex(key))
 
 
 class FileStore(typing.Mapping[_identifiers.ResourceIdentifier, "FileReference"]):
     """Handle to the SCALE-MS nonvolatile data store for a workflow context.
 
-    Not thread safe. User is responsible for serializing access, as necessary.
-
     Used as a Container, serves as a Mapping from identifiers to resource references.
 
     TODO: Consider generalizing the value type of the mapping for general Resource types, per the scalems data model.
     """
 
     _fields: typing.ClassVar = set([field.name for field in dataclasses.fields(Metadata)])
     _instances: typing.ClassVar = weakref.WeakValueDictionary()
@@ -191,28 +193,28 @@
         return self._datastore
 
     @property
     def filepath(self) -> pathlib.Path:
         """Path to the metadata backing store.
 
         This is the metadata file used by scalems to track workflow state and
-        file-backed data. Its format is closely related to the scalems API level.
+        file-backed data. Its format is closely tied to the scalems API level.
         """
         if self._filepath is None:
             self._filepath = self.datastore / _metadata_filename
         return self._filepath
 
     @property
     def instance(self):
         return self._data.instance
 
     def __repr__(self):
         return str(self._repr)
 
-    def __getitem__(self, __k: _identifiers.ResourceIdentifier) -> "FileReference":
+    def __getitem__(self, __k: _identifiers.ResourceIdentifier | str) -> "FileReference":
         return FileReference(filestore=self, key=__k)
 
     def __len__(self) -> int:
         return len(self._data.files)
 
     def __iter__(self) -> typing.Iterator[_identifiers.ResourceIdentifier]:
         return iter(self.files)
@@ -228,20 +230,20 @@
         and instead use a FileStoreManager object.
 
         No directory in the filesystem should be managed by more than one FileStore.
         The FileStore class maintains a registry of instances to prevent instantiation of
         a new FileStore for a directory that is already managed.
 
         Raises:
-            ContextError if attempting to instantiate for a directory that is already
-            managed.
+            ContextError: if attempting to instantiate for a directory that is already
+                managed.
         """
         self._directory = pathlib.Path(directory).resolve()
 
-        # TODO: Use a log file!
+        # TODO: Use file backing for journaled operations.
         self._log = []
 
         self._update_lock = threading.Lock()
         self._dirty = threading.Event()
 
         try:
             with _lock.scoped_directory_lock(self._directory):
@@ -341,14 +343,18 @@
                     raise StaleFileStore("Cannot flush stale FileStore.")
                 pathlib.Path(fp.name).rename(self.filepath)
                 self._dirty.clear()
 
     def close(self):
         """Flush, shut down, and disconnect the FileStore from the managed directory.
 
+        Not robustly thread safe. User is responsible for serializing access, as necessary,
+        though ideally *close()* should be called exactly once, after the instance is no
+        longer in use.
+
         Raises:
             StaleFileStore if called on an invalid or outdated handle.
             ScopeError if called from a disallowed context, such as from a forked process.
 
         """
         actual_manager = FileStore._instances.get(self._directory, None)
         if actual_manager is None:
@@ -404,14 +410,16 @@
         return False
 
     async def add_file(
         self, obj: typing.Union[_file.AbstractFile, _file.AbstractFileReference], _name: str = None
     ) -> FileReference:
         """Add a file to the file store.
 
+        Not thread safe. User is responsible for serializing access, as necessary.
+
         We require file paths to be wrapped in a special type so that we can enforce
         that some error checking is possible before the coroutine actually runs. See
 
         This involves placing (copying) the file, reading the file to fingerprint it,
         and then writing metadata for the file. For clarity, we also rename the file
         after fingerprinting to remove a layer of indirection, even though this
         generates additional load on the filesystem.
@@ -444,48 +452,51 @@
         # Note: We can use a more effective and flexible `try: ... except: ...` check
         # once we actually have AbstractFileReference support ready to use here, at which point
         # we can consider removing runtime_checkable from AbstractFileReference to avoid false
         # confidence. However, we may prefer to convert AbstractFileReference to an abc.ABC so
         # that we can actually functools.singledispatchmethod on the provided object.
         if isinstance(obj, _file.AbstractFileReference):
             raise _exceptions.MissingImplementationError("AbstractFileReference input not yet supported.")
+        # Early exit check. We need to check again once we have a lock.
         if self.closed:
             raise StaleFileStore("Cannot add file to a closed FileStore.")
         path: pathlib.Path = pathlib.Path(obj)
-        to_thread = _compat.get_to_thread()
-
         filename = None
         key = None
         _fd, tmpfile_target = tempfile.mkstemp(prefix=self._tmpfile_prefix, dir=self.datastore)
         os.close(_fd)
         tmpfile_target = pathlib.Path(tmpfile_target)
         try:
             # 1. Copy the file.
             kwargs = dict(src=path, dst=tmpfile_target, follow_symlinks=False)
-            _path = await to_thread(shutil.copyfile, **kwargs)
+            _path = await asyncio.to_thread(shutil.copyfile, **kwargs)
             assert tmpfile_target == _path
             assert tmpfile_target.exists()
             # We have now secured a copy of the file. We could just schedule the remaining
             # operations and return. For the initial implementation though, we will wait
             # until we have read the file. When optimizing for inputs that are already
             # fingerprinted, we could return before AbstractFileReference.localize() has
             # finished and schedule a checksum verification that localize() must wait for.
 
             # 2. Fingerprint the file.
-            checksum = await to_thread(obj.fingerprint, **{})
+            checksum = await asyncio.to_thread(obj.fingerprint, **{})
             identifier = _identifiers.ResourceIdentifier(checksum)
 
             # 3. Choose a key.
             key = str(identifier)
 
             # 4. Write metadata.
             if _name is None:
                 _name = key
             filename = self.datastore.joinpath(_name)
             with self._update_lock:
+                # Check again, now that we have the lock.
+                if self.closed:
+                    raise StaleFileStore("Cannot add file to a closed FileStore.")
+
                 if key in self._data.files:
                     raise _exceptions.DuplicateKeyError(f"FileStore is already managing a file with key {key}.")
                 if str(filename) in self._data.files.values():
                     raise _exceptions.DuplicateKeyError(f"FileStore already has {filename}.")
                 else:
                     if filename.exists():
                         raise StaleFileStore(f"Unexpected file in filestore: {filename}.")
@@ -495,28 +506,29 @@
                 # We can create a stronger separation between the metadata manager and
                 # the backing data store and/or restrict assignment to use a general
                 # Data Descriptor that manages our "dirty" flag.
                 self._dirty.set()
                 self._data.files[key] = str(filename)
 
             return FileReference(filestore=self, key=key)
+        except (_exceptions.DuplicateKeyError, StaleFileStore) as e:
+            tmpfile_target.unlink(missing_ok=True)
+            raise e
         except Exception as e:
-            if isinstance(e, (_exceptions.DuplicateKeyError, StaleFileStore)):
-                tmpfile_target.unlink(missing_ok=True)
-            else:
-                # Something went particularly wrong. Let's try to clean up as best we can.
-                logger.exception(f"Unhandled exception while trying to store {obj}")
-                if key and key in self._data.files:
-                    pathlib.Path(self._data.files[key]).unlink(missing_ok=True)
-                    del self._data.files[key]
-                if isinstance(filename, pathlib.Path):
-                    filename.unlink(missing_ok=True)
+            # Something went particularly wrong. Let's try to clean up as best we can.
+            logger.exception(f"Unhandled exception while trying to store {obj}")
+            if key and key in self._data.files:
+                pathlib.Path(self._data.files[key]).unlink(missing_ok=True)
+                del self._data.files[key]
+            if isinstance(filename, pathlib.Path):
+                filename.unlink(missing_ok=True)
+            raise e
+        finally:
             if tmpfile_target.exists():
                 logger.warning(f"Temporary file left at {tmpfile_target}")
-            raise e
 
     @property
     def files(self) -> typing.Mapping[_identifiers.ResourceIdentifier, pathlib.Path]:
         """Proxy to the managed files metadata.
 
         The proxy is read-only, but dynamic. A reference to *FileStore.files*
         will provide a dynamic view for later use.
@@ -550,14 +562,19 @@
             self._dirty.set()
             self._data.objects[str(identity)] = dict(**kwargs)
             # TODO: Take care with the value types that we can serialize and
             #  deserialize them.
 
 
 class FileReference(_file.AbstractFileReference):
+    """Provide access to a :py:class:`File <scalems.file.AbstractFile>` managed by a `FileStore`.
+
+    Implements :py:class:`~scalems.file.AbstractFileReference`.
+    """
+
     def __init__(self, filestore: FileStore, key: _identifiers.ResourceIdentifier | str):
         self._filestore: FileStore = filestore
         if key not in self._filestore.files:
             raise _exceptions.ProtocolError("Cannot create reference to unmanaged file.")
         if not isinstance(key, _identifiers.ResourceIdentifier):
             key = _identifiers.ResourceIdentifier(bytes.fromhex(key))
         self._key = key
@@ -683,15 +700,15 @@
     TODO: Optimize. (This call should only read and fingerprint *obj* once.)
     """
     obj = _file.describe_file(obj.resolve(), mode=mode)
     try:
         file_ref = await filestore.add_file(_file.describe_file(obj, mode=mode))
     except _exceptions.DuplicateKeyError:
         # Return the existing fileref, if it matches the fingerprint of *obj*.
-        fingerprint = await _compat.get_to_thread()(obj.fingerprint)
+        fingerprint = await asyncio.to_thread(obj.fingerprint)
         key = _identifiers.ResourceIdentifier(fingerprint)
         file_ref = filestore.get(key)
     return file_ref
 
 
 @functools.singledispatch
 def get_file_reference(obj, filestore=None, mode="rb") -> typing.Coroutine[None, None, FileReference]:
```

### Comparing `scalems-0.0.0a1/src/scalems/store/_lock.py` & `scalems-0.0.1b1/src/scalems/store/_lock.py`

 * *Files identical despite different names*

### Comparing `scalems-0.0.0a1/src/scalems/subprocess/__init__.py` & `scalems-0.0.1b1/src/scalems/subprocess/__init__.py`

 * *Files identical despite different names*

### Comparing `scalems-0.0.0a1/src/scalems/subprocess/_subprocess.py` & `scalems-0.0.1b1/src/scalems/subprocess/_subprocess.py`

 * *Files 1% similar despite different names*

```diff
@@ -415,10 +415,8 @@
     except json.JSONDecodeError as e:
         logger.critical("Malformed data: " + e.msg)
         raise InternalError("Bug: internal data is not being conditioned properly") from e
     except Exception as e:
         logger.critical("Unhandled " + repr(e))
         raise
 
-    # TODO: The returned value should be a TaskView provided by the Context with
-    #       minimal state or ownership semantics.
     return task_view
```

### Comparing `scalems-0.0.0a1/src/scalems/unique.py` & `scalems-0.0.1b1/src/scalems/unique.py`

 * *Files identical despite different names*

### Comparing `scalems-0.0.0a1/src/scalems/workflow/__init__.py` & `scalems-0.0.1b1/src/scalems/workflow/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,17 +96,15 @@
     If the WorkflowManager from which the ItemView was obtained goes out of scope or
     otherwise becomes invalid, some ItemView interfaces can raise exceptions.
 
     .. todo:: Allows proxied access to future results through attribute access.
 
     """
 
-    # TODO: Update once we require Python 3.9
-    # _workflow_manager: weakref.ReferenceType['WorkflowManager']
-    _workflow_manager: weakref.ReferenceType
+    _workflow_manager: weakref.ReferenceType["WorkflowManager"]
 
     def uid(self) -> bytes:
         """Get the canonical unique identifier for this task.
 
         The identifier is universally unique and can be used to query any
         workflow manager for awareness of the task and (if the context is aware
         of the task) to get a view of the task.
@@ -696,15 +694,25 @@
     #     Returns:
     #         Reference to the new task.
     #
     #     TODO: Resolve operation implementation to dispatch task configuration.
     #     """
     #     ...
 
-    def add_item(self, task_description) -> ItemView:
+    def add_item(self, item) -> ItemView:
+        """
+        Add an item to the managed workflow.
+
+        Args:
+            item: Describe the item to be managed. (Usually a task to be submitted.)
+
+        Returns:
+            View of the managed item.
+
+        """
         if self.closed:
             raise ScopeError("WorkflowManager is closed.")
 
         # # TODO: Resolve implementation details for *operation*.
         # if operation != 'scalems.executable':
         #     raise MissingImplementationError('No implementation for {} in {}'.format(
         #     operation, repr(self)))
@@ -715,46 +723,47 @@
         # if not isinstance(bound_input, scalems.subprocess.SubprocessInput):
         #     raise ValueError('Only scalems.subprocess.SubprocessInput objects
         #     supported as input.')
 
         # TODO: Replace with type-based dispatching or some normative interface test.
         from scalems.subprocess import Subprocess
 
-        if not isinstance(task_description, (Subprocess, dict)):
+        if not isinstance(item, (Subprocess, dict)):
             raise MissingImplementationError("Operation not supported.")
 
         # TODO: Generalize interface check.
-        if isinstance(task_description, Subprocess):
-            uid: bytes = task_description.uid()
+        if isinstance(item, Subprocess):
+            uid: bytes = item.uid()
             if uid in self.tasks:
                 # TODO: Consider decreasing error level to `warning`.
                 raise DuplicateKeyError("Task already present in workflow.")
-            logger.debug("Adding {} to {}".format(str(task_description), str(self)))
-            record = {"uid": uid.hex(), "type": task_description.resource_type().scoped_identifier(), "input": {}}
-            task_input = task_description.input_collection()
+            logger.debug("Adding {} to {}".format(str(item), str(self)))
+            record = {"uid": uid.hex(), "type": item.resource_type().scoped_identifier(), "input": {}}
+            task_input = item.input_collection()
             for field in dataclasses.fields(task_input):
                 name = field.name
                 try:
                     # TODO: Need serialization typing.
                     record["input"][name] = getattr(task_input, name)
                 except AttributeError as e:
                     raise InternalError("Unexpected missing field.") from e
         else:
-            assert isinstance(task_description, dict)
-            assert "uid" in task_description
-            uid = task_description["uid"]
-            implementation_identifier = task_description.get("implementation", None)
+            # WARNING: no coverage
+            assert isinstance(item, dict)
+            assert "uid" in item
+            uid = item["uid"]
+            implementation_identifier = item.get("implementation", None)
             if not isinstance(implementation_identifier, list):
                 raise DispatchError("Bug: bad schema checking?")
 
             if uid in self.tasks:
                 # TODO: Consider decreasing error level to `warning`.
                 raise DuplicateKeyError("Task already present in workflow.")
-            logger.debug("Adding {} to {}".format(str(task_description), str(self)))
-            record = {"uid": uid.hex(), "type": tuple(implementation_identifier), "input": task_description}
+            logger.debug("Adding {} to {}".format(str(item), str(self)))
+            record = {"uid": uid.hex(), "type": tuple(implementation_identifier), "input": item}
         serialized_record = json.dumps(record, default=encode)
 
         # TODO: Make sure there are no artifacts of shallow copies that may result in
         #       a user modifying nested objects unexpectedly.
         item = Task(self, serialized_record)
         # TODO: Check for ability to dispatch.
         #  Note module dependencies, etc. and check in target execution environment
```

### Comparing `scalems-0.0.0a1/src/scalems/wrappers/__init__.py` & `scalems-0.0.1b1/src/scalems/wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `scalems-0.0.0a1/src/scalems/wrappers/gromacs.py` & `scalems-0.0.1b1/src/scalems/wrappers/gromacs.py`

 * *Files identical despite different names*

