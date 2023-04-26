# Comparing `tmp/textrl-0.2.17.tar.gz` & `tmp/textrl-0.2.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textrl-0.2.17.tar", last modified: Wed Apr 26 09:05:01 2023, max compression
+gzip compressed data, was "textrl-0.2.18.tar", last modified: Wed Apr 26 09:35:25 2023, max compression
```

## Comparing `textrl-0.2.17.tar` & `textrl-0.2.18.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 voidful    (501) staff       (20)        0 2023-04-26 09:05:01.065431 textrl-0.2.17/
--rw-r--r--   0 voidful    (501) staff       (20)     4206 2022-12-05 09:09:02.000000 textrl-0.2.17/.gitignore
--rw-r--r--   0 voidful    (501) staff       (20)     1064 2023-02-09 14:54:56.000000 textrl-0.2.17/LICENSE
--rw-r--r--   0 voidful    (501) staff       (20)    18232 2023-04-26 09:05:01.065083 textrl-0.2.17/PKG-INFO
--rw-r--r--   0 voidful    (501) staff       (20)    17515 2023-04-25 10:23:10.000000 textrl-0.2.17/README.md
-drwxr-xr-x   0 voidful    (501) staff       (20)        0 2023-04-26 09:05:01.060263 textrl-0.2.17/example/
--rw-r--r--   0 voidful    (501) staff       (20)     7679 2023-03-27 13:57:09.000000 textrl-0.2.17/example/2022-12-10-textrl-elon-musk.ipynb
-drwxr-xr-x   0 voidful    (501) staff       (20)        0 2023-04-26 09:05:01.060544 textrl-0.2.17/img/
--rw-r--r--   0 voidful    (501) staff       (20)   373908 2023-04-17 05:47:18.000000 textrl-0.2.17/img/Designer.png
--rw-r--r--   0 voidful    (501) staff       (20)       61 2022-12-05 09:17:42.000000 textrl-0.2.17/requirement.txt
--rw-r--r--   0 voidful    (501) staff       (20)       38 2023-04-26 09:05:01.065506 textrl-0.2.17/setup.cfg
--rw-r--r--   0 voidful    (501) staff       (20)     1095 2023-04-26 09:04:05.000000 textrl-0.2.17/setup.py
-drwxr-xr-x   0 voidful    (501) staff       (20)        0 2023-04-26 09:05:01.063251 textrl-0.2.17/textrl/
--rw-r--r--   0 voidful    (501) staff       (20)      184 2023-02-13 19:45:54.000000 textrl-0.2.17/textrl/__init__.py
--rw-r--r--   0 voidful    (501) staff       (20)    13472 2023-04-26 08:50:57.000000 textrl-0.2.17/textrl/actor.py
--rw-r--r--   0 voidful    (501) staff       (20)     1140 2022-12-05 09:09:02.000000 textrl-0.2.17/textrl/dump.py
--rw-r--r--   0 voidful    (501) staff       (20)     7060 2023-04-26 08:59:31.000000 textrl-0.2.17/textrl/environment.py
--rw-r--r--   0 voidful    (501) staff       (20)    23448 2023-02-13 19:43:59.000000 textrl-0.2.17/textrl/evaluator.py
--rw-r--r--   0 voidful    (501) staff       (20)     7511 2023-02-13 19:43:59.000000 textrl-0.2.17/textrl/trainer.py
-drwxr-xr-x   0 voidful    (501) staff       (20)        0 2023-04-26 09:05:01.064761 textrl-0.2.17/textrl.egg-info/
--rw-r--r--   0 voidful    (501) staff       (20)    18232 2023-04-26 09:05:00.000000 textrl-0.2.17/textrl.egg-info/PKG-INFO
--rw-r--r--   0 voidful    (501) staff       (20)      433 2023-04-26 09:05:01.000000 textrl-0.2.17/textrl.egg-info/SOURCES.txt
--rw-r--r--   0 voidful    (501) staff       (20)        1 2023-04-26 09:05:00.000000 textrl-0.2.17/textrl.egg-info/dependency_links.txt
--rw-r--r--   0 voidful    (501) staff       (20)       50 2023-04-26 09:05:00.000000 textrl-0.2.17/textrl.egg-info/entry_points.txt
--rw-r--r--   0 voidful    (501) staff       (20)        1 2022-12-05 09:10:02.000000 textrl-0.2.17/textrl.egg-info/not-zip-safe
--rw-r--r--   0 voidful    (501) staff       (20)       17 2023-04-26 09:05:00.000000 textrl-0.2.17/textrl.egg-info/requires.txt
--rw-r--r--   0 voidful    (501) staff       (20)        7 2023-04-26 09:05:00.000000 textrl-0.2.17/textrl.egg-info/top_level.txt
+drwxr-xr-x   0 voidful    (501) staff       (20)        0 2023-04-26 09:35:25.944076 textrl-0.2.18/
+-rw-r--r--   0 voidful    (501) staff       (20)     4206 2022-12-05 09:09:02.000000 textrl-0.2.18/.gitignore
+-rw-r--r--   0 voidful    (501) staff       (20)     1064 2023-02-09 14:54:56.000000 textrl-0.2.18/LICENSE
+-rw-r--r--   0 voidful    (501) staff       (20)    18232 2023-04-26 09:35:25.943819 textrl-0.2.18/PKG-INFO
+-rw-r--r--   0 voidful    (501) staff       (20)    17515 2023-04-25 10:23:10.000000 textrl-0.2.18/README.md
+drwxr-xr-x   0 voidful    (501) staff       (20)        0 2023-04-26 09:35:25.937995 textrl-0.2.18/example/
+-rw-r--r--   0 voidful    (501) staff       (20)     7679 2023-03-27 13:57:09.000000 textrl-0.2.18/example/2022-12-10-textrl-elon-musk.ipynb
+drwxr-xr-x   0 voidful    (501) staff       (20)        0 2023-04-26 09:35:25.938252 textrl-0.2.18/img/
+-rw-r--r--   0 voidful    (501) staff       (20)   373908 2023-04-17 05:47:18.000000 textrl-0.2.18/img/Designer.png
+-rw-r--r--   0 voidful    (501) staff       (20)       61 2022-12-05 09:17:42.000000 textrl-0.2.18/requirement.txt
+-rw-r--r--   0 voidful    (501) staff       (20)       38 2023-04-26 09:35:25.944128 textrl-0.2.18/setup.cfg
+-rw-r--r--   0 voidful    (501) staff       (20)     1095 2023-04-26 09:35:20.000000 textrl-0.2.18/setup.py
+drwxr-xr-x   0 voidful    (501) staff       (20)        0 2023-04-26 09:35:25.942342 textrl-0.2.18/textrl/
+-rw-r--r--   0 voidful    (501) staff       (20)      184 2023-02-13 19:45:54.000000 textrl-0.2.18/textrl/__init__.py
+-rw-r--r--   0 voidful    (501) staff       (20)    13472 2023-04-26 08:50:57.000000 textrl-0.2.18/textrl/actor.py
+-rw-r--r--   0 voidful    (501) staff       (20)     1140 2022-12-05 09:09:02.000000 textrl-0.2.18/textrl/dump.py
+-rw-r--r--   0 voidful    (501) staff       (20)     7065 2023-04-26 09:35:01.000000 textrl-0.2.18/textrl/environment.py
+-rw-r--r--   0 voidful    (501) staff       (20)    23448 2023-02-13 19:43:59.000000 textrl-0.2.18/textrl/evaluator.py
+-rw-r--r--   0 voidful    (501) staff       (20)     7511 2023-02-13 19:43:59.000000 textrl-0.2.18/textrl/trainer.py
+drwxr-xr-x   0 voidful    (501) staff       (20)        0 2023-04-26 09:35:25.943601 textrl-0.2.18/textrl.egg-info/
+-rw-r--r--   0 voidful    (501) staff       (20)    18232 2023-04-26 09:35:25.000000 textrl-0.2.18/textrl.egg-info/PKG-INFO
+-rw-r--r--   0 voidful    (501) staff       (20)      433 2023-04-26 09:35:25.000000 textrl-0.2.18/textrl.egg-info/SOURCES.txt
+-rw-r--r--   0 voidful    (501) staff       (20)        1 2023-04-26 09:35:25.000000 textrl-0.2.18/textrl.egg-info/dependency_links.txt
+-rw-r--r--   0 voidful    (501) staff       (20)       50 2023-04-26 09:35:25.000000 textrl-0.2.18/textrl.egg-info/entry_points.txt
+-rw-r--r--   0 voidful    (501) staff       (20)        1 2022-12-05 09:10:02.000000 textrl-0.2.18/textrl.egg-info/not-zip-safe
+-rw-r--r--   0 voidful    (501) staff       (20)       17 2023-04-26 09:35:25.000000 textrl-0.2.18/textrl.egg-info/requires.txt
+-rw-r--r--   0 voidful    (501) staff       (20)        7 2023-04-26 09:35:25.000000 textrl-0.2.18/textrl.egg-info/top_level.txt
```

### Comparing `textrl-0.2.17/.gitignore` & `textrl-0.2.18/.gitignore`

 * *Files identical despite different names*

### Comparing `textrl-0.2.17/LICENSE` & `textrl-0.2.18/LICENSE`

 * *Files identical despite different names*

### Comparing `textrl-0.2.17/PKG-INFO` & `textrl-0.2.18/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textrl
-Version: 0.2.17
+Version: 0.2.18
 Summary: TextRL - use reinforcement learning to adjust text generation results.
 Home-page: https://github.com/voidful/TextRL
 Author: Voidful
 Author-email: voidful.stack@gmail.com
 License: Apache
 Keywords: transformer huggingface nlp generation reinforcement learning deep learning
 Platform: UNKNOWN
```

### Comparing `textrl-0.2.17/README.md` & `textrl-0.2.18/README.md`

 * *Files identical despite different names*

### Comparing `textrl-0.2.17/example/2022-12-10-textrl-elon-musk.ipynb` & `textrl-0.2.18/example/2022-12-10-textrl-elon-musk.ipynb`

 * *Files identical despite different names*

### Comparing `textrl-0.2.17/img/Designer.png` & `textrl-0.2.18/img/Designer.png`

 * *Files identical despite different names*

### Comparing `textrl-0.2.17/setup.py` & `textrl-0.2.18/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='textrl',
-    version='0.2.17',
+    version='0.2.18',
     description='TextRL - use reinforcement learning to adjust text generation results.',
     url='https://github.com/voidful/TextRL',
     author='Voidful',
     author_email='voidful.stack@gmail.com',
     long_description=open("README.md", encoding="utf8").read(),
     long_description_content_type="text/markdown",
     setup_requires=['setuptools-git'],
```

### Comparing `textrl-0.2.17/textrl/actor.py` & `textrl-0.2.18/textrl/actor.py`

 * *Files identical despite different names*

### Comparing `textrl-0.2.17/textrl/dump.py` & `textrl-0.2.18/textrl/dump.py`

 * *Files identical despite different names*

### Comparing `textrl-0.2.17/textrl/environment.py` & `textrl-0.2.18/textrl/environment.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 
     @autocast('cuda')
     def _get_obs(self, predicted=[]):
         with torch.inference_mode():
             obs_list = []
             for p_text in predicted:
                 p_text_str = self.tokenizer.convert_tokens_to_string(p_text)
-                if model.__class__.__name__ == 'OPTForCausalLM':
+                if self.model.__class__.__name__ == 'OPTForCausalLM':
                     feature_dict = self.tokenizer([[self.gat_obs_input(self.input_item), p_text_str]],
                                                   return_tensors='pt',
                                                   add_special_tokens=False).to(self.model.device)
                     with torch.cuda.amp.autocast(enabled=False):
                         prediction = self.model(**feature_dict, output_hidden_states=True)
                     outputs = prediction.hidden_states[-self.unfreeze_layer_from_past][:, -1, :]
                 else:
```

### Comparing `textrl-0.2.17/textrl/evaluator.py` & `textrl-0.2.18/textrl/evaluator.py`

 * *Files identical despite different names*

### Comparing `textrl-0.2.17/textrl/trainer.py` & `textrl-0.2.18/textrl/trainer.py`

 * *Files identical despite different names*

### Comparing `textrl-0.2.17/textrl.egg-info/PKG-INFO` & `textrl-0.2.18/textrl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textrl
-Version: 0.2.17
+Version: 0.2.18
 Summary: TextRL - use reinforcement learning to adjust text generation results.
 Home-page: https://github.com/voidful/TextRL
 Author: Voidful
 Author-email: voidful.stack@gmail.com
 License: Apache
 Keywords: transformer huggingface nlp generation reinforcement learning deep learning
 Platform: UNKNOWN
```

