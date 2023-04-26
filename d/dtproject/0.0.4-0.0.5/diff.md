# Comparing `tmp/dtproject-0.0.4.tar.gz` & `tmp/dtproject-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtproject-0.0.4.tar", last modified: Fri Apr 21 04:30:02 2023, max compression
+gzip compressed data, was "dtproject-0.0.5.tar", last modified: Wed Apr 26 13:48:24 2023, max compression
```

## Comparing `dtproject-0.0.4.tar` & `dtproject-0.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-21 04:30:02.826169 dtproject-0.0.4/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      424 2023-04-21 04:30:02.826169 dtproject-0.0.4/PKG-INFO
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       38 2023-04-21 04:30:02.826169 dtproject-0.0.4/setup.cfg
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1765 2023-04-20 03:32:32.000000 dtproject-0.0.4/setup.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-21 04:30:02.826169 dtproject-0.0.4/src/
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-21 04:30:02.826169 dtproject-0.0.4/src/dtproject/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      163 2023-04-21 04:29:56.000000 dtproject-0.0.4/src/dtproject/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      418 2023-04-19 22:08:11.000000 dtproject-0.0.4/src/dtproject/configurations.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     6706 2023-04-21 03:32:51.000000 dtproject-0.0.4/src/dtproject/constants.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    25965 2023-04-21 03:36:57.000000 dtproject-0.0.4/src/dtproject/dtproject.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      480 2023-04-20 03:25:31.000000 dtproject-0.0.4/src/dtproject/exceptions.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     6316 2023-04-20 03:28:28.000000 dtproject-0.0.4/src/dtproject/recipe.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-21 04:30:02.826169 dtproject-0.0.4/src/dtproject/utils/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 02:38:03.000000 dtproject-0.0.4/src/dtproject/utils/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1326 2023-04-20 14:46:26.000000 dtproject-0.0.4/src/dtproject/utils/docker.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1198 2023-04-20 03:17:17.000000 dtproject-0.0.4/src/dtproject/utils/misc.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-21 04:30:02.826169 dtproject-0.0.4/src/dtproject.egg-info/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      424 2023-04-21 04:30:02.000000 dtproject-0.0.4/src/dtproject.egg-info/PKG-INFO
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      446 2023-04-21 04:30:02.000000 dtproject-0.0.4/src/dtproject.egg-info/SOURCES.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        1 2023-04-21 04:30:02.000000 dtproject-0.0.4/src/dtproject.egg-info/dependency_links.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       27 2023-04-21 04:30:02.000000 dtproject-0.0.4/src/dtproject.egg-info/requires.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       10 2023-04-21 04:30:02.000000 dtproject-0.0.4/src/dtproject.egg-info/top_level.txt
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-26 13:48:24.826359 dtproject-0.0.5/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      424 2023-04-26 13:48:24.826359 dtproject-0.0.5/PKG-INFO
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       38 2023-04-26 13:48:24.826359 dtproject-0.0.5/setup.cfg
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1765 2023-04-26 13:48:11.000000 dtproject-0.0.5/setup.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-26 13:48:24.822359 dtproject-0.0.5/src/
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-26 13:48:24.822359 dtproject-0.0.5/src/dtproject/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      163 2023-04-26 13:48:18.000000 dtproject-0.0.5/src/dtproject/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      418 2023-04-19 22:08:11.000000 dtproject-0.0.5/src/dtproject/configurations.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     6721 2023-04-26 13:47:21.000000 dtproject-0.0.5/src/dtproject/constants.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    25965 2023-04-21 03:36:57.000000 dtproject-0.0.5/src/dtproject/dtproject.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      480 2023-04-20 03:25:31.000000 dtproject-0.0.5/src/dtproject/exceptions.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     6316 2023-04-20 03:28:28.000000 dtproject-0.0.5/src/dtproject/recipe.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-26 13:48:24.826359 dtproject-0.0.5/src/dtproject/utils/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 02:38:03.000000 dtproject-0.0.5/src/dtproject/utils/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1326 2023-04-20 14:46:26.000000 dtproject-0.0.5/src/dtproject/utils/docker.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1198 2023-04-20 03:17:17.000000 dtproject-0.0.5/src/dtproject/utils/misc.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-26 13:48:24.826359 dtproject-0.0.5/src/dtproject.egg-info/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      424 2023-04-26 13:48:24.000000 dtproject-0.0.5/src/dtproject.egg-info/PKG-INFO
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      446 2023-04-26 13:48:24.000000 dtproject-0.0.5/src/dtproject.egg-info/SOURCES.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        1 2023-04-26 13:48:24.000000 dtproject-0.0.5/src/dtproject.egg-info/dependency_links.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       27 2023-04-26 13:48:24.000000 dtproject-0.0.5/src/dtproject.egg-info/requires.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       10 2023-04-26 13:48:24.000000 dtproject-0.0.5/src/dtproject.egg-info/top_level.txt
```

### Comparing `dtproject-0.0.4/setup.py` & `dtproject-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `dtproject-0.0.4/src/dtproject/constants.py` & `dtproject-0.0.5/src/dtproject/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 ARCH_TO_PLATFORM_OS = {"arm32v7": "linux", "arm64v8": "linux", "amd64": "linux"}
 
 ARCH_TO_PLATFORM_ARCH = {"arm32v7": "arm", "arm64v8": "arm64", "amd64": "amd64"}
 
 ARCH_TO_PLATFORM_VARIANT = {"arm32v7": "v7", "arm64v8": "", "amd64": ""}
 
 # kept for backward compatibility
-DISTRO_KEY = {"1": "MAJOR", "2": "DISTRO", "3": "DISTRO"}
+DISTRO_KEY = {"1": "MAJOR", "2": "DISTRO", "3": "DISTRO", "4": "DISTRO"}
 
 TEMPLATE_TO_SRC: Dict[ProjectType,
                       Dict[ProjectTypeVersion,
                            Callable[[ProjectName], Tuple[RelativePath, ContainerPath]]]] = {
     # NOTE: these are not templates, they only serve the project matching their names
     "dt-commons": {
         "1": lambda _repo: ("code", "/packages/{:s}/".format(_repo)),
```

### Comparing `dtproject-0.0.4/src/dtproject/dtproject.py` & `dtproject-0.0.5/src/dtproject/dtproject.py`

 * *Files identical despite different names*

### Comparing `dtproject-0.0.4/src/dtproject/recipe.py` & `dtproject-0.0.5/src/dtproject/recipe.py`

 * *Files identical despite different names*

### Comparing `dtproject-0.0.4/src/dtproject/utils/docker.py` & `dtproject-0.0.5/src/dtproject/utils/docker.py`

 * *Files identical despite different names*

### Comparing `dtproject-0.0.4/src/dtproject/utils/misc.py` & `dtproject-0.0.5/src/dtproject/utils/misc.py`

 * *Files identical despite different names*

