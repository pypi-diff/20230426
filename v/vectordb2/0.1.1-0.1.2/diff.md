# Comparing `tmp/vectordb2-0.1.1.tar.gz` & `tmp/vectordb2-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vectordb2-0.1.1.tar", last modified: Tue Apr 25 04:31:47 2023, max compression
+gzip compressed data, was "vectordb2-0.1.2.tar", last modified: Tue Apr 25 23:51:06 2023, max compression
```

## Comparing `vectordb2-0.1.1.tar` & `vectordb2-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-25 04:31:47.382151 vectordb2-0.1.1/
--rw-r--r--   0 prelovac   (502) staff       (20)     1068 2023-04-25 04:13:48.000000 vectordb2-0.1.1/LICENSE
--rw-r--r--   0 prelovac   (502) staff       (20)      822 2023-04-25 04:31:47.381923 vectordb2-0.1.1/PKG-INFO
--rw-r--r--   0 prelovac   (502) staff       (20)     9011 2023-04-25 04:29:42.000000 vectordb2-0.1.1/README.md
--rw-r--r--   0 prelovac   (502) staff       (20)       38 2023-04-25 04:31:47.382221 vectordb2-0.1.1/setup.cfg
--rw-r--r--   0 prelovac   (502) staff       (20)     1117 2023-04-25 04:31:30.000000 vectordb2-0.1.1/setup.py
-drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-25 04:31:47.380452 vectordb2-0.1.1/vectordb/
--rw-r--r--   0 prelovac   (502) staff       (20)       27 2023-04-25 04:10:57.000000 vectordb2-0.1.1/vectordb/__init__.py
--rw-r--r--   0 prelovac   (502) staff       (20)     2546 2023-04-25 04:00:36.000000 vectordb2-0.1.1/vectordb/chunking.py
--rw-r--r--   0 prelovac   (502) staff       (20)      822 2023-04-25 04:00:36.000000 vectordb2-0.1.1/vectordb/embedding.py
--rw-r--r--   0 prelovac   (502) staff       (20)     3703 2023-04-25 04:10:33.000000 vectordb2-0.1.1/vectordb/memory.py
--rw-r--r--   0 prelovac   (502) staff       (20)     1047 2023-04-25 04:00:36.000000 vectordb2-0.1.1/vectordb/storage.py
--rw-r--r--   0 prelovac   (502) staff       (20)      873 2023-04-25 04:00:36.000000 vectordb2-0.1.1/vectordb/vector_search.py
-drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-25 04:31:47.381635 vectordb2-0.1.1/vectordb2.egg-info/
--rw-r--r--   0 prelovac   (502) staff       (20)      822 2023-04-25 04:31:47.000000 vectordb2-0.1.1/vectordb2.egg-info/PKG-INFO
--rw-r--r--   0 prelovac   (502) staff       (20)      319 2023-04-25 04:31:47.000000 vectordb2-0.1.1/vectordb2.egg-info/SOURCES.txt
--rw-r--r--   0 prelovac   (502) staff       (20)        1 2023-04-25 04:31:47.000000 vectordb2-0.1.1/vectordb2.egg-info/dependency_links.txt
--rw-r--r--   0 prelovac   (502) staff       (20)      104 2023-04-25 04:31:47.000000 vectordb2-0.1.1/vectordb2.egg-info/requires.txt
--rw-r--r--   0 prelovac   (502) staff       (20)        9 2023-04-25 04:31:47.000000 vectordb2-0.1.1/vectordb2.egg-info/top_level.txt
+drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-25 23:51:06.460070 vectordb2-0.1.2/
+-rw-r--r--   0 prelovac   (502) staff       (20)     1068 2023-04-25 04:13:48.000000 vectordb2-0.1.2/LICENSE
+-rw-r--r--   0 prelovac   (502) staff       (20)      831 2023-04-25 23:51:06.459824 vectordb2-0.1.2/PKG-INFO
+-rw-r--r--   0 prelovac   (502) staff       (20)     9470 2023-04-25 23:50:42.000000 vectordb2-0.1.2/README.md
+-rw-r--r--   0 prelovac   (502) staff       (20)       38 2023-04-25 23:51:06.460140 vectordb2-0.1.2/setup.cfg
+-rw-r--r--   0 prelovac   (502) staff       (20)     1147 2023-04-25 23:38:12.000000 vectordb2-0.1.2/setup.py
+drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-25 23:51:06.458254 vectordb2-0.1.2/vectordb/
+-rw-r--r--   0 prelovac   (502) staff       (20)       27 2023-04-25 04:10:57.000000 vectordb2-0.1.2/vectordb/__init__.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     2666 2023-04-25 23:50:42.000000 vectordb2-0.1.2/vectordb/chunking.py
+-rw-r--r--   0 prelovac   (502) staff       (20)      822 2023-04-25 04:00:36.000000 vectordb2-0.1.2/vectordb/embedding.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     3703 2023-04-25 04:10:33.000000 vectordb2-0.1.2/vectordb/memory.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     1047 2023-04-25 04:00:36.000000 vectordb2-0.1.2/vectordb/storage.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     2028 2023-04-25 23:49:46.000000 vectordb2-0.1.2/vectordb/vector_search.py
+drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-25 23:51:06.459518 vectordb2-0.1.2/vectordb2.egg-info/
+-rw-r--r--   0 prelovac   (502) staff       (20)      831 2023-04-25 23:51:06.000000 vectordb2-0.1.2/vectordb2.egg-info/PKG-INFO
+-rw-r--r--   0 prelovac   (502) staff       (20)      319 2023-04-25 23:51:06.000000 vectordb2-0.1.2/vectordb2.egg-info/SOURCES.txt
+-rw-r--r--   0 prelovac   (502) staff       (20)        1 2023-04-25 23:51:06.000000 vectordb2-0.1.2/vectordb2.egg-info/dependency_links.txt
+-rw-r--r--   0 prelovac   (502) staff       (20)      114 2023-04-25 23:51:06.000000 vectordb2-0.1.2/vectordb2.egg-info/requires.txt
+-rw-r--r--   0 prelovac   (502) staff       (20)        9 2023-04-25 23:51:06.000000 vectordb2-0.1.2/vectordb2.egg-info/top_level.txt
```

### Comparing `vectordb2-0.1.1/LICENSE` & `vectordb2-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vectordb2-0.1.1/README.md` & `vectordb2-0.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 # VectorDB
 
-VectorDB is a minimal Python package for storing and retrieving text using chunking, embedding, and vector search techniques. It provides an easy-to-use interface for saving, searching, and managing textual data with associated metadata.
+[![](https://dcbadge.vercel.app/api/server/aDNg6E9szy?compact=true&style=flat)](https://discord.gg/aDNg6E9szy) [![Twitter](https://img.shields.io/twitter/follow/KagiHQ?style=social)](https://twitter.com/KagiHQ) [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/license/mit/) 
+
+VectorDB is a lightweight Python package for storing and retrieving text using chunking, embedding, and vector search techniques. It provides an easy-to-use interface for saving, searching, and managing textual data with associated metadata.
 
 ## Installation
 
 To install VectorDB, use pip:
 
 ```
 pip install vectordb2
 ```
 
 ## Usage
 
-Here's a quick example of how to use PyMemory:
+Here's a quick example of how to use VectorDB:
 
 ```
 from vectordb import Memory
 
 memory = Memory()
 
 # text = "..."
@@ -39,15 +41,15 @@
 
 - Initializes the Memory class.
 - **memory_file** (str): Path to the memory file (default: None). If provided, memory will persist to disk.
 - **chunking_strategy** (dict): Dictionary containing the chunking mode (default: {"mode": "sliding_window"})
    Options::
 	{'mode':'sliding_window', 'window_size': 256, 'overlap': 32}
 	{'mode':'paragraph'}
-- **embedding_model** (str): Name of the pre-trained model to be used for embeddings (default: "sentence-transformers/all-MiniLM-L6-v2").
+- **embedding_model** (str): Name of the pre-trained model to be used for embeddings (default: "sentence-transformers/all-MiniLM-L6-v2"). See [Pretrained models](https://www.sbert.net/docs/pretrained_models.html) and [MTEB](https://huggingface.co/spaces/mteb/leaderboard).
 
 **save(self, texts, metadata_list, memory_file=None)**
 
 - Saves the given texts and metadata to memory.
 - **texts** (str or list of str): Text or list of texts to be saved.
 - **metadata_list** (dict or list of dict): Metadata or list of metadata associated with the texts.
 - **memory_file** (str): Path to the memory file (default: None).
```

### Comparing `vectordb2-0.1.1/setup.py` & `vectordb2-0.1.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vectordb2",
-    version="0.1.1",
+    version="0.1.2",
     packages=find_packages(),
     install_requires=[
         "torch>=1.9.0",
         "transformers>=4.10.0",
         "numpy>=1.21.0",
         "scikit-learn>=0.24.0",
         "scipy>=1.7.0",
         "sentence_transformers",
+        "faiss-cpu",
     ],
-    author="Your Name",
-    author_email="your.email@example.com",
-    description="A Python package for storing and retrieving text using chunking, embedding, and vector search",
+    author="Vladimir Prelovac",
+    author_email="vlad@kagi.com",
+    description="A lightweight Python package for storing and retrieving text using chunking, embedding, and vector search",
     keywords="text chunking embedding vector search",
-    url="https://github.com/yourusername/pymemory",
+    url="https://github.com/kagisearch/vectordb",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
```

### Comparing `vectordb2-0.1.1/vectordb/chunking.py` & `vectordb2-0.1.2/vectordb/chunking.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,17 +37,21 @@
     def paragraph_chunking(self, text: str) -> List[str]:
         """
         Splits the input text into paragraphs.
 
         :param text: a string containing the text to be chunked.
         :return: a list of paragraphs extracted from the input text.
         """
-        text = self.clean_text(text)
         paragraphs = text.split("\n\n")
-        return [p.strip() for p in paragraphs if p.strip()]
+        cleaned_paragraphs = []
+        for p in paragraphs:
+            cleaned_p = self.clean_text(p)
+            if cleaned_p:
+                cleaned_paragraphs.append(cleaned_p)
+        return cleaned_paragraphs
 
     def sliding_window_chunking(self, text: str) -> List[str]:
         """
         Splits the input text into chunks using the sliding window technique.
 
         :param text: a string containing the text to be chunked.
         :return: a list of chunks generated from the input text.
```

### Comparing `vectordb2-0.1.1/vectordb/embedding.py` & `vectordb2-0.1.2/vectordb/embedding.py`

 * *Files identical despite different names*

### Comparing `vectordb2-0.1.1/vectordb/memory.py` & `vectordb2-0.1.2/vectordb/memory.py`

 * *Files identical despite different names*

### Comparing `vectordb2-0.1.1/vectordb/storage.py` & `vectordb2-0.1.2/vectordb/storage.py`

 * *Files identical despite different names*

