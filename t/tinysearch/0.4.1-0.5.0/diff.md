# Comparing `tmp/tinysearch-0.4.1.tar.gz` & `tmp/tinysearch-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinysearch-0.4.1.tar", last modified: Sun Apr 23 12:19:46 2023, max compression
+gzip compressed data, was "tinysearch-0.5.0.tar", last modified: Wed Apr 26 07:50:14 2023, max compression
```

## Comparing `tinysearch-0.4.1.tar` & `tinysearch-0.5.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11357 2023-04-23 12:19:29.850110 tinysearch-0.4.1/LICENSE
--rw-r--r--   0        0        0     3189 2023-04-23 12:19:29.850110 tinysearch-0.4.1/README.md
--rw-r--r--   0        0        0     1044 2023-04-23 12:19:46.750129 tinysearch-0.4.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-23 12:19:29.854110 tinysearch-0.4.1/tinysearch/__init__.py
--rw-r--r--   0        0        0     1392 2023-04-23 12:19:29.854110 tinysearch-0.4.1/tinysearch/analyzer.py
--rw-r--r--   0        0        0        0 2023-04-23 12:19:29.854110 tinysearch-0.4.1/tinysearch/base/__init__.py
--rw-r--r--   0        0        0      775 2023-04-23 12:19:29.854110 tinysearch-0.4.1/tinysearch/base/analyzer.py
--rw-r--r--   0        0        0     1464 2023-04-23 12:19:29.854110 tinysearch-0.4.1/tinysearch/document.py
--rw-r--r--   0        0        0     1178 2023-04-23 12:19:29.854110 tinysearch-0.4.1/tinysearch/index.py
--rw-r--r--   0        0        0     3479 2023-04-23 12:19:29.854110 tinysearch-0.4.1/tinysearch/search.py
--rw-r--r--   0        0        0     3690 1970-01-01 00:00:00.000000 tinysearch-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-26 07:50:03.012814 tinysearch-0.5.0/LICENSE
+-rw-r--r--   0        0        0     3873 2023-04-26 07:50:03.016814 tinysearch-0.5.0/README.md
+-rw-r--r--   0        0        0     1044 2023-04-26 07:50:14.125016 tinysearch-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-26 07:50:03.016814 tinysearch-0.5.0/tinysearch/__init__.py
+-rw-r--r--   0        0        0     1230 2023-04-26 07:50:03.016814 tinysearch-0.5.0/tinysearch/analyzer.py
+-rw-r--r--   0        0        0        0 2023-04-26 07:50:03.016814 tinysearch-0.5.0/tinysearch/base/__init__.py
+-rw-r--r--   0        0        0      775 2023-04-26 07:50:03.016814 tinysearch-0.5.0/tinysearch/base/analyzer.py
+-rw-r--r--   0        0        0     1464 2023-04-26 07:50:03.016814 tinysearch-0.5.0/tinysearch/document.py
+-rw-r--r--   0        0        0     1154 2023-04-26 07:50:03.016814 tinysearch-0.5.0/tinysearch/index.py
+-rw-r--r--   0        0        0     3537 2023-04-26 07:50:03.016814 tinysearch-0.5.0/tinysearch/search.py
+-rw-r--r--   0        0        0     4374 1970-01-01 00:00:00.000000 tinysearch-0.5.0/PKG-INFO
```

### Comparing `tinysearch-0.4.1/LICENSE` & `tinysearch-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tinysearch-0.4.1/README.md` & `tinysearch-0.5.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -105,34 +105,57 @@
 ```mermaid
 gantt
 title Search time for different dataset sizes [s]
 dateFormat X
 axisFormat %s
 
 section 100
-0.1, terms=1 : 0, 0.1s
-0.1, terms=2 : 0, 0.1s
-0.1, terms=3 : 0, 0.1s
+0.0, terms=1 : 0, 0.0s
+0.0, terms=2 : 0, 0.0s
+0.0, terms=3 : 0, 0.0s
 
 section 1000
-0.6, terms=1 : 0, 0.6s
-0.6, terms=2 : 0, 0.6s
-0.5, terms=3 : 0, 0.5s
+0.3, terms=1 : 0, 0.3s
+0.2, terms=2 : 0, 0.2s
+0.3, terms=3 : 0, 0.3s
 
 section 10000
-5.2, terms=1 : 0, 5.2s
-4.9, terms=2 : 0, 4.9s
-4.9, terms=3 : 0, 4.9s
+2.7, terms=1 : 0, 2.7s
+2.7, terms=2 : 0, 2.7s
+2.7, terms=3 : 0, 2.7s
 
 section 52478
-26.8, terms=1 : 0, 26.8s
-26.8, terms=2 : 0, 26.8s
-26.8, terms=3 : 0, 26.8s
+15.1, terms=1 : 0, 15.6s
+15.4, terms=2 : 0, 15.1s
+15.6, terms=3 : 0, 15.2s
 ```
 
 Datasets of around 1000 entries might generate reasonable search times,
 which is the intended use case for TinySearch. Still, there is probably
 room for improvement.
 
+## Can we make it faster?
+
+Most time is spent in analyzer, so improving performance means
+improving processing time of the analyzer. The default
+`SimpleEnglishAnalyzer` has already been highly optimized.
+
+The next step to consider is to split the search into two phases:
+indexing and searching. Since analyzer needs to process every document,
+indexing can happen earlier in the process execution and searching when
+the user requests it. This has an additional benefit of indexing once
+and searching multiple times.
+
+```python
+from tinysearch.index import Index
+from tinysearch.search import Search
+
+i = Index(docs)
+
+# ...later...
+s = Search(i, query)
+print(s.results.matches[0])
+```
+
 ## License
 
 See LICENSE.
```

### Comparing `tinysearch-0.4.1/pyproject.toml` & `tinysearch-0.5.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = [
     "search",
     "engine",
 ]
-version = "0.4.1"
+version = "0.5.0"
 
 [project.license]
 text = "Apache-2.0"
 
 [project.urls]
 Homepage = "https://github.com/dmarsic/tinysearch"
```

### Comparing `tinysearch-0.4.1/tinysearch/analyzer.py` & `tinysearch-0.5.0/tinysearch/analyzer.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 """
 Analyzer transforms input text into a token list.
 
 It has a single public method: analyze
 
+analyze method will be called a lot, it needs to be optimized for
+performance as much as possible.
+
 Example usage:
 
     a = Analyzer()
 
     text = "Audacious, original and haunting"
     tokens = a.analyze(text)
 
@@ -23,19 +26,15 @@
 class SimpleEnglishAnalyzer(Analyzer):
     def __init__(self):
         super().__init__()
         self.stemmer = Stemmer.Stemmer("english")
 
     @classmethod
     def remove_nonchars(cls, token: str) -> str:
-        new_chars = []
-        for c in token:
-            if c.isalnum() or c == "-":
-                new_chars.append(c)
-        return ''.join(new_chars)
+        return "".join([c for c in token if c.isalnum() or c == "-"])
 
     @classmethod
     def lower(cls, token: str) -> str:
         return token.lower()
 
     def stem(self, token: str) -> str:
         return self.stemmer.stemWord(token)
@@ -43,15 +42,8 @@
     def analyze(self, text: str) -> List[str]:
         """Transforms input text to a list of tokens."""
 
         # Split on whitespace.
         tokens = re.split(r"\s+", text)
 
         # Apply transformations on each token.
-        new_tokens = []
-        for token in tokens:
-            token = self.remove_nonchars(token)
-            token = self.lower(token)
-            token = self.stem(token)
-            new_tokens.append(token)
-        tokens = new_tokens
-        return tokens
+        return [self.stem(self.lower(self.remove_nonchars(token))) for token in tokens]
```

### Comparing `tinysearch-0.4.1/tinysearch/base/analyzer.py` & `tinysearch-0.5.0/tinysearch/base/analyzer.py`

 * *Files identical despite different names*

### Comparing `tinysearch-0.4.1/tinysearch/document.py` & `tinysearch-0.5.0/tinysearch/document.py`

 * *Files identical despite different names*

### Comparing `tinysearch-0.4.1/tinysearch/index.py` & `tinysearch-0.5.0/tinysearch/index.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,10 +31,9 @@
     def __repr__(self):
         return self.__str__()
 
     def process_docs(self, docs: List[str]) -> List[Document]:
         processed = []
         for doc in docs:
             d = Document(doc, analyzer=self.analyzer)
-            d.analyze()
             processed.append(d)
         return processed
```

### Comparing `tinysearch-0.4.1/tinysearch/search.py` & `tinysearch-0.5.0/tinysearch/search.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     print(s.results.matches[0])
     # Result(doc=..., score=0.20)
 """
 
 from collections import defaultdict
 from dataclasses import dataclass
 from math import log
-from typing import List
+from typing import List, Union
 
 from tinysearch.index import Index
 from tinysearch.document import Document
 from tinysearch.base.analyzer import Analyzer
 from tinysearch.analyzer import SimpleEnglishAnalyzer
 
 
@@ -70,23 +70,23 @@
 
     @property
     def matches(self) -> List[Result]:
         return sorted(self._matches, key=lambda r: r.score, reverse=True)
 
 
 class Search:
-    def __init__(self, docs: List[str], query: str, analyzer: Analyzer = None) -> None:
+    def __init__(self, docs: Union[Index, List[str]], query: str, analyzer: Analyzer = None) -> None:
         if query is None:
             raise ValueError("Query must be text.")
 
         self.analyzer = analyzer if analyzer is not None else SimpleEnglishAnalyzer()
 
         self.query = query
         self.results = Results()
-        self.index = Index(docs, analyzer=self.analyzer)
+        self.index = docs if isinstance(docs, Index) else Index(docs, analyzer=self.analyzer)
         self.search()
 
     def __str__(self):
         return f"Search[query='{self.query}', matches={self.results.count}]"
 
     def __repr__(self):
         return self.__str__()
```

### Comparing `tinysearch-0.4.1/PKG-INFO` & `tinysearch-0.5.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinysearch
-Version: 0.4.1
+Version: 0.5.0
 Summary: Tiny one-phase search engine
 Keywords: search engine
 Author-Email: Domagoj Marsic <dmars@protonmail.com>
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -120,34 +120,57 @@
 ```mermaid
 gantt
 title Search time for different dataset sizes [s]
 dateFormat X
 axisFormat %s
 
 section 100
-0.1, terms=1 : 0, 0.1s
-0.1, terms=2 : 0, 0.1s
-0.1, terms=3 : 0, 0.1s
+0.0, terms=1 : 0, 0.0s
+0.0, terms=2 : 0, 0.0s
+0.0, terms=3 : 0, 0.0s
 
 section 1000
-0.6, terms=1 : 0, 0.6s
-0.6, terms=2 : 0, 0.6s
-0.5, terms=3 : 0, 0.5s
+0.3, terms=1 : 0, 0.3s
+0.2, terms=2 : 0, 0.2s
+0.3, terms=3 : 0, 0.3s
 
 section 10000
-5.2, terms=1 : 0, 5.2s
-4.9, terms=2 : 0, 4.9s
-4.9, terms=3 : 0, 4.9s
+2.7, terms=1 : 0, 2.7s
+2.7, terms=2 : 0, 2.7s
+2.7, terms=3 : 0, 2.7s
 
 section 52478
-26.8, terms=1 : 0, 26.8s
-26.8, terms=2 : 0, 26.8s
-26.8, terms=3 : 0, 26.8s
+15.1, terms=1 : 0, 15.6s
+15.4, terms=2 : 0, 15.1s
+15.6, terms=3 : 0, 15.2s
 ```
 
 Datasets of around 1000 entries might generate reasonable search times,
 which is the intended use case for TinySearch. Still, there is probably
 room for improvement.
 
+## Can we make it faster?
+
+Most time is spent in analyzer, so improving performance means
+improving processing time of the analyzer. The default
+`SimpleEnglishAnalyzer` has already been highly optimized.
+
+The next step to consider is to split the search into two phases:
+indexing and searching. Since analyzer needs to process every document,
+indexing can happen earlier in the process execution and searching when
+the user requests it. This has an additional benefit of indexing once
+and searching multiple times.
+
+```python
+from tinysearch.index import Index
+from tinysearch.search import Search
+
+i = Index(docs)
+
+# ...later...
+s = Search(i, query)
+print(s.results.matches[0])
+```
+
 ## License
 
 See LICENSE.
```

