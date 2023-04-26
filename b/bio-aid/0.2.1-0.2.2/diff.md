# Comparing `tmp/bio-aid-0.2.1.tar.gz` & `tmp/bio-aid-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bio-aid-0.2.1.tar", last modified: Tue Apr 25 21:19:45 2023, max compression
+gzip compressed data, was "bio-aid-0.2.2.tar", last modified: Tue Apr 25 21:36:29 2023, max compression
```

## Comparing `bio-aid-0.2.1.tar` & `bio-aid-0.2.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 21:19:45.319845 bio-aid-0.2.1/
-drwxrwxrwx   0        0        0        0 2023-04-25 21:19:45.286658 bio-aid-0.2.1/BioAid/
--rw-rw-rw-   0        0        0     2304 2023-04-25 21:07:27.000000 bio-aid-0.2.1/BioAid/Kmers.py
-drwxrwxrwx   0        0        0        0 2023-04-25 21:19:45.294790 bio-aid-0.2.1/BioAid/MMBSearchTK/
--rw-rw-rw-   0        0        0     7151 2023-03-01 22:48:52.000000 bio-aid-0.2.1/BioAid/MMBSearchTK/AnnoMMBS.py
--rw-rw-rw-   0        0        0      269 2023-03-01 22:48:19.000000 bio-aid-0.2.1/BioAid/MMBSearchTK/__init__.py
--rw-rw-rw-   0        0        0     1372 2023-03-01 22:49:16.000000 bio-aid-0.2.1/BioAid/MMBSearchTK/makeMMBSearchRef.py
--rw-rw-rw-   0        0        0      500 2023-03-01 22:45:30.000000 bio-aid-0.2.1/BioAid/__init__.py
--rw-rw-rw-   0        0        0     6676 2023-04-25 21:18:57.000000 bio-aid-0.2.1/BioAid/base.py
--rw-rw-rw-   0        0        0     4862 2023-03-01 22:41:08.000000 bio-aid-0.2.1/BioAid/complexity.py
-drwxrwxrwx   0        0        0        0 2023-04-25 21:19:45.295012 bio-aid-0.2.1/BioAid/deepSeqInsH/
--rw-rw-rw-   0        0        0      193 2023-03-01 22:49:33.000000 bio-aid-0.2.1/BioAid/deepSeqInsH/__init__.py
--rw-rw-rw-   0        0        0     2817 2023-03-01 22:50:23.000000 bio-aid-0.2.1/BioAid/deepSeqInsH/annoInsH.py
--rw-rw-rw-   0        0        0     1505 2023-04-25 21:06:56.000000 bio-aid-0.2.1/BioAid/diluter.py
--rw-rw-rw-   0        0        0     1202 2023-03-01 22:53:18.000000 bio-aid-0.2.1/BioAid/makeMMBSearchRef.py
--rw-rw-rw-   0        0        0     2062 2023-04-25 21:08:23.000000 bio-aid-0.2.1/BioAid/paralleltools.py
--rw-rw-rw-   0        0        0      870 2023-03-01 22:43:38.000000 bio-aid-0.2.1/BioAid/popDub.py
--rw-rw-rw-   0        0        0     5169 2023-03-01 22:44:42.000000 bio-aid-0.2.1/BioAid/repeatSearch.py
-drwxrwxrwx   0        0        0        0 2023-04-25 21:19:45.295012 bio-aid-0.2.1/BioAid/variantTK/
--rw-rw-rw-   0        0        0      193 2023-03-01 22:45:37.000000 bio-aid-0.2.1/BioAid/variantTK/__init__.py
--rw-rw-rw-   0        0        0    10973 2023-03-01 22:48:01.000000 bio-aid-0.2.1/BioAid/variantTK/variants.py
--rw-rw-rw-   0        0        0     1101 2023-03-01 22:53:18.000000 bio-aid-0.2.1/LICENSE
--rw-rw-rw-   0        0        0      612 2023-04-25 21:19:45.311773 bio-aid-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     3164 2023-03-01 22:53:18.000000 bio-aid-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-25 21:19:45.311773 bio-aid-0.2.1/bio_aid.egg-info/
--rw-rw-rw-   0        0        0      612 2023-04-25 21:19:45.000000 bio-aid-0.2.1/bio_aid.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      581 2023-04-25 21:19:45.000000 bio-aid-0.2.1/bio_aid.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 21:19:45.000000 bio-aid-0.2.1/bio_aid.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-04-25 21:19:45.000000 bio-aid-0.2.1/bio_aid.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-25 21:19:45.000000 bio-aid-0.2.1/bio_aid.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-25 21:19:45.320006 bio-aid-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      994 2023-04-25 21:18:25.000000 bio-aid-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 21:36:29.083058 bio-aid-0.2.2/
+drwxrwxrwx   0        0        0        0 2023-04-25 21:36:29.057922 bio-aid-0.2.2/BioAid/
+-rw-rw-rw-   0        0        0     2304 2023-04-25 21:07:27.000000 bio-aid-0.2.2/BioAid/Kmers.py
+drwxrwxrwx   0        0        0        0 2023-04-25 21:36:29.057922 bio-aid-0.2.2/BioAid/MMBSearchTK/
+-rw-rw-rw-   0        0        0     7151 2023-03-01 22:48:52.000000 bio-aid-0.2.2/BioAid/MMBSearchTK/AnnoMMBS.py
+-rw-rw-rw-   0        0        0      269 2023-03-01 22:48:19.000000 bio-aid-0.2.2/BioAid/MMBSearchTK/__init__.py
+-rw-rw-rw-   0        0        0     1372 2023-03-01 22:49:16.000000 bio-aid-0.2.2/BioAid/MMBSearchTK/makeMMBSearchRef.py
+-rw-rw-rw-   0        0        0      500 2023-03-01 22:45:30.000000 bio-aid-0.2.2/BioAid/__init__.py
+-rw-rw-rw-   0        0        0     6676 2023-04-25 21:18:57.000000 bio-aid-0.2.2/BioAid/base.py
+-rw-rw-rw-   0        0        0     4862 2023-03-01 22:41:08.000000 bio-aid-0.2.2/BioAid/complexity.py
+drwxrwxrwx   0        0        0        0 2023-04-25 21:36:29.066109 bio-aid-0.2.2/BioAid/deepSeqInsH/
+-rw-rw-rw-   0        0        0      193 2023-03-01 22:49:33.000000 bio-aid-0.2.2/BioAid/deepSeqInsH/__init__.py
+-rw-rw-rw-   0        0        0     2693 2023-04-25 21:33:33.000000 bio-aid-0.2.2/BioAid/deepSeqInsH/annoInsH.py
+-rw-rw-rw-   0        0        0     1505 2023-04-25 21:06:56.000000 bio-aid-0.2.2/BioAid/diluter.py
+-rw-rw-rw-   0        0        0     1202 2023-03-01 22:53:18.000000 bio-aid-0.2.2/BioAid/makeMMBSearchRef.py
+-rw-rw-rw-   0        0        0     2062 2023-04-25 21:08:23.000000 bio-aid-0.2.2/BioAid/paralleltools.py
+-rw-rw-rw-   0        0        0      870 2023-03-01 22:43:38.000000 bio-aid-0.2.2/BioAid/popDub.py
+-rw-rw-rw-   0        0        0     5169 2023-03-01 22:44:42.000000 bio-aid-0.2.2/BioAid/repeatSearch.py
+drwxrwxrwx   0        0        0        0 2023-04-25 21:36:29.066248 bio-aid-0.2.2/BioAid/variantTK/
+-rw-rw-rw-   0        0        0      193 2023-03-01 22:45:37.000000 bio-aid-0.2.2/BioAid/variantTK/__init__.py
+-rw-rw-rw-   0        0        0    10973 2023-03-01 22:48:01.000000 bio-aid-0.2.2/BioAid/variantTK/variants.py
+-rw-rw-rw-   0        0        0     1101 2023-03-01 22:53:18.000000 bio-aid-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0      612 2023-04-25 21:36:29.083058 bio-aid-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3164 2023-03-01 22:53:18.000000 bio-aid-0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-25 21:36:29.083058 bio-aid-0.2.2/bio_aid.egg-info/
+-rw-rw-rw-   0        0        0      612 2023-04-25 21:36:28.000000 bio-aid-0.2.2/bio_aid.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      581 2023-04-25 21:36:28.000000 bio-aid-0.2.2/bio_aid.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 21:36:28.000000 bio-aid-0.2.2/bio_aid.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-04-25 21:36:28.000000 bio-aid-0.2.2/bio_aid.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-25 21:36:28.000000 bio-aid-0.2.2/bio_aid.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-25 21:36:29.083058 bio-aid-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      994 2023-04-25 21:36:07.000000 bio-aid-0.2.2/setup.py
```

### Comparing `bio-aid-0.2.1/BioAid/Kmers.py` & `bio-aid-0.2.2/BioAid/Kmers.py`

 * *Files identical despite different names*

### Comparing `bio-aid-0.2.1/BioAid/MMBSearchTK/AnnoMMBS.py` & `bio-aid-0.2.2/BioAid/MMBSearchTK/AnnoMMBS.py`

 * *Files identical despite different names*

### Comparing `bio-aid-0.2.1/BioAid/MMBSearchTK/makeMMBSearchRef.py` & `bio-aid-0.2.2/BioAid/MMBSearchTK/makeMMBSearchRef.py`

 * *Files identical despite different names*

### Comparing `bio-aid-0.2.1/BioAid/base.py` & `bio-aid-0.2.2/BioAid/base.py`

 * *Files identical despite different names*

### Comparing `bio-aid-0.2.1/BioAid/complexity.py` & `bio-aid-0.2.2/BioAid/complexity.py`

 * *Files identical despite different names*

### Comparing `bio-aid-0.2.1/BioAid/deepSeqInsH/annoInsH.py` & `bio-aid-0.2.2/BioAid/deepSeqInsH/annoInsH.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,26 +4,21 @@
 ## Contents:
 ## dataFrameImport
 ## matchSequence
 ## findReadLength
 ## trimseq
 ## classify
 
-import sys
-import pysam
 import regex as re
 import os
 import pandas as pd
-import matplotlib.pyplot as plt
-import seaborn as sns
-import numpy as np
-from joblib import Parallel, delayed
-
 
 def dataFrameImport(directory,datatype = 'sam'):
+  import pysam
+
   #This function imports all files inside of the specified DIR path into two lists; of panda DF and sample names
   frames_list_samples = []
   sample_names = []
 
   counter=1
 
   #import all files in the directory
```

### Comparing `bio-aid-0.2.1/BioAid/diluter.py` & `bio-aid-0.2.2/BioAid/diluter.py`

 * *Files identical despite different names*

### Comparing `bio-aid-0.2.1/BioAid/makeMMBSearchRef.py` & `bio-aid-0.2.2/BioAid/makeMMBSearchRef.py`

 * *Files identical despite different names*

### Comparing `bio-aid-0.2.1/BioAid/paralleltools.py` & `bio-aid-0.2.2/BioAid/paralleltools.py`

 * *Files identical despite different names*

### Comparing `bio-aid-0.2.1/BioAid/popDub.py` & `bio-aid-0.2.2/BioAid/popDub.py`

 * *Files identical despite different names*

### Comparing `bio-aid-0.2.1/BioAid/repeatSearch.py` & `bio-aid-0.2.2/BioAid/repeatSearch.py`

 * *Files identical despite different names*

### Comparing `bio-aid-0.2.1/BioAid/variantTK/variants.py` & `bio-aid-0.2.2/BioAid/variantTK/variants.py`

 * *Files identical despite different names*

### Comparing `bio-aid-0.2.1/LICENSE` & `bio-aid-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bio-aid-0.2.1/PKG-INFO` & `bio-aid-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bio-aid
-Version: 0.2.1
+Version: 0.2.2
 Summary: Genetic Analysis Tools
 Author: tvarovski (Jerzy Twarowski)
 Author-email: <tvarovski1@gmail.com>
 Keywords: python,biology,bio,genetics,genomics,NGS
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `bio-aid-0.2.1/README.md` & `bio-aid-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `bio-aid-0.2.1/bio_aid.egg-info/PKG-INFO` & `bio-aid-0.2.2/bio_aid.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bio-aid
-Version: 0.2.1
+Version: 0.2.2
 Summary: Genetic Analysis Tools
 Author: tvarovski (Jerzy Twarowski)
 Author-email: <tvarovski1@gmail.com>
 Keywords: python,biology,bio,genetics,genomics,NGS
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `bio-aid-0.2.1/bio_aid.egg-info/SOURCES.txt` & `bio-aid-0.2.2/bio_aid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bio-aid-0.2.1/setup.py` & `bio-aid-0.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 
-VERSION = '0.2.1'
+VERSION = '0.2.2'
 DESCRIPTION = 'Genetic Analysis Tools'
 LONG_DESCRIPTION = 'A package that contains tools for the analysis of genetic sequence and sequencing related data'
 
 # Setting up
 setup(
     name="bio-aid",
     version=VERSION,
```

