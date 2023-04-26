# Comparing `tmp/pqv-0.3.0.tar.gz` & `tmp/pqv-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pqv-0.3.0.tar", last modified: Wed Mar 15 14:24:11 2023, max compression
+gzip compressed data, was "pqv-0.4.0.tar", last modified: Wed Apr 26 19:47:22 2023, max compression
```

## Comparing `pqv-0.3.0.tar` & `pqv-0.4.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 pieter     (501) staff       (20)        0 2023-03-15 14:24:11.167775 pqv-0.3.0/
--rw-r--r--   0 pieter     (501) staff       (20)     1066 2023-02-26 14:17:55.000000 pqv-0.3.0/LICENSE
--rw-r--r--   0 pieter     (501) staff       (20)      225 2023-03-15 14:24:11.167575 pqv-0.3.0/PKG-INFO
--rw-r--r--   0 pieter     (501) staff       (20)      102 2023-02-26 14:42:52.000000 pqv-0.3.0/README.md
-drwxr-xr-x   0 pieter     (501) staff       (20)        0 2023-03-15 14:24:11.165715 pqv-0.3.0/pqv/
--rw-r--r--   0 pieter     (501) staff       (20)        0 2023-02-26 14:09:31.000000 pqv-0.3.0/pqv/__init__.py
--rw-r--r--   0 pieter     (501) staff       (20)     3698 2023-03-15 14:21:49.000000 pqv-0.3.0/pqv/__main__.py
--rw-r--r--   0 pieter     (501) staff       (20)      165 2023-02-26 11:16:27.000000 pqv-0.3.0/pqv/style.css
-drwxr-xr-x   0 pieter     (501) staff       (20)        0 2023-03-15 14:24:11.167299 pqv-0.3.0/pqv.egg-info/
--rw-r--r--   0 pieter     (501) staff       (20)      225 2023-03-15 14:24:11.000000 pqv-0.3.0/pqv.egg-info/PKG-INFO
--rw-r--r--   0 pieter     (501) staff       (20)      236 2023-03-15 14:24:11.000000 pqv-0.3.0/pqv.egg-info/SOURCES.txt
--rw-r--r--   0 pieter     (501) staff       (20)        1 2023-03-15 14:24:11.000000 pqv-0.3.0/pqv.egg-info/dependency_links.txt
--rw-r--r--   0 pieter     (501) staff       (20)       42 2023-03-15 14:24:11.000000 pqv-0.3.0/pqv.egg-info/entry_points.txt
--rw-r--r--   0 pieter     (501) staff       (20)        1 2023-02-26 14:19:07.000000 pqv-0.3.0/pqv.egg-info/not-zip-safe
--rw-r--r--   0 pieter     (501) staff       (20)        4 2023-03-15 14:24:11.000000 pqv-0.3.0/pqv.egg-info/top_level.txt
--rw-r--r--   0 pieter     (501) staff       (20)       38 2023-03-15 14:24:11.167830 pqv-0.3.0/setup.cfg
--rw-r--r--   0 pieter     (501) staff       (20)      529 2023-03-15 14:07:55.000000 pqv-0.3.0/setup.py
+drwxr-xr-x   0 pieter     (501) staff       (20)        0 2023-04-26 19:47:22.797957 pqv-0.4.0/
+-rw-r--r--   0 pieter     (501) staff       (20)     1066 2023-02-26 14:17:55.000000 pqv-0.4.0/LICENSE
+-rw-r--r--   0 pieter     (501) staff       (20)      225 2023-04-26 19:47:22.797748 pqv-0.4.0/PKG-INFO
+-rw-r--r--   0 pieter     (501) staff       (20)      102 2023-02-26 14:42:52.000000 pqv-0.4.0/README.md
+drwxr-xr-x   0 pieter     (501) staff       (20)        0 2023-04-26 19:47:22.795623 pqv-0.4.0/pqv/
+-rw-r--r--   0 pieter     (501) staff       (20)        0 2023-02-26 14:09:31.000000 pqv-0.4.0/pqv/__init__.py
+-rw-r--r--   0 pieter     (501) staff       (20)     3905 2023-04-26 19:43:56.000000 pqv-0.4.0/pqv/__main__.py
+-rw-r--r--   0 pieter     (501) staff       (20)      165 2023-02-26 11:16:27.000000 pqv-0.4.0/pqv/style.css
+drwxr-xr-x   0 pieter     (501) staff       (20)        0 2023-04-26 19:47:22.797468 pqv-0.4.0/pqv.egg-info/
+-rw-r--r--   0 pieter     (501) staff       (20)      225 2023-04-26 19:47:22.000000 pqv-0.4.0/pqv.egg-info/PKG-INFO
+-rw-r--r--   0 pieter     (501) staff       (20)      236 2023-04-26 19:47:22.000000 pqv-0.4.0/pqv.egg-info/SOURCES.txt
+-rw-r--r--   0 pieter     (501) staff       (20)        1 2023-04-26 19:47:22.000000 pqv-0.4.0/pqv.egg-info/dependency_links.txt
+-rw-r--r--   0 pieter     (501) staff       (20)       42 2023-04-26 19:47:22.000000 pqv-0.4.0/pqv.egg-info/entry_points.txt
+-rw-r--r--   0 pieter     (501) staff       (20)        1 2023-02-26 14:19:07.000000 pqv-0.4.0/pqv.egg-info/not-zip-safe
+-rw-r--r--   0 pieter     (501) staff       (20)        4 2023-04-26 19:47:22.000000 pqv-0.4.0/pqv.egg-info/top_level.txt
+-rw-r--r--   0 pieter     (501) staff       (20)       38 2023-04-26 19:47:22.798114 pqv-0.4.0/setup.cfg
+-rw-r--r--   0 pieter     (501) staff       (20)      529 2023-04-26 19:44:38.000000 pqv-0.4.0/setup.py
```

### Comparing `pqv-0.3.0/LICENSE` & `pqv-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pqv-0.3.0/pqv/__main__.py` & `pqv-0.4.0/pqv/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -92,15 +92,20 @@
 
     def on_mount(self) -> None:
         self.group = None
         self.group_index = 0
         self.group_offset = 0
         self.row_index = 0
         self.file_path = sys.argv[1]
-        self.parquet_file = ParquetFile(os.path.expanduser(self.file_path))
+        if not os.path.isfile(self.file_path):
+            sys.exit(f"No such file: {self.file_path}")
+        try:
+            self.parquet_file = ParquetFile(os.path.expanduser(self.file_path))
+        except Exception:
+            sys.exit(f"Error reading file {self.file_path}")
         self.schema = None
         self.update_group()
         self.show_row()
 
 
 def main():
     app = ParquetApp()
```

### Comparing `pqv-0.3.0/setup.py` & `pqv-0.4.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name="pqv",
-    version="0.3.0",
+    version="0.4.0",
     author="Pieter Provoost",
     author_email="pieterprovoost@gmail.com",
     description="Simple parquet viewer",
     url="https://github.com/pieterprovoost/pqv",
     license="MIT",
     packages=find_packages(),
     include_package_data=True,
```

