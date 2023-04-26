# Comparing `tmp/conan-app-launcher-2.0.0b5.tar.gz` & `tmp/conan-app-launcher-2.0.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conan-app-launcher-2.0.0b5.tar", last modified: Thu Mar 30 20:02:21 2023, max compression
+gzip compressed data, was "conan-app-launcher-2.0.0b6.tar", last modified: Mon Apr  3 06:51:32 2023, max compression
```

## Comparing `conan-app-launcher-2.0.0b5.tar` & `conan-app-launcher-2.0.0b6.tar`

### file list

```diff
@@ -1,296 +1,298 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:02:21.071163 conan-app-launcher-2.0.0b5/
--rw-r--r--   0 runner    (1001) docker     (123)     7632 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7928 2023-03-30 20:02:21.071163 conan-app-launcher-2.0.0b5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6959 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:02:21.043162 conan-app-launcher-2.0.0b5/doc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:02:21.047162 conan-app-launcher-2.0.0b5/doc/example_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/doc/example_plugin/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:02:21.047162 conan-app-launcher-2.0.0b5/doc/example_plugin/cal_example_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/doc/example_plugin/cal_example_plugin/example.ui
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-03-30 20:02:21.071163 conan-app-launcher-2.0.0b5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:02:21.043162 conan-app-launcher-2.0.0b5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:02:21.047162 conan-app-launcher-2.0.0b5/src/conan_app_launcher/
--rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:02:21.047162 conan-app-launcher-2.0.0b5/src/conan_app_launcher/app/
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/app/crash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/app/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:02:21.047162 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/config_schema.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:02:21.047162 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/font/
--rw-r--r--   0 runner    (1001) docker     (123)   556216 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/font/NotoSans-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)  1593904 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/font/NotoSansMono.ttf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:02:21.051163 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/Readme.md
--rw-r--r--   0 runner    (1001) docker     (123)    33891 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/conan.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:02:21.055163 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/about.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/add_link.svg
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/app.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/arrow-down-svgrepo-com.svg
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/arrow_down.svg
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/arrow_up.svg
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/back.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/calendar-settings-svgrepo-com.svg
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/chevron-up-svgrepo-com.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/cleanup.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/close.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/code-svgrepo-com.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/copy.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/copy_link.svg
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/dark_mode.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/decrease_font.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/default_package.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/delete.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/document-search-svgrepo-com.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/download_pkg.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/edit.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/edit_file.svg
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/expand.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/file_explorer.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/file_preview.svg
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/forward.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/hide.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/increase_font.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/link-edit-svgrepo-com.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/link-svgrepo-com.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/login.svg
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/maximize.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/menu_stripes.svg
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/minus.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/no-access.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/opened_folder.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/package.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/paste.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/plugin.svg
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/plus.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/plus_rounded.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/rearrange.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/refresh.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/remove-lock.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/rename.svg
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/restore.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/save.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/search.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/settings.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/show.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/view.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:02:21.055163 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/global/
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/global/android.svg
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/global/conan_settings.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/global/grid.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/global/linux.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/global/mac_os.svg
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/global/package-svgrepo-com.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/global/package.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/global/package_explorer.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/global/search_packages.svg
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/global/windows.svg
--rw-r--r--   0 runner    (1001) docker     (123)     9561 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/icon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:02:21.063163 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/material/
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/material/about.svg
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/material/add_link.svg
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/material/app.svg
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/material/arrow_down.svg
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/material/arrow_up.svg
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/material/back.svg
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/material/border_color_FILL0_wght400_GRAD0_opsz48.svg
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/material/cleanup.svg
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/material/close.svg
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/material/cmd.svg
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/material/copy.svg
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/material/copy_link.svg
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/material/copy_to_clipboard.svg
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/material/cut.svg
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/material/dark_mode.svg
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/material/decrease_font.svg
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/material/default_pkg.svg
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/material/delete.svg
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/material/difference_FILL0_wght400_GRAD0_opsz48.svg
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/material/download.svg
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/material/download_pkg.svg
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/material/download_update.svg
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/material/edit.svg
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/material/edit_file.svg
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/material/expand.svg
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/material/expand_b.svg
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/material/expand_less_FILL0_wght400_GRAD0_opsz48.svg
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/material/expand_w.svg
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/material/file_explorer.svg
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/material/file_open_FILL0_wght400_GRAD0_opsz48.svg
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/material/file_preview.svg
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/material/forward.svg
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/material/forward_b.svg
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/material/forward_w.svg
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/material/hide.svg
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/material/increase_font.svg
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/material/lock_open_FILL0_wght400_GRAD0_opsz48.svg
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/material/login.svg
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/material/maximize.svg
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/material/menu_stripes.svg
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/material/minus.svg
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/material/move_up.svg
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/material/no-access.svg
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/material/opened_folder.svg
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/material/package.svg
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/material/paste.svg
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/material/plugin.svg
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/material/plus.svg
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/material/plus_rounded.svg
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/material/rearrange.svg
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/material/refresh.svg
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/material/remove-lock.svg
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/material/remove-lock2.svg
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/material/rename.svg
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/material/restore.svg
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/material/save.svg
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/material/search.svg
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/material/search_packages.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/material/settings.svg
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/material/show.svg
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/material/view.svg
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/launch.bat.in
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/launch.sh.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:02:21.063163 conan-app-launcher-2.0.0b5/src/conan_app_launcher/core/
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20844 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/core/conanV1.py
--rw-r--r--   0 runner    (1001) docker     (123)    13148 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/core/conanV2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9300 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/core/conan_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/core/conan_cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)    10211 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/core/conan_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     8520 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/core/conan_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)    10790 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/core/system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:02:21.063163 conan-app-launcher-2.0.0b5/src/conan_app_launcher/settings/
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9387 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/settings/ini_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:02:21.063163 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:02:21.067163 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/common/
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/common/icon.py
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/common/loading.py
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/common/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5062 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/common/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7852 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/common/theming.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:02:21.067163 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/config/
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/config/json_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    10929 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/dark_style.qss.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:02:21.067163 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/dialogs/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/dialogs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:02:21.067163 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/dialogs/conan_install/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/dialogs/conan_install/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/dialogs/conan_install/conan_install.py
--rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/dialogs/conan_install/conan_install.ui
--rw-r--r--   0 runner    (1001) docker     (123)     7895 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/dialogs/conan_install/conan_install_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/dialogs/conan_remove.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:02:21.067163 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/dialogs/crash/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/dialogs/crash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/dialogs/crash/crash.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/dialogs/crash/crash.ui
--rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/dialogs/crash/crash_ui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:02:21.067163 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/dialogs/file_editor_selection/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/dialogs/file_editor_selection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/dialogs/file_editor_selection/file_editor_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/dialogs/file_editor_selection/file_editor_selector.ui
--rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/dialogs/file_editor_selection/file_editor_selector_ui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:02:21.067163 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/dialogs/reorder_dialog/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/dialogs/reorder_dialog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/dialogs/reorder_dialog/reorder_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/dialogs/reorder_dialog/reorder_dialog.ui
--rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/dialogs/reorder_dialog/reorder_dialog_ui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:02:21.067163 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/fluent_window/
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/fluent_window/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22030 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/fluent_window/fluent_window.py
--rw-r--r--   0 runner    (1001) docker     (123)    42413 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/fluent_window/fluent_window.ui
--rw-r--r--   0 runner    (1001) docker     (123)    29239 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/fluent_window/fluent_window_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/fluent_window/side_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/fluent_window/side_menu.ui
--rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/fluent_window/side_menu_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     9202 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/light_style.qss.in
--rw-r--r--   0 runner    (1001) docker     (123)    14821 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/main_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:02:21.067163 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10753 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/plugin/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/plugins.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:02:21.067163 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:02:21.067163 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/about/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/about/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/about/about.ui
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/about/about_page.py
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/about/about_text.html
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/about/about_ui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:02:21.067163 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/app_grid/
--rw-r--r--   0 runner    (1001) docker     (123)    11643 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/app_grid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10548 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/app_grid/app_link.py
--rw-r--r--   0 runner    (1001) docker     (123)    14046 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/app_grid/app_link.ui
--rw-r--r--   0 runner    (1001) docker     (123)    13191 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/app_grid/app_link_ui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:02:21.071163 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/app_grid/dialogs/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/app_grid/dialogs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8113 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/app_grid/dialogs/app_edit_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     9924 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/app_grid/dialogs/app_edit_dialog.ui
--rw-r--r--   0 runner    (1001) docker     (123)    11450 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/app_grid/dialogs/app_edit_dialog_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)    18594 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/app_grid/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/app_grid/tab.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:02:21.071163 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/conan_conf/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/conan_conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15382 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/conan_conf/conan_conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    20920 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/conan_conf/conan_conf.ui
--rw-r--r--   0 runner    (1001) docker     (123)    22179 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/conan_conf/conan_conf_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/conan_conf/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:02:21.071163 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/conan_conf/dialogs/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/conan_conf/dialogs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/conan_conf/dialogs/remote_edit_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/conan_conf/dialogs/remote_edit_dialog.ui
--rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/conan_conf/dialogs/remote_edit_dialog_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/conan_conf/dialogs/remote_login_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     5725 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/conan_conf/dialogs/remote_login_dialog.ui
--rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/conan_conf/dialogs/remote_login_dialog_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/conan_conf/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:02:21.071163 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/conan_search/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/conan_search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7698 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/conan_search/conan_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    10976 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/conan_search/conan_search.ui
--rw-r--r--   0 runner    (1001) docker     (123)    11698 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/conan_search/conan_search_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/conan_search/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     9082 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/conan_search/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:02:21.071163 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/package_explorer/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/package_explorer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18228 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/package_explorer/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/package_explorer/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/package_explorer/package_explorer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8542 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/package_explorer/package_explorer.ui
--rw-r--r--   0 runner    (1001) docker     (123)     9197 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/package_explorer/package_explorer_ui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:02:21.071163 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/plugins_manager/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/plugins_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/plugins_manager/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/plugins_manager/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/plugins_manager/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/plugins_manager/plugins.ui
--rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/plugins_manager/plugins_ui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:02:21.071163 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/widgets/clickable_icon.py
--rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/widgets/conan_line_edit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/widgets/password_line_edit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/widgets/toggle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:02:21.047162 conan-app-launcher-2.0.0b5/src/conan_app_launcher.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7928 2023-03-30 20:02:20.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13967 2023-03-30 20:02:21.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 20:02:20.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-03-30 20:02:20.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-03-30 20:02:20.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-30 20:02:20.000000 conan-app-launcher-2.0.0b5/src/conan_app_launcher.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:02:21.047162 conan-app-launcher-2.0.0b5/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:02:21.047162 conan-app-launcher-2.0.0b5/test/testdata/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:02:21.047162 conan-app-launcher-2.0.0b5/test/testdata/settings/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:02:21.071163 conan-app-launcher-2.0.0b5/test/testdata/settings/read/
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/test/testdata/settings/read/config.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:02:21.071163 conan-app-launcher-2.0.0b5/test/testdata/settings/write/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-30 20:02:10.000000 conan-app-launcher-2.0.0b5/test/testdata/settings/write/config.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 06:51:32.435138 conan-app-launcher-2.0.0b6/
+-rw-r--r--   0 runner    (1001) docker     (123)     7632 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7928 2023-04-03 06:51:32.435138 conan-app-launcher-2.0.0b6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6959 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 06:51:32.411138 conan-app-launcher-2.0.0b6/doc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 06:51:32.415138 conan-app-launcher-2.0.0b6/doc/example_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/doc/example_plugin/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 06:51:32.415138 conan-app-launcher-2.0.0b6/doc/example_plugin/cal_example_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/doc/example_plugin/cal_example_plugin/example.ui
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-03 06:51:32.435138 conan-app-launcher-2.0.0b6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 06:51:32.411138 conan-app-launcher-2.0.0b6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 06:51:32.415138 conan-app-launcher-2.0.0b6/src/conan_app_launcher/
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 06:51:32.415138 conan-app-launcher-2.0.0b6/src/conan_app_launcher/app/
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/app/crash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/app/loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/app/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10628 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/app/system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 06:51:32.415138 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/config_schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 06:51:32.415138 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/font/
+-rw-r--r--   0 runner    (1001) docker     (123)   556216 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/font/NotoSans-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)  1593904 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/font/NotoSansMono.ttf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 06:51:32.419138 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)    33891 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/conan.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 06:51:32.423138 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/about.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/add_link.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/app.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/arrow-down-svgrepo-com.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/arrow_down.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/arrow_up.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/back.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/calendar-settings-svgrepo-com.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/chevron-up-svgrepo-com.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/cleanup.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/close.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/code-svgrepo-com.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/copy.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/copy_link.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/dark_mode.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/decrease_font.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/default_package.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/delete.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/document-search-svgrepo-com.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/download_pkg.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/edit.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/edit_file.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/expand.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/file_explorer.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/file_preview.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/forward.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/hide.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/increase_font.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/link-edit-svgrepo-com.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/link-svgrepo-com.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/login.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/maximize.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/menu_stripes.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/minus.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/no-access.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/opened_folder.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/package.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/paste.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/plugin.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/plus.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/plus_rounded.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/rearrange.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/refresh.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/remove-lock.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/rename.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/restore.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/save.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/search.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/settings.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/show.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/view.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 06:51:32.423138 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/global/
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/global/android.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/global/conan_settings.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/global/grid.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/global/linux.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/global/mac_os.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/global/package-svgrepo-com.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/global/package.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/global/package_explorer.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/global/search_packages.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/global/windows.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     9561 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/icon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 06:51:32.427138 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/material/
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/material/about.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/material/add_link.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/material/app.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/material/arrow_down.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/material/arrow_up.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/material/back.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/material/border_color_FILL0_wght400_GRAD0_opsz48.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/material/cleanup.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/material/close.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/material/cmd.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/material/copy.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/material/copy_link.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/material/copy_to_clipboard.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/material/cut.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/material/dark_mode.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/material/decrease_font.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/material/default_pkg.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/material/delete.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/material/difference_FILL0_wght400_GRAD0_opsz48.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/material/download.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/material/download_pkg.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/material/download_update.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/material/edit.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/material/edit_file.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/material/expand.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/material/expand_b.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/material/expand_less_FILL0_wght400_GRAD0_opsz48.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/material/expand_w.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/material/file_explorer.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/material/file_open_FILL0_wght400_GRAD0_opsz48.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/material/file_preview.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/material/forward.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/material/forward_b.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/material/forward_w.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/material/hide.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/material/increase_font.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/material/lock_open_FILL0_wght400_GRAD0_opsz48.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/material/login.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/material/maximize.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/material/menu_stripes.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/material/minus.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/material/move_up.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/material/no-access.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/material/opened_folder.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/material/package.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/material/paste.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/material/plugin.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/material/plus.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/material/plus_rounded.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/material/rearrange.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/material/refresh.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/material/remove-lock.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/material/remove-lock2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/material/rename.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/material/restore.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/material/save.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/material/search.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/material/search_packages.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/material/settings.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/material/show.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/material/view.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/launch.bat.in
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/launch.sh.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 06:51:32.427138 conan-app-launcher-2.0.0b6/src/conan_app_launcher/conan_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/conan_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21159 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/conan_wrapper/conanV1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13107 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/conan_wrapper/conanV2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9302 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/conan_wrapper/conan_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/conan_wrapper/conan_cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8354 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/conan_wrapper/conan_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10255 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/conan_wrapper/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 06:51:32.427138 conan-app-launcher-2.0.0b6/src/conan_app_launcher/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9440 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/settings/ini_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 06:51:32.427138 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 06:51:32.427138 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/common/icon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/common/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5062 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/common/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/common/syntax_highlighting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7851 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/common/theming.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 06:51:32.431138 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/config/json_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10929 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/dark_style.qss.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 06:51:32.431138 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/dialogs/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/dialogs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 06:51:32.431138 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/dialogs/conan_install/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/dialogs/conan_install/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8622 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/dialogs/conan_install/conan_install.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/dialogs/conan_install/conan_install.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     7895 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/dialogs/conan_install/conan_install_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/dialogs/conan_remove.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 06:51:32.431138 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/dialogs/crash/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/dialogs/crash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/dialogs/crash/crash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/dialogs/crash/crash.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/dialogs/crash/crash_ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 06:51:32.431138 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/dialogs/file_editor_selection/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/dialogs/file_editor_selection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/dialogs/file_editor_selection/file_editor_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/dialogs/file_editor_selection/file_editor_selector.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/dialogs/file_editor_selection/file_editor_selector_ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 06:51:32.431138 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/dialogs/reorder_dialog/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/dialogs/reorder_dialog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/dialogs/reorder_dialog/reorder_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/dialogs/reorder_dialog/reorder_dialog.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/dialogs/reorder_dialog/reorder_dialog_ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 06:51:32.431138 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/fluent_window/
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/fluent_window/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22029 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/fluent_window/fluent_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42413 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/fluent_window/fluent_window.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    29239 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/fluent_window/fluent_window_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/fluent_window/side_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/fluent_window/side_menu.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/fluent_window/side_menu_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9202 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/light_style.qss.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14796 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/main_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 06:51:32.431138 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10767 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/plugin/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/plugins.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 06:51:32.431138 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 06:51:32.431138 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/about/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/about/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/about/about.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/about/about_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/about/about_text.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/about/about_ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 06:51:32.431138 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/app_grid/
+-rw-r--r--   0 runner    (1001) docker     (123)    11645 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/app_grid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10551 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/app_grid/app_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14046 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/app_grid/app_link.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    13191 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/app_grid/app_link_ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 06:51:32.431138 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/app_grid/dialogs/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/app_grid/dialogs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8115 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/app_grid/dialogs/app_edit_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9924 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/app_grid/dialogs/app_edit_dialog.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    11450 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/app_grid/dialogs/app_edit_dialog_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18605 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/app_grid/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/app_grid/tab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 06:51:32.435138 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/conan_conf/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/conan_conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15221 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/conan_conf/conan_conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20538 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/conan_conf/conan_conf.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    21523 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/conan_conf/conan_conf_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/conan_conf/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 06:51:32.435138 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/conan_conf/dialogs/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/conan_conf/dialogs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/conan_conf/dialogs/remote_edit_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/conan_conf/dialogs/remote_edit_dialog.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/conan_conf/dialogs/remote_edit_dialog_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/conan_conf/dialogs/remote_login_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5725 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/conan_conf/dialogs/remote_login_dialog.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/conan_conf/dialogs/remote_login_dialog_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/conan_conf/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20992 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/conan_conf/ui_conan_conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 06:51:32.435138 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/conan_search/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/conan_search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7883 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/conan_search/conan_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11030 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/conan_search/conan_search.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    11118 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/conan_search/conan_search_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/conan_search/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9126 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/conan_search/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 06:51:32.435138 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/package_explorer/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/package_explorer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18286 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/package_explorer/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/package_explorer/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9496 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/package_explorer/package_explorer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9451 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/package_explorer/package_explorer.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/package_explorer/package_explorer_ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 06:51:32.435138 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/plugins_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/plugins_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/plugins_manager/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/plugins_manager/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/plugins_manager/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/plugins_manager/plugins.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/plugins_manager/plugins_ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 06:51:32.435138 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/widgets/clickable_icon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/widgets/conan_line_edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/widgets/password_line_edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/widgets/toggle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 06:51:32.415138 conan-app-launcher-2.0.0b6/src/conan_app_launcher.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7928 2023-04-03 06:51:32.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14132 2023-04-03 06:51:32.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 06:51:32.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-03 06:51:32.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-03 06:51:32.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-03 06:51:32.000000 conan-app-launcher-2.0.0b6/src/conan_app_launcher.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 06:51:32.411138 conan-app-launcher-2.0.0b6/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 06:51:32.411138 conan-app-launcher-2.0.0b6/test/testdata/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 06:51:32.411138 conan-app-launcher-2.0.0b6/test/testdata/settings/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 06:51:32.435138 conan-app-launcher-2.0.0b6/test/testdata/settings/read/
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/test/testdata/settings/read/config.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 06:51:32.435138 conan-app-launcher-2.0.0b6/test/testdata/settings/write/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-03 06:51:22.000000 conan-app-launcher-2.0.0b6/test/testdata/settings/write/config.ini
```

### Comparing `conan-app-launcher-2.0.0b5/LICENSE` & `conan-app-launcher-2.0.0b6/LICENSE`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/PKG-INFO` & `conan-app-launcher-2.0.0b6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conan-app-launcher
-Version: 2.0.0b5
+Version: 2.0.0b6
 Summary: App Launcher and Package Explorer for Conan
 Home-page: https://github.com/goszpeti/conan_app_launcher
 Author: Péter Gosztolya and Contributors
 License: LGPL v3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -19,15 +19,15 @@
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE
 
 
-# <img src="https://raw.githubusercontent.com/goszpeti/conan_app_launcher/v2.0.0b5/src/conan_app_launcher/assets/icons/icon.ico" width="128">
+# <img src="https://raw.githubusercontent.com/goszpeti/conan_app_launcher/v2.0.0b6/src/conan_app_launcher/assets/icons/icon.ico" width="128">
 
 # Conan App Launcher and Local Package Explorer
 
 ![https://pypi.org/project/conan-app-launcher/](https://img.shields.io/pypi/v/conan-app-launcher)
 ![PyPI Python versions](https://img.shields.io/pypi/pyversions/conan-app-launcher)
 ![MilestoneProgress](https://img.shields.io/github/milestones/progress-percent/goszpeti/conan_app_launcher/17)
 ![Python tests](https://github.com/goszpeti/conan_app_launcher/workflows/Python%20tests/badge.svg)
@@ -41,24 +41,24 @@
 * Browse the local package cache
 * Search Packages in remotes
 * Configure Remotes and Profiles
 
 It is end-user oriented and focuses on using packages, rather then developing them. It can be used on Windows and Linux x64 platforms.
 
 #### Application Link Grid
-# <img src="https://raw.githubusercontent.com/goszpeti/conan_app_launcher/v2.0.0b5/doc/screenshot.png" width="512">
+# <img src="https://raw.githubusercontent.com/goszpeti/conan_app_launcher/v2.0.0b6/doc/screenshot.png" width="512">
 
 #### Local Package Manager
-# <img src="https://raw.githubusercontent.com/goszpeti/conan_app_launcher/v2.0.0b5/doc/screenshot_pkg_explorer.png" width="512">
+# <img src="https://raw.githubusercontent.com/goszpeti/conan_app_launcher/v2.0.0b6/doc/screenshot_pkg_explorer.png" width="512">
 
 #### Conan Search
-# <img src="https://raw.githubusercontent.com/goszpeti/conan_app_launcher/v2.0.0b5/doc/screenshot_conan_search.png" width="512">
+# <img src="https://raw.githubusercontent.com/goszpeti/conan_app_launcher/v2.0.0b6/doc/screenshot_conan_search.png" width="512">
 
 #### Conan Config
-# <img src="https://raw.githubusercontent.com/goszpeti/conan_app_launcher/v2.0.0b5/doc/screenshot_conan_conf.png" width="512">
+# <img src="https://raw.githubusercontent.com/goszpeti/conan_app_launcher/v2.0.0b6/doc/screenshot_conan_conf.png" width="512">
 
 **Main Features**
 - compatible with a wide range of conan versions (from 1.24 onwards)
 - integrated console for information an packages and config file
 - installable with pip
 
 Quicklaunch
```

### Comparing `conan-app-launcher-2.0.0b5/README.md` & `conan-app-launcher-2.0.0b6/README.md`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/doc/example_plugin/cal_example_plugin/example.ui` & `conan-app-launcher-2.0.0b6/doc/example_plugin/cal_example_plugin/example.ui`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/setup.py` & `conan-app-launcher-2.0.0b6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         conan_major_version = "2"
     else:
         conan_major_version = "1"
     print(f"Using Conan version {conan_major_version} from spec: {conan_version_env}")
 
 # Package meta-data.
 NAME = "conan-app-launcher"
-VERSION = "2.0.0-beta5"
+VERSION = "2.0.0-beta6"
 DESCRIPTION = "App Launcher and Package Explorer for Conan"
 URL = "https://github.com/goszpeti/conan_app_launcher"
 AUTHOR = "Péter Gosztolya and Contributors"
 PYTHON_REQUIRES = ">=3.7.0"
 
 # What packages are required for this module to be executed?
 conan_req_spec = "conan>=1.24, <2.1"
```

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/__init__.py` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 """
 Contains all basic constants used in the application.
 No imports from own modules allowed! This is done to resolve circular dependencies.
 """
 import os
 import shutil
 import platform
-try: # from Python 3.8
+try:  # from Python 3.8
     from importlib.metadata import distribution, PackageNotFoundError
 except ImportError:
     from importlib_metadata import distribution, PackageNotFoundError  # type: ignore
-
 from pathlib import Path
 from typing import TypeVar
 
 PathLike = TypeVar("PathLike", str, Path)
 
 ### Global constants ###
 
@@ -22,34 +21,34 @@
 APP_NAME = "Conan Explorer"
 
 try:
     pkg_info = distribution(PKG_NAME)
     __version__ = pkg_info.version
     REPO_URL = pkg_info.metadata.get("home-page", "")  # type: ignore
     AUTHOR = pkg_info.metadata.get("author", "")  # type: ignore
-except PackageNotFoundError: # pragma: no cover
+except PackageNotFoundError:  # pragma: no cover
     # For local usecases, when there is no distribution
     __version__ = "1.0.0"
     REPO_URL = ""
     AUTHOR = ""
 
-ICON_SIZE = 64 # Icon size (width and height) in pixels on an Applink
+ICON_SIZE = 64  # Icon size (width and height) in pixels on an Applink
 MAX_FONT_SIZE = 16
 MIN_FONT_SIZE = 8
 INVALID_PATH = "Unknown"
-INVALID_CONAN_REF = "Invalid/0.0.1@NA/NA" # used to indicate a conan reference is invalid
-SETTINGS_FILE_NAME = "settings" # for storing application settings
+INVALID_CONAN_REF = "Invalid/0.0.1@NA/NA"  # used to indicate a conan reference is invalid
+SETTINGS_FILE_NAME = "settings"  # for storing application settings
 LEGACY_SETTINGS_FILE_NAME = ".cal_config"  # for backwards compatibility till 1.4.1
-DEFAULT_UI_CFG_FILE_NAME = "ui_cfg" # no extension from 1.4.1
+DEFAULT_UI_CFG_FILE_NAME = "ui_cfg"  # no extension from 1.4.1
 LEGACY_UI_CFG_FILE_NAME = "cal_ui.json"  # for backwards compatibility till 1.4.1
-CONAN_LOG_PREFIX = "CONAN: " # logger uses this to indicate a log comes from Conan
+CONAN_LOG_PREFIX = "CONAN: "  # logger uses this to indicate a log comes from Conan
 BUILT_IN_PLUGIN = "built-in"
 
 # Feature flags
-SEARCH_APP_VERSIONS_IN_LOCAL_CACHE = True # get versions directly from the custom cache
+SEARCH_APP_VERSIONS_IN_LOCAL_CACHE = True  # get versions directly from the custom cache
 USE_LOCAL_CACHE_FOR_LOCAL_PKG_PATH = True  # get pkg paths directly from the custom cache TODO can't handle options
 # use conan worker to also search for the package path - works in a addition to USE_LOCAL_CACHE_FOR_LOCAL_PKG_PATH and also installs
 USE_CONAN_WORKER_FOR_LOCAL_PKG_PATH_AND_INSTALL = True
 AUTOCLOSE_SIDE_MENU = False
 
 # From ennvar DEBUG - 0: No debug, 1 = debug logging on, 2 = disable true async loading
 DEBUG_LEVEL = int(os.getenv("CAL_DEBUG_LEVEL", "0"))
@@ -62,25 +61,25 @@
 # must be initialized later, otherwise setup.py can't parse this file
 
 base_path = Path(__file__).absolute().parent
 asset_path = base_path / "assets"
 # to be used for all default paths of configuration files, which will be used for multiple versions
 # noninvasive storage, legacy will be moved
 legacy_user_save_path = Path().home()
-user_save_path =  Path(os.getenv("XDG_CONFIG_HOME", str(legacy_user_save_path / ".config"))) / PKG_NAME if platform.system() == "Linux" \
+user_save_path = Path(os.getenv("XDG_CONFIG_HOME", str(legacy_user_save_path / ".config"))) / PKG_NAME if platform.system() == "Linux" \
     else Path(os.getenv("APPDATA", str(legacy_user_save_path))) / PKG_NAME
 
 # user path migration - move settings and default gui file
 # ui file loading will handle patching the settings, if the default gui file was used
 if user_save_path != legacy_user_save_path:
     os.makedirs(str(user_save_path), exist_ok=True)
     # don't copy if the migrated files already exist
     if (legacy_user_save_path / LEGACY_SETTINGS_FILE_NAME).exists() and \
-        not (user_save_path / (SETTINGS_FILE_NAME + ".ini")).exists():
+            not (user_save_path / (SETTINGS_FILE_NAME + ".ini")).exists():
         print(f"INFO: Moving application settings file from {str(user_save_path)} to {str(legacy_user_save_path)}")
         shutil.move(str(legacy_user_save_path / LEGACY_SETTINGS_FILE_NAME),
                     str(user_save_path / (SETTINGS_FILE_NAME + ".ini")))
     if (legacy_user_save_path / LEGACY_UI_CFG_FILE_NAME).exists() and \
-        not (user_save_path / (DEFAULT_UI_CFG_FILE_NAME + ".json")).exists():
+            not (user_save_path / (DEFAULT_UI_CFG_FILE_NAME + ".json")).exists():
         print(f"INFO: Moving default ui config file from {str(user_save_path)} to {str(legacy_user_save_path)}")
         shutil.move(str(legacy_user_save_path / LEGACY_UI_CFG_FILE_NAME),
                     str(user_save_path / (DEFAULT_UI_CFG_FILE_NAME + ".json")))
```

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/app/__init__.py` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/app/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,67 +1,79 @@
+from conan_app_launcher.conan_wrapper import ConanWorker, ConanApi
 import os
 import platform
 import sys
 
-from conan_app_launcher import APP_NAME, SETTINGS_FILE_NAME, __version__, asset_path, user_save_path
-from conan_app_launcher.core import ConanApi, ConanWorker
 from conan_app_launcher.settings import SETTINGS_INI_TYPE, SettingsInterface, settings_factory
+from conan_app_launcher import APP_NAME, SETTINGS_FILE_NAME, __version__, asset_path, user_save_path
 from .logger import Logger
 
-from PySide6 import QtCore, QtGui, QtWidgets
-
-
-if platform.system() == "Windows":
-    # Workaround for Windows, so that on the taskbar the
-    # correct icon will be shown (and not the default python icon).
-    from ctypes import windll  # Only exists on Windows.
-    MY_APP_ID = 'ConanAppLauncher.' + __version__
-    windll.shell32.SetCurrentProcessExplicitAppUserModelID(MY_APP_ID)
-
 ### Global variables ###
 
 active_settings: SettingsInterface = settings_factory(SETTINGS_INI_TYPE,
                                                       user_save_path / (SETTINGS_FILE_NAME + "." + SETTINGS_INI_TYPE))
-conan_api = ConanApi()
-conan_worker = ConanWorker(conan_api, active_settings)
+conan_api: "ConanApi"  # initialized by load_conan
+conan_worker: "ConanWorker"  # initialized by load_conan
+
 
 def run_application():
     """ Start the Qt application and load the main window """
     # Overwrite the excepthook with our own - this will provide a method to report bugs for the user
-    from conan_app_launcher.ui.common import activate_theme
 
-    if platform.system() == "Darwin":
+    if platform.system() == "Windows":
+        # Workaround for Windows, so that on the taskbar the
+        # correct icon will be shown (and not the default python icon).
+        from ctypes import windll  # Only exists on Windows.
+        MY_APP_ID = 'ConanAppLauncher.' + __version__
+        windll.shell32.SetCurrentProcessExplicitAppUserModelID(MY_APP_ID)
+    elif platform.system() == "Darwin":
         print("Mac OS is currently not supported.")
         sys.exit(1)
+    qt_app = load_qapp()
+    from .loading import AsyncLoader
+    loader = AsyncLoader(None)
+    loader.async_loading(None, load_conan, (), cancel_button=False)
+    loader.wait_for_finished()
+    from conan_app_launcher.ui.main_window import MainWindow
+    main_window = MainWindow(qt_app)
+    from PySide6 import QtGui
+    main_window.setWindowIcon(QtGui.QIcon(str(asset_path / "icons" / "icon.ico")))
+    main_window.show()  # show first, then load appsgrid with progress bar
+    main_window.load()
+    main_window.installEventFilter(main_window)
+
+    qt_app.exec()
+
+    main_window.save_window_state()
+    # cancel conan worker tasks on exit - this can possibly cancel an ongoing install task
+    if conan_worker:
+        conan_worker.finish_working(10)
+
 
+def load_conan():
+    global conan_api, conan_worker
+    from conan_app_launcher.conan_wrapper import ConanApi, ConanWorker
+    conan_api = ConanApi()
+    conan_worker = ConanWorker(conan_api, active_settings)
+    conan_api.init_api()
+
+
+def load_qapp():
     # apply Qt attributes (only possible before QApplication is created)
+    from PySide6 import QtCore, QtWidgets
 
     # to use icons in qss file
     QtCore.QDir.addSearchPath('icons', os.path.join(asset_path, 'icons'))
     # Passthrough seems to work well for high dpi scaling
     try:
         QtWidgets.QApplication.setHighDpiScaleFactorRoundingPolicy(
             QtCore.Qt.HighDpiScaleFactorRoundingPolicy.PassThrough)
     except Exception:
         Logger().debug("Can't set DPI Rounding")
     qt_app = QtWidgets.QApplication([])
     qt_app.setApplicationName(APP_NAME)
     qt_app.setApplicationDisplayName(APP_NAME)
     from .crash import bug_dialog_exc_hook
     sys.excepthook = bug_dialog_exc_hook  # dialog needs qt_app
+    from conan_app_launcher.ui.common import activate_theme
     activate_theme(qt_app)
-
-    from conan_app_launcher.ui.main_window import MainWindow
-    main_window = MainWindow(qt_app)
-    main_window.setWindowIcon(QtGui.QIcon(str(asset_path / "icons" / "icon.ico")))
-
-    conan_api.init_api()
-    main_window.show()  # show first, then load appsgrid with progress bar
-    main_window.load()
-    main_window.installEventFilter(main_window)
-
-    qt_app.exec()
-
-    main_window.save_window_state()
-    # cancel conan worker tasks on exit - this can possibly cancel an ongoing install task
-    if conan_worker:
-        conan_worker.finish_working(10)
+    return qt_app
```

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/app/crash.py` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/app/crash.py`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/app/logger.py` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/app/logger.py`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/config_schema.json` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/config_schema.json`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/font/NotoSans-Regular.ttf` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/font/NotoSans-Regular.ttf`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/font/NotoSansMono.ttf` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/font/NotoSansMono.ttf`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/Readme.md` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/Readme.md`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/conan.png` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/conan.png`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/about.svg` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/about.svg`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/add_link.svg` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/add_link.svg`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/arrow-down-svgrepo-com.svg` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/arrow-down-svgrepo-com.svg`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/arrow_down.svg` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/arrow_down.svg`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/arrow_up.svg` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/arrow_up.svg`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/back.svg` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/back.svg`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/calendar-settings-svgrepo-com.svg` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/calendar-settings-svgrepo-com.svg`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/chevron-up-svgrepo-com.svg` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/chevron-up-svgrepo-com.svg`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/cleanup.svg` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/cleanup.svg`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/close.svg` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/close.svg`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/code-svgrepo-com.svg` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/code-svgrepo-com.svg`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/copy.svg` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/copy.svg`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/copy_link.svg` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/copy_link.svg`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/dark_mode.svg` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/dark_mode.svg`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/decrease_font.svg` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/decrease_font.svg`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/default_package.svg` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/default_package.svg`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/delete.svg` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/delete.svg`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/document-search-svgrepo-com.svg` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/document-search-svgrepo-com.svg`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/download_pkg.svg` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/download_pkg.svg`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/edit.svg` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/edit.svg`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/edit_file.svg` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/edit_file.svg`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/expand.svg` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/expand.svg`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/file_explorer.svg` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/file_explorer.svg`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/file_preview.svg` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/file_preview.svg`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/forward.svg` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/forward.svg`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/hide.svg` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/hide.svg`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/increase_font.svg` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/increase_font.svg`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/link-edit-svgrepo-com.svg` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/link-edit-svgrepo-com.svg`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/link-svgrepo-com.svg` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/link-svgrepo-com.svg`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/login.svg` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/login.svg`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/maximize.svg` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/maximize.svg`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/menu_stripes.svg` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/menu_stripes.svg`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/minus.svg` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/minus.svg`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/no-access.svg` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/no-access.svg`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/opened_folder.svg` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/opened_folder.svg`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/package.svg` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/package.svg`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/paste.svg` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/paste.svg`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/plugin.svg` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/plugin.svg`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/plus.svg` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/plus.svg`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/plus_rounded.svg` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/plus_rounded.svg`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/rearrange.svg` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/rearrange.svg`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/refresh.svg` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/refresh.svg`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/remove-lock.svg` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/remove-lock.svg`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/rename.svg` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/rename.svg`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/restore.svg` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/restore.svg`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/save.svg` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/save.svg`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/search.svg` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/search.svg`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/settings.svg` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/settings.svg`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/show.svg` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/show.svg`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/fluent/view.svg` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/fluent/view.svg`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/global/android.svg` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/global/android.svg`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/global/grid.svg` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/global/grid.svg`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/global/linux.svg` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/global/linux.svg`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/global/mac_os.svg` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/global/mac_os.svg`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/global/package.svg` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/global/package.svg`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/global/package_explorer.svg` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/global/package_explorer.svg`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/global/search_packages.svg` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/global/search_packages.svg`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/global/windows.svg` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/global/windows.svg`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/icon.ico` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/icon.ico`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/material/about.svg` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/material/about.svg`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/material/cleanup.svg` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/material/cleanup.svg`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/material/cut.svg` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/material/cut.svg`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/material/file_preview.svg` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/material/file_preview.svg`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/material/hide.svg` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/material/hide.svg`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/material/no-access.svg` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/material/no-access.svg`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/material/plugin.svg` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/material/plugin.svg`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/material/plus_rounded.svg` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/material/plus_rounded.svg`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/material/remove-lock.svg` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/material/remove-lock.svg`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/material/remove-lock2.svg` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/material/remove-lock2.svg`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/material/search_packages.svg` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/material/search_packages.svg`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/material/settings.svg` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/material/settings.svg`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/material/show.svg` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/material/show.svg`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/assets/icons/material/view.svg` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/assets/icons/material/view.svg`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/core/conanV1.py` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/conan_wrapper/conanV1.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,46 +1,47 @@
+import os
 import platform
-import shutil
-import tempfile
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple
 
-from conan_app_launcher.core.conan_common import ConanPkg, ConanRef,PkgRef,  ConanUnifiedApi, LoggerWriter, create_key_value_pair_list
+from conan_app_launcher.conan_wrapper.types import ConanPkg, ConanRef, PkgRef,  ConanUnifiedApi, LoggerWriter, create_key_value_pair_list
 
 if TYPE_CHECKING:
     from conans.client.cache.remote_registry import Remote
     from .conan_cache import ConanInfoCache
+    from conans.client.conan_api import (ClientCache, ConanAPIV1, UserIO,
+                                         client_version)
 
-from conans.client.conan_api import (ClientCache, ConanAPIV1, UserIO,
-                                        client_version)
-from conans.client.output import ConanOutput
-from conans.errors import ConanException
+    from conans.client.output import ConanOutput
+    from conans.errors import ConanException
 
 try:
     from conans.util.windows import path_shortener
 except Exception:
     pass
 
 from conan_app_launcher import (CONAN_LOG_PREFIX, INVALID_CONAN_REF, INVALID_PATH,
                                 SEARCH_APP_VERSIONS_IN_LOCAL_CACHE, user_save_path)
 from conan_app_launcher.app.logger import Logger
 
+
 class ConanApi(ConanUnifiedApi):
     """ Wrapper around ConanAPIV1 """
 
     def __init__(self):
-        self.conan: ConanAPIV1
-        self.client_cache: ClientCache
+        self.conan: "ConanAPIV1"
+        self.client_cache: "ClientCache"
         self.info_cache: "ConanInfoCache"
-        self.client_version = client_version
         self._short_path_root = Path("Unknown")
 
     def init_api(self):
         """ Instantiate the internal Conan api. In some cases it needs to be instatiated anew. """
-        self.conan= ConanAPIV1(output=ConanOutput(LoggerWriter(
+        from conans.client.conan_api import (ClientCache, ConanAPIV1, UserIO)
+        from conans.client.output import ConanOutput
+        self.conan = ConanAPIV1(output=ConanOutput(LoggerWriter(
             Logger().info, CONAN_LOG_PREFIX), LoggerWriter(Logger().error, CONAN_LOG_PREFIX)))
         self.conan.user_io = UserIO(out=ConanOutput(LoggerWriter(
             Logger().info, CONAN_LOG_PREFIX), LoggerWriter(Logger().error, CONAN_LOG_PREFIX)))
         self.conan.create_app()
         self.conan.user_io.disable_input()  # error on inputs - nowhere to enter
         if self.conan.app:
             self.client_cache = self.conan.app.cache
@@ -70,54 +71,55 @@
             if include_disabled:
                 remotes = self.conan.remote_list()
             else:
                 remotes = self.client_cache.registry.load_remotes().values()
         except Exception as e:
             Logger().error(f"Error while reading remotes file: {str(e)}")
         return remotes
-    
+
     def get_profiles(self) -> List[str]:
         return self.conan.profile_list()
-    
-    def get_profile_settings(self, profile_name: str) -> Dict[str, str]: 
+
+    def get_profile_settings(self, profile_name: str) -> Dict[str, str]:
         profile = self.conan.read_profile(profile_name)
         if not profile:
             return {}
         return dict(profile.settings)
-    
+
     def get_profiles_with_settings(self) -> Dict[str, Dict[str, str]]:
         profiles_dict = {}
         for profile in self.get_profiles():
             profiles_dict[profile] = self.get_profile_settings(profile)
         return profiles_dict
 
-    def get_remote_user_info(self, remote_name: str) -> Tuple[str, bool]: # user_name, autheticated
+    def get_remote_user_info(self, remote_name: str) -> Tuple[str, bool]:  # user_name, autheticated
         user_info = self.conan.users_list(remote_name).get("remotes", {})
         if len(user_info) < 1:
             return ("", False)
         try:
             return (str(user_info[0].get("user_name", "")), user_info[0].get("authenticated", False))
         except Exception:
             Logger().warning(f"Can't get user info for {remote_name}")
             return ("", False)
 
     def get_short_path_root(self) -> Path:
         """ Return short path root for Windows. Sadly there is no built-in way to do  """
         # only need to get once
         if self._short_path_root.exists() or platform.system() != "Windows":
             return self._short_path_root
-        temp_dir = str(path_shortener(tempfile.mkdtemp(), True))
-        gen_short_path = Path(temp_dir)
-        short_path_root = gen_short_path.parents[1]
-        shutil.rmtree(gen_short_path.parent, ignore_errors=True)
-        return short_path_root
+        short_home = os.getenv("CONAN_USER_HOME_SHORT")
+        if not short_home:
+            drive = os.path.splitdrive(self.client_cache.cache_folder)[0].upper()
+            short_home = os.path.join(drive, os.sep, ".conan")
+        os.makedirs(short_home, exist_ok=True)
+        return Path(short_home)
 
     def get_package_folder(self, conan_ref: ConanRef, package_id: str) -> Path:
         """ Get the fully resolved package path from the reference and the specific package (id) """
-        if not package_id: # will give the base path ortherwise
+        if not package_id:  # will give the base path ortherwise
             return Path(INVALID_PATH)
         try:
             layout = self.client_cache.package_layout(conan_ref)
             return Path(layout.package(PkgRef(conan_ref, package_id)))
         except Exception:  # gotta catch 'em all!
             return Path(INVALID_PATH)
 
@@ -144,19 +146,20 @@
     def install_reference(self, conan_ref: ConanRef, conan_settings:  Dict[str, str] = {},
                           conan_options: Dict[str, str] = {}, update=True) -> Tuple[str, Path]:
         """
         Try to install a conan reference (without id) with the provided extra information.
         Uses plain conan install (No auto determination of best matching package)
         Returns the actual pkg_id and the package path.
         """
+        from conans.errors import ConanException
         pkg_id = ""
         options_list = create_key_value_pair_list(conan_options)
         settings_list = create_key_value_pair_list(conan_settings)
         Logger().info(
-            f"Installing '<b>{str(conan_ref)}</b>' with settings: {str(settings_list)}, " \
+            f"Installing '<b>{str(conan_ref)}</b>' with settings: {str(settings_list)}, "
             f"options: {str(options_list)} and update={update}\n")
         try:
             infos = self.conan.install_reference(
                 conan_ref, settings=settings_list, options=options_list, update=update)
             if not infos.get("error", True):
                 pkg_id = infos.get("installed", [{}])[0].get("packages", [{}])[0].get("id", "")
             Logger().info(f"Installation of '<b>{str(conan_ref)}</b>' finished")
@@ -166,19 +169,20 @@
             return (pkg_id, Path(INVALID_PATH))
 
     def install_package(self, conan_ref: ConanRef, package: ConanPkg, update=True) -> bool:
         """
         Try to install a conan package (id) with the provided extra information.
         Returns True, if installation was succesfull.
         """
+        from conans.errors import ConanException
         package_id = package.get("id", "")
         options_list = create_key_value_pair_list(package.get("options", {}))
         settings_list = create_key_value_pair_list(package.get("settings", {}))
         Logger().info(
-            f"Installing '<b>{str(conan_ref)}</b>':{package_id} with settings: {str(settings_list)}, " \
+            f"Installing '<b>{str(conan_ref)}</b>':{package_id} with settings: {str(settings_list)}, "
             f"options: {str(options_list)} and update={update}\n")
         try:
             self.conan.install_reference(conan_ref, update=update,
                                          settings=settings_list, options=options_list)
             Logger().info(f"Installation of '<b>{str(conan_ref)}</b>' finished")
             # Update cache with this package
             self.info_cache.update_local_package_path(
@@ -191,15 +195,16 @@
     def get_path_or_auto_install(self, conan_ref: ConanRef, conan_options: Dict[str, str] = {}, update=False) -> Tuple[str, Path]:
         """ Return the pkg_id and package folder of a conan reference 
         and auto-install it with the best matching package, if it is not available """
         if not update:
             pkg_id, path = self.get_best_matching_package_path(conan_ref, conan_options)
             if pkg_id:
                 return pkg_id, path
-            Logger().info(f"'<b>{conan_ref}</b>' with options {repr(conan_options)} is not installed. Searching for packages to install...")
+            Logger().info(
+                f"'<b>{conan_ref}</b>' with options {repr(conan_options)} is not installed. Searching for packages to install...")
 
         pkg_id, path = self.install_best_matching_package(conan_ref, conan_options, update=update)
         return pkg_id, path
 
     def install_best_matching_package(self, conan_ref: ConanRef,
                                       conan_options: Dict[str, str] = {}, update=False) -> Tuple[str, Path]:
         packages: List[ConanPkg] = self.get_matching_package_in_remotes(conan_ref, conan_options)
@@ -294,14 +299,15 @@
             return res_list
 
         for res in search_results:
             for item in res.get("items", []):
                 res_list.append(ConanRef.loads(item.get("recipe", {}).get("id", "")))
         res_list = list(set(res_list))  # make unique
         res_list.sort()
+        self.info_cache.update_remote_package_list(res_list)
         return res_list
 
     def search_recipe_alternatives_in_remotes(self, conan_ref: ConanRef) -> List[ConanRef]:
         """ Search in all remotes for all versions of a conan ref """
         search_results = []
         local_results = []
         try:
@@ -369,15 +375,16 @@
         # skip search on default invalid recipe
         if str(conan_ref) == INVALID_CONAN_REF:
             return []
 
         found_pkgs: List[ConanPkg] = []
         default_settings: Dict[str, str] = {}
         try:
-            default_settings = dict(self.client_cache.default_profile.settings)  # type: ignore - dynamic prop is ok in try-catch
+            # type: ignore - dynamic prop is ok in try-catch
+            default_settings = dict(self.client_cache.default_profile.settings)
             query = f"(arch=None OR arch={default_settings.get('arch')})" \
                     f" AND (arch_build=None OR arch_build={default_settings.get('arch_build')})" \
                     f" AND (os=None OR os={default_settings.get('os')})"\
                     f" AND (os_build=None OR os_build={default_settings.get('os_build')})"
             found_pkgs = self.get_packages_in_remote(conan_ref, remote, query)
         except Exception:  # no problem, next
             return []
@@ -429,8 +436,8 @@
             if same_comp_pkgs:
                 found_pkgs = same_comp_pkgs
 
             same_comp_version_pkgs = list(filter(lambda pkg: default_settings.get("compiler.version", "") ==
                                                  pkg.get("settings", {}).get("compiler.version", ""), found_pkgs))
             if same_comp_version_pkgs:
                 found_pkgs = same_comp_version_pkgs
-        return found_pkgs
+        return found_pkgs
```

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/core/conanV2.py` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/conan_wrapper/conanV2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 import os
 import inspect as python_inspect
 
 from pathlib import Path
 from typing import TYPE_CHECKING, Dict, List, Optional, Tuple
 
-from conan_app_launcher.core.conan_common import ConanPkg, ConanUnifiedApi
+from conan_app_launcher.conan_wrapper.types import ConanPkg, ConanUnifiedApi
 from conan_app_launcher.app.logger import Logger
 
 if TYPE_CHECKING:
     from conans.client.cache.remote_registry import Remote
     from .conan_cache import ConanInfoCache
 
 from conan.api.conan_api import ConanAPI, client_version
 from conans.client.cache.cache import ClientCache
 from conans.errors import ConanException
 from conan_app_launcher import (INVALID_CONAN_REF, INVALID_PATH,
                                 user_save_path)
-from conan_app_launcher.core.conan_common import ConanPkg, ConanRef, PkgRef,  ConanUnifiedApi, LoggerWriter, create_key_value_pair_list
+from conan_app_launcher.conan_wrapper.types import ConanPkg, ConanRef, PkgRef,  ConanUnifiedApi, LoggerWriter, create_key_value_pair_list
 
 class ConanApi(ConanUnifiedApi):
     """ Wrapper around ConanAPIV2 """
 
     def __init__(self):
         self.conan: ConanAPI
         self.client_cache: ClientCache
         self.info_cache: "ConanInfoCache"
-        self.client_version = client_version
         self._short_path_root = Path("Unknown")
 
     def init_api(self):
         self.conan = ConanAPI()
         self.client_cache = ClientCache(self.conan.cache_folder)
         from .conan_cache import ConanInfoCache
         self.info_cache = ConanInfoCache(user_save_path, self.get_all_local_refs())
```

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/core/conan_cache.py` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/conan_wrapper/conan_cache.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from multiprocessing import RLock
 import os
 from pathlib import Path
 from typing import Dict, List, Optional, Set, Tuple
 
 from conan_app_launcher import INVALID_CONAN_REF, INVALID_PATH, conan_version
 from conan_app_launcher.app.logger import Logger
-from conan_app_launcher.core.conan_common import ConanRef, ConanUnifiedApi
+from conan_app_launcher.conan_wrapper.types import ConanRef, ConanUnifiedApi
 
 class ConanInfoCache():
     """
     This is a cache to accelerate calls which need remote access.
     It also has an option to store the local package path.
     """
     CACHE_FILE_NAME = "cache.json"
```

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/core/conan_cleanup.py` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/conan_wrapper/conan_cleanup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,61 +1,61 @@
-from . import ConanApi
-from pathlib import Path
-import platform
-from typing import Set
-import conans
-from conan_app_launcher.app.logger import Logger
-
-class ConanCleanup():
-
-    def __init__(self, conan_api: ConanApi) -> None:
-        self._conan_api = conan_api
-        self.orphaned_references: Set[str] = set()
-        self.orphaned_packages: Set[str] = set()
-
-    def get_cleanup_cache_paths(self) -> Set[str]:
-        """ Get a list of orphaned short path and cache folders """
-        # Blessed are the users Microsoft products!
-        if platform.system() != "Windows" or conans.__version__.startswith("2"):
-            return set()
-        self.find_orphaned_references()
-        self.find_orphaned_packages()
-        return self.orphaned_references.union(self.orphaned_packages)
-
-    def find_orphaned_references(self):
-        from .conan_common import PackageEditableLayout
-        del_list = []
-        for ref in self._conan_api.client_cache.all_refs():
-            ref_cache = self._conan_api.client_cache.package_layout(ref)
-            try:
-                package_ids = ref_cache.package_ids()
-            except Exception:
-                package_ids = ref_cache.packages_ids()  # type: ignore - old API of Conan
-            for pkg_id in package_ids:
-                short_path_dir = self._conan_api.get_package_folder(ref, pkg_id)
-                pkg_id_dir = None
-                if not isinstance(ref_cache, PackageEditableLayout):
-                    pkg_id_dir = Path(ref_cache.packages()) / pkg_id
-                if not short_path_dir.exists():
-                    Logger().debug(f"Can't find {str(short_path_dir)} for {str(ref)}")
-                    if pkg_id_dir:
-                        del_list.append(str(pkg_id_dir))
-        self.orphaned_references = set(del_list)
-
-    def find_orphaned_packages(self):
-        """ Reverse search for orphaned packages on windows short paths """
-        from .conan_common import CONAN_REAL_PATH
-
-        del_list = []
-        short_path_folders = [f for f in self._conan_api.get_short_path_root().iterdir() if f.is_dir()]
-        for short_path in short_path_folders:
-            rp_file = short_path / CONAN_REAL_PATH
-            if rp_file.is_file():
-                with open(str(rp_file)) as fp:
-                    real_path = fp.read()
-                try:
-                    if not Path(real_path).is_dir():
-                        Logger().debug(f"Can't find {real_path} for {str(short_path)}")
-                        del_list.append(str(short_path))
-                except Exception:
-                    Logger().error(f"Can't read {CONAN_REAL_PATH} in {str(short_path)}")
-        self.orphaned_packages = set(del_list)
+from . import ConanApi
+from pathlib import Path
+import platform
+from typing import Set
+import conans
+from conan_app_launcher.app.logger import Logger
+
+class ConanCleanup():
+
+    def __init__(self, conan_api: ConanApi) -> None:
+        self._conan_api = conan_api
+        self.orphaned_references: Set[str] = set()
+        self.orphaned_packages: Set[str] = set()
+
+    def get_cleanup_cache_paths(self) -> Set[str]:
+        """ Get a list of orphaned short path and cache folders """
+        # Blessed are the users Microsoft products!
+        if platform.system() != "Windows" or conans.__version__.startswith("2"):
+            return set()
+        self.find_orphaned_references()
+        self.find_orphaned_packages()
+        return self.orphaned_references.union(self.orphaned_packages)
+
+    def find_orphaned_references(self):
+        from .types import PackageEditableLayout
+        del_list = []
+        for ref in self._conan_api.client_cache.all_refs():
+            ref_cache = self._conan_api.client_cache.package_layout(ref)
+            try:
+                package_ids = ref_cache.package_ids()
+            except Exception:
+                package_ids = ref_cache.packages_ids()  # type: ignore - old API of Conan
+            for pkg_id in package_ids:
+                short_path_dir = self._conan_api.get_package_folder(ref, pkg_id)
+                pkg_id_dir = None
+                if not isinstance(ref_cache, PackageEditableLayout):
+                    pkg_id_dir = Path(ref_cache.packages()) / pkg_id
+                if not short_path_dir.exists():
+                    Logger().debug(f"Can't find {str(short_path_dir)} for {str(ref)}")
+                    if pkg_id_dir:
+                        del_list.append(str(pkg_id_dir))
+        self.orphaned_references = set(del_list)
+
+    def find_orphaned_packages(self):
+        """ Reverse search for orphaned packages on windows short paths """
+        from .types import CONAN_REAL_PATH
+
+        del_list = []
+        short_path_folders = [f for f in self._conan_api.get_short_path_root().iterdir() if f.is_dir()]
+        for short_path in short_path_folders:
+            rp_file = short_path / CONAN_REAL_PATH
+            if rp_file.is_file():
+                with open(str(rp_file)) as fp:
+                    real_path = fp.read()
+                try:
+                    if not Path(real_path).is_dir():
+                        Logger().debug(f"Can't find {real_path} for {str(short_path)}")
+                        del_list.append(str(short_path))
+                except Exception:
+                    Logger().error(f"Can't read {CONAN_REAL_PATH} in {str(short_path)}")
+        self.orphaned_packages = set(del_list)
```

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/core/conan_common.py` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/conan_wrapper/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Dict, List
 from abc import ABC, abstractmethod
 from conan_app_launcher import conan_version
+
 if TYPE_CHECKING:
-    from typing import TypedDict, Protocol, TypeAlias
-    from conan_app_launcher.core.conan_cache import ConanInfoCache
+    from typing import TypedDict,  TypeAlias
+    from conan_app_launcher.conan_wrapper.conan_cache import ConanInfoCache
+    from conans.client.conan_api import ClientCache
 else:
     try:
         from typing import TypedDict, Protocol, TypeAlias
     except ImportError:
         from typing_extensions import TypedDict, Protocol, TypeAlias
 
 if conan_version.startswith("1"):
@@ -32,18 +34,18 @@
 
 
 class ConanUnifiedApi(ABC):
     """ 
     API abstraction to provide compatiblity betwwen ConanV1 and V2 APIs. 
     Functions, which are not yet implemented in ConanV2 are commented out, so static type checkers can work.
     """
-    
+
     def __init__(self) -> None:
         # no direct Conan API access!
-        self.client_cache: "ClientCache" # TODO: Abstract this
+        self.client_cache: "ClientCache"  # TODO: Abstract this
         self.info_cache: "ConanInfoCache"
         super().__init__()
 
     def init_api(self):
         """ Instantiate the internal Conan api. In some cases it needs to be instatiated anew. """
         raise NotImplementedError
 
@@ -52,15 +54,15 @@
     def remove_locks(self):
         """ Remove local cache locks (Currently for V1 only) """
         raise NotImplementedError
 
     def get_remotes(self, include_disabled=False) -> List[Remote]:
         """ Return a list of all remotes. """
         raise NotImplementedError
-    
+
     def get_profiles(self) -> List[str]:
         """ Return a list of all profiles """
         raise NotImplementedError
 
     # def get_remote_user_info(self, remote_name: str) -> Tuple[str, bool]:  # user_name, authenticated
     #     """ Get username and authenticated info for a remote. """
     #     raise NotImplementedError
@@ -215,16 +217,14 @@
         for item in [arch.lower(), comp_text, comp_toolset.lower(), bt.lower()]:
             if item:
                 alias += "_" + item
 
         return alias
 
 
-
-
 class ConanPkg(TypedDict, total=False):
     """ Dummy class to type conan returned package dicts """
 
     id: str
     options: Dict[str, str]
     settings: Dict[str, str]
     requires: List
```

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/core/conan_worker.py` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/conan_wrapper/conan_worker.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,168 +1,168 @@
-
-from queue import Queue
-from threading import Thread
-# this allows to use forward declarations to avoid circular imports
-from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple
-
-from conan_app_launcher.settings import SettingsInterface
-
-if TYPE_CHECKING:
-    from typing import TypedDict, Protocol
-    from ..core import ConanApi
-else:
-    try:
-        from typing import TypedDict, Protocol
-    except ImportError:
-        from typing_extensions import TypedDict, Protocol
-
-from conan_app_launcher import USE_CONAN_WORKER_FOR_LOCAL_PKG_PATH_AND_INSTALL
-from conan_app_launcher.app.logger import Logger
-from .conan_common import ConanRef, PkgRef
-
-class ConanWorkerElement(TypedDict):
-    ref_pkg_id: str  # format in <ref>:<id>. Id is optional. If id is used options, settings and auto_isntall is ignored
-    options: Dict[str, str]  # conan options with key-value pairs
-    settings: Dict[str, str]  # conan settings with key-value pairs
-    update: bool  # use -u flag for install
-    auto_install: bool  # automatically determine best matching package.
-
-
-class ConanWorkerResultCallback(Protocol):
-    def __call__(self, conan_ref: str, pkg_id: str) -> Any: ...
-
-class ConanWorker():
-    """ Sequential worker with a queue to execute conan install/version alternatives commands """
-    def __init__(self, conan_api: "ConanApi", settings: SettingsInterface):
-        self._conan_api = conan_api
-        self._conan_install_queue: Queue[Tuple[ConanWorkerElement,
-                                               Optional[ConanWorkerResultCallback]]] = Queue(maxsize=0)
-        self._conan_versions_queue: Queue[Tuple[ConanWorkerElement,
-                                                Optional[ConanWorkerResultCallback]]] = Queue(maxsize=0)
-        self._version_worker: Optional[Thread] = None
-        self._install_worker: Optional[Thread] = None
-        self._shutdown_requested = False  # internal flag to cancel worker on shutdown
-        self._settings = settings
-
-    def update_all_info(self, conan_elements: List[ConanWorkerElement],
-                        info_callback: Optional[ConanWorkerResultCallback]):
-        """ 
-        Starts the worker for all given elements. Should be called at start. 
-        info_signal is used to notify the caller, that the worker has finished for a given element.
-        Install and version workers use the same signal. To be able to identify, which package has been finished
-        the signal will send this info: tuple(conan_ref, pkg_id)
-        """
-        # fill up queue
-        for worker_element in conan_elements:
-            if USE_CONAN_WORKER_FOR_LOCAL_PKG_PATH_AND_INSTALL:
-                self._conan_install_queue.put((worker_element, info_callback))
-            # self._conan_versions_queue.put((worker_element, info_callback))
-
-        # start getting versions info in a separate thread in a bundled way to get better performance
-        self._start_install_worker()
-
-    def put_ref_in_version_queue(self, conan_element: ConanWorkerElement, info_callback: Optional[ConanWorkerResultCallback]):
-        self._conan_versions_queue.put((conan_element, info_callback))
-
-    def put_ref_in_install_queue(self, conan_element: ConanWorkerElement, info_callback: Optional[ConanWorkerResultCallback]):
-        """ Add a new entry to work on """
-        self._conan_install_queue.put((conan_element, info_callback))
-        self._start_install_worker()
-
-    def _start_install_worker(self):
-        """ Start worker, if it is not already started (can be called multiple times)"""
-        if not self._install_worker or not self._install_worker.is_alive():
-            self._install_worker = Thread(target=self._work_on_conan_install_queue,
-                                          name="ConanInstallWorker", daemon=True)
-            self._install_worker.start()
-
-    def _start_version_worker(self):
-        """ Start worker, if it is not already started (can be called multiple times)"""
-        if not self._version_worker or not self._version_worker.is_alive():
-            self._version_worker = Thread(target=self._work_on_conan_versions_queue,
-                                          name="ConanVersionWorker", daemon=True)
-            self._version_worker.start()
-
-    def _work_on_conan_install_queue(self):
-        """ Call conan install from queue """
-        info_callback = None
-        conan_ref = None
-        pkg_id = ""
-        while not self._shutdown_requested and not self._conan_install_queue.empty():
-            worker_element, info_callback = self._conan_install_queue.get()
-            ref_pkg_id = worker_element.get("ref_pkg_id", "")
-            conan_options = worker_element.get("options", {})
-            conan_settings = worker_element.get("settings", {})
-            pkg_id = ""
-            update = worker_element.get("update", False)
-            auto_install = worker_element.get("auto_install", True)
-            # package path will be updated in conan cache
-            try:
-                if ":" in ref_pkg_id:  # pkg ref
-                    pkg_ref = PkgRef.loads(ref_pkg_id)
-                    conan_ref = pkg_ref.ref
-                    pkg_id = pkg_ref.id
-                    package = self._conan_api.get_remote_pkg_from_id(pkg_ref)
-                    self._conan_api.install_package(pkg_ref.ref, package, update)
-                else:
-                    conan_ref = ConanRef.loads(ref_pkg_id)
-
-                    if auto_install:
-                        pkg_id, _ = self._conan_api.get_path_or_auto_install(conan_ref, conan_options, update)
-                    else:
-                        pkg_id, _ = self._conan_api.install_reference(conan_ref, conan_settings, conan_options, update=update)
-            except Exception as e:
-                try:
-                    self._conan_install_queue.task_done()
-                except ValueError:
-                    pass # don't care about calling too many times
-                continue
-            Logger().debug("Finish working on " + ref_pkg_id)
-            try:
-                self._conan_install_queue.task_done()
-            except ValueError:
-                pass  # don't care about calling too many times
-            if USE_CONAN_WORKER_FOR_LOCAL_PKG_PATH_AND_INSTALL:
-                if info_callback and not self._shutdown_requested:
-                    try:
-                        info_callback(self._conan_api.generate_canonical_ref(conan_ref), pkg_id)
-                    except Exception as e:
-                        Logger().error(str(e))
-
-    def _work_on_conan_versions_queue(self):
-        """ Get all version and channel combination of a package from all remotes. """
-        info_callback = None
-        conan_ref = ""
-        while not self._shutdown_requested and not self._conan_versions_queue.empty():
-            _, info_callback = self._conan_versions_queue.get()
-            # available versions will be in cache and retrievable for every item from there
-            try:
-                available_refs = self._conan_api.search_recipe_alternatives_in_remotes(
-                    ConanRef.loads(conan_ref))
-            except Exception as e:
-                Logger().debug(f"ERROR in searching for {conan_ref}: {str(e)}")
-                continue
-            Logger().debug(f"Finished available package query for {str(conan_ref)}")
-            if not available_refs:
-                continue
-        if info_callback and not self._shutdown_requested:
-            try:
-                info_callback(conan_ref, "")
-            except Exception as e:
-                Logger().error(str(e))
-
-    def finish_working(self, timeout_s: Optional[float]=None):
-        """ Cancel, if worker is still not finished """
-        self._shutdown_requested = True
-        try:
-            if self._install_worker and self._install_worker.is_alive():
-                self._install_worker.join(timeout_s)
-        except Exception:
-            return  # Conan threads can crash on join
-        try:
-            if self._version_worker and self._version_worker.is_alive():
-                self._version_worker.join(timeout_s)
-        except Exception:
-            return  # Conan threads can crash on join
-        self._conan_install_queue = Queue(maxsize=0)
-        self._install_worker = None  # reset thread for later instantiation
-        self._shutdown_requested = False
+
+from queue import Queue
+from threading import Thread
+# this allows to use forward declarations to avoid circular imports
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple
+
+from conan_app_launcher.settings import SettingsInterface
+
+if TYPE_CHECKING:
+    from typing import TypedDict, Protocol
+    from ..conan_wrapper import ConanApi
+else:
+    try:
+        from typing import TypedDict, Protocol
+    except ImportError:
+        from typing_extensions import TypedDict, Protocol
+
+from conan_app_launcher import USE_CONAN_WORKER_FOR_LOCAL_PKG_PATH_AND_INSTALL
+from conan_app_launcher.app.logger import Logger
+from .types import ConanRef, PkgRef
+
+class ConanWorkerElement(TypedDict):
+    ref_pkg_id: str  # format in <ref>:<id>. Id is optional. If id is used options, settings and auto_isntall is ignored
+    options: Dict[str, str]  # conan options with key-value pairs
+    settings: Dict[str, str]  # conan settings with key-value pairs
+    update: bool  # use -u flag for install
+    auto_install: bool  # automatically determine best matching package.
+
+
+class ConanWorkerResultCallback(Protocol):
+    def __call__(self, conan_ref: str, pkg_id: str) -> Any: ...
+
+class ConanWorker():
+    """ Sequential worker with a queue to execute conan install/version alternatives commands """
+    def __init__(self, conan_api: "ConanApi", settings: SettingsInterface):
+        self._conan_api = conan_api
+        self._conan_install_queue: Queue[Tuple[ConanWorkerElement,
+                                               Optional[ConanWorkerResultCallback]]] = Queue(maxsize=0)
+        self._conan_versions_queue: Queue[Tuple[ConanWorkerElement,
+                                                Optional[ConanWorkerResultCallback]]] = Queue(maxsize=0)
+        self._version_worker: Optional[Thread] = None
+        self._install_worker: Optional[Thread] = None
+        self._shutdown_requested = False  # internal flag to cancel worker on shutdown
+        self._settings = settings
+
+    def update_all_info(self, conan_elements: List[ConanWorkerElement],
+                        info_callback: Optional[ConanWorkerResultCallback]):
+        """ 
+        Starts the worker for all given elements. Should be called at start. 
+        info_signal is used to notify the caller, that the worker has finished for a given element.
+        Install and version workers use the same signal. To be able to identify, which package has been finished
+        the signal will send this info: tuple(conan_ref, pkg_id)
+        """
+        # fill up queue
+        for worker_element in conan_elements:
+            if USE_CONAN_WORKER_FOR_LOCAL_PKG_PATH_AND_INSTALL:
+                self._conan_install_queue.put((worker_element, info_callback))
+            # self._conan_versions_queue.put((worker_element, info_callback))
+
+        # start getting versions info in a separate thread in a bundled way to get better performance
+        self._start_install_worker()
+
+    def put_ref_in_version_queue(self, conan_element: ConanWorkerElement, info_callback: Optional[ConanWorkerResultCallback]):
+        self._conan_versions_queue.put((conan_element, info_callback))
+
+    def put_ref_in_install_queue(self, conan_element: ConanWorkerElement, info_callback: Optional[ConanWorkerResultCallback]):
+        """ Add a new entry to work on """
+        self._conan_install_queue.put((conan_element, info_callback))
+        self._start_install_worker()
+
+    def _start_install_worker(self):
+        """ Start worker, if it is not already started (can be called multiple times)"""
+        if not self._install_worker or not self._install_worker.is_alive():
+            self._install_worker = Thread(target=self._work_on_conan_install_queue,
+                                          name="ConanInstallWorker", daemon=True)
+            self._install_worker.start()
+
+    def _start_version_worker(self):
+        """ Start worker, if it is not already started (can be called multiple times)"""
+        if not self._version_worker or not self._version_worker.is_alive():
+            self._version_worker = Thread(target=self._work_on_conan_versions_queue,
+                                          name="ConanVersionWorker", daemon=True)
+            self._version_worker.start()
+
+    def _work_on_conan_install_queue(self):
+        """ Call conan install from queue """
+        info_callback = None
+        conan_ref = None
+        pkg_id = ""
+        while not self._shutdown_requested and not self._conan_install_queue.empty():
+            worker_element, info_callback = self._conan_install_queue.get()
+            ref_pkg_id = worker_element.get("ref_pkg_id", "")
+            conan_options = worker_element.get("options", {})
+            conan_settings = worker_element.get("settings", {})
+            pkg_id = ""
+            update = worker_element.get("update", False)
+            auto_install = worker_element.get("auto_install", True)
+            # package path will be updated in conan cache
+            try:
+                if ":" in ref_pkg_id:  # pkg ref
+                    pkg_ref = PkgRef.loads(ref_pkg_id)
+                    conan_ref = pkg_ref.ref
+                    pkg_id = pkg_ref.id
+                    package = self._conan_api.get_remote_pkg_from_id(pkg_ref)
+                    self._conan_api.install_package(pkg_ref.ref, package, update)
+                else:
+                    conan_ref = ConanRef.loads(ref_pkg_id)
+
+                    if auto_install:
+                        pkg_id, _ = self._conan_api.get_path_or_auto_install(conan_ref, conan_options, update)
+                    else:
+                        pkg_id, _ = self._conan_api.install_reference(conan_ref, conan_settings, conan_options, update=update)
+            except Exception as e:
+                try:
+                    self._conan_install_queue.task_done()
+                except ValueError:
+                    pass # don't care about calling too many times
+                continue
+            Logger().debug("Finish working on " + ref_pkg_id)
+            try:
+                self._conan_install_queue.task_done()
+            except ValueError:
+                pass  # don't care about calling too many times
+            if USE_CONAN_WORKER_FOR_LOCAL_PKG_PATH_AND_INSTALL:
+                if info_callback and not self._shutdown_requested:
+                    try:
+                        info_callback(self._conan_api.generate_canonical_ref(conan_ref), pkg_id)
+                    except Exception as e:
+                        Logger().error(str(e))
+
+    def _work_on_conan_versions_queue(self):
+        """ Get all version and channel combination of a package from all remotes. """
+        info_callback = None
+        conan_ref = ""
+        while not self._shutdown_requested and not self._conan_versions_queue.empty():
+            _, info_callback = self._conan_versions_queue.get()
+            # available versions will be in cache and retrievable for every item from there
+            try:
+                available_refs = self._conan_api.search_recipe_alternatives_in_remotes(
+                    ConanRef.loads(conan_ref))
+            except Exception as e:
+                Logger().debug(f"ERROR in searching for {conan_ref}: {str(e)}")
+                continue
+            Logger().debug(f"Finished available package query for {str(conan_ref)}")
+            if not available_refs:
+                continue
+        if info_callback and not self._shutdown_requested:
+            try:
+                info_callback(conan_ref, "")
+            except Exception as e:
+                Logger().error(str(e))
+
+    def finish_working(self, timeout_s: Optional[float]=None):
+        """ Cancel, if worker is still not finished """
+        self._shutdown_requested = True
+        try:
+            if self._install_worker and self._install_worker.is_alive():
+                self._install_worker.join(timeout_s)
+        except Exception:
+            return  # Conan threads can crash on join
+        try:
+            if self._version_worker and self._version_worker.is_alive():
+                self._version_worker.join(timeout_s)
+        except Exception:
+            return  # Conan threads can crash on join
+        self._conan_install_queue = Queue(maxsize=0)
+        self._install_worker = None  # reset thread for later instantiation
+        self._shutdown_requested = False
```

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/core/system.py` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/app/system.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,275 +1,282 @@
-""" OS Abstraction Layer for all file based functions """
-
-import os
-import platform
-import shutil
-import subprocess
-import sys
-from contextlib import contextmanager
-# TODO find replacements for deprecated distutils functions
-from distutils.dir_util import copy_tree, remove_tree
-from distutils.file_util import copy_file
-from pathlib import Path
-from typing import List
-
-from conan_app_launcher import INVALID_PATH, PKG_NAME, asset_path
-from conan_app_launcher.app.logger import Logger
-from jinja2 import Template
-from packaging import version
-
-WIN_EXE_FILE_TYPES = [".cmd", ".com", ".bat", ".ps1", ".exe"]
-
-
-@contextmanager
-def escape_venv():
-    # don't do this while testing! if it errors or the gui is closed, while this is running,
-    #  the whole testrun will be compromised!
-    if os.getenv("PYTEST_CURRENT_TEST"):
-        yield
-    if os.getenv("PYTEST_CURRENT_TEST"):
-        return
-    path_var = os.environ.get("PATH", "")
-    bin_path = Path(sys.executable).parent
-    import re
-    path_regex = re.compile(re.escape(str(bin_path)), re.IGNORECASE)
-    new_path_var = path_regex.sub('', path_var)
-    apply_vars = {"PATH": new_path_var}
-    old_env = dict(os.environ)
-    os.environ.update(apply_vars)
-    try:
-        yield
-    finally:
-        os.environ.clear()
-        os.environ.update(old_env)
-
-
-def is_windows_11():
-    """ Main version number is still 10 - thanks MS! """
-    if platform.system() == "Windows" and version.parse(platform.version()) >= version.parse("10.0.22000"):
-        return True
-    return False
-
-
-def run_file(file_path: Path, is_console_app: bool, args: str):
-    """ Decide, if a file should be opened or executed and call the appropriate method """
-    if not file_path.is_file():
-        return
-    try:
-        if is_file_executable(file_path):
-            execute_app(file_path, is_console_app, args)
-        else:
-            open_file(file_path)
-    except Exception:
-        Logger().error(f"Error while executing {str(file_path)} with args: {args}.")
-
-
-def open_in_file_manager(file_path: Path):
-    """ Show file in file manager. """
-    try:
-        if platform.system() == "Linux":
-            # no standardized select functionailty.
-            # However xdg-open on a dir will open the folder in the default file explorer.
-            dir_to_view = file_path.parent if file_path.is_file() else file_path
-            return subprocess.Popen(("xdg-open", str(dir_to_view)))
-        elif platform.system() == "Windows":
-            # select switch for highlighting
-            creationflags = 0
-            if version.parse(platform.python_version()) >= version.parse("3.7.0"):
-                creationflags = subprocess.CREATE_NO_WINDOW  # available since 3.7
-            return subprocess.Popen("explorer /select," + str(file_path), creationflags=creationflags)
-    except Exception as e:
-        Logger().error(f"Can't show path in file-manager: {str(e)}")
-
-def open_cmd_in_path(file_path: Path) -> int:
-    """ Open a terminal in the selected folder. """
-    try:
-        if platform.system() == "Linux":
-            return execute_cmd(["x-terminal-emulator", "-e", '"', "cd", f"{str(file_path)}", "&&", "bash", '"'], True)
-        elif platform.system() == "Windows":
-            cmd_path = shutil.which("cmd")
-            if cmd_path:
-                return execute_app(Path(cmd_path), True, f"/k cd {str(file_path)}")
-        return 0
-    except Exception as e:
-        Logger().error(f"Can't open cmd in path: {str(e)}")
-        return 0
-
-def is_file_executable(file_path: Path) -> bool:
-    """ Checking execution mode is ok on linux, but not enough on windows, since every file with an associated
-     program has this flag. Use custom pathext lists to determine executable file extensions. """
-    is_executable = False
-    if platform.system() == "Linux":
-        if os.access(str(file_path), os.X_OK):
-            is_executable = True
-    elif platform.system() == "Windows":
-        # don't use PATHEXT - some programs write other filetypes like .py in it...
-        path_exts = WIN_EXE_FILE_TYPES
-        if file_path.suffix in path_exts:
-            is_executable = True
-    return is_executable
-
-
-def execute_app(executable: Path, is_console_app: bool, args: str) -> int:
-    """
-    Executes an application with args and optionally spawns a new shell
-    as specified in the app entry.
-    Returns the pid of the new process.
-    """
-    if executable.absolute().is_file():
-        cmd = [str(executable)]
-        if args:
-            cmd += args.strip().split(" ")
-        return execute_cmd(cmd, is_console_app)
-    Logger().warning(f"No executable {str(executable)} to start.")
-    return 0
-
-
-def execute_cmd(cmd: List[str], is_console_app: bool) -> int:
-    """ Generic process execute method. Returns pid. """
-    command_path = Path(cmd[0]).parent
-    try:
-        # Linux call errors on creationflags argument, so the calls must be separated
-        if platform.system() == "Windows":
-            creationflags = 0
-            if is_console_app:
-                creationflags = subprocess.CREATE_NEW_CONSOLE
-                cmd = [generate_launch_script(cmd)]
-            # don't use 'executable' arg of Popen, because then shell scripts won't execute correctly
-            proc = subprocess.Popen(cmd, creationflags=creationflags, cwd=str(command_path))
-            return proc.pid
-        elif platform.system() == "Linux":
-            if is_console_app:
-                # Sadly, there is no default way to do this, because of the miriad terminal emulators available
-                # Use the default distro emulator, with x-terminal-emulator
-                # (sudo update-alternatives --config x-terminal-emulator)
-                # This works only on debian distros.
-                cmd = [generate_launch_script(cmd)]
-                cmd = ["x-terminal-emulator", "-e"] + cmd
-            proc = subprocess.Popen(cmd, cwd=str(command_path))
-            return proc.pid
-        return 0
-    except Exception as e:
-        Logger().error(f"Can't execute cmd: {str(e)}")
-        return 0
-
-def generate_launch_script(cmd: List[str]) -> str:
-    import tempfile
-    launch_templ_file = ""
-
-    if platform.system() == 'Windows':
-        launch_templ_file = "launch.bat.in"
-        temp_fd, temp_path_str = tempfile.mkstemp(".bat", prefix=PKG_NAME, text=True)
-    elif platform.system() == "Linux":
-        launch_templ_file = "launch.sh.in"
-        temp_fd, temp_path_str = tempfile.mkstemp(".sh", prefix=PKG_NAME, text=True)
-    else:
-        Logger().warning(f"Not supported OS.")
-        return ""
-    launch_templ_path = asset_path / launch_templ_file
-    with open(launch_templ_path, "r") as fd:
-        launch_template = Template(fd.read())
-    launch_content = launch_template.render(COMMAND=" ".join(cmd))
-    with os.fdopen(temp_fd, 'w') as f:
-        f.write(launch_content)
-    if platform.system() == 'Linux':
-        os.system(f"chmod +x {temp_path_str}")
-    return temp_path_str
-
-
-def open_file(file: Path):
-    """ Open files with their associated programs """
-    try:
-        if file.absolute().is_file():
-            if platform.system() == 'Windows':
-                os.startfile(str(file))
-            elif platform.system() == "Linux":
-                subprocess.Popen(("xdg-open", str(file)))
-    except Exception as e:
-        Logger().error(f"Can't open file: {str(e)}")
-        return 0
-
-def delete_path(dst: Path):
-    """
-    Delete file or (non-empty) folder recursively. 
-    Exceptions will be caught and message logged to stdout.
-    """
-    try:
-        if dst.is_file():
-            os.remove(dst)
-        elif dst.is_dir():
-            remove_tree(str(dst), verbose=1)
-    except Exception as e:
-        Logger().warning(f"Can't delete {str(dst)}: {str(e)}")
-
-
-def copy_path_with_overwrite(src: Path, dst: Path):
-    """
-    Copy files/directories while overwriting possible files and adding missing ones.
-    Directories will be copied from under source, so you may need to add the orig. folder name, if you want that!
-    Exceptions will be caught and message logged to stdout.
-    """
-    try:
-        if src.is_file():
-            copy_file(str(src), str(dst))
-        else:
-            copy_tree(str(src), str(dst))
-    except Exception as e:
-        Logger().warning(f"Can't copy {str(src)} to {str(dst)}: {str(e)}")
-
-
-def calc_paste_same_dir_name(dst: Path, index=1):
-    """
-    Create a name for a file like /file.txt -> /file (2).txt.
-    It will find the next empty number.
-    If a file with a higher number exists it will ignore it.
-    """
-    if dst.exists():
-        new_path = dst.with_name(f"{dst.stem} ({str(index+1)}){dst.suffix}")
-        possible_path = calc_paste_same_dir_name(new_path, index+1)
-        if possible_path == Path(INVALID_PATH):
-            return new_path
-        else:
-            return dst
-    else:
-        if index == 1:  # if file does not exist
-            return dst
-        return Path(INVALID_PATH)
-
-def get_default_file_editor():
-    if platform.system() == "Windows":
-        editor_executable = find_program_in_windows("Notepad++", partial_match=True, key_to_find="DisplayIcon")
-        if Path(editor_executable).exists():
-            return editor_executable
-        return "notepad.exe"
-    else:
-        return "gedit" # distro dependent, but make something
-
-
-def find_program_in_windows(app_name: str, partial_match=False, key_to_find="InstallLocation") -> str:
-    if platform.system() != "Windows":
-        return ""
-
-    import winreg
-    arch_keys = {winreg.KEY_WOW64_32KEY, winreg.KEY_WOW64_64KEY}
-    for arch_key in arch_keys:
-        key = winreg.OpenKey(winreg.HKEY_LOCAL_MACHINE, 
-                r"SOFTWARE\Microsoft\Windows\CurrentVersion\Uninstall", 0, winreg.KEY_READ | arch_key)
-        for i in range(0, winreg.QueryInfoKey(key)[0]):
-            sub_key_name = winreg.EnumKey(key, i)
-            sub_key = winreg.OpenKey(key, sub_key_name)
-            try:
-                current_app_name = winreg.QueryValueEx(sub_key, "DisplayName")[0]
-                if partial_match:
-                    if app_name in current_app_name:
-                        location = winreg.QueryValueEx(sub_key, key_to_find)[0]
-                        return location
-                if app_name == current_app_name:
-                    location = winreg.QueryValueEx(sub_key, key_to_find)[0]
-                    return location
-            except OSError:
-                pass
-            finally:
-                sub_key.Close()
-    return ""
-
-
+""" OS Abstraction Layer for all file based functions """
+
+import os
+import platform
+import shutil
+import subprocess
+import sys
+from contextlib import contextmanager
+
+from pathlib import Path
+from typing import List
+
+from conan_app_launcher import INVALID_PATH, PKG_NAME, asset_path
+from conan_app_launcher.app.logger import Logger
+
+WIN_EXE_FILE_TYPES = [".cmd", ".com", ".bat", ".ps1", ".exe"]
+
+
+@contextmanager
+def escape_venv():
+    # don't do this while testing! if it errors or the gui is closed, while this is running,
+    #  the whole testrun will be compromised!
+    if os.getenv("PYTEST_CURRENT_TEST"):
+        yield
+    if os.getenv("PYTEST_CURRENT_TEST"):
+        return
+    path_var = os.environ.get("PATH", "")
+    bin_path = Path(sys.executable).parent
+    import re
+    path_regex = re.compile(re.escape(str(bin_path)), re.IGNORECASE)
+    new_path_var = path_regex.sub('', path_var)
+    apply_vars = {"PATH": new_path_var}
+    old_env = dict(os.environ)
+    os.environ.update(apply_vars)
+    try:
+        yield
+    finally:
+        os.environ.clear()
+        os.environ.update(old_env)
+
+
+def is_windows_11():
+    """ Main version number is still 10 - thanks MS! """
+    from packaging import version
+    if platform.system() == "Windows" and version.parse(platform.version()) >= version.parse("10.0.22000"):
+        return True
+    return False
+
+
+def run_file(file_path: Path, is_console_app: bool, args: str):
+    """ Decide, if a file should be opened or executed and call the appropriate method """
+    if not file_path.is_file():
+        return
+    try:
+        if is_file_executable(file_path):
+            execute_app(file_path, is_console_app, args)
+        else:
+            open_file(file_path)
+    except Exception:
+        Logger().error(f"Error while executing {str(file_path)} with args: {args}.")
+
+
+def open_in_file_manager(file_path: Path):
+    """ Show file in file manager. """
+    try:
+        if platform.system() == "Linux":
+            # no standardized select functionailty.
+            # However xdg-open on a dir will open the folder in the default file explorer.
+            dir_to_view = file_path.parent if file_path.is_file() else file_path
+            return subprocess.Popen(("xdg-open", str(dir_to_view)))
+        elif platform.system() == "Windows":
+            # select switch for highlighting
+            creationflags = 0
+            from packaging import version
+            if version.parse(platform.python_version()) >= version.parse("3.7.0"):
+                creationflags = subprocess.CREATE_NO_WINDOW  # available since 3.7
+            return subprocess.Popen("explorer /select," + str(file_path), creationflags=creationflags)
+    except Exception as e:
+        Logger().error(f"Can't show path in file-manager: {str(e)}")
+
+
+def open_cmd_in_path(file_path: Path) -> int:
+    """ Open a terminal in the selected folder. """
+    try:
+        if platform.system() == "Linux":
+            return execute_cmd(["x-terminal-emulator", "-e", '"', "cd", f"{str(file_path)}", "&&", "bash", '"'], True)
+        elif platform.system() == "Windows":
+            cmd_path = shutil.which("cmd")
+            if cmd_path:
+                return execute_app(Path(cmd_path), True, f"/k cd {str(file_path)}")
+        return 0
+    except Exception as e:
+        Logger().error(f"Can't open cmd in path: {str(e)}")
+        return 0
+
+
+def is_file_executable(file_path: Path) -> bool:
+    """ Checking execution mode is ok on linux, but not enough on windows, since every file with an associated
+     program has this flag. Use custom pathext lists to determine executable file extensions. """
+    is_executable = False
+    if platform.system() == "Linux":
+        if os.access(str(file_path), os.X_OK):
+            is_executable = True
+    elif platform.system() == "Windows":
+        # don't use PATHEXT - some programs write other filetypes like .py in it...
+        path_exts = WIN_EXE_FILE_TYPES
+        if file_path.suffix in path_exts:
+            is_executable = True
+    return is_executable
+
+
+def execute_app(executable: Path, is_console_app: bool, args: str) -> int:
+    """
+    Executes an application with args and optionally spawns a new shell
+    as specified in the app entry.
+    Returns the pid of the new process.
+    """
+    if executable.absolute().is_file():
+        cmd = [str(executable)]
+        if args:
+            cmd += args.strip().split(" ")
+        return execute_cmd(cmd, is_console_app)
+    Logger().warning(f"No executable {str(executable)} to start.")
+    return 0
+
+
+def execute_cmd(cmd: List[str], is_console_app: bool) -> int:
+    """ Generic process execute method. Returns pid. """
+    command_path = Path(cmd[0]).parent
+    try:
+        # Linux call errors on creationflags argument, so the calls must be separated
+        if platform.system() == "Windows":
+            creationflags = 0
+            if is_console_app:
+                creationflags = subprocess.CREATE_NEW_CONSOLE
+                cmd = [generate_launch_script(cmd)]
+            # don't use 'executable' arg of Popen, because then shell scripts won't execute correctly
+            proc = subprocess.Popen(cmd, creationflags=creationflags, cwd=str(command_path))
+            return proc.pid
+        elif platform.system() == "Linux":
+            if is_console_app:
+                # Sadly, there is no default way to do this, because of the miriad terminal emulators available
+                # Use the default distro emulator, with x-terminal-emulator
+                # (sudo update-alternatives --config x-terminal-emulator)
+                # This works only on debian distros.
+                cmd = [generate_launch_script(cmd)]
+                cmd = ["x-terminal-emulator", "-e"] + cmd
+            proc = subprocess.Popen(cmd, cwd=str(command_path))
+            return proc.pid
+        return 0
+    except Exception as e:
+        Logger().error(f"Can't execute cmd: {str(e)}")
+        return 0
+
+
+def generate_launch_script(cmd: List[str]) -> str:
+    import tempfile
+    from jinja2 import Template
+
+    launch_templ_file = ""
+
+    if platform.system() == 'Windows':
+        launch_templ_file = "launch.bat.in"
+        temp_fd, temp_path_str = tempfile.mkstemp(".bat", prefix=PKG_NAME, text=True)
+    elif platform.system() == "Linux":
+        launch_templ_file = "launch.sh.in"
+        temp_fd, temp_path_str = tempfile.mkstemp(".sh", prefix=PKG_NAME, text=True)
+    else:
+        Logger().warning(f"Not supported OS.")
+        return ""
+    launch_templ_path = asset_path / launch_templ_file
+    with open(launch_templ_path, "r") as fd:
+        launch_template = Template(fd.read())
+    launch_content = launch_template.render(COMMAND=" ".join(cmd))
+    with os.fdopen(temp_fd, 'w') as f:
+        f.write(launch_content)
+    if platform.system() == 'Linux':
+        os.system(f"chmod +x {temp_path_str}")
+    return temp_path_str
+
+
+def open_file(file: Path):
+    """ Open files with their associated programs """
+    try:
+        if file.absolute().is_file():
+            if platform.system() == 'Windows':
+                os.startfile(str(file))
+            elif platform.system() == "Linux":
+                subprocess.Popen(("xdg-open", str(file)))
+    except Exception as e:
+        Logger().error(f"Can't open file: {str(e)}")
+        return 0
+
+
+def delete_path(dst: Path):
+    """
+    Delete file or (non-empty) folder recursively.
+    Exceptions will be caught and message logged to stdout.
+    """
+    from distutils.dir_util import remove_tree
+    try:
+        if dst.is_file():
+            os.remove(dst)
+        elif dst.is_dir():
+            remove_tree(str(dst), verbose=1)
+    except Exception as e:
+        Logger().warning(f"Can't delete {str(dst)}: {str(e)}")
+
+
+def copy_path_with_overwrite(src: Path, dst: Path):
+    """
+    Copy files/directories while overwriting possible files and adding missing ones.
+    Directories will be copied from under source, so you may need to add the orig. folder name, if you want that!
+    Exceptions will be caught and message logged to stdout.
+    """
+    # TODO find replacements for deprecated distutils functions
+    from distutils.dir_util import copy_tree
+    from distutils.file_util import copy_file
+    try:
+        if src.is_file():
+            copy_file(str(src), str(dst))
+        else:
+            copy_tree(str(src), str(dst))
+    except Exception as e:
+        Logger().warning(f"Can't copy {str(src)} to {str(dst)}: {str(e)}")
+
+
+def calc_paste_same_dir_name(dst: Path, index=1):
+    """
+    Create a name for a file like /file.txt -> /file (2).txt.
+    It will find the next empty number.
+    If a file with a higher number exists it will ignore it.
+    """
+    if dst.exists():
+        new_path = dst.with_name(f"{dst.stem} ({str(index+1)}){dst.suffix}")
+        possible_path = calc_paste_same_dir_name(new_path, index+1)
+        if possible_path == Path(INVALID_PATH):
+            return new_path
+        else:
+            return dst
+    else:
+        if index == 1:  # if file does not exist
+            return dst
+        return Path(INVALID_PATH)
+
+
+def get_default_file_editor():
+    if platform.system() == "Windows":
+        editor_executable = find_program_in_windows("Notepad++", partial_match=True, key_to_find="DisplayIcon")
+        if Path(editor_executable).exists():
+            return editor_executable
+        return "notepad.exe"
+    else:
+        return "gedit"  # distro dependent, but make something
+
+
+def find_program_in_windows(app_name: str, partial_match=False, key_to_find="InstallLocation") -> str:
+    if platform.system() != "Windows":
+        return ""
+
+    import winreg
+    arch_keys = {winreg.KEY_WOW64_32KEY, winreg.KEY_WOW64_64KEY}
+    for arch_key in arch_keys:
+        key = winreg.OpenKey(winreg.HKEY_LOCAL_MACHINE,
+                             r"SOFTWARE\Microsoft\Windows\CurrentVersion\Uninstall", 0, winreg.KEY_READ | arch_key)
+        for i in range(0, winreg.QueryInfoKey(key)[0]):
+            sub_key_name = winreg.EnumKey(key, i)
+            sub_key = winreg.OpenKey(key, sub_key_name)
+            try:
+                current_app_name = winreg.QueryValueEx(sub_key, "DisplayName")[0]
+                if partial_match:
+                    if app_name in current_app_name:
+                        location = winreg.QueryValueEx(sub_key, key_to_find)[0]
+                        return location
+                if app_name == current_app_name:
+                    location = winreg.QueryValueEx(sub_key, key_to_find)[0]
+                    return location
+            except OSError:
+                pass
+            finally:
+                sub_key.Close()
+    return ""
```

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/settings/__init__.py` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/settings/ini_file.py` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/settings/ini_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,53 +2,55 @@
 import os
 from pathlib import Path
 import platform
 from typing import Any, Dict, Optional, Tuple
 
 from conan_app_launcher import BUILT_IN_PLUGIN, PathLike, base_path
 from conan_app_launcher.app.logger import Logger
-from conan_app_launcher.core.system import get_default_file_editor
+from conan_app_launcher.app.system import get_default_file_editor
 
 from . import (AUTO_INSTALL_QUICKLAUNCH_REFS, CONSOLE_SPLIT_SIZES, DEFAULT_INSTALL_PROFILE, FILE_EDITOR_EXECUTABLE, FONT_SIZE,
                GENERAL_SECTION_NAME, GUI_STYLE, GUI_STYLE_FLUENT, GUI_STYLE_MATERIAL,
                GUI_MODE_LIGHT, GUI_MODE, LAST_CONFIG_FILE, PLUGINS_SECTION_NAME, VIEW_SECTION_NAME, WINDOW_SIZE,
                SettingsInterface)
 
+
 def application_settings_spec() -> Dict[str, Dict[str, Any]]:
     return {
-    GENERAL_SECTION_NAME: {
-        LAST_CONFIG_FILE: "",
-        FILE_EDITOR_EXECUTABLE: get_default_file_editor(),
-        AUTO_INSTALL_QUICKLAUNCH_REFS: False,
-        DEFAULT_INSTALL_PROFILE: ""
-    },
-    VIEW_SECTION_NAME: {
-        FONT_SIZE: 12,
-        GUI_STYLE: GUI_STYLE_FLUENT if platform.system() == "Windows" else GUI_STYLE_MATERIAL,
-        GUI_MODE: GUI_MODE_LIGHT,
-        WINDOW_SIZE: "0,0,800,600",
-        CONSOLE_SPLIT_SIZES: "413,126"
-    },
-    PLUGINS_SECTION_NAME: {
-        BUILT_IN_PLUGIN: str(base_path / "ui" / "plugins.ini")
+        GENERAL_SECTION_NAME: {
+            LAST_CONFIG_FILE: "",
+            FILE_EDITOR_EXECUTABLE: get_default_file_editor(),
+            AUTO_INSTALL_QUICKLAUNCH_REFS: False,
+            DEFAULT_INSTALL_PROFILE: ""
+        },
+        VIEW_SECTION_NAME: {
+            FONT_SIZE: 12,
+            GUI_STYLE: GUI_STYLE_FLUENT if platform.system() == "Windows" else GUI_STYLE_MATERIAL,
+            GUI_MODE: GUI_MODE_LIGHT,
+            WINDOW_SIZE: "0,0,800,600",
+            CONSOLE_SPLIT_SIZES: "413,126"
+        },
+        PLUGINS_SECTION_NAME: {
+            BUILT_IN_PLUGIN: str(base_path / "ui" / "plugins.ini")
+        }
+
     }
 
-}
 
 class IniSettings(SettingsInterface):
     """
     Settings mechanism with an ini file to use as a storage.
     File and entries are automatically created from the default value of the class.
     User defined keys are now allowed for nodes specified incustom_key_enabled_sections.
     Settings should be accessed via their constant name.
     """
 
-    def __init__(self, ini_file_path: Optional[PathLike], auto_save=True, 
+    def __init__(self, ini_file_path: Optional[PathLike], auto_save=True,
                  default_values=application_settings_spec(),
-                 custom_key_enabled_sections = [PLUGINS_SECTION_NAME]):
+                 custom_key_enabled_sections=[PLUGINS_SECTION_NAME]):
         """
         Read config.ini file to load settings.
         Create, if not existing, but the directory must already exist!
         Default path is current working dir / settings.ini
         """
         if not ini_file_path:
             self._ini_file_path = Path().cwd() / "settings.ini"
@@ -118,15 +120,15 @@
     def add(self, name: str, value: "str | int | float | bool", node: str):
         if not self._values.get(node):
             self._values[node] = {}
         self._values[node][name] = value
         self.save()
 
     def remove(self, name: str):
-        for node_name,node in self._values.items():
+        for node_name, node in self._values.items():
             if name in node:
                 node.pop(name)
                 del self._parser[node_name][name]
                 break
         self.save()
 
     def save(self):
@@ -148,15 +150,15 @@
                 setting_keys = set(list(self._values[node].keys()))
                 if node in self._custom_key_enabled_sections:
                     setting_keys = setting_keys.union(set(self._get_section(node).keys()))
                 if not self._values[node]:  # empty section - this is a user filled dict
                     update_needed |= self._read_dict_setting(node)
                 for setting in setting_keys:
                     update_needed |= self._read_setting(setting, node)
-                
+
         except Exception as e:
             Logger().error(
                 f"Settings: Can't read ini file: {str(e)}, trying to delete and create a new one...")
             try:
                 os.remove(str(self._ini_file_path))  # let an exeception to the user, file can't be deleted
             except Exception:
                 Logger().error(f"Settings: Can't delete ini file: {str(e)}.")
```

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/__init__.py` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,28 @@
+from conan_app_launcher import DEBUG_LEVEL, INVALID_PATH
 import os
 from pathlib import Path
 
-from conan_app_launcher.app.logger import Logger
 from .main_window import BaseSignals
 from .fluent_window import FluentWindow
 from .plugin import PluginInterfaceV1, PluginFile, PluginDescription
 
 
 def compile_ui_file_if_newer(ui_file: Path):
+    from conan_app_launcher.app.logger import Logger
     py_ui_file = ui_file.parent / (ui_file.stem + "_ui.py")
     if py_ui_file.exists() and py_ui_file.stat().st_mtime > ui_file.stat().st_mtime:
         return
     Logger().debug("Converting " + str(py_ui_file))
     os.system(f"pyside6-uic -o {str(py_ui_file)} {str(ui_file)}")
 
+
 # compile uic files, if needed
-from conan_app_launcher import DEBUG_LEVEL, INVALID_PATH
 if DEBUG_LEVEL > 0:
     current_dir = Path(__file__).parent
     for ui_file in current_dir.glob("**/*.ui"):
         py_ui_file = Path(INVALID_PATH)
         try:
             compile_ui_file_if_newer(ui_file)
         except Exception as e:
+            from conan_app_launcher.app.logger import Logger
             Logger().warning(f"Can't convert {str(py_ui_file)}: {str(e)}")
```

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/common/__init__.py` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/common/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 """ Common ui classes, and functions """
 
 from pathlib import Path
 import conan_app_launcher.app as app
-from conan_app_launcher.core.conan_common import ConanRef
-from conan_app_launcher.core.system import execute_cmd, open_file  # using global module pattern
+from conan_app_launcher.conan_wrapper.types import ConanRef
+from conan_app_launcher.app.system import execute_cmd, open_file  # using global module pattern
 from conan_app_launcher.settings import FILE_EDITOR_EXECUTABLE, FONT_SIZE
 from PySide6.QtGui import QFontMetrics, QFont
 
 from .icon import extract_icon, get_icon_from_image_file, get_inverted_asset_image, get_platform_icon
-from .loading import AsyncLoader, Worker
 from .logger import init_qt_logger, remove_qt_logger
 from .model import TreeModel, TreeModelItem, FileSystemModel
 from .theming import activate_theme, configure_theme, get_user_theme_color, CanSetIconWidgetProtocol, CanSetPixmapWidgetProtocol, ThemedWidget, get_themed_asset_icon, get_asset_image_path, get_gui_dark_mode, get_gui_style
 
 
 def measure_font_width(text: str) -> int:
     """ Return the width of a text in pixels woth the current font and default fontsize """
```

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/common/icon.py` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/common/icon.py`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/common/logger.py` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/common/logger.py`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/common/model.py` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/common/model.py`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/common/theming.py` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/common/theming.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import platform
 from pathlib import Path
 from typing import TYPE_CHECKING, Dict, Optional, Tuple, Union
 
 import conan_app_launcher.app as app
 from conan_app_launcher import base_path
-from conan_app_launcher.core.system import is_windows_11
+from conan_app_launcher.app.system import is_windows_11
 from conan_app_launcher.settings import FONT_SIZE, GUI_MODE, GUI_MODE_LIGHT, GUI_MODE_DARK, GUI_STYLE, GUI_STYLE_FLUENT, GUI_STYLE_MATERIAL
 from conan_app_launcher.app.logger import Logger
 
 from jinja2 import Template
 from PySide6.QtWidgets import QApplication, QWidget
 from PySide6.QtGui import QIcon, QPixmap, QImage, QFont, QFontDatabase
 from PySide6.QtCore import QSize
```

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/config/__init__.py` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/config/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/config/json_file.py` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/config/json_file.py`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/dark_style.qss.in` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/dark_style.qss.in`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/dialogs/conan_install/conan_install.py` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/dialogs/conan_install/conan_install.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from typing import Optional
 
 import conan_app_launcher.app as app
+from conan_app_launcher.app.loading import AsyncLoader
 from conan_app_launcher.app.logger import Logger  # using global module pattern
-from conan_app_launcher.core.conan_worker import ConanWorkerElement
+from conan_app_launcher.conan_wrapper.conan_worker import ConanWorkerElement
 from conan_app_launcher.settings import DEFAULT_INSTALL_PROFILE
 from conan_app_launcher.ui.common import get_themed_asset_icon
 from PySide6.QtCore import QSize, Qt, SignalInstance
 from PySide6.QtWidgets import QDialog, QWidget, QTreeWidgetItem, QComboBox
 
-from conan_app_launcher.core.conan_common import ConanRef
+from conan_app_launcher.conan_wrapper.types import ConanRef
 
 
 class ConanInstallDialog(QDialog):
     MARK_AS_DEFAULT_INSTALL_PROFILE = " *"
 
     def __init__(self, parent: Optional[QWidget], conan_full_ref: str, pkg_installed_signal: Optional[SignalInstance] = None, lock_ref=False):
         """ conan_ref can be in full ref format with <ref>:<id> """
@@ -79,16 +80,17 @@
 
     def load_options(self, conan_full_ref: str):
         # options table
         options = []
         conan_ref = ""
         try:
             conan_ref = conan_full_ref.split(":")[0]
-            self._ref_info = app.conan_api.conan.info(
-                app.conan_api.generate_canonical_ref(ConanRef.loads(conan_ref)))
+            loader = AsyncLoader(self)
+            loader.async_loading(self, self.on_options_query, (conan_ref, ), loading_text="Loading options...")
+            loader.wait_for_finished()
             # TODO: CONAN V2
             options = self._ref_info[0].root.dependencies[0].dst.conanfile.options.items()  # type: ignore
         except Exception:
             Logger().warning("Can't determine options of " + conan_ref)
         # doing this after connecting toggle_auto_install_on_pkg_ref initializes it correctly
         for name, value in options:
             item = QTreeWidgetItem(self._ui.options_widget)
@@ -109,14 +111,21 @@
         self._ui.options_widget.resizeColumnToContents(1)
         self._ui.options_widget.resizeColumnToContents(0)
         self._ui.options_widget.itemDoubleClicked.connect(self.onTreeWidgetItemDoubleClicked)
 
     def onTreeWidgetItemDoubleClicked(self, item):
         self._ui.options_widget.openPersistentEditor(item, 1)
 
+    def on_options_query(self, conan_ref: str):
+        try:
+            self._ref_info = app.conan_api.conan.info(
+                    app.conan_api.generate_canonical_ref(ConanRef.loads(conan_ref)))
+        except Exception:
+            return
+
     def on_auto_install_check(self):
         enabled = True
         if self._ui.auto_install_check_box.isChecked():
             enabled = False
         self._ui.profile_cbox.setEnabled(enabled)
         self._ui.options_widget.setEnabled(enabled)
         self._ui.update_check_box.setEnabled(enabled)
```

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/dialogs/conan_install/conan_install.ui` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/dialogs/conan_install/conan_install.ui`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/dialogs/conan_install/conan_install_ui.py` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/dialogs/conan_install/conan_install_ui.py`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/dialogs/conan_remove.py` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/dialogs/conan_remove.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Optional
 
-import conan_app_launcher.app as app  # using global module pattern
+import conan_app_launcher.app as app
+from conan_app_launcher.app.loading import AsyncLoader  # using global module pattern
 from conan_app_launcher.app.logger import Logger
-from ..common import AsyncLoader
 
 from PySide6.QtCore import SignalInstance
 from PySide6.QtWidgets import QMessageBox, QWidget
 
 
 class ConanRemoveDialog(QMessageBox):
```

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/dialogs/crash/crash.py` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/dialogs/crash/crash.py`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/dialogs/crash/crash.ui` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/dialogs/crash/crash.ui`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/dialogs/crash/crash_ui.py` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/dialogs/crash/crash_ui.py`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/dialogs/file_editor_selection/file_editor_selection.py` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/dialogs/file_editor_selection/file_editor_selection.py`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/dialogs/file_editor_selection/file_editor_selector.ui` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/dialogs/file_editor_selection/file_editor_selector.ui`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/dialogs/file_editor_selection/file_editor_selector_ui.py` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/dialogs/file_editor_selection/file_editor_selector_ui.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 ################################################################################
 ## Form generated from reading UI file 'file_editor_selector.ui'
 ##
-## Created by: Qt User Interface Compiler version 6.4.2
+## Created by: Qt User Interface Compiler version 6.4.3
 ##
 ## WARNING! All changes made in this file will be lost when recompiling UI file!
 ################################################################################
 
 from PySide6.QtCore import (QCoreApplication, QDate, QDateTime, QLocale,
     QMetaObject, QObject, QPoint, QRect,
     QSize, QTime, QUrl, Qt)
```

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/dialogs/reorder_dialog/reorder_dialog.py` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/dialogs/reorder_dialog/reorder_dialog.py`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/dialogs/reorder_dialog/reorder_dialog.ui` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/dialogs/reorder_dialog/reorder_dialog.ui`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/dialogs/reorder_dialog/reorder_dialog_ui.py` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/dialogs/reorder_dialog/reorder_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/fluent_window/__init__.py` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/fluent_window/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/fluent_window/fluent_window.py` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/fluent_window/fluent_window.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 from enum import Enum
 from typing import TYPE_CHECKING, Dict, List, Optional, Tuple, Type, TypeVar
 
 
 # uses Logger, settings and theming related functions
 from conan_app_launcher import AUTOCLOSE_SIDE_MENU
-from conan_app_launcher.core.system import is_windows_11
+from conan_app_launcher.app.system import is_windows_11
 
 from PySide6.QtCore import (QEasingCurve, QEvent, QObject, QPoint,
                             QPropertyAnimation, QRect, QSize, Qt)
 from PySide6.QtGui import QHoverEvent, QMouseEvent
 from PySide6.QtWidgets import (QMainWindow,
                                QPushButton, QSizePolicy, QWidget)
```

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/fluent_window/fluent_window.ui` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/fluent_window/fluent_window.ui`

 * *Files 0% similar despite different names*

#### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/fluent_window/fluent_window.ui` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/fluent_window/fluent_window.ui`

```diff
@@ -447,15 +447,15 @@
                                   <property name="topMargin">
                                     <number>0</number>
                                   </property>
                                   <property name="rightMargin">
                                     <number>2</number>
                                   </property>
                                   <property name="bottomMargin">
-                                    <number>5</number>
+                                    <number>1</number>
                                   </property>
                                   <item>
                                     <widget class="QStackedWidget" name="page_stacked_widget">
                                       <property name="sizePolicy">
                                         <sizepolicy hsizetype="Preferred" vsizetype="Preferred">
                                           <horstretch>0</horstretch>
                                           <verstretch>0</verstretch>
```

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/fluent_window/fluent_window_ui.py` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/fluent_window/fluent_window_ui.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 ################################################################################
 ## Form generated from reading UI file 'fluent_window.ui'
 ##
-## Created by: Qt User Interface Compiler version 6.4.2
+## Created by: Qt User Interface Compiler version 6.4.3
 ##
 ## WARNING! All changes made in this file will be lost when recompiling UI file!
 ################################################################################
 
 from PySide6.QtCore import (QCoreApplication, QDate, QDateTime, QLocale,
     QMetaObject, QObject, QPoint, QRect,
     QSize, QTime, QUrl, Qt)
@@ -192,15 +192,15 @@
         self.content_frame.setMinimumSize(QSize(0, 300))
         self.content_frame.setFrameShape(QFrame.NoFrame)
         self.content_frame.setFrameShadow(QFrame.Raised)
         self.content_frame_layout = QVBoxLayout(self.content_frame)
         self.content_frame_layout.setSpacing(0)
         self.content_frame_layout.setObjectName(u"content_frame_layout")
         self.content_frame_layout.setSizeConstraint(QLayout.SetMinAndMaxSize)
-        self.content_frame_layout.setContentsMargins(2, 0, 2, 5)
+        self.content_frame_layout.setContentsMargins(2, 0, 2, 1)
         self.page_stacked_widget = QStackedWidget(self.content_frame)
         self.page_stacked_widget.setObjectName(u"page_stacked_widget")
         sizePolicy4.setHeightForWidth(self.page_stacked_widget.sizePolicy().hasHeightForWidth())
         self.page_stacked_widget.setSizePolicy(sizePolicy4)
         self.page = QWidget()
         self.page.setObjectName(u"page")
         self.page_layout = QVBoxLayout(self.page)
```

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/fluent_window/side_menu.py` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/fluent_window/side_menu.py`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/fluent_window/side_menu.ui` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/fluent_window/side_menu.ui`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/fluent_window/side_menu_ui.py` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/fluent_window/side_menu_ui.py`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/light_style.qss.in` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/light_style.qss.in`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/main_window.py` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/main_window.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import datetime
 from dataclasses import dataclass
 from shutil import rmtree
 from typing import Optional
 
 import conan_app_launcher.app as app  # using global module pattern
 from conan_app_launcher import APP_NAME, MAX_FONT_SIZE, MIN_FONT_SIZE, PathLike, conan_version
+from conan_app_launcher.app.loading import AsyncLoader
 
 from conan_app_launcher.app.logger import Logger
-from conan_app_launcher.core.conan_cleanup import ConanCleanup
 from conan_app_launcher.settings import (CONSOLE_SPLIT_SIZES, FILE_EDITOR_EXECUTABLE, FONT_SIZE,
                                          GUI_MODE, GUI_MODE_DARK, GUI_MODE_LIGHT, GUI_STYLE, GUI_STYLE_FLUENT,
                                          GUI_STYLE_MATERIAL, LAST_CONFIG_FILE, WINDOW_SIZE)
 from conan_app_launcher.ui.common.theming import get_gui_dark_mode, get_gui_style
 from conan_app_launcher.ui.dialogs.file_editor_selection.file_editor_selection import FileEditorSelDialog
 from conan_app_launcher.ui.plugin.plugins import PluginHandler
 from conan_app_launcher.ui.widgets import AnimatedToggle, WideMessageBox
 from PySide6.QtCore import QRect, SignalInstance, Signal
 from PySide6.QtGui import QKeySequence
 from PySide6.QtWidgets import QApplication, QFileDialog, QWidget, QFrame, QVBoxLayout, QRadioButton
 
-from .common import (AsyncLoader, activate_theme, init_qt_logger,
+from .common import (activate_theme, init_qt_logger,
                      remove_qt_logger)
 from .fluent_window import FluentWindow, SideSubMenu
 from .plugin import PluginInterfaceV1
 from .model import UiApplicationModel
 from .views import AboutPage, AppGridView, PluginsPage
 
 
@@ -122,15 +122,15 @@
             "Icon Style", self._style_chooser_frame, "icons/global/conan_settings.svg", force_v_layout=True)
         view_settings_submenu.add_menu_line()
 
         self.main_general_settings_menu.add_menu_line()
 
         if conan_version.startswith("1"):
             self.main_general_settings_menu.add_button_menu_entry("Remove Locks",
-                                                                  app.conan_api.remove_locks, "icons/remove-lock.svg")
+                                                                  self.on_conan_remove_locks, "icons/remove-lock.svg")
             self.main_general_settings_menu.add_button_menu_entry("Clean Conan Cache",
                                                                   self.open_cleanup_cache_dialog, "icons/cleanup.svg")
             self.main_general_settings_menu.add_menu_line()
         self.add_right_bottom_menu_main_page_entry("Manage Plugins", self.plugins_page, "icons/plugin.svg")
         self.add_right_bottom_menu_main_page_entry("About", self.about_page, "icons/about.svg")
 
     def closeEvent(self, event):  # override QMainWindow
@@ -152,19 +152,15 @@
 
     def load(self, config_source: Optional[PathLike] = None):
         """ Load all application gui elements specified in the GUI config (file) """
         config_source_str = str(config_source)
         if not config_source:
             config_source_str = app.active_settings.get_string(LAST_CONFIG_FILE)
         self._load_plugins()  # creates the objects - must be in this thread
-
-        # model loads incrementally
-        loader = AsyncLoader(self)
-        loader.async_loading(self, self._load_job_quicklaunch, (config_source_str,), cancel_button=False)
-        loader.wait_for_finished()
+        self._load_job_quicklaunch(config_source_str)
         self.loaded = True
 
     def _load_plugins(self):
         self._plugin_handler.load_all_plugins()
 
     def _load_plugin(self, plugin_object: PluginInterfaceV1):
         try:
@@ -181,14 +177,17 @@
     def _load_job_quicklaunch(self, config_source_str):
         # load ui file definitions
         self.model.loadf(config_source_str)
         # now actually load the views - this need signals, to execute in the gui thread
         self.app_grid.model = self.model.app_grid
         self.app_grid.load_signal.emit()
 
+    def on_conan_remove_locks(self):
+        app.conan_api.remove_locks()
+
     def on_font_size_increased(self):
         """ Increase font size by 2. Ignore if font gets too large. """
         new_size = app.active_settings.get_int(FONT_SIZE) + 1
         if new_size > MAX_FONT_SIZE:
             return
         app.active_settings.set(FONT_SIZE, new_size)
         activate_theme(self._qt_app)
@@ -228,14 +227,15 @@
         # all icons must be reloaded
         self.apply_theme()
         for page in self.page_widgets.get_all_pages():
             page.reload_themed_icons()
 
     def open_cleanup_cache_dialog(self):
         """ Open the message box to confirm deletion of invalid cache folders """
+        from conan_app_launcher.conan_wrapper.conan_cleanup import ConanCleanup
         cleaner = ConanCleanup(app.conan_api)
         loader = AsyncLoader(self)
         loader.async_loading(self, cleaner.get_cleanup_cache_paths, )
         loader.wait_for_finished()
         paths = cleaner.orphaned_packages.union(cleaner.orphaned_references)
         if not paths:
             self.write_log("INFO: Nothing found in cache to clean up.")
```

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/model.py` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/model.py`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/plugin/plugins.py` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/plugin/plugins.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import importlib
 import sys
 import types
 from packaging import specifiers, version
 
 import os
 from dataclasses import dataclass
-from distutils.util import strtobool
 from pathlib import Path
 import uuid
 from typing import TYPE_CHECKING, List, Optional
 from conan_app_launcher import BUILT_IN_PLUGIN, conan_version
 
 import conan_app_launcher.app as app
 from conan_app_launcher import base_path
@@ -118,15 +117,15 @@
                 if import_path.is_dir():  # needs an __init__.py
                     assert (import_path / "__init__.py").exists()
 
                 plugin_class = plugin_info.get("plugin_class")
                 assert plugin_class, "field 'plugin_class' is required"
                 description = plugin_info.get("description", "")
                 author = plugin_info.get("author", "Unknown")
-
+                from distutils.util import strtobool
                 side_menu = bool(strtobool(plugin_info.get("side_menu", "False")))
                 conan_versions = plugin_info.get("conan_versions", "")
                 desc = PluginDescription(name, version, author, icon, str(import_path),
                                          plugin_class, description, side_menu, conan_versions)
                 plugins.append(desc)
             except Exception as e:
                 Logger().error(f"Can't read {section} plugin information from {plugin_file_path}: {str(e)}.")
```

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/plugins.ini` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/plugins.ini`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/about/about.ui` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/about/about.ui`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/about/about_page.py` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/about/about_page.py`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/about/about_text.html` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/about/about_text.html`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/about/about_ui.py` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/about/about_ui.py`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/app_grid/__init__.py` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/app_grid/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # using global module pattern
 from conan_app_launcher.ui.common import get_themed_asset_icon
 from conan_app_launcher.settings import AUTO_INSTALL_QUICKLAUNCH_REFS, LAST_CONFIG_FILE  # using global module pattern
 from conan_app_launcher.ui.config import UiAppLinkConfig, UiTabConfig
 from conan_app_launcher.ui.fluent_window import FluentWindow
 from conan_app_launcher.ui.plugin.plugins import PluginInterfaceV1
 from conan_app_launcher.ui.widgets import RoundedMenu, AnimatedToggle
-from conan_app_launcher.core.conan_common import ConanRef, PkgRef
+from conan_app_launcher.conan_wrapper.types import ConanRef, PkgRef
 
 from PySide6.QtCore import Qt, Signal
 from PySide6.QtGui import QIcon, QAction
 from PySide6.QtWidgets import (QInputDialog, QMessageBox, QTabWidget, QFileDialog, QVBoxLayout)
 
 from .model import UiAppLinkModel, UiTabModel
 from .tab import TabList, TabList  # TabGrid
```

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/app_grid/app_link.py` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/app_grid/app_link.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 from pathlib import Path
 from typing import TYPE_CHECKING, Optional
 import conan_app_launcher.app as app
 
 from conan_app_launcher import ICON_SIZE, INVALID_PATH
 from conan_app_launcher.app.logger import Logger
-from conan_app_launcher.core import open_in_file_manager, run_file
+from conan_app_launcher.app.system import open_in_file_manager, run_file
 from conan_app_launcher.ui.common import get_themed_asset_icon, measure_font_width
 from conan_app_launcher.ui.dialogs.reorder_dialog.reorder_dialog import ReorderDialog
 from conan_app_launcher.ui.views.app_grid.model import UiAppLinkModel
 from conan_app_launcher.ui.widgets import RoundedMenu
 from PySide6.QtCore import Qt
 from PySide6.QtGui import QIcon, QAction
 from PySide6.QtWidgets import (QDialog, QFrame, QMessageBox, QWidget)
@@ -100,18 +100,18 @@
         ret = move_dialog.exec()
         if ret == QDialog.DialogCode.Accepted:
             self._parent_tab.redraw(force=True)
 
     def resizeEvent(self, event):
         if not self._parent_tab:
             return
-        content_frame: QWidget = self._parent_tab.parent().parent().parent().parent().parent() # type: ignore
+        content_frame: QWidget = self._parent_tab.parent().parent().parent().parent().parent()  # type: ignore
         max_cl_width = content_frame.width() - self._ui.left_frame.width() - \
             self._ui.right_frame.width()
-        if max_cl_width < 400: # TODO find better solution
+        if max_cl_width < 400:  # TODO find better solution
             self._ui.central_left_frame.setMaximumWidth(0)
             self._ui.central_right_frame.setMaximumWidth(0)
             self._ui.arguments_name_label.setMaximumWidth(0)
             self._ui.arguments_value_label.setMaximumWidth(0)
             self._ui.arguments_value_label.setText("")
             return
         else:
@@ -132,18 +132,18 @@
             self._ui.central_right_frame.setMaximumWidth(max_sum_width)
             self._ui.arguments_name_label.setMaximumWidth(1000)
             self._ui.arguments_name_label.adjustSize()
             self._ui.arguments_value_label.setMaximumWidth(
                 max_sum_width - self._ui.arguments_name_label.width() - 50)
             self.split_into_lines(self._ui.arguments_value_label, self.model.args,
                                   max_sum_width - self._ui.arguments_name_label.width())
-        
+
         super().resizeEvent(event)
 
-    def delete(self): # TODO needed?
+    def delete(self):  # TODO needed?
         pass
 
     def split_into_lines(self, widget, model_value, max_width):
         """ Calculate, how text can be split into multiple lines, based on the current width"""
         px = measure_font_width(model_value)
         if px == 0:
             return
@@ -152,15 +152,15 @@
                 new_length-1 == len(widget.text().split("\n")[0]):
             return
         args = self.word_wrap(model_value, new_length)
         widget.setText(args)
 
     @staticmethod
     def word_wrap(text: str, max_length: int) -> str:
-        if max_length==0:
+        if max_length == 0:
             return text
         split_name = text.split(" ")
         name = ""  # split long titles
         for word in split_name:
             if len(word) < max_length:
                 new_word = word
             else:
```

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/app_grid/app_link.ui` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/app_grid/app_link.ui`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/app_grid/app_link_ui.py` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/app_grid/app_link_ui.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 ################################################################################
 ## Form generated from reading UI file 'app_link.ui'
 ##
-## Created by: Qt User Interface Compiler version 6.4.2
+## Created by: Qt User Interface Compiler version 6.4.3
 ##
 ## WARNING! All changes made in this file will be lost when recompiling UI file!
 ################################################################################
 
 from PySide6.QtCore import (QCoreApplication, QDate, QDateTime, QLocale,
     QMetaObject, QObject, QPoint, QRect,
     QSize, QTime, QUrl, Qt)
```

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/app_grid/dialogs/app_edit_dialog.py` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/app_grid/dialogs/app_edit_dialog.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import conan_app_launcher.app as app  # using global module pattern
 from conan_app_launcher.app.logger import Logger
 from conan_app_launcher.ui.common import measure_font_width
 from conan_app_launcher.ui.common.theming import get_themed_asset_icon
 from conan_app_launcher.ui.views.app_grid.model import UiAppLinkModel
 from conan_app_launcher.ui.dialogs import ConanInstallDialog
-from conan_app_launcher.core.conan_common import ConanRef
+from conan_app_launcher.conan_wrapper.types import ConanRef
 
 from PySide6.QtCore import SignalInstance
 from PySide6.QtWidgets import QWidget, QDialog, QFileDialog, QMessageBox
 
 
 class AppEditDialog(QDialog):
```

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/app_grid/dialogs/app_edit_dialog.ui` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/app_grid/dialogs/app_edit_dialog.ui`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/app_grid/dialogs/app_edit_dialog_ui.py` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/app_grid/dialogs/app_edit_dialog_ui.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 ################################################################################
 ## Form generated from reading UI file 'app_edit_dialog.ui'
 ##
-## Created by: Qt User Interface Compiler version 6.4.2
+## Created by: Qt User Interface Compiler version 6.4.3
 ##
 ## WARNING! All changes made in this file will be lost when recompiling UI file!
 ################################################################################
 
 from PySide6.QtCore import (QCoreApplication, QDate, QDateTime, QLocale,
     QMetaObject, QObject, QPoint, QRect,
     QSize, QTime, QUrl, Qt)
```

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/app_grid/model.py` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/app_grid/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 from pathlib import Path
 from typing import Callable, List, Optional
 
 import conan_app_launcher.app as app  # using global module pattern
 from conan_app_launcher import (
     INVALID_CONAN_REF, INVALID_PATH, USE_CONAN_WORKER_FOR_LOCAL_PKG_PATH_AND_INSTALL,
     USE_LOCAL_CACHE_FOR_LOCAL_PKG_PATH)
-from conan_app_launcher.core.conan_worker import ConanWorkerElement
+from conan_app_launcher.conan_wrapper.conan_worker import ConanWorkerElement
 from conan_app_launcher.app.logger import Logger
 from conan_app_launcher.settings import AUTO_INSTALL_QUICKLAUNCH_REFS
 from conan_app_launcher.ui.common import extract_icon, get_icon_from_image_file, get_themed_asset_icon, get_asset_image_path
 from conan_app_launcher.ui.config import UiAppGridConfig, UiAppLinkConfig, UiTabConfig
-from conan_app_launcher.core.conan_common import ConanRef
+from conan_app_launcher.conan_wrapper.types import ConanRef
 
 # from PySide6.QtCore import QAbstractListModel, QModelIndex, Qt, QObject
 from PySide6.QtGui import QIcon
 from PySide6.QtCore import QAbstractListModel, QModelIndex, QPersistentModelIndex, Qt, QObject
 
 
 class UiAppGridModel(UiAppGridConfig, QObject):
```

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/app_grid/tab.py` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/app_grid/tab.py`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/conan_conf/conan_conf.py` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/conan_conf/conan_conf.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,42 @@
+from os import devnull
 import platform
 import subprocess
 from pathlib import Path
+import sys
 from typing import Optional, TYPE_CHECKING
 
+from conan_app_launcher import conan_version
 import conan_app_launcher.app as app
 from conan_app_launcher.app.logger import Logger
-from conan_app_launcher.core.system import delete_path, escape_venv
+from conan_app_launcher.app.system import delete_path
 from conan_app_launcher.ui.common import get_themed_asset_icon
+from conan_app_launcher.ui.common.syntax_highlighting import ConfigHighlighter
 from conan_app_launcher.ui.plugin.plugins import PluginDescription, PluginInterfaceV1
 from conan_app_launcher.ui.widgets import RoundedMenu
-from conan_app_launcher.core.conan_common import Remote
-from PySide6.QtCore import Qt, Signal
+from conan_app_launcher.conan_wrapper.types import Remote
+from PySide6.QtCore import Qt, Signal, QProcess
 from PySide6.QtGui import QIcon, QAction
 from PySide6.QtWidgets import QApplication, QDialog, QWidget, QMessageBox, QApplication, QInputDialog
 
 from .dialogs import RemoteEditDialog, RemoteLoginDialog
 from .model import ProfilesModel
 from .controller import ConanRemoteController
 
 if TYPE_CHECKING:
     from conan_app_launcher.ui.main_window import BaseSignals
     from conan_app_launcher.ui.fluent_window.fluent_window import FluentWindow
 
 
 class ConanConfigView(PluginInterfaceV1):
 
-    load_signal = Signal() # type: ignore
+    load_signal = Signal()  # type: ignore
 
     def __init__(self, parent: QWidget, plugin_description: PluginDescription,
-                  base_signals: "BaseSignals", page_widgets: Optional["FluentWindow.PageStore"] = None):
+                 base_signals: "BaseSignals", page_widgets: Optional["FluentWindow.PageStore"] = None):
         super().__init__(parent, plugin_description, base_signals)
         from .conan_conf_ui import Ui_Form
         self._ui = Ui_Form()
         self._ui.setupUi(self)
         self.load_signal.connect(self.load)
         self.config_file_path = Path("Unknown")
         self.profiles_path = Path("Unknown")
@@ -52,39 +56,23 @@
         self._load_remotes_tab()
         self._load_profiles_tab()
         self._load_config_file_tab()
         self._load_settings_yml_tab()
 
         # always show first tab on start
         self._ui.config_tab_widget.tabBar().setCurrentIndex(0)
+        self._conan_config_highlighter = ConfigHighlighter(self._ui.config_file_text_browser.document(), "ini")
+        self._profile_highlighter = ConfigHighlighter(self._ui.profiles_text_browser.document(), "ini")
+        self._settings_highlighter = ConfigHighlighter(self._ui.settings_file_text_browser.document(), "yaml")
 
     def _load_info_tab(self):
-        self._ui.conan_cur_version_value_label.setText(app.conan_api.client_version)
-
-        # setup system version outside of own venv
-        with escape_venv():
-            try:  # move to conan?
-                out = subprocess.check_output("conan --version", shell=True).decode("utf-8")
-                conan_sys_version = out.lower().split("version ")[1].rstrip()
-            except Exception:
-                Logger().debug("Conan version unknown...")
-                conan_sys_version = "Unknown"
-            try:  # move to conan?
-                python_exe_name = "python"
-                if platform.system() == "Linux":
-                    python_exe_name = "python3"
-                out = subprocess.check_output(f"{python_exe_name} --version", shell=True).decode("utf-8")
-                python_sys_version = out.lower().split("python ")[1].rstrip()
-            except Exception:
-                python_sys_version = "Unknown"
-
+        self._ui.conan_cur_version_value_label.setText(conan_version)
+        self._ui.python_exe_value_label.setText(sys.executable)
         self._ui.python_cur_version_value_label.setText(platform.python_version())
         self._ui.revision_enabled_checkbox.setChecked(app.conan_api.client_cache.config.revisions_enabled)
-        self._ui.conan_sys_version_value_label.setText(conan_sys_version)
-        self._ui.python_sys_version_value_label.setText(python_sys_version)
         self._ui.conan_usr_home_value_label.setText(app.conan_api.client_cache.cache_folder)
         self._ui.conan_usr_cache_value_label.setText(str(app.conan_api.get_short_path_root()))
         self._ui.conan_storage_path_value_label.setText(str(app.conan_api.client_cache.store))
 
     def _load_settings_yml_tab(self):
         try:
             self._ui.settings_file_text_browser.setText(Path(app.conan_api.client_cache.settings_path).read_text())
@@ -127,20 +115,23 @@
 
     def resizeEvent(self, a0):  # override
         """ Resize remote view columns automatically if window size changes """
         super().resizeEvent(a0)
 
         self._remotes_controller.resize_remote_columns()
         # self._ui.conan_usr_cache_label.adjustSize()
-        #self._ui.revision_enabled_label.setMaximumWidth(self._ui.conan_usr_cache_label.width())
+        # self._ui.revision_enabled_label.setMaximumWidth(self._ui.conan_usr_cache_label.width())
 
     def reload_themed_icons(self):
         super().reload_themed_icons()
         self._init_profile_context_menu()
         self._init_remote_context_menu()
+        self._conan_config_highlighter = ConfigHighlighter(self._ui.config_file_text_browser.document(),"ini")
+        self._profile_highlighter = ConfigHighlighter(self._ui.profiles_text_browser.document(),"ini")
+        self._settings_highlighter = ConfigHighlighter(self._ui.settings_file_text_browser.document(), "yaml")
 
 # Profile
 
     def on_copy_profile_requested(self):
         view_indexes = self._ui.profiles_list_view.selectedIndexes()
         if not view_indexes:
             return
@@ -187,15 +178,14 @@
         message_box.setStandardButtons(QMessageBox.StandardButton.Yes | QMessageBox.StandardButton.No)
         message_box.setIcon(QMessageBox.Icon.Question)
         reply = message_box.exec()
         if reply == QMessageBox.StandardButton.Yes:
             delete_path(self.profiles_path / profile_name)
             self.on_refresh_profiles()
 
-
     def on_refresh_profiles(self):
         self._load_profiles_tab()
 
 # Remote
 
     def _load_remotes_tab(self):
         self._remotes_controller.update()
```

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/conan_conf/conan_conf.ui` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/conan_conf/conan_conf.ui`

 * *Files 2% similar despite different names*

#### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/conan_conf/conan_conf.ui` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/conan_conf/conan_conf.ui`

```diff
@@ -28,15 +28,15 @@
       </property>
       <item>
         <widget class="QTabWidget" name="config_tab_widget">
           <property name="styleSheet">
             <string notr="true"/>
           </property>
           <property name="currentIndex">
-            <number>0</number>
+            <number>3</number>
           </property>
           <widget class="QWidget" name="info_widget">
             <property name="styleSheet">
               <string notr="true"/>
             </property>
             <attribute name="title">
               <string>Info</string>
@@ -74,73 +74,59 @@
                     <layout class="QVBoxLayout" name="verticalLayout_7">
                       <item>
                         <widget class="QGroupBox" name="versions_box">
                           <property name="title">
                             <string>Versions</string>
                           </property>
                           <layout class="QGridLayout" name="gridLayout" columnstretch="1,2">
-                            <item row="0" column="0">
-                              <widget class="QLabel" name="conan_cur_version_label">
+                            <item row="2" column="0">
+                              <widget class="QLabel" name="python_exe_label">
                                 <property name="text">
-                                  <string>Current Conan Version:</string>
+                                  <string>Current Python Executable:</string>
                                 </property>
                               </widget>
                             </item>
-                            <item row="0" column="1">
-                              <widget class="QLabel" name="conan_cur_version_value_label">
+                            <item row="2" column="1">
+                              <widget class="QLabel" name="python_exe_value_label">
                                 <property name="text">
                                   <string>Unknown</string>
                                 </property>
                                 <property name="textInteractionFlags">
                                   <set>Qt::LinksAccessibleByMouse|Qt::TextSelectableByKeyboard|Qt::TextSelectableByMouse</set>
                                 </property>
                               </widget>
                             </item>
-                            <item row="1" column="0">
-                              <widget class="QLabel" name="python_cur_version_label">
+                            <item row="0" column="0">
+                              <widget class="QLabel" name="conan_cur_version_label">
                                 <property name="text">
-                                  <string>Current Python Version:</string>
+                                  <string>Current Conan Version:</string>
                                 </property>
                               </widget>
                             </item>
                             <item row="1" column="1">
                               <widget class="QLabel" name="python_cur_version_value_label">
                                 <property name="text">
                                   <string>Unknown</string>
                                 </property>
                               </widget>
                             </item>
-                            <item row="2" column="0">
-                              <widget class="QLabel" name="conan_sys_version_label">
-                                <property name="text">
-                                  <string>System Conan Version:</string>
-                                </property>
-                              </widget>
-                            </item>
-                            <item row="2" column="1">
-                              <widget class="QLabel" name="conan_sys_version_value_label">
+                            <item row="0" column="1">
+                              <widget class="QLabel" name="conan_cur_version_value_label">
                                 <property name="text">
                                   <string>Unknown</string>
                                 </property>
                                 <property name="textInteractionFlags">
                                   <set>Qt::LinksAccessibleByMouse|Qt::TextSelectableByKeyboard|Qt::TextSelectableByMouse</set>
                                 </property>
                               </widget>
                             </item>
-                            <item row="3" column="0">
-                              <widget class="QLabel" name="python_sys_version_label">
-                                <property name="text">
-                                  <string>System Python Version:</string>
-                                </property>
-                              </widget>
-                            </item>
-                            <item row="3" column="1">
-                              <widget class="QLabel" name="python_sys_version_value_label">
+                            <item row="1" column="0">
+                              <widget class="QLabel" name="python_cur_version_label">
                                 <property name="text">
-                                  <string>Unknown</string>
+                                  <string>Current Python Version:</string>
                                 </property>
                               </widget>
                             </item>
                           </layout>
                         </widget>
                       </item>
                       <item>
@@ -489,14 +475,17 @@
                           </spacer>
                         </item>
                       </layout>
                     </widget>
                   </item>
                   <item row="1" column="0">
                     <widget class="QTextBrowser" name="profiles_text_browser">
+                      <property name="undoRedoEnabled">
+                        <bool>true</bool>
+                      </property>
                       <property name="readOnly">
                         <bool>false</bool>
                       </property>
                     </widget>
                   </item>
                 </layout>
               </item>
@@ -508,14 +497,17 @@
             </attribute>
             <layout class="QVBoxLayout" name="verticalLayout_3">
               <item>
                 <widget class="QTextBrowser" name="config_file_text_browser">
                   <property name="tabChangesFocus">
                     <bool>false</bool>
                   </property>
+                  <property name="undoRedoEnabled">
+                    <bool>true</bool>
+                  </property>
                   <property name="readOnly">
                     <bool>false</bool>
                   </property>
                 </widget>
               </item>
               <item>
                 <widget class="QFrame" name="config_btns_frame">
```

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/conan_conf/conan_conf_ui.py` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/conan_conf/conan_conf_ui.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 ################################################################################
 ## Form generated from reading UI file 'conan_conf.ui'
 ##
-## Created by: Qt User Interface Compiler version 6.4.2
+## Created by: Qt User Interface Compiler version 6.4.3
 ##
 ## WARNING! All changes made in this file will be lost when recompiling UI file!
 ################################################################################
 
 from PySide6.QtCore import (QCoreApplication, QDate, QDateTime, QLocale,
     QMetaObject, QObject, QPoint, QRect,
     QSize, QTime, QUrl, Qt)
@@ -49,56 +49,46 @@
         self.info_contents.setGeometry(QRect(0, 0, 608, 431))
         self.verticalLayout_7 = QVBoxLayout(self.info_contents)
         self.verticalLayout_7.setObjectName(u"verticalLayout_7")
         self.versions_box = QGroupBox(self.info_contents)
         self.versions_box.setObjectName(u"versions_box")
         self.gridLayout = QGridLayout(self.versions_box)
         self.gridLayout.setObjectName(u"gridLayout")
+        self.python_exe_label = QLabel(self.versions_box)
+        self.python_exe_label.setObjectName(u"python_exe_label")
+
+        self.gridLayout.addWidget(self.python_exe_label, 2, 0, 1, 1)
+
+        self.python_exe_value_label = QLabel(self.versions_box)
+        self.python_exe_value_label.setObjectName(u"python_exe_value_label")
+        self.python_exe_value_label.setTextInteractionFlags(Qt.LinksAccessibleByMouse|Qt.TextSelectableByKeyboard|Qt.TextSelectableByMouse)
+
+        self.gridLayout.addWidget(self.python_exe_value_label, 2, 1, 1, 1)
+
         self.conan_cur_version_label = QLabel(self.versions_box)
         self.conan_cur_version_label.setObjectName(u"conan_cur_version_label")
 
         self.gridLayout.addWidget(self.conan_cur_version_label, 0, 0, 1, 1)
 
+        self.python_cur_version_value_label = QLabel(self.versions_box)
+        self.python_cur_version_value_label.setObjectName(u"python_cur_version_value_label")
+
+        self.gridLayout.addWidget(self.python_cur_version_value_label, 1, 1, 1, 1)
+
         self.conan_cur_version_value_label = QLabel(self.versions_box)
         self.conan_cur_version_value_label.setObjectName(u"conan_cur_version_value_label")
         self.conan_cur_version_value_label.setTextInteractionFlags(Qt.LinksAccessibleByMouse|Qt.TextSelectableByKeyboard|Qt.TextSelectableByMouse)
 
         self.gridLayout.addWidget(self.conan_cur_version_value_label, 0, 1, 1, 1)
 
         self.python_cur_version_label = QLabel(self.versions_box)
         self.python_cur_version_label.setObjectName(u"python_cur_version_label")
 
         self.gridLayout.addWidget(self.python_cur_version_label, 1, 0, 1, 1)
 
-        self.python_cur_version_value_label = QLabel(self.versions_box)
-        self.python_cur_version_value_label.setObjectName(u"python_cur_version_value_label")
-
-        self.gridLayout.addWidget(self.python_cur_version_value_label, 1, 1, 1, 1)
-
-        self.conan_sys_version_label = QLabel(self.versions_box)
-        self.conan_sys_version_label.setObjectName(u"conan_sys_version_label")
-
-        self.gridLayout.addWidget(self.conan_sys_version_label, 2, 0, 1, 1)
-
-        self.conan_sys_version_value_label = QLabel(self.versions_box)
-        self.conan_sys_version_value_label.setObjectName(u"conan_sys_version_value_label")
-        self.conan_sys_version_value_label.setTextInteractionFlags(Qt.LinksAccessibleByMouse|Qt.TextSelectableByKeyboard|Qt.TextSelectableByMouse)
-
-        self.gridLayout.addWidget(self.conan_sys_version_value_label, 2, 1, 1, 1)
-
-        self.python_sys_version_label = QLabel(self.versions_box)
-        self.python_sys_version_label.setObjectName(u"python_sys_version_label")
-
-        self.gridLayout.addWidget(self.python_sys_version_label, 3, 0, 1, 1)
-
-        self.python_sys_version_value_label = QLabel(self.versions_box)
-        self.python_sys_version_value_label.setObjectName(u"python_sys_version_value_label")
-
-        self.gridLayout.addWidget(self.python_sys_version_value_label, 3, 1, 1, 1)
-
         self.gridLayout.setColumnStretch(0, 1)
         self.gridLayout.setColumnStretch(1, 2)
 
         self.verticalLayout_7.addWidget(self.versions_box)
 
         self.paths_box = QGroupBox(self.info_contents)
         self.paths_box.setObjectName(u"paths_box")
@@ -310,14 +300,15 @@
         self.verticalLayout_9.addItem(self.profiles_btns_spacer)
 
 
         self.profiles_layout.addWidget(self.profiles_buttons_frame, 0, 1, 2, 1)
 
         self.profiles_text_browser = QTextBrowser(self.profiles)
         self.profiles_text_browser.setObjectName(u"profiles_text_browser")
+        self.profiles_text_browser.setUndoRedoEnabled(True)
         self.profiles_text_browser.setReadOnly(False)
 
         self.profiles_layout.addWidget(self.profiles_text_browser, 1, 0, 1, 1)
 
 
         self.verticalLayout_5.addLayout(self.profiles_layout)
 
@@ -325,14 +316,15 @@
         self.config = QWidget()
         self.config.setObjectName(u"config")
         self.verticalLayout_3 = QVBoxLayout(self.config)
         self.verticalLayout_3.setObjectName(u"verticalLayout_3")
         self.config_file_text_browser = QTextBrowser(self.config)
         self.config_file_text_browser.setObjectName(u"config_file_text_browser")
         self.config_file_text_browser.setTabChangesFocus(False)
+        self.config_file_text_browser.setUndoRedoEnabled(True)
         self.config_file_text_browser.setReadOnly(False)
 
         self.verticalLayout_3.addWidget(self.config_file_text_browser)
 
         self.config_btns_frame = QFrame(self.config)
         self.config_btns_frame.setObjectName(u"config_btns_frame")
         self.config_btns_frame.setFrameShape(QFrame.StyledPanel)
@@ -366,31 +358,29 @@
         self.config_tab_widget.addTab(self.settings_file, "")
 
         self.verticalLayout.addWidget(self.config_tab_widget)
 
 
         self.retranslateUi(Form)
 
-        self.config_tab_widget.setCurrentIndex(0)
+        self.config_tab_widget.setCurrentIndex(3)
 
 
         QMetaObject.connectSlotsByName(Form)
     # setupUi
 
     def retranslateUi(self, Form):
         Form.setWindowTitle(QCoreApplication.translate("Form", u"Form", None))
         self.versions_box.setTitle(QCoreApplication.translate("Form", u"Versions", None))
+        self.python_exe_label.setText(QCoreApplication.translate("Form", u"Current Python Executable:", None))
+        self.python_exe_value_label.setText(QCoreApplication.translate("Form", u"Unknown", None))
         self.conan_cur_version_label.setText(QCoreApplication.translate("Form", u"Current Conan Version:", None))
+        self.python_cur_version_value_label.setText(QCoreApplication.translate("Form", u"Unknown", None))
         self.conan_cur_version_value_label.setText(QCoreApplication.translate("Form", u"Unknown", None))
         self.python_cur_version_label.setText(QCoreApplication.translate("Form", u"Current Python Version:", None))
-        self.python_cur_version_value_label.setText(QCoreApplication.translate("Form", u"Unknown", None))
-        self.conan_sys_version_label.setText(QCoreApplication.translate("Form", u"System Conan Version:", None))
-        self.conan_sys_version_value_label.setText(QCoreApplication.translate("Form", u"Unknown", None))
-        self.python_sys_version_label.setText(QCoreApplication.translate("Form", u"System Python Version:", None))
-        self.python_sys_version_value_label.setText(QCoreApplication.translate("Form", u"Unknown", None))
         self.paths_box.setTitle(QCoreApplication.translate("Form", u"Paths", None))
         self.conan_usr_home_label.setText(QCoreApplication.translate("Form", u"Conan User Home:", None))
         self.conan_usr_home_value_label.setText("")
         self.conan_storage_path_label.setText(QCoreApplication.translate("Form", u"Conan Storage Path:", None))
         self.conan_storage_path_value_label.setText("")
         self.conan_usr_cache_label.setText(QCoreApplication.translate("Form", u"Conan Short Path Cache:", None))
         self.conan_usr_cache_value_label.setText("")
```

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/conan_conf/controller.py` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/conan_conf/controller.py`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/conan_conf/dialogs/remote_edit_dialog.py` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/conan_conf/dialogs/remote_edit_dialog.py`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/conan_conf/dialogs/remote_edit_dialog.ui` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/conan_conf/dialogs/remote_edit_dialog.ui`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/conan_conf/dialogs/remote_edit_dialog_ui.py` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/conan_conf/dialogs/remote_edit_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/conan_conf/dialogs/remote_login_dialog.py` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/conan_conf/dialogs/remote_login_dialog.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 
 from pathlib import Path
 from typing import List, Optional
 
-import conan_app_launcher.app as app  # using global module pattern
-from conan_app_launcher import asset_path
+import conan_app_launcher.app as app
+from conan_app_launcher.app.loading import AsyncLoader  # using global module pattern
 from conan_app_launcher.app.logger import Logger
 from conans.client.cache.remote_registry import Remote
-from conan_app_launcher.ui.common import AsyncLoader
 from PySide6.QtCore import Qt
 from PySide6.QtGui import QIcon
 from PySide6.QtWidgets import QDialog, QWidget, QListWidgetItem
 
 from conan_app_launcher.ui.common.theming import get_themed_asset_icon
```

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/conan_conf/dialogs/remote_login_dialog.ui` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/conan_conf/dialogs/remote_login_dialog.ui`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/conan_conf/dialogs/remote_login_dialog_ui.py` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/conan_conf/dialogs/remote_login_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/conan_conf/model.py` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/conan_conf/model.py`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/conan_search/conan_search.py` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/conan_search/conan_search.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import TYPE_CHECKING, Optional
 
-import conan_app_launcher.app as app  # using global module pattern
+import conan_app_launcher.app as app
+from conan_app_launcher.ui.common.syntax_highlighting import ConfigHighlighter  # using global module pattern
 from conan_app_launcher.ui.plugin.plugins import PluginDescription, PluginInterfaceV1
 from conan_app_launcher.ui.views import LocalConanPackageExplorer
 from conan_app_launcher.ui.widgets import RoundedMenu
 from PySide6.QtCore import QPoint, Qt, Slot, QPropertyAnimation, QEasingCurve
 from PySide6.QtGui import QAction, QShortcut
 from PySide6.QtWidgets import QListWidgetItem, QWidget
 
@@ -54,15 +55,15 @@
             self._base_signals.conan_remotes_updated.connect(self._init_remotes)
         self._ui.search_results_tree_view.setContextMenuPolicy(Qt.ContextMenuPolicy.CustomContextMenu)
         self._ui.search_results_tree_view.customContextMenuRequested.connect(self.on_pkg_context_menu_requested)
         self._init_pkg_context_menu()
         # force_light_mode for disabled icon in dark mode
         self.set_themed_icon(self._ui.search_button, "icons/search.svg", size=(20, 20), force_light_mode=True)
         self.set_themed_icon(self._ui.install_button, "icons/download_pkg.svg", size=(20, 20))
-
+        self._conan_config_highlighter = ConfigHighlighter(self._ui.package_info_text.document(), "yaml")
         self._ui.remote_list.setMinimumHeight(0)
         self._ui.remote_list.setMaximumHeight(0)
         self.remote_toggle_animation = QPropertyAnimation(self._ui.remote_list, b"maximumHeight")
 
         # animation for expanding/collapsing remote list
         def start_animation(checked):
             arrow_type = Qt.ArrowType.DownArrow if checked else Qt.ArrowType.RightArrow
```

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/conan_search/conan_search.ui` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/conan_search/conan_search.ui`

 * *Files 3% similar despite different names*

#### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/conan_search/conan_search.ui` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/conan_search/conan_search.ui`

```diff
@@ -2,16 +2,16 @@
 <ui version="4.0">
   <class>Form</class>
   <widget class="QWidget" name="Form">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
-        <width>447</width>
-        <height>532</height>
+        <width>432</width>
+        <height>391</height>
       </rect>
     </property>
     <property name="windowTitle">
       <string>Conan Search</string>
     </property>
     <property name="styleSheet">
       <string notr="true"/>
@@ -229,32 +229,29 @@
           </property>
           <property name="sortingEnabled">
             <bool>true</bool>
           </property>
         </widget>
       </item>
       <item>
-        <widget class="QSplitter" name="views_splitter">
-          <property name="sizePolicy">
-            <sizepolicy hsizetype="MinimumExpanding" vsizetype="Expanding">
-              <horstretch>0</horstretch>
-              <verstretch>0</verstretch>
-            </sizepolicy>
-          </property>
+        <widget class="QSplitter" name="splitter">
           <property name="orientation">
-            <enum>Qt::Vertical</enum>
+            <enum>Qt::Horizontal</enum>
           </property>
           <property name="childrenCollapsible">
             <bool>false</bool>
           </property>
           <widget class="QWidget" name="layoutWidget_2">
-            <layout class="QVBoxLayout" name="results_layout" stretch="4,1">
+            <layout class="QVBoxLayout" name="results_layout" stretch="0,0">
               <property name="sizeConstraint">
                 <enum>QLayout::SetMinAndMaxSize</enum>
               </property>
+              <property name="leftMargin">
+                <number>4</number>
+              </property>
               <item>
                 <widget class="QLabel" name="results_label">
                   <property name="sizePolicy">
                     <sizepolicy hsizetype="Preferred" vsizetype="Fixed">
                       <horstretch>0</horstretch>
                       <verstretch>0</verstretch>
                     </sizepolicy>
@@ -268,15 +265,15 @@
                     <string>Results</string>
                   </property>
                 </widget>
               </item>
               <item>
                 <widget class="QTreeView" name="search_results_tree_view">
                   <property name="sizePolicy">
-                    <sizepolicy hsizetype="Expanding" vsizetype="Preferred">
+                    <sizepolicy hsizetype="Preferred" vsizetype="Preferred">
                       <horstretch>0</horstretch>
                       <verstretch>0</verstretch>
                     </sizepolicy>
                   </property>
                   <property name="frameShape">
                     <enum>QFrame::NoFrame</enum>
                   </property>
@@ -294,17 +291,20 @@
             </layout>
           </widget>
           <widget class="QWidget" name="layoutWidget_3">
             <layout class="QVBoxLayout" name="pkg_info_layout" stretch="0,0">
               <property name="sizeConstraint">
                 <enum>QLayout::SetMinAndMaxSize</enum>
               </property>
-              <property name="topMargin">
+              <property name="leftMargin">
                 <number>4</number>
               </property>
+              <property name="topMargin">
+                <number>0</number>
+              </property>
               <item>
                 <widget class="QLabel" name="package_info_label">
                   <property name="sizePolicy">
                     <sizepolicy hsizetype="Preferred" vsizetype="Fixed">
                       <horstretch>0</horstretch>
                       <verstretch>0</verstretch>
                     </sizepolicy>
@@ -337,18 +337,21 @@
                     <sizepolicy hsizetype="Preferred" vsizetype="Preferred">
                       <horstretch>0</horstretch>
                       <verstretch>0</verstretch>
                     </sizepolicy>
                   </property>
                   <property name="minimumSize">
                     <size>
-                      <width>0</width>
+                      <width>200</width>
                       <height>20</height>
                     </size>
                   </property>
+                  <property name="frameShape">
+                    <enum>QFrame::NoFrame</enum>
+                  </property>
                   <property name="sizeAdjustPolicy">
                     <enum>QAbstractScrollArea::AdjustToContents</enum>
                   </property>
                 </widget>
               </item>
             </layout>
           </widget>
```

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/conan_search/conan_search_ui.py` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/conan_search/conan_search_ui.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 ################################################################################
 ## Form generated from reading UI file 'conan_search.ui'
 ##
-## Created by: Qt User Interface Compiler version 6.4.2
+## Created by: Qt User Interface Compiler version 6.4.3
 ##
 ## WARNING! All changes made in this file will be lost when recompiling UI file!
 ################################################################################
 
 from PySide6.QtCore import (QCoreApplication, QDate, QDateTime, QLocale,
     QMetaObject, QObject, QPoint, QRect,
     QSize, QTime, QUrl, Qt)
@@ -23,15 +23,15 @@
 
 from conan_app_launcher.ui.widgets.conan_line_edit import ConanRefLineEdit
 
 class Ui_Form(object):
     def setupUi(self, Form):
         if not Form.objectName():
             Form.setObjectName(u"Form")
-        Form.resize(447, 532)
+        Form.resize(432, 391)
         Form.setStyleSheet(u"")
         self.verticalLayout = QVBoxLayout(Form)
         self.verticalLayout.setObjectName(u"verticalLayout")
         self.search_text_button_layout = QHBoxLayout()
         self.search_text_button_layout.setObjectName(u"search_text_button_layout")
         self.search_text_button_layout.setSizeConstraint(QLayout.SetDefaultConstraint)
         self.search_line = ConanRefLineEdit(Form)
@@ -127,90 +127,81 @@
         self.remote_list.setLayoutMode(QListView.Batched)
         self.remote_list.setUniformItemSizes(True)
         self.remote_list.setSelectionRectVisible(True)
         self.remote_list.setSortingEnabled(True)
 
         self.verticalLayout.addWidget(self.remote_list)
 
-        self.views_splitter = QSplitter(Form)
-        self.views_splitter.setObjectName(u"views_splitter")
-        sizePolicy3 = QSizePolicy(QSizePolicy.MinimumExpanding, QSizePolicy.Expanding)
-        sizePolicy3.setHorizontalStretch(0)
-        sizePolicy3.setVerticalStretch(0)
-        sizePolicy3.setHeightForWidth(self.views_splitter.sizePolicy().hasHeightForWidth())
-        self.views_splitter.setSizePolicy(sizePolicy3)
-        self.views_splitter.setOrientation(Qt.Vertical)
-        self.views_splitter.setChildrenCollapsible(False)
-        self.layoutWidget_2 = QWidget(self.views_splitter)
+        self.splitter = QSplitter(Form)
+        self.splitter.setObjectName(u"splitter")
+        self.splitter.setOrientation(Qt.Horizontal)
+        self.splitter.setChildrenCollapsible(False)
+        self.layoutWidget_2 = QWidget(self.splitter)
         self.layoutWidget_2.setObjectName(u"layoutWidget_2")
         self.results_layout = QVBoxLayout(self.layoutWidget_2)
         self.results_layout.setObjectName(u"results_layout")
         self.results_layout.setSizeConstraint(QLayout.SetMinAndMaxSize)
-        self.results_layout.setContentsMargins(0, 0, 0, 0)
+        self.results_layout.setContentsMargins(4, 0, 0, 0)
         self.results_label = QLabel(self.layoutWidget_2)
         self.results_label.setObjectName(u"results_label")
-        sizePolicy4 = QSizePolicy(QSizePolicy.Preferred, QSizePolicy.Fixed)
-        sizePolicy4.setHorizontalStretch(0)
-        sizePolicy4.setVerticalStretch(0)
-        sizePolicy4.setHeightForWidth(self.results_label.sizePolicy().hasHeightForWidth())
-        self.results_label.setSizePolicy(sizePolicy4)
+        sizePolicy3 = QSizePolicy(QSizePolicy.Preferred, QSizePolicy.Fixed)
+        sizePolicy3.setHorizontalStretch(0)
+        sizePolicy3.setVerticalStretch(0)
+        sizePolicy3.setHeightForWidth(self.results_label.sizePolicy().hasHeightForWidth())
+        self.results_label.setSizePolicy(sizePolicy3)
         font = QFont()
         font.setBold(True)
         self.results_label.setFont(font)
 
         self.results_layout.addWidget(self.results_label)
 
         self.search_results_tree_view = QTreeView(self.layoutWidget_2)
         self.search_results_tree_view.setObjectName(u"search_results_tree_view")
-        sizePolicy5 = QSizePolicy(QSizePolicy.Expanding, QSizePolicy.Preferred)
-        sizePolicy5.setHorizontalStretch(0)
-        sizePolicy5.setVerticalStretch(0)
-        sizePolicy5.setHeightForWidth(self.search_results_tree_view.sizePolicy().hasHeightForWidth())
-        self.search_results_tree_view.setSizePolicy(sizePolicy5)
+        sizePolicy4 = QSizePolicy(QSizePolicy.Preferred, QSizePolicy.Preferred)
+        sizePolicy4.setHorizontalStretch(0)
+        sizePolicy4.setVerticalStretch(0)
+        sizePolicy4.setHeightForWidth(self.search_results_tree_view.sizePolicy().hasHeightForWidth())
+        self.search_results_tree_view.setSizePolicy(sizePolicy4)
         self.search_results_tree_view.setFrameShape(QFrame.NoFrame)
         self.search_results_tree_view.setSizeAdjustPolicy(QAbstractScrollArea.AdjustIgnored)
         self.search_results_tree_view.setSortingEnabled(True)
         self.search_results_tree_view.setAnimated(True)
 
         self.results_layout.addWidget(self.search_results_tree_view)
 
-        self.results_layout.setStretch(0, 4)
-        self.results_layout.setStretch(1, 1)
-        self.views_splitter.addWidget(self.layoutWidget_2)
-        self.layoutWidget_3 = QWidget(self.views_splitter)
+        self.splitter.addWidget(self.layoutWidget_2)
+        self.layoutWidget_3 = QWidget(self.splitter)
         self.layoutWidget_3.setObjectName(u"layoutWidget_3")
         self.pkg_info_layout = QVBoxLayout(self.layoutWidget_3)
         self.pkg_info_layout.setObjectName(u"pkg_info_layout")
         self.pkg_info_layout.setSizeConstraint(QLayout.SetMinAndMaxSize)
-        self.pkg_info_layout.setContentsMargins(0, 4, 0, 0)
+        self.pkg_info_layout.setContentsMargins(4, 0, 0, 0)
         self.package_info_label = QLabel(self.layoutWidget_3)
         self.package_info_label.setObjectName(u"package_info_label")
-        sizePolicy4.setHeightForWidth(self.package_info_label.sizePolicy().hasHeightForWidth())
-        self.package_info_label.setSizePolicy(sizePolicy4)
+        sizePolicy3.setHeightForWidth(self.package_info_label.sizePolicy().hasHeightForWidth())
+        self.package_info_label.setSizePolicy(sizePolicy3)
         self.package_info_label.setMinimumSize(QSize(20, 0))
         self.package_info_label.setBaseSize(QSize(20, 0))
         self.package_info_label.setFont(font)
 
         self.pkg_info_layout.addWidget(self.package_info_label)
 
         self.package_info_text = QTextBrowser(self.layoutWidget_3)
         self.package_info_text.setObjectName(u"package_info_text")
-        sizePolicy6 = QSizePolicy(QSizePolicy.Preferred, QSizePolicy.Preferred)
-        sizePolicy6.setHorizontalStretch(0)
-        sizePolicy6.setVerticalStretch(0)
-        sizePolicy6.setHeightForWidth(self.package_info_text.sizePolicy().hasHeightForWidth())
-        self.package_info_text.setSizePolicy(sizePolicy6)
-        self.package_info_text.setMinimumSize(QSize(0, 20))
+        sizePolicy4.setHeightForWidth(self.package_info_text.sizePolicy().hasHeightForWidth())
+        self.package_info_text.setSizePolicy(sizePolicy4)
+        self.package_info_text.setMinimumSize(QSize(200, 20))
+        self.package_info_text.setFrameShape(QFrame.NoFrame)
         self.package_info_text.setSizeAdjustPolicy(QAbstractScrollArea.AdjustToContents)
 
         self.pkg_info_layout.addWidget(self.package_info_text)
 
-        self.views_splitter.addWidget(self.layoutWidget_3)
+        self.splitter.addWidget(self.layoutWidget_3)
 
-        self.verticalLayout.addWidget(self.views_splitter)
+        self.verticalLayout.addWidget(self.splitter)
 
 
         self.retranslateUi(Form)
 
         QMetaObject.connectSlotsByName(Form)
     # setupUi
```

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/conan_search/controller.py` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/conan_search/controller.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import pprint
 from typing import TYPE_CHECKING, List, Optional
 
-import conan_app_launcher.app as app  # using global module pattern
-from conan_app_launcher.ui.common import AsyncLoader, show_conanfile
+from conan_app_launcher.app.loading import AsyncLoader  # using global module pattern
+from conan_app_launcher.ui.common import show_conanfile
 from conan_app_launcher.ui.dialogs import ConanInstallDialog
-from conan_app_launcher.core.conan_common import ConanRef
 from PySide6.QtCore import Qt, SignalInstance, QObject
-from PySide6.QtWidgets import (QApplication, QTreeView, QLineEdit, QPushButton, QTextBrowser, QListWidget)
+from PySide6.QtWidgets import (QApplication, QTreeView, QPushButton, QTextBrowser, QListWidget)
+
+from conan_app_launcher.ui.widgets.conan_line_edit import ConanRefLineEdit
 
 from .model import PROFILE_TYPE, PkgSearchModel, SearchedPackageTreeItem
 if TYPE_CHECKING:
     from conan_app_launcher.ui.main_window import BaseSignals
 
 class ConanSearchController(QObject):
 
-    def __init__(self, view: QTreeView, search_line: QLineEdit, search_button: QPushButton, remote_list: QListWidget, 
+    def __init__(self, view: QTreeView, search_line: ConanRefLineEdit, search_button: QPushButton, remote_list: QListWidget, 
                  detail_view: QTextBrowser, conan_pkg_installed: Optional[SignalInstance], 
                  conan_pkg_removed: Optional[SignalInstance]) -> None:
         super().__init__(view)
         self._view = view
         self._search_line = search_line
         self._search_button = search_button
         self._remote_list = remote_list
@@ -48,14 +49,15 @@
 
     def _finish_load_search_model(self):
         """ After conan search adjust the view """
         self._view.setModel(self._model.proxy_model)
         self._resize_package_columns()
         self._view.sortByColumn(1, Qt.SortOrder.AscendingOrder)  # sort by remote at default
         self._view.selectionModel().selectionChanged.connect(self.on_package_selected)
+        self._search_line.load_completion_refs()
 
     def on_package_selected(self):
         """ Display package info only for pkg ref"""
         item = self.get_selected_source_item(self._view)
         if not item:
             return
         if item.type != PROFILE_TYPE:
```

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/conan_search/model.py` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/conan_search/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 from typing import Dict, List, Optional
 
-import conan_app_launcher.app as app  # using global module pattern
+import conan_app_launcher.app as app
+from conan_app_launcher.app.loading import AsyncLoader  # using global module pattern
 from conan_app_launcher.app.logger import Logger
-from conan_app_launcher.core import ConanApi
-from conan_app_launcher.core.conan_common import ConanPkg
+from conan_app_launcher.conan_wrapper import ConanApi
+from conan_app_launcher.conan_wrapper.types import ConanPkg
 from conan_app_launcher.ui.common import TreeModel, TreeModelItem, get_platform_icon, get_themed_asset_icon
-from conan_app_launcher.core.conan_common import ConanRef
+from conan_app_launcher.conan_wrapper.types import ConanRef
 from PySide6 import QtCore, QtGui, QtWidgets
 from PySide6.QtCore import Qt, Slot, SignalInstance
 
-from conan_app_launcher.ui.common.loading import AsyncLoader
-
 REF_TYPE = 0
 PROFILE_TYPE = 1
 
 
 class SearchedPackageTreeItem(TreeModelItem):
     """
     Represents a tree item of a Conan pkg.
@@ -104,14 +103,15 @@
                     recipes_with_remotes[recipe] = remote
 
         if not recipes_with_remotes:
             self.root_item.append_child(SearchedPackageTreeItem(
                 ["No package found!", "", ""], self.root_item, None, PROFILE_TYPE, empty=True))
             return
 
+        # add info if it is installed
         installed_refs = app.conan_api.get_all_local_refs()
         for recipe in recipes_with_remotes:
             recipe_remotes = recipes_with_remotes.get(recipe, "")
             installed = False
             if recipe in installed_refs:
                 installed = True
             conan_item = SearchedPackageTreeItem(
```

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/package_explorer/controller.py` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/package_explorer/controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 import os
 from pathlib import Path
 from typing import TYPE_CHECKING, Optional, Tuple
 
-import conan_app_launcher.app as app  # using global module pattern
+import conan_app_launcher.app as app
+from conan_app_launcher.app.loading import AsyncLoader  # using global module pattern
 from conan_app_launcher.app.logger import Logger
-from conan_app_launcher.core import (open_cmd_in_path, open_file,
-                                     open_in_file_manager, run_file)
-from conan_app_launcher.core.conan_common import ConanPkg, ConanRef
-from conan_app_launcher.core.system import (calc_paste_same_dir_name,
-                                            copy_path_with_overwrite,
-                                            delete_path, execute_cmd)
+from conan_app_launcher.conan_wrapper.types import ConanPkg, ConanRef
+from conan_app_launcher.app.system import (calc_paste_same_dir_name,
+                                           copy_path_with_overwrite,
+                                           delete_path, execute_cmd, open_cmd_in_path, open_in_file_manager, run_file)
 from conan_app_launcher.settings import FILE_EDITOR_EXECUTABLE
-from conan_app_launcher.ui.common import AsyncLoader, FileSystemModel, show_conanfile
+from conan_app_launcher.ui.common import FileSystemModel, show_conanfile
 from conan_app_launcher.ui.common.model import re_register_signal
 from conan_app_launcher.ui.config import UiAppLinkConfig
 from conan_app_launcher.ui.dialogs import ConanRemoveDialog
 from conan_app_launcher.ui.dialogs.conan_install.conan_install import ConanInstallDialog
 from conan_app_launcher.ui.views import AppGridView
 from PySide6.QtCore import (QItemSelectionModel, QMimeData, QModelIndex, QObject,
-                          Qt, QUrl, SignalInstance)
+                            Qt, QUrl, SignalInstance)
 from PySide6.QtWidgets import (QAbstractItemView, QApplication, QLabel,
-                             QLineEdit, QMessageBox, QTreeView, QWidget)
+                               QLineEdit, QMessageBox, QTreeView, QWidget)
 
 from .model import (PROFILE_TYPE, REF_TYPE, PackageFilter, PackageTreeItem,
                     PkgSelectModel)
 
 if TYPE_CHECKING:
     from conan_app_launcher.ui.fluent_window import FluentWindow
     from conan_app_launcher.ui.main_window import BaseSignals
@@ -62,17 +61,17 @@
     def get_selected_pkg_source_item(self) -> Optional[PackageTreeItem]:
         indexes = self._view.selectedIndexes()
         if len(indexes) != 1:
             Logger().debug(f"Mismatch in selected items for context action: {str(len(indexes))}")
             return None
         view_index = self._view.selectedIndexes()[0]
         model: PackageFilter = view_index.model()  # type: ignore
-        source_item: PackageTreeItem = model.mapToSource(view_index).internalPointer() # type: ignore
+        source_item: PackageTreeItem = model.mapToSource(view_index).internalPointer()  # type: ignore
         return source_item
-    
+
     def get_selected_ref_with_pkg_id(self) -> Tuple[str, str]:
         conan_ref = self.get_selected_conan_ref()
         pkg_info = self.get_selected_conan_pkg_info()
         pkg_id = ""
         if pkg_info:
             pkg_id = pkg_info.get("id", "")
         return conan_ref, pkg_id
@@ -194,15 +193,15 @@
         # map to package view model
         proxy_index = self._model.index(ref_row, 0, QModelIndex())
         sel_model = self._view.selectionModel()
         view_model: PackageFilter = self._view.model()  # type: ignore
         self._view.expand(view_model.mapFromSource(proxy_index))
 
         if pkg_id:
-            item: PackageTreeItem = proxy_index.internalPointer() # type: ignore
+            item: PackageTreeItem = proxy_index.internalPointer()  # type: ignore
             i = 0
             for i in range(len(item.child_items)):
                 if item.child_items[i].item_data[0].get("id", "") == pkg_id:
                     break
             internal_sel_index = self._model.index(i, 0, proxy_index)
         else:
             internal_sel_index = proxy_index
@@ -221,17 +220,18 @@
         if not source_item:
             return
         if source_item.type != PROFILE_TYPE:
             return
         conan_ref = self.get_selected_conan_ref()
         self._conan_pkg_selected.emit(conan_ref, self.get_selected_conan_pkg_info())
 
+
 class PackageFileExplorerController(QObject):
 
-    def __init__(self, parent: QWidget, view: QTreeView, pkg_path_label: QLabel, conan_pkg_selected: SignalInstance, 
+    def __init__(self, parent: QWidget, view: QTreeView, pkg_path_label: QLabel, conan_pkg_selected: SignalInstance,
                  base_signals: "BaseSignals", page_widgets: "FluentWindow.PageStore"):
         super().__init__(parent)
         self._model = None
         self._page_widgets = page_widgets
         self._view = view
         self._pkg_path_label = pkg_path_label
         self._base_signals = base_signals
@@ -260,15 +260,15 @@
         self._view.setColumnHidden(2, True)  # file type
         self._model.layoutChanged.connect(self.resize_file_columns)
         self._view.header().setSortIndicator(0, Qt.SortOrder.AscendingOrder)
         re_register_signal(self._view.doubleClicked, self.on_file_double_click)  # type: ignore
         # disable edit on double click, since we want to open
         self._view.setEditTriggers(QAbstractItemView.EditTrigger.EditKeyPressed)
         self._pkg_path_label.setText(str(pkg_path))
-
+        self._pkg_path_label.setAlignment(Qt.AlignmentFlag.AlignRight) # must be called after every text set
         self._view.setContextMenuPolicy(Qt.ContextMenuPolicy.CustomContextMenu)
         self.resize_file_columns()
 
     def on_conan_pkg_removed(self, conan_ref: str, pkg_id: str):
         # clear file view if this pkg is selected
         if self._current_ref == conan_ref:
             self.close_files_view()
@@ -403,22 +403,22 @@
 
     def get_selected_pkg_path(self) -> str:
         if not self._model:
             return ""
         file_view_index = self._get_pkg_file_source_item()
         # if nothing selected return root
         if not file_view_index:
-                return self._model.rootPath()
+            return self._model.rootPath()
         return self._model.fileInfo(file_view_index).absoluteFilePath()
 
     def _is_selected_item_expanded(self):
         file_view_index = self._get_pkg_file_source_item()
         # if nothing selected return root
         if not file_view_index:
-                return False
+            return False
         return self._view.isExpanded(file_view_index)
 
     def resize_file_columns(self):
         if self._view:
             self._view.resizeColumnToContents(3)
             self._view.resizeColumnToContents(2)
             self._view.resizeColumnToContents(1)
```

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/package_explorer/model.py` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/package_explorer/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pprint
 from typing import List
 
 import conan_app_launcher.app as app  # using global module pattern
-from conan_app_launcher.core import ConanApi
-from conan_app_launcher.core.conan_common import ConanPkg
+from conan_app_launcher.conan_wrapper import ConanApi
+from conan_app_launcher.conan_wrapper.types import ConanPkg
 from conan_app_launcher.ui.common import get_platform_icon, get_themed_asset_icon, TreeModel, TreeModelItem
 from PySide6.QtCore import QSortFilterProxyModel, Qt, QModelIndex
 from PySide6.QtGui import QIcon
 
 REF_TYPE = 0
 PROFILE_TYPE = 1
```

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/package_explorer/package_explorer.py` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/package_explorer/package_explorer.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,29 +43,30 @@
         self._ui.package_select_view.setContextMenuPolicy(Qt.ContextMenuPolicy.CustomContextMenu)
         self._ui.package_select_view.customContextMenuRequested.connect(
             self.on_selection_context_menu_requested)
         self._init_selection_context_menu()
         self._ui.refresh_button.clicked.connect(self._pkg_sel_ctrl.on_pkg_refresh_clicked)
         self._ui.package_filter_edit.textChanged.connect(self._pkg_sel_ctrl.set_filter_wildcard)
         self.conan_pkg_selected.connect(self.on_pkg_selection_change)
+        self._ui.package_path_label.setText("<Package path>")
+        self._ui.package_path_label.setAlignment(Qt.AlignmentFlag.AlignRight) # must be called after every text set
         self.updateGeometry()
         self.resize_filter()
 
     def on_pkg_selection_change(self, conan_ref, pkg):
         # init/update the context menu
         re_register_signal(self._ui.package_file_view.customContextMenuRequested,
                            self.on_file_context_menu_requested)
         self._init_pkg_file_context_menu()
 
     def showEvent(self, a0: QShowEvent) -> None:
         self._pkg_sel_ctrl.refresh_pkg_selection_view(update=False)  # only update the first time
         return super().showEvent(a0)
 
     def resizeEvent(self, a0: QResizeEvent) -> None:
-        self.resize_filter()
         self._pkg_file_exp_ctrl.resize_file_columns()
         super().resizeEvent(a0)
 
     def resize_filter(self):
         # resize filter splitter to roughly match file view splitter
         sizes = self._ui.splitter.sizes()
         offset = self._ui.package_filter_label.width() + self._ui.refresh_button.width()
```

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/package_explorer/package_explorer.ui` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/package_explorer/package_explorer.ui`

 * *Files 22% similar despite different names*

#### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/package_explorer/package_explorer.ui` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/package_explorer/package_explorer.ui`

```diff
@@ -2,36 +2,36 @@
 <ui version="4.0">
   <class>Form</class>
   <widget class="QWidget" name="Form">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
-        <width>716</width>
-        <height>573</height>
+        <width>546</width>
+        <height>330</height>
       </rect>
     </property>
     <property name="windowTitle">
       <string>Form</string>
     </property>
     <layout class="QVBoxLayout" name="verticalLayout">
       <property name="spacing">
-        <number>5</number>
+        <number>4</number>
       </property>
       <property name="leftMargin">
         <number>0</number>
       </property>
       <property name="topMargin">
         <number>0</number>
       </property>
       <property name="rightMargin">
         <number>0</number>
       </property>
       <property name="bottomMargin">
-        <number>0</number>
+        <number>3</number>
       </property>
       <item>
         <layout class="QHBoxLayout" name="local_packages_bar_layout">
           <property name="sizeConstraint">
             <enum>QLayout::SetMinimumSize</enum>
           </property>
           <property name="rightMargin">
@@ -97,14 +97,17 @@
                   <horstretch>1</horstretch>
                   <verstretch>1</verstretch>
                 </sizepolicy>
               </property>
               <property name="orientation">
                 <enum>Qt::Horizontal</enum>
               </property>
+              <property name="handleWidth">
+                <number>5</number>
+              </property>
               <property name="childrenCollapsible">
                 <bool>false</bool>
               </property>
               <widget class="QLineEdit" name="package_filter_edit">
                 <property name="enabled">
                   <bool>true</bool>
                 </property>
@@ -112,21 +115,21 @@
                   <sizepolicy hsizetype="Preferred" vsizetype="Minimum">
                     <horstretch>1</horstretch>
                     <verstretch>1</verstretch>
                   </sizepolicy>
                 </property>
                 <property name="minimumSize">
                   <size>
-                    <width>175</width>
+                    <width>150</width>
                     <height>32</height>
                   </size>
                 </property>
                 <property name="maximumSize">
                   <size>
-                    <width>400</width>
+                    <width>350</width>
                     <height>32</height>
                   </size>
                 </property>
                 <property name="font">
                   <font>
                     <pointsize>10</pointsize>
                   </font>
@@ -137,57 +140,61 @@
                 <property name="placeholderText">
                   <string>*</string>
                 </property>
                 <property name="clearButtonEnabled">
                   <bool>true</bool>
                 </property>
               </widget>
-              <widget class="QLabel" name="package_path_label">
+              <widget class="QTextBrowser" name="package_path_label">
                 <property name="sizePolicy">
-                  <sizepolicy hsizetype="Preferred" vsizetype="Fixed">
-                    <horstretch>5</horstretch>
-                    <verstretch>1</verstretch>
+                  <sizepolicy hsizetype="Expanding" vsizetype="Minimum">
+                    <horstretch>0</horstretch>
+                    <verstretch>0</verstretch>
                   </sizepolicy>
                 </property>
-                <property name="minimumSize">
-                  <size>
-                    <width>300</width>
-                    <height>32</height>
-                  </size>
-                </property>
                 <property name="maximumSize">
                   <size>
                     <width>16777215</width>
                     <height>32</height>
                   </size>
                 </property>
-                <property name="baseSize">
-                  <size>
-                    <width>500</width>
-                    <height>0</height>
-                  </size>
+                <property name="styleSheet">
+                  <string notr="true">text-align: right;</string>
                 </property>
-                <property name="text">
-                  <string/>
+                <property name="frameShape">
+                  <enum>QFrame::NoFrame</enum>
                 </property>
-                <property name="scaledContents">
-                  <bool>true</bool>
+                <property name="verticalScrollBarPolicy">
+                  <enum>Qt::ScrollBarAlwaysOff</enum>
                 </property>
-                <property name="alignment">
-                  <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
+                <property name="horizontalScrollBarPolicy">
+                  <enum>Qt::ScrollBarAlwaysOff</enum>
+                </property>
+                <property name="sizeAdjustPolicy">
+                  <enum>QAbstractScrollArea::AdjustToContents</enum>
+                </property>
+                <property name="autoFormatting">
+                  <set>QTextEdit::AutoNone</set>
+                </property>
+                <property name="lineWrapMode">
+                  <enum>QTextEdit::NoWrap</enum>
+                </property>
+                <property name="html">
+                  <string>&lt;!DOCTYPE HTML PUBLIC &quot;-//W3C//DTD HTML 4.0//EN&quot; &quot;http://www.w3.org/TR/REC-html40/strict.dtd&quot;&gt;
+&lt;html&gt;&lt;head&gt;&lt;meta name=&quot;qrichtext&quot; content=&quot;1&quot; /&gt;&lt;meta charset=&quot;utf-8&quot; /&gt;&lt;style type=&quot;text/css&quot;&gt;
+p, li { white-space: pre-wrap; }
+hr { height: 1px; border-width: 0; }
+li.unchecked::marker { content: &quot;\2610&quot;; }
+li.checked::marker { content: &quot;\2612&quot;; }
+&lt;/style&gt;&lt;/head&gt;&lt;body style=&quot; font-family:'Segoe UI'; font-size:9pt; font-weight:400; font-style:normal;&quot;&gt;
+&lt;p style=&quot;-qt-paragraph-type:empty; margin-top:0px; margin-bottom:0px; margin-left:0px; margin-right:0px; -qt-block-indent:0; text-indent:0px;&quot;&gt;&lt;br /&gt;&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
                 </property>
-                <property name="wordWrap">
+                <property name="overwriteMode">
                   <bool>false</bool>
                 </property>
-                <property name="openExternalLinks">
-                  <bool>true</bool>
-                </property>
-                <property name="textInteractionFlags">
-                  <set>Qt::LinksAccessibleByMouse|Qt::TextSelectableByKeyboard|Qt::TextSelectableByMouse</set>
-                </property>
               </widget>
             </widget>
           </item>
         </layout>
       </item>
       <item>
         <widget class="QSplitter" name="splitter">
```

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/package_explorer/package_explorer_ui.py` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/package_explorer/package_explorer_ui.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 # -*- coding: utf-8 -*-
 
 ################################################################################
 ## Form generated from reading UI file 'package_explorer.ui'
 ##
-## Created by: Qt User Interface Compiler version 6.4.2
+## Created by: Qt User Interface Compiler version 6.4.3
 ##
 ## WARNING! All changes made in this file will be lost when recompiling UI file!
 ################################################################################
 
 from PySide6.QtCore import (QCoreApplication, QDate, QDateTime, QLocale,
     QMetaObject, QObject, QPoint, QRect,
     QSize, QTime, QUrl, Qt)
 from PySide6.QtGui import (QBrush, QColor, QConicalGradient, QCursor,
     QFont, QFontDatabase, QGradient, QIcon,
     QImage, QKeySequence, QLinearGradient, QPainter,
     QPalette, QPixmap, QRadialGradient, QTransform)
 from PySide6.QtWidgets import (QAbstractItemView, QAbstractScrollArea, QApplication, QFrame,
     QHBoxLayout, QHeaderView, QLabel, QLayout,
     QLineEdit, QPushButton, QSizePolicy, QSplitter,
-    QTreeView, QVBoxLayout, QWidget)
+    QTextBrowser, QTextEdit, QTreeView, QVBoxLayout,
+    QWidget)
 
 class Ui_Form(object):
     def setupUi(self, Form):
         if not Form.objectName():
             Form.setObjectName(u"Form")
-        Form.resize(716, 573)
+        Form.resize(546, 330)
         self.verticalLayout = QVBoxLayout(Form)
-        self.verticalLayout.setSpacing(5)
+        self.verticalLayout.setSpacing(4)
         self.verticalLayout.setObjectName(u"verticalLayout")
-        self.verticalLayout.setContentsMargins(0, 0, 0, 0)
+        self.verticalLayout.setContentsMargins(0, 0, 0, 3)
         self.local_packages_bar_layout = QHBoxLayout()
         self.local_packages_bar_layout.setObjectName(u"local_packages_bar_layout")
         self.local_packages_bar_layout.setSizeConstraint(QLayout.SetMinimumSize)
         self.local_packages_bar_layout.setContentsMargins(-1, -1, 7, -1)
         self.refresh_button = QPushButton(Form)
         self.refresh_button.setObjectName(u"refresh_button")
         sizePolicy = QSizePolicy(QSizePolicy.Preferred, QSizePolicy.Preferred)
@@ -61,46 +62,48 @@
         self.splitter_filter.setObjectName(u"splitter_filter")
         sizePolicy2 = QSizePolicy(QSizePolicy.Expanding, QSizePolicy.Preferred)
         sizePolicy2.setHorizontalStretch(1)
         sizePolicy2.setVerticalStretch(1)
         sizePolicy2.setHeightForWidth(self.splitter_filter.sizePolicy().hasHeightForWidth())
         self.splitter_filter.setSizePolicy(sizePolicy2)
         self.splitter_filter.setOrientation(Qt.Horizontal)
+        self.splitter_filter.setHandleWidth(5)
         self.splitter_filter.setChildrenCollapsible(False)
         self.package_filter_edit = QLineEdit(self.splitter_filter)
         self.package_filter_edit.setObjectName(u"package_filter_edit")
         self.package_filter_edit.setEnabled(True)
         sizePolicy3 = QSizePolicy(QSizePolicy.Preferred, QSizePolicy.Minimum)
         sizePolicy3.setHorizontalStretch(1)
         sizePolicy3.setVerticalStretch(1)
         sizePolicy3.setHeightForWidth(self.package_filter_edit.sizePolicy().hasHeightForWidth())
         self.package_filter_edit.setSizePolicy(sizePolicy3)
-        self.package_filter_edit.setMinimumSize(QSize(175, 32))
-        self.package_filter_edit.setMaximumSize(QSize(400, 32))
+        self.package_filter_edit.setMinimumSize(QSize(150, 32))
+        self.package_filter_edit.setMaximumSize(QSize(350, 32))
         font = QFont()
         font.setPointSize(10)
         self.package_filter_edit.setFont(font)
         self.package_filter_edit.setInputMethodHints(Qt.ImhNone)
         self.package_filter_edit.setClearButtonEnabled(True)
         self.splitter_filter.addWidget(self.package_filter_edit)
-        self.package_path_label = QLabel(self.splitter_filter)
+        self.package_path_label = QTextBrowser(self.splitter_filter)
         self.package_path_label.setObjectName(u"package_path_label")
-        sizePolicy4 = QSizePolicy(QSizePolicy.Preferred, QSizePolicy.Fixed)
-        sizePolicy4.setHorizontalStretch(5)
-        sizePolicy4.setVerticalStretch(1)
+        sizePolicy4 = QSizePolicy(QSizePolicy.Expanding, QSizePolicy.Minimum)
+        sizePolicy4.setHorizontalStretch(0)
+        sizePolicy4.setVerticalStretch(0)
         sizePolicy4.setHeightForWidth(self.package_path_label.sizePolicy().hasHeightForWidth())
         self.package_path_label.setSizePolicy(sizePolicy4)
-        self.package_path_label.setMinimumSize(QSize(300, 32))
         self.package_path_label.setMaximumSize(QSize(16777215, 32))
-        self.package_path_label.setBaseSize(QSize(500, 0))
-        self.package_path_label.setScaledContents(True)
-        self.package_path_label.setAlignment(Qt.AlignRight|Qt.AlignTrailing|Qt.AlignVCenter)
-        self.package_path_label.setWordWrap(False)
-        self.package_path_label.setOpenExternalLinks(True)
-        self.package_path_label.setTextInteractionFlags(Qt.LinksAccessibleByMouse|Qt.TextSelectableByKeyboard|Qt.TextSelectableByMouse)
+        self.package_path_label.setStyleSheet(u"text-align: right;")
+        self.package_path_label.setFrameShape(QFrame.NoFrame)
+        self.package_path_label.setVerticalScrollBarPolicy(Qt.ScrollBarAlwaysOff)
+        self.package_path_label.setHorizontalScrollBarPolicy(Qt.ScrollBarAlwaysOff)
+        self.package_path_label.setSizeAdjustPolicy(QAbstractScrollArea.AdjustToContents)
+        self.package_path_label.setAutoFormatting(QTextEdit.AutoNone)
+        self.package_path_label.setLineWrapMode(QTextEdit.NoWrap)
+        self.package_path_label.setOverwriteMode(False)
         self.splitter_filter.addWidget(self.package_path_label)
 
         self.local_packages_bar_layout.addWidget(self.splitter_filter)
 
 
         self.verticalLayout.addLayout(self.local_packages_bar_layout)
 
@@ -161,10 +164,17 @@
         Form.setWindowTitle(QCoreApplication.translate("Form", u"Form", None))
 #if QT_CONFIG(tooltip)
         self.refresh_button.setToolTip(QCoreApplication.translate("Form", u"Refresh package list view", None))
 #endif // QT_CONFIG(tooltip)
         self.refresh_button.setText("")
         self.package_filter_label.setText(QCoreApplication.translate("Form", u"Filter:", None))
         self.package_filter_edit.setPlaceholderText(QCoreApplication.translate("Form", u"*", None))
-        self.package_path_label.setText("")
+        self.package_path_label.setHtml(QCoreApplication.translate("Form", u"<!DOCTYPE HTML PUBLIC \"-//W3C//DTD HTML 4.0//EN\" \"http://www.w3.org/TR/REC-html40/strict.dtd\">\n"
+"<html><head><meta name=\"qrichtext\" content=\"1\" /><meta charset=\"utf-8\" /><style type=\"text/css\">\n"
+"p, li { white-space: pre-wrap; }\n"
+"hr { height: 1px; border-width: 0; }\n"
+"li.unchecked::marker { content: \"\\2610\"; }\n"
+"li.checked::marker { content: \"\\2612\"; }\n"
+"</style></head><body style=\" font-family:'Segoe UI'; font-size:9pt; font-weight:400; font-style:normal;\">\n"
+"<p style=\"-qt-paragraph-type:empty; margin-top:0px; margin-bottom:0px; margin-left:0px; margin-right:0px; -qt-block-indent:0; text-indent:0px;\"><br /></p></body></html>", None))
     # retranslateUi
```

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/plugins_manager/controller.py` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/plugins_manager/controller.py`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/plugins_manager/model.py` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/plugins_manager/model.py`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/plugins_manager/plugins.py` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/plugins_manager/plugins.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from typing import TYPE_CHECKING, Optional
 from conan_app_launcher import AUTHOR, BUILT_IN_PLUGIN, DEBUG_LEVEL, __version__
-from PySide6.QtCore import Qt
 from PySide6.QtWidgets import QWidget, QFileDialog, QMessageBox
 from conan_app_launcher.ui.plugin.plugins import PluginDescription, PluginHandler, ThemedWidget, PluginInterfaceV1
 from conan_app_launcher.ui.views.plugins_manager.model import PluginModelItem
 
 from .controller import PluginController
```

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/plugins_manager/plugins.ui` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/plugins_manager/plugins.ui`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/views/plugins_manager/plugins_ui.py` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/views/plugins_manager/plugins_ui.py`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/widgets/__init__.py` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/widgets/clickable_icon.py` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/widgets/clickable_icon.py`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/widgets/conan_line_edit.py` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/widgets/conan_line_edit.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from threading import Thread
 from typing import Callable, List
 
 import conan_app_launcher.app as app  # using global module pattern
 from conan_app_launcher.app.logger import Logger
-from conan_app_launcher.core.conan_common import ConanRef, PkgRef
+from conan_app_launcher.conan_wrapper.types import ConanRef, PkgRef
 from PySide6.QtCore import Qt, Signal
 from PySide6.QtWidgets import QCompleter, QLineEdit, QListView
 
 from conan_app_launcher.ui.common.theming import get_gui_dark_mode
 
 
 class ConanRefLineEdit(QLineEdit):
@@ -45,23 +45,26 @@
         if enabled:
             self.setStyleSheet(f"") # remove grey color
         else:
             self.setStyleSheet(f"color: grey;")
         super().setEnabled(enabled)
 
     def showEvent(self, event):
-        combined_refs = set()
-        combined_refs.update(app.conan_api.info_cache.get_all_local_refs())
-        combined_refs.update(app.conan_api.info_cache.get_all_remote_refs())
-        self.completer().model().setStringList(sorted(combined_refs))  # type: ignore
+        self.load_completion_refs()
         if self._first_show:
             self.completer().popup().hide()
             self._first_show = True
         super().showEvent(event)
 
+    def load_completion_refs(self):
+        combined_refs = set()
+        combined_refs.update(app.conan_api.info_cache.get_all_local_refs())
+        combined_refs.update(app.conan_api.info_cache.get_all_remote_refs())
+        self.completer().model().setStringList(sorted(combined_refs))  # type: ignore
+
     def cleanup(self):
         if self._completion_thread:
             self._completion_thread.join(1)
 
     def set_loading_callback(self, loading_cbk: Callable):
         self._loading_cbk = loading_cbk
```

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/widgets/password_line_edit.py` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/widgets/password_line_edit.py`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher/ui/widgets/toggle.py` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher/ui/widgets/toggle.py`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher.egg-info/PKG-INFO` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conan-app-launcher
-Version: 2.0.0b5
+Version: 2.0.0b6
 Summary: App Launcher and Package Explorer for Conan
 Home-page: https://github.com/goszpeti/conan_app_launcher
 Author: Péter Gosztolya and Contributors
 License: LGPL v3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -19,15 +19,15 @@
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE
 
 
-# <img src="https://raw.githubusercontent.com/goszpeti/conan_app_launcher/v2.0.0b5/src/conan_app_launcher/assets/icons/icon.ico" width="128">
+# <img src="https://raw.githubusercontent.com/goszpeti/conan_app_launcher/v2.0.0b6/src/conan_app_launcher/assets/icons/icon.ico" width="128">
 
 # Conan App Launcher and Local Package Explorer
 
 ![https://pypi.org/project/conan-app-launcher/](https://img.shields.io/pypi/v/conan-app-launcher)
 ![PyPI Python versions](https://img.shields.io/pypi/pyversions/conan-app-launcher)
 ![MilestoneProgress](https://img.shields.io/github/milestones/progress-percent/goszpeti/conan_app_launcher/17)
 ![Python tests](https://github.com/goszpeti/conan_app_launcher/workflows/Python%20tests/badge.svg)
@@ -41,24 +41,24 @@
 * Browse the local package cache
 * Search Packages in remotes
 * Configure Remotes and Profiles
 
 It is end-user oriented and focuses on using packages, rather then developing them. It can be used on Windows and Linux x64 platforms.
 
 #### Application Link Grid
-# <img src="https://raw.githubusercontent.com/goszpeti/conan_app_launcher/v2.0.0b5/doc/screenshot.png" width="512">
+# <img src="https://raw.githubusercontent.com/goszpeti/conan_app_launcher/v2.0.0b6/doc/screenshot.png" width="512">
 
 #### Local Package Manager
-# <img src="https://raw.githubusercontent.com/goszpeti/conan_app_launcher/v2.0.0b5/doc/screenshot_pkg_explorer.png" width="512">
+# <img src="https://raw.githubusercontent.com/goszpeti/conan_app_launcher/v2.0.0b6/doc/screenshot_pkg_explorer.png" width="512">
 
 #### Conan Search
-# <img src="https://raw.githubusercontent.com/goszpeti/conan_app_launcher/v2.0.0b5/doc/screenshot_conan_search.png" width="512">
+# <img src="https://raw.githubusercontent.com/goszpeti/conan_app_launcher/v2.0.0b6/doc/screenshot_conan_search.png" width="512">
 
 #### Conan Config
-# <img src="https://raw.githubusercontent.com/goszpeti/conan_app_launcher/v2.0.0b5/doc/screenshot_conan_conf.png" width="512">
+# <img src="https://raw.githubusercontent.com/goszpeti/conan_app_launcher/v2.0.0b6/doc/screenshot_conan_conf.png" width="512">
 
 **Main Features**
 - compatible with a wide range of conan versions (from 1.24 onwards)
 - integrated console for information an packages and config file
 - installable with pip
 
 Quicklaunch
```

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher.egg-info/SOURCES.txt` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,17 @@
 src/conan_app_launcher.egg-info/SOURCES.txt
 src/conan_app_launcher.egg-info/dependency_links.txt
 src/conan_app_launcher.egg-info/entry_points.txt
 src/conan_app_launcher.egg-info/requires.txt
 src/conan_app_launcher.egg-info/top_level.txt
 src/conan_app_launcher/app/__init__.py
 src/conan_app_launcher/app/crash.py
+src/conan_app_launcher/app/loading.py
 src/conan_app_launcher/app/logger.py
+src/conan_app_launcher/app/system.py
 src/conan_app_launcher/assets/config_schema.json
 src/conan_app_launcher/assets/launch.bat.in
 src/conan_app_launcher/assets/launch.sh.in
 src/conan_app_launcher/assets/font/NotoSans-Regular.ttf
 src/conan_app_launcher/assets/font/NotoSansMono.ttf
 src/conan_app_launcher/assets/icons/Readme.md
 src/conan_app_launcher/assets/icons/conan.png
@@ -143,35 +145,34 @@
 src/conan_app_launcher/assets/icons/material/restore.svg
 src/conan_app_launcher/assets/icons/material/save.svg
 src/conan_app_launcher/assets/icons/material/search.svg
 src/conan_app_launcher/assets/icons/material/search_packages.svg
 src/conan_app_launcher/assets/icons/material/settings.svg
 src/conan_app_launcher/assets/icons/material/show.svg
 src/conan_app_launcher/assets/icons/material/view.svg
-src/conan_app_launcher/core/__init__.py
-src/conan_app_launcher/core/conanV1.py
-src/conan_app_launcher/core/conanV2.py
-src/conan_app_launcher/core/conan_cache.py
-src/conan_app_launcher/core/conan_cleanup.py
-src/conan_app_launcher/core/conan_common.py
-src/conan_app_launcher/core/conan_worker.py
-src/conan_app_launcher/core/system.py
+src/conan_app_launcher/conan_wrapper/__init__.py
+src/conan_app_launcher/conan_wrapper/conanV1.py
+src/conan_app_launcher/conan_wrapper/conanV2.py
+src/conan_app_launcher/conan_wrapper/conan_cache.py
+src/conan_app_launcher/conan_wrapper/conan_cleanup.py
+src/conan_app_launcher/conan_wrapper/conan_worker.py
+src/conan_app_launcher/conan_wrapper/types.py
 src/conan_app_launcher/settings/__init__.py
 src/conan_app_launcher/settings/ini_file.py
 src/conan_app_launcher/ui/__init__.py
 src/conan_app_launcher/ui/dark_style.qss.in
 src/conan_app_launcher/ui/light_style.qss.in
 src/conan_app_launcher/ui/main_window.py
 src/conan_app_launcher/ui/model.py
 src/conan_app_launcher/ui/plugins.ini
 src/conan_app_launcher/ui/common/__init__.py
 src/conan_app_launcher/ui/common/icon.py
-src/conan_app_launcher/ui/common/loading.py
 src/conan_app_launcher/ui/common/logger.py
 src/conan_app_launcher/ui/common/model.py
+src/conan_app_launcher/ui/common/syntax_highlighting.py
 src/conan_app_launcher/ui/common/theming.py
 src/conan_app_launcher/ui/config/__init__.py
 src/conan_app_launcher/ui/config/json_file.py
 src/conan_app_launcher/ui/dialogs/__init__.py
 src/conan_app_launcher/ui/dialogs/conan_remove.py
 src/conan_app_launcher/ui/dialogs/conan_install/__init__.py
 src/conan_app_launcher/ui/dialogs/conan_install/conan_install.py
@@ -216,14 +217,15 @@
 src/conan_app_launcher/ui/views/app_grid/dialogs/app_edit_dialog_ui.py
 src/conan_app_launcher/ui/views/conan_conf/__init__.py
 src/conan_app_launcher/ui/views/conan_conf/conan_conf.py
 src/conan_app_launcher/ui/views/conan_conf/conan_conf.ui
 src/conan_app_launcher/ui/views/conan_conf/conan_conf_ui.py
 src/conan_app_launcher/ui/views/conan_conf/controller.py
 src/conan_app_launcher/ui/views/conan_conf/model.py
+src/conan_app_launcher/ui/views/conan_conf/ui_conan_conf.py
 src/conan_app_launcher/ui/views/conan_conf/dialogs/__init__.py
 src/conan_app_launcher/ui/views/conan_conf/dialogs/remote_edit_dialog.py
 src/conan_app_launcher/ui/views/conan_conf/dialogs/remote_edit_dialog.ui
 src/conan_app_launcher/ui/views/conan_conf/dialogs/remote_edit_dialog_ui.py
 src/conan_app_launcher/ui/views/conan_conf/dialogs/remote_login_dialog.py
 src/conan_app_launcher/ui/views/conan_conf/dialogs/remote_login_dialog.ui
 src/conan_app_launcher/ui/views/conan_conf/dialogs/remote_login_dialog_ui.py
```

### Comparing `conan-app-launcher-2.0.0b5/src/conan_app_launcher.egg-info/requires.txt` & `conan-app-launcher-2.0.0b6/src/conan_app_launcher.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `conan-app-launcher-2.0.0b5/test/testdata/settings/read/config.ini` & `conan-app-launcher-2.0.0b6/test/testdata/settings/read/config.ini`

 * *Files identical despite different names*

