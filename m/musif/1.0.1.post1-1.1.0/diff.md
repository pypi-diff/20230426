# Comparing `tmp/musif-1.0.1.post1.tar.gz` & `tmp/musif-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "musif-1.0.1.post1.tar", last modified: Wed Feb 22 15:57:40 2023, max compression
+gzip compressed data, was "musif-1.1.0.tar", last modified: Wed Apr 26 15:09:24 2023, max compression
```

## Comparing `musif-1.0.1.post1.tar` & `musif-1.1.0.tar`

### file list

```diff
@@ -1,89 +1,94 @@
--rw-r--r--   0        0        0      363 2023-02-07 16:57:58.015884 musif-1.0.1.post1/README.md
--rw-r--r--   0        0        0      258 2023-01-30 15:04:50.288684 musif-1.0.1.post1/musif/__init__.py
--rw-r--r--   0        0        0      232 2023-01-30 15:04:50.288684 musif-1.0.1.post1/musif/cache/__init__.py
--rw-r--r--   0        0        0    16913 2023-01-31 10:36:20.878445 musif-1.0.1.post1/musif/cache/cache.py
--rw-r--r--   0        0        0    16913 2023-01-30 15:04:50.288684 musif-1.0.1.post1/musif/cache/cache.py~
--rw-r--r--   0        0        0     7304 2023-01-31 10:36:20.878445 musif-1.0.1.post1/musif/cache/utils.py
--rw-r--r--   0        0        0     7304 2023-01-30 15:04:50.288684 musif-1.0.1.post1/musif/cache/utils.py~
--rw-r--r--   0        0        0        1 2023-01-30 15:04:50.288684 musif-1.0.1.post1/musif/common/__init__.py
--rw-r--r--   0        0        0      202 2023-01-30 15:04:50.288684 musif-1.0.1.post1/musif/common/_constants.py
--rw-r--r--   0        0        0     2402 2023-01-30 15:04:50.288684 musif-1.0.1.post1/musif/common/_logs.py
--rw-r--r--   0        0        0     3067 2023-01-30 15:04:50.288684 musif-1.0.1.post1/musif/common/_utils.py
--rw-r--r--   0        0        0      826 2023-01-30 15:04:50.288684 musif-1.0.1.post1/musif/common/constants.py
--rw-r--r--   0        0        0     1700 2023-01-30 15:04:50.288684 musif-1.0.1.post1/musif/common/didone_utils.py
--rw-r--r--   0        0        0     1175 2023-01-30 15:04:50.288684 musif-1.0.1.post1/musif/common/exceptions.py
--rw-r--r--   0        0        0     4102 2023-01-30 15:04:50.288684 musif-1.0.1.post1/musif/common/sort.py
--rw-r--r--   0        0        0     2103 2023-01-30 15:04:50.288684 musif-1.0.1.post1/musif/common/translate.py
--rw-r--r--   0        0        0     6873 2023-01-31 10:36:20.885111 musif-1.0.1.post1/musif/config.py
--rw-r--r--   0        0        0     6873 2023-01-30 16:27:17.179605 musif-1.0.1.post1/musif/config.py~
--rw-r--r--   0        0        0       52 2023-01-30 15:04:50.288684 musif-1.0.1.post1/musif/extract/__init__.py
--rw-r--r--   0        0        0        0 2023-01-30 16:27:17.179605 musif-1.0.1.post1/musif/extract/basic_modules/file_name_generic/__init__.py
--rw-r--r--   0        0        0       34 2023-01-30 16:27:17.179605 musif-1.0.1.post1/musif/extract/basic_modules/file_name_generic/constants.py
--rw-r--r--   0        0        0      999 2023-01-30 16:27:17.179605 musif-1.0.1.post1/musif/extract/basic_modules/file_name_generic/handler.py
--rw-r--r--   0        0        0        0 2023-01-30 15:04:50.288684 musif-1.0.1.post1/musif/extract/basic_modules/scoring/__init__.py
--rw-r--r--   0        0        0      646 2023-01-30 15:04:50.288684 musif-1.0.1.post1/musif/extract/basic_modules/scoring/constants.py
--rw-r--r--   0        0        0     5686 2023-01-30 15:04:50.288684 musif-1.0.1.post1/musif/extract/basic_modules/scoring/handler.py
--rw-r--r--   0        0        0     1600 2023-01-30 15:04:50.288684 musif-1.0.1.post1/musif/extract/common.py
--rw-r--r--   0        0        0     1178 2023-01-30 15:04:50.288684 musif-1.0.1.post1/musif/extract/constants.py
--rw-r--r--   0        0        0    27251 2023-01-30 16:27:17.179605 musif-1.0.1.post1/musif/extract/extract.py
--rw-r--r--   0        0        0        0 2023-01-30 15:04:50.288684 musif-1.0.1.post1/musif/extract/features/__init__.py
--rw-r--r--   0        0        0       25 2023-01-30 15:04:50.288684 musif-1.0.1.post1/musif/extract/features/ambitus/__init__.py
--rw-r--r--   0        0        0      270 2023-01-30 15:04:50.288684 musif-1.0.1.post1/musif/extract/features/ambitus/constants.py
--rw-r--r--   0        0        0     2705 2023-01-30 15:04:50.288684 musif-1.0.1.post1/musif/extract/features/ambitus/handler.py
--rw-r--r--   0        0        0        0 2023-01-30 15:04:50.288684 musif-1.0.1.post1/musif/extract/features/core/__init__.py
--rw-r--r--   0        0        0      465 2023-01-30 16:27:17.179605 musif-1.0.1.post1/musif/extract/features/core/constants.py
--rw-r--r--   0        0        0     6760 2023-02-01 16:15:04.027948 musif-1.0.1.post1/musif/extract/features/core/handler.py
--rw-r--r--   0        0        0       55 2023-01-30 15:04:50.288684 musif-1.0.1.post1/musif/extract/features/density/__init__.py
--rw-r--r--   0        0        0       57 2023-01-30 15:04:50.288684 musif-1.0.1.post1/musif/extract/features/density/constants.py
--rw-r--r--   0        0        0     7656 2023-01-30 16:27:17.179605 musif-1.0.1.post1/musif/extract/features/density/handler.py
--rw-r--r--   0        0        0       25 2023-01-30 15:04:50.288684 musif-1.0.1.post1/musif/extract/features/dynamics/__init__.py
--rw-r--r--   0        0        0      711 2023-01-30 15:04:50.288684 musif-1.0.1.post1/musif/extract/features/dynamics/constants.py
--rw-r--r--   0        0        0     9029 2023-01-30 15:04:50.288684 musif-1.0.1.post1/musif/extract/features/dynamics/handler.py
--rw-r--r--   0        0        0        0 2023-01-30 15:04:50.288684 musif-1.0.1.post1/musif/extract/features/harmony/__init__.py
--rw-r--r--   0        0        0      815 2023-01-30 15:04:50.288684 musif-1.0.1.post1/musif/extract/features/harmony/constants.py
--rw-r--r--   0        0        0     2741 2023-01-30 15:04:50.288684 musif-1.0.1.post1/musif/extract/features/harmony/handler.py
--rw-r--r--   0        0        0    26047 2023-01-30 16:27:17.179605 musif-1.0.1.post1/musif/extract/features/harmony/utils.py
--rw-r--r--   0        0        0        0 2023-01-30 15:04:50.292017 musif-1.0.1.post1/musif/extract/features/key/__init__.py
--rw-r--r--   0        0        0      165 2023-01-30 15:04:50.292017 musif-1.0.1.post1/musif/extract/features/key/constants.py
--rw-r--r--   0        0        0     1044 2023-01-30 16:27:17.179605 musif-1.0.1.post1/musif/extract/features/key/handler.py
--rw-r--r--   0        0        0       25 2023-01-30 15:04:50.292017 musif-1.0.1.post1/musif/extract/features/lyrics/__init__.py
--rw-r--r--   0        0        0      113 2023-01-30 15:04:50.292017 musif-1.0.1.post1/musif/extract/features/lyrics/constants.py
--rw-r--r--   0        0        0     3669 2023-01-30 15:04:50.292017 musif-1.0.1.post1/musif/extract/features/lyrics/handler.py
--rw-r--r--   0        0        0       25 2023-02-07 16:21:32.258088 musif-1.0.1.post1/musif/extract/features/melody/__init__.py
--rw-r--r--   0        0        0    10448 2023-02-07 16:21:32.258088 musif-1.0.1.post1/musif/extract/features/melody/constants.py
--rw-r--r--   0        0        0    27913 2023-02-07 16:21:32.258088 musif-1.0.1.post1/musif/extract/features/melody/handler.py
--rw-r--r--   0        0        0     3554 2023-01-30 15:04:50.292017 musif-1.0.1.post1/musif/extract/features/prefix.py
--rw-r--r--   0        0        0        0 2023-01-30 15:04:50.292017 musif-1.0.1.post1/musif/extract/features/rhythm/__init__.py
--rw-r--r--   0        0        0      273 2023-02-07 16:21:32.258088 musif-1.0.1.post1/musif/extract/features/rhythm/constants.py
--rw-r--r--   0        0        0     5983 2023-02-07 16:21:32.258088 musif-1.0.1.post1/musif/extract/features/rhythm/handler.py
--rw-r--r--   0        0        0        0 2023-01-30 15:04:50.292017 musif-1.0.1.post1/musif/extract/features/scale/__init__.py
--rw-r--r--   0        0        0      218 2023-01-30 15:04:50.292017 musif-1.0.1.post1/musif/extract/features/scale/constants.py
--rw-r--r--   0        0        0     3627 2023-01-30 15:04:50.292017 musif-1.0.1.post1/musif/extract/features/scale/handler.py
--rw-r--r--   0        0        0        0 2023-01-30 15:04:50.292017 musif-1.0.1.post1/musif/extract/features/scale_relative/__init__.py
--rw-r--r--   0        0        0      102 2023-01-30 15:04:50.292017 musif-1.0.1.post1/musif/extract/features/scale_relative/constants.py
--rw-r--r--   0        0        0     2842 2023-01-30 16:27:17.179605 musif-1.0.1.post1/musif/extract/features/scale_relative/handler.py
--rw-r--r--   0        0        0     7321 2023-01-30 16:27:17.179605 musif-1.0.1.post1/musif/extract/features/scale_relative/utils.py
--rw-r--r--   0        0        0        0 2023-01-30 15:04:50.292017 musif-1.0.1.post1/musif/extract/features/tempo/__init__.py
--rw-r--r--   0        0        0      306 2023-01-30 15:04:50.292017 musif-1.0.1.post1/musif/extract/features/tempo/constants.py
--rw-r--r--   0        0        0     4795 2023-02-07 16:21:32.258088 musif-1.0.1.post1/musif/extract/features/tempo/handler.py
--rw-r--r--   0        0        0        0 2023-01-30 15:04:50.292017 musif-1.0.1.post1/musif/extract/features/texture/__init__.py
--rw-r--r--   0        0        0       45 2023-01-30 15:04:50.292017 musif-1.0.1.post1/musif/extract/features/texture/constants.py
--rw-r--r--   0        0        0     3077 2023-01-30 15:04:50.292017 musif-1.0.1.post1/musif/extract/features/texture/handler.py
--rw-r--r--   0        0        0    20760 2023-01-30 16:27:17.179605 musif-1.0.1.post1/musif/extract/utils.py
--rw-r--r--   0        0        0     2011 2023-01-30 15:04:50.292017 musif-1.0.1.post1/musif/logs.py
--rw-r--r--   0        0        0       61 2023-01-30 15:04:50.292017 musif-1.0.1.post1/musif/musescore/__init__.py
--rw-r--r--   0        0        0      948 2023-01-30 15:04:50.292017 musif-1.0.1.post1/musif/musescore/common.py
--rw-r--r--   0        0        0       95 2023-01-30 15:04:50.292017 musif-1.0.1.post1/musif/musescore/constants.py
--rw-r--r--   0        0        0       91 2023-01-30 15:04:50.292017 musif-1.0.1.post1/musif/musicxml/__init__.py
--rw-r--r--   0        0        0     6910 2023-01-30 15:04:50.292017 musif-1.0.1.post1/musif/musicxml/common.py
--rw-r--r--   0        0        0    15267 2023-01-30 16:27:17.179605 musif-1.0.1.post1/musif/musicxml/constants.py
--rw-r--r--   0        0        0     2092 2023-01-30 16:27:17.179605 musif-1.0.1.post1/musif/musicxml/key.py
--rw-r--r--   0        0        0    17541 2023-01-30 15:04:50.292017 musif-1.0.1.post1/musif/musicxml/repeat.py
--rw-r--r--   0        0        0     4483 2023-01-30 15:04:50.292017 musif-1.0.1.post1/musif/musicxml/scoring.py
--rw-r--r--   0        0        0     7954 2023-01-30 16:27:17.179605 musif-1.0.1.post1/musif/musicxml/tempo.py
--rw-r--r--   0        0        0        0 2023-01-30 15:04:50.292017 musif-1.0.1.post1/musif/process/__init__.py
--rw-r--r--   0        0        0      410 2023-01-30 15:04:50.292017 musif-1.0.1.post1/musif/process/constants.py
--rw-r--r--   0        0        0    10970 2023-01-30 16:27:17.182939 musif-1.0.1.post1/musif/process/processor.py
--rw-r--r--   0        0        0     7628 2023-02-07 16:21:32.258088 musif-1.0.1.post1/musif/process/utils.py
--rw-r--r--   0        0        0      652 2023-02-22 15:57:04.806483 musif-1.0.1.post1/pyproject.toml
--rw-r--r--   0        0        0      606 1970-01-01 00:00:00.000000 musif-1.0.1.post1/PKG-INFO
+-rw-r--r--   0        0        0      971 2023-04-24 10:50:21.848481 musif-1.1.0/README.md
+-rw-r--r--   0        0        0      258 2023-04-24 10:50:11.261815 musif-1.1.0/musif/__init__.py
+-rw-r--r--   0        0        0     7344 2023-04-24 10:50:21.851815 musif-1.1.0/musif/__main__.py
+-rw-r--r--   0        0        0      232 2023-04-24 10:50:11.261815 musif-1.1.0/musif/cache/__init__.py
+-rw-r--r--   0        0        0    17854 2023-04-24 10:50:21.851815 musif-1.1.0/musif/cache/cache.py
+-rw-r--r--   0        0        0     7606 2023-04-24 10:50:21.851815 musif-1.1.0/musif/cache/utils.py
+-rw-r--r--   0        0        0        1 2023-04-24 10:50:11.261815 musif-1.1.0/musif/common/__init__.py
+-rw-r--r--   0        0        0      202 2023-04-24 10:50:11.261815 musif-1.1.0/musif/common/_constants.py
+-rw-r--r--   0        0        0     2402 2023-04-24 10:50:11.261815 musif-1.1.0/musif/common/_logs.py
+-rw-r--r--   0        0        0     3067 2023-04-24 10:50:11.261815 musif-1.1.0/musif/common/_utils.py
+-rw-r--r--   0        0        0      826 2023-04-24 10:50:11.261815 musif-1.1.0/musif/common/constants.py
+-rw-r--r--   0        0        0     1700 2023-04-24 10:50:11.261815 musif-1.1.0/musif/common/didone_utils.py
+-rw-r--r--   0        0        0     1175 2023-04-24 10:50:11.261815 musif-1.1.0/musif/common/exceptions.py
+-rw-r--r--   0        0        0     4102 2023-04-24 10:50:11.261815 musif-1.1.0/musif/common/sort.py
+-rw-r--r--   0        0        0     2103 2023-04-24 10:50:11.261815 musif-1.1.0/musif/common/translate.py
+-rw-r--r--   0        0        0     7287 2023-04-24 10:50:21.851815 musif-1.1.0/musif/config.py
+-rw-r--r--   0        0        0       52 2023-04-24 10:50:11.261815 musif-1.1.0/musif/extract/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-24 10:50:11.261815 musif-1.1.0/musif/extract/basic_modules/file_name_generic/__init__.py
+-rw-r--r--   0        0        0       34 2023-04-24 10:50:11.261815 musif-1.1.0/musif/extract/basic_modules/file_name_generic/constants.py
+-rw-r--r--   0        0        0      999 2023-04-24 10:50:11.261815 musif-1.1.0/musif/extract/basic_modules/file_name_generic/handler.py
+-rw-r--r--   0        0        0        0 2023-04-24 10:50:11.261815 musif-1.1.0/musif/extract/basic_modules/scoring/__init__.py
+-rw-r--r--   0        0        0      646 2023-04-24 10:50:11.261815 musif-1.1.0/musif/extract/basic_modules/scoring/constants.py
+-rw-r--r--   0        0        0     5686 2023-04-24 10:50:11.261815 musif-1.1.0/musif/extract/basic_modules/scoring/handler.py
+-rw-r--r--   0        0        0     1600 2023-04-24 10:50:11.261815 musif-1.1.0/musif/extract/common.py
+-rw-r--r--   0        0        0     1178 2023-04-24 10:50:11.261815 musif-1.1.0/musif/extract/constants.py
+-rw-r--r--   0        0        0    28678 2023-04-24 10:50:21.851815 musif-1.1.0/musif/extract/extract.py
+-rw-r--r--   0        0        0        0 2023-04-24 10:50:11.261815 musif-1.1.0/musif/extract/features/__init__.py
+-rw-r--r--   0        0        0       25 2023-04-24 10:50:11.261815 musif-1.1.0/musif/extract/features/ambitus/__init__.py
+-rw-r--r--   0        0        0      270 2023-04-24 10:50:11.261815 musif-1.1.0/musif/extract/features/ambitus/constants.py
+-rw-r--r--   0        0        0     2705 2023-04-24 10:50:11.261815 musif-1.1.0/musif/extract/features/ambitus/handler.py
+-rw-r--r--   0        0        0        0 2023-04-24 10:50:11.261815 musif-1.1.0/musif/extract/features/core/__init__.py
+-rw-r--r--   0        0        0      465 2023-04-24 10:50:11.261815 musif-1.1.0/musif/extract/features/core/constants.py
+-rw-r--r--   0        0        0     7246 2023-04-24 10:50:21.851815 musif-1.1.0/musif/extract/features/core/handler.py
+-rw-r--r--   0        0        0       55 2023-04-24 10:50:11.265148 musif-1.1.0/musif/extract/features/density/__init__.py
+-rw-r--r--   0        0        0       57 2023-04-24 10:50:11.265148 musif-1.1.0/musif/extract/features/density/constants.py
+-rw-r--r--   0        0        0     7668 2023-04-24 10:50:21.851815 musif-1.1.0/musif/extract/features/density/handler.py
+-rw-r--r--   0        0        0       25 2023-04-24 10:50:11.265148 musif-1.1.0/musif/extract/features/dynamics/__init__.py
+-rw-r--r--   0        0        0      821 2023-04-24 10:50:21.851815 musif-1.1.0/musif/extract/features/dynamics/constants.py
+-rw-r--r--   0        0        0     9029 2023-04-24 10:50:11.265148 musif-1.1.0/musif/extract/features/dynamics/handler.py
+-rw-r--r--   0        0        0        0 2023-04-24 10:50:11.265148 musif-1.1.0/musif/extract/features/harmony/__init__.py
+-rw-r--r--   0        0        0      815 2023-04-24 10:50:11.265148 musif-1.1.0/musif/extract/features/harmony/constants.py
+-rw-r--r--   0        0        0     2741 2023-04-24 10:50:11.265148 musif-1.1.0/musif/extract/features/harmony/handler.py
+-rw-r--r--   0        0        0    26047 2023-04-24 10:50:11.265148 musif-1.1.0/musif/extract/features/harmony/utils.py
+-rw-r--r--   0        0        0       29 2023-04-24 10:50:21.851815 musif-1.1.0/musif/extract/features/jsymbolic/__init__.py
+-rw-r--r--   0        0        0      282 2023-04-24 10:50:21.851815 musif-1.1.0/musif/extract/features/jsymbolic/__main__.py
+-rw-r--r--   0        0        0     2345 2023-04-24 10:50:21.851815 musif-1.1.0/musif/extract/features/jsymbolic/handler.py
+-rw-r--r--   0        0        0     3381 2023-04-24 10:50:21.851815 musif-1.1.0/musif/extract/features/jsymbolic/utils.py
+-rw-r--r--   0        0        0        0 2023-04-24 10:50:11.265148 musif-1.1.0/musif/extract/features/key/__init__.py
+-rw-r--r--   0        0        0      165 2023-04-24 10:50:11.265148 musif-1.1.0/musif/extract/features/key/constants.py
+-rw-r--r--   0        0        0     1044 2023-04-24 10:50:11.265148 musif-1.1.0/musif/extract/features/key/handler.py
+-rw-r--r--   0        0        0       25 2023-04-24 10:50:11.265148 musif-1.1.0/musif/extract/features/lyrics/__init__.py
+-rw-r--r--   0        0        0      113 2023-04-24 10:50:11.265148 musif-1.1.0/musif/extract/features/lyrics/constants.py
+-rw-r--r--   0        0        0     3669 2023-04-24 10:50:11.265148 musif-1.1.0/musif/extract/features/lyrics/handler.py
+-rw-r--r--   0        0        0       25 2023-04-24 10:50:11.265148 musif-1.1.0/musif/extract/features/melody/__init__.py
+-rw-r--r--   0        0        0    10534 2023-04-24 10:50:21.851815 musif-1.1.0/musif/extract/features/melody/constants.py
+-rw-r--r--   0        0        0    30504 2023-04-24 10:50:21.851815 musif-1.1.0/musif/extract/features/melody/handler.py
+-rw-r--r--   0        0        0       80 2023-04-24 10:50:21.851815 musif-1.1.0/musif/extract/features/music21/__init__.py
+-rw-r--r--   0        0        0      173 2023-04-24 10:50:21.851815 musif-1.1.0/musif/extract/features/music21/constants.py
+-rw-r--r--   0        0        0     2182 2023-04-24 10:50:21.851815 musif-1.1.0/musif/extract/features/music21/handler.py
+-rw-r--r--   0        0        0     3554 2023-04-24 10:50:11.265148 musif-1.1.0/musif/extract/features/prefix.py
+-rw-r--r--   0        0        0        0 2023-04-24 10:50:11.265148 musif-1.1.0/musif/extract/features/rhythm/__init__.py
+-rw-r--r--   0        0        0      273 2023-04-24 10:50:11.265148 musif-1.1.0/musif/extract/features/rhythm/constants.py
+-rw-r--r--   0        0        0     5925 2023-04-24 10:50:21.851815 musif-1.1.0/musif/extract/features/rhythm/handler.py
+-rw-r--r--   0        0        0        0 2023-04-24 10:50:11.265148 musif-1.1.0/musif/extract/features/scale/__init__.py
+-rw-r--r--   0        0        0      269 2023-04-24 10:50:21.851815 musif-1.1.0/musif/extract/features/scale/constants.py
+-rw-r--r--   0        0        0     3627 2023-04-24 10:50:11.265148 musif-1.1.0/musif/extract/features/scale/handler.py
+-rw-r--r--   0        0        0        0 2023-04-24 10:50:11.265148 musif-1.1.0/musif/extract/features/scale_relative/__init__.py
+-rw-r--r--   0        0        0      102 2023-04-24 10:50:11.265148 musif-1.1.0/musif/extract/features/scale_relative/constants.py
+-rw-r--r--   0        0        0     2842 2023-04-24 10:50:11.265148 musif-1.1.0/musif/extract/features/scale_relative/handler.py
+-rw-r--r--   0        0        0     7321 2023-04-24 10:50:11.265148 musif-1.1.0/musif/extract/features/scale_relative/utils.py
+-rw-r--r--   0        0        0        0 2023-04-24 10:50:11.265148 musif-1.1.0/musif/extract/features/tempo/__init__.py
+-rw-r--r--   0        0        0      306 2023-04-24 10:50:11.265148 musif-1.1.0/musif/extract/features/tempo/constants.py
+-rw-r--r--   0        0        0     5145 2023-04-24 10:50:21.851815 musif-1.1.0/musif/extract/features/tempo/handler.py
+-rw-r--r--   0        0        0        0 2023-04-24 10:50:11.265148 musif-1.1.0/musif/extract/features/texture/__init__.py
+-rw-r--r--   0        0        0       45 2023-04-24 10:50:11.265148 musif-1.1.0/musif/extract/features/texture/constants.py
+-rw-r--r--   0        0        0     3077 2023-04-24 10:50:11.265148 musif-1.1.0/musif/extract/features/texture/handler.py
+-rw-r--r--   0        0        0    21081 2023-04-24 10:50:21.851815 musif-1.1.0/musif/extract/utils.py
+-rw-r--r--   0        0        0     2011 2023-04-24 10:50:11.265148 musif-1.1.0/musif/logs.py
+-rw-r--r--   0        0        0       61 2023-04-24 10:50:11.265148 musif-1.1.0/musif/musescore/__init__.py
+-rw-r--r--   0        0        0      948 2023-04-24 10:50:11.265148 musif-1.1.0/musif/musescore/common.py
+-rw-r--r--   0        0        0       95 2023-04-24 10:50:11.265148 musif-1.1.0/musif/musescore/constants.py
+-rw-r--r--   0        0        0       91 2023-04-24 10:50:11.265148 musif-1.1.0/musif/musicxml/__init__.py
+-rw-r--r--   0        0        0     7532 2023-04-24 10:50:21.851815 musif-1.1.0/musif/musicxml/common.py
+-rw-r--r--   0        0        0    15310 2023-04-24 10:50:21.851815 musif-1.1.0/musif/musicxml/constants.py
+-rw-r--r--   0        0        0     2092 2023-04-24 10:50:11.265148 musif-1.1.0/musif/musicxml/key.py
+-rw-r--r--   0        0        0    17541 2023-04-24 10:50:11.268481 musif-1.1.0/musif/musicxml/repeat.py
+-rw-r--r--   0        0        0     4513 2023-04-24 10:50:21.851815 musif-1.1.0/musif/musicxml/scoring.py
+-rw-r--r--   0        0        0     8151 2023-04-24 10:50:21.851815 musif-1.1.0/musif/musicxml/tempo.py
+-rw-r--r--   0        0        0        0 2023-04-24 10:50:11.268481 musif-1.1.0/musif/process/__init__.py
+-rw-r--r--   0        0        0      410 2023-04-24 10:50:11.268481 musif-1.1.0/musif/process/constants.py
+-rw-r--r--   0        0        0    11327 2023-04-24 10:50:21.851815 musif-1.1.0/musif/process/processor.py
+-rw-r--r--   0        0        0     7824 2023-04-24 10:50:21.855148 musif-1.1.0/musif/process/utils.py
+-rw-r--r--   0        0        0      650 2023-04-24 10:50:21.855148 musif-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1212 1970-01-01 00:00:00.000000 musif-1.1.0/PKG-INFO
```

### Comparing `musif-1.0.1.post1/musif/cache/cache.py` & `musif-1.1.0/musif/cache/cache.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 import random
-import traceback
+import weakref
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from deepdiff import DeepHash, deephash
 
 from musif.common.exceptions import CannotResurrectObject, SmartCacheModified
 from musif.logs import pinfo, pwarn
 
@@ -60,14 +60,18 @@
             pinfo(f"Resurrecting via function call: {func}{args}")
             self.reference = func(*args)
             # self.deephash = DeepHash(self.reference)
 
     def get_attr(self, name: str) -> Any:
         if not hasattr(self, "reference") or self.reference is None:
             # pinfo(f"Resurrecting reference object due to call to attribute '{name}'")
+            # traceback = __import__('traceback')
+            # traceback.print_list(
+            #     [f for f in traceback.extract_stack() if "musif" in f.filename]
+            # )
             self._try_resurrect()
         return getattr(self.reference, name)
 
     def __getstate__(self):
         return dict(
             resurrect_reference=self.resurrect_reference,
             parent=self.parent,
@@ -251,14 +255,15 @@
     def __delattr__(self, name):
         del self.cache[name]
 
     def __setattr__(self, name, value):
         pwarn(
             "You are using a music21 object in writing mode! consider change your code so that SmartModuleCache works correctly. See the stack-trace:"
         )
+        # traceback = __import__('traceback')
         # traceback.print_list(
         #     [f for f in traceback.extract_stack() if "musif" in f.filename]
         # )
         if self.cache["_reference"].reference is not None:
             self.cache["_reference"].get_attr("__setattr__")(name, value)
 
     def _get_new_attr(self, name: str) -> Any:
@@ -326,14 +331,15 @@
             self.cache[f"__item_{k}"] = v
         return v
 
     def __setitem__(self, k, v):
         pwarn(
             "You are using a music21 object in writing mode! consider change your code so that SmartModuleCache works correctly. See the stack-trace:"
         )
+        # traceback = __import__('traceback')
         # traceback.print_list(
         #     [f for f in traceback.extract_stack() if "musif" in f.filename]
         # )
         try:
             v = self.cache["_reference"].get_attr("__getitem__")(k)
         except KeyError:
             pass
@@ -374,32 +380,49 @@
 
     Note that `DeepHash` may be much slower than the builtin `hash()` function,
     so for large and complex objects like `music21.Score`, just use a
     `SmartModuleCache` wrapper.
     """
 
     def __init__(self, *args, **kwargs):
-        self.args = args
-        self.kwargs = kwargs
+        self.args = []
+        self.kwargs = {}
+
+        # removing weakreferences (cannot be pickled)
+        for arg in args:
+            if isinstance(arg, weakref.ReferenceType):
+                __import__('ipdb').set_trace()
+                self.args.append(arg())
+            else:
+                self.args.append(arg)
+
+        for k, v in kwargs.items():
+            if isinstance(k, weakref.ReferenceType):
+                __import__('ipdb').set_trace()
+                k = k()
+            if isinstance(v, weakref.ReferenceType):
+                __import__('ipdb').set_trace()
+                v = v()
+            kwargs[k] = v
 
         h = ""
 
-        # hashing  SmartModuleCache
+        # hashing SmartModuleCache
         for arg in self.args:
             if type(arg) is SmartModuleCache:
                 h += str(hash(arg))
 
         kwargs_keys = sorted(self.kwargs.keys())
         for k in kwargs_keys:
             v = self.kwargs[k]
             if type(v) is SmartModuleCache:
                 h += str(hash(v))
 
         # hashing other object types by value
-        all_args = (args, kwargs)
+        all_args = (self.args, self.kwargs)
         h += DeepHash(all_args, exclude_types=[SmartModuleCache])[all_args]
 
         self._hash = int(h, 16)
 
     def __hash__(self):
         return self._hash
 
@@ -472,18 +495,19 @@
         else:
             attr = self.reference.get_attr(self.name)
             if self.special_method:
                 args = [arg.cache["_reference"].reference for arg in args]
                 kwargs = {k: v.cache["_reference"].reference for k, v in kwargs.items()}
             res = attr(*args, **kwargs)
             if res is None:
-                res = _MyNone
+                # caching _MyNone and returning None
+                self.cache[call_args] = _MyNone
             else:
                 res = self._wmo(res, args=(*args, *kwargs.values()))
-            self.cache[call_args] = res
+                self.cache[call_args] = res
             if self.check_reference_changes and self.reference.ischanged():
                 pwarn(str(SmartCacheModified(self, self.name)))
             return res
 
     def smartforcecache(self, *args, **kwargs):
         self.__call__(*args, **kwargs)
         assert (
```

### Comparing `musif-1.0.1.post1/musif/cache/utils.py` & `musif-1.1.0/musif/cache/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import builtins
 import pickle
+import weakref
 from pathlib import PurePath, Path
 from typing import Any, List, Optional, Tuple
 
 import music21 as m21
 import pandas as pd
 
 from musif.cache.cache import MethodCache, ObjectReference, SmartModuleCache
@@ -85,15 +86,23 @@
 ):
     """
     Returns the object wrapped with `SmartModuleCache` class if it was defined
     in one of the `target_addresses`
 
     If `obj` is a list or a tuple, e new list/tuple this function works
     recursively on their objects.
-    """
+
+    If the object is an instance of `weakref.ReferenceType`
+    this function converts the object to a regular
+    reference and then applies the wrapping.
+    """
+    if isinstance(obj, weakref.ReferenceType):
+        __import__('ipdb').set_trace()
+        return obj()
+
     __module = obj.__class__.__module__
     for module in target_addresses:
         if __module.startswith(module):
             return SmartModuleCache(
                 reference=obj,
                 target_addresses=target_addresses,
                 resurrect_reference=resurrect_reference,
@@ -112,17 +121,16 @@
                 (*name, "__getitem__"),
                 (*args, (i,)),
             )
             for i, v in enumerate(obj)
         ]
         if isinstance(obj, list):
             return ret
-        else:
+        elif isinstance(obj, tuple):
             return tuple(ret)
-
     return obj
 
 
 def store_score_df(score, fname):
     """
     Stores `score` into `fname` (a file-like object, a string or a Path object)
     using dataframes and returns the object saved.
```

### Comparing `musif-1.0.1.post1/musif/common/_logs.py` & `musif-1.1.0/musif/common/_logs.py`

 * *Files identical despite different names*

### Comparing `musif-1.0.1.post1/musif/common/_utils.py` & `musif-1.1.0/musif/common/_utils.py`

 * *Files identical despite different names*

### Comparing `musif-1.0.1.post1/musif/common/constants.py` & `musif-1.1.0/musif/common/constants.py`

 * *Files identical despite different names*

### Comparing `musif-1.0.1.post1/musif/common/didone_utils.py` & `musif-1.1.0/musif/common/didone_utils.py`

 * *Files identical despite different names*

### Comparing `musif-1.0.1.post1/musif/common/exceptions.py` & `musif-1.1.0/musif/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `musif-1.0.1.post1/musif/common/sort.py` & `musif-1.1.0/musif/common/sort.py`

 * *Files identical despite different names*

### Comparing `musif-1.0.1.post1/musif/common/translate.py` & `musif-1.1.0/musif/common/translate.py`

 * *Files identical despite different names*

### Comparing `musif-1.0.1.post1/musif/config.py` & `musif-1.1.0/musif/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,25 +9,29 @@
 LOG = "log"
 LOG_FILE_PATH = "log_file"
 FILE_LOG_LEVEL = "file_log_level"
 CONSOLE_LOG_LEVEL = "console_log_level"
 XML_DIR = "xml_dir"
 MUSESCORE_DIR = "musescore_dir"
 CACHE_DIR = "cache_dir"
+IGNORE_ERRORS = "ignore_errors"
 PARALLEL = "parallel"
 FEATURES = "features"
 BASIC_MODULES = "basic_modules"
 BASIC_MODULES_ADDRESSES = "basic_modules_addresses"
 FEATURE_MODULES_ADDRESSES = "feature_modules_addresses"
 PARTS_FILTER = "parts_filter"
 EXPAND_REPEATS = "expand_repeats"
 WINDOW_SIZE = "window_size"
 OVERLAP = "overlap"
 PRECACHE_HOOKS = "precache_hooks"
+REMOVE_UNPITCHED_OBJECTS = "remove_unpitched_objects"
 MSCORE_EXEC = "mscore_exec"
+JSYMBOLIC_CONFIG_FILE = "jsymbolic_config_file"
+JSYMBOLIC_MAX_RAM = "jsymbolic_max_ram"
 # Didone specific?
 SPLIT_KEYWORDS = "split_keywords"
 
 DELETE_FILES = "delete_failed_files"
 DELETE_HARMONY = "delete_files_without_harmony"
 UNBUNDLE_INSTRUMENTATION = "separate_intrumentation_column"
 INSTRUMENTS_TO_KEEP = "instruments_to_keep"
@@ -36,38 +40,44 @@
 STARTSWITH = "columns_startswith"
 CONTAIN = "columns_contain"
 MATCH = "columns_match"
 REPLACE_NANS = "replace_nans"
 DFS_DIR = "dfs_dir"
 GROUPED = "grouped_analysis"
 MERGE_VOICES = "merge_voices"
+MAX_NAN_COLUMNS = "max_nan_columns"
+MAX_NAN_ROWS = "max_nan_rows"
 
 _CONFIG_LOG_FALLBACK = {
     LOG_FILE_PATH: "./musif.log",
     FILE_LOG_LEVEL: "DEBUG",
     CONSOLE_LOG_LEVEL: "ERROR",
 }
 
 _CONFIG_FALLBACK = {
     XML_DIR: None,
     MUSESCORE_DIR: None,
     CACHE_DIR: None,
     PARALLEL: 1,
     PRECACHE_HOOKS: [],
     BASIC_MODULES: [],
+    IGNORE_ERRORS: False,
     BASIC_MODULES_ADDRESSES: ["musif.extract.basic_modules"],
     FEATURE_MODULES_ADDRESSES: ["musif.extract.features"],
     FEATURES: ["core"],
     SPLIT_KEYWORDS: [],
     PARTS_FILTER: [],
     EXPAND_REPEATS: False,
     WINDOW_SIZE: None,
     OVERLAP: 2,
     MSCORE_EXEC: None,
     DFS_DIR: None,
+    REMOVE_UNPITCHED_OBJECTS: True,
+    JSYMBOLIC_MAX_RAM: "4g",
+    JSYMBOLIC_CONFIG_FILE: None
 }
 
 _CONFIG_POST_FALLBACK = {
     DELETE_FILES: False,
     GROUPED: False,
     DELETE_FILES: False,
     DELETE_HARMONY: False,
@@ -75,15 +85,17 @@
     MERGE_VOICES: True,
     INSTRUMENTS_TO_KEEP: [],
     INSTRUMENTS_TO_DELETE: [],
     ENDSWITH: [],
     STARTSWITH: [],
     CONTAIN: [],
     REPLACE_NANS: [],
-    MATCH: []
+    MATCH: [],
+    MAX_NAN_COLUMNS: None,
+    MAX_NAN_ROWS: None
 }
 
 
 class GenericConfiguration:
     """
     Generic class for configuration objects.
```

### Comparing `musif-1.0.1.post1/musif/config.py~` & `musif-1.1.0/musif/__main__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,213 +1,180 @@
-from pathlib import PurePath
-
-from musif.common._logs import create_logger
-from musif.common._utils import read_object_from_yaml_file
-from musif.extract.constants import REQUIRE_MSCORE
-
-# TODO: add documentation for these variables
-LOGGER_NAME = "musiF"
-LOG = "log"
-LOG_FILE_PATH = "log_file"
-FILE_LOG_LEVEL = "file_log_level"
-CONSOLE_LOG_LEVEL = "console_log_level"
-XML_DIR = "xml_dir"
-MUSESCORE_DIR = "musescore_dir"
-CACHE_DIR = "cache_dir"
-PARALLEL = "parallel"
-FEATURES = "features"
-BASIC_MODULES = "basic_modules"
-BASIC_MODULES_ADDRESSES = "basic_modules_addresses"
-FEATURE_MODULES_ADDRESSES = "feature_modules_addresses"
-PARTS_FILTER = "parts_filter"
-EXPAND_REPEATS = "expand_repeats"
-WINDOW_SIZE = "window_size"
-OVERLAP = "overlap"
-PRECACHE_HOOKS = "precache_hooks"
-MSCORE_EXEC = "mscore_exec"
-# Didone specific?
-SPLIT_KEYWORDS = "split_keywords"
-
-DELETE_FILES = "delete_failed_files"
-DELETE_HARMONY = "delete_files_without_harmony"
-UNBUNDLE_INSTRUMENTATION = "separate_intrumentation_column"
-INSTRUMENTS_TO_KEEP = "instruments_to_keep"
-INSTRUMENTS_TO_DELETE = "instruments_to_delete"
-ENDSWITH = "columns_endswith"
-STARTSWITH = "columns_startswith"
-CONTAIN = "columns_contain"
-MATCH = "columns_match"
-REPLACE_NANS = "replace_nans"
-DFS_DIR = "dfs_dir"
-GROUPED = "grouped_analysis"
-MERGE_VOICES = "merge_voices"
-
-_CONFIG_LOG_FALLBACK = {
-    LOG_FILE_PATH: "./musiF.log",
-    FILE_LOG_LEVEL: "DEBUG",
-    CONSOLE_LOG_LEVEL: "ERROR",
-}
-
-_CONFIG_FALLBACK = {
-    XML_DIR: None,
-    MUSESCORE_DIR: None,
-    CACHE_DIR: None,
-    PARALLEL: 1,
-    PRECACHE_HOOKS: [],
-    BASIC_MODULES: [],
-    BASIC_MODULES_ADDRESSES: ["musif.extract.basic_modules"],
-    FEATURE_MODULES_ADDRESSES: ["musif.extract.features"],
-    FEATURES: ["core"],
-    SPLIT_KEYWORDS: [],
-    PARTS_FILTER: [],
-    EXPAND_REPEATS: False,
-    WINDOW_SIZE: None,
-    OVERLAP: 2,
-    MSCORE_EXEC: None,
-    DFS_DIR: None,
-}
-
-_CONFIG_POST_FALLBACK = {
-    DELETE_FILES: False,
-    GROUPED: False,
-    DELETE_FILES: False,
-    DELETE_HARMONY: False,
-    UNBUNDLE_INSTRUMENTATION: False,
-    MERGE_VOICES: True,
-    INSTRUMENTS_TO_KEEP: [],
-    INSTRUMENTS_TO_DELETE: [],
-    ENDSWITH: [],
-    STARTSWITH: [],
-    CONTAIN: [],
-    REPLACE_NANS: [],
-    MATCH: []
-}
-
-
-class GenericConfiguration:
-    """
-    Generic class for configuration objects.
-
-    When subclassing, you should override the `_get_fallback` method.
-    """
-
-    def _get_fallback(self):
-        """
-        Returns a dictionary containing the default values for this configuration
-        object. Such values will be always available, but can be overriden by the
-        user.
-        """
-        return {}
-
-    def __init__(self, arg, **kwargs):
-        """
-        It set up the `Configuration` object in this way:
-
-            #. it sets the default values returned by `self._get_fallback()` as filed of
-               the object (i.e. in the `__dict__` dictionary)
-            #. it load the configuration file `arg` provided by the user
-            #. it overrides the configuration file with the keyword arguments
-            #. it sets the values obtained, overriding the one already available, in
-               `__dict_`, making them avilable as usual fields
-        """
-        # set default values
-        for fallback in [_CONFIG_LOG_FALLBACK, self._get_fallback()]:
-            for k, v in fallback.items():
-                self.__dict__[k] = v
-
-        # load configuration file
-        config_data = {}
-        if arg is not None:
-            if isinstance(arg, str) or isinstance(arg, PurePath):
-                config_data = read_object_from_yaml_file(arg)
-            elif isinstance(arg, dict):
-                config_data = arg
-            elif isinstance(arg, GenericConfiguration):
-                config_data = arg.to_dict()
-            else:
-                raise TypeError(
-                    f"The argument type is {type(arg)}, and it was expected a dictionary, a Configuration or a string object"
+import sys
+from typing import Optional
+from pathlib import Path
+
+import musif.musicxml.constants as musicxml_c
+from musif.config import ExtractConfiguration, PostProcessConfiguration
+from musif.extract.extract import FeaturesExtractor
+from musif.logs import perr, pinfo
+from musif.process.processor import DataProcessor
+
+
+def main(
+    *paths,
+    output_path: str = "musif_features.csv",
+    source_dir: str = None,
+    extension: str = ".xml",
+    njobs: int = -1,
+    cache_dir: str = "musif_cache",
+    ignore_errors: bool = True,
+    yaml: str = None,
+    tweaks: dict = {},
+    harmony: Optional[str] = None,
+):
+    """
+    Python tool for extracting features from music score files.
+
+    This tool uses `music21` to load files, so any file format supported by `music21`
+    also works, e.g. MIDI, MusicXML, Kern, ABC files. It uses cache, parallel
+    processing, and ignore errors by default. See the options to disable them.
+
+    This tool uses a default configuration that should work well in most cases. See
+    [paper] for more benchmarks. By default, it extracts all features except the ones
+    that require harmonic annotations. You can use `-y/--yaml` and `-c/--config` for
+    more tweaks.
+
+    Examples of usage:
+        musif dataset/**/*.mid
+            -> process all the midi files in `dataset`, searching files recursively in
+            all the sub-directories
+        musif *.xml --cache_dir=None
+            -> process all xml files in this directory without using cache
+        musif --source_dir=dataset --extension=.krn
+            -> process all kern files in the directory `dataset`, searching files
+            recursively in all the sub-drectories
+        musif -- -h
+            -> shows this help
+
+    Installation:
+        If you have musif installed in your environment, you can access this tool using
+        `python -m musif`.
+
+        Alternatively, you can install musif system-wide with `pipx install musif`
+        (see pipx documentation for instructions: https://pypa.github.io/pipx/)
+
+    Args:
+        paths : one or more paths to file; if provided, the extraction is limited to
+            them; these paths can be absolute or relative to the current
+            directory; all the paths should contain a common parent part;
+            incompatible with `--source_dir`
+        output_path : output file; extension is added or changed to 'csv'
+        extension : extension, including the dot, e.g. '.mid', '.krn', '.mxl'; only
+            has effect if `source_dir` is used, otherwise it's
+            inferred from the file names; if one of ['.mxl', '.xml',
+            '.musicxml'] is passed, all the other used as well; you can
+            set it to a list or to a tuple to include multiple
+            extensions;
+        source_dir : relative path to the directory; searched recursively;
+            incompatible with other files provided
+        njobs : number of jobs used, according to joblib: -1 means "all the
+            available virtual cores"; 1 means no parallel processing
+        cache_dir : directory where cache files are saved; set to 'None' to disable
+        ignore_errors : True or False; if False, blocks when a file cannot be
+            processed, if True, cprints a warning and continue
+        yaml : path to a configuration file that will be used for both extraction and
+            post-processing; command line options have the precedence on this yaml file
+        tweaks : Further flags can be used to change musif's configuration
+            (see the docs for possible options); for this, you should
+            pass them as a dictionary, e.g. `musif -t
+            '{musescore_dir: "mscore_data"}'`
+        harmony : extract harmonic features using musescore files from this directory
+    """
+
+    if source_dir is not None and len(paths) > 0:
+        perr("Please, provide only one option between `source_dir` and file paths")
+        sys.exit(1)
+
+    if source_dir is None and len(paths) == 0:
+        perr("Please, provide at least one option between `source_dir` and file paths")
+        sys.exit(2)
+
+    if source_dir is None:
+        # look for the common parent part into `limit_to_files`
+        first_file = Path(paths[0])
+        source_dir = first_file.parent
+
+        _source_dir = str(source_dir)
+        extension = first_file.suffix
+
+        for file in paths[1:]:
+            file_ = Path(file)
+            if file_.suffix != extension:
+                perr(
+                    f"Please provide files with only one extension: first file has extension {extension}, but {file_} has extension {file_.suffix}"
                 )
+            while not file.startswith(_source_dir):
+                source_dir = source_dir.parent
+                _source_dir = str(source_dir)
+        pinfo(f"Detected parent directory: {_source_dir}")
+        pinfo(f"Detected extension: {extension}")
+    else:
+        paths = None
+        if extension in [".xml", ".mxl", ".musicxml"]:
+            extension = [".xml", ".mxl", ".musicxml"]
+
+    config = ExtractConfiguration(
+        yaml,
+        xml_dir=source_dir,
+        cache_dir=cache_dir,
+        parallel=njobs,
+        musescore_dir=harmony,
+        ignore_errors=ignore_errors,
+        **tweaks,
+    )
+    if config.features == ["core"]:
+        config.features = [
+            "core",
+            "ambitus",
+            "melody",
+            "tempo",
+            "density",
+            "texture",
+            "lyrics",
+            "scale",
+            "key",
+            "dynamics",
+            "rhythm",
+            "music21",
+        ]
+    if harmony is not None:
+        config.features += ["harmony", "scale_relative"]
+    if len(config.basic_modules) == 0:
+        config.basic_modules = ["scoring"]
+    musicxml_c.MUSIC21_FILE_EXTENSIONS = extension
+    raw_df = FeaturesExtractor(config, limit_files=paths).extract()
+
+    output_path = Path(output_path).with_suffix(".csv")
+    # raw_df.to_csv(output_path.with_suffix(".raw.csv"), index=False)
+
+    config = PostProcessConfiguration(yaml, **tweaks)
+    if len(config.columns_contain) == 0:
+        config.columns_contain = [
+            "_Count",
+            "_SmallestInterval",
+            "_NumberOfFilteredParts",
+        ]
+    if len(config.replace_nans) == 0:
+        config.replace_nans = ["Interval", "Degree", "Harmony"]
+    if config.max_nan_rows is None:
+        # if the columns without nans would produce a table with columns/row ratio <
+        # 0.25, we remove the rows that are outliers of the 0.99 quantile
+        raw_df_na = raw_df.isna()
+        num_columns_without_na = (~raw_df_na.any(axis=0)).sum()
+        if num_columns_without_na / raw_df.shape[0] < 0.1:
+            nans = raw_df_na.sum(axis=1)
+            config.max_nan_rows = 1 / 0.99 * nans.quantile(0.99) / raw_df.shape[1]
+        else:
+            config.max_nan_rows = 1.0
+    if config.max_nan_columns is None:
+        config.max_nan_columns = 0.0
+    processed_df = DataProcessor(raw_df, config).process().data
+    # replace empty strings with "NA" only in string columns
+    string_cols = processed_df.select_dtypes(include=["object", "string"]).columns
+    processed_df[string_cols] = processed_df[string_cols].replace("", "-")
+    processed_df.to_csv(output_path, index=False)
 
-        # override values with kwargs
-        config_data.update(kwargs)
-        log_config = config_data.get(LOG, {})
-        for config in [config_data, log_config]:
-            for k, v in config.items():
-                if k == LOG:
-                    continue
-                self.__dict__[k] = v
-
-        create_logger(
-            LOGGER_NAME, self.log_file, self.file_log_level, self.console_log_level
-        )
-
-    def to_dict(self) -> dict:
-        """
-        Returns a dictionary having as keys the public fields of this object.
-        """
-        return {k: v for k, v in self.__dict__.items() if not k.startswith("_")}
-
-
-class ExtractConfiguration(GenericConfiguration):
-    """
-    Configuration object used by :class: `musif.extract.extract.FeatureExtractor`
 
-    It additionaly sets the following properties:
-
-    ..  code-block:: python
-
-        from musif.musicxml import constants as musicxml_c
-        self.scoring_family_order = musicxml_c.SCORING_FAMILY_ORDER
-        self.scoring_order = musicxml_c.SCORING_ORDER
-        self.sound_to_family = musicxml_c.SOUND_TO_FAMILY
-        self.family_to_abbreviation = musicxml_c.FAMILY_TO_ABBREVIATION
-        self.sound_to_abbreviation = musicxml_c.SOUND_TO_ABBREVIATION
-
-    The above settings can be overriden by the user both by changing
-    the variables in `musicxml.constants` and by adding them to the configuration.
-    """
-
-    def __init__(self, *args, **kwargs):
-        from musif.musicxml import constants as musicxml_c
-        # ^--- here to avoid circular imports
-        self.scoring_family_order = musicxml_c.SCORING_FAMILY_ORDER
-        self.scoring_order = musicxml_c.SCORING_ORDER
-        self.sound_to_family = musicxml_c.SOUND_TO_FAMILY
-        self.family_to_abbreviation = musicxml_c.FAMILY_TO_ABBREVIATION
-        self.sound_to_abbreviation = musicxml_c.SOUND_TO_ABBREVIATION
-        super().__init__(*args, **kwargs)
-
-    def _get_fallback(self):
-        return _CONFIG_FALLBACK
-
-    def is_requested_musescore_file(self) -> bool:
-        """
-        Returns `True` if any of the requested features needs musescore files for the
-        harmonic annotations.
-        Returns `False` otherwise.
-        """
-
-        for feature in REQUIRE_MSCORE:
-            if self.is_requested_feature_category(feature):
-                return True
-        return False
-
-    def is_requested_feature_category(self, feature: str) -> bool:
-        """
-        Returns `True` if `feature` is among the requeste features, according to the
-        configuration.
-        Returns `False` otherwise.
-        """
-
-        if self.features is None:
-            return True
-        return feature in self.features
-
-
-class PostProcessConfiguration(GenericConfiguration):
-    """
-    Configuration object used by :class: `musif.process.DataProcessor`
-    """
+if __name__ == "__main__":
+    import fire
 
-    def _get_fallback(self):
-        return _CONFIG_POST_FALLBACK
+    fire.Fire(main, name="musif")
```

### Comparing `musif-1.0.1.post1/musif/extract/basic_modules/file_name_generic/handler.py` & `musif-1.1.0/musif/extract/basic_modules/file_name_generic/handler.py`

 * *Files identical despite different names*

### Comparing `musif-1.0.1.post1/musif/extract/basic_modules/scoring/constants.py` & `musif-1.1.0/musif/extract/basic_modules/scoring/constants.py`

 * *Files identical despite different names*

### Comparing `musif-1.0.1.post1/musif/extract/basic_modules/scoring/handler.py` & `musif-1.1.0/musif/extract/basic_modules/scoring/handler.py`

 * *Files identical despite different names*

### Comparing `musif-1.0.1.post1/musif/extract/common.py` & `musif-1.1.0/musif/extract/common.py`

 * *Files identical despite different names*

### Comparing `musif-1.0.1.post1/musif/extract/constants.py` & `musif-1.1.0/musif/extract/constants.py`

 * *Files identical despite different names*

### Comparing `musif-1.0.1.post1/musif/extract/extract.py` & `musif-1.1.0/musif/extract/extract.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,33 +21,38 @@
     SmartModuleCache,
     store_score_df,
 )
 from musif.common._constants import GENERAL_FAMILY
 from musif.common.exceptions import FeatureError, ParseFileError
 from musif.config import ExtractConfiguration
 from musif.extract.common import _filter_parts_data
-from musif.extract.utils import extract_global_time_signature, process_musescore_file, cast_mixed_dtypes
-from musif.logs import ldebug, lerr, linfo, lwarn, perr, pinfo, pdebug, pwarn
+from musif.extract.utils import (
+    cast_mixed_dtypes,
+    extract_global_time_signature,
+    process_musescore_file,
+)
+from musif.logs import ldebug, lerr, linfo, lwarn, pdebug, perr, pinfo
 from musif.musescore import constants as mscore_c
 from musif.musicxml import constants as musicxml_c
-from musif.musicxml import extract_numeric_tempo, split_layers
+from musif.musicxml import extract_numeric_tempo, name_parts, split_layers
 from musif.musicxml.scoring import (
     _extract_abbreviated_part,
     extract_sound,
     to_abbreviation,
 )
 
 _cache = FileCacheIntoRAM(10000)  # To cache scanned scores
 
 
 def parse_filename(
     file_path: str,
     split_keywords: List[str],
     expand_repeats: bool = False,
     export_dfs_to: Union[str, PurePath] = None,
+    remove_unpitched_objects: bool = True,
 ) -> Score:
     """
     This function parses a musicxml file and returns a music21 Score object. If
     the file has already been parsed, it will be loaded from cache instead of
     processing it again. Split a part in different parts if the instrument
     family is in keywords argument and expands repeats if indicated.
 
@@ -76,14 +81,21 @@
         return score
     try:
         score = parse(file_path)
         if export_dfs_to is not None:
             dest_path = Path(export_dfs_to)
             dest_path /= Path(file_path).with_suffix(".pkl").name
             store_score_df(score, dest_path)
+        # give a name to all parts in the score
+        name_parts(score)
+        if remove_unpitched_objects:
+            unpitched_objs = list(
+                score.flatten().getElementsByClass(["PercussionChord", "Unpitched"])
+            )
+            score.remove(unpitched_objs, recurse=True)
         split_layers(score, split_keywords)
         if expand_repeats:
             score = score.expandRepeats()
         _cache.put(file_path, score)
     except Exception as e:
         print(file_path)
         raise ParseFileError(file_path) from e
@@ -121,37 +133,37 @@
         harmonic_analysis = None
         print(file_path)
         raise ParseFileError(file_path) from e
     return harmonic_analysis
 
 
 def find_files(
-    extension: str,
+    extensions: str or List[str],
     base_dir: Union[str, List[Union[str, PurePath]]],
     limit_files: List[str] = None,
     exclude_files: List[str] = None,
 ) -> List[PurePath]:
     """Extracts the paths to files given an extension
 
     Given a directory path, return a list of paths of files found, in alphabetic order.
     It searches recursively inside `base_dir`. If `base_dir` is a fileor a list of paths
     or directories with `extension`, it is returned in a list. If given neither a string
     nor list of strings raise a TypeError and if the file doesn't exists returns a
     ValueError.
 
     Parameters
     ----------
-    extension: str
-        A string representing the extension that will be looked for
+    extension: str or Iterable[str]
+        A list of strings representing the extensions that will be looked for
     base_dir : Union[str, Iterable[str]]
         A path or directory
-    limit_files: List[str] = None
+    limit_files: Iterable[str] = None
         List of file names relative to `base_dir`. Only these files are taken.
         Incompatible with `exclude_files`
-    exclude_files: List[str] = None
+    exclude_files: Iterable[str] = None
         List of file names relative to `base_dir`. None of these files are taken.
         Incompatible with `limit_files`
 
     Returns
     -------
     resp : List[PurePath]
       The list of musicxml files found in the provided arguments
@@ -161,45 +173,52 @@
     ------
     TypeError
       If the type is not the expected (str or List[str]).
 
     ValueError
       If the provided string is neither a directory nor a file path
     """
+    if isinstance(extensions, str):
+        extensions = [extensions]
+
     if base_dir is None:
         return []
     base_dir = Path(base_dir)
     if not base_dir.exists():
         raise ValueError(f"File {base_dir} doesn't exist")
     elif base_dir.is_dir():
-        ret = sorted(base_dir.glob(f"**/*{extension}"))
+        ret = []
+        for ext in extensions:
+            ret += sorted([f for f in base_dir.glob(f"**/*{ext}") if f.is_file()])
         if limit_files is not None:
             limit_stems = set(map(lambda x: Path(x).stem, limit_files))
             return [f for f in ret if f.stem in limit_stems]
         elif exclude_files is not None:
             exclude_stems = set(map(lambda x: Path(x).stem, exclude_files))
             return [f for f in ret if f.stem not in exclude_stems]
         else:
             return ret
-    elif base_dir.is_file() and base_dir.suffix == f"{extension}":
+    elif base_dir.is_file() and base_dir.suffix in extensions:
         return [base_dir]
     else:
         return []
 
 
 #  sorted(obj.glob(f"*{extension}"))
 class FeaturesExtractor:
     """
     Extract features for a score or a list of scores, according to the parameters
-    established in the configurtaion files. It extracts musical features from .xml and
-    .mscx files based on the configuration and stores them in a dictionary
-    (score features) that at the end will be returned as a DataFrame. Features
-    corresponds to modules placed in musif/features directory, and will be computed in
-    order according to the configuration. Some features might depend on the previous
-    ones, so order is important.
+    established in the configuration files. It extracts musical features using music21
+    and ms3 library, based on the configuration and stores them in a dictionary
+    (score features) that at the end will be returned as a DataFrame by the
+    `extract` method.
+
+    During the parsing, unpitched objects, (e.g. objects referred to percussion
+    instruments) may be removed (see the option
+    `remove_unpitched_objects` in the configuration).
 
     """
 
     def __init__(self, *args, **kwargs):
         """
         Parameters
         ----------
@@ -231,14 +250,20 @@
         )
         # self.regex = re.compile("from {FEATURES_MODULES}.([\w\.]+) import")
         # creates the directory for the cache
         if self._cfg.cache_dir is not None:
             pinfo("Cache activated!")
             Path(self._cfg.cache_dir).mkdir(exist_ok=True)
 
+        if "jsymbolic" in self._cfg.features:
+            from musif.extract.features import jsymbolic
+
+            jsymbolic.utils.download_jsymbolic()
+            jsymbolic.utils.get_java_path()
+
     def extract(self) -> DataFrame:
         """
         Extracts features given in the configuration data getting a file, directory or several file paths,
         returning a DataFrame containing musical features.
 
         Returns
         ------
@@ -250,15 +275,15 @@
            If the musicxml file can't be parsed for any reason.
         KeyError
            If features aren't loaded in corrected order or dependencies
         """
         linfo("--- Analyzing scores ---\n".center(120, " "))
 
         xml_filenames = find_files(
-            musicxml_c.MUSICXML_FILE_EXTENSION,
+            musicxml_c.MUSIC21_FILE_EXTENSIONS,
             self._cfg.xml_dir,
             limit_files=self.limit_files,
             exclude_files=self.exclude_files,
         )
         musescore_filenames = find_files(
             mscore_c.MUSESCORE_FILE_EXTENSION,
             self._cfg.musescore_dir,
@@ -294,18 +319,27 @@
 
         return score_df
 
     def _process_corpus(
         self, filenames: List[PurePath]
     ) -> Tuple[List[dict], List[dict]]:
         def process_corpus_par(idx, filename):
-            if self._cfg.window_size is not None:
-                score_features = self._process_score_windows(idx, filename)
-            else:
-                score_features = self._process_score(idx, filename)
+            try:
+                if self._cfg.window_size is not None:
+                    score_features = self._process_score_windows(idx, filename)
+                else:
+                    score_features = self._process_score(idx, filename)
+            except Exception as e:
+                if self._cfg.ignore_errors:
+                    lerr(
+                        f"Error while extracting features for file {filename}, skipping it because `ignore_errors` is True!"
+                    )
+                    return {}
+                else:
+                    raise e
             return score_features
 
         scores_features = Parallel(n_jobs=self._cfg.parallel)(
             delayed(process_corpus_par)(idx, fname)
             for idx, fname in enumerate(tqdm(filenames))
         )
 
@@ -316,22 +350,25 @@
                 df_score = df_score.reindex(sorted(df_score.columns), axis=1)
                 df_score.replace("NA", pd.NA, inplace=True)
                 all_dfs.append(df_score)
             all_dfs = pd.concat(all_dfs, axis=0, keys=range(len(all_dfs)))
         else:
             all_dfs = DataFrame(scores_features)
             all_dfs = all_dfs.reindex(sorted(all_dfs.columns), axis=1)
-            all_dfs.replace("NA", pd.NA, inplace=True)
+            all_dfs = all_dfs.replace("NA", pd.NA)
         return all_dfs
 
     def _init_score_processing(self, idx: int, filename: PurePath):
         if self._cfg.cache_dir is not None:
-            cache_name = Path(self._cfg.cache_dir) / (
-                filename.with_suffix(CACHE_FILE_EXTENSION).name
+            cache_name = (
+                Path(self._cfg.cache_dir)
+                / filename.parent
+                / (filename.name + CACHE_FILE_EXTENSION)
             )
+            cache_name.parent.mkdir(parents=True, exist_ok=True)
         else:
             cache_name = None
         score_data = self._get_score_data(filename, load_cache=cache_name)
         parts_data = [
             self._get_part_data(score_data, part)
             for part in score_data[C.DATA_SCORE].parts
         ]
@@ -346,28 +383,26 @@
 
         (
             basic_features,
             cache_name,
             parts_data,
             score_data,
         ) = self._init_score_processing(idx, filename)
+        extract_global_time_signature(score_data)
         score_features = self.extract_modules(
             self._cfg.feature_modules_addresses, score_data, parts_data, basic=False
         )
-        extract_global_time_signature(score_data)
         score_features = {**basic_features, **score_features}
         score_features[C.WINDOW_ID] = 0
 
         if self._cfg.cache_dir is not None:
             pickle.dump(score_data, open(cache_name, "wb"))
         return score_features
 
-    def _process_score_windows(
-        self, idx: int, filename: PurePath
-    ) -> List[dict]:
+    def _process_score_windows(self, idx: int, filename: PurePath) -> List[dict]:
         (
             basic_features,
             cache_name,
             parts_data,
             score_data,
         ) = self._init_score_processing(idx, filename)
 
@@ -408,22 +443,25 @@
 
             all_windows_features.append(window_features)
             first_window_measure = last_window_measure - self._cfg.overlap
 
         if self._cfg.cache_dir is not None:
             pickle.dump(score_data, open(cache_name, "wb"))
         return all_windows_features
-    
+
     def _select_window_data(
         self, score_data: dict, parts_data: list, first_measure: int, last_measure: int
     ):
         window_score = score_data[C.DATA_SCORE].measures(
             first_measure, last_measure, indicesNotNumbers=True
         )
-        window_parts = window_score.parts
+        filtered_partNames = [i.partName for i in score_data["parts"]]
+        window_parts = [
+            i for i in window_score.parts if i.partName in filtered_partNames
+        ]
         if (
             self._cfg.is_requested_musescore_file()
             and score_data[C.DATA_MUSESCORE_SCORE] is not None
         ):
             window_mscore = score_data[C.DATA_MUSESCORE_SCORE].loc[
                 (score_data[C.DATA_MUSESCORE_SCORE]["mn"] <= last_measure)
                 & (score_data[C.DATA_MUSESCORE_SCORE]["mn"] >= first_measure)
@@ -468,29 +506,30 @@
                 raise RuntimeError(
                     "Cannot find musescore executable. Please provide xml files or the path to a musescore installation with the configuration `mscore_exec`"
                 )
             if not isinstance(mscore, (list, tuple)):
                 # this is needed to allow stuffs like `xvfb-run -a mscore`
                 mscore = (mscore,)
             tmp_d, tmp_path = mkstemp(
-                prefix=filename.stem, suffix=musicxml_c.MUSICXML_FILE_EXTENSION
+                prefix=filename.stem, suffix=musicxml_c.MUSIC21_FILE_EXTENSIONS[0]
             )
             process = mscore + ("-fo", tmp_path, filename)
             res = subprocess.run(process, stdout=DEVNULL, stderr=DEVNULL)
             if res.returncode != 0:
                 raise RuntimeError(
                     f"Error while converting musescore file to xml: {filename}"
                 )
         else:
             tmp_path = filename
         score = parse_filename(
             tmp_path,
             self._cfg.split_keywords,
             expand_repeats=self._cfg.expand_repeats,
             export_dfs_to=self._cfg.dfs_dir,
+            remove_unpitched_objects=self._cfg.remove_unpitched_objects,
         )
         numeric_tempo = extract_numeric_tempo(tmp_path)
         if filename.suffix == mscore_c.MUSESCORE_FILE_EXTENSION:
             os.close(tmp_d)
             os.remove(tmp_path)
         filtered_parts = self._filter_parts(score)
         return score, tuple(filtered_parts), numeric_tempo
@@ -542,15 +581,15 @@
                 C.DATA_FILE: str(filename),
                 C.DATA_FILTERED_PARTS: filtered_parts,
                 C.DATA_MUSESCORE_SCORE: data_musescore,
                 C.DATA_NUMERIC_TEMPO: numeric_tempo,
             }
             if len(self._cfg.precache_hooks) > 0:
                 for hook in self._cfg.precache_hooks:
-                    if isinstance(hook,str):
+                    if isinstance(hook, str):
                         hook = __import__(hook, fromlist=[""])
                     hook.execute(self._cfg, data)
             if self._cfg.cache_dir is not None:
                 m21_objects = SmartModuleCache(
                     (data[C.DATA_SCORE], data[C.DATA_FILTERED_PARTS]),
                     resurrect_reference=(
                         self._load_xml_data,
@@ -580,15 +619,15 @@
             except ParseFileError as e:
                 data_musescore = None
                 lerr(str(e))
                 return None
 
     def _filter_parts(self, score: Score) -> List[Part]:
         parts = list(score.parts)
-        self._deal_with_dupicated_parts(parts)
+        # self._deal_with_dupicated_parts(parts)
         if self._cfg.parts_filter is None or len(self._cfg.parts_filter) == 0:
             return parts
         filter_set = set(self._cfg.parts_filter)
         return (
             part
             for part in parts
             if to_abbreviation(part, parts, self._cfg) in filter_set
@@ -628,15 +667,15 @@
                 module = __import__(f.__name__ + "." + name, fromlist=[""])
             except ModuleNotFoundError as e:
                 return e
         return module
 
     def _find_modules(self, package: str, basic: bool):
         found_features = set()
-        if isinstance(package,str):
+        if isinstance(package, str):
             package = __import__(package, fromlist=[""])
         if basic:
             to_extract = self._cfg.basic_modules
         else:
             to_extract = self._cfg.features
         for feature in to_extract:
             feature_package = self._get_module_or_attribute(package, feature)
```

### Comparing `musif-1.0.1.post1/musif/extract/features/ambitus/handler.py` & `musif-1.1.0/musif/extract/features/ambitus/handler.py`

 * *Files identical despite different names*

### Comparing `musif-1.0.1.post1/musif/extract/features/core/handler.py` & `musif-1.1.0/musif/extract/features/core/handler.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from os import path
 from typing import List
 import pandas as pd
 from music21 import *
 from music21.stream import Measure
-from musif.extract.constants import DATA_FILTERED_PARTS 
+from musif.extract.constants import DATA_FILTERED_PARTS
 from musif.extract.features.tempo.constants import TIME_SIGNATURE
 
 from musif.config import ExtractConfiguration
 from musif.extract.basic_modules.scoring.constants import (
     FAMILY_ABBREVIATION,
     NUMBER_OF_FILTERED_PARTS,
     SOUND_ABBREVIATION,
@@ -84,26 +84,26 @@
         and (not score_data[DATA_MUSESCORE_SCORE].empty)
     ):
         tonality_ms3 = score_data[DATA_MUSESCORE_SCORE].globalkey[0]
         if key_name != tonality_ms3:
             score_key = key.Key(tonality_ms3)
             mode, key_name = get_name_from_key(score_key)
 
-    score_features[FILE_NAME] = path.basename(score_data[DATA_FILE])
+    score_features[FILE_NAME] = path.abspath(score_data[DATA_FILE])
     num_measures = len(score.parts[0].getElementsByClass(Measure))
     key_signature = _get_key_signature(score_key)
-    
+
     part = score.parts[0]
-    time_signature = _get_time_signature(list(part.getElementsByClass(Measure)), score_data)
+    time_signature = _get_time_signature(score_data)
 
     score_data.update(
         {
             DATA_KEY: score_key,
             KEY_SIGNATURE: key_signature,
-            TIME_SIGNATURE: time_signature,      
+            TIME_SIGNATURE: time_signature,
             KEY_SIGNATURE: key_signature,
             DATA_KEY_NAME: key_name,
             DATA_MODE: mode,
             DATA_MEASURES: num_measures,
         }
     )
 
@@ -171,13 +171,31 @@
     features[get_score_feature(NUM_NOTES)] = notes
     features[get_score_feature(NOTES_MEAN)] = notes_mean
     features[get_score_feature(NUM_SOUNDING_MEASURES)] = sounding_measures
     features[get_score_feature(SOUNDING_MEASURES_MEAN)] = sounding_measures_mean
     features[NUM_MEASURES] = num_measures
     score_features.update(features)
 
-def _get_time_signature(measures: list, score_data: dict):
-    if GLOBAL_TIME_SIGNATURE in score_data:
+
+def _get_time_signature(score_data: dict) -> str:
+    """
+    This function takes in a dictionary of score data and returns the global time
+    signature of the score as a string.
+
+    Parameters:
+    score_data (dict): A dictionary containing score data.
+
+    Returns:
+    str: A string representing the time signature of the score. It is `'NA'`
+        if no time signature is found.
+    """
+    if hasattr(score_data.get(GLOBAL_TIME_SIGNATURE), 'ratioString'):
         time_signature = score_data[GLOBAL_TIME_SIGNATURE].ratioString
     else:
-        time_signature = score_data[DATA_FILTERED_PARTS][0].getElementsByClass(Measure)[0].timeSignature.ratioString
+        first_measure = score_data[DATA_FILTERED_PARTS][0].getElementsByClass(Measure)[
+            0
+        ]
+        if hasattr(first_measure.timeSignature, 'ratioString'):
+            time_signature = first_measure.timeSignature.ratioString
+        else:
+            time_signature = "NA"
     return time_signature
```

### Comparing `musif-1.0.1.post1/musif/extract/features/density/handler.py` & `musif-1.1.0/musif/extract/features/density/handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,20 +48,21 @@
 def update_part_objects(
     score_data: dict, part_data: dict, cfg: ExtractConfiguration, part_features: dict
 ):
     if not _part_matches_filter(part_data[DATA_PART_ABBREVIATION], cfg.parts_filter):
         return {}
     notes = part_data[DATA_NOTES]
     sounding_measures = part_data[DATA_SOUNDING_MEASURES]
-    measures = part_data[DATA_MEASURES]
+    # measures = part_data[DATA_MEASURES]
     # time_signature = score_data[TIME_SIGNATURE].split(",")
-    time_signatures = score_data[TIME_SIGNATURES]
-    sounding_measures = range(
-        0, len(sounding_measures)
-    )  ## TODO: cuando haya repeticiones, revisar esto. Lo hice por un error en la numeracion cuando hay 70x1 (celdillas)
+    time_signatures = part_data[TIME_SIGNATURES]
+    # sounding_measures = range(
+    #     0, len(sounding_measures)
+    # )  
+    ## TODO: cuando haya repeticiones, revisar esto. Lo hice por un error en la numeracion cuando hay 70x1 (celdillas)
     sounding_time_signatures = [time_signatures[i] for i in sounding_measures]
 
     part_features.update(
         {
             SOUNDING_DENSITY: len(notes)
             / _calculate_total_number_of_beats(sounding_time_signatures)
             if len(sounding_time_signatures) > 0
```

### Comparing `musif-1.0.1.post1/musif/extract/features/dynamics/constants.py` & `musif-1.1.0/musif/extract/features/dynamics/constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 
 DYNAMIC = "Dynamic"  # all coulf be in a dictionary with this variables?
 TEXTEXPRESSION = "TextExpression"
 TIMESIGNATURE = "TimeSignature"
 REST = "Rest"
 
 DYNAMIC_VALUES = {
+    "sfz": 127,
+    "fz": 120,
+    "ffff": 116,
+    "fff": 112,
     "ff": 101,
     "più f": 96,
     "f assai": 94,
     "assaif": 94,
     "f": 88,
     "sempre f": 88,
     "poco f": 80,
@@ -21,14 +25,17 @@
     "p": 49,
     "più p": 46,
     "sempre p": 49,
     "p dolce": 49,
     "poco p": 49,
     "p assai": 42,
     "pp": 36,
+    "ppp": 24,
+    "sfp": 20,
+    "pppp": 12,
     "sempre pp": 36,
     "sotto voce assai": 36,
     "dolce": 49,
 }
 
 DYNAMIC_LAST_WORD = ["assai", "dolce"]
```

### Comparing `musif-1.0.1.post1/musif/extract/features/dynamics/handler.py` & `musif-1.1.0/musif/extract/features/dynamics/handler.py`

 * *Files identical despite different names*

### Comparing `musif-1.0.1.post1/musif/extract/features/harmony/constants.py` & `musif-1.1.0/musif/extract/features/harmony/constants.py`

 * *Files identical despite different names*

### Comparing `musif-1.0.1.post1/musif/extract/features/harmony/handler.py` & `musif-1.1.0/musif/extract/features/harmony/handler.py`

 * *Files identical despite different names*

### Comparing `musif-1.0.1.post1/musif/extract/features/harmony/utils.py` & `musif-1.1.0/musif/extract/features/harmony/utils.py`

 * *Files identical despite different names*

### Comparing `musif-1.0.1.post1/musif/extract/features/key/handler.py` & `musif-1.1.0/musif/extract/features/key/handler.py`

 * *Files identical despite different names*

### Comparing `musif-1.0.1.post1/musif/extract/features/lyrics/handler.py` & `musif-1.1.0/musif/extract/features/lyrics/handler.py`

 * *Files identical despite different names*

### Comparing `musif-1.0.1.post1/musif/extract/features/melody/constants.py` & `musif-1.1.0/musif/extract/features/melody/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,14 +117,16 @@
 
 SPEED_AVG_ABS = "Spe_avg_abs"
 ACCELERATION_AVG_ABS = "Acc_avg_abs"
 ASCENDENT_AVERAGE = "Asc_avg"
 DESCENDENT_AVERAGE = "Dsc_avg"
 ASCENDENT_PROPORTION = "Asc_prp"
 DESCENDENT_PROPORTION = "Dsc_prp"
+MOTION_STEPS = [0.125, 0.25, 0.5, 1.0, 2.0, 4.0, 8.0]
+MOTION_WINS = [2, 4, 8, 16, 32]
 
 SCORE_FEATURES = [
     MEAN_INTERVAL,
     INTERVALLIC_MEAN,
     INTERVALLIC_STD,
     ABSOLUTE_INTERVALLIC_MEAN,
     ABSOLUTE_INTERVALLIC_STD,
```

### Comparing `musif-1.0.1.post1/musif/extract/features/melody/handler.py` & `musif-1.1.0/musif/extract/features/melody/handler.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-import re
-from asyncio import constants
 from collections import Counter
+from itertools import groupby
 from statistics import mean, stdev
-from typing import List, Tuple
+from typing import List, Tuple, Dict, Union
 
 import numpy as np
+import pandas as pd
 from music21.interval import Interval
 from scipy.stats import kurtosis, skew
 from scipy.stats.mstats import trimmed_mean, trimmed_std
 
+from musif.cache import hasattr
 from musif.common._utils import extract_digits
 from musif.config import ExtractConfiguration
 from musif.extract.common import _mix_data_with_precedent_data
 from musif.extract.constants import DATA_PART_ABBREVIATION, DATA_SOUND_ABBREVIATION
 from musif.extract.features.core.constants import DATA_INTERVALS
 from musif.extract.features.prefix import (
     get_part_feature,
@@ -24,53 +25,59 @@
 from .constants import *
 
 
 def update_part_objects(
     score_data: dict, part_data: dict, cfg: ExtractConfiguration, part_features: dict
 ):
     intervals = part_data[DATA_INTERVALS]
-    motion_features = get_motion_features(part_data)
-    part_features.update(motion_features)
 
+    part_features.update(get_motion_features(part_data))
     part_features.update(get_interval_features(intervals))
     part_features.update(get_interval_count_features(intervals))
     part_features.update(get_interval_type_features(intervals))
     part_features.update(get_interval_stats_features(intervals))
 
 
 def update_score_objects(
     score_data: dict,
     parts_data: List[dict],
     cfg: ExtractConfiguration,
     parts_features: List[dict],
     score_features: dict,
 ):
-
     if len(parts_data) == 0:
         return
 
     features = {}
     for part_data, part_features in zip(parts_data, parts_features):
         part = part_data[DATA_PART_ABBREVIATION]
-        features[get_part_feature(part, SPEED_AVG_ABS)] = part_features[SPEED_AVG_ABS]
-        features[get_part_feature(part, ACCELERATION_AVG_ABS)] = part_features[
-            ACCELERATION_AVG_ABS
-        features[get_part_feature(part, ASCENDENT_AVERAGE)] = part_features[
-            ASCENDENT_AVERAGE
-        ]
-        features[get_part_feature(part, DESCENDENT_AVERAGE)] = part_features[
-            DESCENDENT_AVERAGE
-        ]
-        features[get_part_feature(part, ASCENDENT_PROPORTION)] = part_features[
-            ASCENDENT_PROPORTION
-        ]
-        features[get_part_feature(part, DESCENDENT_PROPORTION)] = part_features[
-            DESCENDENT_PROPORTION
-        ]
-        
+        for step in MOTION_STEPS:
+            for win in MOTION_WINS:
+                if step > win:
+                    continue
+                key_postfix = _motion_postfix(step, win)
+                features[
+                    get_part_feature(part, SPEED_AVG_ABS + key_postfix)
+                ] = part_features[SPEED_AVG_ABS + key_postfix]
+                features[
+                    get_part_feature(part, ACCELERATION_AVG_ABS + key_postfix)
+                ] = part_features[ACCELERATION_AVG_ABS + key_postfix]
+                features[
+                    get_part_feature(part, ASCENDENT_AVERAGE + key_postfix)
+                ] = part_features[ASCENDENT_AVERAGE + key_postfix]
+                features[
+                    get_part_feature(part, DESCENDENT_AVERAGE + key_postfix)
+                ] = part_features[DESCENDENT_AVERAGE + key_postfix]
+                features[
+                    get_part_feature(part, ASCENDENT_PROPORTION + key_postfix)
+                ] = part_features[ASCENDENT_PROPORTION + key_postfix]
+                features[
+                    get_part_feature(part, DESCENDENT_PROPORTION + key_postfix)
+                ] = part_features[DESCENDENT_PROPORTION + key_postfix]
+
         part_prefix = get_part_prefix(part_data[DATA_PART_ABBREVIATION])
         intervals = part_data[DATA_INTERVALS]
         interval_features = get_interval_features(intervals, part_prefix)
         interval_count_features = get_interval_count_features(intervals, part_prefix)
         interval_type_features = get_interval_type_features(intervals, part_prefix)
         interval_stats_features = get_interval_stats_features(intervals, part_prefix)
 
@@ -316,15 +323,14 @@
         interval_features[INTERVAL_PER.format(prefix=prefix, interval=interval)] = (
             count / total_count if total_count else 0
         )
     return interval_features
 
 
 def get_interval_type_features(intervals_list: List[Interval], prefix: str = ""):
-
     repeated_notes_list = []
     stepwise_list = []
     leaps_list = []
     within_octave_list = []
     beyond_octave_list = []
     perfect_list = []
     major_list = []
@@ -588,72 +594,88 @@
             else None
         )
         absolute_intervals_kurtosis = (
             kurtosis(absolute_numeric_intervals, bias=False)
             if [i for i in absolute_numeric_intervals if i != 0]
             else None
         )
-        
+
     return {
         f"{prefix}{INTERVALLIC_SKEWNESS}": intervals_skewness,
         f"{prefix}{INTERVALLIC_KURTOSIS}": intervals_kurtosis,
         f"{prefix}{ABSOLUTE_INTERVALLIC_SKEWNESS}": absolute_intervals_skewness,
         f"{prefix}{ABSOLUTE_INTERVALLIC_KURTOSIS}": absolute_intervals_kurtosis,
     }
 
 
-def get_motion_features(part_data) -> dict:
-    notes_midi = []
-    notes_duration = []
-    for note in part_data["notes_and_rests"]:
-        if hasattr(note, "pitch"):
-            notes_midi.append(note.pitch.midi)
-            notes_duration.append(note.duration.quarterLength)
-    
-    notes_midi = np.asarray(notes_midi)
-    notes_duration = np.asarray(notes_duration)
+def _motion_postfix(step, win):
+    key_postfix = f"_step_{step}_win_{win}"
+    return key_postfix
+
+
+def _motion_features_single_window_step(
+    notes_duration: List[float], notes_midi: List[int], step: float, win: int
+) -> Dict[str, Union[float, np.ndarray]]:
+    """
+    Calculates motion features for a single window step of an aria.
+
+    Parameters:
+    notes_duration (List[float]): List of note durations in seconds.
+    notes_midi (List[int]): List of MIDI note numbers.
+    step (float): Step size in seconds.
+    win (int): Window size in compasses.
+
+    Returns:
+    Dict[str, Union[float, np.ndarray]]: Dictionary containing the following motion features:
+        - SPEED_AVG_ABS_{step}_{win} Average absolute speed.
+        - ACCELERATION_AVG_ABS_{step}_{win} Average absolute acceleration.
+        - ASCENDENT_AVERAGE_{step}_{win} Average length of prolonged ascent chunks in the smoothed midis of the aria.
+        - DESCENDENT_AVERAGE_{step}_{win} Average length of prolonged descent chunks in the smoothed midis of the aria.
+        - ASCENDENT_PROPORTION_{step}_{win} Proportion of prolonged ascent chunks over the total of the aria.
+        - DESCENDENT_PROPORTION_{step}_{win} Proportion of prolonged descent chunks over the total of the aria.
+    """
+    key_postfix = _motion_postfix(step, win)
+    default_dict = {
+        SPEED_AVG_ABS + key_postfix: 0,
+        ACCELERATION_AVG_ABS + key_postfix: 0,
+        ASCENDENT_AVERAGE + key_postfix: 0,
+        DESCENDENT_AVERAGE + key_postfix: 0,
+        ASCENDENT_PROPORTION + key_postfix: 0,
+        DESCENDENT_PROPORTION + key_postfix: 0,
+    }
     
     if len(notes_midi) == 0:
-        return {
-            SPEED_AVG_ABS: 0,
-            ACCELERATION_AVG_ABS: 0,
-            ASCENDENT_AVERAGE: 0,
-            DESCENDENT_AVERAGE: 0,
-            ASCENDENT_PROPORTION: 0,
-            DESCENDENT_PROPORTION: 0,
-        }
+        return default_dict
+    midis_raw = np.repeat(notes_midi, np.divide(notes_duration, step).astype(int), axis=0)
+    if midis_raw.size == 0:
+        return default_dict
 
-    step = 0.125
-    midis_raw = np.repeat(notes_midi, [i / step for i in notes_duration], axis=0)
+    # Absolute means of speed and acceleration
     spe_raw = np.diff(midis_raw) / step
+    if spe_raw.size > 0:
+        spe_avg_abs = np.mean(abs(spe_raw))
+    else:
+        spe_avg_abs = 0
     acc_raw = np.diff(spe_raw) / step
-
-    # Absolute means of speed and acceleration
-    spe_avg_abs = np.mean(abs(spe_raw))
-    acc_avg_abs = np.mean(abs(acc_raw))
+    if acc_raw.size > 0:
+        acc_avg_abs = np.mean(abs(acc_raw))
+    else:
+        acc_avg_abs = 0
 
     # Rolling mean to smooth the midis by +-1 compasses -- not required for
     # statistics based on means but important for detecting increasing sequences
     # with a tolerance.
-    measure = 4
     midis_smo_series = pd.Series(midis_raw)
     midis_smo = [
-        np.mean(i.to_list())
-        for i in midis_smo_series.rolling(2 * measure + 1, center=True)
+        np.mean(i.to_list()) for i in midis_smo_series.rolling(2 * win + 1, center=True)
     ]
 
-    # midis_smo = np.rollmean(midis_raw, k = 2 * compass + 1, align = "center")
-
-    # spe_smo = np.diff(midis_smo) / step
-    # acc_smo = np.diff(spe_smo) / step
-
     # Prolonged ascent/descent chunks in smoothed midis of the aria (allows for
     # small violations in the form of decrements/increments that do not
     # decrease/increase the rolling mean).
-
     dife = np.diff(midis_smo)
 
     asc = [(k, sum(1 for i in g)) for k, g in groupby(dife > 0)]
     dsc = [(k, sum(1 for i in g)) for k, g in groupby(dife < 0)]
 
     asc = [i for b, i in asc if b]
     dsc = [i for b, i in dsc if b]
@@ -663,14 +685,48 @@
     dsc_avg = mean(dsc) if dsc else np.nan
 
     # Proportion of ascent/descent chunks over the total of the aria
     asc_prp = sum(asc) / (len(dife) - 1) if asc else np.nan
     dsc_prp = sum(dsc) / (len(dife) - 1) if dsc else np.nan
 
     return {
-        SPEED_AVG_ABS: spe_avg_abs,
-        ACCELERATION_AVG_ABS: acc_avg_abs,
-        ASCENDENT_AVERAGE: asc_avg,
-        DESCENDENT_AVERAGE: dsc_avg,
-        ASCENDENT_PROPORTION: asc_prp,
-        DESCENDENT_PROPORTION: dsc_prp,
+        SPEED_AVG_ABS + key_postfix: spe_avg_abs,
+        ACCELERATION_AVG_ABS + key_postfix: acc_avg_abs,
+        ASCENDENT_AVERAGE + key_postfix: asc_avg,
+        DESCENDENT_AVERAGE + key_postfix: dsc_avg,
+        ASCENDENT_PROPORTION + key_postfix: asc_prp,
+        DESCENDENT_PROPORTION + key_postfix: dsc_prp,
     }
+
+
+def get_motion_features(part_data) -> dict:
+    """
+    Extracts motion features from the given part data.
+
+    Parameters:
+    part_data (dict): A dictionary containing the notes and rests of a music part.
+
+    Returns:
+    dict: A dictionary containing the extracted motion features.
+
+    Raises:
+    This function does not raise any exceptions.
+    """
+    notes_midi = []
+    notes_duration = []
+    for note in part_data["notes_and_rests"]:
+        if hasattr(note, "pitch"):
+            notes_midi.append(note.pitch.midi)
+            notes_duration.append(note.duration.quarterLength)
+
+    notes_midi = np.asarray(notes_midi)
+    notes_duration = np.asarray(notes_duration)
+
+    return_dict = {}
+    for step in MOTION_STEPS:
+        for win in MOTION_WINS:
+            return_dict.update(
+                _motion_features_single_window_step(
+                    notes_duration, notes_midi, step, win
+                )
+            )
+    return return_dict
```

### Comparing `musif-1.0.1.post1/musif/extract/features/prefix.py` & `musif-1.1.0/musif/extract/features/prefix.py`

 * *Files identical despite different names*

### Comparing `musif-1.0.1.post1/musif/extract/features/rhythm/handler.py` & `musif-1.1.0/musif/extract/features/rhythm/handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 from collections import Counter, defaultdict
-from itertools import groupby
 from statistics import mean
 from typing import List
 
 import numpy as np
-import pandas as pd
 
-from musif.cache import hasattr
 from musif.config import ExtractConfiguration
 from musif.extract.constants import DATA_PART_ABBREVIATION, GLOBAL_TIME_SIGNATURE
 from musif.extract.features.core.constants import DATA_NOTES
 from musif.extract.features.prefix import get_part_feature, get_score_feature
 from musif.extract.utils import _get_beat_position
 from musif.musicxml.tempo import get_number_of_beats
 
@@ -30,15 +27,15 @@
     rhythm_intensity_period = []
     rhythm_dot = 0
     rhythm_double_dot = 0
     total_beats = 0
     total_sounding_beats = 0
     beat_count = (
         score_data[GLOBAL_TIME_SIGNATURE].beatCount
-        if GLOBAL_TIME_SIGNATURE in score_data
+        if hasattr(score_data.get(GLOBAL_TIME_SIGNATURE), 'beatCount')
         else 1
     )
     # motion_features = get_motion_features(part_data)
     # part_features.update(motion_features)
 
     for measure in part_data["measures"]:
         for i, element in enumerate(measure.elements):
```

### Comparing `musif-1.0.1.post1/musif/extract/features/scale/handler.py` & `musif-1.1.0/musif/extract/features/scale/handler.py`

 * *Files identical despite different names*

### Comparing `musif-1.0.1.post1/musif/extract/features/scale_relative/handler.py` & `musif-1.1.0/musif/extract/features/scale_relative/handler.py`

 * *Files identical despite different names*

### Comparing `musif-1.0.1.post1/musif/extract/features/scale_relative/utils.py` & `musif-1.1.0/musif/extract/features/scale_relative/utils.py`

 * *Files identical despite different names*

### Comparing `musif-1.0.1.post1/musif/extract/features/tempo/handler.py` & `musif-1.1.0/musif/extract/features/tempo/handler.py`

 * *Files 22% similar despite different names*

```diff
@@ -29,17 +29,28 @@
     FAST = "Fast"
 
 
 def update_part_objects(
     score_data: dict, part_data: dict, cfg: ExtractConfiguration, part_features: dict
 ):
     part = part_data[DATA_PART]
-    time_signature = list(part.getTimeSignatures())[0].ratioString
-    time_signature_grouped = get_time_signature_type(time_signature)
-    number_of_beats = get_number_of_beats(time_signature)
+
+    (
+        time_signature,
+        measures,
+        time_signatures,
+        time_signature_grouped,
+        number_of_beats,
+    ) = extract_time_signatures(list(part.getElementsByClass(Measure)), score_data)
+    part_data.update(
+        {
+            C.TIME_SIGNATURES: time_signatures,
+            C.TS_MEASURES: measures,
+        }
+    )
     part_features.update(
         {
             C.TIME_SIGNATURE: time_signature,
             C.TIME_SIGNATURE_GROUPED: time_signature_grouped,
             C.NUMBER_OF_BEATS: number_of_beats,
         }
     )
@@ -49,87 +60,90 @@
     score_data: dict,
     parts_data: List[dict],
     cfg: ExtractConfiguration,
     parts_features: List[dict],
     score_features: dict,
 ):
 
-    # cogemos la part de la voz, y de ahí sacamos el time signature, aparte de
-    # devolverla para su posterior uso cambiamos la forma de extraer la voz --- se hace
-    # con el atributo de part, 'instrumentSound'. Este atributo indica el tipo de
-    # instrumento y por ultimo el nombre. voice.soprano, strings.violin o strings.viola
-    # for part in score.parts:
-    # m = list(part.getTimeSignatures())
-    # time_signature = m[0].ratioString
-    # time_signatures.append(time_signature)
-
     score = score_data[DATA_SCORE]
+    # for the features, we use the first part as reference!
     part = score.parts[0]
     numeric_tempo, tempo_mark = extract_tempo(score_data, part)
     tempo_grouped_1 = get_tempo_grouped_1(tempo_mark)
     tempo_grouped_2 = get_tempo_grouped_2(tempo_grouped_1)
 
     (
         time_signature,
         measures,
         time_signatures,
         time_signature_grouped,
         number_of_beats,
     ) = extract_time_signatures(list(part.getElementsByClass(Measure)), score_data)
 
-    score_data.update(
-        {
-            C.TIME_SIGNATURE: time_signature,
-            C.TIME_SIGNATURES: time_signatures,
-            C.TS_MEASURES: measures,
-        }
-    )
-
     score_features.update(
         {
             C.TEMPO: tempo_mark,
             C.NUMERIC_TEMPO: numeric_tempo,
-            C.TIME_SIGNATURE: time_signature.split(",")[0],
+            C.TIME_SIGNATURE: time_signature,
             C.TIME_SIGNATURE_GROUPED: time_signature_grouped,
+            C.NUMBER_OF_BEATS: number_of_beats,
             C.TEMPO_GROUPED_1: tempo_grouped_1,
             C.TEMPO_GROUPED_2: tempo_grouped_2,
-            C.NUMBER_OF_BEATS: number_of_beats,
         }
     )
 
 
-def extract_time_signatures(measures: list, score_data: dict):
-    ts_measures = []
+def extract_time_signatures(measures: list, score_data: dict) -> tuple:
+    """
+    Extracts time signatures from a list of measures and returns relevant information.
+
+    Args:
+        measures (list): A list of measures.
+        score_data (dict): A dictionary containing score data.
+
+    Returns:
+        tuple: A tuple containing the time signature, dictionary of measures and their
+        indices, list of time signatures, time signature type, and number of beats.
+
+    The function extracts time signatures from a list of measures and returns
+    relevant information. The function takes two arguments, measures and
+    score_data. measures is a list of measures and score_data is a dictionary
+    containing score data. The function returns a tuple containing the time
+    signature, dictionary of measures and their indices, list of time signatures,
+    time signature type, and number of beats.
+
+    The function ases `'NA'` as the time signature if no time signature is found
+    in the score.
+    """
+
+    ts_measures = {}
     time_signatures = []
     for i, element in enumerate(measures):
-        ts_measures.append(element.measureNumber)
-        if element.measureNumber not in ts_measures[:-1]:
-            if element.timeSignature:
+        if element.measureNumber not in ts_measures:
+            if element.timeSignature is not None:
                 time_signatures.append(element.timeSignature.ratioString)
             else:
                 if len(time_signatures) >= 1:
                     time_signatures.append(time_signatures[-1])
-                elif GLOBAL_TIME_SIGNATURE in score_data:
+                elif hasattr(score_data.get(GLOBAL_TIME_SIGNATURE), 'ratioString'):
                     time_signatures.append(
                         score_data[GLOBAL_TIME_SIGNATURE].ratioString
                     )
                 else:
-                    raise Exception("There was an error when omputing time signatures of the score.")
-                    
+                    time_signatures.append("NA")
+
+            ts_measures[element.measureNumber] = i
         else:
-            time_signatures.append(
-                time_signatures[ts_measures.index(element.measureNumber)]
-            )
+            time_signatures.append(time_signatures[ts_measures[element.measureNumber]])
 
     time_signatures_set = set(time_signatures)
-    time_signature = ",".join(
-        list(sorted(time_signatures_set, key=time_signatures.index))
-    )
-    time_signature_grouped = get_time_signature_type(time_signature.split(",")[0])
-    number_of_beats = get_number_of_beats(time_signature.split(",")[0])
+    time_signature = list(sorted(time_signatures_set, key=time_signatures.index))[0]
+
+    time_signature_grouped = get_time_signature_type(time_signature)
+    number_of_beats = get_number_of_beats(time_signature)
 
     return (
         time_signature,
         ts_measures,
         time_signatures,
         time_signature_grouped,
         number_of_beats,
@@ -143,8 +157,7 @@
         if isinstance(measure, Measure):
             for element in measure:
                 if isinstance(element, TextExpression):
                     if get_tempo_grouped_1(element.content) != "NA":
                         tempo_mark = element.content
             break  # only take into account the first bar!
     return numeric_tempo, tempo_mark
-
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `musif-1.0.1.post1/musif/extract/features/texture/handler.py` & `musif-1.1.0/musif/extract/features/texture/handler.py`

 * *Files identical despite different names*

### Comparing `musif-1.0.1.post1/musif/extract/utils.py` & `musif-1.1.0/musif/extract/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import itertools
-import os
 from typing import Union
 
 import ms3
 import music21 as m21
-from music21.stream.base import Measure
-from musif.logs import pwarn
 import pandas as pd
+from music21.stream.base import Measure
 from pandas import DataFrame
 
 import musif.extract.constants as C
 from musif.cache import isinstance
 from musif.extract.constants import PLAYTHROUGH
+from musif.logs import pwarn
 from musif.musicxml.tempo import get_number_of_beats
 
 file_names = []
 repeat_bracket = False
 
 
 def process_musescore_file(file_path: str, expand_repeats: bool = False) -> DataFrame:
@@ -34,19 +33,25 @@
         Dataframe containing harmonic information
     """
 
     msc3_score = ms3.score.Score(file_path, logger_cfg={"level": "ERROR"})
     harmonic_analysis = msc3_score.mscx.expanded()
     harmonic_analysis.reset_index(inplace=True)
     if expand_repeats:
-        mn = ms3.parse.next2sequence(msc3_score.mscx.measures.set_index("mc").next)
-        mn = pd.Series(mn, name="mc_playthrough")
-        harmonic_analysis = ms3.parse.unfold_repeats(harmonic_analysis, mn)
+        harmonic_analysis = msc3_score.mscx.expanded(unfold=True)
+        harmonic_analysis.reset_index(inplace=True)
+        # unfolded_mc=msc3_score.mscx.measures().set_index("mc").next
+        # mn = next2sequence(unfolded_mc)
+        # mn = ms3.utils.next2sequence(unfolded_mc)
+        # mn = pd.Series(mn, name="mc_playthrough")
+        # harmonic_analysis = ms3.utils.unfold_repeats(harmonic_analysis, mn)
         harmonic_analysis.rename(columns={"mc_playthrough": PLAYTHROUGH}, inplace=True)
     else:
+        harmonic_analysis = msc3_score.mscx.expanded()
+        harmonic_analysis.reset_index(inplace=True)
         if harmonic_analysis.mn[0] == 0:
             harmonic_analysis[PLAYTHROUGH] = harmonic_analysis["mc"]
         else:
             harmonic_analysis[PLAYTHROUGH] = harmonic_analysis["mn"]
     _include_beats_column(harmonic_analysis)
     return harmonic_analysis
 
@@ -576,22 +581,25 @@
         newtype = col[notna].map(type).mode()[0]
         if issubclass(newtype, float):
             #  convert fractions like '1/3' to float
             col[notna] = col[notna].apply(pd.eval)
             col = col.convert_dtypes()
         elif issubclass(newtype, int):
             # convert to string
-            col = col.astype('string')
+            col = col.astype("string")
     return col
 
+
 def extract_global_time_signature(score_data):
     """
     Extracts a global time signature for the score for cases where is not possibel to get measure-by-measure TS
     """
-    global_ts = score_data[C.GLOBAL_TIME_SIGNATURE] = (
+    global_ts = (
         score_data[C.DATA_FILTERED_PARTS][0]
         .getElementsByClass(Measure)[0]
         .timeSignature
     )
     if global_ts is None:
-        pwarn('Global Time Signature could not possible to be extracted!')
-    return global_ts
+        pwarn("Couldn't extract Global Time Sigature!")
+        global_ts = "NA"
+    score_data[C.GLOBAL_TIME_SIGNATURE] = global_ts
+    return global_ts
```

### Comparing `musif-1.0.1.post1/musif/logs.py` & `musif-1.1.0/musif/logs.py`

 * *Files identical despite different names*

### Comparing `musif-1.0.1.post1/musif/musescore/common.py` & `musif-1.1.0/musif/musescore/common.py`

 * *Files identical despite different names*

### Comparing `musif-1.0.1.post1/musif/musicxml/common.py` & `musif-1.1.0/musif/musicxml/common.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from music21.stream.base import Measure, Part, Score, Voice
 from music21.text import assembleLyrics
 from roman import toRoman
 
 from musif.cache import isinstance
 
 
-
 def is_voice(part: Part) -> bool:
     """
     Returns True if the part is a singer part, otherwise returns False
 
     Parameters
     ----------
     part : Part
@@ -23,14 +22,33 @@
 
     instrument = part.getInstrument(returnDefault=False)
     if instrument is None or instrument.instrumentSound is None:
         return False
     return "voice" in instrument.instrumentSound
 
 
+def name_parts(score: Score):
+    """
+    This function assign a name to each part in the score. If a name is already present,
+    we keep it there, otherwise, we create a name of type `missingName#` where # is an
+    incremental number,
+    """
+    i = 0
+    for part in score.parts:
+        increment = False
+        if part.partName is None:
+            part.partName = f"NoName{i}"
+            increment = True
+        if part.partAbbreviation is None:
+            part.partAbbreviation = f"NoName{i}"
+            increment = True
+        if increment:
+            i += 1
+
+
 def split_layers(score: Score, split_keywords: List[str]):
     """
     Function used to split possible layers. Those instruments that include to parts in the same staff
     will be separated in two diferent parts so they can be treated separately.
 
     Parameters
     ----------
@@ -43,15 +61,15 @@
     """
 
     final_parts = []
     for part_index, part in enumerate(score.parts):
         instrument = part.getInstrument(returnDefault=False)
 
         possible_layers = False
-        if instrument.instrumentSound is not None:
+        if instrument is not None and instrument.instrumentSound is not None:
             for keyword in split_keywords:
                 if keyword in instrument.instrumentSound:
                     possible_layers = True
                     break
 
         if possible_layers:
             has_voices = False
@@ -91,17 +109,20 @@
     ----------
     part : Part
       Music21 part to extract the info from.
 
     """
 
     measures = list(part.getElementsByClass(Measure))
-    sounding_measures = [measure for measure in measures if len(measure.notes) > 0]
-    original_notes = [note for measure in measures for note in measure.notes if
-                      isinstance(note, Note)]
+    sounding_measures = [
+        idx for idx, measure in enumerate(measures) if len(measure.notes) > 0
+    ]
+    original_notes = [
+        note for measure in measures for note in measure.notes if isinstance(note, Note)
+    ]
     notes_and_rests = [n for measure in measures for n in measure.notesAndRests]
 
     return original_notes, measures, sounding_measures, notes_and_rests
 
 
 def _separate_info_in_two_parts(score, final_parts, part):
     parts_splitted = part.voicesToParts().elements
```

### Comparing `musif-1.0.1.post1/musif/musicxml/constants.py` & `musif-1.1.0/musif/musicxml/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-MUSICXML_FILE_EXTENSION = ".xml"
-"""Extension of the MusicXML file. Defaults to ".xml"."""
+MUSIC21_FILE_EXTENSIONS = [".xml", ".mxl", ".musicxml"]
+"""Extensions used by music21. Defaults to `[".xml", ".mxl", ".musicxml"]`"""
 
 
 SOUND_TO_ABBREVIATION = {
     "accordion": "acc",
     "alto flute": "afl",
     "alto": "alt",
     "voice": "v",
```

### Comparing `musif-1.0.1.post1/musif/musicxml/key.py` & `musif-1.1.0/musif/musicxml/key.py`

 * *Files identical despite different names*

### Comparing `musif-1.0.1.post1/musif/musicxml/repeat.py` & `musif-1.1.0/musif/musicxml/repeat.py`

 * *Files identical despite different names*

### Comparing `musif-1.0.1.post1/musif/musicxml/scoring.py` & `musif-1.1.0/musif/musicxml/scoring.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,14 +76,15 @@
         part) or _get_part_roman_number_by_position(part, parts)
     other_number = _get_part_normal_number(part)
     part_number = fromRoman(part_roman_number) if part_roman_number else (other_number if other_number else 0)
     sound_abbreviation = abbreviation.split('(')[0]
     return abbreviation + (part_roman_number or ""), sound_abbreviation, part_number
 
 def _get_part_normal_number(part: Part) -> Optional[str]:
+    # this is didone-specific
     if '(' and ')' in part.partAbbreviation:
         return part.partAbbreviation.split('(')[1].split(')')[0]
     return None
 
 def _get_part_roman_number(part: Part) -> Optional[str]:
     for number in ROMAN_NUMERALS_FROM_1_TO_20:
         if part.partAbbreviation.endswith(f". {number}") or part.partName.endswith(
```

### Comparing `musif-1.0.1.post1/musif/musicxml/tempo.py` & `musif-1.1.0/musif/musicxml/tempo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import re
 import xml.etree.ElementTree as ET
 from enum import Enum
 from typing import Optional
 
+import pandas as pd
+
 
 class TempoGroup2(Enum):
     """
     Contains constants refering to grouped tempo on the second level that will be used by the tempo module.
     """
 
     NA = "NA"
@@ -244,27 +246,31 @@
 
 def get_number_of_beats(time_signature: str) -> int:
     """
     Returns the number of beats corresponding to a time signature.
 
     By default, this returns the numerator, with the exceptions when the numerator is
     6, 9, or 12 and when the time signature is C or 3/8. If it is empty, it returns 1.
+    If it is `"NA"`, it returns `pd.NA`.
 
     Parameters
     ----------
         time_signature: str
             Time signature in the form of string separated by '/' to obtain the time
             signature type.
 
     """
+    # we only take the first time signature in case we receive more than one
     time_signature = time_signature.split(",")[0]
     if time_signature == "C":
         return 4
     elif time_signature == "":
         return 1
+    elif time_signature == "NA":
+        return pd.NA
     num, den = time_signature.split("/")
     if num == "3" and den == "8":
         return 1
     elif num == "6":
         return 2
     elif num == "9":
         return 3
@@ -273,15 +279,16 @@
     else:
         return int(num)
         # raise ValueError(f"The {time_signature} is not a known time signature")
 
 
 def extract_numeric_tempo(file_path: str) -> Optional[int]:
     """
-    Finds the numeric tempo in a musixml file by looking at the tempo marking in the xml code.
+    Finds the numeric tempo in a musixml file by looking at the tempo marking in
+    the xml code.
 
     Parameters
     ----------
 
         file_path: str
         Path to xml file to get the tempo from.
```

### Comparing `musif-1.0.1.post1/musif/process/processor.py` & `musif-1.1.0/musif/process/processor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import os
 from pathlib import PurePath
 from typing import Union
-from musif.common.sort import sort_columns
 
 import pandas as pd
 from pandas import DataFrame
 
+from musif.common.sort import sort_columns
 from musif.config import PostProcessConfiguration
+from musif.extract.basic_modules.file_name_generic.constants import ARTIST, TITLE
 from musif.extract.basic_modules.scoring.constants import INSTRUMENTATION
-from musif.extract.basic_modules.file_name_generic.constants import TITLE, ARTIST
-
 from musif.extract.constants import ID, WINDOW_ID
 from musif.extract.features.core.constants import FILE_NAME
 from musif.extract.features.harmony.constants import (
     HARMONY_AVAILABLE,
     KEY_MODULATORY,
     KEY_PREFIX,
 )
@@ -96,15 +95,15 @@
                     info, low_memory=False, sep=",", encoding_errors="replace"
                 )
                 if df.empty:
                     raise FileNotFoundError("The .csv file could not be found.")
                 return df
 
             elif isinstance(info, DataFrame):
-                pinfo("\nProcessing DataFrame...")
+                # pinfo("\nProcessing DataFrame...")
                 return info
             else:
                 perr(
                     "Wrong info type! You must introduce either a DataFrame either the name of a .csv file."
                 )
                 return pd.DataFrame()
 
@@ -120,24 +119,24 @@
         and merges those that are needed according to config.yml file.
 
         Returns
         ------
         Dataframe object
         """
 
-        pinfo("\nPreprocessing data...")
+        pinfo("\nPost-processing data...")
         self.data.dropna(axis=1, how="all", inplace=True)
         if self._post_config.delete_files_without_harmony:
             self.delete_files_without_harmony()
 
         if self._post_config.separate_intrumentation_column:
             pinfo('\nSeparating "Instrumentation" column...')
             self.separate_instrumentation_column()
 
-        self.delete_undesired_columns()
+        self.delete_undesired()
 
         if self._post_config.grouped_analysis:
             self.group_columns()
 
         self._final_data_processing()
         return self
 
@@ -182,16 +181,16 @@
 
         self.data[[i for i in self.data if PRESENCE + "_" in i]] = (
             self.data[[i for i in self.data if PRESENCE + "_" in i]]
             .fillna(0)
             .astype(int)
         )
 
-    def delete_undesired_columns(self, **kwargs) -> None:
-        """Deletes not necessary columns for statistical analysis.
+    def delete_undesired(self, **kwargs) -> None:
+        """Deletes not necessary columns and rows for statistical analysis.
 
         If keyword arguments are passed in, they overwrite those found
         into configurationg file
 
         Parameters
         ----------
         **kwargs : str, optional
@@ -202,32 +201,44 @@
         ------
         KeyError
             If any of the columns required to delete is not found
             in the original DataFrame.
         """
         config_data = self._post_config.__dict__
         config_data.update(kwargs)  # Override values
-        try:
-            _delete_columns(self.data, config_data)
-        except KeyError:
-            perr("Some columns are already not present in the Dataframe")
+
+        # deleting columns that are completely nans
+        idx = self.data.isna().all()
+        to_delete = self.data.columns[idx].to_list()
+        self.data.drop(columns=to_delete, inplace=True)
+
+        # deleting rows
+        th = config_data["max_nan_rows"] or 1.0
+        idx = self.data.isna().sum(axis=1) / self.data.shape[1] > th
+        to_delete = self.data.index[idx]
+        self.data.drop(index=to_delete, inplace=True)
+
+        # delete cols
+        _delete_columns(self.data, config_data)
 
     def replace_nans(self) -> None:
-        pinfo("Replacing NaN values in selected columns")
+        # pinfo("Replacing NaN values in selected columns")
         cols = []
         for col in self.data.columns:
             if any(
                 substring.lower() in col.lower()
                 for substring in tuple(self._post_config.replace_nans)
             ):
                 cols.append(col)
-        cols = self.data[cols].select_dtypes(include='number').columns
+        cols = self.data[cols].select_dtypes(include="number").columns
         self.data[cols] = self.data[cols].fillna(0)
 
-    def save(self, dest_path: Union[str, PurePath], ext=".csv", ft="csv", **kwargs) -> None:
+    def save(
+        self, dest_path: Union[str, PurePath], ext=".csv", ft="csv", **kwargs
+    ) -> None:
         """Saves current information into a file given the name of dest_path
 
         To load one of those file, remember to set the index to
         `musif.extract.constant.ID`, and, if windows are used, to
         `musif.extract.constant.WINDOW_ID`:
 
         ```python
@@ -246,16 +257,16 @@
             Type of file for saving. The filetype must be supported by `pandas`, e.g.
             `to_csv`, `to_feather`, `to_parquet`, etc. Default: `csv`
         """
 
         pinfo(f"Writing data to {dest_path}_*{ext}")
         ft = "to_" + ft
         dest_path = str(dest_path)
-        if ft == 'csv':
-            kwargs['index'] = False
+        if ft == "csv":
+            kwargs["index"] = False
         getattr(self.data, ft)(dest_path + "_alldata" + ext, **kwargs)
 
     def _group_keys_modulatory(self) -> None:
         self.data.update(
             self.data[
                 [i for i in self.data.columns if KEY_PREFIX + KEY_MODULATORY in i]
             ].fillna(0)
@@ -291,12 +302,12 @@
         )
 
     def _final_data_processing(self) -> None:
         self.data.sort_values([ID, WINDOW_ID], inplace=True)
         self.replace_nans()
         self.data = self.data.reindex(sorted(self.data.columns), axis=1)
         if TITLE and ARTIST in self.data.columns:
-            priority_columns =[FILE_NAME, TITLE, ARTIST]
+            priority_columns = [FILE_NAME, TITLE, ARTIST]
         else:
-            priority_columns=[] 
+            priority_columns = []
         self.data = sort_columns(self.data, [ID, WINDOW_ID] + priority_columns)
         self.data.drop("index", axis=1, inplace=True, errors="ignore")
```

### Comparing `musif-1.0.1.post1/musif/process/utils.py` & `musif-1.1.0/musif/process/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import re
 from logging.config import dictConfig
 from typing import List
-from musif.extract.features.prefix import get_part_prefix
 
 import pandas as pd
 from pandas import DataFrame
 
 from musif.config import (
     ENDSWITH,
     INSTRUMENTS_TO_DELETE,
@@ -19,14 +18,15 @@
 from musif.extract.features.harmony.constants import (
     KEY_MODULATORY,
     KEY_PERCENTAGE,
     KEY_PREFIX,
     CHORD_prefix,
 )
 from musif.extract.features.melody.constants import TRIMMED_INTERVALLIC_MEAN
+from musif.extract.features.prefix import get_part_prefix
 from musif.extract.features.scale.constants import DEGREE_PREFIX
 from musif.logs import pinfo
 
 from .constants import voices_list_prefixes
 
 
 def replace_nans(df):
@@ -73,27 +73,29 @@
     pinfo(str(novoices_counter))
     # pinfo(f"\nTotal files skipped by duetos/trietos: {len(duetos_counter)}")
     # pinfo(str(duetos_counter))
     pinfo(f"\nFinal shape of the DataFrame: {df.shape[0]} rows, {df.shape[1]} features")
 
 
 def _delete_columns(data: DataFrame, config: dictConfig) -> None:
-    pinfo("\nDeleting not useful columns...")
+    # pinfo("\nDeleting not useful columns...")
     to_delete = []
-    instruments_to_keep = [get_part_prefix(i) for i in config[INSTRUMENTS_TO_KEEP]] 
+    instruments_to_keep = [get_part_prefix(i) for i in config[INSTRUMENTS_TO_KEEP]]
     for inst in config[INSTRUMENTS_TO_DELETE]:
         # for i in data.columns:
         #     if "Part" + inst + "_" in i
-        part_prefix = "Part" + inst #+ "_"
+        part_prefix = "Part" + inst  # + "_"
         for col in data.columns:
-                if part_prefix in col and all(inst not in col for inst in instruments_to_keep):
-                    pass
-                    to_delete.append(col)
-                else:
-                    pass
+            if part_prefix in col and all(
+                inst not in col for inst in instruments_to_keep
+            ):
+                pass
+                to_delete.append(col)
+            else:
+                pass
         # to_delete += [i for i in data.columns if part_prefix in i and instrument not in i for instrument in instruments_to_keep]
 
     to_delete += [i for i in data.columns if i.endswith(tuple(config[ENDSWITH]))]
     to_delete += [i for i in data.columns if i.startswith(tuple(config[STARTSWITH]))]
     to_delete += [
         col
         for col in data.columns
@@ -111,14 +113,20 @@
     # Remove empty voices
     to_delete += [
         col
         for col in data.columns
         if col.startswith(tuple(voices_list_prefixes))
         and all(data[col].isnull().values)
     ]
+
+    # removing columns containing nans
+    th = config["max_nan_columns"] or 0.0
+    idx = data.isna().sum(axis=0) / data.shape[0] > th
+    to_delete += data.columns[idx].to_list()
+
     data.drop(columns=to_delete, inplace=True, errors="ignore")
 
 
 def join_keys(df: DataFrame) -> None:
     key_SD = [
         i
         for i in [
```

### Comparing `musif-1.0.1.post1/pyproject.toml` & `musif-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     "roman>=3.3",
     "joblib>=1.0.0",
     "scipy>=1.6.0",
     "music21>=8,<9",
     "deepdiff>=6.2.1",
 ]
 name = "musif"
-version = "1.0.1-1"
+version = "1.1.0"
 description = "Music feature extraction library from the DIDONE project"
 authors = [
     { name = "Didone Project", email = "didone@iccmu.es" },
 ]
 requires-python = ">=3.10"
 readme = "README.md"
```

