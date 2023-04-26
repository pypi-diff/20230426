# Comparing `tmp/fhirsearchhelper-0.0.4.tar.gz` & `tmp/fhirsearchhelper-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fhirsearchhelper-0.0.4.tar", last modified: Wed Apr 26 15:12:10 2023, max compression
+gzip compressed data, was "fhirsearchhelper-0.0.5.tar", last modified: Wed Apr 26 15:18:48 2023, max compression
```

## Comparing `fhirsearchhelper-0.0.4.tar` & `fhirsearchhelper-0.0.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 astevens37 (1977913256) ICL\Domain Users (429306830)        0 2023-04-26 15:12:10.721091 fhirsearchhelper-0.0.4/
--rw-r--r--   0 astevens37 (1977913256) ICL\Domain Users (429306830)     1070 2022-09-06 16:49:23.000000 fhirsearchhelper-0.0.4/LICENSE
--rw-r--r--   0 astevens37 (1977913256) ICL\Domain Users (429306830)     4915 2023-04-26 15:12:10.720867 fhirsearchhelper-0.0.4/PKG-INFO
--rw-r--r--   0 astevens37 (1977913256) ICL\Domain Users (429306830)     2783 2023-04-25 13:59:42.000000 fhirsearchhelper-0.0.4/README.md
-drwxr-xr-x   0 astevens37 (1977913256) ICL\Domain Users (429306830)        0 2023-04-26 15:12:10.713049 fhirsearchhelper-0.0.4/fhirsearchhelper/
--rw-r--r--   0 astevens37 (1977913256) ICL\Domain Users (429306830)       32 2023-04-26 15:11:44.000000 fhirsearchhelper-0.0.4/fhirsearchhelper/__init__.py
-drwxr-xr-x   0 astevens37 (1977913256) ICL\Domain Users (429306830)        0 2023-04-26 15:12:10.716615 fhirsearchhelper-0.0.4/fhirsearchhelper/capabilitystatements/
--rw-r--r--   0 astevens37 (1977913256) ICL\Domain Users (429306830)        0 2023-04-19 20:55:07.000000 fhirsearchhelper-0.0.4/fhirsearchhelper/capabilitystatements/__init__.py
-drwxr-xr-x   0 astevens37 (1977913256) ICL\Domain Users (429306830)        0 2023-04-26 15:12:10.718605 fhirsearchhelper-0.0.4/fhirsearchhelper/helpers/
--rw-r--r--   0 astevens37 (1977913256) ICL\Domain Users (429306830)        0 2022-09-06 16:51:47.000000 fhirsearchhelper-0.0.4/fhirsearchhelper/helpers/__init__.py
--rw-r--r--   0 astevens37 (1977913256) ICL\Domain Users (429306830)     1925 2023-04-25 12:11:40.000000 fhirsearchhelper-0.0.4/fhirsearchhelper/helpers/capabilitystatement.py
--rw-r--r--   0 astevens37 (1977913256) ICL\Domain Users (429306830)     2907 2023-04-25 12:21:50.000000 fhirsearchhelper-0.0.4/fhirsearchhelper/helpers/fhirfilter.py
--rw-r--r--   0 astevens37 (1977913256) ICL\Domain Users (429306830)     2079 2023-04-25 12:40:19.000000 fhirsearchhelper-0.0.4/fhirsearchhelper/helpers/gapanalysis.py
--rw-r--r--   0 astevens37 (1977913256) ICL\Domain Users (429306830)     3368 2023-04-25 13:54:48.000000 fhirsearchhelper-0.0.4/fhirsearchhelper/main.py
-drwxr-xr-x   0 astevens37 (1977913256) ICL\Domain Users (429306830)        0 2023-04-26 15:12:10.720179 fhirsearchhelper-0.0.4/fhirsearchhelper/models/
--rw-r--r--   0 astevens37 (1977913256) ICL\Domain Users (429306830)        0 2022-09-06 17:51:34.000000 fhirsearchhelper-0.0.4/fhirsearchhelper/models/__init__.py
--rw-r--r--   0 astevens37 (1977913256) ICL\Domain Users (429306830)      382 2023-04-19 21:10:05.000000 fhirsearchhelper-0.0.4/fhirsearchhelper/models/models.py
-drwxr-xr-x   0 astevens37 (1977913256) ICL\Domain Users (429306830)        0 2023-04-26 15:12:10.716280 fhirsearchhelper-0.0.4/fhirsearchhelper.egg-info/
--rw-r--r--   0 astevens37 (1977913256) ICL\Domain Users (429306830)     4915 2023-04-26 15:12:10.000000 fhirsearchhelper-0.0.4/fhirsearchhelper.egg-info/PKG-INFO
--rw-r--r--   0 astevens37 (1977913256) ICL\Domain Users (429306830)      569 2023-04-26 15:12:10.000000 fhirsearchhelper-0.0.4/fhirsearchhelper.egg-info/SOURCES.txt
--rw-r--r--   0 astevens37 (1977913256) ICL\Domain Users (429306830)        1 2023-04-26 15:12:10.000000 fhirsearchhelper-0.0.4/fhirsearchhelper.egg-info/dependency_links.txt
--rw-r--r--   0 astevens37 (1977913256) ICL\Domain Users (429306830)       60 2023-04-26 15:12:10.000000 fhirsearchhelper-0.0.4/fhirsearchhelper.egg-info/requires.txt
--rw-r--r--   0 astevens37 (1977913256) ICL\Domain Users (429306830)       17 2023-04-26 15:12:10.000000 fhirsearchhelper-0.0.4/fhirsearchhelper.egg-info/top_level.txt
--rw-r--r--   0 astevens37 (1977913256) ICL\Domain Users (429306830)     2044 2023-04-26 15:11:50.000000 fhirsearchhelper-0.0.4/pyproject.toml
--rw-r--r--   0 astevens37 (1977913256) ICL\Domain Users (429306830)       38 2023-04-26 15:12:10.721161 fhirsearchhelper-0.0.4/setup.cfg
+drwxr-xr-x   0 astevens37 (1977913256) ICL\Domain Users (429306830)        0 2023-04-26 15:18:48.752640 fhirsearchhelper-0.0.5/
+-rw-r--r--   0 astevens37 (1977913256) ICL\Domain Users (429306830)     1070 2022-09-06 16:49:23.000000 fhirsearchhelper-0.0.5/LICENSE
+-rw-r--r--   0 astevens37 (1977913256) ICL\Domain Users (429306830)     4915 2023-04-26 15:18:48.752428 fhirsearchhelper-0.0.5/PKG-INFO
+-rw-r--r--   0 astevens37 (1977913256) ICL\Domain Users (429306830)     2783 2023-04-25 13:59:42.000000 fhirsearchhelper-0.0.5/README.md
+drwxr-xr-x   0 astevens37 (1977913256) ICL\Domain Users (429306830)        0 2023-04-26 15:18:48.744884 fhirsearchhelper-0.0.5/fhirsearchhelper/
+-rw-r--r--   0 astevens37 (1977913256) ICL\Domain Users (429306830)       32 2023-04-26 15:11:44.000000 fhirsearchhelper-0.0.5/fhirsearchhelper/__init__.py
+drwxr-xr-x   0 astevens37 (1977913256) ICL\Domain Users (429306830)        0 2023-04-26 15:18:48.747754 fhirsearchhelper-0.0.5/fhirsearchhelper/capabilitystatements/
+-rw-r--r--   0 astevens37 (1977913256) ICL\Domain Users (429306830)        0 2023-04-19 20:55:07.000000 fhirsearchhelper-0.0.5/fhirsearchhelper/capabilitystatements/__init__.py
+drwxr-xr-x   0 astevens37 (1977913256) ICL\Domain Users (429306830)        0 2023-04-26 15:18:48.750401 fhirsearchhelper-0.0.5/fhirsearchhelper/helpers/
+-rw-r--r--   0 astevens37 (1977913256) ICL\Domain Users (429306830)        0 2022-09-06 16:51:47.000000 fhirsearchhelper-0.0.5/fhirsearchhelper/helpers/__init__.py
+-rw-r--r--   0 astevens37 (1977913256) ICL\Domain Users (429306830)     1928 2023-04-26 15:17:55.000000 fhirsearchhelper-0.0.5/fhirsearchhelper/helpers/capabilitystatement.py
+-rw-r--r--   0 astevens37 (1977913256) ICL\Domain Users (429306830)     2912 2023-04-26 15:18:02.000000 fhirsearchhelper-0.0.5/fhirsearchhelper/helpers/fhirfilter.py
+-rw-r--r--   0 astevens37 (1977913256) ICL\Domain Users (429306830)     2082 2023-04-26 15:18:09.000000 fhirsearchhelper-0.0.5/fhirsearchhelper/helpers/gapanalysis.py
+-rw-r--r--   0 astevens37 (1977913256) ICL\Domain Users (429306830)     3371 2023-04-26 15:18:21.000000 fhirsearchhelper-0.0.5/fhirsearchhelper/main.py
+drwxr-xr-x   0 astevens37 (1977913256) ICL\Domain Users (429306830)        0 2023-04-26 15:18:48.751709 fhirsearchhelper-0.0.5/fhirsearchhelper/models/
+-rw-r--r--   0 astevens37 (1977913256) ICL\Domain Users (429306830)        0 2022-09-06 17:51:34.000000 fhirsearchhelper-0.0.5/fhirsearchhelper/models/__init__.py
+-rw-r--r--   0 astevens37 (1977913256) ICL\Domain Users (429306830)      381 2023-04-26 15:18:15.000000 fhirsearchhelper-0.0.5/fhirsearchhelper/models/models.py
+drwxr-xr-x   0 astevens37 (1977913256) ICL\Domain Users (429306830)        0 2023-04-26 15:18:48.746896 fhirsearchhelper-0.0.5/fhirsearchhelper.egg-info/
+-rw-r--r--   0 astevens37 (1977913256) ICL\Domain Users (429306830)     4915 2023-04-26 15:18:48.000000 fhirsearchhelper-0.0.5/fhirsearchhelper.egg-info/PKG-INFO
+-rw-r--r--   0 astevens37 (1977913256) ICL\Domain Users (429306830)      569 2023-04-26 15:18:48.000000 fhirsearchhelper-0.0.5/fhirsearchhelper.egg-info/SOURCES.txt
+-rw-r--r--   0 astevens37 (1977913256) ICL\Domain Users (429306830)        1 2023-04-26 15:18:48.000000 fhirsearchhelper-0.0.5/fhirsearchhelper.egg-info/dependency_links.txt
+-rw-r--r--   0 astevens37 (1977913256) ICL\Domain Users (429306830)       60 2023-04-26 15:18:48.000000 fhirsearchhelper-0.0.5/fhirsearchhelper.egg-info/requires.txt
+-rw-r--r--   0 astevens37 (1977913256) ICL\Domain Users (429306830)       17 2023-04-26 15:18:48.000000 fhirsearchhelper-0.0.5/fhirsearchhelper.egg-info/top_level.txt
+-rw-r--r--   0 astevens37 (1977913256) ICL\Domain Users (429306830)     2044 2023-04-26 15:14:22.000000 fhirsearchhelper-0.0.5/pyproject.toml
+-rw-r--r--   0 astevens37 (1977913256) ICL\Domain Users (429306830)       38 2023-04-26 15:18:48.752711 fhirsearchhelper-0.0.5/setup.cfg
```

### Comparing `fhirsearchhelper-0.0.4/LICENSE` & `fhirsearchhelper-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fhirsearchhelper-0.0.4/PKG-INFO` & `fhirsearchhelper-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fhirsearchhelper
-Version: 0.0.4
+Version: 0.0.5
 Summary: A package to help FHIR searching with needed search parameters are not available
 Author-email: Andrew Stevens <andrew.stevens@gtri.gatech.edu>
 Maintainer-email: Andrew Stevens <andrew.stevens@gtri.gatech.edu>
 License: MIT License
         
         Copyright (c) 2022 Andrew Stevens
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fhirsearchhelper Version: 0.0.4 Summary: A package
+Metadata-Version: 2.1 Name: fhirsearchhelper Version: 0.0.5 Summary: A package
 to help FHIR searching with needed search parameters are not available Author-
 email: Andrew Stevens
 stevens@gtri.gatech.edu> Maintainer-email: Andrew Stevens
 stevens@gtri.gatech.edu> License: MIT License Copyright (c) 2022 Andrew Stevens
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
```

### Comparing `fhirsearchhelper-0.0.4/README.md` & `fhirsearchhelper-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `fhirsearchhelper-0.0.4/fhirsearchhelper/helpers/capabilitystatement.py` & `fhirsearchhelper-0.0.5/fhirsearchhelper/helpers/capabilitystatement.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 '''File to handle all operations around a CapabilityStatement'''
 
-from fhir.resources.R4B.capabilitystatement import CapabilityStatement
-import requests
-from pathlib import Path
 import os
+from pathlib import Path
+
+import requests
+from fhir.resources.R4B.capabilitystatement import CapabilityStatement
 
-from models.models import SupportedSearchParams
+from ..models.models import SupportedSearchParams
 
 
 def load_capability_statement(url: str = None, file_path: str  = None) -> CapabilityStatement: # type: ignore
     '''Function to load a CapabilityStatement into memory'''
 
     if not url and not file_path:
         raise ValueError('You need to pass a url, an option to specify a preloaded CapabilityStatement, or a file path.')
```

### Comparing `fhirsearchhelper-0.0.4/fhirsearchhelper/helpers/fhirfilter.py` & `fhirsearchhelper-0.0.5/fhirsearchhelper/helpers/fhirfilter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 '''File to perform filtering of returned FHIR resources using output from gap analysis'''
 
+from copy import deepcopy
+
 from fhir.resources.R4B.bundle import Bundle
 from fhir.resources.R4B.fhirtypes import BundleEntryType
-from models.models import QuerySearchParams
-from copy import deepcopy
+
+from ..models.models import QuerySearchParams
+
 
 def filter_bundle(input_bundle: Bundle, search_params: QuerySearchParams, gap_analysis_output: list[str]) -> Bundle:
     '''Function that takes an input bundle, the original search params, and the output from the gap analysis to filter a Bundle'''
 
     returned_resources: list[BundleEntryType] = input_bundle.entry
     filtered_entries: list[BundleEntryType] = []
     output_bundle: Bundle = deepcopy(input_bundle)
```

### Comparing `fhirsearchhelper-0.0.4/fhirsearchhelper/helpers/gapanalysis.py` & `fhirsearchhelper-0.0.5/fhirsearchhelper/helpers/gapanalysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 '''File to perform the search parameter gap analysis'''
 
-from models.models import SupportedSearchParams, QuerySearchParams
-
 from fhir.resources.R4B.capabilitystatement import CapabilityStatementRestResourceSearchParam
 
+from ..models.models import QuerySearchParams, SupportedSearchParams
+
+
 def run_gap_analysis(supported_search_params: list[SupportedSearchParams], query_search_params: QuerySearchParams) -> list[str]:
     resource_type = query_search_params.resourceType
 
     resouce_supported_search_params: SupportedSearchParams = list(filter(lambda x: x.resourceType == resource_type, supported_search_params))[0]
 
     query_params_names = list(query_search_params.searchParams.keys())
     temp_supported_params_names: list[str] = [rsc.name for rsc in resouce_supported_search_params.searchParams]
```

### Comparing `fhirsearchhelper-0.0.4/fhirsearchhelper/main.py` & `fhirsearchhelper-0.0.5/fhirsearchhelper/main.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 '''Main file for entrypoint to package'''
 
-from fhir.resources.R4B.capabilitystatement import CapabilityStatement
-from fhir.resources.R4B.bundle import Bundle
 import requests
+from fhir.resources.R4B.bundle import Bundle
+from fhir.resources.R4B.capabilitystatement import CapabilityStatement
 
-from helpers.capabilitystatement import load_capability_statement, get_supported_search_params
-
-from models.models import QuerySearchParams, SupportedSearchParams
-from helpers.gapanalysis import run_gap_analysis
-from helpers.fhirfilter import filter_bundle
+from .helpers.capabilitystatement import get_supported_search_params, load_capability_statement
+from .helpers.fhirfilter import filter_bundle
+from .helpers.gapanalysis import run_gap_analysis
+from .models.models import QuerySearchParams, SupportedSearchParams
 
 
 def run_fhir_query(base_url: str = None, query_headers: dict[str, str] = None, resource_type: str = None, search_params: QuerySearchParams = None, query: str = None, # type: ignore
                    capability_statement_file: str = None, capability_statement_url: str = None) -> Bundle | None: # type: ignore
     '''
     Entry function to run FHIR query using a CapabilityStatement and returning filtered resources
     WARNING: There is currently not a way to use a CapabilityStatement out of the box. See README.md of source for details.
```

### Comparing `fhirsearchhelper-0.0.4/fhirsearchhelper.egg-info/PKG-INFO` & `fhirsearchhelper-0.0.5/fhirsearchhelper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fhirsearchhelper
-Version: 0.0.4
+Version: 0.0.5
 Summary: A package to help FHIR searching with needed search parameters are not available
 Author-email: Andrew Stevens <andrew.stevens@gtri.gatech.edu>
 Maintainer-email: Andrew Stevens <andrew.stevens@gtri.gatech.edu>
 License: MIT License
         
         Copyright (c) 2022 Andrew Stevens
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fhirsearchhelper Version: 0.0.4 Summary: A package
+Metadata-Version: 2.1 Name: fhirsearchhelper Version: 0.0.5 Summary: A package
 to help FHIR searching with needed search parameters are not available Author-
 email: Andrew Stevens
 stevens@gtri.gatech.edu> Maintainer-email: Andrew Stevens
 stevens@gtri.gatech.edu> License: MIT License Copyright (c) 2022 Andrew Stevens
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
```

### Comparing `fhirsearchhelper-0.0.4/fhirsearchhelper.egg-info/SOURCES.txt` & `fhirsearchhelper-0.0.5/fhirsearchhelper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fhirsearchhelper-0.0.4/pyproject.toml` & `fhirsearchhelper-0.0.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "fhirsearchhelper"  # Required
-version = "0.0.4"  # Required
+version = "0.0.5"  # Required
 description = "A package to help FHIR searching with needed search parameters are not available"  # Optional
 readme = "README.md" # Optional
 requires-python = ">=3.10"
 license = {file = "LICENSE"}
 keywords = ["fhir", "fhirsearching"]  # Optional
 authors = [
   {name = "Andrew Stevens", email = "andrew.stevens@gtri.gatech.edu" } # Optional
```

