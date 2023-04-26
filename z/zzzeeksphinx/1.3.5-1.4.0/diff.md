# Comparing `tmp/zzzeeksphinx-1.3.5.tar.gz` & `tmp/zzzeeksphinx-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zzzeeksphinx-1.3.5.tar", last modified: Wed Jun 22 17:01:56 2022, max compression
+gzip compressed data, was "zzzeeksphinx-1.4.0.tar", last modified: Tue Apr 25 23:30:03 2023, max compression
```

## Comparing `zzzeeksphinx-1.3.5.tar` & `zzzeeksphinx-1.4.0.tar`

### file list

```diff
@@ -1,51 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 17:01:56.102243 zzzeeksphinx-1.3.5/
--rw-r--r--   0 runner    (1001) docker     (121)     1133 2022-06-22 17:01:49.000000 zzzeeksphinx-1.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-06-22 17:01:49.000000 zzzeeksphinx-1.3.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3713 2022-06-22 17:01:56.102243 zzzeeksphinx-1.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3219 2022-06-22 17:01:49.000000 zzzeeksphinx-1.3.5/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      323 2022-06-22 17:01:56.102243 zzzeeksphinx-1.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1415 2022-06-22 17:01:49.000000 zzzeeksphinx-1.3.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 17:01:56.098243 zzzeeksphinx-1.3.5/zzzeeksphinx/
--rw-r--r--   0 runner    (1001) docker     (121)      552 2022-06-22 17:01:49.000000 zzzeeksphinx-1.3.5/zzzeeksphinx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13742 2022-06-22 17:01:49.000000 zzzeeksphinx-1.3.5/zzzeeksphinx/autodoc_mods.py
--rw-r--r--   0 runner    (1001) docker     (121)    12148 2022-06-22 17:01:49.000000 zzzeeksphinx-1.3.5/zzzeeksphinx/dialect_info.py
--rw-r--r--   0 runner    (1001) docker     (121)     1885 2022-06-22 17:01:49.000000 zzzeeksphinx-1.3.5/zzzeeksphinx/extras.py
--rw-r--r--   0 runner    (1001) docker     (121)     4391 2022-06-22 17:01:49.000000 zzzeeksphinx-1.3.5/zzzeeksphinx/mako.py
--rw-r--r--   0 runner    (1001) docker     (121)     2662 2022-06-22 17:01:49.000000 zzzeeksphinx-1.3.5/zzzeeksphinx/render_pydomains.py
--rw-r--r--   0 runner    (1001) docker     (121)     2073 2022-06-22 17:01:49.000000 zzzeeksphinx-1.3.5/zzzeeksphinx/scss.py
--rw-r--r--   0 runner    (1001) docker     (121)     4937 2022-06-22 17:01:49.000000 zzzeeksphinx-1.3.5/zzzeeksphinx/sqlformatter.py
--rw-r--r--   0 runner    (1001) docker     (121)      440 2022-06-22 17:01:49.000000 zzzeeksphinx-1.3.5/zzzeeksphinx/theme.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 17:01:56.094243 zzzeeksphinx-1.3.5/zzzeeksphinx/themes/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 17:01:56.102243 zzzeeksphinx-1.3.5/zzzeeksphinx/themes/zsbase/
--rw-r--r--   0 runner    (1001) docker     (121)     1891 2022-06-22 17:01:49.000000 zzzeeksphinx-1.3.5/zzzeeksphinx/themes/zsbase/genindex.mako
--rw-r--r--   0 runner    (1001) docker     (121)    10020 2022-06-22 17:01:49.000000 zzzeeksphinx-1.3.5/zzzeeksphinx/themes/zsbase/layout.mako
--rw-r--r--   0 runner    (1001) docker     (121)      289 2022-06-22 17:01:49.000000 zzzeeksphinx-1.3.5/zzzeeksphinx/themes/zsbase/notfound.mako
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-06-22 17:01:49.000000 zzzeeksphinx-1.3.5/zzzeeksphinx/themes/zsbase/page.mako
--rw-r--r--   0 runner    (1001) docker     (121)      401 2022-06-22 17:01:49.000000 zzzeeksphinx-1.3.5/zzzeeksphinx/themes/zsbase/search.mako
--rw-r--r--   0 runner    (1001) docker     (121)     1073 2022-06-22 17:01:49.000000 zzzeeksphinx-1.3.5/zzzeeksphinx/themes/zsbase/static_base.mako
--rw-r--r--   0 runner    (1001) docker     (121)      102 2022-06-22 17:01:49.000000 zzzeeksphinx-1.3.5/zzzeeksphinx/themes/zsbase/theme.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 17:01:56.102243 zzzeeksphinx-1.3.5/zzzeeksphinx/themes/zsmako/
--rw-r--r--   0 runner    (1001) docker     (121)     6260 2022-06-22 17:01:49.000000 zzzeeksphinx-1.3.5/zzzeeksphinx/themes/zsmako/layout.mako
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 17:01:56.102243 zzzeeksphinx-1.3.5/zzzeeksphinx/themes/zsmako/static/
--rw-r--r--   0 runner    (1001) docker     (121)     7082 2022-06-22 17:01:49.000000 zzzeeksphinx-1.3.5/zzzeeksphinx/themes/zsmako/static/docs.css
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-06-22 17:01:49.000000 zzzeeksphinx-1.3.5/zzzeeksphinx/themes/zsmako/theme.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 17:01:56.102243 zzzeeksphinx-1.3.5/zzzeeksphinx/themes/zzzeeksphinx/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 17:01:56.102243 zzzeeksphinx-1.3.5/zzzeeksphinx/themes/zzzeeksphinx/static/
--rw-r--r--   0 runner    (1001) docker     (121)    11325 2022-06-22 17:01:49.000000 zzzeeksphinx-1.3.5/zzzeeksphinx/themes/zzzeeksphinx/static/deepalchemy.png
--rw-r--r--   0 runner    (1001) docker     (121)    11757 2022-06-22 17:01:49.000000 zzzeeksphinx-1.3.5/zzzeeksphinx/themes/zzzeeksphinx/static/deepalchemy_original.png
--rw-r--r--   0 runner    (1001) docker     (121)    22828 2022-06-22 17:01:49.000000 zzzeeksphinx-1.3.5/zzzeeksphinx/themes/zzzeeksphinx/static/docs.scss
--rw-r--r--   0 runner    (1001) docker     (121)     6372 2022-06-22 17:01:49.000000 zzzeeksphinx-1.3.5/zzzeeksphinx/themes/zzzeeksphinx/static/dragons.png
--rw-r--r--   0 runner    (1001) docker     (121)     5905 2022-06-22 17:01:49.000000 zzzeeksphinx-1.3.5/zzzeeksphinx/themes/zzzeeksphinx/static/dragons_original.png
--rw-r--r--   0 runner    (1001) docker     (121)     4861 2022-06-22 17:01:49.000000 zzzeeksphinx-1.3.5/zzzeeksphinx/themes/zzzeeksphinx/static/init.js
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-06-22 17:01:49.000000 zzzeeksphinx-1.3.5/zzzeeksphinx/themes/zzzeeksphinx/theme.conf
--rw-r--r--   0 runner    (1001) docker     (121)    11269 2022-06-22 17:01:49.000000 zzzeeksphinx-1.3.5/zzzeeksphinx/toc.py
--rw-r--r--   0 runner    (1001) docker     (121)      400 2022-06-22 17:01:49.000000 zzzeeksphinx-1.3.5/zzzeeksphinx/util.py
--rw-r--r--   0 runner    (1001) docker     (121)    11004 2022-06-22 17:01:49.000000 zzzeeksphinx-1.3.5/zzzeeksphinx/viewsource.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 17:01:56.098243 zzzeeksphinx-1.3.5/zzzeeksphinx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3713 2022-06-22 17:01:56.000000 zzzeeksphinx-1.3.5/zzzeeksphinx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1377 2022-06-22 17:01:56.000000 zzzeeksphinx-1.3.5/zzzeeksphinx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-22 17:01:56.000000 zzzeeksphinx-1.3.5/zzzeeksphinx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      245 2022-06-22 17:01:56.000000 zzzeeksphinx-1.3.5/zzzeeksphinx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-22 17:01:56.000000 zzzeeksphinx-1.3.5/zzzeeksphinx.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-06-22 17:01:56.000000 zzzeeksphinx-1.3.5/zzzeeksphinx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-06-22 17:01:56.000000 zzzeeksphinx-1.3.5/zzzeeksphinx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:30:03.421863 zzzeeksphinx-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-25 23:29:57.000000 zzzeeksphinx-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-25 23:29:57.000000 zzzeeksphinx-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-04-25 23:30:03.421863 zzzeeksphinx-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-04-25 23:29:57.000000 zzzeeksphinx-1.4.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-25 23:30:03.421863 zzzeeksphinx-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-04-25 23:29:57.000000 zzzeeksphinx-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:30:03.413863 zzzeeksphinx-1.4.0/zzzeeksphinx/
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-04-25 23:29:57.000000 zzzeeksphinx-1.4.0/zzzeeksphinx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16385 2023-04-25 23:29:57.000000 zzzeeksphinx-1.4.0/zzzeeksphinx/autodoc_mods.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12608 2023-04-25 23:29:57.000000 zzzeeksphinx-1.4.0/zzzeeksphinx/dialect_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-25 23:29:57.000000 zzzeeksphinx-1.4.0/zzzeeksphinx/extras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-04-25 23:29:57.000000 zzzeeksphinx-1.4.0/zzzeeksphinx/mako.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-04-25 23:29:57.000000 zzzeeksphinx-1.4.0/zzzeeksphinx/render_pydomains.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-04-25 23:29:57.000000 zzzeeksphinx-1.4.0/zzzeeksphinx/scss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10527 2023-04-25 23:29:57.000000 zzzeeksphinx-1.4.0/zzzeeksphinx/sqlformatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-25 23:29:57.000000 zzzeeksphinx-1.4.0/zzzeeksphinx/theme.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:30:03.413863 zzzeeksphinx-1.4.0/zzzeeksphinx/themes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:30:03.417863 zzzeeksphinx-1.4.0/zzzeeksphinx/themes/zsbase/
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-04-25 23:29:57.000000 zzzeeksphinx-1.4.0/zzzeeksphinx/themes/zsbase/genindex.mako
+-rw-r--r--   0 runner    (1001) docker     (123)    10119 2023-04-25 23:29:57.000000 zzzeeksphinx-1.4.0/zzzeeksphinx/themes/zsbase/layout.mako
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-25 23:29:57.000000 zzzeeksphinx-1.4.0/zzzeeksphinx/themes/zsbase/notfound.mako
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-25 23:29:57.000000 zzzeeksphinx-1.4.0/zzzeeksphinx/themes/zsbase/page.mako
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-25 23:29:57.000000 zzzeeksphinx-1.4.0/zzzeeksphinx/themes/zsbase/search.mako
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-25 23:29:57.000000 zzzeeksphinx-1.4.0/zzzeeksphinx/themes/zsbase/static_base.mako
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-25 23:29:57.000000 zzzeeksphinx-1.4.0/zzzeeksphinx/themes/zsbase/theme.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:30:03.417863 zzzeeksphinx-1.4.0/zzzeeksphinx/themes/zsmako/
+-rw-r--r--   0 runner    (1001) docker     (123)     6288 2023-04-25 23:29:57.000000 zzzeeksphinx-1.4.0/zzzeeksphinx/themes/zsmako/layout.mako
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:30:03.417863 zzzeeksphinx-1.4.0/zzzeeksphinx/themes/zsmako/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     7177 2023-04-25 23:29:57.000000 zzzeeksphinx-1.4.0/zzzeeksphinx/themes/zsmako/static/docs.css
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-25 23:29:57.000000 zzzeeksphinx-1.4.0/zzzeeksphinx/themes/zsmako/theme.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:30:03.417863 zzzeeksphinx-1.4.0/zzzeeksphinx/themes/zzzeeksphinx/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:30:03.421863 zzzeeksphinx-1.4.0/zzzeeksphinx/themes/zzzeeksphinx/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-04-25 23:29:57.000000 zzzeeksphinx-1.4.0/zzzeeksphinx/themes/zzzeeksphinx/static/annotated.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11325 2023-04-25 23:29:57.000000 zzzeeksphinx-1.4.0/zzzeeksphinx/themes/zzzeeksphinx/static/deepalchemy.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11757 2023-04-25 23:29:57.000000 zzzeeksphinx-1.4.0/zzzeeksphinx/themes/zzzeeksphinx/static/deepalchemy_original.png
+-rw-r--r--   0 runner    (1001) docker     (123)    25027 2023-04-25 23:29:57.000000 zzzeeksphinx-1.4.0/zzzeeksphinx/themes/zzzeeksphinx/static/docs.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-04-25 23:29:57.000000 zzzeeksphinx-1.4.0/zzzeeksphinx/themes/zzzeeksphinx/static/dragons.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5905 2023-04-25 23:29:57.000000 zzzeeksphinx-1.4.0/zzzeeksphinx/themes/zzzeeksphinx/static/dragons_original.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-04-25 23:29:57.000000 zzzeeksphinx-1.4.0/zzzeeksphinx/themes/zzzeeksphinx/static/init.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6080 2023-04-25 23:29:57.000000 zzzeeksphinx-1.4.0/zzzeeksphinx/themes/zzzeeksphinx/static/nonannotated.png
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-25 23:29:57.000000 zzzeeksphinx-1.4.0/zzzeeksphinx/themes/zzzeeksphinx/theme.conf
+-rw-r--r--   0 runner    (1001) docker     (123)    11715 2023-04-25 23:29:57.000000 zzzeeksphinx-1.4.0/zzzeeksphinx/toc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-25 23:29:57.000000 zzzeeksphinx-1.4.0/zzzeeksphinx/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11004 2023-04-25 23:29:57.000000 zzzeeksphinx-1.4.0/zzzeeksphinx/viewsource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:30:03.417863 zzzeeksphinx-1.4.0/zzzeeksphinx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-04-25 23:30:03.000000 zzzeeksphinx-1.4.0/zzzeeksphinx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-04-25 23:30:03.000000 zzzeeksphinx-1.4.0/zzzeeksphinx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 23:30:03.000000 zzzeeksphinx-1.4.0/zzzeeksphinx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-25 23:30:03.000000 zzzeeksphinx-1.4.0/zzzeeksphinx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 23:30:03.000000 zzzeeksphinx-1.4.0/zzzeeksphinx.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-25 23:30:03.000000 zzzeeksphinx-1.4.0/zzzeeksphinx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-25 23:30:03.000000 zzzeeksphinx-1.4.0/zzzeeksphinx.egg-info/top_level.txt
```

### Comparing `zzzeeksphinx-1.3.5/LICENSE` & `zzzeeksphinx-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zzzeeksphinx-1.3.5/PKG-INFO` & `zzzeeksphinx-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zzzeeksphinx
-Version: 1.3.5
+Version: 1.4.0
 Summary: Zzzeek's Sphinx Layout and Utilities.
 Home-page: https://github.com/sqlalchemyorg/zzzeeksphinx
 Author: Mike Bayer
 Author-email: mike@zzzcomputing.com
 License: MIT
 Keywords: Sphinx
 Platform: UNKNOWN
```

### Comparing `zzzeeksphinx-1.3.5/README.rst` & `zzzeeksphinx-1.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `zzzeeksphinx-1.3.5/setup.py` & `zzzeeksphinx-1.4.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,15 +31,21 @@
     ],
     keywords="Sphinx",
     author="Mike Bayer",
     author_email="mike@zzzcomputing.com",
     url="https://github.com/sqlalchemyorg/zzzeeksphinx",
     license="MIT",
     packages=["zzzeeksphinx"],
-    install_requires=["libsass", "mako", "requests", "sphinx>=4.5.0,<5.1"],
+    install_requires=[
+        "libsass",
+        "mako",
+        "requests",
+        "sphinx>=5.3.0,<6.3",
+        "sphinxcontrib-jquery",
+    ],
     include_package_data=True,
     zip_safe=False,
     entry_points={
         "sphinx.html_themes": [
             "zsbase = zzzeeksphinx.theme",
             "zzzeeksphinx = zzzeeksphinx.theme",
             "zsmako = zzzeeksphinx.theme",
```

### Comparing `zzzeeksphinx-1.3.5/zzzeeksphinx/__init__.py` & `zzzeeksphinx-1.4.0/zzzeeksphinx/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,26 @@
-__version__ = "1.3.5"
+__version__ = "1.4.0"
 
 
 def setup(app):
     from . import (
         autodoc_mods,
         dialect_info,
         mako,
         sqlformatter,
         viewsource,
         scss,
         render_pydomains,
         extras,
     )
 
+    # we use jquery.  See
+    # https://www.sphinx-doc.org/en/master/changes.html#id65
+    app.setup_extension("sphinxcontrib.jquery")
+
     autodoc_mods.setup(app)
     dialect_info.setup(app)
     mako.setup(app)
     sqlformatter.setup(app)
     viewsource.setup(app)
     scss.setup(app)
     render_pydomains.setup(app)
```

### Comparing `zzzeeksphinx-1.3.5/zzzeeksphinx/autodoc_mods.py` & `zzzeeksphinx-1.4.0/zzzeeksphinx/autodoc_mods.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,14 +5,23 @@
 from sphinx import addnodes
 from sphinx.util import logging
 
 LOG = logging.getLogger(__name__)
 
 
 def autodoc_skip_member(app, what, name, obj, skip, options):
+    # sphinx is putting blank __init__ methods, not sure why.
+    # even if I turn off all the extensions here
+    if (
+        what == "class"
+        and name == "__init__"
+        and (not inspect.isfunction(obj) or not obj.__doc__)
+    ):
+        return True
+
     if (
         what == "class"
         and skip
         and name
         in ("__init__", "__eq__", "__ne__", "__lt__", "__le__", "__call__")
         and obj.__doc__
         and getattr(obj, "__objclass__", None)
@@ -207,25 +216,88 @@
                     name_node,
                     refid=refid,
                     classes=["reference", "internal"],
                 ),
                 nodes.Text(param_str, param_str),
             )
 
-            row.append(nodes.entry("", p, classes=["nowrap"]))
+            row.append(nodes.entry("", p, classes=["autosummary-name"]))
             try:
                 para = ad_node[1][0]
                 if isinstance(para, nodes.paragraph):
                     text = para.deepcopy()
                 else:
                     text = nodes.Text("", "")
             except IndexError:
                 text = nodes.Text("", "")
 
-            row.append(nodes.entry("", text))
+            if ad_node.attributes.get("objtype") == "class":
+                member_nodes = []
+
+                for attr_desc in ad_node.traverse(addnodes.desc):
+                    objtype = attr_desc.attributes.get("objtype")
+                    if objtype not in ("classmethod", "method", "attribute"):
+                        continue
+
+                    attr_sig = attr_desc.children[0]
+
+                    attr_ids = attr_sig.attributes.get("ids", [None])
+                    if not attr_ids:
+                        continue
+
+                    attr_ref_id = attr_ids[0]
+                    if not attr_ref_id:
+                        continue
+
+                    attr_name_node = list(
+                        attr_desc.traverse(addnodes.desc_name)
+                    )[0]
+                    attr_name_node = attr_name_node.deepcopy()
+
+                    if objtype in ("classmethod", "method"):
+                        attr_name_node.append(nodes.Text("()"))
+
+                    attr_ref = nodes.reference(
+                        "",
+                        "",
+                        attr_name_node,
+                        refid=attr_ref_id,
+                        classes=["reference", "internal"],
+                    )
+
+                    member_nodes.append(attr_ref)
+
+                if member_nodes:
+                    method_list = nodes.paragraph("", "", member_nodes[0])
+
+                    for ref in member_nodes[1:]:
+                        method_list.append(nodes.Text(", "))
+                        method_list.append(ref)
+
+                    method_box = nodes.container(
+                        "",
+                        nodes.paragraph(
+                            "", "", nodes.strong("", nodes.Text("Members"))
+                        ),
+                        method_list,
+                        classes=["class-members"],
+                    )
+
+                    content = ad_node.traverse(addnodes.desc_content)
+                    if content:
+                        content = list(content)[0]
+                        for i, n in enumerate(content.children):
+                            if isinstance(n, (addnodes.index, addnodes.desc)):
+                                content.insert(i - 1, method_box)
+                                break
+
+            entry = nodes.entry("", text)
+
+            row.append(entry)
+
             body.append(row)
 
         if where > 0:
             node.insert(where, table)
 
 
 def fix_up_autodoc_headers(app, doctree):
@@ -300,15 +372,15 @@
         return (signature, return_annotation)
 
 
 def autodoc_process_docstring(app, what, name, obj, options, lines):
     # skipping superclass classlevel docs for now, as these
     # get in the way of using autosummary.
 
-    if what == "class":
+    if what in ("class", "exception"):
         _track_autodoced[name] = obj
 
         # need to translate module names for bases, others
         # as we document lots of symbols in namespace modules
         # outside of their source
         bases = []
         try:
@@ -356,15 +428,15 @@
             if clsname in _track_autodoced:
                 cls = _track_autodoced[clsname]
                 found = False
                 for supercls in cls.__mro__:
                     if attrname in supercls.__dict__:
                         found = True
                         break
-                if found and supercls is not cls:
+                if found and supercls is not cls and supercls is not object:
                     adjusted_mod = _adjust_rendered_mod_name(
                         app.env.config, supercls.__module__, supercls.__name__
                     )
 
                     _inherited_names.add(
                         "%s.%s" % (adjusted_mod, supercls.__name__)
                     )
```

### Comparing `zzzeeksphinx-1.3.5/zzzeeksphinx/dialect_info.py` & `zzzeeksphinx-1.4.0/zzzeeksphinx/dialect_info.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,15 +43,26 @@
                 "directive has been established" % dialect_name
             )
 
         output = []
 
         content = self._parse_content()
 
-        parent_section_ref = self.state.parent.children[0]["ids"][0]
+        # in sphinx 5.1.1 and earlier, we did this:
+        # old_parent_section_ref = self.state.parent.children[0]["ids"][0]
+
+        # however in 5.3.0, parent is an empty section.  not clear if this is
+        # due to content changes or changes in how automodule works, etc.
+        # so now we manufacture it as follows:
+        parent_section_ref = (
+            f"module-sqlalchemy.dialects.{dialect_name}.{dbapi_name}"
+        )
+        # if automodule's naming scheme changes etc., this would silently
+        # break
+
         self._append_dbapi_bullet(
             dialect_name, dbapi_name, content["name"], parent_section_ref
         )
 
         p = nodes.paragraph(
             "",
             "",
```

### Comparing `zzzeeksphinx-1.3.5/zzzeeksphinx/extras.py` & `zzzeeksphinx-1.4.0/zzzeeksphinx/extras.py`

 * *Files 17% similar despite different names*

```diff
@@ -18,14 +18,24 @@
 
 class DeepAlchemy(BaseAdmonition):
 
     required_arguments = 0
     node_class = deepalchemy
 
 
+class legacy(Admonition, Element):
+    pass
+
+
+class Legacy(BaseAdmonition):
+
+    required_arguments = 0
+    node_class = legacy
+
+
 class FooterTopic(Topic):
 
     node_class = footer_topic
 
 
 def visit_footer_topic(self, node):
     self.visit_topic(node)
@@ -35,55 +45,60 @@
     self.depart_topic(node)
 
 
 def visit_deepalchemy(self, node):
     self.visit_admonition(node, "deepalchemy")
 
 
-def depart_deepalchemy(self, node):
+def visit_legacy(self, node):
+    self.visit_admonition(node, "legacy")
+
+
+def depart_admonition(self, node):
     self.depart_admonition(node)
 
 
-deepalchemy_visit = (visit_deepalchemy, depart_deepalchemy)
+deepalchemy_visit = (visit_deepalchemy, depart_admonition)
+
+legacy_visit = (visit_legacy, depart_admonition)
 
 footer_topic_visit = (visit_footer_topic, depart_footer_topic)
 
 
 def move_footer(app, doctree):
 
     if doctree.traverse(footer_topic):
         dec = nodes.decoration()
         doctree.append(dec)
         for f1 in doctree.traverse(footer_topic):
             dec.append(f1.deepcopy())
             f1.parent.remove(f1)
 
 
-def setup(app):
+visit_keys = [
+    "html",
+    "html5",
+    "latex",
+    "text",
+    "xml",
+    "texinfo",
+    "manpage",
+]
 
-    admonitionlabels["deepalchemy"] = _("Deep Alchemy")
 
-    app.add_directive("deepalchemy", DeepAlchemy)
+def setup(app):
 
     app.add_directive("footer_topic", FooterTopic)
 
-    app.add_node(
-        deepalchemy,
-        **{
-            key: deepalchemy_visit
-            for key in [
-                "html",
-                "html5",
-                "latex",
-                "text",
-                "xml",
-                "texinfo",
-                "manpage",
-            ]
-        }
-    )
+    admonitionlabels["deepalchemy"] = _("Deep Alchemy")
+    app.add_directive("deepalchemy", DeepAlchemy)
+    app.add_node(deepalchemy, **{key: deepalchemy_visit for key in visit_keys})
+
+    admonitionlabels["legacy"] = _("Legacy Feature")
+    app.add_directive("legacy", Legacy)
+    app.add_node(legacy, **{key: legacy_visit for key in visit_keys})
 
     app.add_node(
         footer_topic, **{key: footer_topic_visit for key in ["html", "html5"]}
     )
 
     app.connect("doctree-read", move_footer)
```

### Comparing `zzzeeksphinx-1.3.5/zzzeeksphinx/mako.py` & `zzzeeksphinx-1.4.0/zzzeeksphinx/mako.py`

 * *Files identical despite different names*

### Comparing `zzzeeksphinx-1.3.5/zzzeeksphinx/render_pydomains.py` & `zzzeeksphinx-1.4.0/zzzeeksphinx/render_pydomains.py`

 * *Files identical despite different names*

### Comparing `zzzeeksphinx-1.3.5/zzzeeksphinx/scss.py` & `zzzeeksphinx-1.4.0/zzzeeksphinx/scss.py`

 * *Files identical despite different names*

### Comparing `zzzeeksphinx-1.3.5/zzzeeksphinx/themes/zsbase/genindex.mako` & `zzzeeksphinx-1.4.0/zzzeeksphinx/themes/zsbase/genindex.mako`

 * *Files identical despite different names*

### Comparing `zzzeeksphinx-1.3.5/zzzeeksphinx/themes/zsbase/layout.mako` & `zzzeeksphinx-1.4.0/zzzeeksphinx/themes/zsbase/layout.mako`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 ## coding: utf-8
 
 <%!
+    import datetime
+
     local_script_files = []
 
     default_css_files = [
         '_static/pygments.css',
     ]
 %>
 
@@ -300,14 +302,17 @@
 
 
     <p><b>flambé!</b> the dragon and <b><i>The Alchemist</i></b> image designs created and generously donated by <a href="https://github.com/vmalloc">Rotem Yaari</a>.</p>
 
     % if show_sphinx:
         Created using <a href="http://sphinx.pocoo.org/">Sphinx</a> ${sphinx_version|h}.
     % endif
+
+    Documentation last generated: ${datetime.datetime.now().strftime("%c")}
+
     </div>
 </div>
 
 </div>
 
 <%block name="lower_scripts">
```

#### html2text {}

```diff
@@ -1,13 +1,14 @@
-## coding: utf-8 <%! local_script_files = [] default_css_files = [ '_static/
-pygments.css', ] %> <%doc> Structural elements are all prefixed with "docs-" to
-prevent conflicts when the structure is integrated into the main site. docs-
-container -> docs-top-navigation-container -> docs-header -> docs-version-
-header docs-top-navigation docs-top-page-control docs-navigation-banner docs-
-body-container -> docs-sidebar docs-body docs-bottom-navigation docs-copyright
+## coding: utf-8 <%! import datetime local_script_files = [] default_css_files
+= [ '_static/pygments.css', ] %> <%doc> Structural elements are all prefixed
+with "docs-" to prevent conflicts when the structure is integrated into the
+main site. docs-container -> docs-top-navigation-container -> docs-header -
+> docs-version-header docs-top-navigation docs-top-page-control docs-
+navigation-banner docs-body-container -> docs-sidebar docs-body docs-bottom-
+navigation docs-copyright
 doc> <%inherit file="${context['base']}"/> <% if builder == 'epub': next.body()
 return %> <% withsidebar = bool(toc) and ( theme_index_sidebar is True or
 current_page_name != 'index' ) %> <%block name="head_title"> % if
 theme_index_sidebar or current_page_name != 'index': ${capture(self.show_title)
 | util.striptags} — % endif ${docstitle|h}
 block> <%def name="show_title()"> ${title}
 def>
@@ -76,12 +77,13 @@
 % if prevtopic: Previous: ${prevtopic['title']} % endif % if nexttopic: Next: $
 {nexttopic['title']} % endif
 % if hasdoc('copyright'): © Copyright ${copyright|h}. % else: © Copyright $
 {copyright|h}. % endif
 flambÃ©! the dragon and The Alchemist image designs created and generously
 donated by Rotem_Yaari.
 % if show_sphinx: Created using Sphinx ${sphinx_version|h}. % endif
+Documentation last generated: ${datetime.datetime.now().strftime("%c")}
 <%block name="lower_scripts">
   % for scriptfile in script_files + self.attr.local_script_files:
  % endfor
 
 block>
```

### Comparing `zzzeeksphinx-1.3.5/zzzeeksphinx/themes/zsbase/static_base.mako` & `zzzeeksphinx-1.4.0/zzzeeksphinx/themes/zsbase/static_base.mako`

 * *Files identical despite different names*

### Comparing `zzzeeksphinx-1.3.5/zzzeeksphinx/themes/zsmako/layout.mako` & `zzzeeksphinx-1.4.0/zzzeeksphinx/themes/zsmako/layout.mako`

 * *Files 1% similar despite different names*

```diff
@@ -135,15 +135,15 @@
 
     <div id="docs-sidebar">
     <div id="sidebar-banner">
         ${self.bannerad()}
     </div>
 
     <h3><a href="${pathto('index')}">Table of Contents</a></h3>
-    ${toc}
+    <div id="sidebar-toc">${toc}</div>
 
     % if prevtopic:
     <h4>Previous Topic</h4>
     <p>
     <a href="${prevtopic['link']|h}" title="${_('previous chapter')}">${prevtopic['title']}</a>
     </p>
     % endif
```

#### html2text {}

```diff
@@ -32,15 +32,16 @@
 ${docstitle|h} % if parents: % for parent in parents: Â» ${parent['title']} %
 endfor % endif % if current_page_name != 'index': Â» ${self.show_title()} %
 endif
 ***** <%block name="show_title"> ${title} block> *****
 % if withsidebar:
 ${self.bannerad()}
 **** Table_of_Contents ****
-${toc} % if prevtopic:
+${toc}
+% if prevtopic:
 *** Previous Topic ***
 ${prevtopic['title']}
 % endif % if nexttopic:
 *** Next Topic ***
 ${nexttopic['title']}
 % endif
 *** Quick Search ***
```

### Comparing `zzzeeksphinx-1.3.5/zzzeeksphinx/themes/zsmako/static/docs.css` & `zzzeeksphinx-1.4.0/zzzeeksphinx/themes/zsmako/static/docs.css`

 * *Files 1% similar despite different names*

```diff
@@ -166,29 +166,33 @@
 
 #docs-sidebar > ul {
   font-size:.9em;
 }
 
 #docs-sidebar {
   float:left;
-  width:212px;
+  width:237px;
   padding: 10px 0 0 15px;
   /*font-size:.85em;*/
 }
 
+#docs-sidebar #sidebar-toc {
+    overflow:auto;
+}
+
 #docs-sidebar h3, #docs-sidebar h4 {
     background-color: #DDDDDD;
     color: #222222;
     font-family: Tahoma, Geneva,sans-serif;
     font-size: 1.1em;
     font-weight: normal;
     margin: 10px 0 0 -15px;
     padding: 5px 10px 5px 10px;
     text-shadow: 1px 1px 0 white;
-    width:210px;
+    width:235px;
 }
 
 #docs-sidebar h3 a, #docs-sidebar h4 a {
   color: #222222;
 }
 #docs-sidebar ul {
   margin: 10px 10px 10px 0px;
@@ -206,15 +210,15 @@
 
 #docs-body {
   background-color:#FFFFFF;
   padding:1px 10px 10px 10px;
 }
 
 #docs-body.withsidebar {
-  margin: 0 0 0 230px;
+  margin: 0 0 0 255px;
   border-left:3px solid #DFDFDF;
 }
 
 #docs-body h1,
 #docs-body h2,
 #docs-body h3,
 #docs-body h4 {
@@ -259,22 +263,26 @@
   line-height:1.3em;
 }
 
 #docs-container #fixed-sidebar {
   border-bottom: 1px solid;
 }
 
-.popup_sql, .show_sql
+.popup_sql, .show_sql, .show_sql_print
 {
-    background-color: #FBFBEE;
     padding:5px 10px;
     margin:10px -5px;
     border:1px dashed;
 }
 
+.popup_sql, .show_sql
+{
+    background-color: #FBFBEE;
+}
+
 /* the [SQL] links used to display SQL */
 #docs-container .sql_link
 {
   font-weight:normal;
   font-family: arial, sans-serif;
   font-size:.9em;
   text-transform: uppercase;
```

### Comparing `zzzeeksphinx-1.3.5/zzzeeksphinx/themes/zzzeeksphinx/static/deepalchemy.png` & `zzzeeksphinx-1.4.0/zzzeeksphinx/themes/zzzeeksphinx/static/deepalchemy.png`

 * *Files identical despite different names*

### Comparing `zzzeeksphinx-1.3.5/zzzeeksphinx/themes/zzzeeksphinx/static/deepalchemy_original.png` & `zzzeeksphinx-1.4.0/zzzeeksphinx/themes/zzzeeksphinx/static/deepalchemy_original.png`

 * *Files identical despite different names*

### Comparing `zzzeeksphinx-1.3.5/zzzeeksphinx/themes/zzzeeksphinx/static/docs.scss` & `zzzeeksphinx-1.4.0/zzzeeksphinx/themes/zzzeeksphinx/static/docs.scss`

 * *Files 4% similar despite different names*

```diff
@@ -32,61 +32,83 @@
 $primary-font-family: "Libre Franklin", sans-serif;
 $header-font-family: "Libre Franklin", Arial, sans-serif;
 $top-header-font-family: "Libre Franklin", Arial, sans-serif;
 $sidebar-font-family: "Libre Franklin", Verdana, sans-serif;
 
 $narrow-max-screen-width: 980px;
 
-$primary-background-color: #fdfbfc;
 $topmost-header-color: #ebebee;
 $popout-color: #fbfbee;
 $sidebar-color: #efefef;
-$sidebar-header-background-color: #dddddd;
+$sidebar-header-background-color: inherit;
 $sidebar-header-color: #222222;
 $notebox-background-color: #eeffef;
 $code-sig-background-color: #efefef;
 $deprecated-background-color: #fcf0f6;
+$legacy-background-color: #fcffc0;
 $warning-background-color: #fcf0f6;
 $deepalchemy-background-color: #f6e8fd;
 $versionchanged-background-color: #f9f9d9;
+$outer-border-style: none;
 $border-style: 1px solid #ccc;
-$divider-line-style: 1px solid #ccc;
+$index-divider-line-style: 1px solid #ccc;
 
-$box-shadow-style: 2px 2px 3px #dfdfdf;
 $box-top-margin: 10px;
 $box-margin: $box-top-margin 10px 20px 0px;
+
+// this is optimized for the site.  with the vanilla docs, the
+// vertical padding is too much.   not sure how to fix
 $box-padding: 1rem 1em 2px 1rem;
+
+// looks better with vanilla docs but not w/ the site
+// $box-padding: 0 1em 0 1rem;
+
 $box-title-padding: 0 2em 0 1.5em;
 $box-header-color: #c5cec2;
 $box-background-color: #f8f9f0;
 
-$hyperlink-color: #990000;
+// note main text is on top of docs-body-background
+$primary-background-color: #ffffff;
+
+// passes:
+// https://webaim.org/resources/linkcontrastchecker/?fcolor=110000&bcolor=FFFFFF&lcolor=BB0000
+$docs-body-background: #ffffff;
+$text-color: #110000;
+$hyperlink-color: #BB0000;
+$hyperlink-hover-color: #FF0000;
+
+//$spacing-between-outer-boxes: 10px;
+$spacing-between-outer-boxes: 0;
+
 $keyword-color: #480717;
 $keyword-background-color: #f2f2f2;
 
 $highlighted-nav-link-background-color: #ddd;
 $orm-background-color: #e2f3f4;
 $core-background-color: #aecaf7;
 
-$sidebar-popout-height: 160px;
+$sidebar-popout-height: 171px;
 
 $max-container-width: 100em; // 100 * 16 == 1600px;
-$fixed-sidebar-width: 328px;
-$docs-body-sidebar-left: 338px;
+$fixed-sidebar-width: 360px;
+$inner-fixed-sidebar-width: $fixed-sidebar-width - 40px;
+
+$docs-body-sidebar-left: 360px;
+$docs-body-sidebar-horiz-padding: 45px;
 
 /* global */
 
 .body-background {
     background-color: $primary-background-color;
 }
 
 body {
     background-color: $primary-background-color;
     margin: 0 38px;
-    color: #333333;
+    color: $text-color;
 }
 
 blockquote {
     margin-right: inherit;
 }
 
 a {
@@ -106,15 +128,15 @@
 
 a:link,
 a:visited,
 a:active {
     color: $hyperlink-color;
 }
 a:hover {
-    color: #ff0000;
+    color: $hyperlink-hover-color;
     text-decoration: underline;
 }
 
 /* paragraph links after sections.
    These aren't visible until hovering
    over the <h> tag, then have a
    "reverse video" effect over the actual
@@ -138,30 +160,30 @@
     color: white;
 }
 
 /* Container setup */
 
 #docs-container {
     max-width: $max-container-width;
-    margin: 10px auto;
+    margin: $spacing-between-outer-boxes auto;
     position: relative;
     font-size: 120%;
     line-height: 1.4em;
 }
 
 /* header/footer elements */
 
 #docs-header {
     font-family: $primary-font-family;
 
     font-size: 0.9em;
     position: relative;
 
     background-color: $topmost-header-color;
-    border: $border-style;
+    border: $outer-border-style;
     height: 75px;
 
     display: flex;
     align-items: center;
 
     h1 {
         font-size: 20px;
@@ -172,15 +194,15 @@
 
 #docs-sidebar-popout,
 #docs-bottom-navigation,
 #index-nav,
 #narrow-index-nav {
     font-family: $sidebar-font-family;
     background-color: $popout-color;
-    border: $border-style;
+    border: $outer-border-style;
     font-size: 0.8em;
 }
 
 #docs-bottom-navigation,
 #index-nav {
     padding: 10px;
 }
@@ -192,19 +214,19 @@
 }
 
 .docs-navigation-links {
     font-family: $primary-font-family;
 }
 
 #docs-bottom-navigation {
-    margin: 1em 0 1em 0;
+    margin: $spacing-between-outer-boxes 0 $spacing-between-outer-boxes 0;
 }
 
 #docs-bottom-navigation.withsidebar {
-    margin-left: $docs-body-sidebar-left;
+    margin-left: $fixed-sidebar-width;
 }
 
 #docs-copyright {
     font-size: 0.85em;
     padding: 5px 0px;
 }
 
@@ -253,15 +275,15 @@
 
 #docs-body {
     min-height: 700px;
 }
 
 #index-nav {
     position: relative;
-    margin-top: 10px;
+    margin-top: $spacing-between-outer-boxes;
     padding: 10px 10px 25px 10px;
 }
 
 #index-nav form {
     padding-top: 10px;
     float: right;
 }
@@ -278,14 +300,15 @@
 #sidebar-search {
     margin: 10px 0px 10px 0px;
 }
 
 #docs-sidebar {
     top: $sidebar-popout-height + 18px;
     width: $fixed-sidebar-width;
+    margin-right: $fixed-sidebar-width - $inner-fixed-sidebar-width;
     bottom: 0;
     min-height: 0;
     overflow-y: auto;
     overflow-x: hidden;
     margin-top: 5px;
     margin-right: 5px;
     z-index: 3;
@@ -331,21 +354,22 @@
         width: 14em;
         font-size: 1em;
     }
 }
 
 #docs-sidebar-inner {
     padding-left: 10px;
+    margin-right:40px;
     /*width:212px;*/
 
     font-family: $sidebar-font-family;
 
     font-size: 0.85em;
 
-    border: $border-style;
+    border: $outer-border-style;
     background-color: $sidebar-color;
 
     > ul {
         font-size: 0.85em;
     }
 
     span.link-container {
@@ -357,22 +381,23 @@
     }
 
     li.current > span.link-container {
         background-color: $highlighted-nav-link-background-color;
     }
 
     h3,
-    h4 {
+    h4,
+    h5 {
         background-color: $sidebar-header-background-color;
         color: $sidebar-header-color;
         font-family: $sidebar-font-family;
         font-size: 1.1em;
         font-weight: normal;
         margin: 10px 0 0 -15px;
-        padding: 5px 10px 5px 15px;
+        padding: 15px 10px 5px 15px;
         text-shadow: 1px 1px 0 white;
 
         a {
             color: $sidebar-header-color;
         }
     }
 
@@ -423,14 +448,16 @@
     // note that init.js will change this dynamically
     // to "fixed" or "absolute"
     position: absolute;
     float: left;
     width: $fixed-sidebar-width;
     top: 0;
     bottom: 0;
+    background-color: $sidebar-color;
+
 }
 
 #fixed-sidebar #docs-sidebar {
     position: absolute;
 }
 
 #fixed-sidebar #docs-sidebar:after {
@@ -440,24 +467,26 @@
 }
 
 #docs-sidebar {
     position: fixed;
 }
 
 #docs-body {
-    background-color: #ffffff;
-    padding: 1px 10px 10px 10px;
+    background-color: $docs-body-background;
+    padding: 10px 10px 10px 10px;
 
-    border: $border-style;
-    margin-top: 10px;
+    border: $outer-border-style;
+    margin-top: $spacing-between-outer-boxes;
 }
 
 #docs-body.withsidebar {
     margin-left: $docs-body-sidebar-left;
 
+    padding: 10px $docs-body-sidebar-horiz-padding 0 $docs-body-sidebar-horiz-padding;
+
     div.section,
     section {
         /* to limit text width inside the container */
         /*max-width: 1024px;*/
     }
 }
 
@@ -465,23 +494,23 @@
     display: none;
 }
 
 #narrow-index-nav {
     display: none;
 }
 
-/* disable sidebar on narrow screens */
+/* disable sidebar on mobile / narrow screens */
 @media only screen and (max-width: $narrow-max-screen-width) {
     #fixed-sidebar {
         display: none;
     }
     #narrow-index-nav {
         display: block;
         padding: 1rem;
-        margin: 10px 0 10px 0;
+        margin: $spacing-between-outer-boxes 0 $spacing-between-outer-boxes 0;
     }
 
     #docs-body.withsidebar {
         margin-left: 0;
     }
     #docs-bottom-navigation.withsidebar {
         margin-left: 0;
@@ -506,15 +535,15 @@
         left: 8px;
         right: 0;
         bottom: 8px;
     }
 }
 
 #docs-narrow-top-navigation {
-    border: $border-style;
+    border: $outer-border-style;
     background-color: $sidebar-color;
     font-family: $sidebar-font-family;
     font-size: 0.85rem;
 
     h2 {
         margin: 16px 4px 7px 5px;
         font-size: 1.6em;
@@ -524,14 +553,15 @@
     }
 }
 
 #docs-body h1,
 #docs-body h2,
 #docs-body h3,
 #docs-body h4,
+#docs-body h5,
 #docs-body .h2 {
     font-family: $header-font-family;
     font-weight: bold;
     /* don't put a clear:both here. use less floats */
 }
 
 #docs-body {
@@ -543,50 +573,76 @@
 
     h1 {
         font-size: 1.7rem;
     }
 
     h2 {
         font-size: 1.6rem;
-        border-top: $divider-line-style;
+        border-top: $index-divider-line-style;
         padding-top: 20px;
     }
 
     #sqlalchemy-documentation h2 {
         border-top: none;
         padding-top: 0;
     }
     h3 {
         font-size: 1.4rem;
     }
 
     h4 {
         font-size: 1.2rem;
     }
+
+    h5 {
+        font-size: 1.05rem;
+    }
 }
 
 /* SQL popup, code styles */
 
 .highlight {
     background: none;
 }
 
 #docs-container {
     pre {
         font-size: .85rem;
         background-color: #f0f0f0;
         border: $border-style;
-        box-shadow: $box-shadow-style;
         padding: 10px;
         margin: $box-margin;
         overflow: auto;
         line-height: 1.3em;
         clear: both;
     }
 
+    @media only screen and (max-width: ($narrow-max-screen-width + 300)) {
+        pre {
+            padding: 10px 10px 30px 10px;
+        }
+    }
+
+    /* python annotation key */
+    div.code-annotations-key, div.code-non-annotations-key {
+        position:absolute;
+        right:1.2em;
+        bottom:.05em;
+        width: 180px;
+        background-size: 180px;
+        height: 30px;
+    }
+    div.code-annotations-key {
+        background-image: url("annotated.png");
+    }
+    div.code-non-annotations-key {
+        background-image: url("nonannotated.png");
+    }
+
+
     /* the [SQL] links used to display SQL */
     .sql_link {
         font-weight: normal;
         font-family: helvetica, arial, sans-serif;
         font-size: 0.9em;
         text-transform: uppercase;
         color: #990000;
@@ -614,20 +670,24 @@
         font-size: 0.8em;
         padding: 0 4px 0 4px;
         text-decoration: none;
     }
 }
 
 .popup_sql,
-.show_sql {
-    background-color: $popout-color;
+.show_sql,
+.show_sql_print {
     padding: 5px 10px;
-    margin: 10px -5px;
+    margin: 10px -5px 10px -5px;
     border: 1px dashed;
 }
+.popup_sql,
+.show_sql {
+    background-color: $popout-color;
+}
 /* SQL popups are always on at the moment, disable the button */
 .sql_link {
     display: none;
 }
 
 /* tables */
 
@@ -653,14 +713,19 @@
             background-color: transparent;
             vertical-align: middle;
             font-size: 90%;
             margin: 0;
             overflow: visible;
             padding: 8px 16px;
         }
+
+        td.autosummary-name {
+            vertical-align: top;
+        }
+
     }
 
     tr.row-even {
         td {
             background-color: #f3f6f6;
         }
     }
@@ -671,20 +736,22 @@
 th.field-name {
     text-align: right;
     position: absolute;
     padding: 0px;
     margin: 0px;
 }
 
+
 td.field-body {
     padding-top: 1em;
     ul.first {
         padding-left: 17px;
         padding-top: 1em;
     }
+
 }
 
 div.faq {
     background-color: #efefef;
 }
 
 div.faq ul {
@@ -758,20 +825,20 @@
         > p {
             font-size: 0.9em;
         }
 
         padding: 0 20px 0 20px;
         background-color: $box-background-color;
         border: $border-style;
-        box-shadow: $box-shadow-style;
 
         margin: $box-margin;
     }
 }
 
+
 div.sidebar {
     background-color: #ffffee;
     float: right;
     width: 40%;
     margin: 10px 10px 5px 10px;
 }
 
@@ -813,22 +880,27 @@
 }
 
 div.deepalchemy {
     > .admonition-title {
         margin-left: -140px;
     }
     background-image: url("deepalchemy.png");
-    background-position: left top;
+    background-size: auto 100px;
+    background-position: 6px 9px;
     background-repeat: no-repeat;
     background-color: $deepalchemy-background-color;
     clear: right;
-    min-height: 180px;
+    min-height: 120px;
     padding-left: 140px;
 }
 
+div.legacy {
+    background-color: $legacy-background-color;
+}
+
 @media only screen and (max-width: $narrow-max-screen-width) {
     div.note,
     div.warning {
         > .admonition-title {
             margin-left: -14px;
             padding-left: 10px;
         }
@@ -853,29 +925,32 @@
 .versionadded > p:first-child > span:first-child,
 .versionchanged > p:first-child > span:first-child,
 .deprecated > p:first-child > span:first-child {
     color: #990000;
     font-weight: bold;
 }
 
-div.class-bases {
+div.class-bases, div.class-members {
     border: $border-style;
-    box-shadow: $box-shadow-style;
     padding: 5px 5px;
 
     padding: $box-padding;
 
     font-size: 0.9em;
     margin: $box-margin;
+}
+div.class-bases {
     background-color: #eefbfb;
 }
+div.class-members {
+    background-color: #ebedfa;
+}
 
 div.inherited-member {
     border: $border-style;
-    box-shadow: $box-shadow-style;
     padding: 5px 5px;
     font-size: 0.9em;
     background-color: #eefbfb;
 
     p {
         margin: 0;
     }
@@ -889,26 +964,24 @@
 dl.function > dt,
 dl.attribute > dt,
 dl.classmethod > dt,
 dl.method > dt,
 dl.class > dt,
 dl.exception > dt {
     border: $border-style;
-    box-shadow: $box-shadow-style;
     background-color: $code-sig-background-color;
     margin: 25px -10px 10px 10px;
     padding: 8px 10px;
 }
 
 /* parameters / returns lists for functions and methods */
 dl.field-list {
     border-left: $border-style;
     border-right: $border-style;
     border-bottom: $border-style;
-    box-shadow: $box-shadow-style;
     margin: $box-top-margin 10px 0 0;
 
     li > p {
         margin: 0.5em 0 0.5em 0;
     }
 }
 
@@ -1029,50 +1102,64 @@
 }
 div#sqlalchemy-documentation a,
 div#sqlalchemy-documentation li {
     padding: 5px 0px;
 }
 
 div#getting-started {
-    border-bottom: $divider-line-style;
+    border-bottom: $index-divider-line-style;
 }
 
 div#tutorials {
-    border-bottom: $divider-line-style;
+    border-bottom: $index-divider-line-style;
 }
 
 /* new index layout thing */
 
 #docs-body.index {
     padding: 0;
 }
 
 div.left-right-container {
     display: flex;
-    border-bottom: $divider-line-style;
 
+    p.h2 {
+        display: block;
+        font-weight: bold;
+        font-size: 1.4em;
+    }
+
+    .container {
+        border-bottom: $index-divider-line-style;
+        //margin: 0 20px 0 20px;
+        padding-right:10px;
+
+    }
+
+    &:last-of-type {
+        .container {
+            border-bottom: none;
+        }
+    }
     .orm {
         background-color: $orm-background-color;
+        margin-right: 0;
     }
-
     .core {
         background-color: $core-background-color;
-    }
-
-    p.h2 {
-        display: block;
-        font-weight: bold;
-        font-size: 1.4em;
+        margin-left: 0;
     }
 
     .leftmost {
         width: 15em;
         max-width: 15em;
         background-color: #e4e4e8;
         padding-left: 10px;
+        border-bottom: none;
+        margin: 0;
     }
 
     div {
         flex: 3;
         padding-left: 10px;
     }
 }
@@ -1090,14 +1177,15 @@
             max-width: none;
             padding: 10px 10px 10px 10px;
         }
 
         div.container {
             padding-bottom: 1rem;
             max-width: none;
+            margin: 0;
         }
 
         .orm, .core {
             padding-bottom: 1rem;
         }
 
     }
@@ -1118,15 +1206,15 @@
 }
 
 div#sqlalchemy-documentation div#sqlalchemy-orm {
     float: left;
     width: 48%;
     min-height: 400px;
     padding-left: 10px;
-    border-right: $divider-line-style;
+    border-right: $index-divider-line-style;
     h2 {
         margin: 0;
     }
 }
 
 div#sqlalchemy-documentation div#sqlalchemy-core {
     margin: 0;
@@ -1136,15 +1224,15 @@
 
     h2 {
         margin: 0;
     }
 }
 
 div#dialect-documentation {
-    border-top: $divider-line-style;
+    border-top: $index-divider-line-style;
     clear: both;
 }
 
 /* core/orm tabbed thing */
 
 @mixin card-line-style() {
     box-shadow: 0px 0px 2px #ccc;
@@ -1157,15 +1245,16 @@
     }
 }
 
 #docs-body {
     div.orm-core, section.orm-core {
         h2,
         h3,
-        h4 {
+        h4,
+        h5 {
             border: none;
         }
     }
 
     div.orm-header, section.orm-header {
         @include card-line-style();
         border-left: 2.2em solid $orm-background-color;
```

### Comparing `zzzeeksphinx-1.3.5/zzzeeksphinx/themes/zzzeeksphinx/static/dragons.png` & `zzzeeksphinx-1.4.0/zzzeeksphinx/themes/zzzeeksphinx/static/dragons.png`

 * *Files identical despite different names*

### Comparing `zzzeeksphinx-1.3.5/zzzeeksphinx/themes/zzzeeksphinx/static/dragons_original.png` & `zzzeeksphinx-1.4.0/zzzeeksphinx/themes/zzzeeksphinx/static/dragons_original.png`

 * *Files identical despite different names*

### Comparing `zzzeeksphinx-1.3.5/zzzeeksphinx/themes/zzzeeksphinx/static/init.js` & `zzzeeksphinx-1.4.0/zzzeeksphinx/themes/zzzeeksphinx/static/init.js`

 * *Files identical despite different names*

### Comparing `zzzeeksphinx-1.3.5/zzzeeksphinx/toc.py` & `zzzeeksphinx-1.4.0/zzzeeksphinx/toc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 #!coding: utf-8
+import re
 from typing import cast
 
 from docutils import nodes as docutils_nodes
 from sphinx.application import Sphinx
 from sphinx.builders.html import StandaloneHTMLBuilder
 from sphinx.environment.adapters.toctree import TocTree
 
 
+UNDERSCORE_RE = re.compile(r"_\w+\.(.+)$")
+
+
 class TOCMixin:
 
     app: Sphinx
 
     def get_current_subtoc(self, current_page_name, start_from=None):
         """Return a TOC for sub-files and sub-elements of the current file.
 
@@ -250,31 +254,41 @@
                     ] = f"#{the_top_anchor}"
 
         return cast(StandaloneHTMLBuilder, self.app.builder).render_partial(
             local_toc_tree
         )["fragment"]
 
     def _link_node(self, refuri, text_nodes):
+        text_nodes = list(self._sub_out_underscores(text_nodes))
         link = docutils_nodes.reference("", "", text_nodes[0], refuri=refuri)
         link.extend(text_nodes[1:])
         cp = docutils_nodes.inline(classes=["link-container"])
         cp.append(link)
         return cp
 
     def _strong_node(self, refuri, text_nodes):
         cp = docutils_nodes.inline(classes=["link-container"])
         n1 = docutils_nodes.strong()
-        n1.extend(text_nodes)
+        n1.extend(self._sub_out_underscores(text_nodes))
         cp.append(n1)
         paramlink = docutils_nodes.reference(
             "",
             "",
             docutils_nodes.Text("¶", "¶"),
             refid="",
             # paramlink is our own CSS class, headerlink
             # is theirs.  Trying to get everything we can for existing
             # symbols...
             classes=["paramlink", "headerlink"],
         )
 
         cp.append(paramlink)
         return cp
+
+    def _sub_out_underscores(self, nodes):
+        for node in nodes:
+            for lt in node.traverse(docutils_nodes.Text):
+                m = UNDERSCORE_RE.match(str(lt))
+                if m:
+                    lt.parent.replace(lt, docutils_nodes.Text(m.group(1)))
+
+            yield node
```

### Comparing `zzzeeksphinx-1.3.5/zzzeeksphinx/viewsource.py` & `zzzeeksphinx-1.4.0/zzzeeksphinx/viewsource.py`

 * *Files identical despite different names*

### Comparing `zzzeeksphinx-1.3.5/zzzeeksphinx.egg-info/PKG-INFO` & `zzzeeksphinx-1.4.0/zzzeeksphinx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zzzeeksphinx
-Version: 1.3.5
+Version: 1.4.0
 Summary: Zzzeek's Sphinx Layout and Utilities.
 Home-page: https://github.com/sqlalchemyorg/zzzeeksphinx
 Author: Mike Bayer
 Author-email: mike@zzzcomputing.com
 License: MIT
 Keywords: Sphinx
 Platform: UNKNOWN
```

### Comparing `zzzeeksphinx-1.3.5/zzzeeksphinx.egg-info/SOURCES.txt` & `zzzeeksphinx-1.4.0/zzzeeksphinx.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -29,13 +29,15 @@
 zzzeeksphinx/themes/zsbase/search.mako
 zzzeeksphinx/themes/zsbase/static_base.mako
 zzzeeksphinx/themes/zsbase/theme.conf
 zzzeeksphinx/themes/zsmako/layout.mako
 zzzeeksphinx/themes/zsmako/theme.conf
 zzzeeksphinx/themes/zsmako/static/docs.css
 zzzeeksphinx/themes/zzzeeksphinx/theme.conf
+zzzeeksphinx/themes/zzzeeksphinx/static/annotated.png
 zzzeeksphinx/themes/zzzeeksphinx/static/deepalchemy.png
 zzzeeksphinx/themes/zzzeeksphinx/static/deepalchemy_original.png
 zzzeeksphinx/themes/zzzeeksphinx/static/docs.scss
 zzzeeksphinx/themes/zzzeeksphinx/static/dragons.png
 zzzeeksphinx/themes/zzzeeksphinx/static/dragons_original.png
-zzzeeksphinx/themes/zzzeeksphinx/static/init.js
+zzzeeksphinx/themes/zzzeeksphinx/static/init.js
+zzzeeksphinx/themes/zzzeeksphinx/static/nonannotated.png
```

