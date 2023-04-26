# Comparing `tmp/spacy_huggingface_pipelines-0.0.1.tar.gz` & `tmp/spacy_huggingface_pipelines-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacy_huggingface_pipelines-0.0.1.tar", last modified: Mon Apr 24 08:23:49 2023, max compression
+gzip compressed data, was "spacy_huggingface_pipelines-0.0.2.tar", last modified: Wed Apr 26 13:18:52 2023, max compression
```

## Comparing `spacy_huggingface_pipelines-0.0.1.tar` & `spacy_huggingface_pipelines-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-24 08:23:49.551715 spacy_huggingface_pipelines-0.0.1/
--rw-r--r--   0 vsts      (1001) docker     (122)     1073 2023-04-24 08:21:39.000000 spacy_huggingface_pipelines-0.0.1/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)      102 2023-04-24 08:21:39.000000 spacy_huggingface_pipelines-0.0.1/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)     9287 2023-04-24 08:23:49.551715 spacy_huggingface_pipelines-0.0.1/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     8223 2023-04-24 08:21:39.000000 spacy_huggingface_pipelines-0.0.1/README.md
--rw-r--r--   0 vsts      (1001) docker     (122)       88 2023-04-24 08:21:39.000000 spacy_huggingface_pipelines-0.0.1/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (122)     1573 2023-04-24 08:23:49.551715 spacy_huggingface_pipelines-0.0.1/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)      171 2023-04-24 08:21:39.000000 spacy_huggingface_pipelines-0.0.1/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-24 08:23:49.547715 spacy_huggingface_pipelines-0.0.1/spacy_huggingface_pipelines/
--rw-r--r--   0 vsts      (1001) docker     (122)      147 2023-04-24 08:21:39.000000 spacy_huggingface_pipelines-0.0.1/spacy_huggingface_pipelines/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-24 08:23:49.547715 spacy_huggingface_pipelines-0.0.1/spacy_huggingface_pipelines/tests/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-24 08:21:39.000000 spacy_huggingface_pipelines-0.0.1/spacy_huggingface_pipelines/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)       45 2023-04-24 08:21:39.000000 spacy_huggingface_pipelines-0.0.1/spacy_huggingface_pipelines/tests/enable_gpu.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2833 2023-04-24 08:21:39.000000 spacy_huggingface_pipelines-0.0.1/spacy_huggingface_pipelines/tests/test_pipeline_components.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3453 2023-04-24 08:21:39.000000 spacy_huggingface_pipelines-0.0.1/spacy_huggingface_pipelines/text_classification.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6049 2023-04-24 08:21:39.000000 spacy_huggingface_pipelines-0.0.1/spacy_huggingface_pipelines/token_classification.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-24 08:23:49.547715 spacy_huggingface_pipelines-0.0.1/spacy_huggingface_pipelines.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)     9287 2023-04-24 08:23:49.000000 spacy_huggingface_pipelines-0.0.1/spacy_huggingface_pipelines.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)      720 2023-04-24 08:23:49.000000 spacy_huggingface_pipelines-0.0.1/spacy_huggingface_pipelines.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-24 08:23:49.000000 spacy_huggingface_pipelines-0.0.1/spacy_huggingface_pipelines.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      183 2023-04-24 08:23:49.000000 spacy_huggingface_pipelines-0.0.1/spacy_huggingface_pipelines.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-24 08:23:49.000000 spacy_huggingface_pipelines-0.0.1/spacy_huggingface_pipelines.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)       61 2023-04-24 08:23:49.000000 spacy_huggingface_pipelines-0.0.1/spacy_huggingface_pipelines.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       28 2023-04-24 08:23:49.000000 spacy_huggingface_pipelines-0.0.1/spacy_huggingface_pipelines.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-26 13:18:52.302397 spacy_huggingface_pipelines-0.0.2/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1073 2023-04-26 13:18:35.000000 spacy_huggingface_pipelines-0.0.2/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      102 2023-04-26 13:18:35.000000 spacy_huggingface_pipelines-0.0.2/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)     9718 2023-04-26 13:18:52.302397 spacy_huggingface_pipelines-0.0.2/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     8455 2023-04-26 13:18:35.000000 spacy_huggingface_pipelines-0.0.2/README.md
+-rw-r--r--   0 vsts      (1001) docker     (122)       88 2023-04-26 13:18:35.000000 spacy_huggingface_pipelines-0.0.2/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (122)     1766 2023-04-26 13:18:52.306397 spacy_huggingface_pipelines-0.0.2/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)      171 2023-04-26 13:18:35.000000 spacy_huggingface_pipelines-0.0.2/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-26 13:18:52.302397 spacy_huggingface_pipelines-0.0.2/spacy_huggingface_pipelines/
+-rw-r--r--   0 vsts      (1001) docker     (122)      143 2023-04-26 13:18:35.000000 spacy_huggingface_pipelines-0.0.2/spacy_huggingface_pipelines/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-26 13:18:52.302397 spacy_huggingface_pipelines-0.0.2/spacy_huggingface_pipelines/tests/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-26 13:18:35.000000 spacy_huggingface_pipelines-0.0.2/spacy_huggingface_pipelines/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)       45 2023-04-26 13:18:35.000000 spacy_huggingface_pipelines-0.0.2/spacy_huggingface_pipelines/tests/enable_gpu.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3028 2023-04-26 13:18:35.000000 spacy_huggingface_pipelines-0.0.2/spacy_huggingface_pipelines/tests/test_pipeline_components.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3701 2023-04-26 13:18:35.000000 spacy_huggingface_pipelines-0.0.2/spacy_huggingface_pipelines/text_classification.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6764 2023-04-26 13:18:35.000000 spacy_huggingface_pipelines-0.0.2/spacy_huggingface_pipelines/token_classification.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-26 13:18:52.302397 spacy_huggingface_pipelines-0.0.2/spacy_huggingface_pipelines.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)     9718 2023-04-26 13:18:52.000000 spacy_huggingface_pipelines-0.0.2/spacy_huggingface_pipelines.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)      720 2023-04-26 13:18:52.000000 spacy_huggingface_pipelines-0.0.2/spacy_huggingface_pipelines.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-26 13:18:52.000000 spacy_huggingface_pipelines-0.0.2/spacy_huggingface_pipelines.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      183 2023-04-26 13:18:52.000000 spacy_huggingface_pipelines-0.0.2/spacy_huggingface_pipelines.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-26 13:18:52.000000 spacy_huggingface_pipelines-0.0.2/spacy_huggingface_pipelines.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)       61 2023-04-26 13:18:52.000000 spacy_huggingface_pipelines-0.0.2/spacy_huggingface_pipelines.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       28 2023-04-26 13:18:52.000000 spacy_huggingface_pipelines-0.0.2/spacy_huggingface_pipelines.egg-info/top_level.txt
```

### Comparing `spacy_huggingface_pipelines-0.0.1/LICENSE` & `spacy_huggingface_pipelines-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spacy_huggingface_pipelines-0.0.1/PKG-INFO` & `spacy_huggingface_pipelines-0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: spacy_huggingface_pipelines
-Version: 0.0.1
+Version: 0.0.2
 Summary: spaCy wrapper for Hugging Face Transformers pipelines
-Home-page: https://spacy.io
+Home-page: https://github.com/explosion/spacy-huggingface-pipelines
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
-Classifier: Development Status :: 5 - Production/Stable
+Project-URL: Release notes, https://github.com/explosion/spacy-huggingface-pipelines/releases
+Project-URL: Source, https://github.com/explosion/spacy-huggingface-pipelines
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
@@ -88,37 +90,36 @@
 
 ```ini
 [components.hf_token_pipe]
 factory = "hf_token_pipe"
 model = "dslim/bert-base-NER"     # Model name or path
 revision = "main"                 # Model revision
 aggregation_strategy = "average"  # "simple", "first", "average", "max"
-stride = 16                       # Use stride > 0 to process long texts in
-                                  # overlapping windows of the model max length.
-                                  # The value is the length of the window
-                                  # overlap in transformer tokenizer tokens,
-                                  # NOT the length of the stride.
+stride = 16                       # If stride >= 0, process long texts in
+                                  # overlapping windows of the model max
+                                  # length. The value is the length of the
+                                  # window overlap in transformer tokenizer
+                                  # tokens, NOT the length of the stride.
 kwargs = {}                       # Any additional arguments for
                                   # TokenClassificationPipeline
 alignment_mode = "strict"         # "strict", "contract", "expand"
 annotate = "ents"                 # "ents", "pos", "spans", "tag"
 annotate_spans_key = null         # Doc.spans key for annotate = "spans"
 scorer = null                     # Optional scorer
 ```
 
 #### `TokenClassificationPipeline` settings
 
 - `model`: The model name or path.
 - `revision`: The model revision. For production use, a specific git commit is
   recommended instead of the default `main`.
-- `stride`: For `stride > 0`, the text is processed in overlapping windows where
-  the `stride` setting specifies the number of overlapping tokens between
-  windows (NOT the stride length). If `stride` is `0`, then the text is
-  processed as a whole, which may lead to model errors for texts longer than the
-  model max length.
+- `stride`: For `stride >= 0`, the text is processed in overlapping windows
+  where the `stride` setting specifies the number of overlapping tokens between
+  windows (NOT the stride length). If `stride` is `None`, then the text may be
+  truncated. `stride` is only supported for fast tokenizers.
 - `aggregation_strategy`: The aggregation strategy determines the word-level
   tags for cases where subwords within one word do not receive the same
   predicted tag. See:
   https://huggingface.co/docs/transformers/main_classes/pipelines#transformers.TokenClassificationPipeline.aggregation_strategy
 - `kwargs`: Any additional arguments to
   [`TokenClassificationPipeline`](https://huggingface.co/docs/transformers/main_classes/pipelines#transformers.TokenClassificationPipeline).
 
@@ -237,14 +238,19 @@
 Both token and text classification support batching with `nlp.pipe`:
 
 ```python
 for doc in nlp.pipe(texts, batch_size=256):
     do_something(doc)
 ```
 
+If the component runs into an error processing a batch (e.g. on an empty text),
+`nlp.pipe` will back off to processing each text individually. If it runs into
+an error on an individual text, a warning is shown and the doc is returned
+without additional annotation.
+
 Switch to GPU:
 
 ```python
 import spacy
 spacy.require_gpu()
 
 for doc in nlp.pipe(texts):
```

#### html2text {}

```diff
@@ -1,27 +1,30 @@
-Metadata-Version: 2.1 Name: spacy_huggingface_pipelines Version: 0.0.1 Summary:
+Metadata-Version: 2.1 Name: spacy_huggingface_pipelines Version: 0.0.2 Summary:
 spaCy wrapper for Hugging Face Transformers pipelines Home-page: https://
-spacy.io Author: Explosion Author-email: contact@explosion.ai License: MIT
-Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
-:: Console Classifier: Intended Audience :: Developers Classifier: Intended
-Audience :: Science/Research Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
-:: POSIX :: Linux Classifier: Operating System :: MacOS :: MacOS X Classifier:
-Operating System :: Microsoft :: Windows Classifier: Programming Language ::
-Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
-Python: >=3.8 Description-Content-Type: text/markdown License-File: LICENSE
-[https://explosion.ai/assets/img/logo.svg] # spacy-huggingface-pipelines: Use
-pretrained transformer models for text and token classification This package
-provides [spaCy](https://github.com/explosion/spaCy) components to use
-pretrained [Hugging Face Transformers pipelines](https://huggingface.co/docs/
-transformers/main_classes/pipelines) for inference only. [![PyPi](https://
-img.shields.io/pypi/v/spacy-huggingface-pipelines.svg?style=flat-
+github.com/explosion/spacy-huggingface-pipelines Author: Explosion Author-
+email: contact@explosion.ai License: MIT Project-URL: Release notes, https://
+github.com/explosion/spacy-huggingface-pipelines/releases Project-URL: Source,
+https://github.com/explosion/spacy-huggingface-pipelines Classifier:
+Development Status :: 4 - Beta Classifier: Environment :: Console Classifier:
+Intended Audience :: Developers Classifier: Intended Audience :: Science/
+Research Classifier: Topic :: Scientific/Engineering Classifier: Topic ::
+Scientific/Engineering :: Artificial Intelligence Classifier: License :: OSI
+Approved :: MIT License Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
+:: Microsoft :: Windows Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Requires-Python: >=3.8
+Description-Content-Type: text/markdown License-File: LICENSE [https://
+explosion.ai/assets/img/logo.svg] # spacy-huggingface-pipelines: Use pretrained
+transformer models for text and token classification This package provides
+[spaCy](https://github.com/explosion/spaCy) components to use pretrained
+[Hugging Face Transformers pipelines](https://huggingface.co/docs/transformers/
+main_classes/pipelines) for inference only. [![PyPi](https://img.shields.io/
+pypi/v/spacy-huggingface-pipelines.svg?style=flat-
 square&logo=pypi&logoColor=white)](https://pypi.python.org/pypi/spacy-
 huggingface-pipelines) [![GitHub](https://img.shields.io/github/release/
 explosion/spacy-huggingface-pipelines/all.svg?style=flat-square&logo=github)]
 (https://github.com/explosion/spacy-huggingface-pipelines/releases) ## Features
 - Apply pretrained transformers models like [`dslim/bert-base-NER`](https://
 huggingface.co/dslim/bert-base-NER) and [`distilbert-base-uncased-finetuned-
 sst-2-english`](https://huggingface.co/distilbert-base-uncased-finetuned-sst-2-
@@ -45,30 +48,30 @@
 if you are loading pipelines in an environment with limited internet access,
 make sure the model is available in your [transformers cache directory](https:/
 /huggingface.co/docs/transformers/main/en/installation#cache-setup) and enable
 offline mode if needed. ### Token classification Config settings for
 `hf_token_pipe`: ```ini [components.hf_token_pipe] factory = "hf_token_pipe"
 model = "dslim/bert-base-NER" # Model name or path revision = "main" # Model
 revision aggregation_strategy = "average" # "simple", "first", "average", "max"
-stride = 16 # Use stride > 0 to process long texts in # overlapping windows of
-the model max length. # The value is the length of the window # overlap in
-transformer tokenizer tokens, # NOT the length of the stride. kwargs = {} # Any
+stride = 16 # If stride >= 0, process long texts in # overlapping windows of
+the model max # length. The value is the length of the # window overlap in
+transformer tokenizer # tokens, NOT the length of the stride. kwargs = {} # Any
 additional arguments for # TokenClassificationPipeline alignment_mode =
 "strict" # "strict", "contract", "expand" annotate = "ents" # "ents", "pos",
 "spans", "tag" annotate_spans_key = null # Doc.spans key for annotate = "spans"
 scorer = null # Optional scorer ``` #### `TokenClassificationPipeline` settings
 - `model`: The model name or path. - `revision`: The model revision. For
 production use, a specific git commit is recommended instead of the default
-`main`. - `stride`: For `stride > 0`, the text is processed in overlapping
+`main`. - `stride`: For `stride >= 0`, the text is processed in overlapping
 windows where the `stride` setting specifies the number of overlapping tokens
-between windows (NOT the stride length). If `stride` is `0`, then the text is
-processed as a whole, which may lead to model errors for texts longer than the
-model max length. - `aggregation_strategy`: The aggregation strategy determines
-the word-level tags for cases where subwords within one word do not receive the
-same predicted tag. See: https://huggingface.co/docs/transformers/main_classes/
+between windows (NOT the stride length). If `stride` is `None`, then the text
+may be truncated. `stride` is only supported for fast tokenizers. -
+`aggregation_strategy`: The aggregation strategy determines the word-level tags
+for cases where subwords within one word do not receive the same predicted tag.
+See: https://huggingface.co/docs/transformers/main_classes/
 pipelines#transformers.TokenClassificationPipeline.aggregation_strategy -
 `kwargs`: Any additional arguments to [`TokenClassificationPipeline`](https://
 huggingface.co/docs/transformers/main_classes/
 pipelines#transformers.TokenClassificationPipeline). #### spaCy settings -
 `alignment_mode` determines how transformer predictions are aligned to spaCy
 token boundaries as described for [`Doc.char_span`](https://spacy.io/api/
 doc#char_span). - `annotate` and `annotate_spans_key` configure how the
@@ -104,12 +107,16 @@
 docs/transformers/main_classes/
 pipelines#transformers.TextClassificationPipeline). #### Example ```python
 import spacy nlp = spacy.blank("en") nlp.add_pipe( "hf_text_pipe", config=
 {"model": "distilbert-base-uncased-finetuned-sst-2-english"}, ) doc = nlp("This
 is great!") print(doc.cats) # {'POSITIVE': 0.9998694658279419, 'NEGATIVE':
 0.00013048505934420973} ``` ### Batching and GPU Both token and text
 classification support batching with `nlp.pipe`: ```python for doc in nlp.pipe
-(texts, batch_size=256): do_something(doc) ``` Switch to GPU: ```python import
-spacy spacy.require_gpu() for doc in nlp.pipe(texts): do_something(doc) ``` ##
-Bug reports and issues Please report bugs in the [spaCy issue tracker](https://
-github.com/explosion/spaCy/issues) or open a new thread on the [discussion
-board](https://github.com/explosion/spaCy/discussions) for other issues.
+(texts, batch_size=256): do_something(doc) ``` If the component runs into an
+error processing a batch (e.g. on an empty text), `nlp.pipe` will back off to
+processing each text individually. If it runs into an error on an individual
+text, a warning is shown and the doc is returned without additional annotation.
+Switch to GPU: ```python import spacy spacy.require_gpu() for doc in nlp.pipe
+(texts): do_something(doc) ``` ## Bug reports and issues Please report bugs in
+the [spaCy issue tracker](https://github.com/explosion/spaCy/issues) or open a
+new thread on the [discussion board](https://github.com/explosion/spaCy/
+discussions) for other issues.
```

### Comparing `spacy_huggingface_pipelines-0.0.1/README.md` & `spacy_huggingface_pipelines-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -61,37 +61,36 @@
 
 ```ini
 [components.hf_token_pipe]
 factory = "hf_token_pipe"
 model = "dslim/bert-base-NER"     # Model name or path
 revision = "main"                 # Model revision
 aggregation_strategy = "average"  # "simple", "first", "average", "max"
-stride = 16                       # Use stride > 0 to process long texts in
-                                  # overlapping windows of the model max length.
-                                  # The value is the length of the window
-                                  # overlap in transformer tokenizer tokens,
-                                  # NOT the length of the stride.
+stride = 16                       # If stride >= 0, process long texts in
+                                  # overlapping windows of the model max
+                                  # length. The value is the length of the
+                                  # window overlap in transformer tokenizer
+                                  # tokens, NOT the length of the stride.
 kwargs = {}                       # Any additional arguments for
                                   # TokenClassificationPipeline
 alignment_mode = "strict"         # "strict", "contract", "expand"
 annotate = "ents"                 # "ents", "pos", "spans", "tag"
 annotate_spans_key = null         # Doc.spans key for annotate = "spans"
 scorer = null                     # Optional scorer
 ```
 
 #### `TokenClassificationPipeline` settings
 
 - `model`: The model name or path.
 - `revision`: The model revision. For production use, a specific git commit is
   recommended instead of the default `main`.
-- `stride`: For `stride > 0`, the text is processed in overlapping windows where
-  the `stride` setting specifies the number of overlapping tokens between
-  windows (NOT the stride length). If `stride` is `0`, then the text is
-  processed as a whole, which may lead to model errors for texts longer than the
-  model max length.
+- `stride`: For `stride >= 0`, the text is processed in overlapping windows
+  where the `stride` setting specifies the number of overlapping tokens between
+  windows (NOT the stride length). If `stride` is `None`, then the text may be
+  truncated. `stride` is only supported for fast tokenizers.
 - `aggregation_strategy`: The aggregation strategy determines the word-level
   tags for cases where subwords within one word do not receive the same
   predicted tag. See:
   https://huggingface.co/docs/transformers/main_classes/pipelines#transformers.TokenClassificationPipeline.aggregation_strategy
 - `kwargs`: Any additional arguments to
   [`TokenClassificationPipeline`](https://huggingface.co/docs/transformers/main_classes/pipelines#transformers.TokenClassificationPipeline).
 
@@ -210,14 +209,19 @@
 Both token and text classification support batching with `nlp.pipe`:
 
 ```python
 for doc in nlp.pipe(texts, batch_size=256):
     do_something(doc)
 ```
 
+If the component runs into an error processing a batch (e.g. on an empty text),
+`nlp.pipe` will back off to processing each text individually. If it runs into
+an error on an individual text, a warning is shown and the doc is returned
+without additional annotation.
+
 Switch to GPU:
 
 ```python
 import spacy
 spacy.require_gpu()
 
 for doc in nlp.pipe(texts):
```

#### html2text {}

```diff
@@ -31,30 +31,30 @@
 if you are loading pipelines in an environment with limited internet access,
 make sure the model is available in your [transformers cache directory](https:/
 /huggingface.co/docs/transformers/main/en/installation#cache-setup) and enable
 offline mode if needed. ### Token classification Config settings for
 `hf_token_pipe`: ```ini [components.hf_token_pipe] factory = "hf_token_pipe"
 model = "dslim/bert-base-NER" # Model name or path revision = "main" # Model
 revision aggregation_strategy = "average" # "simple", "first", "average", "max"
-stride = 16 # Use stride > 0 to process long texts in # overlapping windows of
-the model max length. # The value is the length of the window # overlap in
-transformer tokenizer tokens, # NOT the length of the stride. kwargs = {} # Any
+stride = 16 # If stride >= 0, process long texts in # overlapping windows of
+the model max # length. The value is the length of the # window overlap in
+transformer tokenizer # tokens, NOT the length of the stride. kwargs = {} # Any
 additional arguments for # TokenClassificationPipeline alignment_mode =
 "strict" # "strict", "contract", "expand" annotate = "ents" # "ents", "pos",
 "spans", "tag" annotate_spans_key = null # Doc.spans key for annotate = "spans"
 scorer = null # Optional scorer ``` #### `TokenClassificationPipeline` settings
 - `model`: The model name or path. - `revision`: The model revision. For
 production use, a specific git commit is recommended instead of the default
-`main`. - `stride`: For `stride > 0`, the text is processed in overlapping
+`main`. - `stride`: For `stride >= 0`, the text is processed in overlapping
 windows where the `stride` setting specifies the number of overlapping tokens
-between windows (NOT the stride length). If `stride` is `0`, then the text is
-processed as a whole, which may lead to model errors for texts longer than the
-model max length. - `aggregation_strategy`: The aggregation strategy determines
-the word-level tags for cases where subwords within one word do not receive the
-same predicted tag. See: https://huggingface.co/docs/transformers/main_classes/
+between windows (NOT the stride length). If `stride` is `None`, then the text
+may be truncated. `stride` is only supported for fast tokenizers. -
+`aggregation_strategy`: The aggregation strategy determines the word-level tags
+for cases where subwords within one word do not receive the same predicted tag.
+See: https://huggingface.co/docs/transformers/main_classes/
 pipelines#transformers.TokenClassificationPipeline.aggregation_strategy -
 `kwargs`: Any additional arguments to [`TokenClassificationPipeline`](https://
 huggingface.co/docs/transformers/main_classes/
 pipelines#transformers.TokenClassificationPipeline). #### spaCy settings -
 `alignment_mode` determines how transformer predictions are aligned to spaCy
 token boundaries as described for [`Doc.char_span`](https://spacy.io/api/
 doc#char_span). - `annotate` and `annotate_spans_key` configure how the
@@ -90,12 +90,16 @@
 docs/transformers/main_classes/
 pipelines#transformers.TextClassificationPipeline). #### Example ```python
 import spacy nlp = spacy.blank("en") nlp.add_pipe( "hf_text_pipe", config=
 {"model": "distilbert-base-uncased-finetuned-sst-2-english"}, ) doc = nlp("This
 is great!") print(doc.cats) # {'POSITIVE': 0.9998694658279419, 'NEGATIVE':
 0.00013048505934420973} ``` ### Batching and GPU Both token and text
 classification support batching with `nlp.pipe`: ```python for doc in nlp.pipe
-(texts, batch_size=256): do_something(doc) ``` Switch to GPU: ```python import
-spacy spacy.require_gpu() for doc in nlp.pipe(texts): do_something(doc) ``` ##
-Bug reports and issues Please report bugs in the [spaCy issue tracker](https://
-github.com/explosion/spaCy/issues) or open a new thread on the [discussion
-board](https://github.com/explosion/spaCy/discussions) for other issues.
+(texts, batch_size=256): do_something(doc) ``` If the component runs into an
+error processing a batch (e.g. on an empty text), `nlp.pipe` will back off to
+processing each text individually. If it runs into an error on an individual
+text, a warning is shown and the doc is returned without additional annotation.
+Switch to GPU: ```python import spacy spacy.require_gpu() for doc in nlp.pipe
+(texts): do_something(doc) ``` ## Bug reports and issues Please report bugs in
+the [spaCy issue tracker](https://github.com/explosion/spaCy/issues) or open a
+new thread on the [discussion board](https://github.com/explosion/spaCy/
+discussions) for other issues.
```

### Comparing `spacy_huggingface_pipelines-0.0.1/setup.cfg` & `spacy_huggingface_pipelines-0.0.2/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 [metadata]
-version = 0.0.1
+version = 0.0.2
 description = spaCy wrapper for Hugging Face Transformers pipelines
-url = https://spacy.io
+url = https://github.com/explosion/spacy-huggingface-pipelines
 author = Explosion
 author_email = contact@explosion.ai
 license = MIT
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
-	Development Status :: 5 - Production/Stable
+	Development Status :: 4 - Beta
 	Environment :: Console
 	Intended Audience :: Developers
 	Intended Audience :: Science/Research
 	Topic :: Scientific/Engineering
 	Topic :: Scientific/Engineering :: Artificial Intelligence
 	License :: OSI Approved :: MIT License
 	Operating System :: POSIX :: Linux
 	Operating System :: MacOS :: MacOS X
 	Operating System :: Microsoft :: Windows
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+project_urls = 
+	Release notes = https://github.com/explosion/spacy-huggingface-pipelines/releases
+	Source = https://github.com/explosion/spacy-huggingface-pipelines
 
 [options]
 zip_safe = false
 include_package_data = true
 python_requires = >=3.8
 install_requires = 
 	spacy>=3.0.0,<4.0.0
```

### Comparing `spacy_huggingface_pipelines-0.0.1/spacy_huggingface_pipelines/tests/test_pipeline_components.py` & `spacy_huggingface_pipelines-0.0.2/spacy_huggingface_pipelines/tests/test_pipeline_components.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,21 @@
 
 torch.set_num_threads(1)
 
 
 @pytest.mark.parametrize("aggregation_strategy", ("simple", "first", "average", "max"))
 @pytest.mark.parametrize("annotate", ("ents", "spans", "tag"))
 @pytest.mark.parametrize("n_process", (1, 2))
-@pytest.mark.filterwarnings("ignore::UserWarning")
+@pytest.mark.filterwarnings(
+    "ignore:Unable to process, skipping annotation for doc ' ':UserWarning"
+)
+@pytest.mark.filterwarnings(
+    "ignore:Unable to process, skipping annotation for doc '':UserWarning"
+)
+@pytest.mark.filterwarnings("ignore:Unable to process texts as batch:UserWarning")
 def test_hf_token_pipe(aggregation_strategy, annotate, n_process):
     if (
         n_process > 1
         and isinstance(get_torch_default_device().index, int)
         and get_torch_default_device().index >= 0
     ):
         return
@@ -28,22 +34,22 @@
             "annotate": annotate,
             "annotate_spans_key": "tiny",
             "alignment_mode": "expand",
         },
     )
     doc = nlp("a")
     _check_tok_cls_annotation(doc, annotate)
-    doc = nlp("a bc def " * 1000)
+    doc = nlp("a b c d e f " * 1000)
     _check_tok_cls_annotation(doc, annotate)
 
     doc = nlp("")
     doc = nlp(" ")
 
     for doc in nlp.pipe(
-        ["a", "b", " ", "c", "", "aaaaabbbbccc bbbccc cccc", "a bc def " * 500],
+        ["a", "b", " ", "c", "", "a b c d e a b c d e", "a b c d e f " * 250],
         batch_size=2,
         n_process=n_process,
     ):
         _check_tok_cls_annotation(doc, annotate)
 
 
 def _check_tok_cls_annotation(doc, annotate):
@@ -58,15 +64,14 @@
         elif annotate == "spans":
             assert len(doc.spans["tiny"]) > 0
             for span in doc.spans["tiny"]:
                 assert span.label_.startswith("LABEL_")
 
 
 @pytest.mark.parametrize("n_process", (1, 2))
-@pytest.mark.filterwarnings("ignore::UserWarning")
 def test_hf_text_pipe(n_process):
     if (
         n_process > 1
         and isinstance(get_torch_default_device().index, int)
         and get_torch_default_device().index >= 0
     ):
         return
```

### Comparing `spacy_huggingface_pipelines-0.0.1/spacy_huggingface_pipelines/text_classification.py` & `spacy_huggingface_pipelines-0.0.2/spacy_huggingface_pipelines/text_classification.py`

 * *Files 9% similar despite different names*

```diff
@@ -36,35 +36,35 @@
     except Exception:
         device = -1
     if model == "":
         raise ValueError(
             "No model provided. Specify the model in your config, e.g.:\n\n"
             'nlp.add_pipe("hf_text_pipe", config={"model": "distilbert-base-uncased-finetuned-sst-2-english"})'
         )
-    tf_pipeline = pipeline(
+    hf_pipeline = pipeline(
         task="text-classification",
         model=model,
         revision=revision,
         device=device,
         truncation=True,
         **kwargs,
     )
-    return TrfTextPipe(
+    return HfTextPipe(
         name=name,
-        tf_pipeline=tf_pipeline,
+        hf_pipeline=hf_pipeline,
         scorer=scorer,
     )
 
 
-class TrfTextPipe(Pipe):
+class HfTextPipe(Pipe):
     def __init__(
-        self, name: str, tf_pipeline: pipeline, *, scorer: Optional[Callable] = None
+        self, name: str, hf_pipeline: pipeline, *, scorer: Optional[Callable] = None
     ):
         self.name = name
-        self.tf_pipeline = tf_pipeline
+        self.hf_pipeline = hf_pipeline
         self.scorer = scorer
 
     def __call__(self, doc: Doc) -> Doc:
         """Set transformers pipeline output on a spaCy Doc.
 
         doc (Doc): The doc to process.
         RETURNS (Doc): The spaCy Doc object.
@@ -75,35 +75,41 @@
         for docs in util.minibatch(stream, size=batch_size):
             outputs = self._get_annotations(docs, batch_size=batch_size)
             for doc, output in zip(docs, outputs):
                 doc.cats.update({a["label"]: a["score"] for a in output})
                 yield doc
 
     def _get_annotations(self, docs: List[Doc], batch_size) -> List[List[dict]]:
-        # TODO: warn when truncating? (I'm not sure you can detect this
-        # easily through the current pipeline API)
-        try:
-            with warnings.catch_warnings():
-                warnings.simplefilter("ignore", category=UserWarning)
-                return self.tf_pipeline(
-                    [doc.text for doc in docs], batch_size=batch_size, top_k=None
-                )
-        except Exception:
-            # TODO: better UX
-            pass
-        outputs = []
-        for doc in docs:
-            try:
-                with warnings.catch_warnings():
-                    warnings.simplefilter("ignore", category=UserWarning)
-                    outputs.append(self.tf_pipeline(doc.text, top_k=None))
-            except Exception:
-                # TODO: better UX
-                warnings.warn(f"Unable to process, skipping doc {repr(doc)}")
-                outputs.append([])
+        with warnings.catch_warnings():
+            warnings.filterwarnings(
+                "ignore",
+                message="You seem to be using the pipelines sequentially on GPU",
+                category=UserWarning,
+            )
+            if len(docs) > 1:
+                try:
+                    return self.hf_pipeline(
+                        [doc.text for doc in docs], batch_size=batch_size, top_k=None
+                    )
+                except Exception:
+                    warnings.warn(
+                        "Unable to process texts as batch, backing off to processing texts individually"
+                    )
+            outputs = []
+            for doc in docs:
+                try:
+                    outputs.append(self.hf_pipeline(doc.text, top_k=None))
+                except Exception:
+                    text_excerpt = (
+                        doc.text if len(doc.text) < 100 else doc.text[:100] + "..."
+                    )
+                    warnings.warn(
+                        f"Unable to process, skipping annotation for doc '{text_excerpt}'"
+                    )
+                    outputs.append([])
         return outputs
 
     # dummy serialization methods
     def to_bytes(self, **kwargs):
         return b""
 
     def from_bytes(self, _bytes_data, **kwargs):
```

### Comparing `spacy_huggingface_pipelines-0.0.1/spacy_huggingface_pipelines/token_classification.py` & `spacy_huggingface_pipelines-0.0.2/spacy_huggingface_pipelines/token_classification.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,17 +27,17 @@
     default_score_weights={},
 )
 def make_hf_token_pipe(
     nlp: Language,
     name: str,
     model: str,
     revision: str,
-    # maddeningly, the tokenizer stride is the size of the overlap, not the
-    # size of the stride (TODO: rename for this factory?)
-    stride: int,
+    # note that the tokenizer stride is the size of the overlap, not the size of
+    # the stride
+    stride: Optional[int],
     # this is intentionally omitting "none" from the aggregation strategies
     aggregation_strategy: Literal["simple", "first", "average", "max"],
     annotate: Literal["ents", "pos", "spans", "tag"],
     annotate_spans_key: Optional[str],
     alignment_mode: Literal["strict", "contract", "expand"],
     scorer: Optional[Callable],
     kwargs: dict,
@@ -49,46 +49,46 @@
     except Exception:
         device = -1
     if model == "":
         raise ValueError(
             "No model provided. Specify the model in your config, e.g.:\n\n"
             'nlp.add_pipe("hf_token_pipe", config={"model": "dslim/bert-base-NER"})'
         )
-    tf_pipeline = pipeline(
+    hf_pipeline = pipeline(
         task="token-classification",
         model=model,
         revision=revision,
         aggregation_strategy=aggregation_strategy,
         device=device,
         stride=stride,
         **kwargs,
     )
-    return TrfTokenPipe(
+    return HfTokenPipe(
         name=name,
-        tf_pipeline=tf_pipeline,
+        hf_pipeline=hf_pipeline,
         annotate=annotate,
         annotate_spans_key=annotate_spans_key,
         alignment_mode=alignment_mode,
         scorer=scorer,
     )
 
 
-class TrfTokenPipe(Pipe):
+class HfTokenPipe(Pipe):
     def __init__(
         self,
         name: str,
-        tf_pipeline: pipeline,
+        hf_pipeline: pipeline,
         *,
         annotate: Literal["ents", "pos", "spans", "tag"] = "ents",
         annotate_spans_key: Optional[str] = None,
         alignment_mode: str = "strict",
         scorer: Optional[Callable] = None,
     ):
         self.name = name
-        self.tf_pipeline = tf_pipeline
+        self.hf_pipeline = hf_pipeline
         self.annotate = annotate
         if self.annotate == "spans":
             if isinstance(annotate_spans_key, str):
                 self.annotate_spans_key = annotate_spans_key
             else:
                 raise ValueError(
                     "'annotate_spans_key' setting required to set spans annotations for hf_token_pipe"
@@ -116,41 +116,57 @@
                         if (
                             output_span is not None
                             and output_span.start_char >= prev_ann_end
                         ):
                             output_spans.append(output_span)
                             prev_ann_end = ann["end"]
                         else:
+                            text_excerpt = (
+                                doc.text
+                                if len(doc.text) < 100
+                                else doc.text[:100] + "..."
+                            )
                             warnings.warn(
-                                f"Skipping annotation, {ann} is overlapping or can't be aligned for span {repr(doc.text)}"
+                                f"Skipping annotation, {ann} is overlapping or can't be aligned for doc '{text_excerpt}'"
                             )
                 self._set_annotation_from_spans(doc, output_spans)
                 yield doc
 
     def _get_annotations(self, docs: List[Doc]) -> List[List[dict]]:
-        # TODO: warn when truncating? (I'm not sure you can detect this
-        # easily through the current pipeline API)
-        try:
-            with warnings.catch_warnings():
-                warnings.simplefilter("ignore", category=UserWarning)
-                return self.tf_pipeline([doc.text for doc in docs])
-        except Exception:
-            # TODO: better UX
-            pass
-        outputs = []
-        for doc in docs:
-            try:
-                with warnings.catch_warnings():
-                    warnings.simplefilter("ignore", category=UserWarning)
-                    outputs.append(self.tf_pipeline(doc.text))
-            except Exception:
-                # TODO: better UX
-                warnings.warn(f"Unable to process, skipping doc {repr(doc.text)}")
-                outputs.append([])
-        return outputs
+        with warnings.catch_warnings():
+            # the PipelineChunkIterator does not report its length correctly,
+            # leading to many spurious warnings from torch
+            warnings.filterwarnings(
+                "ignore", message="Length of IterableDataset", category=UserWarning
+            )
+            warnings.filterwarnings(
+                "ignore",
+                message="You seem to be using the pipelines sequentially on GPU",
+                category=UserWarning,
+            )
+            if len(docs) > 1:
+                try:
+                    return self.hf_pipeline([doc.text for doc in docs])
+                except Exception:
+                    warnings.warn(
+                        "Unable to process texts as batch, backing off to processing texts individually"
+                    )
+            outputs = []
+            for doc in docs:
+                try:
+                    outputs.append(self.hf_pipeline(doc.text))
+                except Exception:
+                    text_excerpt = (
+                        doc.text if len(doc.text) < 100 else doc.text[:100] + "..."
+                    )
+                    warnings.warn(
+                        f"Unable to process, skipping annotation for doc '{text_excerpt}'"
+                    )
+                    outputs.append([])
+            return outputs
 
     def _set_annotation_from_spans(self, doc: Doc, spans: List[Span]) -> Doc:
         if self.annotate == "ents":
             doc.set_ents(spans)
         elif self.annotate == "spans":
             doc.spans[self.annotate_spans_key] = spans
         elif self.annotate == "tag":
```

### Comparing `spacy_huggingface_pipelines-0.0.1/spacy_huggingface_pipelines.egg-info/PKG-INFO` & `spacy_huggingface_pipelines-0.0.2/spacy_huggingface_pipelines.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: spacy-huggingface-pipelines
-Version: 0.0.1
+Version: 0.0.2
 Summary: spaCy wrapper for Hugging Face Transformers pipelines
-Home-page: https://spacy.io
+Home-page: https://github.com/explosion/spacy-huggingface-pipelines
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
-Classifier: Development Status :: 5 - Production/Stable
+Project-URL: Release notes, https://github.com/explosion/spacy-huggingface-pipelines/releases
+Project-URL: Source, https://github.com/explosion/spacy-huggingface-pipelines
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
@@ -88,37 +90,36 @@
 
 ```ini
 [components.hf_token_pipe]
 factory = "hf_token_pipe"
 model = "dslim/bert-base-NER"     # Model name or path
 revision = "main"                 # Model revision
 aggregation_strategy = "average"  # "simple", "first", "average", "max"
-stride = 16                       # Use stride > 0 to process long texts in
-                                  # overlapping windows of the model max length.
-                                  # The value is the length of the window
-                                  # overlap in transformer tokenizer tokens,
-                                  # NOT the length of the stride.
+stride = 16                       # If stride >= 0, process long texts in
+                                  # overlapping windows of the model max
+                                  # length. The value is the length of the
+                                  # window overlap in transformer tokenizer
+                                  # tokens, NOT the length of the stride.
 kwargs = {}                       # Any additional arguments for
                                   # TokenClassificationPipeline
 alignment_mode = "strict"         # "strict", "contract", "expand"
 annotate = "ents"                 # "ents", "pos", "spans", "tag"
 annotate_spans_key = null         # Doc.spans key for annotate = "spans"
 scorer = null                     # Optional scorer
 ```
 
 #### `TokenClassificationPipeline` settings
 
 - `model`: The model name or path.
 - `revision`: The model revision. For production use, a specific git commit is
   recommended instead of the default `main`.
-- `stride`: For `stride > 0`, the text is processed in overlapping windows where
-  the `stride` setting specifies the number of overlapping tokens between
-  windows (NOT the stride length). If `stride` is `0`, then the text is
-  processed as a whole, which may lead to model errors for texts longer than the
-  model max length.
+- `stride`: For `stride >= 0`, the text is processed in overlapping windows
+  where the `stride` setting specifies the number of overlapping tokens between
+  windows (NOT the stride length). If `stride` is `None`, then the text may be
+  truncated. `stride` is only supported for fast tokenizers.
 - `aggregation_strategy`: The aggregation strategy determines the word-level
   tags for cases where subwords within one word do not receive the same
   predicted tag. See:
   https://huggingface.co/docs/transformers/main_classes/pipelines#transformers.TokenClassificationPipeline.aggregation_strategy
 - `kwargs`: Any additional arguments to
   [`TokenClassificationPipeline`](https://huggingface.co/docs/transformers/main_classes/pipelines#transformers.TokenClassificationPipeline).
 
@@ -237,14 +238,19 @@
 Both token and text classification support batching with `nlp.pipe`:
 
 ```python
 for doc in nlp.pipe(texts, batch_size=256):
     do_something(doc)
 ```
 
+If the component runs into an error processing a batch (e.g. on an empty text),
+`nlp.pipe` will back off to processing each text individually. If it runs into
+an error on an individual text, a warning is shown and the doc is returned
+without additional annotation.
+
 Switch to GPU:
 
 ```python
 import spacy
 spacy.require_gpu()
 
 for doc in nlp.pipe(texts):
```

#### html2text {}

```diff
@@ -1,27 +1,30 @@
-Metadata-Version: 2.1 Name: spacy-huggingface-pipelines Version: 0.0.1 Summary:
+Metadata-Version: 2.1 Name: spacy-huggingface-pipelines Version: 0.0.2 Summary:
 spaCy wrapper for Hugging Face Transformers pipelines Home-page: https://
-spacy.io Author: Explosion Author-email: contact@explosion.ai License: MIT
-Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
-:: Console Classifier: Intended Audience :: Developers Classifier: Intended
-Audience :: Science/Research Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
-:: POSIX :: Linux Classifier: Operating System :: MacOS :: MacOS X Classifier:
-Operating System :: Microsoft :: Windows Classifier: Programming Language ::
-Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
-Python: >=3.8 Description-Content-Type: text/markdown License-File: LICENSE
-[https://explosion.ai/assets/img/logo.svg] # spacy-huggingface-pipelines: Use
-pretrained transformer models for text and token classification This package
-provides [spaCy](https://github.com/explosion/spaCy) components to use
-pretrained [Hugging Face Transformers pipelines](https://huggingface.co/docs/
-transformers/main_classes/pipelines) for inference only. [![PyPi](https://
-img.shields.io/pypi/v/spacy-huggingface-pipelines.svg?style=flat-
+github.com/explosion/spacy-huggingface-pipelines Author: Explosion Author-
+email: contact@explosion.ai License: MIT Project-URL: Release notes, https://
+github.com/explosion/spacy-huggingface-pipelines/releases Project-URL: Source,
+https://github.com/explosion/spacy-huggingface-pipelines Classifier:
+Development Status :: 4 - Beta Classifier: Environment :: Console Classifier:
+Intended Audience :: Developers Classifier: Intended Audience :: Science/
+Research Classifier: Topic :: Scientific/Engineering Classifier: Topic ::
+Scientific/Engineering :: Artificial Intelligence Classifier: License :: OSI
+Approved :: MIT License Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
+:: Microsoft :: Windows Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Requires-Python: >=3.8
+Description-Content-Type: text/markdown License-File: LICENSE [https://
+explosion.ai/assets/img/logo.svg] # spacy-huggingface-pipelines: Use pretrained
+transformer models for text and token classification This package provides
+[spaCy](https://github.com/explosion/spaCy) components to use pretrained
+[Hugging Face Transformers pipelines](https://huggingface.co/docs/transformers/
+main_classes/pipelines) for inference only. [![PyPi](https://img.shields.io/
+pypi/v/spacy-huggingface-pipelines.svg?style=flat-
 square&logo=pypi&logoColor=white)](https://pypi.python.org/pypi/spacy-
 huggingface-pipelines) [![GitHub](https://img.shields.io/github/release/
 explosion/spacy-huggingface-pipelines/all.svg?style=flat-square&logo=github)]
 (https://github.com/explosion/spacy-huggingface-pipelines/releases) ## Features
 - Apply pretrained transformers models like [`dslim/bert-base-NER`](https://
 huggingface.co/dslim/bert-base-NER) and [`distilbert-base-uncased-finetuned-
 sst-2-english`](https://huggingface.co/distilbert-base-uncased-finetuned-sst-2-
@@ -45,30 +48,30 @@
 if you are loading pipelines in an environment with limited internet access,
 make sure the model is available in your [transformers cache directory](https:/
 /huggingface.co/docs/transformers/main/en/installation#cache-setup) and enable
 offline mode if needed. ### Token classification Config settings for
 `hf_token_pipe`: ```ini [components.hf_token_pipe] factory = "hf_token_pipe"
 model = "dslim/bert-base-NER" # Model name or path revision = "main" # Model
 revision aggregation_strategy = "average" # "simple", "first", "average", "max"
-stride = 16 # Use stride > 0 to process long texts in # overlapping windows of
-the model max length. # The value is the length of the window # overlap in
-transformer tokenizer tokens, # NOT the length of the stride. kwargs = {} # Any
+stride = 16 # If stride >= 0, process long texts in # overlapping windows of
+the model max # length. The value is the length of the # window overlap in
+transformer tokenizer # tokens, NOT the length of the stride. kwargs = {} # Any
 additional arguments for # TokenClassificationPipeline alignment_mode =
 "strict" # "strict", "contract", "expand" annotate = "ents" # "ents", "pos",
 "spans", "tag" annotate_spans_key = null # Doc.spans key for annotate = "spans"
 scorer = null # Optional scorer ``` #### `TokenClassificationPipeline` settings
 - `model`: The model name or path. - `revision`: The model revision. For
 production use, a specific git commit is recommended instead of the default
-`main`. - `stride`: For `stride > 0`, the text is processed in overlapping
+`main`. - `stride`: For `stride >= 0`, the text is processed in overlapping
 windows where the `stride` setting specifies the number of overlapping tokens
-between windows (NOT the stride length). If `stride` is `0`, then the text is
-processed as a whole, which may lead to model errors for texts longer than the
-model max length. - `aggregation_strategy`: The aggregation strategy determines
-the word-level tags for cases where subwords within one word do not receive the
-same predicted tag. See: https://huggingface.co/docs/transformers/main_classes/
+between windows (NOT the stride length). If `stride` is `None`, then the text
+may be truncated. `stride` is only supported for fast tokenizers. -
+`aggregation_strategy`: The aggregation strategy determines the word-level tags
+for cases where subwords within one word do not receive the same predicted tag.
+See: https://huggingface.co/docs/transformers/main_classes/
 pipelines#transformers.TokenClassificationPipeline.aggregation_strategy -
 `kwargs`: Any additional arguments to [`TokenClassificationPipeline`](https://
 huggingface.co/docs/transformers/main_classes/
 pipelines#transformers.TokenClassificationPipeline). #### spaCy settings -
 `alignment_mode` determines how transformer predictions are aligned to spaCy
 token boundaries as described for [`Doc.char_span`](https://spacy.io/api/
 doc#char_span). - `annotate` and `annotate_spans_key` configure how the
@@ -104,12 +107,16 @@
 docs/transformers/main_classes/
 pipelines#transformers.TextClassificationPipeline). #### Example ```python
 import spacy nlp = spacy.blank("en") nlp.add_pipe( "hf_text_pipe", config=
 {"model": "distilbert-base-uncased-finetuned-sst-2-english"}, ) doc = nlp("This
 is great!") print(doc.cats) # {'POSITIVE': 0.9998694658279419, 'NEGATIVE':
 0.00013048505934420973} ``` ### Batching and GPU Both token and text
 classification support batching with `nlp.pipe`: ```python for doc in nlp.pipe
-(texts, batch_size=256): do_something(doc) ``` Switch to GPU: ```python import
-spacy spacy.require_gpu() for doc in nlp.pipe(texts): do_something(doc) ``` ##
-Bug reports and issues Please report bugs in the [spaCy issue tracker](https://
-github.com/explosion/spaCy/issues) or open a new thread on the [discussion
-board](https://github.com/explosion/spaCy/discussions) for other issues.
+(texts, batch_size=256): do_something(doc) ``` If the component runs into an
+error processing a batch (e.g. on an empty text), `nlp.pipe` will back off to
+processing each text individually. If it runs into an error on an individual
+text, a warning is shown and the doc is returned without additional annotation.
+Switch to GPU: ```python import spacy spacy.require_gpu() for doc in nlp.pipe
+(texts): do_something(doc) ``` ## Bug reports and issues Please report bugs in
+the [spaCy issue tracker](https://github.com/explosion/spaCy/issues) or open a
+new thread on the [discussion board](https://github.com/explosion/spaCy/
+discussions) for other issues.
```

### Comparing `spacy_huggingface_pipelines-0.0.1/spacy_huggingface_pipelines.egg-info/SOURCES.txt` & `spacy_huggingface_pipelines-0.0.2/spacy_huggingface_pipelines.egg-info/SOURCES.txt`

 * *Files identical despite different names*

