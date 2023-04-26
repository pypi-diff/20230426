# Comparing `tmp/promptest-0.1.4.tar.gz` & `tmp/promptest-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptest-0.1.4.tar", last modified: Sat Apr 22 12:27:32 2023, max compression
+gzip compressed data, was "promptest-0.1.5.tar", last modified: Wed Apr 26 00:53:21 2023, max compression
```

## Comparing `promptest-0.1.4.tar` & `promptest-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 yenkel     (501) staff       (20)        0 2023-04-22 12:27:32.594483 promptest-0.1.4/
--rw-r--r--   0 yenkel     (501) staff       (20)     1075 2023-04-20 18:44:34.000000 promptest-0.1.4/LICENSE
--rw-r--r--   0 yenkel     (501) staff       (20)      156 2023-04-22 12:27:32.594375 promptest-0.1.4/PKG-INFO
--rw-r--r--   0 yenkel     (501) staff       (20)     4688 2023-04-21 22:50:59.000000 promptest-0.1.4/README.md
-drwxr-xr-x   0 yenkel     (501) staff       (20)        0 2023-04-22 12:27:32.593572 promptest-0.1.4/promptest/
--rw-r--r--   0 yenkel     (501) staff       (20)       32 2023-04-20 21:23:20.000000 promptest-0.1.4/promptest/__init__.py
--rw-r--r--   0 yenkel     (501) staff       (20)     2836 2023-04-20 21:23:43.000000 promptest-0.1.4/promptest/main.py
--rw-r--r--   0 yenkel     (501) staff       (20)     4129 2023-04-22 12:18:53.000000 promptest-0.1.4/promptest/tester.py
-drwxr-xr-x   0 yenkel     (501) staff       (20)        0 2023-04-22 12:27:32.594220 promptest-0.1.4/promptest.egg-info/
--rw-r--r--   0 yenkel     (501) staff       (20)      156 2023-04-22 12:27:32.000000 promptest-0.1.4/promptest.egg-info/PKG-INFO
--rw-r--r--   0 yenkel     (501) staff       (20)      286 2023-04-22 12:27:32.000000 promptest-0.1.4/promptest.egg-info/SOURCES.txt
--rw-r--r--   0 yenkel     (501) staff       (20)        1 2023-04-22 12:27:32.000000 promptest-0.1.4/promptest.egg-info/dependency_links.txt
--rw-r--r--   0 yenkel     (501) staff       (20)       51 2023-04-22 12:27:32.000000 promptest-0.1.4/promptest.egg-info/entry_points.txt
--rw-r--r--   0 yenkel     (501) staff       (20)       17 2023-04-22 12:27:32.000000 promptest-0.1.4/promptest.egg-info/requires.txt
--rw-r--r--   0 yenkel     (501) staff       (20)       10 2023-04-22 12:27:32.000000 promptest-0.1.4/promptest.egg-info/top_level.txt
--rw-r--r--   0 yenkel     (501) staff       (20)       38 2023-04-22 12:27:32.594524 promptest-0.1.4/setup.cfg
--rw-r--r--   0 yenkel     (501) staff       (20)      306 2023-04-22 12:26:47.000000 promptest-0.1.4/setup.py
+drwxr-xr-x   0 yenkel     (501) staff       (20)        0 2023-04-26 00:53:21.968479 promptest-0.1.5/
+-rw-r--r--   0 yenkel     (501) staff       (20)     1075 2023-04-20 18:44:34.000000 promptest-0.1.5/LICENSE
+-rw-r--r--   0 yenkel     (501) staff       (20)      156 2023-04-26 00:53:21.968364 promptest-0.1.5/PKG-INFO
+-rw-r--r--   0 yenkel     (501) staff       (20)     5120 2023-04-26 00:52:54.000000 promptest-0.1.5/README.md
+drwxr-xr-x   0 yenkel     (501) staff       (20)        0 2023-04-26 00:53:21.967444 promptest-0.1.5/promptest/
+-rw-r--r--   0 yenkel     (501) staff       (20)       32 2023-04-20 21:23:20.000000 promptest-0.1.5/promptest/__init__.py
+-rw-r--r--   0 yenkel     (501) staff       (20)     2893 2023-04-25 19:55:58.000000 promptest-0.1.5/promptest/main.py
+-rw-r--r--   0 yenkel     (501) staff       (20)     5487 2023-04-26 00:41:41.000000 promptest-0.1.5/promptest/tester.py
+drwxr-xr-x   0 yenkel     (501) staff       (20)        0 2023-04-26 00:53:21.968192 promptest-0.1.5/promptest.egg-info/
+-rw-r--r--   0 yenkel     (501) staff       (20)      156 2023-04-26 00:53:21.000000 promptest-0.1.5/promptest.egg-info/PKG-INFO
+-rw-r--r--   0 yenkel     (501) staff       (20)      286 2023-04-26 00:53:21.000000 promptest-0.1.5/promptest.egg-info/SOURCES.txt
+-rw-r--r--   0 yenkel     (501) staff       (20)        1 2023-04-26 00:53:21.000000 promptest-0.1.5/promptest.egg-info/dependency_links.txt
+-rw-r--r--   0 yenkel     (501) staff       (20)       51 2023-04-26 00:53:21.000000 promptest-0.1.5/promptest.egg-info/entry_points.txt
+-rw-r--r--   0 yenkel     (501) staff       (20)       28 2023-04-26 00:53:21.000000 promptest-0.1.5/promptest.egg-info/requires.txt
+-rw-r--r--   0 yenkel     (501) staff       (20)       10 2023-04-26 00:53:21.000000 promptest-0.1.5/promptest.egg-info/top_level.txt
+-rw-r--r--   0 yenkel     (501) staff       (20)       38 2023-04-26 00:53:21.968515 promptest-0.1.5/setup.cfg
+-rw-r--r--   0 yenkel     (501) staff       (20)      327 2023-04-25 17:02:24.000000 promptest-0.1.5/setup.py
```

### Comparing `promptest-0.1.4/LICENSE` & `promptest-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `promptest-0.1.4/README.md` & `promptest-0.1.5/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 Here, `/path/to/prompt.yaml` should be the path to a YAML file containing the template for your LLM, and `/path/to/inputs.yaml` should be the path to a YAML file containing the inputs for your tests.
 
 For more information on the command line arguments that `promptest` supports, run:
 ```bash
 promptest --help
 ```
 
-
 ## Example
 Here are a few examples of how to use `promptest` to test LLM prompts.
 
 ### Test output with exact match
 
 1. Create a YAML file `prompt.yaml` containing the template for your LLM:
     ```yaml
@@ -105,14 +104,19 @@
 
 ### Running the tests
 Run the following command to test the prompt templates:
 ```bash
 promptest --prompt prompt.yaml --tests tests.yaml
 ```
 
+### Supported models
+The following models are supported:
+- [OpenAI](https://platform.openai.com/docs/models): "gpt-4", "gpt-4-0314", "gpt-4-32k", "gpt-4-32k-0314", "gpt-3.5-turbo", "gpt-3.5-turbo-0301", "text-davinci-003", "text-davinci-002", "text-curie-001", "text-babbage-001", "text-ada-001"
+- [gpt4all](https://github.com/nomic-ai/pygpt4all#gpt4all-model): specify the path to the model as a string, e.g. "./model/gpt4all.bin"
+
 ### Output
 The tests output detailed results for each model, including the number of test cases passed and the pass ratio.
 
 When you run `promptest`, the tool will execute tests for each LLM model specified in the `tests.yaml` file. For each model, `promptest` will run the tests and output the results to the console. In addition to the console output, `promptest` will also create a file containing the detailed test results.
 
 The file will be named model_name_test_result.yml, where model_name is the name of the LLM model being tested (e.g., text-davinci-002, text-ada-001, etc.). The file will be written to a directory named prompt_test_results in the current working directory. The directory will be named with a timestamp and the name of the template file being used, in the following format:
 ```
```

### Comparing `promptest-0.1.4/promptest/main.py` & `promptest-0.1.5/promptest/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,15 +35,17 @@
             'total': total
         },
         'temperature': temperature,
         'max_tokens': max_tokens,
         'prompt_template': template
     }
 
-    filename = f"{model_name}_test_result.yml"
+    model_file_name = os.path.basename(model_name)
+
+    filename = f"{model_file_name}_test_result.yml"
     file_path = os.path.join(output_directory, filename)
 
     with open(file_path, 'w') as outfile:
         yaml.dump(test_data, outfile, default_flow_style=None, allow_unicode=True, width=float('inf'), line_break='\n')
 
 def parse_input_files(prompt_path, tests_path):
     with open(prompt_path, 'r') as file:
```

### Comparing `promptest-0.1.4/promptest/tester.py` & `promptest-0.1.5/promptest/tester.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,55 @@
 import re
 import os
-from langchain.llms import OpenAI
+from langchain.llms import OpenAI, GPT4All
 from langchain.chat_models import ChatOpenAI
 from langchain.chains import LLMChain
 from langchain.prompts import PromptTemplate
 from langchain.prompts.chat import (
     HumanMessagePromptTemplate,
     ChatPromptTemplate
 )
 import yaml
 
+
 CHAT_MODELS=["gpt-4", "gpt-4-0314", "gpt-4-32k", "gpt-4-32k-0314", "gpt-3.5-turbo", "gpt-3.5-turbo-0301"]
+COMPLETION_MODELS=["text-davinci-003", "text-davinci-002", "text-curie-001", "text-babbage-001", "text-ada-001"]
+
+def _extract_default_output(o):
+    return o.strip()
+
+def _extract_gpt4all_output(output_str):
+    answer = "Answer:"
+    index = output_str.find(answer)
+    if index != -1:
+        return output_str[index + len(answer):].strip()
+    else:
+        return ""
+
+def _create_llm_chain(model_name, template, input_variables, temperature, max_tokens):
+    extractor = _extract_default_output
+    if model_name in CHAT_MODELS:
+        llm = ChatOpenAI(model_name=model_name, temperature=temperature, max_tokens=max_tokens)
+        prompt_template = ChatPromptTemplate.from_messages([HumanMessagePromptTemplate.from_template(template=template)])
+    elif model_name in COMPLETION_MODELS:
+        llm = OpenAI(model_name=model_name, temperature=temperature, max_tokens=max_tokens)
+        prompt_template = PromptTemplate(template=template, input_variables=input_variables)
+    elif os.path.isabs(model_name) or model_name.startswith('./') or model_name.startswith('../'):
+        llm = GPT4All(model=model_name, temp=temperature, n_predict=max_tokens)
+        # we wrap the original template in a request/response format so
+        # - there's a better chance gpt4all does the right thing
+        # - we can parse the output after response
+        input_template=f'Question: {template}\nAnswer:'
+        prompt_template = PromptTemplate(template=input_template, input_variables=input_variables)
+        # we need to remove the question/answer template
+        extractor = _extract_gpt4all_output
+    else:
+        raise ValueError(f"Invalid model_name: {model_name}. Please use a valid OpenAI model or provide a relative/absolute path for a GPT4All model.")
+
+    return LLMChain(llm=llm, prompt=prompt_template), extractor
 
 def _compare_output(output, expected_output):
     if expected_output['type'] == 'regex':
         pattern = re.compile(expected_output['value'])
         return pattern.match(output) is not None, None
     elif expected_output['type'] == 'string':
         return output == expected_output['value'], None
@@ -40,58 +75,50 @@
         if model in CHAT_MODELS:
             llm = ChatOpenAI(model_name=model, temperature=0, max_tokens=1800)
             prompt_template = ChatPromptTemplate.from_messages([HumanMessagePromptTemplate.from_template(template=template)])
         else:
             llm = OpenAI(model_name=model, temperature=0, max_tokens=1800)
             prompt_template =  PromptTemplate(template=template, input_variables=['input_text', 'conditions'])
 
-        llm_chain = LLMChain(llm=llm, prompt=prompt_template, output_key='validation_result')
+        llm_chain, extractor = LLMChain(llm=llm, prompt=prompt_template, output_key='validation_result')
 
-        validation_result = llm_chain.predict(**params).strip()
+        validation_result = llm_chain.predict(**params)
 
         try:
             validation_result_yaml = yaml.safe_load(validation_result)
             overall_pass = validation_result_yaml.get('pass', False)
             return overall_pass, validation_result_yaml
         except yaml.YAMLError:
             return False
     else:
         return False
 
 def test_models(prompt_data, tests_data):
     template = prompt_data['template']
     input_variables = prompt_data['input_variables']
-    output_key = prompt_data['output_key']
 
     tests = tests_data['tests']
     model_names = tests_data['model_names']
     temperature = tests_data['temperature']
     max_tokens = tests_data['max_tokens']
 
     results = {}
 
     for model_name in model_names:
         total = 0
         passes = 0
         model_results = []
 
-        if model_name in CHAT_MODELS:
-            llm = ChatOpenAI(model_name=model_name, temperature=temperature, max_tokens=max_tokens)
-            prompt_template = ChatPromptTemplate.from_messages([HumanMessagePromptTemplate.from_template(template=template)])
-        else:
-            llm = OpenAI(model_name=model_name, temperature=temperature, max_tokens=max_tokens)
-            prompt_template = PromptTemplate(template=template, input_variables=input_variables)
-
-        llm_chain = LLMChain(llm=llm, prompt=prompt_template, output_key=output_key)
+        llm_chain, extractor = _create_llm_chain(model_name, template, input_variables, temperature, max_tokens)
 
         for item in tests:
             variables = item['variables']
             expected_output = item['expected_output']
 
-            result = llm_chain.predict(**variables).strip()
+            result = extractor(llm_chain.predict(**variables))
 
             comparison_result, extra_data = _compare_output(result, expected_output)
 
             if comparison_result:
                 passes += 1
 
             test_result = {
```

