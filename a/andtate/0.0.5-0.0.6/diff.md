# Comparing `tmp/andtate-0.0.5.tar.gz` & `tmp/andtate-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "andtate-0.0.5.tar", last modified: Mon Apr 24 15:44:15 2023, max compression
+gzip compressed data, was "andtate-0.0.6.tar", last modified: Tue Apr 25 17:01:24 2023, max compression
```

## Comparing `andtate-0.0.5.tar` & `andtate-0.0.6.tar`

### file list

```diff
@@ -1,38 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 15:44:15.613950 andtate-0.0.5/
--rw-rw-rw-   0        0        0     1064 2023-04-22 11:08:16.000000 andtate-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      553 2023-04-24 15:44:15.612952 andtate-0.0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-24 15:44:15.570979 andtate-0.0.5/andtate/
--rw-rw-rw-   0        0        0     1400 2023-04-23 10:24:00.000000 andtate-0.0.5/andtate/AMDL Batch Gradient Descent with early stopping for Softmax Regression.py
--rw-rw-rw-   0        0        0      876 2023-04-23 10:23:38.000000 andtate-0.0.5/andtate/AMDL Linear Regression (Diabetes Dataset).py
--rw-rw-rw-   0        0        0     1558 2023-04-23 10:23:58.000000 andtate-0.0.5/andtate/AMDL Logistic Regression (Iris Dataset).py
--rw-rw-rw-   0        0        0     3299 2023-04-23 10:23:53.000000 andtate-0.0.5/andtate/AMDL MLP for classification of handwritten digits (MNIST Dataset).py
--rw-rw-rw-   0        0        0     1884 2023-04-23 10:23:40.000000 andtate-0.0.5/andtate/AMDL Multinomial Logistic Regression (Iris Dataset).py
--rw-rw-rw-   0        0        0     1260 2023-04-23 10:23:51.000000 andtate-0.0.5/andtate/AMDL SVM classifier (Iris Dataset).py
--rw-rw-rw-   0        0        0     1243 2023-04-23 10:23:46.000000 andtate-0.0.5/andtate/AMDL Train an SVM regressor on the California Housing Dataset.py
--rw-rw-rw-   0        0        0     1029 2023-04-23 10:23:49.000000 andtate-0.0.5/andtate/AMDL Train and fine-tune a Decision Tree for the Moons Dataset.py
--rw-rw-rw-   0        0        0    13739 2023-04-22 09:06:22.000000 andtate-0.0.5/andtate/AMDL.py
--rw-rw-rw-   0        0        0      737 2023-04-23 10:46:47.000000 andtate-0.0.5/andtate/NLP Dependency parsing of a given text.py
--rw-rw-rw-   0        0        0     1317 2023-04-23 10:46:38.000000 andtate-0.0.5/andtate/NLP Implement a tri-gram model.py
--rw-rw-rw-   0        0        0      644 2023-04-23 10:46:48.000000 andtate-0.0.5/andtate/NLP Lemmatization.py
--rw-rw-rw-   0        0        0      667 2023-04-23 10:46:32.000000 andtate-0.0.5/andtate/NLP Named Entity Recognition (NER) using NLTK Library.py
--rw-rw-rw-   0        0        0      491 2023-04-23 10:46:51.000000 andtate-0.0.5/andtate/NLP Named Entity Recognition (NER) using spaCy Library.py
--rw-rw-rw-   0        0        0     4729 2023-04-24 15:26:06.000000 andtate-0.0.5/andtate/NLP POS tagging using HMM.py
--rw-rw-rw-   0        0        0      921 2023-04-23 10:46:44.000000 andtate-0.0.5/andtate/NLP Stemming.py
--rw-rw-rw-   0        0        0     1169 2023-04-23 10:46:46.000000 andtate-0.0.5/andtate/NLP Syntactic parsing of a given text.py
--rw-rw-rw-   0        0        0     2255 2023-04-23 10:46:27.000000 andtate-0.0.5/andtate/NLP Text summarization using NLTK Library.py
--rw-rw-rw-   0        0        0     1178 2023-04-23 10:46:53.000000 andtate-0.0.5/andtate/NLP Text summarization using gensim Library.py
--rw-rw-rw-   0        0        0     2598 2023-04-23 10:46:41.000000 andtate-0.0.5/andtate/NLP Text summarization using spaCy Library.py
--rw-rw-rw-   0        0        0      813 2023-04-23 10:46:28.000000 andtate-0.0.5/andtate/NLP Tokenization using Gensim.py
--rw-rw-rw-   0        0        0      802 2023-04-23 10:46:49.000000 andtate-0.0.5/andtate/NLP Tokenization using NLTK.py
--rw-rw-rw-   0        0        0      710 2023-04-23 10:46:29.000000 andtate-0.0.5/andtate/NLP Tokenization using Python’s split function.py
--rw-rw-rw-   0        0        0      758 2023-04-23 10:46:40.000000 andtate-0.0.5/andtate/NLP Tokenization using Regular Expressions (RegEx).py
--rw-rw-rw-   0        0        0     1062 2023-04-23 10:46:39.000000 andtate-0.0.5/andtate/NLP Tokenization using the spaCy library.py
--rw-rw-rw-   0        0        0    21939 2023-04-24 15:42:21.000000 andtate-0.0.5/andtate/NLP.py
--rw-rw-rw-   0        0        0        0 2023-04-22 10:15:55.000000 andtate-0.0.5/andtate/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 15:44:15.608959 andtate-0.0.5/andtate.egg-info/
--rw-rw-rw-   0        0        0      553 2023-04-24 15:44:13.000000 andtate-0.0.5/andtate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1488 2023-04-24 15:44:13.000000 andtate-0.0.5/andtate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 15:44:13.000000 andtate-0.0.5/andtate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-24 15:44:13.000000 andtate-0.0.5/andtate.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-24 15:44:15.613950 andtate-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      850 2023-04-24 15:43:38.000000 andtate-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 17:01:24.424579 andtate-0.0.6/
+-rw-rw-rw-   0        0        0     1064 2023-04-22 11:08:16.000000 andtate-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0      553 2023-04-25 17:01:24.423451 andtate-0.0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-25 17:01:24.360113 andtate-0.0.6/andtate/
+-rw-rw-rw-   0        0        0     1400 2023-04-23 10:24:00.000000 andtate-0.0.6/andtate/AMDL Batch Gradient Descent with early stopping for Softmax Regression.py
+-rw-rw-rw-   0        0        0      876 2023-04-23 10:23:38.000000 andtate-0.0.6/andtate/AMDL Linear Regression (Diabetes Dataset).py
+-rw-rw-rw-   0        0        0     1558 2023-04-23 10:23:58.000000 andtate-0.0.6/andtate/AMDL Logistic Regression (Iris Dataset).py
+-rw-rw-rw-   0        0        0     3299 2023-04-23 10:23:53.000000 andtate-0.0.6/andtate/AMDL MLP for classification of handwritten digits (MNIST Dataset).py
+-rw-rw-rw-   0        0        0     1884 2023-04-23 10:23:40.000000 andtate-0.0.6/andtate/AMDL Multinomial Logistic Regression (Iris Dataset).py
+-rw-rw-rw-   0        0        0     1260 2023-04-23 10:23:51.000000 andtate-0.0.6/andtate/AMDL SVM classifier (Iris Dataset).py
+-rw-rw-rw-   0        0        0     1243 2023-04-23 10:23:46.000000 andtate-0.0.6/andtate/AMDL Train an SVM regressor on the California Housing Dataset.py
+-rw-rw-rw-   0        0        0     1029 2023-04-23 10:23:49.000000 andtate-0.0.6/andtate/AMDL Train and fine-tune a Decision Tree for the Moons Dataset.py
+-rw-rw-rw-   0        0        0    13739 2023-04-22 09:06:22.000000 andtate-0.0.6/andtate/AMDL.py
+-rw-rw-rw-   0        0        0      737 2023-04-23 10:46:47.000000 andtate-0.0.6/andtate/NLP Dependency parsing of a given text.py
+-rw-rw-rw-   0        0        0     1317 2023-04-23 10:46:38.000000 andtate-0.0.6/andtate/NLP Implement a tri-gram model.py
+-rw-rw-rw-   0        0        0      644 2023-04-23 10:46:48.000000 andtate-0.0.6/andtate/NLP Lemmatization.py
+-rw-rw-rw-   0        0        0      667 2023-04-23 10:46:32.000000 andtate-0.0.6/andtate/NLP Named Entity Recognition (NER) using NLTK Library.py
+-rw-rw-rw-   0        0        0      491 2023-04-23 10:46:51.000000 andtate-0.0.6/andtate/NLP Named Entity Recognition (NER) using spaCy Library.py
+-rw-rw-rw-   0        0        0     4729 2023-04-24 15:26:06.000000 andtate-0.0.6/andtate/NLP POS tagging using HMM.py
+-rw-rw-rw-   0        0        0      921 2023-04-23 10:46:44.000000 andtate-0.0.6/andtate/NLP Stemming.py
+-rw-rw-rw-   0        0        0     1169 2023-04-23 10:46:46.000000 andtate-0.0.6/andtate/NLP Syntactic parsing of a given text.py
+-rw-rw-rw-   0        0        0     2255 2023-04-23 10:46:27.000000 andtate-0.0.6/andtate/NLP Text summarization using NLTK Library.py
+-rw-rw-rw-   0        0        0     1178 2023-04-23 10:46:53.000000 andtate-0.0.6/andtate/NLP Text summarization using gensim Library.py
+-rw-rw-rw-   0        0        0     2598 2023-04-23 10:46:41.000000 andtate-0.0.6/andtate/NLP Text summarization using spaCy Library.py
+-rw-rw-rw-   0        0        0      813 2023-04-23 10:46:28.000000 andtate-0.0.6/andtate/NLP Tokenization using Gensim.py
+-rw-rw-rw-   0        0        0      802 2023-04-23 10:46:49.000000 andtate-0.0.6/andtate/NLP Tokenization using NLTK.py
+-rw-rw-rw-   0        0        0      710 2023-04-23 10:46:29.000000 andtate-0.0.6/andtate/NLP Tokenization using Python’s split function.py
+-rw-rw-rw-   0        0        0      758 2023-04-23 10:46:40.000000 andtate-0.0.6/andtate/NLP Tokenization using Regular Expressions (RegEx).py
+-rw-rw-rw-   0        0        0     1062 2023-04-23 10:46:39.000000 andtate-0.0.6/andtate/NLP Tokenization using the spaCy library.py
+-rw-rw-rw-   0        0        0    21939 2023-04-24 15:42:21.000000 andtate-0.0.6/andtate/NLP.py
+-rw-rw-rw-   0        0        0      671 2023-04-25 15:02:43.000000 andtate-0.0.6/andtate/WM Apriori Algorithm.py
+-rw-rw-rw-   0        0        0      931 2023-04-25 15:02:47.000000 andtate-0.0.6/andtate/WM Develop a basic crawler for the web search for user defined keywords.py
+-rw-rw-rw-   0        0        0     1199 2023-04-25 15:02:41.000000 andtate-0.0.6/andtate/WM Scrape an online E-Commerce Site for Data..py
+-rw-rw-rw-   0        0        0     1462 2023-04-25 15:02:40.000000 andtate-0.0.6/andtate/WM Scrape information from twitter..py
+-rw-rw-rw-   0        0        0     2620 2023-04-25 15:02:39.000000 andtate-0.0.6/andtate/WM Sentiment analysis for reviews by customers and visualize the same.py
+-rw-rw-rw-   0        0        0     2587 2023-04-25 15:02:56.000000 andtate-0.0.6/andtate/WM Text Mining Pre-processing using meta information from the text (Local).py
+-rw-rw-rw-   0        0        0     3007 2023-04-25 15:02:50.000000 andtate-0.0.6/andtate/WM Webpage Pre-processing using meta information from the web pages (Online).py
+-rw-rw-rw-   0        0        0     1144 2023-04-25 15:02:45.000000 andtate-0.0.6/andtate/WM deep search implementation to detect plagiarism.py
+-rw-rw-rw-   0        0        0      860 2023-04-25 15:02:54.000000 andtate-0.0.6/andtate/WM spam classifier.py
+-rw-rw-rw-   0        0        0    14271 2023-04-25 16:19:00.000000 andtate-0.0.6/andtate/WM.py
+-rw-rw-rw-   0        0        0        0 2023-04-22 10:15:55.000000 andtate-0.0.6/andtate/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 17:01:24.419938 andtate-0.0.6/andtate.egg-info/
+-rw-rw-rw-   0        0        0      553 2023-04-25 17:01:22.000000 andtate-0.0.6/andtate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2068 2023-04-25 17:01:22.000000 andtate-0.0.6/andtate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 17:01:22.000000 andtate-0.0.6/andtate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-25 17:01:22.000000 andtate-0.0.6/andtate.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-25 17:01:24.425579 andtate-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      850 2023-04-25 17:00:43.000000 andtate-0.0.6/setup.py
```

### Comparing `andtate-0.0.5/LICENSE` & `andtate-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `andtate-0.0.5/PKG-INFO` & `andtate-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: andtate
-Version: 0.0.5
+Version: 0.0.6
 Summary: andtate
 Author: AndTate
 Author-email: andtateandtate@gmail.com
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `andtate-0.0.5/andtate/AMDL Batch Gradient Descent with early stopping for Softmax Regression.py` & `andtate-0.0.6/andtate/AMDL Batch Gradient Descent with early stopping for Softmax Regression.py`

 * *Files identical despite different names*

### Comparing `andtate-0.0.5/andtate/AMDL Linear Regression (Diabetes Dataset).py` & `andtate-0.0.6/andtate/AMDL Linear Regression (Diabetes Dataset).py`

 * *Files identical despite different names*

### Comparing `andtate-0.0.5/andtate/AMDL Logistic Regression (Iris Dataset).py` & `andtate-0.0.6/andtate/AMDL Logistic Regression (Iris Dataset).py`

 * *Files identical despite different names*

### Comparing `andtate-0.0.5/andtate/AMDL MLP for classification of handwritten digits (MNIST Dataset).py` & `andtate-0.0.6/andtate/AMDL MLP for classification of handwritten digits (MNIST Dataset).py`

 * *Files identical despite different names*

### Comparing `andtate-0.0.5/andtate/AMDL Multinomial Logistic Regression (Iris Dataset).py` & `andtate-0.0.6/andtate/AMDL Multinomial Logistic Regression (Iris Dataset).py`

 * *Files identical despite different names*

### Comparing `andtate-0.0.5/andtate/AMDL SVM classifier (Iris Dataset).py` & `andtate-0.0.6/andtate/AMDL SVM classifier (Iris Dataset).py`

 * *Files identical despite different names*

### Comparing `andtate-0.0.5/andtate/AMDL Train an SVM regressor on the California Housing Dataset.py` & `andtate-0.0.6/andtate/AMDL Train an SVM regressor on the California Housing Dataset.py`

 * *Files identical despite different names*

### Comparing `andtate-0.0.5/andtate/AMDL Train and fine-tune a Decision Tree for the Moons Dataset.py` & `andtate-0.0.6/andtate/AMDL Train and fine-tune a Decision Tree for the Moons Dataset.py`

 * *Files identical despite different names*

### Comparing `andtate-0.0.5/andtate/AMDL.py` & `andtate-0.0.6/andtate/AMDL.py`

 * *Files identical despite different names*

### Comparing `andtate-0.0.5/andtate/NLP Dependency parsing of a given text.py` & `andtate-0.0.6/andtate/NLP Dependency parsing of a given text.py`

 * *Files identical despite different names*

### Comparing `andtate-0.0.5/andtate/NLP Implement a tri-gram model.py` & `andtate-0.0.6/andtate/NLP Implement a tri-gram model.py`

 * *Files identical despite different names*

### Comparing `andtate-0.0.5/andtate/NLP Lemmatization.py` & `andtate-0.0.6/andtate/NLP Lemmatization.py`

 * *Files identical despite different names*

### Comparing `andtate-0.0.5/andtate/NLP Named Entity Recognition (NER) using NLTK Library.py` & `andtate-0.0.6/andtate/NLP Named Entity Recognition (NER) using NLTK Library.py`

 * *Files identical despite different names*

### Comparing `andtate-0.0.5/andtate/NLP POS tagging using HMM.py` & `andtate-0.0.6/andtate/NLP POS tagging using HMM.py`

 * *Files identical despite different names*

### Comparing `andtate-0.0.5/andtate/NLP Stemming.py` & `andtate-0.0.6/andtate/NLP Stemming.py`

 * *Files identical despite different names*

### Comparing `andtate-0.0.5/andtate/NLP Syntactic parsing of a given text.py` & `andtate-0.0.6/andtate/NLP Syntactic parsing of a given text.py`

 * *Files identical despite different names*

### Comparing `andtate-0.0.5/andtate/NLP Text summarization using NLTK Library.py` & `andtate-0.0.6/andtate/NLP Text summarization using NLTK Library.py`

 * *Files identical despite different names*

### Comparing `andtate-0.0.5/andtate/NLP Text summarization using gensim Library.py` & `andtate-0.0.6/andtate/NLP Text summarization using gensim Library.py`

 * *Files identical despite different names*

### Comparing `andtate-0.0.5/andtate/NLP Text summarization using spaCy Library.py` & `andtate-0.0.6/andtate/NLP Text summarization using spaCy Library.py`

 * *Files identical despite different names*

### Comparing `andtate-0.0.5/andtate/NLP Tokenization using Gensim.py` & `andtate-0.0.6/andtate/NLP Tokenization using Gensim.py`

 * *Files identical despite different names*

### Comparing `andtate-0.0.5/andtate/NLP Tokenization using NLTK.py` & `andtate-0.0.6/andtate/NLP Tokenization using NLTK.py`

 * *Files identical despite different names*

### Comparing `andtate-0.0.5/andtate/NLP Tokenization using Python’s split function.py` & `andtate-0.0.6/andtate/NLP Tokenization using Python’s split function.py`

 * *Files identical despite different names*

### Comparing `andtate-0.0.5/andtate/NLP Tokenization using Regular Expressions (RegEx).py` & `andtate-0.0.6/andtate/NLP Tokenization using Regular Expressions (RegEx).py`

 * *Files identical despite different names*

### Comparing `andtate-0.0.5/andtate/NLP Tokenization using the spaCy library.py` & `andtate-0.0.6/andtate/NLP Tokenization using the spaCy library.py`

 * *Files identical despite different names*

### Comparing `andtate-0.0.5/andtate/NLP.py` & `andtate-0.0.6/andtate/NLP.py`

 * *Files identical despite different names*

### Comparing `andtate-0.0.5/andtate.egg-info/PKG-INFO` & `andtate-0.0.6/andtate.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: andtate
-Version: 0.0.5
+Version: 0.0.6
 Summary: andtate
 Author: AndTate
 Author-email: andtateandtate@gmail.com
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `andtate-0.0.5/andtate.egg-info/SOURCES.txt` & `andtate-0.0.6/andtate.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -22,12 +22,22 @@
 andtate/NLP Text summarization using spaCy Library.py
 andtate/NLP Tokenization using Gensim.py
 andtate/NLP Tokenization using NLTK.py
 andtate/NLP Tokenization using Python’s split function.py
 andtate/NLP Tokenization using Regular Expressions (RegEx).py
 andtate/NLP Tokenization using the spaCy library.py
 andtate/NLP.py
+andtate/WM Apriori Algorithm.py
+andtate/WM Develop a basic crawler for the web search for user defined keywords.py
+andtate/WM Scrape an online E-Commerce Site for Data..py
+andtate/WM Scrape information from twitter..py
+andtate/WM Sentiment analysis for reviews by customers and visualize the same.py
+andtate/WM Text Mining Pre-processing using meta information from the text (Local).py
+andtate/WM Webpage Pre-processing using meta information from the web pages (Online).py
+andtate/WM deep search implementation to detect plagiarism.py
+andtate/WM spam classifier.py
+andtate/WM.py
 andtate/__init__.py
 andtate.egg-info/PKG-INFO
 andtate.egg-info/SOURCES.txt
 andtate.egg-info/dependency_links.txt
 andtate.egg-info/top_level.txt
```

### Comparing `andtate-0.0.5/setup.py` & `andtate-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.5'
+VERSION = '0.0.6'
 DESCRIPTION = 'andtate'
 LONG_DESCRIPTION = 'Finding Glitches And Loop Holes In Matrix And Trying To Break The System'
 
 # Setting up
 setup(
     name="andtate",
     version=VERSION,
```

