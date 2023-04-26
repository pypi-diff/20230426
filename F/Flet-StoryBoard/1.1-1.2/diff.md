# Comparing `tmp/Flet StoryBoard-1.1.tar.gz` & `tmp/Flet StoryBoard-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flet StoryBoard-1.1.tar", last modified: Tue Apr 25 14:15:23 2023, max compression
+gzip compressed data, was "Flet StoryBoard-1.2.tar", last modified: Tue Apr 25 19:00:51 2023, max compression
```

## Comparing `Flet StoryBoard-1.1.tar` & `Flet StoryBoard-1.2.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-25 14:15:23.878854 Flet StoryBoard-1.1/
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-25 14:15:23.871600 Flet StoryBoard-1.1/Flet_StoryBoard/
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-25 14:15:23.873201 Flet StoryBoard-1.1/Flet_StoryBoard/Engines/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-23 17:44:35.000000 Flet StoryBoard-1.1/Flet_StoryBoard/Engines/__init__.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     8326 2023-04-23 11:23:40.000000 Flet StoryBoard-1.1/Flet_StoryBoard/Engines/edit_subwidgets_engin.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     8400 2023-04-23 09:53:37.000000 Flet StoryBoard-1.1/Flet_StoryBoard/Engines/edit_widget_engine.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     4927 2023-04-24 14:04:07.000000 Flet StoryBoard-1.1/Flet_StoryBoard/Engines/suggesting_engine.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     2892 2023-04-25 13:53:41.000000 Flet StoryBoard-1.1/Flet_StoryBoard/Engines/viewer_engine.py
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-25 14:15:23.874236 Flet StoryBoard-1.1/Flet_StoryBoard/Tools/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-23 17:43:59.000000 Flet StoryBoard-1.1/Flet_StoryBoard/Tools/__init__.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     3030 2023-04-21 16:25:25.000000 Flet StoryBoard-1.1/Flet_StoryBoard/Tools/color_picker.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      977 2023-04-25 13:40:50.000000 Flet StoryBoard-1.1/Flet_StoryBoard/Tools/create_storyboard.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      702 2023-04-22 11:06:35.000000 Flet StoryBoard-1.1/Flet_StoryBoard/Tools/get_url_icon.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     2857 2023-04-22 13:53:33.000000 Flet StoryBoard-1.1/Flet_StoryBoard/Tools/list_picker.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      118 2023-04-20 11:35:46.000000 Flet StoryBoard-1.1/Flet_StoryBoard/Tools/page_info.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1754 2023-04-25 14:14:21.000000 Flet StoryBoard-1.1/Flet_StoryBoard/Tools/storyboard_class.py
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-25 14:15:23.874531 Flet StoryBoard-1.1/Flet_StoryBoard/WIDGETS/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1117 2023-04-24 11:25:41.000000 Flet StoryBoard-1.1/Flet_StoryBoard/WIDGETS/All.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-23 17:44:18.000000 Flet StoryBoard-1.1/Flet_StoryBoard/WIDGETS/__init__.py
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-25 14:15:23.876272 Flet StoryBoard-1.1/Flet_StoryBoard/WIDGETS/widgets/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-23 17:44:25.000000 Flet StoryBoard-1.1/Flet_StoryBoard/WIDGETS/widgets/__init__.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     2836 2023-04-24 10:12:52.000000 Flet StoryBoard-1.1/Flet_StoryBoard/WIDGETS/widgets/button.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1966 2023-04-24 13:07:17.000000 Flet StoryBoard-1.1/Flet_StoryBoard/WIDGETS/widgets/image.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     2954 2023-04-23 15:09:29.000000 Flet StoryBoard-1.1/Flet_StoryBoard/WIDGETS/widgets/label.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     2077 2023-04-22 15:19:21.000000 Flet StoryBoard-1.1/Flet_StoryBoard/WIDGETS/widgets/markdown.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     2592 2023-04-24 11:23:12.000000 Flet StoryBoard-1.1/Flet_StoryBoard/WIDGETS/widgets/navigator.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     3514 2023-04-23 15:22:36.000000 Flet StoryBoard-1.1/Flet_StoryBoard/WIDGETS/widgets/open_url.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1696 2023-04-23 15:09:43.000000 Flet StoryBoard-1.1/Flet_StoryBoard/WIDGETS/widgets/padding.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     2919 2023-04-24 08:30:46.000000 Flet StoryBoard-1.1/Flet_StoryBoard/WIDGETS/widgets/paragraph.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     7286 2023-04-23 15:54:32.000000 Flet StoryBoard-1.1/Flet_StoryBoard/WIDGETS/widgets/row.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     4927 2023-04-24 10:03:48.000000 Flet StoryBoard-1.1/Flet_StoryBoard/WIDGETS/widgets/textfield.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     2782 2023-04-23 19:24:28.000000 Flet StoryBoard-1.1/Flet_StoryBoard/WIDGETS/widgets/title.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)       92 2023-04-22 14:25:13.000000 Flet StoryBoard-1.1/Flet_StoryBoard/__init__.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1057 2023-04-21 16:27:16.000000 Flet StoryBoard-1.1/Flet_StoryBoard/edit.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1170 2023-04-24 11:12:41.000000 Flet StoryBoard-1.1/Flet_StoryBoard/load_storyboard.py
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-25 14:15:23.876864 Flet StoryBoard-1.1/Flet_StoryBoard/pages/
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-25 14:15:23.877147 Flet StoryBoard-1.1/Flet_StoryBoard/pages/Settings/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-25 13:38:01.000000 Flet StoryBoard-1.1/Flet_StoryBoard/pages/Settings/__init__.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     2028 2023-04-25 14:10:15.000000 Flet StoryBoard-1.1/Flet_StoryBoard/pages/Settings/pages.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-23 17:43:41.000000 Flet StoryBoard-1.1/Flet_StoryBoard/pages/__init__.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     9938 2023-04-24 13:56:02.000000 Flet StoryBoard-1.1/Flet_StoryBoard/pages/create_new_file.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     9941 2023-04-25 14:10:02.000000 Flet StoryBoard-1.1/Flet_StoryBoard/pages/main_page.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     6535 2023-04-25 13:54:52.000000 Flet StoryBoard-1.1/Flet_StoryBoard/pages/settings.py
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-25 14:15:23.877897 Flet StoryBoard-1.1/Flet_StoryBoard/sections/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-23 17:43:49.000000 Flet StoryBoard-1.1/Flet_StoryBoard/sections/__init__.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      623 2023-04-23 08:24:47.000000 Flet StoryBoard-1.1/Flet_StoryBoard/sections/edit_section.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     2033 2023-04-24 08:50:35.000000 Flet StoryBoard-1.1/Flet_StoryBoard/sections/left_section.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      880 2023-04-24 10:23:00.000000 Flet StoryBoard-1.1/Flet_StoryBoard/sections/preview_section.py
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-25 14:15:23.878421 Flet StoryBoard-1.1/Flet_StoryBoard/ui_toolkit/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-23 17:44:08.000000 Flet StoryBoard-1.1/Flet_StoryBoard/ui_toolkit/__init__.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      784 2023-04-22 17:35:05.000000 Flet StoryBoard-1.1/Flet_StoryBoard/ui_toolkit/widget_browser_frame.py
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-25 14:15:23.872506 Flet StoryBoard-1.1/Flet_StoryBoard.egg-info/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      431 2023-04-25 14:15:23.000000 Flet StoryBoard-1.1/Flet_StoryBoard.egg-info/PKG-INFO
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1879 2023-04-25 14:15:23.000000 Flet StoryBoard-1.1/Flet_StoryBoard.egg-info/SOURCES.txt
--rw-r--r--   0 yousifaladwani   (501) staff       (20)        1 2023-04-25 14:15:23.000000 Flet StoryBoard-1.1/Flet_StoryBoard.egg-info/dependency_links.txt
--rw-r--r--   0 yousifaladwani   (501) staff       (20)       21 2023-04-25 14:15:23.000000 Flet StoryBoard-1.1/Flet_StoryBoard.egg-info/requires.txt
--rw-r--r--   0 yousifaladwani   (501) staff       (20)       16 2023-04-25 14:15:23.000000 Flet StoryBoard-1.1/Flet_StoryBoard.egg-info/top_level.txt
--rw-rw-r--   0 yousifaladwani   (501) staff       (20)     1071 2023-02-14 13:25:28.000000 Flet StoryBoard-1.1/LICENSE
--rw-rw-r--   0 yousifaladwani   (501) staff       (20)       24 2023-02-14 13:25:28.000000 Flet StoryBoard-1.1/MANIFEST.in
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      431 2023-04-25 14:15:23.878696 Flet StoryBoard-1.1/PKG-INFO
--rw-rw-r--   0 yousifaladwani   (501) staff       (20)     2487 2023-04-24 14:34:26.000000 Flet StoryBoard-1.1/README.md
--rw-rw-r--   0 yousifaladwani   (501) staff       (20)      103 2023-02-14 13:25:28.000000 Flet StoryBoard-1.1/pyproject.toml
--rw-r--r--   0 yousifaladwani   (501) staff       (20)       38 2023-04-25 14:15:23.878909 Flet StoryBoard-1.1/setup.cfg
--rw-rw-r--   0 yousifaladwani   (501) staff       (20)      592 2023-04-25 09:00:17.000000 Flet StoryBoard-1.1/setup.py
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-25 19:00:51.284163 Flet StoryBoard-1.2/
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-25 19:00:51.277438 Flet StoryBoard-1.2/Flet_StoryBoard/
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-25 19:00:51.279202 Flet StoryBoard-1.2/Flet_StoryBoard/Engines/
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-23 17:44:35.000000 Flet StoryBoard-1.2/Flet_StoryBoard/Engines/__init__.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     8326 2023-04-23 11:23:40.000000 Flet StoryBoard-1.2/Flet_StoryBoard/Engines/edit_subwidgets_engin.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     8400 2023-04-23 09:53:37.000000 Flet StoryBoard-1.2/Flet_StoryBoard/Engines/edit_widget_engine.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     4927 2023-04-24 14:04:07.000000 Flet StoryBoard-1.2/Flet_StoryBoard/Engines/suggesting_engine.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     2892 2023-04-25 13:53:41.000000 Flet StoryBoard-1.2/Flet_StoryBoard/Engines/viewer_engine.py
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-25 19:00:51.280197 Flet StoryBoard-1.2/Flet_StoryBoard/Tools/
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-23 17:43:59.000000 Flet StoryBoard-1.2/Flet_StoryBoard/Tools/__init__.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     3030 2023-04-21 16:25:25.000000 Flet StoryBoard-1.2/Flet_StoryBoard/Tools/color_picker.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      977 2023-04-25 13:40:50.000000 Flet StoryBoard-1.2/Flet_StoryBoard/Tools/create_storyboard.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      702 2023-04-22 11:06:35.000000 Flet StoryBoard-1.2/Flet_StoryBoard/Tools/get_url_icon.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     2857 2023-04-22 13:53:33.000000 Flet StoryBoard-1.2/Flet_StoryBoard/Tools/list_picker.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      118 2023-04-20 11:35:46.000000 Flet StoryBoard-1.2/Flet_StoryBoard/Tools/page_info.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1754 2023-04-25 14:14:21.000000 Flet StoryBoard-1.2/Flet_StoryBoard/Tools/storyboard_class.py
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-25 19:00:51.280480 Flet StoryBoard-1.2/Flet_StoryBoard/WIDGETS/
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1117 2023-04-24 11:25:41.000000 Flet StoryBoard-1.2/Flet_StoryBoard/WIDGETS/All.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-23 17:44:18.000000 Flet StoryBoard-1.2/Flet_StoryBoard/WIDGETS/__init__.py
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-25 19:00:51.282220 Flet StoryBoard-1.2/Flet_StoryBoard/WIDGETS/widgets/
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-23 17:44:25.000000 Flet StoryBoard-1.2/Flet_StoryBoard/WIDGETS/widgets/__init__.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     2836 2023-04-24 10:12:52.000000 Flet StoryBoard-1.2/Flet_StoryBoard/WIDGETS/widgets/button.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1966 2023-04-24 13:07:17.000000 Flet StoryBoard-1.2/Flet_StoryBoard/WIDGETS/widgets/image.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     2954 2023-04-23 15:09:29.000000 Flet StoryBoard-1.2/Flet_StoryBoard/WIDGETS/widgets/label.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     2077 2023-04-22 15:19:21.000000 Flet StoryBoard-1.2/Flet_StoryBoard/WIDGETS/widgets/markdown.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     2592 2023-04-24 11:23:12.000000 Flet StoryBoard-1.2/Flet_StoryBoard/WIDGETS/widgets/navigator.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     3514 2023-04-23 15:22:36.000000 Flet StoryBoard-1.2/Flet_StoryBoard/WIDGETS/widgets/open_url.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1696 2023-04-23 15:09:43.000000 Flet StoryBoard-1.2/Flet_StoryBoard/WIDGETS/widgets/padding.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     2919 2023-04-24 08:30:46.000000 Flet StoryBoard-1.2/Flet_StoryBoard/WIDGETS/widgets/paragraph.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     7286 2023-04-23 15:54:32.000000 Flet StoryBoard-1.2/Flet_StoryBoard/WIDGETS/widgets/row.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     4927 2023-04-24 10:03:48.000000 Flet StoryBoard-1.2/Flet_StoryBoard/WIDGETS/widgets/textfield.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     2782 2023-04-23 19:24:28.000000 Flet StoryBoard-1.2/Flet_StoryBoard/WIDGETS/widgets/title.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)       92 2023-04-22 14:25:13.000000 Flet StoryBoard-1.2/Flet_StoryBoard/__init__.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1615 2023-04-25 18:59:57.000000 Flet StoryBoard-1.2/Flet_StoryBoard/edit.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1170 2023-04-24 11:12:41.000000 Flet StoryBoard-1.2/Flet_StoryBoard/load_storyboard.py
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-25 19:00:51.282871 Flet StoryBoard-1.2/Flet_StoryBoard/pages/
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-25 19:00:51.283125 Flet StoryBoard-1.2/Flet_StoryBoard/pages/Settings/
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-25 13:38:01.000000 Flet StoryBoard-1.2/Flet_StoryBoard/pages/Settings/__init__.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     2028 2023-04-25 14:10:15.000000 Flet StoryBoard-1.2/Flet_StoryBoard/pages/Settings/pages.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-23 17:43:41.000000 Flet StoryBoard-1.2/Flet_StoryBoard/pages/__init__.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     9938 2023-04-24 13:56:02.000000 Flet StoryBoard-1.2/Flet_StoryBoard/pages/create_new_file.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     9941 2023-04-25 14:10:02.000000 Flet StoryBoard-1.2/Flet_StoryBoard/pages/main_page.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     6535 2023-04-25 13:54:52.000000 Flet StoryBoard-1.2/Flet_StoryBoard/pages/settings.py
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-25 19:00:51.283597 Flet StoryBoard-1.2/Flet_StoryBoard/sections/
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-23 17:43:49.000000 Flet StoryBoard-1.2/Flet_StoryBoard/sections/__init__.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      623 2023-04-23 08:24:47.000000 Flet StoryBoard-1.2/Flet_StoryBoard/sections/edit_section.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     2033 2023-04-24 08:50:35.000000 Flet StoryBoard-1.2/Flet_StoryBoard/sections/left_section.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      880 2023-04-24 10:23:00.000000 Flet StoryBoard-1.2/Flet_StoryBoard/sections/preview_section.py
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-25 19:00:51.283811 Flet StoryBoard-1.2/Flet_StoryBoard/ui_toolkit/
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-23 17:44:08.000000 Flet StoryBoard-1.2/Flet_StoryBoard/ui_toolkit/__init__.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      784 2023-04-22 17:35:05.000000 Flet StoryBoard-1.2/Flet_StoryBoard/ui_toolkit/widget_browser_frame.py
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-25 19:00:51.278188 Flet StoryBoard-1.2/Flet_StoryBoard.egg-info/
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      431 2023-04-25 19:00:51.000000 Flet StoryBoard-1.2/Flet_StoryBoard.egg-info/PKG-INFO
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1879 2023-04-25 19:00:51.000000 Flet StoryBoard-1.2/Flet_StoryBoard.egg-info/SOURCES.txt
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)        1 2023-04-25 19:00:51.000000 Flet StoryBoard-1.2/Flet_StoryBoard.egg-info/dependency_links.txt
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)       21 2023-04-25 19:00:51.000000 Flet StoryBoard-1.2/Flet_StoryBoard.egg-info/requires.txt
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)       16 2023-04-25 19:00:51.000000 Flet StoryBoard-1.2/Flet_StoryBoard.egg-info/top_level.txt
+-rw-rw-r--   0 yousifaladwani   (501) staff       (20)     1071 2023-02-14 13:25:28.000000 Flet StoryBoard-1.2/LICENSE
+-rw-rw-r--   0 yousifaladwani   (501) staff       (20)       24 2023-02-14 13:25:28.000000 Flet StoryBoard-1.2/MANIFEST.in
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      431 2023-04-25 19:00:51.284023 Flet StoryBoard-1.2/PKG-INFO
+-rw-rw-r--   0 yousifaladwani   (501) staff       (20)     2487 2023-04-24 14:34:26.000000 Flet StoryBoard-1.2/README.md
+-rw-rw-r--   0 yousifaladwani   (501) staff       (20)      103 2023-02-14 13:25:28.000000 Flet StoryBoard-1.2/pyproject.toml
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)       38 2023-04-25 19:00:51.284205 Flet StoryBoard-1.2/setup.cfg
+-rw-rw-r--   0 yousifaladwani   (501) staff       (20)      592 2023-04-25 19:00:21.000000 Flet StoryBoard-1.2/setup.py
```

### Comparing `Flet StoryBoard-1.1/Flet_StoryBoard/Engines/edit_subwidgets_engin.py` & `Flet StoryBoard-1.2/Flet_StoryBoard/Engines/edit_subwidgets_engin.py`

 * *Files identical despite different names*

### Comparing `Flet StoryBoard-1.1/Flet_StoryBoard/Engines/edit_widget_engine.py` & `Flet StoryBoard-1.2/Flet_StoryBoard/Engines/edit_widget_engine.py`

 * *Files identical despite different names*

### Comparing `Flet StoryBoard-1.1/Flet_StoryBoard/Engines/suggesting_engine.py` & `Flet StoryBoard-1.2/Flet_StoryBoard/Engines/suggesting_engine.py`

 * *Files identical despite different names*

### Comparing `Flet StoryBoard-1.1/Flet_StoryBoard/Engines/viewer_engine.py` & `Flet StoryBoard-1.2/Flet_StoryBoard/Engines/viewer_engine.py`

 * *Files identical despite different names*

### Comparing `Flet StoryBoard-1.1/Flet_StoryBoard/Tools/color_picker.py` & `Flet StoryBoard-1.2/Flet_StoryBoard/Tools/color_picker.py`

 * *Files identical despite different names*

### Comparing `Flet StoryBoard-1.1/Flet_StoryBoard/Tools/create_storyboard.py` & `Flet StoryBoard-1.2/Flet_StoryBoard/Tools/create_storyboard.py`

 * *Files identical despite different names*

### Comparing `Flet StoryBoard-1.1/Flet_StoryBoard/Tools/get_url_icon.py` & `Flet StoryBoard-1.2/Flet_StoryBoard/Tools/get_url_icon.py`

 * *Files identical despite different names*

### Comparing `Flet StoryBoard-1.1/Flet_StoryBoard/Tools/list_picker.py` & `Flet StoryBoard-1.2/Flet_StoryBoard/Tools/list_picker.py`

 * *Files identical despite different names*

### Comparing `Flet StoryBoard-1.1/Flet_StoryBoard/Tools/storyboard_class.py` & `Flet StoryBoard-1.2/Flet_StoryBoard/Tools/storyboard_class.py`

 * *Files identical despite different names*

### Comparing `Flet StoryBoard-1.1/Flet_StoryBoard/WIDGETS/All.py` & `Flet StoryBoard-1.2/Flet_StoryBoard/WIDGETS/All.py`

 * *Files identical despite different names*

### Comparing `Flet StoryBoard-1.1/Flet_StoryBoard/WIDGETS/widgets/button.py` & `Flet StoryBoard-1.2/Flet_StoryBoard/WIDGETS/widgets/button.py`

 * *Files identical despite different names*

### Comparing `Flet StoryBoard-1.1/Flet_StoryBoard/WIDGETS/widgets/image.py` & `Flet StoryBoard-1.2/Flet_StoryBoard/WIDGETS/widgets/image.py`

 * *Files identical despite different names*

### Comparing `Flet StoryBoard-1.1/Flet_StoryBoard/WIDGETS/widgets/label.py` & `Flet StoryBoard-1.2/Flet_StoryBoard/WIDGETS/widgets/label.py`

 * *Files identical despite different names*

### Comparing `Flet StoryBoard-1.1/Flet_StoryBoard/WIDGETS/widgets/markdown.py` & `Flet StoryBoard-1.2/Flet_StoryBoard/WIDGETS/widgets/markdown.py`

 * *Files identical despite different names*

### Comparing `Flet StoryBoard-1.1/Flet_StoryBoard/WIDGETS/widgets/navigator.py` & `Flet StoryBoard-1.2/Flet_StoryBoard/WIDGETS/widgets/navigator.py`

 * *Files identical despite different names*

### Comparing `Flet StoryBoard-1.1/Flet_StoryBoard/WIDGETS/widgets/open_url.py` & `Flet StoryBoard-1.2/Flet_StoryBoard/WIDGETS/widgets/open_url.py`

 * *Files identical despite different names*

### Comparing `Flet StoryBoard-1.1/Flet_StoryBoard/WIDGETS/widgets/padding.py` & `Flet StoryBoard-1.2/Flet_StoryBoard/WIDGETS/widgets/padding.py`

 * *Files identical despite different names*

### Comparing `Flet StoryBoard-1.1/Flet_StoryBoard/WIDGETS/widgets/paragraph.py` & `Flet StoryBoard-1.2/Flet_StoryBoard/WIDGETS/widgets/paragraph.py`

 * *Files identical despite different names*

### Comparing `Flet StoryBoard-1.1/Flet_StoryBoard/WIDGETS/widgets/row.py` & `Flet StoryBoard-1.2/Flet_StoryBoard/WIDGETS/widgets/row.py`

 * *Files identical despite different names*

### Comparing `Flet StoryBoard-1.1/Flet_StoryBoard/WIDGETS/widgets/textfield.py` & `Flet StoryBoard-1.2/Flet_StoryBoard/WIDGETS/widgets/textfield.py`

 * *Files identical despite different names*

### Comparing `Flet StoryBoard-1.1/Flet_StoryBoard/WIDGETS/widgets/title.py` & `Flet StoryBoard-1.2/Flet_StoryBoard/WIDGETS/widgets/title.py`

 * *Files identical despite different names*

### Comparing `Flet StoryBoard-1.1/Flet_StoryBoard/load_storyboard.py` & `Flet StoryBoard-1.2/Flet_StoryBoard/load_storyboard.py`

 * *Files identical despite different names*

### Comparing `Flet StoryBoard-1.1/Flet_StoryBoard/pages/Settings/pages.py` & `Flet StoryBoard-1.2/Flet_StoryBoard/pages/Settings/pages.py`

 * *Files identical despite different names*

### Comparing `Flet StoryBoard-1.1/Flet_StoryBoard/pages/create_new_file.py` & `Flet StoryBoard-1.2/Flet_StoryBoard/pages/create_new_file.py`

 * *Files identical despite different names*

### Comparing `Flet StoryBoard-1.1/Flet_StoryBoard/pages/main_page.py` & `Flet StoryBoard-1.2/Flet_StoryBoard/pages/main_page.py`

 * *Files identical despite different names*

### Comparing `Flet StoryBoard-1.1/Flet_StoryBoard/pages/settings.py` & `Flet StoryBoard-1.2/Flet_StoryBoard/pages/settings.py`

 * *Files identical despite different names*

### Comparing `Flet StoryBoard-1.1/Flet_StoryBoard/sections/edit_section.py` & `Flet StoryBoard-1.2/Flet_StoryBoard/sections/edit_section.py`

 * *Files identical despite different names*

### Comparing `Flet StoryBoard-1.1/Flet_StoryBoard/sections/left_section.py` & `Flet StoryBoard-1.2/Flet_StoryBoard/sections/left_section.py`

 * *Files identical despite different names*

### Comparing `Flet StoryBoard-1.1/Flet_StoryBoard/sections/preview_section.py` & `Flet StoryBoard-1.2/Flet_StoryBoard/sections/preview_section.py`

 * *Files identical despite different names*

### Comparing `Flet StoryBoard-1.1/Flet_StoryBoard/ui_toolkit/widget_browser_frame.py` & `Flet StoryBoard-1.2/Flet_StoryBoard/ui_toolkit/widget_browser_frame.py`

 * *Files identical despite different names*

### Comparing `Flet StoryBoard-1.1/Flet_StoryBoard.egg-info/SOURCES.txt` & `Flet StoryBoard-1.2/Flet_StoryBoard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Flet StoryBoard-1.1/LICENSE` & `Flet StoryBoard-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Flet StoryBoard-1.1/README.md` & `Flet StoryBoard-1.2/README.md`

 * *Files identical despite different names*

### Comparing `Flet StoryBoard-1.1/setup.py` & `Flet StoryBoard-1.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='Flet StoryBoard',
-    version='1.1',
+    version='1.2',
     author='SKbarbon',
     description='A UI-Builder that helps programmers build the front-end without codding it.',
     long_description="https://github.com/SKbarbon/Flet_StoryBoard",
     url='https://github.com/SKbarbon/Flet-StoryBoard',
     install_requires=["flet==0.5.2", "requests"],
     packages=find_packages(),
     classifiers=[
```

