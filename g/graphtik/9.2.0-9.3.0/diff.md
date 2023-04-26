# Comparing `tmp/graphtik-9.2.0.tar.gz` & `tmp/graphtik-9.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/graphtik-9.2.0.tar", last modified: Sat Jul  4 07:28:15 2020, max compression
+gzip compressed data, was "dist/graphtik-9.3.0.tar", last modified: Wed Jul  8 14:06:01 2020, max compression
```

## Comparing `graphtik-9.2.0.tar` & `graphtik-9.3.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-04 07:28:15.708110 graphtik-9.2.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)    53959 2020-07-04 07:26:22.000000 graphtik-9.2.0/CHANGES.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     9137 2020-07-04 07:26:22.000000 graphtik-9.2.0/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)       28 2020-07-04 07:26:22.000000 graphtik-9.2.0/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)    10818 2020-07-04 07:28:15.708110 graphtik-9.2.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     7286 2020-07-04 07:26:22.000000 graphtik-9.2.0/README.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-04 07:28:15.700114 graphtik-9.2.0/graphtik/
--rw-rw-r--   0 travis    (2000) travis    (2000)      948 2020-07-04 07:26:22.000000 graphtik-9.2.0/graphtik/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    33675 2020-07-04 07:26:22.000000 graphtik-9.2.0/graphtik/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9522 2020-07-04 07:26:22.000000 graphtik-9.2.0/graphtik/config.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    31364 2020-07-04 07:26:22.000000 graphtik-9.2.0/graphtik/execution.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    38415 2020-07-04 07:26:22.000000 graphtik-9.2.0/graphtik/fnop.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19452 2020-07-04 07:26:22.000000 graphtik-9.2.0/graphtik/jsonpointer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    41695 2020-07-04 07:26:22.000000 graphtik-9.2.0/graphtik/modifier.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    21162 2020-07-04 07:26:22.000000 graphtik-9.2.0/graphtik/pipeline.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    30170 2020-07-04 07:26:22.000000 graphtik-9.2.0/graphtik/planning.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    61394 2020-07-04 07:26:22.000000 graphtik-9.2.0/graphtik/plot.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-04 07:28:15.704112 graphtik-9.2.0/graphtik/sphinxext/
--rw-rw-r--   0 travis    (2000) travis    (2000)    19400 2020-07-04 07:26:22.000000 graphtik-9.2.0/graphtik/sphinxext/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7842 2020-07-04 07:26:22.000000 graphtik-9.2.0/graphtik/sphinxext/_graphtikbuilder.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10141 2020-07-04 07:26:22.000000 graphtik-9.2.0/graphtik/sphinxext/doctestglobs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      285 2020-07-04 07:26:22.000000 graphtik-9.2.0/graphtik/sphinxext/graphtik.css
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-04 07:28:15.704112 graphtik-9.2.0/graphtik.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)    10818 2020-07-04 07:28:15.000000 graphtik-9.2.0/graphtik.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1001 2020-07-04 07:28:15.000000 graphtik-9.2.0/graphtik.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-07-04 07:28:15.000000 graphtik-9.2.0/graphtik.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      972 2020-07-04 07:28:15.000000 graphtik-9.2.0/graphtik.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       14 2020-07-04 07:28:15.000000 graphtik-9.2.0/graphtik.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-07-04 07:28:15.000000 graphtik-9.2.0/graphtik.egg-info/zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)      359 2020-07-04 07:26:22.000000 graphtik-9.2.0/pyproject.toml
--rw-rw-r--   0 travis    (2000) travis    (2000)      746 2020-07-04 07:28:15.708110 graphtik-9.2.0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     4443 2020-07-04 07:26:22.000000 graphtik-9.2.0/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-04 07:28:15.704112 graphtik-9.2.0/test/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-04 07:28:15.708110 graphtik-9.2.0/test/sphinxext/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-07-04 07:26:22.000000 graphtik-9.2.0/test/sphinxext/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      654 2020-07-04 07:26:22.000000 graphtik-9.2.0/test/sphinxext/conftest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3540 2020-07-04 07:26:22.000000 graphtik-9.2.0/test/sphinxext/test_directive.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1571 2020-07-04 07:26:22.000000 graphtik-9.2.0/test/sphinxext/test_image_purgatory.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16452 2020-07-04 07:26:22.000000 graphtik-9.2.0/test/test_base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10362 2020-07-04 07:26:22.000000 graphtik-9.2.0/test/test_combine.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6394 2020-07-04 07:26:22.000000 graphtik-9.2.0/test/test_execution.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    30113 2020-07-04 07:26:22.000000 graphtik-9.2.0/test/test_graphtik.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16581 2020-07-04 07:26:22.000000 graphtik-9.2.0/test/test_hierarchical.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12323 2020-07-04 07:26:22.000000 graphtik-9.2.0/test/test_jsonpointer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12225 2020-07-04 07:26:22.000000 graphtik-9.2.0/test/test_modifier.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22201 2020-07-04 07:26:22.000000 graphtik-9.2.0/test/test_op.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4506 2020-07-04 07:26:22.000000 graphtik-9.2.0/test/test_planning.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23056 2020-07-04 07:26:22.000000 graphtik-9.2.0/test/test_plot.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6157 2020-07-04 07:26:22.000000 graphtik-9.2.0/test/test_remerge.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13819 2020-07-04 07:26:22.000000 graphtik-9.2.0/test/test_sideffects.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2396 2020-07-04 07:26:22.000000 graphtik-9.2.0/test/test_site.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-08 14:06:01.575889 graphtik-9.3.0/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    54881 2020-07-08 14:04:02.000000 graphtik-9.3.0/CHANGES.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9137 2020-07-08 14:04:02.000000 graphtik-9.3.0/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)       28 2020-07-08 14:04:02.000000 graphtik-9.3.0/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10818 2020-07-08 14:06:01.575889 graphtik-9.3.0/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7286 2020-07-08 14:04:02.000000 graphtik-9.3.0/README.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-08 14:06:01.571889 graphtik-9.3.0/graphtik/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      948 2020-07-08 14:04:02.000000 graphtik-9.3.0/graphtik/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    33725 2020-07-08 14:04:02.000000 graphtik-9.3.0/graphtik/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9522 2020-07-08 14:04:02.000000 graphtik-9.3.0/graphtik/config.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    31366 2020-07-08 14:04:02.000000 graphtik-9.3.0/graphtik/execution.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    38952 2020-07-08 14:04:02.000000 graphtik-9.3.0/graphtik/fnop.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19452 2020-07-08 14:04:02.000000 graphtik-9.3.0/graphtik/jsonpointer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41813 2020-07-08 14:04:02.000000 graphtik-9.3.0/graphtik/modifier.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21302 2020-07-08 14:04:02.000000 graphtik-9.3.0/graphtik/pipeline.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    30170 2020-07-08 14:04:02.000000 graphtik-9.3.0/graphtik/planning.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    61493 2020-07-08 14:04:02.000000 graphtik-9.3.0/graphtik/plot.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-08 14:06:01.571889 graphtik-9.3.0/graphtik/sphinxext/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20716 2020-07-08 14:04:02.000000 graphtik-9.3.0/graphtik/sphinxext/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7842 2020-07-08 14:04:02.000000 graphtik-9.3.0/graphtik/sphinxext/_graphtikbuilder.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10141 2020-07-08 14:04:02.000000 graphtik-9.3.0/graphtik/sphinxext/doctestglobs.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      285 2020-07-08 14:04:02.000000 graphtik-9.3.0/graphtik/sphinxext/graphtik.css
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-08 14:06:01.571889 graphtik-9.3.0/graphtik.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10818 2020-07-08 14:06:01.000000 graphtik-9.3.0/graphtik.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1001 2020-07-08 14:06:01.000000 graphtik-9.3.0/graphtik.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-07-08 14:06:01.000000 graphtik-9.3.0/graphtik.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      972 2020-07-08 14:06:01.000000 graphtik-9.3.0/graphtik.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       14 2020-07-08 14:06:01.000000 graphtik-9.3.0/graphtik.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-07-08 14:06:01.000000 graphtik-9.3.0/graphtik.egg-info/zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)      359 2020-07-08 14:04:02.000000 graphtik-9.3.0/pyproject.toml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      746 2020-07-08 14:06:01.575889 graphtik-9.3.0/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4443 2020-07-08 14:04:02.000000 graphtik-9.3.0/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-08 14:06:01.575889 graphtik-9.3.0/test/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-08 14:06:01.575889 graphtik-9.3.0/test/sphinxext/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-07-08 14:04:02.000000 graphtik-9.3.0/test/sphinxext/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      654 2020-07-08 14:04:02.000000 graphtik-9.3.0/test/sphinxext/conftest.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3540 2020-07-08 14:04:02.000000 graphtik-9.3.0/test/sphinxext/test_directive.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1571 2020-07-08 14:04:02.000000 graphtik-9.3.0/test/sphinxext/test_image_purgatory.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16452 2020-07-08 14:04:02.000000 graphtik-9.3.0/test/test_base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10362 2020-07-08 14:04:02.000000 graphtik-9.3.0/test/test_combine.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6394 2020-07-08 14:04:02.000000 graphtik-9.3.0/test/test_execution.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    30113 2020-07-08 14:04:02.000000 graphtik-9.3.0/test/test_graphtik.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16583 2020-07-08 14:04:02.000000 graphtik-9.3.0/test/test_hierarchical.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12323 2020-07-08 14:04:02.000000 graphtik-9.3.0/test/test_jsonpointer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12228 2020-07-08 14:04:02.000000 graphtik-9.3.0/test/test_modifier.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21972 2020-07-08 14:04:02.000000 graphtik-9.3.0/test/test_op.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4506 2020-07-08 14:04:02.000000 graphtik-9.3.0/test/test_planning.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23056 2020-07-08 14:04:02.000000 graphtik-9.3.0/test/test_plot.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6157 2020-07-08 14:04:02.000000 graphtik-9.3.0/test/test_remerge.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13807 2020-07-08 14:04:02.000000 graphtik-9.3.0/test/test_sideffects.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2396 2020-07-08 14:04:02.000000 graphtik-9.3.0/test/test_site.py
```

### Comparing `graphtik-9.2.0/CHANGES.rst` & `graphtik-9.3.0/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -39,21 +39,23 @@
 
   - doc:
 
     - [ ] Merge tutorial (operations + composition)
 
   - DROPPED
 
-    - [-] Solution-retriever modifier;
+    - [X] Solution-retriever modifier;
       WONTFIX: easier and more generic to access solution from Op-context.
       REINSTATED to support simple conveyor belts from json-pointer paths.
-    - [-] `solution.executed` pre-populated with all operations
-    - [-] parallel batches restart from last position in steps
-    - [-] covert custom op classes & modifiers directly into mergeable networkx graphs;
+    - [X] `solution.executed` pre-populated with all operations
+    - [X] parallel batches restart from last position in steps
+    - [X] covert custom op classes & modifiers directly into mergeable networkx graphs;
       WONTFIX bc foreign function would not work with merged deps.
+    - [X] conditionals
+      WONTFIX bc it permits pipelines with too complex execution flow to debug.
 
     - v9.0.0
     - [X] Accept jsonp inputs & outputs,
       WONTFIX user's business to expand into given Inputs, Outputs already working.
     - [x] REVERT rename subdocs;
       WONTFIX bc eventually made it work correctly and added TC.
     - [x] REFACT: separate op-decorator from factory
@@ -73,18 +75,34 @@
 
 https://github.com/pygraphkit/graphtik/releases
 
 Changelog
 %%%%%%%%%
 
 
+v9.3.0 (8 Jul 2020, @ankostis): Sphinx AutoDocumenter; fix plot sfx-nodes
+=========================================================================
+- FIX/FEAT(SPHINXEXT): so far, :func:`.operation`-annotated module functions were
+  excluded from generated sites.  Until the installed *autodoc* function-documenter
+  was instructed how to render the  wrapped function in place of the wrapping
+  ``FnOp``:
+
+  - fix(fnop, pipeline): wrapped function attributes are conveyed to wrapping `FnOp`.
+
+- FIX(plot): sideffect templates were left broken by recent privatization
+  of modifier fields;  add x2 Jinja-filters encapsulating the access to these fields.
+- fix(op): fully fake callables by attaching a ``__qualname__`` property on operations;
+  also teach :func:`.func_name()` not to choke if ``__qualname__`` missing.
+
+
 v9.2.0 (4 Jul 2020, @ankostis): Drop MultiValueError
-====================================================
+----------------------------------------------------
 Delayed raising of needs errors hindered debug.
 
+
 v9.1.0 (4 Jul 2020, @ankostis): Bugfix, panda-polite, privatize modifier fields
 ===============================================================================
 - BREAK(modifier): privatize all :class:`._Modifier` properties;  it is uncanny
   for a str to have more public attributes.
 - fix: avoid equality checks on results, to avoid pandas notorious
   "The truth value of a Series/DataFrame is ambiguous."
 - break(plot): Rename theme property ``include_steps => show_steps``.
```

### Comparing `graphtik-9.2.0/LICENSE` & `graphtik-9.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `graphtik-9.2.0/PKG-INFO` & `graphtik-9.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: graphtik
-Version: 9.2.0
+Version: 9.3.0
 Summary: A lightweight Python-3.6+ lib for solving & executing graphs of functions
 Home-page: http://github.com/pygraphkit/graphtik
 Author: Kostis Anagnostopoulos, Huy Nguyen, Arel Cordero, Pierre Garrigues, Rob Hess, Tobi Baumgartner, Clayton Mellina
 Author-email: ankostis@gmail.com
 License: Apache-2.0
 Project-URL: Documentation, https://graphtik.readthedocs.io/
 Project-URL: Release Notes, https://graphtik.readthedocs.io/en/latest/changes.html
 Project-URL: Sources, https://github.com/pygraphkit/graphtik
 Project-URL: Bug Tracker, https://github.com/pygraphkit/graphtik/issues
 Description: Graphtik
         ========
         
         |python-ver| |dev-status| |gh-version| |pypi-version|
-        (build-version: v9.2.0, build-date: 2020-07-04T07:28:15.497736)
+        (build-version: v9.3.0, build-date: 2020-07-08T14:06:01.366371)
         |travis-status| |doc-status| |cover-status| |codestyle| |proj-lic|
         
         |gh-watch| |gh-star| |gh-fork| |gh-issues|
         
         .. epigraph::
         
             It's a DAG all the way down!
```

### Comparing `graphtik-9.2.0/README.rst` & `graphtik-9.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `graphtik-9.2.0/graphtik/__init__.py` & `graphtik-9.3.0/graphtik/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright 2016, Yahoo Inc.
 # Licensed under the terms of the Apache License, Version 2.0. See the LICENSE file associated with the project for terms.
 """Lightweight :term:`computation` graphs for Python."""
 
-__version__ = "9.2.0"
-__release_date__ = "4 Jul 2020, 10:16"
+__version__ = "9.3.0"
+__release_date__ = "8 Jul 2020, 16:52"
 __title__ = "graphtik"
 __summary__ = __doc__.splitlines()[0]
 __license__ = "Apache-2.0"
 __uri__ = "https://github.com/pygraphkit/graphtik"
 __author__ = "hnguyen, ankostis"  # chronologically ordered
```

### Comparing `graphtik-9.2.0/graphtik/base.py` & `graphtik-9.3.0/graphtik/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,15 +210,18 @@
             fn_name = f"{fn_name}({args_str})"
 
         return fn_name
 
     try:
         if human and inspect.isbuiltin(fn):
             return str(fn)
-        fn_name = fn.__qualname__ if fqdn else fn.__name__
+        # Not possible for all objects to fake ``__qualname__``.
+        fn_name = (
+            fn.__qualname__ if fqdn and hasattr(fn, "__qualname__") else fn.__name__
+        )
         assert fn_name
 
         mod_name = getattr(fn, "__module__", None)
         if mod and mod_name:
             fn_name = ".".join((mod_name, fn_name))
         return fn_name
     except Exception as ex:
@@ -852,18 +855,14 @@
 
     name: str
     needs: Items
     op_needs: Items
     provides: Items
     op_provides: Items
 
-    @property
-    def __name__(self) -> str:
-        return self.name
-
     @abc.abstractmethod
     def compute(self, named_inputs, outputs=None):
         """
         Compute (optional) asked `outputs` for the given `named_inputs`.
 
         It is called by :class:`.Network`.
         End-users should simply call the operation with `named_inputs` as kwargs.
```

### Comparing `graphtik-9.2.0/graphtik/config.py` & `graphtik-9.3.0/graphtik/config.py`

 * *Files identical despite different names*

### Comparing `graphtik-9.2.0/graphtik/execution.py` & `graphtik-9.3.0/graphtik/execution.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,15 +189,15 @@
         accessors = [get_accessor(o) for o in outputs]
         if any(accessors):
             ## Group out-values by their `update` accessor (or None).
             update_groups = defaultdict(list)
             for ac, kv in zip(accessors, outputs.items()):
                 update_groups[ac and ac.update].append(kv)
 
-            ## Values without :attr:`Accessor.update` are to be set one-by-one,
+            ## Values without :attr:`._accessor.update` are to be set one-by-one,
             #  further below.
             outputs = update_groups.pop(None, None)
 
             for upd, pairs in update_groups.items():
                 upd(op_layer, pairs)
 
         if outputs:
```

### Comparing `graphtik-9.2.0/graphtik/fnop.py` & `graphtik-9.3.0/graphtik/fnop.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     (<5ms on a 2019 fast PC)
 """
 
 import itertools as itt
 import logging
 import textwrap
 from collections import abc as cabc
-from functools import wraps
+from functools import update_wrapper, wraps
 from typing import (
     Any,
     Callable,
     Collection,
     Hashable,
     List,
     Mapping,
@@ -211,15 +211,15 @@
               dependency consumed/produced by underlying functions, in the order
               they are first met (the rest duplicate `sideffected` are discarded).
             - any :func:`.sfx` are simply dropped;
 
         `op_deps`
             any :func:`.sfxed` are replaced by a sequence of ":func:`singularized
             <.dep_singularized>`" instances, one for each item in their
-            :attr:`._Modifier.sfx_list` attribute, in the order they are first met
+            :attr:`._Modifier._sfx_list` attribute, in the order they are first met
             (any duplicates are discarded, order is irrelevant, since they don't reach
             the function);
     """
 
     #: The dedupe  any `sideffected`.
     seen_sideffecteds = set()
 
@@ -337,14 +337,30 @@
         #: The :term:`operation`'s underlying function.
         self.fn = fn
         #: a name for the operation (e.g. `'conv1'`, `'sum'`, etc..);
         #: any "parents split by dots(``.``)".
         #: :seealso: :ref:`operation-nesting`
         self.name = name
 
+        #: Fake function attributes.
+        #:
+        if fn:
+            update_wrapper(
+                self,
+                fn,
+                assigned=("__module__", "__doc__", "__annotations__"),
+                updated=(),
+            )
+        self.__name__ = name
+        qname = getattr(fn, "__qualname__", None) or name
+        if qname:
+            # "ab.cd" => "ab.NAME", "ab" => "NAME", "" => "NAME"
+            qname = ".".join((*qname.split(".")[:-1], name))
+        self.__qualname__ = qname
+
         #: The :term:`needs` almost as given by the user
         #: (which may contain MULTI-sideffecteds and dupes),
         #: roughly morphed into `_fn_provides` + sideffects
         #: (DUPES, SFX, SINGULARIZED :term:`sideffected`\s).
         #: It is stored for builder functionality to work.
         self.needs = needs
         #: Value names ready to lay the graph for :term:`pruning`
@@ -871,15 +887,15 @@
     *,
     rescheduled=UNSET,
     endured=UNSET,
     parallel=UNSET,
     marshalled=UNSET,
     returns_dict=UNSET,
     node_props: Mapping = UNSET,
-):
+) -> FnOp:
     r"""
     An :term:`operation` factory that works like a "fancy decorator".
 
     :param fn:
         The callable underlying this operation:
 
           - if not given, it returns the the :meth:`withset()` method as the decorator,
```

### Comparing `graphtik-9.2.0/graphtik/jsonpointer.py` & `graphtik-9.3.0/graphtik/jsonpointer.py`

 * *Files identical despite different names*

### Comparing `graphtik-9.2.0/graphtik/modifier.py` & `graphtik-9.3.0/graphtik/modifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,15 +167,15 @@
         Factory function:func:`_modifier()` may return a plain string, if no other
         arg but ``name`` is given.
     """
 
     #: pre-calculated representation
     _repr: str
     #: The name of a modifier function here, needed to reconstruct
-    #: cstor code in :attr:`cmd`
+    #: cstor code in :meth:`.cmd()`
     _func: str
     #: Map my name in `needs` into this kw-argument of the function.
     #: :func:`get_keyword()` returns it.
     _keyword: str = None
     #: required is None, regular optional or varargish?
     #: :func:`is_optional()` returns it.
     #: All regulars are `keyword`.
@@ -188,15 +188,15 @@
     _sideffected: str = None
     #: At least one name(s) denoting the :term:`sideffects` modification(s) on
     #: the :term:`sideffected`, performed/required by the operation.
     #:
     #: - If it is an empty tuple`, it is an abstract sideffect,
     #:    and :func:`is_pure_optional()` returns True.
     #: - If not empty :func:`is_sfxed()` returns true
-    #:   (the :attr:`sideffected`).
+    #:   (the :attr:`._sideffected`).
     _sfx_list: Tuple[Union[str, None]] = ()
 
     def __new__(
         cls,
         name,
         _repr,
         _func,
@@ -1008,27 +1008,27 @@
 def get_keyword(dep) -> Optional[str]:
     """
     Check if a :term:`dependency` is keyword (and get it).
 
     All non-varargish optionals are "keyword" (including sideffected ones).
 
     :return:
-        the :attr:`.keyword`
+        the :attr:`._keyword`
     """
     return getattr(dep, "_keyword", None)
 
 
 def is_optional(dep) -> Optional[_Optionals]:
     """
     Check if a :term:`dependency` is optional.
 
     Varargish & optional sideffects are included.
 
     :return:
-        the :attr:`.optional`
+        the :attr:`._optional`
     """
     return getattr(dep, "_optional", None)
 
 
 def is_vararg(dep) -> bool:
     """Check if an :term:`optionals` dependency is `vararg`."""
     return getattr(dep, "_optional", None) == _Optionals.vararg
@@ -1050,35 +1050,40 @@
 
 
 def is_sfx(dep) -> Optional[str]:
     """
     Check if a dependency is :term:`sideffects` or :term:`sideffected`.
 
     :return:
-        the :attr:`.sideffected`
+        the :attr:`._sideffected`
     """
     return getattr(dep, "_sideffected", None)
 
 
 def is_pure_sfx(dep) -> bool:
     """Check if it is :term:`sideffects` but not a :term:`sideffected`."""
     return getattr(dep, "_sideffected", None) and not getattr(dep, "_sfx_list", None)
 
 
 def is_sfxed(dep) -> bool:
-    """Check if it is :term:`sideffected`."""
+    """
+    Check if it is :term:`sideffected`.
+
+    :return:
+        the :attr:`._sfx_list` if it is  a *sideffected* dep, None/empty-tuple otherwise
+    """
     return getattr(dep, "_sideffected", None) and getattr(dep, "_sfx_list", None)
 
 
 def get_accessor(dep) -> bool:
     """
     Check if dependency has an :term:`accessor`, and get it (if funcs below are unfit)
 
     :return:
-        the :attr:`accessor`
+        the :attr:`._accessor`
     """
     return getattr(dep, "_accessor", None)
 
 
 def acc_contains(dep) -> Callable[[Collection, str], Any]:
     """
     A fn like :func:`operator.contains` for any `dep` (with-or-without :term:`accessor`)
@@ -1113,15 +1118,15 @@
 
 def dependency(dep) -> str:
     """
     Returns the underlying dependency name (just str)
 
     For non-sideffects, it coincides with str(), otherwise,
     the the pure-sideffect string or the existing :term:`sideffected` dependency
-    stored in :attr:`sideffected`.
+    stored in :attr:`._sideffected`.
     """
     return str(dep) if is_sfx(dep) else dep._sideffected
 
 
 def dep_renamed(dep, ren) -> Union[_Modifier, str]:
     """
     Renames `dep` as `ren` or call `ren`` (if callable) to decide its name,
@@ -1147,26 +1152,26 @@
         dep = renamer(dep)
 
     return dep
 
 
 def dep_singularized(dep) -> Iterable[Union[str, _Modifier]]:
     """
-    Yield one sideffected for each sfx in :attr:`.sfx_list`, or iterate `dep` in other cases.
+    Yield one sideffected for each sfx in :attr:`._sfx_list`, or iterate `dep` in other cases.
     """
     return (
         (modifier_withset(dep, sfx_list=(s,)) for s in dep._sfx_list)
         if is_sfxed(dep)
         else (dep,)
     )
 
 
 def dep_stripped(dep) -> Union[str, _Modifier]:
     """
-    Return the :attr:`_Modifier.sideffected` if `dep` is :term:`sideffected`, `dep` otherwise,
+    Return the :attr:`._sideffected` if `dep` is :term:`sideffected`, `dep` otherwise,
 
     conveying all other properties of the original modifier to the stripped dependency.
     """
     if is_sfxed(dep):
         dep = modifier_withset(
             dep, name=dep._sideffected, sideffected=None, sfx_list=()
         )
```

### Comparing `graphtik-9.2.0/graphtik/pipeline.py` & `graphtik-9.3.0/graphtik/pipeline.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,16 +169,20 @@
 
                 *Operations may only be added once, ...*
         """
         from .fnop import reparse_operation_data
 
         ## Set data asap, for debugging, although `net.withset()` will reset them.
         self.name = name
-        # Remember Outputs for future `compute()`?
+        #: Fake function attributes.
+        self.__name__ = self.__qualname__ = name
+
+        #: Remember Outputs for future `compute()`?
         self.outputs = outputs
+        #: Remember Outputs for future `compute()`?
         self.predicate = predicate
 
         # Prune network
         self.net = build_network(
             operations, rescheduled, endured, parallel, marshalled, node_props, renamer,
         )
         self.name, self.needs, self.provides, _aliases = reparse_operation_data(
```

### Comparing `graphtik-9.2.0/graphtik/planning.py` & `graphtik-9.3.0/graphtik/planning.py`

 * *Files identical despite different names*

### Comparing `graphtik-9.2.0/graphtik/plot.py` & `graphtik-9.3.0/graphtik/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -330,14 +330,16 @@
     )
     env.filters["slug"] = jinja2.evalcontextfilter(
         partial(_escape_or_none, escaper=as_identifier)
     )
     env.filters["hrefer"] = _drop_gt_lt
     env.filters["ex"] = _format_exception
     env.filters["truncate"] = _reversing_truncate
+    env.filters["sideffected"] = is_sfx or None
+    env.filters["sfx_list"] = is_sfxed or None
 
     return env
 
 
 #: Environment to append our own jinja2 filters.
 _jinja2_env = _make_jinja2_environment()
 
@@ -470,16 +472,16 @@
     kw_data_sideffect = {
         "color": "blue",
         "fontcolor": "blue",
     }
     kw_data_sideffected = {
         "label": make_template(
             """
-            <{{ nx_item.sideffected | eee }}<BR/>
-            (<I>sfx:</I> {{ nx_item.sfx_list | join(', ') | eee }})>
+            <{{ nx_item | sideffected | eee }}<BR/>
+            (<I>sfx:</I> {{ nx_item | sfx_list | join(', ') | eee }})>
             """
         ),
     }
     kw_data_to_evict = {
         "color": Ref("evicted"),
         "fontcolor": Ref("evicted"),
         "style": ["dashed"],
```

### Comparing `graphtik-9.2.0/graphtik/sphinxext/__init__.py` & `graphtik-9.3.0/graphtik/sphinxext/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,28 +18,32 @@
 from docutils.parsers.rst import roles as rst_roles
 from sphinx.application import Sphinx
 from sphinx.config import Config
 from sphinx.domains import Domain, Index, ObjType
 from sphinx.domains.std import StandardDomain
 from sphinx.environment import BuildEnvironment
 from sphinx.ext import doctest as extdoctest
+from sphinx.ext.autodoc import ModuleDocumenter
 from sphinx.locale import _, __
 from sphinx.roles import XRefRole
+from sphinx.util import inspect
 from sphinx.util import logging
 from sphinx.util.console import bold  # pylint: disable=no-name-in-module
 from sphinx.writers.html import HTMLTranslator
 from sphinx.writers.latex import LaTeXTranslator
 
+from graphtik.fnop import FnOp
+
 from .. import __version__
 
 try:
     import importlib.resources as pkg_resources
 except ImportError:
     # Use backported to PY<3.7 `importlib_resources` lib.
-    import importlib_resources as pkg_resources
+    import importlib_resources as pkg_resources  # noqa
 
 obj_name = "graphtik diagram"
 role_name = "graphtik"
 log = logging.getLogger(__name__)
 
 
 class graphtik_node(nodes.General, nodes.Element):
@@ -497,19 +501,46 @@
 def _validate_and_apply_configs(app: Sphinx, config: Config):
     """Callback of `config-inited`` event. """
     config.graphtik_default_graph_format is None or _valid_format_option(
         config.graphtik_default_graph_format
     )
 
 
-def setup(app: Sphinx):
-    setup.app = app
-    app.require_sphinx("2.0")
-    app.setup_extension("sphinx.ext.doctest")
+def _teach_documenter_about_operations(FuncDocClass):
+    original__can_document_member = FuncDocClass.can_document_member
+
+    def patched__can_document_member(cls, member, membername, isattr, parent):
+        return original__can_document_member(member, membername, isattr, parent) or (
+            isinstance(member, FnOp) and isinstance(parent, ModuleDocumenter)
+        )
+
+    FuncDocClass.can_document_member = classmethod(patched__can_document_member)
+
+
+def process_fnop_signature(app, what, name, obj, options, signature, return_annotation):
+    try:
+        if isinstance(obj, FnOp):
+            fn = obj.fn
+            fn_sig = inspect.signature(fn)
+            signature = str(fn_sig)
+            return_annotation = None
+    except Exception as ex:
+        log.error("Failed `autodoc-process-signature`: %s", ex, exc_info=1)
+    return (signature, return_annotation)
+
 
+def _setup_autodoc(app: Sphinx):
+    app.setup_extension("sphinx.ext.autodoc")
+
+    _teach_documenter_about_operations(app.registry.documenters["function"])
+    app.connect("autodoc-process-signature", process_fnop_signature)
+
+
+def _setup_directive(app: Sphinx):
+    app.setup_extension("sphinx.ext.doctest")
     app.add_config_value(
         "graphtik_graph_formats_by_builder",
         {"html": "svg", "readthedocs": "svg", "latex": "pdf"},
         "html",
         [cabc.Mapping],
     )
     app.add_config_value("graphtik_default_graph_format", None, "html", [str, None])
@@ -560,12 +591,20 @@
     app.connect("build-finished", _copy_graphtik_static_assets)
 
     app.add_css_file(_css_fname)
 
     # Permanently set this, or else, e.g. +SKIP will not work!
     app.config.trim_doctest_flags = False
 
+
+def setup(app: Sphinx):
+    setup.app = app
+    app.require_sphinx("2.0")
+
+    _setup_autodoc(app)
+    _setup_directive(app)
+
     return {
         "version": __version__,
         "parallel_read_safe": True,
         "parallel_write_safe": True,
     }
```

### Comparing `graphtik-9.2.0/graphtik/sphinxext/_graphtikbuilder.py` & `graphtik-9.3.0/graphtik/sphinxext/_graphtikbuilder.py`

 * *Files identical despite different names*

### Comparing `graphtik-9.2.0/graphtik/sphinxext/doctestglobs.py` & `graphtik-9.3.0/graphtik/sphinxext/doctestglobs.py`

 * *Files identical despite different names*

### Comparing `graphtik-9.2.0/graphtik.egg-info/PKG-INFO` & `graphtik-9.3.0/graphtik.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: graphtik
-Version: 9.2.0
+Version: 9.3.0
 Summary: A lightweight Python-3.6+ lib for solving & executing graphs of functions
 Home-page: http://github.com/pygraphkit/graphtik
 Author: Kostis Anagnostopoulos, Huy Nguyen, Arel Cordero, Pierre Garrigues, Rob Hess, Tobi Baumgartner, Clayton Mellina
 Author-email: ankostis@gmail.com
 License: Apache-2.0
 Project-URL: Documentation, https://graphtik.readthedocs.io/
 Project-URL: Release Notes, https://graphtik.readthedocs.io/en/latest/changes.html
 Project-URL: Sources, https://github.com/pygraphkit/graphtik
 Project-URL: Bug Tracker, https://github.com/pygraphkit/graphtik/issues
 Description: Graphtik
         ========
         
         |python-ver| |dev-status| |gh-version| |pypi-version|
-        (build-version: v9.2.0, build-date: 2020-07-04T07:28:15.497736)
+        (build-version: v9.3.0, build-date: 2020-07-08T14:06:01.366371)
         |travis-status| |doc-status| |cover-status| |codestyle| |proj-lic|
         
         |gh-watch| |gh-star| |gh-fork| |gh-issues|
         
         .. epigraph::
         
             It's a DAG all the way down!
```

### Comparing `graphtik-9.2.0/graphtik.egg-info/SOURCES.txt` & `graphtik-9.3.0/graphtik.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `graphtik-9.2.0/graphtik.egg-info/requires.txt` & `graphtik-9.3.0/graphtik.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -6,46 +6,46 @@
 [:python_version < "3.7"]
 contextvars
 
 [:python_version >= "3.5"]
 networkx
 
 [all]
-pydot
-readme-renderer
-dill
-sphinxcontrib-spelling
 sphinx>=2
+pytest-cov
 jinja2
-pandas
-pytest-sphinx
 matplotlib
-pytest
-pytest-cov
+sphinxcontrib-spelling
 html5lib
+dill
+pytest
+pytest-sphinx
+pydot
+readme-renderer
+pandas
 black
 pylint
 mypy
 
 [all:python_version < "3.7"]
 importlib_resources
 
 [dev]
-pydot
-readme-renderer
-dill
-sphinxcontrib-spelling
 sphinx>=2
+pytest-cov
 jinja2
-pandas
-pytest-sphinx
 matplotlib
-pytest
-pytest-cov
+sphinxcontrib-spelling
 html5lib
+dill
+pytest
+pytest-sphinx
+pydot
+readme-renderer
+pandas
 black
 pylint
 mypy
 
 [dev:python_version < "3.7"]
 importlib_resources
 
@@ -72,22 +72,22 @@
 jinja2
 sphinx>=2
 
 [sphinx:python_version < "3.7"]
 importlib_resources
 
 [test]
-pydot
-readme-renderer
-dill
-sphinxcontrib-spelling
 sphinx>=2
+pytest-cov
 jinja2
-pandas
-pytest-sphinx
 matplotlib
-pytest
-pytest-cov
+sphinxcontrib-spelling
 html5lib
+dill
+pytest
+pytest-sphinx
+pydot
+readme-renderer
+pandas
 
 [test:python_version < "3.7"]
 importlib_resources
```

### Comparing `graphtik-9.2.0/setup.cfg` & `graphtik-9.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `graphtik-9.2.0/setup.py` & `graphtik-9.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `graphtik-9.2.0/test/sphinxext/conftest.py` & `graphtik-9.3.0/test/sphinxext/conftest.py`

 * *Files identical despite different names*

### Comparing `graphtik-9.2.0/test/sphinxext/test_directive.py` & `graphtik-9.3.0/test/sphinxext/test_directive.py`

 * *Files identical despite different names*

### Comparing `graphtik-9.2.0/test/sphinxext/test_image_purgatory.py` & `graphtik-9.3.0/test/sphinxext/test_image_purgatory.py`

 * *Files identical despite different names*

### Comparing `graphtik-9.2.0/test/test_base.py` & `graphtik-9.3.0/test/test_base.py`

 * *Files identical despite different names*

### Comparing `graphtik-9.2.0/test/test_combine.py` & `graphtik-9.3.0/test/test_combine.py`

 * *Files identical despite different names*

### Comparing `graphtik-9.2.0/test/test_execution.py` & `graphtik-9.3.0/test/test_execution.py`

 * *Files identical despite different names*

### Comparing `graphtik-9.2.0/test/test_graphtik.py` & `graphtik-9.3.0/test/test_graphtik.py`

 * *Files identical despite different names*

### Comparing `graphtik-9.2.0/test/test_hierarchical.py` & `graphtik-9.3.0/test/test_hierarchical.py`

 * *Files 0% similar despite different names*

```diff
@@ -173,15 +173,15 @@
             return True
         if ra.typ.endswith(".jsonpart"):
             return False
         if dep == "tasks":
             return True
         # if is_sfxed(dep):
         #     return modifier_withset(
-        #         dep, sfx_list=[f"{ra.parent.name}.{s}" for s in dep.sfx_list]
+        #         dep, sfx_list=[f"{ra.parent.name}.{s}" for s in dep._sfx_list]
         #     )
         if dep == "daily_tasks":
             return dep_renamed(dep, lambda n: f"{n}/{ra.parent.name}")
         return False
 
     week = compose("week", *weekdays, nest=nester)
     assert str(week) == re.sub(
@@ -336,15 +336,15 @@
             return True
         if ra.typ.endswith(".jsonpart"):
             return False
         if dep == "tasks":
             return True
         # if is_sfxed(dep):
         #     return modifier_withset(
-        #         dep, sfx_list=[f"{ra.parent.name}.{s}" for s in dep.sfx_list]
+        #         dep, sfx_list=[f"{ra.parent.name}.{s}" for s in dep._sfx_list]
         #     )
         if dep == "daily_tasks":
             return dep_renamed(dep, lambda n: f"{n}/{ra.parent.name}")
         return False
 
     week = compose("week", *weekdays, nest=nester)
     assert str(week) == re.sub(
```

### Comparing `graphtik-9.2.0/test/test_jsonpointer.py` & `graphtik-9.3.0/test/test_jsonpointer.py`

 * *Files identical despite different names*

### Comparing `graphtik-9.2.0/test/test_modifier.py` & `graphtik-9.3.0/test/test_modifier.py`

 * *Files 0% similar despite different names*

```diff
@@ -244,17 +244,17 @@
 def test_modifs_rename_fn(mod, exp, ser_method):
     renamer = lambda n: f"p.{n}"
     dep = mod()
     got = dep_renamed(dep, renamer)
     assert repr(got) == exp
     assert repr(ser_method(got)) == exp
 
-    if getattr(dep, "sideffected", None):
+    if getattr(dep, "_sideffected", None):
         # Check not just(!) `_repr` has changed.
-        assert got.sideffected != dep.sideffected
+        assert got._sideffected != dep._sideffected
 
     if getattr(dep, "_jsonp", None):
         assert got._jsonp != dep._jsonp
         assert got._jsonp == jsonp_path(got)
         assert got._jsonp == jsonp_path(str(got))
```

### Comparing `graphtik-9.2.0/test/test_op.py` & `graphtik-9.3.0/test/test_op.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,16 @@
     tasks_in_parallel,
     tasks_marshalled,
 )
 from graphtik.fnop import FnOp, Operation, as_renames, reparse_operation_data
 from graphtik.modifier import dep_renamed
 from graphtik.planning import yield_ops
 
+from .helpers import oneliner
+
 
 @pytest.fixture(params=[None, "got"])
 def opname(request):
     return request.param
 
 
 @pytest.fixture(params=[None, "some"])
@@ -606,23 +608,21 @@
     def renamer(na):
         if na.name and na.typ.endswith(".jsonpart"):
             return f"PP.{na.name}"
 
     ren = op.withset(renamer=renamer)
     got = str(ren)
     print(got)
-    assert got == re.sub(
-        r"[\n ]+",  # collapse all space-chars into a single space
-        " ",
+    assert got == oneliner(
         """
         FnOp(name='op1',
             needs=[sfx('a/b'), '/PP.a/PP.b'($)],
             provides=['PP.b/PP.c'($), sfxed('PP.d/PP.e/PP.f'($), 'k/l')],
             aliases=[('PP.b/PP.c'($), '/PP.b/PP.t'($))], fn='str')
-        """.strip(),
+        """,
     )
 
 
 def test_pipe_rename():
     pipe = compose(
         "t",
         operation(str, name="op1", needs=sfx("a")),
@@ -644,38 +644,34 @@
     got = str(ren)
     assert got == (
         """
     Pipeline('t', needs=[sfx('PP.a')], provides=['PP.a', sfx('PP.b'), 'PP.b'], x2 ops: PP.op1, PP.op2)
         """.strip()
     )
     got = str(ren.ops)
-    assert got == re.sub(
-        r"[\n ]+",  # collapse all space-chars into a single space
-        " ",
+    assert got == oneliner(
         """
         [FnOp(name='PP.op1', needs=[sfx('PP.a')], fn='str'),
          FnOp(name='PP.op2', needs=[sfx('PP.a')], provides=['PP.a', sfx('PP.b')],
          aliases=[('PP.a', 'PP.b')], fn='str')]
-        """.strip(),
+        """
     )
 
     ## Check dictionary with callables
     #
     ren = pipe.withset(
         renamer={"op1": lambda n: "OP1", "op2": False, "a": optional("a"), "b": "B",}
     )
     got = str(ren.ops)
-    assert got == re.sub(
-        r"[\n ]+",  # collapse all space-chars into a single space
-        " ",
+    assert got == oneliner(
         """
         [FnOp(name='OP1', needs=[sfx('a')], fn='str'),
          FnOp(name='op2', needs=[sfx('a')], provides=['a'(?), sfx('b')],
          aliases=[('a'(?), 'B')], fn='str')]
-        """.strip(),
+        """
     )
 
 
 def test_conveyor_identity_fn():
     op = operation(name="copy values", needs="a")()
     assert not op.fn
     op = operation(None, needs="a", provides="A")
```

### Comparing `graphtik-9.2.0/test/test_planning.py` & `graphtik-9.3.0/test/test_planning.py`

 * *Files identical despite different names*

### Comparing `graphtik-9.2.0/test/test_plot.py` & `graphtik-9.3.0/test/test_plot.py`

 * *Files identical despite different names*

### Comparing `graphtik-9.2.0/test/test_remerge.py` & `graphtik-9.3.0/test/test_remerge.py`

 * *Files identical despite different names*

### Comparing `graphtik-9.2.0/test/test_sideffects.py` & `graphtik-9.3.0/test/test_sideffects.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Licensed under the terms of the Apache License, Version 2.0. See the LICENSE file associated with the project for terms.
 """Test :term:`sideffects`."""
 import re
 import types
 from itertools import cycle
 from operator import add, mul, sub
 from textwrap import dedent
-from typing import Tuple
+from typing import Any, Tuple
 
 import pytest
 
 from graphtik import NO_RESULT, NO_RESULT_BUT_SFX, compose, operation, sfx, sfxed
 from graphtik.config import get_execution_pool, is_marshal_tasks
 from graphtik.pipeline import Pipeline
 
@@ -270,40 +270,43 @@
     pipeline = compose("t", op1, op2, parallel=exemethod)
     sol = pipeline.compute()
     assert sol == {"a": 1, an_sfx: False, "b": 1}
     sol = pipeline.compute(outputs="b")
     assert sol == {"b": 1}
 
 
+DataFrame = Any
+
+
 @pytest.fixture(params=[0, 1])
 def calc_prices_pipeline(request, exemethod):
     """A pipeline that may work even without VAT-rates."""
 
     @operation(needs="order_items", provides=sfxed("ORDER", "Items", "Prices"))
-    def new_order(items: list) -> "pd.DataFrame":
+    def new_order(items: list) -> DataFrame:
         order = {"items": items}
         # Pretend we get the prices from sales.
         order["prices"] = list(range(1, len(order["items"]) + 1))
         return order
 
     @operation(
         needs=[sfxed("ORDER", "Items"), "vat rate"],
         provides=sfxed("ORDER", "VAT rates"),
     )
-    def fill_in_vat_ratios(order: "pd.DataFrame", base_vat: float) -> "pd.DataFrame":
+    def fill_in_vat_ratios(order: DataFrame, base_vat: float) -> DataFrame:
         order["VAT_rates"] = [
             v for _, v in zip(order["prices"], cycle((base_vat, 2 * base_vat)))
         ]
         return order
 
     @operation(
         needs=[sfxed("ORDER", "Prices"), sfxed("ORDER", "VAT rates", optional=True),],
         provides=[sfxed("ORDER", "VAT", "Totals"), "vat owed"],
     )
-    def finalize_prices(order: "pd.DataFrame") -> Tuple["pd.DataFrame", float]:
+    def finalize_prices(order: DataFrame) -> Tuple[DataFrame, float]:
         if "VAT_rates" in order:
             order["VAT"] = [p * v for p, v in zip(order["prices"], order["VAT_rates"])]
             order["totals"] = [p + v for p, v in zip(order["prices"], order["VAT"])]
             vat_to_pay = sum(order["VAT"])
         else:
             order["totals"] = order["prices"][::]
             vat_to_pay = None
@@ -362,15 +365,15 @@
     ## Break `fill_in_vat_ratios()`.
     #
     @operation(
         needs=[sfxed("ORDER", "Items"), "vat rate"],
         provides=sfxed("ORDER", "VAT rates"),
         endured=True,
     )
-    def fill_in_vat_ratios(order: "pd.DataFrame", base_vat: float) -> "pd.DataFrame":
+    def fill_in_vat_ratios(order: DataFrame, base_vat: float) -> DataFrame:
         raise ValueError("EC transactions have no VAT!")
 
     calc_prices_pipeline = compose(
         calc_prices_pipeline.name, fill_in_vat_ratios, calc_prices_pipeline, nest=False
     )
 
     sol = calc_prices_pipeline.compute(
```

### Comparing `graphtik-9.2.0/test/test_site.py` & `graphtik-9.3.0/test/test_site.py`

 * *Files identical despite different names*

