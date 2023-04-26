# Comparing `tmp/faster-whisper-0.4.1.tar.gz` & `tmp/faster-whisper-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faster-whisper-0.4.1.tar", last modified: Tue Apr  4 10:18:20 2023, max compression
+gzip compressed data, was "faster-whisper-0.5.0.tar", last modified: Tue Apr 25 15:02:25 2023, max compression
```

## Comparing `faster-whisper-0.4.1.tar` & `faster-whisper-0.5.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 10:18:20.594184 faster-whisper-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-04 10:18:17.000000 faster-whisper-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-04 10:18:17.000000 faster-whisper-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9040 2023-04-04 10:18:20.594184 faster-whisper-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6838 2023-04-04 10:18:17.000000 faster-whisper-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 10:18:20.590183 faster-whisper-0.4.1/faster_whisper/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-04 10:18:17.000000 faster-whisper-0.4.1/faster_whisper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 10:18:20.590183 faster-whisper-0.4.1/faster_whisper/assets/
--rw-r--r--   0 runner    (1001) docker     (123)  1807524 2023-04-04 10:18:17.000000 faster-whisper-0.4.1/faster_whisper/assets/silero_vad.onnx
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-04-04 10:18:17.000000 faster-whisper-0.4.1/faster_whisper/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-04-04 10:18:17.000000 faster-whisper-0.4.1/faster_whisper/feature_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-04-04 10:18:17.000000 faster-whisper-0.4.1/faster_whisper/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    29909 2023-04-04 10:18:17.000000 faster-whisper-0.4.1/faster_whisper/transcribe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-04-04 10:18:17.000000 faster-whisper-0.4.1/faster_whisper/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9840 2023-04-04 10:18:17.000000 faster-whisper-0.4.1/faster_whisper/vad.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 10:18:20.590183 faster-whisper-0.4.1/faster_whisper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9040 2023-04-04 10:18:20.000000 faster-whisper-0.4.1/faster_whisper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-04 10:18:20.000000 faster-whisper-0.4.1/faster_whisper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 10:18:20.000000 faster-whisper-0.4.1/faster_whisper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-04 10:18:20.000000 faster-whisper-0.4.1/faster_whisper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-04 10:18:20.000000 faster-whisper-0.4.1/faster_whisper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-04 10:18:20.594184 faster-whisper-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-04-04 10:18:17.000000 faster-whisper-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:02:25.441650 faster-whisper-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-25 15:02:22.000000 faster-whisper-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-25 15:02:22.000000 faster-whisper-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9820 2023-04-25 15:02:25.441650 faster-whisper-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7474 2023-04-25 15:02:22.000000 faster-whisper-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:02:25.441650 faster-whisper-0.5.0/faster_whisper/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-25 15:02:22.000000 faster-whisper-0.5.0/faster_whisper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:02:25.441650 faster-whisper-0.5.0/faster_whisper/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)  1807524 2023-04-25 15:02:22.000000 faster-whisper-0.5.0/faster_whisper/assets/silero_vad.onnx
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-04-25 15:02:22.000000 faster-whisper-0.5.0/faster_whisper/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-04-25 15:02:22.000000 faster-whisper-0.5.0/faster_whisper/feature_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-04-25 15:02:22.000000 faster-whisper-0.5.0/faster_whisper/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33067 2023-04-25 15:02:22.000000 faster-whisper-0.5.0/faster_whisper/transcribe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-04-25 15:02:22.000000 faster-whisper-0.5.0/faster_whisper/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9840 2023-04-25 15:02:22.000000 faster-whisper-0.5.0/faster_whisper/vad.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:02:25.441650 faster-whisper-0.5.0/faster_whisper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9820 2023-04-25 15:02:25.000000 faster-whisper-0.5.0/faster_whisper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-25 15:02:25.000000 faster-whisper-0.5.0/faster_whisper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 15:02:25.000000 faster-whisper-0.5.0/faster_whisper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-25 15:02:25.000000 faster-whisper-0.5.0/faster_whisper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-25 15:02:25.000000 faster-whisper-0.5.0/faster_whisper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-25 15:02:25.441650 faster-whisper-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-04-25 15:02:22.000000 faster-whisper-0.5.0/setup.py
```

### Comparing `faster-whisper-0.4.1/LICENSE` & `faster-whisper-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `faster-whisper-0.4.1/PKG-INFO` & `faster-whisper-0.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faster-whisper
-Version: 0.4.1
+Version: 0.5.0
 Summary: Faster Whisper transcription with CTranslate2
 Home-page: https://github.com/guillaumekln/faster-whisper
 Author: Guillaume Klein
 License: MIT
 Description: [![CI](https://github.com/guillaumekln/faster-whisper/workflows/CI/badge.svg)](https://github.com/guillaumekln/faster-whisper/actions?query=workflow%3ACI) [![PyPI version](https://badge.fury.io/py/faster-whisper.svg)](https://badge.fury.io/py/faster-whisper)
         
         # Faster Whisper transcription with CTranslate2
@@ -67,16 +67,14 @@
         
         ### GPU support
         
         GPU execution requires the NVIDIA libraries cuBLAS 11.x and cuDNN 8.x to be installed on the system. Please refer to the [CTranslate2 documentation](https://opennmt.net/CTranslate2/installation.html).
         
         ## Usage
         
-        ### Library
-        
         ```python
         from faster_whisper import WhisperModel
         
         model_size = "large-v2"
         
         # Run on GPU with FP16
         model = WhisperModel(model_size, device="cuda", compute_type="float16")
@@ -90,45 +88,65 @@
         
         print("Detected language '%s' with probability %f" % (info.language, info.language_probability))
         
         for segment in segments:
             print("[%.2fs -> %.2fs] %s" % (segment.start, segment.end, segment.text))
         ```
         
-        #### Word-level timestamps
+        **Warning:** `segments` is a *generator* so the transcription only starts when you iterate over it. The transcription can be run to completion by gathering the segments in a list or a `for` loop:
+        
+        ```python
+        segments, _ = model.transcribe("audio.mp3")
+        segments = list(segments)  # The transcription will actually run here.
+        ```
+        
+        ### Word-level timestamps
         
         ```python
         segments, _ = model.transcribe("audio.mp3", word_timestamps=True)
         
         for segment in segments:
             for word in segment.words:
                 print("[%.2fs -> %.2fs] %s" % (word.start, word.end, word.word))
         ```
         
-        #### VAD filter
+        ### VAD filter
         
         The library integrates the [Silero VAD](https://github.com/snakers4/silero-vad) model to filter out parts of the audio without speech:
         
         ```python
         segments, _ = model.transcribe("audio.mp3", vad_filter=True)
         ```
         
         The default behavior is conservative and only removes silence longer than 2 seconds. See the available VAD parameters and default values in the function [`get_speech_timestamps`](https://github.com/guillaumekln/faster-whisper/blob/master/faster_whisper/vad.py). They can be customized with the dictionary argument `vad_parameters`:
         
         ```python
         segments, _ = model.transcribe("audio.mp3", vad_filter=True, vad_parameters=dict(min_silence_duration_ms=500))
         ```
         
-        #### Going further
+        ### Logging
+        
+        The library logging level can be configured like this:
+        
+        ```python
+        import logging
+        
+        logging.basicConfig()
+        logging.getLogger("faster_whisper").setLevel(logging.DEBUG)
+        ```
+        
+        ### Going further
         
         See more model and transcription options in the [`WhisperModel`](https://github.com/guillaumekln/faster-whisper/blob/master/faster_whisper/transcribe.py) class implementation.
         
-        ### CLI
+        ## Community integrations
+        
+        Here is a non exhaustive list of open-source projects using *faster-whisper*. Feel free to add your project to the list!
         
-        You can use [jordimas/whisper-ctranslate2](https://github.com/jordimas/whisper-ctranslate2) to access `faster-whisper` through a CLI interface similar to what is offered by Whisper.
+        * [whisper-ctranslate2](https://github.com/jordimas/whisper-ctranslate2) is a command line client based on `faster-whisper` and compatible with the original client from openai/whisper.
         
         ## Model conversion
         
         When loading a model from its size such as `WhisperModel("large-v2")`, the correspondig CTranslate2 model is automatically downloaded from the [Hugging Face Hub](https://huggingface.co/guillaumekln).
         
         We also provide a script to convert any Whisper models compatible with the Transformers library. They could be the original OpenAI models or user fine-tuned models.
```

### Comparing `faster-whisper-0.4.1/README.md` & `faster-whisper-0.5.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -60,16 +60,14 @@
 
 ### GPU support
 
 GPU execution requires the NVIDIA libraries cuBLAS 11.x and cuDNN 8.x to be installed on the system. Please refer to the [CTranslate2 documentation](https://opennmt.net/CTranslate2/installation.html).
 
 ## Usage
 
-### Library
-
 ```python
 from faster_whisper import WhisperModel
 
 model_size = "large-v2"
 
 # Run on GPU with FP16
 model = WhisperModel(model_size, device="cuda", compute_type="float16")
@@ -83,45 +81,65 @@
 
 print("Detected language '%s' with probability %f" % (info.language, info.language_probability))
 
 for segment in segments:
     print("[%.2fs -> %.2fs] %s" % (segment.start, segment.end, segment.text))
 ```
 
-#### Word-level timestamps
+**Warning:** `segments` is a *generator* so the transcription only starts when you iterate over it. The transcription can be run to completion by gathering the segments in a list or a `for` loop:
+
+```python
+segments, _ = model.transcribe("audio.mp3")
+segments = list(segments)  # The transcription will actually run here.
+```
+
+### Word-level timestamps
 
 ```python
 segments, _ = model.transcribe("audio.mp3", word_timestamps=True)
 
 for segment in segments:
     for word in segment.words:
         print("[%.2fs -> %.2fs] %s" % (word.start, word.end, word.word))
 ```
 
-#### VAD filter
+### VAD filter
 
 The library integrates the [Silero VAD](https://github.com/snakers4/silero-vad) model to filter out parts of the audio without speech:
 
 ```python
 segments, _ = model.transcribe("audio.mp3", vad_filter=True)
 ```
 
 The default behavior is conservative and only removes silence longer than 2 seconds. See the available VAD parameters and default values in the function [`get_speech_timestamps`](https://github.com/guillaumekln/faster-whisper/blob/master/faster_whisper/vad.py). They can be customized with the dictionary argument `vad_parameters`:
 
 ```python
 segments, _ = model.transcribe("audio.mp3", vad_filter=True, vad_parameters=dict(min_silence_duration_ms=500))
 ```
 
-#### Going further
+### Logging
+
+The library logging level can be configured like this:
+
+```python
+import logging
+
+logging.basicConfig()
+logging.getLogger("faster_whisper").setLevel(logging.DEBUG)
+```
+
+### Going further
 
 See more model and transcription options in the [`WhisperModel`](https://github.com/guillaumekln/faster-whisper/blob/master/faster_whisper/transcribe.py) class implementation.
 
-### CLI
+## Community integrations
+
+Here is a non exhaustive list of open-source projects using *faster-whisper*. Feel free to add your project to the list!
 
-You can use [jordimas/whisper-ctranslate2](https://github.com/jordimas/whisper-ctranslate2) to access `faster-whisper` through a CLI interface similar to what is offered by Whisper.
+* [whisper-ctranslate2](https://github.com/jordimas/whisper-ctranslate2) is a command line client based on `faster-whisper` and compatible with the original client from openai/whisper.
 
 ## Model conversion
 
 When loading a model from its size such as `WhisperModel("large-v2")`, the correspondig CTranslate2 model is automatically downloaded from the [Hugging Face Hub](https://huggingface.co/guillaumekln).
 
 We also provide a script to convert any Whisper models compatible with the Transformers library. They could be the original OpenAI models or user fine-tuned models.
```

### Comparing `faster-whisper-0.4.1/faster_whisper/assets/silero_vad.onnx` & `faster-whisper-0.5.0/faster_whisper/assets/silero_vad.onnx`

 * *Files identical despite different names*

### Comparing `faster-whisper-0.4.1/faster_whisper/audio.py` & `faster-whisper-0.5.0/faster_whisper/audio.py`

 * *Files identical despite different names*

### Comparing `faster-whisper-0.4.1/faster_whisper/feature_extractor.py` & `faster-whisper-0.5.0/faster_whisper/feature_extractor.py`

 * *Files identical despite different names*

### Comparing `faster-whisper-0.4.1/faster_whisper/tokenizer.py` & `faster-whisper-0.5.0/faster_whisper/tokenizer.py`

 * *Files identical despite different names*

### Comparing `faster-whisper-0.4.1/faster_whisper/transcribe.py` & `faster-whisper-0.5.0/faster_whisper/transcribe.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import itertools
+import logging
 import os
 import zlib
 
 from typing import BinaryIO, Iterable, List, NamedTuple, Optional, Tuple, Union
 
 import ctranslate2
 import numpy as np
 import tokenizers
 
 from faster_whisper.audio import decode_audio
 from faster_whisper.feature_extractor import FeatureExtractor
 from faster_whisper.tokenizer import Tokenizer
-from faster_whisper.utils import download_model
+from faster_whisper.utils import download_model, format_timestamp, get_logger
 from faster_whisper.vad import (
     SpeechTimestampsMap,
     collect_chunks,
     get_speech_timestamps,
 )
 
 
@@ -23,26 +24,25 @@
     start: float
     end: float
     word: str
     probability: float
 
 
 class Segment(NamedTuple):
+    id: int
+    seek: int
     start: float
     end: float
     text: str
-    words: Optional[List[Word]]
-    avg_log_prob: float
+    tokens: List[int]
+    temperature: float
+    avg_logprob: float
+    compression_ratio: float
     no_speech_prob: float
-
-
-class AudioInfo(NamedTuple):
-    language: str
-    language_probability: float
-    duration: float
+    words: Optional[List[Word]]
 
 
 class TranscriptionOptions(NamedTuple):
     beam_size: int
     best_of: int
     patience: float
     length_penalty: float
@@ -58,23 +58,32 @@
     without_timestamps: bool
     max_initial_timestamp: float
     word_timestamps: bool
     prepend_punctuations: str
     append_punctuations: str
 
 
+class TranscriptionInfo(NamedTuple):
+    language: str
+    language_probability: float
+    duration: float
+    transcription_options: TranscriptionOptions
+
+
 class WhisperModel:
     def __init__(
         self,
         model_size_or_path: str,
         device: str = "auto",
         device_index: Union[int, List[int]] = 0,
         compute_type: str = "default",
         cpu_threads: int = 0,
         num_workers: int = 1,
+        download_root: Optional[str] = None,
+        local_files_only: Optional[bool] = False,
     ):
         """Initializes the Whisper model.
 
         Args:
           model_size_or_path: Size of the model to use (tiny, tiny.en, base, base.en,
             small, small.en, medium, medium.en, large-v1, or large-v2) or a path to a converted
             model directory. When a size is configured, the converted model is downloaded
@@ -88,19 +97,27 @@
             See https://opennmt.net/CTranslate2/quantization.html.
           cpu_threads: Number of threads to use when running on CPU (4 by default).
             A non zero value overrides the OMP_NUM_THREADS environment variable.
           num_workers: When transcribe() is called from multiple Python threads,
             having multiple workers enables true parallelism when running the model
             (concurrent calls to self.model.generate() will run in parallel).
             This can improve the global throughput at the cost of increased memory usage.
+          download_root: Directory where the model should be saved. If not set, the model
+            is saved in the standard Hugging Face cache directory.
+          local_files_only:  If True, avoid downloading the file and return the path to the
+            local cached file if it exists.
         """
+        self.logger = get_logger()
+
         if os.path.isdir(model_size_or_path):
             model_path = model_size_or_path
         else:
-            model_path = download_model(model_size_or_path)
+            model_path = download_model(
+                model_size_or_path, download_root, local_files_only
+            )
 
         self.model = ctranslate2.models.Whisper(
             model_path,
             device=device,
             device_index=device_index,
             compute_type=compute_type,
             intra_threads=cpu_threads,
@@ -155,15 +172,15 @@
         without_timestamps: bool = False,
         max_initial_timestamp: float = 1.0,
         word_timestamps: bool = False,
         prepend_punctuations: str = "\"'“¿([{-",
         append_punctuations: str = "\"'.。,，!！?？:：”)]}、",
         vad_filter: bool = False,
         vad_parameters: Optional[dict] = None,
-    ) -> Tuple[Iterable[Segment], AudioInfo]:
+    ) -> Tuple[Iterable[Segment], TranscriptionInfo]:
         """Transcribes an input file.
 
         Arguments:
           audio: Path to the input file (or a file-like object), or the audio waveform.
           language: The language spoken in the audio. It should be a language code such
             as "en" or "fr". If not set, the language will be detected in the first 30 seconds
             of audio.
@@ -205,27 +222,50 @@
           vad_parameters: Dictionary of Silero VAD parameters (see available parameters and
             default values in the function `get_speech_timestamps`).
 
         Returns:
           A tuple with:
 
             - a generator over transcribed segments
-            - an instance of AudioInfo
+            - an instance of TranscriptionInfo
         """
+        sampling_rate = self.feature_extractor.sampling_rate
+
         if not isinstance(audio, np.ndarray):
-            audio = decode_audio(
-                audio, sampling_rate=self.feature_extractor.sampling_rate
-            )
+            audio = decode_audio(audio, sampling_rate=sampling_rate)
 
-        duration = audio.shape[0] / self.feature_extractor.sampling_rate
+        duration = audio.shape[0] / sampling_rate
+
+        self.logger.info(
+            "Processing audio with duration %s", format_timestamp(duration)
+        )
 
         if vad_filter:
             vad_parameters = {} if vad_parameters is None else vad_parameters
             speech_chunks = get_speech_timestamps(audio, **vad_parameters)
             audio = collect_chunks(audio, speech_chunks)
+
+            self.logger.info(
+                "VAD filter removed %s of audio",
+                format_timestamp(duration - (audio.shape[0] / sampling_rate)),
+            )
+
+            if self.logger.isEnabledFor(logging.DEBUG):
+                self.logger.debug(
+                    "VAD filter kept the following audio segments: %s",
+                    ", ".join(
+                        "[%s -> %s]"
+                        % (
+                            format_timestamp(chunk["start"] / sampling_rate),
+                            format_timestamp(chunk["end"] / sampling_rate),
+                        )
+                        for chunk in speech_chunks
+                    ),
+                )
+
         else:
             speech_chunks = None
 
         features = self.feature_extractor(audio)
 
         encoder_output = None
 
@@ -235,14 +275,20 @@
                 language_probability = 1
             else:
                 segment = features[:, : self.feature_extractor.nb_max_frames]
                 encoder_output = self.encode(segment)
                 results = self.model.detect_language(encoder_output)
                 language_token, language_probability = results[0][0]
                 language = language_token[2:-2]
+
+                self.logger.info(
+                    "Detected language '%s' with probability %.2f",
+                    language,
+                    language_probability,
+                )
         else:
             language_probability = 1
 
         tokenizer = Tokenizer(
             self.hf_tokenizer,
             self.model.is_multilingual,
             task=task,
@@ -271,34 +317,34 @@
             prepend_punctuations=prepend_punctuations,
             append_punctuations=append_punctuations,
         )
 
         segments = self.generate_segments(features, tokenizer, options, encoder_output)
 
         if speech_chunks:
-            segments = restore_speech_timestamps(
-                segments, speech_chunks, self.feature_extractor.sampling_rate
-            )
+            segments = restore_speech_timestamps(segments, speech_chunks, sampling_rate)
 
-        audio_info = AudioInfo(
+        info = TranscriptionInfo(
             language=language,
             language_probability=language_probability,
             duration=duration,
+            transcription_options=options,
         )
 
-        return segments, audio_info
+        return segments, info
 
     def generate_segments(
         self,
         features: np.ndarray,
         tokenizer: Tokenizer,
         options: TranscriptionOptions,
         encoder_output: Optional[ctranslate2.StorageView] = None,
     ) -> Iterable[Segment]:
         content_frames = features.shape[-1] - self.feature_extractor.nb_max_frames
+        idx = 0
         seek = 0
         all_tokens = []
         prompt_reset_since = 0
 
         if options.initial_prompt is not None:
             initial_prompt = " " + options.initial_prompt.strip()
             initial_prompt_tokens = tokenizer.encode(initial_prompt)
@@ -308,41 +354,55 @@
             time_offset = seek * self.feature_extractor.time_per_frame
             segment = features[:, seek : seek + self.feature_extractor.nb_max_frames]
             segment_size = min(
                 self.feature_extractor.nb_max_frames, content_frames - seek
             )
             segment_duration = segment_size * self.feature_extractor.time_per_frame
 
+            if self.logger.isEnabledFor(logging.DEBUG):
+                self.logger.debug(
+                    "Processing segment at %s", format_timestamp(time_offset)
+                )
+
             previous_tokens = all_tokens[prompt_reset_since:]
             prompt = self.get_prompt(
                 tokenizer,
                 previous_tokens,
                 without_timestamps=options.without_timestamps,
                 prefix=options.prefix if seek == 0 else None,
             )
 
             if encoder_output is None:
                 encoder_output = self.encode(segment)
 
-            result, avg_log_prob, temperature = self.generate_with_fallback(
-                encoder_output, prompt, tokenizer, options
-            )
+            (
+                result,
+                avg_logprob,
+                temperature,
+                compression_ratio,
+            ) = self.generate_with_fallback(encoder_output, prompt, tokenizer, options)
 
             if options.no_speech_threshold is not None:
                 # no voice activity check
                 should_skip = result.no_speech_prob > options.no_speech_threshold
 
                 if (
                     options.log_prob_threshold is not None
-                    and avg_log_prob > options.log_prob_threshold
+                    and avg_logprob > options.log_prob_threshold
                 ):
                     # don't skip if the logprob is high enough, despite the no_speech_prob
                     should_skip = False
 
                 if should_skip:
+                    self.logger.debug(
+                        "No speech threshold is met (%f > %f)",
+                        result.no_speech_prob,
+                        options.no_speech_threshold,
+                    )
+
                     # fast-forward to the next segment boundary
                     seek += segment_size
                     continue
 
             tokens = result.sequences_ids[0]
 
             previous_seek = seek
@@ -419,17 +479,14 @@
                         end=time_offset + duration,
                         tokens=tokens,
                     )
                 )
 
                 seek += segment_size
 
-            if not options.condition_on_previous_text or temperature > 0.5:
-                prompt_reset_since = len(all_tokens)
-
             if options.word_timestamps:
                 self.add_word_timestamps(
                     current_segments,
                     tokenizer,
                     encoder_output,
                     segment_size,
                     options.prepend_punctuations,
@@ -454,28 +511,37 @@
                 tokens = segment["tokens"]
                 text = tokenizer.decode(tokens)
 
                 if segment["start"] == segment["end"] or not text.strip():
                     continue
 
                 all_tokens.extend(tokens)
+                idx += 1
 
                 yield Segment(
+                    id=idx,
+                    seek=seek,
                     start=segment["start"],
                     end=segment["end"],
                     text=text,
+                    tokens=tokens,
+                    temperature=temperature,
+                    avg_logprob=avg_logprob,
+                    compression_ratio=compression_ratio,
+                    no_speech_prob=result.no_speech_prob,
                     words=(
                         [Word(**word) for word in segment["words"]]
                         if options.word_timestamps
                         else None
                     ),
-                    avg_log_prob=avg_log_prob,
-                    no_speech_prob=result.no_speech_prob,
                 )
 
+            if not options.condition_on_previous_text or temperature > 0.5:
+                prompt_reset_since = len(all_tokens)
+
     def encode(self, features: np.ndarray) -> ctranslate2.StorageView:
         # When the model is running on multiple GPUs, the encoder output should be moved
         # to the CPU since we don't know which GPU will handle the next job.
         to_cpu = self.model.device == "cuda" and len(self.model.device_index) > 1
 
         features = np.expand_dims(features, 0)
         features = get_ctranslate2_storage(features)
@@ -484,18 +550,19 @@
 
     def generate_with_fallback(
         self,
         encoder_output: ctranslate2.StorageView,
         prompt: List[int],
         tokenizer: Tokenizer,
         options: TranscriptionOptions,
-    ) -> Tuple[ctranslate2.models.WhisperGenerationResult, float, float]:
+    ) -> Tuple[ctranslate2.models.WhisperGenerationResult, float, float, float]:
         result = None
-        avg_log_prob = None
+        avg_logprob = None
         final_temperature = None
+        compression_ratio = None
 
         max_initial_timestamp_index = int(
             round(options.max_initial_timestamp / self.time_precision)
         )
 
         for temperature in options.temperatures:
             if temperature > 0:
@@ -525,38 +592,52 @@
                 **kwargs,
             )[0]
 
             tokens = result.sequences_ids[0]
 
             # Recover the average log prob from the returned score.
             seq_len = len(tokens)
-            cum_log_prob = result.scores[0] * (seq_len**options.length_penalty)
-            avg_log_prob = cum_log_prob / (seq_len + 1)
+            cum_logprob = result.scores[0] * (seq_len**options.length_penalty)
+            avg_logprob = cum_logprob / (seq_len + 1)
 
             text = tokenizer.decode(tokens).strip()
             compression_ratio = get_compression_ratio(text)
 
             needs_fallback = False
 
             if (
                 options.compression_ratio_threshold is not None
                 and compression_ratio > options.compression_ratio_threshold
             ):
                 needs_fallback = True  # too repetitive
 
+                self.logger.debug(
+                    "Compression ratio threshold is not met with temperature %.1f (%f > %f)",
+                    temperature,
+                    compression_ratio,
+                    options.compression_ratio_threshold,
+                )
+
             if (
                 options.log_prob_threshold is not None
-                and avg_log_prob < options.log_prob_threshold
+                and avg_logprob < options.log_prob_threshold
             ):
                 needs_fallback = True  # average log probability is too low
 
+                self.logger.debug(
+                    "Log probability threshold is not met with temperature %.1f (%f < %f)",
+                    temperature,
+                    avg_logprob,
+                    options.log_prob_threshold,
+                )
+
             if not needs_fallback:
                 break
 
-        return result, avg_log_prob, final_temperature
+        return result, avg_logprob, final_temperature, compression_ratio
 
     def get_prompt(
         self,
         tokenizer: Tokenizer,
         previous_tokens: List[int],
         without_timestamps: bool = False,
         prefix: Optional[str] = None,
@@ -711,28 +792,33 @@
     ts_map = SpeechTimestampsMap(speech_chunks, sampling_rate)
 
     for segment in segments:
         if segment.words:
             words = []
             for word in segment.words:
                 # Ensure the word start and end times are resolved to the same chunk.
-                chunk_index = ts_map.get_chunk_index(word.start)
+                middle = (word.start + word.end) / 2
+                chunk_index = ts_map.get_chunk_index(middle)
                 word = word._replace(
                     start=ts_map.get_original_time(word.start, chunk_index),
                     end=ts_map.get_original_time(word.end, chunk_index),
                 )
                 words.append(word)
-        else:
-            words = segment.words
 
-        segment = segment._replace(
-            start=ts_map.get_original_time(segment.start),
-            end=ts_map.get_original_time(segment.end),
-            words=words,
-        )
+            segment = segment._replace(
+                start=words[0].start,
+                end=words[-1].end,
+                words=words,
+            )
+
+        else:
+            segment = segment._replace(
+                start=ts_map.get_original_time(segment.start),
+                end=ts_map.get_original_time(segment.end),
+            )
 
         yield segment
 
 
 def get_ctranslate2_storage(segment: np.ndarray) -> ctranslate2.StorageView:
     segment = np.ascontiguousarray(segment)
     segment = ctranslate2.StorageView.from_array(segment)
```

### Comparing `faster-whisper-0.4.1/faster_whisper/utils.py` & `faster-whisper-0.5.0/faster_whisper/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 import os
 
 from typing import Optional
 
 import huggingface_hub
 
 from tqdm.auto import tqdm
@@ -21,39 +22,50 @@
 
 
 def get_assets_path():
     """Returns the path to the assets directory."""
     return os.path.join(os.path.dirname(os.path.abspath(__file__)), "assets")
 
 
-def download_model(size: str, output_dir: Optional[str] = None):
+def get_logger():
+    """Returns the module logger."""
+    return logging.getLogger("faster_whisper")
+
+
+def download_model(
+    size: str,
+    output_dir: Optional[str] = None,
+    local_files_only: Optional[bool] = False,
+):
     """Downloads a CTranslate2 Whisper model from the Hugging Face Hub.
 
     The model is downloaded from https://huggingface.co/guillaumekln.
 
     Args:
       size: Size of the model to download (tiny, tiny.en, base, base.en, small, small.en,
         medium, medium.en, large-v1, or large-v2).
       output_dir: Directory where the model should be saved. If not set, the model is saved in
         the standard Hugging Face cache directory.
+      local_files_only:  If True, avoid downloading the file and return the path to the local
+        cached file if it exists.
 
     Returns:
       The path to the downloaded model.
 
     Raises:
       ValueError: if the model size is invalid.
     """
     if size not in _MODELS:
         raise ValueError(
             "Invalid model size '%s', expected one of: %s" % (size, ", ".join(_MODELS))
         )
 
     repo_id = "guillaumekln/faster-whisper-%s" % size
     kwargs = {}
-
+    kwargs["local_files_only"] = local_files_only
     if output_dir is not None:
         kwargs["local_dir"] = output_dir
         kwargs["local_dir_use_symlinks"] = False
 
     allow_patterns = [
         "config.json",
         "model.bin",
```

### Comparing `faster-whisper-0.4.1/faster_whisper/vad.py` & `faster-whisper-0.5.0/faster_whisper/vad.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     audio: np.ndarray,
     *,
     threshold: float = 0.5,
     min_speech_duration_ms: int = 250,
     max_speech_duration_s: float = float("inf"),
     min_silence_duration_ms: int = 2000,
     window_size_samples: int = 1024,
-    speech_pad_ms: int = 200,
+    speech_pad_ms: int = 400,
 ) -> List[dict]:
     """This method is used for splitting long audios into speech chunks using silero VAD.
 
     Args:
       audio: One dimensional float array.
       threshold: Speech threshold. Silero VAD outputs speech probabilities for each audio chunk,
         probabilities ABOVE this value are considered as SPEECH. It is better to tune this
```

### Comparing `faster-whisper-0.4.1/faster_whisper.egg-info/PKG-INFO` & `faster-whisper-0.5.0/faster_whisper.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faster-whisper
-Version: 0.4.1
+Version: 0.5.0
 Summary: Faster Whisper transcription with CTranslate2
 Home-page: https://github.com/guillaumekln/faster-whisper
 Author: Guillaume Klein
 License: MIT
 Description: [![CI](https://github.com/guillaumekln/faster-whisper/workflows/CI/badge.svg)](https://github.com/guillaumekln/faster-whisper/actions?query=workflow%3ACI) [![PyPI version](https://badge.fury.io/py/faster-whisper.svg)](https://badge.fury.io/py/faster-whisper)
         
         # Faster Whisper transcription with CTranslate2
@@ -67,16 +67,14 @@
         
         ### GPU support
         
         GPU execution requires the NVIDIA libraries cuBLAS 11.x and cuDNN 8.x to be installed on the system. Please refer to the [CTranslate2 documentation](https://opennmt.net/CTranslate2/installation.html).
         
         ## Usage
         
-        ### Library
-        
         ```python
         from faster_whisper import WhisperModel
         
         model_size = "large-v2"
         
         # Run on GPU with FP16
         model = WhisperModel(model_size, device="cuda", compute_type="float16")
@@ -90,45 +88,65 @@
         
         print("Detected language '%s' with probability %f" % (info.language, info.language_probability))
         
         for segment in segments:
             print("[%.2fs -> %.2fs] %s" % (segment.start, segment.end, segment.text))
         ```
         
-        #### Word-level timestamps
+        **Warning:** `segments` is a *generator* so the transcription only starts when you iterate over it. The transcription can be run to completion by gathering the segments in a list or a `for` loop:
+        
+        ```python
+        segments, _ = model.transcribe("audio.mp3")
+        segments = list(segments)  # The transcription will actually run here.
+        ```
+        
+        ### Word-level timestamps
         
         ```python
         segments, _ = model.transcribe("audio.mp3", word_timestamps=True)
         
         for segment in segments:
             for word in segment.words:
                 print("[%.2fs -> %.2fs] %s" % (word.start, word.end, word.word))
         ```
         
-        #### VAD filter
+        ### VAD filter
         
         The library integrates the [Silero VAD](https://github.com/snakers4/silero-vad) model to filter out parts of the audio without speech:
         
         ```python
         segments, _ = model.transcribe("audio.mp3", vad_filter=True)
         ```
         
         The default behavior is conservative and only removes silence longer than 2 seconds. See the available VAD parameters and default values in the function [`get_speech_timestamps`](https://github.com/guillaumekln/faster-whisper/blob/master/faster_whisper/vad.py). They can be customized with the dictionary argument `vad_parameters`:
         
         ```python
         segments, _ = model.transcribe("audio.mp3", vad_filter=True, vad_parameters=dict(min_silence_duration_ms=500))
         ```
         
-        #### Going further
+        ### Logging
+        
+        The library logging level can be configured like this:
+        
+        ```python
+        import logging
+        
+        logging.basicConfig()
+        logging.getLogger("faster_whisper").setLevel(logging.DEBUG)
+        ```
+        
+        ### Going further
         
         See more model and transcription options in the [`WhisperModel`](https://github.com/guillaumekln/faster-whisper/blob/master/faster_whisper/transcribe.py) class implementation.
         
-        ### CLI
+        ## Community integrations
+        
+        Here is a non exhaustive list of open-source projects using *faster-whisper*. Feel free to add your project to the list!
         
-        You can use [jordimas/whisper-ctranslate2](https://github.com/jordimas/whisper-ctranslate2) to access `faster-whisper` through a CLI interface similar to what is offered by Whisper.
+        * [whisper-ctranslate2](https://github.com/jordimas/whisper-ctranslate2) is a command line client based on `faster-whisper` and compatible with the original client from openai/whisper.
         
         ## Model conversion
         
         When loading a model from its size such as `WhisperModel("large-v2")`, the correspondig CTranslate2 model is automatically downloaded from the [Hugging Face Hub](https://huggingface.co/guillaumekln).
         
         We also provide a script to convert any Whisper models compatible with the Transformers library. They could be the original OpenAI models or user fine-tuned models.
```

### Comparing `faster-whisper-0.4.1/setup.py` & `faster-whisper-0.5.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 install_requires = get_requirements(os.path.join(base_dir, "requirements.txt"))
 conversion_requires = get_requirements(
     os.path.join(base_dir, "requirements.conversion.txt")
 )
 
 setup(
     name="faster-whisper",
-    version="0.4.1",
+    version="0.5.0",
     license="MIT",
     description="Faster Whisper transcription with CTranslate2",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     author="Guillaume Klein",
     url="https://github.com/guillaumekln/faster-whisper",
     classifiers=[
```

