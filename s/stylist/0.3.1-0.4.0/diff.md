# Comparing `tmp/stylist-0.3.1.tar.gz` & `tmp/stylist-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/stylist-0.3.1.tar", last modified: Thu Dec  1 15:44:13 2022, max compression
+gzip compressed data, was "/tmp/persistent/mhambley/stylist/dist/.tmp-ghg5eegh/stylist-0.4.0.tar", last modified: Tue Apr 25 15:22:38 2023, max compression
```

## Comparing `stylist-0.3.1.tar` & `stylist-0.4.0.tar`

### file list

```diff
@@ -1,182 +1,49 @@
-drwxr-xr-x   0 mhambley (10374) users     (1000)        0 2022-12-01 15:44:13.000000 stylist-0.3.1/
--rw-r--r--   0 mhambley (10374) users     (1000)     3215 2022-08-10 10:05:46.000000 stylist-0.3.1/CONTRIBUTING.md
--rw-r--r--   0 mhambley (10374) users     (1000)     1550 2022-08-10 10:05:46.000000 stylist-0.3.1/LICENSE
--rw-r--r--   0 mhambley (10374) users     (1000)      147 2022-08-10 10:05:46.000000 stylist-0.3.1/MANIFEST.in
--rw-r--r--   0 mhambley (10374) users     (1000)     5475 2022-12-01 15:44:13.000000 stylist-0.3.1/PKG-INFO
--rw-r--r--   0 mhambley (10374) users     (1000)     4509 2022-12-01 15:41:12.000000 stylist-0.3.1/README.rst
-drwxr-xr-x   0 mhambley (10374) users     (1000)        0 2022-12-01 15:44:12.000000 stylist-0.3.1/documentation/
--rw-r--r--   0 mhambley (10374) users     (1000)       34 2022-08-10 10:05:46.000000 stylist-0.3.1/documentation/.gitignore
--rw-r--r--   0 mhambley (10374) users     (1000)      630 2022-08-10 10:05:46.000000 stylist-0.3.1/documentation/Makefile
-drwxr-xr-x   0 mhambley (10374) users     (1000)        0 2022-12-01 15:44:12.000000 stylist-0.3.1/documentation/build/
-drwxr-xr-x   0 mhambley (10374) users     (1000)        0 2022-12-01 15:44:12.000000 stylist-0.3.1/documentation/build/doctrees/
-drwxr-xr-x   0 mhambley (10374) users     (1000)        0 2022-12-01 15:44:12.000000 stylist-0.3.1/documentation/build/doctrees/developer-information/
-drwxr-xr-x   0 mhambley (10374) users     (1000)        0 2022-12-01 15:44:12.000000 stylist-0.3.1/documentation/build/doctrees/developer-information/api/
--rw-r--r--   0 mhambley (10374) users     (1000)    50683 2022-08-11 09:30:58.000000 stylist-0.3.1/documentation/build/doctrees/developer-information/api/stylist.configuration.doctree
--rw-r--r--   0 mhambley (10374) users     (1000)    16565 2022-08-11 09:30:58.000000 stylist-0.3.1/documentation/build/doctrees/developer-information/api/stylist.doctree
--rw-r--r--   0 mhambley (10374) users     (1000)    12996 2022-08-11 09:30:58.000000 stylist-0.3.1/documentation/build/doctrees/developer-information/api/stylist.engine.doctree
--rw-r--r--   0 mhambley (10374) users     (1000)    96856 2022-08-11 09:30:59.000000 stylist-0.3.1/documentation/build/doctrees/developer-information/api/stylist.fortran.doctree
--rw-r--r--   0 mhambley (10374) users     (1000)    24151 2022-08-11 09:30:59.000000 stylist-0.3.1/documentation/build/doctrees/developer-information/api/stylist.issue.doctree
--rw-r--r--   0 mhambley (10374) users     (1000)    18766 2022-08-11 09:30:59.000000 stylist-0.3.1/documentation/build/doctrees/developer-information/api/stylist.rule.doctree
--rw-r--r--   0 mhambley (10374) users     (1000)   164012 2022-08-11 09:30:59.000000 stylist-0.3.1/documentation/build/doctrees/developer-information/api/stylist.source.doctree
--rw-r--r--   0 mhambley (10374) users     (1000)    23806 2022-08-11 09:30:59.000000 stylist-0.3.1/documentation/build/doctrees/developer-information/api/stylist.style.doctree
--rw-r--r--   0 mhambley (10374) users     (1000)     4810 2022-08-11 09:30:58.000000 stylist-0.3.1/documentation/build/doctrees/developer-information/api.doctree
--rw-r--r--   0 mhambley (10374) users     (1000)     8263 2022-08-11 09:30:59.000000 stylist-0.3.1/documentation/build/doctrees/developer-information/environment.doctree
--rw-r--r--   0 mhambley (10374) users     (1000)     6628 2022-08-11 09:54:55.000000 stylist-0.3.1/documentation/build/doctrees/developer-information/index.doctree
--rw-r--r--   0 mhambley (10374) users     (1000)     2432 2022-08-11 09:30:59.000000 stylist-0.3.1/documentation/build/doctrees/developer-information/new-rules.doctree
--rw-r--r--   0 mhambley (10374) users     (1000)    14982 2022-08-11 09:54:55.000000 stylist-0.3.1/documentation/build/doctrees/developer-information/overview.doctree
--rw-r--r--   0 mhambley (10374) users     (1000)    14006 2022-08-11 09:56:22.000000 stylist-0.3.1/documentation/build/doctrees/developer-information/rules.doctree
--rw-r--r--   0 mhambley (10374) users     (1000)    28671 2022-08-11 09:47:31.000000 stylist-0.3.1/documentation/build/doctrees/developer-information/structure.doctree
--rw-r--r--   0 mhambley (10374) users     (1000)     2895 2022-08-11 09:30:59.000000 stylist-0.3.1/documentation/build/doctrees/developer-information/todo.doctree
--rw-r--r--   0 mhambley (10374) users     (1000)   269008 2022-08-11 12:34:45.000000 stylist-0.3.1/documentation/build/doctrees/environment.pickle
--rw-r--r--   0 mhambley (10374) users     (1000)     5361 2022-08-11 12:13:10.000000 stylist-0.3.1/documentation/build/doctrees/index.doctree
-drwxr-xr-x   0 mhambley (10374) users     (1000)        0 2022-12-01 15:44:12.000000 stylist-0.3.1/documentation/build/doctrees/user-manual/
--rw-r--r--   0 mhambley (10374) users     (1000)     7231 2022-08-11 12:13:10.000000 stylist-0.3.1/documentation/build/doctrees/user-manual/configuration.doctree
--rw-r--r--   0 mhambley (10374) users     (1000)     4212 2022-08-11 12:34:45.000000 stylist-0.3.1/documentation/build/doctrees/user-manual/index.doctree
--rw-r--r--   0 mhambley (10374) users     (1000)    11609 2022-08-11 09:30:59.000000 stylist-0.3.1/documentation/build/doctrees/user-manual/preparation.doctree
--rw-r--r--   0 mhambley (10374) users     (1000)    29455 2022-08-11 09:31:00.000000 stylist-0.3.1/documentation/build/doctrees/user-manual/rule-list.doctree
-drwxr-xr-x   0 mhambley (10374) users     (1000)        0 2022-12-01 15:44:12.000000 stylist-0.3.1/documentation/build/html/
--rw-r--r--   0 mhambley (10374) users     (1000)      230 2022-08-11 12:34:45.000000 stylist-0.3.1/documentation/build/html/.buildinfo
-drwxr-xr-x   0 mhambley (10374) users     (1000)        0 2022-12-01 15:44:12.000000 stylist-0.3.1/documentation/build/html/_sources/
-drwxr-xr-x   0 mhambley (10374) users     (1000)        0 2022-12-01 15:44:12.000000 stylist-0.3.1/documentation/build/html/_sources/developer-information/
-drwxr-xr-x   0 mhambley (10374) users     (1000)        0 2022-12-01 15:44:13.000000 stylist-0.3.1/documentation/build/html/_sources/developer-information/api/
--rw-r--r--   0 mhambley (10374) users     (1000)      234 2022-08-11 09:30:57.000000 stylist-0.3.1/documentation/build/html/_sources/developer-information/api/stylist.configuration.rst.txt
--rw-r--r--   0 mhambley (10374) users     (1000)      187 2022-08-11 09:30:58.000000 stylist-0.3.1/documentation/build/html/_sources/developer-information/api/stylist.engine.rst.txt
--rw-r--r--   0 mhambley (10374) users     (1000)      388 2022-08-11 09:30:58.000000 stylist-0.3.1/documentation/build/html/_sources/developer-information/api/stylist.fortran.rst.txt
--rw-r--r--   0 mhambley (10374) users     (1000)      178 2022-08-11 09:30:58.000000 stylist-0.3.1/documentation/build/html/_sources/developer-information/api/stylist.issue.rst.txt
--rw-r--r--   0 mhambley (10374) users     (1000)      375 2022-08-11 09:30:57.000000 stylist-0.3.1/documentation/build/html/_sources/developer-information/api/stylist.rst.txt
--rw-r--r--   0 mhambley (10374) users     (1000)      199 2022-08-11 09:30:58.000000 stylist-0.3.1/documentation/build/html/_sources/developer-information/api/stylist.rule.rst.txt
--rw-r--r--   0 mhambley (10374) users     (1000)      551 2022-08-11 09:30:58.000000 stylist-0.3.1/documentation/build/html/_sources/developer-information/api/stylist.source.rst.txt
--rw-r--r--   0 mhambley (10374) users     (1000)      254 2022-08-11 09:30:58.000000 stylist-0.3.1/documentation/build/html/_sources/developer-information/api/stylist.style.rst.txt
--rw-r--r--   0 mhambley (10374) users     (1000)      176 2022-08-10 10:05:46.000000 stylist-0.3.1/documentation/build/html/_sources/developer-information/api.rst.txt
--rw-r--r--   0 mhambley (10374) users     (1000)     1503 2022-08-11 08:14:12.000000 stylist-0.3.1/documentation/build/html/_sources/developer-information/environment.rst.txt
--rw-r--r--   0 mhambley (10374) users     (1000)      639 2022-08-11 09:51:29.000000 stylist-0.3.1/documentation/build/html/_sources/developer-information/index.rst.txt
--rw-r--r--   0 mhambley (10374) users     (1000)       37 2022-08-11 08:16:03.000000 stylist-0.3.1/documentation/build/html/_sources/developer-information/new-rules.rst.txt
--rw-r--r--   0 mhambley (10374) users     (1000)     3813 2022-08-11 09:52:11.000000 stylist-0.3.1/documentation/build/html/_sources/developer-information/overview.rst.txt
--rw-r--r--   0 mhambley (10374) users     (1000)     1949 2022-08-11 09:55:51.000000 stylist-0.3.1/documentation/build/html/_sources/developer-information/rules.rst.txt
--rw-r--r--   0 mhambley (10374) users     (1000)     4357 2022-08-11 09:47:25.000000 stylist-0.3.1/documentation/build/html/_sources/developer-information/structure.rst.txt
--rw-r--r--   0 mhambley (10374) users     (1000)      182 2022-08-10 10:05:46.000000 stylist-0.3.1/documentation/build/html/_sources/developer-information/todo.rst.txt
--rw-r--r--   0 mhambley (10374) users     (1000)     1036 2022-08-11 12:12:24.000000 stylist-0.3.1/documentation/build/html/_sources/index.rst.txt
-drwxr-xr-x   0 mhambley (10374) users     (1000)        0 2022-12-01 15:44:13.000000 stylist-0.3.1/documentation/build/html/_sources/user-manual/
--rw-r--r--   0 mhambley (10374) users     (1000)     1624 2022-08-11 10:13:14.000000 stylist-0.3.1/documentation/build/html/_sources/user-manual/configuration.rst.txt
--rw-r--r--   0 mhambley (10374) users     (1000)      544 2022-08-11 12:34:40.000000 stylist-0.3.1/documentation/build/html/_sources/user-manual/index.rst.txt
--rw-r--r--   0 mhambley (10374) users     (1000)     2105 2022-08-10 10:05:46.000000 stylist-0.3.1/documentation/build/html/_sources/user-manual/preparation.rst.txt
--rw-r--r--   0 mhambley (10374) users     (1000)     1692 2022-08-10 10:05:46.000000 stylist-0.3.1/documentation/build/html/_sources/user-manual/rule-list.rst.txt
-drwxr-xr-x   0 mhambley (10374) users     (1000)        0 2022-12-01 15:44:13.000000 stylist-0.3.1/documentation/build/html/_static/
--rw-r--r--   0 mhambley (10374) users     (1000)    14692 2022-08-11 12:34:45.000000 stylist-0.3.1/documentation/build/html/_static/basic.css
-drwxr-xr-x   0 mhambley (10374) users     (1000)        0 2022-12-01 15:44:13.000000 stylist-0.3.1/documentation/build/html/_static/css/
--rw-r--r--   0 mhambley (10374) users     (1000)     3275 2022-04-04 15:40:49.000000 stylist-0.3.1/documentation/build/html/_static/css/badge_only.css
-drwxr-xr-x   0 mhambley (10374) users     (1000)        0 2022-12-01 15:44:13.000000 stylist-0.3.1/documentation/build/html/_static/css/fonts/
--rw-r--r--   0 mhambley (10374) users     (1000)    87624 2022-04-04 15:40:50.000000 stylist-0.3.1/documentation/build/html/_static/css/fonts/Roboto-Slab-Bold.woff
--rw-r--r--   0 mhambley (10374) users     (1000)    67312 2022-04-04 15:40:50.000000 stylist-0.3.1/documentation/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
--rw-r--r--   0 mhambley (10374) users     (1000)    86288 2022-04-04 15:40:50.000000 stylist-0.3.1/documentation/build/html/_static/css/fonts/Roboto-Slab-Regular.woff
--rw-r--r--   0 mhambley (10374) users     (1000)    66444 2022-04-04 15:40:50.000000 stylist-0.3.1/documentation/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
--rw-r--r--   0 mhambley (10374) users     (1000)   165742 2022-04-04 15:40:50.000000 stylist-0.3.1/documentation/build/html/_static/css/fonts/fontawesome-webfont.eot
--rw-r--r--   0 mhambley (10374) users     (1000)   444379 2022-04-04 15:40:50.000000 stylist-0.3.1/documentation/build/html/_static/css/fonts/fontawesome-webfont.svg
--rw-r--r--   0 mhambley (10374) users     (1000)   165548 2022-04-04 15:40:50.000000 stylist-0.3.1/documentation/build/html/_static/css/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 mhambley (10374) users     (1000)    98024 2022-04-04 15:40:50.000000 stylist-0.3.1/documentation/build/html/_static/css/fonts/fontawesome-webfont.woff
--rw-r--r--   0 mhambley (10374) users     (1000)    77160 2022-04-04 15:40:50.000000 stylist-0.3.1/documentation/build/html/_static/css/fonts/fontawesome-webfont.woff2
--rw-r--r--   0 mhambley (10374) users     (1000)   323344 2022-04-04 15:40:50.000000 stylist-0.3.1/documentation/build/html/_static/css/fonts/lato-bold-italic.woff
--rw-r--r--   0 mhambley (10374) users     (1000)   193308 2022-04-04 15:40:50.000000 stylist-0.3.1/documentation/build/html/_static/css/fonts/lato-bold-italic.woff2
--rw-r--r--   0 mhambley (10374) users     (1000)   309728 2022-04-04 15:40:50.000000 stylist-0.3.1/documentation/build/html/_static/css/fonts/lato-bold.woff
--rw-r--r--   0 mhambley (10374) users     (1000)   184912 2022-04-04 15:40:50.000000 stylist-0.3.1/documentation/build/html/_static/css/fonts/lato-bold.woff2
--rw-r--r--   0 mhambley (10374) users     (1000)   328412 2022-04-04 15:40:50.000000 stylist-0.3.1/documentation/build/html/_static/css/fonts/lato-normal-italic.woff
--rw-r--r--   0 mhambley (10374) users     (1000)   195704 2022-04-04 15:40:50.000000 stylist-0.3.1/documentation/build/html/_static/css/fonts/lato-normal-italic.woff2
--rw-r--r--   0 mhambley (10374) users     (1000)   309192 2022-04-04 15:40:50.000000 stylist-0.3.1/documentation/build/html/_static/css/fonts/lato-normal.woff
--rw-r--r--   0 mhambley (10374) users     (1000)   182708 2022-04-04 15:40:50.000000 stylist-0.3.1/documentation/build/html/_static/css/fonts/lato-normal.woff2
--rw-r--r--   0 mhambley (10374) users     (1000)   129674 2022-04-04 15:40:50.000000 stylist-0.3.1/documentation/build/html/_static/css/theme.css
--rw-r--r--   0 mhambley (10374) users     (1000)    10766 2022-04-04 08:21:05.000000 stylist-0.3.1/documentation/build/html/_static/doctools.js
--rw-r--r--   0 mhambley (10374) users     (1000)      425 2022-08-11 12:34:45.000000 stylist-0.3.1/documentation/build/html/_static/documentation_options.js
--rw-r--r--   0 mhambley (10374) users     (1000)      286 2022-04-04 08:21:05.000000 stylist-0.3.1/documentation/build/html/_static/file.png
--rw-r--r--   0 mhambley (10374) users     (1000)   287630 2022-04-04 08:21:05.000000 stylist-0.3.1/documentation/build/html/_static/jquery-3.5.1.js
--rw-r--r--   0 mhambley (10374) users     (1000)    89476 2022-04-04 08:21:05.000000 stylist-0.3.1/documentation/build/html/_static/jquery.js
-drwxr-xr-x   0 mhambley (10374) users     (1000)        0 2022-12-01 15:44:13.000000 stylist-0.3.1/documentation/build/html/_static/js/
--rw-r--r--   0 mhambley (10374) users     (1000)      934 2022-04-04 15:40:50.000000 stylist-0.3.1/documentation/build/html/_static/js/badge_only.js
--rw-r--r--   0 mhambley (10374) users     (1000)     4370 2022-04-04 15:40:50.000000 stylist-0.3.1/documentation/build/html/_static/js/html5shiv-printshiv.min.js
--rw-r--r--   0 mhambley (10374) users     (1000)     2734 2022-04-04 15:40:50.000000 stylist-0.3.1/documentation/build/html/_static/js/html5shiv.min.js
--rw-r--r--   0 mhambley (10374) users     (1000)     5023 2022-04-04 15:40:50.000000 stylist-0.3.1/documentation/build/html/_static/js/theme.js
--rw-r--r--   0 mhambley (10374) users     (1000)    10854 2022-08-11 12:34:45.000000 stylist-0.3.1/documentation/build/html/_static/language_data.js
--rw-r--r--   0 mhambley (10374) users     (1000)       90 2022-04-04 08:21:05.000000 stylist-0.3.1/documentation/build/html/_static/minus.png
--rw-r--r--   0 mhambley (10374) users     (1000)       90 2022-04-04 08:21:05.000000 stylist-0.3.1/documentation/build/html/_static/plus.png
--rw-r--r--   0 mhambley (10374) users     (1000)     4819 2022-08-11 12:34:45.000000 stylist-0.3.1/documentation/build/html/_static/pygments.css
--rw-r--r--   0 mhambley (10374) users     (1000)    16634 2022-04-04 08:21:05.000000 stylist-0.3.1/documentation/build/html/_static/searchtools.js
--rw-r--r--   0 mhambley (10374) users     (1000)     3167 2022-08-10 10:05:46.000000 stylist-0.3.1/documentation/build/html/_static/stylist.png
--rw-r--r--   0 mhambley (10374) users     (1000)    68420 2022-04-04 08:21:05.000000 stylist-0.3.1/documentation/build/html/_static/underscore-1.13.1.js
--rw-r--r--   0 mhambley (10374) users     (1000)    19530 2022-04-04 08:21:05.000000 stylist-0.3.1/documentation/build/html/_static/underscore.js
-drwxr-xr-x   0 mhambley (10374) users     (1000)        0 2022-12-01 15:44:13.000000 stylist-0.3.1/documentation/build/html/developer-information/
-drwxr-xr-x   0 mhambley (10374) users     (1000)        0 2022-12-01 15:44:13.000000 stylist-0.3.1/documentation/build/html/developer-information/api/
--rw-r--r--   0 mhambley (10374) users     (1000)    21212 2022-08-11 09:31:00.000000 stylist-0.3.1/documentation/build/html/developer-information/api/stylist.configuration.html
--rw-r--r--   0 mhambley (10374) users     (1000)     9494 2022-08-11 09:31:00.000000 stylist-0.3.1/documentation/build/html/developer-information/api/stylist.engine.html
--rw-r--r--   0 mhambley (10374) users     (1000)    37364 2022-08-11 09:31:00.000000 stylist-0.3.1/documentation/build/html/developer-information/api/stylist.fortran.html
--rw-r--r--   0 mhambley (10374) users     (1000)    10011 2022-08-11 09:31:00.000000 stylist-0.3.1/documentation/build/html/developer-information/api/stylist.html
--rw-r--r--   0 mhambley (10374) users     (1000)    12422 2022-08-11 09:31:00.000000 stylist-0.3.1/documentation/build/html/developer-information/api/stylist.issue.html
--rw-r--r--   0 mhambley (10374) users     (1000)    11281 2022-08-11 09:31:00.000000 stylist-0.3.1/documentation/build/html/developer-information/api/stylist.rule.html
--rw-r--r--   0 mhambley (10374) users     (1000)    57028 2022-08-11 09:31:00.000000 stylist-0.3.1/documentation/build/html/developer-information/api/stylist.source.html
--rw-r--r--   0 mhambley (10374) users     (1000)    13180 2022-08-11 09:31:00.000000 stylist-0.3.1/documentation/build/html/developer-information/api/stylist.style.html
--rw-r--r--   0 mhambley (10374) users     (1000)     5955 2022-08-11 09:31:00.000000 stylist-0.3.1/documentation/build/html/developer-information/api.html
--rw-r--r--   0 mhambley (10374) users     (1000)     8954 2022-08-11 09:31:01.000000 stylist-0.3.1/documentation/build/html/developer-information/environment.html
--rw-r--r--   0 mhambley (10374) users     (1000)     7785 2022-08-11 09:56:22.000000 stylist-0.3.1/documentation/build/html/developer-information/index.html
--rw-r--r--   0 mhambley (10374) users     (1000)     5316 2022-08-11 09:31:01.000000 stylist-0.3.1/documentation/build/html/developer-information/new-rules.html
--rw-r--r--   0 mhambley (10374) users     (1000)    10727 2022-08-11 09:54:55.000000 stylist-0.3.1/documentation/build/html/developer-information/overview.html
--rw-r--r--   0 mhambley (10374) users     (1000)    10856 2022-08-11 09:56:22.000000 stylist-0.3.1/documentation/build/html/developer-information/rules.html
--rw-r--r--   0 mhambley (10374) users     (1000)    13937 2022-08-11 09:47:32.000000 stylist-0.3.1/documentation/build/html/developer-information/structure.html
--rw-r--r--   0 mhambley (10374) users     (1000)     6459 2022-08-11 09:31:01.000000 stylist-0.3.1/documentation/build/html/developer-information/todo.html
--rw-r--r--   0 mhambley (10374) users     (1000)    23250 2022-08-11 12:34:45.000000 stylist-0.3.1/documentation/build/html/genindex.html
--rw-r--r--   0 mhambley (10374) users     (1000)     6778 2022-08-11 12:34:45.000000 stylist-0.3.1/documentation/build/html/index.html
--rw-r--r--   0 mhambley (10374) users     (1000)     1318 2022-08-11 12:34:45.000000 stylist-0.3.1/documentation/build/html/objects.inv
--rw-r--r--   0 mhambley (10374) users     (1000)     5746 2022-08-11 12:34:45.000000 stylist-0.3.1/documentation/build/html/py-modindex.html
--rw-r--r--   0 mhambley (10374) users     (1000)     3887 2022-08-11 12:34:45.000000 stylist-0.3.1/documentation/build/html/search.html
--rw-r--r--   0 mhambley (10374) users     (1000)    16499 2022-08-11 12:34:45.000000 stylist-0.3.1/documentation/build/html/searchindex.js
-drwxr-xr-x   0 mhambley (10374) users     (1000)        0 2022-12-01 15:44:13.000000 stylist-0.3.1/documentation/build/html/user-manual/
--rw-r--r--   0 mhambley (10374) users     (1000)     7357 2022-08-11 12:13:10.000000 stylist-0.3.1/documentation/build/html/user-manual/configuration.html
--rw-r--r--   0 mhambley (10374) users     (1000)     6393 2022-08-11 12:34:45.000000 stylist-0.3.1/documentation/build/html/user-manual/index.html
--rw-r--r--   0 mhambley (10374) users     (1000)     9529 2022-08-11 09:31:01.000000 stylist-0.3.1/documentation/build/html/user-manual/preparation.html
--rw-r--r--   0 mhambley (10374) users     (1000)    13205 2022-08-11 09:31:01.000000 stylist-0.3.1/documentation/build/html/user-manual/rule-list.html
-drwxr-xr-x   0 mhambley (10374) users     (1000)        0 2022-12-01 15:44:13.000000 stylist-0.3.1/documentation/source/
-drwxr-xr-x   0 mhambley (10374) users     (1000)        0 2022-12-01 15:44:13.000000 stylist-0.3.1/documentation/source/_static/
--rwxr-xr-x   0 mhambley (10374) users     (1000)     3167 2022-08-10 10:05:46.000000 stylist-0.3.1/documentation/source/_static/stylist.png
--rw-r--r--   0 mhambley (10374) users     (1000)     2651 2022-08-10 10:05:46.000000 stylist-0.3.1/documentation/source/conf.py
-drwxr-xr-x   0 mhambley (10374) users     (1000)        0 2022-12-01 15:44:13.000000 stylist-0.3.1/documentation/source/developer-information/
-drwxr-xr-x   0 mhambley (10374) users     (1000)        0 2022-12-01 15:44:13.000000 stylist-0.3.1/documentation/source/developer-information/api/
--rw-r--r--   0 mhambley (10374) users     (1000)      234 2022-08-11 09:30:57.000000 stylist-0.3.1/documentation/source/developer-information/api/stylist.configuration.rst
--rw-r--r--   0 mhambley (10374) users     (1000)      187 2022-08-11 09:30:58.000000 stylist-0.3.1/documentation/source/developer-information/api/stylist.engine.rst
--rw-r--r--   0 mhambley (10374) users     (1000)      388 2022-08-11 09:30:58.000000 stylist-0.3.1/documentation/source/developer-information/api/stylist.fortran.rst
--rw-r--r--   0 mhambley (10374) users     (1000)      178 2022-08-11 09:30:58.000000 stylist-0.3.1/documentation/source/developer-information/api/stylist.issue.rst
--rw-r--r--   0 mhambley (10374) users     (1000)      375 2022-08-11 09:30:57.000000 stylist-0.3.1/documentation/source/developer-information/api/stylist.rst
--rw-r--r--   0 mhambley (10374) users     (1000)      199 2022-08-11 09:30:58.000000 stylist-0.3.1/documentation/source/developer-information/api/stylist.rule.rst
--rw-r--r--   0 mhambley (10374) users     (1000)      551 2022-08-11 09:30:58.000000 stylist-0.3.1/documentation/source/developer-information/api/stylist.source.rst
--rw-r--r--   0 mhambley (10374) users     (1000)      254 2022-08-11 09:30:58.000000 stylist-0.3.1/documentation/source/developer-information/api/stylist.style.rst
--rw-r--r--   0 mhambley (10374) users     (1000)      176 2022-08-10 10:05:46.000000 stylist-0.3.1/documentation/source/developer-information/api.rst
--rw-r--r--   0 mhambley (10374) users     (1000)     1503 2022-08-22 12:48:22.000000 stylist-0.3.1/documentation/source/developer-information/environment.rst
--rw-r--r--   0 mhambley (10374) users     (1000)      639 2022-08-22 12:48:22.000000 stylist-0.3.1/documentation/source/developer-information/index.rst
--rw-r--r--   0 mhambley (10374) users     (1000)     3813 2022-08-22 12:48:22.000000 stylist-0.3.1/documentation/source/developer-information/overview.rst
--rw-r--r--   0 mhambley (10374) users     (1000)     1949 2022-08-22 12:48:22.000000 stylist-0.3.1/documentation/source/developer-information/rules.rst
--rw-r--r--   0 mhambley (10374) users     (1000)      182 2022-08-10 10:05:46.000000 stylist-0.3.1/documentation/source/developer-information/todo.rst
--rw-r--r--   0 mhambley (10374) users     (1000)     1036 2022-08-22 12:48:22.000000 stylist-0.3.1/documentation/source/index.rst
-drwxr-xr-x   0 mhambley (10374) users     (1000)        0 2022-12-01 15:44:13.000000 stylist-0.3.1/documentation/source/user-manual/
--rw-r--r--   0 mhambley (10374) users     (1000)     1624 2022-08-22 12:48:22.000000 stylist-0.3.1/documentation/source/user-manual/configuration.rst
--rw-r--r--   0 mhambley (10374) users     (1000)      571 2022-08-22 12:48:22.000000 stylist-0.3.1/documentation/source/user-manual/index.rst
--rw-r--r--   0 mhambley (10374) users     (1000)     2836 2022-08-15 13:13:43.000000 stylist-0.3.1/documentation/source/user-manual/preparation.rst
--rw-r--r--   0 mhambley (10374) users     (1000)     1949 2022-11-01 16:10:57.000000 stylist-0.3.1/documentation/source/user-manual/rule-list.rst
-drwxr-xr-x   0 mhambley (10374) users     (1000)        0 2022-12-01 15:44:13.000000 stylist-0.3.1/documentation/uml/
--rw-r--r--   0 mhambley (10374) users     (1000)     4899 2022-08-10 10:05:46.000000 stylist-0.3.1/documentation/uml/CheckerDesign.puml
--rw-r--r--   0 mhambley (10374) users     (1000)     2641 2022-08-10 10:05:46.000000 stylist-0.3.1/documentation/uml/StylerDesign.puml
--rw-r--r--   0 mhambley (10374) users     (1000)      708 2022-12-01 15:44:13.000000 stylist-0.3.1/setup.cfg
--rw-r--r--   0 mhambley (10374) users     (1000)     1296 2022-11-01 13:57:43.000000 stylist-0.3.1/setup.py
-drwxr-xr-x   0 mhambley (10374) users     (1000)        0 2022-12-01 15:44:12.000000 stylist-0.3.1/source/
-drwxr-xr-x   0 mhambley (10374) users     (1000)        0 2022-12-01 15:44:13.000000 stylist-0.3.1/source/stylist/
--rw-r--r--   0 mhambley (10374) users     (1000)      603 2022-12-01 15:43:44.000000 stylist-0.3.1/source/stylist/__init__.py
--rwxr-xr-x   0 mhambley (10374) users     (1000)     5972 2022-10-28 12:37:50.000000 stylist-0.3.1/source/stylist/__main__.py
--rw-r--r--   0 mhambley (10374) users     (1000)     3921 2022-08-15 13:13:43.000000 stylist-0.3.1/source/stylist/configuration.py
--rw-r--r--   0 mhambley (10374) users     (1000)     1544 2022-10-28 09:51:17.000000 stylist-0.3.1/source/stylist/engine.py
--rw-r--r--   0 mhambley (10374) users     (1000)    28811 2022-11-30 13:15:04.000000 stylist-0.3.1/source/stylist/fortran.py
--rw-r--r--   0 mhambley (10374) users     (1000)     1941 2022-10-28 09:51:17.000000 stylist-0.3.1/source/stylist/issue.py
--rw-r--r--   0 mhambley (10374) users     (1000)     1561 2022-10-29 13:59:38.000000 stylist-0.3.1/source/stylist/rule.py
--rw-r--r--   0 mhambley (10374) users     (1000)    19176 2022-10-28 12:37:50.000000 stylist-0.3.1/source/stylist/source.py
--rw-r--r--   0 mhambley (10374) users     (1000)     1697 2022-10-28 09:51:17.000000 stylist-0.3.1/source/stylist/style.py
-drwxr-xr-x   0 mhambley (10374) users     (1000)        0 2022-12-01 15:44:13.000000 stylist-0.3.1/source/stylist.egg-info/
--rw-r--r--   0 mhambley (10374) users     (1000)     5475 2022-12-01 15:44:12.000000 stylist-0.3.1/source/stylist.egg-info/PKG-INFO
--rw-r--r--   0 mhambley (10374) users     (1000)     8409 2022-12-01 15:44:12.000000 stylist-0.3.1/source/stylist.egg-info/SOURCES.txt
--rw-r--r--   0 mhambley (10374) users     (1000)        1 2022-12-01 15:44:12.000000 stylist-0.3.1/source/stylist.egg-info/dependency_links.txt
--rw-r--r--   0 mhambley (10374) users     (1000)       50 2022-12-01 15:44:12.000000 stylist-0.3.1/source/stylist.egg-info/entry_points.txt
--rw-r--r--   0 mhambley (10374) users     (1000)      167 2022-12-01 15:44:12.000000 stylist-0.3.1/source/stylist.egg-info/requires.txt
--rw-r--r--   0 mhambley (10374) users     (1000)        8 2022-12-01 15:44:12.000000 stylist-0.3.1/source/stylist.egg-info/top_level.txt
+drwxr-xr-x   0 mhambley (10374) users     (1000)        0 2023-04-25 15:22:38.000000 stylist-0.4.0/
+-rw-r--r--   0 mhambley (10374) users     (1000)     3215 2023-04-20 10:09:12.000000 stylist-0.4.0/CONTRIBUTING.md
+-rw-r--r--   0 mhambley (10374) users     (1000)     1550 2023-04-20 10:09:12.000000 stylist-0.4.0/LICENSE
+-rw-r--r--   0 mhambley (10374) users     (1000)      147 2023-04-20 10:09:12.000000 stylist-0.4.0/MANIFEST.in
+-rw-r--r--   0 mhambley (10374) users     (1000)     5404 2023-04-25 15:22:38.000000 stylist-0.4.0/PKG-INFO
+-rw-r--r--   0 mhambley (10374) users     (1000)     4666 2023-04-21 10:04:37.000000 stylist-0.4.0/README.rst
+drwxr-xr-x   0 mhambley (10374) users     (1000)        0 2023-04-25 15:22:38.000000 stylist-0.4.0/documentation/
+-rw-r--r--   0 mhambley (10374) users     (1000)       34 2023-04-20 10:09:12.000000 stylist-0.4.0/documentation/.gitignore
+-rw-r--r--   0 mhambley (10374) users     (1000)      630 2023-04-20 10:09:12.000000 stylist-0.4.0/documentation/Makefile
+drwxr-xr-x   0 mhambley (10374) users     (1000)        0 2023-04-25 15:22:38.000000 stylist-0.4.0/documentation/source/
+drwxr-xr-x   0 mhambley (10374) users     (1000)        0 2023-04-25 15:22:38.000000 stylist-0.4.0/documentation/source/_static/
+-rwxr-xr-x   0 mhambley (10374) users     (1000)     3167 2023-04-20 10:09:12.000000 stylist-0.4.0/documentation/source/_static/stylist.png
+-rw-r--r--   0 mhambley (10374) users     (1000)     2651 2023-04-20 10:09:12.000000 stylist-0.4.0/documentation/source/conf.py
+drwxr-xr-x   0 mhambley (10374) users     (1000)        0 2023-04-25 15:22:38.000000 stylist-0.4.0/documentation/source/developer-information/
+-rw-r--r--   0 mhambley (10374) users     (1000)      176 2023-04-20 10:09:12.000000 stylist-0.4.0/documentation/source/developer-information/api.rst
+-rw-r--r--   0 mhambley (10374) users     (1000)     1503 2023-04-20 10:09:12.000000 stylist-0.4.0/documentation/source/developer-information/environment.rst
+-rw-r--r--   0 mhambley (10374) users     (1000)      639 2023-04-20 10:09:12.000000 stylist-0.4.0/documentation/source/developer-information/index.rst
+-rw-r--r--   0 mhambley (10374) users     (1000)     3813 2023-04-20 10:09:12.000000 stylist-0.4.0/documentation/source/developer-information/overview.rst
+-rw-r--r--   0 mhambley (10374) users     (1000)     1949 2023-04-20 10:09:12.000000 stylist-0.4.0/documentation/source/developer-information/rules.rst
+-rw-r--r--   0 mhambley (10374) users     (1000)      182 2023-04-20 10:09:12.000000 stylist-0.4.0/documentation/source/developer-information/todo.rst
+-rw-r--r--   0 mhambley (10374) users     (1000)     1036 2023-04-20 10:09:12.000000 stylist-0.4.0/documentation/source/index.rst
+drwxr-xr-x   0 mhambley (10374) users     (1000)        0 2023-04-25 15:22:38.000000 stylist-0.4.0/documentation/source/user-manual/
+-rw-r--r--   0 mhambley (10374) users     (1000)     1624 2023-04-20 10:09:12.000000 stylist-0.4.0/documentation/source/user-manual/configuration.rst
+-rw-r--r--   0 mhambley (10374) users     (1000)      571 2023-04-20 10:09:12.000000 stylist-0.4.0/documentation/source/user-manual/index.rst
+-rw-r--r--   0 mhambley (10374) users     (1000)     2836 2023-04-20 10:09:12.000000 stylist-0.4.0/documentation/source/user-manual/preparation.rst
+-rw-r--r--   0 mhambley (10374) users     (1000)     1949 2023-04-21 10:04:37.000000 stylist-0.4.0/documentation/source/user-manual/rule-list.rst
+drwxr-xr-x   0 mhambley (10374) users     (1000)        0 2023-04-25 15:22:38.000000 stylist-0.4.0/documentation/uml/
+-rw-r--r--   0 mhambley (10374) users     (1000)     4899 2023-04-20 10:09:12.000000 stylist-0.4.0/documentation/uml/CheckerDesign.puml
+-rw-r--r--   0 mhambley (10374) users     (1000)     2641 2023-04-20 10:09:12.000000 stylist-0.4.0/documentation/uml/StylerDesign.puml
+-rw-r--r--   0 mhambley (10374) users     (1000)     1078 2023-04-24 08:29:13.000000 stylist-0.4.0/pyproject.toml
+-rw-r--r--   0 mhambley (10374) users     (1000)      708 2023-04-25 15:22:38.000000 stylist-0.4.0/setup.cfg
+drwxr-xr-x   0 mhambley (10374) users     (1000)        0 2023-04-25 15:22:38.000000 stylist-0.4.0/source/
+drwxr-xr-x   0 mhambley (10374) users     (1000)        0 2023-04-25 15:22:38.000000 stylist-0.4.0/source/stylist/
+-rw-r--r--   0 mhambley (10374) users     (1000)      603 2023-04-25 15:08:10.000000 stylist-0.4.0/source/stylist/__init__.py
+-rwxr-xr-x   0 mhambley (10374) users     (1000)     5901 2023-04-21 10:04:37.000000 stylist-0.4.0/source/stylist/__main__.py
+-rw-r--r--   0 mhambley (10374) users     (1000)     3929 2023-04-24 08:28:48.000000 stylist-0.4.0/source/stylist/configuration.py
+-rw-r--r--   0 mhambley (10374) users     (1000)     1547 2023-04-21 10:04:37.000000 stylist-0.4.0/source/stylist/engine.py
+-rw-r--r--   0 mhambley (10374) users     (1000)    29774 2023-04-24 08:28:48.000000 stylist-0.4.0/source/stylist/fortran.py
+-rw-r--r--   0 mhambley (10374) users     (1000)     2564 2023-04-21 10:04:37.000000 stylist-0.4.0/source/stylist/issue.py
+-rw-r--r--   0 mhambley (10374) users     (1000)     2470 2023-04-21 10:04:37.000000 stylist-0.4.0/source/stylist/rule.py
+-rw-r--r--   0 mhambley (10374) users     (1000)    18911 2023-04-24 08:28:48.000000 stylist-0.4.0/source/stylist/source.py
+-rw-r--r--   0 mhambley (10374) users     (1000)     1671 2023-04-21 10:04:37.000000 stylist-0.4.0/source/stylist/style.py
+drwxr-xr-x   0 mhambley (10374) users     (1000)        0 2023-04-25 15:22:38.000000 stylist-0.4.0/source/stylist.egg-info/
+-rw-r--r--   0 mhambley (10374) users     (1000)     5404 2023-04-25 15:22:38.000000 stylist-0.4.0/source/stylist.egg-info/PKG-INFO
+-rw-r--r--   0 mhambley (10374) users     (1000)     1270 2023-04-25 15:22:38.000000 stylist-0.4.0/source/stylist.egg-info/SOURCES.txt
+-rw-r--r--   0 mhambley (10374) users     (1000)        1 2023-04-25 15:22:38.000000 stylist-0.4.0/source/stylist.egg-info/dependency_links.txt
+-rw-r--r--   0 mhambley (10374) users     (1000)       50 2023-04-25 15:22:38.000000 stylist-0.4.0/source/stylist.egg-info/entry_points.txt
+-rw-r--r--   0 mhambley (10374) users     (1000)      216 2023-04-25 15:22:38.000000 stylist-0.4.0/source/stylist.egg-info/requires.txt
+-rw-r--r--   0 mhambley (10374) users     (1000)        8 2023-04-25 15:22:38.000000 stylist-0.4.0/source/stylist.egg-info/top_level.txt
```

### Comparing `stylist-0.3.1/CONTRIBUTING.md` & `stylist-0.4.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `stylist-0.3.1/LICENSE` & `stylist-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stylist-0.3.1/PKG-INFO` & `stylist-0.4.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,33 @@
 Metadata-Version: 2.1
 Name: stylist
-Version: 0.3.1
-Summary: Extensible code style checker currently supporting Fortran, PSyclone DSL, etc
+Version: 0.4.0
+Summary: Flexible source code style checking tool
 Home-page: https://github.com/MetOffice/stylist
 Author: Met Office
-License: BSD 3-Clause
+License: BSD 3-Clause License
+Project-URL: homepage, https://github.com/MetOffice/stylist/
+Project-URL: documentation, https://metoffice.github.io/stylist
 Project-URL: Bug Reports, https://github.com/MetOffice/stylist/issues
-Project-URL: Source, https://github.com/MetOffice/stylist/
+Project-URL: repository, https://github.com/MetOffice/stylist/
 Keywords: linter fortran psyclone
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Quality Assurance
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7, <4
+Classifier: Programming Language :: Python :: 3
+Requires-Python: <4,>=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 Provides-Extra: test
+Provides-Extra: performance
 Provides-Extra: docs
 Provides-Extra: release
 License-File: LICENSE
 
 Stylist
 =======
 
-|BSD3 License| |GitHub release| |PyPI version| |GitHub merge testing|
+|BSD3 License| |GitHub release| |PyPI version| |Conda version| |GitHub merge testing|
 
 Stylist is a tool for checking code style. It implements a framework which
 supports multiple styles across multiple languages.
 
 But aren't there many such tools out there, why create a new one?
 
 The simple reason is that few of them support Fortran, a language still in
@@ -56,27 +52,30 @@
 
 .. |GitHub release| image:: https://img.shields.io/github/release/MetOffice/stylist.svg
    :target: https://github.com/MetOffice/stylist/
 
 .. |PyPI version| image:: https://badge.fury.io/py/stylist.svg
    :target: https://pypi.python.org/pypi/stylist/
 
+.. |Conda version| image:: https://img.shields.io/conda/vn/conda-forge/stylist.svg
+   :target: https://anaconda.org/conda-forge/stylist
+
 .. |GitHub merge testing| image:: https://github.com/MetOffice/stylist/workflows/Merge%20Test/badge.svg
    :target: https://github.com/MetOffice/stylist/actions
 
 
 Installation
 ~~~~~~~~~~~~
 
 Installation can be as simple as ``pip install stylist`` or
 ``conda install -c conda-forge stylist``.
 
-As always it is also possible to install from the project source by running
-``python setup.py``. The source may be obtained by downloading a tarball or by
-cloning the repository.
+As always it is also possible to install from the project source using
+``pip install --editable .``. The source may be obtained by downloading a
+tarball or by cloning the repository.
 
 
 Usage
 ~~~~~
 
 Stylist provides a command-line tool ``stylist`` for normal use. It can also be
 used as a package if you want to integrate it with another tool. Documentation
@@ -138,10 +137,10 @@
 
 An illustrative example::
 
   from re import compile as recompile
   from stylist.style import Style
   from stylist.fortran import FortranCharacterset, KindPattern
   
-  simple = Style(FortranCharactersest(),
+  simple = Style(FortranCharacterset(),
                  KindPattern(integer=recompile(r'i_.+'),
-                             real=recompile(r'r_.+'))
+                             real=recompile(r'r_.+')))
```

### Comparing `stylist-0.3.1/README.rst` & `stylist-0.4.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Stylist
 =======
 
-|BSD3 License| |GitHub release| |PyPI version| |GitHub merge testing|
+|BSD3 License| |GitHub release| |PyPI version| |Conda version| |GitHub merge testing|
 
 Stylist is a tool for checking code style. It implements a framework which
 supports multiple styles across multiple languages.
 
 But aren't there many such tools out there, why create a new one?
 
 The simple reason is that few of them support Fortran, a language still in
@@ -30,27 +30,30 @@
 
 .. |GitHub release| image:: https://img.shields.io/github/release/MetOffice/stylist.svg
    :target: https://github.com/MetOffice/stylist/
 
 .. |PyPI version| image:: https://badge.fury.io/py/stylist.svg
    :target: https://pypi.python.org/pypi/stylist/
 
+.. |Conda version| image:: https://img.shields.io/conda/vn/conda-forge/stylist.svg
+   :target: https://anaconda.org/conda-forge/stylist
+
 .. |GitHub merge testing| image:: https://github.com/MetOffice/stylist/workflows/Merge%20Test/badge.svg
    :target: https://github.com/MetOffice/stylist/actions
 
 
 Installation
 ~~~~~~~~~~~~
 
 Installation can be as simple as ``pip install stylist`` or
 ``conda install -c conda-forge stylist``.
 
-As always it is also possible to install from the project source by running
-``python setup.py``. The source may be obtained by downloading a tarball or by
-cloning the repository.
+As always it is also possible to install from the project source using
+``pip install --editable .``. The source may be obtained by downloading a
+tarball or by cloning the repository.
 
 
 Usage
 ~~~~~
 
 Stylist provides a command-line tool ``stylist`` for normal use. It can also be
 used as a package if you want to integrate it with another tool. Documentation
@@ -112,10 +115,10 @@
 
 An illustrative example::
 
   from re import compile as recompile
   from stylist.style import Style
   from stylist.fortran import FortranCharacterset, KindPattern
   
-  simple = Style(FortranCharactersest(),
+  simple = Style(FortranCharacterset(),
                  KindPattern(integer=recompile(r'i_.+'),
-                             real=recompile(r'r_.+'))
+                             real=recompile(r'r_.+')))
```

### Comparing `stylist-0.3.1/documentation/Makefile` & `stylist-0.4.0/documentation/Makefile`

 * *Files identical despite different names*

### Comparing `stylist-0.3.1/documentation/build/html/_sources/developer-information/environment.rst.txt` & `stylist-0.4.0/documentation/source/developer-information/environment.rst`

 * *Files identical despite different names*

### Comparing `stylist-0.3.1/documentation/build/html/_sources/developer-information/index.rst.txt` & `stylist-0.4.0/documentation/source/developer-information/index.rst`

 * *Files identical despite different names*

### Comparing `stylist-0.3.1/documentation/build/html/_sources/developer-information/overview.rst.txt` & `stylist-0.4.0/documentation/source/developer-information/overview.rst`

 * *Files identical despite different names*

### Comparing `stylist-0.3.1/documentation/build/html/_sources/developer-information/rules.rst.txt` & `stylist-0.4.0/documentation/source/developer-information/rules.rst`

 * *Files identical despite different names*

### Comparing `stylist-0.3.1/documentation/build/html/_sources/index.rst.txt` & `stylist-0.4.0/documentation/source/index.rst`

 * *Files identical despite different names*

### Comparing `stylist-0.3.1/documentation/build/html/_sources/user-manual/configuration.rst.txt` & `stylist-0.4.0/documentation/source/user-manual/configuration.rst`

 * *Files identical despite different names*

### Comparing `stylist-0.3.1/documentation/build/html/_sources/user-manual/index.rst.txt` & `stylist-0.4.0/documentation/source/user-manual/index.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 User Manual
 ===========
 
 Welcome to the **Stylist** code style checking tool.
 
 The goal of this tool is to provide a flexible way of checking source code
-against a set of rules. Rather than require that you adopt a particular set of
-rules it aims to offer you the chance to build up the style you like.
+against a set of rules. Rather than require that you adopt a particular style
+laid down by the Stylist developers it aims to offer you the chance to build
+up the one you like.
 
 The need to check Fortran source motivated the creation of this tool. As such
 Fortran is currently the only language supported but there is no reason it
 would not work for others.
 
 .. toctree::
```

### Comparing `stylist-0.3.1/documentation/build/html/_sources/user-manual/preparation.rst.txt` & `stylist-0.4.0/documentation/source/user-manual/preparation.rst`

 * *Files 17% similar despite different names*

```diff
@@ -13,42 +13,66 @@
 .. _PyPI: https://pypi.org/project/stylist/
 .. _CondaForge: https://anaconda.org/conda-forge/stylist
 
 Getting started
 ---------------
 
 With the tool installed and available you will need to create a configuration
-for your project. This is a simple Windows ``.ini`` format file. At a minimum
-it should define a style of at least one rule.
+for your project. This is a simple Python script which defines suitable
+variables. At a minimum it should define a style of at least one rule.
 
-For example, create a file called ``stylist.ini`` containing::
+For example, create a file called ``stylist.py`` containing::
 
-    [style.simple]
-    rules = MissingImplicit
+    from stylist.fortran import MissingImplicit
+    from stylist.style import Style
+
+    simple = Style(MissingImplicit())
 
 You may then check your source code using this style with::
 
-    stylist -configuration stylist.ini <path to source>
+    stylist -configuration stylist.py <path to source>
 
 The tool will alert you to any place where a program unit has been declared
 without an ``implicit`` statement.
 
-The "rules" field is a comma-separated list so to add a second rule just append
-``, MissingIntent``. Running the tool again will now warn you of both missing
-``implicit`` statements and procedure arguments without ``intent`` properties.
+The Style object is constructed with all the rules which make up that style.
+To add a second rule just import it and append ``, MissingIntent()`` to the
+argument list::
+
+    from stylist.fortran import MissingImplicit, MissingIntent
+    from stylist.style import Style
+
+    simple = Style(MissingImplicit(), MissingIntent())
+
+Running the tool again will now warn you of both missing ``implicit``
+statements and procedure arguments without ``intent`` properties.
 
 You may define as many styles as you like in the configuration file. Lets add
-a second to our example. Just add the following at the end::
+a second to our example. Just extend the import and add the following at the
+end::
 
-    [style.extra]
-    rules = FortranCharacterset
+    extra = Style(FortranCharacterset())
 
 If the tool is given no guidance it will always choose the first style in the
 configuration. If you want to use a different style (or be explicit) you can
 use::
 
-    stylist -configuration stylist.ini -style extra <path to source>
+    stylist -configuration stylist.py -style extra <path to source>
 
 Some rules take arguments. Let's get bossy about the names which can be used
-for type kinds. To the "extra" rules add
-``, KindPattern(integer=r'i_.*', real=r'r_.*')``. This requires that all
-integer kinds start with "i\_" and all real kinds start with "r\_".
+for type kinds::
+
+    from re import compile as recompile
+    from stylist.rule import (MissingImplicit,
+                              MissingIntent,
+                              FortranCharacterset,
+                              KindPattern)
+    from stylist.style import Style
+
+    simple = Style(MissingImplicit(), MissingIntent())
+
+    extra = Style(FortranCharacterset(),
+                  KindPattern(integer=recompile(r'i_.*'),
+                              real=recompile(r'r_.*')))
+
+This requires that all integer kinds start with "i\_" and all real kinds
+start with "r\_".
```

### Comparing `stylist-0.3.1/documentation/build/html/_sources/user-manual/rule-list.rst.txt` & `stylist-0.4.0/documentation/source/user-manual/rule-list.rst`

 * *Files 16% similar despite different names*

```diff
@@ -22,14 +22,19 @@
 Rules relating to Fortran source code.
 
 .. autoclass:: stylist.fortran.AutoCharArrayIntent
    :noindex:
    :no-show-inheritance:
    :exclude-members: examine, examine_fortran
 
+.. autoclass:: stylist.fortran.ForbidUsage
+   :noindex:
+   :no-show-inheritance:
+   :exclude-members: examine, examine_fortran
+
 .. autoclass:: stylist.fortran.FortranCharacterset
    :noindex:
    :no-show-inheritance:
    :exclude-members: examine, examine_fortran
 
 .. autoclass:: stylist.fortran.IntrinsicModule
    :noindex:
@@ -61,7 +66,12 @@
    :no-show-inheritance:
    :exclude-members: examine, examine_fortran
 
 .. autoclass:: stylist.fortran.MissingPointerInit
    :noindex:
    :no-show-inheritance:
    :exclude-members: examine, examine_fortran
+
+.. autoclass:: stylist.fortran.NakedLiteral
+   :noindex:
+   :no-show-inheritance:
+   :exclude-members: examine, examine_fortran
```

### Comparing `stylist-0.3.1/documentation/build/html/_static/stylist.png` & `stylist-0.4.0/documentation/source/_static/stylist.png`

 * *Files identical despite different names*

### Comparing `stylist-0.3.1/documentation/source/conf.py` & `stylist-0.4.0/documentation/source/conf.py`

 * *Files identical despite different names*

### Comparing `stylist-0.3.1/documentation/uml/CheckerDesign.puml` & `stylist-0.4.0/documentation/uml/CheckerDesign.puml`

 * *Files identical despite different names*

### Comparing `stylist-0.3.1/documentation/uml/StylerDesign.puml` & `stylist-0.4.0/documentation/uml/StylerDesign.puml`

 * *Files identical despite different names*

### Comparing `stylist-0.3.1/setup.cfg` & `stylist-0.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `stylist-0.3.1/source/stylist/__init__.py` & `stylist-0.4.0/source/stylist/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # The file LICENCE, distributed with this code, contains details of the terms
 # under which the code may be used.
 ##############################################################################
 """
 Extensible code style checker currently supporting Fortran, PSyclone DSL, etc
 """
 
-__version__ = '0.3.1'
+__version__ = '0.4.0'
 
 
 class StylistException(Exception):
     """
     Allows exceptions from stylist to be distinguished from other exceptions.
     """
     pass
```

### Comparing `stylist-0.3.1/source/stylist/__main__.py` & `stylist-0.4.0/source/stylist/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 ##############################################################################
 """
 Tool for checking code style.
 """
 import argparse
 import logging
 from os import linesep
-import os.path
 from pathlib import Path
 import sys
 from textwrap import indent
 from typing import List, Sequence
 
 from stylist import StylistException
 from stylist.configuration import (Configuration,
@@ -31,20 +30,20 @@
     Parse the command line for stylist arguments.
     """
     description = 'Perform various code style checks on source code.'
 
     max_key_len: int = max(len(key) for key in ConfigTools.language_keys())
     parsers = [key.ljust(max_key_len)
                + ' - '
-               + str(ConfigTools.language(key))
+               + ConfigTools.language(key).get_name()
                for key in ConfigTools.language_keys()]
     max_key_len = max(len(key) for key in ConfigTools.preprocessor_keys())
     preproc = [key.ljust(max_key_len)
                + ' - '
-               + str(ConfigTools.preprocessor(key))
+               + ConfigTools.preprocessor(key).get_name()
                for key in ConfigTools.preprocessor_keys()]
     epilog = f"""
 IDs used in specifying extension pipelines:
   Parsers:
 {indent(linesep.join(parsers), '    ')}
   Preprocessors:
 {indent(linesep.join(preproc), '    ')}
@@ -58,56 +57,55 @@
     cli_parser.add_argument('-help', '-h', '--help', action='help')
     cli_parser.add_argument('-verbose', action="store_true",
                             help="Produce a running commentary on progress.")
     cli_parser.add_argument('-configuration',
                             type=Path,
                             metavar='FILENAME',
                             help="File which configures the tool.")
-    help = "Style to use for check. May be specified repeatedly."
+    message = "Style to use for check. May be specified repeatedly."
     cli_parser.add_argument('-style',
                             action='append',
                             metavar='NAME',
-                            help=help)
+                            help=message)
     message = 'Add a mapping between file extension and pipeline'
     cli_parser.add_argument('-map-extension',
                             metavar='EXTENSION:PARSER[:PREPROCESSOR]...',
                             dest='map_extension',
                             default=[],
                             action='append',
                             help=message)
     cli_parser.add_argument('source', metavar='FILE', nargs='+',
+                            type=Path,
                             help='Filename of source file or directory')
 
     arguments = cli_parser.parse_args()
 
     return arguments
 
 
-def _process(candidates: List[str], styles: Sequence[Style]) -> List[Issue]:
+def _process(candidates: List[Path], styles: Sequence[Style]) -> List[Issue]:
     """
     Examines files for style compliance.
 
     Any directories specified will be descended looking for files to examine.
     """
     engine = CheckEngine(styles)
 
     hot_extensions = SourceFactory.get_extensions()
 
     issues: List[Issue] = []
     while candidates:
-        filename = candidates.pop(0).strip()
-        if os.path.isdir(filename):
-            for leaf in os.listdir(filename):
-                leaf_filename = os.path.join(filename, leaf)
-                _, extension = os.path.splitext(leaf_filename)
-                if extension[1:] in hot_extensions \
-                   or os.path.isdir(leaf_filename):
+        file_object = candidates.pop(0)
+        if file_object.is_dir():
+            for leaf_filename in file_object.iterdir():
+                if leaf_filename.suffix[1:] in hot_extensions \
+                   or leaf_filename.is_dir():
                     candidates.append(leaf_filename)
         else:  # Is a file
-            issues.extend(engine.check(filename))
+            issues.extend(engine.check(file_object))
 
     return issues
 
 
 def _configure(project_file: Path) -> Configuration:
     configuration = load_configuration(project_file)
     # TODO /etc/fab.ini
```

### Comparing `stylist-0.3.1/source/stylist/configuration.py` & `stylist-0.4.0/source/stylist/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
                             PlainText,
                             SourceTree,
                             TextProcessor)
 from stylist.style import Style
 
 
 class Configuration:
-    def __init__(self):
+    def __init__(self) -> None:
         self._pipes: Dict[str, FilePipe] = {}
         self._styles: Dict[str, Style] = {}
 
     def add_pipe(self, extension: str, pipe: FilePipe):
         self._pipes[extension] = pipe
 
     def add_style(self, name: str, style: Style):
```

### Comparing `stylist-0.3.1/source/stylist/engine.py` & `stylist-0.4.0/source/stylist/engine.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,40 +4,42 @@
 # The file LICENCE, distributed with this code, contains details of the terms
 # under which the code may be used.
 ##############################################################################
 """
 Core of the style checking tool.
 """
 import logging
+from pathlib import Path
 from typing import Sequence
 
 from stylist.issue import Issue
 from stylist.source import SourceFactory
 from stylist.style import Style
 
 
-class CheckEngine(object):
+class CheckEngine:
     """
     Manages the checking of source files against style lists.
     """
     def __init__(self, styles: Sequence[Style]) -> None:
         """
         :param styles: Styles to use when checking source.
         """
         self._styles = styles
 
-    def check(self, source_filename: str) -> Sequence[Issue]:
+    def check(self, source_filename: Path) -> Sequence[Issue]:
         """
         Passes the eyes of all registered style lists over the source file.
 
-        :param source_filename: Path to source file.
+        :param source_filename: File to be checked.
         """
         issues = []
         with open(source_filename, 'rt') as source_file:
-            logging.getLogger(__name__).info('Examining: ' + source_filename)
+            message = f"Examining: {str(source_filename)}"
+            logging.getLogger(__name__).info(message)
             source = SourceFactory.read_file(source_file)
             for astyle in self._styles:
                 for new_issue in astyle.check(source):
                     new_issue.set_filename(source_filename)
                     issues.append(new_issue)
-        issues.sort(key=lambda x: (x.filename, x.line, x.description))
+        issues.sort()
         return issues
```

### Comparing `stylist-0.3.1/source/stylist/fortran.py` & `stylist-0.4.0/source/stylist/fortran.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # The file LICENCE, distributed with this code, contains details of the terms
 # under which the code may be used.
 ##############################################################################
 """
 Rules relating to Fortran source.
 """
 import re
-from abc import ABCMeta, abstractmethod
+from abc import ABC, abstractmethod
 from collections import defaultdict
 from typing import (Container, Dict, List, Optional, Pattern, Sequence, Type,
                     Union)
 
 import fparser.two.Fortran2003 as Fortran2003  # type: ignore
 import fparser.two.Fortran2008 as Fortran2008  # type: ignore
 from fparser.two.utils import (get_child as fp_get_child,  # type: ignore
@@ -33,15 +33,15 @@
     """
     target = node
     while target.item is None:
         target = target.parent
     return target.item.span[0]
 
 
-class FortranRule(Rule, metaclass=ABCMeta):
+class FortranRule(Rule, ABC):
     """
     Parent for style rules pertaining to Fortran source.
     """
 
     def examine(self, subject: FortranSource) -> List[Issue]:
         """
         Base for rules which scruitinise the parse tree of Fortran source.
@@ -161,16 +161,19 @@
         if self._require_everywhere:
             scope_units.extend(subject.path(['Main_Program',
                                              'Internal_Subprogram_Part',
                                              'Internal_Subprogram']))
             scope_units.extend(subject.path(['Module',
                                              'Module_Subprogram_Part',
                                              'Module_Subprogram']))
+        filtered_units = filter(lambda s: not isinstance(s,
+                                                         Fortran2003.Comment),
+                                scope_units)
         scope: Fortran2003.Block
-        for scope in scope_units:
+        for scope in filtered_units:
             scope_statement = subject.get_first_statement(root=scope)
 
             implication = subject.path(['Specification_Part',
                                         'Implicit_Part',
                                         'Implicit_Stmt'],
                                        root=scope.content[1:])
             if not implication:
@@ -187,15 +190,15 @@
     """
     Catches cases where a function or subroutine's dummy arguments don't
     have specified intent.
     """
 
     def examine_fortran(self, subject: FortranSource) -> List[Issue]:
         issues: List[Issue] = []
-        scope_units: List[Fortran2003.Block] = []
+        scope_units: List[Fortran2003.Base] = []
 
         # get all subprograms (functions and subroutines) within programs
         scope_units.extend(subject.path(['Main_Program',
                                          'Internal_Subprogram_Part',
                                          'Internal_Subprogram']))
 
         # get all subprograms within modules
@@ -233,26 +236,41 @@
             if specs is not None:
                 for spec in specs.children:
                     if spec.__class__ == Fortran2008.Type_Declaration_Stmt:
 
                         # check if type declaration has an intent
                         attributes = spec.children[1]
                         if attributes is not None:
-                            for attribute in spec.children[1].children:
-                                if attribute.__class__ == \
-                                        Fortran2003.Intent_Attr_Spec:
+                            for attribute in attributes.children:
+                                if attribute.__class__ \
+                                        == Fortran2003.Intent_Attr_Spec:
 
                                     # if so, remove argument names from
                                     # dummy_args
                                     for arg in spec.children[2].children:
                                         arg_name = arg.children[
                                             0].string.lower()
                                         if arg_name in dummy_args:
                                             dummy_args.remove(arg_name)
 
+                    elif spec.__class__ \
+                            == Fortran2003.Procedure_Declaration_Stmt:
+                        print(repr(spec))
+                        attributes = spec.children[1]
+                        if attributes is not None:
+                            for attribute in attributes.children:
+                                if attribute.__class__ \
+                                        == Fortran2003.Proc_Attr_Spec:
+                                    # if so, remove argument names from
+                                    # dummy_args
+                                    for arg in spec.children[2].children:
+                                        arg_name = arg.string.lower()
+                                        if arg_name in dummy_args:
+                                            dummy_args.remove(arg_name)
+
             # get the type of block
             if type(scope) == Fortran2003.Subroutine_Subprogram:
                 unit_type = 'subroutine'
             elif type(scope) == Fortran2003.Function_Subprogram:
                 unit_type = 'function'
 
             # any remaining dummy arguments lack intent
@@ -557,15 +575,15 @@
                           (Fortran2003.Data_Component_Def_Stmt,
                            Fortran2003.Type_Declaration_Stmt)):
                 type_spec: Fortran2003.Intrinsic_Type_Spec = candidate.items[0]
                 kind_selector: Fortran2003.Kind_Selector = type_spec.items[1]
 
                 if isinstance(kind_selector, Fortran2003.Kind_Selector):
                     data_type: str = type_spec.items[0].lower()
-                    kind: str = kind_selector.string.strip('()')
+                    kind: str = str(kind_selector.children[1])
                     match = self._patterns[data_type].match(kind)
                     if match is None:
                         entity_declaration = candidate.items[2]
                         message = self._ISSUE_TEMPLATE.format(
                             type=data_type,
                             kind=kind,
                             name=entity_declaration,
@@ -678,15 +696,14 @@
                                 (Fortran2003.Entity_Decl,
                                  Fortran2003.Component_Decl)):
                     name = str(fp_get_child(constant.parent.parent,
                                             Fortran2003.Name))
                     message = f'Literal value assigned to "{name}"' \
                               ' without kind'
                 else:
-                    print(repr(constant.parent.parent))
                     message = 'Literal value without "kind"'
                 issues.append(Issue(message, line=_line(constant)))
 
         return issues
 
 
 class ForbidUsage(FortranRule):
```

### Comparing `stylist-0.3.1/source/stylist/issue.py` & `stylist-0.4.0/source/stylist/issue.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,47 +3,65 @@
 # (c) Crown copyright 2019 Met Office. All rights reserved.
 # The file LICENCE, distributed with this code, contains details of the terms
 # under which the code may be used.
 ##############################################################################
 """
 Issues found in the source.
 """
-from typing import Optional
+from pathlib import Path
+from typing import Any, Optional
 
 
-class Issue(object):
+class Issue:
     """
     Holds details pertaining to an issue with the source.
     """
     def __init__(self,
                  description: str,
                  line: Optional[int] = None,
-                 filename: Optional[str] = None) -> None:
+                 filename: Optional[Path] = None) -> None:
         """
         :param description: Free-format string describing the issue.
         :param line: Line number where issue found.
         :param filename: File in which issue found.
         """
         self._filename = filename
         self._line = line
         self._description = description
 
+    def __lt__(self, other: Any):
+        """
+        Bespoke less-than operator.
+
+        This is provided in order to support sorting of lists of issues.
+        """
+        if not isinstance(other, Issue):
+            raise ValueError(f"Can't compare Issue with {other._class__}")
+
+        self_key = (self.filename or Path('/'),
+                    self.line or 0,
+                    self.description)
+        other_key = (other.filename or Path('/'),
+                     other.line or 0,
+                     other.description)
+        return self_key < other_key
+
     def __str__(self) -> str:
         string = ''
         if self._filename:
-            string += '{filename}: '
+            string += f'{str(self._filename)}: '
         if self._line:
-            string += '{line}: '
-        string += '{description}'
+            string += f'{self._line}: '
+        string += f'{self._description}'
         return string.format(filename=self._filename,
                              line=self._line,
                              description=self._description)
 
     @property
-    def filename(self) -> Optional[str]:
+    def filename(self) -> Optional[Path]:
         """
         Filename associated with this issue.
         """
         return self._filename
 
     @property
     def line(self) -> Optional[int]:
@@ -55,12 +73,12 @@
     @property
     def description(self) -> str:
         """
         Description of this issue.
         """
         return self._description
 
-    def set_filename(self, filename: str) -> None:
+    def set_filename(self, filename: Path) -> None:
         """
         Associates a filename with this issue.
         """
         self._filename = filename
```

### Comparing `stylist-0.3.1/source/stylist/rule.py` & `stylist-0.4.0/source/stylist/rule.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 # (c) Crown copyright 2019 Met Office. All rights reserved.
 # The file LICENCE, distributed with this code, contains details of the terms
 # under which the code may be used.
 ##############################################################################
 """
 None language specific rules.
 """
-from abc import ABCMeta, abstractmethod
+from abc import ABC, abstractmethod
 import re
 from typing import List
 
 from stylist.issue import Issue
 from stylist.source import SourceText
 
 
-class Rule(object, metaclass=ABCMeta):
+class Rule(ABC):
     """
     Abstract parent of all rules.
     """
     @abstractmethod
     def examine(self, subject) -> List[Issue]:
         """
         Examines the provided source code object for issues.
@@ -44,7 +44,35 @@
             line_tally += 1
             match = self._TRAILING_SPACE_PATTERN.search(line)
             if match:
                 description = 'Found trailing white space'
                 issues.append(Issue(description, line=line_tally))
 
         return issues
+
+
+class LimitLineLength(Rule):
+    """
+    Report instances of lines being too long.
+    """
+    def __init__(self,
+                 length: int = 79,
+                 ignore_leading_whitespace: bool = False) -> None:
+        self._length = length
+        self._ignore_leading_whitespace = ignore_leading_whitespace
+
+    def examine(self, subject: SourceText) -> List[Issue]:
+        issues: List[Issue] = []
+
+        line_tally = 0
+        line: str
+        for line in subject.get_text().splitlines():
+            line_tally += 1
+            if self._ignore_leading_whitespace:
+                line = line.lstrip()
+            if len(line) > self._length:
+                description = f"Line exceeds {self._length} characters"
+                if self._ignore_leading_whitespace:
+                    description += " after leading whitespace"
+                issues.append(Issue(description, line=line_tally))
+
+        return issues
```

### Comparing `stylist-0.3.1/source/stylist/source.py` & `stylist-0.4.0/source/stylist/source.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,34 +3,34 @@
 # (c) Crown copyright 2019 Met Office. All rights reserved.
 # The file LICENCE, distributed with this code, contains details of the terms
 # under which the code may be used.
 ##############################################################################
 """
 Manages source code in various flavours.
 """
-from abc import ABCMeta, abstractmethod
+from abc import ABC, abstractmethod
+from pathlib import Path
 import re
-import os.path
 from typing import (Generator,
-                    IO,
                     Iterable,
                     List,
                     Optional,
+                    TextIO,
                     Type,
                     Union)
 
 import fparser.common.readfortran as readfortran  # type: ignore
 import fparser.two.Fortran2003 as Fortran2003  # type: ignore
 from fparser.two.parser import ParserFactory  # type:ignore
 from fparser.two.utils import FparserException  # type: ignore
 
 from stylist import StylistException
 
 
-class SourceText(object, metaclass=ABCMeta):
+class SourceText(ABC):
     """
     Handles source code at the text level. Makes use of the decorator pattern
     to perform text level preprocessing.
     """
     @abstractmethod
     def get_text(self) -> str:
         """
@@ -39,21 +39,20 @@
         raise NotImplementedError()
 
 
 class SourceFileReader(SourceText):
     """
     Reads text source from a file.
     """
-    def __init__(self, source_file: Union[IO[str], str]) -> None:
+    def __init__(self, source_file: Union[TextIO, Path]) -> None:
         """
         :param source_file: The file to examine.
         """
-        if isinstance(source_file, str):
-            with open(source_file, 'rt') as handle:
-                self._cache = handle.read()
+        if isinstance(source_file, Path):
+            self._cache = source_file.read_text()
         else:
             self._cache = source_file.read()
 
     def get_text(self) -> str:
         return self._cache
 
 
@@ -67,122 +66,126 @@
         """
         self._source_string = source_string
 
     def get_text(self) -> str:
         return self._source_string
 
 
-class TextProcessor(SourceText, metaclass=ABCMeta):
+class TextProcessor(SourceText, ABC):
     """
     Preprocessor decorators inherit from this. This is part of the decorator
     pattern.
     """
     def __init__(self, source: SourceText) -> None:
         """
         :param source: The source to be preprocessed.
         """
         self._source = source
 
-
-class MetaCPreProcessor(ABCMeta):
-    """
-    Identifies the C preprocessor.
-    """
-    def __str__(self) -> str:
-        return "C preprocessor"
+    @staticmethod
+    @abstractmethod
+    def get_name() -> str:
+        """
+        Gets the name of the processing stage.
+        """
+        raise NotImplementedError()
 
 
-class CPreProcessor(TextProcessor, metaclass=MetaCPreProcessor):
+class CPreProcessor(TextProcessor):
     """
     Strips out preprocessor directives.
 
     It is assumed that you want to syntax check all the Source so all
     conditional directives such as ``#ifdef`` are stripped out.
     """
     _CONDITIONAL_DIRECTIVE_PATTERN = re.compile(r'^(\s*)(#if(def|\s+)*)$',
                                                 re.MULTILINE)
     _OTHER_DIRECTIVE_PATTERN = re.compile(r'^(\s*)(#.*)$', re.MULTILINE)
 
+    @staticmethod
+    def get_name() -> str:
+        return "C preprocessor"
+
     def get_text(self) -> str:
         """
         :return: Source as text with preprocessor directives removed.
         """
         text = self._source.get_text()
         text = self._CONDITIONAL_DIRECTIVE_PATTERN.sub(r'\1// \2', text)
         text = self._OTHER_DIRECTIVE_PATTERN.sub(r'\1// \2', text)
         return text
 
 
-class MetaFortranPreProcessor(ABCMeta):
-    """
-    Identifies the Fortran preprocessor.
-    """
-    def __str__(self) -> str:
-        return "Fortran preprocessor"
-
-
-class FortranPreProcessor(TextProcessor, metaclass=MetaFortranPreProcessor):
+class FortranPreProcessor(TextProcessor):
     """
     Strips out preprocessor directives.
 
     It is assumed that you want to syntax check all the Source so all
     conditional directives such as ``#ifdef`` are stripped out.
     """
     _CONDITIONAL_DIRECTIVE_PATTERN = re.compile(r'^(\s*)(#if(def|\s+)*)$',
                                                 re.MULTILINE)
     _OTHER_DIRECTIVE_PATTERN = re.compile(r'^(\s*)(#.*)$', re.MULTILINE)
 
+    @staticmethod
+    def get_name() -> str:
+        return "Fortran preprocessor"
+
     def get_text(self) -> str:
         """
         :return: Source as text with preprocessor directives removed.
         """
         text = self._source.get_text()
         text = self._CONDITIONAL_DIRECTIVE_PATTERN.sub(r'\1! \2', text)
         text = self._OTHER_DIRECTIVE_PATTERN.sub(r'\1! \2', text)
         return text
 
 
-class MetaPFUnitProcessor(ABCMeta):
-    """
-    Identifies the pFUnit preprocessor.
-    """
-    def __str__(self) -> str:
-        return "pFUnit preprocessor"
-
-
-class PFUnitProcessor(TextProcessor, metaclass=MetaPFUnitProcessor):
+class PFUnitProcessor(TextProcessor):
     """
     Strips out pFUnit directives.
     """
     _DIRECTIVE_PATTERN = re.compile(r'^(\s*)(@\w+.*)$', re.MULTILINE)
 
+    @staticmethod
+    def get_name() -> str:
+        return "pFUnit preprocessor"
+
     def get_text(self) -> str:
         """
         :return: Source as text with preprocessor directives removed.
         """
         text = self._source.get_text()
         text = self._DIRECTIVE_PATTERN.sub(r'\1! \2', text)
         return text
 
 
-class SourceTree(object, metaclass=ABCMeta):
+class SourceTree(ABC):
     """
-    Abstract parent of all actual language source files.
+    Abstract parent of all actual language  files.
     """
     def __init__(self, text: SourceText) -> None:
         """
         :param text: Source as text.
         """
         if not isinstance(text, SourceText):
             raise Exception('text argument must derive from SourceText.')
 
         self._text = text
         self._tree = None
         self._tree_error: Optional[str] = 'Not parsed yet'
 
+    @staticmethod
+    @abstractmethod
+    def get_name() -> str:
+        """
+        Gets the name of the source tree type.
+        """
+        raise NotImplementedError()
+
     @abstractmethod
     def get_tree(self):
         """
         Gets a parse-tree representation of the source file.
         """
         raise NotImplementedError()
 
@@ -196,26 +199,22 @@
     def get_text(self) -> str:
         """
         :return: Original source text.
         """
         return self._text.get_text()
 
 
-class MetaFortranSource(ABCMeta):
+class FortranSource(SourceTree):
     """
-    Identifies Fortran source.
+    Holds a Fortran source file as both a text block and parse tree.
     """
-    def __str__(self) -> str:
+    @staticmethod
+    def get_name() -> str:
         return 'Fortran source'
 
-
-class FortranSource(SourceTree, metaclass=MetaFortranSource):
-    """
-    Holds a Fortran source file as both a text block and parse tree.
-    """
     def get_tree(self) -> Optional[Fortran2003.Program]:
         """
         :return: Program unit object.
         """
         if not self._tree:
             # We don't use the tree directly. Instead we let all the decorators
             # have a go first.
@@ -242,34 +241,35 @@
             -> Fortran2003.StmtBase:
         """
         Gets the first "statement" part of the syntax tree or part thereof.
 
         :param root: Point in parse tree to start. If unspecified implies the
                      whole tree.
         """
-        if not root:
+        if root is None:
             root = self._tree.content
 
-        root = [root]
+        candidates = [root]
 
-        while root:
-            candidate = root.pop(0)
+        while candidates:
+            candidate = candidates.pop(0)
             if isinstance(candidate, Fortran2003.StmtBase):
                 return candidate
 
             if isinstance(candidate, Fortran2003.BlockBase):
-                root.extend(candidate.content)
+                candidates.extend(candidate.content)
             elif isinstance(candidate, Fortran2003.SequenceBase):
-                root.extend(candidate.items)
+                candidates.extend(candidate.items)
             elif isinstance(candidate, Fortran2003.Comment):
                 pass
             else:
                 message = 'Unexpected candidate type: {0}'
                 raise Exception(message.format(candidate.__class__.__name__))
-        raise StylistException("Block without any statements.")
+        message = f"Block without any statements: {root.tofortran()}"
+        raise StylistException(message)
 
     def path(self,
              path: Union[Iterable, str],
              root: Optional[Fortran2003.Block] = None) \
             -> List[Fortran2003.Base]:
         """
         Gets the tree nodes at the given path.
@@ -412,61 +412,53 @@
             print(' ' * indent + child.__class__.__name__)
             if isinstance(child, Fortran2003.BlockBase):
                 FortranSource.print_tree(child.content, indent+1)
             elif isinstance(child, Fortran2003.SequenceBase):
                 FortranSource.print_tree(child.items, indent+1)
 
 
-class MetaCSource(ABCMeta):
-    """
-    Identifies C source.
-    """
-    def __str__(self) -> str:
-        return "C source"
-
-
-class CSource(SourceTree, metaclass=MetaCSource):
+class CSource(SourceTree):
     """
     Holds a C/C++ source file as both a text block and parse tree.
 
     .. todo::
        This is just a stub to illustrate how it would be done. It is not
        useable.
     """
+    @staticmethod
+    def get_name() -> str:
+        return "C source"
+
     def get_tree(self):
         raise NotImplementedError('C/C++ source is not supported yet.')
 
     def get_tree_error(self) -> Optional[str]:
         raise NotImplementedError('C/C++ source is not supported yet.')
 
 
-class MetaPlainText(ABCMeta):
+class PlainText(SourceTree):
     """
-    Identifies plain text.
+    Holds a plain text file as though it were source.
     """
-    def __str__(self) -> str:
+    @staticmethod
+    def get_name() -> str:
         return "plain text"
 
-
-class PlainText(SourceTree, metaclass=MetaPlainText):
-    """
-    Holds a plain text file as though it were source.
-    """
     def get_tree(self) -> Generator[str, None, None]:
         """
         :return: File content line by line.
         """
         for line in self.get_text().splitlines():
             yield line
 
     def get_tree_error(self) -> Optional[str]:
         return None
 
 
-class FilePipe(object):
+class FilePipe:
     """
     Holds the chain of objects needed to understand a particular file
     extension.
     """
     def __init__(self,
                  parser: Type[SourceTree],
                  *preprocessors: Type[TextProcessor]) -> None:
@@ -474,15 +466,15 @@
         :param parser: Underlying language parser.
         :param preprocessors: Any preprocessors to apply before parsing.
         """
         self.parser = parser
         self.preprocessors = preprocessors
 
 
-class SourceFactory(object):
+class SourceFactory:
     """
     Manages the handling of source file. Knows what chains of objects are
     needed to handle each file extension.
 
     It is hard to lay down hard and fast rules about what should go in the
     default list of extensions. Language standards do not generally specify an
     extension since that is an OS level concept. Some filesystems do not use
@@ -541,31 +533,31 @@
     def get_extensions(cls) -> Iterable[str]:
         """
         Gets the file extensions recognised by the ``read_file()`` method.
         """
         return cls._extension_map.keys()
 
     @classmethod
-    def read_file(cls, source_file: Union[IO[str], str]) -> SourceTree:
+    def read_file(cls, source_file: Union[TextIO, Path]) -> SourceTree:
         """
         Creates a Source object from a file.
 
         The file extension is used to determine the source type so this will
         not work on file-like objects which do not have a filename.
         """
-        if isinstance(source_file, str):
+        if isinstance(source_file, Path):
             filename = source_file
         else:
-            filename = source_file.name
+            filename = Path(source_file.name)
 
-        ext = os.path.splitext(filename)[1][1:]
-        if ext not in cls._extension_map:
-            raise Exception('Source file extension "{0}" not in handler map'
-                            .format(ext))
+        extension = filename.suffix[1:]
+        if extension not in cls._extension_map:
+            message = f"Source file extension '{extension}' not in handler map"
+            raise Exception(message)
 
-        chain = cls._extension_map[ext]
+        chain = cls._extension_map[extension]
         reader: SourceText = SourceFileReader(source_file)
         # Decorate reader
         for handler_class in chain.preprocessors:
             reader = handler_class(reader)
 
         return chain.parser(reader)
```

### Comparing `stylist-0.3.1/source/stylist/style.py` & `stylist-0.4.0/source/stylist/style.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 # (c) Crown copyright 2019 Met Office. All rights reserved.
 # The file LICENCE, distributed with this code, contains details of the terms
 # under which the code may be used.
 ##############################################################################
 """
 Classes relating to styles made up of rules.
 """
-from abc import ABCMeta
+from abc import ABC
 import logging
 from typing import List
 
 import stylist.fortran
 import stylist.issue
 from stylist.rule import Rule
 import stylist.source
 
 
-class Style(object, metaclass=ABCMeta):
+class Style(ABC):
     """
     Abstract parent of all style lists.
     """
     def __init__(self, *rules: Rule) -> None:
         """
         :param *args: Rules which make up this style.
         """
```

### Comparing `stylist-0.3.1/source/stylist.egg-info/PKG-INFO` & `stylist-0.4.0/source/stylist.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,33 @@
 Metadata-Version: 2.1
 Name: stylist
-Version: 0.3.1
-Summary: Extensible code style checker currently supporting Fortran, PSyclone DSL, etc
+Version: 0.4.0
+Summary: Flexible source code style checking tool
 Home-page: https://github.com/MetOffice/stylist
 Author: Met Office
-License: BSD 3-Clause
+License: BSD 3-Clause License
+Project-URL: homepage, https://github.com/MetOffice/stylist/
+Project-URL: documentation, https://metoffice.github.io/stylist
 Project-URL: Bug Reports, https://github.com/MetOffice/stylist/issues
-Project-URL: Source, https://github.com/MetOffice/stylist/
+Project-URL: repository, https://github.com/MetOffice/stylist/
 Keywords: linter fortran psyclone
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Quality Assurance
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7, <4
+Classifier: Programming Language :: Python :: 3
+Requires-Python: <4,>=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 Provides-Extra: test
+Provides-Extra: performance
 Provides-Extra: docs
 Provides-Extra: release
 License-File: LICENSE
 
 Stylist
 =======
 
-|BSD3 License| |GitHub release| |PyPI version| |GitHub merge testing|
+|BSD3 License| |GitHub release| |PyPI version| |Conda version| |GitHub merge testing|
 
 Stylist is a tool for checking code style. It implements a framework which
 supports multiple styles across multiple languages.
 
 But aren't there many such tools out there, why create a new one?
 
 The simple reason is that few of them support Fortran, a language still in
@@ -56,27 +52,30 @@
 
 .. |GitHub release| image:: https://img.shields.io/github/release/MetOffice/stylist.svg
    :target: https://github.com/MetOffice/stylist/
 
 .. |PyPI version| image:: https://badge.fury.io/py/stylist.svg
    :target: https://pypi.python.org/pypi/stylist/
 
+.. |Conda version| image:: https://img.shields.io/conda/vn/conda-forge/stylist.svg
+   :target: https://anaconda.org/conda-forge/stylist
+
 .. |GitHub merge testing| image:: https://github.com/MetOffice/stylist/workflows/Merge%20Test/badge.svg
    :target: https://github.com/MetOffice/stylist/actions
 
 
 Installation
 ~~~~~~~~~~~~
 
 Installation can be as simple as ``pip install stylist`` or
 ``conda install -c conda-forge stylist``.
 
-As always it is also possible to install from the project source by running
-``python setup.py``. The source may be obtained by downloading a tarball or by
-cloning the repository.
+As always it is also possible to install from the project source using
+``pip install --editable .``. The source may be obtained by downloading a
+tarball or by cloning the repository.
 
 
 Usage
 ~~~~~
 
 Stylist provides a command-line tool ``stylist`` for normal use. It can also be
 used as a package if you want to integrate it with another tool. Documentation
@@ -138,10 +137,10 @@
 
 An illustrative example::
 
   from re import compile as recompile
   from stylist.style import Style
   from stylist.fortran import FortranCharacterset, KindPattern
   
-  simple = Style(FortranCharactersest(),
+  simple = Style(FortranCharacterset(),
                  KindPattern(integer=recompile(r'i_.+'),
-                             real=recompile(r'r_.+'))
+                             real=recompile(r'r_.+')))
```

