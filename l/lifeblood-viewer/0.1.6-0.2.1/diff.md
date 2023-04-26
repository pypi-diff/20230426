# Comparing `tmp/lifeblood-viewer-0.1.6.tar.gz` & `tmp/lifeblood-viewer-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lifeblood-viewer-0.1.6.tar", last modified: Thu Jan 19 10:37:04 2023, max compression
+gzip compressed data, was "lifeblood-viewer-0.2.1.tar", last modified: Wed Apr 26 08:48:19 2023, max compression
```

## Comparing `lifeblood-viewer-0.1.6.tar` & `lifeblood-viewer-0.2.1.tar`

### file list

```diff
@@ -1,5 +1,46 @@
-drwxrwxr-x   0 xapkohheh  (1000) xapkohheh  (1000)        0 2023-01-19 10:37:04.174972 lifeblood-viewer-0.1.6/
--rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     2781 2023-01-19 10:37:04.174972 lifeblood-viewer-0.1.6/PKG-INFO
--rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     2298 2023-01-01 15:25:16.000000 lifeblood-viewer-0.1.6/README.md
--rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)      103 2021-12-18 19:33:37.000000 lifeblood-viewer-0.1.6/pyproject.toml
--rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)      949 2023-01-19 10:37:04.174972 lifeblood-viewer-0.1.6/setup.cfg
+drwxrwxr-x   0 xapkohheh  (1000) xapkohheh  (1000)        0 2023-04-26 08:48:19.307749 lifeblood-viewer-0.2.1/
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     2781 2023-04-26 08:48:19.307749 lifeblood-viewer-0.2.1/PKG-INFO
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     2298 2023-01-01 15:25:16.000000 lifeblood-viewer-0.2.1/README.md
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)      103 2021-12-18 19:33:37.000000 lifeblood-viewer-0.2.1/pyproject.toml
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)      943 2023-04-26 08:48:19.307749 lifeblood-viewer-0.2.1/setup.cfg
+drwxrwxr-x   0 xapkohheh  (1000) xapkohheh  (1000)        0 2023-04-26 08:48:19.303749 lifeblood-viewer-0.2.1/src/
+drwxrwxr-x   0 xapkohheh  (1000) xapkohheh  (1000)        0 2023-04-26 08:48:19.307749 lifeblood-viewer-0.2.1/src/lifeblood_viewer/
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)        0 2021-12-18 19:33:37.000000 lifeblood-viewer-0.2.1/src/lifeblood_viewer/__init__.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)    86248 2021-12-18 19:33:37.000000 lifeblood-viewer-0.2.1/src/lifeblood_viewer/breeze_resources.py
+drwxrwxr-x   0 xapkohheh  (1000) xapkohheh  (1000)        0 2023-04-26 08:48:19.307749 lifeblood-viewer-0.2.1/src/lifeblood_viewer/code_editor/
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)        0 2021-12-18 19:33:37.000000 lifeblood-viewer-0.2.1/src/lifeblood_viewer/code_editor/__init__.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)    10227 2023-04-23 22:17:49.000000 lifeblood-viewer-0.2.1/src/lifeblood_viewer/code_editor/editor.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)    37259 2023-04-25 23:02:00.000000 lifeblood-viewer-0.2.1/src/lifeblood_viewer/connection_worker.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)    10233 2022-08-14 22:56:33.000000 lifeblood-viewer-0.2.1/src/lifeblood_viewer/create_task_dialog.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)      668 2022-04-24 13:58:26.000000 lifeblood-viewer-0.2.1/src/lifeblood_viewer/db_misc.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     1076 2021-12-18 19:33:37.000000 lifeblood-viewer-0.2.1/src/lifeblood_viewer/dialogs.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     1529 2023-03-26 23:30:58.000000 lifeblood-viewer-0.2.1/src/lifeblood_viewer/flashy_label.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)    84954 2023-04-23 22:55:27.000000 lifeblood-viewer-0.2.1/src/lifeblood_viewer/graphics_items.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)    73078 2023-04-20 10:09:16.000000 lifeblood-viewer-0.2.1/src/lifeblood_viewer/graphics_scene.py
+drwxrwxr-x   0 xapkohheh  (1000) xapkohheh  (1000)        0 2023-04-26 08:48:19.307749 lifeblood-viewer-0.2.1/src/lifeblood_viewer/icons/
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     8561 2022-06-06 23:22:35.000000 lifeblood-viewer-0.2.1/src/lifeblood_viewer/icons/lifeblood.svg
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     2768 2022-06-08 10:09:00.000000 lifeblood-viewer-0.2.1/src/lifeblood_viewer/launch.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)    15724 2023-04-22 22:07:35.000000 lifeblood-viewer-0.2.1/src/lifeblood_viewer/lifeblood_viewer.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     1542 2023-03-26 22:47:24.000000 lifeblood-viewer-0.2.1/src/lifeblood_viewer/long_op.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)      225 2023-04-22 21:44:42.000000 lifeblood-viewer-0.2.1/src/lifeblood_viewer/menu_entry_base.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     2109 2021-12-18 19:33:37.000000 lifeblood-viewer-0.2.1/src/lifeblood_viewer/node_extra_items.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)    42091 2023-04-22 22:05:18.000000 lifeblood-viewer-0.2.1/src/lifeblood_viewer/nodeeditor.py
+drwxrwxr-x   0 xapkohheh  (1000) xapkohheh  (1000)        0 2023-04-26 08:48:19.307749 lifeblood-viewer-0.2.1/src/lifeblood_viewer/nodeeditor_windows/
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)        0 2023-04-22 16:48:54.000000 lifeblood-viewer-0.2.1/src/lifeblood_viewer/nodeeditor_windows/__init__.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     4795 2023-04-22 16:51:58.000000 lifeblood-viewer-0.2.1/src/lifeblood_viewer/nodeeditor_windows/ui_create_node_popup.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)      637 2023-04-23 22:17:28.000000 lifeblood-viewer-0.2.1/src/lifeblood_viewer/nodeeditor_windows/ui_parameters_window.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)      665 2023-04-22 22:05:06.000000 lifeblood-viewer-0.2.1/src/lifeblood_viewer/nodeeditor_windows/ui_undo_window.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     2080 2022-03-31 23:17:21.000000 lifeblood-viewer-0.2.1/src/lifeblood_viewer/save_node_settings_dialog.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)    15347 2023-04-23 12:42:13.000000 lifeblood-viewer-0.2.1/src/lifeblood_viewer/scene_ops.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     3673 2023-04-22 17:48:43.000000 lifeblood-viewer-0.2.1/src/lifeblood_viewer/ui_elements_base.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     3529 2023-04-22 17:48:43.000000 lifeblood-viewer-0.2.1/src/lifeblood_viewer/ui_scene_elements.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     4038 2023-03-26 23:05:40.000000 lifeblood-viewer-0.2.1/src/lifeblood_viewer/ui_snippets.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     2386 2023-04-09 17:45:38.000000 lifeblood-viewer-0.2.1/src/lifeblood_viewer/undo_stack.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)    13396 2023-03-24 00:41:49.000000 lifeblood-viewer-0.2.1/src/lifeblood_viewer/worker_list.py
+drwxrwxr-x   0 xapkohheh  (1000) xapkohheh  (1000)        0 2023-04-26 08:48:19.307749 lifeblood-viewer-0.2.1/src/lifeblood_viewer.egg-info/
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     2781 2023-04-26 08:48:19.000000 lifeblood-viewer-0.2.1/src/lifeblood_viewer.egg-info/PKG-INFO
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     1499 2023-04-26 08:48:19.000000 lifeblood-viewer-0.2.1/src/lifeblood_viewer.egg-info/SOURCES.txt
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)        1 2023-04-26 08:48:19.000000 lifeblood-viewer-0.2.1/src/lifeblood_viewer.egg-info/dependency_links.txt
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)       81 2023-04-26 08:48:19.000000 lifeblood-viewer-0.2.1/src/lifeblood_viewer.egg-info/entry_points.txt
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)       99 2023-04-26 08:48:19.000000 lifeblood-viewer-0.2.1/src/lifeblood_viewer.egg-info/requires.txt
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)       17 2023-04-26 08:48:19.000000 lifeblood-viewer-0.2.1/src/lifeblood_viewer.egg-info/top_level.txt
```

### Comparing `lifeblood-viewer-0.1.6/PKG-INFO` & `lifeblood-viewer-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lifeblood-viewer
-Version: 0.1.6
+Version: 0.2.1
 Summary: view the LIFEBLOOD !!
 Home-page: https://github.com/pedohorse/lifeblood
 Author: XAPKOHHEH
 Project-URL: Bug Tracker, https://github.com/pedohorse/lifeblood/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `lifeblood-viewer-0.1.6/README.md` & `lifeblood-viewer-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `lifeblood-viewer-0.1.6/setup.cfg` & `lifeblood-viewer-0.2.1/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 [metadata]
 name = lifeblood-viewer
-version = 0.1.6
+version = 0.2.1
 author = XAPKOHHEH
 description = view the LIFEBLOOD !!
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pedohorse/lifeblood
 project_urls = 
 	Bug Tracker = https://github.com/pedohorse/lifeblood/issues
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 	Operating System :: OS Independent
 
 [options]
 package_dir = 
-	= ../src
+	= src
 packages = find:
 python_requires = >=3.8, <3.11
 install_requires = 
 	imgui~=1.4
 	glfw~=2.5
 	PyOpenGL~=3.1
 	PySide2~=5.15
 	lz4~=4.0
 	lifeblood~=0.1
 	grandalf~=0.7
 	numpy~=1.21
 
 [options.packages.find]
-where = ../src
+where = src
 include = lifeblood_viewer*
 
 [options.package_data]
 lifeblood_viewer = icons/*
 
 [options.entry_points]
 console_scripts =
```

