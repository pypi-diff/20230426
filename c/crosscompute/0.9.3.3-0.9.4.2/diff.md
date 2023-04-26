# Comparing `tmp/crosscompute-0.9.3.3.tar.gz` & `tmp/crosscompute-0.9.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crosscompute-0.9.3.3.tar", last modified: Sat Feb 25 13:03:27 2023, max compression
+gzip compressed data, was "crosscompute-0.9.4.2.tar", last modified: Wed Apr 26 00:25:44 2023, max compression
```

## Comparing `crosscompute-0.9.3.3.tar` & `crosscompute-0.9.4.2.tar`

### file list

```diff
@@ -1,101 +1,113 @@
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-02-25 13:03:27.946950 crosscompute-0.9.3.3/
--rw-rw-r--   0 rhh       (1000) rhh       (1000)     1057 2022-08-15 04:38:47.000000 crosscompute-0.9.3.3/LICENSE.md
--rw-r--r--   0 rhh       (1000) rhh       (1000)     4974 2023-02-25 13:03:27.947950 crosscompute-0.9.3.3/PKG-INFO
--rw-r--r--   0 rhh       (1000) rhh       (1000)     3690 2023-02-18 06:45:43.000000 crosscompute-0.9.3.3/README.md
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-02-25 13:03:27.931949 crosscompute-0.9.3.3/crosscompute/
--rw-r--r--   0 rhh       (1000) rhh       (1000)       22 2023-02-18 06:45:42.000000 crosscompute-0.9.3.3/crosscompute/__init__.py
--rw-rw-r--   0 rhh       (1000) rhh       (1000)       38 2022-08-15 04:38:47.000000 crosscompute-0.9.3.3/crosscompute/__main__.py
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-02-25 13:03:27.940950 crosscompute-0.9.3.3/crosscompute/assets/
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1082 2023-02-18 06:45:42.000000 crosscompute-0.9.3.3/crosscompute/assets/automation.html
--rw-r--r--   0 rhh       (1000) rhh       (1000)      986 2023-02-18 06:45:42.000000 crosscompute-0.9.3.3/crosscompute/assets/base.html
--rw-r--r--   0 rhh       (1000) rhh       (1000)      628 2023-02-18 06:45:42.000000 crosscompute-0.9.3.3/crosscompute/assets/checkbox-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      579 2023-02-18 06:45:42.000000 crosscompute-0.9.3.3/crosscompute/assets/checkbox-input.html
--rw-r--r--   0 rhh       (1000) rhh       (1000)      183 2023-02-18 06:45:42.000000 crosscompute-0.9.3.3/crosscompute/assets/checkbox-input.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      109 2023-02-18 06:45:42.000000 crosscompute-0.9.3.3/crosscompute/assets/checkbox-output.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)     8932 2023-02-24 12:23:07.000000 crosscompute-0.9.3.3/crosscompute/assets/configuration.yml
--rw-r--r--   0 rhh       (1000) rhh       (1000)       85 2023-02-18 06:45:42.000000 crosscompute-0.9.3.3/crosscompute/assets/default.css
--rw-r--r--   0 rhh       (1000) rhh       (1000)       22 2023-02-18 06:45:42.000000 crosscompute-0.9.3.3/crosscompute/assets/embedded.css
--rw-r--r--   0 rhh       (1000) rhh       (1000)    22382 2023-02-18 06:45:42.000000 crosscompute-0.9.3.3/crosscompute/assets/favicon.ico
--rw-r--r--   0 rhh       (1000) rhh       (1000)      234 2023-02-18 06:45:42.000000 crosscompute-0.9.3.3/crosscompute/assets/flex-vertical.css
--rw-r--r--   0 rhh       (1000) rhh       (1000)      180 2023-02-18 06:45:42.000000 crosscompute-0.9.3.3/crosscompute/assets/frame-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      106 2023-02-18 06:45:42.000000 crosscompute-0.9.3.3/crosscompute/assets/frame-output.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      138 2023-02-18 06:45:42.000000 crosscompute-0.9.3.3/crosscompute/assets/image-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      106 2023-02-18 06:45:42.000000 crosscompute-0.9.3.3/crosscompute/assets/image-output.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      156 2023-02-18 06:45:42.000000 crosscompute-0.9.3.3/crosscompute/assets/json-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      139 2023-02-24 12:23:07.000000 crosscompute-0.9.3.3/crosscompute/assets/json-output.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      149 2023-02-18 06:45:42.000000 crosscompute-0.9.3.3/crosscompute/assets/link-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      106 2023-02-18 06:45:42.000000 crosscompute-0.9.3.3/crosscompute/assets/link-output.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)     2553 2023-02-18 06:45:43.000000 crosscompute-0.9.3.3/crosscompute/assets/live.html
--rw-r--r--   0 rhh       (1000) rhh       (1000)      301 2023-02-18 06:45:42.000000 crosscompute-0.9.3.3/crosscompute/assets/markdown-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      142 2023-02-18 06:45:42.000000 crosscompute-0.9.3.3/crosscompute/assets/markdown-output.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      594 2023-02-18 06:45:42.000000 crosscompute-0.9.3.3/crosscompute/assets/radio-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      575 2023-02-18 06:45:42.000000 crosscompute-0.9.3.3/crosscompute/assets/radio-input.html
--rw-r--r--   0 rhh       (1000) rhh       (1000)       96 2023-02-18 06:45:42.000000 crosscompute-0.9.3.3/crosscompute/assets/radio-input.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      106 2023-02-18 06:45:42.000000 crosscompute-0.9.3.3/crosscompute/assets/radio-output.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      285 2023-02-18 06:45:42.000000 crosscompute-0.9.3.3/crosscompute/assets/root.html
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1167 2023-02-18 06:45:42.000000 crosscompute-0.9.3.3/crosscompute/assets/step-body.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      134 2023-02-18 06:45:42.000000 crosscompute-0.9.3.3/crosscompute/assets/step-main.html
--rw-r--r--   0 rhh       (1000) rhh       (1000)      479 2023-02-18 06:45:42.000000 crosscompute-0.9.3.3/crosscompute/assets/step.html
--rw-r--r--   0 rhh       (1000) rhh       (1000)      369 2023-02-18 06:45:42.000000 crosscompute-0.9.3.3/crosscompute/assets/string-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      432 2023-02-18 06:45:42.000000 crosscompute-0.9.3.3/crosscompute/assets/string-input.html
--rw-r--r--   0 rhh       (1000) rhh       (1000)       65 2023-02-18 06:45:42.000000 crosscompute-0.9.3.3/crosscompute/assets/string-input.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      122 2023-02-18 06:45:42.000000 crosscompute-0.9.3.3/crosscompute/assets/string-output.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1095 2023-02-18 06:45:42.000000 crosscompute-0.9.3.3/crosscompute/assets/table-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      139 2023-02-18 06:45:42.000000 crosscompute-0.9.3.3/crosscompute/assets/table-output.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      109 2023-02-18 06:45:42.000000 crosscompute-0.9.3.3/crosscompute/assets/text-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      159 2023-02-18 06:45:42.000000 crosscompute-0.9.3.3/crosscompute/assets/text-input.html
--rw-r--r--   0 rhh       (1000) rhh       (1000)      136 2023-02-18 06:45:42.000000 crosscompute-0.9.3.3/crosscompute/assets/text-input.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      138 2023-02-18 06:45:42.000000 crosscompute-0.9.3.3/crosscompute/assets/text-output.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)     2521 2023-02-25 12:30:17.000000 crosscompute-0.9.3.3/crosscompute/constants.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     5072 2023-02-18 06:45:42.000000 crosscompute-0.9.3.3/crosscompute/dependencies.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1055 2023-02-18 06:45:42.000000 crosscompute-0.9.3.3/crosscompute/exceptions.py
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-02-25 13:03:27.941950 crosscompute-0.9.3.3/crosscompute/macros/
--rw-rw-r--   0 rhh       (1000) rhh       (1000)        0 2022-08-15 04:38:47.000000 crosscompute-0.9.3.3/crosscompute/macros/__init__.py
--rw-rw-r--   0 rhh       (1000) rhh       (1000)      717 2022-08-15 04:38:47.000000 crosscompute-0.9.3.3/crosscompute/macros/disk.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1530 2023-02-18 06:45:42.000000 crosscompute-0.9.3.3/crosscompute/macros/iterable.py
--rw-rw-r--   0 rhh       (1000) rhh       (1000)      597 2022-08-15 04:38:47.000000 crosscompute-0.9.3.3/crosscompute/macros/package.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1349 2023-02-18 06:45:42.000000 crosscompute-0.9.3.3/crosscompute/macros/security.py
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-02-25 13:03:27.942950 crosscompute-0.9.3.3/crosscompute/routers/
--rw-r--r--   0 rhh       (1000) rhh       (1000)        0 2023-02-18 06:45:42.000000 crosscompute-0.9.3.3/crosscompute/routers/__init__.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     7009 2023-02-18 06:45:42.000000 crosscompute-0.9.3.3/crosscompute/routers/automation.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1626 2023-02-18 06:45:42.000000 crosscompute-0.9.3.3/crosscompute/routers/mutation.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     3291 2023-02-18 06:45:42.000000 crosscompute-0.9.3.3/crosscompute/routers/root.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)      523 2023-02-18 06:45:42.000000 crosscompute-0.9.3.3/crosscompute/routers/token.py
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-02-25 13:03:27.944950 crosscompute-0.9.3.3/crosscompute/routines/
--rw-rw-r--   0 rhh       (1000) rhh       (1000)        0 2022-08-15 04:38:47.000000 crosscompute-0.9.3.3/crosscompute/routines/__init__.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)      591 2023-02-18 06:45:42.000000 crosscompute-0.9.3.3/crosscompute/routines/asset.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     3457 2023-02-18 06:45:42.000000 crosscompute-0.9.3.3/crosscompute/routines/authorization.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)    27739 2023-02-18 06:45:42.000000 crosscompute-0.9.3.3/crosscompute/routines/automation.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     3537 2023-02-18 06:45:42.000000 crosscompute-0.9.3.3/crosscompute/routines/batch.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)    42939 2023-02-18 06:45:42.000000 crosscompute-0.9.3.3/crosscompute/routines/configuration.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     6436 2023-02-18 06:45:42.000000 crosscompute-0.9.3.3/crosscompute/routines/database.py
--rw-rw-r--   0 rhh       (1000) rhh       (1000)      914 2022-08-15 04:38:47.000000 crosscompute-0.9.3.3/crosscompute/routines/interface.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1404 2023-02-18 06:45:42.000000 crosscompute-0.9.3.3/crosscompute/routines/log.py
--rw-rw-r--   0 rhh       (1000) rhh       (1000)      545 2022-08-15 04:38:47.000000 crosscompute-0.9.3.3/crosscompute/routines/printer.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     6468 2023-02-18 06:45:42.000000 crosscompute-0.9.3.3/crosscompute/routines/server.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     5494 2023-02-25 13:03:12.000000 crosscompute-0.9.3.3/crosscompute/routines/step.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)    29494 2023-02-18 06:45:42.000000 crosscompute-0.9.3.3/crosscompute/routines/variable.py
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-02-25 13:03:27.945950 crosscompute-0.9.3.3/crosscompute/scripts/
--rw-rw-r--   0 rhh       (1000) rhh       (1000)        0 2022-08-15 04:38:47.000000 crosscompute-0.9.3.3/crosscompute/scripts/__init__.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     3896 2023-02-18 06:45:42.000000 crosscompute-0.9.3.3/crosscompute/scripts/configure.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     3799 2023-02-18 06:45:42.000000 crosscompute-0.9.3.3/crosscompute/scripts/launch.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     5504 2023-02-18 06:45:42.000000 crosscompute-0.9.3.3/crosscompute/scripts/print.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1708 2023-02-18 06:45:42.000000 crosscompute-0.9.3.3/crosscompute/scripts/run.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     4868 2023-02-18 06:45:42.000000 crosscompute-0.9.3.3/crosscompute/scripts/serve.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1531 2023-02-18 06:45:42.000000 crosscompute-0.9.3.3/crosscompute/settings.py
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-02-25 13:03:27.932949 crosscompute-0.9.3.3/crosscompute.egg-info/
--rw-r--r--   0 rhh       (1000) rhh       (1000)     4974 2023-02-25 13:03:27.000000 crosscompute-0.9.3.3/crosscompute.egg-info/PKG-INFO
--rw-r--r--   0 rhh       (1000) rhh       (1000)     2965 2023-02-25 13:03:27.000000 crosscompute-0.9.3.3/crosscompute.egg-info/SOURCES.txt
--rw-r--r--   0 rhh       (1000) rhh       (1000)        1 2023-02-25 13:03:27.000000 crosscompute-0.9.3.3/crosscompute.egg-info/dependency_links.txt
--rw-r--r--   0 rhh       (1000) rhh       (1000)      739 2023-02-25 13:03:27.000000 crosscompute-0.9.3.3/crosscompute.egg-info/entry_points.txt
--rw-r--r--   0 rhh       (1000) rhh       (1000)      398 2023-02-25 13:03:27.000000 crosscompute-0.9.3.3/crosscompute.egg-info/requires.txt
--rw-r--r--   0 rhh       (1000) rhh       (1000)       13 2023-02-25 13:03:27.000000 crosscompute-0.9.3.3/crosscompute.egg-info/top_level.txt
--rw-r--r--   0 rhh       (1000) rhh       (1000)        1 2022-08-22 13:00:05.000000 crosscompute-0.9.3.3/crosscompute.egg-info/zip-safe
--rw-r--r--   0 rhh       (1000) rhh       (1000)     3137 2023-02-25 13:03:27.948950 crosscompute-0.9.3.3/setup.cfg
--rw-rw-r--   0 rhh       (1000) rhh       (1000)       39 2022-08-15 04:38:47.000000 crosscompute-0.9.3.3/setup.py
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-02-25 13:03:27.946950 crosscompute-0.9.3.3/tests/
--rw-rw-r--   0 rhh       (1000) rhh       (1000)      168 2022-08-15 04:38:47.000000 crosscompute-0.9.3.3/tests/test_macros_iterable.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)      428 2023-02-18 06:45:42.000000 crosscompute-0.9.3.3/tests/test_macros_security.py
--rw-rw-r--   0 rhh       (1000) rhh       (1000)      655 2022-08-15 04:38:47.000000 crosscompute-0.9.3.3/tests/test_routines_automation.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     3914 2023-02-18 06:45:42.000000 crosscompute-0.9.3.3/tests/test_routines_configuration.py
--rw-rw-r--   0 rhh       (1000) rhh       (1000)     2285 2022-08-15 04:38:47.000000 crosscompute-0.9.3.3/tests/test_routines_variable.py
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-04-26 00:25:44.837256 crosscompute-0.9.4.2/
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1057 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/LICENSE.md
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     4987 2023-04-26 00:25:44.837256 crosscompute-0.9.4.2/PKG-INFO
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     3703 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/README.md
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-04-26 00:25:44.820255 crosscompute-0.9.4.2/crosscompute/
+-rw-r--r--   0 rhh       (1000) rhh       (1000)       22 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/__init__.py
+-rw-rw-r--   0 rhh       (1000) rhh       (1000)       38 2022-08-15 04:38:47.000000 crosscompute-0.9.4.2/crosscompute/__main__.py
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-04-26 00:25:44.830255 crosscompute-0.9.4.2/crosscompute/assets/
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1286 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/assets/automation.html
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      910 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/assets/base.html
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      230 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/assets/button-panel.html
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      183 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/assets/checkbox-input-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      579 2023-02-18 06:45:42.000000 crosscompute-0.9.4.2/crosscompute/assets/checkbox-input.html
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      628 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/assets/checkbox-output-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      109 2023-02-18 06:45:42.000000 crosscompute-0.9.4.2/crosscompute/assets/checkbox-output.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)    13294 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/assets/configuration.yml
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      224 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/assets/default.css
+-rw-r--r--   0 rhh       (1000) rhh       (1000)       48 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/assets/embedded.css
+-rw-r--r--   0 rhh       (1000) rhh       (1000)    22382 2023-02-18 06:45:42.000000 crosscompute-0.9.4.2/crosscompute/assets/favicon.ico
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      765 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/assets/file-input-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      165 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/assets/file-input.html
+-rw-r--r--   0 rhh       (1000) rhh       (1000)        0 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/assets/file-input.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      578 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/assets/flex.css
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      180 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/assets/frame-output-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      106 2023-02-18 06:45:42.000000 crosscompute-0.9.4.2/crosscompute/assets/frame-output.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      138 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/assets/image-output-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      106 2023-02-18 06:45:42.000000 crosscompute-0.9.4.2/crosscompute/assets/image-output.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      156 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/assets/json-output-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      139 2023-04-25 22:48:18.000000 crosscompute-0.9.4.2/crosscompute/assets/json-output.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      149 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/assets/link-output-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      106 2023-02-18 06:45:42.000000 crosscompute-0.9.4.2/crosscompute/assets/link-output.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     2566 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/assets/live.html
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      301 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/assets/markdown-output-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      142 2023-02-18 06:45:42.000000 crosscompute-0.9.4.2/crosscompute/assets/markdown-output.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      136 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/assets/pdf-output-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      137 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/assets/pdf-output.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)       64 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/assets/pdf.css
+-rw-r--r--   0 rhh       (1000) rhh       (1000)       53 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/assets/printed.css
+-rw-r--r--   0 rhh       (1000) rhh       (1000)       96 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/assets/radio-input-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      575 2023-02-18 06:45:42.000000 crosscompute-0.9.4.2/crosscompute/assets/radio-input.html
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      594 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/assets/radio-output-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      106 2023-02-18 06:45:42.000000 crosscompute-0.9.4.2/crosscompute/assets/radio-output.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      285 2023-02-18 06:45:42.000000 crosscompute-0.9.4.2/crosscompute/assets/root.html
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     3271 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/assets/step-body.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      874 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/assets/step.html
+-rw-r--r--   0 rhh       (1000) rhh       (1000)       65 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/assets/string-input-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      432 2023-02-18 06:45:42.000000 crosscompute-0.9.4.2/crosscompute/assets/string-input.html
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      369 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/assets/string-output-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      122 2023-02-18 06:45:42.000000 crosscompute-0.9.4.2/crosscompute/assets/string-output.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1095 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/assets/table-output-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      139 2023-02-18 06:45:42.000000 crosscompute-0.9.4.2/crosscompute/assets/table-output.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      159 2023-02-18 06:45:42.000000 crosscompute-0.9.4.2/crosscompute/assets/text-input.html
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      136 2023-02-18 06:45:42.000000 crosscompute-0.9.4.2/crosscompute/assets/text-input.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      109 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/assets/text-output-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      138 2023-02-18 06:45:42.000000 crosscompute-0.9.4.2/crosscompute/assets/text-output.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     2886 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/constants.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     5072 2023-04-01 20:58:16.000000 crosscompute-0.9.4.2/crosscompute/dependencies.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1055 2023-02-18 06:45:42.000000 crosscompute-0.9.4.2/crosscompute/exceptions.py
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-04-26 00:25:44.831256 crosscompute-0.9.4.2/crosscompute/macros/
+-rw-rw-r--   0 rhh       (1000) rhh       (1000)        0 2022-08-15 04:38:47.000000 crosscompute-0.9.4.2/crosscompute/macros/__init__.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      717 2023-04-05 23:51:33.000000 crosscompute-0.9.4.2/crosscompute/macros/disk.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1530 2023-02-18 06:45:42.000000 crosscompute-0.9.4.2/crosscompute/macros/iterable.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1088 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/macros/log.py
+-rw-rw-r--   0 rhh       (1000) rhh       (1000)      597 2022-08-15 04:38:47.000000 crosscompute-0.9.4.2/crosscompute/macros/package.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1349 2023-02-18 06:45:42.000000 crosscompute-0.9.4.2/crosscompute/macros/security.py
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-04-26 00:25:44.832255 crosscompute-0.9.4.2/crosscompute/routers/
+-rw-r--r--   0 rhh       (1000) rhh       (1000)        0 2023-02-18 06:45:42.000000 crosscompute-0.9.4.2/crosscompute/routers/__init__.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     7020 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/routers/automation.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1142 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/routers/file.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     3286 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/routers/root.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1240 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/routers/stream.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      523 2023-02-18 06:45:42.000000 crosscompute-0.9.4.2/crosscompute/routers/token.py
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-04-26 00:25:44.835255 crosscompute-0.9.4.2/crosscompute/routines/
+-rw-rw-r--   0 rhh       (1000) rhh       (1000)        0 2022-08-15 04:38:47.000000 crosscompute-0.9.4.2/crosscompute/routines/__init__.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     3195 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/routines/asset.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     3457 2023-02-18 06:45:42.000000 crosscompute-0.9.4.2/crosscompute/routines/authorization.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     4877 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/routines/automation.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     3537 2023-02-18 06:45:42.000000 crosscompute-0.9.4.2/crosscompute/routines/batch.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)    42043 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/routines/configuration.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     9315 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/routines/database.py
+-rw-rw-r--   0 rhh       (1000) rhh       (1000)      914 2022-08-15 04:38:47.000000 crosscompute-0.9.4.2/crosscompute/routines/interface.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1404 2023-02-18 06:45:42.000000 crosscompute-0.9.4.2/crosscompute/routines/log.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1523 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/routines/mutation.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     6222 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/routines/printer.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     6967 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/routines/server.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     7181 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/routines/step.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      605 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/routines/uri.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)    30285 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/routines/variable.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)    28255 2023-04-26 00:24:10.000000 crosscompute-0.9.4.2/crosscompute/routines/work.py
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-04-26 00:25:44.836256 crosscompute-0.9.4.2/crosscompute/scripts/
+-rw-rw-r--   0 rhh       (1000) rhh       (1000)        0 2022-08-15 04:38:47.000000 crosscompute-0.9.4.2/crosscompute/scripts/__init__.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     3866 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/scripts/configure.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     3829 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/scripts/launch.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1123 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/scripts/print.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1721 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/scripts/run.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     4065 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/scripts/serve.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1338 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/settings.py
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-04-26 00:25:44.821255 crosscompute-0.9.4.2/crosscompute.egg-info/
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     4987 2023-04-26 00:25:44.000000 crosscompute-0.9.4.2/crosscompute.egg-info/PKG-INFO
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     3437 2023-04-26 00:25:44.000000 crosscompute-0.9.4.2/crosscompute.egg-info/SOURCES.txt
+-rw-r--r--   0 rhh       (1000) rhh       (1000)        1 2023-04-26 00:25:44.000000 crosscompute-0.9.4.2/crosscompute.egg-info/dependency_links.txt
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      831 2023-04-26 00:25:44.000000 crosscompute-0.9.4.2/crosscompute.egg-info/entry_points.txt
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      436 2023-04-26 00:25:44.000000 crosscompute-0.9.4.2/crosscompute.egg-info/requires.txt
+-rw-r--r--   0 rhh       (1000) rhh       (1000)       13 2023-04-26 00:25:44.000000 crosscompute-0.9.4.2/crosscompute.egg-info/top_level.txt
+-rw-r--r--   0 rhh       (1000) rhh       (1000)        1 2022-08-22 13:00:05.000000 crosscompute-0.9.4.2/crosscompute.egg-info/zip-safe
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     3273 2023-04-26 00:25:44.839256 crosscompute-0.9.4.2/setup.cfg
+-rw-rw-r--   0 rhh       (1000) rhh       (1000)       39 2022-08-15 04:38:47.000000 crosscompute-0.9.4.2/setup.py
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-04-26 00:25:44.837256 crosscompute-0.9.4.2/tests/
+-rw-rw-r--   0 rhh       (1000) rhh       (1000)      168 2022-08-15 04:38:47.000000 crosscompute-0.9.4.2/tests/test_macros_iterable.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      428 2023-02-18 06:45:42.000000 crosscompute-0.9.4.2/tests/test_macros_security.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     3759 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/tests/test_routines_configuration.py
+-rw-rw-r--   0 rhh       (1000) rhh       (1000)     2285 2022-08-15 04:38:47.000000 crosscompute-0.9.4.2/tests/test_routines_variable.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      656 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/tests/test_routines_work.py
```

### Comparing `crosscompute-0.9.3.3/LICENSE.md` & `crosscompute-0.9.4.2/LICENSE.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-Copyright 2022 CrossCompute Inc.
+Copyright 2023 CrossCompute Inc.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `crosscompute-0.9.3.3/PKG-INFO` & `crosscompute-0.9.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crosscompute
-Version: 0.9.3.3
+Version: 0.9.4.2
 Summary: Automate your Jupyter notebooks and scripts as tools, reports, dashboards.
 Home-page: https://crosscompute.com
 Author: CrossCompute Inc.
 Author-email: support@crosscompute.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/crosscompute/crosscompute/issues
 Project-URL: Documentation, https://github.com/crosscompute/crosscompute-docs
@@ -56,26 +56,28 @@
 - markdown
 - image
 - radio
 - checkbox
 - table
 - frame
 - json
+- pdf
+- file
 - map-mapbox (crosscompute-views-map)
 - map-mapbox-location (crosscompute-views-map)
 - map-deck-screengrid (crosscompute-views-map)
 - barcode (crosscompute-views-barcode)
 
 [Here are the currently supported configuration options](https://github.com/crosscompute/crosscompute/blob/develop/crosscompute/templates/configuration.yaml).
 
 ## Usage
 
 ```bash
 # Upgrade package
-pip install crosscompute>=0.9.3 --upgrade
+pip install crosscompute>=0.9.4 --upgrade
 
 # Initialize configuration
 crosscompute
 
 # Serve automation
 crosscompute automate.yml
 ```
@@ -126,15 +128,15 @@
 ```
 sudo dnf -y install python3.10
 # sudo apt -y install python3.10
 
 python3.10 -m venv ~/.virtualenvs/crosscompute
 source ~/.virtualenvs/crosscompute/bin/activate
 
-pip install crosscompute>=0.9.3
+pip install crosscompute>=0.9.4
 ```
 
 ## Acknowledgments
 
 - [Olga Ryabtseva](https://www.linkedin.com/in/olga-creutzburg)
 - [Salah Ahmed](https://www.linkedin.com/in/salahspage)
 - [Rodrigo Guarachi](https://www.linkedin.com/in/rmguarachi)
```

### Comparing `crosscompute-0.9.3.3/README.md` & `crosscompute-0.9.4.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -26,26 +26,28 @@
 - markdown
 - image
 - radio
 - checkbox
 - table
 - frame
 - json
+- pdf
+- file
 - map-mapbox (crosscompute-views-map)
 - map-mapbox-location (crosscompute-views-map)
 - map-deck-screengrid (crosscompute-views-map)
 - barcode (crosscompute-views-barcode)
 
 [Here are the currently supported configuration options](https://github.com/crosscompute/crosscompute/blob/develop/crosscompute/templates/configuration.yaml).
 
 ## Usage
 
 ```bash
 # Upgrade package
-pip install crosscompute>=0.9.3 --upgrade
+pip install crosscompute>=0.9.4 --upgrade
 
 # Initialize configuration
 crosscompute
 
 # Serve automation
 crosscompute automate.yml
 ```
@@ -96,15 +98,15 @@
 ```
 sudo dnf -y install python3.10
 # sudo apt -y install python3.10
 
 python3.10 -m venv ~/.virtualenvs/crosscompute
 source ~/.virtualenvs/crosscompute/bin/activate
 
-pip install crosscompute>=0.9.3
+pip install crosscompute>=0.9.4
 ```
 
 ## Acknowledgments
 
 - [Olga Ryabtseva](https://www.linkedin.com/in/olga-creutzburg)
 - [Salah Ahmed](https://www.linkedin.com/in/salahspage)
 - [Rodrigo Guarachi](https://www.linkedin.com/in/rmguarachi)
```

### Comparing `crosscompute-0.9.3.3/crosscompute/assets/automation.html` & `crosscompute-0.9.4.2/crosscompute/assets/automation.html`

 * *Files 24% similar despite different names*

```diff
@@ -14,27 +14,33 @@
 <a href="{{ root_uri or '/' }}">Root</a> &gt;
 <a href="{{ root_uri }}{{ uri }}">{{ name }}</a>
 {% endif %}
 {% endblock %}
 
 {% block main_html %}
 {% if step_name != 'none' %}
-{{ super() }}
-{% include 'step-main.html' %}
+{{ super() -}}
 {% endif %}
+{% endblock %}
+
+{% block footer_html %}
 {% if not for_embed %}
 <ul class="_batches">
-{% for batch in batches %}
+{% for batch_definition in batch_definitions %}
+{% set absolute_batch_uri = root_uri + uri + batch_definition.uri %}
 <li>
-{{ batch['name'] }}
-<a href="{{ root_uri }}{{ uri }}{{ batch['uri'] }}/i">[input]</a>
-<a href="{{ root_uri }}{{ uri }}{{ batch['uri'] }}/o">[output]</a>
+{{ batch_definition.name }}
+<a href="{{ absolute_batch_uri }}/i">input</a>
+<a href="{{ absolute_batch_uri }}/o">output</a>
+{% if automation_definition.variable_definitions_by_step_name['print'] %}
+<a href="{{ absolute_batch_uri }}/p">print</a>
+{% endif %}
 </li>
 {% endfor %}
 </ul>
 {% endif %}
 {% endblock %}
 
 {% block body_js %}
 {% include 'step-body.js' %}
-{{ super() }}
+{{ super() -}}
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,14 +1,17 @@
 {% extends live_template_path %} {% block head_html %} {{ super() -}}
 
 
 
 
  {% endblock %} {% block header_html %} {% if not for_embed %} Root > {{_name
 }} {% endif %} {% endblock %} {% block main_html %} {% if step_name != 'none'
-%} {{ super() }} {% include 'step-main.html' %} {% endif %} {% if not for_embed
-%}
-    * {% for batch in batches %}
-    * {{ batch['name'] }} [input] [output]
+%} {{ super() -}} {% endif %} {% endblock %} {% block footer_html %} {% if not
+for_embed %}
+    * {% for batch_definition in batch_definitions %} {% set absolute_batch_uri
+      = root_uri + uri + batch_definition.uri %}
+    * {{ batch_definition.name }} input output {% if
+      automation_definition.variable_definitions_by_step_name['print'] %} print
+      {% endif %}
     * {% endfor %}
 {% endif %} {% endblock %} {% block body_js %} {% include 'step-body.js' %} {
-{ super() }} {% endblock %}
+{ super() -}} {% endblock %}
```

### Comparing `crosscompute-0.9.3.3/crosscompute/assets/checkbox-header.js` & `crosscompute-0.9.4.2/crosscompute/assets/checkbox-output-header.js`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.3.3/crosscompute/assets/checkbox-input.html` & `crosscompute-0.9.4.2/crosscompute/assets/checkbox-input.html`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.3.3/crosscompute/assets/favicon.ico` & `crosscompute-0.9.4.2/crosscompute/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.3.3/crosscompute/assets/live.html` & `crosscompute-0.9.4.2/crosscompute/assets/live.html`

 * *Files 27% similar despite different names*

```diff
@@ -1,99 +1,97 @@
 {% extends base_template_path %}
 
 {% block head_html %}
 {{ super() -}}
 <script>
-const variables = {}, callbacks = {}, isSecure = location.protocol == 'https:', getTime = () => (new Date).getTime(), sleep = t => new Promise(r => setTimeout(r, t));
+const getTime = () => (new Date).getTime(), sleep = t => new Promise(r => setTimeout(r, t)), rootUri = '{{ root_uri }}', variables = {}, callbacks = {}, isSecure = location.protocol == 'https:';
 function register(xs, k, v) {
   const ys = xs[k];
   if (ys === undefined) {
     xs[k] = [v];
   } else {
     ys.push(v);
   }
 }
 function registerCallback(variableId, f) {
   register(callbacks, variableId, f);
 }
 </script>
-{%- endblock %}
+{% endblock %}
 
 {% block body_js %}
 {% if step_name != 'input' %}
-async function runEach(xs) {
-  await Promise.all((xs || []).map(_ => _()));
-}
 async function refreshVariable(variableId) {
   await runEach(functions[variableId]);
   await runEach(callbacks[variableId]);
-{% if not with_restart %}
+{% if not with_restart and not has_interval %}
   if (variableId == 'return_code') {
-    isDone = 1;
+    mutationStream.close();
   }
 {% endif %}
 }
+async function runEach(xs) {
+  await Promise.all((xs || []).map(_ => _()));
+}
 {% endif %}
 {{ super() -}}
 {% if with_restart or is_done == 0 %}
-async function processMutations() {
-  const uri = '{{ root_uri }}{{ mutation_uri }}';
-  try {
-    const r = await fetch(`${uri}?t=${mutationTimestamp}`), d = await r.json(), { styles: ss, variables: vs } = d;
-{% if with_restart %}
-    if (
-      d.server_timestamp != {{ server_timestamp }} ||
-      d.configurations.length ||
-      d.templates.length
-    ) {
-      refreshPage();
-    } else if (ss.length) {
-      refreshStyle();
-    }
-{% endif %}
-{% if step_name != 'input' %}
-    await Promise.all(vs.map(_ => refreshVariable(_.id)));
-{% endif %}
-    mutationTimestamp = d.mutation_timestamp;
-    pingInterval = {{ minimum_ping_interval_in_milliseconds }};
-  } catch (e) {
-    if (pingInterval < {{ maximum_ping_interval_in_milliseconds }}) {
-      pingInterval *= 1.1;
-    }
-    console.error(e);
-  }
-  schedulePolling();
-}
 {% if with_restart %}
 async function refreshPage() {
-  const r = await fetch(location.href, { method: 'head' });
-  if (r.ok) {
-    location.reload();
-  } else {
-    location.href = '{{ root_uri or '/' }}';
+  const { status } = await fetch(location.href, { method: 'head' });
+  switch (status) {
+    case 200:
+      location.reload();
+      break;
+    case 404:
+      location.href = '{{ root_uri or '/' }}';
+      break;
+    default:
+      setTimeout(refreshPage, 1000);
   }
 }
 function refreshStyle() {
   const { origin } = location;
   for (var l of document.getElementsByTagName('link')) {
     if (l.rel !== 'stylesheet' || new URL(l.href).origin !== origin) {
       continue;
     }
     l.href += '?' + Date.now();
   }
 }
 {% endif %}
-function schedulePolling() {
-{% if not with_restart %}
-  if (isDone) {
-    return;
-  }
+function setupMutationStream() {
+  mutationStream = new EventSource(rootUri + '/streams{{ mutation_uri }}?t=' + mutationTime);
+  mutationStream.onopen = () => {
+    retrySeconds = 1;
+  };
+  mutationStream.onerror = () => {
+    mutationStream.close();
+    clearTimeout(mutationTimeout);
+    mutationTimeout = setTimeout(setupMutationStream, retrySeconds);
+    if (retrySeconds < 60) {
+      retrySeconds *= 2;
+    }
+  };
+  mutationStream.onmessage = async ({ data }) => {
+    d = JSON.parse(data);
+{% if with_restart %}
+    if (
+      d.server_time != {{ server_time }} ||
+      d.configurations.length ||
+      d.templates.length
+    ) {
+      refreshPage();
+    } else if (d.styles.length) {
+      refreshStyle();
+    }
 {% endif %}
-  setTimeout(processMutations, pingInterval);
-}
-let mutationTimestamp = {{ mutation_timestamp }}, pingInterval = {{ minimum_ping_interval_in_milliseconds }};
-{% if not with_restart %}
-let isDone = 0;
+{% if step_name != 'input' %}
+    await Promise.all(d.variables.map(_ => refreshVariable(_.id)));
 {% endif %}
-schedulePolling();
+    mutationTime = d.mutation_time;
+  };
+}
+let mutationStream, mutationTimeout, mutationTime = {{ mutation_time }}, retrySeconds = 1;
+setupMutationStream();
 {% endif %}
-{%- endblock %}
+{% endblock %}
```

#### html2text {}

```diff
@@ -1,27 +1,27 @@
 {% extends base_template_path %} {% block head_html %} {{ super() -}}
- {%- endblock %} {% block body_js %} {% if step_name != 'input' %} async
-function runEach(xs) { await Promise.all((xs || []).map(_ => _())); } async
+ {% endblock %} {% block body_js %} {% if step_name != 'input' %} async
 function refreshVariable(variableId) { await runEach(functions[variableId]);
-await runEach(callbacks[variableId]); {% if not with_restart %} if (variableId
-== 'return_code') { isDone = 1; } {% endif %} } {% endif %} {{ super() -}} {%
-if with_restart or is_done == 0 %} async function processMutations() { const
-uri = '{{ root_uri }}{{ mutation_uri }}'; try { const r = await fetch(`$
-{uri}?t=${mutationTimestamp}`), d = await r.json(), { styles: ss, variables: vs
-} = d; {% if with_restart %} if ( d.server_timestamp != {{ server_timestamp }}
-|| d.configurations.length || d.templates.length ) { refreshPage(); } else if
-(ss.length) { refreshStyle(); } {% endif %} {% if step_name != 'input' %} await
-Promise.all(vs.map(_ => refreshVariable(_.id))); {% endif %} mutationTimestamp
-= d.mutation_timestamp; pingInterval = {{ minimum_ping_interval_in_milliseconds
-}}; } catch (e) { if (pingInterval < {{ maximum_ping_interval_in_milliseconds
-}}) { pingInterval *= 1.1; } console.error(e); } schedulePolling(); } {% if
-with_restart %} async function refreshPage() { const r = await fetch
-(location.href, { method: 'head' }); if (r.ok) { location.reload(); } else
-{ location.href = '{{ root_uri or '/' }}'; } } function refreshStyle() { const
-{ origin } = location; for (var l of document.getElementsByTagName('link'))
-{ if (l.rel !== 'stylesheet' || new URL(l.href).origin !== origin) { continue;
-} l.href += '?' + Date.now(); } } {% endif %} function schedulePolling() { {%
-if not with_restart %} if (isDone) { return; } {% endif %} setTimeout
-(processMutations, pingInterval); } let mutationTimestamp = {
-{ mutation_timestamp }}, pingInterval = {
-{ minimum_ping_interval_in_milliseconds }}; {% if not with_restart %} let
-isDone = 0; {% endif %} schedulePolling(); {% endif %} {%- endblock %}
+await runEach(callbacks[variableId]); {% if not with_restart and not
+has_interval %} if (variableId == 'return_code') { mutationStream.close(); } {%
+endif %} } async function runEach(xs) { await Promise.all((xs || []).map(_ => _
+())); } {% endif %} {{ super() -}} {% if with_restart or is_done == 0 %} {% if
+with_restart %} async function refreshPage() { const { status } = await fetch
+(location.href, { method: 'head' }); switch (status) { case 200:
+location.reload(); break; case 404: location.href = '{{ root_uri or '/' }}';
+break; default: setTimeout(refreshPage, 1000); } } function refreshStyle()
+{ const { origin } = location; for (var l of document.getElementsByTagName
+('link')) { if (l.rel !== 'stylesheet' || new URL(l.href).origin !== origin)
+{ continue; } l.href += '?' + Date.now(); } } {% endif %} function
+setupMutationStream() { mutationStream = new EventSource(rootUri + '/streams{
+{ mutation_uri }}?t=' + mutationTime); mutationStream.onopen = () =>
+{ retrySeconds = 1; }; mutationStream.onerror = () => { mutationStream.close();
+clearTimeout(mutationTimeout); mutationTimeout = setTimeout
+(setupMutationStream, retrySeconds); if (retrySeconds < 60) { retrySeconds *=
+2; } }; mutationStream.onmessage = async ({ data }) => { d = JSON.parse(data);
+{% if with_restart %} if ( d.server_time != {{ server_time }} ||
+d.configurations.length || d.templates.length ) { refreshPage(); } else if
+(d.styles.length) { refreshStyle(); } {% endif %} {% if step_name != 'input' %}
+await Promise.all(d.variables.map(_ => refreshVariable(_.id))); {% endif %}
+mutationTime = d.mutation_time; }; } let mutationStream, mutationTimeout,
+mutationTime = {{ mutation_time }}, retrySeconds = 1; setupMutationStream(); {%
+endif %} {% endblock %}
```

### Comparing `crosscompute-0.9.3.3/crosscompute/assets/radio-header.js` & `crosscompute-0.9.4.2/crosscompute/assets/radio-output-header.js`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.3.3/crosscompute/assets/radio-input.html` & `crosscompute-0.9.4.2/crosscompute/assets/radio-input.html`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.3.3/crosscompute/assets/table-header.js` & `crosscompute-0.9.4.2/crosscompute/assets/table-output-header.js`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.3.3/crosscompute/constants.py` & `crosscompute-0.9.4.2/crosscompute/constants.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,99 +1,122 @@
 import re
 from enum import IntEnum
 from os import getenv
 from pathlib import Path
 
 
+class Status(IntEnum):
+
+    NEW = 0
+    FAILED = -1
+    DONE = 100
+
+
 class Error(IntEnum):
 
     CONFIGURATION_NOT_FOUND = -100
     COMMAND_NOT_RUNNABLE = -10
     COMMAND_INTERRUPTED = -1
 
 
-class Status(IntEnum):
+class Info:
 
-    NEW = 0
-    FAILED = -1
-    DONE = 100
+    CONFIGURATION = 'c'
+    SCRIPT = 'f'
+    DATASET = 'd'
+    VARIABLE = 'v'
+    TEMPLATE = 't'
+    STYLE = 's'
+
+
+class Task:
+
+    RUN_PRINT = 'r'
+    PRINT_ONLY = 'p'
 
 
 PACKAGE_FOLDER = Path(__file__).parent
 ASSETS_FOLDER = PACKAGE_FOLDER / 'assets'
 TEMPLATE_PATH_BY_ID = {
     'base': str(ASSETS_FOLDER / 'base.html'),
     'live': str(ASSETS_FOLDER / 'live.html'),
     'root': str(ASSETS_FOLDER / 'root.html'),
     'automation': str(ASSETS_FOLDER / 'automation.html'),
     'batch': str(ASSETS_FOLDER / 'batch.html'),
     'step': str(ASSETS_FOLDER / 'step.html')}
+CACHE_FOLDER = Path('~/.crosscompute').expanduser()
+FILES_FOLDER = CACHE_FOLDER / 'files'
 
 
 ID_LENGTH = 32
 TOKEN_LENGTH = 32
 
 
 AUTOMATION_NAME = 'Automation X'
 AUTOMATION_VERSION = '0.0.0'
 AUTOMATION_PATH = Path('automate.yml')
 
 
 HOST = '127.0.0.1'
 PORT = 7000
-DISK_POLL_IN_MILLISECONDS = 1000
-DISK_DEBOUNCE_IN_MILLISECONDS = 1000
+DISK_DEBOUNCE_IN_MILLISECONDS = 1600
+DISK_STEP_IN_MILLISECONDS = 50
 
 
 AUTOMATION_ROUTE = '/a/{automation_slug}'
 BATCH_ROUTE = '/b/{batch_slug}'
 STEP_ROUTE = '/{step_code}'
 VARIABLE_ROUTE = '/{variable_id}'
-STYLE_ROUTE = '/s/{style_name}.css'
+FILES_ROUTE = '/files.json'
+STREAM_ROUTE = '/streams'
+STYLE_ROUTE = '/styles/{style_name}.css'
 MUTATION_ROUTE = '/mutations{uri}.json'
 PORT_ROUTE = '/ports{uri}'
 
 
+PRINTER_NAMES = 'pdf',
+
+
 PACKAGE_MANAGER_NAMES = 'apt', 'dnf', 'npm', 'pip'
 DESIGN_NAMES_BY_PAGE_ID = {
     'automation': ['input', 'output', 'none'],
-    'input': ['flex-vertical', 'none'],
-    'output': ['flex-vertical', 'none'],
-    'log': ['flex-vertical', 'none'],
-    'debug': ['flex-vertical', 'none'],
-}
-BUTTON_TEXT_BY_ID = {'run': 'Run'}
+    'input': ['flex', 'none'],
+    'output': ['flex', 'none'],
+    'log': ['flex', 'none'],
+    'debug': ['flex', 'none'],
+    'print': ['flex', 'none']}
+BUTTON_TEXT_BY_ID = {
+    'back': 'Back',
+    'continue': 'Continue'}
 
 
 INTERVAL_UNIT_NAMES = 'seconds', 'minutes', 'hours', 'days', 'weeks'
-STEP_NAMES = 'input', 'output', 'log', 'debug'
+STEP_NAMES = 'input', 'output', 'log', 'debug', 'print'
 STEP_NAME_BY_CODE = {_[0]: _ for _ in STEP_NAMES}
 STEP_CODE_BY_NAME = {k: v for v, k in STEP_NAME_BY_CODE.items()}
-MINIMUM_PING_INTERVAL_IN_SECONDS = 1
-MAXIMUM_PING_INTERVAL_IN_SECONDS = 30
 MAXIMUM_MUTATION_AGE_IN_SECONDS = 180
 
 
 VARIABLE_ID_PATTERN = re.compile(r'[a-zA-Z0-9-_ ]+$')
 VARIABLE_ID_TEMPLATE_PATTERN = re.compile(r'{ *([a-zA-Z0-9-_| ]+?) *}')
 VARIABLE_ID_WHITELIST_PATTERN = re.compile(r'{ *(ROOT_URI) *}')
 CACHED_FILE_SIZE_LIMIT_IN_BYTES = 1024
 MAXIMUM_FILE_CACHE_LENGTH = 256
 
 
-PRINTER_BY_NAME = {}
-VIEW_BY_NAME = {}
-
-
 MINIMUM_PORT = int(getenv('CROSSCOMPUTE_MINIMUM_PORT', 1024))
 MAXIMUM_PORT = int(getenv('CROSSCOMPUTE_MAXIMUM_PORT', 65535))
 PROXY_URI = getenv('CROSSCOMPUTE_PROXY_URI', '')
 
 
 DEBUG_VARIABLE_DICTIONARIES = [{
+    'id': 'source_time',
+    'view': 'number',
+    'path': 'variables.dictionary',
+}, {
     'id': 'execution_time_in_seconds',
     'view': 'number',
     'path': 'variables.dictionary',
 }, {
     'id': 'return_code',
     'view': 'number',
     'path': 'variables.dictionary'}]
```

### Comparing `crosscompute-0.9.3.3/crosscompute/dependencies.py` & `crosscompute-0.9.4.2/crosscompute/dependencies.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.3.3/crosscompute/exceptions.py` & `crosscompute-0.9.4.2/crosscompute/exceptions.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.3.3/crosscompute/macros/disk.py` & `crosscompute-0.9.4.2/crosscompute/macros/disk.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.3.3/crosscompute/macros/iterable.py` & `crosscompute-0.9.4.2/crosscompute/macros/iterable.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.3.3/crosscompute/macros/package.py` & `crosscompute-0.9.4.2/crosscompute/macros/package.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.3.3/crosscompute/macros/security.py` & `crosscompute-0.9.4.2/crosscompute/macros/security.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.3.3/crosscompute/routers/automation.py` & `crosscompute-0.9.4.2/crosscompute/routers/automation.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from time import time
 
 from fastapi import APIRouter, Depends, Request, Response, HTTPException
 from fastapi.responses import FileResponse
 from invisibleroads_macros_disk import make_random_folder
 
 from ..constants import (
+    Task,
     AUTOMATION_ROUTE,
     BATCH_ROUTE,
     ID_LENGTH,
     MUTATION_ROUTE,
     STEP_ROUTE,
     VARIABLE_ROUTE)
 from ..dependencies import (
@@ -64,16 +65,17 @@
     return TemplateResponse(template_path_by_id['automation'], {
         'request': request, 'title_text': automation_definition.name,
         'description': automation_definition.description,
         'host_uri': request_uri.scheme + '://' + request_uri.netloc,
         'name': automation_definition.name, 'uri': automation_uri,
         'automation_definition': automation_definition,
         'step_name': design_name,
-        'batches': guard.get_batch_definitions(automation_definition),
-        'mutation_timestamp': time(),
+        'batch_definitions': guard.get_batch_definitions(
+            automation_definition),
+        'mutation_time': time(),
     } | d, headers=response.headers)
 
 
 @router.post(
     AUTOMATION_ROUTE + '.json',
     tags=['automation'])
 async def run_automation_json(
@@ -89,17 +91,17 @@
     batch_definition = BatchDefinition({
         'folder': folder}, data_by_id=data_by_id, is_run=True)
     debug_folder = folder / 'debug'
     guard.save_identities(debug_folder / 'identities.dictionary')
     remove_variable_data(debug_folder / 'variables.dictionary', [
         'return_code'])
 
-    queue = site['queue']
-    environment = site['environment']
-    queue.put((automation_definition, batch_definition, environment))
+    site['tasks'].append((
+        automation_definition, batch_definition, site['environment'],
+        Task.RUN_PRINT))
     automation_definition.batch_definitions.append(batch_definition)
 
     step_code = 'l' if automation_definition.get_variable_definitions(
         'log') else 'o'
     return {
         'batch_slug': batch_definition.name,
         'step_code': step_code}
@@ -137,15 +139,15 @@
         request.query_params)
     return TemplateResponse(template_path_by_id['step'], {
         'request': request,
         'title_text': batch_definition.name,
         'automation_definition': automation_definition,
         'batch_definition': batch_definition,
         'step_name': step_name,
-        'mutation_timestamp': time(),
+        'mutation_time': time(),
     } | page_dictionary, headers=response.headers)
 
 
 @router.get(
     AUTOMATION_ROUTE + BATCH_ROUTE + STEP_ROUTE + VARIABLE_ROUTE + '.json',
     tags=['automation'])
 async def see_automation_batch_step_variable_json(
```

### Comparing `crosscompute-0.9.3.3/crosscompute/routers/root.py` & `crosscompute-0.9.4.2/crosscompute/routers/root.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     return TemplateResponse(template_path_by_id['root'], {
         'request': request,
         'title_text': site['name'],
         'css_uris': configuration.css_uris,
         'automation_definitions': guard.get_automation_definitions(
             configuration),
         'mutation_uri': MUTATION_ROUTE.format(uri=''),
-        'mutation_timestamp': time(),
+        'mutation_time': time(),
     }, headers=response.headers)
 
 
 @router.get('/favicon.ico', tags=['root'])
 async def see_icon(response: Response):
     return FileResponse(
         ASSETS_FOLDER / 'favicon.ico', headers=response.headers)
```

### Comparing `crosscompute-0.9.3.3/crosscompute/routers/token.py` & `crosscompute-0.9.4.2/crosscompute/routers/token.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.3.3/crosscompute/routines/authorization.py` & `crosscompute-0.9.4.2/crosscompute/routines/authorization.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.3.3/crosscompute/routines/automation.py` & `crosscompute-0.9.4.2/crosscompute/routines/work.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,173 +1,70 @@
-# TODO: Return unvalidated configuration when there is an exception
-# TODO: Watch multiple folders if not all under parent folder
-import requests
+# TODO: Consider giving scripts access to CROSSCOMPUTE_ROOT_URI
 import shlex
 import subprocess
-from contextlib import contextmanager
 from collections import defaultdict
 from concurrent.futures import (
     ProcessPoolExecutor, ThreadPoolExecutor, as_completed)
-from datetime import datetime
+from contextlib import contextmanager
 from logging import getLogger
 from os import environ, getenv, symlink
 from os.path import relpath
-from pathlib import Path
+from random import choice
+from threading import Thread
 from time import sleep, time
 from urllib.error import URLError
-from urllib.request import urlretrieve as download_url
+from urllib.request import urlretrieve as download_uri
 
+import requests
 from invisibleroads_macros_disk import make_folder
 from invisibleroads_macros_web.port import find_open_port
 from jinja2 import Template
 
 from ..constants import (
     Error,
-    AUTOMATION_PATH,
+    Info,
+    Task,
     AUTOMATION_ROUTE,
     BATCH_ROUTE,
-    DISK_DEBOUNCE_IN_MILLISECONDS,
-    DISK_POLL_IN_MILLISECONDS,
-    HOST,
     MAXIMUM_PORT,
     MINIMUM_PORT,
-    PORT,
     PORT_ROUTE,
     PROXY_URI,
     STEP_CODE_BY_NAME,
-    STEP_NAMES,
-    TOKEN_LENGTH)
+    STEP_NAMES)
 from ..exceptions import (
     CrossComputeConfigurationError,
-    CrossComputeConfigurationFormatError,
-    CrossComputeConfigurationNotFoundError,
     CrossComputeDataError,
-    CrossComputeError,
-    CrossComputeExecutionError)
-from ..macros.iterable import group_by
-from ..macros.security import DictionarySafe
-from ..settings import multiprocessing_context
-from .configuration import get_folder_plus_path, load_configuration
-from .interface import Automation
-from .server import DiskServer
+    CrossComputeExecutionError,
+    CrossComputeError)
+from ..macros.iterable import find_item, group_by
+from .configuration import (
+    get_folder_plus_path)
+from .printer import (
+    print_batch)
+from .uri import (
+    get_automation_slug,
+    get_batch_slug)
 from .variable import (
     get_variable_data_by_id,
     get_variable_value_by_id,
     process_variable_data,
     save_variable_data,
     update_variable_data)
 
 
-class DiskAutomation(Automation):
-
-    @classmethod
-    def load(Class, path_or_folder=None):
-        instance = Class()
-        path_or_folder = Path(path_or_folder)
-        if path_or_folder.is_dir():
-            instance._initialize_from_folder(path_or_folder)
-        else:
-            instance._initialize_from_path(path_or_folder)
-        with ThreadPoolExecutor() as executor:
-            futures = []
-            for automation_definition in instance.definitions:
-                futures.extend(executor.submit(
-                    _.get_command_string
-                ) for _ in automation_definition.script_definitions)
-            for future in as_completed(futures):
-                future.result()
-        return instance
-
-    def run(self, environment, with_rebuild=True):
-        for automation_definition in self.definitions:
-            prepare_automation(automation_definition, with_rebuild)
-        recurring_definitions = []
-        for automation_definition in self.definitions:
-            run_automation(
-                automation_definition, environment, with_rebuild)
-            if automation_definition.interval_timedelta:
-                recurring_definitions.append(automation_definition)
-        if not recurring_definitions:
-            return
-        while True:
-            for automation_definition in recurring_definitions:
-                last = automation_definition.interval_datetime
-                delta = automation_definition.interval_timedelta
-                if datetime.now() > last + delta:
-                    run_automation(
-                        automation_definition, environment, with_rebuild=False)
-            sleep(1)
-
-    def serve(
-            self, environment, host=HOST, port=PORT, with_restart=True,
-            with_prefix=True, with_hidden=True, root_uri='',
-            allowed_origins=None,
-            disk_poll_in_milliseconds=DISK_POLL_IN_MILLISECONDS,
-            disk_debounce_in_milliseconds=DISK_DEBOUNCE_IN_MILLISECONDS):
-        queue = multiprocessing_context.Queue()
-        with multiprocessing_context.Manager() as manager:
-            changes = manager.dict()
-            safe = DictionarySafe(manager.dict(), TOKEN_LENGTH)
-            DiskServer(
-                environment, safe, queue, _work, changes, host, port,
-                with_restart, with_prefix, with_hidden, root_uri,
-                allowed_origins,
-            ).watch(
-                self.configuration,
-                disk_poll_in_milliseconds,
-                disk_debounce_in_milliseconds,
-                self._reload)
-
-    def _reload(self):
-        path = self.path
-        if path.exists():
-            self._initialize_from_path(path)
-        else:
-            self._initialize_from_folder(self.folder)
-        return self.configuration
-
-    def _initialize_from_folder(self, folder):
-        paths = list(folder.iterdir())
-        default_automation_path = folder / AUTOMATION_PATH
-        if default_automation_path in paths:
-            paths.remove(default_automation_path)
-            paths.insert(0, default_automation_path)
-        for path in paths:
-            if path.is_dir():
-                continue
-            try:
-                self._initialize_from_path(path)
-            except CrossComputeConfigurationFormatError:
-                continue
-            except (CrossComputeConfigurationError, CrossComputeDataError):
-                raise
-            except CrossComputeError:
-                continue
-            break
-        else:
-            raise CrossComputeConfigurationNotFoundError(
-                'configuration not found')
-
-    def _initialize_from_path(self, path):
-        configuration = load_configuration(path)
-        self.configuration = configuration
-        self.path = path
-        self.folder = configuration.folder
-        self.definitions = configuration.automation_definitions
-
-
 class AbstractEngine():
 
     def __init__(self, with_rebuild=True):
         self.with_rebuild = with_rebuild
 
     def run_batch(
             self, automation_definition, batch_definition, user_environment):
         reference_time = time()
-        batch_folder, batch_environment = _prepare_batch(
+        batch_folder, batch_environment = prepare_batch(
             automation_definition, batch_definition)
         if not automation_definition.script_definitions:
             return
         batch_identifier = ' '.join([
             automation_definition.name, automation_definition.version,
             str(batch_folder)])
         L.info('%s running', batch_identifier)
@@ -191,15 +88,16 @@
             'output', 'log', 'debug',
         ], {'debug': {
             'source_time': reference_time,
             'execution_time_in_seconds': time() - reference_time,
             'return_code': return_code}})
 
     def prepare(self, automation_definition):
-        pass
+        for s in automation_definition.script_definitions:
+            s.get_command_string()
 
 
 class UnsafeEngine(AbstractEngine):
 
     def run(self, automation_definition, batch_folder, custom_environment):
         step_folder_by_name = _get_step_folder_by_name(
             automation_definition.folder, batch_folder)
@@ -227,16 +125,16 @@
             return
         automation_folder = automation_definition.folder
         (automation_folder / CONTAINER_FILE_NAME).write_text(
             _prepare_container_file_text(automation_definition))
         (automation_folder / '.containerignore').write_text(
             CONTAINER_IGNORE_TEXT)
         command_texts = [
-            _.get_command_string().format(**CONTAINER_STEP_FOLDER_BY_NAME)
-            for _ in automation_definition.script_definitions]
+            s.get_command_string().format(**CONTAINER_STEP_FOLDER_BY_NAME)
+            for s in automation_definition.script_definitions]
         (automation_folder / CONTAINER_SCRIPT_NAME).write_text(
             '\n'.join([_ + CONTAINER_PIPE_TEXT for _ in command_texts]))
         if subprocess.run([
             'podman', 'build', '-t', image_name, '-f', CONTAINER_FILE_NAME,
         ], cwd=automation_folder).returncode != 0:
             raise CrossComputeExecutionError(f'could not build "{image_name}"')
 
@@ -257,28 +155,43 @@
         except KeyboardInterrupt:
             return_code = Error.COMMAND_INTERRUPTED
         except Exception:
             raise
         finally:
             _set_podman_folder_owner(absolute_batch_folder, 0)
             _run_podman_command({}, ['kill', container_id])
-        if return_code in [126, 127]:
-            x = 'denied permission' if return_code == 126 else 'not found'
-            error = CrossComputeConfigurationError(
-                'command %s in container; check script definitions' % x)
-            error.code = Error.COMMAND_NOT_RUNNABLE
-            raise error
-        elif return_code != 0:
-            error_text = (
-                automation_folder / batch_folder / 'debug' / 'stderr.txt'
-            ).read_text()
-            error = CrossComputeExecutionError(error_text.rstrip())
-            error.code = return_code
-            raise error
-        return return_code
+        return _process_podman_return_code(return_code, absolute_batch_folder)
+
+
+def run_automation(automation_definition, user_environment, with_rebuild=True):
+    ds = []
+    run_batch = get_script_engine(
+        automation_definition.engine_name, with_rebuild).run_batch
+    concurrency_name = automation_definition.batch_concurrency_name
+    update_datasets(automation_definition)
+    try:
+        if concurrency_name == 'single':
+            ds.extend(_run_automation_single(
+                automation_definition, run_batch, user_environment))
+        else:
+            ds.extend(_run_automation_multiple(
+                automation_definition, run_batch, user_environment,
+                concurrency_name))
+    except CrossComputeError as e:
+        e.automation_definition = automation_definition
+        L.error(e)
+    return ds
+
+
+def run_batch(automation_definition, batch_definition, user_environment):
+    engine = get_script_engine(
+        automation_definition.engine_name, with_rebuild=False)
+    update_datasets(automation_definition)
+    engine.run_batch(
+        automation_definition, batch_definition, user_environment)
 
 
 def get_script_engine(engine_name, with_rebuild=True):
     try:
         ScriptEngine = {
             'unsafe': UnsafeEngine,
             'podman': PodmanEngine,
@@ -300,77 +213,254 @@
             if target_path.is_symlink():
                 if target_path.resolve() == source_path.resolve():
                     continue
                 target_path.unlink()
             elif target_path.exists():
                 continue
             symlink(relpath(source_path, target_folder), target_path)
-        elif 'url' in reference_configuration:
-            reference_url = reference_configuration['url']
+        elif 'uri' in reference_configuration:
+            reference_uri = reference_configuration['uri']
             try:
-                download_url(reference_url, target_path)
+                download_uri(reference_uri, target_path)
             except URLError:
-                L.error(f'could not download dataset from {reference_url}')
+                L.error(f'could not download dataset from {reference_uri}')
+
+
+def process_loop(
+        automation_definitions, automation_tasks, live_uris, file_changes,
+        user_environment, server_uri, with_rebuild):
+    for a in automation_definitions:
+        prepare_automation(a, with_rebuild)
+        for b in a.batch_definitions:
+            prepare_batch(a, b)
+    try:
+        while True:
+            sleep(1)
+            try:
+                automation_task = _get_automation_task(
+                    automation_tasks, automation_definitions, live_uris,
+                    file_changes, user_environment)
+            except IndexError:
+                continue
+            thread = Thread(
+                target=_process_task, args=automation_task + (server_uri,),
+                daemon=True)
+            thread.start()
+    except KeyboardInterrupt:
+        pass
 
 
 def prepare_automation(automation_definition, with_rebuild=True):
     engine = get_script_engine(automation_definition.engine_name, with_rebuild)
     engine.prepare(automation_definition)
 
 
-def run_automation(automation_definition, user_environment, with_rebuild=True):
-    ds = []
-    run_batch = get_script_engine(
-        automation_definition.engine_name, with_rebuild).run_batch
-    concurrency_name = automation_definition.batch_concurrency_name
-    update_datasets(automation_definition)
-    try:
-        if concurrency_name == 'single':
-            ds.extend(_run_automation_single(
-                automation_definition, run_batch, user_environment))
-        else:
-            ds.extend(_run_automation_multiple(
-                automation_definition, run_batch, user_environment,
-                concurrency_name))
-    except CrossComputeError as e:
-        e.automation_definition = automation_definition
-        L.error(e)
-    automation_definition.interval_datetime = datetime.now()
-    return ds
+def prepare_batch(automation_definition, batch_definition):
+    variable_definitions = automation_definition.get_variable_definitions(
+        'input')
+    variable_definitions_by_path = group_by(variable_definitions, 'path')
+    data_by_id = batch_definition.data_by_id
+    batch_folder = batch_definition.folder
+    batch_environment = _prepare_batch_environment(
+        automation_definition,
+        variable_definitions_by_path.pop('ENVIRONMENT', []),
+        data_by_id)
+    step_folder_by_name = _make_step_folder_by_name(
+        automation_definition.folder, batch_folder)
+    if not data_by_id:
+        return batch_folder, batch_environment
+    input_folder = step_folder_by_name['input_folder']
+    for path, variable_definitions in variable_definitions_by_path.items():
+        input_path = input_folder / path
+        save_variable_data(input_path, data_by_id, variable_definitions)
+    return batch_folder, batch_environment
 
 
 def _run_automation_single(automation_definition, run_batch, user_environment):
     ds = []
     for batch_definition in automation_definition.batch_definitions:
         ds.append(run_batch(
             automation_definition, batch_definition, user_environment))
     return ds
 
 
 def _run_automation_multiple(
         automation_definition, run_batch, user_environment, concurrency_name):
     ds = []
-    if concurrency_name == 'process':
-        BatchExecutor = ProcessPoolExecutor
-    else:
+    if concurrency_name == 'thread':
         BatchExecutor = ThreadPoolExecutor
+    else:
+        BatchExecutor = ProcessPoolExecutor
     with BatchExecutor() as executor:
         futures = []
         for batch_definition in automation_definition.batch_definitions:
             futures.append(executor.submit(
                 run_batch, automation_definition, batch_definition,
                 user_environment))
         try:
             for future in as_completed(futures):
                 ds.append(future.result())
         except KeyboardInterrupt:
             pass
     return ds
 
 
+def _get_automation_task(
+        automation_tasks, automation_definitions, live_uris, file_changes,
+        user_environment):
+    if automation_tasks:
+        return automation_tasks.pop(0)
+    automation_definition = None
+    if live_uris:
+        try:
+            automation_definition, batch_definition = _get_automation_pack(
+                automation_definitions, choice(live_uris))
+        except IndexError:
+            pass
+        if automation_definition:
+            task_mode = _get_task_mode(
+                automation_definition, batch_definition, file_changes)
+            if task_mode is None:
+                automation_definition = None
+    if not automation_definition:
+        selected_automation_definitions = [
+            _ for _ in automation_definitions if _.is_interval_strict]
+        if selected_automation_definitions:
+            automation_definition = choice(selected_automation_definitions)
+            batch_definition = choice(automation_definition.batch_definitions)
+            if automation_definition.is_interval_ready(batch_definition):
+                task_mode = Task.RUN_PRINT
+            else:
+                automation_definition = None
+    if automation_definition:
+        batch_clock = batch_definition.clock
+        if batch_clock.is_in('run') or batch_clock.is_in('print'):
+            automation_definition = None
+    if not automation_definition:
+        raise IndexError
+    return automation_definition, batch_definition, user_environment, task_mode
+
+
+def _get_automation_pack(automation_definitions, reference_uri):
+    automation_slug = get_automation_slug(reference_uri)
+    if not automation_slug:
+        raise IndexError
+    try:
+        automation_definition = find_item(
+            automation_definitions, 'slug', automation_slug,
+            normalize=str.casefold)
+    except StopIteration:
+        raise IndexError
+    batch_slug = get_batch_slug(reference_uri)
+    if batch_slug:
+        try:
+            batch_definition = find_item(
+                automation_definition.batch_definitions, 'slug', batch_slug)
+        except StopIteration:
+            raise IndexError
+    else:
+        batch_definition = automation_definition.batch_definitions[0]
+    return automation_definition, batch_definition
+
+
+def _get_task_mode(automation_definition, batch_definition, file_changes):
+    batch_clock = batch_definition.clock
+    run_time = batch_clock.get_start_time('run')
+    if not run_time:
+        return Task.RUN_PRINT
+    print_time = batch_clock.get_start_time('print')
+    for t, infos in file_changes.items():
+        if t < run_time:
+            continue
+        for info in infos:
+            match info['code']:
+                case Info.VARIABLE:
+                    if info['step'] != 'i' or batch_clock.is_in('run', t):
+                        continue
+                    return Task.RUN_PRINT
+                case Info.SCRIPT:
+                    try:
+                        automation_definition.script_definitions[
+                            info['index']].command = None
+                    except AttributeError:
+                        pass
+                    return Task.RUN_PRINT
+                case Info.DATASET:
+                    return Task.RUN_PRINT
+        if t < print_time:
+            continue
+        for info in infos:
+            if info['code'] in [Info.STYLE, Info.TEMPLATE]:
+                return Task.PRINT_ONLY
+    if automation_definition.is_interval_ready(batch_definition):
+        return Task.RUN_PRINT
+
+
+def _process_task(
+        automation_definition, batch_definition, user_environment, task_mode,
+        server_uri):
+    batch_clock = batch_definition.clock
+    try:
+        if task_mode == Task.RUN_PRINT:
+            with batch_clock.time('run'):
+                run_batch(
+                    automation_definition, batch_definition, user_environment)
+        with batch_clock.time('print'):
+            print_batch(
+                automation_definition, batch_definition, server_uri,
+                is_draft=True)
+    except CrossComputeError as e:
+        e.automation_definition = automation_definition
+        L.error(e)
+    except KeyboardInterrupt:
+        pass
+
+
+def _prepare_batch_environment(
+        automation_definition, variable_definitions, data_by_id):
+    batch_environment = {}
+    for variable_id in automation_definition.environment_variable_ids:
+        batch_environment[variable_id] = environ[variable_id]
+    for variable_id in (_.id for _ in variable_definitions):
+        if variable_id in data_by_id:
+            continue
+        try:
+            batch_environment[variable_id] = environ[variable_id]
+        except KeyError:
+            raise CrossComputeConfigurationError(
+                f'{variable_id} is missing in the environment')
+    variable_data_by_id = get_variable_data_by_id(
+        variable_definitions, data_by_id, with_exceptions=False)
+    variable_value_by_id = get_variable_value_by_id(variable_data_by_id)
+    return batch_environment | variable_value_by_id
+
+
+def _prepare_script_environment(
+        step_folder_by_name, custom_environment, with_path=False):
+    script_environment = custom_environment | {
+        'CROSSCOMPUTE_' + k.upper(): v for k, v in step_folder_by_name.items()}
+    if with_path:
+        script_environment['PATH'] = getenv('PATH', '')
+    return script_environment
+
+
+def _make_step_folder_by_name(automation_folder, batch_folder):
+    step_folder_by_name = _get_step_folder_by_name(
+        automation_folder, batch_folder)
+    for folder in step_folder_by_name.values():
+        folder.mkdir(parents=True, exist_ok=True)
+    return step_folder_by_name
+
+
+def _get_step_folder_by_name(automation_folder, batch_folder):
+    return {
+        _ + '_folder': automation_folder / batch_folder / _
+        for _ in STEP_NAMES}
+
+
 def _run_script(
         script_definition, step_folder_by_name, script_environment,
         stdout_file, stderr_file):
     command_string = script_definition.get_command_string()
     if not command_string:
         return
     command_text = command_string.format(**step_folder_by_name)
@@ -401,14 +491,83 @@
         e_file.seek(0)
         error = CrossComputeExecutionError(e_file.read().rstrip())
         error.code = e.returncode
         raise error
     return process.returncode
 
 
+def _process_batch(
+        automation_definition, batch_definition, step_names,
+        extra_data_by_id_by_step_name):
+    variable_data_by_id_by_step_name = {}
+    automation_folder = automation_definition.folder
+    batch_folder = batch_definition.folder
+    for step_name in step_names:
+        variable_data_by_id_by_step_name[step_name] = variable_data_by_id = {}
+        extra_data_by_id = extra_data_by_id_by_step_name.get(step_name, {})
+        step_folder = automation_folder / batch_folder / step_name
+        variable_definitions = automation_definition.get_variable_definitions(
+            step_name)
+        for variable_definition in variable_definitions:
+            variable_id = variable_definition.id
+            variable_path = variable_definition.path
+            if variable_id in extra_data_by_id:
+                continue
+            path = step_folder / variable_path
+            try:
+                variable_data = process_variable_data(
+                    path, variable_definition)
+            except CrossComputeDataError as e:
+                e.automation_definition = automation_definition
+                L.error(e)
+                continue
+            variable_data_by_id[variable_id] = variable_data
+        if extra_data_by_id:
+            update_variable_data(
+                step_folder / 'variables.dictionary', extra_data_by_id)
+            variable_data_by_id.update(extra_data_by_id)
+    return variable_data_by_id_by_step_name
+
+
+def _prepare_container_file_text(automation_definition):
+    path_folders = set()
+    package_ids_by_manager_name = defaultdict(set)
+    for package_definition in automation_definition.package_definitions:
+        manager_name = package_definition.manager_name
+        package_ids_by_manager_name[manager_name].add(package_definition.id)
+    root_package_commands, user_package_commands = [], []
+    if 'apt' in package_ids_by_manager_name:
+        s = ' '.join(sorted(package_ids_by_manager_name['apt']))
+        root_package_commands.append(
+            f'apt update && apt -y install {s} && apt clean')
+    if 'dnf' in package_ids_by_manager_name:
+        s = ' '.join(sorted(package_ids_by_manager_name['dnf']))
+        root_package_commands.append(
+            f'dnf -y install {s} && dnf clean all')
+    if 'npm' in package_ids_by_manager_name:
+        s = ' '.join(sorted(package_ids_by_manager_name['npm']))
+        user_package_commands.append(
+            f'npm install {s} --prefix ~/.local -g && '
+            f'npm cache clean --force')
+        path_folders.add('/home/user/.local/bin')
+    if 'pip' in package_ids_by_manager_name:
+        s = ' '.join(sorted(package_ids_by_manager_name['pip']))
+        user_package_commands.append(
+            f'pip install {s} --user && '
+            f'pip cache purge && rm -rf ~/.cache')
+        path_folders.add('/home/user/.local/bin')
+    return CONTAINER_FILE_TEXT.render(
+        parent_image_name=automation_definition.parent_image_name,
+        root_package_commands=root_package_commands,
+        user_package_commands=user_package_commands,
+        path_folders=path_folders,
+        port_numbers=[str(
+            _.number) for _ in automation_definition.port_definitions])
+
+
 def _has_podman_image(image_name):
     return _run_podman_command({}, [
         'image', 'exists', image_name]).returncode == 0
 
 
 def _run_podman_image(automation_definition, batch_folder, custom_environment):
     automation_folder = automation_definition.folder
@@ -440,17 +599,24 @@
         }, ['run'] + command_terms + ['-d', image_name])
         if process.returncode == 0:
             break
     container_id = process.stdout.decode().rstrip()
     return container_id, port_packs
 
 
+def _get_image_name(automation_definition):
+    automation_slug = automation_definition.slug
+    automation_version = automation_definition.version
+    return f'{automation_slug}:{automation_version}'
+
+
 @contextmanager
 def _proxy_podman_ports(
         automation_definition, batch_folder, custom_environment, port_packs):
+    # TODO: Check if this works in jupyterlab extension
     origin_uri = custom_environment.get('CROSSCOMPUTE_ORIGIN_URI', '')
     relative_uris = []
     if PROXY_URI:
         def get_port_uri(target_uri, relative_uri):
             requests.post(PROXY_URI + relative_uri, json={
                 'target': target_uri})
             relative_uris.append(relative_uri)
@@ -489,189 +655,44 @@
     for dataset_definition in automation_definition.dataset_definitions:
         dataset_path = dataset_definition.path
         _make_podman_folder(container_id, dataset_path.parent)
         _run_podman_command({'cwd': automation_folder}, [
             'cp', dataset_path, f'{container_id}:{dataset_path}'])
 
 
-def _make_podman_folder(container_id, folder):
-    _run_podman_command({}, ['exec', container_id, 'mkdir', folder, '-p'])
-
-
 def _set_podman_folder_owner(folder, user_id):
     _run_podman_command({}, [
         'unshare', 'chown', f'{user_id}:{user_id}', str(folder), '-R'])
 
 
+def _make_podman_folder(container_id, folder):
+    _run_podman_command({}, ['exec', container_id, 'mkdir', folder, '-p'])
+
+
 def _run_podman_command(options, terms):
     command_terms = ['podman'] + terms
     L.debug(command_terms)
     return subprocess.run(command_terms, **options)
 
 
-def _work(automation_queue):
-    try:
-        while automation_pack := automation_queue.get():
-            worker_process = multiprocessing_context.Process(
-                target=_work_one, args=(automation_pack,), daemon=True)
-            worker_process.start()
-    except KeyboardInterrupt:
-        pass
-
-
-def _work_one(automation_pack):
-    try:
-        automation_definition = automation_pack[0]
-        engine = get_script_engine(
-            automation_definition.engine_name, with_rebuild=False)
-        update_datasets(automation_definition)
-        engine.run_batch(*automation_pack)
-    except CrossComputeError as e:
-        e.automation_definition = automation_definition
-        L.error(e)
-    except KeyboardInterrupt:
-        pass
-
-
-def _prepare_batch(automation_definition, batch_definition):
-    variable_definitions = automation_definition.get_variable_definitions(
-        'input')
-    variable_definitions_by_path = group_by(variable_definitions, 'path')
-    data_by_id = batch_definition.data_by_id
-    batch_folder = batch_definition.folder
-    batch_environment = _prepare_batch_environment(
-        automation_definition,
-        variable_definitions_by_path.pop('ENVIRONMENT', []),
-        data_by_id)
-    step_folder_by_name = _make_step_folder_by_name(
-        automation_definition.folder, batch_folder)
-    if not data_by_id:
-        return batch_folder, batch_environment
-    input_folder = step_folder_by_name['input_folder']
-    for path, variable_definitions in variable_definitions_by_path.items():
-        input_path = input_folder / path
-        save_variable_data(input_path, data_by_id, variable_definitions)
-    return batch_folder, batch_environment
-
-
-def _make_step_folder_by_name(automation_folder, batch_folder):
-    step_folder_by_name = _get_step_folder_by_name(
-        automation_folder, batch_folder)
-    for folder in step_folder_by_name.values():
-        folder.mkdir(parents=True, exist_ok=True)
-    return step_folder_by_name
-
-
-def _get_step_folder_by_name(automation_folder, batch_folder):
-    return {
-        _ + '_folder': automation_folder / batch_folder / _
-        for _ in STEP_NAMES}
-
-
-def _prepare_container_file_text(automation_definition):
-    path_folders = set()
-    package_ids_by_manager_name = defaultdict(set)
-    for package_definition in automation_definition.package_definitions:
-        manager_name = package_definition.manager_name
-        package_ids_by_manager_name[manager_name].add(package_definition.id)
-    root_package_commands, user_package_commands = [], []
-    if 'apt' in package_ids_by_manager_name:
-        s = ' '.join(sorted(package_ids_by_manager_name['apt']))
-        root_package_commands.append(
-            f'apt update && apt -y install {s} && apt clean')
-    if 'dnf' in package_ids_by_manager_name:
-        s = ' '.join(sorted(package_ids_by_manager_name['dnf']))
-        root_package_commands.append(
-            f'dnf -y install {s} && dnf clean all')
-    if 'npm' in package_ids_by_manager_name:
-        s = ' '.join(sorted(package_ids_by_manager_name['npm']))
-        user_package_commands.append(
-            f'npm install {s} --prefix ~/.local -g && '
-            f'npm cache clean --force')
-        path_folders.add('/home/user/.local/bin')
-    if 'pip' in package_ids_by_manager_name:
-        s = ' '.join(sorted(package_ids_by_manager_name['pip']))
-        user_package_commands.append(
-            f'pip install {s} --user && '
-            f'pip cache purge && rm -rf ~/.cache')
-        path_folders.add('/home/user/.local/bin')
-    return CONTAINER_FILE_TEXT.render(
-        parent_image_name=automation_definition.parent_image_name,
-        root_package_commands=root_package_commands,
-        user_package_commands=user_package_commands,
-        path_folders=path_folders,
-        port_numbers=[str(
-            _.number) for _ in automation_definition.port_definitions])
-
-
-def _prepare_script_environment(
-        step_folder_by_name, custom_environment, with_path=False):
-    script_environment = custom_environment | {
-        'CROSSCOMPUTE_' + k.upper(): v for k, v in step_folder_by_name.items()}
-    if with_path:
-        script_environment['PATH'] = getenv('PATH', '')
-    return script_environment
-
-
-def _prepare_batch_environment(
-        automation_definition, variable_definitions, data_by_id):
-    batch_environment = {}
-    for variable_id in automation_definition.environment_variable_ids:
-        batch_environment[variable_id] = environ[variable_id]
-    for variable_id in (_.id for _ in variable_definitions):
-        if variable_id in data_by_id:
-            continue
-        try:
-            batch_environment[variable_id] = environ[variable_id]
-        except KeyError:
-            raise CrossComputeConfigurationError(
-                f'{variable_id} is missing in the environment')
-    variable_data_by_id = get_variable_data_by_id(
-        variable_definitions, data_by_id, with_exceptions=False)
-    variable_value_by_id = get_variable_value_by_id(variable_data_by_id)
-    return batch_environment | variable_value_by_id
-
-
-def _process_batch(
-        automation_definition, batch_definition, step_names,
-        extra_data_by_id_by_step_name):
-    variable_data_by_id_by_step_name = {}
-    automation_folder = automation_definition.folder
-    batch_folder = batch_definition.folder
-    for step_name in step_names:
-        variable_data_by_id_by_step_name[step_name] = variable_data_by_id = {}
-        extra_data_by_id = extra_data_by_id_by_step_name.get(step_name, {})
-        step_folder = automation_folder / batch_folder / step_name
-        variable_definitions = automation_definition.get_variable_definitions(
-            step_name)
-        for variable_definition in variable_definitions:
-            variable_id = variable_definition.id
-            variable_path = variable_definition.path
-            if variable_id in extra_data_by_id:
-                continue
-            path = step_folder / variable_path
-            try:
-                variable_data = process_variable_data(
-                    path, variable_definition)
-            except CrossComputeDataError as e:
-                e.automation_definition = automation_definition
-                L.error(e)
-                continue
-            variable_data_by_id[variable_id] = variable_data
-        if extra_data_by_id:
-            update_variable_data(
-                step_folder / 'variables.dictionary', extra_data_by_id)
-            variable_data_by_id.update(extra_data_by_id)
-    return variable_data_by_id_by_step_name
-
-
-def _get_image_name(automation_definition):
-    automation_slug = automation_definition.slug
-    automation_version = automation_definition.version
-    return f'{automation_slug}:{automation_version}'
+def _process_podman_return_code(return_code, absolute_batch_folder):
+    if return_code in [126, 127]:
+        x = 'denied permission' if return_code == 126 else 'not found'
+        error = CrossComputeConfigurationError(
+            'command %s in container; check script definitions' % x)
+        error.code = Error.COMMAND_NOT_RUNNABLE
+        raise error
+    elif return_code != 0:
+        error_text = (
+            absolute_batch_folder / 'debug' / 'stderr.txt'
+        ).read_text()
+        error = CrossComputeExecutionError(error_text.rstrip())
+        error.code = return_code
+        raise error
+    return return_code
 
 
 CONTAINER_IGNORE_TEXT = '''\
 **/.git
 **/.gitignore
 **/.gitmodules
 **/.ipynb_checkpoints
@@ -702,16 +723,14 @@
 {% endif %}
 {% if port_numbers %}
 EXPOSE {{ ' '.join(port_numbers) }}
 {% endif %}
 COPY --chown=user:user . .
 CMD ["sleep", "infinity"]''', trim_blocks=True)
 CONTAINER_PIPE_TEXT = (
-    ' 1>>runs/next/debug/stdout.txt'
-    ' 2>>runs/next/debug/stderr.txt')
+    ' 1>runs/next/debug/stdout.txt'
+    ' 2>runs/next/debug/stderr.txt')
 CONTAINER_SCRIPT_NAME = '.run.sh'
 CONTAINER_ENV_NAME = '.run.env'
 CONTAINER_STEP_FOLDER_BY_NAME = {
     _ + '_folder': 'runs/next/' + _ for _ in STEP_NAMES}
-
-
 L = getLogger(__name__)
```

### Comparing `crosscompute-0.9.3.3/crosscompute/routines/batch.py` & `crosscompute-0.9.4.2/crosscompute/routines/batch.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.3.3/crosscompute/routines/configuration.py` & `crosscompute-0.9.4.2/crosscompute/routines/configuration.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # TODO: Save to ini, toml
 import json
 import shutil
 from collections import Counter
 from configparser import ConfigParser
-from datetime import timedelta
+from datetime import datetime, timedelta
 from logging import getLogger
 from os import environ
 from os.path import basename, relpath, splitext
 from pathlib import Path
 from string import Template
 from time import time
 
 import tomli
 from invisibleroads_macros_log import format_path
-from invisibleroads_macros_text import format_slug
+from invisibleroads_macros_text import format_name, format_slug
 from nbconvert import PythonExporter
 from nbformat import read as load_notebook, NO_CONVERT
 from ruamel.yaml import YAML
 from ruamel.yaml.error import YAMLError
 
 from .. import __version__
 from ..constants import (
@@ -27,28 +27,32 @@
     AUTOMATION_VERSION,
     BATCH_ROUTE,
     BUTTON_TEXT_BY_ID,
     DEBUG_VARIABLE_DICTIONARIES,
     DESIGN_NAMES_BY_PAGE_ID,
     INTERVAL_UNIT_NAMES,
     PACKAGE_MANAGER_NAMES,
-    PRINTER_BY_NAME,
+    PRINTER_NAMES,
     STEP_NAMES,
     STYLE_ROUTE,
     VARIABLE_ID_PATTERN,
-    VARIABLE_ID_TEMPLATE_PATTERN,
-    VIEW_BY_NAME)
+    VARIABLE_ID_TEMPLATE_PATTERN)
 from ..exceptions import (
     CrossComputeConfigurationError,
     CrossComputeConfigurationFormatError,
     CrossComputeConfigurationNotImplementedError,
     CrossComputeError)
 from ..macros.iterable import find_item
+from ..macros.log import Clock
 from ..macros.package import is_equivalent_version
-from .printer import initialize_printer_by_name
+from ..settings import (
+    printer_by_name,
+    view_by_name)
+from .printer import (
+    initialize_printer_by_name)
 from .variable import (
     format_text,
     get_data_by_id_from_folder,
     initialize_view_by_name,
     YIELD_DATA_BY_ID_BY_EXTENSION)
 
 
@@ -92,57 +96,48 @@
             validate_batches,
             validate_datasets,
             validate_scripts,
             validate_environment,
             validate_display_styles,
             validate_display_templates,
             validate_display_pages,
-            validate_display_buttons,
-            validate_prints]
+            validate_display_buttons]
 
     def get_variable_definitions(self, step_name, with_all=False):
         variable_definitions = self.variable_definitions_by_step_name.get(
             step_name, [])
         if with_all:
             variable_definitions = variable_definitions.copy()
             for STEP_NAME in STEP_NAMES:
                 if step_name == STEP_NAME:
                     continue
                 variable_definitions.extend(self.get_variable_definitions(
                     STEP_NAME))
         return variable_definitions
 
-    def get_template_text(self, step_name):
-        automation_folder = self.folder
-        variable_definitions = self.get_variable_definitions(step_name)
-        template_definitions = self.template_definitions_by_step_name[
-            step_name]
-        return get_template_text(
-            template_definitions, automation_folder, variable_definitions)
-
     def get_design_name(self, page_id):
         design_name = DESIGN_NAMES_BY_PAGE_ID[page_id][0]
         if page_id in self.page_definition_by_id:
             page_definition = self.page_definition_by_id[page_id]
             design_name = page_definition.configuration.get(
                 'design', design_name)
         elif page_id in STEP_NAMES:
             variable_definitions = self.get_variable_definitions(page_id)
             if not variable_definitions:
                 design_name = 'none'
         return design_name
 
-    def get_button_text(self, button_id):
-        button_text = BUTTON_TEXT_BY_ID[button_id]
-        button_definition_by_id = self.button_definition_by_id
-        if button_id in button_definition_by_id:
-            button_definition = button_definition_by_id[button_id]
-            button_configuration = button_definition.configuration
-            button_text = button_configuration.get('button-text', button_text)
-        return button_text
+    def is_interval_ready(self, batch_definition):
+        interval_timedelta = self.interval_timedelta
+        if interval_timedelta:
+            run_datetime = datetime.fromtimestamp(
+                batch_definition.clock.get_end_time('run'))
+            if datetime.now() > run_datetime + interval_timedelta:
+                return True
+        return False
 
 
 class VariableDefinition(Definition):
 
     def _initialize(self, kwargs):
         self.step_name = kwargs['step_name']
         self._validation_functions = [
@@ -210,20 +205,21 @@
                     'exporting %s to %s in %s', self.path, script_path, folder)
                 try:
                     script_text = PythonExporter().from_notebook_node(
                         load_notebook(old_path, NO_CONVERT))[0]
                     with new_path.open('wt') as script_file:
                         script_file.write(script_text)
                 except Exception as e:
-                    raise CrossComputeConfigurationError(e)
+                    e = CrossComputeConfigurationError(e)
+                    e.path = new_path
+                    L.error(e)
         elif 'function' in self:
             script_path = '.run.py'
-            new_path = folder / script_path
             function_string = self['function']
-            with new_path.open('wt') as f:
+            with (folder / script_path).open('wt') as f:
                 f.write(RUN_PY.substitute({
                     'module_name': function_string.split('.')[0],
                     'function_string': function_string}))
         else:
             return
         self.command = command_string = f'python3 "{script_path}"'
         return command_string
@@ -284,34 +280,27 @@
 class PermissionDefinition(Definition):
 
     def _initialize(self, kwargs):
         self._validation_functions = [
             validate_permission_identifiers]
 
 
-class PrintDefinition(Definition):
-
-    def _initialize(self, kwargs):
-        self._validation_functions = [
-            validate_print_identifiers,
-            validate_print_configuration,
-            validate_header_footer_options,
-            validate_page_number_options]
-
-
 def save_raw_configuration(configuration_path, configuration):
     configuration_format = get_configuration_format(configuration_path)
     save_raw_configuration = {
         'yaml': save_raw_configuration_yaml,
     }[configuration_format]
     return save_raw_configuration(configuration_path, configuration)
 
 
 def save_raw_configuration_yaml(configuration_path, configuration):
+    # TODO: Add --- at top
     yaml = YAML()
+    yaml.explicit_start = True
+    yaml.indent(mapping=2, sequence=4, offset=2)
     try:
         with open(configuration_path, 'wt') as configuration_file:
             yaml.dump(configuration, configuration_file)
     except (OSError, YAMLError) as e:
         raise CrossComputeConfigurationError(e)
     return configuration_path
 
@@ -433,14 +422,16 @@
         'import_configurations': import_configurations,
         'automation_definitions': automation_definitions}
 
 
 def validate_variables(configuration):
     variable_definitions_by_step_name = {}
     view_names = set()
+    if 'print' in configuration:
+        initialize_printer_by_name()
     for step_name in STEP_NAMES:
         step_configuration = get_dictionary(configuration, step_name)
         variable_dictionaries = get_dictionaries(
             step_configuration, 'variables')
         if step_name == 'debug':
             variable_dictionaries[:0] = DEBUG_VARIABLE_DICTIONARIES
         variable_definitions = [VariableDefinition(
@@ -453,19 +444,18 @@
     L.debug('view_names = %s', list(view_names))
     return {
         'variable_definitions_by_step_name': variable_definitions_by_step_name,
         '___view_names': view_names}
 
 
 def validate_variable_views(configuration):
-    # TODO: Validate variable view configurations
     initialize_view_by_name()
     for view_name in configuration.___view_names:
         try:
-            View = VIEW_BY_NAME[view_name]
+            View = view_by_name[view_name]
         except KeyError:
             raise CrossComputeConfigurationError(f'{view_name} not installed')
         environment_variable_ids = get_environment_variable_ids(
             View.environment_variable_definitions)
         if environment_variable_ids:
             L.debug('%s.environment_variable_ids = %s', view_name, list(
                 environment_variable_ids))
@@ -477,16 +467,16 @@
     automation_folder = configuration.folder
     for step_name in STEP_NAMES:
         step_configuration = get_dictionary(configuration, step_name)
         template_definitions = [TemplateDefinition(
             _, automation_folder=automation_folder, step_name=step_name,
         ) for _ in get_dictionaries(step_configuration, 'templates')]
         assert_unique_values([
-            _.id for _ in template_definitions],
-            f'duplicate template id {{x}} in {step_name}')
+            _.path for _ in template_definitions
+        ], f'duplicate template path {{x}} in {step_name}')
         template_definitions_by_step_name[step_name] = template_definitions
     return {
         'template_definitions_by_step_name': template_definitions_by_step_name}
 
 
 def validate_batches(configuration):
     batch_definitions = []
@@ -511,29 +501,30 @@
 def validate_environment(configuration):
     d = get_dictionary(configuration, 'environment')
     port_definitions = get_port_definitions(
         d, configuration.get_variable_definitions('log')
         + configuration.get_variable_definitions('debug'))
     environment_variable_ids = get_environment_variable_ids(get_dictionaries(
         d, 'variables'))
-    batch_concurrency_name = d.get('batch', 'process').lower()
+    batch_concurrency_name = d.get('batch', 'thread').lower()
     if batch_concurrency_name not in ('process', 'thread', 'single'):
         raise CrossComputeConfigurationError(
             f'"{batch_concurrency_name}" batch concurrency is not supported')
-    interval_text = d.get('interval', '').strip()
-    interval_timedelta = get_interval_timedelta(interval_text)
+    interval_timedelta, is_interval_strict = get_interval_pack(d.get(
+        'interval', '').strip())
     return {
         'engine_name': get_engine_name(d),
         'parent_image_name': d.get('image', 'python').strip(),
         'package_definitions': [PackageDefinition(_) for _ in get_dictionaries(
             d, 'packages')],
         'port_definitions': port_definitions,
         'environment_variable_ids': environment_variable_ids,
         'batch_concurrency_name': batch_concurrency_name,
-        'interval_timedelta': interval_timedelta}
+        'interval_timedelta': interval_timedelta,
+        'is_interval_strict': is_interval_strict}
 
 
 def validate_datasets(configuration):
     automation_folder = configuration.folder
     dataset_definitions = [DatasetDefinition(
         _, automation_folder=automation_folder,
     ) for _ in get_dictionaries(configuration, 'datasets')]
@@ -581,15 +572,16 @@
     template_path_by_id = {}
     display_dictionary = get_dictionary(configuration, 'display')
     automation_folder = configuration.folder
     for raw_template_definition in get_dictionaries(
             display_dictionary, 'templates'):
         template_definition = TemplateDefinition(
             raw_template_definition, automation_folder=automation_folder)
-        template_id = template_definition.id
+        template_id = raw_template_definition.get(
+            'id', template_definition.path.stem)
         template_path_by_id[template_id] = template_definition.path
     return {'template_path_by_id': template_path_by_id}
 
 
 def validate_display_pages(configuration):
     display_dictionary = get_dictionary(configuration, 'display')
     page_definitions = [PageDefinition(_) for _ in get_dictionaries(
@@ -598,16 +590,23 @@
     return {'page_definition_by_id': page_definition_by_id}
 
 
 def validate_display_buttons(configuration):
     display_dictionary = get_dictionary(configuration, 'display')
     button_definitions = [ButtonDefinition(_) for _ in get_dictionaries(
         display_dictionary, 'buttons')]
-    button_definition_by_id = {_.id: _ for _ in button_definitions}
-    return {'button_definition_by_id': button_definition_by_id}
+    button_text_by_id = {}
+    for button_definition in button_definitions:
+        button_id = button_definition.id
+        button_text = button_definition.configuration.get(
+            'button-text', '').strip()
+        if not button_text:
+            continue
+        button_text_by_id[button_id] = button_text
+    return {'button_text_by_id': button_text_by_id}
 
 
 def validate_authorization(configuration):
     authorization_dictionary = get_dictionary(configuration, 'authorization')
     token_definitions = [TokenDefinition(
         _, automation_folder=configuration.folder,
     ) for _ in get_dictionaries(authorization_dictionary, 'tokens')]
@@ -619,60 +618,74 @@
         authorization_dictionary, 'groups')]
     group_definitions = child_group_definitions + parent_group_definitions
     return {
         'identities_by_token': identities_by_token,
         'group_definitions': group_definitions}
 
 
-def validate_prints(configuration):
-    print_definitions = [PrintDefinition(_) for _ in get_dictionaries(
-        configuration, 'prints')]
-    return {'print_definitions': print_definitions}
-
-
 def validate_template_identifiers(template_dictionary):
     try:
         template_path = template_dictionary['path']
     except KeyError as e:
         raise CrossComputeConfigurationError(f'{e} required for each template')
     automation_folder = template_dictionary.automation_folder
     template_path = Path(template_path)
     if not (automation_folder / template_path).exists():
         raise CrossComputeConfigurationError(
             f'could not find template {template_path}')
     return {
-        'id': template_dictionary.get('id', template_path.stem),
-        'path': template_path}
+        'path': template_path,
+        'expression': template_dictionary.get('expression', '')}
 
 
 def validate_variable_identifiers(variable_dictionary):
     try:
         variable_id = variable_dictionary['id']
         view_name = variable_dictionary['view']
         variable_path = variable_dictionary['path']
     except KeyError as e:
         raise CrossComputeConfigurationError(f'{e} required for each variable')
     if not VARIABLE_ID_PATTERN.match(variable_id):
         raise CrossComputeConfigurationError(
             f'{variable_id} is not a valid variable id; please use only '
             'lowercase, uppercase, numbers, hyphens, underscores and spaces')
+    if variable_dictionary.step_name == 'print':
+        if view_name in ['link']:
+            pass
+        elif view_name not in PRINTER_NAMES:
+            raise CrossComputeConfigurationError(
+                f'{view_name} is not a supported printer')
+        elif view_name not in printer_by_name:
+            raise CrossComputeConfigurationError(
+                f'pip install crosscompute-printers-{view_name}')
     if relpath(variable_path).startswith('..'):
         raise CrossComputeConfigurationError(
             f'path {variable_path} for variable {variable_id} must be within '
             'the folder')
+    label = variable_dictionary.get('label', format_name(variable_id)).strip()
     return {
         'id': variable_id,
         'view_name': view_name,
-        'path': Path(variable_path)}
+        'path': Path(variable_path),
+        'label': label}
 
 
 def validate_variable_configuration(variable_dictionary):
-    variable_configuration = get_dictionary(
+    # TODO: Validate variable view configurations
+    c = get_dictionary(
         variable_dictionary, 'configuration')
-    return {'configuration': variable_configuration}
+    if variable_dictionary.step_name == 'print':
+        variable_id = variable_dictionary.id
+        view_name = variable_dictionary.view_name
+        if view_name == 'link':
+            pass
+        else:
+            process_header_footer_options(variable_id, c)
+            process_page_number_options(variable_id, c)
+    return {'configuration': c}
 
 
 def validate_batch_identifiers(batch_dictionary):
     is_run = batch_dictionary.is_run
     try:
         folder = get_scalar_text(batch_dictionary, 'folder')
     except KeyError as e:
@@ -690,32 +703,28 @@
         except CrossComputeConfigurationError as e:
             batch_configuration = get_dictionary(
                 batch_dictionary, 'configuration')
             if 'path' in batch_configuration:
                 e.path = batch_configuration['path']
             raise
     d = {'folder': Path(folder), 'name': name, 'slug': slug}
-    if data_by_id:
-        for k, v in d.items():
-            if k in batch_dictionary:
-                batch_dictionary[k] = v
     if data_by_id is not None:
         if not is_run:
-            slug = format_slug(slug)
-        uri = BATCH_ROUTE.format(batch_slug=slug)
-        d.update({'slug': slug, 'uri': uri})
+            d['slug'] = slug = format_slug(slug)
+        d['uri'] = BATCH_ROUTE.format(batch_slug=slug)
     return d
 
 
 def validate_batch_configuration(batch_dictionary):
     batch_reference = get_dictionary(batch_dictionary, 'reference')
     batch_configuration = get_dictionary(batch_dictionary, 'configuration')
     return {
         'reference': batch_reference,
-        'configuration': batch_configuration}
+        'configuration': batch_configuration,
+        'clock': Clock()}
 
 
 def validate_dataset_identifiers(dataset_dictionary):
     return {'path': get_folder_plus_path(dataset_dictionary)}
 
 
 def validate_dataset_reference(dataset_dictionary):
@@ -739,33 +748,39 @@
                 'refusing to overwrite existing dataset; please delete '
                 f'{target_path} from the disk as defined')
     return {'reference': dataset_reference}
 
 
 def validate_script_identifiers(script_dictionary):
     folder = script_dictionary.get('folder', '.').strip()
+    method_count = 0
+
+    if 'command' in script_dictionary:
+        command = script_dictionary['command'].strip()
+        method_count += 1
+    else:
+        command = None
 
     if 'path' in script_dictionary:
         path = Path(script_dictionary['path'].strip())
         suffix = path.suffix
         if suffix not in ['.ipynb', '.py']:
             raise CrossComputeConfigurationError(
                 f'{suffix} not supported for script path')
+        method_count += 1
     else:
         path = None
 
-    if 'command' in script_dictionary:
-        command = script_dictionary['command'].strip()
-    else:
-        command = None
+    if 'function' in script_dictionary:
+        method_count += 1
 
-    return {
-        'folder': Path(folder),
-        'path': path,
-        'command': command}
+    if method_count > 1:
+        raise CrossComputeConfigurationError(
+            'set script command or path or function')
+    return {'folder': Path(folder), 'command': command, 'path': path}
 
 
 def validate_package_identifiers(package_dictionary):
     try:
         package_id = package_dictionary['id']
         manager_name = package_dictionary['manager']
     except KeyError as e:
@@ -894,65 +909,14 @@
     permission_action = permission_dictionary.get('action', 'accept')
     if permission_action not in PERMISSION_ACTIONS:
         raise CrossComputeConfigurationError(
             f'"{permission_action}" action not supported')
     return {'id': permission_id, 'action': permission_action}
 
 
-def validate_print_identifiers(print_dictionary):
-    initialize_printer_by_name()
-    print_format = print_dictionary.get('format', '').strip()
-    if print_format:
-        try:
-            PRINTER_BY_NAME[print_format]
-        except KeyError:
-            printer_names = PRINTER_BY_NAME.keys()
-            if printer_names:
-                extra_message = 'try ' + ' '.join(printer_names)
-            else:
-                extra_message = 'install crosscompute-printers-pdf'
-            raise CrossComputeConfigurationError(
-                f'{print_format} is not a supported printer; {extra_message}')
-    print_folder = Path(print_dictionary.get('folder', '')).expanduser()
-    print_name = print_dictionary.get('name', '')
-    return {
-        'format': print_format,
-        'folder': print_folder,
-        'name': print_name}
-
-
-def validate_print_configuration(print_dictionary):
-    print_configuration = get_dictionary(
-        print_dictionary, 'configuration')
-    return {'configuration': print_configuration}
-
-
-def validate_header_footer_options(print_dictionary):
-    print_configuration = print_dictionary.configuration
-    key = 'header-footer'
-    options = get_dictionary(print_configuration, key)
-    options['skip-first'] = bool(options.get('skip-first'))
-    return {}
-
-
-def validate_page_number_options(print_dictionary):
-    print_configuration = print_dictionary.configuration
-    key = 'page-number'
-    options = get_dictionary(print_configuration, key)
-    location = options.get('location')
-    if location and location not in ['header', 'footer']:
-        raise CrossComputeConfigurationError(
-            f'{location} location not supported for {key}')
-    alignment = options.get('alignment')
-    if alignment and alignment not in ['left', 'center', 'right']:
-        raise CrossComputeConfigurationError(
-            f'{alignment} alignment not supported for {key}')
-    return {}
-
-
 def get_configuration_format(path):
     file_extension = path.suffix
     try:
         configuration_format = {
             '.cfg': 'ini',
             '.ini': 'ini',
             '.toml': 'toml',
@@ -962,30 +926,14 @@
     except KeyError:
         raise CrossComputeConfigurationFormatError((
             f'{file_extension} format not supported for automation '
             'configuration').lstrip())
     return configuration_format
 
 
-def get_template_text(
-        template_definitions, automation_folder, variable_definitions):
-    template_texts = []
-    for template_definition in template_definitions:
-        path = automation_folder / template_definition.path
-        with open(path, 'rt') as f:
-            template_text = f.read().strip()
-        if not template_text:
-            continue
-        template_texts.append(template_text)
-    if not template_texts:
-        variable_ids = [_.id for _ in variable_definitions]
-        template_texts = ['\n'.join('{%s}' % _ for _ in variable_ids)]
-    return '\n'.join(template_texts)
-
-
 def get_engine_name(environment_dictionary):
     engine_name = environment_dictionary.get('engine', 'unsafe').strip()
     if engine_name == 'podman':
         if not shutil.which('podman'):
             L.warning('podman is not available on this machine')
     elif engine_name == 'unsafe':
         L.warning(
@@ -1028,33 +976,34 @@
         except KeyError:
             raise CrossComputeConfigurationError(
                 f'{variable_id} is missing in the environment as defined')
         variable_ids.add(variable_id)
     return variable_ids
 
 
-def get_interval_timedelta(interval_text):
+def get_interval_pack(interval_text):
     if not interval_text:
-        return
+        return None, None
     try:
-        count, name = interval_text.split()
+        count, name = interval_text.split(maxsplit=1)
         count = int(count)
     except ValueError:
         raise CrossComputeConfigurationError(
             f'unparseable interval "{interval_text}"; '
             f'expected something like "30 minutes"')
     for unit_name in INTERVAL_UNIT_NAMES:
         if name.startswith(unit_name[:-1]):
             break
     else:
         unit_names_text = ' '.join(INTERVAL_UNIT_NAMES)
         raise CrossComputeConfigurationError(
             f'unsupported interval unit "{name}" in "{interval_text}"; '
             f'expected {unit_names_text}')
-    return timedelta(**{unit_name: count})
+    is_strict = True if '!' in name else False
+    return timedelta(**{unit_name: count}), is_strict
 
 
 def get_scalar_text(d, key, default=None):
     value = d.get(key) or default
     if value is None:
         raise KeyError(key)
     if isinstance(value, dict):
@@ -1100,14 +1049,35 @@
     return batch_definitions
 
 
 def make_automation_name(automation_index):
     return AUTOMATION_NAME.replace('X', str(automation_index))
 
 
+def process_header_footer_options(variable_id, print_configuration):
+    k = 'header-footer'
+    d = get_dictionary(print_configuration, k)
+    d['skip-first'] = bool(d.get('skip-first'))
+
+
+def process_page_number_options(variable_id, print_configuration):
+    k = 'page-number'
+    d = get_dictionary(print_configuration, k)
+    location = d.get('location')
+    if location and location not in ['header', 'footer']:
+        raise CrossComputeConfigurationError(
+            f'print variable {variable_id} configuration {k} '
+            f'location {location} not supported')
+    alignment = d.get('alignment')
+    if alignment and alignment not in ['left', 'center', 'right']:
+        raise CrossComputeConfigurationError(
+            f'print variable {variable_id} configuration {k} '
+            f'alignment {alignment} not supported')
+
+
 def get_folder_plus_path(d):
     folder = d.get('folder', '').strip()
     path = d.get('path', '').strip()
     if not folder and not path:
         return
     return Path(folder, path)
 
@@ -1137,26 +1107,29 @@
 def assert_unique_values(xs, message):
     for x, count in Counter(xs).items():
         if count > 1:
             raise CrossComputeConfigurationError(message.format(x=x))
 
 
 RUN_PY = Template('''\
-import inspect
+from inspect import signature
 from os import getenv
 from pathlib import Path
 
 import $module_name
 
 
 folder_by_name = {}
 for x in 'input_folder', 'output_folder', 'log_folder', 'debug_folder':
     folder_by_name[x] = Path(getenv('CROSSCOMPUTE_' + x.upper()))
+function_signature = signature($function_string)
 d = {}
-for x in inspect.getargspec($function_string).args:
+for x in function_signature.parameters:
+    if x not in folder_by_name:
+        continue
     d[x] = folder_by_name[x]
 $function_string(**d)''')
 
 
 PERMISSION_IDS = [
     'add_token',
     'see_root',
```

### Comparing `crosscompute-0.9.3.3/crosscompute/routines/database.py` & `crosscompute-0.9.4.2/crosscompute/routines/printer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,173 +1,149 @@
-from logging import getLogger
-from pathlib import Path
-from time import time
-
-from invisibleroads_macros_disk import is_path_in_folder
-
-from ..constants import (
-    BATCH_ROUTE,
-    STEP_CODE_BY_NAME,
-    STEP_ROUTE)
-
-
-class DiskDatabase():
-
-    def __init__(self, configuration, changes):
-        self._configuration = configuration
-        self._changes = changes
-        self._memory = learn(configuration)
-
-    def grok(self, paths):
-        changed_infos = []
-        variable_ids = []
-        for path in paths:
-            path = Path(path).resolve()
-            if path.is_dir():
+import json
+from collections import defaultdict
+from importlib_metadata import entry_points
+from os import symlink
+
+from invisibleroads_macros_disk import remove_path
+from invisibleroads_macros_log import get_timestamp, LONGSTAMP_TEMPLATE
+
+from crosscompute.macros.package import import_attribute
+from crosscompute.routines.variable import (
+    format_text,
+    get_data_by_id)
+from crosscompute.settings import printer_by_name
+
+
+class BatchPrinter:
+
+    view_name = None
+
+    def __init__(self, server_uri, is_draft):
+        self.server_uri = server_uri
+        self.is_draft = is_draft
+        self.reset()
+
+    def reset(self):
+        self._packs_by_view_name = defaultdict(list)
+        self._pack_by_path = {}
+        self._link_packs = []
+        self._timestamp = get_timestamp(template=LONGSTAMP_TEMPLATE)
+
+    def add(self, automation_definition, batch_definitions):
+        packs_by_view_name = self._packs_by_view_name
+        batch_dictionaries = self._get_batch_dictionaries(
+            automation_definition, batch_definitions)
+        print_configurations_by_view_name = defaultdict(list)
+        print_definitions = automation_definition.get_variable_definitions(
+            'print')
+        this_view_name = self.view_name
+        for print_definition in print_definitions:
+            view_name = print_definition.view_name
+            if this_view_name and this_view_name != view_name:
                 continue
-            try:
-                infos = self._get(path)
-            except KeyError:
+            if view_name not in printer_by_name:
                 continue
-            for info in infos:
-                if info['code'] == 'v':
-                    variable_id = info['id']
-                    if info['id'] in variable_ids:
-                        continue
-                    variable_ids.append(variable_id)
-                changed_infos.append(info)
-        if changed_infos:
-            self._changes[time()] = changed_infos
-        return changed_infos
-
-    def _get(self, path):
-        configuration = self._configuration
-        for automation_definition in configuration.automation_definitions:
-            automation_folder = automation_definition.folder
-            runs_folder = automation_folder / 'runs'
-            if not is_path_in_folder(path, runs_folder):
-                continue
-            run_id = path.relative_to(runs_folder).parts[0]
-            batch_uri = BATCH_ROUTE.format(batch_slug=run_id)
-            memory = DiskMemory()
-            add_variable_infos_from_folder(
-                memory, automation_definition, runs_folder / run_id, batch_uri)
-            infos = memory.get(path)
-            break
-        else:
-            infos = self._memory.get(path)
-        return infos
-
-
-class DiskMemory():
-
-    def __init__(self):
-        self._d = {}
-
-    def add(self, path, info):
-        path = Path(path).resolve()
-        if path not in self._d:
-            self._d[path] = []
-        self._d[path].append(info)
-
-    def get(self, path):
-        path = Path(path).resolve()
-        return self._d[path]
-
-
-def learn(configuration):
-    'Get c = configuration, v = variable, t = template, s = style'
-    memory = DiskMemory()
-    add_configuration_infos(memory, configuration)
-    add_variable_infos(memory, configuration)
-    add_template_infos(memory, configuration)
-    add_style_infos(memory, configuration)
-    return memory
-
-
-def add_configuration_infos(memory, configuration):
-    info = {'code': 'c'}
-    # Get automation configuration paths
-    memory.add(configuration.path, info)
-    for import_configuration in configuration.import_configurations:
-        memory.add(import_configuration['path'], info)
-    # Get batch configuration paths
-    for automation_definition in configuration.automation_definitions:
-        automation_folder = automation_definition.folder
-        # Use raw batch definitions
-        raw_batch_definitions = automation_definition.get('batches', [])
-        for raw_batch_definition in raw_batch_definitions:
-            batch_configuration = raw_batch_definition.get('configuration', {})
-            if 'path' not in batch_configuration:
-                continue
-            memory.add(automation_folder / batch_configuration['path'], info)
-
-
-def add_variable_infos(memory, configuration):
-    for automation_definition in configuration.automation_definitions:
-        automation_folder = automation_definition.folder
-        # Use computed batch definitions
-        for batch_definition in automation_definition.batch_definitions:
-            add_variable_infos_from_folder(
-                memory,
-                automation_definition,
-                automation_folder / batch_definition.folder,
-                batch_definition.uri)
-
-
-def add_variable_infos_from_folder(
-        memory, automation_definition, absolute_batch_folder, batch_uri):
-    info = {'code': 'v'}
-    automation_uri = automation_definition.uri
-    uri = automation_uri + batch_uri
-    d = automation_definition.variable_definitions_by_step_name
-    for step_name, variable_definitions in d.items():
-        step_code = STEP_CODE_BY_NAME[step_name]
-        step_uri = STEP_ROUTE.format(step_code=step_code)
-        folder = absolute_batch_folder / step_name
-        for variable_definition in variable_definitions:
-            variable_id = variable_definition.id
-            if variable_id != 'return_code':
-                info_uri = uri + step_uri
-            else:
-                info_uri = uri
-            variable_info = info | {'id': variable_id, 'uri': info_uri}
-            variable_configuration = variable_definition.configuration
-            if 'path' in variable_configuration:
-                path = folder / variable_configuration['path']
-                memory.add(path, variable_info)
-            path = folder / variable_definition.path
-            memory.add(path, variable_info)
-
-
-def add_template_infos(memory, configuration):
-    info = {'code': 't'}
-    for automation_definition in configuration.automation_definitions:
+            print_configuration = print_definition.configuration
+            print_configurations_by_view_name[view_name].append(
+                print_configuration)
+        for (
+            view_name,
+            print_configurations,
+        ) in print_configurations_by_view_name.items():
+            packs_by_view_name[view_name].append((
+                batch_dictionaries, print_configurations))
+
+    def run(self):
+        is_draft = self.is_draft
+        if is_draft:
+            for draft_path in self._pack_by_path:
+                if draft_path.is_symlink():
+                    remove_path(draft_path)
+        for view_name, packs in self._packs_by_view_name.items():
+            Printer = printer_by_name[view_name]
+            printer = Printer(self.server_uri, is_draft)
+            for batch_dictionaries, print_configurations in packs:
+                printer.render(batch_dictionaries, print_configurations)
+        self._save_link_configurations()
+        self.reset()
+
+    def _get_batch_dictionaries(
+            self, automation_definition, batch_definitions):
+        batch_dictionaries = []
         automation_folder = automation_definition.folder
         automation_uri = automation_definition.uri
-        template_info = info | {'uri': automation_uri}
-        d = automation_definition.template_definitions_by_step_name
-        for step_name, template_definitions in d.items():
-            for template_definition in template_definitions:
-                if 'path' not in template_definition:
-                    continue
-                path = automation_folder / template_definition.path
-                memory.add(path, template_info)
-        d = automation_definition.template_path_by_id
-        for template_id, template_path in d.items():
-            path = automation_folder / template_path
-            memory.add(path, template_info)
-
-
-def add_style_infos(memory, configuration):
-    info = {'code': 's'}
-    automation_definitions = configuration.automation_definitions
-    for automation_definition in automation_definitions:
-        automation_folder = automation_definition.folder
-        for style_definition in automation_definition.style_definitions:
-            if 'path' not in style_definition:
+        is_draft, pack_by_path = self.is_draft, self._pack_by_path
+        link_packs, timestamp = self._link_packs, self._timestamp
+        extra_data_by_id = {'timestamp': {'value': timestamp}}
+        print_folder = automation_folder / 'prints' / timestamp
+        for print_definition in automation_definition.get_variable_definitions(
+                'print'):
+            view_name = print_definition.view_name
+            variable_path = print_definition.path
+            for batch_definition in batch_definitions:
+                batch_folder = batch_definition.folder
+                batch_uri = batch_definition.uri
+                draft_folder = automation_folder / batch_folder / 'print'
+                if view_name in printer_by_name:
+                    draft_path = draft_folder / variable_path
+                    print_name = _format_print_name(
+                        automation_definition, batch_definition,
+                        print_definition, extra_data_by_id)
+                    print_path = print_folder / print_name
+                    batch_dictionaries.append({
+                        'path': str(draft_path if is_draft else print_path),
+                        'uri': automation_uri + batch_uri})
+                    pack_by_path[draft_path] = print_folder, print_name
+                elif view_name == 'link':
+                    link_packs.append((draft_folder, print_definition))
+        return batch_dictionaries
+
+    def _save_link_configurations(self):
+        pack_by_path = self._pack_by_path
+        if not self.is_draft:
+            for draft_path, (
+                print_folder, print_name,
+            ) in pack_by_path.items():
+                symlink(print_folder / print_name, remove_path(draft_path))
+        for (
+            draft_folder, variable_definition,
+        ) in self._link_packs:
+            variable_configuration = variable_definition.configuration
+            if 'path' not in variable_configuration:
                 continue
-            path = automation_folder / style_definition['path']
-            memory.add(path, info)
-
-
-L = getLogger(__name__)
+            variable_path = variable_definition.path
+            draft_path = draft_folder / variable_path
+            print_name = pack_by_path[draft_path][1]
+            d = {}
+            if 'link-text' not in variable_configuration:
+                d['link-text'] = print_name
+            if 'file-name' not in variable_configuration:
+                d['file-name'] = print_name
+            with (
+                draft_folder / variable_configuration['path']
+            ).open('wt') as f:
+                json.dump(d, f)
+
+
+def initialize_printer_by_name():
+    for entry_point in entry_points().select(group='crosscompute.printers'):
+        printer_by_name[entry_point.name] = import_attribute(entry_point.value)
+    return printer_by_name
+
+
+def print_batch(automation_definition, batch_definition, server_uri, is_draft):
+    batch_printer = BatchPrinter(server_uri, is_draft)
+    batch_printer.add(automation_definition, [batch_definition])
+    batch_printer.run()
+
+
+def _format_print_name(
+        automation_definition, batch_definition, print_definition,
+        extra_data_by_id):
+    view_name = print_definition.view_name
+    variable_configuration = print_definition.configuration
+    batch_name = batch_definition.name
+    name_template = variable_configuration.get(
+        'name', '').strip() or f'{batch_name}.{view_name}'
+    data_by_id = get_data_by_id(
+        automation_definition, batch_definition) | extra_data_by_id
+    return format_text(name_template, data_by_id)
```

### Comparing `crosscompute-0.9.3.3/crosscompute/routines/interface.py` & `crosscompute-0.9.4.2/crosscompute/routines/interface.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.3.3/crosscompute/routines/log.py` & `crosscompute-0.9.4.2/crosscompute/routines/log.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.3.3/crosscompute/routines/server.py` & `crosscompute-0.9.4.2/crosscompute/routines/server.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,56 +7,72 @@
 from fastapi.exception_handlers import http_exception_handler
 from fastapi.middleware.cors import CORSMiddleware
 from fastapi.responses import PlainTextResponse
 from invisibleroads_macros_web.starlette import ExtraResponseHeadersMiddleware
 from starlette.exceptions import HTTPException as StarletteHTTPException
 from watchfiles import watch
 
-from ..constants import HOST, PORT, TEMPLATE_PATH_BY_ID
-from ..exceptions import CrossComputeError
-from ..routers import automation, mutation, root, token
+from ..constants import (
+    Info,
+    BUTTON_TEXT_BY_ID,
+    DISK_DEBOUNCE_IN_MILLISECONDS,
+    DISK_STEP_IN_MILLISECONDS,
+    HOST,
+    PORT,
+    TEMPLATE_PATH_BY_ID)
+from ..exceptions import (
+    CrossComputeError)
+from ..routers import (
+    automation,
+    file,
+    root,
+    stream,
+    token)
 from ..settings import (
-    StoppableProcess, site, template_environment, template_globals,
+    StoppableProcess,
+    button_text_by_id,
+    site,
+    template_environment,
+    template_globals,
     template_path_by_id)
-from .database import DiskDatabase
-from .interface import Server
+from .database import (
+    DiskDatabase,
+    PositiveFileFilter)
+from .interface import (
+    Server)
 
 
 class DiskServer(Server):
 
     def __init__(
-            self, environment, safe, queue, work, changes,
-            host=HOST, port=PORT, with_restart=True, with_prefix=True,
-            with_hidden=True, root_uri='', allowed_origins=None):
+            self, work, environment, safe,
+            uris, tasks, changes,
+            host=HOST, port=PORT, root_uri='', allowed_origins=None,
+            with_restart=True, with_prefix=True, with_hidden=True):
+        self._work = work
         self._environment = environment
         self._safe = safe
-        self._queue = queue
-        self._work = work
+        self._uris = uris
+        self._tasks = tasks
         self._changes = changes
         self._host = host
         self._port = port
+        self._root_uri = root_uri
+        self._allowed_origins = allowed_origins
         self._with_restart = with_restart
         self._with_prefix = with_prefix
         self._with_hidden = with_hidden
-        self._root_uri = root_uri
-        self._allowed_origins = allowed_origins
 
     def serve(self, configuration):
-        worker_process = StoppableProcess(
-            name='worker', target=self._work, args=(self._queue,))
-        worker_process.start()
-        host, port, root_uri, with_restart, with_prefix, allowed_origins = [
-            self._host, self._port, self._root_uri, self._with_restart,
-            self._with_prefix, self._allowed_origins]
-        self._refresh(configuration)
-        app = get_app(root_uri, with_prefix)
-        if with_restart:
-            app.add_middleware(
-                ExtraResponseHeadersMiddleware,
-                headers={'Cache-Control': 'no-store'})
+        host, port, root_uri, allowed_origins = [
+            self._host, self._port, self._root_uri, self._allowed_origins]
+        app = get_app(root_uri, self._with_prefix)
+        if self._with_restart:
+            app.add_middleware(ExtraResponseHeadersMiddleware, headers={
+                'Cache-Control': 'no-store'})
         if allowed_origins:
             app.add_middleware(
                 CORSMiddleware, allow_origins=allowed_origins,
                 allow_credentials=True, allow_methods=['*'],
                 allow_headers=['*'])
         L.info('serving at http://%s:%s%s', host, port, root_uri)
         try:
@@ -65,92 +81,105 @@
                 access_log=L.getEffectiveLevel() <= DEBUG)
         except AssertionError:
             L.error(f'could not start server at {host}:{port}')
         except KeyboardInterrupt:
             pass
         except Exception as e:
             L.exception(e)
-        finally:
-            worker_process.stop()
 
-    def watch(
-            self, configuration, disk_poll_in_milliseconds,
-            disk_debounce_in_milliseconds, reload):
-        server_process, disk_database = self._start(configuration)
+    def watch(self, configuration, reload):
+        s_process, w_process, d_database = self.start(configuration)
         try:
             for changed_packs in watch(
-                    configuration.folder, step=disk_poll_in_milliseconds,
-                    debounce=disk_debounce_in_milliseconds):
-                L.debug(changed_packs)
+                    configuration.folder,
+                    watch_filter=PositiveFileFilter(),
+                    debounce=DISK_DEBOUNCE_IN_MILLISECONDS,
+                    step=DISK_STEP_IN_MILLISECONDS):
                 changed_paths = [_[1] for _ in changed_packs]
-                changed_infos = disk_database.grok(changed_paths)
-                L.debug(changed_infos)
+                changed_infos = d_database.grok(changed_paths)
                 should_restart_server = False
                 for info in changed_infos:
-                    if info['code'] == 'c':
+                    if info['code'] == Info.CONFIGURATION:
                         should_restart_server = True
                 if self._with_restart and should_restart_server:
                     try:
                         configuration = reload()
                     except CrossComputeError as e:
                         L.error(e)
                         continue
-                    server_process.stop()
-                    server_process, disk_database = self._start(configuration)
+                    s_process.stop()
+                    w_process.stop()
+                    s_process, w_process, d_database = self.start(
+                        configuration)
         except KeyboardInterrupt:
             pass
         except Exception as e:
             L.exception(e)
         finally:
-            server_process.stop()
+            s_process.stop()
+            w_process.stop()
 
-    def _start(self, configuration):
+    def start(self, configuration):
+        self.refresh(configuration)
         server_process = StoppableProcess(
-            name='server', target=self.serve, args=(configuration,))
+            name='server', target=self.serve,
+            args=(configuration,))
         server_process.start()
-        disk_database = DiskDatabase(configuration, self._changes)
-        return server_process, disk_database
+        worker_process = StoppableProcess(
+            name='worker', target=self._work,
+            args=(
+                configuration.automation_definitions,
+                self._tasks,
+                self._uris,
+                self._changes,
+                self._environment,
+                f'http://127.0.0.1:{self._port}{self._root_uri}'),
+            kwargs={'with_rebuild': True})
+        worker_process.start()
+        disk_database = DiskDatabase(
+            configuration, self._changes, self._with_restart)
+        return server_process, worker_process, disk_database
 
-    def _refresh(self, configuration):
-        configuration_name = configuration.name
-        if configuration_name == 'Automation 0':
-            configuration_name = 'Automations'
-        configuration_folder = configuration.folder
-        root_uri, with_restart = self._root_uri, self._with_restart
+    def refresh(self, configuration):
+        name = configuration.name
         site.update({
-            'name': configuration_name,
+            'name': 'Automations' if name == 'Automation 0' else name,
             'configuration': configuration,
             'definitions': configuration.automation_definitions,
             'environment': self._environment,
             'safe': self._safe,
-            'queue': self._queue,
+            'uris': self._uris,
+            'tasks': self._tasks,
             'changes': self._changes,
             'with_prefix': self._with_prefix,
             'with_hidden': self._with_hidden})
         template_path_by_id.update(TEMPLATE_PATH_BY_ID)
         for template_id, path in configuration.template_path_by_id.items():
-            template_path_by_id[template_id] = str(configuration_folder / path)
+            template_path_by_id[template_id] = str(configuration.folder / path)
         template_globals.update({
             'base_template_path': template_path_by_id['base'],
             'live_template_path': template_path_by_id['live'],
             'google_analytics_id': getenv('GOOGLE_ANALYTICS_ID', ''),
-            'server_timestamp': time(),
-            'root_uri': root_uri,
-            'with_restart': with_restart})
-        template_environment.auto_reload = with_restart
+            'server_time': time(),
+            'root_uri': self._root_uri,
+            'with_restart': self._with_restart})
+        template_environment.auto_reload = self._with_restart
+        button_text_by_id.update(BUTTON_TEXT_BY_ID)
+        button_text_by_id.update(configuration.button_text_by_id)
 
 
 def get_app(root_uri, with_prefix):
     prefix = root_uri if with_prefix else ''
     app = FastAPI(root_path='' if with_prefix else root_uri)
     app.add_exception_handler(StarletteHTTPException, handle_http_exception)
     app.include_router(root.router, prefix=prefix)
     app.include_router(automation.router, prefix=prefix)
-    app.include_router(mutation.router, prefix=prefix)
+    app.include_router(file.router, prefix=prefix)
     app.include_router(token.router, prefix=prefix)
+    app.include_router(stream.router, prefix=prefix)
     return app
 
 
 async def handle_http_exception(request, e):
     if request.url.path.endswith('.json'):
         response = await http_exception_handler(request, e)
     else:
```

### Comparing `crosscompute-0.9.3.3/crosscompute/routines/variable.py` & `crosscompute-0.9.4.2/crosscompute/routines/variable.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,73 @@
 # TODO: Validate variable view configurations
 import csv
 import json
 import shutil
 from dataclasses import dataclass
 from logging import getLogger
+from os import symlink
 from urllib.request import urlretrieve as download_uri
 
 from importlib_metadata import entry_points
 from invisibleroads_macros_log import format_path
-from invisibleroads_macros_text import format_name, format_slug
+from invisibleroads_macros_text import format_slug
 from invisibleroads_macros_web.escape import (
     escape_quotes_html,
     escape_quotes_js)
 
 from ..constants import (
     CACHED_FILE_SIZE_LIMIT_IN_BYTES,
+    FILES_FOLDER,
+    FILES_ROUTE,
     MAXIMUM_FILE_CACHE_LENGTH,
-    VARIABLE_ID_TEMPLATE_PATTERN,
-    VIEW_BY_NAME)
+    VARIABLE_ID_TEMPLATE_PATTERN)
 from ..exceptions import (
     CrossComputeConfigurationError,
     CrossComputeConfigurationNotImplementedError,
     CrossComputeDataError)
 from ..macros.disk import FileCache
 from ..macros.iterable import find_item
 from ..macros.package import import_attribute
-from .asset import asset_storage
+from ..settings import (
+    template_globals,
+    view_by_name)
+from .asset import (
+    CHECKBOX_INPUT_HEADER_JS,
+    CHECKBOX_INPUT_HTML,
+    CHECKBOX_OUTPUT_HEADER_JS,
+    CHECKBOX_OUTPUT_JS,
+    FILE_INPUT_HEADER_JS,
+    FILE_INPUT_HTML,
+    FRAME_OUTPUT_HEADER_JS,
+    FRAME_OUTPUT_JS,
+    IMAGE_OUTPUT_HEADER_JS,
+    IMAGE_OUTPUT_JS,
+    JSON_OUTPUT_HEADER_JS,
+    JSON_OUTPUT_JS,
+    LINK_OUTPUT_HEADER_JS,
+    LINK_OUTPUT_JS,
+    MARKDOWN_OUTPUT_HEADER_JS,
+    MARKDOWN_OUTPUT_JS,
+    PDF_CSS,
+    PDF_OUTPUT_HEADER_JS,
+    PDF_OUTPUT_JS,
+    RADIO_INPUT_HTML,
+    RADIO_INPUT_HEADER_JS,
+    RADIO_OUTPUT_HEADER_JS,
+    RADIO_OUTPUT_JS,
+    STRING_INPUT_HEADER_JS,
+    STRING_INPUT_HTML,
+    STRING_OUTPUT_HEADER_JS,
+    STRING_OUTPUT_JS,
+    TABLE_OUTPUT_HEADER_JS,
+    TABLE_OUTPUT_JS,
+    TEXT_INPUT_HTML,
+    TEXT_INPUT_JS,
+    TEXT_OUTPUT_HEADER_JS,
+    TEXT_OUTPUT_JS)
 from .interface import Batch
 
 
 @dataclass(repr=False, eq=False, order=False, frozen=True)
 class Element():
 
     id: str
@@ -50,15 +88,15 @@
         self.variable_id = variable_definition.id
         self.variable_path = variable_definition.path
 
     @classmethod
     def get_from(Class, variable_definition):
         view_name = variable_definition.view_name
         try:
-            View = VIEW_BY_NAME[view_name]
+            View = view_by_name[view_name]
         except KeyError:
             L.error('%s view not installed', view_name)
             View = Class
         return View(variable_definition)
 
     def parse(self, data):
         return data
@@ -74,33 +112,35 @@
         page_dictionary = render(b, x)
         main_text = page_dictionary['main_text']
         if x.design_name != 'none':
             if main_text.endswith('</a>') or main_text.endswith('</span>'):
                 tag_name = 'span'
             else:
                 tag_name = 'div'
-            page_dictionary['main_text'] = '<%s class="_view">%s</%s>' % (
+            main_text = add_label_html(
+                main_text, self.variable_definition, x.id)
+            page_dictionary['main_text'] = '<%s class="_view">\n%s\n</%s>' % (
                 tag_name, main_text, tag_name)
         return page_dictionary
 
     def render_input(self, b: Batch, x: Element):
         return {
             'css_uris': [],
+            'css_texts': [],
             'js_uris': [],
-            'main_text': '',
             'js_texts': [],
-        }
+            'main_text': ''}
 
     def render_output(self, b: Batch, x: Element):
         return {
             'css_uris': [],
+            'css_texts': [],
             'js_uris': [],
-            'main_text': '',
             'js_texts': [],
-        }
+            'main_text': ''}
 
 
 class LinkView(VariableView):
 
     view_name = 'link'
 
     def render_output(self, b: Batch, x: Element):
@@ -112,36 +152,31 @@
         file_name = c.get('file-name', self.variable_path.name)
         link_text = c.get('link-text', file_name)
         main_text = (
             f'<a id="{element_id}" href="{data_uri}" '
             f'class="_{x.mode_name} _{self.view_name} {variable_id}" '
             f'download="{escape_quotes_html(file_name)}">'
             f'{link_text}</a>')
-        if x.design_name not in ['none']:
-            main_text = add_label_html(main_text, c, variable_id, element_id)
         js_texts = [
-            LINK_JS_HEADER,
-            LINK_JS_OUTPUT.substitute({
+            LINK_OUTPUT_HEADER_JS,
+            LINK_OUTPUT_JS.substitute({
                 'variable_id': variable_id,
                 'element_id': element_id,
-                'link_text': escape_quotes_js(link_text),
-            }),
-        ]
+                'link_text': escape_quotes_js(link_text)})]
         return {
-            'css_uris': [], 'js_uris': [], 'main_text': main_text,
-            'js_texts': js_texts}
+            'css_uris': [], 'css_texts': [], 'js_uris': [],
+            'js_texts': js_texts, 'main_text': main_text}
 
 
 class StringView(VariableView):
 
     view_name = 'string'
     input_type = 'text'
     function_by_name = {
-        'title': str.title,
-    }
+        'title': str.title}
 
     def get_value(self, b: Batch, x: Element):
         variable_definition = self.variable_definition
         data = b.load_data_from(x.request_params, variable_definition)
         if 'value' in data:
             value = data['value']
         elif 'path' in data:
@@ -153,59 +188,52 @@
     def render_input(self, b: Batch, x: Element):
         variable_definition = self.variable_definition
         variable_id = self.variable_id
         view_name = self.view_name
         element_id = x.id
         value = self.get_value(b, x)
         c = b.get_variable_configuration(variable_definition)
-        main_text = STRING_HTML_INPUT.render({
+        main_text = STRING_INPUT_HTML.render({
             'element_id': element_id,
             'mode_name': x.mode_name,
             'view_name': view_name,
             'variable_id': variable_id,
             'value': escape_quotes_html(value),
             'input_type': self.input_type,
-            'suggestions': c.get('suggestions', []),
-        })
-        if x.design_name not in ['none']:
-            main_text = add_label_html(main_text, c, variable_id, element_id)
+            'suggestions': c.get('suggestions', [])})
         js_texts = [
-            STRING_JS_INPUT.substitute({'view_name': view_name}),
-        ]
+            STRING_INPUT_HEADER_JS.substitute({'view_name': view_name})]
         return {
-            'css_uris': [], 'js_uris': [], 'main_text': main_text,
-            'js_texts': js_texts}
+            'css_uris': [], 'css_texts': [], 'js_uris': [],
+            'main_text': main_text, 'js_texts': js_texts}
 
     def render_output(self, b: Batch, x: Element):
         value = self.get_value(b, x)
         try:
             value = apply_functions(
                 value, x.function_names, self.function_by_name)
         except KeyError as e:
             L.error('%s function not supported for %s', e, self.view_name)
         variable_definition = self.variable_definition
         variable_id = self.variable_id
         element_id = x.id
         data_uri = b.get_data_uri(variable_definition, x)
-        c = b.get_variable_configuration(variable_definition)
         main_text = (
             f'<span id="{x.id}" '
             f'class="_{x.mode_name} _{self.view_name} {self.variable_id}">'
             f'{value}</span>')
-        if x.design_name not in ['none']:
-            main_text = add_label_html(main_text, c, variable_id, element_id)
         js_texts = [
-            STRING_JS_HEADER,
-            STRING_JS_OUTPUT.substitute({
+            STRING_OUTPUT_HEADER_JS,
+            STRING_OUTPUT_JS.substitute({
                 'variable_id': variable_id,
                 'element_id': element_id,
                 'data_uri': data_uri})]
         return {
-            'css_uris': [], 'js_uris': [], 'main_text': main_text,
-            'js_texts': js_texts}
+            'css_uris': [], 'css_texts': [], 'js_uris': [],
+            'js_texts': js_texts, 'main_text': main_text}
 
 
 class NumberView(StringView):
 
     view_name = 'number'
     input_type = 'number'
 
@@ -238,274 +266,302 @@
     def render_input(self, b: Batch, x: Element):
         variable_definition = self.variable_definition
         data = get_data_from(x.request_params, variable_definition)
         value = data.get('value', '')
         variable_id = self.variable_id
         view_name = self.view_name
         element_id = x.id
-        c = b.get_variable_configuration(variable_definition)
-        main_text = TEXT_HTML_INPUT.substitute({
+        main_text = TEXT_INPUT_HTML.substitute({
             'element_id': element_id,
             'mode_name': x.mode_name,
             'view_name': view_name,
             'variable_id': variable_id,
             'attribute_string': '' if value else ' disabled',
             'value': value})
-        if x.design_name not in ['none']:
-            main_text = add_label_html(main_text, c, variable_id, element_id)
         js_texts = [
-            STRING_JS_HEADER,
-            STRING_JS_INPUT.substitute({'view_name': view_name})]
+            STRING_OUTPUT_HEADER_JS,
+            STRING_INPUT_HEADER_JS.substitute({'view_name': view_name})]
         if not value:
             js_texts.extend([
-                TEXT_JS_HEADER,
-                TEXT_JS_INPUT.substitute({
+                TEXT_OUTPUT_HEADER_JS,
+                TEXT_INPUT_JS.substitute({
                     'element_id': element_id,
                     'data_uri': b.get_data_uri(variable_definition, x)})])
         return {
-            'css_uris': [], 'js_uris': [], 'main_text': main_text,
-            'js_texts': js_texts}
+            'css_uris': [], 'css_texts': [], 'js_uris': [],
+            'main_text': main_text, 'js_texts': js_texts}
 
     def render_output(self, b: Batch, x: Element):
         variable_definition = self.variable_definition
         variable_id = self.variable_id
         element_id = x.id
         data_uri = b.get_data_uri(variable_definition, x)
-        c = b.get_variable_configuration(variable_definition)
         main_text = (
             f'<span id="{x.id}" '
             f'class="_{x.mode_name} _{self.view_name} {self.variable_id}">'
             '</span>')
-        if x.design_name not in ['none']:
-            main_text = add_label_html(main_text, c, variable_id, element_id)
         js_texts = [
-            STRING_JS_HEADER,
-            TEXT_JS_HEADER,
-            TEXT_JS_OUTPUT.substitute({
+            STRING_OUTPUT_HEADER_JS,
+            TEXT_OUTPUT_HEADER_JS,
+            TEXT_OUTPUT_JS.substitute({
                 'variable_id': variable_id,
                 'element_id': element_id,
                 'data_uri': data_uri})]
         return {
-            'css_uris': [], 'js_uris': [], 'main_text': main_text,
-            'js_texts': js_texts}
+            'css_uris': [], 'css_texts': [], 'js_uris': [],
+            'js_texts': js_texts, 'main_text': main_text}
 
 
 class MarkdownView(TextView):
 
     view_name = 'markdown'
-    js_uris = [
-        'https://cdn.jsdelivr.net/npm/marked/marked.min.js',
-    ]
+    js_uris = ['https://cdn.jsdelivr.net/npm/marked/marked.min.js']
 
     def render_output(self, b: Batch, x: Element):
         variable_definition = self.variable_definition
         variable_id = self.variable_id
         element_id = x.id
         data_uri = b.get_data_uri(variable_definition, x)
-        c = b.get_variable_configuration(variable_definition)
         main_text = (
             f'<span id="{x.id}" '
             f'class="_{x.mode_name} _{self.view_name} {self.variable_id}">'
             '</span>')
-        if x.design_name not in ['none']:
-            main_text = add_label_html(main_text, c, variable_id, element_id)
         js_texts = [
-            STRING_JS_HEADER,
-            MARKDOWN_JS_HEADER,
-            MARKDOWN_JS_OUTPUT.substitute({
+            STRING_OUTPUT_HEADER_JS,
+            MARKDOWN_OUTPUT_HEADER_JS,
+            MARKDOWN_OUTPUT_JS.substitute({
                 'variable_id': variable_id,
                 'element_id': element_id,
                 'data_uri': data_uri})]
         return {
-            'css_uris': [], 'js_uris': self.js_uris, 'main_text': main_text,
-            'js_texts': js_texts}
+            'css_uris': [], 'css_texts': [], 'js_uris': self.js_uris,
+            'js_texts': js_texts, 'main_text': main_text}
 
 
 class ImageView(VariableView):
 
     view_name = 'image'
 
     def render_output(self, b: Batch, x: Element):
         variable_definition = self.variable_definition
         variable_id = self.variable_id
         element_id = x.id
         data_uri = b.get_data_uri(variable_definition, x)
-        c = b.get_variable_configuration(variable_definition)
         main_text = (
             f'<img id="{x.id}" '
             f'class="_{x.mode_name} _{self.view_name} {variable_id}" '
             f'src="{data_uri}" alt="">')
         # TODO: Show spinner on error
-        if x.design_name not in ['none']:
-            main_text = add_label_html(main_text, c, variable_id, element_id)
         js_texts = [
-            IMAGE_JS_HEADER,
-            IMAGE_JS_OUTPUT.substitute({
+            IMAGE_OUTPUT_HEADER_JS,
+            IMAGE_OUTPUT_JS.substitute({
                 'variable_id': variable_id,
                 'element_id': element_id,
                 'data_uri': data_uri})]
         return {
-            'css_uris': [], 'js_uris': [], 'main_text': main_text,
-            'js_texts': js_texts}
+            'css_uris': [], 'css_texts': [], 'js_uris': [],
+            'js_texts': js_texts, 'main_text': main_text}
 
 
 class RadioView(VariableView):
 
     view_name = 'radio'
 
     def render_input(self, b: Batch, x: Element):
         variable_definition = self.variable_definition
         variable_id = self.variable_id
         view_name = self.view_name
         element_id = x.id
         c = b.get_variable_configuration(variable_definition)
         data = b.load_data_from(x.request_params, variable_definition)
         value = data.get('value', '')
-        main_text = RADIO_HTML_INPUT.render({
+        main_text = RADIO_INPUT_HTML.render({
             'element_id': element_id,
             'mode_name': x.mode_name,
             'view_name': view_name,
             'variable_id': variable_id,
             'options': get_configuration_options(c, [value]),
             'value': value})
-        if x.design_name not in ['none']:
-            main_text = add_label_html(main_text, c, variable_id, element_id)
         js_texts = [
-            RADIO_JS_INPUT.substitute({'view_name': view_name})]
+            RADIO_INPUT_HEADER_JS.substitute({'view_name': view_name})]
         if variable_definition.step_name != 'input':
             data_uri = b.get_data_uri(variable_definition, x)
             js_texts.extend([
-                RADIO_JS_HEADER,
-                RADIO_JS_OUTPUT.substitute({
+                RADIO_OUTPUT_HEADER_JS,
+                RADIO_OUTPUT_JS.substitute({
                     'variable_id': variable_id, 'element_id': element_id,
                     'data_uri': data_uri})])
         return {
-            'css_uris': [], 'js_uris': [], 'main_text': main_text,
-            'js_texts': js_texts}
+            'css_uris': [], 'css_texts': [], 'js_uris': [],
+            'main_text': main_text, 'js_texts': js_texts}
 
 
 class CheckboxView(VariableView):
 
     view_name = 'checkbox'
 
     def render_input(self, b: Batch, x: Element):
         element_id = x.id
         view_name = self.view_name
         variable_id = self.variable_id
         variable_definition = self.variable_definition
         c = b.get_variable_configuration(variable_definition)
         data = b.load_data_from(x.request_params, variable_definition)
         values = data.get('value', '').splitlines()
-        main_text = CHECKBOX_HTML_INPUT.render({
+        main_text = CHECKBOX_INPUT_HTML.render({
             'element_id': element_id,
             'mode_name': x.mode_name,
             'view_name': view_name,
             'variable_id': variable_id,
             'options': get_configuration_options(c, values),
             'values': values})
-        if x.design_name not in ['none']:
-            main_text = add_label_html(main_text, c, variable_id, element_id)
         js_texts = [
-            CHECKBOX_JS_INPUT.substitute({'view_name': view_name})]
+            CHECKBOX_INPUT_HEADER_JS.substitute({'view_name': view_name})]
         if variable_definition.step_name != 'input':
             data_uri = b.get_data_uri(variable_definition, x)
             js_texts.extend([
-                CHECKBOX_JS_HEADER,
-                CHECKBOX_JS_OUTPUT.substitute({
+                CHECKBOX_OUTPUT_HEADER_JS,
+                CHECKBOX_OUTPUT_JS.substitute({
                     'variable_id': variable_id,
                     'element_id': element_id,
                     'data_uri': data_uri})])
         return {
-            'css_uris': [], 'js_uris': [], 'main_text': main_text,
-            'js_texts': js_texts}
+            'css_uris': [], 'css_texts': [], 'js_uris': [],
+            'main_text': main_text, 'js_texts': js_texts}
 
 
 class TableView(VariableView):
 
     view_name = 'table'
 
     def render_output(self, b: Batch, x: Element):
         variable_definition = self.variable_definition
         variable_id = self.variable_id
         element_id = x.id
         data_uri = b.get_data_uri(variable_definition, x)
-        c = b.get_variable_configuration(variable_definition)
         main_text = (
             f'<table id="{element_id}" '
             f'class="_{x.mode_name} _{self.view_name} {variable_id}">'
             '<thead/><tbody/></table>')
-        if x.design_name not in ['none']:
-            main_text = add_label_html(main_text, c, variable_id, element_id)
         js_texts = [
-            TABLE_JS_HEADER,
-            TABLE_JS_OUTPUT.substitute({
+            TABLE_OUTPUT_HEADER_JS,
+            TABLE_OUTPUT_JS.substitute({
                 'variable_id': variable_id,
                 'element_id': element_id,
                 'data_uri': data_uri})]
         return {
-            'css_uris': [], 'js_uris': [], 'main_text': main_text,
-            'js_texts': js_texts}
+            'css_uris': [], 'css_texts': [], 'js_uris': [],
+            'js_texts': js_texts, 'main_text': main_text}
 
 
 class FrameView(VariableView):
 
     view_name = 'frame'
 
     def render_output(self, b: Batch, x: Element):
         variable_definition = self.variable_definition
         variable_id = self.variable_id
         element_id = x.id
         data_uri = b.get_data_uri(variable_definition, x)
-        c = b.get_variable_configuration(variable_definition)
         data = b.load_data(variable_definition)
         if 'value' in data:
             value = data['value']
         else:
             value = ''
         main_text = (
             f'<iframe id="{element_id}" '
             f'class="_{x.mode_name} _{self.view_name} {variable_id}" '
             f'src="{escape_quotes_html(value)}" frameborder="0">'
             '</iframe>')
-        if x.design_name not in ['none']:
-            main_text = add_label_html(main_text, c, variable_id, element_id)
-
         js_texts = [
-            FRAME_JS_HEADER,
-            FRAME_JS_OUTPUT.substitute({
+            FRAME_OUTPUT_HEADER_JS,
+            FRAME_OUTPUT_JS.substitute({
                 'variable_id': variable_id,
                 'element_id': element_id,
                 'data_uri': data_uri})]
         return {
-            'css_uris': [], 'js_uris': [], 'main_text': main_text,
-            'js_texts': js_texts}
+            'css_uris': [], 'css_texts': [], 'js_uris': [],
+            'js_texts': js_texts, 'main_text': main_text}
 
 
 class JsonView(VariableView):
 
     view_name = 'json'
 
     def render_output(self, b: Batch, x: Element):
         variable_definition = self.variable_definition
         variable_id = self.variable_id
         data_uri = b.get_data_uri(variable_definition, x)
         js_texts = [
-            JSON_JS_HEADER,
-            JSON_JS_OUTPUT.substitute({
+            JSON_OUTPUT_HEADER_JS,
+            JSON_OUTPUT_JS.substitute({
+                'variable_id': variable_id,
+                'data_uri': data_uri})]
+        return {
+            'css_uris': [], 'css_texts': [], 'js_uris': [],
+            'js_texts': js_texts, 'main_text': ''}
+
+
+class PdfView(VariableView):
+
+    view_name = 'pdf'
+    css_texts = [PDF_CSS]
+
+    def render_output(self, b: Batch, x: Element):
+        variable_definition = self.variable_definition
+        variable_id = self.variable_id
+        element_id = x.id
+        data_uri = b.get_data_uri(variable_definition, x)
+        js_texts = [
+            PDF_OUTPUT_HEADER_JS,
+            PDF_OUTPUT_JS.substitute({
                 'variable_id': variable_id,
+                'element_id': element_id,
                 'data_uri': data_uri})]
+        main_text = (
+            f'<iframe id="{element_id}" '
+            f'class="_{x.mode_name} _{self.view_name} {variable_id}" '
+            f'src="{data_uri}" frameborder="0">'
+            '</iframe>')
         return {
-            'css_uris': [], 'js_uris': [], 'main_text': '',
-            'js_texts': js_texts}
+            'css_uris': [], 'css_texts': self.css_texts, 'js_uris': [],
+            'js_texts': js_texts, 'main_text': main_text}
+
+
+class FileView(VariableView):
+
+    view_name = 'file'
+
+    def render_input(self, b: Batch, x: Element):
+        element_id = x.id
+        view_name = self.view_name
+        variable_id = self.variable_id
+        variable_definition = self.variable_definition
+        c = b.get_variable_configuration(variable_definition)
+        mime_types = c.get('mime-types', [])
+        root_uri = template_globals['root_uri']
+        js_texts = [
+            FILE_INPUT_HEADER_JS.substitute({
+                'view_name': view_name,
+                'files_uri': root_uri + FILES_ROUTE})]
+        main_text = FILE_INPUT_HTML.substitute({
+            'element_id': element_id,
+            'mode_name': x.mode_name,
+            'view_name': view_name,
+            'variable_id': variable_id,
+            'accept_what': ','.join(mime_types)})
+        return {
+            'css_uris': [], 'css_texts': [], 'js_uris': [],
+            'js_texts': js_texts, 'main_text': main_text}
 
 
 def initialize_view_by_name():
     for entry_point in entry_points().select(group='crosscompute.views'):
-        VIEW_BY_NAME[entry_point.name] = import_attribute(entry_point.value)
-    return VIEW_BY_NAME
+        view_by_name[entry_point.name] = import_attribute(entry_point.value)
+    return view_by_name
 
 
 def save_variable_data(target_path, data_by_id, variable_definitions):
     target_path.parent.mkdir(parents=True, exist_ok=True)
     variable_data_by_id = get_variable_data_by_id(
         variable_definitions, data_by_id)
     if target_path.suffix == '.dictionary':
@@ -519,21 +575,55 @@
     else:
         variable_id, variable_data = list(variable_data_by_id.items())[0]
         if 'value' in variable_data:
             open(target_path, 'wt').write(variable_data['value'])
         elif 'path' in variable_data:
             shutil.copy(variable_data['path'], target_path)
         elif 'uri' in variable_data:
-            download_uri(variable_data['uri'], target_path)
+            variable_uri = variable_data['uri']
+            if variable_uri.startswith(
+                'http://'
+            ) or variable_uri.startswith('https://'):
+                download_uri(variable_data['uri'], target_path)
+            elif variable_uri.startswith('/f/'):
+                link_files(target_path, variable_uri)
         variable_definition = find_item(
             variable_definitions, 'id', variable_id)
         variable_view = VariableView.get_from(variable_definition)
         variable_view.process(target_path)
 
 
+def link_files(path_template, variable_uri):
+    folder = FILES_FOLDER / variable_uri.replace('/f/', '')
+    with open(folder / 'files.json', 'rt') as f:
+        file_dictionaries = json.load(f)
+    for file_index, file_dictionary in enumerate(file_dictionaries):
+        file_path = folder / str(file_index)
+        file_extension = file_dictionary['extension']
+        target_path = str(path_template).format(
+            index=file_index, extension=file_extension)
+        symlink(file_path, target_path)
+        L.debug(f'linked {file_path} to {target_path}')
+        if target_path == path_template:
+            break
+
+
+def get_data_by_id(automation_definition, batch_definition):
+    automation_folder = automation_definition.folder
+    batch_folder = batch_definition.folder
+    absolute_batch_folder = automation_folder / batch_folder
+    input_data_by_id = get_data_by_id_from_folder(
+        absolute_batch_folder / 'input',
+        automation_definition.get_variable_definitions('input'))
+    output_data_by_id = get_data_by_id_from_folder(
+        absolute_batch_folder / 'output',
+        automation_definition.get_variable_definitions('output'))
+    return input_data_by_id | output_data_by_id
+
+
 def get_data_by_id_from_folder(folder, variable_definitions):
     data_by_id = {}
     for variable_definition in variable_definitions:
         variable_id = variable_definition.id
         variable_path = variable_definition.path
         variable_data = load_variable_data(folder / variable_path, variable_id)
         data_by_id[variable_id] = variable_data
@@ -652,15 +742,19 @@
     variable_view = VariableView.get_from(variable_definition)
     variable_data = load_variable_data(path, variable_id)
     variable_view.process(path)
     return variable_data
 
 
 def load_variable_data(path, variable_id):
-    file_data = FILE_DATA_CACHE[path]
+    try:
+        file_data = FILE_DATA_CACHE[path]
+    except OSError:
+        raise CrossComputeDataError(
+            f'variable {variable_id} not found at {format_path(path)}')
     if path.suffix == '.dictionary':
         file_value = file_data['value']
         try:
             variable_value = file_value[variable_id]
         except KeyError:
             raise CrossComputeDataError(
                 f'variable {variable_id} not found in {format_path(path)}')
@@ -725,16 +819,15 @@
                     f'{variable_id} not defined in batch configuration')
         variable_data_by_id[variable_id] = variable_data
     return variable_data_by_id
 
 
 def get_variable_value_by_id(data_by_id):
     return {
-        variable_id: data['value'] for variable_id, data in data_by_id.items()
-    }
+        variable_id: data['value'] for variable_id, data in data_by_id.items()}
 
 
 def format_text(text, data_by_id):
     text = str(text)
     if not data_by_id:
         return text
 
@@ -769,94 +862,34 @@
             f = function_by_name[function_name]
         except KeyError:
             raise
         value = f(value)
     return value
 
 
-def add_label_html(main_text, variable_configuration, variable_id, element_id):
-    label_text = get_label_text(variable_configuration, variable_id)
+def add_label_html(main_text, variable_definition, element_id):
+    label_text = variable_definition.label
     if label_text:
         main_text = '<label for="%s">%s</label> %s' % (
             element_id, label_text, main_text)
     return main_text
 
 
-def get_label_text(variable_configuration, variable_id):
-    if 'label' in variable_configuration:
-        label_text = variable_configuration['label'] or ''
-    else:
-        label_text = format_name(variable_id)
-    return label_text.strip()
-
-
 def get_configuration_options(variable_configuration, variable_values):
     options = []
     for i, d in enumerate(variable_configuration.get('options', [{
             'value': _} for _ in variable_values])):
         option_value = d['value']
         options.append({
             'id': d.get('id', i),
             'name': d.get('name', option_value),
             'value': option_value})
     return options
 
 
-L = getLogger(__name__)
-
-
-LINK_JS_HEADER = asset_storage.load_raw_text('link-header.js')
-LINK_JS_OUTPUT = asset_storage.load_string_text('link-output.js')
-
-
-STRING_HTML_INPUT = asset_storage.load_jinja_text('string-input.html')
-STRING_JS_INPUT = asset_storage.load_string_text('string-input.js')
-STRING_JS_HEADER = asset_storage.load_raw_text('string-header.js')
-STRING_JS_OUTPUT = asset_storage.load_string_text('string-output.js')
-
-
-TEXT_HTML_INPUT = asset_storage.load_string_text('text-input.html')
-TEXT_JS_HEADER = asset_storage.load_raw_text('text-header.js')
-TEXT_JS_INPUT = asset_storage.load_string_text('text-input.js')
-TEXT_JS_OUTPUT = asset_storage.load_string_text('text-output.js')
-
-
-MARKDOWN_JS_HEADER = asset_storage.load_raw_text('markdown-header.js')
-MARKDOWN_JS_OUTPUT = asset_storage.load_string_text('markdown-output.js')
-
-
-IMAGE_JS_HEADER = asset_storage.load_raw_text('image-header.js')
-IMAGE_JS_OUTPUT = asset_storage.load_string_text('image-output.js')
-
-
-RADIO_HTML_INPUT = asset_storage.load_jinja_text('radio-input.html')
-RADIO_JS_HEADER = asset_storage.load_raw_text('radio-header.js')
-RADIO_JS_INPUT = asset_storage.load_string_text('radio-input.js')
-RADIO_JS_OUTPUT = asset_storage.load_string_text('radio-output.js')
-
-
-CHECKBOX_HTML_INPUT = asset_storage.load_jinja_text('checkbox-input.html')
-CHECKBOX_JS_HEADER = asset_storage.load_raw_text('checkbox-header.js')
-CHECKBOX_JS_INPUT = asset_storage.load_string_text('checkbox-input.js')
-CHECKBOX_JS_OUTPUT = asset_storage.load_string_text('checkbox-output.js')
-
-
-TABLE_JS_HEADER = asset_storage.load_raw_text('table-header.js')
-TABLE_JS_OUTPUT = asset_storage.load_string_text('table-output.js')
-
-
-FRAME_JS_HEADER = asset_storage.load_raw_text('frame-header.js')
-FRAME_JS_OUTPUT = asset_storage.load_string_text('frame-output.js')
-
-
-JSON_JS_HEADER = asset_storage.load_raw_text('json-header.js')
-JSON_JS_OUTPUT = asset_storage.load_string_text('json-output.js')
-
-
 YIELD_DATA_BY_ID_BY_EXTENSION = {
     '.csv': yield_data_by_id_from_csv,
     '.txt': yield_data_by_id_from_txt}
-
-
 FILE_DATA_CACHE = FileCache(
     load_file_data=load_file_data,
     maximum_length=MAXIMUM_FILE_CACHE_LENGTH)
+L = getLogger(__name__)
```

### Comparing `crosscompute-0.9.3.3/crosscompute/scripts/configure.py` & `crosscompute-0.9.4.2/crosscompute/scripts/configure.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from argparse import ArgumentParser
-from invisibleroads_macros_log import format_path
 from logging import getLogger
 from pathlib import Path
 
+from invisibleroads_macros_log import format_path
+
 from crosscompute import __version__
 from crosscompute.constants import (
     ASSETS_FOLDER,
     AUTOMATION_NAME,
     AUTOMATION_PATH,
     AUTOMATION_VERSION)
 from crosscompute.exceptions import (
@@ -50,15 +51,14 @@
         try:
             configuration = load_raw_configuration(
                 path_or_folder, with_comments=True)
         except CrossComputeError:
             pass
     configuration, configuration_path = input_configuration(
         configuration, path_or_folder)
-    print(dict(configuration))
     save_configuration(configuration_path, configuration)
     return configuration_path
 
 
 def input_configuration(configuration, path_or_folder):
     if not configuration:
         configuration = load_raw_configuration(
```

### Comparing `crosscompute-0.9.3.3/crosscompute/scripts/launch.py` & `crosscompute-0.9.4.2/crosscompute/scripts/launch.py`

 * *Files 14% similar despite different names*

```diff
@@ -35,34 +35,30 @@
     if launch_id == 'configure':
         configure_with(args)
         return
     automation = _get_automation_from(args)
     if launch_id == 'print':
         print_with(automation, args)
         return
-    processes = []
     if launch_id in ['serve', 'all']:
         check_port(args.port)
-        processes.append(StoppableProcess(
-            name='serve', target=serve_with, args=(automation, args)))
-    if launch_id in ['run', 'all']:
-        processes.append(StoppableProcess(
-            name='run', target=run_with, args=(automation, args)))
+        process = StoppableProcess(
+            name='serve', target=serve_with, args=(automation, args))
+    elif launch_id in ['run']:
+        process = StoppableProcess(
+            name='run', target=run_with, args=(automation, args))
     try:
-        for process in processes:
-            process.start()
-        for process in reversed(processes):
-            process.join()
+        process.start()
+        process.join()
     except KeyboardInterrupt:
-        L.info('waiting for processes to stop')
+        L.info('waiting for process to stop')
     except Exception as e:
         L.exception(e)
     finally:
-        for process in processes:
-            process.stop()
+        process.stop()
 
 
 def configure_argument_parser_for_launching(a):
     a.add_argument(
         '--configure', dest='is_configure_only', action='store_true',
         help='configure only')
     a.add_argument(
@@ -70,14 +66,17 @@
         help='serve only')
     a.add_argument(
         '--run', dest='is_run_only', action='store_true',
         help='run only')
     a.add_argument(
         '--print', dest='is_print_only', action='store_true',
         help='print only')
+    a.add_argument(
+        '--version', dest='is_version_only', action='store_true',
+        help='show version')
 
 
 def get_launch_id_from(args):
     launch_id = 'all'
     if args.is_configure_only:
         launch_id = 'configure'
     elif args.is_run_only:
@@ -93,14 +92,17 @@
     a = ArgumentParser()
     configure_argument_parser_for_logging(a)
     configure_argument_parser_for_launching(a)
     configure_argument_parser_for_configuring(a)
     configure_argument_parser_for_serving(a)
     configure_argument_parser_for_running(a)
     args = a.parse_args(arguments)
+    if args.is_version_only:
+        print(__version__)
+        raise SystemExit
     try:
         configure_logging_from(args)
         configure_serving_from(args)
         configure_running_from(args)
     except CrossComputeError as e:
         L.error(e)
         raise SystemExit
```

### Comparing `crosscompute-0.9.3.3/crosscompute/scripts/run.py` & `crosscompute-0.9.4.2/crosscompute/scripts/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
 def run_with(automation, args):
     return run(automation, args.environment, args.with_rebuild)
 
 
 def run(automation, environment, with_rebuild=True):
     try:
-        automation.run(environment, with_rebuild)
+        automation.run(environment, with_rebuild=with_rebuild)
     except CrossComputeError as e:
         L.error(e)
     except KeyboardInterrupt:
         pass
 
 
 L = getLogger(__name__)
```

### Comparing `crosscompute-0.9.3.3/crosscompute/scripts/serve.py` & `crosscompute-0.9.4.2/crosscompute/scripts/serve.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 from invisibleroads_macros_web.browser import (
     open_browser)
 from invisibleroads_macros_web.port import (
     find_open_port,
     is_port_in_use)
 
 from crosscompute.constants import (
-    DISK_DEBOUNCE_IN_MILLISECONDS,
-    DISK_POLL_IN_MILLISECONDS,
     HOST,
     MAXIMUM_PORT,
     MINIMUM_PORT,
     PORT)
 from crosscompute.exceptions import (
     CrossComputeError)
 from crosscompute.routines.automation import (
@@ -74,22 +72,14 @@
         '--root-uri', metavar='X',
         default='',
         help='specify root uri for all routes')
     a.add_argument(
         '--origins', metavar='X', nargs='+', dest='allowed_origins',
         default=[],
         help='specify allowed origins')
-    a.add_argument(
-        '--disk-poll', metavar='X', type=int,
-        default=DISK_POLL_IN_MILLISECONDS,
-        help='interval in milliseconds to check disk for changes')
-    a.add_argument(
-        '--disk-debounce', metavar='X', type=int,
-        default=DISK_DEBOUNCE_IN_MILLISECONDS,
-        help='interval in milliseconds to wait until changes stop')
 
 
 def configure_serving_from(args):
     root_uri = args.root_uri
     if root_uri and not root_uri.startswith('/'):
         args.root_uri = '/' + root_uri
 
@@ -101,40 +91,34 @@
         host=args.host,
         port=args.port,
         with_browser=args.with_browser,
         with_restart=args.with_restart,
         with_prefix=args.with_prefix,
         with_hidden=args.with_hidden,
         root_uri=args.root_uri,
-        allowed_origins=args.allowed_origins,
-        disk_poll_in_milliseconds=args.disk_poll,
-        disk_debounce_in_milliseconds=args.disk_debounce)
+        allowed_origins=args.allowed_origins)
 
 
 def serve(
         automation, environment, host=HOST, port=PORT, with_browser=True,
         with_restart=True, with_prefix=True, with_hidden=True, root_uri='',
-        allowed_origins=None,
-        disk_poll_in_milliseconds=DISK_POLL_IN_MILLISECONDS,
-        disk_debounce_in_milliseconds=DISK_DEBOUNCE_IN_MILLISECONDS):
+        allowed_origins=None):
     try:
         if with_browser and 'DISPLAY' in environ:
             L.info('opening browser; set --no-browser to disable')
             open_browser(f'http://localhost:{port}{root_uri}')
         automation.serve(
             environment,
             host=host,
             port=port,
             with_restart=with_restart,
             with_prefix=with_prefix,
             with_hidden=with_hidden,
             root_uri=root_uri,
-            allowed_origins=allowed_origins,
-            disk_poll_in_milliseconds=disk_poll_in_milliseconds,
-            disk_debounce_in_milliseconds=disk_debounce_in_milliseconds)
+            allowed_origins=allowed_origins)
     except CrossComputeError as e:
         L.error(e)
     except KeyboardInterrupt:
         pass
 
 
 def check_port(port):
```

### Comparing `crosscompute-0.9.3.3/crosscompute/settings.py` & `crosscompute-0.9.4.2/crosscompute/settings.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,45 +5,43 @@
 from invisibleroads_macros_web.jinja import (
     PathTemplateLoader,
     RelativeTemplateEnvironment)
 from invisibleroads_macros_web.starlette import (
     TemplateResponseFactory)
 
 from .constants import (
-    MAXIMUM_PING_INTERVAL_IN_SECONDS,
-    MINIMUM_PING_INTERVAL_IN_SECONDS,
     TEMPLATE_PATH_BY_ID)
 
 
 multiprocessing_context = mp.get_context('fork')
 StoppableProcess = partial(
     invisibleroads_macros_process.StoppableProcess,
     multiprocessing_context.Process)
 site = {
     'name': 'Automations',
     'configuration': None,
     'definitions': [],
     'environment': {},
     'safe': None,
-    'queue': None,
+    'uris': [],
+    'tasks': [],
     'changes': {},
     'with_prefix': True,
     'with_hidden': True}
 template_path_by_id = TEMPLATE_PATH_BY_ID.copy()
 template_environment = RelativeTemplateEnvironment(
     loader=PathTemplateLoader(),
     autoescape=True,
     trim_blocks=True,
     lstrip_blocks=True)
 template_globals = template_environment.globals = {
     'base_template_path': template_path_by_id['base'],
     'live_template_path': template_path_by_id['live'],
     'google_analytics_id': '',
-    'server_timestamp': 0,
+    'server_time': 0,
     'root_uri': '',
-    'with_restart': True,
-    'maximum_ping_interval_in_milliseconds':
-        MAXIMUM_PING_INTERVAL_IN_SECONDS * 1000,
-    'minimum_ping_interval_in_milliseconds':
-        MINIMUM_PING_INTERVAL_IN_SECONDS * 1000}
+    'with_restart': True}
 TemplateResponse = TemplateResponseFactory(
     template_environment).TemplateResponse
+printer_by_name = {}
+view_by_name = {}
+button_text_by_id = {}
```

### Comparing `crosscompute-0.9.3.3/crosscompute.egg-info/PKG-INFO` & `crosscompute-0.9.4.2/crosscompute.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crosscompute
-Version: 0.9.3.3
+Version: 0.9.4.2
 Summary: Automate your Jupyter notebooks and scripts as tools, reports, dashboards.
 Home-page: https://crosscompute.com
 Author: CrossCompute Inc.
 Author-email: support@crosscompute.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/crosscompute/crosscompute/issues
 Project-URL: Documentation, https://github.com/crosscompute/crosscompute-docs
@@ -56,26 +56,28 @@
 - markdown
 - image
 - radio
 - checkbox
 - table
 - frame
 - json
+- pdf
+- file
 - map-mapbox (crosscompute-views-map)
 - map-mapbox-location (crosscompute-views-map)
 - map-deck-screengrid (crosscompute-views-map)
 - barcode (crosscompute-views-barcode)
 
 [Here are the currently supported configuration options](https://github.com/crosscompute/crosscompute/blob/develop/crosscompute/templates/configuration.yaml).
 
 ## Usage
 
 ```bash
 # Upgrade package
-pip install crosscompute>=0.9.3 --upgrade
+pip install crosscompute>=0.9.4 --upgrade
 
 # Initialize configuration
 crosscompute
 
 # Serve automation
 crosscompute automate.yml
 ```
@@ -126,15 +128,15 @@
 ```
 sudo dnf -y install python3.10
 # sudo apt -y install python3.10
 
 python3.10 -m venv ~/.virtualenvs/crosscompute
 source ~/.virtualenvs/crosscompute/bin/activate
 
-pip install crosscompute>=0.9.3
+pip install crosscompute>=0.9.4
 ```
 
 ## Acknowledgments
 
 - [Olga Ryabtseva](https://www.linkedin.com/in/olga-creutzburg)
 - [Salah Ahmed](https://www.linkedin.com/in/salahspage)
 - [Rodrigo Guarachi](https://www.linkedin.com/in/rmguarachi)
```

### Comparing `crosscompute-0.9.3.3/crosscompute.egg-info/SOURCES.txt` & `crosscompute-0.9.4.2/crosscompute.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -13,79 +13,91 @@
 crosscompute.egg-info/dependency_links.txt
 crosscompute.egg-info/entry_points.txt
 crosscompute.egg-info/requires.txt
 crosscompute.egg-info/top_level.txt
 crosscompute.egg-info/zip-safe
 crosscompute/assets/automation.html
 crosscompute/assets/base.html
-crosscompute/assets/checkbox-header.js
+crosscompute/assets/button-panel.html
+crosscompute/assets/checkbox-input-header.js
 crosscompute/assets/checkbox-input.html
-crosscompute/assets/checkbox-input.js
+crosscompute/assets/checkbox-output-header.js
 crosscompute/assets/checkbox-output.js
 crosscompute/assets/configuration.yml
 crosscompute/assets/default.css
 crosscompute/assets/embedded.css
 crosscompute/assets/favicon.ico
-crosscompute/assets/flex-vertical.css
-crosscompute/assets/frame-header.js
+crosscompute/assets/file-input-header.js
+crosscompute/assets/file-input.html
+crosscompute/assets/file-input.js
+crosscompute/assets/flex.css
+crosscompute/assets/frame-output-header.js
 crosscompute/assets/frame-output.js
-crosscompute/assets/image-header.js
+crosscompute/assets/image-output-header.js
 crosscompute/assets/image-output.js
-crosscompute/assets/json-header.js
+crosscompute/assets/json-output-header.js
 crosscompute/assets/json-output.js
-crosscompute/assets/link-header.js
+crosscompute/assets/link-output-header.js
 crosscompute/assets/link-output.js
 crosscompute/assets/live.html
-crosscompute/assets/markdown-header.js
+crosscompute/assets/markdown-output-header.js
 crosscompute/assets/markdown-output.js
-crosscompute/assets/radio-header.js
+crosscompute/assets/pdf-output-header.js
+crosscompute/assets/pdf-output.js
+crosscompute/assets/pdf.css
+crosscompute/assets/printed.css
+crosscompute/assets/radio-input-header.js
 crosscompute/assets/radio-input.html
-crosscompute/assets/radio-input.js
+crosscompute/assets/radio-output-header.js
 crosscompute/assets/radio-output.js
 crosscompute/assets/root.html
 crosscompute/assets/step-body.js
-crosscompute/assets/step-main.html
 crosscompute/assets/step.html
-crosscompute/assets/string-header.js
+crosscompute/assets/string-input-header.js
 crosscompute/assets/string-input.html
-crosscompute/assets/string-input.js
+crosscompute/assets/string-output-header.js
 crosscompute/assets/string-output.js
-crosscompute/assets/table-header.js
+crosscompute/assets/table-output-header.js
 crosscompute/assets/table-output.js
-crosscompute/assets/text-header.js
 crosscompute/assets/text-input.html
 crosscompute/assets/text-input.js
+crosscompute/assets/text-output-header.js
 crosscompute/assets/text-output.js
 crosscompute/macros/__init__.py
 crosscompute/macros/disk.py
 crosscompute/macros/iterable.py
+crosscompute/macros/log.py
 crosscompute/macros/package.py
 crosscompute/macros/security.py
 crosscompute/routers/__init__.py
 crosscompute/routers/automation.py
-crosscompute/routers/mutation.py
+crosscompute/routers/file.py
 crosscompute/routers/root.py
+crosscompute/routers/stream.py
 crosscompute/routers/token.py
 crosscompute/routines/__init__.py
 crosscompute/routines/asset.py
 crosscompute/routines/authorization.py
 crosscompute/routines/automation.py
 crosscompute/routines/batch.py
 crosscompute/routines/configuration.py
 crosscompute/routines/database.py
 crosscompute/routines/interface.py
 crosscompute/routines/log.py
+crosscompute/routines/mutation.py
 crosscompute/routines/printer.py
 crosscompute/routines/server.py
 crosscompute/routines/step.py
+crosscompute/routines/uri.py
 crosscompute/routines/variable.py
+crosscompute/routines/work.py
 crosscompute/scripts/__init__.py
 crosscompute/scripts/configure.py
 crosscompute/scripts/launch.py
 crosscompute/scripts/print.py
 crosscompute/scripts/run.py
 crosscompute/scripts/serve.py
 tests/test_macros_iterable.py
 tests/test_macros_security.py
-tests/test_routines_automation.py
 tests/test_routines_configuration.py
-tests/test_routines_variable.py
+tests/test_routines_variable.py
+tests/test_routines_work.py
```

### Comparing `crosscompute-0.9.3.3/crosscompute.egg-info/entry_points.txt` & `crosscompute-0.9.4.2/crosscompute.egg-info/entry_points.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 [console_scripts]
 crosscompute = crosscompute.scripts.launch:do
 
 [crosscompute.views]
 checkbox = crosscompute.routines.variable.CheckboxView
 email = crosscompute.routines.variable.EmailView
+file = crosscompute.routines.variable.FileView
 frame = crosscompute.routines.variable.FrameView
 image = crosscompute.routines.variable.ImageView
 json = crosscompute.routines.variable.JsonView
 link = crosscompute.routines.variable.LinkView
 markdown = crosscompute.routines.variable.MarkdownView
 number = crosscompute.routines.variable.NumberView
 password = crosscompute.routines.variable.PasswordView
+pdf = crosscompute.routines.variable.PdfView
 radio = crosscompute.routines.variable.RadioView
 string = crosscompute.routines.variable.StringView
 table = crosscompute.routines.variable.TableView
 text = crosscompute.routines.variable.TextView
```

### Comparing `crosscompute-0.9.3.3/setup.cfg` & `crosscompute-0.9.4.2/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = crosscompute
-version = 0.9.3.3
+version = 0.9.4.2
 description = Automate your Jupyter notebooks and scripts as tools, reports, dashboards.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://crosscompute.com
 author = CrossCompute Inc.
 author_email = support@crosscompute.com
 license = MIT
@@ -30,29 +30,31 @@
 	Source Code = https://github.com/crosscompute/crosscompute
 
 [options]
 packages = find:
 python_requires = >=3.10
 install_requires = 
 	fastapi
-	importlib-metadata >= 4.10.1
+	importlib-metadata >= 6.6.0
 	invisibleroads-macros-disk >= 1.3.0
 	invisibleroads-macros-log >= 1.0.6
 	invisibleroads-macros-process >= 0.2.0
 	invisibleroads-macros-security >= 1.0.3
 	invisibleroads-macros-text >= 1.1.2
-	invisibleroads-macros-web[jinja,markdown,starlette] >= 0.2.4
+	invisibleroads-macros-web[jinja,markdown,starlette] >= 0.3.0
 	jinja2
 	markdown
 	nbconvert
 	nbformat
+	python-multipart
 	requests
 	ruamel.yaml
+	sse-starlette
 	tomli
-	uvicorn
+	uvicorn >= 0.21.1
 	watchfiles
 zip_safe = True
 
 [options.package_data]
 crosscompute = 
 	assets/*.css
 	assets/*.html
@@ -73,14 +75,16 @@
 	markdown = crosscompute.routines.variable.MarkdownView
 	image = crosscompute.routines.variable.ImageView
 	radio = crosscompute.routines.variable.RadioView
 	checkbox = crosscompute.routines.variable.CheckboxView
 	table = crosscompute.routines.variable.TableView
 	frame = crosscompute.routines.variable.FrameView
 	json = crosscompute.routines.variable.JsonView
+	pdf = crosscompute.routines.variable.PdfView
+	file = crosscompute.routines.variable.FileView
 
 [options.extras_require]
 test = 
 	pytest-cov
 	pytest-xdist
 	requests-cache
```

### Comparing `crosscompute-0.9.3.3/tests/test_routines_automation.py` & `crosscompute-0.9.4.2/tests/test_routines_work.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from pytest import raises
 
 from crosscompute.exceptions import (
     CrossComputeConfigurationError,
     CrossComputeExecutionError)
-from crosscompute.routines.automation import _run_command
+from crosscompute.routines.work import (
+    _run_command)
 
 
 def test_run_command(tmp_path):
     o_path = tmp_path / 'o.txt'
     e_path = tmp_path / 'e.txt'
     with open(o_path, 'wt') as o_file, open(e_path, 'w+t') as e_file:
         with raises(CrossComputeConfigurationError):
```

### Comparing `crosscompute-0.9.3.3/tests/test_routines_variable.py` & `crosscompute-0.9.4.2/tests/test_routines_variable.py`

 * *Files identical despite different names*

