# Comparing `tmp/texta-bert-tagger-3.0.1.tar.gz` & `tmp/texta-bert-tagger-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "texta-bert-tagger-3.0.1.tar", last modified: Tue Apr 25 13:52:45 2023, max compression
+gzip compressed data, was "texta-bert-tagger-3.0.2.tar", last modified: Wed Apr 26 13:04:34 2023, max compression
```

## Comparing `texta-bert-tagger-3.0.1.tar` & `texta-bert-tagger-3.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 13:52:45.516687 texta-bert-tagger-3.0.1/
--rw-rw-rw-   0 root         (0) root         (0)    35065 2023-04-24 12:12:11.000000 texta-bert-tagger-3.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1630 2023-04-25 13:52:45.512687 texta-bert-tagger-3.0.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1359 2023-04-25 11:46:25.000000 texta-bert-tagger-3.0.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)        6 2023-04-25 13:41:47.000000 texta-bert-tagger-3.0.1/VERSION
--rw-rw-rw-   0 root         (0) root         (0)      130 2023-04-24 12:12:11.000000 texta-bert-tagger-3.0.1/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-25 13:52:45.516687 texta-bert-tagger-3.0.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      687 2023-04-24 12:12:11.000000 texta-bert-tagger-3.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 13:52:45.512687 texta-bert-tagger-3.0.1/texta_bert_tagger/
--rw-rw-rw-   0 root         (0) root         (0)    11119 2023-04-24 12:12:11.000000 texta-bert-tagger-3.0.1/texta_bert_tagger/attributions.py
--rw-rw-rw-   0 root         (0) root         (0)     3360 2023-04-24 12:12:11.000000 texta-bert-tagger-3.0.1/texta_bert_tagger/config.py
--rw-rw-rw-   0 root         (0) root         (0)      454 2023-04-24 12:12:11.000000 texta-bert-tagger-3.0.1/texta_bert_tagger/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)    42547 2023-04-25 12:58:32.000000 texta-bert-tagger-3.0.1/texta_bert_tagger/tagger.py
--rw-rw-rw-   0 root         (0) root         (0)     2863 2023-04-24 12:12:11.000000 texta-bert-tagger-3.0.1/texta_bert_tagger/tagging_report.py
--rw-rw-rw-   0 root         (0) root         (0)     6422 2023-04-24 12:12:11.000000 texta-bert-tagger-3.0.1/texta_bert_tagger/validators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 13:52:45.512687 texta-bert-tagger-3.0.1/texta_bert_tagger.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1630 2023-04-25 13:52:45.000000 texta-bert-tagger-3.0.1/texta_bert_tagger.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-25 13:52:45.000000 texta-bert-tagger-3.0.1/texta_bert_tagger.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 13:52:45.000000 texta-bert-tagger-3.0.1/texta_bert_tagger.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      131 2023-04-25 13:52:45.000000 texta-bert-tagger-3.0.1/texta_bert_tagger.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-04-25 13:52:45.000000 texta-bert-tagger-3.0.1/texta_bert_tagger.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 13:04:34.473790 texta-bert-tagger-3.0.2/
+-rw-rw-rw-   0 root         (0) root         (0)    35065 2023-04-24 12:12:11.000000 texta-bert-tagger-3.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1630 2023-04-26 13:04:34.473790 texta-bert-tagger-3.0.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1359 2023-04-26 11:52:38.000000 texta-bert-tagger-3.0.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        6 2023-04-26 08:55:49.000000 texta-bert-tagger-3.0.2/VERSION
+-rw-rw-rw-   0 root         (0) root         (0)      130 2023-04-24 12:12:11.000000 texta-bert-tagger-3.0.2/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-26 13:04:34.473790 texta-bert-tagger-3.0.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      687 2023-04-24 12:12:11.000000 texta-bert-tagger-3.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 13:04:34.473790 texta-bert-tagger-3.0.2/texta_bert_tagger/
+-rw-rw-rw-   0 root         (0) root         (0)    11119 2023-04-24 12:12:11.000000 texta-bert-tagger-3.0.2/texta_bert_tagger/attributions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3360 2023-04-24 12:12:11.000000 texta-bert-tagger-3.0.2/texta_bert_tagger/config.py
+-rw-rw-rw-   0 root         (0) root         (0)      454 2023-04-24 12:12:11.000000 texta-bert-tagger-3.0.2/texta_bert_tagger/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    42547 2023-04-26 08:55:49.000000 texta-bert-tagger-3.0.2/texta_bert_tagger/tagger.py
+-rw-rw-rw-   0 root         (0) root         (0)     2863 2023-04-24 12:12:11.000000 texta-bert-tagger-3.0.2/texta_bert_tagger/tagging_report.py
+-rw-rw-rw-   0 root         (0) root         (0)     6422 2023-04-24 12:12:11.000000 texta-bert-tagger-3.0.2/texta_bert_tagger/validators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 13:04:34.473790 texta-bert-tagger-3.0.2/texta_bert_tagger.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1630 2023-04-26 13:04:34.000000 texta-bert-tagger-3.0.2/texta_bert_tagger.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-26 13:04:34.000000 texta-bert-tagger-3.0.2/texta_bert_tagger.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 13:04:34.000000 texta-bert-tagger-3.0.2/texta_bert_tagger.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      131 2023-04-26 13:04:34.000000 texta-bert-tagger-3.0.2/texta_bert_tagger.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-04-26 13:04:34.000000 texta-bert-tagger-3.0.2/texta_bert_tagger.egg-info/top_level.txt
```

### Comparing `texta-bert-tagger-3.0.1/LICENSE` & `texta-bert-tagger-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `texta-bert-tagger-3.0.1/PKG-INFO` & `texta-bert-tagger-3.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: texta-bert-tagger
-Version: 3.0.1
+Version: 3.0.2
 Summary: texta-bert-tagger
 Home-page: https://git.texta.ee/texta/texta-bert-tagger-python
 Author: TEXTA
 Author-email: info@texta.ee
 License: GPLv3
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -53,9 +53,9 @@
 result = bert_tagger.tag_text("How awful!")
 print(result)
 ```
 
 #### Output
 
 ```
-[{"prediction": "bad", "probability": 0.55200404, "attributions": []}]
+[{"prediction": "bad", "probability": 0.55200404, "attributions": {}}]
 ```
```

### Comparing `texta-bert-tagger-3.0.1/README.md` & `texta-bert-tagger-3.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -42,9 +42,9 @@
 result = bert_tagger.tag_text("How awful!")
 print(result)
 ```
 
 #### Output
 
 ```
-[{"prediction": "bad", "probability": 0.55200404, "attributions": []}]
+[{"prediction": "bad", "probability": 0.55200404, "attributions": {}}]
 ```
```

### Comparing `texta-bert-tagger-3.0.1/setup.py` & `texta-bert-tagger-3.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `texta-bert-tagger-3.0.1/texta_bert_tagger/attributions.py` & `texta-bert-tagger-3.0.2/texta_bert_tagger/attributions.py`

 * *Files identical despite different names*

### Comparing `texta-bert-tagger-3.0.1/texta_bert_tagger/config.py` & `texta-bert-tagger-3.0.2/texta_bert_tagger/config.py`

 * *Files identical despite different names*

### Comparing `texta-bert-tagger-3.0.1/texta_bert_tagger/tagger.py` & `texta-bert-tagger-3.0.2/texta_bert_tagger/tagger.py`

 * *Files 0% similar despite different names*

```diff
@@ -971,15 +971,15 @@
 
         predicted_label = self.config.label_reverse_index[prediction]
 
         all_preds = [
             {
                 "prediction": self.config.label_reverse_index[i],
                 "probability": probabilities[0][i],
-                "attributions": []
+                "attributions": {}
             }
             for i in range(self.config.n_classes)
         ]
 
         all_preds.sort(key = lambda x: x["probability"], reverse=True)
 
         if multiclass_output:
```

### Comparing `texta-bert-tagger-3.0.1/texta_bert_tagger/tagging_report.py` & `texta-bert-tagger-3.0.2/texta_bert_tagger/tagging_report.py`

 * *Files identical despite different names*

### Comparing `texta-bert-tagger-3.0.1/texta_bert_tagger/validators.py` & `texta-bert-tagger-3.0.2/texta_bert_tagger/validators.py`

 * *Files identical despite different names*

### Comparing `texta-bert-tagger-3.0.1/texta_bert_tagger.egg-info/PKG-INFO` & `texta-bert-tagger-3.0.2/texta_bert_tagger.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: texta-bert-tagger
-Version: 3.0.1
+Version: 3.0.2
 Summary: texta-bert-tagger
 Home-page: https://git.texta.ee/texta/texta-bert-tagger-python
 Author: TEXTA
 Author-email: info@texta.ee
 License: GPLv3
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -53,9 +53,9 @@
 result = bert_tagger.tag_text("How awful!")
 print(result)
 ```
 
 #### Output
 
 ```
-[{"prediction": "bad", "probability": 0.55200404, "attributions": []}]
+[{"prediction": "bad", "probability": 0.55200404, "attributions": {}}]
 ```
```

