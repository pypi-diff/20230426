# Comparing `tmp/jurebes-0.1.1a5-py3-none-any.whl.zip` & `tmp/jurebes-0.1.1a6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5704 bytes, number of entries: 7
--rw-r--r--  2.0 unx    17224 b- defN 23-Apr-25 05:52 jurebes/__init__.py
--rw-r--r--  2.0 unx      177 b- defN 23-Apr-25 05:52 jurebes/version.py
--rw-r--r--  2.0 unx      753 b- defN 23-Apr-25 05:52 jurebes-0.1.1a5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-25 05:52 jurebes-0.1.1a5.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Apr-25 05:52 jurebes-0.1.1a5.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Apr-25 05:52 jurebes-0.1.1a5.dist-info/zip-safe
--rw-rw-r--  2.0 unx      543 b- defN 23-Apr-25 05:52 jurebes-0.1.1a5.dist-info/RECORD
-7 files, 18798 bytes uncompressed, 4736 bytes compressed:  74.8%
+Zip file size: 5738 bytes, number of entries: 7
+-rw-r--r--  2.0 unx    17310 b- defN 23-Apr-25 16:35 jurebes/__init__.py
+-rw-r--r--  2.0 unx      177 b- defN 23-Apr-25 16:35 jurebes/version.py
+-rw-r--r--  2.0 unx      753 b- defN 23-Apr-25 16:35 jurebes-0.1.1a6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-25 16:35 jurebes-0.1.1a6.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Apr-25 16:35 jurebes-0.1.1a6.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Apr-25 16:35 jurebes-0.1.1a6.dist-info/zip-safe
+-rw-rw-r--  2.0 unx      543 b- defN 23-Apr-25 16:35 jurebes-0.1.1a6.dist-info/RECORD
+7 files, 18884 bytes uncompressed, 4770 bytes compressed:  74.7%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: jurebes/__init__.py
 Comment: 
 
 Filename: jurebes/version.py
 Comment: 
 
-Filename: jurebes-0.1.1a5.dist-info/METADATA
+Filename: jurebes-0.1.1a6.dist-info/METADATA
 Comment: 
 
-Filename: jurebes-0.1.1a5.dist-info/WHEEL
+Filename: jurebes-0.1.1a6.dist-info/WHEEL
 Comment: 
 
-Filename: jurebes-0.1.1a5.dist-info/top_level.txt
+Filename: jurebes-0.1.1a6.dist-info/top_level.txt
 Comment: 
 
-Filename: jurebes-0.1.1a5.dist-info/zip-safe
+Filename: jurebes-0.1.1a6.dist-info/zip-safe
 Comment: 
 
-Filename: jurebes-0.1.1a5.dist-info/RECORD
+Filename: jurebes-0.1.1a6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## jurebes/__init__.py

```diff
@@ -254,18 +254,20 @@
         total = sum(i.confidence for i in classified_intents)
         normbonus = (1 - total) / len(intents)
 
         for i in intents:
             i.confidence += normbonus
             yield i
 
-    def calc_intent(self, query):
+    def calc_intent(self, query, threshold=0):
         intents = list(self.calc_intents(query))
         if len(intents):
-            return max(intents, key=lambda k: k.confidence)
+            best = max(intents, key=lambda k: k.confidence)
+            if best.confidence >= threshold:
+                return best
         return None
 
     @staticmethod
     def _transform_iob_to_dataset(tagged_sentences):
         X, y = [], []
 
         for tagged in tagged_sentences:
```

## jurebes/version.py

```diff
@@ -1,7 +1,7 @@
 # The following lines are replaced during the release process.
 # START_VERSION_BLOCK
 VERSION_MAJOR = 0
 VERSION_MINOR = 1
 VERSION_BUILD = 1
-VERSION_ALPHA = 5
+VERSION_ALPHA = 6
 # END_VERSION_BLOCK
```

## Comparing `jurebes-0.1.1a5.dist-info/METADATA` & `jurebes-0.1.1a6.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jurebes
-Version: 0.1.1a5
+Version: 0.1.1a6
 Summary: A intent parser from OpenVoiceOS
 Home-page: https://github.com/OpenVoiceOS/jurebes
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

