# Comparing `tmp/quark-engine-23.3.1.tar.gz` & `tmp/quark-engine-23.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quark-engine-23.3.1.tar", last modified: Tue Mar 28 07:09:46 2023, max compression
+gzip compressed data, was "quark-engine-23.4.1.tar", last modified: Wed Apr 26 07:28:06 2023, max compression
```

## Comparing `quark-engine-23.3.1.tar` & `quark-engine-23.4.1.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 07:09:46.635993 quark-engine-23.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-28 07:09:31.000000 quark-engine-23.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9189 2023-03-28 07:09:46.635993 quark-engine-23.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8644 2023-03-28 07:09:31.000000 quark-engine-23.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 07:09:46.631993 quark-engine-23.3.1/quark/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-28 07:09:31.000000 quark-engine-23.3.1/quark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13512 2023-03-28 07:09:31.000000 quark-engine-23.3.1/quark/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-03-28 07:09:31.000000 quark-engine-23.3.1/quark/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 07:09:46.631993 quark-engine-23.3.1/quark/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 07:09:31.000000 quark-engine-23.3.1/quark/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-03-28 07:09:31.000000 quark-engine-23.3.1/quark/core/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    11054 2023-03-28 07:09:31.000000 quark-engine-23.3.1/quark/core/apkinfo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 07:09:46.631993 quark-engine-23.3.1/quark/core/axmlreader/
--rw-r--r--   0 runner    (1001) docker     (123)    12946 2023-03-28 07:09:31.000000 quark-engine-23.3.1/quark/core/axmlreader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-03-28 07:09:31.000000 quark-engine-23.3.1/quark/core/axmlreader/axml_definition
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 07:09:46.631993 quark-engine-23.3.1/quark/core/interface/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 07:09:31.000000 quark-engine-23.3.1/quark/core/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6000 2023-03-28 07:09:31.000000 quark-engine-23.3.1/quark/core/interface/baseapkinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-03-28 07:09:31.000000 quark-engine-23.3.1/quark/core/parallelquark.py
--rw-r--r--   0 runner    (1001) docker     (123)    30135 2023-03-28 07:09:31.000000 quark-engine-23.3.1/quark/core/quark.py
--rw-r--r--   0 runner    (1001) docker     (123)    19589 2023-03-28 07:09:31.000000 quark-engine-23.3.1/quark/core/rzapkinfo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 07:09:46.631993 quark-engine-23.3.1/quark/core/struct/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 07:09:31.000000 quark-engine-23.3.1/quark/core/struct/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-03-28 07:09:31.000000 quark-engine-23.3.1/quark/core/struct/bytecodeobject.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-03-28 07:09:31.000000 quark-engine-23.3.1/quark/core/struct/methodobject.py
--rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-03-28 07:09:31.000000 quark-engine-23.3.1/quark/core/struct/registerobject.py
--rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-03-28 07:09:31.000000 quark-engine-23.3.1/quark/core/struct/ruleobject.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-03-28 07:09:31.000000 quark-engine-23.3.1/quark/core/struct/tableobject.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 07:09:46.631993 quark-engine-23.3.1/quark/evaluator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 07:09:31.000000 quark-engine-23.3.1/quark/evaluator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25228 2023-03-28 07:09:31.000000 quark-engine-23.3.1/quark/evaluator/pyeval.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 07:09:46.631993 quark-engine-23.3.1/quark/forensic/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-28 07:09:31.000000 quark-engine-23.3.1/quark/forensic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-03-28 07:09:31.000000 quark-engine-23.3.1/quark/forensic/forensic.py
--rw-r--r--   0 runner    (1001) docker     (123)     7219 2023-03-28 07:09:31.000000 quark-engine-23.3.1/quark/forensic/vt_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-03-28 07:09:31.000000 quark-engine-23.3.1/quark/freshquark.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-03-28 07:09:31.000000 quark-engine-23.3.1/quark/logo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-03-28 07:09:31.000000 quark-engine-23.3.1/quark/radiocontrast.py
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-03-28 07:09:31.000000 quark-engine-23.3.1/quark/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-03-28 07:09:31.000000 quark-engine-23.3.1/quark/rulegeneration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 07:09:46.631993 quark-engine-23.3.1/quark/script/
--rw-r--r--   0 runner    (1001) docker     (123)    18224 2023-03-28 07:09:31.000000 quark-engine-23.3.1/quark/script/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-03-28 07:09:31.000000 quark-engine-23.3.1/quark/script/ciphey.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 07:09:46.635993 quark-engine-23.3.1/quark/script/frida/
--rw-r--r--   0 runner    (1001) docker     (123)     6946 2023-03-28 07:09:31.000000 quark-engine-23.3.1/quark/script/frida/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-03-28 07:09:31.000000 quark-engine-23.3.1/quark/script/frida/agent.js
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-03-28 07:09:31.000000 quark-engine-23.3.1/quark/script/objection.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-03-28 07:09:31.000000 quark-engine-23.3.1/quark/script/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 07:09:46.635993 quark-engine-23.3.1/quark/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 07:09:31.000000 quark-engine-23.3.1/quark/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-03-28 07:09:31.000000 quark-engine-23.3.1/quark/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     9510 2023-03-28 07:09:31.000000 quark-engine-23.3.1/quark/utils/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-03-28 07:09:31.000000 quark-engine-23.3.1/quark/utils/output.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-03-28 07:09:31.000000 quark-engine-23.3.1/quark/utils/pprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-03-28 07:09:31.000000 quark-engine-23.3.1/quark/utils/regex.py
--rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-03-28 07:09:31.000000 quark-engine-23.3.1/quark/utils/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-03-28 07:09:31.000000 quark-engine-23.3.1/quark/utils/weight.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 07:09:46.635993 quark-engine-23.3.1/quark/webreport/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 07:09:31.000000 quark-engine-23.3.1/quark/webreport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21921 2023-03-28 07:09:31.000000 quark-engine-23.3.1/quark/webreport/analysis_report_layout.html
--rw-r--r--   0 runner    (1001) docker     (123)    10416 2023-03-28 07:09:31.000000 quark-engine-23.3.1/quark/webreport/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)    24449 2023-03-28 07:09:31.000000 quark-engine-23.3.1/quark/webreport/genrule_report_layout.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 07:09:46.635993 quark-engine-23.3.1/quark_engine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9189 2023-03-28 07:09:46.000000 quark-engine-23.3.1/quark_engine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-03-28 07:09:46.000000 quark-engine-23.3.1/quark_engine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 07:09:46.000000 quark-engine-23.3.1/quark_engine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-28 07:09:46.000000 quark-engine-23.3.1/quark_engine.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-28 07:09:46.000000 quark-engine-23.3.1/quark_engine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-28 07:09:46.000000 quark-engine-23.3.1/quark_engine.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-28 07:09:46.635993 quark-engine-23.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-03-28 07:09:31.000000 quark-engine-23.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 07:09:46.635993 quark-engine-23.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 07:09:31.000000 quark-engine-23.3.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-03-28 07:09:31.000000 quark-engine-23.3.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-03-28 07:09:31.000000 quark-engine-23.3.1/tests/test_freshquark.py
--rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-03-28 07:09:31.000000 quark-engine-23.3.1/tests/test_report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:28:06.557241 quark-engine-23.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-26 07:27:50.000000 quark-engine-23.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9189 2023-04-26 07:28:06.557241 quark-engine-23.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8644 2023-04-26 07:27:50.000000 quark-engine-23.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:28:06.553241 quark-engine-23.4.1/quark/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13512 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:28:06.553241 quark-engine-23.4.1/quark/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/core/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11451 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/core/apkinfo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:28:06.553241 quark-engine-23.4.1/quark/core/axmlreader/
+-rw-r--r--   0 runner    (1001) docker     (123)    12946 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/core/axmlreader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/core/axmlreader/axml_definition
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:28:06.553241 quark-engine-23.4.1/quark/core/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/core/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/core/interface/baseapkinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/core/parallelquark.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30135 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/core/quark.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19911 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/core/rzapkinfo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:28:06.557241 quark-engine-23.4.1/quark/core/struct/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/core/struct/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/core/struct/bytecodeobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/core/struct/methodobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/core/struct/registerobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/core/struct/ruleobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/core/struct/tableobject.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:28:06.557241 quark-engine-23.4.1/quark/evaluator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/evaluator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25228 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/evaluator/pyeval.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:28:06.557241 quark-engine-23.4.1/quark/forensic/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/forensic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/forensic/forensic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7219 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/forensic/vt_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/freshquark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/logo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/radiocontrast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/rulegeneration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:28:06.557241 quark-engine-23.4.1/quark/script/
+-rw-r--r--   0 runner    (1001) docker     (123)    18224 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/script/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/script/ciphey.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:28:06.557241 quark-engine-23.4.1/quark/script/frida/
+-rw-r--r--   0 runner    (1001) docker     (123)     6946 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/script/frida/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/script/frida/agent.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/script/objection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/script/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:28:06.557241 quark-engine-23.4.1/quark/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9510 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/utils/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/utils/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/utils/pprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/utils/regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/utils/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/utils/weight.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:28:06.557241 quark-engine-23.4.1/quark/webreport/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/webreport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21921 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/webreport/analysis_report_layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10416 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/webreport/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24449 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/webreport/genrule_report_layout.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:28:06.557241 quark-engine-23.4.1/quark_engine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9189 2023-04-26 07:28:06.000000 quark-engine-23.4.1/quark_engine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-04-26 07:28:06.000000 quark-engine-23.4.1/quark_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 07:28:06.000000 quark-engine-23.4.1/quark_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-26 07:28:06.000000 quark-engine-23.4.1/quark_engine.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-26 07:28:06.000000 quark-engine-23.4.1/quark_engine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-26 07:28:06.000000 quark-engine-23.4.1/quark_engine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 07:28:06.557241 quark-engine-23.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-26 07:27:51.000000 quark-engine-23.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:28:06.557241 quark-engine-23.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:27:51.000000 quark-engine-23.4.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-04-26 07:27:51.000000 quark-engine-23.4.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-26 07:27:51.000000 quark-engine-23.4.1/tests/test_freshquark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-04-26 07:27:51.000000 quark-engine-23.4.1/tests/test_report.py
```

### Comparing `quark-engine-23.3.1/LICENSE` & `quark-engine-23.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `quark-engine-23.3.1/PKG-INFO` & `quark-engine-23.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quark-engine
-Version: 23.3.1
+Version: 23.4.1
 Summary: An Obfuscation-Neglect Android Malware Scoring System
 Home-page: https://github.com/quark-engine/quark-engine
 Author: YuShiang Dang, ShengFeng Lu, KunYu Chen
 Author-email: pulorsok@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: quark-engine Version: 23.3.1 Summary: An
+Metadata-Version: 2.1 Name: quark-engine Version: 23.4.1 Summary: An
 Obfuscation-Neglect Android Malware Scoring System Home-page: https://
 github.com/quark-engine/quark-engine Author: YuShiang Dang, ShengFeng Lu, KunYu
 Chen Author-email: pulorsok@gmail.com Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: GNU General Public License
 v3 (GPLv3) Classifier: Operating System :: OS Independent Classifier: Topic ::
 Security Requires-Python: >=3.8 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `quark-engine-23.3.1/README.md` & `quark-engine-23.4.1/README.md`

 * *Files identical despite different names*

### Comparing `quark-engine-23.3.1/quark/cli.py` & `quark-engine-23.4.1/quark/cli.py`

 * *Files identical despite different names*

### Comparing `quark-engine-23.3.1/quark/core/analysis.py` & `quark-engine-23.4.1/quark/core/analysis.py`

 * *Files identical despite different names*

### Comparing `quark-engine-23.3.1/quark/core/apkinfo.py` & `quark-engine-23.4.1/quark/core/apkinfo.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,29 @@
 
         manifest_root = self.apk.get_android_manifest_xml()
         application = manifest_root.find("application")
 
         return application.findall("activity")
 
     @property
+    def receivers(self) -> List[XMLElement]:
+        """
+        Return all receivers from the given APK.
+
+        :return: a list of all receivers
+        """
+        if self.ret_type == "DEX":
+            return []
+
+        manifest_root = self.apk.get_android_manifest_xml()
+        application = manifest_root.find("application")
+
+        return application.findall("receiver")
+
+    @property
     def android_apis(self) -> Set[MethodObject]:
         apis = set()
 
         for external_cls in self.analysis.get_external_classes():
             for meth_analysis in external_cls.get_methods():
                 if meth_analysis.is_android_api():
                     apis.add(meth_analysis)
```

### Comparing `quark-engine-23.3.1/quark/core/axmlreader/__init__.py` & `quark-engine-23.4.1/quark/core/axmlreader/__init__.py`

 * *Files identical despite different names*

### Comparing `quark-engine-23.3.1/quark/core/axmlreader/axml_definition` & `quark-engine-23.4.1/quark/core/axmlreader/axml_definition`

 * *Files identical despite different names*

### Comparing `quark-engine-23.3.1/quark/core/interface/baseapkinfo.py` & `quark-engine-23.4.1/quark/core/interface/baseapkinfo.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,14 +87,24 @@
 
         :return: a list of all activities
         """
         pass
 
     @property
     @abstractmethod
+    def receivers(self) -> List[XMLElement]:
+        """
+        Return all receivers from the given APK.
+
+        :return: a list of all receivers
+        """
+        pass
+
+    @property
+    @abstractmethod
     def android_apis(self) -> Set[MethodObject]:
         """
         Return all Android native APIs from given APK.
 
         :return: a set of all Android native APIs MethodObject
         """
         pass
```

### Comparing `quark-engine-23.3.1/quark/core/parallelquark.py` & `quark-engine-23.4.1/quark/core/parallelquark.py`

 * *Files identical despite different names*

### Comparing `quark-engine-23.3.1/quark/core/quark.py` & `quark-engine-23.4.1/quark/core/quark.py`

 * *Files identical despite different names*

### Comparing `quark-engine-23.3.1/quark/core/rzapkinfo.py` & `quark-engine-23.4.1/quark/core/rzapkinfo.py`

 * *Files 1% similar despite different names*

```diff
@@ -264,14 +264,26 @@
         :return: a list of all activities
         """
         axml = AxmlReader(self._manifest)
         root = axml.get_xml_tree()
 
         return root.findall("application/activity")
 
+    @functools.cached_property
+    def receivers(self) -> List[XMLElement]:
+        """
+        Return all receivers from the given APK.
+
+        :return: a list of all receivers
+        """
+        axml = AxmlReader(self._manifest)
+        root = axml.get_xml_tree()
+
+        return root.findall("application/receiver")
+
     @property
     def android_apis(self) -> Set[MethodObject]:
         return {
             method
             for method in self.all_methods
             if method.is_android_api() and method.cache.is_imported
         }
```

### Comparing `quark-engine-23.3.1/quark/core/struct/bytecodeobject.py` & `quark-engine-23.4.1/quark/core/struct/bytecodeobject.py`

 * *Files identical despite different names*

### Comparing `quark-engine-23.3.1/quark/core/struct/methodobject.py` & `quark-engine-23.4.1/quark/core/struct/methodobject.py`

 * *Files identical despite different names*

### Comparing `quark-engine-23.3.1/quark/core/struct/registerobject.py` & `quark-engine-23.4.1/quark/core/struct/registerobject.py`

 * *Files identical despite different names*

### Comparing `quark-engine-23.3.1/quark/core/struct/ruleobject.py` & `quark-engine-23.4.1/quark/core/struct/ruleobject.py`

 * *Files identical despite different names*

### Comparing `quark-engine-23.3.1/quark/core/struct/tableobject.py` & `quark-engine-23.4.1/quark/core/struct/tableobject.py`

 * *Files identical despite different names*

### Comparing `quark-engine-23.3.1/quark/evaluator/pyeval.py` & `quark-engine-23.4.1/quark/evaluator/pyeval.py`

 * *Files identical despite different names*

### Comparing `quark-engine-23.3.1/quark/forensic/forensic.py` & `quark-engine-23.4.1/quark/forensic/forensic.py`

 * *Files identical despite different names*

### Comparing `quark-engine-23.3.1/quark/forensic/vt_analysis.py` & `quark-engine-23.4.1/quark/forensic/vt_analysis.py`

 * *Files identical despite different names*

### Comparing `quark-engine-23.3.1/quark/freshquark.py` & `quark-engine-23.4.1/quark/freshquark.py`

 * *Files identical despite different names*

### Comparing `quark-engine-23.3.1/quark/logo.py` & `quark-engine-23.4.1/quark/logo.py`

 * *Files identical despite different names*

### Comparing `quark-engine-23.3.1/quark/radiocontrast.py` & `quark-engine-23.4.1/quark/radiocontrast.py`

 * *Files identical despite different names*

### Comparing `quark-engine-23.3.1/quark/report.py` & `quark-engine-23.4.1/quark/report.py`

 * *Files identical despite different names*

### Comparing `quark-engine-23.3.1/quark/rulegeneration.py` & `quark-engine-23.4.1/quark/rulegeneration.py`

 * *Files identical despite different names*

### Comparing `quark-engine-23.3.1/quark/script/__init__.py` & `quark-engine-23.4.1/quark/script/__init__.py`

 * *Files identical despite different names*

### Comparing `quark-engine-23.3.1/quark/script/frida/__init__.py` & `quark-engine-23.4.1/quark/script/frida/__init__.py`

 * *Files identical despite different names*

### Comparing `quark-engine-23.3.1/quark/script/frida/agent.js` & `quark-engine-23.4.1/quark/script/frida/agent.js`

 * *Files identical despite different names*

### Comparing `quark-engine-23.3.1/quark/script/objection.py` & `quark-engine-23.4.1/quark/script/objection.py`

 * *Files identical despite different names*

### Comparing `quark-engine-23.3.1/quark/utils/colors.py` & `quark-engine-23.4.1/quark/utils/colors.py`

 * *Files identical despite different names*

### Comparing `quark-engine-23.3.1/quark/utils/graph.py` & `quark-engine-23.4.1/quark/utils/graph.py`

 * *Files identical despite different names*

### Comparing `quark-engine-23.3.1/quark/utils/output.py` & `quark-engine-23.4.1/quark/utils/output.py`

 * *Files identical despite different names*

### Comparing `quark-engine-23.3.1/quark/utils/pprint.py` & `quark-engine-23.4.1/quark/utils/pprint.py`

 * *Files identical despite different names*

### Comparing `quark-engine-23.3.1/quark/utils/regex.py` & `quark-engine-23.4.1/quark/utils/regex.py`

 * *Files identical despite different names*

### Comparing `quark-engine-23.3.1/quark/utils/tools.py` & `quark-engine-23.4.1/quark/utils/tools.py`

 * *Files identical despite different names*

### Comparing `quark-engine-23.3.1/quark/utils/weight.py` & `quark-engine-23.4.1/quark/utils/weight.py`

 * *Files identical despite different names*

### Comparing `quark-engine-23.3.1/quark/webreport/analysis_report_layout.html` & `quark-engine-23.4.1/quark/webreport/analysis_report_layout.html`

 * *Files identical despite different names*

### Comparing `quark-engine-23.3.1/quark/webreport/generate.py` & `quark-engine-23.4.1/quark/webreport/generate.py`

 * *Files identical despite different names*

### Comparing `quark-engine-23.3.1/quark/webreport/genrule_report_layout.html` & `quark-engine-23.4.1/quark/webreport/genrule_report_layout.html`

 * *Files identical despite different names*

### Comparing `quark-engine-23.3.1/quark_engine.egg-info/PKG-INFO` & `quark-engine-23.4.1/quark_engine.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quark-engine
-Version: 23.3.1
+Version: 23.4.1
 Summary: An Obfuscation-Neglect Android Malware Scoring System
 Home-page: https://github.com/quark-engine/quark-engine
 Author: YuShiang Dang, ShengFeng Lu, KunYu Chen
 Author-email: pulorsok@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: quark-engine Version: 23.3.1 Summary: An
+Metadata-Version: 2.1 Name: quark-engine Version: 23.4.1 Summary: An
 Obfuscation-Neglect Android Malware Scoring System Home-page: https://
 github.com/quark-engine/quark-engine Author: YuShiang Dang, ShengFeng Lu, KunYu
 Chen Author-email: pulorsok@gmail.com Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: GNU General Public License
 v3 (GPLv3) Classifier: Operating System :: OS Independent Classifier: Topic ::
 Security Requires-Python: >=3.8 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `quark-engine-23.3.1/quark_engine.egg-info/SOURCES.txt` & `quark-engine-23.4.1/quark_engine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quark-engine-23.3.1/setup.py` & `quark-engine-23.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `quark-engine-23.3.1/tests/conftest.py` & `quark-engine-23.4.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `quark-engine-23.3.1/tests/test_freshquark.py` & `quark-engine-23.4.1/tests/test_freshquark.py`

 * *Files identical despite different names*

### Comparing `quark-engine-23.3.1/tests/test_report.py` & `quark-engine-23.4.1/tests/test_report.py`

 * *Files identical despite different names*

