# Comparing `tmp/edpm-1.0.8.tar.gz` & `tmp/edpm-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edpm-1.0.8.tar", last modified: Wed Aug  3 13:51:02 2022, max compression
+gzip compressed data, was "edpm-1.0.9.tar", last modified: Wed Aug  3 13:57:29 2022, max compression
```

## Comparing `edpm-1.0.8.tar` & `edpm-1.0.9.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxr-x   0 romanov   (1000) romanov   (1000)        0 2022-08-03 13:51:02.224944 edpm-1.0.8/
--rw-r--r--   0 romanov   (1000) romanov   (1000)     1073 2022-07-09 18:31:18.000000 edpm-1.0.8/LICENSE
--rw-r--r--   0 romanov   (1000) romanov   (1000)      109 2022-07-09 18:35:35.000000 edpm-1.0.8/MANIFEST.in
--rw-rw-r--   0 romanov   (1000) romanov   (1000)     6610 2022-08-03 13:51:02.224944 edpm-1.0.8/PKG-INFO
--rw-r--r--   0 romanov   (1000) romanov   (1000)    19597 2022-07-11 13:17:28.000000 edpm-1.0.8/README.md
-drwxrwxr-x   0 romanov   (1000) romanov   (1000)        0 2022-08-03 13:51:02.220944 edpm-1.0.8/edpm/
--rw-r--r--   0 romanov   (1000) romanov   (1000)     3868 2022-07-11 13:18:26.000000 edpm-1.0.8/edpm/__init__.py
-drwxrwxr-x   0 romanov   (1000) romanov   (1000)        0 2022-08-03 13:51:02.220944 edpm-1.0.8/edpm/cli/
--rw-r--r--   0 romanov   (1000) romanov   (1000)        0 2022-07-09 18:31:18.000000 edpm-1.0.8/edpm/cli/__init__.py
--rw-r--r--   0 romanov   (1000) romanov   (1000)     2789 2022-07-09 18:35:35.000000 edpm-1.0.8/edpm/cli/clean.py
--rw-r--r--   0 romanov   (1000) romanov   (1000)     3864 2022-07-09 18:35:35.000000 edpm-1.0.8/edpm/cli/config.py
--rw-r--r--   0 romanov   (1000) romanov   (1000)     1932 2022-07-09 18:35:35.000000 edpm-1.0.8/edpm/cli/env.py
--rw-r--r--   0 romanov   (1000) romanov   (1000)     1145 2022-07-09 18:35:35.000000 edpm-1.0.8/edpm/cli/example_command.py
--rw-r--r--   0 romanov   (1000) romanov   (1000)      606 2022-07-09 18:35:35.000000 edpm-1.0.8/edpm/cli/find.py
--rw-r--r--   0 romanov   (1000) romanov   (1000)     2613 2022-07-11 13:17:28.000000 edpm-1.0.8/edpm/cli/info.py
--rw-r--r--   0 romanov   (1000) romanov   (1000)    10202 2022-07-19 20:51:34.000000 edpm-1.0.8/edpm/cli/install.py
--rw-r--r--   0 romanov   (1000) romanov   (1000)     1204 2022-07-09 18:35:35.000000 edpm-1.0.8/edpm/cli/mergedb.py
--rw-r--r--   0 romanov   (1000) romanov   (1000)     3155 2022-07-09 18:35:35.000000 edpm-1.0.8/edpm/cli/pwd.py
--rw-r--r--   0 romanov   (1000) romanov   (1000)     2538 2022-07-27 03:33:50.000000 edpm-1.0.8/edpm/cli/req.py
--rw-r--r--   0 romanov   (1000) romanov   (1000)     3263 2022-07-09 18:35:35.000000 edpm-1.0.8/edpm/cli/rm.py
--rw-r--r--   0 romanov   (1000) romanov   (1000)      979 2022-07-09 18:35:35.000000 edpm-1.0.8/edpm/cli/set.py
-drwxrwxr-x   0 romanov   (1000) romanov   (1000)        0 2022-08-03 13:51:02.224944 edpm-1.0.8/edpm/engine/
--rw-r--r--   0 romanov   (1000) romanov   (1000)       21 2022-07-14 17:50:24.000000 edpm-1.0.8/edpm/engine/__init__.py
--rw-r--r--   0 romanov   (1000) romanov   (1000)    11194 2022-07-26 23:17:42.000000 edpm-1.0.8/edpm/engine/api.py
--rw-r--r--   0 romanov   (1000) romanov   (1000)     3253 2022-07-09 18:31:18.000000 edpm-1.0.8/edpm/engine/commands.py
--rw-r--r--   0 romanov   (1000) romanov   (1000)      576 2022-07-09 18:31:18.000000 edpm-1.0.8/edpm/engine/convig.py
--rw-r--r--   0 romanov   (1000) romanov   (1000)    10080 2022-07-10 20:53:42.000000 edpm-1.0.8/edpm/engine/db.py
--rw-r--r--   0 romanov   (1000) romanov   (1000)     5954 2022-07-09 18:31:18.000000 edpm-1.0.8/edpm/engine/env_gen.py
--rw-r--r--   0 romanov   (1000) romanov   (1000)     3793 2022-07-09 18:35:35.000000 edpm-1.0.8/edpm/engine/git_cmake_recipe.py
--rw-r--r--   0 romanov   (1000) romanov   (1000)     2998 2022-07-09 18:31:18.000000 edpm-1.0.8/edpm/engine/output.py
--rw-r--r--   0 romanov   (1000) romanov   (1000)      246 2022-07-09 18:31:18.000000 edpm-1.0.8/edpm/engine/py23.py
--rw-r--r--   0 romanov   (1000) romanov   (1000)     3721 2022-07-09 18:31:18.000000 edpm-1.0.8/edpm/engine/recipe.py
--rw-r--r--   0 romanov   (1000) romanov   (1000)     6267 2022-07-11 13:17:28.000000 edpm-1.0.8/edpm/engine/recipe_manager.py
--rw-r--r--   0 romanov   (1000) romanov   (1000)      124 2022-07-09 18:31:18.000000 edpm-1.0.8/edpm/engine/standard_actions.py
-drwxrwxr-x   0 romanov   (1000) romanov   (1000)        0 2022-08-03 13:51:02.224944 edpm-1.0.8/edpm/recipes/
--rw-r--r--   0 romanov   (1000) romanov   (1000)        3 2022-07-09 18:31:18.000000 edpm-1.0.8/edpm/recipes/__init__.py
--rw-r--r--   0 romanov   (1000) romanov   (1000)     3772 2022-07-26 22:58:10.000000 edpm-1.0.8/edpm/recipes/acts.py
--rw-r--r--   0 romanov   (1000) romanov   (1000)     2223 2022-07-26 23:02:50.000000 edpm-1.0.8/edpm/recipes/clhep.py
--rw-r--r--   0 romanov   (1000) romanov   (1000)     4789 2022-07-26 22:58:42.000000 edpm-1.0.8/edpm/recipes/dd4hep.py
--rw-r--r--   0 romanov   (1000) romanov   (1000)     7176 2022-07-28 01:20:38.000000 edpm-1.0.8/edpm/recipes/detector.py
--rw-rw-r--   0 romanov   (1000) romanov   (1000)     2400 2022-07-26 23:49:44.000000 edpm-1.0.8/edpm/recipes/edm4hep.py
--rw-rw-r--   0 romanov   (1000) romanov   (1000)     4964 2022-07-27 03:31:01.000000 edpm-1.0.8/edpm/recipes/eicrecon.py
--rw-r--r--   0 romanov   (1000) romanov   (1000)     1199 2022-07-26 22:59:14.000000 edpm-1.0.8/edpm/recipes/eigen3.py
--rw-r--r--   0 romanov   (1000) romanov   (1000)     7830 2022-07-26 22:59:51.000000 edpm-1.0.8/edpm/recipes/geant4.py
--rw-r--r--   0 romanov   (1000) romanov   (1000)     2582 2022-07-26 23:00:02.000000 edpm-1.0.8/edpm/recipes/hepmc3.py
--rw-r--r--   0 romanov   (1000) romanov   (1000)     2149 2022-07-26 23:00:37.000000 edpm-1.0.8/edpm/recipes/jana2.py
--rw-r--r--   0 romanov   (1000) romanov   (1000)     2517 2022-07-26 23:01:01.000000 edpm-1.0.8/edpm/recipes/npdet.py
--rw-rw-r--   0 romanov   (1000) romanov   (1000)     1901 2022-07-26 23:01:11.000000 edpm-1.0.8/edpm/recipes/phasm.py
--rw-r--r--   0 romanov   (1000) romanov   (1000)     2872 2022-07-26 23:01:32.000000 edpm-1.0.8/edpm/recipes/podio.py
--rw-r--r--   0 romanov   (1000) romanov   (1000)     5676 2022-07-26 23:02:33.000000 edpm-1.0.8/edpm/recipes/pythia8.py
--rw-r--r--   0 romanov   (1000) romanov   (1000)    20624 2022-07-27 03:45:39.000000 edpm-1.0.8/edpm/recipes/root.py
--rw-r--r--   0 romanov   (1000) romanov   (1000)      181 2022-08-03 13:50:57.000000 edpm-1.0.8/edpm/version.py
-drwxrwxr-x   0 romanov   (1000) romanov   (1000)        0 2022-08-03 13:51:02.220944 edpm-1.0.8/edpm.egg-info/
--rw-rw-r--   0 romanov   (1000) romanov   (1000)     6610 2022-08-03 13:51:02.000000 edpm-1.0.8/edpm.egg-info/PKG-INFO
--rw-rw-r--   0 romanov   (1000) romanov   (1000)     1159 2022-08-03 13:51:02.000000 edpm-1.0.8/edpm.egg-info/SOURCES.txt
--rw-rw-r--   0 romanov   (1000) romanov   (1000)        1 2022-08-03 13:51:02.000000 edpm-1.0.8/edpm.egg-info/dependency_links.txt
--rw-rw-r--   0 romanov   (1000) romanov   (1000)       39 2022-08-03 13:51:02.000000 edpm-1.0.8/edpm.egg-info/entry_points.txt
--rw-rw-r--   0 romanov   (1000) romanov   (1000)       14 2022-08-03 13:51:02.000000 edpm-1.0.8/edpm.egg-info/requires.txt
--rw-rw-r--   0 romanov   (1000) romanov   (1000)        5 2022-08-03 13:51:02.000000 edpm-1.0.8/edpm.egg-info/top_level.txt
--rw-r--r--   0 romanov   (1000) romanov   (1000)     6062 2022-07-11 13:17:28.000000 edpm-1.0.8/pip_readme.md
--rw-r--r--   0 romanov   (1000) romanov   (1000)       54 2022-08-03 13:51:02.224944 edpm-1.0.8/setup.cfg
--rw-r--r--   0 romanov   (1000) romanov   (1000)     1368 2022-07-11 13:18:20.000000 edpm-1.0.8/setup.py
+drwxrwxr-x   0 romanov   (1000) romanov   (1000)        0 2022-08-03 13:57:29.625009 edpm-1.0.9/
+-rw-r--r--   0 romanov   (1000) romanov   (1000)     1073 2022-07-09 18:31:18.000000 edpm-1.0.9/LICENSE
+-rw-r--r--   0 romanov   (1000) romanov   (1000)      109 2022-07-09 18:35:35.000000 edpm-1.0.9/MANIFEST.in
+-rw-rw-r--   0 romanov   (1000) romanov   (1000)     6610 2022-08-03 13:57:29.625009 edpm-1.0.9/PKG-INFO
+-rw-r--r--   0 romanov   (1000) romanov   (1000)    19597 2022-07-11 13:17:28.000000 edpm-1.0.9/README.md
+drwxrwxr-x   0 romanov   (1000) romanov   (1000)        0 2022-08-03 13:57:29.621009 edpm-1.0.9/edpm/
+-rw-r--r--   0 romanov   (1000) romanov   (1000)     3868 2022-07-11 13:18:26.000000 edpm-1.0.9/edpm/__init__.py
+drwxrwxr-x   0 romanov   (1000) romanov   (1000)        0 2022-08-03 13:57:29.621009 edpm-1.0.9/edpm/cli/
+-rw-r--r--   0 romanov   (1000) romanov   (1000)        0 2022-07-09 18:31:18.000000 edpm-1.0.9/edpm/cli/__init__.py
+-rw-r--r--   0 romanov   (1000) romanov   (1000)     2789 2022-07-09 18:35:35.000000 edpm-1.0.9/edpm/cli/clean.py
+-rw-r--r--   0 romanov   (1000) romanov   (1000)     3864 2022-07-09 18:35:35.000000 edpm-1.0.9/edpm/cli/config.py
+-rw-r--r--   0 romanov   (1000) romanov   (1000)     1932 2022-07-09 18:35:35.000000 edpm-1.0.9/edpm/cli/env.py
+-rw-r--r--   0 romanov   (1000) romanov   (1000)     1145 2022-07-09 18:35:35.000000 edpm-1.0.9/edpm/cli/example_command.py
+-rw-r--r--   0 romanov   (1000) romanov   (1000)      606 2022-07-09 18:35:35.000000 edpm-1.0.9/edpm/cli/find.py
+-rw-r--r--   0 romanov   (1000) romanov   (1000)     2613 2022-07-11 13:17:28.000000 edpm-1.0.9/edpm/cli/info.py
+-rw-r--r--   0 romanov   (1000) romanov   (1000)    10202 2022-07-19 20:51:34.000000 edpm-1.0.9/edpm/cli/install.py
+-rw-r--r--   0 romanov   (1000) romanov   (1000)     1204 2022-07-09 18:35:35.000000 edpm-1.0.9/edpm/cli/mergedb.py
+-rw-r--r--   0 romanov   (1000) romanov   (1000)     3155 2022-07-09 18:35:35.000000 edpm-1.0.9/edpm/cli/pwd.py
+-rw-r--r--   0 romanov   (1000) romanov   (1000)     2538 2022-07-27 03:33:50.000000 edpm-1.0.9/edpm/cli/req.py
+-rw-r--r--   0 romanov   (1000) romanov   (1000)     3263 2022-07-09 18:35:35.000000 edpm-1.0.9/edpm/cli/rm.py
+-rw-r--r--   0 romanov   (1000) romanov   (1000)      979 2022-07-09 18:35:35.000000 edpm-1.0.9/edpm/cli/set.py
+drwxrwxr-x   0 romanov   (1000) romanov   (1000)        0 2022-08-03 13:57:29.621009 edpm-1.0.9/edpm/engine/
+-rw-r--r--   0 romanov   (1000) romanov   (1000)       21 2022-07-14 17:50:24.000000 edpm-1.0.9/edpm/engine/__init__.py
+-rw-r--r--   0 romanov   (1000) romanov   (1000)    11194 2022-07-26 23:17:42.000000 edpm-1.0.9/edpm/engine/api.py
+-rw-r--r--   0 romanov   (1000) romanov   (1000)     3253 2022-07-09 18:31:18.000000 edpm-1.0.9/edpm/engine/commands.py
+-rw-r--r--   0 romanov   (1000) romanov   (1000)      576 2022-07-09 18:31:18.000000 edpm-1.0.9/edpm/engine/convig.py
+-rw-r--r--   0 romanov   (1000) romanov   (1000)    10080 2022-07-10 20:53:42.000000 edpm-1.0.9/edpm/engine/db.py
+-rw-r--r--   0 romanov   (1000) romanov   (1000)     5954 2022-07-09 18:31:18.000000 edpm-1.0.9/edpm/engine/env_gen.py
+-rw-r--r--   0 romanov   (1000) romanov   (1000)     3793 2022-07-09 18:35:35.000000 edpm-1.0.9/edpm/engine/git_cmake_recipe.py
+-rw-r--r--   0 romanov   (1000) romanov   (1000)     2998 2022-07-09 18:31:18.000000 edpm-1.0.9/edpm/engine/output.py
+-rw-r--r--   0 romanov   (1000) romanov   (1000)      246 2022-07-09 18:31:18.000000 edpm-1.0.9/edpm/engine/py23.py
+-rw-r--r--   0 romanov   (1000) romanov   (1000)     3721 2022-07-09 18:31:18.000000 edpm-1.0.9/edpm/engine/recipe.py
+-rw-r--r--   0 romanov   (1000) romanov   (1000)     6267 2022-07-11 13:17:28.000000 edpm-1.0.9/edpm/engine/recipe_manager.py
+-rw-r--r--   0 romanov   (1000) romanov   (1000)      124 2022-07-09 18:31:18.000000 edpm-1.0.9/edpm/engine/standard_actions.py
+drwxrwxr-x   0 romanov   (1000) romanov   (1000)        0 2022-08-03 13:57:29.625009 edpm-1.0.9/edpm/recipes/
+-rw-r--r--   0 romanov   (1000) romanov   (1000)        3 2022-07-09 18:31:18.000000 edpm-1.0.9/edpm/recipes/__init__.py
+-rw-r--r--   0 romanov   (1000) romanov   (1000)     3772 2022-07-26 22:58:10.000000 edpm-1.0.9/edpm/recipes/acts.py
+-rw-r--r--   0 romanov   (1000) romanov   (1000)     2223 2022-07-26 23:02:50.000000 edpm-1.0.9/edpm/recipes/clhep.py
+-rw-r--r--   0 romanov   (1000) romanov   (1000)     4789 2022-07-26 22:58:42.000000 edpm-1.0.9/edpm/recipes/dd4hep.py
+-rw-r--r--   0 romanov   (1000) romanov   (1000)     7217 2022-08-03 13:56:47.000000 edpm-1.0.9/edpm/recipes/detector.py
+-rw-rw-r--   0 romanov   (1000) romanov   (1000)     2485 2022-08-03 13:56:47.000000 edpm-1.0.9/edpm/recipes/edm4hep.py
+-rw-rw-r--   0 romanov   (1000) romanov   (1000)     4964 2022-07-27 03:31:01.000000 edpm-1.0.9/edpm/recipes/eicrecon.py
+-rw-r--r--   0 romanov   (1000) romanov   (1000)     1199 2022-07-26 22:59:14.000000 edpm-1.0.9/edpm/recipes/eigen3.py
+-rw-r--r--   0 romanov   (1000) romanov   (1000)     7830 2022-07-26 22:59:51.000000 edpm-1.0.9/edpm/recipes/geant4.py
+-rw-r--r--   0 romanov   (1000) romanov   (1000)     2582 2022-07-26 23:00:02.000000 edpm-1.0.9/edpm/recipes/hepmc3.py
+-rw-r--r--   0 romanov   (1000) romanov   (1000)     2149 2022-07-26 23:00:37.000000 edpm-1.0.9/edpm/recipes/jana2.py
+-rw-r--r--   0 romanov   (1000) romanov   (1000)     2517 2022-07-26 23:01:01.000000 edpm-1.0.9/edpm/recipes/npdet.py
+-rw-rw-r--   0 romanov   (1000) romanov   (1000)     1901 2022-07-26 23:01:11.000000 edpm-1.0.9/edpm/recipes/phasm.py
+-rw-r--r--   0 romanov   (1000) romanov   (1000)     2872 2022-07-26 23:01:32.000000 edpm-1.0.9/edpm/recipes/podio.py
+-rw-r--r--   0 romanov   (1000) romanov   (1000)     5676 2022-07-26 23:02:33.000000 edpm-1.0.9/edpm/recipes/pythia8.py
+-rw-r--r--   0 romanov   (1000) romanov   (1000)    20624 2022-07-27 03:45:39.000000 edpm-1.0.9/edpm/recipes/root.py
+-rw-r--r--   0 romanov   (1000) romanov   (1000)      181 2022-08-03 13:57:01.000000 edpm-1.0.9/edpm/version.py
+drwxrwxr-x   0 romanov   (1000) romanov   (1000)        0 2022-08-03 13:57:29.621009 edpm-1.0.9/edpm.egg-info/
+-rw-rw-r--   0 romanov   (1000) romanov   (1000)     6610 2022-08-03 13:57:29.000000 edpm-1.0.9/edpm.egg-info/PKG-INFO
+-rw-rw-r--   0 romanov   (1000) romanov   (1000)     1159 2022-08-03 13:57:29.000000 edpm-1.0.9/edpm.egg-info/SOURCES.txt
+-rw-rw-r--   0 romanov   (1000) romanov   (1000)        1 2022-08-03 13:57:29.000000 edpm-1.0.9/edpm.egg-info/dependency_links.txt
+-rw-rw-r--   0 romanov   (1000) romanov   (1000)       39 2022-08-03 13:57:29.000000 edpm-1.0.9/edpm.egg-info/entry_points.txt
+-rw-rw-r--   0 romanov   (1000) romanov   (1000)       14 2022-08-03 13:57:29.000000 edpm-1.0.9/edpm.egg-info/requires.txt
+-rw-rw-r--   0 romanov   (1000) romanov   (1000)        5 2022-08-03 13:57:29.000000 edpm-1.0.9/edpm.egg-info/top_level.txt
+-rw-r--r--   0 romanov   (1000) romanov   (1000)     6062 2022-07-11 13:17:28.000000 edpm-1.0.9/pip_readme.md
+-rw-r--r--   0 romanov   (1000) romanov   (1000)       54 2022-08-03 13:57:29.625009 edpm-1.0.9/setup.cfg
+-rw-r--r--   0 romanov   (1000) romanov   (1000)     1368 2022-07-11 13:18:20.000000 edpm-1.0.9/setup.py
```

### Comparing `edpm-1.0.8/LICENSE` & `edpm-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `edpm-1.0.8/PKG-INFO` & `edpm-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edpm
-Version: 1.0.8
+Version: 1.0.9
 Summary: EIC Development Package Manager
 Home-page: https://github.com/eic/edpm
 Author: Dmitry Romanov
 Author-email: romanov@jlab.org
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `edpm-1.0.8/README.md` & `edpm-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `edpm-1.0.8/edpm/__init__.py` & `edpm-1.0.9/edpm/__init__.py`

 * *Files identical despite different names*

### Comparing `edpm-1.0.8/edpm/cli/clean.py` & `edpm-1.0.9/edpm/cli/clean.py`

 * *Files identical despite different names*

### Comparing `edpm-1.0.8/edpm/cli/config.py` & `edpm-1.0.9/edpm/cli/config.py`

 * *Files identical despite different names*

### Comparing `edpm-1.0.8/edpm/cli/env.py` & `edpm-1.0.9/edpm/cli/env.py`

 * *Files identical despite different names*

### Comparing `edpm-1.0.8/edpm/cli/example_command.py` & `edpm-1.0.9/edpm/cli/example_command.py`

 * *Files identical despite different names*

### Comparing `edpm-1.0.8/edpm/cli/find.py` & `edpm-1.0.9/edpm/cli/find.py`

 * *Files identical despite different names*

### Comparing `edpm-1.0.8/edpm/cli/info.py` & `edpm-1.0.9/edpm/cli/info.py`

 * *Files identical despite different names*

### Comparing `edpm-1.0.8/edpm/cli/install.py` & `edpm-1.0.9/edpm/cli/install.py`

 * *Files identical despite different names*

### Comparing `edpm-1.0.8/edpm/cli/mergedb.py` & `edpm-1.0.9/edpm/cli/mergedb.py`

 * *Files identical despite different names*

### Comparing `edpm-1.0.8/edpm/cli/pwd.py` & `edpm-1.0.9/edpm/cli/pwd.py`

 * *Files identical despite different names*

### Comparing `edpm-1.0.8/edpm/cli/req.py` & `edpm-1.0.9/edpm/cli/req.py`

 * *Files identical despite different names*

### Comparing `edpm-1.0.8/edpm/cli/rm.py` & `edpm-1.0.9/edpm/cli/rm.py`

 * *Files identical despite different names*

### Comparing `edpm-1.0.8/edpm/cli/set.py` & `edpm-1.0.9/edpm/cli/set.py`

 * *Files identical despite different names*

### Comparing `edpm-1.0.8/edpm/engine/api.py` & `edpm-1.0.9/edpm/engine/api.py`

 * *Files identical despite different names*

### Comparing `edpm-1.0.8/edpm/engine/commands.py` & `edpm-1.0.9/edpm/engine/commands.py`

 * *Files identical despite different names*

### Comparing `edpm-1.0.8/edpm/engine/convig.py` & `edpm-1.0.9/edpm/engine/convig.py`

 * *Files identical despite different names*

### Comparing `edpm-1.0.8/edpm/engine/db.py` & `edpm-1.0.9/edpm/engine/db.py`

 * *Files identical despite different names*

### Comparing `edpm-1.0.8/edpm/engine/env_gen.py` & `edpm-1.0.9/edpm/engine/env_gen.py`

 * *Files identical despite different names*

### Comparing `edpm-1.0.8/edpm/engine/git_cmake_recipe.py` & `edpm-1.0.9/edpm/engine/git_cmake_recipe.py`

 * *Files identical despite different names*

### Comparing `edpm-1.0.8/edpm/engine/output.py` & `edpm-1.0.9/edpm/engine/output.py`

 * *Files identical despite different names*

### Comparing `edpm-1.0.8/edpm/engine/recipe.py` & `edpm-1.0.9/edpm/engine/recipe.py`

 * *Files identical despite different names*

### Comparing `edpm-1.0.8/edpm/engine/recipe_manager.py` & `edpm-1.0.9/edpm/engine/recipe_manager.py`

 * *Files identical despite different names*

### Comparing `edpm-1.0.8/edpm/recipes/acts.py` & `edpm-1.0.9/edpm/recipes/acts.py`

 * *Files identical despite different names*

### Comparing `edpm-1.0.8/edpm/recipes/clhep.py` & `edpm-1.0.9/edpm/recipes/clhep.py`

 * *Files identical despite different names*

### Comparing `edpm-1.0.8/edpm/recipes/dd4hep.py` & `edpm-1.0.9/edpm/recipes/dd4hep.py`

 * *Files identical despite different names*

### Comparing `edpm-1.0.8/edpm/recipes/detector.py` & `edpm-1.0.9/edpm/recipes/detector.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         # Set initial values for parent class and self
         super(EpicDetectorRecipe, self).__init__('detector')
         self.clone_command = ''             # is set during self.setup(...)
         self.build_cmd = ''                 # is set during self.setup(...)
         self.config['branch'] = 'main'
         self.config['branch_epic'] = self.config['branch']
         self.config['branch_ip6'] = 'master'    # https://github.com/eic/ip6/issues/1
-        self.required_deps = ['clhep', 'root', 'hepmc3', 'dd4hep', 'acts']
+        self.required_deps = ['clhep', 'eigen3', 'root', 'hepmc3', 'podio', 'edm4hep', 'geant4', 'acts',  'dd4hep']
         self.config['repo_address_epic'] = 'https://github.com/eic/epic'
         self.config['repo_address_ip6'] = 'https://github.com/eic/ip6'
 
     def setup(self, db):
         """Sets all variables like source dirs, build dirs, etc"""
 
         #
```

### Comparing `edpm-1.0.8/edpm/recipes/edm4hep.py` & `edpm-1.0.9/edpm/recipes/edm4hep.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         """
         Installs Genfit track fitting framework
         """
 
         # Set initial values for parent class and self
         super(Edm4HepRecipe, self).__init__('edm4hep')                          # This name will be used in edpm commands
         self.config['branch'] = 'v00-05'                                        # The branch or tag to be cloned (-b flag)
-        self.required_deps = ['podio']
+        self.required_deps = ['clhep', 'eigen3', 'root', 'hepmc3', 'podio', 'edm4hep', 'geant4', 'acts', 'dd4hep', 'jana2']
         self.config['repo_address'] = 'https://github.com/key4hep/EDM4hep'      # Repo address
         self.config['cmake_flags'] = '-DUSE_EXTERNAL_CATCH2=OFF'
         self.config['cxx_standard'] = 17
 
     @staticmethod
     def gen_env(data):
         """Generates environments to be set"""
```

### Comparing `edpm-1.0.8/edpm/recipes/eicrecon.py` & `edpm-1.0.9/edpm/recipes/eicrecon.py`

 * *Files identical despite different names*

### Comparing `edpm-1.0.8/edpm/recipes/eigen3.py` & `edpm-1.0.9/edpm/recipes/eigen3.py`

 * *Files identical despite different names*

### Comparing `edpm-1.0.8/edpm/recipes/geant4.py` & `edpm-1.0.9/edpm/recipes/geant4.py`

 * *Files identical despite different names*

### Comparing `edpm-1.0.8/edpm/recipes/hepmc3.py` & `edpm-1.0.9/edpm/recipes/hepmc3.py`

 * *Files identical despite different names*

### Comparing `edpm-1.0.8/edpm/recipes/jana2.py` & `edpm-1.0.9/edpm/recipes/jana2.py`

 * *Files identical despite different names*

### Comparing `edpm-1.0.8/edpm/recipes/npdet.py` & `edpm-1.0.9/edpm/recipes/npdet.py`

 * *Files identical despite different names*

### Comparing `edpm-1.0.8/edpm/recipes/phasm.py` & `edpm-1.0.9/edpm/recipes/phasm.py`

 * *Files identical despite different names*

### Comparing `edpm-1.0.8/edpm/recipes/podio.py` & `edpm-1.0.9/edpm/recipes/podio.py`

 * *Files identical despite different names*

### Comparing `edpm-1.0.8/edpm/recipes/pythia8.py` & `edpm-1.0.9/edpm/recipes/pythia8.py`

 * *Files identical despite different names*

### Comparing `edpm-1.0.8/edpm/recipes/root.py` & `edpm-1.0.9/edpm/recipes/root.py`

 * *Files identical despite different names*

### Comparing `edpm-1.0.8/edpm.egg-info/PKG-INFO` & `edpm-1.0.9/edpm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edpm
-Version: 1.0.8
+Version: 1.0.9
 Summary: EIC Development Package Manager
 Home-page: https://github.com/eic/edpm
 Author: Dmitry Romanov
 Author-email: romanov@jlab.org
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `edpm-1.0.8/edpm.egg-info/SOURCES.txt` & `edpm-1.0.9/edpm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edpm-1.0.8/pip_readme.md` & `edpm-1.0.9/pip_readme.md`

 * *Files identical despite different names*

### Comparing `edpm-1.0.8/setup.py` & `edpm-1.0.9/setup.py`

 * *Files identical despite different names*

