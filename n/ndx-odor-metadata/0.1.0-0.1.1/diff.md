# Comparing `tmp/ndx-odor-metadata-0.1.0.tar.gz` & `tmp/ndx-odor-metadata-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ndx-odor-metadata-0.1.0.tar", last modified: Thu Mar 16 23:37:40 2023, max compression
+gzip compressed data, was "ndx-odor-metadata-0.1.1.tar", last modified: Tue Apr 25 21:16:43 2023, max compression
```

## Comparing `ndx-odor-metadata-0.1.0.tar` & `ndx-odor-metadata-0.1.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-16 23:37:40.083467 ndx-odor-metadata-0.1.0/
--rw-rw-rw-   0 root         (0) root         (0)     1517 2023-03-16 23:37:15.000000 ndx-odor-metadata-0.1.0/LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)      299 2023-03-16 23:37:15.000000 ndx-odor-metadata-0.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3931 2023-03-16 23:37:40.083467 ndx-odor-metadata-0.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2835 2023-03-16 23:37:15.000000 ndx-odor-metadata-0.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-16 23:37:40.075466 ndx-odor-metadata-0.1.0/build_utils/
--rw-rw-rw-   0 root         (0) root         (0)      946 2023-03-16 23:37:15.000000 ndx-odor-metadata-0.1.0/build_utils/build_backend.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-16 23:37:40.076466 ndx-odor-metadata-0.1.0/docs/
--rw-rw-rw-   0 root         (0) root         (0)     6600 2023-03-16 23:37:15.000000 ndx-odor-metadata-0.1.0/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)     6196 2023-03-16 23:37:15.000000 ndx-odor-metadata-0.1.0/docs/README.md
--rw-rw-rw-   0 root         (0) root         (0)      804 2023-03-16 23:37:15.000000 ndx-odor-metadata-0.1.0/docs/make.bat
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-16 23:37:40.078466 ndx-odor-metadata-0.1.0/docs/source/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-16 23:37:40.079466 ndx-odor-metadata-0.1.0/docs/source/_static/
--rw-rw-rw-   0 root         (0) root         (0)      365 2023-03-16 23:37:15.000000 ndx-odor-metadata-0.1.0/docs/source/_static/theme_overrides.css
--rw-rw-rw-   0 root         (0) root         (0)     3723 2023-03-16 23:37:15.000000 ndx-odor-metadata-0.1.0/docs/source/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     3970 2023-03-16 23:37:15.000000 ndx-odor-metadata-0.1.0/docs/source/conf_doc_autogen.py
--rw-rw-rw-   0 root         (0) root         (0)      167 2023-03-16 23:37:15.000000 ndx-odor-metadata-0.1.0/docs/source/credits.rst
--rw-rw-rw-   0 root         (0) root         (0)       76 2023-03-16 23:37:15.000000 ndx-odor-metadata-0.1.0/docs/source/description.rst
--rw-rw-rw-   0 root         (0) root         (0)      177 2023-03-16 23:37:15.000000 ndx-odor-metadata-0.1.0/docs/source/format.rst
--rw-rw-rw-   0 root         (0) root         (0)      475 2023-03-16 23:37:15.000000 ndx-odor-metadata-0.1.0/docs/source/index.rst
--rw-rw-rw-   0 root         (0) root         (0)       88 2023-03-16 23:37:15.000000 ndx-odor-metadata-0.1.0/docs/source/release_notes.rst
--rw-rw-rw-   0 root         (0) root         (0)     2295 2023-03-16 23:37:15.000000 ndx-odor-metadata-0.1.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      316 2023-03-16 23:37:40.084467 ndx-odor-metadata-0.1.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-16 23:37:40.080466 ndx-odor-metadata-0.1.0/spec/
--rw-rw-rw-   0 root         (0) root         (0)     4881 2023-03-16 23:37:15.000000 ndx-odor-metadata-0.1.0/spec/ndx-odor-metadata.extensions.yaml
--rw-rw-rw-   0 root         (0) root         (0)      334 2023-03-16 23:37:15.000000 ndx-odor-metadata-0.1.0/spec/ndx-odor-metadata.namespace.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-16 23:37:40.071466 ndx-odor-metadata-0.1.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-16 23:37:40.072466 ndx-odor-metadata-0.1.0/src/pynwb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-16 23:37:40.081466 ndx-odor-metadata-0.1.0/src/pynwb/ndx_odor_metadata/
--rw-rw-rw-   0 root         (0) root         (0)        5 2023-03-16 23:37:15.000000 ndx-odor-metadata-0.1.0/src/pynwb/ndx_odor_metadata/VERSION
--rw-rw-rw-   0 root         (0) root         (0)    15681 2023-03-16 23:37:15.000000 ndx-odor-metadata-0.1.0/src/pynwb/ndx_odor_metadata/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4990 2023-03-16 23:37:15.000000 ndx-odor-metadata-0.1.0/src/pynwb/ndx_odor_metadata/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-16 23:37:40.083467 ndx-odor-metadata-0.1.0/src/pynwb/ndx_odor_metadata.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3931 2023-03-16 23:37:40.000000 ndx-odor-metadata-0.1.0/src/pynwb/ndx_odor_metadata.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      843 2023-03-16 23:37:40.000000 ndx-odor-metadata-0.1.0/src/pynwb/ndx_odor_metadata.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-16 23:37:40.000000 ndx-odor-metadata-0.1.0/src/pynwb/ndx_odor_metadata.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-16 23:37:39.000000 ndx-odor-metadata-0.1.0/src/pynwb/ndx_odor_metadata.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      192 2023-03-16 23:37:40.000000 ndx-odor-metadata-0.1.0/src/pynwb/ndx_odor_metadata.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-03-16 23:37:40.000000 ndx-odor-metadata-0.1.0/src/pynwb/ndx_odor_metadata.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 21:16:43.201173 ndx-odor-metadata-0.1.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1517 2023-04-25 21:16:17.000000 ndx-odor-metadata-0.1.1/LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)      299 2023-04-25 21:16:17.000000 ndx-odor-metadata-0.1.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    11041 2023-04-25 21:16:43.202173 ndx-odor-metadata-0.1.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     9945 2023-04-25 21:16:17.000000 ndx-odor-metadata-0.1.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 21:16:43.193173 ndx-odor-metadata-0.1.1/build_utils/
+-rw-rw-rw-   0 root         (0) root         (0)      946 2023-04-25 21:16:17.000000 ndx-odor-metadata-0.1.1/build_utils/build_backend.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 21:16:43.194172 ndx-odor-metadata-0.1.1/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     6600 2023-04-25 21:16:17.000000 ndx-odor-metadata-0.1.1/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)     6196 2023-04-25 21:16:17.000000 ndx-odor-metadata-0.1.1/docs/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      804 2023-04-25 21:16:17.000000 ndx-odor-metadata-0.1.1/docs/make.bat
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 21:16:43.197173 ndx-odor-metadata-0.1.1/docs/source/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 21:16:43.197173 ndx-odor-metadata-0.1.1/docs/source/_static/
+-rw-rw-rw-   0 root         (0) root         (0)      365 2023-04-25 21:16:17.000000 ndx-odor-metadata-0.1.1/docs/source/_static/theme_overrides.css
+-rw-rw-rw-   0 root         (0) root         (0)     3711 2023-04-25 21:16:17.000000 ndx-odor-metadata-0.1.1/docs/source/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     3970 2023-04-25 21:16:17.000000 ndx-odor-metadata-0.1.1/docs/source/conf_doc_autogen.py
+-rw-rw-rw-   0 root         (0) root         (0)      167 2023-04-25 21:16:17.000000 ndx-odor-metadata-0.1.1/docs/source/credits.rst
+-rw-rw-rw-   0 root         (0) root         (0)       76 2023-04-25 21:16:17.000000 ndx-odor-metadata-0.1.1/docs/source/description.rst
+-rw-rw-rw-   0 root         (0) root         (0)      177 2023-04-25 21:16:17.000000 ndx-odor-metadata-0.1.1/docs/source/format.rst
+-rw-rw-rw-   0 root         (0) root         (0)      475 2023-04-25 21:16:17.000000 ndx-odor-metadata-0.1.1/docs/source/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)       88 2023-04-25 21:16:17.000000 ndx-odor-metadata-0.1.1/docs/source/release_notes.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2329 2023-04-25 21:16:17.000000 ndx-odor-metadata-0.1.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      316 2023-04-25 21:16:43.202173 ndx-odor-metadata-0.1.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 21:16:43.198173 ndx-odor-metadata-0.1.1/spec/
+-rw-rw-rw-   0 root         (0) root         (0)     4881 2023-04-25 21:16:17.000000 ndx-odor-metadata-0.1.1/spec/ndx-odor-metadata.extensions.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      334 2023-04-25 21:16:17.000000 ndx-odor-metadata-0.1.1/spec/ndx-odor-metadata.namespace.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 21:16:43.190172 ndx-odor-metadata-0.1.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 21:16:43.191172 ndx-odor-metadata-0.1.1/src/pynwb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 21:16:43.199173 ndx-odor-metadata-0.1.1/src/pynwb/ndx_odor_metadata/
+-rw-rw-rw-   0 root         (0) root         (0)        5 2023-04-25 21:16:17.000000 ndx-odor-metadata-0.1.1/src/pynwb/ndx_odor_metadata/VERSION
+-rw-rw-rw-   0 root         (0) root         (0)    16052 2023-04-25 21:16:17.000000 ndx-odor-metadata-0.1.1/src/pynwb/ndx_odor_metadata/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7106 2023-04-25 21:16:17.000000 ndx-odor-metadata-0.1.1/src/pynwb/ndx_odor_metadata/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 21:16:43.201173 ndx-odor-metadata-0.1.1/src/pynwb/ndx_odor_metadata.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11041 2023-04-25 21:16:43.000000 ndx-odor-metadata-0.1.1/src/pynwb/ndx_odor_metadata.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      843 2023-04-25 21:16:43.000000 ndx-odor-metadata-0.1.1/src/pynwb/ndx_odor_metadata.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 21:16:43.000000 ndx-odor-metadata-0.1.1/src/pynwb/ndx_odor_metadata.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 21:16:42.000000 ndx-odor-metadata-0.1.1/src/pynwb/ndx_odor_metadata.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      213 2023-04-25 21:16:43.000000 ndx-odor-metadata-0.1.1/src/pynwb/ndx_odor_metadata.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-04-25 21:16:43.000000 ndx-odor-metadata-0.1.1/src/pynwb/ndx_odor_metadata.egg-info/top_level.txt
```

### Comparing `ndx-odor-metadata-0.1.0/LICENSE.txt` & `ndx-odor-metadata-0.1.1/LICENSE.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2022, Tuan Pham
+Copyright (c) 2023, Tuan Pham
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `ndx-odor-metadata-0.1.0/build_utils/build_backend.py` & `ndx-odor-metadata-0.1.1/build_utils/build_backend.py`

 * *Files identical despite different names*

### Comparing `ndx-odor-metadata-0.1.0/docs/Makefile` & `ndx-odor-metadata-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ndx-odor-metadata-0.1.0/docs/README.md` & `ndx-odor-metadata-0.1.1/docs/README.md`

 * *Files identical despite different names*

### Comparing `ndx-odor-metadata-0.1.0/docs/make.bat` & `ndx-odor-metadata-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ndx-odor-metadata-0.1.0/docs/source/conf.py` & `ndx-odor-metadata-0.1.1/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 # For the full list of built-in configuration values, see the documentation:
 # https://www.sphinx-doc.org/en/master/usage/configuration.html
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = 'ndx-odor-metadata'
-copyright = '2022, Tuan Pham'
+copyright = '2023, Tuan Pham'
 author = 'Tuan Pham'
 
-version = '0.1.0'
+version = '0.1.1'
 release = 'alpha'
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = [
     'sphinx.ext.ifconfig',
@@ -86,15 +86,15 @@
 autoclass_content = 'both'
 autodoc_docstring_signature = True
 autodoc_member_order = 'bysource'
 add_function_parentheses = False
 
 
 # -- HTML sphinx options
-html_theme = "sphinx_rtd_theme"
+html_theme = "furo"
 html_theme_path = [sphinx_rtd_theme.get_html_theme_path()]
 
 # LaTeX Sphinx options
 latex_elements = {
     # The paper size ('letterpaper' or 'a4paper').
     'papersize': 'letterpaper',
```

### Comparing `ndx-odor-metadata-0.1.0/docs/source/conf_doc_autogen.py` & `ndx-odor-metadata-0.1.1/docs/source/conf_doc_autogen.py`

 * *Files identical despite different names*

### Comparing `ndx-odor-metadata-0.1.0/pyproject.toml` & `ndx-odor-metadata-0.1.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 readme = 'README.md'
 license = { text =  'BSD-3' }
 requires-python = ">=3.8"
 dependencies = [
     'pynwb>=1.5.0,<3',
     'hdmf>=3.4.7,<4',
     'pubchempy>=1.0.4',
-    'pyyaml>=5.0'
+    'pyyaml>=5.0',
+    'tqdm>=4.0'
 ]
 keywords = [
     'NeurodataWithoutBorders',
     'NWB',
     'nwb-extension',
     'ndx-extension'
 ]
@@ -47,14 +48,15 @@
     "isort>=5.11",
     "pytest-subtests==0.6.0",
     "hdmf-docutils==0.4.4",
     "codespell",
     "ipython",
     "ipykernel",
     "furo",
+    "pre-commit"
     # "dunamai",
     # "packaging",
     # "grayskull",
     # "myst-parser",
     # "twine"
 ]
```

### Comparing `ndx-odor-metadata-0.1.0/spec/ndx-odor-metadata.extensions.yaml` & `ndx-odor-metadata-0.1.1/spec/ndx-odor-metadata.extensions.yaml`

 * *Files identical despite different names*

### Comparing `ndx-odor-metadata-0.1.0/src/pynwb/ndx_odor_metadata/__init__.py` & `ndx-odor-metadata-0.1.1/src/pynwb/ndx_odor_metadata/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -344,14 +344,21 @@
         {
             "name": "accept_plural_chemtype",
             "type": bool,
             "default": True,
             "doc": "Whether to accept plurals when considering if `stim_type` indicates odor/chemical",
         },
         {
+            "name": "source",
+            "type": str,
+            "default": "pubchempy",
+            "doc": "Source to query. Either 'pubchempy' to query using PubChemPy'\
+            'or a CSV file path where such information is already saved",
+        },
+        {
             "name": "query_pubchem",
             "type": bool,
             "default": True,
             "doc": "Whether to use PubChemPy to query at all.",
         },
         {
             "name": "return_synonyms",
@@ -380,15 +387,21 @@
             "Only applicable if `query_pubchem = True`",
         },
         allow_extra=True,
     )
     def add_stimulus(self, **kwargs):
         accept_plural_chemtype = popargs("accept_plural_chemtype", kwargs)
         pcp_request_opts = popargs_to_dict(
-            ["return_synonyms", "warn_notfound_synonym", "error_notfound_cid"], kwargs
+            [
+                "source",
+                "return_synonyms",
+                "warn_notfound_synonym",
+                "error_notfound_cid",
+            ],
+            kwargs,
         )
         pcp_query_opts = popargs_to_dict(
             ["query_pubchem", "overwrite_pubchem_queries"], kwargs
         )
 
         rkwargs = dict(kwargs)
```

### Comparing `ndx-odor-metadata-0.1.0/src/pynwb/ndx_odor_metadata/utils.py` & `ndx-odor-metadata-0.1.1/src/pynwb/ndx_odor_metadata/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,14 @@
+import os
+import time
 import warnings
 from datetime import datetime
 
 import pandas as pd
+from tqdm import tqdm
 
 try:
     import pubchempy as pcp
 
     PCP_AVAILABLE = True
 except ImportError:
     PCP_AVAILABLE = False
@@ -85,28 +88,98 @@
                     + f"\tOr visit <https://pubchem.ncbi.nlm.nih.gov/#query={cid}>"
                 )
                 warnings.warn(warn_mesg)
 
     return metadata, warn_mesg
 
 
+def read_pubchem_from_file(
+    cid,
+    source,
+    check_all_essentials=True,
+    essential_columns=[
+        "pubchem_cid",
+        "chemical_IUPAC",
+        "chemical_SMILES",
+        "chemical_molecular_formula",
+        "chemical_molecular_weight",
+        "is_validated",
+        "validation_details",
+    ],
+):
+    assert os.path.exists(source), (
+        'When `source` is not "pubchempy", '
+        "it needs to be a valid CSV path to a manual file"
+    )
+
+    df_compounds = pd.read_csv(source, dtype={"pubchem_cid": "int"})
+    source_columns = set(df_compounds.columns)
+
+    assert "pubchem_cid" in source_columns, (
+        f'The file "{source}" needs ' "to at least have the column `pubchem_id`"
+    )
+
+    if check_all_essentials:
+        missing = set(essential_columns) - source_columns
+        assert len(missing) == 0, (
+            f'The file "{source}" is missing these ' f"columns = {missing}"
+        )
+
+    chem_meta = df_compounds.query("pubchem_cid == @cid")
+    assert len(chem_meta) == 1, (
+        "Either could not find or found duplicates of "
+        f'`pubchem_cid = {cid}` in the provided file "{source}". '
+        "Only ONE entry of such condition is allowed."
+    )
+
+    chem_meta = chem_meta.iloc[0]
+    chem_meta["pubchem_cid"] = float(chem_meta["pubchem_cid"])
+    return chem_meta
+
+
+def save_pubchem_requests(
+    cid_list, name_list, file_path, sleep_time=0.1, show_progress=True, **kwargs
+):
+    assert len(cid_list) == len(
+        name_list
+    ), "The length of CID and name lists need to match"
+    chem_df = []
+    iter_obj = list(zip(cid_list, name_list))
+    if show_progress:
+        iter_obj = tqdm(iter_obj)
+
+    for cid, name in iter_obj:
+        chem_df.append(request_pubchem(cid, name, source="pubchempy", **kwargs))
+        if sleep_time is not None:
+            time.sleep(sleep_time)
+
+    chem_df = pd.DataFrame(chem_df)
+    chem_df.to_csv(file_path, index=False)
+
+
 def request_pubchem(
     cid,
     name="",
+    source="pubchempy",
     return_synonyms=True,
     synonym_delim="\n",
     warn_notfound_synonym=True,
     error_notfound_cid=True,
 ):
+    cid = int(cid)
+
+    if source.lower() != "pubchempy":
+        chem_meta = read_pubchem_from_file(cid, source)
+        return chem_meta
+
     assert PCP_AVAILABLE, (
         "PubChemPy is not available to query. "
         "Please install with `pip install pubchempy`"
     )
 
-    cid = int(cid)
     err_mesg = f'`pubchempy` had trouble finding CID="{cid}".\n'
 
     chem_meta = dict()
 
     try:
         # try to find from CID
         compound = pcp.Compound.from_cid(cid)
```

### Comparing `ndx-odor-metadata-0.1.0/src/pynwb/ndx_odor_metadata.egg-info/SOURCES.txt` & `ndx-odor-metadata-0.1.1/src/pynwb/ndx_odor_metadata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

