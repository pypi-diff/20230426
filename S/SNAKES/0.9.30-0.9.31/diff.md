# Comparing `tmp/SNAKES-0.9.30.tar.gz` & `tmp/SNAKES-0.9.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SNAKES-0.9.30.tar", last modified: Thu Mar 16 11:56:28 2023, max compression
+gzip compressed data, was "SNAKES-0.9.31.tar", last modified: Wed Apr 26 13:34:46 2023, max compression
```

## Comparing `SNAKES-0.9.30.tar` & `SNAKES-0.9.31.tar`

### file list

```diff
@@ -1,153 +1,153 @@
-drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2023-03-16 11:56:28.395639 SNAKES-0.9.30/
--rw-r--r--   0 franck    (1000) franck    (1000)       60 2016-09-20 08:55:14.798269 SNAKES-0.9.30/.gitignore
--rw-r--r--   0 franck    (1000) franck    (1000)      423 2015-03-14 16:15:28.936069 SNAKES-0.9.30/BUGS
--rw-rw-r--   0 franck    (1000) franck    (1000)     7642 2022-05-13 06:38:09.861553 SNAKES-0.9.30/LICENCE.md
--rw-r--r--   0 franck    (1000) franck    (1000)     3747 2023-03-16 11:56:28.387639 SNAKES-0.9.30/MANIFEST
--rw-r--r--   0 franck    (1000) franck    (1000)       95 2016-06-20 09:18:26.643131 SNAKES-0.9.30/MANIFEST.in
--rw-r--r--   0 franck    (1000) franck    (1000)     1133 2020-10-14 14:14:50.647564 SNAKES-0.9.30/Makefile
--rw-rw-r--   0 franck    (1000) franck    (1000)      987 2023-03-16 11:56:28.395639 SNAKES-0.9.30/PKG-INFO
--rw-r--r--   0 franck    (1000) franck    (1000)     2331 2021-06-09 15:58:26.142109 SNAKES-0.9.30/README.md
--rw-r--r--   0 franck    (1000) franck    (1000)        7 2023-03-16 11:55:27.227837 SNAKES-0.9.30/VERSION
-drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2023-03-16 11:56:28.391639 SNAKES-0.9.30/bin/
--rwxr-xr-x   0 franck    (1000) franck    (1000)       80 2015-03-14 16:15:28.936069 SNAKES-0.9.30/bin/abcd
--rwxr-xr-x   0 franck    (1000) franck    (1000)     4018 2015-03-14 16:15:28.936069 SNAKES-0.9.30/bin/snkc
--rwxr-xr-x   0 franck    (1000) franck    (1000)     1908 2015-03-14 16:15:28.936069 SNAKES-0.9.30/bin/snkd
-drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2023-03-16 11:56:28.391639 SNAKES-0.9.30/doc/
--rw-r--r--   0 franck    (1000) franck    (1000)     7639 2015-03-14 16:15:28.936069 SNAKES-0.9.30/doc/COPYING
--rw-r--r--   0 franck    (1000) franck    (1000)    13756 2015-03-14 16:15:28.936069 SNAKES-0.9.30/doc/abcd.txt
-drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2023-03-16 11:56:28.391639 SNAKES-0.9.30/doc/examples/
-drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2023-03-16 11:56:28.391639 SNAKES-0.9.30/doc/examples/abcd/
--rw-r--r--   0 franck    (1000) franck    (1000)      274 2015-03-14 16:15:28.936069 SNAKES-0.9.30/doc/examples/abcd/README
-drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2023-03-16 11:56:28.391639 SNAKES-0.9.30/doc/examples/abcd/ns/
--rw-r--r--   0 franck    (1000) franck    (1000)    10652 2015-03-14 16:15:28.936069 SNAKES-0.9.30/doc/examples/abcd/ns/dolev_yao.py
--rw-r--r--   0 franck    (1000) franck    (1000)     1590 2015-03-14 16:15:28.936069 SNAKES-0.9.30/doc/examples/abcd/ns/ns.abcd
--rw-r--r--   0 franck    (1000) franck    (1000)      595 2015-03-14 16:15:28.936069 SNAKES-0.9.30/doc/examples/abcd/ns/ns.py
--rw-r--r--   0 franck    (1000) franck    (1000)      439 2015-03-14 16:15:28.936069 SNAKES-0.9.30/doc/examples/abcd/philo.abcd
--rw-r--r--   0 franck    (1000) franck    (1000)      469 2015-03-14 16:15:28.936069 SNAKES-0.9.30/doc/examples/abcd/prod-cons.abcd
--rw-r--r--   0 franck    (1000) franck    (1000)      878 2015-03-14 16:15:28.936069 SNAKES-0.9.30/doc/examples/abcd/railroad.abcd
--rw-r--r--   0 franck    (1000) franck    (1000)      482 2015-03-14 16:15:28.936069 SNAKES-0.9.30/doc/examples/abcd/railroad.py
--rw-r--r--   0 franck    (1000) franck    (1000)    21394 2015-03-14 16:15:28.936069 SNAKES-0.9.30/doc/queries.txt
--rw-r--r--   0 franck    (1000) franck    (1000)      922 2015-03-14 16:15:28.936069 SNAKES-0.9.30/doc/simple-coloured.pnml
--rw-r--r--   0 franck    (1000) franck    (1000)      805 2015-03-14 16:15:28.936069 SNAKES-0.9.30/doc/simple-pt.pnml
--rw-r--r--   0 franck    (1000) franck    (1000)    19513 2015-03-14 16:15:28.936069 SNAKES-0.9.30/doc/snakes-pnml.txt
--rw-r--r--   0 franck    (1000) franck    (1000)    15652 2015-03-14 16:15:28.936069 SNAKES-0.9.30/doc/tutorial.png
--rw-r--r--   0 franck    (1000) franck    (1000)    51066 2015-03-14 16:15:28.936069 SNAKES-0.9.30/doc/tutorial.txt
--rw-r--r--   0 franck    (1000) franck    (1000)      693 2015-03-14 16:15:28.936069 SNAKES-0.9.30/mklang.py
--rw-r--r--   0 franck    (1000) franck    (1000)     3381 2021-06-09 16:04:05.542667 SNAKES-0.9.30/setup.py
-drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2023-03-16 11:56:28.391639 SNAKES-0.9.30/snakes/
--rw-rw-r--   0 franck    (1000) franck    (1000)     1603 2023-03-16 11:55:27.227837 SNAKES-0.9.30/snakes/__init__.py
--rw-r--r--   0 franck    (1000) franck    (1000)      537 2017-12-09 15:45:08.326904 SNAKES-0.9.30/snakes/compat.py
--rw-r--r--   0 franck    (1000) franck    (1000)    32205 2015-03-14 16:15:28.936069 SNAKES-0.9.30/snakes/data.py
--rw-r--r--   0 franck    (1000) franck    (1000)    11922 2015-03-14 16:15:28.940069 SNAKES-0.9.30/snakes/hashables.py
-drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2023-03-16 11:56:28.391639 SNAKES-0.9.30/snakes/lang/
--rw-r--r--   0 franck    (1000) franck    (1000)     6396 2015-03-14 16:15:28.940069 SNAKES-0.9.30/snakes/lang/__init__.py
-drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2023-03-16 11:56:28.391639 SNAKES-0.9.30/snakes/lang/abcd/
--rw-r--r--   0 franck    (1000) franck    (1000)        0 2015-03-14 16:15:28.940069 SNAKES-0.9.30/snakes/lang/abcd/__init__.py
--rw-r--r--   0 franck    (1000) franck    (1000)    31781 2015-03-14 16:15:28.940069 SNAKES-0.9.30/snakes/lang/abcd/asdl.py
--rw-r--r--   0 franck    (1000) franck    (1000)    37555 2015-03-14 16:15:28.940069 SNAKES-0.9.30/snakes/lang/abcd/parser.py
--rw-r--r--   0 franck    (1000) franck    (1000)   290093 2015-03-14 16:15:28.940069 SNAKES-0.9.30/snakes/lang/abcd/pgen.py
--rw-r--r--   0 franck    (1000) franck    (1000)     9839 2015-03-14 16:15:28.940069 SNAKES-0.9.30/snakes/lang/asdl.py
--rw-r--r--   0 franck    (1000) franck    (1000)    10235 2015-03-14 16:15:28.940069 SNAKES-0.9.30/snakes/lang/astjy25.py
--rw-r--r--   0 franck    (1000) franck    (1000)    11941 2015-03-14 16:15:28.940069 SNAKES-0.9.30/snakes/lang/astpy25.py
--rw-r--r--   0 franck    (1000) franck    (1000)    10324 2015-03-14 16:15:28.940069 SNAKES-0.9.30/snakes/lang/astpypy.py
-drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2023-03-16 11:56:28.391639 SNAKES-0.9.30/snakes/lang/ctlstar/
--rw-r--r--   0 franck    (1000) franck    (1000)        0 2015-03-14 16:15:28.940069 SNAKES-0.9.30/snakes/lang/ctlstar/__init__.py
--rw-r--r--   0 franck    (1000) franck    (1000)    29069 2015-03-14 16:15:28.940069 SNAKES-0.9.30/snakes/lang/ctlstar/asdl.py
--rw-r--r--   0 franck    (1000) franck    (1000)    27179 2015-03-14 16:15:28.940069 SNAKES-0.9.30/snakes/lang/ctlstar/parser.py
--rw-r--r--   0 franck    (1000) franck    (1000)   286604 2015-03-14 16:15:28.944069 SNAKES-0.9.30/snakes/lang/ctlstar/pgen.py
--rw-r--r--   0 franck    (1000) franck    (1000)    49093 2015-03-14 16:15:28.944069 SNAKES-0.9.30/snakes/lang/pgen.py
-drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2023-03-16 11:56:28.391639 SNAKES-0.9.30/snakes/lang/pylib/
--rw-r--r--   0 franck    (1000) franck    (1000)        0 2015-03-14 16:15:28.944069 SNAKES-0.9.30/snakes/lang/pylib/__init__.py
--rw-r--r--   0 franck    (1000) franck    (1000)    11630 2015-03-14 16:15:28.944069 SNAKES-0.9.30/snakes/lang/pylib/asdl.py
--rw-r--r--   0 franck    (1000) franck    (1000)    26841 2015-03-14 16:15:28.944069 SNAKES-0.9.30/snakes/lang/pylib/spark.py
--rw-r--r--   0 franck    (1000) franck    (1000)    14022 2015-03-14 16:15:28.944069 SNAKES-0.9.30/snakes/lang/pylib/unparse.py
-drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2023-03-16 11:56:28.391639 SNAKES-0.9.30/snakes/lang/python/
--rw-r--r--   0 franck    (1000) franck    (1000)        0 2015-03-14 16:15:28.944069 SNAKES-0.9.30/snakes/lang/python/__init__.py
--rw-r--r--   0 franck    (1000) franck    (1000)    22425 2015-03-14 16:15:28.944069 SNAKES-0.9.30/snakes/lang/python/asdl.py
--rw-r--r--   0 franck    (1000) franck    (1000)    97603 2015-03-14 16:15:28.944069 SNAKES-0.9.30/snakes/lang/python/parser.py
--rw-r--r--   0 franck    (1000) franck    (1000)   210533 2015-03-14 16:15:28.948069 SNAKES-0.9.30/snakes/lang/python/pgen.py
--rw-r--r--   0 franck    (1000) franck    (1000)    14221 2015-03-14 16:15:28.948069 SNAKES-0.9.30/snakes/lang/unparse.py
--rw-r--r--   0 franck    (1000) franck    (1000)   158724 2022-10-24 13:00:21.585567 SNAKES-0.9.30/snakes/nets.py
-drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2023-03-16 11:56:28.395639 SNAKES-0.9.30/snakes/plugins/
--rw-r--r--   0 franck    (1000) franck    (1000)     7659 2015-03-14 16:15:28.948069 SNAKES-0.9.30/snakes/plugins/__init__.py
--rw-r--r--   0 franck    (1000) franck    (1000)     5850 2017-09-12 12:54:19.889129 SNAKES-0.9.30/snakes/plugins/bound.py
--rw-r--r--   0 franck    (1000) franck    (1000)    15116 2015-03-14 16:15:28.948069 SNAKES-0.9.30/snakes/plugins/clusters.py
--rw-r--r--   0 franck    (1000) franck    (1000)    17105 2023-03-16 10:10:42.618753 SNAKES-0.9.30/snakes/plugins/gv.py
--rw-r--r--   0 franck    (1000) franck    (1000)     1022 2015-03-14 16:15:28.948069 SNAKES-0.9.30/snakes/plugins/hello.py
--rw-r--r--   0 franck    (1000) franck    (1000)    11004 2015-03-14 16:15:28.948069 SNAKES-0.9.30/snakes/plugins/labels.py
--rw-r--r--   0 franck    (1000) franck    (1000)     3461 2016-10-10 16:15:27.918489 SNAKES-0.9.30/snakes/plugins/let.py
--rw-r--r--   0 franck    (1000) franck    (1000)     4689 2017-11-05 15:30:00.859886 SNAKES-0.9.30/snakes/plugins/modules.py
--rw-r--r--   0 franck    (1000) franck    (1000)    11449 2017-05-18 12:26:14.243229 SNAKES-0.9.30/snakes/plugins/ops.py
--rw-r--r--   0 franck    (1000) franck    (1000)    11054 2015-03-14 16:15:28.952069 SNAKES-0.9.30/snakes/plugins/pids.py
--rw-r--r--   0 franck    (1000) franck    (1000)    13387 2017-05-18 12:24:24.007225 SNAKES-0.9.30/snakes/plugins/pos.py
--rw-r--r--   0 franck    (1000) franck    (1000)     9573 2015-03-14 16:15:28.956069 SNAKES-0.9.30/snakes/plugins/query.py
--rw-r--r--   0 franck    (1000) franck    (1000)    25669 2017-05-18 12:25:58.315229 SNAKES-0.9.30/snakes/plugins/status.py
--rw-r--r--   0 franck    (1000) franck    (1000)    38797 2015-03-14 16:15:28.956069 SNAKES-0.9.30/snakes/plugins/synchro.py
--rw-r--r--   0 franck    (1000) franck    (1000)    31015 2015-03-14 16:15:28.956069 SNAKES-0.9.30/snakes/pnml.py
--rw-r--r--   0 franck    (1000) franck    (1000)    52213 2015-03-14 16:15:28.956069 SNAKES-0.9.30/snakes/typing.py
-drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2023-03-16 11:56:28.395639 SNAKES-0.9.30/snakes/utils/
--rw-r--r--   0 franck    (1000) franck    (1000)      382 2015-03-14 16:15:28.956069 SNAKES-0.9.30/snakes/utils/__init__.py
-drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2023-03-16 11:56:28.395639 SNAKES-0.9.30/snakes/utils/abcd/
--rw-r--r--   0 franck    (1000) franck    (1000)      630 2015-03-14 16:15:28.956069 SNAKES-0.9.30/snakes/utils/abcd/__init__.py
--rw-r--r--   0 franck    (1000) franck    (1000)    24866 2017-04-19 21:46:39.152750 SNAKES-0.9.30/snakes/utils/abcd/build.py
--rw-r--r--   0 franck    (1000) franck    (1000)     2505 2016-11-15 09:57:29.928644 SNAKES-0.9.30/snakes/utils/abcd/checker.py
--rw-r--r--   0 franck    (1000) franck    (1000)    17492 2015-03-14 16:15:28.956069 SNAKES-0.9.30/snakes/utils/abcd/html.py
--rw-r--r--   0 franck    (1000) franck    (1000)    10458 2016-10-10 16:27:06.566514 SNAKES-0.9.30/snakes/utils/abcd/main.py
-drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2023-03-16 11:56:28.395639 SNAKES-0.9.30/snakes/utils/abcd/resources/
--rw-r--r--   0 franck    (1000) franck    (1000)      249 2015-03-14 16:15:28.956069 SNAKES-0.9.30/snakes/utils/abcd/resources/about.html
--rw-r--r--   0 franck    (1000) franck    (1000)     1806 2015-03-14 16:15:28.956069 SNAKES-0.9.30/snakes/utils/abcd/resources/alive.txt
-drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2023-03-16 11:56:28.395639 SNAKES-0.9.30/snakes/utils/abcd/resources/css/
--rw-r--r--   0 franck    (1000) franck    (1000)    14936 2015-03-14 16:15:28.956069 SNAKES-0.9.30/snakes/utils/abcd/resources/css/bootstrap-theme.css
--rw-r--r--   0 franck    (1000) franck    (1000)    38388 2015-03-14 16:15:28.956069 SNAKES-0.9.30/snakes/utils/abcd/resources/css/bootstrap-theme.css.map
--rw-r--r--   0 franck    (1000) franck    (1000)   121220 2015-03-14 16:15:28.960069 SNAKES-0.9.30/snakes/utils/abcd/resources/css/bootstrap.css
--rw-r--r--   0 franck    (1000) franck    (1000)   245960 2015-03-14 16:15:28.960069 SNAKES-0.9.30/snakes/utils/abcd/resources/css/bootstrap.css.map
--rw-r--r--   0 franck    (1000) franck    (1000)    73046 2015-03-14 16:15:28.964069 SNAKES-0.9.30/snakes/utils/abcd/resources/css/docs.css
--rw-r--r--   0 franck    (1000) franck    (1000)   146525 2015-03-14 16:15:28.964069 SNAKES-0.9.30/snakes/utils/abcd/resources/d3.min.js
-drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2023-03-16 11:56:28.395639 SNAKES-0.9.30/snakes/utils/abcd/resources/fonts/
--rw-r--r--   0 franck    (1000) franck    (1000)    20335 2015-03-14 16:15:28.964069 SNAKES-0.9.30/snakes/utils/abcd/resources/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 franck    (1000) franck    (1000)    62927 2015-03-14 16:15:28.964069 SNAKES-0.9.30/snakes/utils/abcd/resources/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 franck    (1000) franck    (1000)    41280 2015-03-14 16:15:28.964069 SNAKES-0.9.30/snakes/utils/abcd/resources/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 franck    (1000) franck    (1000)    23320 2015-03-14 16:15:28.964069 SNAKES-0.9.30/snakes/utils/abcd/resources/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0 franck    (1000) franck    (1000)     3842 2015-03-14 16:15:28.964069 SNAKES-0.9.30/snakes/utils/abcd/resources/index.html
--rw-r--r--   0 franck    (1000) franck    (1000)   247350 2015-03-14 16:15:28.968069 SNAKES-0.9.30/snakes/utils/abcd/resources/jquery.min.js
--rw-r--r--   0 franck    (1000) franck    (1000)     2640 2015-03-14 16:15:28.968069 SNAKES-0.9.30/snakes/utils/abcd/resources/jquery.periodic.js
-drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2023-03-16 11:56:28.395639 SNAKES-0.9.30/snakes/utils/abcd/resources/js/
--rw-r--r--   0 franck    (1000) franck    (1000)     4602 2015-03-14 16:15:28.968069 SNAKES-0.9.30/snakes/utils/abcd/resources/js/bootstrap.file-input.js
--rw-r--r--   0 franck    (1000) franck    (1000)    29110 2015-03-14 16:15:28.968069 SNAKES-0.9.30/snakes/utils/abcd/resources/js/bootstrap.min.js
--rw-r--r--   0 franck    (1000) franck    (1000)      923 2015-03-14 16:15:28.968069 SNAKES-0.9.30/snakes/utils/abcd/resources/js/petri.js
--rw-r--r--   0 franck    (1000) franck    (1000)     1533 2015-03-14 16:15:28.968069 SNAKES-0.9.30/snakes/utils/abcd/resources/model.css
--rw-r--r--   0 franck    (1000) franck    (1000)      960 2015-03-14 16:15:28.968069 SNAKES-0.9.30/snakes/utils/abcd/resources/model.html
--rw-r--r--   0 franck    (1000) franck    (1000)     1689 2015-03-14 16:15:28.968069 SNAKES-0.9.30/snakes/utils/abcd/resources/model.js
--rw-r--r--   0 franck    (1000) franck    (1000)     1939 2015-03-14 16:15:28.968069 SNAKES-0.9.30/snakes/utils/abcd/resources/simulator.css
--rw-r--r--   0 franck    (1000) franck    (1000)    66924 2015-03-14 16:15:28.968069 SNAKES-0.9.30/snakes/utils/abcd/resources/simulator.js
--rw-r--r--   0 franck    (1000) franck    (1000)     3880 2015-03-14 16:15:28.968069 SNAKES-0.9.30/snakes/utils/abcd/simul.py
--rw-r--r--   0 franck    (1000) franck    (1000)     3101 2015-03-14 16:15:28.968069 SNAKES-0.9.30/snakes/utils/abcd/transform.py
--rw-r--r--   0 franck    (1000) franck    (1000)    25530 2017-05-18 12:20:59.263218 SNAKES-0.9.30/snakes/utils/apidoc.py
-drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2023-03-16 11:56:28.395639 SNAKES-0.9.30/snakes/utils/ctlstar/
--rw-r--r--   0 franck    (1000) franck    (1000)     1157 2015-03-14 16:15:28.968069 SNAKES-0.9.30/snakes/utils/ctlstar/__init__.py
--rw-r--r--   0 franck    (1000) franck    (1000)     6154 2015-03-14 16:15:28.968069 SNAKES-0.9.30/snakes/utils/ctlstar/build.py
-drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2023-03-16 11:56:28.395639 SNAKES-0.9.30/snakes/utils/simul/
--rw-r--r--   0 franck    (1000) franck    (1000)     8786 2016-09-16 08:14:17.115513 SNAKES-0.9.30/snakes/utils/simul/__init__.py
--rw-r--r--   0 franck    (1000) franck    (1000)     2548 2015-04-09 12:05:23.690282 SNAKES-0.9.30/snakes/utils/simul/html.py
--rw-r--r--   0 franck    (1000) franck    (1000)     7165 2020-10-30 13:38:52.892044 SNAKES-0.9.30/snakes/utils/simul/httpd.py
--rw-r--r--   0 franck    (1000) franck    (1000)     7136 2015-03-14 16:15:28.968069 SNAKES-0.9.30/snakes/utils/simul/logger.py
-drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2023-03-16 11:56:28.395639 SNAKES-0.9.30/snakes/utils/simul/resources/
--rw-r--r--   0 franck    (1000) franck    (1000)        0 2015-03-14 16:15:28.968069 SNAKES-0.9.30/snakes/utils/simul/resources/about.css
--rw-r--r--   0 franck    (1000) franck    (1000)      241 2015-03-14 16:15:28.968069 SNAKES-0.9.30/snakes/utils/simul/resources/about.html
--rw-r--r--   0 franck    (1000) franck    (1000)        0 2015-03-14 16:15:28.968069 SNAKES-0.9.30/snakes/utils/simul/resources/about.js
--rw-r--r--   0 franck    (1000) franck    (1000)     1806 2015-03-14 16:15:28.968069 SNAKES-0.9.30/snakes/utils/simul/resources/alive.txt
--rw-r--r--   0 franck    (1000) franck    (1000)     1621 2015-03-14 16:15:28.968069 SNAKES-0.9.30/snakes/utils/simul/resources/index.html
--rw-r--r--   0 franck    (1000) franck    (1000)    96381 2015-03-14 16:15:28.968069 SNAKES-0.9.30/snakes/utils/simul/resources/jquery.min.js
--rw-r--r--   0 franck    (1000) franck    (1000)     2653 2015-03-14 16:15:28.968069 SNAKES-0.9.30/snakes/utils/simul/resources/jquery.periodic.js
--rw-r--r--   0 franck    (1000) franck    (1000)       57 2015-03-14 16:15:28.968069 SNAKES-0.9.30/snakes/utils/simul/resources/model.css
--rw-r--r--   0 franck    (1000) franck    (1000)      195 2015-03-14 16:15:28.968069 SNAKES-0.9.30/snakes/utils/simul/resources/model.html
--rw-r--r--   0 franck    (1000) franck    (1000)        0 2015-03-14 16:15:28.968069 SNAKES-0.9.30/snakes/utils/simul/resources/model.js
--rw-r--r--   0 franck    (1000) franck    (1000)     1939 2015-03-14 16:15:28.968069 SNAKES-0.9.30/snakes/utils/simul/resources/simulator.css
--rw-r--r--   0 franck    (1000) franck    (1000)     4341 2015-03-14 16:15:28.968069 SNAKES-0.9.30/snakes/utils/simul/resources/simulator.js
--rw-r--r--   0 franck    (1000) franck    (1000)       57 2015-03-14 16:15:28.968069 SNAKES-0.9.30/snakes/utils/simul/resources/trace.css
--rw-r--r--   0 franck    (1000) franck    (1000)        0 2015-03-14 16:15:28.968069 SNAKES-0.9.30/snakes/utils/simul/resources/trace.js
--rw-r--r--   0 franck    (1000) franck    (1000)     2044 2015-03-14 16:15:28.972069 SNAKES-0.9.30/test.py
-drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2023-03-16 11:56:28.395639 SNAKES-0.9.30/utils/
--rw-r--r--   0 franck    (1000) franck    (1000)      226 2015-03-14 16:15:28.972069 SNAKES-0.9.30/utils/abcd-mode.el
--rw-r--r--   0 franck    (1000) franck    (1000)     3112 2016-06-20 09:09:40.347122 SNAKES-0.9.30/utils/abcd-mode.elc
--rw-r--r--   0 franck    (1000) franck    (1000)      777 2016-06-23 13:09:38.208567 SNAKES-0.9.30/version.py
+drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2023-04-26 13:34:46.875182 SNAKES-0.9.31/
+-rw-r--r--   0 franck    (1000) franck    (1000)       60 2016-09-20 08:55:14.798269 SNAKES-0.9.31/.gitignore
+-rw-r--r--   0 franck    (1000) franck    (1000)      423 2015-03-14 16:15:28.936069 SNAKES-0.9.31/BUGS
+-rw-rw-r--   0 franck    (1000) franck    (1000)     7642 2022-05-13 06:38:09.861553 SNAKES-0.9.31/LICENCE.md
+-rw-r--r--   0 franck    (1000) franck    (1000)     3747 2023-04-26 13:34:46.867182 SNAKES-0.9.31/MANIFEST
+-rw-r--r--   0 franck    (1000) franck    (1000)       95 2016-06-20 09:18:26.643131 SNAKES-0.9.31/MANIFEST.in
+-rw-r--r--   0 franck    (1000) franck    (1000)     1133 2020-10-14 14:14:50.647564 SNAKES-0.9.31/Makefile
+-rw-rw-r--   0 franck    (1000) franck    (1000)      987 2023-04-26 13:34:46.875182 SNAKES-0.9.31/PKG-INFO
+-rw-r--r--   0 franck    (1000) franck    (1000)     2331 2021-06-09 15:58:26.142109 SNAKES-0.9.31/README.md
+-rw-r--r--   0 franck    (1000) franck    (1000)        7 2023-04-26 13:34:30.631210 SNAKES-0.9.31/VERSION
+drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2023-04-26 13:34:46.871182 SNAKES-0.9.31/bin/
+-rwxr-xr-x   0 franck    (1000) franck    (1000)       80 2015-03-14 16:15:28.936069 SNAKES-0.9.31/bin/abcd
+-rwxr-xr-x   0 franck    (1000) franck    (1000)     4018 2015-03-14 16:15:28.936069 SNAKES-0.9.31/bin/snkc
+-rwxr-xr-x   0 franck    (1000) franck    (1000)     1908 2015-03-14 16:15:28.936069 SNAKES-0.9.31/bin/snkd
+drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2023-04-26 13:34:46.871182 SNAKES-0.9.31/doc/
+-rw-r--r--   0 franck    (1000) franck    (1000)     7639 2015-03-14 16:15:28.936069 SNAKES-0.9.31/doc/COPYING
+-rw-r--r--   0 franck    (1000) franck    (1000)    13756 2015-03-14 16:15:28.936069 SNAKES-0.9.31/doc/abcd.txt
+drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2023-04-26 13:34:46.867182 SNAKES-0.9.31/doc/examples/
+drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2023-04-26 13:34:46.871182 SNAKES-0.9.31/doc/examples/abcd/
+-rw-r--r--   0 franck    (1000) franck    (1000)      274 2015-03-14 16:15:28.936069 SNAKES-0.9.31/doc/examples/abcd/README
+drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2023-04-26 13:34:46.871182 SNAKES-0.9.31/doc/examples/abcd/ns/
+-rw-r--r--   0 franck    (1000) franck    (1000)    10652 2015-03-14 16:15:28.936069 SNAKES-0.9.31/doc/examples/abcd/ns/dolev_yao.py
+-rw-r--r--   0 franck    (1000) franck    (1000)     1590 2015-03-14 16:15:28.936069 SNAKES-0.9.31/doc/examples/abcd/ns/ns.abcd
+-rw-r--r--   0 franck    (1000) franck    (1000)      595 2015-03-14 16:15:28.936069 SNAKES-0.9.31/doc/examples/abcd/ns/ns.py
+-rw-r--r--   0 franck    (1000) franck    (1000)      439 2015-03-14 16:15:28.936069 SNAKES-0.9.31/doc/examples/abcd/philo.abcd
+-rw-r--r--   0 franck    (1000) franck    (1000)      469 2015-03-14 16:15:28.936069 SNAKES-0.9.31/doc/examples/abcd/prod-cons.abcd
+-rw-r--r--   0 franck    (1000) franck    (1000)      878 2015-03-14 16:15:28.936069 SNAKES-0.9.31/doc/examples/abcd/railroad.abcd
+-rw-r--r--   0 franck    (1000) franck    (1000)      482 2015-03-14 16:15:28.936069 SNAKES-0.9.31/doc/examples/abcd/railroad.py
+-rw-r--r--   0 franck    (1000) franck    (1000)    21394 2015-03-14 16:15:28.936069 SNAKES-0.9.31/doc/queries.txt
+-rw-r--r--   0 franck    (1000) franck    (1000)      922 2015-03-14 16:15:28.936069 SNAKES-0.9.31/doc/simple-coloured.pnml
+-rw-r--r--   0 franck    (1000) franck    (1000)      805 2015-03-14 16:15:28.936069 SNAKES-0.9.31/doc/simple-pt.pnml
+-rw-r--r--   0 franck    (1000) franck    (1000)    19513 2015-03-14 16:15:28.936069 SNAKES-0.9.31/doc/snakes-pnml.txt
+-rw-r--r--   0 franck    (1000) franck    (1000)    15652 2015-03-14 16:15:28.936069 SNAKES-0.9.31/doc/tutorial.png
+-rw-r--r--   0 franck    (1000) franck    (1000)    51066 2015-03-14 16:15:28.936069 SNAKES-0.9.31/doc/tutorial.txt
+-rw-r--r--   0 franck    (1000) franck    (1000)      693 2015-03-14 16:15:28.936069 SNAKES-0.9.31/mklang.py
+-rw-r--r--   0 franck    (1000) franck    (1000)     3381 2021-06-09 16:04:05.542667 SNAKES-0.9.31/setup.py
+drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2023-04-26 13:34:46.871182 SNAKES-0.9.31/snakes/
+-rw-rw-r--   0 franck    (1000) franck    (1000)     1603 2023-04-26 13:34:30.631210 SNAKES-0.9.31/snakes/__init__.py
+-rw-r--r--   0 franck    (1000) franck    (1000)      537 2017-12-09 15:45:08.326904 SNAKES-0.9.31/snakes/compat.py
+-rw-r--r--   0 franck    (1000) franck    (1000)    32205 2015-03-14 16:15:28.936069 SNAKES-0.9.31/snakes/data.py
+-rw-r--r--   0 franck    (1000) franck    (1000)    11922 2015-03-14 16:15:28.940069 SNAKES-0.9.31/snakes/hashables.py
+drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2023-04-26 13:34:46.871182 SNAKES-0.9.31/snakes/lang/
+-rw-r--r--   0 franck    (1000) franck    (1000)     6396 2015-03-14 16:15:28.940069 SNAKES-0.9.31/snakes/lang/__init__.py
+drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2023-04-26 13:34:46.871182 SNAKES-0.9.31/snakes/lang/abcd/
+-rw-r--r--   0 franck    (1000) franck    (1000)        0 2015-03-14 16:15:28.940069 SNAKES-0.9.31/snakes/lang/abcd/__init__.py
+-rw-r--r--   0 franck    (1000) franck    (1000)    31781 2015-03-14 16:15:28.940069 SNAKES-0.9.31/snakes/lang/abcd/asdl.py
+-rw-r--r--   0 franck    (1000) franck    (1000)    37555 2015-03-14 16:15:28.940069 SNAKES-0.9.31/snakes/lang/abcd/parser.py
+-rw-r--r--   0 franck    (1000) franck    (1000)   290093 2015-03-14 16:15:28.940069 SNAKES-0.9.31/snakes/lang/abcd/pgen.py
+-rw-r--r--   0 franck    (1000) franck    (1000)     9839 2015-03-14 16:15:28.940069 SNAKES-0.9.31/snakes/lang/asdl.py
+-rw-r--r--   0 franck    (1000) franck    (1000)    10235 2015-03-14 16:15:28.940069 SNAKES-0.9.31/snakes/lang/astjy25.py
+-rw-r--r--   0 franck    (1000) franck    (1000)    11941 2015-03-14 16:15:28.940069 SNAKES-0.9.31/snakes/lang/astpy25.py
+-rw-r--r--   0 franck    (1000) franck    (1000)    10324 2015-03-14 16:15:28.940069 SNAKES-0.9.31/snakes/lang/astpypy.py
+drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2023-04-26 13:34:46.871182 SNAKES-0.9.31/snakes/lang/ctlstar/
+-rw-r--r--   0 franck    (1000) franck    (1000)        0 2015-03-14 16:15:28.940069 SNAKES-0.9.31/snakes/lang/ctlstar/__init__.py
+-rw-r--r--   0 franck    (1000) franck    (1000)    29069 2015-03-14 16:15:28.940069 SNAKES-0.9.31/snakes/lang/ctlstar/asdl.py
+-rw-r--r--   0 franck    (1000) franck    (1000)    27179 2015-03-14 16:15:28.940069 SNAKES-0.9.31/snakes/lang/ctlstar/parser.py
+-rw-r--r--   0 franck    (1000) franck    (1000)   286604 2015-03-14 16:15:28.944069 SNAKES-0.9.31/snakes/lang/ctlstar/pgen.py
+-rw-r--r--   0 franck    (1000) franck    (1000)    49093 2015-03-14 16:15:28.944069 SNAKES-0.9.31/snakes/lang/pgen.py
+drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2023-04-26 13:34:46.871182 SNAKES-0.9.31/snakes/lang/pylib/
+-rw-r--r--   0 franck    (1000) franck    (1000)        0 2015-03-14 16:15:28.944069 SNAKES-0.9.31/snakes/lang/pylib/__init__.py
+-rw-r--r--   0 franck    (1000) franck    (1000)    11630 2015-03-14 16:15:28.944069 SNAKES-0.9.31/snakes/lang/pylib/asdl.py
+-rw-r--r--   0 franck    (1000) franck    (1000)    26841 2015-03-14 16:15:28.944069 SNAKES-0.9.31/snakes/lang/pylib/spark.py
+-rw-r--r--   0 franck    (1000) franck    (1000)    14022 2015-03-14 16:15:28.944069 SNAKES-0.9.31/snakes/lang/pylib/unparse.py
+drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2023-04-26 13:34:46.871182 SNAKES-0.9.31/snakes/lang/python/
+-rw-r--r--   0 franck    (1000) franck    (1000)        0 2015-03-14 16:15:28.944069 SNAKES-0.9.31/snakes/lang/python/__init__.py
+-rw-r--r--   0 franck    (1000) franck    (1000)    22425 2015-03-14 16:15:28.944069 SNAKES-0.9.31/snakes/lang/python/asdl.py
+-rw-r--r--   0 franck    (1000) franck    (1000)    97603 2015-03-14 16:15:28.944069 SNAKES-0.9.31/snakes/lang/python/parser.py
+-rw-r--r--   0 franck    (1000) franck    (1000)   210533 2015-03-14 16:15:28.948069 SNAKES-0.9.31/snakes/lang/python/pgen.py
+-rw-r--r--   0 franck    (1000) franck    (1000)    14221 2015-03-14 16:15:28.948069 SNAKES-0.9.31/snakes/lang/unparse.py
+-rw-r--r--   0 franck    (1000) franck    (1000)   158724 2022-10-24 13:00:21.585567 SNAKES-0.9.31/snakes/nets.py
+drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2023-04-26 13:34:46.871182 SNAKES-0.9.31/snakes/plugins/
+-rw-r--r--   0 franck    (1000) franck    (1000)     7731 2023-04-26 13:32:18.999430 SNAKES-0.9.31/snakes/plugins/__init__.py
+-rw-r--r--   0 franck    (1000) franck    (1000)     5850 2017-09-12 12:54:19.889129 SNAKES-0.9.31/snakes/plugins/bound.py
+-rw-r--r--   0 franck    (1000) franck    (1000)    15116 2023-04-26 13:16:22.245726 SNAKES-0.9.31/snakes/plugins/clusters.py
+-rw-r--r--   0 franck    (1000) franck    (1000)    17105 2023-03-16 10:10:42.618753 SNAKES-0.9.31/snakes/plugins/gv.py
+-rw-r--r--   0 franck    (1000) franck    (1000)     1022 2015-03-14 16:15:28.948069 SNAKES-0.9.31/snakes/plugins/hello.py
+-rw-r--r--   0 franck    (1000) franck    (1000)    11004 2015-03-14 16:15:28.948069 SNAKES-0.9.31/snakes/plugins/labels.py
+-rw-r--r--   0 franck    (1000) franck    (1000)     3461 2016-10-10 16:15:27.918489 SNAKES-0.9.31/snakes/plugins/let.py
+-rw-r--r--   0 franck    (1000) franck    (1000)     4689 2017-11-05 15:30:00.859886 SNAKES-0.9.31/snakes/plugins/modules.py
+-rw-r--r--   0 franck    (1000) franck    (1000)    11449 2017-05-18 12:26:14.243229 SNAKES-0.9.31/snakes/plugins/ops.py
+-rw-r--r--   0 franck    (1000) franck    (1000)    11054 2015-03-14 16:15:28.952069 SNAKES-0.9.31/snakes/plugins/pids.py
+-rw-r--r--   0 franck    (1000) franck    (1000)    13387 2017-05-18 12:24:24.007225 SNAKES-0.9.31/snakes/plugins/pos.py
+-rw-r--r--   0 franck    (1000) franck    (1000)     9573 2015-03-14 16:15:28.956069 SNAKES-0.9.31/snakes/plugins/query.py
+-rw-r--r--   0 franck    (1000) franck    (1000)    25669 2017-05-18 12:25:58.315229 SNAKES-0.9.31/snakes/plugins/status.py
+-rw-r--r--   0 franck    (1000) franck    (1000)    38797 2015-03-14 16:15:28.956069 SNAKES-0.9.31/snakes/plugins/synchro.py
+-rw-r--r--   0 franck    (1000) franck    (1000)    31015 2015-03-14 16:15:28.956069 SNAKES-0.9.31/snakes/pnml.py
+-rw-r--r--   0 franck    (1000) franck    (1000)    52213 2015-03-14 16:15:28.956069 SNAKES-0.9.31/snakes/typing.py
+drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2023-04-26 13:34:46.871182 SNAKES-0.9.31/snakes/utils/
+-rw-r--r--   0 franck    (1000) franck    (1000)      382 2015-03-14 16:15:28.956069 SNAKES-0.9.31/snakes/utils/__init__.py
+drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2023-04-26 13:34:46.871182 SNAKES-0.9.31/snakes/utils/abcd/
+-rw-r--r--   0 franck    (1000) franck    (1000)      630 2015-03-14 16:15:28.956069 SNAKES-0.9.31/snakes/utils/abcd/__init__.py
+-rw-r--r--   0 franck    (1000) franck    (1000)    24866 2017-04-19 21:46:39.152750 SNAKES-0.9.31/snakes/utils/abcd/build.py
+-rw-r--r--   0 franck    (1000) franck    (1000)     2505 2016-11-15 09:57:29.928644 SNAKES-0.9.31/snakes/utils/abcd/checker.py
+-rw-r--r--   0 franck    (1000) franck    (1000)    17492 2015-03-14 16:15:28.956069 SNAKES-0.9.31/snakes/utils/abcd/html.py
+-rw-r--r--   0 franck    (1000) franck    (1000)    10458 2016-10-10 16:27:06.566514 SNAKES-0.9.31/snakes/utils/abcd/main.py
+drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2023-04-26 13:34:46.871182 SNAKES-0.9.31/snakes/utils/abcd/resources/
+-rw-r--r--   0 franck    (1000) franck    (1000)      249 2015-03-14 16:15:28.956069 SNAKES-0.9.31/snakes/utils/abcd/resources/about.html
+-rw-r--r--   0 franck    (1000) franck    (1000)     1806 2015-03-14 16:15:28.956069 SNAKES-0.9.31/snakes/utils/abcd/resources/alive.txt
+drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2023-04-26 13:34:46.871182 SNAKES-0.9.31/snakes/utils/abcd/resources/css/
+-rw-r--r--   0 franck    (1000) franck    (1000)    14936 2015-03-14 16:15:28.956069 SNAKES-0.9.31/snakes/utils/abcd/resources/css/bootstrap-theme.css
+-rw-r--r--   0 franck    (1000) franck    (1000)    38388 2015-03-14 16:15:28.956069 SNAKES-0.9.31/snakes/utils/abcd/resources/css/bootstrap-theme.css.map
+-rw-r--r--   0 franck    (1000) franck    (1000)   121220 2015-03-14 16:15:28.960069 SNAKES-0.9.31/snakes/utils/abcd/resources/css/bootstrap.css
+-rw-r--r--   0 franck    (1000) franck    (1000)   245960 2015-03-14 16:15:28.960069 SNAKES-0.9.31/snakes/utils/abcd/resources/css/bootstrap.css.map
+-rw-r--r--   0 franck    (1000) franck    (1000)    73046 2015-03-14 16:15:28.964069 SNAKES-0.9.31/snakes/utils/abcd/resources/css/docs.css
+-rw-r--r--   0 franck    (1000) franck    (1000)   146525 2015-03-14 16:15:28.964069 SNAKES-0.9.31/snakes/utils/abcd/resources/d3.min.js
+drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2023-04-26 13:34:46.871182 SNAKES-0.9.31/snakes/utils/abcd/resources/fonts/
+-rw-r--r--   0 franck    (1000) franck    (1000)    20335 2015-03-14 16:15:28.964069 SNAKES-0.9.31/snakes/utils/abcd/resources/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 franck    (1000) franck    (1000)    62927 2015-03-14 16:15:28.964069 SNAKES-0.9.31/snakes/utils/abcd/resources/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 franck    (1000) franck    (1000)    41280 2015-03-14 16:15:28.964069 SNAKES-0.9.31/snakes/utils/abcd/resources/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 franck    (1000) franck    (1000)    23320 2015-03-14 16:15:28.964069 SNAKES-0.9.31/snakes/utils/abcd/resources/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0 franck    (1000) franck    (1000)     3842 2015-03-14 16:15:28.964069 SNAKES-0.9.31/snakes/utils/abcd/resources/index.html
+-rw-r--r--   0 franck    (1000) franck    (1000)   247350 2015-03-14 16:15:28.968069 SNAKES-0.9.31/snakes/utils/abcd/resources/jquery.min.js
+-rw-r--r--   0 franck    (1000) franck    (1000)     2640 2015-03-14 16:15:28.968069 SNAKES-0.9.31/snakes/utils/abcd/resources/jquery.periodic.js
+drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2023-04-26 13:34:46.871182 SNAKES-0.9.31/snakes/utils/abcd/resources/js/
+-rw-r--r--   0 franck    (1000) franck    (1000)     4602 2015-03-14 16:15:28.968069 SNAKES-0.9.31/snakes/utils/abcd/resources/js/bootstrap.file-input.js
+-rw-r--r--   0 franck    (1000) franck    (1000)    29110 2015-03-14 16:15:28.968069 SNAKES-0.9.31/snakes/utils/abcd/resources/js/bootstrap.min.js
+-rw-r--r--   0 franck    (1000) franck    (1000)      923 2015-03-14 16:15:28.968069 SNAKES-0.9.31/snakes/utils/abcd/resources/js/petri.js
+-rw-r--r--   0 franck    (1000) franck    (1000)     1533 2015-03-14 16:15:28.968069 SNAKES-0.9.31/snakes/utils/abcd/resources/model.css
+-rw-r--r--   0 franck    (1000) franck    (1000)      960 2015-03-14 16:15:28.968069 SNAKES-0.9.31/snakes/utils/abcd/resources/model.html
+-rw-r--r--   0 franck    (1000) franck    (1000)     1689 2015-03-14 16:15:28.968069 SNAKES-0.9.31/snakes/utils/abcd/resources/model.js
+-rw-r--r--   0 franck    (1000) franck    (1000)     1939 2015-03-14 16:15:28.968069 SNAKES-0.9.31/snakes/utils/abcd/resources/simulator.css
+-rw-r--r--   0 franck    (1000) franck    (1000)    66924 2015-03-14 16:15:28.968069 SNAKES-0.9.31/snakes/utils/abcd/resources/simulator.js
+-rw-r--r--   0 franck    (1000) franck    (1000)     3880 2015-03-14 16:15:28.968069 SNAKES-0.9.31/snakes/utils/abcd/simul.py
+-rw-r--r--   0 franck    (1000) franck    (1000)     3101 2015-03-14 16:15:28.968069 SNAKES-0.9.31/snakes/utils/abcd/transform.py
+-rw-r--r--   0 franck    (1000) franck    (1000)    25530 2017-05-18 12:20:59.263218 SNAKES-0.9.31/snakes/utils/apidoc.py
+drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2023-04-26 13:34:46.871182 SNAKES-0.9.31/snakes/utils/ctlstar/
+-rw-r--r--   0 franck    (1000) franck    (1000)     1157 2015-03-14 16:15:28.968069 SNAKES-0.9.31/snakes/utils/ctlstar/__init__.py
+-rw-r--r--   0 franck    (1000) franck    (1000)     6154 2015-03-14 16:15:28.968069 SNAKES-0.9.31/snakes/utils/ctlstar/build.py
+drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2023-04-26 13:34:46.875182 SNAKES-0.9.31/snakes/utils/simul/
+-rw-r--r--   0 franck    (1000) franck    (1000)     8786 2016-09-16 08:14:17.115513 SNAKES-0.9.31/snakes/utils/simul/__init__.py
+-rw-r--r--   0 franck    (1000) franck    (1000)     2548 2015-04-09 12:05:23.690282 SNAKES-0.9.31/snakes/utils/simul/html.py
+-rw-r--r--   0 franck    (1000) franck    (1000)     7165 2020-10-30 13:38:52.892044 SNAKES-0.9.31/snakes/utils/simul/httpd.py
+-rw-r--r--   0 franck    (1000) franck    (1000)     7136 2015-03-14 16:15:28.968069 SNAKES-0.9.31/snakes/utils/simul/logger.py
+drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2023-04-26 13:34:46.875182 SNAKES-0.9.31/snakes/utils/simul/resources/
+-rw-r--r--   0 franck    (1000) franck    (1000)        0 2015-03-14 16:15:28.968069 SNAKES-0.9.31/snakes/utils/simul/resources/about.css
+-rw-r--r--   0 franck    (1000) franck    (1000)      241 2015-03-14 16:15:28.968069 SNAKES-0.9.31/snakes/utils/simul/resources/about.html
+-rw-r--r--   0 franck    (1000) franck    (1000)        0 2015-03-14 16:15:28.968069 SNAKES-0.9.31/snakes/utils/simul/resources/about.js
+-rw-r--r--   0 franck    (1000) franck    (1000)     1806 2015-03-14 16:15:28.968069 SNAKES-0.9.31/snakes/utils/simul/resources/alive.txt
+-rw-r--r--   0 franck    (1000) franck    (1000)     1621 2015-03-14 16:15:28.968069 SNAKES-0.9.31/snakes/utils/simul/resources/index.html
+-rw-r--r--   0 franck    (1000) franck    (1000)    96381 2015-03-14 16:15:28.968069 SNAKES-0.9.31/snakes/utils/simul/resources/jquery.min.js
+-rw-r--r--   0 franck    (1000) franck    (1000)     2653 2015-03-14 16:15:28.968069 SNAKES-0.9.31/snakes/utils/simul/resources/jquery.periodic.js
+-rw-r--r--   0 franck    (1000) franck    (1000)       57 2015-03-14 16:15:28.968069 SNAKES-0.9.31/snakes/utils/simul/resources/model.css
+-rw-r--r--   0 franck    (1000) franck    (1000)      195 2015-03-14 16:15:28.968069 SNAKES-0.9.31/snakes/utils/simul/resources/model.html
+-rw-r--r--   0 franck    (1000) franck    (1000)        0 2015-03-14 16:15:28.968069 SNAKES-0.9.31/snakes/utils/simul/resources/model.js
+-rw-r--r--   0 franck    (1000) franck    (1000)     1939 2015-03-14 16:15:28.968069 SNAKES-0.9.31/snakes/utils/simul/resources/simulator.css
+-rw-r--r--   0 franck    (1000) franck    (1000)     4341 2015-03-14 16:15:28.968069 SNAKES-0.9.31/snakes/utils/simul/resources/simulator.js
+-rw-r--r--   0 franck    (1000) franck    (1000)       57 2015-03-14 16:15:28.968069 SNAKES-0.9.31/snakes/utils/simul/resources/trace.css
+-rw-r--r--   0 franck    (1000) franck    (1000)        0 2015-03-14 16:15:28.968069 SNAKES-0.9.31/snakes/utils/simul/resources/trace.js
+-rw-r--r--   0 franck    (1000) franck    (1000)     2044 2015-03-14 16:15:28.972069 SNAKES-0.9.31/test.py
+drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2023-04-26 13:34:46.875182 SNAKES-0.9.31/utils/
+-rw-r--r--   0 franck    (1000) franck    (1000)      226 2015-03-14 16:15:28.972069 SNAKES-0.9.31/utils/abcd-mode.el
+-rw-r--r--   0 franck    (1000) franck    (1000)     3112 2016-06-20 09:09:40.347122 SNAKES-0.9.31/utils/abcd-mode.elc
+-rw-r--r--   0 franck    (1000) franck    (1000)      777 2016-06-23 13:09:38.208567 SNAKES-0.9.31/version.py
```

### Comparing `SNAKES-0.9.30/LICENCE.md` & `SNAKES-0.9.31/LICENCE.md`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/MANIFEST` & `SNAKES-0.9.31/MANIFEST`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/Makefile` & `SNAKES-0.9.31/Makefile`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/PKG-INFO` & `SNAKES-0.9.31/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: SNAKES
-Version: 0.9.30
+Version: 0.9.31
 Summary: SNAKES is the Net Algebra Kit for Editors and Simulators
 Home-page: http://snakes.ibisc.univ-evry.fr/
 Author: Franck Pommereau
 Author-email: franck.pommereau@univ-evry.fr
 License: UNKNOWN
 Description: SNAKES is a general purpose Petri net Python
         library allowing to define and execute most classes of Petri
```

### Comparing `SNAKES-0.9.30/README.md` & `SNAKES-0.9.31/README.md`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/bin/snkc` & `SNAKES-0.9.31/bin/snkc`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/bin/snkd` & `SNAKES-0.9.31/bin/snkd`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/doc/COPYING` & `SNAKES-0.9.31/doc/COPYING`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/doc/abcd.txt` & `SNAKES-0.9.31/doc/abcd.txt`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/doc/examples/abcd/ns/dolev_yao.py` & `SNAKES-0.9.31/doc/examples/abcd/ns/dolev_yao.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/doc/examples/abcd/ns/ns.abcd` & `SNAKES-0.9.31/doc/examples/abcd/ns/ns.abcd`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/doc/examples/abcd/ns/ns.py` & `SNAKES-0.9.31/doc/examples/abcd/ns/ns.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/doc/examples/abcd/railroad.abcd` & `SNAKES-0.9.31/doc/examples/abcd/railroad.abcd`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/doc/queries.txt` & `SNAKES-0.9.31/doc/queries.txt`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/doc/simple-coloured.pnml` & `SNAKES-0.9.31/doc/simple-coloured.pnml`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/doc/simple-pt.pnml` & `SNAKES-0.9.31/doc/simple-pt.pnml`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/doc/snakes-pnml.txt` & `SNAKES-0.9.31/doc/snakes-pnml.txt`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/doc/tutorial.png` & `SNAKES-0.9.31/doc/tutorial.png`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/doc/tutorial.txt` & `SNAKES-0.9.31/doc/tutorial.txt`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/mklang.py` & `SNAKES-0.9.31/mklang.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/setup.py` & `SNAKES-0.9.31/setup.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/__init__.py` & `SNAKES-0.9.31/snakes/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 @copyright: (C) 2005-2013 Franck Pommereau
 @license: GNU Lesser General Public Licence (aka. GNU LGPL), see the
     file `doc/COPYING` in the distribution or visit the [GNU web
     site](http://www.gnu.org/licenses/licenses.html#LGPL)
 @contact: franck.pommereau@ibisc.univ-evry.fr
 """
 
-version = "0.9.30"
+version = "0.9.31"
 defaultencoding = "utf-8"
 
 """## Module `snakes`
 
 This module only provides the exceptions used throughout SNAKES.
 """
```

### Comparing `SNAKES-0.9.30/snakes/compat.py` & `SNAKES-0.9.31/snakes/compat.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/data.py` & `SNAKES-0.9.31/snakes/data.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/hashables.py` & `SNAKES-0.9.31/snakes/hashables.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/lang/__init__.py` & `SNAKES-0.9.31/snakes/lang/__init__.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/lang/abcd/asdl.py` & `SNAKES-0.9.31/snakes/lang/abcd/asdl.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/lang/abcd/parser.py` & `SNAKES-0.9.31/snakes/lang/abcd/parser.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/lang/abcd/pgen.py` & `SNAKES-0.9.31/snakes/lang/abcd/pgen.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/lang/asdl.py` & `SNAKES-0.9.31/snakes/lang/asdl.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/lang/astjy25.py` & `SNAKES-0.9.31/snakes/lang/astjy25.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/lang/astpy25.py` & `SNAKES-0.9.31/snakes/lang/astpy25.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/lang/astpypy.py` & `SNAKES-0.9.31/snakes/lang/astpypy.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/lang/ctlstar/asdl.py` & `SNAKES-0.9.31/snakes/lang/ctlstar/asdl.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/lang/ctlstar/parser.py` & `SNAKES-0.9.31/snakes/lang/ctlstar/parser.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/lang/ctlstar/pgen.py` & `SNAKES-0.9.31/snakes/lang/ctlstar/pgen.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/lang/pgen.py` & `SNAKES-0.9.31/snakes/lang/pgen.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/lang/pylib/asdl.py` & `SNAKES-0.9.31/snakes/lang/pylib/asdl.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/lang/pylib/spark.py` & `SNAKES-0.9.31/snakes/lang/pylib/spark.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/lang/pylib/unparse.py` & `SNAKES-0.9.31/snakes/lang/pylib/unparse.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/lang/python/asdl.py` & `SNAKES-0.9.31/snakes/lang/python/asdl.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/lang/python/parser.py` & `SNAKES-0.9.31/snakes/lang/python/parser.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/lang/python/pgen.py` & `SNAKES-0.9.31/snakes/lang/python/pgen.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/lang/unparse.py` & `SNAKES-0.9.31/snakes/lang/unparse.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/nets.py` & `SNAKES-0.9.31/snakes/nets.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/plugins/__init__.py` & `SNAKES-0.9.31/snakes/plugins/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,14 +158,16 @@
             for name in depends :
                 if name not in loaded :
                     module = load(name, module)
                     loaded.update(module.__plugins__)
             conf = set(conflicts) & loaded
             if len(conf) > 0 :
                 raise ValueError("plugin conflict (%s)" % ", ".join(conf))
+            if fun.__module__ in loaded :
+                return module
             objects = fun(module)
             if type(objects) is not tuple :
                 objects = (objects,)
             return build(fun.__module__, module, *objects)
         module = sys.modules[fun.__module__]
         module.__test__ = {"extend" : extend}
         objects = fun(__import__(base, fromlist=["__name__"]))
```

### Comparing `SNAKES-0.9.30/snakes/plugins/bound.py` & `SNAKES-0.9.31/snakes/plugins/bound.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/plugins/clusters.py` & `SNAKES-0.9.31/snakes/plugins/clusters.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/plugins/gv.py` & `SNAKES-0.9.31/snakes/plugins/gv.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/plugins/hello.py` & `SNAKES-0.9.31/snakes/plugins/hello.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/plugins/labels.py` & `SNAKES-0.9.31/snakes/plugins/labels.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/plugins/let.py` & `SNAKES-0.9.31/snakes/plugins/let.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/plugins/modules.py` & `SNAKES-0.9.31/snakes/plugins/modules.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/plugins/ops.py` & `SNAKES-0.9.31/snakes/plugins/ops.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/plugins/pids.py` & `SNAKES-0.9.31/snakes/plugins/pids.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/plugins/pos.py` & `SNAKES-0.9.31/snakes/plugins/pos.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/plugins/query.py` & `SNAKES-0.9.31/snakes/plugins/query.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/plugins/status.py` & `SNAKES-0.9.31/snakes/plugins/status.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/plugins/synchro.py` & `SNAKES-0.9.31/snakes/plugins/synchro.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/pnml.py` & `SNAKES-0.9.31/snakes/pnml.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/typing.py` & `SNAKES-0.9.31/snakes/typing.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/utils/abcd/__init__.py` & `SNAKES-0.9.31/snakes/utils/abcd/__init__.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/utils/abcd/build.py` & `SNAKES-0.9.31/snakes/utils/abcd/build.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/utils/abcd/checker.py` & `SNAKES-0.9.31/snakes/utils/abcd/checker.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/utils/abcd/html.py` & `SNAKES-0.9.31/snakes/utils/abcd/html.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/utils/abcd/main.py` & `SNAKES-0.9.31/snakes/utils/abcd/main.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/utils/abcd/resources/alive.txt` & `SNAKES-0.9.31/snakes/utils/abcd/resources/alive.txt`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/utils/abcd/resources/css/bootstrap-theme.css` & `SNAKES-0.9.31/snakes/utils/abcd/resources/css/bootstrap-theme.css`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/utils/abcd/resources/css/bootstrap-theme.css.map` & `SNAKES-0.9.31/snakes/utils/abcd/resources/css/bootstrap-theme.css.map`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/utils/abcd/resources/css/bootstrap.css` & `SNAKES-0.9.31/snakes/utils/abcd/resources/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/utils/abcd/resources/css/bootstrap.css.map` & `SNAKES-0.9.31/snakes/utils/abcd/resources/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/utils/abcd/resources/css/docs.css` & `SNAKES-0.9.31/snakes/utils/abcd/resources/css/docs.css`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/utils/abcd/resources/d3.min.js` & `SNAKES-0.9.31/snakes/utils/abcd/resources/d3.min.js`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/utils/abcd/resources/fonts/glyphicons-halflings-regular.eot` & `SNAKES-0.9.31/snakes/utils/abcd/resources/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/utils/abcd/resources/fonts/glyphicons-halflings-regular.svg` & `SNAKES-0.9.31/snakes/utils/abcd/resources/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/utils/abcd/resources/fonts/glyphicons-halflings-regular.ttf` & `SNAKES-0.9.31/snakes/utils/abcd/resources/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/utils/abcd/resources/fonts/glyphicons-halflings-regular.woff` & `SNAKES-0.9.31/snakes/utils/abcd/resources/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/utils/abcd/resources/index.html` & `SNAKES-0.9.31/snakes/utils/abcd/resources/index.html`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/utils/abcd/resources/jquery.min.js` & `SNAKES-0.9.31/snakes/utils/abcd/resources/jquery.min.js`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/utils/abcd/resources/jquery.periodic.js` & `SNAKES-0.9.31/snakes/utils/abcd/resources/jquery.periodic.js`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/utils/abcd/resources/js/bootstrap.file-input.js` & `SNAKES-0.9.31/snakes/utils/abcd/resources/js/bootstrap.file-input.js`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/utils/abcd/resources/js/bootstrap.min.js` & `SNAKES-0.9.31/snakes/utils/abcd/resources/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/utils/abcd/resources/js/petri.js` & `SNAKES-0.9.31/snakes/utils/abcd/resources/js/petri.js`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/utils/abcd/resources/model.css` & `SNAKES-0.9.31/snakes/utils/abcd/resources/model.css`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/utils/abcd/resources/model.html` & `SNAKES-0.9.31/snakes/utils/abcd/resources/model.html`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/utils/abcd/resources/model.js` & `SNAKES-0.9.31/snakes/utils/abcd/resources/model.js`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/utils/abcd/resources/simulator.css` & `SNAKES-0.9.31/snakes/utils/abcd/resources/simulator.css`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/utils/abcd/resources/simulator.js` & `SNAKES-0.9.31/snakes/utils/abcd/resources/simulator.js`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/utils/abcd/simul.py` & `SNAKES-0.9.31/snakes/utils/abcd/simul.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/utils/abcd/transform.py` & `SNAKES-0.9.31/snakes/utils/abcd/transform.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/utils/apidoc.py` & `SNAKES-0.9.31/snakes/utils/apidoc.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/utils/ctlstar/__init__.py` & `SNAKES-0.9.31/snakes/utils/ctlstar/__init__.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/utils/ctlstar/build.py` & `SNAKES-0.9.31/snakes/utils/ctlstar/build.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/utils/simul/__init__.py` & `SNAKES-0.9.31/snakes/utils/simul/__init__.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/utils/simul/html.py` & `SNAKES-0.9.31/snakes/utils/simul/html.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/utils/simul/httpd.py` & `SNAKES-0.9.31/snakes/utils/simul/httpd.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/utils/simul/logger.py` & `SNAKES-0.9.31/snakes/utils/simul/logger.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/utils/simul/resources/alive.txt` & `SNAKES-0.9.31/snakes/utils/simul/resources/alive.txt`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/utils/simul/resources/index.html` & `SNAKES-0.9.31/snakes/utils/simul/resources/index.html`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/utils/simul/resources/jquery.min.js` & `SNAKES-0.9.31/snakes/utils/simul/resources/jquery.min.js`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/utils/simul/resources/jquery.periodic.js` & `SNAKES-0.9.31/snakes/utils/simul/resources/jquery.periodic.js`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/utils/simul/resources/simulator.css` & `SNAKES-0.9.31/snakes/utils/simul/resources/simulator.css`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/snakes/utils/simul/resources/simulator.js` & `SNAKES-0.9.31/snakes/utils/simul/resources/simulator.js`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/test.py` & `SNAKES-0.9.31/test.py`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/utils/abcd-mode.elc` & `SNAKES-0.9.31/utils/abcd-mode.elc`

 * *Files identical despite different names*

### Comparing `SNAKES-0.9.30/version.py` & `SNAKES-0.9.31/version.py`

 * *Files identical despite different names*

