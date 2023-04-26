# Comparing `tmp/soscucu-0.1.0.tar.gz` & `tmp/soscucu-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soscucu-0.1.0.tar", last modified: Wed Apr 26 02:08:49 2023, max compression
+gzip compressed data, was "soscucu-0.1.1.tar", last modified: Wed Apr 26 02:20:02 2023, max compression
```

## Comparing `soscucu-0.1.0.tar` & `soscucu-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,14 @@
-drwxrwxr-x   0 lee       (1000) lee       (1000)        0 2023-04-26 02:08:49.310635 soscucu-0.1.0/
--rw-rw-r--   0 lee       (1000) lee       (1000)      967 2023-04-26 02:08:49.310635 soscucu-0.1.0/PKG-INFO
--rw-rw-r--   0 lee       (1000) lee       (1000)      209 2023-04-26 01:23:06.000000 soscucu-0.1.0/README.md
--rw-rw-r--   0 lee       (1000) lee       (1000)       38 2023-04-26 02:08:49.310635 soscucu-0.1.0/setup.cfg
--rw-rw-r--   0 lee       (1000) lee       (1000)      948 2023-04-26 02:08:47.000000 soscucu-0.1.0/setup.py
-drwxrwxr-x   0 lee       (1000) lee       (1000)        0 2023-04-26 02:08:49.310635 soscucu-0.1.0/soscucu.egg-info/
--rw-rw-r--   0 lee       (1000) lee       (1000)      967 2023-04-26 02:08:49.000000 soscucu-0.1.0/soscucu.egg-info/PKG-INFO
--rw-rw-r--   0 lee       (1000) lee       (1000)      142 2023-04-26 02:08:49.000000 soscucu-0.1.0/soscucu.egg-info/SOURCES.txt
--rw-rw-r--   0 lee       (1000) lee       (1000)        1 2023-04-26 02:08:49.000000 soscucu-0.1.0/soscucu.egg-info/dependency_links.txt
--rw-rw-r--   0 lee       (1000) lee       (1000)        1 2023-04-26 02:08:49.000000 soscucu-0.1.0/soscucu.egg-info/top_level.txt
+drwxrwxr-x   0 lee       (1000) lee       (1000)        0 2023-04-26 02:20:02.644125 soscucu-0.1.1/
+-rw-rw-r--   0 lee       (1000) lee       (1000)      967 2023-04-26 02:20:02.644125 soscucu-0.1.1/PKG-INFO
+-rw-rw-r--   0 lee       (1000) lee       (1000)      209 2023-04-26 01:23:06.000000 soscucu-0.1.1/README.md
+-rw-rw-r--   0 lee       (1000) lee       (1000)       38 2023-04-26 02:20:02.644125 soscucu-0.1.1/setup.cfg
+-rw-rw-r--   0 lee       (1000) lee       (1000)      948 2023-04-26 02:20:00.000000 soscucu-0.1.1/setup.py
+drwxrwxr-x   0 lee       (1000) lee       (1000)        0 2023-04-26 02:20:02.644125 soscucu-0.1.1/soscucu/
+-rw-rw-r--   0 lee       (1000) lee       (1000)        0 2023-04-26 01:21:26.000000 soscucu-0.1.1/soscucu/__init__.py
+-rw-rw-r--   0 lee       (1000) lee       (1000)       36 2023-04-26 01:22:23.000000 soscucu-0.1.1/soscucu/english.py
+-rw-rw-r--   0 lee       (1000) lee       (1000)       38 2023-04-26 01:22:11.000000 soscucu-0.1.1/soscucu/korean.py
+drwxrwxr-x   0 lee       (1000) lee       (1000)        0 2023-04-26 02:20:02.644125 soscucu-0.1.1/soscucu.egg-info/
+-rw-rw-r--   0 lee       (1000) lee       (1000)      967 2023-04-26 02:20:02.000000 soscucu-0.1.1/soscucu.egg-info/PKG-INFO
+-rw-rw-r--   0 lee       (1000) lee       (1000)      199 2023-04-26 02:20:02.000000 soscucu-0.1.1/soscucu.egg-info/SOURCES.txt
+-rw-rw-r--   0 lee       (1000) lee       (1000)        1 2023-04-26 02:20:02.000000 soscucu-0.1.1/soscucu.egg-info/dependency_links.txt
+-rw-rw-r--   0 lee       (1000) lee       (1000)        8 2023-04-26 02:20:02.000000 soscucu-0.1.1/soscucu.egg-info/top_level.txt
```

### Comparing `soscucu-0.1.0/PKG-INFO` & `soscucu-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soscucu
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple greeting package
 Home-page: https://github.com/yourusername/greeting
 Author: Choongin
 Author-email: choongin.lee@kaist.ac.kr
 License: UNKNOWN
 Description: # Greeting Package
```

### Comparing `soscucu-0.1.0/setup.py` & `soscucu-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 # 이전 빌드 파일 삭제
 dist_path = 'dist'
 if os.path.exists(dist_path):
     shutil.rmtree(dist_path)
 setup(
     name="soscucu",
-    version="0.1.0",
+    version="0.1.1",
     packages=find_packages(),
     install_requires=[],
     author="Choongin",
     author_email="choongin.lee@kaist.ac.kr",
     description="A simple greeting package",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
```

### Comparing `soscucu-0.1.0/soscucu.egg-info/PKG-INFO` & `soscucu-0.1.1/soscucu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soscucu
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple greeting package
 Home-page: https://github.com/yourusername/greeting
 Author: Choongin
 Author-email: choongin.lee@kaist.ac.kr
 License: UNKNOWN
 Description: # Greeting Package
```

