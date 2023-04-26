# Comparing `tmp/lino_react-23.3.1.tar.gz` & `tmp/lino_react-23.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lino_react-23.3.1.tar", last modified: Tue Mar 28 06:49:01 2023, max compression
+gzip compressed data, was "lino_react-23.4.0.tar", last modified: Wed Apr 26 03:16:46 2023, max compression
```

## Comparing `lino_react-23.3.1.tar` & `lino_react-23.4.0.tar`

### file list

```diff
@@ -1,56 +1,46 @@
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-03-28 06:49:01.350806 lino_react-23.3.1/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    34523 2023-02-28 05:23:19.000000 lino_react-23.3.1/COPYING
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      157 2023-02-28 05:23:19.000000 lino_react-23.3.1/MANIFEST.in
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     1069 2023-03-28 06:49:01.350806 lino_react-23.3.1/PKG-INFO
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      178 2023-02-28 05:23:19.000000 lino_react-23.3.1/README.rst
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-03-28 06:49:01.338806 lino_react-23.3.1/lino_react/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      283 2023-02-28 05:23:19.000000 lino_react-23.3.1/lino_react/__init__.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-03-28 06:49:01.338806 lino_react-23.3.1/lino_react/react/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     3843 2023-03-18 12:41:25.000000 lino_react-23.3.1/lino_react/react/__init__.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-03-28 06:49:01.338806 lino_react-23.3.1/lino_react/react/__pycache__/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     2761 2023-03-18 12:41:27.000000 lino_react-23.3.1/lino_react/react/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     2980 2023-02-28 05:23:19.000000 lino_react-23.3.1/lino_react/react/__pycache__/__init__.cpython-38.pyc
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     4013 2023-02-28 06:16:51.000000 lino_react-23.3.1/lino_react/react/__pycache__/icons.cpython-310.pyc
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     3793 2023-02-28 05:23:19.000000 lino_react-23.3.1/lino_react/react/__pycache__/icons.cpython-38.pyc
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     1422 2023-02-28 06:16:51.000000 lino_react-23.3.1/lino_react/react/__pycache__/models.cpython-310.pyc
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     1412 2023-02-28 05:23:19.000000 lino_react-23.3.1/lino_react/react/__pycache__/models.cpython-38.pyc
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    18490 2023-03-23 08:30:57.000000 lino_react-23.3.1/lino_react/react/__pycache__/renderer.cpython-310.pyc
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    18127 2023-02-28 05:23:19.000000 lino_react-23.3.1/lino_react/react/__pycache__/renderer.cpython-38.pyc
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    20615 2023-03-18 12:41:29.000000 lino_react-23.3.1/lino_react/react/__pycache__/views.cpython-310.pyc
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    20473 2023-02-28 05:23:19.000000 lino_react-23.3.1/lino_react/react/__pycache__/views.cpython-38.pyc
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-03-28 06:49:01.334806 lino_react-23.3.1/lino_react/react/config/
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-03-28 06:49:01.342806 lino_react-23.3.1/lino_react/react/config/react/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:19.000000 lino_react-23.3.1/lino_react/react/config/react/linoweb.json
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     1797 2023-02-28 05:23:19.000000 lino_react-23.3.1/lino_react/react/config/react/main.html
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    16246 2023-03-24 10:35:36.000000 lino_react-23.3.1/lino_react/react/config/react/service-worker.js
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     3893 2023-02-28 05:23:19.000000 lino_react-23.3.1/lino_react/react/icons.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)       36 2023-02-28 05:23:19.000000 lino_react-23.3.1/lino_react/react/index.js
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      950 2023-02-28 05:23:19.000000 lino_react-23.3.1/lino_react/react/models.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    28961 2023-03-23 08:28:49.000000 lino_react-23.3.1/lino_react/react/renderer.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-03-28 06:49:01.334806 lino_react-23.3.1/lino_react/react/static/
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-03-28 06:49:01.346806 lino_react-23.3.1/lino_react/react/static/media/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    10355 2023-02-28 05:23:19.000000 lino_react-23.3.1/lino_react/react/static/media/color.6441e63a.png
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    10355 2023-02-28 05:23:19.000000 lino_react-23.3.1/lino_react/react/static/media/color.c7a33805.png
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    13112 2023-02-28 05:23:19.000000 lino_react-23.3.1/lino_react/react/static/media/line.567f5738.gif
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    39748 2023-02-28 05:23:19.000000 lino_react-23.3.1/lino_react/react/static/media/primeicons.2d2afb27.eot
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    57384 2023-02-28 05:23:19.000000 lino_react-23.3.1/lino_react/react/static/media/primeicons.3a0d4a58.ttf
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    39648 2023-02-28 05:23:19.000000 lino_react-23.3.1/lino_react/react/static/media/primeicons.66ee0deb.woff
--rw-rw-r--   0 blurry    (1000) blurry    (1000)   234640 2023-02-28 05:23:19.000000 lino_react-23.3.1/lino_react/react/static/media/primeicons.c55d94a2.svg
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    39572 2023-02-28 05:23:19.000000 lino_react-23.3.1/lino_react/react/static/media/primeicons.df0140f8.ttf
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    57560 2023-02-28 05:23:19.000000 lino_react-23.3.1/lino_react/react/static/media/primeicons.dfbfef2d.eot
--rw-rw-r--   0 blurry    (1000) blurry    (1000)   163568 2023-02-28 05:23:19.000000 lino_react-23.3.1/lino_react/react/static/media/primeicons.e5e0e944.svg
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    57460 2023-02-28 05:23:19.000000 lino_react-23.3.1/lino_react/react/static/media/primeicons.e61f3495.woff
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-03-28 06:49:01.350806 lino_react-23.3.1/lino_react/react/static/react/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)  1774967 2023-03-24 10:36:55.000000 lino_react-23.3.1/lino_react/react/static/react/main.js
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     2437 2023-03-24 10:35:36.000000 lino_react-23.3.1/lino_react/react/static/react/main.js.LICENSE.txt
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    28705 2023-03-18 12:41:25.000000 lino_react-23.3.1/lino_react/react/views.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     1431 2023-03-28 06:48:35.000000 lino_react-23.3.1/lino_react/setup_info.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-03-28 06:49:01.338806 lino_react-23.3.1/lino_react.egg-info/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     1069 2023-03-28 06:49:01.000000 lino_react-23.3.1/lino_react.egg-info/PKG-INFO
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     1770 2023-03-28 06:49:01.000000 lino_react-23.3.1/lino_react.egg-info/SOURCES.txt
--rw-rw-r--   0 blurry    (1000) blurry    (1000)        1 2023-03-28 06:49:01.000000 lino_react-23.3.1/lino_react.egg-info/dependency_links.txt
--rw-rw-r--   0 blurry    (1000) blurry    (1000)        1 2023-02-28 05:23:26.000000 lino_react-23.3.1/lino_react.egg-info/not-zip-safe
--rw-rw-r--   0 blurry    (1000) blurry    (1000)        5 2023-03-28 06:49:01.000000 lino_react-23.3.1/lino_react.egg-info/requires.txt
--rw-rw-r--   0 blurry    (1000) blurry    (1000)       11 2023-03-28 06:49:01.000000 lino_react-23.3.1/lino_react.egg-info/top_level.txt
--rw-rw-r--   0 blurry    (1000) blurry    (1000)       38 2023-03-28 06:49:01.350806 lino_react-23.3.1/setup.cfg
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      183 2023-02-28 05:23:19.000000 lino_react-23.3.1/setup.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:16:46.111742 lino_react-23.4.0/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    34523 2021-04-12 19:37:56.000000 lino_react-23.4.0/COPYING
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      157 2020-04-27 23:26:14.000000 lino_react-23.4.0/MANIFEST.in
+-rw-rw-r--   0 luc       (1000) www-data    (33)     1069 2023-04-26 03:16:46.111742 lino_react-23.4.0/PKG-INFO
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      178 2021-05-23 18:57:15.000000 lino_react-23.4.0/README.rst
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:16:46.103742 lino_react-23.4.0/lino_react/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      283 2021-05-23 18:57:15.000000 lino_react-23.4.0/lino_react/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:16:46.103742 lino_react-23.4.0/lino_react/react/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     3843 2023-03-25 09:38:34.000000 lino_react-23.4.0/lino_react/react/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:16:46.103742 lino_react-23.4.0/lino_react/react/config/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:16:46.103742 lino_react-23.4.0/lino_react/react/config/react/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2018-11-27 12:45:09.000000 lino_react-23.4.0/lino_react/react/config/react/linoweb.json
+-rw-rw-r--   0 luc       (1000) www-data    (33)     1797 2023-01-07 15:27:20.000000 lino_react-23.4.0/lino_react/react/config/react/main.html
+-rw-rw-r--   0 luc       (1000) www-data    (33)    16246 2022-11-30 04:23:52.000000 lino_react-23.4.0/lino_react/react/config/react/service-worker.js
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     3893 2023-04-24 18:09:52.000000 lino_react-23.4.0/lino_react/react/icons.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       36 2018-11-22 22:23:05.000000 lino_react-23.4.0/lino_react/react/index.js
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2023-03-28 18:53:35.000000 lino_react-23.4.0/lino_react/react/models.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)    29236 2023-04-18 13:23:50.000000 lino_react-23.4.0/lino_react/react/renderer.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:16:46.103742 lino_react-23.4.0/lino_react/react/static/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:16:46.107742 lino_react-23.4.0/lino_react/react/static/media/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    10355 2021-05-17 15:54:58.000000 lino_react-23.4.0/lino_react/react/static/media/color.6441e63a.png
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    10355 2021-01-26 04:29:47.000000 lino_react-23.4.0/lino_react/react/static/media/color.c7a33805.png
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    13112 2020-09-29 17:55:04.000000 lino_react-23.4.0/lino_react/react/static/media/line.567f5738.gif
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    39748 2021-01-26 04:29:47.000000 lino_react-23.4.0/lino_react/react/static/media/primeicons.2d2afb27.eot
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    57384 2021-05-17 15:54:58.000000 lino_react-23.4.0/lino_react/react/static/media/primeicons.3a0d4a58.ttf
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    39648 2021-01-26 04:29:47.000000 lino_react-23.4.0/lino_react/react/static/media/primeicons.66ee0deb.woff
+-rw-rw-rw-   0 luc       (1000) www-data    (33)   234640 2021-05-17 15:54:58.000000 lino_react-23.4.0/lino_react/react/static/media/primeicons.c55d94a2.svg
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    39572 2021-01-26 04:29:47.000000 lino_react-23.4.0/lino_react/react/static/media/primeicons.df0140f8.ttf
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    57560 2021-05-17 15:54:58.000000 lino_react-23.4.0/lino_react/react/static/media/primeicons.dfbfef2d.eot
+-rw-rw-rw-   0 luc       (1000) www-data    (33)   163568 2021-01-26 04:29:47.000000 lino_react-23.4.0/lino_react/react/static/media/primeicons.e5e0e944.svg
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    57460 2021-05-17 15:54:58.000000 lino_react-23.4.0/lino_react/react/static/media/primeicons.e61f3495.woff
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:16:46.107742 lino_react-23.4.0/lino_react/react/static/react/
+-rw-rw-r--   0 luc       (1000) www-data    (33)  1776677 2023-04-18 13:23:50.000000 lino_react-23.4.0/lino_react/react/static/react/main.js
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2437 2021-09-23 03:04:12.000000 lino_react-23.4.0/lino_react/react/static/react/main.js.LICENSE.txt
+-rw-rw-r--   0 luc       (1000) www-data    (33)    28705 2023-03-24 10:38:37.000000 lino_react-23.4.0/lino_react/react/views.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)     1431 2023-04-26 03:16:36.000000 lino_react-23.4.0/lino_react/setup_info.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:16:46.103742 lino_react-23.4.0/lino_react.egg-info/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1069 2023-04-26 03:16:46.000000 lino_react-23.4.0/lino_react.egg-info/PKG-INFO
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1260 2023-04-26 03:16:46.000000 lino_react-23.4.0/lino_react.egg-info/SOURCES.txt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2023-04-26 03:16:46.000000 lino_react-23.4.0/lino_react.egg-info/dependency_links.txt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2019-01-08 09:40:17.000000 lino_react-23.4.0/lino_react.egg-info/not-zip-safe
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        5 2023-04-26 03:16:46.000000 lino_react-23.4.0/lino_react.egg-info/requires.txt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       11 2023-04-26 03:16:46.000000 lino_react-23.4.0/lino_react.egg-info/top_level.txt
+-rw-rw-r--   0 luc       (1000) www-data    (33)       38 2023-04-26 03:16:46.111742 lino_react-23.4.0/setup.cfg
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      183 2021-04-06 11:15:38.000000 lino_react-23.4.0/setup.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      348 2021-05-23 18:57:15.000000 lino_react-23.4.0/tasks.py
```

### Comparing `lino_react-23.3.1/COPYING` & `lino_react-23.4.0/COPYING`

 * *Files identical despite different names*

### Comparing `lino_react-23.3.1/PKG-INFO` & `lino_react-23.4.0/lino_react.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: lino_react
-Version: 23.3.1
+Name: lino-react
+Version: 23.4.0
 Summary: The React front end for Lino
 Home-page: https://gitlab.com/lino-framework/react
 Author: Rumma & Ko Ltd
 Author-email: info@lino-framework.org
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier:   Programming Language :: Python
```

### Comparing `lino_react-23.3.1/lino_react/react/__init__.py` & `lino_react-23.4.0/lino_react/react/__init__.py`

 * *Files identical despite different names*

### Comparing `lino_react-23.3.1/lino_react/react/__pycache__/icons.cpython-310.pyc` & `lino_react-23.4.0/lino_react/react/icons.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,251 +1,244 @@
-00000000: 6f0d 0d0a 0000 0000 c78f fd63 350f 0000  o..........c5...
-00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0008 0000 0040 0000 0073 1201 0000 6400  .....@...s....d.
-00000030: 6401 6c00 6d01 5a01 0100 6402 a002 a100  d.l.m.Z...d.....
-00000040: 5a03 6900 6403 6404 9301 6405 6406 9301  Z.i.d.d...d.d...
-00000050: 6407 6408 9301 6409 640a 9301 640b 640c  d.d...d.d...d.d.
-00000060: 9301 640d 640e 9301 640f 6410 9301 6411  ..d.d...d.d...d.
-00000070: 6412 9301 6413 6404 9301 6414 6415 9301  d...d.d...d.d...
-00000080: 6416 6417 9301 6418 6419 9301 641a 641b  d.d...d.d...d.d.
-00000090: 9301 641c 641d 9301 641e 641f 9301 6420  ..d.d...d.d...d 
-000000a0: 6421 9301 6422 6404 9301 6900 6423 6424  d!..d"d...i.d#d$
-000000b0: 9301 6425 6426 9301 6427 6426 9301 6428  ..d%d&..d'd&..d(
-000000c0: 6429 9301 642a 6404 9301 642b 642c 9301  d)..d*d...d+d,..
-000000d0: 642d 642e 9301 642f 6430 9301 6431 6404  d-d...d/d0..d1d.
-000000e0: 9301 6432 6404 9301 6433 6404 9301 6434  ..d2d...d3d...d4
-000000f0: 6435 9301 6436 6437 9301 6438 6429 9301  d5..d6d7..d8d)..
-00000100: 6439 641f 9301 643a 641f 9301 643b 643c  d9d...d:d...d;d<
-00000110: 9301 a501 643d 643e 643c 643f 6404 6404  ....d=d>d<d?d.d.
-00000120: 6440 9c06 a501 5a04 6504 a005 6441 6442  d@....Z.e...dAdB
-00000130: 8400 6503 4400 8301 a101 0100 6404 5300  ..e.D.......d.S.
-00000140: 2943 e900 0000 0029 01da 0a49 434f 4e5f  )C.....)...ICON_
-00000150: 4e41 4d45 5361 7f09 0000 7069 2d73 7465  NAMESa....pi-ste
-00000160: 702d 6261 636b 7761 7264 2d61 6c74 0a70  p-backward-alt.p
-00000170: 692d 7374 6570 2d66 6f72 7761 7264 2d61  i-step-forward-a
-00000180: 6c74 0a70 692d 666f 7277 6172 640a 7069  lt.pi-forward.pi
-00000190: 2d62 6163 6b77 6172 640a 7069 2d66 6173  -backward.pi-fas
-000001a0: 742d 6261 636b 7761 7264 0a70 692d 6661  t-backward.pi-fa
-000001b0: 7374 2d66 6f72 7761 7264 0a70 692d 7061  st-forward.pi-pa
-000001c0: 7573 650a 7069 2d70 6c61 790a 7069 2d63  use.pi-play.pi-c
-000001d0: 6f6d 7061 7373 0a70 692d 6964 2d63 6172  ompass.pi-id-car
-000001e0: 640a 7069 2d74 6963 6b65 740a 7069 2d66  d.pi-ticket.pi-f
-000001f0: 696c 652d 6f0a 7069 2d72 6570 6c79 0a70  ile-o.pi-reply.p
-00000200: 692d 6469 7265 6374 696f 6e73 2d61 6c74  i-directions-alt
-00000210: 0a70 692d 6469 7265 6374 696f 6e73 0a70  .pi-directions.p
-00000220: 692d 7468 756d 6273 2d75 700a 7069 2d74  i-thumbs-up.pi-t
-00000230: 6875 6d62 732d 646f 776e 0a70 692d 736f  humbs-down.pi-so
-00000240: 7274 2d6e 756d 6572 6963 2d64 6f77 6e2d  rt-numeric-down-
-00000250: 616c 740a 7069 2d73 6f72 742d 6e75 6d65  alt.pi-sort-nume
-00000260: 7269 632d 7570 2d61 6c74 0a70 692d 736f  ric-up-alt.pi-so
-00000270: 7274 2d61 6c70 6861 2d64 6f77 6e2d 616c  rt-alpha-down-al
-00000280: 740a 7069 2d73 6f72 742d 616c 7068 612d  t.pi-sort-alpha-
-00000290: 7570 2d61 6c74 0a70 692d 736f 7274 2d6e  up-alt.pi-sort-n
-000002a0: 756d 6572 6963 2d64 6f77 6e0a 7069 2d73  umeric-down.pi-s
-000002b0: 6f72 742d 6e75 6d65 7269 632d 7570 0a70  ort-numeric-up.p
-000002c0: 692d 736f 7274 2d61 6c70 6861 2d64 6f77  i-sort-alpha-dow
-000002d0: 6e0a 7069 2d73 6f72 742d 616c 7068 612d  n.pi-sort-alpha-
-000002e0: 7570 0a70 692d 736f 7274 2d61 6c74 0a70  up.pi-sort-alt.p
-000002f0: 692d 736f 7274 2d61 6d6f 756e 742d 7570  i-sort-amount-up
-00000300: 0a70 692d 736f 7274 2d61 6d6f 756e 742d  .pi-sort-amount-
-00000310: 646f 776e 0a70 692d 736f 7274 2d61 6d6f  down.pi-sort-amo
-00000320: 756e 742d 646f 776e 2d61 6c74 0a70 692d  unt-down-alt.pi-
-00000330: 736f 7274 2d61 6d6f 756e 742d 7570 2d61  sort-amount-up-a
-00000340: 6c74 0a70 692d 7061 6c65 7474 650a 7069  lt.pi-palette.pi
-00000350: 2d75 6e64 6f0a 7069 2d64 6573 6b74 6f70  -undo.pi-desktop
-00000360: 0a70 692d 736c 6964 6572 732d 760a 7069  .pi-sliders-v.pi
-00000370: 2d73 6c69 6465 7273 2d68 0a70 692d 7365  -sliders-h.pi-se
-00000380: 6172 6368 2d70 6c75 730a 7069 2d73 6561  arch-plus.pi-sea
-00000390: 7263 682d 6d69 6e75 730a 7069 2d66 696c  rch-minus.pi-fil
-000003a0: 652d 6578 6365 6c0a 7069 2d66 696c 652d  e-excel.pi-file-
-000003b0: 7064 660a 7069 2d63 6865 636b 2d73 7175  pdf.pi-check-squ
-000003c0: 6172 650a 7069 2d63 6861 7274 2d6c 696e  are.pi-chart-lin
-000003d0: 650a 7069 2d75 7365 722d 6564 6974 0a70  e.pi-user-edit.p
-000003e0: 692d 6578 636c 616d 6174 696f 6e2d 6369  i-exclamation-ci
-000003f0: 7263 6c65 0a70 692d 616e 6472 6f69 640a  rcle.pi-android.
-00000400: 7069 2d67 6f6f 676c 650a 7069 2d61 7070  pi-google.pi-app
-00000410: 6c65 0a70 692d 6d69 6372 6f73 6f66 740a  le.pi-microsoft.
-00000420: 7069 2d68 6561 7274 0a70 692d 6d6f 6269  pi-heart.pi-mobi
-00000430: 6c65 0a70 692d 7461 626c 6574 0a70 692d  le.pi-tablet.pi-
-00000440: 6b65 790a 7069 2d73 686f 7070 696e 672d  key.pi-shopping-
-00000450: 6361 7274 0a70 692d 636f 6d6d 656e 7473  cart.pi-comments
-00000460: 0a70 692d 636f 6d6d 656e 740a 7069 2d62  .pi-comment.pi-b
-00000470: 7269 6566 6361 7365 0a70 692d 6265 6c6c  riefcase.pi-bell
-00000480: 0a70 692d 7061 7065 7263 6c69 700a 7069  .pi-paperclip.pi
-00000490: 2d73 6861 7265 2d61 6c74 0a70 692d 656e  -share-alt.pi-en
-000004a0: 7665 6c6f 7065 0a70 692d 766f 6c75 6d65  velope.pi-volume
-000004b0: 2d64 6f77 6e0a 7069 2d76 6f6c 756d 652d  -down.pi-volume-
-000004c0: 7570 0a70 692d 766f 6c75 6d65 2d6f 6666  up.pi-volume-off
-000004d0: 0a70 692d 656a 6563 740a 7069 2d6d 6f6e  .pi-eject.pi-mon
-000004e0: 6579 2d62 696c 6c0a 7069 2d69 6d61 6765  ey-bill.pi-image
-000004f0: 730a 7069 2d69 6d61 6765 0a70 692d 7369  s.pi-image.pi-si
-00000500: 676e 2d69 6e0a 7069 2d73 6967 6e2d 6f75  gn-in.pi-sign-ou
-00000510: 740a 7069 2d77 6966 690a 7069 2d73 6974  t.pi-wifi.pi-sit
-00000520: 656d 6170 0a70 692d 6368 6172 742d 6261  emap.pi-chart-ba
-00000530: 720a 7069 2d63 616d 6572 610a 7069 2d64  r.pi-camera.pi-d
-00000540: 6f6c 6c61 720a 7069 2d6c 6f63 6b2d 6f70  ollar.pi-lock-op
-00000550: 656e 0a70 692d 7461 626c 650a 7069 2d6d  en.pi-table.pi-m
-00000560: 6170 2d6d 6172 6b65 720a 7069 2d6c 6973  ap-marker.pi-lis
-00000570: 740a 7069 2d65 7965 2d73 6c61 7368 0a70  t.pi-eye-slash.p
-00000580: 692d 6579 650a 7069 2d66 6f6c 6465 722d  i-eye.pi-folder-
-00000590: 6f70 656e 0a70 692d 666f 6c64 6572 0a70  open.pi-folder.p
-000005a0: 692d 7669 6465 6f0a 7069 2d69 6e62 6f78  i-video.pi-inbox
-000005b0: 0a70 692d 6c6f 636b 0a70 692d 756e 6c6f  .pi-lock.pi-unlo
-000005c0: 636b 0a70 692d 7461 6773 0a70 692d 7461  ck.pi-tags.pi-ta
-000005d0: 670a 7069 2d70 6f77 6572 2d6f 6666 0a70  g.pi-power-off.p
-000005e0: 692d 7361 7665 0a70 692d 7175 6573 7469  i-save.pi-questi
-000005f0: 6f6e 2d63 6972 636c 650a 7069 2d71 7565  on-circle.pi-que
-00000600: 7374 696f 6e0a 7069 2d63 6f70 790a 7069  stion.pi-copy.pi
-00000610: 2d66 696c 650a 7069 2d63 6c6f 6e65 0a70  -file.pi-clone.p
-00000620: 692d 6361 6c65 6e64 6172 2d74 696d 6573  i-calendar-times
-00000630: 0a70 692d 6361 6c65 6e64 6172 2d6d 696e  .pi-calendar-min
-00000640: 7573 0a70 692d 6361 6c65 6e64 6172 2d70  us.pi-calendar-p
-00000650: 6c75 730a 7069 2d65 6c6c 6970 7369 732d  lus.pi-ellipsis-
-00000660: 760a 7069 2d65 6c6c 6970 7369 732d 680a  v.pi-ellipsis-h.
-00000670: 7069 2d62 6f6f 6b6d 6172 6b0a 7069 2d67  pi-bookmark.pi-g
-00000680: 6c6f 6265 0a70 692d 7265 706c 6179 0a70  lobe.pi-replay.p
-00000690: 692d 6669 6c74 6572 0a70 692d 7072 696e  i-filter.pi-prin
-000006a0: 740a 7069 2d61 6c69 676e 2d72 6967 6874  t.pi-align-right
-000006b0: 0a70 692d 616c 6967 6e2d 6c65 6674 0a70  .pi-align-left.p
-000006c0: 692d 616c 6967 6e2d 6365 6e74 6572 0a70  i-align-center.p
-000006d0: 692d 616c 6967 6e2d 6a75 7374 6966 790a  i-align-justify.
-000006e0: 7069 2d63 6f67 0a70 692d 636c 6f75 642d  pi-cog.pi-cloud-
-000006f0: 646f 776e 6c6f 6164 0a70 692d 636c 6f75  download.pi-clou
-00000700: 642d 7570 6c6f 6164 0a70 692d 636c 6f75  d-upload.pi-clou
-00000710: 640a 7069 2d70 656e 6369 6c0a 7069 2d75  d.pi-pencil.pi-u
-00000720: 7365 7273 0a70 692d 636c 6f63 6b0a 7069  sers.pi-clock.pi
-00000730: 2d75 7365 722d 6d69 6e75 730a 7069 2d75  -user-minus.pi-u
-00000740: 7365 722d 706c 7573 0a70 692d 7472 6173  ser-plus.pi-tras
-00000750: 680a 7069 2d77 696e 646f 772d 6d69 6e69  h.pi-window-mini
-00000760: 6d69 7a65 0a70 692d 7769 6e64 6f77 2d6d  mize.pi-window-m
-00000770: 6178 696d 697a 650a 7069 2d65 7874 6572  aximize.pi-exter
-00000780: 6e61 6c2d 6c69 6e6b 0a70 692d 7265 6672  nal-link.pi-refr
-00000790: 6573 680a 7069 2d75 7365 720a 7069 2d65  esh.pi-user.pi-e
-000007a0: 7863 6c61 6d61 7469 6f6e 2d74 7269 616e  xclamation-trian
-000007b0: 676c 650a 7069 2d63 616c 656e 6461 720a  gle.pi-calendar.
-000007c0: 7069 2d63 6865 7672 6f6e 2d63 6972 636c  pi-chevron-circl
-000007d0: 652d 6c65 6674 0a70 692d 6368 6576 726f  e-left.pi-chevro
-000007e0: 6e2d 6369 7263 6c65 2d64 6f77 6e0a 7069  n-circle-down.pi
-000007f0: 2d63 6865 7672 6f6e 2d63 6972 636c 652d  -chevron-circle-
-00000800: 7269 6768 740a 7069 2d63 6865 7672 6f6e  right.pi-chevron
-00000810: 2d63 6972 636c 652d 7570 0a70 692d 616e  -circle-up.pi-an
-00000820: 676c 652d 646f 7562 6c65 2d64 6f77 6e0a  gle-double-down.
-00000830: 7069 2d61 6e67 6c65 2d64 6f75 626c 652d  pi-angle-double-
-00000840: 6c65 6674 0a70 692d 616e 676c 652d 646f  left.pi-angle-do
-00000850: 7562 6c65 2d72 6967 6874 0a70 692d 616e  uble-right.pi-an
-00000860: 676c 652d 646f 7562 6c65 2d75 700a 7069  gle-double-up.pi
-00000870: 2d61 6e67 6c65 2d64 6f77 6e0a 7069 2d61  -angle-down.pi-a
-00000880: 6e67 6c65 2d6c 6566 740a 7069 2d61 6e67  ngle-left.pi-ang
-00000890: 6c65 2d72 6967 6874 0a70 692d 616e 676c  le-right.pi-angl
-000008a0: 652d 7570 0a70 692d 7570 6c6f 6164 0a70  e-up.pi-upload.p
-000008b0: 692d 646f 776e 6c6f 6164 0a70 692d 6261  i-download.pi-ba
-000008c0: 6e0a 7069 2d73 7461 722d 6f0a 7069 2d73  n.pi-star-o.pi-s
-000008d0: 7461 720a 7069 2d63 6865 7672 6f6e 2d6c  tar.pi-chevron-l
-000008e0: 6566 740a 7069 2d63 6865 7672 6f6e 2d72  eft.pi-chevron-r
-000008f0: 6967 6874 0a70 692d 6368 6576 726f 6e2d  ight.pi-chevron-
-00000900: 646f 776e 0a70 692d 6368 6576 726f 6e2d  down.pi-chevron-
-00000910: 7570 0a70 692d 6361 7265 742d 6c65 6674  up.pi-caret-left
-00000920: 0a70 692d 6361 7265 742d 7269 6768 740a  .pi-caret-right.
-00000930: 7069 2d63 6172 6574 2d64 6f77 6e0a 7069  pi-caret-down.pi
-00000940: 2d63 6172 6574 2d75 700a 7069 2d73 6561  -caret-up.pi-sea
-00000950: 7263 680a 7069 2d63 6865 636b 0a70 692d  rch.pi-check.pi-
-00000960: 6368 6563 6b2d 6369 7263 6c65 0a70 692d  check-circle.pi-
-00000970: 7469 6d65 730a 7069 2d74 696d 6573 2d63  times.pi-times-c
-00000980: 6972 636c 650a 7069 2d70 6c75 730a 7069  ircle.pi-plus.pi
-00000990: 2d70 6c75 732d 6369 7263 6c65 0a70 692d  -plus-circle.pi-
-000009a0: 6d69 6e75 730a 7069 2d6d 696e 7573 2d63  minus.pi-minus-c
-000009b0: 6972 636c 650a 7069 2d63 6972 636c 652d  ircle.pi-circle-
-000009c0: 6f6e 0a70 692d 6369 7263 6c65 2d6f 6666  on.pi-circle-off
-000009d0: 0a70 692d 736f 7274 2d64 6f77 6e0a 7069  .pi-sort-down.pi
-000009e0: 2d73 6f72 742d 7570 0a70 692d 736f 7274  -sort-up.pi-sort
-000009f0: 0a70 692d 7374 6570 2d62 6163 6b77 6172  .pi-step-backwar
-00000a00: 640a 7069 2d73 7465 702d 666f 7277 6172  d.pi-step-forwar
-00000a10: 640a 7069 2d74 682d 6c61 7267 650a 7069  d.pi-th-large.pi
-00000a20: 2d61 7272 6f77 2d64 6f77 6e0a 7069 2d61  -arrow-down.pi-a
-00000a30: 7272 6f77 2d6c 6566 740a 7069 2d61 7272  rrow-left.pi-arr
-00000a40: 6f77 2d72 6967 6874 0a70 692d 6172 726f  ow-right.pi-arro
-00000a50: 772d 7570 0a70 692d 6261 7273 0a70 692d  w-up.pi-bars.pi-
-00000a60: 6172 726f 772d 6369 7263 6c65 2d64 6f77  arrow-circle-dow
-00000a70: 6e0a 7069 2d61 7272 6f77 2d63 6972 636c  n.pi-arrow-circl
-00000a80: 652d 6c65 6674 0a70 692d 6172 726f 772d  e-left.pi-arrow-
-00000a90: 6369 7263 6c65 2d72 6967 6874 0a70 692d  circle-right.pi-
-00000aa0: 6172 726f 772d 6369 7263 6c65 2d75 700a  arrow-circle-up.
-00000ab0: 7069 2d69 6e66 6f0a 7069 2d69 6e66 6f2d  pi-info.pi-info-
-00000ac0: 6369 7263 6c65 0a70 692d 686f 6d65 0a70  circle.pi-home.p
-00000ad0: 692d 7370 696e 6e65 72da 0a61 7272 6f77  i-spinner..arrow
-00000ae0: 5f6a 6f69 6e4e da08 6172 726f 775f 7570  _joinN..arrow_up
-00000af0: 7a0b 7069 2d61 7272 6f77 2d75 70da 0a61  z.pi-arrow-up..a
-00000b00: 7272 6f77 5f64 6f77 6e7a 0d70 692d 6172  rrow_downz.pi-ar
-00000b10: 726f 772d 646f 776e da06 6465 6c65 7465  row-down..delete
-00000b20: 7a08 7069 2d74 7261 7368 da03 6164 647a  z.pi-trash..addz
-00000b30: 0e70 692d 706c 7573 2d63 6972 636c 65da  .pi-plus-circle.
-00000b40: 0962 6f6f 6b5f 6c69 6e6b 7a10 7069 2d65  .book_linkz.pi-e
-00000b50: 7874 6572 6e61 6c2d 6c69 6e6b da03 6579  xternal-link..ey
-00000b60: 657a 0670 692d 6579 65da 0662 6173 6b65  ez.pi-eye..baske
-00000b70: 747a 1070 692d 7368 6f70 7069 6e67 2d63  tz.pi-shopping-c
-00000b80: 6172 74da 0e65 6d6f 7469 636f 6e5f 736d  art..emoticon_sm
-00000b90: 696c 65da 0670 656e 6369 6c7a 0969 702d  ile..pencilz.ip-
-00000ba0: 7065 6e63 696c da05 6372 6f73 737a 0870  pencil..crossz.p
-00000bb0: 692d 7469 6d65 73da 056d 6f6e 6579 7a0d  i-times..moneyz.
-00000bc0: 7069 2d6d 6f6e 6579 2d62 696c 6cda 1061  pi-money-bill..a
-00000bd0: 7070 6c69 6361 7469 6f6e 5f66 6f72 6d7a  pplication_formz
-00000be0: 0870 692d 7461 626c 65da 1561 7070 6c69  .pi-table..appli
-00000bf0: 6361 7469 6f6e 5f76 6965 775f 6c69 7374  cation_view_list
-00000c00: 7a07 7069 2d6c 6973 74da 1761 7070 6c69  z.pi-list..appli
-00000c10: 6361 7469 6f6e 5f76 6965 775f 6465 7461  cation_view_deta
-00000c20: 696c 7a0a 7069 2d69 642d 6361 7264 da04  ilz.pi-id-card..
-00000c30: 6469 736b 7a07 7069 2d73 6176 65da 0968  diskz.pi-save..h
-00000c40: 6f75 7267 6c61 7373 da08 6461 7465 5f61  ourglass..date_a
-00000c50: 6464 7a10 7069 2d63 616c 656e 6461 722d  ddz.pi-calendar-
-00000c60: 706c 7573 da09 656d 6169 6c5f 6164 647a  plus..email_addz
-00000c70: 0b70 692d 656e 7665 6c6f 7065 da08 656d  .pi-envelope..em
-00000c80: 6169 6c5f 676f da06 7363 7269 7074 7a09  ail_go..scriptz.
-00000c90: 7069 2d66 696c 652d 6fda 0a73 6372 6970  pi-file-o..scrip
-00000ca0: 745f 6164 64da 0462 656c 6c7a 0770 692d  t_add..bellz.pi-
-00000cb0: 6265 6c6c da08 6361 6c65 6e64 6172 7a0b  bell..calendarz.
-00000cc0: 7069 2d63 616c 656e 6461 72da 0770 7269  pi-calendar..pri
-00000cd0: 6e74 6572 7a08 7069 2d70 7269 6e74 da09  nterz.pi-print..
-00000ce0: 6c69 6768 746e 696e 67da 0e70 7269 6e74  lightning..print
-00000cf0: 6572 5f64 656c 6574 65da 0c61 7272 6f77  er_delete..arrow
-00000d00: 5f64 6976 6964 65da 1270 6167 655f 7768  _divide..page_wh
-00000d10: 6974 655f 6163 726f 6261 747a 0b70 692d  ite_acrobatz.pi-
-00000d20: 6669 6c65 2d70 6466 da0a 7061 6765 5f65  file-pdf..page_e
-00000d30: 7863 656c 7a0d 7069 2d66 696c 652d 6578  xcelz.pi-file-ex
-00000d40: 6365 6cda 0468 746d 6cda 0576 6361 7264  cel..html..vcard
-00000d50: da09 7663 6172 645f 6164 64da 0677 7265  ..vcard_add..wre
-00000d60: 6e63 687a 0670 692d 636f 677a 0f70 692d  nchz.pi-cogz.pi-
-00000d70: 636c 6f75 642d 7570 6c6f 6164 7a0f 7069  cloud-uploadz.pi
-00000d80: 2d63 6865 636b 2d63 6972 636c 657a 0f70  -check-circlez.p
-00000d90: 692d 7469 6d65 732d 6369 7263 6c65 2906  i-times-circle).
-00000da0: da08 7472 616e 736d 6974 da06 6163 6365  ..transmit..acce
-00000db0: 7074 da0d 6461 7461 6261 7365 5f67 6561  pt..database_gea
-00000dc0: 72da 0663 616e 6365 6cda 0a66 6c61 675f  r..cancel..flag_
-00000dd0: 6772 6565 6eda 0964 6174 655f 6e65 7874  green..date_next
-00000de0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00000df0: 0004 0000 0043 0000 0073 1200 0000 6900  .....C...s....i.
-00000e00: 7c00 5d05 7d01 7c01 7c01 9302 7102 5300  |.].}.|.|...q.S.
-00000e10: a900 722b 0000 0029 02da 022e 30da 0469  ..r+...)....0..i
-00000e20: 636f 6e72 2b00 0000 722b 0000 00fa 422f  conr+...r+....B/
-00000e30: 686f 6d65 2f62 6c75 7272 792f 6c69 6e6f  home/blurry/lino
-00000e40: 2f65 6e76 2f72 6570 6f73 6974 6f72 6965  /env/repositorie
-00000e50: 732f 7265 6163 742f 6c69 6e6f 5f72 6561  s/react/lino_rea
-00000e60: 6374 2f72 6561 6374 2f69 636f 6e73 2e70  ct/react/icons.p
-00000e70: 79da 0a3c 6469 6374 636f 6d70 3ee4 0000  y..<dictcomp>...
-00000e80: 0073 0200 0000 1200 722f 0000 0029 06da  .s......r/...)..
-00000e90: 136c 696e 6f2e 636f 7265 2e63 6f6e 7374  .lino.core.const
-00000ea0: 616e 7473 7202 0000 00da 0573 706c 6974  antsr......split
-00000eb0: da10 5245 4143 545f 4943 4f4e 5f4e 414d  ..REACT_ICON_NAM
-00000ec0: 4553 da12 5245 4143 545f 4943 4f4e 5f4d  ES..REACT_ICON_M
-00000ed0: 4150 5049 4e47 da06 7570 6461 7465 722b  APPING..updater+
-00000ee0: 0000 0072 2b00 0000 722b 0000 0072 2e00  ...r+...r+...r..
-00000ef0: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-00000f00: 73a8 0000 000c 0002 0200 7f04 3400 8102  s...........4...
-00000f10: cc00 7f02 3604 0102 ff04 0202 fe04 0302  ....6...........
-00000f20: fd04 0402 fc04 0502 fb04 0602 fa04 0702  ................
-00000f30: f904 0802 f804 0902 f704 0a02 f604 0b02  ................
-00000f40: f504 0c02 f404 0d02 f304 0e02 f204 0f02  ................
-00000f50: f104 1002 f004 1104 ef04 1202 ee04 1302  ................
-00000f60: ed04 1402 ec04 1502 eb04 1602 ea04 1702  ................
-00000f70: e904 1802 e804 1902 e704 1a02 e604 1b02  ................
-00000f80: e504 1c02 e404 1d02 e304 1e02 e204 1f02  ................
-00000f90: e104 2002 e004 2102 df04 2204 de02 2302  .. ...!..."...#.
-00000fa0: 0102 0102 0102 0102 0108 d818 2c         ............,
+00000000: 6672 6f6d 206c 696e 6f2e 636f 7265 2e63  from lino.core.c
+00000010: 6f6e 7374 616e 7473 2069 6d70 6f72 7420  onstants import 
+00000020: 4943 4f4e 5f4e 414d 4553 0a0a 5245 4143  ICON_NAMES..REAC
+00000030: 545f 4943 4f4e 5f4e 414d 4553 203d 2022  T_ICON_NAMES = "
+00000040: 2222 7069 2d73 7465 702d 6261 636b 7761  ""pi-step-backwa
+00000050: 7264 2d61 6c74 0a70 692d 7374 6570 2d66  rd-alt.pi-step-f
+00000060: 6f72 7761 7264 2d61 6c74 0a70 692d 666f  orward-alt.pi-fo
+00000070: 7277 6172 640a 7069 2d62 6163 6b77 6172  rward.pi-backwar
+00000080: 640a 7069 2d66 6173 742d 6261 636b 7761  d.pi-fast-backwa
+00000090: 7264 0a70 692d 6661 7374 2d66 6f72 7761  rd.pi-fast-forwa
+000000a0: 7264 0a70 692d 7061 7573 650a 7069 2d70  rd.pi-pause.pi-p
+000000b0: 6c61 790a 7069 2d63 6f6d 7061 7373 0a70  lay.pi-compass.p
+000000c0: 692d 6964 2d63 6172 640a 7069 2d74 6963  i-id-card.pi-tic
+000000d0: 6b65 740a 7069 2d66 696c 652d 6f0a 7069  ket.pi-file-o.pi
+000000e0: 2d72 6570 6c79 0a70 692d 6469 7265 6374  -reply.pi-direct
+000000f0: 696f 6e73 2d61 6c74 0a70 692d 6469 7265  ions-alt.pi-dire
+00000100: 6374 696f 6e73 0a70 692d 7468 756d 6273  ctions.pi-thumbs
+00000110: 2d75 700a 7069 2d74 6875 6d62 732d 646f  -up.pi-thumbs-do
+00000120: 776e 0a70 692d 736f 7274 2d6e 756d 6572  wn.pi-sort-numer
+00000130: 6963 2d64 6f77 6e2d 616c 740a 7069 2d73  ic-down-alt.pi-s
+00000140: 6f72 742d 6e75 6d65 7269 632d 7570 2d61  ort-numeric-up-a
+00000150: 6c74 0a70 692d 736f 7274 2d61 6c70 6861  lt.pi-sort-alpha
+00000160: 2d64 6f77 6e2d 616c 740a 7069 2d73 6f72  -down-alt.pi-sor
+00000170: 742d 616c 7068 612d 7570 2d61 6c74 0a70  t-alpha-up-alt.p
+00000180: 692d 736f 7274 2d6e 756d 6572 6963 2d64  i-sort-numeric-d
+00000190: 6f77 6e0a 7069 2d73 6f72 742d 6e75 6d65  own.pi-sort-nume
+000001a0: 7269 632d 7570 0a70 692d 736f 7274 2d61  ric-up.pi-sort-a
+000001b0: 6c70 6861 2d64 6f77 6e0a 7069 2d73 6f72  lpha-down.pi-sor
+000001c0: 742d 616c 7068 612d 7570 0a70 692d 736f  t-alpha-up.pi-so
+000001d0: 7274 2d61 6c74 0a70 692d 736f 7274 2d61  rt-alt.pi-sort-a
+000001e0: 6d6f 756e 742d 7570 0a70 692d 736f 7274  mount-up.pi-sort
+000001f0: 2d61 6d6f 756e 742d 646f 776e 0a70 692d  -amount-down.pi-
+00000200: 736f 7274 2d61 6d6f 756e 742d 646f 776e  sort-amount-down
+00000210: 2d61 6c74 0a70 692d 736f 7274 2d61 6d6f  -alt.pi-sort-amo
+00000220: 756e 742d 7570 2d61 6c74 0a70 692d 7061  unt-up-alt.pi-pa
+00000230: 6c65 7474 650a 7069 2d75 6e64 6f0a 7069  lette.pi-undo.pi
+00000240: 2d64 6573 6b74 6f70 0a70 692d 736c 6964  -desktop.pi-slid
+00000250: 6572 732d 760a 7069 2d73 6c69 6465 7273  ers-v.pi-sliders
+00000260: 2d68 0a70 692d 7365 6172 6368 2d70 6c75  -h.pi-search-plu
+00000270: 730a 7069 2d73 6561 7263 682d 6d69 6e75  s.pi-search-minu
+00000280: 730a 7069 2d66 696c 652d 6578 6365 6c0a  s.pi-file-excel.
+00000290: 7069 2d66 696c 652d 7064 660a 7069 2d63  pi-file-pdf.pi-c
+000002a0: 6865 636b 2d73 7175 6172 650a 7069 2d63  heck-square.pi-c
+000002b0: 6861 7274 2d6c 696e 650a 7069 2d75 7365  hart-line.pi-use
+000002c0: 722d 6564 6974 0a70 692d 6578 636c 616d  r-edit.pi-exclam
+000002d0: 6174 696f 6e2d 6369 7263 6c65 0a70 692d  ation-circle.pi-
+000002e0: 616e 6472 6f69 640a 7069 2d67 6f6f 676c  android.pi-googl
+000002f0: 650a 7069 2d61 7070 6c65 0a70 692d 6d69  e.pi-apple.pi-mi
+00000300: 6372 6f73 6f66 740a 7069 2d68 6561 7274  crosoft.pi-heart
+00000310: 0a70 692d 6d6f 6269 6c65 0a70 692d 7461  .pi-mobile.pi-ta
+00000320: 626c 6574 0a70 692d 6b65 790a 7069 2d73  blet.pi-key.pi-s
+00000330: 686f 7070 696e 672d 6361 7274 0a70 692d  hopping-cart.pi-
+00000340: 636f 6d6d 656e 7473 0a70 692d 636f 6d6d  comments.pi-comm
+00000350: 656e 740a 7069 2d62 7269 6566 6361 7365  ent.pi-briefcase
+00000360: 0a70 692d 6265 6c6c 0a70 692d 7061 7065  .pi-bell.pi-pape
+00000370: 7263 6c69 700a 7069 2d73 6861 7265 2d61  rclip.pi-share-a
+00000380: 6c74 0a70 692d 656e 7665 6c6f 7065 0a70  lt.pi-envelope.p
+00000390: 692d 766f 6c75 6d65 2d64 6f77 6e0a 7069  i-volume-down.pi
+000003a0: 2d76 6f6c 756d 652d 7570 0a70 692d 766f  -volume-up.pi-vo
+000003b0: 6c75 6d65 2d6f 6666 0a70 692d 656a 6563  lume-off.pi-ejec
+000003c0: 740a 7069 2d6d 6f6e 6579 2d62 696c 6c0a  t.pi-money-bill.
+000003d0: 7069 2d69 6d61 6765 730a 7069 2d69 6d61  pi-images.pi-ima
+000003e0: 6765 0a70 692d 7369 676e 2d69 6e0a 7069  ge.pi-sign-in.pi
+000003f0: 2d73 6967 6e2d 6f75 740a 7069 2d77 6966  -sign-out.pi-wif
+00000400: 690a 7069 2d73 6974 656d 6170 0a70 692d  i.pi-sitemap.pi-
+00000410: 6368 6172 742d 6261 720a 7069 2d63 616d  chart-bar.pi-cam
+00000420: 6572 610a 7069 2d64 6f6c 6c61 720a 7069  era.pi-dollar.pi
+00000430: 2d6c 6f63 6b2d 6f70 656e 0a70 692d 7461  -lock-open.pi-ta
+00000440: 626c 650a 7069 2d6d 6170 2d6d 6172 6b65  ble.pi-map-marke
+00000450: 720a 7069 2d6c 6973 740a 7069 2d65 7965  r.pi-list.pi-eye
+00000460: 2d73 6c61 7368 0a70 692d 6579 650a 7069  -slash.pi-eye.pi
+00000470: 2d66 6f6c 6465 722d 6f70 656e 0a70 692d  -folder-open.pi-
+00000480: 666f 6c64 6572 0a70 692d 7669 6465 6f0a  folder.pi-video.
+00000490: 7069 2d69 6e62 6f78 0a70 692d 6c6f 636b  pi-inbox.pi-lock
+000004a0: 0a70 692d 756e 6c6f 636b 0a70 692d 7461  .pi-unlock.pi-ta
+000004b0: 6773 0a70 692d 7461 670a 7069 2d70 6f77  gs.pi-tag.pi-pow
+000004c0: 6572 2d6f 6666 0a70 692d 7361 7665 0a70  er-off.pi-save.p
+000004d0: 692d 7175 6573 7469 6f6e 2d63 6972 636c  i-question-circl
+000004e0: 650a 7069 2d71 7565 7374 696f 6e0a 7069  e.pi-question.pi
+000004f0: 2d63 6f70 790a 7069 2d66 696c 650a 7069  -copy.pi-file.pi
+00000500: 2d63 6c6f 6e65 0a70 692d 6361 6c65 6e64  -clone.pi-calend
+00000510: 6172 2d74 696d 6573 0a70 692d 6361 6c65  ar-times.pi-cale
+00000520: 6e64 6172 2d6d 696e 7573 0a70 692d 6361  ndar-minus.pi-ca
+00000530: 6c65 6e64 6172 2d70 6c75 730a 7069 2d65  lendar-plus.pi-e
+00000540: 6c6c 6970 7369 732d 760a 7069 2d65 6c6c  llipsis-v.pi-ell
+00000550: 6970 7369 732d 680a 7069 2d62 6f6f 6b6d  ipsis-h.pi-bookm
+00000560: 6172 6b0a 7069 2d67 6c6f 6265 0a70 692d  ark.pi-globe.pi-
+00000570: 7265 706c 6179 0a70 692d 6669 6c74 6572  replay.pi-filter
+00000580: 0a70 692d 7072 696e 740a 7069 2d61 6c69  .pi-print.pi-ali
+00000590: 676e 2d72 6967 6874 0a70 692d 616c 6967  gn-right.pi-alig
+000005a0: 6e2d 6c65 6674 0a70 692d 616c 6967 6e2d  n-left.pi-align-
+000005b0: 6365 6e74 6572 0a70 692d 616c 6967 6e2d  center.pi-align-
+000005c0: 6a75 7374 6966 790a 7069 2d63 6f67 0a70  justify.pi-cog.p
+000005d0: 692d 636c 6f75 642d 646f 776e 6c6f 6164  i-cloud-download
+000005e0: 0a70 692d 636c 6f75 642d 7570 6c6f 6164  .pi-cloud-upload
+000005f0: 0a70 692d 636c 6f75 640a 7069 2d70 656e  .pi-cloud.pi-pen
+00000600: 6369 6c0a 7069 2d75 7365 7273 0a70 692d  cil.pi-users.pi-
+00000610: 636c 6f63 6b0a 7069 2d75 7365 722d 6d69  clock.pi-user-mi
+00000620: 6e75 730a 7069 2d75 7365 722d 706c 7573  nus.pi-user-plus
+00000630: 0a70 692d 7472 6173 680a 7069 2d77 696e  .pi-trash.pi-win
+00000640: 646f 772d 6d69 6e69 6d69 7a65 0a70 692d  dow-minimize.pi-
+00000650: 7769 6e64 6f77 2d6d 6178 696d 697a 650a  window-maximize.
+00000660: 7069 2d65 7874 6572 6e61 6c2d 6c69 6e6b  pi-external-link
+00000670: 0a70 692d 7265 6672 6573 680a 7069 2d75  .pi-refresh.pi-u
+00000680: 7365 720a 7069 2d65 7863 6c61 6d61 7469  ser.pi-exclamati
+00000690: 6f6e 2d74 7269 616e 676c 650a 7069 2d63  on-triangle.pi-c
+000006a0: 616c 656e 6461 720a 7069 2d63 6865 7672  alendar.pi-chevr
+000006b0: 6f6e 2d63 6972 636c 652d 6c65 6674 0a70  on-circle-left.p
+000006c0: 692d 6368 6576 726f 6e2d 6369 7263 6c65  i-chevron-circle
+000006d0: 2d64 6f77 6e0a 7069 2d63 6865 7672 6f6e  -down.pi-chevron
+000006e0: 2d63 6972 636c 652d 7269 6768 740a 7069  -circle-right.pi
+000006f0: 2d63 6865 7672 6f6e 2d63 6972 636c 652d  -chevron-circle-
+00000700: 7570 0a70 692d 616e 676c 652d 646f 7562  up.pi-angle-doub
+00000710: 6c65 2d64 6f77 6e0a 7069 2d61 6e67 6c65  le-down.pi-angle
+00000720: 2d64 6f75 626c 652d 6c65 6674 0a70 692d  -double-left.pi-
+00000730: 616e 676c 652d 646f 7562 6c65 2d72 6967  angle-double-rig
+00000740: 6874 0a70 692d 616e 676c 652d 646f 7562  ht.pi-angle-doub
+00000750: 6c65 2d75 700a 7069 2d61 6e67 6c65 2d64  le-up.pi-angle-d
+00000760: 6f77 6e0a 7069 2d61 6e67 6c65 2d6c 6566  own.pi-angle-lef
+00000770: 740a 7069 2d61 6e67 6c65 2d72 6967 6874  t.pi-angle-right
+00000780: 0a70 692d 616e 676c 652d 7570 0a70 692d  .pi-angle-up.pi-
+00000790: 7570 6c6f 6164 0a70 692d 646f 776e 6c6f  upload.pi-downlo
+000007a0: 6164 0a70 692d 6261 6e0a 7069 2d73 7461  ad.pi-ban.pi-sta
+000007b0: 722d 6f0a 7069 2d73 7461 720a 7069 2d63  r-o.pi-star.pi-c
+000007c0: 6865 7672 6f6e 2d6c 6566 740a 7069 2d63  hevron-left.pi-c
+000007d0: 6865 7672 6f6e 2d72 6967 6874 0a70 692d  hevron-right.pi-
+000007e0: 6368 6576 726f 6e2d 646f 776e 0a70 692d  chevron-down.pi-
+000007f0: 6368 6576 726f 6e2d 7570 0a70 692d 6361  chevron-up.pi-ca
+00000800: 7265 742d 6c65 6674 0a70 692d 6361 7265  ret-left.pi-care
+00000810: 742d 7269 6768 740a 7069 2d63 6172 6574  t-right.pi-caret
+00000820: 2d64 6f77 6e0a 7069 2d63 6172 6574 2d75  -down.pi-caret-u
+00000830: 700a 7069 2d73 6561 7263 680a 7069 2d63  p.pi-search.pi-c
+00000840: 6865 636b 0a70 692d 6368 6563 6b2d 6369  heck.pi-check-ci
+00000850: 7263 6c65 0a70 692d 7469 6d65 730a 7069  rcle.pi-times.pi
+00000860: 2d74 696d 6573 2d63 6972 636c 650a 7069  -times-circle.pi
+00000870: 2d70 6c75 730a 7069 2d70 6c75 732d 6369  -plus.pi-plus-ci
+00000880: 7263 6c65 0a70 692d 6d69 6e75 730a 7069  rcle.pi-minus.pi
+00000890: 2d6d 696e 7573 2d63 6972 636c 650a 7069  -minus-circle.pi
+000008a0: 2d63 6972 636c 652d 6f6e 0a70 692d 6369  -circle-on.pi-ci
+000008b0: 7263 6c65 2d6f 6666 0a70 692d 736f 7274  rcle-off.pi-sort
+000008c0: 2d64 6f77 6e0a 7069 2d73 6f72 742d 7570  -down.pi-sort-up
+000008d0: 0a70 692d 736f 7274 0a70 692d 7374 6570  .pi-sort.pi-step
+000008e0: 2d62 6163 6b77 6172 640a 7069 2d73 7465  -backward.pi-ste
+000008f0: 702d 666f 7277 6172 640a 7069 2d74 682d  p-forward.pi-th-
+00000900: 6c61 7267 650a 7069 2d61 7272 6f77 2d64  large.pi-arrow-d
+00000910: 6f77 6e0a 7069 2d61 7272 6f77 2d6c 6566  own.pi-arrow-lef
+00000920: 740a 7069 2d61 7272 6f77 2d72 6967 6874  t.pi-arrow-right
+00000930: 0a70 692d 6172 726f 772d 7570 0a70 692d  .pi-arrow-up.pi-
+00000940: 6261 7273 0a70 692d 6172 726f 772d 6369  bars.pi-arrow-ci
+00000950: 7263 6c65 2d64 6f77 6e0a 7069 2d61 7272  rcle-down.pi-arr
+00000960: 6f77 2d63 6972 636c 652d 6c65 6674 0a70  ow-circle-left.p
+00000970: 692d 6172 726f 772d 6369 7263 6c65 2d72  i-arrow-circle-r
+00000980: 6967 6874 0a70 692d 6172 726f 772d 6369  ight.pi-arrow-ci
+00000990: 7263 6c65 2d75 700a 7069 2d69 6e66 6f0a  rcle-up.pi-info.
+000009a0: 7069 2d69 6e66 6f2d 6369 7263 6c65 0a70  pi-info-circle.p
+000009b0: 692d 686f 6d65 0a70 692d 7370 696e 6e65  i-home.pi-spinne
+000009c0: 7222 2222 2e73 706c 6974 2829 0a0a 5245  r""".split()..RE
+000009d0: 4143 545f 4943 4f4e 5f4d 4150 5049 4e47  ACT_ICON_MAPPING
+000009e0: 203d 207b 0a20 2020 2022 6172 726f 775f   = {.    "arrow_
+000009f0: 6a6f 696e 223a 204e 6f6e 652c 0a20 2020  join": None,.   
+00000a00: 2022 6172 726f 775f 7570 223a 2022 7069   "arrow_up": "pi
+00000a10: 2d61 7272 6f77 2d75 7022 2c0a 2020 2020  -arrow-up",.    
+00000a20: 2261 7272 6f77 5f64 6f77 6e22 3a20 2270  "arrow_down": "p
+00000a30: 692d 6172 726f 772d 646f 776e 222c 0a20  i-arrow-down",. 
+00000a40: 2020 2022 6465 6c65 7465 223a 2022 7069     "delete": "pi
+00000a50: 2d74 7261 7368 222c 0a20 2020 2022 6164  -trash",.    "ad
+00000a60: 6422 3a20 2270 692d 706c 7573 2d63 6972  d": "pi-plus-cir
+00000a70: 636c 6522 2c0a 2020 2020 2262 6f6f 6b5f  cle",.    "book_
+00000a80: 6c69 6e6b 223a 2022 7069 2d65 7874 6572  link": "pi-exter
+00000a90: 6e61 6c2d 6c69 6e6b 222c 0a20 2020 2022  nal-link",.    "
+00000aa0: 6579 6522 3a20 2270 692d 6579 6522 2c0a  eye": "pi-eye",.
+00000ab0: 2020 2020 2262 6173 6b65 7422 3a20 2270      "basket": "p
+00000ac0: 692d 7368 6f70 7069 6e67 2d63 6172 7422  i-shopping-cart"
+00000ad0: 2c0a 2020 2020 2265 6d6f 7469 636f 6e5f  ,.    "emoticon_
+00000ae0: 736d 696c 6522 3a20 4e6f 6e65 2c0a 2020  smile": None,.  
+00000af0: 2020 2270 656e 6369 6c22 3a20 2269 702d    "pencil": "ip-
+00000b00: 7065 6e63 696c 222c 0a20 2020 2022 6372  pencil",.    "cr
+00000b10: 6f73 7322 3a20 2270 692d 7469 6d65 7322  oss": "pi-times"
+00000b20: 2c0a 2020 2020 226d 6f6e 6579 223a 2022  ,.    "money": "
+00000b30: 7069 2d6d 6f6e 6579 2d62 696c 6c22 2c0a  pi-money-bill",.
+00000b40: 2020 2020 2261 7070 6c69 6361 7469 6f6e      "application
+00000b50: 5f66 6f72 6d22 3a20 2270 692d 7461 626c  _form": "pi-tabl
+00000b60: 6522 2c0a 2020 2020 2261 7070 6c69 6361  e",.    "applica
+00000b70: 7469 6f6e 5f76 6965 775f 6c69 7374 223a  tion_view_list":
+00000b80: 2022 7069 2d6c 6973 7422 2c0a 2020 2020   "pi-list",.    
+00000b90: 2261 7070 6c69 6361 7469 6f6e 5f76 6965  "application_vie
+00000ba0: 775f 6465 7461 696c 223a 2022 7069 2d69  w_detail": "pi-i
+00000bb0: 642d 6361 7264 222c 0a20 2020 2022 6469  d-card",.    "di
+00000bc0: 736b 223a 2022 7069 2d73 6176 6522 2c0a  sk": "pi-save",.
+00000bd0: 2020 2020 2268 6f75 7267 6c61 7373 223a      "hourglass":
+00000be0: 204e 6f6e 652c 0a20 2020 2022 6461 7465   None,.    "date
+00000bf0: 5f61 6464 223a 2022 7069 2d63 616c 656e  _add": "pi-calen
+00000c00: 6461 722d 706c 7573 222c 0a20 2020 2022  dar-plus",.    "
+00000c10: 656d 6169 6c5f 6164 6422 3a20 2270 692d  email_add": "pi-
+00000c20: 656e 7665 6c6f 7065 222c 0a20 2020 2022  envelope",.    "
+00000c30: 656d 6169 6c5f 676f 223a 2022 7069 2d65  email_go": "pi-e
+00000c40: 6e76 656c 6f70 6522 2c0a 2020 2020 2273  nvelope",.    "s
+00000c50: 6372 6970 7422 3a20 2270 692d 6669 6c65  cript": "pi-file
+00000c60: 2d6f 222c 0a20 2020 2022 7363 7269 7074  -o",.    "script
+00000c70: 5f61 6464 223a 204e 6f6e 652c 0a20 2020  _add": None,.   
+00000c80: 2022 6265 6c6c 223a 2022 7069 2d62 656c   "bell": "pi-bel
+00000c90: 6c22 2c0a 2020 2020 2263 616c 656e 6461  l",.    "calenda
+00000ca0: 7222 3a20 2270 692d 6361 6c65 6e64 6172  r": "pi-calendar
+00000cb0: 222c 0a20 2020 2022 7072 696e 7465 7222  ",.    "printer"
+00000cc0: 3a20 2270 692d 7072 696e 7422 2c0a 2020  : "pi-print",.  
+00000cd0: 2020 226c 6967 6874 6e69 6e67 223a 204e    "lightning": N
+00000ce0: 6f6e 652c 0a20 2020 2022 7072 696e 7465  one,.    "printe
+00000cf0: 725f 6465 6c65 7465 223a 204e 6f6e 652c  r_delete": None,
+00000d00: 0a20 2020 2022 6172 726f 775f 6469 7669  .    "arrow_divi
+00000d10: 6465 223a 204e 6f6e 652c 0a20 2020 2022  de": None,.    "
+00000d20: 7061 6765 5f77 6869 7465 5f61 6372 6f62  page_white_acrob
+00000d30: 6174 223a 2022 7069 2d66 696c 652d 7064  at": "pi-file-pd
+00000d40: 6622 2c0a 2020 2020 2270 6167 655f 6578  f",.    "page_ex
+00000d50: 6365 6c22 3a20 2270 692d 6669 6c65 2d65  cel": "pi-file-e
+00000d60: 7863 656c 222c 0a20 2020 2022 6874 6d6c  xcel",.    "html
+00000d70: 223a 2022 7069 2d66 696c 652d 6f22 2c0a  ": "pi-file-o",.
+00000d80: 2020 2020 2276 6361 7264 223a 2022 7069      "vcard": "pi
+00000d90: 2d69 642d 6361 7264 222c 0a20 2020 2022  -id-card",.    "
+00000da0: 7663 6172 645f 6164 6422 3a20 2270 692d  vcard_add": "pi-
+00000db0: 6964 2d63 6172 6422 2c0a 2020 2020 2277  id-card",.    "w
+00000dc0: 7265 6e63 6822 3a20 2270 692d 636f 6722  rench": "pi-cog"
+00000dd0: 2c0a 2020 2020 2274 7261 6e73 6d69 7422  ,.    "transmit"
+00000de0: 3a20 2270 692d 636c 6f75 642d 7570 6c6f  : "pi-cloud-uplo
+00000df0: 6164 222c 0a20 2020 2022 6163 6365 7074  ad",.    "accept
+00000e00: 223a 2022 7069 2d63 6865 636b 2d63 6972  ": "pi-check-cir
+00000e10: 636c 6522 2c0a 2020 2020 2264 6174 6162  cle",.    "datab
+00000e20: 6173 655f 6765 6172 223a 2022 7069 2d63  ase_gear": "pi-c
+00000e30: 6f67 222c 2023 206e 6f74 2070 6572 6665  og", # not perfe
+00000e40: 6374 2e2e 2e0a 2020 2020 2263 616e 6365  ct....    "cance
+00000e50: 6c22 3a20 2270 692d 7469 6d65 732d 6369  l": "pi-times-ci
+00000e60: 7263 6c65 222c 0a20 2020 2022 666c 6167  rcle",.    "flag
+00000e70: 5f67 7265 656e 223a 204e 6f6e 652c 0a20  _green": None,. 
+00000e80: 2020 2022 6461 7465 5f6e 6578 7422 3a20     "date_next": 
+00000e90: 4e6f 6e65 2c20 2320 7072 206f 6e6c 7920  None, # pr only 
+00000ea0: 6861 7320 6361 6c2c 2063 616c 2b20 6361  has cal, cal+ ca
+00000eb0: 6c2d 2061 6e64 2063 616c 780a 7d0a 0a23  l- and calx.}..#
+00000ec0: 2061 6c6c 6f77 2064 6972 6563 7420 6d61   allow direct ma
+00000ed0: 7070 696e 6720 7069 2d75 706c 6f61 6473  pping pi-uploads
+00000ee0: 202d 3e20 7069 2d75 706c 6f61 6473 0a52   -> pi-uploads.R
+00000ef0: 4541 4354 5f49 434f 4e5f 4d41 5050 494e  EACT_ICON_MAPPIN
+00000f00: 472e 7570 6461 7465 287b 6963 6f6e 203a  G.update({icon :
+00000f10: 2069 636f 6e20 666f 7220 6963 6f6e 2069   icon for icon i
+00000f20: 6e20 5245 4143 545f 4943 4f4e 5f4e 414d  n REACT_ICON_NAM
+00000f30: 4553 7d29 0a                             ES}).
```

### Comparing `lino_react-23.3.1/lino_react/react/config/react/main.html` & `lino_react-23.4.0/lino_react/react/config/react/main.html`

 * *Files identical despite different names*

### Comparing `lino_react-23.3.1/lino_react/react/config/react/service-worker.js` & `lino_react-23.4.0/lino_react/react/config/react/service-worker.js`

 * *Files identical despite different names*

### Comparing `lino_react-23.3.1/lino_react/react/renderer.py` & `lino_react-23.4.0/lino_react/react/renderer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 # -*- coding: UTF-8 -*-
-# Copyright 2012-2022 Rumma & Ko Ltd
+# Copyright 2012-2023 Rumma & Ko Ltd
 # License: GNU Affero General Public License v3 (see file COPYING for details)
 
-
 import os
 from pathlib import Path
 from html import escape
 from django.conf import settings
 from django.db import models
 from django.utils.text import format_lazy
 from django.utils import translation
 
 from lino.core import constants as ext_requests
-from lino.core.renderer import add_user_language, JsRenderer, HtmlRenderer
-from lino.core.renderer_mixins import JsCacheRenderer
+from lino.core.renderer import add_user_language, JsCacheRenderer
 
 from lino.core.menus import Menu, MenuItem
 from lino.core import constants
 from lino.core import choicelists
 from lino.core.gfks import ContentType
 from lino.modlib.extjs.ext_renderer import ExtRenderer
 
@@ -54,28 +52,27 @@
             x = key(x)
         if x == target:
             return i
     else:
         return -1
 
 
-class Renderer(JsRenderer, JsCacheRenderer):
+class Renderer(JsCacheRenderer):
     """
     A front-end renderer that uses the React Javascript framework.
     """
     is_interactive = True
     can_auth = True
 
     lino_web_template = "react/linoweb.json"
     file_type = '.json'
     support_dashboard_layout = True  # Used to prevent any dashboard items being rendered from main html dashboard.
 
     def __init__(self, front_end):
-        JsRenderer.__init__(self, front_end)
-        JsCacheRenderer.__init__(self)
+        super().__init__(front_end)
         jsgen.register_converter(self.py2js_converter)
 
     def write_lino_js(self, f):
         """
         Creates what is known as window.App.state.site_data in React code.
 
         :param f: File object
@@ -97,14 +94,16 @@
         plugins = settings.SITE.plugins
         data = dict(
             actions={a.action_name: self.action2json(a) for a in actions},
             # actors={a.actor_id: a for a in self.actors_list},
             menu=settings.SITE.get_site_menu(get_user_profile()),
             use_dashboard_layouts=plugins.system.use_dashboard_layouts,
             site_title=settings.SITE.title,
+            editing_frontend=self.front_end.url_prefix is not None,
+            languages={lang.django_code: lang.name for lang in settings.SITE.languages},
             )
         if settings.SITE.is_installed('memo'):
             # [#,@] key triggers
             data.update(
                 suggestors=list(plugins.memo.parser.suggesters.keys()))
 
         # if settings.SITE.never_build_site_cache:
@@ -443,29 +442,36 @@
 
         a = bound_action.action
         # fullname = ".".join(bound_action.full_name().rsplit(".", 1)[::-1])  # moves action name to first arg,
         actorId, an = bound_action.full_name().rsplit(".", 1)
 
         if not status:
             status = {}
-        if ar and ar._status:
-            status.update(ar._status)
+
+        if ar is not None and hasattr(ar, 'get_status'):
+            status = ar.get_status(**status)
 
         if ar and ar.subst_user:
             status[constants.URL_PARAM_SUBST_USER] = ar.subst_user
-        if isinstance(a, ShowEmptyTable):
-            status.update(record_id=-99998)
-        if ar and ar.master_instance is not None:
-            mi = ar.master_instance
-            bp = {
-                constants.URL_PARAM_MASTER_PK: mi.pk}
-            if issubclass(mi.__class__, models.Model):
-                mt = ContentType.objects.get_for_model(mi.__class__)
-                bp[constants.URL_PARAM_MASTER_TYPE] = mt
-            status.update(base_params=bp)
+
+        # if ar and ar._status:
+        #     status.update(ar._status)
+        #
+        # if ar and ar.subst_user:
+        #     status[constants.URL_PARAM_SUBST_USER] = ar.subst_user
+        # if isinstance(a, ShowEmptyTable):
+        #     status.update(record_id=-99998)
+        # if ar and ar.master_instance is not None:
+        #     mi = ar.master_instance
+        #     bp = {
+        #         constants.URL_PARAM_MASTER_PK: mi.pk}
+        #     if issubclass(mi.__class__, models.Model):
+        #         mt = ContentType.objects.get_for_model(mi.__class__)
+        #         bp[constants.URL_PARAM_MASTER_TYPE] = mt
+        #     status.update(base_params=bp)
         if an == 'grid' and hasattr(status, 'record_id'):
             del status['record_id']
 
         rp = None if ar is None else ar.requesting_panel
 
         return "window.App.runAction(%s)" % py2js(dict(
             an=an,
```

### Comparing `lino_react-23.3.1/lino_react/react/static/media/color.6441e63a.png` & `lino_react-23.4.0/lino_react/react/static/media/color.6441e63a.png`

 * *Files identical despite different names*

### Comparing `lino_react-23.3.1/lino_react/react/static/media/color.c7a33805.png` & `lino_react-23.4.0/lino_react/react/static/media/color.c7a33805.png`

 * *Files identical despite different names*

### Comparing `lino_react-23.3.1/lino_react/react/static/media/line.567f5738.gif` & `lino_react-23.4.0/lino_react/react/static/media/line.567f5738.gif`

 * *Files identical despite different names*

### Comparing `lino_react-23.3.1/lino_react/react/static/media/primeicons.2d2afb27.eot` & `lino_react-23.4.0/lino_react/react/static/media/primeicons.2d2afb27.eot`

 * *Files identical despite different names*

### Comparing `lino_react-23.3.1/lino_react/react/static/media/primeicons.3a0d4a58.ttf` & `lino_react-23.4.0/lino_react/react/static/media/primeicons.3a0d4a58.ttf`

 * *Files identical despite different names*

### Comparing `lino_react-23.3.1/lino_react/react/static/media/primeicons.66ee0deb.woff` & `lino_react-23.4.0/lino_react/react/static/media/primeicons.66ee0deb.woff`

 * *Files identical despite different names*

### Comparing `lino_react-23.3.1/lino_react/react/static/media/primeicons.c55d94a2.svg` & `lino_react-23.4.0/lino_react/react/static/media/primeicons.c55d94a2.svg`

 * *Files identical despite different names*

### Comparing `lino_react-23.3.1/lino_react/react/static/media/primeicons.df0140f8.ttf` & `lino_react-23.4.0/lino_react/react/static/media/primeicons.df0140f8.ttf`

 * *Files identical despite different names*

### Comparing `lino_react-23.3.1/lino_react/react/static/media/primeicons.dfbfef2d.eot` & `lino_react-23.4.0/lino_react/react/static/media/primeicons.dfbfef2d.eot`

 * *Files identical despite different names*

### Comparing `lino_react-23.3.1/lino_react/react/static/media/primeicons.e5e0e944.svg` & `lino_react-23.4.0/lino_react/react/static/media/primeicons.e5e0e944.svg`

 * *Files identical despite different names*

### Comparing `lino_react-23.3.1/lino_react/react/static/media/primeicons.e61f3495.woff` & `lino_react-23.4.0/lino_react/react/static/media/primeicons.e61f3495.woff`

 * *Files identical despite different names*

### Comparing `lino_react-23.3.1/lino_react/react/static/react/main.js` & `lino_react-23.4.0/lino_react/react/static/react/main.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -134,14 +134,15 @@
                                     router: e.props.router,
                                     actorId: e.props.actorId,
                                     packId: e.props.packId,
                                     key: e.props.packId + "." + e.props.actorId,
                                     actorData: t,
                                     mk: e.props.mk,
                                     mt: e.props.mt,
+                                    parentBody: !0,
                                     widthInCh: e.container.offsetWidth / e.chInPx.offsetWidth
                                 }))
                             }))), o.createElement("div", {
                                 ref: function(t) {
                                     return e.chInPx = t
                                 },
                                 style: {
@@ -173,41 +174,40 @@
                     lodash__WEBPACK_IMPORTED_MODULE_5__ = __webpack_require__(4159),
                     lodash__WEBPACK_IMPORTED_MODULE_5___default = __webpack_require__.n(lodash__WEBPACK_IMPORTED_MODULE_5__),
                     _DataProvider__WEBPACK_IMPORTED_MODULE_6__ = __webpack_require__(6141),
                     _DashboardItems__WEBPACK_IMPORTED_MODULE_7__ = __webpack_require__(1526),
                     _Table__WEBPACK_IMPORTED_MODULE_8__ = __webpack_require__(4251),
                     _Menu__WEBPACK_IMPORTED_MODULE_9__ = __webpack_require__(4897),
                     _AppMenu__WEBPACK_IMPORTED_MODULE_10__ = __webpack_require__(2420),
-                    _AppTopbar__WEBPACK_IMPORTED_MODULE_11__ = __webpack_require__(9323),
-                    _AppInlineProfile__WEBPACK_IMPORTED_MODULE_12__ = __webpack_require__(3667),
-                    _Actor__WEBPACK_IMPORTED_MODULE_13__ = __webpack_require__(93),
-                    _LinoDialog__WEBPACK_IMPORTED_MODULE_14__ = __webpack_require__(4596),
-                    _LinoChatter_LinoChats__WEBPACK_IMPORTED_MODULE_15__ = __webpack_require__(7573),
-                    _LinoBbar__WEBPACK_IMPORTED_MODULE_16__ = __webpack_require__(4439),
-                    _LinoToolbar__WEBPACK_IMPORTED_MODULE_17__ = __webpack_require__(5783),
-                    _LinoUtils__WEBPACK_IMPORTED_MODULE_18__ = __webpack_require__(9502),
-                    _constants__WEBPACK_IMPORTED_MODULE_35__ = __webpack_require__(1008),
-                    primereact_sidebar__WEBPACK_IMPORTED_MODULE_19__ = __webpack_require__(8392),
-                    primereact_panelmenu__WEBPACK_IMPORTED_MODULE_20__ = __webpack_require__(8659),
-                    primereact_button__WEBPACK_IMPORTED_MODULE_21__ = __webpack_require__(3374),
-                    primereact_scrollpanel__WEBPACK_IMPORTED_MODULE_22__ = __webpack_require__(2657),
-                    primereact_overlaypanel__WEBPACK_IMPORTED_MODULE_23__ = __webpack_require__(1868),
-                    primereact_progressspinner__WEBPACK_IMPORTED_MODULE_24__ = __webpack_require__(4457),
-                    primereact_toast__WEBPACK_IMPORTED_MODULE_25__ = __webpack_require__(8844),
-                    primereact_resources_themes_rhea_theme_css__WEBPACK_IMPORTED_MODULE_26__ = __webpack_require__(7788),
-                    primereact_resources_primereact_min_css__WEBPACK_IMPORTED_MODULE_27__ = __webpack_require__(448),
-                    primeicons_primeicons_css__WEBPACK_IMPORTED_MODULE_28__ = __webpack_require__(848),
-                    primeflex_primeflex_css__WEBPACK_IMPORTED_MODULE_29__ = __webpack_require__(1145),
-                    _layout_layout_css__WEBPACK_IMPORTED_MODULE_30__ = __webpack_require__(7194),
-                    _App_css__WEBPACK_IMPORTED_MODULE_31__ = __webpack_require__(9638),
-                    react_router_dom__WEBPACK_IMPORTED_MODULE_36__ = __webpack_require__(9394),
-                    react_router_dom__WEBPACK_IMPORTED_MODULE_37__ = __webpack_require__(1399),
-                    whatwg_fetch__WEBPACK_IMPORTED_MODULE_32__ = __webpack_require__(8404),
-                    reconnecting_websocket__WEBPACK_IMPORTED_MODULE_33__ = __webpack_require__(7956),
-                    _SiteContext__WEBPACK_IMPORTED_MODULE_34__ = __webpack_require__(7239);
+                    _AppTopbar__WEBPACK_IMPORTED_MODULE_11__ = __webpack_require__(9341),
+                    _Actor__WEBPACK_IMPORTED_MODULE_12__ = __webpack_require__(93),
+                    _LinoDialog__WEBPACK_IMPORTED_MODULE_13__ = __webpack_require__(4596),
+                    _LinoChatter_LinoChats__WEBPACK_IMPORTED_MODULE_14__ = __webpack_require__(7573),
+                    _LinoBbar__WEBPACK_IMPORTED_MODULE_15__ = __webpack_require__(4439),
+                    _LinoToolbar__WEBPACK_IMPORTED_MODULE_16__ = __webpack_require__(5783),
+                    _LinoUtils__WEBPACK_IMPORTED_MODULE_17__ = __webpack_require__(9502),
+                    _constants__WEBPACK_IMPORTED_MODULE_34__ = __webpack_require__(1008),
+                    primereact_sidebar__WEBPACK_IMPORTED_MODULE_18__ = __webpack_require__(8392),
+                    primereact_panelmenu__WEBPACK_IMPORTED_MODULE_19__ = __webpack_require__(8659),
+                    primereact_button__WEBPACK_IMPORTED_MODULE_20__ = __webpack_require__(3374),
+                    primereact_scrollpanel__WEBPACK_IMPORTED_MODULE_21__ = __webpack_require__(2657),
+                    primereact_overlaypanel__WEBPACK_IMPORTED_MODULE_22__ = __webpack_require__(1868),
+                    primereact_progressspinner__WEBPACK_IMPORTED_MODULE_23__ = __webpack_require__(4457),
+                    primereact_toast__WEBPACK_IMPORTED_MODULE_24__ = __webpack_require__(8844),
+                    primereact_resources_themes_rhea_theme_css__WEBPACK_IMPORTED_MODULE_25__ = __webpack_require__(7788),
+                    primereact_resources_primereact_min_css__WEBPACK_IMPORTED_MODULE_26__ = __webpack_require__(448),
+                    primeicons_primeicons_css__WEBPACK_IMPORTED_MODULE_27__ = __webpack_require__(848),
+                    primeflex_primeflex_css__WEBPACK_IMPORTED_MODULE_28__ = __webpack_require__(1145),
+                    _layout_layout_css__WEBPACK_IMPORTED_MODULE_29__ = __webpack_require__(7194),
+                    _App_css__WEBPACK_IMPORTED_MODULE_30__ = __webpack_require__(9638),
+                    react_router_dom__WEBPACK_IMPORTED_MODULE_35__ = __webpack_require__(9394),
+                    react_router_dom__WEBPACK_IMPORTED_MODULE_36__ = __webpack_require__(1399),
+                    whatwg_fetch__WEBPACK_IMPORTED_MODULE_31__ = __webpack_require__(8404),
+                    reconnecting_websocket__WEBPACK_IMPORTED_MODULE_32__ = __webpack_require__(7956),
+                    _SiteContext__WEBPACK_IMPORTED_MODULE_33__ = __webpack_require__(7239);
 
                 function _typeof(e) {
                     return _typeof = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
                         return typeof e
                     } : function(e) {
                         return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
                     }, _typeof(e)
@@ -345,17 +345,17 @@
                             return _classCallCheck(this, App), _this = _super.call(this), _this.fetch_user_settings = function(e, t, n) {
                                 t || _this.setState({
                                     su_id: void 0,
                                     site_loading: !0,
                                     site_data: null,
                                     menu_data: null,
                                     user_settings: null
-                                });
-                                var o = "user/settings/";
-                                e && (o += "?su=".concat(e)), (0, whatwg_fetch__WEBPACK_IMPORTED_MODULE_32__.he)(o).then(_this.handleAjaxResponse).then((function(e) {
+                                }), window.localStorage.clear();
+                                var o = {};
+                                e && (o.su = e), _this.data.selectedLanguage && (o[_constants__WEBPACK_IMPORTED_MODULE_34__.fH] = _this.data.selectedLanguage), (0, whatwg_fetch__WEBPACK_IMPORTED_MODULE_31__.he)("".concat("user/settings/", "?").concat(query_string__WEBPACK_IMPORTED_MODULE_4__.stringify(o))).then(_this.handleAjaxResponse).then((function(e) {
                                     return _this.setState({
                                         user_settings: e,
                                         su_id: e.su_id
                                     }), _this.notification_web_socket(e), _this.fetch_site_data(e.site_data, n)
                                 })).catch((function(e) {
                                     return window.App.handleAjaxException(e)
                                 }))
@@ -365,25 +365,25 @@
                                         delete e.menu, _this.setState({
                                             menu_data: _this.create_menu(t),
                                             site_data: e,
                                             site_loading: !1
                                         }), e.theme_name && e.theme_name !== _this.data.themeName && (_this.data.themeName = e.theme_name, _this.setTheme(_assertThisInitialized(_this))), _this.updatePushSubscription()
                                     },
                                     o = function(e) {
-                                        (0, whatwg_fetch__WEBPACK_IMPORTED_MODULE_32__.he)(e).then((function(e) {
+                                        (0, whatwg_fetch__WEBPACK_IMPORTED_MODULE_31__.he)(e).then((function(e) {
                                             return 200 !== e.status ? _this.setState({
                                                 placeholder: "Something went wrong"
                                             }) : _this.handleAjaxResponse(e)
                                         })).then((function(e) {
                                             window.localStorage.setObject(r, e), n(e)
                                         })).catch((function(e) {
                                             _this.handleAjaxException(e)
                                         }))
                                     },
-                                    r = (0, _LinoUtils__WEBPACK_IMPORTED_MODULE_18__.ah)();
+                                    r = (0, _LinoUtils__WEBPACK_IMPORTED_MODULE_17__.ah)();
                                 if (t) {
                                     var i = e;
                                     o(i += "?v=" + Math.round(1e6 * Math.random()).toString())
                                 } else {
                                     var a = window.localStorage.getObject(r);
                                     a ? n(a) : o(e)
                                 }
@@ -436,26 +436,26 @@
                             }, _this.handleAjaxException = function(e) {
                                 _this.removeLoadMask(), console.error(e), _this.toast.show({
                                     severity: "error",
                                     summary: "Error",
                                     detail: e.message
                                 })
                             }, _this.runAction = function(e) {
-                                (0, _LinoUtils__WEBPACK_IMPORTED_MODULE_18__.rX)(e.an) ? window.Detail.onDirtyLeave({}, "INAPP", _this.wrappedRunAction, e): _this.wrappedRunAction(e)
+                                (0, _LinoUtils__WEBPACK_IMPORTED_MODULE_17__.rX)(e.an) ? window.Detail.onDirtyLeave({}, "INAPP", _this.wrappedRunAction, e): _this.wrappedRunAction(e)
                             }, _this.wrappedRunAction = function() {
                                 var e = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {},
                                     t = e.an,
                                     n = e.actorId,
                                     o = e.rp,
                                     r = e.status,
                                     i = e.sr,
                                     a = e.response_callback,
                                     l = e.onFinished,
                                     s = e.clickCatch,
-                                    p = (0, _LinoUtils__WEBPACK_IMPORTED_MODULE_18__.qI)(o, _this.rps, !0),
+                                    p = (0, _LinoUtils__WEBPACK_IMPORTED_MODULE_17__.qI)(o, _this.rps, !0),
                                     u = p.rp_obj;
                                 o = p.rp, u && u.save && "submit_detail" !== t && u.save();
                                 var c, d, f = _this.state.site_data.actions[t],
                                     h = query_string__WEBPACK_IMPORTED_MODULE_4__.parse(_this.router.history.location.search),
                                     m = {};
                                 r && (c = r.rqdata, d = r.xcallback, delete r.rqdata, delete r.xcallback, r.data && (m = r.data, delete r.data));
                                 var b = {
@@ -469,25 +469,25 @@
                                     response_callback: a,
                                     data: m,
                                     rqdata: c,
                                     xcallback: d,
                                     clickCatch: s
                                 };
                                 if (r && r.hasOwnProperty("record_id") ? b.sr = [r.record_id] : b.sr = i, c && d) return _this.excuteAction(b);
-                                if (r && r.base_params && (r.base_params.mt && (b.mk = r.base_params.mk), r.base_params.mk && (b.mt = r.base_params.mt)), "grid" === t || "show" === t || "detail" === t) _SiteContext__WEBPACK_IMPORTED_MODULE_34__.T8.prototype.getData(n, (function(e) {
+                                if (r && r.base_params && (r.base_params.mt && (b.mk = r.base_params.mk), r.base_params.mk && (b.mt = r.base_params.mt)), "grid" === t || "show" === t || "detail" === t) _SiteContext__WEBPACK_IMPORTED_MODULE_33__.T8.prototype.getData(n, (function(e) {
                                     var t = query_string__WEBPACK_IMPORTED_MODULE_4__.parse(_this.router.history.location.search),
                                         o = {};
                                     Object.keys(t).forEach((function(e) {
-                                        _constants__WEBPACK_IMPORTED_MODULE_35__.gM.includes(e) && (o[e] = t[e])
+                                        _constants__WEBPACK_IMPORTED_MODULE_34__.gM.includes(e) && (o[e] = t[e])
                                     }));
                                     var a = {
                                         pathname: "/api/".concat(n.split(".").join("/"), "/"),
                                         search: o
                                     };
-                                    if (r.hasOwnProperty("record_id") && ![null, void 0].includes(r.record_id) ? a.pathname += "".concat(r.record_id) : i && (a.pathname += "".concat(i[0])), r.base_params && r.base_params.mk && (a.search.mk = r.base_params.mk), r.base_params && r.base_params.mt && (a.search.mt = r.base_params.mt), r.param_values && (a.search.pv = (0, _LinoUtils__WEBPACK_IMPORTED_MODULE_18__.ku)(r.param_values, e.params_fields)), a.search = query_string__WEBPACK_IMPORTED_MODULE_4__.stringify(a.search), s) {
+                                    if (r.hasOwnProperty("record_id") && ![null, void 0].includes(r.record_id) ? a.pathname += "".concat(r.record_id) : i && (a.pathname += "".concat(i[0])), r.base_params && r.base_params.mk && (a.search.mk = r.base_params.mk), r.base_params && r.base_params.mt && (a.search.mt = r.base_params.mt), r.param_values && (a.search.pv = (0, _LinoUtils__WEBPACK_IMPORTED_MODULE_17__.ku)(r.param_values, e.params_fields)), a.search = query_string__WEBPACK_IMPORTED_MODULE_4__.stringify(a.search), s) {
                                         var p = "#".concat(a.pathname);
                                         "" !== a.search && (p += "?".concat(a.search)), window.open(p)
                                     } else a.pathname === _this.router.history.location.pathname && a.search === _this.router.history.location.search ? l && l() : _this.router.history.push(a)
                                 }));
                                 else if (f.window_action) {
                                     var g = {
                                         an: t,
@@ -496,15 +496,15 @@
                                         data: "verify" === t ? {
                                             email: _this.state.user_settings.email,
                                             verification_code: ""
                                         } : {},
                                         action_dialog: "insert" !== t,
                                         originalData: {},
                                         isClosable: function(e) {
-                                            if ((0, _LinoUtils__WEBPACK_IMPORTED_MODULE_18__.dm)(e.props.data, e.props.originalData)) return !0;
+                                            if ((0, _LinoUtils__WEBPACK_IMPORTED_MODULE_17__.dm)(e.props.data, e.props.originalData)) return !0;
                                             _this.askToCloseDialog({
                                                 ParentlinoDialog: e
                                             })
                                         },
                                         onClose: function() {
                                             var e = _this.data.dialogs.filter((function(e) {
                                                 return e !== g
@@ -514,21 +514,21 @@
                                             }), l && l(), _this.setState({
                                                 loading: !1
                                             })
                                         },
                                         onOk: function() {
                                             b.data = g.data, b.status && b.status.fv && delete b.status.fv, _this.excuteAction(b)
                                         },
-                                        footer: "insert" === t ? void 0 : react__WEBPACK_IMPORTED_MODULE_0__.createElement("div", null, react__WEBPACK_IMPORTED_MODULE_0__.createElement(primereact_button__WEBPACK_IMPORTED_MODULE_21__.z, {
+                                        footer: "insert" === t ? void 0 : react__WEBPACK_IMPORTED_MODULE_0__.createElement("div", null, react__WEBPACK_IMPORTED_MODULE_0__.createElement(primereact_button__WEBPACK_IMPORTED_MODULE_20__.z, {
                                             id: "confirm-cancel",
                                             label: "Cancel",
                                             onClick: function() {
                                                 g.onClose()
                                             }
-                                        }), react__WEBPACK_IMPORTED_MODULE_0__.createElement(primereact_button__WEBPACK_IMPORTED_MODULE_21__.z, {
+                                        }), react__WEBPACK_IMPORTED_MODULE_0__.createElement(primereact_button__WEBPACK_IMPORTED_MODULE_20__.z, {
                                             id: "confirm-ok",
                                             label: "OK",
                                             onClick: function() {
                                                 g.onOk()
                                             }
                                         }))
                                     };
@@ -536,15 +536,15 @@
                                     else if (r.field_values) g.data = r.field_values, g.originalData = _objectSpread({}, r.field_values);
                                     else if ("insert" === t) {
                                         var v = {
                                             an: t,
                                             fmt: "json",
                                             rp: o
                                         };
-                                        h.mk && (v.mk = h.mk), h.mt && (v.mt = h.mt), (0, whatwg_fetch__WEBPACK_IMPORTED_MODULE_32__.he)("api/".concat(n.replace(".", "/"), "/-99999?").concat(query_string__WEBPACK_IMPORTED_MODULE_4__.stringify(v))).then(_this.handleAjaxResponse).then((function(e) {
+                                        h.mk && (v.mk = h.mk), h.mt && (v.mt = h.mt), (0, whatwg_fetch__WEBPACK_IMPORTED_MODULE_31__.he)("api/".concat(n.replace(".", "/"), "/-99999?").concat(query_string__WEBPACK_IMPORTED_MODULE_4__.stringify(v))).then(_this.handleAjaxResponse).then((function(e) {
                                             var t = (0, lodash__WEBPACK_IMPORTED_MODULE_5__.cloneDeep)(e.data.disabled_fields);
                                             delete e.data.disabled_fields;
                                             var n = _this.data.dialogs.find((function(e) {
                                                 return e === g
                                             }));
                                             n.data.mk && (e.data.mk = n.data.mk), n.data.mt && (e.data.mt = n.data.mt), n.data = e.data, n.distabled_fields = t, n.originalData = _objectSpread({}, e.data), n.title = e.title, _this.setState({
                                                 loading: !1
@@ -602,15 +602,15 @@
                                     })), xhr.lino_callbackdata = {
                                         rp: rp_obj || rp,
                                         response_callback
                                     }, xhr.send(formData), void(onFinished && onFinished())
                                 }
                                 var makeCall = function() {
                                     var e = "api/".concat(actorId.split(".").join("/"));
-                                    null != urlSr && (e += "/".concat(urlSr)), "GET" === action.http_method && (e += "?".concat(query_string__WEBPACK_IMPORTED_MODULE_4__.stringify(args))), (0, whatwg_fetch__WEBPACK_IMPORTED_MODULE_32__.he)(e, {
+                                    null != urlSr && (e += "/".concat(urlSr)), "GET" === action.http_method && (e += "?".concat(query_string__WEBPACK_IMPORTED_MODULE_4__.stringify(args))), (0, whatwg_fetch__WEBPACK_IMPORTED_MODULE_31__.he)(e, {
                                         method: action.http_method,
                                         body: ["POST", "PUT"].includes(action.http_method) ? new URLSearchParams(query_string__WEBPACK_IMPORTED_MODULE_4__.stringify(args)) : void 0,
                                         headers: {
                                             "Content-Type": "application/x-www-form-urlencoded; charset=UTF-8",
                                             "X-Requested-With": "XMLHttpRequest"
                                         }
                                     }).then((function(e) {
@@ -627,15 +627,15 @@
                                 };
                                 if (rqdata && xcallback) return Object.assign(args, rqdata), args["xcallback__" + xcallback.xcallback_id] = xcallback.choice, void makeCall();
                                 if (status && void 0 !== status.fv && Object.assign(args, {
                                         fv: status.fv
                                     }), "grid_put" === an || "grid_post" === an) {
                                     var editingValues = rp_obj.data.editingValues,
                                         values = {};
-                                    _SiteContext__WEBPACK_IMPORTED_MODULE_34__.T8.prototype.getData(actorId, (function(e) {
+                                    _SiteContext__WEBPACK_IMPORTED_MODULE_33__.T8.prototype.getData(actorId, (function(e) {
                                         Object.keys(editingValues).sort().forEach((function(t, n) {
                                             var o = e.col.find((function(e) {
                                                 return e.fields_index == t
                                             }));
                                             void 0 === o && (o = e.col.find((function(e) {
                                                 return e.fields_index + 1 == t
                                             }))), void 0 !== o && (values[void 0 === values[o.name] ? o.name : o.name + "Hidden"] = editingValues[t])
@@ -662,15 +662,15 @@
                                                 })), _this.setState({
                                                     loading: !1
                                                 })
                                             },
                                             rp,
                                             closable: !1,
                                             footer: react__WEBPACK_IMPORTED_MODULE_0__.createElement("div", null, " ", buttons.map((function(button) {
-                                                return react__WEBPACK_IMPORTED_MODULE_0__.createElement(primereact_button__WEBPACK_IMPORTED_MODULE_21__.z, {
+                                                return react__WEBPACK_IMPORTED_MODULE_0__.createElement(primereact_button__WEBPACK_IMPORTED_MODULE_20__.z, {
                                                     id: "confirm-".concat(button[0]),
                                                     key: button[0],
                                                     className: "p-button-secondary",
                                                     label: button[1],
                                                     onClick: function onClick() {
                                                         diag_props.onClose(), eval(response.xcallback[button[0] + "_resendEvalJs"])
                                                     }
@@ -738,16 +738,19 @@
                             }, _this.data = {
                                 dialogs: [],
                                 miStore: [],
                                 themeName: "default",
                                 onDashboard: !1,
                                 editorDirty: !1,
                                 versionMismatch: !1,
-                                searchDict: {}
-                            }, _this.rps = {}, _this.setRpRef = (0, _LinoUtils__WEBPACK_IMPORTED_MODULE_18__.a_)(_this.rps), _this.dialogRefs = {}, _this.setupDialogRefs = (0, _LinoUtils__WEBPACK_IMPORTED_MODULE_18__.a_)(_this.dialogRefs), _this.response_callbacks = {}, _this.createAccount = _this.createAccount.bind(_assertThisInitialized(_this)), _this.messageInterceptor = _this.messageInterceptor.bind(_assertThisInitialized(_this)), _this.onHrefClick = _this.onHrefClick.bind(_assertThisInitialized(_this)), _this.onKeyDown = _this.onKeyDown.bind(_assertThisInitialized(_this)), _this.handleVerification = _this.handleVerification.bind(_assertThisInitialized(_this)), _this.onWrapperClick = _this.onWrapperClick.bind(_assertThisInitialized(_this)), _this.onToggleMenu = _this.onToggleMenu.bind(_assertThisInitialized(_this)), _this.onSidebarClick = _this.onSidebarClick.bind(_assertThisInitialized(_this)), _this.onMenuItemClick = _this.onMenuItemClick.bind(_assertThisInitialized(_this)), _this.onHomeButton = _this.onHomeButton.bind(_assertThisInitialized(_this)), _this.onSignOutIn = _this.onSignOutIn.bind(_assertThisInitialized(_this)), _this.handleActionResponse = _this.handleActionResponse.bind(_assertThisInitialized(_this)), _this.runAction = _this.runAction.bind(_assertThisInitialized(_this)), _this.wrappedRunAction = _this.wrappedRunAction.bind(_assertThisInitialized(_this)), _this.onAuthoritiesSelect = _this.onAuthoritiesSelect.bind(_assertThisInitialized(_this)), _this.add_su = _this.add_su.bind(_assertThisInitialized(_this)), _this.setLoadMask = _this.setLoadMask.bind(_assertThisInitialized(_this)), _this.removeLoadMask = _this.removeLoadMask.bind(_assertThisInitialized(_this)), _this.notification_web_socket = _this.notification_web_socket.bind(_assertThisInitialized(_this)), _this.push = _this.push.bind(_assertThisInitialized(_this)), _this.pushChat = _this.pushChat.bind(_assertThisInitialized(_this)), _this.sendChat = _this.sendChat.bind(_assertThisInitialized(_this)), _this.sendSeenAction = _this.sendSeenAction.bind(_assertThisInitialized(_this)), _this.OpenConversation = _this.OpenConversation.bind(_assertThisInitialized(_this)), _this.onChatButton = _this.onChatButton.bind(_assertThisInitialized(_this)), _this.positionChatOp = _this.positionChatOp.bind(_assertThisInitialized(_this)), _this.chatwindow = react__WEBPACK_IMPORTED_MODULE_0__.createRef(), _this.onMainWindowUpdate = _this.onMainWindowUpdate.bind(_assertThisInitialized(_this)), window.App = _assertThisInitialized(_this), _this
+                                selectedLanguage: null,
+                                searchDict: {},
+                                scroll: {},
+                                scrollIndex: []
+                            }, _this.rps = {}, _this.setRpRef = (0, _LinoUtils__WEBPACK_IMPORTED_MODULE_17__.a_)(_this.rps), _this.dialogRefs = {}, _this.setupDialogRefs = (0, _LinoUtils__WEBPACK_IMPORTED_MODULE_17__.a_)(_this.dialogRefs), _this.response_callbacks = {}, _this.createAccount = _this.createAccount.bind(_assertThisInitialized(_this)), _this.messageInterceptor = _this.messageInterceptor.bind(_assertThisInitialized(_this)), _this.onHrefClick = _this.onHrefClick.bind(_assertThisInitialized(_this)), _this.onKeyDown = _this.onKeyDown.bind(_assertThisInitialized(_this)), _this.handleVerification = _this.handleVerification.bind(_assertThisInitialized(_this)), _this.onWrapperClick = _this.onWrapperClick.bind(_assertThisInitialized(_this)), _this.onToggleMenu = _this.onToggleMenu.bind(_assertThisInitialized(_this)), _this.onSidebarClick = _this.onSidebarClick.bind(_assertThisInitialized(_this)), _this.onMenuItemClick = _this.onMenuItemClick.bind(_assertThisInitialized(_this)), _this.onHomeButton = _this.onHomeButton.bind(_assertThisInitialized(_this)), _this.onSignOutIn = _this.onSignOutIn.bind(_assertThisInitialized(_this)), _this.handleActionResponse = _this.handleActionResponse.bind(_assertThisInitialized(_this)), _this.runAction = _this.runAction.bind(_assertThisInitialized(_this)), _this.wrappedRunAction = _this.wrappedRunAction.bind(_assertThisInitialized(_this)), _this.onAuthoritiesSelect = _this.onAuthoritiesSelect.bind(_assertThisInitialized(_this)), _this.add_su = _this.add_su.bind(_assertThisInitialized(_this)), _this.setLoadMask = _this.setLoadMask.bind(_assertThisInitialized(_this)), _this.removeLoadMask = _this.removeLoadMask.bind(_assertThisInitialized(_this)), _this.notification_web_socket = _this.notification_web_socket.bind(_assertThisInitialized(_this)), _this.push = _this.push.bind(_assertThisInitialized(_this)), _this.pushChat = _this.pushChat.bind(_assertThisInitialized(_this)), _this.sendChat = _this.sendChat.bind(_assertThisInitialized(_this)), _this.sendSeenAction = _this.sendSeenAction.bind(_assertThisInitialized(_this)), _this.OpenConversation = _this.OpenConversation.bind(_assertThisInitialized(_this)), _this.onChatButton = _this.onChatButton.bind(_assertThisInitialized(_this)), _this.positionChatOp = _this.positionChatOp.bind(_assertThisInitialized(_this)), _this.chatwindow = react__WEBPACK_IMPORTED_MODULE_0__.createRef(), _this.onMainWindowUpdate = _this.onMainWindowUpdate.bind(_assertThisInitialized(_this)), window.App = _assertThisInitialized(_this), _this
                         }
                         return _createClass(App, [{
                             key: "componentDidMount",
                             value: function() {
                                 var e = null;
                                 if (Object.keys(query_string__WEBPACK_IMPORTED_MODULE_4__.parse(window.location.search)).includes("update_found")) {
                                     var t = window.location.origin;
@@ -861,15 +864,15 @@
                                     }()
                                 } else this.runAction(t)
                             }
                         }, {
                             key: "onSignOutIn",
                             value: function(e) {
                                 var t = this;
-                                this.state.user_settings.logged_in ? (0, whatwg_fetch__WEBPACK_IMPORTED_MODULE_32__.he)("auth").then((function(e) {
+                                this.state.user_settings.logged_in ? (0, whatwg_fetch__WEBPACK_IMPORTED_MODULE_31__.he)("auth").then((function(e) {
                                     t.webSocketBridge && t.webSocketBridge.close(), t.chatOp && t.chatOp.hide(), t.fetch_user_settings(), t.router.history.push("/")
                                 })) : this.runAction({
                                     actorId: "about.About",
                                     an: "sign_in",
                                     onMain: !0,
                                     rp: null,
                                     status: {}
@@ -998,15 +1001,15 @@
                             }
                         }, {
                             key: "notification_web_socket",
                             value: function(e) {
                                 var t = this;
                                 console.warn("NWS"), window.Lino && window.Lino.useWebSockets && ((e || this.state.user_settings).user_id, this.webSocketBridge && (this.webSocketBridge.close(), this.setState({
                                     WS: !1
-                                })), this.webSocketBridge = new reconnecting_websocket__WEBPACK_IMPORTED_MODULE_33__.Z(("https:" === window.location.protocol ? "wss" : "ws") + "://" + window.location.host + "/WS/", [], {}), this.webSocketBridge.addEventListener("close", (function(e) {
+                                })), this.webSocketBridge = new reconnecting_websocket__WEBPACK_IMPORTED_MODULE_32__.Z(("https:" === window.location.protocol ? "wss" : "ws") + "://" + window.location.host + "/WS/", [], {}), this.webSocketBridge.addEventListener("close", (function(e) {
                                     t.state.WS, t.setState((function() {
                                         return {
                                             WS: !1,
                                             foo: !0
                                         }
                                     }))
                                 })), this.webSocketBridge.addEventListener("open", (function() {
@@ -1104,21 +1107,21 @@
                                                 return e !== r
                                             })), e.setState({
                                                 loading: !1
                                             })
                                         },
                                         closeOnEscape: !0,
                                         closable: !0,
-                                        footer: react__WEBPACK_IMPORTED_MODULE_0__.createElement("div", null, react__WEBPACK_IMPORTED_MODULE_0__.createElement(primereact_button__WEBPACK_IMPORTED_MODULE_21__.z, {
+                                        footer: react__WEBPACK_IMPORTED_MODULE_0__.createElement("div", null, react__WEBPACK_IMPORTED_MODULE_0__.createElement(primereact_button__WEBPACK_IMPORTED_MODULE_20__.z, {
                                             id: "confirm-no",
                                             label: "No",
                                             onClick: function() {
                                                 r.onClose()
                                             }
-                                        }), react__WEBPACK_IMPORTED_MODULE_0__.createElement(primereact_button__WEBPACK_IMPORTED_MODULE_21__.z, {
+                                        }), react__WEBPACK_IMPORTED_MODULE_0__.createElement(primereact_button__WEBPACK_IMPORTED_MODULE_20__.z, {
                                             id: "confirm-yes",
                                             label: "Yes",
                                             onClick: function() {
                                                 r.onClose(void 0, "closeParent"), o && o.props.onClose()
                                             }
                                         })),
                                         title: "Confirmation",
@@ -1127,402 +1130,184 @@
                                 this.data.dialogs = [r].concat(this.data.dialogs), this.setState({
                                     loading: !1
                                 })
                             }
                         }, {
                             key: "render",
                             value: function() {
-                                var e, t = this,
-                                    n = classnames__WEBPACK_IMPORTED_MODULE_3___default()("layout-wrapper", {
+                                var e = this,
+                                    t = classnames__WEBPACK_IMPORTED_MODULE_3___default()("layout-wrapper", {
                                         "layout-overlay": "overlay" === this.state.layoutMode,
                                         "layout-static": "static" === this.state.layoutMode,
                                         "layout-static-sidebar-inactive": this.state.staticMenuInactive && "static" === this.state.layoutMode,
                                         "layout-overlay-sidebar-active": this.state.overlayMenuActive && "overlay" === this.state.layoutMode,
                                         "layout-mobile-sidebar-active": this.state.mobileMenuActive
                                     }),
-                                    o = classnames__WEBPACK_IMPORTED_MODULE_3___default()("layout-sidebar", {
+                                    n = classnames__WEBPACK_IMPORTED_MODULE_3___default()("layout-sidebar", {
                                         "layout-sidebar-dark": "dark" === this.state.layoutColorMode
                                     });
-                                return react__WEBPACK_IMPORTED_MODULE_0__.createElement(react_router_dom__WEBPACK_IMPORTED_MODULE_36__.UT, {
-                                    ref: function(e) {
-                                        return t.router = e
+                                return react__WEBPACK_IMPORTED_MODULE_0__.createElement(react_router_dom__WEBPACK_IMPORTED_MODULE_35__.UT, {
+                                    ref: function(t) {
+                                        return e.router = t
                                     }
-                                }, react__WEBPACK_IMPORTED_MODULE_0__.createElement(react__WEBPACK_IMPORTED_MODULE_0__.Fragment, null, this.state.loadMask && react__WEBPACK_IMPORTED_MODULE_0__.createElement(_LinoBbar__WEBPACK_IMPORTED_MODULE_16__.W, null), react__WEBPACK_IMPORTED_MODULE_0__.createElement(primereact_toast__WEBPACK_IMPORTED_MODULE_25__.F, {
-                                    ref: function(e) {
-                                        return t.toast = e
+                                }, react__WEBPACK_IMPORTED_MODULE_0__.createElement(react__WEBPACK_IMPORTED_MODULE_0__.Fragment, null, this.state.loadMask && react__WEBPACK_IMPORTED_MODULE_0__.createElement(_LinoBbar__WEBPACK_IMPORTED_MODULE_15__.W, null), react__WEBPACK_IMPORTED_MODULE_0__.createElement(primereact_toast__WEBPACK_IMPORTED_MODULE_24__.F, {
+                                    ref: function(t) {
+                                        return e.toast = t
                                     }
                                 }), this.state.server_error && react__WEBPACK_IMPORTED_MODULE_0__.createElement(react__WEBPACK_IMPORTED_MODULE_0__.Fragment, null, react__WEBPACK_IMPORTED_MODULE_0__.createElement("div", {
                                     style: {
                                         textAlign: "center"
                                     }
-                                }, this.state.recursive_vm ? react__WEBPACK_IMPORTED_MODULE_0__.createElement("p", null, "You are running on obsolete cached data. Please clear site data manually.") : react__WEBPACK_IMPORTED_MODULE_0__.createElement(react__WEBPACK_IMPORTED_MODULE_0__.Fragment, null, react__WEBPACK_IMPORTED_MODULE_0__.createElement("p", null, "There was a problem on the server. If the problem persists, contact your site maintainer."), react__WEBPACK_IMPORTED_MODULE_0__.createElement(primereact_button__WEBPACK_IMPORTED_MODULE_21__.z, {
+                                }, this.state.recursive_vm ? react__WEBPACK_IMPORTED_MODULE_0__.createElement("p", null, "You are running on obsolete cached data. Please clear site data manually.") : react__WEBPACK_IMPORTED_MODULE_0__.createElement(react__WEBPACK_IMPORTED_MODULE_0__.Fragment, null, react__WEBPACK_IMPORTED_MODULE_0__.createElement("p", null, "There was a problem on the server. If the problem persists, contact your site maintainer."), react__WEBPACK_IMPORTED_MODULE_0__.createElement(primereact_button__WEBPACK_IMPORTED_MODULE_20__.z, {
                                     label: "Reinitialize",
-                                    onClick: function(e) {
-                                        t.setState({
+                                    onClick: function(t) {
+                                        e.setState({
                                             server_error: !1
-                                        }), t.fetch_user_settings(null, !1, !0)
+                                        }), e.fetch_user_settings(null, !1, !0)
                                     }
-                                })))), this.state.site_loading || this.state.server_error ? !this.state.server_error && react__WEBPACK_IMPORTED_MODULE_0__.createElement(_LinoToolbar__WEBPACK_IMPORTED_MODULE_17__.MB, {
+                                })))), this.state.site_loading || this.state.server_error ? !this.state.server_error && react__WEBPACK_IMPORTED_MODULE_0__.createElement(_LinoToolbar__WEBPACK_IMPORTED_MODULE_16__.MB, {
                                     parent: this
                                 }) : react__WEBPACK_IMPORTED_MODULE_0__.createElement("div", {
-                                    className: n,
+                                    className: t,
                                     onClick: this.onWrapperClick,
-                                    ref: function(e) {
-                                        return t.topDiv = e
+                                    ref: function(t) {
+                                        return e.topDiv = t
                                     }
                                 }, react__WEBPACK_IMPORTED_MODULE_0__.createElement(_AppTopbar__WEBPACK_IMPORTED_MODULE_11__.w, {
                                     onToggleMenu: this.onToggleMenu,
                                     onHomeButton: this.onHomeButton,
                                     WS: this.state.WS,
                                     useChat: this.state.user_settings && this.state.user_settings.logged_in && window.Lino && window.Lino.useChats,
                                     onChatButton: this.onChatButton
                                 }), react__WEBPACK_IMPORTED_MODULE_0__.createElement("div", {
-                                    ref: function(e) {
-                                        return t.sidebar = e
+                                    ref: function(t) {
+                                        return e.sidebar = t
                                     },
-                                    className: o,
+                                    className: n,
                                     onClick: this.onSidebarClick
-                                }, react__WEBPACK_IMPORTED_MODULE_0__.createElement(primereact_scrollpanel__WEBPACK_IMPORTED_MODULE_22__.P, {
+                                }, react__WEBPACK_IMPORTED_MODULE_0__.createElement(primereact_scrollpanel__WEBPACK_IMPORTED_MODULE_21__.P, {
                                     style: {
                                         height: "100%"
                                     }
                                 }, react__WEBPACK_IMPORTED_MODULE_0__.createElement("div", {
                                     className: "layout-sidebar-scroll-content"
-                                }, this.state.site_loading ? react__WEBPACK_IMPORTED_MODULE_0__.createElement(primereact_progressspinner__WEBPACK_IMPORTED_MODULE_24__.G, null) : react__WEBPACK_IMPORTED_MODULE_0__.createElement("div", null, !this.state.site_data.no_user_model && react__WEBPACK_IMPORTED_MODULE_0__.createElement(_AppInlineProfile__WEBPACK_IMPORTED_MODULE_12__.m, (_defineProperty(e = {
-                                    username: this.state.user_settings.username,
-                                    logged_in: this.state.user_settings.logged_in,
-                                    authorities: this.state.user_settings.authorities,
-                                    onActAsSelf: function() {
-                                        return t.onAuthoritiesSelect([void 0])
-                                    },
-                                    su_id: this.state.su_id,
-                                    su_name: this.state.user_settings.su_name,
-                                    act_as_subtext: this.state.user_settings.act_as_subtext,
-                                    act_as_title_text: this.state.user_settings.act_as_title_text,
-                                    act_as_button_text: this.state.user_settings.act_as_button_text,
-                                    act_as_self_text: this.state.user_settings.act_as_self_text
-                                }, "act_as_self_text", this.state.user_settings.act_as_self_text), _defineProperty(e, "onAuthoritiesSelect", this.onAuthoritiesSelect), _defineProperty(e, "my_setting_text", this.state.user_settings.my_setting_text), _defineProperty(e, "onSignOutIn", (function(e) {
-                                    return t.onSignOutIn(e)
-                                })), _defineProperty(e, "createAccount", this.createAccount), _defineProperty(e, "authAppendTo", this.topDiv), _defineProperty(e, "onMysettings", (function(e) {
-                                    return t.onMysettings(e)
-                                })), e)), react__WEBPACK_IMPORTED_MODULE_0__.createElement(_AppMenu__WEBPACK_IMPORTED_MODULE_10__.Z, {
+                                }, this.state.site_loading ? react__WEBPACK_IMPORTED_MODULE_0__.createElement(primereact_progressspinner__WEBPACK_IMPORTED_MODULE_23__.G, null) : react__WEBPACK_IMPORTED_MODULE_0__.createElement("div", null, react__WEBPACK_IMPORTED_MODULE_0__.createElement(_AppMenu__WEBPACK_IMPORTED_MODULE_10__.Z, {
                                     model: this.state.menu_data,
                                     onMenuItemClick: this.onMenuItemClick
                                 }))))), react__WEBPACK_IMPORTED_MODULE_0__.createElement("div", {
                                     className: "layout-main"
-                                }, react__WEBPACK_IMPORTED_MODULE_0__.createElement(react_router_dom__WEBPACK_IMPORTED_MODULE_37__.AW, {
+                                }, react__WEBPACK_IMPORTED_MODULE_0__.createElement(react_router_dom__WEBPACK_IMPORTED_MODULE_36__.AW, {
                                     exact: !0,
                                     path: "/",
-                                    render: function(e) {
-                                        return window.App.state.site_data.use_dashboard_layouts ? react__WEBPACK_IMPORTED_MODULE_0__.createElement(_Actor__WEBPACK_IMPORTED_MODULE_13__.v, {
-                                            router: e,
+                                    render: function(t) {
+                                        return window.App.state.site_data.use_dashboard_layouts ? react__WEBPACK_IMPORTED_MODULE_0__.createElement(_Actor__WEBPACK_IMPORTED_MODULE_12__.v, {
+                                            router: t,
                                             actorId: "Dashboard",
                                             packId: "system",
-                                            su: t.state.user_settings.su_name,
-                                            key: e.match.params.packId + "." + e.match.params.actorId + "." + t.state.user_settings.su_name
+                                            su: e.state.user_settings.su_name,
+                                            key: t.match.params.packId + "." + t.match.params.actorId + "." + e.state.user_settings.su_name
                                         }) : react__WEBPACK_IMPORTED_MODULE_0__.createElement(_DashboardItems__WEBPACK_IMPORTED_MODULE_7__.n, {
-                                            ref: function(e) {
-                                                t.dashboard = e, t.setRpRef(e)
+                                            ref: function(t) {
+                                                e.dashboard = t, e.setRpRef(t)
                                             },
-                                            dashboard_items: t.state.user_settings ? t.state.user_settings.dashboard_items : 0,
-                                            user: t.state.user_settings ? t.state.user_settings.username : "notloaded"
+                                            dashboard_items: e.state.user_settings ? e.state.user_settings.dashboard_items : 0,
+                                            user: e.state.user_settings ? e.state.user_settings.username : "notloaded"
                                         })
                                     }
-                                }), react__WEBPACK_IMPORTED_MODULE_0__.createElement(_SiteContext__WEBPACK_IMPORTED_MODULE_34__.DN.Provider, {
+                                }), react__WEBPACK_IMPORTED_MODULE_0__.createElement(_SiteContext__WEBPACK_IMPORTED_MODULE_33__.DN.Provider, {
                                     value: this.state.site_data
-                                }, react__WEBPACK_IMPORTED_MODULE_0__.createElement(react_router_dom__WEBPACK_IMPORTED_MODULE_37__.AW, {
+                                }, react__WEBPACK_IMPORTED_MODULE_0__.createElement(react_router_dom__WEBPACK_IMPORTED_MODULE_36__.AW, {
                                     path: "/api/:packId/:actorId",
-                                    render: function(e) {
-                                        var n = new URLSearchParams(e.location.search);
-                                        return t.state.site_loading ? react__WEBPACK_IMPORTED_MODULE_0__.createElement(primereact_progressspinner__WEBPACK_IMPORTED_MODULE_24__.G, null) : react__WEBPACK_IMPORTED_MODULE_0__.createElement(_Actor__WEBPACK_IMPORTED_MODULE_13__.v, {
-                                            router: e,
-                                            actorId: e.match.params.actorId,
-                                            packId: e.match.params.packId,
+                                    render: function(t) {
+                                        var n = new URLSearchParams(t.location.search);
+                                        return e.state.site_loading ? react__WEBPACK_IMPORTED_MODULE_0__.createElement(primereact_progressspinner__WEBPACK_IMPORTED_MODULE_23__.G, null) : react__WEBPACK_IMPORTED_MODULE_0__.createElement(_Actor__WEBPACK_IMPORTED_MODULE_12__.v, {
+                                            router: t,
+                                            actorId: t.match.params.actorId,
+                                            packId: t.match.params.packId,
                                             mk: n.get("mk"),
                                             mt: n.get("mt"),
-                                            su: t.state.user_settings.su_name,
-                                            key: e.match.params.packId + "." + e.match.params.actorId + "." + t.state.user_settings.su_name
+                                            su: e.state.user_settings.su_name,
+                                            key: t.match.params.packId + "." + t.match.params.actorId + "." + e.state.user_settings.su_name
                                         })
                                     }
-                                }))), react__WEBPACK_IMPORTED_MODULE_0__.createElement(_SiteContext__WEBPACK_IMPORTED_MODULE_34__.DN.Provider, {
+                                }))), react__WEBPACK_IMPORTED_MODULE_0__.createElement(_SiteContext__WEBPACK_IMPORTED_MODULE_33__.DN.Provider, {
                                     value: this.state.site_data
                                 }, react__WEBPACK_IMPORTED_MODULE_0__.createElement("div", {
                                     className: "layout-mask"
                                 }), react__WEBPACK_IMPORTED_MODULE_0__.createElement("iframe", {
                                     id: "temp",
                                     name: "temp",
                                     style: {
                                         display: "none"
                                     }
-                                }), this.data.dialogs.map((function(e) {
-                                    return react__WEBPACK_IMPORTED_MODULE_0__.createElement(_SiteContext__WEBPACK_IMPORTED_MODULE_34__.T8, {
-                                        key: weak_key__WEBPACK_IMPORTED_MODULE_2___default()(e),
-                                        actorId: e.actorId
-                                    }, react__WEBPACK_IMPORTED_MODULE_0__.createElement(_LinoDialog__WEBPACK_IMPORTED_MODULE_14__.p, _extends({}, e, {
-                                        action: e.action,
-                                        actorId: e.actorId,
-                                        key: weak_key__WEBPACK_IMPORTED_MODULE_2___default()(e),
-                                        onClose: e.onClose,
-                                        onOk: e.onOk,
-                                        data: e.data,
-                                        title: e.title,
-                                        content: e.content,
-                                        isClosable: e.isClosable,
-                                        closable: e.closable,
-                                        footer: e.footer,
-                                        router: t.router,
+                                }), this.data.dialogs.map((function(t) {
+                                    return react__WEBPACK_IMPORTED_MODULE_0__.createElement(_SiteContext__WEBPACK_IMPORTED_MODULE_33__.T8, {
+                                        key: weak_key__WEBPACK_IMPORTED_MODULE_2___default()(t),
+                                        actorId: t.actorId
+                                    }, react__WEBPACK_IMPORTED_MODULE_0__.createElement(_LinoDialog__WEBPACK_IMPORTED_MODULE_13__.p, _extends({}, t, {
+                                        action: t.action,
+                                        actorId: t.actorId,
+                                        key: weak_key__WEBPACK_IMPORTED_MODULE_2___default()(t),
+                                        onClose: t.onClose,
+                                        onOk: t.onOk,
+                                        data: t.data,
+                                        title: t.title,
+                                        content: t.content,
+                                        isClosable: t.isClosable,
+                                        closable: t.closable,
+                                        footer: t.footer,
+                                        router: e.router,
                                         update_value: function(n) {
-                                            Object.assign(e.data, n), t.data.dialogs = [e]
+                                            Object.assign(t.data, n), e.data.dialogs = [t]
                                         },
-                                        ref: t.setupDialogRefs
+                                        ref: e.setupDialogRefs
                                     })))
-                                }))), this.state.user_settings && this.state.user_settings.logged_in && window.Lino && window.Lino.useChats && react__WEBPACK_IMPORTED_MODULE_0__.createElement(react__WEBPACK_IMPORTED_MODULE_0__.Fragment, null, react__WEBPACK_IMPORTED_MODULE_0__.createElement(primereact_overlaypanel__WEBPACK_IMPORTED_MODULE_23__.T, {
+                                }))), this.state.user_settings && this.state.user_settings.logged_in && window.Lino && window.Lino.useChats && react__WEBPACK_IMPORTED_MODULE_0__.createElement(react__WEBPACK_IMPORTED_MODULE_0__.Fragment, null, react__WEBPACK_IMPORTED_MODULE_0__.createElement(primereact_overlaypanel__WEBPACK_IMPORTED_MODULE_22__.T, {
                                     dismissable: !1,
                                     onHide: function() {
-                                        t.LinoChats.groupChatChooserMountPoint = null, t.LinoChats.setState({
+                                        e.LinoChats.groupChatChooserMountPoint = null, e.LinoChats.setState({
                                             loading: !1
                                         })
                                     },
                                     onShow: function() {
-                                        var e = t.chatOp.overlayRef.current;
-                                        e.style.setProperty("left", "auto"), t.LinoChats.groupChatChooserMountPoint = t.GroupChatChooserMountPoint, t.LinoChats.setState({
+                                        var t = e.chatOp.overlayRef.current;
+                                        t.style.setProperty("left", "auto"), e.LinoChats.groupChatChooserMountPoint = e.GroupChatChooserMountPoint, e.LinoChats.setState({
                                             loading: !1
                                         }), setTimeout((function() {
-                                            return e.style.setProperty("--overlayArrowLeft", (.9 * e.offsetWidth).toString() + "px")
+                                            return t.style.setProperty("--overlayArrowLeft", (.9 * t.offsetWidth).toString() + "px")
                                         }), 50)
                                     },
-                                    ref: function(e) {
-                                        return t.chatOp = e
+                                    ref: function(t) {
+                                        return e.chatOp = t
                                     },
                                     style: {
                                         position: "absolute",
                                         right: "20px"
                                     }
                                 }, react__WEBPACK_IMPORTED_MODULE_0__.createElement("div", {
                                     className: "group-chat-container",
-                                    ref: function(e) {
-                                        return t.GroupChatChooserMountPoint = e
+                                    ref: function(t) {
+                                        return e.GroupChatChooserMountPoint = t
                                     }
-                                })), react__WEBPACK_IMPORTED_MODULE_0__.createElement(_LinoChatter_LinoChats__WEBPACK_IMPORTED_MODULE_15__.S, {
+                                })), react__WEBPACK_IMPORTED_MODULE_0__.createElement(_LinoChatter_LinoChats__WEBPACK_IMPORTED_MODULE_14__.S, {
                                     chatsUnseenBadgeMountPoint: this.chatButton,
                                     sendChat: this.sendChat,
                                     sendSeenAction: this.sendSeenAction,
                                     OpenConversation: this.OpenConversation,
                                     openedconversations: this.state.openedconversations,
-                                    ref: function(e) {
-                                        return t.LinoChats = e
+                                    ref: function(t) {
+                                        return e.LinoChats = t
                                     }
                                 })))))
                             }
                         }]), App
                     }(react__WEBPACK_IMPORTED_MODULE_0__.Component),
                     wrapper = document.getElementById("root");
                 wrapper && react_dom__WEBPACK_IMPORTED_MODULE_1__.render(react__WEBPACK_IMPORTED_MODULE_0__.createElement(App, null), wrapper)
             },
-            3667: (e, t, n) => {
-                "use strict";
-                n.d(t, {
-                    m: () => g
-                });
-                var o = n(2437),
-                    r = n(5904),
-                    i = n.n(r),
-                    a = n(6318),
-                    l = n.n(a),
-                    s = n(1868),
-                    p = n(1674),
-                    u = n(3374);
-
-                function c(e) {
-                    return c = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
-                        return typeof e
-                    } : function(e) {
-                        return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
-                    }, c(e)
-                }
-
-                function d(e, t) {
-                    for (var n = 0; n < t.length; n++) {
-                        var o = t[n];
-                        o.enumerable = o.enumerable || !1, o.configurable = !0, "value" in o && (o.writable = !0), Object.defineProperty(e, o.key, o)
-                    }
-                }
-
-                function f(e, t) {
-                    return f = Object.setPrototypeOf || function(e, t) {
-                        return e.__proto__ = t, e
-                    }, f(e, t)
-                }
-
-                function h(e, t) {
-                    if (t && ("object" === c(t) || "function" == typeof t)) return t;
-                    if (void 0 !== t) throw new TypeError("Derived constructors may only return object or undefined");
-                    return m(e)
-                }
-
-                function m(e) {
-                    if (void 0 === e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
-                    return e
-                }
-
-                function b(e) {
-                    return b = Object.setPrototypeOf ? Object.getPrototypeOf : function(e) {
-                        return e.__proto__ || Object.getPrototypeOf(e)
-                    }, b(e)
-                }
-                var g = function(e) {
-                    ! function(e, t) {
-                        if ("function" != typeof t && null !== t) throw new TypeError("Super expression must either be null or a function");
-                        Object.defineProperty(e, "prototype", {
-                            value: Object.create(t && t.prototype, {
-                                constructor: {
-                                    value: e,
-                                    writable: !0,
-                                    configurable: !0
-                                }
-                            }),
-                            writable: !1
-                        }), t && f(e, t)
-                    }(c, e);
-                    var t, n, r, a, l = (r = c, a = function() {
-                        if ("undefined" == typeof Reflect || !Reflect.construct) return !1;
-                        if (Reflect.construct.sham) return !1;
-                        if ("function" == typeof Proxy) return !0;
-                        try {
-                            return Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], (function() {}))), !0
-                        } catch (e) {
-                            return !1
-                        }
-                    }(), function() {
-                        var e, t = b(r);
-                        if (a) {
-                            var n = b(this).constructor;
-                            e = Reflect.construct(t, arguments, n)
-                        } else e = t.apply(this, arguments);
-                        return h(this, e)
-                    });
-
-                    function c() {
-                        var e;
-                        return function(e, t) {
-                            if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
-                        }(this, c), (e = l.call(this)).state = {
-                            expanded: !1
-                        }, e.onClick = e.onClick.bind(m(e)), e
-                    }
-                    return t = c, (n = [{
-                        key: "onClick",
-                        value: function(e) {
-                            this.setState({
-                                expanded: !this.state.expanded
-                            }), e.preventDefault()
-                        }
-                    }, {
-                        key: "renderActAsOverLay",
-                        value: function() {
-                            var e = this,
-                                t = this.props,
-                                n = t.act_as_title_text,
-                                r = t.act_as_subtext;
-                            return o.createElement(s.T, {
-                                ref: function(t) {
-                                    return e.op = t
-                                },
-                                appendTo: this.props.authAppendTo,
-                                className: "l-actas"
-                            }, o.createElement(p.Z, {
-                                title: n,
-                                subTitle: r
-                            }, this.props.authorities.map((function(t) {
-                                return o.createElement(o.Fragment, {
-                                    key: t[0]
-                                }, o.createElement(u.z, {
-                                    label: t[1],
-                                    onClick: function(n) {
-                                        e.props.onAuthoritiesSelect(t), e.op.hide()
-                                    }
-                                }), o.createElement("br", null))
-                            }))))
-                        }
-                    }, {
-                        key: "render",
-                        value: function() {
-                            var e = this,
-                                t = this.props,
-                                n = t.username,
-                                r = t.su_name,
-                                a = t.su_id,
-                                l = this.props,
-                                s = l.act_as_button_text,
-                                p = l.act_as_self_text,
-                                u = l.my_setting_text;
-                            return n = r ? "".concat(n, " acting as ").concat(r) : n, o.createElement("div", {
-                                className: "profile"
-                            }, o.createElement("a", {
-                                className: "profile-link",
-                                onClick: this.onClick
-                            }, o.createElement("span", {
-                                className: "username"
-                            }, n), o.createElement("i", {
-                                className: "pi pi-fw pi-cog"
-                            })), o.createElement("ul", {
-                                className: i()({
-                                    "profile-expanded": this.state.expanded
-                                })
-                            }, o.createElement("li", {
-                                onClick: this.props.onSignOutIn
-                            }, o.createElement("a", null, o.createElement("i", {
-                                className: "pi pi-fw pi-power-off"
-                            }), this.props.logged_in ? o.createElement("span", null, "Sign out") : o.createElement("span", null, "Sign in"))), !this.props.logged_in && Object.keys(window.App.state.site_data.actions).includes("create_account") && o.createElement("li", {
-                                onClick: this.props.createAccount
-                            }, o.createElement("a", null, o.createElement("i", {
-                                className: "pi pi-plus-circle"
-                            }), o.createElement("span", null, "Create account"))), a && o.createElement("li", {
-                                onClick: this.props.onActAsSelf
-                            }, o.createElement("a", null, o.createElement("i", {
-                                className: "pi pi-fw pi-user"
-                            }), o.createElement("span", null, p))), this.props.authorities.length > 0 && o.createElement("li", {
-                                onClick: function(t) {
-                                    t.target = e.actAsEl, e.op.toggle(t)
-                                },
-                                ref: function(t) {
-                                    return e.actAsEl = t
-                                }
-                            }, o.createElement("a", null, o.createElement("i", {
-                                className: "pi pi-fw pi-users"
-                            }), o.createElement("span", null, s))), this.props.logged_in && o.createElement("li", {
-                                onClick: this.props.onMysettings
-                            }, o.createElement("a", null, o.createElement("i", {
-                                className: "pi pi-fw pi-sliders-v"
-                            }), o.createElement("span", null, u)))), this.renderActAsOverLay())
-                        }
-                    }]) && d(t.prototype, n), Object.defineProperty(t, "prototype", {
-                        writable: !1
-                    }), c
-                }(o.Component);
-                g.propTypes = {
-                    logged_in: l().bool,
-                    username: l().string.isRequired,
-                    onSignOutIn: l().func.isRequired,
-                    authorities: l().array,
-                    onAuthoritiesSelect: l().func,
-                    onActAsSelf: l().func,
-                    authAppendTo: l().instanceOf(Element),
-                    su_name: l().string,
-                    su_id: l().oneOfType([l().number, l().instanceOf(void 0)]),
-                    act_as_button_text: l().string,
-                    act_as_title_text: l().string,
-                    act_as_subtext: l().string,
-                    act_as_self_text: l().string,
-                    my_setting_text: l().string,
-                    onMysettings: l().func.isRequired
-                }, g.defaultProps = {
-                    authorities: []
-                }
-            },
             2420: (e, t, n) => {
                 "use strict";
                 n.d(t, {
                     Z: () => _
                 });
                 var o = n(2437),
                     r = n(6318),
@@ -1893,27 +1678,27 @@
                     model: null,
                     onMenuItemClick: null
                 }, _.propTypes = {
                     model: i().array,
                     onMenuItemClick: i().func
                 }
             },
-            9323: (e, t, n) => {
+            9341: (e, t, n) => {
                 "use strict";
                 n.d(t, {
-                    w: () => g
+                    w: () => P
                 });
                 var o = n(2437),
-                    r = n(6318),
+                    r = n(5904),
                     i = n.n(r),
-                    a = n(5904),
+                    a = n(6318),
                     l = n.n(a),
-                    s = n(3379),
-                    p = n.n(s),
-                    u = n(5790);
+                    s = n(1868),
+                    p = n(1674),
+                    u = n(3374);
 
                 function c(e) {
                     return c = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
                         return typeof e
                     } : function(e) {
                         return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
                     }, c(e)
@@ -1944,33 +1729,29 @@
                 }
 
                 function b(e) {
                     return b = Object.setPrototypeOf ? Object.getPrototypeOf : function(e) {
                         return e.__proto__ || Object.getPrototypeOf(e)
                     }, b(e)
                 }
-                p()(u.Z, {
-                    insert: "head",
-                    singleton: !1
-                }), u.Z.locals;
                 var g = function(e) {
                     ! function(e, t) {
                         if ("function" != typeof t && null !== t) throw new TypeError("Super expression must either be null or a function");
                         Object.defineProperty(e, "prototype", {
                             value: Object.create(t && t.prototype, {
                                 constructor: {
                                     value: e,
                                     writable: !0,
                                     configurable: !0
                                 }
                             }),
                             writable: !1
                         }), t && f(e, t)
-                    }(s, e);
-                    var t, n, r, i, a = (r = s, i = function() {
+                    }(l, e);
+                    var t, n, r, i, a = (r = l, i = function() {
                         if ("undefined" == typeof Reflect || !Reflect.construct) return !1;
                         if (Reflect.construct.sham) return !1;
                         if ("function" == typeof Proxy) return !0;
                         try {
                             return Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], (function() {}))), !0
                         } catch (e) {
                             return !1
@@ -1980,71 +1761,323 @@
                         if (i) {
                             var n = b(this).constructor;
                             e = Reflect.construct(t, arguments, n)
                         } else e = t.apply(this, arguments);
                         return h(this, e)
                     });
 
+                    function l() {
+                        var e;
+                        return function(e, t) {
+                            if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
+                        }(this, l), (e = a.call(this)).state = {
+                            expanded: !1
+                        }, e.onClick = e.onClick.bind(m(e)), e
+                    }
+                    return t = l, (n = [{
+                        key: "onClick",
+                        value: function(e) {
+                            this.pop && this.pop.toggle(e), this.setState({
+                                expanded: !this.state.expanded
+                            }), e.preventDefault()
+                        }
+                    }, {
+                        key: "renderActAsOverLay",
+                        value: function() {
+                            var e = this,
+                                t = this.props,
+                                n = t.act_as_title_text,
+                                r = t.act_as_subtext;
+                            return o.createElement(s.T, {
+                                ref: function(t) {
+                                    return e.op = t
+                                },
+                                appendTo: this.props.authAppendTo,
+                                className: "l-actas"
+                            }, o.createElement(p.Z, {
+                                title: n,
+                                subTitle: r
+                            }, this.props.authorities.map((function(t) {
+                                return o.createElement(o.Fragment, {
+                                    key: t[0]
+                                }, o.createElement(u.z, {
+                                    label: t[1],
+                                    onClick: function(n) {
+                                        e.props.onAuthoritiesSelect(t), e.op.hide()
+                                    }
+                                }), o.createElement("br", null))
+                            }))))
+                        }
+                    }, {
+                        key: "render",
+                        value: function() {
+                            var e = this,
+                                t = this.props,
+                                n = t.username,
+                                r = t.su_name,
+                                i = t.su_id,
+                                a = this.props,
+                                l = a.act_as_button_text,
+                                p = a.act_as_self_text,
+                                c = a.my_setting_text;
+                            n = r ? "".concat(n, " acting as ").concat(r) : n;
+                            var d = window.App.data.selectedLanguage || window.App.state.user_settings.lang;
+                            return o.createElement("div", {
+                                className: "profile"
+                            }, o.createElement(u.z, {
+                                label: window.App.state.site_data.languages[d],
+                                onClick: function(t) {
+                                    return e.lsop.toggle(t)
+                                }
+                            }), o.createElement("span", null, " | "), o.createElement(s.T, {
+                                ref: function(t) {
+                                    return e.lsop = t
+                                }
+                            }, Object.keys(window.App.state.site_data.languages).filter((function(e) {
+                                return e != d
+                            })).map((function(e) {
+                                return o.createElement(o.Fragment, {
+                                    key: e
+                                }, o.createElement(u.z, {
+                                    label: window.App.state.site_data.languages[e],
+                                    onClick: function(t) {
+                                        window.App.data.selectedLanguage = e, window.App.fetch_user_settings(i, !1, !0)
+                                    }
+                                }), o.createElement("br", null))
+                            }))), this.props.logged_in ? o.createElement(o.Fragment, null, o.createElement(u.z, {
+                                icon: "pi pi-cog",
+                                iconPos: "right",
+                                label: n,
+                                onClick: this.onClick
+                            }), o.createElement(s.T, {
+                                ref: function(t) {
+                                    return e.pop = t
+                                }
+                            }, o.createElement(u.z, {
+                                icon: "pi pi-power-off",
+                                label: "Sign out",
+                                onClick: this.props.onSignOutIn
+                            }), o.createElement("br", null), i && o.createElement(u.z, {
+                                icon: "pi pi-user",
+                                label: p,
+                                onClick: this.props.onActAsSelf
+                            }), o.createElement("br", null), this.props.authorities.length > 0 && o.createElement(u.z, {
+                                icon: "pi pi-users",
+                                label: l,
+                                onClick: function(t) {
+                                    t.target = e.actAsEl, e.op.toggle(t)
+                                },
+                                ref: function(t) {
+                                    return e.actAsEl = t
+                                }
+                            }), o.createElement("br", null), o.createElement(u.z, {
+                                icon: "pi pi-sliders-v",
+                                label: c,
+                                onClick: this.props.onMysettings
+                            })), this.renderActAsOverLay()) : o.createElement(o.Fragment, null, o.createElement(u.z, {
+                                icon: "pi pi-power-off",
+                                label: "Sign in",
+                                onClick: this.props.onSignOutIn
+                            }), o.createElement(u.z, {
+                                icon: "pi pi-plus-circle",
+                                label: "Create account",
+                                onClick: this.props.createAccount
+                            })))
+                        }
+                    }]) && d(t.prototype, n), Object.defineProperty(t, "prototype", {
+                        writable: !1
+                    }), l
+                }(o.Component);
+                g.propTypes = {
+                    logged_in: l().bool,
+                    username: l().string.isRequired,
+                    onSignOutIn: l().func.isRequired,
+                    authorities: l().array,
+                    onAuthoritiesSelect: l().func,
+                    onActAsSelf: l().func,
+                    authAppendTo: l().instanceOf(Element),
+                    su_name: l().string,
+                    su_id: l().oneOfType([l().number, l().instanceOf(void 0)]),
+                    act_as_button_text: l().string,
+                    act_as_title_text: l().string,
+                    act_as_subtext: l().string,
+                    act_as_self_text: l().string,
+                    my_setting_text: l().string,
+                    onMysettings: l().func.isRequired
+                }, g.defaultProps = {
+                    authorities: []
+                };
+                var v = n(3379),
+                    y = n.n(v),
+                    w = n(5790);
+
+                function k(e) {
+                    return k = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
+                        return typeof e
+                    } : function(e) {
+                        return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
+                    }, k(e)
+                }
+
+                function x(e, t, n) {
+                    return t in e ? Object.defineProperty(e, t, {
+                        value: n,
+                        enumerable: !0,
+                        configurable: !0,
+                        writable: !0
+                    }) : e[t] = n, e
+                }
+
+                function _(e, t) {
+                    for (var n = 0; n < t.length; n++) {
+                        var o = t[n];
+                        o.enumerable = o.enumerable || !1, o.configurable = !0, "value" in o && (o.writable = !0), Object.defineProperty(e, o.key, o)
+                    }
+                }
+
+                function E(e, t) {
+                    return E = Object.setPrototypeOf || function(e, t) {
+                        return e.__proto__ = t, e
+                    }, E(e, t)
+                }
+
+                function O(e, t) {
+                    if (t && ("object" === k(t) || "function" == typeof t)) return t;
+                    if (void 0 !== t) throw new TypeError("Derived constructors may only return object or undefined");
+                    return C(e)
+                }
+
+                function C(e) {
+                    if (void 0 === e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
+                    return e
+                }
+
+                function S(e) {
+                    return S = Object.setPrototypeOf ? Object.getPrototypeOf : function(e) {
+                        return e.__proto__ || Object.getPrototypeOf(e)
+                    }, S(e)
+                }
+                y()(w.Z, {
+                    insert: "head",
+                    singleton: !1
+                }), w.Z.locals;
+                var P = function(e) {
+                    ! function(e, t) {
+                        if ("function" != typeof t && null !== t) throw new TypeError("Super expression must either be null or a function");
+                        Object.defineProperty(e, "prototype", {
+                            value: Object.create(t && t.prototype, {
+                                constructor: {
+                                    value: e,
+                                    writable: !0,
+                                    configurable: !0
+                                }
+                            }),
+                            writable: !1
+                        }), t && E(e, t)
+                    }(s, e);
+                    var t, n, r, a, l = (r = s, a = function() {
+                        if ("undefined" == typeof Reflect || !Reflect.construct) return !1;
+                        if (Reflect.construct.sham) return !1;
+                        if ("function" == typeof Proxy) return !0;
+                        try {
+                            return Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], (function() {}))), !0
+                        } catch (e) {
+                            return !1
+                        }
+                    }(), function() {
+                        var e, t = S(r);
+                        if (a) {
+                            var n = S(this).constructor;
+                            e = Reflect.construct(t, arguments, n)
+                        } else e = t.apply(this, arguments);
+                        return O(this, e)
+                    });
+
                     function s() {
                         var e;
                         return function(e, t) {
                             if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
-                        }(this, s), (e = a.call(this)).renderChatButton = e.renderChatButton.bind(m(e)), e
+                        }(this, s), (e = l.call(this)).renderChatButton = e.renderChatButton.bind(C(e)), e
                     }
                     return t = s, (n = [{
                         key: "renderChatButton",
                         value: function() {
                             return o.createElement("a", {
                                 onClick: this.props.onChatButton,
                                 ref: function(e) {
                                     return window.App.chatButton = e
                                 }
                             }, o.createElement("span", {
-                                className: l()("layout-topbar-icon pi pi-comments", {
+                                className: i()("layout-topbar-icon pi pi-comments", {
                                     "no-ws": !this.props.WS
                                 })
                             }))
                         }
                     }, {
                         key: "render",
                         value: function() {
-                            var e = "l-site-title ";
-                            return "whitewall" === window.App.data.themeName && (e += "l-whitewall-site-title "), o.createElement("div", {
+                            var e, t = "l-site-title ";
+                            return "whitewall" === window.App.data.themeName && (t += "l-whitewall-site-title "), o.createElement("div", {
                                 className: "layout-topbar clearfix"
                             }, o.createElement("a", {
                                 className: "layout-menu-button",
                                 onClick: this.props.onToggleMenu
                             }, o.createElement("span", {
                                 className: "pi pi-bars"
                             })), o.createElement("a", {
                                 className: "layout-home-button",
                                 onClick: this.props.onHomeButton
                             }, o.createElement("span", {
                                 className: "pi pi-home"
+                            })), window.App.state.site_data.editing_frontend && o.createElement("a", {
+                                className: "layout-home-button",
+                                onClick: function(e) {
+                                    var t = "_self";
+                                    e.ctrlKey && (t = "_blank"), window.open(location.origin, t)
+                                }
+                            }, o.createElement("span", {
+                                className: "pi pi-globe"
                             })), o.createElement("div", {
                                 className: "layout-topbar-icons"
-                            }, "whitewall" === window.App.data.themeName && o.createElement("div", null, o.createElement("a", {
-                                className: e,
+                            }, !window.App.state.site_loading && !window.App.state.site_data.no_user_model && o.createElement(g, (x(e = {
+                                username: window.App.state.user_settings.username,
+                                logged_in: window.App.state.user_settings.logged_in,
+                                authorities: window.App.state.user_settings.authorities,
+                                onActAsSelf: function() {
+                                    return window.App.onAuthoritiesSelect([void 0])
+                                },
+                                su_id: window.App.state.su_id,
+                                su_name: window.App.state.user_settings.su_name,
+                                act_as_subtext: window.App.state.user_settings.act_as_subtext,
+                                act_as_title_text: window.App.state.user_settings.act_as_title_text,
+                                act_as_button_text: window.App.state.user_settings.act_as_button_text,
+                                act_as_self_text: window.App.state.user_settings.act_as_self_text
+                            }, "act_as_self_text", window.App.state.user_settings.act_as_self_text), x(e, "onAuthoritiesSelect", window.App.onAuthoritiesSelect), x(e, "my_setting_text", window.App.state.user_settings.my_setting_text), x(e, "onSignOutIn", (function(e) {
+                                return window.App.onSignOutIn(e)
+                            })), x(e, "createAccount", window.App.createAccount), x(e, "authAppendTo", window.App.topDiv), x(e, "onMysettings", (function(e) {
+                                return window.App.onMysettings(e)
+                            })), e)), "whitewall" === window.App.data.themeName && o.createElement("div", null, o.createElement("a", {
+                                className: t,
                                 onClick: this.props.onHomeButton
                             }, o.createElement("span", null, window.App.state.site_data.site_title))), this.props.useChat && this.renderChatButton()))
                         }
-                    }]) && d(t.prototype, n), Object.defineProperty(t, "prototype", {
+                    }]) && _(t.prototype, n), Object.defineProperty(t, "prototype", {
                         writable: !1
                     }), s
                 }(o.Component);
-                g.defaultProps = {
+                P.defaultProps = {
                     onToggleMenu: null,
                     unseenCount: 0
-                }, g.propTypes = {
-                    onToggleMenu: i().func.isRequired,
-                    onHomeButton: i().func.isRequired,
-                    onChatButton: i().func,
-                    useChat: i().bool,
-                    WS: i().bool,
-                    unseenCount: i().number
+                }, P.propTypes = {
+                    onToggleMenu: l().func.isRequired,
+                    onHomeButton: l().func.isRequired,
+                    onChatButton: l().func,
+                    useChat: l().bool,
+                    WS: l().bool,
+                    unseenCount: l().number
                 }
             },
             1526: (e, t, n) => {
                 "use strict";
                 n.d(t, {
                     n: () => b
                 });
@@ -2352,15 +2385,15 @@
                                 var e = this;
                                 this.setState({
                                     loaded: !1
                                 });
                                 var t = {
                                     fmt: "json"
                                 };
-                                window.App.add_su(t), t[d.xX] = window.App.state.site_data.revision_number, y(this.props.endpoint + "?".concat(a.stringify(t)), {
+                                window.App.add_su(t), t[d.xX] = window.App.state.site_data.revision_number, t[d.fH] = window.App.data.selectedLanguage || window.App.state.user_settings.lang, y(this.props.endpoint + "?".concat(a.stringify(t)), {
                                     signal: this.controller.signal
                                 }).then((function(t) {
                                     return 200 !== t.status ? (e.setState({
                                         placeholder: "Something went wrong"
                                     }), {
                                         status: t.status$
                                     }) : t.json()
@@ -2747,15 +2780,15 @@
                     i = n(5397);
                 r()(i.Z, {
                     insert: "head",
                     singleton: !1
                 }), i.Z.locals;
                 var a = n(2437),
                     l = n(1399),
-                    s = n(4159),
+                    s = (n(6727), n(4159)),
                     p = n.n(s),
                     u = n(2279),
                     c = n.n(u),
                     d = n(6318),
                     f = n.n(d),
                     h = n(6959),
                     m = n.n(h),
@@ -4904,15 +4937,15 @@
                         ! function(e, t) {
                             if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
                         }(this, d), t = u.call(this, e);
                         var n = parseInt(e.widthInCh),
                             o = void 0;
                         e.actorData.display_mode && (o = (0, _.ol)(e.actorData.display_mode, n));
                         var r = (0, _.tq)();
-                        return t.state = {
+                        return window.App.isMobile = r, t.state = {
                             data_view: !!(e.actorData.contain_media || o && [me.do, me.OW, me.UZ].includes(o)),
                             isMobile: r,
                             layout: e.actorData.contain_media ? me.dI : [me.do, me.OW, me.UZ].includes(o) ? o : me.C2,
                             loading: !0,
                             show_top_toolbar: !e.actorData.hide_top_toolbar && !r,
                             showPVDialog: !1,
                             static_page: "show" === e.actorData.default_action,
@@ -4946,25 +4979,39 @@
                             })),
                             sortCol: void 0,
                             sortField: void 0,
                             sortFieldName: void 0,
                             sortOrder: 0,
                             title: "",
                             topRow: 0
-                        }, t.actionWrapper = t.actionWrapper.bind(Ze(t)), t.consumeServerResponse = t.consumeServerResponse.bind(Ze(t)), t.get_current_grid_config = t.get_current_grid_config.bind(Ze(t)), t.get_full_id = t.get_full_id.bind(Ze(t)), t.getData = t.getData.bind(Ze(t)), t.getOne = t.getOne.bind(Ze(t)), t.getUri = t.getUri.bind(Ze(t)), t.handleWindowChange = (0, _.Ds)(t.handleWindowChange.bind(Ze(t)), 50), t.messageInterceptor = t.messageInterceptor.bind(Ze(t)), t.multiRowView = t.multiRowView.bind(Ze(t)), t.onKeyDown = t.onKeyDown.bind(Ze(t)), t.onRowDoubleClick = t.onRowDoubleClick.bind(Ze(t)), t.onSort = t.onSort.bind(Ze(t)), t.refresh = t.refresh.bind(Ze(t)), t.quickFilter = (0, _.Ds)(t.quickFilter.bind(Ze(t)), 200), t.reload = t.reload.bind(Ze(t)), t.reset = t.reset.bind(Ze(t)), t.update_params_values = t.update_params_values.bind(Ze(t)), t.updateUrlValues = t.updateUrlValues.bind(Ze(t)), t
+                        }, t.actionWrapper = t.actionWrapper.bind(Ze(t)), t.consumeServerResponse = t.consumeServerResponse.bind(Ze(t)), t.get_current_grid_config = t.get_current_grid_config.bind(Ze(t)), t.get_full_id = t.get_full_id.bind(Ze(t)), t.getData = t.getData.bind(Ze(t)), t.getOne = t.getOne.bind(Ze(t)), t.getUri = t.getUri.bind(Ze(t)), t.handleWindowChange = (0, _.Ds)(t.handleWindowChange.bind(Ze(t)), 50), t.messageInterceptor = t.messageInterceptor.bind(Ze(t)), t.registerScroll = t.registerScroll.bind(Ze(t)), t.multiRowView = t.multiRowView.bind(Ze(t)), t.onKeyDown = t.onKeyDown.bind(Ze(t)), t.onRowDoubleClick = t.onRowDoubleClick.bind(Ze(t)), t.onSort = t.onSort.bind(Ze(t)), t.refresh = t.refresh.bind(Ze(t)), t.quickFilter = (0, _.Ds)(t.quickFilter.bind(Ze(t)), 200), t.reload = t.reload.bind(Ze(t)), t.reset = t.reset.bind(Ze(t)), t.update_params_values = t.update_params_values.bind(Ze(t)), t.updateUrlValues = t.updateUrlValues.bind(Ze(t)), t
                     }
                     return t = d, n = [{
                         key: "get_full_id",
                         value: function() {
                             return "".concat(this.props.packId, ".").concat(this.props.actorId)
                         }
                     }, {
                         key: "componentDidMount",
                         value: function() {
-                            this.controller = new(m()), this.refresh(), window.addEventListener("resize", this.handleWindowChange), window.addEventListener("keydown", this.onKeyDown), window.addEventListener("message", this.messageInterceptor)
+                            if (this.controller = new(m()), this.refresh(), window.addEventListener("resize", this.handleWindowChange), window.addEventListener("keydown", this.onKeyDown), window.addEventListener("message", this.messageInterceptor), this.props.parentBody) {
+                                window.addEventListener("scroll", this.registerScroll);
+                                var e = this.props.router.history.location.pathname,
+                                    t = window.App.data.scrollIndex,
+                                    n = t.indexOf(e);
+                                n >= 0 ? t.pop(n) : t.length >= 99 && (t.pop(0), delete window.App.data.scroll[e]), t.push(e)
+                            }
+                        }
+                    }, {
+                        key: "registerScroll",
+                        value: function(e) {
+                            this.firstScrollIngonred ? window.App.data.scroll[this.props.router.history.location.pathname] = Object.assign({}, {
+                                scrollX: window.scrollX,
+                                scrollY: window.scrollY
+                            }) : this.firstScrollIngonred = !0
                         }
                     }, {
                         key: "getSnapshotBeforeUpdate",
                         value: function(e, t) {
                             var n = {};
                             (this.props.pk !== e.pk || this.props.mk !== e.mk || this.props.mt !== e.mt || 0 !== e.reload_timestamp && this.props.reload_timestamp !== e.reload_timestamp) && (n.requireRefresh = !0), e.router.match.isExact === this.props.router.match.isExact && e.actorData.detail_action === this.props.actorData.detail_action || (n.detail_window = !this.props.router.match.isExact || "show" === this.props.actorData.default_action);
                             var o = (0, _.eJ)(this.props);
@@ -4974,15 +5021,15 @@
                         key: "componentDidUpdate",
                         value: function(e, t, n) {
                             if (null !== n) return n.hasOwnProperty("id") ? (Object.assign(this.data, n), void this.reload()) : n.hasOwnProperty("detail_window") ? (Object.assign(this.data, n), this.data.id = (0, _.eJ)(this.props), void this.reload()) : void(n.hasOwnProperty("requireRefresh") && this.refresh())
                         }
                     }, {
                         key: "componentWillUnmount",
                         value: function() {
-                            this.controller.abort(), window.removeEventListener("resize", this.handleWindowChange), window.removeEventListener("keydown", this.onKeyDown), window.removeEventListener("message", this.messageInterceptor)
+                            this.controller.abort(), window.removeEventListener("resize", this.handleWindowChange), window.removeEventListener("keydown", this.onKeyDown), window.removeEventListener("message", this.messageInterceptor), this.props.parentBody && window.removeEventListener("scroll", this.registerScroll)
                         }
                     }, {
                         key: "messageInterceptor",
                         value: function(e) {
                             "HomeButtonEvent" === e.data ? this.reset() : "row_selected" === e.data ? this.data.rowSelected = !0 : "none_selected" === e.data && (this.data.rowSelected = !1)
                         }
                     }, {
@@ -5139,15 +5186,15 @@
                                 page: h.page,
                                 query: h.query,
                                 sortFieldName: h.sortFieldName,
                                 sortOrder: h.sortOrder,
                                 topRow: h.page * this.data.rowsPerPage
                             });
                             var m = {};
-                            if (m[me.i5] = me.oi, m[me.qg] = h.page * this.data.rowsPerPage, m[me.EL] = this.data.rowsPerPage, m[me.Vk] = h.query, m[me.mQ] = this.rp || c()(this), m[me.Vp] = h.displayMode, m[me.$S] = me.zf, m[me.xX] = window.App.state.site_data.revision_number, m[me.jT] = window.App.state.site_data.mjsts, void 0 !== h.sortFieldName && (m.sort = h.sortFieldName), 0 !== h.sortOrder && (m.dir = 1 === h.sortOrder ? "ASC" : "DESC"), this.props.actorData.use_detail_params_value && this.props.parent_pv) m.pv = (0, _.ku)(this.props.parent_pv, this.props.actorData.params_fields);
+                            if (m[me.i5] = me.oi, m[me.qg] = h.page * this.data.rowsPerPage, m[me.EL] = this.data.rowsPerPage, m[me.Vk] = h.query, m[me.mQ] = this.rp || c()(this), m[me.Vp] = h.displayMode, m[me.$S] = me.zf, m[me.xX] = window.App.state.site_data.revision_number, m[me.fH] = window.App.data.selectedLanguage || window.App.state.user_settings.lang, m[me.jT] = window.App.state.site_data.mjsts, void 0 !== h.sortFieldName && (m.sort = h.sortFieldName), 0 !== h.sortOrder && (m.dir = 1 === h.sortOrder ? "ASC" : "DESC"), this.props.actorData.use_detail_params_value && this.props.parent_pv) m.pv = (0, _.ku)(this.props.parent_pv, this.props.actorData.params_fields);
                             else if (this.props.actorData.params_layout) {
                                 var b = g.parse(this.props.router.history.location.search);
                                 this.props.inDetail || void 0 !== a || 0 !== Object.keys(this.data.params_values).length ? 0 !== Object.keys(this.data.params_values).length && (m.pv = (0, _.ku)(a || this.data.params_values, this.props.actorData.params_fields)) : m.pv = b.pv
                             }
                             return void 0 !== this.props.mk && null !== this.props.mt && (m.mk = this.props.mk), void 0 !== this.props.mt && null !== this.props.mt && (m.mt = this.props.mt), window.App.add_su(m), m
                         }
                     }, {
@@ -5249,15 +5296,20 @@
                                     });
                                     this.data.detail_window || Object.assign(this.data, {
                                         data: e,
                                         detail_window: !1,
                                         title: e.title || ""
                                     })
                                 }
-                                window.postMessage("body_reload", "*")
+                                if (window.postMessage("body_reload", "*"), this.props.parentBody) {
+                                    var r = window.App.data.scroll[this.props.router.history.location.pathname];
+                                    r && window.requestAnimationFrame((function() {
+                                        window.scroll(r.scrollX, r.scrollY)
+                                    }))
+                                }
                             } else window.postMessage("version_mismatch", "*")
                         }
                     }, {
                         key: "handleWindowChange",
                         value: function(e) {
                             var t = window.innerWidth;
                             document.querySelector(".layout-main .l-header").contains(document.activeElement) || this.state.window_width == t || this.setState({
@@ -14193,15 +14245,15 @@
                         }
                     }, {
                         key: "renderComponent",
                         value: function(e, t) {
                             var n = this,
                                 r = Zn[e],
                                 i = !1;
-                            return void 0 === r && (r = Zn.UnknownElement, console.warn("".concat(e, " does not exist"))), !t.elem.hasOwnProperty("items") && t.elem.editable && (this.inputCount += 1, t.tabIndex = this.inputCount), t.elem.hasOwnProperty("items") || !t.elem.editable || An(t) || !t.editing_mode && !t.inDialog || this.focusibleInput === t.tabIndex && (i = !0), o.createElement(r, vn({}, t, {
+                            return void 0 === r && (r = Zn.UnknownElement, console.warn("".concat(e, " does not exist"))), !t.elem.hasOwnProperty("items") && t.elem.editable && (this.inputCount += 1, t.tabIndex = this.inputCount), window.App.isMobile || t.elem.hasOwnProperty("items") || !t.elem.editable || An(t) || !t.editing_mode && !t.inDialog || this.focusibleInput === t.tabIndex && (i = !0), o.createElement(r, vn({}, t, {
                                 setFocus: i
                             }), t.elem.items && t.elem.items.filter((function(e) {
                                 return !e.hidden
                             })).map((function(e, o) {
                                 var r = {};
                                 return "TabPanel" === t.elem.react_name && (r.tabIndex = o), n.renderComponent(e.react_name, gn(gn({}, t), {}, {
                                     key: p()(e),
@@ -15142,15 +15194,15 @@
                         return y(this, n), (o = t.call(this, e)).state = {
                             query: e.parent.data.query || ""
                         }, o.parent = e.parent, o.controller = new(i()), o.renderActionBar = o.renderActionBar.bind(C(o)), o.renderDataViewSortButton = o.renderDataViewSortButton.bind(C(o)), o.renderDetailNavigator = o.renderDetailNavigator.bind(C(o)), o.renderEditorButton = o.renderEditorButton.bind(C(o)), o.renderParamValueControls = o.renderParamValueControls.bind(C(o)), o.renderQuickFilter = o.renderQuickFilter.bind(C(o)), o.renderToggle_colControls = o.renderToggle_colControls.bind(C(o)), o
                     }
                     return k(n, [{
                         key: "componentDidUpdate",
                         value: function(e, t, n) {
-                            this.parent.data.editing_mode || window.App.data.dialogs.length || "calview" === this.parent.props.packId || this.inputEl && this.inputEl.focus()
+                            window.App.isMobile || this.parent.data.editing_mode || window.App.data.dialogs.length || "calview" === this.parent.props.packId || this.inputEl && this.inputEl.focus()
                         }
                     }, {
                         key: "renderActionBar",
                         value: function(e, t) {
                             return o.createElement(d.Z, {
                                 actorData: this.parent.props.actorData,
                                 disabledFields: this.parent.data.disabled_fields,
@@ -15901,22 +15953,23 @@
                         return t = h, (n = [{
                             key: "getData",
                             value: function(e, t) {
                                 var n = window.localStorage,
                                     o = window.App.state.user_settings,
                                     a = o.user_type,
                                     l = o.lang,
-                                    s = window.App.state.user_settings.su_user_type,
-                                    p = (0, i.ah)(e),
-                                    u = n.getObject(p);
-                                if (u) t(u);
+                                    s = window.App.data.selectedLanguage || l,
+                                    p = window.App.state.user_settings.su_user_type,
+                                    u = (0, i.ah)(e),
+                                    c = n.getObject(u);
+                                if (c) t(c);
                                 else {
-                                    var c = "/media/cache/json/";
-                                    c += window.App.state.site_data.no_user_model ? "Lino_".concat(e, "_").concat(l, ".json") : "Lino_".concat(e, "_").concat(s || a, "_").concat(l, ".json"), c += "?v=".concat(Math.round(1e6 * Math.random()).toString()), (0, r.he)(c).then(window.App.handleAjaxResponse).then((function(e) {
-                                        n.setObject(p, e), t(e)
+                                    var d = "/media/cache/json/";
+                                    d += window.App.state.site_data.no_user_model ? "Lino_".concat(e, "_").concat(s, ".json") : "Lino_".concat(e, "_").concat(p || a, "_").concat(s, ".json"), d += "?v=".concat(Math.round(1e6 * Math.random()).toString()), (0, r.he)(d).then(window.App.handleAjaxResponse).then((function(e) {
+                                        n.setObject(u, e), t(e)
                                     }))
                                 }
                             }
                         }, {
                             key: "componentDidMount",
                             value: function() {
                                 var e = this;
@@ -15993,19 +16046,20 @@
                     Jg: () => b,
                     Vk: () => g,
                     qg: () => v,
                     EL: () => y,
                     i5: () => w,
                     oi: () => k,
                     mQ: () => x,
-                    EO: () => _,
-                    SX: () => E,
-                    Td: () => O,
-                    X8: () => C,
-                    gM: () => S
+                    fH: () => _,
+                    EO: () => E,
+                    SX: () => O,
+                    Td: () => C,
+                    X8: () => S,
+                    gM: () => P
                 });
                 var o = "lv",
                     r = "mjsts",
                     i = "wt",
                     a = "d",
                     l = "p",
                     s = "dm",
@@ -16019,19 +16073,20 @@
                     b = "html",
                     g = "query",
                     v = "start",
                     y = "limit",
                     w = "fmt",
                     k = "json",
                     x = "rp",
-                    _ = "cw",
-                    E = "ch",
-                    O = "ci",
-                    C = ["submit_detail", "delete_selected"],
-                    S = ["tab"]
+                    _ = "ul",
+                    E = "cw",
+                    O = "ch",
+                    C = "ci",
+                    S = ["submit_detail", "delete_selected"],
+                    P = ["tab"]
             },
             5617: (e, t, n) => {
                 "use strict";
                 n.d(t, {
                     n: () => S
                 });
                 var o = n(7268),
```

### Comparing `lino_react-23.3.1/lino_react/react/static/react/main.js.LICENSE.txt` & `lino_react-23.4.0/lino_react/react/static/react/main.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lino_react-23.3.1/lino_react/react/views.py` & `lino_react-23.4.0/lino_react/react/views.py`

 * *Files identical despite different names*

### Comparing `lino_react-23.3.1/lino_react/setup_info.py` & `lino_react-23.4.0/lino_react/setup_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: UTF-8 -*-
 # Copyright 2015-2023 Rumma & Ko Ltd
 # License: GNU Affero General Public License v3 (see file COPYING for details)
 
 SETUP_INFO = dict(
     name='lino_react',
-    version='23.3.1',
+    version='23.4.0',
     install_requires=['lino'],
     tests_require=[],
     test_suite='tests',
     description="The React front end for Lino",
     license_files=['COPYING'],
     include_package_data=False,
     zip_safe=False,
```

### Comparing `lino_react-23.3.1/lino_react.egg-info/PKG-INFO` & `lino_react-23.4.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: lino-react
-Version: 23.3.1
+Name: lino_react
+Version: 23.4.0
 Summary: The React front end for Lino
 Home-page: https://gitlab.com/lino-framework/react
 Author: Rumma & Ko Ltd
 Author-email: info@lino-framework.org
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier:   Programming Language :: Python
```

