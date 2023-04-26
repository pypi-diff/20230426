# Comparing `tmp/elevenlabslib-0.5.1.tar.gz` & `tmp/elevenlabslib-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elevenlabslib-0.5.1.tar", last modified: Wed Apr 26 11:24:46 2023, max compression
+gzip compressed data, was "elevenlabslib-0.5.2.tar", last modified: Wed Apr 26 11:48:17 2023, max compression
```

## Comparing `elevenlabslib-0.5.1.tar` & `elevenlabslib-0.5.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 11:24:46.007140 elevenlabslib-0.5.1/
--rw-rw-rw-   0        0        0     1091 2023-02-17 22:48:32.000000 elevenlabslib-0.5.1/LICENSE
--rw-rw-rw-   0        0        0     2706 2023-04-26 11:24:46.007140 elevenlabslib-0.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     2050 2023-04-25 20:14:38.000000 elevenlabslib-0.5.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-26 11:24:45.991573 elevenlabslib-0.5.1/elevenlabslib/
--rw-rw-rw-   0        0        0     4534 2023-04-25 19:28:01.000000 elevenlabslib-0.5.1/elevenlabslib/ElevenLabsHistoryItem.py
--rw-rw-rw-   0        0        0     3021 2023-04-25 18:32:03.000000 elevenlabslib-0.5.1/elevenlabslib/ElevenLabsSample.py
--rw-rw-rw-   0        0        0    13370 2023-04-26 11:22:54.000000 elevenlabslib-0.5.1/elevenlabslib/ElevenLabsUser.py
--rw-rw-rw-   0        0        0    31137 2023-04-25 19:23:19.000000 elevenlabslib-0.5.1/elevenlabslib/ElevenLabsVoice.py
--rw-rw-rw-   0        0        0      445 2023-03-25 13:50:30.000000 elevenlabslib-0.5.1/elevenlabslib/__init__.py
--rw-rw-rw-   0        0        0     5387 2023-04-26 11:22:54.000000 elevenlabslib-0.5.1/elevenlabslib/helpers.py
-drwxrwxrwx   0        0        0        0 2023-04-26 11:24:46.006141 elevenlabslib-0.5.1/elevenlabslib.egg-info/
--rw-rw-rw-   0        0        0     2706 2023-04-26 11:24:45.000000 elevenlabslib-0.5.1/elevenlabslib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      405 2023-04-26 11:24:45.000000 elevenlabslib-0.5.1/elevenlabslib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 11:24:45.000000 elevenlabslib-0.5.1/elevenlabslib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-04-26 11:24:45.000000 elevenlabslib-0.5.1/elevenlabslib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-26 11:24:45.000000 elevenlabslib-0.5.1/elevenlabslib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      846 2023-04-26 11:23:05.000000 elevenlabslib-0.5.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-26 11:24:46.008138 elevenlabslib-0.5.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-26 11:48:17.516280 elevenlabslib-0.5.2/
+-rw-rw-rw-   0        0        0     1091 2023-02-17 22:48:32.000000 elevenlabslib-0.5.2/LICENSE
+-rw-rw-rw-   0        0        0     2706 2023-04-26 11:48:17.515279 elevenlabslib-0.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2050 2023-04-25 20:14:38.000000 elevenlabslib-0.5.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-26 11:48:17.501279 elevenlabslib-0.5.2/elevenlabslib/
+-rw-rw-rw-   0        0        0     4534 2023-04-25 19:28:01.000000 elevenlabslib-0.5.2/elevenlabslib/ElevenLabsHistoryItem.py
+-rw-rw-rw-   0        0        0     3021 2023-04-25 18:32:03.000000 elevenlabslib-0.5.2/elevenlabslib/ElevenLabsSample.py
+-rw-rw-rw-   0        0        0    13370 2023-04-26 11:22:54.000000 elevenlabslib-0.5.2/elevenlabslib/ElevenLabsUser.py
+-rw-rw-rw-   0        0        0    31137 2023-04-25 19:23:19.000000 elevenlabslib-0.5.2/elevenlabslib/ElevenLabsVoice.py
+-rw-rw-rw-   0        0        0      445 2023-03-25 13:50:30.000000 elevenlabslib-0.5.2/elevenlabslib/__init__.py
+-rw-rw-rw-   0        0        0     5524 2023-04-26 11:42:12.000000 elevenlabslib-0.5.2/elevenlabslib/helpers.py
+drwxrwxrwx   0        0        0        0 2023-04-26 11:48:17.515279 elevenlabslib-0.5.2/elevenlabslib.egg-info/
+-rw-rw-rw-   0        0        0     2706 2023-04-26 11:48:17.000000 elevenlabslib-0.5.2/elevenlabslib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      405 2023-04-26 11:48:17.000000 elevenlabslib-0.5.2/elevenlabslib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 11:48:17.000000 elevenlabslib-0.5.2/elevenlabslib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-04-26 11:48:17.000000 elevenlabslib-0.5.2/elevenlabslib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-26 11:48:17.000000 elevenlabslib-0.5.2/elevenlabslib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      856 2023-04-26 11:46:48.000000 elevenlabslib-0.5.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-26 11:48:17.516280 elevenlabslib-0.5.2/setup.cfg
```

### Comparing `elevenlabslib-0.5.1/LICENSE` & `elevenlabslib-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.5.1/PKG-INFO` & `elevenlabslib-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elevenlabslib
-Version: 0.5.1
+Version: 0.5.2
 Summary: Complete python wrapper for the elevenlabs API
 Author-email: lugia19 <lugia19@lugia19.com>
 Project-URL: Documentation, https://elevenlabslib.readthedocs.io/en/latest/
 Project-URL: Homepage, https://github.com/lugia19/elevenlabslib
 Project-URL: Bug Tracker, https://github.com/lugia19/elevenlabslib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `elevenlabslib-0.5.1/README.md` & `elevenlabslib-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.5.1/elevenlabslib/ElevenLabsHistoryItem.py` & `elevenlabslib-0.5.2/elevenlabslib/ElevenLabsHistoryItem.py`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.5.1/elevenlabslib/ElevenLabsSample.py` & `elevenlabslib-0.5.2/elevenlabslib/ElevenLabsSample.py`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.5.1/elevenlabslib/ElevenLabsUser.py` & `elevenlabslib-0.5.2/elevenlabslib/ElevenLabsUser.py`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.5.1/elevenlabslib/ElevenLabsVoice.py` & `elevenlabslib-0.5.2/elevenlabslib/ElevenLabsVoice.py`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.5.1/elevenlabslib/helpers.py` & `elevenlabslib-0.5.2/elevenlabslib/helpers.py`

 * *Files 5% similar despite different names*

```diff
@@ -94,19 +94,22 @@
         soundfile is used for the conversion, so it supports any format it does.
 
         Parameters:
             audioData: The audio data.
             saveLocation: The path (or file-like object) where the data will be saved.
             outputFormat: The format in which the audio will be saved
         """
+    tempSoundFile = soundfile.SoundFile(io.BytesIO(audioData))
 
     if isinstance(saveLocation, str):
-        saveLocation = open(saveLocation, "wb")
-    tempSoundFile = soundfile.SoundFile(io.BytesIO(audioData))
-    sf.write(saveLocation, tempSoundFile.read(), tempSoundFile.samplerate, format=outputFormat)
+        with open(saveLocation, "wb") as fp:
+            sf.write(fp, tempSoundFile.read(), tempSoundFile.samplerate, format=outputFormat)
+    else:
+        sf.write(saveLocation, tempSoundFile.read(), tempSoundFile.samplerate, format=outputFormat)
+        saveLocation.flush()
 
 #This class just helps with the callback stuff.
 class _SDPlaybackWrapper:
     def __init__(self, audioData, deviceID, onPlaybackStart:Callable=lambda: None, onPlaybackEnd:Callable=lambda: None):
         soundFile = sf.SoundFile(io.BytesIO(audioData))
         soundFile.seek(0)
         self.onPlaybackStart = onPlaybackStart
```

### Comparing `elevenlabslib-0.5.1/elevenlabslib.egg-info/PKG-INFO` & `elevenlabslib-0.5.2/elevenlabslib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elevenlabslib
-Version: 0.5.1
+Version: 0.5.2
 Summary: Complete python wrapper for the elevenlabs API
 Author-email: lugia19 <lugia19@lugia19.com>
 Project-URL: Documentation, https://elevenlabslib.readthedocs.io/en/latest/
 Project-URL: Homepage, https://github.com/lugia19/elevenlabslib
 Project-URL: Bug Tracker, https://github.com/lugia19/elevenlabslib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `elevenlabslib-0.5.1/pyproject.toml` & `elevenlabslib-0.5.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [build-system]
 requires = ["setuptools>=61.0",
             "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "elevenlabslib"
-version = "0.5.1"
+version = "0.5.2"
 authors = [
   { name="lugia19", email="lugia19@lugia19.com" },
 ]
 description = "Complete python wrapper for the elevenlabs API"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies=[
     "requests",
     "typing",
     "sounddevice",
     "numpy",
-    "soundfile"
+    "soundfile >= 0.12.1"
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Development Status :: 3 - Alpha"
 ]
```

