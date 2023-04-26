# Comparing `tmp/elevenlabs-0.2.6.tar.gz` & `tmp/elevenlabs-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elevenlabs-0.2.6.tar", last modified: Tue Apr 25 07:02:45 2023, max compression
+gzip compressed data, was "elevenlabs-0.2.7.tar", last modified: Tue Apr 25 22:54:36 2023, max compression
```

## Comparing `elevenlabs-0.2.6.tar` & `elevenlabs-0.2.7.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:02:45.953905 elevenlabs-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-25 07:02:45.953905 elevenlabs-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6710 2023-04-25 07:02:34.000000 elevenlabs-0.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:02:45.949905 elevenlabs-0.2.6/elevenlabs/
--rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-04-25 07:02:34.000000 elevenlabs-0.2.6/elevenlabs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:02:45.953905 elevenlabs-0.2.6/elevenlabs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-25 07:02:34.000000 elevenlabs-0.2.6/elevenlabs/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-25 07:02:34.000000 elevenlabs-0.2.6/elevenlabs/api/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-25 07:02:34.000000 elevenlabs-0.2.6/elevenlabs/api/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-25 07:02:34.000000 elevenlabs-0.2.6/elevenlabs/api/tts.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-25 07:02:34.000000 elevenlabs-0.2.6/elevenlabs/api/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-04-25 07:02:34.000000 elevenlabs-0.2.6/elevenlabs/api/voice.py
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-04-25 07:02:34.000000 elevenlabs-0.2.6/elevenlabs/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:02:45.953905 elevenlabs-0.2.6/elevenlabs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-25 07:02:45.000000 elevenlabs-0.2.6/elevenlabs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-25 07:02:45.000000 elevenlabs-0.2.6/elevenlabs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 07:02:45.000000 elevenlabs-0.2.6/elevenlabs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-25 07:02:45.000000 elevenlabs-0.2.6/elevenlabs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-25 07:02:45.000000 elevenlabs-0.2.6/elevenlabs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 07:02:45.953905 elevenlabs-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-25 07:02:34.000000 elevenlabs-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:54:36.109975 elevenlabs-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-25 22:54:36.109975 elevenlabs-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6710 2023-04-25 22:54:21.000000 elevenlabs-0.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:54:36.109975 elevenlabs-0.2.7/elevenlabs/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-25 22:54:21.000000 elevenlabs-0.2.7/elevenlabs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:54:36.109975 elevenlabs-0.2.7/elevenlabs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-25 22:54:21.000000 elevenlabs-0.2.7/elevenlabs/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-04-25 22:54:21.000000 elevenlabs-0.2.7/elevenlabs/api/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-25 22:54:21.000000 elevenlabs-0.2.7/elevenlabs/api/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-25 22:54:21.000000 elevenlabs-0.2.7/elevenlabs/api/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-25 22:54:21.000000 elevenlabs-0.2.7/elevenlabs/api/tts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-25 22:54:21.000000 elevenlabs-0.2.7/elevenlabs/api/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-04-25 22:54:21.000000 elevenlabs-0.2.7/elevenlabs/api/voice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-04-25 22:54:21.000000 elevenlabs-0.2.7/elevenlabs/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-04-25 22:54:21.000000 elevenlabs-0.2.7/elevenlabs/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:54:36.109975 elevenlabs-0.2.7/elevenlabs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-25 22:54:36.000000 elevenlabs-0.2.7/elevenlabs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-25 22:54:36.000000 elevenlabs-0.2.7/elevenlabs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 22:54:36.000000 elevenlabs-0.2.7/elevenlabs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-25 22:54:36.000000 elevenlabs-0.2.7/elevenlabs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-25 22:54:36.000000 elevenlabs-0.2.7/elevenlabs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 22:54:36.109975 elevenlabs-0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-25 22:54:21.000000 elevenlabs-0.2.7/setup.py
```

### Comparing `elevenlabs-0.2.6/PKG-INFO` & `elevenlabs-0.2.7/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elevenlabs
-Version: 0.2.6
+Version: 0.2.7
 Summary: The official elevenlabs python package.
 Home-page: https://github.com/elevenlabs/elevenlabs-python
 Author: Elevenlabs
 Keywords: artificial intelligence,deep learning
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `elevenlabs-0.2.6/README.md` & `elevenlabs-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `elevenlabs-0.2.6/elevenlabs/__init__.py` & `elevenlabs-0.2.7/elevenlabs/simple.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import os
 import re
-import wave
 from collections.abc import Iterator
 from typing import List, Optional, Union
 
 from .api import TTS, Voice, VoiceClone, Voices, VoiceSettings
-from .utils import *  # noqa F403
 
 
 def set_api_key(api_key: str) -> None:
     os.environ["ELEVEN_API_KEY"] = api_key
 
 
 def get_api_key() -> Optional[str]:
```

### Comparing `elevenlabs-0.2.6/elevenlabs/api/base.py` & `elevenlabs-0.2.7/elevenlabs/api/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,60 @@
 import os
 from typing import Optional
 
 import requests  # type: ignore
 from pydantic import BaseModel
 
+from .error import (
+    APIError,
+    AuthorizationError,
+    HTTPError,
+    RateLimitError,
+    UnauthenticatedRateLimitError,
+)
+
 api_base_url_v1 = "https://api.elevenlabs.io/v1"
 
 
 class API(BaseModel):
     class Config:
         # Parse enum to strings when converting to dict
         use_enum_values = True
         # Validate fields when setting manually
         validate_assignment = True
 
     @staticmethod
     def request(url: str, method: str, api_key: Optional[str] = None, **kwargs):
-        headers = {"xi-api-key": api_key or os.environ.get("ELEVEN_API_KEY")}
+        api_key = api_key or os.environ.get("ELEVEN_API_KEY")
+        headers = {"xi-api-key": api_key}
 
         if method == "get":
             response = requests.get(url, headers=headers, **kwargs)
         elif method == "post":
             response = requests.post(url, headers=headers, **kwargs)
         else:
             raise ValueError(f"Invalid request method {method}")
 
-        if response.status_code == 401:
-            raise SystemExit(
-                "Your quota is exceeded or your API key is invalid, please set a"
-                " valid key: ELEVEN_API_KEY"
-            )
-
-        try:
-            response.raise_for_status()
-        except Exception as e:
-            raise type(e)(response.reason, response.text)
-        return response
+        status_code = response.status_code
+
+        if status_code == 200:
+            return response
+
+        error = HTTPError(response)
+
+        if status_code == 401:
+            if error.status == "quota_exceeded":
+                if api_key is None:
+                    raise UnauthenticatedRateLimitError(error)
+                else:
+                    raise RateLimitError(error)
+            elif error.status == "needs_authorization":
+                raise AuthorizationError(error)
+
+        raise APIError(error)
 
     @staticmethod
     def get(url: str, *args, **kwargs):
         return API.request(url, method="get", *args, **kwargs)  # type: ignore
 
     @staticmethod
     def post(url: str, *args, **kwargs):
```

### Comparing `elevenlabs-0.2.6/elevenlabs/api/history.py` & `elevenlabs-0.2.7/elevenlabs/api/history.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-0.2.6/elevenlabs/api/tts.py` & `elevenlabs-0.2.7/elevenlabs/api/tts.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-0.2.6/elevenlabs/api/voice.py` & `elevenlabs-0.2.7/elevenlabs/api/voice.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 from __future__ import annotations
 
-from enum import Enum
 from pathlib import Path
 from typing import List, Optional, Tuple
 
 from pydantic import Field, root_validator, validator
 
 from .base import API, api_base_url_v1
+from .error import APIError
+
+
+class UnauthorizedVoiceCloningError(APIError):
+    pass
 
 
 class VoiceSettings(API):
     stability: float = Field(..., ge=0.0, le=1.0)
     similarity_boost: float = Field(..., ge=0.0, le=1.0)
 
 
@@ -46,50 +50,28 @@
     @classmethod
     def from_clone(cls, voice_clone: VoiceClone) -> Voice:
         url = f"{api_base_url_v1}/voices/add"
         data = voice_clone.dict()
         data["lables"] = str(data.pop("labels"))
         del data["files"]
         files = data.pop("_files_tuple")
-        voice_id = API.post(url, data=data, files=files).json()["voice_id"]
-        return cls.from_id(voice_id)
+        try:
+            voice_id = API.post(url, data=data, files=files).json()["voice_id"]
+        except APIError as e:
+            if e.http_error.status == "can_not_use_instant_voice_cloning":
+                raise UnauthorizedVoiceCloningError(e.http_error)
+            raise
+        return voice_id
 
     @validator("settings")
     def computed_settings(cls, v: VoiceSettings, values) -> VoiceSettings:
         url = f"{api_base_url_v1}/voices/{values['voice_id']}/settings"
         return v if v else VoiceSettings(**cls.get(url).json())
 
 
-class Gender(str, Enum):
-    female = "female"
-    male = "male"
-
-
-class Accent(str, Enum):
-    british = "british"
-    american = "american"
-    african = "african"
-    australian = "australian"
-    indian = "indian"
-
-
-class Age(str, Enum):
-    young = "young"
-    middle_aged = "middle_aged"
-    old = "old"
-
-
-class VoiceDesign(API):
-    text: str = Field(..., max_length=100)
-    gender: Gender
-    accent: Accent
-    accent_strength: float = Field(..., gt=0.3, lt=2.0)
-    age: Age
-
-
 class Voices(API):
     voices: List[Voice]
 
     @classmethod
     def from_api(cls):
         url = f"{api_base_url_v1}/voices"
         response = cls.get(url).json()
```

### Comparing `elevenlabs-0.2.6/elevenlabs/utils.py` & `elevenlabs-0.2.7/elevenlabs/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import os
 import shutil
 import subprocess
 from collections.abc import Iterator
 from pathlib import Path
 
-from IPython.display import Audio, display
-
 
 def is_installed(lib_name: str) -> bool:
     lib = shutil.which(lib_name)
     if lib is None:
         return False
     global_path = Path(lib)
     # else check if path is valid and has the correct access rights
     return global_path.exists() and os.access(global_path, os.X_OK)
 
 
 def play(audio: bytes, notebook: bool = False) -> None:
     if notebook:
+        from IPython.display import Audio, display
+
         display(Audio(audio, rate=44100, autoplay=True))
     else:
         if not is_installed("ffplay"):
             raise ValueError("ffplay from ffmpeg not found, necessary to play audio.")
         args = ["ffplay", "-autoexit", "-", "-nodisp"]
         proc = subprocess.Popen(
             args=args,
```

### Comparing `elevenlabs-0.2.6/elevenlabs.egg-info/PKG-INFO` & `elevenlabs-0.2.7/elevenlabs.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elevenlabs
-Version: 0.2.6
+Version: 0.2.7
 Summary: The official elevenlabs python package.
 Home-page: https://github.com/elevenlabs/elevenlabs-python
 Author: Elevenlabs
 Keywords: artificial intelligence,deep learning
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `elevenlabs-0.2.6/setup.py` & `elevenlabs-0.2.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 from setuptools import find_packages, setup
 
 setup(
     name="elevenlabs",
     packages=find_packages(exclude=[]),
-    version="0.2.6",
+    version="0.2.7",
     description="The official elevenlabs python package.",
     long_description_content_type="text/markdown",
     author="Elevenlabs",
     url="https://github.com/elevenlabs/elevenlabs-python",
     keywords=["artificial intelligence", "deep learning"],
-    install_requires=["pydantic>=1.10", "ipython>=7.0"],
+    install_requires=[
+        "pydantic>=1.10",
+        "ipython>=7.0",
+        "requests>=2.20",
+    ],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.6",
     ],
```

