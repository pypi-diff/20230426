# Comparing `tmp/Quid-2.3.2.tar.gz` & `tmp/Quid-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Quid-2.3.2.tar", last modified: Sun Apr  2 11:25:31 2023, max compression
+gzip compressed data, was "Quid-2.4.0.tar", last modified: Wed Apr 26 11:35:57 2023, max compression
```

## Comparing `Quid-2.3.2.tar` & `Quid-2.4.0.tar`

### file list

```diff
@@ -1,57 +1,59 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 11:25:31.916206 Quid-2.3.2/
--rw-rw-rw-   0 root         (0) root         (0)    11347 2023-04-02 11:23:42.000000 Quid-2.3.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)    13106 2023-04-02 11:25:31.916206 Quid-2.3.2/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 11:25:31.912206 Quid-2.3.2/Quid.egg-info/
--rw-r--r--   0 root         (0) root         (0)    13106 2023-04-02 11:25:31.000000 Quid-2.3.2/Quid.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1227 2023-04-02 11:25:31.000000 Quid-2.3.2/Quid.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-02 11:25:31.000000 Quid-2.3.2/Quid.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       47 2023-04-02 11:25:31.000000 Quid-2.3.2/Quid.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       63 2023-04-02 11:25:31.000000 Quid-2.3.2/Quid.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-04-02 11:25:31.000000 Quid-2.3.2/Quid.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)    12374 2023-04-02 11:23:42.000000 Quid-2.3.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)      103 2023-04-02 11:23:42.000000 Quid-2.3.2/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 11:25:31.912206 Quid-2.3.2/quid/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-02 11:25:14.000000 Quid-2.3.2/quid/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 11:25:31.912206 Quid-2.3.2/quid/cli/
--rw-rw-rw-   0 root         (0) root         (0)    28050 2023-04-02 11:23:42.000000 Quid-2.3.2/quid/cli/QuidCLI.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-02 11:25:14.000000 Quid-2.3.2/quid/cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 11:25:31.916206 Quid-2.3.2/quid/core/
--rw-rw-rw-   0 root         (0) root         (0)      166 2023-04-02 11:23:42.000000 Quid-2.3.2/quid/core/BestMatch.py
--rw-rw-rw-   0 root         (0) root         (0)      208 2023-04-02 11:23:42.000000 Quid-2.3.2/quid/core/InternalMatch.py
--rw-rw-rw-   0 root         (0) root         (0)      442 2023-04-02 11:23:42.000000 Quid-2.3.2/quid/core/InternalMatchSpan.py
--rw-rw-rw-   0 root         (0) root         (0)    17263 2023-04-02 11:23:42.000000 Quid-2.3.2/quid/core/Quid.py
--rw-rw-rw-   0 root         (0) root         (0)    17822 2023-04-02 11:23:42.000000 Quid-2.3.2/quid/core/QuidMatcher.py
--rw-rw-rw-   0 root         (0) root         (0)    14058 2023-04-02 11:23:42.000000 Quid-2.3.2/quid/core/QuidMerger.py
--rw-rw-rw-   0 root         (0) root         (0)      101 2023-04-02 11:23:42.000000 Quid-2.3.2/quid/core/Text.py
--rw-rw-rw-   0 root         (0) root         (0)      110 2023-04-02 11:23:42.000000 Quid-2.3.2/quid/core/Token.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-02 11:25:14.000000 Quid-2.3.2/quid/core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 11:25:31.916206 Quid-2.3.2/quid/helper/
--rw-rw-rw-   0 root         (0) root         (0)     1736 2023-04-02 11:23:42.000000 Quid-2.3.2/quid/helper/Decoder.py
--rw-rw-rw-   0 root         (0) root         (0)     1891 2023-04-02 11:23:42.000000 Quid-2.3.2/quid/helper/Loader.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-02 11:25:14.000000 Quid-2.3.2/quid/helper/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 11:25:31.916206 Quid-2.3.2/quid/match/
--rw-rw-rw-   0 root         (0) root         (0)      157 2023-04-02 11:23:42.000000 Quid-2.3.2/quid/match/Match.py
--rw-rw-rw-   0 root         (0) root         (0)      111 2023-04-02 11:23:42.000000 Quid-2.3.2/quid/match/MatchSpan.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-02 11:25:14.000000 Quid-2.3.2/quid/match/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 11:25:31.916206 Quid-2.3.2/quid/passager/
--rw-rw-rw-   0 root         (0) root         (0)      536 2023-04-02 11:23:42.000000 Quid-2.3.2/quid/passager/AnalyzedWork.py
--rw-rw-rw-   0 root         (0) root         (0)      669 2023-04-02 11:23:42.000000 Quid-2.3.2/quid/passager/CitationSource.py
--rw-rw-rw-   0 root         (0) root         (0)      261 2023-04-02 11:23:42.000000 Quid-2.3.2/quid/passager/CitationSourceLink.py
--rw-rw-rw-   0 root         (0) root         (0)       91 2023-04-02 11:23:42.000000 Quid-2.3.2/quid/passager/Location.py
--rw-rw-rw-   0 root         (0) root         (0)    28856 2023-04-02 11:23:42.000000 Quid-2.3.2/quid/passager/Passager.py
--rw-rw-rw-   0 root         (0) root         (0)      538 2023-04-02 11:23:42.000000 Quid-2.3.2/quid/passager/SourceSegment.py
--rw-rw-rw-   0 root         (0) root         (0)      410 2023-04-02 11:23:42.000000 Quid-2.3.2/quid/passager/TargetLocation.py
--rw-rw-rw-   0 root         (0) root         (0)      503 2023-04-02 11:23:42.000000 Quid-2.3.2/quid/passager/TargetLocationSelection.py
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-04-02 11:23:42.000000 Quid-2.3.2/quid/passager/TargetMatch.py
--rw-rw-rw-   0 root         (0) root         (0)      524 2023-04-02 11:23:42.000000 Quid-2.3.2/quid/passager/TargetText.py
--rw-rw-rw-   0 root         (0) root         (0)      186 2023-04-02 11:23:42.000000 Quid-2.3.2/quid/passager/TargetTextLocationLink.py
--rw-rw-rw-   0 root         (0) root         (0)      219 2023-04-02 11:23:42.000000 Quid-2.3.2/quid/passager/TextWithMatches.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-02 11:25:14.000000 Quid-2.3.2/quid/passager/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 11:25:31.916206 Quid-2.3.2/quid/visualization/
--rw-rw-rw-   0 root         (0) root         (0)      138 2023-04-02 11:23:42.000000 Quid-2.3.2/quid/visualization/Info.py
--rw-rw-rw-   0 root         (0) root         (0)       97 2023-04-02 11:23:42.000000 Quid-2.3.2/quid/visualization/TargetHtml.py
--rw-rw-rw-   0 root         (0) root         (0)      171 2023-04-02 11:23:42.000000 Quid-2.3.2/quid/visualization/TargetTextWithContent.py
--rw-rw-rw-   0 root         (0) root         (0)      270 2023-04-02 11:23:42.000000 Quid-2.3.2/quid/visualization/Visualization.py
--rw-rw-rw-   0 root         (0) root         (0)     9081 2023-04-02 11:23:42.000000 Quid-2.3.2/quid/visualization/Visualizer.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-02 11:25:14.000000 Quid-2.3.2/quid/visualization/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1045 2023-04-02 11:25:31.920206 Quid-2.3.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 11:35:57.016539 Quid-2.4.0/
+-rw-rw-rw-   0 root         (0) root         (0)    11347 2023-04-26 11:32:23.000000 Quid-2.4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    13106 2023-04-26 11:35:57.016539 Quid-2.4.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 11:35:57.008539 Quid-2.4.0/Quid.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    13106 2023-04-26 11:35:56.000000 Quid-2.4.0/Quid.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1289 2023-04-26 11:35:57.000000 Quid-2.4.0/Quid.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 11:35:56.000000 Quid-2.4.0/Quid.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       47 2023-04-26 11:35:56.000000 Quid-2.4.0/Quid.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2023-04-26 11:35:56.000000 Quid-2.4.0/Quid.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-04-26 11:35:56.000000 Quid-2.4.0/Quid.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)    12374 2023-04-26 11:32:23.000000 Quid-2.4.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      103 2023-04-26 11:32:23.000000 Quid-2.4.0/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 11:35:57.008539 Quid-2.4.0/quid/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-26 11:35:30.000000 Quid-2.4.0/quid/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 11:35:57.008539 Quid-2.4.0/quid/cli/
+-rw-rw-rw-   0 root         (0) root         (0)    28626 2023-04-26 11:32:23.000000 Quid-2.4.0/quid/cli/QuidCLI.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-26 11:35:30.000000 Quid-2.4.0/quid/cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 11:35:57.012539 Quid-2.4.0/quid/core/
+-rw-rw-rw-   0 root         (0) root         (0)      166 2023-04-26 11:32:23.000000 Quid-2.4.0/quid/core/BestMatch.py
+-rw-rw-rw-   0 root         (0) root         (0)      208 2023-04-26 11:32:23.000000 Quid-2.4.0/quid/core/InternalMatch.py
+-rw-rw-rw-   0 root         (0) root         (0)      442 2023-04-26 11:32:23.000000 Quid-2.4.0/quid/core/InternalMatchSpan.py
+-rw-rw-rw-   0 root         (0) root         (0)    17263 2023-04-26 11:32:23.000000 Quid-2.4.0/quid/core/Quid.py
+-rw-rw-rw-   0 root         (0) root         (0)    17822 2023-04-26 11:32:23.000000 Quid-2.4.0/quid/core/QuidMatcher.py
+-rw-rw-rw-   0 root         (0) root         (0)    14310 2023-04-26 11:32:23.000000 Quid-2.4.0/quid/core/QuidMerger.py
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-04-26 11:32:23.000000 Quid-2.4.0/quid/core/Text.py
+-rw-rw-rw-   0 root         (0) root         (0)      110 2023-04-26 11:32:23.000000 Quid-2.4.0/quid/core/Token.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-26 11:35:30.000000 Quid-2.4.0/quid/core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 11:35:57.012539 Quid-2.4.0/quid/helper/
+-rw-rw-rw-   0 root         (0) root         (0)     1736 2023-04-26 11:32:23.000000 Quid-2.4.0/quid/helper/Decoder.py
+-rw-rw-rw-   0 root         (0) root         (0)     1891 2023-04-26 11:32:23.000000 Quid-2.4.0/quid/helper/Loader.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-26 11:35:30.000000 Quid-2.4.0/quid/helper/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 11:35:57.012539 Quid-2.4.0/quid/match/
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-04-26 11:32:23.000000 Quid-2.4.0/quid/match/Match.py
+-rw-rw-rw-   0 root         (0) root         (0)      111 2023-04-26 11:32:23.000000 Quid-2.4.0/quid/match/MatchSpan.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-26 11:35:30.000000 Quid-2.4.0/quid/match/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 11:35:57.016539 Quid-2.4.0/quid/passager/
+-rw-rw-rw-   0 root         (0) root         (0)      536 2023-04-26 11:32:23.000000 Quid-2.4.0/quid/passager/AnalyzedWork.py
+-rw-rw-rw-   0 root         (0) root         (0)      669 2023-04-26 11:32:23.000000 Quid-2.4.0/quid/passager/CitationSource.py
+-rw-rw-rw-   0 root         (0) root         (0)      261 2023-04-26 11:32:23.000000 Quid-2.4.0/quid/passager/CitationSourceLink.py
+-rw-rw-rw-   0 root         (0) root         (0)       91 2023-04-26 11:32:23.000000 Quid-2.4.0/quid/passager/Location.py
+-rw-rw-rw-   0 root         (0) root         (0)    28856 2023-04-26 11:32:23.000000 Quid-2.4.0/quid/passager/Passager.py
+-rw-rw-rw-   0 root         (0) root         (0)      538 2023-04-26 11:32:23.000000 Quid-2.4.0/quid/passager/SourceSegment.py
+-rw-rw-rw-   0 root         (0) root         (0)      410 2023-04-26 11:32:23.000000 Quid-2.4.0/quid/passager/TargetLocation.py
+-rw-rw-rw-   0 root         (0) root         (0)      503 2023-04-26 11:32:23.000000 Quid-2.4.0/quid/passager/TargetLocationSelection.py
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-04-26 11:32:23.000000 Quid-2.4.0/quid/passager/TargetMatch.py
+-rw-rw-rw-   0 root         (0) root         (0)      524 2023-04-26 11:32:23.000000 Quid-2.4.0/quid/passager/TargetText.py
+-rw-rw-rw-   0 root         (0) root         (0)      186 2023-04-26 11:32:23.000000 Quid-2.4.0/quid/passager/TargetTextLocationLink.py
+-rw-rw-rw-   0 root         (0) root         (0)      219 2023-04-26 11:32:23.000000 Quid-2.4.0/quid/passager/TextWithMatches.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-26 11:35:30.000000 Quid-2.4.0/quid/passager/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 11:35:57.016539 Quid-2.4.0/quid/visualization/
+-rw-rw-rw-   0 root         (0) root         (0)      138 2023-04-26 11:32:23.000000 Quid-2.4.0/quid/visualization/Info.py
+-rw-rw-rw-   0 root         (0) root         (0)      104 2023-04-26 11:32:23.000000 Quid-2.4.0/quid/visualization/Markup.py
+-rw-rw-rw-   0 root         (0) root         (0)      128 2023-04-26 11:32:23.000000 Quid-2.4.0/quid/visualization/MarkupSpan.py
+-rw-rw-rw-   0 root         (0) root         (0)       97 2023-04-26 11:32:23.000000 Quid-2.4.0/quid/visualization/TargetHtml.py
+-rw-rw-rw-   0 root         (0) root         (0)      171 2023-04-26 11:32:23.000000 Quid-2.4.0/quid/visualization/TargetTextWithContent.py
+-rw-rw-rw-   0 root         (0) root         (0)      270 2023-04-26 11:32:23.000000 Quid-2.4.0/quid/visualization/Visualization.py
+-rw-rw-rw-   0 root         (0) root         (0)    12304 2023-04-26 11:32:23.000000 Quid-2.4.0/quid/visualization/Visualizer.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-26 11:35:30.000000 Quid-2.4.0/quid/visualization/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1045 2023-04-26 11:35:57.020539 Quid-2.4.0/setup.cfg
```

### Comparing `Quid-2.3.2/LICENSE` & `Quid-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Quid-2.3.2/PKG-INFO` & `Quid-2.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Quid
-Version: 2.3.2
+Version: 2.4.0
 Summary: Quid is a tool for quotation detection in texts and can deal with common properties of quotations, for example, ellipses or inaccurate quotations.
 Home-page: https://hu.berlin/quid
 Author: Frederik Arnold
 Author-email: frederik.arnold@hu-berlin.de
 Project-URL: Source, https://hu.berlin/quid
 Keywords: quotation detection,quotation identification,literal citation extraction,key passages,natural language processing,nlp,text reuse
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Quid-2.3.2/Quid.egg-info/PKG-INFO` & `Quid-2.4.0/Quid.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Quid
-Version: 2.3.2
+Version: 2.4.0
 Summary: Quid is a tool for quotation detection in texts and can deal with common properties of quotations, for example, ellipses or inaccurate quotations.
 Home-page: https://hu.berlin/quid
 Author: Frederik Arnold
 Author-email: frederik.arnold@hu-berlin.de
 Project-URL: Source, https://hu.berlin/quid
 Keywords: quotation detection,quotation identification,literal citation extraction,key passages,natural language processing,nlp,text reuse
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Quid-2.3.2/Quid.egg-info/SOURCES.txt` & `Quid-2.4.0/Quid.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -36,12 +36,14 @@
 quid/passager/TargetLocationSelection.py
 quid/passager/TargetMatch.py
 quid/passager/TargetText.py
 quid/passager/TargetTextLocationLink.py
 quid/passager/TextWithMatches.py
 quid/passager/__init__.py
 quid/visualization/Info.py
+quid/visualization/Markup.py
+quid/visualization/MarkupSpan.py
 quid/visualization/TargetHtml.py
 quid/visualization/TargetTextWithContent.py
 quid/visualization/Visualization.py
 quid/visualization/Visualizer.py
 quid/visualization/__init__.py
```

### Comparing `Quid-2.3.2/README.md` & `Quid-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `Quid-2.3.2/quid/cli/QuidCLI.py` & `Quid-2.4.0/quid/cli/QuidCLI.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from quid.passager.SourceSegment import SourceSegment
 from quid.passager.TargetLocation import TargetLocation
 from quid.passager.TargetLocationSelection import TargetLocationSelection
 from quid.passager.TargetText import TargetText
 from quid.passager.TargetTextLocationLink import TargetTextLocationLink
 from quid.match.MatchSpan import MatchSpan
 from quid.visualization.Info import Info
+from quid.visualization.Markup import Markup
 from quid.visualization.TargetTextWithContent import TargetTextWithContent
 from quid.visualization.Visualizer import Visualizer
 from quid.helper.Loader import load_matches, load_citation_sources, load_citation_source_links
 
 
 class OptionValueCheckAction(Action):
 
@@ -64,14 +65,18 @@
 def __json_decoder_target_text(json_input):
     if 'filename' in json_input:
         return TargetText(json_input['my_id'], json_input['filename'], json_input['target_locations'])
     else:
         return TargetLocation(json_input['my_id'], json_input['start'], json_input['end'], json_input['text'])
 
 
+def __json_decoder_markups(json_input):
+    return Markup(json_input['start'], json_input['end'], json_input['klass'])
+
+
 def __json_encoder_quid(obj):
     if isinstance(obj, MatchSpan):
         result_dict = obj.__dict__
 
         if not result_dict['text']:
             del result_dict['text']
 
@@ -299,16 +304,16 @@
 
     with open(join(output_folder_path, 'citation_source_links.json'), 'w', encoding='utf-8') as \
             citation_source_links_output_file:
         content = json.dumps(analyzed_work.citation_source_links, default=__json_encoder_passager)
         citation_source_links_output_file.write(content)
 
 
-def __run_visualize(source_file_path, target_folder_path, passages_folder_path, output_folder_path, title, author,
-                    year, censor):
+def __run_visualize(source_file_path, target_folder_path, passages_folder_path, output_folder_path, markup_file_path,
+                    title, author, year, censor):
     with open(source_file_path, 'r', encoding='utf-8') as source_file:
         source_content = source_file.read()
 
     citation_sources = load_citation_sources(join(passages_folder_path, 'citation_sources.json'))
     citation_source_links = load_citation_source_links(join(passages_folder_path, 'citation_source_links.json'))
 
     with open(join(passages_folder_path, 'target_texts.json'), 'r', encoding='utf-8') as target_texts_file:
@@ -319,17 +324,22 @@
     for target_text in target_texts:
         filename = target_text.filename
         with open(join(target_folder_path, f'{filename}.txt'), 'r', encoding='utf-8') as target_text_file:
             target_content = target_text_file.read()
 
         target_texts_with_content.append(TargetTextWithContent(target_text, target_content))
 
+    markups = None
+    if markup_file_path:
+        with open(markup_file_path, 'r', encoding='utf-8') as markups_file:
+            markups = json.load(markups_file, object_hook=__json_decoder_markups)
+
     visualizer = Visualizer(censor, 25)
     visualization = visualizer.visualize(title, author, year, source_content, citation_sources, citation_source_links,
-                                         target_texts_with_content)
+                                         target_texts_with_content, markups)
 
     with open(join(output_folder_path, 'info.json'), 'w', encoding='utf-8') as info_output_file:
         content = json.dumps(visualization.info, default=__json_encoder_visualization)
         info_output_file.write(content)
 
     with open(join(output_folder_path, 'source' + '.html'), 'w', encoding='utf-8') as source_html_output_file:
         source_html_output_file.write(visualization.source_html)
@@ -454,14 +464,15 @@
     parser_visualize.add_argument("target_folder_path", nargs=1, metavar="target-folder-path",
                                   help="Path to the target texts folder path")
     parser_visualize.add_argument("passages_folder_path", nargs=1, metavar="passages-folder-path",
                                   help="Path to the folder with the key passages files, i.e. the resulting files from"
                                        " quid passage")
     parser_visualize.add_argument("output_folder_path", nargs=1, metavar="output-folder-path",
                                   help="Path to the output folder")
+    parser_visualize.add_argument("--markup-file-path", dest="markup_file_path", help="Path to the markup file")
     parser_visualize.add_argument("--title", dest="title", help="Title of the work", default="NN")
     parser_visualize.add_argument("--author", dest="author", help="Author of the work", default="NN")
     parser_visualize.add_argument("--year", dest="year", help="Year of the work", default="0", type=int)
     parser_visualize.add_argument('--censor', dest="censor", default=False, action='store_true',
                                   help="Censor scholarly works to prevent copyright violations")
 
     args = argument_parser.parse_args(argv)
@@ -515,22 +526,23 @@
 
         __run_passager(source_file_path, target_folder_path, matches_folder_path, output_folder_path)
     elif args.command == 'visualize':
         source_file_path = args.source_file_path[0]
         target_folder_path = args.target_folder_path[0]
         passages_folder_path = args.passages_folder_path[0]
         output_folder_path = args.output_folder_path[0]
-        title = args.title
+        markup_file_path = args.markup_file_path
 
+        title = args.title
         author = args.author
         year = args.year
         censor = args.censor
 
         start_time = time.perf_counter()
-        __run_visualize(source_file_path, target_folder_path, passages_folder_path, output_folder_path, title,
-                        author, year, censor)
+        __run_visualize(source_file_path, target_folder_path, passages_folder_path, output_folder_path, markup_file_path,
+                        title, author, year, censor)
         end_time = time.perf_counter()
         logging.info(f'\n--- Runtime: {end_time - start_time: .2f} seconds ---')
 
 
 if __name__ == '__main__':
     sys.exit(main())
```

### Comparing `Quid-2.3.2/quid/core/Quid.py` & `Quid-2.4.0/quid/core/Quid.py`

 * *Files identical despite different names*

### Comparing `Quid-2.3.2/quid/core/QuidMatcher.py` & `Quid-2.4.0/quid/core/QuidMatcher.py`

 * *Files identical despite different names*

### Comparing `Quid-2.3.2/quid/core/QuidMerger.py` & `Quid-2.4.0/quid/core/QuidMerger.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,16 @@
 
         # self.__print_matches(matches, source_text, target_text)
 
         cleaned_matches: List[InternalMatch] = self.__merge_neighbouring_matches(matches)
         cleaned_matches = self.__remove_matches_with_overlapping_target_match_spans(cleaned_matches)
         cleaned_matches = self.__remove_too_short_matches(cleaned_matches)
         self.__remove_boundary_overshoot(cleaned_matches)
-
+        # After removing boundary overshoot, we can end up with matches which are shorter than the threshold
+        cleaned_matches = self.__remove_too_short_matches(cleaned_matches)
         return cleaned_matches
 
     def __remove_matches_with_overlapping_target_match_spans(self, matches: List[InternalMatch]):
         """
         Removes matches which overlap in the target texts. When keep_ambiguous_matches is true, then matches are only
         removed if they also overlap in the source text.
         :param matches: The input list of matches.
@@ -206,22 +207,24 @@
                     self.tokens[match.target_match_span.token_start_pos].text.startswith('@')):
                 result.append(match)
             elif (match.target_match_span.token_length >= self.min_match_length - 1 and
                   match.target_match_span.token_start_pos - 1 >= self.texts[0].tk_end_pos and
                   (self.tokens[match.target_match_span.token_start_pos].text.startswith('@') or
                    self.tokens[match.target_match_span.token_start_pos - 1].text.startswith('@'))):
                 result.append(match)
+            else:
+                pass
 
         return result
 
     def __remove_boundary_overshoot(self, matches: List[InternalMatch]):
         """
-        Remove tokens after sentence delimiters if they're likely to have matched by accident.
+        Remove tokens after sentence delimiters if they're likely to have matched by accident. Does not return anything
+        but modifies the matches in place.
         :param matches: The list of matches to check.
-        :return: The cleaned matches.
         """
         for match in matches:
             current_source_match_span = match.source_match_span
             current_target_match_span = match.target_match_span
 
             found = False
             if current_source_match_span.token_length > 3:
```

### Comparing `Quid-2.3.2/quid/helper/Decoder.py` & `Quid-2.4.0/quid/helper/Decoder.py`

 * *Files identical despite different names*

### Comparing `Quid-2.3.2/quid/helper/Loader.py` & `Quid-2.4.0/quid/helper/Loader.py`

 * *Files identical despite different names*

### Comparing `Quid-2.3.2/quid/passager/AnalyzedWork.py` & `Quid-2.4.0/quid/passager/AnalyzedWork.py`

 * *Files identical despite different names*

### Comparing `Quid-2.3.2/quid/passager/CitationSource.py` & `Quid-2.4.0/quid/passager/CitationSource.py`

 * *Files identical despite different names*

### Comparing `Quid-2.3.2/quid/passager/Passager.py` & `Quid-2.4.0/quid/passager/Passager.py`

 * *Files identical despite different names*

### Comparing `Quid-2.3.2/quid/passager/SourceSegment.py` & `Quid-2.4.0/quid/passager/SourceSegment.py`

 * *Files identical despite different names*

### Comparing `Quid-2.3.2/quid/passager/TargetText.py` & `Quid-2.4.0/quid/passager/TargetText.py`

 * *Files identical despite different names*

### Comparing `Quid-2.3.2/quid/visualization/Visualizer.py` & `Quid-2.4.0/quid/visualization/Visualizer.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,32 +3,35 @@
 from yattag import Doc
 from math import ceil
 
 from quid.passager.CitationSource import CitationSource
 from quid.visualization.Info import Info
 import re
 
+from quid.visualization.Markup import Markup
+from quid.visualization.MarkupSpan import MarkupSpan
 from quid.visualization.TargetHtml import TargetHtml
 from quid.visualization.TargetTextWithContent import TargetTextWithContent
 from quid.visualization.Visualization import Visualization
 import html
 
 
 # noinspection PyMethodMayBeStatic
 class Visualizer:
 
     def __init__(self, censor: bool = False, keep_range: int = 25):
         self.censor = censor
         self.keep_range = keep_range
 
     def visualize(self, title, author, year, source_content: str, citation_sources: List[CitationSource],
-                  citation_source_links, target_texts_with_content: List[TargetTextWithContent]) -> Visualization:
+                  citation_source_links, target_texts_with_content: List[TargetTextWithContent],
+                  markups: List[Markup] = None) -> Visualization:
 
         info = self.__generate_info_json(title, author, year)
-        source_html = self.__generate_source_html(source_content, citation_sources, citation_source_links)
+        source_html = self.__generate_source_html(source_content, citation_sources, citation_source_links, markups)
         targets_html = self.__generate_target_html(target_texts_with_content)
 
         return Visualization(info, source_html, targets_html)
 
     def __generate_info_json(self, title, author, year) -> Info:
         return Info(title, author, year)
 
@@ -46,91 +49,154 @@
         for citation_source in citation_sources:
             for source_segment in citation_source.source_segments:
                 max_segment_frequency = max(max_segment_frequency, source_segment.frequency)
 
         return max_segment_frequency
 
     def __generate_source_html(self, source_content: str, citation_sources: List[CitationSource],
-                               citation_source_links) -> str:
+                               citation_source_links, markups: List[Markup]) -> str:
 
         max_target_texts_count = self.__calculate_max_target_texts_count(citation_source_links)
         max_segment_frequency = self.__calculate_max_segment_frequency(citation_sources)
 
         doc, tag, text = Doc().tagtext()
 
+        markup_spans = []
+        content_spans = []
         content = ''
         citation_source_start_pos = 0
         segments = []
 
-        for char_pos in range(0, len(source_content)):
+        for char_pos in range(0, len(source_content) + 1):
+            if markups:
+                for mr in markups:
+                    if mr.start == char_pos:
+                        if content:
+                            klasses = ' '.join([x.klass if not x.used else f'{x.klass}_con' for x in markup_spans])
+                            content_spans.append((content, klasses))
+
+                            for ms in markup_spans:
+                                ms.used = True
+
+                        markup_spans.append(MarkupSpan(mr.klass))
+                        content = ''
+
+                    elif mr.end == char_pos:
+                        klasses = ' '.join([x.klass if not x.used else f'{x.klass}_con' for x in markup_spans])
+                        content_spans.append((content, klasses))
+
+                        for ms in markup_spans:
+                            ms.used = True
+                            if ms.klass == mr.klass:
+                                ms.closed = True
+
+                        markup_spans = list(filter(lambda ms: not ms.closed, markup_spans))
+                        content = ''
+
             finished = False
             for citation_source_pos in range(citation_source_start_pos, len(citation_sources)):
                 citation_source = citation_sources[citation_source_pos]
 
                 for segment_pos in range(0, len(citation_source.source_segments)):
                     segment = citation_source.source_segments[segment_pos]
 
                     if char_pos < segment.start:
                         finished = True
                         break
 
                     if segment.start == char_pos:
+                        if content:
+                            klasses = ' '.join([x.klass if not x.used else f'{x.klass}_con' for x in markup_spans])
+                            content_spans.append((content, klasses))
+                            content = ''
+                            for ms in markup_spans:
+                                ms.used = True
+
                         citation_source_start_pos = citation_source_pos
 
                         if segment_pos == 0:
                             with tag('span', klass='text_standard'):
-                                doc.asis(content)
+                                for cs in content_spans:
+                                    if cs[1]:
+                                        with tag('span', klass=cs[1]):
+                                            doc.asis(cs[0])
+                                    else:
+                                        doc.asis(cs[0])
+
                             segments.clear()
                         else:
-                            segments.append(('asis', content))
+                            segments.append(('asis', content_spans.copy()))
 
-                        content = ''
+                        content_spans.clear()
                         finished = True
                         break
                     elif segment.end == char_pos or (segment_pos == len(citation_source.source_segments) - 1 and
                                                      char_pos == len(source_content) - 1):
                         citation_count = self.__calculate_target_text_count(citation_source, citation_source_links)
                         segment_frequency = segment.frequency
                         citation_count_percentage = \
                             int((ceil((citation_count / max_target_texts_count) * 10.0) / 10.0) * 10)
                         segment_frequency_percentage = \
                             int((ceil((segment_frequency / max_segment_frequency) * 10.0) / 10.0) * 10)
                         klass_background = f'source_segment_background_o{citation_count_percentage}'
                         klass_font = f'source_segment_font_s{segment_frequency_percentage}'
                         klass = f'source_segment {klass_background} {klass_font}'
                         tag_id = f'sourceSegment_{citation_source.my_id}_{segment.my_id}'
-                        segments.append(('span', content, klass, tag_id, segment.token_length))
+
+                        klasses = ' '.join([x.klass if not x.used else f'{x.klass}_con' for x in markup_spans])
+                        content_spans.append((content, klasses))
                         content = ''
+
+                        for ms in markup_spans:
+                            ms.used = True
+
+                        segments.append(('span', content_spans.copy(), klass, tag_id, segment.token_length))
+                        content_spans.clear()
                         finished = True
 
                         if segment_pos == len(citation_source.source_segments) - 1:
                             citation_source_start_pos += 1
                             with tag('span', klass='citation_source_container', id=str(citation_source.my_id)):
                                 for segment in segments:
                                     if segment[0] == 'asis':
                                         if segment[1]:
                                             with tag('span', klass='text_standard'):
-                                                doc.asis(segment[1])
+                                                for cs in segment[1]:
+                                                    if cs[1]:
+                                                        with tag('span', klass=cs[1]):
+                                                            doc.asis(cs[0])
+                                                    else:
+                                                        doc.asis(cs[0])
                                     else:
-                                        with tag('span', ('data-token-count', segment[4]), klass=segment[2],
-                                                 id=segment[3]):
-                                            doc.asis(segment[1])
+                                        with tag('span', ('data-token-count', segment[4]), klass=segment[2], id=segment[3]):
+                                            for cs in segment[1]:
+                                                if cs[1]:
+                                                    with tag('span', klass=cs[1]):
+                                                        doc.asis(cs[0])
+                                                else:
+                                                    doc.asis(cs[0])
                         break
 
                 if finished:
                     break
 
-            if source_content[char_pos] == '\n':
-                content += '<br>'
-            else:
-                content += html.escape(source_content[char_pos])
+            if char_pos < len(source_content):
+                if source_content[char_pos] == '\n':
+                    content += '<br>'
+                else:
+                    content += html.escape(source_content[char_pos])
 
-        if len(content) > 0:
+        if len(content_spans) > 0:
             with tag('span', klass='text_standard'):
-                doc.asis(content)
+                for cs in content_spans:
+                    if cs[1]:
+                        with tag('span', klass=cs[1]):
+                            doc.asis(cs[0])
+                    else:
+                        doc.asis(cs[0])
 
         return doc.getvalue()
 
     def __calculate_target_text_count(self, citation_source, citation_source_links):
         for citation_source_link in citation_source_links:
             if citation_source_link.citation_source_id == citation_source.my_id:
                 return len(citation_source_link.target_location_selections)
```

### Comparing `Quid-2.3.2/setup.cfg` & `Quid-2.4.0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = Quid
-version = 2.3.2
+version = 2.4.0
 author = Frederik Arnold
 author_email = frederik.arnold@hu-berlin.de
 description = Quid is a tool for quotation detection in texts and can deal with common properties of quotations, for example, ellipses or inaccurate quotations.
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = quotation detection, quotation identification, literal citation extraction, key passages, natural language processing, nlp, text reuse
 url = https://hu.berlin/quid
@@ -15,18 +15,18 @@
 	License :: OSI Approved :: Apache Software License
 	Operating System :: OS Independent
 
 [options]
 packages = quid, quid.cli, quid.core, quid.helper, quid.match, quid.passager, quid.visualization
 python_requires = >=3.7
 install_requires = 
-	yattag>=1.14.0
-	rapidfuzz>=2.4.2
-	datasketch>=1.5.7
-	tqdm==4.64.1
+	yattag>=1.15.1
+	rapidfuzz>=3.0.0
+	datasketch>=1.5.9
+	tqdm==4.65.0
 
 [options.entry_points]
 console_scripts = 
 	quid = quid.cli.QuidCLI:main
 
 [egg_info]
 tag_build =
```

