# Comparing `tmp/topcast-0.1.5.tar.gz` & `tmp/topcast-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "topcast-0.1.5.tar", last modified: Tue Apr 25 22:42:27 2023, max compression
+gzip compressed data, was "topcast-0.1.6.tar", last modified: Wed Apr 26 19:10:19 2023, max compression
```

## Comparing `topcast-0.1.5.tar` & `topcast-0.1.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:42:27.515304 topcast-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-25 22:42:10.000000 topcast-0.1.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-04-25 22:42:27.515304 topcast-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-04-25 22:42:10.000000 topcast-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 22:42:27.515304 topcast-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-25 22:42:10.000000 topcast-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:42:27.511304 topcast-0.1.5/topcast/
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-25 22:42:10.000000 topcast-0.1.5/topcast/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:42:27.515304 topcast-0.1.5/topcast/chatgpt_themes/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-25 22:42:10.000000 topcast-0.1.5/topcast/chatgpt_themes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-25 22:42:10.000000 topcast-0.1.5/topcast/chatgpt_themes/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-04-25 22:42:10.000000 topcast-0.1.5/topcast/chatgpt_themes/conclusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-04-25 22:42:10.000000 topcast-0.1.5/topcast/chatgpt_themes/interview.py
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-04-25 22:42:10.000000 topcast-0.1.5/topcast/chatgpt_themes/introduction.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-25 22:42:10.000000 topcast-0.1.5/topcast/chatgpt_themes/none_theme.py
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-04-25 22:42:10.000000 topcast-0.1.5/topcast/chatgpt_themes/summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-04-25 22:42:10.000000 topcast-0.1.5/topcast/cutter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-04-25 22:42:10.000000 topcast-0.1.5/topcast/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-04-25 22:42:10.000000 topcast-0.1.5/topcast/topcaster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:42:27.515304 topcast-0.1.5/topcast/tts_providers/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-25 22:42:10.000000 topcast-0.1.5/topcast/tts_providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-25 22:42:10.000000 topcast-0.1.5/topcast/tts_providers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-25 22:42:10.000000 topcast-0.1.5/topcast/tts_providers/elevenlabs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-04-25 22:42:10.000000 topcast-0.1.5/topcast/tts_providers/gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-25 22:42:10.000000 topcast-0.1.5/topcast/tts_providers/gt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:42:27.511304 topcast-0.1.5/topcast.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-04-25 22:42:27.000000 topcast-0.1.5/topcast.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-25 22:42:27.000000 topcast-0.1.5/topcast.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 22:42:27.000000 topcast-0.1.5/topcast.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-25 22:42:27.000000 topcast-0.1.5/topcast.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-25 22:42:27.000000 topcast-0.1.5/topcast.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:10:19.362921 topcast-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-26 19:10:03.000000 topcast-0.1.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6939 2023-04-26 19:10:19.362921 topcast-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6199 2023-04-26 19:10:03.000000 topcast-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 19:10:19.362921 topcast-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-26 19:10:03.000000 topcast-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:10:19.358921 topcast-0.1.6/topcast/
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-26 19:10:03.000000 topcast-0.1.6/topcast/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:10:19.362921 topcast-0.1.6/topcast/chatgpt_themes/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-26 19:10:03.000000 topcast-0.1.6/topcast/chatgpt_themes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-26 19:10:03.000000 topcast-0.1.6/topcast/chatgpt_themes/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-04-26 19:10:03.000000 topcast-0.1.6/topcast/chatgpt_themes/conclusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-04-26 19:10:03.000000 topcast-0.1.6/topcast/chatgpt_themes/interview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-04-26 19:10:03.000000 topcast-0.1.6/topcast/chatgpt_themes/introduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-26 19:10:03.000000 topcast-0.1.6/topcast/chatgpt_themes/none_theme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-04-26 19:10:03.000000 topcast-0.1.6/topcast/chatgpt_themes/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-04-26 19:10:03.000000 topcast-0.1.6/topcast/cutter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-04-26 19:10:03.000000 topcast-0.1.6/topcast/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-04-26 19:10:03.000000 topcast-0.1.6/topcast/topcaster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:10:19.362921 topcast-0.1.6/topcast/tts_providers/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-26 19:10:03.000000 topcast-0.1.6/topcast/tts_providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-26 19:10:03.000000 topcast-0.1.6/topcast/tts_providers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-26 19:10:03.000000 topcast-0.1.6/topcast/tts_providers/elevenlabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-04-26 19:10:03.000000 topcast-0.1.6/topcast/tts_providers/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-26 19:10:03.000000 topcast-0.1.6/topcast/tts_providers/gt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:10:19.362921 topcast-0.1.6/topcast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6939 2023-04-26 19:10:19.000000 topcast-0.1.6/topcast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-26 19:10:19.000000 topcast-0.1.6/topcast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 19:10:19.000000 topcast-0.1.6/topcast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-26 19:10:19.000000 topcast-0.1.6/topcast.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-26 19:10:19.000000 topcast-0.1.6/topcast.egg-info/top_level.txt
```

### Comparing `topcast-0.1.5/LICENSE.txt` & `topcast-0.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `topcast-0.1.5/PKG-INFO` & `topcast-0.1.6/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,97 +1,38 @@
-Metadata-Version: 2.1
-Name: topcast
-Version: 0.1.5
-Summary: A Python package for Topcast
-Home-page: https://github.com/gormlabenz/topcast
-Author: Gorm Labenz
-Author-email: gorm@labenz.io
-License: MIT
-Keywords: topcast tts text-to-speech gcp google openai elevenlabs
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-# Topcast: Turn Text into Podcasts with TTS and Language Models
+# Topcast: Turn Text into Podcasts with TTS and ChatGPT
 
 Topcast is a Python package that allows you to transform text into a podcast using Text-to-Speech (TTS) and language models. With Topcast, you can provide a text, and the package will create a podcast with an introduction, interview, conclusion, sound effects, and more. Topcast supports various TTS providers and language models.
 
 ## Example Implementation
 
 ```python
-import os
-from topcast import (
-    set_elevenlab_api_key,
-    set_google_credentials,
-    set_openai_api_key,
-    Topcaster,
-)
-
-from topcast.tts_providers import GCP
-from topcast.chatgpt_themes import Summary
+from topcast import Topcaster, set_openai_api_key
+from topcast.chatgpt_themes import Introduction
 
-from dotenv import load_dotenv
-
-load_dotenv()
-
-set_elevenlab_api_key(os.environ["ELEVENLAB_API_KEY"])
-set_openai_api_key(os.environ["OPENAI_API_KEY"])
-set_google_credentials("gcp-keyfile.json")
+set_openai_api_key("XXX-XXX-XXX-XXX-XXX")
 
 topcast = Topcaster()
 
-topcast.add_chapter(
-    audio_layers=[
-        {
-            "audio": "sounds/jingle.wav",
-            "sets_length": True,
-        }
-    ]
-)
-topcast.add_chapter(
-    audio_layers=[
-        {
-            "audio": {
-                "content": "It features the westernmost point in continental Europe, and its Iberian portion is bordered to the west and south by the Atlantic Ocean and to the north and east by Spain.",
-            },
-            "sets_length": True,
-            "fade_in": 1200,
-            "fade_out": 1200,
-        },
-        {"audio": "sounds/background.mp3", "sets_length": False, "volume": 0.5},
-    ],
-    crossfade=2400,
-)
+topcast.add_chapter(audio_layers=[{ "audio" : "sounds/jingle.wav" }])
 topcast.add_chapter(
     audio_layers=[
         {
             "audio": {
-                "content": "It features the westernmost point in continental Europe, and its Iberian portion is bordered to the west and south by the Atlantic Ocean and to the north and east by Spain.",
-                "tts_provider": GCP, 
-                "theme": Summary,
+                "content": "Topcast is a Python package that allows you to transform text into a podcast using Text-to-Speech (TTS) and language models. With Topcast, you can provide a text, and the package will create a podcast with an introduction, interview, conclusion, sound effects, and more. Topcast supports various TTS providers and language models.",
+                "theme": Introduction,
             },
-            "sets_length": True,
-            "fade_in": 1200,
-            "fade_out": 1200,
         },
     ],
     crossfade=2400,
 )
 
 topcast.generate()
 topcast.export("podcast.wav", format="wav")
 
+
 ```
 
 ## Installation
 Install the package using pip:
 
 ```bash
 pip install topcast
@@ -108,116 +49,158 @@
     set_openai_api_key,
     Topcaster,
 )
 
 from topcast.tts_providers import GCP
 from topcast.chatgpt_themes import Summary
 
-from dotenv import load_dotenv
-
-load_dotenv()
-
-set_elevenlab_api_key(os.environ["ELEVENLAB_API_KEY"])
-set_openai_api_key(os.environ["OPENAI_API_KEY"])
-set_google_credentials("gcp-keyfile.json")
+set_elevenlab_api_key("XXX-XXX-XXX") # if you want to use elvenlabs for tts
+set_google_credentials("gcp-keyfile.json") # if you want google cloud platform for tts
+set_openai_api_key("XXX-XXX-XXX") # if you want to use a ChatGPT theme
 ```
 
 2. Create a Topcaster object and add chapters with the desired podcast structure:
 
 ```python
 topcast = Topcaster()
 
 topcast.add_chapter(
     audio_layers=[
         {
-            "audio": "sounds/jingle.wav",
+            "audio": "sounds/jingle.wav", # use a audio file
             "sets_length": True,
         }
     ]
 )
 topcast.add_chapter(
     audio_layers=[
         {
             "audio": {
-                "content": "Portugal...",
-                "tts_provider": GCP,
-                "theme": Summary,
+                "content": "Portugal...", 
+                "tts_provider": GCP, # use google cloud platform for tts
+                "theme": Summary, # generate a summary of the text using ChatGPT
             },
-            "sets_length": True,
-            "fade_in": 1200,
-            "fade_out": 1200,
+            "sets_length": True, # this audio_layer sets the length of the chapter, only one audio_layer can set the length per chapter
+            "fade_in": 1200, # fade in 1200 ms
+            "fade_out": 1200, # fade out 1200 ms
         },
-        {"audio": "sounds/background.mp3", "sets_length": False, "volume": 0.5},
+        {"audio": "sounds/background.mp3", "sets_length": False, "volume": 0.5}, # overlay audio
     ],
-    crossfade=2400,
+    crossfade=2400, # crossfade last chapter
 )
 
 ```
 
 3. Generate and export the podcast:
 
 ```python
 topcast.generate()
-topcast.export("podcast_output.wav", format="wav")
+topcast.export("podcast.wav", format="wav")
 ```
 This will create a podcast using the given chapters and save it as a WAV file named podcast_output.wav.
-##Customization
-You can customize your podcast by adding more chapters to the Topcaster object. Each chapter represents a segment of the podcast. You can add more segments with different themes, TTS providers, and audio layers.
+## ChatGPT Themes
+ChatGPT Themes allow you to transform your text into various structures by leveraging ChatGPT, a large language model. With the available themes, you can transform your text into an interview, introduction, summary, or conclusion. You can also choose to leave the text as it is by using the NoneTheme, which is the default theme.
 
-For example, if you want to add an interview segment, you can include it like this:
+The available ChatGPT Themes are:
 
+- Interview
+- Introduction
+- Summary
+- Conclusion
+- NoneTheme (default)
+### Usage
+To use a specific ChatGPT theme, first import the desired theme:
 ```python
-from topcast import Topcaster
-from topcast.chatgpt_themes import Interview
+from topcast.chatgpt_themes import Interview, Introduction, Summary, Conclusion
+```
+Then, set your OpenAI API key using the set_openai_api_key function:
+```python
+from topcast import set_openai_api_key
 
-topcast = Topcast()
+set_openai_api_key("your-openai-api-key")
 
-topcast.add_chapter(
-    audio_layers=[
-        {
-            "audio": {
-                "content": "It features the westernmost point in continental Europe, and its Iberian portion is bordered to the west and south by the Atlantic Ocean and to the north and east by Spain...", # <- gets automatically converted into an interview script
-                "tts_provider": GCP,
-                "theme": Interview,
-            },
-            "sets_length": True,
-            "fade_in": 1200,
-            "fade_out": 1200,
-        },
-    ],
-    crossfade=2400,
-)
+```
+Finally, set the `theme` property in the audio layer of the desired chapter:
+
+```python
+{
+    "audio": {
+        "content": "Text content...",
+        "theme": Introduction,  # Replace with the desired theme
+    },
+}
+
+```
+To keep the original text without any transformation, set NoneTheme or don't set `theme` at all
 
 
+```python
+from topcast.chatgpt_themes import NoneTheme
+
+{
+    "audio": {
+        "content": "Text content...",
+        "theme": NoneTheme,  # Keeps the text as it is
+    },
+}
 ```
+## TTS Providers
+Topcast allows you to use various Text-to-Speech (TTS) providers to convert your text into speech. The currently implemented TTS providers are:
+- GCP (Google Cloud Platform) - Requires a Google Cloud Platform account
+- Elevenlabs - Requires an Elevenlabs account
+- GTTS (Google Translate) - No account required (default)
+### Comparison
+- **Elevenlabs**: Offers the best voices but is expensive and has API limits.
+- **GCP (Google Cloud Platform)**: Relatively cheap but requires a Google Cloud Platform account with the Text-to-Speech API enabled.
+- **GTTS (Google Translate)**: Free and does not require an account, but the voice quality is not as good as the other options.
+### Usage
+First, import the desired TTS provider:
+```python
+from topcast.tts_providers import GCP, Elevenlabs, GTTS
 
-You can also add sound effects or background music by adding additional audio layers within a chapter:
+```
+Next, set the API key or credentials for the provider, if required:
+```python
+from topcast import set_elevenlab_api_key, set_google_credentials
 
+set_elevenlab_api_key("your-elevenlabs-api-key")
+set_google_credentials("path-to-gcp-keyfile.json")
+```
+Finally, specify the tts_provider property in the audio layer of the desired chapter:
 ```python
-from topcast import Topcaster
+{
+    "audio": {
+        "content": "Text content...",
+        "tts_provider": GCP,  # Replace with the desired TTS provider
+    },
+}
 
-topcast = Topcast()
+```
 
+For example, to create a chapter using the GCP TTS provider:
+```python
 topcast.add_chapter(
     audio_layers=[
         {
-            "audio": 'sounds/background_music.wav',
-            "sets_length": False,
-            "volume": 0.3,
-        },
-        {
             "audio": {
                 "content": "Text content...",
                 "tts_provider": GCP,
                 "theme": Summary,
             },
             "sets_length": True,
             "fade_in": 1200,
             "fade_out": 1200,
-        }
+        },
     ],
     crossfade=2400,
 )
+
 ```
-This will add background music with a volume of 0.3 to the chapter.
+To use the default GTTS provider, you can simply omit the tts_provider property:
 
-Remember to adjust the crossfade value for smoother transitions between chapters.
+```python
+{
+    "audio": {
+        "content": "Text content...",
+    },
+}
+```
```

### Comparing `topcast-0.1.5/setup.py` & `topcast-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="topcast",
-    version="0.1.5",
+    version="0.1.6",
     author="Gorm Labenz",
     author_email="gorm@labenz.io",
     description="A Python package for Topcast",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/gormlabenz/topcast",
     packages=find_packages(),
```

### Comparing `topcast-0.1.5/topcast/chatgpt_themes/base.py` & `topcast-0.1.6/topcast/chatgpt_themes/base.py`

 * *Files identical despite different names*

### Comparing `topcast-0.1.5/topcast/chatgpt_themes/conclusion.py` & `topcast-0.1.6/topcast/chatgpt_themes/conclusion.py`

 * *Files identical despite different names*

### Comparing `topcast-0.1.5/topcast/chatgpt_themes/interview.py` & `topcast-0.1.6/topcast/chatgpt_themes/interview.py`

 * *Files identical despite different names*

### Comparing `topcast-0.1.5/topcast/chatgpt_themes/introduction.py` & `topcast-0.1.6/topcast/chatgpt_themes/introduction.py`

 * *Files identical despite different names*

### Comparing `topcast-0.1.5/topcast/chatgpt_themes/summary.py` & `topcast-0.1.6/topcast/chatgpt_themes/summary.py`

 * *Files identical despite different names*

### Comparing `topcast-0.1.5/topcast/cutter.py` & `topcast-0.1.6/topcast/cutter.py`

 * *Files identical despite different names*

### Comparing `topcast-0.1.5/topcast/models.py` & `topcast-0.1.6/topcast/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,17 +13,17 @@
     audio_list: List[AudioSegment] = []
 
     class Config:
         arbitrary_types_allowed = True
         
 class AudioItem(BaseModel):
     from topcast.tts_providers.base import TTSProviderBase
-    from topcast.tts_providers.gt import GTTS # <-- make default provider
+    from topcast.tts_providers.gt import GTTS 
     from topcast.chatgpt_themes.base import ChatGPTThemeBase
-    from topcast.chatgpt_themes.none_theme import NoneTheme# <-- make default theme
+    from topcast.chatgpt_themes.none_theme import NoneTheme
     
     content: str
     theme: Optional[Type[ChatGPTThemeBase]] = Field(default=NoneTheme)
     tts_provider: Optional[Type[TTSProviderBase]] = Field(default=GTTS)
 
     @validator("theme")
     def check_theme_base_class(cls, value):
```

### Comparing `topcast-0.1.5/topcast/topcaster.py` & `topcast-0.1.6/topcast/topcaster.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,29 +4,50 @@
 from .models import Timeline, AudioItem, ChapterData, Chapter
 from .cutter import Cutter
 
 class Topcaster:
     def __init__(self, timeline: Timeline = []):
         self.timeline = Timeline(timeline=timeline)
         self.topcast = AudioSegment.empty()
+        self.already_generated = False
         
     def add_chapter(self, audio_layers = [], fade_in: int = 1, fade_out: int = 1 , padding_start: int = 0 , padding_end: int = 0 , crossfade: int = 0, volume: float = 1):
+        self.already_generated = False
         
         chapter = Chapter(audio_layers=audio_layers, fade_in=fade_in, fade_out=fade_out, padding_start=padding_start, padding_end=padding_end, crossfade=crossfade, volume=volume)
         self.timeline.timeline.append(chapter)
         
-    def generate(self):
+    def generate(self):        
+        self.set_length_setter()
         self.add_chapter_data_dict()
         self.open_audio_files()
         asyncio.run(self.generate_text())
         asyncio.run(self.generate_speech())
         self.cut()
         
+        self.already_generated = True
         return self.topcast
 
+    def set_length_setter(self):
+        for chapter in self.timeline.timeline:
+            have_set_length = False
+            
+            if(len(chapter.audio_layers) == 1):
+                chapter.audio_layers[0].sets_length = True
+                print("Only one audio layer in chapter, setting length setter")
+                continue
+            
+            for audio_layer in chapter.audio_layers:
+                if audio_layer.sets_length:
+                    if have_set_length:
+                        raise Exception("Only one audio layer can set the length of a chapter")
+                    else:
+                        print("Setting length setter")
+                        have_set_length = True
+                
     def add_chapter_data_dict(self):
         for chapter in self.timeline.timeline:
             for audio_layer in chapter.audio_layers:
                 audio_layer.data = ChapterData(raw_audio= None, text_list=[], audio_list= [])
                 
     def open_audio_files(self):
         for chapter in self.timeline.timeline:
@@ -76,8 +97,10 @@
             )
             
             
         results = await asyncio.gather(*tasks)        
         audio_layer.data.audio_list = results
         
     def export(self, file_name = "topcast.mp3", format="mp3"):
+        if not self.already_generated:
+            raise Exception("You need to generate the podcast before you can export it")
         self.topcast.export(file_name, format = format)
```

### Comparing `topcast-0.1.5/topcast/tts_providers/elevenlabs.py` & `topcast-0.1.6/topcast/tts_providers/elevenlabs.py`

 * *Files identical despite different names*

### Comparing `topcast-0.1.5/topcast/tts_providers/gcp.py` & `topcast-0.1.6/topcast/tts_providers/gcp.py`

 * *Files identical despite different names*

### Comparing `topcast-0.1.5/topcast/tts_providers/gt.py` & `topcast-0.1.6/topcast/tts_providers/gt.py`

 * *Files identical despite different names*

### Comparing `topcast-0.1.5/topcast.egg-info/PKG-INFO` & `topcast-0.1.6/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: topcast
-Version: 0.1.5
+Version: 0.1.6
 Summary: A Python package for Topcast
 Home-page: https://github.com/gormlabenz/topcast
 Author: Gorm Labenz
 Author-email: gorm@labenz.io
 License: MIT
 Keywords: topcast tts text-to-speech gcp google openai elevenlabs
 Classifier: Development Status :: 3 - Alpha
@@ -15,83 +15,45 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# Topcast: Turn Text into Podcasts with TTS and Language Models
+# Topcast: Turn Text into Podcasts with TTS and ChatGPT
 
 Topcast is a Python package that allows you to transform text into a podcast using Text-to-Speech (TTS) and language models. With Topcast, you can provide a text, and the package will create a podcast with an introduction, interview, conclusion, sound effects, and more. Topcast supports various TTS providers and language models.
 
 ## Example Implementation
 
 ```python
-import os
-from topcast import (
-    set_elevenlab_api_key,
-    set_google_credentials,
-    set_openai_api_key,
-    Topcaster,
-)
-
-from topcast.tts_providers import GCP
-from topcast.chatgpt_themes import Summary
-
-from dotenv import load_dotenv
+from topcast import Topcaster, set_openai_api_key
+from topcast.chatgpt_themes import Introduction
 
-load_dotenv()
-
-set_elevenlab_api_key(os.environ["ELEVENLAB_API_KEY"])
-set_openai_api_key(os.environ["OPENAI_API_KEY"])
-set_google_credentials("gcp-keyfile.json")
+set_openai_api_key("XXX-XXX-XXX-XXX-XXX")
 
 topcast = Topcaster()
 
-topcast.add_chapter(
-    audio_layers=[
-        {
-            "audio": "sounds/jingle.wav",
-            "sets_length": True,
-        }
-    ]
-)
-topcast.add_chapter(
-    audio_layers=[
-        {
-            "audio": {
-                "content": "It features the westernmost point in continental Europe, and its Iberian portion is bordered to the west and south by the Atlantic Ocean and to the north and east by Spain.",
-            },
-            "sets_length": True,
-            "fade_in": 1200,
-            "fade_out": 1200,
-        },
-        {"audio": "sounds/background.mp3", "sets_length": False, "volume": 0.5},
-    ],
-    crossfade=2400,
-)
+topcast.add_chapter(audio_layers=[{ "audio" : "sounds/jingle.wav" }])
 topcast.add_chapter(
     audio_layers=[
         {
             "audio": {
-                "content": "It features the westernmost point in continental Europe, and its Iberian portion is bordered to the west and south by the Atlantic Ocean and to the north and east by Spain.",
-                "tts_provider": GCP, 
-                "theme": Summary,
+                "content": "Topcast is a Python package that allows you to transform text into a podcast using Text-to-Speech (TTS) and language models. With Topcast, you can provide a text, and the package will create a podcast with an introduction, interview, conclusion, sound effects, and more. Topcast supports various TTS providers and language models.",
+                "theme": Introduction,
             },
-            "sets_length": True,
-            "fade_in": 1200,
-            "fade_out": 1200,
         },
     ],
     crossfade=2400,
 )
 
 topcast.generate()
 topcast.export("podcast.wav", format="wav")
 
+
 ```
 
 ## Installation
 Install the package using pip:
 
 ```bash
 pip install topcast
@@ -108,116 +70,158 @@
     set_openai_api_key,
     Topcaster,
 )
 
 from topcast.tts_providers import GCP
 from topcast.chatgpt_themes import Summary
 
-from dotenv import load_dotenv
-
-load_dotenv()
-
-set_elevenlab_api_key(os.environ["ELEVENLAB_API_KEY"])
-set_openai_api_key(os.environ["OPENAI_API_KEY"])
-set_google_credentials("gcp-keyfile.json")
+set_elevenlab_api_key("XXX-XXX-XXX") # if you want to use elvenlabs for tts
+set_google_credentials("gcp-keyfile.json") # if you want google cloud platform for tts
+set_openai_api_key("XXX-XXX-XXX") # if you want to use a ChatGPT theme
 ```
 
 2. Create a Topcaster object and add chapters with the desired podcast structure:
 
 ```python
 topcast = Topcaster()
 
 topcast.add_chapter(
     audio_layers=[
         {
-            "audio": "sounds/jingle.wav",
+            "audio": "sounds/jingle.wav", # use a audio file
             "sets_length": True,
         }
     ]
 )
 topcast.add_chapter(
     audio_layers=[
         {
             "audio": {
-                "content": "Portugal...",
-                "tts_provider": GCP,
-                "theme": Summary,
+                "content": "Portugal...", 
+                "tts_provider": GCP, # use google cloud platform for tts
+                "theme": Summary, # generate a summary of the text using ChatGPT
             },
-            "sets_length": True,
-            "fade_in": 1200,
-            "fade_out": 1200,
+            "sets_length": True, # this audio_layer sets the length of the chapter, only one audio_layer can set the length per chapter
+            "fade_in": 1200, # fade in 1200 ms
+            "fade_out": 1200, # fade out 1200 ms
         },
-        {"audio": "sounds/background.mp3", "sets_length": False, "volume": 0.5},
+        {"audio": "sounds/background.mp3", "sets_length": False, "volume": 0.5}, # overlay audio
     ],
-    crossfade=2400,
+    crossfade=2400, # crossfade last chapter
 )
 
 ```
 
 3. Generate and export the podcast:
 
 ```python
 topcast.generate()
-topcast.export("podcast_output.wav", format="wav")
+topcast.export("podcast.wav", format="wav")
 ```
 This will create a podcast using the given chapters and save it as a WAV file named podcast_output.wav.
-##Customization
-You can customize your podcast by adding more chapters to the Topcaster object. Each chapter represents a segment of the podcast. You can add more segments with different themes, TTS providers, and audio layers.
+## ChatGPT Themes
+ChatGPT Themes allow you to transform your text into various structures by leveraging ChatGPT, a large language model. With the available themes, you can transform your text into an interview, introduction, summary, or conclusion. You can also choose to leave the text as it is by using the NoneTheme, which is the default theme.
 
-For example, if you want to add an interview segment, you can include it like this:
+The available ChatGPT Themes are:
 
+- Interview
+- Introduction
+- Summary
+- Conclusion
+- NoneTheme (default)
+### Usage
+To use a specific ChatGPT theme, first import the desired theme:
+```python
+from topcast.chatgpt_themes import Interview, Introduction, Summary, Conclusion
+```
+Then, set your OpenAI API key using the set_openai_api_key function:
 ```python
-from topcast import Topcaster
-from topcast.chatgpt_themes import Interview
+from topcast import set_openai_api_key
 
-topcast = Topcast()
+set_openai_api_key("your-openai-api-key")
 
-topcast.add_chapter(
-    audio_layers=[
-        {
-            "audio": {
-                "content": "It features the westernmost point in continental Europe, and its Iberian portion is bordered to the west and south by the Atlantic Ocean and to the north and east by Spain...", # <- gets automatically converted into an interview script
-                "tts_provider": GCP,
-                "theme": Interview,
-            },
-            "sets_length": True,
-            "fade_in": 1200,
-            "fade_out": 1200,
-        },
-    ],
-    crossfade=2400,
-)
+```
+Finally, set the `theme` property in the audio layer of the desired chapter:
 
+```python
+{
+    "audio": {
+        "content": "Text content...",
+        "theme": Introduction,  # Replace with the desired theme
+    },
+}
 
 ```
+To keep the original text without any transformation, set NoneTheme or don't set `theme` at all
+
 
-You can also add sound effects or background music by adding additional audio layers within a chapter:
+```python
+from topcast.chatgpt_themes import NoneTheme
+
+{
+    "audio": {
+        "content": "Text content...",
+        "theme": NoneTheme,  # Keeps the text as it is
+    },
+}
+```
+## TTS Providers
+Topcast allows you to use various Text-to-Speech (TTS) providers to convert your text into speech. The currently implemented TTS providers are:
+- GCP (Google Cloud Platform) - Requires a Google Cloud Platform account
+- Elevenlabs - Requires an Elevenlabs account
+- GTTS (Google Translate) - No account required (default)
+### Comparison
+- **Elevenlabs**: Offers the best voices but is expensive and has API limits.
+- **GCP (Google Cloud Platform)**: Relatively cheap but requires a Google Cloud Platform account with the Text-to-Speech API enabled.
+- **GTTS (Google Translate)**: Free and does not require an account, but the voice quality is not as good as the other options.
+### Usage
+First, import the desired TTS provider:
+```python
+from topcast.tts_providers import GCP, Elevenlabs, GTTS
 
+```
+Next, set the API key or credentials for the provider, if required:
 ```python
-from topcast import Topcaster
+from topcast import set_elevenlab_api_key, set_google_credentials
 
-topcast = Topcast()
+set_elevenlab_api_key("your-elevenlabs-api-key")
+set_google_credentials("path-to-gcp-keyfile.json")
+```
+Finally, specify the tts_provider property in the audio layer of the desired chapter:
+```python
+{
+    "audio": {
+        "content": "Text content...",
+        "tts_provider": GCP,  # Replace with the desired TTS provider
+    },
+}
 
+```
+
+For example, to create a chapter using the GCP TTS provider:
+```python
 topcast.add_chapter(
     audio_layers=[
         {
-            "audio": 'sounds/background_music.wav',
-            "sets_length": False,
-            "volume": 0.3,
-        },
-        {
             "audio": {
                 "content": "Text content...",
                 "tts_provider": GCP,
                 "theme": Summary,
             },
             "sets_length": True,
             "fade_in": 1200,
             "fade_out": 1200,
-        }
+        },
     ],
     crossfade=2400,
 )
+
 ```
-This will add background music with a volume of 0.3 to the chapter.
+To use the default GTTS provider, you can simply omit the tts_provider property:
 
-Remember to adjust the crossfade value for smoother transitions between chapters.
+```python
+{
+    "audio": {
+        "content": "Text content...",
+    },
+}
+```
```

### Comparing `topcast-0.1.5/topcast.egg-info/SOURCES.txt` & `topcast-0.1.6/topcast.egg-info/SOURCES.txt`

 * *Files identical despite different names*

