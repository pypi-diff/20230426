# Comparing `tmp/gptrim-0.1.4-py3-none-any.whl.zip` & `tmp/gptrim-0.1.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 4045 bytes, number of entries: 7
+Zip file size: 4097 bytes, number of entries: 7
 -rw-rw-r--  2.0 unx       25 b- defN 23-Apr-16 12:45 gptrim/__init__.py
--rw-rw-r--  2.0 unx     3772 b- defN 23-Apr-23 14:48 gptrim/gptrim.py
--rw-rw-r--  2.0 unx     1070 b- defN 23-Apr-23 14:53 gptrim-0.1.4.dist-info/LICENSE
--rw-rw-r--  2.0 unx     1113 b- defN 23-Apr-23 14:53 gptrim-0.1.4.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-23 14:53 gptrim-0.1.4.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-Apr-23 14:53 gptrim-0.1.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      526 b- defN 23-Apr-23 14:53 gptrim-0.1.4.dist-info/RECORD
-7 files, 6605 bytes uncompressed, 3115 bytes compressed:  52.8%
+-rw-rw-r--  2.0 unx     3918 b- defN 23-Apr-25 18:13 gptrim/gptrim.py
+-rw-rw-r--  2.0 unx     1070 b- defN 23-Apr-25 18:16 gptrim-0.1.5.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     1113 b- defN 23-Apr-25 18:16 gptrim-0.1.5.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-25 18:16 gptrim-0.1.5.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-Apr-25 18:16 gptrim-0.1.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      526 b- defN 23-Apr-25 18:16 gptrim-0.1.5.dist-info/RECORD
+7 files, 6751 bytes uncompressed, 3167 bytes compressed:  53.1%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: gptrim/__init__.py
 Comment: 
 
 Filename: gptrim/gptrim.py
 Comment: 
 
-Filename: gptrim-0.1.4.dist-info/LICENSE
+Filename: gptrim-0.1.5.dist-info/LICENSE
 Comment: 
 
-Filename: gptrim-0.1.4.dist-info/METADATA
+Filename: gptrim-0.1.5.dist-info/METADATA
 Comment: 
 
-Filename: gptrim-0.1.4.dist-info/WHEEL
+Filename: gptrim-0.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: gptrim-0.1.4.dist-info/top_level.txt
+Filename: gptrim-0.1.5.dist-info/top_level.txt
 Comment: 
 
-Filename: gptrim-0.1.4.dist-info/RECORD
+Filename: gptrim-0.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gptrim/gptrim.py

```diff
@@ -1,7 +1,8 @@
+import re
 from typing import Optional
 
 import nltk
 from nltk.corpus import stopwords
 from nltk.stem import PorterStemmer, SnowballStemmer, LancasterStemmer
 
 nltk.download('punkt')
@@ -71,27 +72,30 @@
         "wouldnt",
     ],
 }
 
 
 def trim(
     text: str, stemmer: Optional[str] = None, language: str = "english", remove_spaces: bool = True,
-        remove_stopwords: bool = True
-) -> str:
+        remove_stopwords: bool = True, remove_punctuation: bool = False) -> str:
 
     if language not in stopwords.fileids():
         raise ValueError("Unsupported language")
 
     accepted_stemmers = ("snowball", "porter", "lancaster")
     if stemmer and stemmer not in accepted_stemmers:
         raise ValueError("Stemmer must be one of", accepted_stemmers)
 
     # merge contractions
     text = text.replace("'", "").replace("’", "")
 
+    # remove punctuation
+    if remove_punctuation:
+        text = re.sub(r'[.,\'\"?!;:-]', '', text)
+
     # tokenize words, keep uppercase
     tokenized = nltk.word_tokenize(text)
 
     if remove_stopwords:
         nltk_stopwords = stopwords.words(language)
         words_to_exclude = set(
             nltk_stopwords + ARTICLES_PREPOSITIONS.get(language, [])
```

## Comparing `gptrim-0.1.4.dist-info/LICENSE` & `gptrim-0.1.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `gptrim-0.1.4.dist-info/METADATA` & `gptrim-0.1.5.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptrim
-Version: 0.1.4
+Version: 0.1.5
 Summary: Reduce the size of GPT inputs by 40-60% without losing most of the information.
 Home-page: https://github.com/vlad-ds/gptrim
 Author: Vlad Gheorghe
 Author-email: vlad.datapro@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

