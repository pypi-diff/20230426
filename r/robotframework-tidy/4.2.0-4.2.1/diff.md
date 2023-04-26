# Comparing `tmp/robotframework-tidy-4.2.0.tar.gz` & `tmp/robotframework-tidy-4.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-tidy-4.2.0.tar", last modified: Wed Apr 19 08:55:50 2023, max compression
+gzip compressed data, was "robotframework-tidy-4.2.1.tar", last modified: Wed Apr 26 08:27:57 2023, max compression
```

## Comparing `robotframework-tidy-4.2.0.tar` & `robotframework-tidy-4.2.1.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:55:50.517036 robotframework-tidy-4.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-04-19 08:55:50.517036 robotframework-tidy-4.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:55:50.501036 robotframework-tidy-4.2.0/robotframework_tidy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-04-19 08:55:50.000000 robotframework-tidy-4.2.0/robotframework_tidy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-04-19 08:55:50.000000 robotframework-tidy-4.2.0/robotframework_tidy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 08:55:50.000000 robotframework-tidy-4.2.0/robotframework_tidy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-19 08:55:50.000000 robotframework-tidy-4.2.0/robotframework_tidy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-19 08:55:50.000000 robotframework-tidy-4.2.0/robotframework_tidy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-19 08:55:50.000000 robotframework-tidy-4.2.0/robotframework_tidy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:55:50.505035 robotframework-tidy-4.2.0/robotidy/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:55:50.509036 robotframework-tidy-4.2.0/robotidy/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-19 08:55:50.000000 robotframework-tidy-4.2.0/robotidy/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-19 08:55:50.000000 robotframework-tidy-4.2.0/robotidy/__pycache__/version.cpython-311.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/app.py
--rw-r--r--   0 runner    (1001) docker     (123)    14328 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    15343 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     6706 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/disablers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/files.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/rich_console.py
--rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/skip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:55:50.517036 robotframework-tidy-4.2.0/robotidy/transformers/
--rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/transformers/AddMissingEnd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/transformers/AlignKeywordsSection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/transformers/AlignSettingsSection.py
--rw-r--r--   0 runner    (1001) docker     (123)     7483 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/transformers/AlignTemplatedTestCases.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/transformers/AlignTestCasesSection.py
--rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/transformers/AlignVariablesSection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/transformers/DiscardEmptySections.py
--rw-r--r--   0 runner    (1001) docker     (123)     6881 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/transformers/GenerateDocumentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9875 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/transformers/IndentNestedKeywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    12649 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/transformers/InlineIf.py
--rw-r--r--   0 runner    (1001) docker     (123)     7673 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/transformers/MergeAndOrderSections.py
--rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/transformers/NormalizeAssignments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/transformers/NormalizeComments.py
--rw-r--r--   0 runner    (1001) docker     (123)     5755 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/transformers/NormalizeNewLines.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/transformers/NormalizeSectionHeaderName.py
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/transformers/NormalizeSeparators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/transformers/NormalizeSettingName.py
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/transformers/NormalizeTags.py
--rw-r--r--   0 runner    (1001) docker     (123)     8471 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/transformers/OrderSettings.py
--rw-r--r--   0 runner    (1001) docker     (123)     8834 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/transformers/OrderSettingsSection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/transformers/OrderTags.py
--rw-r--r--   0 runner    (1001) docker     (123)     4175 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/transformers/RemoveEmptySettings.py
--rw-r--r--   0 runner    (1001) docker     (123)     8421 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/transformers/RenameKeywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/transformers/RenameTestCases.py
--rw-r--r--   0 runner    (1001) docker     (123)    17838 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/transformers/RenameVariables.py
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/transformers/ReplaceBreakContinue.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/transformers/ReplaceEmptyValues.py
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/transformers/ReplaceReturns.py
--rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/transformers/ReplaceRunKeywordIf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/transformers/SmartSortKeywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    12317 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/transformers/SplitTooLongLine.py
--rw-r--r--   0 runner    (1001) docker     (123)    10020 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/transformers/Translate.py
--rw-r--r--   0 runner    (1001) docker     (123)    19687 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23065 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/transformers/aligners_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/transformers/run_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    13625 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 08:55:50.517036 robotframework-tidy-4.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:27:57.109992 robotframework-tidy-4.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-04-26 08:27:57.109992 robotframework-tidy-4.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:27:57.101992 robotframework-tidy-4.2.1/robotframework_tidy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-04-26 08:27:57.000000 robotframework-tidy-4.2.1/robotframework_tidy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-04-26 08:27:57.000000 robotframework-tidy-4.2.1/robotframework_tidy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 08:27:57.000000 robotframework-tidy-4.2.1/robotframework_tidy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-26 08:27:57.000000 robotframework-tidy-4.2.1/robotframework_tidy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-26 08:27:57.000000 robotframework-tidy-4.2.1/robotframework_tidy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-26 08:27:57.000000 robotframework-tidy-4.2.1/robotframework_tidy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:27:57.105992 robotframework-tidy-4.2.1/robotidy/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:27:57.105992 robotframework-tidy-4.2.1/robotidy/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-26 08:27:56.000000 robotframework-tidy-4.2.1/robotidy/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-26 08:27:56.000000 robotframework-tidy-4.2.1/robotidy/__pycache__/version.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14328 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15395 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6706 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/disablers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/rich_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/skip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:27:57.109992 robotframework-tidy-4.2.1/robotidy/transformers/
+-rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/transformers/AddMissingEnd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/transformers/AlignKeywordsSection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/transformers/AlignSettingsSection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7483 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/transformers/AlignTemplatedTestCases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/transformers/AlignTestCasesSection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/transformers/AlignVariablesSection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/transformers/DiscardEmptySections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6881 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/transformers/GenerateDocumentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9875 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/transformers/IndentNestedKeywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12649 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/transformers/InlineIf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7673 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/transformers/MergeAndOrderSections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/transformers/NormalizeAssignments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/transformers/NormalizeComments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5755 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/transformers/NormalizeNewLines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/transformers/NormalizeSectionHeaderName.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/transformers/NormalizeSeparators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/transformers/NormalizeSettingName.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/transformers/NormalizeTags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8471 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/transformers/OrderSettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8834 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/transformers/OrderSettingsSection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/transformers/OrderTags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4175 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/transformers/RemoveEmptySettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8421 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/transformers/RenameKeywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/transformers/RenameTestCases.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17838 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/transformers/RenameVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/transformers/ReplaceBreakContinue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/transformers/ReplaceEmptyValues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/transformers/ReplaceReturns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/transformers/ReplaceRunKeywordIf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/transformers/SmartSortKeywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12317 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/transformers/SplitTooLongLine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10020 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/transformers/Translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19687 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23065 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/transformers/aligners_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/transformers/run_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13625 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/robotidy/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 08:27:57.109992 robotframework-tidy-4.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-04-26 08:27:39.000000 robotframework-tidy-4.2.1/setup.py
```

### Comparing `robotframework-tidy-4.2.0/LICENSE` & `robotframework-tidy-4.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.0/PKG-INFO` & `robotframework-tidy-4.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-tidy
-Version: 4.2.0
+Version: 4.2.1
 Summary: Code autoformatter for Robot Framework
 Home-page: https://github.com/MarketSquare/robotframework-tidy
 Author: MarketSquare - Robot Framework community
 Author-email: bartek.hirsz@gmail.com
 License: Apache License 2.0
 Keywords: robotframework
 Platform: any
```

### Comparing `robotframework-tidy-4.2.0/README.md` & `robotframework-tidy-4.2.1/README.md`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.0/robotframework_tidy.egg-info/PKG-INFO` & `robotframework-tidy-4.2.1/robotframework_tidy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-tidy
-Version: 4.2.0
+Version: 4.2.1
 Summary: Code autoformatter for Robot Framework
 Home-page: https://github.com/MarketSquare/robotframework-tidy
 Author: MarketSquare - Robot Framework community
 Author-email: bartek.hirsz@gmail.com
 License: Apache License 2.0
 Keywords: robotframework
 Platform: any
```

### Comparing `robotframework-tidy-4.2.0/robotframework_tidy.egg-info/SOURCES.txt` & `robotframework-tidy-4.2.1/robotframework_tidy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.0/robotidy/api.py` & `robotframework-tidy-4.2.1/robotidy/api.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.0/robotidy/app.py` & `robotframework-tidy-4.2.1/robotidy/app.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.0/robotidy/cli.py` & `robotframework-tidy-4.2.1/robotidy/cli.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.0/robotidy/config.py` & `robotframework-tidy-4.2.1/robotidy/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -246,14 +246,16 @@
 
         If the sources tuple is empty, look for most common configuration file and load sources from there.
         """
         if sources:
             return sources
         src = Path(".").resolve()
         config_path = files.find_source_config_file(src, self.default.ignore_git_dir)
+        if not config_path:
+            return None
         config = files.read_pyproject_config(config_path)
         if not config or "src" not in config:
             return None
         raw_config = self.default.from_config_file(config, config_path)
         loaded_config = Config.from_raw_config(raw_config)
         self.loaded_configs[str(loaded_config.config_directory)] = loaded_config
         return tuple(config["src"])
```

### Comparing `robotframework-tidy-4.2.0/robotidy/decorators.py` & `robotframework-tidy-4.2.1/robotidy/decorators.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.0/robotidy/disablers.py` & `robotframework-tidy-4.2.1/robotidy/disablers.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.0/robotidy/exceptions.py` & `robotframework-tidy-4.2.1/robotidy/exceptions.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.0/robotidy/files.py` & `robotframework-tidy-4.2.1/robotidy/files.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.0/robotidy/skip.py` & `robotframework-tidy-4.2.1/robotidy/skip.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.0/robotidy/transformers/AddMissingEnd.py` & `robotframework-tidy-4.2.1/robotidy/transformers/AddMissingEnd.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.0/robotidy/transformers/AlignKeywordsSection.py` & `robotframework-tidy-4.2.1/robotidy/transformers/AlignKeywordsSection.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.0/robotidy/transformers/AlignSettingsSection.py` & `robotframework-tidy-4.2.1/robotidy/transformers/AlignSettingsSection.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.0/robotidy/transformers/AlignTemplatedTestCases.py` & `robotframework-tidy-4.2.1/robotidy/transformers/AlignTemplatedTestCases.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.0/robotidy/transformers/AlignTestCasesSection.py` & `robotframework-tidy-4.2.1/robotidy/transformers/AlignTestCasesSection.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.0/robotidy/transformers/AlignVariablesSection.py` & `robotframework-tidy-4.2.1/robotidy/transformers/AlignVariablesSection.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.0/robotidy/transformers/DiscardEmptySections.py` & `robotframework-tidy-4.2.1/robotidy/transformers/DiscardEmptySections.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.0/robotidy/transformers/GenerateDocumentation.py` & `robotframework-tidy-4.2.1/robotidy/transformers/GenerateDocumentation.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.0/robotidy/transformers/IndentNestedKeywords.py` & `robotframework-tidy-4.2.1/robotidy/transformers/IndentNestedKeywords.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.0/robotidy/transformers/InlineIf.py` & `robotframework-tidy-4.2.1/robotidy/transformers/InlineIf.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.0/robotidy/transformers/MergeAndOrderSections.py` & `robotframework-tidy-4.2.1/robotidy/transformers/MergeAndOrderSections.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.0/robotidy/transformers/NormalizeAssignments.py` & `robotframework-tidy-4.2.1/robotidy/transformers/NormalizeAssignments.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.0/robotidy/transformers/NormalizeComments.py` & `robotframework-tidy-4.2.1/robotidy/transformers/NormalizeComments.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.0/robotidy/transformers/NormalizeNewLines.py` & `robotframework-tidy-4.2.1/robotidy/transformers/NormalizeNewLines.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.0/robotidy/transformers/NormalizeSectionHeaderName.py` & `robotframework-tidy-4.2.1/robotidy/transformers/NormalizeSectionHeaderName.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.0/robotidy/transformers/NormalizeSeparators.py` & `robotframework-tidy-4.2.1/robotidy/transformers/NormalizeSeparators.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.0/robotidy/transformers/NormalizeSettingName.py` & `robotframework-tidy-4.2.1/robotidy/transformers/NormalizeSettingName.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.0/robotidy/transformers/NormalizeTags.py` & `robotframework-tidy-4.2.1/robotidy/transformers/NormalizeTags.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.0/robotidy/transformers/OrderSettings.py` & `robotframework-tidy-4.2.1/robotidy/transformers/OrderSettings.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.0/robotidy/transformers/OrderSettingsSection.py` & `robotframework-tidy-4.2.1/robotidy/transformers/OrderSettingsSection.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.0/robotidy/transformers/OrderTags.py` & `robotframework-tidy-4.2.1/robotidy/transformers/OrderTags.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.0/robotidy/transformers/RemoveEmptySettings.py` & `robotframework-tidy-4.2.1/robotidy/transformers/RemoveEmptySettings.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.0/robotidy/transformers/RenameKeywords.py` & `robotframework-tidy-4.2.1/robotidy/transformers/RenameKeywords.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.0/robotidy/transformers/RenameTestCases.py` & `robotframework-tidy-4.2.1/robotidy/transformers/RenameTestCases.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.0/robotidy/transformers/RenameVariables.py` & `robotframework-tidy-4.2.1/robotidy/transformers/RenameVariables.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.0/robotidy/transformers/ReplaceBreakContinue.py` & `robotframework-tidy-4.2.1/robotidy/transformers/ReplaceBreakContinue.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.0/robotidy/transformers/ReplaceEmptyValues.py` & `robotframework-tidy-4.2.1/robotidy/transformers/ReplaceEmptyValues.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.0/robotidy/transformers/ReplaceReturns.py` & `robotframework-tidy-4.2.1/robotidy/transformers/ReplaceReturns.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.0/robotidy/transformers/ReplaceRunKeywordIf.py` & `robotframework-tidy-4.2.1/robotidy/transformers/ReplaceRunKeywordIf.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.0/robotidy/transformers/SmartSortKeywords.py` & `robotframework-tidy-4.2.1/robotidy/transformers/SmartSortKeywords.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.0/robotidy/transformers/SplitTooLongLine.py` & `robotframework-tidy-4.2.1/robotidy/transformers/SplitTooLongLine.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.0/robotidy/transformers/Translate.py` & `robotframework-tidy-4.2.1/robotidy/transformers/Translate.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.0/robotidy/transformers/__init__.py` & `robotframework-tidy-4.2.1/robotidy/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.0/robotidy/transformers/aligners_core.py` & `robotframework-tidy-4.2.1/robotidy/transformers/aligners_core.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.0/robotidy/transformers/run_keywords.py` & `robotframework-tidy-4.2.1/robotidy/transformers/run_keywords.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.0/robotidy/utils.py` & `robotframework-tidy-4.2.1/robotidy/utils.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.2.0/setup.py` & `robotframework-tidy-4.2.1/setup.py`

 * *Files identical despite different names*

