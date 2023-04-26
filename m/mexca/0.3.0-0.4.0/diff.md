# Comparing `tmp/mexca-0.3.0.tar.gz` & `tmp/mexca-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mexca-0.3.0.tar", last modified: Wed Apr  5 14:07:31 2023, max compression
+gzip compressed data, was "mexca-0.4.0.tar", last modified: Wed Apr 26 15:06:49 2023, max compression
```

## Comparing `mexca-0.3.0.tar` & `mexca-0.4.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:07:31.519878 mexca-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-05 14:06:54.000000 mexca-0.3.0/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-04-05 14:06:54.000000 mexca-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-05 14:06:54.000000 mexca-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-05 14:06:54.000000 mexca-0.3.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     9902 2023-04-05 14:07:31.519878 mexca-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8943 2023-04-05 14:06:54.000000 mexca-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:07:31.511878 mexca-0.3.0/mexca/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-05 14:06:54.000000 mexca-0.3.0/mexca/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:07:31.515879 mexca-0.3.0/mexca/audio/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-05 14:06:54.000000 mexca-0.3.0/mexca/audio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11512 2023-04-05 14:06:54.000000 mexca-0.3.0/mexca/audio/extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)    47780 2023-04-05 14:06:54.000000 mexca-0.3.0/mexca/audio/features.py
--rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-04-05 14:06:54.000000 mexca-0.3.0/mexca/audio/identification.py
--rw-r--r--   0 runner    (1001) docker     (123)    11088 2023-04-05 14:06:54.000000 mexca-0.3.0/mexca/container.py
--rw-r--r--   0 runner    (1001) docker     (123)    21097 2023-04-05 14:06:54.000000 mexca-0.3.0/mexca/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     9526 2023-04-05 14:06:54.000000 mexca-0.3.0/mexca/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:07:31.515879 mexca-0.3.0/mexca/text/
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-05 14:06:54.000000 mexca-0.3.0/mexca/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-04-05 14:06:54.000000 mexca-0.3.0/mexca/text/sentiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     9655 2023-04-05 14:06:54.000000 mexca-0.3.0/mexca/text/transcription.py
--rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-04-05 14:06:54.000000 mexca-0.3.0/mexca/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    27922 2023-04-05 14:06:54.000000 mexca-0.3.0/mexca/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:07:31.515879 mexca-0.3.0/mexca.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9902 2023-04-05 14:07:31.000000 mexca-0.3.0/mexca.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-05 14:07:31.000000 mexca-0.3.0/mexca.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 14:07:31.000000 mexca-0.3.0/mexca.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-05 14:07:31.000000 mexca-0.3.0/mexca.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 14:07:02.000000 mexca-0.3.0/mexca.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-04-05 14:07:31.000000 mexca-0.3.0/mexca.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-05 14:07:31.000000 mexca-0.3.0/mexca.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-05 14:06:54.000000 mexca-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-04-05 14:07:31.519878 mexca-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-05 14:06:54.000000 mexca-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:07:31.519878 mexca-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-04-05 14:06:54.000000 mexca-0.3.0/tests/test_audio_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)    10623 2023-04-05 14:06:54.000000 mexca-0.3.0/tests/test_audio_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-04-05 14:06:54.000000 mexca-0.3.0/tests/test_audio_identification.py
--rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-04-05 14:06:54.000000 mexca-0.3.0/tests/test_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     8782 2023-04-05 14:06:54.000000 mexca-0.3.0/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-04-05 14:06:54.000000 mexca-0.3.0/tests/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-04-05 14:06:54.000000 mexca-0.3.0/tests/test_text_sentiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-04-05 14:06:54.000000 mexca-0.3.0/tests/test_text_transcription.py
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-04-05 14:06:54.000000 mexca-0.3.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8880 2023-04-05 14:06:54.000000 mexca-0.3.0/tests/test_video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:06:49.101131 mexca-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-26 15:06:04.000000 mexca-0.4.0/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-04-26 15:06:04.000000 mexca-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-26 15:06:04.000000 mexca-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-26 15:06:04.000000 mexca-0.4.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     9997 2023-04-26 15:06:49.101131 mexca-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8987 2023-04-26 15:06:04.000000 mexca-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:06:49.081131 mexca-0.4.0/mexca/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-26 15:06:04.000000 mexca-0.4.0/mexca/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:06:49.085131 mexca-0.4.0/mexca/audio/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-26 15:06:04.000000 mexca-0.4.0/mexca/audio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23559 2023-04-26 15:06:04.000000 mexca-0.4.0/mexca/audio/extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67298 2023-04-26 15:06:04.000000 mexca-0.4.0/mexca/audio/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-04-26 15:06:04.000000 mexca-0.4.0/mexca/audio/identification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11966 2023-04-26 15:06:04.000000 mexca-0.4.0/mexca/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28611 2023-04-26 15:06:04.000000 mexca-0.4.0/mexca/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9526 2023-04-26 15:06:04.000000 mexca-0.4.0/mexca/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:06:49.085131 mexca-0.4.0/mexca/text/
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-26 15:06:04.000000 mexca-0.4.0/mexca/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-04-26 15:06:04.000000 mexca-0.4.0/mexca/text/sentiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9655 2023-04-26 15:06:04.000000 mexca-0.4.0/mexca/text/transcription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7811 2023-04-26 15:06:04.000000 mexca-0.4.0/mexca/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28529 2023-04-26 15:06:04.000000 mexca-0.4.0/mexca/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:06:49.081131 mexca-0.4.0/mexca.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9997 2023-04-26 15:06:49.000000 mexca-0.4.0/mexca.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-26 15:06:49.000000 mexca-0.4.0/mexca.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 15:06:49.000000 mexca-0.4.0/mexca.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-26 15:06:49.000000 mexca-0.4.0/mexca.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 15:06:17.000000 mexca-0.4.0/mexca.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-26 15:06:49.000000 mexca-0.4.0/mexca.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-26 15:06:49.000000 mexca-0.4.0/mexca.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-26 15:06:04.000000 mexca-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-04-26 15:06:49.101131 mexca-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-26 15:06:04.000000 mexca-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:06:49.101131 mexca-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-26 15:06:04.000000 mexca-0.4.0/tests/test_audio_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15766 2023-04-26 15:06:04.000000 mexca-0.4.0/tests/test_audio_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-04-26 15:06:04.000000 mexca-0.4.0/tests/test_audio_identification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-04-26 15:06:04.000000 mexca-0.4.0/tests/test_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8782 2023-04-26 15:06:04.000000 mexca-0.4.0/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-04-26 15:06:04.000000 mexca-0.4.0/tests/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-04-26 15:06:04.000000 mexca-0.4.0/tests/test_text_sentiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-04-26 15:06:04.000000 mexca-0.4.0/tests/test_text_transcription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-04-26 15:06:04.000000 mexca-0.4.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8880 2023-04-26 15:06:04.000000 mexca-0.4.0/tests/test_video.py
```

### Comparing `mexca-0.3.0/CITATION.cff` & `mexca-0.4.0/CITATION.cff`

 * *Files 15% similar despite different names*

```diff
@@ -13,17 +13,17 @@
     orcid: "https://orcid.org/0000-0002-1330-0585"
   - family-names: Pipal
     given-names: Christian
     orcid: "https://orcid.org/0000-0002-5395-2035"
   - family-names: Schumacher
     given-names: Gijs
     orcid: "https://orcid.org/0000-0002-6503-4514"
-date-released: 2023-04-05
+date-released: 2023-04-26
 doi: 10.5281/zenodo.6976414
-version: "0.3.0"
+version: "0.4.0"
 repository-code: "https://github.com/mexca/mexca"
 keywords:
   - emotion
   - multimodal
   - expression
 message: "If you use this software, please cite it using these metadata."
 license: Apache-2.0
```

### Comparing `mexca-0.3.0/LICENSE` & `mexca-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mexca-0.3.0/PKG-INFO` & `mexca-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: mexca
-Version: 0.3.0
+Version: 0.4.0
 Summary: Emotion expression capture from multiple modalities.
 Home-page: https://github.com/mexca/mexca
 Author: Malte Luken
 Author-email: m.luken@esciencecenter.nl
 Project-URL: Bug Tracker, https://github.com/mexca/mexca/issues
 Keywords: emotion,multimodal,expression
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Python: <3.10,>=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: vid
 Provides-Extra: spe
 Provides-Extra: voi
 Provides-Extra: tra
 Provides-Extra: sen
@@ -101,14 +102,20 @@
 
 The dependencies for the additional components can be installed via:
 
 ```console
 pip install mexca[vid,spe,voi,tra,sen]
 ```
 
+or:
+
+```console
+pip install mexca[all]
+```
+
 The abbreviations indicate:
 
 * `vid`: FaceExtractor
 * `spe`: SpeakerIdentifier
 * `voi`: VoiceExtractor
 * `tra`: AudioTranscriber
 * `sen`: SentimentExtractor
```

### Comparing `mexca-0.3.0/README.md` & `mexca-0.4.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -71,14 +71,20 @@
 
 The dependencies for the additional components can be installed via:
 
 ```console
 pip install mexca[vid,spe,voi,tra,sen]
 ```
 
+or:
+
+```console
+pip install mexca[all]
+```
+
 The abbreviations indicate:
 
 * `vid`: FaceExtractor
 * `spe`: SpeakerIdentifier
 * `voi`: VoiceExtractor
 * `tra`: AudioTranscriber
 * `sen`: SentimentExtractor
```

### Comparing `mexca-0.3.0/mexca/audio/features.py` & `mexca-0.4.0/mexca/audio/features.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from copy import copy
 from typing import List, Optional, Tuple, Union
 import librosa
 import numpy as np
 from scipy.interpolate import interp1d
 from scipy.signal import find_peaks
 from scipy.signal.windows import get_window
+from sklearn.linear_model import LinearRegression
 from mexca.utils import ClassInitMessage
 
 
 class BaseSignal:
     """Store a signal.
 
     Parameters
@@ -100,14 +101,54 @@
         mono: bool, default=True
             Whether to convert the signal to mono.
         """
         sig, nat_sr = librosa.load(path=filename, sr=sr, mono=mono)
         return cls(sig, nat_sr, mono, filename)
 
 
+class FormantAudioSignal(AudioSignal):
+    def __init__(
+        self,
+        sig: np.ndarray,
+        sr: int,
+        mono: bool,
+        filename: Optional[str],
+        preemphasis_from: Optional[float],
+    ):
+        self.preemphasis_from = preemphasis_from
+        super().__init__(sig, sr, mono, filename)
+
+    @staticmethod
+    def _calc_preemphasis_coef(preemphasis_from: float, sr: float) -> float:
+        return math.exp(-2 * math.pi * preemphasis_from * (1 / sr))
+
+    @classmethod
+    def from_audio_signal(
+        cls, audio_sig_obj: AudioSignal, preemphasis_from: Optional[float] = 50.0
+    ):
+        sig = audio_sig_obj.sig
+
+        if preemphasis_from is not None:
+            pre_coef = cls._calc_preemphasis_coef(preemphasis_from, audio_sig_obj.sr)
+            sig = librosa.effects.preemphasis(sig, coef=pre_coef)
+
+        return cls(
+            sig,
+            audio_sig_obj.sr,
+            audio_sig_obj.mono,
+            audio_sig_obj.filename,
+            preemphasis_from,
+        )
+
+    @staticmethod
+    def _preemphasize(sig: np.ndarray, sr: float, preemphasis_from: float):
+        pre_coef = math.exp(-2 * math.pi * preemphasis_from * (1 / sr))
+        return librosa.effects.preemphasis(sig, coef=pre_coef)
+
+
 class BaseFrames:
     """Create and store signal frames.
 
     A frame is an (overlapping, padded) slice of a signal for which higher-order
     features can be computed.
 
     Parameters
@@ -332,15 +373,15 @@
 class SpecFrames(BaseFrames):
     """Create and store spectrogram frames.
 
     Computes a spectrogram of a signal using the short-time Fourier transform (STFT).
 
     Parameters
     ----------
-    frames: np.ndarray
+    frames: numpy.ndarray
         Spectrogram frames.
     window: str
         The window that was applied before the STFT.
 
     Notes
     -----
     Frames contain complex arrays `x` where ``np.abs(x)`` is the magnitude and
@@ -360,26 +401,33 @@
         frame_len: int,
         hop_len: int,
         center: bool = True,
         pad_mode: str = "constant",
     ) -> None:
         self.logger = logging.getLogger("mexca.audio.extraction.SpecFrames")
         self.window = window
+        self._freqs = None
         super().__init__(frames, sr, frame_len, hop_len, center, pad_mode)
         self.logger.debug(ClassInitMessage())
 
+    @property
+    def freqs(self):
+        if self._freqs is None:
+            self._freqs = librosa.fft_frequencies(sr=self.sr, n_fft=self.frame_len)
+        return self._freqs
+
     @classmethod
     def from_signal(
         cls,
         sig_obj: BaseSignal,
         frame_len: int,
         hop_len: Optional[int] = None,
         center: bool = True,
         pad_mode: str = "constant",
-        window: Union[str, float, Tuple] = "hamming",
+        window: Union[str, float, Tuple] = "hann",
     ):
         """Transform a signal into spectrogram frames.
 
         Parameters
         ----------
         sig_obj: BaseSignal
             Signal object.
@@ -462,15 +510,15 @@
         hop_len: int,
         center: bool = True,
         pad_mode: str = "constant",
         max_formants: int = 5,
         lower: float = 50.0,
         upper: float = 5450.0,
         preemphasis_from: Optional[float] = 50.0,
-        window: Optional[Union[str, float, Tuple]] = "praat_gaussian"
+        window: Optional[Union[str, float, Tuple]] = "praat_gaussian",
     ) -> None:
         self.logger = logging.getLogger("mexca.audio.extraction.FormantFrames")
         self.max_formants = max_formants
         self.lower = lower
         self.upper = upper
         self.preemphasis_from = preemphasis_from
         self.window = window
@@ -478,52 +526,52 @@
         self.logger.debug(ClassInitMessage())
 
     @property
     def idx(self) -> np.ndarray:
         if self._idx is None:
             self._idx = np.arange(len(self.frames))
         return self._idx
-    
 
     @staticmethod
     def _praat_gauss_window(frame_len: int):
         # This is the Gaussian window that is used in Praat for formant estimation
         # See: https://github.com/YannickJadoul/Parselmouth/blob/master/praat/fon/Sound_to_Formant.cpp
-        sample_idx = np.arange(frame_len)+1
+        sample_idx = np.arange(frame_len) + 1
         idx_mid = 0.5 * (frame_len + 1)
         edge = np.exp(-12.0)
-        return (np.exp(-48.0 * (sample_idx - idx_mid)**2 / (frame_len)**2) - edge) / (1.0 - edge)
-
+        return (
+            np.exp(-48.0 * (sample_idx - idx_mid) ** 2 / (frame_len) ** 2) - edge
+        ) / (1.0 - edge)
 
     @classmethod
     def from_frames(
         cls,
         sig_frames_obj: BaseFrames,
         max_formants: int = 5,
         lower: float = 50.0,
         upper: float = 5450.0,
         preemphasis_from: Optional[float] = 50.0,
-        window: Optional[Union[str, float, Tuple]] = "praat_gaussian"
+        window: Optional[Union[str, float, Tuple]] = "praat_gaussian",
     ):
         """Extract formants from signal frames.
 
         Parameters
         ----------
         sig_frames_obj: BaseFrames
             Signal frames object.
         max_formants: int, default=5
-            The maximum number of formants that were extracted.
+            The maximum number of formants that are extracted.
         lower: float, default=50.0
             Lower limit for formant frequencies (in Hz).
         upper: float, default=5450.0
             Upper limit for formant frequencies (in Hz).
         preemphasis_from: float, default=50.0
-            Starting value for the preemphasis function.
+            Starting value for the preemphasis function (in Hz).
         window: str
-            Window function.
+            Window function that is applied before formant estimation.
 
         """
         frames = sig_frames_obj.frames
 
         if preemphasis_from is not None:
             pre_coef = math.exp(
                 -2 * math.pi * preemphasis_from * (1 / sig_frames_obj.sr)
@@ -642,28 +690,28 @@
             Spectrogram frames object.
         pitch_frames_obj: PitchFrames
             Pitch frames object.
         n_harmonics: int, default=100
             Number of harmonics to estimate.
 
         """
-        freqs = librosa.fft_frequencies(
-            sr=spec_frames_obj.sr, n_fft=spec_frames_obj.frame_len
-        )
 
         # harmonics = librosa.f0_harmonics(
         #     np.abs(spec_frames_obj.frames),
         #     freqs=freqs,
         #     f0=pitch_frames_obj.frames,
         #     harmonics=np.arange(n_harmonics) + 1,  # Shift one up
         #     axis=-1,
         # )
 
         harmonics = cls._calc_f0_harmonics(
-            spec_frames_obj.frames, freqs, pitch_frames_obj.frames, n_harmonics
+            spec_frames_obj.frames,
+            spec_frames_obj.freqs,
+            pitch_frames_obj.frames,
+            n_harmonics,
         )
 
         return cls(
             harmonics,
             spec_frames_obj.sr,
             spec_frames_obj.frame_len,
             spec_frames_obj.hop_len,
@@ -763,21 +811,23 @@
         """Estimate formant amplitudes from formant, pitch harmonics, and pitch frames.
 
         Parameters
         ----------
         formant_frames_obj: FormantFrames
             Formant frames object.
         harmonics_frames_obj: PitchHarmonicsFrames
+            Pitch harmonics frames object.
         pitch_frames_obj: PitchFrames
+            Pitch frames object.
         lower: float, optional, default=0.8
             Lower boundary for peak amplitude search interval.
         upper: float, optional, default=1.2
             Upper boundary for peak amplitude search interval.
         rel_f0: bool, optional, default=True
-            Whether the amplitude is divide by the fundamental frequency amplitude.
+            Whether the amplitude is divided by the fundamental frequency amplitude.
         """
         amp_frames = []
 
         for i in range(formant_frames_obj.max_formants):
             freqs = formant_frames_obj.select_formant_attr(i, 0)
             harmonic_freqs = (
                 pitch_frames_obj.frames[:, None]
@@ -788,19 +838,25 @@
             freqs_upper = upper * freqs
             freq_in_bounds = np.logical_and(
                 harmonic_freqs > freqs_lower[:, None],
                 harmonic_freqs < freqs_upper[:, None],
             )
             harmonics_amp = copy(harmonics_frames_obj.frames)
             harmonics_amp[~freq_in_bounds] = np.nan
-            harmonic_peaks = np.nanmax(harmonics_amp, axis=1)
-            harmonic_peaks_db = 20 * np.log10(harmonic_peaks)
+            # Set all-nan frames to nan (otherwise np.nanmax throws warning)
+            harmonic_peaks = np.zeros(harmonics_amp.shape[0:1])
+            harmonics_amp_all_na = np.all(np.isnan(harmonics_amp), axis=1)
+            harmonic_peaks[harmonics_amp_all_na] = np.nan
+            harmonic_peaks[~harmonics_amp_all_na] = np.nanmax(
+                harmonics_amp[~harmonics_amp_all_na], axis=1
+            )
+            harmonic_peaks_db = librosa.amplitude_to_db(harmonic_peaks)
 
             if rel_f0:
-                harmonic_peaks_db = harmonic_peaks_db - 20 * np.log10(f0_amp)
+                harmonic_peaks_db = harmonic_peaks_db - librosa.amplitude_to_db(f0_amp)
 
             amp_frames.append(harmonic_peaks_db)
 
         return cls(
             np.array(amp_frames).T,
             formant_frames_obj.sr,
             formant_frames_obj.frame_len,
@@ -1056,14 +1112,20 @@
         mask = np.logical_and(periods > lower, periods < upper)
 
         # Split periods according to mask and remove masked periods
         periods = np.array_split(periods[mask], np.where(~mask)[0])
 
         return periods, mask
 
+    @staticmethod
+    def _check_ratio(x_arr: np.ndarray, threshold: float) -> np.ndarray:
+        valid = np.logical_and(np.isfinite(x_arr[1:]), x_arr[1:] > 0)
+        valid[valid] = x_arr[:-1][valid] / x_arr[1:][valid] < threshold
+        return valid
+
 
 class JitterFrames(PitchPeriodFrames):
     """Extract and store voice jitter frames.
 
     Parameters
     ----------
     frames: numpy.ndarray
@@ -1154,43 +1216,45 @@
         cls,
         pulses: List[Tuple],
         rel: bool,
         lower: float,
         upper: float,
         max_period_ratio: float,
     ):
-        if len(pulses) > 0:
-            # Calc period length as first order diff of pulse ts
-            periods, _ = cls._calc_period_length(pulses, lower, upper)
-
-            # Calc avg of first order diff in period length
-            # only consider period pairs where ratio is < max_period_ratio
-            avg_period_diff = np.nanmean(
-                np.array(
-                    [
-                        np.mean(
-                            np.abs(
-                                np.diff(period)[
-                                    (period[:-1] / period[1:]) < max_period_ratio
-                                ]
-                            )
-                        )
-                        for period in periods
-                        if len(period) > 0
-                    ]
-                )
+        if len(pulses) == 0:
+            return np.nan
+
+        # Calc period length as first order diff of pulse ts
+        periods, _ = cls._calc_period_length(pulses, lower, upper)
+
+        if len(periods) == 0 or all(len(period) <= 1 for period in periods):
+            return np.nan
+
+        # Calc avg of first order diff in period length
+        # only consider period pairs where ratio is < max_period_ratio
+        period_diff = [
+            np.abs(np.diff(period)[cls._check_ratio(period, max_period_ratio)])
+            for period in periods
+            if len(period) > 1
+        ]
+
+        if len(period_diff) == 0 or all(len(period) == 0 for period in period_diff):
+            return np.nan
+
+        avg_period_diff = np.nanmean(
+            np.array([np.mean(period) for period in period_diff])
+        )
+
+        if rel:  # Relative to mean period length
+            avg_period_len = np.nanmean(
+                np.array([np.mean(period) for period in periods if len(period) > 1])
             )
+            return avg_period_diff / avg_period_len
 
-            if rel:  # Relative to mean period length
-                avg_period_len = np.nanmean(
-                    np.array([np.mean(period) for period in periods if len(period) > 0])
-                )
-                return avg_period_diff / avg_period_len
-            return avg_period_diff
-        return np.nan
+        return avg_period_diff
 
 
 class ShimmerFrames(PitchPeriodFrames):
     """Extract and store voice shimmer frames.
 
     Parameters
     ----------
@@ -1250,15 +1314,15 @@
         """Extract voice shimmer frames from glottal pulse frames.
 
         Parameters
         ----------
         pitch_pulse_frames_obj: PitchPulseFrames
             Glottal pulse frames object.
         rel: bool, optional, default=True
-            Divide shimmer by the average pitch period.
+            Divide shimmer by the average pulse amplitude.
         lower: float, optional, default=0.0001
             Lower limit for periods between glottal pulses.
         upper: float, optional, default=0.02
             Upper limit for periods between glottal pulses.
         max_period_ratio: float, optional, default=1.3
             Maximum ratio between consecutive periods for shimmer extraction.
         max_amp_factor: float, optional, default=1.6
@@ -1293,48 +1357,56 @@
         pulses: List[Tuple],
         rel: bool,
         lower: float,
         upper: float,
         max_period_ratio: float,
         max_amp_factor: float,
     ) -> float:
-        if len(pulses) > 0:
-            # Calc period length as first order diff of pulse ts
-            periods, mask = cls._calc_period_length(pulses, lower, upper)
-            amps = cls._get_amplitude(pulses, mask)
-
-            # Calc avg of first order diff in amplitude
-            # only consider period pairs where period ratio is < max_period_ratio and
-            # where amplitude ratio is < max_amp_factor
-            avg_amp_diff = np.nanmean(
-                np.array(
-                    [
-                        np.mean(
-                            np.abs(
-                                np.diff(amp)[
-                                    np.logical_and(
-                                        (period[:-1] / period[1:]) < max_period_ratio,
-                                        (amp[:-1] / amp[1:]) < max_amp_factor,
-                                    )
-                                ]
-                            )
-                        )
-                        for amp, period in zip(amps, periods)
-                        if len(period) > 0
-                    ]
-                )
+        if len(pulses) == 0:
+            return np.nan
+
+        # Calc period length as first order diff of pulse ts
+        periods, mask = cls._calc_period_length(pulses, lower, upper)
+        amps = cls._get_amplitude(pulses, mask)
+
+        if (
+            len(periods) == 0
+            or len(amps) == 0
+            or all(len(period) <= 1 for period in periods)
+        ):
+            return np.nan
+
+        # Calc avg of first order diff in amplitude
+        # only consider period pairs where period ratio is < max_period_ratio and
+        # where amplitude ratio is < max_amp_factor
+        amp_diff = [
+            np.abs(
+                np.diff(amp)[
+                    np.logical_and(
+                        cls._check_ratio(period, max_period_ratio),
+                        cls._check_ratio(amp, max_amp_factor),
+                    )
+                ]
             )
+            for amp, period in zip(amps, periods)
+            if len(period) > 1 and len(amp) > 1
+        ]
 
-            if rel:  # Relative to mean amplitude
-                avg_amp = np.nanmean(
-                    np.array([np.mean(amp) for amp in amps if len(amp) > 0])
-                )
-                return avg_amp_diff / avg_amp
-            return avg_amp_diff
-        return np.nan
+        if len(amp_diff) == 0 or all(len(amp) == 0 for amp in amp_diff):
+            return np.nan
+
+        avg_amp_diff = np.nanmean(np.array([np.mean(amp) for amp in amp_diff]))
+
+        if rel:  # Relative to mean amplitude
+            avg_amp = np.nanmean(
+                np.array([np.mean(amp) for amp in amps if len(amp) > 1])
+            )
+            return avg_amp_diff / avg_amp
+
+        return avg_amp_diff
 
     @staticmethod
     def _get_amplitude(pulses: List[Tuple], mask: np.ndarray) -> List:
         # Get amplitudes
         amps = np.array([puls[2] for puls in pulses])[
             1:
         ]  # Skip first amplitude to align with periods
@@ -1410,16 +1482,16 @@
             cls._find_max_peak, 1, auto_cor[:, 1:], sr=sig_frames_obj.sr, lower=lower
         )
         harmonic_comp = harmonic_strength / auto_cor[:, 0]
         hnr = harmonic_comp / (1 - harmonic_comp)
         silence_mask = np.max(
             np.abs(sig_frames_obj.frames), axis=1
         ) > rel_silence_threshold * np.max(np.abs(sig_frames_obj.frames))
-        hnr[~silence_mask] = np.nan
-        hnr_db = 10 * np.log10(hnr)
+        hnr[np.logical_or(~silence_mask, hnr <= 0)] = np.nan
+        hnr_db = librosa.power_to_db(hnr)  # HNR is on power scale
         return cls(
             hnr_db,
             sig_frames_obj.sr,
             sig_frames_obj.frame_len,
             sig_frames_obj.hop_len,
             sig_frames_obj.center,
             sig_frames_obj.pad_mode,
@@ -1427,24 +1499,593 @@
             rel_silence_threshold,
         )
 
     @staticmethod
     def _find_max_peak(auto_cor: np.ndarray, sr: int, lower: float) -> float:
         if np.all(np.isnan(auto_cor)):
             return np.nan
-        
+
         auto_cor_peak_lags = find_peaks(auto_cor)[0]
         auto_cor_peaks = auto_cor[auto_cor_peak_lags]
         auto_cor_peak_periods = 1 / auto_cor_peak_lags * sr
         auto_cor_peaks_voiced = auto_cor_peaks[
             np.logical_and(
                 auto_cor_peak_periods > lower, auto_cor_peak_periods < sr / 2
             )
         ]
 
         if len(auto_cor_peaks_voiced) == 0:
             return np.nan
-        
-        auto_cor_max_peak_lag = np.argmax(
-            auto_cor_peaks_voiced
+
+        auto_cor_max_peak_lag = np.argmax(auto_cor_peaks_voiced)
+
+        return auto_cor_peaks_voiced[auto_cor_max_peak_lag]
+
+
+class AlphaRatioFrames(BaseFrames):
+    """Calculate and store spectogram alpha ratios.
+
+    Parameters
+    ----------
+    frames: numpy.ndarray
+        Alpha ratio frames in dB with shape (num_frames,).
+    lower_band: tuple
+        Boundaries of the lower frequency band (start, end) in Hz.
+    upper_band: tuple
+        Boundaries of the upper frequency band (start, end) in Hz.
+
+    Notes
+    -----
+    Calculate the alpha ratio by dividing the energy (sum of magnitude) in the lower frequency band
+    by the energy in the upper frequency band. The ratio is then converted to dB.
+
+    """
+
+    def __init__(
+        self,
+        frames: np.ndarray,
+        sr: int,
+        frame_len: int,
+        hop_len: int,
+        center: bool,
+        pad_mode: str,
+        lower_band: Tuple[float],
+        upper_band: Tuple[float],
+    ):
+        self.logger = logging.getLogger("mexca.audio.extraction.AlphaRatioFrames")
+        self.lower_band = lower_band
+        self.upper_band = upper_band
+        super().__init__(frames, sr, frame_len, hop_len, center, pad_mode)
+        self.logger.debug(ClassInitMessage())
+
+    @classmethod
+    def from_spec_frames(
+        cls,
+        spec_frames_obj: SpecFrames,
+        lower_band: Tuple = (50.0, 1000.0),
+        upper_band: Tuple = (1000.0, 5000.0),
+    ):
+        """Calculate the alpha ratio from spectrogram frames.
+
+        Parameters
+        ----------
+        spec_frames_obj: SpecFrames
+            Spectrogram frames object.
+        lower_band: tuple, default=(50.0, 1000.0)
+            Boundaries of the lower frequency band (start, end) in Hz.
+        upper_band: tuple, default=(1000.0, 5000.0)
+            Boundaries of the upper frequency band (start, end) in Hz.
+
+        """
+        lower_band_bins = np.logical_and(
+            spec_frames_obj.freqs > lower_band[0],
+            spec_frames_obj.freqs <= lower_band[1],
+        )
+        lower_band_energy = np.nansum(
+            np.abs(spec_frames_obj.frames[:, lower_band_bins]), axis=1
+        )
+        upper_band_bins = np.logical_and(
+            spec_frames_obj.freqs > upper_band[0],
+            spec_frames_obj.freqs <= upper_band[1],
+        )
+        upper_band_energy = np.nansum(
+            np.abs(spec_frames_obj.frames[:, upper_band_bins]), axis=1
+        )
+        alpha_ratio_frames = np.zeros(lower_band_energy.shape)
+
+        upper_band_energy_is_valid = np.logical_and(
+            np.isfinite(upper_band_energy), upper_band_energy != 0
+        )
+
+        alpha_ratio_frames[~upper_band_energy_is_valid] = np.nan
+        alpha_ratio_frames[upper_band_energy_is_valid] = (
+            lower_band_energy[upper_band_energy_is_valid]
+            / upper_band_energy[upper_band_energy_is_valid]
+        )
+
+        alpha_ratio_frames_db = 20.0 * np.log10(alpha_ratio_frames)
+
+        return cls(
+            alpha_ratio_frames_db,
+            spec_frames_obj.sr,
+            spec_frames_obj.frame_len,
+            spec_frames_obj.hop_len,
+            spec_frames_obj.center,
+            spec_frames_obj.pad_mode,
+            lower_band,
+            upper_band,
+        )
+
+
+class HammarIndexFrames(BaseFrames):
+    """Calculate and store the spectogram Hammarberg index.
+
+    Parameters
+    ----------
+    frames: numpy.ndarray
+        Hammarberg index frames in dB with shape (num_frames,).
+    pivot_point: float
+        Point separating the lower and upper frequency regions in Hz.
+    upper: float
+        Upper limit for the upper frequency region in Hz.
+
+    Notes
+    -----
+    Calculate the Hammarberg index by dividing the peak magnitude in the spectrogram region below `pivot_point`
+    by the peak magnitude in region between `pivot_point` and `upper`. The ratio is then converted to dB.
+
+    """
+
+    def __init__(
+        self,
+        frames: np.ndarray,
+        sr: int,
+        frame_len: int,
+        hop_len: int,
+        center: bool,
+        pad_mode: str,
+        pivot_point: float,
+        upper: float,
+    ):
+        self.logger = logging.getLogger("mexca.audio.extraction.HammarIndexFrames")
+        self.pivot_point = pivot_point
+        self.upper = upper
+        super().__init__(frames, sr, frame_len, hop_len, center, pad_mode)
+        self.logger.debug(ClassInitMessage())
+
+    @classmethod
+    def from_spec_frames(
+        cls,
+        spec_frames_obj: SpecFrames,
+        pivot_point: float = 2000.0,
+        upper: float = 5000.0,
+    ):
+        """Calculate the Hammarberg index from spectrogram frames.
+
+        Parameters
+        ----------
+        spec_frames_obj: SpecFrames
+            Spectrogram frames object.
+        pivot_point: float, default=2000.0
+            Point separating the lower and upper frequency regions in Hz.
+        upper: float, default=5000.0
+            Upper limit for the upper frequency region in Hz.
+
+        """
+        lower_band = np.abs(
+            spec_frames_obj.frames[:, spec_frames_obj.freqs <= pivot_point]
+        )
+        upper_band_freqs = np.logical_and(
+            spec_frames_obj.freqs > pivot_point, spec_frames_obj.freqs <= upper
+        )
+        upper_band = np.abs(spec_frames_obj.frames[:, upper_band_freqs])
+
+        hammar_index_frames = np.zeros(lower_band.shape[0])
+
+        upper_band_is_valid = np.logical_and(
+            np.any(np.isfinite(upper_band), axis=1), np.all(upper_band > 0, axis=1)
+        )
+
+        hammar_index_frames[~upper_band_is_valid] = np.nan
+        hammar_index_frames[upper_band_is_valid] = np.nanmax(
+            lower_band[upper_band_is_valid, :], axis=1
+        ) / np.nanmax(upper_band[upper_band_is_valid, :], axis=1)
+
+        hammar_index_frames_db = librosa.amplitude_to_db(hammar_index_frames)
+
+        return cls(
+            hammar_index_frames_db,
+            spec_frames_obj.sr,
+            spec_frames_obj.frame_len,
+            spec_frames_obj.hop_len,
+            spec_frames_obj.center,
+            spec_frames_obj.pad_mode,
+            pivot_point,
+            upper,
+        )
+
+
+class SpectralSlopeFrames(BaseFrames):
+    """Estimate and store spectral slopes.
+
+    Parameters
+    ----------
+    frames: numpy.ndarray
+        Spectral slope frames with shape (num_frames, num_bands).
+    bands: tuple
+        Frequency bands in Hz for which slopes were estimated.
+
+    Notes
+    -----
+    Estimate spectral slopes by fitting linear models to frequency bands predicting power in dB from frequency in Hz.
+    Fits separate models for each frame and band.
+
+    """
+
+    def __init__(
+        self,
+        frames: np.ndarray,
+        sr: int,
+        frame_len: int,
+        hop_len: int,
+        center: bool,
+        pad_mode: str,
+        bands: Tuple[Tuple[float]],
+    ):
+        self.logger = logging.getLogger("mexca.audio.extraction.HammarIndexFrames")
+        self.bands = bands
+        super().__init__(frames, sr, frame_len, hop_len, center, pad_mode)
+        self.logger.debug(ClassInitMessage())
+
+    @classmethod
+    def from_spec_frames(
+        cls,
+        spec_frames_obj: SpecFrames,
+        bands: Tuple[Tuple[float]] = ((0.0, 500.0), (500.0, 1500.0)),
+    ):
+        """Estimate spectral slopes from spectrogram frames.
+
+        Parameters
+        ----------
+        spec_frames_obj: SpecFrames
+            Spectrogram frames object.
+        bands: tuple, default=((0.0, 500.0), (500.0, 1500.0))
+            Frequency bands in Hz for which slopes are estimated.
+
+        """
+        spectral_slopes = np.zeros(shape=(spec_frames_obj.idx.shape[0], len(bands)))
+
+        for i, band in enumerate(bands):
+            band_freqs_mask = np.logical_and(
+                spec_frames_obj.freqs > band[0], spec_frames_obj.freqs <= band[1]
+            )
+            band_power = np.abs(spec_frames_obj.frames[:, band_freqs_mask])
+            band_freqs = spec_frames_obj.freqs[band_freqs_mask]
+            spectral_slopes[:, i] = np.apply_along_axis(
+                cls._calc_spectral_slope, 1, band_power, band_freqs=band_freqs
+            ).squeeze()
+
+        return cls(
+            spectral_slopes,
+            spec_frames_obj.sr,
+            spec_frames_obj.frame_len,
+            spec_frames_obj.hop_len,
+            spec_frames_obj.center,
+            spec_frames_obj.pad_mode,
+            bands,
+        )
+
+    @staticmethod
+    def _calc_spectral_slope(
+        band_power: np.ndarray, band_freqs: np.ndarray
+    ) -> np.ndarray:
+        band_power_is_valid = np.logical_and(np.isfinite(band_power), band_power > 0)
+
+        if np.all(~band_power_is_valid):
+            return np.nan
+
+        band_freqs_finite = band_freqs[band_power_is_valid]
+        band_power_finite_db = librosa.amplitude_to_db(band_power[band_power_is_valid])
+
+        linear_model = LinearRegression()
+        linear_model.fit(band_freqs_finite.reshape(-1, 1), band_power_finite_db)
+        return linear_model.coef_
+
+
+class MelSpecFrames(SpecFrames):
+    """Calculate and store Mel spectrograms.
+
+    Parameters
+    ----------
+    frames: numpy.ndarray
+        Spectrogram frames on the Mel power scale with shape (num_frames, n_mels).
+    n_mels: int
+        Number of Mel filters.
+    lower: float
+        Lower frequency boundary in Hz.
+    upper: float
+        Upper frequency boundary in Hz.
+
+    See Also
+    --------
+    librosa.feature.melspectrogram
+
+    """
+
+    def __init__(
+        self,
+        frames: np.ndarray,
+        sr: int,
+        window: str,
+        frame_len: int,
+        hop_len: int,
+        center: bool,
+        pad_mode: str,
+        n_mels: int,
+        lower: float,
+        upper: float,
+    ):
+        self.logger = logging.getLogger("mexca.audio.extraction.MelSpecFrames")
+        self.n_mels = n_mels
+        self.lower = lower
+        self.upper = upper
+        super().__init__(frames, sr, window, frame_len, hop_len, center, pad_mode)
+        self.logger.debug(ClassInitMessage())
+
+    @classmethod
+    def from_spec_frames(
+        cls,
+        spec_frames_obj: SpecFrames,
+        n_mels: int = 26,
+        lower: float = 20.0,
+        upper: float = 8000.0,
+    ):
+        """Calculate Mel spectrograms from spectrogram frames.
+
+        spec_frames_obj: SpecFrames
+            Spectrogram frames object.
+        n_mels: int, default=26
+            Number of Mel filters.
+        lower: float, default=20.0
+            Lower frequency boundary in Hz.
+        upper: float, default=8000.0
+            Upper frequency boundary in Hz.
+
+        """
+        mel_spec_frames = librosa.feature.melspectrogram(
+            S=np.abs(spec_frames_obj.frames.T) ** 2,  # requires power spectrum
+            sr=spec_frames_obj.sr,
+            n_fft=spec_frames_obj.frame_len,
+            hop_length=spec_frames_obj.hop_len,
+            window=spec_frames_obj.window,
+            center=spec_frames_obj.center,
+            pad_mode=spec_frames_obj.pad_mode,
+            n_mels=n_mels,
+            fmin=lower,
+            fmax=upper,
+        )
+
+        return cls(
+            mel_spec_frames.T,  # outputs power spectrum
+            spec_frames_obj.sr,
+            spec_frames_obj.window,
+            spec_frames_obj.frame_len,
+            spec_frames_obj.hop_len,
+            spec_frames_obj.center,
+            spec_frames_obj.pad_mode,
+            n_mels,
+            lower,
+            upper,
+        )
+
+
+class MfccFrames(MelSpecFrames):
+    """Estimate and store Mel frequency cepstral coefficients (MFCCs).
+
+    Parameters
+    ----------
+    frames: numpy.ndarray
+        MFCC frames with shape (num_frames, n_mfcc).
+    n_mfcc: int
+        Number of coeffcients that were estimated per frame.
+    lifter: float
+        Cepstral liftering coefficient. Must be >= 0. If zero, no liftering is applied.
+
+
+    """
+
+    def __init__(
+        self,
+        frames: np.ndarray,
+        sr: int,
+        window: str,
+        frame_len: int,
+        hop_len: int,
+        center: bool,
+        pad_mode: str,
+        n_mels: int,
+        lower: float,
+        upper: float,
+        n_mfcc: int,
+        lifter: float,
+    ):
+        self.logger = logging.getLogger("mexca.audio.extraction.MfccFrames")
+        self.n_mfcc = n_mfcc
+        self.lifter = lifter
+        super().__init__(
+            frames,
+            sr,
+            window,
+            frame_len,
+            hop_len,
+            center,
+            pad_mode,
+            n_mels,
+            lower,
+            upper,
+        )
+        self.logger.debug(ClassInitMessage())
+
+    @classmethod
+    def from_mel_spec_frames(
+        cls, mel_spec_frames_obj: MelSpecFrames, n_mfcc: int = 4, lifter: float = 22.0
+    ):
+        """Estimate MFCCs from Mel spectogram frames.
+
+        Parameters
+        ----------
+        mel_spec_frames_obj: MelSpecFrames
+            Mel spectrogram frames object.
+        n_mfcc: int, default=4
+            Number of coeffcients that were estimated per frame.
+        lifter: float, default=22.0
+            Cepstral liftering coefficient. Must be >= 0. If zero, no liftering is applied.
+
+        See Also
+        --------
+        librosa.feature.mfcc
+
+        """
+        mfcc_frames = librosa.feature.mfcc(
+            S=librosa.power_to_db(mel_spec_frames_obj.frames.T),  # dB on power spectrum
+            sr=mel_spec_frames_obj.sr,
+            n_mfcc=n_mfcc,
+            lifter=lifter,
+        )
+
+        return cls(
+            mfcc_frames.T,
+            mel_spec_frames_obj.sr,
+            mel_spec_frames_obj.window,
+            mel_spec_frames_obj.frame_len,
+            mel_spec_frames_obj.hop_len,
+            mel_spec_frames_obj.center,
+            mel_spec_frames_obj.pad_mode,
+            mel_spec_frames_obj.n_mels,
+            mel_spec_frames_obj.lower,
+            mel_spec_frames_obj.upper,
+            n_mfcc,
+            lifter,
+        )
+
+
+class SpectralFluxFrames(SpecFrames):
+    """Calculate and store spectral flux.
+
+    Parameters
+    ----------
+    frames: numpy.ndarray
+        Spectral flux frames with shape (num_frames-1,).
+    lower: float
+        Lower limit for frequency bins.
+    upper: float
+        Upper limit for frequency bins
+
+    Notes
+    -----
+    Compute the spectral flux as:
+
+    1. Compute the normalized magnitudes of the frame spectra by dividing the magnitude
+       at each frequency bin by the sum of all frequency bins.
+    2. Compute the first-order difference of normalized magnitudes for each frequency bin within [`lower`, `upper`) across frames.
+    3. Sum up the squared differences for each frame.
+
+    Due to the first-order difference, the object has a frame less than the
+    spectrogram from which it has been computed.
+
+
+    """
+
+    def __init__(
+        self,
+        frames: np.ndarray,
+        sr: int,
+        window: str,
+        frame_len: int,
+        hop_len: int,
+        center: bool,
+        pad_mode: str,
+        lower: float,
+        upper: float,
+    ) -> None:
+        self.logger = logging.getLogger("mexca.audio.extraction.SpectralFluxFrames")
+        self.lower = lower
+        self.upper = upper
+        super().__init__(frames, sr, window, frame_len, hop_len, center, pad_mode)
+        self.logger.debug(ClassInitMessage())
+
+    @classmethod
+    def from_spec_frames(
+        cls, spec_frames_obj: SpecFrames, lower: float = 0.0, upper: float = 5000.0
+    ):
+        """Calculate the spectral flux from spectrogram frames.
+
+        Parameters
+        ----------
+        spec_frames_obj: SpecFrames
+            Spectrogram frames object.
+        lower: float, default=0.0
+            Lower limit for frequency bins.
+        upper: float, default=5000.0
+            Upper limit for frequency bins
+
+        """
+        spec_freq_mask = np.logical_and(
+            spec_frames_obj.freqs >= lower, spec_frames_obj.freqs < upper
+        )
+        spec_mag = np.abs(spec_frames_obj.frames)
+        spec_norm = np.sum(spec_mag, axis=1)
+        spec_diff = np.diff(spec_mag[:, spec_freq_mask] / spec_norm[:, None], axis=0)
+        spec_flux_frames = np.sum(spec_diff**2, axis=1)
+
+        return cls(
+            spec_flux_frames,
+            spec_frames_obj.sr,
+            spec_frames_obj.window,
+            spec_frames_obj.frame_len,
+            spec_frames_obj.hop_len,
+            spec_frames_obj.center,
+            spec_frames_obj.pad_mode,
+            lower,
+            upper,
+        )
+
+
+class RmsEnergyFrames(SpecFrames):
+    """Calculate and store the root mean squared (RMS) energy.
+
+    Parameters
+    ---------
+    frames: numpy.ndarray
+        RMS energy frames in dB with shape (num_frames,).
+
+    """
+
+    @classmethod
+    def from_spec_frames(cls, spec_frames_obj: SpecFrames):
+        """Calculate the RMS energy from spectrogram frames.
+
+        Parameters
+        ----------
+        spec_frames_obj: SpecFrames
+            Spectrogram frames object.
+
+        """
+        rms_frames = librosa.amplitude_to_db(
+            librosa.feature.rms(  # to dB
+                S=np.abs(spec_frames_obj.frames).T,
+                frame_length=spec_frames_obj.frame_len,
+                hop_length=spec_frames_obj.hop_len,
+                center=spec_frames_obj.center,
+                pad_mode=spec_frames_obj.pad_mode,
+            )
+        )
+
+        return cls(
+            rms_frames.squeeze(),
+            spec_frames_obj.sr,
+            spec_frames_obj.window,
+            spec_frames_obj.frame_len,
+            spec_frames_obj.hop_len,
+            spec_frames_obj.center,
+            spec_frames_obj.pad_mode,
         )
-        return auto_cor[auto_cor_max_peak_lag]
```

### Comparing `mexca-0.3.0/mexca/audio/identification.py` & `mexca-0.4.0/mexca/audio/identification.py`

 * *Files identical despite different names*

### Comparing `mexca-0.3.0/mexca/container.py` & `mexca-0.4.0/mexca/container.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 
 import os
 from typing import List, Optional, Tuple, Union
 import docker
 from docker.errors import DockerException
 from docker.types import Mount
 from mexca import __version__ as VERSION
-from mexca.data import AudioTranscription, SentimentAnnotation, SpeakerAnnotation, VideoAnnotation, VoiceFeatures
+from mexca.data import (AudioTranscription, SentimentAnnotation, SpeakerAnnotation, VideoAnnotation, VoiceFeatures,
+                        VoiceFeaturesConfig)
 
 
 class BaseContainer:
     """Base class for container components. Only for internal use.
 
     Parameters
     ----------
@@ -80,25 +81,26 @@
 
     See Also
     --------
     FaceExtractor
 
     """
 
-    def __init__(
+    def __init__( #pylint: disable=too-many-arguments,too-many-locals
         self,
         num_faces: Optional[int],
         min_face_size: int = 20,
         thresholds: Tuple[float] = (0.6, 0.7, 0.7),
         factor: float = 0.709,
         post_process: bool = True,
         select_largest: bool = True,
         selection_method: Optional[str] = None,
         keep_all: bool = True,
         device: Optional["torch.device"] = "cpu",
+        max_cluster_frames: Optional[int] = None,
         embeddings_model: str = "vggface2",
         au_model: str = "xgb",
         landmark_model: str = "mobilefacenet",
         image_name: str = "mexca/face-extractor",
         get_latest_tag: bool = False,
     ):
         self.num_faces = num_faces
@@ -106,14 +108,15 @@
         self.thresholds = thresholds
         self.factor = factor
         self.post_process = post_process
         self.select_largest = select_largest
         self.selection_method = selection_method
         self.keep_all = keep_all
         self.device = device
+        self.max_cluster_frames = max_cluster_frames
         self.embeddings_model = embeddings_model
         self.au_model = au_model
         self.landmark_model = landmark_model
 
         super().__init__(image_name=image_name, get_latest_tag=get_latest_tag)
 
     def apply(
@@ -150,14 +153,16 @@
             self.select_largest,
             "--selection-method",
             self.selection_method,
             "--keep-all",
             self.keep_all,
             "--device",
             self.device,
+            "--max-cluster-frames",
+            self.max_cluster_frames,
             "--embeddings-model",
             self.embeddings_model,
             "--au-model",
             self.au_model,
             "--landmark-model",
             self.landmark_model,
         ]
@@ -224,39 +229,51 @@
 
 
 class VoiceExtractorContainer(BaseContainer):
     """Container for `VoiceExtractor` component.
 
     Other Parameters
     ----------------
+    config: VoiceFeaturesConfig, optional, default=None
+        Voice feature extraction configuration object. If `None`, uses :class:`VoiceFeaturesConfig`'s default configuration.
     image_name: str, default='mexca-voice-extractor'
         Name of the image to create a container from.
         Pulls the image from Docker Hub if not found locally.
 
     See Also
     --------
     VoiceExtractor
 
     """
 
     def __init__(
-        self, image_name: str = "mexca/voice-extractor", get_latest_tag: bool = False
+        self, config: Optional[VoiceFeaturesConfig] = None, image_name: str = "mexca/voice-extractor", get_latest_tag: bool = False
     ):
+        self.config = config
         super().__init__(image_name=image_name, get_latest_tag=get_latest_tag)
 
     def apply(
         self, filepath: str, time_step: float, skip_frames: int = 1
     ) -> VoiceFeatures:
+        outdir = self._create_mounts(filepath=filepath)
+
         cmd_args = ["--time-step", str(time_step), "--skip-frames", str(skip_frames)]
-        cmd = self._create_base_cmd(filepath=filepath)
 
-        outdir = self._create_mounts(filepath=filepath)
+        if self.config is not None:
+            config_path = self._create_out_path_stem(filepath=filepath, outdir=outdir) + "voice_features_config.yml"
+            self.config.write_yaml(config_path)
+            cmd_args.extend(["--config-filepath", config_path])
+        
+        cmd = self._create_base_cmd(filepath=filepath)
 
         self._run_container(cmd + cmd_args)
 
+        if self.config is not None:
+            os.remove(config_path)
+
         return VoiceFeatures.from_json(
             self._create_out_path_stem(filepath=filepath, outdir=outdir)
             + "_voice_features.json"
         )
 
 
 class AudioTranscriberContainer(BaseContainer):
```

### Comparing `mexca-0.3.0/mexca/pipeline.py` & `mexca-0.4.0/mexca/pipeline.py`

 * *Files identical despite different names*

### Comparing `mexca-0.3.0/mexca/text/sentiment.py` & `mexca-0.4.0/mexca/text/sentiment.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Extract sentiment from text.
 """
 
 import argparse
 import logging
 import os
 from typing import Optional
+import torch
 from intervaltree import Interval
 from scipy.special import softmax
 from tqdm import tqdm
 from transformers import AutoModelForSequenceClassification, AutoTokenizer, XLMRobertaForSequenceClassification
 from mexca.data import AudioTranscription, SentimentAnnotation, SentimentData
 from mexca.utils import ClassInitMessage, str2bool
 
@@ -17,43 +18,53 @@
     """Extract sentiment from text.
 
     Parameters
     ----------
     model_name: str, optional
         The name of the text sequence classification model on Hugging Face hub used for
         sentiment prediction. By default `'cardiffnlp/twitter-xlm-roberta-base-sentiment'`.
+    device: torch.device, optional, default=None
+        The device on which sentiment extraction is performed. If `None`, defaults to `'cpu'`.
 
     Attributes
     ----------
     tokenizer: transformers.PreTrainedTokenizer
         The pretrained tokenizer for sequence classification.
         Loaded automatically from `model_name`.
 
     """
-    def __init__(self, model_name: Optional[str] = None):
+    def __init__(self, model_name: Optional[str] = None, device: Optional[torch.device] = None):
         self.logger = logging.getLogger('mexca.text.extraction.SentimentExtractor')
         if not model_name:
             model_name = "cardiffnlp/twitter-xlm-roberta-base-sentiment"
             self.logger.debug('Using default pretrained model %s because "model_name=None"', model_name)
 
+        if device is None:
+            device = "cpu"
+
+        self.device = device
         self.model_name = model_name
         self.tokenizer = AutoTokenizer.from_pretrained(model_name)
         # Lazy initialization
         self._classifier = None
         self.logger.debug(ClassInitMessage())
 
 
     # Initialize pretrained models only when needed
     @property
     def classifier(self) -> XLMRobertaForSequenceClassification:
         """The pretrained sequence classification model for sentiment prediction.
         Loaded automatically from `model_name`.
         """
         if not self._classifier:
-            self._classifier = AutoModelForSequenceClassification.from_pretrained(self.model_name)
+            self._classifier = AutoModelForSequenceClassification.from_pretrained(
+                self.model_name,
+                device_map="auto",
+                load_in_8bit=self.device == "cuda"
+            )
             self.logger.debug('Initialized sentiment extraction model')
 
         return self._classifier
 
 
     # Delete pretrained models when not needed anymore
     @classifier.deleter
@@ -84,17 +95,17 @@
 
         """
 
         sentiment_annotation = SentimentAnnotation()
 
         for i, sent in tqdm(enumerate(transcription.subtitles), total=len(transcription), disable=not show_progress):
             self.logger.debug('Extracting sentiment for sentence %s', i)
-            tokens = self.tokenizer(sent.data.text, return_tensors='pt')
+            tokens = self.tokenizer(sent.data.text, return_tensors='pt').to(self.device)
             output = self.classifier(**tokens)
-            logits = output.logits.detach().numpy()
+            logits = output.logits.detach().cpu().numpy()
             scores = softmax(logits)[0]
             sentiment_annotation.add(Interval(
                 begin=sent.begin,
                 end=sent.end,
                 data=SentimentData(
                     text=sent.data.text,
                     pos=float(scores[2]),
```

### Comparing `mexca-0.3.0/mexca/text/transcription.py` & `mexca-0.4.0/mexca/text/transcription.py`

 * *Files identical despite different names*

### Comparing `mexca-0.3.0/mexca/utils.py` & `mexca-0.4.0/mexca/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from mexca.data import (AudioTranscription, Multimodal, SentimentAnnotation, SpeakerAnnotation, VideoAnnotation,
                         VoiceFeatures)
 
 
 # Adapted from whisper.utils
 # See: https://github.com/openai/whisper/blob/28769fcfe50755a817ab922a7bc83483159600a9/whisper/utils.py
 
+
 def str2bool(string: str):
     str2val = {"True": True, "False": False}
     if string in str2val:
         return str2val[string]
 
     raise ValueError(f"Expected one of {set(str2val.keys())}, got {string}")
 
@@ -27,120 +28,191 @@
 
 
 def optional_str(string: str):
     return None if string == "None" else str(string)
 
 
 def bool_or_str(string: str):
-    try: 
+    try:
         return str2bool(string)
     except ValueError:
         return string
 
 
 class ClassInitMessage:
     def __init__(self):
-        self.message = 'Initialized class instance'
+        self.message = "Initialized class instance"
 
     def __str__(self):
         return self.message
 
 
 def _validate_face_features(multimodal: Multimodal):
-    assert multimodal.features.face_box.dtype == 'object'
-    assert multimodal.features.face_prob.dtype == 'float64'
-    assert multimodal.features.face_landmarks.dtype == 'object'
-    assert multimodal.features.face_aus.dtype == 'object'
-    assert multimodal.features.face_label.dtype == 'float64'
-    assert multimodal.features.face_confidence.dtype == 'float64'
+    assert multimodal.features.face_box.dtype == "object"
+    assert multimodal.features.face_prob.dtype == "float64"
+    assert multimodal.features.face_landmarks.dtype == "object"
+    assert multimodal.features.face_aus.dtype == "object"
+    assert multimodal.features.face_label.dtype == "float64"
+    assert multimodal.features.face_confidence.dtype == "float64"
 
     assert all(len(bbox) == 4 for bbox in multimodal.features.face_box.dropna())
     assert all(len(lmks) == 68 for lmks in multimodal.features.face_landmarks.dropna())
     assert all(len(aus) == 20 for aus in multimodal.features.face_aus.dropna())
 
-    assert multimodal.features.face_box.isna().eq(multimodal.features.face_prob.isna()).all()
-    assert multimodal.features.face_box.isna().eq(multimodal.features.face_landmarks.isna()).all()
-    assert multimodal.features.face_box.isna().eq(multimodal.features.face_aus.isna()).all()
-    assert multimodal.features.face_box.isna().eq(multimodal.features.face_label.isna()).all()
+    assert (
+        multimodal.features.face_box.isna()
+        .eq(multimodal.features.face_prob.isna())
+        .all()
+    )
+    assert (
+        multimodal.features.face_box.isna()
+        .eq(multimodal.features.face_landmarks.isna())
+        .all()
+    )
+    assert (
+        multimodal.features.face_box.isna()
+        .eq(multimodal.features.face_aus.isna())
+        .all()
+    )
+    assert (
+        multimodal.features.face_box.isna()
+        .eq(multimodal.features.face_label.isna())
+        .all()
+    )
 
 
 def _validate_speech_segments(multimodal: Multimodal):
-    assert multimodal.features.segment_start.dtype == 'float64'
-    assert multimodal.features.segment_end.dtype == 'float64'
-    assert multimodal.features.segment_speaker_label.dtype == 'object'
-    assert multimodal.features.segment_start.le(multimodal.features.time, fill_value=0).all()
-    assert multimodal.features.segment_end.ge(multimodal.features.time, fill_value=multimodal.features.time.max()).all()
-    assert multimodal.features.segment_start.dropna().lt(multimodal.features.segment_end.dropna()).all()
-    assert multimodal.features.segment_start.isna().eq(multimodal.features.segment_end.isna()).all()
-    assert multimodal.features.segment_start.isna().eq(multimodal.features.segment_speaker_label.isna()).all()
+    assert multimodal.features.segment_start.dtype == "float64"
+    assert multimodal.features.segment_end.dtype == "float64"
+    assert multimodal.features.segment_speaker_label.dtype == "object"
+    assert multimodal.features.segment_start.le(
+        multimodal.features.time, fill_value=0
+    ).all()
+    assert multimodal.features.segment_end.ge(
+        multimodal.features.time, fill_value=multimodal.features.time.max()
+    ).all()
+    assert (
+        multimodal.features.segment_start.dropna()
+        .lt(multimodal.features.segment_end.dropna())
+        .all()
+    )
+    assert (
+        multimodal.features.segment_start.isna()
+        .eq(multimodal.features.segment_end.isna())
+        .all()
+    )
+    assert (
+        multimodal.features.segment_start.isna()
+        .eq(multimodal.features.segment_speaker_label.isna())
+        .all()
+    )
 
     for seg in multimodal.audio_annotation.items():
         assert seg.begin in multimodal.features.segment_start.to_numpy()
         assert seg.end in multimodal.features.segment_end.to_numpy()
-        assert str(seg.data.name) in multimodal.features.segment_speaker_label.to_numpy().astype(str)
+        assert str(
+            seg.data.name
+        ) in multimodal.features.segment_speaker_label.to_numpy().astype(str)
 
 
-def _validate_voice_feature(feat: pd.Series, ref_feat: np.ndarray, d_type: str = 'float64', is_pos: bool = False):
+def _validate_voice_feature(
+    feat: pd.Series, ref_feat: np.ndarray, d_type: str = "float64", is_pos: bool = False
+):
     assert feat.dtype == d_type
     assert len(feat.dropna()) > 0
     if is_pos:
         assert feat[np.isfinite(feat)] > 0
-    
+
     for f in feat[:-1]:
         if np.isfinite(f):
             assert f in ref_feat
 
 
 def _validate_voice_features(multimodal: Multimodal):
     for feat_name in multimodal.voice_features.__dict__:
-        if feat_name not in ("frame", "time"):
-            _validate_voice_feature(multimodal.features[feat_name], getattr(multimodal.voice_features, feat_name))
+        if feat_name not in (
+            "frame",
+            "time",
+            "hnr_db",
+            "f1_amplitude_rel_f0",
+            "f2_amplitude_rel_f0",
+            "f3_amplitude_rel_f0",
+            "h1_f3_diff_db",
+        ):
+            _validate_voice_feature(
+                multimodal.features[feat_name],
+                getattr(multimodal.voice_features, feat_name),
+            )
 
 
 def _validate_transcription(multimodal: Multimodal):
-    assert multimodal.features.span_start.dtype == 'float64'
-    assert multimodal.features.span_end.dtype == 'float64'
-    assert multimodal.features.span_text.dtype == 'object'
-    assert multimodal.features.span_start.le(multimodal.features.time, fill_value=0).all()
-    assert multimodal.features.span_end.ge(multimodal.features.time, fill_value=multimodal.features.time.max()).all()
+    assert multimodal.features.span_start.dtype == "float64"
+    assert multimodal.features.span_end.dtype == "float64"
+    assert multimodal.features.span_text.dtype == "object"
+    assert multimodal.features.span_start.le(
+        multimodal.features.time, fill_value=0
+    ).all()
+    assert multimodal.features.span_end.ge(
+        multimodal.features.time, fill_value=multimodal.features.time.max()
+    ).all()
     # assert multimodal.features.span_start.le(multimodal.features.segment_end, fill_value=0).all()
     # assert multimodal.features.span_end.le(multimodal.features.segment_end, fill_value=0).all()
-    assert multimodal.features.span_start.isna().eq(multimodal.features.span_end.isna()).all()
-    assert multimodal.features.span_start.isna().eq(multimodal.features.span_text.isna()).all()
+    assert (
+        multimodal.features.span_start.isna()
+        .eq(multimodal.features.span_end.isna())
+        .all()
+    )
+    assert (
+        multimodal.features.span_start.isna()
+        .eq(multimodal.features.span_text.isna())
+        .all()
+    )
 
     for seg in multimodal.transcription.subtitles.items():
         assert seg.begin in multimodal.features.span_start.to_numpy()
         assert seg.end in multimodal.features.span_end.to_numpy()
         assert seg.data.text in multimodal.features.span_text.to_numpy()
 
 
 def _validate_sentiment(multimodal: Multimodal):
-    assert multimodal.features.span_sent_pos.dtype == 'float64'
-    assert multimodal.features.span_sent_neg.dtype == 'float64'
-    assert multimodal.features.span_sent_neu.dtype == 'float64'
-    assert multimodal.features.span_start.isna().eq(multimodal.features.span_sent_pos.isna()).all()
-    assert multimodal.features.span_start.isna().eq(multimodal.features.span_sent_neg.isna()).all()
-    assert multimodal.features.span_start.isna().eq(multimodal.features.span_sent_neu.isna()).all()
+    assert multimodal.features.span_sent_pos.dtype == "float64"
+    assert multimodal.features.span_sent_neg.dtype == "float64"
+    assert multimodal.features.span_sent_neu.dtype == "float64"
+    assert (
+        multimodal.features.span_start.isna()
+        .eq(multimodal.features.span_sent_pos.isna())
+        .all()
+    )
+    assert (
+        multimodal.features.span_start.isna()
+        .eq(multimodal.features.span_sent_neg.isna())
+        .all()
+    )
+    assert (
+        multimodal.features.span_start.isna()
+        .eq(multimodal.features.span_sent_neu.isna())
+        .all()
+    )
 
     for seg in multimodal.sentiment.items():
         assert seg.begin in multimodal.features.span_start.to_numpy()
         assert seg.end in multimodal.features.span_end.to_numpy()
         assert seg.data.pos in multimodal.features.span_sent_pos.to_numpy()
         assert seg.data.neg in multimodal.features.span_sent_neg.to_numpy()
         assert seg.data.neu in multimodal.features.span_sent_neu.to_numpy()
 
 
 def _validate_multimodal(
-        output: Multimodal,
-        check_video_annotation: bool = True,
-        check_audio_annotation: bool = True,
-        check_voice_features: bool = True,
-        check_transcription: bool = True,
-        check_sentiment: bool = True
-    ):
+    output: Multimodal,
+    check_video_annotation: bool = True,
+    check_audio_annotation: bool = True,
+    check_voice_features: bool = True,
+    check_transcription: bool = True,
+    check_sentiment: bool = True,
+):
     assert isinstance(output, Multimodal)
 
     if check_video_annotation:
         assert isinstance(output.video_annotation, VideoAnnotation)
         _validate_face_features(output)
     if check_audio_annotation:
         assert isinstance(output.audio_annotation, SpeakerAnnotation)
```

### Comparing `mexca-0.3.0/mexca/video.py` & `mexca-0.4.0/mexca/video.py`

 * *Files 2% similar despite different names*

```diff
@@ -196,14 +196,18 @@
         if multiple faces are detected.
     selection_method : {None, 'probability', 'largest', 'largest_over_threshold', 'center_weighted_size'}, optional, default=None
         The heuristic used for selecting detected faces. If not `None`, overrides `select_largest`.
     keep_all: bool, default=True
         Whether all faces should be returned in the order of `select_largest`.
     device: torch.device, optional, default=None
         The device on which face detection and embedding computations are performed.
+    max_cluster_frames : int, optional, default=None
+        Maximum number of frames that are used for spectral clustering. If the number of frames exceeds the maximum,
+        hierarchical clustering is applied first to reduce the frames to this number. This can reduce the computational
+        costs for long videos.
     embeddings_model : {'vggface2', 'casia-webface'}, default='vggface2'
         Pretrained Inception Resnet V1 model for computing face embeddings.
     au_model : {'xgb', 'svm'}, default='xgb'
         Pretrained model for predicting facial action unit activations.
     landmark_model : {'mobilefacenet', 'mobilenet', 'pfld'}, default='mobilefacenet'
         Pretrained model for detecting facial landmarks.
 
@@ -221,14 +225,15 @@
         thresholds: Tuple[float] = (0.6, 0.7, 0.7),
         factor: float = 0.709,
         post_process: bool = True,
         select_largest: bool = True,
         selection_method: Optional[str] = None,
         keep_all: bool = True,
         device: Optional[torch.device] = None,
+        max_cluster_frames: Optional[int] = None,
         embeddings_model: str = 'vggface2',
         au_model: str = 'xgb',
         landmark_model: str = 'mobilefacenet'
     ):
         self.logger = logging.getLogger('mexca.video.FaceExtractor')
         self.min_face_size = min_face_size
         self.thresholds = thresholds
@@ -238,14 +243,15 @@
         self.selection_method = selection_method
         self.keep_all = keep_all
         self.device = device
         self.embeddings_model = embeddings_model
         self.num_faces = num_faces
         self.au_model = au_model
         self.landmark_model = landmark_model
+        self.max_cluster_frames = max_cluster_frames
         
         # Lazy initialization: See getter functions
         self._detector = None
         self._encoder = None
         self._clusterer = None
         self._extractor = None
         
@@ -304,15 +310,16 @@
     def clusterer(self) -> SpectralClusterer:
         """The spectral clustering model for identifying faces based on embeddings.
         See `spectralcluster <https://wq2012.github.io/SpectralCluster/>`_ for details.
         """
         if not self._clusterer:
             self._clusterer = SpectralClusterer(
                 min_clusters=self.num_faces,
-                max_clusters=self.num_faces
+                max_clusters=self.num_faces,
+                max_spectral_size=self.max_cluster_frames
             )
             self.logger.debug('Initialized spectral clusterer')
         return self._clusterer
 
 
     @clusterer.deleter
     def clusterer(self):
@@ -397,15 +404,15 @@
         -------
         numpy.ndarray
             Embeddings of the N face images with dimensions (N, 512).
 
         """
 
         self.logger.debug('Encoding faces')
-        embeddings = self.encoder(faces).detach().cpu().numpy()
+        embeddings = self.encoder(faces.to(self.device)).detach().cpu().numpy()
 
         return embeddings
 
 
     def identify(self, embeddings: np.ndarray) -> np.ndarray:
         """Cluster faces based on their embeddings.
 
@@ -710,14 +717,15 @@
     parser.add_argument('--thresholds', type=float, nargs=3, default=[0.6, 0.7, 0.7])
     parser.add_argument('--factor', type=float, default=0.709)
     parser.add_argument('--post-process', type=str2bool, default=True, dest='post_process')
     parser.add_argument('--select-largest', type=str2bool, default=True, dest='select_largest')
     parser.add_argument('--selection-method', type=str, default=None, dest='selection_method')
     parser.add_argument('--keep-all', type=str2bool, default=True, dest='keep_all')
     parser.add_argument('--device', type=str, default='cpu')
+    parser.add_argument('--max-cluster-frames', type=optional_int, default=None, dest='max_cluster_frames')
     parser.add_argument('--embeddings-model', type=str, default='vggface2', dest='embeddings_model')
     parser.add_argument('--au-model', type=str, default='xgb', dest='au_model')
     parser.add_argument('--landmark-model', type=str, default='mobilefacenet', dest='landmark_model')
 
     args = parser.parse_args().__dict__
 
     filepath: str = args.pop('filepath')
```

### Comparing `mexca-0.3.0/mexca.egg-info/PKG-INFO` & `mexca-0.4.0/mexca.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: mexca
-Version: 0.3.0
+Version: 0.4.0
 Summary: Emotion expression capture from multiple modalities.
 Home-page: https://github.com/mexca/mexca
 Author: Malte Luken
 Author-email: m.luken@esciencecenter.nl
 Project-URL: Bug Tracker, https://github.com/mexca/mexca/issues
 Keywords: emotion,multimodal,expression
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Python: <3.10,>=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: vid
 Provides-Extra: spe
 Provides-Extra: voi
 Provides-Extra: tra
 Provides-Extra: sen
@@ -101,14 +102,20 @@
 
 The dependencies for the additional components can be installed via:
 
 ```console
 pip install mexca[vid,spe,voi,tra,sen]
 ```
 
+or:
+
+```console
+pip install mexca[all]
+```
+
 The abbreviations indicate:
 
 * `vid`: FaceExtractor
 * `spe`: SpeakerIdentifier
 * `voi`: VoiceExtractor
 * `tra`: AudioTranscriber
 * `sen`: SentimentExtractor
```

### Comparing `mexca-0.3.0/mexca.egg-info/SOURCES.txt` & `mexca-0.4.0/mexca.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mexca-0.3.0/mexca.egg-info/requires.txt` & `mexca-0.4.0/mexca.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 docker==6.0.1
 intervaltree==3.1.0
 moviepy>=1.0.3
-numpy==1.21.6
+numpy>=1.21.6
 pandas==1.3
+pyyaml==6.0
 scipy==1.7.3
 srt==3.5.2
 tqdm>=4.64.0
 
 [all]
 mexca[sen,spe,tra,vid,voi]
 
 [demo]
 ipywidgets
-pyyaml
 
 [dev]
 bump2version
 prospector[with_pyroma]==1.7.7
 pylint==2.15.6
 isort
 pytest
@@ -28,32 +28,34 @@
 myst_parser
 
 [publishing]
 twine
 wheel
 
 [sen]
+accelerate==0.18.0
+bitsandbytes==0.38.1
 protobuf==3.20
 sentencepiece
 torch==1.12.0
-transformers==4.19.2
+transformers==4.25.1
 
 [spe]
 pyannote.audio==2.1.1
 pyannote.core<5.0,>=4.4
 torch==1.12.0
 
 [tra]
 openai-whisper
 stable-ts==1.1.5
 torch==1.12.0
-transformers==4.19.2
+transformers==4.25.1
 
 [vid]
 facenet-pytorch==2.5.2
 py-feat==0.5.0
-spectralcluster==0.2.5
+spectralcluster==0.2.16
 torch==1.12.0
 torchvision==0.13.0
 
 [voi]
 librosa<0.10.0
```

### Comparing `mexca-0.3.0/setup.cfg` & `mexca-0.4.0/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -5,38 +5,40 @@
 	Development Status :: 4 - Beta
 	Intended Audience :: Developers
 	License :: OSI Approved :: Apache Software License
 	Natural Language :: English
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
 description = Emotion expression capture from multiple modalities.
 keywords = 
 	emotion
 	multimodal
 	expression
 long_description = file: README.md
 long_description_content_type = text/markdown
 name = mexca
 project_urls = 
 	Bug Tracker = https://github.com/mexca/mexca/issues
 url = https://github.com/mexca/mexca
-version = 0.3.0
+version = 0.4.0
 
 [options]
 zip_safe = False
 include_package_data = True
 packages = find:
 python_requires = >=3.7,<3.10
 install_requires = 
 	docker==6.0.1
 	intervaltree==3.1.0
 	moviepy>=1.0.3
-	numpy==1.21.6
+	numpy>=1.21.6
 	pandas==1.3
+	pyyaml==6.0
 	scipy==1.7.3
 	srt==3.5.2
 	tqdm>=4.64.0
 
 [options.entry_points]
 console_scripts = 
 	extract-faces = mexca.video:cli
@@ -47,37 +49,38 @@
 
 [options.data_files]
 
 [options.extras_require]
 vid = 
 	facenet-pytorch==2.5.2
 	py-feat==0.5.0
-	spectralcluster==0.2.5
+	spectralcluster==0.2.16
 	torch==1.12.0
 	torchvision==0.13.0
 spe = 
 	pyannote.audio==2.1.1
 	pyannote.core>=4.4,<5.0
 	torch==1.12.0
 voi = 
 	librosa<0.10.0
 tra = 
 	openai-whisper
 	stable-ts==1.1.5
 	torch==1.12.0
-	transformers==4.19.2
+	transformers==4.25.1
 sen = 
+	accelerate==0.18.0
+	bitsandbytes==0.38.1
 	protobuf==3.20
 	sentencepiece
 	torch==1.12.0
-	transformers==4.19.2
+	transformers==4.25.1
 all = mexca[vid,spe,voi,tra,sen]
 demo = 
 	ipywidgets
-	pyyaml
 dev = 
 	bump2version
 	prospector[with_pyroma]==1.7.7
 	pylint==2.15.6
 	isort
 	pytest
 	pytest-cov
```

### Comparing `mexca-0.3.0/tests/test_audio_identification.py` & `mexca-0.4.0/tests/test_audio_identification.py`

 * *Files identical despite different names*

### Comparing `mexca-0.3.0/tests/test_container.py` & `mexca-0.4.0/tests/test_container.py`

 * *Files identical despite different names*

### Comparing `mexca-0.3.0/tests/test_data.py` & `mexca-0.4.0/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `mexca-0.3.0/tests/test_pipeline.py` & `mexca-0.4.0/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `mexca-0.3.0/tests/test_text_sentiment.py` & `mexca-0.4.0/tests/test_text_sentiment.py`

 * *Files identical despite different names*

### Comparing `mexca-0.3.0/tests/test_text_transcription.py` & `mexca-0.4.0/tests/test_text_transcription.py`

 * *Files identical despite different names*

### Comparing `mexca-0.3.0/tests/test_utils.py` & `mexca-0.4.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `mexca-0.3.0/tests/test_video.py` & `mexca-0.4.0/tests/test_video.py`

 * *Files identical despite different names*

