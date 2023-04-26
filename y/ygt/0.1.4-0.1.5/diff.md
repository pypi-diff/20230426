# Comparing `tmp/ygt-0.1.4.tar.gz` & `tmp/ygt-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ygt-0.1.4.tar", last modified: Wed Apr 19 18:35:13 2023, max compression
+gzip compressed data, was "ygt-0.1.5.tar", last modified: Wed Apr 26 01:18:16 2023, max compression
```

## Comparing `ygt-0.1.4.tar` & `ygt-0.1.5.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-04-19 18:35:13.975925 ygt-0.1.4/
--rw-r--r--   0 peterbaker   (504) staff       (20)    11358 2022-11-11 22:39:04.000000 ygt-0.1.4/LICENSE
--rw-r--r--   0 peterbaker   (504) staff       (20)      181 2023-04-16 16:44:10.000000 ygt-0.1.4/MANIFEST.in
--rw-r--r--   0 peterbaker   (504) staff       (20)     2839 2023-04-19 18:35:13.975801 ygt-0.1.4/PKG-INFO
--rw-r--r--   0 peterbaker   (504) staff       (20)     2443 2023-04-19 18:25:54.000000 ygt-0.1.4/README.md
--rw-r--r--   0 peterbaker   (504) staff       (20)      786 2023-04-19 18:06:11.000000 ygt-0.1.4/pyproject.toml
--rw-r--r--   0 peterbaker   (504) staff       (20)       38 2023-04-19 18:35:13.975956 ygt-0.1.4/setup.cfg
--rw-r--r--   0 peterbaker   (504) staff       (20)       38 2022-11-11 22:39:05.000000 ygt-0.1.4/setup.py
-drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-04-19 18:35:13.960430 ygt-0.1.4/src/
-drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-04-19 18:35:13.966839 ygt-0.1.4/src/ygt/
--rw-r--r--   0 peterbaker   (504) staff       (20)        1 2022-11-11 22:39:05.000000 ygt-0.1.4/src/ygt/__init__.py
--rw-r--r--   0 peterbaker   (504) staff       (20)       64 2023-04-06 15:04:52.000000 ygt-0.1.4/src/ygt/__main__.py
--rw-r--r--   0 peterbaker   (504) staff       (20)     1673 2023-04-12 11:23:21.000000 ygt-0.1.4/src/ygt/autohint_trash.py
--rw-r--r--   0 peterbaker   (504) staff       (20)     3729 2023-04-14 00:53:44.000000 ygt-0.1.4/src/ygt/cvGuesser.py
--rw-r--r--   0 peterbaker   (504) staff       (20)     5390 2023-04-19 16:46:17.000000 ygt-0.1.4/src/ygt/fontViewDialog.py
-drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-04-19 18:35:13.967737 ygt-0.1.4/src/ygt/fonts/
--rw-rw-r--   0 peterbaker   (504) staff       (20)   119788 2012-09-20 04:00:00.000000 ygt-0.1.4/src/ygt/fonts/SourceCodePro-Regular.ttf
--rw-r--r--   0 peterbaker   (504) staff       (20)    12272 2023-04-19 13:14:59.000000 ygt-0.1.4/src/ygt/freetypeFont.py
-drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-04-19 18:35:13.975601 ygt-0.1.4/src/ygt/icons/
--rw-r--r--   0 peterbaker   (504) staff       (20)    26646 2022-11-11 22:39:05.000000 ygt-0.1.4/src/ygt/icons/align.png
--rw-r--r--   0 peterbaker   (504) staff       (20)    24080 2022-11-11 22:39:05.000000 ygt-0.1.4/src/ygt/icons/anchor.png
--rw-r--r--   0 peterbaker   (504) staff       (20)    15786 2022-11-11 22:39:05.000000 ygt-0.1.4/src/ygt/icons/black_distance.png
--rw-r--r--   0 peterbaker   (504) staff       (20)     6769 2022-11-11 22:39:05.000000 ygt-0.1.4/src/ygt/icons/cursor-icon-off.png
--rw-r--r--   0 peterbaker   (504) staff       (20)     6681 2022-11-11 22:39:05.000000 ygt-0.1.4/src/ygt/icons/cursor-icon-on.png
--rw-r--r--   0 peterbaker   (504) staff       (20)    10657 2022-12-01 22:00:45.000000 ygt-0.1.4/src/ygt/icons/cv.png
--rw-r--r--   0 peterbaker   (504) staff       (20)     9754 2022-12-18 19:55:30.000000 ygt-0.1.4/src/ygt/icons/cv_guess.png
--rw-r--r--   0 peterbaker   (504) staff       (20)    15405 2022-11-11 22:39:05.000000 ygt-0.1.4/src/ygt/icons/gray_distance.png
--rw-r--r--   0 peterbaker   (504) staff       (20)     6447 2022-11-11 22:39:05.000000 ygt-0.1.4/src/ygt/icons/hand-icon-off.png
--rw-r--r--   0 peterbaker   (504) staff       (20)     6330 2022-11-11 22:39:05.000000 ygt-0.1.4/src/ygt/icons/hand-icon-on.png
--rw-r--r--   0 peterbaker   (504) staff       (20)     7662 2023-01-23 03:27:58.000000 ygt-0.1.4/src/ygt/icons/horizontal-off.png
--rw-r--r--   0 peterbaker   (504) staff       (20)     7714 2023-01-23 03:31:16.000000 ygt-0.1.4/src/ygt/icons/horizontal-on.png
--rw-r--r--   0 peterbaker   (504) staff       (20)    16295 2022-11-11 22:39:05.000000 ygt-0.1.4/src/ygt/icons/interpolate.png
--rw-r--r--   0 peterbaker   (504) staff       (20)    22063 2022-11-11 22:39:05.000000 ygt-0.1.4/src/ygt/icons/make_set.png
--rw-r--r--   0 peterbaker   (504) staff       (20)   536171 2022-11-12 02:29:09.000000 ygt-0.1.4/src/ygt/icons/program.png
--rw-r--r--   0 peterbaker   (504) staff       (20)    28381 2022-11-11 22:39:05.000000 ygt-0.1.4/src/ygt/icons/shift.png
--rw-r--r--   0 peterbaker   (504) staff       (20)    24089 2023-04-12 17:06:29.000000 ygt-0.1.4/src/ygt/icons/stem_distance.png
--rw-r--r--   0 peterbaker   (504) staff       (20)     7025 2023-01-23 03:32:57.000000 ygt-0.1.4/src/ygt/icons/vertical-off.png
--rw-r--r--   0 peterbaker   (504) staff       (20)     6856 2023-01-23 03:32:24.000000 ygt-0.1.4/src/ygt/icons/vertical-on.png
--rw-r--r--   0 peterbaker   (504) staff       (20)    15484 2022-11-11 22:39:05.000000 ygt-0.1.4/src/ygt/icons/white_distance.png
--rw-r--r--   0 peterbaker   (504) staff       (20)     6060 2023-04-14 21:42:13.000000 ygt-0.1.4/src/ygt/macfuncDialog.py
--rw-r--r--   0 peterbaker   (504) staff       (20)    55765 2023-04-11 17:09:51.000000 ygt-0.1.4/src/ygt/makeCVDialog.py
--rwxrwxrwx   0 peterbaker   (504) staff       (20)    64711 2023-04-17 10:32:58.000000 ygt-0.1.4/src/ygt/window.py
--rw-r--r--   0 peterbaker   (504) staff       (20)     2052 2023-04-13 13:41:11.000000 ygt-0.1.4/src/ygt/ygError.py
--rw-rw-r--   0 peterbaker   (504) staff       (20)   112941 2023-04-16 17:05:35.000000 ygt-0.1.4/src/ygt/ygHintEditor.py
--rw-rw-r--   0 peterbaker   (504) staff       (20)   136673 2023-04-19 17:52:17.000000 ygt-0.1.4/src/ygt/ygModel.py
--rwxrwxrwx   0 peterbaker   (504) staff       (20)     8929 2023-04-13 14:28:02.000000 ygt-0.1.4/src/ygt/ygPreferences.py
--rw-r--r--   0 peterbaker   (504) staff       (20)    22475 2023-04-17 16:29:50.000000 ygt-0.1.4/src/ygt/ygPreview.py
--rw-r--r--   0 peterbaker   (504) staff       (20)    10000 2023-04-13 02:48:06.000000 ygt-0.1.4/src/ygt/ygSchema.py
--rw-r--r--   0 peterbaker   (504) staff       (20)     4847 2023-04-15 15:27:33.000000 ygt-0.1.4/src/ygt/ygStems.py
--rw-r--r--   0 peterbaker   (504) staff       (20)    13056 2023-04-17 10:22:52.000000 ygt-0.1.4/src/ygt/ygYAMLEditor.py
-drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-04-19 18:35:13.967619 ygt-0.1.4/src/ygt.egg-info/
--rw-r--r--   0 peterbaker   (504) staff       (20)     2839 2023-04-19 18:35:13.000000 ygt-0.1.4/src/ygt.egg-info/PKG-INFO
--rw-r--r--   0 peterbaker   (504) staff       (20)     1257 2023-04-19 18:35:13.000000 ygt-0.1.4/src/ygt.egg-info/SOURCES.txt
--rw-r--r--   0 peterbaker   (504) staff       (20)        1 2023-04-19 18:35:13.000000 ygt-0.1.4/src/ygt.egg-info/dependency_links.txt
--rw-r--r--   0 peterbaker   (504) staff       (20)       40 2023-04-19 18:35:13.000000 ygt-0.1.4/src/ygt.egg-info/entry_points.txt
--rw-r--r--   0 peterbaker   (504) staff       (20)      159 2023-04-19 18:35:13.000000 ygt-0.1.4/src/ygt.egg-info/requires.txt
--rw-r--r--   0 peterbaker   (504) staff       (20)        4 2023-04-19 18:35:13.000000 ygt-0.1.4/src/ygt.egg-info/top_level.txt
--rw-r--r--   0 peterbaker   (504) staff       (20)       38 2023-01-30 03:58:20.000000 ygt-0.1.4/src/ygt.py
+drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-04-26 01:18:16.311863 ygt-0.1.5/
+-rw-r--r--   0 peterbaker   (504) staff       (20)    11358 2022-11-11 22:39:04.000000 ygt-0.1.5/LICENSE
+-rw-r--r--   0 peterbaker   (504) staff       (20)      181 2023-04-16 16:44:10.000000 ygt-0.1.5/MANIFEST.in
+-rw-r--r--   0 peterbaker   (504) staff       (20)     2839 2023-04-26 01:18:16.311750 ygt-0.1.5/PKG-INFO
+-rw-r--r--   0 peterbaker   (504) staff       (20)     2443 2023-04-19 18:25:54.000000 ygt-0.1.5/README.md
+-rw-r--r--   0 peterbaker   (504) staff       (20)      786 2023-04-26 01:05:06.000000 ygt-0.1.5/pyproject.toml
+-rw-r--r--   0 peterbaker   (504) staff       (20)       38 2023-04-26 01:18:16.311896 ygt-0.1.5/setup.cfg
+-rw-r--r--   0 peterbaker   (504) staff       (20)       38 2022-11-11 22:39:05.000000 ygt-0.1.5/setup.py
+drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-04-26 01:18:16.296095 ygt-0.1.5/src/
+drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-04-26 01:18:16.303400 ygt-0.1.5/src/ygt/
+-rw-r--r--   0 peterbaker   (504) staff       (20)        1 2022-11-11 22:39:05.000000 ygt-0.1.5/src/ygt/__init__.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)       64 2023-04-06 15:04:52.000000 ygt-0.1.5/src/ygt/__main__.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)     1673 2023-04-12 11:23:21.000000 ygt-0.1.5/src/ygt/autohint_trash.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)     3729 2023-04-14 00:53:44.000000 ygt-0.1.5/src/ygt/cvGuesser.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)     5234 2023-04-25 12:51:05.000000 ygt-0.1.5/src/ygt/fontViewDialog.py
+drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-04-26 01:18:16.304277 ygt-0.1.5/src/ygt/fonts/
+-rw-rw-r--   0 peterbaker   (504) staff       (20)   119788 2012-09-20 04:00:00.000000 ygt-0.1.5/src/ygt/fonts/SourceCodePro-Regular.ttf
+-rw-r--r--   0 peterbaker   (504) staff       (20)    12952 2023-04-26 00:07:28.000000 ygt-0.1.5/src/ygt/freetypeFont.py
+drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-04-26 01:18:16.311475 ygt-0.1.5/src/ygt/icons/
+-rw-r--r--   0 peterbaker   (504) staff       (20)    26646 2022-11-11 22:39:05.000000 ygt-0.1.5/src/ygt/icons/align.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)    24080 2022-11-11 22:39:05.000000 ygt-0.1.5/src/ygt/icons/anchor.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)    15786 2022-11-11 22:39:05.000000 ygt-0.1.5/src/ygt/icons/black_distance.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)     6769 2022-11-11 22:39:05.000000 ygt-0.1.5/src/ygt/icons/cursor-icon-off.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)     6681 2022-11-11 22:39:05.000000 ygt-0.1.5/src/ygt/icons/cursor-icon-on.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)    10657 2022-12-01 22:00:45.000000 ygt-0.1.5/src/ygt/icons/cv.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)     9754 2022-12-18 19:55:30.000000 ygt-0.1.5/src/ygt/icons/cv_guess.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)    15405 2022-11-11 22:39:05.000000 ygt-0.1.5/src/ygt/icons/gray_distance.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)     6447 2022-11-11 22:39:05.000000 ygt-0.1.5/src/ygt/icons/hand-icon-off.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)     6330 2022-11-11 22:39:05.000000 ygt-0.1.5/src/ygt/icons/hand-icon-on.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)     7662 2023-01-23 03:27:58.000000 ygt-0.1.5/src/ygt/icons/horizontal-off.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)     7714 2023-01-23 03:31:16.000000 ygt-0.1.5/src/ygt/icons/horizontal-on.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)    16295 2022-11-11 22:39:05.000000 ygt-0.1.5/src/ygt/icons/interpolate.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)    22063 2022-11-11 22:39:05.000000 ygt-0.1.5/src/ygt/icons/make_set.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)   536171 2022-11-12 02:29:09.000000 ygt-0.1.5/src/ygt/icons/program.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)    28381 2022-11-11 22:39:05.000000 ygt-0.1.5/src/ygt/icons/shift.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)    24089 2023-04-12 17:06:29.000000 ygt-0.1.5/src/ygt/icons/stem_distance.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)     7025 2023-01-23 03:32:57.000000 ygt-0.1.5/src/ygt/icons/vertical-off.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)     6856 2023-01-23 03:32:24.000000 ygt-0.1.5/src/ygt/icons/vertical-on.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)    15484 2022-11-11 22:39:05.000000 ygt-0.1.5/src/ygt/icons/white_distance.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)     6060 2023-04-14 21:42:13.000000 ygt-0.1.5/src/ygt/macfuncDialog.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)    56264 2023-04-21 04:37:29.000000 ygt-0.1.5/src/ygt/makeCVDialog.py
+-rwxrwxrwx   0 peterbaker   (504) staff       (20)    65307 2023-04-25 21:18:30.000000 ygt-0.1.5/src/ygt/window.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)     2052 2023-04-13 13:41:11.000000 ygt-0.1.5/src/ygt/ygError.py
+-rw-rw-r--   0 peterbaker   (504) staff       (20)   116392 2023-04-25 21:18:08.000000 ygt-0.1.5/src/ygt/ygHintEditor.py
+-rw-rw-r--   0 peterbaker   (504) staff       (20)   137596 2023-04-24 10:33:58.000000 ygt-0.1.5/src/ygt/ygModel.py
+-rwxrwxrwx   0 peterbaker   (504) staff       (20)     8929 2023-04-13 14:28:02.000000 ygt-0.1.5/src/ygt/ygPreferences.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)    22140 2023-04-26 00:03:21.000000 ygt-0.1.5/src/ygt/ygPreview.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)    10040 2023-04-21 04:31:07.000000 ygt-0.1.5/src/ygt/ygSchema.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)     5674 2023-04-22 03:26:07.000000 ygt-0.1.5/src/ygt/ygStems.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)    13056 2023-04-17 10:22:52.000000 ygt-0.1.5/src/ygt/ygYAMLEditor.py
+drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-04-26 01:18:16.304167 ygt-0.1.5/src/ygt.egg-info/
+-rw-r--r--   0 peterbaker   (504) staff       (20)     2839 2023-04-26 01:18:16.000000 ygt-0.1.5/src/ygt.egg-info/PKG-INFO
+-rw-r--r--   0 peterbaker   (504) staff       (20)     1257 2023-04-26 01:18:16.000000 ygt-0.1.5/src/ygt.egg-info/SOURCES.txt
+-rw-r--r--   0 peterbaker   (504) staff       (20)        1 2023-04-26 01:18:16.000000 ygt-0.1.5/src/ygt.egg-info/dependency_links.txt
+-rw-r--r--   0 peterbaker   (504) staff       (20)       40 2023-04-26 01:18:16.000000 ygt-0.1.5/src/ygt.egg-info/entry_points.txt
+-rw-r--r--   0 peterbaker   (504) staff       (20)      159 2023-04-26 01:18:16.000000 ygt-0.1.5/src/ygt.egg-info/requires.txt
+-rw-r--r--   0 peterbaker   (504) staff       (20)        4 2023-04-26 01:18:16.000000 ygt-0.1.5/src/ygt.egg-info/top_level.txt
+-rw-r--r--   0 peterbaker   (504) staff       (20)       38 2023-01-30 03:58:20.000000 ygt-0.1.5/src/ygt.py
```

### Comparing `ygt-0.1.4/LICENSE` & `ygt-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ygt-0.1.4/PKG-INFO` & `ygt-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ygt
-Version: 0.1.4
+Version: 0.1.5
 Summary: A graphical hint editor for TrueType fonts
 Author-email: "Peter S. Baker" <b.tarde@mail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10.4
 Description-Content-Type: text/markdown
```

### Comparing `ygt-0.1.4/README.md` & `ygt-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `ygt-0.1.4/src/ygt/autohint_trash.py` & `ygt-0.1.5/src/ygt/autohint_trash.py`

 * *Files identical despite different names*

### Comparing `ygt-0.1.4/src/ygt/cvGuesser.py` & `ygt-0.1.5/src/ygt/cvGuesser.py`

 * *Files identical despite different names*

### Comparing `ygt-0.1.4/src/ygt/fontViewDialog.py` & `ygt-0.1.5/src/ygt/fontViewDialog.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,18 +30,16 @@
             self, filename: str, yg_font: ygFont, glyph_list: list, top_window
         ) -> None:
         super().__init__()
         self.valid = True
         self.top_window = top_window
         self.setWindowTitle("Font View")
         self.glyph_name_list = []
-        self.name_to_index = {}
         for g in glyph_list:
             self.glyph_name_list.append(g[1])
-            self.name_to_index[g[1]] = g[0]
         self.yg_font = yg_font
         if self.yg_font.source_file.source_type == "yaml":
             self.face = freetypeFont(filename, size=24, render_mode=RENDER_GRAYSCALE)
         else:
             temp_font = copy.deepcopy(self.yg_font.preview_font)
             tf = SpooledTemporaryFile(max_size=3000000, mode='b')
             options = subset.Options(glyph_names=True)
@@ -129,15 +127,14 @@
                 brush.setColor(QColor("black"))
             else:
                 brush.setColor(QColor("white"))
         brush.setStyle(Qt.BrushStyle.SolidPattern)
         rect = QRect(0, 0, self.width(), self.height())
         painter.fillRect(rect, brush)
 
-        # self.dialog.face.set_char(self.dialog.face.name_to_index(self.glyph))
         ind = self.dialog.face.name_to_index(self.glyph)
         self.dialog.face.set_char(ind)
         baseline = (
             round((36 - self.dialog.face.face_height) / 2) + self.dialog.face.ascender
         )
         xpos = round((36 - self.dialog.face.advance) / 2)
         self.dialog.face.draw_char(painter, xpos, baseline, dark_theme = dark_theme)
```

### Comparing `ygt-0.1.4/src/ygt/fonts/SourceCodePro-Regular.ttf` & `ygt-0.1.5/src/ygt/fonts/SourceCodePro-Regular.ttf`

 * *Files identical despite different names*

### Comparing `ygt-0.1.4/src/ygt/freetypeFont.py` & `ygt-0.1.5/src/ygt/freetypeFont.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Optional
 import freetype as ft # type: ignore
 import numpy
 import copy
 from tempfile import SpooledTemporaryFile
 from PyQt6.QtGui import QColor, QPen
-from PyQt6.QtCore import QRect
+from PyQt6.QtCore import QRect, QLine
 
 
 RENDER_GRAYSCALE = 1
 RENDER_LCD_1 = 2
 RENDER_LCD_2 = 3
 
 
@@ -187,15 +187,23 @@
         for i in range(rows):
             data.extend(self.glyph_slot.bitmap.buffer[i * pitch : i * pitch + width])
         if render_mode == RENDER_GRAYSCALE:
             return numpy.array(data, dtype=numpy.ubyte).reshape(rows, width)
         else:
             return numpy.array(data, dtype=numpy.ubyte).reshape(rows, int(width / 3), 3)
 
-    def _draw_char_lcd(self, painter, x, y, spacing_mark = False, dark_theme = False):
+    def _draw_char_lcd(
+            self,
+            painter,
+            x,
+            y,
+            spacing_mark = False,
+            dark_theme = False,
+            is_target = False
+        ):
         """Draws a bitmap with subpixel rendering (suitable for an lcd screen)
 
         Params:
 
         painter (QPainter): a Qt tool to draw with
 
         x (int): The left origin of the glyph
@@ -235,14 +243,20 @@
                     qp.setColor(qc)
                     painter.setPen(qp)
                     painter.drawPoint(xpos, ypos)
                 xpos += 1
             ypos += 1
         ending_xpos = starting_xpos + round(gdata["advance"])
         ending_ypos = starting_ypos + gdata["rows"]
+        if is_target:
+            ul_y = ending_ypos + 4
+            qc = QPen(QColor("red"))
+            qc.setWidth(2)
+            painter.setPen(qc)
+            painter.drawLine(QLine(starting_xpos, ul_y, ending_xpos, ul_y))
         if abs(ending_ypos - starting_ypos) <= 5:
             starting_ypos -= 3
             ending_ypos += 3
         self.rect_list.append(
             ygLetterBox(
                 starting_xpos,
                 starting_ypos,
@@ -251,15 +265,22 @@
                 glyph_index=self.glyph_index,
                 size=self.size,
                 gname=self.index_to_name(self.glyph_index),
             )
         )
         return gdata["advance"]
 
-    def _draw_char_grayscale(self, painter, x, y, spacing_mark=False, dark_theme = False):
+    def _draw_char_grayscale(
+            self,
+            painter,
+            x,
+            y,
+            spacing_mark=False,
+            dark_theme = False,
+            is_target = False):
         """Draws a bitmap with grayscale rendering
 
         Params:
 
         painter (QPainter): a Qt tool to draw with
 
         x (int): The left origin of the glyph
@@ -289,14 +310,20 @@
                     qp.setColor(self.bw_colors[col])
                 painter.setPen(qp)
                 painter.drawPoint(xpos, ypos)
                 xpos += 1
             ypos += 1
         ending_xpos = starting_xpos + round(gdata["advance"])
         ending_ypos = starting_ypos + gdata["rows"]
+        if is_target:
+            ul_y = ending_ypos + 4
+            qc = QPen(QColor("red"))
+            qc.setWidth(2)
+            painter.setPen(qc)
+            painter.drawLine(QLine(starting_xpos, ul_y, ending_xpos, ul_y))
         if abs(ending_ypos - starting_ypos) <= 5:
             starting_ypos -= 3
             ending_ypos += 3
         self.rect_list.append(
             ygLetterBox(
                 starting_xpos,
                 starting_ypos,
```

### Comparing `ygt-0.1.4/src/ygt/icons/align.png` & `ygt-0.1.5/src/ygt/icons/align.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.4/src/ygt/icons/anchor.png` & `ygt-0.1.5/src/ygt/icons/anchor.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.4/src/ygt/icons/black_distance.png` & `ygt-0.1.5/src/ygt/icons/black_distance.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.4/src/ygt/icons/cursor-icon-off.png` & `ygt-0.1.5/src/ygt/icons/cursor-icon-off.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.4/src/ygt/icons/cursor-icon-on.png` & `ygt-0.1.5/src/ygt/icons/cursor-icon-on.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.4/src/ygt/icons/cv.png` & `ygt-0.1.5/src/ygt/icons/cv.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.4/src/ygt/icons/cv_guess.png` & `ygt-0.1.5/src/ygt/icons/cv_guess.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.4/src/ygt/icons/gray_distance.png` & `ygt-0.1.5/src/ygt/icons/gray_distance.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.4/src/ygt/icons/hand-icon-off.png` & `ygt-0.1.5/src/ygt/icons/hand-icon-off.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.4/src/ygt/icons/hand-icon-on.png` & `ygt-0.1.5/src/ygt/icons/hand-icon-on.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.4/src/ygt/icons/horizontal-off.png` & `ygt-0.1.5/src/ygt/icons/horizontal-off.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.4/src/ygt/icons/horizontal-on.png` & `ygt-0.1.5/src/ygt/icons/horizontal-on.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.4/src/ygt/icons/interpolate.png` & `ygt-0.1.5/src/ygt/icons/interpolate.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.4/src/ygt/icons/make_set.png` & `ygt-0.1.5/src/ygt/icons/make_set.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.4/src/ygt/icons/program.png` & `ygt-0.1.5/src/ygt/icons/program.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.4/src/ygt/icons/shift.png` & `ygt-0.1.5/src/ygt/icons/shift.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.4/src/ygt/icons/stem_distance.png` & `ygt-0.1.5/src/ygt/icons/stem_distance.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.4/src/ygt/icons/vertical-off.png` & `ygt-0.1.5/src/ygt/icons/vertical-off.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.4/src/ygt/icons/vertical-on.png` & `ygt-0.1.5/src/ygt/icons/vertical-on.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.4/src/ygt/icons/white_distance.png` & `ygt-0.1.5/src/ygt/icons/white_distance.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.4/src/ygt/macfuncDialog.py` & `ygt-0.1.5/src/ygt/macfuncDialog.py`

 * *Files identical despite different names*

### Comparing `ygt-0.1.4/src/ygt/makeCVDialog.py` & `ygt-0.1.5/src/ygt/makeCVDialog.py`

 * *Files 0% similar despite different names*

```diff
@@ -864,25 +864,37 @@
 
         self.init_graphics = QCheckBox("Initialize graphics")
         self.init_graphics.stateChanged.connect(self.toggle_init_graphics)
 
         self.assume_always_y = QCheckBox("Assume axis always y")
         self.assume_always_y.stateChanged.connect(self.toggle_assume_always_y)
 
+        self.counterclockwise = QCheckBox("Outer contours counter-clockwise")
+        self.counterclockwise.stateChanged.connect(self.toggle_counterclockwise)
+
         self.cleartype = QCheckBox("Cleartype")
         self.cleartype.stateChanged.connect(self.toggle_cleartype)
 
         self.layout_obj.addWidget(self.tt_defaults)
         self.layout_obj.addWidget(self.init_graphics)
         self.layout_obj.addWidget(self.assume_always_y)
+        self.layout_obj.addWidget(self.counterclockwise)
         self.layout_obj.addWidget(self.cleartype)
         self.setLayout(self.layout_obj)
 
         self.refresh()
 
+    def toggle_counterclockwise(self) -> None:
+        if self.ignore_signal:
+            return
+        if self.counterclockwise.isChecked():
+            self.defaults.set_default({"counterclockwise": True})
+        else:
+            self.defaults.del_default("counterclockwise")
+
     def toggle_tt_defaults(self) -> None:
         if self.ignore_signal:
             return
         if self.tt_defaults.isChecked():
             self.defaults.set_default({"use-truetype-defaults": True})
         else:
             self.defaults.del_default("use-truetype-defaults")
```

### Comparing `ygt-0.1.4/src/ygt/window.py` & `ygt-0.1.5/src/ygt/window.py`

 * *Files 0% similar despite different names*

```diff
@@ -583,14 +583,21 @@
 
     @pyqtSlot(bool)
     def set_mouse_editing(self, editing_on: bool) -> None:
         if self.glyph_pane:
             if editing_on:
                 self.glyph_pane.setDragMode(QGraphicsView.DragMode.NoDrag)
 
+    @pyqtSlot(object)
+    def set_panning_editing(self, mode) -> None:
+        if mode == QGraphicsView.DragMode.ScrollHandDrag:
+            self.hand_action.setChecked(True)
+        else:
+            self.cursor_action.setChecked(True)
+
     #
     # Preview panes
     #
 
     @pyqtSlot()
     def preview_error(self) -> None:
         emsg = "Error compiling YAML or Xgridfit code. "
@@ -617,14 +624,17 @@
             self.glyph_pane.viewer.yg_glyph.set_auto_preview_connection()
         except Exception as e:
             # print(e)
             pass
 
     @pyqtSlot()
     def preview_current_glyph(self) -> None:
+        self._preview_current_glyph()
+
+    def _preview_current_glyph(self) -> None:
         try:
             if self.preview_maker != None and self.preview_maker.isRunning():
                 return
         except RuntimeError as e:
             # We get this RuntimeError when self.thread has been garbage collected.
             # It means that it's safe to run the rest of this function.
             pass
@@ -873,14 +883,15 @@
         self.coord_label_action.triggered.connect(self.coord_labels)
 
     def setup_nav_connections(self) -> None:
         self.next_glyph_action.triggered.connect(self.glyph_pane.next_glyph)
         self.previous_glyph_action.triggered.connect(self.glyph_pane.previous_glyph)
         self.goto_action.triggered.connect(self.show_goto_dialog)
         self.glyph_pane.setup_goto_signal(self.show_goto_dialog)
+        self.glyph_pane.setup_toggle_drag_mode_signal(self.set_panning_editing)
         self.font_view_action.triggered.connect(self.show_font_view)
 
     def setup_undo_connections(self) -> None:
         self.undo_action.triggered.connect(self.undo_group.undo)
         self.redo_action.triggered.connect(self.undo_group.redo)
 
     def setup_cursor_connections(self) -> None:
@@ -1292,21 +1303,24 @@
                 initGlyph = self.preferences["current_glyph"][self.yg_font.full_name()]
             else:
                 initGlyph = "A"
             modelGlyph = ygGlyph(self.preferences, self.yg_font, initGlyph)
             modelGlyph.set_yaml_editor(self.source_editor)
             viewer = ygGlyphScene(self.preferences, modelGlyph)
             view = ygGlyphView(self.preferences, viewer, self.yg_font)
+            viewer.owner = view
             self.add_glyph_pane(view)
             view.centerOn(view.viewer.center_x, view.sceneRect().center().y())
             self.set_window_title()
             self.set_up_instance_list()
             self.setup_editor_connections()
             self.setup_preview_instance_connections()
             self.setup_point_label_connections()
+            # Should we send a signal for preview update from here?
+            self._preview_current_glyph()
         return 0
 
     #
     # GUI management
     #
 
     def setup_stem_buttons(self, axis):
@@ -1528,19 +1542,24 @@
 
     @pyqtSlot(object)
     def go_to_glyph(self, g: str) -> None:
         self.glyph_pane.go_to_glyph(g)
 
     @pyqtSlot()
     def show_ppem_dialog(self):
-        text, ok = QInputDialog().getText(
-            self, "Set Points per Em", "Points per em:", QLineEdit.EchoMode.Normal
+        i, ok = QInputDialog().getInt(
+            self,
+            "Set Points per Em",
+            "Points per em:",
+            value = 30,
+            min = 10,
+            max = 400,
         )
-        if ok and text:
-            self.yg_preview.set_size(text)
+        if ok:
+            self.yg_preview.set_size(i)
 
     #
     # Program exit
     #
 
     def save_query(self) -> int:
         msg_box = QMessageBox()
```

### Comparing `ygt-0.1.4/src/ygt/ygError.py` & `ygt-0.1.5/src/ygt/ygError.py`

 * *Files identical despite different names*

### Comparing `ygt-0.1.4/src/ygt/ygHintEditor.py` & `ygt-0.1.5/src/ygt/ygHintEditor.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     QPainterPath,
     QPen,
     QBrush,
     QColor,
     QPolygonF,
     QAction,
     QPainter,
+    QPalette,
 )
 from PyQt6.QtWidgets import (
     QWidget,
     QApplication,
     QGraphicsScene,
     QGraphicsView,
     QGraphicsItem,
@@ -56,14 +57,15 @@
     QDialog,
     QInputDialog,
     QLineEdit,
     QGraphicsProxyWidget,
     QStyleOptionGraphicsItem,
 )
 from fontTools.pens.basePen import BasePen  # type: ignore
+from fontTools.pens.boundsPen import BoundsPen
 from .ygPreferences import ygPreferences
 
 
 HINT_ARROW_WIDTH = 3
 HINT_ANCHOR_WIDTH = 3
 HINT_LINK_WIDTH = 1
 HINT_ARROWHEAD_WIDTH = 2
@@ -1352,35 +1354,48 @@
     sig_round_hint = pyqtSignal(object)
     sig_min_dist = pyqtSignal(object)
     sig_swap_macfunc_points = pyqtSignal(object)
     sig_toggle_point_numbers = pyqtSignal()
     sig_set_category = pyqtSignal(object)
     sig_name_points = pyqtSignal(object)
 
-    def __init__(self, preferences: ygPreferences, yg_glyph: ygGlyph) -> None:
+    def __init__(
+            self, preferences: ygPreferences,
+            yg_glyph: ygGlyph,
+            owner: Optional["ygGlyphView"] = None) -> None:
         """yg_glyph is a ygGlyph object from ygModel."""
         self.preferences = preferences
 
+        # Set up glyph info
+
+        self.yg_glyph = yg_glyph
+        self.owner = owner
+
         self.yg_point_view_index: dict = {}
         self.yg_point_view_list: list = []
         # No use for this one (right now)
         # self.yg_hint_view_index: dict = {}
         self.yg_hint_view_list: list = []
         super(ygGlyphScene, self).__init__()
         self.cv_error_msg = "Error while looking for a control value."
 
         # Current display preferences
 
-        self.off_curve_points_showing = self.preferences.show_off_curve_points()
+        if self.preferences.top_window().show_off_curve_points != None:
+            self.off_curve_points_showing = self.preferences.top_window().show_off_curve_points
+        else:
+            self.off_curve_points_showing = self.preferences.show_off_curve_points()
         self.point_numbers_showing = self.preferences.top_window().show_point_numbers
-        self.zoom_factor = self.preferences.zoom_factor()
-
-        # Set up glyph info
+        self.zoom_factor = 1.0
+        self.initial_zoom_factor = None
+        self.canvas_size = self._calc_canvas_size()
+        self.setSceneRect(QRectF(0, 0, self.canvas_size[0], self.canvas_size[1]))
+        self.xTranslate = self.canvas_size[2]
+        self.yTranslate = self.canvas_size[3]
 
-        self.yg_glyph = yg_glyph
 
         # Try to get rid of ref to this scene in the model's ygGlyph class.
         # For now, we've got to ignore the type so as to avoid circular imports.
         self.yg_glyph.glyph_viewer = self  # type: ignore
 
         # Make graphical points
 
@@ -1391,18 +1406,15 @@
 
         # Set up dimensions; scale the glyph.
 
         self.adv = 0
         self.lsb = 0
         self.xTranslate = 0
         self.yTranslate = 0
-        # Not gonna mess with types from fontTools.
         self.original_coordinates: Any = None
-        self.scale_glyph()
-        self.center_x = self.xTranslate + round(self.adv / 2)
         self.center_x = self.xTranslate + round(self.adv / 2)
 
         # Setup for selecting
 
         # selectionRect is the rubber band. None when no selection is underway.
         self.selectionRect: Optional[SelectionRect] = None
         # Set dragBeginPoint whenever left mouse button is pressed, in case of
@@ -1455,23 +1467,27 @@
         print("xTranslate: " + str(self.xTranslate))
         print("yTranslate: " + str(self.yTranslate))
         ft_font = self.yg_glyph.yg_font.ft_font
         oc = ft_font["glyf"]._getCoordinatesAndControls(
             self.yg_glyph.gname, ft_font["hmtx"].metrics
         )[0]
         print("First point: " + str(oc[0]))
-        print("Canvas rect: " + str(self.sceneRect()))
+        qr = self.sceneRect()
+        #print("Canvas rect: " + str(self.sceneRect()))
+        print("Canvas rect: " + str(qr.x()) + " " + str(qr.y()) + " " + str(qr.width()) + " " + str(qr.height()))
         print("")
 
     def set_zoom_factor(self, new_zoom: float) -> None:
         self.zoom_factor = new_zoom
+        # We are ignoring the zoom_factor setting in the preferences now, in favor
+        # of setting an optimal zoom factor in the __init__ of ygGlyphScene. Survey
+        # uses of the preferences object to make sure this is so.
         self.preferences.top_window().zoom_factor = self.zoom_factor
         self.scale_glyph()
         self.center_x = self.xTranslate + round(self.adv / 2)
-        self.center_x = self.xTranslate + round(self.adv / 2)
         self.update()
         self.install_hints(self.yg_glyph.hints())
         # This will have the effect of moving point labels to the new positions
         # of the points. Affect only those already visible.
         for p in self.yg_point_view_list:
             if p.has_label():
                 p.add_label()
@@ -1557,32 +1573,71 @@
             adjust = POINT_ONCURVE_DIA / 2
         else:
             adjust = POINT_OFFCURVE_DIA / 2
         # These are the coordinates for the points
         # print("x: " + str(thisx - adjust))
         # print("y: " + str(thisy - adjust))
         return QPointF(thisx - adjust, thisy - adjust)
+    
+    def mid_point_y(self):
+        if len(self.yg_point_view_list) > 0:
+            highest, lowest = self.yg_glyph.extreme_points_y()
+            highest_coord = self.yg_point_view_list[highest[0]].glocation.y()
+            lowest_coord = self.yg_point_view_list[lowest[0]].glocation.y()
+            return lowest_coord - round((lowest_coord - highest_coord) / 2)
+        else:
+            if self.owner:
+                return self.owner.sceneRect().center().y()
+            return 500
 
     #
     # Overrides
     #
 
     def drawBackground(self, painter: QPainter, rect) -> None:
         """The glyph outline is drawn as the background layer for this scene.
         Points and hints are drawn in the item layer, and the foreground
         layer is not used at this time.
         """
+        if not self.initial_zoom_factor:
+            visible_x = rect.width()
+            visible_y = rect.height()
+            optimal_x = round(visible_x * 0.8)
+            optimal_y = round(visible_y * 0.8)
+            width, height = self.yg_glyph.dimensions()
+            if width != 0:
+                x_ratio = optimal_x / width
+            else:
+                x_ratio = 1
+            if height != 0:
+                y_ratio = optimal_y / height
+            else:
+                y_ratio = 1
+            # Limit the initial zoom factor to max of 2.0. This prevents little glyphs
+            # like period from becoming disconcertingly large.
+            self.initial_zoom_factor = min(2.0, min(x_ratio, y_ratio))
+            self.set_zoom_factor(self.initial_zoom_factor)
+            if self.owner:
+                self.owner.centerOn(self.center_x, self.mid_point_y())
+
+
         painter.scale(1.0, -1.0)
         painter.translate(QPointF(self.xTranslate, self.yTranslate * -1))
 
         pen = painter.pen()
 
         if self.preferences["show_metrics"]:
+            text_hsv_value = self.palette().color(QPalette.ColorRole.WindowText).value()
+            bg_hsv_value = self.palette().color(QPalette.ColorRole.Base).value()
+            dark_theme = text_hsv_value > bg_hsv_value
             pen.setWidth(1)
-            pen.setColor(QColor(50, 50, 50, 50))
+            if dark_theme:
+                pen.setColor(QColor(200, 200, 200, 50))
+            else:
+                pen.setColor(QColor(50, 50, 50, 50))
             painter.setPen(pen)
             painter.drawLine(QLine(-abs(self.xTranslate), 0, round(self.width()), 0))
             ya = -abs(self.yTranslate)
             painter.drawLine(QLine(0, ya, 0, round(self.height())))
             painter.drawLine(QLine(self.adv, ya, self.adv, round(self.height())))
 
         pen.setWidth(CHAR_OUTLINE_WIDTH)
@@ -1652,15 +1707,14 @@
 
     @pyqtSlot(object)
     def edit_macfunc_params(self, hint: ygHintView) -> None:
         ed_dialog = macfuncDialog(hint)
         r = ed_dialog.exec()
         if r == QDialog.DialogCode.Accepted:
             hint.yg_hint.set_macfunc_other_args(ed_dialog.result_dict)
-            # hint.yg_hint.hint_has_changed(hint.yg_hint)
 
     @pyqtSlot()
     def toggle_off_curve_visibility(self) -> None:
         self.off_curve_points_showing = not self.off_curve_points_showing
         self.preferences.top_window().show_off_curve_points = (
             self.off_curve_points_showing
         )
@@ -1704,14 +1758,16 @@
         # params: ygModel.ygHint, list of ygModel.ygPoint, touched ygModel.ygPoint, callback func.
         self.yg_glyph.make_set(
             hint_model, new_list, touched_point.yg_point, hint._update_touches
         )
         self.yg_glyph.hint_changed(hint_model)
 
     def make_control_value(self) -> None:
+        """ With one or two points selected, launch a dialog for making a pos or dist CV.
+        """
         sel = self.selected_objects(True)
         if len(sel) == 0:
             return
         if len(sel) >= 1:
             p1 = self._model_point(sel[0])
         p2 = None
         if len(sel) >= 2:
@@ -2786,36 +2842,42 @@
     convenience functions supplying various kinds of information about the
     font.
 
     parent: Is this used at all?
     """
 
     sig_goto = pyqtSignal(object)
+    sig_toggle_drag_mode = pyqtSignal(object)
 
     def __init__(
         self,
         preferences: ygPreferences,
         viewer: ygGlyphScene,
         font: ygFont,
         parent=None,
     ) -> None:
         super(ygGlyphView, self).__init__(viewer, parent=parent)
         self.setAttribute(Qt.WidgetAttribute.WA_AcceptTouchEvents, False)
         self.viewer = viewer
         self.yg_font = font
         self.preferences = preferences
         self.visited_glyphs: Dict[str, ygGlyphScene] = {}
+        self.drag_mode_backup = QGraphicsView.DragMode.NoDrag
+
 
     @pyqtSlot()
     def make_control_value(self) -> None:
         self.viewer.make_control_value()
 
     def setup_goto_signal(self, o: Callable) -> None:
         self.sig_goto.connect(o)
 
+    def setup_toggle_drag_mode_signal(self, o: Callable) -> None:
+        self.sig_toggle_drag_mode.connect(o)
+
     def _current_index(self) -> int:
         return self.yg_font.get_glyph_index(
             self.viewer.yg_glyph.gname, short_index=True
         )
 
     def go_to_glyph(self, g: str) -> None:
         self.preferences["top_window"].disconnect_editor_signals()
@@ -2864,21 +2926,22 @@
             new_glyph = self.viewer.yg_glyph
             # If we're returning to a glyph, we have to undo the cleanup
             # we did when we left it.
             new_glyph.undo_stack.setActive()
             new_glyph.restore_gsource()
         else:
             new_glyph = ygGlyph(self.preferences, self.yg_font, gname)
-            self.viewer = ygGlyphScene(self.preferences, new_glyph)
+            self.viewer = ygGlyphScene(self.preferences, new_glyph, owner = self)
         self.preferences.set_current_glyph(self.yg_font.full_name(), gname)
         self.setScene(self.viewer)
         self.centerOn(self.viewer.center_x, self.sceneRect().center().y())
         self.parent().parent().set_window_title()  # type: ignore
         ed = self.preferences.top_window().source_editor
         new_glyph.set_yaml_editor(ed)
+        new_glyph.sig_hints_changed.emit(new_glyph.hints())
 
     @pyqtSlot()
     def guess_cv(self) -> None:
         try:
             self.viewer.guess_cv()
         except Exception:
             self.yg_font.send_error_message(
@@ -2933,15 +2996,16 @@
     # Why does sender return None when we use the decorator? What's best in this
     # situation? Here are problems: sender_text param is not consulted. Should it be
     # omitted? Make sure params match, esp. if we change them.
     # @pyqtSlot(object)
     def zoom(self, sender_text: str) -> None:
         sender_text = self.sender().text()  # type: ignore
         if sender_text == "Original Size":
-            self.viewer.set_zoom_factor(1)
+            #self.viewer.set_zoom_factor(1)
+            self.viewer.set_zoom_factor(self.viewer.initial_zoom_factor)
         elif sender_text == "Zoom In":
             if self.viewer.zoom_factor <= 5.75:
                 self.viewer.set_zoom_factor(self.viewer.zoom_factor + 0.25)
         elif sender_text == "Zoom Out":
             if self.viewer.zoom_factor >= 0.5:
                 self.viewer.set_zoom_factor(self.viewer.zoom_factor - 0.25)
 
@@ -2950,15 +3014,26 @@
         # Qt methods I've tried. So we're defaulting to having the center of the
         # glyph in the center--which at least is easy.
 
         # v = self.viewport().geometry()
         # qp = QPoint(round(v.x() + (v.width() / 2)), round(v.y() + (v.height() / 2)))
         # self.centerOn(self.mapToScene(qp))
 
-        self.centerOn(self.viewer.center_x, self.sceneRect().center().y())
+        # self.centerOn(self.viewer.center_x, self.sceneRect().center().y())
+        self.centerOn(self.viewer.center_x, self.viewer.mid_point_y())
 
     def keyPressEvent(self, event) -> None:
         if event.key() in [16777219, 16777223]:
             self.viewer.delete_selected_hints()
+        elif event.key() == 32 and not event.isAutoRepeat():
+            self.drag_mode_backup = self.dragMode()
+            if self.drag_mode_backup == QGraphicsView.DragMode.NoDrag:
+                self.sig_toggle_drag_mode.emit(QGraphicsView.DragMode.ScrollHandDrag)
+
+    def keyReleaseEvent(self, event):
+        if event.key() == 32 and not event.isAutoRepeat():
+            if self.drag_mode_backup != self.dragMode():
+                self.sig_toggle_drag_mode.emit(self.drag_mode_backup)
+
 
     def focusInEvent(self, event) -> None:
         self.viewer.yg_glyph.undo_stack.setActive(True)
```

### Comparing `ygt-0.1.4/src/ygt/ygModel.py` & `ygt-0.1.5/src/ygt/ygModel.py`

 * *Files 1% similar despite different names*

```diff
@@ -368,15 +368,15 @@
             try:
                 self.ft_font = ttLib.TTFont(fontfile)
             except FileNotFoundError as ferr:
                 ft_open_error = True
         elif extension == ".ufo":
             try:
                 ufo = defcon.Font(fontfile)
-                self.ft_font = compileTTF(ufo, useProductionNames=False)
+                self.ft_font = compileTTF(ufo, useProductionNames=False, reverseDirection=False)
             except Exception as e:
                 print(e)
                 ft_open_error = True
         if ft_open_error:
             raise Exception("Can't find font file " + str(fontfile))
             # Fix this! Need a dialog box and a chance to try again for a valid font.
 
@@ -644,30 +644,15 @@
                 c = unicodedata.category(chr(u))
             except Exception:
                 pass
         return c
 
     def extreme_points(self, glyph_name: str) -> tuple[tuple, tuple]:
         """Helper for setting up an initial cvt."""
-        g = ygGlyph(ygPreferences(), self, glyph_name)
-        last_highest = highest = -10000
-        last_lowest = lowest = 10000
-        highest_point = -1
-        lowest_point = -1
-        plist = g.point_list
-        for i, p in enumerate(plist):
-            highest = max(highest, p.font_y)
-            if highest != last_highest:
-                last_highest = highest
-                highest_point = i
-            lowest = min(lowest, p.font_y)
-            if lowest != last_lowest:
-                last_lowest = lowest
-                lowest_point = i
-        return (highest_point, highest), (lowest_point, lowest)
+        return ygGlyph(ygPreferences(), self, glyph_name).extreme_points_y()
 
     def family_name(self) -> str:
         return self.ft_font["name"].getName(1, 3, 1, 0x409)
 
     def style_name(self) -> str:
         return self.ft_font["name"].getName(2, 3, 1, 0x409)
 
@@ -2342,14 +2327,55 @@
                 return random_point
         return 0
 
     #
     # Accessing glyph data
     #
 
+    def extreme_points_y(self):
+        last_highest = highest = -100000
+        last_lowest = lowest = 100000
+        highest_point = -1
+        lowest_point = -1
+        for i, p in enumerate(self.point_list):
+            highest = max(highest, p.font_y)
+            if highest != last_highest:
+                last_highest = highest
+                highest_point = i
+            lowest = min(lowest, p.font_y)
+            if lowest != last_lowest:
+                last_lowest = lowest
+                lowest_point = i
+        return (highest_point, highest), (lowest_point, lowest)
+
+    def extreme_points_x(self):
+        last_right = right = -100000
+        last_left = left = 100000
+        rightmost_point = -1
+        leftmost_point = -1
+        for i, p in enumerate(self.point_list):
+            right = max(right, p.font_x)
+            if right != last_right:
+                last_right = right
+                rightmost_point = i
+            left = min(left, p.font_x)
+            if left != last_left:
+                last_left = left
+                leftmost_point = i
+        return (rightmost_point, right), (leftmost_point, left)
+    
+    def dimensions(self):
+        if len(self.point_list) == 0:
+            return 0, 0
+        x_right, x_left = self.extreme_points_x()
+        y_top, y_bottom = self.extreme_points_y()
+        x_dim = x_right[1] - x_left[1]
+        y_dim = y_top[1] - y_bottom[1]
+        return x_dim, y_dim
+
     def get_category(self, long_name: bool = False) -> str:
         cat = self.props.get_property("category")
         if cat == None:
             cat = self.yg_font.get_unicode_category(self.gname)
         if long_name:
             return unicode_cat_names[cat]
         return cat
```

### Comparing `ygt-0.1.4/src/ygt/ygPreferences.py` & `ygt-0.1.5/src/ygt/ygPreferences.py`

 * *Files identical despite different names*

### Comparing `ygt-0.1.4/src/ygt/ygPreview.py` & `ygt-0.1.5/src/ygt/ygPreview.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
     def __init__(self, top_window) -> None:
         super().__init__()
         self.top_window = top_window
         self.face: Optional[freetypeFont] = None
         self.hinting = "on"
         self.glyph_index = 0
-        self.char_size = 30
+        self.char_size = 25
         self.label = QLabel()
         self.label.setStyleSheet("QLabel {background-color: transparent; color: red;}")
         self.label.setText(str(self.char_size) + "ppem")
         self.label.setParent(self)
         self.label.move(50, 30)
         self.minimum_x = PREVIEW_WIDTH
         self.minimum_y = PREVIEW_HEIGHT
@@ -75,15 +75,14 @@
         # Two- or three-dimensional array shaped by numpy.
         self.Z: list = []
         self.instance_dict: Optional[dict] = None
         self.instance: Optional[str] = None
         text_hsv_value = self.palette().color(QPalette.ColorRole.WindowText).value()
         bg_hsv_value = self.palette().color(QPalette.ColorRole.Base).value()
         self.dark_theme = text_hsv_value > bg_hsv_value
-        print(self.dark_theme)
         self.colors = self.mk_color_list()
         self.render_mode = RENDER_LCD_1
         self.hinting_on = True
         self.paintEvent = self.paintEvent_b # type: ignore
 
     def set_up_signal(self, func: Callable) -> None:
         self.sig_preview_paint_done.connect(func)
@@ -339,17 +338,14 @@
                 painter.drawLine(QLine(left, y_top, left, y_bot))
                 left += self.pixel_size
 
     def paintEvent_a(self, event) -> None:
         """Paint grayscale glyph."""
         painter = QPainter(self)
         brush = QBrush()
-        #text_hsv_value = self.palette().color(QPalette.ColorRole.WindowText).value()
-        #bg_hsv_value = self.palette().color(QPalette.ColorRole.Base).value()
-        #self.dark_theme = text_hsv_value > bg_hsv_value
         if self.dark_theme:
             brush.setColor(QColor("black"))
         else:
             brush.setColor(QColor("white"))
         brush.setStyle(Qt.BrushStyle.SolidPattern)
         rect = QRect(0, 0, self.width(), self.height())
         painter.fillRect(rect, brush)
@@ -374,17 +370,14 @@
         painter.end()
         self.sig_preview_paint_done.emit(None)
 
     def paintEvent_b(self, event) -> None:
         """Paint subpixel rendering with solid pixels."""
         painter = QPainter(self)
         brush = QBrush()
-        #text_hsv_value = self.palette().color(QPalette.ColorRole.WindowText).value()
-        #bg_hsv_value = self.palette().color(QPalette.ColorRole.Base).value()
-        #self.dark_theme = text_hsv_value > bg_hsv_value
         if self.dark_theme:
             brush.setColor(QColor("black"))
         else:
             brush.setColor(QColor("white"))
         brush.setStyle(Qt.BrushStyle.SolidPattern)
         rect = QRect(0, 0, self.width(), self.height())
         painter.fillRect(rect, brush)
@@ -510,38 +503,41 @@
         else:
             brush.setColor(QColor("white"))
         brush.setStyle(Qt.BrushStyle.SolidPattern)
         rect = QRect(0, 0, self.width(), self.height())
         painter.fillRect(rect, brush)
 
     def paintEvent_a(self, event) -> None:
+        target_size = self.yg_preview.char_size
         painter = QPainter(self)
         self._fill_background(painter)
         if self.face == None:
             painter.end()
             return
         if not self.yg_preview:
             return
         self.face.reset_rect_list()
         xposition = 25
         yposition = 66
         for s in range(10, 100):
+            this_is_target = (s == target_size)
             self.face.set_params(
                 glyph=self.yg_preview.glyph_index,
                 render_mode=self.yg_preview.render_mode,
                 hinting_on=self.yg_preview.hinting_on,
                 size=s,
                 instance=self.yg_preview.instance,
             )
             advance = self.face.draw_char(
                 painter,
                 xposition,
                 yposition,
                 spacing_mark=True,
-                dark_theme=self.yg_preview.dark_theme
+                dark_theme=self.yg_preview.dark_theme,
+                is_target=this_is_target
             )
             xposition += advance
             if xposition + advance > (PREVIEW_WIDTH - 50):
                 if yposition == 66:
                     xposition = 25
                     yposition = 133
                 else:
```

### Comparing `ygt-0.1.4/src/ygt/ygSchema.py` & `ygt-0.1.5/src/ygt/ygSchema.py`

 * *Files 1% similar despite different names*

```diff
@@ -254,14 +254,15 @@
 ]
 
 defaults_struct = {
     Optional("use-truetype-defaults"): bool,
     Optional("init-graphics"): bool,
     Optional("assume-always-y"): bool,
     Optional("cleartype"): bool,
+    Optional("counterclockwise"): bool,
     Optional("round"): hint_types,
     Optional("no-round"): hint_types,
     Optional("cv_vars_generated"): bool,
 }
 
 properties_struct = {
     Optional("category"): Or(
```

### Comparing `ygt-0.1.4/src/ygt/ygStems.py` & `ygt-0.1.5/src/ygt/ygStems.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Optional, List, TYPE_CHECKING
 from .ygModel import ygPoint, ygGlyph
 
 
 class stemFinder:
     def __init__(self, p1: ygPoint, p2: ygPoint, yg_glyph: ygGlyph) -> None:
         self.yg_glyph = yg_glyph
+        self.counter_clockwise = bool(self.yg_glyph.yg_font.defaults.get_default("counterclockwise"))
         self.contours = []
         contour = []
         points = yg_glyph.points()
         for p in points:
             contour.append(p)
             if p.end_of_contour:
                 self.contours.append(contour)
@@ -68,46 +69,70 @@
             prev_point function (to be supplied).
         """
         contour = self.which_contour(pt)
         next_point = self.next_point(pt, contour)
         this_x = pt.font_x
         next_x = next_point.font_x
         if next_x > this_x:
-            return "right"
+            if self.counter_clockwise:
+                return("left")
+            else:
+                return "right"
         elif this_x > next_x:
-            return "left"
+            if self.counter_clockwise:
+                return "right"
+            else:
+                return "left"
         # If the points are aligned on this axis we're probably at the end of a stem.
         prev_point = self.prev_point(pt, contour)
         prev_x = prev_point.font_x
         if prev_x < this_x:
-            return "right"
+            if self.counter_clockwise:
+                return("left")
+            else:
+                return "right"
         elif this_x < prev_x:
-            return "left"
+            if self.counter_clockwise:
+                return "right"
+            else:
+                return "left"
         return "same"
 
         
     def y_direction(self, pt: ygPoint) -> str:
         """ Find the y direction of a line or curve at the location of
             point pt. Returns "up," "down," or "same" if this pt
             has the same y location as the next pt.
         """
         contour = self.which_contour(pt)
         next_point = self.next_point(pt, contour)
         next_y = next_point.font_y
         this_y = pt.font_y
         if next_y > this_y:
-            return "up"
+            if self.counter_clockwise:
+                return "down"
+            else:
+                return "up"
         elif this_y > next_y:
-            return "down"
+            if self.counter_clockwise:
+                return "up"
+            else:
+                return "down"
         prev_point = self.prev_point(pt, contour)
         prev_y = prev_point.font_y
         if prev_y > this_y:
-            return "right"
+            if self.counter_clockwise:
+                return "up"
+            else:
+                return "down"
         elif this_y > prev_y:
-            return "left"
+            if self.counter_clockwise:
+                return "down"
+            else:
+                return "up"
         return "same"
         
     def get_color(self) -> str:
         """ Recommends a distance type for the stem formed by self.high_point
             and self.low_point, based on this class's analysis of the stem.
         """
         result = "graydist"
```

### Comparing `ygt-0.1.4/src/ygt/ygYAMLEditor.py` & `ygt-0.1.5/src/ygt/ygYAMLEditor.py`

 * *Files identical despite different names*

### Comparing `ygt-0.1.4/src/ygt.egg-info/PKG-INFO` & `ygt-0.1.5/src/ygt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ygt
-Version: 0.1.4
+Version: 0.1.5
 Summary: A graphical hint editor for TrueType fonts
 Author-email: "Peter S. Baker" <b.tarde@mail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10.4
 Description-Content-Type: text/markdown
```

### Comparing `ygt-0.1.4/src/ygt.egg-info/SOURCES.txt` & `ygt-0.1.5/src/ygt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

