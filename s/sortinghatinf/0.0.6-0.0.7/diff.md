# Comparing `tmp/sortinghatinf-0.0.6.tar.gz` & `tmp/sortinghatinf-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/bobotran/Desktop/Homework/cse234/SortingHatLib/dist/tmpl_356_uz/sortinghatinf-0.0.6.tar", last modified: Sun Dec 12 07:26:48 2021, max compression
+gzip compressed data, was "sortinghatinf-0.0.7.tar", last modified: Wed Apr 26 07:56:21 2023, max compression
```

## Comparing `sortinghatinf-0.0.6.tar` & `sortinghatinf-0.0.7.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxr-x   0 bobotran  (1000) bobotran  (1000)        0 2021-12-12 07:26:48.000000 sortinghatinf-0.0.6/
--rw-rw-r--   0 bobotran  (1000) bobotran  (1000)     3635 2021-12-11 09:41:23.000000 sortinghatinf-0.0.6/README.md
-drwxrwxr-x   0 bobotran  (1000) bobotran  (1000)        0 2021-12-12 07:26:48.000000 sortinghatinf-0.0.6/sortinghatinf.egg-info/
--rw-rw-r--   0 bobotran  (1000) bobotran  (1000)     3979 2021-12-12 07:26:48.000000 sortinghatinf-0.0.6/sortinghatinf.egg-info/PKG-INFO
--rw-rw-r--   0 bobotran  (1000) bobotran  (1000)        1 2021-12-12 07:26:48.000000 sortinghatinf-0.0.6/sortinghatinf.egg-info/dependency_links.txt
--rw-rw-r--   0 bobotran  (1000) bobotran  (1000)       52 2021-12-12 07:26:48.000000 sortinghatinf-0.0.6/sortinghatinf.egg-info/requires.txt
--rw-rw-r--   0 bobotran  (1000) bobotran  (1000)       14 2021-12-12 07:26:48.000000 sortinghatinf-0.0.6/sortinghatinf.egg-info/top_level.txt
--rw-rw-r--   0 bobotran  (1000) bobotran  (1000)      413 2021-12-12 07:26:48.000000 sortinghatinf-0.0.6/sortinghatinf.egg-info/SOURCES.txt
--rw-rw-r--   0 bobotran  (1000) bobotran  (1000)     3979 2021-12-12 07:26:48.000000 sortinghatinf-0.0.6/PKG-INFO
--rw-rw-r--   0 bobotran  (1000) bobotran  (1000)       38 2021-12-12 07:26:48.000000 sortinghatinf-0.0.6/setup.cfg
-drwxrwxr-x   0 bobotran  (1000) bobotran  (1000)        0 2021-12-12 07:26:48.000000 sortinghatinf-0.0.6/sortinghatinf/
--rw-rw-r--   0 bobotran  (1000) bobotran  (1000)    12811 2021-12-11 09:33:39.000000 sortinghatinf-0.0.6/sortinghatinf/pylib.py
-drwxrwxr-x   0 bobotran  (1000) bobotran  (1000)        0 2021-12-12 07:26:48.000000 sortinghatinf-0.0.6/sortinghatinf/resources/
--rw-rw-r--   0 bobotran  (1000) bobotran  (1000)  7649704 2021-11-16 12:31:53.000000 sortinghatinf-0.0.6/sortinghatinf/resources/compressed_rf.pbz2
--rw-rw-r--   0 bobotran  (1000) bobotran  (1000)    62660 2021-11-16 09:42:15.000000 sortinghatinf-0.0.6/sortinghatinf/resources/dictionaryName.pkl
--rw-rw-r--   0 bobotran  (1000) bobotran  (1000)    99103 2021-11-16 09:42:15.000000 sortinghatinf-0.0.6/sortinghatinf/resources/dictionarySample.pkl
--rw-rw-r--   0 bobotran  (1000) bobotran  (1000)      116 2021-12-11 09:27:22.000000 sortinghatinf-0.0.6/sortinghatinf/__init__.py
--rw-rw-r--   0 bobotran  (1000) bobotran  (1000)      647 2021-11-23 03:07:05.000000 sortinghatinf-0.0.6/sortinghatinf/model_loading.py
--rw-rw-r--   0 bobotran  (1000) bobotran  (1000)      684 2021-12-11 09:27:25.000000 sortinghatinf-0.0.6/setup.py
+drwxrwxr-x   0 bobotran  (1000) bobotran  (1000)        0 2023-04-26 07:56:21.856750 sortinghatinf-0.0.7/
+-rw-r--r--   0 bobotran  (1000) bobotran  (1000)    10771 2021-11-02 07:21:27.000000 sortinghatinf-0.0.7/LICENSE
+-rw-rw-r--   0 bobotran  (1000) bobotran  (1000)     3981 2023-04-26 07:56:21.852750 sortinghatinf-0.0.7/PKG-INFO
+-rw-rw-r--   0 bobotran  (1000) bobotran  (1000)     3635 2021-12-11 09:41:23.000000 sortinghatinf-0.0.7/README.md
+-rw-rw-r--   0 bobotran  (1000) bobotran  (1000)       38 2023-04-26 07:56:21.856750 sortinghatinf-0.0.7/setup.cfg
+-rw-rw-r--   0 bobotran  (1000) bobotran  (1000)     1270 2023-04-26 06:30:29.000000 sortinghatinf-0.0.7/setup.py
+drwxrwxr-x   0 bobotran  (1000) bobotran  (1000)        0 2023-04-26 07:56:21.824750 sortinghatinf-0.0.7/sortinghatinf/
+-rw-rw-r--   0 bobotran  (1000) bobotran  (1000)      116 2023-04-26 07:24:31.000000 sortinghatinf-0.0.7/sortinghatinf/__init__.py
+-rw-rw-r--   0 bobotran  (1000) bobotran  (1000)     1249 2022-02-19 01:15:01.000000 sortinghatinf-0.0.7/sortinghatinf/model_loading.py
+-rw-rw-r--   0 bobotran  (1000) bobotran  (1000)    13513 2023-04-26 06:08:22.000000 sortinghatinf-0.0.7/sortinghatinf/pylib.py
+drwxrwxr-x   0 bobotran  (1000) bobotran  (1000)        0 2023-04-26 07:56:21.852750 sortinghatinf-0.0.7/sortinghatinf/resources/
+-rw-rw-r--   0 bobotran  (1000) bobotran  (1000)  7597854 2023-04-26 07:23:49.000000 sortinghatinf-0.0.7/sortinghatinf/resources/compressed_rf.pbz2
+-rw-rw-r--   0 bobotran  (1000) bobotran  (1000)    35549 2023-04-26 07:23:53.000000 sortinghatinf-0.0.7/sortinghatinf/resources/dictionaryName.pkl
+-rw-rw-r--   0 bobotran  (1000) bobotran  (1000)    56070 2023-04-26 07:23:53.000000 sortinghatinf-0.0.7/sortinghatinf/resources/dictionarySample.pkl
+drwxrwxr-x   0 bobotran  (1000) bobotran  (1000)        0 2023-04-26 07:56:21.828750 sortinghatinf-0.0.7/sortinghatinf.egg-info/
+-rw-rw-r--   0 bobotran  (1000) bobotran  (1000)     3981 2023-04-26 07:56:21.000000 sortinghatinf-0.0.7/sortinghatinf.egg-info/PKG-INFO
+-rw-rw-r--   0 bobotran  (1000) bobotran  (1000)      421 2023-04-26 07:56:21.000000 sortinghatinf-0.0.7/sortinghatinf.egg-info/SOURCES.txt
+-rw-rw-r--   0 bobotran  (1000) bobotran  (1000)        1 2023-04-26 07:56:21.000000 sortinghatinf-0.0.7/sortinghatinf.egg-info/dependency_links.txt
+-rw-rw-r--   0 bobotran  (1000) bobotran  (1000)       50 2023-04-26 07:56:21.000000 sortinghatinf-0.0.7/sortinghatinf.egg-info/requires.txt
+-rw-rw-r--   0 bobotran  (1000) bobotran  (1000)       14 2023-04-26 07:56:21.000000 sortinghatinf-0.0.7/sortinghatinf.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `sortinghatinf-0.0.6/README.md` & `sortinghatinf-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `sortinghatinf-0.0.6/sortinghatinf.egg-info/PKG-INFO` & `sortinghatinf-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: sortinghatinf
-Version: 0.0.6
+Version: 0.0.7
 Summary: A library that executes SortingHat feature type inference on Pandas dataframes
 Home-page: https://github.com/bobotran/SortingHatLib
 Author: Vraj Shah
 Author-email: pvn251@gmail.com
 License: MIT
-Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # SortingHatInf
 
 SortingHatInf is a library that implements ML-based feature type inference as seen in the paper [here](https://adalabucsd.github.io/papers/2021_SortingHat_SIGMOD.pdf). Feature type inference is the task of predicting the feature types of the columns of a given dataset.
 
 ## Feature Types
 ### SortingHat
@@ -119,9 +119,7 @@
 # Infer the ARFF feature types.
 # The function `get_feature_types_as_arff()` also returns the SortingHat feature types.
 infer_arff, infer_sh = sortinghatinf.get_feature_types_as_arff(X)
 ```
 
 
 
-
-
```

### Comparing `sortinghatinf-0.0.6/PKG-INFO` & `sortinghatinf-0.0.7/sortinghatinf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: sortinghatinf
-Version: 0.0.6
+Version: 0.0.7
 Summary: A library that executes SortingHat feature type inference on Pandas dataframes
 Home-page: https://github.com/bobotran/SortingHatLib
 Author: Vraj Shah
 Author-email: pvn251@gmail.com
 License: MIT
-Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # SortingHatInf
 
 SortingHatInf is a library that implements ML-based feature type inference as seen in the paper [here](https://adalabucsd.github.io/papers/2021_SortingHat_SIGMOD.pdf). Feature type inference is the task of predicting the feature types of the columns of a given dataset.
 
 ## Feature Types
 ### SortingHat
@@ -119,9 +119,7 @@
 # Infer the ARFF feature types.
 # The function `get_feature_types_as_arff()` also returns the SortingHat feature types.
 infer_arff, infer_sh = sortinghatinf.get_feature_types_as_arff(X)
 ```
 
 
 
-
-
```

### Comparing `sortinghatinf-0.0.6/sortinghatinf/pylib.py` & `sortinghatinf-0.0.7/sortinghatinf/pylib.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+#Copyright 2021 Ryan Tran, Victor Zhu, Arun Kumar
+#
+#Licensed under the Apache License, Version 2.0 (the "License");
+#you may not use this file except in compliance with the License.
+#You may obtain a copy of the License at
+#
+#    http://www.apache.org/licenses/LICENSE-2.0
+#
+#Unless required by applicable law or agreed to in writing, software
+#distributed under the License is distributed on an "AS IS" BASIS,
+#WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#See the License for the specific language governing permissions and
+#limitations under the License.
+
 import pandas as pd
 import numpy as np
 import os
 from pandas.api.types import is_numeric_dtype
 import re
 from nltk.corpus import stopwords 
 from nltk.tokenize import word_tokenize 
@@ -255,15 +269,18 @@
     return data2
 
 
 def load_RF(df):
     """
     Runs the Random Forest Classifier on the given data.
     """
-    y_RF = Pickled_LR_Model.predict(df).tolist()
+    # import pdb; pdb.set_trace()
+    # Avoid sklearn error from mixed column name types
+    arr = df.to_numpy()
+    y_RF = Pickled_LR_Model.predict(arr).tolist()
     return y_RF
 
 ### Public Functions ###
 
 def get_sortinghat_types(df: pd.DataFrame) -> List[str]:
     """
     Returns a list of the predicted SortingHat feature types on the columns of the specified Pandas dataframe
```

