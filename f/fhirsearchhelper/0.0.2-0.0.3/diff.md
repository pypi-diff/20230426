# Comparing `tmp/fhirsearchhelper-0.0.2.tar.gz` & `tmp/fhirsearchhelper-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fhirsearchhelper-0.0.2.tar", last modified: Wed Apr 26 15:07:59 2023, max compression
+gzip compressed data, was "fhirsearchhelper-0.0.3.tar", last modified: Wed Apr 26 15:10:38 2023, max compression
```

## Comparing `fhirsearchhelper-0.0.2.tar` & `fhirsearchhelper-0.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 astevens37 (1977913256) ICL\Domain Users (429306830)        0 2023-04-26 15:07:59.493678 fhirsearchhelper-0.0.2/
--rw-r--r--   0 astevens37 (1977913256) ICL\Domain Users (429306830)     1070 2022-09-06 16:49:23.000000 fhirsearchhelper-0.0.2/LICENSE
--rw-r--r--   0 astevens37 (1977913256) ICL\Domain Users (429306830)     4915 2023-04-26 15:07:59.493474 fhirsearchhelper-0.0.2/PKG-INFO
--rw-r--r--   0 astevens37 (1977913256) ICL\Domain Users (429306830)     2783 2023-04-25 13:59:42.000000 fhirsearchhelper-0.0.2/README.md
-drwxr-xr-x   0 astevens37 (1977913256) ICL\Domain Users (429306830)        0 2023-04-26 15:07:59.488119 fhirsearchhelper-0.0.2/fhirsearchhelper/
--rw-r--r--   0 astevens37 (1977913256) ICL\Domain Users (429306830)       43 2023-04-26 15:07:13.000000 fhirsearchhelper-0.0.2/fhirsearchhelper/__init__.py
-drwxr-xr-x   0 astevens37 (1977913256) ICL\Domain Users (429306830)        0 2023-04-26 15:07:59.490359 fhirsearchhelper-0.0.2/fhirsearchhelper/capabilitystatements/
--rw-r--r--   0 astevens37 (1977913256) ICL\Domain Users (429306830)        0 2023-04-19 20:55:07.000000 fhirsearchhelper-0.0.2/fhirsearchhelper/capabilitystatements/__init__.py
--rw-r--r--   0 astevens37 (1977913256) ICL\Domain Users (429306830)     3368 2023-04-25 13:54:48.000000 fhirsearchhelper-0.0.2/fhirsearchhelper/fhirsearchhelper.py
-drwxr-xr-x   0 astevens37 (1977913256) ICL\Domain Users (429306830)        0 2023-04-26 15:07:59.492131 fhirsearchhelper-0.0.2/fhirsearchhelper/helpers/
--rw-r--r--   0 astevens37 (1977913256) ICL\Domain Users (429306830)        0 2022-09-06 16:51:47.000000 fhirsearchhelper-0.0.2/fhirsearchhelper/helpers/__init__.py
--rw-r--r--   0 astevens37 (1977913256) ICL\Domain Users (429306830)     1925 2023-04-25 12:11:40.000000 fhirsearchhelper-0.0.2/fhirsearchhelper/helpers/capabilitystatement.py
--rw-r--r--   0 astevens37 (1977913256) ICL\Domain Users (429306830)     2907 2023-04-25 12:21:50.000000 fhirsearchhelper-0.0.2/fhirsearchhelper/helpers/fhirfilter.py
--rw-r--r--   0 astevens37 (1977913256) ICL\Domain Users (429306830)     2079 2023-04-25 12:40:19.000000 fhirsearchhelper-0.0.2/fhirsearchhelper/helpers/gapanalysis.py
-drwxr-xr-x   0 astevens37 (1977913256) ICL\Domain Users (429306830)        0 2023-04-26 15:07:59.492923 fhirsearchhelper-0.0.2/fhirsearchhelper/models/
--rw-r--r--   0 astevens37 (1977913256) ICL\Domain Users (429306830)        0 2022-09-06 17:51:34.000000 fhirsearchhelper-0.0.2/fhirsearchhelper/models/__init__.py
--rw-r--r--   0 astevens37 (1977913256) ICL\Domain Users (429306830)      382 2023-04-19 21:10:05.000000 fhirsearchhelper-0.0.2/fhirsearchhelper/models/models.py
-drwxr-xr-x   0 astevens37 (1977913256) ICL\Domain Users (429306830)        0 2023-04-26 15:07:59.490032 fhirsearchhelper-0.0.2/fhirsearchhelper.egg-info/
--rw-r--r--   0 astevens37 (1977913256) ICL\Domain Users (429306830)     4915 2023-04-26 15:07:59.000000 fhirsearchhelper-0.0.2/fhirsearchhelper.egg-info/PKG-INFO
--rw-r--r--   0 astevens37 (1977913256) ICL\Domain Users (429306830)      581 2023-04-26 15:07:59.000000 fhirsearchhelper-0.0.2/fhirsearchhelper.egg-info/SOURCES.txt
--rw-r--r--   0 astevens37 (1977913256) ICL\Domain Users (429306830)        1 2023-04-26 15:07:59.000000 fhirsearchhelper-0.0.2/fhirsearchhelper.egg-info/dependency_links.txt
--rw-r--r--   0 astevens37 (1977913256) ICL\Domain Users (429306830)       60 2023-04-26 15:07:59.000000 fhirsearchhelper-0.0.2/fhirsearchhelper.egg-info/requires.txt
--rw-r--r--   0 astevens37 (1977913256) ICL\Domain Users (429306830)       17 2023-04-26 15:07:59.000000 fhirsearchhelper-0.0.2/fhirsearchhelper.egg-info/top_level.txt
--rw-r--r--   0 astevens37 (1977913256) ICL\Domain Users (429306830)     2044 2023-04-26 15:07:43.000000 fhirsearchhelper-0.0.2/pyproject.toml
--rw-r--r--   0 astevens37 (1977913256) ICL\Domain Users (429306830)       38 2023-04-26 15:07:59.493746 fhirsearchhelper-0.0.2/setup.cfg
+drwxr-xr-x   0 astevens37 (1977913256) ICL\Domain Users (429306830)        0 2023-04-26 15:10:38.344992 fhirsearchhelper-0.0.3/
+-rw-r--r--   0 astevens37 (1977913256) ICL\Domain Users (429306830)     1070 2022-09-06 16:49:23.000000 fhirsearchhelper-0.0.3/LICENSE
+-rw-r--r--   0 astevens37 (1977913256) ICL\Domain Users (429306830)     4915 2023-04-26 15:10:38.344689 fhirsearchhelper-0.0.3/PKG-INFO
+-rw-r--r--   0 astevens37 (1977913256) ICL\Domain Users (429306830)     2783 2023-04-25 13:59:42.000000 fhirsearchhelper-0.0.3/README.md
+drwxr-xr-x   0 astevens37 (1977913256) ICL\Domain Users (429306830)        0 2023-04-26 15:10:38.337360 fhirsearchhelper-0.0.3/fhirsearchhelper/
+-rw-r--r--   0 astevens37 (1977913256) ICL\Domain Users (429306830)       48 2023-04-26 15:09:51.000000 fhirsearchhelper-0.0.3/fhirsearchhelper/__init__.py
+drwxr-xr-x   0 astevens37 (1977913256) ICL\Domain Users (429306830)        0 2023-04-26 15:10:38.340942 fhirsearchhelper-0.0.3/fhirsearchhelper/capabilitystatements/
+-rw-r--r--   0 astevens37 (1977913256) ICL\Domain Users (429306830)        0 2023-04-19 20:55:07.000000 fhirsearchhelper-0.0.3/fhirsearchhelper/capabilitystatements/__init__.py
+-rw-r--r--   0 astevens37 (1977913256) ICL\Domain Users (429306830)     3368 2023-04-25 13:54:48.000000 fhirsearchhelper-0.0.3/fhirsearchhelper/fhirsearchhelper_main.py
+drwxr-xr-x   0 astevens37 (1977913256) ICL\Domain Users (429306830)        0 2023-04-26 15:10:38.342870 fhirsearchhelper-0.0.3/fhirsearchhelper/helpers/
+-rw-r--r--   0 astevens37 (1977913256) ICL\Domain Users (429306830)        0 2022-09-06 16:51:47.000000 fhirsearchhelper-0.0.3/fhirsearchhelper/helpers/__init__.py
+-rw-r--r--   0 astevens37 (1977913256) ICL\Domain Users (429306830)     1925 2023-04-25 12:11:40.000000 fhirsearchhelper-0.0.3/fhirsearchhelper/helpers/capabilitystatement.py
+-rw-r--r--   0 astevens37 (1977913256) ICL\Domain Users (429306830)     2907 2023-04-25 12:21:50.000000 fhirsearchhelper-0.0.3/fhirsearchhelper/helpers/fhirfilter.py
+-rw-r--r--   0 astevens37 (1977913256) ICL\Domain Users (429306830)     2079 2023-04-25 12:40:19.000000 fhirsearchhelper-0.0.3/fhirsearchhelper/helpers/gapanalysis.py
+drwxr-xr-x   0 astevens37 (1977913256) ICL\Domain Users (429306830)        0 2023-04-26 15:10:38.344071 fhirsearchhelper-0.0.3/fhirsearchhelper/models/
+-rw-r--r--   0 astevens37 (1977913256) ICL\Domain Users (429306830)        0 2022-09-06 17:51:34.000000 fhirsearchhelper-0.0.3/fhirsearchhelper/models/__init__.py
+-rw-r--r--   0 astevens37 (1977913256) ICL\Domain Users (429306830)      382 2023-04-19 21:10:05.000000 fhirsearchhelper-0.0.3/fhirsearchhelper/models/models.py
+drwxr-xr-x   0 astevens37 (1977913256) ICL\Domain Users (429306830)        0 2023-04-26 15:10:38.340517 fhirsearchhelper-0.0.3/fhirsearchhelper.egg-info/
+-rw-r--r--   0 astevens37 (1977913256) ICL\Domain Users (429306830)     4915 2023-04-26 15:10:38.000000 fhirsearchhelper-0.0.3/fhirsearchhelper.egg-info/PKG-INFO
+-rw-r--r--   0 astevens37 (1977913256) ICL\Domain Users (429306830)      586 2023-04-26 15:10:38.000000 fhirsearchhelper-0.0.3/fhirsearchhelper.egg-info/SOURCES.txt
+-rw-r--r--   0 astevens37 (1977913256) ICL\Domain Users (429306830)        1 2023-04-26 15:10:38.000000 fhirsearchhelper-0.0.3/fhirsearchhelper.egg-info/dependency_links.txt
+-rw-r--r--   0 astevens37 (1977913256) ICL\Domain Users (429306830)       60 2023-04-26 15:10:38.000000 fhirsearchhelper-0.0.3/fhirsearchhelper.egg-info/requires.txt
+-rw-r--r--   0 astevens37 (1977913256) ICL\Domain Users (429306830)       17 2023-04-26 15:10:38.000000 fhirsearchhelper-0.0.3/fhirsearchhelper.egg-info/top_level.txt
+-rw-r--r--   0 astevens37 (1977913256) ICL\Domain Users (429306830)     2044 2023-04-26 15:10:22.000000 fhirsearchhelper-0.0.3/pyproject.toml
+-rw-r--r--   0 astevens37 (1977913256) ICL\Domain Users (429306830)       38 2023-04-26 15:10:38.345076 fhirsearchhelper-0.0.3/setup.cfg
```

### Comparing `fhirsearchhelper-0.0.2/LICENSE` & `fhirsearchhelper-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fhirsearchhelper-0.0.2/PKG-INFO` & `fhirsearchhelper-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fhirsearchhelper
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package to help FHIR searching with needed search parameters are not available
 Author-email: Andrew Stevens <andrew.stevens@gtri.gatech.edu>
 Maintainer-email: Andrew Stevens <andrew.stevens@gtri.gatech.edu>
 License: MIT License
         
         Copyright (c) 2022 Andrew Stevens
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fhirsearchhelper Version: 0.0.2 Summary: A package
+Metadata-Version: 2.1 Name: fhirsearchhelper Version: 0.0.3 Summary: A package
 to help FHIR searching with needed search parameters are not available Author-
 email: Andrew Stevens
 stevens@gtri.gatech.edu> Maintainer-email: Andrew Stevens
 stevens@gtri.gatech.edu> License: MIT License Copyright (c) 2022 Andrew Stevens
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
```

### Comparing `fhirsearchhelper-0.0.2/README.md` & `fhirsearchhelper-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `fhirsearchhelper-0.0.2/fhirsearchhelper/fhirsearchhelper.py` & `fhirsearchhelper-0.0.3/fhirsearchhelper/fhirsearchhelper_main.py`

 * *Files identical despite different names*

### Comparing `fhirsearchhelper-0.0.2/fhirsearchhelper/helpers/capabilitystatement.py` & `fhirsearchhelper-0.0.3/fhirsearchhelper/helpers/capabilitystatement.py`

 * *Files identical despite different names*

### Comparing `fhirsearchhelper-0.0.2/fhirsearchhelper/helpers/fhirfilter.py` & `fhirsearchhelper-0.0.3/fhirsearchhelper/helpers/fhirfilter.py`

 * *Files identical despite different names*

### Comparing `fhirsearchhelper-0.0.2/fhirsearchhelper/helpers/gapanalysis.py` & `fhirsearchhelper-0.0.3/fhirsearchhelper/helpers/gapanalysis.py`

 * *Files identical despite different names*

### Comparing `fhirsearchhelper-0.0.2/fhirsearchhelper.egg-info/PKG-INFO` & `fhirsearchhelper-0.0.3/fhirsearchhelper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fhirsearchhelper
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package to help FHIR searching with needed search parameters are not available
 Author-email: Andrew Stevens <andrew.stevens@gtri.gatech.edu>
 Maintainer-email: Andrew Stevens <andrew.stevens@gtri.gatech.edu>
 License: MIT License
         
         Copyright (c) 2022 Andrew Stevens
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fhirsearchhelper Version: 0.0.2 Summary: A package
+Metadata-Version: 2.1 Name: fhirsearchhelper Version: 0.0.3 Summary: A package
 to help FHIR searching with needed search parameters are not available Author-
 email: Andrew Stevens
 stevens@gtri.gatech.edu> Maintainer-email: Andrew Stevens
 stevens@gtri.gatech.edu> License: MIT License Copyright (c) 2022 Andrew Stevens
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
```

### Comparing `fhirsearchhelper-0.0.2/fhirsearchhelper.egg-info/SOURCES.txt` & `fhirsearchhelper-0.0.3/fhirsearchhelper.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 LICENSE
 README.md
 pyproject.toml
 fhirsearchhelper/__init__.py
-fhirsearchhelper/fhirsearchhelper.py
+fhirsearchhelper/fhirsearchhelper_main.py
 fhirsearchhelper.egg-info/PKG-INFO
 fhirsearchhelper.egg-info/SOURCES.txt
 fhirsearchhelper.egg-info/dependency_links.txt
 fhirsearchhelper.egg-info/requires.txt
 fhirsearchhelper.egg-info/top_level.txt
 fhirsearchhelper/capabilitystatements/__init__.py
 fhirsearchhelper/helpers/__init__.py
```

### Comparing `fhirsearchhelper-0.0.2/pyproject.toml` & `fhirsearchhelper-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "fhirsearchhelper"  # Required
-version = "0.0.2"  # Required
+version = "0.0.3"  # Required
 description = "A package to help FHIR searching with needed search parameters are not available"  # Optional
 readme = "README.md" # Optional
 requires-python = ">=3.10"
 license = {file = "LICENSE"}
 keywords = ["fhir", "fhirsearching"]  # Optional
 authors = [
   {name = "Andrew Stevens", email = "andrew.stevens@gtri.gatech.edu" } # Optional
```

