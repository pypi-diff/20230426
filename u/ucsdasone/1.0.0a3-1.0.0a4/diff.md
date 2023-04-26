# Comparing `tmp/ucsdasone-1.0.0a3.tar.gz` & `tmp/ucsdasone-1.0.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ucsdasone-1.0.0a3.tar", last modified: Wed Apr 26 06:26:01 2023, max compression
+gzip compressed data, was "ucsdasone-1.0.0a4.tar", last modified: Wed Apr 26 08:19:32 2023, max compression
```

## Comparing `ucsdasone-1.0.0a3.tar` & `ucsdasone-1.0.0a4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 06:26:01.697245 ucsdasone-1.0.0a3/
--rw-rw-rw-   0        0        0     1087 2023-04-26 02:03:10.000000 ucsdasone-1.0.0a3/LICENSE
--rw-rw-rw-   0        0        0     2207 2023-04-26 06:26:01.695246 ucsdasone-1.0.0a3/PKG-INFO
--rw-rw-rw-   0        0        0       14 2023-04-26 01:59:26.000000 ucsdasone-1.0.0a3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-26 06:26:01.683329 ucsdasone-1.0.0a3/asone/
--rw-rw-rw-   0        0        0      967 2023-04-26 03:56:37.000000 ucsdasone-1.0.0a3/asone/__init__.py
--rw-rw-rw-   0        0        0       64 2023-04-26 03:35:05.000000 ucsdasone-1.0.0a3/asone/__main__.py
--rw-rw-rw-   0        0        0     2727 2023-04-26 03:02:50.000000 ucsdasone-1.0.0a3/asone/scraper.py
--rw-rw-rw-   0        0        0     1081 2023-04-26 06:24:38.000000 ucsdasone-1.0.0a3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-26 06:26:01.697245 ucsdasone-1.0.0a3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-26 06:26:01.693243 ucsdasone-1.0.0a3/ucsdasone.egg-info/
--rw-rw-rw-   0        0        0     2207 2023-04-26 06:26:01.000000 ucsdasone-1.0.0a3/ucsdasone.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      217 2023-04-26 06:26:01.000000 ucsdasone-1.0.0a3/ucsdasone.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 06:26:01.000000 ucsdasone-1.0.0a3/ucsdasone.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-26 06:26:01.000000 ucsdasone-1.0.0a3/ucsdasone.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-26 08:19:32.190304 ucsdasone-1.0.0a4/
+-rw-rw-rw-   0        0        0     1087 2023-04-26 02:03:10.000000 ucsdasone-1.0.0a4/LICENSE
+-rw-rw-rw-   0        0        0     2218 2023-04-26 08:19:32.190304 ucsdasone-1.0.0a4/PKG-INFO
+-rw-rw-rw-   0        0        0       14 2023-04-26 01:59:26.000000 ucsdasone-1.0.0a4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-26 08:19:32.137138 ucsdasone-1.0.0a4/asone/
+-rw-rw-rw-   0        0        0     1135 2023-04-26 08:15:35.000000 ucsdasone-1.0.0a4/asone/__init__.py
+-rw-rw-rw-   0        0        0       64 2023-04-26 03:35:05.000000 ucsdasone-1.0.0a4/asone/__main__.py
+-rw-rw-rw-   0        0        0     3031 2023-04-26 08:17:27.000000 ucsdasone-1.0.0a4/asone/scraper.py
+-rw-rw-rw-   0        0        0     1092 2023-04-26 08:18:14.000000 ucsdasone-1.0.0a4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-26 08:19:32.190304 ucsdasone-1.0.0a4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-26 08:19:32.188297 ucsdasone-1.0.0a4/ucsdasone.egg-info/
+-rw-rw-rw-   0        0        0     2218 2023-04-26 08:19:32.000000 ucsdasone-1.0.0a4/ucsdasone.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2023-04-26 08:19:32.000000 ucsdasone-1.0.0a4/ucsdasone.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 08:19:32.000000 ucsdasone-1.0.0a4/ucsdasone.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-26 08:19:32.000000 ucsdasone-1.0.0a4/ucsdasone.egg-info/top_level.txt
```

### Comparing `ucsdasone-1.0.0a3/LICENSE` & `ucsdasone-1.0.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `ucsdasone-1.0.0a3/PKG-INFO` & `ucsdasone-1.0.0a4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ucsdasone
-Version: 1.0.0a3
-Summary: An API wrapper and web scraper for the UCSD AS One grade archive
+Version: 1.0.0a4
+Summary: An API wrapper and web scraper for the UCSD AS One instructor grade archive
 Author-email: Jacob Lee <Jacob.J.Lee@outlook.com>
 License: MIT License
         
         Copyright (c) 2023 Jacob Lee
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `ucsdasone-1.0.0a3/asone/__init__.py` & `ucsdasone-1.0.0a4/asone/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import argparse
 from importlib import metadata
+import pathlib
 
 from .scraper import GradeArchive
 
 
 NAME = metadata.metadata("ucsdasone")["name"]
 VERSION = metadata.version("ucsdasone")
 
@@ -16,14 +17,15 @@
         version=f"{NAME} {VERSION}"
     )
     parser.add_argument("-q", "--quarter", type=str)
     parser.add_argument("-y", "--year", type=int)
     parser.add_argument("-i", "--instructor", type=str)
     parser.add_argument("-s", "--subject", type=str)
     parser.add_argument("-c", "--code", type=str)
+    parser.add_argument("-o", "--output", type=str)
 
     return parser
 
 
 def main() -> None:
     parser = _parser()
     args = parser.parse_args()
@@ -31,9 +33,13 @@
     archive = GradeArchive(
         quarter=args.quarter,
         year=args.year,
         instructor=args.instructor,
         subject=args.subject,
         code=args.code
     )
+    dataframe = archive.data()
 
-    print(archive.data())
+    if args.output:
+        archive.export(args.output)
+
+    print(dataframe.to_string())
```

### Comparing `ucsdasone-1.0.0a3/asone/scraper.py` & `ucsdasone-1.0.0a4/asone/scraper.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 """
 
 import datetime
+import pathlib
 import re
 import typing
 
 import pandas as pd
 import requests
 
 
@@ -70,31 +71,42 @@
         self.form_data = {
             "quarter": self.quarter,
             "year": str(self.year),
             "instructor": self.instructor,
             "subject": self.subject,
             "courseNumber": self.code
         }
-        
-    def request(self) -> requests.Response:
-        """
-        :return:
-        """
-        return requests.post(self.address, self.form_data, timeout=100)
+        self.response = requests.post(self.address, self.form_data, timeout=100)
 
     def data(self) -> pd.DataFrame:
         """
         :return:
         """
-        with self.request() as response:
-            try:
-                dfs = pd.read_html(response.text)
-            except ValueError:
-                return pd.DataFrame()
+        try:
+            dfs = pd.read_html(self.response.text)
+        except ValueError:
+            return pd.DataFrame()
 
         assert len(dfs) == 1
         dataframe = dfs[0]
 
         columns = ["A", "B", "C", "D", "F", "W", "P", "NP"]
         dataframe[columns] = dataframe[columns].applymap(lambda x: float(x.strip("%")))
 
         return dataframe
+
+    def export(self, path: typing.Union[str, pathlib.Path]) -> pathlib.Path:
+        """
+
+        :param path:
+        :return:
+        """
+        path = pathlib.Path(path)
+        dataframe = self.data()
+
+        if path.suffix == ".csv":
+            dataframe.to_csv(path)
+        else:
+            with open(path, "w", encoding="utf-8") as file:
+                dataframe.to_string(file)
+
+        return path
```

### Comparing `ucsdasone-1.0.0a3/pyproject.toml` & `ucsdasone-1.0.0a4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ucsdasone"
-version = "1.0.0-a.3"
-description = "An API wrapper and web scraper for the UCSD AS One grade archive"
+version = "1.0.0-a.4"
+description = "An API wrapper and web scraper for the UCSD AS One instructor grade archive"
 readme = "README.md"
 authors = [ { name = "Jacob Lee", email = "Jacob.J.Lee@outlook.com" } ]
 license = { file = "LICENSE" }
 classifiers = [
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
```

### Comparing `ucsdasone-1.0.0a3/ucsdasone.egg-info/PKG-INFO` & `ucsdasone-1.0.0a4/ucsdasone.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ucsdasone
-Version: 1.0.0a3
-Summary: An API wrapper and web scraper for the UCSD AS One grade archive
+Version: 1.0.0a4
+Summary: An API wrapper and web scraper for the UCSD AS One instructor grade archive
 Author-email: Jacob Lee <Jacob.J.Lee@outlook.com>
 License: MIT License
         
         Copyright (c) 2023 Jacob Lee
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

