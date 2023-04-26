# Comparing `tmp/spiralflow-0.0.2.tar.gz` & `tmp/spiralflow-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spiralflow-0.0.2.tar", last modified: Thu Apr 20 04:20:49 2023, max compression
+gzip compressed data, was "spiralflow-0.0.3.tar", last modified: Wed Apr 26 01:42:57 2023, max compression
```

## Comparing `spiralflow-0.0.2.tar` & `spiralflow-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 04:20:49.827964 spiralflow-0.0.2/
--rw-rw-rw-   0        0        0     1092 2023-04-09 17:15:16.000000 spiralflow-0.0.2/LICENSE
--rw-rw-rw-   0        0        0    12765 2023-04-20 04:20:49.823975 spiralflow-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0    12239 2023-04-20 04:15:29.000000 spiralflow-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-04-20 04:20:49.827964 spiralflow-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      877 2023-04-20 04:20:43.000000 spiralflow-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-20 04:20:49.810801 spiralflow-0.0.2/spiralflow/
--rw-rw-rw-   0        0        0       22 2023-04-20 04:20:31.000000 spiralflow-0.0.2/spiralflow/__init__.py
--rw-rw-rw-   0        0        0     5385 2023-04-14 04:47:37.000000 spiralflow-0.0.2/spiralflow/chat_history.py
--rw-rw-rw-   0        0        0     1330 2023-04-14 04:47:37.000000 spiralflow-0.0.2/spiralflow/chat_llm.py
--rw-rw-rw-   0        0        0    52297 2023-04-19 15:05:49.000000 spiralflow-0.0.2/spiralflow/flow.py
--rw-rw-rw-   0        0        0     7781 2023-04-19 15:05:48.000000 spiralflow-0.0.2/spiralflow/memory.py
--rw-rw-rw-   0        0        0    16849 2023-04-19 15:05:24.000000 spiralflow-0.0.2/spiralflow/message.py
--rw-rw-rw-   0        0        0     2266 2023-04-14 15:31:34.000000 spiralflow-0.0.2/spiralflow/tools.py
-drwxrwxrwx   0        0        0        0 2023-04-20 04:20:49.821813 spiralflow-0.0.2/spiralflow.egg-info/
--rw-rw-rw-   0        0        0    12765 2023-04-20 04:20:49.000000 spiralflow-0.0.2/spiralflow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      350 2023-04-20 04:20:49.000000 spiralflow-0.0.2/spiralflow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 04:20:49.000000 spiralflow-0.0.2/spiralflow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-04-20 04:20:49.000000 spiralflow-0.0.2/spiralflow.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-20 04:20:49.000000 spiralflow-0.0.2/spiralflow.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-26 01:42:57.185700 spiralflow-0.0.3/
+-rw-rw-rw-   0        0        0     1092 2023-04-09 17:15:16.000000 spiralflow-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0    12978 2023-04-26 01:42:57.181188 spiralflow-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0    12452 2023-04-24 19:26:36.000000 spiralflow-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-26 01:42:57.185700 spiralflow-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      877 2023-04-26 01:42:31.000000 spiralflow-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 01:42:57.165616 spiralflow-0.0.3/spiralflow/
+-rw-rw-rw-   0        0        0       23 2023-04-26 01:42:42.000000 spiralflow-0.0.3/spiralflow/__init__.py
+-rw-rw-rw-   0        0        0     5385 2023-04-24 19:26:36.000000 spiralflow-0.0.3/spiralflow/chat_history.py
+-rw-rw-rw-   0        0        0     1330 2023-04-24 19:26:36.000000 spiralflow-0.0.3/spiralflow/chat_llm.py
+-rw-rw-rw-   0        0        0    53659 2023-04-26 01:41:18.000000 spiralflow-0.0.3/spiralflow/flow.py
+-rw-rw-rw-   0        0        0     6835 2023-04-26 01:38:32.000000 spiralflow-0.0.3/spiralflow/memory.py
+-rw-rw-rw-   0        0        0    16849 2023-04-24 19:26:36.000000 spiralflow-0.0.3/spiralflow/message.py
+-rw-rw-rw-   0        0        0     7464 2023-04-26 01:41:35.000000 spiralflow-0.0.3/spiralflow/tools.py
+drwxrwxrwx   0        0        0        0 2023-04-26 01:42:57.179188 spiralflow-0.0.3/spiralflow.egg-info/
+-rw-rw-rw-   0        0        0    12978 2023-04-26 01:42:56.000000 spiralflow-0.0.3/spiralflow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      350 2023-04-26 01:42:57.000000 spiralflow-0.0.3/spiralflow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 01:42:56.000000 spiralflow-0.0.3/spiralflow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-04-26 01:42:56.000000 spiralflow-0.0.3/spiralflow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-26 01:42:56.000000 spiralflow-0.0.3/spiralflow.egg-info/top_level.txt
```

### Comparing `spiralflow-0.0.2/LICENSE` & `spiralflow-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `spiralflow-0.0.2/PKG-INFO` & `spiralflow-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: spiralflow
-Version: 0.0.2
+Version: 0.0.3
 Summary: A framework for creating chat spirals for Large Language Models finetuned for conversations. Currently work-in-progress.
 Home-page: https://github.com/Tiger767/Spiralflow
 Author: Travis Hammond
 License: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# spiral-flow (Work-In-Progress)
+# spiralflow (Work-In-Progress)
 A framework for creating guided spirals for Large Language Models
 
 This project is designed to help with creating, formatting, and extracting data from text-based conversations with OpenAI language models to allow for more complicated ideas such as Flows and Spirals. It includes the following key components:
 
 *   `Message`: A base class representing a message with content, role, and variables.
 *   `InputMessage`: A class to create input messages with pre-defined content formats.
 *   `OutputMessage`: A class to create output messages and extract variables from them.
@@ -32,14 +32,17 @@
 *   `History`: A class that allows for more complicated flows of histories, utilizing the ChatHistoryManager.
 *   `MemoryChatFlow`: A class that allows a chat flow to query external memory.
 *   `ConditonalChatFlow`: A class to represent a conversation flow with multiple branches that depend on an output of a flow.
 *   `SequentialChatFlows`: A class to represent multiple conversation flows, flowing sequentially.
 *   `ConcurrentChatFlows`: A class to represent multiple conversation flows, flowing separately and concurrently.
 *   `ChatSpiral`: A class to represent a spiral of conversation flows.
 
+Example Projects
+------------
+[Data Chat](https://github.com/Tiger767/spiralflow-data-chat) - A constructued ChatFlow for responding to prompts using your data, google search results, and general LLM knowledge.
 
 Installation
 ------------
 
 To use this project, you will need to install the required dependencies:
 
 1.  Install Python 3.9 or higher.
```

### Comparing `spiralflow-0.0.2/README.md` & `spiralflow-0.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# spiral-flow (Work-In-Progress)
+# spiralflow (Work-In-Progress)
 A framework for creating guided spirals for Large Language Models
 
 This project is designed to help with creating, formatting, and extracting data from text-based conversations with OpenAI language models to allow for more complicated ideas such as Flows and Spirals. It includes the following key components:
 
 *   `Message`: A base class representing a message with content, role, and variables.
 *   `InputMessage`: A class to create input messages with pre-defined content formats.
 *   `OutputMessage`: A class to create output messages and extract variables from them.
@@ -18,14 +18,17 @@
 *   `History`: A class that allows for more complicated flows of histories, utilizing the ChatHistoryManager.
 *   `MemoryChatFlow`: A class that allows a chat flow to query external memory.
 *   `ConditonalChatFlow`: A class to represent a conversation flow with multiple branches that depend on an output of a flow.
 *   `SequentialChatFlows`: A class to represent multiple conversation flows, flowing sequentially.
 *   `ConcurrentChatFlows`: A class to represent multiple conversation flows, flowing separately and concurrently.
 *   `ChatSpiral`: A class to represent a spiral of conversation flows.
 
+Example Projects
+------------
+[Data Chat](https://github.com/Tiger767/spiralflow-data-chat) - A constructued ChatFlow for responding to prompts using your data, google search results, and general LLM knowledge.
 
 Installation
 ------------
 
 To use this project, you will need to install the required dependencies:
 
 1.  Install Python 3.9 or higher.
```

### Comparing `spiralflow-0.0.2/setup.py` & `spiralflow-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="spiralflow",
-    version="0.0.2",
+    version="0.0.3",
     author="Travis Hammond",
     description="A framework for creating chat spirals for Large Language Models finetuned for conversations. Currently work-in-progress.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Tiger767/Spiralflow",
     packages=setuptools.find_packages(),
     install_requires=[
```

### Comparing `spiralflow-0.0.2/spiralflow/chat_history.py` & `spiralflow-0.0.3/spiralflow/chat_history.py`

 * *Files identical despite different names*

### Comparing `spiralflow-0.0.2/spiralflow/chat_llm.py` & `spiralflow-0.0.3/spiralflow/chat_llm.py`

 * *Files identical despite different names*

### Comparing `spiralflow-0.0.2/spiralflow/flow.py` & `spiralflow-0.0.3/spiralflow/flow.py`

 * *Files 0% similar despite different names*

```diff
@@ -549,25 +549,28 @@
         Runs the chat flow through an LLM.
 
         :param input_variables: Dictionary of input variables.
         :param chat_llm: Optional chat language model to use for the chat flow.
         :param input_chat_history: Optional input chat history. Will not be used, but internal chat flow may use default.
         :return: Tuple of dictionary of output variables and a tuple of empty input and internal chat histories.
         """
+        original_input_chat_history = input_chat_history
         if not self._allow_input_history:
             input_chat_history = None
         if self._disallow_default_history:
             input_chat_history = ChatHistory()
 
         variables, histories = self._chat_flow.flow(
             input_variables, chat_llm=chat_llm, input_chat_history=input_chat_history
         )
 
         if not self._allow_rtn_internal_history:
             histories = (histories[0], [])
+        if not self._allow_input_history:
+            histories = ([original_input_chat_history], histories[1])
         if not self._allow_rtn_input_history:
             histories = ([], histories[1])
 
         return variables, histories
 
 
 class NoOldSystemHistory(ChatFlowWrapper):
@@ -1277,14 +1280,25 @@
         self,
         input_variables: dict,
         reset_history: bool = False,
         chat_llm: Optional[ChatLLM] = None,
         input_chat_history: Optional[ChatHistory] = None,
         max_iterations: Optional[int] = None,
     ) -> Tuple[Dict[str, str], ChatHistory]:
+        """
+        Runs the chat flow through an LLM continuously.
+
+        :param input_variables: Dictionary of input variables.
+        :param reset_history: Whether to reset the chat history after each chat flow completion.
+        :param chat_llm: Optional chat language model to use for the chat flow.
+        :param input_chat_history: Optional input chat history.
+        :param max_iterations: Maximum number of iterations to run through the chat flow.
+
+        :return: Tuple of dictionary of output variables and chat history
+        """
         variables = dict(input_variables)
         chat_history = input_chat_history
         try:
             count = 0
             while True:
                 if max_iterations is not None and count >= max_iterations:
                     raise ChatSpiral.Exit
@@ -1307,14 +1321,26 @@
         input_variables: dict,
         reset_history: bool = False,
         chat_llm: Optional[ChatLLM] = None,
         input_chat_history: Optional[ChatHistory] = None,
         max_iterations: Optional[int] = None,
         return_all: bool = True,
     ) -> Tuple[Dict[str, str], ChatHistory]:
+        """
+        Runs the chat flow through an LLM continuously.
+
+        :param input_variables: Dictionary of input variables.
+        :param reset_history: Whether to reset the chat history after each chat flow completion.
+        :param chat_llm: Optional chat language model to use for the chat flow.
+        :param input_chat_history: Optional input chat history.
+        :param max_iterations: Maximum number of iterations to run through the chat flow.
+        :param return_all: Whether to return all output variables.
+
+        :return: Tuple of dictionary of output variables and chat history
+        """
         variables, history = self.spiral(
             input_variables,
             reset_history=reset_history,
             chat_llm=chat_llm,
             input_chat_history=input_chat_history,
             max_iterations=max_iterations,
         )
```

### Comparing `spiralflow-0.0.2/spiralflow/memory.py` & `spiralflow-0.0.3/spiralflow/memory.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 import numpy as np
 import pandas as pd
 import faiss
 from typing import Dict, Optional
 import pickle
-import tiktoken
 from openai.embeddings_utils import get_embedding
 
 
 def combine_on_overlap(str1: str, str2: str, threshold: float) -> Optional[str]:
     """
     Combines two strings if they overlap by a certain threshold.
-
     :param str1: First string to combine.
     :param str2: Second string to combine.
     :param threshold: Threshold for ratio of overlap to combine results from multiple queries.
     :return: Combined string if they overlap by a certain threshold, otherwise None.
     """
-    if str1 in str2:
-        return str2
-    if str2 in str1:
-        return str1
 
     max_overlap = min(len(str1), len(str2))
     best_overlap = 0
     best_overlap_index = -1
     overlap_type = None
 
     # Check for overlaps at the end of str1 and the beginning of str2
@@ -52,27 +46,22 @@
 
 
 class Memory:
     def __init__(
         self,
         filepath: Optional[str] = None,
         embedding_model: str = "text-embedding-ada-002",
-        max_tokens: int = 500,
     ) -> None:
         """
         Initializes the memory.
-
         :param filepath: Path to a pickle file to load and save the memory to.
                          If None, the memory is created with text and metadata fields.
         :param embedding_model: Model to use for the embedding.
-        :param max_tokens: Maximum number of tokens to use for the embedding.
         """
         self.embedding_model = embedding_model
-        self.max_tokens = max_tokens
-        self.encoding = tiktoken.encoding_for_model(self.embedding_model)
 
         if filepath is None:
             self.data = pd.DataFrame(columns=["text", "metadata"])
             self.index = None
         else:
             self.filepath = filepath
             self.load()
@@ -81,60 +70,49 @@
         _, d = embeddings.shape
         self.index = faiss.IndexFlatL2(d)
         self.index.add(embeddings)
 
     def save(self, filepath: Optional[str] = None) -> None:
         """
         Saves the memory to a file.
-
         :param filepath: Path to the pickle file to save the memory to. If None, the filepath passed in the constructor is used.
         """
         if filepath is None:
             filepath = self.filepath
 
-        self.encoding, encoding = None, self.encoding
         with open(filepath + ".pkl", "wb") as f:
             pickle.dump(self, f)
-        self.encoding = encoding
 
     def load(self, filepath: Optional[str] = None) -> None:
         """
         :param filepath: Path to a pickle file to load the memory from. If None, the filepath passed in the constructor is used.
         """
         if filepath is None:
             filepath = self.filepath
 
         with open(filepath, "rb") as f:
             loaded_memory = pickle.load(f)
             self.data = loaded_memory.data
             self.index = loaded_memory.index
             self.embedding_model = loaded_memory.embedding_model
-            self.max_tokens = loaded_memory.max_tokens
-            self.encoding = tiktoken.encoding_for_model(self.embedding_model)
 
     def add(
         self, data: Dict[str, str], save: bool = False, filepath: Optional[str] = None
     ) -> None:
         """
         Adds data to memory.
-
         :param data: Dict of data with a text and metadata field to add to memory.
         :param save: Whether to save the memory to a file.
         :param filepath: Path to the file (csv or parquet) to save the memory to.
                          If None, the filepath passed in the constructor is used.
         """
 
         if "text" not in data:
             raise ValueError("Data must have a 'text' field.")
 
-        if len(self.encoding.encode(data["text"])) > self.max_tokens:
-            raise ValueError(
-                "Text must be less than {} tokens.".format(self.max_tokens)
-            )
-
         # get embedding of text
         embedding = np.array(
             [get_embedding(data["text"], engine=self.embedding_model)], dtype=np.float32
         )
 
         data = pd.DataFrame(data, index=[0])
         self.data = pd.concat([self.data, data], ignore_index=True)
@@ -148,31 +126,25 @@
             self.save(filepath)
 
     def query(
         self, query: str, k: int = 1, combine_threshold: Optional[float] = None
     ) -> list[Dict[str, str]]:
         """
         Queries the memory with the given query.
-
         :param query: Query to use to get memory.
         :param k: Max number of results to return.
         :param combine_threshold: Threshold for ratio of overlap to combine results from multiple queries.
                                   If None, no combining is done.
         :return: Memory obtained from external memories.
         """
         if self.data.empty:
             raise ValueError(
                 "No memory to query. Add data to memory by calling Memory.add() before querying."
             )
 
-        if len(self.encoding.encode(query)) > self.max_tokens:
-            raise ValueError(
-                "Text must be less than {} tokens.".format(self.max_tokens)
-            )
-
         # get embedding of query
         embeded_query = np.array([get_embedding(query, engine=self.embedding_model)])
 
         # search for the indexes with similar embeddings
         scores, similar_indexes = self.index.search(embeded_query, k=k)
 
         print(scores)
```

### Comparing `spiralflow-0.0.2/spiralflow/message.py` & `spiralflow-0.0.3/spiralflow/message.py`

 * *Files identical despite different names*

### Comparing `spiralflow-0.0.2/spiralflow.egg-info/PKG-INFO` & `spiralflow-0.0.3/spiralflow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: spiralflow
-Version: 0.0.2
+Version: 0.0.3
 Summary: A framework for creating chat spirals for Large Language Models finetuned for conversations. Currently work-in-progress.
 Home-page: https://github.com/Tiger767/Spiralflow
 Author: Travis Hammond
 License: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# spiral-flow (Work-In-Progress)
+# spiralflow (Work-In-Progress)
 A framework for creating guided spirals for Large Language Models
 
 This project is designed to help with creating, formatting, and extracting data from text-based conversations with OpenAI language models to allow for more complicated ideas such as Flows and Spirals. It includes the following key components:
 
 *   `Message`: A base class representing a message with content, role, and variables.
 *   `InputMessage`: A class to create input messages with pre-defined content formats.
 *   `OutputMessage`: A class to create output messages and extract variables from them.
@@ -32,14 +32,17 @@
 *   `History`: A class that allows for more complicated flows of histories, utilizing the ChatHistoryManager.
 *   `MemoryChatFlow`: A class that allows a chat flow to query external memory.
 *   `ConditonalChatFlow`: A class to represent a conversation flow with multiple branches that depend on an output of a flow.
 *   `SequentialChatFlows`: A class to represent multiple conversation flows, flowing sequentially.
 *   `ConcurrentChatFlows`: A class to represent multiple conversation flows, flowing separately and concurrently.
 *   `ChatSpiral`: A class to represent a spiral of conversation flows.
 
+Example Projects
+------------
+[Data Chat](https://github.com/Tiger767/spiralflow-data-chat) - A constructued ChatFlow for responding to prompts using your data, google search results, and general LLM knowledge.
 
 Installation
 ------------
 
 To use this project, you will need to install the required dependencies:
 
 1.  Install Python 3.9 or higher.
```

