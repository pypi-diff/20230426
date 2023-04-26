# Comparing `tmp/thinkgpt-0.0.4.tar.gz` & `tmp/thinkgpt-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thinkgpt-0.0.4.tar", max compression
+gzip compressed data, was "thinkgpt-0.0.5.tar", max compression
```

## Comparing `thinkgpt-0.0.4.tar` & `thinkgpt-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11357 2023-04-14 15:21:33.490604 thinkgpt-0.0.4/LICENSE
--rw-r--r--   0        0        0     6871 2023-04-20 23:12:15.079797 thinkgpt-0.0.4/README.md
--rw-r--r--   0        0        0      562 2023-04-24 01:10:43.645079 thinkgpt-0.0.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-14 15:28:05.934649 thinkgpt-0.0.4/thinkgpt/__init__.py
--rw-r--r--   0        0        0     4067 2023-04-24 00:39:46.959405 thinkgpt-0.0.4/thinkgpt/abstract.py
--rw-r--r--   0        0        0     2349 2023-04-24 00:39:46.956963 thinkgpt-0.0.4/thinkgpt/condition.py
--rw-r--r--   0        0        0     3668 2023-04-24 00:41:27.830853 thinkgpt-0.0.4/thinkgpt/gpt_select.py
--rw-r--r--   0        0        0     1165 2023-04-16 03:45:24.127522 thinkgpt-0.0.4/thinkgpt/helper.py
--rw-r--r--   0        0        0     2938 2023-04-24 00:43:29.599263 thinkgpt-0.0.4/thinkgpt/infer.py
--rw-r--r--   0        0        0     4453 2023-04-24 01:05:55.882845 thinkgpt-0.0.4/thinkgpt/llm.py
--rw-r--r--   0        0        0     2602 2023-04-24 00:49:11.780601 thinkgpt-0.0.4/thinkgpt/memory.py
--rw-r--r--   0        0        0     1742 2023-04-24 00:46:00.737818 thinkgpt-0.0.4/thinkgpt/refine.py
--rw-r--r--   0        0        0     3049 2023-04-24 00:46:00.734818 thinkgpt-0.0.4/thinkgpt/summarize.py
--rw-r--r--   0        0        0     7772 1970-01-01 00:00:00.000000 thinkgpt-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-14 15:21:33.490604 thinkgpt-0.0.5/LICENSE
+-rw-r--r--   0        0        0     8095 2023-04-25 15:24:53.616328 thinkgpt-0.0.5/README.md
+-rw-r--r--   0        0        0      562 2023-04-25 15:38:13.266488 thinkgpt-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-14 15:28:05.934649 thinkgpt-0.0.5/thinkgpt/__init__.py
+-rw-r--r--   0        0        0     3906 2023-04-24 17:17:15.104859 thinkgpt-0.0.5/thinkgpt/abstract.py
+-rw-r--r--   0        0        0     2190 2023-04-24 17:17:15.101408 thinkgpt-0.0.5/thinkgpt/condition.py
+-rw-r--r--   0        0        0     3650 2023-04-24 17:17:15.093655 thinkgpt-0.0.5/thinkgpt/gpt_select.py
+-rw-r--r--   0        0        0     1165 2023-04-16 03:45:24.127522 thinkgpt-0.0.5/thinkgpt/helper.py
+-rw-r--r--   0        0        0     2779 2023-04-24 17:17:15.108158 thinkgpt-0.0.5/thinkgpt/infer.py
+-rw-r--r--   0        0        0     4426 2023-04-25 15:26:36.146838 thinkgpt-0.0.5/thinkgpt/llm.py
+-rw-r--r--   0        0        0     2393 2023-04-24 17:17:15.111894 thinkgpt-0.0.5/thinkgpt/memory.py
+-rw-r--r--   0        0        0     1587 2023-04-24 17:17:15.115188 thinkgpt-0.0.5/thinkgpt/refine.py
+-rw-r--r--   0        0        0     2890 2023-04-24 17:17:15.097660 thinkgpt-0.0.5/thinkgpt/summarize.py
+-rw-r--r--   0        0        0     8996 1970-01-01 00:00:00.000000 thinkgpt-0.0.5/PKG-INFO
```

### Comparing `thinkgpt-0.0.4/LICENSE` & `thinkgpt-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `thinkgpt-0.0.4/README.md` & `thinkgpt-0.0.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -6,17 +6,18 @@
 * add intelligent decisions to your code base
 
 
 ## Key Features ✨
 * Thinking building blocks 🧱:
     * Memory 🧠: GPTs that can remember experience
     * Self-refinement 🔧: Improve model-generated content by addressing critics
-    * Abstraction 🌐: Encourages LLMs to generalize rules from examples or observations
+    * Compress knowledge 🌐: Compress knowledge and fit it in LLM's context either by anstracring rules out of observations or summarize large content
     * Inference 💡️: Make educated guesses based on available information
     * Natural Language Conditions 📝: Easily express choices and conditions in natural language
+    * Finetuning 📚: Agents that can learn by finetuning (coming soon!)
 * Efficient and Measurable GPT context length 📐
 * Extremely easy setup and pythonic API 🎯 thanks to [DocArray](https://github.com/docarray/docarray)
 
 ## Installation 💻
 You can install ThinkGPT using pip:
 
 ```shell
@@ -73,15 +74,39 @@
 ```text
 import re
 print('hello world')
 ```
 
 One of the applications is self-healing code generation implemented by projects like [gptdeploy](https://github.com/jina-ai/gptdeploy) and [wolverine](https://github.com/biobootloader/wolverine)
 
-### Induce rules from observations
+### Compressing knowledge
+In case you want your knowledge to fit into the LLM's context, you can use the following techniques to compress it:
+#### Summarize content
+Summarize content using the LLM itself.
+We offer 2 methods
+1. one-shot summarization using the LLM
+```python
+llm.summarize(
+  large_content,
+  max_tokens= 1000,
+  instruction_hint= 'Pay attention to code snippets, links and scientific terms.'
+)
+```
+Since this technique relies on summarizing using a single LLM call, you can only pass content that does not exceed the LLM's context length.
+2. Chunked summarization
+```python
+llm.chunked_summarize(
+  very_large_content,
+  max_tokens= 4096,
+  instruction_hint= 'Pay attention to code snippets, links and scientific terms.'
+)
+```
+This technique relies on splitting the content into different chunks, summarizing each of those chunks and then combining them all together using an LLM.
+
+#### Induce rules from observations
 Amount to higher level and more general observations from current observations:
 ```python
 llm.abstract(observations=[
     "in tunisian, I did not eat is \"ma khditech\"",
     "I did not work is \"ma khdemtech\"",
     "I did not go is \"ma mchitech\"",
 ])
@@ -107,17 +132,18 @@
 ```python
 llm.select(
     question="Which animal is the king of the jungle?",
     options=["Lion", "Elephant", "Tiger", "Giraffe"]
 )
 ```
 ```text
-Lion
+['Lion']
 ```
 
+You can also prompt the LLM to choose an exact number of answers using `num_choices`. By default, it's set to `None` which means the LLM will select any number he thinks it's correct.
 ## Use Cases 🚀
 Find out below example demos you can do with `thinkgpt`
 ### Teaching ThinkGPT a new language
 ```python
 from thinkgpt.llm import ThinkGPT
 
 llm = ThinkGPT(model_name="gpt-3.5-turbo")
```

### Comparing `thinkgpt-0.0.4/pyproject.toml` & `thinkgpt-0.0.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "thinkgpt"
-version = "0.0.4"
+version = "0.0.5"
 description = "ThinkGPT is a Python library aimed at implementing Chain of Thoughts for Large Language Models (LLMs), prompting the model to think, reason, and to create generative agents."
 authors = ["Alaeddine Abdessalem <alaeddine-13@live.fr>"]
 license = "Apache 2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.7,<4.0"
```

### Comparing `thinkgpt-0.0.4/thinkgpt/abstract.py` & `thinkgpt-0.0.5/thinkgpt/abstract.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,18 +82,14 @@
             return {'action': 'FINISH', 'value': text.strip()}
 
 class AbstractChain(LLMChain):
     """Prompts the LLM to request to remember memory as needed"""
     def __init__(self, **kwargs):
         super().__init__(prompt=ABSTRACTION_PROMPT, **kwargs)
 
-    @classmethod
-    def from_llm(cls, llm: BaseLLM, verbose: bool = True) -> LLMChain:
-        return cls(prompt=ABSTRACTION_PROMPT, llm=llm, verbose=verbose)
-
     def predict(self, instruction_hint: str = '', **kwargs: Any) -> str:
         return super().predict(instruction_hint=instruction_hint, **kwargs)
 
 
 class AbstractMixin:
     abstract_chain: AbstractChain
```

### Comparing `thinkgpt-0.0.4/thinkgpt/condition.py` & `thinkgpt-0.0.5/thinkgpt/condition.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,18 +51,14 @@
             return "Wrong format of the answer"
 
 
 class ConditionChain(LLMChain):
     def __init__(self, **kwargs):
         super().__init__(prompt=CONDITION_PROMPT, **kwargs)
 
-    @classmethod
-    def from_llm(cls, llm: BaseLLM, verbose: bool = True) -> LLMChain:
-        return cls(prompt=CONDITION_PROMPT, llm=llm, verbose=verbose)
-
     def predict(self, question: str, instruction_hint: str = '', **kwargs: Any) -> bool:
         result = super().predict(question=question, instruction_hint=instruction_hint, **kwargs)
         return ConditionOutputParser().parse(result)
 
 
 class ConditionMixin:
     condition_chain: ConditionChain
```

### Comparing `thinkgpt-0.0.4/thinkgpt/gpt_select.py` & `thinkgpt-0.0.5/thinkgpt/gpt_select.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,23 +9,28 @@
 SELECT_EXAMPLES = [
     {
         "question": "Which animal is known as the king of the jungle?",
         "options_text": '\n'.join(["Lion", "Elephant", "Tiger", "Giraffe"]),
         "answer": "Lion"
     },
     {
-        "question": "Which planet is closest to the Sun?",
-        "options_text": '\n'.join(["Mars", "Earth", "Venus", "Mercury"]),
-        "answer": "Mercury"
-    },
-    {
         "question": "What color do you get when you mix blue and yellow?",
         "options_text": '\n'.join(["Green", "Orange", "Purple", "Brown"]),
         "answer": "Green"
     },
+    {
+        "question": "Which animal is a carnivore?",
+        "options_text": '\n'.join(["Lion", "Elephant", "Tiger", "Giraffe"]),
+        "answer": "Lion\nTiger"
+    },
+    {
+        "question": "Which of these are plants?",
+        "options_text": '\n'.join(["Lily", "Giraffe", "Cactus", "Rose"]),
+        "answer": "Lily\nGiraffe\nCactus\nRose"
+    },
 ]
 
 SELECT_EXAMPLE_PROMPT = PromptTemplate(template="""
 Question:
 {question}
 
 Options:
@@ -39,57 +44,51 @@
 
 def format_options(options: List[str]) -> str:
     return "\n".join(options)
 
 
 
 
-class SelectOutputParser(BaseOutputParser[Optional[str]]):
+class SelectOutputParser(BaseOutputParser[List[str]]):
     options: List[str]
 
-    def parse(self, text: str) -> Optional[str]:
-        if text.strip().lower() not in [option.lower() for option in self.options]:
-            return None
-        return text.strip()
+    def parse(self, text: str) -> List[str]:
+        results = []
+        answers = text.split('\n')
+        for answer in answers:
+            if answer.strip().lower() in [option.lower() for option in self.options]:
+                results.append(answer.strip())
+        return results
 
 
 class SelectChain(LLMChain):
     def __init__(self, select_examples: Optional[List] = None, **kwargs):
         SELECT_PROMPT = FewShotPromptTemplate(
-            prefix="Choose the correct answer for the following question from the provided options.",
+            prefix="Choose the correct answer(s) for the following question from the provided options. If there are "
+                   "many answers, return each one in a separate line. {num_choices_hint}",
             examples=select_examples or SELECT_EXAMPLES,
             example_prompt=SELECT_EXAMPLE_PROMPT,
             suffix="{instruction_hint}\nQuestion:\n{question}\nOptions:\n{options_text}\nAnswer:\n",
-            input_variables=["instruction_hint", "question", "options_text"]
+            input_variables=["instruction_hint", "question", "options_text", "num_choices_hint"]
         )
         super().__init__(prompt=SELECT_PROMPT, **kwargs)
 
-    @classmethod
-    def from_llm(cls, llm: BaseLLM, select_examples: Optional[List] = None, verbose: bool = True) -> LLMChain:
-        SELECT_PROMPT = FewShotPromptTemplate(
-            prefix="Choose the correct answer for the following question from the provided options.",
-            examples=select_examples or SELECT_EXAMPLES,
-            example_prompt=SELECT_EXAMPLE_PROMPT,
-            suffix="{instruction_hint}\nQuestion:\n{question}\nOptions:\n{options_text}\nAnswer:\n",
-            input_variables=["instruction_hint", "question", "options_text"]
-        )
-        return cls(prompt=SELECT_PROMPT, llm=llm, verbose=verbose)
-
-    def predict(self, question: str, options: List[str], instruction_hint: str = '', **kwargs: Any) -> str:
+    def predict(self, question: str, options: List[str], instruction_hint: str = '', num_choices: int = None, **kwargs: Any) -> List[str]:
+        num_choices_hint = f"Return exactly {num_choices} answer" if num_choices else ''
         options_text = format_options(options)
-        result = super().predict(question=question, options_text=options_text, instruction_hint=instruction_hint,
+        result = super().predict(question=question, options_text=options_text, instruction_hint=instruction_hint, num_choices_hint=num_choices_hint,
                                  **kwargs)
         return SelectOutputParser(options=options).parse(result)
 
 
 class SelectMixin:
     select_chain: SelectChain
 
-    def select(self, question: str, options: List[str], instruction_hint: str = '', select_chain: Optional[SelectChain] = None) -> str:
+    def select(self, question: str, options: List[str], instruction_hint: str = '', select_chain: Optional[SelectChain] = None, num_choices: int = None) -> List[str]:
        chain = select_chain or self.select_chain
-       return chain.predict(question=question, options=options, instruction_hint=instruction_hint)
+       return chain.predict(question=question, options=options, instruction_hint=instruction_hint, num_choices=num_choices)
 
 
 if __name__ == '__main__':
     chain = SelectChain(llm=ChatOpenAI(model_name="gpt-3.5-turbo"))
     print(chain.predict(question="Which animal is known as the king of the jungle?",
                         options=["Lion", "Elephant", "Tiger", "Giraffe"], instruction_hint=""))
```

### Comparing `thinkgpt-0.0.4/thinkgpt/helper.py` & `thinkgpt-0.0.5/thinkgpt/helper.py`

 * *Files identical despite different names*

### Comparing `thinkgpt-0.0.4/thinkgpt/infer.py` & `thinkgpt-0.0.5/thinkgpt/infer.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,18 +50,14 @@
 
 
 class InferChain(LLMChain):
     """Prompts the LLM to generate new observations based on the given facts"""
     def __init__(self, **kwargs):
         super().__init__(prompt=INFERENCE_PROMPT, **kwargs)
 
-    @classmethod
-    def from_llm(cls, llm: BaseLLM, verbose: bool = True) -> LLMChain:
-        return cls(prompt=INFERENCE_PROMPT, llm=llm, verbose=verbose)
-
     def predict(self, instruction_hint: str = '', **kwargs: Any) -> str:
         return super().predict(instruction_hint=instruction_hint, **kwargs)
 
 
 class InferMixin:
     infer_chain: InferChain
```

### Comparing `thinkgpt-0.0.4/thinkgpt/llm.py` & `thinkgpt-0.0.5/thinkgpt/llm.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
                  # TODO: model name can be specified per mixin
                  **kwargs
                  ):
         super().__init__(**kwargs)
         # TODO: offer more docarray backends
         self.memory = memory or DocumentArray()
         self.embeddings_model = OpenAIEmbeddings()
-        self.openai = ChatOpenAI(model_name=kwargs.get('model_name'))
+        self.openai = ChatOpenAI(**kwargs)
         self.execute_with_context_chain = execute_with_context_chain or ExecuteWithContextChain(
             llm=self.openai, verbose=verbose)
         self.abstract_chain = abstract_chain or AbstractChain(
             llm=self.openai, verbose=verbose)
         self.refine_chain = refine_chain or RefineChain(
             llm=self.openai, verbose=verbose)
         self.condition_chain = condition_chain or ConditionChain(
```

### Comparing `thinkgpt-0.0.4/thinkgpt/memory.py` & `thinkgpt-0.0.5/thinkgpt/memory.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,19 +17,14 @@
 
 
 class ExecuteWithContextChain(LLMChain):
     """Prompts the LLM to execute a request with potential context"""
     def __init__(self, **kwargs):
         super().__init__(prompt=EXECUTE_WITH_CONTEXT_PROMPT, **kwargs)
 
-    @classmethod
-    def from_llm(cls, llm: BaseLLM, verbose: bool = True) -> LLMChain:
-        """Get the response parser."""
-        return cls(prompt=EXECUTE_WITH_CONTEXT_PROMPT, llm=llm, verbose=verbose)
-
 
 class MemoryMixin:
     memory: DocumentArray
     mem_cnt: int
     embeddings_model: OpenAIEmbeddings
 
     def memorize(self, concept: Union[str, Document, DocumentArray, List]):
```

### Comparing `thinkgpt-0.0.4/thinkgpt/refine.py` & `thinkgpt-0.0.5/thinkgpt/refine.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,17 +18,14 @@
 
 
 class RefineChain(LLMChain):
     """Prompts the LLM to request to remember memory as needed"""
     def __init__(self, **kwargs):
         super().__init__(prompt=REFINE_PROMPT, **kwargs)
 
-    @classmethod
-    def from_llm(cls, llm: BaseLLM, verbose: bool = True) -> LLMChain:
-        return cls(prompt=REFINE_PROMPT, llm=llm, verbose=verbose)
 
     def predict(self, instruction_hint: str = '', **kwargs: Any) -> str:
         return super().predict(instruction_hint=instruction_hint, **kwargs)
 
 
 class RefineMixin:
     refine_chain: RefineChain
```

### Comparing `thinkgpt-0.0.4/thinkgpt/summarize.py` & `thinkgpt-0.0.5/thinkgpt/summarize.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,18 +21,14 @@
     def __init__(self,
                  summarizer_chunk_size: int = 3000,
                  **kwargs
                  ):
         super().__init__(prompt=SUMMARIZE_PROMPT, **kwargs)
         self.summarizer_chunk_size = summarizer_chunk_size
 
-    @classmethod
-    def from_llm(cls, llm: BaseLLM, verbose: bool = True) -> LLMChain:
-        return cls(prompt=SUMMARIZE_PROMPT, llm=llm, verbose=verbose)
-
     def predict(self, content, **kwargs: Any) -> str:
         return super().predict(
             content=content,
             **kwargs)
 
 
 class SummarizeMixin:
```

### Comparing `thinkgpt-0.0.4/PKG-INFO` & `thinkgpt-0.0.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thinkgpt
-Version: 0.0.4
+Version: 0.0.5
 Summary: ThinkGPT is a Python library aimed at implementing Chain of Thoughts for Large Language Models (LLMs), prompting the model to think, reason, and to create generative agents.
 License: Apache 2.0
 Author: Alaeddine Abdessalem
 Author-email: alaeddine-13@live.fr
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -27,17 +27,18 @@
 * add intelligent decisions to your code base
 
 
 ## Key Features ✨
 * Thinking building blocks 🧱:
     * Memory 🧠: GPTs that can remember experience
     * Self-refinement 🔧: Improve model-generated content by addressing critics
-    * Abstraction 🌐: Encourages LLMs to generalize rules from examples or observations
+    * Compress knowledge 🌐: Compress knowledge and fit it in LLM's context either by anstracring rules out of observations or summarize large content
     * Inference 💡️: Make educated guesses based on available information
     * Natural Language Conditions 📝: Easily express choices and conditions in natural language
+    * Finetuning 📚: Agents that can learn by finetuning (coming soon!)
 * Efficient and Measurable GPT context length 📐
 * Extremely easy setup and pythonic API 🎯 thanks to [DocArray](https://github.com/docarray/docarray)
 
 ## Installation 💻
 You can install ThinkGPT using pip:
 
 ```shell
@@ -94,15 +95,39 @@
 ```text
 import re
 print('hello world')
 ```
 
 One of the applications is self-healing code generation implemented by projects like [gptdeploy](https://github.com/jina-ai/gptdeploy) and [wolverine](https://github.com/biobootloader/wolverine)
 
-### Induce rules from observations
+### Compressing knowledge
+In case you want your knowledge to fit into the LLM's context, you can use the following techniques to compress it:
+#### Summarize content
+Summarize content using the LLM itself.
+We offer 2 methods
+1. one-shot summarization using the LLM
+```python
+llm.summarize(
+  large_content,
+  max_tokens= 1000,
+  instruction_hint= 'Pay attention to code snippets, links and scientific terms.'
+)
+```
+Since this technique relies on summarizing using a single LLM call, you can only pass content that does not exceed the LLM's context length.
+2. Chunked summarization
+```python
+llm.chunked_summarize(
+  very_large_content,
+  max_tokens= 4096,
+  instruction_hint= 'Pay attention to code snippets, links and scientific terms.'
+)
+```
+This technique relies on splitting the content into different chunks, summarizing each of those chunks and then combining them all together using an LLM.
+
+#### Induce rules from observations
 Amount to higher level and more general observations from current observations:
 ```python
 llm.abstract(observations=[
     "in tunisian, I did not eat is \"ma khditech\"",
     "I did not work is \"ma khdemtech\"",
     "I did not go is \"ma mchitech\"",
 ])
@@ -128,17 +153,18 @@
 ```python
 llm.select(
     question="Which animal is the king of the jungle?",
     options=["Lion", "Elephant", "Tiger", "Giraffe"]
 )
 ```
 ```text
-Lion
+['Lion']
 ```
 
+You can also prompt the LLM to choose an exact number of answers using `num_choices`. By default, it's set to `None` which means the LLM will select any number he thinks it's correct.
 ## Use Cases 🚀
 Find out below example demos you can do with `thinkgpt`
 ### Teaching ThinkGPT a new language
 ```python
 from thinkgpt.llm import ThinkGPT
 
 llm = ThinkGPT(model_name="gpt-3.5-turbo")
```

