# Comparing `tmp/topcast-0.1.4.tar.gz` & `tmp/topcast-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "topcast-0.1.4.tar", last modified: Mon Apr 24 20:15:27 2023, max compression
+gzip compressed data, was "topcast-0.1.5.tar", last modified: Tue Apr 25 22:42:27 2023, max compression
```

## Comparing `topcast-0.1.4.tar` & `topcast-0.1.5.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 gormlabenz   (501) staff       (20)        0 2023-04-24 20:15:27.140623 topcast-0.1.4/
--rw-r--r--   0 gormlabenz   (501) staff       (20)     1055 2023-04-23 19:15:51.000000 topcast-0.1.4/LICENSE.txt
--rw-r--r--   0 gormlabenz   (501) staff       (20)     5443 2023-04-24 20:15:27.140496 topcast-0.1.4/PKG-INFO
--rw-r--r--   0 gormlabenz   (501) staff       (20)     4683 2023-04-24 07:47:53.000000 topcast-0.1.4/README.md
--rw-r--r--   0 gormlabenz   (501) staff       (20)       38 2023-04-24 20:15:27.140674 topcast-0.1.4/setup.cfg
--rw-r--r--   0 gormlabenz   (501) staff       (20)     1145 2023-04-24 20:13:11.000000 topcast-0.1.4/setup.py
-drwxr-xr-x   0 gormlabenz   (501) staff       (20)        0 2023-04-24 20:15:27.138277 topcast-0.1.4/topcast/
--rw-r--r--   0 gormlabenz   (501) staff       (20)      497 2023-04-24 07:47:52.000000 topcast-0.1.4/topcast/__init__.py
--rw-r--r--   0 gormlabenz   (501) staff       (20)      598 2023-04-24 19:33:45.000000 topcast-0.1.4/topcast/chatgpt.py
-drwxr-xr-x   0 gormlabenz   (501) staff       (20)        0 2023-04-24 20:15:27.139765 topcast-0.1.4/topcast/chatgpt_themes/
--rw-r--r--   0 gormlabenz   (501) staff       (20)      136 2023-04-24 07:47:52.000000 topcast-0.1.4/topcast/chatgpt_themes/__init__.py
--rw-r--r--   0 gormlabenz   (501) staff       (20)      702 2023-04-24 07:47:52.000000 topcast-0.1.4/topcast/chatgpt_themes/base.py
--rw-r--r--   0 gormlabenz   (501) staff       (20)     3806 2023-04-24 07:47:52.000000 topcast-0.1.4/topcast/chatgpt_themes/conclusion.py
--rw-r--r--   0 gormlabenz   (501) staff       (20)     7482 2023-04-24 07:47:52.000000 topcast-0.1.4/topcast/chatgpt_themes/interview.py
--rw-r--r--   0 gormlabenz   (501) staff       (20)     2232 2023-04-24 07:47:52.000000 topcast-0.1.4/topcast/chatgpt_themes/introduction.py
--rw-r--r--   0 gormlabenz   (501) staff       (20)     3164 2023-04-24 07:47:52.000000 topcast-0.1.4/topcast/chatgpt_themes/summary.py
--rw-r--r--   0 gormlabenz   (501) staff       (20)     2084 2023-04-24 07:47:52.000000 topcast-0.1.4/topcast/cutter.py
--rw-r--r--   0 gormlabenz   (501) staff       (20)     2053 2023-04-24 07:47:52.000000 topcast-0.1.4/topcast/models.py
--rw-r--r--   0 gormlabenz   (501) staff       (20)     2707 2023-04-24 07:47:52.000000 topcast-0.1.4/topcast/podcaster.py
-drwxr-xr-x   0 gormlabenz   (501) staff       (20)        0 2023-04-24 20:15:27.140287 topcast-0.1.4/topcast/tts_providers/
--rw-r--r--   0 gormlabenz   (501) staff       (20)       56 2023-04-24 07:47:52.000000 topcast-0.1.4/topcast/tts_providers/__init__.py
--rw-r--r--   0 gormlabenz   (501) staff       (20)      306 2023-04-24 07:47:52.000000 topcast-0.1.4/topcast/tts_providers/base.py
--rw-r--r--   0 gormlabenz   (501) staff       (20)      706 2023-04-24 07:47:52.000000 topcast-0.1.4/topcast/tts_providers/elevenlabs.py
--rw-r--r--   0 gormlabenz   (501) staff       (20)     1444 2023-04-24 07:47:52.000000 topcast-0.1.4/topcast/tts_providers/gcp.py
-drwxr-xr-x   0 gormlabenz   (501) staff       (20)        0 2023-04-24 20:15:27.138880 topcast-0.1.4/topcast.egg-info/
--rw-r--r--   0 gormlabenz   (501) staff       (20)     5443 2023-04-24 20:15:27.000000 topcast-0.1.4/topcast.egg-info/PKG-INFO
--rw-r--r--   0 gormlabenz   (501) staff       (20)      621 2023-04-24 20:15:27.000000 topcast-0.1.4/topcast.egg-info/SOURCES.txt
--rw-r--r--   0 gormlabenz   (501) staff       (20)        1 2023-04-24 20:15:27.000000 topcast-0.1.4/topcast.egg-info/dependency_links.txt
--rw-r--r--   0 gormlabenz   (501) staff       (20)       68 2023-04-24 20:15:27.000000 topcast-0.1.4/topcast.egg-info/requires.txt
--rw-r--r--   0 gormlabenz   (501) staff       (20)        8 2023-04-24 20:15:27.000000 topcast-0.1.4/topcast.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:42:27.515304 topcast-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-25 22:42:10.000000 topcast-0.1.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-04-25 22:42:27.515304 topcast-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-04-25 22:42:10.000000 topcast-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 22:42:27.515304 topcast-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-25 22:42:10.000000 topcast-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:42:27.511304 topcast-0.1.5/topcast/
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-25 22:42:10.000000 topcast-0.1.5/topcast/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:42:27.515304 topcast-0.1.5/topcast/chatgpt_themes/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-25 22:42:10.000000 topcast-0.1.5/topcast/chatgpt_themes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-25 22:42:10.000000 topcast-0.1.5/topcast/chatgpt_themes/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-04-25 22:42:10.000000 topcast-0.1.5/topcast/chatgpt_themes/conclusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-04-25 22:42:10.000000 topcast-0.1.5/topcast/chatgpt_themes/interview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-04-25 22:42:10.000000 topcast-0.1.5/topcast/chatgpt_themes/introduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-25 22:42:10.000000 topcast-0.1.5/topcast/chatgpt_themes/none_theme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-04-25 22:42:10.000000 topcast-0.1.5/topcast/chatgpt_themes/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-04-25 22:42:10.000000 topcast-0.1.5/topcast/cutter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-04-25 22:42:10.000000 topcast-0.1.5/topcast/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-04-25 22:42:10.000000 topcast-0.1.5/topcast/topcaster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:42:27.515304 topcast-0.1.5/topcast/tts_providers/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-25 22:42:10.000000 topcast-0.1.5/topcast/tts_providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-25 22:42:10.000000 topcast-0.1.5/topcast/tts_providers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-25 22:42:10.000000 topcast-0.1.5/topcast/tts_providers/elevenlabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-04-25 22:42:10.000000 topcast-0.1.5/topcast/tts_providers/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-25 22:42:10.000000 topcast-0.1.5/topcast/tts_providers/gt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:42:27.511304 topcast-0.1.5/topcast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-04-25 22:42:27.000000 topcast-0.1.5/topcast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-25 22:42:27.000000 topcast-0.1.5/topcast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 22:42:27.000000 topcast-0.1.5/topcast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-25 22:42:27.000000 topcast-0.1.5/topcast.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-25 22:42:27.000000 topcast-0.1.5/topcast.egg-info/top_level.txt
```

### Comparing `topcast-0.1.4/LICENSE.txt` & `topcast-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `topcast-0.1.4/PKG-INFO` & `topcast-0.1.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,177 +1,223 @@
 Metadata-Version: 2.1
 Name: topcast
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Python package for Topcast
 Home-page: https://github.com/gormlabenz/topcast
 Author: Gorm Labenz
 Author-email: gorm@labenz.io
 License: MIT
 Keywords: topcast tts text-to-speech gcp google openai elevenlabs
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Topcast: Turn Text into Podcasts with TTS and Language Models
+
 Topcast is a Python package that allows you to transform text into a podcast using Text-to-Speech (TTS) and language models. With Topcast, you can provide a text, and the package will create a podcast with an introduction, interview, conclusion, sound effects, and more. Topcast supports various TTS providers and language models.
 
-##Example Implementation
+## Example Implementation
+
 ```python
-from topcast.chatgpt_themes import Introduction, Interview, Conclusion, Summary
-from topcast.tts_providers import ElevenLabs, GCP
 import os
-from topcast import generate, set_elevenlab_api_key, set_google_credentials, set_openai_api_key
+from topcast import (
+    set_elevenlab_api_key,
+    set_google_credentials,
+    set_openai_api_key,
+    Topcaster,
+)
+
+from topcast.tts_providers import GCP
+from topcast.chatgpt_themes import Summary
 
 from dotenv import load_dotenv
 
 load_dotenv()
 
 set_elevenlab_api_key(os.environ["ELEVENLAB_API_KEY"])
 set_openai_api_key(os.environ["OPENAI_API_KEY"])
-set_google_credentials('gcp-keyfile.json')
+set_google_credentials("gcp-keyfile.json")
 
-timeline = [
-    {
-        "audio_layers": [
-            {
-                "audio": 'sounds/jingle.wav', 
-                "is_main": True, 
-            }
-        ],
-    },
-    {
-    "audio_layers": [
+topcast = Topcaster()
+
+topcast.add_chapter(
+    audio_layers=[
         {
-            "audio": {
-                "content": "Portugal (Portuguese pronunciation: [puɾtuˈɣal]), officially the Portuguese Republic (Portuguese: República Portuguesa [ʁɛˈpuβlikɐ puɾtuˈɣezɐ]),[note 4] is a country located on the Iberian Peninsula, in southwestern Europe, and whose territory also includes the Atlantic archipelagos of the Azores and Madeira. It features the westernmost point in continental Europe, and its Iberian portion is bordered to the west and south by the Atlantic Ocean and to the north and east by Spain, the sole country to have a land border with Portugal. Its two archipelagos form two autonomous regions with their own regional governments. Lisbon is the capital and largest city by population.",
-                "theme": Introduction,
-                "tts_provider": ElevenLabs
-            }, 
-            "is_main": True, 
+            "audio": "sounds/jingle.wav",
+            "sets_length": True,
         }
+    ]
+)
+topcast.add_chapter(
+    audio_layers=[
+        {
+            "audio": {
+                "content": "It features the westernmost point in continental Europe, and its Iberian portion is bordered to the west and south by the Atlantic Ocean and to the north and east by Spain.",
+            },
+            "sets_length": True,
+            "fade_in": 1200,
+            "fade_out": 1200,
+        },
+        {"audio": "sounds/background.mp3", "sets_length": False, "volume": 0.5},
     ],
+    crossfade=2400,
+)
+topcast.add_chapter(
+    audio_layers=[
+        {
+            "audio": {
+                "content": "It features the westernmost point in continental Europe, and its Iberian portion is bordered to the west and south by the Atlantic Ocean and to the north and east by Spain.",
+                "tts_provider": GCP, 
+                "theme": Summary,
+            },
+            "sets_length": True,
+            "fade_in": 1200,
+            "fade_out": 1200,
+        },
+    ],
+    crossfade=2400,
+)
 
-    "crossfade": 2400, 
-},
-]
+topcast.generate()
+topcast.export("podcast.wav", format="wav")
 
-podcast = generate(timeline)
-podcast.export("podcast_3.wav", format="wav")
 ```
-##Installation
+
+## Installation
 Install the package using pip:
 
 ```bash
 pip install topcast
-````
+```
+
+## Usage
 
-##Usage
 1. Import the necessary modules and set the API keys:
+
 ```python
-from topcast.chatgpt_themes import Introduction, Interview, Conclusion, Summary
-from topcast.tts_providers import ElevenLabs, GCP
-import os
-from topcast import generate, set_elevenlab_api_key, set_google_credentials, set_openai_api_key
+from topcast import (
+    set_elevenlab_api_key,
+    set_google_credentials,
+    set_openai_api_key,
+    Topcaster,
+)
+
+from topcast.tts_providers import GCP
+from topcast.chatgpt_themes import Summary
 
 from dotenv import load_dotenv
 
 load_dotenv()
 
 set_elevenlab_api_key(os.environ["ELEVENLAB_API_KEY"])
 set_openai_api_key(os.environ["OPENAI_API_KEY"])
-set_google_credentials('gcp-keyfile.json')
+set_google_credentials("gcp-keyfile.json")
 ```
-2. Create a timeline with the desired podcast structure:
+
+2. Create a Topcaster object and add chapters with the desired podcast structure:
+
 ```python
-timeline = [
-    {
-        "audio_layers": [
-            {
-                "audio": 'sounds/jingle.wav', 
-                "is_main": True, 
-            }
-        ],
-    },
-    {
-    "audio_layers": [
+topcast = Topcaster()
+
+topcast.add_chapter(
+    audio_layers=[
+        {
+            "audio": "sounds/jingle.wav",
+            "sets_length": True,
+        }
+    ]
+)
+topcast.add_chapter(
+    audio_layers=[
         {
             "audio": {
                 "content": "Portugal...",
-                "theme": Introduction,
-                "tts_provider": ElevenLabs
-            }, 
-            "is_main": True, 
-        }
+                "tts_provider": GCP,
+                "theme": Summary,
+            },
+            "sets_length": True,
+            "fade_in": 1200,
+            "fade_out": 1200,
+        },
+        {"audio": "sounds/background.mp3", "sets_length": False, "volume": 0.5},
     ],
+    crossfade=2400,
+)
 
-    "crossfade": 2400, 
-},
-]
 ```
+
 3. Generate and export the podcast:
+
 ```python
-podcast = generate(timeline)
-podcast.export("podcast_output.wav", format="wav")
+topcast.generate()
+topcast.export("podcast_output.wav", format="wav")
 ```
-
-This will create a podcast using the given *timeline* and save it as a WAV file named *podcast_output.wav*.
+This will create a podcast using the given chapters and save it as a WAV file named podcast_output.wav.
 ##Customization
-You can customize your podcast by modifying the *timeline* list. Each element in the list represents a segment of the podcast. You can add more segments with different themes, TTS providers, and audio layers.
+You can customize your podcast by adding more chapters to the Topcaster object. Each chapter represents a segment of the podcast. You can add more segments with different themes, TTS providers, and audio layers.
 
 For example, if you want to add an interview segment, you can include it like this:
+
 ```python
-{
-    "audio_layers": [
+from topcast import Topcaster
+from topcast.chatgpt_themes import Interview
+
+topcast = Topcast()
+
+topcast.add_chapter(
+    audio_layers=[
         {
             "audio": {
-                "content": "Interview text...",
+                "content": "It features the westernmost point in continental Europe, and its Iberian portion is bordered to the west and south by the Atlantic Ocean and to the north and east by Spain...", # <- gets automatically converted into an interview script
+                "tts_provider": GCP,
                 "theme": Interview,
-                "tts_provider": GCP
-            }, 
-            "is_main": True, 
-        }
+            },
+            "sets_length": True,
+            "fade_in": 1200,
+            "fade_out": 1200,
+        },
     ],
-    "crossfade": 2400, 
-}
+    crossfade=2400,
+)
+
 
 ```
 
-You can also add sound effects or background music by adding additional audio layers:
+You can also add sound effects or background music by adding additional audio layers within a chapter:
 
 ```python
-{
-    "audio_layers": [
+from topcast import Topcaster
+
+topcast = Topcast()
+
+topcast.add_chapter(
+    audio_layers=[
         {
             "audio": 'sounds/background_music.wav',
-            "is_main": False,
+            "sets_length": False,
             "volume": 0.3,
         },
         {
             "audio": {
                 "content": "Text content...",
-                "theme": Conclusion,
-                "tts_provider": ElevenLabs
-            }, 
-            "is_main": True, 
+                "tts_provider": GCP,
+                "theme": Summary,
+            },
+            "sets_length": True,
+            "fade_in": 1200,
+            "fade_out": 1200,
         }
     ],
-    "crossfade": 2400, 
-}
+    crossfade=2400,
+)
 ```
-This will add background music with a volume of 0.3 to the conclusion segment.
-
-Remember to adjust the *crossfade* value for smoother transitions between segments.
-
-
-
-
-
+This will add background music with a volume of 0.3 to the chapter.
 
+Remember to adjust the crossfade value for smoother transitions between chapters.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `topcast-0.1.4/README.md` & `topcast-0.1.5/topcast.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,153 +1,223 @@
+Metadata-Version: 2.1
+Name: topcast
+Version: 0.1.5
+Summary: A Python package for Topcast
+Home-page: https://github.com/gormlabenz/topcast
+Author: Gorm Labenz
+Author-email: gorm@labenz.io
+License: MIT
+Keywords: topcast tts text-to-speech gcp google openai elevenlabs
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 # Topcast: Turn Text into Podcasts with TTS and Language Models
+
 Topcast is a Python package that allows you to transform text into a podcast using Text-to-Speech (TTS) and language models. With Topcast, you can provide a text, and the package will create a podcast with an introduction, interview, conclusion, sound effects, and more. Topcast supports various TTS providers and language models.
 
-##Example Implementation
+## Example Implementation
+
 ```python
-from topcast.chatgpt_themes import Introduction, Interview, Conclusion, Summary
-from topcast.tts_providers import ElevenLabs, GCP
 import os
-from topcast import generate, set_elevenlab_api_key, set_google_credentials, set_openai_api_key
+from topcast import (
+    set_elevenlab_api_key,
+    set_google_credentials,
+    set_openai_api_key,
+    Topcaster,
+)
+
+from topcast.tts_providers import GCP
+from topcast.chatgpt_themes import Summary
 
 from dotenv import load_dotenv
 
 load_dotenv()
 
 set_elevenlab_api_key(os.environ["ELEVENLAB_API_KEY"])
 set_openai_api_key(os.environ["OPENAI_API_KEY"])
-set_google_credentials('gcp-keyfile.json')
+set_google_credentials("gcp-keyfile.json")
+
+topcast = Topcaster()
 
-timeline = [
-    {
-        "audio_layers": [
-            {
-                "audio": 'sounds/jingle.wav', 
-                "is_main": True, 
-            }
-        ],
-    },
-    {
-    "audio_layers": [
+topcast.add_chapter(
+    audio_layers=[
         {
-            "audio": {
-                "content": "Portugal (Portuguese pronunciation: [puɾtuˈɣal]), officially the Portuguese Republic (Portuguese: República Portuguesa [ʁɛˈpuβlikɐ puɾtuˈɣezɐ]),[note 4] is a country located on the Iberian Peninsula, in southwestern Europe, and whose territory also includes the Atlantic archipelagos of the Azores and Madeira. It features the westernmost point in continental Europe, and its Iberian portion is bordered to the west and south by the Atlantic Ocean and to the north and east by Spain, the sole country to have a land border with Portugal. Its two archipelagos form two autonomous regions with their own regional governments. Lisbon is the capital and largest city by population.",
-                "theme": Introduction,
-                "tts_provider": ElevenLabs
-            }, 
-            "is_main": True, 
+            "audio": "sounds/jingle.wav",
+            "sets_length": True,
         }
+    ]
+)
+topcast.add_chapter(
+    audio_layers=[
+        {
+            "audio": {
+                "content": "It features the westernmost point in continental Europe, and its Iberian portion is bordered to the west and south by the Atlantic Ocean and to the north and east by Spain.",
+            },
+            "sets_length": True,
+            "fade_in": 1200,
+            "fade_out": 1200,
+        },
+        {"audio": "sounds/background.mp3", "sets_length": False, "volume": 0.5},
     ],
+    crossfade=2400,
+)
+topcast.add_chapter(
+    audio_layers=[
+        {
+            "audio": {
+                "content": "It features the westernmost point in continental Europe, and its Iberian portion is bordered to the west and south by the Atlantic Ocean and to the north and east by Spain.",
+                "tts_provider": GCP, 
+                "theme": Summary,
+            },
+            "sets_length": True,
+            "fade_in": 1200,
+            "fade_out": 1200,
+        },
+    ],
+    crossfade=2400,
+)
 
-    "crossfade": 2400, 
-},
-]
+topcast.generate()
+topcast.export("podcast.wav", format="wav")
 
-podcast = generate(timeline)
-podcast.export("podcast_3.wav", format="wav")
 ```
-##Installation
+
+## Installation
 Install the package using pip:
 
 ```bash
 pip install topcast
-````
+```
+
+## Usage
 
-##Usage
 1. Import the necessary modules and set the API keys:
+
 ```python
-from topcast.chatgpt_themes import Introduction, Interview, Conclusion, Summary
-from topcast.tts_providers import ElevenLabs, GCP
-import os
-from topcast import generate, set_elevenlab_api_key, set_google_credentials, set_openai_api_key
+from topcast import (
+    set_elevenlab_api_key,
+    set_google_credentials,
+    set_openai_api_key,
+    Topcaster,
+)
+
+from topcast.tts_providers import GCP
+from topcast.chatgpt_themes import Summary
 
 from dotenv import load_dotenv
 
 load_dotenv()
 
 set_elevenlab_api_key(os.environ["ELEVENLAB_API_KEY"])
 set_openai_api_key(os.environ["OPENAI_API_KEY"])
-set_google_credentials('gcp-keyfile.json')
+set_google_credentials("gcp-keyfile.json")
 ```
-2. Create a timeline with the desired podcast structure:
+
+2. Create a Topcaster object and add chapters with the desired podcast structure:
+
 ```python
-timeline = [
-    {
-        "audio_layers": [
-            {
-                "audio": 'sounds/jingle.wav', 
-                "is_main": True, 
-            }
-        ],
-    },
-    {
-    "audio_layers": [
+topcast = Topcaster()
+
+topcast.add_chapter(
+    audio_layers=[
+        {
+            "audio": "sounds/jingle.wav",
+            "sets_length": True,
+        }
+    ]
+)
+topcast.add_chapter(
+    audio_layers=[
         {
             "audio": {
                 "content": "Portugal...",
-                "theme": Introduction,
-                "tts_provider": ElevenLabs
-            }, 
-            "is_main": True, 
-        }
+                "tts_provider": GCP,
+                "theme": Summary,
+            },
+            "sets_length": True,
+            "fade_in": 1200,
+            "fade_out": 1200,
+        },
+        {"audio": "sounds/background.mp3", "sets_length": False, "volume": 0.5},
     ],
+    crossfade=2400,
+)
 
-    "crossfade": 2400, 
-},
-]
 ```
+
 3. Generate and export the podcast:
+
 ```python
-podcast = generate(timeline)
-podcast.export("podcast_output.wav", format="wav")
+topcast.generate()
+topcast.export("podcast_output.wav", format="wav")
 ```
-
-This will create a podcast using the given *timeline* and save it as a WAV file named *podcast_output.wav*.
+This will create a podcast using the given chapters and save it as a WAV file named podcast_output.wav.
 ##Customization
-You can customize your podcast by modifying the *timeline* list. Each element in the list represents a segment of the podcast. You can add more segments with different themes, TTS providers, and audio layers.
+You can customize your podcast by adding more chapters to the Topcaster object. Each chapter represents a segment of the podcast. You can add more segments with different themes, TTS providers, and audio layers.
 
 For example, if you want to add an interview segment, you can include it like this:
+
 ```python
-{
-    "audio_layers": [
+from topcast import Topcaster
+from topcast.chatgpt_themes import Interview
+
+topcast = Topcast()
+
+topcast.add_chapter(
+    audio_layers=[
         {
             "audio": {
-                "content": "Interview text...",
+                "content": "It features the westernmost point in continental Europe, and its Iberian portion is bordered to the west and south by the Atlantic Ocean and to the north and east by Spain...", # <- gets automatically converted into an interview script
+                "tts_provider": GCP,
                 "theme": Interview,
-                "tts_provider": GCP
-            }, 
-            "is_main": True, 
-        }
+            },
+            "sets_length": True,
+            "fade_in": 1200,
+            "fade_out": 1200,
+        },
     ],
-    "crossfade": 2400, 
-}
+    crossfade=2400,
+)
+
 
 ```
 
-You can also add sound effects or background music by adding additional audio layers:
+You can also add sound effects or background music by adding additional audio layers within a chapter:
 
 ```python
-{
-    "audio_layers": [
+from topcast import Topcaster
+
+topcast = Topcast()
+
+topcast.add_chapter(
+    audio_layers=[
         {
             "audio": 'sounds/background_music.wav',
-            "is_main": False,
+            "sets_length": False,
             "volume": 0.3,
         },
         {
             "audio": {
                 "content": "Text content...",
-                "theme": Conclusion,
-                "tts_provider": ElevenLabs
-            }, 
-            "is_main": True, 
+                "tts_provider": GCP,
+                "theme": Summary,
+            },
+            "sets_length": True,
+            "fade_in": 1200,
+            "fade_out": 1200,
         }
     ],
-    "crossfade": 2400, 
-}
+    crossfade=2400,
+)
 ```
-This will add background music with a volume of 0.3 to the conclusion segment.
-
-Remember to adjust the *crossfade* value for smoother transitions between segments.
-
-
-
+This will add background music with a volume of 0.3 to the chapter.
 
+Remember to adjust the crossfade value for smoother transitions between chapters.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `topcast-0.1.4/setup.py` & `topcast-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="topcast",
-    version="0.1.4",
+    version="0.1.5",
     author="Gorm Labenz",
     author_email="gorm@labenz.io",
     description="A Python package for Topcast",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/gormlabenz/topcast",
     packages=find_packages(),
@@ -29,9 +29,10 @@
     install_requires=[
         "openai",
         "protobuf",
         "pydantic",
         "pydub",
         "elevenlabs",
         "google-cloud-texttospeech",
+        "gTTS"
     ],
 )
```

### Comparing `topcast-0.1.4/topcast/chatgpt_themes/base.py` & `topcast-0.1.5/topcast/chatgpt_themes/base.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from abc import ABC, abstractmethod
+import openai
 
 class ChatGPTThemeBase(ABC):
     def __init__(self):
         self.system_prompt = ""
         self.messages = []
         
     def get_messages(self, input_message:str):
@@ -12,14 +13,25 @@
             "role":"system", "content": self.system_prompt})
     
         messages.append({
           "role":"user", "content": self.create_content(input_message)})
         
         return messages
     
+    async def create_chat_completion(self, input_message: str):
+            messages = self.get_messages(input_message=input_message)
+            
+            completion = openai.ChatCompletion.create(
+                model="gpt-3.5-turbo",
+                messages=messages
+            )
+            content = completion.choices[0].message.content
+            
+            return self.extract_content(content)
+        
     @abstractmethod
     def create_content(self, input_content: str):
         pass
       
     @abstractmethod
     def extract_content(self, response_content: str):
         pass
```

### Comparing `topcast-0.1.4/topcast/chatgpt_themes/conclusion.py` & `topcast-0.1.5/topcast/chatgpt_themes/conclusion.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from .base import ChatGPTThemeBase
-from topcast.models import TTSText
+from topcast.models import TTSItem
 
 class Conclusion(ChatGPTThemeBase):
   def __init__(self):
     super().__init__()
     
     self.system_prompt = "You are an AI language model that generates an entertaining conclusion about a text. Ensure that the conclusion is engaging, informative, and captures the audience's attention. The conclusion should be no longer than three sentences."
     self.messages = [
        {"role": "user", "content": """Could you send me a conclusion of an text? Here is the text:
         
-In Persia's semi-desert towns, oases were fed through aqueducts carrying mountain water to support intensive food production, nurtured by wastes from the communities.[5] In Machu Picchu, water was conserved and reused as part of the stepped architecture of the city, and vegetable beds were designed to gather sun in order to prolong the growing season.[5]
+In Persia's semi-desert towns, oases were fed through aqueducts carrying mountain water to support intensive food production, nurtured by wastes from the communities.[5] In Machu Picchu, water was conserved and reused as part of the chapterped architecture of the city, and vegetable beds were designed to gather sun in order to prolong the growing season.[5]
 The idea of supplemental food production beyond rural farming operations and distant imports is not new. It was used during war and depression times when food shortage issues arose, as well as during times of relative abundance. Allotment gardens emerged in Germany in the early 19th century as a response to poverty and food insecurity.[6]
 In 1893, citizens of a depression-struck Detroit were asked to use vacant lots to grow vegetables. They were nicknamed Pingree's Potato Patches after the mayor, Hazen S. Pingree, who came up with the idea. He intended for these gardens to produce income, food supply, and boost independence during times of hardship.[7] Victory gardens sprouted during WWI and WWII and were fruit, vegetable, and herb gardens in the US, Canada, and UK. This effort was undertaken by citizens to reduce pressure on food production that was to support the war effort.
 During World War I, President Woodrow Wilson called upon all American citizens to utilize any available open food growth, seeing this as a way to pull them out of a potentially damaging situation.[8] Since most of Europe was consumed with war, they were unable to produce sufficient food supplies to be shipped to the US and a new plan was implemented with the goal of feeding the US and even supply a surplus to other countries in need. By 1919, over 5 million plots were growing food and over 500 million pounds of produce was harvested.
 A very similar practice came into use during the Great Depression that provided a purpose, job and food to those who would otherwise be without anything during such harsh times. These efforts helped raise spirits and boost economic growth. Over 2.8 million dollars worth of food was produced from the subsistence gardens during the Depression. By World War II, the War/Food Administration set up a National Victory Garden Program that set out to systematically establish functioning agriculture within cities. With this new plan in action, as many as 5.5 million Americans took part in the victory garden movement and over nine million pounds of fruit and vegetables were grown a year, accounting for 44% of US-grown produce throughout that time.[9]"""},
            {"role": "assistant", "content": """In the face of adversity, humanity has historically turned to urban agriculture as a means of sustenance and resilience. From ancient Persia to the victory gardens of WWII, communities have united to grow food in times of hardship and abundance alike. The enduring legacy of these gardens highlights the power of ingenuity, collaboration, and resourcefulness in addressing global challenges."""}
   ]
  
@@ -21,8 +21,8 @@
     return  f"""Could you send me another conclusion? Here is the text: 
   
   {input_content}
   
   """
   
   def extract_content(self, response_content: str):
-    return [TTSText(text=response_content, gender="female")]
+    return [TTSItem(text=response_content, gender="female")]
```

### Comparing `topcast-0.1.4/topcast/chatgpt_themes/interview.py` & `topcast-0.1.5/topcast/chatgpt_themes/interview.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from .base import ChatGPTThemeBase
-from topcast.models import TTSText
+from topcast.models import TTSItem
 import re 
 
 class Interview(ChatGPTThemeBase):
   def __init__(self):
     super().__init__()
     
     self.system_prompt = "You are an AI language model that generates an entertaining interview between two speakers discussing the intricacies and fascinating aspects of a specific topic. Ensure that the dialogue is engaging, informative, and captures the audience's attention. The speakers must be called Interviewer and Expert so the text can be used."
     self.messages = [
        {"role": "user", "content": """Could you send me a script of an interview? Please keep in mind, it is very importend that in the script the interviewer must be called Interviewer and the interviewer Expert. Here is the text the interview should be based on:
 
-In Persia's semi-desert towns, oases were fed through aqueducts carrying mountain water to support intensive food production, nurtured by wastes from the communities.[5] In Machu Picchu, water was conserved and reused as part of the stepped architecture of the city, and vegetable beds were designed to gather sun in order to prolong the growing season.[5]
+In Persia's semi-desert towns, oases were fed through aqueducts carrying mountain water to support intensive food production, nurtured by wastes from the communities.[5] In Machu Picchu, water was conserved and reused as part of the chapterped architecture of the city, and vegetable beds were designed to gather sun in order to prolong the growing season.[5]
 The idea of supplemental food production beyond rural farming operations and distant imports is not new. It was used during war and depression times when food shortage issues arose, as well as during times of relative abundance. Allotment gardens emerged in Germany in the early 19th century as a response to poverty and food insecurity.[6]
 In 1893, citizens of a depression-struck Detroit were asked to use vacant lots to grow vegetables. They were nicknamed Pingree's Potato Patches after the mayor, Hazen S. Pingree, who came up with the idea. He intended for these gardens to produce income, food supply, and boost independence during times of hardship.[7] Victory gardens sprouted during WWI and WWII and were fruit, vegetable, and herb gardens in the US, Canada, and UK. This effort was undertaken by citizens to reduce pressure on food production that was to support the war effort.
 During World War I, President Woodrow Wilson called upon all American citizens to utilize any available open food growth, seeing this as a way to pull them out of a potentially damaging situation.[8] Since most of Europe was consumed with war, they were unable to produce sufficient food supplies to be shipped to the US and a new plan was implemented with the goal of feeding the US and even supply a surplus to other countries in need. By 1919, over 5 million plots were growing food and over 500 million pounds of produce was harvested.
 A very similar practice came into use during the Great Depression that provided a purpose, job and food to those who would otherwise be without anything during such harsh times. These efforts helped raise spirits and boost economic growth. Over 2.8 million dollars worth of food was produced from the subsistence gardens during the Depression. By World War II, the War/Food Administration set up a National Victory Garden Program that set out to systematically establish functioning agriculture within cities. With this new plan in action, as many as 5.5 million Americans took part in the victory garden movement and over nine million pounds of fruit and vegetables were grown a year, accounting for 44% of US-grown produce throughout that time.[9]"""},
            {"role": "assistant", "content": """Interviewer: Welcome to today's show! Today, we have a special guest, an expert in the history of urban agriculture. Please welcome our Dr. Green! Dr. Green, Can you give us a brief introduction to urban agriculture and its historical significance?
 
 Expert: Thank you for having me! Urban agriculture is the practice of growing, processing, and distributing food in or around urban areas. Its roots can be traced back to ancient civilizations like Persia and the Inca Empire, where people used innovative techniques to support intensive food production. The concept has been adapted in various forms throughout history, particularly during times of war, depression, or food shortages.
@@ -46,10 +46,10 @@
   def extract_content(self, response_content: str):
     pattern = r"(Interviewer|Expert): (.*?)\n"
     matches = re.findall(pattern, response_content, re.MULTILINE)
         
     extracted_text = []
     
     for match in matches:
-      extracted_text.append(TTSText(text=match[1], gender="male" if match[0] == "Interviewer" else "female"))
+      extracted_text.append(TTSItem(text=match[1], gender="male" if match[0] == "Interviewer" else "female"))
         
     return extracted_text
```

### Comparing `topcast-0.1.4/topcast/chatgpt_themes/introduction.py` & `topcast-0.1.5/topcast/chatgpt_themes/introduction.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from .base import ChatGPTThemeBase
-from topcast.models import TTSText
+from topcast.models import TTSItem
 
 class Introduction(ChatGPTThemeBase):
   def __init__(self):
     super().__init__()
     
     self.system_prompt = "You are an AI language model, and your task is to generate a brief and entertaining introductions of a text. Make it interesting and engaging without revealing too much about it." 
     self.messages = [
@@ -15,8 +15,8 @@
            {"role": "assistant", "content": """Welcome to our podcast, where we'll dive into the fascinating world of Finland's Olkiluoto Nuclear Power Plant - home to Europe's strongest reactor, the Energizer Bunny of the nuclear world, and just a hop, skip, and a jump from the bustling metropolis of Pori!"""}
   ]
  
   def create_content(self, input_content: str):
     return  f"""Could you write another introduction? Here are some information about the topic: {input_content}"""
   
   def extract_content(self, response_content: str):
-    return [TTSText(text=response_content, gender="female")]
+    return [TTSItem(text=response_content, gender="female")]
```

### Comparing `topcast-0.1.4/topcast/chatgpt_themes/summary.py` & `topcast-0.1.5/topcast/chatgpt_themes/summary.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from .base import ChatGPTThemeBase
-from topcast.models import TTSText
+from topcast.models import TTSItem
 
 class Summary(ChatGPTThemeBase):
   def __init__(self):
     super().__init__()
     
     self.system_prompt = "You are an AI language model, and your task is to generate a brief and entertaining summary of a text. Make it interesting and engaging."   
     self.messages = [
@@ -23,8 +23,8 @@
 So, grab your Geiger counters and protective gear, because we're about to embark on an entertaining and electrifying journey into the heart of Finland's Olkiluoto Nuclear Power Plant!"""}
   ]
  
   def create_content(self, input_content: str):
     return  f"""Could you write another summary? Here are some information about it: {input_content}"""
   
   def extract_content(self, response_content: str):
-    return [TTSText(text=response_content, gender="female")]
+    return [TTSItem(text=response_content, gender="female")]
```

### Comparing `topcast-0.1.4/topcast/models.py` & `topcast-0.1.5/topcast/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 from pydantic import BaseModel, Field, validator
-from typing import List, Union, Any, Type
+from typing import List, Union, Any, Type, Optional
 from pydub.audio_segment import AudioSegment
 
 
-class TTSText(BaseModel):
+class TTSItem(BaseModel):
     text: str
     gender: str
 
-class StepData(BaseModel):
+class ChapterData(BaseModel):
     raw_audio: AudioSegment = None
-    text_list: List[TTSText] = []
+    text_list: List[TTSItem] = []
     audio_list: List[AudioSegment] = []
 
     class Config:
         arbitrary_types_allowed = True
         
-class AudioContent(BaseModel):
+class AudioItem(BaseModel):
     from topcast.tts_providers.base import TTSProviderBase
+    from topcast.tts_providers.gt import GTTS # <-- make default provider
     from topcast.chatgpt_themes.base import ChatGPTThemeBase
+    from topcast.chatgpt_themes.none_theme import NoneTheme# <-- make default theme
     
     content: str
-    theme: Type[ChatGPTThemeBase]
-    tts_provider: Type[TTSProviderBase]
+    theme: Optional[Type[ChatGPTThemeBase]] = Field(default=NoneTheme)
+    tts_provider: Optional[Type[TTSProviderBase]] = Field(default=GTTS)
 
     @validator("theme")
     def check_theme_base_class(cls, value):
         from topcast.chatgpt_themes.base import ChatGPTThemeBase
         
         if not issubclass(value, ChatGPTThemeBase):
             raise ValueError("The provided theme class does not inherit from ChatGPTThemeBase.")
@@ -36,32 +38,31 @@
         from topcast.tts_providers.base import TTSProviderBase
         
         if not issubclass(value, TTSProviderBase):
             raise ValueError("The provided TTS provider class does not inherit from TTSProviderBase.")
         return value
 
 class AudioLayer(BaseModel):
-    audio: Union[str, AudioSegment, AudioContent]
-    data: StepData = None
-    is_main: bool = False
+    audio: Union[str, AudioSegment, AudioItem]
+    data: ChapterData = None
+    sets_length: bool = False
     fade_in: int = Field(1, ge=1)
     fade_out: int = Field(1, ge=1)
     padding_start: int = Field(0, ge=0)
     padding_end: int = Field(0, ge=0)
     crossfade: int = Field(0, ge=0)
     volume: int = Field(1, ge=0, le=1)
     
     class Config:
         arbitrary_types_allowed = True
         
-class Step(BaseModel):
+class Chapter(BaseModel):
     audio_layers: List[AudioLayer]
     fade_in: int = Field(1, ge=1)
     fade_out: int = Field(1, ge=1)
     padding_start: int = Field(0, ge=0)
     padding_end: int = Field(0, ge=0)
     crossfade: int = Field(0, ge=0)
     volume: float = Field(1, ge=0, le=1)
-    
 
 class Timeline(BaseModel):
-    timeline: List[Step]
+    timeline: List[Chapter]
```

### Comparing `topcast-0.1.4/topcast/podcaster.py` & `topcast-0.1.5/topcast/topcaster.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,67 +1,73 @@
 import asyncio
 from pydub import AudioSegment
 
-from .models import Timeline, AudioContent, StepData
-from .chatgpt import ChatGPT
+from .models import Timeline, AudioItem, ChapterData, Chapter
 from .cutter import Cutter
 
-class Podcaster:
-    def __init__(self, timeline: Timeline):
+class Topcaster:
+    def __init__(self, timeline: Timeline = []):
         self.timeline = Timeline(timeline=timeline)
-        self.podcast = AudioSegment.empty()
+        self.topcast = AudioSegment.empty()
+        
+    def add_chapter(self, audio_layers = [], fade_in: int = 1, fade_out: int = 1 , padding_start: int = 0 , padding_end: int = 0 , crossfade: int = 0, volume: float = 1):
+        
+        chapter = Chapter(audio_layers=audio_layers, fade_in=fade_in, fade_out=fade_out, padding_start=padding_start, padding_end=padding_end, crossfade=crossfade, volume=volume)
+        self.timeline.timeline.append(chapter)
         
     def generate(self):
-        self.add_step_data_dict()
+        self.add_chapter_data_dict()
         self.open_audio_files()
         asyncio.run(self.generate_text())
         asyncio.run(self.generate_speech())
         self.cut()
         
-        return self.podcast
+        return self.topcast
 
-    def add_step_data_dict(self):
-        for step in self.timeline.timeline:
-            for audio_layer in step.audio_layers:
-                audio_layer.data = StepData(raw_audio= None, text_list=[], audio_list= [])
+    def add_chapter_data_dict(self):
+        for chapter in self.timeline.timeline:
+            for audio_layer in chapter.audio_layers:
+                audio_layer.data = ChapterData(raw_audio= None, text_list=[], audio_list= [])
                 
     def open_audio_files(self):
-        for step in self.timeline.timeline:
-            for audio_layer in step.audio_layers:
+        for chapter in self.timeline.timeline:
+            for audio_layer in chapter.audio_layers:
                 if type(audio_layer.audio) == str:
                     audio_layer.data.raw_audio = AudioSegment.from_file(audio_layer.audio)              
 
     async def generate_text(self):
         tasks = []
-        for step in self.timeline.timeline:
-            for audio_layer in step.audio_layers:
-                if isinstance(audio_layer.audio, AudioContent):
+        for chapter in self.timeline.timeline:
+            for audio_layer in chapter.audio_layers:
+                if isinstance(audio_layer.audio, AudioItem):
                     tasks.append(
                         self.generate_text_and_assign(audio_layer)
                     )
         await asyncio.gather(*tasks)
         
     async def generate_speech(self):
         tasks = []
         
-        for step in self.timeline.timeline:
-            for audio_layer in step.audio_layers:
-                if isinstance(audio_layer.audio, AudioContent):
+        for chapter in self.timeline.timeline:
+            for audio_layer in chapter.audio_layers:
+                if isinstance(audio_layer.audio, AudioItem):
                     tasks.append(self.generate_speech_and_assign(audio_layer))
                     
         await asyncio.gather(*tasks)
         
     def cut(self):
         
-        podcast =  Cutter(self.timeline).cut()
-        self.podcast = podcast
+        topcast =  Cutter(self.timeline).cut()
+        self.topcast = topcast
     
     async def generate_text_and_assign(self, audio_layer):
-        chatgpt = ChatGPT(audio_layer.audio)
-        generated_text = await chatgpt.create_chat_completion(audio_layer.audio.content)
+        chatgpt_theme = audio_layer.audio.theme()
+        
+        generated_text = await chatgpt_theme.create_chat_completion(audio_layer.audio.content)
+        
         audio_layer.data.text_list = generated_text
         
     async def generate_speech_and_assign(self, audio_layer):
         provider = audio_layer.audio.tts_provider()
         tasks = []
         
         for text in audio_layer.data.text_list:
@@ -69,9 +75,9 @@
                 provider.tts(text)
             )
             
             
         results = await asyncio.gather(*tasks)        
         audio_layer.data.audio_list = results
         
-    def save(self, file_name = "podcast.mp3", format="mp3"):
-        self.podcast.export(file_name, format = format)
+    def export(self, file_name = "topcast.mp3", format="mp3"):
+        self.topcast.export(file_name, format = format)
```

### Comparing `topcast-0.1.4/topcast/tts_providers/elevenlabs.py` & `topcast-0.1.5/topcast/tts_providers/elevenlabs.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 from .base import TTSProviderBase
-from ..models import TTSText
+from ..models import TTSItem
 
 import asyncio
 from elevenlabs import generate
 from pydub import AudioSegment
 from io import BytesIO
 
-
-
 class ElevenLabs(TTSProviderBase):
     def __init__(self):
         super().__init__()
         self.voices = {
             'male': "Adam",
             'female': "Bella"
         }
 
-    async def tts(self, tts_text: TTSText):
+    async def tts(self, tts_text: TTSItem):
         voice = self.get_voice(tts_text.gender)
         
         def _synthesize_speech():
           return  AudioSegment.from_file(BytesIO(generate(text=tts_text.text, voice=voice)))
     
     # Run the synchronous Text-to-Speech code in a separate thread
         return await asyncio.to_thread(_synthesize_speech)
```

### Comparing `topcast-0.1.4/topcast/tts_providers/gcp.py` & `topcast-0.1.5/topcast/tts_providers/gcp.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from .base import TTSProviderBase
 from google.cloud import texttospeech
 import asyncio
-from topcast.models import TTSText
+from topcast.models import TTSItem
 from pydub import AudioSegment
 from io import BytesIO
 
 class GCP(TTSProviderBase):
     def __init__(self):
         super().__init__()
         self.voices = {
@@ -15,15 +15,15 @@
             ),
             'female': texttospeech.VoiceSelectionParams(
                 language_code="en-US", ssml_gender=texttospeech.SsmlVoiceGender.FEMALE,
                 name="en-US-Neural2-C"
             )
         }
         
-    async def tts(self, tts_text: TTSText):
+    async def tts(self, tts_text: TTSItem):
         voice = self.get_voice(tts_text.gender)
         
         def _synthesize_speech():
           client = texttospeech.TextToSpeechClient()
 
           # Set the audio configuration
           audio_config = texttospeech.AudioConfig(
```

### Comparing `topcast-0.1.4/topcast.egg-info/PKG-INFO` & `topcast-0.1.5/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,177 +1,202 @@
-Metadata-Version: 2.1
-Name: topcast
-Version: 0.1.4
-Summary: A Python package for Topcast
-Home-page: https://github.com/gormlabenz/topcast
-Author: Gorm Labenz
-Author-email: gorm@labenz.io
-License: MIT
-Keywords: topcast tts text-to-speech gcp google openai elevenlabs
-Platform: UNKNOWN
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
 # Topcast: Turn Text into Podcasts with TTS and Language Models
+
 Topcast is a Python package that allows you to transform text into a podcast using Text-to-Speech (TTS) and language models. With Topcast, you can provide a text, and the package will create a podcast with an introduction, interview, conclusion, sound effects, and more. Topcast supports various TTS providers and language models.
 
-##Example Implementation
+## Example Implementation
+
 ```python
-from topcast.chatgpt_themes import Introduction, Interview, Conclusion, Summary
-from topcast.tts_providers import ElevenLabs, GCP
 import os
-from topcast import generate, set_elevenlab_api_key, set_google_credentials, set_openai_api_key
+from topcast import (
+    set_elevenlab_api_key,
+    set_google_credentials,
+    set_openai_api_key,
+    Topcaster,
+)
+
+from topcast.tts_providers import GCP
+from topcast.chatgpt_themes import Summary
 
 from dotenv import load_dotenv
 
 load_dotenv()
 
 set_elevenlab_api_key(os.environ["ELEVENLAB_API_KEY"])
 set_openai_api_key(os.environ["OPENAI_API_KEY"])
-set_google_credentials('gcp-keyfile.json')
+set_google_credentials("gcp-keyfile.json")
+
+topcast = Topcaster()
 
-timeline = [
-    {
-        "audio_layers": [
-            {
-                "audio": 'sounds/jingle.wav', 
-                "is_main": True, 
-            }
-        ],
-    },
-    {
-    "audio_layers": [
+topcast.add_chapter(
+    audio_layers=[
         {
-            "audio": {
-                "content": "Portugal (Portuguese pronunciation: [puɾtuˈɣal]), officially the Portuguese Republic (Portuguese: República Portuguesa [ʁɛˈpuβlikɐ puɾtuˈɣezɐ]),[note 4] is a country located on the Iberian Peninsula, in southwestern Europe, and whose territory also includes the Atlantic archipelagos of the Azores and Madeira. It features the westernmost point in continental Europe, and its Iberian portion is bordered to the west and south by the Atlantic Ocean and to the north and east by Spain, the sole country to have a land border with Portugal. Its two archipelagos form two autonomous regions with their own regional governments. Lisbon is the capital and largest city by population.",
-                "theme": Introduction,
-                "tts_provider": ElevenLabs
-            }, 
-            "is_main": True, 
+            "audio": "sounds/jingle.wav",
+            "sets_length": True,
         }
+    ]
+)
+topcast.add_chapter(
+    audio_layers=[
+        {
+            "audio": {
+                "content": "It features the westernmost point in continental Europe, and its Iberian portion is bordered to the west and south by the Atlantic Ocean and to the north and east by Spain.",
+            },
+            "sets_length": True,
+            "fade_in": 1200,
+            "fade_out": 1200,
+        },
+        {"audio": "sounds/background.mp3", "sets_length": False, "volume": 0.5},
+    ],
+    crossfade=2400,
+)
+topcast.add_chapter(
+    audio_layers=[
+        {
+            "audio": {
+                "content": "It features the westernmost point in continental Europe, and its Iberian portion is bordered to the west and south by the Atlantic Ocean and to the north and east by Spain.",
+                "tts_provider": GCP, 
+                "theme": Summary,
+            },
+            "sets_length": True,
+            "fade_in": 1200,
+            "fade_out": 1200,
+        },
     ],
+    crossfade=2400,
+)
 
-    "crossfade": 2400, 
-},
-]
+topcast.generate()
+topcast.export("podcast.wav", format="wav")
 
-podcast = generate(timeline)
-podcast.export("podcast_3.wav", format="wav")
 ```
-##Installation
+
+## Installation
 Install the package using pip:
 
 ```bash
 pip install topcast
-````
+```
+
+## Usage
 
-##Usage
 1. Import the necessary modules and set the API keys:
+
 ```python
-from topcast.chatgpt_themes import Introduction, Interview, Conclusion, Summary
-from topcast.tts_providers import ElevenLabs, GCP
-import os
-from topcast import generate, set_elevenlab_api_key, set_google_credentials, set_openai_api_key
+from topcast import (
+    set_elevenlab_api_key,
+    set_google_credentials,
+    set_openai_api_key,
+    Topcaster,
+)
+
+from topcast.tts_providers import GCP
+from topcast.chatgpt_themes import Summary
 
 from dotenv import load_dotenv
 
 load_dotenv()
 
 set_elevenlab_api_key(os.environ["ELEVENLAB_API_KEY"])
 set_openai_api_key(os.environ["OPENAI_API_KEY"])
-set_google_credentials('gcp-keyfile.json')
+set_google_credentials("gcp-keyfile.json")
 ```
-2. Create a timeline with the desired podcast structure:
+
+2. Create a Topcaster object and add chapters with the desired podcast structure:
+
 ```python
-timeline = [
-    {
-        "audio_layers": [
-            {
-                "audio": 'sounds/jingle.wav', 
-                "is_main": True, 
-            }
-        ],
-    },
-    {
-    "audio_layers": [
+topcast = Topcaster()
+
+topcast.add_chapter(
+    audio_layers=[
+        {
+            "audio": "sounds/jingle.wav",
+            "sets_length": True,
+        }
+    ]
+)
+topcast.add_chapter(
+    audio_layers=[
         {
             "audio": {
                 "content": "Portugal...",
-                "theme": Introduction,
-                "tts_provider": ElevenLabs
-            }, 
-            "is_main": True, 
-        }
+                "tts_provider": GCP,
+                "theme": Summary,
+            },
+            "sets_length": True,
+            "fade_in": 1200,
+            "fade_out": 1200,
+        },
+        {"audio": "sounds/background.mp3", "sets_length": False, "volume": 0.5},
     ],
+    crossfade=2400,
+)
 
-    "crossfade": 2400, 
-},
-]
 ```
+
 3. Generate and export the podcast:
+
 ```python
-podcast = generate(timeline)
-podcast.export("podcast_output.wav", format="wav")
+topcast.generate()
+topcast.export("podcast_output.wav", format="wav")
 ```
-
-This will create a podcast using the given *timeline* and save it as a WAV file named *podcast_output.wav*.
+This will create a podcast using the given chapters and save it as a WAV file named podcast_output.wav.
 ##Customization
-You can customize your podcast by modifying the *timeline* list. Each element in the list represents a segment of the podcast. You can add more segments with different themes, TTS providers, and audio layers.
+You can customize your podcast by adding more chapters to the Topcaster object. Each chapter represents a segment of the podcast. You can add more segments with different themes, TTS providers, and audio layers.
 
 For example, if you want to add an interview segment, you can include it like this:
+
 ```python
-{
-    "audio_layers": [
+from topcast import Topcaster
+from topcast.chatgpt_themes import Interview
+
+topcast = Topcast()
+
+topcast.add_chapter(
+    audio_layers=[
         {
             "audio": {
-                "content": "Interview text...",
+                "content": "It features the westernmost point in continental Europe, and its Iberian portion is bordered to the west and south by the Atlantic Ocean and to the north and east by Spain...", # <- gets automatically converted into an interview script
+                "tts_provider": GCP,
                 "theme": Interview,
-                "tts_provider": GCP
-            }, 
-            "is_main": True, 
-        }
+            },
+            "sets_length": True,
+            "fade_in": 1200,
+            "fade_out": 1200,
+        },
     ],
-    "crossfade": 2400, 
-}
+    crossfade=2400,
+)
+
 
 ```
 
-You can also add sound effects or background music by adding additional audio layers:
+You can also add sound effects or background music by adding additional audio layers within a chapter:
 
 ```python
-{
-    "audio_layers": [
+from topcast import Topcaster
+
+topcast = Topcast()
+
+topcast.add_chapter(
+    audio_layers=[
         {
             "audio": 'sounds/background_music.wav',
-            "is_main": False,
+            "sets_length": False,
             "volume": 0.3,
         },
         {
             "audio": {
                 "content": "Text content...",
-                "theme": Conclusion,
-                "tts_provider": ElevenLabs
-            }, 
-            "is_main": True, 
+                "tts_provider": GCP,
+                "theme": Summary,
+            },
+            "sets_length": True,
+            "fade_in": 1200,
+            "fade_out": 1200,
         }
     ],
-    "crossfade": 2400, 
-}
+    crossfade=2400,
+)
 ```
-This will add background music with a volume of 0.3 to the conclusion segment.
-
-Remember to adjust the *crossfade* value for smoother transitions between segments.
-
-
-
-
-
+This will add background music with a volume of 0.3 to the chapter.
 
+Remember to adjust the crossfade value for smoother transitions between chapters.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `topcast-0.1.4/topcast.egg-info/SOURCES.txt` & `topcast-0.1.5/topcast.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 LICENSE.txt
 README.md
 setup.py
 topcast/__init__.py
-topcast/chatgpt.py
 topcast/cutter.py
 topcast/models.py
-topcast/podcaster.py
+topcast/topcaster.py
 topcast.egg-info/PKG-INFO
 topcast.egg-info/SOURCES.txt
 topcast.egg-info/dependency_links.txt
 topcast.egg-info/requires.txt
 topcast.egg-info/top_level.txt
 topcast/chatgpt_themes/__init__.py
 topcast/chatgpt_themes/base.py
 topcast/chatgpt_themes/conclusion.py
 topcast/chatgpt_themes/interview.py
 topcast/chatgpt_themes/introduction.py
+topcast/chatgpt_themes/none_theme.py
 topcast/chatgpt_themes/summary.py
 topcast/tts_providers/__init__.py
 topcast/tts_providers/base.py
 topcast/tts_providers/elevenlabs.py
-topcast/tts_providers/gcp.py
+topcast/tts_providers/gcp.py
+topcast/tts_providers/gt.py
```

