# Comparing `tmp/adaptive-cards-py-0.0.2.tar.gz` & `tmp/adaptive-cards-py-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adaptive-cards-py-0.0.2.tar", last modified: Wed Apr 26 19:04:42 2023, max compression
+gzip compressed data, was "adaptive-cards-py-0.0.3.tar", last modified: Wed Apr 26 19:07:57 2023, max compression
```

## Comparing `adaptive-cards-py-0.0.2.tar` & `adaptive-cards-py-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,28 @@
-drwxr-xr-x   0 dennis    (1000) dennis    (1000)        0 2023-04-26 19:04:42.552104 adaptive-cards-py-0.0.2/
--rw-r--r--   0 dennis    (1000) dennis    (1000)     1068 2023-04-24 18:32:53.000000 adaptive-cards-py-0.0.2/LICENSE
--rw-r--r--   0 dennis    (1000) dennis    (1000)     8379 2023-04-26 19:04:42.542104 adaptive-cards-py-0.0.2/PKG-INFO
--rw-r--r--   0 dennis    (1000) dennis    (1000)     6713 2023-04-26 17:52:15.000000 adaptive-cards-py-0.0.2/README.md
-drwxr-xr-x   0 dennis    (1000) dennis    (1000)        0 2023-04-26 19:04:42.542104 adaptive-cards-py-0.0.2/adaptive_cards/
--rw-r--r--   0 dennis    (1000) dennis    (1000)        0 2023-04-26 18:21:59.000000 adaptive-cards-py-0.0.2/adaptive_cards/__init__.py
--rw-r--r--   0 dennis    (1000) dennis    (1000)     3602 2023-04-25 16:45:04.000000 adaptive-cards-py-0.0.2/adaptive_cards/actions.py
--rw-r--r--   0 dennis    (1000) dennis    (1000)     5180 2023-04-26 18:03:04.000000 adaptive-cards-py-0.0.2/adaptive_cards/card.py
--rw-r--r--   0 dennis    (1000) dennis    (1000)     4402 2023-04-25 16:45:04.000000 adaptive-cards-py-0.0.2/adaptive_cards/card_types.py
--rw-r--r--   0 dennis    (1000) dennis    (1000)     8375 2023-04-25 16:45:04.000000 adaptive-cards-py-0.0.2/adaptive_cards/containers.py
--rw-r--r--   0 dennis    (1000) dennis    (1000)     6013 2023-04-25 16:45:04.000000 adaptive-cards-py-0.0.2/adaptive_cards/elements.py
--rw-r--r--   0 dennis    (1000) dennis    (1000)     5753 2023-04-25 16:45:04.000000 adaptive-cards-py-0.0.2/adaptive_cards/inputs.py
--rw-r--r--   0 dennis    (1000) dennis    (1000)      246 2023-04-25 16:45:04.000000 adaptive-cards-py-0.0.2/adaptive_cards/interface.py
--rw-r--r--   0 dennis    (1000) dennis    (1000)      216 2023-04-25 16:45:04.000000 adaptive-cards-py-0.0.2/adaptive_cards/utils.py
--rw-r--r--   0 dennis    (1000) dennis    (1000)     3140 2023-04-26 17:52:15.000000 adaptive-cards-py-0.0.2/adaptive_cards/validation.py
-drwxr-xr-x   0 dennis    (1000) dennis    (1000)        0 2023-04-26 19:04:42.542104 adaptive-cards-py-0.0.2/adaptive_cards_py.egg-info/
--rw-r--r--   0 dennis    (1000) dennis    (1000)     8379 2023-04-26 19:04:42.000000 adaptive-cards-py-0.0.2/adaptive_cards_py.egg-info/PKG-INFO
--rw-r--r--   0 dennis    (1000) dennis    (1000)      503 2023-04-26 19:04:42.000000 adaptive-cards-py-0.0.2/adaptive_cards_py.egg-info/SOURCES.txt
--rw-r--r--   0 dennis    (1000) dennis    (1000)        1 2023-04-26 19:04:42.000000 adaptive-cards-py-0.0.2/adaptive_cards_py.egg-info/dependency_links.txt
--rw-r--r--   0 dennis    (1000) dennis    (1000)       17 2023-04-26 19:04:42.000000 adaptive-cards-py-0.0.2/adaptive_cards_py.egg-info/requires.txt
--rw-r--r--   0 dennis    (1000) dennis    (1000)       15 2023-04-26 19:04:42.000000 adaptive-cards-py-0.0.2/adaptive_cards_py.egg-info/top_level.txt
--rw-r--r--   0 dennis    (1000) dennis    (1000)      621 2023-04-26 19:04:22.000000 adaptive-cards-py-0.0.2/pyproject.toml
--rw-r--r--   0 dennis    (1000) dennis    (1000)       38 2023-04-26 19:04:42.552104 adaptive-cards-py-0.0.2/setup.cfg
+drwxr-xr-x   0 dennis    (1000) dennis    (1000)        0 2023-04-26 19:07:57.572086 adaptive-cards-py-0.0.3/
+-rw-r--r--   0 dennis    (1000) dennis    (1000)     1068 2023-04-24 18:32:53.000000 adaptive-cards-py-0.0.3/LICENSE
+-rw-r--r--   0 dennis    (1000) dennis    (1000)       41 2023-04-26 19:07:24.000000 adaptive-cards-py-0.0.3/MANIFEST.in
+-rw-r--r--   0 dennis    (1000) dennis    (1000)     8379 2023-04-26 19:07:57.572086 adaptive-cards-py-0.0.3/PKG-INFO
+-rw-r--r--   0 dennis    (1000) dennis    (1000)     6713 2023-04-26 17:52:15.000000 adaptive-cards-py-0.0.3/README.md
+drwxr-xr-x   0 dennis    (1000) dennis    (1000)        0 2023-04-26 19:07:57.572086 adaptive-cards-py-0.0.3/adaptive_cards/
+-rw-r--r--   0 dennis    (1000) dennis    (1000)        0 2023-04-26 18:21:59.000000 adaptive-cards-py-0.0.3/adaptive_cards/__init__.py
+-rw-r--r--   0 dennis    (1000) dennis    (1000)     3602 2023-04-25 16:45:04.000000 adaptive-cards-py-0.0.3/adaptive_cards/actions.py
+-rw-r--r--   0 dennis    (1000) dennis    (1000)     5180 2023-04-26 18:03:04.000000 adaptive-cards-py-0.0.3/adaptive_cards/card.py
+-rw-r--r--   0 dennis    (1000) dennis    (1000)     4402 2023-04-25 16:45:04.000000 adaptive-cards-py-0.0.3/adaptive_cards/card_types.py
+-rw-r--r--   0 dennis    (1000) dennis    (1000)     8375 2023-04-25 16:45:04.000000 adaptive-cards-py-0.0.3/adaptive_cards/containers.py
+-rw-r--r--   0 dennis    (1000) dennis    (1000)     6013 2023-04-25 16:45:04.000000 adaptive-cards-py-0.0.3/adaptive_cards/elements.py
+-rw-r--r--   0 dennis    (1000) dennis    (1000)     5753 2023-04-25 16:45:04.000000 adaptive-cards-py-0.0.3/adaptive_cards/inputs.py
+-rw-r--r--   0 dennis    (1000) dennis    (1000)      246 2023-04-25 16:45:04.000000 adaptive-cards-py-0.0.3/adaptive_cards/interface.py
+-rw-r--r--   0 dennis    (1000) dennis    (1000)      216 2023-04-25 16:45:04.000000 adaptive-cards-py-0.0.3/adaptive_cards/utils.py
+-rw-r--r--   0 dennis    (1000) dennis    (1000)     3140 2023-04-26 17:52:15.000000 adaptive-cards-py-0.0.3/adaptive_cards/validation.py
+drwxr-xr-x   0 dennis    (1000) dennis    (1000)        0 2023-04-26 19:07:57.572086 adaptive-cards-py-0.0.3/adaptive_cards_py.egg-info/
+-rw-r--r--   0 dennis    (1000) dennis    (1000)     8379 2023-04-26 19:07:57.000000 adaptive-cards-py-0.0.3/adaptive_cards_py.egg-info/PKG-INFO
+-rw-r--r--   0 dennis    (1000) dennis    (1000)      591 2023-04-26 19:07:57.000000 adaptive-cards-py-0.0.3/adaptive_cards_py.egg-info/SOURCES.txt
+-rw-r--r--   0 dennis    (1000) dennis    (1000)        1 2023-04-26 19:07:57.000000 adaptive-cards-py-0.0.3/adaptive_cards_py.egg-info/dependency_links.txt
+-rw-r--r--   0 dennis    (1000) dennis    (1000)       17 2023-04-26 19:07:57.000000 adaptive-cards-py-0.0.3/adaptive_cards_py.egg-info/requires.txt
+-rw-r--r--   0 dennis    (1000) dennis    (1000)       15 2023-04-26 19:07:57.000000 adaptive-cards-py-0.0.3/adaptive_cards_py.egg-info/top_level.txt
+drwxr-xr-x   0 dennis    (1000) dennis    (1000)        0 2023-04-26 19:07:57.562086 adaptive-cards-py-0.0.3/examples/
+drwxr-xr-x   0 dennis    (1000) dennis    (1000)        0 2023-04-26 19:07:57.572086 adaptive-cards-py-0.0.3/examples/simple_card/
+-rw-r--r--   0 dennis    (1000) dennis    (1000)     7670 2023-04-26 17:52:15.000000 adaptive-cards-py-0.0.3/examples/simple_card/simple_card.jpg
+-rw-r--r--   0 dennis    (1000) dennis    (1000)    20672 2023-04-26 17:52:15.000000 adaptive-cards-py-0.0.3/examples/simple_card/simple_card_2.jpg
+-rw-r--r--   0 dennis    (1000) dennis    (1000)      621 2023-04-26 19:07:41.000000 adaptive-cards-py-0.0.3/pyproject.toml
+-rw-r--r--   0 dennis    (1000) dennis    (1000)       38 2023-04-26 19:07:57.572086 adaptive-cards-py-0.0.3/setup.cfg
```

### Comparing `adaptive-cards-py-0.0.2/LICENSE` & `adaptive-cards-py-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `adaptive-cards-py-0.0.2/PKG-INFO` & `adaptive-cards-py-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adaptive-cards-py
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python wrapper library for building beautiful adaptive cards
 License: MIT License
         
         Copyright (c) 2023 Dennis Eder
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `adaptive-cards-py-0.0.2/README.md` & `adaptive-cards-py-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `adaptive-cards-py-0.0.2/adaptive_cards/actions.py` & `adaptive-cards-py-0.0.3/adaptive_cards/actions.py`

 * *Files identical despite different names*

### Comparing `adaptive-cards-py-0.0.2/adaptive_cards/card.py` & `adaptive-cards-py-0.0.3/adaptive_cards/card.py`

 * *Files identical despite different names*

### Comparing `adaptive-cards-py-0.0.2/adaptive_cards/card_types.py` & `adaptive-cards-py-0.0.3/adaptive_cards/card_types.py`

 * *Files identical despite different names*

### Comparing `adaptive-cards-py-0.0.2/adaptive_cards/containers.py` & `adaptive-cards-py-0.0.3/adaptive_cards/containers.py`

 * *Files identical despite different names*

### Comparing `adaptive-cards-py-0.0.2/adaptive_cards/elements.py` & `adaptive-cards-py-0.0.3/adaptive_cards/elements.py`

 * *Files identical despite different names*

### Comparing `adaptive-cards-py-0.0.2/adaptive_cards/inputs.py` & `adaptive-cards-py-0.0.3/adaptive_cards/inputs.py`

 * *Files identical despite different names*

### Comparing `adaptive-cards-py-0.0.2/adaptive_cards/validation.py` & `adaptive-cards-py-0.0.3/adaptive_cards/validation.py`

 * *Files identical despite different names*

### Comparing `adaptive-cards-py-0.0.2/adaptive_cards_py.egg-info/PKG-INFO` & `adaptive-cards-py-0.0.3/adaptive_cards_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adaptive-cards-py
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python wrapper library for building beautiful adaptive cards
 License: MIT License
         
         Copyright (c) 2023 Dennis Eder
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `adaptive-cards-py-0.0.2/pyproject.toml` & `adaptive-cards-py-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "adaptive-cards-py"
-version = "0.0.2"
+version = "0.0.3"
 description = "Python wrapper library for building beautiful adaptive cards"
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 readme = "README.md"
```

