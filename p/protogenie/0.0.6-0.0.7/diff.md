# Comparing `tmp/protogenie-0.0.6.tar.gz` & `tmp/protogenie-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protogenie-0.0.6.tar", last modified: Tue Apr 25 17:22:02 2023, max compression
+gzip compressed data, was "protogenie-0.0.7.tar", last modified: Tue Apr 25 17:50:25 2023, max compression
```

## Comparing `protogenie-0.0.6.tar` & `protogenie-0.0.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 tclerice  (1000) tclerice  (1000)        0 2023-04-25 17:22:02.559441 protogenie-0.0.6/
--rw-rw-r--   0 tclerice  (1000) tclerice  (1000)     2725 2023-04-25 17:22:02.559441 protogenie-0.0.6/PKG-INFO
--rw-rw-r--   0 tclerice  (1000) tclerice  (1000)     1535 2023-04-25 09:52:20.000000 protogenie-0.0.6/README.md
-drwxrwxr-x   0 tclerice  (1000) tclerice  (1000)        0 2023-04-25 17:22:02.559441 protogenie-0.0.6/protogenie/
--rw-rw-r--   0 tclerice  (1000) tclerice  (1000)        0 2023-04-25 09:52:20.000000 protogenie-0.0.6/protogenie/__init__.py
--rw-rw-r--   0 tclerice  (1000) tclerice  (1000)     8720 2023-04-25 16:47:36.000000 protogenie-0.0.6/protogenie/cli.py
--rw-rw-r--   0 tclerice  (1000) tclerice  (1000)      936 2023-04-25 09:52:20.000000 protogenie-0.0.6/protogenie/cli_utils.py
--rw-rw-r--   0 tclerice  (1000) tclerice  (1000)     7339 2023-04-25 15:22:15.000000 protogenie-0.0.6/protogenie/configs.py
--rw-rw-r--   0 tclerice  (1000) tclerice  (1000)      175 2023-04-25 09:52:20.000000 protogenie-0.0.6/protogenie/defaults.py
--rw-rw-r--   0 tclerice  (1000) tclerice  (1000)    17857 2023-04-25 14:37:24.000000 protogenie-0.0.6/protogenie/dispatch.py
--rw-rw-r--   0 tclerice  (1000) tclerice  (1000)      909 2023-04-25 09:52:20.000000 protogenie-0.0.6/protogenie/io_utils.py
--rw-rw-r--   0 tclerice  (1000) tclerice  (1000)    19994 2023-04-25 17:14:27.000000 protogenie-0.0.6/protogenie/postprocessing.py
--rw-rw-r--   0 tclerice  (1000) tclerice  (1000)     3120 2023-04-25 15:10:20.000000 protogenie-0.0.6/protogenie/reader.py
--rw-rw-r--   0 tclerice  (1000) tclerice  (1000)     1382 2023-04-25 10:48:26.000000 protogenie-0.0.6/protogenie/sentence_matchers.py
--rw-rw-r--   0 tclerice  (1000) tclerice  (1000)     8494 2023-04-25 15:22:15.000000 protogenie-0.0.6/protogenie/splitters.py
--rw-rw-r--   0 tclerice  (1000) tclerice  (1000)     4017 2023-04-25 17:19:07.000000 protogenie-0.0.6/protogenie/toolbox.py
-drwxrwxr-x   0 tclerice  (1000) tclerice  (1000)        0 2023-04-25 17:22:02.559441 protogenie-0.0.6/protogenie.egg-info/
--rw-rw-r--   0 tclerice  (1000) tclerice  (1000)     2725 2023-04-25 17:22:02.000000 protogenie-0.0.6/protogenie.egg-info/PKG-INFO
--rw-rw-r--   0 tclerice  (1000) tclerice  (1000)      508 2023-04-25 17:22:02.000000 protogenie-0.0.6/protogenie.egg-info/SOURCES.txt
--rw-rw-r--   0 tclerice  (1000) tclerice  (1000)        1 2023-04-25 17:22:02.000000 protogenie-0.0.6/protogenie.egg-info/dependency_links.txt
--rw-rw-r--   0 tclerice  (1000) tclerice  (1000)       52 2023-04-25 17:22:02.000000 protogenie-0.0.6/protogenie.egg-info/entry_points.txt
--rw-rw-r--   0 tclerice  (1000) tclerice  (1000)       74 2023-04-25 17:22:02.000000 protogenie-0.0.6/protogenie.egg-info/requires.txt
--rw-rw-r--   0 tclerice  (1000) tclerice  (1000)       11 2023-04-25 17:22:02.000000 protogenie-0.0.6/protogenie.egg-info/top_level.txt
--rw-rw-r--   0 tclerice  (1000) tclerice  (1000)       38 2023-04-25 17:22:02.559441 protogenie-0.0.6/setup.cfg
--rw-rw-r--   0 tclerice  (1000) tclerice  (1000)     3922 2023-04-25 17:21:44.000000 protogenie-0.0.6/setup.py
+drwxrwxr-x   0 tclerice  (1000) tclerice  (1000)        0 2023-04-25 17:50:25.302235 protogenie-0.0.7/
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)     2725 2023-04-25 17:50:25.302235 protogenie-0.0.7/PKG-INFO
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)     1535 2023-04-25 09:52:20.000000 protogenie-0.0.7/README.md
+drwxrwxr-x   0 tclerice  (1000) tclerice  (1000)        0 2023-04-25 17:50:25.302235 protogenie-0.0.7/protogenie/
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)        0 2023-04-25 09:52:20.000000 protogenie-0.0.7/protogenie/__init__.py
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)     8720 2023-04-25 16:47:36.000000 protogenie-0.0.7/protogenie/cli.py
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)      936 2023-04-25 09:52:20.000000 protogenie-0.0.7/protogenie/cli_utils.py
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)     7339 2023-04-25 15:22:15.000000 protogenie-0.0.7/protogenie/configs.py
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)      175 2023-04-25 09:52:20.000000 protogenie-0.0.7/protogenie/defaults.py
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)    17857 2023-04-25 14:37:24.000000 protogenie-0.0.7/protogenie/dispatch.py
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)      909 2023-04-25 09:52:20.000000 protogenie-0.0.7/protogenie/io_utils.py
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)    20054 2023-04-25 17:47:36.000000 protogenie-0.0.7/protogenie/postprocessing.py
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)     3120 2023-04-25 15:10:20.000000 protogenie-0.0.7/protogenie/reader.py
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)     1382 2023-04-25 10:48:26.000000 protogenie-0.0.7/protogenie/sentence_matchers.py
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)     8494 2023-04-25 15:22:15.000000 protogenie-0.0.7/protogenie/splitters.py
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)     4017 2023-04-25 17:19:07.000000 protogenie-0.0.7/protogenie/toolbox.py
+drwxrwxr-x   0 tclerice  (1000) tclerice  (1000)        0 2023-04-25 17:50:25.302235 protogenie-0.0.7/protogenie.egg-info/
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)     2725 2023-04-25 17:50:25.000000 protogenie-0.0.7/protogenie.egg-info/PKG-INFO
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)      508 2023-04-25 17:50:25.000000 protogenie-0.0.7/protogenie.egg-info/SOURCES.txt
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)        1 2023-04-25 17:50:25.000000 protogenie-0.0.7/protogenie.egg-info/dependency_links.txt
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)       52 2023-04-25 17:50:25.000000 protogenie-0.0.7/protogenie.egg-info/entry_points.txt
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)       74 2023-04-25 17:50:25.000000 protogenie-0.0.7/protogenie.egg-info/requires.txt
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)       11 2023-04-25 17:50:25.000000 protogenie-0.0.7/protogenie.egg-info/top_level.txt
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)       38 2023-04-25 17:50:25.302235 protogenie-0.0.7/setup.cfg
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)     3922 2023-04-25 17:50:09.000000 protogenie-0.0.7/setup.py
```

### Comparing `protogenie-0.0.6/PKG-INFO` & `protogenie-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protogenie
-Version: 0.0.6
+Version: 0.0.7
 Summary: Pre-processing of NLP training corpora
 Home-page: https://github.com/ponteineptique/nlp-pie-taggers
 Author: Thibault Clérice
 License: MIT
 Description: 
         Protogenie
         ====================
```

### Comparing `protogenie-0.0.6/README.md` & `protogenie-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `protogenie-0.0.6/protogenie/cli.py` & `protogenie-0.0.7/protogenie/cli.py`

 * *Files identical despite different names*

### Comparing `protogenie-0.0.6/protogenie/cli_utils.py` & `protogenie-0.0.7/protogenie/cli_utils.py`

 * *Files identical despite different names*

### Comparing `protogenie-0.0.6/protogenie/configs.py` & `protogenie-0.0.7/protogenie/configs.py`

 * *Files identical despite different names*

### Comparing `protogenie-0.0.6/protogenie/dispatch.py` & `protogenie-0.0.7/protogenie/dispatch.py`

 * *Files identical despite different names*

### Comparing `protogenie-0.0.6/protogenie/io_utils.py` & `protogenie-0.0.7/protogenie/io_utils.py`

 * *Files identical despite different names*

### Comparing `protogenie-0.0.6/protogenie/postprocessing.py` & `protogenie-0.0.7/protogenie/postprocessing.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,19 @@
     from .configs import CorpusConfiguration
 from .sentence_matchers import SentenceMatcherProto, SentenceRegexpMatcher
 Numeric = Union[int, float]
 
 
 def adhoc_reader(file: TextIO, delimiter: str) -> Iterable[List[str]]:
     for line in file.readlines():
-        yield [x for x in line.strip().split(delimiter) if x]
+        line = line.strip()
+        if line:
+            yield line.split(delimiter)
+        else:
+            yield None
 
 
 class PostProcessing(ABC):
     NodeName = "XML-NODE-LOCAL-NAME"  # Name of the node to match
 
     @abstractmethod
     def apply(self, file_path: str, config: "CorpusConfiguration"):
```

### Comparing `protogenie-0.0.6/protogenie/reader.py` & `protogenie-0.0.7/protogenie/reader.py`

 * *Files identical despite different names*

### Comparing `protogenie-0.0.6/protogenie/sentence_matchers.py` & `protogenie-0.0.7/protogenie/sentence_matchers.py`

 * *Files identical despite different names*

### Comparing `protogenie-0.0.6/protogenie/splitters.py` & `protogenie-0.0.7/protogenie/splitters.py`

 * *Files identical despite different names*

### Comparing `protogenie-0.0.6/protogenie/toolbox.py` & `protogenie-0.0.7/protogenie/toolbox.py`

 * *Files identical despite different names*

### Comparing `protogenie-0.0.6/protogenie.egg-info/PKG-INFO` & `protogenie-0.0.7/protogenie.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protogenie
-Version: 0.0.6
+Version: 0.0.7
 Summary: Pre-processing of NLP training corpora
 Home-page: https://github.com/ponteineptique/nlp-pie-taggers
 Author: Thibault Clérice
 License: MIT
 Description: 
         Protogenie
         ====================
```

### Comparing `protogenie-0.0.6/setup.py` & `protogenie-0.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 # Package meta-data.
 NAME = 'protogenie'
 DESCRIPTION = "Pre-processing of NLP training corpora"
 URL = 'https://github.com/ponteineptique/nlp-pie-taggers'
 AUTHOR = 'Thibault Clérice'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = "0.0.6"
+VERSION = "0.0.7"
 
 # What packages are required for this module to be executed?
 
 with open(os.path.join(here, 'requirements.txt')) as f:
     REQUIRED = f.read().splitlines()
 
 # What packages are optional?
```

