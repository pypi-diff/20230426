# Comparing `tmp/developergpt-0.2.3.tar.gz` & `tmp/developergpt-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "developergpt-0.2.3.tar", last modified: Mon Apr 17 16:09:06 2023, max compression
+gzip compressed data, was "developergpt-0.2.4.tar", last modified: Tue Apr 25 16:13:46 2023, max compression
```

## Comparing `developergpt-0.2.3.tar` & `developergpt-0.2.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:09:06.212778 developergpt-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-17 16:08:56.000000 developergpt-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-17 16:08:56.000000 developergpt-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-04-17 16:09:06.212778 developergpt-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-04-17 16:08:56.000000 developergpt-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:09:06.208778 developergpt-0.2.3/developergpt/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-17 16:08:56.000000 developergpt-0.2.3/developergpt/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 16:08:56.000000 developergpt-0.2.3/developergpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-17 16:08:56.000000 developergpt-0.2.3/developergpt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7615 2023-04-17 16:08:56.000000 developergpt-0.2.3/developergpt/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-17 16:08:56.000000 developergpt-0.2.3/developergpt/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10663 2023-04-17 16:08:56.000000 developergpt-0.2.3/developergpt/huggingface_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9380 2023-04-17 16:08:56.000000 developergpt-0.2.3/developergpt/openai_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7741 2023-04-17 16:08:56.000000 developergpt-0.2.3/developergpt/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:09:06.212778 developergpt-0.2.3/developergpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-04-17 16:09:06.000000 developergpt-0.2.3/developergpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-17 16:09:06.000000 developergpt-0.2.3/developergpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 16:09:06.000000 developergpt-0.2.3/developergpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-17 16:09:06.000000 developergpt-0.2.3/developergpt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-17 16:09:06.000000 developergpt-0.2.3/developergpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-17 16:09:06.000000 developergpt-0.2.3/developergpt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 16:09:06.212778 developergpt-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-17 16:08:56.000000 developergpt-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:09:06.212778 developergpt-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 16:08:56.000000 developergpt-0.2.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-17 16:08:56.000000 developergpt-0.2.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-17 16:08:56.000000 developergpt-0.2.3/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:13:46.332788 developergpt-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-25 16:13:29.000000 developergpt-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-25 16:13:29.000000 developergpt-0.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-04-25 16:13:46.328788 developergpt-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-04-25 16:13:29.000000 developergpt-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:13:46.328788 developergpt-0.2.4/developergpt/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-25 16:13:29.000000 developergpt-0.2.4/developergpt/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:13:29.000000 developergpt-0.2.4/developergpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-25 16:13:29.000000 developergpt-0.2.4/developergpt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7615 2023-04-25 16:13:29.000000 developergpt-0.2.4/developergpt/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-25 16:13:29.000000 developergpt-0.2.4/developergpt/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10663 2023-04-25 16:13:29.000000 developergpt-0.2.4/developergpt/huggingface_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9380 2023-04-25 16:13:29.000000 developergpt-0.2.4/developergpt/openai_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7741 2023-04-25 16:13:29.000000 developergpt-0.2.4/developergpt/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:13:46.328788 developergpt-0.2.4/developergpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-04-25 16:13:46.000000 developergpt-0.2.4/developergpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-25 16:13:46.000000 developergpt-0.2.4/developergpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 16:13:46.000000 developergpt-0.2.4/developergpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-25 16:13:46.000000 developergpt-0.2.4/developergpt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-25 16:13:46.000000 developergpt-0.2.4/developergpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-25 16:13:46.000000 developergpt-0.2.4/developergpt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 16:13:46.332788 developergpt-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-25 16:13:29.000000 developergpt-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:13:46.328788 developergpt-0.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:13:29.000000 developergpt-0.2.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-25 16:13:29.000000 developergpt-0.2.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-25 16:13:29.000000 developergpt-0.2.4/tests/test_cli.py
```

### Comparing `developergpt-0.2.3/LICENSE` & `developergpt-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `developergpt-0.2.3/PKG-INFO` & `developergpt-0.2.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,21 @@
-Metadata-Version: 2.1
-Name: developergpt
-Version: 0.2.3
-Summary: developergpt is a command line tool that allows users to use natural language to execute commands and chat with the latest LLMs
-Home-page: https://github.com/luo-anthony/DeveloperGPT/
-Author: luo-anthony
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE
-
 # DeveloperGPT
 [![License](https://img.shields.io/badge/license-MIT-green)](./LICENSE)
 [![CI](https://github.com/luo-anthony/DeveloperGPT/actions/workflows/main.yml/badge.svg)](https://github.com/luo-anthony/DeveloperGPT/actions/workflows/main.yml)
 [![PyPI](https://img.shields.io/pypi/v/developergpt)](https://pypi.org/project/developergpt/)
 [![LLMs](https://img.shields.io/badge/Supported%20LLMs-GPT3.5,%20BLOOM-blue)](https://img.shields.io/badge/Supported%20LLMs-GPT3.5,%20BLOOM-blue)
 
 
 <!-- [![codecov](https://codecov.io/gh/luo-anthony/DeveloperGPT/branch/main/graph/badge.svg?token=DeveloperGPT_token_here)](https://codecov.io/gh/luo-anthony/DeveloperGPT) -->
 
-DeveloperGPT is a terminal application that uses the latest LLMs to help developers be more productive. 
+DeveloperGPT is a terminal application that uses the latest LLMs to help developers be more productive. It is one of the first developer productivity terminal applications that supports **open source LLMs** such as the [BLOOM](https://bigscience.huggingface.co/blog/bloom) model in addition to OpenAI GPT LLMs. 
 
-By default, DeveloperGPT uses the [gpt-3.5-turbo](https://platform.openai.com/docs/models) model from OpenAI, but you can also use the open-source [BLOOM](https://bigscience.huggingface.co/blog/bloom) model. Support for more models and features is coming soon! 
+By default, DeveloperGPT uses the [gpt-3.5-turbo](https://platform.openai.com/docs/models) model from OpenAI (requires an OpenAI API Key), but it also supports the open-source [BLOOM](https://bigscience.huggingface.co/blog/bloom) model. Using BLOOM with DeveloperGPT is **completely free** and does **not require an API key** (rate-limited) thanks to the Hugging Face Inference API. 
 
-In our testing, we recommend GPT-3.5 (default) as it generally yields better results and is able to handle more complex requests. 
+In our testing, GPT-3.5 (default) generally yields better results and is able to handle more complex requests. 
 
 DeveloperGPT has two main features:
 #### 1. Natural Language to Terminal Commands
 **Supported Models:** GPT3.5 (default), BLOOM
 ![Natural Language Example](https://github.com/luo-anthony/DeveloperGPT/raw/main/samples/cmddemo.gif)
 
 **NOTE:** The BLOOM model command output may not be accurate, especially for more complex commands. Using the BLOOM model may also result in unexpected or undefined behavior. 
@@ -56,15 +45,15 @@
 # set OpenAI API Key (using zsh for example)
 $ echo 'export OPENAI_API_KEY=[your_key_here]' >> ~/.zshenv
 
 # reload the environment (or just quit and open a new terminal)
 $ source ~/.zshenv
 ```
 
-If you want to use the BLOOM model instead, you can optionally set up a [Hugging Face User Access](https://huggingface.co/settings/tokens) or [Inference API](https://huggingface.co/docs/api-inference/index) token. Setting up a token is not required (BLOOM model will work without any token or key), but it will allow you to make more requests without being rate limited. 
+To use the BLOOM model instead, you can optionally set up a [Hugging Face User Access](https://huggingface.co/settings/tokens) or [Inference API](https://huggingface.co/docs/api-inference/index) token. Setting up a token is not required (BLOOM model will work without any token or key), but it will allow you to make more requests without being rate limited. 
 
 ```bash
 # Do this once 
 # set Hugging Face API token (using zsh for example)
 $ echo 'export HUGGING_FACE_API_KEY=[your_key_here]' >> ~/.zshenv
 
 # reload the environment (or just quit and open a new terminal)
@@ -88,15 +77,15 @@
 # natural langauge to terminal commands using BLOOM model instead
 $ developergpt --model bloom cmd
 
 # give feedback
 $ developergpt feedback
 ```
 
-**NOTE:**: DeveloperGPT is **NOT** to be used for any purposes forbidden by the terms of use of the LLMs used (GPT-3.5, BLOOM). Additionally, DeveloperGPT itself (apart from the LLMs) is a proof of concept tool and is not intended to be used for any serious or commerical work. 
+**NOTE:** DeveloperGPT is **NOT** to be used for any purposes forbidden by the terms of use of the LLMs used (GPT-3.5, BLOOM). Additionally, DeveloperGPT itself (apart from the LLMs) is a proof of concept tool and is not intended to be used for any serious or commerical work. 
 
 ### OpenAI API Usage (GPT-3.5)
 You can monitor your OpenAI API usage here: https://platform.openai.com/account/usage
 
 DeveloperGPT uses the `gpt-3.5-turbo` model which is very cost efficient (1/10 the cost of models such as `text-davinci-003`). Based on preliminary testing, using DeveloperGPT should cost no more than 10 cents per day (assuming ~100 requests/day). 
 
 ### Hugging-Face Usage (BLOOM)
@@ -107,8 +96,7 @@
 
 ### Future Roadmap
 - Add support for open-source models (Alpaca, Vicuna, Dolly, etc.)
 
 ## Credit
 - Thanks to Hugging Face and the NLP community for open-source models and prompts! 
 - This project uses the Python project template from https://github.com/rochacbruno/python-project-template
-- This project was written with assistance from ChatGPT and Github CoPilot.
```

### Comparing `developergpt-0.2.3/README.md` & `developergpt-0.2.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,32 @@
+Metadata-Version: 2.1
+Name: developergpt
+Version: 0.2.4
+Summary: developergpt is a command line tool that allows users to use natural language to execute commands and chat with the latest LLMs
+Home-page: https://github.com/luo-anthony/DeveloperGPT/
+Author: luo-anthony
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+Provides-Extra: test
+License-File: LICENSE
+
 # DeveloperGPT
 [![License](https://img.shields.io/badge/license-MIT-green)](./LICENSE)
 [![CI](https://github.com/luo-anthony/DeveloperGPT/actions/workflows/main.yml/badge.svg)](https://github.com/luo-anthony/DeveloperGPT/actions/workflows/main.yml)
 [![PyPI](https://img.shields.io/pypi/v/developergpt)](https://pypi.org/project/developergpt/)
 [![LLMs](https://img.shields.io/badge/Supported%20LLMs-GPT3.5,%20BLOOM-blue)](https://img.shields.io/badge/Supported%20LLMs-GPT3.5,%20BLOOM-blue)
 
 
 <!-- [![codecov](https://codecov.io/gh/luo-anthony/DeveloperGPT/branch/main/graph/badge.svg?token=DeveloperGPT_token_here)](https://codecov.io/gh/luo-anthony/DeveloperGPT) -->
 
-DeveloperGPT is a terminal application that uses the latest LLMs to help developers be more productive. 
+DeveloperGPT is a terminal application that uses the latest LLMs to help developers be more productive. It is one of the first developer productivity terminal applications that supports **open source LLMs** such as the [BLOOM](https://bigscience.huggingface.co/blog/bloom) model in addition to OpenAI GPT LLMs. 
 
-By default, DeveloperGPT uses the [gpt-3.5-turbo](https://platform.openai.com/docs/models) model from OpenAI, but you can also use the open-source [BLOOM](https://bigscience.huggingface.co/blog/bloom) model. Support for more models and features is coming soon! 
+By default, DeveloperGPT uses the [gpt-3.5-turbo](https://platform.openai.com/docs/models) model from OpenAI (requires an OpenAI API Key), but it also supports the open-source [BLOOM](https://bigscience.huggingface.co/blog/bloom) model. Using BLOOM with DeveloperGPT is **completely free** and does **not require an API key** (rate-limited) thanks to the Hugging Face Inference API. 
 
-In our testing, we recommend GPT-3.5 (default) as it generally yields better results and is able to handle more complex requests. 
+In our testing, GPT-3.5 (default) generally yields better results and is able to handle more complex requests. 
 
 DeveloperGPT has two main features:
 #### 1. Natural Language to Terminal Commands
 **Supported Models:** GPT3.5 (default), BLOOM
 ![Natural Language Example](https://github.com/luo-anthony/DeveloperGPT/raw/main/samples/cmddemo.gif)
 
 **NOTE:** The BLOOM model command output may not be accurate, especially for more complex commands. Using the BLOOM model may also result in unexpected or undefined behavior. 
@@ -45,15 +56,15 @@
 # set OpenAI API Key (using zsh for example)
 $ echo 'export OPENAI_API_KEY=[your_key_here]' >> ~/.zshenv
 
 # reload the environment (or just quit and open a new terminal)
 $ source ~/.zshenv
 ```
 
-If you want to use the BLOOM model instead, you can optionally set up a [Hugging Face User Access](https://huggingface.co/settings/tokens) or [Inference API](https://huggingface.co/docs/api-inference/index) token. Setting up a token is not required (BLOOM model will work without any token or key), but it will allow you to make more requests without being rate limited. 
+To use the BLOOM model instead, you can optionally set up a [Hugging Face User Access](https://huggingface.co/settings/tokens) or [Inference API](https://huggingface.co/docs/api-inference/index) token. Setting up a token is not required (BLOOM model will work without any token or key), but it will allow you to make more requests without being rate limited. 
 
 ```bash
 # Do this once 
 # set Hugging Face API token (using zsh for example)
 $ echo 'export HUGGING_FACE_API_KEY=[your_key_here]' >> ~/.zshenv
 
 # reload the environment (or just quit and open a new terminal)
@@ -77,15 +88,15 @@
 # natural langauge to terminal commands using BLOOM model instead
 $ developergpt --model bloom cmd
 
 # give feedback
 $ developergpt feedback
 ```
 
-**NOTE:**: DeveloperGPT is **NOT** to be used for any purposes forbidden by the terms of use of the LLMs used (GPT-3.5, BLOOM). Additionally, DeveloperGPT itself (apart from the LLMs) is a proof of concept tool and is not intended to be used for any serious or commerical work. 
+**NOTE:** DeveloperGPT is **NOT** to be used for any purposes forbidden by the terms of use of the LLMs used (GPT-3.5, BLOOM). Additionally, DeveloperGPT itself (apart from the LLMs) is a proof of concept tool and is not intended to be used for any serious or commerical work. 
 
 ### OpenAI API Usage (GPT-3.5)
 You can monitor your OpenAI API usage here: https://platform.openai.com/account/usage
 
 DeveloperGPT uses the `gpt-3.5-turbo` model which is very cost efficient (1/10 the cost of models such as `text-davinci-003`). Based on preliminary testing, using DeveloperGPT should cost no more than 10 cents per day (assuming ~100 requests/day). 
 
 ### Hugging-Face Usage (BLOOM)
@@ -96,8 +107,7 @@
 
 ### Future Roadmap
 - Add support for open-source models (Alpaca, Vicuna, Dolly, etc.)
 
 ## Credit
 - Thanks to Hugging Face and the NLP community for open-source models and prompts! 
 - This project uses the Python project template from https://github.com/rochacbruno/python-project-template
-- This project was written with assistance from ChatGPT and Github CoPilot.
```

### Comparing `developergpt-0.2.3/developergpt/cli.py` & `developergpt-0.2.4/developergpt/cli.py`

 * *Files identical despite different names*

### Comparing `developergpt-0.2.3/developergpt/config.py` & `developergpt-0.2.4/developergpt/config.py`

 * *Files identical despite different names*

### Comparing `developergpt-0.2.3/developergpt/huggingface_adapter.py` & `developergpt-0.2.4/developergpt/huggingface_adapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 
 TIMEOUT = 25  # seconds
 
 
 def model_command(user_input: str, console: "Console", api_token: str) -> str:
     model = "bigscience/bloom"
     client = InferenceAPIClient(model, token=api_token, timeout=TIMEOUT)
-    MAX_RESPONSE_TOKENS = 256
+    MAX_RESPONSE_TOKENS = 384
 
     messages = copy.deepcopy(BLOOM_EXAMPLE_CMDS)
     messages.append(format_user_cmd_request(user_input))
 
     model_input = model_input = (
         BLOOM_CMD_PROMPT + "\n" + "\n".join(messages) + "\nAssistant:"
     )
```

### Comparing `developergpt-0.2.3/developergpt/openai_adapter.py` & `developergpt-0.2.4/developergpt/openai_adapter.py`

 * *Files identical despite different names*

### Comparing `developergpt-0.2.3/developergpt/utils.py` & `developergpt-0.2.4/developergpt/utils.py`

 * *Files identical despite different names*

### Comparing `developergpt-0.2.3/developergpt.egg-info/PKG-INFO` & `developergpt-0.2.4/developergpt.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: developergpt
-Version: 0.2.3
+Version: 0.2.4
 Summary: developergpt is a command line tool that allows users to use natural language to execute commands and chat with the latest LLMs
 Home-page: https://github.com/luo-anthony/DeveloperGPT/
 Author: luo-anthony
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
@@ -14,19 +14,19 @@
 [![CI](https://github.com/luo-anthony/DeveloperGPT/actions/workflows/main.yml/badge.svg)](https://github.com/luo-anthony/DeveloperGPT/actions/workflows/main.yml)
 [![PyPI](https://img.shields.io/pypi/v/developergpt)](https://pypi.org/project/developergpt/)
 [![LLMs](https://img.shields.io/badge/Supported%20LLMs-GPT3.5,%20BLOOM-blue)](https://img.shields.io/badge/Supported%20LLMs-GPT3.5,%20BLOOM-blue)
 
 
 <!-- [![codecov](https://codecov.io/gh/luo-anthony/DeveloperGPT/branch/main/graph/badge.svg?token=DeveloperGPT_token_here)](https://codecov.io/gh/luo-anthony/DeveloperGPT) -->
 
-DeveloperGPT is a terminal application that uses the latest LLMs to help developers be more productive. 
+DeveloperGPT is a terminal application that uses the latest LLMs to help developers be more productive. It is one of the first developer productivity terminal applications that supports **open source LLMs** such as the [BLOOM](https://bigscience.huggingface.co/blog/bloom) model in addition to OpenAI GPT LLMs. 
 
-By default, DeveloperGPT uses the [gpt-3.5-turbo](https://platform.openai.com/docs/models) model from OpenAI, but you can also use the open-source [BLOOM](https://bigscience.huggingface.co/blog/bloom) model. Support for more models and features is coming soon! 
+By default, DeveloperGPT uses the [gpt-3.5-turbo](https://platform.openai.com/docs/models) model from OpenAI (requires an OpenAI API Key), but it also supports the open-source [BLOOM](https://bigscience.huggingface.co/blog/bloom) model. Using BLOOM with DeveloperGPT is **completely free** and does **not require an API key** (rate-limited) thanks to the Hugging Face Inference API. 
 
-In our testing, we recommend GPT-3.5 (default) as it generally yields better results and is able to handle more complex requests. 
+In our testing, GPT-3.5 (default) generally yields better results and is able to handle more complex requests. 
 
 DeveloperGPT has two main features:
 #### 1. Natural Language to Terminal Commands
 **Supported Models:** GPT3.5 (default), BLOOM
 ![Natural Language Example](https://github.com/luo-anthony/DeveloperGPT/raw/main/samples/cmddemo.gif)
 
 **NOTE:** The BLOOM model command output may not be accurate, especially for more complex commands. Using the BLOOM model may also result in unexpected or undefined behavior. 
@@ -56,15 +56,15 @@
 # set OpenAI API Key (using zsh for example)
 $ echo 'export OPENAI_API_KEY=[your_key_here]' >> ~/.zshenv
 
 # reload the environment (or just quit and open a new terminal)
 $ source ~/.zshenv
 ```
 
-If you want to use the BLOOM model instead, you can optionally set up a [Hugging Face User Access](https://huggingface.co/settings/tokens) or [Inference API](https://huggingface.co/docs/api-inference/index) token. Setting up a token is not required (BLOOM model will work without any token or key), but it will allow you to make more requests without being rate limited. 
+To use the BLOOM model instead, you can optionally set up a [Hugging Face User Access](https://huggingface.co/settings/tokens) or [Inference API](https://huggingface.co/docs/api-inference/index) token. Setting up a token is not required (BLOOM model will work without any token or key), but it will allow you to make more requests without being rate limited. 
 
 ```bash
 # Do this once 
 # set Hugging Face API token (using zsh for example)
 $ echo 'export HUGGING_FACE_API_KEY=[your_key_here]' >> ~/.zshenv
 
 # reload the environment (or just quit and open a new terminal)
@@ -88,15 +88,15 @@
 # natural langauge to terminal commands using BLOOM model instead
 $ developergpt --model bloom cmd
 
 # give feedback
 $ developergpt feedback
 ```
 
-**NOTE:**: DeveloperGPT is **NOT** to be used for any purposes forbidden by the terms of use of the LLMs used (GPT-3.5, BLOOM). Additionally, DeveloperGPT itself (apart from the LLMs) is a proof of concept tool and is not intended to be used for any serious or commerical work. 
+**NOTE:** DeveloperGPT is **NOT** to be used for any purposes forbidden by the terms of use of the LLMs used (GPT-3.5, BLOOM). Additionally, DeveloperGPT itself (apart from the LLMs) is a proof of concept tool and is not intended to be used for any serious or commerical work. 
 
 ### OpenAI API Usage (GPT-3.5)
 You can monitor your OpenAI API usage here: https://platform.openai.com/account/usage
 
 DeveloperGPT uses the `gpt-3.5-turbo` model which is very cost efficient (1/10 the cost of models such as `text-davinci-003`). Based on preliminary testing, using DeveloperGPT should cost no more than 10 cents per day (assuming ~100 requests/day). 
 
 ### Hugging-Face Usage (BLOOM)
@@ -107,8 +107,7 @@
 
 ### Future Roadmap
 - Add support for open-source models (Alpaca, Vicuna, Dolly, etc.)
 
 ## Credit
 - Thanks to Hugging Face and the NLP community for open-source models and prompts! 
 - This project uses the Python project template from https://github.com/rochacbruno/python-project-template
-- This project was written with assistance from ChatGPT and Github CoPilot.
```

### Comparing `developergpt-0.2.3/developergpt.egg-info/SOURCES.txt` & `developergpt-0.2.4/developergpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `developergpt-0.2.3/setup.py` & `developergpt-0.2.4/setup.py`

 * *Files identical despite different names*

