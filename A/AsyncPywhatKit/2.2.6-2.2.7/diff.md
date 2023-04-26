# Comparing `tmp/AsyncPywhatKit-2.2.6.tar.gz` & `tmp/AsyncPywhatKit-2.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AsyncPywhatKit-2.2.6.tar", last modified: Sat Apr  1 15:48:45 2023, max compression
+gzip compressed data, was "AsyncPywhatKit-2.2.7.tar", last modified: Tue Apr 25 14:28:48 2023, max compression
```

## Comparing `AsyncPywhatKit-2.2.6.tar` & `AsyncPywhatKit-2.2.7.tar`

### file list

```diff
@@ -1,55 +1,156 @@
-drwxrwxr-x   0 balasai   (1000) balasai   (1000)        0 2023-04-01 15:48:45.124389 AsyncPywhatKit-2.2.6/
-drwxrwxr-x   0 balasai   (1000) balasai   (1000)        0 2023-04-01 15:48:45.120385 AsyncPywhatKit-2.2.6/AsyncPywhatKit/
-drwxrwxr-x   0 balasai   (1000) balasai   (1000)        0 2023-04-01 15:48:45.120385 AsyncPywhatKit-2.2.6/AsyncPywhatKit/docs/
-drwxrwxr-x   0 balasai   (1000) balasai   (1000)        0 2023-04-01 15:48:45.120385 AsyncPywhatKit-2.2.6/AsyncPywhatKit/docs/_build/
-drwxrwxr-x   0 balasai   (1000) balasai   (1000)        0 2023-04-01 15:48:45.120385 AsyncPywhatKit-2.2.6/AsyncPywhatKit/docs/_build/html/
-drwxrwxr-x   0 balasai   (1000) balasai   (1000)        0 2023-04-01 15:48:45.124389 AsyncPywhatKit-2.2.6/AsyncPywhatKit/docs/_build/html/_static/
--rw-rw-r--   0 balasai   (1000) balasai   (1000)      286 2023-04-01 15:17:56.000000 AsyncPywhatKit-2.2.6/AsyncPywhatKit/docs/_build/html/_static/file.png
--rw-rw-r--   0 balasai   (1000) balasai   (1000)       90 2023-04-01 15:17:56.000000 AsyncPywhatKit-2.2.6/AsyncPywhatKit/docs/_build/html/_static/minus.png
--rw-rw-r--   0 balasai   (1000) balasai   (1000)       90 2023-04-01 15:17:56.000000 AsyncPywhatKit-2.2.6/AsyncPywhatKit/docs/_build/html/_static/plus.png
-drwxrwxr-x   0 balasai   (1000) balasai   (1000)        0 2023-04-01 15:48:45.124389 AsyncPywhatKit-2.2.6/AsyncPywhatKit/src/
-drwxrwxr-x   0 balasai   (1000) balasai   (1000)        0 2023-04-01 15:48:45.124389 AsyncPywhatKit-2.2.6/AsyncPywhatKit/src/Core/
--rw-rw-r--   0 balasai   (1000) balasai   (1000)       65 2023-04-01 15:17:56.000000 AsyncPywhatKit-2.2.6/AsyncPywhatKit/src/Core/__init__.py
--rw-rw-r--   0 balasai   (1000) balasai   (1000)     8775 2023-04-01 15:17:56.000000 AsyncPywhatKit-2.2.6/AsyncPywhatKit/src/Core/core.py
-drwxrwxr-x   0 balasai   (1000) balasai   (1000)        0 2023-04-01 15:48:45.124389 AsyncPywhatKit-2.2.6/AsyncPywhatKit/src/Core/data/
--rw-rw-r--   0 balasai   (1000) balasai   (1000)      317 2023-04-01 15:17:56.000000 AsyncPywhatKit-2.2.6/AsyncPywhatKit/src/Core/data/document.png
--rw-rw-r--   0 balasai   (1000) balasai   (1000)      234 2023-04-01 15:17:56.000000 AsyncPywhatKit-2.2.6/AsyncPywhatKit/src/Core/data/img_icon.png
--rw-rw-r--   0 balasai   (1000) balasai   (1000)      496 2023-04-01 15:17:56.000000 AsyncPywhatKit-2.2.6/AsyncPywhatKit/src/Core/data/link.png
--rw-rw-r--   0 balasai   (1000) balasai   (1000)      479 2023-04-01 15:17:56.000000 AsyncPywhatKit-2.2.6/AsyncPywhatKit/src/Core/data/link2.png
--rw-rw-r--   0 balasai   (1000) balasai   (1000)      434 2023-04-01 15:17:56.000000 AsyncPywhatKit-2.2.6/AsyncPywhatKit/src/Core/data/photo_or_video.png
--rw-rw-r--   0 balasai   (1000) balasai   (1000)      629 2023-04-01 15:17:56.000000 AsyncPywhatKit-2.2.6/AsyncPywhatKit/src/Core/data/pywhatkit_smile.png
--rw-rw-r--   0 balasai   (1000) balasai   (1000)      656 2023-04-01 15:17:56.000000 AsyncPywhatKit-2.2.6/AsyncPywhatKit/src/Core/data/pywhatkit_smile1.png
--rw-rw-r--   0 balasai   (1000) balasai   (1000)     2161 2023-04-01 15:17:56.000000 AsyncPywhatKit-2.2.6/AsyncPywhatKit/src/Core/data/searchbar2.png
--rw-rw-r--   0 balasai   (1000) balasai   (1000)      787 2023-04-01 15:17:56.000000 AsyncPywhatKit-2.2.6/AsyncPywhatKit/src/Core/data/unread_icon.png
--rw-rw-r--   0 balasai   (1000) balasai   (1000)      840 2023-04-01 15:17:56.000000 AsyncPywhatKit-2.2.6/AsyncPywhatKit/src/Core/exceptions.py
--rw-rw-r--   0 balasai   (1000) balasai   (1000)     2307 2023-04-01 15:17:56.000000 AsyncPywhatKit-2.2.6/AsyncPywhatKit/src/Core/log.py
--rw-rw-r--   0 balasai   (1000) balasai   (1000)      715 2023-04-01 15:27:45.000000 AsyncPywhatKit-2.2.6/AsyncPywhatKit/src/__init__.py
--rw-rw-r--   0 balasai   (1000) balasai   (1000)      934 2023-04-01 15:17:56.000000 AsyncPywhatKit-2.2.6/AsyncPywhatKit/src/ascii_art.py
--rw-rw-r--   0 balasai   (1000) balasai   (1000)      781 2023-04-01 15:17:56.000000 AsyncPywhatKit-2.2.6/AsyncPywhatKit/src/handwriting.py
--rw-rw-r--   0 balasai   (1000) balasai   (1000)     1448 2023-04-01 15:17:56.000000 AsyncPywhatKit-2.2.6/AsyncPywhatKit/src/mail.py
--rw-rw-r--   0 balasai   (1000) balasai   (1000)     2815 2023-04-01 15:17:56.000000 AsyncPywhatKit-2.2.6/AsyncPywhatKit/src/misc.py
--rw-rw-r--   0 balasai   (1000) balasai   (1000)     7884 2023-04-01 15:17:56.000000 AsyncPywhatKit-2.2.6/AsyncPywhatKit/src/remotekit.py
--rw-rw-r--   0 balasai   (1000) balasai   (1000)     1792 2023-04-01 15:17:56.000000 AsyncPywhatKit-2.2.6/AsyncPywhatKit/src/sc.py
--rw-rw-r--   0 balasai   (1000) balasai   (1000)    12045 2023-04-01 15:44:50.000000 AsyncPywhatKit-2.2.6/AsyncPywhatKit/src/whats.py
-drwxrwxr-x   0 balasai   (1000) balasai   (1000)        0 2023-04-01 15:48:45.124389 AsyncPywhatKit-2.2.6/AsyncPywhatKit.egg-info/
--rw-rw-r--   0 balasai   (1000) balasai   (1000)     5393 2023-04-01 15:48:45.000000 AsyncPywhatKit-2.2.6/AsyncPywhatKit.egg-info/PKG-INFO
--rw-rw-r--   0 balasai   (1000) balasai   (1000)     1343 2023-04-01 15:48:45.000000 AsyncPywhatKit-2.2.6/AsyncPywhatKit.egg-info/SOURCES.txt
--rw-rw-r--   0 balasai   (1000) balasai   (1000)        1 2023-04-01 15:48:45.000000 AsyncPywhatKit-2.2.6/AsyncPywhatKit.egg-info/dependency_links.txt
--rw-rw-r--   0 balasai   (1000) balasai   (1000)      164 2023-04-01 15:48:45.000000 AsyncPywhatKit-2.2.6/AsyncPywhatKit.egg-info/requires.txt
--rw-rw-r--   0 balasai   (1000) balasai   (1000)       15 2023-04-01 15:48:45.000000 AsyncPywhatKit-2.2.6/AsyncPywhatKit.egg-info/top_level.txt
--rw-rw-r--   0 balasai   (1000) balasai   (1000)    11350 2023-04-01 15:17:56.000000 AsyncPywhatKit-2.2.6/LICENSE.md
--rw-rw-r--   0 balasai   (1000) balasai   (1000)       94 2023-04-01 15:48:38.000000 AsyncPywhatKit-2.2.6/MANIFEST.in
--rw-rw-r--   0 balasai   (1000) balasai   (1000)     5393 2023-04-01 15:48:45.124389 AsyncPywhatKit-2.2.6/PKG-INFO
--rw-rw-r--   0 balasai   (1000) balasai   (1000)     4447 2023-04-01 15:17:56.000000 AsyncPywhatKit-2.2.6/README.md
--rw-rw-r--   0 balasai   (1000) balasai   (1000)       38 2023-04-01 15:48:45.124389 AsyncPywhatKit-2.2.6/setup.cfg
--rw-rw-r--   0 balasai   (1000) balasai   (1000)     1604 2023-04-01 15:41:33.000000 AsyncPywhatKit-2.2.6/setup.py
-drwxrwxr-x   0 balasai   (1000) balasai   (1000)        0 2023-04-01 15:48:45.120385 AsyncPywhatKit-2.2.6/venv/
-drwxrwxr-x   0 balasai   (1000) balasai   (1000)        0 2023-04-01 15:48:45.120385 AsyncPywhatKit-2.2.6/venv/lib/
-drwxrwxr-x   0 balasai   (1000) balasai   (1000)        0 2023-04-01 15:48:45.120385 AsyncPywhatKit-2.2.6/venv/lib/python3.8/
-drwxrwxr-x   0 balasai   (1000) balasai   (1000)        0 2023-04-01 15:48:45.120385 AsyncPywhatKit-2.2.6/venv/lib/python3.8/site-packages/
-drwxrwxr-x   0 balasai   (1000) balasai   (1000)        0 2023-04-01 15:48:45.124389 AsyncPywhatKit-2.2.6/venv/lib/python3.8/site-packages/werkzeug/
-drwxrwxr-x   0 balasai   (1000) balasai   (1000)        0 2023-04-01 15:48:45.124389 AsyncPywhatKit-2.2.6/venv/lib/python3.8/site-packages/werkzeug/debug/
-drwxrwxr-x   0 balasai   (1000) balasai   (1000)        0 2023-04-01 15:48:45.124389 AsyncPywhatKit-2.2.6/venv/lib/python3.8/site-packages/werkzeug/debug/shared/
--rw-rw-r--   0 balasai   (1000) balasai   (1000)      507 2023-04-01 15:21:54.000000 AsyncPywhatKit-2.2.6/venv/lib/python3.8/site-packages/werkzeug/debug/shared/console.png
--rw-rw-r--   0 balasai   (1000) balasai   (1000)      191 2023-04-01 15:21:54.000000 AsyncPywhatKit-2.2.6/venv/lib/python3.8/site-packages/werkzeug/debug/shared/less.png
--rw-rw-r--   0 balasai   (1000) balasai   (1000)      200 2023-04-01 15:21:54.000000 AsyncPywhatKit-2.2.6/venv/lib/python3.8/site-packages/werkzeug/debug/shared/more.png
+drwxrwxrwx   0        0        0        0 2023-04-25 14:28:48.124290 AsyncPywhatKit-2.2.7/
+drwxrwxrwx   0        0        0        0 2023-04-25 14:28:47.766130 AsyncPywhatKit-2.2.7/.github/
+-rw-rw-rw-   0        0        0      706 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/.github/FUNDING.yml
+drwxrwxrwx   0        0        0        0 2023-04-25 14:28:47.772786 AsyncPywhatKit-2.2.7/.idea/
+-rw-rw-rw-   0        0        0      452 2023-04-25 13:55:47.000000 AsyncPywhatKit-2.2.7/.idea/AsyncPywhatKit.iml
+drwxrwxrwx   0        0        0        0 2023-04-25 14:28:47.772786 AsyncPywhatKit-2.2.7/.idea/inspectionProfiles/
+-rw-rw-rw-   0        0        0     1641 2023-04-25 13:55:47.000000 AsyncPywhatKit-2.2.7/.idea/inspectionProfiles/Project_Default.xml
+-rw-rw-rw-   0        0        0      174 2023-04-25 13:55:47.000000 AsyncPywhatKit-2.2.7/.idea/inspectionProfiles/profiles_settings.xml
+-rw-rw-rw-   0        0        0      287 2023-04-25 13:55:47.000000 AsyncPywhatKit-2.2.7/.idea/modules.xml
+-rw-rw-rw-   0        0        0      172 2023-04-25 13:55:47.000000 AsyncPywhatKit-2.2.7/.idea/vcs.xml
+drwxrwxrwx   0        0        0        0 2023-04-25 14:28:47.772786 AsyncPywhatKit-2.2.7/AsyncPywhatKit/
+-rw-rw-rw-   0        0        0       69 2023-04-25 01:14:18.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 14:28:47.813852 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/
+-rw-rw-rw-   0        0        0      654 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-04-25 14:28:47.724685 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/
+drwxrwxrwx   0        0        0        0 2023-04-25 14:28:47.831722 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/doctrees/
+-rw-rw-rw-   0        0        0    93627 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/doctrees/environment.pickle
+-rw-rw-rw-   0        0        0     5037 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/doctrees/index.doctree
+-rw-rw-rw-   0        0        0     2704 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/doctrees/modules.doctree
+-rw-rw-rw-   0        0        0    51929 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/doctrees/src.Core.doctree
+-rw-rw-rw-   0        0        0   138274 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/doctrees/src.doctree
+drwxrwxrwx   0        0        0        0 2023-04-25 14:28:47.851042 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/html/
+-rw-rw-rw-   0        0        0      234 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/html/.buildinfo
+drwxrwxrwx   0        0        0        0 2023-04-25 14:28:47.866844 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/html/_modules/
+-rw-rw-rw-   0        0        0     3983 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/html/_modules/index.html
+drwxrwxrwx   0        0        0        0 2023-04-25 14:28:47.883373 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/html/_modules/src/
+drwxrwxrwx   0        0        0        0 2023-04-25 14:28:47.898415 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/html/_modules/src/Core/
+-rw-rw-rw-   0        0        0    28427 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/html/_modules/src/Core/core.html
+-rw-rw-rw-   0        0        0     6931 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/html/_modules/src/Core/exceptions.html
+-rw-rw-rw-   0        0        0    18133 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/html/_modules/src/Core/log.html
+-rw-rw-rw-   0        0        0     9377 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/html/_modules/src/ascii_art.html
+-rw-rw-rw-   0        0        0     7644 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/html/_modules/src/handwriting.html
+-rw-rw-rw-   0        0        0    10995 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/html/_modules/src/mail.html
+-rw-rw-rw-   0        0        0    17872 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/html/_modules/src/misc.html
+-rw-rw-rw-   0        0        0    34189 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/html/_modules/src/remotekit.html
+-rw-rw-rw-   0        0        0    11609 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/html/_modules/src/sc.html
+-rw-rw-rw-   0        0        0    52364 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/html/_modules/src/whats.html
+drwxrwxrwx   0        0        0        0 2023-04-25 14:28:47.904611 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/html/_sources/
+-rw-rw-rw-   0        0        0      478 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/html/_sources/index.rst.txt
+-rw-rw-rw-   0        0        0       53 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/html/_sources/modules.rst.txt
+-rw-rw-rw-   0        0        0      606 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/html/_sources/src.Core.rst.txt
+-rw-rw-rw-   0        0        0     1141 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/html/_sources/src.rst.txt
+drwxrwxrwx   0        0        0        0 2023-04-25 14:28:47.946747 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/html/_static/
+-rw-rw-rw-   0        0        0     4552 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/html/_static/_sphinx_javascript_frameworks_compat.js
+-rw-rw-rw-   0        0        0    15519 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/html/_static/basic.css
+drwxrwxrwx   0        0        0        0 2023-04-25 14:28:47.946747 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/html/_static/css/
+-rw-rw-rw-   0        0        0     3229 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/html/_static/css/badge_only.css
+drwxrwxrwx   0        0        0        0 2023-04-25 14:28:48.024845 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/html/_static/css/fonts/
+-rw-rw-rw-   0        0        0    87624 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff
+-rw-rw-rw-   0        0        0    67312 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
+-rw-rw-rw-   0        0        0    86288 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff
+-rw-rw-rw-   0        0        0    66444 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
+-rw-rw-rw-   0        0        0   165742 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot
+-rw-rw-rw-   0        0        0   447050 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg
+-rw-rw-rw-   0        0        0   165548 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf
+-rw-rw-rw-   0        0        0    98024 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff
+-rw-rw-rw-   0        0        0    77160 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2
+-rw-rw-rw-   0        0        0   323344 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/html/_static/css/fonts/lato-bold-italic.woff
+-rw-rw-rw-   0        0        0   193308 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/html/_static/css/fonts/lato-bold-italic.woff2
+-rw-rw-rw-   0        0        0   309728 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/html/_static/css/fonts/lato-bold.woff
+-rw-rw-rw-   0        0        0   184912 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/html/_static/css/fonts/lato-bold.woff2
+-rw-rw-rw-   0        0        0   328412 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/html/_static/css/fonts/lato-normal-italic.woff
+-rw-rw-rw-   0        0        0   195704 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/html/_static/css/fonts/lato-normal-italic.woff2
+-rw-rw-rw-   0        0        0   309192 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/html/_static/css/fonts/lato-normal.woff
+-rw-rw-rw-   0        0        0   182708 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/html/_static/css/fonts/lato-normal.woff2
+-rw-rw-rw-   0        0        0   131660 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/html/_static/css/theme.css
+-rw-rw-rw-   0        0        0     4628 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/html/_static/doctools.js
+-rw-rw-rw-   0        0        0      435 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/html/_static/documentation_options.js
+-rw-rw-rw-   0        0        0      286 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/html/_static/file.png
+-rw-rw-rw-   0        0        0   299461 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/html/_static/jquery-3.6.0.js
+-rw-rw-rw-   0        0        0    89503 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/html/_static/jquery.js
+drwxrwxrwx   0        0        0        0 2023-04-25 14:28:48.027501 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/html/_static/js/
+-rw-rw-rw-   0        0        0      934 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/html/_static/js/badge_only.js
+-rw-rw-rw-   0        0        0     4373 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/html/_static/js/html5shiv-printshiv.min.js
+-rw-rw-rw-   0        0        0     2737 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/html/_static/js/html5shiv.min.js
+-rw-rw-rw-   0        0        0     5023 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/html/_static/js/theme.js
+-rw-rw-rw-   0        0        0     4957 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/html/_static/language_data.js
+-rw-rw-rw-   0        0        0       90 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/html/_static/minus.png
+-rw-rw-rw-   0        0        0       90 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/html/_static/plus.png
+-rw-rw-rw-   0        0        0     4892 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/html/_static/pygments.css
+-rw-rw-rw-   0        0        0    18781 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/html/_static/searchtools.js
+-rw-rw-rw-   0        0        0     4856 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/html/_static/sphinx_highlight.js
+-rw-rw-rw-   0        0        0    70462 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/html/_static/underscore-1.13.1.js
+-rw-rw-rw-   0        0        0    19535 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/html/_static/underscore.js
+-rw-rw-rw-   0        0        0    14094 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/html/genindex.html
+-rw-rw-rw-   0        0        0     4550 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/html/index.html
+-rw-rw-rw-   0        0        0    11393 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/html/modules.html
+-rw-rw-rw-   0        0        0      808 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/html/objects.inv
+-rw-rw-rw-   0        0        0     6136 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/html/py-modindex.html
+-rw-rw-rw-   0        0        0     3775 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/html/search.html
+-rw-rw-rw-   0        0        0    12074 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/html/searchindex.js
+-rw-rw-rw-   0        0        0    26114 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/html/src.Core.html
+-rw-rw-rw-   0        0        0    63958 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/_build/html/src.html
+-rw-rw-rw-   0        0        0     1200 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/conf.py
+-rw-rw-rw-   0        0        0      478 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/index.rst
+-rwxrwxrwx   0        0        0      800 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/make.bat
+-rw-rw-rw-   0        0        0       53 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/modules.rst
+-rw-rw-rw-   0        0        0      606 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/src.Core.rst
+-rw-rw-rw-   0        0        0     1141 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/docs/src.rst
+drwxrwxrwx   0        0        0        0 2023-04-25 14:28:48.056978 AsyncPywhatKit-2.2.7/AsyncPywhatKit/src/
+drwxrwxrwx   0        0        0        0 2023-04-25 14:28:48.063164 AsyncPywhatKit-2.2.7/AsyncPywhatKit/src/Core/
+-rw-rw-rw-   0        0        0       68 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/src/Core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 14:28:48.076918 AsyncPywhatKit-2.2.7/AsyncPywhatKit/src/Core/__pycache__/
+-rw-rw-rw-   0        0        0      232 2023-04-24 06:35:01.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/src/Core/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     7926 2023-04-24 06:35:01.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/src/Core/__pycache__/core.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1533 2023-04-24 06:35:01.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/src/Core/__pycache__/exceptions.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1994 2023-04-24 06:35:02.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/src/Core/__pycache__/log.cpython-310.pyc
+-rw-rw-rw-   0        0        0     9080 2023-04-24 06:53:09.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/src/Core/core.py
+drwxrwxrwx   0        0        0        0 2023-04-25 14:28:48.104202 AsyncPywhatKit-2.2.7/AsyncPywhatKit/src/Core/data/
+-rw-rw-rw-   0        0        0      317 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/src/Core/data/document.png
+-rw-rw-rw-   0        0        0      234 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/src/Core/data/img_icon.png
+-rw-rw-rw-   0        0        0      496 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/src/Core/data/link.png
+-rw-rw-rw-   0        0        0      479 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/src/Core/data/link2.png
+-rw-rw-rw-   0        0        0      434 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/src/Core/data/photo_or_video.png
+-rw-rw-rw-   0        0        0      629 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/src/Core/data/pywhatkit_smile.png
+-rw-rw-rw-   0        0        0      656 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/src/Core/data/pywhatkit_smile1.png
+-rw-rw-rw-   0        0        0     2161 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/src/Core/data/searchbar2.png
+-rw-rw-rw-   0        0        0      787 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/src/Core/data/unread_icon.png
+-rw-rw-rw-   0        0        0      889 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/src/Core/exceptions.py
+-rw-rw-rw-   0        0        0     2375 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/src/Core/log.py
+-rw-rw-rw-   0        0        0        0 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/src/MANIFEST.in
+-rw-rw-rw-   0        0        0      739 2023-04-05 09:47:58.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 14:28:48.124290 AsyncPywhatKit-2.2.7/AsyncPywhatKit/src/__pycache__/
+-rw-rw-rw-   0        0        0     1058 2023-04-24 06:33:10.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/src/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1297 2023-04-24 06:33:10.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/src/__pycache__/ascii_art.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1114 2023-04-24 06:35:02.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/src/__pycache__/handwriting.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1522 2023-04-24 06:35:02.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/src/__pycache__/mail.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3012 2023-04-24 06:35:02.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/src/__pycache__/misc.cpython-310.pyc
+-rw-rw-rw-   0        0        0     8226 2023-04-24 06:35:05.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/src/__pycache__/remotekit.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1608 2023-04-24 06:35:02.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/src/__pycache__/sc.cpython-310.pyc
+-rw-rw-rw-   0        0        0    10816 2023-04-24 06:35:02.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/src/__pycache__/whats.cpython-310.pyc
+-rw-rw-rw-   0        0        0      968 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/src/ascii_art.py
+-rw-rw-rw-   0        0        0      799 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/src/handwriting.py
+-rw-rw-rw-   0        0        0     1504 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/src/mail.py
+-rw-rw-rw-   0        0        0     2903 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/src/misc.py
+-rw-rw-rw-   0        0        0        0 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/src/py.typed
+-rw-rw-rw-   0        0        0     8207 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/src/remotekit.py
+-rw-rw-rw-   0        0        0     1854 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/src/sc.py
+-rw-rw-rw-   0        0        0    13006 2023-04-25 13:59:28.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit/src/whats.py
+drwxrwxrwx   0        0        0        0 2023-04-25 14:28:47.794075 AsyncPywhatKit-2.2.7/AsyncPywhatKit.egg-info/
+-rw-rw-rw-   0        0        0     5501 2023-04-25 14:28:47.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6211 2023-04-25 14:28:47.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 14:28:47.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       79 2023-04-25 14:28:47.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-25 14:28:47.000000 AsyncPywhatKit-2.2.7/AsyncPywhatKit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3690 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0    11551 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/LICENSE.md
+-rw-rw-rw-   0        0        0       31 2023-04-24 06:12:23.000000 AsyncPywhatKit-2.2.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     5501 2023-04-25 14:28:48.124290 AsyncPywhatKit-2.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0     4534 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/README.md
+-rwxrwxrwx   0        0        0       92 2023-04-24 06:42:48.000000 AsyncPywhatKit-2.2.7/build.bat
+-rwxrwxrwx   0        0        0      126 2023-04-24 06:41:10.000000 AsyncPywhatKit-2.2.7/build_and_deploy.bat
+-rw-rw-rw-   0        0        0       66 2023-04-01 13:36:13.000000 AsyncPywhatKit-2.2.7/requirements-dev.txt
+-rw-rw-rw-   0        0        0       86 2023-04-24 06:23:31.000000 AsyncPywhatKit-2.2.7/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-25 14:28:48.124290 AsyncPywhatKit-2.2.7/setup.cfg
+-rw-rw-rw-   0        0        0     1694 2023-04-25 14:28:06.000000 AsyncPywhatKit-2.2.7/setup.py
```

### Comparing `AsyncPywhatKit-2.2.6/AsyncPywhatKit/src/Core/data/pywhatkit_smile.png` & `AsyncPywhatKit-2.2.7/AsyncPywhatKit/src/Core/data/pywhatkit_smile.png`

 * *Files identical despite different names*

### Comparing `AsyncPywhatKit-2.2.6/AsyncPywhatKit/src/Core/data/pywhatkit_smile1.png` & `AsyncPywhatKit-2.2.7/AsyncPywhatKit/src/Core/data/pywhatkit_smile1.png`

 * *Files identical despite different names*

### Comparing `AsyncPywhatKit-2.2.6/AsyncPywhatKit/src/Core/data/searchbar2.png` & `AsyncPywhatKit-2.2.7/AsyncPywhatKit/src/Core/data/searchbar2.png`

 * *Files identical despite different names*

### Comparing `AsyncPywhatKit-2.2.6/AsyncPywhatKit/src/Core/data/unread_icon.png` & `AsyncPywhatKit-2.2.7/AsyncPywhatKit/src/Core/data/unread_icon.png`

 * *Files identical despite different names*

### Comparing `AsyncPywhatKit-2.2.6/AsyncPywhatKit/src/Core/log.py` & `AsyncPywhatKit-2.2.7/AsyncPywhatKit/src/Core/log.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,68 +1,68 @@
-import os
-import time
-
-from .core import check_number
-
-
-async def format_message(message: str) -> str:
-    """Formats the Message to remove redundant Spaces and Newline chars"""
-    msg_l = message.split(" ")
-    new = []
-    for x in msg_l:
-        if "\n" in x:
-            x = x.replace("\n", "")
-            new.append(x) if not len(x) == 0 else None
-
-        elif len(x) != 0:
-            new.append(x)
-
-    return " ".join(new)
-
-
-async def log_message(_time: time.struct_time, receiver: str, message: str) -> None:
-    """Logs the Message Information after it is Sent"""
-
-    if not os.path.exists("PyWhatKit_DB.txt"):
-        file = open("PyWhatKit_DB.txt", "w+")
-        file.close()
-
-    message = await format_message(message)
-
-    with open("PyWhatKit_DB.txt", "a", encoding="utf-8") as file:
-        if await check_number(receiver):
-            file.write(
-                f"Date: {_time.tm_mday}/{_time.tm_mon}/{_time.tm_year}\nTime: {_time.tm_hour}:{_time.tm_min}\n"
-                f"Phone Number: {receiver}\nMessage: {message}"
-            )
-        else:
-            file.write(
-                f"Date: {_time.tm_mday}/{_time.tm_mon}/{_time.tm_year}\nTime: {_time.tm_hour}:{_time.tm_min}\n"
-                f"Group ID: {receiver}\nMessage: {message}"
-            )
-        file.write("\n--------------------\n")
-        file.close()
-
-
-async def log_image(_time: time.struct_time, path: str, receiver: str, caption: str) -> None:
-    """Logs the Image Information after it is Sent"""
-
-    if not os.path.exists("PyWhatKit_DB.txt"):
-        file = open("PyWhatKit_DB.txt", "w+")
-        file.close()
-
-    caption = format_message(caption)
-
-    with open("PyWhatKit_DB.txt", "a", encoding="utf-8") as file:
-        if await check_number(number=receiver):
-            file.write(
-                f"Date: {_time.tm_mday}/{_time.tm_mon}/{_time.tm_year}\nTime: {_time.tm_hour}:{_time.tm_min}\n"
-                f"Phone Number: {receiver}\nImage: {path}\nCaption: {caption}"
-            )
-
-        else:
-            file.write(
-                f"Date: {_time.tm_mday}/{_time.tm_mon}/{_time.tm_year}\nTime: {_time.tm_hour}:{_time.tm_min}\n"
-                f"Group ID: {receiver}\nImage: {path}\nCaption: {caption}"
-            )
-        file.write("\n--------------------\n")
-        file.close()
+import os
+import time
+
+from .core import check_number
+
+
+async def format_message(message: str) -> str:
+    """Formats the Message to remove redundant Spaces and Newline chars"""
+    msg_l = message.split(" ")
+    new = []
+    for x in msg_l:
+        if "\n" in x:
+            x = x.replace("\n", "")
+            new.append(x) if not len(x) == 0 else None
+
+        elif len(x) != 0:
+            new.append(x)
+
+    return " ".join(new)
+
+
+async def log_message(_time: time.struct_time, receiver: str, message: str) -> None:
+    """Logs the Message Information after it is Sent"""
+
+    if not os.path.exists("PyWhatKit_DB.txt"):
+        file = open("PyWhatKit_DB.txt", "w+")
+        file.close()
+
+    message = await format_message(message)
+
+    with open("PyWhatKit_DB.txt", "a", encoding="utf-8") as file:
+        if await check_number(receiver):
+            file.write(
+                f"Date: {_time.tm_mday}/{_time.tm_mon}/{_time.tm_year}\nTime: {_time.tm_hour}:{_time.tm_min}\n"
+                f"Phone Number: {receiver}\nMessage: {message}"
+            )
+        else:
+            file.write(
+                f"Date: {_time.tm_mday}/{_time.tm_mon}/{_time.tm_year}\nTime: {_time.tm_hour}:{_time.tm_min}\n"
+                f"Group ID: {receiver}\nMessage: {message}"
+            )
+        file.write("\n--------------------\n")
+        file.close()
+
+
+async def log_image(_time: time.struct_time, path: str, receiver: str, caption: str) -> None:
+    """Logs the Image Information after it is Sent"""
+
+    if not os.path.exists("PyWhatKit_DB.txt"):
+        file = open("PyWhatKit_DB.txt", "w+")
+        file.close()
+
+    caption = format_message(caption)
+
+    with open("PyWhatKit_DB.txt", "a", encoding="utf-8") as file:
+        if await check_number(number=receiver):
+            file.write(
+                f"Date: {_time.tm_mday}/{_time.tm_mon}/{_time.tm_year}\nTime: {_time.tm_hour}:{_time.tm_min}\n"
+                f"Phone Number: {receiver}\nImage: {path}\nCaption: {caption}"
+            )
+
+        else:
+            file.write(
+                f"Date: {_time.tm_mday}/{_time.tm_mon}/{_time.tm_year}\nTime: {_time.tm_hour}:{_time.tm_min}\n"
+                f"Group ID: {receiver}\nImage: {path}\nCaption: {caption}"
+            )
+        file.write("\n--------------------\n")
+        file.close()
```

### Comparing `AsyncPywhatKit-2.2.6/AsyncPywhatKit/src/ascii_art.py` & `AsyncPywhatKit-2.2.7/AsyncPywhatKit/src/ascii_art.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-from typing import Optional
-
-from PIL import Image
-
-
-async def image_to_ascii_art(
-    img_path: str, output_file: Optional[str] = "pywhatkit_asciiart"
-) -> str:
-    """Convert an Image to ASCII Art"""
-
-    img = Image.open(img_path).convert("L")
-
-    width, height = img.size
-    aspect_ratio = height / width
-    new_width = 80
-    new_height = aspect_ratio * new_width * 0.55
-    img = img.resize((new_width, int(new_height)))
-
-    pixels = img.getdata()
-
-    chars = ["*", "S", "#", "&", "@", "$", "%", "*", "!", ":", "."]
-    new_pixels = [chars[pixel // 25] for pixel in pixels]
-    new_pixels = "".join(new_pixels)
-
-    new_pixels_count = len(new_pixels)
-    ascii_image = [
-        new_pixels[index : index + new_width]
-        for index in range(0, new_pixels_count, new_width)
-    ]
-    ascii_image = "\n".join(ascii_image)
-
-    with open(f"{output_file}.txt", "w") as f:
-        f.write(ascii_image)
-    return ascii_image
+from typing import Optional
+
+from PIL import Image
+
+
+async def image_to_ascii_art(
+    img_path: str, output_file: Optional[str] = "pywhatkit_asciiart"
+) -> str:
+    """Convert an Image to ASCII Art"""
+
+    img = Image.open(img_path).convert("L")
+
+    width, height = img.size
+    aspect_ratio = height / width
+    new_width = 80
+    new_height = aspect_ratio * new_width * 0.55
+    img = img.resize((new_width, int(new_height)))
+
+    pixels = img.getdata()
+
+    chars = ["*", "S", "#", "&", "@", "$", "%", "*", "!", ":", "."]
+    new_pixels = [chars[pixel // 25] for pixel in pixels]
+    new_pixels = "".join(new_pixels)
+
+    new_pixels_count = len(new_pixels)
+    ascii_image = [
+        new_pixels[index : index + new_width]
+        for index in range(0, new_pixels_count, new_width)
+    ]
+    ascii_image = "\n".join(ascii_image)
+
+    with open(f"{output_file}.txt", "w") as f:
+        f.write(ascii_image)
+    return ascii_image
```

### Comparing `AsyncPywhatKit-2.2.6/AsyncPywhatKit/src/handwriting.py` & `AsyncPywhatKit-2.2.7/AsyncPywhatKit/src/handwriting.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-import aiohttp
-
-from AsyncPywhatKit.src.Core import exceptions
-
-
-async def text_to_handwriting(
-    string: str, save_to: str = "pywhatkit.png", rgb: tuple = (0, 0, 0)
-) -> None:
-    """Convert the given String to Handwritten Characters"""
-    async with aiohttp.ClientSession() as session:
-        async with session.get(f"https://pywhatkit.herokuapp.com/handwriting?text={string}&rgb={rgb[0]},{rgb[1]},{rgb[2]}") as response:
-            status_code = response.status
-            if status_code == 200:
-                with open(save_to, "wb") as file:
-                    file.write(await response.read())
-                    file.close()
-            elif 400 <= status_code <= 599:
-                raise exceptions.UnableToAccessApi("Unable to access Pywhatkit api right now")
+import aiohttp
+
+from AsyncPywhatKit.src.Core import exceptions
+
+
+async def text_to_handwriting(
+    string: str, save_to: str = "pywhatkit.png", rgb: tuple = (0, 0, 0)
+) -> None:
+    """Convert the given String to Handwritten Characters"""
+    async with aiohttp.ClientSession() as session:
+        async with session.get(f"https://pywhatkit.herokuapp.com/handwriting?text={string}&rgb={rgb[0]},{rgb[1]},{rgb[2]}") as response:
+            status_code = response.status
+            if status_code == 200:
+                with open(save_to, "wb") as file:
+                    file.write(await response.read())
+                    file.close()
+            elif 400 <= status_code <= 599:
+                raise exceptions.UnableToAccessApi("Unable to access Pywhatkit api right now")
```

### Comparing `AsyncPywhatKit-2.2.6/AsyncPywhatKit/src/mail.py` & `AsyncPywhatKit-2.2.7/AsyncPywhatKit/src/mail.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-import re
-import smtplib
-from email.message import EmailMessage
-from email.mime.text import MIMEText
-from typing import Union
-
-from .Core.exceptions import UnsupportedEmailProvider
-
-
-async def send_mail(
-    email_sender: str,
-    password: str,
-    subject: str,
-    message: Union[str, MIMEText],
-    email_receiver: str,
-) -> None:
-    """Send an Email"""
-
-    domain = re.search("(?<=@)[^.]+(?=\\.)", email_sender)
-
-    hostnames = {
-        "gmail": "smtp.gmail.com",
-        "yahoo": "smtp.mail.yahoo.com",
-        "outlook": "smtp.live.com",
-        "aol": "smtp.aol.com",
-    }
-
-    hostname = None
-    for x in hostnames:
-        if x == domain.group():
-            hostname = hostnames[x]
-            break
-
-    if hostname is None:
-        raise UnsupportedEmailProvider(f"{domain.group()} is not Supported Currently!")
-
-    with smtplib.SMTP_SSL(hostname, 465) as smtp:
-        smtp.login(email_sender, password)
-
-        msg = EmailMessage()
-        msg["Subject"] = subject
-        msg["From"] = email_sender
-        msg["To"] = email_receiver
-        msg.set_content(message)
-
-        smtp.send_message(msg)
-        print("Email Sent Successfully!")
-
-
-async def send_hmail(
-    email_sender: str, password: str, subject: str, html_code: str, email_receiver: str
-) -> None:
-    """Send an Email with HTML Code"""
-
-    message = MIMEText(html_code, "html")
-    await send_mail(email_sender, password, subject, message, email_receiver)
+import re
+import smtplib
+from email.message import EmailMessage
+from email.mime.text import MIMEText
+from typing import Union
+
+from .Core.exceptions import UnsupportedEmailProvider
+
+
+async def send_mail(
+    email_sender: str,
+    password: str,
+    subject: str,
+    message: Union[str, MIMEText],
+    email_receiver: str,
+) -> None:
+    """Send an Email"""
+
+    domain = re.search("(?<=@)[^.]+(?=\\.)", email_sender)
+
+    hostnames = {
+        "gmail": "smtp.gmail.com",
+        "yahoo": "smtp.mail.yahoo.com",
+        "outlook": "smtp.live.com",
+        "aol": "smtp.aol.com",
+    }
+
+    hostname = None
+    for x in hostnames:
+        if x == domain.group():
+            hostname = hostnames[x]
+            break
+
+    if hostname is None:
+        raise UnsupportedEmailProvider(f"{domain.group()} is not Supported Currently!")
+
+    with smtplib.SMTP_SSL(hostname, 465) as smtp:
+        smtp.login(email_sender, password)
+
+        msg = EmailMessage()
+        msg["Subject"] = subject
+        msg["From"] = email_sender
+        msg["To"] = email_receiver
+        msg.set_content(message)
+
+        smtp.send_message(msg)
+        print("Email Sent Successfully!")
+
+
+async def send_hmail(
+    email_sender: str, password: str, subject: str, html_code: str, email_receiver: str
+) -> None:
+    """Send an Email with HTML Code"""
+
+    message = MIMEText(html_code, "html")
+    await send_mail(email_sender, password, subject, message, email_receiver)
```

### Comparing `AsyncPywhatKit-2.2.6/AsyncPywhatKit/src/remotekit.py` & `AsyncPywhatKit-2.2.7/AsyncPywhatKit/src/remotekit.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,493 +1,513 @@
-00000000: 696d 706f 7274 206c 6f67 6769 6e67 0a69  import logging.i
-00000010: 6d70 6f72 7420 7379 730a 696d 706f 7274  mport sys.import
-00000020: 2074 6872 6561 6469 6e67 0a0a 696d 706f   threading..impo
-00000030: 7274 2070 7961 7574 6f67 7569 2061 7320  rt pyautogui as 
-00000040: 700a 6672 6f6d 2066 6c61 736b 2069 6d70  p.from flask imp
-00000050: 6f72 7420 466c 6173 6b2c 2072 6571 7565  ort Flask, reque
-00000060: 7374 0a0a 6c6f 6720 3d20 6c6f 6767 696e  st..log = loggin
-00000070: 672e 6765 744c 6f67 6765 7228 2277 6572  g.getLogger("wer
-00000080: 6b7a 6575 6722 290a 6c6f 672e 7365 744c  kzeug").log.setL
-00000090: 6576 656c 286c 6f67 6769 6e67 2e45 5252  evel(logging.ERR
-000000a0: 4f52 290a 0a63 6c69 203d 2073 7973 2e6d  OR)..cli = sys.m
-000000b0: 6f64 756c 6573 5b22 666c 6173 6b2e 636c  odules["flask.cl
-000000c0: 6922 5d0a 636c 692e 7368 6f77 5f73 6572  i"].cli.show_ser
-000000d0: 7665 725f 6261 6e6e 6572 203d 206c 616d  ver_banner = lam
-000000e0: 6264 6120 2a78 3a20 4e6f 6e65 0a0a 6170  bda *x: None..ap
-000000f0: 7020 3d20 466c 6173 6b28 2261 7070 2229  p = Flask("app")
-00000100: 0a0a 702e 4641 494c 5341 4645 203d 2046  ..p.FAILSAFE = F
-00000110: 616c 7365 0a6d 6f76 696e 6720 3d20 4661  alse.moving = Fa
-00000120: 6c73 650a 6472 6167 203d 2046 616c 7365  lse.drag = False
-00000130: 0a74 7970 655f 6461 7461 203d 2022 220a  .type_data = "".
-00000140: 6f6c 645f 6461 7461 203d 2022 220a 636f  old_data = "".co
-00000150: 6f72 6473 203d 2028 302c 2030 290a 6c61  ords = (0, 0).la
-00000160: 7374 636f 7264 7320 3d20 2830 2c20 3029  stcords = (0, 0)
-00000170: 0a6c 7374 6d63 6f72 6420 3d20 2830 2c20  .lstmcord = (0, 
-00000180: 3029 0a6c 7374 6c65 6e20 3d20 300a 636f  0).lstlen = 0.co
-00000190: 6f72 6473 203d 205b 2830 2c20 3029 5d0a  ords = [(0, 0)].
-000001a0: 0a0a 4061 7070 2e72 6f75 7465 2822 2f22  ..@app.route("/"
-000001b0: 2c20 6d65 7468 6f64 733d 5b22 4745 5422  , methods=["GET"
-000001c0: 2c20 2250 4f53 5422 5d29 0a64 6566 2073  , "POST"]).def s
-000001d0: 656e 6428 2920 2d3e 2073 7472 3a0a 2020  end() -> str:.  
-000001e0: 2020 2320 7072 696e 7428 2268 6572 6522    # print("here"
-000001f0: 290a 2020 2020 6966 2072 6571 7565 7374  ).    if request
-00000200: 2e6d 6574 686f 6420 3d3d 2022 504f 5354  .method == "POST
-00000210: 223a 0a20 2020 2020 2020 2023 2070 7269  ":.        # pri
-00000220: 6e74 2872 6571 7565 7374 2e67 6574 5f6a  nt(request.get_j
-00000230: 736f 6e28 2929 0a20 2020 2020 2020 2072  son()).        r
-00000240: 6574 7572 6e20 226f 6b22 0a20 2020 2072  eturn "ok".    r
-00000250: 6574 7572 6e20 2222 223c 2144 4f43 5459  eturn """<!DOCTY
-00000260: 5045 2068 746d 6c3e 0a3c 6874 6d6c 3e0a  PE html>.<html>.
-00000270: 2020 3c68 6561 643e 0a20 2020 203c 6d65    <head>.    <me
-00000280: 7461 2068 7474 702d 6571 7569 763d 2263  ta http-equiv="c
-00000290: 6f6e 7465 6e74 2d74 7970 6522 2063 6f6e  ontent-type" con
-000002a0: 7465 6e74 3d22 7465 7874 2f68 746d 6c3b  tent="text/html;
-000002b0: 2063 6861 7273 6574 3d75 7466 2d38 222f   charset=utf-8"/
-000002c0: 3e0a 2020 2020 3c6d 6574 6120 6e61 6d65  >.    <meta name
-000002d0: 3d27 7669 6577 706f 7274 270a 2020 2020  ='viewport'.    
-000002e0: 2063 6f6e 7465 6e74 3d27 7769 6474 683d   content='width=
-000002f0: 6465 7669 6365 2d77 6964 7468 2c20 696e  device-width, in
-00000300: 6974 6961 6c2d 7363 616c 653d 312e 302c  itial-scale=1.0,
-00000310: 206d 6178 696d 756d 2d73 6361 6c65 3d31   maximum-scale=1
-00000320: 2e30 2c0a 2020 2020 2075 7365 722d 7363  .0,.     user-sc
-00000330: 616c 6162 6c65 3d30 2720 3e0a 2020 2020  alable=0' >.    
-00000340: 3c73 6372 6970 7420 7479 7065 3d22 7465  <script type="te
-00000350: 7874 2f6a 6176 6173 6372 6970 7422 2063  xt/javascript" c
-00000360: 6861 7273 6574 3d22 7574 662d 3822 3e0a  harset="utf-8">.
-00000370: 2020 2020 6675 6e63 7469 6f6e 2069 6e69      function ini
-00000380: 7428 2920 7b0a 2020 2020 2020 2020 7661  t() {.        va
-00000390: 7220 746f 7563 687a 6f6e 6520 3d20 646f  r touchzone = do
-000003a0: 6375 6d65 6e74 2e67 6574 456c 656d 656e  cument.getElemen
-000003b0: 7442 7949 6428 227a 6f6e 6522 293b 0a20  tById("zone");. 
-000003c0: 2020 2020 2020 2074 6f75 6368 7a6f 6e65         touchzone
-000003d0: 2e61 6464 4576 656e 744c 6973 7465 6e65  .addEventListene
-000003e0: 7228 2274 6f75 6368 656e 6422 2c20 636c  r("touchend", cl
-000003f0: 6963 6b65 2c20 6661 6c73 6529 3b0a 2020  icke, false);.  
-00000400: 2020 2020 2020 746f 7563 687a 6f6e 652e        touchzone.
-00000410: 6164 6445 7665 6e74 4c69 7374 656e 6572  addEventListener
-00000420: 2822 746f 7563 686d 6f76 6522 2c20 6861  ("touchmove", ha
-00000430: 6e64 6c65 2c20 6661 6c73 6529 3b0a 2020  ndle, false);.  
-00000440: 2020 2020 2020 746f 7563 687a 6f6e 652e        touchzone.
-00000450: 6164 6445 7665 6e74 4c69 7374 656e 6572  addEventListener
-00000460: 2822 746f 7563 6873 7461 7274 222c 2074  ("touchstart", t
-00000470: 6f73 7461 7274 2c20 6661 6c73 6529 3b0a  ostart, false);.
-00000480: 2020 2020 2020 2020 7661 7220 7363 726f          var scro
-00000490: 6c6c 7a6f 6e65 203d 2064 6f63 756d 656e  llzone = documen
-000004a0: 742e 6765 7445 6c65 6d65 6e74 4279 4964  t.getElementById
-000004b0: 2822 7363 726f 6c6c 2229 3b0a 2020 2020  ("scroll");.    
-000004c0: 2020 2020 7363 726f 6c6c 7a6f 6e65 2e61      scrollzone.a
-000004d0: 6464 4576 656e 744c 6973 7465 6e65 7228  ddEventListener(
-000004e0: 2274 6f75 6368 6d6f 7665 222c 2073 6372  "touchmove", scr
-000004f0: 6f6c 6c6d 6f76 652c 2066 616c 7365 293b  ollmove, false);
-00000500: 0a20 2020 2020 2020 2073 6372 6f6c 6c7a  .        scrollz
-00000510: 6f6e 652e 6164 6445 7665 6e74 4c69 7374  one.addEventList
-00000520: 656e 6572 2822 746f 7563 6873 7461 7274  ener("touchstart
-00000530: 222c 2074 6f73 7461 7274 2c20 6661 6c73  ", tostart, fals
-00000540: 6529 3b0a 2020 2020 7d0a 0a66 756e 6374  e);.    }..funct
-00000550: 696f 6e20 7363 726f 6c6c 6d6f 7665 2865  ion scrollmove(e
-00000560: 7665 6e74 297b 0a20 2076 6172 2061 2020  vent){.  var a  
-00000570: 2020 3d20 6576 656e 742e 746f 7563 6865    = event.touche
-00000580: 735b 305d 2e70 6167 6558 3b0a 2020 7661  s[0].pageX;.  va
-00000590: 7220 6220 2020 2020 3d20 6576 656e 742e  r b     = event.
-000005a0: 746f 7563 6865 735b 305d 2e70 6167 6559  touches[0].pageY
-000005b0: 3b0a 2020 7661 7220 7868 7474 7020 3d20  ;.  var xhttp = 
-000005c0: 6e65 7720 584d 4c48 7474 7052 6571 7565  new XMLHttpReque
-000005d0: 7374 2829 3b0a 2020 7868 7474 702e 6f6e  st();.  xhttp.on
-000005e0: 7265 6164 7973 7461 7465 6368 616e 6765  readystatechange
-000005f0: 203d 2066 756e 6374 696f 6e28 2920 7b0a   = function() {.
-00000600: 2020 7d3b 0a20 2078 6874 7470 2e6f 7065    };.  xhttp.ope
-00000610: 6e28 2250 4f53 5422 2c20 2273 6372 6f6c  n("POST", "scrol
-00000620: 6c65 7222 2c20 7472 7565 293b 0a20 2078  ler", true);.  x
-00000630: 6874 7470 2e73 6574 5265 7175 6573 7448  http.setRequestH
-00000640: 6561 6465 7228 2243 6f6e 7465 6e74 2d74  eader("Content-t
-00000650: 7970 6522 2c20 2261 7070 6c69 6361 7469  ype", "applicati
-00000660: 6f6e 2f78 2d77 7777 2d66 6f72 6d2d 7572  on/x-www-form-ur
-00000670: 6c65 6e63 6f64 6564 2229 3b0a 2020 7868  lencoded");.  xh
-00000680: 7474 702e 7365 6e64 2822 613d 222b 612b  ttp.send("a="+a+
-00000690: 2226 623d 222b 6229 3b0a 7d0a 0a0a 6675  "&b="+b);.}...fu
-000006a0: 6e63 7469 6f6e 2074 6f73 7461 7274 2865  nction tostart(e
-000006b0: 7665 6e74 297b 0a20 2076 6172 2061 2020  vent){.  var a  
-000006c0: 2020 3d20 6576 656e 742e 746f 7563 6865    = event.touche
-000006d0: 735b 305d 2e70 6167 6558 3b0a 2020 7661  s[0].pageX;.  va
-000006e0: 7220 6220 2020 2020 3d20 6576 656e 742e  r b     = event.
-000006f0: 746f 7563 6865 735b 305d 2e70 6167 6559  touches[0].pageY
-00000700: 3b0a 2020 7661 7220 7868 7474 7020 3d20  ;.  var xhttp = 
-00000710: 6e65 7720 584d 4c48 7474 7052 6571 7565  new XMLHttpReque
-00000720: 7374 2829 3b0a 2020 7868 7474 702e 6f6e  st();.  xhttp.on
-00000730: 7265 6164 7973 7461 7465 6368 616e 6765  readystatechange
-00000740: 203d 2066 756e 6374 696f 6e28 2920 7b0a   = function() {.
-00000750: 2020 7d3b 0a20 2078 6874 7470 2e6f 7065    };.  xhttp.ope
-00000760: 6e28 2250 4f53 5422 2c20 2274 7374 6172  n("POST", "tstar
-00000770: 7422 2c20 7472 7565 293b 0a20 2078 6874  t", true);.  xht
-00000780: 7470 2e73 6574 5265 7175 6573 7448 6561  tp.setRequestHea
-00000790: 6465 7228 2243 6f6e 7465 6e74 2d74 7970  der("Content-typ
-000007a0: 6522 2c20 2261 7070 6c69 6361 7469 6f6e  e", "application
-000007b0: 2f78 2d77 7777 2d66 6f72 6d2d 7572 6c65  /x-www-form-urle
-000007c0: 6e63 6f64 6564 2229 3b0a 2020 7868 7474  ncoded");.  xhtt
-000007d0: 702e 7365 6e64 2822 613d 222b 612b 2226  p.send("a="+a+"&
-000007e0: 623d 222b 6229 3b0a 7d0a 0a66 756e 6374  b="+b);.}..funct
-000007f0: 696f 6e20 636c 6963 6b65 2865 7665 6e74  ion clicke(event
-00000800: 2920 7b0a 2020 7661 7220 7868 7474 7020  ) {.  var xhttp 
-00000810: 3d20 6e65 7720 584d 4c48 7474 7052 6571  = new XMLHttpReq
-00000820: 7565 7374 2829 3b0a 2020 7868 7474 702e  uest();.  xhttp.
-00000830: 6f6e 7265 6164 7973 7461 7465 6368 616e  onreadystatechan
-00000840: 6765 203d 2066 756e 6374 696f 6e28 2920  ge = function() 
-00000850: 7b0a 2020 7d3b 0a20 2076 6172 2061 203d  {.  };.  var a =
-00000860: 2065 7665 6e74 2e63 6861 6e67 6564 546f   event.changedTo
-00000870: 7563 6865 735b 305d 2e70 6167 6559 3b0a  uches[0].pageY;.
-00000880: 2020 7868 7474 702e 6f70 656e 2822 504f    xhttp.open("PO
-00000890: 5354 222c 2022 636c 6963 6b22 2c20 7472  ST", "click", tr
-000008a0: 7565 293b 0a20 2078 6874 7470 2e73 6574  ue);.  xhttp.set
-000008b0: 5265 7175 6573 7448 6561 6465 7228 2243  RequestHeader("C
-000008c0: 6f6e 7465 6e74 2d74 7970 6522 2c20 2261  ontent-type", "a
-000008d0: 7070 6c69 6361 7469 6f6e 2f78 2d77 7777  pplication/x-www
-000008e0: 2d66 6f72 6d2d 7572 6c65 6e63 6f64 6564  -form-urlencoded
-000008f0: 2229 3b0a 2020 7868 7474 702e 7365 6e64  ");.  xhttp.send
-00000900: 2822 613d 222b 6129 3b0a 7d0a 0a66 756e  ("a="+a);.}..fun
-00000910: 6374 696f 6e20 6472 6167 6d28 2920 7b0a  ction dragm() {.
-00000920: 2020 2020 7661 7220 6274 6e20 3d20 646f      var btn = do
-00000930: 6375 6d65 6e74 2e67 6574 456c 656d 656e  cument.getElemen
-00000940: 7442 7949 6428 2264 7261 6722 293b 0a20  tById("drag");. 
-00000950: 2020 2076 6172 2078 6874 7470 203d 206e     var xhttp = n
-00000960: 6577 2058 4d4c 4874 7470 5265 7175 6573  ew XMLHttpReques
-00000970: 7428 293b 0a20 2020 2078 6874 7470 2e6f  t();.    xhttp.o
-00000980: 6e72 6561 6479 7374 6174 6563 6861 6e67  nreadystatechang
-00000990: 6520 3d20 6675 6e63 7469 6f6e 2829 207b  e = function() {
-000009a0: 0a20 2020 207d 3b0a 2020 2020 7868 7474  .    };.    xhtt
-000009b0: 702e 6f70 656e 2822 504f 5354 222c 2022  p.open("POST", "
-000009c0: 6472 6164 6861 6e64 6c65 7222 2c20 7472  dradhandler", tr
-000009d0: 7565 293b 0a20 2020 2078 6874 7470 2e73  ue);.    xhttp.s
-000009e0: 6574 5265 7175 6573 7448 6561 6465 7228  etRequestHeader(
-000009f0: 2243 6f6e 7465 6e74 2d74 7970 6522 2c20  "Content-type", 
-00000a00: 2261 7070 6c69 6361 7469 6f6e 2f78 2d77  "application/x-w
-00000a10: 7777 2d66 6f72 6d2d 7572 6c65 6e63 6f64  ww-form-urlencod
-00000a20: 6564 2229 3b0a 2020 2020 7868 7474 702e  ed");.    xhttp.
-00000a30: 7365 6e64 2829 3b0a 0a20 2020 2069 6620  send();..    if 
-00000a40: 2862 746e 2e69 6e6e 6572 4854 4d4c 203d  (btn.innerHTML =
-00000a50: 3d20 2244 7261 6720 6d6f 7573 6522 297b  = "Drag mouse"){
-00000a60: 0a20 2020 2020 2020 2062 746e 2e69 6e6e  .        btn.inn
-00000a70: 6572 4854 4d4c 203d 2022 4d6f 7665 206d  erHTML = "Move m
-00000a80: 6f75 7365 223b 0a20 2020 207d 0a20 2020  ouse";.    }.   
-00000a90: 2065 6c73 657b 0a20 2020 2020 2020 2062   else{.        b
-00000aa0: 746e 2e69 6e6e 6572 4854 4d4c 203d 2022  tn.innerHTML = "
-00000ab0: 4472 6167 206d 6f75 7365 223b 0a20 2020  Drag mouse";.   
-00000ac0: 207d 0a7d 0a0a 6675 6e63 7469 6f6e 2073   }.}..function s
-00000ad0: 656e 6444 6174 6128 612c 622c 6729 207b  endData(a,b,g) {
-00000ae0: 0a20 2076 6172 2078 6874 7470 203d 206e  .  var xhttp = n
-00000af0: 6577 2058 4d4c 4874 7470 5265 7175 6573  ew XMLHttpReques
-00000b00: 7428 293b 0a20 2078 6874 7470 2e6f 6e72  t();.  xhttp.onr
-00000b10: 6561 6479 7374 6174 6563 6861 6e67 6520  eadystatechange 
-00000b20: 3d20 6675 6e63 7469 6f6e 2829 207b 0a20  = function() {. 
-00000b30: 207d 3b0a 2020 7868 7474 702e 6f70 656e   };.  xhttp.open
-00000b40: 2822 504f 5354 222c 2022 6861 6e64 6c65  ("POST", "handle
-00000b50: 7222 2c20 7472 7565 293b 0a20 2078 6874  r", true);.  xht
-00000b60: 7470 2e73 6574 5265 7175 6573 7448 6561  tp.setRequestHea
-00000b70: 6465 7228 2243 6f6e 7465 6e74 2d74 7970  der("Content-typ
-00000b80: 6522 2c20 2261 7070 6c69 6361 7469 6f6e  e", "application
-00000b90: 2f78 2d77 7777 2d66 6f72 6d2d 7572 6c65  /x-www-form-urle
-00000ba0: 6e63 6f64 6564 2229 3b0a 2020 7868 7474  ncoded");.  xhtt
-00000bb0: 702e 7365 6e64 2822 613d 222b 612b 2226  p.send("a="+a+"&
-00000bc0: 623d 222b 6229 3b0a 7d0a 0a0a 2066 756e  b="+b);.}... fun
-00000bd0: 6374 696f 6e20 6861 6e64 6c65 2865 7665  ction handle(eve
-00000be0: 6e74 2920 7b0a 2020 7661 7220 616c 7068  nt) {.  var alph
-00000bf0: 6120 2020 203d 2065 7665 6e74 2e74 6f75  a    = event.tou
-00000c00: 6368 6573 5b30 5d2e 7061 6765 583b 0a20  ches[0].pageX;. 
-00000c10: 2076 6172 2062 6574 6120 2020 2020 3d20   var beta     = 
-00000c20: 6576 656e 742e 746f 7563 6865 735b 305d  event.touches[0]
-00000c30: 2e70 6167 6559 3b0a 2020 7365 6e64 4461  .pageY;.  sendDa
-00000c40: 7461 2861 6c70 6861 2c62 6574 6129 3b0a  ta(alpha,beta);.
-00000c50: 7d0a 0a0a 6675 6e63 7469 6f6e 206f 6e5f  }...function on_
-00000c60: 696e 7075 7428 297b 0a20 2076 6172 2064  input(){.  var d
-00000c70: 6174 6120 3d20 646f 6375 6d65 6e74 2e67  ata = document.g
-00000c80: 6574 456c 656d 656e 7442 7949 6428 2269  etElementById("i
-00000c90: 6e70 6669 656c 6422 292e 7661 6c75 653b  npfield").value;
-00000ca0: 0a20 2076 6172 2078 6874 7470 203d 206e  .  var xhttp = n
-00000cb0: 6577 2058 4d4c 4874 7470 5265 7175 6573  ew XMLHttpReques
-00000cc0: 7428 293b 0a20 2078 6874 7470 2e6f 6e72  t();.  xhttp.onr
-00000cd0: 6561 6479 7374 6174 6563 6861 6e67 6520  eadystatechange 
-00000ce0: 3d20 6675 6e63 7469 6f6e 2829 207b 0a20  = function() {. 
-00000cf0: 207d 3b0a 2020 7868 7474 702e 6f70 656e   };.  xhttp.open
-00000d00: 2822 504f 5354 222c 2022 7479 7065 6422  ("POST", "typed"
-00000d10: 2c20 7472 7565 293b 0a20 2078 6874 7470  , true);.  xhttp
-00000d20: 2e73 6574 5265 7175 6573 7448 6561 6465  .setRequestHeade
-00000d30: 7228 2243 6f6e 7465 6e74 2d74 7970 6522  r("Content-type"
-00000d40: 2c20 2261 7070 6c69 6361 7469 6f6e 2f78  , "application/x
-00000d50: 2d77 7777 2d66 6f72 6d2d 7572 6c65 6e63  -www-form-urlenc
-00000d60: 6f64 6564 2229 3b0a 2020 7868 7474 702e  oded");.  xhttp.
-00000d70: 7365 6e64 2822 6461 7461 3d22 2b64 6174  send("data="+dat
-00000d80: 6129 3b0a 7d0a 6675 6e63 7469 6f6e 2065  a);.}.function e
-00000d90: 6e74 6572 5f62 7574 2829 7b0a 2020 7661  nter_but(){.  va
-00000da0: 7220 7868 7474 7020 3d20 6e65 7720 584d  r xhttp = new XM
-00000db0: 4c48 7474 7052 6571 7565 7374 2829 3b0a  LHttpRequest();.
-00000dc0: 2020 7868 7474 702e 6f6e 7265 6164 7973    xhttp.onreadys
-00000dd0: 7461 7465 6368 616e 6765 203d 2066 756e  tatechange = fun
-00000de0: 6374 696f 6e28 2920 7b0a 2020 7d3b 0a20  ction() {.  };. 
-00000df0: 2078 6874 7470 2e6f 7065 6e28 2250 4f53   xhttp.open("POS
-00000e00: 5422 2c20 2265 6e74 6572 222c 2074 7275  T", "enter", tru
-00000e10: 6529 3b0a 2020 7868 7474 702e 7365 7452  e);.  xhttp.setR
-00000e20: 6571 7565 7374 4865 6164 6572 2822 436f  equestHeader("Co
-00000e30: 6e74 656e 742d 7479 7065 222c 2022 6170  ntent-type", "ap
-00000e40: 706c 6963 6174 696f 6e2f 782d 7777 772d  plication/x-www-
-00000e50: 666f 726d 2d75 726c 656e 636f 6465 6422  form-urlencoded"
-00000e60: 293b 0a20 2078 6874 7470 2e73 656e 6428  );.  xhttp.send(
-00000e70: 2264 6174 613d 222b 2264 6174 6122 293b  "data="+"data");
-00000e80: 0a7d 0a0a 0a0a 0a20 2020 203c 2f73 6372  .}.....    </scr
-00000e90: 6970 743e 0a0a 2020 2020 3c6d 6574 6120  ipt>..    <meta 
-00000ea0: 6e61 6d65 3d22 2220 636f 6e74 656e 743d  name="" content=
-00000eb0: 2222 3e0a 2020 2020 3c74 6974 6c65 3e3c  "">.    <title><
-00000ec0: 2f74 6974 6c65 3e0a 2020 3c73 7479 6c65  /title>.  <style
-00000ed0: 3e0a 2020 2e63 656e 7465 727b 0a20 2020  >.  .center{.   
-00000ee0: 2070 6f73 6974 696f 6e3a 2066 6978 6564   position: fixed
-00000ef0: 3b0a 2020 2020 6261 636b 6772 6f75 6e64  ;.    background
-00000f00: 2d63 6f6c 6f72 3a20 7267 6228 3233 302c  -color: rgb(230,
-00000f10: 3233 302c 3233 3029 3b0a 2020 2020 7769  230,230);.    wi
-00000f20: 6474 683a 3830 253b 0a20 2020 2068 6569  dth:80%;.    hei
-00000f30: 6768 743a 3430 3070 783b 0a20 2020 2074  ght:400px;.    t
-00000f40: 6f70 3a33 3030 7078 3b0a 2020 2020 6c65  op:300px;.    le
-00000f50: 6674 3a34 3625 3b0a 2020 2020 636f 6c6f  ft:46%;.    colo
-00000f60: 723a 7267 6228 3230 302c 3230 302c 3230  r:rgb(200,200,20
-00000f70: 3029 3b0a 2020 2020 666f 6e74 2d77 6569  0);.    font-wei
-00000f80: 6768 743a 626f 6c64 3b0a 2020 2020 7472  ght:bold;.    tr
-00000f90: 616e 7366 6f72 6d3a 2074 7261 6e73 6c61  ansform: transla
-00000fa0: 7465 282d 3530 252c 2d35 3025 293b 0a20  te(-50%,-50%);. 
-00000fb0: 2020 202d 7765 626b 6974 2d74 6f75 6368     -webkit-touch
-00000fc0: 2d63 616c 6c6f 7574 3a20 6e6f 6e65 3b0a  -callout: none;.
-00000fd0: 2020 2020 2d77 6562 6b69 742d 7573 6572      -webkit-user
-00000fe0: 2d73 656c 6563 743a 206e 6f6e 653b 0a20  -select: none;. 
-00000ff0: 2020 202d 6b68 746d 6c2d 7573 6572 2d73     -khtml-user-s
-00001000: 656c 6563 743a 206e 6f6e 653b 0a20 2020  elect: none;.   
-00001010: 202d 6d6f 7a2d 7573 6572 2d73 656c 6563   -moz-user-selec
-00001020: 743a 206e 6f6e 653b 0a20 2020 202d 6d73  t: none;.    -ms
-00001030: 2d75 7365 722d 7365 6c65 6374 3a20 6e6f  -user-select: no
-00001040: 6e65 3b0a 2020 2020 7573 6572 2d73 656c  ne;.    user-sel
-00001050: 6563 743a 206e 6f6e 653b 0a20 2020 7d0a  ect: none;.   }.
-00001060: 2020 2068 746d 6c7b 0a20 2020 746f 7563     html{.   touc
-00001070: 682d 6163 7469 6f6e 3a70 616e 2d64 6f77  h-action:pan-dow
-00001080: 6e0a 2020 207d 0a0a 2020 202e 7363 726f  n.   }..   .scro
-00001090: 6c6c 6172 6561 7b0a 2020 2020 706f 7369  llarea{.    posi
-000010a0: 7469 6f6e 3a20 6669 7865 643b 0a20 2020  tion: fixed;.   
-000010b0: 2062 6163 6b67 726f 756e 642d 636f 6c6f   background-colo
-000010c0: 723a 2072 6762 2832 3330 2c32 3330 2c32  r: rgb(230,230,2
-000010d0: 3330 293b 0a20 2020 2077 6964 7468 3a33  30);.    width:3
-000010e0: 3070 783b 0a20 2020 2068 6569 6768 743a  0px;.    height:
-000010f0: 3430 3070 783b 0a20 2020 2074 6f70 3a33  400px;.    top:3
-00001100: 3030 7078 3b0a 2020 2020 6c65 6674 3a39  00px;.    left:9
-00001110: 322e 3035 253b 0a20 2020 2063 6f6c 6f72  2.05%;.    color
-00001120: 3a72 6762 2832 3030 2c32 3030 2c32 3030  :rgb(200,200,200
-00001130: 293b 0a20 2020 2066 6f6e 742d 7765 6967  );.    font-weig
-00001140: 6874 3a62 6f6c 643b 0a20 2020 2074 7261  ht:bold;.    tra
-00001150: 6e73 666f 726d 3a20 7472 616e 736c 6174  nsform: translat
-00001160: 6528 2d35 3025 2c2d 3530 2529 3b0a 2020  e(-50%,-50%);.  
-00001170: 2020 2d77 6562 6b69 742d 746f 7563 682d    -webkit-touch-
-00001180: 6361 6c6c 6f75 743a 206e 6f6e 653b 0a20  callout: none;. 
-00001190: 2020 202d 7765 626b 6974 2d75 7365 722d     -webkit-user-
-000011a0: 7365 6c65 6374 3a20 6e6f 6e65 3b0a 2020  select: none;.  
-000011b0: 2020 2d6b 6874 6d6c 2d75 7365 722d 7365    -khtml-user-se
-000011c0: 6c65 6374 3a20 6e6f 6e65 3b0a 2020 2020  lect: none;.    
-000011d0: 2d6d 6f7a 2d75 7365 722d 7365 6c65 6374  -moz-user-select
-000011e0: 3a20 6e6f 6e65 3b0a 2020 2020 2d6d 732d  : none;.    -ms-
-000011f0: 7573 6572 2d73 656c 6563 743a 206e 6f6e  user-select: non
-00001200: 653b 0a20 2020 2075 7365 722d 7365 6c65  e;.    user-sele
-00001210: 6374 3a20 6e6f 6e65 3b0a 2020 2020 7465  ct: none;.    te
-00001220: 7874 2d61 6c69 676e 3a63 656e 7465 723b  xt-align:center;
-00001230: 0a20 2020 7d0a 0a0a 2020 3c2f 7374 796c  .   }...  </styl
-00001240: 653e 0a20 203c 2f68 6561 643e 0a20 203c  e>.  </head>.  <
-00001250: 626f 6479 206f 6e6c 6f61 643d 2269 6e69  body onload="ini
-00001260: 7428 2922 3e0a 2020 3c70 2073 7479 6c65  t()">.  <p style
-00001270: 3d22 7465 7874 2d61 6c69 676e 3a63 656e  ="text-align:cen
-00001280: 7465 723b 223e 5479 7065 206f 6e20 5043  ter;">Type on PC
-00001290: 0a20 203c 696e 7075 7420 6964 3d22 696e  .  <input id="in
-000012a0: 7066 6965 6c64 2274 7970 653d 2274 6578  pfield"type="tex
-000012b0: 7422 206f 6e69 6e70 7574 3d6f 6e5f 696e  t" oninput=on_in
-000012c0: 7075 7428 293e 3c2f 696e 7075 743e 0a20  put()></input>. 
-000012d0: 203c 6275 7474 6f6e 2074 7970 653d 2262   <button type="b
-000012e0: 7574 746f 6e22 206f 6e63 6c69 636b 3d22  utton" onclick="
-000012f0: 656e 7465 725f 6275 7428 2922 3e45 6e74  enter_but()">Ent
-00001300: 6572 3c2f 6275 7474 6f6e 3e3c 2f70 3e0a  er</button></p>.
-00001310: 2020 3c64 6976 2073 7479 6c65 3d22 7465    <div style="te
-00001320: 7874 2d61 6c69 676e 3a63 656e 7465 723b  xt-align:center;
-00001330: 223e 0a20 2020 2020 203c 6275 7474 6f6e  ">.      <button
-00001340: 2069 643d 2264 7261 6722 2074 7970 653d   id="drag" type=
-00001350: 2262 7574 746f 6e22 206f 6e63 6c69 636b  "button" onclick
-00001360: 3d22 6472 6167 6d28 2922 3e44 7261 6720  ="dragm()">Drag 
-00001370: 6d6f 7573 653c 2f62 7574 746f 6e3e 0a20  mouse</button>. 
-00001380: 203c 2f64 6976 3e0a 2020 2020 3c64 6976   </div>.    <div
-00001390: 2063 6c61 7373 3d22 6365 6e74 6572 2220   class="center" 
-000013a0: 6964 3d22 7a6f 6e65 223e 0a20 2020 2020  id="zone">.     
-000013b0: 2020 203c 7020 616c 6967 6e3d 2263 656e     <p align="cen
-000013c0: 7465 7222 3e3c 6272 3e3c 6272 3e3c 6272  ter"><br><br><br
-000013d0: 3e3c 6272 3e3c 6272 3e3c 6272 3e4c 6566  ><br><br><br>Lef
-000013e0: 7420 636c 6963 6b20 6172 6561 3c62 723e  t click area<br>
-000013f0: 3c62 723e 3c62 723e 3c62 723e 3c62 723e  <br><br><br><br>
-00001400: 3c62 723e 3c68 723e 3c2f 703e 0a20 2020  <br><hr></p>.   
-00001410: 2020 2020 203c 7020 616c 6967 6e3d 2263       <p align="c
-00001420: 656e 7465 7222 3e3c 6272 3e52 6967 6874  enter"><br>Right
-00001430: 2063 6c69 636b 2061 7265 613c 2f70 3e0a   click area</p>.
-00001440: 2020 2020 3c2f 6469 763e 0a20 2020 203c      </div>.    <
-00001450: 6469 7620 636c 6173 733d 2273 6372 6f6c  div class="scrol
-00001460: 6c61 7265 6122 2069 643d 2273 6372 6f6c  larea" id="scrol
-00001470: 6c22 3e0a 2020 2020 2020 203c 703e 3c62  l">.       <p><b
-00001480: 723e 3c62 723e 3c62 723e 3c62 723e 3c62  r><br><br><br><b
-00001490: 723e 533c 6272 3e43 3c62 723e 523c 6272  r>S<br>C<br>R<br
-000014a0: 3e4f 3c62 723e 4c3c 6272 3e4c 3c2f 703e  >O<br>L<br>L</p>
-000014b0: 0a20 2020 203c 2f64 6976 3e0a 2020 3c2f  .    </div>.  </
-000014c0: 626f 6479 3e0a 3c2f 6874 6d6c 3e22 2222  body>.</html>"""
-000014d0: 0a0a 0a40 6170 702e 726f 7574 6528 222f  ...@app.route("/
-000014e0: 6861 6e64 6c65 7222 2c20 6d65 7468 6f64  handler", method
-000014f0: 733d 5b22 504f 5354 225d 290a 6465 6620  s=["POST"]).def 
-00001500: 6861 6e64 6c65 2829 202d 3e20 7374 723a  handle() -> str:
-00001510: 0a20 2020 2067 6c6f 6261 6c20 6d6f 7669  .    global movi
-00001520: 6e67 2c20 636f 7264 6c73 742c 206c 6173  ng, cordlst, las
-00001530: 7463 6f72 6473 0a20 2020 206c 7374 203d  tcords.    lst =
-00001540: 205b 5d0a 2020 2020 6120 3d20 7265 7175   [].    a = requ
-00001550: 6573 742e 666f 726d 5b22 6122 5d0a 2020  est.form["a"].  
-00001560: 2020 6220 3d20 7265 7175 6573 742e 666f    b = request.fo
-00001570: 726d 5b22 6222 5d0a 2020 2020 6120 3d20  rm["b"].    a = 
-00001580: 666c 6f61 7428 6129 0a20 2020 2062 203d  float(a).    b =
-00001590: 2066 6c6f 6174 2862 290a 2020 2020 6d6f   float(b).    mo
-000015a0: 7669 6e67 203d 2054 7275 650a 2020 2020  ving = True.    
-000015b0: 636f 6f72 6473 203d 2028 612c 2062 290a  coords = (a, b).
-000015c0: 2020 2020 6c78 2c20 6c79 203d 206c 6173      lx, ly = las
-000015d0: 7463 6f72 6473 0a20 2020 2063 782c 2063  tcords.    cx, c
-000015e0: 7920 3d20 636f 6f72 6473 0a20 2020 2023  y = coords.    #
-000015f0: 2070 7269 6e74 2863 782c 6379 290a 2020   print(cx,cy).  
-00001600: 2020 2320 702e 6d6f 7665 5265 6c28 2863    # p.moveRel((c
-00001610: 782d 6c78 292f 322c 2863 792d 6c79 292f  x-lx)/2,(cy-ly)/
-00001620: 3229 0a20 2020 2074 6872 6561 6469 6e67  2).    threading
-00001630: 2e54 6872 6561 6428 7461 7267 6574 3d6c  .Thread(target=l
-00001640: 616d 6264 613a 2070 2e6d 6f76 6552 656c  ambda: p.moveRel
-00001650: 2828 6378 202d 206c 7829 202a 2032 2c20  ((cx - lx) * 2, 
-00001660: 2863 7920 2d20 6c79 2920 2a20 3229 292e  (cy - ly) * 2)).
-00001670: 7374 6172 7428 290a 2020 2020 6c61 7374  start().    last
-00001680: 636f 7264 7320 3d20 636f 6f72 6473 0a20  cords = coords. 
-00001690: 2020 2072 6574 7572 6e20 2231 220a 0a0a     return "1"...
-000016a0: 4061 7070 2e72 6f75 7465 2822 2f73 6372  @app.route("/scr
-000016b0: 6f6c 6c65 7222 2c20 6d65 7468 6f64 733d  oller", methods=
-000016c0: 5b22 504f 5354 225d 290a 6465 6620 7363  ["POST"]).def sc
-000016d0: 726f 6c6c 6572 7228 2920 2d3e 2073 7472  rollerr() -> str
-000016e0: 3a0a 2020 2020 676c 6f62 616c 206d 6f76  :.    global mov
-000016f0: 696e 672c 2063 6f72 646c 7374 2c20 6c61  ing, cordlst, la
-00001700: 7374 636f 7264 7332 0a20 2020 2061 203d  stcords2.    a =
-00001710: 2072 6571 7565 7374 2e66 6f72 6d5b 2261   request.form["a
-00001720: 225d 0a20 2020 2062 203d 2072 6571 7565  "].    b = reque
-00001730: 7374 2e66 6f72 6d5b 2262 225d 0a20 2020  st.form["b"].   
-00001740: 2061 203d 2066 6c6f 6174 2861 290a 2020   a = float(a).  
-00001750: 2020 6220 3d20 666c 6f61 7428 6229 0a20    b = float(b). 
-00001760: 2020 2063 6f6f 7264 7320 3d20 2861 2c20     coords = (a, 
-00001770: 6229 0a20 2020 206c 782c 206c 7920 3d20  b).    lx, ly = 
-00001780: 6c61 7374 636f 7264 7332 0a20 2020 2063  lastcords2.    c
-00001790: 782c 2063 7920 3d20 636f 6f72 6473 0a20  x, cy = coords. 
-000017a0: 2020 2069 6620 6379 203c 206c 793a 0a20     if cy < ly:. 
-000017b0: 2020 2020 2020 2074 6872 6561 6469 6e67         threading
-000017c0: 2e54 6872 6561 6428 7461 7267 6574 3d6c  .Thread(target=l
-000017d0: 616d 6264 613a 2070 2e73 6372 6f6c 6c28  ambda: p.scroll(
-000017e0: 3530 2929 2e73 7461 7274 2829 0a20 2020  50)).start().   
-000017f0: 2069 6620 6379 203e 206c 793a 0a20 2020   if cy > ly:.   
-00001800: 2020 2020 2074 6872 6561 6469 6e67 2e54       threading.T
-00001810: 6872 6561 6428 7461 7267 6574 3d6c 616d  hread(target=lam
-00001820: 6264 613a 2070 2e73 6372 6f6c 6c28 2d35  bda: p.scroll(-5
-00001830: 3029 292e 7374 6172 7428 290a 2020 2020  0)).start().    
-00001840: 6c61 7374 636f 7264 7332 203d 2063 6f6f  lastcords2 = coo
-00001850: 7264 730a 2020 2020 7265 7475 726e 2022  rds.    return "
-00001860: 3122 0a0a 0a40 6170 702e 726f 7574 6528  1"...@app.route(
-00001870: 222f 7473 7461 7274 222c 206d 6574 686f  "/tstart", metho
-00001880: 6473 3d5b 2250 4f53 5422 5d29 0a64 6566  ds=["POST"]).def
-00001890: 2073 7461 7274 7428 2920 2d3e 2073 7472   startt() -> str
-000018a0: 3a0a 2020 2020 676c 6f62 616c 206c 6173  :.    global las
-000018b0: 7463 6f72 6473 2c20 6c61 7374 636f 7264  tcords, lastcord
-000018c0: 7332 0a20 2020 2023 2070 7269 6e74 2822  s2.    # print("
-000018d0: 656e 6422 290a 2020 2020 6120 3d20 7265  end").    a = re
-000018e0: 7175 6573 742e 666f 726d 5b22 6122 5d0a  quest.form["a"].
-000018f0: 2020 2020 6220 3d20 7265 7175 6573 742e      b = request.
-00001900: 666f 726d 5b22 6222 5d0a 2020 2020 2320  form["b"].    # 
-00001910: 7072 696e 7428 612c 6229 0a20 2020 2061  print(a,b).    a
-00001920: 203d 2066 6c6f 6174 2861 290a 2020 2020   = float(a).    
-00001930: 6220 3d20 666c 6f61 7428 6229 0a20 2020  b = float(b).   
-00001940: 206c 6173 7463 6f72 6473 203d 2028 612c   lastcords = (a,
-00001950: 2062 290a 2020 2020 6c61 7374 636f 7264   b).    lastcord
-00001960: 7332 203d 2028 612c 2062 290a 2020 2020  s2 = (a, b).    
-00001970: 7265 7475 726e 2022 3122 0a0a 0a40 6170  return "1"...@ap
-00001980: 702e 726f 7574 6528 222f 636c 6963 6b22  p.route("/click"
-00001990: 2c20 6d65 7468 6f64 733d 5b22 504f 5354  , methods=["POST
-000019a0: 225d 290a 6465 6620 646f 5f63 6c69 636b  "]).def do_click
-000019b0: 2829 202d 3e20 7374 723a 0a20 2020 2067  () -> str:.    g
-000019c0: 6c6f 6261 6c20 6d6f 7669 6e67 0a20 2020  lobal moving.   
-000019d0: 2069 6620 6e6f 7420 6d6f 7669 6e67 3a0a   if not moving:.
-000019e0: 2020 2020 2020 2020 6120 3d20 7265 7175          a = requ
-000019f0: 6573 742e 666f 726d 5b22 6122 5d0a 2020  est.form["a"].  
-00001a00: 2020 2020 2020 2320 7072 696e 7428 6129        # print(a)
-00001a10: 0a20 2020 2020 2020 2061 203d 2066 6c6f  .        a = flo
-00001a20: 6174 2861 290a 2020 2020 2020 2020 6966  at(a).        if
-00001a30: 2061 203c 2034 3030 3a0a 2020 2020 2020   a < 400:.      
-00001a40: 2020 2020 2020 702e 636c 6963 6b28 290a        p.click().
-00001a50: 2020 2020 2020 2020 6966 2061 203e 3d20          if a >= 
-00001a60: 3430 303a 0a20 2020 2020 2020 2020 2020  400:.           
-00001a70: 2070 2e72 6967 6874 436c 6963 6b28 290a   p.rightClick().
-00001a80: 0a20 2020 206d 6f76 696e 6720 3d20 4661  .    moving = Fa
-00001a90: 6c73 650a 2020 2020 7265 7475 726e 2022  lse.    return "
-00001aa0: 3122 0a0a 0a40 6170 702e 726f 7574 6528  1"...@app.route(
-00001ab0: 222f 7479 7065 6422 2c20 6d65 7468 6f64  "/typed", method
-00001ac0: 733d 5b22 504f 5354 225d 290a 6465 6620  s=["POST"]).def 
-00001ad0: 7479 7065 6974 2829 202d 3e20 7374 723a  typeit() -> str:
-00001ae0: 0a20 2020 2067 6c6f 6261 6c20 7479 7065  .    global type
-00001af0: 5f64 6174 612c 206f 6c64 5f64 6174 610a  _data, old_data.
-00001b00: 2020 2020 6461 7461 203d 2072 6571 7565      data = reque
-00001b10: 7374 2e66 6f72 6d5b 2264 6174 6122 5d0a  st.form["data"].
-00001b20: 2020 2020 7479 7065 5f64 6174 6120 3d20      type_data = 
-00001b30: 7374 7228 6461 7461 290a 2020 2020 6966  str(data).    if
-00001b40: 206c 656e 2874 7970 655f 6461 7461 2920   len(type_data) 
-00001b50: 3e20 6c65 6e28 6f6c 645f 6461 7461 293a  > len(old_data):
-00001b60: 0a20 2020 2020 2020 2070 2e74 7970 6577  .        p.typew
-00001b70: 7269 7465 2874 7970 655f 6461 7461 5b6c  rite(type_data[l
-00001b80: 656e 2874 7970 655f 6461 7461 2920 2d20  en(type_data) - 
-00001b90: 315d 290a 2020 2020 656c 7365 3a0a 2020  1]).    else:.  
-00001ba0: 2020 2020 2020 702e 7072 6573 7328 2262        p.press("b
-00001bb0: 6163 6b73 7061 6365 222c 206c 656e 286f  ackspace", len(o
-00001bc0: 6c64 5f64 6174 6129 202d 206c 656e 2874  ld_data) - len(t
-00001bd0: 7970 655f 6461 7461 2929 0a20 2020 206f  ype_data)).    o
-00001be0: 6c64 5f64 6174 6120 3d20 7479 7065 5f64  ld_data = type_d
-00001bf0: 6174 610a 2020 2020 7265 7475 726e 2022  ata.    return "
-00001c00: 3122 0a0a 0a40 6170 702e 726f 7574 6528  1"...@app.route(
-00001c10: 222f 656e 7465 7222 2c20 6d65 7468 6f64  "/enter", method
-00001c20: 733d 5b22 504f 5354 225d 290a 6465 6620  s=["POST"]).def 
-00001c30: 736c 6173 684e 2829 202d 3e20 7374 723a  slashN() -> str:
-00001c40: 0a20 2020 2070 2e70 7265 7373 2822 656e  .    p.press("en
-00001c50: 7465 7222 290a 2020 2020 7265 7475 726e  ter").    return
-00001c60: 2022 3122 0a0a 0a40 6170 702e 726f 7574   "1"...@app.rout
-00001c70: 6528 222f 6472 6164 6861 6e64 6c65 7222  e("/dradhandler"
-00001c80: 2c20 6d65 7468 6f64 733d 5b22 504f 5354  , methods=["POST
-00001c90: 225d 290a 6465 6620 6768 6173 6974 5f6d  "]).def ghasit_m
-00001ca0: 6f75 7365 2829 202d 3e20 7374 723a 0a20  ouse() -> str:. 
-00001cb0: 2020 2067 6c6f 6261 6c20 6472 6167 0a20     global drag. 
-00001cc0: 2020 2023 2070 7269 6e74 2864 7261 6729     # print(drag)
-00001cd0: 0a20 2020 2069 6620 6472 6167 203d 3d20  .    if drag == 
-00001ce0: 5472 7565 3a0a 2020 2020 2020 2020 6472  True:.        dr
-00001cf0: 6167 203d 2046 616c 7365 0a20 2020 2020  ag = False.     
-00001d00: 2020 2070 2e6d 6f75 7365 5570 2829 0a0a     p.mouseUp()..
-00001d10: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00001d20: 2020 6472 6167 203d 2054 7275 650a 2020    drag = True.  
-00001d30: 2020 2020 2020 702e 6d6f 7573 6544 6f77        p.mouseDow
-00001d40: 6e28 290a 0a20 2020 2072 6574 7572 6e20  n()..    return 
-00001d50: 2231 220a 0a0a 6465 6620 7374 6172 745f  "1"...def start_
-00001d60: 7365 7276 6572 2870 6f72 743d 3830 3030  server(port=8000
-00001d70: 2c20 7072 696e 745f 6d73 673d 5472 7565  , print_msg=True
-00001d80: 293a 0a20 2020 2069 6620 7072 696e 745f  ):.    if print_
-00001d90: 6d73 673a 0a20 2020 2020 2020 2070 7269  msg:.        pri
-00001da0: 6e74 2822 5365 7276 6572 2073 7461 7274  nt("Server start
-00001db0: 6564 2061 7420 6c6f 6361 6c5f 6970 5f6f  ed at local_ip_o
-00001dc0: 665f 7468 6973 5f70 633a 2573 2220 2520  f_this_pc:%s" % 
-00001dd0: 706f 7274 290a 2020 2020 2020 2020 7072  port).        pr
-00001de0: 696e 7428 2250 7269 6e74 2043 7472 6c2b  int("Print Ctrl+
-00001df0: 4320 746f 2065 7869 7422 290a 2020 2020  C to exit").    
-00001e00: 6170 702e 7275 6e28 686f 7374 3d22 302e  app.run(host="0.
-00001e10: 302e 302e 3022 2c20 706f 7274 3d70 6f72  0.0.0", port=por
-00001e20: 7429 0a0a 0a23 2061 7070 2e72 756e 2868  t)...# app.run(h
-00001e30: 6f73 743d 2730 2e30 2e30 2e30 2729 0a23  ost='0.0.0.0').#
-00001e40: 0a23 0a23 2064 6566 206d 6169 6e28 293a  .#.# def main():
-00001e50: 0a23 2020 2020 2061 7070 2e72 756e 2868  .#     app.run(h
-00001e60: 6f73 743d 2231 3932 2e31 3638 2e34 332e  ost="192.168.43.
-00001e70: 3137 222c 2070 6f72 743d 3333 290a 230a  17", port=33).#.
-00001e80: 230a 2320 6966 205f 5f6e 616d 655f 5f20  #.# if __name__ 
-00001e90: 3d3d 2022 5f5f 6d61 696e 5f5f 223a 0a23  == "__main__":.#
-00001ea0: 2020 2020 206d 6169 6e28 290a 2320 2020       main().#   
-00001eb0: 2020 6170 702e 7275 6e28 686f 7374 3d27    app.run(host='
-00001ec0: 6c6f 6361 6c68 6f73 7427 290a            localhost').
+00000000: 696d 706f 7274 206c 6f67 6769 6e67 0d0a  import logging..
+00000010: 696d 706f 7274 2073 7973 0d0a 696d 706f  import sys..impo
+00000020: 7274 2074 6872 6561 6469 6e67 0d0a 0d0a  rt threading....
+00000030: 696d 706f 7274 2070 7961 7574 6f67 7569  import pyautogui
+00000040: 2061 7320 700d 0a66 726f 6d20 666c 6173   as p..from flas
+00000050: 6b20 696d 706f 7274 2046 6c61 736b 2c20  k import Flask, 
+00000060: 7265 7175 6573 740d 0a0d 0a6c 6f67 203d  request....log =
+00000070: 206c 6f67 6769 6e67 2e67 6574 4c6f 6767   logging.getLogg
+00000080: 6572 2822 7765 726b 7a65 7567 2229 0d0a  er("werkzeug")..
+00000090: 6c6f 672e 7365 744c 6576 656c 286c 6f67  log.setLevel(log
+000000a0: 6769 6e67 2e45 5252 4f52 290d 0a0d 0a63  ging.ERROR)....c
+000000b0: 6c69 203d 2073 7973 2e6d 6f64 756c 6573  li = sys.modules
+000000c0: 5b22 666c 6173 6b2e 636c 6922 5d0d 0a63  ["flask.cli"]..c
+000000d0: 6c69 2e73 686f 775f 7365 7276 6572 5f62  li.show_server_b
+000000e0: 616e 6e65 7220 3d20 6c61 6d62 6461 202a  anner = lambda *
+000000f0: 783a 204e 6f6e 650d 0a0d 0a61 7070 203d  x: None....app =
+00000100: 2046 6c61 736b 2822 6170 7022 290d 0a0d   Flask("app")...
+00000110: 0a70 2e46 4149 4c53 4146 4520 3d20 4661  .p.FAILSAFE = Fa
+00000120: 6c73 650d 0a6d 6f76 696e 6720 3d20 4661  lse..moving = Fa
+00000130: 6c73 650d 0a64 7261 6720 3d20 4661 6c73  lse..drag = Fals
+00000140: 650d 0a74 7970 655f 6461 7461 203d 2022  e..type_data = "
+00000150: 220d 0a6f 6c64 5f64 6174 6120 3d20 2222  "..old_data = ""
+00000160: 0d0a 636f 6f72 6473 203d 2028 302c 2030  ..coords = (0, 0
+00000170: 290d 0a6c 6173 7463 6f72 6473 203d 2028  )..lastcords = (
+00000180: 302c 2030 290d 0a6c 7374 6d63 6f72 6420  0, 0)..lstmcord 
+00000190: 3d20 2830 2c20 3029 0d0a 6c73 746c 656e  = (0, 0)..lstlen
+000001a0: 203d 2030 0d0a 636f 6f72 6473 203d 205b   = 0..coords = [
+000001b0: 2830 2c20 3029 5d0d 0a0d 0a0d 0a40 6170  (0, 0)]......@ap
+000001c0: 702e 726f 7574 6528 222f 222c 206d 6574  p.route("/", met
+000001d0: 686f 6473 3d5b 2247 4554 222c 2022 504f  hods=["GET", "PO
+000001e0: 5354 225d 290d 0a64 6566 2073 656e 6428  ST"])..def send(
+000001f0: 2920 2d3e 2073 7472 3a0d 0a20 2020 2023  ) -> str:..    #
+00000200: 2070 7269 6e74 2822 6865 7265 2229 0d0a   print("here")..
+00000210: 2020 2020 6966 2072 6571 7565 7374 2e6d      if request.m
+00000220: 6574 686f 6420 3d3d 2022 504f 5354 223a  ethod == "POST":
+00000230: 0d0a 2020 2020 2020 2020 2320 7072 696e  ..        # prin
+00000240: 7428 7265 7175 6573 742e 6765 745f 6a73  t(request.get_js
+00000250: 6f6e 2829 290d 0a20 2020 2020 2020 2072  on())..        r
+00000260: 6574 7572 6e20 226f 6b22 0d0a 2020 2020  eturn "ok"..    
+00000270: 7265 7475 726e 2022 2222 3c21 444f 4354  return """<!DOCT
+00000280: 5950 4520 6874 6d6c 3e0d 0a3c 6874 6d6c  YPE html>..<html
+00000290: 3e0d 0a20 203c 6865 6164 3e0d 0a20 2020  >..  <head>..   
+000002a0: 203c 6d65 7461 2068 7474 702d 6571 7569   <meta http-equi
+000002b0: 763d 2263 6f6e 7465 6e74 2d74 7970 6522  v="content-type"
+000002c0: 2063 6f6e 7465 6e74 3d22 7465 7874 2f68   content="text/h
+000002d0: 746d 6c3b 2063 6861 7273 6574 3d75 7466  tml; charset=utf
+000002e0: 2d38 222f 3e0d 0a20 2020 203c 6d65 7461  -8"/>..    <meta
+000002f0: 206e 616d 653d 2776 6965 7770 6f72 7427   name='viewport'
+00000300: 0d0a 2020 2020 2063 6f6e 7465 6e74 3d27  ..     content='
+00000310: 7769 6474 683d 6465 7669 6365 2d77 6964  width=device-wid
+00000320: 7468 2c20 696e 6974 6961 6c2d 7363 616c  th, initial-scal
+00000330: 653d 312e 302c 206d 6178 696d 756d 2d73  e=1.0, maximum-s
+00000340: 6361 6c65 3d31 2e30 2c0d 0a20 2020 2020  cale=1.0,..     
+00000350: 7573 6572 2d73 6361 6c61 626c 653d 3027  user-scalable=0'
+00000360: 203e 0d0a 2020 2020 3c73 6372 6970 7420   >..    <script 
+00000370: 7479 7065 3d22 7465 7874 2f6a 6176 6173  type="text/javas
+00000380: 6372 6970 7422 2063 6861 7273 6574 3d22  cript" charset="
+00000390: 7574 662d 3822 3e0d 0a20 2020 2066 756e  utf-8">..    fun
+000003a0: 6374 696f 6e20 696e 6974 2829 207b 0d0a  ction init() {..
+000003b0: 2020 2020 2020 2020 7661 7220 746f 7563          var touc
+000003c0: 687a 6f6e 6520 3d20 646f 6375 6d65 6e74  hzone = document
+000003d0: 2e67 6574 456c 656d 656e 7442 7949 6428  .getElementById(
+000003e0: 227a 6f6e 6522 293b 0d0a 2020 2020 2020  "zone");..      
+000003f0: 2020 746f 7563 687a 6f6e 652e 6164 6445    touchzone.addE
+00000400: 7665 6e74 4c69 7374 656e 6572 2822 746f  ventListener("to
+00000410: 7563 6865 6e64 222c 2063 6c69 636b 652c  uchend", clicke,
+00000420: 2066 616c 7365 293b 0d0a 2020 2020 2020   false);..      
+00000430: 2020 746f 7563 687a 6f6e 652e 6164 6445    touchzone.addE
+00000440: 7665 6e74 4c69 7374 656e 6572 2822 746f  ventListener("to
+00000450: 7563 686d 6f76 6522 2c20 6861 6e64 6c65  uchmove", handle
+00000460: 2c20 6661 6c73 6529 3b0d 0a20 2020 2020  , false);..     
+00000470: 2020 2074 6f75 6368 7a6f 6e65 2e61 6464     touchzone.add
+00000480: 4576 656e 744c 6973 7465 6e65 7228 2274  EventListener("t
+00000490: 6f75 6368 7374 6172 7422 2c20 746f 7374  ouchstart", tost
+000004a0: 6172 742c 2066 616c 7365 293b 0d0a 2020  art, false);..  
+000004b0: 2020 2020 2020 7661 7220 7363 726f 6c6c        var scroll
+000004c0: 7a6f 6e65 203d 2064 6f63 756d 656e 742e  zone = document.
+000004d0: 6765 7445 6c65 6d65 6e74 4279 4964 2822  getElementById("
+000004e0: 7363 726f 6c6c 2229 3b0d 0a20 2020 2020  scroll");..     
+000004f0: 2020 2073 6372 6f6c 6c7a 6f6e 652e 6164     scrollzone.ad
+00000500: 6445 7665 6e74 4c69 7374 656e 6572 2822  dEventListener("
+00000510: 746f 7563 686d 6f76 6522 2c20 7363 726f  touchmove", scro
+00000520: 6c6c 6d6f 7665 2c20 6661 6c73 6529 3b0d  llmove, false);.
+00000530: 0a20 2020 2020 2020 2073 6372 6f6c 6c7a  .        scrollz
+00000540: 6f6e 652e 6164 6445 7665 6e74 4c69 7374  one.addEventList
+00000550: 656e 6572 2822 746f 7563 6873 7461 7274  ener("touchstart
+00000560: 222c 2074 6f73 7461 7274 2c20 6661 6c73  ", tostart, fals
+00000570: 6529 3b0d 0a20 2020 207d 0d0a 0d0a 6675  e);..    }....fu
+00000580: 6e63 7469 6f6e 2073 6372 6f6c 6c6d 6f76  nction scrollmov
+00000590: 6528 6576 656e 7429 7b0d 0a20 2076 6172  e(event){..  var
+000005a0: 2061 2020 2020 3d20 6576 656e 742e 746f   a    = event.to
+000005b0: 7563 6865 735b 305d 2e70 6167 6558 3b0d  uches[0].pageX;.
+000005c0: 0a20 2076 6172 2062 2020 2020 203d 2065  .  var b     = e
+000005d0: 7665 6e74 2e74 6f75 6368 6573 5b30 5d2e  vent.touches[0].
+000005e0: 7061 6765 593b 0d0a 2020 7661 7220 7868  pageY;..  var xh
+000005f0: 7474 7020 3d20 6e65 7720 584d 4c48 7474  ttp = new XMLHtt
+00000600: 7052 6571 7565 7374 2829 3b0d 0a20 2078  pRequest();..  x
+00000610: 6874 7470 2e6f 6e72 6561 6479 7374 6174  http.onreadystat
+00000620: 6563 6861 6e67 6520 3d20 6675 6e63 7469  echange = functi
+00000630: 6f6e 2829 207b 0d0a 2020 7d3b 0d0a 2020  on() {..  };..  
+00000640: 7868 7474 702e 6f70 656e 2822 504f 5354  xhttp.open("POST
+00000650: 222c 2022 7363 726f 6c6c 6572 222c 2074  ", "scroller", t
+00000660: 7275 6529 3b0d 0a20 2078 6874 7470 2e73  rue);..  xhttp.s
+00000670: 6574 5265 7175 6573 7448 6561 6465 7228  etRequestHeader(
+00000680: 2243 6f6e 7465 6e74 2d74 7970 6522 2c20  "Content-type", 
+00000690: 2261 7070 6c69 6361 7469 6f6e 2f78 2d77  "application/x-w
+000006a0: 7777 2d66 6f72 6d2d 7572 6c65 6e63 6f64  ww-form-urlencod
+000006b0: 6564 2229 3b0d 0a20 2078 6874 7470 2e73  ed");..  xhttp.s
+000006c0: 656e 6428 2261 3d22 2b61 2b22 2662 3d22  end("a="+a+"&b="
+000006d0: 2b62 293b 0d0a 7d0d 0a0d 0a0d 0a66 756e  +b);..}......fun
+000006e0: 6374 696f 6e20 746f 7374 6172 7428 6576  ction tostart(ev
+000006f0: 656e 7429 7b0d 0a20 2076 6172 2061 2020  ent){..  var a  
+00000700: 2020 3d20 6576 656e 742e 746f 7563 6865    = event.touche
+00000710: 735b 305d 2e70 6167 6558 3b0d 0a20 2076  s[0].pageX;..  v
+00000720: 6172 2062 2020 2020 203d 2065 7665 6e74  ar b     = event
+00000730: 2e74 6f75 6368 6573 5b30 5d2e 7061 6765  .touches[0].page
+00000740: 593b 0d0a 2020 7661 7220 7868 7474 7020  Y;..  var xhttp 
+00000750: 3d20 6e65 7720 584d 4c48 7474 7052 6571  = new XMLHttpReq
+00000760: 7565 7374 2829 3b0d 0a20 2078 6874 7470  uest();..  xhttp
+00000770: 2e6f 6e72 6561 6479 7374 6174 6563 6861  .onreadystatecha
+00000780: 6e67 6520 3d20 6675 6e63 7469 6f6e 2829  nge = function()
+00000790: 207b 0d0a 2020 7d3b 0d0a 2020 7868 7474   {..  };..  xhtt
+000007a0: 702e 6f70 656e 2822 504f 5354 222c 2022  p.open("POST", "
+000007b0: 7473 7461 7274 222c 2074 7275 6529 3b0d  tstart", true);.
+000007c0: 0a20 2078 6874 7470 2e73 6574 5265 7175  .  xhttp.setRequ
+000007d0: 6573 7448 6561 6465 7228 2243 6f6e 7465  estHeader("Conte
+000007e0: 6e74 2d74 7970 6522 2c20 2261 7070 6c69  nt-type", "appli
+000007f0: 6361 7469 6f6e 2f78 2d77 7777 2d66 6f72  cation/x-www-for
+00000800: 6d2d 7572 6c65 6e63 6f64 6564 2229 3b0d  m-urlencoded");.
+00000810: 0a20 2078 6874 7470 2e73 656e 6428 2261  .  xhttp.send("a
+00000820: 3d22 2b61 2b22 2662 3d22 2b62 293b 0d0a  ="+a+"&b="+b);..
+00000830: 7d0d 0a0d 0a66 756e 6374 696f 6e20 636c  }....function cl
+00000840: 6963 6b65 2865 7665 6e74 2920 7b0d 0a20  icke(event) {.. 
+00000850: 2076 6172 2078 6874 7470 203d 206e 6577   var xhttp = new
+00000860: 2058 4d4c 4874 7470 5265 7175 6573 7428   XMLHttpRequest(
+00000870: 293b 0d0a 2020 7868 7474 702e 6f6e 7265  );..  xhttp.onre
+00000880: 6164 7973 7461 7465 6368 616e 6765 203d  adystatechange =
+00000890: 2066 756e 6374 696f 6e28 2920 7b0d 0a20   function() {.. 
+000008a0: 207d 3b0d 0a20 2076 6172 2061 203d 2065   };..  var a = e
+000008b0: 7665 6e74 2e63 6861 6e67 6564 546f 7563  vent.changedTouc
+000008c0: 6865 735b 305d 2e70 6167 6559 3b0d 0a20  hes[0].pageY;.. 
+000008d0: 2078 6874 7470 2e6f 7065 6e28 2250 4f53   xhttp.open("POS
+000008e0: 5422 2c20 2263 6c69 636b 222c 2074 7275  T", "click", tru
+000008f0: 6529 3b0d 0a20 2078 6874 7470 2e73 6574  e);..  xhttp.set
+00000900: 5265 7175 6573 7448 6561 6465 7228 2243  RequestHeader("C
+00000910: 6f6e 7465 6e74 2d74 7970 6522 2c20 2261  ontent-type", "a
+00000920: 7070 6c69 6361 7469 6f6e 2f78 2d77 7777  pplication/x-www
+00000930: 2d66 6f72 6d2d 7572 6c65 6e63 6f64 6564  -form-urlencoded
+00000940: 2229 3b0d 0a20 2078 6874 7470 2e73 656e  ");..  xhttp.sen
+00000950: 6428 2261 3d22 2b61 293b 0d0a 7d0d 0a0d  d("a="+a);..}...
+00000960: 0a66 756e 6374 696f 6e20 6472 6167 6d28  .function dragm(
+00000970: 2920 7b0d 0a20 2020 2076 6172 2062 746e  ) {..    var btn
+00000980: 203d 2064 6f63 756d 656e 742e 6765 7445   = document.getE
+00000990: 6c65 6d65 6e74 4279 4964 2822 6472 6167  lementById("drag
+000009a0: 2229 3b0d 0a20 2020 2076 6172 2078 6874  ");..    var xht
+000009b0: 7470 203d 206e 6577 2058 4d4c 4874 7470  tp = new XMLHttp
+000009c0: 5265 7175 6573 7428 293b 0d0a 2020 2020  Request();..    
+000009d0: 7868 7474 702e 6f6e 7265 6164 7973 7461  xhttp.onreadysta
+000009e0: 7465 6368 616e 6765 203d 2066 756e 6374  techange = funct
+000009f0: 696f 6e28 2920 7b0d 0a20 2020 207d 3b0d  ion() {..    };.
+00000a00: 0a20 2020 2078 6874 7470 2e6f 7065 6e28  .    xhttp.open(
+00000a10: 2250 4f53 5422 2c20 2264 7261 6468 616e  "POST", "dradhan
+00000a20: 646c 6572 222c 2074 7275 6529 3b0d 0a20  dler", true);.. 
+00000a30: 2020 2078 6874 7470 2e73 6574 5265 7175     xhttp.setRequ
+00000a40: 6573 7448 6561 6465 7228 2243 6f6e 7465  estHeader("Conte
+00000a50: 6e74 2d74 7970 6522 2c20 2261 7070 6c69  nt-type", "appli
+00000a60: 6361 7469 6f6e 2f78 2d77 7777 2d66 6f72  cation/x-www-for
+00000a70: 6d2d 7572 6c65 6e63 6f64 6564 2229 3b0d  m-urlencoded");.
+00000a80: 0a20 2020 2078 6874 7470 2e73 656e 6428  .    xhttp.send(
+00000a90: 293b 0d0a 0d0a 2020 2020 6966 2028 6274  );....    if (bt
+00000aa0: 6e2e 696e 6e65 7248 544d 4c20 3d3d 2022  n.innerHTML == "
+00000ab0: 4472 6167 206d 6f75 7365 2229 7b0d 0a20  Drag mouse"){.. 
+00000ac0: 2020 2020 2020 2062 746e 2e69 6e6e 6572         btn.inner
+00000ad0: 4854 4d4c 203d 2022 4d6f 7665 206d 6f75  HTML = "Move mou
+00000ae0: 7365 223b 0d0a 2020 2020 7d0d 0a20 2020  se";..    }..   
+00000af0: 2065 6c73 657b 0d0a 2020 2020 2020 2020   else{..        
+00000b00: 6274 6e2e 696e 6e65 7248 544d 4c20 3d20  btn.innerHTML = 
+00000b10: 2244 7261 6720 6d6f 7573 6522 3b0d 0a20  "Drag mouse";.. 
+00000b20: 2020 207d 0d0a 7d0d 0a0d 0a66 756e 6374     }..}....funct
+00000b30: 696f 6e20 7365 6e64 4461 7461 2861 2c62  ion sendData(a,b
+00000b40: 2c67 2920 7b0d 0a20 2076 6172 2078 6874  ,g) {..  var xht
+00000b50: 7470 203d 206e 6577 2058 4d4c 4874 7470  tp = new XMLHttp
+00000b60: 5265 7175 6573 7428 293b 0d0a 2020 7868  Request();..  xh
+00000b70: 7474 702e 6f6e 7265 6164 7973 7461 7465  ttp.onreadystate
+00000b80: 6368 616e 6765 203d 2066 756e 6374 696f  change = functio
+00000b90: 6e28 2920 7b0d 0a20 207d 3b0d 0a20 2078  n() {..  };..  x
+00000ba0: 6874 7470 2e6f 7065 6e28 2250 4f53 5422  http.open("POST"
+00000bb0: 2c20 2268 616e 646c 6572 222c 2074 7275  , "handler", tru
+00000bc0: 6529 3b0d 0a20 2078 6874 7470 2e73 6574  e);..  xhttp.set
+00000bd0: 5265 7175 6573 7448 6561 6465 7228 2243  RequestHeader("C
+00000be0: 6f6e 7465 6e74 2d74 7970 6522 2c20 2261  ontent-type", "a
+00000bf0: 7070 6c69 6361 7469 6f6e 2f78 2d77 7777  pplication/x-www
+00000c00: 2d66 6f72 6d2d 7572 6c65 6e63 6f64 6564  -form-urlencoded
+00000c10: 2229 3b0d 0a20 2078 6874 7470 2e73 656e  ");..  xhttp.sen
+00000c20: 6428 2261 3d22 2b61 2b22 2662 3d22 2b62  d("a="+a+"&b="+b
+00000c30: 293b 0d0a 7d0d 0a0d 0a0d 0a20 6675 6e63  );..}...... func
+00000c40: 7469 6f6e 2068 616e 646c 6528 6576 656e  tion handle(even
+00000c50: 7429 207b 0d0a 2020 7661 7220 616c 7068  t) {..  var alph
+00000c60: 6120 2020 203d 2065 7665 6e74 2e74 6f75  a    = event.tou
+00000c70: 6368 6573 5b30 5d2e 7061 6765 583b 0d0a  ches[0].pageX;..
+00000c80: 2020 7661 7220 6265 7461 2020 2020 203d    var beta     =
+00000c90: 2065 7665 6e74 2e74 6f75 6368 6573 5b30   event.touches[0
+00000ca0: 5d2e 7061 6765 593b 0d0a 2020 7365 6e64  ].pageY;..  send
+00000cb0: 4461 7461 2861 6c70 6861 2c62 6574 6129  Data(alpha,beta)
+00000cc0: 3b0d 0a7d 0d0a 0d0a 0d0a 6675 6e63 7469  ;..}......functi
+00000cd0: 6f6e 206f 6e5f 696e 7075 7428 297b 0d0a  on on_input(){..
+00000ce0: 2020 7661 7220 6461 7461 203d 2064 6f63    var data = doc
+00000cf0: 756d 656e 742e 6765 7445 6c65 6d65 6e74  ument.getElement
+00000d00: 4279 4964 2822 696e 7066 6965 6c64 2229  ById("inpfield")
+00000d10: 2e76 616c 7565 3b0d 0a20 2076 6172 2078  .value;..  var x
+00000d20: 6874 7470 203d 206e 6577 2058 4d4c 4874  http = new XMLHt
+00000d30: 7470 5265 7175 6573 7428 293b 0d0a 2020  tpRequest();..  
+00000d40: 7868 7474 702e 6f6e 7265 6164 7973 7461  xhttp.onreadysta
+00000d50: 7465 6368 616e 6765 203d 2066 756e 6374  techange = funct
+00000d60: 696f 6e28 2920 7b0d 0a20 207d 3b0d 0a20  ion() {..  };.. 
+00000d70: 2078 6874 7470 2e6f 7065 6e28 2250 4f53   xhttp.open("POS
+00000d80: 5422 2c20 2274 7970 6564 222c 2074 7275  T", "typed", tru
+00000d90: 6529 3b0d 0a20 2078 6874 7470 2e73 6574  e);..  xhttp.set
+00000da0: 5265 7175 6573 7448 6561 6465 7228 2243  RequestHeader("C
+00000db0: 6f6e 7465 6e74 2d74 7970 6522 2c20 2261  ontent-type", "a
+00000dc0: 7070 6c69 6361 7469 6f6e 2f78 2d77 7777  pplication/x-www
+00000dd0: 2d66 6f72 6d2d 7572 6c65 6e63 6f64 6564  -form-urlencoded
+00000de0: 2229 3b0d 0a20 2078 6874 7470 2e73 656e  ");..  xhttp.sen
+00000df0: 6428 2264 6174 613d 222b 6461 7461 293b  d("data="+data);
+00000e00: 0d0a 7d0d 0a66 756e 6374 696f 6e20 656e  ..}..function en
+00000e10: 7465 725f 6275 7428 297b 0d0a 2020 7661  ter_but(){..  va
+00000e20: 7220 7868 7474 7020 3d20 6e65 7720 584d  r xhttp = new XM
+00000e30: 4c48 7474 7052 6571 7565 7374 2829 3b0d  LHttpRequest();.
+00000e40: 0a20 2078 6874 7470 2e6f 6e72 6561 6479  .  xhttp.onready
+00000e50: 7374 6174 6563 6861 6e67 6520 3d20 6675  statechange = fu
+00000e60: 6e63 7469 6f6e 2829 207b 0d0a 2020 7d3b  nction() {..  };
+00000e70: 0d0a 2020 7868 7474 702e 6f70 656e 2822  ..  xhttp.open("
+00000e80: 504f 5354 222c 2022 656e 7465 7222 2c20  POST", "enter", 
+00000e90: 7472 7565 293b 0d0a 2020 7868 7474 702e  true);..  xhttp.
+00000ea0: 7365 7452 6571 7565 7374 4865 6164 6572  setRequestHeader
+00000eb0: 2822 436f 6e74 656e 742d 7479 7065 222c  ("Content-type",
+00000ec0: 2022 6170 706c 6963 6174 696f 6e2f 782d   "application/x-
+00000ed0: 7777 772d 666f 726d 2d75 726c 656e 636f  www-form-urlenco
+00000ee0: 6465 6422 293b 0d0a 2020 7868 7474 702e  ded");..  xhttp.
+00000ef0: 7365 6e64 2822 6461 7461 3d22 2b22 6461  send("data="+"da
+00000f00: 7461 2229 3b0d 0a7d 0d0a 0d0a 0d0a 0d0a  ta");..}........
+00000f10: 0d0a 2020 2020 3c2f 7363 7269 7074 3e0d  ..    </script>.
+00000f20: 0a0d 0a20 2020 203c 6d65 7461 206e 616d  ...    <meta nam
+00000f30: 653d 2222 2063 6f6e 7465 6e74 3d22 223e  e="" content="">
+00000f40: 0d0a 2020 2020 3c74 6974 6c65 3e3c 2f74  ..    <title></t
+00000f50: 6974 6c65 3e0d 0a20 203c 7374 796c 653e  itle>..  <style>
+00000f60: 0d0a 2020 2e63 656e 7465 727b 0d0a 2020  ..  .center{..  
+00000f70: 2020 706f 7369 7469 6f6e 3a20 6669 7865    position: fixe
+00000f80: 643b 0d0a 2020 2020 6261 636b 6772 6f75  d;..    backgrou
+00000f90: 6e64 2d63 6f6c 6f72 3a20 7267 6228 3233  nd-color: rgb(23
+00000fa0: 302c 3233 302c 3233 3029 3b0d 0a20 2020  0,230,230);..   
+00000fb0: 2077 6964 7468 3a38 3025 3b0d 0a20 2020   width:80%;..   
+00000fc0: 2068 6569 6768 743a 3430 3070 783b 0d0a   height:400px;..
+00000fd0: 2020 2020 746f 703a 3330 3070 783b 0d0a      top:300px;..
+00000fe0: 2020 2020 6c65 6674 3a34 3625 3b0d 0a20      left:46%;.. 
+00000ff0: 2020 2063 6f6c 6f72 3a72 6762 2832 3030     color:rgb(200
+00001000: 2c32 3030 2c32 3030 293b 0d0a 2020 2020  ,200,200);..    
+00001010: 666f 6e74 2d77 6569 6768 743a 626f 6c64  font-weight:bold
+00001020: 3b0d 0a20 2020 2074 7261 6e73 666f 726d  ;..    transform
+00001030: 3a20 7472 616e 736c 6174 6528 2d35 3025  : translate(-50%
+00001040: 2c2d 3530 2529 3b0d 0a20 2020 202d 7765  ,-50%);..    -we
+00001050: 626b 6974 2d74 6f75 6368 2d63 616c 6c6f  bkit-touch-callo
+00001060: 7574 3a20 6e6f 6e65 3b0d 0a20 2020 202d  ut: none;..    -
+00001070: 7765 626b 6974 2d75 7365 722d 7365 6c65  webkit-user-sele
+00001080: 6374 3a20 6e6f 6e65 3b0d 0a20 2020 202d  ct: none;..    -
+00001090: 6b68 746d 6c2d 7573 6572 2d73 656c 6563  khtml-user-selec
+000010a0: 743a 206e 6f6e 653b 0d0a 2020 2020 2d6d  t: none;..    -m
+000010b0: 6f7a 2d75 7365 722d 7365 6c65 6374 3a20  oz-user-select: 
+000010c0: 6e6f 6e65 3b0d 0a20 2020 202d 6d73 2d75  none;..    -ms-u
+000010d0: 7365 722d 7365 6c65 6374 3a20 6e6f 6e65  ser-select: none
+000010e0: 3b0d 0a20 2020 2075 7365 722d 7365 6c65  ;..    user-sele
+000010f0: 6374 3a20 6e6f 6e65 3b0d 0a20 2020 7d0d  ct: none;..   }.
+00001100: 0a20 2020 6874 6d6c 7b0d 0a20 2020 746f  .   html{..   to
+00001110: 7563 682d 6163 7469 6f6e 3a70 616e 2d64  uch-action:pan-d
+00001120: 6f77 6e0d 0a20 2020 7d0d 0a0d 0a20 2020  own..   }....   
+00001130: 2e73 6372 6f6c 6c61 7265 617b 0d0a 2020  .scrollarea{..  
+00001140: 2020 706f 7369 7469 6f6e 3a20 6669 7865    position: fixe
+00001150: 643b 0d0a 2020 2020 6261 636b 6772 6f75  d;..    backgrou
+00001160: 6e64 2d63 6f6c 6f72 3a20 7267 6228 3233  nd-color: rgb(23
+00001170: 302c 3233 302c 3233 3029 3b0d 0a20 2020  0,230,230);..   
+00001180: 2077 6964 7468 3a33 3070 783b 0d0a 2020   width:30px;..  
+00001190: 2020 6865 6967 6874 3a34 3030 7078 3b0d    height:400px;.
+000011a0: 0a20 2020 2074 6f70 3a33 3030 7078 3b0d  .    top:300px;.
+000011b0: 0a20 2020 206c 6566 743a 3932 2e30 3525  .    left:92.05%
+000011c0: 3b0d 0a20 2020 2063 6f6c 6f72 3a72 6762  ;..    color:rgb
+000011d0: 2832 3030 2c32 3030 2c32 3030 293b 0d0a  (200,200,200);..
+000011e0: 2020 2020 666f 6e74 2d77 6569 6768 743a      font-weight:
+000011f0: 626f 6c64 3b0d 0a20 2020 2074 7261 6e73  bold;..    trans
+00001200: 666f 726d 3a20 7472 616e 736c 6174 6528  form: translate(
+00001210: 2d35 3025 2c2d 3530 2529 3b0d 0a20 2020  -50%,-50%);..   
+00001220: 202d 7765 626b 6974 2d74 6f75 6368 2d63   -webkit-touch-c
+00001230: 616c 6c6f 7574 3a20 6e6f 6e65 3b0d 0a20  allout: none;.. 
+00001240: 2020 202d 7765 626b 6974 2d75 7365 722d     -webkit-user-
+00001250: 7365 6c65 6374 3a20 6e6f 6e65 3b0d 0a20  select: none;.. 
+00001260: 2020 202d 6b68 746d 6c2d 7573 6572 2d73     -khtml-user-s
+00001270: 656c 6563 743a 206e 6f6e 653b 0d0a 2020  elect: none;..  
+00001280: 2020 2d6d 6f7a 2d75 7365 722d 7365 6c65    -moz-user-sele
+00001290: 6374 3a20 6e6f 6e65 3b0d 0a20 2020 202d  ct: none;..    -
+000012a0: 6d73 2d75 7365 722d 7365 6c65 6374 3a20  ms-user-select: 
+000012b0: 6e6f 6e65 3b0d 0a20 2020 2075 7365 722d  none;..    user-
+000012c0: 7365 6c65 6374 3a20 6e6f 6e65 3b0d 0a20  select: none;.. 
+000012d0: 2020 2074 6578 742d 616c 6967 6e3a 6365     text-align:ce
+000012e0: 6e74 6572 3b0d 0a20 2020 7d0d 0a0d 0a0d  nter;..   }.....
+000012f0: 0a20 203c 2f73 7479 6c65 3e0d 0a20 203c  .  </style>..  <
+00001300: 2f68 6561 643e 0d0a 2020 3c62 6f64 7920  /head>..  <body 
+00001310: 6f6e 6c6f 6164 3d22 696e 6974 2829 223e  onload="init()">
+00001320: 0d0a 2020 3c70 2073 7479 6c65 3d22 7465  ..  <p style="te
+00001330: 7874 2d61 6c69 676e 3a63 656e 7465 723b  xt-align:center;
+00001340: 223e 5479 7065 206f 6e20 5043 0d0a 2020  ">Type on PC..  
+00001350: 3c69 6e70 7574 2069 643d 2269 6e70 6669  <input id="inpfi
+00001360: 656c 6422 7479 7065 3d22 7465 7874 2220  eld"type="text" 
+00001370: 6f6e 696e 7075 743d 6f6e 5f69 6e70 7574  oninput=on_input
+00001380: 2829 3e3c 2f69 6e70 7574 3e0d 0a20 203c  ()></input>..  <
+00001390: 6275 7474 6f6e 2074 7970 653d 2262 7574  button type="but
+000013a0: 746f 6e22 206f 6e63 6c69 636b 3d22 656e  ton" onclick="en
+000013b0: 7465 725f 6275 7428 2922 3e45 6e74 6572  ter_but()">Enter
+000013c0: 3c2f 6275 7474 6f6e 3e3c 2f70 3e0d 0a20  </button></p>.. 
+000013d0: 203c 6469 7620 7374 796c 653d 2274 6578   <div style="tex
+000013e0: 742d 616c 6967 6e3a 6365 6e74 6572 3b22  t-align:center;"
+000013f0: 3e0d 0a20 2020 2020 203c 6275 7474 6f6e  >..      <button
+00001400: 2069 643d 2264 7261 6722 2074 7970 653d   id="drag" type=
+00001410: 2262 7574 746f 6e22 206f 6e63 6c69 636b  "button" onclick
+00001420: 3d22 6472 6167 6d28 2922 3e44 7261 6720  ="dragm()">Drag 
+00001430: 6d6f 7573 653c 2f62 7574 746f 6e3e 0d0a  mouse</button>..
+00001440: 2020 3c2f 6469 763e 0d0a 2020 2020 3c64    </div>..    <d
+00001450: 6976 2063 6c61 7373 3d22 6365 6e74 6572  iv class="center
+00001460: 2220 6964 3d22 7a6f 6e65 223e 0d0a 2020  " id="zone">..  
+00001470: 2020 2020 2020 3c70 2061 6c69 676e 3d22        <p align="
+00001480: 6365 6e74 6572 223e 3c62 723e 3c62 723e  center"><br><br>
+00001490: 3c62 723e 3c62 723e 3c62 723e 3c62 723e  <br><br><br><br>
+000014a0: 4c65 6674 2063 6c69 636b 2061 7265 613c  Left click area<
+000014b0: 6272 3e3c 6272 3e3c 6272 3e3c 6272 3e3c  br><br><br><br><
+000014c0: 6272 3e3c 6272 3e3c 6872 3e3c 2f70 3e0d  br><br><hr></p>.
+000014d0: 0a20 2020 2020 2020 203c 7020 616c 6967  .        <p alig
+000014e0: 6e3d 2263 656e 7465 7222 3e3c 6272 3e52  n="center"><br>R
+000014f0: 6967 6874 2063 6c69 636b 2061 7265 613c  ight click area<
+00001500: 2f70 3e0d 0a20 2020 203c 2f64 6976 3e0d  /p>..    </div>.
+00001510: 0a20 2020 203c 6469 7620 636c 6173 733d  .    <div class=
+00001520: 2273 6372 6f6c 6c61 7265 6122 2069 643d  "scrollarea" id=
+00001530: 2273 6372 6f6c 6c22 3e0d 0a20 2020 2020  "scroll">..     
+00001540: 2020 3c70 3e3c 6272 3e3c 6272 3e3c 6272    <p><br><br><br
+00001550: 3e3c 6272 3e3c 6272 3e53 3c62 723e 433c  ><br><br>S<br>C<
+00001560: 6272 3e52 3c62 723e 4f3c 6272 3e4c 3c62  br>R<br>O<br>L<b
+00001570: 723e 4c3c 2f70 3e0d 0a20 2020 203c 2f64  r>L</p>..    </d
+00001580: 6976 3e0d 0a20 203c 2f62 6f64 793e 0d0a  iv>..  </body>..
+00001590: 3c2f 6874 6d6c 3e22 2222 0d0a 0d0a 0d0a  </html>"""......
+000015a0: 4061 7070 2e72 6f75 7465 2822 2f68 616e  @app.route("/han
+000015b0: 646c 6572 222c 206d 6574 686f 6473 3d5b  dler", methods=[
+000015c0: 2250 4f53 5422 5d29 0d0a 6465 6620 6861  "POST"])..def ha
+000015d0: 6e64 6c65 2829 202d 3e20 7374 723a 0d0a  ndle() -> str:..
+000015e0: 2020 2020 676c 6f62 616c 206d 6f76 696e      global movin
+000015f0: 672c 2063 6f72 646c 7374 2c20 6c61 7374  g, cordlst, last
+00001600: 636f 7264 730d 0a20 2020 206c 7374 203d  cords..    lst =
+00001610: 205b 5d0d 0a20 2020 2061 203d 2072 6571   []..    a = req
+00001620: 7565 7374 2e66 6f72 6d5b 2261 225d 0d0a  uest.form["a"]..
+00001630: 2020 2020 6220 3d20 7265 7175 6573 742e      b = request.
+00001640: 666f 726d 5b22 6222 5d0d 0a20 2020 2061  form["b"]..    a
+00001650: 203d 2066 6c6f 6174 2861 290d 0a20 2020   = float(a)..   
+00001660: 2062 203d 2066 6c6f 6174 2862 290d 0a20   b = float(b).. 
+00001670: 2020 206d 6f76 696e 6720 3d20 5472 7565     moving = True
+00001680: 0d0a 2020 2020 636f 6f72 6473 203d 2028  ..    coords = (
+00001690: 612c 2062 290d 0a20 2020 206c 782c 206c  a, b)..    lx, l
+000016a0: 7920 3d20 6c61 7374 636f 7264 730d 0a20  y = lastcords.. 
+000016b0: 2020 2063 782c 2063 7920 3d20 636f 6f72     cx, cy = coor
+000016c0: 6473 0d0a 2020 2020 2320 7072 696e 7428  ds..    # print(
+000016d0: 6378 2c63 7929 0d0a 2020 2020 2320 702e  cx,cy)..    # p.
+000016e0: 6d6f 7665 5265 6c28 2863 782d 6c78 292f  moveRel((cx-lx)/
+000016f0: 322c 2863 792d 6c79 292f 3229 0d0a 2020  2,(cy-ly)/2)..  
+00001700: 2020 7468 7265 6164 696e 672e 5468 7265    threading.Thre
+00001710: 6164 2874 6172 6765 743d 6c61 6d62 6461  ad(target=lambda
+00001720: 3a20 702e 6d6f 7665 5265 6c28 2863 7820  : p.moveRel((cx 
+00001730: 2d20 6c78 2920 2a20 322c 2028 6379 202d  - lx) * 2, (cy -
+00001740: 206c 7929 202a 2032 2929 2e73 7461 7274   ly) * 2)).start
+00001750: 2829 0d0a 2020 2020 6c61 7374 636f 7264  ()..    lastcord
+00001760: 7320 3d20 636f 6f72 6473 0d0a 2020 2020  s = coords..    
+00001770: 7265 7475 726e 2022 3122 0d0a 0d0a 0d0a  return "1"......
+00001780: 4061 7070 2e72 6f75 7465 2822 2f73 6372  @app.route("/scr
+00001790: 6f6c 6c65 7222 2c20 6d65 7468 6f64 733d  oller", methods=
+000017a0: 5b22 504f 5354 225d 290d 0a64 6566 2073  ["POST"])..def s
+000017b0: 6372 6f6c 6c65 7272 2829 202d 3e20 7374  crollerr() -> st
+000017c0: 723a 0d0a 2020 2020 676c 6f62 616c 206d  r:..    global m
+000017d0: 6f76 696e 672c 2063 6f72 646c 7374 2c20  oving, cordlst, 
+000017e0: 6c61 7374 636f 7264 7332 0d0a 2020 2020  lastcords2..    
+000017f0: 6120 3d20 7265 7175 6573 742e 666f 726d  a = request.form
+00001800: 5b22 6122 5d0d 0a20 2020 2062 203d 2072  ["a"]..    b = r
+00001810: 6571 7565 7374 2e66 6f72 6d5b 2262 225d  equest.form["b"]
+00001820: 0d0a 2020 2020 6120 3d20 666c 6f61 7428  ..    a = float(
+00001830: 6129 0d0a 2020 2020 6220 3d20 666c 6f61  a)..    b = floa
+00001840: 7428 6229 0d0a 2020 2020 636f 6f72 6473  t(b)..    coords
+00001850: 203d 2028 612c 2062 290d 0a20 2020 206c   = (a, b)..    l
+00001860: 782c 206c 7920 3d20 6c61 7374 636f 7264  x, ly = lastcord
+00001870: 7332 0d0a 2020 2020 6378 2c20 6379 203d  s2..    cx, cy =
+00001880: 2063 6f6f 7264 730d 0a20 2020 2069 6620   coords..    if 
+00001890: 6379 203c 206c 793a 0d0a 2020 2020 2020  cy < ly:..      
+000018a0: 2020 7468 7265 6164 696e 672e 5468 7265    threading.Thre
+000018b0: 6164 2874 6172 6765 743d 6c61 6d62 6461  ad(target=lambda
+000018c0: 3a20 702e 7363 726f 6c6c 2835 3029 292e  : p.scroll(50)).
+000018d0: 7374 6172 7428 290d 0a20 2020 2069 6620  start()..    if 
+000018e0: 6379 203e 206c 793a 0d0a 2020 2020 2020  cy > ly:..      
+000018f0: 2020 7468 7265 6164 696e 672e 5468 7265    threading.Thre
+00001900: 6164 2874 6172 6765 743d 6c61 6d62 6461  ad(target=lambda
+00001910: 3a20 702e 7363 726f 6c6c 282d 3530 2929  : p.scroll(-50))
+00001920: 2e73 7461 7274 2829 0d0a 2020 2020 6c61  .start()..    la
+00001930: 7374 636f 7264 7332 203d 2063 6f6f 7264  stcords2 = coord
+00001940: 730d 0a20 2020 2072 6574 7572 6e20 2231  s..    return "1
+00001950: 220d 0a0d 0a0d 0a40 6170 702e 726f 7574  "......@app.rout
+00001960: 6528 222f 7473 7461 7274 222c 206d 6574  e("/tstart", met
+00001970: 686f 6473 3d5b 2250 4f53 5422 5d29 0d0a  hods=["POST"])..
+00001980: 6465 6620 7374 6172 7474 2829 202d 3e20  def startt() -> 
+00001990: 7374 723a 0d0a 2020 2020 676c 6f62 616c  str:..    global
+000019a0: 206c 6173 7463 6f72 6473 2c20 6c61 7374   lastcords, last
+000019b0: 636f 7264 7332 0d0a 2020 2020 2320 7072  cords2..    # pr
+000019c0: 696e 7428 2265 6e64 2229 0d0a 2020 2020  int("end")..    
+000019d0: 6120 3d20 7265 7175 6573 742e 666f 726d  a = request.form
+000019e0: 5b22 6122 5d0d 0a20 2020 2062 203d 2072  ["a"]..    b = r
+000019f0: 6571 7565 7374 2e66 6f72 6d5b 2262 225d  equest.form["b"]
+00001a00: 0d0a 2020 2020 2320 7072 696e 7428 612c  ..    # print(a,
+00001a10: 6229 0d0a 2020 2020 6120 3d20 666c 6f61  b)..    a = floa
+00001a20: 7428 6129 0d0a 2020 2020 6220 3d20 666c  t(a)..    b = fl
+00001a30: 6f61 7428 6229 0d0a 2020 2020 6c61 7374  oat(b)..    last
+00001a40: 636f 7264 7320 3d20 2861 2c20 6229 0d0a  cords = (a, b)..
+00001a50: 2020 2020 6c61 7374 636f 7264 7332 203d      lastcords2 =
+00001a60: 2028 612c 2062 290d 0a20 2020 2072 6574   (a, b)..    ret
+00001a70: 7572 6e20 2231 220d 0a0d 0a0d 0a40 6170  urn "1"......@ap
+00001a80: 702e 726f 7574 6528 222f 636c 6963 6b22  p.route("/click"
+00001a90: 2c20 6d65 7468 6f64 733d 5b22 504f 5354  , methods=["POST
+00001aa0: 225d 290d 0a64 6566 2064 6f5f 636c 6963  "])..def do_clic
+00001ab0: 6b28 2920 2d3e 2073 7472 3a0d 0a20 2020  k() -> str:..   
+00001ac0: 2067 6c6f 6261 6c20 6d6f 7669 6e67 0d0a   global moving..
+00001ad0: 2020 2020 6966 206e 6f74 206d 6f76 696e      if not movin
+00001ae0: 673a 0d0a 2020 2020 2020 2020 6120 3d20  g:..        a = 
+00001af0: 7265 7175 6573 742e 666f 726d 5b22 6122  request.form["a"
+00001b00: 5d0d 0a20 2020 2020 2020 2023 2070 7269  ]..        # pri
+00001b10: 6e74 2861 290d 0a20 2020 2020 2020 2061  nt(a)..        a
+00001b20: 203d 2066 6c6f 6174 2861 290d 0a20 2020   = float(a)..   
+00001b30: 2020 2020 2069 6620 6120 3c20 3430 303a       if a < 400:
+00001b40: 0d0a 2020 2020 2020 2020 2020 2020 702e  ..            p.
+00001b50: 636c 6963 6b28 290d 0a20 2020 2020 2020  click()..       
+00001b60: 2069 6620 6120 3e3d 2034 3030 3a0d 0a20   if a >= 400:.. 
+00001b70: 2020 2020 2020 2020 2020 2070 2e72 6967             p.rig
+00001b80: 6874 436c 6963 6b28 290d 0a0d 0a20 2020  htClick()....   
+00001b90: 206d 6f76 696e 6720 3d20 4661 6c73 650d   moving = False.
+00001ba0: 0a20 2020 2072 6574 7572 6e20 2231 220d  .    return "1".
+00001bb0: 0a0d 0a0d 0a40 6170 702e 726f 7574 6528  .....@app.route(
+00001bc0: 222f 7479 7065 6422 2c20 6d65 7468 6f64  "/typed", method
+00001bd0: 733d 5b22 504f 5354 225d 290d 0a64 6566  s=["POST"])..def
+00001be0: 2074 7970 6569 7428 2920 2d3e 2073 7472   typeit() -> str
+00001bf0: 3a0d 0a20 2020 2067 6c6f 6261 6c20 7479  :..    global ty
+00001c00: 7065 5f64 6174 612c 206f 6c64 5f64 6174  pe_data, old_dat
+00001c10: 610d 0a20 2020 2064 6174 6120 3d20 7265  a..    data = re
+00001c20: 7175 6573 742e 666f 726d 5b22 6461 7461  quest.form["data
+00001c30: 225d 0d0a 2020 2020 7479 7065 5f64 6174  "]..    type_dat
+00001c40: 6120 3d20 7374 7228 6461 7461 290d 0a20  a = str(data).. 
+00001c50: 2020 2069 6620 6c65 6e28 7479 7065 5f64     if len(type_d
+00001c60: 6174 6129 203e 206c 656e 286f 6c64 5f64  ata) > len(old_d
+00001c70: 6174 6129 3a0d 0a20 2020 2020 2020 2070  ata):..        p
+00001c80: 2e74 7970 6577 7269 7465 2874 7970 655f  .typewrite(type_
+00001c90: 6461 7461 5b6c 656e 2874 7970 655f 6461  data[len(type_da
+00001ca0: 7461 2920 2d20 315d 290d 0a20 2020 2065  ta) - 1])..    e
+00001cb0: 6c73 653a 0d0a 2020 2020 2020 2020 702e  lse:..        p.
+00001cc0: 7072 6573 7328 2262 6163 6b73 7061 6365  press("backspace
+00001cd0: 222c 206c 656e 286f 6c64 5f64 6174 6129  ", len(old_data)
+00001ce0: 202d 206c 656e 2874 7970 655f 6461 7461   - len(type_data
+00001cf0: 2929 0d0a 2020 2020 6f6c 645f 6461 7461  ))..    old_data
+00001d00: 203d 2074 7970 655f 6461 7461 0d0a 2020   = type_data..  
+00001d10: 2020 7265 7475 726e 2022 3122 0d0a 0d0a    return "1"....
+00001d20: 0d0a 4061 7070 2e72 6f75 7465 2822 2f65  ..@app.route("/e
+00001d30: 6e74 6572 222c 206d 6574 686f 6473 3d5b  nter", methods=[
+00001d40: 2250 4f53 5422 5d29 0d0a 6465 6620 736c  "POST"])..def sl
+00001d50: 6173 684e 2829 202d 3e20 7374 723a 0d0a  ashN() -> str:..
+00001d60: 2020 2020 702e 7072 6573 7328 2265 6e74      p.press("ent
+00001d70: 6572 2229 0d0a 2020 2020 7265 7475 726e  er")..    return
+00001d80: 2022 3122 0d0a 0d0a 0d0a 4061 7070 2e72   "1"......@app.r
+00001d90: 6f75 7465 2822 2f64 7261 6468 616e 646c  oute("/dradhandl
+00001da0: 6572 222c 206d 6574 686f 6473 3d5b 2250  er", methods=["P
+00001db0: 4f53 5422 5d29 0d0a 6465 6620 6768 6173  OST"])..def ghas
+00001dc0: 6974 5f6d 6f75 7365 2829 202d 3e20 7374  it_mouse() -> st
+00001dd0: 723a 0d0a 2020 2020 676c 6f62 616c 2064  r:..    global d
+00001de0: 7261 670d 0a20 2020 2023 2070 7269 6e74  rag..    # print
+00001df0: 2864 7261 6729 0d0a 2020 2020 6966 2064  (drag)..    if d
+00001e00: 7261 6720 3d3d 2054 7275 653a 0d0a 2020  rag == True:..  
+00001e10: 2020 2020 2020 6472 6167 203d 2046 616c        drag = Fal
+00001e20: 7365 0d0a 2020 2020 2020 2020 702e 6d6f  se..        p.mo
+00001e30: 7573 6555 7028 290d 0a0d 0a20 2020 2065  useUp()....    e
+00001e40: 6c73 653a 0d0a 2020 2020 2020 2020 6472  lse:..        dr
+00001e50: 6167 203d 2054 7275 650d 0a20 2020 2020  ag = True..     
+00001e60: 2020 2070 2e6d 6f75 7365 446f 776e 2829     p.mouseDown()
+00001e70: 0d0a 0d0a 2020 2020 7265 7475 726e 2022  ....    return "
+00001e80: 3122 0d0a 0d0a 0d0a 6465 6620 7374 6172  1"......def star
+00001e90: 745f 7365 7276 6572 2870 6f72 743d 3830  t_server(port=80
+00001ea0: 3030 2c20 7072 696e 745f 6d73 673d 5472  00, print_msg=Tr
+00001eb0: 7565 293a 0d0a 2020 2020 6966 2070 7269  ue):..    if pri
+00001ec0: 6e74 5f6d 7367 3a0d 0a20 2020 2020 2020  nt_msg:..       
+00001ed0: 2070 7269 6e74 2822 5365 7276 6572 2073   print("Server s
+00001ee0: 7461 7274 6564 2061 7420 6c6f 6361 6c5f  tarted at local_
+00001ef0: 6970 5f6f 665f 7468 6973 5f70 633a 2573  ip_of_this_pc:%s
+00001f00: 2220 2520 706f 7274 290d 0a20 2020 2020  " % port)..     
+00001f10: 2020 2070 7269 6e74 2822 5072 696e 7420     print("Print 
+00001f20: 4374 726c 2b43 2074 6f20 6578 6974 2229  Ctrl+C to exit")
+00001f30: 0d0a 2020 2020 6170 702e 7275 6e28 686f  ..    app.run(ho
+00001f40: 7374 3d22 302e 302e 302e 3022 2c20 706f  st="0.0.0.0", po
+00001f50: 7274 3d70 6f72 7429 0d0a 0d0a 0d0a 2320  rt=port)......# 
+00001f60: 6170 702e 7275 6e28 686f 7374 3d27 302e  app.run(host='0.
+00001f70: 302e 302e 3027 290d 0a23 0d0a 230d 0a23  0.0.0')..#..#..#
+00001f80: 2064 6566 206d 6169 6e28 293a 0d0a 2320   def main():..# 
+00001f90: 2020 2020 6170 702e 7275 6e28 686f 7374      app.run(host
+00001fa0: 3d22 3139 322e 3136 382e 3433 2e31 3722  ="192.168.43.17"
+00001fb0: 2c20 706f 7274 3d33 3329 0d0a 230d 0a23  , port=33)..#..#
+00001fc0: 0d0a 2320 6966 205f 5f6e 616d 655f 5f20  ..# if __name__ 
+00001fd0: 3d3d 2022 5f5f 6d61 696e 5f5f 223a 0d0a  == "__main__":..
+00001fe0: 2320 2020 2020 6d61 696e 2829 0d0a 2320  #     main()..# 
+00001ff0: 2020 2020 6170 702e 7275 6e28 686f 7374      app.run(host
+00002000: 3d27 6c6f 6361 6c68 6f73 7427 290d 0a    ='localhost')..
```

### Comparing `AsyncPywhatKit-2.2.6/AsyncPywhatKit/src/sc.py` & `AsyncPywhatKit-2.2.7/AsyncPywhatKit/src/sc.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,62 +1,62 @@
-import os
-import platform
-
-try:
-    import winerror
-except ImportError or ModuleNotFoundError:
-    pass
-
-osname = platform.system()
-
-
-async def shutdown(time: int = 20) -> None:
-    """Schedules a Shutdown after the Specified Time"""
-
-    if "window" in osname.lower():
-        cont = f"shutdown -s -t {time}"
-        error_code = os.system(cont)
-        if error_code in [winerror.ERROR_SHUTDOWN_IN_PROGRESS, 1115]:
-            print("A Shutdown Process has already been Scheduled!")
-        else:
-            print(f"Your System will Shutdown in {time} Seconds!")
-
-    elif "linux" in osname.lower():
-        cont = f"shutdown -h {time}"
-        os.system(cont)
-        print(f"Your System will Shutdown in {time} Minutes!")
-
-    elif "darwin" in osname.lower():
-        cont = f"shutdown -h -t {time}"
-        os.system(cont)
-        print(f"Your System will Shutdown in {time} Minutes!")
-
-    else:
-        raise Warning(
-            f"Available on Windows, Mac and Linux only, can't Execute on {osname}"
-        )
-
-
-def cancel_shutdown() -> None:
-    """Cancels the Scheduled Shutdown"""
-
-    if "window" in osname.lower():
-        error_code = os.system("shutdown /a")
-        if error_code == winerror.ERROR_NO_SHUTDOWN_IN_PROGRESS:
-            print(
-                "Shutdown Cancellation process has been Aborted! [NO Shutdown Scheduled]"
-            )
-        else:
-            print("Shutdown has been Cancelled!")
-
-    elif "linux" in osname.lower():
-        os.system("shutdown -c")
-        print("Shutdown has been Cancelled!")
-
-    elif "darwin" in osname.lower():
-        os.system("killall shutdown")
-        print("Shutdown has been Cancelled!")
-
-    else:
-        raise Warning(
-            f"Available on Windows, Mac and Linux only, can't Execute on {osname}"
-        )
+import os
+import platform
+
+try:
+    import winerror
+except ImportError or ModuleNotFoundError:
+    pass
+
+osname = platform.system()
+
+
+async def shutdown(time: int = 20) -> None:
+    """Schedules a Shutdown after the Specified Time"""
+
+    if "window" in osname.lower():
+        cont = f"shutdown -s -t {time}"
+        error_code = os.system(cont)
+        if error_code in [winerror.ERROR_SHUTDOWN_IN_PROGRESS, 1115]:
+            print("A Shutdown Process has already been Scheduled!")
+        else:
+            print(f"Your System will Shutdown in {time} Seconds!")
+
+    elif "linux" in osname.lower():
+        cont = f"shutdown -h {time}"
+        os.system(cont)
+        print(f"Your System will Shutdown in {time} Minutes!")
+
+    elif "darwin" in osname.lower():
+        cont = f"shutdown -h -t {time}"
+        os.system(cont)
+        print(f"Your System will Shutdown in {time} Minutes!")
+
+    else:
+        raise Warning(
+            f"Available on Windows, Mac and Linux only, can't Execute on {osname}"
+        )
+
+
+def cancel_shutdown() -> None:
+    """Cancels the Scheduled Shutdown"""
+
+    if "window" in osname.lower():
+        error_code = os.system("shutdown /a")
+        if error_code == winerror.ERROR_NO_SHUTDOWN_IN_PROGRESS:
+            print(
+                "Shutdown Cancellation process has been Aborted! [NO Shutdown Scheduled]"
+            )
+        else:
+            print("Shutdown has been Cancelled!")
+
+    elif "linux" in osname.lower():
+        os.system("shutdown -c")
+        print("Shutdown has been Cancelled!")
+
+    elif "darwin" in osname.lower():
+        os.system("killall shutdown")
+        print("Shutdown has been Cancelled!")
+
+    else:
+        raise Warning(
+            f"Available on Windows, Mac and Linux only, can't Execute on {osname}"
+        )
```

### Comparing `AsyncPywhatKit-2.2.6/AsyncPywhatKit/src/whats.py` & `AsyncPywhatKit-2.2.7/AsyncPywhatKit/src/whats.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,365 +1,376 @@
-import time
-import typing
-import webbrowser as web
-from datetime import datetime
-from re import fullmatch
-from typing import List
-from urllib.parse import quote
-import pyperclip
-import pathlib
-import pyautogui as pg
-import asyncio
-from .Core import core, log, exceptions
-
-pg.FAILSAFE = False
-
-
-async def main():
-    """Check the internet connection."""
-    await core.check_connection()
-
-
-loop = asyncio.get_event_loop()
-loop.run_until_complete(main())
-
-
-async def sendwhatmsg_instantly(
-        phone_no: str,
-        message: str,
-        wait_time: int = 15,
-        tab_close: bool = True,
-        close_time: int = 3
-) -> None:
-    """Send a WhatsApp message instantly.
-    
-    This function opens a new tab in the default web browser, navigates to the WhatsApp web page, and sends a message to the specified phone number.
-    
-    Parameters:
-    message: The message to be sent.
-    phone_no: The phone number to send the message to.
-    wait_time: The time to wait before sending the message (in seconds).
-    tab_close: A flag indicating whether to close the tab after sending the message.
-    close_time: The time to wait before closing the tab (in seconds).
-    
-    Returns:
-    None.
-    """
-    print(phone_no)
-    print(await core.check_number(number=phone_no))
-    if not await core.check_number(number=phone_no):
-        raise exceptions.CountryCodeException("Country Code Missing in Phone Number!")
-    phone_no = phone_no.replace(" ", "")
-    print(phone_no)
-    if not fullmatch(r"^\+?[0-9]{2,4}\s?[0-9]{9,15}", phone_no):
-        raise exceptions.InvalidPhoneNumber("Invalid Phone Number.")
-    phone_no = phone_no.replace(" ", "")
-    web.open(f"https://web.whatsapp.com/send?phone={phone_no}&text={quote(message)}", new=0)
-    await asyncio.sleep(wait_time)
-    pg.press('enter')
-    await asyncio.sleep(close_time)
-    if tab_close:
-        await core.close_tab(wait_time=close_time)
-
-
-async def sendwhatmsg(
-        phone_no: str = None,
-        message: str = None,
-        time_hour: int = None,
-        time_min: int = None,
-        wait_time: int = 15,
-        tab_close: bool = False,
-        close_time: int = 3,
-) -> None:
-    """Send a WhatsApp message at a certain time.
-    
-    This function schedules the sending of a WhatsApp message to a specified phone number at a specified time.
-    
-    Parameters:
-    phone_no: The phone number to send the message to.
-    message: The message to be sent.
-    time_hour: The hour at which to send the message (in 24-hour format).
-    time_min: The minute at which to send the message.
-    wait_time: The time to wait before sending the message (in seconds).
-    tab_close: A flag indicating whether to close the tab after sending the message.
-    close_time: The time to wait before closing the tab (in seconds).
-    
-    Returns:
-    None.
-    """
-    if not core.check_number(number=phone_no):
-        raise exceptions.CountryCodeException("Country Code Missing in Phone Number!")
-
-    phone_no = phone_no.replace(" ", "")
-    if not fullmatch(r"^\+?[0-9]{2,4}\s?[0-9]{9,15}", phone_no):
-        raise exceptions.InvalidPhoneNumber("Invalid Phone Number.")
-
-    if time_hour not in range(25) or time_min not in range(60):
-        raise Warning("Invalid Time Format!")
-
-    current_time = time.localtime()
-    left_time = datetime.strptime(
-        f"{time_hour}:{time_min}:0", "%H:%M:%S"
-    ) - datetime.strptime(
-        f"{current_time.tm_hour}:{current_time.tm_min}:{current_time.tm_sec}",
-        "%H:%M:%S",
-    )
-
-    if left_time.seconds < wait_time:
-        raise exceptions.CallTimeException(
-            "Call Time must be Greater than Wait Time as WhatsApp Web takes some Time to Load!"
-        )
-
-    sleep_time = left_time.seconds - wait_time
-    print(
-        f"In {sleep_time} Seconds WhatsApp will open and after {wait_time} Seconds Message will be Delivered!"
-    )
-    await asyncio.sleep(sleep_time)
-    await sendwhatmsg_instantly(message, phone_no)
-    if tab_close:
-        await core.close_tab(wait_time=close_time)
-
-
-async def sendwhatmsg_to_group(
-        group_id: str,
-        message: str,
-        time_hour: int,
-        time_min: int,
-        wait_time: int = 15,
-        tab_close: bool = False,
-        close_time: int = 3,
-) -> None:
-    """Send a WhatsApp message to a group at a certain time.
-    
-    This function schedules the sending of a WhatsApp message to a specified group at a specified time.
-    
-    Parameters:
-    group_id: The ID of the group to send the message to.
-    message: The message to be sent.
-    time_hour: The hour at which to send the message (in 24-hour format).
-    time_min: The minute at which to send the message.
-    wait_time: The time to wait before sending the message (in seconds).
-    tab_close: A flag indicating whether to close the tab after sending the message.
-    close_time: The time to wait before closing the tab (in seconds).
-    
-    Returns:
-    None.
-    """
-    if time_hour not in range(25) or time_min not in range(60):
-        raise Warning("Invalid Time Format!")
-
-    current_time = time.localtime()
-    left_time = datetime.strptime(
-        f"{time_hour}:{time_min}:0", "%H:%M:%S"
-    ) - datetime.strptime(
-        f"{current_time.tm_hour}:{current_time.tm_min}:{current_time.tm_sec}",
-        "%H:%M:%S",
-    )
-
-    if left_time.seconds < wait_time:
-        raise exceptions.CallTimeException(
-            "Call Time must be Greater than Wait Time as WhatsApp Web takes some Time to Load!"
-        )
-
-    sleep_time = left_time.seconds - wait_time
-    print(
-        f"In {sleep_time} Seconds WhatsApp will open and after {wait_time} Seconds Message will be Delivered!"
-    )
-    await asyncio.sleep(sleep_time)
-    await sendwhatmsg_instantly(group_id, message)
-    await log.log_message(_time=current_time, receiver=group_id, message=message)
-    if tab_close:
-        await core.close_tab(wait_time=close_time)
-
-
-async def sendwhatmsg_to_group_instantly(
-        group_id: str,
-        message: str,
-        wait_time: int = 15,
-        tab_close: bool = False,
-        close_time: int = 3,
-) -> None:
-    """Send a WhatsApp message to a group instantly.
-    
-    This function opens the WhatsApp Web page in a new tab and sends a message to the specified group.
-    
-    Parameters:
-    group_id: The ID of the group to send the message to.
-    message: The message to be sent.
-    wait_time: The time to wait before sending the message (in seconds).
-    tab_close: A flag indicating whether to close the tab after sending the message.
-    close_time: The time to wait before closing the tab (in seconds).
-    
-    Returns:
-    None.
-    """
-    current_time = time.localtime()
-    await asyncio.sleep(4)
-    await sendwhatmsg_instantly(group_id, message)
-    await log.log_message(_time=current_time, receiver=group_id, message=message)
-
-    if tab_close:
-        await core.close_tab(wait_time=close_time)
-
-
-async def sendwhatsmsg_to_all(
-        phone_nos: List[str],
-        message: str,
-        time_hour: int,
-        time_min: int,
-        wait_time: int = 15,
-        tab_close: bool = False,
-        close_time: int = 3,
-) -> None:
-    """Send a WhatsApp message to a list of phone numbers at a certain time.
-    
-    This function schedules the sending of a WhatsApp message to a list of specified phone numbers at a specified time.
-    
-    Parameters:
-    phone_nos: The list of phone numbers to send the message to.
-    message: The message to be sent.
-    time_hour: The hour at which to send the message (in 24-hour format).
-    time_min: The minute at which to send the message.
-    wait_time: The time to wait before sending the message (in seconds).
-    tab_close: A flag indicating whether to close the tab after sending the message.
-    close_time: The time to wait before closing the tab (in seconds).
-    
-    Returns:
-    None.
-    """
-    for phone_n in phone_nos:
-        await sendwhatmsg(
-            phone_n, message, time_hour, time_min, wait_time, tab_close, close_time
-        )
-
-
-async def sendimg_or_video_immediately(
-        phone_no: str,
-        path: typing.Union[str, List[str]],
-        message: str = None,
-        wait_time: int = 15,
-        tab_close: bool = False,
-        close_time: int = 3,
-) -> None:
-    """Send an image or video file via WhatsApp instantly.
-    
-    This function opens a new tab in the default web browser, navigates to the WhatsApp web page, and sends an image or video file to the specified phone number.
-    
-    Parameters:
-    phone_no: The phone number to send the file to.
-    path: The file path of the image or video file to be sent.
-    wait_time: The time to wait before sending the file (in seconds).
-    tab_close: A flag indicating whether to close the tab after sending the file.
-    close_time: The time to wait before closing the tab (in seconds).
-    
-    Returns:
-    None.
-    """
-
-    if not await core.check_number(number=phone_no):
-        raise exceptions.CountryCodeException("Country Code Missing in Phone Number!")
-
-    phone_no = phone_no.replace(" ", "")
-    if not fullmatch(r"^\+?[0-9]{2,4}\s?[0-9]{9,15}", phone_no):
-        raise exceptions.InvalidPhoneNumber("Invalid Phone Number.")
-
-    web.open(f"https://web.whatsapp.com/send?phone={phone_no}")
-    time.sleep(wait_time)
-    await core.find_link()
-    time.sleep(1)
-    await core.find_photo_or_video()
-    if isinstance(path, str):
-        path = pathlib.Path(path)
-        pyperclip.copy(str(path.resolve()))
-        print("Copied")
-    else:
-        str_n = []
-        for paths in path:
-            path_a = str(pathlib.Path(paths).resolve())
-            str_n.append(f'"{path_a}"')
-
-        print(" ".join(str_n))
-        pyperclip.copy(" ".join(str_n))
-    time.sleep(1)
-    pg.hotkey('ctrl', 'v')
-    time.sleep(1)
-    pg.press('enter')
-    time.sleep(1)
-    if message is not None:
-        pyperclip.copy(message)
-        pg.hotkey('ctrl', 'v')
-    time.sleep(3)
-    pg.hotkey('enter')
-    if tab_close:
-        await core.close_tab(wait_time=close_time)
-
-
-async def sendwhatsdoc_immediately(
-        phone_no: str,
-        path: str,
-        message: str = None,
-        wait_time: int = 15,
-        tab_close: bool = True,
-        close_time: int = 3,
-) -> None:
-    """Send a WhatsApp document instantly.
-
-This function opens a new tab in the default web browser, navigates to the WhatsApp web page, and sends a document to the specified phone number.
-
-Parameters:
-phone_no: The phone number to send the document to.
-path: The file path of the document to be sent.
-wait_time: The time to wait before sending the document (in seconds).
-tab_close: A flag indicating whether to close the tab after sending the document.
-close_time: The time to wait before closing the tab (in seconds).
-
-Returns:
-None.
-"""
-
-    if not await core.check_number(number=phone_no):
-        raise exceptions.CountryCodeException("Country Code Missing in Phone Number!")
-
-    phone_no = phone_no.replace(" ", "")
-    if not fullmatch(r"^\+?[0-9]{2,4}\s?[0-9]{9,15}", phone_no):
-        raise exceptions.InvalidPhoneNumber("Invalid Phone Number.")
-
-    web.open(f"https://web.whatsapp.com/send?phone={phone_no}")
-    time.sleep(wait_time)
-    await core.find_link()
-    time.sleep(1)
-    await core.find_document()
-    if type(path) == str:
-        path = pathlib.Path(path)
-        pyperclip.copy(str(path.resolve()))
-        print("Copied")
-    else:
-        strn = []
-        for paths in path:
-            path_a = str(pathlib.Path(paths).resolve())
-            strn.append(f'"{path_a}"')
-
-        print(" ".join(strn))
-        pyperclip.copy(" ".join(strn))
-
-    time.sleep(1)
-    pg.hotkey('ctrl', 'v')
-    time.sleep(1)
-    pg.press('enter')
-    time.sleep(1)
-    if message is not None:
-        pyperclip.copy(message)
-    time.sleep(5)
-    pg.press('enter')
-    if tab_close:
-        await core.close_tab(wait_time=close_time)
-
-
-def open_web() -> bool:
-    """Opens WhatsApp Web """
-
-    try:
-        web.open("https://web.whatsapp.com")
-    except web.Error:
-        return False
-    else:
-        return True
+import time
+import typing
+import webbrowser as web
+from datetime import datetime
+from re import fullmatch
+from typing import List
+from urllib.parse import quote
+import pyperclip
+import pathlib
+import pyautogui as pg
+import asyncio
+from .Core import core, log, exceptions
+
+pg.FAILSAFE = False
+
+
+async def main():
+    """Check the internet connection."""
+    await core.check_connection()
+
+
+loop = asyncio.get_event_loop()
+loop.run_until_complete(main())
+
+
+async def sendwhatmsg_instantly(
+        phone_no: str,
+        message: str,
+        wait_time: int = 15,
+        tab_close: bool = True,
+        close_time: int = 3
+) -> None:
+    """Send a WhatsApp message instantly.
+    
+    This function opens a new tab in the default web browser, navigates to the WhatsApp web page, and sends a message to the specified phone number.
+    
+    Parameters:
+    message: The message to be sent.
+    phone_no: The phone number to send the message to.
+    wait_time: The time to wait before sending the message (in seconds).
+    tab_close: A flag indicating whether to close the tab after sending the message.
+    close_time: The time to wait before closing the tab (in seconds).
+    
+    Returns:
+    None.
+    """
+    print(phone_no)
+    print(await core.check_number(number=phone_no))
+    if not await core.check_number(number=phone_no):
+        raise exceptions.CountryCodeException("Country Code Missing in Phone Number!")
+    phone_no = phone_no.replace(" ", "")
+    print(phone_no)
+    if not fullmatch(r"^\+?[0-9]{2,4}\s?[0-9]{9,15}", phone_no):
+        raise exceptions.InvalidPhoneNumber("Invalid Phone Number.")
+    phone_no = phone_no.replace(" ", "")
+    web.open(f"https://web.whatsapp.com/send?phone={phone_no}&text={quote(message)}", new=0)
+    await asyncio.sleep(wait_time)
+    pg.press('enter')
+    await asyncio.sleep(close_time)
+    if tab_close:
+        await core.close_tab(wait_time=close_time)
+
+
+async def sendwhatmsg(
+        phone_no: str = None,
+        message: str = None,
+        time_hour: int = None,
+        time_min: int = None,
+        wait_time: int = 15,
+        tab_close: bool = False,
+        close_time: int = 3,
+) -> None:
+    """Send a WhatsApp message at a certain time.
+    
+    This function schedules the sending of a WhatsApp message to a specified phone number at a specified time.
+    
+    Parameters:
+    phone_no: The phone number to send the message to.
+    message: The message to be sent.
+    time_hour: The hour at which to send the message (in 24-hour format).
+    time_min: The minute at which to send the message.
+    wait_time: The time to wait before sending the message (in seconds).
+    tab_close: A flag indicating whether to close the tab after sending the message.
+    close_time: The time to wait before closing the tab (in seconds).
+    
+    Returns:
+    None.
+    """
+    if not core.check_number(number=phone_no):
+        raise exceptions.CountryCodeException("Country Code Missing in Phone Number!")
+
+    phone_no = phone_no.replace(" ", "")
+    if not fullmatch(r"^\+?[0-9]{2,4}\s?[0-9]{9,15}", phone_no):
+        raise exceptions.InvalidPhoneNumber("Invalid Phone Number.")
+
+    if time_hour not in range(25) or time_min not in range(60):
+        raise Warning("Invalid Time Format!")
+
+    current_time = time.localtime()
+    left_time = datetime.strptime(
+        f"{time_hour}:{time_min}:0", "%H:%M:%S"
+    ) - datetime.strptime(
+        f"{current_time.tm_hour}:{current_time.tm_min}:{current_time.tm_sec}",
+        "%H:%M:%S",
+    )
+
+    if left_time.seconds < wait_time:
+        raise exceptions.CallTimeException(
+            "Call Time must be Greater than Wait Time as WhatsApp Web takes some Time to Load!"
+        )
+
+    sleep_time = left_time.seconds - wait_time
+    print(
+        f"In {sleep_time} Seconds WhatsApp will open and after {wait_time} Seconds Message will be Delivered!"
+    )
+    await asyncio.sleep(sleep_time)
+    await sendwhatmsg_instantly(message, phone_no)
+    if tab_close:
+        await core.close_tab(wait_time=close_time)
+
+
+async def sendwhatmsg_to_group(
+        group_id: str,
+        message: str,
+        time_hour: int,
+        time_min: int,
+        wait_time: int = 15,
+        tab_close: bool = False,
+        close_time: int = 3,
+) -> None:
+    """Send a WhatsApp message to a group at a certain time.
+    
+    This function schedules the sending of a WhatsApp message to a specified group at a specified time.
+    
+    Parameters:
+    group_id: The ID of the group to send the message to.
+    message: The message to be sent.
+    time_hour: The hour at which to send the message (in 24-hour format).
+    time_min: The minute at which to send the message.
+    wait_time: The time to wait before sending the message (in seconds).
+    tab_close: A flag indicating whether to close the tab after sending the message.
+    close_time: The time to wait before closing the tab (in seconds).
+    
+    Returns:
+    None.
+    """
+    if time_hour not in range(25) or time_min not in range(60):
+        raise Warning("Invalid Time Format!")
+
+    current_time = time.localtime()
+    left_time = datetime.strptime(
+        f"{time_hour}:{time_min}:0", "%H:%M:%S"
+    ) - datetime.strptime(
+        f"{current_time.tm_hour}:{current_time.tm_min}:{current_time.tm_sec}",
+        "%H:%M:%S",
+    )
+
+    if left_time.seconds < wait_time:
+        raise exceptions.CallTimeException(
+            "Call Time must be Greater than Wait Time as WhatsApp Web takes some Time to Load!"
+        )
+
+    sleep_time = left_time.seconds - wait_time
+    print(
+        f"In {sleep_time} Seconds WhatsApp will open and after {wait_time} Seconds Message will be Delivered!"
+    )
+    await asyncio.sleep(sleep_time)
+    await sendwhatmsg_to_group_instantly(group_id, message, wait_time, tab_close, close_time)
+    await log.log_message(_time=current_time, receiver=group_id, message=message)
+    if tab_close:
+        await core.close_tab(wait_time=close_time)
+
+
+async def sendwhatmsg_to_group_instantly(
+        group_id: str,
+        message: str,
+        wait_time: int = 15,
+        tab_close: bool = False,
+        close_time: int = 3,
+) -> None:
+    """Send a WhatsApp message to a group instantly.
+    
+    This function opens the WhatsApp Web page in a new tab and sends a message to the specified group.
+    
+    Parameters:
+    group_id: The ID of the group to send the message to.
+    message: The message to be sent.
+    wait_time: The time to wait before sending the message (in seconds).
+    tab_close: A flag indicating whether to close the tab after sending the message.
+    close_time: The time to wait before closing the tab (in seconds).
+    
+    Returns:
+    None.
+    """
+    current_time = time.localtime()
+    await asyncio.sleep(4)
+    web.open(f"https://web.whatsapp.com/accept?code={group_id}", new=0)
+    await asyncio.sleep(wait_time)
+    pyperclip.copy(message)
+    pg.hotkey('ctrl','v')
+    await asyncio.sleep(1)
+    pg.press('enter')
+    await asyncio.sleep(close_time)
+    if tab_close:
+        await core.close_tab(wait_time=close_time)
+
+    if tab_close:
+        await core.close_tab(wait_time=close_time)
+
+
+async def sendwhatsmsg_to_all(
+        phone_nos: List[str],
+        message: str,
+        time_hour: int,
+        time_min: int,
+        wait_time: int = 15,
+        tab_close: bool = False,
+        close_time: int = 3,
+) -> None:
+    """Send a WhatsApp message to a list of phone numbers at a certain time.
+    
+    This function schedules the sending of a WhatsApp message to a list of specified phone numbers at a specified time.
+    
+    Parameters:
+    phone_nos: The list of phone numbers to send the message to.
+    message: The message to be sent.
+    time_hour: The hour at which to send the message (in 24-hour format).
+    time_min: The minute at which to send the message.
+    wait_time: The time to wait before sending the message (in seconds).
+    tab_close: A flag indicating whether to close the tab after sending the message.
+    close_time: The time to wait before closing the tab (in seconds).
+    
+    Returns:
+    None.
+    """
+    for phone_n in phone_nos:
+        await sendwhatmsg(
+            phone_n, message, time_hour, time_min, wait_time, tab_close, close_time
+        )
+
+
+async def sendimg_or_video_immediately(
+        phone_no: str,
+        path: typing.Union[str, List[str]],
+        message: str = None,
+        group_id:str = None,
+        wait_time: int = 15,
+        tab_close: bool = False,
+        close_time: int = 3,
+) -> None:
+    """Send an image or video file via WhatsApp instantly.
+    
+    This function opens a new tab in the default web browser, navigates to the WhatsApp web page, and sends an image or video file to the specified phone number.
+    
+    Parameters:
+    phone_no: The phone number to send the file to.
+    path: The file path of the image or video file to be sent.
+    wait_time: The time to wait before sending the file (in seconds).
+    tab_close: A flag indicating whether to close the tab after sending the file.
+    close_time: The time to wait before closing the tab (in seconds).
+    
+    Returns:
+    None.
+    """
+
+    if not await core.check_number(number=phone_no):
+        raise exceptions.CountryCodeException("Country Code Missing in Phone Number!")
+    if(phone_no is not None):
+        phone_no = phone_no.replace(" ", "")
+        if not fullmatch(r"^\+?[0-9]{2,4}\s?[0-9]{9,15}", phone_no):
+            raise exceptions.InvalidPhoneNumber("Invalid Phone Number.")
+        web.open(f"https://web.whatsapp.com/send?phone={phone_no}")
+    elif(group_id is not None):
+        web.open(f"https://web.whatsapp.com/accept?code={group_id}")
+    time.sleep(wait_time)
+    await core.find_link()
+    time.sleep(1)
+    await core.find_photo_or_video()
+    if isinstance(path, str):
+        path = pathlib.Path(path)
+        pyperclip.copy(str(path.resolve()))
+        print("Copied")
+    else:
+        str_n = []
+        for paths in path:
+            path_a = str(pathlib.Path(paths).resolve())
+            str_n.append(f'"{path_a}"')
+
+        print(" ".join(str_n))
+        pyperclip.copy(" ".join(str_n))
+    time.sleep(1)
+    pg.hotkey('ctrl', 'v')
+    time.sleep(1)
+    pg.press('enter')
+    time.sleep(1)
+    if message is not None:
+        pyperclip.copy(message)
+        pg.hotkey('ctrl', 'v')
+    time.sleep(3)
+    pg.hotkey('enter')
+    if tab_close:
+        await core.close_tab(wait_time=close_time)
+
+
+async def sendwhatsdoc_immediately(
+        phone_no: str=None,
+        path: str = None,
+        group_id:str = None,
+        message: str = None,
+        wait_time: int = 15,
+        tab_close: bool = True,
+        close_time: int = 3,
+) -> None:
+    """Send a WhatsApp document instantly.
+
+This function opens a new tab in the default web browser, navigates to the WhatsApp web page, and sends a document to the specified phone number.
+
+Parameters:
+phone_no: The phone number to send the document to.
+path: The file path of the document to be sent.
+wait_time: The time to wait before sending the document (in seconds).
+tab_close: A flag indicating whether to close the tab after sending the document.
+close_time: The time to wait before closing the tab (in seconds).
+
+Returns:
+None.
+"""
+
+    if not await core.check_number(number=phone_no):
+        raise exceptions.CountryCodeException("Country Code Missing in Phone Number!")
+    if(phone_no is not None):
+        phone_no = phone_no.replace(" ", "")
+        if not fullmatch(r"^\+?[0-9]{2,4}\s?[0-9]{9,15}", phone_no):
+            raise exceptions.InvalidPhoneNumber("Invalid Phone Number.")
+        web.open(f"https://web.whatsapp.com/send?phone={phone_no}")
+    elif(group_id is not None):
+        web.open(f"https://web.whatsapp.com/accept?code={group_id}")
+    time.sleep(wait_time)
+    await core.find_link()
+    time.sleep(1)
+    await core.find_document()
+    if type(path) == str:
+        path = pathlib.Path(path)
+        pyperclip.copy(str(path.resolve()))
+        print("Copied")
+    else:
+        strn = []
+        for paths in path:
+            path_a = str(pathlib.Path(paths).resolve())
+            strn.append(f'"{path_a}"')
+
+        print(" ".join(strn))
+        pyperclip.copy(" ".join(strn))
+
+    time.sleep(1)
+    pg.hotkey('ctrl', 'v')
+    time.sleep(1)
+    pg.press('enter')
+    time.sleep(1)
+    if message is not None:
+        pyperclip.copy(message)
+    time.sleep(5)
+    pg.press('enter')
+    if tab_close:
+        await core.close_tab(wait_time=close_time)
+
+
+def open_web() -> bool:
+    """Opens WhatsApp Web """
+
+    try:
+        web.open("https://web.whatsapp.com")
+    except web.Error:
+        return False
+    else:
+        return True
```

### Comparing `AsyncPywhatKit-2.2.6/AsyncPywhatKit.egg-info/PKG-INFO` & `AsyncPywhatKit-2.2.7/AsyncPywhatKit.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,108 +1,108 @@
-Metadata-Version: 2.1
-Name: AsyncPywhatKit
-Version: 2.2.6
-Summary: AsyncPywhatKit is a Simple and Powerful WhatsApp Automation Library with many useful Features
-Home-page: https://github.com/SigireddyBalasai/AsyncPywhatKit
-Download-URL: https://github.com/SigireddyBalasai/AsyncPywhatKit/archive/refs/tags/1.0.tar.gz
-Author: SigireddyBalasai
-Author-email: sigireddybalasai@gmail.com
-License: MIT
-Keywords: sendwhatmsg,info,playonyt,search,watch_tutorial,async pywhatkit
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
-![image](https://media.discordapp.net/attachments/842794167134453820/882227960613048350/unknown.png?width=1440&height=420)
-
-[![image](https://flat.badgen.net/github/stars/SigireddyBalasai/AsyncPywhatKit)](https://github.com/SigireddyBalasai/AsyncPywhatKit/stargazers)
-[![image](https://flat.badgen.net/github/forks/SigireddyBalasai/AsyncPywhatKit)](https://github.com/SigireddyBalasai/AsyncPywhatKit/network/members)
-[![image](https://flat.badgen.net/github/open-issues/SigireddyBalasai/AsyncPywhatKit)](https://github.com/SigireddyBalasai/AsyncPywhatKit/issues)
-[![image](https://flat.badgen.net/github/open-prs/SigireddyBalasai/AsyncPywhatKit)](https://github.com/SigireddyBalasai/AsyncPywhatKit/pulls)
-[![image](https://flat.badgen.net/github/commits/SigireddyBalasai/AsyncPywhatKit)](https://github.com/SigireddyBalasai/AsyncPywhatKit/commits/master)
-[![image](https://flat.badgen.net/github/license/SigireddyBalasai/AsyncPywhatKit)](https://github.com/SigireddyBalasai/AsyncPywhatKit/LICENCE)
-[![image](https://flat.badgen.net/github/contributors/SigireddyBalasai/AsyncPywhatKit)](https://github.com/SigireddyBalasai/AsyncPywhatKit/graphs/contributors)
-[![image](https://flat.badgen.net/github/release/SigireddyBalasai/AsyncPywhatKit)](https://github.com/SigireddyBalasai/AsyncPywhatKit/releases)
-![image](https://img.shields.io/github/languages/count/SigireddyBalasai/AsyncPywhatKit)
-![image](https://img.shields.io/github/languages/top/SigireddyBalasai/AsyncPywhatKit)
-![image](https://img.shields.io/librariesio/release/pypi/AsyncPywhatKit)
-![image](https://img.shields.io/github/repo-size/SigireddyBalasai/AsyncPywhatKit)
-[![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FSigireddyBalasai%2FAsyncpywhatkit&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false)](https://hits.seeyoufarm.com)
-<a href="https://scan.coverity.com/projects/sigireddybalasai-asyncpywhatkit">
-  <img alt="Coverity Scan Build Status"
-       src="https://img.shields.io/coverity/scan/27211.svg"/>
-</a>
-<!-- ![logo](https://github.com/Ankit404butfound/PyWhatKit/raw/master/Images/logo.png?raw=true) -->
-
-
-[AsyncPywhatKit](https://pypi.org/project/AsyncPywhatKit/) is a Python library with various helpful features. It's easy-to-use and does not require you to do any additional setup. Currently, it is one of the most popular library for WhatsApp and YouTube automation. New updates are released frequently with new features and bug fixes.
-
-# Links
-
-- **Join our discord server - https://discord.gg/NDXdB6tNwa**
-- **Documentation - [Wiki](https://github.com/SigireddyBalasai/AsyncPywhatKit/wiki/)**
-
-## Installation and Supported Versions
-
-AsyncPywhatKit is available on PyPi:
-
-```bash
-python3 -m pip install AsyncPywhatKit
-```
-
-```bash
-pip3 install AsyncPywhatKit
-```
-
-PyWhatKit officially supports Python 3.8+.
-
-## Cloning the Repository
-
-```bash
-git clone https://github.com/SigireddyBalasai/AsyncPywhatKit
-```
-```py
-import asyncio
-import AsyncPywhatKit
-
-
-async def main():
-    # Send a WhatsApp Message to a Contact at 1:30 PM
-    await AsyncPywhatKit.sendwhatmsg("+910123456789", "Hi", 13, 30)
-
-    # Same as above but Closes the Tab in 2 Seconds after Sending the Message
-    await AsyncPywhatKit.src.sendwhatmsg("+910123456789", "Hi", 13, 30, 15, True, 2)
-
-    # Send an Image to a Group with the Caption as Hello
-    await AsyncPywhatKit.src.sendwhats_image("AB123CDEFGHijklmn", "Images/Hello.png", "Hello")
-
-    # Send an Image to a Contact with the no Caption
-    await AsyncPywhatKit.src.sendwhats_image("+910123456789", "Images/Hello.png")
-
-    # Send a WhatsApp Message to a Group at 12:00 AM
-    await AsyncPywhatKit.src.sendwhatmsg_to_group("AB123CDEFGHijklmn", "Hey All!", 0, 0)
-
-    # Send a WhatsApp Message to a Group instantly
-    await AsyncPywhatKit.src.sendwhatmsg_to_group_instantly("AB123CDEFGHijklmn", "Hey All!")
-
-
-asyncio.run(main())
-```
-
-For more Examples and Functions, have a look at the [Wiki](https://github.com/SigireddyBalasai/AsyncPywhatKit/wiki/).
-
-## Contributing
-
-Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
-Be sure to read the [Guidelines](https://github.com/SigireddyBalasai/AsyncPywhatKit/blob/main/CONTRIBUTING.md) before Contributing.
-
-## License
-
-Apache license 2.0
-For more information see [this](https://github.com/SigireddyBalasai/AsyncPywhatKit/blob/main/LICENSE)
+Metadata-Version: 2.1
+Name: AsyncPywhatKit
+Version: 2.2.7
+Summary: AsyncPywhatKit is a Simple and Powerful WhatsApp Automation Library with many useful Features
+Home-page: https://github.com/SigireddyBalasai/AsyncPywhatKit
+Download-URL: https://github.com/SigireddyBalasai/AsyncPywhatKit/archive/refs/tags/1.0.tar.gz
+Author: SigireddyBalasai
+Author-email: sigireddybalasai@gmail.com
+License: MIT
+Keywords: sendwhatmsg,info,playonyt,search,watch_tutorial,async pywhatkit
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+![image](https://media.discordapp.net/attachments/842794167134453820/882227960613048350/unknown.png?width=1440&height=420)
+
+[![image](https://flat.badgen.net/github/stars/SigireddyBalasai/AsyncPywhatKit)](https://github.com/SigireddyBalasai/AsyncPywhatKit/stargazers)
+[![image](https://flat.badgen.net/github/forks/SigireddyBalasai/AsyncPywhatKit)](https://github.com/SigireddyBalasai/AsyncPywhatKit/network/members)
+[![image](https://flat.badgen.net/github/open-issues/SigireddyBalasai/AsyncPywhatKit)](https://github.com/SigireddyBalasai/AsyncPywhatKit/issues)
+[![image](https://flat.badgen.net/github/open-prs/SigireddyBalasai/AsyncPywhatKit)](https://github.com/SigireddyBalasai/AsyncPywhatKit/pulls)
+[![image](https://flat.badgen.net/github/commits/SigireddyBalasai/AsyncPywhatKit)](https://github.com/SigireddyBalasai/AsyncPywhatKit/commits/master)
+[![image](https://flat.badgen.net/github/license/SigireddyBalasai/AsyncPywhatKit)](https://github.com/SigireddyBalasai/AsyncPywhatKit/LICENCE)
+[![image](https://flat.badgen.net/github/contributors/SigireddyBalasai/AsyncPywhatKit)](https://github.com/SigireddyBalasai/AsyncPywhatKit/graphs/contributors)
+[![image](https://flat.badgen.net/github/release/SigireddyBalasai/AsyncPywhatKit)](https://github.com/SigireddyBalasai/AsyncPywhatKit/releases)
+![image](https://img.shields.io/github/languages/count/SigireddyBalasai/AsyncPywhatKit)
+![image](https://img.shields.io/github/languages/top/SigireddyBalasai/AsyncPywhatKit)
+![image](https://img.shields.io/librariesio/release/pypi/AsyncPywhatKit)
+![image](https://img.shields.io/github/repo-size/SigireddyBalasai/AsyncPywhatKit)
+[![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FSigireddyBalasai%2FAsyncpywhatkit&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false)](https://hits.seeyoufarm.com)
+<a href="https://scan.coverity.com/projects/sigireddybalasai-asyncpywhatkit">
+  <img alt="Coverity Scan Build Status"
+       src="https://img.shields.io/coverity/scan/27211.svg"/>
+</a>
+<!-- ![logo](https://github.com/Ankit404butfound/PyWhatKit/raw/master/Images/logo.png?raw=true) -->
+
+
+[AsyncPywhatKit](https://pypi.org/project/AsyncPywhatKit/) is a Python library with various helpful features. It's easy-to-use and does not require you to do any additional setup. Currently, it is one of the most popular library for WhatsApp and YouTube automation. New updates are released frequently with new features and bug fixes.
+
+# Links
+
+- **Join our discord server - https://discord.gg/NDXdB6tNwa**
+- **Documentation - [Wiki](https://github.com/SigireddyBalasai/AsyncPywhatKit/wiki/)**
+
+## Installation and Supported Versions
+
+AsyncPywhatKit is available on PyPi:
+
+```bash
+python3 -m pip install AsyncPywhatKit
+```
+
+```bash
+pip3 install AsyncPywhatKit
+```
+
+PyWhatKit officially supports Python 3.8+.
+
+## Cloning the Repository
+
+```bash
+git clone https://github.com/SigireddyBalasai/AsyncPywhatKit
+```
+```py
+import asyncio
+import AsyncPywhatKit
+
+
+async def main():
+    # Send a WhatsApp Message to a Contact at 1:30 PM
+    await AsyncPywhatKit.sendwhatmsg("+910123456789", "Hi", 13, 30)
+
+    # Same as above but Closes the Tab in 2 Seconds after Sending the Message
+    await AsyncPywhatKit.src.sendwhatmsg("+910123456789", "Hi", 13, 30, 15, True, 2)
+
+    # Send an Image to a Group with the Caption as Hello
+    await AsyncPywhatKit.src.sendwhats_image("AB123CDEFGHijklmn", "Images/Hello.png", "Hello")
+
+    # Send an Image to a Contact with the no Caption
+    await AsyncPywhatKit.src.sendwhats_image("+910123456789", "Images/Hello.png")
+
+    # Send a WhatsApp Message to a Group at 12:00 AM
+    await AsyncPywhatKit.src.sendwhatmsg_to_group("AB123CDEFGHijklmn", "Hey All!", 0, 0)
+
+    # Send a WhatsApp Message to a Group instantly
+    await AsyncPywhatKit.src.sendwhatmsg_to_group_instantly("AB123CDEFGHijklmn", "Hey All!")
+
+
+asyncio.run(main())
+```
+
+For more Examples and Functions, have a look at the [Wiki](https://github.com/SigireddyBalasai/AsyncPywhatKit/wiki/).
+
+## Contributing
+
+Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
+Be sure to read the [Guidelines](https://github.com/SigireddyBalasai/AsyncPywhatKit/blob/main/CONTRIBUTING.md) before Contributing.
+
+## License
+
+Apache license 2.0
+For more information see [this](https://github.com/SigireddyBalasai/AsyncPywhatKit/blob/main/LICENSE)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: AsyncPywhatKit Version: 2.2.6 Summary:
+Metadata-Version: 2.1 Name: AsyncPywhatKit Version: 2.2.7 Summary:
 AsyncPywhatKit is a Simple and Powerful WhatsApp Automation Library with many
 useful Features Home-page: https://github.com/SigireddyBalasai/AsyncPywhatKit
 Download-URL: https://github.com/SigireddyBalasai/AsyncPywhatKit/archive/refs/
 tags/1.0.tar.gz Author: SigireddyBalasai Author-email:
 sigireddybalasai@gmail.com License: MIT Keywords:
 sendwhatmsg,info,playonyt,search,watch_tutorial,async pywhatkit Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
```

### Comparing `AsyncPywhatKit-2.2.6/LICENSE.md` & `AsyncPywhatKit-2.2.7/LICENSE.md`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [2021] [SigireddyBalasai]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [2021] [SigireddyBalasai]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `AsyncPywhatKit-2.2.6/PKG-INFO` & `AsyncPywhatKit-2.2.7/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,108 +1,108 @@
-Metadata-Version: 2.1
-Name: AsyncPywhatKit
-Version: 2.2.6
-Summary: AsyncPywhatKit is a Simple and Powerful WhatsApp Automation Library with many useful Features
-Home-page: https://github.com/SigireddyBalasai/AsyncPywhatKit
-Download-URL: https://github.com/SigireddyBalasai/AsyncPywhatKit/archive/refs/tags/1.0.tar.gz
-Author: SigireddyBalasai
-Author-email: sigireddybalasai@gmail.com
-License: MIT
-Keywords: sendwhatmsg,info,playonyt,search,watch_tutorial,async pywhatkit
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
-![image](https://media.discordapp.net/attachments/842794167134453820/882227960613048350/unknown.png?width=1440&height=420)
-
-[![image](https://flat.badgen.net/github/stars/SigireddyBalasai/AsyncPywhatKit)](https://github.com/SigireddyBalasai/AsyncPywhatKit/stargazers)
-[![image](https://flat.badgen.net/github/forks/SigireddyBalasai/AsyncPywhatKit)](https://github.com/SigireddyBalasai/AsyncPywhatKit/network/members)
-[![image](https://flat.badgen.net/github/open-issues/SigireddyBalasai/AsyncPywhatKit)](https://github.com/SigireddyBalasai/AsyncPywhatKit/issues)
-[![image](https://flat.badgen.net/github/open-prs/SigireddyBalasai/AsyncPywhatKit)](https://github.com/SigireddyBalasai/AsyncPywhatKit/pulls)
-[![image](https://flat.badgen.net/github/commits/SigireddyBalasai/AsyncPywhatKit)](https://github.com/SigireddyBalasai/AsyncPywhatKit/commits/master)
-[![image](https://flat.badgen.net/github/license/SigireddyBalasai/AsyncPywhatKit)](https://github.com/SigireddyBalasai/AsyncPywhatKit/LICENCE)
-[![image](https://flat.badgen.net/github/contributors/SigireddyBalasai/AsyncPywhatKit)](https://github.com/SigireddyBalasai/AsyncPywhatKit/graphs/contributors)
-[![image](https://flat.badgen.net/github/release/SigireddyBalasai/AsyncPywhatKit)](https://github.com/SigireddyBalasai/AsyncPywhatKit/releases)
-![image](https://img.shields.io/github/languages/count/SigireddyBalasai/AsyncPywhatKit)
-![image](https://img.shields.io/github/languages/top/SigireddyBalasai/AsyncPywhatKit)
-![image](https://img.shields.io/librariesio/release/pypi/AsyncPywhatKit)
-![image](https://img.shields.io/github/repo-size/SigireddyBalasai/AsyncPywhatKit)
-[![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FSigireddyBalasai%2FAsyncpywhatkit&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false)](https://hits.seeyoufarm.com)
-<a href="https://scan.coverity.com/projects/sigireddybalasai-asyncpywhatkit">
-  <img alt="Coverity Scan Build Status"
-       src="https://img.shields.io/coverity/scan/27211.svg"/>
-</a>
-<!-- ![logo](https://github.com/Ankit404butfound/PyWhatKit/raw/master/Images/logo.png?raw=true) -->
-
-
-[AsyncPywhatKit](https://pypi.org/project/AsyncPywhatKit/) is a Python library with various helpful features. It's easy-to-use and does not require you to do any additional setup. Currently, it is one of the most popular library for WhatsApp and YouTube automation. New updates are released frequently with new features and bug fixes.
-
-# Links
-
-- **Join our discord server - https://discord.gg/NDXdB6tNwa**
-- **Documentation - [Wiki](https://github.com/SigireddyBalasai/AsyncPywhatKit/wiki/)**
-
-## Installation and Supported Versions
-
-AsyncPywhatKit is available on PyPi:
-
-```bash
-python3 -m pip install AsyncPywhatKit
-```
-
-```bash
-pip3 install AsyncPywhatKit
-```
-
-PyWhatKit officially supports Python 3.8+.
-
-## Cloning the Repository
-
-```bash
-git clone https://github.com/SigireddyBalasai/AsyncPywhatKit
-```
-```py
-import asyncio
-import AsyncPywhatKit
-
-
-async def main():
-    # Send a WhatsApp Message to a Contact at 1:30 PM
-    await AsyncPywhatKit.sendwhatmsg("+910123456789", "Hi", 13, 30)
-
-    # Same as above but Closes the Tab in 2 Seconds after Sending the Message
-    await AsyncPywhatKit.src.sendwhatmsg("+910123456789", "Hi", 13, 30, 15, True, 2)
-
-    # Send an Image to a Group with the Caption as Hello
-    await AsyncPywhatKit.src.sendwhats_image("AB123CDEFGHijklmn", "Images/Hello.png", "Hello")
-
-    # Send an Image to a Contact with the no Caption
-    await AsyncPywhatKit.src.sendwhats_image("+910123456789", "Images/Hello.png")
-
-    # Send a WhatsApp Message to a Group at 12:00 AM
-    await AsyncPywhatKit.src.sendwhatmsg_to_group("AB123CDEFGHijklmn", "Hey All!", 0, 0)
-
-    # Send a WhatsApp Message to a Group instantly
-    await AsyncPywhatKit.src.sendwhatmsg_to_group_instantly("AB123CDEFGHijklmn", "Hey All!")
-
-
-asyncio.run(main())
-```
-
-For more Examples and Functions, have a look at the [Wiki](https://github.com/SigireddyBalasai/AsyncPywhatKit/wiki/).
-
-## Contributing
-
-Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
-Be sure to read the [Guidelines](https://github.com/SigireddyBalasai/AsyncPywhatKit/blob/main/CONTRIBUTING.md) before Contributing.
-
-## License
-
-Apache license 2.0
-For more information see [this](https://github.com/SigireddyBalasai/AsyncPywhatKit/blob/main/LICENSE)
+Metadata-Version: 2.1
+Name: AsyncPywhatKit
+Version: 2.2.7
+Summary: AsyncPywhatKit is a Simple and Powerful WhatsApp Automation Library with many useful Features
+Home-page: https://github.com/SigireddyBalasai/AsyncPywhatKit
+Download-URL: https://github.com/SigireddyBalasai/AsyncPywhatKit/archive/refs/tags/1.0.tar.gz
+Author: SigireddyBalasai
+Author-email: sigireddybalasai@gmail.com
+License: MIT
+Keywords: sendwhatmsg,info,playonyt,search,watch_tutorial,async pywhatkit
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+![image](https://media.discordapp.net/attachments/842794167134453820/882227960613048350/unknown.png?width=1440&height=420)
+
+[![image](https://flat.badgen.net/github/stars/SigireddyBalasai/AsyncPywhatKit)](https://github.com/SigireddyBalasai/AsyncPywhatKit/stargazers)
+[![image](https://flat.badgen.net/github/forks/SigireddyBalasai/AsyncPywhatKit)](https://github.com/SigireddyBalasai/AsyncPywhatKit/network/members)
+[![image](https://flat.badgen.net/github/open-issues/SigireddyBalasai/AsyncPywhatKit)](https://github.com/SigireddyBalasai/AsyncPywhatKit/issues)
+[![image](https://flat.badgen.net/github/open-prs/SigireddyBalasai/AsyncPywhatKit)](https://github.com/SigireddyBalasai/AsyncPywhatKit/pulls)
+[![image](https://flat.badgen.net/github/commits/SigireddyBalasai/AsyncPywhatKit)](https://github.com/SigireddyBalasai/AsyncPywhatKit/commits/master)
+[![image](https://flat.badgen.net/github/license/SigireddyBalasai/AsyncPywhatKit)](https://github.com/SigireddyBalasai/AsyncPywhatKit/LICENCE)
+[![image](https://flat.badgen.net/github/contributors/SigireddyBalasai/AsyncPywhatKit)](https://github.com/SigireddyBalasai/AsyncPywhatKit/graphs/contributors)
+[![image](https://flat.badgen.net/github/release/SigireddyBalasai/AsyncPywhatKit)](https://github.com/SigireddyBalasai/AsyncPywhatKit/releases)
+![image](https://img.shields.io/github/languages/count/SigireddyBalasai/AsyncPywhatKit)
+![image](https://img.shields.io/github/languages/top/SigireddyBalasai/AsyncPywhatKit)
+![image](https://img.shields.io/librariesio/release/pypi/AsyncPywhatKit)
+![image](https://img.shields.io/github/repo-size/SigireddyBalasai/AsyncPywhatKit)
+[![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FSigireddyBalasai%2FAsyncpywhatkit&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false)](https://hits.seeyoufarm.com)
+<a href="https://scan.coverity.com/projects/sigireddybalasai-asyncpywhatkit">
+  <img alt="Coverity Scan Build Status"
+       src="https://img.shields.io/coverity/scan/27211.svg"/>
+</a>
+<!-- ![logo](https://github.com/Ankit404butfound/PyWhatKit/raw/master/Images/logo.png?raw=true) -->
+
+
+[AsyncPywhatKit](https://pypi.org/project/AsyncPywhatKit/) is a Python library with various helpful features. It's easy-to-use and does not require you to do any additional setup. Currently, it is one of the most popular library for WhatsApp and YouTube automation. New updates are released frequently with new features and bug fixes.
+
+# Links
+
+- **Join our discord server - https://discord.gg/NDXdB6tNwa**
+- **Documentation - [Wiki](https://github.com/SigireddyBalasai/AsyncPywhatKit/wiki/)**
+
+## Installation and Supported Versions
+
+AsyncPywhatKit is available on PyPi:
+
+```bash
+python3 -m pip install AsyncPywhatKit
+```
+
+```bash
+pip3 install AsyncPywhatKit
+```
+
+PyWhatKit officially supports Python 3.8+.
+
+## Cloning the Repository
+
+```bash
+git clone https://github.com/SigireddyBalasai/AsyncPywhatKit
+```
+```py
+import asyncio
+import AsyncPywhatKit
+
+
+async def main():
+    # Send a WhatsApp Message to a Contact at 1:30 PM
+    await AsyncPywhatKit.sendwhatmsg("+910123456789", "Hi", 13, 30)
+
+    # Same as above but Closes the Tab in 2 Seconds after Sending the Message
+    await AsyncPywhatKit.src.sendwhatmsg("+910123456789", "Hi", 13, 30, 15, True, 2)
+
+    # Send an Image to a Group with the Caption as Hello
+    await AsyncPywhatKit.src.sendwhats_image("AB123CDEFGHijklmn", "Images/Hello.png", "Hello")
+
+    # Send an Image to a Contact with the no Caption
+    await AsyncPywhatKit.src.sendwhats_image("+910123456789", "Images/Hello.png")
+
+    # Send a WhatsApp Message to a Group at 12:00 AM
+    await AsyncPywhatKit.src.sendwhatmsg_to_group("AB123CDEFGHijklmn", "Hey All!", 0, 0)
+
+    # Send a WhatsApp Message to a Group instantly
+    await AsyncPywhatKit.src.sendwhatmsg_to_group_instantly("AB123CDEFGHijklmn", "Hey All!")
+
+
+asyncio.run(main())
+```
+
+For more Examples and Functions, have a look at the [Wiki](https://github.com/SigireddyBalasai/AsyncPywhatKit/wiki/).
+
+## Contributing
+
+Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
+Be sure to read the [Guidelines](https://github.com/SigireddyBalasai/AsyncPywhatKit/blob/main/CONTRIBUTING.md) before Contributing.
+
+## License
+
+Apache license 2.0
+For more information see [this](https://github.com/SigireddyBalasai/AsyncPywhatKit/blob/main/LICENSE)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: AsyncPywhatKit Version: 2.2.6 Summary:
+Metadata-Version: 2.1 Name: AsyncPywhatKit Version: 2.2.7 Summary:
 AsyncPywhatKit is a Simple and Powerful WhatsApp Automation Library with many
 useful Features Home-page: https://github.com/SigireddyBalasai/AsyncPywhatKit
 Download-URL: https://github.com/SigireddyBalasai/AsyncPywhatKit/archive/refs/
 tags/1.0.tar.gz Author: SigireddyBalasai Author-email:
 sigireddybalasai@gmail.com License: MIT Keywords:
 sendwhatmsg,info,playonyt,search,watch_tutorial,async pywhatkit Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
```

### Comparing `AsyncPywhatKit-2.2.6/README.md` & `AsyncPywhatKit-2.2.7/README.md`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,87 +1,87 @@
-![image](https://media.discordapp.net/attachments/842794167134453820/882227960613048350/unknown.png?width=1440&height=420)
-
-[![image](https://flat.badgen.net/github/stars/SigireddyBalasai/AsyncPywhatKit)](https://github.com/SigireddyBalasai/AsyncPywhatKit/stargazers)
-[![image](https://flat.badgen.net/github/forks/SigireddyBalasai/AsyncPywhatKit)](https://github.com/SigireddyBalasai/AsyncPywhatKit/network/members)
-[![image](https://flat.badgen.net/github/open-issues/SigireddyBalasai/AsyncPywhatKit)](https://github.com/SigireddyBalasai/AsyncPywhatKit/issues)
-[![image](https://flat.badgen.net/github/open-prs/SigireddyBalasai/AsyncPywhatKit)](https://github.com/SigireddyBalasai/AsyncPywhatKit/pulls)
-[![image](https://flat.badgen.net/github/commits/SigireddyBalasai/AsyncPywhatKit)](https://github.com/SigireddyBalasai/AsyncPywhatKit/commits/master)
-[![image](https://flat.badgen.net/github/license/SigireddyBalasai/AsyncPywhatKit)](https://github.com/SigireddyBalasai/AsyncPywhatKit/LICENCE)
-[![image](https://flat.badgen.net/github/contributors/SigireddyBalasai/AsyncPywhatKit)](https://github.com/SigireddyBalasai/AsyncPywhatKit/graphs/contributors)
-[![image](https://flat.badgen.net/github/release/SigireddyBalasai/AsyncPywhatKit)](https://github.com/SigireddyBalasai/AsyncPywhatKit/releases)
-![image](https://img.shields.io/github/languages/count/SigireddyBalasai/AsyncPywhatKit)
-![image](https://img.shields.io/github/languages/top/SigireddyBalasai/AsyncPywhatKit)
-![image](https://img.shields.io/librariesio/release/pypi/AsyncPywhatKit)
-![image](https://img.shields.io/github/repo-size/SigireddyBalasai/AsyncPywhatKit)
-[![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FSigireddyBalasai%2FAsyncpywhatkit&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false)](https://hits.seeyoufarm.com)
-<a href="https://scan.coverity.com/projects/sigireddybalasai-asyncpywhatkit">
-  <img alt="Coverity Scan Build Status"
-       src="https://img.shields.io/coverity/scan/27211.svg"/>
-</a>
-<!-- ![logo](https://github.com/Ankit404butfound/PyWhatKit/raw/master/Images/logo.png?raw=true) -->
-
-
-[AsyncPywhatKit](https://pypi.org/project/AsyncPywhatKit/) is a Python library with various helpful features. It's easy-to-use and does not require you to do any additional setup. Currently, it is one of the most popular library for WhatsApp and YouTube automation. New updates are released frequently with new features and bug fixes.
-
-# Links
-
-- **Join our discord server - https://discord.gg/NDXdB6tNwa**
-- **Documentation - [Wiki](https://github.com/SigireddyBalasai/AsyncPywhatKit/wiki/)**
-
-## Installation and Supported Versions
-
-AsyncPywhatKit is available on PyPi:
-
-```bash
-python3 -m pip install AsyncPywhatKit
-```
-
-```bash
-pip3 install AsyncPywhatKit
-```
-
-PyWhatKit officially supports Python 3.8+.
-
-## Cloning the Repository
-
-```bash
-git clone https://github.com/SigireddyBalasai/AsyncPywhatKit
-```
-```py
-import asyncio
-import AsyncPywhatKit
-
-
-async def main():
-    # Send a WhatsApp Message to a Contact at 1:30 PM
-    await AsyncPywhatKit.sendwhatmsg("+910123456789", "Hi", 13, 30)
-
-    # Same as above but Closes the Tab in 2 Seconds after Sending the Message
-    await AsyncPywhatKit.src.sendwhatmsg("+910123456789", "Hi", 13, 30, 15, True, 2)
-
-    # Send an Image to a Group with the Caption as Hello
-    await AsyncPywhatKit.src.sendwhats_image("AB123CDEFGHijklmn", "Images/Hello.png", "Hello")
-
-    # Send an Image to a Contact with the no Caption
-    await AsyncPywhatKit.src.sendwhats_image("+910123456789", "Images/Hello.png")
-
-    # Send a WhatsApp Message to a Group at 12:00 AM
-    await AsyncPywhatKit.src.sendwhatmsg_to_group("AB123CDEFGHijklmn", "Hey All!", 0, 0)
-
-    # Send a WhatsApp Message to a Group instantly
-    await AsyncPywhatKit.src.sendwhatmsg_to_group_instantly("AB123CDEFGHijklmn", "Hey All!")
-
-
-asyncio.run(main())
-```
-
-For more Examples and Functions, have a look at the [Wiki](https://github.com/SigireddyBalasai/AsyncPywhatKit/wiki/).
-
-## Contributing
-
-Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
-Be sure to read the [Guidelines](https://github.com/SigireddyBalasai/AsyncPywhatKit/blob/main/CONTRIBUTING.md) before Contributing.
-
-## License
-
-Apache license 2.0
-For more information see [this](https://github.com/SigireddyBalasai/AsyncPywhatKit/blob/main/LICENSE)
+![image](https://media.discordapp.net/attachments/842794167134453820/882227960613048350/unknown.png?width=1440&height=420)
+
+[![image](https://flat.badgen.net/github/stars/SigireddyBalasai/AsyncPywhatKit)](https://github.com/SigireddyBalasai/AsyncPywhatKit/stargazers)
+[![image](https://flat.badgen.net/github/forks/SigireddyBalasai/AsyncPywhatKit)](https://github.com/SigireddyBalasai/AsyncPywhatKit/network/members)
+[![image](https://flat.badgen.net/github/open-issues/SigireddyBalasai/AsyncPywhatKit)](https://github.com/SigireddyBalasai/AsyncPywhatKit/issues)
+[![image](https://flat.badgen.net/github/open-prs/SigireddyBalasai/AsyncPywhatKit)](https://github.com/SigireddyBalasai/AsyncPywhatKit/pulls)
+[![image](https://flat.badgen.net/github/commits/SigireddyBalasai/AsyncPywhatKit)](https://github.com/SigireddyBalasai/AsyncPywhatKit/commits/master)
+[![image](https://flat.badgen.net/github/license/SigireddyBalasai/AsyncPywhatKit)](https://github.com/SigireddyBalasai/AsyncPywhatKit/LICENCE)
+[![image](https://flat.badgen.net/github/contributors/SigireddyBalasai/AsyncPywhatKit)](https://github.com/SigireddyBalasai/AsyncPywhatKit/graphs/contributors)
+[![image](https://flat.badgen.net/github/release/SigireddyBalasai/AsyncPywhatKit)](https://github.com/SigireddyBalasai/AsyncPywhatKit/releases)
+![image](https://img.shields.io/github/languages/count/SigireddyBalasai/AsyncPywhatKit)
+![image](https://img.shields.io/github/languages/top/SigireddyBalasai/AsyncPywhatKit)
+![image](https://img.shields.io/librariesio/release/pypi/AsyncPywhatKit)
+![image](https://img.shields.io/github/repo-size/SigireddyBalasai/AsyncPywhatKit)
+[![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FSigireddyBalasai%2FAsyncpywhatkit&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false)](https://hits.seeyoufarm.com)
+<a href="https://scan.coverity.com/projects/sigireddybalasai-asyncpywhatkit">
+  <img alt="Coverity Scan Build Status"
+       src="https://img.shields.io/coverity/scan/27211.svg"/>
+</a>
+<!-- ![logo](https://github.com/Ankit404butfound/PyWhatKit/raw/master/Images/logo.png?raw=true) -->
+
+
+[AsyncPywhatKit](https://pypi.org/project/AsyncPywhatKit/) is a Python library with various helpful features. It's easy-to-use and does not require you to do any additional setup. Currently, it is one of the most popular library for WhatsApp and YouTube automation. New updates are released frequently with new features and bug fixes.
+
+# Links
+
+- **Join our discord server - https://discord.gg/NDXdB6tNwa**
+- **Documentation - [Wiki](https://github.com/SigireddyBalasai/AsyncPywhatKit/wiki/)**
+
+## Installation and Supported Versions
+
+AsyncPywhatKit is available on PyPi:
+
+```bash
+python3 -m pip install AsyncPywhatKit
+```
+
+```bash
+pip3 install AsyncPywhatKit
+```
+
+PyWhatKit officially supports Python 3.8+.
+
+## Cloning the Repository
+
+```bash
+git clone https://github.com/SigireddyBalasai/AsyncPywhatKit
+```
+```py
+import asyncio
+import AsyncPywhatKit
+
+
+async def main():
+    # Send a WhatsApp Message to a Contact at 1:30 PM
+    await AsyncPywhatKit.sendwhatmsg("+910123456789", "Hi", 13, 30)
+
+    # Same as above but Closes the Tab in 2 Seconds after Sending the Message
+    await AsyncPywhatKit.src.sendwhatmsg("+910123456789", "Hi", 13, 30, 15, True, 2)
+
+    # Send an Image to a Group with the Caption as Hello
+    await AsyncPywhatKit.src.sendwhats_image("AB123CDEFGHijklmn", "Images/Hello.png", "Hello")
+
+    # Send an Image to a Contact with the no Caption
+    await AsyncPywhatKit.src.sendwhats_image("+910123456789", "Images/Hello.png")
+
+    # Send a WhatsApp Message to a Group at 12:00 AM
+    await AsyncPywhatKit.src.sendwhatmsg_to_group("AB123CDEFGHijklmn", "Hey All!", 0, 0)
+
+    # Send a WhatsApp Message to a Group instantly
+    await AsyncPywhatKit.src.sendwhatmsg_to_group_instantly("AB123CDEFGHijklmn", "Hey All!")
+
+
+asyncio.run(main())
+```
+
+For more Examples and Functions, have a look at the [Wiki](https://github.com/SigireddyBalasai/AsyncPywhatKit/wiki/).
+
+## Contributing
+
+Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
+Be sure to read the [Guidelines](https://github.com/SigireddyBalasai/AsyncPywhatKit/blob/main/CONTRIBUTING.md) before Contributing.
+
+## License
+
+Apache license 2.0
+For more information see [this](https://github.com/SigireddyBalasai/AsyncPywhatKit/blob/main/LICENSE)
```

### Comparing `AsyncPywhatKit-2.2.6/setup.py` & `AsyncPywhatKit-2.2.7/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-from distutils.core import setup
-import pathlib
-import os
-
-dir_path = os.path.dirname(os.path.realpath(__file__))
-
-
-def readme() -> str:
-    with open(r"README.md") as f:
-        README = f.read()
-    return README
-
-
-def reqs():
-    print(dir_path)
-    with open(str(pathlib.Path(dir_path) / "requirements.txt"), "r") as f:
-        requirements = [line.strip() for line in f]
-        return requirements
-
-
-setup(
-    name="AsyncPywhatKit",
-    packages=['AsyncPywhatKit.src', 'AsyncPywhatKit.src.Core'],
-    version="2.2.6",
-    setup_requires=['setuptools_scm'],
-    license="MIT",
-    description="AsyncPywhatKit is a Simple and Powerful WhatsApp Automation Library with many useful Features",
-    author="SigireddyBalasai",
-    author_email="sigireddybalasai@gmail.com",
-    url="https://github.com/SigireddyBalasai/AsyncPywhatKit",
-    download_url="https://github.com/SigireddyBalasai/AsyncPywhatKit/archive/refs/tags/1.0.tar.gz",
-    keywords=["sendwhatmsg", "info", "playonyt", "search", "watch_tutorial", "async pywhatkit"],
-    install_requires=reqs(),
-    include_package_data=True,
-    long_description=readme(),
-    long_description_content_type="text/markdown",
-    classifiers=[
-        "Development Status :: 5 - Production/Stable",
-        "Intended Audience :: Developers",
-        "Topic :: Software Development :: Build Tools",
-        "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
-    ],
-)
+from setuptools import setup
+import pathlib
+import os
+
+dir_path = os.path.dirname(os.path.realpath(__file__))
+
+
+def readme() -> str:
+    with open(r"README.md") as f:
+        README = f.read()
+    return README
+
+
+def reqs():
+    print(dir_path)
+    with open(str(pathlib.Path(dir_path) / "requirements.txt"), "r") as f:
+        requirements = [line.strip() for line in f]
+        return requirements
+
+
+setup(
+    name="AsyncPywhatKit",
+    packages=['AsyncPywhatKit.src','AsyncPywhatKit.src.Core.data','AsyncPywhatKit.src.Core','AsyncPywhatKit'],
+    version="2.2.7",
+    setup_requires=['setuptools_scm'],
+    license="MIT",
+    description="AsyncPywhatKit is a Simple and Powerful WhatsApp Automation Library with many useful Features",
+    author="SigireddyBalasai",
+    author_email="sigireddybalasai@gmail.com",
+    url="https://github.com/SigireddyBalasai/AsyncPywhatKit",
+    download_url="https://github.com/SigireddyBalasai/AsyncPywhatKit/archive/refs/tags/1.0.tar.gz",
+    keywords=["sendwhatmsg", "info", "playonyt", "search", "watch_tutorial", "async pywhatkit"],
+    install_requires=reqs(),
+    include_package_data=True,
+    long_description=readme(),
+    long_description_content_type="text/markdown",
+    classifiers=[
+        "Development Status :: 5 - Production/Stable",
+        "Intended Audience :: Developers",
+        "Topic :: Software Development :: Build Tools",
+        "License :: OSI Approved :: MIT License",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+    ],
+)
```

