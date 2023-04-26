# Comparing `tmp/spamfilter-0.0.1.tar.gz` & `tmp/spamfilter-0.0.2.tar.gz`

## Comparing `spamfilter-0.0.1.tar` & `spamfilter-0.0.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 spamfilter-0.0.1/MANIFEST.in
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 spamfilter-0.0.1/.vscode/settings.json
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 spamfilter-0.0.1/docs/README.md
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 spamfilter-0.0.1/docs/_config.yml
--rw-r--r--   0        0        0   241098 2020-02-02 00:00:00.000000 spamfilter-0.0.1/docs/assets/icon.png
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 spamfilter-0.0.1/src/spamfilter/__init__.py
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 spamfilter-0.0.1/src/spamfilter/filters/__init__.py
--rw-r--r--   0        0        0     2091 2020-02-02 00:00:00.000000 spamfilter-0.0.1/src/spamfilter/filters/blocklist.py
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 spamfilter-0.0.1/src/spamfilter/filters/blocklist_from_json.py
--rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 spamfilter-0.0.1/src/spamfilter/filters/bypass_detection.py
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 spamfilter-0.0.1/src/spamfilter/filters/capitals.py
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 spamfilter-0.0.1/src/spamfilter/filters/email.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 spamfilter-0.0.1/src/spamfilter/filters/filter.py
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 spamfilter-0.0.1/src/spamfilter/filters/length.py
--rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 spamfilter-0.0.1/src/spamfilter/filters/personal_information.py
--rw-r--r--   0        0        0     2650 2020-02-02 00:00:00.000000 spamfilter-0.0.1/src/spamfilter/filters/symbols.py
--rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 spamfilter-0.0.1/src/spamfilter/filters/word_length.py
--rw-r--r--   0        0        0     2351 2020-02-02 00:00:00.000000 spamfilter-0.0.1/src/spamfilter/machines/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spamfilter-0.0.1/src/spamfilter/premade/__init__.py
--rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 spamfilter-0.0.1/src/spamfilter/premade/chat.py
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 spamfilter-0.0.1/src/spamfilter/result/__init__.py
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 spamfilter-0.0.1/tests/test_filters.py
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 spamfilter-0.0.1/tests/test_premade_chat.py
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 spamfilter-0.0.1/.gitignore
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 spamfilter-0.0.1/LICENSE
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 spamfilter-0.0.1/README.md
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 spamfilter-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3000 2020-02-02 00:00:00.000000 spamfilter-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 spamfilter-0.0.2/MANIFEST.in
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 spamfilter-0.0.2/.vscode/settings.json
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 spamfilter-0.0.2/docs/README.md
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 spamfilter-0.0.2/docs/_config.yml
+-rw-r--r--   0        0        0   241098 2020-02-02 00:00:00.000000 spamfilter-0.0.2/docs/assets/icon.png
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 spamfilter-0.0.2/src/spamfilter/__init__.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 spamfilter-0.0.2/src/spamfilter/filters/__init__.py
+-rw-r--r--   0        0        0     2091 2020-02-02 00:00:00.000000 spamfilter-0.0.2/src/spamfilter/filters/blocklist.py
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 spamfilter-0.0.2/src/spamfilter/filters/blocklist_from_json.py
+-rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 spamfilter-0.0.2/src/spamfilter/filters/bypass_detection.py
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 spamfilter-0.0.2/src/spamfilter/filters/capitals.py
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 spamfilter-0.0.2/src/spamfilter/filters/email.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 spamfilter-0.0.2/src/spamfilter/filters/filter.py
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 spamfilter-0.0.2/src/spamfilter/filters/length.py
+-rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 spamfilter-0.0.2/src/spamfilter/filters/personal_information.py
+-rw-r--r--   0        0        0     2650 2020-02-02 00:00:00.000000 spamfilter-0.0.2/src/spamfilter/filters/symbols.py
+-rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 spamfilter-0.0.2/src/spamfilter/filters/word_length.py
+-rw-r--r--   0        0        0     2351 2020-02-02 00:00:00.000000 spamfilter-0.0.2/src/spamfilter/machines/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spamfilter-0.0.2/src/spamfilter/premade/__init__.py
+-rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 spamfilter-0.0.2/src/spamfilter/premade/chat.py
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 spamfilter-0.0.2/src/spamfilter/result/__init__.py
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 spamfilter-0.0.2/tests/test_filters.py
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 spamfilter-0.0.2/tests/test_premade_chat.py
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 spamfilter-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 spamfilter-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 spamfilter-0.0.2/README.md
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 spamfilter-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3001 2020-02-02 00:00:00.000000 spamfilter-0.0.2/PKG-INFO
```

### Comparing `spamfilter-0.0.1/docs/README.md` & `spamfilter-0.0.2/docs/README.md`

 * *Files identical despite different names*

### Comparing `spamfilter-0.0.1/docs/assets/icon.png` & `spamfilter-0.0.2/docs/assets/icon.png`

 * *Files identical despite different names*

### Comparing `spamfilter-0.0.1/src/spamfilter/filters/__init__.py` & `spamfilter-0.0.2/src/spamfilter/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `spamfilter-0.0.1/src/spamfilter/filters/blocklist.py` & `spamfilter-0.0.2/src/spamfilter/filters/blocklist.py`

 * *Files identical despite different names*

### Comparing `spamfilter-0.0.1/src/spamfilter/filters/bypass_detection.py` & `spamfilter-0.0.2/src/spamfilter/filters/bypass_detection.py`

 * *Files identical despite different names*

### Comparing `spamfilter-0.0.1/src/spamfilter/filters/capitals.py` & `spamfilter-0.0.2/src/spamfilter/filters/capitals.py`

 * *Files identical despite different names*

### Comparing `spamfilter-0.0.1/src/spamfilter/filters/email.py` & `spamfilter-0.0.2/src/spamfilter/filters/email.py`

 * *Files identical despite different names*

### Comparing `spamfilter-0.0.1/src/spamfilter/filters/length.py` & `spamfilter-0.0.2/src/spamfilter/filters/length.py`

 * *Files identical despite different names*

### Comparing `spamfilter-0.0.1/src/spamfilter/filters/personal_information.py` & `spamfilter-0.0.2/src/spamfilter/filters/personal_information.py`

 * *Files identical despite different names*

### Comparing `spamfilter-0.0.1/src/spamfilter/filters/symbols.py` & `spamfilter-0.0.2/src/spamfilter/filters/symbols.py`

 * *Files identical despite different names*

### Comparing `spamfilter-0.0.1/src/spamfilter/filters/word_length.py` & `spamfilter-0.0.2/src/spamfilter/filters/word_length.py`

 * *Files identical despite different names*

### Comparing `spamfilter-0.0.1/src/spamfilter/machines/__init__.py` & `spamfilter-0.0.2/src/spamfilter/machines/__init__.py`

 * *Files identical despite different names*

### Comparing `spamfilter-0.0.1/src/spamfilter/premade/chat.py` & `spamfilter-0.0.2/src/spamfilter/premade/chat.py`

 * *Files identical despite different names*

### Comparing `spamfilter-0.0.1/src/spamfilter/result/__init__.py` & `spamfilter-0.0.2/src/spamfilter/result/__init__.py`

 * *Files identical despite different names*

### Comparing `spamfilter-0.0.1/tests/test_filters.py` & `spamfilter-0.0.2/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `spamfilter-0.0.1/tests/test_premade_chat.py` & `spamfilter-0.0.2/tests/test_premade_chat.py`

 * *Files identical despite different names*

### Comparing `spamfilter-0.0.1/.gitignore` & `spamfilter-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `spamfilter-0.0.1/LICENSE` & `spamfilter-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spamfilter-0.0.1/README.md` & `spamfilter-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `spamfilter-0.0.1/pyproject.toml` & `spamfilter-0.0.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "spamfilter"
-version = "0.0.1"
+version = "0.0.2"
 description = "Create spam mitigation models with ease using fully-customizable, object oriented components."
 readme = "README.md"
 authors = [{ name = "Magnus Schlinsog", email = "magnusschlinsog@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -18,9 +18,9 @@
 dependencies = []
 requires-python = ">=3.9"
 
 [project.optional-dependencies]
 dev = ["pip-tools", "pytest"]
 
 [project.urls]
-GitHub = "https://github.com/realpython/reader"
+GitHub = "https://github.com/mags0ft/spamfilter"
 Homepage = "https://mags0ft.github.io/spamfilter/"
```

### Comparing `spamfilter-0.0.1/PKG-INFO` & `spamfilter-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: spamfilter
-Version: 0.0.1
+Version: 0.0.2
 Summary: Create spam mitigation models with ease using fully-customizable, object oriented components.
-Project-URL: GitHub, https://github.com/realpython/reader
+Project-URL: GitHub, https://github.com/mags0ft/spamfilter
 Project-URL: Homepage, https://mags0ft.github.io/spamfilter/
 Author-email: Magnus Schlinsog <magnusschlinsog@gmail.com>
 License: Copyright 2023 Magnus Schlinsog <magnusschlinsog@gmail.com> and GitHub contributors.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

