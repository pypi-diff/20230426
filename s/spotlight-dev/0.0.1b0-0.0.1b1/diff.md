# Comparing `tmp/spotlight-dev-0.0.1b0.tar.gz` & `tmp/spotlight-dev-0.0.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotlight-dev-0.0.1b0.tar", last modified: Mon Apr 24 22:32:01 2023, max compression
+gzip compressed data, was "spotlight-dev-0.0.1b1.tar", last modified: Wed Apr 26 18:04:38 2023, max compression
```

## Comparing `spotlight-dev-0.0.1b0.tar` & `spotlight-dev-0.0.1b1.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 22:32:01.379802 spotlight-dev-0.0.1b0/
--rw-r--r--   0 root         (0) root         (0)      989 2023-04-24 22:32:01.378802 spotlight-dev-0.0.1b0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      460 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-24 22:32:01.379802 spotlight-dev-0.0.1b0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1368 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 22:32:01.353800 spotlight-dev-0.0.1b0/spotlight/
--rw-rw-rw-   0 root         (0) root         (0)       44 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 22:32:01.354800 spotlight-dev-0.0.1b0/spotlight/api/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 22:32:01.355800 spotlight-dev-0.0.1b0/spotlight/api/auth/
--rw-rw-rw-   0 root         (0) root         (0)      214 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/api/auth/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1340 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/api/auth/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     2262 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/api/auth/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)     1726 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/api/auth/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 22:32:01.356800 spotlight-dev-0.0.1b0/spotlight/api/group/
--rw-rw-rw-   0 root         (0) root         (0)      355 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/api/group/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1589 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/api/group/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     4809 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/api/group/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      412 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/api/group/model.py
--rw-rw-rw-   0 root         (0) root         (0)     4284 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/api/group/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 22:32:01.358801 spotlight-dev-0.0.1b0/spotlight/api/group/view/
--rw-rw-rw-   0 root         (0) root         (0)      127 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/api/group/view/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      257 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/api/group/view/__util.py
--rw-rw-rw-   0 root         (0) root         (0)      989 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/api/group/view/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      379 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/api/group/view/model.py
--rw-rw-rw-   0 root         (0) root         (0)      893 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/api/group/view/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 22:32:01.359801 spotlight-dev-0.0.1b0/spotlight/api/job/
--rw-rw-rw-   0 root         (0) root         (0)      273 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/api/job/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      927 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/api/job/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     2977 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/api/job/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      850 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/api/job/model.py
--rw-rw-rw-   0 root         (0) root         (0)     2631 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/api/job/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 22:32:01.361801 spotlight-dev-0.0.1b0/spotlight/api/job/view/
--rw-rw-rw-   0 root         (0) root         (0)      127 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/api/job/view/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       98 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/api/job/view/__util.py
--rw-rw-rw-   0 root         (0) root         (0)      547 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/api/job/view/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      482 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/api/job/view/model.py
--rw-rw-rw-   0 root         (0) root         (0)      508 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/api/job/view/synchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      240 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/api/model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 22:32:01.362801 spotlight-dev-0.0.1b0/spotlight/api/rule/
--rw-rw-rw-   0 root         (0) root         (0)      158 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/api/rule/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1327 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/api/rule/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     4035 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/api/rule/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      820 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/api/rule/model.py
--rw-rw-rw-   0 root         (0) root         (0)     3593 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/api/rule/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 22:32:01.362801 spotlight-dev-0.0.1b0/spotlight/core/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 22:32:01.364801 spotlight-dev-0.0.1b0/spotlight/core/common/
--rw-rw-rw-   0 root         (0) root         (0)       47 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/core/common/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2648 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/core/common/base.py
--rw-rw-rw-   0 root         (0) root         (0)      230 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/core/common/base_enum.py
--rw-rw-rw-   0 root         (0) root         (0)     2718 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/core/common/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 22:32:01.364801 spotlight-dev-0.0.1b0/spotlight/core/common/date/
--rw-rw-rw-   0 root         (0) root         (0)      206 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/core/common/date/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2478 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/core/common/date/function.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 22:32:01.365801 spotlight-dev-0.0.1b0/spotlight/core/common/decorators/
--rw-rw-rw-   0 root         (0) root         (0)      344 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/core/common/decorators/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 22:32:01.366801 spotlight-dev-0.0.1b0/spotlight/core/common/decorators/authorization/
--rw-rw-rw-   0 root         (0) root         (0)      253 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/core/common/decorators/authorization/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1154 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/core/common/decorators/authorization/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     3920 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/core/common/decorators/authorization/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)     3898 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/core/common/decorators/authorization/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 22:32:01.367801 spotlight-dev-0.0.1b0/spotlight/core/common/decorators/data/
--rw-rw-rw-   0 root         (0) root         (0)      190 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/core/common/decorators/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      696 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/core/common/decorators/data/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     1401 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/core/common/decorators/data/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)     1399 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/core/common/decorators/data/synchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      686 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/core/common/decorators/timeit.py
--rw-rw-rw-   0 root         (0) root         (0)      271 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/core/common/enum.py
--rw-rw-rw-   0 root         (0) root         (0)      726 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/core/common/errors.py
--rw-rw-rw-   0 root         (0) root         (0)     4794 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/core/common/function.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 22:32:01.368801 spotlight-dev-0.0.1b0/spotlight/core/common/metaclass/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/core/common/metaclass/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      924 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/core/common/metaclass/singleton.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 22:32:01.369802 spotlight-dev-0.0.1b0/spotlight/core/common/requests/
--rw-rw-rw-   0 root         (0) root         (0)      403 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/core/common/requests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4689 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/core/common/requests/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)     3788 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/core/common/requests/synchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      241 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/core/common/type.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 22:32:01.369802 spotlight-dev-0.0.1b0/spotlight/core/pipeline/
--rw-rw-rw-   0 root         (0) root         (0)     6188 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/core/pipeline/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 22:32:01.370802 spotlight-dev-0.0.1b0/spotlight/core/pipeline/execution/
--rw-rw-rw-   0 root         (0) root         (0)       71 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/core/pipeline/execution/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 22:32:01.371802 spotlight-dev-0.0.1b0/spotlight/core/pipeline/execution/plugin/
--rw-rw-rw-   0 root         (0) root         (0)      224 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/core/pipeline/execution/plugin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1203 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/core/pipeline/execution/plugin/abstract.py
--rw-rw-rw-   0 root         (0) root         (0)     1506 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/core/pipeline/execution/plugin/decorator.py
--rw-rw-rw-   0 root         (0) root         (0)     1079 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/core/pipeline/execution/plugin/registry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 22:32:01.373802 spotlight-dev-0.0.1b0/spotlight/core/pipeline/execution/rule/
--rw-rw-rw-   0 root         (0) root         (0)      178 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/core/pipeline/execution/rule/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1511 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/core/pipeline/execution/rule/abstract.py
--rw-rw-rw-   0 root         (0) root         (0)      130 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/core/pipeline/execution/rule/enum.py
--rw-rw-rw-   0 root         (0) root         (0)     1185 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/core/pipeline/execution/rule/sql_rule.py
--rw-rw-rw-   0 root         (0) root         (0)     2730 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/core/pipeline/execution/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 22:32:01.374802 spotlight-dev-0.0.1b0/spotlight/core/pipeline/model/
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/core/pipeline/model/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1704 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/core/pipeline/model/pipeline.py
--rw-rw-rw-   0 root         (0) root         (0)      242 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/core/pipeline/model/rule.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 22:32:01.375802 spotlight-dev-0.0.1b0/spotlight/core/pipeline/utils/
--rw-rw-rw-   0 root         (0) root         (0)      178 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/core/pipeline/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3926 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/core/pipeline/utils/asynchronously.py
--rw-rw-rw-   0 root         (0) root         (0)     3717 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/core/pipeline/utils/synchronously.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 22:32:01.376802 spotlight-dev-0.0.1b0/spotlight/pandas/
--rw-rw-rw-   0 root         (0) root         (0)       50 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/pandas/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1663 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/pandas/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     1157 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/pandas/plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     1982 2023-04-24 22:31:48.000000 spotlight-dev-0.0.1b0/spotlight/pandas/runners.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 22:32:01.378802 spotlight-dev-0.0.1b0/spotlight_dev.egg-info/
--rw-r--r--   0 root         (0) root         (0)      989 2023-04-24 22:32:01.000000 spotlight-dev-0.0.1b0/spotlight_dev.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3272 2023-04-24 22:32:01.000000 spotlight-dev-0.0.1b0/spotlight_dev.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 22:32:01.000000 spotlight-dev-0.0.1b0/spotlight_dev.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      227 2023-04-24 22:32:01.000000 spotlight-dev-0.0.1b0/spotlight_dev.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-04-24 22:32:01.000000 spotlight-dev-0.0.1b0/spotlight_dev.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 18:04:38.586662 spotlight-dev-0.0.1b1/
+-rw-r--r--   0 root         (0) root         (0)     1413 2023-04-26 18:04:38.586662 spotlight-dev-0.0.1b1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      852 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-26 18:04:38.586662 spotlight-dev-0.0.1b1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1368 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 18:04:38.542659 spotlight-dev-0.0.1b1/spotlight/
+-rw-rw-rw-   0 root         (0) root         (0)       44 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 18:04:38.542659 spotlight-dev-0.0.1b1/spotlight/api/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 18:04:38.544659 spotlight-dev-0.0.1b1/spotlight/api/auth/
+-rw-rw-rw-   0 root         (0) root         (0)      214 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/api/auth/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1340 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/api/auth/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     2262 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/api/auth/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)     1726 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/api/auth/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 18:04:38.546659 spotlight-dev-0.0.1b1/spotlight/api/job/
+-rw-rw-rw-   0 root         (0) root         (0)      273 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/api/job/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      927 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/api/job/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     2975 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/api/job/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      772 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/api/job/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     2629 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/api/job/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 18:04:38.549660 spotlight-dev-0.0.1b1/spotlight/api/job/view/
+-rw-rw-rw-   0 root         (0) root         (0)      127 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/api/job/view/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       98 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/api/job/view/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)      547 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/api/job/view/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      454 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/api/job/view/model.py
+-rw-rw-rw-   0 root         (0) root         (0)      508 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/api/job/view/synchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      236 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/api/model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 18:04:38.551660 spotlight-dev-0.0.1b1/spotlight/api/rule/
+-rw-rw-rw-   0 root         (0) root         (0)      158 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/api/rule/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1317 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/api/rule/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     4007 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/api/rule/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      734 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/api/rule/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     3565 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/api/rule/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 18:04:38.554660 spotlight-dev-0.0.1b1/spotlight/api/tag/
+-rw-rw-rw-   0 root         (0) root         (0)      327 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/api/tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1535 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/api/tag/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     4659 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/api/tag/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      341 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/api/tag/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     4134 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/api/tag/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 18:04:38.557660 spotlight-dev-0.0.1b1/spotlight/api/tag/view/
+-rw-rw-rw-   0 root         (0) root         (0)      127 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/api/tag/view/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      249 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/api/tag/view/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)      963 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/api/tag/view/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      347 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/api/tag/view/model.py
+-rw-rw-rw-   0 root         (0) root         (0)      867 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/api/tag/view/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 18:04:38.558660 spotlight-dev-0.0.1b1/spotlight/core/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 18:04:38.563661 spotlight-dev-0.0.1b1/spotlight/core/common/
+-rw-rw-rw-   0 root         (0) root         (0)       47 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/common/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2648 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/common/base.py
+-rw-rw-rw-   0 root         (0) root         (0)      230 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/common/base_enum.py
+-rw-rw-rw-   0 root         (0) root         (0)     2718 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/common/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 18:04:38.564661 spotlight-dev-0.0.1b1/spotlight/core/common/date/
+-rw-rw-rw-   0 root         (0) root         (0)      206 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/common/date/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2478 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/common/date/function.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 18:04:38.564661 spotlight-dev-0.0.1b1/spotlight/core/common/decorators/
+-rw-rw-rw-   0 root         (0) root         (0)      344 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/common/decorators/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 18:04:38.567661 spotlight-dev-0.0.1b1/spotlight/core/common/decorators/authorization/
+-rw-rw-rw-   0 root         (0) root         (0)      253 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/common/decorators/authorization/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1154 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/common/decorators/authorization/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     3920 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/common/decorators/authorization/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)     3898 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/common/decorators/authorization/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 18:04:38.570661 spotlight-dev-0.0.1b1/spotlight/core/common/decorators/data/
+-rw-rw-rw-   0 root         (0) root         (0)      190 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/common/decorators/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      696 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/common/decorators/data/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     1401 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/common/decorators/data/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)     1399 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/common/decorators/data/synchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      686 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/common/decorators/timeit.py
+-rw-rw-rw-   0 root         (0) root         (0)      271 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/common/enum.py
+-rw-rw-rw-   0 root         (0) root         (0)      726 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/common/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     4794 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/common/function.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 18:04:38.571661 spotlight-dev-0.0.1b1/spotlight/core/common/metaclass/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/common/metaclass/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      924 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/common/metaclass/singleton.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 18:04:38.573661 spotlight-dev-0.0.1b1/spotlight/core/common/requests/
+-rw-rw-rw-   0 root         (0) root         (0)      403 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/common/requests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4689 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/common/requests/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)     3788 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/common/requests/synchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      241 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/common/type.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 18:04:38.573661 spotlight-dev-0.0.1b1/spotlight/core/pipeline/
+-rw-rw-rw-   0 root         (0) root         (0)     5930 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/pipeline/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 18:04:38.574662 spotlight-dev-0.0.1b1/spotlight/core/pipeline/execution/
+-rw-rw-rw-   0 root         (0) root         (0)       71 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/pipeline/execution/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 18:04:38.576662 spotlight-dev-0.0.1b1/spotlight/core/pipeline/execution/plugin/
+-rw-rw-rw-   0 root         (0) root         (0)      224 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/pipeline/execution/plugin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1203 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/pipeline/execution/plugin/abstract.py
+-rw-rw-rw-   0 root         (0) root         (0)     1506 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/pipeline/execution/plugin/decorator.py
+-rw-rw-rw-   0 root         (0) root         (0)     1063 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/pipeline/execution/plugin/registry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 18:04:38.578662 spotlight-dev-0.0.1b1/spotlight/core/pipeline/execution/rule/
+-rw-rw-rw-   0 root         (0) root         (0)      178 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/pipeline/execution/rule/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1511 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/pipeline/execution/rule/abstract.py
+-rw-rw-rw-   0 root         (0) root         (0)      130 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/pipeline/execution/rule/enum.py
+-rw-rw-rw-   0 root         (0) root         (0)     1185 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/pipeline/execution/rule/sql_rule.py
+-rw-rw-rw-   0 root         (0) root         (0)     2730 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/pipeline/execution/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 18:04:38.579662 spotlight-dev-0.0.1b1/spotlight/core/pipeline/model/
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/pipeline/model/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1704 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/pipeline/model/pipeline.py
+-rw-rw-rw-   0 root         (0) root         (0)      213 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/pipeline/model/rule.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 18:04:38.581662 spotlight-dev-0.0.1b1/spotlight/core/pipeline/utils/
+-rw-rw-rw-   0 root         (0) root         (0)      178 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/pipeline/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3573 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/pipeline/utils/asynchronously.py
+-rw-rw-rw-   0 root         (0) root         (0)     3356 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/pipeline/utils/synchronously.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 18:04:38.583662 spotlight-dev-0.0.1b1/spotlight/pandas/
+-rw-rw-rw-   0 root         (0) root         (0)       50 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/pandas/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1663 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/pandas/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     1157 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/pandas/plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     1982 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/pandas/runners.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 18:04:38.585662 spotlight-dev-0.0.1b1/spotlight_dev.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1413 2023-04-26 18:04:38.000000 spotlight-dev-0.0.1b1/spotlight_dev.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3252 2023-04-26 18:04:38.000000 spotlight-dev-0.0.1b1/spotlight_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 18:04:38.000000 spotlight-dev-0.0.1b1/spotlight_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      227 2023-04-26 18:04:38.000000 spotlight-dev-0.0.1b1/spotlight_dev.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-04-26 18:04:38.000000 spotlight-dev-0.0.1b1/spotlight_dev.egg-info/top_level.txt
```

### Comparing `spotlight-dev-0.0.1b0/setup.py` & `spotlight-dev-0.0.1b1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     tag = subprocess.getoutput('git tag --sort=version:refname | tail -n1')
     commits = subprocess.getoutput(f'git rev-list {tag}..HEAD --count')
     return f'{tag}.{commits}'
 
 
 setuptools.setup(
     name="spotlight-dev",
-    version="0.0.1b0",
+    version="0.0.1b1",
     author="Spotlight",
     author_email="hello@spotlight.dev",
     description="Spotlight Python SDK",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://alpha.dev",
     classifiers=[
```

### Comparing `spotlight-dev-0.0.1b0/spotlight/api/auth/__util.py` & `spotlight-dev-0.0.1b1/spotlight/api/auth/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b0/spotlight/api/auth/asynchronous.py` & `spotlight-dev-0.0.1b1/spotlight/api/auth/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b0/spotlight/api/auth/synchronous.py` & `spotlight-dev-0.0.1b1/spotlight/api/auth/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b0/spotlight/api/group/__util.py` & `spotlight-dev-0.0.1b1/spotlight/api/tag/__util.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 from spotlight.api.model import SearchRequest, LookupRequest
-from spotlight.api.group.model import GroupRequest
+from spotlight.api.tag.model import TagRequest
 
 
-def _get_group_request_info(id: str) -> dict:
-    return {"endpoint": f"config/datawatch/group/{id}"}
+def _get_tag_request_info(id: str) -> dict:
+    return {"endpoint": f"config/spotlight/tag/{id}"}
 
 
-def _get_group_by_name_request_info(name: str) -> dict:
-    return {"endpoint": f"config/datawatch/group", "params": {"name": name}}
+def _get_tag_by_name_request_info(name: str) -> dict:
+    return {"endpoint": f"config/spotlight/tag", "params": {"name": name}}
 
 
-def _get_groups_request_info() -> dict:
-    return {"endpoint": f"config/datawatch/group"}
+def _get_tags_request_info() -> dict:
+    return {"endpoint": f"config/spotlight/tag"}
 
 
-def _get_groups_by_lookup_request_info(request: LookupRequest) -> dict:
-    return {"endpoint": f"config/datawatch/group", "json": request.request_dict()}
+def _get_tags_by_lookup_request_info(request: LookupRequest) -> dict:
+    return {"endpoint": f"config/spotlight/tag", "json": request.request_dict()}
 
 
-def _get_groups_by_rule_id_request_info(rule_id: str) -> dict:
-    return {"endpoint": f"config/datawatch/group", "params": {"rule_id": rule_id}}
+def _get_tags_by_rule_id_request_info(rule_id: str) -> dict:
+    return {"endpoint": f"config/spotlight/tag", "params": {"rule_id": rule_id}}
 
 
-def _search_groups_request_info(request: SearchRequest) -> dict:
-    return {"endpoint": f"config/datawatch/group", "json": request.request_dict()}
+def _search_tags_request_info(request: SearchRequest) -> dict:
+    return {"endpoint": f"config/spotlight/tag", "json": request.request_dict()}
 
 
-def _create_group_request_info(request: GroupRequest) -> dict:
-    return {"endpoint": f"config/datawatch/group", "json": request.request_dict()}
+def _create_tag_request_info(request: TagRequest) -> dict:
+    return {"endpoint": f"config/spotlight/tag", "json": request.request_dict()}
 
 
-def _update_group_request_info(id: str, request: GroupRequest) -> dict:
-    return {"endpoint": f"config/datawatch/group/{id}", "json": request.request_dict()}
+def _update_tag_request_info(id: str, request: TagRequest) -> dict:
+    return {"endpoint": f"config/spotlight/tag/{id}", "json": request.request_dict()}
 
 
-def _delete_group_request_info(id: str) -> dict:
-    return {"endpoint": f"config/datawatch/group/{id}"}
+def _delete_tag_request_info(id: str) -> dict:
+    return {"endpoint": f"config/spotlight/tag/{id}"}
 
 
-def _get_group_tags_request_info() -> dict:
-    return {"endpoint": f"config/datawatch/group/tags"}
+def _get_tag_tags_request_info() -> dict:
+    return {"endpoint": f"config/spotlight/tag/tags"}
 
 
-def _unique_group_name_request_info(name: str) -> dict:
+def _unique_tag_name_request_info(name: str) -> dict:
     return {
-        "endpoint": f"config/datawatch/group/unique",
-        "params": {"group_name": name},
+        "endpoint": f"config/spotlight/tag/unique",
+        "params": {"tag_name": name},
     }
```

### Comparing `spotlight-dev-0.0.1b0/spotlight/api/group/asynchronous.py` & `spotlight-dev-0.0.1b1/spotlight/api/tag/asynchronous.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,185 +1,185 @@
 from typing import Dict, Any, List
 
 from spotlight.api.model import SearchRequest, LookupRequest
-from spotlight.api.group.__util import (
-    _get_group_request_info,
-    _get_groups_request_info,
-    _create_group_request_info,
-    _update_group_request_info,
-    _delete_group_request_info,
-    _search_groups_request_info,
-    _unique_group_name_request_info,
-    _get_group_by_name_request_info,
-    _get_groups_by_rule_id_request_info,
-    _get_group_tags_request_info,
-    _get_groups_by_lookup_request_info,
+from spotlight.api.tag.__util import (
+    _get_tag_request_info,
+    _get_tags_request_info,
+    _create_tag_request_info,
+    _update_tag_request_info,
+    _delete_tag_request_info,
+    _search_tags_request_info,
+    _unique_tag_name_request_info,
+    _get_tag_by_name_request_info,
+    _get_tags_by_rule_id_request_info,
+    _get_tag_tags_request_info,
+    _get_tags_by_lookup_request_info,
 )
-from spotlight.api.group.model import GroupRequest
+from spotlight.api.tag.model import TagRequest
 from spotlight.core.common.decorators import async_data_request
 
 from spotlight.core.common.requests import (
     __async_get_request,
     __async_post_request,
     __async_put_request,
     __async_delete_request,
 )
 
 
 @async_data_request
-async def async_get_group(id: str) -> Dict[str, Any]:
+async def async_get_tag(id: str) -> Dict[str, Any]:
     """
-    Asynchronously get group by ID.
+    Asynchronously get tag by ID.
 
     Args:
-        id (str): Group ID
+        id (str): tag ID
 
     Returns:
-        Dict[str, Any]: Group response
+        Dict[str, Any]: tag response
     """
-    request_info = _get_group_request_info(id)
+    request_info = _get_tag_request_info(id)
     return await __async_get_request(**request_info)
 
 
 @async_data_request
-async def async_get_group_by_name(group_name: str) -> Dict[str, Any]:
+async def async_get_tag_by_name(tag_name: str) -> Dict[str, Any]:
     """
-    Asynchronously get group by name.
+    Asynchronously get tag by name.
 
     Args:
-        group_name (str): Group name
+        tag_name (str): tag name
 
     Returns:
-        Dict[str, Any]: Group response
+        Dict[str, Any]: tag response
     """
-    request_info = _get_group_by_name_request_info(group_name)
+    request_info = _get_tag_by_name_request_info(tag_name)
     return await __async_get_request(**request_info)
 
 
 @async_data_request
-async def async_get_groups() -> List[Dict[str, Any]]:
+async def async_get_tags() -> List[Dict[str, Any]]:
     """
-    Asynchronously get all groups.
+    Asynchronously get all tags.
 
     Returns:
-        List[Dict[str, Any]]: List of group responses
+        List[Dict[str, Any]]: List of tag responses
     """
-    request_info = _get_groups_request_info()
+    request_info = _get_tags_request_info()
     return await __async_get_request(**request_info)
 
 
 @async_data_request
-async def async_get_groups_by_lookup(request: LookupRequest) -> List[Dict[str, Any]]:
+async def async_get_tags_by_lookup(request: LookupRequest) -> List[Dict[str, Any]]:
     """
-    Asynchronously get all groups by lookup.
+    Asynchronously get all tags by lookup.
 
     Args:
-        request (LookupRequest): The group information used in the group look up
+        request (LookupRequest): The tag information used in the tag look up
 
     Returns:
-        List[Dict[str, Any]]: List of group responses
+        List[Dict[str, Any]]: List of tag responses
     """
-    request_info = _get_groups_by_lookup_request_info(request)
+    request_info = _get_tags_by_lookup_request_info(request)
     return await __async_post_request(**request_info)
 
 
 @async_data_request
-async def async_get_groups_by_rule_id(rule_id: str) -> List[Dict[str, Any]]:
+async def async_get_tags_by_rule_id(rule_id: str) -> List[Dict[str, Any]]:
     """
-    Asynchronously get all groups by rule ID.
+    Asynchronously get all tags by rule ID.
 
     Args:
         rule_id (str): Rule ID
 
     Returns:
-        List[Dict[str, Any]]: List of group responses
+        List[Dict[str, Any]]: List of tag responses
     """
-    request_info = _get_groups_by_rule_id_request_info(rule_id)
+    request_info = _get_tags_by_rule_id_request_info(rule_id)
     return await __async_get_request(**request_info)
 
 
 @async_data_request
-async def async_search_groups(request: SearchRequest) -> List[Dict[str, Any]]:
+async def async_search_tags(request: SearchRequest) -> List[Dict[str, Any]]:
     """
-    Asynchronously search all groups.
+    Asynchronously search all tags.
 
     Parameters:
         request (SearchRequest): A request carrying the search query
 
     Returns:
-        List[Dict[str, Any]]: List of group responses
+        List[Dict[str, Any]]: List of tag responses
     """
-    request_info = _search_groups_request_info(request)
+    request_info = _search_tags_request_info(request)
     return await __async_post_request(**request_info)
 
 
 @async_data_request
-async def async_create_group(request: GroupRequest) -> Dict[str, Any]:
+async def async_create_tag(request: TagRequest) -> Dict[str, Any]:
     """
-    Asynchronously create group.
+    Asynchronously create tag.
 
     Args:
-        request (GroupRequest): Group request
+        request (TagRequest): tag request
 
     Returns:
-        Dict[str, Any]: Group response
+        Dict[str, Any]: tag response
     """
-    request_info = _create_group_request_info(request)
+    request_info = _create_tag_request_info(request)
     return await __async_put_request(**request_info)
 
 
 @async_data_request
-async def async_update_group(id: str, request: GroupRequest) -> Dict[str, Any]:
+async def async_update_tag(id: str, request: TagRequest) -> Dict[str, Any]:
     """
-    Asynchronously update group.
+    Asynchronously update tag.
 
     Args:
-        id (str): Group ID
-        request (GroupRequest): Group request
+        id (str): tag ID
+        request (TagRequest): tag request
 
     Returns:
-        Dict[str, Any]: Group response
+        Dict[str, Any]: tag response
     """
-    request_info = _update_group_request_info(id, request)
+    request_info = _update_tag_request_info(id, request)
     return await __async_post_request(**request_info)
 
 
 @async_data_request
-async def async_delete_group(id: str) -> None:
+async def async_delete_tag(id: str) -> None:
     """
-    Asynchronously delete group by ID.
+    Asynchronously delete tag by ID.
 
     Args:
-        id (str): Group ID
+        id (str): tag ID
 
     Returns:
         None
     """
-    request_info = _delete_group_request_info(id)
+    request_info = _delete_tag_request_info(id)
     return await __async_delete_request(**request_info)
 
 
 @async_data_request
-async def async_get_group_tags() -> List[str]:
+async def async_get_tag_tags() -> List[str]:
     """
-    Asynchronously get all the tags used by groups
+    Asynchronously get all the tags used by tags
 
     Returns:
-        List[str]: A list of all the tags used for groups
+        List[str]: A list of all the tags used for tags
     """
-    request_info = _get_group_tags_request_info()
+    request_info = _get_tag_tags_request_info()
     return await __async_get_request(**request_info)
 
 
 @async_data_request
-async def async_is_group_name_unique(group_name: str) -> bool:
+async def async_is_tag_name_unique(tag_name: str) -> bool:
     """
-    Asynchronously checks to see if the group name is unique
+    Asynchronously checks to see if the tag name is unique
 
     Args:
-        group_name (str): The new group name that is being tested
+        tag_name (str): The new tag name that is being tested
 
     Returns:
         Bool: A boolean representing if the name is unique
     """
-    request_info = _unique_group_name_request_info(group_name)
+    request_info = _unique_tag_name_request_info(tag_name)
     return await __async_post_request(**request_info)
```

### Comparing `spotlight-dev-0.0.1b0/spotlight/api/group/synchronous.py` & `spotlight-dev-0.0.1b1/spotlight/api/tag/synchronous.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,185 +1,185 @@
 from typing import Dict, Any, List
 
 from spotlight.api.model import SearchRequest, LookupRequest
-from spotlight.api.group.__util import (
-    _get_group_request_info,
-    _get_group_by_name_request_info,
-    _get_groups_request_info,
-    _get_groups_by_rule_id_request_info,
-    _search_groups_request_info,
-    _create_group_request_info,
-    _update_group_request_info,
-    _delete_group_request_info,
-    _get_group_tags_request_info,
-    _unique_group_name_request_info,
-    _get_groups_by_lookup_request_info,
+from spotlight.api.tag.__util import (
+    _get_tag_request_info,
+    _get_tag_by_name_request_info,
+    _get_tags_request_info,
+    _get_tags_by_rule_id_request_info,
+    _search_tags_request_info,
+    _create_tag_request_info,
+    _update_tag_request_info,
+    _delete_tag_request_info,
+    _get_tag_tags_request_info,
+    _unique_tag_name_request_info,
+    _get_tags_by_lookup_request_info,
 )
-from spotlight.api.group.model import GroupRequest
+from spotlight.api.tag.model import TagRequest
 from spotlight.core.common.decorators import data_request
 
 from spotlight.core.common.requests import (
     __get_request,
     __post_request,
     __put_request,
     __delete_request,
 )
 
 
 @data_request
-def get_group(id: str) -> Dict[str, Any]:
+def get_tag(id: str) -> Dict[str, Any]:
     """
-    Get group by ID.
+    Get tag by ID.
 
     Args:
-        id (str): Group ID
+        id (str): Tag ID
 
     Returns:
-        Dict[str, Any]: Group response
+        Dict[str, Any]: Tag response
     """
-    request_info = _get_group_request_info(id)
+    request_info = _get_tag_request_info(id)
     return __get_request(**request_info)
 
 
 @data_request
-def get_group_by_name(group_name: str) -> Dict[str, Any]:
+def get_tag_by_name(tag_name: str) -> Dict[str, Any]:
     """
-    Get group by name.
+    Get tag by name.
 
     Args:
-        group_name (str): Group name
+        tag_name (str): Tag name
 
     Returns:
-        Dict[str, Any]: Group response
+        Dict[str, Any]: Tag response
     """
-    request_info = _get_group_by_name_request_info(group_name)
+    request_info = _get_tag_by_name_request_info(tag_name)
     return __get_request(**request_info)
 
 
 @data_request
-def get_groups() -> List[Dict[str, Any]]:
+def get_tags() -> List[Dict[str, Any]]:
     """
-    Get all groups.
+    Get all tags.
 
     Returns:
-        List[Dict[str, Any]]: List of group responses
+        List[Dict[str, Any]]: List of tag responses
     """
-    request_info = _get_groups_request_info()
+    request_info = _get_tags_request_info()
     return __get_request(**request_info)
 
 
 @data_request
-def get_groups_by_lookup(request: LookupRequest) -> List[Dict[str, Any]]:
+def get_tags_by_lookup(request: LookupRequest) -> List[Dict[str, Any]]:
     """
-    Get all groups by lookup.
+    Get all tags by lookup.
 
     Args:
-        request (LookupRequest): The group information used in the group look up
+        request (LookupRequest): The tag information used in the tag look up
 
     Returns:
-        List[Dict[str, Any]]: List of group responses
+        List[Dict[str, Any]]: List of tag responses
     """
-    request_info = _get_groups_by_lookup_request_info(request)
+    request_info = _get_tags_by_lookup_request_info(request)
     return __post_request(**request_info)
 
 
 @data_request
-def get_groups_by_rule_id(rule_id: str) -> List[Dict[str, Any]]:
+def get_tags_by_rule_id(rule_id: str) -> List[Dict[str, Any]]:
     """
-    Get all groups by rule ID.
+    Get all tags by rule ID.
 
     Args:
         rule_id (str): Rule ID
 
     Returns:
-        List[Dict[str, Any]]: List of group responses
+        List[Dict[str, Any]]: List of tag responses
     """
-    request_info = _get_groups_by_rule_id_request_info(rule_id)
+    request_info = _get_tags_by_rule_id_request_info(rule_id)
     return __get_request(**request_info)
 
 
 @data_request
-def search_groups(request: SearchRequest) -> List[Dict[str, Any]]:
+def search_tags(request: SearchRequest) -> List[Dict[str, Any]]:
     """
-    Search all groups.
+    Search all tags.
 
     Parameters:
         request (SearchRequest): A request carrying the search query
 
     Returns:
-        List[Dict[str, Any]]: List of group responses
+        List[Dict[str, Any]]: List of tag responses
     """
-    request_info = _search_groups_request_info(request)
+    request_info = _search_tags_request_info(request)
     return __post_request(**request_info)
 
 
 @data_request
-def create_group(request: GroupRequest) -> Dict[str, Any]:
+def create_tag(request: TagRequest) -> Dict[str, Any]:
     """
-    Create group.
+    Create tag.
 
     Args:
-        request (GroupRequest): Group request
+        request (TagRequest): Tag request
 
     Returns:
-        Dict[str, Any]: Group response
+        Dict[str, Any]: Tag response
     """
-    request_info = _create_group_request_info(request)
+    request_info = _create_tag_request_info(request)
     return __put_request(**request_info)
 
 
 @data_request
-def update_group(id: str, request: GroupRequest) -> Dict[str, Any]:
+def update_tag(id: str, request: TagRequest) -> Dict[str, Any]:
     """
-    Update group.
+    Update tag.
 
     Args:
-        id (str): Group ID
-        request (GroupRequest): Group request
+        id (str): Tag ID
+        request (TagRequest): Tag request
 
     Returns:
-        Dict[str, Any]: Group response
+        Dict[str, Any]: Tag response
     """
-    request_info = _update_group_request_info(id, request)
+    request_info = _update_tag_request_info(id, request)
     return __post_request(**request_info)
 
 
 @data_request
-def delete_group(id: str) -> None:
+def delete_tag(id: str) -> None:
     """
-    Delete group by ID.
+    Delete tag by ID.
 
     Args:
-        id (str): Group ID
+        id (str): Tag ID
 
     Returns:
         None
     """
-    request_info = _delete_group_request_info(id)
+    request_info = _delete_tag_request_info(id)
     return __delete_request(**request_info)
 
 
 @data_request
-def get_group_tags() -> List[str]:
+def get_tag_tags() -> List[str]:
     """
-    Get all the tags used by groups
+    Get all the tags used by tags
 
     Returns:
-        List[str]: A list of all the tags used for groups
+        List[str]: A list of all the tags used for tags
     """
-    request_info = _get_group_tags_request_info()
+    request_info = _get_tag_tags_request_info()
     return __get_request(**request_info)
 
 
 @data_request
-def is_group_name_unique(group_name: str) -> bool:
+def is_tag_name_unique(tag_name: str) -> bool:
     """
-    Checks to see if the group name is unique
+    Checks to see if the tag name is unique
 
     Args:
-        group_name (str): The new group name that is being tested
+        tag_name (str): The new tag name that is being tested
 
     Returns:
         Bool: A boolean representing if the name is unique
     """
-    request_info = _unique_group_name_request_info(group_name)
+    request_info = _unique_tag_name_request_info(tag_name)
     return __post_request(**request_info)
```

### Comparing `spotlight-dev-0.0.1b0/spotlight/api/group/view/asynchronous.py` & `spotlight-dev-0.0.1b1/spotlight/api/tag/view/asynchronous.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 from typing import Dict, Any
 
-from spotlight.api.group.view.__util import (
-    _get_group_view_request_info,
-    _get_group_view_by_name_request_info,
+from spotlight.api.tag.view.__util import (
+    _get_tag_view_request_info,
+    _get_tag_view_by_name_request_info,
 )
 from spotlight.core.common.decorators import async_data_request
 
 from spotlight.core.common.requests import (
     __async_get_request,
 )
 
 
 @async_data_request
-async def async_get_group_view(id: str) -> Dict[str, Any]:
+async def async_get_tag_view(id: str) -> Dict[str, Any]:
     """
-    Asynchronously get group view by ID.
+    Asynchronously get tag view by ID.
 
     Args:
-        id (str): Group ID
+        id (str): Tag ID
 
     Returns:
-        Dict[str, Any]: Group view response
+        Dict[str, Any]: Tag view response
     """
-    request_info = _get_group_view_request_info(id)
+    request_info = _get_tag_view_request_info(id)
     return __async_get_request(**request_info)
 
 
 @async_data_request
-async def async_get_group_view_by_name(name: str) -> Dict[str, Any]:
+async def async_get_tag_view_by_name(name: str) -> Dict[str, Any]:
     """
-    Asynchronously get group view by name.
+    Asynchronously get tag view by name.
 
     Args:
-        name (str): Group name
+        name (str): Tag name
 
     Returns:
-        Dict[str, Any]: Group view response
+        Dict[str, Any]: Tag view response
     """
-    request_info = _get_group_view_by_name_request_info(name)
+    request_info = _get_tag_view_by_name_request_info(name)
     return await __async_get_request(**request_info)
```

### Comparing `spotlight-dev-0.0.1b0/spotlight/api/group/view/synchronous.py` & `spotlight-dev-0.0.1b1/spotlight/api/tag/view/synchronous.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 from typing import Dict, Any
 
-from spotlight.api.group.view.__util import (
-    _get_group_view_request_info,
-    _get_group_view_by_name_request_info,
+from spotlight.api.tag.view.__util import (
+    _get_tag_view_request_info,
+    _get_tag_view_by_name_request_info,
 )
 from spotlight.core.common.decorators import data_request
 
 from spotlight.core.common.requests import (
     __get_request,
 )
 
 
 @data_request
-def get_group_view(id: str) -> Dict[str, Any]:
+def get_tag_view(id: str) -> Dict[str, Any]:
     """
-    Get group view by ID.
+    Get tag view by ID.
 
     Args:
-        id (str): Group ID
+        id (str): Tag ID
 
     Returns:
-        Dict[str, Any]: Group view response
+        Dict[str, Any]: Tag view response
     """
-    request_info = _get_group_view_request_info(id)
+    request_info = _get_tag_view_request_info(id)
     return __get_request(**request_info)
 
 
 @data_request
-def get_group_view_by_name(name: str) -> Dict[str, Any]:
+def get_tag_view_by_name(name: str) -> Dict[str, Any]:
     """
-    Get group view by name.
+    Get tag view by name.
 
     Args:
-        name (str): Group name
+        name (str): Tag name
 
     Returns:
-        Dict[str, Any]: Group view response
+        Dict[str, Any]: Tag view response
     """
-    request_info = _get_group_view_by_name_request_info(name)
+    request_info = _get_tag_view_by_name_request_info(name)
     return __get_request(**request_info)
```

### Comparing `spotlight-dev-0.0.1b0/spotlight/api/job/__util.py` & `spotlight-dev-0.0.1b1/spotlight/api/job/__util.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from spotlight.api.model import SearchRequest
 from spotlight.api.job.model import JobRequest
 
 
 def _get_job_request_info(id: str) -> dict:
-    return {"endpoint": f"config/datawatch/job/{id}"}
+    return {"endpoint": f"config/spotlight/job/{id}"}
 
 
 def _get_jobs_request_info() -> dict:
-    return {"endpoint": f"config/datawatch/job"}
+    return {"endpoint": f"config/spotlight/job"}
 
 
 def _search_jobs_request_info(request: SearchRequest) -> dict:
-    return {"endpoint": f"config/datawatch/job", "json": request.request_dict()}
+    return {"endpoint": f"config/spotlight/job", "json": request.request_dict()}
 
 
 def _create_job_request_info(request: JobRequest) -> dict:
-    return {"endpoint": f"config/datawatch/job", "json": request.request_dict()}
+    return {"endpoint": f"config/spotlight/job", "json": request.request_dict()}
 
 
 def _update_job_request_info(id: str, request: JobRequest) -> dict:
-    return {"endpoint": f"config/datawatch/job/{id}", "json": request.request_dict()}
+    return {"endpoint": f"config/spotlight/job/{id}", "json": request.request_dict()}
 
 
 def _delete_job_request_info(id: str) -> dict:
-    return {"endpoint": f"config/datawatch/job/{id}"}
+    return {"endpoint": f"config/spotlight/job/{id}"}
 
 
 def _get_job_tags_request_info() -> dict:
-    return {"endpoint": f"config/datawatch/job/tags"}
+    return {"endpoint": f"config/spotlight/job/tags"}
```

### Comparing `spotlight-dev-0.0.1b0/spotlight/api/job/asynchronous.py` & `spotlight-dev-0.0.1b1/spotlight/api/job/asynchronous.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 
 
 @async_data_request
 async def async_update_job(id: str, request: JobRequest) -> Dict[str, Any]:
     """
     Asynchronously update job.
 
-    NOTE: Groups associated to the job are not updated
+    NOTE: Tags associated to the job are not updated
 
     Args:
         id (str): Job ID
         request (JobRequest): Job request
 
     Returns:
         Dict[str, Any]: Job response
```

### Comparing `spotlight-dev-0.0.1b0/spotlight/api/job/model.py` & `spotlight-dev-0.0.1b1/spotlight/api/job/model.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,33 +5,31 @@
 from spotlight.core.common.base import Base
 from spotlight.core.common.enum import Status
 
 
 class JobRequest(Base):
     name: str
     status: Status
-    group_ids: Optional[List[str]] = Field(default=None)
+    tag_ids: Optional[List[str]] = Field(default=None)
     start_time: Optional[int] = Field(default=None)
     end_time: Optional[int] = Field(default=None)
     metadata: Optional[dict] = Field(default=None)
-    tags: Optional[List[str]] = Field(default=None)
 
 
 class JobResponse(Base):
     id: str
     name: str
     status: Status
     start_time: Optional[int]
     end_time: Optional[int]
     metadata: dict
-    tags: List[str]
     created_by: str
     created_at: int
     updated_by: Optional[str]
     updated_at: Optional[int]
 
 
-class JobGroupResponse(Base):
-    group_id: str
+class JobTagResponse(Base):
+    tag_id: str
     rule_id: str
     created_by: str
     created_at: int
```

### Comparing `spotlight-dev-0.0.1b0/spotlight/api/job/synchronous.py` & `spotlight-dev-0.0.1b1/spotlight/api/job/synchronous.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 
 
 @data_request
 def update_job(id: str, request: JobRequest) -> Dict[str, Any]:
     """
     Update job.
 
-    NOTE: Groups associated to the job are not updated
+    NOTE: Tags associated to the job are not updated
 
     Args:
         id (str): Job ID
         request (JobRequest): Job request
 
     Returns:
         Dict[str, Any]: Job response
```

### Comparing `spotlight-dev-0.0.1b0/spotlight/api/job/view/asynchronous.py` & `spotlight-dev-0.0.1b1/spotlight/api/job/view/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b0/spotlight/api/rule/__util.py` & `spotlight-dev-0.0.1b1/spotlight/api/rule/__util.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,40 +2,40 @@
 from typing import List
 
 from spotlight.api.model import SearchRequest, LookupRequest
 from spotlight.api.rule.model import RuleRequest
 
 
 def _get_rule_request_info(id: str) -> dict:
-    return {"endpoint": f"config/datawatch/rule/{id}"}
+    return {"endpoint": f"config/spotlight/rule/{id}"}
 
 
 def _get_rules_request_info() -> dict:
-    return {"endpoint": f"config/datawatch/rule"}
+    return {"endpoint": f"config/spotlight/rule"}
 
 
-def _get_all_rules_by_groups_request_info(request: LookupRequest) -> dict:
-    return {"endpoint": f"config/datawatch/rule", "json": request.request_dict()}
+def _get_all_rules_by_tags_request_info(request: LookupRequest) -> dict:
+    return {"endpoint": f"config/spotlight/rule", "json": request.request_dict()}
 
 
 def _search_rules_request_info(request: SearchRequest) -> dict:
-    return {"endpoint": f"config/datawatch/rule", "json": request.request_dict()}
+    return {"endpoint": f"config/spotlight/rule", "json": request.request_dict()}
 
 
 def _create_rule_request_info(request: RuleRequest) -> dict:
-    return {"endpoint": f"config/datawatch/rule", "json": request.request_dict()}
+    return {"endpoint": f"config/spotlight/rule", "json": request.request_dict()}
 
 
 def _update_rule_request_info(id: str, request: RuleRequest) -> dict:
-    return {"endpoint": f"config/datawatch/rule/{id}", "json": request.request_dict()}
+    return {"endpoint": f"config/spotlight/rule/{id}", "json": request.request_dict()}
 
 
-def _declarative_update_rule_groups_request_info(id: str, group_ids: List[str]) -> dict:
-    return {"endpoint": f"config/datawatch/rule/{id}/group", "json": group_ids}
+def _declarative_update_rule_tags_request_info(id: str, tag_ids: List[str]) -> dict:
+    return {"endpoint": f"config/spotlight/rule/{id}/tag", "json": tag_ids}
 
 
 def _delete_rule_request_info(id: str) -> dict:
-    return {"endpoint": f"config/datawatch/rule/{id}"}
+    return {"endpoint": f"config/spotlight/rule/{id}"}
 
 
 def _get_rule_tags_request_info() -> dict:
-    return {"endpoint": f"config/datawatch/rule/tags"}
+    return {"endpoint": f"config/spotlight/rule/tags"}
```

### Comparing `spotlight-dev-0.0.1b0/spotlight/api/rule/asynchronous.py` & `spotlight-dev-0.0.1b1/spotlight/api/rule/asynchronous.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,16 +5,16 @@
     _get_rule_request_info,
     _get_rules_request_info,
     _create_rule_request_info,
     _update_rule_request_info,
     _delete_rule_request_info,
     _search_rules_request_info,
     _get_rule_tags_request_info,
-    _declarative_update_rule_groups_request_info,
-    _get_all_rules_by_groups_request_info,
+    _declarative_update_rule_tags_request_info,
+    _get_all_rules_by_tags_request_info,
 )
 from spotlight.api.rule.model import RuleRequest
 from spotlight.core.common.decorators import async_data_request
 
 from spotlight.core.common.requests import (
     __async_get_request,
     __async_post_request,
@@ -47,25 +47,25 @@
         List[Dict[str, Any]]: List of rule responses
     """
     request_info = _get_rules_request_info()
     return await __async_get_request(**request_info)
 
 
 @async_data_request
-async def async_get_rules_by_groups(request: LookupRequest) -> List[Dict[str, Any]]:
+async def async_get_rules_by_tags(request: LookupRequest) -> List[Dict[str, Any]]:
     """
-    Asynchronously get all rules by groups.
+    Asynchronously get all rules by tags.
 
     Args:
-        request (LookupRequest): The group information used in the rule look up
+        request (LookupRequest): The tag information used in the rule look up
 
     Returns:
         List[Dict[str, Any]]: List of rule responses
     """
-    request_info = _get_all_rules_by_groups_request_info(request)
+    request_info = _get_all_rules_by_tags_request_info(request)
     return await __async_post_request(**request_info)
 
 
 @async_data_request
 async def async_search_rules(request: SearchRequest) -> List[Dict[str, Any]]:
     """
     Asynchronously search all rules.
@@ -108,28 +108,28 @@
         Dict[str, Any]: Rule response
     """
     request_info = _update_rule_request_info(id, request)
     return await __async_post_request(**request_info)
 
 
 @async_data_request
-async def async_declarative_update_rule_groups(
-    id: str, group_ids: List[str]
+async def async_declarative_update_rule_tags(
+    id: str, tag_ids: List[str]
 ) -> Dict[str, Any]:
     """
-    Asynchronously sets the state of the rule's groups to the ones passed in.
+    Asynchronously sets the state of the rule's tags to the ones passed in.
 
     Args:
         id (str): Rule ID
-        group_ids (List[str]): List of group ids to put the rule in
+        tag_ids (List[str]): List of tag ids to put the rule in
 
     Returns:
-        Dict[str, Any]: Rule group response
+        Dict[str, Any]: Rule tag response
     """
-    request_info = _declarative_update_rule_groups_request_info(id, group_ids)
+    request_info = _declarative_update_rule_tags_request_info(id, tag_ids)
     return await __async_post_request(**request_info)
 
 
 @async_data_request
 async def async_delete_rule(id: str) -> None:
     """
     Asynchronously delete rule by ID.
```

### Comparing `spotlight-dev-0.0.1b0/spotlight/api/rule/model.py` & `spotlight-dev-0.0.1b1/spotlight/api/rule/model.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,29 +8,27 @@
 
 class RuleRequest(Base):
     name: str
     predicate: str
     description: Optional[str] = Field(default=None)
     threshold: Optional[int] = Field(default=None)
     severity: Optional[Severity] = Field(default=Severity.ERROR)
-    tags: Optional[List[str]] = Field(default=None)
 
 
 class RuleResponse(Base):
     id: str
     name: str
     description: Optional[str]
     predicate: str
     threshold: int
     severity: Severity
-    tags: Optional[List[str]]
     created_by: str
     created_at: int
     updated_by: Optional[str]
     updated_at: Optional[int]
 
 
-class RuleGroupResponse(Base):
-    group_id: str
+class RuleTagResponse(Base):
+    tag_id: str
     rule_id: str
     created_by: str
     created_at: int
```

### Comparing `spotlight-dev-0.0.1b0/spotlight/api/rule/synchronous.py` & `spotlight-dev-0.0.1b1/spotlight/api/rule/synchronous.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,16 +5,16 @@
     _get_rule_request_info,
     _get_rules_request_info,
     _create_rule_request_info,
     _update_rule_request_info,
     _delete_rule_request_info,
     _search_rules_request_info,
     _get_rule_tags_request_info,
-    _declarative_update_rule_groups_request_info,
-    _get_all_rules_by_groups_request_info,
+    _declarative_update_rule_tags_request_info,
+    _get_all_rules_by_tags_request_info,
 )
 from spotlight.api.rule.model import RuleRequest
 from spotlight.core.common.decorators import data_request
 from spotlight.core.common.requests import (
     __get_request,
     __post_request,
     __put_request,
@@ -46,25 +46,25 @@
         List[Dict[str, Any]]: List of rule responses
     """
     request_info = _get_rules_request_info()
     return __get_request(**request_info)
 
 
 @data_request
-def get_rules_by_groups(request: LookupRequest) -> List[Dict[str, Any]]:
+def get_rules_by_tags(request: LookupRequest) -> List[Dict[str, Any]]:
     """
-    Get all rules by groups.
+    Get all rules by tags.
 
     Args:
-        request (LookupRequest): The group information used in the rule look up
+        request (LookupRequest): The tag information used in the rule look up
 
     Returns:
         List[Dict[str, Any]]: List of rule responses
     """
-    request_info = _get_all_rules_by_groups_request_info(request)
+    request_info = _get_all_rules_by_tags_request_info(request)
     return __post_request(**request_info)
 
 
 @data_request
 def search_rules(request: SearchRequest) -> List[Dict[str, Any]]:
     """
     Search all rules.
@@ -107,26 +107,26 @@
         Dict[str, Any]: Rule response
     """
     request_info = _update_rule_request_info(id, request)
     return __post_request(**request_info)
 
 
 @data_request
-def declarative_update_rule_groups(id: str, group_ids: List[str]) -> Dict[str, Any]:
+def declarative_update_rule_tags(id: str, tag_ids: List[str]) -> Dict[str, Any]:
     """
-    Sets the state of the rule's groups to the ones passed in.
+    Sets the state of the rule's tags to the ones passed in.
 
     Args:
         id (str): Rule ID
-        group_ids (List[str]): List of group ids to put the rule in
+        tag_ids (List[str]): List of tag ids to put the rule in
 
     Returns:
-        Dict[str, Any]: Rule group response
+        Dict[str, Any]: Rule tag response
     """
-    request_info = _declarative_update_rule_groups_request_info(id, group_ids)
+    request_info = _declarative_update_rule_tags_request_info(id, tag_ids)
     return __post_request(**request_info)
 
 
 @data_request
 def delete_rule(id: str) -> None:
     """
     Delete rule by ID.
```

### Comparing `spotlight-dev-0.0.1b0/spotlight/core/common/base.py` & `spotlight-dev-0.0.1b1/spotlight/core/common/base.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b0/spotlight/core/common/config.py` & `spotlight-dev-0.0.1b1/spotlight/core/common/config.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b0/spotlight/core/common/date/function.py` & `spotlight-dev-0.0.1b1/spotlight/core/common/date/function.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b0/spotlight/core/common/decorators/authorization/__util.py` & `spotlight-dev-0.0.1b1/spotlight/core/common/decorators/authorization/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b0/spotlight/core/common/decorators/authorization/asynchronous.py` & `spotlight-dev-0.0.1b1/spotlight/core/common/decorators/authorization/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b0/spotlight/core/common/decorators/authorization/synchronous.py` & `spotlight-dev-0.0.1b1/spotlight/core/common/decorators/authorization/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b0/spotlight/core/common/decorators/data/__util.py` & `spotlight-dev-0.0.1b1/spotlight/core/common/decorators/data/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b0/spotlight/core/common/decorators/data/asynchronous.py` & `spotlight-dev-0.0.1b1/spotlight/core/common/decorators/data/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b0/spotlight/core/common/decorators/data/synchronous.py` & `spotlight-dev-0.0.1b1/spotlight/core/common/decorators/data/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b0/spotlight/core/common/decorators/timeit.py` & `spotlight-dev-0.0.1b1/spotlight/core/common/decorators/timeit.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b0/spotlight/core/common/errors.py` & `spotlight-dev-0.0.1b1/spotlight/core/common/errors.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b0/spotlight/core/common/function.py` & `spotlight-dev-0.0.1b1/spotlight/core/common/function.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b0/spotlight/core/common/metaclass/singleton.py` & `spotlight-dev-0.0.1b1/spotlight/core/common/metaclass/singleton.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b0/spotlight/core/common/requests/asynchronous.py` & `spotlight-dev-0.0.1b1/spotlight/core/common/requests/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b0/spotlight/core/common/requests/synchronous.py` & `spotlight-dev-0.0.1b1/spotlight/core/common/requests/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b0/spotlight/core/pipeline/__init__.py` & `spotlight-dev-0.0.1b1/spotlight/core/pipeline/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,108 +37,101 @@
     return result
 
 
 def data_quality_pipeline(
     data: Any,
     job_name: str,
     *,
-    group_names: Optional[List[str]] = None,
-    group_ids: Optional[List[str]] = None,
+    tag_names: Optional[List[str]] = None,
+    tag_ids: Optional[List[str]] = None,
     additional_rules: Optional[List[AbstractRule]] = None,
     metadata: Optional[dict] = None,
-    tags: Optional[List[str]] = None,
     multi_processing: bool = False,
     processes: int = 5,
 ) -> JobResponse:
     """
     Runs data through a data quality pipeline.
 
-    NOTE: You must provide the group names and/or the group ids for this method to run.
+    NOTE: You must provide the tag names and/or the tag ids for this method to run.
     NOTE: The number of rules run in parallel is dependent on the number of processes.
 
     Args:
         data (Any): Data that is run through the pipeline
         job_name (str): Name assigned to the job created from running this pipeline
-        group_names (Optional[List[str]]): List of group names to use with the pipeline
-        group_ids (Optional[List[str]]): List of group ids to use with the pipeline
+        tag_names (Optional[List[str]]): List of tag names to use with the pipeline
+        tag_ids (Optional[List[str]]): List of tag ids to use with the pipeline
         additional_rules (List[AbstractRule]): additional rules to run on the pipeline (specifically rules that aren't
         supported in the API i.e. AbstractCustomCodeRules)
         metadata (Optional[dict]): Metadata added to the job information
-        tags (Optional[List[str]]): Tags added to the job
         multi_processing (bool): Optional flag to run the rules over the data concurrently
         processes (int): Optional number of process to spin up when running the rules concurrently
 
     Returns:
         JobResponse: The job response with all the information from the run
     """
     job, rules = start_job(
         job_name=job_name,
-        group_names=group_names,
-        group_ids=group_ids,
+        tag_names=tag_names,
+        tag_ids=tag_ids,
         metadata=metadata,
-        tags=tags,
     )
     rules.extend(additional_rules or [])
     result = __dq_pipeline(data, job.name, rules, multi_processing, processes)
 
     job = stop_job(
         job=job,
         pipeline_result=result,
-        tags=tags,
     )
     return job
 
 
 async def async_data_quality_pipeline(
     data: Any,
     job_name: str,
     *,
-    group_names: Optional[List[str]] = None,
-    group_ids: Optional[List[str]] = None,
+    tag_names: Optional[List[str]] = None,
+    tag_ids: Optional[List[str]] = None,
     additional_rules: Optional[List[AbstractRule]] = None,
     metadata: Optional[dict] = None,
-    tags: Optional[List[str]] = None,
     multi_processing: bool = False,
     processes: int = 5,
 ) -> JobResponse:
     """
     Asynchronously runs data through a data quality pipeline.
 
-    NOTE: You must provide the group names and/or the group ids for this method to run.
+    NOTE: You must provide the tag names and/or the tag ids for this method to run.
     NOTE: The number of rules run in parallel is dependent on the number of processes.
 
     Args:
         data (Any): Data that is run through the pipeline
         job_name (str): Name assigned to the job created from running this pipeline
-        group_names (Optional[List[str]]): List of group names to use with the pipeline
-        group_ids (Optional[List[str]]): List of group ids to use with the pipeline
+        tag_names (Optional[List[str]]): List of tag names to use with the pipeline
+        tag_ids (Optional[List[str]]): List of tag ids to use with the pipeline
         additional_rules (List[AbstractRule]): additional rules to run on the pipeline (specifically rules that aren't
         supported in the API i.e. AbstractCustomCodeRules)
         metadata (Optional[dict]): Metadata added to the job information
         tags (Optional[List[str]]): Tags added to the job
         multi_processing (bool): Optional flag to run the rules over the data concurrently
         processes (int): Optional number of process to spin up when running the rules concurrently
 
     Returns:
         JobResponse: The job response with all the information from the run
     """
     job, rules = await async_start_job(
         job_name=job_name,
-        group_names=group_names,
-        group_ids=group_ids,
+        tag_names=tag_names,
+        tag_ids=tag_ids,
         metadata=metadata,
-        tags=tags,
     )
     rules.extend(additional_rules or [])
     result = __dq_pipeline(data, job.name, rules, multi_processing, processes)
 
     job = await async_stop_job(
         job=job,
         pipeline_result=result,
-        tags=tags,
     )
     return job
 
 
 def offline_data_quality_pipeline(
     job_name: str,
     data: Any,
```

### Comparing `spotlight-dev-0.0.1b0/spotlight/core/pipeline/execution/plugin/abstract.py` & `spotlight-dev-0.0.1b1/spotlight/core/pipeline/execution/plugin/abstract.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b0/spotlight/core/pipeline/execution/plugin/decorator.py` & `spotlight-dev-0.0.1b1/spotlight/core/pipeline/execution/plugin/decorator.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b0/spotlight/core/pipeline/execution/plugin/registry.py` & `spotlight-dev-0.0.1b1/spotlight/core/pipeline/execution/plugin/registry.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Set, Optional, Any
+from typing import Set, Any
 
 from spotlight.core.common.metaclass.singleton import Singleton
 from spotlight.core.pipeline.execution.plugin.abstract import AbstractPlugin
 
 
 class PluginRegistry(metaclass=Singleton):
     """
```

### Comparing `spotlight-dev-0.0.1b0/spotlight/core/pipeline/execution/rule/abstract.py` & `spotlight-dev-0.0.1b1/spotlight/core/pipeline/execution/rule/abstract.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b0/spotlight/core/pipeline/execution/rule/sql_rule.py` & `spotlight-dev-0.0.1b1/spotlight/core/pipeline/execution/rule/sql_rule.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b0/spotlight/core/pipeline/execution/synchronous.py` & `spotlight-dev-0.0.1b1/spotlight/core/pipeline/execution/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b0/spotlight/core/pipeline/model/pipeline.py` & `spotlight-dev-0.0.1b1/spotlight/core/pipeline/model/pipeline.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b0/spotlight/core/pipeline/utils/asynchronously.py` & `spotlight-dev-0.0.1b1/spotlight/core/pipeline/utils/asynchronously.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,111 +1,104 @@
 import copy
 from typing import Optional, List, Tuple
 
-from spotlight.api.group.asynchronous import async_get_groups_by_lookup
-from spotlight.api.group.model import GroupResponse
+from spotlight.api.tag.asynchronous import async_get_tags_by_lookup
+from spotlight.api.tag.model import TagResponse
 from spotlight.api.job import (
     async_create_job,
     async_update_job,
 )
 from spotlight.api.job.model import JobRequest, JobResponse
-from spotlight.api.rule.asynchronous import async_get_rules_by_groups
+from spotlight.api.rule.asynchronous import async_get_rules_by_tags
 from spotlight.api.rule.model import RuleResponse
 from spotlight.api.model import LookupRequest
 from spotlight.core.common.enum import Status
 from spotlight.core.pipeline.execution.rule import SQLRule
 from spotlight.core.pipeline.model.pipeline import PipelineResult
 
 
-async def __async_get_rule_and_group_info(
-    group_names: Optional[List[str]] = None, group_ids: Optional[List[str]] = None
-) -> Tuple[List[GroupResponse], List[RuleResponse]]:
+async def __async_get_rule_and_tag_info(
+    tag_names: Optional[List[str]] = None, tag_ids: Optional[List[str]] = None
+) -> Tuple[List[TagResponse], List[RuleResponse]]:
     """
-    Asynchronous helper method for getting the group of rules from the group_id or group_name.
+    Asynchronous helper method for getting the tag of rules from the tag_id or tag_name.
 
     Args:
-        group_names (Optional[List[str]]): The name of rule groups
-        group_ids (Optional[List[str]]): The id of the rule groups
+        tag_names (Optional[List[str]]): The name of rule tags
+        tag_ids (Optional[List[str]]): The id of the rule tags
 
     Returns:
-        Tuple[List[GroupResponse], List[RuleResponse]]: A list of all the groups, and rules associated with the group
+        Tuple[List[TagResponse], List[RuleResponse]]: A list of all the tags, and rules associated with the tag
         info passed in
     """
     request = LookupRequest(
-        group_names=group_names if group_names else [],
-        group_ids=group_ids if group_ids else [],
+        tag_names=tag_names if tag_names else [],
+        tag_ids=tag_ids if tag_ids else [],
     )
-    response = await async_get_rules_by_groups(request)
+    response = await async_get_rules_by_tags(request)
     rules = [RuleResponse(**rule) for rule in response]
-    group_response = await async_get_groups_by_lookup(request)
-    groups = [GroupResponse(**group) for group in group_response]
-    return groups, rules
+    tag_response = await async_get_tags_by_lookup(request)
+    tags = [TagResponse(**tag) for tag in tag_response]
+    return tags, rules
 
 
 async def async_start_job(
     job_name: str,
     *,
-    group_names: Optional[List[str]] = None,
-    group_ids: Optional[List[str]] = None,
+    tag_names: Optional[List[str]] = None,
+    tag_ids: Optional[List[str]] = None,
     metadata: Optional[dict] = None,
-    tags: Optional[List[str]] = None,
 ) -> Tuple[JobResponse, List[SQLRule]]:
     """
     Asynchronously creates the job with the starting information.
 
-    NOTE: You must provide the group_name or group_id but not both.
+    NOTE: You must provide the tag_name or tag_id but not both.
 
     Args:
         job_name (str): Name assigned to the job created from running this pipeline
-        group_names (Optional[List[str]]): The name of rule groups
-        group_ids (Optional[List[str]]): The id of the rule groups
+        tag_names (Optional[List[str]]): The name of rule tags
+        tag_ids (Optional[List[str]]): The id of the rule tags
         metadata (Optional[dict]): Metadata added to the job information
-        tags (Optional[List[str]]): Tags added to the job
 
     Returns:
         Tuple[JobResponse, List[Rule]]: The created job and the rules used in the job
     """
-    groups, rules = await __async_get_rule_and_group_info(
-        group_names=group_names, group_ids=group_ids
+    tags, rules = await __async_get_rule_and_tag_info(
+        tag_names=tag_names, tag_ids=tag_ids
     )
     request = JobRequest(
         name=job_name,
         status=Status.IN_PROGRESS,
-        group_ids=[group.id for group in groups],
+        tag_ids=[tag.id for tag in tags],
         metadata=metadata,
-        tags=tags,
     )
     response = await async_create_job(request)
     job = JobResponse(**response)
     return job, [SQLRule.from_rule_response(rule) for rule in rules]
 
 
 async def async_stop_job(
     job: JobResponse,
     pipeline_result: PipelineResult,
-    *,
-    tags: Optional[List[str]] = None,
 ) -> JobResponse:
     """
     Asynchronously stops the job and updates it with all the results.
 
     Args:
         job (JobResponse): The job being updated
         pipeline_result (PipelineResult): The result of the piepline
-        tags (Optional[List[str]]): Tags added to the job
 
     Returns:
         JobResponse: The updated job
     """
     combined_metadata = copy.deepcopy(job.metadata)
     combined_metadata.update(pipeline_result.metadata.request_dict())
     request = JobRequest(
         name=job.name,
         status=pipeline_result.status,
         start_time=pipeline_result.start_time,
         end_time=pipeline_result.end_time,
         metadata=combined_metadata,
-        tags=tags or job.tags,
     )
     response = await async_update_job(job.id, request)
     job = JobResponse(**response)
     return job
```

### Comparing `spotlight-dev-0.0.1b0/spotlight/pandas/__util.py` & `spotlight-dev-0.0.1b1/spotlight/pandas/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b0/spotlight/pandas/plugin.py` & `spotlight-dev-0.0.1b1/spotlight/pandas/plugin.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b0/spotlight/pandas/runners.py` & `spotlight-dev-0.0.1b1/spotlight/pandas/runners.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b0/spotlight_dev.egg-info/SOURCES.txt` & `spotlight-dev-0.0.1b1/spotlight_dev.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,24 +3,14 @@
 spotlight/__init__.py
 spotlight/api/__init__.py
 spotlight/api/model.py
 spotlight/api/auth/__init__.py
 spotlight/api/auth/__util.py
 spotlight/api/auth/asynchronous.py
 spotlight/api/auth/synchronous.py
-spotlight/api/group/__init__.py
-spotlight/api/group/__util.py
-spotlight/api/group/asynchronous.py
-spotlight/api/group/model.py
-spotlight/api/group/synchronous.py
-spotlight/api/group/view/__init__.py
-spotlight/api/group/view/__util.py
-spotlight/api/group/view/asynchronous.py
-spotlight/api/group/view/model.py
-spotlight/api/group/view/synchronous.py
 spotlight/api/job/__init__.py
 spotlight/api/job/__util.py
 spotlight/api/job/asynchronous.py
 spotlight/api/job/model.py
 spotlight/api/job/synchronous.py
 spotlight/api/job/view/__init__.py
 spotlight/api/job/view/__util.py
@@ -28,14 +18,24 @@
 spotlight/api/job/view/model.py
 spotlight/api/job/view/synchronous.py
 spotlight/api/rule/__init__.py
 spotlight/api/rule/__util.py
 spotlight/api/rule/asynchronous.py
 spotlight/api/rule/model.py
 spotlight/api/rule/synchronous.py
+spotlight/api/tag/__init__.py
+spotlight/api/tag/__util.py
+spotlight/api/tag/asynchronous.py
+spotlight/api/tag/model.py
+spotlight/api/tag/synchronous.py
+spotlight/api/tag/view/__init__.py
+spotlight/api/tag/view/__util.py
+spotlight/api/tag/view/asynchronous.py
+spotlight/api/tag/view/model.py
+spotlight/api/tag/view/synchronous.py
 spotlight/core/__init__.py
 spotlight/core/common/__init__.py
 spotlight/core/common/base.py
 spotlight/core/common/base_enum.py
 spotlight/core/common/config.py
 spotlight/core/common/enum.py
 spotlight/core/common/errors.py
```

