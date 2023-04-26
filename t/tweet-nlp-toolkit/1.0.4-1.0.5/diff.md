# Comparing `tmp/tweet_nlp_toolkit-1.0.4.tar.gz` & `tmp/tweet_nlp_toolkit-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tweet_nlp_toolkit-1.0.4.tar", last modified: Thu Jan  5 00:12:11 2023, max compression
+gzip compressed data, was "dist/tweet_nlp_toolkit-1.0.5.tar", last modified: Wed Apr 26 00:14:10 2023, max compression
```

## Comparing `tweet_nlp_toolkit-1.0.4.tar` & `tweet_nlp_toolkit-1.0.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 00:12:11.000000 tweet_nlp_toolkit-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-01-05 00:12:11.000000 tweet_nlp_toolkit-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     4710 2023-01-05 00:11:40.000000 tweet_nlp_toolkit-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 00:12:11.000000 tweet_nlp_toolkit-1.0.4/tweet_nlp_toolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-01-05 00:12:11.000000 tweet_nlp_toolkit-1.0.4/tweet_nlp_toolkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      123 2023-01-05 00:12:11.000000 tweet_nlp_toolkit-1.0.4/tweet_nlp_toolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)      606 2023-01-05 00:12:11.000000 tweet_nlp_toolkit-1.0.4/tweet_nlp_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-05 00:12:11.000000 tweet_nlp_toolkit-1.0.4/tweet_nlp_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)     6490 2023-01-05 00:12:11.000000 tweet_nlp_toolkit-1.0.4/tweet_nlp_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-01-05 00:11:40.000000 tweet_nlp_toolkit-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      990 2023-01-05 00:11:40.000000 tweet_nlp_toolkit-1.0.4/setup.py
--rw-r--r--   0 runner    (1001) docker     (122)     6490 2023-01-05 00:12:11.000000 tweet_nlp_toolkit-1.0.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 00:12:11.000000 tweet_nlp_toolkit-1.0.4/tweet_nlp_toolkit/
--rw-r--r--   0 runner    (1001) docker     (122)     1283 2023-01-05 00:11:40.000000 tweet_nlp_toolkit-1.0.4/tweet_nlp_toolkit/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 00:12:11.000000 tweet_nlp_toolkit-1.0.4/tweet_nlp_toolkit/prep/
--rw-r--r--   0 runner    (1001) docker     (122)     4011 2023-01-05 00:11:40.000000 tweet_nlp_toolkit-1.0.4/tweet_nlp_toolkit/prep/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (122)     2919 2023-01-05 00:11:40.000000 tweet_nlp_toolkit-1.0.4/tweet_nlp_toolkit/prep/word_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (122)    10020 2023-01-05 00:11:40.000000 tweet_nlp_toolkit-1.0.4/tweet_nlp_toolkit/prep/text_parser.py
--rw-r--r--   0 runner    (1001) docker     (122)     3787 2023-01-05 00:11:40.000000 tweet_nlp_toolkit-1.0.4/tweet_nlp_toolkit/prep/regexes.py
--rw-r--r--   0 runner    (1001) docker     (122)       50 2023-01-05 00:11:40.000000 tweet_nlp_toolkit-1.0.4/tweet_nlp_toolkit/prep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6467 2023-01-05 00:11:40.000000 tweet_nlp_toolkit-1.0.4/tweet_nlp_toolkit/prep/token.py
--rw-r--r--   0 runner    (1001) docker     (122)     2070 2023-01-05 00:11:40.000000 tweet_nlp_toolkit-1.0.4/tweet_nlp_toolkit/prep/text_prep.py
--rw-r--r--   0 runner    (1001) docker     (122)     7490 2023-01-05 00:11:40.000000 tweet_nlp_toolkit-1.0.4/tweet_nlp_toolkit/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)      232 2023-01-05 00:11:40.000000 tweet_nlp_toolkit-1.0.4/tweet_nlp_toolkit/__version__.py
--rw-r--r--   0 runner    (1001) docker     (122)      271 2023-01-05 00:11:40.000000 tweet_nlp_toolkit-1.0.4/tweet_nlp_toolkit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 00:14:10.000000 tweet_nlp_toolkit-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (122)     6490 2023-04-26 00:14:10.000000 tweet_nlp_toolkit-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4710 2023-04-26 00:13:41.000000 tweet_nlp_toolkit-1.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-26 00:14:10.000000 tweet_nlp_toolkit-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-04-26 00:13:41.000000 tweet_nlp_toolkit-1.0.5/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 00:14:10.000000 tweet_nlp_toolkit-1.0.5/tweet_nlp_toolkit/
+-rw-r--r--   0 runner    (1001) docker     (122)      271 2023-04-26 00:13:41.000000 tweet_nlp_toolkit-1.0.5/tweet_nlp_toolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      232 2023-04-26 00:13:41.000000 tweet_nlp_toolkit-1.0.5/tweet_nlp_toolkit/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7490 2023-04-26 00:13:41.000000 tweet_nlp_toolkit-1.0.5/tweet_nlp_toolkit/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1283 2023-04-26 00:13:41.000000 tweet_nlp_toolkit-1.0.5/tweet_nlp_toolkit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 00:14:10.000000 tweet_nlp_toolkit-1.0.5/tweet_nlp_toolkit/prep/
+-rw-r--r--   0 runner    (1001) docker     (122)       50 2023-04-26 00:13:41.000000 tweet_nlp_toolkit-1.0.5/tweet_nlp_toolkit/prep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2919 2023-04-26 00:13:41.000000 tweet_nlp_toolkit-1.0.5/tweet_nlp_toolkit/prep/word_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6467 2023-04-26 00:13:41.000000 tweet_nlp_toolkit-1.0.5/tweet_nlp_toolkit/prep/token.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2070 2023-04-26 00:13:41.000000 tweet_nlp_toolkit-1.0.5/tweet_nlp_toolkit/prep/text_prep.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4011 2023-04-26 00:13:41.000000 tweet_nlp_toolkit-1.0.5/tweet_nlp_toolkit/prep/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10103 2023-04-26 00:13:41.000000 tweet_nlp_toolkit-1.0.5/tweet_nlp_toolkit/prep/text_parser.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3787 2023-04-26 00:13:41.000000 tweet_nlp_toolkit-1.0.5/tweet_nlp_toolkit/prep/regexes.py
+-rw-r--r--   0 runner    (1001) docker     (122)      990 2023-04-26 00:13:41.000000 tweet_nlp_toolkit-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 00:14:10.000000 tweet_nlp_toolkit-1.0.5/tweet_nlp_toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     6490 2023-04-26 00:14:09.000000 tweet_nlp_toolkit-1.0.5/tweet_nlp_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      123 2023-04-26 00:14:09.000000 tweet_nlp_toolkit-1.0.5/tweet_nlp_toolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      606 2023-04-26 00:14:10.000000 tweet_nlp_toolkit-1.0.5/tweet_nlp_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-04-26 00:14:09.000000 tweet_nlp_toolkit-1.0.5/tweet_nlp_toolkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-26 00:14:09.000000 tweet_nlp_toolkit-1.0.5/tweet_nlp_toolkit.egg-info/dependency_links.txt
```

### Comparing `tweet_nlp_toolkit-1.0.4/README.md` & `tweet_nlp_toolkit-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `tweet_nlp_toolkit-1.0.4/tweet_nlp_toolkit.egg-info/SOURCES.txt` & `tweet_nlp_toolkit-1.0.5/tweet_nlp_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tweet_nlp_toolkit-1.0.4/tweet_nlp_toolkit.egg-info/PKG-INFO` & `tweet_nlp_toolkit-1.0.5/tweet_nlp_toolkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tweet-nlp-toolkit
-Version: 1.0.4
+Version: 1.0.5
 Summary: NLP toolkit for tweets
 Home-page: https://github.com/hitchhicker/tweet_nlp_toolkit
 Author: Bokai Yu
 License: UNKNOWN
 Description: ![ci](https://github.com/hitchhicker/tweet_nlp_toolkit/actions/workflows/makefile.yml/badge.svg)
         
         # tweet_nlp_toolkit
```

### Comparing `tweet_nlp_toolkit-1.0.4/LICENSE` & `tweet_nlp_toolkit-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tweet_nlp_toolkit-1.0.4/setup.py` & `tweet_nlp_toolkit-1.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `tweet_nlp_toolkit-1.0.4/PKG-INFO` & `tweet_nlp_toolkit-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tweet_nlp_toolkit
-Version: 1.0.4
+Version: 1.0.5
 Summary: NLP toolkit for tweets
 Home-page: https://github.com/hitchhicker/tweet_nlp_toolkit
 Author: Bokai Yu
 License: UNKNOWN
 Description: ![ci](https://github.com/hitchhicker/tweet_nlp_toolkit/actions/workflows/makefile.yml/badge.svg)
         
         # tweet_nlp_toolkit
```

### Comparing `tweet_nlp_toolkit-1.0.4/tweet_nlp_toolkit/utils.py` & `tweet_nlp_toolkit-1.0.5/tweet_nlp_toolkit/utils.py`

 * *Files identical despite different names*

### Comparing `tweet_nlp_toolkit-1.0.4/tweet_nlp_toolkit/prep/tokenizer.py` & `tweet_nlp_toolkit-1.0.5/tweet_nlp_toolkit/prep/tokenizer.py`

 * *Files identical despite different names*

### Comparing `tweet_nlp_toolkit-1.0.4/tweet_nlp_toolkit/prep/word_segmentation.py` & `tweet_nlp_toolkit-1.0.5/tweet_nlp_toolkit/prep/word_segmentation.py`

 * *Files identical despite different names*

### Comparing `tweet_nlp_toolkit-1.0.4/tweet_nlp_toolkit/prep/text_parser.py` & `tweet_nlp_toolkit-1.0.5/tweet_nlp_toolkit/prep/text_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 
     @property
     def tokens(self) -> List[Token]:
         return self._tokens
 
     @property
     def hashtags(self) -> List[str]:
-        return list({token.value.strip("#") for token in self._tokens if token.is_hashtag})
+        return list({token.value for token in self._tokens if token.is_hashtag})
 
     @property
     def mentions(self) -> List[str]:
         return [token.value for token in self._tokens if token.is_mention]
 
     @property
     def emoticons(self) -> List[str]:
@@ -139,15 +139,15 @@
 ):
     """
     Preprocess the text
 
     Example:
         In [1]: from tweet_nlp_toolkit.prep.text_parser import parse_text
 
-        In [2]: text = parse_text("123 @hello #world www.url.com 😰 :) abc@gmail.com")
+        In [2]: text = parse_text("123 @hello #world www.url.com 😰 :) abc@gmail.com", emails="remove", emojis="remove", emoticons="remove", urls="remove", digits="remove")  # noqa
 
         In [3]: text.tokens
         Out[3]: ['@hello', '#world']
 
         In [4]: text.hashtags
         Out[4]: ['#world']
```

### Comparing `tweet_nlp_toolkit-1.0.4/tweet_nlp_toolkit/prep/regexes.py` & `tweet_nlp_toolkit-1.0.5/tweet_nlp_toolkit/prep/regexes.py`

 * *Files identical despite different names*

### Comparing `tweet_nlp_toolkit-1.0.4/tweet_nlp_toolkit/prep/token.py` & `tweet_nlp_toolkit-1.0.5/tweet_nlp_toolkit/prep/token.py`

 * *Files identical despite different names*

### Comparing `tweet_nlp_toolkit-1.0.4/tweet_nlp_toolkit/prep/text_prep.py` & `tweet_nlp_toolkit-1.0.5/tweet_nlp_toolkit/prep/text_prep.py`

 * *Files identical despite different names*

### Comparing `tweet_nlp_toolkit-1.0.4/tweet_nlp_toolkit/constants.py` & `tweet_nlp_toolkit-1.0.5/tweet_nlp_toolkit/constants.py`

 * *Files identical despite different names*

