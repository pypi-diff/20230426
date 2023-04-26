# Comparing `tmp/texta-elastic-tools-1.4.1.tar.gz` & `tmp/texta-elastic-tools-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "texta-elastic-tools-1.4.1.tar", last modified: Fri Feb  3 13:09:50 2023, max compression
+gzip compressed data, was "dist/texta-elastic-tools-1.5.0.tar", last modified: Wed Apr 26 14:25:20 2023, max compression
```

## Comparing `texta-elastic-tools-1.4.1.tar` & `texta-elastic-tools-1.5.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-03 13:09:50.582249 texta-elastic-tools-1.4.1/
--rw-rw-rw-   0 root         (0) root         (0)    35062 2023-02-03 13:04:22.000000 texta-elastic-tools-1.4.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      550 2023-02-03 13:09:50.582249 texta-elastic-tools-1.4.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      247 2023-02-03 13:04:22.000000 texta-elastic-tools-1.4.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)        6 2023-02-03 13:05:25.000000 texta-elastic-tools-1.4.1/VERSION
--rw-rw-rw-   0 root         (0) root         (0)      102 2023-02-03 13:04:22.000000 texta-elastic-tools-1.4.1/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-03 13:09:50.582249 texta-elastic-tools-1.4.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      759 2023-02-03 13:04:22.000000 texta-elastic-tools-1.4.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-03 13:09:50.582249 texta-elastic-tools-1.4.1/texta_elastic/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-03 13:04:22.000000 texta-elastic-tools-1.4.1/texta_elastic/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11251 2023-02-03 13:04:22.000000 texta-elastic-tools-1.4.1/texta_elastic/aggregator.py
--rw-rw-rw-   0 root         (0) root         (0)    21412 2023-02-03 13:04:22.000000 texta-elastic-tools-1.4.1/texta_elastic/core.py
--rw-rw-rw-   0 root         (0) root         (0)     1411 2023-02-03 13:04:22.000000 texta-elastic-tools-1.4.1/texta_elastic/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)    14298 2023-02-03 13:04:22.000000 texta-elastic-tools-1.4.1/texta_elastic/document.py
--rw-rw-rw-   0 root         (0) root         (0)      106 2023-02-03 13:04:22.000000 texta-elastic-tools-1.4.1/texta_elastic/enums.py
--rw-rw-rw-   0 root         (0) root         (0)      847 2023-02-03 13:04:22.000000 texta-elastic-tools-1.4.1/texta_elastic/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     5637 2023-02-03 13:04:22.000000 texta-elastic-tools-1.4.1/texta_elastic/mapping_generator.py
--rw-rw-rw-   0 root         (0) root         (0)     2366 2023-02-03 13:04:22.000000 texta-elastic-tools-1.4.1/texta_elastic/mapping_tools.py
--rw-rw-rw-   0 root         (0) root         (0)     3887 2023-02-03 13:04:22.000000 texta-elastic-tools-1.4.1/texta_elastic/query.py
--rw-rw-rw-   0 root         (0) root         (0)    17666 2023-02-03 13:04:22.000000 texta-elastic-tools-1.4.1/texta_elastic/searcher.py
--rw-rw-rw-   0 root         (0) root         (0)     1716 2023-02-03 13:04:22.000000 texta-elastic-tools-1.4.1/texta_elastic/settings.py
--rw-rw-rw-   0 root         (0) root         (0)     5271 2023-02-03 13:04:22.000000 texta-elastic-tools-1.4.1/texta_elastic/spam_detector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-03 13:09:50.582249 texta-elastic-tools-1.4.1/texta_elastic_tools.egg-info/
--rw-r--r--   0 root         (0) root         (0)      550 2023-02-03 13:09:50.000000 texta-elastic-tools-1.4.1/texta_elastic_tools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      618 2023-02-03 13:09:50.000000 texta-elastic-tools-1.4.1/texta_elastic_tools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-03 13:09:50.000000 texta-elastic-tools-1.4.1/texta_elastic_tools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      119 2023-02-03 13:09:50.000000 texta-elastic-tools-1.4.1/texta_elastic_tools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-02-03 13:09:50.000000 texta-elastic-tools-1.4.1/texta_elastic_tools.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 14:25:20.000000 texta-elastic-tools-1.5.0/
+-rw-rw-rw-   0 root         (0) root         (0)    35062 2023-04-26 14:24:11.000000 texta-elastic-tools-1.5.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      570 2023-04-26 14:25:20.000000 texta-elastic-tools-1.5.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      247 2023-04-26 14:24:11.000000 texta-elastic-tools-1.5.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        6 2023-04-26 14:24:11.000000 texta-elastic-tools-1.5.0/VERSION
+-rw-rw-rw-   0 root         (0) root         (0)      102 2023-04-26 14:24:11.000000 texta-elastic-tools-1.5.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-26 14:25:20.000000 texta-elastic-tools-1.5.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      759 2023-04-26 14:24:11.000000 texta-elastic-tools-1.5.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 14:25:20.000000 texta-elastic-tools-1.5.0/texta_elastic/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-26 14:25:09.000000 texta-elastic-tools-1.5.0/texta_elastic/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11251 2023-04-26 14:24:11.000000 texta-elastic-tools-1.5.0/texta_elastic/aggregator.py
+-rw-rw-rw-   0 root         (0) root         (0)    21412 2023-04-26 14:24:11.000000 texta-elastic-tools-1.5.0/texta_elastic/core.py
+-rw-rw-rw-   0 root         (0) root         (0)     1411 2023-04-26 14:24:11.000000 texta-elastic-tools-1.5.0/texta_elastic/decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)    14298 2023-04-26 14:24:11.000000 texta-elastic-tools-1.5.0/texta_elastic/document.py
+-rw-rw-rw-   0 root         (0) root         (0)      106 2023-04-26 14:24:11.000000 texta-elastic-tools-1.5.0/texta_elastic/enums.py
+-rw-rw-rw-   0 root         (0) root         (0)      847 2023-04-26 14:24:11.000000 texta-elastic-tools-1.5.0/texta_elastic/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     5637 2023-04-26 14:24:11.000000 texta-elastic-tools-1.5.0/texta_elastic/mapping_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)     2366 2023-04-26 14:24:11.000000 texta-elastic-tools-1.5.0/texta_elastic/mapping_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     3887 2023-04-26 14:24:11.000000 texta-elastic-tools-1.5.0/texta_elastic/query.py
+-rw-rw-rw-   0 root         (0) root         (0)    17928 2023-04-26 14:24:11.000000 texta-elastic-tools-1.5.0/texta_elastic/searcher.py
+-rw-rw-rw-   0 root         (0) root         (0)     1716 2023-04-26 14:24:11.000000 texta-elastic-tools-1.5.0/texta_elastic/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     5271 2023-04-26 14:24:11.000000 texta-elastic-tools-1.5.0/texta_elastic/spam_detector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 14:25:20.000000 texta-elastic-tools-1.5.0/texta_elastic_tools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      570 2023-04-26 14:25:20.000000 texta-elastic-tools-1.5.0/texta_elastic_tools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      618 2023-04-26 14:25:20.000000 texta-elastic-tools-1.5.0/texta_elastic_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 14:25:20.000000 texta-elastic-tools-1.5.0/texta_elastic_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      119 2023-04-26 14:25:20.000000 texta-elastic-tools-1.5.0/texta_elastic_tools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-04-26 14:25:20.000000 texta-elastic-tools-1.5.0/texta_elastic_tools.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `texta-elastic-tools-1.4.1/LICENSE` & `texta-elastic-tools-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `texta-elastic-tools-1.4.1/setup.py` & `texta-elastic-tools-1.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `texta-elastic-tools-1.4.1/texta_elastic/aggregator.py` & `texta-elastic-tools-1.5.0/texta_elastic/aggregator.py`

 * *Files identical despite different names*

### Comparing `texta-elastic-tools-1.4.1/texta_elastic/core.py` & `texta-elastic-tools-1.5.0/texta_elastic/core.py`

 * *Files identical despite different names*

### Comparing `texta-elastic-tools-1.4.1/texta_elastic/decorators.py` & `texta-elastic-tools-1.5.0/texta_elastic/decorators.py`

 * *Files identical despite different names*

### Comparing `texta-elastic-tools-1.4.1/texta_elastic/document.py` & `texta-elastic-tools-1.5.0/texta_elastic/document.py`

 * *Files identical despite different names*

### Comparing `texta-elastic-tools-1.4.1/texta_elastic/exceptions.py` & `texta-elastic-tools-1.5.0/texta_elastic/exceptions.py`

 * *Files identical despite different names*

### Comparing `texta-elastic-tools-1.4.1/texta_elastic/mapping_generator.py` & `texta-elastic-tools-1.5.0/texta_elastic/mapping_generator.py`

 * *Files identical despite different names*

### Comparing `texta-elastic-tools-1.4.1/texta_elastic/mapping_tools.py` & `texta-elastic-tools-1.5.0/texta_elastic/mapping_tools.py`

 * *Files identical despite different names*

### Comparing `texta-elastic-tools-1.4.1/texta_elastic/query.py` & `texta-elastic-tools-1.5.0/texta_elastic/query.py`

 * *Files identical despite different names*

### Comparing `texta-elastic-tools-1.4.1/texta_elastic/searcher.py` & `texta-elastic-tools-1.5.0/texta_elastic/searcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-from typing import List, Optional
-
 import elasticsearch
 from elasticsearch_dsl import Search
 from elasticsearch_dsl.query import MoreLikeThis
+from typing import List, Optional
 
 from texta_elastic.core import ElasticCore, elastic_connection
 from texta_elastic.settings import TEXTA_TAGS_KEY
 
-
 ES_SCROLL_SIZE = 500
 EMPTY_QUERY = {"query": {"match_all": {}}}
 
 
 class ElasticSearcher:
     """
     Everything related to performing searches in Elasticsearch
@@ -20,15 +18,14 @@
     OUT_DOC = 'doc'  # Gives you only the _source content without index and id metadata.
     OUT_TEXT = 'text'
     OUT_TEXT_WITH_ID = "text_with_id"
     OUT_DOC_WITH_ID = 'doc_with_id'
     OUT_DOC_WITH_TOTAL_HL_AGGS = 'doc_with_total_hl_aggs'
     OUT_META = 'out_meta'
 
-
     def __init__(self,
                  field_data=[],
                  indices=[],
                  query=EMPTY_QUERY,
                  scroll_size=ES_SCROLL_SIZE,
                  output=OUT_DOC,
                  callback_progress=None,
@@ -76,27 +73,25 @@
 
         if self.callback_progress:
             total_elements = self.count()
             if scroll_limit and scroll_limit < total_elements:
                 total_elements = scroll_limit
             callback_progress.set_total(total_elements)
 
-
     def _get_core(self):
         return ElasticCore()
 
-
     def __iter__(self):
         """
         Iterator for iterating through scroll
         """
         return self.scroll()
 
-
-    def more_like_this(self, mlt_fields: List[str], like, exclude=[], min_term_freq=1, max_query_terms=12, min_doc_freq=5, min_word_length=0, max_word_length=0, stop_words=[], size=10, include_meta=False, indices: str = None, flatten: bool = False):
+    def more_like_this(self, mlt_fields: List[str], like, exclude=[], min_term_freq=1, max_query_terms=12, min_doc_freq=5, min_word_length=0, max_word_length=0, stop_words=[],
+                       size=10, include_meta=False, indices: str = None, flatten: bool = False):
         """
 
         Args:
             indices: Coma-separated string of the indices you wish to use.
             mlt_fields: List of strings of the fields you wish to use for analyzation.
             like: Can either be a text field or a list of document metas which is used as a baseline for fetching similar documents.
             exclude: List of document ids that should be ignored.
@@ -110,15 +105,16 @@
             size: How many documents to return with the end result.
             flatten: Whether to flatten nested fields.
         Returns: List of Elasticsearch documents.
 
         """
         indices = indices if indices else ",".join(self.indices)
         s = Search(using=self.core.es, index=indices)
-        mlt = MoreLikeThis(like=like, fields=mlt_fields, min_term_freq=min_term_freq, max_query_terms=max_query_terms, min_doc_freq=min_doc_freq, min_word_length=min_word_length, max_word_length=max_word_length, stop_words=stop_words)
+        mlt = MoreLikeThis(like=like, fields=mlt_fields, min_term_freq=min_term_freq, max_query_terms=max_query_terms, min_doc_freq=min_doc_freq, min_word_length=min_word_length,
+                           max_word_length=max_word_length, stop_words=stop_words)
         s = s.query(mlt).exclude("ids", values=exclude)
         s = s.extra(size=size)
         if include_meta:
             response = []
             for hit in s.execute():
                 item = {
                     "_id": hit.meta.id,
@@ -128,82 +124,79 @@
                 }
                 response.append(item)
             return response
         else:
             response = [self.core.flatten(hit.to_dict()) if flatten else hit.to_dict() for hit in s.execute()]
             return response
 
-
     def update_query(self, query):
         self.query = query
 
-
     def update_field_data(self, field_data):
         self.field_data = field_data
 
-
     def _check_for_field_data(self, dict_key: str) -> bool:
         """
         Helper function for _parse_doc to ensure that the root of nested fields
         and that the leaf of the nested field aren't filtered away by it.
 
         Given the input: {"text": {"content": "arrividerci"}}, it should not filter out fields
         if the given field in self.field_data is either text.content or just text.
         """
         root = dict_key.split(".")[0]
         is_full_nested_path = dict_key in self.field_data
         only_root_key_is_in_nested_path = root in self.field_data
         return any([is_full_nested_path, only_root_key_is_in_nested_path])
 
-
     def _default_filter(self, doc: dict):
         if self.field_data:
             # Splitting k by a dot allows us to also include nested objects which would otherwise be filtered out
             # as they won't match the fields names: so id a document has {"text": {"content": ""}} it will appear as
             # text.content which would otherwise fail the check for just "text".
             parsed_doc = {k: v for k, v in doc.items() if self._check_for_field_data(k)}
             return parsed_doc
         return doc
 
-
     def _parse_doc(self, doc: dict):
         """
         Parses a potentially nested dictionary into a flat one with it's keys delimited by a dot.
         By default, it also only keeps the fields that have been included inside self.field_data.
         """
         parsed_doc, _, _ = self._flatten_doc(doc)
         parsed_doc = self.filter_callback(parsed_doc) if self.filter_callback else self._default_filter(parsed_doc)
         return parsed_doc
 
-
     def _parse_doc_with_highlight(self, doc):
         """
         Parses Elasticsearch hit into something nicer, includes the highlight field
         """
-        parsed_doc, _, highlight = self._flatten_doc(doc)
-        return {'highlight': highlight, 'doc': parsed_doc}
+        parsed_doc, _, highlight, meta = self._flatten_doc(doc, include_meta=True)
+        return {'highlight': highlight, 'doc': parsed_doc, **meta}
 
-
-    def _flatten_doc(self, doc: dict):
+    def _flatten_doc(self, doc: dict, include_meta=False):
         """
         Flattens an Elasticsearch document by changing it's nested structures into a flat one
         where the paths of the keys are made into a dot delimited one.
 
         {"text": {"content": "arrividerci"}} -> {"text.content": "arrividerci"}
 
         Returns the flattened source, the name of the index and the highlight portion.
 
         """
         index = doc['_index']
         highlight = doc['highlight'] if 'highlight' in doc else {}
+        elastic_id = doc["_id"]
         doc = doc['_source']
         if self.flatten:
             doc = self.core.flatten(doc)
-        return doc, index, highlight
 
+        if include_meta is False:
+            return doc, index, highlight
+        else:
+            return doc, index, highlight, {"elastic_id": elastic_id, "elastic_index": index}
 
     def _decode_doc(self, doc, field_path=None):
         decoded_text = doc['_source']
         if field_path:
             # decode if field path known
             for k in field_path.split('.'):
                 # get nested fields encoded as: 'field.sub_field'
@@ -211,23 +204,21 @@
                     decoded_text = decoded_text[k]
                 except:
                     decoded_text = ""
         else:
             pass
         return decoded_text
 
-
     def count(self) -> int:
         try:
             count = self.core.es.count(index=self.indices, body=self.query)
             return count["count"]
         except elasticsearch.NotFoundError:
             return 0
 
-
     def search(self, size=10):
         # by default return all fields
         source_fields = True
         if self.output == self.OUT_META:
             source_fields = False
         # In case size/from is included in query in pagination, don't overwrite it by passing the size parameter
         if 'size' in self.query:
@@ -249,15 +240,14 @@
                 'aggs': response['aggregations'] if 'aggregations' in response else {},
                 'results': [self._parse_doc_with_highlight(doc) for doc in response['hits']['hits']]
             }
 
         else:
             return response
 
-
     def random_documents(self, size=10):
         """
         Returns n random documents, where n=size.
         """
         random_query = {
             "query": {
                 "function_score": {
@@ -268,30 +258,28 @@
         }
         response = self.core.es.search(index=self.indices, body=random_query, size=size)
         if self.output == self.OUT_DOC:
             return [self._parse_doc(doc) for doc in response['hits']['hits']]
         else:
             return response
 
-
     def resolve_field_data(self) -> List[str]:
         """
         Ensure that regardless of the fields inserted, it also always returns the facts
         to avoid problems with other applications.
         """
         if not self.field_data:
             return ["*"]
         elif self.field_data and TEXTA_TAGS_KEY not in self.field_data:
             return self.field_data + [TEXTA_TAGS_KEY]
         elif self.field_data and TEXTA_TAGS_KEY in self.field_data:
             return self.field_data
         else:
             return ["*"]
 
-
     # batch search makes an inital search, and then keeps pulling batches of results, until none are left.
     @elastic_connection
     def scroll(self):
         scroll_id = None
 
         try:
```

### Comparing `texta-elastic-tools-1.4.1/texta_elastic/settings.py` & `texta-elastic-tools-1.5.0/texta_elastic/settings.py`

 * *Files identical despite different names*

### Comparing `texta-elastic-tools-1.4.1/texta_elastic/spam_detector.py` & `texta-elastic-tools-1.5.0/texta_elastic/spam_detector.py`

 * *Files identical despite different names*

### Comparing `texta-elastic-tools-1.4.1/texta_elastic_tools.egg-info/SOURCES.txt` & `texta-elastic-tools-1.5.0/texta_elastic_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

