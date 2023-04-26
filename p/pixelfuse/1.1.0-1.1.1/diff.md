# Comparing `tmp/pixelfuse-1.1.0.tar.gz` & `tmp/pixelfuse-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pixelfuse-1.1.0.tar", max compression
+gzip compressed data, was "pixelfuse-1.1.1.tar", max compression
```

## Comparing `pixelfuse-1.1.0.tar` & `pixelfuse-1.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    35149 2023-04-25 16:54:34.881297 pixelfuse-1.1.0/LICENSE
--rw-r--r--   0        0        0      314 2023-04-25 16:54:34.881297 pixelfuse-1.1.0/README.md
--rw-r--r--   0        0        0      116 2023-04-25 16:54:34.881297 pixelfuse-1.1.0/pixelfuse/__init__.py
--rw-r--r--   0        0        0      112 2023-04-25 16:54:34.881297 pixelfuse-1.1.0/pixelfuse/__main__.py
--rw-r--r--   0        0        0     1346 2023-04-25 16:54:34.881297 pixelfuse-1.1.0/pixelfuse/cli.py
--rw-r--r--   0        0        0     3541 2023-04-25 16:54:34.881297 pixelfuse-1.1.0/pixelfuse/src/f2v.py
--rw-r--r--   0        0        0     2098 2023-04-25 16:54:34.881297 pixelfuse-1.1.0/pixelfuse/src/old_files/d_v1.py
--rw-r--r--   0        0        0     2995 2023-04-25 16:54:34.881297 pixelfuse-1.1.0/pixelfuse/src/v2f.py
--rw-r--r--   0        0        0      667 2023-04-25 16:54:34.881297 pixelfuse-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     1141 1970-01-01 00:00:00.000000 pixelfuse-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-26 08:40:56.424840 pixelfuse-1.1.1/LICENSE
+-rw-r--r--   0        0        0     3202 2023-04-26 08:40:56.424840 pixelfuse-1.1.1/README.md
+-rw-r--r--   0        0        0      116 2023-04-26 08:40:56.424840 pixelfuse-1.1.1/pixelfuse/__init__.py
+-rw-r--r--   0        0        0      112 2023-04-26 08:40:56.424840 pixelfuse-1.1.1/pixelfuse/__main__.py
+-rw-r--r--   0        0        0     1346 2023-04-26 08:40:56.424840 pixelfuse-1.1.1/pixelfuse/cli.py
+-rw-r--r--   0        0        0     3541 2023-04-26 08:40:56.424840 pixelfuse-1.1.1/pixelfuse/src/f2v.py
+-rw-r--r--   0        0        0     2098 2023-04-26 08:40:56.424840 pixelfuse-1.1.1/pixelfuse/src/old_files/d_v1.py
+-rw-r--r--   0        0        0     2995 2023-04-26 08:40:56.424840 pixelfuse-1.1.1/pixelfuse/src/v2f.py
+-rw-r--r--   0        0        0      667 2023-04-26 08:40:56.428840 pixelfuse-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4029 1970-01-01 00:00:00.000000 pixelfuse-1.1.1/PKG-INFO
```

### Comparing `pixelfuse-1.1.0/LICENSE` & `pixelfuse-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pixelfuse-1.1.0/pixelfuse/cli.py` & `pixelfuse-1.1.1/pixelfuse/cli.py`

 * *Files identical despite different names*

### Comparing `pixelfuse-1.1.0/pixelfuse/src/f2v.py` & `pixelfuse-1.1.1/pixelfuse/src/f2v.py`

 * *Files identical despite different names*

### Comparing `pixelfuse-1.1.0/pixelfuse/src/old_files/d_v1.py` & `pixelfuse-1.1.1/pixelfuse/src/old_files/d_v1.py`

 * *Files identical despite different names*

### Comparing `pixelfuse-1.1.0/pixelfuse/src/v2f.py` & `pixelfuse-1.1.1/pixelfuse/src/v2f.py`

 * *Files identical despite different names*

### Comparing `pixelfuse-1.1.0/pyproject.toml` & `pixelfuse-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pixelfuse"
-version = "1.1.0"
+version = "1.1.1"
 description = "Convert any file to video and video to file"
 authors = ["Roman <romantovt31@gmail.com>"]
 license = "GPL-3.0"
 readme = "README.md"
 homepage = "https://github.com/TheTS-labs/PixelFuse"
 repository = "https://github.com/TheTS-labs/PixelFuse"
 keywords = ["video", "file", "converter"]
```

